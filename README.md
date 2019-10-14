# Xtern-Assessment

Through plotting the scooters on a 2D graph, it is evident that there are groups of scooters close to each other.
To identify these clusters, I used k-means clustering to group the scooters into 4 clusters. The cluisters had the
following sizes: (Blue:7050), (Yellow:5813), (Green:4886), (Purple:7919) 
The average charge per scooter in these clusters were 2.49, 2.47, 2.50, 2.52 respectively.
The SuperCharger is quite far from the scooters, and is closest to the green cluster.
The distances between Clusters is mentioned below (assuming unit length to be 1 mile):

Blue-Yellow = 0.43 miles,
Blue-Purple = 1.36,
Blue-Green = 1.57,
Yellow-Purple = 1.86,
Yellow-Green = 1.06

Sinced the scooters have the approx. the same avg charge, we should prioritize charging the scooters in clusters from
the highest to lowest in terms of quantity. i.e, Purple, Blue, Yellow, Green
The distance between Purple and Blue are approx. 1.36 miles, and assuming a speed of 50mph, it will take 1.6 min to travel.
The supercharger should picl up scooters from Purple, and drop them off at Blue and then pick up some more at Blue and drop them off at Purple. Once all the scooters have been charged, the same can be repeated at the Green and Yellow clusters.
The charging will take on avg 2.5 hrs per scooter.
