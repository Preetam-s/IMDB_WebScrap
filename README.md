# IMDB_WebScrap

## The List of top 100 greatest movies from IMDB is accessed using the urllibs request
## The HTML is later parsed using the BeautifulSoup Library 
## Using the .finaALl() on the HTML , the divs, span tags in the soup are accessed and their content are saved to a list , particularly the titles and the the links 
## The links and titles are subsequently saved as JSON dump using the open file in write mode 'w' as links.txt and titles.txt respectively
## Each of the links in the links []  list is iterated through and a connection request is initiated
### For each of the links accessed the HTML is parsed and using the .finalALL() on the appropriate div, span classes the contents of the synopsis is saved.
### The synopsis is stored as synopsis.txt as a JSON dump
## The synopsis.txt is read using json.load() as saved as syn
## This is then saved to a data frame and further processed and cleaned using
### 1. Conversion to lower case
### 2. removing stopwords and punctuations
### 3. word stemming 
## Then using word_tokenization and sentence_tokenization the top words and frequency are calculated and word clouds are generated.
