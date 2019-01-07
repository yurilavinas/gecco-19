# gecco-19

Author Yuri Lavinas - University of Tsukuba.

Co-Author Claus Aranha - University of Tsukuba.

Co-Author Tetsuya Sakurai - University of Tsukuba.

Working title: Understanding priority functions in MOEA/D.

Topic of Study: Multiobjective problems - benchmark functions.

1.	The specific objective of this study was to investigae how priotity functions relate to MOEA/D in terms of performance and how do they influence in their results. We consider four different priority functions: diversity on the image space, in the decision space, a random and the relative improvement (from MOEA/D-DRA). 

2.	There are a few already proposed algorithms. In them, utility functions are used with other variations.Hence, it is not clear how priority functions influence the search of MOEA/D. 

3.	I need to focus on the methodology and results, since describing the methods clearly have a major role here. The results section is also important to show in practice how the priority functions results and what can we can learn from that. Then, it is crucial to demonstrate how each priority function work and how do they influence the results.

4.	Most of the background needed to understand this study are:

    1.	what are multiobjective problems and why are they important.
    
    2.	how are they addressed, show evolutionary algorithms that are used for MOP.
    
    3.	place MOEA/D among them.
    
    4.	describe MOEA/D variants that deal with resource allocation.
    
    5.	describe their limits.

    6.	demonstrate why this study is of relevance.

5.	Results will be comparing a traditional version - MOEA/D-DE - with the four priority functions in different scenarios.

7.	There are three future works considered:
    
    1.	Use this metric as a measure for adaptive techniques.
    
    2.	Consider other diversity metrics - especially those with mathematical justification and with low computational cost.
    
    3.	Consider reference-based strategy to approximate regions of interested of the Pareto Fronts.
    
    4. Do a two step MOEA/D. 1st step considers the subpopulation from the priority function while the 2nd step considered the other subpopulation.

Outline of the paper.

1. Introduction.
    
    1. Topic and importance of it.
    
    2. related works.
    
    3. research addressing the problem - giving subproblems different amount of evaluations.

2.	Experimental design.
    
    1. how to answer the research question.
    
    2. why this method.

3.	Results. 
 
    1. Figures.
    
    2. Statistical analysis.
    
    3. Explanation.

4.	Discussion 

    1. impacts.
    
    2. advantages.
    
    3. disadvantages.

5.	Conclusion.
    
    1. main results.
    
    2. limitations.
    
    3. future works.

