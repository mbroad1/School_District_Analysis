# Module 4 Python and Pandas Challenge: School District Analysis
---
A supervisor in charge of evaluating the school district budget for the following year has asked for a school district analysis using Pandas in Python. In order to make the best decisions for the budget for the coming year, it is important to omit any results regarding the math and reading scores of ninth grade students at Thomas High School as to not skew the data. Likewise, it is important to compare each school's budget with the math, reading, and overall grade outcomes of the students based on different factors like the school size, type of school, and etc.
---
## District Summary

### Updated District Summary:
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20District%20Summary%20DF_Updated.png)
- The **district summary** is unaffected by the new analysis shown above because there were no new scores of reading or math added in this analysis, and no existing scores of reading or math were removed in this analysis.
- The only difference between the new analysis and the older analysis is the formatting of the numbers (see the below image to see the format of the older analysis' numbers)
### Original District Summary:
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20District%20Summary%20DF_Original.png)
---
## School Summary
- In the original analysis for Thomas High School:
  - % Passing Math = 66.91
  - % Passing Reading = 69.66
  - % Overall Passing = 65.08
  
- In the updated analysis for Thomas High School:
  - % Passing Math = 93.27
  - % Passing Reading = 97.31
  - % Overall Passing = 90.95

### Updated School Summary:
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20Summary%20DF_Updated.png)
- The only part of the **school summary** analysis that is affected are Thomas High School's "% Passing Math", "% Passing Reading", and "% Overall Passing" values.
  - These values were affected because in the original analysis (shown in the image below), the 9th graders of Thomas High School were included in the total student count; however, the math scores and reading scores of the 9th graders at Thomas High School are **all** missing.
### Original School Summary: 
![School_District Analysis](https://github.com/mbroad1/School_District_Analysis/blob/main/School%20Summary%20DF_Original.png)
- Since these values are missing, the original calculations for "% Passing Math", "% Passing Reading", and "% Overall Passing" are all skewed to be lower because not all students included in the total for the division to get these percentages have scores (aka, the 9th graders do not have scores).
- Therefore, when you convert the math and reading scores of the 9th graders from Thomas High School to "NaN" (null scores) and exclude the 9th graders in the total student count to get the percentages for math, reading, and overall passing, you will get the right values of what the "% Passing Math", "% Passing Reading", and "% Overall Passing" are actually supposed to be in Thomas High School, which are much higher because the students without scores are not incuded in the total students that are being divided to get the percentages and the nonexistent scores of the 9th graders won't affect the calculations because they are null.
- With the updated analysis, the "% Passing Math", "% Passing Reading", and "% Overall Passing" values of Thomas High School are now similar to those of other charter high schools.
  - Likewise, these respective values are now significantly greater than those of district high schools where previously they were similar or lower to those of district high schools.
---
## How did replacing the 9th grade scores of Thomas High School affect math and reading scores by grade, scores by school spending, scores by school size, and scores by school type?

## Math and Reading Scores by Grade
### Original Math Scores by Grade:
<img src="https://github.com/mbroad1/School_District_Analysis/blob/main/Math%20By%20Grade%20DF_Original.png" width="350" height="500"> 

### Updated Math Scores by Grade: 
<img src="https://github.com/mbroad1/School_District_Analysis/blob/main/Math%20By%20Grade%20DF_Updated.png" width="350" height="500">
- The only score changed by replacing the 9th grade scores of Thomas High School with "NaN" was the average math score for the Thomas High School 9th graders, with the original value of 83.6 being replaced with a "nan"
- No other math score from any other grade nor school was changed due to the replacement of the 9th grade scores with "NaN"

### Original Reading Scores by Grade:
<img src="https://github.com/mbroad1/School_District_Analysis/blob/main/Reading%20By%20Grade%20DF_Original.png" width="350" height="500"> 

### Updated Reading Scores by Grade: 
<img src="https://github.com/mbroad1/School_District_Analysis/blob/main/Reading%20By%20Grade%20DF_Updated.png" width="350" height="500">
- The only score changed by replacing the 9th grade scores of Thomas High School with "NaN" was the average reading score for the Thomas High School 9th graders, with the original value of 83.7 being replaced with a "nan"
- 
- No other reading score from any other grade nor school was changed due to the replacement of the 9th grade scores with "NaN"

