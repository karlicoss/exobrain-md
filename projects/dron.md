
# Table of Contents

-   [related](#rltd) [[infra]] [[cron]] [[systemd]]
-   [\* motivation](#mtvtn) 
    -   [`[2020-02-01]` Rethinking Cron](#rthnkngcrn) 
        -   [`[2020-02-29]` good wishlist for missing cron features](#gdwshlstfrmssngcrnftrs) 
    -   [hmm it's kind of nice that in cron you can embed snippets of code&#x2026; a bit harder in systemd](#hmmtskndfncthtncrnycnmbdsnpptsfcdbthrdrnsystmd) 
-   [\* improvements](#mprvmnts) 
    -   [`[2019-08-25]` maybe forbid creating pycache?](#mybfrbdcrtngpycch) 
    -   [I think I need to enable/start regardless changes; just in case](#thnkndtnblstrtrgrdlsschngsjstncs) 
    -   [managed view &#x2013; would be nice to display timers only; and a command on a keypress. like cron](#mngdvwwldbnctdsplytmrsnlyndcmmndnkyprsslkcrn) 
    -   [conflicting jobs, e.g. promnesia generator and db backer](#cnflctngjbsgprmnsgnrtrnddbbckr) 
    -   [create separate target (instead of timers.target)? that way it'd be less messy](#crtsprttrgtnstdftmrstrgtthtwytdblssmssy) 
    -   [jcu got lots of potentially useful stuff..](#jcgtltsfptntllysflstff) 
    -   [Wonder if there is a way to overview <span class="underline">all</span> systems job failures over past boot?](#wndrfthrswytvrvwllsystmsjbflrsvrpstbt) [[systemd]]
    -   [mode to confirm systemd files diff first?](#mdtcnfrmsystmdflsdfffrst) 
    -   [for running now &#x2013; show time it's been running for](#frrnnngnwshwtmtsbnrnnngfr) 
    -   [show desktop notification on failure](#shwdsktpntfctnnflr) 
-   [\* bugs](#bgs) 
    -   [shit, monitor is consuming quite a bit of CPU. should run less often I guess.. wonder if possible to only run when I look at it?](#shtmntrscnsmngqtbtfcpshldsswndrfpssbltnlyrnwhnlktt) 
    -   [next time should be local instead of utc&#x2026;](#nxttmshldblclnstdftc) 
    -   [might fail if manually disabled the timer?](#mghtflfmnllydsbldthtmr) 
    -   [`[2020-05-29]` I guess what I was confused about was that if the job is running simultaneouslyu to previous instance, it's silently not running](#gsswhtwscnfsdbtwsthtfthjbtprvsnstnctsslntlyntrnnng) 
        -   [`[2020-05-29]` wonder if could email on this!](#wndrfcldmlnths) 
-   [\* publicity](#pblcty) [[publish]]
    -   [lobsters maybe and elsewhere? when it gets a bit more mature](#lbstrsmybndlswhrwhntgtsbtmrmtr) 
    -   [post about it? really need a proper circleci test&#x2026;](#pstbttrllyndprprcrclctst) 
-   [\* readme/post amendemens?](#rdmpstmndmns) [[toblog]]
    -   [`[2020-03-18]` eh, I'm finding that copy paste in crontabs is not too bad as long as you align everything&#x2026;](#hmfndngthtcpypstncrntbssnttbdslngsylgnvrythng) 
    -   [`[2020-04-08]` it's easier to align in python, because of string concatenation](#tssrtlgnnpythnbcsfstrngcnctntn) 
    -   [motivation: crontabs are hard to keep under version control. if you got different on different machines, hard to reconcile](#mtvtncrntbsrhrdtkpndrvrsnfrntndffrntmchnshrdtrcncl) 
    -   [why](#why) 
    -   [simple frontend for Systemd,](#smplfrntndfrsystmd) 
-   [`[2020-01-18]` watchdog?](#wtchdg) [[systemd]]
-   [`[2020-02-01]` schedule python library](#sschdlrdthdcsnstblschdlpythnlbrry) 
-   [---------------------------------------](#7605_7688) 
-   [a perspective a year later?](#prspctvyrltr) [[dron]]
-   [hmm, managed status drops after reinstalling crontabs&#x2026; I guess, timers?](#hmmmngdsttsdrpsftrrnstllngcrntbsgsstmrs) 
-   [if there is an invalid systemd file, it fails to load state hence you have to fix manually](#fthrsnnvldsystmdfltflstldstthncyhvtfxmnlly) 
-   [`[2019-10-24]` to enable the systemd service you can run the following.](#tnblthsystmdsrvcycnrnthfllwng) [[systemd]]
-   [`[2021-02-24]` linux - Proper way to use OnFailure in systemd - Unix & Linux Stack Exchange](#snxstckxchngcmqstnsprprwynflrnsystmdnxlnxstckxchng) [[dron]]
-   [`[2020-01-28]` arch linux - systemd: cpu usage of services - Super User](#ssprsrcmqstnssystmdcpsgfshlnxsystmdcpsgfsrvcssprsr) 
-   [`[2020-01-28]` systemd - systemctl status not showing CPU/Memory usage? - Ask Ubuntu](#sskbntcmqstnssystmctlsttslsttsntshwngcpmmrysgskbnt) 
-   [`[2020-01-26]` Systemd: How to make two services mutually exclusive but run both? - Super User](#ssprsrcmqstnssystmdhwtmktvcsmtllyxclsvbtrnbthsprsr) [[systemd]]
-   [`[2020-01-26]` systemd.service https://www.freedesktop.org/software/systemd/man/systemd.service.html#TimeoutStartSec=](#systmdsrvcswwwfrdsktprgsfmnsystmdsrvchtmltmtstrtsc) 
-   [`[2020-01-28]` systemd-analyze https://www.freedesktop.org/software/systemd/man/systemd-analyze.html](#systmdnlyzswwwfrdsktprgsftwrsystmdmnsystmdnlyzhtml) 
-   [using fzf to start service](#sngfzftstrtsrvc) 
-   [`[2020-01-28]` systemd-cgtop](#swwwfrdsktprgsftwrsystmdmnsystmdcgtphtmlsystmdcgtp) 
-   [`[2020-05-04]` systemd, 10 years later: a historical and technical retrospective](#sblgdrkndgynttchnlgyndxhtltrhstrclndtchnclrtrspctv) 
-   [`[2020-05-29]` ok, so timeouts via RuntimeMaxSec work as expected](#kstmtsvrntmmxscwrksxpctd) [[systemd]]
-   [dron: one year later](#drnnyrltr) [[dron]] [[toblog]]
-   [bug: try stoping an active timer with systemctl explicitly; it will be displayed as some weird big number (should be 'never')](#bgtrystpngnctvtmrwthsystmsplydssmwrdbgnmbrshldbnvr) 
-   [feature: for 'next' if the date is today, hide it](#ftrfrnxtfthdtstdyhdt) 
-   [`[2021-04-18]` [QUESTION] Why is \`systemd-email\` so complex ? · Issue 16 · karlicoss/dron](#sgthbcmkrlcssdrnsssqstnwhsystmdmlscmplxsskrlcssdrn) [[dron]]
-   [systemd-email &#x2013; need full path to make sure it won't fail to deliver email..](#systmdmlndfllpthtmksrtwntfltdlvrml) [[dron]]

Motivating blog post: <https://beepb00p.xyz/scheduler.html>  

Github project: <https://github.com/karlicoss/dron>  




# related       [[infra]] [[cron]] [[systemd]]




# \* motivation

mostly in the blog post, some extra links there too  




## `[2020-02-01]` Rethinking Cron

<https://adam.herokuapp.com/past/2010/4/13/rethinking_cron>  

    Rethinking Cron




### `[2020-02-29]` good wishlist for missing cron features




## hmm it's kind of nice that in cron you can embed snippets of code&#x2026; a bit harder in systemd




# \* improvements





## `[2019-08-25]` maybe forbid creating pycache?




## I think I need to enable/start regardless changes; just in case




## managed view &#x2013; would be nice to display timers only; and a command on a keypress. like cron




## conflicting jobs, e.g. promnesia generator and db backer

maybe there should be multiple tags? if two jobs got same tags, they can't run at the same time  
implemented via flocks on files named same as tags  




## create separate target (instead of timers.target)? that way it'd be less messy




## jcu got lots of potentially useful stuff..

    -t --identifier=STRING     Show entries with the specified syslog identifier
     -p --priority=RANGE        Show entries with the specified priority




## Wonder if there is a way to overview <span class="underline">all</span> systems job failures over past boot?      [[systemd]]




## mode to confirm systemd files diff first?




## for running now &#x2013; show time it's been running for




## show desktop notification on failure




# \* bugs





## shit, monitor is consuming quite a bit of CPU. should run less often I guess.. wonder if possible to only run when I look at it?

-   `[2021-01-25]` ugh. did some work, but it seems that it's just bus communication that still takes cpu and it's sort of inevitable?




## next time should be local instead of utc&#x2026;




## might fail if manually disabled the timer?

    Traceback (most recent call last):
      File "/home/karlicos/.local/bin/dron", line 11, in <module>
        load_entry_point('dron', 'console_scripts', 'dron')()
      File "/code/dron/dron.py", line 1168, in main
        cmd_monitor(params)
      File "/code/dron/dron.py", line 966, in cmd_monitor
        _cmd_monitor(managed, params=params)
      File "/code/dron/dron.py", line 849, in _cmd_monitor
        [service, timer] = gr
    ValueError: not enough values to unpack (expected 2, got 1)




## `[2020-05-29]` I guess what I was confused about was that if the job is running simultaneouslyu to previous instance, it's silently not running





### `[2020-05-29]` wonder if could email on this!




# \* publicity      [[publish]]





## lobsters maybe and elsewhere? when it gets a bit more mature




## post about it? really need a proper circleci test&#x2026;




# \* readme/post amendemens?      [[toblog]]





## `[2020-03-18]` eh, I'm finding that copy paste in crontabs is not too bad as long as you align everything&#x2026;




## `[2020-04-08]` it's easier to align in python, because of string concatenation

compare:  

    export_jobs = [
         job(at('02:08'), arctee(backups / 'feedbin'   /   'feedbin_{utcnow}.json', '--', 'python3.7', soft / 'backup/misc/feedbin.py'            ), unit_name='export-feedbin'),
         job(at('01:07'), arctee(backups / 'myshows'   /   'myshows_{utcnow}.json', '--', 'python3.7', soft / 'backups/myshows/myshows_backup.py' ), unit_name='export-myshows'),
         job(at('01:08'), arctee(backups / 'goodreads' / 'goodreads_{utcnow}.json', '--', 'python3.7', soft / 'backups/myshows/myshdows_backup.py'), unit_name='export-myshows'),
    ]

vs  

    0     0  * * *          $K -s "backup-goodreads"       --low            -- arctee      '/backups/goodreads/goodreads_{utcnow}.xml'           -- /soft/backup/goodrexport/run
    01   01  * * *          $K -s 'backup-pinboard'        --low -c         -- arctee      '/backups/pinboard/bookmarks_{utcnow}.json'           -- /soft/backup/pinbexport/run
    05   01  * * *          $K -s 'backup-lastfm'          --low -c         -- arctee      '/backups/lastfm/lastfm_{utcnow}.json'                -- python3.7 /soft/backup/lastfm/lastfm_backup.py
    07   01  * * *          $K -s "backup-spotify"         --low -c         -- arctee      '/backups/spotify/spotify_{utcnow}.json'              -- /soft/backup/spotify/backup




## motivation: crontabs are hard to keep under version control. if you got different on different machines, hard to reconcile




## why 

-   running custom jobs is easier
-   you can just start any jobs (+autocomplete)




## simple frontend for Systemd,

Not frontend, generator?  




# `[2020-01-18]` watchdog?      [[systemd]]

<https://www.freedesktop.org/software/systemd/man/systemd.service.html>  

    WatchdogSec=
        Configures the watchdog timeout for a service. The watchdog is activated when the start-up is completed. The service must call sd_notify(3) regularly with "WATCHDOG=1" (i.e. the "keep-alive ping")




# `[2020-02-01]` [schedule python library](https://schedule.readthedocs.io/en/stable/)

nope, just a completely custom scheduler, definitely not ideal  




# --------------------------------------- 




# a perspective a year later?      [[dron]]

For dron, thinking about it a year later, a large chunk of the convenience in this dron tool would probably be from  

-   allowing multiple services/timers in the same file (and then splitting them up in the actual systemd files)
-   allowing a different format (something more yaml-like) to make it possible to align jobs vertically. Then it's even fine not to have a general purpose language &#x2013; much easier to keep copypasta if you can block edit it




# hmm, managed status drops after reinstalling crontabs&#x2026; I guess, timers?




# if there is an invalid systemd file, it fails to load state hence you have to fix manually

and impossible to fix. e.g. add some garbage to onCalendar and try applying  




# `[2019-10-24]` to enable the systemd service you can run the following.      [[systemd]]

    systemctl --user enable --now matrixcli




# `[2021-02-24]` [linux - Proper way to use OnFailure in systemd - Unix & Linux Stack Exchange](https://unix.stackexchange.com/questions/441575/proper-way-to-use-onfailure-in-systemd/441662#441662)      [[dron]]

    In the code you run at ExecStopPost=, you can use one of $SERVICE_RESULT, $EXIT_CODE or $EXIT_STATUS to determine the failure condition and act accordingly. See the documentation on those environment variables to check which one is appropriate for you.

hmm can run this on success  




# `[2020-01-28]` [arch linux - systemd: cpu usage of services - Super User](https://superuser.com/questions/1060670/systemd-cpu-usage-of-services)

    If you enabled the cpuacct cgroup subgroup in the kernel. You can try systemd-cgtop to identify which systemd service causes high cpu usage.




# `[2020-01-28]` [systemd - systemctl status not showing CPU/Memory usage? - Ask Ubuntu](https://askubuntu.com/questions/901075/systemctl-status-not-showing-cpu-memory-usage)

    CPUAccounting = yes
    MemoryAccounting = yes




# `[2020-01-26]` [Systemd: How to make two services mutually exclusive but run both? - Super User](https://superuser.com/questions/1492025/systemd-how-to-make-two-services-mutually-exclusive-but-run-both)      [[systemd]]




# `[2020-01-26]` systemd.service <https://www.freedesktop.org/software/systemd/man/systemd.service.html#TimeoutStartSec>=

wonder if this is useful wrt to dependencies and conflicts  




# `[2020-01-28]` systemd-analyze <https://www.freedesktop.org/software/systemd/man/systemd-analyze.html>

    systemd-analyze verify FILE...
    The following errors are currently detected:
        unknown sections and directives,
        missing dependencies which are required to start the given unit,
        man pages listed in Documentation= which are not found in the system,
        commands listed in ExecStart= and similar which are not found in the system or not executable.




# using fzf to start service

    systemctl --user start $(ls ~/.config/systemd/user/ | fzf)




# `[2020-01-28]` [systemd-cgtop](https://www.freedesktop.org/software/systemd/man/systemd-cgtop.html)

    systemd-cgtop — Show top control groups by their resource usage

wonder if I could use it?  




# `[2020-05-04]` [systemd, 10 years later: a historical and technical retrospective](https://blog.darknedgy.net/technology/2020/05/02/0/index.html)

    Yes, we currently handle socket-triggered, bus-triggered, file-triggered, mount-triggered, automount-triggered, device-triggered




# `[2020-05-29]` ok, so timeouts via RuntimeMaxSec work as expected      [[systemd]]




# dron: one year later      [[dron]] [[toblog]]

what worked:  

-   systemd integration is excellent, can hack on systemd to experiment, and then reapply changes properly via dron
-   while mailing is sort of hacky, don't think it has ever let me down

what didn't work  

-   barely used dron edit, mainly dron apply

what to improve:  

-   speed up dron apply?
-   monitor too slow?




# bug: try stoping an active timer with systemctl explicitly; it will be displayed as some weird big number (should be 'never')




# feature: for 'next' if the date is today, hide it




# `[2021-04-18]` [[QUESTION] Why is \`systemd-email\` so complex ? · Issue 16 · karlicoss/dron](https://github.com/karlicoss/dron/issues/16)      [[dron]]

    Hi ! I'm reading your sources with great interest, and i came out to systemd-email, and it looks like to me that the same output can be achieved with this single command: systemctl --user status myFailingUnit.service --lines 99999 -o cat
    Is it really equivalent ?




# systemd-email &#x2013; need full path to make sure it won't fail to deliver email..      [[dron]]

