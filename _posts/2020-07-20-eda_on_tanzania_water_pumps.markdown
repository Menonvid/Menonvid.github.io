---
layout: post
title:      "EDA on Tanzania Water Pumps"
date:       2020-07-20 23:48:39 +0000
permalink:  eda_on_tanzania_water_pumps
---

The complete blog on Medium : https://medium.com/@menonvid/eda-on-tanzania-water-pumps-efcbbde4ee9f

Hand-driven and gravity fed water pumps are a key source of potable water throughout much of Africa and Asia, and the ongoing management and maintenance of such pumps is an ever-present challenge for many communities.Using data from Taarifa and the Tanzanian Ministry of Water, we want to predict which pumps are functional, which need some repairs, and which do not work at all.

We have several factors to go through to understand which of them help in the operations of the water pumps. Let's see if we can understand these and help improve maintenance operations and ensure that clean, potable water is available to communities across Tanzania.

According to Tanzania's Ministry of Water, more than 74,000 such pumps can be found throughout the country. While the installation of these pumps is largely funded via contributions from charitable and other non-governmental organizations (NGO's), their ongoing maintenance is typically the responsibility of the local community within which they reside. Unfortunately, the cost of maintaining the pumps is often beyond the means of the local community, resulting in pumps becoming non-functional. Also, local communities are often unaware of the need to perform the required maintenance due to the apparent lack of any significant problems with a pump up until the point it ultimately fails.

Through this analysis we are going to answer some of the questions as below:
Q1. Does source of water influence the functionality of the wells?
Q2. Does Age effect the condition of the wells?
Q3. What is the best mode of payment for maintenance of wells?
Q4. Does having Public Meetings help to keep the wells functional?
The data set was available on Kaggle. You can also get the data from my Git Hub.
In the article below, I have explained some of the important features to determine the functionality of wells. For a detailed explanation, please check out my git hub.

Exploration of Our Target Variable :
status_group
The target feature in this dataset is the 'status_group' feature. This feature is an indicator of whether or not the water well is 'functional', 'functional needs repairs', or 'non functional'.

We see that there is a lot of imbalance among our classes, hence we will combine "functional needs repair" and "non functional" into one.

Understanding our other features in the Data set.
amount_tsh: Total static head (amount water available to water point)
date_recorded: The date the row was entered
funder: Who funded the well
gps_height: Altitude of the well
installer: Organization that installed the well
longitude: GPS coordinate
latitude: GPS coordinate
wpt_name: Name of the water point if there is one
num_private:
basin: Geographic water basin
subvillage: Geographic location
region: Geographic location
region_code: Geographic location (coded)
district_code: Geographic location (coded)
lga: Geographic location
ward: Geographic location
population: Population around the well
public_meeting: True/False
recorded_by: Group entering this row of data
scheme_management: Who operates the water point
scheme_name: Who operates the water point
permit: If the water point is permitted
construction_year: Year the water point was constructed
extraction_type: The kind of extraction the water point uses
extraction_type_group: The kind of extraction the water point uses
extraction_type_class: The kind of extraction the water point uses
management: How the water point is managed
management_group: How the water point is managed
payment: Payment schedule
payment_type: Payment schedule
water_quality: The quality of the water
quality_group: The quality of the water
quantity: The quantity of water
quantity_group: The quantity of water
source: The source of the water
source_type: The source of the water
source_class: The source of the water
waterpoint_type: The kind of water point
waterpoint_type_group: The kind of water point
