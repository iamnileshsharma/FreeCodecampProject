# Demographic Data Analyzer

This project analyzes demographic data extracted from the 1994 Census database. It calculates various statistics and metrics about education, salary, race, gender, and employment patterns.

## Description

The analyzer performs the following calculations:
- Race distribution in the dataset
- Average age of men
- Percentage of people with Bachelor's degrees
- Percentage of high education vs low education salary comparisons
- Minimum working hours and related salary statistics
- Country-wise salary analysis
- Most popular occupation for high earners in India

## Prerequisites

- Python 3.x
- pandas library

## Installation

1. Clone this repository or download the source code
2. Install required packages:
```sh
pip install pandas
```
3. Ensure the `adult.data.csv` file is in the project directory

## Usage

Run the script:
```sh
python demographic_data_analyzer.py
```

## Data Format

The `adult.data.csv` file should contain the following columns:
- age
- workclass
- fnlwgt
- education
- education-num
- marital-status
- occupation
- relationship
- race
- sex
- capital-gain
- capital-loss
- hours-per-week
- native-country
- salary

## Example Output

```
Number of each race:
White                 27816
Black                  3124
Asian-Pac-Islander     1039
Amer-Indian-Eskimo      311
Other                    271
Average age of men: 39.4
Percentage with Bachelors degrees: 16.4%
Percentage with higher education that earn >50K: 46.5%
Percentage without higher education that earn >50K: 17.4%
Min work time: 1 hours/week
Percentage of rich among those who work fewest hours: 10.0%
Country with highest percentage of rich: Iran
Highest percentage of rich people in country: 41.9%
Top occupations in India: Prof-specialty
```

## Function Documentation

### `calculate_demographic_data(print_data=True)`

Parameters:
- `print_data`: Boolean, determines whether to print results (default: True)

Returns:
- Dictionary containing all calculated statistics

## License

This project is free to use for educational purposes.

## Acknowledgments

Data source: 1994 Census database
