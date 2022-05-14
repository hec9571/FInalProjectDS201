# GPA and Common Behaviors of College Students

### Fahad Habona, Sam Wertz, Hector Morales, Peiqian Chen, Max Ippolito
## Business Understanding

   College students have been notoriously known for doing activities outside of their classes and being a diverse community with combatting interests.  High school students have increasingly become more likely to go to college and with five thousand three hundred colleges in the states currently we see how popular College is today.  This is a time in a student’s life where they go out and try new things which helps them have a taste of adulthood before entering the working world.  During college, men and women are at their physical peak and it is a time period where we see much growth in individuals.  But with everything there are elements in college that can negatively or positively affect one’s physical or mental health.  There are health issues that could arise from heavy drinking, drug use and other factors such as anxiety.  However, independence could lead to better sleep patterns, making new friends and healthier life choices such as more exercise.  In addition, decisions on how long you prepare for exams or even how many meals you have a day could affect your performance in school.  All these newfound responsibilities can hinder or enhance your performance so it will be interesting how these variables interact.

  The results of one study at Purdue University showed that the mean GPA for student organization members and officers was significantly higher than the mean GPA for those not in these organizations (Relationship between Undergraduate Student Activity and Academic Performance Amy L. Hawkins).  This shows that involvement in campus activities could lead to more engagement in school which in turn helps them attain better grades.  Also in the same study they found a negative correlation between fraternity involvement and GPA but a positive correlation between sorority involvement and GPA.  Greek life has been known to help students find a group of friends to hang out with but can increase one’s activities outside the classroom.  Drugs, alcohol and behaviors such as skipping class could arise from this which could substantially affect our grades.  

  But with this there is a decent amount of people that argue that this level of independence at college is needed for growth and is actually ultimately a benefit to your experience.  Making your own decisions will ultimately help you more in the long run and help your academic performance.  Also if people don’t want to be so involved around campus that could translate them to being much more focused on their schoolwork.  This could lead them to attaining better grades even though they are not taking advantage of all that college has to offer.  So ultimately these behaviors could not have a dominant effect on us, everyone is different and being at college could still not change people that much.  

  With this in mind we decided to analyze the following question: **How do common behaviors of college students affect GPA?** We want to see how aspects of Greek life involvement, hours of studying, alcohol use and other factors affect our academic performance at college.

  This study focuses on college students with a multitude of different attributes gathered.  This will hopefully help us understand how life in college affects our performance in the classroom.  Ultimately, we are college students and we want to see how our activities and thoughts in college have a negative or positive effect on our performance.  

  
## Data Organization

This dataset contains data from a survey of students at Penn State University enrolled in in Stat 100, an intro-level statistics course. The data was provided by Trent Gaugler, a current Professor of Mathematics at Lafayette College and former Professor of Statistics at Penn State. The survey was given in 2007 and was administered to 1,485 students enrolled in the Stat 100 course. The survey contains 54 different questions ranging from basic demographics (gender, what type of hometown you grew up in) to academics (your GPA, how often you study and skip class) to social life, political preferences, religious convictions, drug and alcohol usage and more. We selected eight predictor variables, which are outlined in the next section, that we thought might best predict a given student's GPA.

The other variables include factors for each student which include Gender, Hometown, Living Area, Greek Life involvement, Hours of Job Work, Maridal Status of Parents, GPA, Sitting Area in Class, How Often you Skip Class per Week, Hours Studied, Have They Cheated, Organizations Involved In, How Important Religion is to Them, Their Religion, How Many Time they Pray, Abortion Views, Euthanasia Views, Same Sex Marriage Views, Weight, Height, Idle Weight, Idle Height, How They View their Weight, What They are Actively Trying to do about their Weight, Self Attraction, Friend Prefernece, Most Important Feature in a Friend, Amount of People Kissed, Amount of Long-Term Relationships, Hours of Studying per Week Age They Want to get Married, Hours Exercised, Minutes Exercise, Why They Exercise, When They Want their First Child, How Many Children They Want, How Many Siblings They Have, Hours and Minutes of Exercise per Week, If They Smoke Cigarettes, If They Have a Fake ID, How Many Days They Drink Alcohol per Month, Number of Days per Month They Binge Drink Alcohol, Hours of Sleep per Week, Smoking Marajuana, Drinks Usually When Drinking, Virginity, Whether They have Sex with Someone Not in a Relationship and How Many Sex Partners They Have Had.

After condensing the data and identifying some particular trends we looked more closely at these 8 factors listed below:

