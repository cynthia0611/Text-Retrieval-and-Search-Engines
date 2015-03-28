#####Question 1
Consider the instantiation of the vector space model where documents and queries are represented as term frequency vectors. Assume we have the following query and two documents: 

Q = “future of online education” 
D1 = “Coursera is shaping the future of online education; online education is affordable. ” 
D2 = “In the future, online education will dominate.” 

Let V(X) = [c1 c2 c3 c4] represent a part of the term frequency vector for document or query X, where c1, c2, c3, and c4 are the term weights corresponding to “future”, “of”, “online”, and “education”, respectively. Which of the following is true:
 
V(Q) = [1 1 1 1] 	V(D1) = [1 1 2 2] 	V(D2) = [1 1 1 1]			
**V(Q) = [1 1 1 1] 	V(D1) = [1 1 2 2] 	V(D2) = [1 0 1 1]**	 	
V(Q) = [1 1 1 1] 	V(D1) = [1 1 1 1] 	V(D2) = [1 0 1 1]			
 

#####Question 2
Consider the same scenario as in question (1) with the dot product as the similarity measure. Which of the following is the true:
 
Sim(Q,D1) = 6 	Sim(Q,D2) = 4			
**Sim(Q,D1) = 6 	Sim(Q,D2) = 3**

Sim(Q,D1) = 4 	Sim(Q,D2) = 3			
 

#####Question 3
Assume we have two documents with the same raw TF for all the query words (i.e. the query words appear with the same frequency in both documents). Then, using the Okapi/BM25 retrieval function, the longer document will have a lower score.
True			
False 
 

#####Question 4
If we remove the document length normalization term from the Okapi/BM25 retrieval function, and have two documents with the same raw TF for all the query words, then the longer document will have a higher score.
True			
False 
