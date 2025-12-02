Distance Calculation Between Points

This Python script calculates various types of distances between pairs of points in a 2D space. The distances calculated include:

Euclidean Distance

Manhattan Distance

Minkowski Distance (with 
p=3
p=3)

The script reads a dataset from a CSV file, computes the distances for each pair of points, and outputs the results in a new DataFrame.

Features

Calculates Euclidean distance: The straight-line distance between two points.

Calculates Manhattan distance: The sum of the absolute differences of their coordinates.

Calculates Minkowski distance: A generalization of both Euclidean and Manhattan distances with a customizable power parameter (
p
p).

Outputs the results as a Pandas DataFrame.

Requirements

To run this script, you need to have the following Python packages installed:

pandas: For data manipulation and handling CSV files.

scipy: For calculating different distance metrics.

You can install the necessary dependencies by running:

pip install pandas scipy

Input Data

The script expects an input CSV file with the following structure:

Point1_x	Point1_y	Point2_x	Point2_y
1	2	4	6
2	3	5	7
...	...	...	...

Where:

Point1_x and Point1_y are the coordinates of the first point.

Point2_x and Point2_y are the coordinates of the second point.


The results will be printed to the console and look like this:

   Index      Point1      Point2  Euclidean  Manhattan  Minkowski (p=3)
0      0  [1, 2]  [4, 6]  5.0        7.0      5.385164
1      1  [2, 3]  [5, 7]  5.0        8.0      5.385164

Example Output:
Index	Point1	Point2	Euclidean	Manhattan	Minkowski (p=3)
0	[1, 2]	[4, 6]	5.0	7.0	5.385164
1	[2, 3]	[5, 7]	5.0	8.0	5.385164

Euclidean: The straight-line distance between the two points.

Manhattan: The sum of the absolute differences in the horizontal and vertical directions.

Minkowski: A generalized distance metric with 
p=3
p=3, combining aspects of both Euclidean and Manhattan distances.

Output

The calculated distances are displayed for each pair of points, including:

Euclidean distance: The direct "as-the-crow-flies" distance.

Manhattan distance: The total of horizontal and vertical distances.

Minkowski distance (p=3): A generalization of the other two distances with a configurable power parameter.

The results are stored in a Pandas DataFrame, which can easily be exported to a CSV file if needed.

Customization

You can modify the script to calculate other distance metrics by adjusting the distance functions from the scipy.spatial module.

You can also change the value of p in Minkowski distance to compute different variants of this metric.
