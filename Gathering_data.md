### Lesson8:Source: Web Scraping
link:Towards Data Science: Ethics in Web Scraping
>https://towardsdatascience.com/ethics-in-web-scraping-b96b18136f01<br>


### Lesson10 :HTML Files in Python
BeautifulSoup
> https://www.crummy.com/software/BeautifulSoup/bs4/doc/#searching-the-tree<br>

How to remove \xa0 from string in Python?
> https://stackoverflow.com/questions/10993612/how-to-remove-xa0-from-string-in-python<br>

Beautiful Soup and Unicode Problems
> https://stackoverflow.com/questions/19508442/beautiful-soup-and-unicode-problems<br>

How to find elements by class
> https://stackoverflow.com/questions/5041008/how-to-find-elements-by-class<br>


### Lesson11 :Flashforward 1
Example of Tableau 
>https://public.tableau.com/profile/david.venturi#!/vizhome/BestofRottenTomatoesCriticvs_AudienceScores/BestofRottenTomatoesCriticvs_AudienceScores

### Lesson12 :Source: Downloading Files from the Internet

Fundamental course 
> https://classroom.udacity.com/courses/cs253<br>

Python Requests get() Method
> https://2.python-requests.org/en/latest/user/quickstart/#binary-response-content<br>
> https://www.w3schools.com/python/ref_requests_get.asp 

What does 'wb' mean in this code, using Python? 
> https://stackoverflow.com/questions/2665866/what-does-wb-mean-in-this-code-using-python

### Lesson13 :Text File Structure
Structure of txt

Unicode difference
> http://www.differencebetween.net/technology/difference-between-unicode-and-utf-8/
> https://lucumr.pocoo.org/2014/1/5/unicode-in-2-and-3/

Text expample
> https://kunststube.net/encoding/
> https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/

### Lesson14 :Text Files in Python
Unix style pathname pattern expansion¶
> https://docs.python.org/3/library/glob.html
> https://en.wikipedia.org/wiki/Glob_(programming)
Text 
> https://stackoverflow.com/questions/16994552/is-file-object-in-python-an-iterable/16994568#16994568
> https://stackoverflow.com/questions/8009882/how-to-read-a-large-file-line-by-line/8010133#8010133
> https://stackoverflow.com/questions/5250744/difference-between-open-and-codecs-open-in-python/22288895#22288895
### Lesson15 :Source: APIs (Application Programming Interfaces)
What is API ?
> https://www.mediawiki.org/wiki/API:Tutorial

API list for Python
> https://www.mediawiki.org/wiki/API:Client_code#Python
> https://github.com/siznax/wptools

How to use API in Python ?
> https://github.com/siznax/wptools/wiki/Usage#page-usage

Let's try !
> https://en.wikipedia.org/wiki/Mahatma_Gandhi)
> https://en.wikipedia.org/wiki/E.T._the_Extra-Terrestrial

### Lesson16 :JSON File Structure

> JSON arrays → Python lists. JSON objects → Python dictionaries.
https://www.tibco.com/blog/2014/01/23/api-data-exchange-xml-vs-json/

###  Lesson17 :JSON Files in Python

> Reading and Writing JSON to a File in Python
https://github.com/siznax/wptools/wiki/Usage

Example of json array
> page.data['image'][0]

Example of json object 
> page.data['infobox']['director']

###  Lesson18 :Mashup: APIs, Downloading Files Programmatically, and JSON
https://pillow.readthedocs.io/en/stable/
https://stackoverflow.com/questions/28056171/how-to-build-and-fill-pandas-dataframe-from-for-loop/28058264#28058264
https://2.python-requests.org/en/latest/user/quickstart/#binary-response-content


The Jupyter Notebook below contains template code that:
> - Contains title_list, which is a list of all of the Wikipedia page titles for each movie in the Rotten Tomatoes Top 100 Movies of All Time list. This list is in the same order as the Top 100.
> - Creates an empty list, df_list, to which dictionaries will be appended. This list of dictionaries will eventually be converted to a pandas DataFrame (this is the most efficient way of building a DataFrame row by row).
> - Creates an empty folder, bestofrt_posters, to store the downloaded movie poster image files.
> - Creates an empty dictionary, image_errors, to fill to keep track of movie poster image URLs that don't work.
> - Loops through the Wikipedia page titles in title_list and:
> >  - Stores the ranking of that movie in the Top 100 list based on its position in title_list. Ranking is needed so we can join this DataFrame with the master DataFrame later. We can't join on title because the titles of the Rotten Tomatoes pages and the Wikipedia pages differ.
> > - Uses try and except blocks to attempt to query MediaWiki for a movie poster image URL and to attempt to download that image. If the attempt fails and an error is encountered, the offending movie is documented in image_errors.
> >  - Appends a dictionary with ranking, title, and poster_url as the keys and the extracted values for each as the values to df_list.
> - Inspects the images that caused errors and downloads the correct image individually (either via another URL in the image attribute's list or a URL from Google Images)
> - Creates a DataFrame called df by converting df_list using the pd.DataFrame constructor.

###  Lesson21 :Storing Data
df = pd.read_csv('gathered_assessed_cleaned.csv')<br>
df.to_csv('bestofrt_master.csv', **index=False**)<br>
> Often specifying index=False is necessary too if you don't want the DataFrame index showing up as a column in your stored dataset.

### Lesson22 :Relational Database Structure
https://www.cac.cornell.edu/education/Training/DataAnalysis/RelationalDatabases.pdf

### Lesson23 :Relational Databases in Python

https://www.reddit.com/r/Python/comments/1tqjt4/why_do_you_use_pandas_instead_of_sql/
https://www.sqlalchemy.org/

### Lesson24 :Other File Formats

https://pandas.pydata.org/pandas-docs/stable/reference/index.html
http://faculty.econ.ucdavis.edu/faculty/cameron/stata/stataintro.html
https://whatis.techtarget.com/
https://www.neonscience.org/resources/learning-hub/tutorials
https://stackoverflow.com/questions/7501947/understanding-pickling-in-python
https://www.lifewire.com/what-is-an-xlsx-file-2622540
