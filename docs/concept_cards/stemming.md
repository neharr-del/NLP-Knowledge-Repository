Definition:

The process of stemming involves breaking up the word into its most fundamental form known as “stem.” In some cases, the result of this process may not be a proper English word even though it helps in categorizing similar words.
For instance, “playing,” “played,” and “plays” will be stemmed to “play.”
Unlike lemmatization, stemming disregards the meaning and grammatical structure of the word.


Why is it Needed? 

However, it is necessary to state that in the case of NLP applications, the usage of different variations of the same word means the same. The use of variations of words as separate lexical units will increase the number of such units and make it difficult to analyze the text.
The benefits obtained through the use of the Stemming technique include the following:
Vocabulary reduction;<br>
Improvement of the search accuracy;<br>
Speed;<br>
Word clustering.<br>
The efficiency of the technique may be observed in those situations when speed prevails over accuracy.


Working Principle: 

Stemming algorithm involves removing prefixes and suffixes that are common by following some pre-defined rules.
These are the general steps involved: <br>
Read each word.<br>
Recognize the common suffix like –ing, –ed, –ly, or –s.<br>
Remove the suffix.<br>
Return the stem.<br>

Some common stemming algorithms are:
Porter Stemming Algorithm
Snowball Stemming Algorithm
Lancaster Stemming Algorithm


Example :

Input Text
 playing
played
player
plays

Output 
play
play
play
play


Advantages:

An extraordinarily efficient technique.
It is very useful for compressing the document.
Very effective in finding words from the document.
An extraordinarily simple technique to use.


Limitations: 

Generating new words through combination of words from an English dictionary.
There are no considerations for grammar and context.


Real-world Applications: 

Search Engines
Information Retrieval
Document Clustering
Spam Filtering
Text Classification
Search Suggestions


Python Example :

from nltk.stem import PorterStemmer
stemmer = PorterStem2mer()
words = ["playing", "played", "studies", "running"]
for word in words:
    print(word, "→", stemmer.stem(word))


Output 

playing → play
played → play
studies → study
running → run


Diagram:
Input Words

playing
played
plays

      │
      ▼

Porter Stemmer

      │
      ▼

play
play
play


Summary: 
Stemming is a process where words are reduced by cutting off prefixes and suffixes to yield a basic stem. Even though the resultant stem may not always be an actual word, stemming increases efficiency and decreases vocabulary, hence its popularity in search engines.

