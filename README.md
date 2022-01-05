# Analysis Of Mumbai City To Estimate Some Optimal Locations for A New Italian Restaurant

## 1. Background

Mumbai (previously known as Bombay until 1996) is a natural harbor on the west coast of
India, and is the capital city of Maharashtra state. It is India's largest city, and one of the
world's most populous cities. It is the financial capital of India and is a global city, known for
being the home to one of the highest number of billionaires as well as having huge global
influence. The city is the 9th most populous in the world. It has approximately 20 million
people. Along with the neighboring cities of Navi Mumbai and Thane, it forms the world's
4th largest urban agglomeration.

## 2. Business Problem

As you can see from the figures, Mumbai is a city with a high population, In this project we
will try to find an optimal location for a restaurant. Specifically, this report will be targeted
to stakeholders interested in opening an Italian restaurant in Mumbai, India.
Since there are lots of restaurants in Mumbai we will try to detect locations that are not
already crowded with restaurants. We are also particularly interested in areas with no Italian
restaurants in vicinity. We would also prefer locations as close to city.

We will generate a few most promising neighborhoods based on this criteria.


## 3. Data
Following data sources will be needed to extract/generate the required information:

* Centers of candidate areas will be generated algorithmically and approximate addresses of centers of those areas will be obtained using Geopy reverse geocoding.
* Number of restaurants and their type and location in every neighborhood will be obtained using Foursquare API.
* Coordinate of Mumbai center will be obtained using Geopy reverse geocoding.

Based on definition of our problem, factors that will influence our decision are:

* Number of existing restaurants in the neighborhood (any type of restaurant)
* Number of Italian restaurants and distance to Italian restaurants in the neighborhood and distance of neighborhood from city center
* We decided to use regularly spaced grid of locations, centered around city center, to define our neighborhoods.

## 4. Methodology

Python **folium** module was used to visualize the results on the map of Mumbai City.
![alt text](https://github.com/ranjith-p/testing03/blob/master/1.JPG?raw=true)


Visualizing all the collected restaurants in the area in blue color and Italian restaurants in red.
![alt text](https://github.com/ranjith-p/testing03/blob/master/2.JPG?raw=true)

Heatmap showing **density of restaurants**, also a few circles indicating distance of 1km, 2km and 3km from Mumbai Center. 

![alt text](https://github.com/ranjith-p/testing03/blob/master/3.JPG?raw=true)


### To view the full Methodology and the results of this analysis go to this [article](https://www.linkedin.com/pulse/analysis-mumbai-city-estimate-some-optimal-locations-new-panicker/?published=t).
