
# Table of Contents

-   [`[2018-11-10]` ok, trying to break down this thing http://math.mit.edu/~cohn/Thoughts/symplectic.html](#ktryngtbrkdwnthsthngmthmtdchnthghtssymplctchtml) 
    -   [`[2018-11-18]`](#5127_5633) 
        -   [fuck, I don't really understand the closedness thing and it might actually be crutial. maybe, later&#x2026;](#fckdntrllyndrstndthclsdnsngndtmghtctllybcrtlmybltr) 
-   [`[2018-11-16]`  Topics in Representation Theory: Hamiltonian Mechanics and Symplectic Geometry](#tpcsnrprsnttnthryhmltnnmchncsndsymplctcgmtry) 
    -   [print it!&#x2026;](#prntt) 
    -   [looks like really good paper&#x2026; read more from it (or references?)](#lkslkrllygdpprrdmrfrmtrrfrncs) 
-   [`[2018-11-17]` Terence Tao: Phase Space](#trnctphsspc) 
-   [momentum vs velocity](#mmntmvsvlcty) 
    -   [https://physics.stackexchange.com/questions/213991/why-specify-the-state-of-a-particle-in-terms-of-position-and-momentum-not-veloci](#sphyscsstckxchngcmqstnswhtclntrmsfpstnndmmntmntvlc) 
        -   [tl;dr: In classical mechanics, specifying a particle's state in terms of momentum is equivalent to specifying it in terms of velocity, but the specification in terms of momenta often has computational advantages.](#tldrnclssclmchncsspcfyngpmsfmmntftnhscmpttnldvntgs) 
        -   [Quantum mechanics does not have well-defined trajectories q(t), so the notion of a velocity does not make sense. On the contrary, the momentum operator can still be defined as relating to the position operator in the same way as in Hamiltonian mechanics, by replacing the classical Poisson bracket by the quantum commutator of operators.](#qntmmchncsdsnthvwlldfndtrbrcktbythqntmcmmttrfprtrs) 
    -   [hmm, so velocities (q') are just additional 'data' which happens to be related via q = q'(t). initially, you don't have to treat it as derivative.](#hmmsvlctsqrjstddtnldtwhchqqtntllyydnthvttrttsdrvtv) 
-   [that's pretty interesting https://physics.stackexchange.com/questions/123725/what-kind-of-manifold-can-be-the-phase-space-of-a-hamiltonian-system](#thtsprttyntrstngsphyscsstldcnbthphsspcfhmltnnsystm) 
-   [equations of motion are dx/dt = {x, H} and dp/dt = {p, H} &#x2013; hmm, that's interesting&#x2026;](#qtnsfmtnrdxdtxhnddpdtphhmmthtsntrstng) 
-   [https://www.quora.com/What-is-the-significance-of-a-symplectic-manifold](#swwwqrcmwhtsthsgnfcncfsymplctcmnfld) 
    -   [I believe the significance for physics boils down to the following: it turns out that a two-form is precisely what is required to translate an energy functional on phase space (a Hamiltonian) into a flow (a vector field).](#blvthsgnfcncfrphyscsblsdwnphsspchmltnnntflwvctrfld) 
    -   [mmm&#x2026;](#mmm) 
-   [something interesting about the fact that not all symplectic forms can be exact (if the space is not T\*Q for some Q)](#smthngntrstngbtthfctthtntrmscnbxctfthspcsnttqfrsmq) 
-   [where to put it?](#whrtptt) 
-   [some graphical intuition about covectors&#x2026; http://www.physicsinsights.org/pbp\_one\_forms.html](#smgrphclnttnbtcvctrswwwphyscsnsghtsrgpbpnfrmshtml) 
-   [`[2018-11-10]`  digression: [Goldberg] A Little Tase of Symplectic Geometry.pdf &#x2013; very cool!!!](#dgrssngldbrglttltsfsymplctcgmtrypdfvrycl) 
-   [something interesting about basis of tangent vectors?&#x2026; https://math.stackexchange.com/a/454663/15108 v &isin; T<sub>p</sub> M = v<sup>i</sup> &delta;<sub>i</sub>?](#smthngntrstngbtbssftngntvssmthstckxchngcmvntpmvdlt) 
-   [hmm, why are alternating forms important? https://en.wikipedia.org/wiki/Multilinear\_form#Alternating\_multilinear\_forms](#hmmwhyrltrntngfrmsmprtntsltlnrfrmltrntngmltlnrfrms) 
-   ['[Powell] Aspects of Symplectic Geometry in Physics.pdf'](#pwllspctsfsymplctcgmtrynphyscspdf) 
-   [something about symplectomorphisms&#x2026;](#smthngbtsymplctmrphsms) 
-   [`[2018-11-18]` ok, I should implement some simple phase space portrait plotting first](#kshldmplmntsmsmplphsspcprtrtplttngfrst) 
-   [`[2018-11-21]`  understood A LOT while waiting for Metric concert!](#ndrstdltwhlwtngfrmtrccncrt) 
    -   [https://en.wikipedia.org/wiki/Hamiltonian\_mechanics#Deriving\_Hamilton's\_equations](#snwkpdrgwkhmltnnmchncsdrvnghmltnsqtns) 
        -   [mnemonic : p then q (dp/dt = dH/dq)](#mnmncpthnqdpdtdhdq) 
        -   [In fact, as is shown below, the Hamiltonian is the Legendre transform of the Lagrangian when holding q and t fixed and defining p as the dual variable, and thus both approaches give the same equations for the same generalized momentum. The main motivation to use Hamiltonian mechanics instead of Lagrangian mechanics comes from the symplectic structure of Hamiltonian systems.](#nfctssshwnblwthhmltnnsthlmplctcstrctrfhmltnnsystms) 
        -   [Hamilton's equation easily derived by looking at the total differential of Lagrangian on time](#hmltnsqtnslydrvdbylkngtthttldffrntlflgrngnntm) 
        -   [generalised coordinates: just any coordinates that (injectively??) map onto system configuration](#gnrlsdcrdntsjstnycrdntsthtnjctvlympntsystmcnfgrtn) 
        -   [Since this calculation was done off-shell, one can associate corresponding terms from both sides of this equation to yield:](#sncthsclcltnwsdnffshllncngtrmsfrmbthsdsfthsqtntyld) 
        -   [](#16360_17167) 
        -   [If the transformation equations defining the generalized coordinates are independent of t, and the Lagrangian is a sum of products of functions (in the generalized coordinates) which are homogeneous of order 0, 1 or 2, then it can be shown that H is equal to the total energy E = T + V.](#fthtrnsfrmtnqtnsdfnngthgnnbshwnththsqltthttlnrgytv) 
        -   [The solutions to the Hamilton–Jacobi equations for this Hamiltonian are then the same as the geodesics on the manifold. In particular, the Hamiltonian flow in this case is the same thing as the geodesic flow. The existence of such solutions, and the completeness of the set of solutions, are discussed in detail in the article on geodesics. See also Geodesics as Hamiltonian flows.](#thsltnstthhmltnjcbqtnsfrtngdscsslsgdscsshmltnnflws) 
    -   [https://ru.wikipedia.org/wiki/%D0%93%D0%B0%D0%BC%D0%B8%D0%BB%D1%8C%D1%82%D0%BE%D0%BD%D0%BE%D0%B2%D0%B0\_%D0%BC%D0%B5%D1%85%D0%B0%D0%BD%D0%B8%D0%BA%D0%B0](#srwkpdrgwkddbdbcdbdbbdcddbddbdbdbdbcdbddbdbddbdbdb) 
        -   [В полярных координатах обобщённый импульс, соответствующий угловой скорости, — физический угловой момент. Для произвольного выбора обобщённых координат трудно получить интуитивную интерпретацию сопряжённых этим координатам импульсов или угадать их выражение, не используя прямо приведённую выше формулу.](#вполярныхкоординатахобобщямоприведённуювышеформулу) 
        -   [Отсюда, в частности, следует, что если какая-то координата оказалась циклической, то есть если функция Лагранжа от неё не зависит, а зависит только от её производной по времени, то для сопряжённого ей импульса {\displaystyle {\dot {p}}=0} {\dot  {p}}=0, то есть он является интегралом движения (сохраняется во времени), что несколько проясняет смысл обобщённых импульсов.](#отсюдавчастностиследуетчттсмыслобобщённыхимпульсов) 
        -   [Любая гладкая функция {\displaystyle H: M&rarr; \mathbb {R} } H: M&rarr; \mathbb{R}  на симплектическом многообразии {\displaystyle M} M может использоваться, чтобы определить гамильтонову систему. Функция {\displaystyle H} H известна как гамильтониан или энергетическая функция. Симплектическое многообразие называют фазовым пространством. Гамильтониан порождает специальное векторное поле на симплектическом многообразии, известном как симплектическое векторное поле.](#любаягладкаяфункцияdsplysплектическоевекторноеполе) 
        -   [Симплектическое векторное поле (также называется гамильтоновым векторным полем) порождает гамильтонов поток на многообразии. Интегральные кривые векторного поля являются однопараметрическим семейством преобразований многообразия с параметром, называемым время. Эволюция во времени задаётся симплектоморфизмами. Из теоремы Лиувилля следует, что каждый симплектоморфизм сохраняет форму объёма в фазовом пространстве. Множество симплектоморфизмов, порождаемых гамильтоновым потоком, обычно называют гамильтоновой механикой гамильтоновой системы.](#симплектическоевекторноепникойгамильтоновойсистемы) 
        -   [Гамильтоново векторное поле также порождает специальную операцию — скобка Пуассона. Скобка Пуассона действует на функции на симплектическом многообразии, таким образом придавая пространству функций на многообразии структуру алгебры Ли.](#гамильтонововекторноеполеобразииструктуруалгебрыли) 
    -   [phase: from any point on phase space, evolution is unique. it's kinda like initial data for a differential equation](#phsfrmnypntnphsspcvltnsnqtskndlkntldtfrdffrntlqtn) 
-   [`[2018-11-20]` why symplectic spaces?](#whysymplctcspcs) 
    -   [now figure out why is that interesting. lol](#nwfgrtwhysthtntrstngll) 
-   [`[2018-11-10]` intuition - What is a symplectic form intuitively? - MathOverflow](#nttnwhtssymplctcfrmnttvlymthvrflw) 
-   [Hamiltonian vector field - Wikipedia](#hmltnnvctrfldwkpd) 
-   [Tweet from John Carlos Baez (@johncarlosbaez), at Nov 22, 22:01](#twtfrmjhncrlsbzjhncrlsbztnv) 
-   [Legendre transformation - Wikipedia](#lgndrtrnsfrmtnwkpd) 
-   [`[2018-11-10]` What moment map is (as a physical concept) in sympletic geometry - Mathematics Stack Exchange](#whtmmntmpssphysclcncptnsypltcgmtrymthmtcsstckxchng) 
-   [`[2018-11-10]` classical mechanics - Intuition about Momentum Maps - Physics Stack Exchange](#clssclmchncsnttnbtmmntmmpsphyscsstckxchng) 
-   [`[2018-11-14]` sg.symplectic geometry - How to see the Phase Space of a Physical System as the Cotangent Bundle - MathOverflow](#sgsymplctcgmtryhwtsthphssystmsthctngntbndlmthvrflw) 
-   [`[2018-11-19]` Legendre transformation - Wikipedia](#lgndrtrnsfrmtnwkpd) 
-   [`[2018-11-18]` Symplectic integrator - Wikipedia](#symplctcntgrtrwkpd) 
-   [`[2018-11-19]` mathematical physics - Is there an analogue of configuration space in quantum mechanics? - Physics Stack Exchange](#mthmtclphyscssthrnnlgfcnfqntmmchncsphyscsstckxchng) 
-   [`[2018-11-18]` Applying Runge-Kutta method to circular - C++ Forum](#pplyngrngkttmthdtcrclrcfrm) 
-   [`[2018-09-13]` Chel<sub>of</sub><sub>the</sub><sub>sea</sub> comments on ELI5: What is symplectic geometry?](#chlfthscmmntsnlwhtssymplctcgmtry) 
-   [`[2018-08-13]` poisson brackets are related to symplectic geometry (explains phase space)](#pssnbrcktsrrltdtsymplctcgmtryxplnsphsspc) 
-   [`[2018-08-13]` poisson brackets explained](#pssnbrcktsxplnd) 
    -   [`[2019-06-12]` need to add this to drill..](#ndtddthstdrll) 
-   [`[2018-11-15]`](#27192_28438) 
    -   [Spivak's Physics For Mathematicians,](#spvksphyscsfrmthmtcns) 
    -   [configuration space: M (a Manifold). Phase space: cotangent bundle over M (T<sub>\*</sub> M). Also a manifold?? Yeah, ok T<sub>\*</sub> M is also a manifold with dimension twise as what M got.](#cnfgrtnspcmmnfldphsspcctnlsmnfldwthdmnsntwsswhtmgt) 
    -   [right, and symplectic form is defined on the contagent bundle of configuration space! (or on a phase space?)](#rghtndsymplctcfrmsdfndnthntbndlfcnfgrtnspcrnphsspc) 
-   [learn basic QED and QFT](#lrnbscqdndqft) [[study]] [[qed]]
    -   [Feynman QED strange theory of light](#fynmnqdstrngthryflght) 
        -   [feynman diagrams are way of computing quantum amplitude. sum over all diagrams](#fynmndgrmsrwyfcmptngqntmmpltdsmvrlldgrms) 
        -   [renormalization: meh, but only theory parameters depend on it, measurable stuff is not impacted](#rnrmlztnmhbtnlythryprmtrsdpndntmsrblstffsntmpctd) 
    -   [Zee, Feynman. QED: Strange Theory of Light and Matter](#zfynmnqdstrngthryflghtndmttr) 
    -   [(long time ago) Tong, some notes in study/qft](#lngtmgtngsmntsnstdyqft) 
-   [`[2018-12-15]` symplectic geometry - Learn Anything](#symplctcgmtrylrnnythng) 
-   [`[2019-06-18]` Energy drift - Wikipedia](#nrgydrftwkpd) [[symplectic]]
-   [`[2020-01-18]` chakravala/Grassmann.jl: ⟨Leibniz-Grassmann-Clifford⟩ differential geometric algebra / multivector simplicial complex](#chkrvlgrssmnnjllbnzgrssmntrclgbrmltvctrsmplclcmplx) [[symplectic]]
-   [`[2018-11-10]` Tangent bundle - Wikipedia https://en.wikipedia.org/wiki/Tangent\_bundle](#tngntbndlwkpdsnwkpdrgwktngntbndl) [[symplectic]] [[drill]]
-   [Symplectic geometry foundations](#symplctcgmtryfndtns) 
    -   [Intro to symplectic geom](#ntrtsymplctcgm) 
-   [Tweet from John Carlos Baez (@johncarlosbaez), at Jan 21, 18:29](#twtfrmjhncrlsbzjhncrlsbztjn) [[symplectic]] [[towatch]]

`[2018-11-15]`  ok, so trying to consolidate everything  

1.  <https://sbseminar.wordpress.com/2012/01/09/what-is-a-symplectic-manifold-really/>  
    TODO how to link in org mode?? e.g. citations?

here they try to deduce phase space from some reasonable mathematical assumptions (time evolution, energy conservation, flows)  

1.  The Geometry of Hamiltonian Mechanics

So, we have a configuration space N, which is a manifold. Typically, it's the set of positions, more generally, it's the set of all possible 'snapshots' of the system at a certain time.  

(TODO how does that correspond to wavefunctions? how is position special? e.g. momentum is not any worse right?).  

Then take \(M = T^* N\) (cotangent bundle) &#x2013; it's the phase space, and itself a manifold.  

TODO twice the dimensions?  

NOTE: ugh, looks like they are confusing p and q in [1], typically q is position/state and p is monentum. So I'm using the more common notation.  

Some coordinates in M are position coordinates, some are momentum coordinates. (x<sub>q</sub>, x<sub>p</sub>). x<sub>q</sub> corresponds to N, x<sub>p</sub> corresponds to T\* N at x<sub>q</sub>?  

Ok, consider time derivative.  
Time derivative of x<sub>q</sub> is a vector   on N [1]. Note: ok, sort of makes sense.. I guess by vector they mean a point from tangent space? E.g. consider 2-sphere, time derivative is indeed a vector on that sphere.  
Time derivative of x<sub>p</sub> is a covector on N [1]. TODO: this still makes sense I guess? Not really.. I guess my confusion has to do with not understanding what's a thing from T\* N?  

digression:  
consider 1-sphere S (radius 1). Its configurations X are angles phi from 0 to 2 pi. If you consider tangent space though, it's gonna have all possible velocities from -inf to inf.  
ok. but what about cotangent space?? | TODO what does it have to do with 1-forms  
is it just the space of all {mul by v | v in (-inf, inf)}. And then what??  

so time derivative of position is a vector   on N. Agree. I guess we're using the fact that N is a manifold, thus locally it's a vector space.  
   time derivative of momentum is a covector on N. Well, that's a bit more subtle. I mean, it kinda makes sense, but it's a different space than T\*<sub>x</sub> N. Right?  

suppose we have a functional F(t): N -> R, and we want to compute its derivative. By definition, F'(t) = (F(t+dt) - F(t)) / dt. But F(x) = <f, x>. Then, F'(t) = (<f(t + dt), x> - <f(t), x>) / dt = <(f(t + dt) - f(t))/dt, x>. So, it's dual to f', which is a time derivative of a vector, thus a covector. Ugh, ok.  

Again, following [1]. Consider a function E: M -> R.  
Its differential w.r.t. space coordinates is a covector, and w.r.t momentum coordinates is a vector. well, ok  

dE/d(q,p) = (dE/dq1.. dE/dqn, dE/dp1&#x2026;de/dpn)  
Ok, I suppose you could call dE/dq a covector. why though?&#x2026; what does that mean? I guess that if we plug  

TODO shit. don't think I understand that bit really intuitively&#x2026;   but whatever  

Ok. so we established that  
    dx<sub>q</sub>/dt and dE/dx<sub>p</sub> are both vectors  
    dx<sub>p</sub>/dt and dE/dx<sub>q</sub> and both covectors.  
so that?? why the minus sign?  




# `[2018-11-10]` ok, trying to break down this thing <http://math.mit.edu/~cohn/Thoughts/symplectic.html>

the idea is to generalise phase space mechanics to abstract (not necessarily eucledian spaces)  

we want a method to turn hamiltonian function H to a vector field V, then dynamics is the flow across integral curves of this field  

requirements:  

1.  depend only on dH (global shift doesn't matter)
2.  linear dependence on dH

he claims that tensor field, a section of Hom(T\*M, TM), or Hom(TM, T\*M) = (TM -> T\*M) = T\*M tensor T\*M does that  

NOTE: vector bundle &#x2013; vector space, depending on parameter (point)  
NOTE: tensor field by definition is some section on tensor bundle. mmm.  
NOTE: vector fields on manifold &#x2013; a section of tangent bundle. Okay, sort of makes sense. although; you could have said that it's a mapping F: (x: X) -> T(x)  
NOTE: huh, so f: M -> R, df: {m: M} ->  T(M) -> R. TODO wonder if it's interesting that number of arguments is increasing?  
      in general: f: M -> N, df: TM -> TN, meaning that df: {exists m: M}  (T(m) -> T(f(m)))  
      TODO shit, I need agda here?&#x2026;  

jesus, they just don't have nice notation  

tensor field is F: (x: X) -> T(x) ; T(x) is the space of all tensors at x. and that's it!  

note from wikipedia: if f: M -> N, then df: TM -> TN  

ok, so if H: M -> R; then dH: TM -> R = T\*M  
NOTE: when we think of dH, we consider it as a section, sort of with implicit {m: M} argument.  

hmm, what is the tangent space of point on R. still R right? Yes, because it's basically space of 'velocities'  
so dH is a covector field, ok <https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D1%84%D1%84%D0%B5%D1%80%D0%B5%D0%BD%D1%86%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F_%D1%84%D0%BE%D1%80%D0%BC%D0%B0#%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B>  

so we want to turn dH: T(m) -> R into V: (m: M) -> T(m)  

to do that, for every point m, we need a way to map dH<sub>m</sub> into T(m). dH<sub>m</sub>: (T(m) -> R)  

U\* x V = Hom(U, V) = U -> V  

process : (T(m) -> R) -> T(m) =  




## `[2018-11-18]` 

ok, use conservation of energy  
that means that Hamiltonian is constant along the flow. for any H: dH(V<sub>H</sub>) = 0, hence w(V<sub>H</sub>, V<sub>H</sub>) = 0. For every V, we can find its H, s.t. V<sub>H</sub> = V, so w(V, V) = 0 for all V? so the form is alternating  

TODO non-degeneracy?  




### fuck, I don't really understand the closedness thing and it might actually be crutial. maybe, later&#x2026;




# `[2018-11-16]`  Topics in Representation Theory: Hamiltonian Mechanics and Symplectic Geometry

 good point on first page: a more obvious set of equations is gradient flow:  
dp<sub>i</sub>/dt = -df/dp<sub>i</sub>  
dq<sub>i</sub>/dt = -df/dq<sub>i</sub>  

it's a flow along a vector field &nabla;<sub>f</sub>, which comes from: taking -df (1-form); then using inner product on R<sup>2n</sup> to dualise and get a vector field from 1-form.  
that is:  

f -> &nabla;<sub>f</sub>: <&nabla;<sub>f</sub>, x> = -df. Ok, makes sense. We can just substitute vector fields in forms to get forms of lower rank.  

Hamilton's equations are similar, but instead the form is symplectic, not an inner product.  

Sometimes X<sub>H</sub> is called symplectic gradient.  

Flow along the            gradient of f changes f as fast as possible  
Flow along the symplectic gradient of f keeps   f constant  

since dH(X<sub>H</sub>) = -w(X<sub>H</sub>, X<sub>H</sub>) = 0  

NOTE: I guess that's natural, we want to keep energy constant along the phase space movement.  

TODO blah blah something about hamiltonian vector fields and poisson brackets  

NOTE! Right, so contangent bundle is actually just an example (!) of a symplectic manifold, with some canonical structure. Another example is Kahler manifold  

M = T\* N  
Canonical one-form theta an point (a, b) &isin; T\*n by theta<sub>(a,b)</sub>(v) = b(Proj<sub>a</sub> v)  
Then the symplectic form w = d theta  

TODO interesting that we throw away most of v's information. I guess that has to do with degeneracy??  

hmm, <https://en.wikipedia.org/wiki/Tautological_one-form>  
apparently this theta is called canonical one-form  




## print it!&#x2026;




## looks like really good paper&#x2026; read more from it (or references?)

[1] Bryant, R., An Introduction to Lie Groups and Symplectic Geometry, in  
Geometry and Quantum Field Theory, Freed, D., and Uhlenbeck, K., eds.,  
American Mathematical Society, 1995.  
[2] Guillemin, V. and Sternberg, S., Symplectic Techniques in Physics, Cam-  
bridge University Press, 1984.  




# `[2018-11-17]` Terence Tao: Phase Space

ok, so his stuff is pretty similar.  
positions q in conf space M  
momentum p: in cotangent bundle T<sub>q</sub>\* M  
phase space is the cotangent bundle T\* M  

note that velocity lies in tangent bundle T M, but momentum is defined as dL/dq', so it's in a different space  

TODO so most of time, they are kind of same things&#x2026; but not always. I guess I need a better sense of what momentum actually is.  
I guess they are same if Lagrangian depends on v'<sup>2</sup>/2. What would be some interesting and physical examples of Lagrangians where it's not the case?  

ok, he say same thing that Hamilton's equation is analogue to gradient flow for H on the manifold T\*M, but w.r.t. the symplectic form.  

NOTE gradient flow is a curve, such that: x'(t) = - \Nabla F(x(t)).  
Okay, kinda makes sense. Time evolution in the direction of steepest descent.  

TODO something about definition via observables  




# momentum vs velocity





## <https://physics.stackexchange.com/questions/213991/why-specify-the-state-of-a-particle-in-terms-of-position-and-momentum-not-veloci> 





### tl;dr: In classical mechanics, specifying a particle's state in terms of momentum is equivalent to specifying it in terms of velocity, but the specification in terms of momenta often has computational advantages.




### Quantum mechanics does not have well-defined trajectories q(t), so the notion of a velocity does not make sense. On the contrary, the momentum operator can still be defined as relating to the position operator in the same way as in Hamiltonian mechanics, by replacing the classical Poisson bracket by the quantum commutator of operators.




## hmm, so velocities (q') are just additional 'data' which happens to be related via q = q'(t). initially, you don't have to treat it as derivative.




# that's pretty interesting <https://physics.stackexchange.com/questions/123725/what-kind-of-manifold-can-be-the-phase-space-of-a-hamiltonian-system>

maybe visualise a hamiltonian on n-torus?  




# equations of motion are dx/dt = {x, H} and dp/dt = {p, H} &#x2013; hmm, that's interesting&#x2026;

<https://mathoverflow.net/a/16462/29889>  




# <https://www.quora.com/What-is-the-significance-of-a-symplectic-manifold> 





## I believe the significance for physics boils down to the following: it turns out that a two-form is precisely what is required to translate an energy functional on phase space (a Hamiltonian) into a flow (a vector field).




## mmm&#x2026; 

So in some sense, "conservation of symplectic form" is the second most basic conservation law. (The most basic is conservation of energy, which is essentially the definition o  




# something interesting about the fact that not all symplectic forms can be exact (if the space is not T\*Q for some Q)

<https://mathoverflow.net/a/16537/29889>  




# where to put it?

Following [2].  

K   = 1/2 Sum m<sub>a</sub> (v<sup>a</sup>)<sup>2</sup>  
F<sub>a</sub> = -d<sub>a</sub> V(r)  

TODO err, they define cartesian coordinates via generalised coordinates; then generalised velocities; and then rewrite K as 1/2 Sum q'<sup>i</sup> g<sub>ik</sub> q<sup>k</sup>'.  

shit, I don't really follow this :(  

lagrangian is L: T Q -> R, so defined on tangent bundle.  

Next, define the generalised momenta as p<sub>i</sub> = dL/dq'<sup>i</sup>.  
Ans, f<sub>i</sub> = dL/dq<sup>i</sup> is generalised force.  

In generalised coordinates: L(q, q') = 1/2 Sum q'<sup>i</sup> g<sub>ij</sub>(q, m) q'<sup>j</sup> - V(q)  

Components of generalised momentum: p<sub>i</sub> = dL/dq'<sup>i</sup> = Sum<sub>j</sub> g<sub>ij</sub> q'<sup>j</sup>.  

ok, that's sort of interesting  
so, if Q is Riemannian manifold (got metric), then there is a diffeomorphism T Q -> T<sup>\*</sup> Q from tangent space to cotangent space.  

metric tensor is 2-form; which means that when it acts on a vector field, we get 1-form (so momentum is 1-form)  

I don't understand why they started using kinetic and potential energy staright away.  

Ok, good point on page 23:  

-   in Lagrangian  formalism, dynamics takes place on T (T   Q)
-   in Hamiltonian formalise, dynamics takes place on T (T<sup>\*</sup> Q)
-   

on page 24:  

x'(t) = X<sub>H</sub><sub>x</sub>(t) = J dH (x); where J is the symplectic matrix; dH is gradient of hamiltonian function. Hamiltonian vector field.  

pull-backs:  

consider O: M -> T\* M &#x2013; 1-form on phase space &#x2013; ok, as a member of T\* M.  
consider a: Q -> T\* Q &#x2013; 1-form on conf  space.  

right, so a is a linear map from Q to M; and O is a 1-form on M. We can pull back O to Q to get the 1-form a\* O. | err so what??  

canonical poincare 1-form Theta = \Sum<sub>i</sub> p<sub>i</sub> dq<sup>i</sup>, which satisfies a<sup>\*</sup> Theta = a for all a in &#x2026;.  




# some graphical intuition about covectors&#x2026; <http://www.physicsinsights.org/pbp_one_forms.html>




# `[2018-11-10]`  digression: [Goldberg] A Little Tase of Symplectic Geometry.pdf &#x2013; very cool!!!




# something interesting about basis of tangent vectors?&#x2026; <https://math.stackexchange.com/a/454663/15108> v &isin; T<sub>p</sub> M = v<sup>i</sup> &delta;<sub>i</sub>?




# hmm, why are alternating forms important? <https://en.wikipedia.org/wiki/Multilinear_form#Alternating_multilinear_forms>

so they are actually what's called covectors??  




# '[Powell] Aspects of Symplectic Geometry in Physics.pdf'

Suppose \(f\) is observable. It can only depend on position, momentum and possibly time:  

\(f(p_i, q^i)\): \(\dv{f}{t} = \sum_i \pdv{f}{q^i} \dot{q}^i + \pdv{f}{p_i} {\dot p}_i = \sum_i \pdv{f}{q^i} \pdv{H}{p_i} - \pdv{f}{p_i} \pdv{H}{q_i} := \{f, H\}\)  

\(f(p_i, q^i, t)\) &#x2013; if time dependent , then \(\dv{f}{t} = \{f, H\} + \pdv{f}{t}\) &#x2013; makes sense! kinda like flow derivative from Segal  




# something about symplectomorphisms&#x2026;

any 2n-dimensional symplectic manifold looks like R<sup>2n</sup>, w<sub>0</sub>   




# `[2018-11-18]` ok, I should implement some simple phase space portrait plotting first

<https://github.com/BartoszMilewski/gravity-sim>  
haskell or rust?&#x2026; not sure  

try L = 1/2x'<sup>2</sup> + x' - 1/2 x<sup>2</sup>  

TODO what if we make linear dependency on position? That's pretty much coordinate transformation right?  
soo, if it's a linear dependency on velocity&#x2026; it's kind of time coordinate transformation!!  




# `[2018-11-21]`  understood A LOT while waiting for Metric concert!





## <https://en.wikipedia.org/wiki/Hamiltonian_mechanics#Deriving_Hamilton's_equations> 





### mnemonic : p then q (dp/dt = dH/dq)




### In fact, as is shown below, the Hamiltonian is the Legendre transform of the Lagrangian when holding q and t fixed and defining p as the dual variable, and thus both approaches give the same equations for the same generalized momentum. The main motivation to use Hamiltonian mechanics instead of Lagrangian mechanics comes from the symplectic structure of Hamiltonian systems.




### Hamilton's equation easily derived by looking at the total differential of Lagrangian on time




### generalised coordinates: just any coordinates that (injectively??) map onto system configuration




### Since this calculation was done off-shell, one can associate corresponding terms from both sides of this equation to yield:

hmm, wonder if that's kinda like dimensionality argument  




###  

In Cartesian coordinates, the generalized momenta are precisely the physical linear momenta. In circular polar coordinates, the generalized momentum corresponding to the angular velocity is the physical angular momentum. For an arbitrary choice of generalized coordinates, it may not be possible to obtain an intuitive interpretation of the conjugate momenta.  

right, that's interesting that it's not possible to obtain intuitive sense  

One thing which is not too obvious in this coordinate dependent formulation is that different generalized coordinates are really nothing more than different coordinate patches on the same symplectic manifold (see Mathematical formalism, below).  

TODO should read more on that&#x2026; what do they call coordinate patches?  




### If the transformation equations defining the generalized coordinates are independent of t, and the Lagrangian is a sum of products of functions (in the generalized coordinates) which are homogeneous of order 0, 1 or 2, then it can be shown that H is equal to the total energy E = T + V.

not sure, that might be interesting  




### The solutions to the Hamilton–Jacobi equations for this Hamiltonian are then the same as the geodesics on the manifold. In particular, the Hamiltonian flow in this case is the same thing as the geodesic flow. The existence of such solutions, and the completeness of the set of solutions, are discussed in detail in the article on geodesics. See also Geodesics as Hamiltonian flows.

<https://en.wikipedia.org/wiki/Hamiltonian_mechanics#Riemannian_manifolds>  




## <https://ru.wikipedia.org/wiki/%D0%93%D0%B0%D0%BC%D0%B8%D0%BB%D1%8C%D1%82%D0%BE%D0%BD%D0%BE%D0%B2%D0%B0_%D0%BC%D0%B5%D1%85%D0%B0%D0%BD%D0%B8%D0%BA%D0%B0> 





### В полярных координатах обобщённый импульс, соответствующий угловой скорости, — физический угловой момент. Для произвольного выбора обобщённых координат трудно получить интуитивную интерпретацию сопряжённых этим координатам импульсов или угадать их выражение, не используя прямо приведённую выше формулу.

sad&#x2026;  




### Отсюда, в частности, следует, что если какая-то координата оказалась циклической, то есть если функция Лагранжа от неё не зависит, а зависит только от её производной по времени, то для сопряжённого ей импульса {\displaystyle {\dot {p}}=0} {\dot  {p}}=0, то есть он является интегралом движения (сохраняется во времени), что несколько проясняет смысл обобщённых импульсов.

В этой формулировке, зависящей от выбора системы координат, не слишком очевиден тот факт, что различные обобщённые координаты являются в действительности не чем иным, как различными координатизациями одного и того же симплектического многообразия.  




### Любая гладкая функция {\displaystyle H: M&rarr; \mathbb {R} } H: M&rarr; \mathbb{R}  на симплектическом многообразии {\displaystyle M} M может использоваться, чтобы определить гамильтонову систему. Функция {\displaystyle H} H известна как гамильтониан или энергетическая функция. Симплектическое многообразие называют фазовым пространством. Гамильтониан порождает специальное векторное поле на симплектическом многообразии, известном как симплектическое векторное поле.




### Симплектическое векторное поле (также называется гамильтоновым векторным полем) порождает гамильтонов поток на многообразии. Интегральные кривые векторного поля являются однопараметрическим семейством преобразований многообразия с параметром, называемым время. Эволюция во времени задаётся симплектоморфизмами. Из теоремы Лиувилля следует, что каждый симплектоморфизм сохраняет форму объёма в фазовом пространстве. Множество симплектоморфизмов, порождаемых гамильтоновым потоком, обычно называют гамильтоновой механикой гамильтоновой системы.




### Гамильтоново векторное поле также порождает специальную операцию — скобка Пуассона. Скобка Пуассона действует на функции на симплектическом многообразии, таким образом придавая пространству функций на многообразии структуру алгебры Ли.




## phase: from any point on phase space, evolution is unique. it's kinda like initial data for a differential equation




# `[2018-11-20]` why symplectic spaces?

      historically, we empirically noticed/observed that principle of least action works (Lagrangian formulation), and there is an alternative and completely equivalent formulation (Hamiltonian).
    When we study symplectic geometry, we ask: what are the minimum requirements to *define* familiar basic physical concepts (energy/time), and so that we still have the usual properties (e.g. Hamiltonian flow).
    
    As a bonus, we drop the requirement for configuration space, and considering its cotangent bundle -- it can be *any* symplectic space.




## now figure out why is that interesting. lol




# `[2018-11-10]` intuition - What is a symplectic form intuitively? - MathOverflow

<https://mathoverflow.net/questions/19932/what-is-a-symplectic-form-intuitively/19935#19935>  

    soo, all we can do is correlate pairs of coordinate between each other? otherwise we can't tell which are position, which are momentum?




# Hamiltonian vector field - Wikipedia

    Suppose that (M, ω) is a symplectic manifold. Since the symplectic form ω is nondegenerate, it sets up a fiberwise-linear isomorphism




# Tweet from John Carlos Baez (@johncarlosbaez), at Nov 22, 22:01

<https://twitter.com/johncarlosbaez/status/1065727111120310272>  

    I thought about it longer and realized what was going on.
    You get equations like Hamilton's whenever a system *extremizes something subject to constraints*.   A moving particle minimizes action; a box of gas maximizes entropy.
    Read how it works:




# Legendre transformation - Wikipedia

    Legendre transformation, named after Adrien-Marie Legendre, is an involutive transformation on the real-valued convex functions




# `[2018-11-10]` What moment map is (as a physical concept) in sympletic geometry - Mathematics Stack Exchange

<https://math.stackexchange.com/questions/2447269/what-moment-map-is-as-a-physical-concept-in-sympletic-geometry>  




# `[2018-11-10]` classical mechanics - Intuition about Momentum Maps - Physics Stack Exchange

<https://physics.stackexchange.com/questions/203653/intuition-about-momentum-maps>  




# `[2018-11-14]` sg.symplectic geometry - How to see the Phase Space of a Physical System as the Cotangent Bundle - MathOverflow

<https://mathoverflow.net/questions/16460/how-to-see-the-phase-space-of-a-physical-system-as-the-cotangent-bundle/16462#16462>  




# `[2018-11-19]` Legendre transformation - Wikipedia

<https://en.wikipedia.org/wiki/Legendre_transformation#Further_properties>   

    For a strictly convex function, the Legendre transformation can be interpreted as a mapping between the graph of the function and the family of tangents of the graph.




# `[2018-11-18]` Symplectic integrator - Wikipedia

<https://en.wikipedia.org/wiki/Symplectic_integrator>  




# `[2018-11-19]` mathematical physics - Is there an analogue of configuration space in quantum mechanics? - Physics Stack Exchange

<https://physics.stackexchange.com/questions/33897/is-there-an-analogue-of-configuration-space-in-quantum-mechanics>  




# `[2018-11-18]` Applying Runge-Kutta method to circular - C++ Forum

<http://www.cplusplus.com/forum/general/103744/>  




# `[2018-09-13]` Chel<sub>of</sub><sub>the</sub><sub>sea</sub> comments on ELI5: What is symplectic geometry?

<https://www.reddit.com/r/explainlikeimfive/comments/47lwch/eli5_what_is_symplectic_geometry/d0duju7/>  

    It's geometry done on a curved surface that carries enough structure to measure area. In the same way that in Calc III you could do double integral over f dA to measure a sort of 'weighted area', on a symplectic manifold you can (in a suitable sense) take a double integral over f d(omega).




# `[2018-08-13]` poisson brackets are related to symplectic geometry (explains phase space)




# `[2018-08-13]` poisson brackets explained

<https://www.quora.com/What-is-an-intuitive-way-of-explaining-the-Poisson-bracket>  
{fg, h} = f {g, h} + g {f, h}  
looks like leibnitz rule!  
poisson bracket is derivation of the first arg w.r.t. to second  
symplectic manifold: equipped with a symplectic form, that maps any function to a vector on manifold  
so basially {f, g} is applying the form to g, and differentiating f along the integral curves of that vector field  
for hamiltonian,  
df/dt = {f, H} &#x2013; makes sense, motion along integral curve is motion in time  

The nice thing about the Hamiltonian formulation is that you can use lots of different coordinates. They will all work, as long as their Poisson brackets satisfy the equations above.  

If you've studied quantum mechanics, this should look familiar as the algebra of commutators, and Poisson brackets are a nice way to see the connection between classical and quantum mechanics.  

algebra with poisson bracket (lie bracket) is lie algebra  

Thus, the time evolution of a function f on a symplectic manifold can be given as a one-parameter family of symplectomorphisms (i.e., canonical transformations, area-preserving diffeomorphisms), with the time t being the parameter  




## `[2019-06-12]` need to add this to drill..




# `[2018-11-15]` 

phase space: R<sup>3</sup> x R<sup>3</sup> &#x2013; it's a base space for manifold  
Hamiltonaian is defined on manifold, not on its tangent bundle!  

hmm, but lagrangian is defined on the tangent bundle of configuration space?? <https://math.stackexchange.com/questions/1210047/why-is-the-lagrangian-a-function-on-the-tangent-bundle> confusing&#x2026;  

To summarize so far: a path in the tangent space "corresponds" (in the sense demonstrated in the example of h and H) to a path in the base space only if, in physicist notation, the function t↦q˙(t) turns out to be the time-derivative of the function t↦q(t). THAT is what that cryptic thing in your text is trying to say.  




## Spivak's Physics For Mathematicians,




## configuration space: M (a Manifold). Phase space: cotangent bundle over M (T<sub>\*</sub> M). Also a manifold?? Yeah, ok T<sub>\*</sub> M is also a manifold with dimension twise as what M got.




## right, and symplectic form is defined on the contagent bundle of configuration space! (or on a phase space?)




# learn basic QED and QFT      [[study]] [[qed]]

but this time, really really do exercises!  




## Feynman QED strange theory of light

takeaways  




### feynman diagrams are way of computing quantum amplitude. sum over all diagrams

to compute individual jump probabilities: use propagators solutions for free electron (Dirac) and photon (Klein-Gordon).  




### renormalization: meh, but only theory parameters depend on it, measurable stuff is not impacted




## Zee, Feynman. QED: Strange Theory of Light and Matter




## (long time ago) Tong, some notes in study/qft




# `[2018-12-15]` symplectic geometry - Learn Anything

<https://learn-anything.xyz>  




# `[2019-06-18]` Energy drift - Wikipedia      [[symplectic]]

<https://en.wikipedia.org/wiki/Energy_drift>  

    Energy drift - usually damping - is substantial for numerical integration schemes that are not symplectic, such as the Runge-Kutta family.




# `[2020-01-18]` chakravala/Grassmann.jl: ⟨Leibniz-Grassmann-Clifford⟩ differential geometric algebra / multivector simplicial complex      [[symplectic]]

<https://github.com/chakravala/Grassmann.jl>  

    The Grassmann.jl package provides tools for doing computations based on multi-linear algebra, differential geometry, and spin groups using the extended tensor algebra known as Leibniz-Grassmann-Clifford-Hestenes geometric algebra.




# `[2018-11-10]` Tangent bundle - Wikipedia <https://en.wikipedia.org/wiki/Tangent_bundle>      [[symplectic]] [[drill]]

    One of the main roles of the tangent bundle is to provide a domain and range for the derivative of a smooth function. Namely, if f : M → N is a smooth function, with M and N smooth manifolds, its derivative is a smooth function Df : TM → TN.




# Symplectic geometry foundations

    Quite interestingly, Symplectic Geometry is currently under review/investigation for some of the foundational papers in the field having serious gaps and outright errors after closer inspection. These concerns were always spoken of in hush hush tones and only in recent times have people stated their concerns publically. Some of the original authors refuse to retract their papers despite being assured their academic positions (which realistically, came through the reputation built up by these papers) are secure. Here's a quanta article about this fiasco: https://www.quantamagazine.org/the-fight-to-fix-symplectic-g...




## Intro to symplectic geom

    For those into physics, I wholeheartedly recommend Marsden and Ratiu's book, "Introduction to Mechanics and Symmetry", which deals mainly with the different formulations of physics applied to symplectic and associated geometries.




# Tweet from John Carlos Baez (@johncarlosbaez), at Jan 21, 18:29      [[symplectic]] [[towatch]]

    Symplectic geometry is like the evil twin of Euclidean geometry: instead of a dot product with v⋅w = w⋅v, we have one with v⋅w = -w⋅v.   But it's not really evil.   Check out Jonathan Lorand's talk!

<https://twitter.com/johncarlosbaez/status/1087416965012942849>  

