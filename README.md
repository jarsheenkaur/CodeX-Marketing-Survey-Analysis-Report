# CodeX Marketing Survey Analysis Report

Analyzed survey data from 10K respondents for Marketing team of CodeX, a German beverage company, using Excel, Power Query, and Pivot Tables to create interactive dashboards on demographic insights, consumer behavior, market trends, and brand performance. Delivered actionable insights that helped the marketing team optimize campaigns, improve product distribution, and develop data-driven strategies for increasing brand awareness and market share. Quantified business opportunities through pricing, product availability, and competitive analysis, directly contributing to CodeX’s growth in the Indian market.

## Problem Statement

**Provide Insights to the Marketing Team in Food & Beverage Industry**

**Domain:**  F & B      **Function:** Marketing

**CodeX** is a German beverage company that is aiming to make its mark in the Indian market. A few months ago, they launched their energy drink in 10 cities in India.
Their Marketing team is responsible for increasing brand awareness, market share, and product development. They conducted a survey in those 10 cities and received results from **10k** respondents. The task is to convert these survey results into meaningful insights which the team can use to drive actions.

## About Data

The data as well as the problem statement are part of Codebasics Resume Challenge #6 (https://codebasics.io/challenge/codebasics-resume-project-challenge). It consists of the following 3 Tables (as CSV files) :-

Table dim_cities contain 3 columns and 10 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| City_ID             | This column represents the the ID of the city.                                                                                                      |
| City                | This column represents name of the city where the respondent is located. ("Delhi","Mumbai", "Bangalore","Chennai", "Kolkata","Hyderabad", "Ahmedabad","Pune","Jaipur", "Lucknow").                                                                                                                                    |
| Tier             | This column represents the tier category of the city.                                                                                                  |

Table dim_respondents contain 5 columns and 10000 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| Respondent_ID       | This column represents the unique identifier assigned to each respondent in the survey.                                                             |
| Name                | This column represents the name of the respondent who participated in the survey.                                                                   |
| Age_Group           | This column represents the categorized age group of the respondent. Age groups (15-18, 19-30, 31-45,46-65,65+).                                    | 
| Gender              | This column represents the gender of the respondent. (Male, Female, Non-binary).                                                                    |
| City_ID             | This column represents the ID of the city where the respondent is located.                                                                          |

Table fact_survey_responses contain 23 columns and 10000 rows.
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
| Ingredients_expected | This column represents the response received for the question - What ingredients do you expect in an energy drink?                                | | Health_concerns      | This column represents the response received for the question - Are you concerned about the health impacts of energy drinks?                       |
| Interest_in_natural_or_organic | This column represents the response received for the question - Would you be interested in an energy drink with natural or organic ingredients?                                                                                                                                                                |
| Marketing_channels   | This column represents the response received for the question - Which marketing channels or platforms do you often come across energy drink advertisements?                                                                                                                                                             |
| Packaging_preference | This column represents the response received for the question - What type of packaging or bottle design would attract you to purchase an energy drink?                                                                                                                                                                      |
| Limited_edition_packaging | This column represents the response received for the question - Would you be more likely to buy an energy drink with limited edition packaging|
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

