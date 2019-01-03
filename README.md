# Introduction:

The city of Mumbai has a large amount restaurants, but still there is always scope for new ones. Finding a suitable location for it to flourish is the most important factor for a restaurant. It has to be set up in a location where one can attract a good crowd as well as it must be located in an area where there is little or no competition.

We will be able to provide a solution for anyone looking to open an Chinese cuisine restaurant in the city of Mumbai.

The Goal of this problem is to find a location that suits the below criteria. 

1) A location that has many restaurants in the vicinity (European,Intercontinental,Indian) 

2) A location that has no or few Chinese cuisine restaurants, as this will ensure that there very little competition with other competitiors.


# Data:

The data that will be used in this projects is a csv file having data related to all neighborhoods in the city of Mumbai.

Finding a suitable location for a restaurant to flourish is an important

We explore the neighborhoods using Foursquare API to find the avenues within 500 meters of each neighborhood.

The Foursquare API that will be used to explore the neighborhoods is https://api.foursquare.com/v2/venues/explore.

This API returns json response which will be transformed into a Data Frame, taking only the required details into consideration.

# Methodology

Using the Foursquare API venue information is obtained in nearby vicinity of postal locations in Mumbai. A radius is set to cover large neighborhoods in a particular area in Mumbai.

This data is then merege with the Location dataset (Postal Codes) and a clustering algorithm is applied to the data.

K-Means Clustering : The data points are clustered into 4 clusters using K-Means algorithm. The goal of this algorithm is to find groups in the data, with the number of groups represented by the variable K. The algorithm works iteratively to assign each data point to one of K groups based on the features that are provided.

# Results
By exploring the requirements we found only two neighborhoods that match the requirements (Many restaurants in the vicinity & only a few Chinese restaurants)


# Discussion

According to results we observe that most common venues (Top 10) come out to be restaurants and Pizza places and Snack places, which means any new chef/business man can start a restaurant provided that they need to compete with existing restaurants (Other Types) but only if he provides top class facilities to get to top.

# Conclusion 

Based on the Clusters formed it would be a good idea to open a restaurant in Clusters 2 & 3 since the other clusters already have Chinese Restaurants in their vicinities.
Also Cluster 2 & 3 have many restaurants in the vicinity (Pizza restaurants,European,Intercontinental,Indian) so one will be able to attract a good crowd.
Also there is no other competitors in this neighborhood who have set up Chinese restaurants nearby.
These results have limitations The venue data obtained is of top 10 venues in each neighborhood, where we might neglect Chinese restaurants with less frequency.
