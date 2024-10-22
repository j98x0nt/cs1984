java c
STAT 612 (Fall 2024)
Homework Assignment 4
Due Oct.  22, by 11:59 p.m.
Instructions:
1.  This problem set consists of 7 problems (some are multi-part problems) worth a total of 100 points (the points distribution being 10 + 15 + 15 + 10 + 5 + 20 + 25 points, in that order).2.  All submissions must be made online via Canvas as a single pdf ﬁle with your name showing on the ﬁrst page. Your solutions may include typed pages and/or scanned handwritten pages and/or R codes/outputs (if applicable).  But they must be all combined into a single pdf ﬁle.
3.  It is your responsibility to ensure that your uploaded solutions are complete and fully legible, especially if there are scans involved.  If not, the TA may be forced to ignore those parts!
4.  The deadline is strict. No unwarranted exceptions or extension requests will be entertained.
5.  Your proofs/arguments must be rigorous and complete.  Please make sure to show all details of your work, including intermediate steps/reasonings – otherwise points  will be deducted.
6.   You are only allowed to use (without proof) any result from the lecture notes in your solutions– make sure to properly cite them (e.g., slide/result number) when using them in your proofs.
Problems:
1.  For random vectors V1  = (U, W)9  and V2  = (X, Y, Z)9  with a joint distribution, suppose
and conditional on V1 ,

(a)  Derive the marginal (unconditional) distribution of V2 .  [Hint:  use of CFs (carefully!). It is also advisable to prove a general-notation result ﬁrst, then apply it to this case.](b)  Find the distribution of rY + (1 - r)Z conditional on X = x, where r = σz(2)/(σz(2) + σy(2)).(Note: These distributions show up in certain types of interim monitoring problems.)
2.  Suppose
(a)  Find a vector b such that bZ + μ has the same distribution as Y, where Z ~ N (0, 1).
(b) Let G = {G2×2 三 (gij )2×2  | g11 +2g12 +2g21 +4g22  = 1}, and let QG = (Y-μ)/ G(Y-μ). Show that QG ~ χ1(2)(0) for any G ∈ G.
(c) Find an affine set A  ≤ R2   such that P(Y ∈ A) = 1.  Show that for any Y ∈ A, the value of QG is the same for all G ∈ G and that QG ≥ 0, where A is as above.
(d) Suppose Y = (1, 1)/ . Show that for this Y, the value of QG varies over the entire real line (including negative values!) as G varies over G. Why is this behavior. happening?3. Suppose Yn×1 ~ N (μ , Σ) with rank(Σ) ≤ n and μ not necessarily in C(Σ) (unlike Thm. 6and Cor. 2 on Chapt. 3, slides 19–21!). Let Hn×n be symmetric such that ΣH is idempotent,ΣH  0, and rank(HΣ) = rank(H). Show that Y/ HY ~ χk(2)(λ),where k = trace(ΣH) andλ = μ/ Hμ . [Hint: the rank condition on H is related to addressing the issue of μ  C(Σ).]4. Suppose Yn×1  ~ N (μ, σ2 In ), where μ ∈ V for some subspace V ≤ Rn  and σ 2  > 0. Suppose
An×k  is a matrix such that C(A) ≤ V and g : Rn  → Rm  is some function such that g(y + v) = g(y),   for any y ∈ Rn  and v ∈ V.
Show the random vectors Uk×1 = A/Y 代 写STAT 612 (Fall 2024) Homework Assignment 4R
代做程序编程语言and Zm×1 = g(Y) are independent. (Hint: it might help to consider the joint distribution of (In -PA )Y and PAY. Also, note that this result isa generalization of the result that X and Σ(Xi - X)2  are independent for iid Normals.)5. Suppose X1 , X2  are iid N (μ1 , σ 2 ) and Y1 , . . . , Yn  are iid N (μ2 , σ 2 ), and {Xi }i(2)=1 ⊥⊥ {Yj }j(n)=1 .(a) Show that for a suitable choice of K , K(X1  + X2 )/|Y1  - Y2 |  has a t distribution, and
give the values of K, the degrees of freedom and the non-centrality parameter. (b) Show that for a suitable choice of K, the following has an F distribution:
for each a ∈ R,
and give the values of K, the degrees of freedom and the non-centrality parameter.6. Prove the converse direction of Cochran’s Theorem (Chapter 3, slide 29), i.e., the directionnot proved in the slides. Make sure to provide a rigorous and complete proof to get credit.7. Consider the linear regression model: Yn×1 = Xn×kβk×1 + εn×1, with rank(X) = k (and X fixed), E() = 0 and Var() = σ2In. Let βbk×1 = (X0 X)−1X0 Y be the OLS estimator of β.
(a) Show that there exists an orthogonal matrix Pk×k such that P0 (βb − β) ≡ V has zero-mean and uncorrelated components, i.e., E(V) = 0k×1 and Var(V) = ∆k×k for some diagonal matrix ∆. (Make sure to identify clearly what the matrices P and ∆ are!)
(b) Let (Σn)k×k = n1 ni=1 XiXi0(the sample 2nd-moment matrix of X). For any symmetric and nnd matrix Am×m, let λmax(A), λmin(A) ≥ 0 be the maximum and minimum eigenvalues of A, respectively. Then, show that the MSE of βb w.r.t. β satisfies:

(Don’t forget to justify why the constants in the denominators above are non-zero, and why the λmax(·) and λmin(·) definitions as above are applicable to Σbn in the first place!)
(c) For any symmetric nnd matrix A, show that 0 ≤ λmin(A)k vk2 ≤ v0 Av ≤ λmax(A)k vk2, for any v. Using this, show that the coordinate-wise MSEs of βb w.r.t. β further satisfy:

Important: The bounds (1) and (2) establish that as the sample size n grows (i.e., n → ∞), the OLS estimator βb converges to β – as any ‘good’ estimator should! (Recall how the sample mean behaves as an estimator of the population mean.) And the rate of its convergence is 1/√n (coordinate-wise) and p k/n (overall as a vector in Rk, though k is really fixed here). The rate 1/√n is typically the fastest rate any statistical method can achieve (known as the parametric rate as it is achieved only in parametric models).
(d) Assume now that  N(0, σ2In). Using part (a), show that both kbβ−βk2 and kbβk2 are distributed as weighted sums of independent chi-squares, showing clearly (in each case) what the weights are and what the parameters of the individual χ2 distributions are.
(e) Show that k Xβbk2/σ2 ∼ χ2k(δ) and k Xβbk2/(kS2) ∼ Fk,n−k(δ) where δ = k Xβk2/σ2 and S2 = k Y −Xβbk2/(n−k). [S2 more generally defined in Chapter 4 even if rank(X) ≤ k.]







         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
