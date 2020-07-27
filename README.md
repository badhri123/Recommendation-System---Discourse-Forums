# MLTeam5
This is the GitHub Repository for the STEM-Away Machine Learning internship programs team 5.

# Instructions on execution

1) Run ForumCrawler.py 

This script would fetch the links of all topics and store it as a pickle file.

2) Run ForumScraper.py

This script would fetch the text data inside each URL and stores it as a pickle file.

3) Run Recommendation_Model.ipynb

Once the text_submissions.pickle is available, the above script uses that to create a dataset of forum text submissions and then uses 3 approaches of Recommendation.
First, it uses a pre-trained BERT model to obtain sentence embeddings of the all forum submissions. Then, uses them to obtain closest submissions to a given input text.
Second approach is using TF-IDF, a statistical approach based on how important a word is in a document. Similar to the first approach, the embeddings are obtained and the recommendation is done using cosine-similairty metric. Finally, a combination of BERT and TF-IDF is carried out. For all the three approaches, Jaccard similarity is used to evaluate the performance.
