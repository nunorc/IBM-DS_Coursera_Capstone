
# World Capitals Clustering Based on Venues

## Introduction

*Problem*

The problem we trying to solve is how can a travel agency
provide returning customers with targeted promotions to
places that customers will likely enjoy or be interested in?

*Approach*

The goal is to cluster a large number of cities, based on
the venues that cities offer to their visitors. And the main
intuition behind this approach is that if a traveler enjoyed
a particular city (or groups of cities) the chance that he or
she will enjoy a cities that offer similar points of interest
is higher than otherwise.


## Data

We start of with a list of the world capitals, and their
geographical location defined using latitude and longitude.
And then query the Foursquare API to gather information
about the venues available in each world capital. Much in
the same way that we used while segmenting and clustering
neighborhoods in the city of Toronto. We start by gathering
the venues that are in the radius of the city geographical
location, and aggregate the mean of venues across all capitals
by category, and use this to build clusters of city. This
hopefully will create groups of cities that offer a similar
contexts to visitors.
