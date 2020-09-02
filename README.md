# Topic_Modeling_withNLP
Unsupervised Learning

Here the idea is to cover the below topics:
1. What Topic Modeling is?
2. Latent Dirichlet Allocation method
3. Implementation of LDA
4. Non-Negative-Matrix Factorization
5. Implementation of NMF
6. Application of LDA and NMF
-----
1. What Topic Modeling is?

Topic modeling is a way to analyse large volume of text and clustering them into different topics. As the text is unlabeled, that is we don't have scope for applying supervised learning approaches here. We try to discover those labels out of the text. We make cluseters of documents.

2. Latent Dirichlet Allocation :

Peter Johann Gustav Dirichlet was a German Mathematician from 1800, A probabiliy distribution is named after him "Dirichlet Distribution".
2003: LDA was discovered using Dirichlet Distribution.

(Latent means, Gupt (like Latent heat))

Assumptions:
a) Documents of similar cluster use similar group of words.
b) Latent topics can be found by searching group of words that frequently occure together in documents across the corpus.

the same can be said in other words like this:
b) Documents are nothing but probability distribution over topics.
a) Topics are nothing but probability distribution over words.

The basic idea with LDA:
You select K topics, with each having some % in document.
60% business, 20% sports, 13% politics & 7% food

Now each word is assigned probability to each topic,
like for food, apple will have 70%, but table will have 20% probability


Steps in LDA:
1. select K topics (for this we must have some idea, what the text represents and in how many categories are we planning to categorize them)
2. Go through documents and assign each word to any of K topic randomly
3. Iterate over everyword in document
a) p(topic t| document d) : the proportion of word in doc d that are assigned to topic t
b) p(word w| topic t) : the proportion of topics in t from all the documents that comes from word w

c) w is assigned a new topic :  p(topic t| document d) * p(word w| topic t)
This represents that topic t has word w

This step is repeated a number of times.

so we will have output like:
Doc is assigned to topic #2
Most common words in topic are: (dog, cat, rabbit, turtle,.....)






















