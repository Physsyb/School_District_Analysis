# School_District_Analysis
## 1) Overview of the Project
> Explain the purpose of this analysis.

The purpose of this project is to analyse data on students funding and standerdized test scores. Also, to aggregate data and show case school performance.This will assist the board and superintendent in making decisions regarding the school budgeting priorities. While working on the analysis, we are to be aware of the Family Educational Rights and Privacy Act (FERPA), 1974 which protects the privacy of student education records, and applies to all schools that receives funds from the US department of education.
Here are the lists of delivaerabkes for the analysis:
* A high-level snapshot of the district's key metrics, presented in a table format
* An overview of the key metrics for each school, presented in a table format
* Tables presenting each of the following metrics:
  * Top 5 and bottom 5 performing schools, based on the overall passing rate
  * The average math score received by students in each grade level at each school
  * The average reading score received by students in each grade level at each school
  * School performance based on the budget per student
  * School performance based on the school size 
  * School performance based on the type of school.
  These tasks will be completed using `Anaconda` `Jupyter Notebook` `Python` and `Pandas`
 ## Resources
  * Data Source: `students_complete.csv` and `school_complete.csv`
  * Software: Python 3.7.6, Anaconda 4.9.2, Jupyter Notebook 6.1.4
 ### Challenge Background
 The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades     for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help. She has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.
 
 Deliverables of this challenge are:
 * Replace ninth-grade reading and math scores
 * Repeat the svhool district analysis
 * Report for the school district analysis
 ## 2) Results
 > Using bulleted lists and images of DataFrames as support, address the following questions.
 ### a) How is the district summary affected?
 After a clean up was done, there were some slight changes in the scores.
 #### Before Data Cleanup
 * Average Math Score = 79.0
 * Average Reading Score = 81.9
 * % Passing Math = 75
 * % Passing Reading = 86
 * % Overall Passing = 65
 
![1](https://user-images.githubusercontent.com/76136277/105620863-385a7d80-5dcf-11eb-95e8-9e78ccb7c3d0.PNG)
#### After  Data Cleanup
 *  Average Math Score = 78.9
 * Average Reading Score = 81.9
 * % Passing Math = 74.8
 * % Passing Reading = 85.7
 * % Overall Passing = 64.9
 
![2](https://user-images.githubusercontent.com/76136277/105620869-532cf200-5dcf-11eb-916a-9fac08016c6f.PNG)
### b) The school summary DataFrame
Before the cleanup, the overall percentage for Thomas high school was 91%, but after the cleanup, it dropped to 65%.

![3](https://user-images.githubusercontent.com/76136277/105621423-372c4f00-5dd5-11eb-965a-780654577142.PNG)
![4](https://user-images.githubusercontent.com/76136277/105621023-237ee980-5dd1-11eb-9962-d2e716dee13b.PNG)

### c) How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
   Replacing the ninth grade score to NaN automatically drops the ranking of the school.
 ### d) How does replacing the ninth-grade scores affect the following
  * Math and reading scores by grade
     * Replacing Thomas High School 9th grade scores equals to "0"  
     * 491 9th grade students failed math and reading  
![9th](https://user-images.githubusercontent.com/76136277/105621691-3ea12780-5dd8-11eb-9c7e-90c67b3b19f6.PNG)
  * Scores by school spending
     * Thomas High School is in the spending bucket "$630-644" . 
![12](https://user-images.githubusercontent.com/76136277/105623370-3ef4ef00-5de7-11eb-9bbd-a3dd27c0a8b8.PNG)
![8](https://user-images.githubusercontent.com/76136277/105622028-9beaa800-5ddb-11eb-8a67-af84a2712c90.PNG) 
![7](https://user-images.githubusercontent.com/76136277/105622037-a86f0080-5ddb-11eb-8f2d-d772c613496e.PNG)


  * Scores by school size
      * In this category, Thomas High Schools belongs to the medium school size. In the screenshots below, there are slight changes in the figures as well (before and after cleanup)
      
![1](https://user-images.githubusercontent.com/76136277/105623230-351ebc00-5de6-11eb-9fe6-524e467faee9.PNG)
![11](https://user-images.githubusercontent.com/76136277/105623233-3819ac80-5de6-11eb-9247-880ddcfedef3.PNG)

      * Before cleanup, the school had 1635 students but dropped to 1174 students.
 ![0](https://user-images.githubusercontent.com/76136277/105622544-6f855a80-5de0-11eb-8012-e6fefcd71114.PNG)
![9th](https://user-images.githubusercontent.com/76136277/105622564-7f9d3a00-5de0-11eb-82e9-428cafb5e329.PNG)
![000](https://user-images.githubusercontent.com/76136277/105622580-99d71800-5de0-11eb-95f9-7bdef865e9a7.PNG)

  
  * Scores by school type
    * Thomas High School is in the Charter category and there are slight changes in the percentages, average math and reading scores as seen in the screenshots below (before and after data clean up)
![9](https://user-images.githubusercontent.com/76136277/105623138-65198f80-5de5-11eb-894e-1d882850050f.PNG)
![99](https://user-images.githubusercontent.com/76136277/105623139-677be980-5de5-11eb-978b-bdc2650b3764.PNG)

## 3) Summary
> Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

* Changes in the average math and reading scores 
* Changes in the percentage passing and reading scores
* Changes in the overall percentage of the school, from 91% to 65%
* Changes in the student count from 1635 to 1174 students.
