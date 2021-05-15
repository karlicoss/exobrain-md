
# Table of Contents

-   [`[2019-11-03]` Why Create a New Unix Shell?](#whycrtnwnxshll) 
-   [`[2020-02-21]` Ambitions for a Unix Shell | Hacker News](#mbtnsfrnxshllhckrnws) 
-   [`[2018-05-09]` comparing databases](#cmprngdtbss) [[shell]] [[sqlite]]
-   [`[2019-08-26]` Seven God-Like Bash History Shortcuts You Will Actually Use | Lobsters](#svngdlkbshhstryshrtctsywllctllyslbstrs) 
-   [`[2020-04-15]` The first two statements of your BASH script should be…](#sshshbntllthfrsttwsttmntstwsttmntsfyrbshscrptshldb) 
-   [`[2020-05-16]` Nushell | A new type of shell.](#swwwnshllshnshllnwtypfshll) [[shell]] [[malleable]]
    -   [`[2020-05-16]` about | Nushell](#swwwnshllshbthtmlbtnshll) 





# `[2019-11-03]` Why Create a New Unix Shell?

<https://www.oilshell.org/blog/2018/01/28.html>  




# `[2020-02-21]` Ambitions for a Unix Shell | Hacker News

<https://news.ycombinator.com/item?id=22150603>  

    Thanks for the support! Since I may not get to those blog posts in a timely fashion, here's a little outline (and maybe this comment will form the seed of them)




# `[2018-05-09]` comparing databases      [[shell]] [[sqlite]]

One possibility is to use the sqlite3 command line client to export both databases and then diff the output. For example,  

    sqlite3 first.sqlite  .dump >first.dump
    sqlite3 second.sqlite .dump >second.dump
    diff first.dump second.dump




# `[2019-08-26]` Seven God-Like Bash History Shortcuts You Will Actually Use | Lobsters

<https://lobste.rs/s/l2fk5f/seven_god_like_bash_history_shortcuts_you>  




# `[2020-04-15]` [The first two statements of your BASH script should be…](https://ashishb.net/all/the-first-two-statements-of-your-bash-script-should-be/)

    #!/usr/bin/env bash
    set -euo pipefail
    The first statement is a Mac, GNU/Linux, and BSD portable way of finding the location of the bash interpreter. The second statement combines




# `[2020-05-16]` [Nushell | A new type of shell.](https://www.nushell.sh/)      [[shell]] [[malleable]]





## `[2020-05-16]` [about | Nushell](https://www.nushell.sh/about.html)

    dditionally, commands can output structured data (you can think of this as a third kind of stream). Commands that work in the pipeline fit into one of three categories:

