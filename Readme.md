# Aug 2021 - Contest 

Setup:

Clone this repo into your github account

## Task for the participants (Preliminary Round)

Stage-0: Scraping Tamil and English Articles - Completed by us

We are using Kisari Mohan Ganguli's english translation of Mahabharatam and it's line by line tamil translation by Arul Selva Perarasan as sample data set of this exercise. The `resources` directory consists of 10 files (chapters) of Mahabharatham text in both English and Tamil translated version.The files are named similar except for the language codes (`en` for English and `ta` for Tamil).

Stage-1: Building Parallel Dataset

- Using python, split all the data into individual lines accurately such that each sentence in Tamil is aligned with English sentences.
  (Please note that Tamil version has additional context in brackets, additional texts which you can clean up and remove.)
- Push all the aligned sentences and script in a new folder called “data”.

Stage-2: Running a Neural Machine Translation Model

- In this stage, you will have to translate all the Tamil sentences you created in the previous stage to get the machine-translated English sentences.
- You can use this latest open source model on Google Colab platform: https://github.com/AI4Bharat/indicTrans#using-the-model-for-translating-any-input
- After you translate all the Tamil sentences to English, upload the translated sentences in a new folder called “translations” in your repo

Stage-3: Computing the scores of translation

- You should now compute the accuracy of translation, by comparing the original English sentence and translated English sentence.
- Accuracy in translation is generally reported using a metric called BLEU score (although there are many other metrics available)
  - To compute BLEU scores, you can follow this tutorial: https://blog.machinetranslation.io/compute-bleu-score/
- Try to find out the overall BLEU score for all the 10 articles/stories that you scraped, and mention them in the README of your repo.
  - Also push your scripts in a folder called "evaluation"

Stage-4: (Bonus points) Compare the model with other services

- There is a free version of Google Translate (would not be as great as Google’s API) using which you can get the translations for the same Tamil sentences and calculate the accuracy of the service.
- You can use this library: https://github.com/UlionTse/translators
- Similarly to stage-5, mention the BLEU scores for the 10 articles in your repo’s README

## Submission

- Complete the task by the deadline and submit the shared Google form.
  - The form will close sharply by the mentioned deadline (Aug 22 11:59PM IST)
  - Early submissions are welcome
- For any doubts/clarifications regarding the contest, please go to the [_Issues_](https://github.com/venmurasu-programming-team/Aug2021-contest/issues) and raise your question
  (without posting your code or implementation details)
- Please document your strategy of implementation in detail in the repo's README
- Results would be announced within a week after the deadline, and shortlisted candidates would proceed to the final round.

## Selection

Winners will be selected based on the following critieria:
* Completion of the task ( weightage - 10% )
* Quality of sentence alignment ( weightage - 20% )
* Machine translation ( weightage - 30% )
* BLEU score computation ( weightage - 20% )
* Code quality and documentation (weightage - 20% )
