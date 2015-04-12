####Task 1: Stopword Removal
```
cd ~/Desktop/meta/build/
./profile config.toml Assignment1/doc.txt --stop
cd ~/Desktop/meta/build/Assignment1/
python submit.py
```
####Task 2: Stemming
```
cd ~/Desktop/meta/build/
./profile config.toml Assignment1/doc.txt --stem
```
####Task 3: Part-of-Speech Tagging
```
cd ~/Desktop/meta/build/
./profile config.toml Assignment1/doc.txt --pos
```
####Optional: Writing a New Function
https://meta-toolkit.github.io/meta/doxygen/profile_8cpp.html

####Build the Search Engine
####Indexing
```
cd ~/Desktop/meta/build/
./index config.toml
```
####Searching
```
cd ~/Desktop/meta/build/
./interactive-search config.toml
```
####Task 4: BM25
```
cd ~/Desktop/meta/build/
./ranking-experiment config.toml task4
```
####Task 5: BM25 with tuned parameters
```
cd ~/Desktop/meta/build/
./ranking-experiment config.toml task5
```
####Task 6: PL2
```
cd meta/src/index/tools/
In ranking-experiment.cpp, insert the follwing codes:
```
```
double tfn = tf * log2(1 + c * avg_dl / doc_len);
double par_result1 = tfn * log2(tfn / lambda);
double par_result2 = (lambda + 1.0 / (12 * tfn) - tfn) * log2(exp(1));
double par_result3 = 1.0 / 2 * log2(2 * pi * tfn);
double par_result = par_result1 + par_result2 + par_result3;
double score = 1.0 / (tfn + 1) * par_result;
return score;
```
```
cd meta/build
make
```
Then, in config.toml, modify the following part:
```
[ranker]
#method = "bm25"  
#k1 = 1.2  
#b = 0.75  
#k3 = 500  
method = "pl2"  
c = 7  
lambda = 0.1  
```
```
cd meta/build/
./ranking-experiment config.toml task6
```

####Task 7: Tuning PL2
In ranking-experiment.cpp, modify the follwing codes:
```
maxmap = eval.map(); // Change 0 to the correct value
cmax = cvalues[i]; // Change 0 to the correct value
lambdamax = lambdavalues[j]; // Change 0 to the correct value
```
```
cd meta/build
make
./ranking-experiment config.toml task7
```
####Task 8: Relevance Judgments
```
cd ~/Desktop/meta/build/
./relevance-judgements config.toml
```
