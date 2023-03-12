# Introduction-to-Data-Science

This repository contains three assignments for the Term 2 course: Introduction to Data Science. This ReadMe file will outline what you will find within these three assignments and go over the process taken to complete each. The code for these assignments is a mixture of code provided within the assignment notebook, code used in class, and code written by myself. 

Assignment 1 - Contribute to the library of missing datasets

For this assignment, we were tasked to consider an addition to Mimi Onuoha's "Missing Datasets" project. After many courses discussing data sovereignty, I became quite interested in those agencies which hold and use our data, and the power imbalances that creates. The first thing that came to mind was the infamous whistelblower case with Edward Snowden and the U.S. National Security Agency, which revealed that the NSA has illegally obtained and stored data from over a billion individuals world-wide. With this idea, I dove more into the Mimi Onuoha's work and began asking myself questions surrounding this proposed dataset, such as why does it not exist? How did the NSA do this in the first place? Will they stop? These questions led me down a path of research that turned into the paper submitted for this assignment. 


Assignment 2 - Regression Data Exploration Report

For this assignment, we were asked to pick a dataset with at least three numeric variables to be analyzed and fitted with various regression models to research the relationship between said variables. The dataset I have chosen for this is a list of the Top 100 most streamed songs on Spotify, taken from Kaggle. The link to this dataset can be found here: https://www.notion.so/Assignment-2-9107a937dcbc41fe96cb62a71b3a3c05?pvs=4#ad2e609104d047f5bf07238a6e526eea. This dataset includes a variety of attributes about each song, such as beats per minute, valance, danceability (all of which were analyzed for this project), among others such as loudness, length, acousticness, etc. 

I chose to study beats per minute (BPS) against danceability first, to see if tempo (BPS) had any relation to how easy the song was to dance to (danceability). My first step for this was to take a look at my dataset by pulling the minimums, maximums, medians, etc. for each. This gave a foundation for the times of information I would be looking at, and allowed me to pinpoint if there were any outliers that would need to be wrangled before continuing. I then worked through the notebook by plotting my variables against each other and reviewing the r and p scores of their relationship. 

After this, I added in a third independent variable: valance, to see the relationshio between valance (a measure of happiness), and beats per minute and danceability. To do this, I applied a Linear Regression model to the data and used that to see if I could use beats per minute and danceability to predict valance. I selected values which were in my dataset, to see whether the the predictions were accurate or not. For more analysis on these results, please refer to the jupyter notebook within this repository. 


Assignment 3 - Clustering with Numerical Datasets

The third and final assignment for Introduction to Data Science involved selecting a dataset with numeric values to use for clustering. The dataset selected for this was from Kaggle, and contains a series of attributes associated with sleep efficiency, such as bedtime, wake up time, deep sleep percentage, caffein consumption, etc. This dataset can be found here: https://www.kaggle.com/datasets/equilibriumm/sleep-efficiency. For the purpose of clustering, I was interested in looking at the relationship between caffeine consumption and sleep efficiency. 

My first step for this was to load in my dataset and review it to get a good idea of what type of data I would be working with. I then plotted sleep efficiency against caffeine consumption in a reduced dimensional plot to take an early peek at what, if any, clusters might exist within the data. I then continued working through the notebook used in class to apply a clustering model to the data, seeing the BIC scores, testing various n components and covariance types, and changing k values. All of this was to see how changing these values might affect the clusters, and in doing so, change how the data is perceived.

After doing this, I repeated the process using two new variables: deep sleep percentage against exercise frequency to determine if exercise frequency is relational to the amount of deep sleep an individual gets per night. Finally, I conducted the same process of reduced dimensionality and clustering, but on the whole dataset, minus the variables which were not numerical as those cannot be clustered.

To round out the project, I took a look back at caffeine consumption and sleep efficiency, plotting the data without dimensionality reductions or clustering to get a better idea of how the clustering understood the data. My last exercise for this assignment was to plot selections of the features within each cluster from the clustering done with sleep efficiency, caffeine consumption, deep sleep percentage, and exercise efficiency. Again, this was done to better visualize the relationships between the various variables and how they were clustered by the model. 

This concludes all assignments for this course. 
