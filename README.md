# Automatic Phrase Variation Generator

## Overview
This project generates meaningful paraphrases of Spanish sentences by identifying key components such as verbs, nouns, and prepositions. It then translates them into English and generates variations using the Parrot paraphrasing model. This process allows for flexible sentence generation without manually specifying variations for each word.

## Features
- Automatically extracts key words (verbs, nouns, prepositions) from input phrases.
- Translates the phrase to English using Google Translate.
- Generates multiple variations of the translated phrase using Parrot.
- Translates the generated variations back to Spanish.
- Provides diverse paraphrases without manual intervention.

## Why is this useful?
- Helps in language learning by providing multiple ways to express the same idea.
- Useful for natural language processing (NLP) applications.
- Can be adapted for chatbot responses, text augmentation, or content rewriting.

## Requirements
Make sure you have the following installed:
- Python 3.7+
- `googletrans` for translation
- `spacy` for natural language processing
- `Parrot` model for paraphrasing

Install dependencies using:
```bash
pip install googletrans==4.0.0-rc1 spacy torch parrot
```
Additionally, download the Spanish language model for `spaCy`:
```bash
python -m spacy download es_core_news_sm
```

## Usage
### Running the Example (Google Colab)
To test the implementation, you can run the provided example in Google Colab:
1. Upload the script to Google Colab.
2. Install dependencies using the commands above.
3. Run the script and input a Spanish sentence.
4. The program will generate multiple variations of the phrase automatically.

Example input:
```python
frase_es = "Quiero reservar un vuelo a Nueva York el próximo sábado."
```
Example output:
```
1. Quiero reservar un vuelo a Nueva York el próximo domingo.
2. Quiero reservar un vuelo a Nueva York el próximo sábado.
3. Quiero reservar un ticket a Nueva York el próximo sábado.
4. Quiero reservar un vuelo a Nueva York el próximo viernes.
5. Quiero hacer una reserva para un vuelo a Nueva York el próximo sábado.
```

## Notes
- The example uses **Google Colab** for testing, but it can be run locally as well.
- The quality of paraphrasing depends on the Parrot model and Google Translate.

## Future Improvements
- Improve word identification to refine paraphrase quality.
- Support more languages for input and output.
- Allow customization of the variation generation process.

