
# Table of Contents

-   [related](#rltd) [[infra]]
-   [docker](#dckr) [[docker]]
    -   [`[2018-06-15]` `docker system prune` to cleanup](#dckrsystmprntclnp) 
    -   [`[2021-01-12]` figuring out what takes disk space  `docker images | awk '{print $3}' | xargs docker inspect | less`](#fgrngtwhttksdskspcdckrmgswkprntxrgsdckrnspctlss) [[docker]]
    -   [`[2021-02-12]` Docker compose port mapping - Stack Overflow](#sstckvrflwcmqstnsdckrcmpsdckrcmpsprtmppngstckvrflw) 
    -   [`[2021-04-14]` apt-get clean and other strategies for keeping image size small? · Issue 35 · rocker-org/rocker](#sgthbcmrckrrgrckrssssscmmrkpngmgszsmllssrckrrgrckr) [[docker]]
    -   [`[2021-05-02]` Attach and Detach from Docker Container | HowToProgram](#shwtprgrmxyzttchdtchdckrcddtchfrmdckrcntnrhwtprgrm) [[docker]] [[drill]]
-   [systemd](#systmd) [[systemd]]
    -   [debugging: `systemctl --failed`,  `journalctl`](#dbggngsystmctlfldjrnlctl) 
    -   [profiling: `systemd-analyze blame`](#prflngsystmdnlyzblm) 
-   [networking](#ntwrkng) [[network]]
    -   [who uses local port](#whsslclprt) 
    -   [testing if port is open](#tstngfprtspn) 
    -   [`[2020-06-15]` linux - Test if a port on a remote system is reachable (without telnet) - Super User](#ssprsrcmqstnststfprtnrmtstsystmsrchblwthttlntsprsr) 
-   [apt](#pt) 
    -   [install build dependencies: `sudo apt-get build-dep package`](#nstllblddpndncssdptgtblddppckg) 
-   [cron](#crn) [[cron]]
    -   [`[2018-02-26]` if cron fails to start a job, it will send the output to local mail](#fcrnflststrtjbtwllsndthtpttlclml) 
    -   [`[2018-05-10]` mail subject &#x2013; use bash comment operator](#mlsbjctsbshcmmntprtr) 
-   [sandboxing](#sndbxng) [[sandbox]]
    -   [docker is excellent for quick sandboxes (just use `ubuntu:latest` image or something)](#dckrsxcllntfrqcksndbxsjstsbntltstmgrsmthng) [[docker]]
    -   [`firejail` for network sandbox](#frjlfrntwrksndbx) [[network]] [[testing]]
-   [udev](#dv) [[udev]]
    -   [`udevadm info /dev/sdc2`](#dvdmnfdvsdc) 
    -   [`[2019-03-07]` when you update rules file `sudo udevadm control --reload-rules`](#whnypdtrlsflsddvdmcntrlrldrls) 
    -   [`[2019-03-07]` to trigger the target script `sudo udevadm trigger`](#ttrggrthtrgtscrptsddvdmtrggr) 
-   [`[2017-05-08]` Gateway 0.0.0.0 means that the subnet is link-local i.e. there is no gateway involved, the packets are delivered directly to the target](#gtwymnsthtthsbntslnklclthhpcktsrdlvrddrctlytthtrgt) [[network]]
-   [-----------------------------------------](#5121_5206) 
-   [`[2018-06-08]` Linux ignores the setuid bit on all interpreted executables (i.e. executables starting with a `#!` line).](#lnxgnrsthstdbtnllntrprtdxctblsxctblsstrtngwthln) 
-   [`[2020-01-29]` linux - How to make htop sort by PID](#ssprsrcmqstnshwtmkhtpsrtbypdlnxhwtmkhtpsrtbypd) 
-   [`[2020-01-24]` logs - View stdout/stderr of systemd service](#snxstckxchngcmqstnsvwstdtlgsvwstdtstdrrfsystmdsrvc) [[systemd]]
-   [`[2020-01-29]` How to read memory usage in htop? - Server Fault](#hwtrdmmrysgnhtpsrvrflt) [[drill]]
-   [`[2020-12-04]` linux - prevent system freeze/unresponsiveness due to swapping run away memory usage - Super User](#ssprsrcmqstnsprvntsystmfrssdtswppngrnwymmrysgsprsr) 
-   [`[2018-04-27]` guide to XKB](#smdmcmdmksmplhmblbtcmprhnsvgdtxkbfrlnxfdgdtxkb) 
-   [-------------------------------------------](#7142_7228) 
-   [`whereis` command](#whrscmmnd) [[habit]]





# related       [[infra]]




# docker       [[docker]]





## `[2018-06-15]` `docker system prune` to cleanup




## `[2021-01-12]` figuring out what takes disk space  `docker images | awk '{print $3}' | xargs docker inspect | less`      [[docker]]




## `[2021-02-12]` [Docker compose port mapping - Stack Overflow](https://stackoverflow.com/questions/35429837/docker-compose-port-mapping/46220742)

    If you want to bind to the redis port from your nodejs container you will have to expose that port in the redis container:
    
    version: '2'
    services:
      nodejs:
        build:
          context: .
          dockerfile: DockerFile
        ports:
          - "4000:4000"
        links:
          - redis
      redis:
        build:
          context: .
          dockerfile: Dockerfile-redis
        expose:
          - "6379"
    The expose tag will let you expose ports without publishing them to the host machine, but they will be exposed to the containers networks.




## `[2021-04-14]` [apt-get clean and other strategies for keeping image size small? · Issue 35 · rocker-org/rocker](https://github.com/rocker-org/rocker/issues/35#issuecomment-58944297)      [[docker]]

ok, so for debian/ubuntu images don't really need autoclean &#x2013; it's already run automatically  




## `[2021-05-02]` [Attach and Detach from Docker Container | HowToProgram](https://howtoprogram.xyz/2017/03/18/attach-detach-docker-container/)      [[docker]] [[drill]]

    In general, to detach from a Docker container and leave it running, we can use the CTRL-p CTRL-q key sequence.




# systemd       [[systemd]]





## debugging: `systemctl --failed`,  `journalctl`

logs &#x2013; for individual jobs you can see them via status (or sdj)  
presistent is not showing anythin by default?  




## profiling: `systemd-analyze blame`




# networking       [[network]]





## who uses local port

    sudo ss -tulpn | grep 5060
    sudo ss -anpt  | grep 8640




## testing if port is open

    netcat -l 5559

one the other machine  

    echo "TEST" | netcat host 5559




## `[2020-06-15]` [linux - Test if a port on a remote system is reachable (without telnet) - Super User](https://superuser.com/questions/621870/test-if-a-port-on-a-remote-system-is-reachable-without-telnet)

    Nice and verbose! From the man pages.
    Single port:
    nc -zv 127.0.0.1 80

testing if port is open  




# apt 





## install build dependencies: `sudo apt-get build-dep package`




# cron       [[cron]]





## `[2018-02-26]` if cron fails to start a job, it will send the output to local mail

    grep cron /var/log/syslog
    tail -f /var/log/syslog | grep cron




## `[2018-05-10]` mail subject &#x2013; use bash comment operator

    *:* TestJob; cron command

mind the space after colon!  




# sandboxing       [[sandbox]]





## docker is excellent for quick sandboxes (just use `ubuntu:latest` image or something)      [[docker]]




## `firejail` for network sandbox      [[network]] [[testing]]

-   doesn't require root!
-   `firejail --noprofile --net=none`




# udev       [[udev]]





## `udevadm info /dev/sdc2`




## `[2019-03-07]` when you update rules file `sudo udevadm control --reload-rules`




## `[2019-03-07]` to trigger the target script `sudo udevadm trigger`




# `[2017-05-08]` Gateway 0.0.0.0 means that the subnet is link-local i.e. there is no gateway involved, the packets are delivered directly to the target      [[network]]




# ----------------------------------------- 




# `[2018-06-08]` Linux ignores the setuid bit on all interpreted executables (i.e. executables starting with a `#!` line).

ok apparently setuid shell scripts are quite risky&#x2026;  




# `[2020-01-29]` [linux - How to make htop sort by PID](https://superuser.com/questions/275873/how-to-make-htop-sort-by-pid)

press > and select RES  




# `[2020-01-24]` [logs - View stdout/stderr of systemd service](https://unix.stackexchange.com/questions/20399/view-stdout-stderr-of-systemd-service)      [[systemd]]

    Note that using the standard logging mechanism like this will not create persistent logs by default. To do that, you'll need to create /var/log/journal, and then run sudo systemctl restart systemd-journald




# `[2020-01-29]` How to read memory usage in htop? - Server Fault      [[drill]]

<https://serverfault.com/questions/517483/how-to-read-memory-usage-in-htop>  

    Hide user threads (shift + H) and close the process tree view (F5), t




# `[2020-12-04]` [linux - prevent system freeze/unresponsiveness due to swapping run away memory usage - Super User](https://superuser.com/questions/1115983/prevent-system-freeze-unresponsiveness-due-to-swapping-run-away-memory-usage)

    If a process demands a lot of memory, the system moves all other process to the swap file. Including it seems, necessary processes like the X11 server or the terminal.




# `[2018-04-27]` [guide to XKB](https://medium.com/@damko/a-simple-humble-but-comprehensive-guide-to-xkb-for-linux-6f1ad5e13450)




# ------------------------------------------- 




# `whereis` command      [[habit]]

