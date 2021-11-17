# Machines, Writing, and R.A. Lafferty
The project is training a machine learning model (or models) to write like the inimitable sci-fi author R.A. Lafferty. 

## Introduction
I did not know who R.A. Lafferty was until earlier this year. While searching for my next sci-fi read, I came across a [Wired article](https://www.wired.com/story/who-is-r-a-lafferty-best-sci-fi-writer-ever/) with the headline: _Who is R.A. Lafferty Lafferty? And is He the Best Sci-Fi Writer Ever?_ But it was the subheading that grabbed me: _You’ve never heard of him, but your favorite writers have, and_ **_his mad-drunk prose will knock you sideways_**_._ “Mad-drunk prose, eh?” I remember thinking “Count me in!”

How does machine learning fit into all this? I’d been wanting to tackle a natural language processing project, and Lafferty’s “mad” prose has been buzzing around, demanding more attention from my fickle brain. “So, let’s kill two birds with one project,” I thought. 

## Methods and models

Two models were used in this project: RNN (via Keras/TensorFlow) and Markov (via Markovify). 

The notebooks in the /code folder are labeled in order of process. 
 - Extracting text from PDFs | **01_extraction_vision_api_clean.ipynb**
 - Combing text files into single file | **02_text_combine.ipynb**
 - EDA and exploring/visualizing data | **03_eda_visualization.ipynb**
 - Generating text with an RNN model | **04_text_generation_RNN_character.ipynb**
 - Generating text with Markov chains | **05_markov_chains**

## Data
I used a [Google sheet](https://docs.google.com/spreadsheets/d/1RMD_tBTUihWwJuByUOIqBEL6mFQ3EdC6VFhK4wpoc_4/edit?usp=sharing) to keep track of the progress I'd made in finding the author's works. 

- The original PDFs of Lafferty's works are located in **/data/pdf**
- The extracted text files are located in **/data/txt**
- The compiled text file is located in **/data**
- The text files for Isaac Asimov and Philip K Dick are also located in **/data/txt**

A PDF copy of the presentation for this project is saved as **lafferty_presentation.pdf** and can be found in the main directory.

### Sources and credits
- [Who is R.A. Lafferty Lafferty? And is He the Best Sci-Fi Writer Ever?](https://medium.com/r?url=https%3A%2F%2Fwww.wired.com%2Fstory%2Fwho-is-r-a-lafferty-best-sci-fi-writer-ever%2F) by Jason Kehe (Wired)
- [How to Extract the Text from PDFs Using Python and the Google Cloud Vision API](https://towardsdatascience.com/how-to-extract-the-text-from-pdfs-using-python-and-the-google-cloud-vision-api-7a0a798adc13) by Silvia Zeamer (Medium)
- Shoutout to Caroline Schmidt for help with coding the text extraction
- [Text Generation with an RNN](https://www.tensorflow.org/text/tutorials/text_generation) from TensorFlow
- [Markovify](https://github.com/jsvine/markovify) by Jeremy Singer-Vine
- [spaCy 101: Everything You Need to Know](https://spacy.io/usage/spacy-101) from Spacy
