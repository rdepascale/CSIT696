# CSIT696 - Research Methods in Computing
## Investigation of Hyperspectral Data Applications
### Montclair State University Spring 2021
### Advisor Stefan Robila, PhD


## Goals
* Learn about tools available to process document collections
  * Deliverable P2A
    * Processes a set of documents and finds the top 5 most frequently used words in the set (based on a given list of words).
  * Deliverable P2B
    * Processes a set of documents using some classic clustering algorithm.
* Machine grade ELA essays based on readability and vocabulary choice.
  * Deliverable P3B
    * Implementation of readability scores by Flesch-Kincaid, vocabulary scores by TF-IDF.
  * Deliverable P3C
    * Proof of concept on set of 15 ELA papers from a grade 9 classroom.
    * Machine grade each paper based on:
      * Readability Ratio
        * Each paper is assigned Coleman-Liau and Flesch-Kincaid readability score.
        * Score is divided by 12 for grade 12 being end of high school and assumption that an idealized paper should be at least in the 9-12 grade range.
      * Mean Vocabulary Score
        * Average TF-IDF score of 10 most frequent words in corpus for given paper.
        * Average TF-IDF score of 10 most frequend words in given paper.
      * Floor of Sum of Readability Ratio and Mean Vocabulary Score is multiplied by 100 and converted to integer in attempt to avoid inflating machine score.
        * Min Readability of Coleman-Liau and Flesch-Kincaid is used for avoiding inflation as well.
