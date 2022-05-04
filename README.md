# wordpress-export-to-csv
Exporting your wordpress posts gives you an .xml file, which is not easily readable or usable for anything other than importing in another wordpress environment.
This script flattens and filters the xml file into readable rows, one per blog post.

## Current Build
This script has only been tested for my specific use-case. 
The output .csv returns (in addition to other metadata) a column for the post title, content, date, tags, and some comments. 

### Note: Wordpress style isn't consistent 
The content is in html (body, not page). If you have years of posts, as of 2022-05-04, the amount of html in your post content will vary. What amount of markup Wordpress embeds with the content has changed over the years (I.e., markup has increased). I'd welcome contributions to strip or homogenize this, since my scraping / parsing skills are limited.

## Use Case
I wanted a plaintext file format that I could either edit or import at a later date to a non-Wordpress platform. 

This script will convert the .xml file into a data frame with one post per line.
For my purposes, output to csv is sufficient for now, but this can be adapted to output individual .txt or .md files per post. 

## Acknowledgement
The code in this script is adapted from Kenneth Wong's [xml to Dataframe in R](https://urbandatapalette.com/post/2021-03-xml-dataframe-r/).
I am only responsible for streamlining the code with minor modifications and observations specific to the Wordpress export use-case.
Readers are encouraged to work through the above article for a better understanding of xml files. 
This may be necessary if you want to further customize for a slightly different usecase.
