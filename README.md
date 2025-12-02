Distance Calculation Between Points

This Python script calculates various types of distances between pairs of points in a 2D space. The distances calculated include:

Euclidean Distance

Manhattan Distance

Minkowski Distance (with p=3)

The script reads a dataset from a CSV file, computes the distances for each pair of points, and outputs the results in a new DataFrame.

Features

Euclidean Distance: The straight-line distance between two points. It is calculated using the standard formula for Euclidean distance.

Manhattan Distance: The sum of the absolute differences of their coordinates. It’s also known as the "taxicab" or "city block" distance because it calculates the total movement required on a grid (like a taxi traveling along streets in a city).

Minkowski Distance: A generalized version of both Euclidean and Manhattan distances, where you can adjust the power parameter (
p
p) to control the type of distance. In this script, the distance is calculated with 
p=3
p=3, but you can change this value to compute other variations of Minkowski distance.

The script calculates these distances for each pair of points in the dataset and stores the results in a Pandas DataFrame.
