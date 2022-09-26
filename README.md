### Network structure and people’s attitude within work from home community on Reddit
MACS-36000 "Computational Methods Using Online Social Media Data" Final Project

Yujing Sun

Recording of my presentation is here: 

https://drive.google.com/file/d/1dbbpG7KyIzMndnle61wkRPRavPcMmwqs/view?usp=sharing
----------------------



The code is written in Python 3.8.8 and all of its dependencies can be installed by running the following in the terminal (with the `requirements.txt` file included in this repository):

```
pip install -r requirements.txt
```

## Step 1: Process the Data

- The files used to scrap the data from Reddit (`build_user_subreddit_history.py` and `download_subreddits.py`) are saved in folder `data`. 
- Use the `communities data download.ipynb` file to download all the subreddits from Reddit.  
- For the replication, you don't need to scrape the data again since it takes some time. The data is uploaded here: https://drive.google.com/drive/folders/1z8pn0voDqjsuH3MyAIsEwVf0M3pLPyWe?usp=sharing. You can directly download the folder.
- Covid-19 related data is downloaded by https://covid19.who.int/data. The data is in `WHO-COVID-19-global-data.csv`. I filter the raw data to get monthly new cases data `Covid-19 new cases.csv` that I will use in my analysis part.

## Step 2: Coding Replication

### Part 0: Replication preparation

- In order to rerun all the results smoothly, you should put `requirements.txt`, `new_data` folder (which could be downloaded by the google drive link), `Covid-19 new cases.csv`, `network analysis.ipynb`, `synchronic analysis.ipynb`, and `temporal analysis.ipynb` into same path.

### Part 1: Network analysis

- This part contains the following results: 
  -  All the results related with network analysis
- I write and run the `network analysis.ipynb` by google colab. The best way to replicate this part is run in the google colab. Since this part need to use the data in `new_data` folder, you can first save the folder on your google drive. 

### Part 2: Synchronic analysis

- This part contains the following results: 
  -  Topics of all the posts within WFH community. 
  -  Sentiment of each topic.
- The results of sentiment analysis and topic modeling are in `synchronic analysis.ipynb`. I run this part of code in local computer. 

### Part 3: Temporal analysis

- This part contains the following results: 
  -  Monthly sentiment rate, monthly posts number, and Covid-19 new cases. 
  -  Topic modeling for the posts by three seperate years. 
  -  Topic modeling for the posts by four different periods when post positive rate is high.
- The results of sentiment analysis and topic modeling are in `temporal analysis.ipynb`. I run this part of code in local computer. 
