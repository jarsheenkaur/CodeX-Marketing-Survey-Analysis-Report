# CodeX Marketing Survey Analysis Report

## Problem Statement

**Provide Insights to the Marketing Team in Food & Beverage Industry**

**Domain:**  F & B      **Function:** Marketing

**CodeX** is a German beverage company that is aiming to make its mark in the Indian market. A few months ago, they launched their energy drink in 10 cities in India.
Their Marketing team is responsible for increasing brand awareness, market share, and product development. They conducted a survey in those 10 cities and received results from **10k** respondents. The task is to convert these survey results into meaningful insights which the team can use to drive actions.

## About Data

The data as well as the problem statement are part of Codebasics Resume Challenge #6 (https://codebasics.io/challenge/codebasics-resume-project-challenge). It consists of the following 3 Tables (as CSV files) :-

Table dim_cities contains 3 columns and 10 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| City_ID             | This column represents the the ID of the city.                                                                                                      |
| City                | This column represents name of the city where the respondent is located. ("Delhi","Mumbai", "Bangalore","Chennai", "Kolkata","Hyderabad", "Ahmedabad","Pune","Jaipur", "Lucknow").                                                                                                                                    |
| Tier             | This column represents the tier category of the city.                                                                                                  |

Table dim_respondents contains 5 columns and 10000 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| Respondent_ID       | This column represents the unique identifier assigned to each respondent in the survey.                                                             |
| Name                | This column represents the name of the respondent who participated in the survey.                                                                   |
| Age_Group           | This column represents the categorized age group of the respondent. Age groups (15-18, 19-30, 31-45,46-65,65+).                                     | 
| Gender              | This column represents the gender of the respondent. (Male, Female, Non-binary).                                                                    |
| City_ID             | This column represents the ID of the city where the respondent is located.                                                                          |

Table fact_survey_responses contains 23 columns and 10000 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
| room_class          | This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.                                         |
| room_id             | This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.                                                                             |
