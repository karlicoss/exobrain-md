
# Table of Contents

-   [hmm that looks pretty similar&#x2026; https://math.stackexchange.com/a/1792315/15108](#hmmthtlksprttysmlrsmthstckxchngcm) 
-   [Visualisations for SU2, manually entangling loops](#vslstnsfrsmnllyntnglnglps) [[think]]
    -   [hmm. sample random loops and then try to contract them?](#hmmsmplrndmlpsndthntrytcntrctthm) 
-   [`[2019-02-01]` my initial notes](#myntlnts) 
    -   [how to define manifolds? parametric? works for Rn Sn and Tn](#hwtdfnmnfldsprmtrcwrksfrrnsnndtn) 
    -   [somehow use van kampen's theorem?](#smhwsvnkmpnsthrm) 
    -   [`[2019-02-01]` mm. ok this ended up a bit different from what I imagined initially. still though, maybe contracting loops manually is ok, people are better at that?](#mmkthsnddpbtdffrntfrmwhtmtnglpsmnllyskpplrbttrttht) 
    -   [`[2019-02-02]` hmm. if you consider a torus, composed of two triangles, looks like all vertices are labeled in the same](#hmmfycnsdrtrscmpsdftwtrnglslkslkllvrtcsrlbldnthsm) 
-   [`[2019-02-01]` initial python impl in file:projects/fund/main.py](#ntlpythnmplnflprjctsfndmnpy) 
-   [name it 'mental' (for fundamental) instead of topology? or pione??](#nmtmntlfrfndmntlnstdftplgyrpn) 
-   [related](#rltd) [[topology]] [[viz]]
-   [`[2019-02-01]` SnapPea - Wikipedia](#snppwkpd) [[autopology]]
-   [`[2019-02-10]` Dynamical triangulation of the 2-torus - YouTube](#dynmcltrngltnfthtrsytb) [[qg]] [[autopology]]
-   [`[2019-05-10]` Keep it Simplex, Stupid! |   Bartosz Milewski's Programming Cafe](#kptsmplxstpdbrtszmlwsksprgrmmngcf) [[autopology]]
-   [summary on trying to understand triangulated fundamental group](#smmryntryngtndrstndtrngltdfndmntlgrp) [[topology]] [[autopology]]
    -   [https://math.stackexchange.com/questions/1778421/fundamental-group-of-the-sphere-via-triangulation](#smthstckxchngcmqstnsfndmntlgrpfthsphrvtrngltn) [[autopology]]
    -   [http://homepage.divms.uiowa.edu/~jsimon/COURSES/M201Fall08/HandoutsAndHomework/Graph1.pdf](#hmpgdvmswdjsmncrssmfllhndtsndhmwrkgrphpdf) 
    -   [klein bottle (with triangulation) https://math.stackexchange.com/questions/1778465/fundamental-group-klein-bottle-triangulation](#klnbttlwthtrngltnsmthstcksfndmntlgrpklnbttltrngltn) 
    -   [edge-path https://en.wikipedia.org/wiki/Fundamental\_group#Edge-path\_group\_of\_a\_simplicial\_complex](#dgpthsnwkpdrgwkfndmntlgrpdgpthgrpfsmplclcmplx) 
    -   [faces in triangulation must be distinct](#fcsntrngltnmstbdstnct) 
    -   [make sure you don't have loop in spanning tree](#mksrydnthvlpnspnnngtr) 
    -   [fun fact: computing fundamental group is undecidable https://mathoverflow.net/a/304484/29889 (in terms of figuring out whether it's trivial)](#fnfctcmptngfndmntlgrpsndcntntrmsffgrngtwhthrtstrvl) 
        -   [encode turing machines via topological spaces? lol](#ncdtrngmchnsvtplgclspcsll) 
    -   [https://math.stackexchange.com/questions/1666146/fundamental-group-from-triangulation#comment3399175\_1666146](#smthstckxchngcmqstnsfndmntlgrpfrmtrngltncmmnt) 
    -   [basically, I don't understand what all they mean by subcomplex. why do they color all of it???](#bscllydntndrstndwhtllthymnbysbcmplxwhydthyclrllft) 
    -   [book by Armstrong, p. 134. Don't really understand the statement, it's all very vague](#bkbyrmstrngpdntrllyndrstndthsttmnttsllvryvg) 
    -   [torus &#x2013; here they mention there are quite a lot of relations&#x2026;](#trshrthymntnthrrqtltfrltns) 
-   [`[2019-02-10]` at.algebraic topology - Algorithm for computing fundamental group of simplicial complexes - MathOverflow](#tlgbrctplgylgrthmfrcmptnglgrpfsmplclcmplxsmthvrflw) 
-   [`[2019-02-10]` at.algebraic topology - Algorithm for computing fundamental group of simplicial complexes - MathOverflow](#tlgbrctplgylgrthmfrcmptnglgrpfsmplclcmplxsmthvrflw) 

<https://en.wikipedia.org/wiki/Computational_topology>  
<https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D0%BC%D0%BF%D0%BB%D0%B8%D1%86%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B9_%D0%BA%D0%BE%D0%BC%D0%BF%D0%BB%D0%B5%D0%BA%D1%81>  

<http://graphics.stanford.edu/courses/cs468-09-fall/>  
hmm wonder if that does it. they mention triangulation.  

<https://en.wikipedia.org/wiki/Triangulation_(topology)>    
<https://en.wikipedia.org/wiki/Digital_manifold>  




# hmm that looks pretty similar&#x2026; <https://math.stackexchange.com/a/1792315/15108>




# Visualisations for SU2, manually entangling loops      [[think]]

Approximate them by segments, that should work  




## hmm. sample random loops and then try to contract them?




# `[2019-02-01]` my initial notes

Triangulate the manifold  
then do some sort of random walk and stop at the initial point with some probability  
then, do some sort of simulated annealing to transform the loops according to the certain rules.  
basically, we can contract certain subpaths (or expand?) e.g. a -> b -> a can be contracted to a. unless the points are glued?  
try to guess groups from equivalence classes? then try combining them and guessing against known groups?  

to contract, define some sort of 'tension' function? not sure if makes sense  

this is a conservative method in the sense that it can answer what your fundamental group is NOT  
in a sense, fundamental group is a conservative concept too, it can answer what your topological space is NOT  

triangulation, or squares?  

if the point or edge is glued, treat it as special?  




## how to define manifolds? parametric? works for Rn Sn and Tn




## somehow use van kampen's theorem?




## `[2019-02-01]` mm. ok this ended up a bit different from what I imagined initially. still though, maybe contracting loops manually is ok, people are better at that?

basically you declare some of the loops as 'trivial', but manually  




## `[2019-02-02]` hmm. if you consider a torus, composed of two triangles, looks like all vertices are labeled in the same

however, that's not enough to classify, we should be considering edges instead?  




# `[2019-02-01]` initial python impl in <projects/fund/main.py>

pretty inefficient, should rewrite in rust for finer control. also, make multithreaded  




# name it 'mental' (for fundamental) instead of topology? or pione??




# related       [[topology]] [[viz]]




# `[2019-02-01]` SnapPea - Wikipedia      [[autopology]]

<https://en.wikipedia.org/wiki/SnapPea>  




# `[2019-02-10]` Dynamical triangulation of the 2-torus - YouTube      [[qg]] [[autopology]]

<https://www.youtube.com/watch?v=c3NdgSIe030>  




# `[2019-05-10]` Keep it Simplex, Stupid! |   Bartosz Milewski's Programming Cafe      [[autopology]]

<https://bartoszmilewski.com/2018/12/11/keep-it-simplex-stupid/>  




# summary on trying to understand triangulated fundamental group      [[topology]] [[autopology]]

-   State "START"      from              `[2019-02-21]`




## <https://math.stackexchange.com/questions/1778421/fundamental-group-of-the-sphere-via-triangulation>       [[autopology]]

FG for the sphere  




## <http://homepage.divms.uiowa.edu/~jsimon/COURSES/M201Fall08/HandoutsAndHomework/Graph1.pdf> 

most useful so far.. the idea is you construct spanning tree, choose a base point and assign all loops from base point to 1 (for each edge not in the maximal tree). does that work for higher dimensions??  




## klein bottle (with triangulation) <https://math.stackexchange.com/questions/1778465/fundamental-group-klein-bottle-triangulation>




## edge-path <https://en.wikipedia.org/wiki/Fundamental_group#Edge-path_group_of_a_simplicial_complex>




## faces in triangulation must be distinct

<https://math.stackexchange.com/a/1772664/15108>  
<https://math.stackexchange.com/a/954164/15108>  




## make sure you don't have loop in spanning tree

<https://math.stackexchange.com/a/1778957/15108>  




## fun fact: computing fundamental group is undecidable <https://mathoverflow.net/a/304484/29889> (in terms of figuring out whether it's trivial)





### encode turing machines via topological spaces? lol




## <https://math.stackexchange.com/questions/1666146/fundamental-group-from-triangulation#comment3399175_1666146> 

look at remaining  




## basically, I don't understand what all they mean by subcomplex. why do they color all of it???

<https://math.stackexchange.com/questions/2472310/finding-fundamental-group-of-simplicial-complexes>  




## book by Armstrong, p. 134. Don't really understand the statement, it's all very vague




## torus &#x2013; here they mention there are quite a lot of relations&#x2026;

<https://books.google.co.uk/books?id=xwzX9h_hyMUC&pg=PA202&lpg=PA202&dq=%22fundamental+group%22+triangulation+spanning+tree&source=bl&ots=m9NZ4m5lP4&sig=ACfU3U0epWUJDPHbx_RBUiq6uoTL6Zhj6Q&hl=en&sa=X&ved=2ahUKEwjhqcrXr7HgAhXwIjQIHbVmD10Q6AEwBXoECAkQAQ#v=onepage&q=%22fundamental%20group%22%20triangulation%20spanning%20tree&f=false>  
book: simplicial structure by ferrario, p.202  
right, apparently to compute really effeciently we need van kampen theorem..  




# `[2019-02-10]` at.algebraic topology - Algorithm for computing fundamental group of simplicial complexes - MathOverflow

<https://mathoverflow.net/questions/304481/algorithm-for-computing-fundamental-group-of-simplicial-complexes>  

    Kruskal's algorithm will give you a maximal tree, and after that the presentation just involves listing the remaining edges as generators, and listing the relations that come from the 2-simplices. I don't really see anything interesting going on algorithmically once you've selected a maximal tree.




# `[2019-02-10]` at.algebraic topology - Algorithm for computing fundamental group of simplicial complexes - MathOverflow

<https://mathoverflow.net/questions/304481/algorithm-for-computing-fundamental-group-of-simplicial-complexes>  

    Depends on what you mean by "computing" and "algorithm". It is undecidable (even for a two-complex) whether the fundamental group is trivial, though computing a presentation is relatively easy.

