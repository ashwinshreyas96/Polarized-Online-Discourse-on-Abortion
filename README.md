# Polarized-Online-Discourse-on-Abortion

GitHub Repository for the paper - Polarized Online Discourse on Abortion: Different Frames and Expressions of Hostility among Liberals and Conservatives. 
Tweet-ids corresponding to this analysis has been sourced from [#RoeOverturned: Twitter Dataset on the Abortion Rights Controversy](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/STU0J5). Owing to Twitter's policy we are restricted to sharing tweet-ids and users can rehydrate this dataset using [hydrator](https://github.com/DocNow/hydrator). Upon rehydrating the content place them in a .csv file under the data directory.

### Dependencies
Refer to requirements.txt

### Identifying Ideology

To generate embeddings you need to download the FastText Twitter bi-gram model from [Sent2Vec](https://drive.google.com/file/d/0B6VhzidiLvjSeHI4cmdQdXpTRHc/view) and place it in the models directory. Then you can run the Ideology_Detection.ipynb notebook.

### Identifying Hostile Expression

- To identify anger use the [SpanEmo classifier](https://github.com/hasanhuz/SpanEmo).
- To identify toxicity, obscenity and insults use the [Detoxify classifier](https://github.com/unitaryai/detoxify).
- To identify hate speech use the CardiffNLP's [Hate Speech classifier](https://github.com/cardiffnlp/tweeteval).

### Identifying Frames

- Run the Extract_Frame_Keywords.ipynb notebook to extract frame relevant keywords from Wikipedia articles under data directory.

### Analysis

- To replicate results of interrupted time series run the Interrupted_Time_Series.ipynb notebook.
- To replicate results of frame analysis run the Frame_Analysis.ipynb notebook.

