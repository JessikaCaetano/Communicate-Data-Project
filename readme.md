# Communicate Data Findings - Students Performance
## by Jessika Nunes Caetano

## Dataset

Our dataset was obtained from Kaggle and contains 1,000 records of students data, including the variables cited above, parent level of education, whether or not the student completed the preparation course to the tests and math, writing and reading scores for each student. We also added a new column, the mean score, which has the mean of the three subjects (math, writing and reading) scores. The file can be found in the url: https://www.kaggle.com/spscientist/students-performance-in-exams.


## Summary of Findings

> Univariate Exploration

    Gender: Our dataset students are separated in 51.8% females and 48.2% males. Considering that our dataset is composed by 1,000 students, that means 518 female students and 482 male students. We have a higher quantity of females, but still they are in similar numbers. Gender should not have impact in students performance, but we could look at the distribution of performance by gender later on.
    Lunch: Most of the students have regular lunch (645 of them), but there is a considerable amount of students (355 of them) who have free or reduced lunch. Later on I would like to investigate if that interferes in the students performance.
    Test Preparation Course Most of our students has not completed the test preparation course. Only 358 of them have done that. We can check if those students have a better score than the others.
    Race/Ethnicity: The biggest group of students is Group C, followed by Group D and Group B. Race or ethnicity should not be a factor of impact in students performance, but we can check if the groups presented have different social/economic situations by looking at the relation between this variable and others such as lunch and parental level of education.
    Parental Level of Education: The students parents most often have some college, an associate's degree or at least have completed or attended to high school. Most of them, otherwise, did not get to have a bachelor or master's degree. We should see if that interferes in their kids performance.
    Math Score: We can see that the math score distribution is skewed, with most students getting scores around 65-70. A few students got grades between 0 and 10. Later on we can try to understand which factors are characteristics of the students who got lower grades.
    Writing Score: The writing score distribution has two peaks: most students got grades between 70 and 75 (higher than the math score), but the second peak is located aroud 50-55.
    Reading Score: The reading score distribution is similar to the writing distribution, with the higher peak around 70-75. It appears that the students with good writing skills also have good reading skills.
    Mean Score: The mean score has a skewed distribution, as expected, and most students have a mean score around 65-70. We should see which factors interfere in this score later.


> Bivariate Exploration

    Female students have a higher median of mean scores.
    Female students have higher grades in writing and reading scores, but male students have better scores in math. This can also be cause by the hypothesis that students with good reading skills also have good writing skills.
    Mean score vs. lunch: We can clearly see that students that have a free (probably of lower quality than a paid for) or reduced lunch have lower mean scores. That probably happens because those students who eat better also feel physically better and have more physical and mental health in the moments they are studying.
    Mean score vs. test preparation course: Students that have completed the test preparation course have a better performance than others. The course can be considered then effective.
    Parental level of education: Except for the students with parents that only attended to high school, the higher the parental level of education, the higher the students performance, measured by the mean score. The students with parents eith higher lever of education probably have a better financial condiction, home structure and/or inspiration to pursue higher education. In case of students whose parents did not complete high school, we could suppose that a considerable quantity of them could want to have a different reality for themselves.
    Race/Ethnicity vs. Lunch: Looking at the pie chart we can see that the Group A has a higher percentage of students that eat free or reduced lunch, which could indicate that this group is somehow disavantaged by society. We could say the opposite about group E. The other groups seem to share the same place in society.
    Race/Ethnicity vs. Mean Score: Looking at the histograms we can see that group A has a distribution with lower scores than the other groups and that group B has probably better performance than some of the others, but the patterns aren't clear. Using the groupby function we can see that group A really has the lowest performance in mean score an that group E has the best, enforcing our hypothesis of disavantaged and privileged groups. We can also see that group D has better performance than group C, which has better performance than group B.

>Multivariate Exploration

    Females with standart lunch have a 10 points higher score than with free/reduced lunch, while to male students the difference is only 7.3 higher. The impact of lunch variation from free/reduced to standart lunch is stronger to females than to males.
    Relation between reading and writing scores appear to be linear, positive and strong;
    Students with the lowest scores in reading and writing appear to have also low grade in math, and the same happens to students with the highest grades. But in the middle of the grade interval this pattern does not seem to be always mantained.
        Female students have a higher quantity of grades concentraded in higher intervales of writing and reading scores. Their math grade seems to increse with the writing and reading grades, but their math grades seem to be lower than to male students.
        Male students do not have a performance as goos as females in terms of writing and reading scores, but their math scores appear to be much better than the female math scores. Also, the relation between math score and the other two scores in the case of male students, although is evident, do not appear to be as strong as to female students.


## Key Insights for Presentation

> I organized the presentation in orther to tell a story with the data in which each analysis led to another one, and together they formed a final robust analysis.

> Two of the visualizations/insights that I included in the presentation were:
- Variation of gender distribution per subject score (math, writing and reading)
  Female students have higher grades in writing and reading scores, but male students have better scores in math.
  I used violin plots for this. In the presentation, I changed the colors to the pallete 'Set2', and added chart title, x label and y label.
  

- Impact of lunch specifications variation in male and female gender
  The impact of lunch variation from free/reduced to standart lunch is stronger to females than to males.
  I used a heat map plot for this. In the presentation, I changed the colors to the pallete 'flare' because it had close colors to the pallete Set2 that I was using in other charts, and added chart title, x label and y label.

> Other trends were shown in the presentation. I used the pallete Set2 as a pattern and added titles and axis lables to the charts. I also took care of pie charts data labels, so they would appear in percentage.