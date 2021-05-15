
# Table of Contents

-   [Propositional equality](#prpstnlqlty) 
-   [Natural numbers](#ntrlnmbrs) 
-   [Finite type](#fnttyp) 
-   [`[2019-08-12]` YOW! Lambda Jam 2019 - Philip Wadler: (Programming Languages) in Agda = Programming (Languages in Agda) /r/functionalprogramming](#srddtcmrfnctnlprgrmmngcmmnglnggsngdrfnctnlprgrmmng) [[towatch]] [[agda]]
-   [`[2018-10-10]` Agda Beginner(-ish) Tips, Tricks, & Pitfalls - Donnacha Oisín Kidney](#gdbgnnrshtpstrcksptfllsdnnchsínkdny) [[agda]]
-   [A Few Haskell Highlights: Top Haskell Resources of 2019](#fwhskllhghlghtstphskllrsrcsf) [[agda]]
-   [`[2019-04-21]` Cubical Agda and Probability Monads /r/agda](#srddtcmrgdcmmntsbjjrcbclgndscbclgdndprbbltymndsrgd) [[agda]]
-   [`[2018-11-13]` good with explanation https://agda.readthedocs.io/en/latest/language/with-abstraction.html#simultaneous-abstraction](#gdwthxplntnsgdrdthdcsnltshbstrctnhtmlsmltnsbstrctn) [[agda]]
-   [https://math.stackexchange.com/a/1307770/15108 prove isomorphism?](#smthstckxchngcmprvsmrphsm) [[tostudy]] [[agda]]
-   [Philip Wadler and Wen Kokke publish book on Programming Language Foundations in Agda](#phlpwdlrndwnkkkpblshbknprgrmmnglnggfndtnsngd) 
-   [Tweet from Denis Moskvin (@deniok), at Apr 12, 17:20](#twtfrmdnsmskvndnktpr) [[agda]]
-   [Agda stuff](#gdstff) 
    -   [`[2018-11-11]` agda/Records.agda at master · agda/agda](#gdrcrdsgdtmstrgdgd) 
    -   [`[2018-11-11]` agda/Sigma.agda at master · agda/agda](#gdsgmgdtmstrgdgd) 
    -   [`[2018-11-13]` Abstract Algebra in Agda](#bstrctlgbrngd) 
    -   [`[2018-11-13]` With-Abstraction — Agda 2.6.0 documentation](#wthbstrctngddcmnttn) 
-   [`[2019-01-26]` agda-ring-solver https://oisdk.github.io/agda-ring-solver/README.html](#gdrngslvrssdkgthbgdrngslvrrdmhtml) 

  




# Propositional equality

    data _≡_ {A : Set} : A → A → Set where
      refl : {a : A} → a ≡ a
    
    sym : ∀ {A} {a b : A} → a ≡ b -> b ≡ a
    sym refl = refl




# Natural numbers

    data ℕ : Set where
      Z : ℕ
      S : ℕ → ℕ




# Finite type

    data Fin : ℕ → Set where
      fzero : (n : ℕ) -> Fin (S n)
      fsucc : (n : ℕ) -> Fin n -> Fin (S n)
    
    onlyone : (x : Fin (S Z)) → x ≡ fzero Z
    onlyone (fzero .Z) = refl
    onlyone (fsucc .Z ())




# `[2019-08-12]` [YOW! Lambda Jam 2019 - Philip Wadler: (Programming Languages) in Agda = Programming (Languages in Agda)](https://reddit.com/r/functionalprogramming/comments/cnplr3/yow_lambda_jam_2019_philip_wadler_programming/) /r/functionalprogramming      [[towatch]] [[agda]]




# `[2018-10-10]` Agda Beginner(-ish) Tips, Tricks, & Pitfalls - Donnacha Oisín Kidney      [[agda]]

<https://doisinkidney.com/posts/2018-09-20-agda-tips.html>  




# A Few Haskell Highlights: Top Haskell Resources of 2019      [[agda]]

    To get to know Agda better, you can read this introductory post by Danya Rogozin.




# `[2019-04-21]` [Cubical Agda and Probability Monads](https://reddit.com/r/agda/comments/bej1jr/cubical_agda_and_probability_monads/) /r/agda      [[agda]]




# `[2018-11-13]` good with explanation <https://agda.readthedocs.io/en/latest/language/with-abstraction.html#simultaneous-abstraction>      [[agda]]

tldr: write multiple with clauses; then pattern match on them to rewrite and eliminate  




# <https://math.stackexchange.com/a/1307770/15108> prove isomorphism?      [[tostudy]] [[agda]]




# Philip Wadler and Wen Kokke publish book on Programming Language Foundations in Agda

<https://www.reddit.com/r/haskell/comments/a2d3pg/_/eax3ml7?context=1000>  




# Tweet from Denis Moskvin (@deniok), at Apr 12, 17:20      [[agda]]

    В Агдочку Prop'ов завезли! https://t.co/1s98uSyGd8

<https://twitter.com/deniok/status/1116737917421064192>  




# Agda stuff





## `[2018-11-11]` agda/Records.agda at master · agda/agda

<https://github.com/agda/agda/blob/master/examples/SummerSchool07/Lecture/Records.agda>  




## `[2018-11-11]` agda/Sigma.agda at master · agda/agda

<https://github.com/agda/agda/blob/master/src/data/lib/prim/Agda/Builtin/Sigma.agda>  




## `[2018-11-13]` Abstract Algebra in Agda

<https://people.inf.elte.hu/pgj/agda/tutorial/Application.Algebra.html>  




## `[2018-11-13]` With-Abstraction — Agda 2.6.0 documentation

<https://agda.readthedocs.io/en/latest/language/with-abstraction.html#simultaneous-abstraction>  




# `[2019-01-26]` agda-ring-solver <https://oisdk.github.io/agda-ring-solver/README.html>

