# capstone-project-IBM
Problem Statement
From the start of the 21st century terrorism has been an influencing factor on the
economy, tourism and general life aspects of citizens in Middle Eastern and
North African Countries (MENA).
The project aims to present a unique solution for the terrorist group prediction.
Terrorist group predicting consists is identifying the terrorist group responsible
for a certain terrorist attack using a set of common features between each terrorist
attack .


STEPS FOLLOWED 

1. Theoretical Part 
In  report and presentation, a tabular comparison between
binary classification and multi-class classification from these points of view:
1. Definition
2. Types
3. Examples
2. Download and understand the datasets 
a. Global Terroism Database (GTD) 2017
It includes 135 attributes including year, month, type of the attack, weapon type,
specific location of the event (longitude and latitude) and most important of them
all is terrorist group name which is used as the classifier’s label .
Link: https://www.kaggle.com/START- UMD/gtd/home.
b. World Happiness Report (WHR)
World Happiness Report contains 10 attributes including happiness score, freedom
score and GDP per capita (Economy)..
3 versions of World Happiness Report at years 2015, 2016 and 2017 are required
to be used in this assignment to analyze the change and stability against the time
factor in the 3 most recent years to the time of the study.
Link : https://www.kaggle.com/unsdsn/world-happiness
3. Features Selection 
● choose the features you see suitable for training the classifiers
from the 135 features of the GTD and the 10 Features of the World Happiness
Report.
● It is preferable to choose a set a features using intuition and then use trial and
testing to choose the best subset.
● Suggested features from GTD:
○ Weapon Type
○ Attack Type
○ Target
○ City
● Suggested features from WHR:
○ Happiness Score
○ Freedom Score
● group_name from GTD is the class label.
4. Data Preprocessing
a. Select tuples of countries in the MENA area only.
b. GTD contains data from 1970 to 2017, you are required to drop all tuples before
year 2000. (Not including year 2000)
c. Missing Values
You have 2 ways to handle tuples with missing values:
● Mean / Mode
● Drop tuple
d. Encode categorical attributes like city, country ... etc. and the class label
(group_name) to numerical value in order to train the classifiers.
e. Thresholding
Having about 600 terrorist group name (class labels), with some groups with less
than 10 attacks which may cause misleading results. You are required to reduce the
number of class labels to the 5 groups with max number of attacks.
5. Training and Testing 
a. use the tuples of years from [2000. 2016] as training set
b. Tuples of year 2017 will be used as testing set.
c. We have 2 approaches in this assignment
i. Train and test using features of GTD only.
ii.Train and test using features of GTD and WHR combined.
d. F-Measure should be used for performance evaluation.
6. Classifiers 
● You are required to use these classifiers:
i. kNN
ii. Decision Trees
iii. Naive Bayes
iv. SVM
7. Results and Visualizations 
a. Please use tables, graphs and plots whenever possible to present your results.
b. Comment on the results of the 2 testing sets briefly.
