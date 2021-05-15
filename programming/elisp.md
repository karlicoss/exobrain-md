
# Table of Contents

-   [related](#rltd) [[lisp]] [[emacs]]
-   [\* lists manipulation](#lstsmnpltn) 
    -   [use `dash.el`](#sdshl) 
    -   [`append '(a b c) '(d e f)` to concat](#ppndbcdftcnct) 
-   [\* string manipulation](#strngmnpltn) 
    -   [`[2019-09-05]` magnars/s.el: The long lost Emacs string manipulation library](#sgthbcmmgnrsslmgnrsslthlnglstmcsstrngmnpltnlbrry) 
-   [\* debugging](#dbggng) 
    -   [`[2018-10-13]` `(message (buffer-string))`](#mssgbffrstrng) 
-   [\* code style](#cdstyl) 
    -   [defclass?](#dfclss) 
    -   [:type slot; trivial-types lib?](#typslttrvltypslb) 
-   [`[2018-06-18]` sharp-quote names of functions `(mapcar #'fun list)`](#shrpqtnmsffnctnsmpcrfnlst) 
-   [`[2018-04-24]` elisp basics](#lspbscs) 
-   [`[2020-02-02]` /r/emacs: (Almost) All You Need to Know About Variables](#rmcssrddtcmrmcscmmntsxnxhknwbtlmstllyndtknwbtvrbls) 
-   [`[2021-01-06]` unwind-protect works as with / try-finally block](#nwndprtctwrksswthtryfnllyblck) [[python]] [[elisp]]
-   [lisp unpacking like in python  ``(let ((x '(2 3))) `(1 ,@x 4 5))``](#lspnpcknglknpythnltxx) [[drill]] [[python]]
-   [----------------------------------------](#2514_2598) 
-   [`[2019-07-24]` /r/emacs: Tutorial on Good Lisp Programming Style](#rmcssrddtcmrmcscmmntschfvtylttrlngdlspprgrmmngstyl) 
-   [`[2020-12-13]` More batteries included with emacs | Karthinks regexes in elisp](#skrthnkscmsftwrmrbttrsnclclddwthmcskrthnksrgxsnlsp) 
-   [`[2021-01-02]` Wilfred/ht.el: The missing hash table library for Emacs](#sgthbcmwlfrdhtlwlfrdhtlthmssnghshtbllbrryfrmcs) 
-   [`[2020-02-16]` Changing Properties - GNU Emacs Lisp Reference Manual https://www.gnu.org/software/emacs/manual/html\_node/elisp/Changing-Properties.html](#chngngprprtsgnmcslsprfrnchtmlndlspchngngprprtshtml) 
-   [`[2019-09-20]` How to Locate the Variable I Need? : orgmode](#hwtlctthvrblndrgmd) [[toblog]] [[org]] [[elisp]]
-   [mention defvar vs setq](#mntndfvrvsstq) [[emacs]]
-   [`[2020-02-15]` Emacs Should Be Emacs Lisp - Tom Tromey https://braindump.jethro.dev/talks/emacs\_should\_be\_emacs\_lisp/](#mcsshldbmcslsptmtrmysbrndpjthrdvtlksmcsshldbmcslsp) [[elisp]]
-   [`[2020-02-16]` What's the performance · Issue #19 · alphapapa/org-ql https://github.com/alphapapa/org-ql/issues/19](#whtsthprfrmncsslphpprgqlsgthbcmlphpprgqlsss) 
-   [`[2020-02-16]` What's the performance · Issue #19 · alphapapa/org-ql https://github.com/alphapapa/org-ql/issues/19](#whtsthprfrmncsslphpprgqlsgthbcmlphpprgqlsss) 
-   [`[2020-02-24]` bbatsov/emacs-lisp-style-guide: A community-driven Emacs Lisp style guide](#bbtsvmcslspstylgdcmmntydrvnmcslspstylgd) [[elisp]]
-   [`[2021-02-09]` (8) Writing A Spotify Client in 16 Minutes - YouTube](#swwwytbcmwtchvxjktkmygclsndxwrtngsptfyclntnmntsytb) [[elisp]]





# related       [[lisp]] [[emacs]]




# \* lists manipulation





## use `dash.el`




## `append '(a b c) '(d e f)` to concat




# \* string manipulation





## `[2019-09-05]` [magnars/s.el: The long lost Emacs string manipulation library](https://github.com/magnars/s.el)

much saner and more consisten than builtins  




# \* debugging





## `[2018-10-13]` `(message (buffer-string))`




# \* code style

<http://lisp-lang.org/style-guide/>  

-   variable naming  
    
    -   `*earmuff*` style for mutable globals?
    
    but:  
    
    -   dynamic variables have a prefix
    -   local variables (or anything set with a let) do not have a prefix

-   prefer `when cond` to `if cond ...`, prefer `unless cond` to `if (not cond)`

-   predicates  
    end with `p` or `-p`
-   doesn't have namespaces. `package--private-function` `package-public-function`




## defclass? 




## :type slot; trivial-types lib?




# `[2018-06-18]` sharp-quote names of functions `(mapcar #'fun list)`




# `[2018-04-24]` elisp basics

cursor point region <http://ergoemacs.org/emacs/elisp_cursor_position.html>  
<http://ergoemacs.org/emacs/elisp_editing_basics.html>  

<http://ergoemacs.org/emacs/elisp_optional_params.html>  

    &optional prams.
    &rest remaining params

no named params, no type checking..  

thing-at-point  




# `[2020-02-02]` /r/emacs: [(Almost) All You Need to Know About Variables](https://reddit.com/r/emacs/comments/exnxha/withemacs_almost_all_you_need_to_know_about/)




# `[2021-01-06]` unwind-protect works as with / try-finally block      [[python]] [[elisp]]




# lisp unpacking like in python  ``(let ((x '(2 3))) `(1 ,@x 4 5))``      [[drill]] [[python]]




# ---------------------------------------- 




# `[2019-07-24]` /r/emacs: [Tutorial on Good Lisp Programming Style](https://reddit.com/r/emacs/comments/chfv7y/tutorial_on_good_lisp_programming_style/)




# `[2020-12-13]` [More batteries included with emacs | Karthinks](https://karthinks.com/software/more-batteries-included-with-emacs/) regexes in elisp

    A cleaner approach to regular expressions in Emacs, as most package maintainers will tell you, is to use the rx library instead. rx translates regular expressions in sexp form to a regexp string:




# `[2021-01-02]` [Wilfred/ht.el: The missing hash table library for Emacs](https://github.com/Wilfred/ht.el)




# `[2020-02-16]` Changing Properties - GNU Emacs Lisp Reference Manual <https://www.gnu.org/software/emacs/manual/html_node/elisp/Changing-Properties.html>

    Function: add-text-properties start end props &optional object
    This function adds or overrides text properties for the text between start and end in the string or buffer object. If object is nil, it defaults to the current buffer.

jesus  




# `[2019-09-20]` How to Locate the Variable I Need? : orgmode      [[toblog]] [[org]] [[elisp]]

<https://www.reddit.com/r/orgmode/comments/d6wzkr/how_to_locate_the_variable_i_need/>  

    The way I deal with these things: if it's not immediately searchable on stackoverlow, I wouldn't bother doing web search.
    My thinking would be:
    Ok, what builting org function could possibly use number of stars? Right, when I promote/demote the subtree it must be using that at some point.

small tutorial for hacking on emacs?  




# mention defvar vs setq      [[emacs]]




# `[2020-02-15]` Emacs Should Be Emacs Lisp - Tom Tromey <https://braindump.jethro.dev/talks/emacs_should_be_emacs_lisp/>      [[elisp]]




# `[2020-02-16]` What's the performance · Issue #19 · alphapapa/org-ql <https://github.com/alphapapa/org-ql/issues/19>

    Yes, it's generally slower because it checks every heading with predicates. The tradeoff is that the code is more composable and understandable than the 5-screens-long functions in org-agenda.el. Even so, for a lot of use cases, it's fast enough already. There is already a per-buffer, per-query cache that makes performance fast on repeated queries in unchanged buffers, which helps a lot.




# `[2020-02-16]` What's the performance · Issue #19 · alphapapa/org-ql <https://github.com/alphapapa/org-ql/issues/19>

        One cool trick that elfeed implements is JIT-compilation of search queries. If you call a function in a map or a loop or something similar this makes a difference.
    Yeah, I learned that trick from Chris's code. Both the "predicate" function and "action" function are byte-compiled before running the "query".




# `[2020-02-24]` bbatsov/emacs-lisp-style-guide: A community-driven Emacs Lisp style guide      [[elisp]]

<https://github.com/bbatsov/emacs-lisp-style-guide>  




# `[2021-02-09]` [(8) Writing A Spotify Client in 16 Minutes - YouTube](https://www.youtube.com/watch?v=XjKtkEMUYGc&list=WL&index=63)      [[elisp]]

I mean.. ok, but nothing super remarkable idk?  
should do a similar demo in python, for example  