| Attribute   | Data Type   | Description   | Nullable   |
|-------------|-------------|---------------|------------|
|GPA          |Ratio     |Grade Point Average on a 0 to 4.0 scale| No |
|Days Drinking Alcohol|Ratio|Days Drinking Alcohol per Month| No |
|Binge Drinking|Ratio|Days Spent Binge Drinking|Yes|
|Greek Life|Nominal|Involvement in Greek Life on Campus (Fraternities or Sororities)| No|
|Hours Studied|Ratio|Hours Spent Studying per Week|No|
|Hours Excercised|Ratio|Hours of Excercise per Week|No|
|Skip Class|Ratio|Skipped Classes in a given semester|No|
|Organizations|Ratio|Number of Organizations Involved In (Clubs, Sports Teams, Arts, Greek Life, Religious Associations)|Yes|
|Hours of Sleep|Ratio|Hourse of Sleep Per Night (On Average)|No|

## Modeling and Evaluating

### Exploratory Data Analysis

To begin looking at the 5 number summary generated by our data below we can see that our data ranges from 1.670 to 4.000 with 28 values that are catergorised as NA or Not Accessible. Looking at our mean and median they are almost the same with a mere 0.0710 difference indicating a more or less evenly distribution.
   
   |  Min   |  1st Q |  Med   |  Mean  |  3rd Q |  Max   |  NA |  
   |--------|--------|--------|--------|--------|--------|-----|
   |1.670   |2.930   |3.300   |3.229   |3.600   |4.000   |28   |
   
We next ran statistical analyses for on our chosen predictors alongside GPA. For each quantiative variable, we first visualized the distribution of the data with a histogram to check for normality then performed a correlation test to check for predictive power on GPA. All but one of the distributions analyzed had right-skewed distributions and did not have normality. This allowed for us to understand our data and their relationship with variables as seen below in the histogram and scatterplot showing the distribution of GPA.
  
  ![Unknown](https://user-images.githubusercontent.com/72221286/168399761-72d5128d-7853-4b2a-add8-d13f34667395.png)
  
  ![Unknown-2](https://user-images.githubusercontent.com/72221286/168402095-b4b78e78-e293-48ac-8d25-097a79087462.png)
  
### Machiene Learning
Our group decided to use supervised machine learning via linear regression with a quantitative target variable to confirm the findings. After selecting our 7 quantitative predictor variables we ran linear regression of GPA as fucntion of these variables. We then constructed a neural network to futher explore any further relationships.



![Unknown-3](https://user-images.githubusercontent.com/72221286/168402339-94edcbb6-0cb8-4513-a52b-f5ba55e4c33d.png)

## Deployment
The goal of our analysis was to analyze whether certain college student's behaviors had an effect on their GPA's. We explored data on different types of college behaviors and as a result made the following conclusions.

One main observation we were able to see was that days spent drinking and binge drinking had almost no effect on the GPA each student got. We found that hours spent studying and exercised, skipping class, and organizations did have an effect on the GPA that college students received. Overall, if you had different types of involvement throughout college, they would have an impact on your GPA. We observed that for a positive impact on your GPA, they were correlated to the organizations and hours studied and exercised. Negative impacts were correlated with skipping class.

Based on our insights, we can make the following recommendations to future college students. If students currently in college or seeking to attend college would like to achieve a positive GPA, they are better off getting involved with organizations and spending a good amount of hours studying and exercising. If you would rather, for some reason, like to have a negative GPA, you are better off skipping class. From the variables we observed, these were the ones that had an impact on a student's GPA. If a student would like to drink, it appears that it would make no difference to what their final GPA may be.

Moving forward, we would like to further research the correlation between GPA and typical college behavior at different sized institutions. We hypothesize that, similar to the one in this report, there will be an effect on GPA due to college behavior regardless of the size of the institution.

## Youtube
[Click here for our Presentation of our Findings](https://www.youtube.com/watch?v=MfA6G4Z8uVg)
[Click here for our Tutorial video](https://www.youtube.com/watch?v=cl94XWA98Js)


## Inquiries
For any inquiries on this project, please contact Fahad Habona (habonaf@lafayette.edu), Max Ippolito (ippolimh@lafayette.edu, Hector Morales (morales@lafayette.edu), Peiqian Chen (chenp@lafayette.edu), or Samuel Wertz (wertzsr@lafayette.edu)

## Acknowledgements and Link to Project

Hawkins, Amy L., "Relationship between Undergraduate Student Activity and Academic Performance" (2010). College of Technology
           Directed Projects. Paper 13. http://docs.lib.purdue.edu/techdirproj/13


https://colab.research.google.com/drive/1UVctVQ35vJgpS_4fW2aAu_rTraD7uv--#scrollTo=pgWl89D-RXsb

