### Comparing Speech and Text Classification of Native and Non-native English Speakers

#### This repository contains a dataset of speech and text features extracted from the International Corpus Network of Asian Learners of English ([ICNALE](http://language.sakura.ne.jp/icnale/)).

- only the extracted features are available; to get the full data, pleas visit the [official page](http://language.sakura.ne.jp/icnale/download.html)
- the dataset is extracted from speeches of students being asked to discuss the importance of having a part time job (PTJ)
- speech features are extracted using [openSMILE](http://opensmile.audeering.com/) based on the [INTERSPEECH 2010] (http://emotion-research.net/sigs/speech-sig/The%20INTERSPEECH%202010%20Paralinguistic%20Challenge.pdf) paralinguistic challenge
- to [download](https://github.com/senisioi/speech-text-features/releases/download/v1/ICNALE_features.tar.gz), check the release section

#### Description:
- the data is structured in libsvm format with files corresponding to each pair of native languages
- speech.ftrs and function_words.ftrs contain the features and the corresponding integer used in the libsvm representation
- the first line in each pair file is a [libsvm comment](http://www.csie.ntu.edu.tw/~cjlin/libsvm/faq.html#f306) of the form: *1 1:2 2:1 \# , LANG_1, LANG_2* that indicates the labels of the two native languages used

##### Speech:
- the speech files are split into 2 seconds chunks
- each class (native language) is represented by an equal number of chunks randomly sampled

##### Text:
- the text files are short ~110 words/file and used as they are
- except for lowercasing and tokenization, no preprocessing was done on these files

For more details about this particular dataset, mailto:sergiu nisioi  gmail dot com
