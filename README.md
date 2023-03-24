# BrandMeasures (NLP)

## Table of Content

  * Overview
  * Installation
  * Directory Tree
  * About Code and It's challages
  * Bug / Feature Request

## Overview
The code primarily focuses on 
        `audio-to-text conversion, text passed is to spell correction, and keyword extraction`.Why audio ? Now days there many surveys taken through audio, in those cases this will play a major role. However, it's important to note that this is just a part of the overall process of measuring the impact of a brand in the digital space. The impact of a brand can be measured in various ways, such as social media engagement metrics, website traffic, search engine rankings, sentiment analysis, and more. While the code you've seen may not directly measure these metrics, the extracted keywords and sentiment act as indicators of brand impact.

For example, if a particular brand is mentioned frequently and positively in online content, it can indicate a strong brand presence and positive impact. On the other hand, if a brand is mentioned frequently but with negative sentiment, it can indicate a need for brand reputation management.


## Installation
The Code is written in Python 3.6.10. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after the repository:
```bash
pip install -r requirements.txt
```
Basic UI to upload your audio file.

<img width="383" alt="Screenshot 2023-03-24 at 22 23 41" src="https://user-images.githubusercontent.com/45511185/227590482-13a20761-418a-4879-a46f-9313daf4f600.png">

## Important Directory Tree 
```
├── finaloutputsignal
│   ├── StoreDiarizedOutput.py
├── keywordspotter
│   ├── keywordSpotter.py
├── spellingcorrector
│   ├── spellcorrector.py
├── speech_to_text
│   ├── transcriptGenerator.py
├── test
├── clientService.py
├── pythonClientApp.py
```

## About Code and It's challages 

To build an STT engine (Speach to Text) we have many offline modules, in our case we have used SpeechRecognition and pydub. There are many API's provided by Azure,Google,AWS and IBM but they are not for free. An alternate choice of action would be buliding models inspring from model papers. In this we need to to Audio segmentation, we can achive through diffrent pocesses like chunking(used, voice separation or speaker diarization(allows searching audio by speaker). After collecting the above data we pass it through the SpellCorrector to validate our converted text(this is again like wrapper for sanity check). Finally we extract the key words from the conservation. From the key phrases in the text, we can infer the outcomes as described above, such as a high brand presence and favourable impact if a particular brand is frequently and favourably cited in online material. On the other hand, if a brand is frequently discussed but with negative connotations, it may be necessary to control its reputation.



## Bug / Feature Request

If you find a bug (the website couldn't handle the query and / or gave undesired results), kindly open an [issue](https://github.com/BHariKrishnaReddy/BrandMeasures/issues) here by including your search query and the expected result
