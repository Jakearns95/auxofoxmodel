# Auxofox Model

AuxoFox’s risk analysis platform for major retailers uses geospatial, sales and inventory data to analyze and predict losses due to theft at retail stores. By using AuxoFox to create individual risk models for each retail location, Loss Prevention (LP)  professionals can better understand the external risk factors driving theft and how to address them. AuxoFox is currently building its minimum viable product in partnership with a major national retailer and intends to begin beta testing in Q1 of 2019

Our Minimal Viable Product (MVP) will be a model that predicts shrinkage on an annual basis.  To build the model successfully, the following needs to be accomplished:

1.	Import and clean all data sources
  a.	Unzip and change file type for all internal data provided from partner
  b.	Consolidate and clean internal data sources (index: Store number)
  c.	Clean and consolidate UCR data sources (index: Location and zipcode)
  d.	Clean and consolidate Census level data (index: Zipcode and census code)

2.	Build an initial OLS regression model based on historical and employee turnover data

3.	Determine value added predictability police call logs add to model

  a.	Add APIs for Chicago and MKE to model and check predictability
  b.	Scrape police call logs for each store’s location of operation.  This will need to be built to automatically scrape the       data every time the data set is updated (minute, hour, day, etc). 

4.	Continue to add attributes

Goal:  Predict shrinkage within +/- 5 basis points on a yearly basis

More forward looking, we are looking to incorporate all data sets to predict shrinkage on a yearly basis and pull out attributes that lead to increased shrinkage on a monthly basis.  This monthly model will be based on geospatial analysis where a map and prediction will be provided for each unique store location.

