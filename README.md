# News Article Analyzer

## Overview

News Article Analyzer is a Python program that performs text analysis on a news article. The program allows users to search for specific words and generates statistics about the article's content.

The application performs the following tasks:

* Counts occurrences of a specified word
* Identifies the most common word
* Calculates the average word length
* Counts the number of paragraphs
* Counts the number of sentences

## Requirements

* Python 3.x
* Standard Python libraries:

  * `re`
  * `collections.Counter`

No additional installations are required.

## Running the Program

1. Open the project folder (`SummativeLab1`) in Visual Studio Code.
2. Open the file `NewArticleAnalyzer.py`.
3. Run the program:

```bash
python NewArticleAnalyzer.py
```

4. When prompted, enter a word to search for in the article.
5. Review the analysis results displayed in the terminal.

## Features

* Case-insensitive word searching
* Automatic text processing using regular expressions
* Most common word identification
* Average word length calculation
* Paragraph counting
* Sentence counting
* User input validation through string cleaning (`strip()`)

## Functions

### count_specific_word(text, search_word)

Counts the number of occurrences of a specified word in the article and returns the result as an integer.

### identify_most_common_word(text)

Determines the most frequently occurring word in the article and returns it as a string.

### calculate_average_word_length(text)

Calculates and returns the average length of words in the article as a float.

### count_paragraphs(text)

Counts the number of paragraphs based on blank lines separating blocks of text.

### count_sentences(text)

Counts the number of sentences using periods (`.`), exclamation marks (`!`), and question marks (`?`) as sentence delimiters.

## Edge Cases

The program handles the following edge cases:

| Function                        | Empty Input Result |
|                                 |
| identify_most_common_word()     | None               |
| calculate_average_word_length() | 0                  |
| count_paragraphs()              | 1                  |
| count_sentences()               | 1                  |

## Program Structure

The application demonstrates the use of:

* Functions
* Variables
* For loops
* While loops
* If/Else statements
* Regular expressions
* Python collections (`Counter`)

## Testing

To verify functionality:

1. Search for words known to exist in the article (e.g., "Apple", "AI", "technology").
2. Search for words not present in the article.
3. Verify that counts, sentence totals, and paragraph totals are reasonable.
4. Test edge cases using empty strings within the functions.

## Version Control

Recommended Git workflow:

```bash
git init

git add .
git commit -m "Initial project setup"

git add .
git commit -m "Implement text analysis functions"

git add .
git commit -m "Add testing and documentation"
```

## Author

Created as part of the Summative Lab: Analyze a News Article assignment.

