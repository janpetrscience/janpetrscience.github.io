---
layout: post
title: Our work with Gaurav Kucheriya, Allan Lo, Amedeo Sgueglia and Jun Yan on ordered Ramsey numbers is on arXiv!
date: 2026-03-16
inline: false
related_posts: false
---
The preprint is [here](https://arxiv.org/abs/2603.12358).

In graph theory, [Ramsey's theorem (1930)](https://londmathsoc.onlinelibrary.wiley.com/doi/abs/10.1112/plms/s2-30.1.264) states that for any fixed graph $H$ any $2$-edge-colouring of a sufficiently large complete graph contains a monochromatic copy of the given graph. Of interest is the minimum number of vertices (the Ramsey number of $H$, denoted $R(H)$) for this sufficiently large complete graph $K_N$ to contain a monochromatic copy of $G$ no matter the $2$-edge-colouring of $K_N$. For example, $R(K_3)=6$, $R(K_4)=18$ and the precise value of $R(K_5)$ is not yet known. The most relevant value for our research is the Ramsey number of a path on $n$ vertices ($P_n$) obtained by [Gerencsér and Gyarfás (1967)](https://www.renyi.hu/~gyarfas/Cikkek/01_GerencserGyarfas_OnRamseyTypeProblems.pdf): $R(P_n)=\lfloor 3n/2 \rfloor-1$.

There are structures other than graphs for which analogues of the graph-theoretic Ramsey's theorem hold. For example, the ordered graphs -- graphs where the vertices are equipped with a total order. A copy of an ordered graph $H$ in $G$ is now asked to preserve not only adjancences, but also the order. The ordered Ramsey number of $H$, denoted $R_<(H)$, is well-defined and satisfies $R(H) \leq R_<(H) \leq R_<(K_{\mid V(H)\mid})$. Changing the total order of the vertices of $H$ can change the behaviour of $R_<(H)$. Considering a monotone path $MP_n$ where the vertices encountered along the path grow from the smallest to the largest. This problem of finding $R_<(MP_n)$ corresponds to finding the smallest $N$ such that any sequence of $N$ distinct numbers contains a monotone subsequence of length $n$. The classical [Erdős-Szekerés theorem from 1935](https://www.numdam.org/article/CM_1935__2__463_0.pdf) gives $R_<(MP_n)=(n-1)^2+1$.

On the other hand, there are orderings of $P_n$ that have a linear ordered Ramsey number, leading to a value closer to $R(P_n)$. One such ordering gives the alternating path on $n$ vertices, $AP_n$. From one end to the other, the path starts at the smallest vertex, then visits the largest, then the second smallest, then the second largest... In one of the two papers that started a systematic study of the ordered Ramsey numbers, [Balko, Cibulka, Král, and Kynčl (2020)](https://www.combinatorics.org/ojs/index.php/eljc/article/view/v27i1p16) proved $5\lfloor n/2\rfloor-4\leq R_<(AP_n)\leq 2n-3+\sqrt{2n^2-8n+11}$. Moreover, they asked whether among all possible orderings of $P_n$ it is $AP_n$ which minimises the ordered Ramsey number -- a question that is still open.

Our main contribution is an improved upper bound on $R_<(AP_n)$, namely $R_{<}(AP_n)\leq2n-2+\lfloor \frac{\sqrt{2(n-2)^2+(-1)^n}-1}{2} \rfloor$. Our proof starts with an idea from a paper about ordered Turán numbers by [Balko, Jelínek and Valtr (2019)](https://www.sciencedirect.com/science/article/pii/S0095895618300492#!): removing left-most or right-most edges from certain vertices in $n-2$ steps so that if any edge remains at the end of the process, the underlying graph contained a copy of $AP_n$. Purely adapting their approach to the Ramsey setting (removing an edge of each colour from analogously selected vertices) would lead to an upper bound of $(4+o(1))n$. We improve on it by considering only certain copies of $AP_n$, namely those that have their odd vertices in $\{v_1,\ldots, v_a\}$ and even vertices in $\{v_b,\ldots,v_n\}$. This allows us to remove fewer edges in each step of the algorithm; we only need to keep a careful track of the number of edges that can never appear in any such monochromatic copy of $AP_n$. Taking the optimal choices of $a$ and $b$ for this approach we obtain the claimed upper bound.

Despite not expecting our result giving the precise value of $R_<(AP_n)$ it curiously gives correctly all known values, i.e. $n\leq 13$, as given by [Poljak (2023)](https://dspace.cuni.cz/bitstream/handle/20.500.11956/182079/120445995.pdf?sequence=1). In our paper we also consider a few other related ways to order $P_n$ and study their ordered Ramsey numbers. For these orderings, as well as for $AP_n$, we also study their ordered Turán numbers. A recent related and independent work on ordered Turán numbers including an overlapping result is due to [Barát, Freschi and Tóth (2025)](https://arxiv.org/abs/2512.15461).

This project was initiated during [Topics in Ramsey theory](https://sparse-graphs.mimuw.edu.pl/doku.php?id=sessions:2025sessions:2025session1) online workshop organised by Stijn Cambie, Nemanja Draganić, António Girão, Eoin Hurley, and Ross Kang.

Personal webpages of the coauthors:
* [Gaurav Kucheriya](https://sites.google.com/view/gauravkucheriya/home)
* [Allan Lo](https://web.mat.bham.ac.uk/S.A.Lo/)
* [Amedeo Sgueglia](https://amedeosg.github.io/index.html)
* [Jun Yan](https://warwick.ac.uk/fac/sci/maths/people/staff/yan/)
