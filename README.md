# HR-Dashboard
This project is based on ELT and ETL both
Power BI HR-Report – Dashboard (Detailed Document)
Get Data (connected Text CSV File)
ETL and ELT both were involved in stages
Power Query Interface or Power Query Editor (From transform option) in data there were 35 rows which should be converted in 35 columns by split columns option with by delimiter (Common delimiters include spaces, tabs, and commas, but any character or set of characters can be used as a delimiter. First row as header. Conditional columns
Created a new table as measure for adding information through additional columns. Used Data Analysis Expressions (DAX) on Power BI Desktop to create new measures.
Used DAX: COUNT, CALCULATE, Divide
Total Emp = COUNTROWS('HR Analytics Data')
Not Due = CALCULATE([Total Emp],'HR Analytics Data'[Promotion status]="not due")
MALE/FEMALE = CALCULATE([Total Emp],'HR Analytics DIVIDEData'[Gender]="MALE/FEMALE")
Active workers = CALCULATE([Total Emp],'HR Analytics Data'[Retirement]="on service")
Due Promotions for Male = CALCULATE('Table'[Male], 'HR Analytics Data'[Promtion Status]="due for Promotions")
Not Due = CALCULATE([Total Emp],'HR Analytics Data'[Promotion status]="not due")
% Female/Female = DIVIDE([Female/male],'Table'[Total Employees], 0)
For Employee details another table (Text CSV) was connected to get more data which made 1:1 relation with Employee number.
Connected with 1:1
Employee Number(from HR Analytics Data) : Employee Number(from HR Employee Data)
For Visualizations I chose some metrics from Selection features for columns e.g. meter, years, on service……..


![image](https://user-images.githubusercontent.com/100975167/227798161-7ac7284f-f8a7-43ef-8ac0-a1c76431a5f7.png)


