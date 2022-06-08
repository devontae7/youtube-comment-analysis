Dataset link:
1. https://www.kaggle.com/datasets/datasnaek/youtube?select=UScomments.csv
2. https://www.kaggle.com/datasets/datasnaek/youtube-new

Note:-- Both files are over 600+ MB. Please download from provided link.

The dataset includes data gathered from videos on YouTube that are contained within the trending category each day.


The headers in the data are:
video_id (Common id field to both comment and video csv files)
comment_text
video id
likes
replies
title
channel_title
category_id
views
likes
dislikes
thumbnail_link
date 


## Data preprocessing in SQL:
We have imported our dataset in SQL. Then this following queries:

1. Checked the NULL values and replaced with zeros
2. Checked the empty rows and removed them.
3. Checked the datatype and converted few types.

We have removed all the columns except: video_id, comment_text, likes, replies.

## Data analysis in jupter notebook:

Here we did this following analysis:
### Analysis 1: Sentiment Analysis. 
------------------------------------------------------------------------------------------
Polarity analysis takes into account the amount of positive or negative terms that appear in a given sentence. It is useful to some extent, since it does a good job of structuring data sets.

### Analysis 2: WordCloud of positive and negative comments..
----------------------------------------------------------------
 Word cloud is a technique for visualising frequent words in a text where the size of the words represents their frequency.

### Analysis 3: Collect Entire Data of Youtube
--------------------------------------------------------------------------------------------

### Analysis 4: Which Category has maximum likes?
------------------------------------------------------------------------------------------------

### Analysis 5: Check Wheather audience is engaging or not?
------------------------------------------------------------------------------------------------

### Analysis 6: Check Trending videos
------------------------------------------------------------------------------------------------
analysis on which youtube channel produced more trending videos

### Analysis 7: Check if punctutation in title and tags has any connection with the engagement
------------------------------------------------------------------------------------------------

### Analysis 8: Emoji Analysis
----------------------------------------------------------------


## Visualization:

1. Most used Negative and Positive words

![good_wordcloud](https://user-images.githubusercontent.com/106653421/172575933-7f2be4f9-7112-4cc8-86a7-3f57f7d74abe.png)
![bad_wordcloud](https://user-images.githubusercontent.com/106653421/172575951-3d5f5456-62c9-420a-a4a5-68e90da78a56.png)

2. Most used emoji in comments
![emoji usage](https://user-images.githubusercontent.com/106653421/172568094-8ec7755f-60e7-451b-afc2-9d62a4477a7a.png)

3. a lot of people likes 'Music' category.
![top_category](https://user-images.githubusercontent.com/106653421/172568173-23900205-a7d5-4a9e-a998-0ecf9250f294.png)

4. Music, Comedy and Entertainment has most like ratio between all category
![category_Liked](https://user-images.githubusercontent.com/106653421/172568183-4816f35f-8cff-490c-922e-1c6c5727b8cf.png)

5. our correlation value between views and likes is 0.78 and with dislikes is 0.42. When views increases dislikes also increases.
![like_dislike_corr](https://user-images.githubusercontent.com/106653421/172568203-8b30e735-537f-466f-b053-87557ede76a1.png)

6. Top channel with most videos
![top_channel_video](https://user-images.githubusercontent.com/106653421/172568215-7b8596c3-79b2-472f-9dde-7d85529a1f1e.png)

7. Most punctuation used based on views
![punctuation_count](https://user-images.githubusercontent.com/106653421/172568304-1b0a151e-0c9b-4790-b1a9-0c2d77f63354.png)

8. Most emoji usage
![emoji usage](https://user-images.githubusercontent.com/106653421/172568359-10f8f35f-2185-44fa-85e8-7c2345fc239f.png)
