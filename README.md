
# Summary
In this project I will fetch data about NFL positional spending to see if it can be used within models to predict the number of games a team will win or to classify the team as good, bad, or mediocre.  The task at hand is to use regression and classification models to gain information on how to create the optimal NFL team.

# Goals

The goal for NFL teams is simple: win games, but the question is, how do they do that? Teams need need to decide how much money to allocate to each position so that they have the best chance to win. The first goal of the project will be to predict the number of games a team will win based on the salary numbers they are paying. With these results, we will be able to suggest to teams a percentage of their cap space that they should be spending on each position for the optimal team. Second, we anticipate there being more than one team strategy for success. So, we will classify a good team as one with 10+ wins, mediocre as 7-9 wins, and bad as 0-6 wins. From this we will use machine learning techniques to predict a classification based on the way the team allocates their money. With this, there could be multiple strategies found; for example, a team may find success in spending a significant amount on a quarterback and wide receivers, and another team may find success by allocating a significant amount to a running back and offensive line. Ultimately, we will create a way for NFL front offices to see their optimal path to success while also giving them projections of where the team stands as is.

# Motivation and Background

The National Football League is just as much a business as Microsoft, Apple, and every other for profit company. In the NFL, each team’s front office works to put their product on the field: a football team. Just like any other business, the company is only as good as its product and so every organization within the NFL wants to put together the best team possible with the measurement of success being the number of wins accumulated by the end of the season. With a good team, more money is made in many ways such as merchandise, ticket sales, earnings from any playoff games, and more. The goal for every business it to make as much money as possible and generally the better the team is, the more wins they earn, the more money the team will make. There are many approaches to putting together a winning football team and many parts that go into it for each of the 32 teams all with the same goal. For this project, the focus will be put on the allocation of money to the players, by position, within the reigns of the salary cap.

# Data Description
You may create a yelp account here: [Yelp Developer Page](https://www.yelp.com/developers).  And once an account is created, create an app.  Once the app is created, from the manage app page there will be a Client ID and API key.  Put the Client Id in a 'auth' section of the secret.cfg file, and the API key in the 'token' section of the same file - further described in the technical report.

I created a list of categories that I believed would be interesting to college students.  The reason I spent the time going through all these groups rather than just simply seraching for terms like 'food' or 'fun' is because of a limitation with the yelp API.  For any one particular query, a maximum of 1,000 businesses may be obtained with it (offset cannot be used above 1,000) and so with breaking the calls down to more specific categories, that minimizes the number of calls that return a number of businesses greater than 1,000 which results in more data for us both in numbers and of higher quality as less is missing.

Looping through and querying for each category, I ended up with 8752 rows of data with 17 columns.  The API docs are available here: [Yelp API Docs](https://www.yelp.com/developers/documentation/v3/business_search).

# Summary of Files

**Data Source:**
<br>
[SpotTrac](https://www.spotrac.com/nfl/positional/breakdown/2019/)
[Over the Cap](https://overthecap.com/positional-spending/)


**Python Notebooks:**
<br>
[ML Data Analysis](https://github.com/zvance1/come-to-umbc/blob/master/notebooks/clean-and-explore.ipynb)
Note: Not all exploratory analysis made it into the final techincal report - only what I saw as most relevant.
<br>
[Technical Notebook](https://github.com/zvance1/come-to-umbc/blob/master/notebooks/technical-report.ipynb)

**Data Folder (all data in csv format, used in our final python notebooks):**
<br>
[Data](https://github.com/zvance1/come-to-umbc/tree/master/data)

**Data Visualizations Folder (all visualizations used in our final python notebook):**
<br>
[Data Visualizations](https://github.com/zvance1/come-to-umbc/tree/master/images)

**Python Folder (python technical report notebook, and a notebook that fetches the data, and another for the exploration):**
<br>
[Python Files and Notebooks](https://github.com/zvance1/come-to-umbc/tree/master/notebooks)


# Project Info
<pre>
Contributors : <a href=https://github.com/zvance1>Zach Vance</a>
</pre>

<pre>
Languages    : Python3
Tools/IDE    : Anaconda, Jupyter Notebook
Libraries    : pandas, sklearn, matplotlib, numpy, seaborn
</pre>

<pre>
Duration     : September 2020
Last Update  : 10.08.2020
</pre>