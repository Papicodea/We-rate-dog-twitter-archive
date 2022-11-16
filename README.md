# WeRateDogs Prediction
## by Somto Odenigbo

## Dataset

The project consist of 3 different dataset gathered from various sources. the twitter archive was pre download from course work, The image prediction was downloaded programmatically using python request feature and the final data was to be gotten through query of twitterAPI, not in this case however as it was provided also in the course work. 
The twitter archive and image prediction was read into a pandas dataframe after gathering. While the twitterApi gotten file was read first into a tweet.json file line by line and then obtaining specific columns needed for exploration. It was read into a pandas dataframe citing the columns needed: were Tweet_id, favorite_count and retweet_count only.

The 3 dataset was Assessed thoroughly to examine the data and to understand what we are working with. Some issues with the datasets was noticed which lead us to cleaning. Some of the issues noticed were on Quality and Tidiness issues, column names error, datatype error, missing nan values, missing object values, untidiness.

To clean the data, they all needed to be copied first using the pandas .copy funtion. We proceded to change the data type to their correct ones, changing missing object values to nan values.
To get only original tweets and not replies or retweets, we dropped the rows having non original tweets. Missing data in rolls and columns was dropped which was considered unuseful for the analysis. 

Inconsistent names was corrected using the regex feature for the column names in the Image prediction dataset. 
for tidiness, the dog stages was merged into one column and a rating total was deduce.
The cleaned datasets was merged and stored into one master dataset


## Key Insights

For the Analysis, I wanted to look at some of the insights that we can get from our data twitter_master. some of the insights deduced are;
• Common Dog types - The most common Dog type is the "Golden Retriever" with a use score of 139. This makes it the most popular dog type in the area.

• Top rated dogs - the 'Pembroke' tends to be the highest rated among the dog types

• Common Dog names - *Lucy, Charlie, Cooper, Tucker, Oliver*

• Top most liked dogs - The Golden Retriever breed
• Most retweeted dog -  Golden Retriever
