

######Question 1
```
Suppose a query has a total of 5 relevant documents in a collection of 100 documents. System A and System B have each retrieved 10 documents, and the relevance status of the ranked lists is shown below: 

	System A: [+ + - - - - - - - -]
	System B: [- + - - + - - - - +]

where the leftmost entry corresponds to the highest ranked document, and the rightmost entry corresponds to the lowest ranked document. A “+” indicates a relevant document and a “-” corresponds to a non-relevant one. For example, the top ranked document retrieved by System A is relevant whereas the top ranked one by B is non-relevant. 
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
The average precision is the sum of the precisions at each time a relevant document is retrieved divided by the total number of relevant documents. AP(A) = (1/1 + 2/2)/5 = 2/5 and AP(B) = (1/2 + 2/5 + 3/10)/5 = 6/25
