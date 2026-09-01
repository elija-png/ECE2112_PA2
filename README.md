# ECE-2112-PA2
**Made by: Elijah Theodore P. Rojo | 2ECE-D**

This repository contains the Programming Assignment 2 for our course "Advanced Computer Programming" for S.Y. 2026-2027. This project covers three Python problems related to Module 2: NUMERICAL PYTHON (NUMPY).

---

## A. REPRODUCIBLE NORMALIZATION PROBLEM
Create a reproducible random 5 × 5 integer ndarray named X. Use the following two statements before
performing any calculation:

The functions and methods were used in this problem:
* **Numpy's basic statistics tools, such as mean, and a randomizer function courtesy of Numpy.**
---
## B. CUBES DIVISIBLE BY 4 PROBLEM

Using NumPy, create the first 100 positive integers, cube every element, and reshape the result into a
10 × 10 ndarray named C. Thus, C begins with 13 and ends with 1003. Use a Boolean condition on C to obtain every cubed value divisible by 4. Store the selected values in
div by 4. Preserve NumPy’s normal row-major selection order.

The functions and methods used in this problem:
* **`np.arange`**: Sets the range the array should have

---
## C. ABOVE-MEAN SQUARES PROBLEM

Create a 6 × 6 ndarray named S containing the squares of the first 36 positive integers in increasing
row-major order. Compute the mean of all elements of S and store it in S mean. Then use Boolean
filtering to select only the elements strictly greater than S mean. Store these values in above mean.

The functions and methods used in this problem:
* **Extended Iterable Unpacking (`first, *middle, last = item`)**: Extracts the outer elements while capturing all interior elements into a list using the starred expression (`*`).
* **List Construction (`[...]`)**: Creates and returns a new list containing the swapped bookends alongside the unchanged middle elements
* **Unpacking Operator (`*middle`)**: Unpacks individual elements from the `middle` list directly into the new list enclosure.

```python
def swap_bookends(item):
    first, *middle, last = item
    return [last, *middle, first]
```
---
Thank you for reading!  
To see the main Python program for Programming Assignment 1, click this link: https://github.com/elija-png/ECE-2112-PA-1/blob/91ed091e39379f67c2b18320e4cb282aa8f9c49c/ECE2112_PA1_ROJO.ipynb
---
**README Changelog:**  

**SEPTEMBER 1, 2026: INITIAL DRAFT OF README**
