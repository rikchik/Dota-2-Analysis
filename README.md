# Dota 2 Analysis

Dota 2 is MOBA competitive online video game developed by valve. The data is acquired from [Kaggle](https://www.kaggle.com/datasets/devinanzelmo/dota-2-matches).

`cluster_region.csv` consists of all the regions where the servers are hosted.

`hero_names.csv` consists of all the heroes and their ids. In total there are about 110 heroes. 

`item_ids.csv` consists of all the items and their ids. 

`match.csv` consists of all the matches the data was collected for. Data was collected for a total of 50k games.

`patch_dates.csv` consists of all the patches that have been created upto 2017. 

`players.csv` consists data about all the players that played in these 50k games.

# Exploratory Data Analysis

Mainly involved joining the different csvs to generate insights about heroes, matches, regions and the patch itself. No missing data was found.

# Training and Predicting

Utilised `match.csv` and `players.csv` to find whether radiant team composition will win or dire team composition. 

A total of 110 heroes would have ended up creating a sparse matrix, so I made embeddings out of them to create a dense matrix. Utilised Logistic Regression, Random Forest, XG Boost, and Artificial Neural Networks.


Logistic Regression had the highest accuracy of about 60% on 20% of the dataset.

