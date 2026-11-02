# House Price Data Analysis — Assignment 2, Part 3

## Project Overview
This project performs exploratory data analysis (EDA) on the supplied house sales training dataset. The dataset contains **1,460 houses and 81 variables**. The target variable is `SalePrice`.

The analysis explores the distribution of house sale prices and examines how selected property characteristics and neighborhood location are associated with sale price.

## Analysis and Visualizations

1. **Distribution of SalePrice** — A histogram with a KDE curve shows the distribution of house sale prices.
2. **Correlations with SalePrice** — A correlation analysis and heatmap examine relationships among selected numerical variables.
3. **Overall Quality and SalePrice** — A scatter plot explores the relationship between overall quality and sale price.
4. **Living Area and SalePrice** — A scatter plot explores the relationship between above-ground living area and sale price.
5. **Neighborhood and Average SalePrice** — A bar chart compares average sale prices across the ten neighborhoods with the highest mean prices.

## Key Findings

- The mean sale price is **$180,921**, while the median is **$163,000**. The distribution is right-skewed.
- `OverallQual` has the strongest positive correlation with `SalePrice` among the numerical variables examined (**r = 0.79**).
- `GrLivArea` is also strongly positively correlated with `SalePrice` (**r = 0.71**).
- `GarageCars`, `GarageArea`, and `TotalBsmtSF` also show positive correlations with sale price.
- Among the ten neighborhoods with the highest average sale prices, **NoRidge** has the highest average.

These are descriptive associations; correlation does not establish causation.

## Repository Structure

```text
Summer_HousePrice_Assignment2_Part3/
├── Data/
│   └── train.csv
├── Src/
│   └── Assignment_2_Part_3.ipynb
├── Docs/
│   └── Summer_Assignment_2_Part_3_Final_Report.pdf
├── Results/
│   ├── Distribution of House Sale Prices.png
│   ├── Correlation Matrix of Selected Variables.png
│   ├── Overall Quality vs Sale Price.png
│   ├── Above-ground Living Area vs Sale Price.png
│   └── Top 10 Neighborhoods by Average Sale Price.png
└── README.md
```

## Tools and Libraries

- Python
- Jupyter Notebook
- pandas
- NumPy
- Matplotlib
- Seaborn

## How to Run

1. Download or clone this repository.
2. Open `Src/Assignment_2_Part_3.ipynb` in Jupyter Notebook.
3. Run the notebook cells from top to bottom.
4. The notebook reads the dataset from `../Data/train.csv`.
5. Generated charts are saved in the `Results/` folder.

Install the required libraries if needed:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Final Report

The one-page PDF report is available in the `Docs/` folder.

## Data Quality and Limitations

The dataset contains missing values, particularly in `PoolQC`, `MiscFeature`, `Alley`, and `Fence`. The analysis uses the supplied training dataset and does not build a prediction model. Correlation measures linear association and does not prove causation.

## Author

Summer
