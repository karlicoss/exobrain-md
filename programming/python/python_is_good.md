
# Table of Contents

-   [`[2019-07-21]` hacked seaborn to display vs on pairplots](#hckdsbrntdsplyvsnprplts) 
    -   [why python is good: patching seaborn bootstrap](#whypythnsgdptchngsbrnbtstrp) 
-   [hacking logging.Logger to do basicConfig](#hcknglggnglggrtdbsccnfg) 
    -   [`[2019-09-17]` could publish in r/python?](#cldpblshnrpythn) 
    -   [`[2019-09-17]` sometimes it makes sense for your library to configure other loggers (e.g. requests)](#smtmstmkssnsfryrlbrrytcnfgrthrlggrsgrqsts) 
-   [why generators are good: fbchat export example](#whygnrtrsrgdfbchtxprtxmpl) 
-   [another example of cool generator use in fbchat](#nthrxmplfclgnrtrsnfbcht) 
-   [example of hacky setup<sub>logger</sub>](#xmplfhckystplggr) 
-   [hacky 'autonaming'](#hckytnmng) 
-   [why mypy is good: injector DI library](#whymypysgdnjctrdlbrry) [[toblog]] [[mypy]]
-   [Why python is good](#whypythnsgd) [[toblog]]
-   [Literal types and demonstrate mypy? Perhaps timezones as example?](#ltrltypsnddmnstrtmypyprhpstmznssxmpl) [[toblog]] [[mypy]] [[configs]]
-   [By highlighting this i will know what patterns to look for in other languages](#byhghlghtngthswllknwwhtpttrnstlkfrnthrlnggs) [[toblog]]





# `[2019-07-21]` hacked seaborn to display vs on pairplots

used inspect to extract directly from local variables, lol  
<https://github.com/mwaskom/seaborn/blob/master/seaborn/axisgrid.py#L1340-L1341>  




## why python is good: patching seaborn bootstrap

I've had nondeterministic behaviour due to random seed  
was not propagated, but with a patch it's possible to achieve  

<https://github.com/mwaskom/seaborn/blob/065d3c1ed58b029d61913cca8fc315cc985ffc91/seaborn/regression.py#L235>  

    # TODO careful.. need to do this ONCE
    bootstrap_orig = sns.algorithms.bootstrap
    def bootstrap_hacked(*args, **kwargs):
        return bootstrap_orig(*args, random_seed=0, **kwargs)
    sns.algorithms.bootstrap = bootstrap_hacked

<https://github.com/mwaskom/seaborn/issues/1924>  




# hacking logging.Logger to do basicConfig

    logging.basicConfig(
        format='%(asctime)s %(levelname)-8s %(message)s',
        level=logging.INFO,
        datefmt='%Y-%m-%d %H:%M:%S')

However if you are a well-mannered person, you don't want to mess with other loggers and you're probably providing your own logger method  

This is a bit horrible  
<https://stackoverflow.com/a/28330410/706389>  

For my personal projects I'm using logzero which has got a single line setup method. However, for code I'm sharing with other people I prefer to have as little external dependencies as you can  

e.g. libraries should never configure logging  
<https://www.reddit.com/r/learnpython/comments/69grzn/logging_confuses_me/dh6ngvo/>  




## `[2019-09-17]` could publish in r/python?




## `[2019-09-17]` sometimes it makes sense for your library to configure other loggers (e.g. requests)




# why generators are good: fbchat export example

separating network retrieval and storing in database. with generators can do it simultaneously  




# another example of cool generator use in fbchat

    mts = int(r.timestamp)
    if newest is not None and oldest is not None and newest > mts > oldest:
        logger.info('Fetched everything for %s', thread.name)
        break # interrupt, thus interrupting fetching data
    db.insert_message(thread, r)




# example of hacky setup<sub>logger</sub>




# hacky 'autonaming'

    import ast
    import traceback
    import inspect
    
    src = ast.parse(open(__file__).read())
    
    def find_name(lno: int):
        # TODO end_lineno is not set??
        node = None
        for x in src.body:
            if x.lineno >= lno:
                break
            node = x
        [tg] = node.targets
        return tg.id
    
    class Namer:
        @property
        def auto(self) -> str:
            stack = inspect.stack()
            fr = stack[1]
            lno = fr.lineno
            return find_name(lno)
    
    N = Namer()
    
    
    aaaa = (
        1,
        N.auto,
    )
    bbbb = (
        2,
        N.auto,
    )
    
    print(aaaa)
    print(bbbb)




# why mypy is good: injector DI library      [[toblog]] [[mypy]]




# Why python is good      [[toblog]]

generators, decorators and random dynamic things with examples  




# Literal types and demonstrate mypy? Perhaps timezones as example?      [[toblog]] [[mypy]] [[configs]]




# By highlighting this i will know what patterns to look for in other languages      [[toblog]]

