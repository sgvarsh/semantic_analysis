# semantic_analysis

## Difference between syntactical analysis vs semantical analysis in terms of ML

Syntactic Analysis : Syntactic Analysis of a sentence is the task of recognising a sentence and assigning a syntactic structure to it. These syntactic structures are assigned by the Context Free Grammar (mostly PCFG) using parsing algorithms like Cocke-Kasami-Younger (CKY), Earley algorithm, Chart Parser. They are represented in a tree structure. These parse trees serve an important intermediate stage of representation for semantic analysis.

Semantic Analysis : Intermediate meaning representations are composed for linguistic expressions. Mostly meaning representations are assigned to sentences solely on the basis of knowledge gained from the lexicon and the grammar, this approach is referred as syntax-driven semantic analysis. First Order Logic can also be used to represent a sentence in a language.

## How word2vec can bring semantical meaning to models

### Natural Language Processing 
NLP is an area of artificial intelligence focused on allowing computers to understand, process, and analyze human language. NLP is widely used in the tech industry, serving as a backbone to search engines, spam filters, language translation and much more. NLP enables computers to transform human language into a form that it can read and understand, such as a vector or discrete symbol. For example, NLP can take in the sentence So hungry, need food and break it down into four arbitrary symbols: so represented as K45, hungry as J83, need as Q67, and food as P21, all of which can then be processed by the computer. Each unique word is represented by a different symbol; however, the downside is that there is no apparent relationship between the symbols designated to hungry and food. This hinders the NLP model from using what it learned about hungry and applying it to food, which are semantically related. Vector Space Models (VSM) help address this issue by embedding the words in a vector space where similarly defined words are mapped near each other. This space is called a Word Embedding.

### Word2vec
Word2vec, a brainchild of a team of researchers led by Google’s Tomas Mikolov, is one of the most popular models used to create word embeddings. Word2vec has two primary methods of contextualizing words: the Continuous Bag-of-Words model (CBOW) and the Skip-Gram model, which i will summarize in this post. Both models arrive at a similar conclusion, but take nearly inverse paths to get there.

