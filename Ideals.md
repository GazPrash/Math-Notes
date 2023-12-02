# Abstract Algebra - Ideals

## Question

We have I  = <a> , and J = <b>, now then find IJ< I+J, I^J, here a,b are integers.

Now then, let I+J = U = <d>, now then, d = gcd{a, b}. Let I^J = V, where V = <c> = lcm{a,b}. Then IJ = W = <ab>. Now;
d = gcd(a, b) now then d|a and d|b. Then it means;
$$
a = n_1 * d \\
b = n_2 * d \\
so \ a \in \langle d\rangle \\
b \in \langle d\rangle \\
so \ \langle a\rangle \sub \langle d\rangle \\
\langle b\rangle \sub \langle d\rangle \\
so \ \langle a\rangle + \langle b\rangle \sub \langle d\rangle \\
\exist x,y \in Z \\
d = ax + by \\
\langle d\rangle \sub \langle a\rangle + \langle b\rangle \\
equality \ follows
$$
Similarly for c = lcm{a, b}, we have a|c, b|c and so we can say <c> in <a> and <c> in <b>, in fact belongs in their intersection. Now if x in <a>^<b>, then a|x and b|x, but then lcm{a,b} also | x, so c|x which leads to equality.

For the third, we have a in <a> and b in <b> now so ab in <a><b> or we have;
$$
\langle ab \rangle \sub \langle a \rangle \langle b \rangle
$$
Just need to prove vice versa.

## Maximal Ideal

Non Zero Ideal S != R, we have is maximal if there is no proper ideal of R containing S. 

### J = <4> is a max ideal of E = <2>

For this, we know that 2 not in <4>, then we have J != E, now K be an ideal such that J contained in K (assume). Now K < E (proper ideal). Then;
$$
\exist x \in K \ st \ x \notin J \\
$$
Now x cannot be a multiple of 4, so x = 4m + r (say), r = 1,2,3
Then if we analyze cases for r, we deduce that 2 not in E => So E = K.
Thus J is the max ideal.

## Simple Ring

1. If R (ring), then there exists a,b in R, st ab != 0
2. R has no proper ideal or R is with unity and has no proper ideal.

### Every Field is a Simple ring because Ideals of Field F are F and {0} only.

#### Show R = <{0,1,2,3,4,5}, +5, *5> has no proper ideal

Now  R has no a,b st ab = 0 (5 is prime).
Assume I is a proper ideal, then say;
$$
r \in R \ and \ a \in I \\
ra \in I \\
now \ 1 \in I \ (I \sub R) \\
r \cdot 1 \in I \\
R \sub I \\
R = I
$$
Alternate;
$$
\forall r \in R\\
ra \in I \ (a \in I) \\
if \ r = 1 \\
r * a 
$$


##### I^2 = finite sum of {ai*bi}.

## Nilpotent Ideal

I (ideal) of R is nilpotent ideal if for some +ve int n;
$$
I^n = \{0\}
$$


## Nil Ideal

I of R is said to be nil ideal if each element of I is nilpotent i.e
$$
\forall a \in I , \exist n \\
a^n = 0
$$


Every Nilpotent ideal is Nil ideal, converse not true.

# Factor/Quotient Ring

## Factor Ring

I be an ideal of R, then R/I as the set {a+I : a in R}, with the operations;
$$
(a+I) + (b+I) = (a+b) + I \\
(a+I)(b+I) = ab + I
$$
R/I forms a ring.

### Consider I = {6n : n in Z} of the ring Z, then show it is not an ID.

If ab = 0 st a!=0 and b!=0 then it is not ID.
Now consider (2 + I)(3 + I) = 0, even though 2+I and 3+I are not equal to 0.
So I is not an Integral Domain.

# Theorem 33

##### If R is a commutative ring with unity, then R/M is a Field iff M is a maximal ideal of R.

Let M be max ideal of R.
Then R is comm with unity. Now R/M inherits the props, so we have to show that R/M is a field. Now so we have to show every non-zero element in R/M is a unit.
$$
let \ x' \in R/M \\
x' = x + M \ (x \in R) \\ 
xR = \{xr : r \in R\} \\
xR \sub R \\
M \sub xR
$$
Now x in M cannot be 0 so we conclude;
$$
0 \notin M \\
M \sub xR \\
M \neq M + xR = R\\
\exist xr \in xR \ st \ xr \in M \\
but \ M \sub xR \\
xr \notin M \\
implies \ 1 = xr+m \ some \ m \in M \\
1 = xr\\
$$
so x must be a unit. Hence R/M is a field.

For the converse;
$$
1 \notin M \ (\because M \neq R)\\
\exist I \ M \sub \ I \sub R \\
\exist a \in I \ st \ a \notin M \\
so \ a \neq 0 \\
\exist b \in R \\
ab = 1 \\
ab + M = 1 + M \\
1-ab \in M \sub I \\
a \in I \ and \ b \in R \\
ab \in I \ (ideal) \\
1 \in I \\
I = R
$$
So we can see that since I = R, M is the maximal ideal in R.

### nZ is maximal in Z iff n is prime

say nZ is maximal in Z, now we assume n = ab.
then if nZ is maximal so Z is commutative and has unity, then construct Z/nZ.
$$
Z/nZ = x + nZ \ (x \in Z) \\
$$
Will come to this later...

## Prime Ideal

R is commutative ring, an ideal P of R is called prime ideal if for all a,b in R whenever;
$$
when \\
a,b \in R \\
ab \in P \\
it \ follows \\
a \in P \ or \ b \in P
$$
if R is an ID, then <0> is a prime ideal of R because ab in <0> implies that ab = 0, which leads to either a = 0 or b = 0, hence a in <0>  or b in <0>.

in Z, I = <3> is a prime ideal, because;
$$
ab \in I \\
ab = 3n \\
3 | ab \\
3 | a \ or \ 3 | b \\
a = 3m_1 \ or \\
b = 3m_2
$$
then a in <3> or  b in <3> , so I = <3> is a prime ideal.

#### Quotient ring R/M is an integral domain,  iff M is a prime ideal, a = 0 or b = 0 must imply a in M or b in M.

Now, if so lets assume R/M is ID, then wkt it has no zero divisors, then let ab in M;
$$
ab = 0 \in R/M \\
ab \in M \\
a = 0 \ or \ b = 0 \ (\because R/M \ is \ ID) \\
a \in M \ or \ b \in M \\
$$
so M is a prime ideal.

Conversely, we can say M is a prime ideal, then if ab = 0 in R/M we have ab in M leading to a in M or b in M, then a = 0 or b = 0 if ab = 0, so R/M is an ID.

#### R is a commutative ring with unity, then so is  R/M

Now if x in R, then R/M = x+M, then wkt;
$$
1 \in R \\
1 \in M 
$$
because M is an ideal of R, and R has unity, so subring shares the same unity.
Then, we have say;
$$
a,x \in R \\
x = 1 \\
(x+M) * (a + M) = (a * 1 + M) \\
$$
So we can see that (1 + M) is the identity of R/M so it also has unity, similarly;
$$
(a+M) * (b + M) = (ab + M) \\
(b+M) * (a + M) = (ab + M) \\
$$
So it is also commutative.

#### Every maximal ideal is also prime ideal

let M is the maximal ideal, then it must correspond to the field, R/M, so a field is an integral domain, M is a prime ideal.

Converse of above is not true, as <0> is a prime ideal but not a maximal ideal in Z, as <2> is an ideal such that;
<0> sub <2> sub <Z>.