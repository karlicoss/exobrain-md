
# Table of Contents

-   [\* motivation](#mtvtn) 
    -   [why database](#whydtbs) 
    -   [nice feature is that it's easy to compare changes&#x2026; I can simply run sqldiff](#ncftrsthttssytcmprchngscnsmplyrnsqldff) 
    -   [Sqlalchemy orm requires using their adapters (check that). Also check if they support nested stuff](#sqllchmyrmrqrssngthrdptrshtlschckfthyspprtnstdstff) 
        -   [`[2019-07-25]` sqlalchemy core doesn't support binding? that dataset got their own ResultIter adapter](#sqllchmycrdsntspprtbndngthtdtstgtthrwnrslttrdptr) 
        -   [`[2019-07-25]` https://docs.sqlalchemy.org/en/13/core/custom\_types.html somewhat awkward and invasive for existing types](#sdcssqllchmyrgncrcstmtypswhtwkwrdndnvsvfrxstngtyps) 
        -   [`[2019-07-30]` performance: I haven't tested](#prfrmnchvnttstd) 
    -   [combines some of my favorite python features: type annotations, decorators, generators, context managers](#cmbnssmfmyfvrtpythnftrstytnsdcrtrsgnrtrscntxtmngrs) [[python]] [[toblog]]
    -   [`[2019-07-19]` Is it possible to use a namedtuple with SQLalchemy? : Python](#stpssbltsnmdtplwthsqllchmypythn) 
-   [\* prior art/similar projects](#prrrtsmlrprjcts) 
    -   [cattrs](#sgthbcmtnchcttrscttrs) 
        -   [`[2020-05-16]` ok, not sure if it supports NT/dataclasses? Hypothesis tests are nice though](#kntsrftspprtsntdtclssshypthsststsrncthgh) 
    -   [`[2020-05-16]` UnitedIncome/json-syntax: Generates functions to convert Python classes to and from JSON friendly objects](#sgthbcmntdncmjsnsyntxntdnclssstndfrmjsnfrndlybjcts) [[python]] [[json]]
    -   [`[2020-05-26]` freelancer/pavlova: A python deserialisation library built on top of dataclasses](#sgthbcmfrlncrpvlvfrlncrpvsrlstnlbrrybltntpfdtclsss) [[cache]]
        -   [`[2020-07-13]` register types in the same way? https://github.com/freelancer/pavlova#adding-custom-types](#rgstrtypsnthsmwysgthbcmfrlncrpvlvddngcstmtyps) 
    -   [`[2020-03-11]` unmade/apiwrappers: Build API clients that work both with regular and async code](#nmdpwrpprsbldpclntsthtwrkbthwthrglrndsynccd) [[axol]]
-   [\* potential features](#ptntlftrs) 
    -   [thinking about incremenal caching](#thnkngbtncrmnlcchng) 
    -   [preserve traceback?](#prsrvtrcbck) 
    -   [cache is gonna be expired several times a day anyway judging by bleansed backups&#x2026; so I kind of need to do incremental anyway](#cchsgnnbxprdsvrltmsdynywybckpsskndfndtdncrmntlnywy) [[hpi]] [[reddit]]
    -   [maybe instead of key equality, use key comparison? assume that if the key is bigger, in includes all the data for smaller keys](#mybnstdfkyqltyskycmprsnssggrnncldsllthdtfrsmllrkys) 
    -   [could cache as a Protocol.. and then reconstruct back a dataclass? odd but could work?](#cldcchsprtclndthnrcnstrctbckdtclssddbtcldwrk) 
    -   [not sure how to compute dependencies automatically?](#ntsrhwtcmptdpndncstmtclly) 
    -   [should be like Logger. global default + instances for more customization](#shldblklggrglbldfltnstncsfrmrcstmztn) 
    -   [keep data along with hash in the same table?](#kpdtlngwthhshnthsmtbl) 
    -   [create database, continuously updated by an iterable? could be useful for logs](#crtdtbscntnslypdtdbyntrblcldbsflfrlgs) 
    -   [for upgradeable storage &#x2013; I guess it should be a special function, first argument is an iterable that will be populated from the cache regardless. then it's up to the caller to determine what to process?](#frpgrdblstrggsstshldbspcltsptthcllrtdtrmnwhttprcss) [[promnesia]]
    -   [try using with classmethods? https://hynek.me/articles/decorators/#tldr](#trysngwthclssmthdsshynkmrtclsdcrtrstldr) 
    -   [for persisting, I guess it makes sense to use namedtuples, not just json, e.g. custom sql queries might actually use structure](#frprsstnggsstmkssnstsnmdtstmsqlqrsmghtctllysstrctr) 
    -   [Support anon tuples? As long as they are typed&#x2026;](#spprtnntplsslngsthyrtypd) 
        -   [`[2019-08-14]` tried to implement tuples support&#x2026; but it's just too freaking hacky&#x2026;](#trdtmplmnttplsspprtbttsjsttfrknghcky) 
    -   [`[2020-01-13]` Shit! If merging is implemented recursivelyz like Fibonacci, cachew could support properly incremental exports?](#shtfmrgngsmplmntdrcrsvlyzldspprtprprlyncrmntlxprts) 
    -   [use appdirs](#sppdrs) [[cachew]]
    -   [Hide tail call optimization in cachew?? Hmmm](#hdtlcllptmztnncchwhmmm) [[cachew]]
    -   [env variable to turn it off??](#nvvrblttrntff) [[cachew]]
    -   [make it depend on the git hash? I guess global override would be nice](#mktdpndnthgthshgssglblvrrdwldbnc) [[cachew]]
-   [\* publicity](#pblcty) [[publish]]
    -   [`[2020-04-09]` Pyfiddle](#pyfddl) [[demo]]
    -   [`[2020-01-09]` PyCoder’s Weekly on Twitter: "cachew: Persistent Cache/Serialization Powered by Type Hints https://t.co/x587YrhtLE" / Twitter](#pycdrswklyntwttrcchwprsstrdbytyphntsstcxyrhtltwttr) 
    -   [Link to hpi draft and exports draft](#lnkthpdrftndxprtsdrft) [[hpi]] [[exports]]
    -   [could post on HN and lobsters as well](#cldpstnhnndlbstrsswll) [[publish]]
    -   [Perhaps merging bluemaesro databases could be a good example?](#prhpsmrgngblmsrdtbsscldbgdxmpl) [[bluemaestro]]
    -   [could demonstrate this?](#clddmnstrtths) 
    -   [temperature during sleep analysis](#tmprtrdrngslpnlyss) 
    -   [Might be actually worth a separate post; using it in promnesia and axol as well](#mghtbctllywrthsprtpstsngtnprmnsndxlswll) [[cachew]] [[toblog]]
-   [\* readme/docs](#rdmdcs) 
    -   [`[2020-10-09]` karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](#sgthbcmkrlcsscchwkrlcsscctntcchsrlztnpwrdbytyphnts) 
    -   [`[2020-10-09]` karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](#sgthbcmkrlcsscchwkrlcsscctntcchsrlztnpwrdbytyphnts) 
    -   [`[2020-10-09]` karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](#sgthbcmkrlcsscchwkrlcsscctntcchsrlztnpwrdbytyphnts) 
    -   [add autocomplete docs?](#ddtcmpltdcs) [[literate]]
    -   [Come up with a decent example..](#cmpwthdcntxmpl) 
        -   [`[2020-01-08]` pdf annotations could be a really good one. MASSIVE difference](#pdfnnttnscldbrllygdnmssvdffrnc) 
    -   [Use ipynb for docs?](#spynbfrdcs) [[ipython]] [[literate]]
        -   [`[2019-08-18]` pretty nice actually!](#prttyncctlly) 
    -   [generate readme from unit tests?](#gnrtrdmfrmnttsts) [[literate]]
    -   [`[2020-11-14]` karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](#sgthbcmkrlcsscchwxmplskrltntcchsrlztnpwrdbytyphnts) 
    -   [example could be merging of highlights from different sources, e.g. kobo and kindle](#xmplcldbmrgngfhghlghtsfrmdffrntsrcsgkbndkndl) [[toblog]]
    -   [post example log?](#pstxmpllg) 
        -   [`[2019-07-30]` err, log of what?](#rrlgfwht) 
    -   [fuck, if I want people to use it, I'm gonna need some documentation&#x2026;](#fckfwntppltstmgnnndsmdcmnttn) 
-   [\* performance & profiling](#prfrmncprflng) [[performance]]
    -   [some old experiment on speeding up](#smldxprmntnspdngp) 
    -   [`[2019-07-25]` profiling](#prflng) 
        -   [`[2019-07-30]` I haven't bothered much with profiling and optimizing since for now the benefits of using this are clear](#hvntbthrdmchwthprflngndptsncfrnwthbnftsfsngthsrclr) 
    -   [some old comments](#smldcmmnts) 
-   [\* bugs/stability](#bgsstblty) 
    -   [rename 'table' to 'data'? to avoid quoting issues](#rnmtbltdttvdqtngsss) [[cachew]]
    -   [warn when it's running under tests? not sure](#wrnwhntsrnnngndrtstsntsr) 
    -   [hmm, on first initialisation in case of error it shouldn't initialise cache..](#hmmnfrstntlstnncsfrrrtshldntntlscch) [[promnesia]]
        -   [`[2021-03-20]` ok, it behaves correctly so not such bit issue&#x2026;](#ktbhvscrrctlysntschbtss) 
    -   [add a test for schema change](#ddtstfrschmchng) 
    -   [hmm, with overlays, <span class="underline"><span class="underline">module</span></span> gets a weird prefix..](#hmmwthvrlysmdlgtswrdprfx) [[hpi]]
    -   [seems that it may delete whole directories??](#smsthttmydltwhldrctrs) 
    -   [hmm&#x2026; can generate shitty names?](#hmmcngnrtshttynms) [[cachew]]
-   [I guess binder for namedtuples is kinda a separate thing as it could be used separately for 'pickling'](#gssbndrfrnmdtplsskndsprtthngstcldbsdsprtlyfrpcklng) 
-   [ok, thinking about default paths](#kthnkngbtdfltpths) 
-   [related](#rltd) [[python]] [[hpi]]
-   [`[2021-03-08]` calpaterson/pyappcache: A library for application-level caching](#sgthbcmclptrsnpyppcchclptpcchlbrryfrpplctnlvlcchng) [[cachew]]
-   [`[2019-10-01]` github commits integrate well with my. package. also could demonstrate cachew?](#gthbcmmtsntgrtwllwthmypckglsclddmnstrtcchw) 
-   [`[2019-10-01]` demonstrate cachew on pdfs?](#dmnstrtcchwnpdfs) [[hpi]] [[cachew]]

Cachew lets you cache function calls into an sqlite database on your disk in a matter of single decorator (similar to functools.lru<sub>cache</sub>).  
The difference from functools.lru<sub>cache</sub> is that cached data is persisted between program runs, so next time you call your function, it will only be a matter of reading from the cache.  
Cache is invalidated automatically if your function's arguments change, so you don't have to think about maintaining it.  

<https://github.com/karlicoss/cachew#what-is-cachew>  




# \* motivation





## why database

-   compact
-   fast
-   easy iteration
-   possible to use as data interface by querying the db directly

why using separate columns at all  

-   actually appart from potentially nicer queries I'm not sure. I wonder if more time is spent serializing as opposed to simply using json?




## nice feature is that it's easy to compare changes&#x2026; I can simply run sqldiff




## Sqlalchemy orm requires using their adapters (check that). Also check if they support nested stuff





### `[2019-07-25]` sqlalchemy core doesn't support binding? that dataset got their own ResultIter adapter




### `[2019-07-25]` <https://docs.sqlalchemy.org/en/13/core/custom_types.html> somewhat awkward and invasive for existing types




### `[2019-07-30]` performance: I haven't tested




## combines some of my favorite python features: type annotations, decorators, generators, context managers      [[python]] [[toblog]]




## `[2019-07-19]` Is it possible to use a namedtuple with SQLalchemy? : Python

<https://www.reddit.com/r/Python/comments/kz7vj/is_it_possible_to_use_a_namedtuple_with_sqlalchemy/>  

    sqlalchemy needs to attach attributes onto a mapped class, which include one for each column mapped, as well as an attribute _sa_instance_state for bookkeeping. It also, as someone mentioned, needs to create a weak reference to the object. So a SQLAlchemy-mapped class needs to be a "new style class", extending from object.
    If you look at how namedtuple works, it has quite a bit of trickery going on, not the least of which is that it sets __slots__ to (). Then there's some super-nasty frame mutation stuff after that to somehow make it pickleable.
    That said it's straightforward to make your own class that is SQLAlchemy compatible and acts more or less the same as a namedtuple. Just define __iter__, __len__, __repr__, other methods as appropriate. Plus it will be pickleable without injecting variables into stack frames.




# \* prior art/similar projects





## [cattrs](https://github.com/Tinche/cattrs) 

    When you're handed unstructured data (by your network, file system, database...), cattrs helps to convert this data into structured data.
    When you have to convert your structured data into data types other libraries can handle, cattrs turns your classes and enumerations into dictionaries, integers and strings.




### `[2020-05-16]` ok, not sure if it supports NT/dataclasses? Hypothesis tests are nice though




## `[2020-05-16]` [UnitedIncome/json-syntax: Generates functions to convert Python classes to and from JSON friendly objects](https://github.com/UnitedIncome/json-syntax)      [[python]] [[json]]




## `[2020-05-26]` [freelancer/pavlova: A python deserialisation library built on top of dataclasses](https://github.com/freelancer/pavlova)      [[cache]]





### `[2020-07-13]` register types in the same way? <https://github.com/freelancer/pavlova#adding-custom-types>




## `[2020-03-11]` unmade/apiwrappers: Build API clients that work both with regular and async code      [[axol]]

<https://github.com/unmade/apiwrappers>  

    Modern - decode JSON with no effort using dataclasses and type annotations

hmm kind of similar to what I'm doing/want for axol?  




# \* potential features





## thinking about incremenal caching

-   caching diffs  
    
    -   reasonable perf boost
    -   relatively easy? just ignore 'emitted'?
    -   automatically works for changed prefix (bleanser)
    
    ? requires changes to cachew key handling  
    
    -   might be still slowish

-   explicitly querying for cached prefix  
    -   best performance
    -   fairly easy
    -   almost no changes to cachew
    -   requires restructuting code in a specific way, mcachew thing might be harder
    -   gonna be tricky if the prefix can cahnge (bleanser) (although if we can probe for a cached key, it can work?)

-   single cachew decorator (not sure if possible?)  
    -   best performance
    -   pretty simple
    -   still requires 'hack' in the caller for detecting if something was cached or not
    -   if prefix changes won't work
    -   requires cachew changes? some sort of global function context? pretty unclear how to implement  
        -   with cached(f) as cf:  
            return cf(some<sub>args</sub>)
        -   ok, maybe by default cachew is 'recursive'?  
            when we enter the function, we memorize the argument that needs to be cached, but we don't lock the database yet?  
            so, let's consider  
             @cachew  
             def factorials(n: int) -> int:  
                 last = 1  
                 for prev in factorials(n - 1):  
            	 yield prev  
                 yield prev \* n  
            say, we've run factorials(3) before, the cache has [1, 2, 6]  
            factorials(5), cachew memorizes {factorials: 5}, it's the one being computed, goes inside the function  
                 factorials(4) &#x2013; not in the cache. so it goes inside and tries evaluating factorials(3)  
            	factorials(3) &#x2013; in the cache, cachew opens the db ans starts emitting?  
            	factorials(4) shouldn't be writing becase it's not the one being computed  
            	factorials(5) on the other hand should start writing  
            	  kind of a problem however is that it reads and writes at the same time.. I guess that could work with transactions?




## preserve traceback?




## cache is gonna be expired several times a day anyway judging by bleansed backups&#x2026; so I kind of need to do incremental anyway      [[hpi]] [[reddit]]




## maybe instead of key equality, use key comparison? assume that if the key is bigger, in includes all the data for smaller keys




## could cache as a Protocol.. and then reconstruct back a dataclass? odd but could work?




## not sure how to compute dependencies automatically?




## should be like Logger. global default + instances for more customization




## keep data along with hash in the same table?

feels a bit more atomic&#x2026;  




## create database, continuously updated by an iterable? could be useful for logs




## for upgradeable storage &#x2013; I guess it should be a special function, first argument is an iterable that will be populated from the cache regardless. then it's up to the caller to determine what to process?      [[promnesia]]




## try using with classmethods? <https://hynek.me/articles/decorators/#tldr>




## for persisting, I guess it makes sense to use namedtuples, not just json, e.g. custom sql queries might actually use structure




## Support anon tuples? As long as they are typed&#x2026;





### `[2019-08-14]` tried to implement tuples support&#x2026; but it's just too freaking hacky&#x2026;

    def test_typing_tuple(tmp_path):
        tdir = Path(tmp_path)
    
        @cachew(tdir / 'cache')
        def get_data() -> Iterator[Tuple[str, int]]:
            yield ('first' , 1)
            yield ('second', 2)
    
        assert list(get_data())[-1][0] == 'second'
        assert list(get_data())[-1][1] == 2




## `[2020-01-13]` Shit! If merging is implemented recursivelyz like Fibonacci, cachew could support properly incremental exports?




## use appdirs      [[cachew]]

-   maybe allow using app specific subcaches?  
    e.g. make<sub>cachew</sub>(prefix='my')
-   `[2021-03-20]` ok done <https://github.com/karlicoss/cachew/commit/161ce25304bfda77b484f886ff9c0b4b23924563>




## Hide tail call optimization in cachew?? Hmmm      [[cachew]]




## env variable to turn it off??      [[cachew]]




## make it depend on the git hash? I guess global override would be nice      [[cachew]]




# \* publicity      [[publish]]





## `[2020-04-09]` Pyfiddle      [[demo]]

<https://pyfiddle.io/fiddle/4de2f70f-e421-4326-bbb8-b06d5efa547d/?i=true>  
yeah really need to give a demo  




## `[2020-01-09]` PyCoder’s Weekly on Twitter: "cachew: Persistent Cache/Serialization Powered by Type Hints <https://t.co/x587YrhtLE>" / Twitter

<https://twitter.com/pycoders/status/1214956434519154688>  




## Link to hpi draft and exports draft      [[hpi]] [[exports]]




## could post on HN and lobsters as well      [[publish]]




## Perhaps merging bluemaesro databases could be a good example?      [[bluemaestro]]




## could demonstrate this?

perhaps with more processing difference would be even more striking&#x2026;  

    $ time with_my python3 -c 'from my.bluemaestro import get_dataframe; print(get_dataframe())'
    USING CACHEW!!!
                         temp
    dt
    2018-07-15 02:57:00  24.3
    2018-07-15 02:58:00  24.3
    2018-07-15 02:59:00  24.3
    2018-07-15 03:00:00  24.3
    2018-07-15 03:01:00  24.3
    ...                   ...
    2019-07-27 10:42:00  23.8
    2019-07-27 10:43:00  23.8
    2019-07-27 10:44:00  23.8
    2019-07-27 10:45:00  23.8
    2019-07-27 10:46:00  23.8
    
    [549054 rows x 1 columns]
    with_my python3 -c   3.32s user 0.36s system 111% cpu 3.296 total

    $ time with_my python3 -c 'from my.bluemaestro import get_dataframe; print(get_dataframe())'
                         temp
    dt
    2018-07-15 02:57:00  24.3
    2018-07-15 02:58:00  24.3
    2018-07-15 02:59:00  24.3
    2018-07-15 03:00:00  24.3
    2018-07-15 03:01:00  24.3
    ...                   ...
    2019-07-27 10:42:00  23.8
    2019-07-27 10:43:00  23.8
    2019-07-27 10:44:00  23.8
    2019-07-27 10:45:00  23.8
    2019-07-27 10:46:00  23.8
    
    [549054 rows x 1 columns]
    with_my python3 -c   16.03s user 0.37s system 102% cpu 16.019 total




## temperature during sleep analysis




## Might be actually worth a separate post; using it in promnesia and axol as well      [[cachew]] [[toblog]]




# \* readme/docs





## `[2020-10-09]` [karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](https://github.com/karlicoss/cachew)

    During reading cache all that happens is reading rows from sqlite and mapping them onto your target datatype, so the only overhead would be from reading sqlite, which is quite fast.

ugh, grammar is a bit odd  




## `[2020-10-09]` [karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](https://github.com/karlicoss/cachew)

    attemps to cause

to call  




## `[2020-10-09]` [karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](https://github.com/karlicoss/cachew)

    caching for

globally?  




## add autocomplete docs?      [[literate]]




## Come up with a decent example..

Maybe even dal is fine if I illustrate it by integration test?  




### `[2020-01-08]` pdf annotations could be a really good one. MASSIVE difference




## Use ipynb for docs?      [[ipython]] [[literate]]





### `[2019-08-18]` pretty nice actually!




## generate readme from unit tests?      [[literate]]




## `[2020-11-14]` [karlicoss/cachew: Transparent and persistent cache/serialization powered by type hints](https://github.com/karlicoss/cachew#examples)

add a super simple, trivial example. just with some dictionaries maybe?  




## example could be merging of highlights from different sources, e.g. kobo and kindle      [[toblog]]




## post example log?





### `[2019-07-30]` err, log of what?




## fuck, if I want people to use it, I'm gonna need some documentation&#x2026;




# \* performance & profiling      [[performance]]

generally it's fast enough or at least 'much faster', not that it's super high priority&#x2026;  




## some old experiment on speeding up

    from sqlalchemy.interfaces import PoolListener # type: ignore
    # TODO ugh. not much faster...
    class MyListener(PoolListener):
        def connect(self, dbapi_con, con_record):
            pass
            # eh. doesn't seem to help much..
            # dbapi_con.execute('PRAGMA journal_mode=MEMORY')
            # dbapi_con.execute('PRAGMA synchronous=OFF')
    # self.db = sqlalchemy.create_engine(f'sqlite:///{db_path}', listeners=[MyListener()])




## `[2019-07-25]` profiling

test<sub>dbcache</sub><sub>many</sub>  

de8b67cd0896e0b7512d276a5bb0fc9784ea9a49  

    100K: about  3.0 seconds
    500K: about 15.5 seconds
      1M: about 29.4 seconds

after updating to nice binders  

    100K: about  3.2 seconds
    500K: about 15.6 seconds
      1M: about 31.5 seconds




### `[2019-07-30]` I haven't bothered much with profiling and optimizing since for now the benefits of using this are clear




## some old comments

    logger.debug('inserting...')
    from sqlalchemy.sql import text # type: ignore
    from sqlalchemy.sql import text
    nulls = ', '.join("(NULL)" for _ in bound)
    st = text("""INSERT INTO 'table' VALUES """ + nulls)
    engine.execute(st)
    shit. so manual operation is quite a bit faster??
    but we still want serialization :(
    ok, inserting gives noticeable lag
    thiere must be some obvious way to speed this up...
    pylint: disable=no-value-for-parameter
    logger.debug('inserted...')




# \* bugs/stability

generally bugs not a big problem since the cache is temporary & optional, worst case can delete or disable  
although need to make sure there are not data consistency issues&#x2026; maybe expire cache on calendar?  




## rename 'table' to 'data'? to avoid quoting issues      [[cachew]]




## warn when it's running under tests? not sure




## hmm, on first initialisation in case of error it shouldn't initialise cache..      [[promnesia]]





### `[2021-03-20]` ok, it behaves correctly so not such bit issue&#x2026;




## add a test for schema change




## hmm, with overlays, <span class="underline"><span class="underline">module</span></span> gets a weird prefix..      [[hpi]]




## seems that it may delete whole directories??




## hmm&#x2026; can generate shitty names?      [[cachew]]

    ~/.cache/my/my.core.core_config:test_cachew.\<locals\>.cf




# I guess binder for namedtuples is kinda a separate thing as it could be used separately for 'pickling'




# ok, thinking about default paths

Ok, so in 99% of cases it's enough to use the default directory, this will make everything much easier.  

-   [ ] sometimes you'd want to share a cache between computers? Make sure it works over a symlink?

It's annoying to have cache settings in every data provider and in 99% the default is fine.  
So have a global HPI cache setting.  

-   [ ] unclear how to propagate the cache directory down to providers (e.g. reddit. ugh)

But would be nice to be able to customize the cache in advance.  
Maybe, set the attribute to the function? Seems good enough?  

-   [X] possibly need to create the parent dir automatically?
-   [ ] /var/tmp/cachew is better as the default? surfives through
-   [ ] if the path is relative, to it relatively to base dir, not cwd




# related       [[python]] [[hpi]]




# `[2021-03-08]` [calpaterson/pyappcache: A library for application-level caching](https://github.com/calpaterson/pyappcache)      [[cachew]]

    Pyappcache is a library to make it easier to use application-level caching in Python.
    
        Allows putting arbitrary Python objects into the cache
        Uses PEP484 type hints to help you typecheck cache return values
        Supports Memcache, Redis and SQLite




# `[2019-10-01]` github commits integrate well with my. package. also could demonstrate cachew?




# `[2019-10-01]` demonstrate cachew on pdfs?      [[hpi]] [[cachew]]

