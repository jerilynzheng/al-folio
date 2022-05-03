---
layout: descrip
title: Similar Singer
description:
img: /assets/img/simsing.jpg
importance: 1
category:
---

# Similar Singer

*Overview*


**Problem**

**Team**

Timeline

Outcome

Features

Product

Challenges

Launch

Impact

Learnings

This app is different from existing online services like Spotify’s Related Artists feature and Apple Music’s recommendations. These services rely on shared listeners to recommend other artists. Our app utilizes the lyrics similarity between the songs of artists, as well as the genre similarity between artists. It also has the ability to take in more detailed user preferences with liked artists and disliked artists inputs. Similar Singer can also take in multiple liked artists and disliked artists, representing a user’s more general tastes rather than just one artist that they enjoy. We also allowed the user to give a description of the type of music/artist they wanted to see with a linguistic descriptor, allowing them to personalize their suggestions even more. For the output information, we provided the user with more details about the recommended artists, like album reviews and ratings, their top songs, genres, followings, and ranked similarities to the input.

From the first prototype to the second, we added a similarity subscore for genres, computed via Jaccard, to the final score. Since there are both liked and disliked artists, we used Rocchio to combine the Jaccard vectors for each artist given by the user. Using min/max scaling, we normalized both genre and lyric similarity scores to be between 0 and 1. Both scores are equally weighed. Next, we filtered the list of artists by follower count before ranking them by final similarity score. We set the minimum follower count to be a certain percentage of the liked artist’s follower count (in the second prototype, the percentage is 50%).

In the final prototype, we added the score obtained from the linguistic description to the final score. Then we changed the weights around to see which combination gave us results that were highly expected. We ended up weighing the genre score twice as much as the other two scores, because for artists that either do not have lyrics in their songs or use a foreign language, our lyric similarity score is a lot less accurate than genre. We also changed the rocchio coefficients to favor the liked artists’ genres more than the disliked artist’s genres. Also, we lowered the percentage of the liked artists’ average follower count to 20% because with the 50% threshold, the recommended list for popular artists like Drake would be composed solely of other popular artists that may not be so similar in terms of genre or lyrics.

Since the previous prototype, we were able to implement topic modeling for the linguistic description query. We trained an LDA model with a tokenized, lemmatized corpus of around 1,200 Pitchfork album (web-scraped) reviews to identify 10 topics with about 10 words in each. We used these topics to create a mapping from input query to topic to artist. Given a user’s natural language query, we would identify which topic was most likely to be associated with their query. Then, we would find the artists most likely to be associated with that topic and weigh those artists a little bit higher in the final scoring.

Initially, we tried to train the LDA model on a much larger corpus that was a combination of Pitchfork and Amazon music reviews but had issues with noisy data as well as difficulty parsing out non-English reviews (there were lots of Spanish-language reviews in the dataset). Eventually, we narrowed down the dataset to include only words that appeared in at least two documents and excluded words that appeared in more than 80% of the documents. We also trained multiple LDA models to find the optimal topic count to maximize topic coherence and minimize word overlap and found the value to be around k=10.

**Applied Concepts:**

-TF-IDF Matrix - vectorized each artist document which is comprised of the lyrics for their top ten songs

-Cosine Similarity - calculate lyric similarity using the TF-IDF matrix after SVD

-Jaccard Similarity - calculate genre similarity between two artists, stored in a matrix

-Rocchio Update Algorithm - combine liked and disliked artist vectors from the TF-IDF matrix and genre vectors from the Jaccard matrix

-SVD - reduce dimensionality of TF-IDF matrix
