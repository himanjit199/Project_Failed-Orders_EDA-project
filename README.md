


# Project: Failed Orders EDA

## Overview

This project involves an exploratory data analysis (EDA) of failed taxi orders for Gett, a technology platform for corporate Ground Transportation Management (GTM). The goal is to investigate and analyze the metrics related to orders that did not complete successfully, focusing on reasons for failure, hourly trends, time to cancellation, and estimated time of arrival (ETA).

## Data Description

### `data_orders.csv`
- **order_datetime**: Time of the order.
- **origin_longitude**: Longitude of the order's location.
- **origin_latitude**: Latitude of the order's location.
- **m_order_eta**: Time before order arrival (estimated).
- **order_gk**: Order number (unique identifier).
- **order_status_key**: Status of the order, where:
  - `4` - Cancelled by client.
  - `9` - Cancelled by system (rejected).
- **is_driver_assigned_key**: Indicates if a driver was assigned.
- **cancellation_time_in_seconds**: Time (in seconds) before cancellation.

### `data_offers.csv`
- **order_gk**: Order number (corresponds to `order_gk` in `data_orders`).
- **offer_id**: ID of an offer associated with the order.

## Assignment Tasks

1. **Distribution of Orders by Failure Reasons**
   - Analyze the distribution of orders based on reasons for failure: cancellations before and after driver assignment, and reasons for order rejection.
   - Plot the distribution and identify the category with the highest number of failed orders.

2. **Failed Orders by Hour**
   - Plot the distribution of failed orders by hour of the day.
   - Identify if certain hours have a higher proportion of specific failure categories.
   - Analyze the plot to determine which hours have the most significant number of failures and provide potential explanations.

3. **Average Time to Cancellation**
   - Plot the average time to cancellation (with and without driver) by hour.
   - Remove outliers if present and analyze the plot to draw conclusions about cancellation timings.

4. **Average ETA by Hour**
   - Plot the distribution of average ETA by hour of the day.
   - Provide explanations based on the plot to understand how ETA varies throughout the day.

## Methodology

The analysis was performed using Python in a Jupyter Notebook. Key libraries used include:
- `pandas` for data manipulation.
- `matplotlib` and `seaborn` for plotting and visualization.
- `numpy` for numerical operations.

## Results

1. **Failure Reasons Distribution**
   - The analysis revealed the most common reason for failed orders and its distribution.

2. **Hourly Distribution of Failures**
   - Insights into which hours experience the highest number of failed orders and potential reasons for these trends.

3. **Cancellation Time Analysis**
   - Insights into the average time to cancellation and the impact of driver assignment on cancellation timings.

4. **ETA Distribution**
   - Analysis of how average ETA varies throughout the day and possible explanations for observed trends.

## Files

- `data_orders.csv`: Data related to orders.
- `data_offers.csv`: Data related to offers.
- `Failed_Orders_EDA.ipynb`: Jupyter Notebook containing the analysis.

## Installation

To run the analysis, you need to have Python and the following libraries installed:
- `pandas`
- `matplotlib`
- `seaborn`
- `numpy`

You can install the required libraries using pip:

```bash
pip install pandas matplotlib seaborn numpy
```

## Usage

1. Clone the repository.
2. Place the `data_orders.csv` and `data_offers.csv` files in the project directory.
3. Open the `Failed_Orders_EDA.ipynb` notebook in Jupyter.
4. Run the notebook cells to perform the analysis.



## Acknowledgements

- Thanks to the data source for providing the opportunity to analyze real-world data.
- Special thanks to the open-source community for the tools and libraries used in this project.

---


 