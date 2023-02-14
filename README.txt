WeRateDogs Wrangling_Project For Udacity Data Analysis Nano Degree
Data Wrangling Process
In this project, I performed the below wrangling processes to make the data clean and ready for analysis.

Data Gathering
Data Assessing
Data Cleaning
Quality issues
I tackled the below Data Quality and Tidiness issues in the various datasets gathered.

Quality Issues
Archive File
1. Some rows are retweets not original tweets
2. Datatype missmatch need to be corrected i.e timestamp
3. Redundant Columns i.e not needed for analysis, need to be dropped
4. NaNs represented as 'None' (str) for name, doggo, floofer, pupper, and puppo columns need to be rectified.
5. The rating numerator and denometor columns need standardization
6. Extra urls in the text column
7. Name column values need standardisation
Image Prediction File
 1. There are some missing rows in images dataset (2075 rows instead of 2356): 
 either the rows are missing or some tweets didn't have dog images
 2. There are duplicated jpg_url's 
 3. Redundant Columns i.e not needed for analysis, need to be dropped
 4. Column names are non-descriptive
Api Data File
 1. There are some missing rows in the Api Dataset (2323 rows instead of 2356)
 2. id column to be renamed as tweet_id
 3. Only the id, retweet_count and favorite_count are needed for this analysis, the rest will be dropped
 
Tidiness Issues
1. The doggo, puppo, pupper and floofer columns for dog stages in the twitter_archive table are in seperate columns instead 
of a single column
2. p1, p2, p3 can be merged to one prediction column based on the true values of p1_dog, p2_dog and p3_dog. 
P1_conf, p2_conf,P3_config can also be merged to one column to align with the confidence level of the predictions.
3. All three datasets need to be joined into one.

Analyzing and Visualizing Data
In this section, using the cleaned dataset, I was able to analyze and visualize insights below

Insights:
Which is the most owned breed? golden_retriever

Is the Golden retriever also the most favorited or retweeted dog breed? Although the Golden retriever is the most owned, Samoyed breed seems to be the most liked and retweeted dog breed.

Is there a correlation between rating vs retweet counts? Retweet count vs favorite counts? Favourite Counts and Retweet counts have a positive correlation.

What is the most common dog stage? pupper

Is the most common stage also the highest rated? Floofer is the highest rated dog stage and Pupper being the most common dog stage is the least rated



Conclusion
Data wrangling this dataset was fun. Data wrangling is a skill that is needed since so much of the world's data isn't clean. Wrangling the dataset prevented me from making mistakes and missing out on important insights.
