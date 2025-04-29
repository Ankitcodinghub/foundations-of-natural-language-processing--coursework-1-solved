# foundations-of-natural-language-processing--coursework-1-solved
**TO GET THIS SOLUTION VISIT:** [Foundations of Natural Language Processing- Coursework 1 Solved](https://www.ankitcodinghub.com/product/coursework-1-foundations-of-natural-language-processing-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116140&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Foundations of Natural Language Processing- Coursework 1 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (4 votes)    </div>
    </div>
1 Introduction

This coursework consists of two parts in which you demonstrate your understanding of fundamental concepts and methods of Natural Language Processing. The coursework contains open questions and programming tasks with Python, mostly using NLTK. This coursework is worth 12.5% of your final mark for the course. It is marked out of 100.

The files with the template code you need are on the LEARN page for the assignment (click on “Assessment” on the LHS menu, then “Coursework 1 – Language Identification and Classification”). You will download a file called assignment1.tar.gz which can be unpacked using the following command to a shell prompt:

tar -xf assignment1.tar.gz

This will create a directory assignment1 which contains additional Python modules used in this coursework, together with a file named template.py, which you must use as a starting point when attempting the questions for this assignment.

There is an interim checker that runs some automatic tests that you can use to get partial feedback on your solution: https://homepages.inf.ed.ac.uk/cgi/ht/fnlp/interim1_22.py

Submission

Before submitting your assignment:

• Ensure that your code works on DICE. Your modified template.py should fully execute using python3 with or without the answer flag.

• Any character limits to open questions will be strictly enforced. Answers will be passed through an automatic filter that only keeps the first N characters, where N is the character limit given in a question.

When you are ready to submit, rename your modified template.py with your matriculation number: e.g., s1234567.py.

Submit this file via LEARN by uploading it using the interface on the LEARN website for this piece of coursework. If you have trouble please refer to the blogpost here.

Furthermore, you are required to take reasonable measures to protect your assessed work from unauthorised access. For example, if you put any such work on a public repository (e.g., GitHub), then you must set access permissions appropriately (for this coursework, that means only you should be able to access it).

2 Language Identification

In this part of the assignment, we will build a character-level language model using the Brown corpus. To do this, we will use LgramModel from nltk model, provided in assignment1.tar.gz. It is a small modification of the NgramModel you have seen before: in NgramModel we build n-grams of words, while LgramModel builds n-grams of characters (letters).

Corpus preparation: When preparing corpus data, whether from the NLTK Brown corpus or our twitter data, you should convert everything to lower-case. It is important to do this after you remove non-alphabetic tokens.

Complete the function train LM, which we use to train a character-level (or letter) language model. In this function, perform the following steps:

1. Create a list of all alphabetic tokens in a corpus (hint: use Python’s .isalpha() string method.)

2. Train a bigram letter language model using the cleaned data from step 1 (hint: Look at the LgramModel code in the nltk model, particularly the init method). For this question, as in the ‘Going Further’ sections of lab1 and lab2, you should turn on both left and right padding. Do not supply your own estimator. LgramModel will supply a default smoothing estimator.

3. Return the trained LgramModel

Using this function, train a letter language model on the Brown corpus. As the Brown corpus is rather large, training the letter language model will take some time.

Clean up the Twitter corpus to remove all non-alphabetic tokens and any tweets with fewer than 5 tokens remaining (i.e. after token removal). Given the bigram letter language model that you trained in Question 1, complete the function tweet ent in which you compute the average word entropy for each tweet in the ‘cleaned’ version of the Twitter corpus. The function should return a list of pairs of the form:

[(entropy1,tweet1),(entropy2,tweet2),…,(entropyN,tweetN)]

where N is the number of tweets in the ‘cleaned’ version of the Twitter corpus. The list should be sorted in ascending order of average word entropy value. (hint: remember you have an LgramModel and tweets in a form of lists of words. You will need to compute the entropy at the word-level, with left and right padding, and then normalise by “sentence” length. Be sure to review the arguments to LgramModel.entropy.)

Inspect the list of entropy-tweet pairs generated in question 2. What differentiates the beginning and end of the list of tweets and their entropies? Complete function open question 3 with your answer. There is a 500 character limit on this question.

The Twitter data is still noisy, in that not all character sequences are legitimate spellings and/or words of English, despite having removed non-alphabetic strings. Look at the tweets and see what (if any) currently missing preprocessing steps would be likely to improve results. Describe in detail the problems that you have identified with the data and the techniques that you could use for the cleaning up process. Give examples where appropriate. There is a 500 character limit on this question; your answers do not need to be complete sentences and you are not required to implement your suggestions.

Now we will do some tweet filtering to remove tweets that probably aren’t written in English, based on their average word entropy. Complete function tweet filter which performs the following steps:

1. Some of the tweets have non-ASCII characters, making them likely non-English. Create a list of ASCII tweets by removing the bottom 10% of tweets. To do this, use the list of average word entropy-tweet pairs, computed in the previous question. The resulting list should be sorted in ascending order of average word entropy value.

2. Using the ASCII tweets from the previous step, compute their average word entropy mean m and standard deviation σ (hint: consider using the numpy module for these computations.)

3. Using these statistics, compute a threshold t = m+σ that allows us to filter out ASCII tweets that are further away from the mean than one standard deviation. Use t to obtain a list of non-English tweets that are ASCII tweets above this threshold. The resulting list should be sorted in ascending order of average entropy value.

Overall, tweet filter should return mean and standard deviation of the ASCII tweets, and lists of ASCII and non-English tweets.

Suppose you are asked to find out what the average per word entropy of English is.

1. Name 3 problems with this question, and make a simplifying assumption for each of them.

2. What kind of experiment would you perform to estimate the entropy after you have these simplifying assumptions? Justify the main design decisions you make in your experiment.

This is an open question with no single correct answer. There is a limit of 1000 characters for this question.

3 Naive Bayes and Logistic Regression

In this part of the coursework, we look at classification, specifically at resolving attachment ambiguity of prepositional phrases (PPs). We only consider the ambiguity whether a given PP attaches to an NP in object position or to the VP:

Here is an example: the phrase “imposed a gradual ban on virtually all uses of asbestos” has two readings. Attachment to the NP:

[VP imposed [NP a gradual ban [PP on virtually all uses of asbestos]]]

and attachment of the PP to the VP:

[VP[VP imposed [NP a gradual ban]] [PP on virtually all uses of asbestos]]

The data we are going to use is from Ratnaparkhi et al. (1994), who extracted those phrases from the Penn Tree Bank and removed all words except the “head words” in order to reduce data sparsity. The head words are the verb (imposed), the head of the object NP (ban), the preposition (on) and the head of NP embedded in the PP (uses). We use raw accuracy as evaluation metric, i.e. the proportion of correctly resolved attachments out of all examples.

If you want to inspect the data directly, you can find the directory (with read access) on DICE here:

/usr/share/nltk data/corpora/ppattach/

Implement the following functions:

• get vocab (1 mark) which takes the training data as a list of tuples of the form (list with features, label) and computes the set of all features used in the training data for all classes. Use this set for smoothing.

• classify (1 mark) which takes a list of features and computes the most likely class.

A friend of yours used a logistic regression model instead of Naive Bayes and computed the model’s accuracy on the development set for different ways to extract features:

Features Example Acc

[V ] [imposed] 65.93 [N1] [ban] 66.20 [P] [on] 74.13

[N2] [uses] 61.82

[“V ” = V,“N1” = N1,“P” = P,“N2” = N2] [V=imposed, N1=ban, P=on, N2=uses] 81.08

Table 1: Accuracy of a logistic regression model for different ways to extract features. • How do you interpret the differences in accuracy between the different ways to extract features? In particular, what does it say about the task? • In the template code for the previous question, we used the feature extractor in the last row. Compare the accuracy you got in the output for Question 7 with the Naive Bayes model to the results in table 1. If there is a difference, what might be the reason for that?

There is a 500 character limit for this question.

What is the best classifier we can get for disambiguating PP attachment? In this question, we want you to write your own feature templates for a Logistic Regression model.

Inspect the features with the highest (absolute) weights (using the method show most informative features).

• Briefly describe your feature templates and your reasoning for them.

• Pick 3 examples of informative features and discuss why they make sense or why they do not make sense and why you think the model relies on them.

&lt; 81.20 0

≥ 81.20 1

≥ 82.15 2

≥ 83.10 3

≥ 84.05 4

≥ 85.00 5

References
