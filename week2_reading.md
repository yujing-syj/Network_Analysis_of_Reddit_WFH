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

## Key Findings:

![image](https://user-images.githubusercontent.com/89925326/194399703-5e0955e5-eeb9-4062-aad3-7a6da36ac684.png)
![image](https://user-images.githubusercontent.com/89925326/194399776-37ba0616-9864-4fd7-8df2-542194ab3a22.png)
![image](https://user-images.githubusercontent.com/89925326/194399815-390e3a74-d2b5-4636-955e-c602308c8894.png)
![image](https://user-images.githubusercontent.com/89925326/194399866-8233ee73-8dd1-43df-8a9d-0cd09f037929.png)
![image](https://user-images.githubusercontent.com/89925326/194399928-c472664f-8db6-41de-8407-f92ddf8094c2.png)
![image](https://user-images.githubusercontent.com/89925326/194399974-b10361b5-89ea-476d-ac04-cedb548d5584.png)
![image](https://user-images.githubusercontent.com/89925326/194400037-d6fb7632-cb12-4fc0-a419-05e6e82a02f3.png)
![image](https://user-images.githubusercontent.com/89925326/194400096-72451812-7234-4fc2-9cc7-ee5d3f6849fb.png)
![image](https://user-images.githubusercontent.com/89925326/194400141-f078ec33-dbb3-45af-8617-731c83e0f4e2.png)
![image](https://user-images.githubusercontent.com/89925326/194400168-98bc3de2-b86c-47bb-9dc7-bf934f5061c9.png)
