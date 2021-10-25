# Text mining of mental health support groups’ Reddit posts and text features during COVID-19

Stephanie Kyriakakis, Chenxi Liao, Anyi (Ash) Xu

## Topic and Data

**Description of the problem to be analyzed in the Shiny App**

We picked six mental health support groups: alcoholism, health anxiety, social anxiety, autism, 
loneliness and depression. The goal of this project is to apply text mining and NLP techniques 
on the analysis of text and text features of Reddit users from these mental health support 
groups, exploring the word embedding of various groups before and after COVID-19. 

**Proposed data sources**

Reddit Mental Health Dataset, which includes Reddit posts from 826,961 unique users from 2018 to 2020.
https://zenodo.org/record/3941387#.YVXAbW3ML0p

**Status of Literature Review**

Using NLP technique, Low et al. (2020) demonstrates that textual analysis is sensitive to 
uncover mental health complaints as they arise in real time, and shows that NLP features
could be a potential proxy for changes in mental health needs.
Machine learning models have been used to classify and characterize Reddit posts 
originating from mental health subreddits. Shen et al. (2017) achieved 98% accuracy
in separating posts on any of four different anxiety-related subreddits from posts on control 
subreddits. Hutto et al. (2014) proposed a novel model VADER for sentiment analysis of social media text. 
They got an encourageing result from VADER model on different datasets preparing to complex machine learning models, 
such as Support Vector Machine, Naive Bayes, and Maximum Entropy. VADER model is more quick and computationally economical,
easiler to be inspected and understood, and transferable to other domains. 

Hutto, C., & Gilbert, E. (2014). VADER: A Parsimonious Rule-Based Model for Sentiment Analysis of Social Media Text. 
Proceedings of the International AAAI Conference on Web and Social Media, 8(1), 216-225. 
Retrieved from https://ojs.aaai.org/index.php/ICWSM/article/view/14550

Low, D. M., Rumker, L., Talkar, T., Torous, J., Cecchi, G., & Ghosh, S. S. (2020, July 13). 
Natural language processing reveals vulnerable mental health support groups and heightened health anxiety 
on Reddit during COVID-19: an observational study. https://doi.org/10.31234/osf.io/xvwcy

Shen, J.H., Rudzicz, F. (2017). Detecting Anxiety through Reddit.Proceedings of the Fourth Workshop 
on Computational Linguistics and Clinical Psychology — From Linguistic Signal to Clinical Reality, 58–65


## Use Case
**Actor Description**

**Questions of Interest**

At this primary stage, we plan to use R to provide meaningful visualizations, such as t-SNE of wording embeddings and word clouds to assess anxiety, social anxiety, depression, autism and alcoholism before and during the Pandemic. We will compare changes across groups. In our later work, we will consider applying statistical machine learning methods to seek the possibility of using text features to predict what mental health groups future posts would fall into. 

**Fixed or Dynamic Data**

Fixed


## App Concept
**General Layout: (Multi page layout)**

Page 1- Dynamic word cloud for the 6 mental health groups chosen that allows users to pick 
any two categories and compare text patterns.

Page 2- t-SNE that allows the user to visualize the relationship between the mental health
groups. 

Page 3- Machine learning to predict specific mental health groups based on text features 
and allow users to pick any statistical method and to define the hyperparameters. 
(such as adjusting number of trees in random forest, and changing the penalty in
Logistic regression)

Page 4- Trend analysis of COVID-19 related words from December 2019 to August 2020.


**Proposed options for user data manipulations (if any)**

N/A

**Proposed options for user numerical/graphical analysis**

Based on user choice, we will provide t-SNE embeddings and 
word clouds. And we will also give users the ability to compare the visualization of word clouds
for any given two mental health support groups.

**Proposed options for user statistical models and tests**

We will allow users to compare the text feature statistics across various mental health support
groups, and compare the text feature statistics before and during the pandemic within a group.

**Proposed App Theme**

[Simplex theme](https://rstudio.github.io/shinythemes)


## Responsibilities
**Names and Responsibilities for the group members**

*Chenxi Liao*: Review the mental health NLP literature. Create statistical machine learning 
Models for the prediction of mental health groups using text related features. 

*Stephanie Kyriakakis*: Create code for the word cloud for the 5 mental health groups chosen
and host dynamic word clouds on the R Shiny app that allows users to compare groups. 
Create a vignette.

*Anyi Xu*:  Create code for  t-SNE for all 6 mental health groups and host on R Shiny app.


## Collaboration
**Approach to collaboration**

Zoom meeting every Tuesday at 2:30pm to 3:30 pm. 
A GroupMe channel was created for the discussion of ideas.
A Github repository will be created to track the progress of the project.


## Schedule
**Dates for Major Phases and Milestones**

| Date  | Description |
| ------------- | ------------- |
| 10/15/2021  | Gathering of Data  |
| 11/1/2021  | Literature Review  |
| 11/1/2021  | Create repository and host data  |
| 11/15/2021  | Data Preparation |
| 12/1/2021  | Create page 1 of R Shiny App (comparable word cloud for any 2 mental health groups) |
| 12/5/2021  | Create page 2 of R Shiny App (t-SNE embedding) | 
| 12/8/2021  | Create page 4 of R Shiny App (Trend analysis of COVID-19 related words for all groups) |
| 12/10/2021  | Create page 3 of R Shiny App (statistical machine learning models) |
| 12/12/2021  | Oral presentation run through |  
| 12/13/2021  | Produce the Vignette |  
| 12/13/2021  | Submission of  HTML file and .Rmd in a vignette folder on GitHub and note in Canvas |  
| 12/13/2021  | Submission of complete Repo on GitHub and note in Canvas | 

