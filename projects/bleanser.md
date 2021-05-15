
# Table of Contents

-   [related](#rltd) [[exports]] [[backup]] [[infra]]
-   [\* motivation](#mtvtn) 
    -   [reddit processing takes quite a bit.. but I guess bleanser will optimize it](#rddtprcssngtksqtbtbtgssblnsrwllptmzt) [[hpi]] [[bleanser]] [[reddit]]
-   [\* ideas](#ds) 
    -   [pattern of handling unknown data sources](#pttrnfhndlngnknwndtsrcs) [[toblog]]
-   [\* specific data sources](#spcfcdtsrcs) 
    -   [firefox history?](#frfxhstry) [[promnesia]] [[bleanser]]
    -   [github-events &#x2013; prune via triplet approach?](#gthbvntsprnvtrpltpprch) 
    -   [xml: smscalls](#xmlsmsclls) 
    -   [not sure, maybe ignore comment/link karma? it results in lots of differences&#x2026;](#ntsrmybgnrcmmntlnkkrmtrsltsnltsfdffrncs) [[reddit]]
-   [\* bugs](#bgs) 
    -   [shit, dry run still left turds???](#shtdryrnstlllfttrds) 
-   [compress backups?](#cmprssbckps) [[infra]]
    -   [`[2019-03-25]` also compressing rtm](#lscmprssngrtm) 
-   [`[2021-01-11]` move description to github](#mvdscrptntgthb) 
-   [-----------------------------------](#3456_3534) 
-   [generic sqlite databases export](#gnrcsqltdtbssxprt) [[bleanser]]
-   [hmm. they serve sort of the same purpose???](#hmmthysrvsrtfthsmprps) [[bleanser]] [[backupchecker]]
-   [maybe 'dynamic' optimizer for bleanser? and later can use it to actually delete stuff](#mybdynmcptmzrfrblnsrndltrcnsttctllydltstff) [[hpi]]
    -   [`[2021-03-02]` I guess HPI could import it as a dependency..](#gsshpcldmprttsdpndncy) 
-   [github events via triples would be a good example](#gthbvntsvtrplswldbgdxmpl) [[bleanser]]
-   [`[2021-03-02]` Search results · PyPI](#spyprgsrchqprnysrchrsltspyp) [[bleanser]]
-   [`[2021-02-27]` trailofbits/graphtage: A semantic diff utility and library for tree-like files such as JSON, JSON5, XML, HTML, YAML, and CSV.](#sgthbcmtrlfbtsgrphtgtrlfbschsjsnjsnxmlhtmlymlndcsv) [[bleanser]]
-   [ok, triples for browser history are def gonna be impactful](#ktrplsfrbrwsrhstryrdfgnnbmpctfl) [[bleanser]]
-   [`[2021-04-07]` Memory Filesystem — PyFilesystem 2.4.13 documentation](#sdcspyflsystmrgnltstrfrncryflsystmpyflsystmdcmnttn) [[bleanser]]
-   [warn about being disk/tmp intense?](#wrnbtbngdsktmpntns) [[bleanser]]
-   [write about multiprocessing?](#wrtbtmltprcssng) [[bleanser]]
-   ['extract' query](#xtrctqry) [[bleanser]]
-   [hmm, for attributes that can change back and force in json, sorted strategy isn't the best&#x2026; ugh](#hmmfrttrbtsthtcnchngbckndcnjsnsrtdstrtgysntthbstgh) [[bleanser]]
-   [sqlite: hmm&#x2026;.note sure about cascades&#x2026; probably need to disable somehow?](#sqlthmmntsrbtcscdsprbblyndtdsblsmhw) [[bleanser]]
-   [investigating diffs](#nvstgtngdffs) [[bleanser]]
-   [for properly impressive demo should prob run in single threaded mode?](#frprprlymprssvdmshldprbrnnsnglthrddmd) [[bleanser]]
-   [run tox first? to protect from crashes](#rntxfrsttprtctfrmcrshs) [[bleanser]] [[setup]]
-   [could artificially map jsons to line-based format (with full path to the entity?)](#cldrtfcllympjsnstlnbsdfrmtwthfllpthtthntty) [[bleanser]]
-   [kinds of snapshots](#kndsfsnpshts) [[toblog]] [[bleanser]]
-   [moving old files &#x2013; not sure what to do about empty dirs?](#mvngldflsntsrwhttdbtmptydrs) [[bleanser]]
-   [implement 'extract' mode later&#x2026; after writing to blog definitely](#mplmntxtrctmdltrftrwrtngtblgdfntly) [[bleanser]]
-   [readme: gotcha about group boundaries not being removed (nad having empty diff)](#rdmgtchbtgrpbndrsntbngrmvdndhvngmptydff) [[bleanser]]
-   [document what's happening in which case&#x2026; with a literate test](#dcmntwhtshppnngnwhchcswthltrttst) [[bleanser]]
-   [proper end2end test &#x2014; could  run against firefox? reinstalled at about 202006, could track by file size changes](#prprndndtstcldrngnstfrfxrtlldtbtcldtrckbyflszchngs) [[bleanser]]
-   [multiway is a bit more speculative](#mltwysbtmrspcltv) [[bleanser]] [[toblog]]
-   [add for takeouts&#x2026; I even had some script to compare it somewhere](#ddfrtktsvnhdsmscrpttcmprtsmwhr) [[bleanser]]
-   [hypothesis, endomondo, pinboard &#x2013; just use regular json processor](#hypthssndmndpnbrdjstsrglrjsnprcssr) [[bleanser]]
-   [old code for 'extract' bit](#ldcdfrxtrctbt) [[bleanser]] [[pinboard]]
-   [json: sorting stuff might definitely make it more confusing when there is just one volatile attribute that has two values](#jsnsrtngstffmghtdfntlymktrsjstnvltlttrbtththstwvls) [[bleanser]]
-   [foursquare is a good motiation &#x2013; lots of random changing crap even without the changes of underlying data?](#frsqrsgdmttnltsfrndmchngnrpvnwthtthchngsfndrlyngdt) [[bleanser]]

Github page: [karlicoss/bleanser](https://github.com/karlicoss/bleanser)  

Bleanser' stands for 'backup cleanser'.  

The idea is figuring out 'redundant' backups and removing them to  

-   save on disk space
-   same on data access time (see ["data access layer"](https://beepb00p.xyz/exports.html#dal))

This is the most relevant to [incremental/synthetic](https://beepb00p.xyz/exports.html#types) style data exports.  

It's not necessarily hard to implement for something specific, but the challenge is to do it in a data source agnostic way,  
or at least with as minimum effort as possible.  

This is possible for example for JSON: if the export from today is a superset of an export from yesterday, you can safely remove the old export. This actually works surprisingly well as is for many data sources.  
For a few I've got slight adjustments that normalise them before comparing by removing certain fields that change often, but not very important. For example, Reddit upvotes/downvotes always jump, so I just exclude them from the comparison.  
It's similar to extracting the useful fields, but instead it filters the useless ones. That makes it safer in case new fields are added by the backend, I'd rather keep extra data than potentially lose useful information.  




# related       [[exports]] [[backup]] [[infra]]




# \* motivation





## reddit processing takes quite a bit.. but I guess bleanser will optimize it      [[hpi]] [[bleanser]] [[reddit]]




# \* ideas





## pattern of handling unknown data sources      [[toblog]]

lower bound  
  specify data (fields/files etc) to preserve  
if you only do that you might miss new useful data/schema changes like renames etc  

. ideally they meet here  
  .. warn if we ended up here, i.e. dropping is not converting with picking. but keep the data  

if you only do that you end up with too much garbage  
  specify data (fileds/files etc) to drop  
upper bound  




# \* specific data sources





## firefox history?      [[promnesia]] [[bleanser]]




## github-events &#x2013; prune via triplet approach?




## xml: smscalls




## not sure, maybe ignore comment/link karma? it results in lots of differences&#x2026;      [[reddit]]




# \* bugs





## shit, dry run still left turds???




# compress backups?      [[infra]]

started compressing reddit&#x2026;  




## `[2019-03-25]` also compressing rtm




# `[2021-01-11]` move description to github




# ----------------------------------- 




# generic sqlite databases export      [[bleanser]]

-   do not remove; move to killzone
-   get all tables
-   make sure all schemas match
-   maybe convert it to json or something? and then compare jsons&#x2026;
-   checks that entries are dominated?




# hmm. they serve sort of the same purpose???      [[bleanser]] [[backupchecker]]




# maybe 'dynamic' optimizer for bleanser? and later can use it to actually delete stuff      [[hpi]]





## `[2021-03-02]` I guess HPI could import it as a dependency..




# github events via triples would be a good example      [[bleanser]]




# `[2021-03-02]` [Search results · PyPI](https://pypi.org/search/?q=pruny)      [[bleanser]]

could name like this&#x2026;  




# `[2021-02-27]` [trailofbits/graphtage: A semantic diff utility and library for tree-like files such as JSON, JSON5, XML, HTML, YAML, and CSV.](https://github.com/trailofbits/graphtage)      [[bleanser]]




# ok, triples for browser history are def gonna be impactful      [[bleanser]]

maybe before comparison explicitly 'cleanup' stuff  




# `[2021-04-07]` [Memory Filesystem — PyFilesystem 2.4.13 documentation](https://docs.pyfilesystem.org/en/latest/reference/memoryfs.html)      [[bleanser]]

could use for processing&#x2026; maybe via option  




# warn about being disk/tmp intense?      [[bleanser]]




# write about multiprocessing?      [[bleanser]]




# 'extract' query      [[bleanser]]

might be useful as a sanity check? to ensure stuff isn't deleted by accident? (like foreign key triggers)  
e.g.  

-   run extract query first to get a snapshot of data
-   run cleanup query
-   run extract query first to ensure the data we care about is there?




# hmm, for attributes that can change back and force in json, sorted strategy isn't the best&#x2026; ugh      [[bleanser]]




# sqlite: hmm&#x2026;.note sure about cascades&#x2026; probably need to disable somehow?      [[bleanser]]




# investigating diffs      [[bleanser]]

shell globing nice for not typing too much  

    python3 -m bleanser.modules.firefox diff /path/to/database-201906{16,17}*.sqlite | less




# for properly impressive demo should prob run in single threaded mode?      [[bleanser]]




# run tox first? to protect from crashes      [[bleanser]] [[setup]]




# could artificially map jsons to line-based format (with full path to the entity?)      [[bleanser]]

that way might work more reliably&#x2026; hmm  




# kinds of snapshots      [[toblog]] [[bleanser]]

-   append only (e.g. foursquare, hypothesis)
-   rolling (e.g. rescuetime, github, reddit)

either way you can think of it as as set of strings  




# moving old files &#x2013; not sure what to do about empty dirs?      [[bleanser]]

maybe keep all dirs that were there before &#x2013; and only remove new empty dirs?  




# implement 'extract' mode later&#x2026; after writing to blog definitely      [[bleanser]]




# readme: gotcha about group boundaries not being removed (nad having empty diff)      [[bleanser]]




# document what's happening in which case&#x2026; with a literate test      [[bleanser]]

-   e.g. 'all files are same'
-   only added data
-   rolling data (some fake datetime stuff with 30d retention)
-   error in cleaner script




# proper end2end test &#x2014; could  run against firefox? reinstalled at about 202006, could track by file size changes      [[bleanser]]




# multiway is a bit more speculative      [[bleanser]] [[toblog]]




# add for takeouts&#x2026; I even had some script to compare it somewhere      [[bleanser]]




# hypothesis, endomondo, pinboard &#x2013; just use regular json processor      [[bleanser]]




# old code for 'extract' bit      [[bleanser]] [[pinboard]]

     return pipe(
         '.tags  |= .',
         '.posts |= map({href, description, time, tags})', # TODO maybe just delete hash?
         '.notes |= {notes: .notes | map({id, title, updated_at}), count}',  # TODO hhmm, it keeps length but not content?? odd.
    )




# json: sorting stuff might definitely make it more confusing when there is just one volatile attribute that has two values      [[bleanser]]

e.g. on foursquare with isMayor: true &#x2013; hmmm  




# foursquare is a good motiation &#x2013; lots of random changing crap even without the changes of underlying data?      [[bleanser]]

