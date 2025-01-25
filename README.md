## SCMS Delivery History Dataset: Price Prediction
### Overview

This repository contains the SCMS Delivery History dataset aimed at predicting the price of deliveries based on historical data. The dataset includes various delivery-related features such as product details, shipment mode, dates, and financial details, which are used to predict the Unit Price of each delivery.

### Dataset Description
The SCMS Delivery History dataset consists of the following columns:

ID: Unique identifier for each delivery

Project Code: Code associated with the project

PQ #: Purchase Request number

PO / SO #: Purchase Order or Sales Order number

ASN/DN #: Advanced Shipment Notice or Delivery Note number

Country: Country of origin or delivery

Managed By: The team or individual managing the delivery

Fulfill Via: Method or channel used to fulfill the order

Vendor INCO Term: Vendor's International Commercial Terms (Incoterms)

Shipment Mode: Mode of shipment (e.g., air, sea, ground)

PQ First Sent to Client Date: Date when the Purchase Request was first sent to the client

PO Sent to Vendor Date: Date when the Purchase Order was sent to the vendor

Scheduled Delivery Date: Expected delivery date of the shipment

Delivered to Client Date: Actual delivery date to the client

Delivery Recorded Date: Date when the delivery was recorded

Product Group: Group classification of the product

Sub Classification: Subcategory of the product within the group

Vendor: The vendor supplying the product

Item Description: Description of the item being delivered

Molecule/Test Type: Type of molecule or test for pharmaceuticals or lab-related products

Brand: Brand name of the product

Dosage: Dosage information for pharmaceutical items

Dosage Form: Form of the dosage (e.g., tablet, liquid)

Unit of Measure (Per Pack): Measurement unit per pack (e.g., mg, ml)

Line Item Quantity: Quantity of items in the delivery line

Line Item Value: Total value of the line item

Pack Price: Price per pack of items delivered

Unit Price: Price per unit of the item

Manufacturing Site: Site where the product was manufactured

First Line Designation: Main classification or designation for the first line item

Weight (Kilograms): Weight of the delivery item(s) in kilograms

Freight Cost (USD): Freight cost for the delivery in USD

Line Item Insurance (USD): Insurance cost for the line item in USD

### Features
ID: Identifier for the delivery (not used in modeling)

Project Code, PQ #, PO / SO #, ASN/DN #: Identification numbers for various steps in the delivery process

Country: Geographical location of the delivery

Managed By: Entity responsible for the delivery

Fulfill Via,
Shipment Mode: Modes and methods used for fulfillment and shipment

Vendor INCO Term: Terms for the transaction between the vendor and customer

Dates (PQ First Sent to Client, PO Sent to Vendor, etc.): Date-related features for tracking delivery times

Product Group, Sub Classification: Categories defining the product group and subcategory

Vendor, Item Description, Molecule/Test Type, Brand, Dosage, Dosage Form: Product-related features for classification

Weight (Kilograms),
Freight Cost (USD), Line Item Insurance (USD): Quantitative features used to determine the cost and shipping characteristics
Line Item Quantity,

Line Item Value, Pack Price, 

Unit Price: Financial data associated with each item
### Data Preprocessing

To effectively use the dataset for predicting the unit price, the following preprocessing steps are recommended:

### Handle Missing Data:

Ensure there are no missing values in the dataset. If necessary, impute or drop missing values.
### Categorical Encoding:

Convert categorical variables such as "Country", "Vendor", and "Product Group" into numerical representations using one-hot encoding or label encoding.
### Feature Engineering: 

Extract useful information from date-related columns (e.g., calculate delivery delays, or duration between various dates).
### Model Training

You can train various regression models on this dataset, such as:

Linear Regression

Random Forest Regressor

Descion Tree Regressor

Evaluation Metrics

To evaluate the performance of the model, you can use the following metrics:

Mean Absolute Error (MAE)

Mean Squared Error (MSE)

R-squared (R²)
