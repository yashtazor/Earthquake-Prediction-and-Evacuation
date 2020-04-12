# Earthquake-Prediction

This is a project under the 'Algorithms' course. 
The goal of our project was to try to create a ML model manually without using any external libraries like SciKitLearn.

##### What does the flow of control look like?

1. We constructed a manual Linear Regression Model by solving unknowns (which are actually the epicentre distances from the point of consideration) of the equations we generated ourselves by finding the unknowns given a set of s & p values which are the two types of earthquake waves.
2. Then we generated some random amplitudes and then calculated the range by subtracting the maximum and minimum magnitude 
distances. The magnitudes were calculated according to this formula

#### ML = logA + 2.56logD - 1.67

3. Having detected the range, we used the max flow algorithm to evacuate the population as fast as possible and in the most
efficient manner. They were evacuated to the closest node out the earthquake range calculated in the previous point. A Neo4J graph
database was used to store places where every place was represented by a single node.

For additional reading, please refer the following in order.

1. http://www.geo.mtu.edu/UPSeis/locating.html
2. https://www.bgs.ac.uk/discoveringGeology/hazards/earthquakes/magnitudeScaleCalculations.html

### NOTE

These equations were generated by using random values by using random inbuilt function in python which is actually 
wrong considering ML where a dataset is previously already included. But again, our goal here was to create a model which 
would work on a single set of values. Hence, obviously, it can be extended to process large dataset also.


