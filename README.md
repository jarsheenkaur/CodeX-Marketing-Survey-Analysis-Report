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
| Age_Group           | This column represents the categorized age group of the respondent. Age groups (15-18, 19-30, 31-45,46-65,65+).                                     | 
| Gender              | This column represents the gender of the respondent. (Male, Female, Non-binary).                                                                    |
| City_ID             | This column represents the ID of the city where the respondent is located.                                                                          |

Table fact_survey_responses contains 23 columns and 10000 rows.
| Column              | Description                                                                                                                                         |
| :-------------------| :---------------------------------------------------------------------------------------------------------------------------------------------------|
| Response_ID         | This column represents the unique identifier assigned to each response in the survey.                                                               |
| Respondent_ID       | This column represents the unique identifier assigned to each respondent who provided the survey response.                                          |
| Consume_frequency   | This column represents the response received for the below question.
                        How often do you consume energy drinks?
                        a) Daily
                        b) 2-3 times a week
                        c) Once a week
                        d) 2-3 times a month
                        e) Rarely                                                                                                                                           |
| Consume_time   | This column represents the response received for the below question.
When do you typically consume energy drinks?
a) Before exercise
b) To stay awake during work/study
c) For mental alertness
d) Throughout the day                                                                                                                                                       |
| Consume_reason   | This column represents the response received for the below question.
What are the main reasons for consuming energy drinks?
a) Increased energy and focus
b) To combat fatigue
c) To boost performance
d) To enhance sports performance
e) Other                                                                                                                                                                    |
| Heard_before   | This column represents the response received for the below question.
Have you heard of our energy drink before today?
a) Yes
b) No                                                                                                                                                                       |
| Brand_perception   | This column represents the response received for the below question.
What do you think of the brand name/logo/design?
a) Positive
b) Neutral
c) Negative                                                                                                                                                                 |
| General_perception   | This column represents the response received for the below question.
What is your perception of energy drinks in general?
a) Healthy
b) Effective
c) Dangerous
d) Not sure                                                                                                                                                                 |
| Tried_before   | This column represents the response received for the below question.
Have you ever tried our energy drink before?
a) 1 (Poor)
b) 2 (Below Average)
c) 3 (Average)
d) 4 (Good)
e) 5 (Excellent)                                                                                                                                                            |
| Reasons_preventing_trying   | This column represents the response received for the below question.
If no, what are the main reasons preventing you from trying it?
a) Not available locally
b) Not interested in energy drinks
c) Unfamiliar with the brand
d) Health concerns
e) Other                                                                                                                                                                    |
| Current_brands   | This column represents the response received for the below question.
Which energy drink brands do you currently consume or prefer?
a) CodeX
b) Cola-Coka
c) Bepsi
d) Gangster
e) Blue Bull
f) Sky 9
g) Others                                                                                                                                                                   |
| Reasons_for_choosing_brands   | This column represents the response received for the below question.
What are the reasons for choosing those brands over others?
a) Brand reputation
b) Taste/flavor preference
c) Effectiveness
d) Availability
e) Other                                                                                                                                                                    |
| Improvements_desired   | This column represents the response received for the below question.
What improvements would you like to see in energy drinks currently available in the market?
a) Reduced sugar content
b) More natural ingredients
c) Wider range of flavors
d) Healthier alternatives
e) Other                                                                                                                                                                    |
| Ingredients_expected   | This column represents the response received for the below question.
What ingredients do you expect in an energy drink?
a) Caffeine
b) Vitamins 
c) Sugar
d) Guarana                                                                                                                                                                  |
| Health_concerns  | This column represents the response received for the below question.
Are you concerned about the health impacts of energy drinks?
a) Yes
b) No                                                                                                                                                                       |
| Interest_in_natural_or_organic:   | This column represents the response received for the below question.
Would you be interested in an energy drink with natural or organic ingredients?
a) Yes
b) No
c) Not Sure                                                                                                                                                                 |
| Marketing_channels   | This column represents the response received for the below question.
Which marketing channels or platforms do you often come across energy drink advertisements?
a) TV commercials
b) Online ads
c) Print media
d) Outdoor billboards
e) Other                                                                                                                                                                    |
| Packaging_preference   | This column represents the response received for the below question.
What type of packaging or bottle design would attract you to purchase an energy drink?
a) Compact and portable cans
b) Innovative bottle design
c) Eco-friendly design
d) Collectible packaging
e) Other                                                                                                                                                                    |
| Limited_edition_packaging   | This column represents the response received for the below question.
Would you be more likely to buy an energy drink with limited edition packaging?
a) Yes
b) No
c) Not Sure                                                                                                                                                                 |
|  Price_range   | This column represents the response received for the below question.
What price range do you consider reasonable for an energy drink?
a) Below 50
b) 50-99
c) 100-150
d) Above 150                                                                                                                                                                |
| Purchase_location   | This column represents the response received for the below question.
Where do you typically purchase energy drinks?
a) Local stores
b) Supermarkets
c) Online retailers
d) Gyms and fitness centers
e) Other                                                                                                                                                                    |
| Typical_consumption_situations   | This column represents the response received for the below question.
In which situations or activities do you typically consume energy drinks?
a) Sports/exercise
b) Studying/working late
c) Social outings/parties
d) Driving/commuting
e) Other                                                                                                                                                                    |
