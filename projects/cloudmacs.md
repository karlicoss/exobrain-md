
# Table of Contents

-   [`[2019-09-10]` right, I guess just start with few screenshots. Ideally need a proper demo playground&#x2026;](#rghtgssjststrtwthfwscrnshtsdllyndprprdmplygrnd) 
-   [mmm. might be abandoned? https://github.com/yudai/gotty/issues/258](#mmmmghtbbndndsgthbcmydgttysss) 
-   [record a demo?](#rcrddm) 
    -   [just think about a good short script and evaluate it?](#jstthnkbtgdshrtscrptndvltt) [[cloudmacs]]
-   [can build in docker compose?](#cnbldndckrcmps) [[cloudmacs]]
-   [memory footprint sucks. perhaps need to compile without gui or something?](#mmryftprntscksprhpsndtcmplwthtgrsmthng) [[cloudmacs]]
-   [Ttyd ?](#ttyd) 
-   [use minimal package, without x11?](#smnmlpckgwthtx) 
-   [big problem is that all of them are trying to mix hosting files and  editing.](#bgprblmsthtllfthmrtryngtmxhstngflsnddtng) [[cloudmacs]] [[toblog]] [[interop]]
-   [gotty-docker](#gttydckr) [[docker]]
-   [`[2019-09-10]` add a guide on customizing? e.g. suggest to build their own docker image with cloned spacemacs?](#ddgdncstmznggsggsttbldthrwndckrmgwthclndspcmcs) 
-   [demonstrate org-drill on one of my files?](#dmnstrtrgdrllnnfmyfls) 
-   [`[2019-09-10]` shit, 7001 seems to be occupied by nxnode or something](#shtsmstbccpdbynxndrsmthng) 
-   [dockerized over http](#dckrzdvr) 
    -   [`[2019-09-10]` and while vim navigation is doable, TODO links to the package](#ndwhlvmnvgtnsdbltdlnkstthpckg) 
-   [If I dockerize it, could post about it&#x2026;](#fdckrztcldpstbtt) [[toblog]] [[emacs]]
-   [feedback](#fdbck) 
    -   [`[2019-11-26]` Cloudmacs: access your Emacs in browser | Hacker News  https://news.ycombinator.com/item?id=21633149#21635348](#cldmcsccssyrmcsnbrwsrhckrnwssnwsycmbntrcmtmd) 
    -   [`[2019-11-26]` Cloudmacs: access your Emacs in browser | Hacker News  https://news.ycombinator.com/item?id=21633149#21635348](#cldmcsccssyrmcsnbrwsrhckrnwssnwsycmbntrcmtmd) 
    -   [`[2019-11-26]` Cloudmacs: access your Emacs in browser | Hacker News https://news.ycombinator.com/item?id=21633149#21635495](#cldmcsccssyrmcsnbrwsrhckrnwssnwsycmbntrcmtmd) 
-   [`[2019-10-27]` [karlicoss/cloudmacs] Emacs without X (#2) - karlicoss@gmail.com - Gmail](#krlcsscldmcsmcswthtxkrlcssgmlcmgml) 
-   [Related](#rltd) [[emacs]] [[infra]]

Emacs in the cloud <https://beepb00p.xyz/cloudmacs.html>  




# `[2019-09-10]` right, I guess just start with few screenshots. Ideally need a proper demo playground&#x2026;




# mmm. might be abandoned? <https://github.com/yudai/gotty/issues/258>




# record a demo?





## just think about a good short script and evaluate it?      [[cloudmacs]]




# can build in docker compose?      [[cloudmacs]]

ttrss-docker-compose/docker-compose.yml  

    app:
      build:
        context:
          ./app
        args:
          - OWNER_UID=${OWNER_UID}
          - OWNER_GID=${OWNER_GID}
      restart: unless-stopped
      environment:




# memory footprint sucks. perhaps need to compile without gui or something?      [[cloudmacs]]

tried gc &#x2013; didn't help  




# Ttyd ?

    I‘m using ttyd (https://github.com/tsl0922/ttyd) behind an nginx reverse proxy with client certificates. This gives me access from locations where ports other than https are blocked.




# use minimal package, without x11?




# big problem is that all of them are trying to mix hosting files and  editing.      [[cloudmacs]] [[toblog]] [[interop]]

editing could be on JS.  
interfaces are hard, and replicating the whole emacs frontend logic on JS is some massive thankless job  
however you lose all your keybindings etc.  




# gotty-docker       [[docker]]

compose file doesn't declare services <https://github.com/hyeonsangjeon/gotty-docker/blob/master/docker-compose.yml>  




# `[2019-09-10]` add a guide on customizing? e.g. suggest to build their own docker image with cloned spacemacs?




# demonstrate org-drill on one of my files?




# `[2019-09-10]` shit, 7001 seems to be occupied by nxnode or something




# dockerized over http

    I've updated [Filestash](https://github.com/mickael-kerjean/filestash) and somehow broke my Dropbox connection to the directory with org-mode notes, which rendered it useless for me. I'm also moving from Dropbox to Syncthing, so was planning to abandon Filestash anyway as it doesn't allow local files, only ftp, git etc.
    So before trying to support local directories in Filestash or setting up ftp server for the sole purpose of getting access of org files I though that I could try forwarding terminal with Emacs over http. Long story short, I found [emacs Docker image](https://github.com/JAremko/docker-emacs), hacked it a bit TODO gotty and TODO map emacs config and notes.
    I've seen [browsermax](https://github.com/JAremko/browsermax), but Dockerfile is quite complicated, looks like they are trying to use X11 for some reason, whereas I'd be perfectly happy with `emacsclient --tty`.
    Downside would be that it's not so convenient on mobile, but I tend to use Orgzly
    Only keyboard, which is not a limitation for me though.




## `[2019-09-10]` and while vim navigation is doable, TODO links to the package

it's hard to reinvent all the amazing emacs packages and features I'm used to: nerdtree, helm, refile, swoop, agenda, org-drill etc.  
not that elisp is superiour to JS, but reimplementing everything is going to be extremely hard  

Usecases:  

-   public computers where you can't or don't want to install emacs
-   demonstrating emacs packages?




# If I dockerize it, could post about it&#x2026;      [[toblog]] [[emacs]]

Think about mobile though  




# feedback 





## `[2019-11-26]` Cloudmacs: access your Emacs in browser | Hacker News  <https://news.ycombinator.com/item?id=21633149#21635348>

    Although a section explaining how to build container that runs as non-root user in the first place (even though it requires modifying Dockerfile, I think) would be useful, so I'll add it, thanks!




## `[2019-11-26]` Cloudmacs: access your Emacs in browser | Hacker News  <https://news.ycombinator.com/item?id=21633149#21635348>

    suppose the GUI analog to gotty is Apache Guacamole, which should run emacs fine (along with most anything else).




## `[2019-11-26]` Cloudmacs: access your Emacs in browser | Hacker News <https://news.ycombinator.com/item?id=21633149#21635495>

    However you got me thinking: do you know any emacsclient implementations that run purely in browser? Presumably that would be not that hard to implement and will make more sense.




# `[2019-10-27]` [karlicoss/cloudmacs] Emacs without X (#2) - karlicoss@gmail.com - Gmail

    Noticed one of your todos suggested building emacs without GUI as a way to reduce the docker layer.
    Below are the instructions on how to configure and build emacs from source without images and X features

<https://gist.github.com/danielrmeyer/35702082b07d5eb75f3754ce8985e907>  




# Related       [[emacs]] [[infra]]

