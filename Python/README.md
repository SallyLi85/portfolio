# Business Tweets Text analysis and mining
Project background: This is a project I've worked on, with a focus on **<ins>non-structured<ins>** (text data in this project) data analysis. In this project, I applied multiple non-structured data processing methods and statistical modelling to understand the underlined patterns of the data. The application of **<ins>data encryption<ins>** is a good practice on how to work with sensitive/personal data. I used **<ins>Tableau<ins>** for data visualization in this project, and the relevant graphs are shown in this document.

## 1.Load required libraries and set up work directory
Load the necessary Python libraries required for the following analysis, and set up the work directory for this project so that all relevant analyses will be stored in the project folder.

## 2.Data Encryption
I used *cryptography* library in this project to encrypt sensitive and personal data, such as user_ID and file paths. By storing sensitive data in the key file and then reading it as an environment variable, this analysis is running without disclosing any personal/sensitive data.

## 3.Data cleaning
Several steps are applied in this stage to ensure data quality:

+ dataset splitting and merging
+ missing value checking and resolving
+ duplicated value checking and resolving

## 4.Text data pre-processing
Several steps are applied in this stage to make the text data digestible for statistical models and visualization software.

+ Remove stopwords(default & customized stopwords)
+ Remove non-characters (e.g. emojis :point_left:)
+ Text lemmatization >> reduce text to its most basic form
+ Frequency analysis to identify the most mentioned words/bi-grams/trigrams

<img width="424" height="280" alt="image" src="https://github.com/user-attachments/assets/3394da64-ab90-4617-a37d-79f80603e03c" />

## 5.Regression analysis to explore the correlation between user engagement and tweet sentiment level
By applying a linear regression model to this data set, the correlation among variables can be explored. OLS regression result shows that the correlation between tweet sentiment level and user engagement is statistically significant($R^2 = 0.283, p-value = 0$), and the correlation is positive (*coef = 0.6584*).

## 6.Explorative analysis of the correlation between user engagement and customer churn rate
By visualizing customer churn data and its tweet engagement data for the same time period, we can see that when the customer churn increases, the tweet engagement decreases. However, we cannot draw a concrete conslusion from this explorative analysis since there are other factors that aren't being considered here, plus not all users to engage with their tweets are their customers.

<img width="400" height="280" alt="image" src="https://github.com/user-attachments/assets/c96f7d2e-64a3-4dd3-a517-a0d96efbe6ef" />

<img width="400" height="280" alt="image" src="https://github.com/user-attachments/assets/6928e838-fd5d-4ef4-8efc-88376c85b74f" />

## 7.Business innovative area exploration
By doing frequency analysis on pre-processed text data, one innovation area was identified - **Charity**. It shows that this is an area/aspect that their customer pays attention. It indicates the business that more budget might be needed to allocate to relevant projects to increase customer retation rate and gain brand loyalty.
