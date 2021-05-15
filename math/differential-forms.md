
# Table of Contents

-   [`[2018-11-24]` my thoughts on that](#mythghtsntht) 
-   [diffforms.pdf](#dfffrmspdf) [[study]]
    -   [a 1-diff form is an **expression** F(x, y) dx + G(x, y) dy](#dfffrmsnxprssnfxydxgxydy) 
    -   [total differential is an example of diff. form:](#ttldffrntlsnxmplfdfffrm) 
    -   [a diff form is similar to vector field](#dfffrmssmlrtvctrfld) 
    -   [a form is exact if it's a total differential of a scalar function](#frmsxctftsttldffrntlfsclrfnctn) 
    -   [closed &#x2013; if pF/py = pG/px](#clsdfpfpypgpx) 
    -   [exact means that integral is path independent!](#xctmnsthtntgrlspthndpndnt) 
        -   [this is sort of similar to complex analysis?](#thsssrtfsmlrtcmplxnlyss) 
    -   [wedge space: given vector space V:](#wdgspcgvnvctrspcv) 
    -   [2-form: an expression, built using wedges on pairs of 1-forms](#frmnxprssnbltsngwdgsnprsffrms) 
        -   [hmm. are all formal experessions looking like F dx<sup>dy</sup> + G dx<sup>dz</sup> + H dy<sup>dz</sup> looking like that??](#hmmrllfrmlxprssnslknglkfdxdygdxdzhdydzlknglktht) 
    -   [rules for derivative:](#rlsfrdrvtv) 
    -   [orientation: for a curve, direction; for a surface &#x2013; normal direction](#rnttnfrcrvdrctnfrsrfcnrmldrctn) 
        -   [so basically, by definition: integral of 2-form would be](#sbscllybydfntnntgrlffrmwldb) 
        -   [what would it mean to eval surface integral of dx ^ dy + dx ^ dz + dy ^ dz over a sphere?](#whtwldtmntvlsrfcntgrlfdxdydxdzdydzvrsphr) 
        -   [ah! so it's actually a flux: int int<sub>S</sub> F \dot dS = &int; int<sub>S</sub> F<sub>1</sub> dy<sup>dz</sup> + F<sub>2</sub> dz ^ dx + F<sub>3</sub> dx ^ dy](#hstsctllyflxntntsfdtdsntntsfdydzfdzdxfdxdy) 
        -   [NOTE arclength is NOT a differential form (always > 0)](#ntrclngthsntdffrntlfrmlwys) 
        -   [the manifold has to be parameterised for defining diff forms (or at least, for defining integrals?)](#thmnfldhstbprmtrsdfrdfnngdfffrmsrtlstfrdfnngntgrls) 
    -   [page 50: Maxwell's equations. EM field is a 2-form](#pgmxwllsqtnsmfldsfrm) 
-   [https://en.wikipedia.org/wiki/Differential\_form#Intrinsic\_definitions](#snwkpdrgwkdffrntlfrmntrnscdfntns) 
    -   [By the universal property of exterior powers, this is equivalently an alternating multilinear map](#bythnvrslprprtyfxtrrpwrstssqvlntlynltrntngmltlnrmp) 
-   [`[2018-11-06]`  differential forms ^ : wedge/exterior product](#dffrntlfrmswdgxtrrprdct) 
    -   [do in agda?&#x2026;](#dngd) [[agda]]
-   [`[2018-11-25]` ok, so diff forms are special types of tensors. Not all tensors are diff forms](#ksdfffrmsrspcltypsftnsrsntlltnsrsrdfffrms) [[tensor]]
-   [`[2018-11-14]` calculus - What does \(dx\) mean in differential form? - Mathematics Stack Exchange](#clclswhtdsdxmnndffrntlfrmmthmtcsstckxchng) 
    -   [right, here it's a 1-form! so no concerns about antisymmetry etc..](#rghthrtsfrmsncncrnsbtntsymmtrytc) 
    -   [ok, but what if it was curvilinear? What would dx mean then??](#kbtwhtftwscrvlnrwhtwlddxmnthn) 
-   [what are the other examples of 1-forms?](#whtrththrxmplsffrms) 
    -   [gradient &#x2013; ok, definitely pretty intuitive](#grdntkdfntlyprttynttv) 
        -   [hmm. gradient is a vector and total derivative is covector?? https://math.stackexchange.com/questions/47618/definition-of-the-gradient-for-non-cartesian-coordinates](#hmmgrdntsvctrndttldrvtvsctnfthgrdntfrnncrtsncrdnts) 
        -   [The 1-form ̃dfsuch that for any infinites-imally small vectordxfromTp ̃df(dx) =df(3.5)is called the gradient at point P    . ok &#x2013; that makes way more sense!](#thfrm̃dfschthtfrnynfntsmlhgrdnttpntpkthtmkswymrsns) 
        -   [dual 1-form. dual covector field for vector field; is that a thing???](#dlfrmdlcvctrfldfrvctrfldsthtthng) 
        -   [ugh. I guess alla of them are basically derivatives since well.. there isn't much else apart of derivatives there and they form complete basis](#ghgssllfthmrbscllydrvtvssdrvtvsthrndthyfrmcmpltbss) 
-   [some intuitive stuff from NotesOnVectors.pdf](#smnttvstfffrmntsnvctrspdf) 
-   [`[2018-11-10]` Дифференциал (дифференциальная геометрия) — Википедия https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D1%84%D1%84%D0%B5%D1%80%D0%B5%D0%BD%D1%86%D0%B8%D0%B0%D0%BB\_(%D0%B4%D0%B8%D1%84%D1%84%D0%B5%D1%80%D0%B5%D0%BD%D1%86%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F\_%D0%B3%D0%B5%D0%BE%D0%BC%D0%B5%D1%82%D1%80%D0%B8%D1%8F)](#дифференциалдифференциальcdbddbdfdbdbdbdbcdbdddbdf) 
-   [`[2018-11-10]` differentiation in nLab https://ncatlab.org/nlab/show/differentiation](#dffrnttnnnlbsnctlbrgnlbshwdffrnttn) 
-   [`[2018-11-18]` differential geometry - What is a covector and what is it used for? - Mathematics Stack Exchange](#dffrntlgmtrywhtscvctrndwhtstsdfrmthmtcsstckxchng) 
-   [`[2018-11-24]` Closed and exact differential forms - Wikipedia](#clsdndxctdffrntlfrmswkpd) 
-   [`[2019-01-24]` A Visual Introduction to Differential Forms and Calculus on Manifolds | Jon Pierre Fortney | Springer](#vslntrdctntdffrntlfrmsndclsnmnfldsjnprrfrtnysprngr) [[viz]]
    -   [`[2019-06-12]` ok, so illustrations are ok and there are many of them. explanations seemed ok as well I guess](#ksllstrtnsrkndthrrmnyfthmxplntnssmdkswllgss) 





# `[2018-11-24]` my thoughts on that

    so basically, treat dx, dy as formal symbols? you can multiply them by scalar, add them up
    NOTE in agda it would be just n-form with ordered requirement? or just a subset?




# diffforms.pdf       [[study]]





## a 1-diff form is an **expression** F(x, y) dx + G(x, y) dy




## total differential is an example of diff. form:

df = pf/px dx + pf/py dy  




## a diff form is similar to vector field




## a form is exact if it's a total differential of a scalar function




## closed &#x2013; if pF/py = pG/px

exact impllies closed, but not in reverse  




## exact means that integral is path independent!





### this is sort of similar to complex analysis?




## wedge space: given vector space V:

wedge rules: v<sup>u</sup> = -u<sup>v</sup>; u ^ u = 0; and linearity  
build the space: \Wedge<sup>2</sup> V = {Sum<sub>i</sub> u<sub>i</sub> ^ v<sub>i</sub> | u<sub>i</sub> ^ v<sub>i</sub> | u<sub>i</sub>, v<sub>i</sub> in V} are imposed  




## 2-form: an expression, built using wedges on pairs of 1-forms





### hmm. are all formal experessions looking like F dx<sup>dy</sup> + G dx<sup>dz</sup> + H dy<sup>dz</sup> looking like that??




## rules for derivative:

linearity  
d(f alpha) = df ^ alpha + f d alpha  
d (dx) = d (dy) = d(dz) = 0 # TODO hmm what does that one mean??  




## orientation: for a curve, direction; for a surface &#x2013; normal direction

  basically, **continuous** normal field. If it exists, there are two of them: n and minus n  
parameterise the surface by two coordinates u, v so that du ^ dv is the direction of normal  




### so basically, by definition: integral of 2-form would be

int F dx<sup>dy</sup> + G dy<sup>dz</sup> + H dz ^dx = int int [ F p(x, y)/p(u, v) + G p(y, z)/p(u, v) + H p(z, x)/p(u, v)] du dv  




### what would it mean to eval surface integral of dx ^ dy + dx ^ dz + dy ^ dz over a sphere?




### ah! so it's actually a flux: int int<sub>S</sub> F \dot dS = &int; int<sub>S</sub> F<sub>1</sub> dy<sup>dz</sup> + F<sub>2</sub> dz ^ dx + F<sub>3</sub> dx ^ dy




### NOTE arclength is NOT a differential form (always > 0)

but what we can do is to define a metric tensor  




### the manifold has to be parameterised for defining diff forms (or at least, for defining integrals?)




## page 50: Maxwell's equations. EM field is a 2-form




# <https://en.wikipedia.org/wiki/Differential_form#Intrinsic_definitions> 





## By the universal property of exterior powers, this is equivalently an alternating multilinear map

mm, I guess this bit is crucial to my understanding of alternating property  




# `[2018-11-06]`  differential forms ^ : wedge/exterior product

f(x, y, z) dx ^ dy ^ dx &#x2013; integrated over volume, gives volume  
d operation &#x2013; exterior derivative, results in k+1 form  

ok so treat dx, dy, dz formally in form expression  




## do in agda?&#x2026;      [[agda]]




# `[2018-11-25]` ok, so diff forms are special types of tensors. Not all tensors are diff forms      [[tensor]]

<https://en.wikipedia.org/wiki/Antisymmetric_tensor>  
a completely antisymmetric covariant tensor &#x2013; p-form; contravarian &#x2013; p-vector  
<https://en.wikipedia.org/wiki/Volume_form#Riemannian_volume_form>  




# `[2018-11-14]` calculus - What does \(dx\) mean in differential form? - Mathematics Stack Exchange

<https://math.stackexchange.com/questions/664648/what-does-dx-mean-in-differential-form/664674#664674>  
dx<sub>1</sub> is a differential 1-form, linear map acting on tangent space. Action is: (1, 0, &#x2026;. 0)  

dx<sub>i</sub> is a covector field. {dx<sub>i</sub>}<sub>i</sub> span all covector fields. For f &isin; R<sup>n</sup> -> R, you can write df =  [f<sub>1</sub>(x) f<sub>2</sub>(x) .. f<sub>n</sub>(x)] as f<sub>1</sub>(x) dx<sub>1</sub> + &#x2026; + f<sub>n</sub>(x) dx<sub>n</sub>  
in that sense, dx<sub>1</sub> is the derivative of coordinate function f(x<sub>1&#x2026;x</sub><sub>n</sub>) = x<sub>1</sub>  




## right, here it's a 1-form! so no concerns about antisymmetry etc..

so, to compute the 1-form along the path, we:  
split the path gamma(t); t from 0 to 1 into k parts  
each part can be considered a tangent vector at gamma<sub>i</sub>, and plugged into the form. then sum up the numbers  




## ok, but what if it was curvilinear? What would dx mean then??




# what are the other examples of 1-forms?





## gradient &#x2013; ok, definitely pretty intuitive





### hmm. gradient is a vector and total derivative is covector?? <https://math.stackexchange.com/questions/47618/definition-of-the-gradient-for-non-cartesian-coordinates>

hence gradient depends on metric  
ok, so I guess definition might involve coordinates; but otherwise they are coordinate free once we prove they transform properly  




### The 1-form ̃dfsuch that for any infinites-imally small vectordxfromTp ̃df(dx) =df(3.5)is called the gradient at point P    . ok &#x2013; that makes way more sense!




### dual 1-form. dual covector field for vector field; is that a thing???




### ugh. I guess alla of them are basically derivatives since well.. there isn't much else apart of derivatives there and they form complete basis




# some intuitive stuff from NotesOnVectors.pdf

    Examples of how you can picture contravariant and covariant vectors. A contravari-ant vector is a “stick” with a direction to it.  Its “worth” (or “magnitude”) is proportional tothe length of the stick.  A covariant vector is like “lasagna.”  Its worth is proportional to thedensity of noodles; that is, the closer together are the sheets, the larger is the magnitude ofthe covector.  These and other pictorial examples of visualizing contravariant and covariantvectors are discussed in Am.J.Phys.65(1997)1037.Figure  3:   Pictorial  representation  of  the  innerproduct between a contravariant vector and a co-variant  vector.   The  “stick”  is  imbedded  in  the“lasagna”  and  the  inner  product  is  equal  to  thenumber of noodles pierced by the stick.  The in-ner product shown has the value 5.




# `[2018-11-10]` Дифференциал (дифференциальная геометрия) — Википедия <https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D1%84%D1%84%D0%B5%D1%80%D0%B5%D0%BD%D1%86%D0%B8%D0%B0%D0%BB_(%D0%B4%D0%B8%D1%84%D1%84%D0%B5%D1%80%D0%B5%D0%BD%D1%86%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F_%D0%B3%D0%B5%D0%BE%D0%BC%D0%B5%D1%82%D1%80%D0%B8%D1%8F)>

    Пусть {\displaystyle M} M — гладкое многообразие и {\displaystyle f\colon M\to \mathbb {R} } {\displaystyle f\colon M\to \mathbb {R} } гладкая функция. Дифференциал {\displaystyle f} f представляет собой 1-форму на {\displaystyle M} M, обычно обозначается {\displaystyle df} df и определяется соотношением
    {\displaystyle df(X)=d_{p}f(X)=Xf,} {\displaystyle df(X)=d_{p}f(X)=Xf,}
    где {\displaystyle Xf} Xf обозначает производную {\displaystyle f} f по направлению касательного вектора {\displaystyle X} X в точке {\displaystyle p\in M} p\in M.

hmm, that actually makes sense too!  




# `[2018-11-10]` differentiation in nLab <https://ncatlab.org/nlab/show/differentiation>

    1. Idea
    Differentiation is the process that assigns to a function f:X→Y f : X \to Y its derivative, sometimes denoted df d f. The derivative is a function that, roughly speaking, assigns to each point x∈X x \in X the linear transformation dfx d f_x that maps infinitesimal differences y−x y - x (for points y y infinitesimally close to x x) to infinitesimal differences f(y)−f(x) f(y) - f(x).




# `[2018-11-18]` differential geometry - What is a covector and what is it used for? - Mathematics Stack Exchange

<https://math.stackexchange.com/questions/240491/what-is-a-covector-and-what-is-it-used-for>  




# `[2018-11-24]` Closed and exact differential forms - Wikipedia

<https://en.wikipedia.org/wiki/Closed_and_exact_differential_forms>   

     In mathematics, especially vector calculus and differential topology, a closed form is a differential form α whose exterior derivative is zero (dα = 0), and an exact form is a differential form, α, that is the exterior derivative of another differential form β. Thus, an exact form is in the image of d, and a closed form is in the kernel of d.
    
    For an exact form α, α = dβ for some differential form β of degree one less than that of α. The form β is called a "potential form" or "primitive" for α. Since the exterior derivative of a closed form is zero, β is not unique, but can be modified by the addition of any closed form of degree one less than that of α.
    
    Because d2 = 0, any exact form is necessarily closed. The question of whether every closed form is exact depends on the topology of the domain of interest. On a contractible domain, every closed form is exact by the Poincaré lemma. More general questions of this kind on an arbitrary differentiable manifold are the subject of de Rham cohomology, which allows one to obtain purely topological information using differential methods.




# `[2019-01-24]` A Visual Introduction to Differential Forms and Calculus on Manifolds | Jon Pierre Fortney | Springer      [[viz]]

-   State "START"      from "TODO"       `[2019-02-27]`

<https://www.springer.com/us/book/9783319969916>  




## `[2019-06-12]` ok, so illustrations are ok and there are many of them. explanations seemed ok as well I guess

