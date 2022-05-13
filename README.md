# GPA and Common Behaviors of College Students

## Introduction

   College students have been notoriously known for doing activities outside of their classes and being a diverse community with combatting interests.  High school students have increasingly become more likely to go to college and with five thousand three hundred colleges in the states currently we see how popular College is today.  This is a time in a student’s life where they go out and try new things which helps them have a taste of adulthood before entering the working world.  During college, men and women are at their physical peak and it is an excellent time where we see much growth in individuals.  But with everything there are elements in college that can negatively or positively affect one’s physical or mental health.  There are health issues that could arise from heavy drinking, drug use and other factors such as anxiety.  However, independence could lead to better sleep patterns, making new friends and healthier life choices such as more exercise.  In addition, decisions on how long you prepare for exams or even how many meals you have a day could affect your performance in school.  All these newfound responsibilities can hinder or enhance your performance so it will be interesting how these variables interact.

  The results of one study at Purdue University showed that the mean GPA for student organization members and officers was significantly higher than the mean GPA for those not in these organizations (Relationship between Undergraduate Student Activity and Academic Performance Amy L. Hawkins).  This shows that involvement in campus activities could lead to more engagement in school which in turn helps them attain better grades.  Also in the same study they found a negative correlation between fraternity involvement and GPA but a positive correlation between sorority involvement and GPA.  Greek life has been known to help students find a group of friends to hang out with but can increase one’s activities outside the classroom.  Drugs, alcohol and behaviors such as skipping class could arise from this which could substantially affect our grades.  

  But with this there is a decent amount of people that argue that this level of independence at college is needed for growth and is actually ultimately a benefit to your experience.  Making your own decisions will ultimately help you more in the long run and help your academic performance.  Also if people don’t want to be so involved around campus that could translate them to being much more focused on their schoolwork.  This could lead them to attaining better grades even though they are not taking advantage of all that college has to offer.  So ultimately these behaviors could not have a dominant effect on us, everyone is different and being at college could still not change people that much.  

  With this in mind we decided to analyze the following question: **How do common behaviors of college students affect GPA?** We want to see how aspects of Greek life involvement, hours of studying, alcohol use and other factors affect our academic performance at college.

  This study focuses on college students with a multitude of different attributes gathered.  This will hopefully help us understand how life in college affects our performance in the classroom.  Ultimately, we are college students and we want to see how our activities and thoughts in college have a negative or positive effect on our performance.  

  
## Data Organization

For this project we used a dataset by Professor Trent Gaugler who surveyed 1,485 Penn State students.  This data was compiled in the year 2010 for students enrolled in a Stat 100 course.  The data includes a total of 54 factors for each student which include Gender, Hometown, Living Area, Greek Life involvement, Hours of Job Work, Maridal Status of Parents, GPA, Sitting Area in Class, How Often you Skip Class per Week, Hours Studied, Have They Cheated, Organizations Involved In, How Important Religion is to Them, Their Religion, How Many Time they Pray, Abortion Views, Euthanasia Views, Same Sex Marriage Views, Weight, Height, Idle Weight, Idle Height, How They View their Weight, What They are Actively Trying to do about their Weight, Self Attraction, Friend Prefernece, Most Important Feature in a Friend, Amount of People Kissed, Amount of Long-Term Relationships, Hours of Studying per Week Age They Want to get Married, Hours Exercised, Minutes Exercise, Why They Exercise, When They Want their First Child, How Many Children They Want, How Many Siblings They Have, Hours and Minutes of Exercise per Week, If They Smoke Cigarettes, If They Have a Fake ID, How Many Days They Drink Alcohol per Month, Number of Days per Month They Binge Drink Alcohol, Hours of Sleep per Week, Smoking Marajuana, Drinks Usually When Drinking, Virginity, Whether They have Sex with Someone Not in a Relationship and How Many Sex Partners They Have Had.  This is a mix of qualitative and quantitative data that will be condensed into the factors listed below.  

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

## Exploratory Data Analysis

### Distribution of Variables

   To begin looking at the 5 number summary generated by our data below we can see that our data ranges from 1.670 to 4.000 with 28 values that are catergorised as NA or Not Accessible. Looking at our mean and median they are almost the same with a mere 0.0710 difference indicating a more or less evenly distribution.
   
   |  Min   |  1st Q |  Med   |  Mean  |  3rd Q |  Max   |  NA |  
   |--------|--------|--------|--------|--------|--------|-----|
   |1.670   |2.930   |3.300   |3.229   |3.600   |4.000   |28   |
  
The plot below shows a distribution of gpa. From this we can see that the distribution is skewed to the left. In terms of observations students are more likely to have high GPA's with very earning 2.5 or below.
 
![Unknown](https://user-images.githubusercontent.com/72221286/168321501-b4861b63-f040-4b42-8eed-512d0c79c532.jpg)
<Why these plot?>
This plot shows the frequcny of the amount of hours studied. From this plot we can see that our data is skewed to the right meaning that majority of students study anything below 20 hours with highest frequency being observed 10 hours.

![Unknown](https://user-images.githubusercontent.com/72221286/168326459-defba0c0-bd68-4a99-b254-26ea716b89bb.jpg)

From this scatterplot it's evident that there is a relationship fewer days of alcohol and higher GPAs. Majority of the data is clustered from 0 to 5 with outliers at 25 and 35.

![Unknown](https://user-images.githubusercontent.com/72221286/168329466-f3ae862f-8335-4ab1-bf0f-e2c1ca922192.jpg)

