
# Football Predictions and Web Scraping Project

This project aims to build and use a football match prediction model by gathering and analyzing data on teams, players, and match results. It consists of two key components: data gathering through web scraping and predictive modeling for match outcomes. 

## Table of Contents
- [Project Overview](#project-overview)
- [Installation](#installation)
- [Data Collection](#data-collection)
- [Football Prediction Model](#football-prediction-model)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)

## Project Overview

This project is divided into two main parts:
1. **Data Collection**: Gathering football-related data from various websites using web scraping.
2. **Prediction Model**: Developing a machine learning model to predict match results based on historical data.

The project uses Jupyter notebooks for code organization and documentation, with Python libraries like `requests`, `BeautifulSoup`, and `scikit-learn`.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Football-Predictions.git
   cd Football-Predictions
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter notebooks:
   ```bash
   jupyter notebook
   ```
   
## Data Collection

The web scraping component, located in the `4_Webscrapping.ipynb` notebook, is responsible for gathering football data from various sources. It focuses on fetching the following information:
- Team statistics
- Player information
- Match outcomes and scores

### Key Details:
- **Scraping Libraries**: Uses `requests` to handle HTTP requests and `BeautifulSoup` to parse HTML.
- **Data Cleaning**: Once scraped, the data undergoes preliminary cleaning and structuring to make it suitable for analysis.

To start the data scraping process:
1. Run each cell sequentially in the `4_Webscrapping.ipynb` notebook.
2. Scraped data will be saved in the specified output files, ready to be used in the prediction model.

**Note**: Be mindful of the website’s terms of service when scraping data. Use delays and limit requests to avoid potential bans.

## Football Prediction Model

The prediction model, developed in the `4_Football Predictions.ipynb` and `Football Predictions.ipynb` notebooks, uses the scraped data to predict the outcomes of future football matches.

### Steps:
1. **Data Preparation**: Data is preprocessed to remove inconsistencies and null values, and features are engineered to enhance model performance.
2. **Feature Selection**: Important features are selected based on correlation and significance tests.
3. **Model Building**: Several machine learning models, such as Logistic Regression, Random Forest, and SVM, are evaluated.
4. **Performance Evaluation**: Models are assessed using accuracy, precision, recall, and F1-score metrics to identify the best-performing model.

The output of the model is a prediction on match results (e.g., Win, Lose, or Draw), which can assist in decision-making or serve as a tool for sports enthusiasts.

## Usage

1. **Web Scraping**: Open `4_Webscrapping.ipynb` and run the cells to scrape and save data.
2. **Prediction Model**: 
   - Open `4_Football Predictions.ipynb` or `Football Predictions.ipynb`.
   - Ensure the required data from the scraping step is available.
   - Execute the cells to train and evaluate the model.

Example of running the prediction pipeline:

```python
# Assuming the data has already been collected and preprocessed

# Train the model
train_model(data)

# Predict upcoming matches
predictions = predict_matches(upcoming_data)
```

## Dependencies

The project requires the following Python libraries:
- `requests`
- `BeautifulSoup4`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`
- `jupyter`

Ensure all dependencies are installed by running:
```bash
pip install -r requirements.txt
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

