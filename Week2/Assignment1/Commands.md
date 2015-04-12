#####Task 1: Stopword Removal

cd ~/Desktop/meta/build/
./profile config.toml Assignment1/doc.txt --stop

cd ~/Desktop/meta/build/Assignment1/
python submit.py

#####Task 2: Stemming
./profile config.toml Assignment1/doc.txt --stem

#####Task 3: Part-of-Speech Tagging
./profile config.toml Assignment1/doc.txt --pos

#####Optional: Writing a New Function
https://meta-toolkit.github.io/meta/doxygen/profile_8cpp.html

