
# Table of Contents

-   [OpenBCI is best apparently?](#pnbcsbstpprntly) 
    -   [ganglion? https://shop.openbci.com/collections/frontpage/products/pre-order-ganglion-board?variant=13461804483 can do EEG, EMG, ECG](#gnglnsshppnbccmcllctnsfrnprrdrgnglnbrdvrntcndgmgcg) 
    -   [https://neurobb.com/t/is-there-really-no-affordable-user-friendly-neurofeedback-hardware-software-out-there/75](#snrbbcmtsthrrllynffrdblsrndlynrfdbckhrdwrsftwrtthr) 
    -   [https://www.youtube.com/watch?v=QIWswAOFp8w](#swwwytbcmwtchvqwswfpw) 
    -   [https://www.youtube.com/watch?v=agV1B2l-QLw](#swwwytbcmwtchvgvblqlw) 
    -   [print it youself: about 500$ =/](#prnttyslfbt) 
    -   [could try using 3d printer at work?](#cldtrysngdprntrtwrk) 
    -   [http://www.autodidacts.io/getting-started-with-openbci-a-tutorial-on-testing-troubleshooting-and-recording-ekg/](#wwwtddctsgttngstrtdwthpnbntstngtrblshtngndrcrdngkg) 
        -   [+ The OpenBCI arrives pre-assembled and tested, and is relatively straightforward for someone without previous bci experience to get started with — no soldering, hair-tearing, or midnight coding sessions need appl](#thpnbcrrvsprssmbldndtstdntrngrmdnghtcdngsssnsndppl) 
        -   [+ Finally, the OpenBCI’s output is far closer to clinical or research grade than most consumer or amateur systems: It has an excellent sample-rate (250 Hz), works with well-established processing and display software, and can be used with any electrodes with industry-standard “touchproof” connectors, so you aren’t stuck with the type it comes with.](#fnllythpnbcstptsfrclsrtclssyrntstckwththtyptcmswth) 
        -   [? use 32 but Which should you choose? In most cases, it probably doesn’t matter. If you’ve used Arduino before, the 8bit would be a good choice. Also, the Arduino community is quite active and helpful. The 32bit version is more powerful, which means that it can do more processing on the signal before it’s sent over bluetooth. If you plan on doing a lot of with tinkering with the code running on the OpenBCI itself, the 32bit version may be a better choice.](#sbtwhchshldychsnmstcsstprnbctslfthbtvrsnmybbttrchc) 
        -   [? need 10-20 paste?](#ndpst) 
        -   [? TODO how to secure electrodes](#tdhwtscrlctrds) 
    -   [- very little data on the internet and reddit.. unlikely to get any help if i buy it](#vrylttldtnthntrntndrddtnlklytgtnyhlpfbyt) 
    -   [eh. quite costy. so buy it, but ONLY after you consolidate all other sleep trackers so you could compare](#hqtcstysbytbtnlyftrycnsldtllthrslptrckrssycldcmpr) 
-   [Do you have fine control of your head and neck? If so then a headset with a gyro will be much better (Muse by InteraXon or Emotiv).](#dyhvfncntrlfyrhdndnckfsthrwllbmchbttrmsbyntrxnrmtv) 
-   [ultracortex: 3d printed](#ltrcrtxdprntd) 
-   [`[2018-07-15]` how are EMG and EEG different?](#hwrmgndgdffrnt) [[emg]]
-   [EMG?  how can it be used](#mghwcntbsd) [[emg]]
    -   [ok, so on reddit everyone claims relation between EMG and muscle activation is unclear](#ksnrddtvrynclmsrltnbtwnmgndmsclctvtnsnclr) 
    -   [in particular, it's hard to interpret signal correctly](#nprtclrtshrdtntrprtsgnlcrrctly) 
    -   [https://www.reddit.com/r/bodyweightfitness/comments/7x0jqq/\_/](#swwwrddtcmrbdywghtftnsscmmntsxjqq) 
    -   [devices](#dvcs) 
        -   [https://www.amazon.co.uk/ADVANCER-TECHNOLOGIES-Muscle-Sensor-MyoWare/dp/B018TIWR32/ref=sr\_1\_3?ie=UTF8&qid=1531258073&sr=8-3&keywords=EMG+sensor](#swwwmznckdvncrtchnlgsmscltwrrfsrtfqdsrkywrdsmgsnsr) 
        -   [https://shop.openbci.com/collections/frontpage/products/myoware-muscle-sensor?variant=29472011267](#sshppnbccmcllctnsfrntpgprdctsmywrmsclsnsrvrnt) 
        -   [https://www.amazon.co.uk/MyoWare-Muscle-Sensor-Development-Kit/dp/B01LX6MX4P/ref=sr\_1\_5?ie=UTF8&qid=1531258073&sr=8-5&keywords=EMG+sensor](#swwwmznckmywrmsclsnsrdvlpmxprfsrtfqdsrkywrdsmgsnsr) 
        -   [aliexpress?](#lxprss) 
-   [Neurosky?](#nrsky) 
    -   [? 1 channel](#chnnl) 
    -   [+ I did some fairly extensive testing of the Neurosky device while I was working on an app to analyze brainwave signals.](#ddsmfrlyxtnsvtstngfthnrskswrkngnnpptnlyzbrnwvsgnls) 
    -   [- pretty expensive on amazon :( about 150 GBP?](#prttyxpnsvnmznbtgbp) 
-   [Neuroonopen](#nrnpn) 
    -   [+ alarm LED and vibration](#lrmldndvbrtn) 
    -   [? Only four states are recognized though: awake, light sleep, REM sleep and deep sleep. [reddit]](#nlyfrsttsrrcgnzdthghwklghtslprmslpnddpslprddt) 
    -   [- I got it, doesn't do anything regarding helping you achieve polyphasic sleep which is the frigging reason of why I supported the kickstarter in the first place. [reddit]](#gttdsntdnythngrgrdnghlpngdthkckstrtrnthfrstplcrddt) 
    -   [- the hugest minus in my opinion: you can not zoom within your sleep graph. You can see that you fell into deep sleep approximately but you will never know at which hour exactly. This is fairly annoying.](#thhgstmnsnmypnnycnntzmwthtwhchhrxctlythssfrlynnyng) 
    -   [- no news from them](#nnwsfrmthm) 
-   [Emotiv https://www.emotiv.com/comparison/](#mtvswwwmtvcmcmprsn) 
    -   [emotiv insight is 200. If not emotiv, you'd be better off making your own for that price.](#mtvnsghtsfntmtvydbbttrffmkngyrwnfrthtprc) 
    -   [- I have not tried emotiv but I was put off by the $500 SDK. You are selling the device and want people to develop for your platform to extend it and you are charging them for the SDK??](#hvnttrdmtvbtwsptffbythsdkxtndtndyrchrgngthmfrthsdk) 
    -   [- raw data costs a lot](#rwdtcstslt) 
    -   [- have to use their software](#hvtsthrsftwr) 
-   [Muse band](#msbnd) [[buy]] [[qs]] [[meditation]]
    -   [xxx `[2018-07-15]`](#xxx) 
    -   [what's it composed of](#whtstcmpsdf) 
    -   [https://medium.com/pixeldreams/my-40-day-journey-into-meditation-with-muse-the-brain-sensing-headband-12e7b060c6fa](#smdmcmpxldrmsmydyjrnyntmdtnwthmsthbrnsnsnghdbndbcf) 
    -   [final decision: ok, the data is useful and I don't care that much about neurofeedback. instead, invest in proper openbci??](#fnldcsnkthdtssflnddntcrthtnrfdbcknstdnvstnprprpnbc) 
    -   [good review https://www.warrior.do/muse-headband-review/](#gdrvwswwwwrrrdmshdbndrvw) 
-   [mindflex toys??](#mndflxtys) 
-   [https://johnfawkes.com/becoming-superhuman-through-diy-brain-scanning/](#sjhnfwkscmbcmngsprhmnthrghdybrnscnnng) 
-   [bci](#bc) 
-   [`[2019-02-04]` neurable: Announcing the world’s first brain-computer interface for virtual reality](#nrblnnncngthwrldsfrstbrncmptrntrfcfrvrtlrlty) [[eeg]] [[vr]]
    -   [`[2019-02-15]` dunno, almost nothing on reddit, you can't buy it now etc. try again somewhat later&#x2026;](#dnnlmstnthngnrddtycntbytnwtctrygnsmwhtltr) 
-   [`[2019-01-24]` EEG-SMT - Open Source Hardware Board](#gsmtpnsrchrdwrbrd) [[eeg]]
-   [`[2019-01-27]` How to build a brain interface — and why we should connect our minds](#hwtbldbrnntrfcndwhywshldcnnctrmnds) [[eeg]]
-   [`[2019-02-24]` Somaxis EMG EKG EEG sensors – muscle, heart, brain, posture, activity](#smxsmgkggsnsrsmsclhrtbrnpstrctvty) 
-   [Some EEG stuff](#smgstff) 
    -   [`[2019-01-20]` BioShare.info](#bshrnf) 
    -   [`[2019-01-20]` Physiological Monitoring | HaB Direct](#physlgclmntrnghbdrct) 
    -   [`[2019-01-20]` BioHarness 3 Compression Shirts | HaB Direct](#bhrnsscmprssnshrtshbdrct) 
    -   [`[2019-01-20]` SnapECG Portable EKG Monitor, Handheld ECG Heart Rate Monitor for Smart Phone, Wireless Heart Performance Tracking without ECG Electrodes Required, Home Use Ekg Monitoring Devices for iPhone & Android: Amazon.co.uk: Sports & Outdoors](#snpcgprtblkgmntrhndhldcghcsfrphnndrdmzncksprtstdrs) 
    -   [`[2019-01-20]` EKG ECG Heart Rate Monitor: QardioCore Continuous Electrocardiograph ECG/EKG Mobile Machine - Wireless, Portable, Wearable Heart Monitoring Equipment - Bluetooth Mobile Digital Cardio Devices: Amazon.co.uk: Health & Personal Care](#kgcghrtrtmntrqrdcrcntnslctlcrddvcsmznckhlthprsnlcr) 
    -   [`[2019-01-20]` eMotion EMG | shop.bittium.com](#mtnmgshpbttmcm) [[emg]] [[qs]]
    -   [`[2019-01-20]` Bittium Faros - Bittium](#bttmfrsbttm) [[hr]]
    -   [`[2019-01-20]` My Baseline Network Physiology: 10 Days of EEG, EGG, EKG, CGM, Temperature, Activity and Food Logs - Quantified Self / Project Logs - Quantified Self Forum](#mybslnntwrkphyslgydysfgggtfdslfprjctlgsqntfdslffrm) [[qs]]
    -   [`[2019-01-20]` DS1922L-F5# Thermochron iButton [-40 to 85°C] - 8K Memory | iButtonLink](#dslfthrmchrnbttntckmmrybttnlnk) [[qs]]
    -   [`[2019-01-20]` MySignals - eHealth and Medical IoT Development Platform](#mysgnlshlthndmdcltdvlpmntpltfrm) [[qs]] [[gadget]]
    -   [`[2019-01-20]` Reliable wearable ECG - Quantified Self / Apps & Tools - Quantified Self Forum](#rlblwrblcgqntfdslfppstlsqntfdslffrm) [[hr]]
    -   [`[2019-01-20]` Firstbeat Firstbeat Bodyguard 2](#frstbtfrstbtbdygrd) [[hr]]
-   [`[2019-05-10]` New neural implant in trials /r/BrainMachineInterface](#srddtcmrbrnmchnntrfccmmntrlmplntntrlsrbrnmchnntrfc) [[bci]]
    -   [`[2019-05-12]` huh, pretty cool, electrod mesh injected via a vein right into the brain](#hhprttycllctrdmshnjctdvvnrghtntthbrn) 
-   [EEG/EMG](#gmg) 
    -   [`[2019-01-20]` Backyard Brains Store https://backyardbrains.com/products/](#bckyrdbrnsstrsbckyrdbrnscmprdcts) [[hobby]]
        -   [`[2019-01-25]` hmm that looks pretty promising I think](#hmmthtlksprttyprmsngthnk) 
        -   [`[2019-02-24]` huh? free delivery? https://www.onbuy.com/gb/science-and-discovery/backyard-brains-muscle-spikerbox-neuroscience-in-a-box~c2371~p6511442/](#hhfrdlvryswwwnbycmgbscncnbrnsmsclspkrbxnrscncnbxcp) 
    -   [`[2019-01-20]` Myoware EMG Sensor - Arduino Tutorial | Cost Effective EMG Sensor - RootSaid](#mywrmgsnsrrdnttrlcstffctvmgsnsrrtsd) [[emg]]
        -   [`[2019-01-25]` simple tutorial.. but fuck it's so tedious to read the signal! E.g. you need to clean the skin etc.](#smplttrlbtfcktsstdstrdthsgnlgyndtclnthskntc) 
        -   [`[2019-02-24]` https://www.youtube.com/embed/DOFtN67y1j0 hmm, that looks promising..](#swwwytbcmmbddftnyjhmmthtlksprmsng) 
    -   [`[2019-01-25]` Advancer Technologies, LLC: [DIY] Conductive Fabric Electrodes](#dvncrtchnlgsllcdycndctvfbrclctrds) [[emg]]
    -   [`[2019-02-14]` Hacking Your Brain Waves: A Guide To Wearable Meditation Headsets https://www.diygenius.com/hacking-your-brain-waves/](#hckngyrbrnwvsgdtwrblmdttnsswwwdygnscmhckngyrbrnwvs) 
    -   [`[2019-02-24]` TrueSense Exploration Kit | OP Innovations](#trsnsxplrtnktpnnvtns) [[eeg]] [[emg]]
-   [`[2019-04-11]` Anyone had experience with EEG headsets? : QuantifiedSelf https://www.reddit.com/r/QuantifiedSelf/comments/ac5x6u/anyone\_had\_experience\_with\_eeg\_headsets/](#nynhdxprncwthghdstsqntfdsmntscxnynhdxprncwthghdsts) 
-   [`[2019-05-21]` How to Hack Toy EEGs | Frontier Nerds http://www.frontiernerds.com/brain-hack](#hwthcktygsfrntrnrdswwwfrntrnrdscmbrnhck) 
-   [`[2019-05-21]` Home](#hm) [[eeg]] [[vr]]
-   [`[2019-06-22]` Contents — visbrain 0.4.4 documentation](#cntntsvsbrndcmnttn) [[emg]] [[viz]]
-   [`[2019-04-15]` Using deep learning to “read your thoughts” — with Keras and an EEG sensor](#sngdplrnngtrdyrthghtswthkrsndngsnsr) [[eeg]] [[mind]] [[openbci]]
    -   [`[2019-07-31]` very cool! lots of good techniquies with signal processing and neural networks](#vryclltsfgdtchnqswthsgnlprcssngndnrlntwrks) 
-   [`[2019-07-20]` Inria - Comparison of a consumer grade EEG amplifier with medical grade equipment in BCI applications https://hal.inria.fr/hal-01278245](#nrcmprsnfcnsmrgrdgmplfrwtdqpmntnbcpplctnsshlnrfrhl) 
-   [`[2019-07-20]` MIT researcher takes the quantified self to the extreme with an EEG helmet — Quartz https://qz.com/1348242/the-human-cyborg-collecting-his-memories-on-video/](#mtrsrchrtksthqntfdslftthxhhmncybrgcllctnghsmmrsnvd) 
-   [`[2019-02-24]` Alex Grey on Tracking Muscle Data (EMG, ECG) - Quantified Self](#lxgryntrckngmscldtmgcgqntfdslf) [[qs]] [[emg]]
-   [`[2019-02-24]` QS Resource Guide](#qsrsrcgd) [[emg]]
-   [`[2018-07-14]` ici·bici: here's a low cost, open source brain-computer interface](#cbchrslwcstpnsrcbrncmptrntrfc) [[bci]] [[eeg]]
-   [Melon band: dismissed? https://www.reddit.com/r/QuantifiedSelf/comments/6qke2e/what\_to\_do\_with\_this\_melon\_eeg\_headband\_now\_that/](#mlnbnddsmssdswwwrddtcmrqnwhttdwththsmlnghdbndnwtht) 
-   [related](#rltd) [[emg]] [[bci]] [[qs]]
-   [`[2019-09-02]` Mind controlled text writer /r/Python](#srddtcmrpythncmmntscdwmndtrmndcntrlldtxtwrtrrpythn) [[eeg]] [[openbci]]





# OpenBCI is best apparently?

At Drexel we've had a lot of success with openBCI. I can't comment on all of the other choices, but I think for the money, OpenBCI is a great choice. We've had an advanced undergraduate co-op in our lab working with it for about 2 months, and he's gotten a 16ch board put together and connected to a 3d printed headset we bought, gotten openBCI fully running, connected it to OpenVIBE and begun running their modules. Full access to the data, including in Matlab.  
<https://github.com/OpenBCI>  




## ganglion? <https://shop.openbci.com/collections/frontpage/products/pre-order-ganglion-board?variant=13461804483> can do EEG, EMG, ECG




## <https://neurobb.com/t/is-there-really-no-affordable-user-friendly-neurofeedback-hardware-software-out-there/75> 

One option would be to go with OpenBCI hardware and a (relatively) inexpensive proprietary neurofeedback software option like BioEra 290. I have not used BioEra, but it is compatible with OpenBCI and is much more geared towards neurofeedback than BrainBay or OpenViBE. A somewhat more expensive hardware option is Pocket-Neurobics 325, which works with BioEra or BioExplorer, and is apparently popular among home neurofeedback trainers. As @curiositry mentioned, William Croft 104 is a great resource on this topic.  




## <https://www.youtube.com/watch?v=QIWswAOFp8w> 

needs a special bt dongle?  
mark 4 doesnt require any paste, it's dry  




## <https://www.youtube.com/watch?v=agV1B2l-QLw> 

ok, so it looks pretty easy to filter individual frequencies too.  




## print it youself: about 500$ =/




## could try using 3d printer at work?




## <http://www.autodidacts.io/getting-started-with-openbci-a-tutorial-on-testing-troubleshooting-and-recording-ekg/> 





### + The OpenBCI arrives pre-assembled and tested, and is relatively straightforward for someone without previous bci experience to get started with — no soldering, hair-tearing, or midnight coding sessions need appl




### + Finally, the OpenBCI’s output is far closer to clinical or research grade than most consumer or amateur systems: It has an excellent sample-rate (250 Hz), works with well-established processing and display software, and can be used with any electrodes with industry-standard “touchproof” connectors, so you aren’t stuck with the type it comes with.




### ? use 32 but Which should you choose? In most cases, it probably doesn’t matter. If you’ve used Arduino before, the 8bit would be a good choice. Also, the Arduino community is quite active and helpful. The 32bit version is more powerful, which means that it can do more processing on the signal before it’s sent over bluetooth. If you plan on doing a lot of with tinkering with the code running on the OpenBCI itself, the 32bit version may be a better choice.




### ? need 10-20 paste?




### ? TODO how to secure electrodes




## - very little data on the internet and reddit.. unlikely to get any help if i buy it




## eh. quite costy. so buy it, but ONLY after you consolidate all other sleep trackers so you could compare




# Do you have fine control of your head and neck? If so then a headset with a gyro will be much better (Muse by InteraXon or Emotiv).

<https://www.reddit.com/r/eeg/comments/6bqd63/looking_for_affordable_wired_personal_eeg/>  
<https://www.reddit.com/r/eeg/comments/3vxbem/comparison_of_consumer_eeg_devices/>  
<http://www.autodidacts.io/neurotech-hardware-roundup-eeg-bci-tdcs-neurofeedback/>  




# ultracortex: 3d printed




# `[2018-07-15]` how are EMG and EEG different?      [[emg]]

ok, so surface EMG needs two electrodes since it's recording potential difference  




# EMG?  how can it be used      [[emg]]

<https://youtu.be/gHsZ0bwxMsg?t=3m21s>   
stronger exercise &#x2013; stronger signal  
<https://en.wikipedia.org/wiki/Electromyography#Normal_results>  




## ok, so on reddit everyone claims relation between EMG and muscle activation is unclear

<https://www.reddit.com/r/Fitness/comments/ime4r/inside_the_muscles_best_ab_exercises_6/>  
howerer, I could get some pretty interesting data!  




## in particular, it's hard to interpret signal correctly

<https://www.reddit.com/r/bodybuilding/comments/1vcwc0/emg_activity_results_on_backsquats_vs_front_squats/cer04il/?utm_content=permalink&utm_medium=front&utm_source=reddit&utm_name=bodybuilding>  
e.g. you should prob be looking for frequency rather than amplitude  
Being "strong" means exerting the same amount of force with a lower number of recruited motor units.  




## <https://www.reddit.com/r/bodyweightfitness/comments/7x0jqq/_/> 

smth about EMG misuse  




## devices 





### <https://www.amazon.co.uk/ADVANCER-TECHNOLOGIES-Muscle-Sensor-MyoWare/dp/B018TIWR32/ref=sr_1_3?ie=UTF8&qid=1531258073&sr=8-3&keywords=EMG+sensor> 

43 gbp  




### <https://shop.openbci.com/collections/frontpage/products/myoware-muscle-sensor?variant=29472011267> 




### <https://www.amazon.co.uk/MyoWare-Muscle-Sensor-Development-Kit/dp/B01LX6MX4P/ref=sr_1_5?ie=UTF8&qid=1531258073&sr=8-5&keywords=EMG+sensor> 

kit for 99  




### aliexpress? 




# Neurosky? 





## ? 1 channel




## + I did some fairly extensive testing of the Neurosky device while I was working on an app to analyze brainwave signals.




## - pretty expensive on amazon :( about 150 GBP?




# Neuroonopen 

<https://neuroonopen.com/>  




## + alarm LED and vibration




## ? Only four states are recognized though: awake, light sleep, REM sleep and deep sleep. [reddit]




## - I got it, doesn't do anything regarding helping you achieve polyphasic sleep which is the frigging reason of why I supported the kickstarter in the first place. [reddit]




## - the hugest minus in my opinion: you can not zoom within your sleep graph. You can see that you fell into deep sleep approximately but you will never know at which hour exactly. This is fairly annoying.




## - no news from them




# Emotiv <https://www.emotiv.com/comparison/>





## emotiv insight is 200. If not emotiv, you'd be better off making your own for that price.

<http://openeeg.sourceforge.net/doc/>  




## - I have not tried emotiv but I was put off by the $500 SDK. You are selling the device and want people to develop for your platform to extend it and you are charging them for the SDK??




## - raw data costs a lot




## - have to use their software

    The Emotiv forces the user to use their software. Raw data costs A LOT extra. Muse + OpenBCI give raw eeg data free. In fact, they give everything except the hardware for free. OpenBCI is completely open source (their name is proprietary....for prosperity). Emotiv sensors are finnicky. They work, they don't work. You can never tell when they will have a good or bad day. Look at the community around their hardware (from my comment above).
    OpenBCI gives you the freedom to select your own electrodes (wet, dry, amplified, etc.) You are free to use whichever development platform you are comfortable in (matlab, BCI2000, Python, OpenVibe, Go....)
    Muse has a good set of dry sensors. They work. I've even used them in a project at the SF Exploratorium, and at a Tech summit in Shenzhen.

<http://www.exploratorium.edu/press-office/press-releases/new-exhibition-understanding-influencing-brain-activity-opens>  
<http://www.cre8summit.io/>  
OpenBCI and Muse have thriving communities. Here's some of them: <http://neurotechx.com/>  
<https://neurobb.com/>  
<http://openbci.com/community/>  
I am a part of that open community and it really is great to participate with such friendly, open, intelligent people.  
permalinkembedsaveparent  




# Muse band      [[buy]] [[qs]] [[meditation]]

    After purchasing a Muse headset as part of a project to improve focus & reduce distractibility, I started meditating with the band to determine how it can impact my mental focus.
    The Muse headband is a brain wave tracking device that comes with a cell-phone app to measure effectiveness of any meditation session. There are 7 sensors on the headband to get an overall picture of what the brain is doing.

-   ? 4 channels
-   ? 269 GBP
-   PRO sdk is free
-   PRO guy from QS meetup (Tony) recommended it, however his app seemed to be a bit clunky..  
    `[2018-01-22]`
-   CON dont bother even with trying it [–][deleted] 39 points 1 year ago\*  
    
        dont bother even with trying it. while Ive not seen a teardown of this device nearly all of these "mind reading" devices are simply a neurosky thinkgear TGAM module in some packaging and rebranded as some new super tech. these modules are the same ones in those japanese cat ears that read your brain and move the ears, the gaming headsets you are supposed to be able to trigger, and the various "personal mental training devices" like this one.
        its a single channel EEG that basically works as an on off switch when various brainwaves hit enough activity. three problems
        one or just a few channels is not enough data for any real amount of "sensing" nor is it enough channels of data to even get a basic picture of overall brain activity.
        these devices are super slow in response time so they are nearly useless. by the time it senses and you notice its like 2 seconds or so. that makes it only useful for these "meditation" applications since no realtime work or actions can be done with them. (otherwise we would be using decades old EEG tech for lots of cool stuff)
        the actual different brainwaves are usually not individually used and instead are combined into a generic "activity level" which again is of little use.
        if you really want to mess with them buy any of these devices or any of the "mindflex toys" which contain these modules and read the values directly with a microcontroller.

<https://www.reddit.com/r/Biohackers/comments/8imlo7/muse_headband_has_anyone_here_tried_it/>  
 hmm people here generally recommend it&#x2026;  




## xxx `[2018-07-15]`

ok, so apparently objections are that often it can't distinguish between muscular activity and brain activity.  




## what's it composed of

right so it's got 7 sensors  




## <https://medium.com/pixeldreams/my-40-day-journey-into-meditation-with-muse-the-brain-sensing-headband-12e7b060c6fa> 

interesting, spikes on graphs when he had epiphanies. I guess that could be interesting data to see when I experience cool effects?  

yeah. Definitely, these types of plots could keep me motivated. do it.  

the guy is quite decent though. doing lots of self experiments, cool.  




## final decision: ok, the data is useful and I don't care that much about neurofeedback. instead, invest in proper openbci??




## good review <https://www.warrior.do/muse-headband-review/>

If you’re a beginning meditation practitioner, the Muse is great at helping flag when you’re mind is active or calm. The first year of using The Muse, the feedback was amazing to quiet my mind, as I was still learning the basics of the practice.  

But as my skills improved, the device wasn’t as useful as before. I’ve found that if you’re an intermediate or an advanced meditator (whose beta/alpha wave fluctuation are much more subtle), the device is relatively crude in picking up these signals.  

For example, if I’m now in a session and my mind ever so slightly shifts focus away from my breath, I’ll catch these thoughts but it will go undetected on the Muse. I’m in the process of transitioning to a higher-end device that is more accurate and sensitive to these subtle electrical changes in my brainwaves.  




# mindflex toys??




# <https://johnfawkes.com/becoming-superhuman-through-diy-brain-scanning/> 




# bci 

<https://www.scientificamerican.com/article/pogue-6-electronic-devices-you-can-control-with-your-thoughts/>  
<https://www.reddit.com/r/DrugNerds/comments/2pmnxc/im_using_an_eeg_neurofeedback_machine_to_measure/>  




# `[2019-02-04]` neurable: Announcing the world’s first brain-computer interface for virtual reality      [[eeg]] [[vr]]

<https://medium.com/neurable/announcing-the-worlds-first-brain-computer-interface-for-virtual-reality-a3110db62607>  




## `[2019-02-15]` dunno, almost nothing on reddit, you can't buy it now etc. try again somewhat later&#x2026;




# `[2019-01-24]` EEG-SMT - Open Source Hardware Board      [[eeg]]

<https://www.olimex.com/Products/EEG/OpenEEG/EEG-SMT/>  
ok, people on reddit generally recommend it&#x2026;  




# `[2019-01-27]` How to build a brain interface — and why we should connect our minds      [[eeg]]

<https://medium.com/@justlv/how-to-build-a-brain-interface-and-why-we-should-connect-our-minds-35003841c4b7>  
describing various potential neurointerfaces &#x2013; somewhat interesting stuff  




# `[2019-02-24]` Somaxis EMG EKG EEG sensors – muscle, heart, brain, posture, activity

<http://www.somaxis.com/>  
huh that's interesting  




# Some EEG stuff





## `[2019-01-20]` BioShare.info

<https://www.bioshare.info/en>  




## `[2019-01-20]` Physiological Monitoring | HaB Direct

<https://www.habdirect.co.uk/product-category/fitness/fitness-testing-and-sports-performance/activity-monitoring-fitness-testing-and-sports-performance/>  




## `[2019-01-20]` BioHarness 3 Compression Shirts | HaB Direct

<https://www.habdirect.co.uk/product/bioharness-3-compression-shirts/?attribute_size=Medium&gclid=CjwKCAiAsoviBRAoEiwATm8OYIZqIO56Lq78SqDfgoV5j6QuQq9eh5qlh3Y_7fMDN_2kWD66lexhlxoCGykQAvD_BwE>  




## `[2019-01-20]` SnapECG Portable EKG Monitor, Handheld ECG Heart Rate Monitor for Smart Phone, Wireless Heart Performance Tracking without ECG Electrodes Required, Home Use Ekg Monitoring Devices for iPhone & Android: Amazon.co.uk: Sports & Outdoors

<https://www.amazon.co.uk/SnapECG-Portable-Performance-Electrodes-Monitoring/dp/B07FKYPTDQ/ref=sr_1_3?ie=UTF8&qid=1547946837&sr=8-3&keywords=qardiocore>  




## `[2019-01-20]` EKG ECG Heart Rate Monitor: QardioCore Continuous Electrocardiograph ECG/EKG Mobile Machine - Wireless, Portable, Wearable Heart Monitoring Equipment - Bluetooth Mobile Digital Cardio Devices: Amazon.co.uk: Health & Personal Care

<https://www.amazon.co.uk/EKG-Heart-Rate-Monitor-Electrocardiograph/dp/B073VW2ZZV/ref=sr_1_1_a_it?ie=UTF8&qid=1547946837&sr=8-1&keywords=qardiocore>  




## `[2019-01-20]` eMotion EMG | shop.bittium.com      [[emg]] [[qs]]

<https://shop.bittium.com/product/6/emotion-emg>  
fucking hell&#x2026; 4K!  




## `[2019-01-20]` Bittium Faros - Bittium      [[hr]]

<https://www.bittium.com/products__services/medical/bittium_faros#technical_details>  
looks very cool, but also fucking expensive, 3K  




## `[2019-01-20]` My Baseline Network Physiology: 10 Days of EEG, EGG, EKG, CGM, Temperature, Activity and Food Logs - Quantified Self / Project Logs - Quantified Self Forum      [[qs]]

<https://forum.quantifiedself.com/t/my-baseline-network-physiology-10-days-of-eeg-egg-ekg-cgm-temperature-activity-and-food-logs/5671/21>  
awesome correlation experiment between hr, body temperature, food etc  




## `[2019-01-20]` DS1922L-F5# Thermochron iButton [-40 to 85°C] - 8K Memory | iButtonLink      [[qs]]

<https://www.ibuttonlink.com/products/ds1922l>  
think for body temperature tracking&#x2026; although would be very adhoc, would need a patch to hold it or something like that. expect the skin to be irritated  




## `[2019-01-20]` MySignals - eHealth and Medical IoT Development Platform      [[qs]] [[gadget]]

<http://www.my-signals.com/>  
that costs about 1K, but looks pretty cool. EKG,   EMG, respiratory sensor etc. will be inconvenient to wear though  




## `[2019-01-20]` Reliable wearable ECG - Quantified Self / Apps & Tools - Quantified Self Forum      [[hr]]

<https://forum.quantifiedself.com/t/reliable-wearable-ecg/2653>  
a lot of ecg related medical grade tools  




## `[2019-01-20]` Firstbeat Firstbeat Bodyguard 2      [[hr]]

<http://shop.firstbeat.com/us/bodyguard.html#.XEQ3KVX7TMg>  
uses electrodes..  
ok, so apparently currently there is no reliable way of tracking very accurate continuous HR without changing electrodes etc  




# `[2019-05-10]` [New neural implant in trials](https://reddit.com/r/BrainMachineInterface/comments/begb98/new_neural_implant_in_trials/) /r/BrainMachineInterface      [[bci]]





## `[2019-05-12]` huh, pretty cool, electrod mesh injected via a vein right into the brain




# EEG/EMG 





## `[2019-01-20]` Backyard Brains Store <https://backyardbrains.com/products/>      [[hobby]]





### `[2019-01-25]` hmm that looks pretty promising I think




### `[2019-02-24]` huh? free delivery? <https://www.onbuy.com/gb/science-and-discovery/backyard-brains-muscle-spikerbox-neuroscience-in-a-box~c2371~p6511442/>




## `[2019-01-20]` Myoware EMG Sensor - Arduino Tutorial | Cost Effective EMG Sensor - RootSaid      [[emg]]

<https://rootsaid.com/myoware-emg-sensor-arduino/>  




### `[2019-01-25]` simple tutorial.. but fuck it's so tedious to read the signal! E.g. you need to clean the skin etc.




### `[2019-02-24]` <https://www.youtube.com/embed/DOFtN67y1j0> hmm, that looks promising..




## `[2019-01-25]` Advancer Technologies, LLC: [DIY] Conductive Fabric Electrodes      [[emg]]

<http://www.advancertechnologies.com/2013/03/diy-conductive-fabric-electrodes.html>  
hmm, that's pretty cool, could get reusable electrodes that way  




## `[2019-02-14]` Hacking Your Brain Waves: A Guide To Wearable Meditation Headsets <https://www.diygenius.com/hacking-your-brain-waves/>




## `[2019-02-24]` TrueSense Exploration Kit | OP Innovations      [[eeg]] [[emg]]

<https://www.op-innovations.com/en/node/96>  




# `[2019-04-11]` Anyone had experience with EEG headsets? : QuantifiedSelf <https://www.reddit.com/r/QuantifiedSelf/comments/ac5x6u/anyone_had_experience_with_eeg_headsets/>

    I wrote an app for the NeuroSky, but eventually gave up on it because getting a good signal was so tedious.




# `[2019-05-21]` How to Hack Toy EEGs | Frontier Nerds <http://www.frontiernerds.com/brain-hack>




# `[2019-05-21]` Home      [[eeg]] [[vr]]

<https://myndplay.com/>  




# `[2019-06-22]` Contents — visbrain 0.4.4 documentation      [[emg]] [[viz]]

<http://visbrain.org/index.html>  

    Visbrain documentation _static/ico/visbrain.png
    A multi-purpose GPU-accelerated open-source suite for brain data visualization.




# `[2019-04-15]` Using deep learning to “read your thoughts” — with Keras and an EEG sensor      [[eeg]] [[mind]] [[openbci]]

<https://medium.com/@justlv/using-ai-to-read-your-thoughts-with-keras-and-an-eeg-sensor-167ace32e84a>  




## `[2019-07-31]` very cool! lots of good techniquies with signal processing and neural networks




# `[2019-07-20]` Inria - Comparison of a consumer grade EEG amplifier with medical grade equipment in BCI applications <https://hal.inria.fr/hal-01278245>

    Abstract : This paper presents a comparison between a consumer grade EEG (electroencephalography) amplifier and a medical grade equipment. Using the same set of EEG electrodes, signals recorded from the OpenBCI board are compared side-by-side with those recorded from the g.tec g.USBamp device. Two BCI (brain-computer interface) applications are studied: a P300 speller and a workload estimator. In both applications EEG features are highly correlated. Moreover, the classification performances obtained with the OpenBCI board come close to the accuracy achieved with the g.tec g.USBamp. Overall, these preliminary results suggest that the OpenBCI board -- or a similar solution based on the Texas Instrument ADS1299 chip -- may be an alternative to traditional EEG amplifiers, widening the realm of applications and increasing the number of potential users.




# `[2019-07-20]` MIT researcher takes the quantified self to the extreme with an EEG helmet — Quartz <https://qz.com/1348242/the-human-cyborg-collecting-his-memories-on-video/>




# `[2019-02-24]` Alex Grey on Tracking Muscle Data (EMG, ECG) - Quantified Self      [[qs]] [[emg]]

<http://quantifiedself.com/2012/03/alex-grey-on-tracking-muscle-data-emg-ecg/>  




# `[2019-02-24]` QS Resource Guide      [[emg]]

<http://experimentable.com/qs-guide/>  




# `[2018-07-14]` ici·bici: here's a low cost, open source brain-computer interface      [[bci]] [[eeg]]

<https://icibici.github.io/site/>  
<https://www.reddit.com/r/NeuroHacking/comments/89qasr/does_anybody_knows_how_to_buy_this_bci_20_kit/> mm unclear how to buy it&#x2026;  




# Melon band: dismissed? <https://www.reddit.com/r/QuantifiedSelf/comments/6qke2e/what_to_do_with_this_melon_eeg_headband_now_that/>




# related       [[emg]] [[bci]] [[qs]]




# `[2019-09-02]` [Mind controlled text writer](https://reddit.com/r/Python/comments/cdwea0/mind_controlled_text_writer/) /r/Python      [[eeg]] [[openbci]]

<https://www.youtube.com/watch?v=1GdjMx5t4ls>  

    **Idea of P300 speller:**
    Highlight rows and cols and record EEG reaction to these events. If row/col with target character is highlighted \~after 300ms peak on EEG diagram will occur and it's possible to train classifier to  detect it. To remove noise from EEG data repeat it multiple times and use bandpass filter
    
    **Hardware:** [OpenBCI Cyton](https://brainflow.readthedocs.io/en/latest/SupportedBoards.html#openbci-cyton)
    **Software:**
    * [BrainFlow library](https://github.com/Andrey1994/brainflow) to read and preprocess data from OpenBCI board
    * [P300 implementation](https://github.com/Andrey1994/brainapps/tree/master/p300-speller)

