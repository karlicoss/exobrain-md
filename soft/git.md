
# Table of Contents

-   [`[2020-04-19]` The Communicative Value of Using Git Well – Math ∩ Programming](#sjrmykncmthcmmnctvvlfsnggctvvlfsnggtwllmthprgrmmng) [[git]]
-   [`[2017-05-06]` use `hg-fast-export` to convert](#shgfstxprttcnvrt) [[mercurial]] [[git]]
-   [`[2016-09-07]` git stores snapshots, not diffs](#gtstrssnpshtsntdffs) [[git]]
-   [NOCOMMIT global hook?](#ncmmtglblhk) [[git]]
-   [`[2019-08-18]` Highlights from Git 2.23 - The GitHub Blog](#hghlghtsfrmgtthgthbblg) [[git]]
-   [Git blame ignore formatting](#gtblmgnrfrmttng) [[git]]
-   [`[2019-08-24]` Fossil Versus Git | Lobsters](#fsslvrssgtlbstrs) [[git]]
-   [My unorthodox, branchless git workflow | Lobsters](#mynrthdxbrnchlssgtwrkflwlbstrs) [[git]]
-   [a page with my favourite git commands & tricks?](#pgwthmyfvrtgtcmmndstrcks) [[git]] [[toblog]] [[exobrain]]
-   [The Communicative Value of Using Git Well – Math ∩ Programming](#thcmmnctvvlfsnggtwllmthprgrmmng) [[git]]
-   [`[2019-08-02]` git - How do I remove a submodule? - Stack Overflow](#gthwdrmvsbmdlstckvrflw) [[git]]
-   [`[2019-12-11]` git reflog expire &#x2013;expire=now &#x2013;all && git gc &#x2013;prune=now &#x2013;aggressive](#gtrflgxprxprnwllgtgcprnnwggrssv) [[github]]
-   [`[2019-05-10]` git rebase &#x2013;committer-date-is-author-date  &#x2013;autostash HEAD~1](#gtrbscmmttrdtsthrdttstshhd) [[git]]
-   [`[2020-06-08]` Learn to change history with git rebase!](#sgtrbslrntchnghstrywthgtrbs) 
-   [`[2018-11-28]` extraction - How to extract one file with commit history from a git repo with index-filter & co - Stack Overflow](#xtrctnhwtxtrctnflwthcmmthmgtrpwthndxfltrcstckvrflw) [[git]]
    -   [`[2019-04-10]` set up git project commmand](#stpgtprjctcmmmnd) 
-   [`[2020-07-12]` - GitHub + why do we centralize issues, documents for a **distributed** version&#x2026; | Hacker News](#snwsycmbntrcmtmdgthbwhydwcmntsfrdstrbtdvrsnhckrnws) 
-   [`[2018-01-01]` detect file type changes](#dtctfltypchngs) [[git]]
-   [git ssh debugging](#gtsshdbggng) [[git]] [[ssh]]
-   [`[2021-01-11]` How to keep your Git history clean with interactive rebase | GitLab](#sbtgtlbcmblgkpgthstryclnwthstryclnwthntrctvrbsgtlb) 
-   [`[2020-11-16]` Why Git blame sucks for understanding WTF code (and what you should use instead) | Lobsters](#slbstrssnvpwhygtblmscksfrtfcdndwhtyshldsnstdlbstrs) 
-   [`[2019-07-21]` git - How do I remove a submodule? - Stack Overflow https://stackoverflow.com/questions/1260748/how-do-i-remove-a-submodule/7646931#7646931](#gthwdrmvsbmdlstckvrflwsstckvrflwcmqstnshwdrmvsbmdl) [[git]]





# `[2020-04-19]` [The Communicative Value of Using Git Well – Math ∩ Programming](https://jeremykun.com/2020/01/14/the-communicative-value-of-using-git-well/)      [[git]]




# `[2017-05-06]` use `hg-fast-export` to convert      [[mercurial]] [[git]]




# `[2016-09-07]` git stores snapshots, not diffs      [[git]]

    Different from SVN
    It is important to note that this is very different from most SCM systems that you may be familiar with. Subversion, CVS, Perforce, Mercurial and the like all use Delta Storage systems - they store the differences between one commit and the next.
    Git does not do this - it stores a snapshot of what all the files in your project look like in this tree structure each time you commit. This is a very important concept to understand when using Git.
    Git’s pack files are carefully constructed to effectively use disk caches and provide “nice” access patterns for common commands and for reading recently referenced objects.




# NOCOMMIT global hook?      [[git]]




# `[2019-08-18]` Highlights from Git 2.23 - The GitHub Blog      [[git]]

<https://github.blog/2019-08-16-highlights-from-git-2-23/>  

    You may have used git grep to search for some text in your Git project, just as you may have used git diff to view active changes. What do the two have in common? They both display some contents in your repository, and both have support to show the surrounding function context with -p (short for --show-function) or -W (short for --function-context), respectively.




# Git blame ignore formatting      [[git]]

    Configure your git blame to ignore cleanup changes.

<https://www.moxio.com/blog/43/ignoring-bulk-change-commits-w>&#x2026;  




# `[2019-08-24]` Fossil Versus Git | Lobsters      [[git]]

<https://lobste.rs/s/e3blgf/fossil_versus_git>  

    This article is getting a few things about git wrong. They claim git only supports ‘One check-out per repository’. Heard of git worktree?




# My unorthodox, branchless git workflow | Lobsters      [[git]]

    Git revise is especially useful for this commit stack workflow, as I call it. I’m a huge fan.
    
    It’s a better rebase. So much better that it should be obligatory. You can split commits, batch rename them, and you don’t have to stash your work first.




# a page with my favourite git commands & tricks?      [[git]] [[toblog]] [[exobrain]]

wsdiff  
image diff  
nbstirpout  
iadd  
extra worktree dir  




# The Communicative Value of Using Git Well – Math ∩ Programming      [[git]]

    I’ve written up my ideas, under the name ‘Literate Git’, at https://github.com/bennorth/literate-git if you’re interested.
    The tool I wrote turns a structured git history into an interactive web page.
    There’s an example there of how the ideas might work in a tutorial setting.
    After I gave a talk on this work, one of the people in the audience tried it with the Haskell LLVM tutorial: https://lukelau.me/kaleidoscope/




# `[2019-08-02]` git - How do I remove a submodule? - Stack Overflow      [[git]]

<https://stackoverflow.com/questions/1260748/how-do-i-remove-a-submodule/21211232#21211232>  

    git rm the_submodule
    rm -rf .git/modules/the_submodule




# `[2019-12-11]` git reflog expire &#x2013;expire=now &#x2013;all && git gc &#x2013;prune=now &#x2013;aggressive      [[github]]




# `[2019-05-10]` git rebase &#x2013;committer-date-is-author-date  &#x2013;autostash HEAD~1      [[git]]




# `[2020-06-08]` [Learn to change history with git rebase!](https://git-rebase.io/)




# `[2018-11-28]` extraction - How to extract one file with commit history from a git repo with index-filter & co - Stack Overflow      [[git]]

<https://stackoverflow.com/questions/7375528/how-to-extract-one-file-with-commit-history-from-a-git-repo-with-index-filter/37037151>  

    git filter-branch --index-filter 'git read-tree --empty; git reset $GIT_COMMIT -- $your $files $here' -- --all --




## `[2019-04-10]` set up git project commmand




# `[2020-07-12]` [- GitHub + why do we centralize issues, documents for a **distributed** version&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23805931)

    for an academic treatment of the defects in Git read: What's Wrong with Git? A Conceptual Design Analysis S. Perez De Rosso and D. Jackson. In Proceedings of the 2013 ACM International Symposium on New Ideas, New Paradigms, and Reflections on Programming & Software (Onward! 2013) 




# `[2018-01-01]` detect file type changes      [[git]]

    for r in *; do pushd $r; git whatchanged | grep "\.\.\..T"; popd; done




# git ssh debugging      [[git]] [[ssh]]

    GIT_SSH_COMMAND='ssh -v' git fetch




# `[2021-01-11]` [How to keep your Git history clean with interactive rebase | GitLab](https://about.gitlab.com/blog/2020/11/23/keep-git-history-clean-with-interactive-rebase/)




# `[2020-11-16]` [Why Git blame sucks for understanding WTF code (and what you should use instead) | Lobsters](https://lobste.rs/s/in8vp4/why_git_blame_sucks_for_understanding_wtf)

    For archeology I really love git gui blame despite its dated UI




# `[2019-07-21]` git - How do I remove a submodule? - Stack Overflow <https://stackoverflow.com/questions/1260748/how-do-i-remove-a-submodule/7646931#7646931>      [[git]]

    he majority of answers to this question are outdated, incomplete, or unnecessarily complex.
    
    A submodule cloned using git 1.7.8 or newer will leave at most four traces of itself in your local repo. The process for removing those four traces is given by the three commands below:

