# Advanced Machine Learning -- Reinforcement Learning

## Activity-Centric Course Blueprint (1-1-1 Model)

### Course Information

-   **Course:** Advanced Machine Learning -- Reinforcement Learning
-   **Programme:** B.Tech CSE
-   **Semester:** VI
-   **Pattern:** 1-1-1 (Lecture + Tutorial + Lab)
-   **Duration:** 15 Weeks
-   **Contact Hours:** 45 (15L + 15T + 15P)

## Vision

Students progressively build an intelligent reinforcement learning agent
throughout the semester. Every activity contributes to a single evolving
GitHub repository.

## Course Outcomes

1.  Explain reinforcement learning concepts and formulate sequential
    decision problems.
2.  Model environments as Markov Decision Processes and evaluate
    policies.
3.  Design RL solutions using Dynamic Programming, Monte Carlo and
    Temporal Difference learning.
4.  Implement and evaluate Deep Reinforcement Learning algorithms using
    modern frameworks.
5.  Critically analyse AI-generated RL implementations and communicate
    design decisions.

## Semester Modules

  Module      Weeks Theme                                 Activities
  -------- -------- ----------------------------------- ------------
  M1           1--2 RL Foundations                                 6
  M2           3--4 MDPs                                           6
  M3           5--6 Dynamic Programming                            6
  M4           7--8 Monte Carlo                                    6
  M5          9--10 Temporal Difference                            6
  M6         11--12 Deep Q Networks                                6
  M7         13--14 Policy Gradient & Actor-Critic                 6
  M8             15 Capstone, Ethics & AI-assisted RL              3

**Total Activities: 45**

------------------------------------------------------------------------

# Weekly Activity Template

Each week contains: - **Lecture:** Concept introduction +
misconception + worked example - **Tutorial:** Guided reasoning + AI
critique + retrieval quiz - **Lab:** Coding + experimentation + GitHub
submission

------------------------------------------------------------------------

# Activity Map (#commment: only design an activity which can be graded, also consider autograding)

## Module 1: Foundations of Reinforcement Learning (Weeks 1–2)

1.  #### Is Reinforcement Learning the Right Paradigm?; Driving Question: Why can't supervised or unsupervised learning solve every sequential decision problem?; Student Evidence: A comparative concept map, A one-page justification; Bloom Level: Analyze; Assessment: Rubric-based(conceptual accuracy, quality of reasoning, clarity of presentation); Feedback: Addressing Misconceptions, Highlighting strength in reasoning, suggesting improvements.
2.  #### Modeling the World as an RL Problem; Driving Question: Can every real-world problem be represented as a reinforcement learning problem?; Student Evidence: A formal RL representation of one real-world problem (e.g., autonomous driving, elevator scheduling, recommendation systems, traffic management), A one-page explanation justifying the choice of states, actions, rewards, and episode termination conditions; Bloom Level: Apply; Assessment: Rubric-based(Correct Indentification of RL components, Justification of modelling decisions, presentation Quality); Feedback: Modelling Assumptions and completeness.
3.  #### Investigating an Unknown Agent; Driving Question: Can we infer an agent's objective only by observing its behaviour?; Student Evidence: Observation log of at least 100 episodes of CartPole, Learning Journal describing behaviour patterns, A hypothesis explaining the agent;s objective and expected reward structure; Bloom Level: Analyze; Assessment: Rubric-based(Quality of observations, logical hypothesis formulation, evidence supporting conclusions); Feedback: Quality of observations, encouragement to refine their hypotheses
4.  #### Evaluating AI as a learning partner; Driving Question: Can we trust AI-generated explanations of Reinforcement Learning?; Student Evidence: An Annotated comparision between an AI-generated explanation and Sutton & Barto's explanation, Identification of at least five conceptual similarities or differences, Recommendation regarding the reliability of the AI explanation; Bloom Level: Evaluate; Assessment: Rubric-based(Identification of conceptual differences, Critical evaluation, Quality of Recommendation); Feedback: Common misconceptions identified by AI
5.  #### Constructing the Reinforcement Learning Knowledge Network; Driving Question: How are the fundamental concepts of Reinforcement learning connected?; Student Evidence: A concept network linking major RL concepts, Short explanations for every relationship shown; Bloom Level: Analyze; Assessment: Rubric-based(Completeness, Accuracy of Relationships, Visual Clarity); Feedback: Improving concept maps after peer discussion
6.  #### Builiding a Research Learning Portifolio; Driving Question: How can evidence collected throughout the semester demonstrate learning?; Student Evidence: Github respository, Portfolio template, reflection describing personal learning goals for the semester; Bloom Level: Create; Assessment: Rubric-based(Portfolio organization, Documentation quality, Reflection); Feedback: Repository Structure and suggestion for maintaining a professional learning portfolio

## Module 2: Markov Decision Processes (Weeks 3–4)

7.  #### Is the world really Markovian?; Driving Question: Do real-world decision-making problems satisfy the Markov Property?; Student Evidence: Analysis of two real-world systems, written argument discussing whether the Markov Property holds; Bloom Level: Analyze; Assessment: Rubric-based(Correct application of the Markov Property, Logical argumentation, clarity); Feedback: Alternative viewpoints and encourage revision
8.  #### Manual Policy Evaluation; Driving Question: Can policy values be computed without programming? Student Evidence: Complete Calculations, Comparision b/w manual calculations and software output, Reflection on observed differences; Bloom Level: Apply; Assessment: Rubric-based(Computational correctness, Interpretation of results, Reflection); Feeback: Mathematical Reasoning, Computational accuracy 
9.  #### Deriving the Bellman Equation; Driving Question: Why is the Bellman equation considered the foundation of Reinforcement Learning?; Student Evidence: Mathematical derivation, Annotated explanation of each derivation step, one-page summary explaining its significance; Bloom Level: Analyze; Assessment: Rubric-based(Mathematical correctness, quality of explanation, Presentation); Feedback: Comments on Correct/Incorrect derivation
10. #### Experiment Analysis of Policy Evaluation; Driving Question: How efficiently does iterative policy evaluation converge?; Student Evidence: Python Notebook, Convergence Plots, Discussion relating convergence to discount factors; Bloom Level: Analyze; Assessment: Rubric-based(Correct implementation, Experimental Analysis, Visualization quality); Feedback: Experimental design, encouragement to use different parameters
11. #### Verifying AI-generated Mathematics; Driving Question: Can AI correctly derive mathematical equations used in Reinforcement Learning?; Student Evidence: Annotated AI derivation, Error identification report, Corrected derivation with justification; Bloom Level: Evaluate; Assessment: Rubric-based(Error identification, correct mathematical reasoning, justification); Feedback: Common Mathematical misconceptions, importance of evidence-based verification
12. #### Which Policy performs best?; Driving Question: Does improving a policy always improve an agent's performance?; Student Evidence: Comparative experimental results, Performance graphs, Evidence-based conclusion identifying the best-performing policy with reason; Bloom Level: Evaluate; Assessment: Rubric-based(Experimental design, Interpretation of results, quality of conclusion); Feedback: Experimental Methodology, afterwards inclusion in sem portfolio 


##  Dynamic Programming (Weeks 5-6)

