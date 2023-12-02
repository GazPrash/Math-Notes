# Regular and T3 Spaces

## Regular Space

(X, T) is regular iff for every closed 
$$
F \sub X, \exist x \in X
$$
such that 
$$
x \notin F
$$
and with that 
$$
\exist G, H open sets \sub X \\
F \sub G \ and \ x \in H \\
and \ G \cap H = \phi
$$
If we have a Regular space + also T1 then it is called a T3 space

#  Every T3 space is T2

(X, T) is T3, now x, y in X, then we have now wkt X is a T1 space (if it is T3)

so we can say every {x} in X in closed (and so are all the finite sets)

then we have, let any y in X s.t y not in {x}, so we have since X in regular

we can say 
$$
\exist G, H \ st \\
say \ \{x\} \sub G \\
and \ y \ in H \\
G \cap H = \phi
$$
then we can say, there are two open subsets G, H s.t now since {x} in G, we can say  that x in G itself and y in H, so X is T2

# Regular Space prop is hereditary

X, T in regular, let Y sub X, and show Y, T* is regular too

Now let F be a T* closed subset, then we have q in Y s.t q not in F

Now consider Cl(F) = Cl(F) in X ^ Y

Then we can see that F is T* closed so Cl(F) = F

So we have, q not in Cl(F) too

 Now, Cl_x(F) is T* closed and q not in Cl(F) too. 

We can see, (X, T) is regular and Cl_x(F) is closed in X, 
$$
\exist G, h \ st \ q \in G \\
and \ Cl_x(F) \sub H \\
G \cap H = \phi
$$
and now q in Y too so and in G, q in G^Y.
$$
Cl_x(F) \cap Y \sub H \cap Y \\
Cl_x(F) \cap Y = Cl_y(F) = F \\
F \sub H \cap Y
$$
Now consider,
$$
(G \cap Y) \cap (H \cap Y) = \phi \\
take \ G_1 = G\cap Y, H_1 = H\cap Y
$$
They both are T* Open, subsets of Y, now q in G1, and F in H1, while

G1^H1 = phi, so Y, T* is Regular.



# Every compact Hausdorff Space is T3

X,T is compact Hausdorff (T2), now first show X is T1 (it is because T2)

To show:
$$
p \in X \\
\exist F \sub X \ st \ p \notin F \\
\exist G, H \in X \\
F \sub G  \ and \ p \in H \\
G \cap H = \phi
$$
p in X-F, then X is hausdorff, so for each p, x in X, there exist G(x), H(x) s.t
$$
p \in G(x) \ and \ x \in H(x)
$$
C = {H(x) : x in F} is the open cover of F, now F is T-closed, so we can say that since F < X, F is compact too. Now then 
$$
\exist x_i \forall i \in N \\
st \ F \sub \cup \{H(x_i) : x_i, i \in N\} \\
if \ H = \cup {H(x_i)}
$$
and similarly 
$$
G = \cap {G(x_i)}
$$
so we have p in G, since p in G(xi) for all i, so we have , finite union of open sets is open and finite intersection of open sets is also open, consequently, G, H are open. Now F < H, and p not in F, but p in G, since p was arbitary, we have 
$$
G \cap H = \phi
$$
So X is T3.

# T3 Property is Hereditary

X, T is T3, now Y < X, then,

X is regular and T1 => Proove that T1 is hereditary, and regular too

# X is a regular T.S and A is compact subset of X, then if G is an open set containing A, then there exist a closed set H such that 

$$
A \sub H \sub G
$$

Now, let x in A => x in G (A < G)

