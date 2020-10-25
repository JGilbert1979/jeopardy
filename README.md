# Jeopardy

This repo utilizes data obtained from the following reddit subsite:
https://www.reddit.com/r/datasets/comments/1uyd0t/200000_jeopardy_questions_in_a_json_file/


The original data is a json file containing 216,930 Jeopardy questions, answers and other data obtained by crawling www.j-archive.com. 

I have formatted these data as a csv and compressed them into a zip for convenience. The schema is described below. 

According to j-archive, the total number of Jeopardy! questions over the show's span (at the time of collection) is 252,583 - so this is approximately 83% of them. In particular, around the last two years of game play are missing.


The csv file is an unordered list of questions where each question has:

•	'category' : the question category, e.g. "HISTORY"
•	'value' : $ value of the question as string, e.g. "$200"
Note: This is "None" for Final Jeopardy! and Tiebreaker questions
•	'question' : text of question
Note: This sometimes contains hyperlinks and other things messy text such as when there's a picture or video question
•	'answer' : text of answer
•	'round' : one of "Jeopardy!","Double Jeopardy!","Final Jeopardy!" or "Tiebreaker"
Note: Tiebreaker questions do happen but they're very rare (like once every 20 years)
•	'show_number' : string of show number, e.g '4680'
•	'air_date' : the show air date in format YYYY-MM-DD


See the Jeopardy.docx for additional descriptive statistics and information concerning the text portions of this dataset.