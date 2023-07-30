# Market Basket Analysis in Python using Apriori Algorithm

Whenever you visit a retail supermarket, you will find that certain products are strategically positioned together for sales. For example, baby diapers and wipes, bread and butter, pizza base and cheese, beer, and chips are often placed close to each other. This strategic arrangement is based on market basket analysis, which helps identify associations among products frequently bought together by customers.

Market basket analysis is a versatile use case in the retail industry that enables businesses to optimize product placements, cross-sell items, and make personalized recommendations to customers, both in physical outlets and e-commerce platforms.

This project demonstrates how to perform Market Basket Analysis using the Apriori algorithm in Python. The Apriori algorithm is a classic technique for finding frequent itemsets and generating association rules from transactional data.

## Prerequisites

Before running the code, ensure you have the following installed:

- Python 3.x
- NumPy
- Pandas
- apyori (a library for the Apriori algorithm)

You can install the required libraries using `pip`:


## Dataset

The project uses the "Market_Basket_Optimisation.csv" dataset, which contains transactional data representing items purchased together by customers.

The dataset columns represent items purchased, and each row represents a separate transaction.

## Getting Started

1. Clone this repository:


2. Change the directory to the project folder:


3. Run the `market_basket_analysis.py` script:


## Project Structure

The project structure is as follows:

- `market_basket_analysis.py`: The main Python script that performs Market Basket Analysis using the Apriori algorithm.
- `Market_Basket_Optimisation.csv`: The dataset used for analysis.
- `README.md`: This README file.

## Results

After running the script, you will see the association rules mined from the dataset, along with their support, confidence, and lift values.

## Acknowledgments

The dataset used in this project is part of the "Market Basket Optimization" dataset available on the Kaggle platform.

## About the Author

This project was created by [Utkarsh Singh](https://github.com/utkarshx27). Feel free to contact me if you have any questions or suggestions.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
