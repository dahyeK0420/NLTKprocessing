# Semi-Structured Text Data Processing 

The project extracts data from semi-structured text files - COVID-19 related tweets and export it as an organised XML file. Additionally, tweets are also tokenised and organised into corpus vocabularies, unigrams, bigrams, and sparce matrix.

## Scraping Tweets JSON data set and Export it as XML 

**``scrapingJSONTweet_XML``**

The program in the directory scrapes the tweets regarding COVID-19 with two different methods - directly scraping as a text file and by using ``json`` library. 

After scraping the tweets and store them as array of dictionaries, the tweets are then exported as ``XML`` files.

## Text Processing using NLTK

**``textProcessingNLTK** 

The program first scrapes semi-structured tweets from an excel file, ``semiStructuredTweets.xlsx``. After generating a structured data frame using pandas and xlrd, the tweets are all tokenised using ``nltk`` tokenisers. The tokens are exported as corpus vocabulary list. With the corpus vocabularies generated, top-100 most-frequently-appeared bigrams and unigrams are selected and exported into a text file. Additionally, count vectors of the corpus vocabularies are created using CountVectoriser from Sci-kit Learn. 
