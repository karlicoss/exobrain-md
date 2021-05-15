
# Table of Contents

-   [`[2016-08-07]` .](#40_150) 
-   [`[2015-06-20]` Do notation expanded](#dnttnxpndd) 
-   [monads](#mnds) [[monad]]
    -   [writer monad, logger monad](#wrtrmndlggrmnd) 
    -   [reader monad](#rdrmnd) 
    -   [state monad](#sttmnd) 
-   [`[2015-06-20]` monad transformers](#mndtrnsfrmrs) [[monad]]
-   [related](#rltd) [[fp]]
-   [Tweet from Dmitry Kovanikov (@ChShersh), at Jun 1, 04:37](#twtfrmdmtrykvnkvchshrshtjn) [[haskell]]
-   [`[2018-10-23]` krispo/awesome-haskell: A collection of awesome Haskell links, frameworks, libraries and software. Inspired by awesome projects line.](#krspwsmhskllcllctnfwsmhskndsftwrnsprdbywsmprjctsln) [[haskell]]
-   [`[2018-11-24]` debug: what I learnt during setting app hakyll blog..](#dbgwhtlrntdrngsttngpphkyllblg) 
-   [`[2019-01-06]` Resilient-Haskell-Software - Gwern.net](#rslnthskllsftwrgwrnnt) [[haskell]]
-   [`[2019-02-11]` Stackage Server https://www.stackage.org/](#stckgsrvrswwwstckgrg) 
-   [`[2019-04-14]` debugging ghci](#dbggngghc) 
-   [`[2019-01-05]` debug: stack trace](#dbgstcktrc) 
-   [`[2019-01-25]` Henry de Valence on Twitter: "7 years ago i was very smart and wrote my website in haskell and now i can't update it because i forgot how to make a monad out of posts" / Twitter](#hnrydvlncntwttryrsgwsvryscsfrgthwtmkmndtfpststwttr) [[haskell]] [[fun]]
-   [`[2016-02-28]` applicative functors](#pplctvfnctrs) [[haskell]]
-   [`[2016-02-28]` monad vs applicative](#mndvspplctv) [[haskell]]





# `[2016-08-07]` .

ihaskell install  
jupyter console &#x2013;kernel haskell  




# `[2015-06-20]` Do notation expanded

    do e → e
    do { e; stmts } → e >> do { stmts }
    do { v <- e; stmts } → e >>= \v -> do { stmts }
    do { let decls; stmts} → let decls in do { stmts }

This is not quite the whole story, since v might be a pattern instead of a variable. For example, one can write  

do (x:xs) <- foo  
   bar x  
but what happens if foo produces an empty list? Well, remember that ugly fail function in the Monad type class declaration? That’s what happens.  




# monads       [[monad]]





## writer monad, logger monad

    -- l: log type, Monoid
    newtype Writer l a = Writer {
        runWriter :: (a, l)
    }




## reader monad

    newtype Reader r a = Reader {
        runReader :: r -> a
    }




## state monad

    newtype State s a = State {
        runState :: s -> (a, s)
    }




# `[2015-06-20]` monad transformers      [[monad]]

Monad transformers exist only because monads do not compose in general.  
MaybeT : provides the construction for (f of Maybe) for any Monad f.  

    data Compose f g x = Compose (f (g x))
    
    instance (Functor f, Functor g) => Functor (Compose f g) where
          fmap f (Compose z) = Compose (fmap (fmap f) z)
    
    instance (Monad f, Monad g) => Monad (Compose f g) where
          bind :: Compose f g a -> (a -> Compose f g b) -> Compose f g b
          bind (f (g x)) ff =
          bind = ???
          no way!
    
    f a -> (a -> f b) -> f b
    g c -> (c -> g d) -> g d




# related       [[fp]]




# Tweet from Dmitry Kovanikov (@ChShersh), at Jun 1, 04:37      [[haskell]]

    Looks like @iokasimov can write good #haskell jokes 😏

<https://twitter.com/ChShersh/status/1002393643288686592>  




# `[2018-10-23]` krispo/awesome-haskell: A collection of awesome Haskell links, frameworks, libraries and software. Inspired by awesome projects line.      [[haskell]]

-   State "DONE"       from              `[2019-04-22]`

<https://github.com/krispo/awesome-haskell>   




# `[2018-11-24]` debug: what I learnt during setting app hakyll blog..

-   stack ghci
-   Debug.Trace.traceShowM within do block
-   pandoc &#x2013;metadata




# `[2019-01-06]` Resilient-Haskell-Software - Gwern.net      [[haskell]]

<https://www.gwern.net/Resilient-Haskell-Software>  




# `[2019-02-11]` Stackage Server <https://www.stackage.org/>




# `[2019-04-14]` debugging ghci

    stack ghci (module loaded automatically)
    :set args rebuild
    main
    :break 222




# `[2019-01-05]` debug: stack trace

    stack build --profile
    stack exec -- site rebuild +RTS -xc 




# `[2019-01-25]` Henry de Valence on Twitter: "7 years ago i was very smart and wrote my website in haskell and now i can't update it because i forgot how to make a monad out of posts" / Twitter      [[haskell]] [[fun]]

<https://twitter.com/hdevalence/status/1088649294746275840>  




# `[2016-02-28]` applicative functors      [[haskell]]

-   regular functor  
    
        class Functor f where
          fmap :: (a -> b) -> f a -> f b

Laws:  

    fmap id = id                                 -- Identity
    fmap (p . q) = (fmap p) . (fmap q)           -- Homomorphism

-   applicative  
    
        class (Functor f) => Applicative f where
            pure  :: a -> f a
            (<*>) :: f (a -> b) -> f a -> f b

Laws:  

    pure id <*> v = v                            -- Identity
    pure (.) <*> u <*> v <*> w = u <*> (v <*> w) -- Composition
    pure f <*> pure x = pure (f x)               -- Homomorphism
    u <*> pure y = pure ($ y) <*> u              -- Interchange
    fmap f x = pure f <*> x                      -- Fmap

The mapping between Haskell functors is a family of functions parameterized by types. For instance, a mapping between the [] functor and the Maybe functor will map a list of a, [a] into Maybe a.  
Here's an example of such a family of functions called safeHead:  

    safeHead :: [a] -> Maybe a
    safeHead []     = Nothing
    safeHead (x:xs) = Just x




# `[2016-02-28]` monad vs applicative      [[haskell]]

<https://wiki.haskell.org/Typeclassopedia#Intuition_3>  

    Let’s look more closely at the type of (>>=). The basic intuition is that it combines two computations into one larger computation. The first argument, m a, is the first computation.
    However, it would be boring if the second argument were just an m b; then there would be no way for the computations to interact with one another (actually, this is exactly the situation with Applicative).
    So, the second argument to (>>=) has type a -> m b: a function of this type, given a result of the first computation, can produce a second computation to be run.
    In other words, x >>= k is a computation which runs x, and then uses the result(s) of x to decide what computation to run second, using the output of the second computation as the result of the entire computation.

    Actually, because Haskell allows general recursion, one can recursively construct infinite grammars, and hence Applicative (together with Alternative) is enough to parse any context-sensitive language with a finite alphabet.

<http://byorgey.wordpress.com/2012/01/05/parsing-context-sensitive-languages-with-applicative>  

    Here’s the key insight: normally, grammars are defined as finite objects: a finite set of terminals, a finite set of nonterminals, and a finite set of productions.
    However, Haskell’s general recursion means that we can write down a "grammar" with an infinite set of production rules. This is what lets us get away with parsing context-sensitive languages with Applicative: we just make a different production rule for every possible input!

