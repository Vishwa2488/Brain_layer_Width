## **Brain Layer Width detection using brain data**

# Dependencies
python3
# Usage of code

To get the width values and intersection points, call newmapper function with the parameters:

# Usage of mapper() function
1.   **link:** link of json file containing the data
2.   **basecoordinatesindex:** The index of lateral ventricle as per the order in which the features are stored in the json file. This can be got by using the 'seelateralventricle' function defined below. Give the index of the lateral ventricle from which you want the normal to be drawn.
3.   **withsubpiallayer:** The default value of this parameter is 0 meaning subpial layer data won't be visible by default. Subpial layer data can have None type data too. So to avoid it, the default value is 0. But if you give the value as 1, then you can also get the data for subpial layer with some data as None. None is assigned to data that cannot be found with the data in the json file.
4.   **motion:** The default value of this parameter is 1. This parameter states the direction in which the normals are drawn on the given lateral ventricle for finding the data. Giving this as -1 will make the index of coordinates on lateral ventricle boundary to decrease with every iteration.
5. **startingindex:** The default value of this parameter is 0. This gives the first index of list having the coordinates of lateral ventricle at which normal is drawn. This can be changed if 0 index is at a point where there is no required layer for data retrival.


# Usage of seelateralventricle function

Give the path of the json file as parameter to the function and it will show the brain layer and the lateral ventricle and a small starting part. **This starting part will help you understand where the 0 index is present in the lateral ventricle and hence helps you to approximate the startingindex parameter**.
