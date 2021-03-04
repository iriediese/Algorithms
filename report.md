# Report for assignment 4

## Project

Name: Algorithms  

URL: https://github.com/iriediese/Algorithms  

It is a library for algorithms written in Java. 
## Onboarding experience

**Did you choose a new project or continue on the previous one?**  
We chose a new project for this assignment.  

**If you changed the project, how did your experience differ from before?**  
We had fewer issues with building and running the project. The previous project used maven which gave us some trouble since each menber of the group got different errors. This project used instead gradle which we were more familiar with and required less troubleshooting.  

## Effort spent

1. plenary discussions/meetings;
    * Meeting 1: 2h
    * Meeting 2: 6h
    * Meeting 3: 3h
    * Meeting 4: 2h
2. discussions within parts of the group;
    * 3h (split work) during Meeting 3 
3. reading documentation;
    * Group allocated 4h for individual reaserch between meetings 1 and 2
4. configuration and setup;
    * Alex: 30m
    * Ioana: 30m
    * Theodor: 30m
    * Joaquin: 30m
    * Johan: 1.5h 
5. analyzing code/output;
    * All of us: 2.5h
6. writing documentation;
    * 3h
7. writing and running code;
    * All of us: 6h

Johan had a bug with the google code standards failing. The bug also showed for other group members, but we found a workaround in the end. Essentially, the code could be compiled and run (outside the intellij environment), and the bug would not always show. At the same time, using an alternative method to compile and run the code (javac instead of gradle) also prevented the bug.  

## Overview of issue(s) and work done.
Title: Add longest increasing subsequence O(n * log n) implementation.  

URL: https://github.com/williamfiset/Algorithms/issues/12  

Summary in one or two sentences  
The previous implementation had quadratic time complexity. The issue was to write a faster, more efficient implementation, with a time complexity of O(n * log n).  

Scope (functionality and code affected).  
Added an alternative, more efficient implementation of a pre-existing algorithm. We have also included tests. The tests also check the previous implementation, and compare the results of the two.  

Title: Add finding all complete subgraphs (cliques) in a graph  

URL: https://github.com/williamfiset/Algorithms/issues/27  

Summary in one or two sentences  
Write an algorithm that finds all subgraphs in a graph. We have also included tests.  

Scope (functionality and code affected).  
Added a whole new class and methods to the project, as well as a testing class and testing methods.  

## Requirements for the new feature or requirements affected by functionality being refactored  

1. O(n * log n) LIS - implement the longest increasing subsequence algorithm in a more efficient way  
2. LIS tests - include tests for newly-added implementation of the longest increasing subsequence algorithm  
3. LIS file formatting - have new files properly formatted according to the google java formatting standard  
4. LIS documentation - have LIS code properly documented (JavaDocs)  
5. Clique - implement algorithm that finds all cliques (complete subgraphs) in a graph  
6. Clique tests - include tests newly-added clique algorithm  
7. Clique formatting - have new files properly formatted according to the google java formatting standard  
8. Clique documentation - have Clique code properly documented (JavaDocs)  

## Code changes

### Patch

for issue #12 (LIS), https://github.com/iriediese/Algorithms/tree/development  
for issue #27 (Clique), https://github.com/iriediese/Algorithms/tree/secondary  

## Test results

The unit tests we have added all pass. We first started out by adding some tests, then improving the functionality of the code itself, so that more tests pass every time.   

Report currently in build/reports/tests/test/index.html  

## UML class diagram and its description

The UML class diagram includes each newly-added class, together with their methods and parameters.    
![UML diagram](https://github.com/iriediese/Algorithms/blob/both/uml.jpg?raw=true)  

### Key changes/classes affected

FindAllCliques.java  
FindAllCliquesTest.java  

LongestIncreasingSubsequenceFast.java  
LongestIncreasingSubsequenceFastTest.java  

## Overall experience

From the ungraded mandatory assingment for this specific task we have learnt a lot about how much each team member has refactured code before. This was a good learning experience for the team.  

As for the essence standard, we managed to finish all of our milestones in time and succeeded to stick to our deadlines. New requirements were introduced early on and the group managed to adapt and formulate a strategy to deal with the new issues. No backtracking was required during this project and the group worked intensively in parallel or as a group at appointed times and in our virtual office that was hosted on discord. This made us able to work more efficiently and root out mistakes before they were implemented. Thus, we have concluded that our team state is 'performing'.    

What are your main take-aways from this project? What did you learn?   
We have learnt how to better contribute to open source projects and include new functionality in a larger project.  

How did you grow as a team, using the Essence standard to evaluate yourself?  
We have gone from a 'collaborating' team state to a 'performing' team state, which we consider a great success.  

Optional (point 6): How would you put your work in context with best software engineering practice?   
We have included javadocs and appropriate comments, and have also used relevant variable names, and good code standards.   
At the same time, our testing suite covers most use cases.   
