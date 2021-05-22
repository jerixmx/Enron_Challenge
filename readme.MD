# sfor
---
## Scope
sfor is a Python script made specifically for searching through email documents in the Enron Corpus. It employs a record-level index and excludes stopwords from the NLTK Stopwords Corpus<sup>1</sup>.

## Features
It can search for multiple terms and match ANY or ALL of the search terms.

It will index/reindex/load index depending on whether index file (`i_index.txt`) exists within the search directory and whether files in the search directory have been updated since last indexing.

## Usage
Keep `sfor` and `nltk-stopwords.txt` in the same directory.

Syntax:
`./sfor <term1> <term2> ... <termn> -d <path/to/search> [-a]`

By default, sfor will look for matches to ANY of the search terms. To return only results that match ALL terms, use `-a`.

## Demo
A demo gif is available but not linked to this readme due to flashes while rendering.

---
<sup>1</sup>NLTK Stopwords Corpus used is obtained from [NLTK.org](https://www.nltk.org/nltk_data/).