Now G is open so G is nbd of x.
By a well known result;
$$
\exist H_x \ st \ Closure(H_x) \sub G \\
Now \ \{H_x\} = \{H_x : x \in A\}
$$
will be an open cover of A, and wkt A is compact, so finitely many points exists x1, x2, .., xn st;
$$
A \sub \cup\{H_{x_i} : i = 1, 2, .., n\} \\
then \ Cl(H_{x_i}) \sub G
$$
this is true for each i, and we can say that H = union {Cl(H_xi)}, so we have H is closed (finite union of closed sets), then we also know that Cl(Hxi) < G for all i,
$$
H \sub G \\
H_{xi} \sub Cl(H_{xi}) \ (wkt)
$$
then we can say that,
$$
A \sub H \\
and \ ultimately \ A \sub H \sub G
$$

# Normal Space

(X, T) is said to be normal iff for every pair L, M of disjoint closed subsets of X, there exists G, H s.t
$$
L \sub G \ , M \sub H \\
and \ G \cap H = \phi
$$
A normal T1 space is T4 space.

## Example

X = {a, b, c}, and T = {copy from book}

Now, we have {a}, {b,c} both open and closed, if so they can be L, M and G, H both.
also {a} ^ {b, c} = phi. So the space is normal. Now for T3;

Say we have, {b,c} is closed so we know a not in {b,c}, then we have {a} that is open, so we also have {b,c} that is open and it contains {b,c} also a in {a}.
Then Space is regular. 

For T1, we have for b, c no pair open sets that contain either b or c. 
Not T1 => Not T3

Four Hausdorff, for any two points b, c there doesnt not exist G, H open sets, such that G ^ H = phi. So non-Hausdorff space.

# X is normal if and only if:

$$
F \ (closed) \ \sub X \\
G \ (open) \ \sub F \\
\exist V \ (open) \ st \\
F \sub V \ and \  Cl(V) \sub G
$$

### 1. only if part

X is normal, F is closed in X, now we have G open in X st F < G
Now G' will be closed, st;
$$
F \cap G' = \phi
$$
Now, G' and F are closed in X, so since X is normal we must have U, V such that;
$$
G' \sub U \ , \ F \sub V \\
and \ U \cap V = \phi \\
V \sub U' \\
Cl(V) \sub Cl(U') = U' \ (closed)\
$$
Then we have G' < U => U' < G.
so there exist open set V such that, Cl(V) < G.

### 2. only if

Let L, M be closed subsets of X, and L ^ M = phi, Now consider;
L < M' --> open set

Thus, the closed set L is contained in open set M', so there must exist an open set V, such that L < V and; 
Cl(V) < M' --> M < {Cl(V)}'
So we can say; V ^ {Cl(V)}' = phi. (They have nothing in common)

Now V, and Cl(V)' are two disjoint open sets that are containing, L and M, which are two closed sets in X. So X is normal.

# (R, U) is a T4 space

Now, R, U is T1, we need to show its also Normal.

Now L, M < R be two closed subsets, then we have L ^ M = phi.
$$
let \ l \in L \ and \ l \notin M \\
l \in R - M \\
since \ R-M \ is \ open \\ 
\exist e > 0 \\
(l-e, l+e) \sub R-M \\
therefore \ (l-e, l+e) \cap M = \phi \\
let \ G = \cup \{l-e/2, l+e/2 : l \in L\} \\
Then \ L \sub G
$$
Similarly we could construct, 
$$
H = \cup \{m-n/2, m+n/2 : m \in M\} \\
then \ M \sub H
$$
Now G and H are open sets containing L and M, we need to show they are disjoint.

take x in G^H.
$$
x \in G \ and \ x \in H \\
so \ x \in (l-e/2, l+e/2) \\
x \in (m-n/2, m+n/2) \\
now \\
|l-x| < .5e \ and \ |x-m| < .5n \\
|l-m| = |(l-x) + (x-m)| <= |l-x| + |x-m| \\
|l-m| <= 0.5 + 0.5n
$$
Now if n > e;
Then we have |l-m| < n, so we will have
l in (m-n, m+n) -> contradiction

If e > n;
m in (l-e, l+e) -> contradiction

So hypothesis was wrong and
$$
G \cap H = \phi
$$
so R is Normal, it is already T1, so  R is T4.

