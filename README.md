# The Gender Gap in Goodreads Ratings

## Motivation
As an avid reader with a background in Women and Gender Studies, I've long noticed patterns in how books are talked about, marketed, and received depending on who wrote them. Which books get adapted into films. Which ones get dismissed as "smut" while similar content by male authors gets called literary fiction. Which authors hide behind initials to be taken seriously. This project uses data to investigate whether those patterns show up in how readers actually rate books on Goodreads.

## Data
I used the goodbooks-10k dataset, a cleaned collection of 10,000 popular books with rating and authorship data sourced from Goodreads. Author gender was inferred using the gender-guesser Python library based on first names.

## Findings
### 1. Male authors dominate popular books.
Of the 10,000 books in this dataset, male authors outnumber female authors with 4,584 male vs 3,403 female among books where gender could be determined.

<img width="790" height="490" alt="image" src="https://github.com/user-attachments/assets/e3b2372f-0a9b-4392-b45b-9e3e93c189cd" />

### 2. Male authors rate higher on average.
Male authored books average 4.01 vs 3.98 for female authored books. In a dataset where most books cluster within a narrow band, this consistent gap across thousands of books is meaningful.
### 3. Authors using initials rate highest of all.
498 authors use initials instead of first names and average 4.07, higher than both male and female authors. Using initials to obscure gender, most famously practiced by J.K. Rowling at her publisher's suggestion, appears to correlate with higher reader ratings.

## Limitations
**Gender was inferred** from first names which is **imperfect and binary** as it doesn't capture non-binary authors or authors whose names are culturally unfamiliar to the library
This **dataset reflects popular books** and may not represent publishing broadly
**Correlation is not causation** and other factors like genre and marketing likely contribute

## What's Next
1. Genre analysis to examine whether the gender rating gap varies by category
2. Analysis using more recent and comprehensive data
3. Investigating which books get adapted to film or TV by author gender
