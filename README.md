
<h1 align="center">Twitter-Sentimental-Analysis</h1>
<p align="center">
<a href="https://twitter.com/akash_mittal18" target="blank"><img align="center" src="https://img.icons8.com/fluent/48/000000/twitter.png" alt="akash_mittal18" height="30" width="30" /></a>
<a href="https://linkedin.com/in/www.linkedin.com/in/akash-mittal-bb063417a" target="blank"><img align="center" src="https://img.icons8.com/fluent/48/000000/linkedin.png" alt="www.linkedin.com/in/akash-mittal-bb063417a" height="30" width="30" /></a>
<a href="https://instagram.com/akash_mittal18" target="blank"><img align="center" src="https://img.icons8.com/fluent/48/000000/instagram-new.png" alt="akash_mittal18" height="30" width="30" /></a>
<a href="mailto:akash.mittal898@gmail.com" target="blank"><img align="center"  src="https://img.icons8.com/color/48/000000/gmail.png" alt="akash.mittal898" height="30" width="30" /></a>
<a href="https://medium.com/@akashmittal18" target="blank"><img align="center" src="https://img.icons8.com/color/96/000000/medium-monogram.png" alt="akashmittal18" height="30" width="30" /></a>  
<a href="https://dev.to/akashmittal18" target="blank"><img align="center" src="https://d2fltix0v2e0sb.cloudfront.net/dev-badge.svg" alt="Akash Mittal's DEV Profile" height="30" width="30">
</a>
</p>

#### ABOUT

The project is based on Twitter sentimental analysis using Machine Learning .I have used multiple algorithms and based on those shown independent outputs of every algorithm. On the CLI we can see the respective accuracy of each algorithm and we can analyze which performed the best. **The user will input a twitter username and the select number of tweets he wants to analyze. Then he/she will run the program and the output will be shown in a separate window for every tweet!**

#### Instructions to run the code
1. Use command git clone https://github.com/akashmittal18/Twitter-Sentimental-Analysis-.git
2. **Open [_`test.py`_](https://github.com/akashmittal18/Twitter-Sentimental-Analysis-/blob/master/test.py)**
3. **Run**
4. **And a dialog box appears,enter the username or twitter handle of the profile without using '@' symbol**
5. **Use the slider to set the number of tweets you want to fetch**
6. **The result will show up.**

# File Details

<a href="https://github.com/akashmittal18/Twitter-Sentimental-Analysis-/blob/master/PreProcess.py">Preprocess.py</a>: It contains preprocessing function which performs following steps:- 
- It is getting the tweet  
- Removes URL using a regular expression.
- Removes emoticons using a regular expression.
- Removes username using a regular expression.
- Removes digit using a regular expression.
- Convert more than 2 letter repetitions to 2 letters.
- Removes symbols.
- Removes extra white spaces.
- Return preprocessed tweet.

<a href="https://github.com/akashmittal18/Twitter-Sentimental-Analysis-/blob/master/twitter_credentials.py">twitter_credentials.py</a>: 
In this file, we store our access token, access token secret, consumer key, and consumer secret.

<a href="https://github.com/akashmittal18/Twitter-Sentimental-Analysis-/blob/master/test.py">test.py</a>: 
- The TwitterAuthenticator class inherits the OAuthHandler class and passes in the credentials to allow access to Twitter’s API features.
- The TwitterClient class contains all the methods to interact with Twitter API and parsing tweets. Use __init__ function to handle the authentication of the API client.
- Create a object of class TwitterClient() and use the object to get twitter client API using get_twitter_client_api() function.
- create a window using Tkinter and let the user input the hashtag.
- Use API to search for the tweets of the inputted hashtag and store the tweets.
- Extract the labels and sentences and store the outcomes in y and after preprocessing the tweets store them in x.
- Then used count Vectorizer to lowercases text, performed tokenization (converts raw text to smaller units of text), used word-level tokenization (meaning each word is treated as a separate token), ignored single characters during tokenization.
- Now one iterate the tweets and one by one preprocess and transform the tweets and do predictions.

<a href="https://github.com/akashmittal18/Twitter-Sentimental-Analysis-/blob/master/twitter_credentials.py">twitter_credentials.py</a>: In this file we store our access token,access token secret, consumer key and consumer secret.

<a href="https://github.com/akashmittal18/Twitter-Sentimental-Analysis-/blob/master/AllImport.py">AllImport.py</a>: This contains all the imported modules in one place so that we don't have to include it in every file, thus reducing the redundancy.

