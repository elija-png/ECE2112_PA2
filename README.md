# ECE-2112-PA2
**Made by: Elijah Theodore P. Rojo | 2ECE-D**

This repository contains the Programming Assignment 2 for our course "Advanced Computer Programming" for S.Y. 2026-2027. This project covers three Python problems related to Module 2: NUMERICAL PYTHON (NUMPY).

---

## A. REPRODUCIBLE NORMALIZATION PROBLEM
Create a reproducible random 5 × 5 integer ndarray named X. Use the following two statements before
performing any calculation:

The functions and methods used in this problem:
* **`np.random.seed()`**: Sets a fixed seed (`2112`) to ensure pseudo-random number generation is reproducible across executions.
* **`np.random.randint()`**: Generates a 5 × 5 array (`X`) containing random integers ranging from 10 to 100.
* **`.mean()`**: Computes the arithmetic mean of all elements in the array `X` (`x_mean = 46.36`).
* **`.std()`**: Calculates the standard deviation of array `X` (`x_std ≈ 25.864`).
* **Array Broadcasting / Arithmetic Operations**: Computes standard normalization on `X` using the formula `(X - x_mean) / x_std`.
* **`np.save()`**: Exports the normalized 2D array to a local file (`X_normalized.npy`).

---

## B. CUBES DIVISIBLE BY 4 PROBLEM

Using NumPy, create the first 100 positive integers, cube every element, and reshape the result into a
10 × 10 ndarray named C. Thus, C begins with 1³ and ends with 100³. Use a Boolean condition on C to obtain every cubed value divisible by 4. Store the selected values in
`div_by_4`. Preserve NumPy’s normal row-major selection order.

The functions and methods used in this problem:
* **`np.arange()`**: Generates a 1D array of the first 100 positive integers (1 to 100).
* **Exponentiation Operator (`**3`)**: Cubes each element of the integer array vectorially.
* **`.reshape()`**: Reshapes the 100-element 1D array into a 10 × 10 2D matrix named `C`.
* **Boolean Indexing / Modulo Operator (`C % 4 == 0`)**: Evaluates a boolean mask to filter and retrieve array elements where the remainder divided by 4 equals 0 (`div_by_4`).
* **`np.save()`**: Saves the resulting 1D filtered array to `divide_by_4.npy`.

---

## C. ABOVE-MEAN SQUARES PROBLEM

Create a 6 × 6 ndarray named S containing the squares of the first 36 positive integers in increasing
row-major order. Compute the mean of all elements of S and store it in `S_mean`. Then use Boolean
filtering to select only the elements strictly greater than `S_mean`. Store these values in `above_mean`.

The functions and methods used in this problem:
* **`np.arange()`**: Generates a 1D array of the first 36 positive integers (1 to 36).
* **Exponentiation Operator (`**2`)**: Computes the square of each element in the array.
* **`.reshape()`**: Converts the 36-element array into a 6 × 6 2D matrix named `S`.
* **`.mean()`**: Calculates the overall mean of array `S` (`S_mean ≈ 450.167`).
* **Boolean Masking (`S > S_mean`)**: Creates a boolean array of identical dimensions (`filter_mean`) marking `True` for entries strictly greater than `S_mean`.
* **Boolean Filtering (`S[S > S_mean]`)**: Filters and extracts all values greater than `S_mean` into a 1D ndarray `above_mean`.
* **`np.save()`**: Saves the filtered ndarray to `above_mean.npy`.

---
Thank you for reading!  
To see the main Python program for Programming Assignment 2, click this link: https://github.com/elija-png/ECE2112_PA2/blob/edb15f46d7b2e5b342e881e9d3fac6992ad597f8/ECE2112_PA2.ipynb
---
**README Changelog:**  

**SEPTEMBER 2, 2026: UPDATED DETAILS OF THE DRAFT. ENTIRE DRAFT**  
**SEPTEMBER 1, 2026: INITIAL DRAFT OF README**
