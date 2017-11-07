# textrank

Implementation of textrank algorithm as described in 'https://web.eecs.umich.edu/~mihalcea/papers/mihalcea.emnlp04.pdf'

textrank.py has the following implementations:
1. Read the articles from articles/ and create a graph based representation of words with POS= ['NN', 'JJ', 'NNP']
2. Create edges between two nodes in the graph if their corresponding words appear in the article within a window of 'N' words
3. Rank the nodes using Pagerank and select top n/3 words, where n=number of unique words in the article.
