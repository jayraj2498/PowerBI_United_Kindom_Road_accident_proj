## This project demonstrates the creation of a comprehensive Road Accident Analyssis of United Kingdom dashboard using Power BI. It covers data extraction from a SQL database, data processing and DAX queries, dashboard design, and sharing insights. The project aims to provide real-time insights into Road Accident , enabling to monitor and analyze performance efficiently.  


- Devlope Comprehensive Road Accident  provides real time weekly insight  
- insight into key performance matrix and trend 
- Enable to stasck honder to moniter and analyze Road Accident  operation effectively wrt to Wheather condition and Road surface conditions 


## 1. Project objective
## 2. Data from SQL
## 3. Data processing & DAX
## 4. Dashboard & insights
## 5. Export & share project

### Project Objective

- To develop a comprehensive road Accident Analysis  dashboard that
provides real-time insights into key
performance metrics and trends,
enabling  to monitor
and analyze  operations
effectively.

### step. 1 import dta from sql   

### step.2 load data tables from sql 

### step. 3 Data processing and DAX queries   
- Month = FORMAT(Calender_of_date[Date],"mmm")

- Month number = MONTH(Calender_of_date[Date])

- Year = YEAR(Calender_of_date[Date]) 

- CY Accident count = TOTALYTD(COUNT(Data[Accident_Index]), Calender_of_date[Date])

- CY Casualties = TOTALYTD(SUM(Data[Number_of_Casualties]),Calender_of_date[Date])

- PY Accidents = CALCULATE(COUNT(Data[Accident_Index]),SAMEPERIODLASTYEAR(Calender_of_date[Date])) 

- PY Casualties = CALCULATE(SUM(Data[Number_of_Casualties]),SAMEPERIODLASTYEAR(Calender_of_date[Date]) )

- YOY Accidents = ([CY Accident count]-[PY Accidents])/[PY Accidents] 

- YOY Casualties = ([CY Casualties]-[PY Casualties])/[PY Casualties]

#### we ake these dashbord wrt week and week 


Project Insights- 2 Year data 2021-22 

- • Total CY year Casuality 51 k 

- • Total CY year Accident  36 k 

- • Overall revenue is 57M

- • Total CY year Fatal Casulity  0.8 k 

- • Total CY year Serious Casulity  6718 

- • Total CY Slight  Casulity  43 K 

- • Most Casualities in Urban area 

- •  Most Casualities Day Light 

- • Most Casualities by road type Single carriageway 


 



