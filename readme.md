# Kaggle Open Dataset: Brewery Operations and Market Analysis Dataset

This project was completed as the final Phase 5, Capstone assessment in the Flatiron School’s Data Science Bootcamp. 

Analysis by Erin Wasserman, July 2024

# Overview

This dataset presents an extensive collection of data from a craft beer brewery, spanning from January 2020 to January 2024. It encapsulates a rich blend of brewing parameters, sales data, and quality assessments, providing a holistic view of the brewing process and its market implications.

# Business Problem


# Data Understanding

**Dataset Description**

[Kaggle Dataset](https://www.kaggle.com/datasets/ankurnapa/brewery-operations-and-market-analysis-dataset/data) <br>

Data Format and Structure:
-The dataset is structured in a tabular format, provided in a CSV file for easy integration with various data analysis tools.
-It comprises over 10 million records, each representing a unique batch with a comprehensive set of features.

Intended Audience:
This dataset is invaluable for data scientists, brewing process engineers, market analysts, supply chain experts, and quality control professionals in the brewing industry. It is also highly relevant for academic research in food technology, fermentation science, and business analytics.

Disclaimer:
-The data is synthetic and intended for educational, analytical, and simulation purposes.
-Users are advised to apply appropriate data processing and analysis techniques for meaningful insights.
-This comprehensive dataset serves as a rich resource for exploring the intricacies of brewing science, market dynamics, and operational efficiency in the craft beer industry.

**Highlighted Data Features**

Brewing Parameters: Includes crucial brewing factors such as fermentation time, temperature, pH level, gravity, and ingredient ratios. These parameters are pivotal in understanding the brewing process and its impact on the final product.

Beer Styles: The dataset categorizes beers into various styles like IPA, Stout, Lager, etc.

Quality Scores: Each batch is rated for its quality on a scale, offering insights into the success and consistency of different brewing approaches.

Application:
Brewing Process Optimization: Ideal for analysis aiming to correlate brewing techniques with beer quality, facilitating the optimization of brewing conditions for superior product quality.

**Data Splits**

-Use the following code to create a reproducible subset of the larger [Kaggle Dataset](https://www.kaggle.com/datasets/ankurnapa/brewery-operations-and-market-analysis-dataset/data) <br>
 
# Load the CSV file
input_csv_path = 'C:YOUR Path\\brewery_data_complete_extended.csv'  # Replace 'YOUR Path' with your input CSV file path
output_csv_path = 'C:YOUR Path\\beer_sample_set.csv'  # Replace 'YOUR Path' with your desired output CSV file path

# Read the CSV file
df = pd.read_csv(input_csv_path)

# Calculate the number of rows to extract
num_rows_to_extract = int(len(df) * 0.025)

# Extract the first 10% of the rows
beer_subset_df = df.iloc[:num_rows_to_extract]

# Save the extracted rows to a new CSV file
beer_subset_df.to_csv(output_csv_path, index=False)

print(f'The first 2.5% of the CSV has been saved to {output_csv_path}')

- The dataset was randomly split into training (80%) and test (20%) sets to evaluate model performance.

**Data Licensing and Usage**

- [Database: Open Database, Contents: Copyright Original Authors](https://creativecommons.org/licenses/by-nc/4.0/)

# Methodology

## Data Preparation

**Data Cleaning and Preprocessing**

## Modeling

# Evaluation

## Limitations

# Key Findings

## Actionable Insights

## Next Steps

# Author

Name: Erin Wasserman

GitHub: [Cellister](https://github.com/cellister)

Email address: cellister at gmail .com

# Repository Structure

* **Notebook**

The [Google Colab Notebook](https://github.com/cellister/Automated_Essay_Scoring/blob/main/automated_essay_scoring_06_18.ipynb), is the key deliverable and contains the details of my data strategy, methodology, data cleaning, visualizations, and actionable insights. [notebook PDF](https://github.com/cellister/Automated_Essay_Scoring/blob/main/Project_PDFs/automated_essay_scoring_notebook.pdf)

* **Presentation**

This 5-7 minute, non-technical [presentation PDF](https://github.com/cellister/Automated_Essay_Scoring/blob/main/Project_PDFs/automated_essay_scoring_presentation.pdf) was made in [Canva](https://www.canva.com/design/DAGH1bsu130/EECBDNF5RDqHKnpQhlo84g/edit?utm_content=DAGH1bsu130&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton) and gives an impactful and brief overview of the key insights and recommendations. 

* **Data**

The data used in this analysis can be found in the [Kaggle Dataset](https://www.kaggle.com/competitions/learning-agency-lab-automated-essay-scoring-2/data).

```

├── Images
│   ├── tf_idf_kmeans
│   ├── tf_idf_nn
│   ├── BERT
│   ├── general
├── Reference
│   ├── Kaggle_official
│   ├── Notebooks
│   ├── mac_environment P4P.yml
│   ├── mac_environment.yml
├── Project_PDFs
│   ├── automated_essay_scoring_presentation.pdf
│   ├── automated_essay_scoring_notebook.pdf
│   └── AES_github_repository.pdf
├── .gitignore
├── automated_essay_scoring_6_XX.ipynb
└── README.md
```