13. #### Why does value iteration converge?; Driving Question: Why does repeatedely updating state values eventually lead to an optimal policy?; Student Evidence: A visual representation of succesive value updates for a small GridWorld environment, A convergence graph showing value estimates across iterations, A one-page explanation describing why convergence occurs and the role of Bellman Optimality Equation; Bloom Level: Analyze; Assessment: Rubric-based(Accuracy of iterative value updates, Interpretation of convergence behaviour, Quality of visualization and explanation); Feedback: Understanding of convergence, discounting, and recursive updates
14. #### Discovering Dynamic Programming principles; Driving Question: What characterstics of a problem make Dynamic Programming possible?; Student Evidence: Classification of six computational problems as suitable/unsuitable for DP, A justification identifying the presence or absence of optimal substructure and overlapping subproblems, A summary describing the two fundamental principles underlying DP; Bloom Level: Analyze; Assessment: Rubric-based(Correct classification of problems, Quality of reasoning and justification, Clarity of summary); Feedback: Reasoning, common misconceptions, update portfolios
15. #### Comparing Policy Iteration and Value Iteration; Driving Question: Do Policcy iteration and Value iteration always produce the same optimal solution, and how do they differ computationally?; Student Evidence: Python implementations of policy and value iteration, Experimental comparision including execution time, number of iterations, and convergence plots, A comparative discussion identifying the advantages and limitations of each algorithm; Bloom Level: Evaluate; Assessment: Rubric-based(Correct implementation, Experimental comparision, Quality of Conclusions); Feedback: Experimental Methodology, Interpretation of Results, Importance of empirical evidence.
16. #### Designing better Rewards for FrozenLake; Driving Question: Can changing the reward structure produce better learning behaviour without changing the algorithm?; Student Evidence: Three alternative reward designs for FrozenLake, Experimental comparision of learning outcomes under each reward structure, graphical analysis of cumulative rewards and convergence, Evidence-based recommendation identifying the most effective reward design; Bloom Level: Create; Assessment: Rubric-based(Creativity and appropriateness of reward design, Experimental evaluation and analysis, Quality of Recommendation); Feedback: Relationship b/w reward engineering and agent behaviour, experimental design
17. #### Debugging a DP Agent; Driving Question: Can systematic debugging reveal why an intelligent agent fails to learn?; Student Evidence: A debugging report identifying all detected errors, Corrected source code with appropriate documentation, A brief explanation describing how each identified error affected the learning behaviour of the agent; Bloom Level: Evaluate; Assessment: Rubric-based(Identification of implementation errors, Quality of debugging and corrections, Explanation of algorithmic impact); Feedback: Debugging strategies, code quality, reasoning.
18. #### Reflecting on the limits of DP; Driving Question: If DP is optimal, why isn't it used to solve every Reinforcement Learning problem?; Student Evidence: A reflective essay discussing the limitations of DP, A comparision table contrasting DP with model-free reinforcement learning approaches, A concept map illustrating where DP fits within the broader RL landscape; Bloom Level: Evaluate; Assessment: Rubric-based(Conceptual understanding of DP limitations, Depth of critical reflection, Organization and clarity of presentation); Feedback: Individualized feedback highlighting the quality of students' disciplinary reasoning, and their ability to synthesize concepts across the module, Revision and incorporation of final version into sem learning portfolio as evidence of conceptual growth

## Monte Carlo Methods (Weeks 7-8) 

