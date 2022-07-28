# School District Analysis

## Analysis Overview
The purpose of this analysis was to examine the performances of district schools based on several parameters. Average grade percentages were calulated for all 15 schools, and these grade averages were examined based on school size, school type, funding, and were also broken down by grade level. After the initial analysis was performed, it was found that some of the results for the ninth graders from Thomas High School may have been the result of academic dishonesty. Adjustments were made to the coding and data frames created in the Jupyter Notebook to remove the scores of the Thomas High School freshman, and these new results were then incorporated into the existing data. The following points further examine the impact of these changes on the data.

## Results

### District Summary
The overall impact on the district level average scores and average passing percentages without the scores of the Thomas High School ninth graders is minimal. These students made up around 1.1% of the total student population that was analyzed. The changes in the district level numbers reflected this, with the changes being around a 1.1% difference across the board. The two figures below show - first the original district level results, and second - the results without the Thomas High ninth graders

![School_District_Analysis - original](https://user-images.githubusercontent.com/105682444/181395596-9f5db5ac-6ecd-4f97-a311-d982935f38c5.png)

![School_District_Analysis - without THS 9th](https://user-images.githubusercontent.com/105682444/181395614-f6bf85db-4251-4933-a46a-21a1338d6e59.png)

### School Summary
On a school level, having to remove the scores and passing percentages of the ninth graders at Thomas High School shows a much larger impact. The schools overall passing percentage dropped from 90.9% down to 65.1%. Of course, removing the scores of the ninth graders meant removing the scores of just over 25% of the students. The differences in the average scores and percentages, again, reflect a change of about that degree. The first figure shows the original analysis, with Thomas High School on the 13th line of the dataframe. The second figure shows this same dataframe without the scores of the ninth graders.

![School_Summary - original](https://user-images.githubusercontent.com/105682444/181396348-8568d57d-d6dd-4a90-af47-b71d4f3d7a2f.png)

![School_Summary - without THS 9th](https://user-images.githubusercontent.com/105682444/181396354-d9adc57f-00a0-41a4-a884-c3f353cf525f.png)

### Changes Relative to Other Schools
As can be seen in the figures above, removing the scores of the ninth graders of Thomas High School drastically affects the way the school's performance compares to others in the district. Instead of having passing percentages and scores on par with the smaller schools in the district it would typically be grouped with, the scores are closer to those of schools with twice the student population. This analysis also shows that the schools with a larger student body have, on average, lower performance.

### Changes Across Four Parameters

#### By Grade
Replacing the scores of the ninth graders as null doesn't affect the comparison across grade levels much. The other grades from Thomas High School are still some of the higher scores in the district.

![math_by_grade](https://user-images.githubusercontent.com/105682444/181397414-d8fd3aa2-f6cb-4bc8-a83f-b1f8a906ae3f.png)

![reading_by_grade](https://user-images.githubusercontent.com/105682444/181397431-35e17ed1-e3e8-4aa8-a1c7-e6482b698bc1.png)

#### By School Spending, Size, and Type
The largest change, as mentioned above in the section regarding the comparison to other schools, is in comparing Thomas High School to other school types. With the removal of the ninth grade sacores, Thomas High has by far the lowest overall passing percentage of all the charter schools, with the passing percent being closer to that of a larger district school. The other parameters are affected little to not at all by the change.

## Summary
Overall, needing to replace the ninth grade scores with NaN in the dataframe affected these four things most noticably and predicably :
  - the 1.1% change across the board for all scores and percentages at the district level. This was predictable considering that the Thomas High School ninth graders were about 1.1% of the entire student population
  - the drastic change in passing percentages and scores when Thomas High School is compared to the otehr charter schools
  - the fact that the lower percentages and scores put Thomas High School on a level closer to that of schools twice its size
  - showing that the tenth through twelfth grade scores were still even with the other charter schools, meaning that had there not been allegations of academic dishonesty amongst the ninth graders, the scores would have been at or above the norm for charter schools in the district 
