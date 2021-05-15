
# Table of Contents

-   [testing](#tstng) [[testing]]
    -   [nose is abandoned](#nssbndnd) 
    -   [pytest is the best apparently](#pytststhbstpprntly) [[pytest]]
-   [logging](#lggng) 
    -   [simple](#smpl) 
    -   [use `logzero` for nice colored logs](#slgzrfrncclrdlgs) 
-   [json](#jsn) [[json]]
    -   [`json.dump(jobj, stdout, indent=4, sort_keys=True, ensure_ascii=False)`](#jsndmpjbjstdtndntsrtkystrnsrscfls) 
-   [asyncio](#sync) 
-   [`[2020-02-12]` Guido van Rossum on Twitter: "@jonasrk You missed mypy. Simpler docs use markdown, not ReST (Sphinx). Black is overrated unless your team argues over style a lot. You don't need Pylint if you're using flake8. Never heard of poetry or dependabot. And you should use a CI solution, e.g. Travis-CI, to run your tests." / Twitter https://twitter.com/gvanrossum/status/1227126706089021440](#gdvnrssmntwttrjnsrkymssdmstwttrstwttrcmgvnrssmstts) 
-   [`[2018-05-08]` configuration via class variables &#x2013; not great while testing since configuration has to be reloaded&#x2026;](#cnfgrtnvclssvrblsntgrtwhltstngsnccnfgrtnhstbrldd) 
-   [write about setting up elaborate python project + circleci? maybe demonstrate on grasp?](#wrtbtsttngplbrtpythnprjctcrclcmybdmnstrtngrsp) [[ci]]





# testing       [[testing]]





## nose is abandoned




## pytest is the best apparently      [[pytest]]

-   uses the built in `assert`  
    
        assert 1 == 1, 'This is my error message, which is optional'
-   parameterized tests
-   fixtures: These aren't the setup/teardown fixtures (per-se), but more like dependency injection (and are incredibly useful). You can even inject a fixture into a fixture (say you need to log in a user, but you need an HTTP client for it to work, you probably use that client elsewhere so DRY it up):
-   markers: Easy way to categorize tests (and coincidentally run only those groups)  
    
        @pytest.mark.slow
        def test_slow_running_thing():
            time.sleep(500)
-   parallel execution via xdist




# logging 





## simple 

    import logging
    logging.basicConfig(level=logging.INFO) # apparently callin basicconfig at least one is important
    logging.exception('Caught an error' + str(e))




## use `logzero` for nice colored logs




# json       [[json]]





## `json.dump(jobj, stdout, indent=4, sort_keys=True, ensure_ascii=False)`




# asyncio 




# `[2020-02-12]` Guido van Rossum on Twitter: "@jonasrk You missed mypy. Simpler docs use markdown, not ReST (Sphinx). Black is overrated unless your team argues over style a lot. You don't need Pylint if you're using flake8. Never heard of poetry or dependabot. And you should use a CI solution, e.g. Travis-CI, to run your tests." / Twitter <https://twitter.com/gvanrossum/status/1227126706089021440>

    You don't need Pylint if you're using flake8

hmm  




# `[2018-05-08]` configuration via class variables &#x2013; not great while testing since configuration has to be reloaded&#x2026;




# write about setting up elaborate python project + circleci? maybe demonstrate on grasp?      [[ci]]

