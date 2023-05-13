# DATA-606-Capstone-Project-Conversational-Recommender-System-for-Restaurants

## Project Proposal: Conversational Recommender System for Restaurants
Team Members: Hafsa Chaudhry, Omar Agha Khan, Hetvi Patel, and Sarah Denlinger

Dataset: The dataset can be obtained from Yelp's Open Dataset website (https://www.yelp.com/dataset). 

This dataset includes over 5 million reviews for businesses in 11 metropolitan areas across 4 countries.

Basic Info: The dataset includes information such as the reviewer's name, the date of the review, the rating given by the reviewer, and the text of the review. There are also details about the business such as its name, location, category, and attributes.

A conversational recommender system is a type of recommendation system that is integrated into a chatbot and uses natural language processing (NLP) and machine learning techniques to make recommendations in a conversational manner. To build a conversational recommender system for restaurants, we would need to perform several steps, including:

Analyses:
Pre-processing the data: Clean and prepare the restaurant review data for analysis.
Sentiment Analysis: Determine the overall sentiment (positive, negative, or neutral) of each review.
Text Classification: Classify the reviews into categories based on their content, such as food quality, service quality, atmosphere, etc.
Keyword Extraction: Extract the most frequently mentioned keywords in the reviews to determine the topics being discussed.
Recommendation Engine: Use the results of the sentiment analysis, text classification, and keyword extraction to build a recommendation engine that can suggest restaurants to users based on their preferences and opinions.

Performance Evaluation Metric:
For sentiment analysis, the performance evaluation metric could be the accuracy of the sentiment analysis results.
For text classification, the performance evaluation metric could be the F1-score, which is a measure of the accuracy of the classifier.
For the recommendation engine, the performance evaluation metric could be the Mean Average Precision (MAP), which measures the average precision of the recommendations made by the engine.

Integration into Chatbot: Create a chatbot that can engage in natural language conversations with users and make recommendations based on the results of the recommendation engine. The chatbot can ask questions to gather information about the user's preferences and use that information to make recommendations.  For example, the chatbot might ask questions like "Are you in the mood for Italian food?" or "Do you prefer fine dining or casual dining?" Based on the user's answers, the chatbot can use the recommendation engine to suggest restaurants that match the user's preferences. The chatbot can then provide the user with additional information about the recommended restaurants, such as their locations, menus, and hours of operation

## Pipeline
The user inputs their state and food preferences into the chatbot. The chatbot then validates the user's input and sends it to the recommendation model. The recommendation model then returns restaurant recommendations. The chatbot receives these recommendations and provides them to the user.

![image](https://github.com/ihetvipatel/DATA-606-Capstone-Project-Conversational-Recommender-System-for-Restaurants/assets/129907365/c1102c67-ae39-4f4b-8541-711b010b6346)

## Challenges
One biggest challenges during this project was the size of the dataset. The original dataset included 3,567,667 rows. When running code using this dataset, the code would crash or take hours to run. Due to this, we had to decrease the size of the dataset. This was done by taking 10% of the Yelp Business dataset and merging it with the Yelp Reviews dataset. The dataset was decreased from 3,567,667 rows to 415,066 rows. This helped run time significantly and decreased the frequency of the notebooks crashing while running our code.

## Future Work
One area of this project that we would like to expand on in the future is having the recommendation model factor the time of day that the user is wanting to go to the restaurant into the recommendations. Focusing more on this area would prevent users from being recommended restaurants that are closed at the time that they are wanting to go eat.
