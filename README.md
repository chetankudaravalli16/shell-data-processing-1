# shell-data-processing

## To retrieve text from URL
1. I used "http://shakespeare.mit.edu/romeo_juliet/full.html"
1. The curl command I used to get data from the URL and store in a file is ```curl "http://shakespeare.mit.edu/romeo_juliet/full.html" -O data.txt```

## To process text data
1. ```tr ' ' '\12' < data.txt``` is the command used to maps each line into individual words.
1. ```tr ' ' '\12' < data.txt | sort``` is the command used to sort the text in data file.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c``` is the command used to sort the output and send it to uniq with pipe operator.
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr``` is used to send the output i.e unique words to sort with -nr flag. 
1. ```tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr > result.txt``` is used to store the output to result.txt file. 
1. Up arrow in bash shell is used to view the commands we executed previously. 
1. sort --help displays arguments that are used while sorting with bash commands. 
1. "-n" - To sort the data by comparing with numerical value. 
1. "-r" - To reverse the results. 
1. One dash is used for a single letter flag. 
1. Two dashes are used for flag with more than one letter. 
## Important bash commands 
1. To redirect the content of our directory ls > filename.txt command is used. 
1. Two arrows(>>) are used to append. 
1. ls is the command used to list all the contents in the default directory. 
1. cat command is used to diplay the contents of the file. Example: cat temp.txt 
