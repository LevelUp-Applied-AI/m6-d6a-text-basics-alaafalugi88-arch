Setup
pip install -r requirements.txt
python -m spacy download en_core_web_sm

This installs spaCy and downloads the English language model required for processing text.

Tasks

Complete the three functions in drill.py:

preprocess_text(text, stop_words)
Process raw text using spaCy
Remove punctuation and whitespace
Convert tokens to lowercase
Filter out custom stop words
extract_linguistic_annotations(text)
Extract token-level annotations
Return tuples of:
(token_text, POS_tag, dependency_label)
extract_entities(text)
Use spaCy Named Entity Recognition (NER)
Return detected entities as:
(entity_text, entity_label)
What I implemented
Built a clean preprocessing pipeline for text normalization
Extracted linguistic features (POS + dependency parsing) for each token
Implemented Named Entity Recognition (NER) using spaCy
Fixed a bug in entity extraction to ensure all entities are returned (not just the first one)
How to Run
python drill.py

You should see:

Cleaned tokens output
Token-level linguistic annotations
Extracted named entities
Submission Steps

Create a branch:

git checkout -b drill-6a-text-basics
Complete drill.py

Push your branch:

git push --set-upstream origin drill-6a-text-basics
Open a Pull Request to main
Submit your PR link in:
TalentLMS → Module 6 Week A → Drill 6A