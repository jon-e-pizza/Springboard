# Locating a Fast Food Restaurant

In order to assist a potential franchisee in optimally locating for a retun on investment, we apply statistical analysis and machine learning methods to distinguish successful areas from non successful areas. The investigation is limited to the city of Philadelphia due to financial constraints in procuring current information on existing establishments and patronage but the methods followed in this project can be generalized to an increased amount of locations and leaves room for expansion of investigation.

We use a subset of the census variables provided by [Safegraph](https://www.safegraph.com/open-census-data), [crime statistics provided by the city of Philadelphia](http://metadata.phila.gov/#home/datasetdetails/5543868920583086178c4f8e/representationdetails/570e7621c03327dc14f4b68d/), and walk and transit scores provided by [Walk Score](https://www.walkscore.com) as predictor variables to model output variables of fast food consumer count and patronage obtained from [Safegraph's data shop](https://shop.safegraph.com). As the bulk of our input variables relate to Census Block Groups as input areas, we map all our information to CBGs utilizing the [census geocoding service](https://geocoding.geo.census.gov/geocoder) and [Google Maps API](https://maps.googleapis.com).

Within this directory are the files:
- **[Final Report](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/Locating_Fast_Food-Final_Report.pdf)** detailing our initial proposal for this investigation and each step in the process of producing models for successful
- **[Milestone Report](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/Locating_Fast_Food-Final_Report.pdf)** an earlier revision of our final report produced half way through this project
- **[Final Presentation](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/Locating-Fast-Food-for-Success-Presentation.pdf)** a presentation to review the most essential details of our findings

And directories:
* **[data_wrangling](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneFastFoodEstablishments/data_wrangling)** containing data wrangling steps, but not our processed CSV data due to size and proprietary nature
    * **[Python Notebook](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/data_wrangling/Data_Wrangling.ipynb)** Detailing steps and code to amalgamate various measures and output variables into one CSV
    * **[Report Detailing the Process](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/data_wrangling/DataWranglingForFastFoodDemand.pdf)**
    * **[Output Processed CSV](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/data_wrangling/location_data_wrangled.csv)** indexed by CBG

* **[eda](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneFastFoodEstablishments/eda)** containing initial exploratory data analysis steps
    * **[Python Notebook](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/eda/EDA.ipynb)** Detailing steps and codes analysing statistics of successful CBGs and containing summary visuals
    * related input data consumed by the notebook

* **[learning](https://github.com/jon-e-pizza/Springboard/tree/master/CapstoneFastFoodEstablishments/learning)** containing machine learning modeling processes used in analysis
    * **[Python Notebook](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/learning/machine-learning.ipynb)** Detailing code for machine learning models and steps taken to arrive at optimal models
    * **[Report Detailing the Process](https://github.com/jon-e-pizza/Springboard/blob/master/CapstoneFastFoodEstablishments/learning/MachineLearning-process.pdf)**
    * related input data consumed by the notebook
