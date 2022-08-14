# School District Analysis
# Overview  
The purpose of the School District Analysis is to gather various metrics on school data to deliver the results to a school board. With the focus on the math and reading scores from different schools, our goal was to see how the students performed, how schools ranked among each other, and determine a school's budget and budget per capita. When the School Board noticed dishonesty among the results of Thomas High School's 9th graders, our objective was then to re-run the analysis without those scores being accounted for and see if they had a significant difference on the district summary as a whole. 

# Results of the School District Analysis

### How is the district summary affected?
When we re-ran the district summary analysis after removing scores, we saw only a small change from the original analysis. When we dropped the 9th grade math and reading scores, we were still taking into account all grade levels from the other 14 schools and 10th-12th grade scores from Thomas High School. Removing one grade level from one school had a less then 1% impact on the district summary due to there only being less than 500 9th grade scores from Thomas High School compared to the over 39,000 other students grades that are being taken into account. 

### How is the school summary affected? 
![PerSchoolSummary_original](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/PerSchoolSummary_original.PNG)
After re-running the analysis, Thomas High School's overall passing percentage dropped from a 91% overall passing rate, as seen in the original photo above, to a 65% overall passing rate. When we dropped the 9th grade reading and math scores and only accounted for the 10th-12th grade scores, this caused the rest of the data to correct itself and the new number are based only off of those three grade levels. 
![PerSchoolSummary_new](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/PerSchoolSummary_new.PNG)
### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
In the original analysis, when we ran the top five schools, Thomas High School placed second due to their 91% overall passing score. 
![OriginalTopFive](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/OriginalTopFive.PNG)
In the updated analysis, when Thomas High Schools overall passing percentage dropped to 65%, this caused them to drop out of the top five and move further down the list. 
### How does replacing the ninth-grade scores affect the following:
1. Math and reading scores by grade

In the following images the original math and reading scores analysis by grade can be seen on the right and the new scores on the left. When we removed the 9th grade scores for Thomas High School it caused those values to turn to NaN instead of the original 83.6 and 83.7% because we are no longer taking them into account. 
![MathScoresByGrade](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/MathScoresByGrade.PNG)
![ReadingScoresByGrade](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/ReadingScoresByGrade.PNG)

2. Scores by school spending

In both the original analysis and the updated analysis Thomas High School falls into the $630-$645 spending bracket. Removing the 9th grade math and reading scores did not have much of an impact on this analysis. 

3. Scores by school size

The scores by school size also did not see a great amount of change when we removed the 9th grade scores for Thomas High School. Thomas High School still falls into the Medium size(1000-1999) school category, as seen below. There was a slight difference in the overall passing % column, but not significant enough for Thomas High School to change the bin it falls in to. 
Original School Size:
![OriginalSchoolSize](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/OriginalSchoolSize.PNG)
New School Size:
![NewSchoolSize](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/NewSchoolSize.PNG)

4. Scores by school type

Scores by school type did not have a significant change after we removed the 9th grade scores from Thomas High School. The numbers of the overall passing percentage had a slight change but not significant. 
Original School Type: 
![OriginalSchoolType](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/OriginalSchoolType.PNG)
New School Type:
![NewSchoolType](https://github.com/aarce21/School_District_Analysis/blob/main/Resources/NewSchoolType.PNG)
# Summary 
One of the major changes we saw after changes the scores for Thomas High School's 9th graders to NaN's is that the school's overall passing percentage dropped from 91% down to 65%. This is a drastic decrease and also led to another change. In the original analysis, Thomas High School placed second among the top five performing schools. Removing the scores and re-running the analysis caused them to lose their second place spot and not place in the top five at all. Another change was seen when we ran the analysis to get the math and reading scores by grade level for each school. The 14 other schools had values for 9th-12th grade, whereas Thomas High School only showed values for 10th-12th grade and "NaN" for the 9th grade. The final change after removing the 9th grade scores could be seen when we ran the analysis for overall passing percentage by school size and school type. Although these changes were small, down the the hundrethes place, removing the scores did cause a change. 
