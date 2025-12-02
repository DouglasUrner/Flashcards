# Flashcards Design Notes

- [Flashcards Design Notes](#flashcards-design-notes)
  - [Features](#features)
  - [To Do](#to-do)
  - [Card Object](#card-object)
    - [Word](#word)
    - [POS (part of speech)](#pos-part-of-speech)
    - [AuxiliaryData](#auxiliarydata)
      - [Noun](#noun)
      - [Verb](#verb)

## Features

- Design is intended to support multiple target languages & multiple "home" languages.
- Easy to change out card presentation strategy
- Practice cues:
  - Target language
  - Home language
  - Image
  - Dictation:
    - Single word
    - Phrase/sentence
  - Alternate forms (e.g., perfectum)
  - Prepositions
  - Articles

## To Do

Work out the design for:

- Tagging words (grouping words related to a particular topic). Allow multiple tags.
- Stats (used to drive presentation algorithm(s) and/or judge how well learned the word is).
- Date added (for interest and to allow recent words to be presented).
- Import/export
- Antonyms, synonyms, related words (e.g., plaats, plek, oord; or poes, kat)
- Conjugation / alternate forms

## Card Object

- Card
  - Word
  - Stats

### Word

- POS (part of speech)
- Word
- AuxiliaryData
- Image (image for prompting)
- Pronunciation (audio file of the word pronounced "correctly")
- Examples[]: Example (audio file of the word in "real life")
- Translations[]: Translation (the word translated into another language)

### POS (part of speech)

The part of speech along with "subparts" e.g., the past perfect of a verb.

- Language (assuming that there may be different parts of speech in different languages)
- Short name (e.g., N for noun)
- Long name
- Description

### AuxiliaryData

Per part of speech & per language.

#### Noun

- Language
- Article

#### Verb

- Language
- Regular/Irregular
- Preposition
