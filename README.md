thesis_data_set
===============

A data set consisting of 71.386 sentences from 378 Danish legal rulings by the Danish Companies Appeals Board [http://www.erhvervsankenævnet.dk], which has been pre-processed for use in my master's thesis - Data-driven de-identification of Danish legal rulings. 

The set has been sentence tokenized and a punkt tokenizer trained on a Danish corpus has been applied. The set has further been split into one word per line. A blank line serves as a sentence delimiter. Thus the set is suitable for use by sequential modeling algorithms such as HMM or CRF. I have been using CRF++ [http://crfpp.googlecode.com/svn/trunk/doc/index.html]. The data set can also easily be modified to be used for other data-driven purposes. Also for use by CRF++ is an aligned list of true answer tags. A TRUE tag indicates that a token has been de-identified from the original rulings.

To comply with Danish data protection laws, every token that was originally de-identified (person's names, company names etc.) have been obfuscated by replacing them with random words of a similar structure, e.g. "DaniCon" could be replaced by "FiskHus".

Finally enclosed are the feature sets used to conduct my experiments. These include token shapes, token affixes, token stemming, POS tags and Brown clustering.
