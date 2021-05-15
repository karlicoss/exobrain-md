The repository: [karlicoss/HPI](https://github.com/karlicoss/HPI) and [blog post](https://beepb00p.xyz/hpi.html).  

This is a sort of todo-list with raw ideas and things not (yet?) worthy of github issues.  


# Table of Contents

-   [\* similar projects & efforts](#smlrprjctsffrts) 
    -   [`[2020-01-17]` Chatistics |  Python scripts to parse your Messenger, Hangouts, WhatsApp and Telegram chat logs into DataFrames](#smstrscrtgthbchtstcschtsttsppndtlgrmchtlgsntdtfrms) 
    -   [`[2020-03-21]` KrauseFx/FxLifeSheet: Tracking the key metrics of my life](#sgthbcmkrsfxfxlfshtkrsfxflfshttrckngthkymtrcsfmylf) [[qs]]
    -   [`[2019-12-11]` Solid (web decentralization project) - Wikipedia](#snwkpdrgwksldwbdcntrlztnpctsldwbdcntrlztnprjctwkpd) [[solid]]
    -   [`[2019-12-18]` ErikBjare/chatalysis: Analyse (group)chat messages](#sgthbcmrkbjrchtlyssrkbjrchtlyssnlysgrpchtmssgs) 
    -   [`[2020-05-08]` How this site works | Jack Reid](#sjckrdxyzpsthwthsstwrkshwthsstwrksjckrd) [[hpi]]
    -   [`[2020-05-18]` Quarantine Notes - Week 10 | Ben Congdon](#sbnjmncngdnmblgqrntnntswkqrntnntswkbncngdn) 
    -   [`[2021-02-28]` Archivers](#sgthbcmqnzlrchvstrchvrs) [[hpi]]
    -   [`[2021-03-19]` LifeScope](#slfscplfscp) [[qs]] [[dashboard]] [[hpi]]
    -   [need to outreach solid etc](#ndttrchsldtc) [[social]] [[hpi]]
-   [\* 3rd party integrations](#rdprtyntgrtns) 
    -   [`[2020-05-14]` could caption "HPI meets X"](#cldcptnhpmtsx) [[toblog]]
    -   [`[2021-02-04]` Apache Arrow 3.0 | Hacker News](#snwsycmbntrcmtmdpchrrwhckrnws) [[hpi]]
    -   [`[2020-03-18]` ricklamers/gridstudio: Grid studio is a web-based application for data science with full integration of open source data science frameworks and languages](#sgthbcmrcklmrsgrdstdrcklmpnsrcdtscncfrmwrksndlnggs) [[pandas]]
    -   [`[2020-05-09]` Live demo · andrey-utkin/taskdb Wiki](#sgthbcmndrytkntskdbwklvdmtdshbrdlvdmndrytkntskdbwk) 
    -   [`[2020-09-11]` Kate on Twitter: "I made a super simple CLI plotting thingy, reads numbers on stdin, draws svg to stdout. Just for seeing the shape of data. It's written in awk. https://t.co/TFYKbn2SKT" / Twitter](#stwttrcmthngsktddsttsktntwrttnnwkstctfykbnskttwttr) [[tui]]
    -   [`[2021-02-08]` Bram Wiepjes / baserow · GitLab](#sgtlbcmbrmwbsrwbrmwpjsbsrwgtlb) [[hpi]] [[exobrain]]
    -   [Hpi to anki interface?](#hptnkntrfc) [[hpi]] [[srs]]
    -   [def try redash, seems to be a 'free' interface??](#dftryrdshsmstbfrntrfc) [[influxdb]]
    -   [`[2020-10-31]` Welcome to pyspread | pyspread](#spysprdgtlbwlcmtpysprdpysprd) [[hpi]] [[python]] [[spreadsheets]]
    -   [`[2020-01-10]` Repl.it - Feed  https://repl.it/talk/all?lang=python\_turtle](#rpltfdsrplttlklllngpythntrtl) [[project]] [[promnesia]] [[demo]]
    -   [`[2020-10-16]` Need your insights on a “Self Data Hub” ideation - Quantified Self / Apps & Tools - Quantified Self Forum](#sfrmqntfdslfcmtndyrnsghtsqntfdslfppstlsqntfdslffrm) 
    -   [`[2020-02-03]` Foreign data wrappers - PostgreSQL wiki](#swkpstgrsqlrgwkfrgndtwrpprsfrgndtwrpprspstgrsqlwk) [[hpi]]
    -   [https://observablehq.com/@karlicoss/hpi<sub>meets</sub>\_](#xpsndcnncttbsrvblsbsrvblhqcmkrlcsshpmts) [[observable]]
    -   [trying out visidata](#tryngtvsdt) [[visidata]]
    -   [demo: def need demonstration with Memacs&#x2026;](#dmdfnddmnstrtnwthmmcs) [[memacs]]
    -   [`[2019-12-20]` Datasette — Datasette documentation tool for exploring data?](#dtsttdtsttdcmnttntlfrxplrngdt) 
    -   [demo: with QS ledger: should be easy it is to integrate](#dmwthqsldgrshldbsytstntgrt) [[qs]] [[toblog]]
    -   [`[2021-01-01]` List Of Virtual Tables](#swwwsqltrgvtblsthtmllstfvrtltbls) [[sqlite]]
    -   [use gephi as frontend?](#sgphsfrntnd) 
    -   [`[2020-12-14]` Simon Willison (@simonw): "sqlite-utils 3.1 adds a new command: sqlite-utils analyze-tables my.db It queries every column of every table and outputs useful statistics about them: https://sqlite-utils.readthedocs.io/en/stable/changelog.html#v3-1" | nitter](#snttrntsmnwsttssmnwllsnsmthdcsnstblchnglghtmlvnttr) [[hpi]]
    -   [`[2021-02-14]` influxdata/influxdb-python: Python client for InfluxDB](#sgthbcmnflxdtnflxdbpythnnxdbpythnpythnclntfrnflxdb) [[influx]] [[pandas]] [[hpi]]
    -   [`[2020-06-16]` A Jupyter Kernel for SQLite](#snwsycmbntrcmtmdjpytrkrnlfrsqlt) [[hpi]]
    -   [grafana is good for gaps in data?](#grfnsgdfrgpsndt) [[grafana]] [[hpi]]
    -   [`[2020-05-08]` heedy/heedy: An Open-Source Platform for Quantified Self & IoT](#sgthbcmhdyhdyhdyhdynpnsrcpltfrmfrqntfdslft) [[qs]]
    -   [Make simplified data projections, so plots can be generated in couple of pandas commands](#mksmplfddtprjctnsspltscnbgnrtdncplfpndscmmnds) [[toblog]] [[dashboard]]
    -   [`[2021-02-11]` Repl.it - Hosting Apps with Always On](#sblgrpltlwysnrplthstngppswthlwysn) [[hpi]] [[promnesia]] [[computing]]
    -   [`[2020-10-15]` wger-project/wger: Self hosted FLOSS fitness/workout and weight tracker written with Django](#sgthbcmwgrprjctwgrwgrprjcktndwghttrckrwrttnwthdjng) [[exercise]]
    -   [HPI should be able to generate blueprints for grafana; maybe even send to the API?](#hpshldbbltgnrtblprntsfrgrfnmybvnsndtthp) [[hpi]] [[grafana]]
    -   [maybe load all to postgres? would also work nice with #cachew &#x2026;.](#mybldlltpstgrswldlswrkncwthcchw) [[hpi]] [[grafana]]
    -   [ok, guess I need to figure out a nice interface to connect to grafana?](#kgssndtfgrtncntrfctcnncttgrfn) [[grafana]] [[hpi]]
    -   [upload stats; with coverage?](#pldsttswthcvrg) [[emfit]] [[grafana]]
    -   [`[2020-01-29]` Typesense: Open-Source Alternative to Algolia](#snwsycmbntrcmtmdtypsnspnsrcltrntvtlgl) [[hpi]] [[search]]
    -   [`[2021-03-05]` Simon Willison (@simonw) / Twitter](#stwttrcmsmnwsmnwllsnsmnwtwttr) [[hpi]]
-   [\* documentation & user friendliness improvements](#dcmnttnsrfrndlnssmprvmnts) 
    -   [Add data arbitration example for twitter](#dddtrbtrtnxmplfrtwttr) [[toblog]]
    -   [overlay/extension docs: document how to 'overlay' parts of it? with RSS or twitter as examples](#vrlyxtnsndcsdcmnthwtvrlyprtsftwthrssrtwttrsxmpls) 
    -   [specify export formats in docstrings and autogenerate?](#spcfyxprtfrmtsndcstrngsndtgnrt) 
    -   [doctor diaginfo command?](#dctrdgnfcmmnd) 
    -   [config: improve config helper to warn about the attributes?](#cnfgmprvcnfghlprtwrnbtthttrbts) 
    -   [doc: core primitive: `get_files`](#dccrprmtvgtfls) 
    -   [`[2021-02-26]` karlicoss (ex. jestem króliczkiem) on Twitter: "@nikitavoloboev I guess if I decide on some opinionated defaults it could just be a single container/VM (maybe you'd need to specify the path to data on disk and that's it). After that maybe people can decide whether they are happy with the defaults or are willing to tweak." / Twitter](#stwttrcmkrlcsssttskrlcssxththdfltsrrwllngttwktwttr) [[hpi]] [[dashboard]] [[promnesia]]
    -   [readme: keep list of packages other people forked? suggest to send me links](#rdmkplstfpckgsthrpplfrkdsggsttsndmlnks) 
    -   [`[2020-11-10]` User workflow documentation / understanding how components fit together · Issue 125 · karlicoss/promnesia](#sgthbcmkrlcssprmnsssssrwrpnntsfttgthrsskrlcssprmns) 
    -   [list supported providers in readme](#lstspprtdprvdrsnrdm) 
    -   [Add check methods to each provider, expose in doctor](#ddchckmthdstchprvdrxpsndctr) 
    -   [`[2020-05-18]` HPI/SETUP.org at master · karlicoss/HPI](#sgthbcmkrlcsshpblbmstrdcshmdlshpstprgtmstrkrlcsshp) 
    -   [`[2020-05-08]` intake.github.io/status https://intake.github.io/status](#ntkgthbsttssntkgthbstts) [[inspiration]]
    -   [doc: I guess google takeout would be a good demonstration](#dcgssggltktwldbgddmnstrtn) 
    -   [mention that using `make_config` isn't even necessary if you're not using default attributes](#mntnthtsngmkcnfgsntvnncssryfyrntsngdfltttrbts) 
    -   [doc: giude with pyenv if they don't want to mess up their main environment, use docker](#dcgdwthpynvfthydntwnttmsspthrmnnvrnmntsdckr) [[hpi]]
    -   [add a doctor shortcut for profiling?](#dddctrshrtctfrprflng) 
    -   [avoid `make_config` as far as possible, and just use properties directly instead?? it's only necessary for truly complicated hackery](#vdmkcnfgsfrspssblndjstspryncssryfrtrlycmplctdhckry) 
    -   [doc: when I add strict mode, suggest HPI<sub>STRICT</sub>=true in troubleshooting guide?](#dcwhnddstrctmdsggsthpstrcttrntrblshtnggd) [[hpi]]
    -   [update doc about using `hpi install [--user] my.modulename`](#pdtdcbtsnghpnstllsrmymdlnm) [[hpi]]
    -   [eh, doctor doesn't give meaningful res when running in /data/hpi??](#hdctrdsntgvmnngflrswhnrnnngndthp) 
    -   [`[2019-12-24]` inspiration: hugginn credentials inspiration:](#nsprtnhggnncrdntlsnsprtn) 
    -   [doc: Hmm i wonder if egg links can be used on systems without symlinks?](#dchmmwndrfgglnkscnbsdnsystmswthtsymlnks) [[pip]] [[python]]
-   [\* patterns for writing concise and safe modules](#pttrnsfrwrtngcncsndsfmdls) 
    -   [design: dateclasses &#x2013; mutable vs immutable](#dsgndtclsssmtblvsmmtbl) [[hpi]]
    -   [check for dataframe 'error' column](#chckfrdtfrmrrrclmn) [[errors]] [[pandas]]
    -   [functions with default inputs= argument](#fnctnswthdfltnptsrgmnt) 
    -   [keep date as the first attribute to make sorting easier](#kpdtsthfrstttrbttmksrtngsr) 
    -   [Could use properties for lazier paths](#cldsprprtsfrlzrpths) 
    -   [top level decorator to check that some data was emitted?](#tplvldcrtrtchckthtsmdtwsmttd) 
    -   [maybe have sensible fallbacks for configs? e.g. falling back to documents folder, builtin python packages/site dire/etc](#mybhvsnsblfllbcksfrcnfgsgsfldrbltnpythnpckgsstdrtc) 
    -   [use venv instead of repos symlinks](#svnvnstdfrpssymlnks) [[hpi]]
    -   [Could use protocols (with Literal types) for pandas dfs???](#cldsprtclswthltrltypsfrpndsdfs) [[pandas]] [[mypy]]
    -   [pattern: avoid importing config early so modules can work without it?](#pttrnvdmprtngcnfgrlysmdlscnwrkwthtt) [[hpi]]
    -   [hmm. could just use ripgreppy parsing for processing htmls??](#hmmcldjstsrpgrppyprsngfrprcssnghtmls) [[promnesia]]
    -   [`[2020-05-16]` Lazy — MacroPy3 1.1.0 documentation](#smcrpyrdthdcsnltstlzyhtmllzylzymcrpydcmnttn) [[python]]
    -   [avoid fromtimestamp?](#vdfrmtmstmp) [[python]]
    -   [`[2020-05-03]` reddit: zstd vs lz4 comparison](#rddtzstdvslzcmprsn) [[reddit]] [[exports]] [[hpi]]
    -   [`[2020-05-03]` comparison of zstd vs lz4](#cmprsnfzstdvslz) [[reddit]] [[hpi]]
    -   [wonder if can make Ipython force the iterators?](#wndrfcnmkpythnfrcthtrtrs) [[python]]
    -   [`[2021-03-15]` config: extending base config which has Paths/Pathish and List as the default attribute](#cnfgxtndngbscnfgwhchhspthspthshndlststhdfltttrbt) [[hpi]]
    -   [handles archived stuff via CPath helper](#hndlsrchvdstffvcpthhlpr) [[hpi]]
-   [\* data providers/sources](#dtprvdrssrcs) 
    -   [the fuck??? after about 16019960000803 the timestamps for individual measurements basically stopped updating??](#thfckftrbtthtmstmpsfrndvdlmsrmntsbscllystppdpdtng) [[hpi]] [[bluemaestro]]
    -   [rescuetime: figure out utc or not](#rsctmfgrttcrnt) 
    -   [podcast addict](#pdcstddct) 
    -   [gpslogger?](#sgthbcmkrlcsshppllsscmmntgpslggr) 
    -   [`[2019-09-17]` jlumpe/pyorg: Python library for working with Emacs org mode.](#sgthbcmjlmppyrgjlmppyrgpythnlbrryfrwrkngwthmcsrgmd) [[org]]
    -   [define reasonable ranges for exercises so I could detect errors..](#dfnrsnblrngsfrxrcsssclddtctrrrs) [[wledger]]
    -   [`[2020-10-05]` seanbreckenridge/ipgeocache: A small cache layer for IP geolocation info](#sgthbcmsnbrcknrdgpgcchsnbpgcchsmllcchlyrfrpglctnnf) 
    -   [commits &#x2013; need to cachew?](#cmmtsndtcchw) [[cachew]]
    -   [reddit: maybe get rid of 'unfavorited'?&#x2026;](#rddtmybgtrdfnfvrtd) [[reddit]]
    -   [`[2020-05-21]` `ping/instagram_private_api`: A Python library to access Instagram's private API.](#sgthbcmpngnstgrmprvtppngnthnlbrrytccssnstgrmsprvtp) 
    -   [some ijson warnings](#smjsnwrnngs) [[location]]
    -   [Hmm maybe filter reddit and only include every 10th or something to speed it up?](#hmmmybfltrrddtndnlyncldvrythrsmthngtspdtp) [[hpi_patterns]] [[reddit]]
    -   [check frequencies??](#chckfrqncs) [[bluemaestro]]
    -   [timezone provider issues](#tmznprvdrsss) [[location]]
    -   [twitter archive trims the retweets (TODO put in the documentation?)](#twttrrchvtrmsthrtwtstdptnthdcmnttn) [[twitter]]
    -   [`[2020-10-15]` wger/exercises.json at c70150b4850f2c7ab2fdc7a953c3c11f84d31e8c · wger-project/wger](#sgthbcmwgrprjctwgrblbcbfctcbfcbfdcccfdcwgrprjctwgr) [[exercise]]
    -   [stackexchange gdpr has ip addresses](#stckxchnggdprhspddrsss) 
    -   [location provider: foursquare/swarm](#lctnprvdrfrsqrswrm) 
    -   [twint doesn't get retweets](#twntdsntgtrtwts) [[twint]] [[twitter]]
    -   [need to switch all formats to json.. I guess it's still reasonable to have HTML parser because old takeouts didn't have it](#ndtswtchllfrmtstjsngsstssvhtmlprsrbcsldtktsddnthvt) [[takeout]]
    -   [`[2021-02-04]` seanbreckenridge/discord<sub>data</sub>: Library to parse messages/activity from the discord data export](#sgthbcmsnbrcknrdgdscrddtsssgsctvtyfrmthdscrddtxprt) [[discord]] [[hpi]]
    -   [when searching for commits, make sure archived repos are present](#whnsrchngfrcmmtsmksrrchvdrpsrprsnt) 
    -   [`[2021-02-27]` Upvoted submissions | Hacker News](#snwsycmbntrcmpvtddkrlcsspvtdsbmssnshckrnws) [[hackernews]] [[orger]] [[hpi]]
    -   [`[2020-10-14]` HPI/skype.py at 4a0eb2d8e3ae963e315f0eaa7f538b46ef5513f5 · seanbreckenridge/HPI](#sgthbcmsnbrcknrdghpblbbdfkyppytbdffbffsnbrcknrdghp) 
    -   [attempt to reverse geocache photos](#ttmpttrvrsgcchphts) 
    -   [old last.fm + spotify + bandcamp arbitration](#ldlstfmsptfybndcmprbtrtn) 
    -   [switch pinboard to HPI](#swtchpnbrdthp) [[promnesia]]
    -   [hmm, keeping history of when I followed people on twitter could be useful..](#hmmkpnghstryfwhnfllwdpplntwttrcldbsfl) [[promnesia]] [[hpi]]
    -   [how to make sure all providers are handled?](#hwtmksrllprvdrsrhndld) [[taplog]] [[hpi]]
    -   [allow timestamp for likes? just make it optional and use in orger if possible](#llwtmstmpfrlksjstmktptnlndsnrgrfpssbl) [[twitter]] [[hpi]]
    -   [pdfs: would be interesting to filter by author? dunno it's often not set/empty&#x2026;](#pdfswldbntrstngtfltrbythrdnntsftnntstmpty) [[hpi]]
    -   [pdfs: maybe extract some meta to build index?](#pdfsmybxtrctsmmttbldndx) [[hpi]]
    -   [`[2021-04-05]` piyueh/zoteroutils: Python API to interact with Zotero's local SQLite database.](#sgthbcmpyhztrtlspyhztrtlsptntrctwthztrslclsqltdtbs) [[zotero]] [[HPI]]
    -   [inactive windows are sort of useful too hmm](#nctvwndwsrsrtfsflthmm) [[hpi]] [[arbtt]]
    -   [cache pdfs by file?](#cchpdfsbyfl) [[hpi]] [[cachew]]
-   [\* improving testing & CI](#mprvngtstngc) 
    -   [also see J. Doe., a project aiming to create an artificial person/data narrative](#lssflmscrgjdjdprjctmngtcrtnrtfclprsndtnrrtv) 
    -   [could test against twitter database](#cldtstgnsttwttrdtbs) 
    -   [perhaps, 'fake data' generators belong to DAL/HPI as well? that way easy to keep in sync](#prhpsfkdtgnrtrsblngtdlhpswllthtwysytkpnsync) [[jdoe]]
    -   [sigh.. mimesis can't generate dates between two other, but works with json 'schemas'](#sghmmsscntgnrtdtsbtwntwthrbtwrkswthjsnschms) [[jdoe]]
    -   [use similar sample data download to bokeh? could be good for testing etc.](#ssmlrsmpldtdwnldtbkhcldbgdfrtstngtc) [[dashboard]] [[project]]
-   [\* publicity & reaching out to other people](#pblctyrchngttthrppl) 
    -   [describe what I've done by the commit history? and comments etc](#dscrbwhtvdnbythcmmthstryndcmmntstc) [[toblog]]
    -   [one of the goals is demonstraing the **architecture**](#nfthglssdmnstrngthrchtctr) [[toblog]]
    -   [planetpython etc?](#plntpythntc) [[publish]]
    -   [`[2021-02-15]` (6) InfluxData (@InfluxDB) / Twitter](#stwttrcmnflxdbnflxdtnflxdbtwttr) [[hpi]] [[publish]]
    -   [about endomondo shutting down and using runnerup for workouts, show the commits](#btndmndshttngdwnndsngrnnrpfrwrktsshwthcmmts) [[hpi]] [[tweet]] [[outbox]]
    -   [publish the thing about HPI configs?](#pblshththngbthpcnfgs) [[hpi]] [[toblog]]
    -   [tweet about hpi + photos integration](#twtbthpphtsntgrtn) [[hpi]] [[totweet]] [[outbox]]
-   [\* enhancements](#nhncmnts) 
    -   [get rid of individual cache paths? there is no point in them really&#x2026;](#gtrdfndvdlcchpthsthrsnpntnthmrlly) [[cachew]]
    -   [rename mcachew to cachew?? so it's less confusing](#rnmmcchwtcchwstslsscnfsng) [[cachew]]
    -   [for stats frequency (e.g. bluemaestro), also need to calculate 'reverse frequency'? e.g. how many 1 minute intervals are covered](#frsttsfrqncygblmstrlsndtcrqncyghwmnymntntrvlsrcvrd) 
    -   [async interface (possibly async wrapper for the whole modules?) os it emits iterator of dataframes, and when thedata updated, new df is emitted](#syncntrfcpssblysyncwrpprfrmsndwhnthdtpdtdnwdfsmttd) 
    -   [use it in github provider after I support exceptions](#stngthbprvdrftrspprtxcptns) [[cachew]]
    -   [think about overlaying user config on top of default dynamically? not sure&#x2026;](#thnkbtvrlyngsrcnfgntpfdfltdynmcllyntsr) 
    -   [`[2020-04-11]` stephen-bunn/file-config: Attrs-like file config definitions inspired from https://github.com/hynek/environ\_config](#stphnbnnflcnfgttrslkflcnfprdfrmsgthbcmhynknvrncnfg) [[configs]]
    -   [treat deleted pinboard items as deleted/archived; expliclitly](#trtdltdpnbrdtmssdltdrchvdxplcltly) [[hpi]] [[pinboard]]
    -   [need to add hooks to config that get executed when HPI is imported? so people could hack without changing apps' code](#ndtddhkstcnfgthtgtxctdwhnspplcldhckwthtchngngppscd) 
    -   [in v2.0, get rid of old my.config artifacts](#nvgtrdfldmycnfgrtfcts) 
    -   [`[2019-12-12]` Re: [Scarygami/location-history-json-converter] Streaming parsing (#16)](#rscrygmlctnhstryjsncnvrtrstrmngprsng) [[location]]
    -   [ok, pipenv seems like a pleasant way of experimenting, maybe give it a shot](#kppnvsmslkplsntwyfxprmntngmybgvtsht) 
    -   [maybe have a special tag, e.g. nohpi to shadow entries from hpi? although sometimes nice to retrieve all entries (but basically only one usecase for that, timeline)](#mybhvspcltggnhptshdwntrsfsbtbscllynlynscsfrthttmln) [[org]] [[hpi]]
    -   [`[2019-12-30]` esnme/ultrajson: Ultra fast JSON decoder and encoder written in C with Python bindings](#sgthbcmsnmltrjsnsnmltrjsnncdrwrttnncwthpythnbndngs) 
    -   [`[2020-05-15]` Type alias as a class member is not valid as a type · Issue #7866 · python/mypy](#sgthbcmpythnmypyssstyplssmmbrsntvldstypsspythnmypy) [[mypy]] [[hpi]]
    -   [`[2020-05-12]` HPI/CONFIGURING.org at master · karlicoss/HPI  defensive Protocol stub?](#sgthbcmkrlcsshpblbmstrdccmstrkrlcsshpdfnsvprtclstb) 
    -   [`[2019-12-24]` inspiration: credentials dashboard? Huginn](#nsprtncrdntlsdshbrdhgnn) [[hpi]]
    -   ['hpi shell' command launches python shell](#hpshllcmmndlnchspythnshll) 
    -   [configuration](#cnfgrtn) [[hpi]]
    -   [entity guessing: in materialistic module, make sure hpi stat my.materialistic returns last entity time](#nttygssngnmtrlstcmdlmksrhttmymtrlstcrtrnslstnttytm) [[hpi]]
    -   [automatic ids](#tmtcds) 
    -   [`[2021-04-04]` Shell Completion — Click Documentation (7.x)](#sclckplltsprjctscmnxbshcmpltshllcmpltnclckdcmnttnx) [[hpi]]
-   [\* bugs/issues](#bgssss) 
    -   [github issues](#gthbsss) 
    -   [windows compatibility..](#wndwscmptblty) [[hpi]]
    -   [hmm, iterator in `iter_tzs` never exhausts? cause it doesn't go over the last year. so it won't cache things??](#hmmtrtrntrtzsnvrxhstscstdntgvrthlstyrstwntcchthngs) 
    -   [MY<sub>CONFIG</sub> should resolve path to absolute?](#mycnfgshldrslvpthtbslt) 
    -   [tzabbr hack attempt](#tzbbrhckttmpt) 
    -   [doctor: for compileall check need to use tmp path?](#dctrfrcmplllchckndtstmppth) [[hpi]]
    -   [hmm stats look a bit off?](#hmmsttslkbtff) [[hpi]]
    -   [this is when forget parens after @cachew](#thsswhnfrgtprnsftrcchw) [[hpi]]
-   [\* misc](#msc) 
    -   [integrate with private overlay](#ntgrtwthprvtvrly) 
    -   [Automatic sqlite interface.. People seem to like it?](#tmtcsqltntrfcpplsmtlkt) [[cachew]]
    -   [`[2020-12-07]` CLI Guidelines – A guide to help you write better command-line programs | Hacker News](#snwsycmbntrcmtmdclgdlnsgdtbttrcmmndlnprgrmshckrnws) 
    -   [`[2020-11-14]` Personal Data Warehouses: Reclaiming Your Data | Hacker News](#snwsycmbntrcmtmdprsnldtwrhssrclmngyrdthckrnws) 
    -   [github traffic dashboard for each repo?](#gthbtrffcdshbrdfrchrp) [[hpi]] [[toblog]]
    -   [`[2020-12-07]` Leah Neukirchen (@LeahNeukirchen): "I put my IRC logs of the last decade into that, here is a dot for all 489398 lines I wrote:" | nitter](#snttrntlhnkrchnsttslhnkrcdntththrsdtfrlllnswrtnttr) [[viz]]
    -   [could write a tool to process historic stats for github referrers etc?](#cldwrttltprcsshstrcsttsfrgthbrfrrrstc) [[toblog]] [[coding]]
    -   [`[2021-02-23]` Yet another Тарантога](#stndlrgytnthrtrntgytnthrтарантога) [[hpi]]
    -   [`[2020-10-05]` mention data gathering libraries · seanbreckenridge/HPI@fbe4ffc](#sgthbcmsnbrcknrdghpcmmtfbrnglbrrssnbrcknrdghpfbffc) 
    -   [`[2020-10-19]` Blog/ddde0c1c-8f73-47ff-803a-342f85a5fa72.md at 45f5922e999cc1ad8dba74f695d3762bed3624f6 · dentropy/Blog](#sgthbcmdntrpyblgblbfccddbffmdtfccddbfdbdfdntrpyblg) 
    -   [`[2020-09-19]` iterable -> iterator · seanbreckenridge/HPI@90a16bb](#sgthbcmsnbrcknrdghpcmmtbbcdbtrbltrtrsnbrcknrdghpbb) 
    -   [Slots vs dataclasses](#sltsvsdtclsss) [[python]] [[mypy]]
    -   [`[2020-01-01]` John Stultz on Twitter: "random idea: Want something that I can point it at various services (imap/rss/other web services like gphotos,twitter) or takeout archives and it will import/dedup/index/archive locally on my system." / Twitter https://twitter.com/johnstultz\_work/status/1156691692772196352](#jhnstltzntwttrrndmdwntsmttrstwttrcmjhnstltzwrkstts) [[hpi]] [[webarchive]]
    -   [`[2020-05-16]` User awal | Lobsters](#slbstrswlsrwllbstrs) 
    -   [`[2020-05-02]` hyfen.net/memex/updates/putting-the-memex-into-a-container-shazam-other-memex-sightings](#shyfnntmmxpdtspttngthmmxnxntcntnrshzmthrmmxsghtngs) 
    -   [`[2021-03-09]` tried using monkeypatch to infer output types..](#trdsngmnkyptchtnfrtpttyps) [[types]] [[hpi]]
    -   ["data repository" is a good description?](#dtrpstrysgddscrptn) [[hpi]]
    -   [shit Url alias doesn't work&#x2026;](#shtrllsdsntwrk) [[hpi]]
    -   [`[2021-03-07]` Hypothesis](#shypthsswycvhydstpdklwhypthss) [[hpi]]
    -   [`[2021-03-08]` Instagram/MonkeyType: A system for Python that generates static type annotations by collecting runtime types](#sgthbcmnstgrmmnkytypnstgrypnnttnsbycllctngrntmtyps) [[hpi]] [[cachew]]
    -   [`[2021-04-12]` Extract, transform, load - Wikipedia](#snwkpdrgwkxtrcttrnsfrmldxtrcttrnsfrmldwkpd) [[hpi]]
    -   [`[2021-03-13]` qs<sub>ledger</sub>/instapaper<sub>downloader.ipynb</sub> at master · markwk/qs<sub>ledger</sub>](#sgthbcmmrkwkqsldgrblbmstrwnldrpynbtmstrmrkwkqsldgr) [[hpi]]
-   [--------------------------------------------](#64412_64502) 
-   [classify modules by ease of setup?](#clssfymdlsbysfstp) [[hpi]]
-   [I'm not inventing anything new &#x2013; trying to apply simplicity, decomposition and resilience principles](#mntnvntngnythngnwtryngtpplctydcmpstnndrslncprncpls) [[hpi]]
-   [ids are useful to mark some stuff as public (e.g. annotations)](#dsrsfltmrksmstffspblcgnnttns) [[hpi]] [[memex]]
-   [could implement some helper that prompts visidata for column types](#cldmplmntsmhlprthtprmptsvsdtfrclmntyps) [[visidata]] [[hpi]]




# \* similar projects & efforts





## `[2020-01-17]` [Chatistics |  Python scripts to parse your Messenger, Hangouts, WhatsApp and Telegram chat logs into DataFrames](https://masterscrat.github.io/Chatistics)

pretty nice format; perhaps I should do that?  




## `[2020-03-21]` [KrauseFx/FxLifeSheet: Tracking the key metrics of my life](https://github.com/KrauseFx/FxLifeSheet)      [[qs]]

wow, that looks quite elaborate and cool!  




## `[2019-12-11]` [Solid (web decentralization project) - Wikipedia](https://en.wikipedia.org/wiki/Solid_(web_decentralization_project))      [[solid]]

    Solid (Social Linked Data)[1] is a web decentralization project led by Tim Berners-Lee, the inventor of the World Wide Web, developed collaboratively at the Massachusetts Institute of Technology (MIT). The project "aims to radically change the way Web applications work today, resulting in true data ownership as well as improved privacy"[2] by developing a platform for linked-data applications that are completely decentralized and fully under users' control rather than controlled by other entities. The ultimate goal of Solid is to allow users to have full control of their own data, including access control and storage location. To that end, Tim Berners-Lee formed a company called Inrupt to help build a commercial ecosystem to fuel Solid.




## `[2019-12-18]` [ErikBjare/chatalysis: Analyse (group)chat messages](https://github.com/ErikBjare/chatalysis)

    Currently supports: Facebook Messenger. Planned: Slack, WhatsApp, Telegram, Signal, Wire




## `[2020-05-08]` [How this site works | Jack Reid](https://jackreid.xyz/post/how-this-site-works/)      [[hpi]]




## `[2020-05-18]` [Quarantine Notes - Week 10 | Ben Congdon](https://benjamincongdon.me/blog/2020/05/17/Quarantine-Notes-Week-10/)

    This probably warrants its own post, but I strongly agree with the philosophy of Dogsheep: everything lives in a SQLite database (that you own!), each exporter tool is its own separate CLI, and Datasette is an extremely flexible tool to explore data. The Dogsheep ecosystem is totally self-hosted (you own your data) and free (as in beer), unlike personal data aggregator platforms like Exist.io and Gyroscope.




## `[2021-02-28]` [Archivers](https://github.com/qnzl-archivist)      [[hpi]]




## `[2021-03-19]` [LifeScope](https://lifescope.io/)      [[qs]] [[dashboard]] [[hpi]]

<https://github.com/LifeScopeLabs>  




## need to outreach solid etc      [[social]] [[hpi]]




# \* 3rd party integrations





## `[2020-05-14]` could caption "HPI meets X"      [[toblog]]




## `[2021-02-04]` [Apache Arrow 3.0 | Hacker News](https://news.ycombinator.com/item?id=26018187)      [[hpi]]

    Not only in between processes, but also in between languages in a single process. In this POC I spun up a Python interpreter in a Go process and pass the Arrow data buffer between processes in constant time. https://github.com/nickpoorman/go-py-arrow-bridge

hmm would be pretty cool if possible to use  




## `[2020-03-18]` [ricklamers/gridstudio: Grid studio is a web-based application for data science with full integration of open source data science frameworks and languages](https://github.com/ricklamers/gridstudio)      [[pandas]]

hmm, looks interesting, but it's all dockerized, so might be tricky to expose my data..  




## `[2020-05-09]` [Live demo · andrey-utkin/taskdb Wiki](https://github.com/andrey-utkin/taskdb/wiki/Live-demo#workout-dashboard)

    it is pretty neat already for analysis with querying and visualization. But your stuff is orders of magnitude bigger. Possibly I will set up HPI for myself some day.




## `[2020-09-11]` [Kate on Twitter: "I made a super simple CLI plotting thingy, reads numbers on stdin, draws svg to stdout. Just for seeing the shape of data. It's written in awk. https://t.co/TFYKbn2SKT" / Twitter](https://twitter.com/thingskatedid/status/1286559756967002113)      [[tui]]

    made a super simple CLI plotting thingy, reads numbers on stdin, draws svg to stdout




## `[2021-02-08]` [Bram Wiepjes / baserow · GitLab](https://gitlab.com/bramw/baserow)      [[hpi]] [[exobrain]]

    Open source online database tool and Airtable alternative.




## Hpi to anki interface?      [[hpi]] [[srs]]

That way would be able to easily import and remember lots of tgings. Just need stable IDs..  




## def try redash, seems to be a 'free' interface??      [[influxdb]]

<https://news.ycombinator.com/item?id=13597068>  

-   <https://news.ycombinator.com/item?id=23860281>  
    
        I evaluated on-premise Redash as an alternative for engineers and analysts who don't want to learn tableau. It's harder to setup than Metabase but more intuitive to use (for someone with SQL expertise).




## `[2020-10-31]` [Welcome to pyspread | pyspread](https://pyspread.gitlab.io/)      [[hpi]] [[python]] [[spreadsheets]]

    pyspread expects Python expressions in its grid cells, which makes a spreadsheet specific language obsolete. Each cell returns a Python object that can be accessed from other cells. These objects can represent anything including lists or matrices.




## `[2020-01-10]` Repl.it - Feed  <https://repl.it/talk/all?lang=python_turtle>      [[project]] [[promnesia]] [[demo]]

    Repl from Repo
    Instantly run any GitHub repository.




## `[2020-10-16]` [Need your insights on a “Self Data Hub” ideation - Quantified Self / Apps & Tools - Quantified Self Forum](https://forum.quantifiedself.com/t/need-your-insights-on-a-self-data-hub-ideation/8553/14)

    hook it right into open humans




## `[2020-02-03]` [Foreign data wrappers - PostgreSQL wiki](https://wiki.postgresql.org/wiki/Foreign_data_wrappers)      [[hpi]]

    Twitter




##        [[observable]]




## trying out visidata      [[visidata]]

ok looks promising  

tried <https://www.visidata.org/docs/graph/> on bluemaestro  

    from my.bluemaestro import dataframe
    df = dataframe()
    import visidata
    visidata.view_pandas(df.reset_index()[-1000:])

for all points, it was pretty slow&#x2026; not sure why  




## demo: def need demonstration with Memacs&#x2026;      [[memacs]]




## `[2019-12-20]` Datasette — Datasette documentation tool for exploring data?

    https://datasette.readthedocs.io/en/stable
    Datasette is a tool for exploring and publishing data. It helps people take data of any shape or size and publish that as an interactive, explorable website and accompanying API.
    Datasette is aimed at data journalists, museum curators, archivists, local governments and anyone else who has data that they wish to share with the world.




## demo: with QS ledger: should be easy it is to integrate      [[qs]] [[toblog]]

e.g. <https://github.com/markwk/qs_ledger/blob/master/instapaper/instapaper_data_analysis.ipynb>  
or lastfm ipynb?  




## `[2021-01-01]` [List Of Virtual Tables](https://www.sqlite.org/vtablist.html)      [[sqlite]]

    A virtual table is an object that presents an SQL table interface but which is not stored in the database file, at least not directly. The virtual table mechanism is a feature of SQLite that allows SQLite to access and manipulate resources other than bits in the database file using the powerful SQL query language.




## use gephi as frontend?




## `[2020-12-14]` [Simon Willison (@simonw): "sqlite-utils 3.1 adds a new command: sqlite-utils analyze-tables my.db It queries every column of every table and outputs useful statistics about them: https://sqlite-utils.readthedocs.io/en/stable/changelog.html#v3-1" | nitter](https://nitter.net/simonw/status/1338265856699035648)      [[hpi]]

    sqlite-utils 3.1 adds a new command:
        sqlite-utils analyze-tables my.db
    It queries every column of every table and outputs useful statistics about them




## `[2021-02-14]` [influxdata/influxdb-python: Python client for InfluxDB](https://github.com/influxdata/influxdb-python)      [[influx]] [[pandas]] [[hpi]]

    Additional dependencies are:
        pandas: for writing from and reading to DataFrames (http://pandas.pydata.org/

hmm this is useful.. wonder if could benefit from it  




## `[2020-06-16]` [A Jupyter Kernel for SQLite](https://news.ycombinator.com/item?id=23539541)      [[hpi]]

<https://blog.jupyter.org/a-jupyter-kernel-for-sqlite-9549c5dcf551>  




## grafana is good for gaps in data?      [[grafana]] [[hpi]]




## `[2020-05-08]` [heedy/heedy: An Open-Source Platform for Quantified Self & IoT](https://github.com/heedy/heedy)      [[qs]]




## Make simplified data projections, so plots can be generated in couple of pandas commands      [[toblog]] [[dashboard]]




## `[2021-02-11]` [Repl.it - Hosting Apps with Always On](https://blog.repl.it/alwayson)      [[hpi]] [[promnesia]] [[computing]]

    As a reminder, Replit gives you most of what you need to rapidly build and ship apps in the cloud -- at lightning speed:
        A blazing fast online IDE
        Automatic Package Management
        Automatic hosting
        Automatic SSL/HTTPS
        Domain linking
        A simple and fast Database for persistence
        A secure way to store secrets




## `[2020-10-15]` [wger-project/wger: Self hosted FLOSS fitness/workout and weight tracker written with Django](https://github.com/wger-project/wger)      [[exercise]]

integrate with it?  




## HPI should be able to generate blueprints for grafana; maybe even send to the API?      [[hpi]] [[grafana]]

e.g. depending on the 'aspects' the data provider has, would be different plots/dashboards  




## maybe load all to postgres? would also work nice with #cachew &#x2026;.      [[hpi]] [[grafana]]




## ok, guess I need to figure out a nice interface to connect to grafana?      [[grafana]] [[hpi]]




## upload stats; with coverage?      [[emfit]] [[grafana]]




## `[2020-01-29]` [Typesense: Open-Source Alternative to Algolia](https://news.ycombinator.com/item?id=22181437)      [[hpi]] [[search]]

<https://github.com/typesense/typesense>  




## `[2021-03-05]` [Simon Willison (@simonw) / Twitter](https://twitter.com/simonw)      [[hpi]]

finally need to cooperate with datasette&#x2026;  




# \* documentation & user friendliness improvements





## Add data arbitration example for twitter      [[toblog]]




## overlay/extension docs: document how to 'overlay' parts of it? with RSS or twitter as examples

e.g.  
maybe it's more of a platform to build your own layers etc  
akin to spacemacs/doom  




## specify export formats in docstrings and autogenerate?




## doctor diaginfo command?

dump if install is editable or not  
os/python version?  




## config: improve config helper to warn about the attributes?

        return previsits_to_history(*args, **kwargs, src='whatever')[0] # TODO meh
    src/promnesia/common.py:333: in previsits_to_history
        previsits = list(extr()) # TODO DEFENSIVE HERE!!!
    src/promnesia/sources/takeout.py:105: in index
        from my.google.takeout.paths import get_takeouts
        from dataclasses import dataclass
        from ...core.common import Paths
    
        from my.config import google as user_config
        @dataclass
    >   class google(user_config):
            '''
            Expects [[https://takeout.google.com][Google Takeout]] data.
    E       TypeError: no positional arguments expected




## doc: core primitive: `get_files`

can handle all sorts of things  




## `[2021-02-26]` [karlicoss (ex. jestem króliczkiem) on Twitter: "@nikitavoloboev I guess if I decide on some opinionated defaults it could just be a single container/VM (maybe you'd need to specify the path to data on disk and that's it). After that maybe people can decide whether they are happy with the defaults or are willing to tweak." / Twitter](https://twitter.com/karlicoss/status/1365431101917978624)      [[hpi]] [[dashboard]] [[promnesia]]




## readme: keep list of packages other people forked? suggest to send me links




## `[2020-11-10]` [User workflow documentation / understanding how components fit together · Issue 125 · karlicoss/promnesia](https://github.com/karlicoss/promnesia/issues/125)




## list supported providers in readme




## Add check methods to each provider, expose in doctor




## `[2020-05-18]` [HPI/SETUP.org at master · karlicoss/HPI](https://github.com/karlicoss/HPI/blob/master/doc/SETUP.org#setting-up-the-modules)

    ~/.config/my/my/config.py

eh. not sure about this section&#x2026;  
can't have config/repos dir and config.py at the same time  




## `[2020-05-08]` intake.github.io/status <https://intake.github.io/status>      [[inspiration]]




## doc: I guess google takeout would be a good demonstration




## mention that using `make_config` isn't even necessary if you're not using default attributes

also default attributes are pretty important because of caching, error handling policies, etc  




## doc: giude with pyenv if they don't want to mess up their main environment, use docker      [[hpi]]




## add a doctor shortcut for profiling?




## avoid `make_config` as far as possible, and just use properties directly instead?? it's only necessary for truly complicated hackery




## doc: when I add strict mode, suggest HPI<sub>STRICT</sub>=true in troubleshooting guide?      [[hpi]]




## update doc about using `hpi install [--user] my.modulename`      [[hpi]]




## eh, doctor doesn't give meaningful res when running in /data/hpi??

    my/core/init.py:40: UserWarning: 'my.config' package isn't found! (expected at /home/karlicos/.config/my). This is likely to result in issues.
    See https://github.com/karlicoss/HPI/blob/master/doc/SETUP.org#setting-up-the-modules for more info.
      """.strip())
    ✅ config file: my/config/__init__.py
    ❌ mypy check: failed
       Can't find package 'my.config'




## `[2019-12-24]` inspiration: hugginn credentials inspiration:

<http://localhost:3000/user_credentials>  

    Your Credentials
    Credentials are used to store values used by many Agents. Examples might include "twitter_consumer_secret", "user_full_name", or "user_birthday".

that's quite nice; would be cool to display credentials for my kron thing?  




## doc: Hmm i wonder if egg links can be used on systems without symlinks?      [[pip]] [[python]]




# \* patterns for writing concise and safe modules





## design: dateclasses &#x2013; mutable vs immutable      [[hpi]]

-   generally prefer mutable? errors would be rare, no one expects modifying data to do anything meaningful &#x2013; and if they do, they really want it?
-   better to make immutable via Final (so it's possible to check statically, but have an escape hatch if necessary)




## check for dataframe 'error' column      [[errors]] [[pandas]]




## functions with default inputs= argument

better not to use it:  

-   causes early inputs() calls
-   propagating all the way down wrappers (dataframes/aggregate functions etc) is unrealistic anyway
-   easy to override inputs() in tests, etc, sort of 'dependncy injection'

downsides:  

-   unclear how to cachew()???  
    although could just have lazy inputs() key. not that bad.




## keep date as the first attribute to make sorting easier




## Could use properties for lazier paths




## top level decorator to check that some data was emitted?

that could help for configuration mistakes  




## maybe have sensible fallbacks for configs? e.g. falling back to documents folder, builtin python packages/site dire/etc




## use venv instead of repos symlinks      [[hpi]]




## Could use protocols (with Literal types) for pandas dfs???      [[pandas]] [[mypy]]




## pattern: avoid importing config early so modules can work without it?      [[hpi]]

Add an example, maybe with dynamic my.config module  




## hmm. could just use ripgreppy parsing for processing htmls??      [[promnesia]]




## `[2020-05-16]` [Lazy — MacroPy3 1.1.0 documentation](https://macropy3.readthedocs.io/en/latest/lazy.html#lazy)      [[python]]

hmmm&#x2026; nice  
maybe could try it dith defensive behaviour&#x2026;  




## avoid fromtimestamp?      [[python]]




## `[2020-05-03]` reddit: zstd vs lz4 comparison      [[reddit]] [[exports]] [[hpi]]

about 3803 files  

      du -ch *.xz | tail -n 1
    2.1G	total
      du -ch *.zstd | tail -n1
    2.9G	total




## `[2020-05-03]` comparison of zstd vs lz4      [[reddit]] [[hpi]]

(every tenth file, cache disabled)  

    lz4 : ./test  31.20s user 2.58s system 101% cpu 33.285 total
    zstd: ./test  21.37s user 2.52s system 103% cpu 23.007 total

I mean, 1.5x is kinda nice&#x2026;  




## wonder if can make Ipython force the iterators?      [[python]]




## `[2021-03-15]` config: extending base config which has Paths/Pathish and List as the default attribute      [[hpi]]

e.g. in mycfg  

    class commits:
       roots: Sequence[PathIsh] = [L]

in my.commits  

    @dataclass
    class commits_cfg(user_config):
        roots: Sequence[PathIsh] # --- this complains    ValueError: mutable default <class 'list'> for field roots is not allowed: use default_factory. shit
        emails: Optional[Sequence[str]] = None
        names: Optional[Sequence[str]] = None

huh, so adding  `roots equals field(default_factory=list)` solved it?&#x2026;  




## handles archived stuff via CPath helper      [[hpi]]

requires a bit of cooperation by using isinstance check in DAL? &#x2026; maybe inputs should take str, dunno  




# \* data providers/sources





## the fuck??? after about 16019960000803 the timestamps for individual measurements basically stopped updating??      [[hpi]] [[bluemaestro]]

wtf?????  




## rescuetime: figure out utc or not




## podcast addict

has 'playbackDate' in episodes table  
seems that only podcastAddict.db is useful, the rest is just crap  




## [gpslogger?](https://github.com/karlicoss/HPI/pull/96#issuecomment-719826514) 




## `[2019-09-17]` [jlumpe/pyorg: Python library for working with Emacs org mode.](https://github.com/jlumpe/pyorg)      [[org]]

    >>> org.orgdir  # Obtained automatically from org-directory variable in Emacs
    OrgDir('/home/jlumpe/org/')

huh that's quite mad!  




## define reasonable ranges for exercises so I could detect errors..      [[wledger]]




## `[2020-10-05]` [seanbreckenridge/ipgeocache: A small cache layer for IP geolocation info](https://github.com/seanbreckenridge/ipgeocache)




## commits &#x2013; need to cachew?      [[cachew]]




## reddit: maybe get rid of 'unfavorited'?&#x2026;      [[reddit]]




## `[2020-05-21]` [`ping/instagram_private_api`: A Python library to access Instagram's private API.](https://github.com/ping/instagram_private_api)




## some ijson warnings      [[location]]

    tests/takeout.py::test_location_perf
      /home/karlicos/.local/lib/python3.7/site-packages/ijson/compat.py:47: DeprecationWarning:
      ijson works by reading bytes, but a string reader has been given instead. This
      probably, but not necessarily, means a file-like object has been opened in text
      mode ('t') rather than binary mode ('b').
        warnings.warn(_str_vs_bytes_warning, DeprecationWarning)




## Hmm maybe filter reddit and only include every 10th or something to speed it up?      [[hpi_patterns]] [[reddit]]




## check frequencies??      [[bluemaestro]]




## timezone provider issues      [[location]]

huh, that's random  

    datetime.datetime(2012, 5, 8, 17, 37, 28, 181000, tzinfo=<DstTzInfo 'Europe/Moscow' MSK+4:00:00 STD>),
      'Europe/Moscow'),
     (datetime.datetime(2012, 5, 8, 20, 46, 27, 16000, tzinfo=<DstTzInfo 'Asia/Novosibirsk' +07+7:00:00 STD>),
      'Asia/Novosibirsk'),
     (datetime.datetime(2012, 5, 8, 20, 50, 3, 274000, tzinfo=<DstTzInfo 'Asia/Novosibirsk' +07+7:00:00 STD>),
      'Asia/Novosibirsk'),




## twitter archive trims the retweets (TODO put in the documentation?)      [[twitter]]




## `[2020-10-15]` [wger/exercises.json at c70150b4850f2c7ab2fdc7a953c3c11f84d31e8c · wger-project/wger](https://github.com/wger-project/wger/blob/c70150b4850f2c7ab2fdc7a953c3c11f84d31e8c/wger/exercises/fixtures/exercises.json)      [[exercise]]

    "creation_date": null,
     "category": 12,
     "uuid": "7ce6b090-5099-4cd0-83ae-1a02725c868b",
     "muscles": [
         12
     ],
     "license": 1,
     "name": "Pull-ups"

ok, nice it already has muscles involved.. I could use this data  




## stackexchange gdpr has ip addresses




## location provider: foursquare/swarm




## twint doesn't get retweets      [[twint]] [[twitter]]

<https://github.com/twintproject/twint/issues/786>  

    twint -u karlicoss --retweets




## need to switch all formats to json.. I guess it's still reasonable to have HTML parser because old takeouts didn't have it      [[takeout]]




## `[2021-02-04]` [seanbreckenridge/discord<sub>data</sub>: Library to parse messages/activity from the discord data export](https://github.com/seanbreckenridge/discord_data)      [[discord]] [[hpi]]




## when searching for commits, make sure archived repos are present




## `[2021-02-27]` [Upvoted submissions | Hacker News](https://news.ycombinator.com/upvoted?id=karlicoss)      [[hackernews]] [[orger]] [[hpi]]




## `[2020-10-14]` [HPI/skype.py at 4a0eb2d8e3ae963e315f0eaa7f538b46ef5513f5 · seanbreckenridge/HPI](https://github.com/seanbreckenridge/HPI/blob/4a0eb2d8e3ae963e315f0eaa7f538b46ef5513f5/my/skype.py)




## attempt to reverse geocache photos

ugh. most libraries are outdated&#x2026;  
<https://github.com/thampiman/reverse-geocoder>  
some hackery&#x2026;  

    import geopy
    from geopy.geocoders import Nominatim
    from geopy.extra.rate_limiter import RateLimiter
    locator = Nominatim(user_agent="myGeocoder")
    # getloc = RateLimiter(locator.reverse, min_delay_seconds=0.001)
    #
    from functools import lru_cache
    
    @lru_cache(None)
    def query(p):
        print("UNCACHED!! ", p)
        return locator.reverse(p)
    
    def getloc(p):
        lat, lon = p
        lat = round(lat, ndigits=3)
        lon = round(lon, ndigits=3)
        return query((lat, lon))




## old last.fm + spotify + bandcamp arbitration




## switch pinboard to HPI      [[promnesia]]




## hmm, keeping history of when I followed people on twitter could be useful..      [[promnesia]] [[hpi]]




## how to make sure all providers are handled?      [[taplog]] [[hpi]]




## allow timestamp for likes? just make it optional and use in orger if possible      [[twitter]] [[hpi]]




## pdfs: would be interesting to filter by author? dunno it's often not set/empty&#x2026;      [[hpi]]




## pdfs: maybe extract some meta to build index?      [[hpi]]




## `[2021-04-05]` [piyueh/zoteroutils: Python API to interact with Zotero's local SQLite database.](https://github.com/piyueh/zoteroutils)      [[zotero]] [[HPI]]




## inactive windows are sort of useful too hmm      [[hpi]] [[arbtt]]




## cache pdfs by file?      [[hpi]] [[cachew]]




# \* improving testing & CI





## also see [J. Doe.](misc.md), a project aiming to create an artificial person/data narrative




## could test against twitter database

actually could even commit it to github&#x2026;  
use some really really public account?  




## perhaps, 'fake data' generators belong to DAL/HPI as well? that way easy to keep in sync      [[jdoe]]




## sigh.. mimesis can't generate dates between two other, but works with json 'schemas'      [[jdoe]]

faker can do that but doesn't support schemas out of the box..  

-   mimesis: can't do gauss




## use similar sample data download to bokeh? could be good for testing etc.      [[dashboard]] [[project]]




# \* publicity & reaching out to other people





## describe what I've done by the commit history? and comments etc      [[toblog]]




## one of the goals is demonstraing the **architecture**      [[toblog]]

I appreciate not everyone uses the same data as I do.  
My point is showing that my private layer is actually pretty thin and you can implement something TODO suiting you by looking at mine as an example.  

Same way as TODO think of some analogy? when you're using a todo list app, you've got your own unique pattern. Yet, we all benefit massively from sharing the same infrastructure  




## planetpython etc?      [[publish]]




## `[2021-02-15]` [(6) InfluxData (@InfluxDB) / Twitter](https://twitter.com/InfluxDB)      [[hpi]] [[publish]]

could tweet at them/grafana?  




## about endomondo shutting down and using runnerup for workouts, show the commits      [[hpi]] [[tweet]] [[outbox]]




## publish the thing about HPI configs?      [[hpi]] [[toblog]]




## tweet about hpi + photos integration      [[hpi]] [[totweet]] [[outbox]]

have a screenshot  

    datasette .cache/my.photos.main:_photos  --config max_returned_rows:20000

-   [ ] can bookmark the query, so it's basically stateless
-   [ ] stretch the map height
-   [ ] need to add JS with file links (and possibly thumbnails? not sure if it's gonna work well)




# \* enhancements





## get rid of individual cache paths? there is no point in them really&#x2026;      [[cachew]]




## rename mcachew to cachew?? so it's less confusing      [[cachew]]




## for stats frequency (e.g. bluemaestro), also need to calculate 'reverse frequency'? e.g. how many 1 minute intervals are covered




## async interface (possibly async wrapper for the whole modules?) os it emits iterator of dataframes, and when thedata updated, new df is emitted




## use it in github provider after I support exceptions      [[cachew]]




## think about overlaying user config on top of default dynamically? not sure&#x2026;




## `[2020-04-11]` stephen-bunn/file-config: Attrs-like file config definitions inspired from <https://github.com/hynek/environ_config>      [[configs]]

<https://github.com/stephen-bunn/file-config>  




## treat deleted pinboard items as deleted/archived; expliclitly      [[hpi]] [[pinboard]]

maybe need some nicer algorithm, to prevent flickering (maybe it doesn't happen anymore though)  




## need to add hooks to config that get executed when HPI is imported? so people could hack without changing apps' code




## in v2.0, get rid of old my.config artifacts




## `[2019-12-12]` Re: [Scarygami/location-history-json-converter] Streaming parsing (#16)      [[location]]

    o Scarygami/location-history-json-converter, me, Author
    Streaming parsing (--iterative) is now possible.
    The functionality requires ijson to be installed.




## ok, pipenv seems like a pleasant way of experimenting, maybe give it a shot

see <https://stackoverflow.com/questions/41573587/what-is-the-difference-between-venv-pyvenv-pyenv-virtualenv-virtualenvwrappe>  




## maybe have a special tag, e.g. nohpi to shadow entries from hpi? although sometimes nice to retrieve all entries (but basically only one usecase for that, timeline)      [[org]] [[hpi]]




## `[2019-12-30]` [esnme/ultrajson: Ultra fast JSON decoder and encoder written in C with Python bindings](https://github.com/esnme/ultrajson)

make it optional dependency with fallback?  




## `[2020-05-15]` [Type alias as a class member is not valid as a type · Issue #7866 · python/mypy](https://github.com/python/mypy/issues/7866)      [[mypy]] [[hpi]]

    Alias = NamedTuple("Alias", [("field", str)])

hmm, alias could be used as 'Like' type? for make<sub>config</sub>  




## `[2020-05-12]` [HPI/CONFIGURING.org at master · karlicoss/HPI](https://github.com/karlicoss/HPI/blob/master/doc/CONFIGURING.org)  defensive Protocol stub?

    so using it requires guarding the code with if typing.TYPE_CHECKING, which is a bit confusing and bloating.

could have a defensive import in my.core.typing  




## `[2019-12-24]` inspiration: credentials dashboard? Huginn      [[hpi]]

    Your Credentials
        Credentials are used to store values used by many Agents. Examples might include "twitter_consumer_secret", "user_full_name", or "user_birthday".




## 'hpi shell' command launches python shell




## configuration       [[hpi]]

    from my.config import core as user_config # type: ignore[attr-defined]

maybe instead of defining dynamic bits, import stuff from my.module.config? and then override? not sure  




## entity guessing: in materialistic module, make sure hpi stat my.materialistic returns last entity time      [[hpi]]




## automatic ids




## `[2021-04-04]` [Shell Completion — Click Documentation (7.x)](https://click.palletsprojects.com/en/7.x/bashcomplete/)      [[hpi]]




# \* bugs/issues





## github issues




## windows compatibility..      [[hpi]]

-   [ ] hpi doctor fails with some inf recursion??
-   [ ] my.location.takeout module is mentioned but unavailable??




## hmm, iterator in `iter_tzs` never exhausts? cause it doesn't go over the last year. so it won't cache things??

and then, location caching also never properly happens. uhoh  




## MY<sub>CONFIG</sub> should resolve path to absolute?




## tzabbr hack attempt

    for zone in pytz.all_timezones:
        tz = pytz.timezone(zone)
        infos = getattr(tz, '_tzinfos', [])
        for _, _, x in infos:
            tz_lookup[x] = tz




## doctor: for compileall check need to use tmp path?      [[hpi]]

    ✅ config file : /.config/my/my/config/__init__.py
    Compiling '/.config/my/my/config/__init__.py'...
    *** OSError: [Errno 30] Read-only file system: '/.config/my/my/config/__pycache__'




## hmm stats look a bit off?      [[hpi]]

    ✅ OK  : my.reading.goodreads
    ✅     - stats: {'books': {'books': {'count': 222, 'last': datetime.datetime(2013, 7, 14, 2, 58, 4, tzinfo=datetime.timezone(datetime.timedelta(days=-1, seconds=61200)))}}, 'events': {'events': {'count': 222, 'last': datetime.datetime(2013, 7, 14, 2, 58, 4, tzinfo=datetime.timezone(datetime.timedelta(days=-1, seconds=61200)))}}, 'inputs': {'inputs': {'count': 934}}, 'reviews': {'reviews': {'count': 222}}}




## this is when forget parens after @cachew      [[hpi]]

     ❯ python3 xx.py
    Traceback (most recent call last)
      File "xx.py", line 6, in <module>
        for x in M.bookmarks():
    TypeError: <lambda>() missing 1 required positional argument: 'realf'




# \* misc

Uncategorized stuff  




## integrate with private overlay

need to test behaviour w.r.t order of running local install?  




## Automatic sqlite interface.. People seem to like it?      [[cachew]]




## `[2020-12-07]` [CLI Guidelines – A guide to help you write better command-line programs | Hacker News](https://news.ycombinator.com/item?id=25304257)

    if you are displaying tabular data, present an ncurses interface

feed into visidata?  




## `[2020-11-14]` [Personal Data Warehouses: Reclaiming Your Data | Hacker News](https://news.ycombinator.com/item?id=25090218)

    I believe all data warehouses are limited by the quality of their data model. Most start with good relational intentions over a small domain, but eventually get bogged down arguing how semantic angels might dance on ontological pins. The parts that work become ossified and impossible to change. The system starts to fragment into multiple federated datastores or unstructured file dumps (“big data!”) where you have to build your own integration every time you want to use the data. Someone comes along and proposes a unifying model (“everything is an event!”) and rebuilds the whole thing but with an extra layer of complexity. Someone suggests buying an industry data model instead - surely the data experts will have solved all these problems for us? A skunkworks project spins up and starts implementing the bought model with good relational intentions over a small domain...
    I don’t think personal data warehouses are immune to any of these forces.




## github traffic dashboard for each repo?      [[hpi]] [[toblog]]




## `[2020-12-07]` [Leah Neukirchen (@LeahNeukirchen): "I put my IRC logs of the last decade into that, here is a dot for all 489398 lines I wrote:" | nitter](https://nitter.net/LeahNeukirchen/status/1335669406588923905)      [[viz]]

<https://twitter.com/LeahNeukirchen/status/1335669406588923905>  

    I put my IRC logs of the last decade into that, here is a dot for all 489398 lines I wrote:




## could write a tool to process historic stats for github referrers etc?      [[toblog]] [[coding]]




## `[2021-02-23]` [Yet another Тарантога](https://tiendil.org/yet-another-tarantoga/)      [[hpi]]




## `[2020-10-05]` [mention data gathering libraries · seanbreckenridge/HPI@fbe4ffc](https://github.com/seanbreckenridge/HPI/commit/fbe4ffca13f24ccaed6cc729b4ef0284a7221722)

    Disregarding tools which actively collect data (like [`ttt`](https://github.com/seanbreckenridge/ttt)/[`window_watcher`](https://github.com/seanbreckenridge/aw-watcher-window)), I have some other libraries I've created for this project, to provide more context to some of the data.
    - [`ipgeocache`](https://github.com/seanbreckenridge/ipgeocache) - for any IPs gathered from data exports, provides geolocation info, so I have location info going back to 2013 (thanks facebook)




## `[2020-10-19]` [Blog/ddde0c1c-8f73-47ff-803a-342f85a5fa72.md at 45f5922e999cc1ad8dba74f695d3762bed3624f6 · dentropy/Blog](https://github.com/dentropy/Blog/blob/45f5922e999cc1ad8dba74f695d3762bed3624f6/docs/notes/ddde0c1c-8f73-47ff-803a-342f85a5fa72.md)

    What features would I want in my HPI?




## `[2020-09-19]` [iterable -> iterator · seanbreckenridge/HPI@90a16bb](https://github.com/seanbreckenridge/HPI/commit/90a16bb686c8e3e57ccd48c37647b4f4c57a4cdb)

wonder why did he do that?  
Iterable needs to be iter(), e.g. you can't return list as Iterator  




## Slots vs dataclasses      [[python]] [[mypy]]

    Good writeup. A couple points.
    `zope.interface` is more explicit and scalable than `typing.Protocol`s, and more flexible than `abc.ABC`. There's a mypy plugin for it: https://github.com/Shoobx/mypy-zope
    > The drawback is that code that changes the representation of its data a lot tends not to be fast code.
    That's not a very convincing reason to avoid dataclasses except in the most performance-constrained environments -- and even then I'm doubtful it'd help. Especially with `slots=True`, dataclasses can take less resources.




## `[2020-01-01]` John Stultz on Twitter: "random idea: Want something that I can point it at various services (imap/rss/other web services like gphotos,twitter) or takeout archives and it will import/dedup/index/archive locally on my system." / Twitter <https://twitter.com/johnstultz_work/status/1156691692772196352>      [[hpi]] [[webarchive]]

    John Stultz
    @johnstultz_work
    random idea: Want something that I can point it at various services (imap/rss/other web services like gphotos,twitter) or takeout archives and it will import/dedup/index/archive locally on my system.




## `[2020-05-16]` [User awal | Lobsters](https://lobste.rs/u/awal)

    Anyway, thanks a lot for building all this stuff. Definitely gonna explore and it also helped me refine some of my thoughts on the subject!




## `[2020-05-02]` [hyfen.net/memex/updates/putting-the-memex-into-a-container-shazam-other-memex-sightings](https://hyfen.net/memex/updates/putting-the-memex-into-a-container-shazam-other-memex-sightings)

    My main objective right now is packaging what I’m working on into something that I can easily get to beta testers.




## `[2021-03-09]` tried using monkeypatch to infer output types..      [[types]] [[hpi]]

tried with my.pinboard module for bookmarks() function:  

-   can infer List[Bookmark]
-   can infer List[Union[Bookmark, RuntimeError]]
-   doesn't seems to be able to infer yield&#x2026; pretty annoying

so all in all seems that it would be easier to assume Res[X] and try to guess X?  




## "data repository" is a good description?      [[hpi]]




## shit Url alias doesn't work&#x2026;      [[hpi]]

    Url = NewType('Url', str)

what's up with this Bookmark thing??  

    [ins] In [24]: inspect.signature(Bookmark.url.fget)
    Out[24]: <Signature (self) -> <function NewType.<locals>.new_type at 0x7f9c8626ce50>>




## `[2021-03-07]` [Hypothesis](https://hypothes.is/a/-WYcvHYdEeustePidk7lwA)      [[hpi]]

update hypothesis link?  




## `[2021-03-08]` [Instagram/MonkeyType: A system for Python that generates static type annotations by collecting runtime types](https://github.com/instagram/MonkeyType)      [[hpi]] [[cachew]]

    MonkeyType collects runtime types of function arguments and return values, and can automatically generate stub files or even add draft type annotations directly to your Python code based on the types collected at runtime.

could use for some magic caching/inference of serialization? not sure  




## `[2021-04-12]` [Extract, transform, load - Wikipedia](https://en.wikipedia.org/wiki/Extract,_transform,_load)      [[hpi]]

I guess it's kind of 'auto'? Although ETL sounds a bit magical  




## `[2021-03-13]` [qs<sub>ledger</sub>/instapaper<sub>downloader.ipynb</sub> at master · markwk/qs<sub>ledger</sub>](https://github.com/markwk/qs_ledger/blob/master/instapaper/instapaper_downloader.ipynb)      [[hpi]]

see what's their approach to credentials  




# -------------------------------------------- 




# classify modules by ease of setup?      [[hpi]]




# I'm not inventing anything new &#x2013; trying to apply simplicity, decomposition and resilience principles      [[hpi]]




# ids are useful to mark some stuff as public (e.g. annotations)      [[hpi]] [[memex]]




# could implement some helper that prompts visidata for column types      [[visidata]] [[hpi]]

