
# Table of Contents

-   [\* why use static blog?](#whyssttcblg) 
    -   [`[2019-09-15]` static blog: benefits of having it compiled with git directory &#x2013; it's trivial to track changes](#sttcblgbnftsfhvngtcmpldwthgtdrctrytstrvlttrckchngs) 
    -   [`[2019-09-04]` Normal are too linear, can't trick them into doing what I want](#nrmlrtlnrcnttrckthmntdngwhtwnt) 
    -   [`[2019-09-02]` everything you don't like you can hack in code](#vrythngydntlkycnhckncd) [[self]]
-   [\* what makes it hard?](#whtmksthrd) 
    -   [why it's hard: proper search (e.g. stemming)](#whytshrdprprsrchgstmmng) 
    -   [why it's hard: limiting feed size](#whytshrdlmtngfdsz) 
        -   [make something generic for Hakyll?](#mksmthnggnrcfrhkyll) 
    -   [why it is hard: making them useful for non-programmers](#whytshrdmkngthmsflfrnnprgrmmrs) 
        -   [`[2019-12-26]` link to sad-infra](#lnktsdnfr) 
    -   [ugh, nondeterministic order of outputs?](#ghnndtrmnstcrdrftpts) [[blog]] [[sympy]]
-   [---------------------](#1658_1723) 
-   [don't be afraid to use conventional command line tools](#dntbfrdtscnvntnlcmmndlntls) [[ipynb]]
-   [as a tip: have a test page](#stphvtstpg) 
-   [post about screenshot comparison](#pstbtscrnshtcmprsn) 
    -   [`[2019-09-21]` could post that separately?](#cldpstthtsprtly) 
    -   [`[2019-09-21]` change CSS on tags and demonstrate it?](#chngcssntgsnddmnstrtt) 
-   [checker that anything that was ever on my blog is still available (post about it too!)](#chckrthtnythngthtwsvrnmyblgsstllvlblpstbttt) 
    -   [`[2019-09-02]` link checker kinda does that?](#lnkchckrknddstht) 
-   [firefox responsive view thing](#frfxrspnsvvwthng) 
-   [meta: technical choices](#mttchnclchcs) 
-   [Editing blog](#dtngblg) [[cloudmacs]]
-   [if possible, use `file:` links in `.org` files instead of HTML links](#fpssblssrgmdrgmnlsrchptnsfllnksnrgflsnstdfhtmllnks) [[org]]
-   [about storing data in git repository, report via diff](#btstrngdtngtrpstryrprtvdff) 
-   [Post about symlink watcher thing?](#pstbtsymlnkwtchrthng) 
-   [feature of org-compile: output files. wonder how would you achieve that in pandoc](#ftrfrgcmpltptflswndrhwwldychvthtnpndc) 
-   [`[2020-01-13]` why it's hard: nondeterminism](#whytshrdnndtrmnsm) [[ipynb]]

Some extra info here <https://beepb00p.xyz/site.html#easier_blogs> (probably need to merge the two)  




# \* why use static blog?





## `[2019-09-15]` static blog: benefits of having it compiled with git directory &#x2013; it's trivial to track changes

just need to make sure there are no random ids/hashes etc  




## `[2019-09-04]` Normal are too linear, can't trick them into doing what I want




## `[2019-09-02]` everything you don't like you can hack in code      [[self]]

code can do literally anything you wish, this is very empowering  




# \* what makes it hard?





## why it's hard: proper search (e.g. stemming)




## why it's hard: limiting feed size





### make something generic for Hakyll?




## why it is hard: making them useful for non-programmers





### `[2019-12-26]` link to sad-infra




## ugh, nondeterministic order of outputs?      [[blog]] [[sympy]]

-   didn't help: import random; random.seed(0)




# --------------------- 




# don't be afraid to use conventional command line tools      [[ipynb]]

example with stripping private todos  

why it may seem unreliable or hacky, it's very effortless to try it out and in conjunction with  
version control for your outputs, you're unlikely to mess anything up massively  




# as a tip: have a test page




# post about screenshot comparison





## `[2019-09-21]` could post that separately?




## `[2019-09-21]` change CSS on tags and demonstrate it?




# checker that anything that was ever on my blog is still available (post about it too!)





## `[2019-09-02]` link checker kinda does that?




# firefox responsive view thing




# meta: technical choices

-   State "STRT"      from "TODO"       `[2019-02-18]`

minimalistic design  

disqus: I'd love to use something else&#x2026;  

sorry for that: I'm still allowing guest comments though  
Note: Registered users must now verify their email address prior to posting a comment. Pre-moderation is always enabled for guest comments.  




# Editing blog      [[cloudmacs]]




# if possible, use [`file:`](https://orgmode.org/manual/Search-options.html#Search-options) links in `.org` files instead of HTML links      [[org]]

E.g. instead of  

    [[./sad-infra.html#why][here]]

, you can use:  

    [[file:sad-infra.org::#why][here]]

Benefit of the latter is that link also works in org-mode source (unlike the former). During the export it's automatically resolved to HTML.  




# about storing data in git repository, report via diff




# Post about symlink watcher thing?




# feature of org-compile: output files. wonder how would you achieve that in pandoc




# `[2020-01-13]` why it's hard: nondeterminism      [[ipynb]]

link to issue with seaborn  

