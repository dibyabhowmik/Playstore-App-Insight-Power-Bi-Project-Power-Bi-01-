Project Overview
This project focuses on analyzing Google Play Store applications using Power BI. The objective was to explore app popularity, ratings, user engagement, monetization, app characteristics, and update trends through an interactive multi-page dashboard.
The dataset contains information about apps, categories, ratings, reviews, installs, size, type, price, content rating, genres, and last updated date.

The dashboard is divided into four sections:
Executive Overview
Rating and User Engagement
App Characteristics and Monetization
Advanced Insights and Trends

Interactive slicers for Category and Type (Free/Paid) allow users to explore the analysis based on different app segments.

Objectives:
The main objectives of this project were:
Analyze the overall distribution of apps across categories and content ratings.
Compare free and paid applications.
Identify highly installed and highly reviewed apps.
Analyze app ratings and user engagement.
Understand the relationship between installs, reviews, ratings, price, and app size.
Examine app update trends over the years.
Identify categories and genres with strong install volumes.
Explore monetization patterns among paid applications.
Create an interactive dashboard that converts raw data into meaningful business insights.
Tools & Technologies Used
Power BI – Dashboard creation and data visualization
Power Query – Data cleaning and transformation
DAX – Measures and calculations
Microsoft Excel/CSV – Dataset and initial data handling
Data Analysis Process
1. Data Collection:
The Google Play Store dataset was imported into Power BI for analysis.

The dataset contains fields such as:
App
Category
Rating
Reviews
Installs
Type
Price
Size
Content Rating
Genres
Last Updated
Current Version
Android Version
2. Data Cleaning:
The dataset was inspected for missing values, inconsistent formats, duplicate app records, and invalid observations.
The following transformations were performed:
Converted reviews and installs into numerical formats.
Converted price and app size into usable numerical fields.
Extracted year from the Last Updated field.
Handled missing rating values.
Identified non-numeric size values such as "Varies with device".
Checked duplicate app records.
Identified an invalid rating value outside the normal 0–5 rating scale.
3. Data Transformation:

Additional analytical fields and measures were created to support:
App counts
Average ratings
Reviews
Installs
Average price
Average app size
Update-year analysis
Install ranges
Free vs Paid comparisons
4. Dashboard Development:
Four Power BI dashboard pages were created to present the analysis from different perspectives.

Dashboard 1: Executive Overview

The Executive Overview provides a high-level summary of the Google Play Store dataset.

The dashboard reports:
8,180 apps
Average rating: 4.17
Average price: 1.03
33 categories
The dashboard shows that free applications dominate the dataset, representing approximately 92.64% of the displayed apps, while paid applications account for approximately 7.36%.

The Everyone content-rating category has the largest number of apps, followed by Teen, Mature 17+, and Everyone 10+.

The top-installed app visualization is dominated by applications appearing in the 1 billion+ install range, showing the extremely high adoption achieved by a small number of major applications.

The category-level analysis also highlights strong install volumes in categories such as Communication, Game, Tools, Productivity, and Social.

The yearly update trend shows a very large increase in app updates in 2018, with more than 5K apps updated during that year.

Dashboard 2: Rating and User Engagement:

This section focuses on the relationship between app ratings, reviews, installs, and user engagement.
The average rating across different content-rating groups remains relatively close, generally around 4.1–4.3.
Free apps have significantly higher review volumes than paid apps. This is consistent with the much larger number of free applications and their broader user reach.
The dashboard also identifies highly reviewed applications such as:

Clash of Clans
Clash Royale
Clean Master
Facebook
Instagram
Messenger
Security Master
Subway Surfers
YouTube

The category analysis shows relatively high average ratings for categories such as Game, Social, and Productivity.

The installs-versus-rating visualization indicates that highly installed apps generally have ratings in the higher range, but there is no simple direct relationship between rating and install volume. High popularity appears to depend on several factors beyond rating alone.

Dashboard 3: App Characteristics and Monetization

This dashboard focuses on app size, update activity, content rating, genres, installs, and pricing.

The analysis shows that Communication has the highest average app size among the displayed major categories, followed by Tools, Game, Productivity, and Social.

The content-rating analysis confirms that free applications make up the majority of apps across the displayed content-rating groups.

Among apps with more than 1 million installs, Tools has the highest number of apps in the displayed genre analysis, followed by:

Action
Photography
Communication
Productivity
Entertainment

The app-size versus installs visualization shows that most apps are concentrated at relatively smaller sizes, while only a limited number of apps reach very high install levels.

The paid-app price versus rating analysis shows a wide range of prices, but the visualization does not indicate a clear relationship where higher prices consistently lead to higher ratings.

Dashboard 4: Advanced Insights and Trends

The Advanced Insights section focuses on deeper relationships between reviews, installs, ratings, and genres.

The analysis shows that user engagement is highly concentrated among a relatively small number of popular applications.

The install-level rating analysis shows that ratings generally remain within the 4.0–4.4 range across different install levels. This suggests that increasing install volume does not automatically result in higher ratings.

The average versus median rating comparison by genre provides additional context about the distribution of ratings and helps identify situations where the average may be affected by extreme observations.

The dashboard also provides detailed views of highly reviewed and highly rated applications for further investigation.

Key Insights

Some of the major insights from the analysis are:

The Google Play Store dataset is heavily dominated by free applications.
A relatively small group of applications accounts for a very large share of installs and reviews.
Everyone is the largest content-rating segment.
Communication, Games, Tools, Productivity, and Social are among the major categories associated with high install volumes.
The overall average app rating is approximately 4.17.
Highly installed apps generally maintain ratings around the 4+ range, but installs and ratings do not have a simple one-to-one relationship.
App update activity is heavily concentrated in 2018.
Communication apps have the highest average size among the major categories displayed.
Tools has the highest number of apps among the displayed genres with more than 1 million installs.
Paid applications represent a relatively small portion of the dataset.
Price does not show a clear direct relationship with app rating.
App size also does not appear to be a direct determinant of high install volume.
Data Quality Considerations

During the analysis, several data-quality issues were identified.

The dataset contains missing ratings, duplicate app records, and some non-numeric values in the Size field.

There is also an anomalous record with a rating of 19.0, which is outside the normal Google Play Store rating scale of 0–5. Such records should be corrected or removed before using the dataset for production-level analysis.

The Installs field contains ranges such as 100,000+ and 1,000,000,000+. Therefore, install values should be interpreted as install buckets rather than exact numbers.

Because the dataset contains repeated app names, app-level analysis should also take duplicate records into consideration.
