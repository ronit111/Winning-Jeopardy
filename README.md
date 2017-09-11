# Winning-Jeopardy

Jeopardy is a popular TV show in the US where participants answer questions to win money. It's been running for a few decades, and is a major force in popular culture. If you need help at any point, you can consult our solution notebook here.

Let's say you want to compete on Jeopardy, and you're looking for any edge you can get to win. In this project, you'll work with a dataset of Jeopardy questions to figure out some patterns in the questions that could help you win.

The dataset is named jeopardy.csv, and contains 20000 rows from the beginning of a full dataset of Jeopardy questions. However, we are using only a sample out of this.

Each row in the dataset represents a single question on a single episode of Jeopardy. Here are explanations of each column:

Show Number -- the Jeopardy episode number of the show this question was in.
Air Date -- the date the episode aired.
Round -- the round of Jeopardy that the question was asked in. Jeopardy has several rounds as each episode progresses.
Category -- the category of the question.
Value -- the number of dollars answering the question correctly is worth.
Question -- the text of the question.
Answer -- the text of the answer.

Here are some potential next steps:

Find a better way to eliminate non-informative words than just removing words that are less than 6 characters long. Some ideas:
Manually create a list of words to remove, like the, than, etc.
Find a list of stopwords to remove.
Remove words that occur in more than a certain percentage (like 5%) of questions.
Perform the chi-squared test across more terms to see what terms have larger differences. This is hard to do currently because the code is slow, but here are some ideas:
Use the apply method to make the code that calculates frequencies more efficient.
Only select terms that have high frequencies across the dataset, and ignore the others.
Look more into the Category column and see if any interesting analysis can be done with it. Some ideas:
See which categories appear the most often.
Find the probability of each category appearing in each round.
Use the whole Jeopardy dataset (available here) instead of the subset we used in this mission.
Use phrases instead of single words when seeing if there's overlap between questions. Single words don't capture the whole context of the question well.
