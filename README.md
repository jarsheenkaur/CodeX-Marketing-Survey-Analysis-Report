# CodeX Marketing Survey Analysis Report

Analyzed survey data from 10K respondents for Marketing team of CodeX, a German beverage company, using Excel, Power Query, and Pivot Tables to create interactive dashboards on demographic insights, consumer behavior, market trends, and brand performance. Delivered actionable insights that helped the marketing team optimize campaigns, improve product distribution, and develop data-driven strategies for increasing brand awareness and market share. Quantified business opportunities through pricing, product availability, and competitive analysis, directly contributing to CodeX’s growth in the Indian market.

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
| Age_Group           | This column represents the categorized age group of the respondent. Age groups (15-18, 19-30, 31-45,46-65,65+).                                    | 
| Gender              | This column represents the gender of the respondent. (Male, Female, Non-binary).                                                                    |
| City_ID             | This column represents the ID of the city where the respondent is located.                                                                          |

Table fact_survey_responses contains 23 columns and 10000 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| Response_ID         | This column represents the unique identifier assigned to each response in the survey.                                                               |
| Respondent_ID       | This column represents the unique identifier assigned to each respondent who provided the survey response.                                          |
| Consume_frequency   | This column represents the response received for the question - How often do you consume energy drinks?                                             |
| Consume_time        | This column represents the response received for the question - When do you typically consume energy drinks?                                        |
| Consume_reason      | This column represents the response received for the question - What are the main reasons for consuming energy drinks?                              |
| Heard_before        | This column represents the response received for the question - Have you heard of our energy drink before today?                                    |
| Brand_perception    | This column represents the response received for the question - What do you think of the brand name/logo/design?                                    |
| General_perception  | This column represents the response received for the question - What is your perception of energy drinks in general?                                |
| Tried_before        | This column represents the response received for the question - Have you ever tried our energy drink before?                                        |
| Taste_experience    | This column represents the response received for the question - If yes, how would you rate the taste, flavor, and overall experience?               |
| Reasons_preventing_trying | This column represents the response received for the question - If no, what are the main reasons preventing you from trying it?               |
| Current_brands      | This column represents the response received for the question - Which energy drink brands do you currently consume or prefer?                       |
| Reasons_for_choosing_brands | This column represents the response received for the question - What are the reasons for choosing those brands over others?                 |
| Improvements_desired | This column represents the response received for the question - What improvements would you like to see in energy drinks currently available in the market?                                                                                                                                                                     |
| Ingredients_expected | This column represents the response received for the question - What ingredients do you expect in an energy drink?                                 | | Health_concerns      | This column represents the response received for the question - Are you concerned about the health impacts of energy drinks?                       |
| Interest_in_natural_or_organic | This column represents the response received for the question - Would you be interested in an energy drink with natural or organic ingredients?                                                                                                                                                                |
| Marketing_channels   | This column represents the response received for the question - Which marketing channels or platforms do you often come across energy drink advertisements?                                                                                                                                                             |
| Packaging_preference | This column represents the response received for the question - What type of packaging or bottle design would attract you to purchase an energy drink?                                                                                                                                                                      |
| Limited_edition_packaging | This column represents the response received for the question - Would you be more likely to buy an energy drink with limited edition packaging?|
| Price_range          | This column represents the response received for the question - What price range do you consider reasonable for an energy drink?                   |
| Purchase_location    | This column represents the response received for the question - Where do you typically purchase energy drinks?                                     |
| Typical_consumption_situations | This column represents the response received for the question - In which situations or activities do you typically consume energy drinks?|

## Report Features

- 4 Different Dashboards for Quick Insights.
- Multiple Data Filters.
- Click-on Navigation between Dashboards.
- Visually Appealing Dashboards.
- Variety of Charts and Diagrams make complex data easy to understand at a glance.

## Screenshots

![1  Demographic Insights](https://github.com/user-attachments/assets/df76b52e-7c1b-469c-a655-e68952362aa6)

![2  Consumer Preferences   Purchasing Behavior](https://github.com/user-attachments/assets/396ace91-72bb-4f03-8fcd-2717d480ede6)

![3  Market Research   Competition Analysis](https://github.com/user-attachments/assets/d5845c99-576b-4d5f-97bf-de24416c852b

![4  CodeX Performance](https://github.com/user-attachments/assets/4d049472-7d47-4d30-8067-ee4327fc0cf0)

![5  Pivot Tables](https://github.com/user-attachments/assets/71d06022-07e6-43b0-9c2a-4d2f1673e2d8)

## Key Insights

**1. Demographic Insights**
- Men account for 60% of Energy Drink Sales followed by Women at 35% and Non-Binary at 5%.
- Energy Drinks are more popular among youngsters as 55% of Energy Drinks Consumers belong to age group 19-30. This figure rises to 70% consumers between the ages 15-30.
- Bangalore has highest Energy Drinks Consumers at 28% followed by Hyderabad at 18%. Lucknow has least Energy Drinks Consumers at 2%.
- Energy Drinks are frequently consumed by Males mostly for 2-3 Times a Week.

**2. Consumer Preferences**
- Energy Drinks are mostly consumed to Stay Awake during Work or Study and before Exercise.
- Main reason for consuming Energy Drinks is Increased Energy and Focus.
- Energy Drinks are typically consumed during Sports or Exercise.

**3. Purchasing Behavior**
- Supermarkets are the most common choice for buying Energy Drinks followed by Online Retailers.
- Compact and Portable Cans are preferred Energy Drinks Packaging followed by Innovative Bottle Design.
- Energy Drinks with Limited Edition Packaging is mostly not preferred.
- Consumers consider Energy Drinks to be reasonably priced between 50-99 rupees.

**4. Market Research**
- Online Ads are the most effective marketing channel to reach the consumers especially the youth.
- Energy Drinks are mostly considered to be Effective.
- Caffeine is the most expected ingredient in Energy Drinks followed by Vitamins.
- Reduced Sugar Content is highly desired improvement in Energy Drinks followed by More Natural Ingredients.
- 60% of the Survey Respondents are Concerned about Health Impacts of consuming Energy Drinks.
- 50% of the Survey Respondents are Interested in Natural or Organic Ingredients to be used in Energy Drinks.

**5. Competition Analysis**
- Cola-Coka has the Largest Share in the Energy Drinks Market at 25% closely followed by Bepsi at 21%.
- Main reason for Consumers choosing Current Brand is Brand Reputation at 27% and Taste or Flavor Preference at 20%.

**6. CodeX Performace**
- 56% of the Survey Respondents have Never Heard about CodeX before.
- Only 49% of the Survey Respondents have tasted CodeX before.
- Average CodeX Taste Rating is 3.28.
- Main reasons preventing Energy Drinks Consumers for trying CodeX is that it is not available locally and concerns related to their health.
- Bangalore has the highest availability of CodeX Energy Drinks at 36% whereas Ahemdabad and Lucknow have the least availability at 1% each.
