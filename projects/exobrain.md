
# Table of Contents

-   [\* motivation](#mtvtn) 
    -   [There are lots of cool links which I might never get to explore](#thrrltsfcllnkswhchmghtnvrgttxplr) 
    -   [why?](#why) 
    -   [basically explain, which stuff I maintain and which stuff I keep as a dump. seems like a good compromise](#bscllyxplnwhchstffmntnndwchstffkpsdmpsmslkgdcmprms) 
    -   [`[2020-04-13]` Tanami/websights: Just a personal web directory of stuff that I want to keep in my head.](#sgthbcmtnmwbsghtstnmwbsghdrctryfstffthtwnttkpnmyhd) 
    -   [so I want a personal wiki similar to what Nikita Voloboev got, but with org-mode](#swntprsnlwksmlrtwhtnktvlbvgtbtwthrgmd) [[blog]] [[pkm]]
        -   [`[2019-12-03]` related: is there plugin for fuzzy/stemming search in firefox?](#rltdsthrplgnfrfzzystmmngsrchnfrfx) [[search]] [[browsers]]
    -   [`[2021-01-16]` even if it's just a very raw dump, chances are someone might run into them while googling or searching on github](#vnftsjstvryrwdmpchncsrsmnntthmwhlgglngrsrchngngthb) 
-   [\* current implementation](#crrntmplmnttn) 
    -   [`[2020-01-03]` Mirror org-org export, It could be public, under version control and allow for privacy controls](#mrrrrgrgxprttcldbpblcndrvsncntrlndllwfrprvcycntrls) [[pkm]]
    -   [`[2020-11-15]` logseq/logseq: A privacy-first, open-source platform for knowledge sharing and management.](#sgthbcmlgsqlgsqlgsqlgsqprtfrmfrknwldgshrngndmngmnt) [[logseq]]
    -   [maybe each page got main content, and then just related links/highlights below?](#mybchpggtmncntntndthnjstrltdlnkshghlghtsblw) 
    -   [`[2020-12-15]` Emacs Org-mode: Use good header ids!](#swrtqtrgrtclsmcsrgmdgnrtdshtmlmcsrgmdsgdhdrds) [[blog]] [[org]] [[linkrot]]
    -   [`[2020-12-15]` UOMF: Linking Headings](#skrlvttmflnknghdngsmflnknghdngs) 
    -   [def ned quick capture.. and then maybe dispatch items via tags](#dfndqckcptrndthnmybdsptchtmsvtgs) [[org]]
    -   [need to support self tags in TOC? when I specify custom TOC header they don't seem to work, shit.](#ndtspprtslftgsntcwhnspcfycstmtchdrthydntsmtwrksht) 
    -   [do not emit empty <tag> and nbsp??](#dntmtmptytgndnbsp) [[org]]
    -   [trying to use org-ql, but not sure if it's that good for tag cloud](#tryngtsrgqlbtntsrftsthtgdfrtgcld) 
    -   [scrolling org-mode into active in the sidebar](#scrllngrgmdntctvnthsdbr) 
    -   [on tag click &#x2013; search over all tags](#ntgclcksrchvrlltgs) 
    -   [maybe group by tags? could even do it via orgparse](#mybgrpbytgscldvndtvrgprs) 
    -   [output links (at least the ones with tags) to pinboard?](#tptlnkstlstthnswthtgstpnbrd) 
    -   [not sure what to do about filetags?](#ntsrwhttdbtfltgs) 
    -   [`[2021-01-04]` make public generated files read only?](#mkpblcgnrtdflsrdnly) 
    -   [maybe generate TITLE, set to filename (so logseq doesn't stumble over it)](#mybgnrtttlsttflnmslgsqdsntstmblvrt) [[logseq]] [[org]]
-   [\* alternative ways to build it](#ltrntvwystbldt) 
    -   [`[2019-12-22]` ok, ox-hugo generates some odd artifacts, perhaps would be easier with vanilla md export](#kxhggnrtssmddrtfctsprhpswldbsrwthvnllmdxprt) [[blog]]
    -   [`[2020-02-14]` Building a Second Brain in Roam&#x2026;And Why You Might Want To : RoamResearch https://www.reddit.com/r/RoamResearch/comments/eho7de/building\_a\_second\_brain\_in\_roamand\_why\_you\_might](#bldngscndbrnnrmndwhyymghtbldngscndbrnnrmndwhyymght) 
    -   [`[2020-03-11]` MkDocs](#swwwmkdcsrgmkdcs) 
    -   [try publishing with dendron and publish in discord?](#trypblshngwthdndrnndpblshndscrd) 
        -   [`[2021-01-16]` it's very cool, but similar problems to mdbook &#x2013; if it's not mardown in the first plays, gonna be a lot of work to maintain org->md conversion, and nothing beats emacs](#tsvryclbtsmlrprblmstmdbkftnrgmdcnvrsnndnthngbtsmcs) 
    -   [`[2019-12-22]` Markbook - A replacement for Gitbook/mdBook written in Node.js : javascript](#mrkbkrplcmntfrgtbkmdbkwrttnnndjsjvscrpt) 
        -   [`[2020-03-06]` it's a new project, not sure what's the benefit over mdbook](#tsnwprjctntsrwhtsthbnftvrmdbk) 
    -   [seems that github codespaces would be perfect for it?](#smsthtgthbcdspcswldbprfctfrt) 
    -   [`[2020-11-05]` Org Mode - Dendron](#swwwdndrnsntscddfbdfcbhtmlrgmddndrn) 
    -   [export my stuff as notion database?](#xprtmystffsntndtbs) 
    -   [mdbook](#mdbk) 
        -   [`[2019-12-22]` softprops/awesome-mdbook: 🕶️🗃️ a card catalog of mdbooks for your reading curiosity](#sgthbcmsftprpswsmmdbksftprdctlgfmdbksfryrrdngcrsty) 
        -   [`[2020-03-21]` Configuration - mdBook Documentation](#cnfgrtnmdbkdcmnttn) 
        -   [`[2020-06-30]` remove fontawesome](#rmvfntwsm) 
        -   [`[2020-03-07]` think about using mdbook watch on beepb00p](#thnkbtsngmdbkwtchnbpbp) 
-   [\* potential features and inspiration](#ptntlftrsndnsprtn) 
    -   [`[2020-01-25]` mek.fyi | Home](#smkfyqsmkfyhm) [[blog]]
    -   [split hunks by org outlines somehow?](#splthnksbyrgtlnssmhw) [[git]] [[org]]
    -   [maybe tag-based exporting? export/noexport tags for hieriarchies/whole files? let it be a mess with one huge page?](#mybtgbsdxprtngxprtnxprttgrchswhlflslttbmsswthnhgpg) 
    -   [write a tool to analyse tags](#wrttltnlystgs) [[tagging]] [[pkm]]
    -   [`[2020-05-12]` Tweet from @RobertHaisfield https://twitter.com/RobertHaisfield/status/1259990930917953537](#twtfrmrbrthsfldstwttrcmrbrthsfldstts) 
    -   [graph view: need an ability to 'pin' certain nodes to improve graph rendering?](#grphvwndnbltytpncrtnndstmprvgrphrndrng) [[logseq]]
    -   [add link to the source on each page??](#ddlnktthsrcnchpg) 
    -   [links to featured exobrain items?](#lnkstftrdxbrntms) [[blog]]
    -   [instead of todo states, maybe color the first letter(s)?](#nstdftdsttsmybclrthfrstlttrs) [[blog]]
    -   [how to add redirects for moved stuff?](#hwtddrdrctsfrmvdstff) [[linkrot]]
    -   [could expose cloudmacs instance??](#cldxpscldmcsnstnc) [[cloudmacs]]
    -   [`[2021-01-16]` hmm not sure what to do about long and short titles (LOGSEQ<sub>TITLE</sub> things). maybe it should be a toggle or something](#hmmntsrwhttdbtlngndshrtttthngsmybtshldbtgglrsmthng) [[logseq]]
    -   [build custom agendas? that way, easy to make tag views](#bldcstmgndsthtwysytmktgvws) [[org]]
    -   [`[2020-10-16]` Full introduction to Gkroam, up to version v2.3.7, no voice /r/orgmode](#srddtcmrrgmdcmmntsjclkfllrdctntgkrmptvrsnvnvcrrgmd) 
    -   [`[2019-12-17]` Notes - Gwern.net https://www.gwern.net/Notes](#ntsgwrnntswwwgwrnntnts) [[search]]
    -   [if I add wiki-style links, hide them by default, but show on some hotkey?](#fddwkstyllnkshdthmbydfltbtshwnsmhtky) [[blog]]
    -   [`[2020-05-03]` 🔮Pensieve - Pensieve](#swkrmshndlycmpnsvpnsv) 
    -   [Tweet from @nikitavoloboev](#twtfrmnktvlbv) 
    -   [Implement incremental search, backed by some indexer?](#mplmntncrmntlsrchbckdbysmndxr) [[search]]
-   [\* other's exobrains](#other) 
    -   [`[2020-08-06]` Home](#scmmnplcdbllpntstckdntsfwkshtmlhm) [[org]]
        -   [`[2020-08-25]` ok, nice, using org-mode?  https://doubleloop.net/2020/08/21/how-publish-org-roam-wiki-org-publish/#more-7091](#kncsngrgmdsdbllpnthwpblshrgrmwkrgpblshmr) 
    -   [`[2020-02-21]` Andy Matuschak's Public Notes](#snwsycmbntrcmtmdndymtschkspblcnts) 
        -   [`[2020-03-12]` hmm, no notes? odd..](#hmmnntsdd) 
    -   [`[2020-08-20]` Things and Stuff Wiki](#swkthngsndstffrgmnpgthngsndstffwk) 
    -   [`[2020-05-06]` Notes ‒ Szymon Kaliski nice backlink summary](#sszymnklskcmntsntsszymnklskncbcklnksmmry) 
    -   [`[2020-03-01]` daryllxd/lifelong-learning: ✅ ✅ ✅ A massive repo filled with notes on everything from coding to philosophy to psychology to marketing to product](#sgthbcmdryllxdlflnglrnngdphytpsychlgytmrktngtprdct) 
    -   [`[2020-03-01]` d2s/knowledge: 2016→ — A curated list of Tools and Resources.](#sgthbcmdsknwldgdsknwldgcrtdlstftlsndrsrcs) 
    -   [`[2020-03-05]` Tom Critchlow. Move. Think. Create.](#stmcrtchlwcmwktmcrtchlwmvthnkcrt) 
        -   [`[2020-04-08]` tomcritchlow/tomcritchlow.github.io: Me. Learning to use Github and learning to live life. https://github.com/tomcritchlow/tomcritchlow.github.io](#tmcrtchlwtmcrtchlwgthbmlrbcmtmcrtchlwtmcrtchlwgthb) 
    -   [`[2020-04-02]` davidseah/knowledgebank](#sgthbcmdvdshknwldgbnkdvdshknwldgbnk) 
    -   [`[2020-03-22]` nice, they've got wiki.. https://wiki.mindey.com/](#ncthyvgtwkswkmndycm) 
    -   [`[2020-01-10]` Show your personal websites | Lobsters https://lobste.rs/s/b7lt29/show\_your\_personal\_websites](#shwyrprsnlwbstslbstrsslbstrssbltshwyrprsnlwbsts) [[ideas]]
    -   [`[2020-12-07]` Simon Willison: TIL](#stlsmnwllsnntsmnwllsntl) 
    -   [`[2020-08-26]` barrucadu's memos](#smmbrrcdckbrrcdsmms) 
    -   [`[2020-05-12]` Notes ‒ Szymon Kaliski](#sszymnklskcmntsntsszymnklsk) 
    -   [`[2019-10-17]` Jethro's Braindump  https://braindump.jethro.dev/](#jthrsbrndmpsbrndmpjthrdv) 
    -   [`[2019-12-02]` wayanjimmy/notebook: Personal notes https://github.com/wayanjimmy/notebook](#wynjmmyntbkprsnlntssgthbcmwynjmmyntbk) 
    -   [`[2020-05-12]` About these notes azlen](#sntszlnmgtbyfvbtthsntszln) 
    -   [`[2020-06-12]` seanbreckenridge/exobrain: external brain](#sgthbcmsnbrcknrdgxbrnsnbrcknrdgxbrnxtrnlbrn) 
    -   [`[2020-09-29]` jakechv/wiki: public wiki / knowledge base](#sgthbcmjkchvwkjkchvwkpblcwkknwldgbs) 
    -   [`[2019-12-28]` Personal Notes](#prsnlnts) 
    -   [`[2020-01-13]` Wiki workflow - Everything I know](#wkwrkflwvrythngknw) 
        -   [`[2020-04-26]` would be so damn cool to connect all of these in some sort of search engine?](#wldbsdmncltcnnctllfthsnsmsrtfsrchngn) [[search]] [[agora]]
    -   [`[2020-04-21]` ExoBrain | Jibran Kalia](#sjbrnklcmknwldgxbrnxbrnjbrnkl) 
    -   [`[2020-07-23]` gitbook/exobrain<sub>blog.md</sub> at 1a67afe0d1e20ef31052c3259096c3ec8f89e13b · irosyadi/gitbook](#sgthbcmrsydgtbkblbfdfcccfbrnblgmdtfdfcccfbrsydgtbk) 
    -   [jethrokuan/braindump: knowledge repository managed with org-mode and org-roam.  https://github.com/jethrokuan/braindump](#jthrknbrndmpknwldgrpstrymndrgrmsgthbcmjthrknbrndmp) 
    -   [`[2020-01-30]` davidgasquez/handbook: 📚 Personal bits of knowledge.](#dvdgsqzhndbkprsnlbtsfknwldg) 
    -   [`[2020-01-01]` dvogt23/notes: 📔 knowledge](#dvgtntsknwldg) [[german]] [[inspiration]] [[exobrain]]
        -   [`[2020-01-25]` ok, not very comprehensive, but nice as an example?](#kntvrycmprhnsvbtncsnxmpl) 
    -   [`[2020-01-25]` mek.fyi | Home](#mkfyhm) [[inspiration]]
    -   [barrucadu's memos - Self](#brrcdsmmsslf) 
    -   [`[2020-01-24]` Wiki Index](#wkndx) 
    -   [`[2019-12-23]` wayanjimmy/notebook: Personal notes/knowledge base](#wynjmmyntbkprsnlntsknwldgbs) 
    -   [`[2020-03-24]` 0oo](#19930_20396) [[exobrain]]
        -   [`[2020-06-03]` damn, that seems fascinating on the second glance](#dmnthtsmsfscntngnthscndglnc) 
    -   [`[2019-12-05]` Yoshiki 義樹 on Twitter: "@neauoire @hundredrabbits @visakanv Just found @gordonbrander's patterns page. Personally loving the small pages with clear, focused writing and evocative titles, deeply interconnected, with backlinks for context - it feels like "pure knowledge". This is a lot of fun to get lost in! https://t.co/fxDTQd56zY https://t.co/Y6lxBxAS1D" / Twitter](#yshk義樹ntwttrnrhndrdrbbtsvtcfxdtqdzystcylxbxsdtwttr) [[exobrain]] [[pkm]]
    -   [`[2020-12-02]` barrucadu's memos](#smmbrrcdckbrrcdsmms) 
    -   [`[2020-11-06]` jakeisnt/wiki: public wiki / knowledge base](#sgthbcmjksntwkjksntwkpblcwkknwldgbs) 
    -   [ExoBrain | Jibran Kalia](#xbrnjbrnkl) 
    -   [`[2020-10-18]` Wiki - Contents](#swklpxlndxwkcntnts) [[exobrain]]
    -   [`[2020-08-11]` dufferzafar/notes: A miscellany of thoughts.](#sgthbcmdffrzfrntsdffrzfrntsmscllnyfthghts) 
    -   [`[2021-03-02]` danielsundermeier/knowledge: Wissenssammlung](#sgthbcmdnlsndrmrknwldgdnlsndrmrknwldgwssnssmmlng) [[german]]
    -   [`[2021-03-13]` Fabien Benetou's PIM | Main / HomePage | Search Results](#fbnbntfrmnhmpgctnsrchqknwgfbnbntspmmnhmpgsrchrslts) [[exobrain]]
-   [\* content to add](#cntnttdd) 
    -   [`[2020-06-03]` publish my subscriptions as org-mode](#pblshmysbscrptnssrgmd) [[rss]] [[orger]]
    -   [most 'imporant' tweets def make sense](#mstmprnttwtsdfmksns) [[twitter]]
-   [\* publicity](#pblcty) 
    -   [publish on org-mode reddit maybe with some highlights](#pblshnrgmdrddtmybwthsmhghlghts) [[outbox]]
    -   [about my simple search?](#btmysmplsrch) [[search]] [[toblog]]
    -   [`[2020-12-31]` ok, so lunr.js seems like the best alternative](#kslnrjssmslkthbstltrntv) [[search]]
-   [think about integrating other people's exobrains?](#thnkbtntgrtngthrpplsxbrns) [[social]] [[extendedmind]]
    -   [`[2021-01-16]` someone started thinking about it! https://anagora.org](#smnstrtdthnkngbttsngrrg) [[agora]]
-   [`[2019-08-18]` How to add full text search to your website - Dev Channel - Medium](#smdmcmdvchnnlhwtddflltxtsltxtsrchtyrwbstdvchnnlmdm) [[blog]] [[search]]
-   [update my-awesome-list occasionally](#pdtmywsmlstccsnlly) [[blog]]
-   [`[2020-03-06]` rust-lang/mdBook: Create book from markdown files. Like Gitbook but implemented in Rust](#sgthbcmrstlngmdbkrstlngmddwnflslkgtbkbtmplmntdnrst) [[linkrot]]
-   [`[2019-12-07]` The Sad State of Personal Knowledgebases | Hacker News https://news.ycombinator.com/item?id=10739227](#thsdsttfprsnlknwldgbsshckrnwssnwsycmbntrcmtmd) [[pkm]]
    -   [`[2019-12-07]` The Sad State of Personal Knowledgebases http://marcusvorwaller.com/blog/2015/12/14/personal-knowledgebases/](#thsdsttfprsnlknwldgbssmrcvrwllrcmblgprsnlknwldgbss) 
-   [`[2020-05-17]` Andy Matuschak on Twitter: "Software interfaces undervalue peripheral vision! (a thread) My physical space is full of subtle cues. Books I read or bought most recently are lying out. Papers are lying in stacks on my desk, roughly arranged by their relationships. https://t.co/ee7lo0mdLv" / Twitter](#ndymtschkntwttrsftwrntrfcythrrltnshpsstclmdlvtwttr) [[vr]] [[think]]
-   [`[2020-03-22]` https://merveilles.town/@maxdeviant/103863978808052366 pkm repo](#smrvllstwnmxdvntpkmrp) 
-   [failed attempt to convert heading + link on the next line (after Grasp) into proper org-mode links](#fldttmpttcnvrthdnglnknthnxtlnftrgrspntprprrgmdlnks) [[org]]
-   [related:](#rltd) [[org]] [[blog]] [[pkm]]
-   [maybe embed my blog posts in this graph? e.g. give them different weight or something](#mybmbdmyblgpstsnthsgrphggvthmdffrntwghtrsmthng) [[logseq]] [[exobrain]]
-   [hmm. if I manage to somehow 'fix' some heavy nodes in place (e.g. in corners), it might be pretty approachable. or maybe addinge more repulsive force would do it anyway](#hmmfmngtsmhwfxsmhvyndsnplybddngmrrplsvfrcwlddtnywy) [[logseq]]
-   [when exporting and link isn't wrapped, strip away protocol and wrap it? not sure if whould do it in org->org or org->html stage (latter is prob easier)](#whnxprtngndlnksntwrppdstrnrgrgrrghtmlstglttrsprbsr) [[org]]
-   [reduce font size for h. tags not sure there is much point in  having them bigger, bold is enough](#rdcfntszfrhtgsntsrthrsmchpntnhvngthmbggrbldsngh) 
-   [encode links to base64? so ids are possible to decode?](#ncdlnkstbssdsrpssbltdcd) 
-   [custom colors for certain nodes (sort of featured. maybe control by tags, but start with just config)](#cstmclrsfrcrtnndssrtfftrdntrlbytgsbtstrtwthjstcnfg) [[logseq]]
-   [pages construct of two parts? the top is maintained and curated, the bottom is chaotic notes that haven't been properly processed yet?](#pgscnstrctftwprtsthtpsmnttsththvntbnprprlyprcssdyt) 
-   [`[2020-05-04]` org-mode support? · Issue #1183 · rust-lang/mdBook](#sgthbcmrstlngmdbksssrgmdspprtssrstlngmdbk) 
-   [`[2020-06-13]` What do I mean by node?](#blgrfxnbtthsblgwhtdmnbyndhtmlwhtdmnbynd) [[exobrain]]
-   [`[2019-12-07]` knowledge/wiki-workflow.md at c978beb37bc769a9925fa6664ed9a4f3be183697 · nikitavoloboev/knowledge](#knwldgwkwrkflwmdtcbbbcfdfbnktvlbvknwldg) [[exobrain]]
-   [`[2020-01-01]` RichardLitt/meta-knowledge: 💡 A list of knowledge repositories](#rchrdlttmtknwldglstfknwldgrpstrs) [[publish]] [[exobrain]]
    -   [`[2020-01-17]` later when I publish my org-mode sources](#ltrwhnpblshmyrgmdsrcs) 
-   [`[2020-12-31]` yeraydiazdiaz/lunr.py: A Python implementation of Lunr.js 🌖](#sgthbcmyrydzdzlnrpyyrydzdzlnrpypythnmplmnttnflnrjs) 
-   [`[2020-12-31]` how to get the positions of the term matches · Issue #96 · weixsong/elasticlunr.js](#sgthbcmwxsnglstclnrjsssshhtrmmtchssswxsnglstclnrjs) [[exobrain]]
-   [`[2021-01-02]` The Org Manual](#srgmdrgrghtmlhtmlspcfcxprtsttngsthrgmnl) 
-   [`[2020-12-27]` Digital-Garden/ideas.md at 1cee3b97439a9d9fb1ae30d8c14dbb7ac32280ad · hrwtech/Digital-Garden](#sgthbcmhrwtchdgtlgrdnblbcbdfbdcdbbcdhrwtchdgtlgrdn) [[ideas]]
    -   [`[2021-01-22]` related](#rltd) [[agora]]
-   [`[2020-12-28]` emacs - Assign IDs to every entry in Org-mode - Stack Overflow](#sstckvrflwcmqstnsssgndstvndstvryntrynrgmdstckvrflw) [[exobrain]]
-   [`[2021-01-23]` graph](#grph) [[logseq]]
-   [`[2020-12-16]` My tier list of interesting YouTube channels - Tristan Hume](#sthmcmyytbtrlstmytrlstfntrstngytbchnnlstrstnhm) 
-   [need refile to inherit parent tag? definitely makes sense for exobrain refiles](#ndrfltnhrtprnttgdfntlymkssnsfrxbrnrfls) [[org]]
-   [wtf? priorities are displayed in the graph now?](#wtfprrtsrdsplydnthgrphnw) [[logseq]]
-   [I guess sibling tags have a bigger weight than parent tags (and especially filetags?)](#gsssblngtgshvbggrwghtthnprnttgsndspcllyfltgs) [[logseq]]
-   [move in old drafts from blog drafts](#mvnlddrftsfrmblgdrfts) 
-   [`[2020-04-03]` maybe sort by priority/date on export? or specify sort order in properties](#mybsrtbyprrtydtnxprtrspcfysrtrdrnprprts) [[exobrain]]
-   [processing process](#prcssngprcss) 
-   [I'm a bit fan of tags. I think it first started around 2012? I got annoyed about not being able to place a bookmark under a single subfolder. blah blah pinboard](#mbtfnftgsthnktfrststrtdrnkndrsnglsbfldrblhblhpnbrd) [[toblog]] [[self]] [[exobrain]]
    -   [`[2019-10-08]` perhaps it belongs in personal wiki category? and organizing information?](#prhpstblngsnprsnlwkctgryndrgnzngnfrmtn) 
    -   [`[2019-10-08]` two separate directories. (notes/zim) zim is more like knowledge archive, it's more structred. notes are more chaotic and generally a giant todo list](#twsprtdrctrsntszmzmsmrlkktsrmrchtcndgnrllygnttdlst) 
-   [Summarise things that interest me via org tags](#smmrsthngsthtntrstmvrgtgs) [[exobrain]]
-   [right, seems that async/background export still uses only one process :(](#rghtsmsthtsyncbckgrndxprtstllssnlynprcss) [[org]]
-   [move ideas page into exobrain](#mvdspgntxbrn) [[blog]]
-   [need to jack in public stuff like twitter/hypothesis/reddit/hackernews?](#ndtjcknpblcstfflktwttrhypthssrddthckrnws) [[exobrain]]
-   [snapshot every month and plot an animation for the graph?](#snpshtvrymnthndpltnnmtnfrthgrph) [[exobrain]]
-   [post an announcement](#pstnnnncmnt) [[exobrain]] [[toblog]]
-   [maybe add a keybinding to force clean? this would make it much easier, won't have to rerun anything](#mybddkybndngtfrcclnthswldmktmchsrwnthvtrrnnythng) [[exobrain]]
-   [demonstrate how I wanted to learn physics & be a bit more healthy and over qs, pkm etc it grew into the clusterfuck which is in the middle](#dmnstrthwwntdtlrnphyscsbbwntthclstrfckwhchsnthmddl) [[exobrain]] [[toblog]] [[outbox]]
-   [How to force crawlers to process it?](#hwtfrccrwlrstprcsst) [[exobrain]]
-   [`[2021-01-23]` Force directed graph: custom forces - Tom Roth](#stmrthcmfdgcstmfrcdrctdgrphcstmfrcstmrth) [[blog]] [[inspiration]]
-   [`[2021-01-30]` Getting Started - IndieWeb](#sndwbrggttngstrtdgttngstrtdndwb) 
-   [`[2021-01-06]` garden/exobrain.md at 69fe163b30a00e76e3eb8637c97fa86ac0fb2a9e · flancian/garden](#sgthbcmflncngrdnblbfbbcfcnxbrnmdtfbbcfcfbflncngrdn) 
-   [`[2021-01-23]` vasturiano/react-force-graph: React component for 2D, 3D, VR and AR force directed graphs](#sgthbcmvstrnrctfrcgrphvstnntfrddvrndrfrcdrctdgrphs) [[exobrain]]
-   [export state changes (esp. with comments?)](#xprtsttchngsspwthcmmnts) [[org]]
-   [sync with #pinboard? should be super easy now with inherited tags&#x2026;.](#syncwthpnbrdshldbsprsynwwthnhrtdtgs) [[pinboard]]
-   [`[2020-12-30]` Agora](#sngrrgndgrgr) 
-   ["dragging nodes pins them in fixed position"](#drggngndspnsthmnfxdpstn) [[exobrain]]
-   [notion interface/remnote interface?](#ntnntrfcrmntntrfc) [[exobrain]]
-   [would be nice to highlight actual text (e.g. difference color for property drawers, markup etc)](#wldbncthghlghtctltxtgdffrncclrfrprprtydrwrsmrkptc) [[exobrain]]
-   [interaction: "Do you know about X? Have you seen/heard of X?"](#ntrctndyknwbtxhvysnhrdfx) [[exobrain]]
-   [ok, def need a proper exobrain agenda with all high prio todo/strt items](#kdfndprprxbrngndwthllhghprtdstrttms) [[exobrain]]
-   [things that became evident](#thngsthtbcmvdnt) [[exobrain]] [[totweet]]
-   [`[2021-02-11]` #🧠-v2-personal](#sdscrdcmchnnlsvprsnl) [[exobrain]]
-   [need to make sure there is no "export" tag, otherwise it'll exclude the rest of the file](#ndtmksrthrsnxprttgthrwstllxcldthrstfthfl) 
-   [`[2021-02-14]` Marcin Ignac on Twitter: "I'm fascinated by @andy<sub>matuschak</sub> digital garden of his notes at https://t.co/G9PQ1UaIeq. At the same time i'm disappointed by the tools available to navigate those kind of information spaces. So here is quick thread how I got from the hairball graph to a readable concept map 1/5 https://t.co/rEZhDRpQP5" / Twitter](#stwttrcmmrcngncsttsmrcngnblcncptmpstcrzhdrpqptwttr) [[exobrain]]
    -   [`[2021-02-14]` whoa, need to go through athens discord to figure it out&#x2026; https://discord.com/channels/708122962422792194/708156396906086468](#whndtgthrghthnsdscrdtfgrttsdscrdcmchnnls) 
-   [hmm. use external git repo that commits evey minute? it would track changes automatically and solve all of my timestamp issues?](#hmmsxtrnlgtrpthtcmmtsvymnmtcllyndslvllfmytmstmpsss) [[orgmode]] [[exobrain]]
-   [404 page, suggest to search or look on github history](#pgsggsttsrchrlkngthbhstry) [[exobrain]]
-   [principle: as much as possible should be public](#prncplsmchspssblshldbpblc) [[exobrain]]
-   [Use cdots in toc to indicate level?](#scdtsntctndctlvl) [[exobrain]]
-   [Need a link to homepage..](#ndlnkthmpg) [[exobrain]] [[blog]]
-   [`[2021-03-13]` Fabien Benetou's PIM | Site / AllRecentChanges](#sfbnbntfrstllrcntchngsfbnbntspmstllrcntchngs) [[exobrain]]
-   [need to render todo state changes](#ndtrndrtdsttchngs) [[exobrain]]
-   [generate tag summaries to eliminate the least common?](#gnrttgsmmrstlmntthlstcmmn) [[exobrain]]





# \* motivation





## There are lots of cool links which I might never get to explore

However I did spend time 'curating' them, so perhaps they could serve as a kick off point for someone else  




## why? 

delegate link processing to the outside world. Maybe someone runs into them and gets inspired #extendedmind  




## basically explain, which stuff I maintain and which stuff I keep as a dump. seems like a good compromise




## `[2020-04-13]` [Tanami/websights: Just a personal web directory of stuff that I want to keep in my head.](https://github.com/Tanami/websights)

    my theory: all people eventually reach the point where they accrue enough debris that it becomes necessary to distribute it in order to move forward with their thinking

yes, so much this  




## so I want a personal wiki similar to what Nikita Voloboev got, but with org-mode      [[blog]] [[pkm]]

gitbook has got nice almost realtime search but only supports markdown. also they are not open source?  

<https://github.com/qdot/org-gitbook> &#x2013; weird thing, split my headings into different pages  
had to package-install ox-gfm first  

-   `[2019-12-02]` dunno, maybe starting with single page with links dump (sorted by tags then date?) and that wouldn't even require index?  
    ignore priorities at first?
-   `[2019-12-02]` one simple thing to do would be just generating html pages (with normal emacs export?) and then running JS indexer against HTML pages? could do when blog is compiled

tedious to upgrade though, but a good start?  

-   `[2019-12-03]` maybe, display everything as a single page, then it's easy to search?




### `[2019-12-03]` related: is there plugin for fuzzy/stemming search in firefox?      [[search]] [[browsers]]




## `[2021-01-16]` even if it's just a very raw dump, chances are someone might run into them while googling or searching on github




# \* current implementation

via native emacs org-mode export, see <https://github.com/karlicoss/exobrain-compiler/blob/master/src/build.py>  




## `[2020-01-03]` Mirror org-org export, It could be public, under version control and allow for privacy controls      [[pkm]]




## `[2020-11-15]` [logseq/logseq: A privacy-first, open-source platform for knowledge sharing and management.](https://github.com/logseq/logseq)      [[logseq]]

figuring it out as an extra interface, and for the graph  




## maybe each page got main content, and then just related links/highlights below?




## `[2020-12-15]` [Emacs Org-mode: Use good header ids!](https://writequit.org/articles/emacs-org-mode-generate-ids.html)      [[blog]] [[org]] [[linkrot]]




## `[2020-12-15]` [UOMF: Linking Headings](https://karl-voit.at/2019/11/16/UOMF-Linking-Headings/)

    So I kept using :ID:.




## def ned quick capture.. and then maybe dispatch items via tags      [[org]]




## need to support self tags in TOC? when I specify custom TOC header they don't seem to work, shit.




## do not emit empty <tag> and nbsp??      [[org]]




## trying to use org-ql, but not sure if it's that good for tag cloud

maybe useful for tag summaries?  

    '--directory', root_dir / 'src/org-ql',
    '--directory', root_dir / 'src/ts.el',
    '--directory', root_dir / 'src/peg',
    '--eval', f'''
    (progn
    (message "%s" (org-ql "{input_dir}/memex.org" "memex"))
    )
    '''.strip(),




## scrolling org-mode into active in the sidebar

from mdbook  

    // Scroll sidebar to current active section
    var activeSection = document.getElementById("sidebar").querySelector(".active");
    if (activeSection) {
        // https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollIntoView
        activeSection.scrollIntoView({ block: 'center' });
    }




## on tag click &#x2013; search over all tags




## maybe group by tags? could even do it via orgparse




## output links (at least the ones with tags) to pinboard?

might need a two-step process for a proper diff  




## not sure what to do about filetags?




## `[2021-01-04]` make public generated files read only?




## maybe generate TITLE, set to filename (so logseq doesn't stumble over it)      [[logseq]] [[org]]




# \* alternative ways to build it





## `[2019-12-22]` ok, ox-hugo generates some odd artifacts, perhaps would be easier with vanilla md export      [[blog]]




## `[2020-02-14]` Building a Second Brain in Roam&#x2026;And Why You Might Want To : RoamResearch <https://www.reddit.com/r/RoamResearch/comments/eho7de/building_a_second_brain_in_roamand_why_you_might>




## `[2020-03-11]` [MkDocs](https://www.mkdocs.org/)

hmm, looks pretty nice. wonder if it's better than mdbook  




## try publishing with dendron and publish in discord?





### `[2021-01-16]` it's very cool, but similar problems to mdbook &#x2013; if it's not mardown in the first plays, gonna be a lot of work to maintain org->md conversion, and nothing beats emacs




## `[2019-12-22]` Markbook - A replacement for Gitbook/mdBook written in Node.js : javascript

<https://www.reddit.com/r/javascript/comments/b68k3v/markbook_a_replacement_for_gitbookmdbook_written/>  

    I regarded Gitbook as a FOSS traitor, since it has all but abandoned it's open-source tool for a proprietary web app.




### `[2020-03-06]` it's a new project, not sure what's the benefit over mdbook




## seems that github codespaces would be perfect for it?

I guess I need to get rid of the filter thing? not sure. Would be nice to commit directly into my notes  




## `[2020-11-05]` [Org Mode - Dendron](https://www.dendron.so/notes/c3800271-dd56-46fb-8de7-e850f3c006b7.html)




## export my stuff as notion database?




## mdbook 





### `[2019-12-22]` [softprops/awesome-mdbook: 🕶️🗃️ a card catalog of mdbooks for your reading curiosity](https://github.com/softprops/awesome-mdbook)




### `[2020-03-21]` Configuration - mdBook Documentation

<https://rust-lang.github.io/mdBook/format/config.html>  

    [output.html.search]
    limit-results = 15




### `[2020-06-30]` remove fontawesome




### `[2020-03-07]` think about using mdbook watch on beepb00p




# \* potential features and inspiration





## `[2020-01-25]` [mek.fyi | Home](https://mek.fyi/#qs)      [[blog]]

    (Right click green text to enter Mek's mind map.)

huh, interesting experiment in presenting information  




## split hunks by org outlines somehow?      [[git]] [[org]]




## maybe tag-based exporting? export/noexport tags for hieriarchies/whole files? let it be a mess with one huge page?




## write a tool to analyse tags      [[tagging]] [[pkm]]

-   the tags that are the most common, deserve pages
-   rest are okay to keep adhoc?
-   custom agendas for tags (top level only?)
-   search is really important..




## `[2020-05-12]` Tweet from @RobertHaisfield <https://twitter.com/RobertHaisfield/status/1259990930917953537>

    @RobertHaisfield: @azlenelza I love how you differentiate external from internal links. Very frustrating in other digital gardens to accidentally leave




## graph view: need an ability to 'pin' certain nodes to improve graph rendering?      [[logseq]]




## add link to the source on each page??




## links to featured exobrain items?      [[blog]]




## instead of todo states, maybe color the first letter(s)?      [[blog]]




## how to add redirects for moved stuff?      [[linkrot]]




## could expose cloudmacs instance??      [[cloudmacs]]




## `[2021-01-16]` hmm not sure what to do about long and short titles (LOGSEQ<sub>TITLE</sub> things). maybe it should be a toggle or something      [[logseq]]




## build custom agendas? that way, easy to make tag views      [[org]]




## `[2020-10-16]` [Full introduction to Gkroam, up to version v2.3.7, no voice](https://reddit.com/r/orgmode/comments/jc8lku/full_introduction_to_gkroam_up_to_version_v237_no/) /r/orgmode




## `[2019-12-17]` Notes - Gwern.net <https://www.gwern.net/Notes>      [[search]]

ask gwern if inability to search in collapsed notes bothers him?  




## if I add wiki-style links, hide them by default, but show on some hotkey?      [[blog]]




## `[2020-05-03]` [🔮Pensieve - Pensieve](https://wiki.ramshandilya.com/)

huh, emojis in TOC are quite nice actually?  




## Tweet from @nikitavoloboev

    https://twitter.com/nikitavoloboev/status/1271505869872803849
    @nikitavoloboev: Put in my wiki in @obsdmd and it results in a neat graph of connections.




## Implement incremental search, backed by some indexer?      [[search]]




# \* other's exobrains





## `[2020-08-06]` [Home](https://commonplace.doubleloop.net/?stackedNotes=%2Fwikis.html)      [[org]]





### `[2020-08-25]` ok, nice, using org-mode?  <https://doubleloop.net/2020/08/21/how-publish-org-roam-wiki-org-publish/#more-7091>




## `[2020-02-21]` [Andy Matuschak's Public Notes](https://news.ycombinator.com/item?id=22382094)

<https://notes.andymatuschak.org/About_these_notes>  




### `[2020-03-12]` hmm, no notes? odd..




## `[2020-08-20]` [Things and Stuff Wiki](https://wiki.thingsandstuff.org/Main_Page)

    Things and Stuff Wiki - An organically evolving personal wiki knowledge base

whoa, nice tag cloud on the top  




## `[2020-05-06]` [Notes ‒ Szymon Kaliski](https://szymonkaliski.com/notes/) nice backlink summary




## `[2020-03-01]` [daryllxd/lifelong-learning: ✅ ✅ ✅ A massive repo filled with notes on everything from coding to philosophy to psychology to marketing to product](https://github.com/daryllxd/lifelong-learning)




## `[2020-03-01]` [d2s/knowledge: 2016→ — A curated list of Tools and Resources.](https://github.com/d2s/knowledge)




## `[2020-03-05]` [Tom Critchlow. Move. Think. Create.](https://tomcritchlow.com/wiki/)





### `[2020-04-08]` tomcritchlow/tomcritchlow.github.io: Me. Learning to use Github and learning to live life. <https://github.com/tomcritchlow/tomcritchlow.github.io>

    Me. Learning to use Github and learning to live life. http://tomcritchlow.com




## `[2020-04-02]` [davidseah/knowledgebank](https://github.com/davidseah/knowledgebank)




## `[2020-03-22]` nice, they've got wiki.. <https://wiki.mindey.com/>

also pretty cool, wiki links onto blog pages &#x2013; wonder if I should do it..  




## `[2020-01-10]` Show your personal websites | Lobsters <https://lobste.rs/s/b7lt29/show_your_personal_websites>      [[ideas]]

    My Idea wiki, First written in Erlang, but now in Nim. The Erlang version birthed a simplistic site style that I’ve used a lot in other web app projects. The wiki software behind this site also powers




## `[2020-12-07]` [Simon Willison: TIL](https://til.simonwillison.net/)

    Simon Willison: TIL




## `[2020-08-26]` [barrucadu's memos](https://memo.barrucadu.co.uk/)

looks nice. .  




## `[2020-05-12]` [Notes ‒ Szymon Kaliski](https://szymonkaliski.com/notes)




## `[2019-10-17]` Jethro's Braindump  <https://braindump.jethro.dev/>

    Here lies my exobrain, which started circa 2017. I study about Computer Science, but anything I find noteworthy goes in here. I try to cite as often as I can, but that practice only started recently.




## `[2019-12-02]` wayanjimmy/notebook: Personal notes <https://github.com/wayanjimmy/notebook>




## `[2020-05-12]` [About these notes](https://notes.azlen.me/g3tibyfv/) azlen




## `[2020-06-12]` [seanbreckenridge/exobrain: external brain](https://github.com/seanbreckenridge/exobrain)




## `[2020-09-29]` [jakechv/wiki: public wiki / knowledge base](https://github.com/jakechv/wiki)




## `[2019-12-28]` Personal Notes

<https://wayanjimmy-notebook.netlify.com/introduction>  

    This repository is my knowledge base. I'm using it to remember things and to let my mind interact with yours. Feel free to open issues and pull requests!




## `[2020-01-13]` Wiki workflow - Everything I know

<https://wiki.nikitavoloboev.xyz/other/wiki-workflow#similar-wikis-i-liked>  

    Similar wikis I liked




### `[2020-04-26]` would be so damn cool to connect all of these in some sort of search engine?      [[search]] [[agora]]

I'd rather have my search engine to look over these first  




## `[2020-04-21]` [ExoBrain | Jibran Kalia](https://jibrankalia.com/knowledge/#exobrain)




## `[2020-07-23]` [gitbook/exobrain<sub>blog.md</sub> at 1a67afe0d1e20ef31052c3259096c3ec8f89e13b · irosyadi/gitbook](https://github.com/irosyadi/gitbook/blob/1a67afe0d1e20ef31052c3259096c3ec8f89e13b/irosyadi.github.io/app/exobrain_blog.md)




## jethrokuan/braindump: knowledge repository managed with org-mode and org-roam.  <https://github.com/jethrokuan/braindump>




## `[2020-01-30]` davidgasquez/handbook: 📚 Personal bits of knowledge.

<https://github.com/davidgasquez/handbook>  




## `[2020-01-01]` dvogt23/notes: 📔 knowledge      [[german]] [[inspiration]] [[exobrain]]

<https://github.com/dvogt23/notes>  




### `[2020-01-25]` ok, not very comprehensive, but nice as an example?




## `[2020-01-25]` mek.fyi | Home      [[inspiration]]

<https://mek.fyi/#qs>  

    Right click green text to enter Mek's mind map.




## barrucadu's memos - Self

<https://memo.barrucadu.co.uk/taxon/self.html>  




## `[2020-01-24]` Wiki Index

<https://pbat.ch/wiki>  




## `[2019-12-23]` wayanjimmy/notebook: Personal notes/knowledge base

<https://github.com/wayanjimmy/notebook>  




## `[2020-03-24]` 0oo      [[exobrain]]

<https://0oo.li/>  

    Categories
    Ideas
    Projects
    Users
    About
    Help
    Bug report
    Login
    Light Off
    Multi-Lingual
    Language
    Space to Think
    Understand the world. Discover goals, ideas, projects. Write feedback.




### `[2020-06-03]` damn, that seems fascinating on the second glance




## `[2019-12-05]` Yoshiki 義樹 on Twitter: "@neauoire @hundredrabbits @visakanv Just found @gordonbrander's patterns page. Personally loving the small pages with clear, focused writing and evocative titles, deeply interconnected, with backlinks for context - it feels like "pure knowledge". This is a lot of fun to get lost in! <https://t.co/fxDTQd56zY> <https://t.co/Y6lxBxAS1D>" / Twitter      [[exobrain]] [[pkm]]

<https://twitter.com/yoshikischmitz/status/1202727796755189760>  

    Just found @gordonbrander's  patterns page.
    Personally loving the small pages with clear, focused writing and evocative titles, deeply interconnected, with backlinks for context - it feels like "pure knowledge".




## `[2020-12-02]` [barrucadu's memos](https://memo.barrucadu.co.uk/)

read through their weeknotes  




## `[2020-11-06]` [jakeisnt/wiki: public wiki / knowledge base](https://github.com/jakeisnt/wiki)




## ExoBrain | Jibran Kalia




## `[2020-10-18]` [Wiki - Contents](https://wiki.alopex.li/_index)      [[exobrain]]

cool wiki, by [this person](https://lobste.rs/newest/icefox)  




## `[2020-08-11]` [dufferzafar/notes: A miscellany of thoughts.](https://github.com/dufferzafar/notes)




## `[2021-03-02]` [danielsundermeier/knowledge: Wissenssammlung](https://github.com/danielsundermeier/knowledge)      [[german]]




## `[2021-03-13]` [Fabien Benetou's PIM | Main / HomePage | Search Results](http://fabien.benetou.fr/Main/HomePage?action=search&q=knowledge)      [[exobrain]]




# \* content to add





## `[2020-06-03]` publish my subscriptions as org-mode      [[rss]] [[orger]]




## most 'imporant' tweets def make sense      [[twitter]]

you can't easily sort person's timeline even by objective metrics. let alone picking the tweets that more or less define you  




# \* publicity





## publish on org-mode reddit maybe with some highlights      [[outbox]]




## about my simple search?      [[search]] [[toblog]]




## `[2020-12-31]` ok, so lunr.js seems like the best alternative      [[search]]

<https://github.com/olivernn/lunr.js>  
has (builtin?) highlights, and the linked example looks fairly simple. it still baffles me how hard it is  




# think about integrating other people's exobrains?      [[social]] [[extendedmind]]





## `[2021-01-16]` someone started thinking about it! <https://anagora.org>      [[agora]]




# `[2019-08-18]` [How to add full text search to your website - Dev Channel - Medium](https://medium.com/dev-channel/how-to-add-full-text-search-to-your-website-4e9c80ce2bf4)      [[blog]] [[search]]




# update my-awesome-list occasionally      [[blog]]

<https://github.com/karlicoss/my-awesome-list>  
wonder if some sort of cat (or use references instead)  
mention bookmark archiver as smth that is used for checking url integrity?  




# `[2020-03-06]` [rust-lang/mdBook: Create book from markdown files. Like Gitbook but implemented in Rust](https://github.com/rust-lang/mdBook)      [[linkrot]]

    linkcheck - a backend which will check that all links are valid




# `[2019-12-07]` The Sad State of Personal Knowledgebases | Hacker News <https://news.ycombinator.com/item?id=10739227>      [[pkm]]





## `[2019-12-07]` The Sad State of Personal Knowledgebases <http://marcusvorwaller.com/blog/2015/12/14/personal-knowledgebases/>




# `[2020-05-17]` Andy Matuschak on Twitter: "Software interfaces undervalue peripheral vision! (a thread) My physical space is full of subtle cues. Books I read or bought most recently are lying out. Papers are lying in stacks on my desk, roughly arranged by their relationships. <https://t.co/ee7lo0mdLv>" / Twitter      [[vr]] [[think]]

<https://mobile.twitter.com/andy_matuschak/status/1202663202997170176>  
map my exobrain onto vr somehow?  




# `[2020-03-22]` <https://merveilles.town/@maxdeviant/103863978808052366> pkm repo




# failed attempt to convert heading + link on the next line (after Grasp) into proper org-mode links      [[org]]

    (defun alala ()
      (interactive)
      (let ((res (om-parse-headline-at (point))))
        (edebug)
        (om-headline-set-title! "SUP" nil res)
        (message "%s %s" (point) res)))
    
    ;; (om-headline-set-title! "SUP" nil res)

I don't know wtf is wrong. I don't get how to extract title from the note. (om-get-property :title res) returns some irrelevant shit  




# related:       [[org]] [[blog]] [[pkm]]




# maybe embed my blog posts in this graph? e.g. give them different weight or something      [[logseq]] [[exobrain]]




# hmm. if I manage to somehow 'fix' some heavy nodes in place (e.g. in corners), it might be pretty approachable. or maybe addinge more repulsive force would do it anyway      [[logseq]]




# when exporting and link isn't wrapped, strip away protocol and wrap it? not sure if whould do it in org->org or org->html stage (latter is prob easier)      [[org]]




# reduce font size for h. tags not sure there is much point in  having them bigger, bold is enough




# encode links to base64? so ids are possible to decode?




# custom colors for certain nodes (sort of featured. maybe control by tags, but start with just config)      [[logseq]]




# pages construct of two parts? the top is maintained and curated, the bottom is chaotic notes that haven't been properly processed yet?




# `[2020-05-04]` [org-mode support? · Issue #1183 · rust-lang/mdBook](https://github.com/rust-lang/mdBook/issues/1183)

    I'd be happy to mentor you through the process and review code




# `[2020-06-13]` [What do I mean by node?](http://blog.rfox.eu/en/About_this_blog/What_do_I_mean_by_node.html)      [[exobrain]]

good explanation  




# `[2019-12-07]` knowledge/wiki-workflow.md at c978beb37bc769a9925fa6664ed9a4f3be183697 · nikitavoloboev/knowledge      [[exobrain]]

<https://github.com/nikitavoloboev/knowledge/blob/c978beb37bc769a9925fa6664ed9a4f3be183697/other/wiki-workflow.md#similar-wikis-i-liked>  




# `[2020-01-01]` RichardLitt/meta-knowledge: 💡 A list of knowledge repositories      [[publish]] [[exobrain]]

<https://github.com/RichardLitt/meta-knowledge>  




## `[2020-01-17]` later when I publish my org-mode sources




# `[2020-12-31]` [yeraydiazdiaz/lunr.py: A Python implementation of Lunr.js 🌖](https://github.com/yeraydiazdiaz/lunr.py)




# `[2020-12-31]` [how to get the positions of the term matches · Issue #96 · weixsong/elasticlunr.js](https://github.com/weixsong/elasticlunr.js/issues/96)      [[exobrain]]

ugh. not possible?  




# `[2021-01-02]` [The Org Manual](https://orgmode.org/org.html#HTML-specific-export-settings)




# `[2020-12-27]` [Digital-Garden/ideas.md at 1cee3b97439a9d9fb1ae30d8c14dbb7ac32280ad · hrwtech/Digital-Garden](https://github.com/hrwtech/Digital-Garden/blob/1cee3b97439a9d9fb1ae30d8c14dbb7ac32280ad/Backlog/_Overflow/ideas.md)      [[ideas]]

collect all ideas repos and search over them?  
basically, add to a private search engine thing  




## `[2021-01-22]` related      [[agora]]




# `[2020-12-28]` [emacs - Assign IDs to every entry in Org-mode - Stack Overflow](https://stackoverflow.com/questions/13340616/assign-ids-to-every-entry-in-org-mode)      [[exobrain]]

ugh. not sure about this way&#x2026; at least it's gonna be deterministic then  




# `[2021-01-23]` graph      [[logseq]]

-   repulsive force: charges (forceManyBody)  
    -   distanceMin is interesting (e.g. set to 1000000). pushes unrelated stuff far, but it ends up clumping
    -   distanecMax &#x2013; if I lower it, it ends up clumping + some circular artifacts (although they might be intesting too!)
    -   strenght: setting to something like -400 effectively has the same effect as default zoom? they are just a bit more spread apart  
        ok, -200 is good enough
-   attractive force: forceLink  
    
        return 1 / Math.min(count[link.source.index], count[link.target.index]);
    
    -   defaultStrenght: low value makes it appear like a blob
    -   defaultStrength: smth like 10 completely breaks the simulation?
    -   changing min to max results in 'leafy' nodes pushed very far apart
    -   adding Math.pow(count, 2) &#x2013; weird. I guess pow has similar effect and reduces the force effectively
    -   changing distance to large values &#x2013; again, weird cicrular artifacts??  
        I guess it's sort of an 'expected distance'? and at some point it's dominated by the repulsion anyway. default 30 is good enough




# `[2020-12-16]` [My tier list of interesting YouTube channels - Tristan Hume](https://thume.ca/2020/07/19/my-youtube-tier-list/)




# need refile to inherit parent tag? definitely makes sense for exobrain refiles      [[org]]




# wtf? priorities are displayed in the graph now?      [[logseq]]

for now, suppressing in the config&#x2026;  




# I guess sibling tags have a bigger weight than parent tags (and especially filetags?)      [[logseq]]

e.g. sometimes file has a filetag, but a task is there because it's related for example to exobrain.  
but then it's gonna link the while filetag with the exobrain, which is somewhat misleading  




# move in old drafts from blog drafts




# `[2020-04-03]` maybe sort by priority/date on export? or specify sort order in properties      [[exobrain]]




# processing process

-   use org-ql-search summary (e.g. broken down by tags)
-   if it doesn't belong anywhere, refile to the same file so it 'sinks', esp. useful with 'misc' files




# I'm a bit fan of tags. I think it first started around 2012? I got annoyed about not being able to place a bookmark under a single subfolder. blah blah pinboard      [[toblog]] [[self]] [[exobrain]]

-   State "START"      from "TODO"       `[2019-02-18]`




## `[2019-10-08]` perhaps it belongs in personal wiki category? and organizing information?




## `[2019-10-08]` two separate directories. (notes/zim) zim is more like knowledge archive, it's more structred. notes are more chaotic and generally a giant todo list




# Summarise things that interest me via org tags      [[exobrain]]

That's also an example of how can I use porg  




# right, seems that async/background export still uses only one process :(      [[org]]




# move ideas page into exobrain      [[blog]]




# need to jack in public stuff like twitter/hypothesis/reddit/hackernews?      [[exobrain]]

also how to post-process stuff post-factum? I guess need a way to assign meta-data to stuff.. ugh  
maybe need to generate uid as a property&#x2026;. simple  




# snapshot every month and plot an animation for the graph?      [[exobrain]]




# post an announcement      [[exobrain]] [[toblog]]




# maybe add a keybinding to force clean? this would make it much easier, won't have to rerun anything      [[exobrain]]




# demonstrate how I wanted to learn physics & be a bit more healthy and over qs, pkm etc it grew into the clusterfuck which is in the middle      [[exobrain]] [[toblog]] [[outbox]]

-   some of my oldest notes are on category theory, quantum physics etc. etc (demonstrate some old notes?)
-   same with qs (demonstrate some stats form 2015?)




# How to force crawlers to process it?      [[exobrain]]




# `[2021-01-23]` [Force directed graph: custom forces - Tom Roth](https://tomroth.com.au/fdg-custom/)      [[blog]] [[inspiration]]

    Or maybe you want to utilise your node and link attributes to change the sizes of some nodes over time. You’d use a custom force.

nice indication of links (via background)  




# `[2021-01-30]` [Getting Started - IndieWeb](https://indieweb.org/Getting_Started)




# `[2021-01-06]` [garden/exobrain.md at 69fe163b30a00e76e3eb8637c97fa86ac0fb2a9e · flancian/garden](https://github.com/flancian/garden/blob/69fe163b30a00e76e3eb8637c97fa86ac0fb2a9e/exobrain.md)




# `[2021-01-23]` [vasturiano/react-force-graph: React component for 2D, 3D, VR and AR force directed graphs](https://github.com/vasturiano/react-force-graph)      [[exobrain]]

    Click to expand/collapse nodes (source)

wow, this might really be useful  




# export state changes (esp. with comments?)      [[org]]




# sync with #pinboard? should be super easy now with inherited tags&#x2026;.      [[pinboard]]




# `[2020-12-30]` [Agora](https://anagora.org/node/agora)




# "dragging nodes pins them in fixed position"      [[exobrain]]

add a note that it's convenient to explore the graph  
also need to add link to main exobrain (for now just share it alongside)  
mention mess & slowness  




# notion interface/remnote interface?      [[exobrain]]




# would be nice to highlight actual text (e.g. difference color for property drawers, markup etc)      [[exobrain]]




# interaction: "Do you know about X? Have you seen/heard of X?"      [[exobrain]]

can be answered instantly without waiting for my response!  
again, it's not that removing 'real' interaction is the point, so I'm happy to answer anyway. But it can lead the person to ask a more specific question, for example.  




# ok, def need a proper exobrain agenda with all high prio todo/strt items      [[exobrain]]




# things that became evident      [[exobrain]] [[totweet]]

-   need more toggles/dimension adjustment/graph distance etc etc
-   and&#x2026; need to be decoupled from a specific app




# `[2021-02-11]` [#🧠-v2-personal](https://discord.com/channels/708122962422792194/714656944572596354)      [[exobrain]]

    danieldToday at 7:35 AM
    There is certainly beauty in randomness.
    
    How about an option which presents you a visualisation of a set of random connections in the daily notes (as a link to a new data visualisation page)? Maybe with options to turn on and off certain branches of thought (in cases you are working on something specific). This way you get your daily inspiration right in your daily notes (or you can turn it off if you don't like it).
    
    Ultimately, it would be very unique if these random connections also generate a page with all block and page references to the visualised links. Basically you forgo the problem of an empty page, not knowing where to start.
    
    I am a Social Scientist and my daily bread and butter is to synthesise knowledge, reproduce it, change it and generate new knowledge. However, most importantly, use that knowledge to have an impact in non-academic contexts (where it matters the most, I think).
    Jeff Tang 🏛Today at 8:51 AM
    I was especially thinking about making a Twitter-like feed for mobile, to explore random blocks @danield




# need to make sure there is no "export" tag, otherwise it'll exclude the rest of the file




# `[2021-02-14]` [Marcin Ignac on Twitter: "I'm fascinated by @andy<sub>matuschak</sub> digital garden of his notes at https://t.co/G9PQ1UaIeq. At the same time i'm disappointed by the tools available to navigate those kind of information spaces. So here is quick thread how I got from the hairball graph to a readable concept map 1/5 https://t.co/rEZhDRpQP5" / Twitter](https://twitter.com/marcinignac/status/1282625655725858817)      [[exobrain]]

    I'm fascinated by @andy_matuschak
     digital garden of his notes at http://notes.andymatuschak.org. At the same time i'm disappointed by the tools available to navigate those kind of information spaces. So here is quick thread how I got from the hairball graph to a readable concept map 1/5




## `[2021-02-14]` whoa, need to go through athens discord to figure it out&#x2026; <https://discord.com/channels/708122962422792194/708156396906086468>

<https://github.com/athensresearch/athens/discussions/605>  




# hmm. use external git repo that commits evey minute? it would track changes automatically and solve all of my timestamp issues?      [[orgmode]] [[exobrain]]




# 404 page, suggest to search or look on github history      [[exobrain]]




# principle: as much as possible should be public      [[exobrain]]




# Use cdots in toc to indicate level?      [[exobrain]]




# Need a link to homepage..      [[exobrain]] [[blog]]




# `[2021-03-13]` [Fabien Benetou's PIM | Site / AllRecentChanges](https://fabien.benetou.fr/Site/AllRecentChanges)      [[exobrain]]

recent changes is nice&#x2026;  
but gonna be tricky with org-mode  
maybe enough to generate a view sorted by timestamps  




# need to render todo state changes      [[exobrain]]




# generate tag summaries to eliminate the least common?      [[exobrain]]

