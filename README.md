# nltk-process
the very things about processing text with nltk from top to down

## code graph

```mermaid
flowchart TD
  A(url) -- url_scrapper.py --> E(raw_text);
  B(.txt file) -- read_file.py --> E(raw_text);
  C(.pdf file) -- textract.process --> E(raw_text);
  D(images) -- tesseract wrapper --> E(raw_text);
  E(raw_text) --> F[individual stopwords\ncommon stopwords];
  F --> G(filtered text);
  G -- tokenize_text.py --> H[tokens];
  H --> I(wordcloud);
  H --> J(unique_words);
  H --> K(most common collocations\naka n-grams);
  K --> L(single);
  K --> M(bigram);
  K --> N(trigram);
  K --> O(ngram);
```

### how to into mermaid grapsh
 - https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/
