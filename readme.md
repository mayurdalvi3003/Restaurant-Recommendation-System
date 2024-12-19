# Restaurant Recommendation System
## Overview
This project is a Restaurant Recommendation System built using Python. It utilizes restaurant reviews and metadata to recommend restaurants similar to a user's preference based on reviews and cuisines. The project processes a dataset containing restaurant information and implements natural language processing (NLP) techniques to enhance the recommendation accuracy.

## Features
- Data cleaning and preprocessing for structured and reliable input.
- Text processing to handle customer reviews effectively.
- Calculation of cosine similarity to identify similar restaurants.
- Custom recommendations based on restaurant names.
- Integration of cuisines, cost, and mean ratings in the recommendations.
## Dataset
The dataset used in this project contains:

Name
City
Type
Approximate cost
Online order availability
Booking table availability
Customer reviews and ratings
The dataset is stored locally and loaded for processing.
you can use the link mention below to download the dataset .
Link :- `https://www.kaggle.com/datasets/rishikeshkonapure/zomato`

## Technologies Used
- Programming Language: Python
- Libraries:
- Pandas
- Numpy
- NLTK
- TextBlob
- Scikit-learn
## Project Workflow
### 1.Data Loading:
- The dataset was loaded as a CSV file into a Pandas DataFrame.
### 2.Data Cleaning:
- Renamed columns for better readability.
- Converted the cost column to numeric and handled missing values.
- Processed the rate column to exclude invalid entries such as "NEW" and "-".
- Standardized boolean columns like online_order and book_table.
### 3.Text Preprocessing:
- Lowercased all reviews and removed stopwords using NLTK.
- Stripped URLs and irrelevant patterns from the text data.
### 4.Feature Engineering:
- Added a new column Mean Rating initialized to zero.
- Performed tokenization and vectorization of reviews using TfidfVectorizer.
### 5.Modeling:
- Calculated cosine similarity scores on processed reviews.
- Implemented a recommendation function to suggest restaurants based on similarity.
### Recommendation Output:
- Generated a list of similar restaurants with cuisines, cost, and ratings.
## Usage
### Clone the repository:
Copy code
`git clone https://github.com/your-username/restaurant-recommendation-system.git`

### Install the required dependencies:

pip install -r requirements.txt

## Output

Input the name of a restaurant to get similar recommendations.

Examples

Input: 'Pai Vihar'

Output:

List of top 7 restaurants similar to 'Pai Vihar' with their cuisines, cost, and ratings.

Input: 'Jalsa'

Output:

List of top 10 restaurants similar to 'Jalsa' with their cuisines, cost, and ratings.

## Future Enhancements
- Add geographical filtering to provide more localized recommendations.
- Integrate the system with a web or mobile interface.
- Enhance recommendation accuracy by using deep learning for sentiment analysis.

## Acknowledgments
Thanks to all contributors and open-source libraries that made this project possible.

