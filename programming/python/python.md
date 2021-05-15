
# Table of Contents

-   [\* testing](#tstng) [[testing]]
    -   [`[2020-03-27]` Hypothesis has a set of Pandas strategies for generating data](#hypthsshsstfpndsstrtgsfrgnrtngdt) [[pandas]]
    -   [`[2020-05-05]` python - Run code before and after each test in py.test? - Stack Overflow](#sstckvrflwcmqstnsrncdbfrnndftrchtstnpytststckvrflw) 
    -   [`[2019-08-02]` python - How should I structure a pytest test only package? - Stack Overflow](#pythnhwshldstrctrpytsttstnlypckgstckvrflw) [[testing]] [[project]] [[pip]]
    -   [doctest?](#dctst) 
    -   [pytest can detect recursion](#pytstcndtctrcrsn) [[pytest]]
-   [\* profiling](#prflng) [[performance]]
    -   [`[2020-03-08]` what-studio/profiling: An interactive continuous Python profiler](#whtstdprflngnntrctvcntnspythnprflr) 
        -   [`[2020-07-28]` kinda unmaintainerd though?](#kndnmntnrdthgh) 
    -   [`[2019-07-20]` profiling with cprof](#prflngwthcprf) 
    -   [`[2020-01-13]` rkern/line<sub>profiler</sub>: Line-by-line profiling for Python](#rkrnlnprflrlnbylnprflngfrpythn) 
    -   [`[2018-03-10]` profiling](#prflng) 
    -   [ipython?](#pythn) 
    -   [timeit](#tmt) 
-   [\* packaging](#pckgng) [[pip]]
    -   [`[2020-04-02]` minimal-setup-py/setup.py at master · maet3608/minimal-setup-py](#mnmlstppystppytmstrmtmnmlstppy) 
    -   [install only dependencies: `pip3 install --user -e .`](#nstllnlydpndncsppnstllsr) 
    -   [install multiple packages at once](#nstllmltplpckgstnc) 
    -   [`[2020-04-24]` local PIP dependency: if the repo is in `/path/to/repo`, put `HPI@git+file://DUMMY/path/to/repo@master` in `setup.py`](#lclppdpndncyfthrpsnpthtrppgtfldmmypthtrpmstrnstppy) [[pip]]
    -   [`[2019-12-15]` bast/pypi-howto: How to publish Python packages on PyPI.](#bstpyphwthwtpblshpythnpckgsnpyp) [[pypi]]
    -   [`[2019-07-02]` Testing & Packaging · Homepage of Hynek Schlawack](#tstngpckgnghmpgfhynkschlwck) 
        -   [`[2019-07-25]` o](#4147_4438) 
    -   [releasing on pypi](#rlsngnpyp) [[pypi]]
-   [\* debugging](#dbggng) [[debug]]
    -   [`[2019-04-09]` `with ipdb.launch_ipdb_on_exception()`](#wthpdblnchpdbnxcptn) [[habit]]
    -   [`[2019-12-05]` python3.7 has a `breakpoint()` builtin + more https://hackernoon.com/python-3-7s-new-builtin-breakpoint-a-quick-tour-4f1aebc444c](#pythnhsbrkpntbltnmrshckrnthnsnwbltnbrkpntqcktrfbcc) 
    -   [`ipdb pp` for pretty print](#pdbppfrprttyprnt) [[habit]]
-   [\* bad things about python](#bdthngsbtpythn) 
-   [\* static analysers](#sttcnlysrs) 
    -   [monkeytype &#x2013; automatic typing annotations generation](#mnkytyptmtctypngnnttnsgnrtn) [[mypy]]
    -   [would be nice to have  static analysis that checks you are not using global variables, etc.](#wldbncthvsttcnlyssthtchcksyrntsngglblvrblstc) 
    -   [bandit  &#x2013; security checks](#bndtscrtychcks) [[security]]
        -   [`[2021-01-16]` wouldn't say it's super useful&#x2026; might detect occasional eval or whatever, but won't help with more sophisticated stuff](#wldntsytssprsflmghtdtctccbtwnthlpwthmrsphstctdstff) 
-   [\* libraries](#lbrrs) 
    -   [`[2019-04-02]` peopledoc/workalendar: Worldwide holidays and workdays computational toolkit.](#ppldcwrklndrwrldwdhldysndwrkdyscmpttnltlkt) 
    -   [`[2018-12-09]` Altair: Declarative Visualization in Python — Altair 2.3.0 documentation](#ltrdclrtvvslztnnpythnltrdcmnttn) [[viz]]
-   [\* Import system](#mprtsystm) 
    -   [figure it out &#x2013; very confusing!](#fgrttvrycnfsng) 
    -   [`[2017-12-17]` from . import module](#frmmprtmdl) 
    -   [`[2020-01-17]` Alone Djangonaut – How python's import machinery works](#lndjngnthwpythnsmprtmchnrywrks) 
    -   [`[2019-06-29]` python - Relative imports for the billionth time - Stack Overflow](#pythnrltvmprtsfrthbllnthtmstckvrflw) 
    -   [`[2019-06-11]` relative imports are discouraged](#rltvmprtsrdscrgd) 
-   [\* datetime handling](#dttmhndlng) [[datetime]]
    -   [`[2018-09-04]` utcfromtimestamp &#x2013; returns timestamp, unaware; fromtimestamp &#x2013; returns offset + timestamp, unaware](#tcfrmtmstmprtrnstmstmpnwrmtmstmprtrnsffsttmstmpnwr) 
    -   [`[2018-09-04]` ok, seems that it's better to use `pytz.utc.localize(tz_unaware_datetime)`](#ksmsthttsbttrtspytztclclztznwrdttm) 
    -   [`[2020-05-02]` zachwill/moment: Dealing with dates in Python shouldn't have to suck.](#sgthbcmzchwllmmntzchwllmmgwthdtsnpythnshldnthvtsck) 
    -   [`[2020-05-02]` zachwill/moment: Dealing with dates in Python shouldn't have to suck.](#sgthbcmzchwllmmntzchwllmmgwthdtsnpythnshldnthvtsck) 
-   [\* logging](#lggng) [[logging]]
    -   [`[2018-07-05]` creating top level logger is always bad (may happen before configuring). use factory method](#crtngtplvllggrslwysbdmyhppnbfrcnfgrngsfctrymthd) [[logging]]
-   [\* docs](#dcs) 
    -   [pydoc](#pydc) 
    -   [ipython: ? and ??](#pythnnd) 
-   [\* ipdb](#pdb) [[ipdb]]
    -   [`[2019-04-09]` python - Use IPython magic functions in ipdb shell - Stack Overflow](#pythnspythnmgcfnctnsnpdbshllstckvrflw) 
-   [----------------------------------](#10407_10485) 
-   [`[2019-09-22]` Python3 f-strings - A complete guide to the most well received feature of Python 3. /r/Python](#srddtcmrpythncmmntsdzfhcpmstwllrcvdftrfpythnrpythn) 
-   [`[2019-05-11]` To yield or not to yield](#tyldrnttyld) [[yield]]
    -   [`[2019-07-30]` good point about separating validation and generation](#gdpntbtsprtngvldtnndgnrtn) 
-   [AST `ast.dump(ast.parse("'a' in 'aa' in 'aaa'"))`](#ststdmpstprsnn) 
-   [use for &#x2013; else](#sfrls) [[habit]]
-   [`[2018-06-18]` log optimizers i used](#lgptmzrssd) 
-   [`[2018-06-11]` optimizing python CLI tools https://files.bemusement.org/talks/OSDC2008-FastPython/](#ptmzngpythncltlssflsbmsmntrgtlkssdcfstpythn) 
-   [parser.add<sub>argument</sub>('rest, nargs=argparse.REMAINDER)](#prsrddrgmntrstnrgsrgprsrmndr) [[habit]]
-   [awesome-python https://github.com/vinta/awesome-python](#wsmpythnsgthbcmvntwsmpythn) 
    -   [should definitely subscribe to its feed and go through again](#shlddfntlysbscrbttsfdndgthrghgn) 
    -   [https://github.com/vinta/awesome-python#command-line-tools](#sgthbcmvntwsmpythncmmndlntls) 
    -   [pretty cool https://github.com/timofurrer/try](#prttyclsgthbcmtmfrrrtry) 
    -   [cool https://github.com/dbcli/mycli](#clsgthbcmdbclmycl) 
    -   [hmm try that? http://docopt.org/](#hmmtrythtdcptrg) 
    -   [some of these for nutrino? https://github.com/vinta/awesome-python#database](#smfthsfrntrnsgthbcmvntwsmpythndtbs) 
    -   [hmm that's interesting, visual scraping https://github.com/scrapinghub/portia](#hmmthtsntrstngvslscrpngsgthbcmscrpnghbprt) 
    -   [https://www.reddit.com/r/coolgithubprojects/](#swwwrddtcmrclgthbprjcts) 
    -   [?? https://python.libhunt.com/](#spythnlbhntcm) 
-   [do not use replace tzinfo, always localize..](#dntsrplctznflwyslclz) [[habit]]
-   [`[2019-01-01]` multiline string &#x2013; lstrip('\n') for nicer formatting!](#mltlnstrnglstrpnfrncrfrmttng) 
-   [`[2019-03-20]` Tweet from Vladislav Isenbaev (@isenbaev), at Mar 20, 03:48: pickle просто скотски медленный, если что - кратно медленнее даже json'а](#twtfrmvldslvsnbvsnbvtmrpcтократномедленнеедажеjsnа) 
-   [`[2019-08-11]` multiprocessing vs multithreading vs asyncio in Python 3.4 - Stack Overflow](#mltprcssngvsmltthrdngvssyncnpythnstckvrflw) [[concurrency]] [[performance]]
-   [`[2020-01-03]` adamchainz/patchy: Patch the inner source of python functions at runtime.](#dmchnzptchyptchthnnrsrcfpythnfnctnstrntm) [[lisp]]
-   [`[2019-12-31]` PyPy.js: Python in the web browser | Hacker News](#pypyjspythnnthwbbrwsrhckrnws) [[js]] [[webext]]
-   [`[2018-06-22]` `difflib.unified_diff` is suuuuper slow&#x2026;](#dfflbnfddffssprslw) 
-   [`[2018-04-21]` scrapy debugging](#scrpydbggng) [[scrapy]]
-   [`[2018-08-30]` python's for..else makes in 'syntactially' look like a total function](#pythnsfrlsmksnsyntctllylklkttlfnctn) 
-   [NamedTuple](#nmdtpl) 
    -   [use `typing.NamedTuple`](#stypngnmdtpl) 
    -   [watch out for default <span class="underline"><span class="underline">add</span></span> and <span class="underline"><span class="underline">mul</span></span>, it acts as adding pairs](#wtchtfrdfltddndmltctssddngprs) 
    -   [you can't easily overload <span class="underline"><span class="underline">init</span></span>, so make types of fields robust. Use a helper method instead](#ycntslyvrldntsmktypsffldsrbstshlprmthdnstd) 
-   [Use contextmanager](#scntxtmngr) 
-   [`[2018-12-08]` get current function/method name](#gtcrrntfnctnmthdnm) 
-   [traitlets?](#trtlts) 
-   [`[2019-04-30]` What's the difference between marshmallow and sql-alchemy? /r/flask](#srddtcmrflskcmmntsrtwhtstwnmrshmllwndsqllchmyrflsk) 
-   [`[2019-06-29]` dominatepp/.travis.yml at master · karlicoss/dominatepp](#dmntpptrvsymltmstrkrlcssdmntpp) [[ci]]
-   [`[2019-08-12]` use `re.VERBOSE` for inline comments in regexes](#srvrbsfrnlncmmntsnrgxs) 
-   [`[2019-10-21]` python - What do (lambda) function closures capture? - Stack Overflow](#pythnwhtdlmbdfnctnclsrscptrstckvrflw) [[plt]]
-   [`[2019-12-30]` argparse — Parser for command-line options, arguments and sub-commands — Python 3.8.1 documentation](#rgprsprsrfrcmmndlnptnsrgmntsndsbcmmndspythndcmnttn) 
-   [`[2020-01-07]` Performance — python-rapidjson 0.4 documentation](#prfrmncpythnrpdjsndcmnttn) [[json]]
-   [`[2019-07-19]` python - Argparse: Way to include default values in '&#x2013;help'? - Stack Overflow](#pythnrgprswytnclddfltvlsnhlpstckvrflw) 
-   [`[2019-12-31]` PyPy - packages http://packages.pypy.org](#pypypckgspckgspypyrg) [[pypy]]
-   [Construct: kinda like struct but better? https://construct.readthedocs.io/en/latest/](#cnstrctkndlkstrctbtbttrscnstrctrdthdcsnltst) [[parsing]]
-   [Pyrser: grammars? https://pythonhosted.org/pyrser/](#pyrsrgrmmrsspythnhstdrgpyrsr) [[parsing]]
-   [`[2019-07-21]` kython@git+https://github.com/karlicoss/kython.git@master dependency for setup.cfg](#kythngtsgthbcmkrlcsskythngtmstrdpndncyfrstpcfg) [[pip]]
-   [`[2018-07-22]` PyCon 2018 Talk Videos : Python https://www.reddit.com/r/Python/comments/8j4ep6/pycon\_2018\_talk\_videos/](#pycntlkvdspythnswwwrddtcmrpythncmmntsjppycntlkvds) [[towatch]]
-   [`[2019-08-02]` Basic usage — tox 3.13.3.dev13 documentation](#bscsgtxdvdcmnttn) 
-   [`[2018-06-12]` if there is a 'main.py' in script dir, it gets imported &#x2013; wtf????](#fthrsmnpynscrptdrtgtsmprtdwtf) 
-   [`[2019-07-20]` concurrent.futures https://docs.python.org/3.7/library/concurrent.futures.html?highlight=processpoolexecutor use `map`](#cncrrntftrssdcspythnrglbrhtmlhghlghtprcssplxctrsmp) 
-   [`[2019-08-11]` PyCQA/pyflakes: A simple program which checks Python source files for errors](#pycqpyflkssmplprgrmwhchchckspythnsrcflsfrrrrs) 
-   [`[2019-08-02]` posargs are needed to passing adhoc args, e.g.](#psrgsrnddtpssngdhcrgsg) [[tox]]
-   [`[2018-04-17]` some misc notes](#smmscnts) 
-   [`from http import HTTPStatus`](#frmmprtstts) 
-   [`[2018-01-21]` use nonlocal instead of global](#snnlclnstdfglbl) [[habit]]
-   [!r formatter](#rfrmttr) [[habit]]
-   [`[2019-04-22]` yield is often preferrable because python doesn't have bindings in generators](#yldsftnprfrrblbcspythndsnthvbndngsngnrtrs) 
-   [`[2019-05-01]` there is a difference between returning generator and yield from generator. the latter keeps scope, which might be useful if you have open files](#thrsdffrncbtwnrtrnnggnrtrsscpwhchmghtbsflfyhvpnfls) 
-   [`[2019-07-30]` To yield or not to yield](#tyldrnttyld) [[decorator]]
    -   [`[2019-07-30]` huh, some things are mentioned in the original post actually](#hhsmthngsrmntndnthrgnlpstctlly) 
-   [use putup (pyscaffold) for project generation](#sptppyscffldfrprjctgnrtn) [[habit]]
-   [Poetry instead of pyscaffold?](#ptrynstdfpyscffld) [[python]]
    -   [`[2021-01-16]` eh, don't think it worked for me, I prefer to rely on setup.py](#hdntthnktwrkdfrmprfrtrlynstppy) 
-   [`[2019-08-25]` https://docs.python.org/3.7/library/argparse.html argparse: use `set_defaults`](#sdcspythnrglbrryrgprshtmlrgprssstdflts) 
    -   [`[2019-09-02]` ah, could pass lambda to forward to actual handler function!](#hcldpsslmbdtfrwrdtctlhndlrfnctn) 
-   [generate<sub>ordering</sub>?](#gnrtrdrng) [[python]]
-   [`[2020-07-05]` How can I color Python logging output? - Stack Overflow](#sstckvrflwcmqstnshwcnclrpclrpythnlggngtptstckvrflw) [[logging]] [[kython]]
-   [`[2020-02-16]` Direct URL PEP 508 support and installing sub-dependencies from Git · Issue 5566 · pypa/pip](#drctrlppspprtndnstllngsbdpndncsfrmgtsspyppp) [[pip]]
-   [`[2020-02-16]` Allow direct urls in install<sub>requires</sub> · Issue 6301 · pypa/pip](#llwdrctrlsnnstllrqrssspyppp) [[python]]
-   [`[2019-07-25]` rstojnic/lazydata: Lazydata: Scalable data dependencies for Python projects](#rstjnclzydtlzydtsclbldtdpndncsfrpythnprjcts) 
    -   [`[2020-03-27]` so it kinda keeps textual 'submodules' for data??](#stkndkpstxtlsbmdlsfrdt) 
-   [using pytest fixtures to inject stuff into the module](#sngpytstfxtrstnjctstffntthmdl) [[python]] [[pytest]]
    -   [`[2019-08-02]` like in tz provider](#lkntzprvdr) 
-   [end2end gui semi manual tests](#ndndgsmmnltsts) [[promnesia]] [[python]] [[testing]]
-   [pytest dependencies](#pytstdpndncs) [[python]]
-   [`[2019-12-31]` backoff · PyPI](#bckffpyp) 
-   [Poetry for dep management](#ptryfrdpmngmnt) [[python]]
-   [`[2019-12-15]` Support automatic versioning setuptools<sub>scm</sub>-style? · Issue 140 · python-poetry/poetry](#spprttmtcvrsnngstptlsscmstylsspythnptryptry) 
-   [it's clearly not detecting changes in `install_requires`; needed to reinsall](#tsclrlyntdtctngchngsnnstllrqrsnddtrnsll) [[tox]]
-   [`[2019-07-26]` python - pytest exits with no error but with "collected 0 items" - Stack Overflow](#pythnpytstxtswthnrrrbtwthcllctdtmsstckvrflw) [[pytest]]
-   [`[2019-10-26]` traceback — Print or retrieve a stack traceback — Python 3.8.0 documentation](#trcbckprntrrtrvstcktrcbckpythndcmnttn) [[errors]]
-   [separate testing and linting since mypy's deps might be installed by accident?](#sprttstngndlntngsncmypysdpsmghtbnstlldbyccdnt) [[python]] [[tox]]
-   [`[2019-11-09]` python - Run an OLS regression with Pandas Data Frame - Stack Overflow](#pythnrnnlsrgrssnwthpndsdtfrmstckvrflw) 
-   [figure out a better framework for python multiprocessing&#x2026;](#fgrtbttrfrmwrkfrpythnmltprcssng) [[python]]
-   [`[2019-09-01]` vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources](#vntwsmpythncrtdlstfwsmpytnfrmwrkslbrrssftwrndrsrcs) [[tui]]
-   [sigh&#x2026; don't think it's possible to properly preserve stacktraces&#x2026;](#sghdntthnktspssbltprprlyprsrvstcktrcs) [[python]] [[errors]]
-   [strptime is incapable of handling timezones via %Z direcive??](#strptmsncpblfhndlngtmznsvzdrcv) [[python]] [[timezone]]
    -   [`[2020-03-27]` see takeout provider](#stktprvdr) 
-   [`[2020-03-12]` encode/httpx: A next generation HTTP client for Python. 🦋](#ncdxnxtgnrtnclntfrpythn) 
-   [`[2020-09-02]` Python Prompt Toolkit 3.0 — prompt<sub>toolkit</sub> 3.0.2 documentation](#spythnprmpttlktrdthdcsnmsprmpttlktprmpttlktdcmnttn) [[tui]] [[python]]
-   [`[2020-09-18]` testing - Python/tox Install a dependency as editable - Stack Overflow](#sstckvrflwcmqstnspythntxnstlldpndncysdtblstckvrflw) [[python]] [[tox]] [[pip]]
-   [`[2020-09-18]` testing - Python/tox Install a dependency as editable - Stack Overflow](#sstckvrflwcmqstnspythntxnstlldpndncysdtblstckvrflw) [[hpi]]
-   [`[2020-09-27]` python - What is the difference between venv, pyvenv, pyenv, virtualenv, virtualenvwrapper, pipenv, etc? - Stack Overflow](#sstckvrflwcmqstnswhtsthdfrtlnvwrpprppnvtcstckvrflw) 
-   [adapter thigs with getattr (like in workout provider for org notes) &#x2013; pretty great for adding one missing method](#dptrthgswthgtttrlknwrktprsprttygrtfrddngnmssngmthd) [[python]]
-   [`[2019-08-25]` argparseweb · PyPI](#rgprswbpyp) 
-   [`[2019-09-01]` vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources](#vntwsmpythncrtdlstfwsmpytnfrmwrkslbrrssftwrndrsrcs) [[cli]]
-   [`[2019-08-02]` GrahamDumpleton/wrapt: A Python module for decorators, wrappers and monkey patching.](#grhmdmpltnwrptpythnmdlfrdcrtrswrpprsndmnkyptchng) 
-   [attemt to figure out mixed sem/cal versioning](#ttmttfgrtmxdsmclvrsnng) [[project]] [[pip]]
-   [had to remore username from hatch config? it was overriding <span class="underline"><span class="underline">token</span></span> during the release..](#hdtrmrsrnmfrmhtchcnfgtwsvrrdngtkndrngthrls) [[pypi]]
-   [`[2020-03-31]` why it is hard &#x2013; if you have 2fa you can't upload packages](#whytshrdfyhvfycntpldpckgs) [[pypi]]
    -   [`[2020-03-31]` ah ok, actually it allows for a token, so even better!](#hkctllytllwsfrtknsvnbttr) 
-   [`[2019-12-15]` tox support python-poetry/poetry](#txspprtpythnptryptry) 
-   [find<sub>packages</sub> in setup.py?](#fndpckgsnstppy) [[python]]
-   [eee](#37975_38503) [[ipython]]
-   [`[2019-09-01]` KoffeinFlummi/Chronyk: A Python 3 library for parsing human-written times and dates](#kffnflmmchrnykpythnlbrryfrprsnghmnwrttntmsnddts) 
-   [`[2019-11-17]` sampleproject/setup.py at master · pypa/sampleproject](#smplprjctstppytmstrpypsmplprjct) 
-   [nicer attribute errors](#ncrttrbtrrrs) [[python]]
    -   [would be nice to do this hpi:](#wldbnctdthshp) 
-   [`[2019-07-25]` pytest-profiling · PyPI](#pytstprflngpyp) 
-   [Poetry easy pip publishing](#ptrysypppblshng) 
-   [use quit instead of close?](#sqtnstdfcls) [[selenium]]
-   [`[2020-10-06]` Brython](#sbrythnnfbrythn) [[python]] [[web]]
-   [`[2020-01-09]` logzero: Python logging made easy — logzero 1.5.0 documentation](#lgzrpythnlggngmdsylgzrdcmnttn) 
-   [marshmallow for db handling looks interesting&#x2026;](#mrshmllwfrdbhndlnglksntrstng) [[python]]
-   [PandaPy](#pndpy) 
-   [`[2019-10-27]` Ability to execute certain tests sequentially while using -n (xdist) · Issue #385 · pytest-dev/pytest-xdist](#bltytxctcrtntstssqntllywhngnxdstsspytstdvpytstxdst) 
-   [`[2019-10-27]` pylint exceed maximum recursion depth · Issue #2388 · PyCQA/pylint](#pylntxcdmxmmrcrsndpthsspycqpylnt) 
-   [`[2019-10-27]` Search pylint configuration in setup.cfg and pyproject.toml · Issue #617 · PyCQA/pylint](#srchpylntcnfgrtnnstpcfgndpyprjcttmlsspycqpylnt) 
-   [`[2019-11-08]` How do I use regex in a SQLite query? - Stack Overflow](#hwdsrgxnsqltqrystckvrflw) [[sqlite]]
-   [-pdbcls=IPython.terminal.debugger:TerminalPdb &#x2013;pdb](#pdbclspythntrmnldbggrtrmnlpdbpdb) [[python]] [[ipython]] [[debug]]
-   [wonder how to make sure dataclasses are represented very effecienly?](#wndrhwtmksrdtclsssrrprsntdvryffcnly) [[python]]
-   [`[2020-06-07]` Types at the edges in Python – MeadSteve's Dev Blog](#sblgmdstvdvprgrmmngtypsttpstthdgsnpythnmdstvsdvblg) [[python]]
-   [figuring out why has the package ended up in path](#fgrngtwhyhsthpckgnddpnpth) [[python]]
-   [`[2020-12-08]` Exhaustiveness Checking with Mypy | Haki Benita](#shkbntcmpythnmypyxhstvchchstvnsschckngwthmypyhkbnt) [[python]] [[mypy]]
-   [hvplot: clever algebra on plots](#hvpltclvrlgbrnplts) [[bokeh]]
-   [`[2020-04-09]` naiquevin/pipdeptree: A command line utility to display dependency tree of the installed Python packages [NOT ACCEPTING PRs FOR A WHILE BECAUSE OF MAJOR REFACTORING IN ANOTHER BRANCH]](#nqvnppdptrcmmndlntltytdsplbcsfmjrrfctrngnnthrbrnch) 
-   [`[2020-04-23]` pandas/setup.py at master · pandas-dev/pandas](#sgthbcmpndsdvpndsblbmstrsypndsstppytmstrpndsdvpnds) [[pip]]
    -   [`[2020-05-09]` nice, pandas is using quite elaborate setup.py with proper documentation links](#ncpndsssngqtlbrtstppywthprprdcmnttnlnks) 
-   [`[2019-07-28]` kirankoduru/scrapy-programmatically: Running scrapy spider programmatically.](#krnkdrscrpyprgrmmtcllyrnnngscrpyspdrprgrmmtclly) [[scrape]]
-   [`[2020-04-23]` detect all subpackages properly · karlicoss/promnesia@f7451c4](#sgthbcmkrlcssprmnsrnschckbpckgsprprlykrlcssprmnsfc) 
-   [`[2020-04-05]` Configs suck? Try a real programming language | Hacker News](#cnfgsscktryrlprgrmmnglngghckrnws) 
-   [`[2020-10-14]` google/python-fire: Python Fire is a library for automatically generating command line interfaces (CLIs) from absolutely any Python object.](#sgthbcmgglpythnfrgglpythncsclsfrmbsltlynypythnbjct) [[cli]]
-   [`[2020-04-23]` samuelhwilliams/Eel: A little Python library for making simple Electron-like HTML/JS GUI apps](#sgthbcmsmlhwllmslsmlhwllmmkngsmpllctrnlkhtmljsgpps) [[gui]]
-   [`[2020-04-15]` setuptools/\_<sub>init</sub>\_<sub>.py</sub> at master · pypa/setuptools](#sgthbcmpypstptlsblbmstrstlstptlsntpytmstrpypstptls) 
-   [keeping testss side by side with code](#kpngtstsssdbysdwthcd) [[pytest]]
-   [`[2020-04-30]` pkgutil — Package extension utility — Python 3.8.3rc1 documentation](#sdcspythnrglbrrypkgtlhtmlkgxtnsntltypythnrcdcmnttn) 
-   [`[2020-03-24]` PEP 593 &#x2013; Flexible function and variable annotations | Python.org](#ppflxblfnctnndvrblnnttnspythnrg) 
-   [`[2019-08-24]` Simple dependent types in Python - DEV Community 👩‍💻👨‍💻](#smpldpndnttypsnpythndvcmmnty) [[mypy]] [[python]]
-   [`[2020-07-08]` SymPy - a Python library for symbolic mathematics | Hacker News](#snwsycmbntrcmtmdsympypythrryfrsymblcmthmtcshckrnws) [[sympy]] [[sage]]
-   [`[2020-07-26]` The Qt Console for Jupyter — Jupyter Qt Console 4.7.5 documentation](#sqtcnslrdthdcsnstblthqtcnfrjpytrjpytrqtcnsldcmnttn) 
-   [`[2020-10-15]` Frame Hacks](#frmdvcmsrcscrtsfrmhckfrmhcks) [[python]]
-   [`[2019-03-17]` pylint useful stuff](#pylntsflstff) [[python]]
-   [try using devpi for uploading?](#trysngdvpfrpldng) [[tox]]
-   [`[2020-05-25]` docopt v argparse • Dimitri Merejkowsky](#sdmrjnfblgpstdcptvrgprsdcptvrgprsdmtrmrjkwsky) [[python]]
-   [`[2019-12-08]` Dynamically change <span class="underline"><span class="underline">slots</span></span> in Python 3 - Stack Overflow](#dynmcllychngsltsnpythnstckvrflw) [[python]]
-   [`[2020-10-24]` LiveCode is a modern day HyperCard (2019) | Hacker News](#snwsycmbntrcmtmdlvcdsmdrndyhyprcrdhckrnws) [[python]] [[gui]]
-   [`[2020-01-15]` Show HN: CrossHair – SMT Assisted Testing for Python](#snwsycmbntrcmtmdshwhncrsshrsmtssstdtstngfrpythn) [[testing]] [[python]]
-   [`[2019-11-10]` lihaoyi/macropy: Macros in Python: quasiquotes, case classes, LINQ and more!](#lhymcrpymcrsnpythnqsqtscsclssslnqndmr) [[macro]] [[python]] [[lisp]]
    -   [`[2020-05-16]` wow that's amazing https://macropy3.readthedocs.io/en/latest/discussion.html#function-advice](#wwthtsmzngsmcrpyrdthdcsnltstdscssnhtmlfnctndvc) 
-   [`[2020-01-09]` What does it do? — Logbook](#whtdstdlgbk) [[python]] [[logging]]
-   [`[2019-11-24]` How formulas work — patsy 0.5.1+dev documentation](#hwfrmlswrkptsydvdcmnttn) 
-   [`[2019-12-20]` Pipenv: promises a lot, delivers very little | Chris Warrick](#ppnvprmssltdlvrsvrylttlchrswrrck) [[pip]]
-   [`[2020-08-19]` install<sub>requires</sub> vs requirements files — Python Packaging User Guide](#spckgngpythnrgdscssnsnstlrqrmntsflspythnpckgngsrgd) [[pip]]
-   [`[2019-04-10]` kynan/nbstripout: strip output from Jupyter and IPython notebooks](#kynnnbstrptstrptptfrmjpytrndpythnntbks) [[git]] [[ipython]]
-   [`[2020-08-22]` Plotly vs. Bokeh: Interactive Python Visualisation Pros and Cons | Paul Iacomi](#splcmcmpltlyvbkhhtmlpltlytvpythnvslstnprsndcnsplcm) [[bokeh]] [[viz]]
-   [hack to allow optional git dependencies](#hcktllwptnlgtdpndncs) [[pip]] [[pypi]]
-   [`[2020-03-14]` jestem króliczkiem on Twitter: "or, you can encode dependencies in types: @dataclass(init=False) class FancyPath: path: Path mtime: float def \_<sub>init</sub>\_<sub>(self, path: Path)</sub>: self.path = path self.mtime = path.stat().st<sub>mtime</sub>" / Twitter](#jstmkrólczkmntwttrrycnncdpthslfmtmpthsttstmtmtwttr) [[cachew]] [[python]]
-   [`[2020-04-11]` Traps for the Unwary in Python’s Import System — Nick Coghlan's Python Notes 1.0 documentation](#trpsfrthnwrynpythnsmprtsymnckcghlnspythnntsdcmnttn) [[python]]
-   [`[2020-05-13]` amontalenti/elements-of-python-style: Goes beyond PEP8 to discuss what makes Python code feel great. A Strunk & White for Python.](#sgthbcmmntlntlmntsfpythnsthncdflgrtstrnkwhtfrpythn) [[python]]
-   [`[2020-05-18]` The Definitive Guide to Python import Statements | Chris Yeh](#schrsyhgthbdfntvgdpythnmpgdtpythnmprtsttmntschrsyh) [[python]]
-   [`[2020-08-09]` resize ipython notebook output window - Stack Overflow](#sstckvrflwcmqstnsrszpythnpythnntbktptwndwstckvrflw) 
-   [`[2020-01-26]` Not really. Enable something like MyPy or PyType on a big enough codebase with z&#x2026; | Hacker News](#ntrllynblsmthnglkmypyrpytypnbgnghcdbswthzhckrnws) 
-   [`[2020-07-21]` tmbo/questionary: Python library to build pretty command line user prompts ✨Easy to use multi-select lists, confirmations, free text prompts &#x2026;](#sgthbcmtmbqstnrytmbqstnryctlstscnfrmtnsfrtxtprmpts) [[tui]]
-   [`[2020-09-07]` Good Integration Practices — pytest documentation](#sdcspytstrgnstblgdprctcshdntgrtnprctcspytstdcmnttn) 
-   [`[2019-07-23]` Python Scatterplot Matrix | Plotly](#pythnscttrpltmtrxpltly) [[viz]]
-   [`[2019-08-18]` box/flaky: Plugin for nose or pytest that automatically reruns flaky tests.](#bxflkyplgnfrnsrpytstthttmtcllyrrnsflkytsts) [[pytest]]
-   [`[2019-03-05]` ipython -pylab](#pythnpylb) [[ipython]]
-   [`[2018-12-23]` lambdalisue/jupyter-vim-binding: Jupyter meets Vim. Vimmer will fall in love.](#lmbdlsjpytrvmbndngjpytrmtsvmvmmrwllfllnlv) [[vim]] [[jupyter]]
    -   [`[2019-04-13]` eh, I'm using emacs now&#x2026;](#hmsngmcsnw) 
-   [`[2019-05-10]` Is SQLAlchemy recommended for a highly transactional, large volume database? /r/Python](#srddtcmrpythncmmntspnssqlytrnsctnllrgvlmdtbsrpythn) 
-   [`[2020-02-16]` Command Line Scripts — Python Packaging Tutorial](#cmmndlnscrptspythnpckgngttrl) [[pip]]
    -   [`[2020-12-14]` hmm maybe best to use 'scripts', seems more manageable](#hmmmybbsttsscrptssmsmrmngbl) 
-   [`[2019-10-18]` Hy - Wikipedia](#hywkpd) [[lisp]] [[python]]
-   [`[2019-12-18]` Python VS Common Lisp, workflow and ecosystem - Lisp journey](#pythnvscmmnlspwrkflwndcsystmlspjrny) [[lisp]] [[python]]
-   [`[2019-02-27]` When do you us Beautiful Soup or Scrapy? : Python](#whndysbtflsprscrpypythn) [[scrape]] [[python]]
    -   [`[2019-03-05]` TLDR: scrapy is better](#tldrscrpysbttr) 
-   [`[2019-04-07]` DataFrame — pandas 0.24.2 documentation](#dtfrmpndsdcmnttn) [[pandas]]
-   [`[2019-04-07]` Comparison with SQL — pandas 0.24.2 documentation](#cmprsnwthsqlpndsdcmnttn) [[pandas]]
-   [`[2019-02-14]` There's now a dead simple way to slap a web interface on a command line script : Python (click library)](#thrsnwddsmplwytslpwbntrfcmmndlnscrptpythnclcklbrry) [[tui]] [[web]]
-   [`[2020-05-26]` multiprocess.Pool + submit<sub>async</sub> work properly with timeouts&#x2026; unlike concurrent.futures?](#mltprcssplsbmtsyncwrkprprlywthtmtsnlkcncrrntftrs) [[python]]
-   [`[2020-03-08]` dataset: right, so sync<sub>column</sub> is taking quite a bit of time&#x2026; I suppose because of column detection stuff](#dtstrghtssyncclmnstkngqtbtftmsppsbcsfclmndtctnstff) [[sqlite]] [[python]]
-   [gotcha with yield](#gtchwthyld) [[yield]] [[python]]
-   [`[2019-07-23]` date index](#dtndx) [[pandas]] [[python]] [[data]]
-   [`[2019-07-23]` Which one is better: Bokeh or Plotly? - Quora](#whchnsbttrbkhrpltlyqr) [[viz]] [[python]]
-   [`[2019-07-23]` Plotly vs Bokeh vs &#x2026; : Python](#pltlyvsbkhvspythn) [[viz]] [[python]]
-   [`[2019-05-18]` unwrap vs assert: assert is a statement, so can't do in one line](#nwrpvsssrtssrtssttmntscntdnnln) [[python]]
-   [`[2018-11-10]` imp.load<sub>source</sub> for loading python module from file](#mpldsrcfrldngpythnmdlfrmfl) [[python]]
-   [`[2018-06-21]` Ok, to prevent pollution just assert everything in <span class="underline">\_all</span> isinstance](#ktprvntplltnjstssrtvrythngnllsnstnc) [[python]]
-   [`[2018-08-26]` dill seems to be superior to pickle](#dllsmstbsprrtpckl) 
-   [`[2019-02-12]` Choosing a Python Visualization Tool - Practical Business Python](#chsngpythnvslztntlprctclbsnsspythn) [[python]] [[viz]]
-   [`[2019-02-12]` Quickstart — Bokeh 1.0.4 documentation](#qckstrtbkhdcmnttn) [[viz]]
    -   [`[2019-04-06]` ok, so apparently bokeh is more akin to plotly?](#kspprntlybkhsmrkntpltly) 
-   [`[2019-02-12]` python - how to set readable xticks in seaborn's facetgrid? - Stack Overflow](#pythnhwtstrdblxtcksnsbrnsfctgrdstckvrflw) [[plotting]] [[seaborn]]
-   [`[2019-12-12]` #45 Control color of each marker | seaborn – The Python Graph Gallery](#cntrlclrfchmrkrsbrnthpythngrphgllry) [[seaborn]]
-   [`[2020-01-17]` python - Format x-axis on chart created with pandas plot method - Stack Overflow](#pythnfrmtxxsnchrtcrtdwthpndspltmthdstckvrflw) [[drill]] [[pandas]]
-   [`[2020-04-18]` screw hatch. it's got some weird defaults and doesn't provide much value](#scrwhtchtsgtsmwrddfltsnddsntprvdmchvl) [[pip]]
-   [`[2020-02-16]` python - Argparse: Way to include default values in '&#x2013;help'? - Stack Overflow](#pythnrgprswytnclddfltvlsnhlpstckvrflw) 
-   [`[2019-07-20]` I created a GitHub repository explaining the complete process of gathering data, transforming it, getting insights and making plots using pandas, NumPy, Matplotlib and Seaborn. /r/Python](#srddtcmrpythncmmntscfymcrdsnmpymtpltlbndsbrnrpythn) [[python]] [[viz]]
-   [`[2020-02-18]` google/pytype: A static type analyzer for Python code](#gglpytypsttctypnlyzrfrpythncd) 
-   [`[2020-01-03]` Comparing Python Command-Line Parsing Libraries – Argparse, Docopt, and Click | Hacker News](#cmprngpythncmmndlnprsnglbrrsrgprsdcptndclckhckrnws) [[python]]
-   [`[2020-10-24]` sdispater/pendulum: Python datetimes made easy](#sgthbcmsdsptrpndlmsdsptrpndlmpythndttmsmdsy) [[python]] [[datetime]]
-   [`[2020-09-05]` fastcore: An Underrated Python Library | fastpages](#sfstpgsfstfstcrfstcrnndrrtdpythnlbrryfstpgs) [[python]]
-   [`[2021-01-05]` On Repl-Driven Programming | Hacker News](#snwsycmbntrcmtmdnrpldrvnprgrmmnghckrnws) [[repl]]
-   [`[2020-11-28]` ast — Abstract Syntax Trees — Python 3.9.1rc1 documentation](#sdcspythnrglbrrysthtmlstbrctsyntxtrspythnrcdcmnttn) 
-   [`[2019-12-27]` Why Python is my Favorite Language • Buttondown](#whypythnsmyfvrtlnggbttndwn) 
-   [`[2020-12-17]` wrapt · PyPI](#spyprgprjctwrptwrptpyp) 
-   [`[2020-12-13]` pydot/pydot: Python interface to Graphviz's Dot language](#sgthbcmpydtpydtpydtpydtpythnntrfctgrphvzsdtlngg) [[viz]]
-   [`[2020-12-05]` NBSafety Fearless interactivity for Jupyter notebooks](#snbsftyrgnbsftyfrlssntrctvtyfrjpytrntbks) 
-   [`[2020-12-29]` Top 10 Python libraries of 2020 you should know about | Tryolabs Blog](#strylbscmblgtppythnlbrrsflbrrsfyshldknwbttrylbsblg) 
-   [`[2020-09-03]` Overviews — PyViz 0.0.1 documentation](#spyvzrgvrvwsndxhtmlvrvwspyvzdcmnttn) 
-   [`[2020-12-05]` fastai/nbdev: Create delightful python projects using Jupyter Notebooks](#sgthbcmfstnbdvfstnbdvcrtdlpythnprjctssngjpytrntbks) 
-   [`[2020-12-07]` Running Python code in a subprocess with a time limit | Simon Willison’s TILs](#stlsmnwllsnntpythnsbprcssprcsswthtmlmtsmnwllsnstls) 
-   [`[2020-12-07]` tiangolo/typer: Typer, build great CLIs. Easy to code. Based on Python type hints.](#sgthbcmtngltyprtngltyprtytclssytcdbsdnpythntyphnts) 
-   [`[2020-11-30]` Allow to customize location of .eggs directory · Issue #1854 · pypa/setuptools](#sgthbcmpypstptlssssllwtcslctnfggsdrctrysspypstptls) 
-   [`[2020-10-20]` PyInstrument – A statistical Python profile that focuses on the slow parts | Hacker News](#snwsycmbntrcmtmdpynstrmntlthtfcssnthslwprtshckrnws) 
-   [`[2020-11-25]` python - Extract traceback info from an exception object - Stack Overflow](#sstckvrflwcmqstnsxtrcttrcknffrmnxcptnbjctstckvrflw) [[errors]]
-   [frustrating: so much duplication](#frstrtngsmchdplctn) [[pip]]
-   [`[2020-05-28]` Hypermodern Python | Lobsters](#slbstrssdcjhyprmdrnpythnckvrlkhyprmdrnpythnlbstrs) 
-   [`[2020-05-30]` The Hard Part of Learning a Language • Hillel Wayne](#swwwhlllwyncmpstlrnnglnggthhrdprtflrnnglngghlllwyn) [[toblog]] [[python]]
-   [I've gained massive amounts of random Python knowledge over the past month of actively working on my projects](#vgndmssvmntsfrndmpythnknwtmnthfctvlywrkngnmyprjcts) [[toblog]] [[python]]
-   [`[2020-01-04]` python - How can I make setuptools install a package that's not on PyPI? - Stack Overflow](#pythnhwcnmkstptlsnstllpckgthtsntnpypstckvrflw) 
-   [`[2020-04-17]` pypa/gh-action-pypi-publish: GitHub Action for publishing pre-built distribution packages to PyPI (from \`dist/\` dir)](#sgthbcmpypghctnpyppblshpytdstrbtnpckgstpypfrmdstdr) [[githubci]]
-   [`[2020-04-18]` Publishing package distribution releases using GitHub Actions CI/CD workflows — Python Packaging User Guide](#spckgngpythnrggdspblshngpccdwrkflwspythnpckgngsrgd) [[githubci]]
-   [`[2020-12-22]` uva-graphics/autoimp: Automatic Python imports](#sgthbcmvgrphcstmpvgrphcstmptmtcpythnmprts) 
-   [`[2020-01-25]` My Python setup for 2020 | Noam Elfanbaum https://noamelf.com/posts/my-python-setup-for-2020/](#mypythnstpfrnmlfnbmsnmlfcmpstsmypythnstpfr) 
-   [`[2019-09-17]` Vendoring Python dependencies with pip - Underdog.io Engineering Team - Medium https://medium.com/underdog-io-engineering/vendoring-python-dependencies-with-pip-b9eb6078b9c0](#vndrngpythndpndncswthppnddrngpythndpndncswthppbbbc) [[python]]
-   [`[2020-02-04]` PyPy - Performance https://pypy.org/performance.html#profiler](#pypyprfrmncspypyrgprfrmnchtmlprflr) 
-   [`[2020-05-03]` PEP 612 &#x2013; Parameter Specification Variables | Python.org](#swwwpythnrgdvppsppppprmtrspcfctnvrblspythnrg) 
-   [`[2020-01-06]` Please Fix Your Decorators · Homepage of Hynek Schlawack https://hynek.me/articles/decorators/](#plsfxyrdcrtrshmpgfhynkschlwckshynkmrtclsdcrtrs) 
-   [`[2019-09-23]` bast/somepackage: Show how to structure a Python project. https://github.com/bast/somepackage](#bstsmpckgshwhwtstrctrpythnprjctsgthbcmbstsmpckg) 
-   [`[2019-11-17]` holtzy/The-Python-Graph-Gallery: A website displaying hundreds of charts made with Python https://github.com/holtzy/The-Python-Graph-Gallery](#hltzythpythngrphgllrywbsthbcmhltzythpythngrphgllry) [[viz]]
-   [`[2019-12-05]` Debugging Jupyter notebooks - David Hamann https://davidhamann.de/2017/04/22/debugging-jupyter-notebooks/](#dbggngjpytrntbksdvdhmnnsdvdhmnnddbggngjpytrntbks) 
-   [`[2019-12-13]` python-poetry/poetry: Python dependency management and packaging made easy. https://github.com/python-poetry/poetry](#pythnptryptrypythndpndncygmdsysgthbcmpythnptryptry) 
-   [`[2020-12-13]` Do You Have Any Offline Programming Techniques or Tools? | Lobsters](#slbstrsskpxdyhvnyfflnprgrnprgrmmngtchnqsrtlslbstrs) 
-   [`[2020-02-15]` pschanely/CrossHair: A static analysis tool for Python that blurs the line between testing and type systems. https://github.com/pschanely/CrossHair](#pschnlycrsshrsttcnlysstlfystmssgthbcmpschnlycrsshr) 
-   [`[2020-04-15]` egg-info in local directory makes pip think package is installed · Issue #6558 · pypa/pip](#sgthbcmpypppsssggnfnlcldrsppthnkpckgsnstlldsspyppp) 
-   [`[2020-04-15]` I hate easy-install.pth · Issue #929 · fonttools/fonttools](#sgthbcmfnttlsfnttlsssshtsynstllpthssfnttlsfnttls) 
-   [`[2020-05-16]` macropy: syntactic macros for Python | Lobsters](#slbstrssvyzgmcrpysyntctcmysyntctcmcrsfrpythnlbstrs) 
-   [`[2020-08-22]` Installation — HoloViews 1.13.3 documentation](#hlvwsrgnstlltnhlvwsdcmnttn) 
-   [`[2021-02-14]` ok, naming test modules the same as originals doesn't end up well&#x2026;](#knmngtstmdlsthsmsrgnlsdsntndpwll) [[python]]
-   [`[2021-02-09]` python - Using property() on classmethods - Stack Overflow](#sstckvrflwcmqstnssngprprtprprtynclssmthdsstckvrflw) 
-   [`[2021-02-10]` Web Scraping 101 with Python | Hacker News](#snwsycmbntrcmtmdwbscrpngwthpythnhckrnws) 
-   [&#x2013;system-site-packages?](#systmstpckgs) [[pipx]]
-   [strptime idea &#x2013; cache time string and somehow speed up?](#strptmdcchtmstrngndsmhwspdp) [[python]]
-   [hmm, maybe possible to self-pack minimal package in setup.py? could work&#x2026;](#hmmmybpssbltslfpckmnmlpckgnstppycldwrk) [[python]]
-   [`[2021-02-23]` Tiendil/smart-imports: smart imports for Python](#sgthbcmtndlsmrtmprtstndlsmrtmprtssmrtmprtsfrpythn) [[python]]
-   [`[2021-02-21]` djrobstep/logx: best practice, zero config python logging](#sgthbcmdjrbstplgxlstfswtfxbstprctczrcnfgpythnlggng) [[python]] [[logging]]
-   [`[2021-02-23]` textwrap — Text wrapping and filling — Python 3.8.5 documentation](#flsrshrdcpythnhtmllbrrytxwrppngndfllngpythndcmnttn) 
-   [`[2020-04-09]` thebjorn/pydeps: Python Module Dependency graphs https://github.com/thebjorn/pydeps](#thbjrnpydpspythnmdldpndncygrphssgthbcmthbjrnpydps) [[project]] [[python]]
-   [`[2020-05-15]` Hello flake8 • Dimitri Merejkowsky](#sdmrjnfblgpsthllflkhllflkdmtrmrjkwsky) [[pylint]]
-   [`[2020-07-06]` Brython – A Python 3 implementation for client-side web programming | Hacker News](#snwsycmbntrcmtmdbrythnpytfrclntsdwbprgrmmnghckrnws) [[python]] [[js]]
-   [`[2021-03-16]` leeoniya/uPlot: 📈 A small, fast chart for time series, lines, areas, ohlc & bars](#sgthbcmlnypltlnypltsmllfstchrtfrtmsrslnsrshlcbrs) [[python]] [[dataviz]]
-   [`[2021-04-02]` cleanup; remove unused imports by seanbreckenridge · Pull Request 151 · karlicoss/HPI](#sgthbcmkrlcsshppllsscmmntsnbrcknrdgpllrqstkrlcsshp) [[flake8]]
-   [`[2021-03-23]` Iterables vs. Iterators vs. Generators » nvie.com](#snvcmpststrtrsvsgnrtrstrblsvstrtrsvsgnrtrsnvcm) [[python]]
-   [`[2021-03-07]` hhatto/autopep8: A tool that automatically formats Python code to conform to the PEP 8 style guide.](#sgthbcmhhtttppcnfgrtnhhttspythncdtcnfrmtthppstylgd) [[python]]
-   [`[2021-03-20]` python - Suspend on exception in pdb - Stack Overflow](#sstckvrflwcmqstnssspndnxcnsspndnxcptnnpdbstckvrflw) [[python]] [[debug]]
-   [tips about putting test next to code](#tpsbtpttngtstnxttcd) [[python]] [[toblog]]
-   [`[2021-04-04]` How to make an unaware datetime timezone aware in python - Stack Overflow](#sstckvrflwcmqstnshwtmknnwdttmtmznwrnpythnstckvrflw) [[tz]]
-   [`[2021-04-06]` python - How do I parse an ISO 8601-formatted date? - Stack Overflow](#sstckvrflwcmqstnshwdprsnshwdprsnsfrmttddtstckvrflw) 
-   [`[2021-03-30]` setuptools - python: simple example for a python egg with a one-file source file? - Stack Overflow](#sstckvrflwcmqstnspythnsmpthnggwthnflsrcflstckvrflw) [[pip]]
-   [`[2021-04-04]` Utilities — Click Documentation (7.x)](#sclckplltsprjctscmnxtlsshprgrssbrstltsclckdcmnttnx) [[cli]] [[python]]
-   [`[2021-04-16]` pythonql/pythonql: A Query Language extension for Python: Query files, objects, SQL and NoSQL databases with a built-in query language](#sgthbcmpythnqlpythnqlpythndnsqldtbsswthbltnqrylngg) [[python]]
-   [`[2021-05-01]` PythonPackagingTerminology - Python Wiki](#swkpythnrgmnpythnpckgngtrpythnpckgngtrmnlgypythnwk) [[pip]]





# \* testing      [[testing]]





## `[2020-03-27]` Hypothesis has a set of Pandas strategies for generating data      [[pandas]]

    https://www.hillelwayne.com/talks/beyond-unit-tests/




## `[2020-05-05]` [python - Run code before and after each test in py.test? - Stack Overflow](https://stackoverflow.com/questions/22627659/run-code-before-and-after-each-test-in-py-test)

    py.test fixtures are a technically adequate method to achieve your purpose.
    
    You just need to define a fixture like that:
    
    @pytest.fixture(autouse=True)
    def run_around_tests():




## `[2019-08-02]` python - How should I structure a pytest test only package? - Stack Overflow      [[testing]] [[project]] [[pip]]

<https://stackoverflow.com/questions/48111426/how-should-i-structure-a-pytest-test-only-package/48350323#48350323>  
distribute tests with package..  




## doctest? 




## pytest can detect recursion      [[pytest]]




# \* profiling      [[performance]]





## `[2020-03-08]` what-studio/profiling: An interactive continuous Python profiler

<https://github.com/what-studio/profiling>  

    profiling live-profile webserver.py

ok, this is really nice and easy to use  




### `[2020-07-28]` kinda unmaintainerd though?




## `[2019-07-20]` profiling with cprof

    python3 -m cProfile -o stats.prof script.py
    snakeviz stats.prof




## `[2020-01-13]` rkern/line<sub>profiler</sub>: Line-by-line profiling for Python

<https://github.com/rkern/line_profiler>  




## `[2018-03-10]` profiling

    python3 -m cProfile -s tottime process.py | less
    sudo apt install kcachegrind
    pip3 install --user pyprof2calltree

    https://julien.danjou.info/guide-to-python-profiling-cprofile-concrete-case-carbonara/
    python -m cProfile -o myscript.cprof myscript.py
    pyprof2calltree -k -i myscript.cprof




## ipython? 




## timeit 




# \* packaging      [[pip]]





## `[2020-04-02]` minimal-setup-py/setup.py at master · maet3608/minimal-setup-py

<https://github.com/maet3608/minimal-setup-py/blob/master/setup.py>  




## install only dependencies: `pip3 install --user -e .`




## install multiple packages at once

ok, apparently pip does use some sort of 'set compiling', so worth doing that  
  <https://github.com/pypa/pip/issues/988>  




## `[2020-04-24]` local PIP dependency: if the repo is in `/path/to/repo`, put `HPI@git+file://DUMMY/path/to/repo@master` in `setup.py`      [[pip]]

no idea why you need DUMMY bit, must be some parsing quirk :shrug:  
also, sometimes it needs //DUMMY, sometimes ///DUMMY ???  




## `[2019-12-15]` bast/pypi-howto: How to publish Python packages on PyPI.      [[pypi]]

<https://github.com/bast/pypi-howto>  




## `[2019-07-02]` Testing & Packaging · Homepage of Hynek Schlawack

<https://hynek.me/articles/testing-packaging/>  

    Your tests do not run against the package as it will be installed by its users. They run against whatever the situation in your project directory is.




### `[2019-07-25]` o

    To achieve that, you just move your packages into a src directory and add a where argument to find_packages() in your setup.py:
    
    setup(
        [...]
        packages=find_packages(where="src"),
        package_dir={"": "src"},
    )




## releasing on pypi      [[pypi]]

ok, that seems to be way easier  

    hatch build --clean --verbose
    hatch release --strict "$@"




# \* debugging      [[debug]]





## `[2019-04-09]` `with ipdb.launch_ipdb_on_exception()`      [[habit]]




## `[2019-12-05]` python3.7 has a `breakpoint()` builtin + more <https://hackernoon.com/python-3-7s-new-builtin-breakpoint-a-quick-tour-4f1aebc444c>




## `ipdb pp` for pretty print      [[habit]]




# \* bad things about python

-   lambdas suck  
    -   statements, not expressions, you are essentially restrictet to a single line
    -   no local variables in lambdas (although with walrus operation it's a bit better now)
    -   <http://math.andrej.com/2009/04/09/pythons-lambda-is-broken>
-   scoping (i.e. only local and global scopes)
-   GIL makes the concurrency very annoying at times
-   no static typing (although it's kinda okay now with annotations and #mypy)




# \* static analysers





## monkeytype &#x2013; automatic typing annotations generation      [[mypy]]




## would be nice to have  static analysis that checks you are not using global variables, etc.

however there are not any tools which do that&#x2026;  




## bandit  &#x2013; security checks      [[security]]

<https://github.com/openstack/bandit>  




### `[2021-01-16]` wouldn't say it's super useful&#x2026; might detect occasional eval or whatever, but won't help with more sophisticated stuff




# \* libraries





## `[2019-04-02]` peopledoc/workalendar: Worldwide holidays and workdays computational toolkit.

<https://github.com/peopledoc/workalendar>  




## `[2018-12-09]` Altair: Declarative Visualization in Python — Altair 2.3.0 documentation      [[viz]]

<https://altair-viz.github.io/index.html>  




# \* Import system





## figure it out &#x2013; very confusing!




## `[2017-12-17]` from . import module

local import  




## `[2020-01-17]` Alone Djangonaut – How python's import machinery works

<https://manikos.github.io/how-pythons-import-machinery-works>  

    origin




## `[2019-06-29]` python - Relative imports for the billionth time - Stack Overflow

<https://stackoverflow.com/questions/14132789/relative-imports-for-the-billionth-time>  

    .. are only relative in a package
    However, if your module's name is __main__, it is not considered to be in a package. Its name has no dots, and therefore you cannot use from .. import statements inside it. If you try to do so, you will get the "relative-import in non-package" error.




## `[2019-06-11]` relative imports are discouraged




# \* datetime handling      [[datetime]]





## `[2018-09-04]` utcfromtimestamp &#x2013; returns timestamp, unaware; fromtimestamp &#x2013; returns offset + timestamp, unaware

    In : datetime.fromtimestamp(123)
    Out: datetime.datetime(1970, 1, 1, 4, 2, 3)

    In : datetime.utcfromtimestamp(123)
    Out: datetime.datetime(1970, 1, 1, 0, 2, 3)




## `[2018-09-04]` ok, seems that it's better to use `pytz.utc.localize(tz_unaware_datetime)`




## `[2020-05-02]` [zachwill/moment: Dealing with dates in Python shouldn't have to suck.](https://github.com/zachwill/moment)

    # Create a moment with words in it
    moment.date("December 18, 2012")




## `[2020-05-02]` [zachwill/moment: Dealing with dates in Python shouldn't have to suck.](https://github.com/zachwill/moment)

    # Create a moment that would normally be pretty hard to do
    moment.date("2 weeks ago")




# \* logging      [[logging]]





## `[2018-07-05]` creating top level logger is always bad (may happen before configuring). use factory method      [[logging]]




# \* docs





## pydoc 

-k: keyword search  
-g: gui  




## ipython: ? and ??




# \* ipdb      [[ipdb]]

related #repl  




## `[2019-04-09]` python - Use IPython magic functions in ipdb shell - Stack Overflow

<https://stackoverflow.com/questions/16184487/use-ipython-magic-functions-in-ipdb-shell>  

    shell.find_line_magic('cpaste')()




# ---------------------------------- 




# `[2019-09-22]` [Python3 f-strings - A complete guide to the most well received feature of Python 3.](https://reddit.com/r/Python/comments/d4zfhc/python3_fstrings_a_complete_guide_to_the_most/f0ieyws/) /r/Python

    That’s a part of python’s data model like `len`, `reversed`, `iter`, …:
    `datetime` simply defines [`datetime.__format__`](https://docs.python.org/3/library/datetime.html#datetime.date.__format__). The method [is explained here](https://docs.python.org/3/reference/datamodel.html#object.__format__).




# `[2019-05-11]` To yield or not to yield      [[yield]]

<https://barahilia.github.io/blog/computers/2017/01/04/to-yield-or-not-to-yield.html>  

    Finally we came to this. To me it is more important that generators make code more elegant. Performance is usually relevant to smaller hot spots.
    The idea is simple: in comparison to list interface where computation results are first saved and are returned only at the end, “yielding” could reach faster code and reduce memory usage. As a quick simulation we may use %timeit magic command in IPython with the following two functions:




## `[2019-07-30]` good point about separating validation and generation




# AST `ast.dump(ast.parse("'a' in 'aa' in 'aaa'"))`




# use for &#x2013; else      [[habit]]




# `[2018-06-18]` log optimizers i used




# `[2018-06-11]` optimizing python CLI tools <https://files.bemusement.org/talks/OSDC2008-FastPython/>

interpreter &#x2013; about 10ms  
lazy imports  
profile slow imports  




# parser.add<sub>argument</sub>('rest, nargs=argparse.REMAINDER)      [[habit]]

process remaining arguments  




# awesome-python <https://github.com/vinta/awesome-python>

attrs &#x2013; could be interesting&#x2026; might solve stupid namedtuple addition etc.  
<https://github.com/python-attrs/attrs>  

This gives you the power to use actual classes with actual types in your code instead of confusing tuples or confusingly behaving namedtuples. Which in turn encourages you to write small classes that do one thing well. Never again violate the single responsibility principle just because implementing <span class="underline"><span class="underline">init</span></span> et al is a painful drag.  




## should definitely subscribe to its feed and go through again




## <https://github.com/vinta/awesome-python#command-line-tools> 




## pretty cool <https://github.com/timofurrer/try>




## cool <https://github.com/dbcli/mycli>




## hmm try that? <http://docopt.org/>




## some of these for nutrino? <https://github.com/vinta/awesome-python#database>




## hmm that's interesting, visual scraping <https://github.com/scrapinghub/portia>




## <https://www.reddit.com/r/coolgithubprojects/> 




## ?? <https://python.libhunt.com/>




# do not use replace tzinfo, always localize..      [[habit]]




# `[2019-01-01]` multiline string &#x2013; lstrip('\n') for nicer formatting!




# `[2019-03-20]` Tweet from Vladislav Isenbaev (@isenbaev), at Mar 20, 03:48: pickle просто скотски медленный, если что - кратно медленнее даже json'а

<https://twitter.com/isenbaev/status/1108213595920166912>  




# `[2019-08-11]` multiprocessing vs multithreading vs asyncio in Python 3.4 - Stack Overflow      [[concurrency]] [[performance]]

<https://stackoverflow.com/questions/27435284/multiprocessing-vs-multithreading-vs-asyncio-in-python-3-4>  

    if io_bound:
        if io_very_slow:
            print("Use Asyncio")
        else:
            print("Use Threads")
    else:
        print("Multi Processing")




# `[2020-01-03]` adamchainz/patchy: Patch the inner source of python functions at runtime.      [[lisp]]

<https://github.com/adamchainz/patchy#patchy>  

    Patch the inner source of python functions at runtime.




# `[2019-12-31]` PyPy.js: Python in the web browser | Hacker News      [[js]] [[webext]]

<https://news.ycombinator.com/item?id=17819138>  




# `[2018-06-22]` `difflib.unified_diff` is suuuuper slow&#x2026;




# `[2018-04-21]` scrapy debugging      [[scrapy]]

scrapy shell  

with<sub>secrets</sub> scrapy shell  

from scrapy.http import FormRequest  
request=FormRequest(url='http://www.quantified-mind.com/login',formdata={'Email': USER,'Password':PASSWORD,})  
fetch(request) &#x2013; redirects by default  

sets response variable  

you can do view(response) to view in browser  
mind that it might be different from browsing in chrome. because of user agent?  




# `[2018-08-30]` python's for..else makes in 'syntactially' look like a total function




# NamedTuple 





## use `typing.NamedTuple`




## watch out for default <span class="underline"><span class="underline">add</span></span> and <span class="underline"><span class="underline">mul</span></span>, it acts as adding pairs




## you can't easily overload <span class="underline"><span class="underline">init</span></span>, so make types of fields robust. Use a helper method instead

def N(\*args, \*\*kwargs):  
   reurn NamedTuple(whatevs)  




# Use contextmanager

-   @contextmanager; prepare; yield exactly once, then shutdown
-   `contextlib.redirect_stdout`  
    meh. I think it patches sys module? so it redirects sys.stdout calls only; but  not all stdout




# `[2018-12-08]` get current function/method name

def fname():  
    import inspect  
    return inspect.stack()[1][3]  




# traitlets? 




# `[2019-04-30]` [What's the difference between marshmallow and sql-alchemy?](https://reddit.com/r/flask/comments/9ort38/whats_the_difference_between_marshmallow_and/e7w8ror/) /r/flask

    Marshmallow “converts” (deserializes) dicts to SQLAlchemy models or serializes SQLAlchemy models to dicts.
    SQLAlchemy is an ORM. It maps database schema (tables) and data to Python objects.
    The two packages complement each other. They cannot and do not replace each others’ functionality.
    Flask-Marshmallow gives you a convenient interface to Marshmallow under Flask.




# `[2019-06-29]` dominatepp/.travis.yml at master · karlicoss/dominatepp      [[ci]]

<https://github.com/karlicoss/dominatepp/blob/master/.travis.yml>  
hmm, minimalistic travis is not so bad..  




# `[2019-08-12]` use `re.VERBOSE` for inline comments in regexes




# `[2019-10-21]` python - What do (lambda) function closures capture? - Stack Overflow      [[plt]]

<https://stackoverflow.com/questions/2295290/what-do-lambda-function-closures-capture>  

    Scoping in Python is dynamic and lexical. A closure will always remember the name and scope of the variable, not the object it's pointing to.




# `[2019-12-30]` argparse — Parser for command-line options, arguments and sub-commands — Python 3.8.1 documentation

<https://docs.python.org/3/library/argparse.html>  

    metavar - A name for the argument in usage messages.




# `[2020-01-07]` Performance — python-rapidjson 0.4 documentation      [[json]]

<https://python-rapidjson.readthedocs.io/en/latest/benchmarks.html>  
ok, so loads speedups are not that significant for my purposes  




# `[2019-07-19]` python - Argparse: Way to include default values in '&#x2013;help'? - Stack Overflow

<https://stackoverflow.com/questions/12151306/argparse-way-to-include-default-values-in-help/18507871#18507871>  

    Add '%(default)' to the help parameter to control what is displayed.




# `[2019-12-31]` PyPy - packages <http://packages.pypy.org>      [[pypy]]




# Construct: kinda like struct but better? <https://construct.readthedocs.io/en/latest/>      [[parsing]]




# Pyrser: grammars? <https://pythonhosted.org/pyrser/>      [[parsing]]




# `[2019-07-21]` kython@git+<https://github.com/karlicoss/kython.git@master> dependency for setup.cfg      [[pip]]




# `[2018-07-22]` PyCon 2018 Talk Videos : Python <https://www.reddit.com/r/Python/comments/8j4ep6/pycon_2018_talk_videos/>      [[towatch]]




# `[2019-08-02]` Basic usage — tox 3.13.3.dev13 documentation

<https://tox.readthedocs.io/en/latest/example/basic.html#integration-with-setup-py-test-command>  

    As the python eco-system rather moves away from using setup.py as a tool entry point it’s maybe best to not go for any setup.py test integration.




# `[2018-06-12]` if there is a 'main.py' in script dir, it gets imported &#x2013; wtf????

(while debugging telegram2org)  




# `[2019-07-20]` concurrent.futures <https://docs.python.org/3.7/library/concurrent.futures.html?highlight=processpoolexecutor> use `map`




# `[2019-08-11]` PyCQA/pyflakes: A simple program which checks Python source files for errors

<https://github.com/PyCQA/pyflakes>  

    Pyflakes makes a simple promise: it will never complain about style, and it will try very, very hard to never emit false positives.
    Pyflakes is also faster than Pylint or Pychecker. This is largely because Pyflakes only examines the syntax tree of each file individually. As a consequence, Pyflakes is more limited in the types of things it can check.




# `[2019-08-02]` posargs are needed to passing adhoc args, e.g.      [[tox]]

<https://tox.readthedocs.io/en/latest/example/general.html#interactively-passing-positional-arguments>  




# `[2018-04-17]` some misc notes

    ## Print with @padding
    `print("{:>d}{}".fomat(i, a[i]))` prints i aligned to at least two spaces as a decimal.
    
    ## Infinite dict
    ~~~ { .python }
    infinite_defaultdict = lambda: defaultdict(infinite_defaultdict)
    d = infinite_defaultdict()
    d['x']['y']['z'] = 10
    ~~~
    
    ## Web server
    to start a webserver to serve files from your current dir: python -m SimpleHTTPServer
    
    @enums
    
    ## Enums
    from enum import Enum
    class Fruit(Enum):
        APPLE = 0
        ORANGE = 1
    
    ## Generating @random color
    color = "#%06x" % random.randint(0, 0xFFFFFF)
    
    
    python setup.py install --force
    
    #singleton
    @singleton
    def singleton(cls):
        instances = {}
    
        def get_instance():
            if cls not in instances:
                instances[cls] = cls()
        return instances[cls]
    
    return get_instance
    TODO tbh, easier with lru_cache(1)?




# `from http import HTTPStatus`




# `[2018-01-21]` use nonlocal instead of global      [[habit]]




# !r formatter      [[habit]]




# `[2019-04-22]` yield is often preferrable because python doesn't have bindings in generators




# `[2019-05-01]` there is a difference between returning generator and yield from generator. the latter keeps scope, which might be useful if you have open files




# `[2019-07-30]` To yield or not to yield      [[decorator]]

<https://barahilia.github.io/blog/computers/2017/01/04/to-yield-or-not-to-yield.html>  
hmm. if I decorate function with list constructor, I can get both ease of use and yield in function's body  




## `[2019-07-30]` huh, some things are mentioned in the original post actually




# use putup (pyscaffold) for project generation      [[habit]]




# Poetry instead of pyscaffold?      [[python]]

    The best answer in 2020 is to use poetry.
    http://poetry.eustace.io




## `[2021-01-16]` eh, don't think it worked for me, I prefer to rely on setup.py




# `[2019-08-25]` <https://docs.python.org/3.7/library/argparse.html> argparse: use `set_defaults`

    One particularly effective way of handling sub-commands is to combine the use of the add_subparsers() method with calls to set_defaults() so that each subparser knows which Python function it should execute. For example:
    This way, you can let parse_args() do the job of calling the appropriate function after argument parsing is complete. Associating functions with actions like this is typically the easiest way to handle the different actions for each of your subparsers. However, if it is necessary to check the name of the subparser that was invoked, the dest keyword argument to the add_subparsers() call will work:




## `[2019-09-02]` ah, could pass lambda to forward to actual handler function!




# generate<sub>ordering</sub>?       [[python]]




# `[2020-07-05]` [How can I color Python logging output? - Stack Overflow](https://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output)      [[logging]] [[kython]]

    2020 code, no additional packages required, Python 3




# `[2020-02-16]` Direct URL PEP 508 support and installing sub-dependencies from Git · Issue 5566 · pypa/pip      [[pip]]

<https://github.com/pypa/pip/issues/5566#issuecomment-402417467>  

    We disabled the ability to use PEP 508 URL requirements in dependencies, since we don't want that a package installed from PyPI to result in the pip reaching out to an arbitary web URL. Basically, pip install spam should not make pip reach out to anything except PyPI.




# `[2020-02-16]` Allow direct urls in install<sub>requires</sub> · Issue 6301 · pypa/pip      [[python]]

<https://github.com/pypa/pip/issues/6301>  

    ugh. so I can't have URL dependencies if it's meant to be on pypi???




# `[2019-07-25]` rstojnic/lazydata: Lazydata: Scalable data dependencies for Python projects

<https://github.com/rstojnic/lazydata>  




## `[2020-03-27]` so it kinda keeps textual 'submodules' for data??




# using pytest fixtures to inject stuff into the module      [[python]] [[pytest]]





## `[2019-08-02]` like in tz provider




# end2end gui semi manual tests      [[promnesia]] [[python]] [[testing]]




# pytest dependencies      [[python]]

py, more-itertools, zipp, importlib-metadata, pluggy, six, pyparsing, packaging, atomicwrites, wcwidth, attrs, pytest, orger  




# `[2019-12-31]` backoff · PyPI

<https://pypi.org/project/backoff/>  

    It is also possible to specify an alternate logger with the logger keyword argument. If a string value is specified the logger will be looked up by name.




# Poetry for dep management      [[python]]

    We have moved our dependency management from pipenv to poetry and hasn’t been more happier than now working with and publish Python modules.
    Now we use pyenv with poetry to run all our projects in Python with venv in project instead of decided by poetry default settings. We changed the settings with:
    poetry config settings.virtualenvs.in-project true After this in hgignore or gitignore added .venv folder.
    Now everything is the way we wanted, with Pipenv many times faced issues that the project worked with requirements.txt but not in Pipenv. Didn’t have this issue moving to poetry yet.
    Also with emacs support and automated deployment tools the predictability of poetry made our team easy to work with and publish Python application modules.




# `[2019-12-15]` Support automatic versioning setuptools<sub>scm</sub>-style? · Issue 140 · python-poetry/poetry

<https://github.com/python-poetry/poetry/issues/140>  

    right, poetry can't infer version...




# it's clearly not detecting changes in `install_requires`; needed to reinsall      [[tox]]




# `[2019-07-26]` python - pytest exits with no error but with "collected 0 items" - Stack Overflow      [[pytest]]

<https://stackoverflow.com/questions/37353960/pytest-exits-with-no-error-but-with-collected-0-items>  

    pytest gathers tests according to a naming convention. By default any file that is to contain tests must be named starting with test_ and any function in a file that should be treated as a test must also start with test_.




# `[2019-10-26]` traceback — Print or retrieve a stack traceback — Python 3.8.0 documentation      [[errors]]

<https://docs.python.org/3/library/traceback.html#tracebackexception-objects>  

    TracebackException Objects

hmm, could use that?  




# separate testing and linting since mypy's deps might be installed by accident?      [[python]] [[tox]]




# `[2019-11-09]` python - Run an OLS regression with Pandas Data Frame - Stack Overflow

<https://stackoverflow.com/questions/19991445/run-an-ols-regression-with-pandas-data-frame>  

    I think you can almost do exactly what you thought would be ideal, using the statsmodels package which was one of pandas' optional dependencies before pandas' version 0.20.0 (it was used for a few things in pandas.stats.)




# figure out a better framework for python multiprocessing&#x2026;      [[python]]




# `[2019-09-01]` vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources      [[tui]]

<https://github.com/vinta/awesome-python>  

    urwid - A library for creating terminal GUI applications with strong support for widgets, events, rich colors, etc.




# sigh&#x2026; don't think it's possible to properly preserve stacktraces&#x2026;      [[python]] [[errors]]

    import logging
    logging.basicConfig()
    
    def bad():
        raise RuntimeError('BAD')
    
    xx = RuntimeError('while running "test"')
    ex = None
    try:
        bad()
    except Exception as e:
        ex = e
        ex.__cause__ = xx
        logging.error('inside!')
        logging.exception(ex)
    
    logging.error('outside! note the empty stacktrace :(')
    logging.exception(ex)
    logging.error("also __cause__ is ignored even though it's present: '%s'", ex.__cause__)
    # I guess it just doesn't use __cause__, only traceback information...
    
    test()




# strptime is incapable of handling timezones via %Z direcive??      [[python]] [[timezone]]

    In [20]: ds = "Sep 18 2018 5:48:23 UTC"
    
    In [21]: _TIME_FORMAT = "%b %d %Y %H:%M:%S %Z"
    
    In [22]: datetime.strptime(ds, _TIME_FORMAT)
    Out[22]: datetime.datetime(2018, 9, 18, 5, 48, 23)

fucking hell..  




## `[2020-03-27]` see takeout provider




# `[2020-03-12]` encode/httpx: A next generation HTTP client for Python. 🦋

<https://github.com/encode/httpx>  

    HTTPX is a fully featured HTTP client for Python 3, which provides sync and async APIs, and support for both HTTP/1.1 and HTTP/2.




# `[2020-09-02]` [Python Prompt Toolkit 3.0 — prompt<sub>toolkit</sub> 3.0.2 documentation](https://python-prompt-toolkit.readthedocs.io/en/master/index.html)      [[tui]] [[python]]




# `[2020-09-18]` [testing - Python/tox Install a dependency as editable - Stack Overflow](https://stackoverflow.com/questions/29284244/python-tox-install-a-dependency-as-editable)      [[python]] [[tox]] [[pip]]

how to install a dependency as editable  




# `[2020-09-18]` [testing - Python/tox Install a dependency as editable - Stack Overflow](https://stackoverflow.com/questions/29284244/python-tox-install-a-dependency-as-editable)      [[hpi]]

add this to developer guide.. fucking hell  




# `[2020-09-27]` [python - What is the difference between venv, pyvenv, pyenv, virtualenv, virtualenvwrapper, pipenv, etc? - Stack Overflow](https://stackoverflow.com/questions/41573587/what-is-the-difference-between-venv-pyvenv-pyenv-virtualenv-virtualenvwrappe)

    pipenv- like venv - can be used to create virtual envelopes but additionally rolls-in package management and vulnerability checking functionality. Instead of using requirements.txt, pipenv delivers package management via Pipfile. As PyPA endorses pipenv for PACKAGE MANAGEMENT, that would seem to imply pipfile is to supplant requirements.txt.
    
    HOWEVER: pipenv uses virtualenv as its tool for creating virtual envelopes, NOT venv which is endorsed by PyPA as the go-to tool for creating virtual envelopes.




# adapter thigs with getattr (like in workout provider for org notes) &#x2013; pretty great for adding one missing method      [[python]]




# `[2019-08-25]` argparseweb · PyPI

<https://pypi.org/project/argparseweb>  




# `[2019-09-01]` vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources      [[cli]]

<https://github.com/vinta/awesome-python>  

    Command-line Interface Development
    Libraries for building command-line applications.
        Command-line Application Development




# `[2019-08-02]` GrahamDumpleton/wrapt: A Python module for decorators, wrappers and monkey patching.

<https://github.com/GrahamDumpleton/wrapt>  

    It therefore goes way beyond existing mechanisms such as functools.wraps() to ensure that decorators preserve introspectability, signatures, type checking abilities etc. Th




# attemt to figure out mixed sem/cal versioning      [[project]] [[pip]]

<https://github.com/pypa/setuptools_scm/#default-versioning-scheme>  

    def semcal(v):
        tag = v.tag.base_version
        assert len(tag.split('.')) == 2, tag
        v.time
        # tag is
        breakpoint()
        pass
    
    
    if __name__ == '__main__':
        [pkg] = find_packages('src')
        setup(
            name=pkg,
            # version='0.1.1',
            # use_scm_version=True,
            use_scm_version={
                'version_scheme': semcal,
            },
            setup_requires=['setuptools_scm'],




# had to remore username from hatch config? it was overriding <span class="underline"><span class="underline">token</span></span> during the release..      [[pypi]]




# `[2020-03-31]` why it is hard &#x2013; if you have 2fa you can't upload packages      [[pypi]]





## `[2020-03-31]` ah ok, actually it allows for a token, so even better!




# `[2019-12-15]` tox support python-poetry/poetry

<https://github.com/python-poetry/poetry/issues/222>  

    For now, you can use poetry with tox by using something similar to what I did in pendulum: https://github.com/sdispater/pendulum/blob/master/tox.ini




# find<sub>packages</sub> in setup.py?      [[python]]

    Although, beware that you may need to change `find_packages()` to `find_namespace_packages()` in your setup.py.
    I get burned by that one a lot!




# eee       [[ipython]]

    ldisplay_md("hi")
    TODO shit. try and work on it?
    also provide these as utils..
    from IPython.display import display, Latex
    display(Markdown("Heat equation:"), heat_eq)
    display(Markdown("Boundary conditions:"))
    display(Latex(r"\begin{cases} x \\ y \end{cases}"), bc_left, bc_right)
    display(Markdown('hi'))
    That doesn't look great. `display` is quoting plain




# `[2019-09-01]` KoffeinFlummi/Chronyk: A Python 3 library for parsing human-written times and dates

<https://github.com/KoffeinFlummi/Chronyk>  




# `[2019-11-17]` sampleproject/setup.py at master · pypa/sampleproject

<https://github.com/pypa/sampleproject/blob/master/setup.py>  

    # This field corresponds to the "Description-Content-Type" metadata field:
    # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
    long_description_content_type='text/markdown',  # Optional (see note above)




# nicer attribute errors      [[python]]

    AttributeError: unexpected attribute 'color' to Line, similar attributes are line_color




## would be nice to do this hpi:




# `[2019-07-25]` pytest-profiling · PyPI

<https://pypi.org/project/pytest-profiling/>  




# Poetry easy pip publishing

    Even putting aside it's approach to dependency management, Poetry has a fond place in my heart for making it so much easier to publish to PyPI.
    If poetry did nothing but simply the process of publishing and updating python packages, it would still be an amazing tool.




# use quit instead of close?      [[selenium]]




# `[2020-10-06]` [Brython](https://brython.info/)      [[python]] [[web]]

    Speed of execution is similar to CPython for most operations.




# `[2020-01-09]` logzero: Python logging made easy — logzero 1.5.0 documentation

<https://logzero.readthedocs.io/en/latest/>  

    logzero.setup_logger(name=None, logfile




# marshmallow for db handling looks interesting&#x2026;      [[python]]

<https://github.com/marshmallow-code/marshmallow>  
zoopla/zoopla/schemas.py  




# PandaPy 

    PandaPy has the speed of NumPy and the usability of Pandas - https://news.ycombinator.com/item?id=22142869




# `[2019-10-27]` Ability to execute certain tests sequentially while using -n (xdist) · Issue #385 · pytest-dev/pytest-xdist

<https://github.com/pytest-dev/pytest-xdist/issues/385>  

    Isn't this enough?
    py.test -m sequential
    py.test -m "non sequential" -n8




# `[2019-10-27]` pylint exceed maximum recursion depth · Issue #2388 · PyCQA/pylint

<https://github.com/PyCQA/pylint/issues/2388>  

    Thanks for the tip. I actually had that setting before and still keep it on. --extension-pkg-whitelist=numpy
    However, after upgrading to later versions of python and pylint and astroid I no longer have the issue even with the numpy whitelist setting.
    Python 3.7.1
    pylint 2.3.1
    astroid 2.2.5




# `[2019-10-27]` Search pylint configuration in setup.cfg and pyproject.toml · Issue #617 · PyCQA/pylint

<https://github.com/PyCQA/pylint/issues/617#event-2701192212>  

    Search pylint configuration in setup.cfg and pyproject.toml




# `[2019-11-08]` How do I use regex in a SQLite query? - Stack Overflow      [[sqlite]]

<https://stackoverflow.com/questions/5071601/how-do-i-use-regex-in-a-sqlite-query>  

    With python, assuming con is the connection to SQLite, you can define the required UDF by writing:
    con.create_function('regexp', 2, lambda x, y: 1 if re.search(x,y) else 0)




# -pdbcls=IPython.terminal.debugger:TerminalPdb &#x2013;pdb      [[python]] [[ipython]] [[debug]]




# wonder how to make sure dataclasses are represented very effecienly?      [[python]]




# `[2020-06-07]` [Types at the edges in Python – MeadSteve's Dev Blog](https://blog.meadsteve.dev/programming/2020/02/10/types-at-the-edges-in-python/)      [[python]]

    Pydantic checks that each key I expected exists and is of the correct type. So now all the assumptions I’ve made about the shape of the data is a runtime contract, expressed in native python. If in production it turns out that description is, in fact, optional I’ll get a very descriptive error and the code will fail early.




# figuring out why has the package ended up in path      [[python]]

    d for d in sorted(pkg_resources.working_set, key=lambda p: p.project_name)]




# `[2020-12-08]` [Exhaustiveness Checking with Mypy | Haki Benita](https://hakibenita.com/python-mypy-exhaustive-checking)      [[python]] [[mypy]]

    Exhaustiveness Checking

use else clause with NoReturn, then mypy assists in refining  




# hvplot: clever algebra on plots      [[bokeh]]

    wow! * (same plot) vs + (different plots) is pretty clever!
    also I like how multiplication doesn't commute so the 'first' plot wins the layout parameters




# `[2020-04-09]` naiquevin/pipdeptree: A command line utility to display dependency tree of the installed Python packages [NOT ACCEPTING PRs FOR A WHILE BECAUSE OF MAJOR REFACTORING IN ANOTHER BRANCH]

<https://github.com/naiquevin/pipdeptree>  




# `[2020-04-23]` [pandas/setup.py at master · pandas-dev/pandas](https://github.com/pandas-dev/pandas/blob/master/setup.py)      [[pip]]

    Docum




## `[2020-05-09]` nice, pandas is using quite elaborate setup.py with proper documentation links




# `[2019-07-28]` kirankoduru/scrapy-programmatically: Running scrapy spider programmatically.      [[scrape]]

<https://github.com/kirankoduru/scrapy-programmatically>  




# `[2020-04-23]` [detect all subpackages properly · karlicoss/promnesia@f7451c4](https://github.com/karlicoss/promnesia/runs/612863976?check_suite_focus=true)

    tests/integration_test.py::test_example_config
      /Users/runner/runners/2.169.1/work/promnesia/promnesia/.tox/py3/lib/python3.7/site-packages/hug/use.py:185: DeprecationWarning: invalid escape sequence \d
        status_code = int("".join(re.findall("\d+", response.status)))




# `[2020-04-05]` Configs suck? Try a real programming language | Hacker News

<https://news.ycombinator.com/item?id=22787332>  

    mjw1007 28 minutes ago [-]
    One variant of this is to use Python syntax but parse it with the `ast` module rather than evaluating it.
    This avoids the security problems and the risk that someone will start to write programs inside the configuration file, but gives you the reasonably nice and powerful syntax.




# `[2020-10-14]` [google/python-fire: Python Fire is a library for automatically generating command line interfaces (CLIs) from absolutely any Python object.](https://github.com/google/python-fire)      [[cli]]

    ython Fire is a library for automatically generating command line interfaces (CLIs) from absolutely any Python object.




# `[2020-04-23]` [samuelhwilliams/Eel: A little Python library for making simple Electron-like HTML/JS GUI apps](https://github.com/samuelhwilliams/Eel)      [[gui]]




# `[2020-04-15]` [setuptools/\_<sub>init</sub>\_<sub>.py</sub> at master · pypa/setuptools](https://github.com/pypa/setuptools/blob/master/setuptools/__init__.py#L80-L85)

why is it not including files at all??  




# keeping testss side by side with code      [[pytest]]

    import sys
    # make sure it doesn't need pytest in prod
    if 'pytest' in sys.modules:
        import pytest # type: ignore
    else:
        from unittest.mock import Mock
        pytest = Mock()




# `[2020-04-30]` [pkgutil — Package extension utility — Python 3.8.3rc1 documentation](https://docs.python.org/3/library/pkgutil.html)

    pkgutil.extend_path(path, name)
    
        Extend the search path for the modules which comprise a package. Intended use is to place the following code in a package’s __init__.py:
    
        from pkgutil import extend_path
        __path__ = extend_path(__path__, __name__)
    
        This will add to the package’s __path__ all subdirectories of directories on sys.path named after the package. This is useful if one wants to distribute different parts of a single logical package as multiple directories.




# `[2020-03-24]` PEP 593 &#x2013; Flexible function and variable annotations | Python.org

<https://www.python.org/dev/peps/pep-0593/>  




# `[2019-08-24]` Simple dependent types in Python - DEV Community 👩‍💻👨‍💻      [[mypy]] [[python]]

<https://dev.to/wemake-services/simple-dependent-types-in-python-4e14>  

    Now, we are going to combine our new knowledge about Literal and @overload together to solve our problem with open. At last!




# `[2020-07-08]` [SymPy - a Python library for symbolic mathematics | Hacker News](https://news.ycombinator.com/item?id=23747133)      [[sympy]] [[sage]]

    As one point of comparison, SymPy is comically slow compared to Sage. This is mostly because SymPy is purely Python; Sage on the other hand uses a derivative of GiNaC [1] for its internal symbolic expression representation, and then multiple external libraries for non-trivial operations. Symbolic transformations are mostly Maxima [3]. Sage literally converts expressions to strings, pipes them through a Maxima process, and then parses the result back. This is still much faster than the pure Python SymPy.
    There is an effort to speed up SymPy core, SymEngine [3], but it's been in development for years now, and still isn't integrated into SymPy. Not sure why.
    Case in point: 'expand("(2+3x+4x*y)^60")' takes 5 seconds with SymPy; Sage does the same in 0.02 seconds.




# `[2020-07-26]` [The Qt Console for Jupyter — Jupyter Qt Console 4.7.5 documentation](https://qtconsole.readthedocs.io/en/stable/)

    The Qt console is a very lightweight application that largely feels like a terminal, but provides a number of enhancements only possible in a GUI, such as inline figures, proper multi-line editing with syntax highlighting, graphical calltips, and much more. The Qt console can use any Jupyter kernel.




# `[2020-10-15]` [Frame Hacks](http://farmdev.com/src/secrets/framehack/)      [[python]]




# `[2019-03-17]` pylint useful stuff      [[python]]

    cell-var-from-loop -- can detect bad lambda capturing
     pylint --disable='C,fixme,'




# try using devpi for uploading?      [[tox]]




# `[2020-05-25]` [docopt v argparse • Dimitri Merejkowsky](https://dmerej.info/blog/post/docopt-v-argparse/)      [[python]]

    But for big projects with lots of subcommands, written in Python, using argparse may be a better idea, especially if you need to do advanced stuff for your parsing, like configuring common options in one function, allow plug-ins to change the command line API, and so on …




# `[2019-12-08]` Dynamically change <span class="underline"><span class="underline">slots</span></span> in Python 3 - Stack Overflow      [[python]]

<https://stackoverflow.com/questions/27907373/dynamically-change-slots-in-python-3>  

    Normally, an object's attributes are stored in a dict, which requires a fair bit of memory itself. If you are creating millions of objects then the space required by these dicts becomes prohibitive. __slots__ informs the python machinery that makes the class object that there will only be so many attributes refered to by instances of this class and what the names of the attributes will be. Therefore, the class can make an optimisation by storing the attributes directly on the instance rather than in a dict. It places the memory for the (pointers to the) attributes directly on the object, rather than creating a new dict for the object.




# `[2020-10-24]` [LiveCode is a modern day HyperCard (2019) | Hacker News](https://news.ycombinator.com/item?id=24874102)      [[python]] [[gui]]

    In the spirit of HN contrarian comments, I'd say the closest thing spiritually to a modern-day HyperCard is PySimpleGUI: https://github.com/PySimpleGUI




# `[2020-01-15]` [Show HN: CrossHair – SMT Assisted Testing for Python](https://news.ycombinator.com/item?id=22054433)      [[testing]] [[python]]

<https://github.com/pschanely/CrossHair>  




# `[2019-11-10]` lihaoyi/macropy: Macros in Python: quasiquotes, case classes, LINQ and more!      [[macro]] [[python]] [[lisp]]

<https://github.com/lihaoyi/macropy>  




## `[2020-05-16]` wow that's amazing <https://macropy3.readthedocs.io/en/latest/discussion.html#function-advice>




# `[2020-01-09]` What does it do? — Logbook      [[python]] [[logging]]

<https://logbook.readthedocs.io/en/stable/features.html#advantages-over-logging>  




# `[2019-11-24]` How formulas work — patsy 0.5.1+dev documentation

<https://patsy.readthedocs.io/en/latest/formulas.html>  

    The formula language is actually fairly simple once you get the hang of it, but if you’re ever in doubt as to what some construction means, you can always ask Patsy how it expands.




# `[2019-12-20]` Pipenv: promises a lot, delivers very little | Chris Warrick      [[pip]]

<https://chriswarrick.com/blog/2018/07/17/pipenv-promises-a-lot-delivers-very-little/>  




# `[2020-08-19]` [install<sub>requires</sub> vs requirements files — Python Packaging User Guide](https://packaging.python.org/discussions/install-requires-vs-requirements/)      [[pip]]

    Requirements Files described most simply, are just a list of pip install arguments placed into a file.
    Whereas install_requires defines the dependencies for a single project, Requirements Files are often used to define the requirements for a complete Python environment.
    Whereas install_requires requirements are minimal, requirements files often contain an exhaustive listing of pinned versions for the purpose of achieving repeatable installations of a complete environment.
    Whereas install_requires requirements are “Abstract”, i.e. not associated with any particular index, requirements files often contain pip options like --index-url or --find-links to make requirements “Concrete”, i.e. associated with a particular index or directory of packages. 1
    Whereas install_requires metadata is automatically analyzed by pip during an install, requirements files are not, and only are used when a user specifically installs them using pip install -r.




# `[2019-04-10]` kynan/nbstripout: strip output from Jupyter and IPython notebooks      [[git]] [[ipython]]

<https://github.com/kynan/nbstripout>  




# `[2020-08-22]` [Plotly vs. Bokeh: Interactive Python Visualisation Pros and Cons | Paul Iacomi](https://pauliacomi.com/2020/06/07/plotly-v-bokeh.html)      [[bokeh]] [[viz]]

pretty good comparizon  




# hack to allow optional git dependencies      [[pip]] [[pypi]]

    def building_for_pypi() -> bool:
        return sys.argv[1] == 'sdist'
       for_pypi = building_for_pypi()
               'my': [] if for_pypi else ['HPI @ git+https://github.com/karlicoss/my.git'],
           },




# `[2020-03-14]` jestem króliczkiem on Twitter: "or, you can encode dependencies in types: @dataclass(init=False) class FancyPath: path: Path mtime: float def \_<sub>init</sub>\_<sub>(self, path: Path)</sub>: self.path = path self.mtime = path.stat().st<sub>mtime</sub>" / Twitter      [[cachew]] [[python]]

<https://twitter.com/karlicoss/status/1238791294547353601>  

    @dataclass
    (init=False)
    class FancyPath:
        path: Path
        mtime: float
        def __init__(self, path: Path):
            self.path = path
            self.mtime = path.stat().st_mtime

right, I suppose it's type to use dataclasses  




# `[2020-04-11]` Traps for the Unwary in Python’s Import System — Nick Coghlan's Python Notes 1.0 documentation      [[python]]

<http://python-notes.curiousefficiency.org/en/latest/python_concepts/import_traps.html#the-init-py-trap>  




# `[2020-05-13]` [amontalenti/elements-of-python-style: Goes beyond PEP8 to discuss what makes Python code feel great. A Strunk & White for Python.](https://github.com/amontalenti/elements-of-python-style)      [[python]]

    Use parens (...) for fluent APIs




# `[2020-05-18]` [The Definitive Guide to Python import Statements | Chris Yeh](https://chrisyeh96.github.io/2017/08/08/definitive-guide-python-imports.html)      [[python]]




# `[2020-08-09]` [resize ipython notebook output window - Stack Overflow](https://stackoverflow.com/questions/18770504/resize-ipython-notebook-output-window)

    You can toggle the scroll window in the main menu of the notebook
    Cell -> Current Outputs -> Toggle Scrolling




# `[2020-01-26]` Not really. Enable something like MyPy or PyType on a big enough codebase with z&#x2026; | Hacker News

<https://news.ycombinator.com/item?id=21902827>  

    Not really. Enable something like MyPy or PyType on a big enough codebase with zero explicit annotation and it'll already find plenty of bugs and unhandled cases from the inferred types alone. Some of these are stuff a strong IDE may catch too (using the wrong function name, passing wrong number of args, etc), but some other ones are actually deeper in the code.
    
    So already, with zero annotations, you already get value out, let alone once you type a few tricky variables that are harder for Python to track.




# `[2020-07-21]` [tmbo/questionary: Python library to build pretty command line user prompts ✨Easy to use multi-select lists, confirmations, free text prompts &#x2026;](https://github.com/tmbo/questionary)      [[tui]]




# `[2020-09-07]` [Good Integration Practices — pytest documentation](https://docs.pytest.org/en/stable/goodpractices.html)

tests in a separate dir vs tests in a subpackage  




# `[2019-07-23]` Python Scatterplot Matrix | Plotly      [[viz]]

<https://plot.ly/python/splom/>  




# `[2019-08-18]` box/flaky: Plugin for nose or pytest that automatically reruns flaky tests.      [[pytest]]

<https://github.com/box/flaky>  




# `[2019-03-05]` ipython -pylab      [[ipython]]




# `[2018-12-23]` lambdalisue/jupyter-vim-binding: Jupyter meets Vim. Vimmer will fall in love.      [[vim]] [[jupyter]]

<https://github.com/lambdalisue/jupyter-vim-binding>  




## `[2019-04-13]` eh, I'm using emacs now&#x2026;




# `[2019-05-10]` [Is SQLAlchemy recommended for a highly transactional, large volume database?](https://reddit.com/r/Python/comments/3pn88a/is_sqlalchemy_recommended_for_a_highly/cw8ovva/) /r/Python

    Yes. I've written a few systems using SQLAlchemy that see 50-100k writes  and 200k or so reads per second, and as long as you're using the Core everything works fine. Also allows you to use the ORM for ease-of-development on bits that don't need performance.
    
    SQLAlchemy is probably the one library in which I've never reached the "wait, I need to do something and can't" point. Every single weird edge case I've had to handle has been supported either natively or by being able to access the raw interfaces directly in a clean way. Fantastic library, can't recommend it more highly.
    
    Also, the lead dev is extremely responsive on the google group and is more than happy to answer questions.




# `[2020-02-16]` Command Line Scripts — Python Packaging Tutorial      [[pip]]

<https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point>  




## `[2020-12-14]` hmm maybe best to use 'scripts', seems more manageable




# `[2019-10-18]` Hy - Wikipedia      [[lisp]] [[python]]

<https://en.wikipedia.org/wiki/Hy>  




# `[2019-12-18]` Python VS Common Lisp, workflow and ecosystem - Lisp journey      [[lisp]] [[python]]

<https://lisp-journey.gitlab.io/pythonvslisp>  
don't feel like it's very objective comparison.  
lots of things are picked etc  
although I'm not very positive towards lisp either  




# `[2019-02-27]` When do you us Beautiful Soup or Scrapy? : Python      [[scrape]] [[python]]

<https://www.reddit.com/r/Python/comments/69wym8/when_do_you_us_beautiful_soup_or_scrapy/>  

    why would you never use BS
    The selectors system lack in flexibility, it is slow and its HTML parser is not really good for the modern world of opening a page in a browser and looking at what's there to know what to do.




## `[2019-03-05]` TLDR: scrapy is better




# `[2019-04-07]` DataFrame — pandas 0.24.2 documentation      [[pandas]]

<https://pandas.pydata.org/pandas-docs/stable/reference/frame.html>  




# `[2019-04-07]` Comparison with SQL — pandas 0.24.2 documentation      [[pandas]]

<https://pandas.pydata.org/pandas-docs/stable/getting_started/comparison/comparison_with_sql.html#compare-with-sql-join>  




# `[2019-02-14]` There's now a dead simple way to slap a web interface on a command line script : Python (click library)      [[tui]] [[web]]

<https://www.reddit.com/r/Python/comments/akgctg/theres_now_a_dead_simple_way_to_slap_a_web/>  




# `[2020-05-26]` multiprocess.Pool + submit<sub>async</sub> work properly with timeouts&#x2026; unlike concurrent.futures?      [[python]]




# `[2020-03-08]` dataset: right, so sync<sub>column</sub> is taking quite a bit of time&#x2026; I suppose because of column detection stuff      [[sqlite]] [[python]]




# gotcha with yield      [[yield]] [[python]]

    def wrapped(path: Path):
        try:
            it = ex(path)
            # ugh. keeping yeild in the try section is not ideal, bt
            yield from it
        except Exception as e:
            breakpoint()




# `[2019-07-23]` date index      [[pandas]] [[python]] [[data]]

I guess it's somewhat useful to have multiple stages  

raw providers emit dataframe without any index in case of reporting dateless errors (if that makes sense)  
then consumer can filter out errors and present them and then choose their own index and aggregateion  




# `[2019-07-23]` Which one is better: Bokeh or Plotly? - Quora      [[viz]] [[python]]

<https://www.quora.com/Which-one-is-better-Bokeh-or-Plotly>  

    Compare Bokeh with Plotly
    1. Easy to install. The process is very similar to Plotly.
    2. Bokeh plot is not as interactive as Plotly.
    3. Limitation on drawing string value on plot. It looks like only the bar chart can take the string values. Date time string has to convert to DateTime type first in order to be on non-bar plots such as scatter, line, etc.
    4. It is not easy to overlay different type of plots on one figure.
    5. Less examples online.
    6. Less integrated with Panda than Plotly.




# `[2019-07-23]` Plotly vs Bokeh vs &#x2026; : Python      [[viz]] [[python]]

<https://www.reddit.com/r/Python/comments/5nwk9r/plotly_vs_bokeh_vs/>  

    The last advantage I found that plotly has over bokeh is that almost everything in plotly is a dict. This is really useful because I've found certain plotly functions are really slow for some reason or can't be called when you use the multiprocessing module because of pickling issues. Not a problem, in the end they generate dicts under the hood, you can do the same yourself and still pass those dicts to plotly. Also calling help() on plotly objects tells you what keys and values you need to add to your dict.




# `[2019-05-18]` unwrap vs assert: assert is a statement, so can't do in one line      [[python]]




# `[2018-11-10]` imp.load<sub>source</sub> for loading python module from file      [[python]]




# `[2018-06-21]` Ok, to prevent pollution just assert everything in <span class="underline">\_all</span> isinstance      [[python]]




# `[2018-08-26]` dill seems to be superior to pickle

e.g. unpicling requires exactly same modules etc? might be hard if you want to unpickle elsewhere  

<https://stackoverflow.com/a/25244948/706389>  




# `[2019-02-12]` Choosing a Python Visualization Tool - Practical Business Python      [[python]] [[viz]]

<https://pbpython.com/python-vis-flowchart.html>  




# `[2019-02-12]` Quickstart — Bokeh 1.0.4 documentation      [[viz]]

<https://bokeh.pydata.org/en/latest/docs/user_guide/quickstart.html#userguide-quickstart>  




## `[2019-04-06]` ok, so apparently bokeh is more akin to plotly?




# `[2019-02-12]` python - how to set readable xticks in seaborn's facetgrid? - Stack Overflow      [[plotting]] [[seaborn]]

<https://stackoverflow.com/questions/43727278/how-to-set-readable-xticks-in-seaborns-facetgrid>  

    The seaborn.pointplot is not the right tool for this plot.

plotting a lot of data via seaborn  




# `[2019-12-12]` #45 Control color of each marker | seaborn – The Python Graph Gallery      [[seaborn]]

<https://python-graph-gallery.com/45-control-color-of-each-marker-seaborn/>  

    scatter_kws={'facecolors':df['color']}




# `[2020-01-17]` python - Format x-axis on chart created with pandas plot method - Stack Overflow      [[drill]] [[pandas]]

<https://stackoverflow.com/questions/44496383/format-x-axis-on-chart-created-with-pandas-plot-method>  

    ax = df.plot(kind='bar')
    x_labels = df.index.strftime('%b')
    ax.set_xticklabels(x_labels)

Comment:  

    pandas date ticks




# `[2020-04-18]` screw hatch. it's got some weird defaults and doesn't provide much value      [[pip]]

i.e. default got username set to "", which gets in the way of using <span class="underline"><span class="underline">token</span></span>  




# `[2020-02-16]` python - Argparse: Way to include default values in '&#x2013;help'? - Stack Overflow

<https://stackoverflow.com/questions/12151306/argparse-way-to-include-default-values-in-help>  

    parser = argparse.ArgumentParser(
        # ... other options ...
        formatter_class=argparse.ArgumentDefaultsHelpFormatter)




# `[2019-07-20]` [I created a GitHub repository explaining the complete process of gathering data, transforming it, getting insights and making plots using pandas, NumPy, Matplotlib and Seaborn.](https://reddit.com/r/Python/comments/cf7y1m/i_created_a_github_repository_explaining_the/) /r/Python      [[python]] [[viz]]

-   `[2019-07-24]` I know all of that but maybe good for newbies




# `[2020-02-18]` google/pytype: A static type analyzer for Python code

<https://github.com/google/pytype>  




# `[2020-01-03]` Comparing Python Command-Line Parsing Libraries – Argparse, Docopt, and Click | Hacker News      [[python]]

<https://news.ycombinator.com/item?id=10185290>  

    I had a simpler case that I couldn't figure out using docopt. I was trying to add in tls flags into docker-compose to match docker. I could not get a combination working where you can just specify --tls to mean tls is true while still accepting --tls=true|false|0|1.




# `[2020-10-24]` [sdispater/pendulum: Python datetimes made easy](https://github.com/sdispater/pendulum)      [[python]] [[datetime]]

    Why not Arrow?
    
    Arrow is the most popular datetime library for Python right now, however its behavior and API can be erratic and unpredictable.




# `[2020-09-05]` [fastcore: An Underrated Python Library | fastpages](https://fastpages.fast.ai/fastcore/)      [[python]]




# `[2021-01-05]` [On Repl-Driven Programming | Hacker News](https://news.ycombinator.com/item?id=25620256)      [[repl]]

    Another way is ipython %edit magic command and $EDITOR set to vim and using %autoreload




# `[2020-11-28]` [ast — Abstract Syntax Trees — Python 3.9.1rc1 documentation](https://docs.python.org/3/library/ast.html)

    ast.literal_eval




# `[2019-12-27]` Why Python is my Favorite Language • Buttondown

<https://buttondown.email/hillelwayne/archive/why-python-is-my-favorite-language/>  

    What I need is an “X for Y”, but better. Something like To Ruby from Python or Go for Python Programmers only cover the core. They don’t cover the peripheral libraries or the lagangue ecosystem. Hyperpolyglot is better, but doesn’t talk much about the ecosystem. It also doesn’t compare across language families, which could be very helpful here.




# `[2020-12-17]` [wrapt · PyPI](https://pypi.org/project/wrapt/)

    Module for decorators, wrappers and monkey patching.




# `[2020-12-13]` [pydot/pydot: Python interface to Graphviz's Dot language](https://github.com/pydot/pydot)      [[viz]]




# `[2020-12-05]` [NBSafety](https://nbsafety.org/) Fearless interactivity for Jupyter notebooks




# `[2020-12-29]` [Top 10 Python libraries of 2020 you should know about | Tryolabs Blog](https://tryolabs.com/blog/2020/12/21/top-10-python-libraries-of-2020/)

    To power its capabilities, Typer internally stands on top of Click, which is very well-known and battle-tested. This means that it can leverage all its benefits, community and plugins, while starting simple with less boilerplate code and growing more complex as you need.




# `[2020-09-03]` [Overviews — PyViz 0.0.1 documentation](https://pyviz.org/overviews/index.html)




# `[2020-12-05]` [fastai/nbdev: Create delightful python projects using Jupyter Notebooks](https://github.com/fastai/nbdev)

    Features of Nbdev
        - Automatically generate docs from Jupyter notebooks. These docs are searchable and automatically hyperlinked to appropriate documentation pages by introspecting keywords you surround in backticks.
        - Utilities to automate the publishing of pypi and conda packages including version number management.
        - A robust, two-way sync between notebooks and source code, which allow you to use your IDE for code navigation or quick edits if desired.
        - Fine-grained control on hiding/showing cells: you can choose to hide entire cells, just the output, or just the input. Furthermore, you can embed cells in collapsible elements that are open or closed by default.
        - Ability to write tests directly in notebooks without having to learn special APIs. These tests get executed in parallel with a single CLI command. You can even define certain groups of tests such that you don't have to always run long-running tests.
        - Tools for merge/conflict resolution with notebooks in a human readable format.
        - Continuous integration (CI) comes setup for you with GitHub Actions




# `[2020-12-07]` [Running Python code in a subprocess with a time limit | Simon Willison’s TILs](https://til.simonwillison.net/python/subprocess-time-limit)

    Running Python code in a subprocess with a time limit




# `[2020-12-07]` [tiangolo/typer: Typer, build great CLIs. Easy to code. Based on Python type hints.](https://github.com/tiangolo/typer)

    Typer, build great CLIs. Easy to code. Based on Python type hints.




# `[2020-11-30]` [Allow to customize location of .eggs directory · Issue #1854 · pypa/setuptools](https://github.com/pypa/setuptools/issues/1854)

    My code lives in a read-only partition mounted into a Docker container and therefore the build fails:




# `[2020-10-20]` [PyInstrument – A statistical Python profile that focuses on the slow parts | Hacker News](https://news.ycombinator.com/item?id=24836833)




# `[2020-11-25]` [python - Extract traceback info from an exception object - Stack Overflow](https://stackoverflow.com/questions/11414894/extract-traceback-info-from-an-exception-object)      [[errors]]

    There's a very good reason the traceback is not stored in the exception; because the traceback holds references to its stack's locals, this would result in a circular reference and (temporary) memory leak until the circular GC kicks in. (This is why you should never store the traceback in a local variable.)




# frustrating: so much duplication      [[pip]]

there is github topics, github description, readme, pypi readem, readthedocs readme, classifiers etc  




# `[2020-05-28]` [Hypermodern Python | Lobsters](https://lobste.rs/s/2dcejo/hypermodern_python#c_kvr6lk)

    Agree. I now have a sudden urge to write a guide how to start from very simple (i.e. system interpreter, no packaging, minimal verification) and how to progress further on. And how to decide what tools do you even need to consider and at which stage.
    
    In hindsight as a somewhat experienced Python programmer I can see how each of these tools can be helpful – but if I was a beginner I would be completely overwhelmed.




# `[2020-05-30]` [The Hard Part of Learning a Language • Hillel Wayne](https://www.hillelwayne.com/post/learning-a-language/)      [[toblog]] [[python]]




# I've gained massive amounts of random Python knowledge over the past month of actively working on my projects      [[toblog]] [[python]]

but I have no idea how to communicate it.  
some problems are just obscure to write a proper blog post or something  
self-answering stackoverflow questions??  




# `[2020-01-04]` python - How can I make setuptools install a package that's not on PyPI? - Stack Overflow

<https://stackoverflow.com/questions/3472430/how-can-i-make-setuptools-install-a-package-thats-not-on-pypi>  
why python sucks: dependencies  




# `[2020-04-17]` [pypa/gh-action-pypi-publish: GitHub Action for publishing pre-built distribution packages to PyPI (from \`dist/\` dir)](https://github.com/pypa/gh-action-pypi-publish)      [[githubci]]

    - name: Publish a Python distribution to PyPI
      uses: pypa/gh-action-pypi-publish@master
      with:
        user: __token__
        password: ${{ secrets.pypi_password }}

so much indirection!!  




# `[2020-04-18]` [Publishing package distribution releases using GitHub Actions CI/CD workflows — Python Packaging User Guide](https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/)      [[githubci]]




# `[2020-12-22]` [uva-graphics/autoimp: Automatic Python imports](https://github.com/uva-graphics/autoimp)

    The autoimp module imports all available Python modules automatically at the Python interactive prompt, similarly to Matlab:




# `[2020-01-25]` My Python setup for 2020 | Noam Elfanbaum <https://noamelf.com/posts/my-python-setup-for-2020/>

    pyenv install 3.8.0
    pyenv shell 3.8.0
    https://noamelf.com/posts/my-python-setup-for-2020/




# `[2019-09-17]` Vendoring Python dependencies with pip - Underdog.io Engineering Team - Medium <https://medium.com/underdog-io-engineering/vendoring-python-dependencies-with-pip-b9eb6078b9c0>      [[python]]




# `[2020-02-04]` PyPy - Performance <https://pypy.org/performance.html#profiler>

    PyPy 2.6 introduced vmprof, a very-low-overhead statistical profiler. The standard, non-statistical cProfile is also supported, and can be enabled without turning off the JIT. We do recommend vmprof anyway because turning on cProfile can distort the result (sometimes massively, though hopefully this should not be too common).




# `[2020-05-03]` [PEP 612 &#x2013; Parameter Specification Variables | Python.org](https://www.python.org/dev/peps/pep-0612/)




# `[2020-01-06]` Please Fix Your Decorators · Homepage of Hynek Schlawack <https://hynek.me/articles/decorators/>

    If your Python decorator unintentionally changes the signatures of my callables or doesn’t work with class methods, it’s broken and should be fixed. Sadly most decorators are broken because the web is full of bad advice.




# `[2019-09-23]` bast/somepackage: Show how to structure a Python project. <https://github.com/bast/somepackage>




# `[2019-11-17]` holtzy/The-Python-Graph-Gallery: A website displaying hundreds of charts made with Python <https://github.com/holtzy/The-Python-Graph-Gallery>      [[viz]]




# `[2019-12-05]` Debugging Jupyter notebooks - David Hamann <https://davidhamann.de/2017/04/22/debugging-jupyter-notebooks/>

    There’s also ipdb but importing and calling it directly only works in the terminal, not in notebooks (see this issue).




# `[2019-12-13]` python-poetry/poetry: Python dependency management and packaging made easy. <https://github.com/python-poetry/poetry>

    In other words, poetry uses pyproject.toml to replace setup.py, requirements.txt, setup.cfg, MANIFEST.in and the newly added Pipfile.




# `[2020-12-13]` [Do You Have Any Offline Programming Techniques or Tools? | Lobsters](https://lobste.rs/s/ik1apx/do_you_have_any_offline_programming)

    import pdb; pdb.pm() starts a post-mortem debugger. When you get an error in an interactive session (such as a Jupyter notebook), this will jump to the scene of the error, let you inspect local variables, and let you walk up and down the stack.




# `[2020-02-15]` pschanely/CrossHair: A static analysis tool for Python that blurs the line between testing and type systems. <https://github.com/pschanely/CrossHair>




# `[2020-04-15]` [egg-info in local directory makes pip think package is installed · Issue #6558 · pypa/pip](https://github.com/pypa/pip/issues/6558)

    egg-info in local directory makes pip think package is installed




# `[2020-04-15]` [I hate easy-install.pth · Issue #929 · fonttools/fonttools](https://github.com/fonttools/fonttools/issues/929)

    I hate easy-install.pth

shit. I guess this explains why it was finding mypkgs&#x2026;  




# `[2020-05-16]` [macropy: syntactic macros for Python | Lobsters](https://lobste.rs/s/4vyz7g/macropy_syntactic_macros_for_python)

    acropy is excellent when one wants to use syntactic macros. One problem I had was that, for my scripts, I cannot directly use macropy and other syntax modifiers since they rely on the import hooks, which means that you can not use them directly on the script file. You have to import them separately, which makes their use cumbersome.
    
    This was my project to work around this issue. It works, but is very hacky, and requires adding a new codec to the Python installation.




# `[2020-08-22]` [Installation — HoloViews 1.13.3 documentation](http://holoviews.org/)

    HoloViews is an open-source Python library designed to make data analysis and visualization seamless and simple. With HoloViews, you can usually express what you want to do in very few lines of code, letting you focus on what you are trying to explore and convey, not on the process of plotting.




# `[2021-02-14]` ok, naming test modules the same as originals doesn't end up well&#x2026;      [[python]]

e.g. when I was writing `pytest tests/core/test_pandas.py` vs `pytest tests/core/pandas.py`  




# `[2021-02-09]` [python - Using property() on classmethods - Stack Overflow](https://stackoverflow.com/questions/128573/using-property-on-classmethods)

    Python 3.9 2020 UPDATE
    You can just use them together (taken from the 3.9 docs):
    class G:
        @classmethod
        @property
        def __doc__(cls):
            return f'A doc for {cls.__name__!r}'




# `[2021-02-10]` [Web Scraping 101 with Python | Hacker News](https://news.ycombinator.com/item?id=26090243)

    import pandas as pd
    dfs = pd.read_html(url)

wow. can scrape off table elements?  




# &#x2013;system-site-packages?       [[pipx]]




# strptime idea &#x2013; cache time string and somehow speed up?      [[python]]

could be like re.Pattern, or with automatic cache?  




# hmm, maybe possible to self-pack minimal package in setup.py? could work&#x2026;      [[python]]




# `[2021-02-23]` [Tiendil/smart-imports: smart imports for Python](https://github.com/Tiendil/smart-imports)      [[python]]




# `[2021-02-21]` [djrobstep/logx: best practice, zero config python logging](https://github.com/djrobstep/logx#list-of-sweet-features)      [[python]] [[logging]]

reasonable list (aka why python logging sucks by default)  




# `[2021-02-23]` [textwrap — Text wrapping and filling — Python 3.8.5 documentation](file:///usr/share/doc/python3/html/library/textwrap.html)




# `[2020-04-09]` thebjorn/pydeps: Python Module Dependency graphs <https://github.com/thebjorn/pydeps>      [[project]] [[python]]




# `[2020-05-15]` [Hello flake8 • Dimitri Merejkowsky](https://dmerej.info/blog/post/hello-flake8/)      [[pylint]]

    Itamar Turner-Trauring 2, in the comment section on dev.to gave an interesting example:

handling accidental variable capture in closures  




# `[2020-07-06]` [Brython – A Python 3 implementation for client-side web programming | Hacker News](https://news.ycombinator.com/item?id=23746067)      [[python]] [[js]]




# `[2021-03-16]` [leeoniya/uPlot: 📈 A small, fast chart for time series, lines, areas, ohlc & bars](https://github.com/leeoniya/uPlot)      [[python]] [[dataviz]]

focus on performance?  




# `[2021-04-02]` [cleanup; remove unused imports by seanbreckenridge · Pull Request 151 · karlicoss/HPI](https://github.com/karlicoss/HPI/pull/151#issuecomment-812392144)      [[flake8]]

    find ./my | entr flake8 --ignore=E402,E501,E741,W503,E266,E302,E305,E203,E261,E252,E251,E221,W291,E225,E303,E702,E202,F841,E731,E306,E127 E722,E231 my | grep -v __NOT_HPI_MODULE__




# `[2021-03-23]` [Iterables vs. Iterators vs. Generators » nvie.com](https://nvie.com/posts/iterators-vs-generators/)      [[python]]

good tutorial  




# `[2021-03-07]` [hhatto/autopep8: A tool that automatically formats Python code to conform to the PEP 8 style guide.](https://github.com/hhatto/autopep8#configuration)      [[python]]

Seems like a more sensible alternative to black  




# `[2021-03-20]` [python - Suspend on exception in pdb - Stack Overflow](https://stackoverflow.com/questions/45446944/suspend-on-exception-in-pdb)      [[python]] [[debug]]

    You're looking for postmortem mode:
    
    try:
        code_that_may_raise_exception()
    except Exception:
        import pdb; pdb.post_mortem()
    
    This will break on exception and drop you into a debugger right where it is being raised from

nice! a bit magical, but works exactly as described  




# tips about putting test next to code      [[python]] [[toblog]]

-   no overhead about creating new files
-   no need to worry about pythonpaths etc

how to:  

-   pytest imports in the function itself
-   defensive decorator?
-   fixtures still work! like tmp<sub>path</sub>

TODO mention doctests? pros/cons. how to set up common env for doctests?  




# `[2021-04-04]` [How to make an unaware datetime timezone aware in python - Stack Overflow](https://stackoverflow.com/questions/7065164/how-to-make-an-unaware-datetime-timezone-aware-in-python/7065242)      [[tz]]

    >> unaware.replace(tzinfo=ZoneInfo('localtime'))
    datetime.datetime(2020, 10, 31, 12, 0, tzinfo=zoneinfo.ZoneInfo(key='localtime'))
    >>> str(_)
    '2020-10-31 12:00:00+01:00'
    pip install backports.zoneinfo




# `[2021-04-06]` [python - How do I parse an ISO 8601-formatted date? - Stack Overflow](https://stackoverflow.com/questions/127803/how-do-i-parse-an-iso-8601-formatted-date)

    Although strptime can parse the 'Z' character to UTC, fromisoformat is faster by ~ x40 (see also: A faster strptime):




# `[2021-03-30]` [setuptools - python: simple example for a python egg with a one-file source file? - Stack Overflow](https://stackoverflow.com/questions/2852413/python-simple-example-for-a-python-egg-with-a-one-file-source-file)      [[pip]]

    You can use the py_modules argument instead of the packages argument to list single file modules.
    See https://docs.python.org/3/distutils/setupscript.html#listing-individual-modules




# `[2021-04-04]` [Utilities — Click Documentation (7.x)](https://click.palletsprojects.com/en/7.x/utils/#showing-progress-bars)      [[cli]] [[python]]

progress bars, nice  




# `[2021-04-16]` [pythonql/pythonql: A Query Language extension for Python: Query files, objects, SQL and NoSQL databases with a built-in query language](https://github.com/pythonql/pythonql)      [[python]]

    PythonQL is implemented as a special encoding in a normal python script. When this encoding is specified, the pythonql preprocessor is run, which converts the pythonql syntax to pure python.
    So you should have a line in the beginning of your script:
    #coding: pythonql
    result = [ select y for x in [1,2,3] let y = x**2 ]

whoa  




# `[2021-05-01]` [PythonPackagingTerminology - Python Wiki](https://wiki.python.org/moin/PythonPackagingTerminology)      [[pip]]

    *.egg-link files that contain the name of a built or development egg, to support symbolic linking on platforms that do not have native symbolic links.

