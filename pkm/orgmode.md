
# Table of Contents

-   [related](#rltd) [[pkm]] [[emacs]] [[orgparse]]
-   [organelle is quite good for a project name?](#rgnllsqtgdfrprjctnm) [[project]]
-   [oh for fucks sake it doesn't support file:something.org#::links anymore???](#hfrfckssktdsntspprtflsmthngrglnksnymr) [[github]]
-   [custom timestamp formats for specific file?](#cstmtmstmpfrmtsfrspcfcfl) 
-   [make ,s to "refile to the same file"? i.e. "sink"](#mkstrfltthsmflsnk) 
-   [refile with inherited tags](#rflwthnhrtdtgs) 
    -   [`[2019-02-16]` https://lists.gnu.org/archive/html//emacs-orgmode/2009-04/msg00149.html eh, not very helpful.. looks like it's not there](#slstsgnrgrchvhtmlmcsrgmdmmlhntvryhlpfllkslktsntthr) 
-   [Really need to auto save on some operations? E.g. refile](#rllyndttsvnsmprtnsgrfl) 
-   [`[2019-10-07]` outline sections Weekly /r/Orgmode Open Discussion - October 04, 2019 /r/orgmode](#tlnsctnssrddtcmrrgmdcmmntklyrrgmdpndscssnctbrrrgmd) [[blog]]
-   [`[2018-10-27]` Fast refiling in org-mode with hydras | Josh Moller-Mara https://mollermara.com/blog/Fast-refiling-in-org-mode-with-hydras/](#fstrflngnrgmdwthhydrsjshmmblgfstrflngnrgmdwthhydrs) 
-   [Map unschedule to capital u?](#mpnschdltcptl) 
-   [fucking hell helm tag completion is annyoing](#fcknghllhlmtgcmpltnsnnyng) [[emacs]]
-   [`[2019-10-01]` alphapapa/org-sidebar: A helpful sidebar for Org mode](#lphpprgsdbrhlpflsdbrfrrgmd) 
    -   [`[2019-10-06]` ok, interesting but not sure how it would be useful for me?](#kntrstngbtntsrhwtwldbsflfrm) 
    -   [`[2020-12-06]` org-sidebar-backlinks looks good? maybe  use a sidebar with all todo items summary](#rgsdbrbcklnkslksgdmybssdbrwthlltdtmssmmry) 
-   [`[2019-10-05]` Is it possible to clear src results in org-mode? - Emacs Stack Exchange](#stpssbltclrsrcrsltsnrgmdmcsstckxchng) 
-   [use two different refiles: one file level, another heading level; use heading refile more often](#stwdffrntrflsnfllvlnthrhdnglvlshdngrflmrftn) 
-   [refresh agenda after doing actions on it, right now completed future tasks still appear on agenda](#rfrshgndftrdngctnsntrghtnwcmpltdftrtsksstllpprngnd) 
-   [org-refile: make case insensitive](#rgrflmkcsnsnstv) 
-   [check out more defaul org-evil-agenda bindings](#chcktmrdflrgvlgndbndngs) [[doom]]
-   [`[2020-01-10]` Amazing library for org hackers /r/emacs](#srddtcmrmcscmmntsmrnmznglkrsmznglbrryfrrghckrsrmcs) 
-   [`[2020-02-16]` alphapapa/org-ql: An Org-mode query language, including search commands and saved views](#lphpprgqlnrgmdqrylnggncldngsrchcmmndsndsvdvws) 
-   [Github orgmode handling](#gthbrgmdhndlng) 
    -   [`[2019-07-30]` novoid/github-orgmode-tests: This is a test project where you can explore how github interprets Org-mode files](#nvdgthbrgmdtststhsststprjnxplrhwgthbntrprtsrgmdfls) 
    -   [for fucks sake https://github.com/wallyqs/org-ruby/issues/45](#frfckssksgthbcmwllyqsrgrbysss) 
    -   [named +result heading seems to be broken&#x2026;](#nmdrslthdngsmstbbrkn) 
        -   [`[2020-02-26]` ah, maybe it's fine.. just needs :exports results?](#hmybtsfnjstndsxprtsrslts) 
        -   [`[2020-03-17]` yeah, it's org-ruby and it's `#+results:` thing that's breaking it&#x2026;](#yhtsrgrbyndtsrsltsthngthtsbrkngt) 
        -   [`[2020-05-10]` right. apparently preempting with newline and using a drawe allows not to remove it?](#rghtpprntlyprmptngwthnwlnndsngdrwllwsnttrmvt) 
        -   [`[2020-07-15]` right. apparently, :results scalar wraps it in begin<sub>example</sub> and also works? see kobuddy](#rghtpprntlyrsltssclrwrpstnbgnxmplndlswrksskbddy) 
    -   [ugh, seems that #+result drawer fails to render?](#ghsmsthtrsltdrwrflstrndr) 
    -   [caveat: github doesn't respect your custom ids](#cvtgthbdsntrspctyrcstmds) [[transclusion]] [[github]] [[org]]
-   [search for completed tasks that have todo subtasks?](#srchfrcmpltdtsksththvtdsbtsks) 
-   [perhaps need to filter some files for org-ql search](#prhpsndtfltrsmflsfrrgqlsrch) 
-   [autorefresh agenda?](#trfrshgnd) 
-   [hide drill from agenda](#hddrllfrmgnd) 
-   [`[2019-10-26]` Code blocks - Org Babel reference card](#cdblcksrgbblrfrnccrd) [[blog]]
-   [`[2020-02-06]` Introducing Org Roam - Jethro Kuan](#ntrdcngrgrmjthrkn) 
-   [inline tasks tips](#nlntskstps) 
    -   [`[2019-10-04]` Weekly /r/Orgmode Open Discussion - October 04, 2019 /r/orgmode](#srddtcmrrgmdcmmntsddwrwklklyrrgmdpndscssnctbrrrgmd) 
    -   [`[2019-10-04]` Weekly /r/Orgmode Open Discussion - October 04, 2019 /r/orgmode](#srddtcmrrgmdcmmntsddwrwklklyrrgmdpndscssnctbrrrgmd) 
    -   [`[2019-10-04]` Weekly /r/Orgmode Open Discussion - October 04, 2019 /r/orgmode](#srddtcmrrgmdcmmntsddwrwklklyrrgmdpndscssnctbrrrgmd) 
    -   [`[2019-12-17]` Annotating everything: overview of Linux/Android tools for active reading /r/opensource](#srddtcmrpnsrccmmntsczgsnnlnxndrdtlsfrctvrdngrpnsrc) 
-   [not sure if need to use org-id-track-globally???](#ntsrfndtsrgdtrckglblly) 
-   [think of better hotkeys for agenda deadline and schedule settings](#thnkfbttrhtkysfrgndddlnndschdlsttngs) 
-   [shortcut to insert org style date in arbitrary place](#shrtcttnsrtrgstyldtnrbtrryplc) [[emacs]]
    -   [`[2020-06-03]` ugh! desperately need insert-date things](#ghdsprtlyndnsrtdtthngs) 
    -   [`[2020-06-09]` use my/now C-t? maybe alt-t is better or something](#smynwctmyblttsbttrrsmthng) [[habit]]
-   [`[2019-03-29]` org mode - Update the org-agenda-daily-view automatically on background - Emacs Stack Exchange](#rgmdpdtthrggnddlyvwtmtcllynbckgrndmcsstckxchng) 
-   [`[2019-05-12]` Org-mode Hidden Gems - 01 Document Structure](#rgmdhddngmsdcmntstrctr) 
-   [`[2020-02-27]` wow, highlighting broken file links is very cool](#wwhghlghtngbrknfllnkssvrycl) [[doom]]
-   [`[2020-01-28]` WIP: org-ql-view dispatch popup (like Magit) /r/orgmode](#srddtcmrrgmdcmmntsvkwwprgrgqlvwdsptchppplkmgtrrgmd) [[orgql]]
    -   [`[2020-12-06]` oh wow it's super neat! interactive old-dispatch](#hwwtssprntntrctvlddsptch) 
-   [`[2019-10-26]` m-cat/org-recur: Recurring org-mode tasks](#mctrgrcrrcrrngrgmdtsks) 
    -   [`[2020-06-10]` ugh. |3| didn't work, regardless org-recur-mode or org-recur-agenda-mode&#x2026;](#ghddntwrkrgrdlssrgrcrmdrrgrcrgndmd) 
-   [`[2019-11-02]` Org mode for meeting minutes](#rgmdfrmtngmnts) [[blog]]
-   [add repeat frequency?](#ddrptfrqncy) 
-   [Org agenda bulk reschedule? Via transient mode??](#rggndblkrschdlvtrnsntmd) 
    -   [`[2019-11-02]` mm, ok, I gues 1-7 keys do this well](#mmkgskysdthswll) 
-   [use org-agenda-open-link, set up def browser](#srggndpnlnkstpdfbrwsr) 
-   [hmm, unclear how to emulate RTM behavior with creating new task in regular time periods..](#hmmnclrhwtmltrtmbhvrwthcrtngnwtsknrglrtmprds) 
-   [priority in agenda works in a weird way&#x2026; make sure it jumps at a heading, not body](#prrtyngndwrksnwrdwymksrtjmpsthdngntbdy) 
    -   [`[2020-06-09]` eh? I think it was referring to the priority changing? was resolved probably?](#hthnktwsrfrrngtthprrtychngngwsrslvdprbbly) 
-   [`[2019-02-15]` The Org Manual: Speed keys](#thrgmnlspdkys) 
-   [evil-collection?](#vlcllctn) [[vim]]
-   [:results replace raw appends instead of replacing](#rsltsrplcrwppndsnstdfrplcng) 
-   [use evil-org (subtree manipulation)](#svlrgsbtrmnpltn) 
-   [symlink projects with issues?](#symlnkprjctswthsss) 
-   [have a suggestion for begin<sub>xxx</sub> thing to take in html classes?](#hvsggstnfrbgnxxxthngttknhtmlclsss) 
-   [if it's got pin tag, always keep it on the very top? and don't reorder?](#ftsgtpntglwyskptnthvrytpnddntrrdr) 
-   [maybe need a 'virtual'  "moving notes" mode for orgmode?](#mybndvrtlmvngntsmdfrrgmd) [[think]]
-   [`[2019-10-11]` Weekly /r/Orgmode Open Discussion - October 11, 2019 /r/orgmode](#srddtcmrrgmdcmmntsdgjswklklyrrgmdpndscssnctbrrrgmd) [[performance]]
-   [attempt to display org-ql results in a window](#ttmpttdsplyrgqlrsltsnwndw) [[orgql]]
-   [`[2020-05-06]` (1) EmacsConf 2019 - 05 - Use Org mode when away from the desktop - Zen Monk Alain M. Lafon - YouTube](#swwwytbcmwtchvjjcxylstplmyfrmthdsktpznmnklnmlfnytb) [[blog]]
-   [clipping/capturing images](#clppngcptrngmgs) 
-   [figure out pro and cons lists](#fgrtprndcnslsts) 
    -   [`[2018-06-20]` PRO and CON lists](#prndcnlsts) 
-   [need 'save all'&#x2026; or autosave on refile?](#ndsvllrtsvnrfl) [[emacs]]
-   [`[2018-08-25]` need feedback for org-mode web app - view/search org files from Dropbox on web : orgmode](#ndfdbckfrrgmdwbppvwsrchrgflsfrmdrpbxnwbrgmd) 
    -   [`[2019-01-13]` https://www.reddit.com/r/orgmode/comments/9522eg/need\_feedback\_for\_orgmode\_web\_app\_viewsearch\_org/](#swwwrddtcmrrgmdcmmntsgndfdbckfrrgmdwbppvwsrchrg) 
    -   [`[2019-03-27]` looks broken :(](#lksbrkn) 
    -   [`[2019-05-30]` still no updates&#x2026;](#stllnpdts) 
-   [how to separate or archive org state history?](#hwtsprtrrchvrgstthstry) 
-   [agenda: for sorting, need global list of all scheduled/deadline items sorted by priority](#gndfrsrtngndglbllstfllschdldddlntmssrtdbyprrty) 
-   [do not detect timestamp as cloze? is that even possible?](#dntdtcttmstmpsclzsthtvnpssbl) [[orgdrill]]
-   [`[2019-02-10]` profiler - How do I speed up org-mode agenda generation - Emacs Stack Exchange](#prflrhwdspdprgmdgndgnrtnmcsstckxchng) 
-   [sort by tag for quick regrouping?](#srtbytgfrqckrgrpng) 
-   [support time with seconds precision?](#spprttmwthscndsprcsn) [[setup]]
    -   [`[2019-06-23]` https://stackoverflow.com/a/25668739/706389 Take note that it's defined as a constant, so you're not encouraged to fiddle with it (but you still can:).](#sstckvrflwcmtkntthttsdfndntncrgdtfddlwthtbtystllcn) 
-   [helm-org-refile is a bit stupid; e.g. try refiling to 'watch'](#hlmrgrflsbtstpdgtryrflngtwtch) 
-   [`[2019-10-23]` [O] noweb strip-export](#nwbstrpxprt) 
-   [could potentially be convenient for org mode exports?](#cldptntllybcnvnntfrrgmdxprts) [[mimemacs]]
-   [`[2019-10-05]` emacs - Inline code in org-mode - Stack Overflow](#mcsnlncdnrgmdstckvrflw) 
-   [`[2019-10-26]` Code blocks - Org Babel reference card](#cdblcksrgbblrfrnccrd) [[blog]]
-   [org-next-visible-heading hotkey?](#rgnxtvsblhdnghtky) [[setup]]
-   [`[2020-01-10]` ndwarshuis/om.el: A functional library for org-mode](#ndwrshsmlfnctnllbrryfrrgmd) 
-   [`[2020-05-03]` A Featureful Blog made with Emacs Org-mode : emacs](#swwwrddtcmrmcscmmntsgckvfmdftrflblgmdwthmcsrgmdmcs) 
-   [`[2020-11-24]` landakram/org-z: Lightweight, Org-mode flavored zettelkasten links.](#sgthbcmlndkrmrgzlndkrmrgzwghtrgmdflvrdzttlkstnlnks) 
-   [`[2020-06-09]` my/org-sort-entries &#x2013; actually it's good it's keeping stable sort for same prios](#myrgsrtntrsctllytsgdtskpngstblsrtfrsmprs) 
-   [make ,s to "refile to the same file"? i.e. "sink"](#mkstrfltthsmflsnk) 
-   [try org-sort?](#tryrgsrt) 
-   [`[2020-10-09]` Org Syntax (draft)](#srgmdrgwrgdvrgsyntxhtmlrgsyntxdrft) 
-   [function to 'sink' a heading down till the next priority.. might be unstable though](#fnctntsnkhdngdwntllthnxtprrtymghtbnstblthgh) 
-   [org-ql-search change view format](#rgqlsrchchngvwfrmt) 
-   [`[2019-10-31]` DONE tasks with different color /r/orgmode](#srddtcmrrgmdcmmntsdpkwdnthhdntskswthdffrntclrrrgmd) 
-   [`[2019-11-14]` Python Source Code Blocks in Org Mode](#pythnsrccdblcksnrgmd) 
-   [I think resume doesn't work when you do org-drill-habits](#thnkrsmdsntwrkwhnydrgdrllhbts) [[orgdrill]]
-   [`[2020-04-26]` toshism/org-super-links: Package to create links with auto backlinks](#sgthbcmtshsmrgsprlnkstshskspckgtcrtlnkswthtbcklnks) 
-   [`[2019-10-30]` Weekly tips/trick/etc/ thread /r/emacs](#srddtcmrmcscmmntsdmrlwklythclwklytpstrcktcthrdrmcs) 
-   [Introduction to "organice" - Using Org mode from a smartphone or browser | Lobsters](#ntrdctntrgncsngrgmdfrmsmrtphnrbrwsrlbstrs) 
-   [right, export is weird when output contains \* heading?](#rghtxprtswrdwhntptcntnshdng) 
-   [disable org-indent-mode??](#dsblrgndntmd) [[doom]]
-   [set org-directory just in case? also good for relative path to capture templates](#strgdrctryjstncslsgdfrrltvpthtcptrtmplts) 
-   [clipping images](#clppngmgs) 
-   [`[2019-12-26]` The Org Manual: Literal examples](#thrgmnlltrlxmpls) 
-   [postpone with a small exponent? not sure](#pstpnwthsmllxpnntntsr) 
-   [org-agenda-filter-by-tag (then - to exclude at TAB to select tag) is very nice for ad-hoc switching?](#rggndfltrbytgthntxcldttbtslcttgsvryncfrdhcswtchng) [[habit]]
-   [paranoid mode: check for broken headings](#prndmdchckfrbrknhdngs) [[setup]]
-   [`[2020-11-14]` Who needs GitHub to manage a project when you have Emacs and Org /r/emacs](#srddtcmrmcscmmntsjtydywhnmngprjctwhnyhvmcsndrgrmcs) 
    -   [`[2020-12-11]` tab-bar-mode and global-tab-line-mode ?](#tbbrmdndglbltblnmd) 
-   [`[2020-06-07]` Orgro: an org-mode viewer for mobile /r/emacs](#srddtcmrmcscmmntsgybdbqrgfrmblrgrnrgmdvwrfrmblrmcs) 
    -   [`[2020-10-24]` waiting for fdroid https://github.com/amake/orgro/issues/15](#wtngfrfdrdsgthbcmmkrgrsss) 
-   [`[2020-12-17]` UOMF: Using Org Mode Categories Versus Tags](#skrlvttctgrsvrsstgsmfsngrgmdctgrsvrsstgs) [[habit]]
-   [use ,. for refiling to current file](#sfrrflngtcrrntfl) [[habit]]
-   [have a repository of org-mode demo files? generate it w.r.t to today so it's easy to demonstrate? org could hack current day somehow, but that could be tricky](#hvrpstryfrgmddmflsgnrttwrcrrntdysmhwbtthtcldbtrcky) 
-   [file variables](#flvrbls) 
-   [archive entries (org-archive-subtree)](#rchvntrsrgrchvsbtr) 
-   [archive tag to hide subtree (org-toggle-archive-tag)](#rchvtgthdsbtrrgtgglrchvtg) 
-   [repeat interval cookies](#rptntrvlcks) 
-   [agenda sometimes takes A LOT of time to rerender. I think we need an inotify async server&#x2026;](#gndsmtmstksltftmtrrndrthnkwndnntfysyncsrvr) 
-   [go thought archives occasionally to check for accidentally archived? Then mark](#gthghtrchvsccsnllytchckfrccdntllyrchvdthnmrk) 
-   [tagging files, then org view into them](#tggngflsthnrgvwntthm) 
-   [`[2020-04-12]` Literal Examples (The Org Manual)](#srgmdrgmnlltrlxmplshtmlltrlxmplsthrgmnl) 
-   [habits/drill should probably have importance? So the unimportant things are showed less frequently](#hbtsdrllshldprbblyhvmprtnprtntthngsrshwdlssfrqntly) [[spacedrep]]
-   [for drill, only consider stuff that isn't done?](#frdrllnlycnsdrstffthtsntdn) 
-   [check for corrupted headings, typically it's stars and todo states out of nowhere](#chckfrcrrptdhdngstypcllytsstrsndtdsttstfnwhr) 
-   [`[2019-10-05]` Re: [O] Bug: spurious newline after comment](#rbgsprsnwlnftrcmmnt) 
-   [`[2019-09-22]` alphapapa/org-super-agenda: Supercharge your Org daily/weekly agenda by grouping items](#lphpprgsprgndsprchrgyrrgdlywklygndbygrpngtms) 
-   [weirdness with encoding in Polar documents](#wrdnsswthncdngnplrdcmnts) [[polar]] [[org]] [[emacs]]
-   [`[2019-10-22]` Rethink: Org mode meets professional web design /r/emacs](#srddtcmrmcscmmntsdllhrrthkrgmdmtsprfssnlwbdsgnrmcs) [[org]]
-   [refile is weird in terms of fuzzy matching (log.org)](#rflswrdntrmsffzzymtchnglgrg) [[emacs]] [[org]]
    -   [maybe contribute to spacemacs?? not sure why the source was async in the first place&#x2026;](#mybcntrbttspcmcsntsrwhythsrcwssyncnthfrstplc) 
-   [`[2018-06-10]` fniessen/org-html-themes: How to export Org mode files into awesome HTML in 2 minutes](#fnssnrghtmlthmshwtxprtrgmdflsntwsmhtmlnmnts) [[org]] [[blog]]
    -   [`[2018-10-28]`  eh, not so sure about it. doesn't look nice](#hntssrbttdsntlknc) 
-   [shit, I need agda-like unicode input](#shtndgdlkncdnpt) [[org]] [[emacs]] [[math]] [[study]]
-   [`[2019-10-27]` org babel - How to automatically tangle another source block to file when evaluate a source block in org-mode? - Emacs Stack Exchange](#rgbblhwttmtcllytnglnthrsrtsrcblcknrgmdmcsstckxchng) 
-   [org-clock is oddly satisfying](#rgclcksddlystsfyng) [[org]]
-   [add CREATED to entry (add-created would be enough)](#ddcrtdtntryddcrtdwldbngh) [[emacs]] [[org]]
-   [figure out how to find and jump a file](#fgrthwtfndndjmpfl) [[org]]
-   [`[2017-12-23]` custom timestamp format](#cstmtmstmpfrmt) [[org]]
-   [do not count timestamps as cloze](#dntcnttmstmpssclz) [[emacs]] [[orgdrill]]
-   [Org mode exporting to html](#rgmdxprtngthtml) 
-   [display links as raw links](#dsplylnkssrwlnks) [[emacs]] [[org]]
    -   [`[2019-11-02]` eh?](#h) 
-   [`[2019-07-29]` sort by property TAGS](#srtbyprprtytgs) [[org]]
-   [`[2019-10-23]` The Org Manual: Extracting source code](#thrgmnlxtrctngsrccd) 
-   [`[2019-10-05]` The Org Manual: Structure of code blocks](#thrgmnlstrctrfcdblcks) 
-   [selecting drill items org-drill-entry-p](#slctngdrlltmsrgdrllntryp) [[org]]
-   [two kinds of refiles? one with headings, one without?](#twkndsfrflsnwthhdngsnwtht) [[emacs]]
-   [the 'notes' marker doesn't work as expected? only shows subtasks](#thntsmrkrdsntwrksxpctdnlyshwssbtsks) [[emacs]]
-   [do not make org todo state change pop up as a new window](#dntmkrgtdsttchngpppsnwwndw) [[emacs]]
-   [Exclude done/cancelled from drill?](#xclddncnclldfrmdrll) [[emacs]]
-   [`[2019-12-10]` The Org Manual](#thrgmnl) [[blog]]
-   [Large life-logging org-mode file gets too slow](#lrglflggngrgmdflgtstslw) 
-   [Org-mode Hidden Gems - 03 Hyperlinks](#rgmdhddngmshyprlnks) 
-   [org archive &#x2013; check for not TODOs?](#rgrchvchckfrnttds) [[emacs]]
    -   [`[2019-11-02]` eh?](#h) 
-   [wonder if this was causing issues for me in test.org ?](#wndrfthswscsngsssfrmntstrg) [[doom]]
-   [how to refresh agenda in the background? so it reflects changes in files instantly without saving](#hwtrfrshgndnthbckgrndstrfschngsnflsnstntlywthtsvng) [[emacs]]
-   [`[2020-09-22]` When refiling: Invalid function: org-preserve-local-variables · Issue #1116 · hlissner/doom-emacs](#sgthbcmhlssnrdmmcsssswhnrrsrvlclvrblssshlssnrdmmcs) 
-   [shit, looks my coefficient makes 3,4,5 pretty much irrelevant](#shtlksmycffcntmksprttymchrrlvnt) [[spacedrep]] [[orgdrill]]
-   [hotkey to sort entries by created date](#htkytsrtntrsbycrtddt) [[emacs]]
-   [some items should not contribute to global agenda. e.g. subtasks of an item](#smtmsshldntcntrbttglblgndgsbtsksfntm) [[org]] [[gtd]]
-   [send push on org capture change, sync on android?](#sndpshnrgcptrchngsyncnndrd) [[org]] [[android]]
-   [eh, perhaps I need some automated tool to interact with org mode and move around the items? although clog is kind of ok&#x2026;](#hprhpsndsmtmtdtltntrctwthdmvrndthtmslthghclgskndfk) [[org]]
-   [automatic watch later, deduced by tag, sync with youtube playlist](#tmtcwtchltrddcdbytgsyncwthytbplylst) [[org]]
-   [use org-mode for docs? also make sure to keep old commit link as example of using ipython for literate docs](#srgmdfrdcslsmksrtkpldcmmtnksxmplfsngpythnfrltrtdcs) [[cachew]] [[literate]] [[jupyter]]
-   [`[2019-10-26]` EmacsConf 2019 - Schedule](#mcscnfschdl) [[towatch]]
-   [`[2019-12-04]` Org mode for Emacs – Release notes](#rgmdfrmcsrlsnts) [[org]]
-   [`[2019-10-19]` org-emms - MELPA](#rgmmsmlp) [[org]] [[annotation]]
-   [`[2019-09-25]` Blog Series: Using Org Mode Features (UOMF)](#blgsrssngrgmdftrsmf) [[org]]
-   [`[2020-02-13]` alphapapa/org-almanac: Almanac for Org mode](#lphpprglmnclmncfrrgmd) [[org]]
-   [`[2019-11-15]` alphapapa/org-protocol-capture-html: Capture HTML from the browser selection into Emacs as org-mode content](#lphpprgprtclcptrhtmlcptrhbrwsrslctnntmcssrgmdcntnt) [[org]] [[capture]]
-   [`[2021-01-04]` ~ vs = : the former preserves underscores? so better to use it?](#vsthfrmrprsrvsndrscrssbttrtst) [[org]]
-   [`[2019-07-20]` Org-mode Frequently Asked Questions](#rgmdfrqntlyskdqstns) [[org]]
-   [`[2020-01-28]` Some org-mode features you may not know /r/orgmode](#srddtcmrrgmdcmmntsvxsmrgmnwsmrgmdftrsymyntknwrrgmd) 
-   [`[2019-10-06]` Emacs Org-mode - a system for note-taking and project planning - YouTube](#mcsrgmdsystmfrnttkngndprjctplnnngytb) 
-   [`[2019-09-05]` hmm, actually org-brain is pretty keyboard oriented. not sure how good is it in visualising stuff&#x2026;](#hmmctllyrgbrnsprttykybrdrntdntsrhwgdstnvslsngstff) 
-   [`[2019-09-05]` orgbrain: ok, it was somewhat interesting, but not sure if I it's visual enough&#x2026;](#rgbrnktwssmwhtntrstngbtntsrftsvslngh) 
-   [`[2018-07-24]` Kungsgeten/org-brain: Org-mode wiki + concept-mapping](#kngsgtnrgbrnrgmdwkcncptmppng) [[pkm]]
-   [`[2018-07-24]` Civilizer - Cleverly manage your data/knowledge/idea](#cvlzrclvrlymngyrdtknwldgd) [[pkm]]
-   [`[2019-01-17]` BuboFlash - helps with learning](#bbflshhlpswthlrnng) [[pkm]] [[spacedrep]]
-   [`[2021-01-20]` ugh. need some sanity checker for broken outlines](#ghndsmsntychckrfrbrkntlns) [[org]]
-   [`[2021-01-01]` viebel/klipse: Klipse is a Javacript plugin for embedding interactive code snippets in tech blogs. A simple client-side code evaluator pluggable on any web page: clojure, ruby, javascript, python, scheme, es2017, jsx, brainfuck, c++, reagent, lua, ocaml, reasonml, prolog, common lisp](#sgthbcmvblklpsvblklpsklpscrgntlcmlrsnmlprlgcmmnlsp) [[org]] [[literate]]
-   [`[2021-01-16]` emacs - How to use the function option of org-capture correctly? - Stack Overflow](#sstckvrflwcmqstnshwtsthfntnfrgcptrcrrctlystckvrflw) 
-   [`[2020-12-28]` Advanced Export Configuration (The Org Manual)](#srgmdrgmnldvncdxprtcnfgrtmldvncdxprtcnfgrtnthrgmnl) 
-   [`[2019-05-18]` Weekly /r/Orgmode Open Discussion - May 10, 2019 /r/orgmode](#srddtcmrrgmdcmmntsbmxvlvwrwklyrrgmdpndscssnmyrrgmd) [[toblog]] [[publish]]
-   [name: "You need more Org in your life" or something?](#nmyndmrrgnyrlfrsmthng) [[org]]
-   [refile was hard to appreciate until I got used to navigating among multiple files and using several files as org agenda sources](#rflwshrdtpprctntlgtsdtnvgflsndsngsvrlflssrggndsrcs) [[toblog]] [[org]]
-   [motivation for collecting agenda files by myself: emacs is slow and buggy](#mtvtnfrcllctnggndflsbymyslfmcssslwndbggy) [[blog]] [[org]]
    -   [`[2021-01-24]` not sure what I meant there?](#ntsrwhtmntthr) 
-   [Mention that it's very easy to get lost in org features](#mntnthttsvrysytgtlstnrgftrs) [[toblog]] [[pkm]] [[org]]
    -   [`[2019-09-29]` could actually blog why is it org mode vs markdown vs yaml/whatever for me](#cldctllyblgwhystrgmdvsmrkdwnvsymlwhtvrfrm) 
-   [org-capture main motivation: it's immediately in my filesystem.](#rgcptrmnmtvtntsmmdtlynmyflsystm) [[grasp]]
-   [`[2019-10-08]` capture: often I'd put a quick tag if I expect myself to search for that outline later (e.g. if I need to buy something), or if it's some thought related to one of the projects I'm doing. If it's something I really need to remember I'd also schedule it.](#cptrftndptqcktgfxpctmyslfthngrllyndtrmmbrdlsschdlt) 
-   [`[2019-10-08]` capture: I find it less distracting to keep logs (e.g. quantified self style, like sleep, exercise, weight etc) in a separate file.](#cptrfndtlssdstrctngtkplgstyllkslpxrcswghttcnsprtfl) 
-   [(in post about capture)](#npstbtcptr) [[grasp]]
-   [What’s awesome is that at the time of capture it immediately becomes searchable and indexable as any plaintext would without any extra effort (unlike if you added it to browser bookmarks/pinboard).](#whtswsmsthttthtmfcptrtmmdlkfydddttbrwsrbkmrkspnbrd) [[grasp]]
-   [`[2020-04-13]` http://www.acuriousmix.com/2014/09/03/designing-a-personal-knowledgebase motivation for fast capture there](#wwwcrsmxcmdsgnngprsnlknwldgbsmtvtnfrfstcptrthr) 
-   [ask if it would be nice if org-mode supported inline tags?](#skftwldbncfrgmdspprtdnlntgs) [[outbox]] [[reddit]] [[org]]
-   [HTML<sub>CONTAINER</sub> property could be useful..](#htmlcntnrprprtycldbsfl) [[org]] [[exobrain]] [[blog]]
-   [looks like h is hardcoded here&#x2026;](#lkslkhshrdcddhr) 
-   [`[2019-11-21]` Literate Theorem Proving with Org https://chame.co/writeups/org\_coq/post.html](#ltrtthrmprvngwthrgschmcwrtpsrgcqpsthtml) 
-   [Tecos config? Maintainer of org site](#tcscnfgmntnrfrgst) [[org]]
-   [use files as todos? have a crawler go through them and put in a special tasklist](#sflsstdshvcrwlrgthrghthmndptnspcltsklst) [[org]]
    -   [@publicvoit@graz.social thought you'd be a kind of person who knows it &#x2013; is there some existing tool to crawl the filesystem and maintain an org-mode file with todos corresponding to files matching a certain pattern?](#pblcvtgrzsclthghtydbkndfpspndngtflsmtchngcrtnpttrn) 
-   [implement a tool for 'reviewing' tasks?](#mplmnttlfrrvwngtsks) [[org]]
-   [hmm wonder if possible to display org stuff on remarkable? at least reflect views? and exobrain?](#hmmwndrfpssbltdsplyrgstffnrmrkbltlstrflctvwsndxbrn) [[remarkable]] [[org]]
-   [org-agenda-later/earlier](#rggndltrrlr) [[drill]]
    -   [`[2020-06-10]` hmm, so it doesn't work from agenda, but kinda nice within the task?](#hmmstdsntwrkfrmgndbtkndncwthnthtsk) 
-   [`[2021-01-25]` org-fc didn't work straightaway](#rgfcddntwrkstrghtwy) [[srs]] [[orgmode]]





# related       [[pkm]] [[emacs]] [[orgparse]]




# organelle is quite good for a project name?      [[project]]




# oh for fucks sake it doesn't support <something.org#> anymore???      [[github]]

fuck maybe it just never worked???  
this "For instructions, see the special buffer howto." should be file link.. but not working here  
<https://web.archive.org/web/20190618202202/https://github.com/syl20bnr/spacemacs/blob/master/doc/DOCUMENTATION.org>  




# custom timestamp formats for specific file?

    -*- org-time-stamp-custom-formats: ("<%Y-%m-%d>" . "<%Y%m%d>") -*-

use with 'org-toggle-time-stamp-overlays?'  




# make ,s to "refile to the same file"? i.e. "sink"




# refile with inherited tags

-   State "STRT"      from "TODO"       `[2019-02-16]`




## `[2019-02-16]` <https://lists.gnu.org/archive/html//emacs-orgmode/2009-04/msg00149.html> eh, not very helpful.. looks like it's not there

<https://lists.gnu.org/archive/html/emacs-orgmode/2009-04/msg00133.html>  




# Really need to auto save on some operations? E.g. refile




# `[2019-10-07]` outline sections [Weekly /r/Orgmode Open Discussion - October 04, 2019](https://reddit.com/r/orgmode/comments/dd6wr5/weekly_rorgmode_open_discussion_october_04_2019/f2v6be3/) /r/orgmode      [[blog]]

No &#x2026; But workarounds exist &#x2026; <https://orgmode.org/worg/org-faq.html#closing-outline-sections>  




# `[2018-10-27]` Fast refiling in org-mode with hydras | Josh Moller-Mara <https://mollermara.com/blog/Fast-refiling-in-org-mode-with-hydras/>




# Map unschedule to capital u?




# fucking hell helm tag completion is annyoing      [[emacs]]

perhaps has to do with this&#x2026; <https://emacs.stackexchange.com/questions/32473/edit-org-mode-tags-using-ido-or-ivy-completion>  




# `[2019-10-01]` alphapapa/org-sidebar: A helpful sidebar for Org mode

<https://github.com/alphapapa/org-sidebar>  




## `[2019-10-06]` ok, interesting but not sure how it would be useful for me?




## `[2020-12-06]` org-sidebar-backlinks looks good? maybe  use a sidebar with all todo items summary

need to setup a hook though to refresh it on buffer switch  




# `[2019-10-05]` Is it possible to clear src results in org-mode? - Emacs Stack Exchange

<https://emacs.stackexchange.com/questions/35537/is-it-possible-to-clear-src-results-in-org-mode>  

    Option 2 - Use :results replace drawer




# use two different refiles: one file level, another heading level; use heading refile more often




# refresh agenda after doing actions on it, right now completed future tasks still appear on agenda

CREATED: `[2018-01-23]`  




# org-refile: make case insensitive




# check out more defaul org-evil-agenda bindings      [[doom]]




# `[2020-01-10]` [Amazing library for org hackers](https://reddit.com/r/emacs/comments/emran7/amazing_library_for_org_hackers/) /r/emacs

<https://github.com/ndwarshuis/om.el>  




# `[2020-02-16]` alphapapa/org-ql: An Org-mode query language, including search commands and saved views

<https://github.com/alphapapa/org-ql#helm-org-ql>  

    helm-org-ql
    Note: This command uses non-sexp queries.




# Github orgmode handling





## `[2019-07-30]` novoid/github-orgmode-tests: This is a test project where you can explore how github interprets Org-mode files

<https://github.com/novoid/github-orgmode-tests>  




## for fucks sake <https://github.com/wallyqs/org-ruby/issues/45>




## named +result heading seems to be broken&#x2026;





### `[2020-02-26]` ah, maybe it's fine.. just needs :exports results?




### `[2020-03-17]` yeah, it's org-ruby and it's `#+results:` thing that's breaking it&#x2026;




### `[2020-05-10]` right. apparently preempting with newline and using a drawe allows not to remove it?

see hpi/doc/MODULES.org  




### `[2020-07-15]` right. apparently, :results scalar wraps it in begin<sub>example</sub> and also works? see kobuddy




## ugh, seems that #+result drawer fails to render?

like in arctee  

    #+begin_src sh :results output replace :exports output
    ./arctee.py --help
    #+end_src
    
    #+RESULTS:
    #+begin_example




## caveat: github doesn't respect your custom ids      [[transclusion]] [[github]] [[org]]

e.g. it's generating "How do you use it?" -> how-do-you-use-it  




# search for completed tasks that have todo subtasks?




# perhaps need to filter some files for org-ql search

e.g. files without tags like twitter.org. Maybe the easiest to make them .txt actually??  




# autorefresh agenda?

<https://github.com/m-cat/org-recur#recommended-org-mode-settings>  

    (defun org-agenda-refresh ()
      "Refresh all `org-agenda' buffers."
      (dolist (buffer (buffer-list))
        (with-current-buffer buffer
          (when (derived-mode-p 'org-agenda-mode)
            (org-agenda-maybe-redo)))))




# hide drill from agenda




# `[2019-10-26]` Code blocks - Org Babel reference card      [[blog]]

<https://org-babel.readthedocs.io/en/latest/eval/>  

    You can define a code block somewhere and then call it explicitly elsewhere — provided the code block has a #+name: meta data to label it.




# `[2020-02-06]` Introducing Org Roam - Jethro Kuan

<https://blog.jethro.dev/posts/introducing_org_roam/>  




# inline tasks tips





## `[2019-10-04]` [Weekly /r/Orgmode Open Discussion - October 04, 2019](https://reddit.com/r/orgmode/comments/dd6wr5/weekly_rorgmode_open_discussion_october_04_2019/f2evhwh/) /r/orgmode

    Here's another discussion [https://stackoverflow.com/questions/11718401/how-to-use-todo-tags-in-org-mode-without-defining-headings](https://stackoverflow.com/questions/11718401/how-to-use-todo-tags-in-org-mode-without-defining-headings)




## `[2019-10-04]` [Weekly /r/Orgmode Open Discussion - October 04, 2019](https://reddit.com/r/orgmode/comments/dd6wr5/weekly_rorgmode_open_discussion_october_04_2019/f2ektrl/) /r/orgmode

    There's no way to do that, and it would probably be very messy to implement.  But try "inline tasks."




## `[2019-10-04]` [Weekly /r/Orgmode Open Discussion - October 04, 2019](https://reddit.com/r/orgmode/comments/dd6wr5/weekly_rorgmode_open_discussion_october_04_2019/f2eiggk/) /r/orgmode

     While it is not a solution, i use checkboxes i these kind of situations. Another workaround could be to create a checklist underneath the top heading and link to the subheadings.
    
     ```
     * FooBar
    
     Some text
    
     - foo
     - [ ] [[*bar][bar]]
    
     Some more text
    
     ** foo
     ** TODO bar
     SCHEDULED ...
    ```




## `[2019-12-17]` [Annotating everything: overview of Linux/Android tools for active reading](https://reddit.com/r/opensource/comments/cazgsa/annotating_everything_overview_of_linuxandroid/fb7p2w7/) /r/opensource

    > One big drawback with Org mode (and I believe most of outline/task list formats) though is that if you insert child outline items in the middle of text, it would structurally break it in two parts, so you'd have to append > your commend to the end of current outline (which can be potentially very long). On the other hand, plain list items, which you can insert in arbitrary place, are very limited and don't support most of things outline support like tags, timestamps, priorities etc.
    
    FYI, org mode has inline tasks (org-inlinetask.el)




# not sure if need to use org-id-track-globally???




# think of better hotkeys for agenda deadline and schedule settings




# shortcut to insert org style date in arbitrary place      [[emacs]]





## `[2020-06-03]` ugh! desperately need insert-date things

perhaps it should be smart and add whitespace (move point too)  




## `[2020-06-09]` use my/now C-t? maybe alt-t is better or something      [[habit]]




# `[2019-03-29]` org mode - Update the org-agenda-daily-view automatically on background - Emacs Stack Exchange

<https://emacs.stackexchange.com/questions/47254/update-the-org-agenda-daily-view-automatically-on-background>  

    (run-with-idle-timer 300 t (lambda () (org-agenda nil "a")) )




# `[2019-05-12]` Org-mode Hidden Gems - 01 Document Structure

<https://yiufung.net/post/org-mode-hidden-gems-pt1/>  

    And I only learn the existence of Description list today. Writing:
    
    - Emacs :: An extensible, customizable, free/libre text editor
    - Org mode :: Keeping notes, maintaining TODO lists, planning projects, and
      authoring documents with a fast and effective plain-text system




# `[2020-02-27]` wow, highlighting broken file links is very cool      [[doom]]




# `[2020-01-28]` [WIP: org-ql-view dispatch popup (like Magit)](https://reddit.com/r/orgmode/comments/ev28kw/wip_orgqlview_dispatch_popup_like_magit/) /r/orgmode      [[orgql]]





## `[2020-12-06]` oh wow it's super neat! interactive old-dispatch




# `[2019-10-26]` m-cat/org-recur: Recurring org-mode tasks

<https://github.com/m-cat/org-recur>  

    This package extends org-mode and org-agenda with support for defining recurring tasks and easily scheduling them.




## `[2020-06-10]` ugh. |3| didn't work, regardless org-recur-mode or org-recur-agenda-mode&#x2026;




# `[2019-11-02]` Org mode for meeting minutes      [[blog]]

<https://lists.gnu.org/archive/html/emacs-orgmode/2019-10/msg00300.html>  

    *** Reports from the sub teams

hmm, inline tasks could actually work ok&#x2026; could even hack them in export?  




# add repeat frequency?




# Org agenda bulk reschedule? Via transient mode??





## `[2019-11-02]` mm, ok, I gues 1-7 keys do this well




# use org-agenda-open-link, set up def browser




# hmm, unclear how to emulate RTM behavior with creating new task in regular time periods..

if I set scheduled=deadline, and then postpone via updating schdule, it doesn't really seem to work as expected :(  
so, I could set recurring deadline (with ++ cookie?) and use scheduled. Also hide deadline entries which are before scheduled date for recurring tasks  
WIP in ~/deadline.el  
hmm, wondering what happens to deadline when task completes?  
display as 'postponed'? also for repeating tasks only  
ok I need + cookie ,it's basically 'every'  
ok, nice, when i complete the task, 'scheduled' goes away automatically  
<http://karl-voit.at/2017/01/15/org-clone-subtree-with-time-shift/>  
Mm. Cloning subtree with time shift is ok, but that doesn't help with timestamps like 'first day of month'  

hmm, maybe just mark task as DND (do not delete) in the heading  




# priority in agenda works in a weird way&#x2026; make sure it jumps at a heading, not body





## `[2020-06-09]` eh? I think it was referring to the priority changing? was resolved probably?




# `[2019-02-15]` The Org Manual: Speed keys

<https://orgmode.org/manual/Speed-keys.html>  




# evil-collection?       [[vim]]




# :results replace raw appends instead of replacing

works as expected without raw though..  




# use evil-org (subtree manipulation)




# symlink projects with issues?




# have a suggestion for begin<sub>xxx</sub> thing to take in html classes?




# if it's got pin tag, always keep it on the very top? and don't reorder?




# maybe need a 'virtual'  "moving notes" mode for orgmode?      [[think]]

e.g. in edit mode, alt + hjkl is operating on the structure and can't change the text?  




# `[2019-10-11]` [Weekly /r/Orgmode Open Discussion - October 11, 2019](https://reddit.com/r/orgmode/comments/dgeojs/weekly_rorgmode_open_discussion_october_11_2019/f3dfy7n/) /r/orgmode      [[performance]]

    Several megabytes.  I think the slowest thing in my Org config is activating `org-bullets-mode` and `org-indent-mode`, which only happens when a file is first opened.
    What kind of stutters are you getting, i.e. when do they happen?  You might just need to make a few adjustments to your config.
    > I need to work on refiling to locations based on property values some time.
    `org-ql` can help with that.  For example, if you had a function to refile an entry by its property, you could do something like:
    
        (org-ql "refile.org"
          '(property "refile-property")
          :action #'nick/refile-by-property)




# attempt to display org-ql results in a window      [[orgql]]

should be in org-ql-view&#x2013;display? pop-to-buffer line  

there is bunch of functions in widnow.el (e.g. display-buffer-in-atom-window),  
but couldn't force it  




# `[2020-05-06]` [(1) EmacsConf 2019 - 05 - Use Org mode when away from the desktop - Zen Monk Alain M. Lafon - YouTube](https://www.youtube.com/watch?v=jEJC-9iUXY8&list=PLomc4HLgvuCWuJVVwsT8pbLWYR-n3G8bH&index=4)      [[blog]]

go through slides, it explains well history why how and what for he's using orgmode  




# clipping/capturing images

via some browser extension? the most important thing is to hash the contents (probably add to the name to make it unique)  
then easy to locate with org-mode  




# figure out pro and cons lists





## `[2018-06-20]` PRO and CON lists

TLDR: just use + PRO, + CON and then use the post-export-hook  
<https://lists.gnu.org/archive/html/emacs-orgmode/2010-04/msg00248.html>  




# need 'save all'&#x2026; or autosave on refile?      [[emacs]]




# `[2018-08-25]` need feedback for org-mode web app - view/search org files from Dropbox on web : orgmode

<https://www.reddit.com/r/orgmode/comments/9522eg/need_feedback_for_orgmode_web_app_viewsearch_org/>  

mm, not sure how far he made it&#x2026;  




## `[2019-01-13]` <https://www.reddit.com/r/orgmode/comments/9522eg/need_feedback_for_orgmode_web_app_viewsearch_org/>

<https://orgmodeweb.org/>  

it looks sort of ok, but still bugs in the interface. note sure if better than nuage?  




## `[2019-03-27]` looks broken :(




## `[2019-05-30]` still no updates&#x2026;




# how to separate or archive org state history?




# agenda: for sorting, need global list of all scheduled/deadline items sorted by priority




# do not detect timestamp as cloze? is that even possible?      [[orgdrill]]




# `[2019-02-10]` profiler - How do I speed up org-mode agenda generation - Emacs Stack Exchange

<https://emacs.stackexchange.com/questions/804/how-do-i-speed-up-org-mode-agenda-generation>  

    I've created this workaround, which pregenerates an agenda buffer whenever Emacs is idle for more than 5 seconds. The next time the agenda command is run, generation takes less than a second, since the org buffers have already been loaded.
    
    (run-with-idle-timer 5 nil (lambda () (org-agenda-list) (delete-window)))




# sort by tag for quick regrouping?




# support time with seconds precision?      [[setup]]





## `[2019-06-23]` <https://stackoverflow.com/a/25668739/706389> Take note that it's defined as a constant, so you're not encouraged to fiddle with it (but you still can:).




# helm-org-refile is a bit stupid; e.g. try refiling to 'watch'




# `[2019-10-23]` [O] noweb strip-export

<https://www.mail-archive.com/emacs-orgmode@gnu.org/msg123779.html>  

    Aloha all,
    The noweb strip-export setting leaves empty lines in the export.




# could potentially be convenient for org mode exports?      [[mimemacs]]




# `[2019-10-05]` emacs - Inline code in org-mode - Stack Overflow

<https://stackoverflow.com/questions/16186843/inline-code-in-org-mode>  

    While monospaced is good enough for most cases, inline code blocks have the form src_LANG[headers]{your code}. For example, src_xml[:exports code]{<tag>text</tag>}.
    
    Edit: Code highlighting of inline code is certainly possible, albeit with patching org.el itself: The answer given here https://stackoverflow.com/a/20652913/594138 works as advertised, turning
    
    - Inline code src_sh[:exports code]{echo -e "test"}




# `[2019-10-26]` Code blocks - Org Babel reference card      [[blog]]

<https://org-babel.readthedocs.io/en/latest/eval/>  

    Syntax
    #+call: is for standalone lines: it lives on a block by itself.
    A #+call: line can be named, in order for its results (for the arguments used) to be referenced.
    It has the following syntax, where each header argument portion is optional.
    #+name: <CALL-LINE-NAME>
    #+call: <NAME>[<HEADER-ARGS-FOR-BLOCK>](<ARGUMENTS>) <HEADER-ARGS-FOR-CALL-LINE>




# org-next-visible-heading hotkey?      [[setup]]




# `[2020-01-10]` ndwarshuis/om.el: A functional library for org-mode

<https://github.com/ndwarshuis/om.el>  

    A functional API for org-mode inspired by @magnars's dash.el and s.el libraries.




# `[2020-05-03]` [A Featureful Blog made with Emacs Org-mode : emacs](https://www.reddit.com/r/emacs/comments/gckuv2/a_featureful_blog_made_with_emacs_orgmode/)




# `[2020-11-24]` [landakram/org-z: Lightweight, Org-mode flavored zettelkasten links.](https://github.com/landakram/org-z)




# `[2020-06-09]` my/org-sort-entries &#x2013; actually it's good it's keeping stable sort for same prios

that way I can refile to the end of the same file and it will sink item to the bottom  




# make ,s to "refile to the same file"? i.e. "sink"




# try org-sort?




# `[2020-10-09]` [Org Syntax (draft)](https://orgmode.org/worg/dev/org-syntax.html)




# function to 'sink' a heading down till the next priority.. might be unstable though

maybe just sink the current entry (alt-down), then it'd be automatic  




# org-ql-search change view format

apparently this function, but not configurable at the moment?  

    (defun org-ql-view--format-element (element)




# `[2019-10-31]` [DONE tasks with different color](https://reddit.com/r/orgmode/comments/dpk84w/done_tasks_with_different_color/f5w05hh/) /r/orgmode

    Setting `org-fontify-done-headline` to `t` will (in most themes) make any DONE heading grey. The `leuven` theme also makes the heading ~~strikethrough~~.




# `[2019-11-14]` Python Source Code Blocks in Org Mode

<https://orgmode.org/worg/org-contrib/babel/languages/ob-doc-python.html>  

    Org Mode supports graphical output for LaTeX and HTML documents using Matplotlib.




# I think resume doesn't work when you do org-drill-habits      [[orgdrill]]




# `[2020-04-26]` [toshism/org-super-links: Package to create links with auto backlinks](https://github.com/toshism/org-super-links)

    Package to create links with auto backlinks




# `[2019-10-30]` [Weekly tips/trick/etc/ thread](https://reddit.com/r/emacs/comments/domrl6/weekly_tipstricketc_thread/f5thc8l/) /r/emacs

    Cool, I didn't know about `imenu-add-menubar-index`.
    You may also find `org-sidebar-tree` helpful: https://github.com/alphapapa/org-sidebar




# Introduction to "organice" - Using Org mode from a smartphone or browser | Lobsters

<https://lobste.rs/s/jjcwou/introduction_organice_using_org_mode>  




# right, export is weird when output contains \* heading?




# disable org-indent-mode??      [[doom]]




# set org-directory just in case? also good for relative path to capture templates

also org-default-notes-files for capture without file argument  




# clipping images

via some browser extension? the most important thing is to hash the contents (probably add to the name to make it unique)  
then easy to locate with org-mode  




# `[2019-12-26]` The Org Manual: Literal examples

<https://orgmode.org/manual/Literal-examples.html>  

    For simplicity when using small examples, you can also start the example lines with a colon followed by a space. There may also be additional whitespace before the colon:

Here is an example  

    Some example from a text file.




# postpone with a small exponent? not sure




# org-agenda-filter-by-tag (then - to exclude at TAB to select tag) is very nice for ad-hoc switching?      [[habit]]




# paranoid mode: check for broken headings      [[setup]]

could prob improve, e.g. detect actual stars?  

    rg '..............................*#(A|B|C|D)]'




# `[2020-11-14]` [Who needs GitHub to manage a project when you have Emacs and Org](https://reddit.com/r/emacs/comments/jtydiy/who_needs_github_to_manage_a_project_when_you/) /r/emacs





## `[2020-12-11]` tab-bar-mode and global-tab-line-mode ?




# `[2020-06-07]` [Orgro: an org-mode viewer for mobile](https://reddit.com/r/emacs/comments/gybdbq/orgro_an_orgmode_viewer_for_mobile/) /r/emacs





## `[2020-10-24]` waiting for fdroid <https://github.com/amake/orgro/issues/15>




# `[2020-12-17]` [UOMF: Using Org Mode Categories Versus Tags](https://karl-voit.at/2019/09/25/categories-versus-tags/)      [[habit]]

    So if you press < when being on a line whose task is categorized with "ProjectY", your agenda now only shows tasks of this category, hiding everything else.




# use ,. for refiling to current file      [[habit]]




# have a repository of org-mode demo files? generate it w.r.t to today so it's easy to demonstrate? org could hack current day somehow, but that could be tricky




# file variables

<http://home.fnal.gov/~neilsen/notebook/orgExamples/org-examples.html>  

    Follow the instructions in the emacs manual; begin the file with a line of the form:

    # -*- foo: "bar"; baz: "ham" -*-
    For example, to set the "Up" and "Home" links for an org-mode file, begin it with:
    # -*- org-html-link-up: "http://decam03.fnal.gov:8080/notes/neilsen/";  org-html-link-home: "http://home.fnal.gov/~neilsen" -*-

<https://www.gnu.org/software/emacs/manual/html_node/emacs/Specifying-File-Variables.html#Specifying-File-Variables>  




# archive entries (org-archive-subtree)




# archive tag to hide subtree (org-toggle-archive-tag)




# repeat interval cookies

-   `.+` &#x2013; always + today
-   `++` &#x2013; will always move into the future
-   `+`  &#x2013;  will move exactly x days w.r.t. to deadline date




# agenda sometimes takes A LOT of time to rerender. I think we need an inotify async server&#x2026;




# go thought archives occasionally to check for accidentally archived? Then mark




# tagging files, then org view into them




# `[2020-04-12]` [Literal Examples (The Org Manual)](https://orgmode.org/manual/Literal-Examples.html)

    There is one limitation, however. You must insert a comma right before lines starting with either ‘*’, ‘,*’, ‘#+’ or ‘,#+’, as those may be interpreted as outlines nodes or some other special syntax. Org transparently strips these additional commas whenever it accesses the contents of the block.




# habits/drill should probably have importance? So the unimportant things are showed less frequently      [[spacedrep]]




# for drill, only consider stuff that isn't done?

or cancelled  

    (defcustom org-drill-match
      nil
      "If non-nil, a string specifying a tags/property/TODO query. During
    drill sessions, only items that match this query will be considered."
      :group 'org-drill




# check for corrupted headings, typically it's stars and todo states out of nowhere




# `[2019-10-05]` Re: [O] Bug: spurious newline after comment

<https://lists.gnu.org/archive/html/emacs-orgmode/2016-08/msg00276.html>  

    
    Note that you can
    - use somewhat inline comments with @@comment:...@@ syntax
    - remove commented lines the way you like using a hook:
      `org-export-before-processing-hook'.




# `[2019-09-22]` alphapapa/org-super-agenda: Supercharge your Org daily/weekly agenda by grouping items

<https://github.com/alphapapa/org-super-agenda>  

    If you want to install manually, you must also install these packages:
        Emacs >= 26.1
        dash >= 2.13
        ht >=2.2
        org-mode >= 9.0
        s >= 1.10
        ts




# weirdness with encoding in Polar documents      [[polar]] [[org]] [[emacs]]

-   could set header to # -**- coding: utf-8 -**- ? not sure
-   revert-buffer-with-coding-system
-   mine should be utf8  
    
        (prefer-coding-system 'utf-8)            ; pretty
        (setq locale-coding-system 'utf-8)       ; please




# `[2019-10-22]` [Rethink: Org mode meets professional web design](https://reddit.com/r/emacs/comments/dllhr7/rethink_org_mode_meets_professional_web_design/) /r/emacs      [[org]]

    Hi all,
    I recently posted a link on here about an org mode export template called [Imagine](https://jessekelly881-imagine.surge.sh/). I have been working on a new(and I believe much better) template recently called [Rethink](https://jessekelly881-rethink.surge.sh/). Yes, I know the name isn't the best.
    So far they are just works in progress but I plan to create a smallish collection. I started this because I was looking for good css templates targeted at org mode and I was disappointed by the severe lack of them. Hopefully, someone will find these useful. Again, they are still wip but maybe with a little help from some helpful web designer we can make them much better.
    Also, if you find any bugs or things you wish were different feel free to comment or contact me on [Github](https://github.com/jessekelly881). Thanks!




# refile is weird in terms of fuzzy matching (log.org)      [[emacs]] [[org]]

completing-read apparently?  
see  
org-refile-get-location  

completing-read-function?  

helm&#x2013;completing-read-default  

(defclass helm-source-async (helm-source)  

shit.. has something to do with async sources?&#x2026; spacemace//helm-make-source  

huh.. fixed it via making that&#x2026;  

(add-to-list 'helm-completing-read-handlers-alist '(org-refile . helm-completing-read-sync-default-handler))  




## maybe contribute to spacemacs?? not sure why the source was async in the first place&#x2026;




# `[2018-06-10]` fniessen/org-html-themes: How to export Org mode files into awesome HTML in 2 minutes      [[org]] [[blog]]

<https://github.com/fniessen/org-html-themes>  




## `[2018-10-28]`  eh, not so sure about it. doesn't look nice




# shit, I need agda-like unicode input      [[org]] [[emacs]] [[math]] [[study]]

-   State "DONE"       from "START"      `[2019-02-16]`
-   State "START"      from "TODO"       `[2019-02-16]`




# `[2019-10-27]` org babel - How to automatically tangle another source block to file when evaluate a source block in org-mode? - Emacs Stack Exchange

<https://emacs.stackexchange.com/questions/14153/how-to-automatically-tangle-another-source-block-to-file-when-evaluate-a-source>  




# org-clock is oddly satisfying      [[org]]




# add CREATED to entry (add-created would be enough)      [[emacs]] [[org]]




# figure out how to find and jump a file      [[org]]

CREATED: `[2018-01-24]`  
<http://kitchingroup.cheme.cmu.edu/blog/2016/11/04/New-link-features-in-org-9/>  




# `[2017-12-23]` custom timestamp format      [[org]]

<https://emacs.stackexchange.com/questions/3179/how-to-make-org-mode-dwim-when-it-reads-times-in-timestamps>  




# do not count timestamps as cloze      [[emacs]] [[orgdrill]]




# Org mode exporting to html

<https://www.reddit.com/r/orgmode/comments/c6kc5r/org_mode_exporting_to_html/>  




# display links as raw links      [[emacs]] [[org]]





## `[2019-11-02]` eh?




# `[2019-07-29]` sort by property TAGS      [[org]]




# `[2019-10-23]` The Org Manual: Extracting source code

<https://orgmode.org/manual/Extracting-source-code.html>  

    14.4 Extracting source code
    
    Extracting source code from code blocks is a basic task in literate programming.




# `[2019-10-05]` The Org Manual: Structure of code blocks

<https://orgmode.org/manual/Structure-of-code-blocks.html>  

    An inline code block conforms to this structure:
    src_<language>{<body>}
    or
    src_<language>[<header arguments>]{<body>}




# selecting drill items org-drill-entry-p      [[org]]

looks only by tag&#x2026;  




# two kinds of refiles? one with headings, one without?      [[emacs]]




# the 'notes' marker doesn't work as expected? only shows subtasks      [[emacs]]




# do not make org todo state change pop up as a new window      [[emacs]]




# Exclude done/cancelled from drill?      [[emacs]]




# `[2019-12-10]` The Org Manual      [[blog]]

<https://www.gnu.org/software/emacs/manual/html_mono/org.html>  

    BEGIN_aside
    Lorem ipsum
    END_aside




# Large life-logging org-mode file gets too slow

<https://www.reddit.com/r/orgmode/comments/arg7fk/_/>  




# Org-mode Hidden Gems - 03 Hyperlinks

<https://yiufung.net/post/org-mode-hidden-gems-pt3/>  

Ok looks this guy posted several posts and everyone is fine with that  




# org archive &#x2013; check for not TODOs?      [[emacs]]





## `[2019-11-02]` eh?




# wonder if this was causing issues for me in test.org ?      [[doom]]

    ;; Allow inline image previews of http(s)? urls or data uris
    (org-link-set-parameters "http"  :image-data-fun #'+org-image-link)
    (org-link-set-parameters "https" :image-data-fun #'+org-image-link)
    (org-link-set-parameters "img"   :image-data-fun #'+org-inline-data-image)




# how to refresh agenda in the background? so it reflects changes in files instantly without saving      [[emacs]]




# `[2020-09-22]` [When refiling: Invalid function: org-preserve-local-variables · Issue #1116 · hlissner/doom-emacs](https://github.com/hlissner/doom-emacs/issues/1116)

    ~/.emacs.d/.local/straight/build/org-mode/*.elc




# shit, looks my coefficient makes 3,4,5 pretty much irrelevant      [[spacedrep]] [[orgdrill]]

or maybe, it's fine?  




# hotkey to sort entries by created date      [[emacs]]

-   State "DONE"       from "TODO"       `[2019-02-16]`

org-sort-entries?  
don't need it as often&#x2026;  




# some items should not contribute to global agenda. e.g. subtasks of an item      [[org]] [[gtd]]




# send push on org capture change, sync on android?      [[org]] [[android]]

hmm, maybe disassemble dropsync to hack update frequency via automate on wifi?  




# eh, perhaps I need some automated tool to interact with org mode and move around the items? although clog is kind of ok&#x2026;      [[org]]




# automatic watch later, deduced by tag, sync with youtube playlist      [[org]]




# use org-mode for docs? also make sure to keep old commit link as example of using ipython for literate docs      [[cachew]] [[literate]] [[jupyter]]




# `[2019-10-26]` EmacsConf 2019 - Schedule      [[towatch]]

<https://emacsconf.org/2019/schedule>  

    Managing your life with org-mode and other tools
    Marcin Swieczkowski




# `[2019-12-04]` Org mode for Emacs – Release notes      [[org]]

<https://orgmode.org/Changes.html>  

    New link-type: Attachment




# `[2019-10-19]` org-emms - MELPA      [[org]] [[annotation]]

<https://melpa.org/#/org-emms>  
interesting, could use for annotating?  




# `[2019-09-25]` Blog Series: Using Org Mode Features (UOMF)      [[org]]

<https://karl-voit.at/2019/09/25/using-orgmode/>  

    Using many or few Org mode files
    Agenda filters
    Finding stuff within Org mode
    Update on contact management




# `[2020-02-13]` alphapapa/org-almanac: Almanac for Org mode      [[org]]

<https://github.com/alphapapa/org-almanac>  
how are people using org-mode  




# `[2019-11-15]` alphapapa/org-protocol-capture-html: Capture HTML from the browser selection into Emacs as org-mode content      [[org]] [[capture]]

<https://github.com/alphapapa/org-protocol-capture-html>  




# `[2021-01-04]` ~ vs = : the former preserves underscores? so better to use it?      [[org]]




# `[2019-07-20]` Org-mode Frequently Asked Questions      [[org]]

<https://orgmode.org/worg/org-faq.html#closing-outline-sections>  
The short answer to the question is no. Org-mode adheres to the cascading logic of outlines, in which a section is closed only by another section that occupies an equal or greater level.  




# `[2020-01-28]` [Some org-mode features you may not know](https://reddit.com/r/orgmode/comments/ev5ox4/some_orgmode_features_you_may_not_know/) /r/orgmode

-   `[2020-03-21]` cool, but personally haven't found them useful




# `[2019-10-06]` Emacs Org-mode - a system for note-taking and project planning - YouTube

<https://www.youtube.com/watch?v=oJTwQvgfgMM&list=WL&index=35&t=4s>  
eh, pretty intro level  
Don't think I need to watch org-mode demos anymore, really&#x2026;  




# `[2019-09-05]` hmm, actually org-brain is pretty keyboard oriented. not sure how good is it in visualising stuff&#x2026;




# `[2019-09-05]` orgbrain: ok, it was somewhat interesting, but not sure if I it's visual enough&#x2026;




# `[2018-07-24]` Kungsgeten/org-brain: Org-mode wiki + concept-mapping      [[pkm]]

<https://github.com/Kungsgeten/org-brain>  
mm, the brain looks very GUI and mouse demanding. org is def. better for me  




# `[2018-07-24]` Civilizer - Cleverly manage your data/knowledge/idea      [[pkm]]

<https://suewonjp.github.io/civilizer/>  
meh, looks very basic, is not backed by plaintext, not very googlable&#x2026;  




# `[2019-01-17]` BuboFlash - helps with learning      [[pkm]] [[spacedrep]]

<https://buboflash.eu/bubo5/log-in?called-from=/bubo5/homepage>  
mm, interesting thing, for web annotation. not sure if I want to use it?  




# `[2021-01-20]` ugh. need some sanity checker for broken outlines      [[org]]

some false positives, but kind of ok  

    rg  '[^^*]\*+ .*(\[#.\]|:\s*$)'




# `[2021-01-01]` [viebel/klipse: Klipse is a Javacript plugin for embedding interactive code snippets in tech blogs. A simple client-side code evaluator pluggable on any web page: clojure, ruby, javascript, python, scheme, es2017, jsx, brainfuck, c++, reagent, lua, ocaml, reasonml, prolog, common lisp](https://github.com/viebel/klipse)      [[org]] [[literate]]

hhmm html export has klipse css properties??  




# `[2021-01-16]` [emacs - How to use the function option of org-capture correctly? - Stack Overflow](https://stackoverflow.com/questions/56274067/how-to-use-the-function-option-of-org-capture-correctly/58395117#58395117)

capturing via a function to prompt for the target file  




# `[2020-12-28]` [Advanced Export Configuration (The Org Manual)](https://orgmode.org/manual/Advanced-Export-Configuration.html)

    Defining filters for individual files
    The Org export can filter not just for back-ends, but also for specific files through the ‘BIND’ keyword. Here is an example with two filters; one removes brackets from time stamps, and the other removes strike-through text. The filter functions are defined in a code block in the same Org file, which is a handy location for debugging.

whoa  




# `[2019-05-18]` [Weekly /r/Orgmode Open Discussion - May 10, 2019](https://reddit.com/r/orgmode/comments/bmxvlv/weekly_rorgmode_open_discussion_may_10_2019/en3uler/) /r/orgmode      [[toblog]] [[publish]]

    I would really like to see a book written on org mode taking someone from nothing to having their whole life organised by org mode. The manual is good to find out how stuff works but you kinda need to know what you want to do beforehand. It would be great if something could also show you what is possible, stuff I wouldn't have even thought of...




# name: "You need more Org in your life" or something?      [[org]]




# refile was hard to appreciate until I got used to navigating among multiple files and using several files as org agenda sources      [[toblog]] [[org]]




# motivation for collecting agenda files by myself: emacs is slow and buggy      [[blog]] [[org]]

e.g. agenda tries to include lock files!  




## `[2021-01-24]` not sure what I meant there?




# Mention that it's very easy to get lost in org features      [[toblog]] [[pkm]] [[org]]





## `[2019-09-29]` could actually blog why is it org mode vs markdown vs yaml/whatever for me




# org-capture main motivation: it's immediately in my filesystem.      [[grasp]]

I don't need a dedicated day when I'm manually moving things from bookmarks  
If i add a 'drill' tag, it would be added to my spaced repetition queue immediately.  
It becomes plain text searchable immediately, at which point I can find it by vaguely remembering link title.  




# `[2019-10-08]` capture: often I'd put a quick tag if I expect myself to search for that outline later (e.g. if I need to buy something), or if it's some thought related to one of the projects I'm doing. If it's something I really need to remember I'd also schedule it.

Otherwise I try to spend as little time capturing TODO ??? I found premature organizing to be too time consuming and often distrupting thinking.  




# `[2019-10-08]` capture: I find it less distracting to keep logs (e.g. quantified self style, like sleep, exercise, weight etc) in a separate file.

TODO post about my automatic parsing and extraction?  




# (in post about capture)      [[grasp]]

It's pretty stupid, but such a conceptually simple tool is one of the most useful things I've developed  
It instantly ends up in my knowledge repository, immediately accesible by search, agenda etc  




# What’s awesome is that at the time of capture it immediately becomes searchable and indexable as any plaintext would without any extra effort (unlike if you added it to browser bookmarks/pinboard).      [[grasp]]




# `[2020-04-13]` <http://www.acuriousmix.com/2014/09/03/designing-a-personal-knowledgebase> motivation for fast capture there




# ask if it would be nice if org-mode supported inline tags?      [[outbox]] [[reddit]] [[org]]

although maybe easier to emulate with [[ links?  




# HTML<sub>CONTAINER</sub> property could be useful..      [[org]] [[exobrain]] [[blog]]




# looks like h is hardcoded here&#x2026;

    (format "\n<h%d id=\"%s\">%s</h%d>\n"
         level
         id




# `[2019-11-21]` Literate Theorem Proving with Org <https://chame.co/writeups/org_coq/post.html>




# Tecos config? Maintainer of org site      [[org]]

He's the maintainer for the org-mode website now so he knows whereof he speaks  




# use files as todos? have a crawler go through them and put in a special tasklist      [[org]]

e.g. if it contains TODO, enough already and maybe also parse tags (and timestamp?)  

-   not sure about scheduling it?
-   maybe use queue &#x2013; unique id (file hash?) need to be careful with empty files though
-   voit must have something




## @publicvoit@graz.social thought you'd be a kind of person who knows it &#x2013; is there some existing tool to crawl the filesystem and maintain an org-mode file with todos corresponding to files matching a certain pattern?

My usecase is that I often put TODO in screenshots of bugs, ideas for possible features etc; often on my phone so using [file:] links is not so convenient (+ I tend to move files around)  




# implement a tool for 'reviewing' tasks?      [[org]]

do in python  

-   go by priority/oldest created/etc
-   exclude some tags?
-   keep state (use some simple SR algo?)  
    just use hash of the heading? seems quite enough
-   jump to the file/line via mimemacs?




# hmm wonder if possible to display org stuff on remarkable? at least reflect views? and exobrain?      [[remarkable]] [[org]]




# org-agenda-later/earlier       [[drill]]

Org-add-note  




## `[2020-06-10]` hmm, so it doesn't work from agenda, but kinda nice within the task?

note sure about logbook&#x2026;  




# `[2021-01-25]` org-fc didn't work straightaway      [[srs]] [[orgmode]]

