# Pseudo Code

// This program will scrape an online website delineating the work of Octavia Butler. It will create a spreadsheet archiving the container list content from the website. The spreadsheet will contain the columns: Title, Years, Notes.

// import the necessary libraries, one for downloading html and one for parsing html  
// import csv, to read and write csv files

// WITH FUNCTIONS

// define variable to contain url to scrape

// define function for scraping urls, to deal with pagination on the site. it will have 3 parameters: url, itemCount, output
// url -- the URL to scrape, this will be the URL without pagingation, and page number will be added via itemCount
// itemCount -- references the pagination on the site. the site pagination starts with 1, and adds 5000 to every page, based on the count of items (e.g. 1, 5001, 10001)
// output -- will be for specificying the content from the site to output via this function
def get_content(url, itemCount, output):

// define parameters object for the url, in this case, the url has a "dsc.position" parameter that goes up 5000 every page. so "dsc.position" will be a key with the value of the itemCount.
// make itemCount into a variable, so it can be referenced later in a loop that loops through every page.

// go to a website and download the contents of the website, put that into a variable. include URL parameters

// make beautiful soup object and feed it the html downloaded above. use "html.parser" to specify type of parsing to be done

// use method called select(). i want to select the titles, years and notes for each archive item, using the
// selectors containing this info. use the browser inspector tool to figure out which selectors contain each piece of info

// create lists variable to store output of each content type

// use for loop to go through every element for each content type. for each iteration, append the content to its list variable.
// use text() method from beautiful soup to just print out text. use the strip() method to remove all whitespace
// do the same for all content types.  

// use conditions to return certain content based on parameter for "output"  

// use a while loop to loop through every page on the site, starting with page 1.
    // create variables to store all scraping content

 

   // break out of the while loop when the results are 0, when we are at the end of the loop 
 
   // create a new .csv file to store this information. use "a" to apped, instead of "w," which will overwrite.
    
        // create 3 columns, one for title, years and notes.  
        
        // for each type of content, print the information scrape. also create a new column to store data from each content type using writerow() and pulling from each data type. 
        
        // increase itemCount by 5000, which will go on to the next page every 5000 items 
 
