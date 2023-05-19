# DATA-606-Capstone-Project-Conversational-Recommender-System-for-Restaurants

### Working Demo

![](https://github.com/ihetvipatel/DATA-606-Capstone-Project-Conversational-Recommender-System-for-Restaurants/blob/main/chatbot.gif | width=100)

## Conversational Recommender System for Restaurants
Team Members: Hafsa Chaudhry, Omar Agha Khan, Hetvi Patel, and Sarah Denlinger

## Dataset
The dataset can be obtained from Yelp's Open Dataset website (https://www.yelp.com/dataset). This dataset originally included over 5 million reviews for businesses in 11 metropolitan areas across 4 countries. The dataset was decreased and now only includes restaurants in Philadelphia, PA.

The final dataset was 55,415 rows and 28 columns. It included 416 businesses.

![image](https://github.com/ihetvipatel/DATA-606-Capstone-Project-Conversational-Recommender-System-for-Restaurants/assets/129907365/f47cb799-06b7-4205-916e-4fdfd2fa2d8d)

The image above shows the location of the restaurants in the dataset.

The dataset includes information such as the reviewer's name, the date of the review, the rating given by the reviewer, and the text of the review. There are also details about the business such as its name, location, category, and attributes.

## Our Approach

We built a conversational recommendation system to recommend restaurants to people in Philadelphia. PA. A conversational recommender system is a type of recommendation system that is integrated into a chatbot and uses natural language processing (NLP) and machine learning techniques to make recommendations in a conversational manner. To build a conversational recommender system for restaurants, we would need to perform several steps.

<img width="763" alt="image" src="https://github.com/ihetvipatel/DATA-606-Capstone-Project-Conversational-Recommender-System-for-Restaurants/assets/129907365/8b0ab595-6845-4b9d-bd14-ec937697159c">

The image above depicts our pipeline for preparing the data for the recommendation models.
### Preprocessing Data
We first had to clean and prepare the restaurant review data for analysis. This included filtering out businesses that did not have a "food" or "restaurant" included in their category description. We also merged the Reviews dataset with the Businesses Dataset.

### Sentiment Analysis
We then performed sentiment analysis on the reviews. We used Hugging Face to determine the overall sentiment (positive, negative, or neutral) of each review.

### Keyword Extraction
We also used Rapid Automatic Keyword Extraction to extract the most frequently mentioned keywords and phrases in the reviews to determine the topics being discussed.

### Recommendation Engine
We used the results of the sentiment analysis and keyword extraction to build a recommendation engine that can suggest restaurants to users based on their preferences and opinions.

### Chatbot
We created a chatbot as well using the ChatGPT Turbo 3.5 model. This model interacts with both the user and the recommendation system. The chatbot first asks the user for their zip code and then validates that they gave a valid zip code in Philadelphia. If the user does not enter a valid zip code, the chatbot prompts them to enter their zip code again. The chatbot then sends the information to the location recommendation system. Once the results are returned to the chatbot, the chatbot provides them to the user. The user can also give a restaurant that they like and the content based recommendation system can provide other restaurants that the user may like based off of the restaurant that the user provided.

We also used Gradio to build a front end for the chatbot to make it more user friendly.


## Challenges
One biggest challenges during this project was the size of the dataset. The original dataset included 3,567,667 rows. When running code using this dataset, the code would crash or take hours to run. Due to this, we had to decrease the size of the dataset. This was done by taking 10% of the Yelp Business dataset and merging it with the Yelp Reviews dataset. The dataset was decreased from 3,567,667 rows to 415,066 rows. We still ran into issues with the size of the dataset while running the location based remcommendation model. Due to this issue, we decided to further decrease the size of the dataset by only focusing on restaurants in Philadelphia, PA. This helped run time significantly and decreased the frequency of the notebooks crashing while running our code.

## Future Work
One area of this project that we would like to expand on in the future is having the recommendation model factor the time of day that the user is wanting to go to the restaurant into the recommendations. Focusing more on this area would prevent users from being recommended restaurants that are closed at the time that they are wanting to go eat.
