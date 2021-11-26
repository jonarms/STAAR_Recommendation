# TEXAS_STAAR_MEETS_PREDICTIONS

The State of Texas Asssessments of Academic Readiness is a series of examinations given to Texas Students from grade 3 to graduation to guage student mastery of state education standards. Working under the assumption that every school district is continuously working to provide their educators with the most relivant and up-to-date professional development, my goal was to determine which other actions a district might take to improve overall STAAR performance in all subjects. 

### Datasets present

[district_summary.csv](https://github.com/jonarms/Capstone2/blob/e2e5252b7fb1a27194cbc3305383be1d5b3677c2/district_summary.csv) contains the 2017-18 district snapshot data for all school districts

[wrangled_snapshot](https://github.com/jonarms/Capstone2/blob/e2e5252b7fb1a27194cbc3305383be1d5b3677c2/wrangled_snapshot.csv) contains the dataset after it's been cleaned. 

[unscaledsnap](https://github.com/jonarms/Capstone2/blob/654187a824fc4272d220604c2b83aaa0e4ecb050/unscaledsnap.csv) contains the significant features of the dataset used for preprossing and training.

[starmeets2019](https://github.com/jonarms/Capstone2/blob/654187a824fc4272d220604c2b83aaa0e4ecb050/staar_meets_2019.csv) contains data collected from the TEA snapshot [here](https://tea.texas.gov/texas-schools/accountability/academic-accountability/performance-reporting/snapshot-school-district-profiles). The districts searched for were Bay City ISD and Cleburne ISD. 

[starmeets2020](https://github.com/jonarms/Capstone2/blob/654187a824fc4272d220604c2b83aaa0e4ecb050/staar_meets_2020.csv) is the same as above except collected before 2020 staar results were released. This dataset also included alterations to the data including optimizing the actionable features as well as making more reasonable changes. 

### Notebooks

In [STAAR_Data_Wrangling](https://github.com/jonarms/Capstone2/blob/361c9f6b2c28faba14df24dcd261bb847ec40aa0/STAAR_Data_Wrangling.ipynb) the columns are renamed to a more readable format, basic exploration is done to expose and correct and/or remove erroneous information, and redundant as well as categorical features are removed.

In [Capstone 2 EDA](https://github.com/jonarms/Capstone2/blob/361c9f6b2c28faba14df24dcd261bb847ec40aa0/Capstone%202%20EDA.ipynb) the data is explored to find any patterns to explain or predict STAAR Meets all subjects (known as "target"). 

In [STAAR_Preprossessing](https://github.com/jonarms/Capstone2/blob/20e7ffa9883684f51a610e11b770bda28a1d1946/STAAR_Preprocessing.ipynb) two categorical variables are reintroduced into the dataset and dummy variables are created. 

In [STAAR_Model_Selection](https://github.com/jonarms/Capstone2/blob/e2ef2ef5d0894eca758a66f68b54029b04f6d380/STAAR_Modeling_Selection.ipynb) the data is split into training and testing sets, scaled, and modeled using various algorithms. The model is then further assessed using 2019 data, and finally used to forcast 2020 STAAR scores with the alterations mentioned above. 

This method was able to predict an improvement of more than 10% for both of the districts measured by recommending moderate improvements to:

-Attendance Rate

-Staff % Teachers

-Teacher % With 5 or Fewer Years of Experience

-Teacher Turnover Rate

-Racial Dif Stu/Tea
