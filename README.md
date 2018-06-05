# Arabic-Violence-Twitter
Annotated corpus of Arabic tweets which mention a violence act. It is based on a collection on 20,000 tweets which is manually annotated using crowdflower platform.

# Data collection
As we are only interested in Arabic tweets, we use the Twitter language filter to receive only Arabic tweets. But there are still millions of tweets in Arabic, a small fraction of which may mention some kind of violence. So, further filters are required to find an initial set of tweets that may mention some kind of violence to use for manual classification. Two filters for this purpose that we discuss in this Section.


## Basic Twitter Filter
The first filter uses the Twitter API to receive Arabic tweets which contain any violence words. We prepared a word list containing 237 violence words in Arabic. We used the different stems of the word because the Twitter filter does not have an Arabic morphological analyser. So the different stems of the word are added manually to the list. The following examples show different stems of the word kill (قتل, kill),(قاتل, killer),(قتيل, one had been killed), (قتلى, many have been killed), and (مقتل, report killing action).

# Filteration
An advanced filter is used to filter out the redundant, emotional, sexual adverts, and short tweets.

#Annotation
Every tweet was classified by at least five annotators into one of eight classes i.e. Crime, Accident, Crisis, Conflict, Human Rights Abuse, Violence, Opinion, or other.


# Dataset- files

violenceKeyWords.txt: A list of violence keywords that are used to collect potential violence tweets from twitter feeds.


emoticons.txt: A list of popular emoticons used on twitter. It was collected from different resources and some tweets.


execludeList.txt: A list of Arabic words where any of them may be a sign of non real violence tweet

stop-words_arabic.txt : A list of Arbic stop words.

raw_tweetsID.txt: A list of tweet Ids of the raw collected tweets

selectedID.txt: A list of tweet Ids after applying the advanced filter and all redundant tweets are removed.

rawAnnotations: This folder includes CrowdFlower annotated tweets. It have been annotated on 3 different jobs. It is in json format where every tweet is saved as a separate json object.

mergedAnnotations: This folder contains only one file 'violenceArabicTweets.json' where all annotations are merged together and every tweet in our dataset have only one entry with all annotations. It is saved as a Json file also and the new confidence score is calculated in the same way described in the paper.

# Hint
According to Twitter T&C, we can not distribute the tweets text, So, we only distribute the Tweet ID and you may need to develop your code to grape these set of tweets by ID.


## Citation
```
Alhelbawy Ayman, Massimo Poesio, and Udo Kruschwitz. "Towards a Corpus of Violence Acts in Arabic Social Media." LREC. 2016.
```

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
