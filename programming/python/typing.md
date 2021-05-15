
# Table of Contents

-   [\* 'philosophy' of mypy](#phlsphyfmypy) [[mypy]]
    -   [`[2019-12-08]` similar approach to mine: Statically-typed error handling in Python using Mypy | Hacker News](#smlrpprchtmnsnwsycmbntrcmndlngnpythnsngmypyhckrnws) 
    -   [`[2020-06-22]` We've been running mypy on our project for about a year now and it's one of the best decisions we've made | Hacker News](#snwsycmbntrcmtmdwvbnrnnngtsnfthbstdcsnswvmdhckrnws) [[mypy]]
    -   [`[2021-02-19]` you can use `--exclude`  to exclude (duh) individual files you haven't yet managed to type properly](#smypyrdthdcsnltstcmmndlnhlflsyhvntytmngdttypprprly) 
-   [\* typing tutorials/feature overviews](#typngttrlsftrvrvws) [[types]]
    -   [`[2019-12-30]` good mypy intro, demonstrates many important features: Python Type Hints – NP-Incompleteness](#gdmypyntrdmnstrtsmnymprtntspythntyphntsnpncmpltnss) [[mypy]]
    -   [`[2020-02-05]` Applying mypy to real world projects: very good intro on configuration & fine tuning](#clptrsncmmypyhntshtmlpplyctsvrygdntrncnfgrtnfntnng) [[mypy]]
    -   [`[2021-03-08]` mypy-assisted error handling](#sbpbpxyzmypyrrrhndlnghtmlmypyssstdrrrhndlng) [[mypy]]
    -   [`[2020-12-08]` Exhaustiveness Checking with Mypy | Haki Benita](#shkbntcmpythnmypyxhstvchchstvnsschckngwthmypyhkbnt) [[mypy]]
    -   [`[2020-01-26]` Hypermodern Python Chapter 4: Typing · Claudio Jolowicz's website](#scjlwczgthbpstshyprmdrnpyhnchptrtypngcldjlwczswbst) 
-   [\* various useful mypy tricks/features](#vrssflmypytrcksftrs) [[mypy]]
    -   [`[2018-10-12]` https://mypy.readthedocs.io/en/latest/additional\_features.html#dataclasses-support](#smypyrdthdcsnltstddtnlftrshtmldtclsssspprt) 
    -   [`get_origin/get_args` is nice for metaprogramming/automatic discovery](#gtrgngtrgssncfrmtprgrmmngtmtcdscvry) 
    -   [`[2019-10-26]` reveal<sub>type</sub> can be used during the type checking](#smypyrdthdcsnltstcmmnssshvltypcnbsddrngthtypchckng) 
    -   [flags I like](#sgthbcmkrlcsspympltblbmstrmypynflgslk) 
        -   [`disallow_generic_any` could be good&#x2026;](#dsllwgnrcnycldbgd) [[mypy]]
    -   [`[2020-10-05]` `from __future__ import annotations` to be able to write something like `list[int]`](#frmftrmprtnnttnstbbltwrtsmthnglklstnt) 
    -   [`[2019-12-08]` mypy is aware of `sys.version_info`, it can help for writing backwards compatible code](#swwwpythnrgdvppsppvrsnndphlpfrwrtngbckwrdscmptblcd) 
    -   [`[2020-05-06]` Protocols and structural subtyping](#smypyrdthdcsnstblprtclshtclsprtclsndstrctrlsbtypng) [[mypy]]
    -   [`[2019-10-12]` Protocols and structural subtyping — Mypy](#smypyrdthdcsnltstprtclshtrtclsndstrctrlsbtypngmypy) 
    -   [`[2020-08-19]` Reading a list of files from a file](#smypyrdthdcsnstblrnnngmypfflsfrmflrdnglstfflsfrmfl) [[mypy]]
-   [\* mypy gotchas/bugs](#mypygtchsbgs) [[mypy]]
    -   [`[2019-12-08]` Statically-typed error handling in Python using Mypy | Hacker News](#snwsycmbntrcmtmdsttcllytyndlngnpythnsngmypyhckrnws) 
        -   [`[2021-03-08]` I think it's a really annoying obstacle to typing adoption. Perhaps that's something setuptools could warn the developer about?](#thnktsrllynnyngbstclttypnthngstptlscldwrnthdvlprbt) 
    -   [`[2019-03-12]` looks like mypy doesn't like the lack of <span class="underline"><span class="underline">init</span></span> file, and struggles to discover submodules if it's missing?](#lkslkmypydsntlkthlckfntflrgglstdscvrsbmdlsftsmssng) 
    -   [`[2020-10-31]` mypy + multiple python versions](#mypymltplpythnvrsns) [[mypy]]
    -   [hmm, aliases aren't working with new annotations? `Rows = list[list[str]]`](#hmmlssrntwrkngwthnwnnttnsrwslstlststr) [[mypy]]
    -   [that's odd, behaviour when checking package vs files is different?](#thtsddbhvrwhnchckngpckgvsflssdffrnt) [[mypy]]
    -   [shit. I don't get why there is a difference between checking source and directly???](#shtdntgtwhythrsdffrncbtwnchckngsrcnddrctly) [[mypy]]
    -   [hmm, apparently function parameter/argument names are taken into the account?](#hmmpprntlyfnctnprmtrrgmntnmsrtknntthccnt) [[mypy]]
    -   [`[2018-06-20]` <span class="underline"><span class="underline">all</span></span> and pycharm and mypy](#llndpychrmndmypy) [[mypy]]
    -   [error with reusing exception variable: https://github.com/python/mypy/issues/5080](#rrrwthrsngxcptnvrblsgthbcmpythnmypysss) 
-   [\* typing complicated code](#typngcmplctdcd) [[mypy]]
    -   [`[2019-11-02]` Type hints for naive/aware datetime objects? : Python](#swwwrddtcmrpythncmmntsvddphntsfrnvwrdttmbjctspythn) [[datetime]] [[mypy]]
        -   [`[2019-12-20]` use NewType for that?](#snwtypfrtht) 
    -   [`[2019-10-27]` how to define type of `lru_cache` (also works on similar decorators)](#sgthbcmpythnmypyssshwtdfnypflrcchlswrksnsmlrdcrtrs) 
    -   [`[2020-05-25]` Making a decorator which preserves function signature · Issue 1927 · python/mypy](#sgthbcmpythnmypysssmkngdcsrvsfnctnsgntrsspythnmypy) [[mypy]]
    -   [`[2020-05-03]` Support function decorators excellently · Issue 3157 · python/mypy](#sgthbcmpythnmypyssssscmmndcrtrsxcllntlysspythnmypy) 
    -   [`[2019-12-07]` hack for preventing unnecessary module imports](#swwwrddtcmrpythncmmntshmjkfrprvntngnncssrymdlmprts) 
    -   [`[2019-08-31]` Define a JSON type · Issue 182 · python/typing](#sgthbcmpythntypngsssdfnjsntypsspythntypng) 
        -   [`[2019-08-31]` .](#15874_16091) 
    -   [`[2020-11-25]` Decorated property not supported · Issue 1362 · python/mypy](#sgthbcmpythnmypysssdcrtdprprtyntspprtdsspythnmypy) 
    -   [`[2018-12-11]` use `Protocol` for classes which I can't control, they are very neat!](#sprtclfrclssswhchcntcntrlthyrvrynt) [[python]] [[mypy]] [[habit]]
    -   [`[2021-02-11]` TypeVar to represent a Callable's arguments (for decorators/wrappers)](#sgthbcmpythnmypyssstypvrtllblsrgmntsfrdcrtrswrpprs) 
    -   [`[2019-04-16]` mypy overloads](#mypyvrlds) [[mypy]]
    -   [`[2019-12-07]` Still alive? · Issue 25 · machinalis/mypy-data https://github.com/machinalis/mypy-data/issues/25](#stlllvssmchnlsmypydtsgthbcmmchnlsmypydtsss) [[numpy]]
-   [\* other type checking tools](#thrtypchckngtls) [[types]]
    -   [`[2020-03-12]` pydantic](#spydntcdcshlpmnlpydntc) 
    -   [`[2020-03-22]` MonkeyType: A system for Python that automatically generates type annotations | Hacker News https://news.ycombinator.com/item?id=22624845](#mnkytypsystmfrpythnthttmtnshckrnwssnwsycmbntrcmtmd) 
-   [`[2019-09-16]` typeddjango/awesome-python-typing: Collection of awesome Python types, stubs, plugins, and tools to work with them.](#sgthbcmtypddjngwsmpythntysstbsplgnsndtlstwrkwththm) 
-   [`[2019-09-27]` Python Negatypes • Hillel Wayne](#swwwhlllwyncmpstngtypspythnngtypshlllwyn) [[types]]
-   [`[2020-10-03]` tried this https://github.com/predictive-analytics-lab/data-science-types seems to give many false positives&#x2026;](#trdthssgthbcmprdctvnlytcsscnctypssmstgvmnyflspstvs) [[pandas]] [[mypy]]
-   [https://github.com/wemake-services/wemake-python-styleguide/blob/master/styles/mypy.toml](#sgthbcmwmksrvcswmkpythnstylgdblbmstrstylsmypytml) [[mypy]]
-   [`[2019-12-30]` Show HN: FastAPI: build Python APIs with Go-like speed and automatic UI docs | Hacker News](#snwsycmbntrcmtmdshwhnfstpwthglkspdndtmtcdcshckrnws) 
    -   [`[2020-03-01]` ok, nice, so it uses mypy types, not custom types (like hug?)](#kncstssmypytypsntcstmtypslkhg) 
-   [stricter mypy flags](#strctrmypyflgs) 
-   [hmm, seems like fastapi always has to be wrapped in pydantic. ugh!](#hmmsmslkfstplwyshstbwrppdnpydntcgh) 
-   [PathIsh thing can be generalized to Path constructible?](#pthshthngcnbgnrlzdtpthcnstrctbl) [[mypy]]
    -   [`[2019-06-28]` not sure if <span class="underline"><span class="underline">init</span></span> would do well? https://mypy.readthedocs.io/en/latest/protocols.html](#ntsrfntwlddwllsmypyrdthdcsnltstprtclshtml) 
    -   [`[2019-08-24]` eh, so os.PathLike[str] kinda solves it, but using .pyi file for that is not really worth it](#hsspthlkstrkndslvstbtsngpyflfrthtsntrllywrtht) 
-   [seems like a bug in fbmessenger export (on a branch)](#smslkbgnfbmssngrxprtnbrnch) [[mypy]]
-   [-------------------------------------------------](#22330_22424) 
-   [`[2021-04-05]` crazy how useful it is to have gradual typing when you're gradually hardening the program, adding error hadnling etc](#crzyhwsfltsthvgrdltypngwhnngthprgrmddngrrrhdnlngtc) [[types]]

I used to be in the 'static types only' camp and kind of hated Python. But mypy (and [gradual typing](https://en.wikipedia.org/wiki/Gradual_typing)) changed my mind about dynamic languages in general.  
At some point it 'clicked' and I learnt to sense better when I'm comfortable with some dynamic madness, and when it makes sense to set it in stone by typing.  

Here I'm collecting some guides to get started, cool not well known features I find useful, and some common annoying issues.  
Mostly it's going to be about mypy, but not limited to.  




# \* 'philosophy' of mypy      [[mypy]]

Aka when and how it's best to use or not to use it  




## `[2019-12-08]` similar approach to mine: [Statically-typed error handling in Python using Mypy | Hacker News](https://news.ycombinator.com/item?id=21736620)

    My approach is to dial up strictness gradually as code proves its value. I'll start out building a project and not validating on I/O, but as the requirements get locked down and the code has proven itself, I'll clean up all the edge cases - which will often mean adding in progressively stricter validation on border code.
    The advantage of this is that if you end up not wasting too much time "building the wrong thing". Let's say that you took one form of I/O and built massively strict validation in and then realized later that you should have taken an entirely different form of I/O for your subsystem. All that time building in validation on that useless part of code was a pointless waste.
    I don't have any stats, but my gut feel is that on average 40% of code can end up being tossed in this way (in some projects it's 100% =).
    Prototyping speed is, additionally, not just useful in reducing the cost of building the right kind of code, it's useful in reducing the cost of building the right kind of test (a really underappreciated facet of building mission critical systems).
    In my younger years I used to believe that for mission critical systems "building the wrong thing" was somehow less of a problem in code because you could fix requirements and do architecture upfront with some sort of genius architect. Turns out this was wrong.




## `[2020-06-22]` [We've been running mypy on our project for about a year now and it's one of the best decisions we've made | Hacker News](https://news.ycombinator.com/item?id=22305446)      [[mypy]]

    We implemented it progressively. At first I added it as a make target but didn't make it mandatory in CI so I could learn how to use it.
    Then I made it mandatory for a few files that I was the only active contributor to.
    Then I slowly added more and more files across the project, sometimes as I touched them for other reason and other times as independent changes.
    Eventually as mypy caught more and more bugs in other contributor's changes they started getting on board and adding type hints as well, until the vast majority of the project was hinted (we'll be getting to 100% within a few weeks).

This is super reasonable, especially for existing projects which are hard to type in one go.  




## `[2021-02-19]` [you can use `--exclude` ](https://mypy.readthedocs.io/en/latest/command_line.html#cmdoption-mypy-exclude) to exclude (duh) individual files you haven't yet managed to type properly




# \* typing tutorials/feature overviews      [[types]]





## `[2019-12-30]` good mypy intro, demonstrates many important features: [Python Type Hints – NP-Incompleteness](https://kunigami.blog/2019/12/26/python-type-hints)      [[mypy]]




## `[2020-02-05]` [Applying mypy to real world projects](http://calpaterson.com/mypy-hints.html): very good intro on configuration & fine tuning      [[mypy]]




## `[2021-03-08]` [mypy-assisted error handling](https://beepb00p.xyz/mypy-error-handling.html)      [[mypy]]




## `[2020-12-08]` [Exhaustiveness Checking with Mypy | Haki Benita](https://hakibenita.com/python-mypy-exhaustive-checking#type-narrowing-in-mypy)      [[mypy]]




## `[2020-01-26]` [Hypermodern Python Chapter 4: Typing · Claudio Jolowicz's website](https://cjolowicz.github.io/posts/hypermodern-python-04-typing/)




# \* various useful mypy tricks/features      [[mypy]]





## `[2018-10-12]` <https://mypy.readthedocs.io/en/latest/additional_features.html#dataclasses-support>




## `get_origin/get_args` is nice for metaprogramming/automatic discovery

    get_origin(Union[T, int]) is Union
    get_origin(List[Tuple[T, T]][int]) == list
    get_args(Dict[str, int]) == (str, int)
    get_args(Union[int, Tuple[T, int]][str]) == (int, Tuple[str, int])

-   `[2021-03-08]` started using it in HPI for automatic output detection




## `[2019-10-26]` [reveal<sub>type</sub>](https://mypy.readthedocs.io/en/latest/common_issues.html?highlight=reveal_type#reveal-type) can be used during the type checking

`reveal_type(a)  # N: Revealed type is 'builtins.int'`  

    https://github.com/python/mypy/blob/09c243dcc12935b989367f31d1d25d7fd0ec634c/test-data/unit/check-python38.test

<https://github.com/python/mypy/blob/master/test-data/unit/README.md>  
apparently there is also `reveal_locals()`!  




## [flags I like](https://github.com/karlicoss/pymplate/blob/master/mypy.ini)

    pretty = True
    show_error_context = True
    show_error_codes = True
    check_untyped_defs = True
    namespace_packages = True

they probably make sense everywhere, you might even want to add them to ~/.config/mypy/config  




### `disallow_generic_any` could be good&#x2026;      [[mypy]]




## `[2020-10-05]` `from __future__ import annotations` to be able to write something like `list[int]`

[PEP 585 &#x2013; Type Hinting Generics In Standard Collections | Python.org](https://www.python.org/dev/peps/pep-0585/)  

    Starting with Python 3.7, when from __future__ import annotations is used, function and variable annotations can parameterize standard collections directly.
    haystack: dict[str, list[int]]




## `[2019-12-08]` [mypy is aware of `sys.version_info`](https://www.python.org/dev/peps/pep-0484/#version-and-platform-checking), it can help for writing backwards compatible code




## `[2020-05-06]` [Protocols and structural subtyping](https://mypy.readthedocs.io/en/stable/protocols.html#using-isinstance-with-protocols)      [[mypy]]

    You can use a protocol class with isinstance() if you decorate it with the @runtime_checkable class decorator. The decorator adds support for basic runtime structural checks:




## `[2019-10-12]` [Protocols and structural subtyping — Mypy](https://mypy.readthedocs.io/en/latest/protocols.html)

    isinstance() also works with the predefined protocols in typing such as Iterable.




## `[2020-08-19]` [Reading a list of files from a file](https://mypy.readthedocs.io/en/stable/running_mypy.html#reading-a-list-of-files-from-a-file)      [[mypy]]

    any command-line argument starting with @ reads additional command-line arguments from the file following the @ character.
    This is primarily useful if you have a file containing a list of files that you want to be type-checked




# \* mypy gotchas/bugs      [[mypy]]





## `[2019-12-08]` [Statically-typed error handling in Python using Mypy | Hacker News](https://news.ycombinator.com/item?id=21737700)

you need 'py.typed' file and also [explicitly mentioning it in setup.py](https://github.com/karlicoss/pymplate/blob/aa2b12775d190af44c0ea69fe43ae7f98045464e/setup.py#L24)  

    Third party libraries: I sometimes see them annotated, but what people don't suspect, is that you need to include 'py.typed' file with your package in order for it to be discoverable.




### `[2021-03-08]` I think it's a really annoying obstacle to typing adoption. Perhaps that's something setuptools could warn the developer about?




## `[2019-03-12]` looks like mypy doesn't like the lack of <span class="underline"><span class="underline">init</span></span> file, and struggles to discover submodules if it's missing?

My current workaround [is using `__init__.pyi`](https://github.com/karlicoss/pymplate/blob/master/src/karlicoss_pymplate/__init__.pyi)  




## `[2020-10-31]` mypy + multiple python versions      [[mypy]]

this is mypy friendly  

    if sys.version_info[:2] >= (3, 8):

this isn't  

    if sys.version_info.minor >= 7:




## hmm, aliases aren't working with new annotations? `Rows = list[list[str]]`      [[mypy]]

    TypeError: 'type' object is not subscriptable




## that's odd, behaviour when checking package vs files is different?      [[mypy]]

mypy wereyouhere/extractors/custom.py  

    wereyouhere/extractors/custom.py:56: error: Unexpected keyword argument "line" for "make" of "Loc"
    wereyouhere/extractors/custom.py:144: error: Too few arguments for "make" of "Loc"

mypy wereyouhere  

    no errors?




## shit. I don't get why there is a difference between checking source and directly???      [[mypy]]

    $ mypy my/endomondo.py
    my/endomondo.py:8: error: Skipping analyzing '.core.common': found module but no type hints or library stubs  [import]
        from .core.common import Paths, get_files
        ^
    my/endomondo.py:8: note: See https://mypy.readthedocs.io/en/latest/running_mypy.html#missing-imports
    my/endomondo.py:39: error: Skipping analyzing '.core.error': found module but no type hints or library stubs  [import]
        from .core.error import Res
        ^
    my/endomondo.py:54: error: Skipping analyzing '.core': found module but no type hints or library stubs  [import]
            from .core import stat
        ^
    Found 3 errors in 1 file (checked 1 source file)
    $ mypy -p my.endomondo
    my/endomondo.py: note: In function "workouts":
    my/endomondo.py:48: error: Incompatible types in "yield" (actual type "endoapi.endomondo.Workout", expected type "Union[my.endomondo.Workout, Exception]")  [misc]
                    yield w
                    ^
    Found 1 error in 1 file (checked 1 source file)




## hmm, apparently function parameter/argument names are taken into the account?      [[mypy]]

    def testx(x: int) -> None:
        pass
    
    def testy(y: int) -> None:
        pass
    
    test = testx
    test = testy




## `[2018-06-20]` <span class="underline"><span class="underline">all</span></span> and pycharm and mypy      [[mypy]]

TLDR: messing with <span class="underline"><span class="underline">all</span></span> results in problems, don't do that..  
I guess I have to be careful on module levels then if I don't want unwanted crap&#x2026;  




## error with reusing exception variable: <https://github.com/python/mypy/issues/5080>

    try:
      pass
    except Exception as e:
      pass
    
    for e in []:
      pass




# \* typing complicated code      [[mypy]]





## `[2019-11-02]` [Type hints for naive/aware datetime objects? : Python](https://www.reddit.com/r/Python/comments/79vddc/type_hints_for_naiveaware_datetime_objects)      [[datetime]] [[mypy]]





### `[2019-12-20]` use NewType for that?

    ndt = NewType('ndt', datetime.datetime)
    dt = NewType('dt', datetime.datetime)
    
    def dt_to_ndt(dt: dt) -> ndt:
        pass




## `[2019-10-27]` [how to define type of `lru_cache`](https://github.com/python/mypy/issues/5107) (also works on similar decorators)

    from typing import TYPE_CHECKING, TypeVar
    if TYPE_CHECKING:
        F = TypeVar('F', Callable)
        def lru_cache(f: F) -> F: pass
    else:
        from functools import lru_cache




## `[2020-05-25]` [Making a decorator which preserves function signature · Issue 1927 · python/mypy](https://github.com/python/mypy/issues/1927)      [[mypy]]

    from typing import Any, Callable, TypeVar
    FuncT = TypeVar('FuncT', bound=Callable[..., Any])

ok, this + overrides allowed me to type it properly  




## `[2020-05-03]` [Support function decorators excellently · Issue 3157 · python/mypy](https://github.com/python/mypy/issues/3157#issuecomment-502434084)

    Just for the record: if someone needs to change the return type of the function inside the decorator and still have typed parameters, you can use a custom mypy plugin that literally takes 15 LoC: https://github.com/dry-python/returns/blob/92eda5574a8e41f4f5af4dd29887337886301ee3/returns/contrib/mypy/decorator_plugin.py
    
    Saved me a lot of time!




## `[2019-12-07]` [hack for preventing unnecessary module imports](https://www.reddit.com/r/Python/comments/8hmjq9/the_other_great_benefit_of_python_type_annotations/dyl1wjt)

Type annotation will require importing modules that you wouldn't need to import without it. However there is now a workaround (quote the name and import in a dead if):  

    if False:
        from bar_module import bar
    
    def foo(a: 'bar'):
         pass




## `[2019-08-31]` [Define a JSON type · Issue 182 · python/typing](https://github.com/python/typing/issues/182)

    With that and the idea of string self referencing, JSONType can be defined as:
    
    from typing import Recursive, Union, List, Dict
    
    JSONType = Recursive(
        "JSONType",
        Union[int, float, str, bool, None, List["JSONType"], Dict[str, "JSONType"]]
    )




### `[2019-08-31]` .

    Unless I'm mistaken, recursive types with ForwardRefs can already be checked correctly at runtime by using ForwardRef._evaluate(globals(), locals())




## `[2020-11-25]` [Decorated property not supported · Issue 1362 · python/mypy](https://github.com/python/mypy/issues/1362)

    As a workaround, you could try defining your own alias to the property decorator that is annotated to return Any. If you use your custom property decorator (that at runtime behaves exactly like property) for all decorated properties, mypy will silently give all such properties the Any type.




## `[2018-12-11]` use `Protocol` for classes which I can't control, they are very neat!      [[python]] [[mypy]] [[habit]]




## `[2021-02-11]` [TypeVar to represent a Callable's arguments (for decorators/wrappers)](https://github.com/python/mypy/issues/3028)

    PEP 612 (https://www.python.org/dev/peps/pep-0612/) ended up providing a similar feature. I think we can close this issue now.




## `[2019-04-16]` mypy overloads      [[mypy]]

    @overload
    def fetch_data(raw: Literal[True]) -> bytes: ...
    @overload
    def fetch_data(raw: Literal[False]) -> str: ...
    # Fallback overload if the user provides a regular bool




## `[2019-12-07]` Still alive? · Issue 25 · machinalis/mypy-data <https://github.com/machinalis/mypy-data/issues/25>      [[numpy]]




# \* other type checking tools      [[types]]

Overall everything I've seen (pyre/pydantic) seems to target large codebases.  
They might make sense for huge monorepos, but if you need to cooperate between many libraries (my usecase) they aren't useful. So I don't know much about them.  




## `[2020-03-12]` [pydantic](https://pydantic-docs.helpmanual.io/)

    If validation fails pydantic will raise an error with a breakdown of what was wrong:
    from pydantic import ValidationError
    
    try:
        User(signup_ts='broken', friends=[1, 2, 'not number'])
    except ValidationError as e:
        print(e.json())




## `[2020-03-22]` MonkeyType: A system for Python that automatically generates type annotations | Hacker News <https://news.ycombinator.com/item?id=22624845>

    Check out mypy with "--no-any-expression" flag and Pydantic.




# `[2019-09-16]` [typeddjango/awesome-python-typing: Collection of awesome Python types, stubs, plugins, and tools to work with them.](https://github.com/typeddjango/awesome-python-typing)




# `[2019-09-27]` [Python Negatypes • Hillel Wayne](https://www.hillelwayne.com/post/negatypes)      [[types]]




# `[2020-10-03]` tried this <https://github.com/predictive-analytics-lab/data-science-types> seems to give many false positives&#x2026;      [[pandas]] [[mypy]]




# <https://github.com/wemake-services/wemake-python-styleguide/blob/master/styles/mypy.toml>       [[mypy]]




# `[2019-12-30]` [Show HN: FastAPI: build Python APIs with Go-like speed and automatic UI docs | Hacker News](https://news.ycombinator.com/item?id=19441195)

    To use Python type hints, and get automatic data validation, serialization, and documentation for your API (including interactive UI docs for your API). All that, even for deeply nested JSON bodies. And by using type hints, you get autocomplete everywhere, type error checks, etc.
    Your API gets documented with standards: OpenAPI and JSON Schema.
    Or to be able to have WebSockets.
    Or for its dependency injection system, that saves you a lot of code and plugins.
    You can check the features here: https://fastapi.tiangolo.com/features/
    And you can see alternatives and comparisons here: https://fastapi.tiangolo.com/alternatives/




## `[2020-03-01]` ok, nice, so it uses mypy types, not custom types (like hug?)




# stricter mypy flags

    --strict                  Strict mode; enables the following flags:
    
    --warn-unused-ignores
    --warn-redundant-casts
    
    --warn-unused-configs
    --disallow-subclassing-any
    --disallow-any-generics
    --disallow-untyped-calls
    --disallow-untyped-defs
    --disallow-incomplete-defs
    --check-untyped-defs
    --disallow-untyped-decorators
    --no-implicit-optional
    --warn-return-any

-   `[2021-03-08]` frankly it never stuck to me to use any of these except &#x2013;check-untyped-defs




# hmm, seems like fastapi always has to be wrapped in pydantic. ugh!

run with uvicorn fa:app &#x2013;reload &#x2013;port 9090  

    from typing import NamedTuple
    from fastapi import FastAPI
    app = FastAPI()
    from dataclasses import dataclass

    @dataclass
    class X:
        a: int
        x: str
    
    @app.get("/", response_model=X)
    async def root() -> X:
        return X(a=123, x="fwef")




# PathIsh thing can be generalized to Path constructible?      [[mypy]]





## `[2019-06-28]` not sure if <span class="underline"><span class="underline">init</span></span> would do well? <https://mypy.readthedocs.io/en/latest/protocols.html>




## `[2019-08-24]` eh, so os.PathLike[str] kinda solves it, but using .pyi file for that is not really worth it




# seems like a bug in fbmessenger export (on a branch)      [[mypy]]




# ------------------------------------------------- 




# `[2021-04-05]` crazy how useful it is to have gradual typing when you're gradually hardening the program, adding error hadnling etc      [[types]]

allows to still test happy scenarious even if type checking fails  

