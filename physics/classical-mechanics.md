
# Table of Contents

-   [Definitions](#dfntns) 
    -   [A nonholonomic system &#x2013; state depends on the path taken in order to achieve it.](#nnhlnmcsystmsttdpndsnthpthtknnrdrtchvt) 
    -   [Phase space vs configuration space](#phsspcvscnfgrtnspc) 
-   [Lagrangian](#lgrngn) [[lagrangian]]
    -   [units of energy](#ntsfnrgy) 
    -   [no single expression for all physical systems](#nsnglxprssnfrllphysclsystms) 
    -   [only applicable to systems with holonomic constraints](#nlypplcbltsystmswthhlnmccnstrnts) 
    -   [Why only first derivatives are appearing](#whynlyfrstdrvtvsrpprng) 
    -   [Independent position and velocity](#ndpndntpstnndvlcty) 
        -   [in a sense these are initial conditions so both are necessary](#nsnsthsrntlcndtnssbthrncssry) 
        -   [Let me refer to this great book: "Applied Differential Geometry". By William L. Burke. The very first line of the book (where an author usually says to whom this book is devoted) is this: "To all those who like me have wondered how in the hell you can change q' without changing q"](#ltmrfrtthsgrtbkpplddffrntnthhllycnchngqwthtchngngq) 
        -   [https://physics.stackexchange.com/questions/119992/what-do-the-derivatives-in-these-hamilton-equations-mean](#sphyscsstckxchngcmqstnswhtdthdrvtvsnthshmltnqtnsmn) 
        -   [another explanation from the same guy https://physics.stackexchange.com/questions/60706/lagrangian-mechanics-and-time-derivative-on-general-coordinates](#nthrxplntnfrmthsmgysphyscchncsndtmdrvtvngnrlcrdnts) 
        -   [interesting point that var(q') = d/dt var(q) (why?) https://physics.stackexchange.com/a/985/40624](#ntrstngpntthtvrqddtvrqwhysphyscsstckxchngcm) 
        -   [might be insightful?&#x2026; https://physics.stackexchange.com/a/2895/40624](#mghtbnsghtflsphyscsstckxchngcm) 
        -   [https://physics.stackexchange.com/questions/168551/independence-of-position-and-velocity-in-lagrangian-from-the-point-of-view-of-ph &#x2013; not sure if useful&#x2026;](#sphyscsstckxchngcmqstnsndngnfrmthpntfvwfphntsrfsfl) 
        -   [https://physics.stackexchange.com/questions/60706/lagrangian-mechanics-and-time-derivative-on-general-coordinates &#x2013; not sure if useful..](#sphyscsstckxchngcmqstnslgmdrvtvngnrlcrdntsntsrfsfl) 
    -   [For every symmetry, there is a conserved quantity](#frvrysymmtrythrscnsrvdqntty) 
    -   [Einstein was not satisfied about GR until he derived it from lagrangian (as an indication how powerful is the concept) https://www.reddit.com/r/Physics/comments/3me1hr/explanation\_of\_lagrangian\_mechanics/cveb611/](#nstnwsntstsfdbtgrntlhdrvdmhrxplntnflgrngnmchncscvb) 
    -   [reddit recommends Taylor's book](#rddtrcmmndstylrsbk) 
    -   [as an analogy: when you learn energy, dealing with forces is much easier; when you learn lagrangian, dealing with crazy coordinates and constraints much easier](#snnlgywhnylrnnrgydlngwthfcrzycrdntsndcnstrntsmchsr) 
    -   [When you find the Euler-Lagrange equations for your system, they will be written in terms of these generalized coordinates, and the terms in the equations are known as generalized forces. This is because usually the Euler-Lagrange equations have something that looks a lot like "ma" (mass times acceleration) on one side of the equations, and thus the other terms could be interpreted as "forces", but written in these general variables.](#whnyfndthlrlgrngqtnsfryrssfrcsbtwrttnnthsgnrlvrbls) 
    -   [`[2019-01-15]` http://cp3-origins.dk/a/14332](#cprgnsdk) [[toblog]]
        -   [hmm, interesting about Wick rotation&#x2026;](#hmmntrstngbtwckrttn) 
    -   [Galilean invariance forces classical lagrangian to depend on velocity quadratically](#gllnnvrncfrcsclsscllgrngntdpndnvlctyqdrtclly) 
        -   [`[2019-01-15]` classical mechanics - Deriving the Lagrangian for a free particle - Physics Stack Exchange](#clssclmchncsdrvngthlgrngnfrfrprtclphyscsstckxchng) [[lagrangian]]
        -   [`[2018-11-29]` classical mechanics - Why does Lagrangian of free particle depend on the square of the velocity ? - Physics Stack Exchange](#clssclmchncswhydslgrngnffqrfthvlctyphyscsstckxchng) 
        -   [`[2018-11-29]` newtonian mechanics - Galilean invariance of Lagrangian for non-relativistic free point particle? - Physics Stack Exchange](#nwtnnmchncsgllnnvrncflgrnfrpntprtclphyscsstckxchng) [[lagrangian]]
    -   [`[2018-11-30]` Degenerate Lagrangian? - My Math Forum](#dgnrtlgrngnmymthfrm) 
    -   [`[2018-11-25]` What does a Lagrangian of the form \(L=m^2\dot x^4 +U(x)\dot x^2 -W(x)\) represent? - Physics Stack Exchange](#whtdslgrngnfthfrmlmdtxxdtxwxrprsntphyscsstckxchng) 
    -   [on Lagrangian being extreme value/minimum](#nlgrngnbngxtrmvlmnmm) 
        -   [`[2018-12-04]` lagrangian formalism - Confusion regarding the principle of least action in Landau & Lifshitz "The Classical Theory of Fields" - Physics Stack Exchange](#lgrngnfrmlsmcnfsnrgrdngthlthryffldsphyscsstckxchng) 
        -   [`[2018-12-04]` lagrangian formalism - Hamilton's Principle - Physics Stack Exchange](#lgrngnfrmlsmhmltnsprncplphyscsstckxchng) 
        -   [`[2018-12-02]` http://www.scholarpedia.org/article/Principle\_of\_least\_action#When\_Action\_is\_a\_Minimum](#wwwschlrpdrgrtclprncplflstctnwhnctnsmnmm) 
        -   [`[2018-12-02]` Even more trivial example when least action principle doesn't work](#vnmrtrvlxmplwhnlstctnprncpldsntwrk) 
    -   [`[2018-11-30]` Лагранжиан L {\displaystyle L} L называется вырожденным, если его оператор Эйлера — Лагранжа удовлетворяет нетривиальным тождествам Нётер. В этом случае уравнения Эйлера — Лагранжа не являются независимыми](#лагранжианldsplystylllназнжанеявляютсянезависимыми) 
-   [`[2019-01-15]` Legendre transform](#lgndrtrnsfrm) 
    -   [`[2019-01-15]` nice intuition in terms of areas](#ncnttnntrmsfrs) 
    -   [`[2018-11-29]` Преобразование Лежандра — Википедия](#преобразованиележандравикипедия) [[lagrangian]]
        -   [`[2019-01-15]` В том случае, когда лагранжиан не вырожден по скоростям, то есть](#втомслучаекогдалагранжианвырожденпоскоростямтоесть) 
    -   [`[2019-01-15]` Making Sense of the Legendre Transform](#mkngsnsfthlgndrtrnsfrm) 
    -   [So the Fourier transform and the Legendre transform may be interpreted as the same thing, just over different semirings.](#sthfrrtrnsfrmndthlgndrtrnthsmthngjstvrdffrntsmrngs) 
    -   [https://physicstravelguide.com/advanced\_tools/legendre\_transformation#tab\_\_concrete](#sphyscstrvlgdcmdvncdtlslgndrtrnsfrmtntbcncrt) 
    -   [http://blog.jessriedel.com/2017/06/28/legendre-transform/](#blgjssrdlcmlgndrtrnsfrm) 
-   [Hamiltonian](#hmltnn) 
    -   [has some meaning in statistical physics](#hssmmnngnsttstclphyscs) 
    -   [something about Poisson brackets](#smthngbtpssnbrckts) 
    -   [configuration space with dimension n: 2n Hamilton equations of first order; n Euler-Lagrange of second order](#cnfgrtnspcwthdmnsnnnhmltnsffrstrdrnlrlgrngfscndrdr) 
    -   [Hamiltonians are easier to find transformations to canonical coordinates](#hmltnnsrsrtfndtrnsfrmtnstcnnclcrdnts) 
    -   [`[2019-01-16]` is hamiltonian same thing as energy?](#shmltnnsmthngsnrgy) 
        -   [https://physics.stackexchange.com/questions/11905/when-is-the-hamiltonian-of-a-system-not-equal-to-its-total-energy?noredirect=1&lq=1](#sphyscsstckxchngcmqstnswhstmntqlttsttlnrgynrdrctlq) 
        -   [`[2018-11-25]` classical mechanics - Example where Hamiltonian \(H \neq T+V=E\), but \(E=T+V\) is conserved - Physics Stack Exchange](#clssclmchncsxmplwhrhmltnnttvscnsrvdphyscsstckxchng) 
-   [physics sim for phase space *repos/physics-sim*](#physcssmfrphsspcrpsphyscssm) [[study]] [[viz]] [[lagrangian]]
-   [additional term depending on velocity is kinda like time transformation?](#ddtnltrmdpndngnvlctyskndlktmtrnsfrmtn) [[study]] [[lagrangian]]
-   [-----&#x2013;&#x2014; `[2019-01-15]`  -------&#x2013;&#x2014; review later&#x2026;](#rvwltr) 
-   [`[2018-11-29]` homework and exercises - Lagrangian in a system with a specific velocity dependent potential - Physics Stack Exchange](#hmwrkndxrcsslgrngnnsystmwpndntptntlphyscsstckxchng) [[lagrangian]]
-   [------&#x2013;&#x2014;  `[2019-01-15]`  ---------&#x2013;&#x2014; needs review](#ndsrvw) 
-   [Griffith classical mechanics](#grffthclssclmchncs) 
-   [`[2018-07-24]` Classical Mechanics](#clssclmchncs) 
    -   [lagrangian (kinda + there was some intuition in baez notes?)](#lgrngnkndthrwssmnttnnbznts) 
    -   [hamiltonian (bit more tricky)](#hmltnnbtmrtrcky) 
    -   [poisson brackets: ???](#pssnbrckts) 
    -   [canonical coordinates and derivatives &#x2013; why's that enough? or by definition of 'classical'?](#cnnclcrdntsnddrvtvswhysthtnghrbydfntnfclsscl) 
    -   [????](#15905_15955) 
-   [baez lagrangian mechanics](#bzlgrngnmchncs) [[baez]]
    -   [principle of minumum energy explanation 1.2.2](#prncplfmnmmnrgyxplntn) 
    -   [p.33 special relativity](#pspclrltvty) 
    -   [gauge symmetries](#ggsymmtrs) 
    -   [p46 cool analogy between refraction and riemannian metric in GR](#pclnlgybtwnrfrctnndrmnnnmtrcngr) 
-   [ham vs lagr https://www.reddit.com/r/askscience/comments/6be3ex/what\_are\_lagrangian\_and\_hamiltonian\_mechanics\_in/](#hmvslgrswwwrddtcmrskscnccwhtrlgrngnndhmltnnmchncsn) 
    -   [I think this is sort of misleading, they talk about dependency again&#x2026;](#thnkthsssrtfmsldngthytlkbtdpndncygn) 
-   [How are symmetries precisely defined? - Physics Stack Exchange](#hwrsymmtrsprcslydfndphyscsstckxchng) 
-   [action principle for SR](#ctnprncplfrsr) [[relativity]]
    -   [also problems](#lsprblms) 
    -   [nice book, read more from it?](#ncbkrdmrfrmt) 
-   [https://en.wikipedia.org/wiki/Generalized\_coordinates](#snwkpdrgwkgnrlzdcrdnts) 
-   [`[2018-07-31]` some random notes](#smrndmnts) [[lagrangian]] [[hamiltonian]]
-   [`[2018-11-25]` Zero Hamiltonian and its energies | Physics Forums](#zrhmltnnndtsnrgsphyscsfrms) 
    -   [`[2019-06-18]` eh, they are talking about invariance by reparametrization, but I don't think I really understand what they mean&#x2026;](#hthyrtlkngbtnvrncbyrprmtrntthnkrllyndrstndwhtthymn) 
-   [`[2018-12-02]` Are the Hamiltonian and Lagrangian always convex functions? - Physics Stack Exchange](#rthhmltnnndlgrngnlwyscnvxfnctnsphyscsstckxchng) [[lagrangian]]
    -   [`[2019-01-16]` also good answer, basically explaining that it's not great to impose convexity conditions on only one set of canonical coordinates https://physics.stackexchange.com/a/104279/40624](#lsgdnswrbscllyxplnngthttslcrdntssphyscsstckxchngcm) 
    -   [`[2019-01-16]` https://physics.stackexchange.com/questions/103997/are-the-hamiltonian-and-lagrangian-always-convex-functions#comment760950\_339519](#sphyscsstckxchngcmqstnsrtlgrngnlwyscnvxfnctnscmmnt) 
-   [`[2018-11-15]` Proof by Picture](#prfbypctr) [[viz]]
-   [`[2018-11-18]` book: Structure and Interpretation of Classical Mechanics](#bkstrctrndntrprttnfclssclmchncs) 
-   [hmm, to visualise phase trajectories, we can just do 3D plot, then we know that the particle is moving along isolines](#hmmtvslsphstrjctrswcnjstdknwthtthprtclsmvnglngslns) [[hamiltonian]] [[viz]]
-   [Isotropic lagrangian velocity](#strpclgrngnvlcty) [[lagrangian]]
    -   [`[2019-06-18]` Now since space is isotropic, L should be independent of velocity v⃗ , and should in fact be a function of |v⃗ |2.](#nwsncspcsstrpclshldbndpndlctyv⃗ndshldnfctbfnctnfv⃗) 
-   [discrete lagrangian? vary it on space of matrices??](#dscrtlgrngnvrytnspcfmtrcs) [[think]]
    -   [`[2019-06-18]` https://en.wikipedia.org/wiki/Variational\_integrator](#snwkpdrgwkvrtnlntgrtr) 
-   [`[2018-11-30]` Задачка на Лагранжиан : Помогите решить / разобраться (Ф) - Страница 3](#задачканалагранжианпомогиешитьразобратьсяфстраница) 
-   [`[2020-08-09]` Notes & HW for Section 6.1](#srstwndhhghsjrmntscshtmlntshwfrsctn) [[lagrangian]]
-   [`[2020-08-09]` Structure and Interpretation of Classical Mechanics: Chapter 7](#smtprssmtdstsdfltflsttlsctrprttnfclssclmchncschptr) 
-   [`[2018-08-25]` In classical mechanics, the state of a system is determined by a point in phase space](#nclssclmchncsthsttfsystmsdtrmndbypntnphsspc) [[lagrangian]]
-   [`[2019-03-20]` lagrangian formalism - What is the difference between a complex scalar field and two real scalar fields? - Physics Stack Exchange](#lgrngnfrmlsmwhtsthdffrncbrlsclrfldsphyscsstckxchng) 
-   [`[2018-07-31]` https://en.wikipedia.org/wiki/Ostrogradsky\_instability &#x2013; explanation why differential equations of orders higher than two do not appear in physics](#snwkpdrgwkstrgrdskynstbltdrshghrthntwdntpprnphyscs) [[math]] [[physics]] [[diffeq]]
    -   [`[2021-01-31]` http://www.scholarpedia.org/article/Ostrogradsky%27s\_theorem\_on\_Hamiltonian\_instability more detailed explanation](#wwwschlrpdrgrtclstrgrdskyhmltnnnstbltymrdtldxplntn) 
-   [`[2020-01-15]` Noether’s Theorem – A Quick Explanation (2019)](#snwsycmbntrcmtmdnthrsthrmqckxplntn) 





# Definitions 





## A nonholonomic system &#x2013; state depends on the path taken in order to achieve it.




## Phase space vs configuration space




# Lagrangian       [[lagrangian]]





## units of energy




## no single expression for all physical systems




## only applicable to systems with holonomic constraints




## Why only first derivatives are appearing

Ostrogradsky instability  
<https://physics.stackexchange.com/questions/4102/why-are-there-only-derivatives-to-the-first-order-in-the-lagrangian>  




## Independent position and velocity

<https://physics.stackexchange.com/questions/885/calculus-of-variations-how-does-it-make-sense-to-vary-the-position-and-the-ve>  




### in a sense these are initial conditions so both are necessary




### Let me refer to this great book: "Applied Differential Geometry". By William L. Burke. The very first line of the book (where an author usually says to whom this book is devoted) is this: "To all those who like me have wondered how in the hell you can change q' without changing q"




### <https://physics.stackexchange.com/questions/119992/what-do-the-derivatives-in-these-hamilton-equations-mean> 

q and q' are just labels, treat them independently  
good points about meaning in the very end  




### another explanation from the same guy <https://physics.stackexchange.com/questions/60706/lagrangian-mechanics-and-time-derivative-on-general-coordinates>




### interesting point that var(q') = d/dt var(q) (why?) <https://physics.stackexchange.com/a/985/40624>




### might be insightful?&#x2026; <https://physics.stackexchange.com/a/2895/40624>




### <https://physics.stackexchange.com/questions/168551/independence-of-position-and-velocity-in-lagrangian-from-the-point-of-view-of-ph> &#x2013; not sure if useful&#x2026;




### <https://physics.stackexchange.com/questions/60706/lagrangian-mechanics-and-time-derivative-on-general-coordinates> &#x2013; not sure if useful..




## For every symmetry, there is a conserved quantity




## Einstein was not satisfied about GR until he derived it from lagrangian (as an indication how powerful is the concept) <https://www.reddit.com/r/Physics/comments/3me1hr/explanation_of_lagrangian_mechanics/cveb611/>




## reddit recommends Taylor's book




## as an analogy: when you learn energy, dealing with forces is much easier; when you learn lagrangian, dealing with crazy coordinates and constraints much easier




## When you find the Euler-Lagrange equations for your system, they will be written in terms of these generalized coordinates, and the terms in the equations are known as generalized forces. This is because usually the Euler-Lagrange equations have something that looks a lot like "ma" (mass times acceleration) on one side of the equations, and thus the other terms could be interpreted as "forces", but written in these general variables.




## `[2019-01-15]` <http://cp3-origins.dk/a/14332>      [[toblog]]

    When the action, and hence the phase, is stationary changing it by a small amount doesn’t change the phase by much. In a small region (compared to ℏ) these paths can add up coherently to give a significant contribution to the sum above. This is what we see in the cartoon above for a very small subset of paths.
    Classical mechanics is quantum mechanics using the stationary phase approximation.




### hmm, interesting about Wick rotation&#x2026;

    Paths far from the minimum hardly contribute anything and so it isn’t necessary to calculate the action arbitrarily accurately.

eh?  




## Galilean invariance forces classical lagrangian to depend on velocity quadratically





### `[2019-01-15]` classical mechanics - Deriving the Lagrangian for a free particle - Physics Stack Exchange      [[lagrangian]]

<https://physics.stackexchange.com/questions/23098/deriving-the-lagrangian-for-a-free-particle>  
Comment:  
justification of lagrangian for classical mechanics from Landau&#x2026; weird, didn't really get it  




### `[2018-11-29]` classical mechanics - Why does Lagrangian of free particle depend on the square of the velocity ? - Physics Stack Exchange

<https://physics.stackexchange.com/questions/63370/why-does-lagrangian-of-free-particle-depend-on-the-square-of-the-velocity/92561>   

The Lagrangian should not only be independent of the direction of v⃗ v→ but it should also change correctly under a Galilean transformation. For instance, if KK and K′K′ are two frames of reference with a relative velocity V⃗ V→ then the two Lagrangians LL and L′L′ should differ only by a total time derivative.  




### `[2018-11-29]` newtonian mechanics - Galilean invariance of Lagrangian for non-relativistic free point particle? - Physics Stack Exchange      [[lagrangian]]

<https://physics.stackexchange.com/questions/14875/galilean-invariance-of-lagrangian-for-non-relativistic-free-point-particle>  




## `[2018-11-30]` Degenerate Lagrangian? - My Math Forum

<http://mymathforum.com/differential-equations/43493-degenerate-lagrangian.html>  
a degenerate Lagrangian is one who's Hesse determinant is zero. It's a condition on the second partial derivatives of the Lagrangian.  

there is also a link to pdf, might be worth reading&#x2026;  




## `[2018-11-25]` What does a Lagrangian of the form \(L=m^2\dot x^4 +U(x)\dot x^2 -W(x)\) represent? - Physics Stack Exchange

 <https://physics.stackexchange.com/questions/17406/what-does-a-lagrangian-of-the-form-l-m2-dot-x4-ux-dot-x2-wx-represent>  
eh, weird. complex expression for lagrangian that ends up looking same as classical. well ok  




## on Lagrangian being extreme value/minimum





### `[2018-12-04]` lagrangian formalism - Confusion regarding the principle of least action in Landau & Lifshitz "The Classical Theory of Fields" - Physics Stack Exchange

<https://physics.stackexchange.com/questions/122486/confusion-regarding-the-principle-of-least-action-in-landau-lifshitz-the-clas#comment249472_122504>  
conjugate points; about infinitesimal path, characteristic scale of the problem  
conditions for lagrangian regularity and conjugate points  




### `[2018-12-04]` lagrangian formalism - Hamilton's Principle - Physics Stack Exchange

<https://physics.stackexchange.com/questions/9/hamiltons-principle>  

    Basically, the whole thing is summarized in a nutshell in Richard P. Feynman, The Feynman Lectures on Physics (Addison–Wesley, Reading, MA, 1964), Vol. II, Chap. 19. (I think, please correct me if I'm wrong here). The fundamental idea is that the action integral defines the quantum mechanical amplitude for the position of the particle, and the amplitude is stable to interference effects (-->has nonzero probability of occurrence) only at extrema or saddle points of the action integral. The particle really does explore all alternative paths probabilistically.




### `[2018-12-02]` <http://www.scholarpedia.org/article/Principle_of_least_action#When_Action_is_a_Minimum>

    or some 1D potentials V(x) (those with ∂2V/∂x2≤0 everywhere), e.g. V(x)=0 , V(x)=mgx , and V(x)=−Cx2 , all true trajectories have minimum S . For most potentials, however, only sufficiently short true trajectories have minimum action; the others have an action saddle point. "Sufficiently short" means that the final space-time event occurs before the so-called kinetic focus event of the trajectory.




### `[2018-12-02]` Even more trivial example when least action principle doesn't work

    Принцип наименьшего действия. Часть 2 / Хабр https://habr.com/ru/post/426253/
    
    На рисунке нарисованы обе физически возможные траектории движения шара. Зеленая траектория соответствует покоящемуся шару, в то время как синяя соответствует шару, отскочившему от пружинящей стенки.
    Однако минимальным действием обладает только одна из них, а именно первая! У второй траектории действие больше. Получается, что в данной задаче имеются две физически возможных траектории и всего одна с минимальным действием. Т.е. в данном случае принцип наименьшего действия не работает.




## `[2018-11-30]` Лагранжиан L {\displaystyle L} L называется вырожденным, если его оператор Эйлера — Лагранжа удовлетворяет нетривиальным тождествам Нётер. В этом случае уравнения Эйлера — Лагранжа не являются независимыми

<https://ru.wikipedia.org/wiki/%D0%A2%D0%BE%D0%B6%D0%B4%D0%B5%D1%81%D1%82%D0%B2%D0%B0_%D0%9D%D1%91%D1%82%D0%B5%D1%80>  




# `[2019-01-15]` Legendre transform





## `[2019-01-15]` nice intuition in terms of areas

<https://physics.stackexchange.com/a/69374/40624>  




## `[2018-11-29]` Преобразование Лежандра — Википедия      [[lagrangian]]

<https://ru.wikipedia.org/wiki/%D0%9F%D1%80%D0%B5%D0%BE%D0%B1%D1%80%D0%B0%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5_%D0%9B%D0%B5%D0%B6%D0%B0%D0%BD%D0%B4%D1%80%D0%B0>  




### `[2019-01-15]` В том случае, когда лагранжиан не вырожден по скоростям, то есть

{\displaystyle p=&nabla; \_{u}L(q,u)&ne; 0,} {\displaystyle p=&nabla; \_{u}L(q,u)&ne; 0,}  
можно сделать преобразование Лежандра по скоростям и получить новую функцию, называемую гамильтонианом:  




## `[2019-01-15]` Making Sense of the Legendre Transform

nice pdf, basically they say it's just a different view, sometimes it's easier to control the derivative  
they introduce generalised forces too  
that's not surprising there is connection with thermodynamics, they show some stuff with Gibbs energy etc  
<https://johncarlosbaez.wordpress.com/2012/01/19/classical-mechanics-versus-thermodynamics-part-1/>  




## So the Fourier transform and the Legendre transform may be interpreted as the same thing, just over different semirings.

<http://blog.sigfpe.com/2005/10/quantum-mechanics-and-fourier-legendre.html>  
fucking hell!! that's so cool  




## <https://physicstravelguide.com/advanced_tools/legendre_transformation#tab__concrete> 

(Legendre transformation is "zero temperature limit" of the Laplace Transformation)  




## <http://blog.jessriedel.com/2017/06/28/legendre-transform/> 

Two convex functions f and g are Legendre transforms of each other when their first derivatives are inverse functions:  
and another nice plot with areas intuition as well  
All of the dynamical laws are constructed from derivatives of H and L, and we decline to specify an additive constant for the same reason we do so with conservative potentialsi   and, more generally, anti-derivatives.  




# Hamiltonian 

<https://physics.stackexchange.com/questions/89035/whats-the-point-of-hamiltonian-mechanics#89036>  




## has some meaning in statistical physics




## something about Poisson brackets




## configuration space with dimension n: 2n Hamilton equations of first order; n Euler-Lagrange of second order




## Hamiltonians are easier to find transformations to canonical coordinates




## `[2019-01-16]` is hamiltonian same thing as energy?





### <https://physics.stackexchange.com/questions/11905/when-is-the-hamiltonian-of-a-system-not-equal-to-its-total-energy?noredirect=1&lq=1> 




### `[2018-11-25]` classical mechanics - Example where Hamiltonian \(H \neq T+V=E\), but \(E=T+V\) is conserved - Physics Stack Exchange

<https://physics.stackexchange.com/questions/194772/example-where-hamiltonian-h-neq-tv-e-but-e-tv-is-conserved>  




# physics sim for phase space *repos/physics-sim*      [[study]] [[viz]] [[lagrangian]]




# additional term depending on velocity is kinda like time transformation?      [[study]] [[lagrangian]]




# -----&#x2013;&#x2014; `[2019-01-15]`  -------&#x2013;&#x2014; review later&#x2026;




# `[2018-11-29]` homework and exercises - Lagrangian in a system with a specific velocity dependent potential - Physics Stack Exchange      [[lagrangian]]

<https://physics.stackexchange.com/questions/261221/lagrangian-in-a-system-with-a-specific-velocity-dependent-potential#comment596613_261221>  




# ------&#x2013;&#x2014;  `[2019-01-15]`  ---------&#x2013;&#x2014; needs review




# Griffith classical mechanics




# `[2018-07-24]` Classical Mechanics

 I guess I need to work out some simple classical system by myself  
understand:  




## lagrangian (kinda + there was some intuition in baez notes?)




## hamiltonian (bit more tricky)




## poisson brackets: ???




## canonical coordinates and derivatives &#x2013; why's that enough? or by definition of 'classical'?




## ???? 




# baez lagrangian mechanics      [[baez]]

<http://math.ucr.edu/home/baez/classical/>  




## principle of minumum energy explanation 1.2.2




## p.33 special relativity

Many Lagrangiansdothis,butthe\best"oneshouldgive anactionthatisindependentoftheparameterizationofthepath|sincetheparameterizationis\unphysical":it can'tbe measured.Sotheaction  




## gauge symmetries

Thesesymmetriesgive conservedquantitiesthatworkouttoequalzero!  
gauge symmetries result in conserved quantities&#x2026; which are just equal to zero  




## p46 cool analogy between refraction and riemannian metric in GR




# ham vs lagr <https://www.reddit.com/r/askscience/comments/6be3ex/what_are_lagrangian_and_hamiltonian_mechanics_in/>

Furthermore, whereas in Lagrangian mechanics there is a dependence between the generalized coordinates q and their velocities (the latter being the time derivatives of the former), in Hamiltonian mechanics the momenta are to be regarded are independent from the generalized coordinates.  
With these new coordinates, one proceeds to demand again that the action is minimized, and, instead of the Euler-Lagrange equations, one finds what are known as Hamilton's canonical equations. Again these are the equations of motion of the system, which are to be solved in order to find the trajectory. One key difference is that if your system required N generalized coordinates, and thus N Euler-Lagrange equations, there will be 2N Hamilton canonical equations but they are "half as difficult" to solve.  

That's the best I can do without getting technical. Also, Hamiltonian mechanics is cooler, just saying.  




## I think this is sort of misleading, they talk about dependency again&#x2026;




# How are symmetries precisely defined? - Physics Stack Exchange

<https://physics.stackexchange.com/questions/98714/how-are-symmetries-precisely-defined>  




# action principle for SR      [[relativity]]

<http://fma.if.usp.br/~amsilva/Livros/Zwiebach/chapter5.pdf>  

infer ansatz for action from dimensional analysis  

S<sub>nonrel</sub> = int 1/2 m v<sup>2</sup>(t) dt  
hamilton's equation: dv/dt = 0, hence constant velocity  

doesn't work for sr, rationale: is not forbidding v > c.  

require action to be Lorentz scalar  

S = -mc int ds &#x2013; in the nonrelativistic limit results in same physics ans nonrel lagrangian  
also, that explains the fact that particle traces the path minimizing spacetime interval  

momentum and hamiltonian &#x2013; coincide with energy  
reparameterisation: express invariant via square root of metric and coord. derivatives  

right, and we get euler-lagrange equations as a result d<sup>2</sup> x<sup>u</sup>/ds<sup>2</sup> = 0 &#x2013; basically 4-velocity is constant!  

guessing electric charge lagrangian..  




## also problems




## nice book, read more from it?




# <https://en.wikipedia.org/wiki/Generalized_coordinates> 

Generalized coordinates &#x2013; like normal coordinates, but without redudancy in constraints. They are independent; basically it means that for any generalised coordinates [tuple] there must be a valid system?  
<https://en.wikipedia.org/wiki/Holonomic_constraints#Transformation_to_independent_generalized_coordinates>  

benefit of generalised coordinates is most apparent when considering double pendulum <https://en.wikipedia.org/wiki/Generalized_coordinates#Double_pendulum>  




# `[2018-07-31]` some random notes      [[lagrangian]] [[hamiltonian]]

x'<sup>2</sup> + x<sup>2</sup> = C<sup>2</sup> &#x2013; energy conservation  

Force F(x); potential energy U(x) as integral of force  

Take 1/2 m v<sup>2</sup> + U(x) &#x2013; call it "total energy", it is conserved  

TODO what if force depends on time explicitly?  

Law of physics: there exists a three-dimenstional potential!  

Principle of least action  

Hamiltonian from Lagrangian  

dH/dt = - &part; L / &part; t  

Lagrangian -> Euler-Lagrange equations  

Holonomic constraints take form: f(q<sub>1</sub>, &hellip; q<sub>n</sub>, t) = 0  

Holonomic system => L = K - U  

Nonholomonic system: rubber ball allowed to roll, but not slide/spin  

Lagrange multipliers and forces of constraint, Taylor 278  

If coordinate q<sub>i</sub> is ignorable (dL/dq<sub>i</sub> = 0), the corresponding generalized momentum p<sub>i</sub> = dL/dq'<sub>i</sub> is conserved  

H(q<sub>1</sub> &#x2026; q<sub>n</sub>, p<sub>1</sub> &#x2026; p<sub>n</sub>)  

q' = dH/dp  
p' = -dH/dq  

B = &nabla; x A + &nabla; S  

A is defined up to the gradient of some scalar field, guage field  

Poisson brackets  

-   {A, B} = - {B, A}
-   {A + B, C} = {A, C} + {B, C}
-   {a A, B} = a {A, B}
-   {AB, C} = {A, C} B + A {B, C}

-   {q<sub>i</sub>, q<sub>j</sub>} = 0
-   {p<sub>i</sub>, p<sub>j</sub>} = 0
-   {q<sub>i</sub>, p<sub>j</sub>} = delta<sub>ij</sub>

-   Q' = {Q, H} &#x2013; change of quantity over time
-   {Q, L<sub>y</sub>} &#x2013; change of quantity over rotation




# `[2018-11-25]` Zero Hamiltonian and its energies | Physics Forums

<https://www.physicsforums.com/threads/zero-hamiltonian-and-its-energies.145574/>  

    First of all, you are not understanding what he Hamiltonian is. The Hamiltonian is not the value of the energy, it is a relationship between position and momentum for a particular system. If the Hamiltonian is p^2 + q^2, and the value of p^2 + q^2 is zero, then the Hamiltonian is p^2 + q^2, not zero. It is analogous to Bush being the president. Bush is the current VALUE of "president", but the concept of president is not synonymous with "Bush".




## `[2019-06-18]` eh, they are talking about invariance by reparametrization, but I don't think I really understand what they mean&#x2026;




# `[2018-12-02]` Are the Hamiltonian and Lagrangian always convex functions? - Physics Stack Exchange      [[lagrangian]]

<https://physics.stackexchange.com/questions/103997/are-the-hamiltonian-and-lagrangian-always-convex-functions>  




## `[2019-01-16]` also good answer, basically explaining that it's not great to impose convexity conditions on only one set of canonical coordinates <https://physics.stackexchange.com/a/104279/40624>

    In conclusion, convexity does not seem to be a first principle per se, but rather a consequence of the type of QFTs that we typically are able to make sense of. It might be that it is possible to give a non-perturbative definition of a non-convex (but unitary) theory.




## `[2019-01-16]` <https://physics.stackexchange.com/questions/103997/are-the-hamiltonian-and-lagrangian-always-convex-functions#comment760950_339519>

hmm that's interesting, he got a reply about considering sheets of the hamiltonian, each sheet convex&#x2026; so maybe it does make sense??  




# `[2018-11-15]` Proof by Picture      [[viz]]

<http://www.physicsinsights.org/proof_by_picture.html>  




# `[2018-11-18]` book: Structure and Interpretation of Classical Mechanics

<https://groups.csail.mit.edu/mac/users/gjs/6946/sicm-html/>  




# hmm, to visualise phase trajectories, we can just do 3D plot, then we know that the particle is moving along isolines      [[hamiltonian]] [[viz]]




# Isotropic lagrangian velocity      [[lagrangian]]

<https://physics.stackexchange.com/questions/212909/lagrangian-is-isotropic-in-space>  




## `[2019-06-18]` Now since space is isotropic, L should be independent of velocity v⃗ , and should in fact be a function of |v⃗ |2.




# discrete lagrangian? vary it on space of matrices??      [[think]]





## `[2019-06-18]` <https://en.wikipedia.org/wiki/Variational_integrator>




# `[2018-11-30]` Задачка на Лагранжиан : Помогите решить / разобраться (Ф) - Страница 3

<https://dxdy.ru/post552620.html>  

    les в сообщении #552466 писал(а):
    И как в таком случае вводят импульсы?
    Связями. Если интеренсно, посмотрите книгу Дирак, "Принципы квантовой механики". Бонус-глава "Лекции по квантовой механике
    
    бы очень рекомендовал замечательную книгу
    Гитман Д.М., Тютин И.В. Каноническое квантование полей со связями.
    Думаю, ТС хватит прочитать первые две главы, чтобы получить ответы на инересующие в




# `[2020-08-09]` [Notes & HW for Section 6.1](http://users.etown.edu/h/hughesjr/ma321/notes/c6s1.html)      [[lagrangian]]

classification of critical points  




# `[2020-08-09]` [Structure and Interpretation of Classical Mechanics: Chapter 7](https://mitpress.mit.edu/sites/default/files/titles/content/sicm_edition_2/preface001.html)

    The Lagrangian L must be interpreted as a function of the position and velocity components qi and q˙i, so that the partial derivatives make sense, but then in order for the time derivative d/dt to make sense solution paths must have been inserted into the partial derivatives of the Lagrangian to make functions of time. The traditional use of ambiguous notation is convenient in simple situations, but in more complicated situations it can be a serious handicap to clear reasoning. In order that the reasoning be clear and unambiguous, we have adopted a more precise mathematical notation. Our notation is functional and follows that of modern mathematical presentations.2 An introduction to our functional notation is in an appendix.




# `[2018-08-25]` In classical mechanics, the state of a system is determined by a point in phase space      [[lagrangian]]

It's unique! In the same way as quantum state is unique  




# `[2019-03-20]` lagrangian formalism - What is the difference between a complex scalar field and two real scalar fields? - Physics Stack Exchange

<https://physics.stackexchange.com/questions/3503/what-is-the-difference-between-a-complex-scalar-field-and-two-real-scalar-fields>  

    They're identical. Typically, we use complex fields if we have a U(1)U(1) symmetry, or some more complicated gauge group with complex representations.
    
    Incidentally, the same comment applies to whether we use Majorana spinors or Weyl spinors.




# `[2018-07-31]` <https://en.wikipedia.org/wiki/Ostrogradsky_instability> &#x2013; explanation why differential equations of orders higher than two do not appear in physics      [[math]] [[physics]] [[diffeq]]





## `[2021-01-31]` <http://www.scholarpedia.org/article/Ostrogradsky%27s_theorem_on_Hamiltonian_instability> more detailed explanation




# `[2020-01-15]` [Noether’s Theorem – A Quick Explanation (2019)](https://news.ycombinator.com/item?id=22033012)

<https://quantum-friend-theory.tumblr.com/post/172814384897/noethers-theorem-a-quick-explanation>  

