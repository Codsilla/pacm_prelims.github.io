**Date**: Thursday May 9, 2024\
**Committee**: Noga Alon [N], Maria Chudnovsky [M], Huacheng Yu [H]\
**Topics**: Probabilistic Method, Graph Minors, Algorithms

# Preparation

I was comfortable with all but one of the graph minors questions so I didn't spend too much time on it. For probabilistic method, I wrote down some short notes on details I thought I might forget on the spot and worked out the Azuma problem. For algorithms, I wrote down a sketch of a very incorrect solution which I realized only during the discussion time. 

# The exam
## Graph Minors

**Q1.** Discuss some theorems of the form "If $\vert E(G)\vert  > f(\vert V(G)\vert )$, then $G$ contains some minor". Prove that if $\vert E(G)\vert  > 2^k \vert V(G)\vert $, then $G$ contains $K_k$ as a minor. 

I mentioned Euler's formula implying a $K_{3,3}$ minor or $K_5$ minor. Noga then asked for a theorem implying a single minor, so I said that n edges trivially implies a triangle minor. I then sketched the proof of the $K_k$ minor question.

**Q2.** Suppose G contains H as a minor where H has maximum degree 3. Prove that G contains a subdivision of $H$.

**Q3.** Suppose G is $3$-connected and contains a subgraph isomorphic to a subdivision of $K_5$. Show that either $G = K_5$ or $G$ contains a $K_{3,3}$ minor. 

**Q4.** Prove that the chromatic number of G is at most $tw(G) + 1$. 
I did it the natural way by drawing the tree decomposition and coloring vertices by going down the tree. Maria was fine with but said she had a different proof in mind.

**Q5.** Show that $tw(G)$ is the smallest $w$ for which there exists a tree $T$ such that $G$ is a subgraph of the intersection graph of subtrees of $T$, and every vertex of $T$ appears in at most $w+1$ of the subtrees. 

We didn't get to this question during the prelims and I had not worked it out during my prep time but it's not so bad once you stare at it. 

## Probabilistic Method

There was a standard Ramsey question and a question on the threshold function for every $n/2$ vertices of $G(n,p)$ containing a 5-cycle (which was a homework question from class). 

I then had to sketch a proof of Azuma's inequality. The next question was based on Azuma:
Show that for any eps > 0, there is a $C = C(\varepsilon)$ such that every set $S$ of at least $\varepsilon  4^n$ vertices in $(Z_4)^n$ contains $4$ vectors so that the Hamming distance between any pair of them is at least $n - C\sqrt{n}$. Hint: Show that no more than $3/4$ of the vectors are within distance $C \sqrt{n} / 2$ of $S$. 

I proved the hint easily, got a little confused while completing the argument but solved the problem with some prompting. 

Noga then asked an optional question not given during prep time: prove that $G(n,1/4)$ contains a perfect matching whp. I said you could use Hall's theorem, which he was happy with. 

## Algorithms

**Q1.** Write down an LP for min vertex cover. If G is bipartite, prove that we can round to an integral solution with the same cost. \
**Q2.** For general graphs, prove that we can round to a half-integral solution with the same cost (all vertex weights in $\\{0,1/2,1\\}$).\
**Q3.** Given $k \leq n$, design a polynomial time algorithm that outputs a graph $H$ on at most $2k$ vertices such that $G$ has a vertex cover of size $k$ iff $H$ does. 

I really struggled with algorithms. During prep time I thought I had a solution to the first couple of problems but realized my approach was very wrong when I started writing it out on the board. I then got super flustered and it took me a LOT of hints to get Q1 and Q2, and we ran out of time before getting into Q3 properly. 

# Conclusion

Overall, graph minors and probabilistic method went as well as I could have hoped for, but I definitely didn't do very well on algorithms. Noga, Maria and Huacheng were all super friendly and helped me if I got stuck on something. I would recommend starting with the topic you feel most confident about.

