####Task 1: Stopword Removal

cd ~/Desktop/meta/build/

./profile config.toml Assignment1/doc.txt --stop

cd ~/Desktop/meta/build/Assignment1/

python submit.py

####Task 2: Stemming
cd ~/Desktop/meta/build/

./profile config.toml Assignment1/doc.txt --stem

####Task 3: Part-of-Speech Tagging
cd ~/Desktop/meta/build/

./profile config.toml Assignment1/doc.txt --pos

####Optional: Writing a New Function
https://meta-toolkit.github.io/meta/doxygen/profile_8cpp.html

####Build the Search Engine
####Indexing
cd ~/Desktop/meta/build/

./index config.toml

####Searching
cd ~/Desktop/meta/build/

./interactive-search config.toml

####Task 4: BM25
cd ~/Desktop/meta/build/

./ranking-experiment config.toml task4



