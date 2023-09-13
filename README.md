# This machine learning final project focuses on training a chosen dataset from a Google research dataset. The chosen dataset is called “Google Well-formed Query Dataset” and it is a dataset resulted from crowdsourcing well-formedness annotations for 25,100 queries from Paralex corpus. Every query sentence was annotated by five raters with a rating 1/0 of whether or not the query is well-formed, i.e, grammatically correct. There are three datasets given that have been split into train.tsv, test.tsv, and dev.tsv. We can see a snippet of the dataset: 

Query	Well-formedness rating
Which form of government is still in place in greece ?	1.0
Population of owls just in north america ?	0.0
Is johnny depp a celtic fan ?	0.8
Where did Roald Dahl live in his teenaged years ?	0.6

The snippet of the query shows where a sentence is gramatically correct, and explicit question, and if it contains any spelling errors. The score scaling of 0 to 1 is given with 1 being the most well-formed and 0 being the least. 
To train those datasets, a language model that understands English language, is able to connect the context of the question from the start to end, and produce rating based on how the query is well-formed must be used. 
Transformer models fit the requirements as they can understand sequence of words in a sentence and a little bit of fine-tuning to the model would yield results with great accuracy. 
