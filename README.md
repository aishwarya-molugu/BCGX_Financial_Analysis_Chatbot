# Financial Analysis of Tech Giants & Rule-Based Chatbot

## Project Overview

This project is a comprehensive financial analysis of three major technology companies—Apple (AAPL), Microsoft (MSFT), and Tesla (TSLA)—based on data extracted from their 10-K filings. The analysis involves data cleaning, calculation of key financial ratios, and visualization of trends.

The final output is an interactive, rule-based chatbot developed in Python that allows users to query the analyzed financial data in a user-friendly way. This project was completed as part of the **BCG GenAI Job Simulation on Forage**.

-----

## Key Features

  - 📊 **Data Extraction & Cleaning:** Manually extracted key financial metrics from 10-K reports and cleaned the data using the Pandas library.
  - 📈 **Financial Ratio Analysis:** Calculated and compared key ratios, including the Debt-to-Asset Ratio, Return on Assets (ROA), and Year-over-Year (YoY) growth for revenue and net income.
  - 📉 **Data Visualization:** Created bar charts using Matplotlib and Seaborn to visually compare the financial health and performance of the companies.
  - 🤖 **Interactive Chatbot:** Developed a rule-based chatbot that answers predefined questions about the financial data for a user-selected company.

-----

## Technologies Used

  - **Programming Language:** Python
  - **Libraries:** Pandas, Matplotlib, Seaborn
  - **Development Environment:** Jupyter Notebook

-----

## Setup and Installation

To run this project on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    https://github.com/aishwarya-molugu/BCGX_Financial_Analysis_Chatbot.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd BCGX_Financial_Analysis_Chatbot
    ```
3.  **Install the required libraries:**
    ```bash
    pip install pandas matplotlib seaborn jupyter
    ```

-----

## How to Run the Project

1.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
2.  **Open the Notebook:** In the Jupyter interface, open the `Financial_Analysis.ipynb` file.
3.  **Run the Analysis Cells:** Execute the cells in the notebook sequentially to load the data, perform the analysis, and generate the visualizations.
4.  **Run the Chatbot:** Execute the final cell in the notebook, which contains the `financial_chatbot()` function, to start the interactive chatbot in the command line.

-----

## Summary of Financial Analysis

This analysis examined the financial health and strategy of Apple, Microsoft, and Tesla.

### Apple (AAPL)

  * **Strategy:** Apple pursues a **high-leverage** strategy. It uses a significant amount of debt to finance its operations, as shown by a Debt-to-Asset ratio of approximately **84.4%**. Despite this high debt load, the company is extremely efficient at generating profit, leading its peers with a Return on Assets (ROA) of **25.7%**.
  * **Growth:** Apple's recent growth has shown signs of slowing. For the most recent fiscal year (2024), its revenue grew by a modest **2.0%**, while its net income saw a decline of **-3.4%**.

### Microsoft (MSFT)

  * **Strategy:** Microsoft employs a **balanced and stable** strategy. It maintains a moderate Debt-to-Asset ratio of around **44.5%**. This is coupled with a strong and consistent Return on Assets of **16.4%**, showcasing efficient and lower-risk profit generation.
  * **Growth:** Microsoft has demonstrated robust and consistent growth. In the most recent fiscal year (2025), it posted double-digit growth in both revenue (**14.9%**) and net income (**15.5%**).

### Tesla (TSLA)

  * **Strategy:** Tesla's strategy appears more conservative in its financing, with the lowest Debt-to-Asset ratio of the group at approximately **39.6%**. Its profitability, as measured by Return on Assets, was **5.8%**.
  * **Growth:** Tesla's growth story is the most dramatic. After a strong 2023, the most recent fiscal year (2024) saw a significant slowdown. Revenue growth was nearly flat at **0.9%**. More alarmingly, net income plummeted by **-52.7%**.

-----

## Chatbot Documentation

### How It Works

The chatbot is a Python script that operates in a logical sequence. It relies on the **pandas** library to hold the pre-analyzed financial data. When started, it greets the user and prompts them to select one of the three companies. It then enters a continuous `while True` loop to allow for multiple questions. The user's input is **normalized** (converted to lowercase, etc.) and checked against a series of hard-coded questions using an `if/elif/else` block. When a match is found, a helper function (`get_latest_value`) filters the DataFrame to find the correct data point and returns a formatted, user-friendly response.

### Predefined Queries

The chatbot can answer the following five questions:

1.  What is the most recent total revenue?
2.  What is the most recent net income?
3.  What is the Debt-to-Asset ratio?
4.  What is the Return on Assets?
5.  How did net income change last year?

### Limitations

  * The chatbot can only answer the five specific questions listed above.
  * The financial data is static and is not updated in real-time.
  * It cannot understand synonyms or different phrasings of the questions.

-----

## Acknowledgments

This project was developed as part of the **BCG GenAI Job Simulation** offered by **Forage**.
