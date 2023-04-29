# Wiki-summary-to-speech
This Python script summarizes a given Wikipedia page and then converts the summary into an audio file.


## Installation
To use this notebook, you need to have Python 3 and the following libraries installed:

* transformers
* sentencepiece
* datasets
* wikipedia
* beautifulsoup4*
* num2words
* torch*
* soundfile*

*Already installed in Google Colab Notebook.


## Usage
The script can be executed by running the main.ipynb file, inputting the title of a Wikipedia page in the final cell of the notebook after the "Type the full title of a Wikipedia page: " message and pressing Enter.


## Functions
The script uses four main functions:

summarize_page(wiki_title)
This function takes a Wikipedia page title as input, generates a summary of the page, and returns a list of summaries for each section of the page.

parse_numbers(text)
This function takes a string of text as input, identifies any numbers and measurement abbreviations present in the text, and returns a new string with these numbers and measurements verbalized.

text2audio(text)
This function converts a given text into an audio file. The function uses a text-to-speech model to synthesize speech and a vocoder to convert the generated speech into an audio waveform.

merge_audio(list_of_text)
This function takes a list of strings as input, creates audio files for each string using the previous function, and merges these audio files into a single output file.


## License
This script is licensed under the MIT License.
