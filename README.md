# royalroad-reader
Simple python script to fetch a story from royalroad.com and convert it to epub ebook format.

# Usage

This script uses requests_html python package. https://html.python-requests.org/. Install it. 

    fetch_book.py url_of_story number_of_chapters name_of_ebook

If you want to fetch the best rated story Mother of Learning from the first chapter, execute the following command :

    python fetch_book.py https://www.royalroad.com/fiction/21220/mother-of-learning/chapter/301778/1-good-morning-brother 102 MOL
  
It reads the content of the url given ( url_of_story ) it goes to the next chapter, and it loops number_of_chapters times. name_of_ebook is the name of the file where the HTML source will be stored. MOL.html is written a the working directory.

*Note : this script has been primaly designed to fetch the story "Everybody Love Large Chest", so different stories could be appears wrong in the final file. In particular CSS-designed structure.*

# Conversion to ebook

To convert to your preferred ebook format (AZW3,MOBI,EPUB..) you need to use Calibre : https://en.wikipedia.org/wiki/Calibre_(software).  
Simply import the html file into Calibre (it automatically creates an epub ebook) and you will be able to convert it to your preferred format. 
