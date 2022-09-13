# Spam-Email-Detection

In this project I want to detect spam emails using natural language processing. I have chosen an email dataset from the Kaggle website.

---

<ins>DataSet:</ins>

<p>&#8900; The dataset consists of 5572 entries of emails and contains 2 columns (Category and Message). </p>
<p>&#8900; It does not include any missing values. </p>

<ins>Main features:</ins>

<p>&#8900; Category (Category of the message ham or spam) </p>

<p>&#8900; Message (The text of the message) </p>

---

<ins>Procedure:</ins>

* The datset consists of one categorical variable (Category). So I used LabelEncoding to encode that variable. Where 0 means the message is spam and 1 is ham.

* I removed any duplicates of the messages.

* I cleaned the messages from punctuation and stopwords.

* I convert the cleaned messages into matrix of the most frequent words, using CountVectorizer.

* I split the dataset into training & testing sets and I used the Naive Bayes model on the training set.

---

<ins>Results:</ins>

The Naive Bayes model identified the email messages as spam or not spam with 86% accuracy on the test dataset.

