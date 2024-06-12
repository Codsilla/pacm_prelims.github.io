# Preparation 
I got very lucky as my algorithm's questions were the same as Varun Sivashankar, so I already knew how to solve the first question of that part so I didn't spend much time on the algorithm questions. For the probabilistic method, I quickly skimmed through the proof of LLL and mostly spent my time on the last question which got me to read a similar proof in the book. This proof is somewhat involved and with the stress of the exam, it took me more time than it should have to be able to adapt the proof. For the graph minor part, I spent way too much time ($\approx$ 25 min) to find the proof about the tied quantities and DFS trees. However, during that time, I also found the proof of the next question. I completely gave up on the question about the $2$ $st$ paths as I had only a vague memory that we quickly went over in class at some point and that the proof was way out of my reach with the time remaining. This was also not in the material Paul and I agreed on.



# The Exam
I was given the choice of the order of the subjects.
I choose to start with graph minor as I felt pretty confident in most of my answers. Paul jokingly said that he was dissatisfied with this choice as he wanted to use the time of the other parts to think of hard follow-up questions. I said that, in this case, I made a great choice. We had a good laugh about it.


## Graph Minor
### Question 1
TODO
### Question 2
TODO
### Question 3
TODO
### Question 4
I was very direct and told them that this was not in the material that Paul and I agreed upon for the exam and that I didn't know how to solve it. Paul and Noga were not pleased by this but I think that being this forward was beneficial as I didn't feel like I was "looking dumb" when I was struggling to solve the problem even with their hints. 

### Question 5

## Probabilistic Method

### Question 1 ($\approx$ 10 min)
[Noga] Which version of the theorem do you want to (symmetric or asymmetric)?

[me] Well the symmetric one is just a corollary of the general version so there is not much to prove other than choosing the right weights.

[Noga] Yes I agree, but you can choose to do either.

[me] In that case, I will prove the general one as it contains all the main ideas of why it's true

I then when one to prove the general version. I practiced this proof so many times that I mechanically proved it without much issue other than forgetting to define some variables which Noga and Paul immediately pointed out. Halfway through the proof Noga stopped me and said "Clearly, you know the proof, no need to go further".

### Question 2 ($\approx$ 5 min)
This was a somewhat simple application of LLL and we went through it rather quickly.

### Question 3 ($\approx$ 15 min)
 During my preparation, I realized one of the proofs from Noga's book could be adapted to this problem. The argument had some complicated asymptotics which were mostly skipped in the book which wasn't great. 
I struggled a bit during this one.

Noga asked about this happening for multiple colors at the same time. I said that the proof I just did didn't give it to us for free as we didn't know the dependence between the colors. Noga seemed a bit dissatisfied and said "But we know that we are close to the expectation with high probability for each color". After which I realised that indeed that implied what he asked.

## Algorithms
### Question 1 ($\approx$ 15 min)

I wrote down the LP.
We all joked about the fact that I kept saying random variable instead of just variable when talking about the MILP and the LP relaxation (by that point, I was tired). To get the integer solution from the relaxation, the trick is to notice that each component of the (bipartite) graph induced by the min weight vertices has the same amount of min weight and max weight vertices which allows us to shift weights to make the solution more "integer-like". So not to get confused, I explained this process with an example with weights $0.1$, $0.2$, and $0.9$ (again my brain was semi-fried by that point). We went through all the cases. Huacheng looked satisfied.

### Question 2 ($\approx$ 5 min)

We then went to the second question. Here I explained how we can do the same process as before as long as no two vertices with min weight were connected. This can only happen if the minimum weight is $0.5$. Moreover, if the min weight is $0.5$, there is no reason to have any weight in $(0.5,1)$ as you could always lower that weight to $0.5$ which contradicts the optimality of the LP solution. 

### Question 3 ($\approx$ 10 min)

I was very forward and told them that during my hour and a half preparation, I didn't get to think about that question much and they were understanding.
My initial idea was to use question 2 and to only consider the graph of the vertices with non-zero weights. This didn't quite work. After a hint from Huacheng, I deduced that the idea was to only consider the vertices with weight $0.5$ (and to take all the weight $1$ vertices to complete the vertex cover). This forms a cover because none of the weight $0$ vertices has an edge to the vertex of weight $0.5$, so we are guaranteed that they are covered. This explains why this gives us a vertex cover but not why this is the optimal one. For the optimality, things got a bit messy. After a couple of hints, I slowly understood that if any cover includes one of the $0$ weight vertices, then we can replace it with one of the weight $1$ because of the "Hall-style" condition mentioned in question 1. As my brain wasn't braining anymore, I was having a hard time concluding (the idea is just to prove that after replacing all the vertices with $0$ weight in the cover by ones with weight $1$, we necessarily have all the weight $1$ ones). We stopped there as the time was up.

