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
<img src = "https://github.com/anu-coder/Recommender_System/blob/master/images/types.png">
</p>

### Dataset used: [Millionsongdataset](http://millionsongdataset.com/)

* We have used a part of the dataset containing a subset of 2 Million songs which is also available in the above website.
* Necessary citation : [Bertin-Mahieux2011, ISMIR](http://www.columbia.edu/~tb2332/Papers/ismir11.pdf)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# STEPS and OUTPUTS:

## A glimpse into the dataset: 

Among the 2M songs we have taken a subset of 10K songs, due to the hardware constraint of my system.
The dataset consists of five rows: __user_id, song_id, listen count, title, release, artistname, year, song.__

<p align = "left">
<img src = "https://github.com/anu-coder/Recommender_System/blob/master/images/Datasetglance.PNG">
</p>

## Type 1: Popularity based recommender

Popularity based recommander system is often known as the __cold start__ or __non personalised recommandation__. In this particular type, all the users are recommanded the set of songs which are most popular throughout the system. The determining criterion can be the highest number of views of the song. This is the easiest to implement, and doesnot require to explore other dependencies. It is important to undertsand that this recommendadtion is mainly targetted to the new users, when they havenot listened to any songs yet. so this reccomendation, recommends the same set of songs to all the user. 

There are __365__ distinct user, and __5151__ distinct songs in the 10K dataset we have used. 
Here is the popularity based recommendation to the __364th__ user. 

<p align = "left">
<img src = "https://github.com/anu-coder/Recommender_System/blob/master/images/popularitybasedreco.PNG">
</p>

## Type 2: Item similarity based personalised recommander

This is also known as the __Collaborative Filtering__ which is based on similarity between items. 
It first trains the model with respect to the views of the particular user, and then recommends similar items to the user, depending on their choices. Unlike popularity based recommendation, the moment the user starts listening to song, item similarity based recommandation is implimentated. 

<p align = "left">
<img src = "https://github.com/anu-coder/Recommender_System/blob/master/images/Item%20similaritybasedreco.PNG">
</p>



