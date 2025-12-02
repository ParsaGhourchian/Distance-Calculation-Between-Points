Distance Calculation Between Points

This Python script calculates various types of distances between pairs of points in a 2D space. The distances calculated include:

Euclidean Distance

Manhattan Distance

Minkowski Distance (with 
p=3
p=3)

The script reads a dataset from a CSV file, computes the distances for each pair of points, and outputs the results in a new DataFrame.

Features

Euclidean Distance: This is the straight-line distance between two points. It’s calculated using the standard formula for Euclidean distance.

Manhattan Distance: This is the sum of the absolute differences of their coordinates. It’s also known as the "taxicab" or "city block" distance because it calculates the total movement required on a grid (like a taxi traveling along streets in a city).

Minkowski Distance: A generalized version of both Euclidean and Manhattan distances, where you can adjust the power parameter (
p
p) to control the type of distance. In this script, the distance is calculated with 
p=3
p=3, but you can change this value to compute other variations of Minkowski distance.

The script calculates these distances for each pair of points in the dataset and stores the results in a Pandas DataFrame.

Requirements

To run this script, you need to have the following Python packages installed:

pandas: For data manipulation and handling CSV files.

scipy: For calculating different distance metrics.

You can install the necessary dependencies by running:

pip install pandas scipy

Input Data

The script expects an input CSV file with columns representing the coordinates of two points. The CSV file should have the following structure:

Point1_x and Point1_y: The coordinates of the first point.

Point2_x and Point2_y: The coordinates of the second point.

Here’s an example of how the input CSV should be structured:

Point1_x,Point1_y,Point2_x,Point2_y
1,2,4,6
2,3,5,7


Each row represents one pair of points, and the script will calculate the distances for each pair.

Usage

Save your dataset as input_points.csv in the same directory as the script.


The script will output the calculated distances to the console in a format similar to this:

Index  Point1      Point2      Euclidean  Manhattan  Minkowski (p=3)
0      [1, 2]      [4, 6]      5.0        7.0        5.385164
1      [2, 3]      [5, 7]      5.0        8.0        5.385164


Where:

Index: The row number in the original dataset.

Point1: The coordinates of the first point.

Point2: The coordinates of the second point.

Euclidean: The Euclidean distance between the two points.

Manhattan: The Manhattan distance between the two points.

Minkowski (p=3): The Minkowski distance with 
p=3
p=3 between the two points.

Example Output:

For a sample dataset with two points [1, 2] and [4, 6], the output might look like this:

Index  Point1   Point2   Euclidean  Manhattan  Minkowski (p=3)
0      [1, 2]   [4, 6]   5.0        7.0        5.385164


This output shows the calculated distances for each pair of points in the dataset.

Output

The results will be printed to the console. For each pair of points, the script will display:

Euclidean distance: The straight-line distance between the two points.

Manhattan distance: The total of horizontal and vertical distances.

Minkowski distance (p=3): A generalized distance metric with 
p=3
p=3.

The results are also stored in a Pandas DataFrame, and you can easily export the results to a CSV file if needed.

Customization

You can modify the script to calculate other distance metrics by adjusting the distance functions from the scipy.spatial module.

You can also change the value of p in Minkowski distance to compute different variants of this metric.
