# Closure-of-a-set-of-attributes
INPUT: A set of attributes {A1,A2,A3,......,An} and a set of FD's(Functional Dependencies) S.
OUTPUT: The closure {A1,A2,A3,.....,An}+ 
ALGORITHM: 
1) Split the FD's of S so that each FD in S has a single attribute on the right. 
2) Let X be a set of attributes that eventually will become the closure. Initialize X to be {A1,A2,.....,An} 
3) Repeatedly search for some FD, {B1,B2.....,Bn}->C such that all of B1, B2,......., Bn are in the set of attributes X,    but C is not. Add C to the set X and repeat the search. Since X can only grow, and the number of attributes of any     relation schema must be finite, eventually nothing more can be added to X, and this step ends. 
4) The set X, after no more attributes can be added to it, is the correct value of {A1, A2,.....An}+.     

Source: A first course in database systems (Algorithm 3.7)
