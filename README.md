# Resume Parser

## Description
This project aims to parse resumes into different categories using machine learning techniques. It utilizes natural language processing (NLP) and classification algorithms to analyze the content of resumes and categorize them into various job fields.

## Installation
To run the code, first, ensure you have Python installed on your system. Then, follow these steps:

1. Install the required libraries by running:
```
!pip install kaggle
```
2. Set up your Kaggle API key by creating a `kaggle.json` file with your Kaggle username and API key. Place this file in the `~/.kaggle/` directory.

3. Download the dataset from Kaggle using the following command:
```
!kaggle datasets download -d jillanisofttech/updated-resume-dataset
```
4. Extract the downloaded dataset:
```
import zipfile
zip_ref = zipfile.ZipFile('/content/updated-resume-dataset.zip')
zip_ref.extractall('/content/updated-resume-dataset')
zip_ref.close()
```
5. Run the provided code snippets in a Python environment to execute the resume parsing and classification.

## Usage
Once the installation steps are completed, follow these instructions to use the resume parser:

1. Load the dataset and perform exploratory data analysis (EDA) to understand the structure and contents of the data.

2. Clean the resume text by removing URLs, special characters, and stopwords using the provided `cleanResume()` function.

3. Visualize the dataset to gain insights into the distribution of resumes across different categories.

4. Encode the categorical labels for training the machine learning model using label encoding techniques.

5. Train the model using the provided code snippets, which involve splitting the data into training and testing sets, extracting features from the resumes, and fitting a classification model (e.g., KNeighbors Classifier).

6. Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1-score.

## Features
- Dataset: The provided dataset contains resumes categorized into various job fields.
- Data Cleaning: Resumes are cleaned to remove irrelevant information and standardize the text format.
- Visualization: Visual representations (e.g., count plots, word clouds) provide insights into the dataset.
- Label Encoding: Categorical labels (job categories) are encoded for model training.
- Model Training: Machine learning models (e.g., KNeighbors Classifier) are trained to classify resumes into different categories.
- Testing and Evaluation: The model's performance is evaluated using classification metrics.

## Contributors
- Saksham Raj Gupta

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Acknowledgments
- Special thanks to [Kaggle](https://www.kaggle.com/) for providing the resume dataset.
- Inspired by similar projects and open-source contributions in the field of natural language processing and machine learning.
