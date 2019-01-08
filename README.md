# gecco-19

Author Yuri Lavinas - University of Tsukuba.

Co-Author Claus Aranha - University of Tsukuba.

Co-Author Tetsuya Sakurai - University of Tsukuba.

Working title: New priority functions based on diveristy for resource allocation in MOEA/D
Working title: Resource alocating based on diveristy in MOEA/D
Working title: MOEA/D - New Resource alocation functions based on diversity

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

5.	Results will be comparing a traditional version - MOEA/D-DE - with the four priority functions in different scenarios - 2 benchmark functions and the lunar lading problem.

6.	There are three future works considered:
    
    1.	Is it possible to use priotity functions to other situation: as a measure for adaptive techniques. or another usage?
    
    2.	Consider other priority function, for example, diversity metrics - especially those with mathematical justification and with low computational cost.
    
    3.	Consider reference-based strategy to approximate regions of interested of the Pareto Fronts - maybe not relate, I need to think more about this.
    
    4. Do a two step MOEA/D. 1st step considers the subpopulation from the priority function while the 2nd step considered the other subpopulation.

Outline of the paper.

1. Abstract.

Small summary of the findings of the study. Give the most important characteristics of the work: using MOEA/D and priority functions and the experiments.

2. Introduction.
    
    1. Describe MOPs.
        
        1. Pareto Dominance.
        
        2. Pareto Set/Front.
    
    2. MOEA/D
        
        1. How it is now.
        
        2. Small introduction of works using priority functions.
            
            1. So far two groups: DRA alike and the ones that use archive population.
        
    3. Resource allocation
        
        1. Our idea is to use resource allocation, as others have done, by using priority functions.
        
        2. The novel part is that we isolate the priority functions as the only variation so that it would help us understand how they affect the framework.
            
            1. We use 4 priority fucntions: diversity on the decision space, on the image space, a random and the common used relative improvement (R.I.) from DRA/GRA.
            
3. Related Works **(FOCUS)**

    1. Show that we understand what was studied in the context of Resource allocation and priority functions.

        1. How these work relate to ours and where they differ.
        
        2. Show that we understand where our work fits, that it covers a an area of interest and that we are based on previous works with a good reason.
        
4. Proposed Priority functions **(FOCUS)**

    1. Give their mathematical description of them all.


5.	Experimental design - how to answer the research question.
    
    1. Show what are the algorithms that we are experimenting on. - -DE, 4 priority functions.
    
    2. Show the fuctions we are analysing - UF (benchmark), DTLZ (benchmark) and Lunar landing problem.

    2. Describe parameters.
    
    3. Use of two metrics to evaluate benchmarks - HV (reference points) and IGD while for the Lunar landing problem only the HV (since we do not have a reference pareto front). 

        1. Describe both HV and IGD.
    
    4. Show what statistical analysis is used.

6.	Results. 
 
    1. Figures - Boxplot of HV/IGD values, evolution of HV/IGD of the median execution, and the pareto front found by the median execution.
    
    2. Statistical analysis.
    
    3. Explanation.

7.	Discussion and Conclusion **(FOCUS)**
    
    0. Show the main results. Statistical difference, overall best, overall worst (with and without -de).
    
    2. Show the minor results.

    1. impacts - is it worth to use priority functions? they add complexity in code and in execution time. 
    
    2. Advantages and disadvantages - all priority functions, one by one.
        
        1. advantages - Does it lead to a better search overall? Simple to code? lots of improvement in the performance? Is there any consistency in the results, i.e., is there one priority function that tends to be better then the others? What about the R.I. from DRA: is it better/worse than the others? if it is worse, we have space to improve in terms of priority functions. What do to with the subpopulation that was not prioritized? Leave as it is, or could we do better than that? We can now prioritize characteristics that are interesting for the problem or the decision maker.
        2. disadvantages - hard to code? not much improvement in the performance? Is it easy to understand how the priority function impacts in the performance? Why? How? 
    
    3. limitations - I need to think about this.

