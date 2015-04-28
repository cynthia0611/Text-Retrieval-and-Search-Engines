

######Question 1
```
Suppose a query has a total of 5 relevant documents in a collection of 100 documents. 
System A and System B have each retrieved 10 documents, 
and the relevance status of the ranked lists is shown below: 

	System A: [+ + - - - - - - - -]
	System B: [- + - - + - - - - +]

where the leftmost entry corresponds to the highest ranked document, 
and the rightmost entry corresponds to the lowest ranked document. 
A “+” indicates a relevant document and a “-” corresponds to a non-relevant one. 
For example, the top ranked document retrieved by System A is relevant whereas the top ranked one by B is non-relevant. 
```
What is the precision at 10 documents of both systems?

P(A) = 2/10 	P(B)= 3/10	Correct	1.00	
P(A) = 2/100 	P(B)= 3/100			
P(A) = 2/5 	P(B)= 3/5			
P(A) = 8/100 	P(B)= 7/100

######Question 2
```
Assume the same scenario as in Question 1. What is the recall of both systems?
```
R(A) = 8/100 	R(B)= 7/100			
R(A) = 2/5 	R(B)= 3/5			
R(A) = 2/10 	R(B)= 3/10		
R(A) = 2/100 	R(B)= 3/100


######Question 3
```
Assume the same scenario as in Question 1. What is the average precision of both systems?
```
AP(A) = 2/5 	AP(B) = 6/25			
AP(A) = 2/100 	AP(B) = 3/250			
AP(A) = 3/10 	AP(B) = 9/20			
AP(A) = 2/10 	AP(B) = 3/25

> The average precision is the sum of the precisions at each time a relevant document is retrieved divided by the total number of relevant documents. AP(A) = (1/1 + 2/2)/5 = 2/5 and AP(B) = (1/2 + 2/5 + 3/10)/5 = 6/25

######Question 4
```
Let w1, w2, and w3 represent three words in the dictionary of an inverted index. 
Suppose we have the following document frequency distribution: 
```
Word	Document Frequency
w1	1
w2	5
w3	10

Assume that each posting entry of document ID and term frequency takes exactly the same disk space. Which word's postings list will occupy the largest disk space?

w2			
w3		
w1
> The postings list of w3 has the largest number of entries, and thus occupies the largest space.

######Question 5

> Assume we have the same scenario as in Question 4. If we enter a query Q= “w1 w2 w3” then the maximum possible number of accumulators needed to score all the matching documents is:

1			
16	
10			
5
