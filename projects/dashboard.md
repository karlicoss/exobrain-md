
# Table of Contents

-   [related](#rltd) 
    -   [used to visualize #qs data](#sdtvslzqsdt) [[qs]]
    -   [very similar to #timeline and #memex](#vrysmlrttmlnndmmx) [[timeline]] [[memex]]
    -   [#hpi provides data for my dashboard](#hpprvdsdtfrmydshbrd) [[hpi]]
-   [\* motivation](#mtvtn) 
    -   [why not use something existing?](#whyntssmthngxstng) 
    -   [figuring out core patterns for manipulating and representing this data](#fgrngtcrpttrnsfrmnpltngndrprsntngthsdt) 
    -   [automatically detecting interesting correlations between data](#tmtcllydtctngntrstngcrrltnsbtwndt) 
        -   [`[2019-08-15]` wonder if massive dataframe with literally everything could help](#wndrfmssvdtfrmwthltrllyvrythngcldhlp) 
        -   [maybe just go over all series? and then generate all pairwise correlations and sort by correlation coefficient + R<sup>2</sup>? some sort of pareto surface?](#mybjstgvrllsrsndthngnrtllrrltncffcntrsmsrtfprtsrfc) 
    -   [what I want to figure out:](#whtwnttfgrt) 
        -   [very similar to https://github.com/KrauseFx/FxLifeSheet#questions-to-answer](#vrysmlrtsgthbcmkrsfxfxlfshtqstnstnswr) 
        -   [are 'sleep phases' a thing (or at least the way they are measured in conventional tackers)? how do they impact my waking up, alertness etc?](#rslpphssthngrtlstthwythyrhwdthympctmywkngplrtnsstc) [[sleep]]
        -   [`[2020-10-27]` calculating custom exercise stats](#clcltngcstmxrcsstts) 
    -   [custom/personalized data processing](#cstmprsnlzddtprcssng) 
        -   [splitting exercise into cardio and non-cardio](#splttngxrcsntcrdndnncrd) 
    -   [demo of errors: typical mistake is confuising wlog and weight tags (weight gets unrecognized as exercise)](#dmfrrrstypclmstkscnfsngwlghttgswghtgtsnrcgnzdsxrcs) [[dashboard]]
-   [\* inspiration](#nsprtn) 
    -   [`[2018-06-06]` andreilyskov: qs dashboard example](#sqslfdshbrdhrkppcmndrlyskvqsdshbrdxmpl) [[qs]]
        -   [`[2019-04-06]` interesting dashboards: spotify, writing and reading. otherwise not that much stuff](#ntrstngdshbrdssptfywrtngndrdngthrwsntthtmchstff) 
        -   [`[2020-08-22]` ok seems that they use similar architecture to mine https://forum.quantifiedself.com/t/personal-dashboards-for-self-tracking-data/8202/4](#ksmsthtthyssmlrrchtctrtmnprsnldshbrdsfrslftrckngdt) 
    -   [`[2020-08-22]` Flow Dashboard](#sflwdshcppbtflwdshbrd) 
        -   [`[2021-02-06]` ok, rest api thing is cool, should try connecting it to #hpi](#krstpthngsclshldtrycnnctngtthp) [[hpi]]
    -   [`[2019-11-24]` heedy/heedy: An Open-Source Platform for Quantified Self & IoT](#sgthbcmhdyhdyhdyhdynpnsrcpltfrmfrqntfdslft) 
    -   [`[2019-05-21]` quelf/report.Rmd at master · JakobGM/quelf](#sgthbcmjkbgmqlfblbmstrnlymdqlfrprtrmdtmstrjkbgmqlf) 
    -   [`[2019-09-22]` markwk/qs<sub>ledger</sub>: Quantified Self Personal Data Aggregator and Data Analysis](#sgthbcmmrkwkqsldgrmrkwkqsslfprsnldtggrgtrnddtnlyss) [[qs]] [[dataliberation]]
        -   [`[2019-09-28]` I guess once I export everything could send a link to that guy?](#gssncxprtvrythngcldsndlnktthtgy) 
    -   [`[2020-09-03]` https://github.com/KrauseFx/FxLifeSheet](#sgthbcmkrsfxfxlfsht) 
    -   [`[2020-08-22]` some good dashboards   https://forum.quantifiedself.com/t/personal-dashboards-for-self-tracking-data/8202/15](#smgddshbrdssfrmqntfdslfcmprsnldshbrdsfrslftrckngdt) 
    -   [Juno's Personal Data Exploratory  https://exploratory.openhumans.org/notebooks](#jnsprsnldtxplrtrysxplrtrypnhmnsrgntbks) [[pkm]] [[qs]]
    -   [`[2020-07-02]` jeffshek/betterself: Your body's dashboard.](#sgthbcmjffshkbttrslfjffshkbttrslfyrbdysdshbrd) 
        -   [`[2020-08-24]` demo https://app.betterself.io](#dmsppbttrslf) 
    -   [`[2019-01-13]` Sacha Chua: quantified awesome](#qntfdwsmcmschchqntfdwsm) [[qs]]
        -   [`[2019-04-06]` ok, looks pretty clean, but might require some tinkering](#klksprttyclnbtmghtrqrsmtnkrng) 
        -   [`[2021-02-06]` also pretty much only time tracking?](#lsprttymchnlytmtrckng) 
    -   [`[2020-09-10]` quantifiedbob/bob-body-composition-viz: Jupyter Notebook vizualizing 10+ years of my body composition data](#sgthbcmqntfdbbbbbdycmpstnbkvzlzngyrsfmybdycmpstndt) 
    -   [`[2020-04-04]` ammanvedi/quantified-self-server: Aggregate data about myself (workouts, blog posts, music listening history) into a graphql API](#sgthbcmmmnvdqntfdslfsrvrmtsmsclstnnghstryntgrphqlp) 
    -   [`[2019-04-19]` markwk: How to Create a Time Tracking Dashboard using RescueTime, IFTTT and Google Sheets](#wwwmrkwkcmdtprcssngtmtrckhbrdsngrsctmftttndgglshts) [[qs]]
    -   [`[2019-01-08]` Personal Dashboard /r/QuantifiedSelf](#srddtcmrqntfdslfcmmntscxyshbrdprsnldshbrdrqntfdslf) 
        -   [`[2019-04-11]` it is not very elaborate though&#x2026;](#tsntvrylbrtthgh) 
    -   [minor ideas](#mnrds) 
        -   [keeping query in the address string is pretty clever&#x2026; can bookmark and easily restart it!](#kpngqrynthddrssstrngsprttyclvrcnbkmrkndslyrstrtt) [[datasette]]
        -   [`[2020-08-22]` event chart https://forum.quantifiedself.com/t/best-examples-of-quanitified-self-dashboards/4590/9](#vntchrtsfrmqntfdslfcmtbstxmplsfqntfdslfdshbrds) 
        -   [use tabs within tabs? kinda like in garmin https://connect.garmin.com/modern/activities](#stbswthntbskndlkngrmnscnnctgrmncmmdrnctvts) 
        -   [`[2020-10-27]` Garmin Connect](#scnnctgrmncmmdrnctvtygrmncnnct) 
    -   [`[2021-01-11]` yihong0618/running<sub>page</sub>: Make your own running home page](#sgthbcmyhngrnnngpgyhngrnnngpgmkyrwnrnnnghmpg) 
-   [\* implementation](#mplmnttn) 
    -   [(meta?)goals](#mtgls) 
        -   [keep it modular, I guess](#kptmdlrgss) 
        -   [`[2020-09-01]` similarly to HPI, it's more of a demonstration how it can be done. Ideally people would be able to reuse core and build their own dashboards](#smlrlythptsmrfdmnstrtnhwtbbltrscrndbldthrwndshbrds) 
    -   [it's very important to benefit from the existing data science infrastructure as much as possible. jupyter, pandas, etc.](#tsvrymprtnttbnftfrmthxstnrctrsmchspssbljpytrpndstc) 
    -   [`[2020-12-10]` panel · PyPI](#spyprgprjctpnlpnlpyp) 
    -   [`[2020-12-07]` oschuett/appmode: A Jupyter extensions that turns notebooks into web applications.](#sgthbcmschttppmdschttppmdnsthttrnsntbksntwbpplctns) 
        -   [`[2021-02-06]` ok, nice, has 'edit app' button which opens jupyter to edit??](#knchsdtppbttnwhchpnsjpytrtdt) 
    -   [`[2020-08-23]` ok, #jupyter is the ultimate ad-hoc solution. it preserves state, can be exposed as a frontend and allows for python code](#kjpytrsthltmtdhcsltntprsrpsdsfrntndndllwsfrpythncd) 
    -   [bokeh vs plotly dash](#bkhvspltlydsh) 
        -   [`[2020-09-03]` compromise: keep it as framework independent and decoupled as possible. Support both frameworks!](#cmprmskptsfrmwrkndpndntndcpldspssblspprtbthfrmwrks) 
    -   [basically have a core library that's imported in all notebooks. move stuff to core as long as possible, but allow quick button to mess with the data in notebook](#bscllyhvcrlbrrythtsmprtdnlwqckbttntmsswththdtnntbk) [[toblog]]
    -   [try jupyterlab](#tryjpytrlb) 
    -   [I think dashboard needs to preserve state somehow, it's annoying to edit code every time.. wonder if dash supports it?](#thnkdshbrdndstprsrvsttsmhtdtcdvrytmwndrfdshspprtst) 
    -   [use multiprocessing&#x2026;](#smltprcssng) 
    -   [`[2020-09-10]` Top 50 matplotlib Visualizations - The Master Plots (w/ Full Python Code) | ML+](#swwwmchnlrnngplscmpltstpmnsthmstrpltswfllpythncdml) 
    -   [grafana could simply be one of the interfaces](#grfncldsmplybnfthntrfcs) 
    -   [`[2021-02-17]` apache/superset: Apache Superset is a Data Visualization and Data Exploration Platform](#sgthbcmpchsprstsprstpchspsdtvslztnnddtxplrtnpltfrm) [[dashboard]] [[hpi]]
-   [\* sleep dashboard/experiments](#slpdshbrdxprmnts) [[sleep]]
    -   [Maybe run pca for my sleep data?](#mybrnpcfrmyslpdt) [[sleep]] [[qs]] [[ml]]
    -   [figure out main questions I wanna figure out](#fgrtmnqstnswnnfgrt) [[qs]] [[sleep]]
        -   [e.g. 'what is the best time for me to go asleep'?](#gwhtsthbsttmfrmtgslp) 
        -   ['what is the best sleep duration?'](#whtsthbstslpdrtn) 
    -   [`[2019-08-21]` Respiratory rate - Wikipedia](#rsprtryrtwkpd) [[sleep]]
        -   [`[2020-08-24]` add to dataframe](#ddtdtfrm) 
    -   [correlate with sliding exponential mean instead?](#crrltwthsldngxpnntlmnnstd) [[sleep]]
    -   [add date to tooltip](#dddtttltp) [[sleep]]
    -   [def need to highlight holidays on the background (also annotate if it was indeed a day off), e.g. where have I gone](#dfndthghlghthldysnthbckgrlsnnttftwsndddyffgwhrhvgn) [[sleep]]
    -   [wonder if coverage is correlated with sleep movement&#x2026;](#wndrfcvrgscrrltdwthslpmvmnt) [[sleep]]
    -   [find correlation between bedtime and length of sleep?](#fndcrrltnbtwnbdtmndlngthfslp) [[sleep]]
    -   [Sleep/exercise correlation: could try different deltas/correlation coeff plot](#slpxrcscrrltncldtrydffrntdltscrrltncffplt) 
    -   [old sleep logs from taplog?](#ldslplgsfrmtplg) [[sleep]]
    -   [check waking up in REM?](#chckwkngpnrm) [[sleep]]
    -   [interesting correlation: sleep vs bed time. wonder if that means REM or something?](#ntrstngcrrltnslpvsbdtmwndrfthtmnsrmrsmthng) 
    -   [hmm, sleepy correlates negatively with ex. volume?](#hmmslpycrrltsngtvlywthxvlm) 
    -   [hmm. temperature is interesting &#x2013; looks like it's negatively correlating with HR??](#hmmtmprtrsntrstnglkslktsngtvlycrrltngwthhr) [[qs]]
    -   [sleep plot: highlight holidays/weekends as background color?](#slpplthghlghthldyswkndssbckgrndclr) 
    -   [movements/bed exit in emfit?](#mvmntsbdxtnmft) 
        -   [`[2020-08-25]` could plot on the sleep bars plot?](#cldpltnthslpbrsplt) 
    -   [integrate old melatonin experiment, maybe post about it](#ntgrtldmltnnxprmntmybpstbtt) 
    -   [use ANS balance from emfit?](#snsblncfrmmft) 
    -   [`[2018-06-20]` Emfit qs estimated my sleep high, even though i felt a bit like shit. I wonder if it just correlates with sleep length..](#mftqsstmtdmyslphghvnthghfndrftjstcrrltswthslplngth) 
    -   [temperature during sleep](#tmprtrdrngslp) [[qs]] [[sleep]]
    -   [different style for sleep length bars? currently red and blue are sort of annoyingly make it hard to spot the pattern?](#dffrntstylfrslplngthbrscrfnnynglymkthrdtsptthpttrn) [[emfit]]
    -   [Average temperature](#vrgtmprtr) [[sleep]]
    -   [cross correlate with rescuetime activity](#crsscrrltwthrsctmctvty) [[sleep]]
        -   [`[2020-08-25]` could even plot activity bars](#cldvnpltctvtybrs) 
    -   [figure out alarm wakeup vs 'natural' wakeup, could tell me something about sleep intervals](#fgrtlrmwkpvsntrlwkpcldtllmsmthngbtslpntrvls) [[qs]]
    -   [Emfit recovery &#x2013; wonder if it correlated with exercise days](#mftrcvrywndrftcrrltdwthxrcsdys) [[sleep]] [[emfit]]
    -   [My daughters sleeping patterns for the first 4 months of her life. One continuous spiral starting on the inside when she was born, each revolution representing a single day. Midnight at the top (24 hour clock). [OC]](#mydghtrsslpngpttrnsfrthfrgsngldymdnghttthtphrclckc) [[sleep]] [[inspiration]] [[viz]]
    -   [Melatonin analysis](#mltnnnlyss) 
    -   [wonder what does it mean when morning hrv is higher than evening??](#wndrwhtdstmnwhnmrnnghrvshghrthnvnng) [[qs]] [[hrv]]
    -   [I wonder what happened&#x2026; at some point (around august 2019), coverage  has consistently gone up to 100](#wndrwhthppndtsmpntrndgstcvrghscnsstntlygnpt) [[qs]] [[emfit]]
    -   [Track pizza dependency?](#trckpzzdpndncy) [[qs]] [[sleep]]
    -   [Shit wonder if I'm oversleeping because it's too cold?](#shtwndrfmvrslpngbcststcld) [[qs]] [[sleep]]
    -   [pretty strong negative correlation of temp vs avg hr. wonder if that's searsonal or not? post about it soon?](#prttystrngngtvcrrltnftmpvwndrfthtssrsnlrntpstbttsn) [[qs]]
    -   [look at HRV peaks and try to see what's happening?](#lkthrvpksndtrytswhtshppnng) [[qs]] [[timeline]]
    -   [`[2019-11-14]` Опыт обращения к сомнологу](#опытобращенияксомнологу) [[qs]] [[sleep]]
    -   [Compare hr/hrv before and after holidays](#cmprhrhrvbfrndftrhldys) [[qs]] [[sleep]] [[hpi]]
    -   [Compute differences between rem cycles and plot on histogram?](#cmptdffrncsbtwnrmcyclsndpltnhstgrm) [[qs]] [[sleep]]
    -   [wow, emfit recovery was really shit last night. why???&#x2026; seriosly no reason for it](#wwmftrcvrywsrllyshtlstnghtwhysrslynrsnfrt) [[qs]] [[sleep]]
    -   [wip on figuring out if weekdays impact sleep](#wpnfgrngtfwkdysmpctslp) [[qs]]
    -   [plot my emfit sleep, to be fair even two years of plots is quite cool](#pltmymftslptbfrvntwyrsfpltssqtcl) [[publish]] [[qs]]
    -   [hmm, my hrv really has fallen down? also sleep hr gone up](#hmmmyhrvrllyhsfllndwnlsslphrgnp) [[qs]] [[health]]
    -   [track dependency on meditaion?](#trckdpndncynmdtn) [[sleep]]
    -   [display times in bed definitely&#x2026;](#dsplytmsnbddfntly) [[sleep]]
    -   [would be nice to plot against sunrise/sunset?](#wldbnctpltgnstsnrssnst) [[sleep]]
    -   [`[2020-09-30]` Relationships between HRV, sleep and physical activity in personal Oura ring data - Quantified Self / General Health - Quantified Self Forum](#sfrmqntfdslfcmtrltnshpsbttfdslfgnrlhlthqntfdslffrm) [[hrv]] [[hr]] [[sleep]] [[exercise]]
    -   [`[2020-09-30]` fucking hell! after naples HRV jumped and HR dropped very significantly](#fcknghllftrnplshrvjmpdndhrdrppdvrysgnfcntly) [[self]] [[sleep]]
    -   [correlate dreams with rem/deep etc?](#crrltdrmswthrmdptc) [[sleep]]
    -   [wtf&#x2026; without seasons it seems to correlate less??](#wtfwthtssnstsmstcrrltlss) [[sleep]]
    -   [negative correlation of coverage with temperature is pretty weird](#ngtvcrrltnfcvrgwthtmprtrsprttywrd) [[emfit]]
    -   [Compare fitbit](#cmprftbt) [[hr]] [[qs]]
    -   [For sleep, probably a good idea to log room temperature](#frslpprbblygddtlgrmtmprtr) [[sleep]] [[qs]]
    -   [hmm, maybe I need to remove seasonality from the sleep first and then search other correlations?? not sure..](#hmmmybndtrmvssnltyfrmthslstndthnsrchthrcrrltnsntsr) 
    -   [ugh. today is gonna be confusing](#ghtdysgnnbcnfsng) [[qs]] [[sleep]]
        -   [`[2020-10-18]` maybe really need to try two-parameter regression?](#mybrllyndttrytwprmtrrgrssn) 
        -   [`[2020-10-18]` take into the account past pizza orders? this is gonna have systematic impact on my sundays?](#tkntthccntpstpzzrdrsthssgnnhvsystmtcmpctnmysndys) 
-   [\* exercise dashboard/experiments](#xrcsdshbrdxprmnts) 
    -   [running dashboard &#x2013; custom dataframe + add distance + merge with manual notes in a similar way](#rnnngdshbrdcstmdtfrmdddstncmrgwthmnlntsnsmlrwy) 
    -   [thinking how to contribute data for the energy plot](#thnknghwtcntrbtdtfrthnrgyplt) [[exercise]] [[qs]]
    -   [have some stuff in endomondo comments&#x2026; need to extract it and use. maybe actually just reuse endoexport, and put in a df](#hvsmstffnndmndcmmntsndtxtybctllyjstrsndxprtndptndf) [[qs]]
    -   [Show distance on speed/hr plot](#shwdstncnspdhrplt) [[qs]]
    -   [def need to measure decay to 60 to get more data&#x2026;](#dfndtmsrdcyttgtmrdt) [[qs]] [[hr]] [[toblog]]
    -   [process google location and guess walks from it](#prcssggllctnndgsswlksfrmt) [[exercise]] [[qs]]
    -   [Detect walks and runs from google data and plot them. Mark velocity with colours. Could also do 'walking intervals' (e.g. if was in a shop inbetween)](#dtctwlksndrnsfrmggldtndpldwlkngntrvlsgfwsnshpnbtwn) [[exercise]]
    -   [calculate some sort of 'integral' heart rate and also score for interval trainings?](#clcltsmsrtfntgrlhrtrtndlsscrfrntrvltrnngs) [[exercise]]
        -   [`[2020-09-06]` eh? maybe I wanted to break down my interval trainings per activity bursts?](#hmybwntdtbrkdwnmyntrvltrnngsprctvtybrsts) 
    -   [integrate elliptical workouts? Could plot workout specific things and make them easy to compare](#ntgrtllptclwrktscldpltwrktspcfcthngsndmkthmsytcmpr) 
    -   [filter out specific exercises and plot separately to see the progress](#fltrtspcfcxrcssndpltsprtlytsthprgrss) [[exercise]]
    -   [go through the most common exercise (past) sessions and check them](#gthrghthmstcmmnxrcspstsssnsndchckthm) [[exercise]]
        -   [`[2021-02-06]` I guess it's a more general pattern for reviewing data too](#gsstsmrgnrlpttrnfrrvwngdtt) 
    -   [exercise provider: trust more notes which got HR data](#xrcsprvdrtrstmrntswhchgthrdt) [[qs]]
    -   [Look at hr data, its almost 180 all the time. Is it because i was doing cardio less?](#lkthrdttslmstllthtmstbcswsdngcrdlss) [[qs]] [[health]] [[exercise]]
-   [\* patterns](#pttrns) 
    -   [use dynamic sliders for different regression windows](#sdynmcsldrsfrdffrntrgrssnwndws) 
    -   [Always plot isolated metrics (temp, hr, etc) &#x2013; good for debugging](#lwyspltsltdmtrcstmphrtcgdfrdbggng) [[qs]]
        -   [`[2020-09-03]` also make sure it's easy to do](#lsmksrtssytd) 
    -   [restrict datapoints 'by experiment'? same way it's done with date sliders?](#rstrctdtpntsbyxprmntsmwytsdnwthdtsldrs) 
    -   [need to try different date shifts to see it's not correlated](#ndttrydffrntdtshftststsntcrrltd) 
    -   [labels: need to display weekday (also on HR nodes?)](#lblsndtdsplywkdylsnhrnds) 
    -   [would be nice to zoom individual plots..](#wldbnctzmndvdlplts) 
    -   [\* error hanling](#rrrhnlng) [[errors]]
        -   [about importance of error handling when working with personal data](#btmprtncfrrrhndlngwhnwrkngwthprsnldt) [[toblog]]
        -   [error handling &#x2013; demonstrate on 'multiple sleeps'](#rrrhndlngdmnstrtnmltplslps) 
        -   [demo: running speed/hr plot is a good candidate](#dmrnnngspdhrpltsgdcnddt) 
        -   [demo: unmark one of cardio/non-cardio and demonstrate warnings](#dmnmrknfcrdnncrdnddmnstrtwrnngs) 
        -   [document error handling pattern with 'error'](#dcmntrrrhndlngpttrnwthrrr) [[errors]] [[toblog]]
    -   [for correlations, there is overview + zoomed in individual plots showing all the errors, outliers, etc](#frcrrltnsthrsvrvwzmdnndvdlpltsshwngllthrrrstlrstc) 
    -   [Each rolling plot can also handle seasonality, residuals etc?](#chrllngpltcnlshndlssnltyrsdlstc) 
    -   [would be cool to scale arbitrarily vertically and horizontally, the whole plot](#wldbcltsclrbtrrlyvrtcllyndhrzntllythwhlplt) 
    -   [indicate how recent datapoints are by color? (in the correlations)](#ndcthwrcntdtpntsrbyclrnthcrrltns) 
    -   [corr plot: include influence/leverage etc](#crrpltncldnflnclvrgtc) 
    -   [would be nice to display data source?](#wldbnctdsplydtsrc) 
        -   [`[2019-07-20]` links to event sources (e.g. emfit etc)](#lnkstvntsrcsgmfttc) 
        -   [`[2019-04-12]` src in exercise volume](#srcnxrcsvlm) 
        -   [add src for jawbone/emfit sleep](#ddsrcfrjwbnmftslp) 
    -   [link to original event from point? or just 'context'](#lnktrgnlvntfrmpntrjstcntxt) 
    -   [vertical line tooltip sucks&#x2026; probably need a single point instead](#vrtcllntltpscksprbblyndsnglpntnstd) 
    -   [definitely need to take seasonality (e.g. weekly) into the account, e.g. for multi regression](#dfntlyndttkssnltygwklyntthccntgfrmltrgrssn) 
    -   [I guess need seasonality analisys for each metric? maybe have it on a separate pane, e.g. 'debug/insights'? would be nice to do it for all dataframes?](#gssndssnltynlsysfrchmtrcmnsghtswldbnctdtfrlldtfrms) 
    -   [would be nice to include the org file link to the context&#x2026; then could use mimemacs for it](#wldbnctncldthrgfllnktthcntxtthncldsmmmcsfrt) [[promnesia]]
-   [\* ideas for more dashboards](#dsfrmrdshbrds) 
    -   [rescuetime summarizes my sleep intervals pretty well? could at least have upper bound on sleep during holidays/when not using emfit?](#rsctmsmmrzsmyslpntrvlsprtdnslpdrnghldyswhnntsngmft) [[rescuetime]] [[hpi]]
    -   [temperature &#x2013; probably, seasonality?](#tmprtrprbblyssnlty) [[qs]]
    -   [display photos as an optional layer along with the map?](#dsplyphtssnptnllyrlngwththmp) 
        -   [`[2020-09-06]` just need to integrate dashboard with photomap](#jstndtntgrtdshbrdwthphtmp) 
    -   [links into food dashboards.. I guess I need anchors.](#lnksntfddshbrdsgssndnchrs) [[nutrino]]
    -   [favsmap should be part of dashboard&#x2026; also could be the first bit in my public dashboard?](#fvsmpshldbprtfdshbrdlscldbthfrstbtnmypblcdshbrd) 
    -   [shit. if I had food stats that would be just amazing](#shtfhdfdsttsthtwldbjstmzng) 
    -   [takeout &#x2013; contains list of places](#tktcntnslstfplcs) [[takeout]] [[hpi]]
    -   [money? not sure](#mnyntsr) 
    -   [quantified mind? already have plots](#qntfdmndlrdyhvplts) 
    -   [Add check-ins to favsmap](#ddchcknstfvsmp) 
-   [\* ideas for experiments](#dsfrxprmnts) 
    -   [correlate number of commits/lines vs sleep?](#crrltnmbrfcmmtslnsvsslp) 
    -   [glucose and ketone measurements vs food?](#glcsndktnmsrmntsvsfd) 
        -   [`[2020-09-06]` probably not enough data&#x2026;](#prbblyntnghdt) 
    -   [correlate temp sensor with hiking?](#crrlttmpsnsrwthhkng) [[toblog]] [[qs]] [[lifelogging]]
    -   [hmm, maybe need to try running/eating pizza on a different day? to make sure the seasonality is not due to running?](#hmmmybndttryrnnngtngpzznddytmksrthssnltysntdtrnnng) [[exercise]] [[qs]] [[sleep]]
        -   [`[2020-10-24]` or could check seasonality for months that didn't involve running?](#rcldchckssnltyfrmnthsthtddntnvlvrnnng) 
    -   [volume vs avg temp is an interesting one to demonstrate the correlation that shouldn't exist](#vlmvsvgtmpsnntrstngntdmnstrtthcrrltnthtshldntxst) 
    -   [try to find correlation between sleep and exercise?](#trytfndcrrltnbtwnslpndxrcs) [[qs]]
    -   [temperature plots: would be interesting to have avg plot for 'indoors' and 'outdoors' periods?](#tmprtrpltswldbntrstngthvvgpltfrndrsndtdrsprds) 
    -   [plot spinning power vs heartbeats?](#pltspnnngpwrvshrtbts) [[qs]]
-   [\* plotly dash](#pltlydsh) [[plotly]]
    -   [`[2019-10-27]` plotly/dash@1.4.0](#pltlydsh) 
    -   [`[2020-04-10]` Re: [plotly/plotly.py] Importing plotly takes a lot of time (740)](#rpltlypltlypymprtngpltlytksltftm) 
    -   [`[2019-04-10]` Dash offline is enabled?  plotly/dash](#dshfflnsnbldpltlydsh) 
    -   [wow. showing points on other plots while rectangle selection is really awesome](#wwshwngpntsnthrpltswhlrctnglslctnsrllywsm) [[plotly]]
    -   [would be really nice to properly render pairplots in plotly](#wldbrllynctprprlyrndrprpltsnpltly) 
    -   [err. seems to always consume cpu in background](#rrsmstlwyscnsmcpnbckgrnd) 
    -   [`[2020-08-26]` Re: plotly/plotly.py Importing plotly takes a lot of time (740)](#rpltlypltlypymprtngpltlytksltftm) 
    -   [`[2019-04-07]` Dash User Guide and Documentation - Dash by Plotly](#dshsrgdnddcmnttndshbypltly) 
    -   [`[2019-05-30]` ucg8j/awesome-dash: A curated list of awesome Dash (plotly) resources](#cgjwsmdshcrtdlstfwsmdshpltlyrsrcs) [[viz]]
        -   [`[2019-07-24]` https://dash-gallery.plotly.host/Portal/](#sdshgllrypltlyhstprtl) 
        -   [`[2019-07-24]` eh, dunno otherwise not so interesting? maybe I'm not really lacking anything, I can think of many things I can add that still need to be implemented..](#hdnnthrwsntsntrstngmybmntngscnddthtstllndtbmplmntd) 
-   [-----------------------------------------](#45779_45866) 
-   [come up with a better name? just in case of pypi release&#x2026;](#cmpwthbttrnmjstncsfpyprls) 
-   [how to detect temporal correlation?](#hwtdtcttmprlcrrltn) [[study]] [[qs]]
    -   [`[2020-09-01]` ok, this lag thing in bokeh could work](#kthslgthngnbkhcldwrk) 
-   [`[2019-04-19]` qs<sub>ledger</sub>/example<sub>correlation</sub><sub>explorer</sub><sub>with</sub><sub>plotly.py</sub> at master · markwk/qs<sub>ledger</sub>](#qsldgrxmplcrrltnxplrrwthpltlypytmstrmrkwkqsldgr) 
-   [`[2019-10-15]` Why you should continuously track your energy level and what I've learned from it. /r/Biohackers](#srddtcmrbhckrscmmntsdbwhyylvlndwhtvlrndfrmtrbhckrs) [[qs]]
    -   [`[2019-10-18]` about tracker matching subjective score](#bttrckrmtchngsbjctvscr) 
-   [not sure what mavg is doing. e.g. HR plots of specific exercise &#x2013; if I didn't exercise during the past month mavg for 14 days should just take value of my last exercise. right??](#ntsrwhtmvgsdngghrpltsfspcshldjsttkvlfmylstxrcsrght) 
    -   [`[2020-09-03]` need to test it, just to double check](#ndttsttjsttdblchck) 
-   [`[2019-04-11]` Visualization — pandas 0.24.2 documentation](#vslztnpndsdcmnttn) [[viz]]
-   [`[2020-09-16]` Building a Data Dashboard - Quantified Self / Apps & Tools - Quantified Self Forum](#sfrmqntfdslfcmtbldngdtdshqntfdslfppstlsqntfdslffrm) 
-   [`[2020-08-23]` All | Search powered by Algolia](#shnlglcmdtrngllpgprfxtrqrplrtytypllllsrchpwrdbylgl) 
-   [`[2020-10-11]` Accelerating with WebGL — Bokeh 2.2.1 Documentation](#sdcsbkhrgnltstdcssrgdwbgllcclrtngwthwbglbkhdcmnttn) 
    -   [`[2020-10-11]` Accelerating with WebGL — Bokeh 2.2.1 Documentation](#sdcsbkhrgnltstdcssrgdwbgllcclrtngwthwbglbkhdcmnttn) 
    -   [`[2020-10-11]` hmm, didn't seem to have any effect??](#hmmddntsmthvnyffct) 
-   [`[2020-10-11]` FifthHour/correlator: Timeseries correlation in Python, Bokeh Server and on Heroku](#sgthbcmffthhrcrrltrffthhrcrrltnnpythnbkhsrvrndnhrk) [[bokeh]]
-   [`[2020-11-01]` JupyterLab Documentation — JupyterLab 2.3.0a1 documentation](#sjpytrlbrdthdcsnstbljpytrlbdcmnttnjpytrlbdcmnttn) 
-   [`[2020-11-11]` raphaelvallat/pingouin: Statistical package in Python based on Pandas](#sgthbcmrphlvlltpngnrphlvlsttstclpckgnpythnbsdnpnds) 
-   [`[2020-10-31]` How I built a spreadsheet app with Python to make data science easier | Hacker Noon](#shckrnncmntrdcnggrdstdsprwthpythntmkdtscncsrhckrnn) [[spreadsheet]]
-   [`[2020-10-28]` I just updated my Pandas GUI project to have some sample datasets, here it is working with a Simpsons dataset and proving that the early seasons are the best&#x2026; /r/compsci](#srddtcmrcmpsccmmntsjjfysjgthtthrlyssnsrthbstrcmpsc) 
-   [`[2019-11-24]` Jupyter tools to increase productivity - Towards Data Science](#jpytrtlstncrsprdctvtytwrdsdtscnc) [[jupyter]]
    -   [`[2020-05-12]` widgets, debugging, toc](#wdgtsdbggngtc) 
    -   [`[2020-09-10]` from IPython.core.debugger import set<sub>trace</sub>](#frmpythncrdbggrmprtsttrc) 
-   [need to post it somewhere&#x2026; but not sure how to present to people. could def post some plots to quantifiedself?](#ndtpsttsmwhrbtntsrhwtprsnplclddfpstsmpltstqntfdslf) [[dashboard]] [[toblog]] [[qs]]
-   [`[2019-04-09]` Short- and long-term effects of a single bout of exercise on heart rate variability: comparison between constant and interval training exercises. - PubMed - NCBI](#shrtndlngtrmffctsfsnglbtftndntrvltrnngxrcsspbmdncb) [[hrv]]
-   [`[2019-08-17]` Plotting with categorical data — seaborn 0.9.0 documentation](#plttngwthctgrcldtsbrndcmnttn) [[viz]]
    -   [`[2020-09-02]` not sure if boxplots in particular are usefult to me?](#ntsrfbxpltsnprtclrrsflttm) 
-   [thinking about making it public](#thnkngbtmkngtpblc) [[hpi]]
-   [add more dashboards to web?](#ddmrdshbrdstwb) 
    -   [`[2019-04-10]` could add to dashboard?](#cldddtdshbrd) 
-   ['Other' workouts i'm using for HR decay  &#x2013; shit, I think I lost hr here after 10th minute.  Could detect it automatically I guess?](#thrwrktsmsngfrhrdcyshtthntrthmntclddtctttmtcllygss) [[qs]] [[hr]]
-   [always keep a tab running on one for my desktops? or pinned](#lwyskptbrnnngnnfrmydsktpsrpnnd) 
-   [`[2019-04-06]` shit. influxdb seems to be very unsuitable for the kind of thing I want. also very awkward to render dashboards&#x2026;](#shtnflxdbsmstbvrynstblfrtwntlsvrywkwrdtrndrdshbrds) [[influxdb]]
    -   [`[2021-02-13]` hmm I guess what I meant is that it's for aggregate data only, and a bit awkwards to explore by-point data?](#hmmgsswhtmntsthttsfrggrgtnlyndbtwkwrdstxplrbypntdt) 
-   [I really want proper and fast location history..](#rllywntprprndfstlctnhstry) [[location]]
-   [run with cachew? also integrate with hpi](#rnwthcchwlsntgrtwthhp) [[cachew]] [[nutrino]]
-   [show my dashboard](#shwmydshbrd) [[qs]] [[social]]
-   [`[2020-09-01]` Pandas API — hvPlot 0.6.0 documentation](#shvplthlvzrgsrgdpndsphtmlpndsphvpltdcmnttn) 
-   [mixing in data from taplog](#mxngndtfrmtplg) [[weight]] [[exercise]] [[qs]]
-   [on the hrv plot, diplay as arrow if the trend is up or down](#nthhrvpltdplysrrwfthtrndsprdwn) [[sleep]]
-   [`[2020-11-03]` joshlk/dataclassframe: A container for dataclasses with multi-indexing and bulk operations.](#sgthbcmjshlkdtclssfrmjshllssswthmltndxngndblkprtns) 
    -   [`[2021-02-06]` ah ok, something added.. maybe reevaluate it later](#hksmthngdddmybrvlttltr) 
-   [use for daily dashboard or something?](#sfrdlydshbrdrsmthng) [[remarkable]]
-   [`[2020-09-06]` bokeh/notebook<sub>embed.ipynb</sub> at 2.2.1 · bokeh/bokeh](#sgthbcmbkhbkhblbxmplshwtspynbbkhntbkmbdpynbtbkhbkh) 
-   [https://github.com/thesephist/histools](#sgthbcmthsphsthstls) [[dashboard]] [[viz]]
-   [`[2020-12-30]` manual<sub>exercise</sub>](#mnlxrcshtmlmnlxrcs) [[bokeh]]
-   [Grafana](#grfn) [[timeline]]
    -   [uhh. so unclear how to connect my data to grafana.](#hhsnclrhwtcnnctmydttgrfn) 
    -   [lastfm](#lstfm) 
    -   [I guess, start with weight for simplicity](#gssstrtwthwghtfrsmplcty) 
    -   [then, do sleep](#thndslp) 
-   [figure out grafana..](#fgrtgrfn) 
-   [post on dataisbeautiful?](#pstndtsbtfl) [[reddit]] [[sleep]]
-   [fix dovpandas warnings](#fxdvpndswrnngs) 
-   [when I release it, make sure it works both against public and private hpi bits](#whnrlstmksrtwrksbthgnstpblcndprvthpbts) [[sleep]]
-   [profile stuff a bit?](#prflstffbt) 
-   [`[2020-12-05]` xkcd: Linear Regression](#sxkcdcmxkcdlnrrgrssn) [[toblog]]
-   [`[2019-04-15]` Python Data Visualization 2018: Why So Many Libraries? - Anaconda](#pythndtvslztnwhysmnylbrrsncnd) 
    -   [`[2019-09-10]` try using in dashboard](#trysngndshbrd) 
-   [`[2019-04-14]` iris<sub>splom.py</sub> — Bokeh 1.1.0 documentation](#rssplmpybkhdcmnttn) 
    -   [`[2019-07-23]` eh, defaults don't look great. maybe it's faster but unclear](#hdfltsdntlkgrtmybtsfstrbtnclr) 
-   [`[2020-10-25]` Tableau Desktop](#swwwtblcmngbprdctsdsktptbldsktp) [[viz]] [[qs]]
-   [-----&#x2013;&#x2014; last housekeeping on `[2021-02-06]` ----------](#lsthskpngn) 
-   [can overlay activity data vs sleep data from different tools?](#cnvrlyctvtydtvsslpdtfrmdffrnttls) [[dashboard]] [[sleep]] [[hpi]]
-   [`[2021-02-12]` grafana/worldmap-panel: Worldmap panel plugin for Grafana 3.0 that can be overlaid with circles for data points.](#sgthbcmgrfnwrldmppnlgrfnwhtcnbvrldwthcrclsfrdtpnts) [[location]] [[dashboard]]
-   [`[2021-02-18]` Personal Dashboards for Self-Tracking Data - Quantified Self / Apps & Tools - Quantified Self Forum](#sfrmqntfdslfcmtprsnldshbrqntfdslfppstlsqntfdslffrm) [[hpi]] [[dashboard]] [[publish]]
-   [could use mybinder for demos? same used by jupyterlab](#cldsmybndrfrdmssmsdbyjpytrlb) [[dashboard]] [[hpi]]
-   [`[2021-04-11]` LibrePhotos/librephotos: Self hosted alternative to Google Photos](#sgthbcmlbrphtslbrphtslbrpphtsslfhstdltrntvtgglphts) [[photos]] [[memex]]
-   [`[2021-04-11]` photoprism/photoprism: Personal Photo Management powered by Go and Google TensorFlow](#sgthbcmphtprsmphtprsmphtpmngmntpwrdbygndggltnsrflw) [[photos]] [[memex]]
-   [`[2021-03-05]` Introducing Orion: A Powerful Substitute for OwnTracks Recorder - Blog - Kevin Lin](#sblgkvnlnnfpstntrdcngrnpwtttfrwntrcksrcrdrblgkvnln) [[location]] [[HPI]] [[dashboard]]
-   [`[2019-09-30]` Jupyter notebooks on steroids](#jpytrntbksnstrds) [[dashboard]] [[ipynb]]
    -   [`[2019-10-06]` try ipywidgets?](#trypywdgts) 
-   [`[2021-04-29]` Personal Dashboards for Self-Tracking Data - Quantified Self / Apps & Tools - Quantified Self Forum](#sfrmqntfdslfcmtprsnldshbrqntfdslfppstlsqntfdslffrm) [[qs]]

Dashboard (not a very unique name, I know) is a set of tools to visualize personal data on a, well, some sort of dashboard.  

I'm gradually publishing it [here](https://github.com/karlicoss/dashboard) and got some old screenshots [here](https://www.reddit.com/r/QuantifiedSelf/comments/cokt4f/what_do_you_all_do_with_your_data/ewmucgk).  

Ideally I'd like to reuse existing libraries and other people's projects to the maximum extent possible, so we could join forces.  




# related 





## used to visualize #qs data      [[qs]]




## very similar to #timeline and #memex      [[timeline]] [[memex]]

I haven't quite figured out the difference as well yet. Likely will merge in a single tool.  




## #hpi provides data for my dashboard      [[hpi]]

Although in theory you can plug in any Pandas dataframes in it (assuming they fit the schema).  




# \* motivation

-   same motivation as for [quantified self](../quantifiedself/qs.md)
-   a 'research' goal: figuring out the patterns and common routines for processing and preparing this data for visualizing.




## why not use something existing?

-   low-code/no-code 'platforms' I've seen aren't enough to deal with noisy data or novel usecases.  
    -   filtering outliers, correcting data, etc., is mipossible in a no-code environment
    -   something like seasonality detection would be impossible without a real programming language

-   interoperability: if you want some data source that the platform doesn't support, too bad.




## figuring out core patterns for manipulating and representing this data

Many things are very tedious to redo and reinvent from scratch every time  

-   \#datetime handling  
    -   missing dates (e.g. parsing errors)
    -   some data sources hane timezones, some don't.  
        Some are a mixture, which is even worse. E.g. depending on the language you can't sort the dates with mixed timezones.
-   \#errors handling  
    Quantified self data is often fuzzy/incomplete etc. If manual inputs are involved, parsing errors are inevitable.  
    While in most software it's reasonable to crash on the first error, this would be very annoying if your dashboard breaks of one broken data point!  
    On the other hand, you don't want to filter out errors either, since you'd never know they were present in the first place.  
    
    So it needs to be something in between, a pattern for propagating errors as far as possible, and handling them gracefully during the visualization phase.

-   detecting holidays  
    E.g. for almost all data it makes sense to differentiate/correlate against days off work

-   geographical/location data




## automatically detecting interesting correlations between data





### `[2019-08-15]` wonder if massive dataframe with literally everything could help




### maybe just go over all series? and then generate all pairwise correlations and sort by correlation coefficient + R<sup>2</sup>? some sort of pareto surface?




## what I want to figure out:





### very similar to <https://github.com/KrauseFx/FxLifeSheet#questions-to-answer>




### are 'sleep phases' a thing (or at least the way they are measured in conventional tackers)? how do they impact my waking up, alertness etc?      [[sleep]]




### `[2020-10-27]` calculating custom exercise stats

e.g. I have a few traffic lights on my way that might affect my speed/cadence data, and I might want to filter it out  




## custom/personalized data processing





### splitting exercise into cardio and non-cardio

-   with cardio (at least, endurance styl) there is a somewhat convincing metric &#x2013; number of heartbeats, which is basically the same as calories burnt?
-   with strength training this is something very hard to measure and not sure if makes sense at all?




## demo of errors: typical mistake is confuising wlog and weight tags (weight gets unrecognized as exercise)      [[dashboard]]




# \* inspiration





## `[2018-06-06]` [andreilyskov: qs dashboard example](https://qself-dashboard.herokuapp.com)      [[qs]]

-   "so if you want to collaborate feel free to email me"




### `[2019-04-06]` interesting dashboards: spotify, writing and reading. otherwise not that much stuff




### `[2020-08-22]` ok seems that they use similar architecture to mine <https://forum.quantifiedself.com/t/personal-dashboards-for-self-tracking-data/8202/4>




## `[2020-08-22]` [Flow Dashboard](https://flowdash.co/app/about)

ok, looks kinda slick..  
open source: <https://github.com/onejgordon/flow-dashboard>  

    Public Github commits
    Google Fit - track any activity durations by keyword
    Evernote - pull excerpts from specified notebooks
    Pocket - Sync stored articles & add notes
    Goodreads - Sync currently reading shelf
    Track any abstract data via REST API




### `[2021-02-06]` ok, rest api thing is cool, should try connecting it to #hpi      [[hpi]]




## `[2019-11-24]` [heedy/heedy: An Open-Source Platform for Quantified Self & IoT](https://github.com/heedy/heedy)

    Heedy is an open-source aggregator built for storage and analysis of your personal data.
    It provides a powerful plugin system, allowing easy integration with various services, as well as deep extensibility.

    Extensible: Even a system with fantastic visualizations and powerful analysis has limited utility.
    This is because it can only show what the original authors assumed would be useful. Heedy offers a powerful plugin system - plugin writers can add new integrations, plots, or even modify core functionality with a few lines of python or javascript.
    A registry is planned, so that users can install plugins with the click of a button.

-   `[2020-08-23]` interesing, automatic jupyter notebook connection??
-   `[2021-02-06]` yeah looks like very much what I want
-   `[2021-04-27]` hmm  
    seems that fitbit integration is the only one present so far  
    however after giving it a go, it restarted a couple of times, and ended up with a couple of zombie processes  
    couldn't restart it without completely tearing down the docker container :(  
    Overall not sure where it all fits: there are lots of repositories and not many concrete usecases <https://github.com/heedy>




## `[2019-05-21]` [quelf/report.Rmd at master · JakobGM/quelf](https://github.com/JakobGM/quelf/blob/master/analysis/report.Rmd)

jupyter notebooks  

    Sleep data [sleep as android, sleepcycle]
    Study hours [toggl]
    Exercise [runkeeper, strong]
    Programming [wakatime]




## `[2019-09-22]` [markwk/qs<sub>ledger</sub>: Quantified Self Personal Data Aggregator and Data Analysis](https://github.com/markwk/qs_ledger)      [[qs]] [[dataliberation]]

interesting, but data exports are not very reusable  




### `[2019-09-28]` I guess once I export everything could send a link to that guy?




## `[2020-09-03]` <https://github.com/KrauseFx/FxLifeSheet>

    the dashboard is currently hard-coded in Google Data Studio




## `[2020-08-22]` some good dashboards   <https://forum.quantifiedself.com/t/personal-dashboards-for-self-tracking-data/8202/15>

workouts, weight, sleep, hr  




## Juno's Personal Data Exploratory  <https://exploratory.openhumans.org/notebooks>      [[pkm]] [[qs]]




## `[2020-07-02]` [jeffshek/betterself: Your body's dashboard.](https://github.com/jeffshek/betterself)

<https://github.com/jeffshek/open>  




### `[2020-08-24]` demo <https://app.betterself.io>

-   table with notes is kinda nice?  
    eh. would be nice to have something automatic for dataframes




## `[2019-01-13]` [Sacha Chua: quantified awesome](http://quantifiedawesome.com)      [[qs]]

realtime dashboard  

-   source: <https://github.com/sachac/quantified>




### `[2019-04-06]` ok, looks pretty clean, but might require some tinkering




### `[2021-02-06]` also pretty much only time tracking?




## `[2020-09-10]` [quantifiedbob/bob-body-composition-viz: Jupyter Notebook vizualizing 10+ years of my body composition data](https://github.com/quantifiedbob/bob-body-composition-viz)

ok, but just a plot  




## `[2020-04-04]` [ammanvedi/quantified-self-server: Aggregate data about myself (workouts, blog posts, music listening history) into a graphql API](https://github.com/ammanvedi/quantified-self-server)

    Blog posts (markdown from github)
    Workout data (Strava API)
    Recent music (Tidal API)
    into one graphql API that can be called from my personal site.




## `[2019-04-19]` [markwk: How to Create a Time Tracking Dashboard using RescueTime, IFTTT and Google Sheets](http://www.markwk.com/data-processing-time-tracking.html)      [[qs]]

ok, but too low code for me  




## `[2019-01-08]` [Personal Dashboard](https://reddit.com/r/QuantifiedSelf/comments/acxy1v/personal_dashboard/) /r/QuantifiedSelf

    https://i.redd.it/ufpm4s9k0o821.png




### `[2019-04-11]` it is not very elaborate though&#x2026;




## minor ideas





### keeping query in the address string is pretty clever&#x2026; can bookmark and easily restart it!      [[datasette]]




### `[2020-08-22]` event chart <https://forum.quantifiedself.com/t/best-examples-of-quanitified-self-dashboards/4590/9>




### use tabs within tabs? kinda like in garmin <https://connect.garmin.com/modern/activities>




### `[2020-10-27]` [Garmin Connect](https://connect.garmin.com/modern/activity/5736337040)

pretty nice clean visualizations, I need to borrow these I guess  




## `[2021-01-11]` [yihong0618/running<sub>page</sub>: Make your own running home page](https://github.com/yihong0618/running_page)




# \* implementation

How to actuallly implement it, which software/tools/libraries to use.  




## (meta?)goals 

-   interact with the backend (so it's possible to reload newer data)  
    plotly can do it, bokeh can as well  
    -   ideally, autorefresh?
-   remember the state (e.g. various panes on/off etc)
-   be hackable  
    -   via js
    -   autoreload the code for faster iteradion?
-   be able to derive new data on the fly? not sure how to achieve this in the browser
-   have a jupyter interface for better interactivity? ideally, 'edit' any tab as a jupyter notebook




### keep it modular, I guess

have a core subpackages and various tabs&#x2026; not sure how to refactor them out later  




### `[2020-09-01]` similarly to HPI, it's more of a demonstration how it can be done. Ideally people would be able to reuse core and build their own dashboards




## it's very important to benefit from the existing data science infrastructure as much as possible. jupyter, pandas, etc.




## `[2020-12-10]` [panel · PyPI](https://pypi.org/project/panel/)

<https://panel.holoviz.org/>  

    A high-level app and dashboarding solution for Python
    Panel works with visualizations from Bokeh, Matplotlib, HoloViews, and many other Python plotting libraries

ok, this is super promising:  

    Panel can also be used with the separate Param project to create interactively configurable objects with or without associated visualizations, in a fully declarative way. With this approach, you declare your configurable object using the pure-Python, zero-dependency param library, annotating your code with parameter ranges, documentation, and dependencies between parameters and your code. Using this information, you can make all of your domain-specific code be optionally configurable in a GUI, with optional visual displays and debugging information if you like, all with just a few lines of declarations. With this approach, you don’t ever have to decide whether your code will eventually be used in a notebook, in a GUI app, or completely behind the scenes in batch processing, servers, or reports – the same code can support all of these cases equally well, once you declare the associated parameters and constraints.




## `[2020-12-07]` [oschuett/appmode: A Jupyter extensions that turns notebooks into web applications.](https://github.com/oschuett/appmode)

    A Jupyter extensions that turns notebooks into web applications.




### `[2021-02-06]` ok, nice, has 'edit app' button which opens jupyter to edit??




## `[2020-08-23]` ok, #jupyter is the ultimate ad-hoc solution. it preserves state, can be exposed as a frontend and allows for python code




## bokeh vs plotly dash

there are couple of example apps here  
<https://www.sicara.ai/blog/2018-01-30-bokeh-dash-best-dashboard-framework-python>  

bokeh  

-   seems snappier?

plotly:  

-   possibly better html elements support?




### `[2020-09-03]` compromise: keep it as framework independent and decoupled as possible. Support both frameworks!




## basically have a core library that's imported in all notebooks. move stuff to core as long as possible, but allow quick button to mess with the data in notebook      [[toblog]]




## try jupyterlab




## I think dashboard needs to preserve state somehow, it's annoying to edit code every time.. wonder if dash supports it?




## use multiprocessing&#x2026;

pretty sure pandas frames can be easily serialised?  




## `[2020-09-10]` [Top 50 matplotlib Visualizations - The Master Plots (w/ Full Python Code) | ML+](https://www.machinelearningplus.com/plots/top-50-matplotlib-visualizations-the-master-plots-python/)

    39. Time Series Decomposition Plot

ok, this is pretty intersting  
re: autocorrelation &#x2013; what was up with the 'blue region', significance thing??  
also good: Seasonal Plot  
would be initersting to quickly toggle it in dashboard?  




## grafana could simply be one of the interfaces




## `[2021-02-17]` [apache/superset: Apache Superset is a Data Visualization and Data Exploration Platform](https://github.com/apache/superset#superset)      [[dashboard]] [[hpi]]

    A modern, enterprise-ready business intelligence web application.

whoa looks interesting&#x2026;  

-   `[2021-04-26]` trying sqlite connection

Ugh. it didn't really work &#x2013; seems to be in the process of deprecation  
<https://github.com/apache/superset/issues/9748>  
and still, getting some weird error regardless whether I mount database as read only or not.. and no other logs  

    2021-04-26 14:19:42,813:WARNING:superset.views.base:[SupersetError(message='(sqlite3.OperationalError) unable to open database file\n(Background on this error at: http://sqlalche.me/e/13/e3q8)', error_type=<SupersetErrorType.GENERIC_DB_ENGINE_ERROR: 'GENERIC_DB_ENGINE_ERROR'>, level=<ErrorLevel.ERROR: 'error'>, extra={'engine_name': 'SQLite', 'issue_codes': [{'code': 1002, 'message': 'Issue 1002 - The database returned an unexpected error.'}]})]

-   `[2021-04-26]` right, managed to run against postgre..

a bit finicky overall&#x2026;  
I guess nice that it's possible to separate queries, charts and dashboards&#x2026;  
so one can reuse them in different contexts/for different visualizations  

-   `[2021-04-26]`  
    for fuck's sake, struggling with creating a 'virtual' view with calculated columns&#x2026;  
    getting an error like  
    
        Error: column "_cachew_union_repr_measurement_temp" does not exist
-   `[2021-04-26]` seems possible to share queries?




# \* sleep dashboard/experiments      [[sleep]]

Sleep is one of the biggest things I wanna figure out, and I have quite a few ideas of what to test.  




## Maybe run pca for my sleep data?      [[sleep]] [[qs]] [[ml]]




## figure out main questions I wanna figure out      [[qs]] [[sleep]]





### e.g. 'what is the best time for me to go asleep'?




### 'what is the best sleep duration?'




## `[2019-08-21]` Respiratory rate - Wikipedia      [[sleep]]

<https://en.m.wikipedia.org/wiki/Respiratory_rate>  

    For humans, the typical respiratory rate for a healthy adult at rest is 12–18 breaths per minute.[




### `[2020-08-24]` add to dataframe




## correlate with sliding exponential mean instead?      [[sleep]]




## add date to tooltip      [[sleep]]




## def need to highlight holidays on the background (also annotate if it was indeed a day off), e.g. where have I gone      [[sleep]]




## wonder if coverage is correlated with sleep movement&#x2026;      [[sleep]]




## find correlation between bedtime and length of sleep?      [[sleep]]




## Sleep/exercise correlation: could try different deltas/correlation coeff plot




## old sleep logs from taplog?      [[sleep]]




## check waking up in REM?      [[sleep]]




## interesting correlation: sleep vs bed time. wonder if that means REM or something?




## hmm, sleepy correlates negatively with ex. volume?




## hmm. temperature is interesting &#x2013; looks like it's negatively correlating with HR??      [[qs]]




## sleep plot: highlight holidays/weekends as background color?




## movements/bed exit in emfit?





### `[2020-08-25]` could plot on the sleep bars plot?




## integrate old melatonin experiment, maybe post about it




## use ANS balance from emfit?




## `[2018-06-20]` Emfit qs estimated my sleep high, even though i felt a bit like shit. I wonder if it just correlates with sleep length..




## temperature during sleep      [[qs]] [[sleep]]




## different style for sleep length bars? currently red and blue are sort of annoyingly make it hard to spot the pattern?      [[emfit]]




## Average temperature      [[sleep]]




## cross correlate with rescuetime activity      [[sleep]]





### `[2020-08-25]` could even plot activity bars




## figure out alarm wakeup vs 'natural' wakeup, could tell me something about sleep intervals      [[qs]]




## Emfit recovery &#x2013; wonder if it correlated with exercise days      [[sleep]] [[emfit]]




## My daughters sleeping patterns for the first 4 months of her life. One continuous spiral starting on the inside when she was born, each revolution representing a single day. Midnight at the top (24 hour clock). [OC]      [[sleep]] [[inspiration]] [[viz]]

<https://i.reddituploads.com/10f961abe2744c90844287efdd75ba47?fit=max&h=1536&w=1536&s=f019986ae2343e243ed97811b9f500fe>  
Huh that's a nice way to save on space  




## Melatonin analysis

[Zeo sleep self-experiments](https://www.gwern.net/Zeo)  
[in context](https://hyp.is/3M2-CBdeEeqfbf-fPLr3tw/www.gwern.net/Zeo)  




## wonder what does it mean when morning hrv is higher than evening??      [[qs]] [[hrv]]




## I wonder what happened&#x2026; at some point (around august 2019), coverage  has consistently gone up to 100      [[qs]] [[emfit]]




## Track pizza dependency?      [[qs]] [[sleep]]




## Shit wonder if I'm oversleeping because it's too cold?      [[qs]] [[sleep]]




## pretty strong negative correlation of temp vs avg hr. wonder if that's searsonal or not? post about it soon?      [[qs]]




## look at HRV peaks and try to see what's happening?      [[qs]] [[timeline]]




## `[2019-11-14]` Опыт обращения к сомнологу      [[qs]] [[sleep]]

<http://vsevolodustinov.ru/blog/all/opyt-obrascheniya-k-somnologu/>  

    . Никакого алкоголя
    . Избегать физнагрузку после 17:00. Нагрузка до 17:00 наоборот улучшает сон

try recommendataions from that post and see how they apply to me?  




## Compare hr/hrv before and after holidays      [[qs]] [[sleep]] [[hpi]]




## Compute differences between rem cycles and plot on histogram?      [[qs]] [[sleep]]




## wow, emfit recovery was really shit last night. why???&#x2026; seriosly no reason for it      [[qs]] [[sleep]]




## wip on figuring out if weekdays impact sleep      [[qs]]

    import my.emfit
    by_night = my.emfit.by_night()
    data = [{'date': x.date, 'hr': x.measured_hr_avg} for x in by_night.values()]
    by_dt = pd.DataFrame(data).set_index('date')
    by_dt = by_dt.set_index(pd.to_datetime(by_dt.index))
    onday = lambda d: (d == by_dt.index.dayofweek)
    we = by_dt[onday(0) | onday(1) | onday(6)]
    wd = by_dt[onday(3) | onday(4) | onday(5)]
    ax = wd.rolling('30D').mean().plot()
    we.rolling('30D').mean().plot(ax=ax, color='red')
    plt.show()




## plot my emfit sleep, to be fair even two years of plots is quite cool      [[publish]] [[qs]]




## hmm, my hrv really has fallen down? also sleep hr gone up      [[qs]] [[health]]

wonder if it's related to my quality of sleep?  




## track dependency on meditaion?      [[sleep]]




## display times in bed definitely&#x2026;      [[sleep]]




## would be nice to plot against sunrise/sunset?      [[sleep]]




## `[2020-09-30]` [Relationships between HRV, sleep and physical activity in personal Oura ring data - Quantified Self / General Health - Quantified Self Forum](https://forum.quantifiedself.com/t/relationships-between-hrv-sleep-and-physical-activity-in-personal-oura-ring-data/8524)      [[hrv]] [[hr]] [[sleep]] [[exercise]]

nice, pretty similar to my findings?  




## `[2020-09-30]` fucking hell! after naples HRV jumped and HR dropped very significantly      [[self]] [[sleep]]




## correlate dreams with rem/deep etc?      [[sleep]]




## wtf&#x2026; without seasons it seems to correlate less??      [[sleep]]




## negative correlation of coverage with temperature is pretty weird      [[emfit]]




## Compare fitbit      [[hr]] [[qs]]




## For sleep, probably a good idea to log room temperature      [[sleep]] [[qs]]




## hmm, maybe I need to remove seasonality from the sleep first and then search other correlations?? not sure..




## ugh. today is gonna be confusing      [[qs]] [[sleep]]

exercise will probably have a lot of impact&#x2026; but then hr is elevated because of the pizza  




### `[2020-10-18]` maybe really need to try two-parameter regression?




### `[2020-10-18]` take into the account past pizza orders? this is gonna have systematic impact on my sundays?




# \* exercise dashboard/experiments





## running dashboard &#x2013; custom dataframe + add distance + merge with manual notes in a similar way




## thinking how to contribute data for the energy plot      [[exercise]] [[qs]]

maybe the data is sifted through the elliptical/running/spinning modules and what's left is just taken as is  




## have some stuff in endomondo comments&#x2026; need to extract it and use. maybe actually just reuse endoexport, and put in a df      [[qs]]




## Show distance on speed/hr plot      [[qs]]




## def need to measure decay to 60 to get more data&#x2026;      [[qs]] [[hr]] [[toblog]]




## process google location and guess walks from it      [[exercise]] [[qs]]




## Detect walks and runs from google data and plot them. Mark velocity with colours. Could also do 'walking intervals' (e.g. if was in a shop inbetween)      [[exercise]]




## calculate some sort of 'integral' heart rate and also score for interval trainings?      [[exercise]]





### `[2020-09-06]` eh? maybe I wanted to break down my interval trainings per activity bursts?




## integrate elliptical workouts? Could plot workout specific things and make them easy to compare




## filter out specific exercises and plot separately to see the progress      [[exercise]]




## go through the most common exercise (past) sessions and check them      [[exercise]]





### `[2021-02-06]` I guess it's a more general pattern for reviewing data too




## exercise provider: trust more notes which got HR data      [[qs]]




## Look at hr data, its almost 180 all the time. Is it because i was doing cardio less?      [[qs]] [[health]] [[exercise]]




# \* patterns

as in, patterns of working with data, best practices for visualizing things etc  




## use dynamic sliders for different regression windows




## Always plot isolated metrics (temp, hr, etc) &#x2013; good for debugging      [[qs]]





### `[2020-09-03]` also make sure it's easy to do




## restrict datapoints 'by experiment'? same way it's done with date sliders?




## need to try different date shifts to see it's not correlated




## labels: need to display weekday (also on HR nodes?)




## would be nice to zoom individual plots..




## \* error hanling      [[errors]]





### about importance of error handling when working with personal data      [[toblog]]

data is inherently messy and error prone  
it's sensible to be defensive and try to relax as much as possible (unless you have time to literally tend to them immediately)  
on the other hand, you want to make sure you are aware about the issues in data  
example: running dashboard &#x2013; has a warning about 0 speed  
see screenshot at the same time (fix JS table first so duration & start<sub>time</sub> have proper rendering)  
you can instantly see it on the plot (yellow markers). if you hover, you'll see that the error is about zero speed (and you can also see it in the table)  
in the table, you can clearly spot that the problem is the treadmill &#x2013; indeed, treadmill wasn't connected to the phone in any way, and I'm stationary, so endomondo has no idea how much I moved  
however, I did log the distance (along with the training regime) manually  
by combining the HR data (recorded by endomondo) and manual data we get the complete representation  
(if I add visual highlight on the table, that would be fucking amazing)  

-   `[2020-09-14]` maybe post on QS forum??




### error handling &#x2013; demonstrate on 'multiple sleeps'




### demo: running speed/hr plot is a good candidate

-   show both types of errors (zero speed/no HR)
-   need to disable tooltip on avg plot
-   would be nice to highlight the point under the tooltip?




### demo: unmark one of cardio/non-cardio and demonstrate warnings




### document error handling pattern with 'error'      [[errors]] [[toblog]]




## for correlations, there is overview + zoomed in individual plots showing all the errors, outliers, etc




## Each rolling plot can also handle seasonality, residuals etc?




## would be cool to scale arbitrarily vertically and horizontally, the whole plot




## indicate how recent datapoints are by color? (in the correlations)




## corr plot: include influence/leverage etc




## would be nice to display data source?

e.g. for blood dashboard  




### `[2019-07-20]` links to event sources (e.g. emfit etc)


-   `[2020-09-20]` maybe could be automatic/agnostic? add to cdf check?




### `[2019-04-12]` src in exercise volume




### add src for jawbone/emfit sleep




## link to original event from point? or just 'context'

e.g. endomondo  




## vertical line tooltip sucks&#x2026; probably need a single point instead




## definitely need to take seasonality (e.g. weekly) into the account, e.g. for multi regression




## I guess need seasonality analisys for each metric? maybe have it on a separate pane, e.g. 'debug/insights'? would be nice to do it for all dataframes?




## would be nice to include the org file link to the context&#x2026; then could use mimemacs for it      [[promnesia]]




# \* ideas for more dashboards





## rescuetime summarizes my sleep intervals pretty well? could at least have upper bound on sleep during holidays/when not using emfit?      [[rescuetime]] [[hpi]]




## temperature &#x2013; probably, seasonality?      [[qs]]




## display photos as an optional layer along with the map?





### `[2020-09-06]` just need to integrate dashboard with photomap




## links into food dashboards.. I guess I need anchors.      [[nutrino]]




## favsmap should be part of dashboard&#x2026; also could be the first bit in my public dashboard?

merge google and foursquare, display google labels on top of osm mapS  
rationale: various tools for working with maps in one place  




## shit. if I had food stats that would be just amazing




## takeout &#x2013; contains list of places      [[takeout]] [[hpi]]

basically could merge with 4sq? and custom addresses  




## money? not sure




## quantified mind? already have plots




## Add check-ins to favsmap




# \* ideas for experiments





## correlate number of commits/lines vs sleep?




## glucose and ketone measurements vs food?





### `[2020-09-06]` probably not enough data&#x2026;




## correlate temp sensor with hiking?      [[toblog]] [[qs]] [[lifelogging]]




## hmm, maybe need to try running/eating pizza on a different day? to make sure the seasonality is not due to running?      [[exercise]] [[qs]] [[sleep]]





### `[2020-10-24]` or could check seasonality for months that didn't involve running?




## volume vs avg temp is an interesting one to demonstrate the correlation that shouldn't exist

(although again in theory there might be some seasonality)  




## try to find correlation between sleep and exercise?      [[qs]]

-   State "DONE"       from "TODO"       `[2019-04-06]`

in the simplest approach, try to only use cardio and see how it correlates (binary, for instance). although not enough points..  




## temperature plots: would be interesting to have avg plot for 'indoors' and 'outdoors' periods?




## plot spinning power vs heartbeats?      [[qs]]




# \* plotly dash      [[plotly]]

For now using #bokeh instead  




## `[2019-10-27]` plotly/dash@1.4.0

    plotly/dash@v1.4.0
    Dash v1.4.0




## `[2020-04-10]` Re: [plotly/plotly.py] Importing plotly takes a lot of time (740)

    Import time and initialization time should be much improved on Python 3.7 with PR 2368.




## `[2019-04-10]` Dash offline is enabled?  plotly/dash

<https://github.com/plotly/dash/issues/46>  

    from dash import Dash
    
    app = Dash()
    
    app.css.config.serve_locally = True
    app.scripts.config.serve_locally = True




## wow. showing points on other plots while rectangle selection is really awesome      [[plotly]]




## would be really nice to properly render pairplots in plotly




## err. seems to always consume cpu in background




## `[2020-08-26]` Re: plotly/plotly.py Importing plotly takes a lot of time (740)

    Re: [plotly/plotly.py] Importing plotly takes a lot of time (740




## `[2019-04-07]` Dash User Guide and Documentation - Dash by Plotly

<https://dash.plot.ly/dash-core-components/tabs>  

    Note that this method has a drawback: it requires that you compute the children property for each individual tab upfront and send all of the tab's content over the network at once. The callback method allows you to compute the tab's content on the fly (that is, when the tab is clicked).




## `[2019-05-30]` ucg8j/awesome-dash: A curated list of awesome Dash (plotly) resources      [[viz]]

<https://github.com/ucg8j/awesome-dash>  




### `[2019-07-24]` <https://dash-gallery.plotly.host/Portal/>




### `[2019-07-24]` eh, dunno otherwise not so interesting? maybe I'm not really lacking anything, I can think of many things I can add that still need to be implemented..




# ----------------------------------------- 




# come up with a better name? just in case of pypi release&#x2026;




# how to detect temporal correlation?      [[study]] [[qs]]





## `[2020-09-01]` ok, this lag thing in bokeh could work




# `[2019-04-19]` qs<sub>ledger</sub>/example<sub>correlation</sub><sub>explorer</sub><sub>with</sub><sub>plotly.py</sub> at master · markwk/qs<sub>ledger</sub>

<https://github.com/markwk/qs_ledger/blob/master/example_correlation_explorer_with_plotly.py>  
plotly dash regression example  




# `[2019-10-15]` [Why you should continuously track your energy level and what I've learned from it.](https://reddit.com/r/Biohackers/comments/di60ub/why_you_should_continuously_track_your_energy/) /r/Biohackers      [[qs]]





## `[2019-10-18]` about tracker matching subjective score




# not sure what mavg is doing. e.g. HR plots of specific exercise &#x2013; if I didn't exercise during the past month mavg for 14 days should just take value of my last exercise. right??





## `[2020-09-03]` need to test it, just to double check




# `[2019-04-11]` Visualization — pandas 0.24.2 documentation      [[viz]]

<https://pandas.pydata.org/pandas-docs/stable/user_guide/visualization.html#visualization-autocorrelation>  




# `[2020-09-16]` [Building a Data Dashboard - Quantified Self / Apps & Tools - Quantified Self Forum](https://forum.quantifiedself.com/t/building-a-data-dashboard/449)




# `[2020-08-23]` [All | Search powered by Algolia](https://hn.algolia.com/?dateRange=all&page=0&prefix=true&query=hvplot&sort=byPopularity&type=all)

    Panel, hvPlot, HoloViews, GeoViews, Datashader, Param, Colorcet -- all working together to make Python data visualization easier and more powerful.




# `[2020-10-11]` [Accelerating with WebGL — Bokeh 2.2.1 Documentation](https://docs.bokeh.org/en/latest/docs/user_guide/webgl.html)





## `[2020-10-11]` [Accelerating with WebGL — Bokeh 2.2.1 Documentation](https://docs.bokeh.org/en/latest/docs/user_guide/webgl.html)

    Only a subset of Bokeh’s objects are capable of rendering in WebGL. Currently supported are the circle and line glyphs, and many markers: asterisk, circle, square, diamond, triangle, inverted_triangle, cross, circle_cross, square_cross, diamond_cross, x, square_x, and circle_x. You can safely combine multiple glyphs in a plot, even if some are rendered in WebGL, and some are not.




## `[2020-10-11]` hmm, didn't seem to have any effect??




# `[2020-10-11]` [FifthHour/correlator: Timeseries correlation in Python, Bokeh Server and on Heroku](https://github.com/FifthHour/correlator)      [[bokeh]]




# `[2020-11-01]` [JupyterLab Documentation — JupyterLab 2.3.0a1 documentation](https://jupyterlab.readthedocs.io/en/stable)




# `[2020-11-11]` [raphaelvallat/pingouin: Statistical package in Python based on Pandas](https://github.com/raphaelvallat/pingouin)




# `[2020-10-31]` [How I built a spreadsheet app with Python to make data science easier | Hacker Noon](https://hackernoon.com/introducing-grid-studio-a-spreadsheet-app-with-python-to-make-data-science-easier-tdup38f7)      [[spreadsheet]]




# `[2020-10-28]` [I just updated my Pandas GUI project to have some sample datasets, here it is working with a Simpsons dataset and proving that the early seasons are the best&#x2026;](https://reddit.com/r/compsci/comments/jjf8ys/i_just_updated_my_pandas_gui_project_to_have_some/) /r/compsci




# `[2019-11-24]` Jupyter tools to increase productivity - Towards Data Science      [[jupyter]]

<https://towardsdatascience.com/jupyter-tools-to-increase-productivity-7b3c6b90be09>  

    Jupyter tools to increase productivity




## `[2020-05-12]` widgets, debugging, toc




## `[2020-09-10]` from IPython.core.debugger import set<sub>trace</sub>




# need to post it somewhere&#x2026; but not sure how to present to people. could def post some plots to quantifiedself?      [[dashboard]] [[toblog]] [[qs]]




# `[2019-04-09]` Short- and long-term effects of a single bout of exercise on heart rate variability: comparison between constant and interval training exercises. - PubMed - NCBI      [[hrv]]

<https://www.ncbi.nlm.nih.gov/pubmed/15461995>  

    R-R intervals, TP, and HF/TP were significantly decreased while LF/TP and LF/HF were significantly increased during the early recovery, when compared with control values. This could be a response to the significant decrease in SAP and DAP at this time. Twenty-four and 48 h after the end of the exercise, HRV parameters were at the same levels as before exercises in the supine posture, but a persistent tachycardia continued to be observed in the upright posture, together with reduced TP values, showing that cardiovascular functions were still disturbed. The short-term HRV recovery seemed dependent on the type of exercise, contrary to the long-term recovery.




# `[2019-08-17]` Plotting with categorical data — seaborn 0.9.0 documentation      [[viz]]

<https://seaborn.pydata.org/tutorial/categorical.html#categorical-tutorial>  

    Boxplots
    The first is the familiar boxplot(). This kind of plot shows the three quartile values of the distribution along with extreme values. The “whiskers” extend to points that lie within 1.5 IQRs of the lower and upper quartile, and then observations that fall outside this range are displayed independently. This means that each value in the boxplot corresponds to an actual observation in the data.




## `[2020-09-02]` not sure if boxplots in particular are usefult to me?




# thinking about making it public      [[hpi]]

where to run it? it's gotta be sufficiently dynamic?  
run from google cloud? suck in the data once? or refresh continuously?  
maybe run the original data retrieval? not sure  




# add more dashboards to web?





## `[2019-04-10]` could add to dashboard?




# 'Other' workouts i'm using for HR decay  &#x2013; shit, I think I lost hr here after 10th minute.  Could detect it automatically I guess?      [[qs]] [[hr]]




# always keep a tab running on one for my desktops? or pinned




# `[2019-04-06]` shit. influxdb seems to be very unsuitable for the kind of thing I want. also very awkward to render dashboards&#x2026;      [[influxdb]]





## `[2021-02-13]` hmm I guess what I meant is that it's for aggregate data only, and a bit awkwards to explore by-point data?




# I really want proper and fast location history..      [[location]]




# run with cachew? also integrate with hpi      [[cachew]] [[nutrino]]




# show my dashboard      [[qs]] [[social]]




# `[2020-09-01]` [Pandas API — hvPlot 0.6.0 documentation](https://hvplot.holoviz.org/user_guide/Pandas_API.html)

    Lag Plot
    Lag plots are used to check if a data set or time series is random. Random data should not exhibit any structure in the lag plot. Non-random structure implies that the underlying data are not random.




# mixing in data from taplog      [[weight]] [[exercise]] [[qs]]

Dump an org  table  
Preserve the ids  
Join with taplog (maybe even as a df)  
Win! Maybe check some similarity score too  
Same for weight?  




# on the hrv plot, diplay as arrow if the trend is up or down      [[sleep]]




# `[2020-11-03]` [joshlk/dataclassframe: A container for dataclasses with multi-indexing and bulk operations.](https://github.com/joshlk/dataclassframe)

hmm.. doesn't have any typing imports at all?? what do they mean 'working nicely with type hints', that they don't crash??  




## `[2021-02-06]` ah ok, something added.. maybe reevaluate it later




# use for daily dashboard or something?      [[remarkable]]




# `[2020-09-06]` [bokeh/notebook<sub>embed.ipynb</sub> at 2.2.1 · bokeh/bokeh](https://github.com/bokeh/bokeh/blob/2.2.1/examples/howto/server_embed/notebook_embed.ipynb)




# <https://github.com/thesephist/histools>       [[dashboard]] [[viz]]

    A collection of tools for generating data visualizations from browser history data

looks like a heatmap?  




# `[2020-12-30]`       [[bokeh]]

goddamnit. so frustrating that I can't zoom it properly  




# Grafana       [[timeline]]

eh, I'm not even super sure what I wanna plot&#x2026;  
I guess for beginners would be nice to have sleep plot, maybe estimated from rescuetime  
that could also href to timeline slices  
 plotly plugin  
 geomap plugin  
 <https://forum.quantifiedself.com/t/grafana-influxdb-and-apple-watch-metrics/5323>  
 apparently some people are using influxdb for that stuff? still not worth for me&#x2026;  
 <http://quantifiedself.com/2015/07/2015-qs-visualization-gallery-part-3/>  
 <https://github.com/Freeyourgadget/Gadgetbridge/issues/49>  




## uhh. so unclear how to connect my data to grafana.




## lastfm 

some issues: unable to hide zeros &#x2014;> LOTS of 0 points  
unable to attach labels?  
influx to start terminal client  
lastfm/fill<sub>influxdb.py</sub>  

<http://localhost:3000>  
influxdb on default port&#x2026; everything is admin/admin  




## I guess, start with weight for simplicity




## then, do sleep




# figure out grafana..




# post on dataisbeautiful?      [[reddit]] [[sleep]]




# fix dovpandas warnings




# when I release it, make sure it works both against public and private hpi bits      [[sleep]]




# profile stuff a bit?




# `[2020-12-05]` [xkcd: Linear Regression](https://xkcd.com/1725/)      [[toblog]]




# `[2019-04-15]` Python Data Visualization 2018: Why So Many Libraries? - Anaconda

<https://www.anaconda.com/python-data-visualization-2018-why-so-many-libraries/>  




## `[2019-09-10]` try using in dashboard




# `[2019-04-14]` iris<sub>splom.py</sub> — Bokeh 1.1.0 documentation

<https://bokeh.pydata.org/en/latest/docs/gallery/iris_splom.html>  




## `[2019-07-23]` eh, defaults don't look great. maybe it's faster but unclear




# `[2020-10-25]` [Tableau Desktop](https://www.tableau.com/en-gb/products/desktop)      [[viz]] [[qs]]




# -----&#x2013;&#x2014; last housekeeping on `[2021-02-06]` ----------




# can overlay activity data vs sleep data from different tools?      [[dashboard]] [[sleep]] [[hpi]]




# `[2021-02-12]` [grafana/worldmap-panel: Worldmap panel plugin for Grafana 3.0 that can be overlaid with circles for data points.](https://github.com/grafana/worldmap-panel)      [[location]] [[dashboard]]




# `[2021-02-18]` [Personal Dashboards for Self-Tracking Data - Quantified Self / Apps & Tools - Quantified Self Forum](https://forum.quantifiedself.com/t/personal-dashboards-for-self-tracking-data/8202/50?u=karlicoss)      [[hpi]] [[dashboard]] [[publish]]

some screenshots  




# could use mybinder for demos? same used by jupyterlab      [[dashboard]] [[hpi]]




# `[2021-04-11]` [LibrePhotos/librephotos: Self hosted alternative to Google Photos](https://github.com/LibrePhotos/librephotos)      [[photos]] [[memex]]




# `[2021-04-11]` [photoprism/photoprism: Personal Photo Management powered by Go and Google TensorFlow](https://github.com/photoprism/photoprism)      [[photos]] [[memex]]

looks good &#x2013; I guess need to evaluate on the basis of whether I can share it?  




# `[2021-03-05]` [Introducing Orion: A Powerful Substitute for OwnTracks Recorder - Blog - Kevin Lin](https://blog.kevinlin.info/post/introducing-orion-a-powerful-substitute-for-owntracks-recorder/)      [[location]] [[HPI]] [[dashboard]]

    orion-web provides a fast, interactive, React-based data visualization frontend for the web, powered by deck.gl

whoa ok, this is pretty awesome  




# `[2019-09-30]` Jupyter notebooks on steroids      [[dashboard]] [[ipynb]]

<https://www.slideshare.net/bultako/jupyter-notebooks-on-steroids>  




## `[2019-10-06]` try ipywidgets?




# `[2021-04-29]` [Personal Dashboards for Self-Tracking Data - Quantified Self / Apps & Tools - Quantified Self Forum](https://forum.quantifiedself.com/t/personal-dashboards-for-self-tracking-data/8202/55?u=karlicoss)      [[qs]]

    I pretty much 100% agree with your assessment. I personally would also add:
    
        Automatic backup of data.
        API for simple daily import of data (e.g. from manual or unsupported trackers). To me CSV import is inferior solution, especially for dashboard, where the point is to have the data visualized persistently.
        I would expand the ‘flexible data analysis’ to following specific analysis that I feel are essential (but I haven’t seen anywhere):
        a. cross-correlation across time to uncover temporally delayed relationships between tracked variables
        b. automatic application of the above to all pairs of variables with report of the strongest relationships found
        c. proper reporting of statistical significance of any correlations found
        d. multi-variate regression

motivaion: good points about what's missing from most current solutions  

