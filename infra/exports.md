
# Table of Contents

-   [related](#rltd) 
    -   [.](#625_741) [[silo]]
    -   [.](#741_857) [[infra]]
    -   [.](#857_973) [[backup]]
    -   [.](#973_1089) [[dataliberation]]
-   [\* motivation](#mtvtn) 
    -   [`[2020-03-17]` "GitHub blocked me and all my libraries"  https://news.ycombinator.com/item?id=22593595](#gthbblckdmndllmylbrrssnwsycmbntrcmtmd) 
    -   [motivation for using gdpr/takeouts: convenient when you're migrating off the service? don't have to worry about regular exports](#mtvtnfrsnggdprtktscnvnntwsrvcdnthvtwrrybtrglrxprts) 
    -   [`[2020-05-31]` Own your content on Social Media using the IndieWeb - YouTube](#swwwytbcmwtchvxsrzhgqwnyrcntntnsclmdsngthndwbytb) [[dataliberation]]
-   [\* implementation: goals/tips/practices](#mplmnttnglstpsprctcs) 
    -   [`[2019-10-03]` another big goal is having little operational overhead. I'd rather set up a (potentially elaborate) system once and tthen never have to update it and think how it works](#nthrbgglshvnglttlprtnlvrhhnnvrhvtpdttndthnkhwtwrks) [[exports]] [[infra]]
        -   [`[2019-10-03]` that involves automatic ci](#thtnvlvstmtcc) [[ci]]
        -   [`[2019-10-03]` continuous cloud sync](#cntnscldsync) [[cloud]]
        -   [`[2019-10-03]` automation/cron jobs for orger](#tmtncrnjbsfrrgr) [[dron]]
    -   [`[2021-03-04]` Importance of agnostic exports: ofter you start backing up before you process the data](#mprtncfgnstcxprtsftrystrtbckngpbfryprcssthdt) 
    -   [recommend checking the database to make sure it's got specific things you need](#rcmmndchckngthdtbstmksrtsgtspcfcthngsynd) [[backupchecker]]
    -   [synthetic style exports allow for defensive error handling &#x2013; you can at least get data from the last state](#synthtcstylxprtsllwfrdfnslngycntlstgtdtfrmthlststt) [[errors]]
    -   [eh. maybe get rid of colored logs for export process? presumably no one would look at them often](#hmybgtrdfclrdlgsfrxprtprcssprsmblynnwldlktthmftn) 
    -   [use submodule for common files, but release as a standalone package? I guess it's the best of both](#ssbmdlfrcmmnflsbtrlssstndlnpckggsststhbstfbth) 
    -   [`[2020-01-01]` ChromeDevTools/devtools-protocol: Chrome DevTools Protocol](#chrmdvtlsdvtlsprtclchrmdvtlsprtcl) [[exports]] [[scrape]]
    -   [`[2020-04-19]` open files using utf-8 encoding (fixes #5) by miguelrochefort · Pull Request #6 · karlicoss/rexport](#sgthbcmkrlcssrxprtpllflsplrchfrtpllrqstkrlcssrxprt) 
    -   [backup-wrapper is a more generic tool&#x2026; basically running arb command and saving output with pattern](#bckpwrpprsmrgnrctlbscllyrgrbcmmndndsvngtptwthpttrn) 
    -   [thinking about data providers](#thnkngbtdtprvdrs) [[dataliberation]]
        -   [most users won't care about keeping historic data? Or maybe not keeping data at all? jsut provide lambda?](#mstsrswntcrbtkpnghstrcdtrmybntkpngdttlljstprvdlmbd) 
        -   [most users won't have cron set up?](#mstsrswnthvcrnstp) 
        -   [to backup, use some python patternt library?](#tbckpssmpythnpttrntlbrry) 
        -   [example how it could work:](#xmplhwtcldwrk) 
    -   [dashboard for tokens + expose json or something so any language can have bindings](#dshbrdfrtknsxpsjsnrsmthngsnylnggcnhvbndngs) [[infra]] [[exports]]
        -   [`[2020-04-12]` add this to myinfra repository??](#ddthstmynfrrpstry) 
        -   [`[2020-05-27]` dunno, I'm a bit tired and not as motivated to build it&#x2026; but could post so someone else picks up](#dnnmbttrdndntsmtvtdtbldtbtcldpstssmnlspcksp) [[toblog]]
    -   [ok, exposing a stream is sort of good? and then filtering? makes it easier to use synthetic exports](#kxpsngstrmssrtfgdndthnfltrngmkstsrtssynthtcxprts) [[hpi]] [[exports]] [[dal]]
-   [\* twitter](#twttr) [[twitter]]
    -   [hmm. links that you get through search or API are shortened?](#hmmlnksthtygtthrghsrchrprshrtnd) [[linkrot]] [[twitter]] [[twint]]
        -   [`[2020-04-28]` shit.. also RTs are shortened?? so I need to get retweets properly?](#shtlsrtsrshrtndsndtgtrtwtsprprly) 
    -   [`[2021-01-19]` bisguzar/twitter-scraper: Scrape the Twitter Frontend API without authentication.](#sgthbcmbsgzrtwttrscrprbsgthtwttrfrntndpwthtthntctn) [[twitter]] [[exports]]
    -   [twint itself should work as incremental export&#x2026; and then DAL should combine](#twnttslfshldwrksncrmntlxprtndthndlshldcmbn) [[twint]]
    -   [`[2019-07-28]` jonbakerfish/TweetScraper: TweetScraper is a simple crawler/spider for Twitter Search without using API](#sgthbcmjnbkrfshtwtscrprjnlrspdrfrtwttrsrchwthtsngp) [[twitter]]
        -   [`[2021-02-09]` doesn't work, this error :( https://github.com/bisguzar/twitter-scraper/issues/168](#dsntwrkthsrrrsgthbcmbsgzrtwttrscrprsss) 
    -   [talon databases (lots of them!)](#tlndtbssltsfthm) [[hpi]] [[android]]
    -   [`[2019-07-29]` taspinar/twitterscraper: Scrape Twitter for Tweets](#sgthbcmtspnrtwttrscrprtsptwttrscrprscrptwttrfrtwts) 
        -   [`[2021-02-09]` https://github.com/taspinar/twitterscraper/issues/344 broken as well](#sgthbcmtspnrtwttrscrprsssbrknswll) 
    -   [err, new twitter exports are half gig each?](#rrnwtwttrxprtsrhlfggch) 
    -   [twint: possibly missing reply things (with 'at')](#twntpssblymssngrplythngswtht) [[twint]] [[hpi]]
-   [\* hackernews](#hckrnws) [[hackernews]]
    -   [`[2020-04-05]` Our plan is for the next version of HN's API to simply serve a JSON version of e&#x2026; | Hacker News](#rplnsfrthnxtvrsnfhnsptsmplysrvjsnvrsnfhckrnws) [[hackernews]]
    -   [`[2020-04-07]` Profile: karlicoss | Hacker News](#prflkrlcsshckrnws) 
    -   [`[2020-04-29]` need to mirror HN&#x2026;](#ndtmrrrhn) [[hackernews]] [[exports]]
    -   [materialistic &#x2013; 'read' table](#mtrlstcrdtbl) [[promnesia]]
    -   [`[2021-03-05]` it's impresive that pretty much every tool for exporting has some flaws](#tsmprsvthtprttymchvrytlfrxprtnghssmflws) [[hackernews]]
    -   [HN data provider](#hndtprvdr) [[hpi]] [[orger]] [[promnesia]]
-   [\* google takeout/other google data](#ggltktthrggldt) [[takeout]]
    -   [wonder if it's possible to get watch position?](#wndrftspssbltgtwtchpstn) [[takeout]] [[youtube]]
    -   [automating login & downloading](#tmtnglgndwnldng) 
        -   [`[2019-09-28]` life-vault/selenium<sub>takeout.py</sub> at master · ThorbenJensen/life-vault https://github.com/ThorbenJensen/life-vault/blob/master/src/takeout/selenium\_takeout.py](#lfvltslnmtktpytmstrthrbnjvltblbmstrsrctktslnmtktpy) 
        -   [automating google drive](#tmtngggldrv) [[takeout]] [[backup]] [[exports]]
        -   [automate google takeouts?](#tmtggltkts) 
    -   [`[2021-01-10]` Hypothesis](#shypthssbfmwlhftsmmmqhypthss) [[takeout]]
    -   [could sync mini-takeouts? with only necessary stuff picked from them](#cldsyncmntktswthnlyncssrystffpckdfrmthm) [[takeout]]
    -   [youtube watch history &#x2013; should be accumulated from multiple takeouts](#ytbwtchhstryshldbccmltdfrmmltpltkts) [[youtube]]
    -   [`[2019-06-11]` eh, recompressing to .tar.xz only saved 100 mb](#hrcmprssngttrxznlysvdmb) [[takeout]]
    -   [ugh, also when it's too large, they split archive in two](#ghlswhntstlrgthyspltrchvntw) [[takeout]]
    -   [also disappearing Disover/Myacvitiy??](#lsdspprngdsvrmycvty) [[takeout]]
    -   [`[2020-04-23]` I've found Google Takeouts to silently remove old data | beepb00p](#sbpbpxyztktdtgnhtmlvfndggltktstslntlyrmvlddtbpbp) 
    -   [`[2020-04-24]` Takeout/My Activity/Search data is limited to last 10 years. Please remove limit - Google Search Community](#sspprtgglcmwbsrchfrmgtjjmyrsplsrmvlmtgglsrchcmmnty) 
    -   [`[2020-04-29]` > I’ve already pulled down my 2-300GB Google Photos archive How? I've tried sev&#x2026; | Hacker News](#snwsycmbntrcmtmdvlrdyplldglphtsrchvhwvtrdsvhckrnws) 
    -   [`[2020-05-04]` I replied to a similar point about hashing here - https://news.ycombinator.com/i&#x2026; | Hacker News](#snwsycmbntrcmtmdrpldtsmlrhnghrsnwsycmbntrcmhckrnws) 
    -   [`[2020-01-01]` perkeep/gphotos-cdp: This program uses the Chrome DevTools Protocol to drive a Chrome session that downloads your photos stored in Google Photos.](#prkpgphtscdpthsprgrmssthctdwnldsyrphtsstrdngglphts) [[scrape]]
    -   [`[2019-06-28]` After hoarding over 50k YouTube videos, here is the youtube-dl command I settled on. : DataHoarder](#ftrhrdngvrkytbvdshrsthytbdlcmmndsttldndthrdr) 
    -   [`[2020-01-01]` perkeep/gphotos-cdp: This program uses the Chrome DevTools Protocol to drive a Chrome session that downloads your photos stored in Google Photos. https://github.com/perkeep/gphotos-cdp](#prkpgphtscdpthsprgrmssthcglphtssgthbcmprkpgphtscdp) 
-   [\* emfit sleep tracker](#mftslptrckr) [[emfit]]
    -   [`[2018-08-18]` Emfit has local API; would be nice to use it&#x2026;](#mfthslclpwldbnctst) [[emfit]]
        -   [`[2020-09-11]` sanielfishawy/emfit<sub>data</sub><sub>getter</sub>: Gets heart rate and respiration rate from an Emfit QS device on the same local network.](#sgthbcmsnlfshwymftdtgttrsfrmnmftqsdvcnthsmlclntwrk) [[emfit]]
    -   [`[2019-12-17]` downloadEmfitAPI.py https://gist.github.com/vanne02135/6901cc2b92315881080d0ce0f07c1a17](#dwnldmftppysgstgthbcmvnnccbdcfc) 
    -   [ugh. maybe autorefresh the token? Fuckig hell.](#ghmybtrfrshthtknfckghll) [[emfit]]
        -   [`[2021-02-06]` I think I ended up just using login + password. meh](#thnknddpjstsnglgnpsswrdmh) 
    -   [hmm, with emfit can code some sort of feedback tool which signals me to move when emfit loses signal](#hmmwthmftcncdsmsrtffdbckthchsgnlsmtmvwhnmftlsssgnl) [[emfit]]
    -   [`[2020-05-29]` emfit API didn't work for about three days straight&#x2026;](#mftpddntwrkfrbtthrdysstrght) [[emfit]] [[backup]]
    -   [`[2019-12-21]` samuelmr/emfit-qs: Unofficial Node client for Emfit QS](#smlmrmftqsnffclndclntfrmftqs) 
-   [\* bluemaestro temperature sensor](#blmstrtmprtrsnsr) [[bluemaestro]]
    -   [figure out bluemaestro, make sure all merged](#fgrtblmstrmksrllmrgd) [[bluemaestro]]
    -   [actually wonder if I can connect it to computer?](#ctllywndrfcncnnctttcmptr) [[bluemaestro]]
    -   [merge bluemaestros, plot separate environmental dashboard?](#mrgblmstrspltsprtnvrnmntldshbrd) [[dashboard]]
    -   [automate, about how I back up bluemaestro data](#tmtbthwbckpblmstrdt) [[toblog]]
    -   [`[2019-09-29]` yeah, could elaborate on backing up android data, could be quite generic?](#yhcldlbrtnbckngpndrddtcldbqtgnrc) [[android]]
-   [\* reddit](#rddt) [[reddit]]
    -   [I think cool fact should just be converted into org mode from backups (merged!) but generally there is no point capturing them?](#thnkclfctshldjstbcnvrtdntbtgnrllythrsnpntcptrngthm) [[reddit]]
        -   [`[2019-09-10]` er, I guess for orger need to extract a simple reddit provider that just merges various timestamped backups?](#rgssfrrgrndtxtrctsmplrddtthtjstmrgsvrstmstmpdbckps) 
    -   [I guess just rely on bleanser instead after all? Just make it less spammy](#gssjstrlynblnsrnstdftrlljstmktlssspmmy) [[bleanser]] [[reddit]]
    -   [Check for deleted favorites](#chckfrdltdfvrts) [[reddit]]
        -   [`[2019-08-25]` yep, it def happens; promnesia triggers it](#yptdfhppnsprmnstrggrst) 
    -   [shit. need to bleanse reddit properly, otherwise looks like it's too much data&#x2026;](#shtndtblnsrddtprprlythrwslkslktstmchdt) [[reddit]]
    -   [basically, just go through stuff that doesn't exist anymore but was in favorites ever (and suppress errors for some of them)](#bscllyjstgthrghstffthtdsnrtsvrndspprssrrrsfrsmfthm) [[reddit]]
    -   [`[2020-01-11]` Getting Started — PRAW 3.6.0 documentation](#gttngstrtdprwdcmnttn) [[reddit]]
-   [\* browser history](#brwsrhstry) 
    -   [compress databases as xz? would same about half of space at least, even more on firefox databases](#cmprssdtbsssxzwldsmbthlffspctlstvnmrnfrfxdtbss) [[promnesia]]
        -   [`[2020-09-05]` probably not necessary with pruning](#prbblyntncssrywthprnng) 
    -   [cleanup firefox phone exports&#x2026;](#clnpfrfxphnxprts) 
    -   [firefox history &#x2013; db format has changed??](#frfxhstrydbfrmthschngd) [[hpi]] [[infra]]
    -   [firefox history &#x2013; could compress with zstd? seems like 30x compression](#frfxhstrycldcmprsswthzstdsmslkxcmprssn) [[promnesia]]
        -   [`[2020-06-10]` to start with &#x2013; simply compress locally once the db is synced, will think about doing something smarter later](#tstrtwthsmplycmprsslcllynllthnkbtdngsmthngsmrtrltr) 
    -   [firefox dev history](#frfxdvhstry) [[phone]]
    -   [`[2020-08-29]` seanbreckenridge/ffexport: export and interface with firefox history/visits and site metadata](#sgthbcmsnbrcknrdgffxprtsncwthfrfxhstryvstsndstmtdt) 
-   [\* hypothesis](#hypthss) [[hypothesis]]
    -   [hmm, 9000 limit? might be necessary to do synthetic export instead&#x2026;](#hmmlmtmghtbncssrytdsynthtcxprtnstd) [[hypothesis]]
    -   [Hypothesis API are cloned as well.](#hypthssprclndswll) [[hypothesis]]
        -   [`[2020-01-21]` fix in hypexport?](#fxnhypxprt) 
-   [\* github](#gthb) [[github]]
    -   [`[2020-02-01]` motivation for github backups](#mtvtnfrgthbbckps) [[exports]]
    -   [warn about large repos?](#wrnbtlrgrps) [[github]]
    -   [ghexport &#x2013; read times out](#ghxprtrdtmst) [[ghexport]]
    -   [500 error](#rrr) [[ghexport]]
    -   [backport old github backups to new format? should be enough to just wrap in 'events'](#bckprtldgthbbckpstnwfrmtshldbnghtjstwrpnvnts) [[backup]] [[timeline]] [[promnesia]]
    -   [github &#x2013; starred repos aren't updated??](#gthbstrrdrpsrntpdtd) 
-   [\* whatsapp](#whtspp) [[whatsapp]]
    -   [/data/data/com.whatsapp/databases/msgstore.db](#dtdtcmwhtsppdtbssmsgstrdb) [[whatsapp]]
    -   [`[2020-01-17]` MasterScrat/Chatistics: 💬 Python scripts to parse your Messenger, Hangouts, WhatsApp and Telegram chat logs into DataFrames.](#mstrscrtchtstcspythnscrpttsppndtlgrmchtlgsntdtfrms) [[whatsapp]]
    -   [`[2019-07-13]` tgalal/yowsup: The WhatsApp lib https://github.com/tgalal/yowsup](#tgllywspthwhtspplbsgthbcmtgllywsp) 
-   [\* stackexchange](#stckxchng) [[stackexchange]]
    -   [`[2019-09-01]` Usage of /users/{ids}/favorites <span class='http-method' title='expects a GET HTTP method'>GET</span> - Stack Exchange API](#sgfsrsdsfvrtsspnclssmthdtpctsgtmthdgtspnstckxchngp) [[promnesia]]
        -   [`[2019-09-16]` shit. seems that no way to get upvoted posts&#x2026; https://meta.stackexchange.com/questions/299264/how-to-get-the-list-of-all-posts-ive-upvoted-via-the-api](#shtsmsthtnwytgtpvtdpstssmwtgtthlstfllpstsvpvtdvthp) 
        -   [`[2019-09-16]` https://meta.stackexchange.com/questions/148008/how-can-i-see-comments-that-ive-upvoted](#smtstckxchngcmqstnshwcnscmmntsthtvpvtd) 
        -   [`[2019-09-16]` fuck. I guess I'm gonna have to scrape votes&#x2026; https://stackoverflow.com/users/706389/karlicoss?tab=votes](#fckgssmgnnhvtscrpvtssstckvrflwcmsrskrlcsstbvts) 
    -   [stackexchange &#x2013; there are comments in GDPR requested data](#stckxchngthrrcmmntsngdprrqstddt) [[stackexchange]]
    -   [stackexchange &#x2013; shit](#stckxchngsht) 
    -   [stackexchange &#x2013; need to figure out how to import remaining data&#x2026;](#stckxchngndtfgrthwtmprtrmnngdt) 
    -   [Today I would probably have tried parsing the Stack Exchange Data Dump instead.](#tdywldprbblyhvtrdprsngthstckxchngdtdmpnstd) 
        -   [`[2021-02-06]` hmm, it's actual dump of <span class="underline">all</span> comments&#x2026; bit too much I guess](#hmmtsctldmpfllcmmntsbttmchgss) 
    -   [hmm crashed on json decoding?](#hmmcrshdnjsndcdng) [[stexport]]
-   [\* mastodon](#mstdn) [[mastodon]]
    -   [`[2020-01-11]` kensanata/mastodon-backup: Archive your statuses, favorites and media using the Mastodon API (i.e. login required)](#knsntmstdnbckprchvyrsttssrtsndmdsngthmstdnplgnrqrd) 
    -   [zigg/grabby: tools for scraping your Mastodon account data](#zgggrbbytlsfrscrpngyrmstdnccntdt) [[mastodon]]
    -   [`[2019-12-29]` halcy/Mastodon.py: Python wrapper for the Mastodon ( https://github.com/tootsuite/mastodon/ ) API.](#hlcymstdnpypythnwrpprfrthmstdnsgthbcmttstmstdnp) [[mastodon]]
    -   [tusky android app keeps some history in tuskyDb](#tskyndrdppkpssmhstryntskydb) [[hpi]] [[mastodon]]
-   [\* pinboard](#pnbrd) [[pinboard]]
    -   [huh looks like pinboard is quite unstable with regards to backup&#x2026; unless the backup script is wrong or something?](#hhlkslkpnbrdsqtnstblwthrgssthbckpscrptswrngrsmthng) [[bleanser]]
    -   [`[2019-04-19]` Pinboard on Twitter: "Next question is, does a raw API call give the same results as the website? The API and website search engine run off of different indexes.… https://t.co/CZrLE7YNWo"](#pnbrdntwttrnxtqstnsdsrwpcrnfffdffrntndxsstcczrlynw) [[pinboard]]
-   [-------&#x2013;&#x2014; other data sources  ---------------](#thrdtsrcs) 
-   [Podcast addict data](#pdcstddctdt) 
-   [`[2020-07-31]` alexattia/Maps-Location-History: Get, Concatenate and Process you location history from Google Maps TimeLine](#sgthbcmlxttmpslctnhstrylxssylctnhstryfrmgglmpstmln) [[location]] [[timeline]] [[qs]]
-   [ok, so need to preserve all (incl.older) versions of notebooks? dunno feels a bit excessive](#ksndtprsrvllnclldrvrsnsfntbksdnnflsbtxcssv) [[timeline]] [[remarkable]]
-   [`[2020-10-25]` Garmin Connect](#scnnctgrmncmmdrndlysmmryhrtrtgrmncnnct) [[garmin]]
-   [`[2020-12-30]` Notice: This project is unmaintained · Issue #613 · fbchat-dev/fbchat](#sgthbcmfbchtdvfbchtsssntcrjctsnmntndssfbchtdvfbcht) [[facebook]]
-   [Need my email mirrored](#ndmymlmrrrd) [[email]]
    -   [`[2019-03-12]` I guess I want continuous. Not sure how to achieve that, perhaps some mail client in the background?](#gsswntcntnsntsrhwtchvthtprhpssmmlclntnthbckgrnd) 
-   [`[2019-06-13]` joeyates/imap-backup: Backup GMail (or other IMAP) accounts to disk](#jytsmpbckpbckpgmlrthrmpccntstdsk) [[email]]
-   [Bandcamp history](#bndcmphstry) 
    -   [`[2020-12-13]` https://bandcamp.com/developer no listening history though&#x2026;](#sbndcmpcmdvlprnlstnnghstrythgh) 
-   [hmm memrise personal data request is neat! It's got all you training sessions + learned words and phrases](#hmmmmrsprsnldtrqstsnttsgttrnngsssnslrndwrdsndphrss) [[publish]]
-   [do a full remarkable backup too?](#dfllrmrkblbckpt) [[remarkable]]
    -   [`[2020-11-27]` tech:ssh [reMarkableWiki]](#srmrkblwkcmtchsshtchsshrmrkblwk) 
-   [better docs on what to do on expiry](#bttrdcsnwhttdnxpry) [[monzo]]
-   [huh, thriva uses an api&#x2026;](#hhthrvssnp) 
-   [call history from my old(er?)  phones? (e.g. nokia)](#cllhstryfrmmyldrphnsgnk) 
-   [increase sample rate to 10 seconds maybe?](#ncrssmplrttscndsmyb) [[arbtt]]
-   [process old 'backups' repo?](#prcssldbckpsrp) 
-   [reading hr data](#rdnghrdt) [[wahoo]]
    -   [`[2020-10-09]` also tried gpsbabel, but it resulted in no data&#x2026; weird](#lstrdgpsbblbttrsltdnndtwrd) 
-   [`[2019-04-08]` python - Steam API get historical player count of specific game - Stack Overflow](#pythnstmpgthstrclplyrcntfspcfcgmstckvrflw) 
-   [Feedbin starred stuff](#fdbnstrrdstff) 
-   [`[2019-07-14]` fabianonline/telegram<sub>backup</sub>: Java app to download all your telegram data.](#fbnnlntlgrmbckpjvpptdwnldllyrtlgrmdt) 
-   [eh, should include older account? compare oldest and one of newer files..](#hshldncldldrccntcmprldstndnfnwrfls) [[monzo]]
-   [myshows: hmm, so looks like api v 1.8 is deprecated, for api 2.0 I'd need to email them. can just use raw jsons from existing backup script](#myshwshmmslkslkpvsdprctdftsrwjsnsfrmxstngbckpscrpt) 
-   [compress chrome histories? would require backup script to compress it I suppose&#x2026; maybe just go through them regularly and recompress](#cmprsschrmhstrswldrqrbckptgthrghthmrglrlyndrcmprss) 
-   [bookmarks limit through api???](#bkmrkslmtthrghp) [[instapaper]]
    -   [`[2020-01-04]` need to check historic exports and figure it out](#ndtchckhstrcxprtsndfgrtt) 
-   [gpslogger &#x2013; add to backup checker??](#gpslggrddtbckpchckr) [[location]]
-   [`[2020-10-03]` Statify: Pull your playlist and listening data from the Spotify API to a Sqlite database /r/coolgithubprojects](#srddtcmrclgthbprjctscmmntfyptsqltdtbsrclgthbprjcts) 
-   [monzo export: make sure it works with original repo..](#mnzxprtmksrtwrkswthrgnlrp) [[exports]] [[monzo]]
    -   [`[2019-12-29]` huh, actually the problem might be in saving \_token variable?](#hhctllythprblmmghtbnsvngtknvrbl) 
        -   [`[2019-12-29]` instead could just print it from disk? maybe even that is unnecessary?](#nstdcldjstprnttfrmdskmybvnthtsnncssry) 
-   [ugh, need to retrieve pinboard notes](#ghndtrtrvpnbrdnts) [[pinboard]] [[exports]]
-   [`[2019-04-23]` feedbin/feedbin-api: Feedbin API Documentation](#fdbnfdbnpfdbnpdcmnttn) [[feedbin]]
-   [`[2020-11-27]` Success Stories · tcgoetz/GarminDB Wiki](#sgthbcmtcgtzgrmndbwksccsstrssccssstrstcgtzgrmndbwk) [[garmin]]
-   [`[2020-12-19]` Importing your Goodreads & Accessing them with Open Library’s APIs](#sblgpnlbrryrgmprtngyrgdrdrdsccssngthmwthpnlbrrysps) 
-   [`[2020-06-24]` Telegram Now Lets You Export Your Chats, View Notification Exceptions | Technology News](#sgdgtsndtvcmppsnwstlgrmxpsvwntfctnxcptnstchnlgynws) [[telegram]]
-   [get off the messages stored in old format and make sure nothing  is missing, dedup?](#gtffthmssgsstrdnldfrmtndmksrnthngsmssngddp) [[vk]]
-   [shit, they stopped you from accessing messages api. fuck.](#shtthystppdyfrmccssngmssgspfck) [[vk]]
    -   [`[2019-03-08]` that's very generic trend. I think ultimately we just need better tools to scrape that](#thtsvrygnrctrndthnkltmtlywjstndbttrtlstscrptht) 
-   [Headspace stats](#hdspcstts) [[timeline]]
-   [.polar directory](#plrdrctry) [[timeline]]
-   [`[2019-09-02]` vincaslt/memparse: A Memrise courses parser https://github.com/vincaslt/memparse](#vncsltmmprsmmrscrssprsrsgthbcmvncsltmmprs) 
-   [skype call history?](#skypcllhstry) 
    -   [`[2020-04-19]` shit https://answers.microsoft.com/en-us/skype/forum/all/skype-api/e025d0f6-7ae4-4bc4-9d5a-b2d70136deab](#shtsnswrsmcrsftcmnsskypfrmllskyppdfbcdbddb) 
-   [amazon orders history](#mznrdrshstry) 
    -   [`[2018-05-04]` ugh, order history report is broken for the UK version :( https://www.amazon.co.uk/gp/help/customer/display.html?nodeId=202119330 wrote to support](#ghrdrhstryrprtsbrknfrthkvstmrdsplyhtmlnddwrttspprt) 
    -   [`[2019-02-23]` backups/amazon](#bckpsmzn) 
-   [ugh, bookmarks method in api is not exhaustive (elif item.get("type") == 'bookmark')](#ghbkmrksmthdnpsntxhstvlftmgttypbkmrk) [[instapaper]]
-   [`[2019-04-01]` Polar AccessLink Api Daily Activity Goal /r/Polarfitness](#srddtcmrplrftnsscmmntsbczsslnkpdlyctvtyglrplrftnss) 
-   [just reuse files dir? def no harm in it](#jstrsflsdrdfnhrmnt) [[telegram]]
-   [blinkist: scrape off my highlights](#blnkstscrpffmyhghlghts) 
    -   [`[2019-08-13]` eh, just copy responses manually?](#hjstcpyrspnssmnlly) 
    -   [`[2019-08-13]` huh, actually if webdriver could eavesdrop on json responses would be perfect](#hhctllyfwbdrvrcldvsdrpnjsnrspnsswldbprfct) 
    -   [`[2019-08-13]` post in on github&#x2026;](#pstnngthb) [[toblog]]
-   [export bitbucket](#xprtbtbckt) 
-   [feedbin](#fdbn) 
-   [`[2020-03-05]` signalnerve/roam-backup: Automated Roam Research backups using GitHub Actions and AWS S3](#sgnlnrvrmbckptmtdrmrsrchbckpssnggthbctnsndwss) 
-   [----------------------------------------------------](#48272_48369) 
-   [`[2020-02-03]` Data lake - Wikipedia](#dtlkwkpd) [[dal]] [[exports]]
-   [`[2020-04-21]` fucking hell. so materialistic export stopped working](#fcknghllsmtrlstcxprtstppdwrkng) [[phone]]
-   [start awesome-exports list?](#strtwsmxprtslst) [[exports]] [[publish]]
-   [script to grab files from downloads and move accodingly? e.g. for oyster statements](#scrpttgrbflsfrmdwnldsndmvccdnglygfrystrsttmnts) 
-   [TW at `[2017-01-21]` Играюсь с IMDB, думал придется beautiful soap доставать айтемы из вотчлиста, а там в стейте реакта лежит JSONка](#stwttrcmwbsttstwtиграюсьсамвстейтереакталежитjsnка) [[exports]]
-   [Post about various ways of data handling](#pstbtvrswysfdthndlng) [[toblog]] [[dataliberation]]
-   [`[2019-12-27]` 'hostage model' is a good term](#hstgmdlsgdtrm) [[toblog]] [[dataliberation]] [[sadinfra]]
-   [`[2020-01-15]` Hi, Camlistore author here. Andrew Gerrand worked with me on Camlistore too and&#x2026; | Hacker News](#hcmlstrthrhrndrwgrrndwrkdwthmncmlstrtndhckrnws) [[infra]] [[exports]]
-   [automatic date extraction? could work, e.g. for rescuetime](#tmtcdtxtrctncldwrkgfrrsctm) [[datetime]] [[backupchecker]]
-   [&#x2013;&#x2014; last housekeeping on `[2021-02-06]` --------](#lsthskpngn) 
-   [`[2020-04-13]` twintproject/twint: An advanced Twitter scraping & OSINT tool written in Python that doesn't use Twitter's API, allowing you to scrape a user's followers, following, Tweets and more while evading most API limitations.](#sgthbcmtwntprjcttwnttwntptwtsndmrwhlvdngmstplmttns) 
-   [`[2020-04-23]` MatthieuBizien/roam-to-git: Automatic RoamResearch backup to Git](#sgthbcmmtthbznrmtgtmtthbznrmtgttmtcrmrsrchbckptgt) 
-   [`[2020-04-28]` timgrossmann/InstaPy: 📷 Instagram Bot - Tool for automated Instagram interactions](#sgthbcmtmgrssmnnnstpytmgrrmbttlfrtmtdnstgrmntrctns) 
-   [right, so if you enable sync it seems to suck in history on the phone database? eh. messy](#rghtsfynblsynctsmstscknhstrynthphndtbshmssy) [[firefox]] [[exports]] [[promnesia]]
-   [crap&#x2026; android database has really high granulatity of events??](#crpndrddtbshsrllyhghgrnlttyfvnts) [[rescuetime]]
-   [`[2021-02-05]` Chiaki/VKBK: Инструмент для создания и синхронизации локального бэкапа вашего профиля ВКонтакте (Profile backup & synchronization tool for Vk.com)](#sgthbcmchkvkbkchkvkbkинстrflbckpsynchrnztntlfrvkcm) [[vk]] [[exports]]
-   [`[2021-02-07]` Against developer terms of service? · Issue #171 · Tyrrrz/DiscordChatExporter](#sgthbcmtyrrrzdscrdchtxprtsrvcsstyrrrzdscrdchtxprtr) 
-   [make it kinda smarter?](#mktkndsmrtr) [[backupchecker]]
-   [hmm, takeout has all tcx files?](#hmmtkthslltcxfls) [[endomondo]]
-   [hide praw logs unless interactive? too spammy in syslog](#hdprwlgsnlssntrctvtspmmynsyslg) [[infra]]
-   [hm nice podcast addict simply backs up its database](#hmncpdcstddctsmplybcksptsdtbs) [[exports]]
-   [Hmm maybe need to check for similar dst problems&#x2026; Basically mismatch between hr and sleep start/end?](#hmmmybndtchckfrsmlrdstprblymsmtchbtwnhrndslpstrtnd) [[emfit]]
-   [`[2021-02-25]` ryanmcgrath/twython: Actively maintained, pure Python wrapper for the Twitter API. Supports both normal and streaming Twitter APIs.](#sgthbcmrynmcgrthtwythnrynrtsbthnrmlndstrmngtwttrps) [[python]] [[twitter]]
-   [`[2021-02-04]` Privacy Policy - October 15, 2020 - Reddit](#swwwrddtnccmplcsprvcyplcymtnrqstsprvcyplcyctbrrddt) [[reddit]] [[exports]]
-   [`[2021-02-05]` Rapptz/discord.py: An API wrapper for Discord written in Python.](#sgthbcmrpptzdscrdpyrpptzdnpwrpprfrdscrdwrttnnpythn) [[discord]] [[exports]]
-   [`[2021-02-08]` Oura ring vs. Emfit QS (My detailed comparison) - What do you think? - Quantified Self / Sports, Physical Activity, and Fitness - Quantified Self Forum](#sfrmqntfdslfcmtrrngvsmftqclctvtyndftnssqntfdslffrm) [[emfit]] [[exports]]
-   [list the takeouts that are reduntant](#lstthtktsthtrrdntnt) [[takeout]] [[promnesia]]
-   [runnerup database file? could use existing computations perhaps?](#rnnrpdtbsflcldsxstngcmpttnsprhps) 
-   [maybe for DAL, follow the pattern of exposing a method to read single export?](#mybfrdlfllwthpttrnfxpsngmthdtrdsnglxprt) [[hpi]] [[exports]]
-   [Could utilize monzo categories for mine? I guess they could have errors.. Idk](#cldtlzmnzctgrsfrmngssthycldhvrrrsdk) [[monzo]]
-   [`[2021-03-10]` Quickstart — StackAPI 0.1.12 documentation](#sstckprdthdcsnltstsrqckstfrsltsqckstrtstckpdcmnttn) [[exports]]
-   [`[2021-03-07]` Exporting my own comment content from Disqus? · Discuss Disqus · Disqus](#sdsqscmhmdscssnchnnldscsscntntfrmdsqsdscssdsqsdsqs) [[disqus]] [[exports]]
-   [`[2021-03-23]` Your eBay data](#swwwsrwbbycksryrbydt) [[ebay]]
-   [possible to have exactly same events with different API ids???](#pssblthvxctlysmvntswthdffrntpds) [[github]]
-   [`[2021-04-18]` exobrain/data/exports<sub>gdpr</sub> at master · seanbreckenridge/exobrain](#sgthbcmsnbrcknrdgxbrntrmstsgdprtmstrsnbrcknrdgxbrn) [[exports]] [[gdpr]]
-   [highlights are in UTC](#hghlghtsrntc) [[remarkable]] [[koreader]]

I need data exports to build tools around my personal data, and the actual process of exporting it from a silo is the first step.  

After I export it I use it to build a ['data mirror'](https://beepb00p.xyz/sad-infra.html#data_mirror).  

Here I mostly keep the notes about the data I haven't finished exporting.  
The ones I have already/mostly finished are mentioned here:  

-   [Map of my infrastructure](https://beepb00p.xyz/myinfra.html)
-   [What data on myself I collect and why?](https://beepb00p.xyz/my-data.html)




# related 





## .       [[silo]]




## .       [[infra]]




## .       [[backup]]




## .       [[dataliberation]]




# \* motivation

Similar to [backups](backups.md).  




## `[2020-03-17]` "GitHub blocked me and all my libraries"  <https://news.ycombinator.com/item?id=22593595>




## motivation for using gdpr/takeouts: convenient when you're migrating off the service? don't have to worry about regular exports




## `[2020-05-31]` [Own your content on Social Media using the IndieWeb - YouTube](https://www.youtube.com/watch?v=X3SrZuH00GQ)      [[dataliberation]]




# \* implementation: goals/tips/practices





## `[2019-10-03]` another big goal is having little operational overhead. I'd rather set up a (potentially elaborate) system once and tthen never have to update it and think how it works      [[exports]] [[infra]]





### `[2019-10-03]` that involves automatic ci      [[ci]]




### `[2019-10-03]` continuous cloud sync      [[cloud]]




### `[2019-10-03]` automation/cron jobs for orger      [[dron]]




## `[2021-03-04]` Importance of agnostic exports: ofter you start backing up before you process the data




## recommend checking the database to make sure it's got specific things you need      [[backupchecker]]




## synthetic style exports allow for defensive error handling &#x2013; you can at least get data from the last state      [[errors]]




## eh. maybe get rid of colored logs for export process? presumably no one would look at them often




## use submodule for common files, but release as a standalone package? I guess it's the best of both




## `[2020-01-01]` ChromeDevTools/devtools-protocol: Chrome DevTools Protocol      [[exports]] [[scrape]]

<https://github.com/ChromeDevTools/devtools-protocol>  




## `[2020-04-19]` [open files using utf-8 encoding (fixes #5) by miguelrochefort · Pull Request #6 · karlicoss/rexport](https://github.com/karlicoss/rexport/pull/6/files)

apply this to export helper&#x2026;  




## backup-wrapper is a more generic tool&#x2026; basically running arb command and saving output with pattern




## thinking about data providers      [[dataliberation]]

Easiest option is just to have separate scripts to run regularly?  




### most users won't care about keeping historic data? Or maybe not keeping data at all? jsut provide lambda?

so the backup script could provide TODO  




### most users won't have cron set up?

so need a way to trigger backup from promnesia indexer itself? Fairly easy to achieve as it's all just python code?  




### to backup, use some python patternt library?




### example how it could work:

in promnesia  

    def index_reddit():
        from exporters.reddit import export
        # TODO?
        return




## dashboard for tokens + expose json or something so any language can have bindings      [[infra]] [[exports]]

might be annoying to implement token retrieval on JS only?  




### `[2020-04-12]` add this to myinfra repository??




### `[2020-05-27]` dunno, I'm a bit tired and not as motivated to build it&#x2026; but could post so someone else picks up      [[toblog]]




## ok, exposing a stream is sort of good? and then filtering? makes it easier to use synthetic exports      [[hpi]] [[exports]] [[dal]]




# \* twitter      [[twitter]]

Twitter is a big pain in the ass, they've become very hostile towards API access.  
Even the archives are somewhat incomplete (e.g. favorites lack some metadata).  

E.g. from [Apply for API — Twitter Developers](https://developer.twitter.com/en/application/intent)  

    Be thorough
    We need to completely understand your use case before we can approve it. So, please include as much detail as possible in your application.




## hmm. links that you get through search or API are shortened?      [[linkrot]] [[twitter]] [[twint]]





### `[2020-04-28]` shit.. also RTs are shortened?? so I need to get retweets properly?




## `[2021-01-19]` [bisguzar/twitter-scraper: Scrape the Twitter Frontend API without authentication.](https://github.com/bisguzar/twitter-scraper)      [[twitter]] [[exports]]




## twint itself should work as incremental export&#x2026; and then DAL should combine      [[twint]]

Even though Twint uses db, they seem to treat is as a temporary storage, so the schema might change.  
I'm also not super convinced by how reliable the code is (from quick glance), so would worry about data loss.  




## `[2019-07-28]` [jonbakerfish/TweetScraper: TweetScraper is a simple crawler/spider for Twitter Search without using API](https://github.com/jonbakerfish/TweetScraper)      [[twitter]]





### `[2021-02-09]` doesn't work, this error :( <https://github.com/bisguzar/twitter-scraper/issues/168>




## talon databases (lots of them!)      [[hpi]] [[android]]




## `[2019-07-29]` [taspinar/twitterscraper: Scrape Twitter for Tweets](https://github.com/taspinar/twitterscraper)

    One of the bigger disadvantages of the Search API is that you can only access Tweets written in the past 7 days. This is a major bottleneck for anyone looking for older past data to make a model from. With TwitterScraper there is no such limitation.




### `[2021-02-09]` <https://github.com/taspinar/twitterscraper/issues/344> broken as well




## err, new twitter exports are half gig each?




## twint: possibly missing reply things (with 'at')      [[twint]] [[hpi]]

compare tw-before.org (twint) and tw-after.org (twidump) in views  
retweets in twint are def missing  




# \* hackernews      [[hackernews]]





## `[2020-04-05]` Our plan is for the next version of HN's API to simply serve a JSON version of e&#x2026; | Hacker News      [[hackernews]]

<https://news.ycombinator.com/item?id=22788526>  

    Our plan is for the next version of HN's API to simply serve a JSON version of every page. I'm hoping to get to that this year.




## `[2020-04-07]` Profile: karlicoss | Hacker News

<https://news.ycombinator.com/user?id=karlicoss>  

    user:	karlicoss
    created:	August 25, 2016
    karma:	757

capture HN karma? maybe on all comments  




## `[2020-04-29]` need to mirror HN&#x2026;      [[hackernews]] [[exports]]




## materialistic &#x2013; 'read' table      [[promnesia]]

could also have 'exact' time notion and 'approximate' time &#x2013; when it's guessed from the file timestamp etc  




## `[2021-03-05]` it's impresive that pretty much every tool for exporting has some flaws      [[hackernews]]

don't have ci  

-   <https://github.com/davenicoll/hackernews>  
    -   doesn't even have main??
-   <https://github.com/romaintailhurat/hns>  
    -   uses pickle??
-   <https://github.com/amjd/HN-Saved-Links-Export>  
    -   too defensive
    -   writes to stdout
    -   can't be used as API




## HN data provider      [[hpi]] [[orger]] [[promnesia]]

<https://github.com/HackerNews/API>  
<https://hacker-news.firebaseio.com/v0/user/karlicoss.json?print=pretty> &#x2013; get user data  
extract 'submitted'  
<https://hacker-news.firebaseio.com/v0/item/25971799.json?print=pretty> &#x2013; comment  
<https://hacker-news.firebaseio.com/v0/item/25971380.json?print=pretty> &#x2013; type: "story"  
dunno if useful to keep scores over time?  
not sure if should dump everything in a single json? or split by files?  
can change later I guess  




# \* google takeout/other google data      [[takeout]]

Google Takeout doesn't have a proper API, and periodic expots are kind of annoying&#x2026; would be good to automate them.  

Another difficulty is that the data [seems to have a certain retention](https://beepb00p.xyz/takeout-data-gone.html),  
so you can't just take the latest takeout, for some data you need to merge all of them.  




## wonder if it's possible to get watch position?      [[takeout]] [[youtube]]




## automating login & downloading





### `[2019-09-28]` life-vault/selenium<sub>takeout.py</sub> at master · ThorbenJensen/life-vault <https://github.com/ThorbenJensen/life-vault/blob/master/src/takeout/selenium_takeout.py>




### automating google drive      [[takeout]] [[backup]] [[exports]]

-   ocamlfuse + script to move to desired location
-   basically that only requires you to request new archive occasionally




### automate google takeouts?

maybe release my module for 2FA separately?  
<https://github.com/ThorbenJensen/life-vault/blob/master/src/takeout/selenium_takeout.py>  




## `[2021-01-10]` [Hypothesis](https://hypothes.is/a/b-fmWlHEEeuiFt9suM9mMQ)      [[takeout]]

    Seriously, check out ratarmount if you haven't. Since the Google Takeout spans multiple 50GB tgz files (I'm at ~14, not including Google Drive in the takeout), ratarmount is brilliant. It merges all of the tgz contents into a single folder structure so /path/a/1.jpg and /path/a/1.json might be in different tgz folders but are mounted in to the same folder.




## could sync mini-takeouts? with only necessary stuff picked from them      [[takeout]]




## youtube watch history &#x2013; should be accumulated from multiple takeouts      [[youtube]]




## `[2019-06-11]` eh, recompressing to .tar.xz only saved 100 mb      [[takeout]]




## ugh, also when it's too large, they split archive in two      [[takeout]]




## also disappearing Disover/Myacvitiy??      [[takeout]]

    20180807 My Activity/Discover/MyActivity.html                                    20190523 20181015 My Activity/Discover/MyActivity.html                                    20190522 20181213 My Activity/Discover/MyActivity.html                                    20200122




## `[2020-04-23]` [I've found Google Takeouts to silently remove old data | beepb00p](https://beepb00p.xyz/takeout-data-gone.html)

huh, so with my script to search takeout duplicates, I've figured out that from 2015 at least Search/MyActivity.html hasn't been erased? interesting  
but looks like Chrome/MyActivity.html still being removed  




## `[2020-04-24]` [Takeout/My Activity/Search data is limited to last 10 years. Please remove limit - Google Search Community](https://support.google.com/websearch/forum/AAAAgtjJeM4qYYSPkPYJw8/?hl=en&gpf=%23!topic%2Fwebsearch%2FqYYSPkPYJw8%3Bcontext-place%3Dforum%2Fwebsearch)

    Takeout/My Activity/Search data is limited to last 10 years. Please remove limit




## `[2020-04-29]` [> I’ve already pulled down my 2-300GB Google Photos archive How? I've tried sev&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23015742)

    cuu508 1 hour ago [-]
    Takeout doesn't work in practice for bigger collections (archive creation routinely fails, timeouts while downloading, 50GB max size results in many splits)
    I've used this 3rd party tool and it worked OK: https://github.com/gilesknap/gphotos-sync/
    geekgonecrazy 1 hour ago [-]
    I forgot to mention this. But yes the export failed several dozen times. I believe I ended up doing in chunks. It was hard to get them off




## `[2020-05-04]` [I replied to a similar point about hashing here - https://news.ycombinator.com/i&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23032818)

    You're correct that the methods I described are a far cry from actually guaranteeing that the backup has no errors. In the same way that a unit test doesn't prove code is error-free, but _can_ justify increased confidence in the code, I'm interested in techniques that can justify increased confidence in my backups. Particularly in cases where I don't have direct access to the original data, and where exhaustively checking the data manually is too time-consuming to be worth it.

yes!  




## `[2020-01-01]` perkeep/gphotos-cdp: This program uses the Chrome DevTools Protocol to drive a Chrome session that downloads your photos stored in Google Photos.      [[scrape]]

<https://github.com/perkeep/gphotos-cdp>  

    In our original Perkeep issue, @bradfitz said that we might have to give up on APIs and resort to scraping, noting that the Chrome DevTools Protocol makes this pretty easy.




## `[2019-06-28]` After hoarding over 50k YouTube videos, here is the youtube-dl command I settled on. : DataHoarder

<https://www.reddit.com/r/DataHoarder/comments/c6fh4x/after_hoarding_over_50k_youtube_videos_here_is/>  

    After hoarding over 50k YouTube videos, here is the youtube-dl command I settled on.




## `[2020-01-01]` perkeep/gphotos-cdp: This program uses the Chrome DevTools Protocol to drive a Chrome session that downloads your photos stored in Google Photos. <https://github.com/perkeep/gphotos-cdp>

    we'd like our photos mirrored in seconds or minutes, not weeks.




# \* emfit sleep tracker      [[emfit]]

Emfit QS is my sleep tracker.  




## `[2018-08-18]` Emfit has local API; would be nice to use it&#x2026;      [[emfit]]

<https://gist.github.com/harperreed/9d063322eb84e88bc2d0580885011bdd>  
<https://gist.github.com/karlicoss/3361f6a239048a451daa2a02982ee180>  




### `[2020-09-11]` [sanielfishawy/emfit<sub>data</sub><sub>getter</sub>: Gets heart rate and respiration rate from an Emfit QS device on the same local network.](https://github.com/sanielfishawy/emfit_data_getter)      [[emfit]]




## `[2019-12-17]` downloadEmfitAPI.py <https://gist.github.com/vanne02135/6901cc2b92315881080d0ce0f07c1a17>




## ugh. maybe autorefresh the token? Fuckig hell.      [[emfit]]





### `[2021-02-06]` I think I ended up just using login + password. meh




## hmm, with emfit can code some sort of feedback tool which signals me to move when emfit loses signal      [[emfit]]




## `[2020-05-29]` emfit API didn't work for about three days straight&#x2026;      [[emfit]] [[backup]]




## `[2019-12-21]` samuelmr/emfit-qs: Unofficial Node client for Emfit QS

<https://github.com/samuelmr/emfit-qs>  

    Exchange username and password to a token (expires in 7 days). You can also log in to qs.emfit.com and check the ´remember_token´ parameter passed to API calls (e.g. with developer tools of your browser).




# \* bluemaestro temperature sensor      [[bluemaestro]]





## figure out bluemaestro, make sure all merged      [[bluemaestro]]

-   State "STRT"      from "TODO"       `[2019-03-12]`




## actually wonder if I can connect it to computer?      [[bluemaestro]]




## merge bluemaestros, plot separate environmental dashboard?      [[dashboard]]




## automate, about how I back up bluemaestro data      [[toblog]]




## `[2019-09-29]` yeah, could elaborate on backing up android data, could be quite generic?      [[android]]




# \* reddit      [[reddit]]





## I think cool fact should just be converted into org mode from backups (merged!) but generally there is no point capturing them?      [[reddit]]





### `[2019-09-10]` er, I guess for orger need to extract a simple reddit provider that just merges various timestamped backups?




## I guess just rely on bleanser instead after all? Just make it less spammy      [[bleanser]] [[reddit]]




## Check for deleted favorites      [[reddit]]

-   State "STRT"      from "TODO"       `[2019-03-23]`




### `[2019-08-25]` yep, it def happens; promnesia triggers it




## shit. need to bleanse reddit properly, otherwise looks like it's too much data&#x2026;      [[reddit]]




## basically, just go through stuff that doesn't exist anymore but was in favorites ever (and suppress errors for some of them)      [[reddit]]




## `[2020-01-11]` Getting Started — PRAW 3.6.0 documentation      [[reddit]]

<https://praw.readthedocs.io/en/v3.6.0/pages/getting_started.html#connecting-to-reddit>  

    You may also have realized that the karma values change from run to run. This inconsistency is due to reddit’s obfuscation of the upvotes and downvotes. The obfuscation is done to everything and everybody to thwart potential cheaters. There’s nothing we can do to prevent this.




# \* browser history





## compress databases as xz? would same about half of space at least, even more on firefox databases      [[promnesia]]





### `[2020-09-05]` probably not necessary with pruning




## cleanup firefox phone exports&#x2026;




## firefox history &#x2013; db format has changed??      [[hpi]] [[infra]]




## firefox history &#x2013; could compress with zstd? seems like 30x compression      [[promnesia]]





### `[2020-06-10]` to start with &#x2013; simply compress locally once the db is synced, will think about doing something smarter later




## firefox dev history      [[phone]]




## `[2020-08-29]` [seanbreckenridge/ffexport: export and interface with firefox history/visits and site metadata](https://github.com/seanbreckenridge/ffexport)




# \* hypothesis      [[hypothesis]]





## hmm, 9000 limit? might be necessary to do synthetic export instead&#x2026;      [[hypothesis]]




## Hypothesis API are cloned as well.      [[hypothesis]]





### `[2020-01-21]` fix in hypexport?




# \* github      [[github]]





## `[2020-02-01]` motivation for github backups      [[exports]]

    > if the official repo is taken down, your forks will disappear unless you have a copy.
    https://help.github.com/en/github/collaborating-with-issues-...
    I don't think that's true, I've personally recovered deleted repositories by finding its forks.
    edit: Ah never mind it seems things work differently in the case of DMCA takedowns




## warn about large repos?      [[github]]




## ghexport &#x2013; read times out      [[ghexport]]

    requests.exceptions.ReadTimeout: HTTPSConnectionPool(host='api.github.com', port=443): Read timed out. (read timeout=15)




## 500 error      [[ghexport]]

     File "/home/karlicos/.local/lib/python3.7/site-packages/github/Requester.py",
    line 276, in requestJsonAndCheck
        return self.__check(*self.requestJson(verb, url, parameters, headers,
    input, self.__customConnection(url)))
      File "/home/karlicos/.local/lib/python3.7/site-packages/github/Requester.py",
    line 287, in __check
        raise self.__createException(status, responseHeaders, output)
    github.GithubException.GithubException: 500 None




## backport old github backups to new format? should be enough to just wrap in 'events'      [[backup]] [[timeline]] [[promnesia]]




## github &#x2013; starred repos aren't updated??




# \* whatsapp      [[whatsapp]]

I don't really use it and it's pretty hostile so unlikely I'll bother.  




## /data/data/com.whatsapp/databases/msgstore.db       [[whatsapp]]

actually has messages!  




## `[2020-01-17]` MasterScrat/Chatistics: 💬 Python scripts to parse your Messenger, Hangouts, WhatsApp and Telegram chat logs into DataFrames.      [[whatsapp]]

<https://github.com/MasterScrat/Chatistics>  

    Unfortunately, WhatsApp only lets you export your conversations from your phone and one by one.
    
        On your phone, open the chat conversation you want to export
        On Android, tap on ⋮ > More > Export chat. On iOS, tap on the interlocutor's name > Export chat
        Choose "Without Media"
        Send chat to yourself eg via Email
        Unpack the archive and add the individual .txt files to the folder ./raw_data/whatsapp/




## `[2019-07-13]` tgalal/yowsup: The WhatsApp lib <https://github.com/tgalal/yowsup>

    It seems that recently yowsup gets detected during registration resulting in an instant ban for your number right after registering with the code you receive by sms/voice. I'd strongly recommend to not attempt registration through yowsup until I look further into this. Follow the status of this here.




# \* stackexchange      [[stackexchange]]





## `[2019-09-01]` Usage of /users/{ids}/favorites <span class='http-method' title='expects a GET HTTP method'>GET</span> - Stack Exchange API      [[promnesia]]

<https://api.stackexchange.com/docs/favorites-on-users>  

    Usage of /users/{ids}/favorites GET
    Discussion
    Get the questions that users in {ids} have favorited.
    This method is effectively a view onto a user's favorites tab.
    {ids} can contain up to 100 semicolon delimited ids. To find ids programmatically look for user_id on user or shallow_user objects.
    The sorts accepted by this method operate on the following fields of the question object:
        activity – last_activity_date
        creation – creation_date
        votes – score
        added – when the user favorited the question
    activity is the default sort.
    It is possible to create moderately complex queries using sort, min, max, fromdate, and todate.
    This method returns a list of questions.




### `[2019-09-16]` shit. seems that no way to get upvoted posts&#x2026; <https://meta.stackexchange.com/questions/299264/how-to-get-the-list-of-all-posts-ive-upvoted-via-the-api>




### `[2019-09-16]` <https://meta.stackexchange.com/questions/148008/how-can-i-see-comments-that-ive-upvoted>




### `[2019-09-16]` fuck. I guess I'm gonna have to scrape votes&#x2026; <https://stackoverflow.com/users/706389/karlicoss?tab=votes>




## stackexchange &#x2013; there are comments in GDPR requested data      [[stackexchange]]




## stackexchange &#x2013; shit

    ERROR:stexport:Giving up fetch_backoff(...) after 1 tries (stackapi.stackapi.StackAPIError: ('https://api.stackexchange.com/2.2/users/706389/privileges/?pagesize=100&page=1&filter=%21LVBj2%28M0Wr1s_VedzkH%28VG&site=alcohol.meta', 502, 'throttle_violation', 'too many requests from this IP, more requests available in 50511 seconds')




## stackexchange &#x2013; need to figure out how to import remaining data&#x2026;




## Today I would probably have tried parsing the Stack Exchange Data Dump instead.

Todo promnesia  
from [ip](https://www.instapaper.com/read/1275853358/12253044)   [Lessons learned from writing ShellCheck, GitHub’s now most starred Haskell project – Vidar's Blog](https://www.vidarholen.net/contents/blog/?p=859)  




### `[2021-02-06]` hmm, it's actual dump of <span class="underline">all</span> comments&#x2026; bit too much I guess




## hmm crashed on json decoding?      [[stexport]]

    [INFO stexport 2021-03-10 08:33:48,004 export.py:161] exporting dsp: users/{ids}/favorites
    [INFO stexport 2021-03-10 08:33:48,302 _common.py:86] Backing off fetch_backoff(...) for 0.5s (stackapi.stackapi.StackAPIError: ('https://api.stackexchange.com/2.2/users/706389/comments/?pagesize=100&page=1&filter=%21LVBj2%28M0Wr1s_VedzkH%28VG&&site=dsp', "('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))", "('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))", "('Connection aborted.', RemoteDisconnected('Remote end closed connection without response'))"))
    [ERROR stexport 2021-03-10 08:33:49,124 _common.py:101] Giving up fetch_backoff(...) after 2 tries (stackapi.stackapi.StackAPIError: ('https://api.stackexchange.com/2.2/users/706389/favorites/?pagesize=100&page=1&filter=%21LVBj2%28M0Wr1s_VedzkH%28VG&site=dsp', 'Expecting value: line 1 column 1 (char 0)', 'Expecting value: line 1 column 1 (char 0)', 'Expecting value: line 1 column 1 (char 0)'))
    Traceback (most recent call last):
      File "/home/adhoc/.local/lib/python3.8/site-packages/stackapi/stackapi.py", line 204, in fetch
        response = response.json()
      File "/usr/lib/python3/dist-packages/requests/models.py", line 897, in json
        return complexjson.loads(self.text, **kwargs)
      File "/usr/lib/python3.8/json/__init__.py", line 357, in loads
        return _default_decoder.decode(s)
      File "/usr/lib/python3.8/json/decoder.py", line 337, in decode
        obj, end = self.raw_decode(s, idx=_w(s, 0).end())
      File "/usr/lib/python3.8/json/decoder.py", line 355, in raw_decode
        raise JSONDecodeError("Expecting value", s, err.value) from None
    json.decoder.JSONDecodeError: Expecting value: line 1 column 1 (char 0)




# \* mastodon      [[mastodon]]





## `[2020-01-11]` kensanata/mastodon-backup: Archive your statuses, favorites and media using the Mastodon API (i.e. login required)

<https://github.com/kensanata/mastodon-backup>  

    Thus, if every request gets 20 toots, then we can get at most 6000 toots per five minutes.




## zigg/grabby: tools for scraping your Mastodon account data      [[mastodon]]

<https://github.com/zigg/grabby>  




## `[2019-12-29]` halcy/Mastodon.py: Python wrapper for the Mastodon ( <https://github.com/tootsuite/mastodon/> ) API.      [[mastodon]]

<https://github.com/halcy/Mastodon.py>  




## tusky android app keeps some history in tuskyDb      [[hpi]] [[mastodon]]




# \* pinboard      [[pinboard]]





## huh looks like pinboard is quite unstable with regards to backup&#x2026; unless the backup script is wrong or something?      [[bleanser]]




## `[2019-04-19]` Pinboard on Twitter: "Next question is, does a raw API call give the same results as the website? The API and website search engine run off of different indexes.… <https://t.co/CZrLE7YNWo>"      [[pinboard]]

<https://twitter.com/Pinboard/status/1113807174717792256>  

    Next question is, does a raw API call give the same results as the website? The API and website search engine run off of different indexes.




# -------&#x2013;&#x2014; other data sources  ---------------




# Podcast addict data




# `[2020-07-31]` [alexattia/Maps-Location-History: Get, Concatenate and Process you location history from Google Maps TimeLine](https://github.com/alexattia/Maps-Location-History)      [[location]] [[timeline]] [[qs]]

    In order to export processed data from Google Maps website from a python script, you need to get your actual cookie.

fuck me! it actually exports kml files  




# ok, so need to preserve all (incl.older) versions of notebooks? dunno feels a bit excessive      [[timeline]] [[remarkable]]




# `[2020-10-25]` [Garmin Connect](https://connect.garmin.com/modern/daily-summary/2020-10-25/heartRate)      [[garmin]]

    Looks like you experienced a time change. This may cause some inaccuracies with today's data.

jesus!  




# `[2020-12-30]` [Notice: This project is unmaintained · Issue #613 · fbchat-dev/fbchat](https://github.com/fbchat-dev/fbchat/issues/613)      [[facebook]]




# Need my email mirrored      [[email]]





## `[2019-03-12]` I guess I want continuous. Not sure how to achieve that, perhaps some mail client in the background?




# `[2019-06-13]` joeyates/imap-backup: Backup GMail (or other IMAP) accounts to disk      [[email]]

<https://github.com/joeyates/imap-backup>  




# Bandcamp history





## `[2020-12-13]` <https://bandcamp.com/developer> no listening history though&#x2026;




# hmm memrise personal data request is neat! It's got all you training sessions + learned words and phrases      [[publish]]




# do a full remarkable backup too?      [[remarkable]]





## `[2020-11-27]` [tech:ssh [reMarkableWiki](https://remarkablewiki.com/tech/ssh)]

    # the xochitl binary, if you plan on replacing or modifying it in any way
    scp root@remarkable:/usr/bin/xochitl remarkable-backup/




# better docs on what to do on expiry      [[monzo]]

    Traceback (most recent call last):
      File "pymonzo/monzo_api.py", line 209, in _get_response
        raise TokenExpiredError
    oauthlib.oauth2.rfc6749.errors.TokenExpiredError: (token_expired

this is how token looks like after:  

    modified: .pymonzo-token
    {
        "code": "internal_service",
        "message": "An error occurred processing the request"
    }




# huh, thriva uses an api&#x2026;




# call history from my old(er?)  phones? (e.g. nokia)




# increase sample rate to 10 seconds maybe?      [[arbtt]]




# process old 'backups' repo?




# reading hr data      [[wahoo]]

    import fitparse
    ff = fitparse.FitFile('2020-10-02-161142-TICKR X 076C-1601655102-0.fit')
    [m.get_value('timestamp') for m in ff.messages]

NOTE: not all messages are hr messages, there is also some metadata etc.  
<https://github.com/perrygeo/graph-kickr/blob/master/app.py>  




## `[2020-10-09]` also tried gpsbabel, but it resulted in no data&#x2026; weird

    gpsbabel -i garmin_fit,allpoints=1 -f '2020-10-02-161142-TICKR X 076C-1601655102-0.fit' -o unicsv -F res.csv




# `[2019-04-08]` python - Steam API get historical player count of specific game - Stack Overflow

<https://stackoverflow.com/questions/45983820/steam-api-get-historical-player-count-of-specific-game>  
There is no Steam Web API method for historical player count of a specific game.  




# Feedbin starred stuff




# `[2019-07-14]` fabianonline/telegram<sub>backup</sub>: Java app to download all your telegram data.

<https://github.com/fabianonline/telegram_backup>  

    Use --with-supergroups and / or --with-channels to also download all messages from the supergroups / channels you have joined that have been active in the last time.




# eh, should include older account? compare oldest and one of newer files..      [[monzo]]




# myshows: hmm, so looks like api v 1.8 is deprecated, for api 2.0 I'd need to email them. can just use raw jsons from existing backup script




# compress chrome histories? would require backup script to compress it I suppose&#x2026; maybe just go through them regularly and recompress




# bookmarks limit through api???      [[instapaper]]





## `[2020-01-04]` need to check historic exports and figure it out




# gpslogger &#x2013; add to backup checker??      [[location]]




# `[2020-10-03]` [Statify: Pull your playlist and listening data from the Spotify API to a Sqlite database](https://reddit.com/r/coolgithubprojects/comments/j4kn3y/statify_pull_your_playlist_and_listening_data/) /r/coolgithubprojects




# monzo export: make sure it works with original repo..      [[exports]] [[monzo]]





## `[2019-12-29]` huh, actually the problem might be in saving \_token variable?





### `[2019-12-29]` instead could just print it from disk? maybe even that is unnecessary?




# ugh, need to retrieve pinboard notes      [[pinboard]] [[exports]]

e.g. motivational example of API discovery; I just assumed they all would be retrieved <https://api.pinboard.in/v1/notes/ID>  




# `[2019-04-23]` feedbin/feedbin-api: Feedbin API Documentation      [[feedbin]]

<https://github.com/feedbin/feedbin-api#readme>  

    The base URL for all requests is https://api.feedbin.com/v2/ Only https is supported.
    The Feedbin API uses HTTP Basic authentication
    curl -u 'example@example.com:password' https://api.feedbin.com/v2/subscriptions.json




# `[2020-11-27]` [Success Stories · tcgoetz/GarminDB Wiki](https://github.com/tcgoetz/GarminDB/wiki/Success-Stories)      [[garmin]]




# `[2020-12-19]` [Importing your Goodreads & Accessing them with Open Library’s APIs](https://blog.openlibrary.org/2020/12/13/importing-your-goodreads-accessing-them-with-open-librarys-apis/)

    Importing your Goodreads & Accessing them with Open Library’s APIs




# `[2020-06-24]` [Telegram Now Lets You Export Your Chats, View Notification Exceptions | Technology News](https://gadgets.ndtv.com/apps/news/telegram-export-chats-notifications-exceptions-passport-encryption-1906903)      [[telegram]]




# get off the messages stored in old format and make sure nothing  is missing, dedup?      [[vk]]




# shit, they stopped you from accessing messages api. fuck.      [[vk]]

<https://vk.com/wall-1_390510>  




## `[2019-03-08]` that's very generic trend. I think ultimately we just need better tools to scrape that




# Headspace stats      [[timeline]]

UserTimelineEntry?  




# .polar directory      [[timeline]]




# `[2019-09-02]` vincaslt/memparse: A Memrise courses parser <https://github.com/vincaslt/memparse>




# skype call history?





## `[2020-04-19]` shit <https://answers.microsoft.com/en-us/skype/forum/all/skype-api/e025d0f6-7ae4-4bc4-9d5a-b2d70136deab>

    I regret to inform you but we do not have API or a program in Skype that lets you export your chat history that will include dates, timestamps etc.




# amazon orders history

-   State "STRT"      from "TODO"       `[2019-02-23]`




## `[2018-05-04]` ugh, order history report is broken for the UK version :( <https://www.amazon.co.uk/gp/help/customer/display.html?nodeId=202119330> wrote to support

<https://www.amazon.co.uk/gp/b2b/reports>  
Then could connect to drebedengi and add comments (even with breakdown)  




## `[2019-02-23]` backups/amazon

-   State "STRT"      from              `[2019-02-23]`




# ugh, bookmarks method in api is not exhaustive (elif item.get("type") == 'bookmark')      [[instapaper]]




# `[2019-04-01]` [Polar AccessLink Api Daily Activity Goal](https://reddit.com/r/Polarfitness/comments/b3cz6t/polar_accesslink_api_daily_activity_goal/ejwgklq/) /r/Polarfitness

    The API. You do need a session cookie for it and I didn't find an official documentation. The cookie can be retrieved by mimicking their login form. If you do have specific questions you can send me a DM but basically you just need to copy the requests their web app is making.




# just reuse files dir? def no harm in it      [[telegram]]




# blinkist: scrape off my highlights

<https://www.blinkist.com/en/nc/highlights>  




## `[2019-08-13]` eh, just copy responses manually?




## `[2019-08-13]` huh, actually if webdriver could eavesdrop on json responses would be perfect




## `[2019-08-13]` post in on github&#x2026;      [[toblog]]




# export bitbucket




# feedbin 




# `[2020-03-05]` signalnerve/roam-backup: Automated Roam Research backups using GitHub Actions and AWS S3

<https://github.com/signalnerve/roam-backup>  

    To use it, just fork this repo and add the following secrets to your repo (naming must match!):
        roamEmail
        roamPasswor




# ---------------------------------------------------- 




# `[2020-02-03]` Data lake - Wikipedia      [[dal]] [[exports]]

<https://en.wikipedia.org/wiki/Data_lake>  




# `[2020-04-21]` fucking hell. so materialistic export stopped working      [[phone]]

&#x2026; because I was copying sqlite file only  
and the app suddenly decided to keep everything in WAL. it's been growing over the past week without ever writing into the database  
what the fuck??? how do I deal with it???  




# start awesome-exports list?      [[exports]] [[publish]]




# script to grab files from downloads and move accodingly? e.g. for oyster statements




# [TW](https://twitter.com/i/web/status/822927519586381824) at `[2017-01-21]` Играюсь с IMDB, думал придется beautiful soap доставать айтемы из вотчлиста, а там в стейте реакта лежит JSONка      [[exports]]




# Post about various ways of data handling      [[toblog]] [[dataliberation]]

Mock response from backend  
Ignore method  
Mypy literal  
This is what rust does  




# `[2019-12-27]` 'hostage model' is a good term      [[toblog]] [[dataliberation]] [[sadinfra]]

referring to software/services when data is held  




# `[2020-01-15]` Hi, Camlistore author here. Andrew Gerrand worked with me on Camlistore too and&#x2026; | Hacker News      [[infra]] [[exports]]

<https://news.ycombinator.com/item?id=13700968>  

    bradfitz on Feb 21, 2017 | parent | favorite | on: Upspin – Another option for file sharing
    Hi, Camlistore author here.
    Andrew Gerrand worked with me on Camlistore too and is one of the Upspin authors.
    The main difference I see is that Camlistore can model POSIX filesystems for backup and FUSE, but that's not its preferred view of the world. It is perfectly happy modeling a tweet or a "like" on its own, without any name in the world.
    Upspin's data model is very much a traditional filesystem.
    Also, upspin cared about the interop between different users from day 1 with keyservers etc, whereas for Camlistore that was not the primary design criteria. (We're only starting to work on that now in Camlistore).
    But there is some similarity for sure, and Andrew knows both.




# automatic date extraction? could work, e.g. for rescuetime      [[datetime]] [[backupchecker]]




# &#x2013;&#x2014; last housekeeping on `[2021-02-06]` --------




# `[2020-04-13]` [twintproject/twint: An advanced Twitter scraping & OSINT tool written in Python that doesn't use Twitter's API, allowing you to scrape a user's followers, following, Tweets and more while evading most API limitations.](https://github.com/twintproject/twint)




# `[2020-04-23]` [MatthieuBizien/roam-to-git: Automatic RoamResearch backup to Git](https://github.com/MatthieuBizien/roam-to-git)

     Format [[links]]
    Format #links
    Format attribute::
    Format [[ [[link 1]] [[link 2]] ]]
    Format ((link))




# `[2020-04-28]` [timgrossmann/InstaPy: 📷 Instagram Bot - Tool for automated Instagram interactions](https://github.com/timgrossmann/InstaPy)




# right, so if you enable sync it seems to suck in history on the phone database? eh. messy      [[firefox]] [[exports]] [[promnesia]]




# crap&#x2026; android database has really high granulatity of events??      [[rescuetime]]




# `[2021-02-05]` [Chiaki/VKBK: Инструмент для создания и синхронизации локального бэкапа вашего профиля ВКонтакте (Profile backup & synchronization tool for Vk.com)](https://github.com/Chiaki/VKBK)      [[vk]] [[exports]]

ugh fuck.. apache & mysql? a bit much for me :(  




# `[2021-02-07]` [Against developer terms of service? · Issue #171 · Tyrrrz/DiscordChatExporter](https://github.com/Tyrrrz/DiscordChatExporter/issues/171)




# make it kinda smarter?      [[backupchecker]]

if it's a single file, don't do anything just yet?  
or treat it as 'simple' with month duration or something  
just do it doesn't warn immediately. could be a takeout archive or something  




# hmm, takeout has all tcx files?      [[endomondo]]




# hide praw logs unless interactive? too spammy in syslog      [[infra]]




# hm nice podcast addict simply backs up its database      [[exports]]

(although it only maintains two?)  




# Hmm maybe need to check for similar dst problems&#x2026; Basically mismatch between hr and sleep start/end?      [[emfit]]




# `[2021-02-25]` [ryanmcgrath/twython: Actively maintained, pure Python wrapper for the Twitter API. Supports both normal and streaming Twitter APIs.](https://github.com/ryanmcgrath/twython)      [[python]] [[twitter]]

hmm still working? nice&#x2026;  




# `[2021-02-04]` [Privacy Policy - October 15, 2020 - Reddit](https://www.redditinc.com/policies/privacy-policy#data-subject-and-consumer-information-requests)      [[reddit]] [[exports]]

ugh. gdpr takeout has to be emailed?  




# `[2021-02-05]` [Rapptz/discord.py: An API wrapper for Discord written in Python.](https://github.com/Rapptz/discord.py)      [[discord]] [[exports]]




# `[2021-02-08]` [Oura ring vs. Emfit QS (My detailed comparison) - What do you think? - Quantified Self / Sports, Physical Activity, and Fitness - Quantified Self Forum](https://forum.quantifiedself.com/t/oura-ring-vs-emfit-qs-my-detailed-comparison-what-do-you-think/8978)      [[emfit]] [[exports]]

    Can only store 10 hours of data on the device & 360 days in the cloud

huh? motivation for exports I guess  




# list the takeouts that are reduntant      [[takeout]] [[promnesia]]




# runnerup database file? could use existing computations perhaps?




# maybe for DAL, follow the pattern of exposing a method to read single export?      [[hpi]] [[exports]]

so it could cooperate with HPI&#x2026; egh not sure  




# Could utilize monzo categories for mine? I guess they could have errors.. Idk      [[monzo]]




# `[2021-03-10]` [Quickstart — StackAPI 0.1.12 documentation](https://stackapi.readthedocs.io/en/latest/user/quickstart.html?highlight=limits#change-number-of-results)      [[exports]]

    By default, StackAPI will return up to 500 items in a single call. It may be less than this, if there are less than 500 items to return. This is common on new or low traffic sites.
    The number of results can be modified by changing the page_size and max_pages values. These are multiplied together to get the maximum total number of results. The API paginates the results and StackAPI recombines those pages into a single result.




# `[2021-03-07]` [Exporting my own comment content from Disqus? · Discuss Disqus · Disqus](https://disqus.com/home/discussion/channel-discussdisqus/exporting_my_own_comment_content_from_disqus/)      [[disqus]] [[exports]]

seems hostile against exporting your own data  




# `[2021-03-23]` [Your eBay data](https://www.sarweb.ebay.co.uk/sar)      [[ebay]]

can request data takeout here&#x2026; takes ages to complete though, like a week  




# possible to have exactly same events with different API ids???      [[github]]

    vimdiff <(rg -A 363 -B 1 15538293160 events_20210317T120954Z.json) <(rg -A 363 -B 1 15538293166 events_20210317T120954Z.json)




# `[2021-04-18]` [exobrain/data/exports<sub>gdpr</sub> at master · seanbreckenridge/exobrain](https://github.com/seanbreckenridge/exobrain/tree/master/data/exports_gdpr)      [[exports]] [[gdpr]]

    Some thoughts on how easy to parse/use GDPR/get data exports from different services. A lot of these I did just because I was curious what information/context I could glean into the past about




# highlights are in UTC      [[remarkable]] [[koreader]]

