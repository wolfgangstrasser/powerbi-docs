﻿<properties 
   pageTitle="Excel data in Power BI"
   description="Excel data in Power BI"
   services="powerbi" 
   documentationCenter="" 
   authors="Minewiskan" 
   manager="mblythe" 
   editor=""
   tags=""/>
 
<tags
   ms.service="powerbi"
   ms.devlang="NA"
   ms.topic="article"
   ms.tgt_pltfrm="NA"
   ms.workload="powerbi"
   ms.date="10/14/2015"
   ms.author="owend"/>
# Excel data in Power BI

You can use any XLSX Excel workbook - Excel 2007, 2010, and 2013 - as a dataset for your Power BI dashboards and reports. [Get your Excel data into Power BI](powerbi-service-get-data-from-files.md).

For the best results, your Excel workbook data:
-  is in table format. ( [Instructions for formatting Excel data as a table](https://support.office.com/article/Create-an-Excel-table-in-a-worksheet-e81aa349-b006-4f8a-9806-5af9df0ac664?ui=en-US&rs=en-US&ad=US))
-  is prepared as an Excel data model (typically created using Power Pivot). Don't worry if you don't know how to do this, it's not required.
-  has columns marked by data type (e.g, date, number). For more information:
	-   [data types in Excel data models](https://support.office.com/Article/Data-Types-Supported-in-Data-Models-e2388f62-6122-4e2b-bcad-053e3da9ba90)
	-   [formatting number data types in Excel](https://support.office.com/article/Format-numbers-f27f865b-2dc5-4970-b289-5286be8b994a)

This video demonstrates getting your Excel data ready for Power BI:

<iframe width="500" height="281" src="https://www.youtube.com/embed/l2wy4XgQIu0" frameborder="0" allowfullscreen></iframe>

## What is imported?

Power BI brings in:
-   **The data in the workbook** from worksheet tables or from the Excel data model. Data model content takes precedence over worksheet content.
-   **Power View sheets**, but not PivotTables or PivotCharts or custom fields. If your workbook has PivotTables or PivotCharts, consider [bringing the whole Excel file into Power BI](powerbi-bring-in-whole-excel-files.md) instead.

### Data types

Power BI recognizes values and supports these data types: Whole Number, Decimal Number, Currency, Date, True/False, Text).  Marking data as specific data types in Excel will improve the Power BI experience.

## Refreshing Excel data

-   When you upload an Excel workbook from your computer, you can't refresh the data. 
-   When you connect to an [Excel workbook in OneDrive](powerbi-service-refresh-excel-data-stored-in-onedrive.md), you can [refresh the data](powerbi-refresh-data.md).

## Troubleshooting

Currently, when you connect to an Excel workbook as a dataset, Power BI only imports data that is part of a named table or a data model. As a result:

-   If the workbook contains no named tables, Power View sheets, or Excel data models, you see this error. The article "[We couldn't find any data in your Excel workbook](powerbi-admin-troubleshoot-excel-workbook-data.md)" explains how to fix the workbook and reimport it.

See also

-  [Get data](powerbi-service-get-data.md)
-  [Get started with Power BI](powerbi-service-get-started.md) 
-  [Power BI - Basic Concepts](powerbi-service-basic-concepts.md)
