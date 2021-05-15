Eventually I'll write about it [here](https://beepb00p.xyz/axol.html)  


# Table of Contents

-   [Motivation](#mtvtn) 
    -   [I don't necessarily want to read everything found by 'scott alexander', but it's still interesting to run search to see the overlap between people?](#dntncssrlywnttrdvrythngfntngtrnsrchtsthvrlpbtwnppl) 
    -   [why not hnrss?](#whynthnrss) 
    -   [why axol over rss bridges?](#whyxlvrrssbrdgs) 
    -   [motivation: I don't understand how google search alerts work. e.g. try on openbci query (see my old emails from google alert)](#mtvtndntndrstndhwgglsrchlnpnbcqrysmyldmlsfrmggllrt) 
    -   [`[2019-12-30]` Ask HN: Do you still use RSS? | Hacker News](#skhndystllsrsshckrnws) [[rss]] [[toblog]]
    -   [`[2018-11-24]` problems with diff approach](#prblmswthdffpprch) 
    -   [TW at `[2018-10-02]` А кто-нибудь знает тулы типа https://t.co/EbpbNZWQFC , но чтобы туда можно было вбить грубо говоря любую поисковую кверю, или API (например reddit/github); и оно отслеживало результаты?](#twttrcmkrlcsssttstwtактонионоотслеживалорезультаты) 
    -   [`[2020-06-22]` I feel the same. So many cool things I'd love to learn about, but not enough tim&#x2026; | Hacker News](#snwsycmbntrcmtmdflthsmsmndlvtlrnbtbtntnghtmhckrnws) [[pkm]] [[axol]]
-   [Similar/existing projects](#smlrxstngprjcts) 
    -   [`[2020-03-03]` Show HN: Mailbrew – Automated Email Digests from HN, RSS, Reddit, Twitter](#snwsycmbntrcmtmdshwhnmlbrdmldgstsfrmhnrssrddttwttr) 
    -   [`[2019-12-26]` awesome-selfhosted/awesome-selfhosted: A list of Free Software network services and web applications which can be hosted locally. Selfhosting is the process of hosting and managing applications instead of renting from Software-as-a-Service providers](#wsmslfhstdwsmslfhstdlstfffrntngfrmsftwrssrvcprvdrs) 
    -   [trackreddit only two subscriptions](#trckrddtnlytwsbscrptns) 
    -   [tool to search on reddit or even custom services? special ordering ('least likely' for showing least occuring subreddits). could also do it on rust?](#tltsrchnrddtrvncstmsrvcssstccrngsbrddtscldlsdtnrst) [[pkm]]
-   [\* Make it more user friendly](#mktmrsrfrndly) 
    -   [add axol doctor config](#ddxldctrcnfg) [[project]]
    -   [rely on user config dirs](#rlynsrcnfgdrs) 
    -   [provide an asci diagram for crawler + report + feed reader?](#prvdnscdgrmfrcrwlrrprtfdrdr) 
-   [\* Blacklisting](#blcklstng) 
    -   [maybe button to ban user? it would write to config or something? maybe I can even use some public API constructor?](#mybbttntbnsrtwldwrttcnfgrngmybcnvnssmpblcpcnstrctr) 
    -   [I suppose pouchdb would be perfect for blacklisting](#sppspchdbwldbprfctfrblcklstng) [[couchdb]]
    -   [for blacklisting, instead could just apply custom per-user classes? or even edit them. that would allow to highlight properly](#frblcklstngnstdcldjstpplyhmthtwldllwthghlghtprprly) 
    -   [yeah, blacklisting could both update backend and hide locally](#yhblcklstngcldbthpdtbckndndhdlclly) 
    -   [`[2019-04-15]` axol results for reddit<sub>pkm</sub>, rendered at Fri 12 Apr 2019 05:07](#xlrsltsfrrddtpkmrndrdtpr) 
    -   [shit, top lifelogging tweets are on japanese&#x2026;](#shttplflggngtwtsrnjpns) [[twitter]]
    -   [would be interesting to ignore links I already visited from results. It can even be done automatically&#x2026;.](#wldbntrstngtgnrlnkslrdyvstdfrmrsltstcnvnbdntmtclly) [[promnesia]] [[axol]]
    -   [huh, quite a few bots on reddit?](#hhqtfwbtsnrddt) [[reddit]]
    -   [huh, lots of stuff from twitter is just garbage. need a good way of suppressing it&#x2026;](#hhltsfstfffrmtwttrsjstgrbgndgdwyfspprssngt) [[axol]] [[twitter]]
-   [What would be a good UI for axol?](#whtwldbgdfrxl) 
    -   [I really need some sort of proper frontend browser for it&#x2026;](#rllyndsmsrtfprprfrntndbrwsrfrt) 
    -   [would be nice to have some html dashboard, so it's easy to blacklist terms?](#wldbncthvsmhtmldshbrdstssytblcklsttrms) 
    -   [need a UI to easily add items to axol. e.g. Alexei Kitaev](#ndtslyddtmstxlglxktv) 
    -   [use metabase or something? could use a column to mark as seen? would be much easier than rss](#smtbsrsmthngcldsclmntmrkssnwldbmchsrthnrss) 
    -   [dunno about rss interface&#x2026; really need a more efficient way of processing content, reordering, etc](#dnnbtrssntrfcrllyndmrffcntwyfprcssngcntntrrdrngtc) 
-   [Queries](#qrs) 
    -   [search for 'data export' or something?](#srchfrdtxprtrsmthng) 
    -   [`[2020-01-12]` github.com/karlicoss - Twitter Search / Twitter](#gthbcmkrlcsstwttrsrchtwttr) [[self]]
    -   [`[2020-01-30]` my. package | beepb00p](#mypckgbpbp) [[postprivacy]] [[qs]] [[toread]]
    -   [`[2019-02-15]` What Universal Human Experiences Are You Missing Without Realizing It? | Slate Star Codex](#whtnvrslhmnxprncsrymssngwthtrlzngtsltstrcdx) [[mind]]
    -   [`[2019-06-29]` https://github.com/hypotext/notation - Twitter Search](#sgthbcmhyptxtnttntwttrsrch) 
    -   [`[2020-01-09]` karlicoss/cachew - Twitter Search / Twitter](#krlcsscchwtwttrsrchtwttr) [[cachew]]
    -   [`[2020-08-24]` All | Search powered by Algolia Noon Universe search](#shnlglcmdtrngllpgprfxtrqrllsrchpwrdbylglnnnvrssrch) 
    -   [mypy &#x2013; exclude mypython; prioritize topics](#mypyxcldmypythnprrtztpcs) [[mypy]]
    -   [sleep tracking](#slptrckng) [[sleep]] [[qs]]
    -   [add bret victor?](#ddbrtvctr) [[bretvictor]]
    -   [ted chiang &#x2013; pretty nice to search on twitter](#tdchngprttynctsrchntwttr) [[tedchiang]]
    -   [complex numbers group; argonov; transhumanism?](#cmplxnmbrsgrprgnvtrnshmnsm) [[argonov]]
    -   [kobo; spaced repetition?](#kbspcdrpttn) [[spacedrep]]
    -   [`[2018-08-25]` scott alexander unsong - Twitter Search](#scttlxndrnsngtwttrsrch) 
    -   [karlicoss!](#krlcss) [[self]]
    -   [cancel scott alexander search alert](#cnclscttlxndrsrchlrt) 
    -   [set up alerts for nutrition stuff](#stplrtsfrntrtnstff) 
    -   [add "lagrangian mechanics"???](#ddlgrngnmchncs) [[lagrangian]]
    -   [`[2020-03-09]` #promnesia](#prmns) 
    -   [kedr livansky](#kdrlvnsky) [[kedr]]
    -   [exobrain?](#xbrn) [[exobrain]]
    -   [`[2020-05-01]` Pinboard bookmarks tagged eeg](#spnbrdntgpnbrdbkmrkstggdg) 
    -   [`[2020-05-01]` Pinboard bookmarks tagged km](#spnbrdntkmpnbrdbkmrkstggdkm) [[pkm]]
    -   [memex? esp github](#mmxspgthb) [[memex]]
    -   [george hotz?](#grghtz) 
    -   [add mypy to search??](#ddmypytsrch) 
    -   [`[2019-10-01]` tried aaxol for](#trdxlfr) 
    -   [pkm for twitter can probably be removed&#x2026;](#pkmfrtwttrcnprbblybrmvd) 
    -   [initial query&#x2026;](#ntlqry) [[mypy]]
    -   [cleanup 'extended mind' &#x2013; certainly lots of crap in the database](#clnpxtnddmndcrtnlyltsfcrpnthdtbs) [[twitter]]
    -   [hmm, beepb00p.xyz isn't resolving anything?](#hmmbpbpxyzsntrslvngnythng) [[self]] [[twitter]]
    -   [`[2019-12-02]` axol results for hackernews<sub>pkm</sub>, rendered at 02 Dec 2019 11:05](#xlrsltsfrhckrnwspkmrndrdtdc) 
    -   [`[2019-12-02]` axol results for hackernews<sub>pkm</sub>, rendered at 02 Dec 2019 11:05](#xlrsltsfrhckrnwspkmrndrdtdc) 
    -   [subscribe to more news on QS, BCI and gadgets](#sbscrbtmrnwsnqsbcndgdgts) [[qs]]
-   [Sources](#srcs) 
    -   [wonder if I could search among hypothesis users&#x2026;](#wndrfcldsrchmnghypthsssrs) [[hypothesis]]
    -   [could add google search too I suppose.. but that's def lowest priority](#cldddgglsrchtsppsbtthtsdflwstprrty) 
    -   [implement for reddit. release reddit/github searchers (as library, then import and use)](#mplmntfrrddtrlsrddtgthbsrchrsslbrrythnmprtnds) 
    -   [youtube? could search quantified self at least](#ytbcldsrchqntfdslftlst) 
    -   [World be great to search in comments](#wrldbgrttsrchncmmnts) [[axol]] [[reddit]]
    -   [hypothesis](#hypthss) 
    -   [`[2019-07-28]` Schedule - pushshift.io](#schdlpshshft) 
    -   [`[2019-07-28]` New API endpoint &#x2013; Now you can search comments! : redditdev](#nwpndpntnwycnsrchcmmntsrddtdv) 
    -   [for google search, only notify about new results; not about changes. wonder how?](#frgglsrchnlyntfybtnwrsltsntbtchngswndrhw) 
    -   [`[2019-12-28]` Search Reddit Comments by User](#srchrddtcmmntsbysr) 
    -   [`[2020-01-11]` pushshift/api: Pushshift API](#pshshftppshshftp) 
    -   [duckduckgo?](#dckdckg) 
    -   [`[2019-12-01]` Pushshift Reddit Search](#pshshftrddtsrch) [[reddit]] [[scrape]]
    -   [`[2019-12-15]` hacker-news-favorites-api/main.js at master · reactual/hacker-news-favorites-api](#hckrnwsfvrtspmnjstmstrrctlhckrnwsfvrtsp) 
    -   [`[2020-05-18]` Hypothesis](#shypthsssrchqbpbpxyzhypthss) 
    -   [could run HN more often](#cldrnhnmrftn) [[hackernews]]
    -   [`[2020-05-03]` [[https://grep.app/search?q=import%20my%5C..%2A%24&regexp=true&filter[lang][0]=Python][import my\\..\*$ - grep.app]]](#sgrpppsrchqmprtmycrgxptrfltrlngpythnmprtmygrppp) 
-   [CI/testing](#ctstng) 
    -   [HN is very quick, so prob really good to test on (even on CI)](#hnsvryqcksprbrllygdttstnvnnc) 
-   [Sort tags by number of total occurences?](#srttgsbynmbrfttlccrncs) 
-   [Use cachew and keep stuff as blobs with id](#scchwndkpstffsblbswthd) [[cachew]]
-   [warn when there are too many atom items?](#wrnwhnthrrtmnytmtms) 
-   [suppress some feeds in the config?](#spprsssmfdsnthcnfg) 
-   [`[2020-11-21]` Show HN: I made an alternative to Google Alerts that listens to social media](#snwsycmbntrcmtmdshwhnmdnlntvtggllrtsthtlstnstsclmd) 
    -   [`[2020-12-05]` eh, demands to register etc](#hdmndstrgstrtc) 
-   [shit, seems that the timestamps are wrong and also I got the link wrong](#shtsmsthtthtmstmpsrwrngndlsgtthlnkwrng) 
-   [Maybe record a video on the phone ?](#mybrcrdvdnthphn) [[demo]]
-   [maybe check crawled pinboard users for interesting tags/links?](#mybchckcrwldpnbrdsrsfrntrstngtgslnks) 
    -   [`[2019-06-15]` yeah, need to make this bit more effecient..](#yhndtmkthsbtmrffcnt) 
-   [maybe, summary and 'rendered' are really sort of the same page? just different sorting&#x2026;](#mybsmmryndrndrdrrllysrtfthsmpgjstdffrntsrtng) 
-   [Def interesting to see user stats](#dfntrstngtssrstts) 
-   [Sort tags by number of total occurences?](#srttgsbynmbrfttlccrncs) 
-   [Maybe better way of normalising? E.g. look at ted<sub>chiang</sub>  and gq article. Display 'bumped' entries separately? Like a different way of sorting](#mybbttrwyfnrmlsngglkttdchtrssprtlylkdffrntwyfsrtng) 
-   [prepend # in tag?](#prpndntg) 
-   [could search for interesting tags occurence without them actually being scraped](#cldsrchfrntrstngtgsccrncwthtthmctllybngscrpd) 
-   [might be good to do some sort of fuzzy grouping?](#mghtbgdtdsmsrtffzzygrpng) 
-   [would be interesting to have explorer for users that looks for some relevant taks/keywords?](#wldbntrstngthvxplrrfrsrsthtlksfrsmrlvnttkskywrds) [[pinboard]]
-   [Hmm also need real-time search and notify I guess?](#hmmlsndrltmsrchndntfygss) [[hackernews]]
-   [Eh, better idea would be a tag subscription&#x2026;](#hbttrdwldbtgsbscrptn) [[mypy]]
-   [would be nice to have some efficient frontend + backend thing](#wldbncthvsmffcntfrntndbckndthng) [[timeline]]
    -   [`[2019-12-02]` hmmm. actually could do it in a twitter account??](#hmmmctllyclddtntwttrccnt) 
    -   [`[2019-12-04]` could ask on HN?](#cldsknhn) [[outbox]]
    -   [`[2019-12-04]` or RSS?  https://github.com/awesome-selfhosted/awesome-selfhosted#feed-readers](#rrsssgthbcmwsmslfhstdwsmslfhstdfdrdrs) 
-   [`[2019-12-24]` Edit Feed: beepb00p.xyz - Miniflux](#dtfdbpbpxyzmnflx) 
-   [`[2019-12-24]` Command Line Usage - Documentation](#cmmndlnsgdcmnttn) 
-   [could make a filter to release items slowly? e.g. tweets with more than 10 likes, if update pops it up, then it ends up in the feed. although I need 'processed' entries](#cldmkfltrtrlstmsslwlygtwtdspnthfdlthghndprcssdntrs) 
-   [`[2020-05-27]` Axol: Personal automatic news feed – crawl Reddit/Twitter/HN and read as RSS | Hacker News](#snwsycmbntrcmtmdxlprsnltmddttwttrhnndrdsrsshckrnws) 
-   [perhaps redefine everything in entities? and have relations &#x2013; people, subreddits, urls, tags, etc](#prhpsrdfnvrythngnnttsndhvrltnspplsbrddtsrlstgstc) 
-   [rename adhoc to 'search'?](#rnmdhctsrch) 
-   [think about a special tag to mark stuff that should be autoimported in a similar manner my kibitzr thing worked](#thnkbtspcltgtmrkstffthtshdnsmlrmnnrmykbtzrthngwrkd) 
-   [some todos](#smtds) 
-   [def should keep original results in the DB as far as possible](#dfshldkprgnlrsltsnthdbsfrspssbl) 
-   [to start with, only support exact queries? e.g. demand them in queries and mention that support for fuzzier might be added later](#tstrtwthnlyspprtxctqrsgdmthtspprtfrfzzrmghtbdddltr) 
-   [think about multiple small databases vs one huge?](#thnkbtmltplsmlldtbssvsnhg) 
-   [thinking about query language](#thnkngbtqrylngg) 
-   [for people to try it out it really needs a simplest service possible they can run with docker? ideally without auth etc](#frpplttrytttrllyndssmplsthycnrnwthdckrdllywthtthtc) 
-   [Track most active pinboard users? They might have interesting other stuff](#trckmstctvpnbrdsrsthymghthvntrstngthrstff) 
    -   [`[2019-07-20]` maybe, try to intersect known user's tags and see what they got in common?](#mybtrytntrsctknwnsrstgsndswhtthygtncmmn) 
-   [running under docker results in /app/axol/js/sorttable](#rnnngndrdckrrsltsnppxljssrttbl) 
-   [use different font?](#sdffrntfnt) 
-   [might need two pass algorithm? One for crawling, second for filtering?](#mghtndtwpsslgrthmnfrcrwlngscndfrfltrng) 
-   [related](#rltd) [[pkm]] [[search]] [[degoogle]]
-   [`[2019-04-15]` Pinboard: network for karlicoss](#pnbrdntwrkfrkrlcss) [[pinboard]] [[axol]]
    -   [`[2021-01-16]` in fact it's the most common request to pinboard author apparently](#nfcttsthmstcmmnrqsttpnbrdthrpprntly) 
-   [spinboard: something's not right. e.g. try](#spnbrdsmthngsntrghtgtry) 
    -   [must be some pinboard bug??](#mstbsmpnbrdbg) [[pinboard]]
-   [`[2019-11-06]` classes — classes 0.1.0 documentation](#clsssclsssdcmnttn) 
    -   [`[2020-02-15]` hmm, somethihg  I was trying to do in axol?&#x2026;](#hmmsmthhgwstryngtdnxl) [[axol]]
-   [doesn't look active. all top results are from 2017](#dsntlkctvlltprsltsrfrm) [[axol]] [[upspin]]
-   [`[2019-09-04]` ScriptSmith/socialreaper: Social media scraping / data collection library for Facebook, Twitter, Reddit, YouTube, Pinterest, and Tumblr APIs](#scrptsmthsclrprsclmdscrpnttrrddtytbpntrstndtmblrps) [[reddit]] [[scrape]] [[axol]]
    -   [`[2020-05-16]` ok, seems to be using real APIs, so overall I'm skeptical. but it's got a nice panel for tokens](#ksmstbsngrlpssvrllmskptclbttsgtncpnlfrtkns) [[exports]] [[jdoe]]
-   [pruning &#x2013; for now via sqlitedbbrowser? make sure it locks the db?](#prnngfrnwvsqltdbbrwsrmksrtlcksthdb) [[axol]]




# Motivation 





## I don't necessarily want to read everything found by 'scott alexander', but it's still interesting to run search to see the overlap between people?




## why not hnrss?

it's very likely more convenient to use if you only want a few HN queries, and don't care about historic ones  




## why axol over rss bridges?

rss is awesome! downsides  

-   might be trickier to do various post-filtering
-   with axol, you can compare results across queries (user summary)
-   can be used with promnesia maybe




## motivation: I don't understand how google search alerts work. e.g. try on openbci query (see my old emails from google alert)




## `[2019-12-30]` Ask HN: Do you still use RSS? | Hacker News      [[rss]] [[toblog]]

<https://news.ycombinator.com/item?id=21913598>  

    I've just started using Feedbin about a month ago, and although my HN firehose feed is at like 1100 something, it definitely limits the rest of the HN feeds. The show and ask feeds are both stuck around 400 something.




## `[2018-11-24]` problems with diff approach



### random errors, resulting in empty diff


### small differences in output (e.g. google search)


### not always interested in items disappearing from query

the downside &#x2013; having to keep the state :(  




## [TW](http://twitter.com/karlicoss/status/1047228539156750336) at `[2018-10-02]` А кто-нибудь знает тулы типа <https://t.co/EbpbNZWQFC> , но чтобы туда можно было вбить грубо говоря любую поисковую кверю, или API (например reddit/github); и оно отслеживало результаты?



### `[2019-10-02]` huh




## `[2020-06-22]` [I feel the same. So many cool things I'd love to learn about, but not enough tim&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23018081)      [[pkm]] [[axol]]

    I feel the same. So many cool things I'd love to learn about, but not enough time.




# Similar/existing projects





## `[2020-03-03]` [Show HN: Mailbrew – Automated Email Digests from HN, RSS, Reddit, Twitter](https://news.ycombinator.com/item?id=22474282)

<https://mailbrew.com/>  




## `[2019-12-26]` awesome-selfhosted/awesome-selfhosted: A list of Free Software network services and web applications which can be hosted locally. Selfhosting is the process of hosting and managing applications instead of renting from Software-as-a-Service providers

<https://github.com/awesome-selfhosted/awesome-selfhosted>  

    Search Engines




## trackreddit only two subscriptions

wanted lifelogging  
trackreddit  




## tool to search on reddit or even custom services? special ordering ('least likely' for showing least occuring subreddits). could also do it on rust?      [[pkm]]

searched as 'keyword monitoring tool'  
tried searching on reddit, but nothing really useful..  
<https://github.com/trulia/thoth> &#x2013; unclear what it's doing  

keyword tracking (SERP) &#x2013; not sure if an overkill..  


### `[2018-11-06]` just implement a provider for kibitzr?


### rust? 




# \* Make it more user friendly





## add axol doctor config      [[project]]

also axol doctor to check individual providers + reuse in tests  




## rely on user config dirs




## provide an asci diagram for crawler + report + feed reader?




# \* Blacklisting





## maybe button to ban user? it would write to config or something? maybe I can even use some public API constructor?




## I suppose pouchdb would be perfect for blacklisting      [[couchdb]]




## for blacklisting, instead could just apply custom per-user classes? or even edit them. that would allow to highlight properly




## yeah, blacklisting could both update backend and hide locally




## `[2019-04-15]` axol results for reddit<sub>pkm</sub>, rendered at Fri 12 Apr 2019 05:07

reddit<sub>pkm.html</sub>  
shit. need to ignore the weapons subreddits  
I think generally, my tools needs to have a database&#x2026;  




## shit, top lifelogging tweets are on japanese&#x2026;      [[twitter]]




## would be interesting to ignore links I already visited from results. It can even be done automatically&#x2026;.      [[promnesia]] [[axol]]




## huh, quite a few bots on reddit?      [[reddit]]

aznc<sub>bot</sub>  
bprogramming even maybe?  
autotldr  
tabledresser  




## huh, lots of stuff from twitter is just garbage. need a good way of suppressing it&#x2026;      [[axol]] [[twitter]]



### `[2020-01-01]` twitter<sub>mypy</sub> (211) - Miniflux

<https://axol.karlicoss.xyz/feed/53/entries>  

    /mypy1031


### `[2020-01-01]` twitter<sub>mypy</sub> (211) - Miniflux

<https://axol.karlicoss.xyz/feed/53/entries>  

    /aymk_mypy/status/1211970059205107712 All
    twitter_mypy 7 hours ago Original @Witch_Astaroth みどりさん！この垢にしてから相互になった方の中では割と話せたと思ってます笑 来年もよろしくお願いします！


### `[2020-01-01]` twitter<sub>mypy</sub> (111) - Miniflux

<https://axol.karlicoss.xyz/feed/53/entries>  

    /mypy2424/status/1211845733210443778 All
    twitter_mypy 7 hours ago Original 事実でも噂でも、クズとかいうやつお前はその人より努力してからいえよな〜って思うよ！！！！！ 好きな


### `[2020-01-01]` twitter<sub>mypy</sub> (111) - Miniflux

<https://axol.karlicoss.xyz/feed/53/entries>  

    /soe1113/status/741281801323175936 All
       twitter_mypy 7 hours ago O


### `[2020-01-03]` twitter<sub>lifelogging</sub> (20) - Miniflux

<https://axol.karlicoss.xyz/feed/52/entries>  

    /jager_atami/status/24390787028 All
    twitter_lifelogging 2 days ago Original #udetate #lifelogging 陶房で壺割り 12 個 201


### `[2020-01-03]` twitter<sub>quantified</sub><sub>self</sub> (36) - Miniflux

<https://axol.karlicoss.xyz/feed/55/entries>  

    /hiperesoterismo/status/1212803558203985920 All
        twitter_quantified_self 4 hours ago Original mis únicos 4 moodspic.twitter.com/5RgPiKKhMx ★




# What would be a good UI for axol?





## I really need some sort of proper frontend browser for it&#x2026;




## would be nice to have some html dashboard, so it's easy to blacklist terms?




## need a UI to easily add items to axol. e.g. Alexei Kitaev

maybe some simple cmdline available from anywhere. or org mode as source?  




## use metabase or something? could use a column to mark as seen? would be much easier than rss




## dunno about rss interface&#x2026; really need a more efficient way of processing content, reordering, etc




# Queries 





## search for 'data export' or something?



### `[2019-12-07]` not much on reddit for 'data liberation:


### `[2020-03-10]` 'data export' looks promising on github




## `[2020-01-12]` github.com/karlicoss - Twitter Search / Twitter      [[self]]

<https://twitter.com/search?q=github.com%2Fkarlicoss&src=typed_query&f=live>  


### `[2020-03-10]` right, it looks quite reasonable to have


-   `[2020-11-30]` very few results though


### `[2020-03-30]` All | Search powered by Algolia

<https://hn.algolia.com/?dateRange=all&page=0&prefix=true&query=github.com%2Fkarlicoss&sort=byPopularity&type=story>  




## `[2020-01-30]` my. package | beepb00p      [[postprivacy]] [[qs]] [[toread]]

<https://beepb00p.xyz/mypkg.html>  

    Interesting experiment! Thanks for sharing :-) You might find this person's musings about such experiments interesting: https://www.plomlompom.de/index.en.html#topic_postprivacy


### `[2020-03-01]` axol it




## `[2019-02-15]` What Universal Human Experiences Are You Missing Without Realizing It? | Slate Star Codex      [[mind]]

-   State "STRT"      from "TODO"       `[2019-04-13]`  
    <https://slatestarcodex.com/2014/03/17/what-universal-human-experiences-are-you-missing-without-realizing-it/>

search this post on reddit or something  


### `[2019-04-22]` actually even found something interesting on gh..

<https://github.com/search?q=what-universal-human-experiences-are-you-missing-without-realizing-it&type=Code>  
although, it's code search, not repo search  


### `[2019-04-22]` so trying to google that query

if looking for past month, that basically results in random keywords  
what universal human experiences are you missing without realizing it  


### `[2019-06-13]` yeah, twitter feed is not too huge, so could subscribe to it




## `[2019-06-29]` <https://github.com/hypotext/notation> - Twitter Search

<https://twitter.com/search?q=https%3A%2F%2Fgithub.com%2Fhypotext%2Fnotation&partner=Firefox&source=desktop-search>  


### `[2019-08-09]` axol this?


-   `[2019-08-25]` or aaxol for twitter? although doesn't seem to be posted often




## `[2020-01-09]` karlicoss/cachew - Twitter Search / Twitter      [[cachew]]

<https://twitter.com/search?q=karlicoss%2Fcachew&partner=Firefox&source=desktop-search>  




## `[2020-08-24]` [All | Search powered by Algolia](https://hn.algolia.com/?dateRange=all&page=0&prefix=true&query=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FNoon_Universe&sort=byPopularity&type=all) Noon Universe search




## mypy &#x2013; exclude mypython; prioritize topics      [[mypy]]




## sleep tracking      [[sleep]] [[qs]]




## add bret victor?      [[bretvictor]]



### `[2019-06-13]` uh. need a proper interface for it


-   `[2019-06-13]` what's the quickest possible way to create guis? still gonna be python config, right? perhaps self-checking!

    
    -   `[2019-06-15]` ok, just main function sounds ok..




## ted chiang &#x2013; pretty nice to search on twitter      [[tedchiang]]




## complex numbers group; argonov; transhumanism?      [[argonov]]



### `[2019-06-15]` youtube.com/watch?v=YrXk2buqsgg

can find some interesting stuff on twitter..  


### `[2019-07-28]` "виктор аргонов" got some good results on twitter




## kobo; spaced repetition?      [[spacedrep]]



### `[2019-12-07]` eh, kobo not so interesting..




## `[2018-08-25]` scott alexander unsong - Twitter Search

<https://twitter.com/search?f=tweets&vertical=default&q=scott%20alexander%20unsong&src=typd&lang=en-gb>  


### could add this to my twitter poller thing (again, via API)  or kibitzr?




## karlicoss!       [[self]]



### `[2019-06-15]` doesn't look much on pinboard&#x2026;


### `[2019-12-07]` not much interesting




## cancel scott alexander search alert




## set up alerts for nutrition stuff




## add "lagrangian mechanics"???      [[lagrangian]]



### `[2020-11-30]` or 'Hamiltonian'? at least on HN




## `[2020-03-09]` #promnesia

    GitHub - karlicoss/promnesia - Another piece of your extended mind

search on pinboard? or even axol..  




## kedr livansky      [[kedr]]




## exobrain?       [[exobrain]]




## `[2020-05-01]` [Pinboard bookmarks tagged eeg](https://pinboard.in/t:eeg)




## `[2020-05-01]` [Pinboard bookmarks tagged km](https://pinboard.in/t:km)      [[pkm]]




## memex? esp github      [[memex]]




## george hotz?




## add mypy to search??




## `[2019-10-01]` tried aaxol for



### "pocket export"


### "data liberation"




## pkm for twitter can probably be removed&#x2026;




## initial query&#x2026;      [[mypy]]

mypy  -from:mypy2424  -from:mypy1031 -from:aymk<sub>mypy</sub> -to:aymk<sub>mypy</sub> -from:mypy0229  

ugh, not sure how convenient it'd be to filter this shit  




## cleanup 'extended mind' &#x2013; certainly lots of crap in the database      [[twitter]]




## hmm, beepb00p.xyz isn't resolving anything?      [[self]] [[twitter]]




## `[2019-12-02]` axol results for hackernews<sub>pkm</sub>, rendered at 02 Dec 2019 11:05

axol/summary/hackernews<sub>pkm.html</sub>  

    Personal Knowledge database




## `[2019-12-02]` axol results for hackernews<sub>pkm</sub>, rendered at 02 Dec 2019 11:05

axol/summary/hackernews<sub>pkm.html</sub>  

    Personal knowledge base




## subscribe to more news on QS, BCI and gadgets      [[qs]]

-   State "DONE"       from "STRT"      `[2019-04-22]`


### regular? 


### brain-computer interface      [[bci]]




# Sources 





## wonder if I could search among hypothesis users&#x2026;      [[hypothesis]]



### `[2019-06-15]` eh, search is a bit weird&#x2026;




## could add google search too I suppose.. but that's def lowest priority




## implement for reddit. release reddit/github searchers (as library, then import and use)




## youtube? could search quantified self at least



### `[2019-07-20]` eh, tried few queries and does't look that result appear that often&#x2026;




## World be great to search in comments      [[axol]] [[reddit]]




## hypothesis 



### `[2019-07-28]` not that many results on pkm/quantified self..


### `[2019-07-28]` more on spaced repetition and ted chiang




## `[2019-07-28]` Schedule - pushshift.io

<https://pushshift.io/schedule/>  

    Current Schedule
        April comments should be available around May 20 ,2018.




## `[2019-07-28]` New API endpoint &#x2013; Now you can search comments! : redditdev

<https://www.reddit.com/r/redditdev/comments/3fv8vv/new_api_endpoint_now_you_can_search_comments/>  

    New API endpoint -- Now you can search comments!




## for google search, only notify about new results; not about changes. wonder how?




## `[2019-12-28]` Search Reddit Comments by User

<https://redditcommentsearch.com/>  

    Search through comments of a particular reddit user.




## `[2020-01-11]` pushshift/api: Pushshift API

<https://github.com/pushshift/api>  




## duckduckgo? 




## `[2019-12-01]` Pushshift Reddit Search      [[reddit]] [[scrape]]

<https://redditsearch.io/?term=beepb00p.xyz&dataviz=false&aggs=false&subreddits=&searchtype=posts,comments&search=true&start=0&end=1575221715&size=100>  




## `[2019-12-15]` hacker-news-favorites-api/main.js at master · reactual/hacker-news-favorites-api

<https://github.com/reactual/hacker-news-favorites-api/blob/master/src/main.js>  

    const x = require('x-ray')()

hmm, it's got 'paginate'?  




## `[2020-05-18]` [Hypothesis](https://hypothes.is/search?q=beepb00p.xyz)

eh need to run orger I guess? or axol!  




## could run HN more often      [[hackernews]]

also use more generic hooks?  




## `[2020-05-03]` [[<https://grep.app/search?q=import%20my%5C..%2A%24&regexp=true&filter>[lang][0]=Python][import my\\..\*$ - grep.app]]




# CI/testing 





## HN is very quick, so prob really good to test on (even on CI)




# Sort tags by number of total occurences?




# Use cachew and keep stuff as blobs with id      [[cachew]]

Not sure if I should overwrite or update? Could decide later and query with unique ids to start with?  




# warn when there are too many atom items?




# suppress some feeds in the config?




# `[2020-11-21]` [Show HN: I made an alternative to Google Alerts that listens to social media](https://news.ycombinator.com/item?id=25161117)

<https://www.pmalerts.com/>  




## `[2020-12-05]` eh, demands to register etc




# shit, seems that the timestamps are wrong and also I got the link wrong

might need to work on this: axol/databases/twitter<sub>extended</sub><sub>mind.sqlite</sub>  




# Maybe record a video on the phone ?      [[demo]]




# maybe check crawled pinboard users for interesting tags/links?





## `[2019-06-15]` yeah, need to make this bit more effecient..




# maybe, summary and 'rendered' are really sort of the same page? just different sorting&#x2026;




# Def interesting to see user stats




# Sort tags by number of total occurences?




# Maybe better way of normalising? E.g. look at ted<sub>chiang</sub>  and gq article. Display 'bumped' entries separately? Like a different way of sorting




# prepend # in tag?




# could search for interesting tags occurence without them actually being scraped




# might be good to do some sort of fuzzy grouping?

wonder what's an effecient way of doing it? sort of similarity connected components?  
/TheGoogleDotCom/status/915750443275444226  
Can Google's AI-powered Clips make people care about lifelogging? - TechCrunch <http://ift.tt/2wyk69G>  
2017-10-05 01:28 by TheGoogleDotCom  
/gauravndhankar/status/915750414774972416  
Can Google’s AI-powered Clips make people care about lifelogging? <http://dlvr.it/PsRpwK> pic.twitter.com/IAPiiqacKo  
2017-10-05 01:28 by gauravndhankar  
/animesh1977/status/915749491344596992  
Can Google’s AI-powered Clips make people care about lifelogging? <http://ift.tt/2xUwbaz>  




# would be interesting to have explorer for users that looks for some relevant taks/keywords?      [[pinboard]]




# Hmm also need real-time search and notify I guess?      [[hackernews]]




# Eh, better idea would be a tag subscription&#x2026;      [[mypy]]




# would be nice to have some efficient frontend + backend thing      [[timeline]]





## `[2019-12-02]` hmmm. actually could do it in a twitter account??




## `[2019-12-04]` could ask on HN?      [[outbox]]




## `[2019-12-04]` or RSS?  <https://github.com/awesome-selfhosted/awesome-selfhosted#feed-readers>




# `[2019-12-24]` Edit Feed: beepb00p.xyz - Miniflux

<https://axol.karlicoss.xyz/feed/56/edit>  

    Scraper Rules
    Rewrite Rules
    Title Filter
    Content Filter




# `[2019-12-24]` Command Line Usage - Documentation

<https://miniflux.app/docs/cli.html>  

    miniflux -config-file /etc/miniflux.conf




# could make a filter to release items slowly? e.g. tweets with more than 10 likes, if update pops it up, then it ends up in the feed. although I need 'processed' entries




# `[2020-05-27]` [Axol: Personal automatic news feed – crawl Reddit/Twitter/HN and read as RSS | Hacker News](https://news.ycombinator.com/item?id=23321646)




# perhaps redefine everything in entities? and have relations &#x2013; people, subreddits, urls, tags, etc




# rename adhoc to 'search'?




# think about a special tag to mark stuff that should be autoimported in a similar manner my kibitzr thing worked




# some todos

-   [ ] move individual data sources to files within the repo.. not even submodules, too much hassle  
    if someone needs, they can just import axol.sources.src directly
-   [ ] cleanup the json shit.. ideally use some proper library
-   [ ] not sure what to do with RSS feeds.. but could start with HTML report generation
-   [ ] query language:  
    might be better to adopt  
    service:sub:query  
    e.g.  
    pinboard:tag:whatever  
    or  
    github:some query  
    not sure what to do with colons though.. but maybe think about this later. most won't support searching them anyway




# def should keep original results in the DB as far as possible




# to start with, only support exact queries? e.g. demand them in queries and mention that support for fuzzier might be added later




# think about multiple small databases vs one huge?

multiple small:  

-   easier to mess with/explore
-   easier concurrency
-   easier to remove from reports (although for that need to make sure it's really 1-1 correspondence with source and query? dunno)

single db:  

-   easier to bulk clean/somewhat easier to bulk normalise  
    although this would be kind of useless if I store raw json outputs
-   easier to do queries across multiple (e.g. associating users?)




# thinking about query language

how it could look in adhoc mode  
github:'scott alexander' twitter:'scott alexander'  

in config, allow something nicer like  
[twitter,github,reddit]:'scott alexander'  

or [twitter,github,reddit, pinboard]:['scott alexander', 'quantified self']  
pinboard:tag:scottalexander  

-   [ ] NOTE: echo twitter:'scott alexander' &#x2013; this is gonna get swallowed by bash&#x2026; suggest to always quote?
-   [ ] NOTE: treat " and ' the same? twitter does it&#x2026;
-   [ ] TODO: make sure that query parsing is defensive




# for people to try it out it really needs a simplest service possible they can run with docker? ideally without auth etc




# Track most active pinboard users? They might have interesting other stuff





## `[2019-07-20]` maybe, try to intersect known user's tags and see what they got in common?




# running under docker results in /app/axol/js/sorttable




# use different font?




# might need two pass algorithm? One for crawling, second for filtering?

e.g. I crawled quite a bit of pokemon crap, would be good to filter it?  




# related       [[pkm]] [[search]] [[degoogle]]




# `[2019-04-15]` Pinboard: network for karlicoss      [[pinboard]] [[axol]]

<https://pinboard.in/network/>  
shit&#x2026; too many tweets. I need a way to filter the network&#x2026;  




## `[2021-01-16]` in fact it's the most common request to pinboard author apparently




# spinboard: something's not right. e.g. try

querying *t:quantified-self  
<https://pinboard.in/t:quantified-self>*  
spinboard gives 220 total results. however, on the first page there are 50&#x2026;  
scraper is missing something?  

eh. sooo, there are no dupes even!! BS4 actually sees only 20 per page (pinboard still gives us '50' in the next url).  
whereas chrome does show up 50 entries; but if you go to the second page they are gonna overlap.  




## must be some pinboard bug??      [[pinboard]]




# `[2019-11-06]` classes — classes 0.1.0 documentation

<https://classes.readthedocs.io/en/latest/>  




## `[2020-02-15]` hmm, somethihg  I was trying to do in axol?&#x2026;      [[axol]]




# doesn't look active. all top results are from 2017      [[axol]] [[upspin]]




# `[2019-09-04]` ScriptSmith/socialreaper: Social media scraping / data collection library for Facebook, Twitter, Reddit, YouTube, Pinterest, and Tumblr APIs      [[reddit]] [[scrape]] [[axol]]

<https://github.com/ScriptSmith/socialreaper>  

    Reddit
    Get the top 10 comments from the top 50 threads of all time on reddit




## `[2020-05-16]` ok, seems to be using real APIs, so overall I'm skeptical. but it's got a nice panel for tokens      [[exports]] [[jdoe]]




# pruning &#x2013; for now via sqlitedbbrowser? make sure it locks the db?      [[axol]]

