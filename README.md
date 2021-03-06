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

```mermaid
graph TD;
    25some25-->0some0;
    4some4-->0some0;
    0some0-->4some4;
    0some0-->14some14;
    1some1-->6some6;
    21some21-->2some2;
    27some27-->2some2;
    2some2-->27some27;
    2some2-->26some26;
    8some8-->3some3;
    16some16-->3some3;
    3some3-->15some15;
    5some5-->25some25;
    6some6-->24some24;
    6some6-->21some21;
    20some20-->9some9;
    29some29-->9some9;
    9some9-->18some18;
    9some9-->10some10;
    13some13-->10some10;
    11some11-->10some10;
    10some10-->14some14;
    29some29-->11some11;
    14some14-->11some11;
    25some25-->11some11;
    16some16-->13some13;
    24some24-->13some13;
    25some25-->13some13;
    13some13-->28some28;
    13some13-->23some23;
    14some14-->25some25;
    14some14-->23some23;
    15some15-->26some26;
    15some15-->28some28;
    15some15-->27some27;
    16some16-->27some27;
    19some19-->26some26;
    19some19-->20some20;
```
