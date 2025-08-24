**Executive Summary**

Big Mountain Resort wants to set fair and competitive ticket prices based on what other ski resorts charge. Using data on resort size, lifts, runs, and location, we built a model that predicts fair prices. Our findings recommend a ticket price of around $83. This keeps the resort competitive while also supporting revenue goals. Scenario testing shows this price make sense given the resort’s features. We also explored changing some amenities to improve operational costs, such as adding a lift to a run below 150 feet as well as closing lower performing runs.

**Problem Statement**

The resort wants to know: What should our lift ticket prices be so they are competitive but also fair given our resort’s size and amenities?

**Data Wrangling**

The dataset originally had 330 ski resorts and 27 columns. We removed columns with too many missing values and dropped rows with incomplete or unrealistic data.

**Exploratory Data Analysis (EDA)**

We first explored the dataset visually:

<img width="567" height="453" alt="image" src="https://github.com/user-attachments/assets/16f5fe25-a929-4464-a090-461fd8258827" />

Figure A: Average ticket price by state  
This bar chart shows how prices vary across states. It helped set the context for what’s considered a “normal” range in the U.S. ski market.

<img width="1142" height="1045" alt="image" src="https://github.com/user-attachments/assets/01edaeea-81b0-4bd1-90b9-fb0690e651d8" />

Figure B: Correlation heatmap  
This highlighted which resort features most strongly relate to higher ticket prices.

We were able to also confirm that larger resorts with more terrain and lifts usually charge more.

**Model Preprocessing and Feature Engineering**

We engineered features like region categories, log-transformations of prices, and normalized numeric columns so the models could learn patterns more effectively.

**Algorithms and Evaluation Metrics**

Several models were tested, including Linear Regression and Random Forest Regression. We evaluated them to see how close predictions were to actual prices.

**Conclusion**

Our model-based analysis shows Big Mountain Resort, with 350,000 expected visitors this next season, and an average stay of 5 days, could add a chair-supported additional run below 150+ feet and would warrant an increase in the ticket price to $83, and would amount to $3.89 million in increased revenue. Additionally, Big Mountain could close its least used run and suffer no noticeable loss of revenue. 

**Future Scope of Work**

Gather real transaction data to refine predictions.  
Incorporate customer demographics and travel distance.  
Test revenue impacts of offering bundled passes or dynamic pricing.
