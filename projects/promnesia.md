
# Table of Contents

-   [\* data sources](#dtsrcs) 
    -   [social networks](#sclntwrks) 
    -   [hangouts (from google takeout)](#hngtsfrmggltkt) 
    -   [Local browser database](#lclbrwsrdtbs) 
    -   [Google takeout](#ggltkt) [[takeout]]
        -   [investigation what data is actually contributing to takeout](#nvstgtnwhtdtsctllycntrbtngttkt) 
        -   [youtube watch history from takeout](#ytbwtchhstryfrmtkt) [[youtube]]
    -   [use likes!](#slks) [[twitter]] [[hpi]]
    -   [Slide database &#x2013; visited posts? Same for hn](#slddtbsvstdpstssmfrhn) [[reddit]] [[hpi]]
        -   [`[2020-04-04]` right, SEEN database got some stuff /data/data/me.ccrama.redditslide/SEEN](#rghtsndtbsgtsmstffdtdtmccrmrddtsldsn) 
    -   [use my.pinboard](#smypnbrd) [[hpi]] [[pinboard]]
    -   [org context &#x2013; need to strip away todo state changes&#x2026;](#rgcntxtndtstrpwytdsttchngs) [[org]]
    -   [`[2020-01-25]` http://www.lord-enki.net/links.html import enki's wiki?](#wwwlrdnkntlnkshtmlmprtnkswk) [[exobrain]]
    -   [android resquetime database?](#ndrdrsqtmdtbs) [[hpi]] [[rescuetime]]
    -   [do I need to process org archive?](#dndtprcssrgrchv) [[org]]
    -   [android search history? not sure if worth trouble&#x2026;](#ndrdsrchhstryntsrfwrthtrbl) [[takeout]]
    -   [`[2020-09-05]` hmm, firefox on android has 'combined' view??](#hmmfrfxnndrdhscmbndvw) [[firefox]]
    -   [merge all of takeout histories? maybe as long it appears in both](#mrgllftkthstrsmybslngtpprsnbth) [[takeout]] [[hpi]]
    -   [wow, there is more stuff in takeouts](#wwthrsmrstffntkts) [[takeout]]
    -   [hmm, youtube 'watch-history' is ticking. but Youtube/MyActivity is fully backed up???](#hmmytbwtchhstrystckngbtytbmyctvtysfllybckdp) [[youtube]] [[takeout]]
    -   [`[2020-05-01]` plus.maths.org |](#splsmthsrgcntntplsmthsrg) 
    -   [google takeout &#x2013; parse json instead??](#ggltktprsjsnnstd) [[hpi]] [[takeout]]
    -   [think how should archives (zip/gz/etc) be handled&#x2026;](#thnkhwshldrchvszpgztcbhndld) 
    -   [Guess time based on git blame](#gsstmbsdngtblm) 
    -   [multiple twitter accounts?](#mltpltwttrccnts) [[twitter]]
    -   [deliveroo orders](#dlvrrdrs) 
    -   [stackexchange? reuse votes and favorites](#stckxchngrsvtsndfvrts) 
    -   [stackexchange gdpr has lots of visit data](#stckxchnggdprhsltsfvstdt) 
        -   [`[2020-12-04]` although it's over the whole domain, so not super useful](#lthghtsvrthwhldmnsntsprsfl) 
    -   [right, I am not using chrome anymore, which means takeout history is less and less useful for me](#rghtmntsngchrmnymrwhchmnstkthstryslssndlsssflfrm) [[promnesia]] [[takeout]]
    -   [use twidump as extra source?!](#stwdmpsxtrsrc) [[promnesia]]
    -   [figuring out history from window titles?](#fgrngthstryfrmwndwttls) [[promnesia]] [[arbtt]]
    -   [extract 'regular' links from markdown](#xtrctrglrlnksfrmmrkdwn) [[promnesia]]
-   [\* ideas](#ds) 
    -   [automatic interface](#tmtcntrfc) [[hpi]] [[promnesia]]
    -   [would be interesting to unify](#wldbntrstngtnfy) [[webarchive]] [[promnesia]]
-   [\* extension issues/improvements](#xtnsnsssmprvmnts) 
    -   [clicking on # on a github page causes reloading highlights&#x2026;](#clckngnngthbpgcssrldnghghlghts) 
        -   [`[2020-11-19]` eh. on the one hand, what else it should do? fragment could be anything](#hnthnhndwhtlstshlddfrgmntcldbnythng) 
    -   [improving highlights](#mprvnghghlghts) [[annotation]]
    -   [extension: ok, highlight by source color in 'show visited' definitely makes sense!](#xtnsnkhghlghtbysrcclrnshwvstddfntlymkssns) [[promnesia]]
    -   [performance: pagination should be configurable, i.e. if you run locally you might not need it at all](#prfrmncpgntnshldbcnfgrblfyrnlcllyymghtntndttll) 
    -   [extract canonical from page url as well? not sure how to make it more friendly and responsive&#x2026;](#xtrctcnnclfrmpgrlswllntsrhwtmktmrfrndlyndrspnsv) [[cannon]]
        -   [`[2019-08-31]` document.querySelector("link[rel='canonical']").href;](#dcmntqryslctrlnkrlcnnclhrf) 
        -   [`[2019-08-31]` Determining canonical url](#dtrmnngcnnclrl) 
        -   [`[2019-09-03]` eh, it's a bit tricky because requires extra content script execution and merging. And in 99.99% cases it's gonna be same as canonified url?](#htsbttrckybcsrqrsxtrcntntgngndncsstsgnnbsmscnnfdrl) 
        -   [`[2020-05-01]` maybe use it first? only then fallback on default algo. could make it configurable?](#mybstfrstnlythnfllbckndfltlgcldmktcnfgrbl) 
    -   [trying to debug unresponsiveness after idling](#tryngtdbgnrspnsvnssftrdlng) [[promnesia]]
    -   [`[2020-11-18]` All | Search powered by Algolia](#shnlglcmdtrngllpgprfxtrqrplrtytypllllsrchpwrdbylgl) [[promnesia]]
    -   [`[2020-05-25]` tabs.onActivated - Mozilla | MDN](#sdvlprmzllrgnsdcsmzllddnstbsnctvtdtbsnctvtdmzllmdn) [[promnesia]]
    -   [try loading stuff earlier, while URL updates](#tryldngstffrlrwhlrlpdts) [[promnesia]]
    -   [bug: in chrome](#bgnchrm) [[promnesia]]
    -   [bug: icon disappears on ctrl-t/close , but manual tab swtich with mouse is fine??](#bgcndspprsnctrltclsbtmnltbswtchwthmssfn) [[promnesia]]
    -   [`[2020-05-01]` doesn't work with readability? Quantum Diaries](#dsntwrkwthrdbltyswwwqntmdlctrwksymmtrybrkngqntmdrs) [[promnesia]]
    -   [bug: chrome: callbacks stop triggering after I reload the extension manually. ugh. Looks like due to the same callback hacking in background.js](#bgchrmcllbcksstptrggrngftthsmcllbckhckngnbckgrndjs) [[promnesia]]
        -   [`[2019-09-09]` right, I guess that's because first page that's opened on chrome is options<sub>page</sub>&#x2026;](#rghtgssthtsbcsfrstpgthtspndnchrmsptnspg) 
    -   [need to defensify everything](#ndtdfnsfyvrythng) [[toblog]] [[webext]]
    -   [Expose db from the server??](#xpsdbfrmthsrvr) [[malleable]]
    -   [`[2020-05-11]` Alexander Flores on Twitter: "@karlicoss having a pane like that but scroll synced to content in article would be ideal for me" / Twitter](#stwttrcmjflrssttslxndrflrtcntntnrtclwldbdlfrmtwttr) 
    -   [usability: perhaps easier with overlay in the middle of screen? then there are no issues with displaying&#x2026;](#sbltyprhpssrwthvrlynthmddscrnthnthrrnssswthdsplyng) 
    -   [usability: expand all/collapse all](#sbltyxpndllcllpsll) 
    -   [usability: display summary of available contexts on top?](#sbltydsplysmmryfvlblcntxtsntp) 
    -   [display some sort of 'collapsed' dynamic summary with tags and timestamps only? maybe on the side, and you 'zoom' into it as you scroll](#dsplysmsrtfcllpsddynmcsmmlymybnthsdndyzmnttsyscrll) 
    -   [bug: on 'cancel' after blacklist, still shows notification that it added](#bgncnclftrblcklststllshwsntfctnthttddd) [[promnesia]]
    -   [ui: split in tabs: annotations + plain visits? maybe even split by provider?](#spltntbsnnttnsplnvstsmybvnspltbyprvdr) 
    -   [ui: Sidebar](#sdbr) 
        -   [`[2019-08-01]` eh, ended up implementing mine for now&#x2026;](#hnddpmplmntngmnfrnw) 
        -   [`[2019-07-07]` jeremychurch/FixedContent.js: A mobile-friendly, jQuery plugin that persists sidebar content, nav, etc.](#jrmychrchfxdcntntjsmblfrnlgnthtprsstssdbrcntntnvtc) 
        -   [`[2019-07-07]` arkon/ng-sidebar: Angular sidebar component.](#rknngsdbrnglrsdbrcmpnnt) 
    -   [`[2019-04-19]` ui: Designing a Personal Knowledgebase – A Curious Mix](#dsgnngprsnlknwldgbscrsmx) [[promnesia]] [[org]]
        -   [`[2019-12-26]` i guess it was referring to unhighlighted links etc?](#gsstwsrfrrngtnhghlghtdlnkstc) 
    -   [bug: show visited mess with grasp?? (try selecting over these marks and capturing text)](#bgshwvstdmsswthgrsptryslctngvrthsmrksndcptrngtxt) [[promnesia]]
    -   [excludelist: www.site.com vs site.com](#xcldlstwwwstcmvsstcm) [[promnesia]]
-   [\* github issues](#gthbsss) 
    -   [extension: would be cool to have an option to just 'find' empty space on screen to overlay&#x2026; seems hard though](#xtnsnwldbclthvnptntjstfndtyspcnscrntvrlysmshrdthgh) [[ml]] [[think]]
        -   [`[2019-07-20]` more generally, non-invasive? and not sure if ml is necessary for that at all&#x2026;](#mrgnrllynnnvsvndntsrfmlsncssryfrthttll) 
    -   [`[2020-09-13]` Cannabidiol - PsychonautWiki](#spsychntwkrgwkcnnbdlcnnbdlpsychntwk) 
    -   [multiple processes](#mltplprcsss) 
        -   [use multiple threads for indexing&#x2026;](#smltplthrdsfrndxng) 
        -   [`[2020-11-08]` ugh fuck, def useful for indexing code..](#ghfckdfsflfrndxngcd) 
    -   [load more if page is scrolled? gonna be tricky&#x2026;](#ldmrfpgsscrlldgnnbtrcky) 
-   [\* indexer: bugs/issues](#ndxrbgssss) 
    -   [hmm. if we switch db mode to 'update', then schema changes would break promnesia&#x2026;](#hmmfwswtchdbmdtpdtthnschmchngswldbrkprmns) [[promnesia]]
-   [hmm, what if people used it with older orgparse? (suggest to update in release notes)](#hmmwhtfpplsdtwthldrrgprssggsttpdtnrlsnts) 
-   [personal style settings](#prsnlstylsttngs) 
-   [`[2020-11-22]` extension: twitter is pretty slow & logs are spammy Home / Twitter](#xtnsntwttrsprttyslwlgsrspmmystwttrcmhmhmtwttr) 
    -   [`[2020-11-23]` ugh, so also impacts 'show this thread'](#ghslsmpctsshwthsthrd) 
-   [`[2020-06-07]` inkandswitch/ksp-browser: Connect the things you already know in your browser.](#sgthbcmnkndswtchkspbrwsrnctththngsylrdyknwnyrbrwsr) [[pkm]]
    -   [`[2020-09-11]` hmm, need to outreach them?](#hmmndttrchthm) 
-   [different notions of 'visited'](#dffrntntnsfvstd) [[think]]
-   [figure out what could possibly be the most interesting source of links for people? I'd imagine whatsapp?](#fgrtwhtcldpssblybthmstntrngsrcflnksfrppldmgnwhtspp) 
    -   [`[2019-07-15]` reddit definitely. Slightly harder to motivate backups](#rddtdfntlyslghtlyhrdrtmtvtbckps) [[reddit]]
    -   [`[2019-07-15]` could integrate with my reddit backup script then? reindexing would trigger backup; seems kinda ok](#cldntgrtwthmyrddtbckpscrprndxngwldtrggrbckpsmskndk) 
    -   [`[2019-08-31]` pocket perhaps?](#pcktprhps) 
    -   [`[2019-08-31]` actually, pinboard; keep one backup in repository to test the extractor or demonstrate json extractor?](#ctllypnbrdkpnbckpnrpstrytthxtrctrrdmnstrtjsnxtrctr) [[pinboard]]
-   [`[2019-12-15]` Andy Matuschak on Twitter: "@LiquidTextCorp I'm very excited to try!"](#ndymtschkntwttrlqdtxtcrpmvryxctdttry) [[motivation]]
-   [`[2020-03-22]` It would be also great if it would work backwards aswell, eg.: "the link I found on twitter last week"](#twldblsgrtftwldwrkbckwrdsswllgthlnkfndntwttrlstwk) 
    -   [`[2020-05-28]` I mean it will once I integrate with the database properly&#x2026;](#mntwllncntgrtwththdtbsprprly) 
-   [`[2020-05-03]` (7) Spencer Chang on Twitter: "@jborichevskiy @Twitter @Wikipedia @hypothes<sub>is</sub> @RoamResearch Love this have been thinking in the same space where the content you consume is linked in-place to the content you (or the people you think are important) curate. Looking forward to seeing where this goes!" / Twitter](#stwttrcmspncrcsttsspncrchkngfrwrdtsngwhrthsgstwttr) [[ui]]
-   [`[2020-05-06]` WorldBrain.io on Twitter: "We are starting the development of the Memex Reader, an offline-first Pocket-style reader for desktop and mobile + mobile annotations. https://t.co/5lUpNSImFe Is anyone interested in collaborating/contributing to this? We need some more (wo)man power. ❤️" / Twitter](#stwttrcmwrldbrnsttswrldbrngtthswndsmmrwmnpwr️twttr) [[worldbrain]]
-   [`[2020-06-22]` WorldBrain.io on Twitter: "We're working on sharing/collaboration features of Memex and would love to have your input! Watch a quick rundown on some early mockups: https://t.co/brncMElHFr We'd love to have you for a 30-min call to get a grip on your use cases: https://t.co/AT52JajznO" / Twitter](#stwttrcmwrldbrnsttswrldbrgtgrpnyrscssstctjjzntwttr) [[worldbrain]] [[social]]
-   [`[2020-06-17]` TrailHub on Twitter: "https://t.co/do5RBGjjk4 Ready to give StorexHub a whirl! Take @hypothes<sub>is</sub> annotations, and bookmark the pages in memex so that they will show up as a liked page in memex and be indexed Add Page notes to Memex that link to hypothesis annotations https://t.co/SUk55b3ADn https://t.co/QsybMSwHxo" / Twitter](#stwttrcmtrlhbsttstrlhbntwstcskbdnstcqsybmswhxtwttr) 
-   [`[2020-03-21]` westoncb/mymex](#wstncbmymx) 
-   [demo: on malleable systems collective, with screenshot from the chat itself?](#dmnmllblsystmscllctvwthscrnshtfrmthchttslf) [[promnesia]] [[social]]
-   [usecase: reading hackernews 'new'](#scsrdnghckrnwsnw) 
-   [demo: 'mark visited' on the hackernews top?](#dmmrkvstdnthhckrnwstp) 
-   [`[2020-02-11]` mek.fyi | Home](#mkfyhm) 
    -   [`[2020-11-19]` tweet at Mek after releasing new version?](#twttmkftrrlsngnwvrsn) 
-   [demo: post again on /r/orgmode? with demos of highlights/translusion/backreferences?](#dmpstgnnrrgmdwthdmsfhghlghtstrnslsnbckrfrncs) 
-   [`[2020-11-19]` demo: good demo for mark visited Subscriptions - YouTube](#dmswwwytbcmfdsbscrptnsgddmfrmrkvstdsbscrptnsytb) 
-   [`[2020-11-17]` usecase: New Links | Hacker News](#scssnwsycmbntrcmnwstnxtnnwlnkshckrnws) 
-   [ugh, something's not working with release build in firefox??](#ghsmthngsntwrkngwthrlsbldnfrfx) 
-   [discuss on malleable systems how hard was it to modify youtube's website and inject annotations etc](#dscssnmllblsystmshwhrdwstdfyytbswbstndnjctnnttnstc) [[promnesia]] [[outbox]]
    -   [could also discuss with Oliver from worldbrain memex?](#cldlsdscsswthlvrfrmwrldbrnmmx) [[worldbrain]]
-   [demo: tweet HN new reading when I encounter some user I know](#dmtwthnnwrdngwhnncntrsmsrknw) 
-   [publish: release on lobsters? seems ok](#pblshrlsnlbstrssmsk) 
-   [`[2020-11-21]` control logging in content scripts](#cntrllggngncntntscrpts) 
-   [`[2019-07-08]` testing: unitest/History at master · scriptmasters/unitest](#tstngntsthstrytmstrscrptmstrsntst) [[hpi]] [[jdoe]]
-   [`[2019-11-22]` highlight: https://news.ycombinator.com/item?id=21403294](#hghlghtsnwsycmbntrcmtmd) 
    -   [`[2019-12-27]` I guess if I show it on HN, better get it right](#gssfshwtnhnbttrgttrght) 
-   [test: for the end2end test, run it against a database indexed with an older (PIP) version](#tstfrthndndtstrntgnstdtbsndxdwthnldrppvrsn) 
    -   [`[2020-11-19]` actually not super important; in most cases database is overwritten](#ctllyntsprmprtntnmstcssdtbssvrwrttn) 
-   [docs: make sure it's possible to run merely by creading config, then index, then serve](#dcsmksrtspssbltrnmrlybycrdngcnfgthnndxthnsrv) 
-   [Please visit https://editorjs.io/ to view all documentation articles.  Base concepts](#plsvstsdtrjstvwlldcmnttnrtclsbscncpts) 
-   [for demo, could just anonymize people? that would solve 99% of it](#frdmcldjstnnymzpplthtwldslvft) [[promnesia]] [[demo]]
-   [`[2020-05-11]` deen-chan on Twitter: "@ajflores1604 @karlicoss @jborichevskiy I've implemented this (augmented sidebar) and it's quite hard to come up with something that works well for all sites. You quickly run into sites which don't reflow, assuming a certain layout. But that was years ago. Responsive design is a lot more common these days so might work" / Twitter](#stwttrcmsrdncssttsdnchnntmrcmmnthsdyssmghtwrktwttr) 
-   [`[2020-07-05]` Guide to using filemagic — filemagic 1.6 documentation](#sflmgcrdthdcsnltstgdhtmlgdtsngflmgcflmgcdcmnttn) 
-   [`[2020-05-20]` I remember using this software last time, it is wayyyy~ too buggy, it stalls, cr&#x2026; | Hacker News](#snwsycmbntrcmtmdrmmbrsngtwyyyytbggytstllscrhckrnws) [[promnesia]] [[worldbrain]]
-   [fucking hell. figure out how to fix version exposed during the adhoc install&#x2026;.](#fcknghllfgrthwtfxvrsnxpsddrngthdhcnstll) 
-   [`[2019-12-12]` demo: Digital Tools I Wish Existed :: Up and to the Right — Jonathan Borichevskiy](#dmdgtltlswshxstdpndtthrghtjnthnbrchvsky) 
    -   [`[2020-03-28]` maybe make a screenshot out of it?](#mybmkscrnshttft) 
-   [`[2020-05-20]` Introduce Yourself - Thinking Tools](#sthnkngtlsspctntrdcyrslfntrdcyrslfthnkngtls) [[social]] [[publish]] [[promnesia]]
-   [`[2020-04-29]` integrate in Memex?](#ntgrtnmmx) [[worldbrain]]
-   [post automatic demo gifs](#psttmtcdmgfs) [[publish]]
-   [doc: minimal example to import something in promnesia, with crontab examples etc](#dcmnmlxmpltmprtsmthngnprmnswthcrntbxmplstc) [[promnesia]]
-   [maybe it should be `emacs://` ? not sure](#mybtshldbmcsntsr) [[mimemacs]] [[promnesia]]
    -   [`[2020-05-21]` or `editor://` ??](#rdtr) 
    -   [`[2020-05-29]` ok, so it seems that emacs:/// works and is backwards compatible, which is kinda good news](#kstsmsthtmcswrksndsbckwrdscmptblwhchskndgdnws) 
        -   [`[2020-05-30]` right. so I guess I know what to do](#rghtsgssknwwhttd) 
    -   [`[2020-05-29]` could add to doctor?](#cldddtdctr) 
    -   [`[2020-11-01]` maybe mimes should be configured & tested in the frontend? could add to the extension troubleshooting page](#mybmmsshldbcnfgrdtstdnthfdcldddtthxtnsntrblshtngpg) 
-   [`[2019-12-08]` motivation:](#mtvtn) 
-   [demo: of 'mark visited'](#dmfmrkvstd) [[toblog]] [[promnesia]]
    -   [`[2020-05-16]` hmm, make sure visited marker/css is tweakable? I suppose it needs to be in the 'main', sidebar section. confusing&#x2026;](#hmmmksrvstdmrkrcssstwkblstndstbnthmnsdbrsctncnfsng) 
        -   [`[2020-05-16]` post about it &#x2013; why don't we abuse a human brain which is much better at pattern recognition than computers (so far)](#pstbttwhydntwbshmnbrnwhchrtpttrnrcgntnthncmptrssfr) 
-   [publish packed zips in releases; assemble automatically on ci](#pblshpckdzpsnrlssssmbltmtcllync) [[ci]] [[webext]] [[promnesia]]
-   [remove 'duration' from the database? hopefully no one uses it yet&#x2026;](#rmvdrtnfrmthdtbshpfllynnsstyt) 
    -   [`[2020-05-14]` actually I might need it later.. if I populate them from #arbtt](#ctllymghtndtltrfppltthmfrmrbtt) 
-   [`[2020-01-13]` usecase: l3kn/org-fc: Spaced Repetition System for Emacs org-mode](#scslknrgfcspcdrpttnsystmfrmcsrgmd) 
-   [`[2019-11-01]` ui: Shtetl-Optimized » 2016 » April](#shttlptmzdprl) 
    -   [`[2019-11-04]` allow to be configured via CSS](#llwtbcnfgrdvcss) 
        -   [`[2019-11-04]` how to automate it actually?](#hwttmttctlly) 
-   [`[2019-11-09]` bug: Introduction - Everything I know](#bgntrdctnvrythngknw) 
    -   [`[2019-11-12]` eh. fair enough, it's changing URL. Not sure if there is much that can be done?](#hfrnghtschngngrlntsrfthrsmchthtcnbdn) 
        -   [`[2019-12-25]` except if cannon works clientside. Ugh!](#xcptfcnnnwrksclntsdgh) 
    -   [`[2019-12-07]` can be solved temporarily with proper blacklisting](#cnbslvdtmprrlywthprprblcklstng) 
-   [be less annoying about errors.. not sure how though](#blssnnyngbtrrrsntsrhwthgh) [[errors]]
    -   [`[2019-08-31]` just implement different options for notifications?](#jstmplmntdffrntptnsfrntfctns) 
    -   [`[2019-09-01]` quick option do disable/enable notifications; later find some generic component to snooze them?](#qckptnddsblnblntfctnsltrfndsmgnrccmpnnttsnzthm) 
        -   [`[2019-09-09]` yeah, I guess they'd be ok on sidebar? Basically, make sure sidebar <span class="underline">always</span> slides since it's convenient for settings, access to search etc.](#yhgssthydbknsdbrbscllymkscnvnntfrsttngsccsstsrchtc) 
-   [Def need way to make it less spammy on network errors on phone. System wide notification is too much](#dfndwytmktlssspmmynntwrkrrrsnphnsystmwdntfctnstmch) [[errors]]
-   [test going to different url in same tab; not sure how it would work&#x2026;](#tstgngtdffrntrlnsmtbntsrhwtwldwrk) 
-   [support stuff without tz? or at least warn and maybe instert as utc. or  just pass forward local tz that's ok for most people](#spprtstffwthttzrtlstwrnndssfrwrdlcltzthtskfrmstppl) 
-   [`[2019-08-29]` mozilla/webextension-polyfill: A lightweight polyfill library for Promise-based WebExtension APIs in Chrome](#mzllwbxtnsnplyflllghtwghtryfrprmsbsdwbxtnsnpsnchrm) [[webext]]
-   [`[2019-09-10]` handle when pages aren't available better](#hndlwhnpgsrntvlblbttr) 
    -   [`[2019-09-23]` need to implement at least popup](#ndtmplmnttlstppp) 
-   [`[2019-09-05]` lukeed/tinydate: A tiny (349B) reusable date formatter. Extremely fast!](#lkdtnydttnybrsbldtfrmttrxtrmlyfst) [[datetime]] [[js]]
-   [`[2019-07-14]` Surprisingly Turing-Complete - Gwern.net](#srprsnglytrngcmpltgwrnnt) 
-   [I guess sort of killer feature would be 'hierarchical' visits (e.g. facebook pages, reddit comments, github. etc. for reddit will require some manual rules against canonified urls)](#gsssrtfkllrftrwldbhrrchclllrqrsmmnlrlsgnstcnnfdrls) 
    -   [`[2019-07-22]` search kind of contributes towards that](#srchkndfcntrbtstwrdstht) 
-   [stuff in database seems to be unnormalised (e.g. case). need some sort of checker &#x2026;](#stffndtbssmstbnnrmlsdgcsndsmsrtfchckr) [[cannon]] [[togithub]]
    -   [`[2019-06-16]` hmm, do that I guess  sqlite3 visits.sqlite "select norm<sub>url,tag</sub> from visits where norm<sub>url</sub> LIKE '%usg%'"](#hmmdthtgsssqltvstssqltslcrmrltgfrmvstswhrnrmrllksg) 
-   [useful to populate from old backups (e.g pinboard) in case I delete articles/bookmarks](#sfltppltfrmldbckpsgpnbrdncsdltrtclsbkmrks) [[motivation]] [[promnesia]]
-   [filter links](#fltrlnks) 
-   [warn about anomally long histories?](#wrnbtnmllylnghstrs) 
-   [would be nice to process links/pieces of information that I merely seen!](#wldbnctprcsslnkspcsfnfrmtnthtmrlysn) 
-   [like hypothesis, but process the page server side and highlight against everything in the knowledge base](#lkhypthssbtprcssthpgsrvrsghtgnstvrythngnthknwldgbs) [[hypothesis]] [[pkm]] [[promnesia]]
-   [would be nice to know how I got onto the page&#x2026;](#wldbnctknwhwgtntthpg) [[promnesia]] [[motivation]]
    -   [`[2019-06-02]` use chrome from<sub>visit</sub>?](#schrmfrmvst) 
    -   [`[2021-01-20]` search basically does this](#srchbscllydsths) 
-   [need some thing which normalises and merges messages? or maybe just disregard duplicate links from old and new backups&#x2026;](#ndsmthngwhchnrmlssndmrgsmrddplctlnksfrmldndnwbckps) [[backup]] [[telegram]] [[promnesia]]
-   [could analyse 'how did I get there' from my web archives](#cldnlyshwddgtthrfrmmywbrchvs) [[archivebox]]
    -   [`[2019-07-31]` I guess I meant from plaintext search](#gssmntfrmplntxtsrch) 
-   [publish: /r/dataisbeautiful post my visited urls stats?](#pblshrdtsbtflpstmyvstdrlsstts) 
-   [Tweet from 𝔊𝔴𝔢𝔯𝔫 (@gwern), at Mar 10, 23:59](#twtfrm𝔊𝔴𝔢𝔯𝔫gwrntmr) [[promnesia]] [[motivation]]
-   [`[2019-04-15]` Pinboard: bookmarks for tswaterman tagged 'math'](#pnbrdbkmrksfrtswtrmntggdmth) 
-   [locators need short name along the full path](#lctrsndshrtnmlngthfllpth) 
-   [hmm, def looks like chrome is syncing bits of local database as well. ugh](#hmmdflkslkchrmssyncngbtsflcldtbsswllgh) 
-   [polar got OK design for sidebar](#plrgtkdsgnfrsdbr) [[polar]] [[promnesia]] [[inspiration]]
-   [custom search engine?](#cstmsrchngn) [[search]]
-   ['came from' is just a context. Would cover 99% of cases](#cmfrmsjstcntxtwldcvrfcss) 
-   [tags are pretty useful&#x2026;](#tgsrprttysfl) 
-   [Works really well in conjunction with axol (both dots and contexts)](#wrksrllywllncnjnctnwthxlbthdtsndcntxts) [[axol]] [[promnesia]] [[motivation]]
-   [showvisited: show dots on selection? useful so you don't need to send too many queries. or anchors like surfingkeys?](#shwvstdshwdtsnslctnsflsydndtmnyqrsrnchrslksrfngkys) 
-   [display error in sidebar?](#dsplyrrrnsdbr) [[errors]] [[ui]]
    -   [`[2019-07-14]` could be useful if we can extract URL; but encountered some issues while extracting context etc; could emit both visit and error](#cldbsflfwcnxtrctrlbtncntrngcntxttccldmtbthvstndrrr) 
-   [not sure, maybe I should just use native async/await? Most mobile and desktop browsers support it](#ntsrmybshldjstsntvsyncwtmstmblnddsktpbrwsrsspprtt) 
    -   [`[2019-07-15]` generally figure out how much can I get away with using modern JS as opposed to webpacked](#gnrllyfgrthwmchcngtwywthsngmdrnjssppsdtwbpckd) 
-   [go through existing urls and try to normalise them?](#gthrghxstngrlsndtrytnrmlsthm) [[webarchive]]
-   [ught https://github.com/brookhong/Surfingkeys/blob/57fccbbeeb60ee2be0d2d60cfc50bd3aca3b0436/background.js#L1094](#ghtsgthbcmbrkhngsrfngkysbccbbbbddcfcbdcbbckgrndjsl) [[webext]]
    -   [`[2019-07-07]` shit. ok, so chrome experiment confirms that it just doesn't work for extensions.](#shtkschrmxprmntcnfrmsthttjstdsntwrkfrxtnsns) 
    -   [`[2019-07-07]` shit. do I need bookmarklet or what???](#shtdndbkmrkltrwht) 
-   [`[2019-07-08]` Search · filename:places.sqlite https://github.com/search?p=2&q=filename%3Aplaces.sqlite&type=Code](#srchflnmplcssqltsgthbcmsrchpqflnmplcssqlttypcd) 
-   [`[2019-07-14]` mitchellkrogza/Ultimate.Hosts.Blacklist: The Ultimate Unified Hosts file for protecting your network, computer, smartphones and Wi-Fi devices against millions of bad web sites. Protect your children and family from gaining access to bad web sites and protect your devices and pc from being infected with Malware or Ransomware.](#mtchllkrgzltmthstsblcklstfrmbngnfctdwthmlwrrrnsmwr) 
-   [merge results together? e.g. search for inmotionmagazine](#mrgrsltstgthrgsrchfrnmtnmgzn) 
-   [`[2019-03-08]` motivation: Nikita Lisitsa on Twitter: "@<sub>bravit</sub> У меня так на stackoverflow / math.stackexchange бывает. Ищу ответ на вопрос, нахожу, читаю, ставлю лайк - "вы не можете поставить лайк своему собственному посту"." / Twitter](#mtvtnnktlstsntwttrbrvtумеемусобственномупостуtwttr) [[promnesia]]
-   [`[2019-07-08]` Does Firefox ship with a new default for "history expires after&#x2026;"? - Super User](#dsfrfxshpwthnwdfltfrhstryxprsftrsprsr) 
    -   [`[2019-07-08]` Does Firefox ship with a new default for "history expires after&#x2026;"? - Super User](#dsfrfxshpwthnwdfltfrhstryxprsftrsprsr) 
-   [for mimemacs, could probably support vim primarily (since all users will have it), it could even fallback](#frmmmcscldprbblyspprtvmprncllsrswllhvttcldvnfllbck) [[mimemacs]]
-   [`[2019-07-23]` demo: Best Mangal Bar & Kitchen delivery from Farringdon - Order with Deliveroo](#dmbstmnglbrktchndlvryfrmfrrngdnrdrwthdlvr) 
-   [rss blogs, easy to see what clicked and what hasn't](#rssblgssytswhtclckdndwhthsnt) [[rss]]
-   [should show visual indication on 'no results'](#shldshwvslndctnnnrslts) 
-   [when I merge together browser activity etc, I need to assert on some historic entries to make sure timestamps match properly](#whnmrgtgthrbrwsrctvtytcndtrstmksrtmstmpsmtchprprly) 
-   [would be too annoying to deal with transitions I guess, considering that it's not needed too often. Just rely on jumping into timeline?](#wldbtnnyngtdlwthtrnstnsgsnddtftnjstrlynjmpngnttmln) 
    -   [`[2019-08-01]` ??](#48184_48245) 
-   [open in new tab from search?](#pnnnwtbfrmsrch) 
-   [how did I get here &#x2013; perhaps shouldn't mix context and visits??](#hwddgthrprhpsshldntmxcntxtndvsts) 
-   [yeah, searches useful to have in db for context; even though they'd almost never match and normalise](#yhsrchssflthvndbfrcntxtvnhghthydlmstnvrmtchndnrmls) 
-   [yeah, show url split in parts; then when I click one of the parts in queries more data?](#yhshwrlspltnprtsthnwhnclcknfthprtsnqrsmrdt) 
-   [direct link to css from the extension?](#drctlnktcssfrmthxtnsn) 
    -   [`[2020-04-28]` I guess this is possible judging by greasemonkey](#gssthsspssbljdgngbygrsmnky) 
-   [could expand the grouped things on grey area press?](#cldxpndthgrpdthngsngryrprss) [[promnesia]] [[togithub]]
-   [maybe use two locators? one for linking and one for debugging](#mybstwlctrsnfrlnkngndnfrdbggng) 
    -   [`[2019-12-26]` eh?](#h) 
-   [moz-extension://b966cab9-aded-44e8-b116-a900ab825442/search.html?timestamp=1561844122.151](#mzxtnsnbcbddbbsrchhtmltmstmp) 
-   [hmmm author<sub>url</sub> could be useful?](#hmmmthrrlcldbsfl) [[hpi]] [[reddit]]
-   [bug: on android doesn't respond well on filter clicks, and overall looks a bit weird..](#bgnndrddsntrspndwllnfltrclcksndvrlllksbtwrd) 
-   [shows notification on navigation within page when clicking anchors http://super-memory.com/articles/sleep.htm#biphasic\_sleep ,perhaps shouldn't do that&#x2026;](#shwsntfctnnnvgtnwthnpgwhntmbphscslpprhpsshldntdtht) 
-   [enable back options to always show dots on visited urls?](#nblbckptnstlwysshwdtsnvstdrls) 
-   [`[2019-08-31]` uBlock/manifest.json at 6c34b3c3c96756b6db7ff2f3a0394472d81cde3e · gorhill/uBlock](#blckmnfstjsntcbccbdbfffdcdgrhllblck) [[webext]]
-   [allow per-device settings?](#llwprdvcsttngs) [[webext]]
-   [bug: on restoring tab, shows notification twice. weird](#bgnrstrngtbshwsntfctntwcwrd) 
    -   [`[2019-09-22]` doesn't seem to do with hacky injector backed initialization either. odd](#dsntsmtdwthhckynjctrbckdntlztnthrdd) 
    -   [`[2019-09-22]` also only happens in firefox, apparently&#x2026;](#lsnlyhppnsnfrfxpprntly) 
-   [https://slatestarcodex.com/2014/03/17/what-universal-human-experiences-are-you-missing-without-realizing-it/](#ssltstrcdxcmwhtnvrslhmnxprncsrymssngwthtrlzngt) 
-   [`[2019-07-30]` hmm it triggers on clicking anchors. not sure it's a good idea? also add to end2end tests](#hmmttrggrsnclckngnchrsntsrtsgddlsddtndndtsts) 
-   [local sync vs cloud? Not sure how to handle this properly; maybe have different profiles?](#lclsyncvscldntsrhwthndlthsprprlymybhvdffrntprfls) 
-   [`[2019-09-09]` test: fabianonline/telegram<sub>backup</sub>: Java app to download all your telegram data.](#tstfbnnlntlgrmbckpjvpptdwnldllyrtlgrmdt) 
-   [fails on firefox.com domain; fair enough, but perhaps need to blacklist it?](#flsnfrfxcmdmnfrnghbtprhpsndtblcklstt) 
-   [missing host permission &#x2013; very consistently reproduces on test<sub>visits</sub> if you close/reopen tab](#mssnghstprmssnvrycnsstntlyrprdcsntstvstsfyclsrpntb) 
-   [shit, tag map didn't work with context visits](#shttgmpddntwrkwthcntxtvsts) 
-   [have 'primary' settings profile and just think about rest later](#hvprmrysttngsprflndjstthnkbtrstltr) [[webext]]
-   [on android, maybe should only request on sidebard click? doesn't display icon anyway&#x2026; then basically it'd solve systemwide notification thing](#nndrdmybshldnlyrqstnsdbrdllytdslvsystmwdntfctnthng) [[promnesia]] [[togithub]]
-   [:invalid selector and input validation](#nvldslctrndnptvldtn) [[blog]] [[webext]]
-   [`[2019-10-19]` Re: [fregante/webext-options-sync] Race condition in OptionsSync constructor](#rfrgntwbxtptnssyncrccndtnnptnssynccnstrctr) 
-   [Highlight blacklisted and paywalled websites](#hghlghtblcklstdndpywlldwbsts) 
    -   [`[2020-11-19]` with mark visited it's much easier now.. could even have a special source and apply special style to them?](#wthmrkvstdtsmchsrnwcldvnhspclsrcndpplyspclstyltthm) 
-   [`[2019-11-04]` performance: vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources](#prfrmncvntwsmpythncrtdlstnfrmwrkslbrrssftwrndrsrcs) 
    -   [`[2020-11-14]` hmm, now it's fine but it highlights a bit too much info? not sure what to do about the fragment normalisation&#x2026;](#hmmnwtsfnbtthghlghtsbttmctsrwhttdbtthfrgmntnrmlstn) 
-   [`[2019-11-04]` promnesia/hypothesis.py at master · karlicoss/promnesia](#prmnshypthsspytmstrkrlcssprmns) 
-   [`[2019-11-09]` On todo lists | beepb00p](#ntdlstsbpbp) 
-   [Tweet from Will Manidis (@WillManidis), at Nov 26, 15:44](#twtfrmwllmndswllmndstnv) 
    -   [`[2019-12-26]` ugh, tweet is gone??](#ghtwtsgn) 
-   [ui, phone: don't really have to tweak body? as it's easy to hide/show sidebar](#phndntrllyhvttwkbdystssythdshwsdbr) [[promnesia]] [[togithub]]
-   [I don't like some twitter account I'm following: they are whining too much or whatever](#dntlksmtwttrccntmfllwngthyrwhnngtmchrwhtvr) [[twitter]] [[promnesia]] [[motivation]]
-   [Build client only version as demonstration?](#bldclntnlyvrsnsdmnstrtn) 
-   [query database](#qrydtbs) 
-   [org-mode: comments from LOGBOOK might be useful..](#rgmdcmmntsfrmlgbkmghtbsfl) [[org]]
-   [for search might be good to display original link??](#frsrchmghtbgdtdsplyrgnllnk) 
-   [`[2019-12-15]` bug: Теория вычислимости — Викиконспекты](#bgтеориявычислимостивикиконспекты) 
-   [Could map different people onto the same 'entity'?](#cldmpdffrntpplntthsmntty) 
-   [after loading browser with previously open tabs and then closing them; shows 'host permission' warning](#ftrldngbrwsrwthprvslypntblsngthmshwshstprmssnwrnng) 
-   [should allow running against live database? really why not, could be nice for exploring](#shldllwrnnnggnstlvdtbsrllywhyntcldbncfrxplrng) 
-   [Maybe git tracked server config is not so bad](#mybgttrckdsrvrcnfgsntsbd) 
-   [Use hub/click? And maybe docker to isolate](#shbclckndmybdckrtslt) [[docker]] [[python]]
-   [Would be rad if it was possible to simply run it against GitHub repo straight from ui](#wldbrdftwspssbltsmplyrntgnstgthbrpstrghtfrm) 
-   [`[2020-01-25]` Robot&AIWorld on Twitter: "Here's more footage of MIT's Mini Cheetahs cavorting, frolicking, back-flipping, playing soccer and generally acting fun and cute, courtesy of the Biomimetic Robotics Lab @MITMechE  https://t.co/8ZQzDvCDVW" / Twitter](#rbtwrldntwttrhrsmrftgfmtsslbmtmchstczqzdvcdvwtwttr) 
-   [Allow raw settings backup](#llwrwsttngsbckp) [[webext]]
    -   [`[2021-01-20]` this should really be easier&#x2026;](#thsshldrllybsr) 
-   [shit, google docs trigger a lot of reloads.. really should debounce](#shtggldcstrggrltfrldsrllyshlddbnc) 
-   [duplicating search page &#x2013; fucking hell. still happens on firefox&#x2026;](#dplctngsrchpgfcknghllstllhppnsnfrfx) 
-   [chronic versioning?](#chrncvrsnng) [[project]]
-   [ugh. subdomain needs to be banned..](#ghsbdmnndstbbnnd) 
-   [`[2019-12-27]` Adventures in WhatsApp DB — extracting messages from backups (with code examples)](#dvntrsnwhtsppdbxtrctngmssgsfrmbckpswthcdxmpls) [[promnesia]] [[whatsapp]]
-   [`[2019-12-30]` What am I meditating for? In Pursuit of A Definition of Meditation - Mark Koester](#whtmmdttngfrnprstfdfntnfmdttnmrkkstr) 
-   [warning about module size&#x2026;](#wrnngbtmdlsz) 
-   [not sure about tabs vs activeTab permission](#ntsrbttbsvsctvtbprmssn) [[webext]]
    -   [`[2020-02-15]` maybe instead I could simply check last requested url on tab switch?](#mybnstdcldsmplychcklstrqstdrlntbswtch) 
-   [ok, I guess I could make "tabs" an optional permission; by default only request stuff via click on a popup (that requires 'activeTab'?)](#kgsscldmktbsnptnlprmssnbystffvclcknpppthtrqrsctvtb) 
-   [shit, request on every tab switch is not good&#x2026;](#shtrqstnvrytbswtchsntgd) 
-   [`[2019-08-10]` right, chrome doesn't support android extensions. could use bookmarklet or something?? https://stackoverflow.com/a/10606887/706389](#rghtchrmdsntspprtndrdxtnskmrkltrsmthngsstckvrflwcm) 
-   [as a docker app?](#sdckrpp) 
-   [go through code and create issues?](#gthrghcdndcrtsss) 
-   [eh, web indexer doesn't really work for relative links&#x2026;](#hwbndxrdsntrllywrkfrrltvlnks) 
-   [combine with eye tracking, then could know how much time was spent reading something&#x2026;](#cmbnwthytrckngthncldknwhwmchtmwsspntrdngsmthng) 
-   [would be nice to get stuff collected by axol to promnesia database](#wldbnctgtstffcllctdbyxltprmnsdtbs) [[axol]] [[promnesia]]
-   [shit, 2mb per single page (10K visits) sucks&#x2026;. wonder if should use some different protocol? Or gzip defeats the purpose?](#shtmbprsnglpgkvstssckswnddffrntprtclrgzpdftsthprps) 
-   [`[2019-12-05]` Erik Torenberg (@eriktorenberg) / Twitter](#rktrnbrgrktrnbrgtwttr) [[motivation]] [[demo]]
-   [use dev webdriver??](#sdvwbdrvr) 
-   [demonstrate on that place with great bread](#dmnstrtnthtplcwthgrtbrd) [[promnesia]] [[demo]]
-   [`[2020-01-25]` hyperhype/hyperscript: Create HyperText with JavaScript.](#hyprhyphyprscrptcrthyprtxtwthjvscrpt) 
-   [`[2020-03-30]` Troubleshoot extensions, themes and hardware acceleration issues to solve common Firefox problems | Firefox Help](#trblshtxtnsnsthmsndhrdwrctslvcmmnfrfxprblmsfrfxhlp) [[webext]]
-   [maybe add sidebar menu on mobile only? anyway, need to add blacklist](#mybddsdbrmnnmblnlynywyndtddblcklst) 
-   ['mark visited' works really nice on the phone](#mrkvstdwrksrllyncnthphn) 
-   [doesn't work in private windows (I assume because of the getActiveTab thing)](#dsntwrknprvtwndwsssmbcsfthgtctvtbthng) 
-   [common usecase &#x2013; I follow someone, then I'm annoyed by their tweets and try to figure out why had I followed them in the first place?](#cmmnscsfllwsmnthnmnnydbytrtwhyhdfllwdthmnthfrstplc) 
-   [Maybe we just need a proxy that logs literally all of http requests.. That way history could be agnostic](#mybwjstndprxythtlgsltrllyfrqststhtwyhstrycldbgnstc) 
-   [shit, webdriver only took screenshot of half of the frame&#x2026;.](#shtwbdrvrnlytkscrnshtfhlffthfrm) 
-   [not compatible with gh: style links&#x2026;](#ntcmptblwthghstyllnks) 
-   [`[2020-04-07]` usecase: Idle Words https://idlewords.com/](#scsdlwrdssdlwrdscm) 
-   [could test on twint??](#cldtstntwnt) [[twitter]]
-   [usability: keyboard navigation](#sbltykybrdnvgtn) [[webext]] [[malleable]]
    -   [`[2019-08-01]` ugh. surfingkeys is capable of working on my iframe, but can't switch](#ghsrfngkysscpblfwrkngnmyfrmbtcntswtch) 
    -   [`[2019-08-26]` at least write about it in readme/faq](#tlstwrtbttnrdmfq) 
-   [could draw a small 'visits/contexts' tree? would be fun..](#clddrwsmllvstscntxtstrwldbfn) 
-   [maybe backend could update rules now and then..](#mybbckndcldpdtrlsnwndthn) [[cannon]]
-   [Breakdown of contexts by parts of virtual url in the sidebar](#brkdwnfcntxtsbyprtsfvrtlrlnthsdbr) 
-   [attemt to set up autorealoding](#ttmttstptrldng) [[promnesia]] [[webext]]
-   [Write a post demonstating which bits should not be part of extension](#wrtpstdmnsttngwhchbtsshldntbprtfxtnsn) [[malleable]] [[promnesia]] [[toblog]]
-   [Hmm. Sending fragment can be unsafe?](#hmmsndngfrgmntcnbnsf) 
-   [use arbtt to match the browsing history? that would be fun&#x2026;](#srbtttmtchthbrwsnghstrythtwldbfn) [[arbtt]] [[hpi]]
-   [readme: probably, better to install it via pipx? so HPI etc are easier to upgrade?](#rdmprbblybttrtnstlltvppxshptcrsrtpgrd) [[python]] [[promnesia]]
-   [`[2019-11-21]` raxod502/mercury: Emacs interface to Facebook Messenger](#rxdmrcrymcsntrfctfcbkmssngr) [[facebook]] [[hpi]]
    -   [`[2019-12-02]` could be useful&#x2026;](#cldbsfl) 
-   [`[2019-09-22]` 1397667 - "No matching message handler" error when tabs.update().then(tabs.executeScript())](#nmtchngmssghndlrrrrwhntbspdtthntbsxctscrpt) [[webext]]
-   [`[2019-09-22]` 1290016 - tabs.executeScript in webRequest.onCompleted gives "Unchecked lastError value: Error: No matching message handler"](#tbsxctscrptnwbrqstncmpltdtrrrvlrrrnmtchngmssghndlr) [[webext]]
-   [visual web scraper? geoffrey litt mentioned generalised nocode stuff (Pavel's question)](#vslwbscrprgffrylttmntndgnrlsdncdstffpvlsqstn) 
-   [`[2020-05-07]` eslint-plugin-no-unsafe-innerhtml - npm](#swwwnpmjscmpckgslntplgnnntmlslntplgnnnsfnnrhtmlnpm) [[webext]]
-   [be more informative; show full history or at least last visit and potentially sources (e.g. hypothesis)](#bmrnfrmtvshwfllhstryrtlsttvstndptntllysrcsghypthss) 
-   [attempt at agnostic url extraction (sha ae889fa0fb99f683cd1ba6192a3b55d11a481558)](#ttmpttgnstcrlxtrctnshffbfcdbbd) [[reddit]] [[promnesia]] [[hpi]]
-   [demonstrate jumping to the message on android? ironically it works better on phone](#dmnstrtjmpngtthmssgnndrdrncllytwrksbttrnphn) [[promnesia]] [[demo]]
-   [time spent? only for chrome apparently](#tmspntnlyfrchrmpprntly) [[promnesia]] [[demo]]
-   [Annotating post](#nnttngpst) [[worldbrain]]
-   [`[2020-05-20]` Memex/manifest.json at develop · WorldBrain/Memex](#sgthbcmwrldbrnmmxblbdvlpsmxmnfstjsntdvlpwrldbrnmmx) [[project]]
-   [`[2020-05-23]` Programming Inside a Container | Hacker News](#snwsycmbntrcmtmdprgrmmngnsdcntnrhckrnws) [[docker]] [[hpi]] [[promnesia]]
-   [what if I could apply :visited state for links that I marked as seen?](#whtfcldpplyvstdsttfrlnksthtmrkdssn) 
-   [settings &#x2013; add visual cues for dots/ visits/contexts/sources](#sttngsddvslcsfrdtsvstscntxtssrcs) 
-   [`[2020-05-13]` Native Messaging - Google Chrome](#sdvlprchrmcmxtnsnsntvmssgngntvmssgnggglchrm) [[webext]] [[promnesia]]
-   [`[2020-05-27]` Show HN: Obsidian – A knowledge base that works on local Markdown files | Hacker News](#snwsycmbntrcmtmdshwhnbsdntwrksnlclmrkdwnflshckrnws) 
    -   [`[2021-01-20]` some people apparently already used against obsidian db?](#smpplpprntlylrdysdgnstbsdndb) 
-   [Lesson](#lssn) [[promnesia]] [[publish]] [[think]]
-   [Hmm, maybe do not highlight stuff from archived org files/deleted instapaper/etc?](#hmmmybdnthghlghtstfffrmrchvdrgflsdltdnstpprtc) 
-   [Introduction to Marionette — Firefox Source Tree Docs 78.0a1 documentation](#ntrdctntmrnttfrfxsrctrdcsdcmnttn) [[webext]] [[promnesia]]
-   [tried disabling logic for single background page &#x2013; doesn't help even with persistent background..](#trddsblnglgcfrsnglbckgrndsnthlpvnwthprsstntbckgrnd) 
-   [`[2019-05-24]` useful to have links just added to instapaper to know that you are planning to read them there](#sflthvlnksjstdddtnstpprtknwthtyrplnnngtrdthmthr) 
-   [`[2020-04-29]` TypeError: can't access dead object - JavaScript | MDN](#sdvlprmzllrgnsdcswbjvscrprrcntccssddbjctjvscrptmdn) 
-   [`[2020-05-05]` type alias to union is invalid in runtime context · Issue #5354 · python/mypy](#sgthbcmpythnmypyssstyplstnvldnrntmcntxtsspythnmypy) 
-   [docs: mention that I'll be posting about breaking changes in releases](#dcsmntnthtllbpstngbtbrkngchngsnrlss) 
    -   [`[2020-05-29]` even better to do this in commits and simply reference stuff in releases? or, sync releases with a file in repository](#vnbttrtdthsncmmtsndsmplyrrlssrsyncrlsswthflnrpstry) 
-   [`[2020-06-03]` Using Service Workers - Web APIs | MDN](#sdvlprmzllrgnsdcswbpsrvcwcwrkrssngsrvcwrkrswbpsmdn) [[webext]]
-   [`[2020-06-03]` highlights: Quora Answers by David Pearce (2015 - 2020) : transhumanism with a human face](#hghlghtsswwwhdwbcmqrhtmlpbydvdprctrnshmnsmwthhmnfc) 
    -   [`[2020-11-14]` hmm, performance OK, but it throws ruandom erros now??](#hmmprfrmnckbttthrwsrndmrrsnw) 
-   [They record where you come from, what pages you visit, how long you stay on each, where you click and where you go next.](#thyrcrdwhrycmfrmwhtpgsyvsystynchwhryclckndwhrygnxt) 
-   [`[2019-07-28]` Firefox doesn't recognize telegramdesktop's tg link. /r/firefox](#srddtcmrfrfxcmmntspfrfxdscgnztlgrmdsktpstglnkrfrfx) [[telegram]]
-   [`[2020-05-25]` Dmitry Bobrov on Twitter: "@karlicoss No idea about the service, but I do have experience with Chrome extensions if that’s what you mean" / Twitter](#stwttrcmdvbbrvsttsdmtrybbhrmxtnsnsfthtswhtymntwttr) 
-   [`[2020-06-11]` doc: Share database between machine? · Issue #114 · karlicoss/promnesia](#dcsgthbcmkrlcssprmnssssssdtbsbtwnmchnsskrlcssprmns) 
-   [reuse readability extensions for better content highlight?](#rsrdbltyxtnsnsfrbttrcntnthghlght) 
-   [could use both for reddit cumulative state and promnesia browser exports](#cldsbthfrrddtcmltvsttndprmnsbrwsrxprts) [[hpi]] [[reddit]] [[cachew]]
-   [Post archive org highlights](#pstrchvrghghlghts) [[outbox]]
-   [merge mode &#x2013; could combine public and private data](#mrgmdcldcmbnpblcndprvtdt) 
-   [`[2020-05-11]` ESLint v7.0.0 Released | Hacker News](#snwsycmbntrcmtmdslntvrlsdhckrnws) [[promnesia]] [[webext]]
-   [`[2020-05-25]` Korobochka on Twitter: "@karlicoss Via Twitter?) For the last ~6 months I am developing a Chrome extension at work, can take a look as well." / Twitter](#stwttrcmkrbchksttskrbchknmxtnsntwrkcntklkswlltwttr) 
-   [version detection &#x2013; thing in cachew works pretty well? perhaps it might not work without installing, but otherwise should?](#vrsndtctnthngncchwwrksprtwrkwthtnstllngbtthrwsshld) 
-   [HPI/promnesia: a whitepaper?](#hpprmnswhtppr) [[publish]]
-   [ok, could use some design inspiration from ampie](#kcldssmdsgnnsprtnfrmmp) [[ampie]]
-   [`[2020-09-25]` (20) Anyone use Promnesia? | Building a Second Brain](#sbldngscndbrncrclscmcsrgmrmnsnynsprmnsbldngscndbrn) 
-   [hm, for serving reuse config, but allow to split config bits to make defensive?? not sure..](#hmfrsrvngrscnfgbtllwtspltcnfgbtstmkdfnsvntsr) 
-   [could use pandoc for serving HTML?](#cldspndcfrsrvnghtml) 
-   [about realtime indexing (give a demo of entr??)](#btrltmndxnggvdmfntr) [[totweet]] [[promnesia]]
-   [support child visits etc for inbrowser history](#spprtchldvststcfrnbrwsrhstry) 
-   [dynamic JS hook only in dev mode?](#dynmcjshknlyndvmd) 
-   [how to display warnings in the very end? extract from warnings module maybe?](#hwtdsplywrnngsnthvryndxtrctfrmwrnngsmdlmyb) 
-   [using generators to defer UI updates?](#snggnrtrstdfrpdts) [[toblog]] [[promnesia]] [[js]]
-   [ideally configuration would be kinda like a grid? for every (almost) source and for every function](#dllycnfgrtnwldbkndlkgrdfrvrylmstsrcndfrvryfnctn) 
-   [sharing links with surfingkeys? e.g. they could both filter crap links](#shrnglnkswthsrfngkysgthycldbthfltrcrplnks) 
-   [sidebar isn't opening if new tab, then google search (firefox)](#sdbrsntpnngfnwtbthngglsrchfrfx) 
-   [check blacklist right before querying backend as the last resort?](#chckblcklstrghtbfrqryngbckndsthlstrsrt) 
-   [for excludes, 'do not mark this link' and 'do not mark this element'&#x2026; the latter is gonna be way harder](#frxcldsdntmrkthslnknddntmkthslmntthlttrsgnnbwyhrdr) [[togithub]] [[promnesia]]
-   [usecase: when I follow someone on github/twitter/etc I'll make a quick note. Next time I'll know why](#scswhnfllwsmnngthbtwttrtcllmkqckntnxttmllknwwhy) [[demo]]
-   [`[2020-11-10]` inkandswitch/ksp-browser: Connect the things you already know in your browser.](#sgthbcmnkndswtchkspbrwsrnctththngsylrdyknwnyrbrwsr) 
-   [`[2020-11-19]` Essays · Gwern.net](#swwwgwrnntndxssysgwrnnt) 
-   [`[2020-11-18]` Watch later - YouTube](#swwwytbcmplylstlstwlwtchltrytb) 
-   [`[2020-11-17]` Merveilles    it's pretty dynamic and might not work well with 'mark visited'](#smrvllstwnwbgttngstrtdmrvcndmghtntwrkwllwthmrkvstd) 
-   [`[2020-11-17]` Withings body+ vs. Withings body cardio : QuantifiedSelf](#swwwrddtcmrqntfdslfcmmntsbdyvswthngsbdycrdqntfdslf) 
-   [`[2020-11-14]` What forces layout/reflow. The comprehensive list.](#sgstgthbcmplrshdfbbcwhtfrcslytrflwthcmprhnsvlst) 
-   [`[2020-11-16]` TweetDeck](#stwtdcktwttrcmtwtdck) 
-   [hmm, could serve the exlcudelist from the backend???](#hmmcldsrvthxlcdlstfrmthbcknd) 
-   [`[2020-11-22]` The File System Access API: simplifying access to local files](#swbdvflsystmccssthflsystmccsspsmplfyngccsstlclfls) [[promnesia]]
-   [visited marks might impact ellipsized content](#vstdmrksmghtmpctllpszdcntnt) 
-   [faq: some pages may prevent extensions on working on them](#fqsmpgsmyprvntxtnsnsnwrkngnthm) 
    -   [`[2020-11-22]` eh, not sure if this is the case with extensions? bookmarklets (like Hypothesis on HN &#x2013; yeah)](#hntsrfthssthcswthxtnsnsbkmrkltslkhypthssnhnyh) 
-   [Add donation link, to bastien?](#dddntnlnktbstn) 
-   [if I use sidebar, it will work even on websites that forbid html injections?](#fssdbrtwllwrkvnnwbststhtfrbdhtmlnjctns) [[togithub]] [[firefox]]
-   [maybe I need something a bit more discrete for contexts notification&#x2026;](#mybndsmthngbtmrdscrtfrcntxtsntfctn) 
-   [shows host error exceptions in firefox on pdfs](#shwshstrrrxcptnsnfrfxnpdfs) [[promnesia]] [[togithub]]
    -   [`[2019-12-26]` could be disabled via blacklisting \*.pdf probably?](#cldbdsbldvblcklstngpdfprbbly) 
-   [process archive as well?](#prcssrchvswll) [[promnesia]] [[org]] [[togithub]]
-   [could hide annotations via tags?](#cldhdnnttnsvtgs) [[promnesia]] [[togithub]]
-   [backlist: tampermonkey?](#bcklsttmprmnky) 
    -   [`[2020-11-16]` eh?](#h) 
-   [`[2020-05-25]` iorate/uBlacklist: Blocks specific sites from appearing in Google search results](#sgthbcmrtblcklstrtblcklstcstsfrmpprngngglsrchrslts) [[webext]] [[promnesia]]
-   [add some throttling for the notification at least](#ddsmthrttlngfrthntfctntlst) 
    -   [`[2020-02-25]` added suppressing..](#dddspprssng) 
    -   [`[2020-03-23]` maybe, it's better just to turn it off by default&#x2026;](#mybtsbttrjstttrntffbydflt) 
-   [prefill with domain name?](#prfllwthdmnnm) [[promnesia]] [[search]]
-   [ublock content picker is awesome&#x2026; would be nice to find one..](#blckcntntpckrswsmwldbnctfndn) 
-   [blacklisted: allow to force loading (from sidebar)](#blcklstdllwtfrcldngfrmsdbr) 
-   [sidebar doesn't work while search is open :( :(](#sdbrdsntwrkwhlsrchspn) 
-   [`[2020-05-02]` Plain text linkifiers comparison (work in progress) (http://jsbench.github.io/#54315d74264c857856c73f18c81278dc)](#sgstgthbcmskndccfcdcplntxknprgrssjsbnchgthbdccfcdc) 
-   [closing tab before it's finished loading causing error. I guess that's fine and shouldn't be defensified..](#clsngtbbfrtsfnshdldngcsngrgssthtsfnndshldntbdfnsfd) 
-   [not sure how to handle desktop notifications vs builtin? I'd prefer to use system as far as we can I guess but they are not easy to fine tune](#ntsrhwthndldsktpntfctnsvssfrswcngssbtthyrntsytfntn) [[webext]] [[togithub]]
-   [host permission on closing and reopening tab?](#hstprmssnnclsngndrpnngtb) 
-   [right, switching to highlight.js/codejar does make it 110kb (vs 170 kb)](#rghtswtchngthghlghtjscdjrdsmktkbvskb) 
-   [#hypothesis adds special element <hypothesis-highlight>? wtf??](#hypthssddsspcllmnthypthsshghlghtwtf) 
-   [`[2020-03-02]` windows 10 - Disable Chrome to ask for confirmation to open external application everytime - Super User](#wndwsdsblchrmtskfrcnfrmtntpnxtrnlpplctnvrytmsprsr) [[promnesia]] [[mimemacs]]
-   [ignored entries should be colored as black](#gnrdntrsshldbclrdsblck) [[promnesia]] [[togithub]]
-   [could merge (e.g. chrome and takeout) both on client and server; not sure which would be best](#cldmrggchrmndtktbthnclntndsrvrntsrwhchwldbbst) 
-   [replace fixture with tmp<sub>path</sub> like in orger?](#rplcfxtrwthtmppthlknrgr) 
-   [`[2019-09-15]` bug: raw.githubusercontent.com/karlicoss/dotfiles/master/surfingkeys/config.txt](#bgrwgthbsrcntntcmkrlcssdtflsmstrsrfngkyscnfgtxt) 
    -   [`[2019-09-22]` ugh. works fine in dev firefox and doesn't even have sources on release?](#ghwrksfnndvfrfxnddsntvnhvsrcsnrls) 
    -   [`[2019-09-23]` also seems to be fine in chrome, however doesn't display kkj](#lssmstbfnnchrmhwvrdsntdsplykkj) 
-   [process confidences and somehow add this information in visit line](#prcsscnfdncsndsmhwddthsnfrmtnnvstln) 
-   [show with discarded url get params?](#shwwthdscrddrlgtprms) [[promnesia]] [[togithub]]
    -   [`[2019-06-02]` eh??](#h) 
    -   [`[2019-12-27]` I guess I meant ignore normalisation etc](#gssmntgnrnrmlstntc) 
-   [pinboard last seen](#pnbrdlstsn) 
    -   [I guess needs a pinboard provider?](#gssndspnbrdprvdr) 
-   [fuck :D google takeout had json formats for activity&#x2026;](#fckdggltkthdjsnfrmtsfrctvty) [[backup]] [[promnesia]] [[takeout]]
-   [use really really old takeout and see what happens](#srllyrllyldtktndswhthppns) 
-   [ctrl-r doesn't seem to update extension icon for stale tab](#ctrlrdsntsmtpdtxtnsncnfrstltb) 
-   [Motivation for browser history: its just easier to grab than google takeout data. I just need to merge them together i suppose](#mtvtnfrbrwsrhstrytsjstsrtktdtjstndtmrgthmtgthrspps) [[motivation]]
-   [option to disable dots on the page (permanently or temrporary)](#ptntdsbldtsnthpgprmnntlyrtmrprry) 
-   [Maybe desktop integration?](#mybdsktpntgrtn) 
    -   [`[2019-12-26]` what?](#wht) 
    -   [`[2021-01-20]` like a remembrance agent maybe?](#lkrmmbrncgntmyb) 
-   [backend: URL extraction via NN?](#bckndrlxtrctnvnn) 
-   [hmm it sort of around when I'm clicking links on the page.. would be interesting to see how that works](#hmmtsrtfrndwhnmclcknglnkshpgwldbntrstngtshwthtwrks) 
    -   [`[2019-08-05]` eh?](#h) 
-   [Watch "There is No Algorithm for Truth - with Tom Scott" on YouTube](#wtchthrsnlgrthmfrtrthwthtmscttnytb) [[promnesia]] [[motivation]]
    -   [`[2019-11-21]` eh, not sure..](#hntsr) 
-   [people who followed you?](#pplwhfllwdy) 
    -   [`[2020-11-20]` not sure what I meant here?](#ntsrwhtmnthr) 
-   [wonder if it would help me to figure out what was the video https://www.youtube.com/watch?v=Z-R2xO3phVM](#wndrftwldhlpmtfgrtwhtwsthvdswwwytbcmwtchvzrxphvm) 
-   [fallback in sequence?](#fllbcknsqnc) 
-   [right, spend a bit debugging sidebar with 10K visits](#rghtspndbtdbggngsdbrwthkvsts) 
-   [tell about fake systemd?](#tllbtfksystmd) [[toblog]]
-   [Would be fun to run the backend on Android..](#wldbfntrnthbckndnndrd) 
-   [need to fix compare db to allow for small relative changes? at least for pinboard and reddit](#ndtfxcmprdbtllwfrsmllrltvchngstlstfrpnbrdndrddt) 
-   [pydeps src/promnesia](#pydpssrcprmns) [[python]] [[hpi]] [[promnesia]]
-   [Hmm wonder if could adapt promnesia for Next browser?](#hmmwndrfclddptprmnsfrnxtbrwsr) 
-   [`[2020-04-24]` usecase: compute-space/compute-space.md at master · jauntywunderkind/compute-space](#scssgthbcmjntywndrkndcmptmdtmstrjntywndrkndcmptspc) 
-   [`[2020-04-24]` usecase: westoncb/mymex](#scssgthbcmwstncbmymxwstncbmymx) 
-   [`[2020-05-06]` Firefox for Mobile now supports NoScript, PrivacyBadger, HTTPS Everywhere | Hacker News](#snwsycmbntrcmtmdfrfxfrmblptprvcybdgrsvrywhrhckrnws) 
-   [`[2019-01-19]` Switching over to communicating via private server](#swtchngvrtcmmnctngvprvtsrvr) 
-   [`[2020-06-30]` Native messaging is extremely broken and has bad documentation. I never got repl&#x2026; | Hacker News](#snwsycmbntrcmtmdntvmssgngsbddcmnttnnvrgtrplhckrnws) [[webext]]
-   [browser history: clicked 'forget about this site' for google.com by accident.. wonder if it's gonna erase stuff](#brwsrhstryclckdfrgtbtthsscmbyccdntwndrftsgnnrsstff) 
-   [`[2020-07-06]` Linux kernel coders propose inclusive terminology coding guidelines, note: 'Arguments about why people should not be offended do not scale' • The Register](#swwwthrgstrcmlnxkrnlcdrspshldntbffndddntsclthrgstr) 
-   [`[2020-11-06]` jeanralphaviles/comment<sub>parser</sub>: Python module to extract comments from source code files of various types.](#sgthbcmjnrlphvlscmmntprsrcmmntsfrmsrccdflsfvrstyps) 
-   [`[2020-11-08]` target browsers insteadd of Node, remove old react stuff, update eslint babel · karlicoss/promnesia@c8380e0](#sgthbcmkrlcssprmnsrnschcktffpdtslntbblkrlcssprmnsc) 
-   [`[2020-11-16]` uBlock/webext.js at 5aca41960373656c79d547b1a983f053e6adb633 · gorhill/uBlock](#sgthbcmgrhllblckblbccdbfdckwbxtjstccdbfdbgrhllblck) 
-   [bug: right, seems that extension disconnects after a timeout in chrome based browsers](#bgrghtsmsthtxtnsndscnnctsftrtmtnchrmbsdbrwsrs) 
-   [`[2019-09-01]` keepassxc-browser/manifest.json at develop · keepassxreboot/keepassxc-browser](#kpssxcbrwsrmnfstjsntdvlpkpssxrbtkpssxcbrwsr) [[webext]]
    -   [`[2019-09-08]` figure out why is this necessary?](#fgrtwhysthsncssry) 
-   [hmm, need to overwrite database in order to handle schema updates? not sure what would be a clean way of doing it&#x2026;](#hmmndtvrwrtdtbsnrdrthndlspdtsntsrwhtwldbclnwyfdngt) 
    -   [`[2019-08-07]` I guess similar to cachew?](#gsssmlrtcchw) 
    -   [`[2019-09-03]` ok, although haven't tested that behaviour](#klthghhvnttstdthtbhvr) 
-   [I really need page notes&#x2026; e.g. reasons why I removed the bookmark and whether I already visited it..](#rllyndpgntsgrsnswhyrmvdthbkmrkndwhthrlrdyvstdt) 
    -   [maybe, set up inotify to update the database?](#mybstpntfytpdtthdtbs) 
-   [maybe show yellow icon if we only have chrome visits? so in a sense, green is more 'interesting' visits. also, maybe blink with green for a while (and have a timer whether we blinked in the past hour or something)](#mybshwyllwcnfwnlyhvchrmvshthrwblnkdnthpsthrrsmthng) 
    -   [`[2019-06-01]` need automatic generation for differently colored icons&#x2026;](#ndtmtcgnrtnfrdffrntlyclrdcns) 
    -   [`[2019-06-02]` distinguish contexts as well](#dstngshcntxtsswll) 
    -   [`[2019-08-08]` just needs a better documenting..](#jstndsbttrdcmntng) 
-   [share code with js &#x2026;. ugh, all the projects I found really suck&#x2026;](#shrcdwthjsghllthprjctsfndrllysck) [[ffi]] [[malleable]]
-   [highlight/color certain tags (configure that in settings)](#hghlghtclrcrtntgscnfgrthtnsttngs) 
    -   [`[2019-06-01]` suggest tags? maybe by querying from api, although presumably there wouldn't be too many. make the config YAML](#sggsttgsmybbyqryngfrmplthythrwldntbtmnymkthcnfgyml) 
-   [make sure it searches in archive&#x2026;](#mksrtsrchsnrchv) 
-   [Use cachew for browser history](#scchwfrbrwsrhstry) [[promnesia]] [[cachew]]
-   [`[2020-05-27]` sshkarupa/url-handlers](#sgthbcmsshkrprlhndlrssshkrprlhndlrs) [[mimemacs]]
-   [`[2019-09-01]` vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources](#vntwsmpythncrtdlstfwsmpytnfrmwrkslbrrssftwrndrsrcs) 
-   [at first, make filters private when I release it](#tfrstmkfltrsprvtwhnrlst) 
    -   [`[2019-10-12]` ok, they do save a bit of space for me, e.g. 575Mb vs 376 Mb. I guess keep my private ones for now and keep them empty in config, can resolve later](#kthydsvbtfspcfrmgmbvsmbgsndkpthmmptyncnfgcnrslvltr) 
        -   [`[2019-10-27]` fuck I'm so glad I'm keeping notes! Would have never remembered why db size changed otherwise..](#fckmsgldmkpngntswldhvnvrrmmbrdwhydbszchngdthrws) 
-   [reddit link in context](#rddtlnkncntxt) 
-   [would be also useful to highlight visited posts, e.g. here https://www.lesswrong.com/posts/vwqLfDfsHmiavFAGP/the-library-of-scott-alexandria](#wldblssflthghlghtvstdpstsfshmvfgpthlbrryfscttlxndr) [[promnesia]] [[demo]]
-   [attempt to use prismjs](#ttmpttsprsmjs) 
-   [wonder if I can embed in a page, as an Iframe?](#wndrfcnmbdnpgsnfrm) 
    -   [`[2019-12-26]` would be hard because of need to login, etc&#x2026;](#wldbhrdbcsfndtlgntc) 
-   [`[2020-02-18]` Upload Add-on :: Promnesia :: Add-ons for Firefox](#sddnsmzllrgnsdvlprsddnprmsbmtpldddnprmnsddnsfrfrfx) 
-   [`[2020-10-28]` thesephist/histools: A collection of tools for generating data visualizations from browser history data](#sgthbcmthsphsthstlsthsphsgdtvslztnsfrmbrwsrhstrydt) 
-   [release: suggest to update the backend](#rlssggsttpdtthbcknd) 
-   [need to figure out how to keep error traceback/context..](#ndtfgrthwtkprrrtrcbckcntxt) [[python]] [[promnesia]] [[errors]]
-   [I failed miserably at reaching out to Worldbrain/Hypothesis to discuss whether we should collaborate :worldbrain:hypothesis](#fldmsrblytrchngttwrldbrnhwshldcllbrtwrldbrnhypthss) 
-   [How to run as a proxy server? So it would work with any apps](#hwtrnsprxysrvrstwldwrkwthnypps) 
-   [Tweet from @posobin](#twtfrmpsbn) [[promnesia]] [[inspiration]]
-   [`[2020-11-07]` ugh. looked in codemirror src, but unclear how to optimize the size further. it's just big **shrug**](#ghlkdncdmrrrsrcbtnclrhwtptmzthszfrthrtsjstbgshrg) 
-   [`[2020-05-06]` agnostic extraction &#x2013; extracting context is pretty much impossible](#gnstcxtrctnxtrctngcntxtsprttymchmpssbl) [[promnesia]] [[hpi]]
-   [`[2020-11-01]` profiling: so overall it seems that half time spent in parsing org-mode, half in url extraction. meh](#prflngsvrlltsmsththlftmsptnprsngrgmdhlfnrlxtrctnmh) 
    -   [`[2021-01-20]` this py-spy thing is very nice](#thspyspythngsvrync) [[performance]] [[python]]
-   [https://www.freecodecamp.org/news/lossless-web-navigation-spatial-model-37f83438201d/ https://merveilles.town/@aynish/105139837128207627](#swwwfrcdcmprgnwslsslsswbntnsptlmdlfdsmrvllstwnynsh) 
-   [email mek](#mlmk) 
-   [mark visited &#x2013; maybe for ignored links add an attribute/explanation or something](#mrkvstdmybfrgnrdlnksddnttrbtxplntnrsmthng) 
-   [what if I add 'fake' history into browser database? wonder if that would work&#x2026;](#whtfddfkhstryntbrwsrdtbswndrfthtwldwrk) 
-   [`[2020-11-26]` Nyxt](#snyxttlsngnrftrsnyxt) 
-   [`[2020-11-27]` showvisited: Новые серии / MyShows.me](#shwvstdsmyshwsmprflновыесерииmyshwsm) 
-   [`[2020-12-14]` Gephi - The Open Graph Viz Platform](#sgphrggphthpngrphvzpltfrm) [[timeline]]
    -   [`[2020-12-14]` could draw en edge if the visits are close in time?](#clddrwndgfthvstsrclsntm) 
-   [`[2020-05-17]` All Time - Hacker News Top Links](#wwwhntplnkscmlllltmhckrnwstplnks) 
-   [`[2020-01-22]` Playing around with Chrome's history https://gist.github.com/dropmeaword/9372cbeb29e8390521c2#chrome](#plyngrndwthchrmshstrysgstgthbcmdrpmwrdcbbcchrm) [[chrome]]
-   [`[2020-12-05]` interop: DIYgod/RSSHub: 🍰 Everything is RSSible](#ntrpsgthbcmdygdrsshbdygdrsshbvrythngsrssbl) [[rss]] [[promnesia]] [[wildcard]]
-   [`[2020-12-06]` Org-roam User Manual](#swwwrgrmcmmnlhtmlrgrmsrmnl) 
-   [`[2020-12-06]` Org-roam User Manual](#swwwrgrmcmmnlhtmlrmprtclrgrmsrmnl) [[grasp]] [[promnesia]]
-   [`[2020-12-06]` Newsletter 10 - Neovim v0.4.4 - Neovim](#snvmnwsnwslttrnvmvnvm) 
-   [`[2020-12-13]` showvisited: Mile End Climbing Wall](#shwvstdswwwmlndwllrgkmlndclmbngwll) 
-   [somehow lower priority for org<sub>archive</sub> stuff](#smhwlwrprrtyfrrgrchvstff) [[org]]
-   [`[2020-04-13]` Show HN: Built an extension to put an end to paywalls and popups | Hacker News](#snwsycmbntrcmtmdshwhnbltnptnndtpywllsndpppshckrnws) 
-   [`[2021-01-19]` markdown bug #promnesia](#mrkdwnbgsdscrdcmchnnlsprmns) [[promnesia]]
-   [`[2020-05-20]` shell script - Launching a terminal emulator without knowing which ones are installed - Unix & Linux Stack Exchange](#snxstckxchngcmqstnslnchngchnsrnstlldnxlnxstckxchng) [[promnesia]] [[emacs]]
-   [`[2020-11-02]` Repl.it - Node.js Online Compiler and IDE - Fast, Powerful, Free](#srpltlnggsndjsrpltndjsnlncmplrnddfstpwrflfr) [[js]] [[datetime]] [[promnesia]]
-   [`[2021-01-18]` promnesia/TROUBLESHOOTING.org at master · karlicoss/promnesia](#sgthbcmkrlcssprmnsblbmstrblshtngrgtmstrkrlcssprmns) 
-   [`[2021-01-03]` html - CSS set default scroll position - Stack Overflow](#sstckvrflwcmqstnscssstdflsstdfltscrllpstnstckvrflw) [[promnesia]]
-   [`[2021-01-17]` #annotation-talks](#sdscrdcmchnnlsnnttntlks) 
-   [fetch all new posts and match them against promnesia?](#ftchllnwpstsndmtchthmgnstprmns) [[promnesia]] [[hackernews]]
-   [I'd say the biggest problem with something like this is that it's a silo. You're&#x2026; | Hacker News](#dsythbggstprblmwthsmthnglkthssthttsslyrhckrnws) [[worldbrain]] [[interop]] [[promnesia]]
-   [`[2020-05-02]` Vision, Mission & Values — 2020 Update - WorldBrain.io - Medium](#smdmcmwrldbrnvsnmssnvlspdtdvsnmssnvlspdtwrldbrnmdm) [[worldbrain]]
    -   [`[2020-05-09]` hmm, this storex hub thing could be used to feed in promnesia data](#hmmthsstrxhbthngcldbsdtfdnprmnsdt) 
-   [Potential social features (other people's annotations)](#ptntlsclftrsthrpplsnnttns) 
-   [demonstrate on some provider how it works as plaintext (e.g. grep), then as json and then as specific provider (and what do we get from that?)](#dmnstrtnsmprvdrhwtwrkssplspcfcprvdrndwhtdwgtfrmtht) 
-   [demonstrate indexing as json and as more specific instapaper?](#dmnstrtndxngsjsnndsmrspcfcnstppr) [[promnesia]]
-   [in contexts if you add extra text it may potentially mess with highlighting. will be resolved with fuzzy I guess](#ncntxtsfyddxtrtxttmyptntllghtngwllbrslvdwthfzzygss) [[promnesia]]
-   [It could be a tool similar to browser. Maybe you don't use it very often, but when you want it it's pretty good to have it, like browser history. Also it's a an actually working prototype unlike most of other snippet's I've  seen](#tcldbtlsmlrtbrwsrmybydntsprttypnlkmstfthrsnpptsvsn) 
-   [not sure how to decouple in the future?](#ntsrhwtdcplnthftr) 
-   [motivaiton: If you're digging for some topic you find yourself increasingly running at the same people](#mtvtnfyrdggngfrsmtpcyfndyrslfncrsnglyrnnngtthsmppl) 
-   [Crucial ability is jumping right into context (tweet/tg message/etc). That complements search really well](#crclbltysjmpngrghtntcntxtgtcthtcmplmntssrchrllywll) [[infra]] [[promnesia]]
-   [Tweet from @jethroksy](#twtfrmjthrksy) [[promnesia]]
    -   [`[2020-04-27]` ok, I think it ties it via ID or something.. so not so agnostic..](#kthnkttstvdrsmthngsntsgnstc) 
-   [@dalmo3: Built this chrome extension to get your @hypothes<sub>is</sub> annotations into @RoamResearch https://t.co/X3A1AxfFkg](#dlmbltthschrmxtnsntgtyrhysnnttnsntrmrsrchstcxxffkg) [[promnesia]]
-   [`[2020-05-24]` Vivaldi browser v1.8 released, with calendar-style browsing history | Hacker News](#snwsycmbntrcmtmdvvldbrwsrndrstylbrwsnghstryhckrnws) [[promnesia]]
-   [People clearly like curating bookmarks. I could pitch it](#pplclrlylkcrtngbkmrkscldptcht) [[toblog]]
-   [andy matuschak https://twitter.com/andy\_matuschak/status/1206055315000528898](#ndymtschkstwttrcmndymtschkstts) 
-   [`[2020-04-28]` tweet at mek?](#twttmk) 
-   [I tried to make sure it's as resilient as possible](#trdtmksrtssrslntspssbl) [[promnesia]] [[errors]]
-   [highlight css styling among features](#hghlghtcssstylngmngftrs) [[css]]
-   [attempt to implement uniform engine for annotation: not necessary for hypothesis to do so](#ttmpttmplmntnfrmngnfrnnttnntncssryfrhypthsstds) [[promnesia]]
-   [design: few things became apparent: realtime updates are tedious to implement, however it's way easier to make stuff recompute everything from scratch. kcache was motivated by that](#dsgnfwthngsbcmpprntrltmpdfrmscrtchkcchwsmtvtdbytht) [[toblog]] [[promnesia]]
-   [design: There is no way to implement this without keeping the data locally (or to be more specific, in one place)](#dsgnthrsnwytmplmntthswthtgthdtlcllyrtbmrspcfcnnplc) 
-   [`[2019-08-25]` demo: HN Classics https://posobin.com/hn\_classics/](#dmhnclsscsspsbncmhnclsscs) 
    -   [`[2020-04-27]` eh, red dots don't look nice here?](#hrddtsdntlknchr) 
-   [I was to make an emphasis: it's not a vaporware!](#wstmknmphsstsntvprwr) 
-   [in the process I had to fix the python url extraction library&#x2026;](#nthprcsshdtfxthpythnrlxtrctnlbrry) [[promnesia]] [[toblog]]
    -   [`[2020-04-29]` could add this to yak shaving section](#cldddthstykshvngsctn) 
-   [Ideally I'd want some sort of AI assistant that would detect relevant bits and highlight them](#dllydwntsmsrtfssstntthtwlddtctrlvntbtsndhghlghtthm) 
-   [benefit of using browser history (sqlite) databases: easier to sync them around (or if you can't be bothered to do google takeout every now and then)](#bnftfsngbrwsrhstrysqltdtbtbbthrdtdggltktvrynwndthn) [[promnesia]]
-   [bug: database might be lock while creating index? probably because of periodic indexer](#bgdtbsmghtblckwhlcrtngndxprbblybcsfprdcndxr) 
-   [exclude fonts](#xcldfnts) [[promnesia]]
-   [was in some sort of infinite/super slow binding loop in the sidebar on discord, turned it off for now](#wsnsmsrtfnfntsprslwbndnglpnthsdbrndscrdtrndtfffrnw) [[promnesia]]
-   [further directions](#frthrdrctns) [[promnesia]] [[toblog]]
-   [hmm, interferes?  e.g. try highlighting over a 'visited' mark](#hmmntrfrsgtryhghlghtngvrvstdmrk) [[promnesia]] [[hypothesis]]
-   [need to log less in serve?](#ndtlglssnsrv) [[promnesia]]
-   [querying for datetimes accounting for tz `SELECT norm_url, dt, src, (coalesce(datetime(substr(dt,1,instr(dt,' ')-1)), datetime(dt))) FROM visits WHERE rowid IN (SELECT rowid FROM visits ORDER BY RANDOM() LIMIT 1000)`](#qryngfrdttmsccntngfrtzslclctrwdfrmvstsrdrbyrndmlmt) [[promnesia]] [[sqlite]]
-   [`[2021-02-07]` Insidious Big Brother Database User Manual: 1. BBDB](#bbdbsrcfrgntbbdbhtmlnsdsbgbrthrdtbssrmnlbbdb) [[promnesia]]
-   [`[2021-02-07]` Latest Nyxt topics - Atlas](#sdscrstlsngnrcnyxtltstnyxttpcstls) [[promnesia]]
-   [right, url extraction: https://github.com/lipoja/URLExtract/issues/13#issuecomment-467635302 and also I guess cut off trailing dots?](#rghtrlxtrctnsgthbcmlpjrlxscmmntndlsgssctfftrlngdts) 
-   [`[2021-03-28]` installable mobile addon promnesia – Add-ons for Firefox (en-GB)](#nstllblmblddnsddnsmzllrgnnsprmnsprmnsddnsfrfrfxngb) [[promnesia]]
-   [`[2021-03-26]` Convert to ES6 compatible library by AStoker · Pull Request 65 · apvarun/toastify-js](#sgthbcmpvrntstfyjspllcnvrybystkrpllrqstpvrntstfyjs) [[promnesia]]
-   [`[2021-05-03]` agora: promnesia-howto](#sngrrgprmnshwtgrprmnshwt) [[promnesia]]

Blog post: <https://beepb00p.xyz/promnesia.html>  

Project: <https://github.com/karlicoss/promnesia>  




# \* data sources





## social networks




## hangouts (from google takeout)




## Local browser database




## Google takeout      [[takeout]]





### investigation what data is actually contributing to takeout

visited <http://slatestarcodex.com/superintelligence-faq/> through google search  
from there jumped to <http://slatestarcodex.com/2018/03/07/open-thread-96-75/>  
err weird, both are displayed in google activity (online); but only first one is in Search/MyActivity.html takeout. But last on is in Chrome/MyActivity.html. Right.. so I guess Chrome/MyActivity is a bit more useful?&#x2026;  
ugh. whatever, just use them all, there is no downside.  




### youtube watch history from takeout      [[youtube]]

here is something for youtube <https://github.com/pixelventures/youtube-history-querier/blob/f6da9ac88f93f776d41fcc159fc5632f64210d06/python-parser/main.py>  




## use likes!      [[twitter]] [[hpi]]

not sure what to do about dates.. support None for datetime??  




## Slide database &#x2013; visited posts? Same for hn      [[reddit]] [[hpi]]





### `[2020-04-04]` right, SEEN database got some stuff /data/data/me.ccrama.redditslide/SEEN




## use my.pinboard      [[hpi]] [[pinboard]]




## org context &#x2013; need to strip away todo state changes&#x2026;      [[org]]




## `[2020-01-25]` <http://www.lord-enki.net/links.html> import enki's wiki?      [[exobrain]]




## android resquetime database?      [[hpi]] [[rescuetime]]




## do I need to process org archive?      [[org]]




## android search history? not sure if worth trouble&#x2026;      [[takeout]]

also wonder, maybe I should turn google search history off?  




## `[2020-09-05]` hmm, firefox on android has 'combined' view??      [[firefox]]

right, it seems to group stuff  

    select date, url, title, history_guid from combined where history_id != -1 ORDER BY history_guid




## merge all of takeout histories? maybe as long it appears in both      [[takeout]] [[hpi]]




## wow, there is more stuff in takeouts      [[takeout]]

shit ok, takeouts are a decent way to preload it&#x2026;  

    2232156  2019-09-13 00:32   Takeout/YouTube/history/search-history.html
    2365963  2019-09-13 00:32   Takeout/YouTube/playlists/likes.json




## hmm, youtube 'watch-history' is ticking. but Youtube/MyActivity is fully backed up???      [[youtube]] [[takeout]]




## `[2020-05-01]` [plus.maths.org |](https://plus.maths.org/content/)

hypothesis extractor could generate a nicer title of the document?  




## google takeout &#x2013; parse json instead??      [[hpi]] [[takeout]]




## think how should archives (zip/gz/etc) be handled&#x2026;




## Guess time based on git blame




## multiple twitter accounts?      [[twitter]]




## deliveroo orders




## stackexchange? reuse votes and favorites




## stackexchange gdpr has lots of visit data





### `[2020-12-04]` although it's over the whole domain, so not super useful




## right, I am not using chrome anymore, which means takeout history is less and less useful for me      [[promnesia]] [[takeout]]




## use twidump as extra source?!      [[promnesia]]




## figuring out history from window titles?      [[promnesia]] [[arbtt]]

bit too excessive I guess&#x2026; although nice correlating events to jump in history?  




## extract 'regular' links from markdown      [[promnesia]]

i.e. ones without http prefix  




# \* ideas





## automatic interface      [[hpi]] [[promnesia]]

-   datetime
-   url
-   exclude Json (not sure how?)
-   [ ] first go through some data sources and see how well it's gonna work

start with 'static' version  

-   datetime: figure out by annotations  
    TODO shit gonna be tricky with tz aware/unaware stuff
-   url: figure out by  'url'/'href' attribute name (types don't seem to work?..)

then switch  

-   datetimes by isinstance
-   url: dynamically by checking if 'http' or something in strings? but might be tricky




## would be interesting to unify      [[webarchive]] [[promnesia]]

-   <https://transhumanist-party.org/2019/06/09/transhumanism-teleology/>
-   <https://turingchurch.net/how-transhumanism-changed-my-views-on-teleology-231d24d7a3bd> was deleted, but I have some instapaper annotations




# \* extension issues/improvements





## clicking on # on a github page causes reloading highlights&#x2026;

i guess just need to ignore explicitly for now  




### `[2020-11-19]` eh. on the one hand, what else it should do? fragment could be anything

and also doesn't happen anywhere else  




## improving highlights      [[annotation]]

on this page, the whole body is highlighted because of 'How does it work?'  
<https://github.com/karlicoss/promnesia#how-does-it-work>  




## extension: ok, highlight by source color in 'show visited' definitely makes sense!      [[promnesia]]




## performance: pagination should be configurable, i.e. if you run locally you might not need it at all




## extract canonical from page url as well? not sure how to make it more friendly and responsive&#x2026;      [[cannon]]





### `[2019-08-31]` document.querySelector("link[rel='canonical']").href;




### `[2019-08-31]` Determining canonical url

sort of a standard is using link rel canonical tag.  




### `[2019-09-03]` eh, it's a bit tricky because requires extra content script execution and merging. And in 99.99% cases it's gonna be same as canonified url?

<https://physicstravelguide.com/advanced_tools/gauge_symmetry#tab__faq> this for example gives gauge<sub>symmetry</sub> page as canonical  




### `[2020-05-01]` maybe use it first? only then fallback on default algo. could make it configurable?




## trying to debug unresponsiveness after idling      [[promnesia]]

-   chrome.runtime.onSuspend.addListener &#x2013; aaaah, ok seems that it's  triggering (errors are logged to 'extensions' settings page, oddly)  
    
        function handleSuspend() {
          console.error("Suspending event page");
          // handle cleanup
        }
        
        chrome.runtime.onSuspend.addListener(handleSuspend);

-   persistent: true &#x2013; let's see  
    TODO wonder if it would also remove the need for bckg injector?  
    
    ok, almost def has to do with it!




## `[2020-11-18]` [All | Search powered by Algolia](https://hn.algolia.com/?dateRange=all&page=0&prefix=true&query=browsercompany&sort=byPopularity&type=all)      [[promnesia]]

breaks this header..  




## `[2020-05-25]` [tabs.onActivated - Mozilla | MDN](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/API/tabs/onActivated)      [[promnesia]]

might need to respond to this  




## try loading stuff earlier, while URL updates      [[promnesia]]

I guess if notification off, it's not really a problem. just make sure it's caching and not querying too much  
and test it too?  




## bug: in chrome      [[promnesia]]

open any site  
open sidebar  
press search  
close search  
icon goes to grey, showing 'no visits'  




## bug: icon disappears on ctrl-t/close , but manual tab swtich with mouse is fine??      [[promnesia]]




## `[2020-05-01]` doesn't work with readability? [Quantum Diaries](https://www.quantumdiaries.org/2011/11/21/why-do-we-expect-a-higgs-boson-part-i-electroweak-symmetry-breaking/)      [[promnesia]]

doesn't work with readability extension?  
add an explicit "refresh" button?  




## bug: chrome: callbacks stop triggering after I reload the extension manually. ugh. Looks like due to the same callback hacking in background.js      [[promnesia]]





### `[2019-09-09]` right, I guess that's because first page that's opened on chrome is options<sub>page</sub>&#x2026;

maybe frontend pages need to 'ask' backend to register callbacks?&#x2026;  




## need to defensify everything      [[toblog]] [[webext]]




## Expose db from the server??      [[malleable]]




## `[2020-05-11]` [Alexander Flores on Twitter: "@karlicoss having a pane like that but scroll synced to content in article would be ideal for me" / Twitter](https://twitter.com/ajflores1604/status/1259752083315703810)

    having a pane like that but scroll synced to content in article would be ideal for me




## usability: perhaps easier with overlay in the middle of screen? then there are no issues with displaying&#x2026;




## usability: expand all/collapse all




## usability: display summary of available contexts on top?




## display some sort of 'collapsed' dynamic summary with tags and timestamps only? maybe on the side, and you 'zoom' into it as you scroll




## bug: on 'cancel' after blacklist, still shows notification that it added      [[promnesia]]




## ui: split in tabs: annotations + plain visits? maybe even split by provider?




## ui: Sidebar





### `[2019-08-01]` eh, ended up implementing mine for now&#x2026;




### `[2019-07-07]` jeremychurch/FixedContent.js: A mobile-friendly, jQuery plugin that persists sidebar content, nav, etc.

<https://github.com/jeremychurch/FixedContent.js>  
hmm,that looks interesting. sticky  




### `[2019-07-07]` arkon/ng-sidebar: Angular sidebar component.

<https://github.com/arkon/ng-sidebar>  
another sidebar, seems ok  




## `[2019-04-19]` ui: Designing a Personal Knowledgebase – A Curious Mix      [[promnesia]] [[org]]

<http://www.acuriousmix.com/2014/09/03/designing-a-personal-knowledgebase>  
eh, need to improve rendering of context. look at this link, for instance  




### `[2019-12-26]` i guess it was referring to unhighlighted links etc?




## bug: show visited mess with grasp?? (try selecting over these marks and capturing text)      [[promnesia]]




## excludelist: www.site.com vs site.com      [[promnesia]]




# \* github issues





## extension: would be cool to have an option to just 'find' empty space on screen to overlay&#x2026; seems hard though      [[ml]] [[think]]





### `[2019-07-20]` more generally, non-invasive? and not sure if ml is necessary for that at all&#x2026;




## `[2020-09-13]` [Cannabidiol - PsychonautWiki](https://psychonautwiki.org/wiki/Cannabidiol)

extension works weird on this page w.r.t. scrolling  




## multiple processes





### use multiple threads for indexing&#x2026;




### `[2020-11-08]` ugh fuck, def useful for indexing code..




## load more if page is scrolled? gonna be tricky&#x2026;




# \* indexer: bugs/issues





## hmm. if we switch db mode to 'update', then schema changes would break promnesia&#x2026;      [[promnesia]]




# hmm, what if people used it with older orgparse? (suggest to update in release notes)




# personal style settings

    .promnesia *[data-sources*=code] .context {
      font-family: monospace;
    }

    /* tweak 'visited' marks: specify hex color here */
    :root {
      --promnesia-src-sourcename-color: #ff00ff;
      /* e.g.
      --promnesia-src-reddit-color: #ff0000;
      or
      */
      --promnesia-src-twitter-color: #00acee77;
      --promnesia-src-notes-color: #00ff0077;
    }




# `[2020-11-22]` extension: twitter is pretty slow & logs are spammy [Home / Twitter](https://twitter.com/home)

fuck, seems that twitter updates all the time? when scrolling  
also bindSidebarData (in logs) is quite slow and also logs are spammy  




## `[2020-11-23]` ugh, so also impacts 'show this thread'




# `[2020-06-07]` [inkandswitch/ksp-browser: Connect the things you already know in your browser.](https://github.com/inkandswitch/ksp-browser)      [[pkm]]





## `[2020-09-11]` hmm, need to outreach them?




# different notions of 'visited'      [[think]]

one is actually physically clicking  
anothe is visual, i.e. scrape off the links that were on the screen and store (kinda like web archiver/memex)  




# figure out what could possibly be the most interesting source of links for people? I'd imagine whatsapp?





## `[2019-07-15]` reddit definitely. Slightly harder to motivate backups      [[reddit]]




## `[2019-07-15]` could integrate with my reddit backup script then? reindexing would trigger backup; seems kinda ok




## `[2019-08-31]` pocket perhaps?




## `[2019-08-31]` actually, pinboard; keep one backup in repository to test the extractor or demonstrate json extractor?      [[pinboard]]




# `[2019-12-15]` Andy Matuschak on Twitter: "@LiquidTextCorp I'm very excited to try!"      [[motivation]]

<https://twitter.com/andy_matuschak/status/1206055315000528898>  

    @andy_matuschak:  @LiquidTextCorp @spiralstairs
    I'm very excited to try!
    I worry about the opacity of the app container model. Conceptually speaking, I want the LiquidText canvas at the level of the OS! Across not just some PDFs, but also web pages, mail messages, etc. The model pushes towards little app silos—it's a bummer.

should tweet at Andy Matuschak perhaps?  




# `[2020-03-22]` It would be also great if it would work backwards aswell, eg.: "the link I found on twitter last week"

<https://news.ycombinator.com/threads?id=karlicoss#22657236>  

    I love this idea and I would def use it! It would be also great if it would work backwards aswell, eg.: "the link I found on twitter last week"




## `[2020-05-28]` I mean it will once I integrate with the database properly&#x2026;




# `[2020-05-03]` [(7) Spencer Chang on Twitter: "@jborichevskiy @Twitter @Wikipedia @hypothes<sub>is</sub> @RoamResearch Love this have been thinking in the same space where the content you consume is linked in-place to the content you (or the people you think are important) curate. Looking forward to seeing where this goes!" / Twitter](https://twitter.com/spencerc99/status/1256747294482825216)      [[ui]]

    Love this have been thinking in the same space where the content you consume is linked in-place to the content you (or the people you think are important) curate. Looking forward to seeing where this goes!




# `[2020-05-06]` [WorldBrain.io on Twitter: "We are starting the development of the Memex Reader, an offline-first Pocket-style reader for desktop and mobile + mobile annotations. https://t.co/5lUpNSImFe Is anyone interested in collaborating/contributing to this? We need some more (wo)man power. ❤️" / Twitter](https://twitter.com/worldbrain/status/1258031458356277249)      [[worldbrain]]

    We are starting the development of the Memex Reader, an offline-first Pocket-style reader for desktop and mobile + mobile annotations.
    https://notion.so/worldbrain/Reader-Web-Archiver-Mobile-Annotations-extension-mobile-4ce4576dd1154f3f87f33eb6830ecebf
    
    Is anyone interested in collaborating/contributing to this?
    We need some more (wo)man power.




# `[2020-06-22]` [WorldBrain.io on Twitter: "We're working on sharing/collaboration features of Memex and would love to have your input! Watch a quick rundown on some early mockups: https://t.co/brncMElHFr We'd love to have you for a 30-min call to get a grip on your use cases: https://t.co/AT52JajznO" / Twitter](https://twitter.com/worldbrain/status/1275042929845903361)      [[worldbrain]] [[social]]

    We're working on sharing/collaboration features of Memex and would love to have your input!
    
    Watch a quick rundown on some early mockups:
    https://loom.com/share/5d9173ccf63a4865a99c84481abd5347
    
    We'd love to have you for a 30-min call to get a grip on your use cases:




# `[2020-06-17]` [TrailHub on Twitter: "https://t.co/do5RBGjjk4 Ready to give StorexHub a whirl! Take @hypothes<sub>is</sub> annotations, and bookmark the pages in memex so that they will show up as a liked page in memex and be indexed Add Page notes to Memex that link to hypothesis annotations https://t.co/SUk55b3ADn https://t.co/QsybMSwHxo" / Twitter](https://twitter.com/TrailHub1/status/1273226379757322243)

    Ready to give StorexHub a whirl!
    Take @hypothes_is
     annotations, and bookmark the pages in memex so that they will show up as a liked page in memex and be indexed
    Add Page notes to Memex that link to hypothesis annotations




# `[2020-03-21]` westoncb/mymex

<https://github.com/westoncb/mymex>  

    Mymex[0] is an application designed for quick retreival of information from a variety of (web/local) data sources. One of its main goals is to make pieces of information located on the web easier and more reliable to return to. It does this by:
        automatically storing local renderings of web resources
        allowing tags and notes to be attached to web resources




# demo: on malleable systems collective, with screenshot from the chat itself?      [[promnesia]] [[social]]




# usecase: reading hackernews 'new'

-   interesting domains are highlighted
-   users on which profiles I clicked before are highlighted (so I'm likely to pay attention to their posts)
-   posts I've seen before are highlighted (so I get to boost them hopefully to discuss later)




# demo: 'mark visited' on the hackernews top?




# `[2020-02-11]` mek.fyi | Home

<https://mek.fyi/#about-me>  

    Historia (Provenance) #chrome-extension

fuck me! Some very similar goals  




## `[2020-11-19]` tweet at Mek after releasing new version?




# demo: post again on /r/orgmode? with demos of highlights/translusion/backreferences?




# `[2020-11-19]` demo: [good demo for mark visited Subscriptions - YouTube](https://www.youtube.com/feed/subscriptions)

this would be a good demo for 'mark visited'  




# `[2020-11-17]` usecase: [New Links | Hacker News](https://news.ycombinator.com/newest?next=25125588&n=31)

I think I've figured out how to read hackernews 'new' page  




# ugh, something's not working with release build in firefox??

    Error: The storage API will not work with a temporary addon ID. Please add an explicit addon ID to your manifest. For more information see https://bugzil.la/1323228.




# discuss on malleable systems how hard was it to modify youtube's website and inject annotations etc      [[promnesia]] [[outbox]]





## could also discuss with Oliver from worldbrain memex?      [[worldbrain]]




# demo: tweet HN new reading when I encounter some user I know




# publish: release on lobsters? seems ok




# `[2020-11-21]` control logging in content scripts

    Installed it and it seemed to work! But it was spammy in the console and I'm doing webdev, so I had to uninstall it. Would reinstall if you could silence the debug stuff

ugh fuck  




# `[2019-07-08]` testing: unitest/History at master · scriptmasters/unitest      [[hpi]] [[jdoe]]

<https://github.com/scriptmasters/unitest/blob/master/%7E/.e2e-chrome-profile/Default/History>  




# `[2019-11-22]` highlight: <https://news.ycombinator.com/item?id=21403294>

if 'most' of page matches, then highlight is prob. wrong?  




## `[2019-12-27]` I guess if I show it on HN, better get it right




# test: for the end2end test, run it against a database indexed with an older (PIP) version





## `[2020-11-19]` actually not super important; in most cases database is overwritten




# docs: make sure it's possible to run merely by creading config, then index, then serve

test it on a fresh docker  




# Please visit <https://editorjs.io/> to view all documentation articles.  Base concepts




# for demo, could just anonymize people? that would solve 99% of it      [[promnesia]] [[demo]]




# `[2020-05-11]` [deen-chan on Twitter: "@ajflores1604 @karlicoss @jborichevskiy I've implemented this (augmented sidebar) and it's quite hard to come up with something that works well for all sites. You quickly run into sites which don't reflow, assuming a certain layout. But that was years ago. Responsive design is a lot more common these days so might work" / Twitter](https://twitter.com/sir_deenicus/status/1259792881679818752)

    deen-chan
    @sir_deenicus
    Level 5:
    Replying to
    @ajflores1604
    @karlicoss
     and
    @jborichevskiy
    I've implemented this (augmented sidebar) and it's quite hard to come up with something that works well for all sites. You quickly run into sites which don't reflow, assuming a certain layout. But that was years ago. Responsive design is a lot more common these days so might work




# `[2020-07-05]` [Guide to using filemagic — filemagic 1.6 documentation](https://filemagic.readthedocs.io/en/latest/guide.html)

    Before installing filemagic, the libmagic library will need to be availabile. To test this is the check for the presence of the file command and/or the libmagic man page.




# `[2020-05-20]` [I remember using this software last time, it is wayyyy~ too buggy, it stalls, cr&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23230915)      [[promnesia]] [[worldbrain]]

    I remember using this software last time, it is wayyyy~ too buggy, it stalls, crashes, and slows down the browser. Also that import feature is actually crawling the site, beware if you are using a proxy or something with rate limit.




# fucking hell. figure out how to fix version exposed during the adhoc install&#x2026;.




# `[2019-12-12]` demo: Digital Tools I Wish Existed :: Up and to the Right — Jonathan Borichevskiy

<https://jborichevskiy.com/posts/digital-tools>  
potentially good example of highlights  
also they don't look quite well in dark mode?  




## `[2020-03-28]` maybe make a screenshot out of it?




# `[2020-05-20]` [Introduce Yourself - Thinking Tools](https://thinkingtools.space/t/introduce-yourself/16)      [[social]] [[publish]] [[promnesia]]




# `[2020-04-29]` integrate in Memex?      [[worldbrain]]




# post automatic demo gifs      [[publish]]




# doc: minimal example to import something in promnesia, with crontab examples etc      [[promnesia]]




# maybe it should be `emacs://` ? not sure      [[mimemacs]] [[promnesia]]





## `[2020-05-21]` or `editor://` ??




## `[2020-05-29]` ok, so it seems that emacs:/// works and is backwards compatible, which is kinda good news

for editor, could set it up as mime type? dunno.  




### `[2020-05-30]` right. so I guess I know what to do

-   During the indexing, detect either. If detected emacs:, then warn about deprecation and suggest to remove  
    Need to think how to accumulate indexing warnings and show in the end&#x2026; but later I guess  
    If only old script detected, use emacs://, otherwise use editor://
-   still can't use line=, col= because extension wouldn't support it. Or maybe it's fine actually!  
    Version it!




## `[2020-05-29]` could add to doctor?




## `[2020-11-01]` maybe mimes should be configured & tested in the frontend? could add to the extension troubleshooting page




# `[2019-12-08]` motivation:

<https://news.ycombinator.com/threads?id=grblovrflowerrr&next=17598881>  

    j2kun on June 1, 2018 [-]
    How is this like the demo? This looks like "unify all N productivity apps; now I have N+1 productivity apps!"




# demo: of 'mark visited'      [[toblog]] [[promnesia]]

also use some guessing magic to quickly disable it? could test on <https://pinboard.in/popular/>  
or just hide stuff that linked more than once on the page?  




## `[2020-05-16]` hmm, make sure visited marker/css is tweakable? I suppose it needs to be in the 'main', sidebar section. confusing&#x2026;

if I make marker larger instead and the same color as links, it might be easier to filter out visually?  

    proromnesia-visited::after {
        content: "⚫XXXXX";
        color: #FF4500;
        vertical-align: super;
        font-size: smaller;
        user-select: none;
        position: absolute;
        z-index: 100;

actually even this works quite well  

    .promnesia-visited {
        background-color:
        red;
    }

TODO filter: invert, but don't think it's possible without js?  
border actually works quite well!  
this isn't supper pretty, but enough to visually glance and notice  




### `[2020-05-16]` post about it &#x2013; why don't we abuse a human brain which is much better at pattern recognition than computers (so far)




# publish packed zips in releases; assemble automatically on ci      [[ci]] [[webext]] [[promnesia]]




# remove 'duration' from the database? hopefully no one uses it yet&#x2026;





## `[2020-05-14]` actually I might need it later.. if I populate them from #arbtt




# `[2020-01-13]` usecase: l3kn/org-fc: Spaced Repetition System for Emacs org-mode

<https://github.com/l3kn/org-fc>  

    drill

very nice, apparently ran into that guy on merveilles and was able to track it in search!  




# `[2019-11-01]` ui: Shtetl-Optimized » 2016 » April

<https://www.scottaaronson.com/blog/?m=201604>  
maybe, make the notification more subtle?  




## `[2019-11-04]` allow to be configured via CSS





### `[2019-11-04]` how to automate it actually?




# `[2019-11-09]` bug: Introduction - Everything I know

<https://wiki.nikitavoloboev.xyz/?q=gree>  
constantly reloads on this page :(  




## `[2019-11-12]` eh. fair enough, it's changing URL. Not sure if there is much that can be done?





### `[2019-12-25]` except if cannon works clientside. Ugh!




## `[2019-12-07]` can be solved temporarily with proper blacklisting




# be less annoying about errors.. not sure how though      [[errors]]





## `[2019-08-31]` just implement different options for notifications?




## `[2019-09-01]` quick option do disable/enable notifications; later find some generic component to snooze them?





### `[2019-09-09]` yeah, I guess they'd be ok on sidebar? Basically, make sure sidebar <span class="underline">always</span> slides since it's convenient for settings, access to search etc.




# Def need way to make it less spammy on network errors on phone. System wide notification is too much      [[errors]]




# test going to different url in same tab; not sure how it would work&#x2026;




# support stuff without tz? or at least warn and maybe instert as utc. or  just pass forward local tz that's ok for most people




# `[2019-08-29]` mozilla/webextension-polyfill: A lightweight polyfill library for Promise-based WebExtension APIs in Chrome      [[webext]]

<https://github.com/mozilla/webextension-polyfill>  
Use this thing?  




# `[2019-09-10]` handle when pages aren't available better

<https://tuxspace.net/@Qwxlea>  
check when pages are not available&#x2026;  




## `[2019-09-23]` need to implement at least popup




# `[2019-09-05]` lukeed/tinydate: A tiny (349B) reusable date formatter. Extremely fast!      [[datetime]] [[js]]

<https://github.com/lukeed/tinydate>  




# `[2019-07-14]` Surprisingly Turing-Complete - Gwern.net

<https://www.gwern.net/Turing-complete#on-seeing-through-and-unseeing>  
anchors are good examples of 'direct' visits and siblings?  




# I guess sort of killer feature would be 'hierarchical' visits (e.g. facebook pages, reddit comments, github. etc. for reddit will require some manual rules against canonified urls)





## `[2019-07-22]` search kind of contributes towards that




# stuff in database seems to be unnormalised (e.g. case). need some sort of checker &#x2026;      [[cannon]] [[togithub]]





## `[2019-06-16]` hmm, do that I guess  sqlite3 visits.sqlite "select norm<sub>url,tag</sub> from visits where norm<sub>url</sub> LIKE '%usg%'"




# useful to populate from old backups (e.g pinboard) in case I delete articles/bookmarks      [[motivation]] [[promnesia]]

-   State "STRT"      from "TODO"       `[2019-03-12]`




# filter links

    chrome:// (history/apps/newtab
      newtab is interesting data though!




# warn about anomally long histories?




# would be nice to process links/pieces of information that I merely seen!




# like hypothesis, but process the page server side and highlight against everything in the knowledge base      [[hypothesis]] [[pkm]] [[promnesia]]




# would be nice to know how I got onto the page&#x2026;      [[promnesia]] [[motivation]]





## `[2019-06-02]` use chrome from<sub>visit</sub>?




## `[2021-01-20]` search basically does this




# need some thing which normalises and merges messages? or maybe just disregard duplicate links from old and new backups&#x2026;      [[backup]] [[telegram]] [[promnesia]]




# could analyse 'how did I get there' from my web archives      [[archivebox]]





## `[2019-07-31]` I guess I meant from plaintext search




# publish: /r/dataisbeautiful post my visited urls stats?




# Tweet from 𝔊𝔴𝔢𝔯𝔫 (@gwern), at Mar 10, 23:59      [[promnesia]] [[motivation]]

    Several times in the past few weeks I or an acquaintance read something awesome only to realize we'd read it years ago & simply forgot! Another use for 'anti-spaced repetition' (https://t.co/jD4SsY6VBW): track great stuff & remind you to re-read it only 𝘢𝘧𝘵𝘦𝘳 it's forgotten.

<https://twitter.com/gwern/status/1104879445368864773>  




# `[2019-04-15]` Pinboard: bookmarks for tswaterman tagged 'math'

<https://pinboard.in/u:tswaterman/t:math/>  
I definitely need to integrate promnesia crawling with webpages backups, that way I'd have way more context  




# locators need short name along the full path




# hmm, def looks like chrome is syncing bits of local database as well. ugh




# polar got OK design for sidebar      [[polar]] [[promnesia]] [[inspiration]]




# custom search engine?      [[search]]




# 'came from' is just a context. Would cover 99% of cases




# tags are pretty useful&#x2026;




# Works really well in conjunction with axol (both dots and contexts)      [[axol]] [[promnesia]] [[motivation]]

Example a complete guide for tagging  




# showvisited: show dots on selection? useful so you don't need to send too many queries. or anchors like surfingkeys?




# display error in sidebar?      [[errors]] [[ui]]





## `[2019-07-14]` could be useful if we can extract URL; but encountered some issues while extracting context etc; could emit both visit and error




# not sure, maybe I should just use native async/await? Most mobile and desktop browsers support it





## `[2019-07-15]` generally figure out how much can I get away with using modern JS as opposed to webpacked

also def worth it for debugging and developing  




# go through existing urls and try to normalise them?      [[webarchive]]




# ught <https://github.com/brookhong/Surfingkeys/blob/57fccbbeeb60ee2be0d2d60cfc50bd3aca3b0436/background.js#L1094>      [[webext]]

switching frames works fine on <https://web.hypothes.is/blog/annotation-is-now-a-web-standard/>  
though  




## `[2019-07-07]` shit. ok, so chrome experiment confirms that it just doesn't work for extensions.




## `[2019-07-07]` shit. do I need bookmarklet or what???




# `[2019-07-08]` Search · filename:places.sqlite <https://github.com/search?p=2&q=filename%3Aplaces.sqlite&type=Code>




# `[2019-07-14]` mitchellkrogza/Ultimate.Hosts.Blacklist: The Ultimate Unified Hosts file for protecting your network, computer, smartphones and Wi-Fi devices against millions of bad web sites. Protect your children and family from gaining access to bad web sites and protect your devices and pc from being infected with Malware or Ransomware.

<https://github.com/mitchellkrogza/Ultimate.Hosts.Blacklist>  




# merge results together? e.g. search for inmotionmagazine




# `[2019-03-08]` motivation: Nikita Lisitsa on Twitter: "@<sub>bravit</sub> У меня так на stackoverflow / math.stackexchange бывает. Ищу ответ на вопрос, нахожу, читаю, ставлю лайк - "вы не можете поставить лайк своему собственному посту"." / Twitter      [[promnesia]]

<https://twitter.com/lisyarus/status/1104104035588755457>  




# `[2019-07-08]` Does Firefox ship with a new default for "history expires after&#x2026;"? - Super User

<https://superuser.com/questions/1114637/does-firefox-ship-with-a-new-default-for-history-expires-after>  

    places.history.expiration.max_pages is maximum number of pages that are retained before pages are expired.
    I had system disk fil




## `[2019-07-08]` Does Firefox ship with a new default for "history expires after&#x2026;"? - Super User

<https://superuser.com/questions/1114637/does-firefox-ship-with-a-new-default-for-history-expires-after>  

    Workaround
    Consider using the extension Expire history by days.
    Ironically this extension was written by the developer who changed the previous behaviour. See the blog post below.




# for mimemacs, could probably support vim primarily (since all users will have it), it could even fallback      [[mimemacs]]




# `[2019-07-23]` demo: Best Mangal Bar & Kitchen delivery from Farringdon - Order with Deliveroo

<https://deliveroo.co.uk/menu/london/farringdon/best-mangal-farringdon>  
allow breaking down important and unimportant schema parts from extensions?  




# rss blogs, easy to see what clicked and what hasn't      [[rss]]




# should show visual indication on 'no results'




# when I merge together browser activity etc, I need to assert on some historic entries to make sure timestamps match properly




# would be too annoying to deal with transitions I guess, considering that it's not needed too often. Just rely on jumping into timeline?





## `[2019-08-01]` ??




# open in new tab from search?




# how did I get here &#x2013; perhaps shouldn't mix context and visits??




# yeah, searches useful to have in db for context; even though they'd almost never match and normalise




# yeah, show url split in parts; then when I click one of the parts in queries more data?




# direct link to css from the extension?





## `[2020-04-28]` I guess this is possible judging by greasemonkey




# could expand the grouped things on grey area press?      [[promnesia]] [[togithub]]




# maybe use two locators? one for linking and one for debugging





## `[2019-12-26]` eh?




# moz-extension://b966cab9-aded-44e8-b116-a900ab825442/search.html?timestamp=1561844122.151 

looks sort of messy. should collapse and somehow make more unique&#x2026;  




# hmmm author<sub>url</sub> could be useful?      [[hpi]] [[reddit]]

media<sub>embed</sub> only got html  
secure<sub>media</sub>\_ contains more stuff and could actually be useful  

ugh. some have both media and secure<sub>media</sub>??  




# bug: on android doesn't respond well on filter clicks, and overall looks a bit weird..




# shows notification on navigation within page when clicking anchors <http://super-memory.com/articles/sleep.htm#biphasic_sleep> ,perhaps shouldn't do that&#x2026;




# enable back options to always show dots on visited urls?




# `[2019-08-31]` uBlock/manifest.json at 6c34b3c3c96756b6db7ff2f3a0394472d81cde3e · gorhill/uBlock      [[webext]]

<https://github.com/gorhill/uBlock/blob/6c34b3c3c96756b6db7ff2f3a0394472d81cde3e/platform/webext/manifest.json>  

    "optional_permissions": [
       "file:///*"
     ],




# allow per-device settings?      [[webext]]




# bug: on restoring tab, shows notification twice. weird

in debugger looks like code just starts running at     for (const action of (await actions()))  




## `[2019-09-22]` doesn't seem to do with hacky injector backed initialization either. odd




## `[2019-09-22]` also only happens in firefox, apparently&#x2026;




# <https://slatestarcodex.com/2014/03/17/what-universal-human-experiences-are-you-missing-without-realizing-it/> 

looks like some visits duplicate; and also they aren't grouped  




# `[2019-07-30]` hmm it triggers on clicking anchors. not sure it's a good idea? also add to end2end tests

<https://beepb00p.xyz/annotating.html#org000001b>  




# local sync vs cloud? Not sure how to handle this properly; maybe have different profiles?




# `[2019-09-09]` test: fabianonline/telegram<sub>backup</sub>: Java app to download all your telegram data.

<https://github.com/fabianonline/telegram_backup>  

    fabianonline/telegram_backup

clicking on title causes page reloading, also shows notification etc. a bit spammy. I guess for now having setting to prevent context notification is OK  




# fails on firefox.com domain; fair enough, but perhaps need to blacklist it?




# missing host permission &#x2013; very consistently reproduces on test<sub>visits</sub> if you close/reopen tab




# shit, tag map didn't work with context visits




# have 'primary' settings profile and just think about rest later      [[webext]]




# on android, maybe should only request on sidebard click? doesn't display icon anyway&#x2026; then basically it'd solve systemwide notification thing      [[promnesia]] [[togithub]]




# :invalid selector and input validation      [[blog]] [[webext]]




# `[2019-10-19]` Re: [fregante/webext-options-sync] Race condition in OptionsSync constructor




# Highlight blacklisted and paywalled websites

Like ft, technology review  




## `[2020-11-19]` with mark visited it's much easier now.. could even have a special source and apply special style to them?




# `[2019-11-04]` performance: vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources

<https://github.com/vinta/awesome-python>  

    Loggi

pretty slow on thins page&#x2026; I guess highlights  




## `[2020-11-14]` hmm, now it's fine but it highlights a bit too much info? not sure what to do about the fragment normalisation&#x2026;




# `[2019-11-04]` promnesia/hypothesis.py at master · karlicoss/promnesia

<https://github.com/karlicoss/promnesia/blob/master/src/promnesia/indexers/hypothesis.py>  

    # TODO what I really need is my hypothesis provider... is it possible to share somehow?
    for x in annotations:

I think I need to figure out how to make them standalone basically? Need some sort of defensive policy for dependencies?  




# `[2019-11-09]` On todo lists | beepb00p

<http://127.0.0.1:8000/pkm-todos.html>  
bindSidebarData fails on quick refresh  




# Tweet from Will Manidis (@WillManidis), at Nov 26, 15:44

    I spend my life copy/pasting links and screenshots of interesting content to friends. Solving infrastructure level information-transfer problems like this is also core to accelerating human progress.
    @shohinigupta built something amazing to solve this

<https://twitter.com/WillManidis/status/1199337719295381509>  




## `[2019-12-26]` ugh, tweet is gone??




# ui, phone: don't really have to tweak body? as it's easy to hide/show sidebar      [[promnesia]] [[togithub]]




# I don't like some twitter account I'm following: they are whining too much or whatever      [[twitter]] [[promnesia]] [[motivation]]

but why did I follow them in the first place, there must have been good reason?  




# Build client only version as demonstration?




# query database

    sqlite3 promnesia.sqlite 'SELECT norm_url, group_concat(src) FROM (SELECT norm_url, src FROM visits WHERE context != "" ORDER BY norm_url, src) GROUP BY norm_url'  | grep instapaper | grep notes | less




# org-mode: comments from LOGBOOK might be useful..      [[org]]




# for search might be good to display original link??

e.g. how did I get here?? <https://mortoray.com/2019/06/11/a-failed-experiment-with-python-type-annotations/>  




# `[2019-12-15]` bug: Теория вычислимости — Викиконспекты

<http://neerc.ifmo.ru/wiki/index.php?title=%D0%A2%D0%B5%D0%BE%D1%80%D0%B8%D1%8F_%D0%B2%D1%8B%D1%87%D0%B8%D1%81%D0%BB%D0%B8%D0%BC%D0%BE%D1%81%D1%82%D0%B8>  
not sure, shouldn't show popup on every transition&#x2026; have a timer or something?  




# Could map different people onto the same 'entity'?




# after loading browser with previously open tabs and then closing them; shows 'host permission' warning




# should allow running against live database? really why not, could be nice for exploring




# Maybe git tracked server config is not so bad




# Use hub/click? And maybe docker to isolate      [[docker]] [[python]]




# Would be rad if it was possible to simply run it against GitHub repo straight from ui




# `[2020-01-25]` Robot&AIWorld on Twitter: "Here's more footage of MIT's Mini Cheetahs cavorting, frolicking, back-flipping, playing soccer and generally acting fun and cute, courtesy of the Biomimetic Robotics Lab @MITMechE  <https://t.co/8ZQzDvCDVW>" / Twitter

<https://twitter.com/RobotAndAIWorld/status/1192429991813881856>  
should be handled, I liked/RTd it on twitter  




# Allow raw settings backup      [[webext]]





## `[2021-01-20]` this should really be easier&#x2026;




# shit, google docs trigger a lot of reloads.. really should debounce




# duplicating search page &#x2013; fucking hell. still happens on firefox&#x2026;




# chronic versioning?      [[project]]




# ugh. subdomain needs to be banned..

www.services.online-banking.hsbc.co.uk  




# `[2019-12-27]` Adventures in WhatsApp DB — extracting messages from backups (with code examples)      [[promnesia]] [[whatsapp]]

<https://medium.com/@1522933668924/extracting-whatsapp-messages-from-backups-with-code-examples-49186de94ab4>  
wow, someone managed to get whatsapp export working?  




# `[2019-12-30]` What am I meditating for? In Pursuit of A Definition of Meditation - Mark Koester

<http://www.markwk.com/what-is-meditation.html>  
Highlight domain differently?  




# warning about module size&#x2026;

<https://webpack.js.org/guides/code-splitting/>  




# not sure about tabs vs activeTab permission      [[webext]]

e.g. if the page is updated in the background (e.g. youtube video), do we want to refresh promnesia stats? although it's basically only limited to youtube  




## `[2020-02-15]` maybe instead I could simply check last requested url on tab switch?




# ok, I guess I could make "tabs" an optional permission; by default only request stuff via click on a popup (that requires 'activeTab'?)




# shit, request on every tab switch is not good&#x2026;




# `[2019-08-10]` right, chrome doesn't support android extensions. could use bookmarklet or something?? <https://stackoverflow.com/a/10606887/706389>




# as a docker app?




# go through code and create issues?




# eh, web indexer doesn't really work for relative links&#x2026;




# combine with eye tracking, then could know how much time was spent reading something&#x2026;




# would be nice to get stuff collected by axol to promnesia database      [[axol]] [[promnesia]]




# shit, 2mb per single page (10K visits) sucks&#x2026;. wonder if should use some different protocol? Or gzip defeats the purpose?




# `[2019-12-05]` Erik Torenberg (@eriktorenberg) / Twitter      [[motivation]] [[demo]]

<https://twitter.com/eriktorenberg>  
ran into twitter account recommendation (by michael nielsen, clicked it, found out I've already got few liked tweets by that guy  




# use dev webdriver??

    profile = webdriver.FirefoxProfile('/home/xxx/.mozilla/firefox/abadadw.dev-edition-default')




# demonstrate on that place with great bread      [[promnesia]] [[demo]]




# `[2020-01-25]` hyperhype/hyperscript: Create HyperText with JavaScript.

<https://github.com/hyperhype/hyperscript>  




# `[2020-03-30]` Troubleshoot extensions, themes and hardware acceleration issues to solve common Firefox problems | Firefox Help      [[webext]]

<https://support.mozilla.org/en-US/kb/troubleshoot-extensions-themes-to-fix-problems#w_checking-extension-settings>  




# maybe add sidebar menu on mobile only? anyway, need to add blacklist




# 'mark visited' works really nice on the phone




# doesn't work in private windows (I assume because of the getActiveTab thing)




# common usecase &#x2013; I follow someone, then I'm annoyed by their tweets and try to figure out why had I followed them in the first place?




# Maybe we just need a proxy that logs literally all of http requests.. That way history could be agnostic




# shit, webdriver only took screenshot of half of the frame&#x2026;.




# not compatible with gh: style links&#x2026;




# `[2020-04-07]` usecase: Idle Words <https://idlewords.com/>




# could test on twint??      [[twitter]]




# usability: keyboard navigation      [[webext]] [[malleable]]

<https://github.com/karlicoss/promnesia/issues/13>  




## `[2019-08-01]` ugh. surfingkeys is capable of working on my iframe, but can't switch

look somewhere along  
<https://github.com/brookhong/Surfingkeys/blob/57fccbbeeb60ee2be0d2d60cfc50bd3aca3b0436/background.js#L1091>  
<https://github.com/brookhong/Surfingkeys/blob/f27a6cd30df285b05d78922a201b9e71912edd0e/content_scripts/front.js#L362>  




## `[2019-08-26]` at least write about it in readme/faq




# could draw a small 'visits/contexts' tree? would be fun..




# maybe backend could update rules now and then..      [[cannon]]




# Breakdown of contexts by parts of virtual url in the sidebar




# attemt to set up autorealoding      [[promnesia]] [[webext]]

    web-ext run --verbose in the extension folder

had some issues  
changes were detected on touch, but not on build  
   clean plugin should be handling properly, i.e. keeping dist/ dir and only removing files  
    <https://github.com/johnagan/clean-webpack-plugin/issues/106>  
   tried commenting/uncommenting clean plugin, and then it stopped happening????  

in the future, try to investigate it by going to dist/ dir and trying ls in terminal  




# Write a post demonstating which bits should not be part of extension      [[malleable]] [[promnesia]] [[toblog]]

Codejar/codemirror &#x2013; let the user choose the editor  
Linkify &#x2013; third party link hihlighter  
What else???  




# Hmm. Sending fragment can be unsafe?

    I think this part is a little off:
    > Perhaps you have no sympathy for web applications that store sensitive data in query strings, as that’s widely recognized as an insecure pattern. The URL fragment is more serious. That otherwise is a safe way to store sensitive information, so it’s alarming to see a third-party library sending a copy to an external server.
    > Firefox Send and Mega.nz are both examples of popular web apps that use the URL fragment to store client-side encryption keys so that users can save end-to-end encrypted files to the cloud without the server ever having access to the underlying data.
    The URL fragment is not designed to be any more secure than anything else in the URL, it's just a funny quirk of how web browsers evolved that it doesn't happen to be sent to the webserver. That popular platforms are (mis)using it to pass information without that information hitting their webservers is unfortunate. But it doesn't mean that the URL Fragment is somehow special or should be thought of as "secure" - that's not a guarantee that the URL scheme makes.
    For example, those fragments will easily appear in browser history for anyone else who uses your same device...




# use arbtt to match the browsing history? that would be fun&#x2026;      [[arbtt]] [[hpi]]




# readme: probably, better to install it via pipx? so HPI etc are easier to upgrade?      [[python]] [[promnesia]]




# `[2019-11-21]` raxod502/mercury: Emacs interface to Facebook Messenger      [[facebook]] [[hpi]]

<https://github.com/raxod502/mercury>  




## `[2019-12-02]` could be useful&#x2026;




# `[2019-09-22]` 1397667 - "No matching message handler" error when tabs.update().then(tabs.executeScript())      [[webext]]

<https://bugzilla.mozilla.org/show_bug.cgi?id=1397667>  




# `[2019-09-22]` 1290016 - tabs.executeScript in webRequest.onCompleted gives "Unchecked lastError value: Error: No matching message handler"      [[webext]]

<https://bugzilla.mozilla.org/show_bug.cgi?id=1290016>  




# visual web scraper? geoffrey litt mentioned generalised nocode stuff (Pavel's question)




# `[2020-05-07]` [eslint-plugin-no-unsafe-innerhtml - npm](https://www.npmjs.com/package/eslint-plugin-no-unsafe-innerhtml)      [[webext]]




# be more informative; show full history or at least last visit and potentially sources (e.g. hypothesis)

maybe icons for mobile/desktop?  




# attempt at agnostic url extraction (sha ae889fa0fb99f683cd1ba6192a3b55d11a481558)      [[reddit]] [[promnesia]] [[hpi]]

I mean not sure what I feel about it. it's very adhoc in the first place, and still requires some hardcoded knowledge about useful and useless fields. I suppose not worth it at this stage  




# demonstrate jumping to the message on android? ironically it works better on phone      [[promnesia]] [[demo]]




# time spent? only for chrome apparently      [[promnesia]] [[demo]]

could make a screenshot from a test<sub>chrome</sub><sub>visits</sub> test  




# Annotating post      [[worldbrain]]

    I have been using Memex for more than a year now. Here are the things that really annoy me
    - occasional freezing and sudden disappearance of your bookmarks
    - no real way to programmatically access your Memex database. I know they have released the storage backend, but the lack of helpful documentation is a deal-breaker.
    - lack of collaborative annotation (the way Hypothesis does)
    - only few results in search results!




# `[2020-05-20]` [Memex/manifest.json at develop · WorldBrain/Memex](https://github.com/WorldBrain/Memex/blob/develop/src/manifest.json)      [[project]]

    "omnibox": {
        "keyword": "m"
    },

nice idea&#x2026;  




# `[2020-05-23]` [Programming Inside a Container | Hacker News](https://news.ycombinator.com/item?id=23275315)      [[docker]] [[hpi]] [[promnesia]]




# what if I could apply :visited state for links that I marked as seen?




# settings &#x2013; add visual cues for dots/ visits/contexts/sources




# `[2020-05-13]` [Native Messaging - Google Chrome](https://developer.chrome.com/extensions/nativeMessaging)      [[webext]] [[promnesia]]




# `[2020-05-27]` [Show HN: Obsidian – A knowledge base that works on local Markdown files | Hacker News](https://news.ycombinator.com/item?id=23324598)





## `[2021-01-20]` some people apparently already used against obsidian db?




# Lesson       [[promnesia]] [[publish]] [[think]]

Maybe a big lesson is that I need to write about ideas, frustrations and experiments earlier.  
I could have released promnesia on hn a year ago and by now could repost again! Crazy!  




# Hmm, maybe do not highlight stuff from archived org files/deleted instapaper/etc?

Hmmm. I guess src map is going to be js hook for dynamically transforming visits? Provide a small dsl  




# Introduction to Marionette — Firefox Source Tree Docs 78.0a1 documentation      [[webext]] [[promnesia]]

<https://firefox-source-docs.mozilla.org/testing/marionette/Intro.html>  




# tried disabling logic for single background page &#x2013; doesn't help even with persistent background..




# `[2019-05-24]` useful to have links just added to instapaper to know that you are planning to read them there




# `[2020-04-29]` [TypeError: can't access dead object - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors/Dead_object)

shit.. wonder if it could happen because of messing with window. or something??  




# `[2020-05-05]` [type alias to union is invalid in runtime context · Issue #5354 · python/mypy](https://github.com/python/mypy/issues/5354)

usecase: find all occurences of the bug in your code (e.g. if it got fixed)  




# docs: mention that I'll be posting about breaking changes in releases





## `[2020-05-29]` even better to do this in commits and simply reference stuff in releases? or, sync releases with a file in repository




# `[2020-06-03]` [Using Service Workers - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API/Using_Service_Workers)      [[webext]]




# `[2020-06-03]` highlights: [Quora Answers by David Pearce (2015 - 2020) : transhumanism with a human face](https://www.hedweb.com/quora/2015.html#purposesuf)

not great here  




## `[2020-11-14]` hmm, performance OK, but it throws ruandom erros now??




# They record where you come from, what pages you visit, how long you stay on each, where you click and where you go next.

imagine if this information was available to you instead  
[Against an Increasingly User-Hostile Web - Neustadt.fr](https://neustadt.fr/essays/against-a-user-hostile-web/)  
[in context](https://hyp.is/skitAqDSEeqkeb8sgw1DCw/neustadt.fr/essays/against-a-user-hostile-web/)  




# `[2019-07-28]` [Firefox doesn't recognize telegramdesktop's tg link.](https://reddit.com/r/firefox/comments/6p6470/firefox_doesnt_recognize_telegramdesktops_tg_link/dpap5ok/) /r/firefox      [[telegram]]

    I bumped on this post today while I was trying to find the solution for the org capture protocol. It's been a while since you posted it, but no one posted the solution, so I guess this might be helpful.
    The thing is that any new protocol must be introduced by clicking on the link instead of passing the address to the location bar directly. Once you connect the new protocol with the app it will work regularly.
    * Go to `about:config`
    * Add new boolean named `network.protocol-handler.expose.tg` and set it to `false`
    * Create the link by opening an empty tab and typing the following in the location bar
    `data:text/html,<a href="tg://resolve?domain=Bold">Link</a>`
    * Click on Link and Firefox should ask you to choose the program
    * Check the box in order to remember it for future use




# `[2020-05-25]` [Dmitry Bobrov on Twitter: "@karlicoss No idea about the service, but I do have experience with Chrome extensions if that’s what you mean" / Twitter](https://twitter.com/dvbobrov/status/1264995425175711745)

    No idea about the service, but I do have experience with Chrome extensions if that’s what you mean




# `[2020-06-11]` doc: [Share database between machine? · Issue #114 · karlicoss/promnesia](https://github.com/karlicoss/promnesia/issues/114#issuecomment-642710398)




# reuse readability extensions for better content highlight?




# could use both for reddit cumulative state and promnesia browser exports      [[hpi]] [[reddit]] [[cachew]]




# Post archive org highlights      [[outbox]]




# merge mode &#x2013; could combine public and private data




# `[2020-05-11]` [ESLint v7.0.0 Released | Hacker News](https://news.ycombinator.com/item?id=23143315)      [[promnesia]] [[webext]]

    There is a rule in eslint that warns you when a promise is dangling and hasn't been handled.
    
    PLEASE USE THAT RULE. So many bugs in the JS world is because of dangling promises.




# `[2020-05-25]` [Korobochka on Twitter: "@karlicoss Via Twitter?) For the last ~6 months I am developing a Chrome extension at work, can take a look as well." / Twitter](https://twitter.com/korobochka191/status/1265029486782922752)

    Via Twitter?)
    For the last ~6 months I am developing a Chrome extension at work, can take a look as well.




# version detection &#x2013; thing in cachew works pretty well? perhaps it might not work without installing, but otherwise should?




# HPI/promnesia: a whitepaper?      [[publish]]




# ok, could use some design inspiration from ampie      [[ampie]]

-   floating sidebar. make the position configurable, so it doesn't overlap with other potential extensions
-   hmm. for firefox it knows the time spent?? I wonder how  
    uhoh. seems like it's keeping track via js&#x2026; <https://github.com/posobin/ampie/blob/da50f2c5abc1b59de2fc8379b13c7d6d813577e7/src/main/ampie/content_script/amplify.cljs#L328>
-   site icons &#x2013; although not sure how to extract them.. from the browser history?  
    def site icons for sources? Could specify sources favicons in js config, maybe
-   moz-extension://d55e97e7-da63-4685-a3bc-dffc93092eb4/hello.html &#x2013; very nice&#x2026; perhaps could include promnesia tutorial
-   list of all links on the page &#x2013; nice!




# `[2020-09-25]` [(20) Anyone use Promnesia? | Building a Second Brain](https://building-a-second-brain.circle.so/c/emacs-org-mode/anyone-use-promnesia)




# hm, for serving reuse config, but allow to split config bits to make defensive?? not sure..




# could use pandoc for serving HTML?

one downside is that need to return both? one for display, another for matching highlights?  




# about realtime indexing (give a demo of entr??)      [[totweet]] [[promnesia]]




# support child visits etc for inbrowser history




# dynamic JS hook only in dev mode?




# how to display warnings in the very end? extract from warnings module maybe?




# using generators to defer UI updates?      [[toblog]] [[promnesia]] [[js]]




# ideally configuration would be kinda like a grid? for every (almost) source and for every function




# sharing links with surfingkeys? e.g. they could both filter crap links




# sidebar isn't opening if new tab, then google search (firefox)




# check blacklist right before querying backend as the last resort?




# for excludes, 'do not mark this link' and 'do not mark this element'&#x2026; the latter is gonna be way harder      [[togithub]] [[promnesia]]




# usecase: when I follow someone on github/twitter/etc I'll make a quick note. Next time I'll know why      [[demo]]




# `[2020-11-10]` [inkandswitch/ksp-browser: Connect the things you already know in your browser.](https://github.com/inkandswitch/ksp-browser)

    Backlinks
    
    A backlink is a link to this page from somewhere else you've been. It might be a blog post you read, or another page on the same site. It could also be a link saved in a local note on your computer.




# `[2020-11-19]` [Essays · Gwern.net](https://www.gwern.net/index)

tweet at gwern & share  




# `[2020-11-18]` [Watch later - YouTube](https://www.youtube.com/playlist?list=WL)

share youtube watchlist with highlights  




# `[2020-11-17]` [Merveilles   ](https://merveilles.town/web/getting-started) it's pretty dynamic and might not work well with 'mark visited'

some websites  

basically log them along with the URL  




# `[2020-11-17]` [Withings body+ vs. Withings body cardio : QuantifiedSelf](https://www.reddit.com/r/QuantifiedSelf/comments/jp9xw5/withings_body_vs_withings_body_cardio/)

for mark visited blacklist, need to normalise? not sure&#x2026;  
I guess ideally, yes..  




# `[2020-11-14]` [What forces layout/reflow. The comprehensive list.](https://gist.github.com/paulirish/5d52fb081b3570c81e3a)




# `[2020-11-16]` [TweetDeck](https://tweetdeck.twitter.com/)

sidebar isn't closing on this page..  
unless you press 'close'?? wtf..  




# hmm, could serve the exlcudelist from the backend???




# `[2020-11-22]` [The File System Access API: simplifying access to local files](https://web.dev/file-system-access/)      [[promnesia]]




# visited marks might impact ellipsized content

<https://github.com/karlicoss/promnesia>  




# faq: some pages may prevent extensions on working on them

    Content Security Policy: The page's settings blocked the loading of a resource at inline ("style-src").




## `[2020-11-22]` eh, not sure if this is the case with extensions? bookmarklets (like Hypothesis on HN &#x2013; yeah)




# Add donation link, to bastien?




# if I use sidebar, it will work even on websites that forbid html injections?      [[togithub]] [[firefox]]




# maybe I need something a bit more discrete for contexts notification&#x2026;




# shows host error exceptions in firefox on pdfs      [[promnesia]] [[togithub]]

<https://www.fordfoundation.org/media/2976/roads-and-bridges-the-unseen-labor-behind-our-digital-infrastructure.pdf>  




## `[2019-12-26]` could be disabled via blacklisting \*.pdf probably?




# process archive as well?      [[promnesia]] [[org]] [[togithub]]




# could hide annotations via tags?      [[promnesia]] [[togithub]]




# backlist: tampermonkey?





## `[2020-11-16]` eh?




# `[2020-05-25]` [iorate/uBlacklist: Blocks specific sites from appearing in Google search results](https://github.com/iorate/uBlacklist)      [[webext]] [[promnesia]]

good support for blacklist, reportedly good code quality  




# add some throttling for the notification at least





## `[2020-02-25]` added suppressing..




## `[2020-03-23]` maybe, it's better just to turn it off by default&#x2026;




# prefill with domain name?      [[promnesia]] [[search]]




# ublock content picker is awesome&#x2026; would be nice to find one..




# blacklisted: allow to force loading (from sidebar)




# sidebar doesn't work while search is open :( :(




# `[2020-05-02]` [Plain text linkifiers comparison (work in progress) (http://jsbench.github.io/#54315d74264c857856c73f18c81278dc)](https://gist.github.com/Isk1n/54315d74264c857856c73f18c81278dc)




# closing tab before it's finished loading causing error. I guess that's fine and shouldn't be defensified..




# not sure how to handle desktop notifications vs builtin? I'd prefer to use system as far as we can I guess but they are not easy to fine tune      [[webext]] [[togithub]]

perhaps I could sketch some simple library/api similarly to how android does that?  




# host permission on closing and reopening tab?




# right, switching to highlight.js/codejar does make it 110kb (vs 170 kb)




# #hypothesis adds special element <hypothesis-highlight>? wtf??




# `[2020-03-02]` windows 10 - Disable Chrome to ask for confirmation to open external application everytime - Super User      [[promnesia]] [[mimemacs]]

<https://superuser.com/questions/1481851/disable-chrome-to-ask-for-confirmation-to-open-external-application-everytime>  

    Disable Chrome to ask for confirmation to open external application everytime




# ignored entries should be colored as black      [[promnesia]] [[togithub]]




# could merge (e.g. chrome and takeout) both on client and server; not sure which would be best




# replace fixture with tmp<sub>path</sub> like in orger?




# `[2019-09-15]` bug: raw.githubusercontent.com/karlicoss/dotfiles/master/surfingkeys/config.txt

<https://raw.githubusercontent.com/karlicoss/dotfiles/master/surfingkeys/config.txt>  
shows error on this file very consistently..  




## `[2019-09-22]` ugh. works fine in dev firefox and doesn't even have sources on release?




## `[2019-09-23]` also seems to be fine in chrome, however doesn't display kkj




# process confidences and somehow add this information in visit line




# show with discarded url get params?      [[promnesia]] [[togithub]]





## `[2019-06-02]` eh??




## `[2019-12-27]` I guess I meant ignore normalisation etc




# pinboard last seen





## I guess needs a pinboard provider?




# fuck :D google takeout had json formats for activity&#x2026;      [[backup]] [[promnesia]] [[takeout]]




# use really really old takeout and see what happens




# ctrl-r doesn't seem to update extension icon for stale tab




# Motivation for browser history: its just easier to grab than google takeout data. I just need to merge them together i suppose      [[motivation]]




# option to disable dots on the page (permanently or temrporary)




# Maybe desktop integration?





## `[2019-12-26]` what?




## `[2021-01-20]` like a remembrance agent maybe?




# backend: URL extraction via NN?




# hmm it sort of around when I'm clicking links on the page.. would be interesting to see how that works





## `[2019-08-05]` eh?




# Watch "There is No Algorithm for Truth - with Tom Scott" on YouTube      [[promnesia]] [[motivation]]

<https://youtu.be/leX541Dr2rU>  

Why did I add this video? I don't know the speaker or anything  




## `[2019-11-21]` eh, not sure..




# people who followed you?





## `[2020-11-20]` not sure what I meant here?




# wonder if it would help me to figure out what was the video <https://www.youtube.com/watch?v=Z-R2xO3phVM>

title is missing; i suppose because I should have merged takeouts  




# fallback in sequence?

e.g.  
 jq  -> dumb json  
 bs4 -> grep  




# right, spend a bit debugging sidebar with 10K visits

I mean, even if I don't add the container to the hierarchy immediately, rendering (in particular, createElement) takes a bit  
I guess it's not very reasonable to expect 10K items to render really really fast  

1.  Limit number of items returned from the backend? think about it later
2.  Perhaps it's indeed better to delay it until opening the sidebar?




# tell about fake systemd?      [[toblog]]




# Would be fun to run the backend on Android..




# need to fix compare db to allow for small relative changes? at least for pinboard and reddit




# pydeps src/promnesia      [[python]] [[hpi]] [[promnesia]]




# Hmm wonder if could adapt promnesia for Next browser?

    I agree :-)
    The user should have the power. Also the interface should be as powerful as possible. One such browser that embraces this philosophy is Next https://github.com/atlas-engineer/next. Source: biased author




# `[2020-04-24]` usecase: [compute-space/compute-space.md at master · jauntywunderkind/compute-space](https://github.com/jauntywunderkind/compute-space/blob/master/compute-space.md)

found that bookmark in my notes without any comments. why did I add it?  
click on local &#x2013; found rektide's post!  




# `[2020-04-24]` usecase: [westoncb/mymex](https://github.com/westoncb/mymex)

useful for processing bookmarks  
e.g. I've got a list of websites/projects I bookmkrked.  
sometimes they are a bit experimental and cryptic, and I struggle to remember why I added it in the first place  
here &#x2013; click on last visit results in HN post  




# `[2020-05-06]` [Firefox for Mobile now supports NoScript, PrivacyBadger, HTTPS Everywhere | Hacker News](https://news.ycombinator.com/item?id=23085188)

    I fear they're going to force it as the release version while supporting just 1% of most used extensions, forgetting that it's a fat-tailed distribution. I use video background fix to play youtube with a minimized browser (no I don't want to use a separate app if I don't have to).
    
    At that point I'm just going to switch to Brave.




# `[2019-01-19]` Switching over to communicating via private server

ok, keeping the items in memory was definitely a bad idea..  
looks like the way to go is just running a server in parallel. the benefit is being able to run against the remote server, so not having to sync the links  

-   the database thing &#x2013; better, but still kinda clunky to update etc
-   also, we could optimize easier if it's not js, presumably some users might want to store a <span class="underline">lot</span> of links. Also more opportunity for interaction with FS and realtime watch
-   also normalisation code doesn't have to be shared with JS




# `[2020-06-30]` [Native messaging is extremely broken and has bad documentation. I never got repl&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23173724)      [[webext]]

    Native messaging is extremely broken and has bad documentation. I never got replies to my bug reports about it and gave up and just used websockets.




# browser history: clicked 'forget about this site' for google.com by accident.. wonder if it's gonna erase stuff




# `[2020-07-06]` [Linux kernel coders propose inclusive terminology coding guidelines, note: 'Arguments about why people should not be offended do not scale' • The Register](https://www.theregister.com/2020/07/06/linux_kernel_coders_propose_inclusive/)

    Words to be avoided include "slave", with suggested substitutions such as secondary, subordinate, replica or follower, and "blacklist", for which the replacements could be blocklist or denylist.




# `[2020-11-06]` [jeanralphaviles/comment<sub>parser</sub>: Python module to extract comments from source code files of various types.](https://github.com/jeanralphaviles/comment_parser)

hmm, try on this first? also wonder why its libmagic version is fixed??  




# `[2020-11-08]` [target browsers insteadd of Node, remove old react stuff, update eslint babel · karlicoss/promnesia@c8380e0](https://github.com/karlicoss/promnesia/runs/1368981214?check_suite_focus=true)

    test_blacklist_builtin

failed on github ci selenium.common.exceptions.NoAlertPresentException: Message:  
test<sub>blacklist</sub><sub>builtin</sub>  




# `[2020-11-16]` [uBlock/webext.js at 5aca41960373656c79d547b1a983f053e6adb633 · gorhill/uBlock](https://github.com/gorhill/uBlock/blob/5aca41960373656c79d547b1a983f053e6adb633/platform/chromium/webext.js)

async chrome apis examples  




# bug: right, seems that extension disconnects after a timeout in chrome based browsers

e.g. leave a tab open for several minutes and do smth else &#x2013; it stops responding  




# `[2019-09-01]` keepassxc-browser/manifest.json at develop · keepassxreboot/keepassxc-browser      [[webext]]

<https://github.com/keepassxreboot/keepassxc-browser/blob/develop/keepassxc-browser/manifest.json>  

    "applications": {
       "gecko": {
           "id": "keepassxc-browser@keepassxc.org",
           "strict_min_version": "52.0"
       }




## `[2019-09-08]` figure out why is this necessary?




# hmm, need to overwrite database in order to handle schema updates? not sure what would be a clean way of doing it&#x2026;





## `[2019-08-07]` I guess similar to cachew?




## `[2019-09-03]` ok, although haven't tested that behaviour




# I really need page notes&#x2026; e.g. reasons why I removed the bookmark and whether I already visited it..





## maybe, set up inotify to update the database?




# maybe show yellow icon if we only have chrome visits? so in a sense, green is more 'interesting' visits. also, maybe blink with green for a while (and have a timer whether we blinked in the past hour or something)





## `[2019-06-01]` need automatic generation for differently colored icons&#x2026;




## `[2019-06-02]` distinguish contexts as well




## `[2019-08-08]` just needs a better documenting..




# share code with js &#x2026;. ugh, all the projects I found really suck&#x2026;      [[ffi]] [[malleable]]

I guess just share the 'normalizing regex'?  




# highlight/color certain tags (configure that in settings)





## `[2019-06-01]` suggest tags? maybe by querying from api, although presumably there wouldn't be too many. make the config YAML




# make sure it searches in archive&#x2026;

-   State "DONE"       from "TODO"       `[2019-02-16]`




# Use cachew for browser history      [[promnesia]] [[cachew]]




# `[2020-05-27]` [sshkarupa/url-handlers](https://github.com/sshkarupa/url-handlers)      [[mimemacs]]




# `[2019-09-01]` vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources

<https://github.com/vinta/awesome-python>  

    Mistune - Fastest and full featured pure Python parsers of Markdown.




# at first, make filters private when I release it





## `[2019-10-12]` ok, they do save a bit of space for me, e.g. 575Mb vs 376 Mb. I guess keep my private ones for now and keep them empty in config, can resolve later





### `[2019-10-27]` fuck I'm so glad I'm keeping notes! Would have never remembered why db size changed otherwise..




# reddit link in context




# would be also useful to highlight visited posts, e.g. here <https://www.lesswrong.com/posts/vwqLfDfsHmiavFAGP/the-library-of-scott-alexandria>      [[promnesia]] [[demo]]

-   State "DONE"       from "TODO"       `[2019-02-16]`




# attempt to use prismjs

not sure what was wrong, but it didn't work with codejar. line numbers were broken on line breaks  
kinda suspicious, he gives prism in demo, but uses highlight js himself..  

    const PJ = await import(
        'prismjs/prism.js'
    );
    const Prism = PJ.default;
    await import(
        /* webpackChunkName: "codemirror.css" */
        // $FlowFixMe
        'prismjs/themes/prism.css'
    );
    TODO use highlightElement? like example 3 here https://medv.io/codejar




# wonder if I can embed in a page, as an Iframe?





## `[2019-12-26]` would be hard because of need to login, etc&#x2026;




# `[2020-02-18]` [Upload Add-on :: Promnesia :: Add-ons for Firefox](https://addons.mozilla.org/en-US/developers/addon/promnesia/versions/submit/)




# `[2020-10-28]` [thesephist/histools: A collection of tools for generating data visualizations from browser history data](https://github.com/thesephist/histools)




# release: suggest to update the backend

later, would be nice to propagate it to the extension ui&#x2026;  




# need to figure out how to keep error traceback/context..      [[python]] [[promnesia]] [[errors]]




# I failed miserably at reaching out to Worldbrain/Hypothesis to discuss whether we should collaborate :worldbrain:hypothesis

and instead engaged in a coding/refactoring streak. oh well  




# How to run as a proxy server? So it would work with any apps




# Tweet from @posobin      [[promnesia]] [[inspiration]]

<https://twitter.com/posobin/status/1330005221410529282>  

    @posobin: I really like it when an interface responds to holding some key down, and gets back when you let the key go, the immediacy of that is cool. Added such a feature to ampie: hold alt/option and the tooltips for all the ampersand badges to open up, let it go and they disappear. https://t.co/tw7bVltXXX




# `[2020-11-07]` ugh. looked in codemirror src, but unclear how to optimize the size further. it's just big **shrug**




# `[2020-05-06]` agnostic extraction &#x2013; extracting context is pretty much impossible      [[promnesia]] [[hpi]]




# `[2020-11-01]` profiling: so overall it seems that half time spent in parsing org-mode, half in url extraction. meh

    time py-spy record -o profile.svg -r 1000 -- scripts/promnesia demo data/notes/

results in source-org-profile.svg  




## `[2021-01-20]` this py-spy thing is very nice      [[performance]] [[python]]




# <https://www.freecodecamp.org/news/lossless-web-navigation-spatial-model-37f83438201d/> <https://merveilles.town/@aynish/105139837128207627>




# email mek




# mark visited &#x2013; maybe for ignored links add an attribute/explanation or something




# what if I add 'fake' history into browser database? wonder if that would work&#x2026;




# `[2020-11-26]` [Nyxt](https://nyxt.atlas.engineer/#features)

    Tree based history- lossless by design.




# `[2020-11-27]` showvisited: [Новые серии / MyShows.me](https://myshows.me/profile/)

visited marks shift the left menu  




# `[2020-12-14]` [Gephi - The Open Graph Viz Platform](https://gephi.org/)      [[timeline]]





## `[2020-12-14]` could draw en edge if the visits are close in time?




# `[2020-05-17]` [All Time - Hacker News Top Links](http://www.hntoplinks.com/all)




# `[2020-01-22]` Playing around with Chrome's history <https://gist.github.com/dropmeaword/9372cbeb29e8390521c2#chrome>      [[chrome]]




# `[2020-12-05]` interop: [DIYgod/RSSHub: 🍰 Everything is RSSible](https://github.com/DIYgod/RSSHub)      [[rss]] [[promnesia]] [[wildcard]]

hmm extractors for different sites could be reused  




# `[2020-12-06]` [Org-roam User Manual](https://www.orgroam.com/manual.html)

    • The roam-file protocol:
    • The roam-ref protocol:




# `[2020-12-06]` [Org-roam User Manual](https://www.orgroam.com/manual.html#Roam-Protocol-1)      [[grasp]] [[promnesia]]

fucking hell.. protocols and mime handling are a mess  




# `[2020-12-06]` [Newsletter 10 - Neovim v0.4.4 - Neovim](https://neovim.io/news/2020/10/)

moves the top navigation here  




# `[2020-12-13]` showvisited: [Mile End Climbing Wall](https://www.mileendwall.org.uk/)

moves around links here  




# somehow lower priority for org<sub>archive</sub> stuff      [[org]]




# `[2020-04-13]` [Show HN: Built an extension to put an end to paywalls and popups | Hacker News](https://news.ycombinator.com/item?id=22857232)

highlight paywalled links?  
although out of scope, probably  




# `[2021-01-19]` markdown bug [#promnesia](https://discord.com/channels/727903265437777944/800189382837534720)      [[promnesia]]

    ok, i figure it out, in md , only the [](url) could be recognized a true data, nor plain text link or paragraph link




# `[2020-05-20]` [shell script - Launching a terminal emulator without knowing which ones are installed - Unix & Linux Stack Exchange](https://unix.stackexchange.com/questions/137782/launching-a-terminal-emulator-without-knowing-which-ones-are-installed)      [[promnesia]] [[emacs]]

    else try xdg-terminal
    else try x-terminal-emulator




# `[2020-11-02]` [Repl.it - Node.js Online Compiler and IDE - Fast, Powerful, Free](https://repl.it/languages/nodejs)      [[js]] [[datetime]] [[promnesia]]

gh. tried dayjs.. but it doesn't seem to be able to handle timezones specified by offsets. ugh.  

    
    var dayjs = require('dayjs')
    require('dayjs/locale/en')
    var timezone = require('dayjs/plugin/timezone')
    dayjs.extend(timezone)
    var customParseFormat = require('dayjs/plugin/customParseFormat')
    dayjs.extend(customParseFormat)
    dayjs('21 Jun 2020 12:58:01 -0500', 'DD MMM YYYY HH:mm:ss ZZ', 'en').format()




# `[2021-01-18]` [promnesia/TROUBLESHOOTING.org at master · karlicoss/promnesia](https://github.com/karlicoss/promnesia/blob/master/doc/TROUBLESHOOTING.org#general-notes)

readme: add the 'check backend'?  




# `[2021-01-03]` [html - CSS set default scroll position - Stack Overflow](https://stackoverflow.com/questions/953083/css-set-default-scroll-position)      [[promnesia]]

    canonical: stackoverflow.com/users/21886/richiehindlesources : codestackoverflow::users/{ids}/favorites::[]::answers::[]::owner::linkstexport/data/stackexchange_20201204T020325Z.json04/12/2020, 02:03:25

ugh..  




# `[2021-01-17]` [#annotation-talks](https://discord.com/channels/727903265437777944/772319656471822337)

    Weird.. but thanks for letting me know. There is a promnesia doctor command that troubleshoots some common problems, I can suggest users to run it with python3 -m promnesia doctor, so it can detect the missing .local/bin and warn them!




# fetch all new posts and match them against promnesia?      [[promnesia]] [[hackernews]]

even simple rss + local email could work  




# I'd say the biggest problem with something like this is that it's a silo. You're&#x2026; | Hacker News      [[worldbrain]] [[interop]] [[promnesia]]

<https://news.ycombinator.com/item?id=21310988>  

-   `[2019-11-23]` xx

    I'd say the biggest problem with something like this is that it's a silo. You're suddenly 100% reliant on them providing the right tools and functions to access your data in the way you want/need. And if your needs/preferences change, then you're entirely reliant on whether the silo has foreseen the new use case.
    I already have an existing knowledge base (that not only consists of webpages, but also org files, videos, pdf's, etc.) that's accessible and synchronized across multiple devices - and while having a complete searchable history of all my browsing would be fantastic, there's no way to integrate it into my system (or any other system) with my own tools.




# `[2020-05-02]` [Vision, Mission & Values — 2020 Update - WorldBrain.io - Medium](https://medium.com/@WorldBrain/vision-mission-values-2020-update-d70aa35a638)      [[worldbrain]]





## `[2020-05-09]` hmm, this storex hub thing could be used to feed in promnesia data

I guess my big difference is the  

-   backend
-   normalization
-   context and 'child visits'

I've already had the UI. Next step would be seeing if we can cooperate. I'll try to reach some people in Memex and chat perhaps.  




# Potential social features (other people's annotations)




# demonstrate on some provider how it works as plaintext (e.g. grep), then as json and then as specific provider (and what do we get from that?)




# demonstrate indexing as json and as more specific instapaper?      [[promnesia]]




# in contexts if you add extra text it may potentially mess with highlighting. will be resolved with fuzzy I guess      [[promnesia]]




# It could be a tool similar to browser. Maybe you don't use it very often, but when you want it it's pretty good to have it, like browser history. Also it's a an actually working prototype unlike most of other snippet's I've  seen




# not sure how to decouple in the future?




# motivaiton: If you're digging for some topic you find yourself increasingly running at the same people




# Crucial ability is jumping right into context (tweet/tg message/etc). That complements search really well      [[infra]] [[promnesia]]




# Tweet from @jethroksy      [[promnesia]]

<https://twitter.com/jethroksy/status/1233408971437821952>  

    @jethroksy: I wrote a feature for Org-roam I really like! Have notes tied to arbitrary web pages, use a Firefox bookmarklet to instantaneously bring you to the correct notes file. Template flexible, can prefill with all kinds of things! https://t.co/KpMGazgS0I




## `[2020-04-27]` ok, I think it ties it via ID or something.. so not so agnostic..




# @dalmo3: Built this chrome extension to get your @hypothes<sub>is</sub> annotations into @RoamResearch <https://t.co/X3A1AxfFkg>      [[promnesia]]

<https://twitter.com/dalmo3/status/1229733827595001856>  




# `[2020-05-24]` [Vivaldi browser v1.8 released, with calendar-style browsing history | Hacker News](https://news.ycombinator.com/item?id=13984122)      [[promnesia]]

    This. Susan Dumais at Microsoft had a project called "Stuff I've Seen" [1] in the early days of desktop search. In a nutshell, it's indexing and information retrieval on the data that you use in your daily life -- web browsing, calendar events, etc.
    
    I've often thought about trying to re-implement some of their ideas with a local caching proxy or a browser extension. If there's an open source attempt at this already, I'd love to hear about it.




# People clearly like curating bookmarks. I could pitch it      [[toblog]]




# andy matuschak <https://twitter.com/andy_matuschak/status/1206055315000528898>




# `[2020-04-28]` tweet at mek?

    @mekarpeles hey, I've ran into your google doc https://docs.google.com/document/d/1QlrVpAl59gmJD7Kl--q3uyfZo936iZIb45fim6EV53k , I'm working on a browser extension that's addressing Problem 1 https://github.com/karlicoss/promnesia#readme




# I tried to make sure it's as resilient as possible      [[promnesia]] [[errors]]

in js, it's very easy to swallow errors. at best it just stops code halfway and renders system weird (exceptions would only be visible in extensions logs which no user would look at)  
worst case you end up with inconsistent state (TODO reformulate) or break some invariants  
I've wrapped everything in TODO defensify  
But that manifested in lots of spurious errors for various edge cases, so I had to deal with it. tests; fuzzing  




# highlight css styling among features      [[css]]




# attempt to implement uniform engine for annotation: not necessary for hypothesis to do so      [[promnesia]]




# design: few things became apparent: realtime updates are tedious to implement, however it's way easier to make stuff recompute everything from scratch. kcache was motivated by that      [[toblog]] [[promnesia]]




# design: There is no way to implement this without keeping the data locally (or to be more specific, in one place)




# `[2019-08-25]` demo: HN Classics <https://posobin.com/hn_classics/>

nice, 'show dots' works really well for that  




## `[2020-04-27]` eh, red dots don't look nice here?




# I was to make an emphasis: it's not a vaporware!

It's not even a prototype! It's a but raw, but it works for me, and there is no reason it won't work for you apart from some infrastructural overhead.  
I would like to raise a discussion on making this easier. I appreciate it may still be far from being possible to use by non-technical people, but at least my goal is so people who know/capable how to git clone and run from jobs could set this up  




# in the process I had to fix the python url extraction library&#x2026;      [[promnesia]] [[toblog]]





## `[2020-04-29]` could add this to yak shaving section




# Ideally I'd want some sort of AI assistant that would detect relevant bits and highlight them

for now we can at least do some sort of fuzzy highlighting?  




# benefit of using browser history (sqlite) databases: easier to sync them around (or if you can't be bothered to do google takeout every now and then)      [[promnesia]]

Two sided?  
The only downside is you won't have timestamps unless you write them out  




# bug: database might be lock while creating index? probably because of periodic indexer

    sqlalchemy.exc.OperationalError: (sqlite3.OperationalError) database is locked
    [SQL: CREATE INDEX index_norm_url ON visits (norm_url)]
    (Background on this error at: http://sqlalche.me/e/13/e3q8)




# exclude fonts      [[promnesia]]

    'While indexing exobrain/exobrain-logseq/static/fonts/IBMPlexMono-Text-Latin1.woff', 'No extractor for suffix .woff, mime font/woff




# was in some sort of infinite/super slow binding loop in the sidebar on discord, turned it off for now      [[promnesia]]




# further directions      [[promnesia]] [[toblog]]

I'd like to solve some general problems, so we can all benefit  

-   cannon
-   timeline storage etc
-   how to embed metadata into the page?  
    usually  
    empty space detection




# hmm, interferes?  e.g. try highlighting over a 'visited' mark      [[promnesia]] [[hypothesis]]




# need to log less in serve?      [[promnesia]]

maybe allow changing logging level via a signal??  




# querying for datetimes accounting for tz `SELECT norm_url, dt, src, (coalesce(datetime(substr(dt,1,instr(dt,' ')-1)), datetime(dt))) FROM visits WHERE rowid IN (SELECT rowid FROM visits ORDER BY RANDOM() LIMIT 1000)`      [[promnesia]] [[sqlite]]




# `[2021-02-07]` [Insidious Big Brother Database User Manual: 1. BBDB](http://bbdb.sourceforge.net/bbdb.html)      [[promnesia]]

someone from Matrix nyxt suggested it's similar?  




# `[2021-02-07]` [Latest Nyxt topics - Atlas](https://discourse.atlas.engineer/c/nyxt/5)      [[promnesia]]




# right, url extraction: <https://github.com/lipoja/URLExtract/issues/13#issuecomment-467635302> and also I guess cut off trailing dots?




# `[2021-03-28]` installable mobile addon [promnesia – Add-ons for Firefox (en-GB)](https://addons.mozilla.org/en-GB/firefox/collections/14595094/promnesia/)      [[promnesia]]




# `[2021-03-26]` [Convert to ES6 compatible library by AStoker · Pull Request 65 · apvarun/toastify-js](https://github.com/apvarun/toastify-js/pull/65)      [[promnesia]]

    Convert to ES6 compatible library




# `[2021-05-03]` [agora: promnesia-howto](https://anagora.org/promnesia-howto)      [[promnesia]]

