# Computational-Linguistics-II-Report

## Corpus Structure

|  | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **Size** (in characters) | 3.164  | 3.031  | 3.112  | 3.448 | 3.378  |
| **Year**  | 1907  | 1927  | 1947  | 1969  | 2009  |


## Pipeline:
- **Automatic sentence splitting/tokenization and manual revision**
- **Automatic morphosyntactic parsing and manual revision** using UD Annotatrix
- **Interannotator Agreement** with a colleague
- **Disagreements resolution** and **Gold Corpus creation**
- **ISDT and Postwita Validation**

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
### Postwita
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
- **POS and dep**
## Annotators disagreements analysis
