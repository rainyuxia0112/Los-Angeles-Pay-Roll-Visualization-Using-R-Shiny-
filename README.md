# Los Angeles Pay Roll Visualization Using R Shiny 
Demo(webapp):https://yuxiarain.shinyapps.io/LA-City-Payroll/

Use tidyverse and bash to explore following two data sets.

## Q1 LA City Employee Payroll

The `/home/m280data/la_payroll/City_Employee_Payroll.csv` file on teaching server contains payroll information of LA City employees in years 2013-2018. It was downloaded from [LA City Controller's Office](https://controllerdata.lacity.org/Payroll/City-Employee-Payroll/pazn-qyym). Make a Shiny app to facilitate visualization of this data.


1. **Total payroll by LA City**. Visualize the total LA City payroll of each year, with breakdown into base pay, overtime pay, and other pay.

  **See datapreprocessing.R**

2. **Who earned most?** Visualize the payroll information (total payment with breakdown into base pay, overtime pay, and other pay, Department, Job Title) of the top $n$ highest paid LA City employees in a specific year. User specifies $n$ (default 10) and year (default 2017).

  **See datapreprocessing.R**

3. **Which departments earn most?** Visualize the mean or median payroll, with breakdown into base pay, overtime pay, and other pay, of top $n$ earning departments. User specifies $n$ (default 5), year (default 2017), and method (mean or median, default median).

  **See datapreprocessing.R**

4. **Which departments cost most?** Visualize the total payroll, with breakdown into base pay, overtime pay, and other pay, of top $n$ expensive departments. User specifies $n$ (default 5) and year (default 2017).

  **See datapreprocessing.R**

5. Visualize any other information you are interested in.

  **Answer: I have chosen to visualize the distribution of the employment type of employees in each year with pie charts displaying percents of employees who worked full-time, part-time, or event employees.**

6. Publish your Shiny app to <https://www.shinyapps.io> and share the link.

  https://yuxiarain.shinyapps.io/LA-City-Payroll/

## Q2 LA City Parking War

The SQLite database `/home/m280data/la_parking/LA_Parking_Citations.sqlite` on teaching server contains information about parking tickets in LA City. It was downloaded from [LA Open Data Portal](https://data.lacity.org/A-Well-Run-City/Parking-Citations/wjz9-h9np). Connect to the database and answer following questions using plots and summary statistics. In this exercise, you are **not** allowed to load whole data into memory. Use the _transform in database, plot in R_ strategy.

1. How many tickets are in this data set? Which time period do these tickets span? Which years have most data?

  **Answer: There are 7656418	tickets in total within the data set. The tickets span from 01:00 on 07/02/2015 to 23:00 on 01/25/2019. 2017 has the most citation tickets.**

2. When (which hour, weekday, month day, and month) are you most likely to get a ticket and when are you least likely to get a ticket?

  **Answer: The most likely time to receive tickets is 12 PM while the least likely time to receive tickets is 5AM. The most likely weekday to receive tickets is Wednesday while the least likely weekday to receive tickets is Monday. The most likely day to receive tickets is 13th of the month while the least likely day to receive tickets is the 31st of the month. The most likely month to receive tickets is August while the least likely weekday to receive tickets is February.**

3. Which car makes received most citations?

  **Answer: TOYT had the most tickets.**

4. How many different colors of cars were ticketed? Which color attracted most tickets?

  **Answer: There are 103 different colors, and BK attracted the most tickets.**

5. What are the most common ticket types?

  **Answer: NO PARK/STREET CLEAN, METER EXP., RED ZONE, and PREFERENTIAL PARKING are the most common types of citation.**

6. How much money was collected on parking tickets in 2016, 2017 and 2018?

  **Answer: 152145538 dollars in 2016; 157122489	dollars in 2017; and 138875787 dollars in 2018.**

7. If you've been ticketed in LA County, did you find your ticket in this data set?

  **Answer: I did not receive a ticket in LA County.**

8. Read the blog <http://www.brettrics.com/9-million-parking-tickets-la/> and try to reproduce plots using your data. [pdf](./What\ 9\ Million\ Parking\ Tickets\ Says\ About\ Los\ Angeles\ ·\ Brettrics.pdf)
