# Analyze A/B Test Results - DAND03
This repository contains a Jupyter Notebook analyze_ab_test_results.ipynb that demonstrates an analysis of an A/B test run by an e-commerce website. The goal of this analysis is to help the company understand if they should:
1. Implement the new webpage,
1. Keep the old webpage, or
1. Run the experiment longer to make their decision.

## Table of Contents
The Jupyter Notebook is divided into three main parts, and a conclusion:
1. Probability
1. A/B Test
1. Regression
1. Conclusions

## Libraries Used
The following libraries are used in this project:
* pandas
* numpy
* random
* matplotlib

## Data
The data used in this project is stored in ab_data.csv. The data contains 5 columns:
* user_id: Unique ID (int64)
* timestamp: Time stamp when the user visited the webpage
* group: In the current A/B experiment, the users are categorized into two broad groups. The control group users are expected to be served with old_page; and treatment group users are matched with the new_page. However, some inaccurate rows are present in the initial data, such as a control group user is matched with a new_page. ['control', 'treatment']
* landing_page: It denotes whether the user visited the old or new webpage. ['old_page', 'new_page']
* converted: It denotes whether the user decided to pay for the company's product. Here, 1 means yes, the user bought the product. [0, 1]
