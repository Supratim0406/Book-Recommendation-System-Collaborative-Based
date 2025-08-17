# Book-Recommendation-System
Recommend books using various machine learning algorithms.
During the last few decades, with the rise of Youtube, Amazon, Netflix, and many other such web services, recommender systems have taken more and more place in our lives. 
In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy, or anything else depending on industries).

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/68fc50ad-4897-4f41-939e-2850b8d76650" />


## Data Description
The Book-Crossing dataset comprises 3 files.

### 1. Users
Contains the users. Note that user IDs ( ) have been anonymized and map to integers. Demographic data is provided ( , Age) if available. Otherwise, these fields contain NULL values.

### 2. Books
Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.

### 3. Ratings
Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

#
We tried to make models from various perspective like
### 1. POPULARITY BASED MODEL
#### 1.1 Highest total book rating
Top 50 Books are arranged in such a way that the books with the highest average ratings are at the top.


### 2. COLLABORATIVE Based FILTERING 
This model find the top 4 highly-rated books that meet these two conditions:
* Each book has received at least 50 ratings
* These ratings come from active readers who have rated 200 or more books
* This analysis uses collaborative filtering, which makes recommendations based on user behavior patterns and preferences.

  ### Demo 
