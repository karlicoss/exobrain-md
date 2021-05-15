
# Table of Contents

-   [`[2016-07-30]` Conway games](#mthwrldwlfrmcmcnwygmhtmlcnwygms) 
-   [= ({0}, {0}) = {0|0}](#527_2073) 
-   [related](#rltd) [[math]]





# `[2016-07-30]` [Conway games](http://mathworld.wolfram.com/ConwayGame.html)

1.  L, R : sets of games, then G = <L, R> is a game
2.  DGC: no infinite sequence of games G<sup>i</sup> = <L<sup>i</sup>, R<sup>i</sup>> with G<sup>(i+1)</sup> &isin; L<sup>i</sup> &cup; R<sup>i</sup> for all i &isin; N

L and R are left and right options of G.  

G = {L<sub>1</sub>, L<sub>2</sub>, &#x2026; L<sub>n</sub> | R<sub>1</sub>, R<sub>2</sub> &#x2026; R<sub>m</sub> }  

0  = ({} , {})  = {|}  
1  = ({0}, {}}  = {0|}  
-1 = ({} , {0}) = {|0}  




# = ({0}, {0}) = {0|0}

n = {n - 1|}  
1/2 = {0|1}  

Conway induction: ICGN. 0 satisfies automatically.  
Proof: infinite sequence of games not satisfying the property, contradiciton.  

Conway induction implies DGC  

Finitely many positions: short  

Same moves: impartial game  

Abelian group:  

1.  0 = {|}
2.  G + H = {(G<sup>L</sup> + H) &cup; (G + H<sup>L</sup> | (G<sup>R</sup> + H) &cup; (G + H<sup>R</sup>)}
3.  -G = {-G<sup>R</sup> | -G<sup>L</sup>}

The set of all Conway games forms a partial order with respect to the comparison operations:  

1.  G=H. If the second player to move in the game G-H can win (G and H are equal).
2.  G||H. If the first player to move in the game G-H can win (G and H are fuzzy).
3.  G>H. If Left can win the game G-H whether he plays first or not (G is greater than H).
4.  G<H. If Right can win the game G-H whether he plays first or not (G is less than H).

A basic theorem shows that all games may be put in a canonical form, which allows an easy test for equality. The canon  
ical form depends on two types of simplification:  

1.  Removal of a dominated option: if G={{L<sub>1,L</sub><sub>2</sub>,&#x2026;}|G<sup>R</sup>} and L<sub>2</sub>>=L<sub>1</sub>, then G={{L<sub>2</sub>,&#x2026;}|G<sup>R</sup>}; and if G={G<sup>L</sup>|{R<sub>1,R</sub>\_

2,&#x2026;}} and R<sub>1</sub>>=R<sub>2</sub>, then  G={G<sup>L</sup>|{R<sub>2</sub>,&#x2026;}}.  

1.  Replacement of reversible moves: if G={{{A<sup>L</sup>|{A<sup>(R<sub>1</sub>)</sup>,A<sup>(R<sub>2</sub>)</sup>,&#x2026;}},G<sup>(L<sub>2</sub>)</sup>,&#x2026;}|G<sup>R</sup>}, and A<sup>(R<sub>1</sub>)</sup><=G, then G={{{A^

(R<sub>1</sub><sup>L</sup>)},G<sup>(L<sub>2</sub>)</sup>,&#x2026;}|G<sup>R</sup>}.  

G is said to be in canonical form if it has no dominated options or reversible moves. If G and H are both in canonical  
 form, they both have the same sets of left and right options and so are equal.  




# related       [[math]]

