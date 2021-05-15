
# Table of Contents

-   [resource recommendations](#rsrcrcmmndtns) 
-   [baez tutorial](#bzttrl) 
    -   [http://math.ucr.edu/home/baez/einstein/node3.html](#mthcrdhmbznstnndhtml) 
    -   [http://math.ucr.edu/home/baez/einstein/node6a.html newthon's law derivation &#x2013; go through](#mthcrdhmbznstnndhtmlnwthnslwdrvtngthrgh) 
-   [`[2014-07-15]`  sean carroll lecture notes on general relativity](#sncrrlllctrntsngnrlrltvty) 
    -   [parallel transport depends on path. actually that's why relative velocity doesn't make sense.](#prllltrnsprtdpndsnpthctllthtswhyrltvvlctydsntmksns) 
    -   [equation of paralllel transport. in a sense, it's a IVP](#qtnfprlllltrnsprtnsnstsvp) 
-   [ANN [Carroll][2014] Spacetime and Geometry. An Introduction to General Relativity.pdf](#nncrrllspctmndgmtrynntrdctntgnrlrltvtypdf) 
    -   [p.6 synchronised clocks: from point a to b and back to a, then t<sub>b</sub> = (t<sub>a</sub> + t<sub>a</sub>') / 2](#psynchrnsdclcksfrmpnttbndbcktthntbtt) 
    -   [p.8 coordinates are superscripts, metric tensor is subscripts](#pcrdntsrsprscrptsmtrctnsrssbscrpts) 
    -   [p.9 timelike particles is travelling slower than light](#ptmlkprtclsstrvllngslwrthnlght) 
    -   [p.11 nonstraight path has a shorter proper time](#pnnstrghtpthhsshrtrprprtm) 
    -   [p. 13 Lorentz transformations, lorentz group](#plrntztrnsfrmtnslrntzgrp) 
    -   [p.15 once the space is curved, we can't move vectors freely anymore. tangent space T<sub>p</sub>](#pncthspcscrvdwcntmvvctrsfrlynymrtngntspctp) 
    -   [p. 19](#p) 
    -   [p.24](#p) 
        -   [hmm, must have something to do with determinant? https://physics.stackexchange.com/a/281185/40624](#hmmmsthvsmthngtdwthdtrmnntsphyscsstckxchngcm) 
        -   [magnetic and electric fields &#x2013; are only vectors under rotations in space. in facet &#x2013; components of EM (0, 2) tensor](#mgntcndlctrcfldsrnlyvctrsttnsnspcnfctcmpnntsfmtnsr) 
    -   [p. 30 &#x2013; covariant form of equations means tensorial &#x2013; has nothing to do with 'covariant' as oppposed to 'contravariant'](#pcvrntfrmfqtnsmnstnsrlhsntdwthcvrntspppsdtcntrvrnt) 
    -   [p 31 &#x2013; the fact that spacetime is flat allows a unique choice of straight line between the points](#pthfctthtspctmsfltllwsnqchcfstrghtlnbtwnthpnts) 
    -   [p 32](#p) 
        -   [eq 1.106 &#x2013; wonder if it's the 'type directed' inference that guy mentioned](#qwndrftsthtypdrctdnfrncthtgymntnd) 
    -   [p 33](#p) 
    -   [p 34](#p) 
    -   [ok, do exercises, p. 45](#kdxrcssp) 
-   [some pdf at work.. calculating levi-civita symbols for cylinder](#smpdftwrkclcltnglvcvtsymblsfrcylndr) 
-   [play with metric tensor a bit](#plywthmtrctnsrbt) 
    -   [suppose metric is dS = x<sup>2</sup> dx + dy<sup>2</sup>.  What does that mean?](#sppsmtrcsdsxdxdywhtdsthtmn) 
    -   [ok, let's do something more funny&#x2026; suppose dS = y<sup>2dx</sup><sup>2</sup> + x<sup>2dy</sup><sup>2</sup>](#kltsdsmthngmrfnnysppsdsydxxdy) 
    -   [ok, another attempt&#x2026; ds = dr<sup>2</sup> + r<sup>2</sup> dq<sup>2</sup>](#knthrttmptdsdrrdq) 
    -   [leftovers during me doing the exercise](#lftvrsdrngmdngthxrcs) 
-   [physicspages stuff &#x2013; it's actually very decent!](#physcspgsstfftsctllyvrydcnt) 
    -   [2D exponential metric http://physicspages.com/pdf/Moore/Moore%20Problems%2008.06.pdf](#dxpnntlmtrcphyscspgscmpdfmrmrprblmspdf) 
    -   [geodesics on a sphere http://www.physicspages.com/Index%20-%20Relativity.html](#gdscsnsphrwwwphyscspgscmndxrltvtyhtml) 
-   [[Takeuchi][2010] An Illustrated Guide to Relativity](#tkchnllstrtdgdtrltvty) 
-   [`[2015-03-16]` some old notes](#smldnts) 
-   [related](#rltd) [[physics]] [[relativity]]
-   [`[2018-07-25]` The Meaning of Einstein's Equation](#thmnngfnstnsqtn) [[baez]]
-   [make up some crazy metric (e.g. g = Diag[x<sup>2y</sup><sup>2z</sup><sup>2</sup>, 1, 1]) can we do something cool about it?](#mkpsmcrzymtrcggdgxyzcnwdsmthngclbtt) [[think]]
-   [susskind lectures](#ssskndlctrs) [[study]] [[towatch]]
-   [`[2019-06-18]` MITGameLab/OpenRelativity: An open source framework to add the effects of traveling at relativistic speeds to visualizations or games](#mtgmlbpnrltvtynpnsrcfrmwrgtrltvstcspdstvslztnsrgms) [[game]]
    -   [`[2019-06-18]` OpenRelativity: An Open-Source Toolkit for Unity3D by MIT Game Lab - YouTube](#pnrltvtynpnsrctlktfrntydbymtgmlbytb) [[vr]]
-   [https://flannelhead.github.io/posts/2016-03-11-blackstar.html](#sflnnlhdgthbpstsblckstrhtml) 
-   [`[2018-11-20]` general relativity - Why is the covariant derivative of the metric tensor zero? - Physics Stack Exchange](#gnrlrltvtywhysthcvrntdrvtmtrctnsrzrphyscsstckxchng) 
-   [`[2018-11-19]` differential geometry - Is there a good way to compute Christoffel Symbols - Mathematics Stack Exchange](#dffrntlgmtrysthrgdwytcmptfflsymblsmthmtcsstckxchng) 
-   [`[2018-11-19]` differential geometry - Why may geodesic not be the shortest path on a surface? - Mathematics Stack Exchange](#dffrntlgmtrywhymygdscntbttpthnsrfcmthmtcsstckxchng) 
-   [`[2020-07-21]` gravitational waves - So Black Holes Actually Merge! In 1/5th of a Second - How? - Physics Stack Exchange](#sphyscsstckxchngcmqstnssbnthfscndhwphyscsstckxchng) 
-   [`[2020-07-21]` event horizon - What is exactly the density of a black hole and how can it be calculated? - Physics Stack Exchange](#sphyscsstckxchngcmqstnswhcntbclcltdphyscsstckxchng) 
-   [`[2020-07-21]` general relativity - Is a black hole's mass uniformly distributed? - Physics Stack Exchange](#sphyscsstckxchngcmqstnssbmlydstrbtdphyscsstckxchng) 
-   [`[2020-07-21]` Why does gas form a star instead of a black hole? - Astronomy Stack Exchange](#sstrnmystckxchngcmqstnswhstdfblckhlstrnmystckxchng) 
-   [`[2020-07-21]` Ask Ethan: Does A Time-Stopping Paradox Prevent Black Holes From Growing?](#swwwfrbscmstsstrtswthbngsgprdxprvntblckhlsfrmgrwng) 
-   [`[2020-07-21]` The Best Tower Fans To Cool Down Your Home](#swwwfrbscmstsfrbsprsnlshpwrfnthbsttwrfnstcldwnyrhm) 
-   [hmm, how would forces work inside the black hole event horizon if the force carriers can't go backwards?](#hmmhwwldfrcswrknsdthblckhrznfthfrccrrrscntgbckwrds) [[quantum]]
-   [`[2020-07-14]` Ask HN: Without Einstein, would General Relativity be discovered by now? | Hacker News](#snwsycmbntrcmtmdskhnwthtnlrltvtybdscvrdbynwhckrnws) 

Geodesics: takes vectors that are tangent to themselves and keeps them tangent while they are parallel transported  




# resource recommendations

<https://physics.stackexchange.com/questions/363/books-for-general-relativity>  




# baez tutorial

<http://math.ucr.edu/home/baez/gr/gr.html>  




## <http://math.ucr.edu/home/baez/einstein/node3.html> 

We promised to state Einstein's equation in plain English, but have not done so yet. Here it is  
   Given a small ball of freely falling test particles initially at rest with respect to each other, the rate at which it begins to shrink is proportional to its volume times: the energy density at the center of the ball, plus the pressure in the \(x\) direction at that point, plus the pressure in the \(y\) direction, plus the pressure in the \(z\) direction.  

huh!  




## <http://math.ucr.edu/home/baez/einstein/node6a.html> newthon's law derivation &#x2013; go through




# `[2014-07-15]`  sean carroll lecture notes on general relativity

many people recommend it (e.g. on Reddit)  
<http://www.preposterousuniverse.com/grnotes/>  




## parallel transport depends on path. actually that's why relative velocity doesn't make sense.




## equation of paralllel transport. in a sense, it's a IVP

parallel propagator  
ok, we get geodesic equatiion from the parellel transport equation  




# ANN [Carroll][2014] Spacetime and Geometry. An Introduction to General Relativity.pdf





## p.6 synchronised clocks: from point a to b and back to a, then t<sub>b</sub> = (t<sub>a</sub> + t<sub>a</sub>') / 2

natural generalisation of cartesian coordinates in space  
if we construct coordinates that way, it's called inertial frame  




## p.8 coordinates are superscripts, metric tensor is subscripts




## p.9 timelike particles is travelling slower than light

proper time is ds (where -ds<sup>2</sup> < 0)  




## p.11 nonstraight path has a shorter proper time

interval &#x2013; integral of sqrt(n<sub>uv</sub> d<sup>u</sup>/dlam d<sup>v</sup>/dlam dlam)  




## p. 13 Lorentz transformations, lorentz group

boost - rotations between space and time  
Poincare group  

spacetime transformations: axes are orthogonal in the lorenzian sense  




## p.15 once the space is curved, we can't move vectors freely anymore. tangent space T<sub>p</sub>




## p. 19

T<sub>p</sub> &#x2013; contravariant vectors  
T<sup>\*</sup><sub>p</sub> &#x2013; covariant vectors  

gradient &#x2013; dual vector  
levi-civita symbol: eps<sub>uvpo</sub> = +1/-1/0 &#x2013; if even/odd permutation/otherwise  




## p.24 

metric, inverse metric, kronecker delta and the levi-civita symbol &#x2013; their components are unchanged in <span class="underline">any</span> inertial coordinate frame in flat spacetime (and these are the <span class="underline">only</span> tensors with suck property)  
kronecker &#x2013; identity map from vectors to vectors, so should have same components regardless  




### hmm, must have something to do with determinant? <https://physics.stackexchange.com/a/281185/40624>

  if we are referring to the same Levi-Civita symbol, i.e. the completely antisymmetric symbol, then this is not a tensor. It is a tensor density of weight −1, which means that under a general coordinate transformation it gets multiplied by the inverse Jacobian of the transformation.  
hmm  




### magnetic and electric fields &#x2013; are only vectors under rotations in space. in facet &#x2013; components of EM (0, 2) tensor




## p. 30 &#x2013; covariant form of equations means tensorial &#x2013; has nothing to do with 'covariant' as oppposed to 'contravariant'




## p 31 &#x2013; the fact that spacetime is flat allows a unique choice of straight line between the points

timelike particles &#x2013; useful to parameterise them by proper time (sometimes you can experess tau(lambda) and then transform to x(tau)). 4-velocity is the tangent vector in this parameterisation  
4-velocity is always normalised &#x2013; makes sense since it's velocity through spacetime  




## p 32

mass is a fixed quantity independent of inertial frame, 'rest mass'  
hmmm, unclear&#x2026;  
wiki says that by definition the invariant mass is ratio of 4-momentum to 4-velocity  
  The invariant mass, rest mass, intrinsic mass, proper mass, or in the case of bound systems simply mass, is the portion of the total mass of an object or system of objects that is independent of the overall motion of the system.  
that actually makes more sense  




### eq 1.106 &#x2013; wonder if it's the 'type directed' inference that guy mentioned




## p 33

energy-momentum tensor &#x2013; flux of momentum p<sup>u</sup> throught a surface of constant x<sup>v</sup>  




## p 34

derivation of energy-momentum tensor for dust  




## ok, do exercises, p. 45




# some pdf at work.. calculating levi-civita symbols for cylinder




# play with metric tensor a bit





## suppose metric is dS = x<sup>2</sup> dx + dy<sup>2</sup>.  What does that mean?

first, analyse the dS. The further away we are from origin, the longer is line element.  
TODO what does that mean?  
TODO dS = d(x<sup>2</sup>/2) + dy<sup>2</sup> &#x2013; wonder if that transformation is useful?  

-   So, our metric tensor is Diag[x<sup>2</sup>, 1]?  
    TODO is the metric being positive definite important? &#x2013; ok, if it's not, that's non Riemannian geometry, apparently some crazy shit.

Geodesic equation: <https://en.wikipedia.org/wiki/Solving_the_geodesic_equations#The_geodesic_equation>  
TODO t is arbitrary parameter?  
d<sup>2</sup> x<sup>a</sup>/dt<sup>2</sup> + G<sup>a</sup><sub>bc</sub> dx<sup>b</sup>/dt dx<sup>c</sup>/dt = 0  
so we need Christoffel symbols. for diagonal metric, we can cheat <https://math.stackexchange.com/a/799027/15108>  
 since g<sub>xx</sub> = x<sup>2</sup> and g<sub>yy</sub> = 1, we can see only G<sup>i</sup><sub>ii</sub> are non zero and G<sub>xx</sub> = 1/x, G<sub>yy</sub> = 0.  
hence, substituting into the equation above, get system  
 d<sup>2</sup> x/dt<sup>2</sup> + 1/x (dx/dt)<sup>2</sup> = 0  
 d<sup>2</sup> y/dt<sup>2</sup> = 0  
<https://www.wolframalpha.com/input/?i=d%5E2y%2Fdt%5E2+%3D+0,+d%5E2x%2Fdt%5E2+%2B+1%2Fx+(dx%2Fdt)>%5E2+%3D+0  
so,  
y = yt + C &#x2013; right, that means geodesic in flat space got constant velocity and direction. makes sense  

x = A sqrt(B + 2 t)  

Solve the IVP next. Assume x0 = 0, y0 =0; we get  
  y = y'<sub>0</sub> t (duh)  
  x = x'<sub>0</sub> sqrt(2 t)  

Right, so what all of that means?  
In a sense, it's just moving slower through X axis in comparison to as if it was moving in 'normal' metric?  
but basically, it's just a coordinate transformation right?  
I guess the difference is: we have figured out via experiment that our world has got 'uniform' coordinates.  
in the world with the metric above:  
wait&#x2026; we haven't introduced time there. so doesn't make much sense to reason about it.  
ok suppose we do introduce time. assuming they dependency of parameter on time is linear (is it??), then suggest the following experiment:  
  Alice: goes for 1 minute in one direction, then turns back and walks for one minute.  
  Bob: goes for 1 minute in the orthogonal direction, then turns back and walks for one minute.  
hmm, how do they measure distance? ah doesn't even matter, what matters is that they don't meet at the same point?  
oh.. wait  
ah it's fine. one observer travels 1 minute up, 1 minute right, 1 minute down, 1 minute left. nope.. wouldn't work.  
so it is undetectable after all??  
this is actually quite similar to universe expansion?  
ok, so take two observers. one is at 0, another is at 100.  
right&#x2026; so curves don't have intrinsic curvature! therefore, curvature is undetectable by the inhabitants of that world  




## ok, let's do something more funny&#x2026; suppose dS = y<sup>2dx</sup><sup>2</sup> + x<sup>2dy</sup><sup>2</sup>

metric tensor  
Diag [y<sup>2</sup>, x<sup>2</sup>]  
christoffel symbols  
G<sup>i</sup><sub>ii</sub> = 0  
G<sup>i</sup><sub>ji</sub> = delta<sub>j</sub> ln sqrt(x<sup>j</sup><sup>2</sup>)  
G<sup>x</sup><sub>yx</sub> = delta<sub>y</sub> ln sqrt y<sup>2</sup> = 1/y &#x2013; ok, same for the other one, G<sup>y</sup><sub>xy</sub> = 1/x  
G<sup>x</sup><sub>yy</sub> = -1/2 1/g<sub>xx</sub> delta<sub>x</sub> g<sub>yy</sub> = -1/2 1/y<sup>2</sup> d(x<sup>2</sup>) = -x/y<sup>2</sup>. Same for G<sup>y</sup><sub>xx</sub> = -y/x<sup>2</sup>  
right&#x2026; so what?, substitute!  
x''<sup>2</sup>  = (-x/y<sup>2</sup> y'<sup>2</sup> + 1/y x' y') = 0, symmetric for y  

yikes! <https://wolframalpha.com/input/?i=solve+x%27%27+%2B>+(-x%2Fy%5E2+y%27%5E2)+%2B1%2Fy+x%27+y%27+%3D+0,+y%27%27+%2B+(-y%2Fx%5E2+x%27%5E2)++%2B+1%2Fx+x%27+y%27+%3D+0  




## ok, another attempt&#x2026; ds = dr<sup>2</sup> + r<sup>2</sup> dq<sup>2</sup>

Diag[1, R<sup>2</sup>]  
christoffel:  
G<sup>R</sup><sub>qq</sub> = -R  
G<sup>q</sup><sub>Rq</sub> = 1/R  
<https://www.wolframalpha.com/input/?i=solve+x%27%27+-+x+y%27%27+%3D+0,+y%27%27+%2B+1%2Fx+x%27+y%27++%3D+0>  
ugh&#x2026; pretty bad too.  
huh it's actually in Caroll lecture notes, page 60  




## leftovers during me doing the exercise

in general its too hard to do geodesics in full generality. sooften we justchoose a path and see if its a geodesic! and a natural one to choose is a pathdefined by only one of the parameters - its called a parameter curve  

<http://astro.dur.ac.uk/~done/gr/l6.pdf>  
ex5.pdf in downloads &#x2013; direct solution  

<https://en.wikipedia.org/wiki/Deriving_the_Schwarzschild_solution> &#x2013; might be useful  
<https://en.wikipedia.org/wiki/Schwarzschild_metric#Alternative_coordinates>  
<https://en.wikipedia.org/wiki/Line_element>  
line element is g(dq, dq)  
right, so I'm gonna need spherical or cylindrical geometry  
The easiest way to find the metric of the 2-sphere (or the sphere in any dimen-sion) is to picture it as embedded in one higher dimension of Euclidean space,then restrict to constant radius &#x2013; hmm..  

So Christoffel symbols are like the metric - they do tell us about curvature(what we are interested in) but they also tell us about what coordinate systemwe have chosen (which isn’t at all fundamental).  




# physicspages stuff &#x2013; it's actually very decent!

<http://www.physicspages.com/Index%20-%20Relativity.html>  




## 2D exponential metric <http://physicspages.com/pdf/Moore/Moore%20Problems%2008.06.pdf>




## geodesics on a sphere <http://www.physicspages.com/Index%20-%20Relativity.html>




# [Takeuchi][2010] An Illustrated Guide to Relativity

-   Your Bookmark on Page 43 | Added on Sunday, August 4, 2013 12:00:22 AM  
    illustration how a unit cell in c-t space shifts to a parallelogram, not very interesting
-   Your Bookmark on Page 96 | Added on Sunday, August 4, 2013 12:15:55 AM  
    same&#x2026;
-   Your Bookmark on page 110 | Added on Sunday, September 27, 2015 4:13:18 PM  
    addition of velocities? not interesting&#x2026;




# `[2015-03-16]` some old notes

    Parallel transport: TODO
    
    Riemann tensor: describes how vector is changed during the parallel transport along a loop. Describes curvature.
    
    R(u, v, w) = R^a_bcd u^b v^c w^d
    
    Ricci tensor:
    R_bd = R^c_bcd
    
    R^a_d = g^ab R_bd
    
    Ricci scalar: R^a_a
    
    Geometrically, the Ricci curvature is the mathematical object that controls the growth rate of the volume of metric balls in a manifold.
    
    Paralllel transport on the Earth surface might change the direction
    
    For fun, notice that if we think of the earth as a unit sphere, it's area is 4 pi, and our Roman has just travelled around a region of land having area one eighth of that, hence pi/2. His javelin has rotated by an angle of pi/2! This is no coincidence: on the unit sphere, whenever you go around a simple closed curve enclosing an area A, parallel translation gives a rotation of angle A.
    
    
    Again, all this is easier to visualize in 2d space rather than 4d spacetime. A person walking on a sphere `following their nose' will trace out a geodesic -- that is, a great circle. Suppose two people stand side-by-side on the equator and start walking north, both following geodesics. Though they start out walking parallel to each other, the distance between them will gradually start to shrink, until finally they bump into each other at the north pole. If they didn't understand the curved geometry of the sphere, they might think a `force' was pulling them together.
    
    Similarly, in general relativity gravity is not really a `force', but just a manifestation of the curvature of spacetime. Note: not the curvature of space, but of spacetime. The distinction is crucial. If you toss a ball, it follows a parabolic path. This is far from being a geodesic in space: space is curved by the Earth's gravitational field, but it is certainly not so curved as all that! The point is that while the ball moves a short distance in space, it moves an enormous distance in time, since one second equals about 300,000 kilometers in units where $c = 1$. This allows a slight amount of spacetime curvature to have a noticeable effect.
    
    Problem Book in Relativity and Gravitation, A. Lightman and R. H. Price (Princeton University Press, Princeton, 1975).
    
    http://math.ucr.edu/home/baez/einstein/node15.html
    
    
    Contravariant vectors describe those quantities where the distance units comes at the numerator (like velocity), whereas covariant are those where the distance unit is at the denominator (like temperature gradient).
    
    Covariant vectors are linear funcitonals.
    
    Spherical coordinates:
    ds = dr^2 + r^2 dtheta^2 + r^2 sin^2 theta d phi^2
    g_11 = 1
    g_22 = r^2
    g_33 = r^2 sin^2 theta
    Non constant metric tensor!
    
    g^u_v = delta^u_v
    g^v_u = delta^v_u
    
    
    Riemann tensor symmetries and identities https://en.wikibooks.org/wiki/General_Relativity/Riemann_tensor
    
    Парадокс альфы центавры
    
    TODO: https://en.wikipedia.org/wiki/Four-vector
    I don't like the word "norm" in the article.
    
    
    Twin paradox in closed spaces (for instance, toroidal space):
    
    * Compact space case http://arxiv.org/abs/gr-qc/0101014
    * http://arxiv.org/abs/astro-ph/0606559
    * http://arxiv.org/abs/gr-qc/0503070
    Global preferred inertial frame
    * Jeffrey R. Weeks: The Twin Paradox in a Closed Universe
    
    TODO: okay, what about curved?
    
    'Compactification' breaks the Lorentz invariance.
    * Poincare symmetry
    
    http://van.physics.illinois.edu/qa/listing.php?id=15308
    
    In a closed loop with circumference R, there is a preferred rest frame. Special relativity predicts that someone moving with respect to the loop will measure its circumference as being smaller than R, so the preferred rest frame is one that views the closed loop with its maximum circumference.
    
    https://www.physicsforums.com/threads/twin-paradox-in-a-closed-universe.375432/
    
    gamma m (1, v, 0, 0)
    
    photons:
    
    E (1, 1, 0, 0)
    
    For massive particles: P^\mu = m U^\mu; m is the rest mass
    
    Four-momentum is conserved
    
    Lorentz factor: gamma = 1 / sqrt{1 - v^2}
    
    
    Scalar curvature: an invariant of a Riemannian manifold
    
    Dark energy: cosmological constant??
    
    https://en.wikipedia.org/wiki/Four-vector




# related       [[physics]] [[relativity]]




# `[2018-07-25]` The Meaning of Einstein's Equation      [[baez]]

<http://math.ucr.edu/home/baez/einstein/>  




# make up some crazy metric (e.g. g = Diag[x<sup>2y</sup><sup>2z</sup><sup>2</sup>, 1, 1]) can we do something cool about it?      [[think]]




# susskind lectures      [[study]] [[towatch]]

    General Relativity by Leonard Susskind. Особенно хороши серии 6 и 9. В 9-й type-directed вывод уравнения Эйнштейна, невероятно красиво.




# `[2019-06-18]` MITGameLab/OpenRelativity: An open source framework to add the effects of traveling at relativistic speeds to visualizations or games      [[game]]

<https://github.com/MITGameLab/OpenRelativity>  




## `[2019-06-18]` OpenRelativity: An Open-Source Toolkit for Unity3D by MIT Game Lab - YouTube      [[vr]]

<https://www.youtube.com/watch?v=qol-zP9W5J4>  

    OpenRelativity: An Open-Source Toolkit for Unity3D by MIT Game Lab

nice VR visulaisations of lorenz contraction and redshift  




# <https://flannelhead.github.io/posts/2016-03-11-blackstar.html> 

raytracer on haskell  




# `[2018-11-20]` general relativity - Why is the covariant derivative of the metric tensor zero? - Physics Stack Exchange

<https://physics.stackexchange.com/questions/47919/why-is-the-covariant-derivative-of-the-metric-tensor-zero>  




# `[2018-11-19]` differential geometry - Is there a good way to compute Christoffel Symbols - Mathematics Stack Exchange

<https://math.stackexchange.com/questions/24294/is-there-a-good-way-to-compute-christoffel-symbols>  




# `[2018-11-19]` differential geometry - Why may geodesic not be the shortest path on a surface? - Mathematics Stack Exchange

<https://math.stackexchange.com/questions/1432985/why-may-geodesic-not-be-the-shortest-path-on-a-surface>  




# `[2020-07-21]` [gravitational waves - So Black Holes Actually Merge! In 1/5th of a Second - How? - Physics Stack Exchange](https://physics.stackexchange.com/questions/235307/so-black-holes-actually-merge-in-1-5th-of-a-second-how)

    The same principle applies to the merging black holes. We have two objects that can't actually be real black holes because in any finite universe we know real black holes cannot exist. However they are experimentally indistinguishable from real black holes.




# `[2020-07-21]` [event horizon - What is exactly the density of a black hole and how can it be calculated? - Physics Stack Exchange](https://physics.stackexchange.com/questions/26515/what-is-exactly-the-density-of-a-black-hole-and-how-can-it-be-calculated)

    Alternatively, a super supermassive black hole with the mass of 4.3 billion Suns would have a density equal to one i.e. the same density as water.




# `[2020-07-21]` [general relativity - Is a black hole's mass uniformly distributed? - Physics Stack Exchange](https://physics.stackexchange.com/questions/196542/is-a-black-holes-mass-uniformly-distributed)

    For some reason it is popular to ignore the part where you have to wait a long time and you only get approximately the simple solution. Really it is just that there are only a small number of rather simple back holes that things can approach over time. There are many ways it can be as it approaches the final state. It's like if you leave some hot metal out in a room, there is just one final temperature it approaches, an equilibrium temperature, but it takes forever to reach it, so it is always a bit hotter than the room but starts to get really really really close.




# `[2020-07-21]` [Why does gas form a star instead of a black hole? - Astronomy Stack Exchange](https://astronomy.stackexchange.com/questions/21422/why-does-gas-form-a-star-instead-of-a-black-hole/21434#21434?newreg=7160bc0c46e4439b89cd910f7c72a20e)

    n the present day universe, this does not happen for two reasons. First, the gas is unstable to fragmentation as it collapses. The reason for this is that the Jeans mass, the smallest mass that is likely to collapse, scales as T3/2/ρ1/2, where T is the temperature and ρ the density. If the gas can cool as it collapses, then the temperature remains roughly constant, the Jeans mass falls and the cloud breaks up into smaller cores. These cores are usually much smaller than the (at least) several solar masses required to form a black hole (see below).




# `[2020-07-21]` [Ask Ethan: Does A Time-Stopping Paradox Prevent Black Holes From Growing?](https://www.forbes.com/sites/startswithabang/2020/01/11/ask-ethan-does-a-time-stopping-paradox-prevent-black-holes-from-growing/)

    The thing is, with an extra solar mass of material at just a little more than 3 kilometers away from the predicted central singularity, we now have two solar masses of material in this particular region of space. The event horizon of a two solar mass object is 6 kilometers in radius, meaning that all of this material is now inside the event horizon, after all!




# `[2020-07-21]` [The Best Tower Fans To Cool Down Your Home](https://www.forbes.com/sites/forbes-personal-shopper/2020/07/20/best-tower-fan-2020/)

    Black holes really do grow over time, and all observers can agree exactly when and by how much.

I guess basically, different observers may disagree how big are the black holes.  

For an observer falling into the black hole with a lot of mass, the black hole would be smaller. Whereas for an observer outside the black hole, they might already be inside the 'new' even horizon  




# hmm, how would forces work inside the black hole event horizon if the force carriers can't go backwards?      [[quantum]]




# `[2020-07-14]` [Ask HN: Without Einstein, would General Relativity be discovered by now? | Hacker News](https://news.ycombinator.com/item?id=23450827)

    DavidSJ 36 days ago [–]
    
    David Hilbert discovered general relativity at practically the same moment as Einstein.
    
    gnramires 26 days ago [–]
    
    I believe there was a race at that time, physicists knew there was a need to generalize SR to non-inertial frames, and that perhaps that it involved metric spaces (following the lorentz transformations). Hilbert was working on it, but apparently did not make much progress at deriving the GR equations (I don't have a source, sorry -- scattered articles on GR). You're right that eventually he or someone else would have made it, but how long would it take is speculation.
    
    Edit: More information here https://en.wikipedia.org/wiki/Relativity_priority_dispute
    
    I think the main takeaway is that Hilbert and Einstein ended in amicable terms, and it seems both contributed greatly to eachother's result. 

