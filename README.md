# Textual-Analysis-Framework-for-Web-Extracted-Data

This project was part of my internship so due to privacy guidelines i have not uploaded the data files 

## Objective 

To extract textual data articles from the URL given in excel file and perform text analysis to compute following variables and store the results in the output files. 

Each url has its unique url_id.

- POSITIVE SCORE
- NEGATIVE SCORE
- POLARITY SCORE
- SUBJECTIVITY SCORE
- PERCENTAGE OF COMPLEX WORDS
- FOG INDEX
- AVG NUMBER OF WORDS PER SENTENCE
- COMPLEX WORD COUNT
- WORD COUNT
- PERSONAL PRONOUNS
- AVG WORD LENGTH


# Approach to solution 

Starting with the objective, I througly analyzed all the sub tasks I need to do 

1. I created a function that extracts article title and text from a URL and saves it to a text file named after url_id in output folder. This function takes url and url_id as parameters.

2. Then i created a function that combines all the stopwords file into one(combined stopwords file) for easy processing.

3. Then i created a stopwords list using combined stopwords file.

4. then i created a list of positive and negative words on basis that they are not present in stopwords list.

5. Then creating a list of path all the files which we will need for further processing.

6. Then i created a function , remove_stopwords which takes three parameters as input file list in which we have all the location of all the files , list of stopwords, and path of output folder in which it will store the filtered files . The output of this function is in filteredFiles folder.

7. Then I proceded with the calculation of parameters asked for each file and after calculating them , simply storing them into the output_file . All the considerations given in text analysis document were taken care of while calculating the parameters except the one in which i had doubt.


## Some relevant screenshots 

- this ss shows the format of excel file , data has been blurred for privacy reasons.

- the first two columns were url_id and url , and then followed by the variables in which we have to write values.


![App Screenshot](https://github.com/SidCodes0001/Textual-Analysis-Framework-for-Web-Extracted-Data/blob/main/github%20ss.PNG?raw=true)


## Learnings from project

- Learned about web scrapping using beautiful soup library.
- learned how to efficiently read and write excel files.
- learned how to evaluate sentiment of the article or textual data on the basis of some parameters.




