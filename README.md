# MedTourEasy-
Project on Analysis of Chemical Components




# README for Cosmetic Product Analysis Project

## Project Title
**Analysis of Chemical Components in Cosmetics**

## Overview
This project aims to create a content-based recommendation system for cosmetic products based on their chemical components. By analyzing ingredient lists from 1,472 cosmetic products available on Sephora, we utilize data science techniques to predict suitable products for consumers, particularly those with sensitive skin. The project includes data preprocessing, ingredient similarity analysis, and visualization using t-distributed Stochastic Neighbor Embedding (t-SNE) and the Bokeh library for interactive visualizations.

## Table of Contents
- [Project Description](#project-description)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Implementation Steps](#implementation-steps)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Project Description
The primary objective of this project is to assist consumers in making informed decisions when purchasing cosmetic products. The project achieves this by:
- Analyzing ingredient lists to identify similarities between products.
- Creating a recommendation system that suggests products based on ingredient compatibility.
- Visualizing the relationships between products using interactive plots.

## Dataset
The dataset used in this project is named **cosmetics.csv**, which contains the following columns:
- **Label**: Type of product (e.g., Moisturizer)
- **Brand**: Brand name of the product
- **Name**: Specific product name
- **Price**: Retail price of the product
- **Rank**: Product rating
- **Ingredients**: List of ingredients in the product
- **Combination**: Indicates suitability for combination skin (1 for yes, 0 for no)
- **Dry**: Indicates suitability for dry skin (1 for yes, 0 for no)
- **Normal**: Indicates suitability for normal skin (1 for yes, 0 for no)
- **Oily**: Indicates suitability for oily skin (1 for yes, 0 for no)
- **Sensitive**: Indicates suitability for sensitive skin (1 for yes, 0 for no)

### Sample Data
| Label       | Brand          | Name                         | Price | Rank | Ingredients                                                                                                      |
|-------------|----------------|------------------------------|-------|------|------------------------------------------------------------------------------------------------------------------|
| Moisturizer | LA MER         | Crème de la Mer              | 175   | 4.1  | Algae (Seaweed) Extract, Mineral Oil, Petrolatum, Glycerin, ...                                               |
| Moisturizer | SK-II          | Facial Treatment Essence      | 179   | 4.1  | Galactomyces Ferment Filtrate (Pitera), Butylene Glycol, Water, Sodium Benzoate, ...                          |
| Moisturizer | DRUNK ELEPHANT | Protini™ Polypeptide Cream    | 68    | 4.4  | Water, Dicaprylyl Carbonate, Glycerin, Cetearyl Alcohol, ...                                                  |

## Installation
To run this project, you will need the following software installed on your machine:
- Python 3.x
- Jupyter Notebook
- Required Python libraries: pandas, scikit-learn, bokeh, numpy, and matplotlib.

You can install the required libraries using pip:
```bash
pip install pandas scikit-learn bokeh numpy matplotlib
```

## Usage
1. Clone this repository to your local machine using:
   ```bash
   git clone https://github.com/yourusername/cosmetic-product-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd cosmetic-product-analysis
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open the notebook file (e.g., `cosmetic_analysis.ipynb`) and run the cells to execute the analysis.

## Implementation Steps
1. **Data Loading**: Load the cosmetics dataset into a pandas DataFrame.
2. **Data Preprocessing**: Clean the dataset by removing duplicates and handling missing values. Tokenize the ingredient lists for analysis.
3. **Vectorization**: Convert the ingredient lists into numerical format using TF-IDF or word embedding techniques.
4. **Dimensionality Reduction**: Apply t-SNE to reduce the dimensionality of the ingredient vectors for visualization.
5. **Visualization**: Create interactive scatter plots using Bokeh to visualize the relationships between different cosmetic products based on their ingredients.
6. **Recommendation System**: Develop a content-based recommendation system that suggests products based on ingredient similarities.

## Results
The analysis reveals distinct clusters of cosmetic products based on their ingredient similarities. The interactive visualizations allow users to explore the relationships between products, making it easier to identify suitable options based on individual skin types and preferences. The project empowers consumers by providing insights into the chemical components of cosmetics, enhancing their shopping experience.

## Future Work
Future enhancements for this project could include:
- Expanding the dataset to include more products and brands.
- Integrating user reviews and ratings for more personalized recommendations.
- Developing a web or mobile application for easier access to the recommendation system.
- Incorporating safety data about cosmetic ingredients to inform users about potentially harmful components.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Special thanks to the authors of the dataset and the libraries used in this project.
- This project was inspired by the need for informed decision-making in the cosmetics industry, particularly for individuals with sensitive skin.



