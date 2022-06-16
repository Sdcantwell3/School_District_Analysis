# School_District_Analysis
## Overview of School District Analysis
### Background
  This analysis is looking into evidence of academic dishonesty associated with the math and reading scores for the 9th grade class at Thomas High School.  
### Purpose
  We will be sifting through all of the reading and math score data that was supplied to us for the entire school district with the goal of identifying and removing data that is believed to be inaccurate (compromised). Once the inaccuracy's are removed we will be doing a formal analysis comparing the reading and math scores of all of the schools in the district.
## Results
  Original Analysis:
![Original Aanalysis Summary](https://user-images.githubusercontent.com/104606589/173966038-b861630d-eaec-4e9c-bc9f-1e81e3ae44e7.png)

Upon being informed that the scores from the 9th grade class at Thomas High School were untrustworthy we decided to replace all values with null data.  After doing so we recalcuated all of the math, reading, and overall passing percentages for the school district. You will notice that total number of students stayed the same because that perameter was calculated based off student ID and was not replaced by a null value.

  Analysis W/O Thomas Highs School Math and Reading Scores:
  ![without 9th grade ths scores](https://user-images.githubusercontent.com/104606589/173967459-33a5f328-3c8e-408a-ac2d-c468ae7d9563.png)

The overall values did not change significantly.  The data set is comprised of a little less then 40,000 students and the removal of the Thomas High School scores accounted for less then 500 data points. 

## Thomas High School Summary Comparison

Thomas High School was in the top 5 of all school districts when the original analysis was performed. 

Original Analysis:
![top 5 Schools](https://user-images.githubusercontent.com/104606589/173970695-8b47fc51-b0c2-4153-b0ed-94edef3c98bf.png)

As you can see above the overall passing percentage for the school was almost 91%.

Analysis W/O 9th Grade scores:
![THS Overall withouth 9th](https://user-images.githubusercontent.com/104606589/173970979-4a9c30de-9f03-483c-bec1-fd0d4c510367.png)


Removing the suspicious scores from the 9th grade dropped the overall passin to 65%.  This is a significant decrease and would lead us to believe that the scores where infact fraudulent.  This drop in overall passing puts Thomas High School in the middle of the pack when looking at all schools in the district.

# Looking at other metrics after removing the 9th grade data.
## Adjusted Averages Score by School by Grade

Below you can see the data for Thomas High School has been removed and replaced with "NaN".  The original passing percentages were 83.6% (math) and 83.7% (reading).

###          Adjusted Math ------------------------------------ Adjusted Reading
![Math scores by school by grade](https://user-images.githubusercontent.com/104606589/173972852-b79e7d10-0859-474e-87eb-5aa231231322.png)        ![Reading scores by school by grade](https://user-images.githubusercontent.com/104606589/173972865-7d3661d9-ee93-47f1-b212-c1d2a23bb2d9.png)

## Scores by School Spending

Thomas High School's overall spending fell into the $630-644 total spending bucket.  The removal of the data did not change this category significantly.  It is likely that there is a large amount of schools in this range and the dropping the less then 500 scores would not have a big impact on the overall trend.

### Original Analysis:
![Scores by School spend original](https://user-images.githubusercontent.com/104606589/173974438-50bf5d64-168c-4933-b667-0a09d2a7520d.png)


### Adjusted Analysis:
![Scores by School spend updated](https://user-images.githubusercontent.com/104606589/173973764-8100b4b8-44d0-4591-be2e-d846a2d6aa01.png)

## Scores by School Size

When considering the change from removing the suspicious data while looking at school size we can again see that the change was negligable.  

### Original Analysis:
![Scores by School Size original](https://user-images.githubusercontent.com/104606589/173974690-8bc91cc3-d38a-442a-b29b-e10b842d9302.png)

### Adjusted Analysis:
![Scores by School Size updated](https://user-images.githubusercontent.com/104606589/173974734-8ee49d7e-91ec-44a1-9654-ac5179b54d3b.png)

This again would point to the small amount of change in data overall by just removing the 9th grade scores.

## Scores by School type

The change in data does not seem to have a large impact on the overall trend.  Thomas High School is a charter school and you can see below tha there was very little change due to the removal of the data for the math and reading scores for Thomas High's 9th grade class.

### Original Analysis:
![School Type original](https://user-images.githubusercontent.com/104606589/173975430-0798d351-d745-4c85-b8e4-c13b51766ecd.png)

### Adjusted Analysis:
![School Type new](https://user-images.githubusercontent.com/104606589/173975480-0bfc1d0d-1171-41a0-8f03-f67ea94f858a.png)

# Summary/Take Aways

1. The biggest impact was felt by Thomas High School Directly. We saw a dramatic drop in overall passing from 91% to 65%.
2. This dropped the overall ranking of Thomas High School Among Charter and Non-Charter schools.
3. The larger trends for the district where mostly unaffected by the removal of the data from Thomas High School.
4. When looking at the data for all of the 9th grade school it will be important to keep in mind that all data for Thomas High School will appear as "NaN".

The impact of our changes will not be seen when looking at the aggregate as a whole, but will be noticeable if you looking into that disaggregated data.











