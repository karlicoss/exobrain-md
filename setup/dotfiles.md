
# Table of Contents

-   [awesome-dotfiles https://github.com/webpro/awesome-dotfiles](#wsmdtflssgthbcmwbprwsmdtfls) 
-   [What I tried](#whttrd) 
    -   [gnu stow?](#gnstw) 
    -   [fresh to build gh config? https://github.com/freshshell/fresh](#frshtbldghcnfgsgthbcmfrshshllfrsh) 
    -   [homesick? https://github.com/technicalpickles/homesick](#hmscksgthbcmtchnclpcklshmsck) 
    -   [mackup? https://github.com/lra/mackup](#mckpsgthbcmlrmckp) 
    -   [vcsh http://blog.tfnico.com/2014/03/managing-dot-files-with-vcsh-and-myrepos.html](#vcshblgtfnccmmngngdtflswthvcshndmyrpshtml) 
    -   [dotbot?](#dtbt) 
    -   [dotdrop https://github.com/deadc0de6/dotdrop](#dtdrpsgthbcmddcddtdrp) 
    -   [dotgit https://github.com/kobus-v-schoor/dotgit](#dtgtsgthbcmkbsvschrdtgt) 
    -   [https://github.com/evanpurkhiser/dots has post installation script](#sgthbcmvnprkhsrdtshspstnstlltnscrpt) 
-   [using git repository with symlinks + external ~ working directory](#snggtrpstrywthsymlnksxtrnlwrkngdrctry) [[git]]
    -   [bootstrapping](#btstrppng) 
    -   [workflow](#wrkflw) 
    -   [try git lfs?](#trygtlfs) 
-   [something about files which can't be kept in git](#smthngbtflswhchcntbkptngt) [[git]]
    -   [for configs which are patched via script, symlink what patches it](#frcnfgswhchrptchdvscrptsymlnkwhtptchst) [[setup]]
-   [Tooling](#tlng) 
    -   [jq for patching JSON](#jqfrptchngjsn) [[json]]
-   [`[2018-06-20]` configs which are not symlinking &#x2013; have a script which checks them against reference every few hours and complains if config doesn't match the reference?](#cnfgswhchrntsymlnknghvscrmplnsfcnfgdsntmtchthrfrnc) 
-   [related](#rltd) [[infra]]
-   [`[2019-06-01]` motivation for core.worktree](#mtvtnfrcrwrktr) [[git]] [[setup]] [[dotfiles]]
-   [`[2020-07-12]` Manage your dotfiles with Git - openSUSE News](#snwspnssrgmngdtflswthgtmngyrdtflswthgtpnssnws) [[git]]
-   [`[2020-05-26]` Dotfiles - Joe Yates' Blog](#sjytsnfdtflsdtflsjytsblg) [[git]] [[dotfiles]]





# awesome-dotfiles <https://github.com/webpro/awesome-dotfiles>

TODO check occasionally?  




# What I tried





## gnu stow?

apparently a parallel hierarchy with symlinks?  
would be nice to specify, which directories should be created and which should just be symlinked. Otherwise stuff might end up in symlinked folders  

-   very clumsy to use, hard to replace existing entries, no apparent way of deleting them (unlike git)




## fresh to build gh config? <https://github.com/freshshell/fresh>

you can write a configuration, and it will symlinka all automatically  
apparently can source from gh repos, so you could just 'follow' someones' dotfiles (not very portable though)  




## homesick? <https://github.com/technicalpickles/homesick>

looks like a parallel hierarchy of dotfiles mimicing /home? could be convenient to manage with symlinks&#x2026;  
wonder if .homesick directory is configurable  

ok, so if i create home dir and add relative symlinks to it, it sort of works fine.  
add a script to check symlink integrity?  
still unclear what should i do with patch files. maybe have a manual dir with symlinks as well?  
homesick track? although it's a bit weird if configuration comes from different files, but i guess it's quite rare  

ugh.. homedir<sub>subdir</sub> is a bit weird.. could make it support relative symlinks within repo  
ugh.. homesick seems to rewrite relative symlinks to absolute&#x2026; wtf???  




## mackup? <https://github.com/lra/mackup>

apparently just backs up and symlinks configs for some applications  
hmm, so it supports doublecmd. wonder how they handle their configs..  
nope, just copies. nothing interesting  

-   `[2021-05-04]` doesn't support mc




## vcsh <http://blog.tfnico.com/2014/03/managing-dot-files-with-vcsh-and-myrepos.html>

weird stuff, messes with git and uses mr tool to manipulate on multiple repos at the same time  
take another look at it?  
mm &#x2013; ok, so apparently it's just like single repo view but routing to different subrepos  
e.g. vcsh init vim; vcsh vim commit .vimrc  




## dotbot? 

yaml configs.. ugh  




## dotdrop <https://github.com/deadc0de6/dotdrop>

allows templating thanks to jinja2  
erm.. it copies, not symlinks apparently  




## dotgit <https://github.com/kobus-v-schoor/dotgit>

hmm encryption!  
aims to keep all in single repository  
too comlicated.  




## <https://github.com/evanpurkhiser/dots> has post installation script

was updated 2 years ago  




# using git repository with symlinks + external ~ working directory      [[git]]

/repos/configuration  
cgit command  

-   cons: not dropbox friendly because of symlinks  
    maybe sync via syncthing?  
    -   TODO how to make todos here?

-   keep only symlinks to files unless it absolutely makes sense to symlink directory  
    why: if it's a directory locally and a symlink in the repo (e.g. with autostart dir), it won't merge easily

-   symlink into from various repos  
    -   public dotfiles
    -   private dotfiles
    -   machine specific dotfiles
    -   files which aren't under git (configs-nogit)  
        config-nogit: use tree command to store contents  
        maybe git lfs would be better for that??
    -   scripts
    -   histories: bash, python, etc.
    -   etc




## bootstrapping 

-   alias cgit='git &#x2013;git-dir=/repos/configuration/.git &#x2013;work-tree=/home/karlicos'
-   cgit ireset &#x2013; to restore working dir state
-   run check.sh from ~ and restore all the missing symlinks  
    resolve filtype configs (file vs symlinks)




## workflow 

cgit status to see if anything has changed  
cgit add / cgit commit / cgit push  




## try git lfs?




# something about files which can't be kept in git      [[git]]





## for configs which are patched via script, symlink what patches it      [[setup]]

`ln -s "$(realpath $BASH_SOURCE)" "$CDIR"`  




# Tooling 





## jq for patching JSON      [[json]]

<https://jqplay.org/> is also quite convenient  




# `[2018-06-20]` configs which are not symlinking &#x2013; have a script which checks them against reference every few hours and complains if config doesn't match the reference?

I guess it would belong to configuration repository  




# related       [[infra]]




# `[2019-06-01]` motivation for core.worktree      [[git]] [[setup]] [[dotfiles]]

can't use bare repository since they don't have index  
we don't want to use working directory since it's just confusing  
solution is git config core.worktree $HOME  




# `[2020-07-12]` [Manage your dotfiles with Git - openSUSE News](https://news.opensuse.org/2020/03/27/Manage-dotfiles-with-Git/)      [[git]]




# `[2020-05-26]` [Dotfiles - Joe Yates' Blog](https://joeyates.info/2018/12/16/dotfiles/)      [[git]] [[dotfiles]]

very similal to how I manage it &#x2013; the git based approach is super simple, portable and predictable  

