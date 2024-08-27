# Cooperative-Intent
## An Exploration of Computational Learning in a Discrete Preference Space. 

[thesis pdf save-as/](Cooperative-Intent_Thesis_Stanton_2023.pdf)  
Submitted 14th December 2023.  
Conferred 20th March 2024.  
CC-BY.  

DOI: \url{https://doi.org/10.25959/26122150.v1}

@phdthesis{Stanton2024,  
  title        = {Cooperative Intent: an exploration of computational learning in a discrete preference space},  
  author       = {Simon C Stanton},  
  year         = 2024,  
  month        = {March},  
  address      = {Hobart, Tasmania},  
  note         = {Available at \url{https://figshare.utas.edu.au/articles/thesis/Cooperative_intent_an_exploration_of_computational_learning_in_a_discrete_preference_space/26122150/1}},  
  school       = {University of Tasmania},  
  type         = {PhD thesis}  
}  
  
## Abstract

This thesis is an exploration of cooperation, game theory, and machine learning. The aim is to develop a method for profiling cooperative intent as found in the behaviour of learning algorithms over highly constrained games of cooperation; in order to step towards the future use of cooperation-as-policy in the reinforcement learning domain, and contribute to the theory of grounding emergent software systems.

The fundamental question explored is whether an agent can construct an online model—derived from a strictly ordinal 𝟐×𝟐 preference space—of its behaviour, to bridge numerical reward with the symbolism inherent to descriptive game theory models. Identification of a game model has utility in assessing the current state of a system, the current state of an agent, and, to assessing an agents’ cooperative intent, i.e., the cooperatively-contextualised reification of an agent’s internal state representation, or state-of-mind congruent to action. In doing this, the benefits and risks inherent in the anthropomorphisation of machine systems are placed within a mitigatory scope: defining intent, ultimately, as the reification of a trajectory between states (a state being found by a mapping from the agent’s behaviour to any one of the game models in a strictly ordinal preference space) that an agent may experience, which leads to the hypothesis that in nominating target states, and rewarding agents for reaching those targets, the application (via reflection) of cooperation as a policy instrument in machine learning algorithms may deliver beneficial outcomes to the agent and to the system as a whole.

This thesis develops through three sets of experiments that progressively undergo constraint devolution such that the rules and bounds of imperfect- and incomplete-information are (in-part) relaxed, while remaining based in Markov formalism. The initial set of experiments conducts a multi-model tournament to calculate a mutual cooperation rate metric on the performance of algorithms drawn from the game theory, bandit, and foundational reinforcement learning literature. The second set of experiments examines variance in the behaviour of agents under specific conditions of change and confirms that foundational reinforcement learning algorithms are sensitive to isomorphic changes in input; a finding that guides the third set of experiments with the development of a method for reflective-mapping, i.e., the identification of game models in sequential 𝟐×𝟐 matrix games; where agents are constrained by perfect- and incomplete-information visibility. For single agents, this method maps into the strictly ordinal preference space with a one-in-twelve resolution of the correct game model. An external observer, with the relaxed constraint of complete-information, offers singleton mapping into the strictly ordinal space. A singleton mapping is the recognition of an agent’s actions corresponding to the strategic dynamics of the game model constituting the environment.

These experiments are conducted in the context of concepts of cooperation, as have been developed in biological science, and their use in computational learning. This thesis attempts to place machine cooperation as a cooperative mode that is at once like, and unlike, biological cooperation, framed as the latter is by theories of evolution to which machines need not abide. Therefore, constraints that apply to biological modes of cooperation may not apply in an algorithmic context, as machine behaviour can manifest in unexpected, and seemingly irrational, ways. To gain traction on these problems, a descriptivist approach to game theory is pursued in an ethological manner, in order to empirically assess agent behaviour with respect to cooperative dynamics.


## Table of Contents

```
Declaration of Originality ............................................. ii  
Statement of Authority of Access ....................................... ii  
Publications Related to this Research .................................. ii  
Declaration of Code and Data Availability .............................. ii  
Acknowledgements ....................................................... iii  
Table of Contents ...................................................... iv  
List of Tables ......................................................... viii  
List of Figures ........................................................ xi  
List of Algorithms ..................................................... xiv  
Abstract ............................................................... xv  

Chapter One: Introduction .............................................. 1  

1.1 AI Now: Bias, Risk and Aspiration .................................. 2  
1.1.1 Mechanism and Function ........................................... 5  
1.2 Autonomous Agents and Cooperation................................... 6  
1.2.1 Cooperative Intent ............................................... 9  
1.2.1.1 Reflection ..................................................... 11  
1.2.1.2 Intention Recognition .......................................... 11  
1.3 Research Scope...................................................... 12  
1.3.1 On-line .......................................................... 13  
1.3.2 State Information Visibility ..................................... 13  
1.3.3 Infinite Horizon ................................................. 14  
1.3.4 Agent / Environment Boundary ..................................... 15  
1.3.5 No ‘Talk’ ........................................................ 15  
1.4 Thesis Structure and Outline of Experiments ........................ 16  

Chapter Two: Computing Cooperation ..................................... 18  

2.1 Concepts of Cooperation ............................................ 18  
2.1.1 Definitions ...................................................... 19  
2.1.2 Cooperative Modalities in Evolutionary Science ................... 19  
2.1.2.1 Kin-selection .................................................. 20  
2.1.2.2 Reciprocal Altruism ............................................ 21  
2.1.2.3 Group-selection ................................................ 22  
2.1.2.4 Gene-level-selection ........................................... 23  
2.1.2.5 Institutional Cooperation ...................................... 23  
2.2 Computational Learning ............................................. 25  
2.2.1 Learning from a Dilemma .......................................... 27  
2.2.2 Imperfect Information Markov Games ............................... 28  
2.2.3 Practical Considerations for Adaptive Agents ..................... 29  
2.2.3.1 The Problem of Now ............................................. 29  
2.2.3.2 Algorithmic Generalisation ..................................... 30  
2.2.3.3 Discontinuities & Lock-In ...................................... 31  
2.2.4 Algorithm Groups ................................................. 32  
2.3 Computational Game Theory .......................................... 33  
2.3.1 Prisoner’s Dilemma ............................................... 35  
2.3.1.1 Axelrod’s Single-Model Tournament .............................. 36  
2.3.1.2 Related Work ................................................... 38  
2.3.2 Social Dilemmas .................................................. 42  
2.3.3 Taxonomies, Typologies, and Topologies ........................... 44  
2.3.3.1 A Typology of 2×2 Games ........................................ 45  
2.3.3.2 Brams’ Dynamic Game Theory ..................................... 46  
2.3.3.3 Preferential Taxonomies ........................................ 47  
2.3.3.4 A 2×2 Topology ................................................. 48  
2.3.3.5 Further Topological Treatments ................................. 50  
2.4 In Summary ......................................................... 52  

Chapter Three: Robinson-Goforth Space .................................. 54  

3.1 The Reduced RGS Graph, G. .......................................... 54  

Chapter Four: Multi-Model Tournaments .................................. 58  

4.1 Multi-Model Tournament Experiment Type ............................. 60  
4.1.2 Algorithms ....................................................... 60  
4.1.2.1 Game-Theoretic.................................................. 60  
4.1.2.2 Binary Bandits ................................................. 61  
4.1.2.3 Foundational Reinforcement Learning (fRL) ...................... 63  
4.1.3 Evaluation Metrics ............................................... 63  
4.2 Results ............................................................ 65  
4.2.1 Match Pairing Validation ......................................... 66  
4.2.2 Two-Stage Round-Robin Tournament ................................. 66  
4.2.2.1 Game-Theoretic Round-Robin ..................................... 67  
4.2.2.2 Binary Bandit Round-Robin ...................................... 69  
4.2.2.3 Foundational RL Round-Robin .................................... 72  
4.2.2.4 Final Round-Robin .............................................. 74  
4.3 Discussion ......................................................... 77  

Chapter Five: Representational Equivalence ............................. 81  

5.1 Asserting Formal Equivalence ....................................... 84  
5.2 Methodology ........................................................ 86  
5.2.1 Evaluation Metrics ............................................... 88  
5.3 Results ............................................................ 88  
5.3.1 Normality......................................................... 88  
5.3.2 Peak Cooperative Outcome ......................................... 89  
5.3.3 Behavioural Profile Visualisation ................................ 89  
5.3.4 Experiment Group One.............................................. 90  
5.3.5 Experiment Group Two ............................................. 95  
5.3.6 Experiment Group Three ........................................... 97  
5.3.7 Experiment Group Four ............................................ 98  
5.4 Discussion ......................................................... 100  
5.4.1 Principal Finding ................................................ 100  
5.4.2 Distribution Shift ............................................... 101  
5.4.3 Expectations of Stability of Behaviour ........................... 102  
5.4.4 Sources of Stochasticity ......................................... 103  
5.4.5 Validity of the Inequalities ..................................... 103  
5.4.6 Impact on Thesis ................................................. 104  
5.5 Summary ............................................................ 105  

Chapter Six: Game Model Recognition .................................... 106  

6.1 Methodology & Scope ................................................ 108  
6.2 Game Model Recognition ............................................. 110  
6.2.1 Direct Mapping by Reward ......................................... 110  
6.2.2 Preference Mapping by Reward and Behaviour ....................... 112  
6.3 Comparing the Methods .............................................. 114  
6.3.1 Direct Mapping ................................................... 114  
6.3.2 Preference Mapping ............................................... 114  
6.3.3 Three Dilemmas and a Coordination Game ........................... 119  
6.4 Discussion ......................................................... 120  

Chapter Seven: In Conclusion ........................................... 125  

7.1 Empirical and Conceptual Findings .................................. 125  
7.2 Contribution........................................................ 129  
7.3 Future Work ........................................................ 130  

References ............................................................. 133  

Appendix A: Agent Model Overview ....................................... 154  

A.1 Initial Hyperparameter Values ...................................... 156  
A.2 Sources of Variance ................................................ 156  
A.3 Memory Depth ....................................................... 157  
A.4 Energy Use ......................................................... 157  
A.4.1 Energy Use Formula ............................................... 157  
A.4.2 Energy Use Experiment Series One ................................. 157  
A.4.3 Energy Use Experiment Series Two ................................. 158  
A.4.4 Energy Use Experiment Series Three ............................... 159  
A.4.5 Energy Use Total.................................................. 159  

Appendix B: Supplementary Material ..................................... 160  

B.1 rRGS Graph Adjacency List .......................................... 160  
B.2 Experiment Series One .............................................. 163  
B.2.1 Experiment IDs & Analysis Datasheets ............................. 163  
B.2.2 Supplementary Data ............................................... 163  
B.2.3 Tournament Framework Validation .................................. 174  
B.3 Experiment Series Two .............................................. 176  
B.3.1 Experiment IDs & Analysis Datasheets ............................. 176  
B.3.2 Normality Test Data .............................................. 177  
B.3.3 Wilcoxon Signed Rank Test ........................................ 184  
B.3.4 Behavioural Profile Surface Maps ................................. 191  
B.4 Experiment Series Three ............................................ 220  
B.4.1 Experiment IDs & Analysis Datasheets ............................. 220  
B.4.2 Supplementary Data ............................................... 221  
B.5 Code & Data Availability ........................................... 239  
```

## Errata
  
1. p54 I cannot count, obviously.  
 8 May 2024  
 \- where six game models will have six edges  
 \+ where four game models will have six edges  
  
2. pviii missing word   
 1 August 2024  
 \- 4.14: Correlation of TR (reward) and MCR (mutual cooperation rate) ......................................... 77  
 \+ 4.14: Correlation of TR (total reward) and MCR (mutual cooperation rate) ......................................... 77  
  
3. p1 incorrect tense  
 6 August 2024  
 \- AI _safely_; indeed, this question is now becoming an issue with currency rather than remaining solely as a theoretical, and distant, possibility.  
 \+ AI _safely_; indeed, this question has now become an issue with currency, no longer remaining solely a theoretical, and distant, possibility.  
  
4. p2 simplify the sentence  
 27 August 2024  
 \- To achieve this outcome, this research attempts to weave the threads of cooperation, computational game theory, and computational learning together.  
 \+ To achieve this outcome this research attempts to weave the threads of cooperation, computational game theory, and computational learning.  
  
5. p2 rephrase  
 \- Measuring the value of AI in our lives is difficult, and likely to become an ever more intractable undertaking given not just the immense complexity of the interactions of these systems, on society, but also the  
 \+ Measuring the value of AI in our lives is difficult, and likely to become an ever more intractable undertaking given not just the immense complexity of the interactions of these systems with human society, but also, the  
  
  
## GPTZero Assessment of Abstract

[<img src="https://raw.githubusercontent.com/simoncstanton/Cooperative-Intent/3f072150fedf417d59fdb94cbd8e21e72da82069/gptzero-abstract-assessment-lo.jpg">](https://github.com/simoncstanton/Cooperative-Intent/blob/3f072150fedf417d59fdb94cbd8e21e72da82069/gptzero-abstract-assessment.jpg?raw=true)