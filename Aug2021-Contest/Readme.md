# Aug 2021 - Contest 

The `resources` directory consists of 10 files (chapters) of Mahabharatham text in both English and Tamil translated version.The files are named similar except for the language codes (`en` for English and `ta` for Tamil).

## Task for the participants

* Pick any one set of chapters and sentence align the text between the English and Tamil versions
* From the Tamil version containing split sentences, generate the machine translated version of the sentences in English using the Open Source NLP library [IndicTrans](https://github.com/AI4Bharat/indicTrans) 
* Compute the BLEU score between each of the machine translated English sentences and the original English version using NLTK [BLEU Score Module](https://www.nltk.org/api/nltk.translate.html#module-nltk.translate.bleu_score)
* The final submission should be in the form of Python script that takes two `args` and generates the results in `output` folder in the same working directory

```
aug2021contest_<team name>.py <english_chapter_name.txt> <tamil_chapter_name.txt> 

```
`output` folder should contain following files:
* `sentence_aligned.txt` containing aligned sentences for the input files with each sentence separated by `|` (pipe) character and sentences are newline (\n) delimited 
* `machine_translated.txt` containing Tamil text and equivalent machine translated version separated by `|` (pipe) character with sentences newline (\n) delimited 
* `bleu_score.txt` containing average computed score for the translated version
 


