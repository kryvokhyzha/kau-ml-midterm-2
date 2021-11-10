# pump-it-up-challenge-solution _(kau-ml-midterm-2)_
**Author:** Roman Kryvokhyzha<br>
**Dataset:** Pump It Up Challenge: Driven Data [[kaggle](https://www.kaggle.com/sumeetsawant/pump-it-up-challenge-driven-data) | [drivendata](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/25/)]

## Challenge Summary
**Can you predict which water pumps are faulty?**<br>
Using data from Taarifa and the Tanzanian Ministry of Water, can you predict which pumps are functional, which need some repairs, and which don't work at all? This is an intermediate-level practice competition. Predict one of these three classes based on a number of variables about what kind of pump is operating, when it was installed, and how it is managed. A smart understanding of which waterpoints will fail can improve maintenance operations and ensure that clean, potable water is available to communities across Tanzania.

## Dataset description
Your goal is to predict the operating condition of a waterpoint for each record in the dataset. You are provided the following set of information about the waterpoints:

### Features
+ `amount_tsh` - Total static head (amount water available to waterpoint)
+ `date_recorded` - The date the row was entered
+ `funder` - Who funded the well
+ `gps_height` - Altitude of the well
+ `installer` - Organization that installed the well
+ `longitude` - GPS coordinate
+ `latitude` - GPS coordinate
+ `wpt_name` - Name of the waterpoint if there is one
+ `num_private` - **<span style="color: red">Description is empty</span>**
+ `basin` - Geographic water basin
+ `subvillage` - Geographic location
+ `region` - Geographic location
+ `region_code` - Geographic location (coded)
+ `district_code` - Geographic location (coded)
+ `lga` - Geographic location
+ `ward` - Geographic location
+ `population` - Population around the well
+ `public_meeting` - True/False
+ `recorded_by` - Group entering this row of data
+ `scheme_management` - Who operates the waterpoint
+ `scheme_name` - Who operates the waterpoint
+ `permit` - If the waterpoint is permitted
+ `construction_year` - Year the waterpoint was constructed
+ `extraction_type` - The kind of extraction the waterpoint uses
+ `extraction_type_group` - The kind of extraction the waterpoint uses
+ `extraction_type_class` - The kind of extraction the waterpoint uses
+ `management` - How the waterpoint is managed
+ `management_group` - How the waterpoint is managed
+ `payment` - What the water costs
+ `payment_type` - What the water costs
+ `water_quality` - The quality of the water
+ `quality_group` - The quality of the water
+ `quantity` - The quantity of water
+ `quantity_group` - The quantity of water
+ `source` - The source of the water
+ `source_type` - The source of the water
+ `source_class` - The source of the water
+ `waterpoint_type` - The kind of waterpoint
+ `waterpoint_type_group` - The kind of waterpoint

### Labels
The labels in this dataset are simple. There are three possible values:
+ `functional` - the waterpoint is operational and there are no repairs needed
+ `functional needs repair` - the waterpoint is operational, but needs repairs
+ `non functional` - the waterpoint is not operational

## Evaluation
The metric used for this competition is the classification rate, which calculates the percentage of rows where the predicted class __*y_hat*__ in the submission matches the actual class __*y*__ in the rest test set.
The maximum is 1 and the minimum is 0. THe goal is to maximize the classification rate.

## Problem
+ Choose any dataset for multiclass classification on [Kaggle](https://www.kaggle.com/) (go to "Datasets" section, choose "Filter" and enter "multiclass classification" into the "Tags" field). 
+ Perform classification with few methods. I expect you to use at least SVM (linear and rbf) and random forest.
+ Try getting the best result with each of the methods. I expect you to use at least GridSearch for hyperparameters tuning.
+ Try feature engineering. I expect you to use at least PCA for dimensionality reduction.
+ Calculate accuracy and confusion matrix for each of the methods.
+ Draw conclusions. Which method is the best? Why? If the dataset has any articles linked, compare your results with the state of the art.

## Grading criteria:
+ I expect a confident usage of sklearn methods.
+ I expect understanding of basics of models assessment.
+ I expect you to be able to learn PCA method on your own.
+ I expect the ability of succinct, cohesive, and coherent expression of your thoughts, i.e. clearly state (in a few sentences) what is the problem you are solving, what approaches do you propose, and what conclusions can be drawn regarding these approaches in the context of the problem.

