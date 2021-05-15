
# Table of Contents

-   [related](#rltd) [[infra]] [[linkrot]]
-   [\* why?](#why) 
    -   [motivation: If I do it, I would be able to search on all pages I ever visited](#mtvtnfdtwldbbltsrchnllpgsvrvstd) [[search]] [[memex]]
    -   [Archiving-URLs - Gwern.net](#rchvngrlsgwrnnt) 
        -   [`[2018-11-05]` just backup everything you can find in promnesia?](#jstbckpvrythngycnfndnprmns) [[promnesia]]
-   [\* archivebox](#rchvbx) [[archivebox]]
    -   [ok, first instapaper run](#kfrstnstpprrn) 
    -   [issues](#sss) 
        -   [hmm wonder how did it manage to do user mapping??? is 1000 just dome default docker thing?](#hmmwndrhwddtmngtdsrmppngsjstdmdfltdckrthng) 
        -   [suggest to use `run --rm`](#sggsttsrnrm) 
        -   [crap, timestamps, not shas are used&#x2026; again??](#crptmstmpsntshsrsdgn) 
        -   [ok, need to multithread..](#kndtmltthrd) 
        -   [add command &#x2013; set maximum limit for data transferred?](#ddcmmndstmxmmlmtfrdttrnsfrrd) 
        -   [prune command &#x2013; I think I had some scripts already&#x2026;](#prncmmndthnkhdsmscrptslrdy) 
        -   [index web interface &#x2013; might be useful to have size? for detecting largest offenders](#ndxwbntrfcmghtbsflthvszfrdtctnglrgstffndrs) 
        -   [index web interface &#x2013; would be nice to mark sites that errored? Not sure what's the actionable outcome of that though](#ndxwbntrfcwldbnctmrkststhtsrwhtsthctnbltcmfthtthgh) 
        -   [this issue https://github.com/pirate/ArchiveBox/issues/412](#thssssgthbcmprtrchvbxsss) 
        -   [`[2020-08-11]` ok, need to starti without the pdf, screenshot etc&#x2026; takes too long](#kndtstrtwthtthpdfscrnshttctkstlng) 
    -   [`[2020-08-05]` Release Major new ArchiveBox version, with a brand new CLI, UI, and SQLite index · pirate/ArchiveBox](#sgthbcmprtrchvbxrlsstgvrlrndnwclndsqltndxprtrchvbx) 
    -   [trying out the new one](#tryngtthnwn) [[archivebox]]
        -   [`[2020-10-25]` would be nice to have parallel execution or something..](#wldbncthvprlllxctnrsmthng) 
        -   [`[2020-10-25]`  hmm, if archiving is interrupted, how to carry on?  apparently 'archivebox update'?](#hmmfrchvngsntrrptdhwtcrrynpprntlyrchvbxpdt) 
        -   [`[2020-10-25]` media &#x2013; could def download later/in parallel..](#mdclddfdwnldltrnprlll) 
    -   [ok, I think I just want to take promnesia and run it against all non-browser sources](#kthnkjstwntttkprmnsndrntgnstllnnbrwsrsrcs) [[promnesia]]
    -   [bookmark Archiver https://pirate.github.io/bookmark-archiver](#bkmrkrchvrsprtgthbbkmrkrchvr) 
        -   [maybe just feed promnesia database to it??](#mybjstfdprmnsdtbstt) 
        -   [right, so just archive redoes the index? Should run in against wereyouhere I suppose&#x2026;](#rghtsjstrchvrdsthndxshldrnngnstwryhrspps) 
        -   [commit my changes to archiver, maybe even add the scripts?](#cmmtmychngstrchvrmybvnddthscrpts) 
        -   [figure out 404 etc](#fgrttc) 
        -   [`[2019-04-06]` should run it after I normalise all the wereyouhere links?](#shldrntftrnrmlsllthwryhrlnks) 
        -   [`[2019-04-16]` ok, he's working on django backend where we can use hashes  https://github.com/pirate/ArchiveBox/issues/74](#khswrkngndjngbckndwhrwcnshshssgthbcmprtrchvbxsss) 
    -   [I guess some sites (with comments) &#x2013; useful to update regularly, but most are okay with one snapshot?](#gsssmstswthcmmntssfltpdtrglrlybtmstrkywthnsnpsht) 
    -   [status command is kinda similar to my old blame script? (might be on a branch)](#sttscmmndskndsmlrtmyldblmscrptmghtbnbrnch) 
    -   [only save mp3 for youtube videos? I guess it should be selective&#x2026; or maybe dpeend on number of views](#nlysvmpfrytbvdsgsstshldbslctvrmybdpndnnmbrfvws) 
    -   [wonder if my exporters could be useful for archivebox](#wndrfmyxprtrscldbsflfrrchvbx) [[orger]] [[promnesia]]
    -   [`[2019-04-16]` pirate/ArchiveBox: 🗃 The open source self-hosted web archive. Takes browser history/bookmarks/Pocket/Pinboard/etc., saves HTML, JS, PDFs, media, and more&#x2026;](#prtrchvbxthpnsrcslfhstdwbnbrdtcsvshtmljspdfsmdndmr) 
    -   [`[2019-04-16]` pirate/ArchiveBox: 🗃 The open source self-hosted web archive. Takes browser history/bookmarks/Pocket/Pinboard/etc., saves HTML, JS, PDFs, media, and more&#x2026;](#prtrchvbxthpnsrcslfhstdwbnbrdtcsvshtmljspdfsmdndmr) 
    -   [`[2019-04-16]` [pirate/ArchiveBox] Bugfixes, new data integrity and invariant checks, remove title prefetching](#prtrchvbxbgfxsnwdtntgrtyndnvrntchcksrmvttlprftchng) 
    -   [backup config?](#bckpcnfg) 
-   [prioritise never bookmarked over bookmarked with errors](#prrtsnvrbkmrkdvrbkmrkdwthrrrs) 
    -   [commit it??](#cmmtt) 
-   [some links are pretty crazy&#x2026; maybe prune huge pages manually and ignore](#smlnksrprttycrzymybprnhgpgsmnllyndgnr) 
-   [`[2018-10-03]` kanishka-linux/reminiscence: Self-Hosted Bookmark And Archive Manager](#knshklnxrmnscncslfhstdbkmrkndrchvmngr) 
    -   [`[2018-10-05]` wonder how is it different from my bookmark archiver?](#wndrhwstdffrntfrmmybkmrkrchvr) 
-   [https://github.com/webrecorder/webrecorder](#sgthbcmwbrcrdrwbrcrdr) [[webarchive]]
-   [Tweet from @gwern](#twtfrmgwrn) [[linkrot]]
-   [`[2019-12-20]` Web Archiving Community · pirate/ArchiveBox Wiki](#wbrchvngcmmntyprtrchvbxwk) [[linkrot]]
-   [`[2019-12-11]` Verizon/Yahoo Blocking Attempts to Archive Yahoo Groups – Deletion: Dec. 14 | Hacker News](#vrznyhblckngttmptstrchvyhgrpsdltndchckrnws) 
-   [`[2020-05-28]` site-deaths - IndieWeb](#sndwbrgstdthsstdthsndwb) [[linkrot]]
-   [`[2019-04-19]` Bret Victor on Twitter: "60% of my fav links from 10 yrs ago are 404. I wonder if Library of Congress expects 60% of their collection to go up in smoke every decade."](#brtvctrntwttrfmyfvlnksfrmtsfthrcllctntgpnsmkvrydcd) [[linkrot]]
-   [`[2019-06-13]` Time Travel: Find Mementos in Internet Archive, Archive-It, British Library, archive.today, GitHub and many more! http://timetravel.mementoweb.org/](#tmtrvlfndmmntsnntrntrchvrgthbndmnymrtmtrvlmmntwbrg) [[search]] [[linkrot]]
-   [`[2019-12-22]` This Page is Designed to Last](#snwsycmbntrcmtmdthspgsdsgndtlst) [[linkrot]]
-   [`[2019-07-08]` Fund: On-Demand Web Archiving of Annotated Pages – Hypothesis https://web.hypothes.is/blog/fund-on-demand-web-archiving-of-annotated-pages/](#fndndmndwbrchvngfnnttdpgsfndndmndwbrchvngfnnttdpgs) [[linkrot]]
-   [`[2020-03-06]` Archiving URLs | Hacker News https://news.ycombinator.com/item?id=6504331](#rchvngrlshckrnwssnwsycmbntrcmtmd) 
-   [`[2021-02-25]` Wikipedia:Database download - Wikipedia](#snwkpdrgwkwkpddtbsdwnldwkpddtbsdwnldwkpd) [[wikipedia]]
-   [ugh. image preservation is a mess&#x2026;](#ghmgprsrvtnsmss) [[wikipedia]] [[webarchive]]
-   [`[2021-02-25]` Wikipedia:Database download - Wikipedia](#snwkpdrgwkwkpddtbsdwnldwkpddtbsdwnldwkpd) 
-   [`[2021-02-25]` Main Page - Kiwix](#swkkwxrgwkmnpgmnpgkwx) [[prepping]] [[wikipedia]]
-   [`[2021-02-25]` jeharu comments on The full English Wikipedia on Kiwix now weighs 79Gb instead of 94Gb thanks to improvements in image compression](#swwwrddtcmrdthrdrcmmntskhbthnkstmprvmntsnmgcmprssn) [[kiwix]] [[prepping]]
-   [`[2021-02-25]` Wikipedia:Database download - Wikipedia](#snwkpdrgwkwkpddtbsdwnldwkpddtbsdwnldwkpd) 
-   [would be nice to maybe tag urls&#x2026; e.g. which source they are coming from](#wldbnctmybtgrlsgwhchsrcthyrcmngfrm) [[archivebox]]
-   [def archive things I post (e.g. referenced in my own tweets/comments etc)](#dfrchvthngspstgrfrncdnmywntwtscmmntstc) [[self]] [[archivebox]]
-   [could also check archive.is api?](#cldlschckrchvsp) [[webarchive]]
-   [hmm, a bit confused about archive.is &#x2013; how reliable is it? is it backed up somewhere? perhaps still should save stuff from there locally&#x2026;](#hmmbtcnfsdbtrchvshwrlblststllshldsvstfffrmthrlclly) [[webarchive]]
-   [pdfs on the other hand are a bit of higher priority?](#pdfsnththrhndrbtfhghrprrty) [[webarchive]]
-   [`[2021-03-26]` AdGuardHome/whotracksme.json at master · AdguardTeam/AdGuardHome](#sgthbcmdgrdtmdgrdhmblbmstrcksmjsntmstrdgrdtmdgrdhm) [[archivebox]]





# related       [[infra]] [[linkrot]]




# \* why?





## motivation: If I do it, I would be able to search on all pages I ever visited      [[search]] [[memex]]




## Archiving-URLs - Gwern.net

    The most ambitious & total approach to local caching is to set up a proxy to do your browsing through, and record literally all your web traffic; for example, using Live Archiving Proxy (LAP) or WarcProxy which will save as WARC files every page you visit through it. (Zachary Vance explains how to set up a local HTTPS certificate to MITM your HTTPS browsing as well.)
    
    One may be reluctant to go this far, and prefer something lighter-weight, such as periodically extracting a list of visited URLs from one’s web browser and then attempting to archive them.




### `[2018-11-05]` just backup everything you can find in promnesia?      [[promnesia]]




# \* archivebox      [[archivebox]]

The tool I'm currently using, very decent <https://github.com/ArchiveBox/ArchiveBox#readme>  




## ok, first instapaper run

    [√] 2020-08-11 01:33:33 Update of 252 pages complete (146.68 min)
        - 0 links skipped
        - 228 links updated
        - 24 links had errors
    ...
    535M	./1597100812.87
    609M	./1597100812.31
    757M	./1597100812.221
    1.1G	./1597100812.173
    8.5G	.

Ok, and second run the next day said it's already added all of them to index. Nice!  




## issues 





### hmm wonder how did it manage to do user mapping??? is 1000 just dome default docker thing?




### suggest to use `run --rm`




### crap, timestamps, not shas are used&#x2026; again??




### ok, need to multithread..




### add command &#x2013; set maximum limit for data transferred?




### prune command &#x2013; I think I had some scripts already&#x2026;




### index web interface &#x2013; might be useful to have size? for detecting largest offenders




### index web interface &#x2013; would be nice to mark sites that errored? Not sure what's the actionable outcome of that though




### this issue <https://github.com/pirate/ArchiveBox/issues/412>

-   run archivebox init

-   run some export

-   run another export (potentially overlapping?, but with new urls)

-   it seems to fail&#x2026;




### `[2020-08-11]` ok, need to starti without the pdf, screenshot etc&#x2026; takes too long

also make sure it's possibe to add pdfs as an afterthought?  




## `[2020-08-05]` [Release Major new ArchiveBox version, with a brand new CLI, UI, and SQLite index · pirate/ArchiveBox](https://github.com/pirate/ArchiveBox/releases/tag/v0.4.9)

    Major new ArchiveBox version, with a brand new CLI, UI, and SQLite index




## trying out the new one      [[archivebox]]

-   how does it retrieve images?
-   singlefile vs wget &#x2013; not sure?? singlefile is nice though
-   mercury??? apparently not documented yet, but same as readability?
-   readability is pretty neat &#x2013; also contains images (as base64)
-   warc??
-   hmm, DOM is probably HTML??




### `[2020-10-25]` would be nice to have parallel execution or something..




### `[2020-10-25]`  hmm, if archiving is interrupted, how to carry on?  apparently 'archivebox update'?


-   `[2020-10-25]` ok, it fetches new data on config change when running update? that's nice




### `[2020-10-25]` media &#x2013; could def download later/in parallel..




## ok, I think I just want to take promnesia and run it against all non-browser sources      [[promnesia]]

would be nice to mark different sources as well if possible?  




## bookmark Archiver <https://pirate.github.io/bookmark-archiver>





### maybe just feed promnesia database to it??


-   I guess need promnesia  provider. is it like my.links?      [[hpi]]

-   move run script somewhere else; add ability to put output dir somewhere else




### right, so just archive redoes the index? Should run in against wereyouhere I suppose&#x2026;




### commit my changes to archiver, maybe even add the scripts?




### figure out 404 etc




### `[2019-04-06]` should run it after I normalise all the wereyouhere links?

I guess filter out all suspicious ones, containing special characters?  




### `[2019-04-16]` ok, he's working on django backend where we can use hashes  <https://github.com/pirate/ArchiveBox/issues/74>




## I guess some sites (with comments) &#x2013; useful to update regularly, but most are okay with one snapshot?




## status command is kinda similar to my old blame script? (might be on a branch)




## only save mp3 for youtube videos? I guess it should be selective&#x2026; or maybe dpeend on number of views




## wonder if my exporters could be useful for archivebox      [[orger]] [[promnesia]]




## `[2019-04-16]` pirate/ArchiveBox: 🗃 The open source self-hosted web archive. Takes browser history/bookmarks/Pocket/Pinboard/etc., saves HTML, JS, PDFs, media, and more&#x2026;

<https://github.com/pirate/ArchiveBox/>  

    Storage Requirements
    Because ArchiveBox is designed to ingest a firehose of browser history and bookmark feeds to a local disk, it can be much more disk-space intensive than a centralized service like the Internet Archive or Archive.today. However, as storage space gets cheaper and compression improves, you should be able to use it continuously over the years without having to delete anything. In my experience, ArchiveBox uses about 5gb per 1000 articles, but your milage may vary depending on which options you have enabled and what types of sites you're archiving. By default, it archives everything in as many formats as possible, meaning it takes more space than a using a single method, but more content is accurately replayable over extended periods of time. Storage requirements can be reduced by using a compressed/deduplicated filesystem like ZFS/BTRFS, or by setting FETCH_MEDIA=False to skip audio & video files.




## `[2019-04-16]` pirate/ArchiveBox: 🗃 The open source self-hosted web archive. Takes browser history/bookmarks/Pocket/Pinboard/etc., saves HTML, JS, PDFs, media, and more&#x2026;

<https://github.com/pirate/ArchiveBox/>  

    Support for saving multiple snapshots of each site over time will be added soon (along with the ability to view diffs of the changes between runs).




## `[2019-04-16]` [pirate/ArchiveBox] Bugfixes, new data integrity and invariant checks, remove title prefetching

    re-save index after archiving completes to update titles and urls
    emove title prefetching in favor of new FETCH_TITLE archive method




## backup config?




# prioritise never bookmarked over bookmarked with errors





## commit it??




# some links are pretty crazy&#x2026; maybe prune huge pages manually and ignore

e.g. wget -N -E -np -x -H -k -K -S &#x2013;restrict-file-names=unix -p &#x2013;user-agent=Bookmark Archiver &#x2013;no-check-certificate <https://charlie-charlie.ru/breakfast>  
&#x2013; about 150M  




# `[2018-10-03]` kanishka-linux/reminiscence: Self-Hosted Bookmark And Archive Manager

<https://github.com/kanishka-linux/reminiscence>  




## `[2018-10-05]` wonder how is it different from my bookmark archiver?




# <https://github.com/webrecorder/webrecorder>       [[webarchive]]




# Tweet from @gwern      [[linkrot]]

<https://twitter.com/gwern/status/1233112807253716992>  

@gwern: @karlicoss @thomas536 Not documented in there yet is my latest archiving tool: <https://t.co/If2Ypw1T1M> <https://t.co/NLh23nrkrh> Currently costs 20GB for 7,677 PDFs & self-contained single-file HTML mirrors.  




# `[2019-12-20]` Web Archiving Community · pirate/ArchiveBox Wiki      [[linkrot]]

<https://github.com/pirate/ArchiveBox/wiki/Web-Archiving-Community>  




# `[2019-12-11]` Verizon/Yahoo Blocking Attempts to Archive Yahoo Groups – Deletion: Dec. 14 | Hacker News

<https://news.ycombinator.com/item?id=21737696>  

    ven if we still had the Library of Alexandria, it may have shed zero light on the actual lives of citizens. Archiving content on the internet means capturing thousands of individual level perspectives and experiences. We don't know what will end up being important to historians 50 or 100 years from now. I would bet there are dozens if not hundreds of historians that would give anything for a record of their favorite time period that contains even a fraction of the amount of content today's archive efforts are storing.




# `[2020-05-28]` [site-deaths - IndieWeb](https://indieweb.org/site-deaths)      [[linkrot]]




# `[2019-04-19]` Bret Victor on Twitter: "60% of my fav links from 10 yrs ago are 404. I wonder if Library of Congress expects 60% of their collection to go up in smoke every decade."      [[linkrot]]

<https://twitter.com/worrydream/status/478087637031325697>  




# `[2019-06-13]` Time Travel: Find Mementos in Internet Archive, Archive-It, British Library, archive.today, GitHub and many more! <http://timetravel.mementoweb.org/>      [[search]] [[linkrot]]




# `[2019-12-22]` [This Page is Designed to Last](https://news.ycombinator.com/item?id=21840140)      [[linkrot]]

<https://jeffhuang.com/designed_to_last/>  




# `[2019-07-08]` Fund: On-Demand Web Archiving of Annotated Pages – Hypothesis <https://web.hypothes.is/blog/fund-on-demand-web-archiving-of-annotated-pages/>      [[linkrot]]




# `[2020-03-06]` Archiving URLs | Hacker News <https://news.ycombinator.com/item?id=6504331>




# `[2021-02-25]` [Wikipedia:Database download - Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:Database_download)      [[wikipedia]]

    pages-articles-multistream.xml.bz2 – Current revisions only, no talk or user pages; this is probably what you want, and is approximately 18 GB compressed (expands to over 78 GB when decompressed).




# ugh. image preservation is a mess&#x2026;      [[wikipedia]] [[webarchive]]




# `[2021-02-25]` [Wikipedia:Database download - Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:Database_download)

    pages-articles.xml.bz2 and pages-articles-multistream.xml.bz2 both contain the same xml contents. So if you unpack either, you get the same data. But with multistream, it is possible to get an article from the archive without unpacking the whole thing.




# `[2021-02-25]` [Main Page - Kiwix](https://wiki.kiwix.org/wiki/Main_Page)      [[prepping]] [[wikipedia]]




# `[2021-02-25]` [jeharu comments on The full English Wikipedia on Kiwix now weighs 79Gb instead of 94Gb thanks to improvements in image compression](https://www.reddit.com/r/DataHoarder/comments/khjv59/the_full_english_wikipedia_on_kiwix_now_weighs/ggm8ijt/)      [[kiwix]] [[prepping]]

    [–]jeharu54TB 46 points 2 months ago
    no support yet for incremental updating, right? bummer.
    
        permalinkembedsavereportgive awardreply
    [–]The_other_kiwix_guy[S] 66 points 2 months ago
    We've started working on a prototype but that'll take time and a lot more money than we have. Would not expect anything before another 2-3 years.

hm okay sad.. guess I can do a backup per year or smth for now  




# `[2021-02-25]` [Wikipedia:Database download - Wikipedia](https://en.wikipedia.org/wiki/Wikipedia:Database_download)

    The only downside to multistream is that it is marginally larger




# would be nice to maybe tag urls&#x2026; e.g. which source they are coming from      [[archivebox]]

or just have a special source for manual notes/exobrainy stuff and another one for the rest?  
<https://github.com/ArchiveBox/ArchiveBox/issues/660>  




# def archive things I post (e.g. referenced in my own tweets/comments etc)      [[self]] [[archivebox]]




# could also check archive.is api?      [[webarchive]]

e.g. it archives medium-like stuff? <https://archive.is/20181031123930/https://howwegettonext.com/exploring-the-future-without-cyberpunks-neon-and-noir-8e23562819e3>  




# hmm, a bit confused about archive.is &#x2013; how reliable is it? is it backed up somewhere? perhaps still should save stuff from there locally&#x2026;      [[webarchive]]




# pdfs on the other hand are a bit of higher priority?      [[webarchive]]




# `[2021-03-26]` [AdGuardHome/whotracksme.json at master · AdguardTeam/AdGuardHome](https://github.com/AdguardTeam/AdGuardHome/blob/master/client/src/helpers/trackers/whotracksme.json)      [[archivebox]]

could use this to prune?  

