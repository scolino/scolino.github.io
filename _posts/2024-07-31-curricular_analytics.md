---
layout: post
title: What is Curricular Analytics and Why do We Care?
---

The field of curricular analytics was born out of the idea that the progression within a university curriculum is cornerstone of a student's academic success. Imagine a curriculum where a student must pass one specific course in order complete any other course in the major. If a student struggles in that course, they are likely to be delayed in graduating or leave school altogether.  Overall, the field analyzes structural and instructional factors of a curriculum from a rigorous, analytic perspective. If researchers can identify bottle necks in curriculums, they can help guide university administrations on curricular reforms that positively influence student outcomes.

## Quantifying a Curriculum
In thier 2018 paper, Heileman et al developed a framework for quantifying the structural and instructional factors of a curriculum (a very interesting read).  Mainly, the overall curricular complexity of a program is a function of instructional complexity, which includes how courses are taught and supported, and structural complexity, which includes the order and prerequisites of the courses.  

The structural factors of a curriculum can be represented as a directed, acyclic graph, where each vertex is a course in the curriculum and the edges connect courses in sequential order in which they must be taken with a curriculum. It is from this graph, and graph algorithms, that the following metrics are derived. 

*Delay Factor*: 
In many STEM curriculums, courses have a pre-req structure that need to be completed in a specific order. Failure to complete a course in the sequence on time can delay students time to graduation since the remainder of the sequence is delayed by one term.  More formally, the delay factor for a given course in the number of course vertices in the longest path in the curriculum graph that passes through that vertex. The overall curriculum delay factor is the sum of the delay factor for each vertex.

*Blocking Factor*:
Blocking factor comes out of the idea that there are highly "important" classes in a curriculum. A highly important class arises from the fact that certain courses are pre-req courses to many other downstream courses in a curriculum. Therefore, the blocking factor measures the number of courses reachable from given course vertex. The overall curriculum blocking factor is the sum of the blocking factor for each vertex.

*Structural Complexity*:
The final metric of overall structural complexity can be calculated from the above metrics.  For a curriculum's structural complexity, we can take an unweighted linear combination of the curriculum's overall blocking factor and overall delay factor. 

## So What?
Heileman et al (2018) point out a few applications for curricular analytics in thier paper. Most importantly to the current project, having a quantifiable way in which to understand curriculum allows researchers to compare across schools and within a school during curricula reform.  As researchers, we can dig deeper into the curricula of similar programs between different schools to better understand how course requirements and pre-req structure differs, and how those differences impact student outcomes.  

For example, the CIC (Lionelle et al. 2024) conducted a study which looked at the impact of curricular complexity on female diversity with students graduating from 4-year bachelor computer science degree programs. They found that the percent of females graduating from CS programs (as per IPEDS completions data) was inversely correlated with the program’s curricular complexity.  Additionally, the study looked at the number of CS courses and the number of math courses with the CS curriculums, finding that differences in either were not significant when looking at differences in female representation.  This could indicate that the courses themselves are not leading to impacts on diversity, but the structure in which the courses assembled within the curriculum.

My current DREAM study expands on the work of Lionelle et al (2024) by focusing on curricular differences within ABET accredited CS programs and non-ABET accredited programs. More specifically, we are interested in the impact that ABET accreditation criteria has the structural complexity of CS programs, and how this complexity may influence diversity within the completions of CS undergraduate programs.


References:
Gregory L. Heileman, Chaouki T. Abdallah, Ahmad Slim, and Michael Hickman. 2018.
Curricular Analytics: A Framework for Quantifying the Impact of Curricular Reforms
and Pedagogical Innovations. (11 2018). http://arxiv.org/abs/1811.09676

Albert Lionelle, McKenna Quam, Carla Brodley, and Catherine Gill. 2024. Does Curricular Complexity in Computer Science Influence the Representation of Women CS
Graduates? Proceedings of the 55th ACM Technical Symposium on Computer Science
Education V. 1. https://doi.org/10.1145/3626252.3630835




