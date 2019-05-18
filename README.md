
# CitiBike

This application provides an analysis and visualization of CitiBike Usage in the Jersey City Area.

# Technologies Used

* Tableau
* Python for Data Munging

# Reference

* GitHub: https://github.com/daddyjab/CitiBike
* Data Munging (Jupyter Notebook): https://github.com/daddyjab/CitiBike/blob/master/Citibike_Exploration_JAB.ipynb
* Visualization (on Tableau Public): https://public.tableau.com/profile/jeffery.brown#!/vizhome/CitiBike_with_Paths_Idle_Time_JAB_v5/StoryCitiBike
* Tableau file (tbwx): https://github.com/daddyjab/CitiBike/blob/master/CitiBike_with_Paths_Idle_Time_JAB_v5.twbx

# Contributions

* Jeffery Brown: Designed and implemented all code and visualations for this application.
* Data:
    * Citi Bike System Data: https://www.citibikenyc.com/system-data

# Summary

This application provides a visualization of CitiBike usage data for Jersey City, New Jersey for the month of 2/2019.

Data Munging was performed using Python to clean the dataset and prepare it for use within Tableau.  This included:



| Figure 1: CitiBike - Data Munging in Python with Jupyter Notebook |
|----------|
<figure class="video container"> <iframe src="https://github.com/daddyjab/CitiBike/blob/master/Citibike_Exploration_JAB.ipynb" width="90%"> </iframe> </figure>

| Figure 1: CitiBike - Data Munging in Python with Jupyter Notebook |
|----------|
| ![Screenshot](docs/StockReports-Screenshot.png "Figure 1: StockReports - Input Data and Results") |

# Design

Figure 2 below shows the general design/flow of the application code.

* The main function `ProcessAllWorksheets` loops through each worksheet in the workbook that contains Stock data.
* The function `CalcStockMetrics` loops through each stock in the list of stock data, uses the `FindTickerIndex` function to manage a list of unique stock tickers for the output table, and tallies needed max/min and volume information.  This loop also updates the overall results table information.  Finally, the function uses functions `PopCalcTableHeader` and `PopCalcTableRow` to create the per-stock and overall results tables on the worksheet being processed.

| Figure 2: StockReports - Design |
|----------|
| ![Design Diagram](docs/StockReports-Design.png "Figure 2: StockReports - Design") |

