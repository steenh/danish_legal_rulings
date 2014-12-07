thesis_data_set
===============

This repository contains a data set consisting of Danish legal rulings from the Danish Companies Appeals Board, which I have parepared for use in my thesis - Data-driven de-identification of Danish legal Rulings. 

The set has been split into one word per line. A blank line serves as a sentence delimiter. Thus the set is suitable for use by CRF++ [http://crfpp.googlecode.com/svn/trunk/doc/index.html], but can also easily be modified to be used for other machine learning purposes.

Also for use by CRF++ is an aligned list of true answer tags. These tags indicates which words have been de-identified from the original rulings. To comply with Danish data protection laws, the original words (person's names, company names etc.) have been obfuscated by replacing them with random words of a similar structure. Repeated words are of course replaced by the same obfuscated words.

Finally I have included the feature sets which I have used to conduct my experiments.
