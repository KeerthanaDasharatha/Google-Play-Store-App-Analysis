

# Introduction and Data Overview:
This project explores and analyzes mobile applications available on the Google Play Store.
It combines app metadata and user reviews to gain insights into trends, user sentiment, and app popularity.

![image](https://github.com/user-attachments/assets/537e199d-b308-4372-9460-471d30c8100b)



googleplaystore.csv:                
Contains metadata for over 10,000 apps including ratings, category, reviews, installs, type, price, content rating, and update information.

googleplaystore_user_reviews.csv:                                                                                                                                                          
    Includes user reviews with sentiment analysis (positive, negative, neutral), sentiment polarity, and subjectivity.

# Column Names:
## 1.Googleplaystore.csv

App: Name of the app.
Category: App category (e.g., GAME, EDUCATION).

Rating: User rating of the app (0 to 5).

Reviews: Number of user reviews.

Size: Size of the app (e.g., 12M, 25k); can contain text.

Installs: Number of installations (e.g., 1,000+, 5,000,000+).

Type: Indicates if the app is Free or Paid.

Price: Price of the app (free v/s paid)

Content: Rating	Target age group (e.g., Everyone, Teen).

Genres: App genres (can be multiple or more specific than category).

Last Updated: Date the app was last updated.

Current Ver: Current version of the app.

Android Ver: Minimum Android version required to run the app.

## 2.googleplaystore_user_reviews:

App: Name of the app (used to join with the first dataset).

Translated_Review: Review left by user (translated to English).

Sentiment	Classified sentiment: Positive, Negative, or Neutral.

Sentiment_Polarity: Score from -1 (very negative) to 1 (very positive).

Sentiment_Subjectivity: Score from 0 (objective) to 1 (subjective).

## Libraries Used:
pandas, numpy – for data manipulation and cleaning.

matplotlib, seaborn – for data visualization.

datetime – for handling dates in the Last Updated column.

## Data Acquisition & Preparation:

Merged both datasets on the App column.

Cleaned columns: removed duplicates, handled missing values.

Converted columns like Reviews, Installs, Size, and Price into numeric formats.

Extracted sentiment metrics from the reviews dataset.

## Research Problem Statement
With the rapid growth of mobile applications on platforms like the Google Play Store, understanding what drives user satisfaction and app success is critical for developers, marketers, and business stakeholders. User ratings and sentiment are key indicators of app performance and user engagement. However, the factors influencing these indicators are complex and multifaceted. While previous research and app store optimization strategies have highlighted variables like app quality, user interface, and functionality, there is still a lack of comprehensive analysis regarding how pricing, number of installs, and app category directly influence user satisfaction and ratings.

This study aims to explore the relationship between app features—such as pricing (free vs. paid), popularity (measured by the number of installs), and app category (e.g., Games, Education, Health)—and their impact on user feedback in terms of ratings and sentiment in user reviews.

## Objectives:

Identify top-rated categories and genres.

Compare free vs paid apps.

Analyze user sentiment based on app features.

Explore correlations between app size, rating, installs, and last updated.

## Key Insights:
* Most apps are rated highly (right-skewed rating distribution).

* Free apps dominate the Play Store, but paid apps have varied install trends.

* Apps with frequent updates tend to maintain better ratings.

* Most apps are free and fall under the “Everyone” content rating.

* Highly rated apps are often regularly updated and lightweight.

* Sentiment polarity is positively skewed for top apps.

* Categories like “GAME” and “PRODUCTIVITY” receive the most user engagement.

* Positive sentiment is more common in apps with high ratings.

## Conclusion:
The Play Store is dominated by free apps with high ratings and frequent updates. Sentiment analysis and feature exploration reveal valuable patterns that can guide app development and marketing strategies.



