In this is a project, I analysed the national anthems of countries across the world

# How I analysed most common words:
I used a database of national anthems created by [Lucas Turtle](https://www.kaggle.com/datasets/lucasturtle/national-anthems-of-the-world) to get the text of national anthems.<br />

I then calculated the most frequent words appearing in the national anthems. I then realised that some of the frequent words included minor words such as "to" and "your". I considered cutting by length of word. However, some short words are significant, such as "joy". <br />

I therefore decided to create a database of minor words. <br />

#### Here are my sources::
[Pronouns] (https://www.thefreedictionary.com/List-of-pronouns.htm)<br/>
[Articles] (https://7esl.com/english-articles/)<br/>
[Common Prepositions] (https://www.englishclub.com/grammar/prepositions-list.php)<br/>
[Conjunctions] (https://englishgrammarhere.com/conjunctions/100-conjunction-words-definition-and-example-sentences/) <br />
Basic verbs: handpicked eg. have, are, be<br />

You can see all the minor words I selected [here](https://github.com/ivynyayieka/anthems/blob/main/minor_words.csv)<br />

I removed these words from the list of most common words. <br />

The remaining words I then used R to create a word bubble with.<br />

# How I analysed the inclusion of the words for God in the national anthems:
Using the text of the national anthems, I searched for the words God and Lord and created a new column that indicated whether they were present and absent.<br />

To cross-check the trend for Africa, I filled in any missing data for African countries through an online search  <br />

To draw the conclusion on former British colonies in Africa being more likely to include the word God in them, I used the map. <br />

A more indepth analysis could involve merging two data sets matching countries' names to a dataset of countries' names and colonies and comparing percentages. <br />

I think another point of analysis could consider more words eg. 'Prophet', which, even though it does not reference God, can signal a countries religiousness. However, I do not know how far that expansion could go. For instance, would the words "sacred" signal religion? How about "blessed"?

# How I analysed danceability, positivity and sadness
For this, I used Spotify API to scrape national anthem tracks. <br />

In it, I extracted measures of danceability, positivity and modes or keys used for the songs. <br />

I got a lot of support for this section from looking at [LUIZ FERNANDO TOLEDO's analysis of Iron Maiden songs](
https://github.com/luizftoledo/luizftoledo.github.io/blob/main/iron-maiden-happiness/docs/data_analysis_maiden.ipynb)

# How I used the text of the  national anthems to analyse the mood 

For this, I ran the text through an emotion lexicon used by the [New York Times](https://www.nytimes.com/interactive/2017/02/28/upshot/trump-sounds-different-tone-in-first-address-to-congress.html) and also [Jonathan Soma's guidlines](https://investigate.ai/upshot-trump-emolex/trump-vs-state-of-the-union-addresses/) on reproducing the analysis.<br />

A further analysis could include more countries' national anthems translated to English so that one can compare positivity of the text using this analysis, for instance, to positivity of the music using Spotify's API to crosscheck findings. <br />

# Sources
[Lucas Turtle](https://www.kaggle.com/datasets/lucasturtle/national-anthems-of-the-world)<br/>
[Pronouns] (https://www.thefreedictionary.com/List-of-pronouns.htm)<br/>
[Articles] (https://7esl.com/english-articles/)<br/>
[Common Prepositions] (https://www.englishclub.com/grammar/prepositions-list.php)<br/>
[Conjunctions:] (https://englishgrammarhere.com/conjunctions/100-conjunction-words-definition-and-example-sentences/) <br/>
Basic verbs: handpicked eg. have, are, be <br/>
[Spotify API](https://developer.spotify.com/documentation/web-api/reference/#/operations/get-several-audio-features)<br/>
[New York Times](https://www.nytimes.com/interactive/2017/02/28/upshot/trump-sounds-different-tone-in-first-address-to-congress.html)<br/>
[Jonathan Soma's guidlines](https://investigate.ai/upshot-trump-emolex/trump-vs-state-of-the-union-addresses/)<br/>
[LUIZ FERNANDO TOLEDO's analysis of Iron Maiden songs] (
https://github.com/luizftoledo/luizftoledo.github.io/blob/main/iron-maiden-happiness/docs/data_analysis_maiden.ipynb)
