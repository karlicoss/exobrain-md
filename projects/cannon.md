
# Table of Contents

-   [related](#rltd) 
    -   [promnesia as a primary application (for me)](#prmnssprmrypplctnfrm) [[promnesia]]
    -   [.](#930_1046) [[linkrot]]
-   [\* motivation](#mtvtn) 
    -   [`[2020-04-04]` I want urls that represent information, regardless the way it's presented](#wntrlsthtrprsntnfrmtnrgrdlssthwytsprsntd) 
        -   [`[2020-05-23]` "document equivalence" is a good term: How to establish (or avoid) document equivalence in the Hypothesis system : Hypothesis](#dcmntqvlncsgdtrmswbhypthslncnthhypthsssystmhypthss) 
    -   [why not use "rel=canonical" metadata field?](#whyntsrlcnnclmtdtfld) 
        -   [`[2020-05-27]` Google no longer providing original URL in AMP for image search results](#snwsycmbntrcmtmdgglnlngrpdngrgnlrlnmpfrmgsrchrslts) 
        -   [`[2019-10-11]` mobile versions of sites sometimes have different "canonical", e.g. mobile.twitter.com](#mblvrsnsfstssmtmshvdffrntcnnclgmbltwttrcm) 
        -   [`[2020-05-28]` archive.org is messing with canonical](#rchvrgsmssngwthcnncl) [[cannon]]
        -   [`[2019-11-02]` e.g. this link doesn't have 'canonical' even though it's a mirror: https://solar.lowtechmagazine.com/2016/11/the-curse-of-the-modern-office.html](#gthslnkdsnthvcnnclvnthghtmgzncmthcrsfthmdrnffchtml) 
        -   [`[2019-11-08]` no canonical on gist https://gist.github.com/dneto/2258454](#ncnnclngstsgstgthbcmdnt) 
    -   [`[2019-08-19]` parent and sibling relations can be determined from the URL](#prntndsblngrltnscnbdtrmndfrmthrl) [[cannon]] [[promnesia]]
    -   [`[2019-11-01]` if the original page is gone I can still easily link my saved annotations (Instapaper/Pocket/Hypothesis) to archived page](#fthrgnlpgsgncnstllslylnkmnstpprpckthypthsstrchvdpg) 
    -   [`[2019-09-07]` urls a good candidate to determine 'entities' because they sure at least somewhat curated](#rlsgdcnddttdtrmnnttsbcsthysrtlstsmwhtcrtd) [[cannon]]
    -   [`[2019-02-24]` normalization is tricky.. for some urls, stuff after # is important https://en.wikipedia.org/wiki/Tendon#cite\_note-14 . for some, it's utter garbage](#nrmlztnstrckyfrsmrlsstfffrgwktndnctntfrsmtsttrgrbg) 
    -   [`[2019-08-07]` The Problem With URLs https://blog.codinghorror.com/the-problem-with-urls/](#thprblmwthrlssblgcdnghrrrcmthprblmwthrls) 
    -   [`[2020-01-02]` motivation: siloing: instapaper 'imports' pages and assigns an id: https://www.instapaper.com/read/1265139707](#mtvtnslngnstpprmprtspgsndssgnsndswwwnstpprcmrd) 
    -   [`[2021-03-07]` could normalize historic URLs which are already down?](#cldnrmlzhstrcrlswhchrlrdydwn) [[linkrot]]
-   [\* projects that could benefit from it](#prjctsthtcldbnftfrmt) 
    -   [`[2019-06-27]` Hmm could be helpful for hypothesis?](#hmmcldbhlpflfrhypthss) [[hypothesis]]
        -   [`[2021-01-16]` discuss about cannon (maybe on Slack)?](#dscssbtcnnnmybnslck) [[hypothesis]] [[cannon]]
        -   [`[2019-05-24]` Annotation of content on sites like Facebook or Twitter? - Google Groups](#sgrpsgglcmlsthypthssfrmtpntnstslkfcbkrtwttrgglgrps) [[hypothesis]]
    -   [`[2021-01-30]` Ignore URL parameters - Feature Requests - Memex Community](#scmmntywrldbrntgnrrlprmtrrlprmtrsftrrqstsmmxcmmnty) [[worldbrain]]
    -   [`[2021-01-22]` wonder if we could cooperate?](#wndrfwcldcprt) [[agora]] [[cannon]]
    -   [`[2021-01-24]` would be useful to use the same normalising engine for #archivebox for example?](#wldbsfltsthsmnrmlsngngnfrrchvbxfrxmpl) [[webarchive]]
    -   [`[2021-02-07]` could be useful for surfingkey/nyxt browser to hint 'interesting' urls?](#cldbsflfrsrfngkynyxtbrwsrthntntrstngrls) 
    -   [`[2019-12-26]` archive.org](#rchvrg) [[linkrot]]
    -   [if it's implemented as a helper extension/library, it could be useful for many other extensions](#ftsmplmntdshlprxtnsnlbrrytcldbsflfrmnythrxtnsns) 
    -   [`[2020-12-07]` einaregilsson/Redirector: Browser extension (Firefox, Chrome, Opera, Edge) to redirect urls based on regex patterns, like a client side `mod_rewrite` ](#sgthbcmnrglssnrdrctrnrglsdnrgxpttrnslkclntsdmdrwrt) 
    -   [`[2020-11-20]` could reuse URL underlying etc with ampie?](#cldrsrlndrlyngtcwthmp) [[ampie]]
-   [\* prior art](#prrrt) 
    -   [`[2020-06-30]` ClearURLs / Addon: looks super super promising](#sgthbcmclrrlsddnpplctnclrrlsddnlkssprsprprmsng) 
        -   [`[2021-03-10]` https://github.com/ClearURLs/Addon/wiki/Rules:  Not super convinced JSON would work well in general, but anyway it's already pretty good.](#sgthbcmclrrlsddnwkrlsntsplngnrlbtnywytslrdyprttygd) 
    -   [`[2020-11-22]` WorldBrain/memex-url-utils: Shared URL processing utilities for Memex extension and mobile apps.](#sgthbcmwrldbrnmmxrltlswrlsngtltsfrmmxxtnsnndmblpps) [[worldbrain]]
    -   [`[2019-07-09]` h/uri.py at 0fc8a0d345741d43b4f80856a7cbb8f5afa70f80 · hypothesis/h https://github.com/hypothesis/h/blob/0fc8a0d345741d43b4f80856a7cbb8f5afa70f80/h/util/uri.py](#hrpytfcddbfcbbfffhypthsshhsshblbfcddbfcbbfffhtlrpy) [[hypothesis]]
        -   [`[2019-07-09]` excluded query params!](#xclddqryprms) 
        -   [`[2019-07-09]` right, I could probably reuse hypothesis's canonify and contribute back. looks very similar to mine](#rghtcldprbblyrshypthssscnyndcntrbtbcklksvrysmlrtmn) 
    -   [`[2020-05-12]` coleifer/micawber: a small library for extracting rich content from urls](#sgthbcmclfrmcwbrclfrmcwbrryfrxtrctngrchcntntfrmrls) 
        -   [`[2021-03-10]` ok, pretty interesting. it probably uses network, but could at least use it for testing (or maybe even 'enriching'?)](#kprttyntrstngtprbblyssntwtlststfrtstngrmybvnnrchng) 
    -   [`[2019-03-27]` sindresorhus/compare-urls: Compare URLs by first normalizing them](#sgthbcmsndrsrhscmprrlssndlscmprrlsbyfrstnrmlzngthm) 
        -   [`[2019-12-25]` sindresorhus/normalize-url](#sgthbcmsndrsrhsnrmlzrlsndrsrhsnrmlzrl) 
    -   [`[2019-07-09]` hypothesis: `h/normalize_uris_test.py`](#sgthbcmhypthsshblbfcddbfctstpyhypthsshnrmlzrststpy) 
    -   [`[2019-04-16]` niksite/url-normalize: URL normalization for Python](#sgthbcmnkstrlnrmlznkstrlnrmlzrlnrmlztnfrpythn) 
    -   [`[2020-04-27]` john-kurkowski/tldextract: Accurately separate the TLD from the registered domain and subdomains of a URL, using the Public Suffix List.](#sgthbcmjhnkrkwsktldxtrctjsbdmnsfrlsngthpblcsffxlst) 
    -   [`[2019-03-27]` rbaier/python-urltools: Some functions to parse and normalize URLs.](#sgthbcmrbrpythnrltlsrbrpytlssmfnctnstprsndnrmlzrls) 
-   [\* ideas](#ds) 
    -   [`[2021-03-07]` maybe we can achieve 95% accuracy with generic rules and by handling the most popular websites](#mybwcnchvccrcywthgnrcrlsndbyhndlngthmstpplrwbsts) 
    -   [if 'children' relations can't be determined by substring matching, perhaps cannon should generate 'virtual' urls?](#fchldrnrltnscntbdtrmndbysgprhpscnnnshldgnrtvrtlrls) [[promnesia]] [[cannon]]
    -   [a special service to resolve siloed links like t.co ?](#spclsrvctrslvsldlnkslktc) [[linkrot]]
    -   [just specify admissible regexes for urls so it's easier to unify?](#jstspcfydmssblrgxsfrrlsstssrtnfy) 
        -   [`[2019-11-09]` also this to summarize](#lsthstsmmrz) 
    -   [rethinking the whole approach&#x2026;](#rthnkngthwhlpprch) 
    -   [use shared JS/python tests for canonifying?](#sshrdjspythntstsfrcnnfyng) [[ffi]] [[promnesia]]
    -   [`[2019-09-03]` should be idempotent?](#shldbdmptnt) 
    -   [hmm, maybe the extension can learn normalisation ruls over time? by looking at canonical and refining the rules?](#hmmmybthxtnsncnlrnnrmlstnmbylkngtcnnclndrfnngthrls) 
    -   [sample random links and their canonicals for testing](#smplrndmlnksndthrcnnclsfrtstng) 
    -   [background thing that sucks in canonical urls and provides data for testing?](#bckgrndthngthtscksncnnclrlsndprvdsdtfrtstng) [[promnesia]]
    -   [how do we prune links that are potentially not secure to store? like certain URL parameters](#hwdwprnlnksthtrptntllyntscrtstrlkcrtnrlprmtrs) 
    -   [need checks that url don't contain stupid shit like trailing colons etc](#ndchcksthtrldntcntnstpdshtlktrlngclnstc) 
    -   [hmm could use this api for checking normalization?](#hmmcldsthspfrchckngnrmlztn) [[cannon]]
-   [\* testcases](#tstcss) 
    -   [`[2020-11-15]` Wendover Productions - YouTube](#swwwytbcmcwndvrprdctnsvdswndvrprdctnsytb) 
    -   [`[2020-04-19]` roam links](#rmlnks) 
    -   [`[2021-02-07]` https://app.element.io/#/room/#blockchain:fosdem.org](#spplmntrmblckchnfsdmrg) [[cannon]]
    -   [`[2021-02-16]` A Relational Turn for Data Protection? by Neil M. Richards, Woodrow Hartzog :: SSRN](#spprsssrncmslpprscfmbstrcnbynlmrchrdswdrwhrtzgssrn) [[cannon]]
    -   [`[2019-06-23]` A Brief Intro to Topological Quantum Field Theories. - YouTube https://www.youtube.com/watch?v=59uLGIrkMxM&list=WL&index=61&t=0s](#brfntrttplgclqntmfldthrsybcmwtchvlgrkmxmlstwlndxts) 
    -   [`[2020-11-16]` normalise DOI](#stwttrcmmghjlhlsttsnrmlsd) 
    -   [m.wikipedia normalisation could also be useful for hypothesis?](#mwkpdnrmlstncldlsbsflfrhypthss) [[hypothesis]]
        -   [`[2019-07-23]` X.m.wikipedia.org](#xmwkpdrg) 
        -   [`[2019-07-23]` mm, it's got canonical though..](#mmtsgtcnnclthgh) 
        -   [`[2019-07-23]` perhaps promnesia should respond both to canonical and its own idea of normalised (preferring canonical)](#prhpsprmnsshldrspndbthtcndtswndfnrmlsdprfrrngcnncl) 
    -   [`[2019-04-20]` fragments: Aharonov-Bohm Experiment https://physicstravelguide.com/experiments/aharonov-bohm#tab\_\_concrete](#frgmntshrnvbhmxprmntsphysgdcmxprmntshrnvbhmtbcncrt) 
        -   [`[2019-08-26]` here I guess it could yield url with hash + parent url?](#hrgsstcldyldrlwthhshprntrl) 
        -   [`[2019-08-26]` always assume that parents in uri hierarchy are actual parents? I guess that's fairly reasonable](#lwysssmthtprntsnrhrrchyrctlprntsgssthtsfrlyrsnbl) 
    -   [`[2019-08-25]` stuff like this:  youtu.be/1TKSfAkWWN0](#stfflkthsytbtksfkwwn) 
        -   [`[2019-08-25]` this is also motivation for canonifying. this is a redirect link in tweet, and there is no way to associate it with canonical](#thsslsmtvtnfrcnnfyngthssrwtndthrsnwytsscttwthcnncl) 
    -   [`[2020-05-02]` https://hubs.mozilla.com/#/](#shbsmzllcm) [[cannon]]
    -   [`[2020-04-30]` Writing well | defmacro](#wwwdfmcrrgwrtngwllhtmlwrtngwlldfmcr) 
        -   [`[2020-05-28]` Wayback Machine https://web.archive.org/web/2019\*/http://www.defmacro.org/2016/12/22/writing-well.html](#wybckmchnswbrchvrgwbwwwdfmcrrgwrtngwllhtml) 
    -   [`[2019-11-15]` maybe https://youtu.be/zRxI0DaQrag?t=1380 ?](#mybsytbzrxdqrgt) 
    -   [`[2019-11-09]` github: https://twitter.com/i/web/status/928602151286386688 this end up trimmed with &#x2026; :(](#gthbstwttrcmwbsttsthsndptrmmdwth) 
    -   [`[2019-11-07]` github: https://twitter.com/i/web/status/1156086851633131520](#gthbstwttrcmwbstts) 
    -   [`[2021-01-24]` https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=941827](#sbgsdbnrgcgbnbgrprtcgbg) [[cannon]]
    -   [`[2021-02-28]` https://undeadly.org/cgi?action=article;sid=20170930133438](#snddlyrgcgctnrtclsd) [[cannon]]
    -   [hmm, server doesn't normalise properly?? (url escaping)](#hmmsrvrdsntnrmlsprprlyrlscpng) 
    -   [semiconductors video should be unified properly. well, or again hierarchical thing? might be too spammy for 'watch later'](#smcndctrsvdshldbnfdprprlylthngmghtbtspmmyfrwtchltr) 
    -   [`[2019-12-23]` https://cstheory.stackexchange.com/questions/1920/examples-of-unrelated-mathematics-playing-a-fundamental-role-in-tcs/1925#1925: need parent link to trigger on this in cannon](#scsthrystckxchngcmqstnsxmsndprntlnkttrggrnthsncnnn) 
    -   [`[2020-06-16]` https://news.ycombinator.com/item?id=23537243#23540421 hmm, both id and # ?](#snwsycmbntrcmtmdhmmbthdnd) 
    -   [`[2020-02-08]` https://bugzilla.mozilla.org/show\_bug.cgi?id=1411873 : ugh need to keep id](#sbgzllmzllrgshwbgcgdghndtkpd) 
    -   [`[2020-01-12]` old.reddit and new reddit](#ldrddtndnwrddt) 
    -   [`[2019-06-02]` handle google.com/search](#hndlgglcmsrch) 
    -   [`[2020-11-30]` https://www.c-span.org/video/?c4808083/rust-language-chosen the ? is sneaky](#swwwcspnrgvdcrstlnggchsnthssnky) 
    -   [`[2020-11-22]` https://melpa.org/#/async # is just redundant?](#smlprgsyncsjstrdndnt) 
    -   [`[2019-08-25]` Lisp Language http://wiki.c2.com/?LispLanguage ? is sneaky](#lsplnggwkccmlsplnggssnky) 
    -   [better regex for url extraction](#bttrrgxfrrlxtrctn) 
    -   [`[2020-11-18]` Vanquishing ‘Monsters’ in Foundations of Computer Science: Euclid, Dedekind, Frege, Russell, Gödel, Wittgenstein, Church, Turing, and Jaśkowski didn’t get them all … by Carl Hewitt :: SSRN](#spprsssrncmslpprscfmbstrckddntgtthmllbycrlhwttssrn) 
    -   [should be more defensive](#shldbmrdfnsv) 
        -   [`[2019-08-26]` did I do it?\*\* `[2020-12-09]` https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=955208 'bug' parameter](#dddtsbgsdbnrgcgbnbgrprtcgbgbgprmtr) 
    -   [`[2020-12-04]` https://unix.stackexchange.com/questions/117609/capture-error-of-ls-to-file#comment183614\_117609](#snxstckxchngcmqstnscptrrrrflstflcmmnt) 
    -   [`[2019-02-18]` make sure ? extracted correctly https://play.google.com/store/apps/details?id=com.faultexception.reader](#mksrxtrctdcrrctlysplygglcmstrppsdtlsdcmfltxcptnrdr) 
    -   [`[2019-05-04]` https://news.ycombinator.com/item?id=12973788](#snwsycmbntrcmtmd) 
    -   [`[2021-03-15]` wiki.c2.com pages don't even have canonical?](#wkccmpgsdntvnhvcnncl) [[cannon]]
-   [\* misc](#msc) 
    -   [would be convenient to normalise reddit annotations so annotations from all comments would be collected](#wldbcnvnnttnrmlsrddtnnttnttnsfrmllcmmntswldbcllctd) 
    -   [`[2019-09-03]` potential pypi project? https://pypi.org/project/cannon](#ptntlpypprjctspyprgprjctcnnn) 
    -   [hypothesis: wonder how it works on timestamped archive.org stuff?](#hypthsswndrhwtwrksntmstmpdrchvrgstff) 
    -   [hmm some local and remote pages may overlap](#hmmsmlclndrmtpgsmyvrlp) 
    -   [`[2020-05-11]` Vision, Mission & Values — 2020 Update - WorldBrain.io - Medium](#smdmcmwrldbrnvsnmssnvlspdbbvsnmssnvlspdtwrldbrnmdm) 
    -   [`[2019-07-09]` Changed how threading works. by JakeHartnell · Pull Request 952 · hypothesis/h https://github.com/hypothesis/h/pull/952](#chngdhwthrdngwrksbyjkhrtnypthsshsgthbcmhypthsshpll) [[hypothesis]] [[reddit]]
    -   [reddit: tested on https://www.reddit.com/r/explainlikeimfive/comments/1vavyq/eli5\_godels\_ontological\_proof/ceqlupx/](#rddttstdnswwwrddtcmrxplnltsvvyqlgdlsntlgclprfcqlpx) [[hypothesis]]
        -   [`[2019-07-09]` so look like reddit referes to the 'post' page as canonical. Right.](#slklkrddtrfrstthpstpgscnnclrght) 
-   [--------------------------------------------------](#25808_25903) 
-   [`[2021-03-26]` URLTeam - Archiveteam](#swkrchvtmrgndxphpttlrltmrltmrchvtm) [[cannon]]
-   [`[2021-03-25]` seomoz/url-py: URL Transformation, Sanitization](#sgthbcmsmzrlpysmzrlpyrltrnsfrmtnsntztn) [[cannon]]
-   [`[2021-03-03]` (5) Jon Borichevskiy (@jondotbo) / Twitter](#stwttrcmjndtbjnbrchvskyjndtbtwttr) [[promnesia]] [[cannon]]

Cannon is an idea for a project attempting to compute canonical/normalised URLs and extract some information from them ('entities'), merely by looking at the URL, and ideally without using the "rel=canonical" metadata.  
I describe the problem it tries to solve here: ["urls are broken"](https://beepb00p.xyz/promnesia.html#urls_broken), also see "motivation".  

At the moment it's a subproject of promnesia: see [cannon.py](https://github.com/karlicoss/promnesia/blob/master/src/promnesia/cannon.py)  
and [tests/cannon.py](https://github.com/karlicoss/promnesia/blob/master/tests/cannon.py).  

If anyone knows of similar efforts/prior art, **please let me know**! I'd really like to avoid reinvening the wheel here.  




# related 





## promnesia as a primary application (for me)      [[promnesia]]




## .       [[linkrot]]




# \* motivation

Once you are sold on motivation in this section, and wondering why would this require a separate library/database, check out "testcases" section.  




## `[2020-04-04]` I want urls that represent information, regardless the way it's presented

let alone all the tracking/etc crap  




### `[2020-05-23]` "document equivalence" is a good term: [How to establish (or avoid) document equivalence in the Hypothesis system : Hypothesis](https://web.hypothes.is/help/how-to-establish-or-avoid-document-equivalence-in-the-hypothesis-system/)




## why not use "rel=canonical" metadata field?





### `[2020-05-27]` [Google no longer providing original URL in AMP for image search results](https://news.ycombinator.com/item?id=23322730)




### `[2019-10-11]` mobile versions of sites sometimes have different "canonical", e.g. mobile.twitter.com

No one would argue that a tweet is the same regardless where it's presented, yet there is no easy way to unify this  




### `[2020-05-28]` archive.org is messing with canonical      [[cannon]]




### `[2019-11-02]` e.g. this link doesn't have 'canonical' even though it's a mirror: <https://solar.lowtechmagazine.com/2016/11/the-curse-of-the-modern-office.html>




### `[2019-11-08]` no canonical on gist <https://gist.github.com/dneto/2258454>

same as <https://gist.github.com/2258454> &#x2013; hmm, this thing redirects now..  




## `[2019-08-19]` parent and sibling relations can be determined from the URL      [[cannon]] [[promnesia]]

e.g. subreddit-post/user-comment/user-tweet, etc.  




## `[2019-11-01]` if the original page is gone I can still easily link my saved annotations (Instapaper/Pocket/Hypothesis) to archived page

<https://web.archive.org/web/20090902224414/http://reason.com/news/show/119237.html>  




## `[2019-09-07]` urls a good candidate to determine 'entities' because they sure at least somewhat curated      [[cannon]]




## `[2019-02-24]` normalization is tricky.. for some urls, stuff after # is important <https://en.wikipedia.org/wiki/Tendon#cite_note-14> . for some, it's utter garbage

however we can sort of get away with normalizing on server only?  




## `[2019-08-07]` The Problem With URLs <https://blog.codinghorror.com/the-problem-with-urls/>

-   `[2019-08-27]` not very insigntful, example of msdn with weird characters in urls




## `[2020-01-02]` motivation: siloing: instapaper 'imports' pages and assigns an id: <https://www.instapaper.com/read/1265139707>

so you can't connect your annotations on instapaper to notes etc  




## `[2021-03-07]` could normalize historic URLs which are already down?      [[linkrot]]

perhaps not super useful if we can't access them, but still  




# \* projects that could benefit from it

Apart from Promnesia, I believe it could be quite useful for other projects.  




## `[2019-06-27]` Hmm could be helpful for hypothesis?      [[hypothesis]]

-   `[2020-04-29]` write about it? the future?




### `[2021-01-16]` discuss about cannon (maybe on Slack)?      [[hypothesis]] [[cannon]]




### `[2019-05-24]` [Annotation of content on sites like Facebook or Twitter? - Google Groups](https://groups.google.com/a/list.hypothes.is/forum/#!topic/dev/kcmS7H8ssis)      [[hypothesis]]

kinda related since they basically want canonical urls  




## `[2021-01-30]` [Ignore URL parameters - Feature Requests - Memex Community](https://community.worldbrain.io/t/ignore-url-parameters/551/5)      [[worldbrain]]




## `[2021-01-22]` wonder if we could cooperate?      [[agora]] [[cannon]]




## `[2021-01-24]` would be useful to use the same normalising engine for #archivebox for example?      [[webarchive]]

-   `[2021-03-10]` although I guess it needs to fetch the page anyway so "rel=canonical" works we ll enough




## `[2021-02-07]` could be useful for surfingkey/nyxt browser to hint 'interesting' urls?




## `[2019-12-26]` archive.org      [[linkrot]]

e.g. if the link is not present in archive.org, it doesn't mean it's not archived under a different canonical  




## if it's implemented as a helper extension/library, it could be useful for many other extensions

e.g. blockers, various highlighters, hypothesis, etc  




## `[2020-12-07]` [einaregilsson/Redirector: Browser extension (Firefox, Chrome, Opera, Edge) to redirect urls based on regex patterns, like a client side `mod_rewrite` ](https://github.com/einaregilsson/Redirector)




## `[2020-11-20]` could reuse URL underlying etc with ampie?      [[ampie]]




# \* prior art

URL normalization algorithm should be shared with other projects to the maximum extent possible.  
If not the exact algorithm, at least the 'curated' parts of it like regexes, testcases, etc should be shared.  
It's a crap boring work that should be only done once (e.g. like timezones database).  




## `[2020-06-30]` [ClearURLs / Addon](https://github.com/ClearURLs/Addon#application): looks super super promising

    Once ClearURLs has cleaned the address, it will look like this: https://www.amazon.com/dp/exampleProduct




### `[2021-03-10]` <https://github.com/ClearURLs/Addon/wiki/Rules>:  Not super convinced JSON would work well in general, but anyway it's already pretty good.




## `[2020-11-22]` [WorldBrain/memex-url-utils: Shared URL processing utilities for Memex extension and mobile apps.](https://github.com/WorldBrain/memex-url-utils)      [[worldbrain]]




## `[2019-07-09]` h/uri.py at 0fc8a0d345741d43b4f80856a7cbb8f5afa70f80 · hypothesis/h <https://github.com/hypothesis/h/blob/0fc8a0d345741d43b4f80856a7cbb8f5afa70f80/h/util/uri.py>      [[hypothesis]]





### `[2019-07-09]` excluded query params!




### `[2019-07-09]` right, I could probably reuse hypothesis's canonify and contribute back. looks very similar to mine




## `[2020-05-12]` [coleifer/micawber: a small library for extracting rich content from urls](https://github.com/coleifer/micawber)





### `[2021-03-10]` ok, pretty interesting. it probably uses network, but could at least use it for testing (or maybe even 'enriching'?)




## `[2019-03-27]` [sindresorhus/compare-urls: Compare URLs by first normalizing them](https://github.com/sindresorhus/compare-urls)

    compareUrls('HTTP://sindresorhus.com/?b=b&a=a', 'sindresorhus.com/?a=a&b=b');




### `[2019-12-25]` [sindresorhus/normalize-url](https://github.com/sindresorhus/normalize-url)

`stripWWW` can't handle amp etc  




## `[2019-07-09]` [hypothesis: `h/normalize_uris_test.py`](https://github.com/hypothesis/h/blob/0fc8a0d345741d43b4f80856a7cbb8f5afa70f80/tests/h/cli/commands/normalize_uris_test.py)




## `[2019-04-16]` [niksite/url-normalize: URL normalization for Python](https://github.com/niksite/url-normalize)




## `[2020-04-27]` [john-kurkowski/tldextract: Accurately separate the TLD from the registered domain and subdomains of a URL, using the Public Suffix List.](https://github.com/john-kurkowski/tldextract)

hmm could use this for better extraction&#x2026;  




## `[2019-03-27]` [rbaier/python-urltools: Some functions to parse and normalize URLs.](https://github.com/rbaier/python-urltools)




# \* ideas





## `[2021-03-07]` maybe we can achieve 95% accuracy with generic rules and by handling the most popular websites

for the rest  

-   allow user to customize
-   allow user to submit normalization errors (where?)




## if 'children' relations can't be determined by substring matching, perhaps cannon should generate 'virtual' urls?      [[promnesia]] [[cannon]]




## a special service to resolve siloed links like t.co ?      [[linkrot]]

Could also be useful for Archive.org/archivebox/etc. But a bit out of scope for this project..  




## just specify admissible regexes for urls so it's easier to unify?

e.g. twitter.com/user/status/statusid  

maybe normalise to this?  
twitter.com/i/web/status/1053151870791835649  

reddit.com/comments/5ombk8 &#x2013; huh, normalise to this?  
TODO m.readdit/old.reddit  

en.m.wikipedia/ru.m.wikipedia  
maybe stripp off subdom completely?  

youtube.com/watch?v=xAy&#x2014;wp<sub>DQ</sub>&list=PL0k<sub>yDgrqAiU</sub><sub>EF5d7krLIds1ebhTxCjm</sub>&shuffle=221  
youtube.com/watch?v=Woa3MPijE3s&list=PL0k<sub>yDgrqAiXKspaa1GIS0jbbLrsAa3sk</sub>&spfreload=10  




### `[2019-11-09]` also this to summarize

sqlite3 promnesia.sqlite 'select domain, count(domain) from (select substr(norm<sub>url</sub>, 0, instr(norm<sub>url</sub>, "/")) as domain from visits) group by domain order by count(domain)'  




## rethinking the whole approach&#x2026;

consider <https://www.youtube.com/watch?v=wHrCkyoe72U&list=WL>  
basically  

-   cut of protocol just merely for simplicity? I guess makes everything much easier
-   the result is always 'composed of' inputs. e.g. maps to youtube/wHrCkyoe72U, both parts are in the original link  
    might not be the case if domain names are remapped though.. e.g. youtu.be
-   sort query parts alphabetically  
    (although might make sense to make it hierarchy aware?)
-   treat parts & query the same way, parts are query with None keys
-   to handle domain names better, replace dots before first / with *: e.g. www.youtube.com* -> www/youtube/com  
    then cat treat the same way as subpaths  
    i.e. we get  
    None www          | drop  
    None youtube      | keep  
    None com          | drop  
    None watch        | drop  
    list WL           | keep? &#x2013; actually this could be considered a 'tag'? unclear  
    v    wHrCkyoe72U  | keep

ok so how do we generalize from two examples?  
 e.g. say we also have  
 youtube.ru/watch?v=abacaba -> youtube/abacaba  
 we get  
      youtube | keep  
      ru      | drop  
      watch   | drop  
 v    abacaba | keep  
I suppose it could guess that if we keep a query parameter once, we'll keep it always?  
and if we extracted a certain substring without a query parameter, we'll also always keep it as is?  

TODO how about this?  
<https://news.ycombinator.com/reply?id=25100810&goto=item%3Fid%3D25099862%2325100810>  
it's a reply to       <https://news.ycombinator.com/item?id=25100035>  
which is a comment to <https://news.ycombinator.com/item?id=25099862>  




## use shared JS/python tests for canonifying?      [[ffi]] [[promnesia]]




## `[2019-09-03]` should be idempotent?




## hmm, maybe the extension can learn normalisation ruls over time? by looking at canonical and refining the rules?




## sample random links and their canonicals for testing




## background thing that sucks in canonical urls and provides data for testing?      [[promnesia]]




## how do we prune links that are potentially not secure to store? like certain URL parameters




## need checks that url don't contain stupid shit like trailing colons etc




## hmm could use this api for checking normalization?      [[cannon]]

    http get 'http://archive.org/wayback/available?url=https://stackoverflow.com/questions/1425892/how-do-you-merge-two-git-repositories'
    {
        "archived_snapshots": {
            "closest": {
                "available": true,
                "status": "200",
                "timestamp": "20210219235548",
                "url": "http://web.archive.org/web/20210219235548/https://stackoverflow.com/questions/1425892/how-do-you-merge-two-git-repositories"
            }
        },
        "url": "https://stackoverflow.com/questions/1425892/how-do-you-merge-two-git-repositories"
    }




# \* testcases

Some tricky cases which would be nice to get right  




## `[2020-11-15]` [Wendover Productions - YouTube](https://www.youtube.com/c/Wendoverproductions/videos)




## `[2020-04-19]` roam links




## `[2021-02-07]` <https://app.element.io/#/room/#blockchain:fosdem.org>      [[cannon]]




## `[2021-02-16]` [A Relational Turn for Data Protection? by Neil M. Richards, Woodrow Hartzog :: SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3745973)      [[cannon]]

abstract<sub>id</sub>  




## `[2019-06-23]` A Brief Intro to Topological Quantum Field Theories. - YouTube <https://www.youtube.com/watch?v=59uLGIrkMxM&list=WL&index=61&t=0s>

eh, rules might be a bit complicated. E.g. if both v and list are present, we wanna ditch list, otherwise keep list  




## `[2020-11-16]` [normalise DOI](https://twitter.com/amogh_jalihal/status/1328393853599059970)

    Ah sure: This DOI: https://doi.org/10.1073/pnas.1211902109  should lead to this paper: https://pnas.org/content/109/48/E3324 .




## m.wikipedia normalisation could also be useful for hypothesis?      [[hypothesis]]





### `[2019-07-23]` X.m.wikipedia.org




### `[2019-07-23]` mm, it's got canonical though..




### `[2019-07-23]` perhaps promnesia should respond both to canonical and its own idea of normalised (preferring canonical)




## `[2019-04-20]` fragments: Aharonov-Bohm Experiment <https://physicstravelguide.com/experiments/aharonov-bohm#tab__concrete>

url normalising&#x2026; this is an example where fragments are important  




### `[2019-08-26]` here I guess it could yield url with hash + parent url?




### `[2019-08-26]` always assume that parents in uri hierarchy are actual parents? I guess that's fairly reasonable




## `[2019-08-25]` stuff like this:  youtu.be/1TKSfAkWWN0





### `[2019-08-25]` this is also motivation for canonifying. this is a redirect link in tweet, and there is no way to associate it with canonical




## `[2020-05-02]` <https://hubs.mozilla.com/#/>      [[cannon]]




## `[2020-04-30]` [Writing well | defmacro](http://www.defmacro.org/2016/12/22/writing-well.html)

support for archive.org and test on this page  




### `[2020-05-28]` Wayback Machine <https://web.archive.org/web/2019*/http://www.defmacro.org/2016/12/22/writing-well.html>




## `[2019-11-15]` maybe <https://youtu.be/zRxI0DaQrag?t=1380> ?




## `[2019-11-09]` github: <https://twitter.com/i/web/status/928602151286386688> this end up trimmed with &#x2026; :(




## `[2019-11-07]` github: <https://twitter.com/i/web/status/1156086851633131520>




## `[2021-01-24]` <https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=941827>      [[cannon]]

    https://wiki.debian.org/SecureBoot#MOK_-_Machine_Owner_Keycanonical: wiki.debian.org/SecureBootsources : notes[[https://wiki.debian.org/SecureBoot][SecureBoot - Debian Wiki]]




## `[2021-02-28]` <https://undeadly.org/cgi?action=article;sid=20170930133438>      [[cannon]]

'sid' matters here  




## hmm, server doesn't normalise properly?? (url escaping)

    ru.wikipedia.org/wiki/Грамматикализация




## semiconductors video should be unified properly. well, or again hierarchical thing? might be too spammy for 'watch later'




## `[2019-12-23]` <https://cstheory.stackexchange.com/questions/1920/examples-of-unrelated-mathematics-playing-a-fundamental-role-in-tcs/1925#1925>: need parent link to trigger on this in cannon




## `[2020-06-16]` <https://news.ycombinator.com/item?id=23537243#23540421> hmm, both id and # ?




## `[2020-02-08]` <https://bugzilla.mozilla.org/show_bug.cgi?id=1411873> : ugh need to keep id




## `[2020-01-12]` old.reddit and new reddit




## `[2019-06-02]` handle google.com/search




## `[2020-11-30]` <https://www.c-span.org/video/?c4808083/rust-language-chosen> the ? is sneaky




## `[2020-11-22]` <https://melpa.org/#/async> # is just redundant?




## `[2019-08-25]` Lisp Language <http://wiki.c2.com/?LispLanguage> ? is sneaky




## better regex for url extraction

eh, urls can have commas&#x2026;  e.g. <http://adit.io/posts/2013-04-17-functors,_applicatives,_and_monads_in_pictures.html>  
so, for csv need a separate extractor.  




## `[2020-11-18]` [Vanquishing ‘Monsters’ in Foundations of Computer Science: Euclid, Dedekind, Frege, Russell, Gödel, Wittgenstein, Church, Turing, and Jaśkowski didn’t get them all … by Carl Hewitt :: SSRN](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3603021)




## should be more defensive

    ValueError: netloc ' +79869929087, mak34@gmail.com' contains invalid characters under NFKC normalization




### `[2019-08-26]` did I do it?\*\* `[2020-12-09]` <https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=955208> 'bug' parameter




## `[2020-12-04]` <https://unix.stackexchange.com/questions/117609/capture-error-of-ls-to-file#comment183614_117609>




## `[2019-02-18]` make sure ? extracted correctly <https://play.google.com/store/apps/details?id=com.faultexception.reader>




## `[2019-05-04]` <https://news.ycombinator.com/item?id=12973788>

id here is important  




## `[2021-03-15]` wiki.c2.com pages don't even have canonical?      [[cannon]]




# \* misc





## would be convenient to normalise reddit annotations so annotations from all comments would be collected




## `[2019-09-03]` potential pypi project? <https://pypi.org/project/cannon>




## hypothesis: wonder how it works on timestamped archive.org stuff?




## hmm some local and remote pages may overlap

e.g. this is very likely to be mapped to normal py docss  
<file:///usr/share/doc/python3/html/library/contextlib.html>  




## `[2020-05-11]` [Vision, Mission & Values — 2020 Update - WorldBrain.io - Medium](https://medium.com/@WorldBrain/vision-mission-values-2020-update-d70aa35a638#0b0b)

fragments are often random and useless  
even default org-mode is guilty  




## `[2019-07-09]` Changed how threading works. by JakeHartnell · Pull Request 952 · hypothesis/h <https://github.com/hypothesis/h/pull/952>      [[hypothesis]] [[reddit]]




## reddit: tested on <https://www.reddit.com/r/explainlikeimfive/comments/1vavyq/eli5_godels_ontological_proof/ceqlupx/>      [[hypothesis]]

huh, so reddit seems to normalise to the main page, and displays annotations as 'orphaned' for comment views?  




### `[2019-07-09]` so look like reddit referes to the 'post' page as canonical. Right.




# -------------------------------------------------- 




# `[2021-03-26]` [URLTeam - Archiveteam](https://wiki.archiveteam.org/index.php?title=URLTeam)      [[cannon]]




# `[2021-03-25]` [seomoz/url-py: URL Transformation, Sanitization](https://github.com/seomoz/url-py)      [[cannon]]




# `[2021-03-03]` [(5) Jon Borichevskiy (@jondotbo) / Twitter](https://twitter.com/jondotbo)      [[promnesia]] [[cannon]]

hmm how to resolve twitter renames?&#x2026;  

