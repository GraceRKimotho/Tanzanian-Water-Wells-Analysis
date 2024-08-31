# Tanzania-Water-Wells-Analysis
![Screenshot 2024-08-31 083941](https://github.com/user-attachments/assets/f50da159-c96b-4f4e-a059-6028eb615a51)


## 1. Overview
Tanzania, as a developing country, struggles with providing clean water to its population of over 65.5M (as of 2022). There are many water points already established in the country, but some are in need of repair while others have failed altogether.Only 61% of households in Tanzania currently have access to a basic water-supply. Tanzania has had to contend with death and disease as immediate consequences of this, with the burden falling heaviest on women, children, and the poor and vulnerable. The estimated 31,000 deaths each year due to inadequate WASH services are over 10% of preventable deaths in Tanzania, and cost the economy more than $2.4 billion each year in excess medical costs and lost productivity.

More often than not, the clean water a developing community desperately needs is right underneath them and a relatively small investment to get to it can make such a dramatic difference in so many lives. 

 #### Business Problem
 GreenPace is an NGO which aims to alleviate the water crisis in Tanzania by establishing more water wells 
 in the country. They aim to partner with the best organizations and choose the most suitable 
 geographical locations to ensure the best outcome. The model we build is supposed to help make 
 predictions that will inform the NGO's final decisions.


 #### Objectives
- To build a classifier that predicts the condition of water well as either functional or non-funtional.
- To determine the regions with more chances of having functional water points for future planning
- To determine the funders funding a high number of functional water points.

 ## Data Understanding
 The dataset used in this analysis is the Tanzanian Water Well dataset, hosted by driven data. 
 It is subdivided further into three datasets; Training_set_values, Training_set_labels and 
 Test_set_Values.

 From conducting EDA we found the data contained in the dataset contained many NaN and 0 
 values. Some columns also contained similar values(duplicates) and missing values. Data 
 cleaning was thereby paramount to address these issues, before the modeling process.

 We also observed the relationships of the different status groups vs features such as basins, funders, installers, gps height among others. Below are some visualizations that show this:

**status group vs basins**

 ![Screenshot 2024-08-31 095726](https://github.com/user-attachments/assets/b9d49be7-5499-4061-b970-0c0c1d015d6f)

 **status group vs installer**

![Screenshot 2024-08-31 085857](https://github.com/user-attachments/assets/38ac0a92-0484-4c41-aaa9-e41fa6ceaf5e)

**status group vs funder**

![Screenshot 2024-08-31 095322](https://github.com/user-attachments/assets/55529b32-a72e-4973-84c3-4049ccc9302f)

 


 ## 2. Modelling
The EDA and Data Cleaning processes revealed our data contained a mix of both numerical and categorical values. This factored into deciding which models to explore before determining the best one. We therefore decided to use a logistic regression model, a confusion matrix and a decision tree classifier.

#### Model Evaluation
Different metrics were used in evaluating the chosen models: Accuracy Score fr score, precision and recall are the ones applied. We  established that the best mode to use was the decision Tree Classifier because it had a higher accuracy than the Logistic Regression Model.

## 3. Conclusion/Findings
- There are typically more functional wells in locations with higher population densities.
- Certain locations are more likely to have access to clean water, particularly if they are close to the appropriate basins.
- Despite being one of the most populous cities, Dar es Salaam has 35% non-functional good water quality points.
- The majority of government-funded wells are inoperable.
- The majority of the water points established by the district council and central government are not working.
- The Logistic Regression model had an accuracy  score of 62% while the Decision Tree Classifier model yielded an accuracy score of 64%.

## 4. Recommendations
- The project excecuters should carefully consider the geographical locations of their wells since this is directly linked to the functionality/quantity of water that a well can yield.
- We recommend DWE as a potential partner(if needed) since the analysis has shown that most of the wells they have funded/installed are functional.
- The gps height should also be considered in order to determine the type of pumps to be used at the wells.
- Proximity to basins like Rufiji, Lake Victoria and Pangani is recommended for higher productivity.
  


  
 
  
