# Beyond News - YouTube Comments Analysis

## Introduction
This section contains data we used for our analysis. Within the code the data is often chached in different steps. Therefore we only provide the end result and external data. 
As the comment data is to big we only provide a sample, get the whole data here: https://drive.google.com/file/d/12B0-njTEKwxo0V9FSl7lx4iLRstCdKAh/view?usp=sharing
It follows a short description of the data used:

## Data:

1. **btw21_gewaehlte-fortschreibung_utf8:** This data contains information about all elected german politicians in 2022 provided by: https://www.bundeswahlleiterin.de/bundestagswahlen/2021/ergebnisse
    ```
    btw21_gewaehlte-fortschreibung_utf8.csv
    ```

2. **pol:** This picture is used for the word clouds
    ```
    pol.jpg
    ```

3. **stopwords_ger** This data contains german stopwrods provided by:  https://github.com/stopwords-iso/stopwords-de/blob/master/stopwords-de.txt adjusted by hand
    ```
    stopwords_ger.txt
    ```

4. **videos:** This data contains all videos and the corresponding statistics and analyses 
    ```
    videos.csv:
    videoPublishedAt DATETIME: Datetime when video was published
    title STRING: Title of video
    description STRING: description of video
    viewCOUNT INT: Views of video
    likeCOUNT INT: like of video
    commentCount INT: Number of comment of Video
    videoChannelID STRING: ID that uniquely identifies channel of video
    channelName STRING: Name of channel
    transcript STRING: Transcript of video
    sentiment_transcript STRING["positive","neutral","negativ"]: Sentiment prediction of BERT model
    prob_pos_transcript FLOAT [0-1]: Sentiment prediction of BERT model
    prob_neu_transcript FLOAT [0-1]: Sentiment prediction of BERT model
    prob_neg_transcript FLOAT [0-1]: Sentiment prediction of BERT model
        

5. **comments_final_sample:**This data contains only a sample of all comments and theier analyses.
    ```
    comments_final_sample.csv:
    coomentID STRING: Id that uniquely identifies each comment
    text STRING: Text of the comment
    clean_tokens LIST[STRING]: Cleaned tokens of text
    clean_text STRING: Tokens as string
    publishedAT DATETIME: Datetime of comment posted
    authorID STRING: Id that uniquely identitifies each author
    likeCount INT: Number of likes comment has
    totalReplyCount INT: Number of second level replies comment has
    parentID STRING: commentID of first level if comment is second level
    user_replies INT: Number of replies found for user with regex
    repliedID STRING: authorID of reply found with regex
    repliedName STRING: Username of reply found with regex
    videoID STRING: Id that uniquely identifies video under which comment was posted
    channelID STRING: Id that uniqely identifies channel of video
    channelName STRING: Name of channel
    username STRING: Username of author
    threat FLOAT [0-1]: Perspective API value for text
    toxicity FLOAT [0-1]: Perspective API value for text
    identity_attack FLOAT [0-1]: Perspective API value for text
    insult FLOAT [0-1]: Perspective API value for text
    severe_toxicity FLOAT [0-1]: Perspective API value for text
    sentiment SRING ["positive","neutral","negativ"]: Sentiment prediction of BERT model
    prob_pos FLOAT [0-1]: Sentiment prediction of BERT model
    prob_neu FLOAT [0-1]: Sentiment prediction of BERT model
    prob_neg FLOAT [0-1]: Sentiment prediction of BERT model
    in_cluster INT [0|1]: 1 if in big cluster > 10 users
    cluster FLOAT: Mean toxicity in cluster
    cluster_values LIST[FLOAT]: List of mean toxicity values for cluster
    stable_tox INT [0|1]: 1 if in a stable clique using toxicity
    stable_sent INT [0|1]: 1 if in a stable clique using sentiment
    personal_attack INT [0|1]: 1 if text mentiones politician
    personal_attack_name LIST[STRING]: Name of politicians mentioned
    personal_attack_gender LIST[STRING]: Gender of politicians mentioned
    personal_attack_party LIST[STRING]: Party of politicians mentioned

6. **ids:**This ordner contains three txt files in which the video id's are safed we focus on
    ```

This concludes the overview of the Beyonf News YouTube Comments Analysis project data and resources. Should you require further assistance or have inquiries, kindly contact us. We appreciate your interest in our project.
