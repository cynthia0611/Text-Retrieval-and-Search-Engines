```
####Question 1
The sentence “A man saw a boy with a telescope” is syntactically ambiguous and has two distinct syntactic structures.
True
False			
```

Question 2
Which of the following is false:
Your Answer		Score	Explanation
Querying and browsing are both examples of the text pull mode			
Search engines rely on the text push mode			
Recommender systems are based on the text push mode			
Browsing is suitable when the user doesn't know what keywords to use	Inorrect	0.00	
Total		0.00 / 1.00	

Question 3
Consider the instantiation of the vector space model where documents and queries are represented as bit vectors. Assume we have the following query and two documents: 

Q = “healthy diet plans” 
D1 = “healthy plans for weight loss. Check out other healthy plans” 
D2 = “the presidential candidate plans to change the educational system.” 

Let V(X) = [b1 b2 b3] represent a part of the bit vector for document or query X, where b1, b2, and b3 are the bits corresponding to “healthy”, “diet”, and “plans”, respectively. Which of the following is true:
Your Answer		Score	Explanation
V(Q) = [1 1 1] 	V(D1) = [1 1 1] 	V(D2) = [0 0 0]			
V(Q) = [1 1 1] 	V(D1) = [1 1 1] 	V(D2) = [0 0 1]			
V(Q) = [1 1 1] 	V(D1) = [2 0 2] 	V(D2) = [0 0 1]			
V(Q) = [1 1 1] 	V(D1) = [1 0 1] 	V(D2) = [0 0 1]	Correct	1.00	
Total		1.00 / 1.00	

Question 4
Consider the same scenario as in question (3) with dot product as the similarity measure. Which of the following is true:
Your Answer		Score	Explanation
Sim(Q,D1) = 4 	Sim(Q,D2) = 1			
Sim(Q,D1) = 3 	Sim(Q,D2) = 1			
Sim(Q,D1) = 3 	Sim(Q,D2) = 0			
Sim(Q,D1) = 2 	Sim(Q,D2) = 1	Correct	1.00	
Total		1.00 / 1.00	

Question 5
When we use the Okapi/BM25 retrieval function to score documents for a query that has only one term, the ranking of documents is not affected by IDF weighting, i.e. if we remove the IDF weighting term from the ranking function, we will still get the same ranked list of documents.
Your Answer		Score	Explanation
False			
True	Correct	1.00	
Total		1.00 / 1.00	

Question 6
Which of the following is not true about the Okapi/BM25 ranking function:
Your Answer		Score	Explanation
It implements the TF and IDF heuristics			
The TF can grow to plus infinity			
It penalizes long documents and rewards short ones			
It is a member of the vector space model	Inorrect	0.00	
Total		0.00 / 1.00	

Question 7
Suppose we compute the term vector for a baseball sports news article in a collection of general news articles using TF weighting only. Which of the following words do you expect to have the highest weight?
Your Answer		Score	Explanation
the	Correct	1.00	
baseball			
computer			
Total		1.00 / 1.00	

Question 8
Assume the same scenario as in (7) but with TF-IDF weighting. Which of the following words do you expect to have the highest weight in this case?
Your Answer		Score	Explanation
the			
computer			
baseball	Correct	1.00	
Total		1.00 / 1.00	

Question 9
Consider the following retrieval formula: 



where c(w, D) is the count of word w in document D, dl is the document length, avdl is the average document length of the collection, N is the total number of documents in the collection, and df (w) is the number of documents containing word w. Which of the following is true about the given scoring function:
Your Answer		Score	Explanation
It rewards longer documents rather than penalizing them, and its IDF component rewards common terms instead of penalizing them.			
It will perform well as it supports all the retrieval heuristics.	Inorrect	0.00	
It implements TF weighting and document length normalization appropriately, but its IDF component rewards common terms instead of penalizing them			
It implements TF-IDF weighting appropriately, but it rewards longer documents rather than penalizing them.			
Total		0.00 / 1.00	

Question 10
When using the Okapi/BM25 retrieval function on a corpus where each document has exactly the same length, removing the document length normalization term from the retrieval function will change the ranking of documents.
Your Answer		Score	Explanation
False	Correct	1.00	
True			
Total		1.00 / 1.00
