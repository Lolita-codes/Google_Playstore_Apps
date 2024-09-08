# Google_Playstore_Apps
This analysis provides comprehensive insights into various facets of the Android app market, from app ratings and reviews to category competitiveness and pricing strategies. It helps developers make informed decisions about app development, pricing, and category selection for better success in the highly competitive Google Play Store.
# Table of contents
• **Project Objective**  
This analysis compares thousands of apps in the Google Play Store, providing insights into various aspects of the Android app ecosystem.

•	**Methods Used** 
The analysis encompasses the following methods:   
o	Data Cleaning  
o	Preliminary Data Exploration  
o	Data Visualization  

•	**Technologies Utilized**
o	Python  
o	Pandas    
o	Plotly 

•	**Project Description**  
App data was scraped from the Google Play Store by Lavanya Gupta in 2018. Original files listed [here](
https://www.kaggle.com/lava18/google-play-store-apps).
The dataset contains 10,841 rows and 12 columns as outlined below:
o App: The name of the application.
o Category: The genre or type of the app (e.g., SOCIAL, FAMILY, GAME, etc.).
o Rating: The average user rating of the app (ranging from 0 to 5).
o Reviews: The total number of user reviews submitted for the app.
o Size_MBs: The size of the app in megabytes (MB).
o Installs: The number of installations the app has, ranging from a few downloads to over a billion.
o Type: Indicates whether the app is Free or Paid.
o Price: The price of the app in US dollars, with free apps listed as $0.
o Content_Rating: The age group suitability of the app, such as "Everyone", "Teen", "Mature 17+", etc.
o Genres: The specific genre or genres to which the app belongs (e.g., Arcade, Personalization, Business).
o Last_Updated: The last date when the app was updated.
o Android_Ver: The minimum Android version required to run the app.

•	**Project Results**  
1. **Highest Rated Apps**
The top 10 highest-rated apps include KBA-EZ Health Guide, Sway Medical, AJ Men’s Grooming, FK Dedinje BGD, and CB Video Vision, among others. Interestingly, many of these highly-rated apps have very few reviews and low install counts, suggesting that perfect 5-star ratings may be influenced by friends and family rather than a broad user base.


2. **Largest Apps by Size**
None of the apps in the dataset exceed 100 MB in size, which suggests there may be a size limit imposed by the Play Store. Several apps hit exactly this size limit, indicating developers may be optimizing their app sizes to comply with this constraint.

3. **Apps with the Most Reviews**
The most popular apps based on review count include Facebook, WhatsApp, Instagram, YouTube, Clash of Titans, and Subway Surfers. Notably, none of the top 50 most-reviewed apps are paid apps, highlighting the dominance of free apps in gaining significant user engagement.

4. **Visualizing Content Ratings**
Each Android app is assigned a content rating such as "Everyone", "Teen", or "Mature 17+". Using Plotly for visualization, it was found that 80.8% of apps are rated for "Everyone", while 11.1% are for "Teens", and smaller percentages are for other categories like "Mature 17+", "Everyone 10+", and "Adults Only 18+". Only 0.0122% of apps were unrated.

5. **Number of Installs**
Twenty apps have achieved over 1 billion installs, while three apps have only a single install. This highlights a significant disparity in the distribution of app downloads.

6. **Most Expensive Apps**
A new column, Revenue_Estimate, was created by multiplying the app's price by its install count for this purpose. The analysis uncovered 15 "I am Rich" apps with dubious prices above $300. These apps were removed from the dataset by filtering out prices above $250. The top-grossing paid app was found to be Minecraft, with estimated revenue close to $70 million, and most of the top-grossing apps were Games. This calculation assumes that all installs occurred at the listed price, although promotions and discounts are common in app stores.

7. **Most Competitive & Popular App Categories**
The Family and Game categories have the most apps, making them highly competitive which means releasing an app in these categories may be challenging in terms of visibility. The Games and Tools categories have the highest number of installs, indicating their popularity. Further analysis revealed that categories like Family, Tools, and Games have a high number of apps sharing a large number of downloads, while categories like Video Players and Entertainment have concentrated downloads in a few apps.
    
8. **Types of Genres**
There are 53 distinct genres in the Google Play Store, with Tools, Education, and Entertainment being the most prominent genres in terms of app count

9. **Free vs Paid Apps by Category**
The median number of downloads for free apps is 500,000, whereas the median for paid apps is around 5,000. While most apps on the Google Play Store are free, certain categories have a relatively higher number of paid apps, such as Personalization, Medical, and Weather. Medical apps have the highest median price at $5.49, followed by Business ($4.99) and Dating ($6.99). On the other hand, Personalization apps are cheaper, with a median price of $1.49. This suggests that users in categories like Medical and Business are more willing to pay a premium for apps.

**Key Questions Addressed by the Analysis:**
o Which apps have the highest number of reviews? Are there any paid apps among the top 50?
o What is the size of the largest Android apps in the Google Play Store?
o Is there a concentration of downloads in a few apps, or are they spread across many apps?
o How many different genres are there, and can an app belong to more than one genre?
o Should developers focus on competitive categories with many apps or popular categories with a high number of downloads?
o What should be the price of an app in various categories, and how much revenue could it potentially generate?
o How many downloads could be lost by charging for an app compared to offering it for free?
