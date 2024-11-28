# Shark Tank Sentiment & Text Analysis

## Introduction

In this project, we apply text mining techniques to analyze Shark Tank episode descriptions and predict whether the entrepreneurs secured a deal. The analysis involves extracting meaningful insights from the text, such as frequently occurring words, sentiment analysis, and word cloud generation.

## 2.1 Pick Out the Deal (Dependent Variable) and Description Columns into a Separate Data Frame

The dataset from Shark Tank contains several features, but for text mining, we are primarily interested in the **deal** (whether the entrepreneur secured a deal) and the **description** of the pitch. We extract these two columns into a new data frame for analysis.

### Example of Data Frame:

Here’s a preview of the new data frame, containing the **deal** and **description** columns:

| deal  | description                                          |
|-------|------------------------------------------------------|
| True  | Vice meets virtue with this new wine spritzer...     |
| True  | Breathometer makes breathalyzer tests accessible... |
| True  | Love the outdoors but bummed about the prospect...  |
| False | A ticketless coat checking system for events...     |
| False | Diamond Dallas Page puts the DDP in DDP Yoga...     |

## 2.2 Create Two Corpora: One for Those Who Secured a Deal, the Other for Those Who Did Not Secure a Deal

We split the data into two corpora:
- **Corpus 1:** Pitches from entrepreneurs who secured a deal.
- **Corpus 2:** Pitches from entrepreneurs who did not secure a deal.

### Example of Corpora:

- **Corpus 1 - Deal Secured:**

| description                                        |
|----------------------------------------------------|
| Vice meets virtue with this new wine spritzer...  |
| Breathometer makes breathalyzer tests accessible...|
| Love the outdoors but bummed about the prospect...|

- **Corpus 2 - Deal Not Secured:**

| description                                        |
|----------------------------------------------------|
| A ticketless coat checking system for events...   |
| Diamond Dallas Page puts the DDP in DDP Yoga...   |

## 2.3 The Following Exercise is Done for Both the Corpora:

### a) Find the Number of Characters in Both Corpora

- **Number of characters in the corpus of those who secured a deal:** 62,360
- **Number of characters in the corpus of those who did not secure a deal:** 45,997

### b) Remove Stop Words from the Corpora

Stop words such as "also", "made", "makes", "like", "this", "even", "company" were removed from the corpora to focus on more meaningful words.

### c) Top 3 Most Frequently Occurring Words in Both Corpora

After removing stop words, the top 3 most frequent words in each corpus were identified:

- **Corpus – Deal Secured:**
  1. Products
  2. Designed
  3. Without

- **Corpus – Deal Not Secured:**
  1. Water
  2. Use
  3. System

### d) Plot the Word Cloud for Both Corpora

Here are the word clouds generated from both corpora:

- **Word Cloud for Deal Secured Corpus:**


<img width="464" alt="image" src="https://github.com/user-attachments/assets/4e2931fa-0cc5-4b55-a433-10abc1ca820c">

- **Word Cloud for Deal Not Secured Corpus:**


<img width="486" alt="image" src="https://github.com/user-attachments/assets/91c4c359-d402-454c-b366-a6df82c87315">


## 2.4 Inferences from the Word Clouds

From the word clouds, we can infer that words like "product", "use", and "design" appear frequently in both corpora. This suggests that entrepreneurs who secured deals often focused on the usability and design of their products, which may have been key to their success.

## 2.5 Analysis of Entrepreneurs Who Introduced Devices

Looking at the word clouds, we cannot definitively conclude that entrepreneurs who introduced devices were less likely to secure a deal. However, it appears that those who focused on products that were simple to use and clearly designed for their target audience (e.g., children, easy systems) had a better chance of securing a deal.

## Conclusion

Through this text analysis of Shark Tank pitch descriptions, we were able to extract key insights about the types of products or ideas that attract investors. The project highlights the value of text mining techniques like word cloud generation and frequent word analysis in understanding business trends and investor preferences.
