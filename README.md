#**NLP Assignment**

---

###You are given a JSON file (tweets.json) that contains tweets (sentences) along with the name of the author.


###**Objective 1:** Get the most frequent entities from the tweets.

###**Objective 2:** Find out the sentiment/polarity of each author towards each of the entities.


###**Sample Input:**

###**Assume we have only 4 tweets:**

Tweet1 by Author1: Pink Pearl Apples are tasty but Empire Apples are not.

Tweet2 by Author2: Empire Apples are very tasty.

Tweet3 by Author3: Pink Pearl Apples are not tasty.

Tweet4 by Author1: Pink Pearl Apples smells really good.

###**Sample output:**

**Entities in the topics extracted:** 

Share a CSV with extracted entities and the frequency of the extracted entity from all the tweets in the following format.

##**objective1.csv**

##**entity / frequency**

Pink  Pearl  Apples  2

Empire  Apples  2

**Sentiment/polarity of Authors:**

Share a CSV file with predicted sentiment values with extracted
entities as columns and unique authors as rows. See the example CSV below.

##**objective2.csv**

**entity / author_name / overall_polarity**

Pink Pearl Apples   Author1   Positive

Empire Apples Author1 Negative

Empire Apples Author2 Positive

Pink Pearl Apples Author3 Negative


###**Downloading and reading the JSON file:**

Get the JSON file here: http://bit.ly/akaiketech_cll_tweets_json

###**Python code for reading the JSON file:**

import json

with open('tweets.json') as jfile:

d = json.load(jfile)

d

would be a dictionary with tweet_id as key and another dictionary as a value. The inner dictionary contains the information tweet_text and tweet_author.

See the sample below.


{"1374140386071961602":
● {tweet_author:"Hematopoiesis News"
● tweet_text:"⚕️ Scientists conducted a Phase II study of acalabrutinib in
patients with relapsed/refractory #CLL who were ibrutinib-intolerant,
and found an overall response rate of 73%. https://t.co/eJ6m4QpC5P
https://t.co/kuZz6ZO47r"}
...
}


###Instructions:

Make sure to discuss the following aspects in a text document:

● Document your approach to solve the problem, discussing the difficulties and how your proposed solution tackles them.

● Discuss the technique used and the reason why you have chosen it.

● Discuss the shortcomings or mistakes of your proposed solution with a few examples.

● If there are any shortcomings or mistakes, discuss how you would go about tackling them given more resources and time.


###Keep this in mind while implementing your solution:

● The programming language used should be Python.

● You can use any NLP technique, library or code. For some ideas, explore notable NLP toolkits like NLTK, Spacy, StanfordNLP, AllenNLP, HuggingFace Transformers, and so on. (Note that the entire solution to this assignment won’t be directly available anywhere).

● Open source implementations of some research papers related to text mining and
different types of sentiment analysis could be of help too.

● Treat this as an open ended problem and solve as much as you could. ●
Any open source code used should be credited to the author or the source.

###Submission (share below files in a zipped folder):

1. Share a text document discussing the above-mentioned items.

2. Share all the code or notebooks that computed the output. (See sample output section for required output).

3. Use the following file names for sharing the final results and upload to the appropriate slot in the google forms

Objective 1 - objective1.csv

Objective 2 - objective2.csv

Use the column names and format exactly as described in the sample output section


##Load the data


##Convert the data dictionary into DataFrame


#Dropping id as it is of no use

##Cleaning the tweets

###Below user-defined function is to remove unwanted text in the tweets.

####Removing the @user, hashtags, words starting with https, removing special characters. Lower strings.

## Tokenization
---------------
### Tokenization is a process of dividing the text into smaller segments. You can either divide the text into sentences, or words.

## Stemming
-----------
### Stemming is a text processing task in which we reduce the words to their root, which is the core part.

## Parts-of-speech tagging
--------------------------
### POS is a grammatical term that deals with the roles words play when you use them together in a sentence.

##Filtering the stop words

##Remove all the short words

---

Words that length is less than 2 letters

###**TextBlob is a python library that is built on top of nltk.**

it's easier to use and provides same additional funcitionality, such as rules-based sentiment scores.


--> In this problem, we are going to be use this function.

--> TextBlob finds all of the words and phrases that it can assign a polarity and subjectivity to an averages all of them together.

####Combining words into one list and count the appearance of each entity.

###Frequency counting of all the tweets

##**Sample output:**


Entities in the topics extracted:

-->Share a CSV with extracted entities and the frequency of the
extracted entity from all the tweets in the following format
**objective1.csv**

###**Convert the entities dataframe into Objective.csv file**

##Display the most frequent Entities from the tweets

# story generation and visualization

##**Solutions for Objective: 2**

---

####**Objective 2:** Find out the sentiment/polarity of each author towards each of the entities.

#Sentiment Analysis

# Applying Model, Variable Creation

# Converting 0 to 1 Decimal Score to a Categorical Variable

### Copying DataFrame1(df1) in DataFrame2(df2) for changing the the format for submission and conversion in csv file.

###Dropping all columns except Entity , Author_Name and Overall_polarity

#Making the entites along with author sentiments on it as a list

###Change the order of columns what in the problem statements

###**Displaying the Most frequent Entities in the topics extracted:**

###**Displaying the Sentiment/polarity of Authors**


#Approaches:

##**Tried to solve the problems.**

####--> I know there is a lot of technology involved. All about it can be learned through experience.

####--> I hope we can learn this experience from your company.

####--> I may have omitted many of these. I think there is no understanding of it.

####--> There is no such thing as difficult. It would be even better if we got more time to know about it.

####--> A few shortcome in Solution, that is not affecting most of solution. Nouns phrases can be sometimes illogical, and treating as an Entity is a waste.


####--> Removing the subjects from the Tweets and other elements that look unnecessary, But unavoidable as something like Get high accuracy of the Machine learning.

####--> I have tried to solve as much as I can.

####--> For solving problems, I look at the reference from outside and fixed it as much as I can.
