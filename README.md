# Predicting Midwest Consumer Sentiment
Miami University Farmer School of Business

ISA 514 Project

Team Members: Aaron Black, Jackson Chlebowy, Logan Loftus, Maguire Sheppard

Professor: Dr. Jay Shan

## Project Overview

In a period marked by persistent inflation and shifting consumer behavior, understanding public sentiment toward prices has become a critical challenge for economists, businesses, and policymakers alike. Price volatility directly impacts the budgets of millions of families, influences consumer support and confidence, and shapes policy decisions at the government level. Understanding what economic factors exactly drive changes in consumer sentiment can provide individuals with answers to commonly overlooked behavioral and emotional patterns in response to inflation. Developing a predictive model that integrates economic and behavioral data can help explain how people perceive and react to the constantly changing prices at the store. By comparing these patterns with consumer price indexes and predicting sentiment analysis, our project addresses the gap between economic data and public perception, creating a more responsive, forward-looking understanding of consumer attitudes.

## Contents of the Repository

- Executive summary document

- Structured Economic data used in the analysis

- Unstructured Reddit sentiment data used in the analysis

- Python scripts to merging data and conducting analysis

- Final presentation

## Steps to Follow to Replicate our Analysis

All files required to replicate our analysis are included in this repository. All .ipynb files were developed and saved using a Jupyter Notebook web-based IDE- more specifically, a university-hosted JupyterHub server.

To gain an initial understanding of the project and the problem addressed in this analysis,  please refer to the document **Excecutive Summary - ISA 514 Project_ Predicting Consumer Sentiment (1).pdf**. 

After defining the business problem and domain of interest, the next step is to collect relevant data and prepare the collected data  into clean, structured datasets. The economic data that which serve as predictors in this analysis was collected from the BLS and BEA, these files can be found in **Economic Data.zip**. Next step is to combine these various datsets of data gathered from various sources into one dataset, refernced as **Master_df.csv**, the coding steps and documentation are done in the codebook **Combining_datasets.ipynb**. 

As the goal of our analysis is to predict consumer sentiment in the Midwest, relevant data representing this prediction target must be collected and prepared. The collection steps are taken in the codebook **RedditCleaned.ipynb**. This codebook contains the code used to scrape Reddit posts related to the economy from the five Midwest states of Ohio, Wisconsin, Indiana, Illinois, and Michigan. It uses the VADER sentiment analyzer to perform sentiment analysis on the post titles, and exports the results into .csv files for each state. The resulting datasets are stored in  the zip folder called **Reddit Files.zip** containing Ohio_2015-2025.csv, Wisconsin_2015-2025.csv, Indiana_2015-2025.csv, Illinois_2015-2025.csv, and Michigan_2015-2025.csv. Similar to how the predictor datasets were combined, the multiple datasets including the target at the state level must be combined into one dataset,  the steps taken to merge are shown in **MidwestCleaned.ipynb**. The resulting dataset is the final merged dataset for modeling called **ModelData.csv**.

Now that all the collected data has been prepared for modeling, the next step is to build machine learning models that provide a data-driven solution to the proposed business problem. The codebooks **Logistic Regression.ipynb** and **Random Forest.ipynb** document our modeling processes. These codeebooks contain the code used to train, and evaluate the respective machine learning models designed to predict consumer sentiment in the Midwest. 


Lastly, all work and insights were organized into a slide deck that was presented to the class. The presentation file is in a pdf format named **Presentation. Consumer Sentiment - ISA 514 Group 3A.pdf**, and contains a summary our methodology, process, modeling approach, and key findings, and serves as the final deliverable of the project.

