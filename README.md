# Topic-Modelling-On-Jeopardy-Questions-LDA
## Goal

The goal of this porject is to analyze topics of the questions asked in the game show Jeopardy! based on the year, round and the monetary value of the questions using the Latent Dirichlet Allocation (LDA) model. LDA an unsupervised generative statistical machine learning model that views documents(questions in this case) as bags of words. 

Topic modeling will performed on these questions to analyze two main things:
#### 1. Game Dynamics : 
Jeopardy!has been around for a long time (from 1984-2020) and one goal of this analysis is to explore how thematic topics covered in the game’s questions have changed over 35 years. 
#### 2. Question Difficulty :
Monetary  value  acts  as  a  proxy  for  the  difficulty  of  the  questions  asked  in Jeopardy!.Through our analysis we will explore what aspects of the  questions make them more difficult. And,tying this to the above, how have these trends changed over time?

## Dataset
The dataset used for this project is available on Reddit- [Jeopardy! Questions Dataset](https://www.reddit.com/r/datasets/comments/1uyd0t/200000_jeopardy_questions_in_a_json_file/) . The dataset has 216,930 questions asked on the show between the year 1984 - 2012 and during different rounds levels through the show. For this project we will only be using the questions asked during the Jeopardy!, Double Jeopardy!, and Final Jeopardy! rounds.

## Steps for Modeling
1. Clean the text of the questions
2. Use TFIDF vectorizer to vectorize the data
3. Use LDA model to get the top 5 topics with highest probability.
4. Find top 10 words for each topic
5. For each question, find the probability that a question belongs to a topic; assign the question to the topic that has highest probabilty 
6. Visualize the words in each topic and the distribution of questions in each topic
