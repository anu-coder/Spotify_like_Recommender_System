# Spotify like Recommender System

Music recommender systems (MRS) have recently exploded in popularity. Thanks to music streaming services like Spotify, Pandora and Apple Music. By some accounts, almost half of all current music consumption is by the way of these services. While recommender systems have been around for quite some time and are very well researched, music recommender systems differ from their more common siblings in some characteristically important ways: the duration of the items is less (3-5 min for a song vs 90 minutes for a movie or months/years for a book or shopping item), the size of the catalog of items is larger (10s of millions of songs), the items are consumed in sequence with multiple items consumed in a session, repeated recommendations have a different significance. Music Recommender Systems then require different approaches from traditional recommender systems.

## Project objective

* Objective of the project is to create a recommender system for automatic playlist continuation. 
* Given a set of playlist features, recommender systems should be able to generate a list of recommended tracks that can be added to that playlist, thereby ‘continuing’ the playlist.

## Approaches

1. __Non-Personalized Approaches:__ It includes recommending which is popular across the whole system. Simple and relatively easier to implement.
2. __Collaborative Filtering:__ Personalized recommendations, based on similarity between either users or items. User based CF assumes that users who behaved similarly (buying patterns, preference in movies or music, job application) in the past will behave similarly again in the future. 
3. __Content Based Filtering:__ The actual content of item refers to the actual characteristics of an item and these attributes are broken down into ‘tags’ and items are then matched to user preferences (as modelled by the tags) accordingly.

<p align = "center">
<img src = "https://github.com/anu-coder/Recommender_System/blob/master/Recommander%20types.PNG">
</p>

### Dataset used: [Millionsongdataset](http://millionsongdataset.com/)

* We have used a part of the dataset containing a subset of 2 Million songs which is also available in the above website.
* Necessary citation : [Bertin-Mahieux2011, ISMIR](http://www.columbia.edu/~tb2332/Papers/ismir11.pdf)

