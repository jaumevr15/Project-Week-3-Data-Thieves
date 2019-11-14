<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# A Brief Exploration of Porn Statistics
*[Maria Platas, Alieldin Ramadan, Jaume Vicens]*

*[November 2019 - Ironhack Barcelona]*

## Content
- [Project Description](#project-description)
- [Questions & Hypotheses](#questions-hypotheses)
- [Dataset](#dataset)
- [Database](#database)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

## Project Description
Porn is one of the most controversial elements in today's Internet. Known by most but openly admitted by a very few. Porn websites are source of huge, enormous databases of content, categories, users and algorithms that can be compared to the ones from most accessible sites like Youtube or Facebook. 

This umbrageous, but at the same time vast and interesting topic seemed perfect to be analyzed to have a better understanding of an unknown but still very big part the current consumption of internet.

We are currently halfway the completion of the Data Analytics Bootcamp, a 9-weeks full-time course where Python, SQL, Pandas and Tableau are covered, and these tools together make a difference when trying to analyze the available data.

## Questions & Hypotheses
We had a few questions we wanted to answer:
1. Which are the main categories, or tags used at porn sites?
2. Which are the most popular categories, and which ones have more content?
3. Which are the best rated categories?
4. Is there a correlation between the number of videos that a category has and the average views per video?

## Dataset
For this project, we used three different sources to get the most diverse and complete information possible:
Redtube Api [api.redtube.com] The official Redtube Api, which allowed a maximum of 30000 requests per day. 51901 rows of data.
Pornhub Database, csv file from Kaggle [www.kaggle.com], with 191532 rows of data.
Xhamster Database, csv file from Sexualitics [https://sexualitics.github.io/] with 785119 rows of data which we limited to 100000 for easy manipulation.
The information decided to use and manage is the following: [Video title]: Name of the video. [Number of views]: Accumulated amount of views per video. [Rating]: Average rating per video, from 0.0 to 1000 [Category 1]: Category or tag of the video. [Category 2]: Second category of the video. [Category 3]: Third category of the video. [Website]: Source of the video Either Redtube, Pornhub, Xhamster. A video has always a designated category [Category_1] but can also have others [Category_2] and [Category_3] which are optional. The original dataset varies from 1 to 20 categories in one video. We decided to limit it to three to standarize it.

## Database
We have decided to create one big table with the data. The information of the database contains the Categories, number of videos and average ratings.

## Workflow
We followed the following workflow:
1.- Decide topic (explore if feasible).
2.- Find datasets
3.- Clean Datasets
4.- Combine Dataset
5.- Upload them to Database
6.- Analyze Dataset
7.- Extraction of conclusions.

## Organization
In order to have our project organized we decided to use Trello, so that we took everything into account.
The repository is as follows:
     Main folder:
        .gitignore
        Kick-off
        you-project (folder):
            Paper.ipynb
            Best_practices.txt
            README.md
            code (folder):
                0_xhams_cleaning.ipynb
                1_DataCleaning_Pornhub.ipynb
                2_DataCleaning_Redtube_API.ipynb
                3_categories_cleaning_code.ipynb
                4_analysis.ipynb
            Charts (folder):
                0Top_10_bycat_bynumber_views
                1Cat_by_views
                2Mean_Views_related_Total_videos
                3Mean_Views_related_Total_videos_no_outliers
            databases (folder):
                    1_videos_combined_database.csv
                    2_combined_category.csv
                    
## Links
Links below:

[Repository](https://github.com/jaumevr15/Project-Week-3-Data-Thieves)  
[Slides](https://docs.google.com/presentation/d/1sF4Ao7nEZW3Pv4eE4LkACFA7GhjfwAfKBvuTK1jauVs/edit?usp=sharing)  
[Trello](https://trello.com/b/lh2KPMD9/project-3)  
