#####Question 1
Suppose a query has a total of 4 relevant documents in the collection. System A and System B have each retrieved 10 documents, and the relevance status of the ranked lists is shown below: 

	System A: [- + - - - - - - - -]
	System B: [+ + - - - - - - - -]

where the leftmost entry corresponds to the highest ranked document, and the rightmost entry corresponds to the lowest ranked document. A “+” indicates a relevant document and a “-” corresponds to a non-relevant one. For example, the top ranked document retrieved by System A is non-relevant, whereas the top ranked one by B is relevant. 

What is the precision at 10 documents of both systems?
Your Answer		Score	Explanation
P(A) = 1/4 	P(B)= 2/4			
P(A) = 9/10 	P(B)= 8/10			
P(A) = 1/10 	P(B)= 2/10	Correct	1.00	
P(A) = 1/40 	P(B)= 2/40			

#####Question 2
Assume the same scenario as in Question 1. What is the recall of both systems?
Your Answer		Score	Explanation
R(A) = 1/4 	R(B)= 2/4	Correct	1.00	
R(A) = 1/10 	R(B)= 2/10			
R(A) = 1/40 	R(B)= 2/40			
R(A) = 9/10 	R(B)= 8/10			

#####Question 3
Assume the same scenario as in Question 1. What is the average precision of both systems?
Your Answer		Score	Explanation
AP(A) = 1/20 	AP(B) = 1/5			
AP(A) = 7/20 	AP(B) = 7/10			
AP(A) = 1/10 	AP(B) = 1/5			
AP(A) = 1/8 	AP(B) = 1/2	Correct	1.00	

#####Question 4
Assume you have two retrieval systems X and Y. For a specific query, system X has a higher precision at 10 documents compared to Y. Can system Y have a higher average precision on the same query?
Your Answer		Score	Explanation
No			
Yes	Correct	1.00	

#####Question 5
Let w1, w2, and w3 represent three words in the dictionary of an inverted index. Suppose we have the following document frequency distribution: 

Word	Document Frequency
w1	1000
w2	100
w3	10

Assume that each posting entry of document ID and term frequency takes exactly the same disk space. Which word, if removed from the inverted index, will save the most disk space?
Your Answer		Score	Explanation
w1	Correct	1.00	
w3			
w2			
We cannot tell from the given information.			

#####Question 6
Assume we have the same scenario as in Question 5. If we enter the query Q= “w1 w2” then the minimum possible number of accumulators needed to score all the matching documents is:
Your Answer		Score	Explanation
1000			
10	Inorrect	0.00	
100			
1100			

#####Question 7
The gamma code for the term frequency of a certain document is 1110010. What is the term frequency of the document?
Your Answer		Score	Explanation
11			
10			
12			
9	Inorrect	0.00	

#####Question 8
When using an inverted index for scoring documents for queries, a shorter query always uses fewer score accumulators than a longer query.
Your Answer		Score	Explanation
True	Inorrect	0.00	
False			

#####Question 9
Can a retrieval system have an F1 score of 0.75 and a precision of 0.5?
Your Answer		Score	Explanation
No	Correct	1.00	
Yes			

#####Question 10
For any ranked list of search results, precision at 10 documents is always higher than precision at 20 documents.
Your Answer		Score	Explanation
False	Correct	1.00	
True
