# Pseudo Code

// This program will create csv from arena api scrape for my recent channel adds. It will then turn this csv scrape into a JSON file.

// import arena and time libraries


#api data
// add access token to variable
// add username (z-ai) to variable
// add all blocks i intend to scrape to an array variable


#create arrays to store data
// create arrays for days, block ids, titles, images, block types, sources, channels and channel types. each of these will be an individual array that will be pushed to later.


#iterate thru blocks
// for each block in the array of blocks,
   // assign data variables for block id, title, content, day, block type, channel, channel type.

   // if there's no block title and no content, list as "untitled." if no title and content, list title as the content

   // if block has a source, list the source URL. otherwise list "no url"

   // if block has image, list display img url as a string. otherwise, list "no image"

   // append this data to each individual array variable.  

   // prevent blockage by setting time breaks

# create csv

// import csv and json libraries

// create new csv and write to it

       // create headers in csv

       // store data under each header column in csv



# create json

// create new function, args are exiting csv file and future json file   

   // new dictionary to store data

   // read csv


       // each row turned into dictionary and is added to data dictionary

           // 1st column will be the the primary key   

   // open json writer, and use the json.dumps() function to dump data

// declare file paths  

// call json function      
