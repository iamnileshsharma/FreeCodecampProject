# Mean, Variance, and Standard Deviation Calculator

This project provides a Python function to calculate the mean, variance, standard deviation, maximum, minimum, and sum for a 3x3 matrix constructed from a list of 9 numbers. The calculations are performed along both axes and for the flattened matrix.

## File Structure

- [`mean_var_std.py`](mean_var_std.py): Contains the main function for performing the calculations.

## Usage

1. Ensure you have [NumPy](https://numpy.org/) installed:
    ```sh
    pip install numpy
    ```

2. Run the script:
    ```sh
    python mean_var_std.py
    ```

3. The script will output the calculations for the example list `[0,1,2,3,4,5,6,7,8]`.

## Function

- `calculate(list)`:  
  Accepts a list of 9 numbers, reshapes it into a 3x3 matrix, and returns a dictionary with the following keys:
    - `'mean'`
    - `'variance'`
    - `'standard deviation'`
    - `'max'`
    - `'min'`
    - `'sum'`

  Each key maps to a list containing:
    1. Calculations along columns (axis 0)
    2. Calculations along rows (axis 1)
    3. Calculation for the entire matrix

## Example Output

```python
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.666..., 0.666..., 0.666...], 6.666...],
  'standard deviation': [[2.449..., 2.449..., 2.449...], [0.816..., 0.816..., 0.816...], 2.581...],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

## License

This project is provided for educational purposes.