![1  Demographic Insights](https://github.com/user-attachments/assets/4df42e0f-1471-4f61-9001-b58a9a7daa7e)

![2  Consumer Preferences   Purchasing Behavior](https://github.com/user-attachments/assets/396ace91-72bb-4f03-8fcd-2717d480ede6)

![3  Market Research   Competition Analysis](https://github.com/user-attachments/assets/99f41e46-ecea-469a-941e-8e3d37df39d2)

![4  CodeX Performance](https://github.com/user-attachments/assets/4d049472-7d47-4d30-8067-ee4327fc0cf0)

![5  Pivot Tables](https://github.com/user-attachments/assets/71d06022-07e6-43b0-9c2a-4d2f1673e2d8)

## Key Insights

### **1. Demographic Insights**
- **Gender Breakdown:** 60% of energy drink consumers are male, 35% female, and 5% non-binary. The energy drink market globally is often dominated by male consumers, who are seen as more inclined toward products associated with physical activity, performance enhancement, and sports.
- **Age Distribution:** 55% of energy drink consumers are aged 19-30, with the figure rising to 70% in the 15-30 age bracket. Globally, younger demographics are the largest consumers of energy drinks, as they are marketed for high-energy lifestyles such as sports and long study or work hours.
- **City Insights:** Bangalore leads with 28% of energy drink consumers, followed by Hyderabad at 18%. In contrast, Lucknow accounts for only 2%. Urban areas tend to have higher energy drink consumption due to the fast-paced lifestyle, which aligns with the growth of energy drinks in metro cities like Bangalore.
- **Consumption Frequency:** Energy drinks are frequently consumed 2-3 times per week, primarily by males and individuals aged 18-30.

### **2. Consumer Preferences**
- **Primary Consumption Reasons:** Consumers primarily drink energy beverages to stay awake during work/study and before exercise, with the top motivations being increased energy and focus. Globally, the energy drink market thrives on the promise of alertness and productivity boosts, valued highly by students and professionals.
- **Consumption Occasions:** Most respondents consume energy drinks during sports or exercise, mirroring global trends where energy drinks are heavily marketed to athletes and fitness enthusiasts for performance enhancement.

### **3. Purchasing Behavior**
- **Preferred Purchase Channels:** Supermarkets are the most common purchase location, followed by online retailers. In India, the rapid rise of e-commerce has driven the growth of online purchases of energy drinks, especially during the pandemic.
- **Packaging Preference:** Consumers favor compact and portable cans, followed by innovative bottle designs. This reflects the global trend where convenience in consumption plays a significant role, with compact packaging preferred for ease of transportation and storage. Additionally, there is little interest in limited edition packaging, indicating that energy drink packaging should focus on everyday practicality rather than exclusivity or novelty.
- **Price Sensitivity:** The preferred price range for energy drinks is between INR 50-99. Pricing is a critical factor in the Indian market, where affordability often determines brand loyalty, especially in the youth segment.

### **4. Market Research**
- **Effective Marketing Channels:** Online ads are most effective in reaching young consumers, particularly through platforms like Instagram and YouTube. Globally, digital marketing has proven to be the most powerful tool for energy drinks, particularly in engaging younger, tech-savvy audiences.
- **Key Ingredients:** Caffeine is the most expected ingredient, followed by vitamins. Caffeine has long been the cornerstone of energy drinks worldwide, known for boosting alertness. However, consumers are increasingly expecting healthier ingredients like vitamins.
- **Perceived Effectiveness of Energy Drinks:** Consumers generally view energy drinks as effective, primarily for boosting energy, focus, and endurance. This perception underscores their continued use during demanding activities such as work, study, and exercise, highlighting energy drinks' role in improving performance and alertness.
- **Desired Improvements:** Consumers are calling for reduced sugar content and more natural ingredients, in line with a global shift toward health-conscious beverages. Brands like Red Bull have already begun offering sugar-free options to meet this growing demand.
- **Health Concerns:** 60% of respondents are concerned about health impacts, and 50% are interested in natural or organic ingredients. This reflects a global consumer trend where awareness of energy drink health risks (heart problems, high sugar content) has led to demand for healthier alternatives.

### **5. Competition Analysis**
- **Market Share:** Cola-Coka dominates the Indian energy drinks market with a 25% share, closely followed by Bepsi at 21%. 
- **Brand Choice Factors:** Consumers select their preferred brands primarily based on brand reputation (27%) and taste/flavor preference (20%). Established brands benefit from high brand equity, making it difficult for new entrants like CodeX to penetrate the market without significant differentiation . 

### **6. CodeX Performace**
- **Brand Awareness:** 56% of respondents have never heard of CodeX, indicating a critical need for increased marketing efforts. This suggests that CodeX has not yet established a strong brand presence, a major factor in the competitive energy drink market .
- **Trial Rates:** Only 49% of respondents have tried CodeX, indicating a gap in market penetration. 
- **Taste Rating:** CodeX’s taste rating of 3.28 shows room for improvement, especially since taste/flavor is the second most important factor for brand preference .
- **Barriers to Trial:** Limited availability and health concerns are the main reasons preventing consumers from trying CodeX. This indicates that the brand needs to address both distribution challenges and health-related perceptions to succeed .
- **City-wise Availability:** CodeX is most available in Bangalore (36%), but barely available in cities like Ahmedabad and Lucknow (1%). Expanding availability in these regions could lead to increased trials and brand growth.
