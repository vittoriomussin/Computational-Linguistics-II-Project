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
|  | Cooking Texts |  |  | Art Texts |  |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| **UPOS** | 94.74  | 97.44  | 90.56  | 96.28 | 96.31  |
| **XPOS**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **UFeats**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **Lemmas**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **UAS**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **LAS**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **BLEX**  | 0.97  | 0.96  | 0.96  | 0.97  | 0.96  |
| **Year**  | **1907**  | **1927**  | **1947**  | **1969**  | **2009**  |
### Postwita

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
