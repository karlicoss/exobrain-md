
# Table of Contents

-   [related](#rltd) [[math]] [[qft]]
-   [Definitions & theorems](#dfntnsthrms) 
    -   [subrepresentation W &#x2013; vector subspace of V invariant under G.](#sbrprsnttnwvctrsbspcfvnvrntndrg) 
    -   [trivial subrepr &#x2013; V and {0}.](#trvlsbrprvnd) 
    -   [irreducible &#x2013; no nontrival subrepr](#rrdcblnnntrvlsbrpr) 
    -   [group center &#x2013; elements that are commuting with every other element](#grpcntrlmntsthtrcmmtngwthvrythrlmnt) 
    -   [inner automorphism &#x2013; conjugation with group element f<sub>a</sub>(g) = a g a<sup>-1</sup>](#nnrtmrphsmcnjgtnwthgrplmntfgg) 
    -   [Schur's lemma - only useful for complex reprs (relies on eigenvalue existence)](#schrslmmnlysflfrcmplxrprsrlsngnvlxstnc) 
    -   [commutative G &#x2013; all irrep are one dimensional](#cmmttvgllrrprndmnsnl) 
-   [U(1)](#1412_1817) 
    -   [U(1) &#x2013; rotations e<sup>i</sup> theta](#rttnstht) 
    -   [all irrep of U(1) are unitary; pi<sub>k</sub> : exp(i theta) -> exp(i k theta), k in Z.](#llrrpfrntrypkxpthtxpkthtknz) 
-   [`[2018-09-05]` Woit book is quite elaborate. Ugh, it's all very hard :(](#wtbksqtlbrtghtsllvryhrd) 
    -   [`[2019-01-20]`  SU 2 (chapter 3)](#schptr) 
        -   [some annotations in Polar](#smnnttnsnplr) 
    -   [`[2019-01-20]` chapter 5. .. skipped it for now](#chptrskppdtfrnw) 
    -   [Spin(3) = Sp(1), unitary quaternions](#spnspntryqtrnns) 
    -   [`[2019-01-23]`  chapter 10.2.1](#chptr) 
-   [SU(2)](#s) 
    -   [Representation theory of SU(2) - Wikipedia](#rprsnttnthryfswkpd) 
        -   [right, so reprs of SU 2 are actually found by considering su(2) reprs? similar to what woit was doing, yep. explains choice of pauli matrices as well](#rghtsrprsfsrctllyfndbycnsdngypxplnschcfplmtrcsswll) 
    -   [SU(n) &#x2013; n dim matrices with det equal to 1](#snndmmtrcswthdtqlt) 
        -   [SU(2) = ((a, -b\*), (b\*, a)); norm(a)<sup>2</sup> + norm(b)<sup>2</sup> = 1](#sbbnrmnrmb) 
    -   [SU(2). for C<sup>2</sup> self adjoint operators are always expressed in terms of Pauli matrices](#sfrcslfdjntprtrsrlwysxprssdntrmsfplmtrcs) 
    -   [Symmetry in quantum mechanics - Wikipedia](#symmtrynqntmmchncswkpd) [[symmetry]]
        -   [`[2018-09-06]`](#4220_4713) 
        -   [`[2018-09-06]`](#4713_5058) 
        -   [`[2018-09-06]`](#5058_5361) 
        -   [`[2019-01-23]` Representation of a Lie group - Wikipedia](#rprsnttnflgrpwkpd) [[lie]]
    -   [Spinors](#spnrs) [[spinor]]
        -   [`[2019-02-07]` Spinors, on the other hand, are constructed in such a way that makes them sensitive to how the gradual rotation of the coordinates arrived there: they exhibit path-dependence. It turns out that, for any final configuration of the coordinates, there are actually two ("topologically") inequivalent gradual (continuous) rotations of the coordinate system that result in this same configuration. This ambiguity is called the homotopy class of the gradual rotation](#spnrsnththrhndrcnstrctdnslldthhmtpyclssfthgrdlrttn) 
        -   [`[2019-02-07]` This group acts by conjugation on the real vector space spanned by the Pauli matrices themselves,[nb 12] realizing it as a group of rotations among them,[nb 13] but it also acts on the column vectors (that is, the spinors).](#thsgrpctsbycnjgtnnthrlvcttsnthclmnvctrsthtsthspnrs) 
        -   [`[2019-02-07]` onetheless, the concept is generally considered notoriously difficult to understand, as illustrated by Michael Atiyah's statement that is recounted by Dirac's biographer Graham Farmelo:](#nthlssthcncptsgnrllycnsdrrcntdbydrcsbgrphrgrhmfrml) 
        -   [`[2019-02-07]` What is a spinor? - Physics Stack Exchange](#whtsspnrphyscsstckxchng) 
        -   [`[2019-01-14]` Plate trick - Wikipedia](#plttrckwkpd) [[viz]]
        -   [`[2019-01-23]` Eigenspinor - Wikipedia](#gnspnrwkpd) 
-   [`[2019-01-23]` SO(3)](#s) 
-   [`[2019-01-20]`  misc stuff vvvvvvvvvvvvvvvv](#mscstffvvvvvvvvvvvvvvvv) 
-   [`[2019-01-20]` Irreducible representation - Wikipedia](#rrdcblrprsnttnwkpd) 
-   [`[2018-09-03]` representation theory of the lorenz group](#rprsnttnthryfthlrnzgrp) [[reprtheory]]
-   [`[2018-08-25]` symmetry groups](#symmtrygrps) [[symmetry]]
    -   [I encourage everyone to learn the derivation of Schrödinger's equation straight from the representation theory of the Galilei group! It's cool.](#ncrgvryntlrnthdrvtnfschrörprsnttnthryfthgllgrptscl) 
-   [`[2018-11-16]` Representation Theory](#rprsnttnthry) 
-   [`[2018-09-03]`  This holds in particular for any representation of a finite group over the complex numbers, since the characteristic of the complex numbers is zero, which never divides the size of a group.](#thshldsnprtclrfrnyrprsnttbrsszrwhchnvrdvdsthszfgrp) [[reprtheory]]
-   [`[2018-11-10]` Introduction to gauge theory - Wikipedia](#ntrdctntggthrywkpd) [[reprtheory]] [[symmetry]]
    -   [`[2019-01-10]`  Suppose that there existed some process by which one could briefly violate conservation of charge by creating a charge q at a certain point in space, 1, moving it to some other point 2, and then destroying it. We might imagine that this process was consistent with conservation of energy. We could posit a rule stating that creating the charge required an input of energy E1=qV1 and destroying it released E2=qV2, which would seem natural since qV measures the extra energy stored in the electric field because of the existence of a charge at a certain point. Outside of the interval during which the particle exists, conservation of energy would be satisfied, because the net energy released by creation and destruction of the particle, qV2-qV1, would be equal to the work done in moving the particle from 1 to 2, qV2-qV1. But although this scenario salvages conservation of energy, it violates gauge symmetry. Gauge symmetry requires that the laws of physics be invariant under the transformation {\displaystyle V&rarr; V+C} V&rarr; V+C, which implies that no experiment should be able to measure the absolute potential, without reference to some external standard such as an electrical ground. But the proposed rules E1=qV1 and E2=qV2 for the energies of creation and destruction would allow an experimenter to determine the absolute potential, simply by comparing the energy input required to create the charge q at a particular point in space in the case where the potential is {\displaystyle V} V and {\displaystyle V+C} V+C respectively. The conclusion is that if gauge symmetry holds, and energy is conserved, then charge must be conserved.[1](#sppsthtthrxstdsmprcssbywhyscnsrvdthnchrgmstbcnsrvd) 
    -   [`[2019-01-10]`](#14087_14758) 
    -   [`[2019-01-10]`](#14758_15659) 
    -   [`[2019-01-10]` uu, nice demo for Aharonov-Bohm effect!](#ncdmfrhrnvbhmffct) 
-   [unitary repr pi(g) = e<sup>A</sup> for g close to identity A\* = -A, skew symetric, but B=iA &#x2013; self adjoint!](#ntryrprpgfrgclstdnttyskwsymtrcbtbslfdjnt) 
    -   [time translation: representation of R (additive). pi(t) = exp(-i/h H t). Hamiltonian!](#tmtrnsltnrprsnttnfrddtvptxphhthmltnn) 
-   [any unitary repr is a direct sum of irrep](#nyntryrprsdrctsmfrrp) 
    -   [non unitary counterexample:](#nnntrycntrxmpl) 
-   [Baez lie groups throught examples](#bzlgrpsthrghtxmpls) [[lie]] [[math]] [[physics]]
    -   [`[2018-10-09]` ok hold on for now; he assumes we know what's a lie algebra, etc..](#khldnfrnwhssmswknwwhtsllgbrtc) 
-   [`[2018-09-11]` http://blog.sigfpe.com/2007/11/whats-all-this-e8-stuff-about-then-part.html](#blgsgfpcmwhtsllthsstffbtthnprthtml) 
-   [lie groups course](#lgrpscrs) [[lie]] [[physics]]
    -   [Brian Hall Lie groups lie algebras and representations (Baez recommendation)](#brnhlllgrpsllgbrsndrprsnttnsbzrcmmndtn) 
        -   [`[2018-10-18]` p.4. matrix Lie group &#x2013; closed subgroup of general linear.](#pmtrxlgrpclsdsbgrpfgnrllnr) 
    -   [Fulton representation theory (Baez recommended)](#fltnrprsnttnthrybzrcmmndd) 
-   [lie groups nlab](#lgrpsnlb) [[lie]]
-   [Symmetry in quantum mechanics - Wikipedia](#symmtrynqntmmchncswkpd) 
-   [`[2018-10-09]`  people also recommend Duistermaat-Kolk: Lie Groups.](#ppllsrcmmnddstrmtklklgrps) 
-   [going through liegroups.pdf file:study/reprtheory/liegroups.pdf](#gngthrghlgrpspdfflstdyrprthrylgrpspdf) 
    -   [`[2018-10-09]`  trying to prove that identity connected component of a lie group is a normal  subgroup and a lie group](#tryngtprvthtdnttycnnctdcmpnntflgrpsnrmlsbgrpndlgrp) 
        -   [why it's a group](#whytsgrp) 
        -   [why is it normal](#whystnrml) 
        -   [why is it a lie group. well trivial I suppose? continuity etc is induced](#whystlgrpwlltrvlsppscntntytcsndcd) 
        -   [why quotient is discrete???](#whyqtntsdscrt) 
        -   [It's theorem is useful; we essentially split study of lie groups into discrete groups and connected. he mentions we can further simplify and study simply connected.](#tsthrmssflwssntllyspltstdhrsmplfyndstdysmplycnnctd) 
    -   [`[2018-10-15]` carrying on&#x2026;](#crryngn) 
        -   [ok, I'm a bit stuck at understanding topologocal continuity again I think. shame :(](#kmbtstcktndrstndngtplgclcntntygnthnkshm) 
        -   [I thhink I got an intuition for quotient space topology. basically: we map X to X/~. So, to derive topoplogy for quotient space, let's just assume ~ is continuous. then we'd naturally want open subsets in quotient space to be the ones with open preimage](#thhnkgtnnttnfrqtntspctplgtsnqtntspctbthnswthpnprmg) 
    -   [`[2018-10-18]` carrying on&#x2026; quotient topology is discrete](#crryngnqtnttplgysdscrt) 
        -   [The connected components are always closed (but in general not open) (from wiki). errrr](#thcnnctdcmpnntsrlwysclsdbtngnrlntpnfrmwkrrrr) 
    -   [cover, universal cover&#x2026;](#cvrnvrslcvr) 
        -   [nice intuition about Riemann sheets https://math.stackexchange.com/a/95331/15108](#ncnttnbtrmnnshtssmthstckxchngcm) 
        -   [https://math.stackexchange.com/questions/95302/covering-spaces-why-are-they-useful](#smthstckxchngcmqstnscvrngspcswhyrthysfl) 
        -   [universal cover: simply connected](#nvrslcvrsmplycnnctd) 
    -   [`[2018-10-18]` uh&#x2026; skipped to 2.4](#hskppdt) 
-   [Old&#x2026; v](#ldv) 
-   [С4 group](#сgrp) 
    -   [e, a, b, c = 1, i, -1, -i , complex numbers multiplication](#bccmplxnmbrsmltplctn) 
    -   [e, a, b, c = 0, 1, 2, 3   , addition modulo 4](#bcddtnmdl) 
    -   [matrix representation     , matrix multiplication](#mtrxrprsnttnmtrxmltplctn) 
    -   [geometric representation: marked square rotations](#gmtrcrprsnttnmrkdsqrrttns) 
-   [`[2018-09-11]` O(n) http://mathworld.wolfram.com/OrthogonalGroup.html](#nmthwrldwlfrmcmrthgnlgrphtml) 
    -   [O(p, q) &#x2013; preserves symplectic quadratic form with signature (p, q), e.g. Q(v, w) = Q(Av, Aw)](#pqprsrvssymplctcqdrtcfrmwthsgntrpqgqvwqvw) 
-   [`[2019-01-20]` misc](#msc) 
    -   [`[2018-08-26]` quantum field theory - Why particles are thought as irreducible representation in plain English? - Physics Stack Exchange](#qntmfldthrywhyprtclsrthghnnplnnglshphyscsstckxchng) 
    -   [`[2018-12-07]` Worked problems in physics using representation theory? : AskPhysics](#wrkdprblmsnphyscssngrprsnttnthryskphyscs) 
-   [. Wigner himself did a lot to improve the situation, writing a book entitled Group Theory and Its Application to the Quantum Mechanics of Atomic Spectra in 1931. It explained groups and representations in a language closer to that with which physicists were familiar.](#wgnrhmslfddlttmprvthsttnwtthtwthwhchphyscstswrfmlr) 
-   [`[2019-01-24]` Short Introduction to and Motivation for Representation Theory – Jakob Schwichtenberg](#shrtntrdctntndmtvtnfrrprsnttnthryjkbschwchtnbrg) [[reprtheory]]
-   [`[2019-01-24]` What’s so special about the adjoint representation of a Lie group? – Jakob Schwichtenberg](#whtssspclbtthdjntrprsnttnflgrpjkbschwchtnbrg) [[reprtheory]]
-   [`[2019-01-23]` Best intro to representation theory? /r/math](#srddtcmrmthcmmntskjwhbstnrkbstntrtrprsnttnthryrmth) 
-   [`[2019-01-23]` Representation Theory /r/math](#srddtcmrmthcmmntsmnmrprsnnthrycpyprprsnttnthryrmth) 
-   [`[2019-01-23]` Representation Theory /r/math](#srddtcmrmthcmmntsmnmrprsnthrycqrdlrprsnttnthryrmth) 
-   [`[2019-01-23]` Can Representation Theory be Explained Using Basic Abstract and Linear Algebra? /r/math](#srddtcmrmthcmmntstcnrprsnsngbscbstrctndlnrlgbrrmth) 
-   [`[2019-01-23]` Book suggestions for modern representation theory? /r/math](#srddtcmrmthcmmntscxbksggstnsfrmdrnrprsnttnthryrmth) 
-   [`[2019-01-23]` Everything about Representation theory of finite groups /r/math](#srddtcmrmthcmmntsxsvrythntrprsnttnthryffntgrpsrmth) 
-   [`[2019-01-23]` Everything about Representation theory of finite groups /r/math](#srddtcmrmthcmmntsxsvrythntrprsnttnthryffntgrpsrmth) 
-   [`[2018-09-03]` grand unified theory resources](#grndnfdthryrsrcs) [[study]] [[reprtheory]]
-   [`[2020-08-03]` Eric Weinstein on Twitter: "You can call S<sup>3</sup> by all of the following names: S<sup>3</sup>, Spin(3), SU(2), Sp(1) only they lead to **different** generalizations. Unfortunately Spin(4)=SU(2)xSU(2) is seldom written Spin(4)=Sp(1)xS<sup>3</sup> which should be preferred. But why is one naming better? It‘s because it generalizes." / Twitter](#stwttrcmrcrwnstnsttsrcwnsnmngbttrtsbcstgnrlzstwttr) 
-   [`[2019-01-20]` Physics from Symmetry - Jakob Schwichtenberg - Google Books](#physcsfrmsymmtryjkbschwchtnbrggglbks) [[book]] [[reprtheory]]
-   [representations as monoids?](#rprsnttnssmnds) [[think]]
-   [`[2019-02-24]` Nikita Lisitsa on Twitter: "Representation theory of finite groups in action. Here are 3 lowest-energy orbitals of a hypothetical H₃²⁺ ion, with hydrogen nuclei arranged into a regular triangle. The permutation group S₃ acts on the system simply by permuting the nuclei. https://t.co/KvFsQVHuCG" / Twitter](#nktlstsntwttrrprsnttnthrytngthnclstckvfsqvhcgtwttr) 





# related       [[math]] [[qft]]




# Definitions & theorems

GL(V) &#x2013; group of linear maps of V (automorphisms, isomorphisms from group to itself)  
p is representation  
sometimes V is called a representation (if there is little ambiguity about the map onto it)  

gv = def =  p(g)(v) &#x2013; group action  

G-linear map &#x2013; map between representations V -> W, s.t g . phi and phi . g commute for all g  




## subrepresentation W &#x2013; vector subspace of V invariant under G.




## trivial subrepr &#x2013; V and {0}.




## irreducible &#x2013; no nontrival subrepr




## group center &#x2013; elements that are commuting with every other element




## inner automorphism &#x2013; conjugation with group element f<sub>a</sub>(g) = a g a<sup>-1</sup>




## Schur's lemma - only useful for complex reprs (relies on eigenvalue existence)




## commutative G &#x2013; all irrep are one dimensional




# U(1) 





## U(1) &#x2013; rotations e<sup>i</sup> theta




## all irrep of U(1) are unitary; pi<sub>k</sub> : exp(i theta) -> exp(i k theta), k in Z.

the sqlf adjoint operator is multiplication by k.  
integral k comes because of periodicity of unit circle, if it was R, it would be different  




# `[2018-09-05]` Woit book is quite elaborate. Ugh, it's all very hard :(





## `[2019-01-20]`  SU 2 (chapter 3)

ok, still unclear what is spin 0. it shouldn't change under coordinate transformations right, but what is it from the representation theory point of view??  




### some annotations in Polar




## `[2019-01-20]` chapter 5. .. skipped it for now




## Spin(3) = Sp(1), unitary quaternions

and Sp(1) = SU(2)  
SO(3) is kinda like S<sup>3</sup> but with opposite points of the sphere identified  




## `[2019-01-23]`  chapter 10.2.1

important point &#x2013; schrodinger equation  
i h d/dt |psi> = H |psi>  
(U(t), \H) is a representation of R in state space  




# SU(2) 





## Representation theory of SU(2) - Wikipedia

<https://en.m.wikipedia.org/wiki/Representation_theory_of_SU(2)>  




### right, so reprs of SU 2 are actually found by considering su(2) reprs? similar to what woit was doing, yep. explains choice of pauli matrices as well




## SU(n) &#x2013; n dim matrices with det equal to 1





### SU(2) = ((a, -b\*), (b\*, a)); norm(a)<sup>2</sup> + norm(b)<sup>2</sup> = 1


-   a, b &#x2013; complex hense a<sub>1</sub><sup>2</sup> + a)2<sup>2</sup> + b<sub>1</sub><sup>2</sup> + b<sub>2</sub><sup>2</sup> = 1, so 3-sphere

-   isomorphic to unit quaternions




## SU(2). for C<sup>2</sup> self adjoint operators are always expressed in terms of Pauli matrices

directions of spin &#x2013; one direction for each of the Pauli matrices  
observables give rise to representations  
exp(i theta Pauli<sub>j</sub>) = (cos theta) 1 + i Pauli<sub>j</sub> (sin theta)  
as theta goes from 0 to 2pi, exp traces a circle in the space of unitary 2x2 matrices, subgroup  
only for Pauli<sub>3</sub> it's diagonal. ugh, don't understand anything  




## Symmetry in quantum mechanics - Wikipedia      [[symmetry]]





### `[2018-09-06]` 

    The spin vector operator is denoted S ^ = ( S x ^ , S y ^ , S z ^ ) {\displaystyle {\widehat {\mathbf {S} }}=({\widehat {S_{x}}},{\widehat {S_{y}}},{\widehat {S_{z}}})} {\widehat {\mathbf {S} }}=({\widehat {S_{x}}},{\widehat {S_{y}}},{\widehat {S_{z}}}). The eigenvalues of its components are the possible outcomes (in units of ℏ {\displaystyle \hbar } \hbar ) of a measurement of the spin projected onto one of the basis directions.




### `[2018-09-06]` 

    Rotations (of ordinary space) about an axis a ^ {\displaystyle {\hat {\mathbf {a} }}} {\hat {\mathbf {a} }} through angle θ about the unit vector a ^ {\displaystyle {\hat {a}}} {\hat {a}} in space acting on a multicomponent wave function (spinor) at a point in space is represented by:




### `[2018-09-06]` 

    In relativistic quantum mechanics, wavefunctions are no longer single-component scalar fields, but now 2(2s + 1) component spinor fields, where s is the spin of the particle. The transformations of these functions in spacetime are given below.




### `[2019-01-23]` Representation of a Lie group - Wikipedia      [[lie]]

<https://en.wikipedia.org/wiki/Representation_of_a_Lie_group#An_example:_The_rotation_group_SO.283.29>  

    ne subtlety of this analysis is that the representations of the group and the Lie algebra are not in one-to-one correspondence, a point that is critical in understanding the distinction between integer spin and half-integer spin.




## Spinors       [[spinor]]

from wiki:  




### `[2019-02-07]` Spinors, on the other hand, are constructed in such a way that makes them sensitive to how the gradual rotation of the coordinates arrived there: they exhibit path-dependence. It turns out that, for any final configuration of the coordinates, there are actually two ("topologically") inequivalent gradual (continuous) rotations of the coordinate system that result in this same configuration. This ambiguity is called the homotopy class of the gradual rotation




### `[2019-02-07]` This group acts by conjugation on the real vector space spanned by the Pauli matrices themselves,[nb 12] realizing it as a group of rotations among them,[nb 13] but it also acts on the column vectors (that is, the spinors).




### `[2019-02-07]` onetheless, the concept is generally considered notoriously difficult to understand, as illustrated by Michael Atiyah's statement that is recounted by Dirac's biographer Graham Farmelo:

No one fully understands spinors. Their algebra is formally understood but their general significance is mysterious. In some sense they describe the "square root" of geometry and, just as understanding the square root of −1 took centuries, the same might be true of spinors.[11]  




### `[2019-02-07]` What is a spinor? - Physics Stack Exchange

A spinor is a mathematical representation of a harmonic standing-wave quantum field "topological structure" or excitation which typically exhibits a spin ½ geometry  




### `[2019-01-14]` Plate trick - Wikipedia      [[viz]]

<https://en.wikipedia.org/wiki/Plate_trick>  




### `[2019-01-23]` Eigenspinor - Wikipedia

<https://en.wikipedia.org/wiki/Eigenspinor>  




# `[2019-01-23]` SO(3)

<https://en.wikipedia.org/wiki/3D_rotation_group#Topology>  
mmm.. proof of no simple connectedness is a bit tricky&#x2026;  
the antipodal points argument &#x2013; dunno, if the points are same why can't we just contract it? it's not intuitive at all!  

Maybe the intuition with torus works? But the torus is more of a long pipe  




# `[2019-01-20]`  misc stuff vvvvvvvvvvvvvvvv




# `[2019-01-20]` Irreducible representation - Wikipedia

<https://en.wikipedia.org/wiki/Irreducible_representation>  

    In quantum physics and quantum chemistry, each set of degenerate eigenstates of the Hamiltonian operator comprises a vector space V for a representation of the symmetry group of the Hamiltonian, a "multiplet", best studied through reduction to its irreducible parts. Identifying the irreducible representations therefore allows one to label the states, predict how they will split under perturbations; or transition to other states in V. Thus, in quantum mechanics, irreducible representations of the symmetry group of the system partially or completely label the energy levels of the system, allowing the selection rules to be determined.[5]




# `[2018-09-03]` representation theory of the lorenz group      [[reprtheory]]

<https://en.wikipedia.org/wiki/Representation_theory_of_the_Lorentz_group>  




# `[2018-08-25]` symmetry groups      [[symmetry]]

what is the meaning of symmetry? I guess that the actually observed values are unchanged  

<http://math.ucr.edu/home/baez/symmetries.html>  
E(N) - eucledean group, symmetries of n dimensional eucledean space  

-   E(2)  
    hmm he calls it 3 dimensional group. It's cause of degrees of freedom I suppose?  
    x shift  
    y shift  
    xy rotation

-   E(3)  
    z shift  
    xz rotation  
    yz rotation
-   laws of physics are not changing with time, E(3)+R &#x2013; naive spacetime symmetries  
    t shift
-   Galilei transformations: x -> x + vt  
    x, y, z galilei transformation  
    10 dimensional so far  
    symmetries of classical mechanics  
    Galilei boost is translation in momentum space &#x2013; makes sense
-   Poincare transformations &#x2013; instead, t -> cosh(s) t + sinh(s) x, x -> sinh(s) t + cosh(s) x; s is 'rapidity', v = tanh s; c = 1  
    10 dimensional as well!  
    <http://math.ucr.edu/home/baez/boosts.html> &#x2013; boosts symmetries  
    TODO eh, still didn't fully get it. Should work out by myself.
-   Maxwell equations are also symmetric under scaling (x -> ax, y->ay, z->az, t -> at). Weyl group (11 degrees)  
    only massless particles are invariant!

A representation of a group is a way to think of its elements as operators, and this is what we need to understand symmetries in quantum physics.  




## I encourage everyone to learn the derivation of Schrödinger's equation straight from the representation theory of the Galilei group! It's cool.

The mathematical foundations of quantum physics:  
Josef M. Jauch, Foundations of Quantum Mechanics, Addison-Wesley, 1968. (Very thoughtful and literate. Get a taste of quantum logic.)  
George Mackey, The Mathematical Foundations of Quantum Mechanics, Dover, New York, 1963. (Especially good for mathematicians who only know a little physics.)  




# `[2018-11-16]` Representation Theory

<https://www.math.columbia.edu/~woit/RepThy/>  




# `[2018-09-03]`  This holds in particular for any representation of a finite group over the complex numbers, since the characteristic of the complex numbers is zero, which never divides the size of a group.      [[reprtheory]]




# `[2018-11-10]` Introduction to gauge theory - Wikipedia      [[reprtheory]] [[symmetry]]

<https://en.wikipedia.org/wiki/Introduction_to_gauge_theory>  




## `[2019-01-10]`  Suppose that there existed some process by which one could briefly violate conservation of charge by creating a charge q at a certain point in space, 1, moving it to some other point 2, and then destroying it. We might imagine that this process was consistent with conservation of energy. We could posit a rule stating that creating the charge required an input of energy E1=qV1 and destroying it released E2=qV2, which would seem natural since qV measures the extra energy stored in the electric field because of the existence of a charge at a certain point. Outside of the interval during which the particle exists, conservation of energy would be satisfied, because the net energy released by creation and destruction of the particle, qV2-qV1, would be equal to the work done in moving the particle from 1 to 2, qV2-qV1. But although this scenario salvages conservation of energy, it violates gauge symmetry. Gauge symmetry requires that the laws of physics be invariant under the transformation {\displaystyle V&rarr; V+C} V&rarr; V+C, which implies that no experiment should be able to measure the absolute potential, without reference to some external standard such as an electrical ground. But the proposed rules E1=qV1 and E2=qV2 for the energies of creation and destruction would allow an experimenter to determine the absolute potential, simply by comparing the energy input required to create the charge q at a particular point in space in the case where the potential is {\displaystyle V} V and {\displaystyle V+C} V+C respectively. The conclusion is that if gauge symmetry holds, and energy is conserved, then charge must be conserved.[1

huh, that' very interesting point!!  

interesting, also in sense it's similar to comparing absolute units and diferernces as differet times! (datetime vs timesdelta). I wonder if this can somehow aid understanding??  

not sure if it's very convincing, e.g. proposed rules are pretty arbitrary  




## `[2019-01-10]` 

Not only that, but it is not even necessary to change the speed of each clock by a fixed amount. We could change the angle of the hand on each clock by a varying amount θ, where θ could depend on both the position in space and on time. This would have no effect on the result of the experiment, since the final observation of the location of the electron occurs at a single place and time, so that the phase shift in each electron's "clock" would be the same, and the two effects would cancel out. This is another example of a gauge transformation: it is local, and it does not change the results of experiments.  




## `[2019-01-10]` 

As a way of visualizing the choice of a gauge, consider whether it is possible to tell if a cylinder has been twisted. If the cylinder has no bumps, marks, or scratches on it, we cannot tell. We could, however, draw an arbitrary curve along the cylinder, defined by some function θ(x), where x measures distance along the axis of the cylinder. Once this arbitrary choice (the choice of gauge) has been made, it becomes possible to detect it if someone later twists the cylinde  

In 1954, Chen Ning Yang and Robert Mills proposed to generalize these ideas to noncommutative groups. A noncommutative gauge group can describe a field that, unlike the electromagnetic field, interacts with itself. For example, general relativity states that gravitational fields have energy, and special relativity concludes that energy is equivalent to mass.  




## `[2019-01-10]` uu, nice demo for Aharonov-Bohm effect!

<https://www.youtube.com/watch?v=OgDPK5MLVnE>  
so it gets global phase shift?  




# unitary repr pi(g) = e<sup>A</sup> for g close to identity A\* = -A, skew symetric, but B=iA &#x2013; self adjoint!

lie group actions provide us with observables many of which happen to be of physical interest  




## time translation: representation of R (additive). pi(t) = exp(-i/h H t). Hamiltonian!




# any unitary repr is a direct sum of irrep





## non unitary counterexample:

C<sup>2</sup>, upper triangular matrices W = k (1 0) for k in C is a subrepr, but there is no complement  




# Baez lie groups throught examples      [[lie]] [[math]] [[physics]]





## `[2018-10-09]` ok hold on for now; he assumes we know what's a lie algebra, etc..

<http://math.ucr.edu/home/baez/qg-fall2008/>  
<https://golem.ph.utexas.edu/category/2008/09/lie_theory_through_examples_1.html>  
<http://math.ucr.edu/home/baez/qg-fall2008/lie1.pdf>  




# `[2018-09-11]` <http://blog.sigfpe.com/2007/11/whats-all-this-e8-stuff-about-then-part.html>

lie algebras describe rate of change of element of lie group, they are not wrapping around!  




# lie groups course      [[lie]] [[physics]]

<http://math.ucr.edu/home/baez/lie/lie.html>  
eh, can't say I understood much&#x2026;  

<https://math.stackexchange.com/a/1823425/15108> &#x2013; so(3) are skew symmetric matrices  




## Brian Hall Lie groups lie algebras and representations (Baez recommendation)





### `[2018-10-18]` p.4. matrix Lie group &#x2013; closed subgroup of general linear.

SO group: A\* = A<sup>(-1)</sup>  
SO is subgroup of O  
UGH . stuck here. too sleepy I suppose.  




## Fulton representation theory (Baez recommended)

hmm, still a bit too advanced&#x2026;  




# lie groups nlab      [[lie]]

<https://ncatlab.org/nlab/show/Lie+group>  
very elaborate stuff..  

should know  

-   general linear
-   orthogonal + special
-   unitary + special
-   symplectic

interesting things are  

-   loop group  
    -




# Symmetry in quantum mechanics - Wikipedia

The generators of the group are the partial derivatives of the group elements with respect to the group parameters with the result evaluated when the parameter is set to zero:  

X j = ∂ g ∂ ξ j | ξ j = 0 {\displaystyle X<sub>j</sub>=\left.{\frac {&part; g}{&part; &xi; \_{j}}}\right|<sub>&xi; \_{j}=0</sub>} X<sub>j</sub>=\left.{\frac {&part; g}{&part; &xi; \_{j}}}\right|<sub>&xi; \_{j}=0</sub>  

In the language of manifolds, the generators are the elements of the tangent space to G at the identity. The generators are also known as infinitesimal group elements or as the elements of the Lie algebra of G. (See the discussion below of the commutator.)  




# `[2018-10-09]`  people also recommend Duistermaat-Kolk: Lie Groups.




# going through liegroups.pdf <study/reprtheory/liegroups.pdf>





## `[2018-10-09]`  trying to prove that identity connected component of a lie group is a normal  subgroup and a lie group

first of all &#x2013; shy is it normal.  

after that, through why is it a group at all&#x2026; need some understanding of connectedness in groups  




### why it's a group

use path connectedness for simplicity for now?  

e.g. if a is connected to 0  
ok, -a is kinda obvious? reverse path is still a path  

than means that for all delta exists {a<sub>1</sub> &#x2026; a<sub>N</sub>}, s.t. a<sub>1</sub> x &#x2026; x a<sub>n</sub> = a  
ams for b. than, for a + b just take N = N<sub>a</sub> + N<sub>b</sub> and  

ahh ok. path is a function from [0, 1] to space, s.t. p(0) = start, p(1) = end  
right, so p<sub>a</sub>(0) = 0, p<sub>a</sub>(1) = a; p<sub>b</sub>(0) = 0, p<sub>b</sub>(1) = b;  
then p<sub>(a+b)</sub>(t) = p<sub>a</sub>(t)  + p<sub>b</sub>(t). p(0) = 0; p(a + b) = a + b; the mapping is continuous since group operation is smooth  




### why is it normal

take any a in G<sub>0</sub> and g in G  
g a inv(g) &#x2014; ???  
there is a path in G<sub>0</sub> , so for t from 0 to 1 : g p(t) inv(g) &#x2014; ???  
not sure if that leads us somewhere&#x2026;  

ok, looked up the answer. it's pretty trivial; connected space is connected under a cont. map; since conjugation is continuous, it maps onto a connected space. since it maps identity into identity, that connected space is G<sub>0</sub>.  
eh, I'm an idiot. actually, my path approach does solve it, just literally notice that p<sub>b</sub>(t) = g p<sub>a</sub>(t) inv(g) is a continuous map connecting 0 with some point.  

<https://math.stackexchange.com/a/511184/15108>  
<https://topospaces.subwiki.org/wiki/Connected_component>  




### why is it a lie group. well trivial I suppose? continuity etc is induced




### why quotient is discrete???


-   need to understand what quotient space topology is

    <https://en.wikipedia.org/wiki/Quotient_space_(topology)>  




### It's theorem is useful; we essentially split study of lie groups into discrete groups and connected. he mentions we can further simplify and study simply connected.




## `[2018-10-15]` carrying on&#x2026;





### ok, I'm a bit stuck at understanding topologocal continuity again I think. shame :(

ok, so let's build a counterexample. suppose there is an O<sub>Y</sub>, that preimage of O<sub>Y</sub> is not open. (trivial example: X = trivial topology; Y = discrete topology). And f is identity  

-   <https://math.stackexchange.com/a/2686384/15108> aha, they are continuous iff finer actuok, but what's the intuition?

    so all functions from discrete topology are continuous&#x2026;. ok, but what's the intuition?  

-   <https://math.stackexchange.com/questions/658305/continuous-mapping-between-topological-spaces>

    Let X and Y be topological spaces. The mapping f:X→Y is continuous if the preimage of the open set is an open set.  
    "If the topology on X is finer it is "easier" for f to be continuous" (∗)  
    hmm, ok  

-   ah shit. closedness makes way more sense now. sooo

    A function {\displaystyle f:X&rarr; Y} f:X&rarr; Y is continuous at a point {\displaystyle p} p iff {\displaystyle p&isin; \operatorname {cl} (A)&rArr; f(p)&isin; \operatorname {cl} (f(A))} p&isin; \operatorname {cl}(A)&rArr; f(p)&isin; \operatorname {cl}(f(A)).  
    WHERE X IS NOT NECESSARILY IN A!  
    so , take X = Y = {1, 2, 3}. f = id; X topoplogy is trivial; Y is discrete.  
    then take p = 1 and A = {2, 3}.  
    p is in closure of A, so touches it.  
    but. f(p) is not in closure of f(A).  

-   soo, points that seemed closes ended up apart under the map f

    in trivial topology, all points seem close; however when mapped to discrete, they fall apart  
    in the same sense, the function is not continuous if two points that seemed indistinguishable end up in topoplogically distinguishable sets  
    e.g. step function that is 0 if x <= 0 and 1 if x > 0:  
    0 is not distinguishable from eps > 0. However it gets distinguished by the image space topology.  
    so, take the open set in Y: S<sub>Y</sub> = {0}. its preimage S<sub>x</sub> is (-inf, 0]. it's not open. what's the proplem with that?  
    take any larger open set T, containing S<sub>y</sub>. its image is Y = {0,1}. or maybe even a sequence of open sets? they all get mapped to Y. But there will be a sudden jump to just {0} in the limit  
    
    in terms of closure, it's a bit easier. 0 is close to (0, inf). however f(0), which is 0 is not close to closure({1}), which is {1}.  




### I thhink I got an intuition for quotient space topology. basically: we map X to X/~. So, to derive topoplogy for quotient space, let's just assume ~ is continuous. then we'd naturally want open subsets in quotient space to be the ones with open preimage

for x ~ y == x - y is integer:  
interesting case I suppose is when a set S contains 0. then, we split it in two parts: 'left' to 0 and 'right or zero' (well defined, otherwise it's all space)  
the only interesting case if (-a, b)? Otherwise can't be open since contains limit points.  
preimage of (-a, 0): infinite union of Union<sub>k</sub> (k-a, k)  
preimage of [0, b): infinite union Union<sub>k</sub> [k, k + b)  
regrouping, we get infinite union Unkion<sub>k</sub> (k - a, k + b); which is an open set.  
ok, boring, we get the original topology  




## `[2018-10-18]` carrying on&#x2026; quotient topology is discrete

Q = G/G<sup>0</sup>  
suppose T<sub>Q</sub> (topology) is not discrete. that means there is A<sub>Q</sub> in Q such that {A<sub>Q</sub>} is not open. A<sub>Q</sub> corresponds to G<sup>0</sup> + [some] A, so that means it is not open in the original topology T. however, that contradicts G<sup>0</sup> + A being connected component.  




### The connected components are always closed (but in general not open) (from wiki). errrr


-   ugh. think of counterexample I suppose&#x2026;

    Every component is a closed subset of the original space. It follows that, in the case where their number is finite, each component is also an open subset. However, if their number is infinite, this might not be the case; for instance, the connected components of the set of the rational numbers are the one-point sets (singletons), which are not open.  
    
    ok. so manifolds are locally path connected and connected components of locally connected space are also open.  




## cover, universal cover&#x2026;

X: top space  
C is a covering space if there is a surjective map p: C -> X, such that for every x in X there is U(x), s.t. p<sup>-1</sup>(U) is a union of disjoint open sets in C, each of them is mapped homeomorphically onto U.  
covering map is more important than covering space.  
S<sup>1</sup> -> S<sup>1</sup> : x -> x<sup>k</sup> (complex), k is degree  




### nice intuition about Riemann sheets <https://math.stackexchange.com/a/95331/15108>

define function on double cover instead of original space  




### <https://math.stackexchange.com/questions/95302/covering-spaces-why-are-they-useful> 

the definition probably only seems fiddly if you haven't seen it (or related) definitions before. What is says is the following: a map p:Y→X is a covering map if p locally looks like the projection from  
X× a discrete space→X.  
A little more precisely: each point x∈X has a neighbourhood U such that the map  
p−1(U)→U  
is isomorphic to a projection  
U× a discrete space→U.  




### universal cover: simply connected




## `[2018-10-18]` uh&#x2026; skipped to 2.4




# Old&#x2026; v




# С4 group

  a b c  
a b c e  
b c e a  
c e a b  

Representation  




## e, a, b, c = 1, i, -1, -i , complex numbers multiplication




## e, a, b, c = 0, 1, 2, 3   , addition modulo 4




## matrix representation     , matrix multiplication




## geometric representation: marked square rotations




# `[2018-09-11]` O(n) <http://mathworld.wolfram.com/OrthogonalGroup.html>

O(n) preserve the quadratic form sum (x<sup>i</sup>)<sup>2</sup> (hence, circles for O(2))  




## O(p, q) &#x2013; preserves symplectic quadratic form with signature (p, q), e.g. Q(v, w) = Q(Av, Aw)

lorenz group: O(3, 1)  
O(1, 1) &#x2013; preserves x<sup>2</sup> - y<sup>2</sup> (hyperobolas)  




# `[2019-01-20]` misc





## `[2018-08-26]` quantum field theory - Why particles are thought as irreducible representation in plain English? - Physics Stack Exchange

<https://physics.stackexchange.com/questions/277986/why-particles-are-thought-as-irreducible-representation-in-plain-english>  




## `[2018-12-07]` Worked problems in physics using representation theory? : AskPhysics

<https://www.reddit.com/r/AskPhysics/comments/93clmt/worked_problems_in_physics_using_representation/>   
I haven't read the mechanics book you mentioned, so I don't know how similar these are to that, but some good books I've used that go into representation theory outside of particle physics are Hamermesh's Group theory and its application to physical problems and Petrashen's Applications of group theory in quantum mechanics.  

I am a math student and I like seeing the narrative of math applied to physics. I am reading through Georgi's "Lie Algebras in Particle Physics" now, and chapters 1.16 and 1.17 use representation theory to easily characterize the normal modes of a quirky system of springs and blocks.  

I once read through the book "Solved Problems in Lagrangian and Hamiltonian Mechanics" by Gignoux & Silvestre-Brac, and it helped me see the non-pure side of the symplectic dynamics/variational calculus I was learning. I really liked this applied section in Georgi. I never saw these techniques in undergrad physics and I find it really cool. Do you know of any other sources that go through specific examples/calculation problems in physics and apply representation theory?  




# . Wigner himself did a lot to improve the situation, writing a book entitled Group Theory and Its Application to the Quantum Mechanics of Atomic Spectra in 1931. It explained groups and representations in a language closer to that with which physicists were familiar.

    . Wigner himself did a lot to improve the situation, writing a book entitled Group Theory and Its Application to the Quantum Mechanics of Atomic Spectra in 1931. It explained groups and representations in a language closer to that with which physicists were familiar.




# `[2019-01-24]` Short Introduction to and Motivation for Representation Theory – Jakob Schwichtenberg      [[reprtheory]]

<http://jakobschwichtenberg.com/short-introduction-motivation-representation-theory/>  
well, ok it's really basic  




# `[2019-01-24]` What’s so special about the adjoint representation of a Lie group? – Jakob Schwichtenberg      [[reprtheory]]

<http://jakobschwichtenberg.com/adjoint-representation/>  

    P.S. I wrote a textbook which is in some sense the book I wished had existed when I started my journey in physics. It's called "Physics from Symmetry" and you can buy it, for example, at Amazon.




# `[2019-01-23]` [Best intro to representation theory?](https://reddit.com/r/math/comments/3k3jwh/best_intro_to_representation_theory/cuugprk/) /r/math

    I think Fulton and Harris has become one of the gold standards. Serre's "Linear Representations of Finite Groups " is fantastic, but is a bit more terse and requires lots of mathematical maturity.




# `[2019-01-23]` [Representation Theory](https://reddit.com/r/math/comments/1emn1m/representation_theory/ca1pyp4/) /r/math

    Representation Theory is fucking everywhere. It's the opposite of a dead end. A co-dead end. The only issue is that at first glance it doesn't seem that exciting. Then, as you continue your studies, it will start to pop-up everywhere because it gives you invaluable tools with which to study abstract groups.




# `[2019-01-23]` [Representation Theory](https://reddit.com/r/math/comments/1emn1m/representation_theory/ca1qrdl/) /r/math

    I have to agree with functor7 that representation theory comes up everywhere. I think it's rather exciting from a basic level too.

    Studying finite groups, you might think the prime object of study is permutations: to understand your group, you look how it acts on some finite set, by permuting elements around. However, it is quite tricky to get all the information you might want from it.
    Another very profitable way to understand your finite group is to let it act, not by permutations, but by linear transformations, on a vector space instead of just a set. This is a representation. You lose a bit of information this way, but you usually can end up saying so much more. The key is to understand the irreducible representations. For instance, the order of the group is the sum of the squares of the dimensions of the different irreducible representations of the group. Much more can be said, of course.

    What's amazing is that this approach generalises to so many other contexts.
    You can do representation theory of Lie groups. For instance, representation theory of the circle group (group of unit norm complex numbers) encodes Fourier series, and you can vastly generalise this to Pontryagin duality, Peter-Weyl duality, and beyond (automorphic representations...).
    You can do representation theory of Lie algebras, and this is the essential ingredient in the classification of semisimple Lie algebras (say over the complex numbers).
    You can do representation theory of rings. This is just the notion of a module over a ring, which comes up everywhere in commutative algebra!
    You can do representation theory of quivers. This is really tantalising: you start with a collection of dots, and arrows between the dots. A representation of this consists just of a vector space for each dot, and for each arrow a linear map between the corresponding beginning and endpoint vector spaces. It sounds silly, but is an incredibly powerful tool.
    And so on, and so on...

    Another very powerful tool is to look at categories of representations. Given for instance a finite group G (but it could be any of the other things representations makes sense for), you kind of reverse the construction I did for quivers. You put a dot for each representation of G, and an arrow for each linear map between representations which respects the actions (a so called intertwiner). You forget everything else, so you don't remember how the group acts on each vector space, you just have a dot instead. This is the category of representations of G, and it's very interesting to see its structures, and whether you can figure out the group knowing just this category. For many interesting reasons, it turns out you can't. However, this category has subtle extra structures; for instance you can take tensor products of representations. If you remember this tensor product structure explicitly (which comes down to remembering explicit associativity isomorphisms [; (A \otimes B) \otimes C \cong A \otimes ( B \otimes C) ;]) then you can actually recover the group! It's quite a fantastic statement really, when you realise it seems like we forgot so much about the group and are just looking at a collection of dots and arrows!
    This point of view explains things like what the character table of a group does and does not see, and explains why you can't recover the group from the character table.




# `[2019-01-23]` [Can Representation Theory be Explained Using Basic Abstract and Linear Algebra?](https://reddit.com/r/math/comments/i73t4/can_representation_theory_be_explained_using/c21iiba/) /r/math

    Sternberg's *Group Theory and Physics*.
    Go to Amazon and order it [*right now*](http://www.amazon.com/Group-Theory-Physics-S-Sternberg/dp/0521558859).  It's an easy book^1 that will put you **ridiculously far ahead** of anyone else with a similar background.  That's because representation theory is usually taught abstractly, and Sternberg contains nothing but concrete examples.  With *numbers*.  So while everyone else is trying to parse  word-salad about rings of maps between modules over groups of categoric chain algebras, you'll already have a fairly good idea of what's happening by analogy with what you already know.
    I'm not saying that the more abstract material isn't worth learning, just that learning the concrete stuff first is a faster way to get there that a lot of people have forgotten about.  Plus you learn about spectroscopy, crystal structure, and quantum mechanics, basically for free.

    [1] For math, anyway.  You still have to "read" it with pen & paper.




# `[2019-01-23]` [Book suggestions for modern representation theory?](https://reddit.com/r/math/comments/1c9uax/book_suggestions_for_modern_representation_theory/c9ehg8n/) /r/math

    How much representation theory do you already know? If you're just starting out and want a good book to help develop intuition I recommend [Groups, Representations, and Characters](http://product.half.ebay.com/Groups-Representations-and-Characters-by-Victor-E-Hill-1976-Hardcover/1315464&tg=info) by Hill. It takes a sort of naive approach, so it's not awfully rigorous, but I found it to be a great companion to the denser graduate stuff. It doesn't cover harmonic analysis or compact groups, but it was the only gently written text on rep theory I could find during a semester of independent study.




# `[2019-01-23]` [Everything about Representation theory of finite groups](https://reddit.com/r/math/comments/8i7x6s/everything_about_representation_theory_of_finite/dyq2qxg/) /r/math

    Really all of QM depends on representation theory. Take a potential, and find all the operations \(rotations, inversions, etc.\) which leave it invariant. For example, take a potential from 3 protons in an equilateral triangle. There are 6 'covering' operations: Rotation by 60/120 degrees with the axis of rotation normal to the plane of the triangle and 3 180 degree rotations about axes in the plane of the triangle. This is the [Dihedral Group D3](http://mathworld.wolfram.com/DihedralGroupD3.html). Like any group, it is closed under multiplication of the elements, where in this case multiplication AB is defined as applying operation B then applying operation A. So a multiplication table can be made that show every possible product in the group.
    As of now, the elements of the group are just operations. Representation theory is writing a set of matrices  homomorphic to the group, where each matrix represents a particular operation. In this case, this means the matrices must obey the multiplication table of the group. Keep in mind that setting all matrices to the scalar 1 forms a representation for any group, because If you need to satisfy AB = C then 1\*1 = 1. After a bunch of math, group theory tells us that there are a set number of possible representations with different matrix dimensions \(all square\). At the end of the day, we can define all operations which leave the Hamiltonian in QM unchanged as the group of the Schrodinger equation \(this is the same as saying the group of all operations which commute with the Hamiltonian\). The KE operator has no effect on the symmetry, so we can just look to the potential for the operations which leave the hamiltonian invariant.
    Suppose we have some state psi that satisfied H psi = E psi \(the time\-independent Schrodinger Equation\). Act on this equation with one of the operations in the group of the Schrodinger equation. Then RH psi = R E psi, which means H \(R psi\) = E \(R psi\), so \(R psi\) is a new eigenfunction which has the same energy as the original. We can continue with all operations in the group to find all the degenerate wavefunctions corresponding to the eigenvalue E. This set of N wavefunctions \(N is the number of elements in the group\) forms a basis for an N dimensional vector space now. We know any wavefunction in this invariant subspace can be written as a linear combination of the basis vectors, so we can see how R affects each of the basis functions we have chosen. In the terms of linear algebra, R now becomes a transformation matrix that turns the constituent basis vectors into whatever the operator changes them to. These transformation matrices actually form a representation of the group of the Schrodinger equation \(which I haven't proved\). These representations are unique up to a change of basis \(equivalent to a similarity transform\), so this means each possible eigenvalue of the Hamiltonian 'belongs' to a certain representation of the group of the Schrodinger Equation.
    Remember that there can be many representations of the same group. Take our D3 group. Representation theory tells us that the only possible representations \(up to similarity transforms\) have dimensionality 1, 1 and 2. Well these representation matrices are the same ones that just came up in the description about the representation for each eigenvalue. From this, we can clearly see that we can only possibly have states with either no degeneracy or a degeneracy of 2 \(remember the dimension of the matrix dictates how many basis functions we need\). Also remember that each eigenvalue has its own representation, so different eigenvalues of the same Hamiltonian can have different degeneracy. This information can be found before we even begin to do calculations involving the Hamiltonian, so that's really nice.
    Now, going back to this vector space where we defined basis functions for the degenerate space, we have a convenient way to characterize the state. First we give the eigenvalue, which we commonly label by ordering the eigenvalues from smallest to largest and using it's place as the label n. Now, we have a set of degenerate functions corresponding to this label n, but we can apply a 2nd label \(call it 'l'\) to each basis function. Well now we can uniquely label any eigenfunction of the Hamiltonian with the labels \(n,l\). These are known as quantum numbers, which you've most likely heard in relation to the hydrogen atom. The 3 'p' orbitals are the basis functions for a 3\-dimensional vector space of eigensolutions, and they are generated by applying rotation operators which are in the group of the Schrodinger equation. There's some extra subtlety here, because there is also an s orbital which is degenerate to the p orbitals. Normally, if the degeneracy cannot be explained by symmetry then it is known as an 'accidental' degeneracy, but Fock showed that there is actually a set of operations in 4\-D which exploits the symmetry. The hydrogen potential has the group O\(4\), and you should be able to understand most of the language in the introduction [here](https://www.jstor.org/stable/2100327?seq=1#page_scan_tab_contents). With something like Hydrogen, we actually end up factoring the full group into direct product groups which commute with each other, so we can further simplify the quantum numbers.
    Obviously molecules have symmetries arising from their shape, so we know what kind of representations their energy levels must correspond to. By applying a perturbation like an electric field, we can couple different energy levels together which may belong to different representations. Since the perturbation itself will have its own representation within the group, we can use these determine which transitions are allowed by symmetry \(usually called selection rules\). I haven't really given any of the details on why this happens here, but it's an important use. This is how we interpret the results we get from spectroscopy.
    Crystals are another place where group theory/representation theory is really important. You have a unit cell of atoms which has some group of operators which leaves it invariant. Then you put it in a lattice, so now we have an infinite number of group elements corresponding to translations by the lattice constant \(in the appropriate directions\). As long as the unit cell \(point group\) lattice is 'compatible' with the lattice, the space group of the crystal can be formed by taking all possibly combinations of operations. We can write the general operation as {R|t} where R is some generalized rotation \(coming from the unit cell symmetries\) and t is a translation \(coming from the repetition symmetry\).
    For now let's just look at the group of the translations, and only in one dimension for simplicity. Pick any eigenvalue of the Hamiltonian. We know that the wavefunction\(s\) corresponding to this eigenvalue must be a representation of the group of the Schrodinger equation \(the translation operators\). The group is a cyclic group generated by the element Ta, where Ta is a translation by one 'unit cell.' Cyclic in this case means any general T = Ta\^n for some n. These groups are obviously Abelian since every element will commute \(Ta always commutes with itself and every element is Ta\*Ta\*...\*Ta\).
    Well another group theory fact I left out is that there are as many representations of a group as there are conjugacy classes. The conjugacy class of an element A is XAX\^\-1 for all X in the group, repeat this for every element in the group and discard any repeats and you get all the classes.  This means we have a representation for each operator. These classes are way more important than they may have seemed from what I've previously written, because you'll often see groups written in terms of their character table, where character is defined as the trace of the representation matrix. Group elements in the same class will have the same character, this can be pretty easily seen since A and B being in the same class means XAX\^\-1 = B for some X. Well now just think of that instead as matrices, which is what we are doing in our representation. This corresponds to a similarity transform \(notice these showed up before as well\), and it is easily proven that elements connected by a similarity transform have the same trace.
    Back to a 1\-dimensional crystal: Clearly each element in an Abelian group forms its own class because the X and X\^\-1 will commute through the A and cancel out, so each element will only generate itself. Crystals actually have a finite number of elements, so the way we have stated the problem the operators won't form a group because they aren't closed under Ta\^\(N\+1\), where we have 'walked off' the end of the crystal. So to simulate the effects of an 'infinite' crystal, we use periodic boundary conditions and suppose that the end loops back around to the beginning. So now we have a nice cyclic group of N elements with N representations since each element forms its own class. The laws of group theory also fix the sum of the squares of the dimensions of the representations to be equal to the number of elements in the group, so this fixes each representation to be one dimensional, or in other words each representation is just some scalar. Say that in a particular representation the generating element Ta is written as r, so r\^N = 1 by the periodic boundary conditions. So r = exp\(2\*pi\*i\*p/h\), where p = 1,2,3 ... h. But since psi must belong to a representation of the group, we must have Ta psi\(x\) = psi\(x \+ a\) = exp\(2\*pi\*i\*p/h\), and we eventually find that any function satisfying these conditions can be written as u\(x\)e\^\(ikx\), which is the very important Bloch Theorem. My derivation here doesn't have all the explanations, and I skipped the entire process of relabeling p to k, but I actually have to go so maybe I'll come back later and fix it.




# `[2019-01-23]` [Everything about Representation theory of finite groups](https://reddit.com/r/math/comments/8i7x6s/everything_about_representation_theory_of_finite/dyq36b0/) /r/math

    I tried to add at the top that this all follows almost exactly from Tinkham's Group Theory and Quantum Mechanics. But that put me over the character limit so I decided to just say it in a reply. I'm not an expert on this stuff and I don't even have a 100&#37; grasp on the stuff I wrote above, but I'm working on it. Also there's a decent chance you already know basic group theory. I mostly just put that stuff in for myself because I'm terrible at it and I need to repeat it every chance I can get.




# `[2018-09-03]` grand unified theory resources      [[study]] [[reprtheory]]

<http://jakobschwichtenberg.com/resources-that-helped-me-understand-grand-unified-theories/>  




# `[2020-08-03]` [Eric Weinstein on Twitter: "You can call S<sup>3</sup> by all of the following names: S<sup>3</sup>, Spin(3), SU(2), Sp(1) only they lead to **different** generalizations. Unfortunately Spin(4)=SU(2)xSU(2) is seldom written Spin(4)=Sp(1)xS<sup>3</sup> which should be preferred. But why is one naming better? It‘s because it generalizes." / Twitter](https://twitter.com/EricRWeinstein/status/1290383725599973376)

    You can call S^3 by all of the following names:
    
    S^3, Spin(3), SU(2), Sp(1)




# `[2019-01-20]` Physics from Symmetry - Jakob Schwichtenberg - Google Books      [[book]] [[reprtheory]]

-   State "STRT"      from "TODO"       `[2019-02-27]`

<https://books.google.co.uk/books?id=bipBDwAAQBAJ&pg=PA91&lpg=PA91&dq=%22spin+0%22+representation&source=bl&ots=tn4XLPmWDc&sig=ACfU3U1dUSMAyjpvDV-6Vx0f6k0oXTrguw&hl=en&sa=X&ved=2ahUKEwjz7LC_2vzfAhUlQRUIHXxOBrwQ6AEwEHoECBYQAQ#v=onepage&q=%22spin%200%22%20representation&f=false>  




# representations as monoids?      [[think]]

<https://mathoverflow.net/questions/37115/why-arent-representations-of-monoids-studied-so-much>  




# `[2019-02-24]` Nikita Lisitsa on Twitter: "Representation theory of finite groups in action. Here are 3 lowest-energy orbitals of a hypothetical H₃²⁺ ion, with hydrogen nuclei arranged into a regular triangle. The permutation group S₃ acts on the system simply by permuting the nuclei. <https://t.co/KvFsQVHuCG>" / Twitter

<https://twitter.com/lisyarus/status/1099620329612365824>  

