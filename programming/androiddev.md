
# Table of Contents

-   [related](#rltd) [[android]]
-   [Android studio plugins](#ndrdstdplgns) [[setup]]
-   [Phone apps](#phnpps) 
-   [`[2015-11-20]` Why asynctasks are bad?](#whysynctsksrbd) 
-   [`[2016-04-06]` running strace on device](#rnnngstrcndvc) 
-   [debugging with adb](#dbggngwthdb) [[adb]]
    -   [Wireless adb:](#wrlssdb) 
    -   [Clearing the app data](#clrngthppdt) 
    -   [Start an activity](#strtnctvty) 
    -   [Start service](#strtsrvc) 
    -   [Debug activity/service starts](#dbgctvtysrvcstrts) 
    -   [View activity stack:](#vwctvtystck) 
    -   [Run certain tests:](#rncrtntsts) 
-   [`[2019-08-28]` I made something to turn any mobile website into an iPhone app&#x2026; /r/webdev](#srddtcmrwbdvcmmntsllbfmdstrnnymblwbstntnphnpprwbdv) [[android]]
-   [`[2019-08-28]` What is the difference between PhoneGap and Ionic? /r/learnprogramming](#srddtcmrlrnprgrmmngcmmntsbtwnphngpndncrlrnprgrmmng) [[android]]
-   [`[2019-08-28]` Do people use plain Cordova to build apps ? Or do most people use it in a framework like Ionic or PhoneGap /r/javascript](#srddtcmrjvscrptcmmntsfcgcnfrmwrklkncrphngprjvscrpt) [[android]]
-   [`[2019-08-28]` PhoneGap/Cordova vs Ionic vs React Native /r/webdev](#srddtcmrwbdvcmmntsdnnzphnhngpcrdvvsncvsrctntvrwbdv) 
-   [`[2019-08-18]` JStumpp/awesome-android: A curated list of awesome Android packages and resources.](#jstmppwsmndrdcrtdlstfwsmndrdpckgsndrsrcs) 
-   [`[2019-10-11]` fastlane/fastlane: 🚀 The easiest way to automate building and releasing your iOS and Android apps](#fstlnfstlnthsstwyttmtbldngndrlsngyrsndndrdpps) [[androiddev]]
-   [`[2019-06-12]` udev - Android adb no permission - Ask Ubuntu](#dvndrddbnprmssnskbnt) [[adb]]
-   [`[2019-12-27]` How to Debug a Third Party Android App | Lobsters https://lobste.rs/s/vlawsw/how\_debug\_third\_party\_android\_app](#hwtdbgthrdprtyndrdpplbstrsvlwswhwdbgthrdprtyndrdpp) 
-   [`[2021-01-11]` Allow using a different directory than Documents for local storage · Issue 999 · jonasoreland/runnerup](#sgthbcmjnsrlndrnnrpsssllwtsfrlclstrgssjnsrlndrnnrp) [[androiddev]]





# related       [[android]]




# Android studio plugins      [[setup]]

-   ADB Idea
-   Bash support
-   CheckStyle - IDEA
-   Drawable importer
-   Findbugs - IDEA
-   IdeaVim
-   Lombok
-   Markdown
-   Python support
-   Sqldelight
-   Teamcity




# Phone apps

-   Cheatdroid: shared prefs editor




# `[2015-11-20]` Why asynctasks are bad?

1.  AsyncTasks are not composable, To run two (or more) dependent asyncTasks you need to run one from another.
2.  Error handling needs boilerplate: To handle error in main thread you need to return null as result (and losing error information in onPostExecute), or wrap your result in some kind of Either, where you provide result or error
3.  AsyncTasks force you to handle result in main thread (even when it's intermediate result, and should not be handled in main thread yet)
4.  And of course Activity/Fragment lifecycle, but that's the point why loaders were introduced.




# `[2016-04-06]` running strace on device

    setenforce 0  # In Android 4.3 and later, if SELinux is enabled, strace will fail with "strace: wait: Permission denied"
    set `ps | grep zygote` ; strace -p $2 -f -tt -T -s 500 -o /sdcard/strace.txt




# debugging with adb      [[adb]]





## Wireless adb:

    adb shell netcfg




## Clearing the app data

    adb shell pm clear com.google.mail




## Start an activity

    adb shell am start PACKAGE_NAME/ACTIVITY_IN_PACKAGE
    adb shell am start PACKAGE_NAME/FULLY_QUALIFIED_ACTIVITY
    
    # example
    adb shell am start -n com.growingwiththeweb.example/.MainActivity
    adb shell am start -n com.growingwiththeweb.example/com.growingwiththeweb.example.MainActivity




## Start service

    adb shell am startservice -n "ru.yandex.mail/com.yandex.mail.service.AbookCacheService"




## Debug activity/service starts

    logcat -b events | grep "google.mail"




## View activity stack:

    adb shell dumpsys activity activities | sed -En -e '/Stack #/p' -e '/Running activities/,/Run #0/p'




## Run certain tests:

    adb shell am instrument -w -e class com.yandex.mail.tests.FolderTest,com.yandex.mail.tests.MessageListTest ru.yandex.mail.test/com.yandex.mail.UiTestsRunner




# `[2019-08-28]` [I made something to turn any mobile website into an iPhone app&#x2026;](https://reddit.com/r/webdev/comments/3allbf/i_made_something_to_turn_any_mobile_website_into/csdvqf4/) /r/webdev      [[android]]

    Why you didn't use the tags?
    ><meta name="apple-mobile-web-app-capable" content="yes">
    ><meta name="apple-mobile-web-app-status-bar-style" content="black">
    It works amazingly with Chrome: https://developer.chrome.com/multidevice/android/installtohomescreen
    You get the App icon on your screen, full screen, etc!




# `[2019-08-28]` [What is the difference between PhoneGap and Ionic?](https://reddit.com/r/learnprogramming/comments/4cah35/what_is_the_difference_between_phonegap_and_ionic/d1gvba6/) /r/learnprogramming      [[android]]

    Ionic is just a UI.
    Think of all the UI peculiarities when you use your iPhone. Now imagine trying to hand roll all of that in CSS. Doable, but a real PITA. That's why Ionic was developed.
    Phone gap is a totally different thing and is what compiles your code into somethin iOS or android understands.




# `[2019-08-28]` [Do people use plain Cordova to build apps ? Or do most people use it in a framework like Ionic or PhoneGap](https://reddit.com/r/javascript/comments/4f5cgc/do_people_use_plain_cordova_to_build_apps_or_do/d262u2o/) /r/javascript      [[android]]

    Hello!
    Using cordova on it's own has grown out of fashion due to the amount of things you are required to set it up to make it look like a semi decent app. That said, there are those who still do that, but they likely have a suite of things they've developed over time to make use of it.
    Phonegap isn't a different framework though, it's the non open source version of Cordova that is marketed by Adobe.
    Ionic is the framework you'd most likely be looking, as they do provide a number of useful mobile components, and styles.
    You could also look into React Native, as the community is growing at a faster rate than Ionic did. It doesn't use Cordova at all, but rather the JavaScript runtime on iOS & Android to make use of the platforms' native UI components.




# `[2019-08-28]` [PhoneGap/Cordova vs Ionic vs React Native](https://reddit.com/r/webdev/comments/90dnnz/phonegapcordova_vs_ionic_vs_react_native/e2pp3rd/) /r/webdev

    Ionic is basically Cordova with Angular on top with a convenient CLI. In my experience Cordova apps tend to be laggy in the long run and the debugging process is relatively annoying when trying to debug native plugins (you have to build the app via xcode etc.). You should be aware that Cordova uses the web view to display the app. So it’s kinda like running a web page on your phone and trying to convince the user it’s a native app.
    React native on the other hand uses the native components of the OS. So it’s not a web view, which means your app will feel much smoother. The downside of react native is that it uses its own components on top of the native ones which makes it hard to reuse your frontend code to the extent you  could with a Cordova app.
    Personal opinion: In my opinion and based on my past experience I would go with react native if I had to choose a framework based on JavaScript.
    Hope this helps :)




# `[2019-08-18]` JStumpp/awesome-android: A curated list of awesome Android packages and resources.

<https://github.com/JStumpp/awesome-android#readme>  

    Development Alternatives




# `[2019-10-11]` fastlane/fastlane: 🚀 The easiest way to automate building and releasing your iOS and Android apps      [[androiddev]]

<https://github.com/fastlane/fastlane>  




# `[2019-06-12]` udev - Android adb no permission - Ask Ubuntu      [[adb]]

<https://askubuntu.com/questions/680591/android-adb-no-permission>  

    Change the USB mode in your phone to File Transfer. That's what worked for me.




# `[2019-12-27]` How to Debug a Third Party Android App | Lobsters <https://lobste.rs/s/vlawsw/how_debug_third_party_android_app>




# `[2021-01-11]` [Allow using a different directory than Documents for local storage · Issue 999 · jonasoreland/runnerup](https://github.com/jonasoreland/runnerup/issues/999)      [[androiddev]]

    The problem is scooped storage in newer Android versions. An app only has access to its specific directories.
    With older Android than 10 it is possible.
    This piece of code need to be changed when targeting Android 111 (before next fall) as getExternalStoragePublicDirectory() is not supported then.

