
# Table of Contents

-   [standard library](#stndrdlbrry) 
    -   [very inconsistent naming](#vryncnsstntnmng) 
        -   [hmm how to arrange it with 'documentation' section?](#hmmhwtrrngtwthdcmnttnsctn) 
        -   [`[2021-01-25]` to be fair to Elisp, I'm finding clojure suffering from the same problem](#tbfrtlspmfndngcljrsffrngfrmthsmprblm) [[clojure]] [[lisp]]
    -   [list manipulation routines are bad](#lstmnpltnrtnsrbd) 
        -   [`cadr` `cdar` `cadddr` &#x2013; what the fuck.](#cdrcdrcdddrwhtthfck) 
        -   [`[2021-01-25]` the short answer is to use `dash.el`](#thshrtnswrstsdshl) 
    -   [string manipulation is bad](#strngmnpltnsbd) 
        -   [`[2021-01-25]` the short answer is to use s.el](#thshrtnswrstssl) 
    -   [error handling is bad](#rrrhndlngsbd) 
    -   [`[2020-02-27]` regexps are case sensitive](#rgxpsrcssnstv) 
        -   [`[2021-01-25]` on the other hand, in a way it's nice that it's easily customizable without having to think too hard about APIs](#nththrhndnwytsncthttsslycmzblwththvngtthnkthrdbtps) 
    -   [why elisp sucks: no `check_output` / `check_call`](#whylspscksnchcktptchckcll) [[elisp]]
-   [documentation](#dcmnttn) 
-   [no types](#ntyps) 
    -   [sort of hard to express&#x2026; but basically](#srtfhrdtxprssbtbsclly) 
-   [extra links](#xtrlnks) 
    -   [`[2019-10-18]` EmacsWiki: Why Does Elisp Suck](#swwwmcswkrgmcswhydslspsckmcswkwhydslspsck) 
-   [--------------------------------------------](#9766_9853) 
-   [defaul error reporting sucks](#dflrrrrprtngscks) [[elisp]]
-   [`[2019-12-26]` Fuck Elisp, issue 20191226](#stwttrcmkrlcsssttsfcklspss) 
-   [Actually if lisp is so extensible and you can do anything home come I can't write my emacs config in Python??](#ctllyflspssxtnsblndycndnyhmcmcntwrtmymcscnfgnpythn) [[lisp]]
-   [`[2019-10-20]` Output Functions - GNU Emacs Lisp Reference Manual](#tptfnctnsgnmcslsprfrncmnl) [[elisp]] [[lisp]]
-   [why elisp sucks:  buffer-size](#whylspscksbffrsz) [[elisp]]
-   [`[2021-01-16]` gnu.org/software/emacs/manual/html<sub>node</sub>/eintr/else.html](#swwwgnrgsftwrmcsmnlhtmlndftwrmcsmnlhtmlndntrlshtml) [[elisp]]
-   [`[2019-12-26]` Do you have any resources to read? I've been genuinely looking for 'modern elisp' guides, but failed to find anything decent, quite opposite, people opposing use of dash/s/etc.](#stwttrcmkrlcsssttsdyhvnyrcntqtppstpplppsngsfdshstc) 
-   [`[2019-12-26]` Also, I had to read reasonable amount of elisp (org-mode mostly, but other packages as well), and I really fail to see features you mentioned in use. Very often it's verbose car/cdr mess lacking abstractions and basic code reuse.](#stwttrcmkrlcsssttslshdtrdmsslckngbstrctnsndbsccdrs) 
-   [--------------------------------------------](#13599_13688) 
-   [`[2019-12-26]` I appreciate eshell/monkey patching/edebug, but that doesn't really strike me as **that** good. I mean, most modern interpreted languages have this, unless I'm missing on something?](#stwttrcmkrlcsssttspprctshggshvthsnlssmmssngnsmthng) 
-   [things common to lisp in general (mostly paren based stuff?)](#thngscmmntlspngnrlmstlyprnbsdstff) [[lisp]]
    -   [awkward indentation apparently aids parinfer in placing parens, however sometimes it results in code errors without noticing](#wkwrdndnttnpprntlydsprnfrtmstrsltsncdrrrswthtntcng) 
    -   [why lisp sucks: reliance on tabulation (e.g. if you change let to let\* <span class="underline">everything</span> shifts)](#whylspscksrlncntbltngfychnglttltvrythngshfts) 
    -   [why style sucks: comments after )))) (on last line). too many git changes when you add one line](#whystylsckscmmntsftrnlstlntmnygtchngswhnyddnln) 
    -   [lisp: discourages intermediate variables](#lspdscrgsntrmdtvrbls) 
-   [good parts](#gdprts) 
    -   [good: parinfer sometimes is quite nice](#gdprnfrsmtmssqtnc) [[elisp]]
    -   [good parts](#gdprts) [[elisp]] [[toblog]]
    -   [good things: hacking on the config while loading stuff via eval-defun](#gdthngshckngnthcnfgwhlldngstffvvldfn) [[elisp]]
    -   [why elisp is good: eshell, easy to mess with IDE](#whylspsgdshllsytmsswthd) [[elisp]]
    -   [appreciation why is something good is hard, you don't notice it as easy as bad things](#pprctnwhyssmthnggdshrdydntntctssysbdthngs) 
-   [Write a post comparing what elisp/common lisp offers and compare to python](#wrtpstcmprngwhtlspcmmnlspffrsndcmprtpythn) [[toblog]] [[python]] [[lisp]] [[elisp]]
-   ["How do we kill Elisp?"](#hwdwklllsp) [[elisp]] [[toblog]]
-   [when I paste stuff  from org-mode source to experiment, I often end up with ruined code (as in, broken code!)](#whnpststfffrmrgmdsrctxprmntftnndpwthrndcdsnbrkncd) 
-   [debugging: very often it's much easier to copy over the function and use output debug](#dbggngvryftntsmchsrtcpyvrthfnctnndstptdbg) [[elisp]]
-   [try finding out how to take nth character of a string](#tryfndngthwttknthchrctrfstrng) [[elisp_sucks]]
-   [`[2021-02-06]` elisp - How to determine if the current character is a letter - Emacs Stack Exchange](#smcsstckxchngcmqstnshwtdtntchrctrslttrmcsstckxchng) [[elisp_sucks]]
-   [I haven't written proper Elisp libraries/packages, only hacks/function/etc, so apologise I am missing out on some important aspects](#hvntwrttnprprlsplbrrspckgplgsmmssngtnsmmprtntspcts) [[elisp]]
-   [Structure as problem&#x2013; solution](#strctrsprblmsltn) 
-   [problem with car and cdr is not that they are the standard building blocks, but that they are abused](#prblmwthcrndcdrsntthtthyrdrdbldngblcksbtthtthyrbsd) [[elisp]]

Emacs is often praised for Elisp, which is presented as some sort of silver bullet and magical tool that solves everything.  
In my opinion, this raises the expectations too high, and then you end up disappointed when you struggle to do very simple things (and you even end up having impostor thoughts).  
Emacs is possibly the most malleable environment out there, I use it all the time and enjoy hacking it, however I like the result, not the process. I often feel that I have to do it despite Elisp.  

The purpose of this not is not just to rant, but  

-   share annoyances and point people at ways of coping with them
-   share clues for people familiar with other languages (like python/js)
-   hopefully if many people have the same problems, we can even improve Elisp language or certain default behaviours

`[2019-10-19]` [how it started](https://twitter.com/karlicoss/status/1185607527460937729)  

    I just started writing down reasons why elisp sucks every time I'm frustrated, so I can let off the steam instead of shitposting and ranting. It might actually result into something useful.

Some of my context.  

-   I'm familiar with many programming languages, paradigms and programming language theory  
    (not bragging or anything, I just think it makes it easier to discuss if we refer to the concepts we are all familiar with)
-   most days, I write Python  
    -   TODO link on python-is-good
-   I've spent a fair bit of time hacking on my emacs config and scripts for building the blog, etc, so I feel like I might be in the top percentile of Emacs users who engage with lisps
-   Elisp is the first actual Lisp I've coded on. Pretty much the only too, the other one is clojure, and only since very recently.  
    Also some things I mention are common to all lisps, but since there are many people for who Elisp is the only one they use, I hope it's valid.




# standard library

Disclaimer: different people obviously engage with different parts of standard library so YYMV.  




## very inconsistent naming

Of course naming is a hard problem, but it's not that big of an issue in some other languages:  

-   in C++/Java (OO languages), you can refer to the documentation of the objects' class, e.g. [`std::vector`](https://en.cppreference.com/w/cpp/container/vector#Member_functions)  
    granted, someone has to generate the documentation in the first place, but in the worst case you can check the class' source code/header file
-   in Python/JS you can do the same (e.g. [python's list docs](https://docs.python.org/3/tutorial/datastructures.html#more-on-lists))  
    in addition, you can use the REPL (something like `dir/vars`) to discover which methods/properties the object has
-   Haskell is not OO, but you can use something like [Hoogle](https://hoogle.haskell.org/?hoogle=Text%20-%3E%20Text) to discover all functions that operate on a given data type

In untyped language like Elisp all bets are off, the only way to find out how to use the object are  

-   rely on the documentation (and it's a mess)
-   read the package source code to discover all the functions available, perhaps search over variable names  
    this is usually what I have to resort to, even for builtin packages like org-mode




### hmm how to arrange it with 'documentation' section?




### `[2021-01-25]` to be fair to Elisp, I'm finding clojure suffering from the same problem      [[clojure]] [[lisp]]

Although naming is better subjectively (possibly because the language is yonger), it's still a mess of untyped walls of text  

-   <https://clojure.org/api/cheatsheet>
-   <https://clojuredocs.org/quickref#sequences>

The nice thing clojure docs have are the community provided examples  

I hope this is a constructive thing I (or someone else) can borrow from Clojure for Elisp.  




## list manipulation routines are bad

This is very important because dealing with list-like structures is a massive part of any programming.  




### `cadr` `cdar` `cadddr` &#x2013; what the fuck.

it's beautiful that matter is made out of atoms  
it's not great if you have to think about individual atoms to move your fingers  




### `[2021-01-25]` the short answer is to use `dash.el`

I mean, simply compare [its reference](https://github.com/magnars/dash.el#functions) with the [mess](https://www.gnu.org/software/emacs/manual/html_node/elisp/Lists.html) the builtin documentation is.  




## string manipulation is bad

Similarly, something we have to deal with all the time, and **especially** in a text editor.  




### `[2021-01-25]` the short answer is to use s.el




## error handling is bad

And again, a very important part of programming &#x2013; how to make your programs behave predictably under any circumstances?  

-   `[2020-04-12]` [another excellent piece of standard elisp library: What happens if a connection error/HTTP error happens? Who the fuck knows 🤷 pic.twitter.com/ksR3C41VXk](https://twitter.com/karlicoss/status/1249271137105838084)  
    -   `[2020-04-12]` [Spoiler: it actually dumps HTTP headers in the buffer and you're meant to parse them manually I guess. Of course, often no one bothers and assumes it's succeded](https://twitter.com/karlicoss/status/1249271166335946753)  
        -   `[2020-04-12]` [Of course there are decent and modern requests-like libraries for elisp. I just want to raise awareness that standard elisp library is garbage and we should throw it away to stay sane.](https://twitter.com/karlicoss/status/1249271524076531713)




## `[2020-02-27]` regexps are case sensitive

<https://www.reddit.com/r/emacs/comments/5jip0g/strange_replaceregexpinstring_behavior/>  

    So, if you want case sensitive, do
    (let ((case-fold-search nil))
         (replace-regexp-in-string "my" "your" "mycat.txt" t t)
    )

fucking hell.. regexes in elisp are case sensitive, and that's controlled by a fucking variable. jesus  




### `[2021-01-25]` on the other hand, in a way it's nice that it's easily customizable without having to think too hard about APIs

as long as the author extracted the variable in defvar, it's hackable  




## why elisp sucks: no `check_output` / `check_call`      [[elisp]]

<https://github.com/karlicoss/subprocess.el/blob/master/subprocess.el>  




# documentation 

-   `[2020-02-27]` [Elisp docs feel really, really bad. Hard to pinpoint what exactly, but often the descriptions are vague, repetitive, and include random and not very relevant trivia pic.twitter.com/aXhYWidKLP](https://twitter.com/karlicoss/status/1232976150856642560)

-   `[2019-11-22]` [I'm constantly seeing people praising emacs/elisp for its great documentation, however all my anecdotal evidence so far suggests the opposite  shell-command-to-string:     "Execute shell command COMMAND and return its output as a string."](https://twitter.com/karlicoss/status/1197984586082508800)  
    -   `[2019-11-22]` [ok documentation is **sort of** there, BUT &#x2026;. sweet jesus pic.twitter.com/lrywbopRe7](https://twitter.com/karlicoss/status/1197986577194070016)  
        -   `[2019-11-22]` [Output in messages buffer at least. Although it happily ignores exit code too, so discarding stderr would be even more consistent (as wrong as it sounds)](https://twitter.com/karlicoss/status/1197990100925394944)

Somehow I almost never manage to figure out (or at least much left often comparing to other PLs).  
Thankfully, in emacs you can use `find-function` and just read the source code, it's often easier.  




# no types

for the context, I don't mean strict/static types or whatever. I just want something like optional gradual typing, like #mypy  

-   yes, elisp is very dynamic and it's kind of futile (and often counterproductive) to annotate everything with types  
    but some things are clearly typeable  
    
    -   nullable string (`?string` in JS flow)
    -   list of 'things' (.e.g. `any[]` in typescript)
    -   side effect only function (`None` return type in mypy)
    
    As a result of missing types, this has to be repeated in the documentation, in vague human language.

-   yes, in elisp it's often easier to just inspect the object in question (e.g. in repl or the debugger) instead of thinking of it in terms of types
-   yes, you can add type checking (clojure things?), but I've never really seen it done except for `defcustom`




## sort of hard to express&#x2026; but basically

maybe it's just org-mode thing since this is the only 'big' elisp system I worked with  
example with org-element-set/adopt in exobrain source code  
if it was language with 'real' types, it would be easy to dir() or somethign to see what methods are available  
but maybe it would be less flexible, I dunno  
on the other hands it means that you can always hack it **somehow** and then maybe figure out 'proper'  
but discoverability really suffers  




# extra links





## `[2019-10-18]` [EmacsWiki: Why Does Elisp Suck](https://www.emacswiki.org/emacs/WhyDoesElispSuck)




# -------------------------------------------- 




# defaul error reporting sucks      [[elisp]]

e.g. try making a typo here. by default it dumps a single message with absolutely no context whatsoever (file/line number)  

    (advice-add #'org-org-section         :befoire #'exobrain/before-org-org-section)

stacktrace is pretty useful too  




# `[2019-12-26]` [Fuck Elisp, issue 20191226](https://twitter.com/karlicoss/status/1210252416479838208)

-   fuck poor standard library and need for cl-lib  
    "buffers are a better abstraction than strings"?  
    <https://twitter.com/zeRusski/status/1210254995628707840>  
    -   hmm okay this has a point, I have to think about it.  
        I guess it's true to some extent, but sometimes I do want to manipulate strings to make the code more pure

-   fuck lack of proper lexical binding  
    file-local variable  
    also not sure what was the last time it bothered me&#x2026; maybe some deafults changed?
-   fuck lack of currying  
    currying : dash.el `it` things, also partial/rpartial  
    kind of cool actually that it's implemented xxx (on the other hand would be possible in python too? with a special object or something)
-   fuck parentheses (admit this one is subjective)  
    multiple types of parens makes it much better (like in clojure)  
    but unlikely it's something solvable within elisp




# Actually if lisp is so extensible and you can do anything home come I can't write my emacs config in Python??      [[lisp]]




# `[2019-10-20]` Output Functions - GNU Emacs Lisp Reference Manual      [[elisp]] [[lisp]]

<https://www.gnu.org/software/emacs/manual/html_node/elisp/Output-Functions.html#Output-Functions>  

    why lisp sucks




# why elisp sucks:  buffer-size      [[elisp]]

doesn't take an argument so need with-current-buffer  

<https://www.gnu.org/software/emacs/manual/html_node/eintr/Buffer-Size-_0026-Locations.html>  

can't jump to source code because it's in C?  

whereas buffer-filename takes optional argument  
<https://www.gnu.org/software/emacs/manual/html_node/elisp/Buffer-File-Name.html>  




# `[2021-01-16]` [gnu.org/software/emacs/manual/html<sub>node</sub>/eintr/else.html](https://www.gnu.org/software/emacs/manual/html_node/eintr/else.html)      [[elisp]]

    Note that the different levels of indentation make it easy to distinguish the then-part from the else-part.

ugh, this is bullshit. how the fuck is this makes it easier.  
e.g. if you swap if and else clauses, indentation changes  




# `[2019-12-26]` [Do you have any resources to read? I've been genuinely looking for 'modern elisp' guides, but failed to find anything decent, quite opposite, people opposing use of dash/s/etc.](https://twitter.com/karlicoss/status/1210287560649584642)




# `[2019-12-26]` [Also, I had to read reasonable amount of elisp (org-mode mostly, but other packages as well), and I really fail to see features you mentioned in use. Very often it's verbose car/cdr mess lacking abstractions and basic code reuse.](https://twitter.com/karlicoss/status/1210288518637006849)

-   `[2019-12-26]` [Admit though that it may have to do with people rather than language (kinda like people misusing c++).](https://twitter.com/karlicoss/status/1210288820081565696) :tweet:




# -------------------------------------------- 




# `[2019-12-26]` [I appreciate eshell/monkey patching/edebug, but that doesn't really strike me as **that** good. I mean, most modern interpreted languages have this, unless I'm missing on something?](https://twitter.com/karlicoss/status/1210287248467517440)




# things common to lisp in general (mostly paren based stuff?)      [[lisp]]





## awkward indentation apparently aids parinfer in placing parens, however sometimes it results in code errors without noticing




## why lisp sucks: reliance on tabulation (e.g. if you change let to let\* <span class="underline">everything</span> shifts)




## why style sucks: comments after )))) (on last line). too many git changes when you add one line




## lisp: discourages intermediate variables

let bindings struct is <span class="underline">really</span> annoying, which discourages naming variables  

    собственно мотивационный пример на питоне
    
    def normalize(vec):
       x, y = vec
       len = sqrt(x ** 2 + y ** 2)
       if len == 0:
           raise RuntimeError(f'bad vector {vec}')
    
       nx = x / len
       ny = y / len
       return (nx, ny)
    
    на елиспе
    
    (defun normalize (vec)
      (let* ((x   (car vec))
             (y   (cdr vec)))
             (len (sqrt (* x x) (* y y))))
        (if (=0 len)
            (error (format "bad vector %s" vec)))
        (let* ((nx (/ x len))
               (ny (/ y len)))
          `(,nx ,ny)))
    
    а я хочу как-то так
    
    (defun normalize (vec)
      (let' (x y) vec) ;; can't do in elisp?? maybe with cl-destructuring-bind...
      (let' len   (sqrt (* x x) (* y y)))
      (if (= 0 len)
          (error (format "bad vector %s" vec))
      (let' nx (/ x len)
            ny (/ y len))
      `(,nx ,ny)))
    
    наверное это можно добиться если добавить какую-нибудь магию вроде макроса (scope ...), который эти let' правильно интерпретирует




# good parts





## good: parinfer sometimes is quite nice      [[elisp]]

sometimes though it arbitrarily reararnges parens. e..g I have to be <span class="underline">really</span> careful when pasting big source blocks from elsewhere  




## good parts      [[elisp]] [[toblog]]

advice-patch  




## good things: hacking on the config while loading stuff via eval-defun      [[elisp]]

i.e. I think people who advocate for REPL are pitching for a completely wrong thing &#x2013; I want to keep my code tidy, it's just nice to execute it instantly  




## why elisp is good: eshell, easy to mess with IDE      [[elisp]]

to be fair, same is probably true for e.g. sublime?  




## appreciation why is something good is hard, you don't notice it as easy as bad things

let's compare: e.g. vimscript. When I used vim I haven't even attempted to customize it, I tried once and the whole thing was just futile.  




# Write a post comparing what elisp/common lisp offers and compare to python      [[toblog]] [[python]] [[lisp]] [[elisp]]




# "How do we kill Elisp?"      [[elisp]] [[toblog]]




# when I paste stuff  from org-mode source to experiment, I often end up with ruined code (as in, broken code!)

example: (defun org-html-format-headline-default-function  
maybe I need to disable parinfer during pasting, not sure  




# debugging: very often it's much easier to copy over the function and use output debug      [[elisp]]

also use with-current-buffer and a separate buffer &#x2013; oftern much easier than repl&#x2026;  




# try finding out how to take nth character of a string      [[elisp_sucks]]




# `[2021-02-06]` [elisp - How to determine if the current character is a letter - Emacs Stack Exchange](https://emacs.stackexchange.com/questions/8261/how-to-determine-if-the-current-character-is-a-letter)      [[elisp_sucks]]

    n case you were very concerned about national characters and precise treatment of Unicode character classes, then the only solution I was able to find so far is the Python regex library. Both grep and Perl (to my utter surprise!) didn't do the job properly.




# I haven't written proper Elisp libraries/packages, only hacks/function/etc, so apologise I am missing out on some important aspects      [[elisp]]




# Structure as problem&#x2013; solution

E.g. bad docs? Enjoy easy jump-to-source  




# problem with car and cdr is not that they are the standard building blocks, but that they are abused      [[elisp]]

in the same vein consistently using `head . tail . tail` in Haskell to access the third element would be insane (I'm not sure if it's actually common though)  

