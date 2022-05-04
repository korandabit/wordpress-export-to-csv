# wordpress-export-to-csv
Rmarkdown script to convert WP exported xml file

## Context

Exporting your wordpress posts gives you an .xml file, which is not easily readable or usable for anything other than importing in another wordpress environment.

## Use Case
I want a plaintext file format that I can either edit or import at a later date to a non-Wordpress platform. Right now, this will likely be github pages.

This script will convert the .xml file into a data frame with one post per line.
For my purposes, output to csv is sufficient for now, but this can be adapted to output individual .txt or .md files per post. 

## Acknowledgement
The code in this script is adapted from Kenneth Wong's [xml to Dataframe in R](https://urbandatapalette.com/post/2021-03-xml-dataframe-r/).
I am only responsible for streamlining the code with minor modifications and observations specific to the Wordpress export use-case.
Readers are encouraged to work through the above article for a better understanding of xml files. 
This may be necessary if you want to further customize for a slightly different usecase.
