
# Table of Contents

-   [related](#rltd) 
    -   [.](#574_690) [[infra]]
    -   [.](#690_806) [[offline]]
    -   [.](#806_922) [[selfhosted]]
    -   [.](#922_1038) [[cloud]]
-   [Syncthing](#syncthng) [[syncthing]]
-   [Dropbox](#drpbx) [[dropbox]]
-   [Nextcloud](#nxtcld) 
-   [MEGA](#mg) 
-   [Seafile](#sfl) 
    -   [try android client](#tryndrdclnt) 
-   [misc](#msc) 
    -   [spideroak](#spdrk) 
    -   [OneDrive is accessible through third-party scripts](#ndrvsccssblthrghthrdprtyscrpts) 
    -   [InSync offers unofficial Google Drive Linux support (for a fee)](#nsyncffrsnffclggldrvlnxspprtfrf) 

Continuous sync of my data and information is a biggie for me.  

-   first, I've always had one desktop/big sturdy laptop and one small portable for travel/coffee shops/etc
-   second, I need to be able to access information on my phone, when I may not have good network (or any)

Eventual sync (e.g. via Git) might be fine for personal wiki.  
For todo-list or just random documents, however, I really don't want to have this overhead of thinking whether I need to do some extra work in order to sync.  




# related 





## .       [[infra]]




## .       [[offline]]




## .       [[selfhosted]]




## .       [[cloud]]




# Syncthing       [[syncthing]]

I'm using it at the moment, and it works great.  

pros:  

-   uses filesystem
-   opn source, can be selfhosted
-   decentralized, no need for 'main' device

cons:  

-   no web interface

on Android: [Syncthing-Fork](https://play.google.com/store/apps/details?id=com.github.catfriend1.syncthingandroid) is better than the original Android app.  
  [Some differences](https://github.com/Catfriend1/syncthing-android#major-enhancements-in-this-fork-are):  

-   "Battery eater" problem is fixed
-   UI explains why syncthing is running or not.
-   Individual sync conditions can be applied per device and per folder




# Dropbox       [[dropbox]]

I stopped using it in favor of Syncthing, info might be a bit outdated (circa 2019?). If you don't want  

pros:  

-   uses filesystem
-   has revision history, so you can restore deleted files

cons:  

-   apparently symlink handling is quite bad&#x2026; <http://www.paulingraham.com/dropbox-and-symlinks.html>  
    possible solution: do not point to stuff under dropbox directly, instead make a dir like dropbox-links and point there?

on Android: [dropsync](https://play.google.com/store/apps/details?id=com.ttxapps.dropsync) is nice  




# Nextcloud 

It seems to be more like google services (docs/contacts/maps/etc) rather than just file syncing. Still haven't tried it myself though.  

Nexcloud is a fork of Owncloud (the latter has gone enterprise or something). Apparently it's much more open source  

pros:  

-   can replace google services #degoogle  
    e.g. [maps](https://apps.nextcloud.com/apps/maps)
-   open source, can be selfhosted

cons:  

-   [can mount as a filesystem](https://ownyourbits.com/2017/04/18/different-ways-to-access-your-nextcloud-files), but it's not a primary interface
-   centralized, requires a 'main' server
-   ???




# MEGA 

pros:  

-   ???

cons:  

-   symlinks doesn't work? (or WIP?)
-   closed source
-   centralized




# Seafile 

Dind't end up using it, so in my understanding it's kinda like Dropbox?  

pros:  

-   open source
-   delta sync, headless, dedup, selective encryption

cons:  

-   not distributed, requires a running server

-   <https://neowwayyuh.wordpress.com/2015/11/30/seafile-vs-syncthing>




## try android client

<https://github.com/haiwen/seadroid/issues/502>  
mm, only can access, can't sync as dropsync or syncthing would :(  
use webdav syncer as a workaround? <https://github.com/haiwen/seadroid/issues/502#issuecomment-286056463>  




# misc 





## spideroak 

apparently sync is weird, cluncy client  
<https://www.reddit.com/r/privacytoolsIO/comments/84kktv/thoughts_on_spideroak/>  




## OneDrive is accessible through third-party scripts




## InSync offers unofficial Google Drive Linux support (for a fee)

