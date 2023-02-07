WeRateDogs Wrangling_Project For Udacity Data Analysis Nano Degree
Data Wrangling Process
In this project, I performed the below wrangling processes to make the data clean and ready for analysis.

Data Gathering
Data Assessing
Data Cleaning
Quality issues
I tackled the below Data Quality and Tidiness issues in the various datasets gathered.

twitter-archive-enhanced.csv
The timestamp column was an object datatype instead of datetime.

Seeveral columns had null objects represented as 'None' instead of NaN.

Dog Name column had invalid names i.e 'None', 'quite', 'such', 'the 'a', 'an' etc.

Some rows had several identical values in the expanded_url column.

These columns types (in_reply_to_status_id, in_reply_to_user_id, retweeted_status_id, retweeted_status_user_id and tweet_id) were identified as float instead of string.

image-predictions.tsv
Tweet_id field in the three datasets were stored as int values and should be strings.

Missing values from images dataset (2075 rows instead of 2356). (This was resolved at the end of the data wrangling)

Some tweet_ids had the same jpg_url.

Additional twitter data from Json file
Create_date is object datatype instead of datetime.
Tidiness issues
twitter-archive-enhanced.csv
Dog stages (doggo, floofer, pupper, puppo) were spread in different columns.

Dataset contained retweeted tweets instead of strictly original tweets. The retweet data is in columns like retweeted_status_id, retweeted_status_user_id and retweeted_status_timestamp.

Reply tweets are not “original tweets” either; this data is stored in the columns in_reply_to_status_id and in_reply_to_user_id. SOLVED

image-predictions.tsv
Breed Predictions, Confidence intervals and Dog tests are spread in three columns.
Additional twitter data from Json file
Create_date exists already in twitter-archive-enhanced.tsv.
After resolving the above issues using the data cleaning (define, code and test steps), cleaned copies were made and then they were merged into 1 using tweet_id. The wrangling process was then taken a step further to discover some key insights.

Analyzing and Visualizing Data
In this section, using the cleaned dataset, I was able to analyze and visualize insights below

Insights:
What is the most common dog breed? golden_retriever

What is the most common dog stage? pupper

What dog stage has the highest average retweet_count? puppo

What tweets have the highest average retweet_count? 744234799360020481

What are the most common dog names? Lucy

What are the most common tweet sources? Twitter for iPhone

Who are the top 5 favorite golden retrievers? Zoey, dog with ID 795464331001561088, Barney, Bella, dog with id 883482846933004288 and Alfy

what is the correlation between retweet and favorite count? 0.9143525273402237

Conclusion
Data wrangling this dataset was fun. Data wrangling is a skill that is needed since so much of the world's data isn't clean. Wrangling the dataset prevented me from making mistakes and missing out on important insights.