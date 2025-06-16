# DASC5300 Assignment 3

This assignment focuses on leveraging MySQL for disk-based analysis. You will import a large dataset into a MySQL database and conduct a series of queries to extract meaningful insights.

# Objectives

- Import the data into a MySQL database
- Analysis using simple queries
- Analysis using complex queries

# Dataset

The dataset is a subset of the Stack Overflow data dump from 2008 to 2010. I have already imported the data into a MySQL database. The file is available on Canvas.

# User Selection

Using your student ID, set the seed on `np.random`. There are 299,397 users in the dataset. Use the `np.random.randint` function to select 4200 users.

# (40 points) Becoming Familair with the Data

For the first part of the assignment, you should familiarize yourself with the schema of the dataset so that you can write correct queries. For each of the questions below, you should provide the query that you used to answer the question along with a description of the query.

- How many questions are in your subset of the data?
- How many answers are in your subset of the data?
- What is the most popular tag in your subset of the data?
- What is the average reputation of users in your subset of the data?
- How many unanswered questions are in your subset of the data?

# (40 points) Analysis

For the second part of the assignment, you will conduct a series of analyses using the dataset. For each of the questions below, you should provide the query that you used to answer the question along with a description of the query. You should also provide a visualization of the results where applicable. You can use any visualization library that you would like, and the quality of your visualizations will be considered in your grade.

## Questions and Answers

Many users come to StackOverflow to get help on their programming questions. Fewer users come to the site to answer questions. In this section, you will analyze the questions and answers in your subset of the data to answer the question: **What percentage of users are actively answering questions versus asking them?**

There are many valid ways to answer this question. Your solution to this should include three core parts.

1. You should define what it means to be an "active" user. For example, you could define an active user as a user that has asked or answered at least 10 questions.
2. You should provide a query that returns the number of active users and the total number of users in your subset.
3. You should provide a visualization that shows the percentage of active users versus total users.

## Popularity of Tags over Time

Trends come and go in the programming world. In this section, you will analyze the popularity of tags over time to answer the question: **What are the most popular tags over time?** Since the dataset only spans 2 years, you will need to aggregate the data by month. You should provide a visualization that shows the popularity of tags over time.

1. What are the most popular tags for each month (this should provide you with 24 data points)?
2. Visualize the tags over time using a plot.

## User Reputation Growth

In this section, you will analyze the growth of user reputation to answer the question: **What are the top 10 users that experience the fastest growth in reputation?** You can define whatever time frame you think is necessary to determine growth rate. You could show the top 10 users based on growth for each month or the top 10 fastest growing users across any 1 month time span. Whatever you choose to do for your analysis, make sure you provide your rationale, query, and visualization.

## Hot Questions

In this section you should provide answers to the following questions.

1. What are the top 20 questions that have the most answers?
2. Of those top 20, how many answers were provided by users in your subset?
3. How do the tags associated with the top 20 questions compare to the most popular tags?

# (20 points) Report

In your notebook file, each section of code should be preceded by a text cell that describes what the code is doing. The code should be formatted cleanly and easy to read.