
# IBM Applied Data Science Capstone Project
## Week 4 Report - 1st Draft

### Project Title: Clustering for Similarities in NYC & Toronto<br><br>
#### Table of Contents
1. [1. Introduction & Problem Statement](#PartOne)
2. [2. Data Acquisition & Preparation](#PartTwo)

<a id='PartOne'></a>
****
#### 1. Introduction & Problem Statement
****

##### 1.1 Introduction
During this long voyage through IBM's Professional Certificate track, we've learned so much about the whole notion of using the data all around us to create stories and say something meaningful with them. This is my attempt at exactly that.
In this Capstone Project, we will try and visualize, in different ways while using different techniques, the similarities between NYC and Toronto.
New York City (NYC) is one of the most populous cities in the USA, having a wide range of diversity, be it cultural or otherwise. Also, we are looking at one of the most powerful states, in economic terms. Besides her illustrious fame, acquired with the exposure in so many mediums (TV shows, movies, etc), her beauty makes her one of the most visited places in the world, for the past several years. In Nyc we have five (5) boroughs: Manhattan, Staten Island, Queens, Brooklyn and the Bronx.
Toronto shares many of NYC's characteristics, from the get-go. Also, the most populous city in Canada, as well as being one of it's most powerful centers for businesses, manufacturing etc. Here, in Toronto, things might be a lot more toned down compared to NYC, but it's beauty is still there for travelers to enjoy.

##### 1.2 Problem Statement
Using data wrangling techniques and location data we will study, analyze, cluster and compare the neighbourhoods of NYC and Toronto. We will dive headlong into the data at hand, using most of the techniques passed on to us throughout this course and try to see the similarities between the two cities.
The provided analysis and conclusion will give a better understanding to anyone interested, be it a business enthusiast, an avid traveler or just a data fan, as to what makes these two cities "identical" (may be a strong word!), or "unique"!

<a id='PartTwo'></a>
*****
#### 2. Data Acquisition & Preparation
*****

##### 2.1 Data Acquisition
We have in our disposal two basic data structures to handle; the first being our 'Neighbourhood Data' and the second, our 'Venues Data'.
- **A. Neighbourhood Data**

The datasets used for our two cities came from two (2) different sources; for NYC, they were provided by the staff of IBM's "Data Science Professional Certificate" and for Toronto, internet scraping was used. For both, the data acquired consist of major, albeit basic, information such as Neighbourhood, Borough, Latitude and Longitude coordinates.
- **B. Venues Data**

Here we used FourSquare's API to obtain information about the venues in our cities' neighbourhoods. They consist of many different information fields, but using the right code parameters, we got just the needed fields. FourSquare is one of the largest location and venue data sources and their API was utilized to demonstrate our project idea.
<center><i>Reserved space for future example tables</i></center>

##### 2.2 Data Preparation


**A. Neighbourhood data**  
 - ***New York City***  
 As stated above, the dataset for NYC's neighbourhoods were provided by the course's staff. It came in a <i>.json</i> format file, with all the required information we need to divide up the city by it's inner territories. Storing the data in a <i>Panda's Dataframe</i> with the needed data wrangling techniques, gave us the desired result. With the final data at hand, we are now able to "explore" NYC's neighbourhoods, at least in a basic, for now, way.


 <center><i>Reserved space for future example tables</i></center>

 - ***Toronto***  
 For Toronto, we had to get our hands more "dirty", in order to compile the desired data structure. The information was provided via the Wikipedia page for Toronto's neighbourhoods ([wiki link](https://en.wikipedia.org/w/index.php?title=List_of_postal_codes_of_Canada:_M&oldid=942851379)), but on an earlier version state than the current, because of the data format used now on the wiki page, being incompatible for scraping <i>(or at least our current techniques!)</i>. This came, as expected, in <i>.html</i> format. Next, using a dataset provided yet again by the course's staff containing each of Toronto's neighbourhood' corresponding Post Code along with their respective lat/lng coordinates, in <i>.csv</i> format. Combining the two sets with the proper parameters and cleaning, the desired data structure was at our disposal.


 <center><i>Reserved space for future example tables</i></center>

**A. Venues data**  

The FourSquare API provided us with a large amount of venue information about our two cities. With the proper keys to use this API (as most API's need nowadays), and the right code to "hit" those calls successfully towards the API, we gathered our information.
Retrieving data and then going through all the notions to get them in the format that is needed can be a long and arduous procedure. Here comes the power of Python and its Object Oriented nature. We were able to combine the knowledge and techniques acquired through the entire specialization, in order to define 3 major functions in our code, that ultimately gave us the ability to reach our end-goal with as little as 1 line of code!


 <center><i>Reserved space for future example tables</i></center>

In further detail, first we defined the proper way to "talk" to FourSquare <i>(function get_near_by_venues)</i> and retrieve the basic data for our Venues, Venue Name & Category and lat/lng coordinates, in respect to their neighbourhoods.


 <center><i>Reserved space for future example tables</i></center>

Then, defining our one-hot encoding techniques and data normalization, the data now are grouped and transformed in a way that is easier for us to understand and manipulate further. <i>(functions explore_borough and return_venues_for_boroughs)</i>


 <center><i>Reserved space for future example tables</i></center>

Finally, both datasets were in a format that was not just aligned to one another, but also provided useful information, again, within a few lines of code and the backing power of Python and Object Oriented Programming Design, with the use of functions to be used generally and on the spot.


 <center><i>Reserved space for future example tables</i></center>

This is our first, brave step, towards our end-goal.    
Getting our idea, around the data provided around us, then using the proper skillset and techniques, <i>(also provided abundantly with the fine example of IBM's courses)</i>, in order to have that idea tell a story.  
A Digital Story of a Data Scientist.


```python

```
