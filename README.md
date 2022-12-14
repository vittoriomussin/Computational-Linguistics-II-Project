# Computational-Linguistics-II-Project

Objective:
- Construction of a gold corpus to evaluate the accuracy of
analysis of an automatic linguistic annotation chain

Work phases:
1. Automatic annotation of a textual corpus
2. Manual review of automatic annotation
3. Verification of agreement between two manual reviewers
4. Use of the manually reviewed corpus for the validation of automatic analysis using 2 UDPipe models (ISDT & PoSTWITA)
trained on two different varieties of the Italian language


## Corpus Structure

|  | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **Size** (in characters) | 3.164  | 3.031  | 3.112  | 3.448 | 3.378  |
| **Year**  | 1907  | 1927  | 1947  | 1969  | 2009  |


## Validation Results

### ISDT
| F1-Measure | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **UPOS** | 94.74  | 97.44  | 90.56  | 96.28 | 96.31  |
| **XPOS**  | 94.74  | 96.08 | 89.47  | 96.61  | 96.46  |
| **UFeats**  | 93.20 |97.44 |89.78   | 97.42| 98.15  |
| **Lemmas**  | 91.34 |95.22 |90.09  | 98.71| 95.54   |
| **UAS**  | 84.70 |89.59 |78.79  | 87.88 |88.15  |
| **LAS**  | 78.05| 82.42 |70.43 | 84.65 | 85.08  |
| **BLEX**  | 58.66 |67.19 |50.14  |76.73 |72.49 |
| **Year**  | **1907**  | **1927**  | **1947**  | **1969**  | **2009**  |
### PoSTWITA
| F1-Measure | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **UPOS** | 87.48 |90.44 |89.63  | 91.28 |87.54  |
| **XPOS**  | 86.09| 89.08| 86.69   | 90.31 |86.77  |
| **UFeats**  | 83.62| 87.71 |86.22 | 90.63 |88.77 |
| **Lemmas**  | 86.40 |88.91 |83.90 | 90.31 |86.62 |
| **UAS**  | 76.82 |75.26 |76.16 |75.44 |70.77 |
| **LAS**  | 67.23| 67.06| 65.63 | 70.60 |63.85 |
| **BLEX**  | 47.38 |47.72 |42.05 |55.44 |45.95 |
| **Year**  | **1907**  | **1927**  | **1947**  | **1969**  | **2009**  |

## Interannotator Agreement Results

### Part Of Speech
|  | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **Average observed agreement** | 0.97  | 0.96  | 0.97  | 0.97 | 0.96  |
| **Cohen's kappa**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **Year**  | **1907**  | **1927**  | **1947**  | **1969**  | **2009**  |

### Dependency Reletions
|  | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **Average observed agreement** | 0.85  | 0.80  | 0.83  | 0.88  | 0.87  |
| **Cohen's kappa**  | 0.85  | 0.79  | 0.83  | 0.88  | 0.87  |
| **Year**  | **1907**  | **1927**  | **1947**  | **1969**  | **2009**  |

## Automatic Parsing Error Analysis

- **Sentence Splitting and Tokenization**

|  | Cooking Texts (in wich there are most of the clitics) |  |  |
| ------------- | ------------- | ------------- | ------------- |
| **correctly parsed clitics** | 44%  | 63%  | 33%  |
| **n?? of clitics**  | 36 | 8  | 18 |
| **Year**  | 1907  | 1927  | 1947  |

- **POS and dep**

|  | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **correctly parsed roots** | 90% | 96%  |74%  | 73% | 76%  |
| **n?? of sentences**  | 29  | 28  | 31  | 15  | 17  |
| **Year**  | 1907  | 1927  | 1947  | 1969  | 2009  |

> **Causes of error in root recognition**
> |  | Scorrect POS | Subordinates before root sentence | Nominal and Split sentences |
> | ------------- | ------------- | ------------- | ------------- |
> | **Cases** | 50%  | 15%  | 35%  |

### ISDT - Error Analysis (incorrect tag - correct tag)

> ### **POS**
> 
> Cooking Texts 
> |VERB - ADJ |DET - PRON| VERB - NOUN |NOUN - ADJ |
> | ------------- | ------------- | ------------- | ------------- |
> |17%| 13% |11% |10% |
> 
> Art Texts
> |NOUN - ADJ  |VERB - ADJ |AUX - VERB |PRON - SCONJ |
> | ------------- | ------------- | ------------- | ------------- |
> |27% |20% |13%| 10% |

> ### **dep**
> 
> Cooking Texts 
> |nmod - obl |nsubj - obj |det - obj |obj - obl|
> | ------------- | ------------- | ------------- | ------------- |
> |9% |3% |3% |3% |
> 
> Art Texts
> |nmod - obl |case - fixed| case - flat:name |nmod - appos  |
> | ------------- | ------------- | ------------- | ------------- |
> |9% |5% |4% |4% |

> ### **Lemma**
> 
> Cooking Texts   
> |il - lo |dosare - dosato |
> | ------------- | ------------- |
> |10%| 3% |
> 
> Art Texts
> |gentile - Gentile |suddividere - suddiviso |
> | ------------- | ------------- |
> |21% |7% |

### PoSTWITA  - Error Analysis (incorrect tag - correct tag)
> ### **POS**
> 
> Cooking Texts 
> |VERB - NOUN |ADJ - NOUN |ADJ - VERB |DET - PRON|
> | ------------- | ------------- | ------------- | ------------- |
> |15% |14% |12% |9% |
> 
> Art Texts
> |ADJ - NOUN |DET - NUM |DET - PRON |ADJ - VERB|
> | ------------- | ------------- | ------------- | ------------- |
> |19% |18% |9% |8%|

> ### **dep**
> 
> Cooking Texts 
> |nmod - obl |amod - obj |nummod  - det|  ccomp - xcomp|
> | ------------- | ------------- | ------------- | ------------- |
> |6% |3% |2% |2% |
> 
> Art Texts 
> |nmod - obl| nummod - det | case - flat:name |case - fixed |
> | ------------- | ------------- | ------------- | ------------- |
> |8% |7% |2% |2%|

> ### **Lemma**
> 
> Cooking Texts 
> |l??? - il |fara - farina |d??? - di | la - lo |
> | ------------- | ------------- | ------------- | ------------- |
> |6%| 4% |4% |4% |
> 
> Art Texts
> |l??? - il | li - il| gentile - Gentile |le - il |
> | ------------- | ------------- | ------------- | ------------- |
> |17% |9% |6% |3% |


## Annotators disagreements analysis (Annotator_1 tag - Annotator_2 tag)
> ### **POS**
> 
> Cooking Texts 
> |DET - NOUN |AUX-VERB |ADJ - VERB| ADV - NOUN|
> | ------------- | ------------- | ------------- | ------------- |
> |23% |23% |10% |8%|
> 
> Art Texts
> |NOUN - PROPN| AUX - VERB |ADJ - NOUN |ADJ - VERB |
> | ------------- | ------------- | ------------- | ------------- |
> |23% |19%| 15% |11% |

> ### **dep**
> 
> Cooking Texts 
> |appos - nummod| nmod - obl |amod - compound| obj - xcomp |
> | ------------- | ------------- | ------------- | ------------- |
> |4.8% |4.4% |4% |3.5% |
> 
> Art Texts
> |nmod - obl |appos - nmod |flat:name - nmod |advmod - case|
> | ------------- | ------------- | ------------- | ------------- |
> |5.7% |4.7% |4.7% |4.7% |
