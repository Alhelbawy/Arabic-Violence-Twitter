===============================
Towards a corpus of violence acts in Arabic social media
Dataset Description
By: Ayman Alhelbawy
date: 10/3/2016
===============================

violenceKeyWords.txt: A list of violence keywords that are used to collect potential violence tweets from twitter feeds.
emoticons.txt: A list of popular emoticons used on twitter. It was collected from different resources and some tweets.

execludeList.txt: A list of Arabic words where any of them may be a sign of non real violence tweet
stop-words_arabic.txt : A list of Arbic stop words.

raw_tweetsID.txt: A list of tweet Ids of the raw collected tweets

selectedID.txt: A list of tweet Ids after applying the advanced filter and all redundant tweets are removed.

rawAnnotations: This folder includes CrowdFlower annotated tweets. It have been annotated on 3 different jobs. It is in json format where every tweet is saved as a separate json object.

mergedAnnotations: This folder contains only one file 'violenceArabicTweets.json' where all annotations are merged together and every tweet in our dataset have only one entry with all annotations. It is saved as a Json file also and the new confidence score is calculated in the same way described in the paper.

