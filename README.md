# NLP App with Streamlit
## This app is design to capture sentences and returns an automatic text summarization.

This [project](https://mhidayatz-streamlit-deploymentapp-8mcqfx.streamlitapp.com/) is deployed via Streamlit.

![](https://github.com/MHidayatz/StreamLit/blob/main/Visuals/00_Main.PNG)

## How to use the app:

### Method 1 - Home Page
User simply copy & paste text into the text editor. 
<br> Click analyze to see the results.

### Method 2 - NLP (files) 
Click on the Menu drop down menu page and select NLP (files).
<br>
Select any PDF, Docx or Txt file for app to start analyzing.

![](https://github.com/MHidayatz/StreamLit/blob/main/Visuals/02_Menu.png)

### What happens in the hood: 

- Upon reading the text, a text analysis function will loop through each word in each sentence into token using [spaCy](https://spacy.io/).
- Entities will clean the text and classify the text into specific objects with [NeatText](https://pypi.org/project/neattext/).
- Word Stats counts the number of vowels, consonants and stopwords with [NeatText](https://pypi.org/project/neattext/).
- Word Frequency counts the most number of occurance of each word. Here shows the top 5 words from corpus using [spaCy](https://spacy.io/).
- Top Keywords returns the most number of word in the corpus with [NeatText](https://pypi.org/project/neattext/).
- POS (Part of Speech Tagging) refers to assigning parts of speech to individual words in a sentence using [spaCy](https://spacy.io/).
- Sentiment is a float within the range [-1.0, 1.0]. The subjectivity is a float within the range [0.0, 1.0] where 0.0 is very objective and 1.0 is very subjective. This is perform using with [TextBlob](https://textblob.readthedocs.io/en/dev/quickstart.html).
- Plot WordCloud display the most common word used in the corpus. This is generated with [WordCloud](https://amueller.github.io/word_cloud/).
- LexRank provides a summary of the corpus that was provided using [Sumy](https://pypi.org/project/sumy/).




 
