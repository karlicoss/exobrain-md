
# Table of Contents

-   [tips etc](#tpstc) 
    -   [Apply the Javascript best practices](#pplythjvscrptbstprctcs) [[js]]
-   [addons.mozilla.org publishing](#ddnsmzllrgpblshng) [[amo]]
    -   [releasing new PUBLIC version on AMO](#rlsngnwpblcvrsnnm) 
-   [`[2019-08-18]` fregante/Awesome-WebExtensions: A curated list of awesome resources for WebExtensions development.](#sgthbcmfrgntwsmwbxtnsnsrdwsmrsrcsfrwbxtnsnsdvlpmnt) [[promnesia]] [[grasp]] [[webext]]
    -   [`[2019-09-02]` https://github.com/LinusU/wext-shipit this works also for firefox?](#sgthbcmlnswxtshptthswrkslsfrfrfx) [[webext]] [[firefox]]
-   [`[2019-08-18]` use sinon-chrome? Mocks the Chrome Extensions API for testing](#sgthbcmcvtkvsnnchrmssnnchmmcksthchrmxtnsnspfrtstng) [[grasp]] [[promnesia]] [[webext]]
-   [`[2019-08-28]` Working with quota on mobile browsers: A research report on browser storage - HTML5 Rocks](#wrkngwthqtnmblbrwsrsrsrchrprtnbrwsrstrghtmlrcks) [[html]] [[webext]]
    -   [`[2019-09-07]` To do this research, I have built a tool called Browser Storage Abuser to minimize the manual work. You can store as much data as possible to see the limit of each storage on your browser.](#tdthsrsrchhvblttlclldbrwssbltsthlmtfchstrgnyrbrwsr) 
    -   [`[2019-09-07]` Android firefox: For IndexedDB, you can use up to 50MB on desktop, 5MB on mobile for free. However, the user can allow the limit to be removed by granting permission.](#ndrdfrfxfrndxddbycnsptmbnthlmttbrmvdbygrntngprmssn) 
-   [`[2019-05-01]` telotortium/org-capture-extension at native-messaging-host](#tltrtmrgcptrxtnsntntvmssgnghst) 
    -   [`[2019-08-10]` hmm firefox also got it?](#sdvlprmzllrgnsdcsmzllddnsnsnsntvmssgnghmmfrfxlsgtt) 
    -   [`[2020-02-15]` ok, seems tricky, and apparently requires installing via OS](#ksmstrckyndpprntlyrqrsnstllngvs) 
-   [`[2019-09-08]` fregante/webext-options-sync: Helps you manage and autosave your extension's options. Chrome and Firefox.](#sgthbcmfrgntwbxtptnssyncftsvyrxtnsnsptnschrmndfrfx) [[promnesia]] [[grasp]]
-   [`[2019-08-29]` javascript - Chrome messaging: chrome.runtime.sendMessage not working on the newest release 49 - Stack Overflow](#sstckvrflwcmqstnschrmmssgtwrkngnthnwstrlsstckvrflw) [[webext]]
-   [browser<sub>action</sub> impacts presense of menu item on android..](#brwsrctnmpctsprsnsfmntmnndrd) [[webext]]
-   [`[2019-10-27]` Re: [fregante/webext-options-sync] feat: optionally use chrome.storage.local (#19) - karlicoss@gmail.com - Gmail](#rfrgntwbxtptnssyncftptnllchrmstrglclkrlcssgmlcmgml) 
-   [`[2019-09-08]` let the user decide what storage type shall be used by obama · Pull Request #8 · fregante/webext-options-sync](#sgthbcmfrgntwbxtptnssyncpmpllrqstfrgntwbxtptnssync) 
-   [`[2019-09-08]` notlmn/browser-extension-template: Barebones boilerplate with webpack, options handler and auto-publishing](#ntlmnbrwsrxtnsntmpltbrbnshwbpckptnshndlrndtpblshng) [[grasp]] [[webext]]
-   [`[2020-02-08]` Discontinuing support for beta versions | Mozilla Add-ons Blog](#sblgmzllrgddnsdscntnngsppspprtfrbtvrsnsmzllddnsblg) 
-   [`[2020-02-15]` How to add comments to package.json? - DEV Community 👩‍💻👨‍💻](#sdvtnplxhwtddcmmntstpckgjtddcmmntstpckgjsndvcmmnty) [[toblog]]
-   [`[2020-02-15]` xo - npm](#swwwnpmjscmpckgxxnpm) 
-   [`[2020-02-15]` browser-extension-template/options-storage.js at master · notlmn/browser-extension-template](#sgthbcmntlmnbrwsrxtnsntmptmstrntlmnbrwsrxtnsntmplt) 
-   [`[2020-02-15]` notlmn/browser-extension-template: Barebones boilerplate with webpack, options handler and auto-publishing](#sgthbcmntlmnbrwsrxtnsntmphwbpckptnshndlrndtpblshng) 
-   [`[2020-02-15]` DrewML/chrome-webstore-upload-cli: Upload/Publish Chrome Web Store extensions from the CLI](#sgthbcmdrwmlchrmwbstrpldclshchrmwbstrxtnsnsfrmthcl) [[webext]]
-   [`[2020-02-21]` Choosing a browser to write extensions for | Lobsters](#slbstrssbqzchsngbrwsrwrtxngbrwsrtwrtxtnsnsfrlbstrs) 
-   [`[2020-02-18]` mozilla/web-ext: A command line tool to help build, run, and test web extensions](#sgthbcmmzllwbxtmzllwbxtcmntlthlpbldrnndtstwbxtnsns) 
-   [`[2020-02-18]` Add \`web-ext submit\` to submit listed add-ons to AMO · Issue #804 · mozilla/web-ext](#sgthbcmmzllwbxtsssddwbxtstsbmtlstdddnstmssmzllwbxt) 
-   [`[2018-11-08]` Shraymonks/flow-interfaces-chrome: Flow interface declarations for the Chrome extensions API](#shrymnksflwntrfcschrmflwnrfcdclrtnsfrthchrmxtnsnsp) [[js]] [[flow]]
-   [`[2020-02-17]` Introducing Prism: An awesome new syntax highlighter | Lea Verou](#slvrmntrdcngprsmnwsmnwsynrsmnwsmnwsyntxhghlghtrlvr) 
-   [chrome got far better profiling, better debugging information + screenshots](#chrmgtfrbttrprflngbttrdbggngnfrmtnscrnshts) [[webext]]
-   [ugh, can't force webpack/chrome into using date in the version&#x2026;](#ghcntfrcwbpckchrmntsngdtnthvrsn) [[webext]]
-   [`[2020-04-05]` roam-toolkit/webpack.config.js at master · roam-unofficial/roam-toolkit](#sgthbcmrmnffclrmtlktblbmskcnfgjstmstrrmnffclrmtlkt) [[webext]]
-   [`[2018-03-29]` how webext works?](#hwwbxtwrks) 
-   [logging](#lggng) 
-   [`[2020-11-04]` softvar/awesome-web-storage: Everything you need to know about Client-side Storage.](#sgthbcmsftvrwsmwbstrgsftvrythngyndtknwbtclntsdstrg) [[webext]] [[js]]
-   [`[2020-05-14]` Let's guess what Google requires in 14 days or they kill our extension | Hacker News](#snwsycmbntrcmtmdltsgsswhtsndysrthykllrxtnsnhckrnws) [[webext]]
-   [for fucks sake. releasing even without 'unlisted' channel doesn't make it automatically submitted for manual review???](#frfcksskrlsngvnwthtnlstdctmkttmtcllysbmttdfrmnlrvw) 
    -   [`[2020-02-15]` ok, first time you need to create manually; after that, get the id (it's public, so ok to put in a git repo) and use it with the build script](#kfrsttmyndtcrtmnllyftrthttptngtrpndstwththbldscrpt) 
    -   [`[2020-05-17]` listed vs unlisted](#lstdvsnlstd) 
    -   [ugh why did I end up with several versions of grasp on AMO??](#ghwhyddndpwthsvrlvrsnsfgrspnm) 
-   [`[2020-05-24]` Manage Events with Background Scripts - Google Chrome](#sdvlprchrmcmxtnsnsbckgrndtswthbckgrndscrptsgglchrm) 
-   [`[2020-05-13]` Let's guess what Google requires in 14 days or they kill our extension | Hacker News](#snwsycmbntrcmtmdltsgsswhtsndysrthykllrxtnsnhckrnws) [[google]]
-   [`[2019-07-07]` client/security.rst at 734e3a25318364819a8c38ef881e4788a2b06365 · hypothesis/client](#clntscrtyrsttcfbhypthssclnt) [[webext]] [[security]]
    -   [`[2019-08-04]` For example: in order to draw highlights, the annotated page needs to know the location of annotations, but it does not ever need to know the body text of an an annotation, and so it should not be possible to expose this over the messaging interface.](#frxmplnrdrtdrwhghlghtsthnsbltxpsthsvrthmssgngntrfc) 
-   [`[2020-11-09]` Web Developer's Toolbox – Add-ons for Firefox (en-GB)](#sddnsmzllrgngbfrfxcllctnswbdvlprstlbxddnsfrfrfxngb) [[webext]]
-   [android debugging](#ndrddbggng) 
    -   [`[2019-08-10]` remote debugging; use `Shift-F8` to open web ide https://developer.mozilla.org/en-US/docs/Tools/Remote\_Debugging/Debugging\_Firefox\_for\_Android\_with\_WebIDE#Enable\_remote\_debugging\_in\_Firefox\_for\_Android](#rmtdbggngsshftftpnwbdsdvlbdnblrmtdbggngnfrfxfrndrd) 
-   [`[2019-02-16]` Creating a Chrome extension in 2018: The good, the bad and the meh | Checkly](#crtngchrmxtnsnnthgdthbdndthmhchckly) 
    -   [`[2019-08-10]` basic intro with examples of testing and explaining the extensions architecture](#bscntrwthxmplsftstngndxplnngthxtnsnsrchtctr) 
    -   [`[2019-06-01]` Creating a Chrome extension in 2018: The good, the bad and the meh](#crtngchrmxtnsnnthgdthbdndthmh) [[grasp]]
-   [`[2019-06-29]` Using Firefox WebExtensions with Selenium](#sngfrfxwbxtnsnswthslnm) 
-   [`[2019-06-29]` Standard8/example-webextension: Example repository containing templates and good practices for creating a WebExtension for Firefox](#stndrdxmplwbxtnsnxmplrpstrctcsfrcrtngwbxtnsnfrfrfx) 
-   [`[2019-07-08]` GUI and Headless Browser Testing - Travis CI](#gndhdlssbrwsrtstngtrvsc) [[ci]]
-   [`[2019-06-12]` Getting started with web-ext - Mozilla | MDN](#gttngstrtdwthwbxtmzllmdn) 
    -   [`[2019-08-10]` web-ext is a nice tool for signing, linting and even simple browser testing (e.g. web-ext run)](#wbxtsnctlfrsgnnglntngndvnsmplbrwsrtstnggwbxtrn) 
-   [`[2019-06-12]` Extensions in Firefox 66 | Mozilla Add-ons Blog](#xtnsnsnfrfxmzllddnsblg) 
-   [`[2019-06-12]` commands.update() - Mozilla | MDN](#cmmndspdtmzllmdn) 
    -   [`[2019-06-12]` 1475043 - Allow commands.update() to un-set a shortcut, disabling the command](#llwcmmndspdttnstshrtctdsblngthcmmnd) 
-   [`[2019-06-12]` Differences between desktop and Android extensions - Mozilla | MDN](#dffrncsbtwndsktpndndrdxtnsnsmzllmdn) 
-   [`[2019-06-12]` 1520119 - Support removing a shortcut in manage shortcuts](#spprtrmvngshrtctnmngshrtcts) 
-   [`[2019-06-12]` Debugging Firefox for Android over WiFi - Firefox Developer Tools | MDN](#dbggngfrfxfrndrdvrwffrfxdvlprtlsmdn) 
-   [`[2019-06-12]` Developing extensions for Firefox for Android - Mozilla | MDN](#dvlpngxtnsnsfrfrfxfrndrdmzllmdn) 
    -   [`[2019-08-10]` need to open browser on android prior to running web-ext command!](#ndtpnbrwsrnndrdprrtrnnngwbxtcmmnd) 
-   [`[2019-06-12]` Setting up an extension development environment - Archive of obsolete content | MDN](#sttngpnxtnsndvlpmntnvrnmntrchvfbsltcntntmdn) 
-   [`[2019-07-07]` javascript - How to make side panel in chrome extension? - Stack Overflow](#jvscrpthwtmksdpnlnchrmxtnsnstckvrflw) 
-   [`[2019-06-01]` Extensionizr - boilerplate for your chrome extension](#xtnsnzrblrpltfryrchrmxtnsn) 
-   [`[2019-06-01]` Creating a history clearing Chrome extension | Jake Lee](#crtnghstryclrngchrmxtnsnjkl) 
    -   [`[2019-08-10]` pretty simple guide](#prttysmplgd) 
-   [`[2019-06-13]` what is the state of add-on/extensions development for firefox? : firefox](#whtsthsttfddnxtnsnsdvlpmntfrfrfxfrfx) 
-   [`[2020-12-07]` Webext special commands](#wbxtspclcmmnds) [[webext]]
-   [`[2020-11-09]` Element | Malleable Systems Collective](#spplmntrmmllblsystmsmtrxrglmntmllblsystmscllctv) 
-   [`[2019-09-22]` javascript - Chrome extension - page update twice then removed on YouTube - Stack Overflow](#jvscrptchrmxtnsnpgpdttwcthnrmvdnytbstckvrflw) [[promnesia]]
-   [`[2020-05-05]` wildcard/chrome-autoreload.js at master · geoffreylitt/wildcard](#sgthbcmgffrylttwldcrdblbmtrldjstmstrgffrylttwldcrd) [[webext]]
-   [`[2019-12-09]` Request the right permissions | Extension Workshop](#rqstthrghtprmssnsxtnsnwrkshp) 
-   [`[2020-07-28]` Mozilla Add-ons Blog](#mzllddnsblg) 
-   [`[2020-05-05]` feat: Added option to \`&#x2013;watch-file\` to address eager reloading by jezhou · Pull Request #1784 · mozilla/web-ext](#sgthbcmmzllwbxtpllftdddptrldngbyjzhpllrqstmzllwbxt) 
-   [`[2020-05-24]` Understanding Google Chrome Extensions](#sgstgthbcmjjprzgngndrstndnggglchrmxtnsns) 
-   [`[2019-08-29]` Implement a settings page - Mozilla | MDN](#mplmntsttngspgmzllmdn) [[webext]]
-   [`[2019-04-21]` When to use margin vs padding in CSS - Stack Overflow](#whntsmrgnvspddngncssstckvrflw) [[css]]
    -   [`[2019-05-13]` {margins} collapse {paddings} dont](#mrgnscllpspddngsdnt) [[drill]] [[css]]
        -   [`[2019-10-27]` mnemonic is alphabetic order? dunno.](#mnmncslphbtcrdrdnn) 
    -   [`[2019-05-13]` this is also a good example for drill](#thsslsgdxmplfrdrll) [[spacedrep]] [[toblog]]
-   [js library for chrome settings, too annoying to bind them manually..](#jslbrryfrchrmsttngstnnyngtbndthmmnlly) [[promnesia]] [[grasp]]
    -   [`[2019-08-24]` found something the other day; must be in links](#fndsmthngththrdymstbnlnks) 
-   [`[2019-11-19]` [Question] How to set cors headers? · Issue #308 · http-party/http-server](#qstnhwtstcrshdrsssprtysrvr) [[cors]]
-   [`[2019-11-18]` python - Enable access control on simple HTTP server - Stack Overflow](#pythnnblccsscntrlnsmplsrvrstckvrflw) [[cors]]
-   [right, set up logins in about:profiles .after that it gets cloned](#rghtstplgnsnbtprflsftrthttgtsclnd) [[webext]]
-   [`[2019-06-13]` fuck. looks like firefox doesn't allow persistent dev extensions, that really sucks. and unbranded version doesn't have PPA? wtf? how are developers supposed to test their stuff](#fcklkslkfrfxdsntllwprsstnhwrdvlprssppsdttstthrstff) [[firefox]]
-   [`[2019-08-31]` uBlock/manifest.json at 6c34b3c3c96756b6db7ff2f3a0394472d81cde3e · gorhill/uBlock](#blckmnfstjsntcbccbdbfffdcdgrhllblck) 
-   [`[2019-09-01]` keepassxc-browser/manifest.json at develop · keepassxreboot/keepassxc-browser](#kpssxcbrwsrmnfstjsntdvlpkpssxrbtkpssxcbrwsr) [[webext]]
-   [`[2020-11-15]` Content scripts - Mozilla | MDN](#sdvlprmzllrgnsdcsmzllddnsdmssgngcntntscrptsmzllmdn) 
-   [`[2020-10-19]` 1309288 - Install addons permanently from about:debugging](#sbgzllmzllrgshwbgcgdnstllddnsprmnntlyfrmbtdbggng) 
-   [`[2020-11-10]` In Chrome Extension development, how do I pass a variable from background.js to a content script that embedded as a script node? - Stack Overflow](#sstckvrflwcmqstnsnchrmxtnthtmbdddsscrptndstckvrflw) 
-   [`[2020-11-10]` Chrome extension: message from background.js to content.js - Stack Overflow](#sstckvrflwcmqstnschrmxtnsckgrndjstcntntjsstckvrflw) 
-   [What I learned about writing web extensions](#whtlrndbtwrtngwbxtnsns) [[webext]] [[blog]]
    -   [there is an incredible lack of documentation for building web extensions and the best practices](#thrsnncrdbllckfdcmnttnfrbldngwbxtnsnsndthbstprctcs) [[webext]] [[blog]]
    -   [1. Use JS Flow 2. Use async. I mean, seriously.](#sjsflwssyncmnsrsly) [[js]] [[webext]]
        -   [`[2019-09-29]` could link that stackoverflow post and replace typescript advice with flow?](#cldlnkthtstckvrflwpstndrplctypscrptdvcwthflw) 
    -   [structure my post like](#strctrmypstlk) [[toblog]] [[webext]]
    -   [developing firefox/chrome extensions?](#dvlpngfrfxchrmxtnsns) 
    -   [post about testing grasp?](#pstbttstnggrsp) [[testing]]
-   [`[2020-01-25]` [h-dev] Abridged summary of dev@list.hypothes.is - 1 update in 1 topic](#hdvbrdgdsmmryfdvlsthypthsspdtntpc) 
-   [`[2019-12-09]` Add \`web-ext submit\` to submit listed add-ons to AMO · Issue #804 · mozilla/web-ext https://github.com/mozilla/web-ext/issues/804](#ddwbxtsbmttsbmtlstdddnstmzllwbxtsgthbcmmzllwbxtsss) 
-   [`[2020-04-22]` Publish Firefox extension on addons.mozilla.org · Issue #310 · hypothesis/browser-extension](#sgthbcmhypthssbrwsrxtnsnsmzllrgsshypthssbrwsrxtnsn) 
-   [`[2020-11-09]` A-C: WebExtensions and AddOns](#sgthbcmrgsmzllmblprjctscrdcwbxtnsnsndddns) 
-   [`[2021-03-12]` Mozilla is a political organisation now. Has been for a few years. Install kiwi&#x2026; | Hacker News](#snwsycmbntrcmtmdmzllspltchsbnfrfwyrsnstllkwhckrnws) [[firefox]] [[webext]]





# tips etc





## Apply the Javascript best practices      [[js]]

use  

-   Flow or Typescript
-   ES6
-   Promise API
-   Fetch API




# addons.mozilla.org publishing      [[amo]]





## releasing new PUBLIC version on AMO

apparently doesn't work through webext regardless. once it's autosigned, you're screwed??  
so to publish on AMO you always have to upload the zip  

-   with<sub>secrets</sub> ./build &#x2013;firefox &#x2013;release &#x2013;lint  
    dump the zip extension
-   choose to upload it AS LISTED on AMO
-   git archive master &#x2013;output=promnesia-source.zip &#x2013; upload source

huh. interesting, it seemed to have published instantly&#x2026;  

-   `[2020-05-19]` and again, published immediately&#x2026; odd!




# `[2019-08-18]` [fregante/Awesome-WebExtensions: A curated list of awesome resources for WebExtensions development.](https://github.com/fregante/Awesome-WebExtensions#readme)      [[promnesia]] [[grasp]] [[webext]]

    Chrome Webstore Upload - Upload the extension to the Chrome Web Store via cli (or on Travis, automatically).




## `[2019-09-02]` <https://github.com/LinusU/wext-shipit> this works also for firefox?      [[webext]] [[firefox]]




# `[2019-08-18]` [use sinon-chrome? Mocks the Chrome Extensions API for testing](https://github.com/acvetkov/sinon-chrome)      [[grasp]] [[promnesia]] [[webext]]




# `[2019-08-28]` Working with quota on mobile browsers: A research report on browser storage - HTML5 Rocks      [[html]] [[webext]]

:LOGBOOK:  

-   State "START"      from "TODO"       `[2019-09-07]`

:END: <https://www.html5rocks.com/en/tutorials/offline/quota-research/>   




## `[2019-09-07]` To do this research, I have built a tool called Browser Storage Abuser to minimize the manual work. You can store as much data as possible to see the limit of each storage on your browser.




## `[2019-09-07]` Android firefox: For IndexedDB, you can use up to 50MB on desktop, 5MB on mobile for free. However, the user can allow the limit to be removed by granting permission.




# `[2019-05-01]` telotortium/org-capture-extension at native-messaging-host

<https://github.com/telotortium/org-capture-extension/tree/native-messaging-host>  

    Native Messaging Host
    This is a version of the Org Capture Extension using the Chrome Native Messaging host




## `[2019-08-10]` [hmm firefox also got it?](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Native_messaging)




## `[2020-02-15]` ok, seems tricky, and apparently requires installing via OS




# `[2019-09-08]` [fregante/webext-options-sync: Helps you manage and autosave your extension's options. Chrome and Firefox.](https://github.com/fregante/webext-options-sync)      [[promnesia]] [[grasp]]

    webext-domain-permission-toggle -




# `[2019-08-29]` [javascript - Chrome messaging: chrome.runtime.sendMessage not working on the newest release 49 - Stack Overflow](https://stackoverflow.com/questions/35857606/chrome-messaging-chrome-runtime-sendmessage-not-working-on-the-newest-release-4)      [[webext]]

    This is the intended behaviour. Messages were not supposed to be received by the sending page. The old behaviour was a bug. This is discussed in these bug reports: 479425 479951.




# browser<sub>action</sub> impacts presense of menu item on android..      [[webext]]




# `[2019-10-27]` Re: [fregante/webext-options-sync] feat: optionally use chrome.storage.local (#19) - karlicoss@gmail.com - Gmail

    I'd rather not offer this option because I think cross-device sync is always preferable from the user's point of view, but I'm willing to add this for extensions with options that are meant to be local (e.g. a port number)
    PR welcome, documentation included.




# `[2019-09-08]` [let the user decide what storage type shall be used by obama · Pull Request #8 · fregante/webext-options-sync](https://github.com/fregante/webext-options-sync/pull/8/commits/58aea6988d268b73f197894839a3318d909b06a0)




# `[2019-09-08]` notlmn/browser-extension-template: Barebones boilerplate with webpack, options handler and auto-publishing      [[grasp]] [[webext]]

<https://github.com/notlmn/browser-extension-template>  

    Features
        Use modern Promise-based browser.* APIs webextension-polyfill.
        Auto-syncing options.
        Auto-publishing with auto-versioning and support for manual releases.
        Extensive configuration documentation.




# `[2020-02-08]` [Discontinuing support for beta versions | Mozilla Add-ons Blog](https://blog.mozilla.org/addons/2018/02/28/discontinuing-support-for-beta-versions/)

    AMO supports signing self-hosted (unlisted) versions, which we believe is a good replacement. With self-hosted versions, developers can create multiple development update channels if needed. They can easily move users between channels. The main caveat is that the files and update mechanisms need to be hosted by the developer




# `[2020-02-15]` [How to add comments to package.json? - DEV Community 👩‍💻👨‍💻](https://dev.to/napolux/how-to-add-comments-to-packagejson-5doi)      [[toblog]]

    How to add comments to package.json?




# `[2020-02-15]` [xo - npm](https://www.npmjs.com/package/xo)

    Opinionated but configurable ESLint wrapper with lots of goodies included. Enforces strict and readable code. Never discuss code style on a pull request again! No decision-making. No .eslintrc or .jshintrc to manage. It just works!




# `[2020-02-15]` [browser-extension-template/options-storage.js at master · notlmn/browser-extension-template](https://github.com/notlmn/browser-extension-template/blob/master/source/options-storage.js)

    import OptionsSync from 'webext-options-sync';




# `[2020-02-15]` [notlmn/browser-extension-template: Barebones boilerplate with webpack, options handler and auto-publishing](https://github.com/notlmn/browser-extension-template#publishing)

    Target respective browsers using .babelrc.




# `[2020-02-15]` [DrewML/chrome-webstore-upload-cli: Upload/Publish Chrome Web Store extensions from the CLI](https://github.com/DrewML/chrome-webstore-upload-cli)      [[webext]]

    chrome-webstore-upload-cli

-   comment

    guide for publishing on chrome store




# `[2020-02-21]` [Choosing a browser to write extensions for | Lobsters](https://lobste.rs/s/2bq29z/choosing_browser_write_extensions_for)

    Thanks for the advice! I was actually inspired to go down this route by seeing the things you’ve been building. I think my interests are similar, but not quite the same.
    There are two main extensions I want to build. First, a way to archive and mark up webpages. There is a Chrome extension called Weava that does something similar, but it’s SaaS and I doesn’t seem to have a convenient export format.
    Second, I would like better history tools. In particular, often have the problem that I read an article or page and want to link to it in a blog post (or similar), but I’ve forgotten how I found it. I’d like an extension that can maintain “chains” of followed links so that I can always look up how I found something.
    I’m happy to get in touch and consider collaborating if you’re interested.




# `[2020-02-18]` [mozilla/web-ext: A command line tool to help build, run, and test web extensions](https://github.com/mozilla/web-ext)

    Hi! This tool is under active development. To get involved you can watch the repo, file issues, create pull requests, or ask a question on dev-addons




# `[2020-02-18]` [Add \`web-ext submit\` to submit listed add-ons to AMO · Issue #804 · mozilla/web-ext](https://github.com/mozilla/web-ext/issues/804)

    web-ext submit would submit to amo only. If you want the zip you can already use web-ext build




# `[2018-11-08]` Shraymonks/flow-interfaces-chrome: Flow interface declarations for the Chrome extensions API      [[js]] [[flow]]

<https://github.com/Shraymonks/flow-interfaces-chrome/>  

    npm install --save-dev flow-interfaces-chrome




# `[2020-02-17]` [Introducing Prism: An awesome new syntax highlighter | Lea Verou](https://lea.verou.me/2012/07/introducing-prism-an-awesome-new-syntax-highlighter/#more-1841)




# chrome got far better profiling, better debugging information + screenshots      [[webext]]




# ugh, can't force webpack/chrome into using date in the version&#x2026;      [[webext]]

<https://developer.chrome.com/apps/manifest/version>  




# `[2020-04-05]` [roam-toolkit/webpack.config.js at master · roam-unofficial/roam-toolkit](https://github.com/roam-unofficial/roam-toolkit/blob/master/webpack.config.js)      [[webext]]

    new webpack.DefinePlugin({
    			'NODE_ENV': JSON.stringify(nodeEnv),
    			'WEB_BROWSER': JSON.stringify(webBrowser),
    		}),

-   comment

    hmm wonder if this is useful?




# `[2018-03-29]` how webext works?

background runs all the time. communicate with extension via message passing. TODO runtime<sub>handlers</sub>?  
content scripts have no access to background  
make sure you return false at the end  




# logging 

from content page, `console.log` goes to the page console, whereas from the rest to `background.html`  




# `[2020-11-04]` [softvar/awesome-web-storage: Everything you need to know about Client-side Storage.](https://github.com/softvar/awesome-web-storage)      [[webext]] [[js]]




# `[2020-05-14]` [Let's guess what Google requires in 14 days or they kill our extension | Hacker News](https://news.ycombinator.com/item?id=23168874)      [[webext]]

    In practice I was able to use native messaging to spawn the executable but to actually talk with it I needed to use a websocket, kind of defeating the point.




# for fucks sake. releasing even without 'unlisted' channel doesn't make it automatically submitted for manual review???





## `[2020-02-15]` ok, first time you need to create manually; after that, get the id (it's public, so ok to put in a git repo) and use it with the build script




## `[2020-05-17]` listed vs unlisted

so according to this <https://blog.mozilla.org/addons/2017/01/26/mixing-listed-and-unlisted-on-amo> , you can have mixed self distributed/AMO with the same extension id, but not the same version  
so adding &#x2013;unlisted is a reasonable way to beta test  
the only confusing bit is why it is still queueing for reviews??  




## ugh why did I end up with several versions of grasp on AMO??

it feels that signing is enough to upload. next time try waiting for a bit..  
<https://addons.mozilla.org/en-US/developers/addons>  




# `[2020-05-24]` [Manage Events with Background Scripts - Google Chrome](https://developer.chrome.com/extensions/background_pages)

    The only occasion to keep a background script persistently active is if the extension uses chrome.webRequest API to block or modify network requests. The webRequest API is incompatible with non-persistent background pages.




# `[2020-05-13]` [Let's guess what Google requires in 14 days or they kill our extension | Hacker News](https://news.ycombinator.com/item?id=23168874#23171176)      [[google]]

-   `[2020-05-13]` [Let's guess what Google requires in 14 days or they kill our extension | Hacker News](https://news.ycombinator.com/item?id=23168874)




# `[2019-07-07]` client/security.rst at 734e3a25318364819a8c38ef881e4788a2b06365 · hypothesis/client      [[webext]] [[security]]

<https://github.com/hypothesis/client/blob/734e3a25318364819a8c38ef881e4788a2b06365/docs/developers/security.rst>  




## `[2019-08-04]` For example: in order to draw highlights, the annotated page needs to know the location of annotations, but it does not ever need to know the body text of an an annotation, and so it should not be possible to expose this over the messaging interface.




# `[2020-11-09]` [Web Developer's Toolbox – Add-ons for Firefox (en-GB)](https://addons.mozilla.org/en-GB/firefox/collections/4757633/webdeveloper/)      [[webext]]




# android debugging

`web-ext run --target=firefox-android --android-device=XXXX`  




## `[2019-08-10]` remote debugging; use `Shift-F8` to open web ide <https://developer.mozilla.org/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_with_WebIDE#Enable_remote_debugging_in_Firefox_for_Android>




# `[2019-02-16]` Creating a Chrome extension in 2018: The good, the bad and the meh | Checkly

<https://checklyhq.com/blog/2018/08/creating-a-chrome-extension-in-2018-the-good-the-bad-and-the-meh/>  




## `[2019-08-10]` basic intro with examples of testing and explaining the extensions architecture




## `[2019-06-01]` Creating a Chrome extension in 2018: The good, the bad and the meh      [[grasp]]

<https://blog.checklyhq.com/creating-a-chrome-extension-in-2018-the-good-the-bad-and-the-meh/>  

    // boots a Chrome instance using Puppeteer and adds the extension we build in the earlier test
      test('it installs the extension', async () => {
        const options = {




# `[2019-06-29]` Using Firefox WebExtensions with Selenium

<https://intoli.com/blog/firefox-extensions-with-selenium/>  
nice, this guy contributed to selenium?  




# `[2019-06-29]` Standard8/example-webextension: Example repository containing templates and good practices for creating a WebExtension for Firefox

<https://github.com/Standard8/example-webextension/>  

    Example repository containing templates and good practices for creating a WebExtension for Firefox




# `[2019-07-08]` GUI and Headless Browser Testing - Travis CI      [[ci]]

<https://docs.travis-ci.com/user/gui-and-headless-browsers/#using-the-chrome-addon-in-the-headless-mode>  

    Using the Firefox addon in headless mode #
    
    Starting with version 56, Firefox can be used in “headless” mode, which is suitable for driving browser-based tests using Selenium and other tools. Headless mode can be enabled using the MOZ_HEADLESS environment variable:
    
    env:
      - MOZ_HEADLESS=1
    addons:
      firefox: latest




# `[2019-06-12]` Getting started with web-ext - Mozilla | MDN

<https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Getting_started_with_web-ext>  




## `[2019-08-10]` web-ext is a nice tool for signing, linting and even simple browser testing (e.g. web-ext run)




# `[2019-06-12]` Extensions in Firefox 66 | Mozilla Add-ons Blog

<https://blog.mozilla.org/addons/2019/02/15/extensions-in-firefox-66/>  

    Firefox no longer emits a warning when the manifest property `background.persistent` is set to `true`.




# `[2019-06-12]` commands.update() - Mozilla | MDN

<https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/API/commands/update>  




## `[2019-06-12]` 1475043 - Allow commands.update() to un-set a shortcut, disabling the command

<https://bugzilla.mozilla.org/show_bug.cgi?id=1475043>  




# `[2019-06-12]` Differences between desktop and Android extensions - Mozilla | MDN

<https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Differences_between_desktop_and_Android>  




# `[2019-06-12]` 1520119 - Support removing a shortcut in manage shortcuts

<https://bugzilla.mozilla.org/show_bug.cgi?id=1520119>  




# `[2019-06-12]` Debugging Firefox for Android over WiFi - Firefox Developer Tools | MDN

<https://developer.mozilla.org/en-US/docs/Tools/Remote_Debugging/Debugging_Firefox_for_Android_over_Wifi>  

    The computer with desktop Firefox and your Android device must be connected to the same Wi-Fi network. Desktop Firefox cannot be using a wired connection that routes to the Wi-Fi network; both must truly be on Wi-Fi.




# `[2019-06-12]` Developing extensions for Firefox for Android - Mozilla | MDN

<https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Developing_WebExtensions_for_Firefox_for_Android#Install_and_run_your_extension_in_Firefox_for_Android>  




## `[2019-08-10]` need to open browser on android prior to running web-ext command!




# `[2019-06-12]` Setting up an extension development environment - Archive of obsolete content | MDN

<https://developer.mozilla.org/en-US/docs/Archive/Add-ons/Setting_up_extension_development_environment>  




# `[2019-07-07]` javascript - How to make side panel in chrome extension? - Stack Overflow

<https://stackoverflow.com/questions/39610205/how-to-make-side-panel-in-chrome-extension>  




# `[2019-06-01]` Extensionizr - boilerplate for your chrome extension

    http://extensionizr.com/!#{%22modules%22:[%22hidden-mode%22,%22with-bg%22,%22with-persistent-bg%22,%22no-options%22,%22no-override%22],%22boolean_perms%22:[],%22match_ptrns%22:[]}




# `[2019-06-01]` Creating a history clearing Chrome extension | Jake Lee

<https://blog.jakelee.co.uk/creating-a-history-clearing-chrome-extension/>  




## `[2019-08-10]` pretty simple guide




# `[2019-06-13]` what is the state of add-on/extensions development for firefox? : firefox

<https://www.reddit.com/r/firefox/comments/886wms/what_is_the_state_of_addonextensions_development/>  

    I think you're supposed to call "browser.*" and I would not be surprised if calling "chrome.*" gets deprecated on the long term)




# `[2020-12-07]` Webext special commands      [[webext]]

\_execute<sub>browser</sub><sub>action</sub>: works like a click on the extension's browser action.  
\_execute<sub>page</sub><sub>action</sub>: works like a click on the extension's page action.  
\_execute<sub>sidebar</sub><sub>action</sub>: opens the extension's sidebar. Only supported in Firefox 54 and newer.  




# `[2020-11-09]` [Element | Malleable Systems Collective](https://app.element.io/#/room/#malleable-systems:matrix.org)

    Ohh thanks! I thought the 'browser console' was just a log at first, apparently you have to enable devtools.chrome.enabled in about:config first for the terminal to show up!




# `[2019-09-22]` javascript - Chrome extension - page update twice then removed on YouTube - Stack Overflow      [[promnesia]]

<https://stackoverflow.com/questions/36808309/chrome-extension-page-update-twice-then-removed-on-youtube/36818991#36818991>  




# `[2020-05-05]` [wildcard/chrome-autoreload.js at master · geoffreylitt/wildcard](https://github.com/geoffreylitt/wildcard/blob/master/chrome-autoreload.js)      [[webext]]




# `[2019-12-09]` Request the right permissions | Extension Workshop

<https://extensionworkshop.com/documentation/develop/request-the-right-permissions/#Request_permissions_at_runtime>  

    A good example of this approach is Gesturefy, which offers users the following advice:




# `[2020-07-28]` Mozilla Add-ons Blog

<https://blog.mozilla.org/addons/>  




# `[2020-05-05]` [feat: Added option to \`&#x2013;watch-file\` to address eager reloading by jezhou · Pull Request #1784 · mozilla/web-ext](https://github.com/mozilla/web-ext/pull/1784)




# `[2020-05-24]` [Understanding Google Chrome Extensions](https://gist.github.com/jjperezaguinaga/4243341)




# `[2019-08-29]` Implement a settings page - Mozilla | MDN      [[webext]]

<https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Implement_a_settings_page>  

    You can also open this page programmatically using the runtime.openOptionsPage() function.




# `[2019-04-21]` When to use margin vs padding in CSS - Stack Overflow      [[css]]

<https://stackoverflow.com/questions/2189452/when-to-use-margin-vs-padding-in-css>  

    To me, the biggest difference between padding and margin is that vertical margins auto-collapse, and padding doesn't.




## `[2019-05-13]` {margins} collapse {paddings} dont      [[drill]] [[css]]





### `[2019-10-27]` mnemonic is alphabetic order? dunno.




## `[2019-05-13]` this is also a good example for drill      [[spacedrep]] [[toblog]]




# js library for chrome settings, too annoying to bind them manually..      [[promnesia]] [[grasp]]





## `[2019-08-24]` found something the other day; must be in links




# `[2019-11-19]` [Question] How to set cors headers? · Issue #308 · http-party/http-server      [[cors]]

<https://github.com/http-party/http-server/issues/308>  
fucking hell, why is that shit so hard???  




# `[2019-11-18]` python - Enable access control on simple HTTP server - Stack Overflow      [[cors]]

<https://stackoverflow.com/questions/21956683/enable-access-control-on-simple-http-server>  

    @HairOfTheDog The SimpleHTTPRequestHandler doesn’t support the OPTIONS HTTP method. You could add it if you want (read the Python manual about HTTP servers); or you could just not try to access the server like that.




# right, set up logins in about:profiles .after that it gets cloned      [[webext]]




# `[2019-06-13]` fuck. looks like firefox doesn't allow persistent dev extensions, that really sucks. and unbranded version doesn't have PPA? wtf? how are developers supposed to test their stuff      [[firefox]]




# `[2019-08-31]` uBlock/manifest.json at 6c34b3c3c96756b6db7ff2f3a0394472d81cde3e · gorhill/uBlock

<https://github.com/gorhill/uBlock/blob/6c34b3c3c96756b6db7ff2f3a0394472d81cde3e/platform/webext/manifest.json>  

    "options_ui": {
        "page": "dashboard.html",
        "open_in_tab": true
      },




# `[2019-09-01]` keepassxc-browser/manifest.json at develop · keepassxreboot/keepassxc-browser      [[webext]]

<https://github.com/keepassxreboot/keepassxc-browser/blob/develop/keepassxc-browser/manifest.json>  

    "options_ui": {
        "page": "options/options.html",
        "open_in_tab": true
    },




# `[2020-11-15]` [Content scripts - Mozilla | MDN](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_scripts#Connection-based_messaging)




# `[2020-10-19]` [1309288 - Install addons permanently from about:debugging](https://bugzilla.mozilla.org/show_bug.cgi?id=1309288)




# `[2020-11-10]` [In Chrome Extension development, how do I pass a variable from background.js to a content script that embedded as a script node? - Stack Overflow](https://stackoverflow.com/questions/49209913/in-chrome-extension-development-how-do-i-pass-a-variable-from-background-js-to)

    getBackgroundPage returns the JavaScript 'window' object for the background page running inside the current extension and not in the content script.




# `[2020-11-10]` [Chrome extension: message from background.js to content.js - Stack Overflow](https://stackoverflow.com/questions/26766268/chrome-extension-message-from-background-js-to-content-js)

    chrome.runtime.sendMessage sends a message to all open extension pages (i.e. background, popup, etc.)
    chrome.tabs.sendMessage sends a message to all content scripts from the extension in a given tab (possibly filtered by frame ID)




# What I learned about writing web extensions      [[webext]] [[blog]]





## there is an incredible lack of documentation for building web extensions and the best practices      [[webext]] [[blog]]

combining it with npm/webpack weirdness and kind of slow feedback loop (reloading etc, it makes it very hard)  




## 1. Use JS Flow 2. Use async. I mean, seriously.      [[js]] [[webext]]





### `[2019-09-29]` could link that stackoverflow post and replace typescript advice with flow?




## structure my post like      [[toblog]] [[webext]]

-   what is very hard or broken
-   what it's ought to be?
-   how I fixed it in the meantime




## developing firefox/chrome extensions?




## post about testing grasp?      [[testing]]




# `[2020-01-25]` [h-dev] Abridged summary of dev@list.hypothes.is - 1 update in 1 topic

    I think that it works last I checked! There is only a need to get the build
    infrastructure working and have an owner on addons.mozilla.org, and for
    Mozilla to approve it.




# `[2019-12-09]` Add \`web-ext submit\` to submit listed add-ons to AMO · Issue #804 · mozilla/web-ext <https://github.com/mozilla/web-ext/issues/804>

    Automate all the things! wink Here people discussed the Chrome Web Store version, but it also applies to AMO sindresorhus/module-requests#66




# `[2020-04-22]` [Publish Firefox extension on addons.mozilla.org · Issue #310 · hypothesis/browser-extension](https://github.com/hypothesis/browser-extension/issues/310)

    I know it's not perfect and I would also like to see a Firefox addon, but some friends and I have been using Hypothesis seamlessly in Firefox, both for desktop and for mobile, following the instructions I posted here: https://medium.com/@delahera/hypothesis-web-annotation-mobile-358db1f9ec46




# `[2020-11-09]` [A-C: WebExtensions and AddOns](https://github.com/orgs/mozilla-mobile/projects/44#card-26664450)




# `[2021-03-12]` [Mozilla is a political organisation now. Has been for a few years. Install kiwi&#x2026; | Hacker News](https://news.ycombinator.com/item?id=26423981)      [[firefox]] [[webext]]

    Install kiwi on Android for extension enabled Chromium.

