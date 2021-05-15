
# Table of Contents

-   [related](#rltd) 
    -   [memex is the ultiplate knowledge management solution](#mmxsthltpltknwldgmngmntsltn) [[pkm]]
    -   [memex makes lifelogging data alive useful](#mmxmkslflggngdtlvsfl) [[lifelogging]]
    -   [memex can give you quantified self insights](#mmxcngvyqntfdslfnsghts) [[qs]]
-   [\* my current progress](#mycrrntprgrss) 
    -   [Human Programming Interface](#flprjctshprghmnprgrmmngntrfc) [[hpi]]
    -   [promnesia](#flprjctsprmnsrgprmns) [[promnesia]]
    -   [dashboard](#flprjctsdshbrdrgdshbrd) [[dashboard]]
    -   [orger](#flprjctsrgrrgrgr) [[orger]]
    -   [timeline](#flprjctstmlnrgtmln) [[timeline]]
-   [\* prior art & inspiration](#prrrtnsprtn) 
    -   [`[2020-03-07]` Memex by Andrew Louis + RubyConf 2018 talk](#shyfnntmmxmmxbyndrwlsswwwcmwtchvdfwxvqncfrbycnftlk) 
    -   [`[2020-05-25]` Memri: a very promising project with the focus on user data ownership and privacy](#smmrcldmmrvryprmsngprjctwththfcsnsrdtwnrshpndprvcy) 
    -   [`[2021-01-31]` NickSto/life-browser: View a timeline of your own history through your personal data.](#sgthbcmnckstlfbrwsrnckstlnfyrwnhstrythrghyrprsnldt) [[timeline]] [[memex]]
        -   [`[2021-04-27]` ok, interesting, but looks fairly basic, no UI yet and only contacts/location/hangouts/voice](#kntrstngbtlksfrlybscnytndnlycntctslctnhngtsvc) 
        -   [`[2020-05-11]` Thanks, I'll check it out! Yep, agree about the common codebase, that's why I'm&#x2026; | Hacker News](#snwsycmbntrcmtmdthnksllchthcmmncdbsthtswhymhckrnws) 
    -   [`[2021-03-15]` Heapy/Komodo-CRM: Life and collaboration assistant.](#sgthbcmhpykmdcrmhpykmdcrmlfndcllbrtnssstnt) [[memex]]
    -   [`[2021-01-21]` steve-1820/memex: A brief POC of what a Memex could potentially be.](#sgthbcmstvmmxstvmmxbrfpcfwhtmmxcldptntllyb) [[memex]]
-   [\* remembrance agents](#remembrance_agent) 
    -   [`[2020-01-06]` Remembrance Agent: A continuously running automated information retrieval system (1997)](#lmnmdmtdrhdspprsrmmbrnchtrnnngtmtdnfrmtnrtrvlsystm) 
    -   [`[2020-04-28]` A Desktop Remembrance Agent](#sgthbcmrmmbrncgntdsktprmmbrncgnt) 
-   [\* ideas & concepts](#dscncpts) 
    -   [`[2020-06-06]` hyfen.net/memex/updates/bad-remembrance-machines triplestore](#shyfnntmmxpdtsbdrmmbrncmcpdtsbdrmmbrncmchnstrplstr) [[lifelogging]]
    -   [`[2019-12-03]` Digital Tools I Wish Existed: A centralized search interface for my digital brain](#sjnbpstsdgtltlscntrlzdsrctrlzdsrchntrfcfrmydgtlbrn) [[jonbo]]
    -   [`[2020-05-10]` lehrjulian/status/1259526773236215814](#stwttrcmlhrjlnsttslhrjlnstts) [[timeline]]
    -   [maybe prolog for queries?](#mybprlgfrqrs) [[memex]] [[hpi]]
    -   [`[2020-01-08]` samsquire/ideas: life engine](#sgthbcmsmsqrdssmsqrdslfngn) 
    -   [`[2021-03-22]` What have you failed to build? | Lobsters](#slbstrssfgtzmwhthvyfldbldcttmfwhthvyfldtbldlbstrs) [[objectbrowser]]
-   [\* features & usecases](#ftrsscss) 
    -   [show random photos](#shwrndmphts) [[spacedrep]] [[lifelogging]]
    -   [`[2021-03-26]` Nextcloud - Wikipedia](#snwkpdrgwknxtcldnxtcldwkpd) [[location]] [[degoogle]] [[memex]]
-   [\* communities](#cmmnts) [[social]]
    -   [`[2020-05-28]` karlicoss/status/1266090022123470851](#stwttrcmkrlcsssttskrlcssstts) 
        -   [`[2021-01-04]` sadly haven't had time to set up something so far, also wouldn't want to overlap with existing ones](#sdlyhvnthdtmtstpsmthngsfrlswldntwnttvrlpwthxstngns) 
-   [`[2018-09-04]` tesseract is best apparently? but couldn't handle elliptical photos..](#tssrctsbstpprntlybtcldnthndlllptclphts) [[ocr]]
-   [`[2020-10-07]` eh, would be really nice to have some sort of memex at this point](#hwldbrllyncthvsmsrtfmmxtthspnt) [[promnesia]] [[memex]]
-   [ugh. it's still more convenient to use google location than any of my tools..](#ghtsstllmrcnvnnttsggllctnthnnyfmytls) [[dashboard]] [[grafana]] [[memex]] [[location]]
-   [`[2021-02-23]` Экзокортекс 3.5](#stndlrgxcrtxэкзокортекс) [[memex]]
-   [`[2021-02-23]` Экзокортекс: минимальная функциональность](#stndlrgxcrtxmnmlfnctnltyэнимальнаяфункциональность) [[memex]]
    -   [`[2021-03-14]` good summary and memex design requirements (in Russian)](#gdsmmryndmmxdsgnrqrmntsnrssn) 
-   [----------------------------](#11096_11168) 
-   [Tweet from @mekarpeles](#twtfrmmkrpls) [[memex]]
-   [`[2020-11-30]` appaquet/exocore: A distributed private application framework](#sgthbcmppqtxcrrdmpppqtxcrdstrbtdprvtpplctnfrmwrk) 
-   [`[2021-03-23]` Biograph](#swwwslpwbgrphbgrph) [[lifelogging]] [[inspiration]]
-   [`[2021-04-16]` SQLite the only database you will ever need in most cases | Lobsters](#slbstrsstshjqsqltnlydtbsydtbsywllvrndnmstcsslbstrs) [[location]] [[sqlite]]
-   [`[2020-08-28]` from email discussion](#frmmldscssn) 

Memex is a system that keeps all your data and acts as an ultimate interface to it.  
It gives you fast (ideally instant access), convenient interfaces and ultimately makes you better at thinking and analysing, acting as an auxiliary brain.  
Arguably so far none have been built :)  

I write more on why would you want it in [The sad state of personal data and infrastructure](https://beepb00p.xyz/sad-infra.html#why).  




# related 





## memex is the ultiplate knowledge management solution      [[pkm]]




## memex makes lifelogging data alive useful      [[lifelogging]]




## memex can give you quantified self insights      [[qs]]




# \* my current progress

My Memex so far isn't a single unified system, but has multiple facets and interfaces.  




## [Human Programming Interface](projects/hpi.md)      [[hpi]]

The backbone of my memex, providing data for other components.  




## [promnesia](projects/promnesia.md)       [[promnesia]]

Promnesia connects the web browser to the rest of your personal data.  




## [dashboard](projects/dashboard.md)       [[dashboard]]

My quantified self component to Memex.  




## [orger](projects/orger.md)       [[orger]]

Reflects my data for easier search, providing a plaintext interface.  




## [timeline](projects/timeline.md)       [[timeline]]




# \* prior art & inspiration





## `[2020-03-07]` [Memex](https://hyfen.net/memex) by Andrew Louis + [RubyConf 2018 talk](https://www.youtube.com/watch?v=DFWxvQn4cf8)

whoa, this is awesome  
he mentions the same problems I struggled with literally in the same words!  




## `[2020-05-25]` [Memri](https://memri.cloud): a very promising project with the focus on user data ownership and privacy




## `[2021-01-31]` [NickSto/life-browser: View a timeline of your own history through your personal data.](https://github.com/NickSto/life-browser)      [[timeline]] [[memex]]

    This is a project I began to try to collate all the digital breadcrumbs of my life and show them in an easily viewable timeline.




### `[2021-04-27]` ok, interesting, but looks fairly basic, no UI yet and only contacts/location/hangouts/voice




### `[2020-05-11]` [Thanks, I'll check it out! Yep, agree about the common codebase, that's why I'm&#x2026; | Hacker News](https://news.ycombinator.com/item?id=23131402)

    Hmm it's interesting how diverse the data sources people are actually using, but there's definitely overlap.




## `[2021-03-15]` [Heapy/Komodo-CRM: Life and collaboration assistant.](https://github.com/Heapy/Komodo-CRM)      [[memex]]

ran into it from  
<https://github.com/Heapy/Komodo-CRM/issues/72>  




## `[2021-01-21]` [steve-1820/memex: A brief POC of what a Memex could potentially be.](https://github.com/steve-1820/memex)      [[memex]]

ok, so it's more of a prototype at this point? and they are reinventing editor/annotation&#x2026; not sure  




# \* remembrance agents

    Remembrance Agents are a set of applications that watch over a user’s shoulder and suggest information relevant to the current situation




## `[2020-01-06]` [Remembrance Agent: A continuously running automated information retrieval system (1997)](http://alumni.media.mit.edu/~rhodes/Papers/remembrance.html)

This looks cool, but doesn't seem to work anymore?  

-   `[2019-12-28]` [The Remembrance Agent | Hacker News](https://news.ycombinator.com/item?id=4246330)




## `[2020-04-28]` [A Desktop Remembrance Agent](https://github.com/remembrance-agent)

    As you type, every five seconds the prior 60 characters of your keyboard buffer are sent to the RA. Suggestions are presented as clickable buttons

Ok, this looks pretty cool.. maybe need to contact them and discuss  




# \* ideas & concepts





## `[2020-06-06]` [hyfen.net/memex/updates/bad-remembrance-machines](https://hyfen.net/memex/updates/bad-remembrance-machines) triplestore      [[lifelogging]]

    This maps pretty well to the triplestore architecture that stores triples of subject-predicate-object




## `[2019-12-03]` [Digital Tools I Wish Existed: A centralized search interface for my digital brain](https://jon.bo/posts/digital-tools/#a-centralized-search-interface-for-my-digital-brain-memex)      [[jonbo]]

    This tool should: accept and parse the following queries:
     spacex announcement type:video 2016
     links from:jon@test.org topic:python
     paper on temperature, productivity referenced in book:Uninhabitable Earth
     type:pdf habits digital interfaces
     reading comprehension type:blog post
     printer ink receipt
     type:book read:2017 finance
     file:py datetime parse




## `[2020-05-10]` [lehrjulian/status/1259526773236215814](https://twitter.com/lehrjulian/status/1259526773236215814)      [[timeline]]

    I like the idea of converting a calendar into a diary / life log by integrating different data layers.
    Other layers I'd like to add:
    • Locations (Google Maps, Swarm)
    • Media consumption (books, Netflix)
    • Browser history / Screentime
    • Stress levels (Oura, Apple Watch)
    
    @aaronzlewis : concept: a Spotify calendar integration that lets you see what you were listening to alongside your old meetings and events. revisit the vibe of any moment with the Musical Time Machine




## maybe prolog for queries?      [[memex]] [[hpi]]




## `[2020-01-08]` [samsquire/ideas: life engine](https://github.com/samsquire/ideas)

    Life engine is a dashboard that attempts to collect information about your life and display relevant data on a single screen.




## `[2021-03-22]` [What have you failed to build? | Lobsters](https://lobste.rs/s/fgt5zm/what_have_you_failed_build#c_ott0mf)      [[objectbrowser]]

    I’ve been dreaming of making a “semantic history” browser add-on for ages, but never started.
    (As in something that would collect all the RDFa/microdata/microformats/JSON-LD/… objects on web pages you’ve seen, and give you an interface to browse not just pages, but these various objects like Organization, Person, Article, etc.    )




# \* features & usecases





## show random photos      [[spacedrep]] [[lifelogging]]




## `[2021-03-26]` [Nextcloud - Wikipedia](https://en.wikipedia.org/wiki/Nextcloud)      [[location]] [[degoogle]] [[memex]]

    Viewer for Maps

hmm, wonder if it could replace gmaps?  




# \* communities      [[social]]

This is something we can't build alone. Let's find each other and cooperate.  




## `[2020-05-28]` [karlicoss/status/1266090022123470851](https://twitter.com/karlicoss/status/1266090022123470851)

    I think I want to create some sort of community chat on the topic of knowledge management and tools around it, with the emphasis on interoperability, malleability, owning your data, local-first, org-mode etc.

-   `[2020-06-18]` I think I want the focus on existing tools and setup rather than discussing mockups and vague concepts. both are important, but I want to build something now
-   `[2020-06-18]` I want it to be a space to discuss configuration, and get detailed technical help etc. So needs to be more like an IM chat, with fine grained topics (so you can steer off a discussion without spamming everyone)




### `[2021-01-04]` sadly haven't had time to set up something so far, also wouldn't want to overlap with existing ones

Some existing communities:  

-   [Malleable Systems Collective](https://malleable.systems) + Matrix chat
-   <https://thinkingtools.space>
-   [The Productivitst Discord](https://disboard.org/server/join/727903265437777944)
-   [dendron Discord](https://discord.gg/AE3NRw9)
-   [logseq Discord](https://discord.gg/KpN4eHY)




# `[2018-09-04]` tesseract is best apparently? but couldn't handle elliptical photos..      [[ocr]]




# `[2020-10-07]` eh, would be really nice to have some sort of memex at this point      [[promnesia]] [[memex]]

maybe it could have some basic core (e.g. with couchdb), and then used in different apps?  
e.g. promnesia uses it to jump and browse the history  
dashboard uses to display all events  
timeline &#x2013; similarly for all life events  




# ugh. it's still more convenient to use google location than any of my tools..      [[dashboard]] [[grafana]] [[memex]] [[location]]

-   `[2021-02-22]` to be fair I didn't really do much on it yet




# `[2021-02-23]` [Экзокортекс 3.5](https://tiendil.org/exocortex-3-5/)      [[memex]]




# `[2021-02-23]` [Экзокортекс: минимальная функциональность](https://tiendil.org/exocortex-minimal-functionality/)      [[memex]]





## `[2021-03-14]` good summary and memex design requirements (in Russian)




# ---------------------------- 




# Tweet from @mekarpeles      [[memex]]

<https://twitter.com/mekarpeles/status/1271226785439428608>  

    @mekarpeles: Finally made a short 📽️ of https://t.co/glrT8wpAk2: Free + open source v. of @wikidata meets @RoamResearch (both which I 👍)




# `[2020-11-30]` [appaquet/exocore: A distributed private application framework](https://github.com/appaquet/exocore#roadmap)

    Exocore is a distributed applications framework with private and encrypted data storage. Think of like an infrastructure that allows a user to own his own personal cloud that is extensible via WebAssembly applications and accessible via Web/Mobile SDKs. It is designed to be resilient to failures, allow offline usage (ex: on mobile).




# `[2021-03-23]` [Biograph](https://www.saul.pw/biograph/)      [[lifelogging]] [[inspiration]]

nice 2d representation  




# `[2021-04-16]` [SQLite the only database you will ever need in most cases | Lobsters](https://lobste.rs/s/tsh0jq/sqlite_only_database_you_will_ever_need)      [[location]] [[sqlite]]

    I used to use SQLite all the time for geospatial data using the SpatiaLite extensions, it made dealing with data in many different formats much easier (and scriptable) and just simplified a lot of the work we had to do to manage weird datasets on nationalmap.gov.au(/renewables - sadly recently made defunct due to lack of government funding).
    We’d pretty regularly get CSVs with columns for LAT and LON, and need to do some actual work with the data, or turn it into another format like GeoJSON. Or we’d get a bunch of GeoJSON data that we wanted to manipulate.




# `[2020-08-28]` from email discussion

    Having stale data from manual exports is still useful, but adds a lot of mental friction ("is the export up-to-date enough to actually have what I need?").
    Very good point! Just thought, perhaps some meta information about the 'recency' of the data could be included in the interface, that might remove some of the friction.

