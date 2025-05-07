# Production_System
## 🎯Objective:
Build a simple Production System capable of inferring new facts based on a set of predefined rules and initial facts using **Forward Chaining** and **Backward Chaining** techniques.
## 📌 Key Points:
1. Read Rules and Facts from Files; parse both files and convert them into a structured format for processing:
    - provided with two text files: 
        - rules.txt: Contains all the production rules 
        - facts.txt: Contains a list of known initial facts. 
2. Implement Forward Chaining from scratch. 
3. Implement Backward Chaining from scratch. 
4. Print facts each cycle in two algorithms. 
## 🧩 How To Solve?
### 1. Forward Chaining:
```
Given a certain set of facts in the working memory, use the rules to generate new facts until the desired goal is reached. 
    1. Match the IF part of each rule with facts in working memory.
    2. Fire (use) the rule that match.
    3. If new facts are obtained add them to working memory.
    4. Stop (or exit) when the conclusion is added to the working memory or when no more rules could be used [Either that 'All rules were fired' or 'Not enough Facts to Fire another rule'].
```
### 2. Backward Chaining:
```
Works backwards from a hypothesized goal, attempting to prove it by linking the goal to the initial facts.
    1. Select rules with conclusions matching the goal.
    2. Replace the goal by the rule's premises. These become sub-goals.
    3. Work backwards until all sub-goals are known to be true [Achieved either by 'Facts (in the working memory)' or 'Information is provided in other rules']
```