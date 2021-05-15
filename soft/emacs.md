
# Table of Contents

-   [related](#rltd) [[elisp]]
-   [`[2019-12-23]` What feature of emacs you tried in 2019 and now you can't live without? /r/emacs](#srddtcmrmcscmmntsmbwhtftrcsytrdnndnwycntlvwthtrmcs) [[setup]]
    -   [`[2020-02-28]` hmm, what could I use direnv for?](#hmmwhtcldsdrnvfr) 
-   [`[2019-05-18]` Refactoring in Spacemacs using iedit and helm-edit /r/spacemacs](#srddtcmrspcmcscmmntsbnlgkspcmcssngdtndhlmdtrspcmcs) 
-   [`[2020-01-30]` deadgrep](#ddgrp) [[pkm]]
-   [dash.el (defmacro &#x2013;> (x &rest forms)](#dshldfmcrxrstfrms) [[elisp]]
-   [need to either exclude ipynb or somehow exclude binary strings](#ndtthrxcldpynbrsmhwxcldbnrystrngs) [[pkm]] [[search]]
    -   [`[2020-10-13]` ok, limit line width?](#klmtlnwdth) 
-   [need to hack on to prevent reordering etc I guess helm-rg&#x2013;helm-pattern-to-ripgrep-regexp](#ndthckntprvntrrdrngtcgsshlmrghlmpttrntrpgrprgxp) 
-   [`[2019-09-05]` Deft for Emacs](#dftfrmcs) 
-   [`[2019-12-26]` cask/cask: Project management tool for Emacs](#cskcskprjctmngmnttlfrmcs) 
-   [(setq graphviz-dot-preview-extension "svg")](#stqgrphvzdtprvwxtnsnsvg) 
-   [autorevert?](#trvrt) 
-   [learn to use ediff](#lrntsdff) [[habit]]
-   [use tramp hops](#strmphps) [[docker]] [[ssh]]
-   [disable evil last non blank](#dsblvllstnnblnk) 
-   [`[2018-12-26]` millejoh/emacs-ipython-notebook: Jupyter notebook client in Emacs](#mlljhmcspythnntbkjpytrntbkclntnmcs) 
-   [Tweet from ¬¬(Dan Piponi) (@sigfpe), at May 31, 22:14](#twtfrmdnppnsgfptmy) 
-   [ok, so important bits were adding subfolder project and switching in to 'extension'. Also, use error log buffer](#ksmprtntbtswrddngsbfldrprwtchngntxtnsnlssrrrlgbffr) [[setup]] [[lsp]]
-   [`[2019-09-01]` emacs-tw/awesome-emacs: A community driven list of useful Emacs packages, libraries and others.](#mcstwwsmmcscmmntydrvnlstfsflmcspckgslbrrsndthrs) 
-   [`[2019-09-02]` noctuid/evil-guide: Draft of a guide for using emacs with evil](#nctdvlgddrftfgdfrsngmcswthvl) 
-   [`[2019-07-30]` EmacsConf 2019 - Call for Proposals](#mcscnfcllfrprpsls) 
-   [`[2019-10-18]` EmacsConf 2019 Schedule /r/emacs](#srddtcmrmcscmmntsdjfhtmcscnfschdlmcscnfschdlrmcs) [[towatch]]
-   [ein is adding some metadata?? wtf?](#nsddngsmmtdtwtf) [[ipython]]
-   [output-type-preference](#tpttypprfrnc) [[ipython]]
    -   [that seems to have fixed some output issues](#thtsmsthvfxdsmtptsss) 
-   [use SPC \* similarly to \*](#sspcsmlrlyt) [[habit]]
-   [`[2019-12-23]` What feature of emacs you tried in 2019 and now you can't live without? /r/emacs](#srddtcmrmcscmmntsmbwhtftrcsytrdnndnwycntlvwthtrmcs) 
-   [`[2019-10-20]` Enabling helm-follow-mode on a per-command basis. · Issue 2006 · emacs-helm/helm](#nblnghlmfllwmdnprcmmndbssssmcshlmhlm) 
-   [`[2020-01-03]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration](#mtthwzmdmcsdmmcscstmzdfllftrdgnmcscnfgrtn) 
-   [`[2019-12-29]` Forge – Work with Git forges from the comfort of Magit | Hacker News](#frgwrkwthgtfrgsfrmthcmfrtfmgthckrnws) 
-   [emacs need something like check<sub>call</sub> in case rg is missing](#mcsndsmthnglkchckcllncsrgsmssng) [[elisp]]
-   [fucking hell. didn't manage to set up deadgrep](#fcknghllddntmngtstpddgrp) 
-   [https://github.com/alphapapa/link-hint.el](#sgthbcmlphpplnkhntl) 
-   [.emacs.d/local? not sure if need it under git](#mcsdlclntsrfndtndrgt) [[dotfiles]]
-   [andrewtropin кроме paredit, есть ещё любопытная штуковина parinfer: https://shaunlebron.github.io/parinfer/](#ndrwtrpnкромеprdtестьещёлинаprnfrsshnlbrngthbprnfr) [[elisp]] [[lisp]]
-   [`[2019-09-28]` eli-oat/pillow-fort.org: A literate emacs configuration](#ltpllwfrtrgltrtmcscnfgrtn) [[literate]]
-   [`[2019-09-07]` raxod502/el-patch: ✨ Future-proof your Emacs Lisp customizations!](#rxdlptchftrprfyrmcslspcstmztns) [[setup]]
-   [`[2019-11-03]` Ambrevar / emacs-gif-screencast · GitLab](#mbrvrmcsgfscrncstgtlb) 
-   [`[2019-11-08]` Whats your emacs setup like ? | Lobsters](#whtsyrmcsstplklbstrs) [[toblog]]
-   [Set up ipynb mode in emacs, display locals?](#stppynbmdnmcsdsplylcls) [[python]]
-   [implement search in filenames?](#mplmntsrchnflnms) [[pkm]]
-   [configure source location for builtin stuff](#cnfgrsrclctnfrbltnstff) 
-   [`[2020-01-03]` (Officially) Introducing M-EMACS ;) : emacs](#ffcllyntrdcngmmcsmcs) 
-   [pip3 install &#x2013;user "python-language-server[all]"](#ppnstllsrpythnlnggsrvrll) [[setup]]
-   [cl-typecase](#cltypcs) [[elisp]]
-   [use pp-eval-expression (SPC-;)](#sppvlxprssnspc) [[habit]]
-   [`[2020-02-28]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration](#mtthwzmdmcsdmmcscstmzdfllftrdgnmcscnfgrtn) 
-   [`[2020-02-28]` bbatsov/super-save: Save Emacs buffers when they lose focus](#bbtsvsprsvsvmcsbffrswhnthylsfcs) 
-   [`[2020-02-28]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration](#mtthwzmdmcsdmmcscstmzdfllftrdgnmcscnfgrtn) 
-   [hmmm](#hmmm) 
-   [setting up locate db&#x2026;](#sttngplctdb) 
-   [`[2020-04-12]` How do I prevent messages from showing in the minibuffer? · Issue 2878 · hlissner/doom-emacs](#hwdprvntmssgsfrmshwngnthmnbffrsshlssnrdmmcs) 
-   [`[2020-05-07]` EmacsWiki: Category Extension Language](#swwwmcswkrgmcsctgryxtnsnlnggmcswkctgryxtnsnlngg) 
-   [hmm maybe highlight closing parens less than opening? not sure](#hmmmybhghlghtclsngprnslssthnpnngntsr) [[elisp]]
-   [`[2020-02-28]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration](#mtthwzmdmcsdmmcscstmzdfllftrdgnmcscnfgrtn) 
-   [emacs &#x2013; leader key takes ridiculous time to process](#mcsldrkytksrdclstmtprcss) [[setup]]
-   [`[2020-01-10]` alphapapa/makem.sh: Makefile-like script for building and testing Emacs Lisp packages](#lphppmkmshmkfllkscrptfrbldngndtstngmcslsppckgs) 
-   [`[2020-02-24]` doom-emacs/api.org at develop · hlissner/doom-emacs](#dmmcsprgtdvlphlssnrdmmcs) [[doom]]
-   [`[2020-02-24]` doom-emacs/index.org at develop · hlissner/doom-emacs](#dmmcsndxrgtdvlphlssnrdmmcs) 
-   [`[2020-03-14]` manateelazycat/emacs-application-framework: Emacs application framework](#mntlzyctmcspplctnfrmwrkmcspplctnfrmwrk) 
-   [use alt-n for 'default' filename completion? useful to rename things quickly](#sltnfrdfltflnmcmpltnsfltrnmthngsqckly) [[emacs]] [[habit]]
-   [indicate if there are some unsaved changes?](#ndctfthrrsmnsvdchngs) 
    -   [`[2020-06-19]` maybe in title??](#mybnttl) 
-   [tramp hangs while sending password](#trmphngswhlsndngpsswrd) [[setup]]
-   [audio annotation?](#dnnttn) 
-   [agenda on F12 press? on constantly loaded emacs instance](#gndnfprssncnstntlylddmcsnstnc) [[setup]]
-   [Spacemacs ABC](#spcmcsbc) 
-   [traad for refactoring](#trdfrrfctrng) [[python]]
-   [`[2018-11-05]` alphapapa/org-ql: An Org query language, and experimental code for a next-generation Org Agenda](#lphpprgqlnrgqrylnggndxprmntlcdfrnxtgnrtnrggnd) 
-   [try skeletor](#tryskltr) 
-   [haskell ide engine thing](#hsklldngnthng) [[haskell]]
    -   [ok, so lsp-demote thing is no bound to any key. I might help with that?](#kslspdmtthngsnbndtnykymghthlpwththt) 
    -   [right! lsp-ui-sideline-apply-code-actions](#rghtlspsdlnpplycdctns) 
-   [helm stupid behaviour when trying to rename file](#hlmstpdbhvrwhntryngtrnmfl) 
-   [http://www.viemu.com/a-why-vi-vim.html](#wwwvmcmwhyvvmhtml) [[vim]]
-   [`[2019-09-04]` kunalb/poet: An emacs theme that's well suited for modes using variable pitch: particularly org-mode and markdown-mode.](#knlbptnmcsthmthtswllstdfrtchprtclrlyrgmdndmrkdwnmd) 
-   [(agda-input-add-translations '( ("pd" . "∂") ))](#gdnptddtrnsltnspd) 
-   [agda input](#gdnpt) 
-   [memoize &#x2013; if function returns nil (e.g. empty list, the value is always recomputed)](#mmzffnctnrtrnsnlgmptylstthvlslwysrcmptd) [[elisp]]
-   [`[2019-10-31]` camcorder.el - Creating Animated Gifs & Videos for Spacemacs | jr0cket](#cmcrdrlcrtngnmtdgfsvdsfrspcmcsjrckt) 
-   [`[2019-12-20]` belak/emacs-grayscale-theme](#blkmcsgrysclthm) 
-   [`[2019-12-20]` Whats your emacs setup like ? | Lobsters](#whtsyrmcsstplklbstrs) 
-   [ein evil mode :w](#nvlmdw) [[jupyter]]
-   [`[2018-11-06]` narendraj9/hledger-mode: An Emacs major mode for Hledger](#nrndrjhldgrmdnmcsmjrmdfrhldgr) 
-   [email?](#ml) 
-   [can use setf?](#cnsstf) [[elisp]]
-   [Tweet from @burntsushi5](#twtfrmbrntssh) 
-   [`[2020-01-03]` (Officially) Introducing M-EMACS ;) : emacs](#ffcllyntrdcngmmcsmcs) 
-   [helm-locate-library](#hlmlctlbrry) [[habit]]
-   [`[2020-05-01]` on the usability of editable software | Lobsters](#slbstrssqkpwpnsbltydtblsfrnthsbltyfdtblsftwrlbstrs) 
-   [Habits](#hbts) 
    -   [use org-created-to-inline {, c}](#srgcrtdtnlnc) [[habit]]
    -   [[SPC e l] error list](#spclrrrlst) 
    -   [it's fine to use C-c and C-v in insert mode](#tsfntsccndcvnnsrtmd) [[habit]]
    -   [{>aR} demote subtree](#rdmtsbtr) [[habit]] [[org]]
    -   [use SPC-t](#sspct) [[habit]] [[org]]
    -   [selecting class: {v close sqbracket open sqbracket}](#slctngclssvclssqbrcktpnsqbrckt) [[habit]]
    -   [use eshell more](#sshllmr) [[habit]]
    -   [use SPC S c and SPC s i to search code and info](#sspcscndspcstsrchcdndnf) [[habit]]
    -   [Use magit more, many people claim its superior to cli](#smgtmrmnypplclmtssprrtcl) [[habit]] [[git]]
    -   [use 'light'](#slght) [[habit]]
    -   [use SPC p P](#sspcpp) [[habit]]
    -   [Use prj: to link to file in the same project](#sprjtlnktflnthsmprjct) [[habit]]
    -   [Use tramp](#strmp) [[oldhabit]]
    -   [use helm-resume SPC h l to resume search](#shlmrsmspchltrsmsrch) [[habit]]
    -   [use eshell:](#sshll) [[habit]]
    -   [use X to delete](#sxtdlt) [[habit]]
    -   [use # and T](#sndt) [[habit]]
    -   [use C-g to interrupt stuck commands](#scgtntrrptstckcmmnds) [[habit]]
    -   [J for joining lines](#jfrjnnglns) [[vim]] [[habit]]
    -   [use {SPC x o} (link hint open link)](#sspcxlnkhntpnlnk) [[habit]]
    -   [use SPC A for agenda](#sspcfrgnd) [[habit]]
    -   [{.} repeats last change](#rptslstchng) [[vim]] [[habit]]
    -   [chmod +x for a file: SPC f j for dired jump, then M](#chmdxfrflspcfjfrdrdjmpthnm) [[habit]]
    -   [use C-j and C-k in helm](#scjndcknhlm) [[habit]]
    -   [use {SPC s G} for google search](#sspcsgfrgglsrch) [[habit]]
        -   [maybe, add other engines later??](#mybddthrngnsltr) 
    -   [emacs ispell](#mcsspll) [[habit]]
    -   [use ,, in evil mode to insert note](#snvlmdtnsrtnt) [[habit]]
    -   [,> and ,< for demote and promote](#ndfrdmtndprmt) [[habit]]
    -   [use {,\\} for tex input](#sfrtxnpt) [[habit]]
-   [bad encoding..](#bdncdng) [[docker]] [[setup]]
-   [`[2020-02-20]` raxod502/straight.el: 🍀 Next-generation, purely functional package manager for the Emacs hacker.](#rxdstrghtlnxtgnrtnprlyfnctnlpckgmngrfrthmcshckr) 
-   [`[2020-07-06]` .emacs.d/index.md at 7e8514c98b63724ad0e97b8b3c56b96d00d56b7f · shrysr/.emacs.d](#sgthbcmshrysrmcsdblbcbdbbxmdtcbdbbcbddbfshrysrmcsd) 
-   [`[2020-07-06]` .emacs.d/emacs-config.org at 7e8514c98b63724ad0e97b8b3c56b96d00d56b7f · shrysr/.emacs.d](#sgthbcmshrysrmcsdblbcbdbbgrgtcbdbbcbddbfshrysrmcsd) 
-   [idpb tty to emacs config??](#dpbttytmcscnfg) [[ipdb]]
-   [`[2019-10-06]` My Emacs + Scimax configuration | Shreyas Ragavan](#mymcsscmxcnfgrtnshrysrgvn) 
-   [probably easier to hack ein to use different tags? than messing with nbstripout?](#prbblysrthckntsdffrnttgsthnmssngwthnbstrpt) [[jupyter]]
-   [`[2019-10-11]` My Personal Emacs History](#myprsnlmcshstry) 
    -   [`[2019-10-21]` As a drawback, I sometimes seem to repel others when I start praising my setup. My long journey with Emacs did result in a personal cozy environment that normal computer users do not seem to understand any more. Therefore, I have to remember to suppress the urge of mentioning the virtues of my environment. I have to stick to mentioning only the ultimate basics when I promote Emacs to normal computer users. Which is a pity, in my opinion.](#sdrwbcksmtmssmtrplthrswhnrmlcmptrsrswhchsptynmypnn) 
-   [`[2020-12-09]` Favorite Emacs Packages | Lobsters](#slbstrssccdgnfvrtmcspckgsfvrtmcspckgslbstrs) 
-   [`[2020-09-25]` Toward a “Modern” Emacs](#snwsycmbntrcmtmdtwrdmdrnmcs) [[emacs]]
-   [explore doom-snippets?](#xplrdmsnppts) [[python]]
-   [profiling emacs](#prflngmcs) [[emacs]]
-   [`[2020-03-24]` Wilfred/helpful: A better Emacs **help** buffer](#wlfrdhlpflbttrmcshlpbffr) [[emacs]]
-   [`[2019-11-15]` Voice typing in emacs talk](#vctypngnmcstlk) [[dictation]] [[emacs]]
-   [`[2019-08-18]` emacs-tw/awesome-emacs: A community driven list of useful Emacs packages, libraries and others.](#mcstwwsmmcscmmntydrvnlstfsflmcspckgslbrrsndthrs) [[emacs]]
-   [`[2019-12-24]` (Officially) Introducing M-EMACS ;) /r/emacs](#srddtcmrmcscmmntswwyhffclmmcsffcllyntrdcngmmcsrmcs) [[emacs]]
    -   [`[2020-02-28]` good example of reasonable emacs configurations (althrough Doom has most of it)](#gdxmplfrsnblmcscnfgrtnslthrghdmhsmstft) 
-   [`[2019-09-06]` emacsclient Options - GNU Emacs Manual](#mcsclntptnsgnmcsmnl) [[emacs]]
-   [emacs startup](#mcsstrtp) [[emacs]]
-   [`[2018-05-02]` debugging flycheck problems: 'flycheck-compile' will show you the command](#dbggngflychckprblmsflychckcmplwllshwythcmmnd) [[emacs]]
-   [debugging](#dbggng) [[emacs]] [[debug]]
-   [`[2020-02-04]` alphapapa/emacs-package-dev-handbook: An Emacs package development handbook. Built with Emacs, by Emacs package developers, for Emacs package developers.](#lphppmcspckgdvhndbknmcspcpckgdvlprsfrmcspckgdvlprs) [[elisp]]
-   [`[2020-12-30]` Leveraging Emacs Introspection | Irreal](#srrlrgblgplvrgngmcsntrspctnrrl) [[exobrain]] [[emacs]] [[debugging]]
-   [`[2020-10-28]` Add support for fd shell command · emacs-helm/helm@c11779c](#sgthbcmmcshlmhlmcmmtccdfctfrfdshllcmmndmcshlmhlmcc) 
-   [most common commands I'm using? could collect some stats automatically perhaps](#mstcmmncmmndsmsngcldcllctsmsttstmtcllyprhps) [[emacs]] [[toblog]]
-   [`[2019-11-21]` How do you use Emacs? /r/emacs](#srddtcmrmcscmmntsdznyjhwdysmcshwdysmcsrmcs) 
    -   [`[2019-12-02]` link on blog?](#lnknblg) [[toblog]]
-   [`[2020-12-28]` Redo stopped working (user-error: Customize ‘evil-undo-system’ for redo functionality.) · Issue #4135 · hlissner/doom-emacs](#sgthbcmhlssnrdmmcssssrdstfrrdfnctnltysshlssnrdmmcs) 
-   [`[2020-02-22]` .doom.d/config.el at master · nmartin84/.doom.d https://github.com/nmartin84/.doom.d/blob/master/config.el](#dmdcnfgltmstrnmrtndmdsgthbcmnmrtndmdblbmstrcnfgl) 
-   [`[2020-02-22]` nmartin84/.doom.d: This is my private DOOM emacs configuration. https://github.com/nmartin84/.doom.d](#nmrtndmdthssmyprvtdmmcscnfgrtnsgthbcmnmrtndmd) 
-   [`[2020-01-03]` Exploring large projects with Projectile and Helm Projectile https://tuhdo.github.io/helm-projectile.html](#xplrnglrgprjctswthprjctlnjctlsthdgthbhlmprjctlhtml) 
-   [`[2020-02-22]` Why is doom emacs so fast? · Issue #310 · hlissner/doom-emacs https://github.com/hlissner/doom-emacs/issues/310](#whysdmmcssfstsshlssnrdmmcssgthbcmhlssnrdmmcssss) 
-   [`[2020-02-21]` doom-emacs/getting<sub>started.org</sub> at develop · hlissner/doom-emacs https://github.com/hlissner/doom-emacs/blob/develop/docs/getting\_started.org](#dmmcsgttngstrtdrgtdvlphlsmcsblbdvlpdcsgttngstrtdrg) 
-   [`[2020-02-27]` hlissner/emacs-doom-themes: An opinionated pack of modern color-themes https://github.com/hlissner/emacs-doom-themes](#hlssnrmcsdmthmsnpnntdpckfhmssgthbcmhlssnrmcsdmthms) 
-   [`[2020-12-13]` Batteries included with Emacs | Karthinks](#skrthnkscmsftwrbttrsnclddcsbttrsnclddwthmcskrthnks) 
-   [`[2020-12-28]` Magit: How to show differences within lines - Emacs Stack Exchange](#smcsstckxchngcmqstnsmgthwffrncswthnlnsmcsstckxchng) 
-   [C-k/C-j for browsing images](#ckcjfrbrwsngmgs) [[emacs]] [[drill]]
-   [doom-big-font-mode](#dmbgfntmd) [[habit]] [[emacs]]





# related       [[elisp]]




# `[2019-12-23]` [What feature of emacs you tried in 2019 and now you can't live without?](https://reddit.com/r/emacs/comments/eemb76/what_feature_of_emacs_you_tried_in_2019_and_now/fbuoo9s/) /r/emacs      [[setup]]

    helm -- it's like it reads my mind of what file, buffer, command, etc that I want
    pytest-one and pytest-all -- easy  way  to run your python tests (in pytest, of course)
    direnv-mode -- a .envrc file has become my emacs config




## `[2020-02-28]` hmm, what could I use direnv for?




# `[2019-05-18]` [Refactoring in Spacemacs using iedit and helm-edit](https://reddit.com/r/spacemacs/comments/bnlgkv/refactoring_in_spacemacs_using_iedit_and_helmedit/) /r/spacemacs




# `[2020-01-30]` deadgrep      [[pkm]]

<https://beepb00p.xyz/pkm-search.html>  

    Wilfred•an hour ago
    Have you played with deadgrep at all for Emacs usage with ripgrep?
    It's not incremental, but you get a persistent results buffer, which can be really useful.




# dash.el (defmacro &#x2013;> (x &rest forms)      [[elisp]]




# need to either exclude ipynb or somehow exclude binary strings      [[pkm]] [[search]]





## `[2020-10-13]` ok, limit line width?




# need to hack on to prevent reordering etc I guess helm-rg&#x2013;helm-pattern-to-ripgrep-regexp




# `[2019-09-05]` Deft for Emacs

<https://jblevins.org/projects/deft>  

    Deft is an Emacs mode for quickly browsing, filtering, and editing directories of plain text notes, inspired by Notational Velocity. It was designed for increased productivity when writing and taking notes by making it fast and simple to find the right file at the right time and by automating many of the usual tasks such as creating new files and saving files.




# `[2019-12-26]` cask/cask: Project management tool for Emacs

<https://github.com/cask/cask>  

    Cask is a project management tool for Emacs that helps automate the package development cycle; development, dependencies, testing, building, packaging and more.




# (setq graphviz-dot-preview-extension "svg")




# autorevert? 




# learn to use ediff      [[habit]]

n/p to navigate  
a/b to move between  
start using it instead of vimdiff?  




# use tramp hops      [[docker]] [[ssh]]

I haven't tried it with docker, but you can chain tramp hops:  
/ssh:user@host|docker:foobar:/etc/whatever  




# disable evil last non blank




# `[2018-12-26]` millejoh/emacs-ipython-notebook: Jupyter notebook client in Emacs

<https://github.com/millejoh/emacs-ipython-notebook>  




# Tweet from ¬¬(Dan Piponi) (@sigfpe), at May 31, 22:14

    Set up my vim statusline so it shows contents of registers " and *. More useful than I expected. Made me realise how many times there were opportunities to streamline actions by making use of them.

<https://twitter.com/sigfpe/status/1134568962140753920>  




# ok, so important bits were adding subfolder project and switching in to 'extension'. Also, use error log buffer      [[setup]] [[lsp]]




# `[2019-09-01]` emacs-tw/awesome-emacs: A community driven list of useful Emacs packages, libraries and others.

<https://github.com/emacs-tw/awesome-emacs>  




# `[2019-09-02]` noctuid/evil-guide: Draft of a guide for using emacs with evil

<https://github.com/noctuid/evil-guide>  

    emacs-state-ma




# `[2019-07-30]` EmacsConf 2019 - Call for Proposals

<https://emacsconf.org/2019/cfp>  




# `[2019-10-18]` [EmacsConf 2019 Schedule](https://reddit.com/r/emacs/comments/djfh3t/emacsconf_2019_schedule/) /r/emacs      [[towatch]]




# ein is adding some metadata?? wtf?      [[ipython]]




# output-type-preference       [[ipython]]





## that seems to have fixed some output issues

    (setq ein:output-type-preference
         '(emacs-lisp svg png jpeg html text latex javascript))




# use SPC \* similarly to \*      [[habit]]




# `[2019-12-23]` [What feature of emacs you tried in 2019 and now you can't live without?](https://reddit.com/r/emacs/comments/eemb76/what_feature_of_emacs_you_tried_in_2019_and_now/) /r/emacs

    Modes, packages, themes, starter-kits you tried this year which blown you away.
    
    Mine: emacs itself




# `[2019-10-20]` Enabling helm-follow-mode on a per-command basis. · Issue 2006 · emacs-helm/helm

<https://github.com/emacs-helm/helm/issues/2006>  

    We have helm-moccur and helm-occur perfectly integrated in helm, faster
    than helm-swoop and well maintained, it is also highly configurable so
    that you can configure it to behave like helm-swoop.




# `[2020-01-03]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration

<https://github.com/MatthewZMD/.emacs.d#org3642bad>  

    (fset 'yes-or-no-p 'y-or-n-p)




# `[2019-12-29]` Forge – Work with Git forges from the comfort of Magit | Hacker News

<https://news.ycombinator.com/item?id=19137353>  

    That's so true! Emacs has got some modern and really well crafted packages during last decade (e.g. Magit, Org or Notmuch). It's a really interesting and vibrant platform right now. I have high hopes for lsp-mode.
    Another package with great UI is calfw.
    Of course, there were already plenty of great classic packages (e.g. Dired, Calc, Gnus or Eshell) and modes (e.g. AucTeX, SLIME, ESS...). But things are getting really good lately.
    ELPA and use-package have also done away with lots of friction points when installing and updating packages.




# emacs need something like check<sub>call</sub> in case rg is missing      [[elisp]]




# fucking hell. didn't manage to set up deadgrep

    default-directory seems to be responsible
    (let ((default-directory "/path/to/dir")) (deadgrep "test"))

but multiple dirs aren't working. spent 20 minutes trying to figure out how it's propagated to the source, but couldn't :crying:  




# <https://github.com/alphapapa/link-hint.el> 




# .emacs.d/local? not sure if need it under git      [[dotfiles]]




# andrewtropin кроме paredit, есть ещё любопытная штуковина parinfer: <https://shaunlebron.github.io/parinfer/>      [[elisp]] [[lisp]]




# `[2019-09-28]` eli-oat/pillow-fort.org: A literate emacs configuration      [[literate]]

<https://github.com/eli-oat/pillow-fort.org>  




# `[2019-09-07]` raxod502/el-patch: ✨ Future-proof your Emacs Lisp customizations!      [[setup]]

<https://github.com/raxod502/el-patch>  

    Why does it exist
    Emacs provides a comprehensive set of customizable variables and hooks as well as a powerful advice system. Sometimes, however, these are not enough and you must override an entire function in order to change a detail of its implementation.
    Such a situation is not ideal, since the original definition of the function might change when you update Emacs or one of its packages, and your overridden version would then be outdated. This could prevent you from benefitting from bugfixes made to the original function, or introduce new bugs into your configuration. Even worse, there is no way to tell when the original definition has changed! The correctness of your configuration is basically based on faith.




# `[2019-11-03]` Ambrevar / emacs-gif-screencast · GitLab

<https://gitlab.com/ambrevar/emacs-gif-screencast>  




# `[2019-11-08]` Whats your emacs setup like ? | Lobsters      [[toblog]]

<https://lobste.rs/s/754vk6/whats_your_emacs_setup_like>  

    I have an extensive literate configuration that configures many different subsystems, changes many default, etc. It’s rather verbose, but I hope it’s written in a way that even someone with minimal experiences my understand. I loosely inspired, but shorter and simpler configuration be found here (but watch out, the comments are in German!).




# Set up ipynb mode in emacs, display locals?      [[python]]




# implement search in filenames?      [[pkm]]




# configure source location for builtin stuff

find-function-C-source-directory  
ugh couldn't find in apt  




# `[2020-01-03]` (Officially) Introducing M-EMACS ;) : emacs

<https://www.reddit.com/r/emacs/comments/eewwyh/officially_introducing_memacs/>  

        add-to-list
    
    :mode keyword




# pip3 install &#x2013;user "python-language-server[all]"      [[setup]]




# cl-typecase       [[elisp]]




# use pp-eval-expression (SPC-;)      [[habit]]




# `[2020-02-28]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration

<https://github.com/MatthewZMD/.emacs.d#snails>  

    Snails, a fuzzy search framework




# `[2020-02-28]` bbatsov/super-save: Save Emacs buffers when they lose focus

<https://github.com/bbatsov/super-save>  

    super-save auto-saves your buffers, when certain events happen - e.g. you switch between buffers, an Emacs frame loses focus, etc.




# `[2020-02-28]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration

<https://github.com/MatthewZMD/.emacs.d#super-save>  

    (recentf-exclude '((expand-file-name package-user-dir)
                        ".cache"
                        ".cask"
                        ".elfeed"
                        "bookmarks"




# hmmm 

    (dotimes (i 9)
      (defalias (intern (format "+workspace/switch-to-%d" i))
        (lambda () (interactive) (+workspace/switch-to i))
        (format "Switch to workspace #%d" (1+ i))))




# setting up locate db&#x2026;

use. map SPC s f?  

    (helm-locate-with-db "/tmp/locate.db")




# `[2020-04-12]` How do I prevent messages from showing in the minibuffer? · Issue 2878 · hlissner/doom-emacs

<https://github.com/hlissner/doom-emacs/issues/2878>  

    What have you tried?
    
    I've read about inhibit-message, which apparently is used in
    ivy. However, I'm still seeing the GC me




# `[2020-05-07]` [EmacsWiki: Category Extension Language](https://www.emacswiki.org/emacs/CategoryExtensionLanguage)




# hmm maybe highlight closing parens less than opening? not sure      [[elisp]]




# `[2020-02-28]` MatthewZMD/.emacs.d: M-EMACS, a customized full-featured GNU Emacs configuration

<https://github.com/MatthewZMD/.emacs.d>  

    (Optional) On Ubuntu, emacs-snapshot is a great way to get latest version of Emacs.
    
    sudo add-apt-repository -y ppa:ubuntu-elisp
    sudo apt-get update
    sudo apt-get install emacs-snapshot




# emacs &#x2013; leader key takes ridiculous time to process      [[setup]]




# `[2020-01-10]` alphapapa/makem.sh: Makefile-like script for building and testing Emacs Lisp packages

<https://github.com/alphapapa/makem.sh>  

    Makefile-like script for building and testing Emacs Lisp packages




# `[2020-02-24]` doom-emacs/api.org at develop · hlissner/doom-emacs      [[doom]]

<https://github.com/hlissner/doom-emacs/blob/develop/docs/api.org>  

    after!

what's the difference from with-eval-after-load  




# `[2020-02-24]` doom-emacs/index.org at develop · hlissner/doom-emacs

<https://github.com/hlissner/doom-emacs/blob/develop/docs/index.org>  

    Doom is a configuration framework for GNU Emacs 26.3+ tailored for Emacs bankruptcy veterans who want less framework in their frameworks and the performance of a hand rolled config (or better). It can be a foundation for your own config or a resource for Emacs enthusiasts to learn more about our favorite OS.




# `[2020-03-14]` manateelazycat/emacs-application-framework: Emacs application framework

<https://github.com/manateelazycat/emacs-application-framework>  

    EAF is a GUI application framework that revolutionizes Emacs graphical capabilities to ultimately Live in Emacs.

hmm nice apparently you can write non-elisp code and easily intergrate?  




# use alt-n for 'default' filename completion? useful to rename things quickly      [[emacs]] [[habit]]




# indicate if there are some unsaved changes?





## `[2020-06-19]` maybe in title??




# tramp hangs while sending password      [[setup]]

<https://www.reddit.com/r/emacs/comments/7f62pn/tramp_hang_after_sending_password/dq9rfsq/>  




# audio annotation?




# agenda on F12 press? on constantly loaded emacs instance      [[setup]]

    emacs -nw --eval "(progn (setq org-agenda-window-setup 'only-window) (org-agenda-list))"




# Spacemacs ABC

<https://www.youtube.com/watch?v=ZFV5EqpZ6_s>  
undo-tree-visualize: SPC a u  
dired: SPC a d  
org: SPC a o  
process editor: SPC a P how to vim mode?  

SPC / vs SPC \*? 1  

SPC SPC M-x  

g c &#x2013; comment  
SPC F1: fuzzy search emacs stuff  
SPC ? : keybindings  

<https://www.youtube.com/watch?v=B39tFs2ifHg>  




# traad for refactoring      [[python]]




# `[2018-11-05]` alphapapa/org-ql: An Org query language, and experimental code for a next-generation Org Agenda

<https://github.com/alphapapa/org-ql>  




# try skeletor

creating project templates  
<https://www.reddit.com/r/emacs/comments/8j15ji/_/dywc329?context=1000>  
<https://www.reddit.com/r/emacs/comments/8j15ji/how_has_emacs_ever_really_blown_you_away/dyzfucv/>  




# haskell ide engine thing      [[haskell]]





## ok, so lsp-demote thing is no bound to any key. I might help with that?




## right! lsp-ui-sideline-apply-code-actions




# helm stupid behaviour when trying to rename file

<https://github.com/syl20bnr/spacemacs/issues/9044>  

    (setq-default helm-display-function 'helm-default-display-buffer) -- kinda works...




# <http://www.viemu.com/a-why-vi-vim.html>       [[vim]]

di : delete innte, basiclaly like d%, but you don't have to be in the beginning of block  
']]' and the likes to navigate by functions, etc.  
vaS &#x2013; select sentence, selects current function  
vaB &#x2013; select block  
>aB &#x2013; indent block  




# `[2019-09-04]` kunalb/poet: An emacs theme that's well suited for modes using variable pitch: particularly org-mode and markdown-mode.

<https://github.com/kunalb/poet>  




# (agda-input-add-translations '( ("pd" . "∂") ))




# agda input

    (load-file (let ((coding-system-for-read 'utf-8))
                    (shell-command-to-string "agda-mode locate")))
    t
     (require 'agda-input)
    agda-input




# memoize &#x2013; if function returns nil (e.g. empty list, the value is always recomputed)      [[elisp]]




# `[2019-10-31]` camcorder.el - Creating Animated Gifs & Videos for Spacemacs | jr0cket

<http://jr0cket.co.uk/2017/01/spacemacs-creating-animated-gifs-videos.html>  

    camcorder.el - Creating Animated Gifs & Videos for Spacemacs




# `[2019-12-20]` belak/emacs-grayscale-theme

<https://github.com/belak/emacs-grayscale-theme>  




# `[2019-12-20]` Whats your emacs setup like ? | Lobsters

<https://lobste.rs/s/754vk6/whats_your_emacs_setup_like>  




# ein evil mode :w      [[jupyter]]




# `[2018-11-06]` narendraj9/hledger-mode: An Emacs major mode for Hledger

<https://github.com/narendraj9/hledger-mode>  




# email? 

maybe switch to emacs?  
Perhaps I should switch to thunderbird? Not sure what is used real world TODO?  




# can use setf?      [[elisp]]

    (when super-groups
      (let ((org-super-agenda-groups (cl-etypecase super-groups
                                       (symbol (symbol-value super-groups))
                                       (list super-groups))))
        (setf strings (org-super-agenda--group-items strings))))




# Tweet from @burntsushi5

    https://twitter.com/burntsushi5/status/1232467306887860225
    @burntsushi5: Hah. This is very likely due to ripgrep's parallelism (which includes walking the directory tree in parallel too). `find` is not parallel at all. try `rg -j1 <whatever>` to put it on more even footing. :-)




# `[2020-01-03]` (Officially) Introducing M-EMACS ;) : emacs

<https://www.reddit.com/r/emacs/comments/eewwyh/officially_introducing_memacs/>  

        add-hook
    if you already use use-package, there's absolutely no need to use it, since there is :hook keyword




# helm-locate-library       [[habit]]




# `[2020-05-01]` [on the usability of editable software | Lobsters](https://lobste.rs/s/qkpwpa/on_usability_editable_software)

    
    emoses avatar emoses 2 hours ago | link |
    
    Emacs is great for this, especially if you use straight. Straight makes a local clone of each package repo. If you want to edit it, edit it and commit (or don’t), and your emacs will use the local copy.




# Habits 





## use org-created-to-inline {, c}      [[habit]]




## [SPC e l] error list




## it's fine to use C-c and C-v in insert mode      [[habit]]




## {>aR} demote subtree      [[habit]] [[org]]

<https://github.com/Somelauw/evil-org-mode>  




## use SPC-t      [[habit]] [[org]]




## selecting class: {v close sqbracket open sqbracket}      [[habit]]




## use eshell more      [[habit]]




## use SPC S c and SPC s i to search code and info      [[habit]]




## Use magit more, many people claim its superior to cli      [[habit]] [[git]]

<https://github.com/syl20bnr/spacemacs/tree/master/layers/%2Bsource-control/git#quick-guide-for-recurring-use-cases-in-magit>  




## use 'light'      [[habit]]




## use SPC p P      [[habit]]




## Use prj: to link to file in the same project      [[habit]]




## Use tramp      [[oldhabit]]

ssh:target:/&#x2026;  




## use helm-resume SPC h l to resume search      [[habit]]




## use eshell:      [[habit]]




## use X to delete      [[habit]]




## use # and T      [[habit]]

hash is the opposite of \*?  




## use C-g to interrupt stuck commands      [[habit]]




## J for joining lines      [[vim]] [[habit]]




## use {SPC x o} (link hint open link)      [[habit]]




## use SPC A for agenda      [[habit]]

maybe swap a and A? note sure  




## {.} repeats last change      [[vim]] [[habit]]




## chmod +x for a file: SPC f j for dired jump, then M      [[habit]]




## use C-j and C-k in helm      [[habit]]




## use {SPC s G} for google search      [[habit]]





### maybe, add other engines later??




## emacs ispell      [[habit]]




## use ,, in evil mode to insert note      [[habit]]




## ,> and ,< for demote and promote      [[habit]]




## use {,\\} for tex input      [[habit]]




# bad encoding..      [[docker]] [[setup]]




# `[2020-02-20]` raxod502/straight.el: 🍀 Next-generation, purely functional package manager for the Emacs hacker.

<https://github.com/raxod502/straight.el#comparison-to-packageel>  




# `[2020-07-06]` [.emacs.d/index.md at 7e8514c98b63724ad0e97b8b3c56b96d00d56b7f · shrysr/.emacs.d](https://github.com/shrysr/.emacs.d/blob/7e8514c98b63724ad0e97b8b3c56b96d00d56b7f/index.md)




# `[2020-07-06]` [.emacs.d/emacs-config.org at 7e8514c98b63724ad0e97b8b3c56b96d00d56b7f · shrysr/.emacs.d](https://github.com/shrysr/.emacs.d/blob/7e8514c98b63724ad0e97b8b3c56b96d00d56b7f/emacs-config.org)




# idpb tty to emacs config??      [[ipdb]]

    import sys; import ipdb
    if sys.stdin.isatty():
        ipdb.set_trace()




# `[2019-10-06]` My Emacs + Scimax configuration | Shreyas Ragavan

<https://shrysr.github.io/docs/sr-config/>  

    Swiper

I use swiper for a general search. However helm-swoop is awesome.  




# probably easier to hack ein to use different tags? than messing with nbstripout?      [[jupyter]]




# `[2019-10-11]` My Personal Emacs History

<https://karl-voit.at/2017/06/03/emacs-history/>  

    My Personal Emacs History




## `[2019-10-21]` As a drawback, I sometimes seem to repel others when I start praising my setup. My long journey with Emacs did result in a personal cozy environment that normal computer users do not seem to understand any more. Therefore, I have to remember to suppress the urge of mentioning the virtues of my environment. I have to stick to mentioning only the ultimate basics when I promote Emacs to normal computer users. Which is a pity, in my opinion.

huh, very similar experience  




# `[2020-12-09]` [Favorite Emacs Packages | Lobsters](https://lobste.rs/s/cocdgn/favorite_emacs_packages)

    deadgrep. When using counsel-rg gives to many results, deadgrep offers a very clean interface to view and navigate the results of a search. I especially love that by default it finds the root of the project (a Git project for example) so it DWIMs pretty well.




# `[2020-09-25]` [Toward a “Modern” Emacs](https://news.ycombinator.com/item?id=24593616)      [[emacs]]

<https://lwn.net/SubscriberLink/832311/03910e26a3f3e814/>  




# explore doom-snippets?      [[python]]




# profiling emacs      [[emacs]]

`emacs --debug-init --timed-requires`  

(will create a buffer with load times)  
vim core/core-debug.el , (defvar spacemacs-debug-timer-threshold 0.05 to adjust  

`emacs --debug-init --profile` &#x2013; will create CPU and memory profile  




# `[2020-03-24]` Wilfred/helpful: A better Emacs **help** buffer      [[emacs]]

<https://github.com/Wilfred/helpful>  




# `[2019-11-15]` Voice typing in emacs talk      [[dictation]] [[emacs]]

Main point I guess is using refactorings and modifiers (e.g. camel before saying car name)  
Optimizing the most common ops first  




# `[2019-08-18]` emacs-tw/awesome-emacs: A community driven list of useful Emacs packages, libraries and others.      [[emacs]]

<https://github.com/emacs-tw/awesome-emacs#readme>  




# `[2019-12-24]` [(Officially) Introducing M-EMACS ;)](https://reddit.com/r/emacs/comments/eewwyh/officially_introducing_memacs/) /r/emacs      [[emacs]]

    It's the end of 2019, I realized that I have worked on [M-EMACS](https://github.com/MatthewZMD/.emacs.d) for nearly a year now. M-EMACS is my personal Emacs setup and configurations, I have been spreading it for some time in comment sections and received some positive feedback from the community, but somehow I never bother to write a post to officially introduce it ;)

    So here I am.

    Besides some Emacs' killer-features nicely configured out-of-box for you (e.g `lsp`, `ivy`, `company`, `erc`, `eaf`, `mu4e`, `tramp`, etc.), M-EMACS README is aiming to be one of the best `org-mode` Emacs config available. While heavily using `use-package` in the code, and providing a link with a one-sentence description to each package it uses, it also has a little `Prerequisite` note for any *heavier* packages that require more setup than just copy-and-paste elisp code ;)

    With [M-EMACS](https://github.com/MatthewZMD/.emacs.d), I am also exploring a new way to organize Emacs config files. AFAIK, most of the people (who cared enough to heavily organize `.emacs.d`) in the community either put their config in a subdirectory called `lisp` or `elisp` with many files like `init-xx.el`, or they put their entire config in a **HUGE** `.org` file with numerous `#+BEGIN_SRC` and `#+END_SRC` blocks, and use `org-babel-load-file` in `init.el` to load all the elisp code on startup. The former is well-organized but can get complicated and frustrating for anyone other than the owner to navigate through the code. The latter is much more user-friendly, it's so much nicer to navigate through a Github README page and really helpful to any Emacs user who just wants to quickly find a config snippet for a particular package. However, the downside is that `org-babel-load-file` can get *pretty* slow sometimes, wasting a lot of startup time.

    [M-EMACS](https://github.com/MatthewZMD/.emacs.d), on the other hand, combines these two approaches together: all elisp code is organized in an `elisp` folder, with some `#+INCLUDE` statements in an `org` file, elisp code are populated into a Github-friendly README with a single command. Below is the snippet from the [About README](https://github.com/MatthewZMD/.emacs.d#about-readme) section:

    > This README is originated from `init.org` that is generated using `M-x org-gfm-export-to-markdown`. Every block of code is generated through this function - it exports the section of code from the `elisp/` directory. You will not see their presence in `init.org`.

    The result is an organized, detailed and user-friendly README with super-fast startup time, best of both worlds.

    Anyways, enough babbling, feel free to [check it out](https://github.com/MatthewZMD/.emacs.d) during this holiday season :)




## `[2020-02-28]` good example of reasonable emacs configurations (althrough Doom has most of it)




# `[2019-09-06]` emacsclient Options - GNU Emacs Manual      [[emacs]]

<https://www.gnu.org/software/emacs/manual/html_node/emacs/emacsclient-Options.html>  

    ‘--alternate-editor=command’
        Specify a shell command to run if emacsclient fails to contact Emacs. This is useful when running emacsclient in a script. The command may include arguments, which may be quoted "like this". Currently, escaping of quotes is not supported.
    
        As a special exception, if command is the empty string, then emacsclient starts Emacs in daemon mode (as ‘emacs --daemon’) and then tries connecting again.
    
        The environment variable ALTERNATE_EDITOR has the same effect as the ‘-a’ option. If both are present, the latter takes precedence. 




# emacs startup      [[emacs]]

<https://www.gnu.org/software/emacs/manual/html_node/elisp/Startup-Summary.html>  

before-init-hook  
after-init-hook  
emacs-startup-hook  




# `[2018-05-02]` debugging flycheck problems: 'flycheck-compile' will show you the command      [[emacs]]




# debugging       [[emacs]] [[debug]]

(debug-on-entry 'funcname')  

c &#x2013; exit debugger  
d &#x2013; continue debugging (or 's'???)  
e &#x2013; eval expression  




# `[2020-02-04]` alphapapa/emacs-package-dev-handbook: An Emacs package development handbook. Built with Emacs, by Emacs package developers, for Emacs package developers.      [[elisp]]

<https://github.com/alphapapa/emacs-package-dev-handbook>  

    The Emacs Package Developer’s Handbook




# `[2020-12-30]` [Leveraging Emacs Introspection | Irreal](https://irreal.org/blog/?p=9156)      [[exobrain]] [[emacs]] [[debugging]]




# `[2020-10-28]` [Add support for fd shell command · emacs-helm/helm@c11779c](https://github.com/emacs-helm/helm/commit/c11779cd11a1f62cd160ea9507641f8cc1a9d321)

    Add support for fd shell command




# most common commands I'm using? could collect some stats automatically perhaps      [[emacs]] [[toblog]]




# `[2019-11-21]` [How do you use Emacs?](https://reddit.com/r/emacs/comments/dzn3yj/how_do_you_use_emacs/) /r/emacs

    Hi everyone.
    Considering our beloved Emacs can be used as anything from an all encompassing GUI window manager/userspace behemoth to a casual simple text editor via emacsclient similar to what vimmers do, where is your sweet spot?
    If you don't do exwm, what's your favorite de/wm? (assuming of course you use Linux (The Gnu system of which Linux is just a kernel of don't stone me gnu guys))
    How much of general computing you do in emacs? Email, Internet, etc.
    I would love to hear your input.




## `[2019-12-02]` link on blog?      [[toblog]]




# `[2020-12-28]` [Redo stopped working (user-error: Customize ‘evil-undo-system’ for redo functionality.) · Issue #4135 · hlissner/doom-emacs](https://github.com/hlissner/doom-emacs/issues/4135)

    Either enable :emacs undo (for undo-fu), :emacs (undo +tree) (for undo-tree), or upgrade to Emacs 28 (for undo-redo). If you don't know which one to pick, I recommend the first.




# `[2020-02-22]` .doom.d/config.el at master · nmartin84/.doom.d <https://github.com/nmartin84/.doom.d/blob/master/config.el>




# `[2020-02-22]` nmartin84/.doom.d: This is my private DOOM emacs configuration. <https://github.com/nmartin84/.doom.d>




# `[2020-01-03]` Exploring large projects with Projectile and Helm Projectile <https://tuhdo.github.io/helm-projectile.html>




# `[2020-02-22]` Why is doom emacs so fast? · Issue #310 · hlissner/doom-emacs <https://github.com/hlissner/doom-emacs/issues/310>




# `[2020-02-21]` doom-emacs/getting<sub>started.org</sub> at develop · hlissner/doom-emacs <https://github.com/hlissner/doom-emacs/blob/develop/docs/getting_started.org>

    Important: you may encounter errors after up/downgrading Emacs. Emacs bytecode is generally not forward compatible. You will have to recompile or reinstall your packages to fix this, i.e.
    
        doom build, to rebuild all your installed packages,




# `[2020-02-27]` hlissner/emacs-doom-themes: An opinionated pack of modern color-themes <https://github.com/hlissner/emacs-doom-themes>

    Re-set org-todo' & org-headline-done' faces to make them respect underlying faces (i.e. don't override the :height or :background of underlying faces).

-   very nice!




# `[2020-12-13]` [Batteries included with Emacs | Karthinks](https://karthinks.com/software/batteries-included-with-emacs/)

    Pulse (pulse.el)
    The included pulse library provides functions to flash a region of text. The most useful general application is to flash the line the cursor is on as a navigational aid or accessibility feature.




# `[2020-12-28]` [Magit: How to show differences within lines - Emacs Stack Exchange](https://emacs.stackexchange.com/questions/43643/magit-how-to-show-differences-within-lines)

    If you want to store that in your config, like me, just add
    (setq magit-diff-refine-hunk (quote all))




# C-k/C-j for browsing images      [[emacs]] [[drill]]




# doom-big-font-mode       [[habit]] [[emacs]]