19. #### Can an Agent learn without knowing the environment?; Driving Question: Is it possible for an agent to learn an optimal policy without knowing the transition probabilities of the environment?; Student Evidence: A comparative concept map illustrating the differences betweem model-based and model=free reinforcement learning, A one-page explanation discussing why Monte Carlo methods eliminate the need for explicit transition models, Two real-world examples where Monto Carlo methods are more appropriate than DP; Bloom Level: Analyze; Assessment: Rubric-based(Conceptual understanding of model-free learning, Quality of comparative reasoning, Organization and presentation); Feedback: Conceptual understanding of model-free learning and common misconceptions regarding environment models
20. #### Estimating returns in Blackjack; Driving Question: How can an agent estimate the value of a decision using only experience?; Student Evidence: Manual return calculations for selected Blackjack episodes, Python notebook estimating state values from simulated episodes, Graph showing the convergence of estimated returns as the number of episodes increases, A brief discussion explaining the relationship between sampling and value estimation; Bloom Level: Apply; Assessment: Rubric-based(Accuracy of return estimation, Correct implementation and visualization, Interpretation of convergence); Feedback: Computational accuracy, Sources of Sampling Error, Compare their estimates with theoretical expectations
21. #### Which Monte Carlo strategy learns better?; Driving Question: Does First-Visit Monte Carlo always outperform Every-Visit Monte Carlo, or does the choice depend on the problem?; Student Evidence: Implementations of both Monte Carlo approaches, Comparative graphs showing convergence and value estimates, Experimental report discussing similarities, differences, and situations where one method may be preferred over the other; Bloom Level: Evaluate; Assessment: Rubric-based(Correct implementation of both algorithms, Quality of experimental comparision, Evidence-based conclusions); Feedback: Experimental methodology, Interpretation of results, Encouragement to justify conclusions using empirical evidence rather than intuition
22. #### Building a Monte Carlo Prediction Agent; Driving Question: Can an intelligent agent accurately estimate value functions through repeated interaction with its environment?; Student Evidence: Python implementation of Monte Carlo prediction, Experimental notebook documenting multiple simulation runs, Performance graphs illustrating value estimation over increasing episodes, Reflection discussing the strengths and limitations of Monte Carlo Prediction; Bloom Level: Create; Assessment: Rubric-based(Correct implementation, Experimental design and analysis, Reflection on algorithmic behaviour; Feedback: Implementation Quality, Experimental Design, and Interpretation of Results
23. #### Evaluating AI-generated Monte Carlo implementations; Driving Question: Can AI-generated reinforcement learning code be trusted without verification?; Student Evidence: Annotated AI-generated Monte Carlo code, Error analysis report identifying conceptual and programming mistakes, Corrected implementation with explanations for every modification, Reflection discussing the strengths and limitations of AI-assisted programming; Bloom Level: Evaluate; Assessment: Rubric-based(Identification of implementation errors, Quality of corrections and justifications, Reflection on responsible AI usage; Feedback: AI-generated misconceptions, Evidence-based verification practices
24. #### Peer Review of Monte Carlo investigations; Driving Question: Can scientific peer-review improve the quality and credibility of reinforcement learning experiments?; Student Evidence: A completed peer-review rubric evaluating another students' Monte Carlo Investigation, Written feedback highlighting strengths, weakness, and recommendations, a revised version of their own investigation incorporarting peer feedback, A short reflection describing how peer review influenced the quality of their work; Bloom Level: Evaluate; Assessment: Rubric-based(Quality and fairness of peer evaluation, Constructiveness of written feedback, Evidence of improvement in revised submission); Feedback: Peer-review moderation, Feedback quality validation, Additional Guidance 

## Weeks 9--10 (Activities 25--30)

25. Temporal Difference intuition.
26. TD(0) calculations.
27. Implement SARSA.
28. Implement Q-learning.
29. Compare SARSA vs Q-learning.
30. Mini competition.

## Weeks 11--12 (Activities 31--36)

31. Neural approximation lecture.
32. Experience replay discussion.
33. Implement DQN.
34. Debug DQN instability.
35. AI-generated DQN review.
36. Hyperparameter tuning.

## Weeks 13--14 (Activities 37--42)

37. Policy Gradient derivation.
38. REINFORCE implementation.
39. Actor-Critic implementation.
40. PPO concept seminar.
41. Research paper discussion.
42. Performance benchmarking.

## Week 15 (Activities 43--45)

43. Final capstone integration.
44. Live demonstration and peer evaluation.
45. Reflective portfolio and viva.

------------------------------------------------------------------------

# Assessment

  Component                    Marks
  -------------------------- -------
  Weekly Retrieval Quizzes        15
  Tutorials                       10
  Labs                            15
  Semester Project                10
  SEE Theory                      20
  SEE Practical                   30

## AI Integration

-   Validate AI-generated code.
-   Compare multiple LLM solutions.
-   Document prompt engineering.
-   Explain why generated solutions succeed or fail.

## Semester Project Milestones

Random Agent → MDP Solver → DP Agent → Monte Carlo Agent → Q-Learning
Agent → DQN → Actor-Critic → Final Competition

## Deliverables

-   GitHub portfolio
-   Weekly reflections
-   Lab notebooks
-   Final report
-   Live demonstration
