# School District Analysis
PyCity Schools Data Analysis Utilizing Python/Jupyter/Pandas

## Overview

The PyCity School District initially asked "the Team" to analyze school and student performance data for directors, board members and stakeholders to annually review. The
first iteration focused on key student metrics for the 15 schools in the district: math and reading scores, their averages, passing percentages in both subjects and
overall passing percentage. This data was then sorted and presented into formats for review by individual school, school type, school spending per student and school
size.

It was during this first assessment that a concern was raised regarding Thomas High School and 9th Grade student data possibly being erroneous. "The Team" was then 
asked to remove the data for this school and grade level, and recomputed a new analysis for comparison. This analysis focuses on this data removal and its effect on
the district's reporting.

## Results
#### District Summary
1. District Summary First Iteration (all data)
![](/Resources/figure03.png)

2. District Summary Amended (Thomas High School 9th grade data removed)
![](/Resources/figure04.png)

* Removing the suspect 9th grade data from Thomas High School had a minimal impact on the overall District metrics: dropping Average Math Score, Average Reading Score, % Passing Math, % Passing Reading and % Overall Passing between 0.1 and 0.3 points.


#### School Summary: Thomas High School
1. School Summary Thomas High School First Iteration (all data)
![](/Resources/figure01.png)

2. School Summary Thomas High School Amended (9th grade data removed)
![](/Resources/figure02.png)

* On the individual school level, removing the 9th grade data for Thomas High School had a drastic impact in metrics. This is to be expected since, in theory, this removes data for approximately 1/4th of the student body. All % Passing scores dropped from values in the 90% range down to the 60% range.
* Calculating just on 10th to 12th grade data restores all % Passing scores to their former values.


#### Relative Performance of Thomas High School (THS) with Amended Data

* Removal of the 9th grade data from calculations moved THS from the one of highest performing school in the district in % Overall Passing (90.95%) to one of the lowest at 65.08%. However, as noted earlier, percentage calculations on just the 10th to 12th grade datasets yield previous results.
* No 9th grade data for THS gives no values (NaN) to compare at the same grade level with other schools in the district.
* There was no variation in output with THS's 9th grade data removal for scores relative to other school spending, other school size or other school type.

## Summary

At first glance, removing THS's 9th grade data had a drastic impact on the school's % Passing Math, % Passing Reading and % Overall Passing scores. This was initially
due to removing data for approximately 1/4th of the student body in calculations. However, calculating against just 10th to 12th grade for THS restored values previously seen. Removal of the 9th grade data for THS had minimal to no impact on overall district statistics given that large aggregate data from the remaining 14 schools in the district.
