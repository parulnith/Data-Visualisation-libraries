



# Data Visualisation with Tableau

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#our-goal-as-data-analysts-is-to-arrange-the-insights-of-our-data-in-such-a-way-that-everybody-who-sees-them-is-able-to-clearly-understand-their-implications-or-their-truths-and-how-to-act-on-them)Our goal as Data Analysts is to arrange the insights of our data in such a way that everybody who sees them is able to clearly understand their implications, or their truths and how to act on them.

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-is-the-widely-used-data-analytics-and-visualization-tool-that-many-consider-indispensable-for-data-science-related-work-its-drag-and-drop-interface-makes-it-easy-to-sort-compare-and-analyze-data-from-multiple-sources-including-excel-sql-server-and-cloud-based-data-repositories)Tableau is the widely used data analytics and visualization tool that many consider indispensable for data-science-related work. Its drag-and-drop interface makes it easy to sort, compare, and analyze data from multiple sources, including Excel, SQL Server, and cloud-based data repositories.

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#in-this-tutorial-we-will-learn-how-to-analyze-and-display-data-using-tableau-and-make-better-more-data-driven-decisions-this-tutorial-will-cover-the-following-topics)In this tutorial, we will learn how to analyze and display data using Tableau and make better, more data-driven decisions. This tutorial will cover the following topics:

-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#1-introduction-to-tableau)[1. Introduction to Tableau](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#introduction-to-tableau)
    
    -   Overview
    -   Installation
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#2-getting-started)[2. Getting Started](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#getting-started)
    
    -   Tableau Workspace
    -   Connecting to a Data Source
    -   Creating a view
    -   Refining the view
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#3-emphasize-the-results)[3. Emphasize the Results](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#emphasise-the-results)
    
    -   Adding Filters to the view
    -   Adding Colors to the view
    -   Key Findings
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#4-map-view)[4. Map View](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#map-view)
    
    -   Building a Map View
    -   Getting into details
    -   Identifying the Key points
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#5-dashboard)[5. Dashboard](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#dashboard)
    
    -   Creating a dashboard
    -   Adding Interactiveness
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#6-story)[6. Story](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#story)
    
    -   Building a Story
    -   Making a Conclusion
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#7-tableaus-integration-with-r-python--sql-server)[7. Tableau's integration with R, Python & SQL Server](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau_with_R,Python,SQL)
    
    -   Tableau & R
    -   Tableau & Python
    -   Tableau & SQL Server
-   #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#8-saving-the-work)[8. Saving the Work](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#saving)
    

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#1introduction-to-tableau)1.Introduction to Tableau

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#overview)Overview

[Tableau Software](https://www.tableau.com/)  is an American computer software company headquartered in Seattle, WA, USA. It generates interactive data visualization products which focused on BI. The company was established at Stanford University’s Department of Computer Science between 1997 and 2002.

The main products offered by tableau are:  [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Introduction%20to%20tableau/Tableau%20Product%20suite.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Introduction%20to%20tableau/Tableau%20Product%20suite.png)

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-desktop-tableau-public-and-tableau-online-all-offer-data-visual-creation-and-choice-depends-upon-the-type-of-work)**Tableau Desktop, Tableau Public, and Tableau Online**, all offer Data Visual Creation and choice depends upon the type of work

[![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Introduction%20to%20tableau/Tableau%20Products.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Introduction%20to%20tableau/Tableau%20Products.png)

> ### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#in-this-tutorial-we-will-be-working-with-tableau-desktop)In this tutorial, we will be working with Tableau Desktop.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#installation)Installation

Depending upon the choice of product, download the software on to the computer. The installation is a very straightforward process in which you need to accept the license agreement. You can verify the installation by clicking the Tableau Icon. If the following screen appears, you are good to go.

[![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Introduction%20to%20tableau/installation.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Introduction%20to%20tableau/installation.png)

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#2getting-started)2.Getting Started

In this section, we will learn some basic operations in Tableau to get acquainted with its interface.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-workspace)Tableau Workspace

The Tableau workspace consists of menus, a toolbar, the Data pane, cards and shelves, and one or more sheets. Sheets can be worksheets, dashboards, or stories. The image below highlights the major components of the workspace. However, more familiarity will be achieved once we work with actual data.

[![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/Tableau%20Workspace.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Tableau%20Workspace.png)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#connecting-to-a-data-source)Connecting to a Data Source

Before we can build a view and analyze our data, Tableau must be first connected to the intended data. Tableau supports connection to a wide variety of data, stored in a variety of places. For example, your data might be stored on your computer in a spreadsheet or a text file, or in a big data, relational, or cube (multidimensional) database on a server in your enterprise. Or, you might connect to public domain data available on the web such as U.S. Census Bureau information, or to a cloud database source, such as Google Analytics, Amazon Redshift, or Salesforce.

When you launch Tableau Desktop, the data connectors that are available to you are listed on the  `Connect`  pane, which is the left pane on the  `Start page`. File types are listed first, then common server types, or servers that you've recently connected to. Click  `More`  to see the complete list of data connectors you can use. Under  `Open`, you can open workbooks that you have already created. Under  `Sample Workbooks`, view sample dashboards and worksheets that come with Tableau Desktop. Under  `Discover`, find additional resources like video tutorials, forums, or the “Viz of the week” to get ideas about what you can build.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/connecting_to_dataource.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/connecting_to_dataource.gif)

For supported files and databases, Tableau provides built-in connectors that are built for and optimized for those types of data. If your file or database type is listed under Connect, use this named connector to connect to your data. If your file or database type is not listed, you might have the option of creating your own connection using Other Databases (ODBC) or Web Data Connector. Tableau provides limited support for connections that you create using either of these options

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#connecting-to-the-sample-superstore-data-set)Connecting to the  [Sample-Superstore data set](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/Data%20Visualisation%20with%20Tableau/Sample-Superstore%20.xls)

For convenience, let’s use the sample data set that comes with Tableau installation named sample superstore.xls.However, in this tutorial, we will download it from here and load it as an excel sheet. The data is that of a United States’ Superstore. It contains information about products, sales, profits, and so on that you can use to identify key areas for improvement within this fictitious company.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps)`Steps`

> 1.  Import the Data into tableau workspace from the computer.
>     
> 2.  Under the Sheets Tab, three sheets will become visible namely Orders, People, and Returns. However, we will focus only on Orders data. Double click on Orders Sheet and it opens up just like a spreadsheet.
>     
> 3.  We observe the first three rows of data looks a bit different and is not in the desired format. Here we make use of Data Interpreter, also present under Sheets Tab. By clicking on it we get a nicely formatted sheet. If you wish to view the exact changes that it made, click on Review the results, and choose the Orders tab in the opened Excel sheet. it will show, it simply removed the erroneous data.
>     

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-1)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/connectingToData2.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/connectingToData2.gif)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#creating-a-view)Creating a View

We will start by creating a simple chart. In this section, we will get to know our data and will start to ask questions about the data to gain insights There are some important terms that we will encounter in this section.

`Dimension`

`Measures`

`Aggregation`

Dimensions are qualitative data, such as a name or date. By default, Tableau automatically classifies data that contains qualitative or categorical information as a dimension, for example, any field with text or date values. These fields generally appear as column headers for rows of data, such as Customer Name or Order Date, and also define the level of granularity that shows in the view.

Measures are quantitative numerical data. By default, Tableau treats any field containing this kind of data as a measure, for example, sales transactions or profit. Data that is classified as a measure can be aggregated based on a given dimension, for example, total sales (Measure) by region (Dimension).

Row-level data rolled up to a higher category, such as the sum of sales or total profit. Tableau does this automatically so you can break data down to the level of detail that you want to work with.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-1)`Steps`

> 1.  Go to the worksheet. Click on the tab  `Sheet 1`  at the bottom left of the tableau workspace.
> 
> [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/creating%20a%20view.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/creating%20a%20view.png)
> 
> 2.  Once, you are in the worksheet, from Dimensions in the Data pane, drag Order Date to the Columns shelf.
> 
> _When you drag Order Date to the columns shelf, Tableau creates a column for each year in your data set. Under each column is an Abc indicator. This indicates that you can drag text or numerical data here, like what you might see in an Excel spreadsheet. If you were to drag Sales to this area, Tableau creates a cross-tab (like a spreadsheet) and displays the sales totals for each year._
> 
> 3.  From Measures, drag Sales to the Rows shelf.
> 
> _Tableau generates a chart with sales rolled up as a sum (aggregated). Total aggregated sales for each year by order date is displayed.Tableau always generates a line chart for a view that includes time (in this case Order Date)_

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-2)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/creating%20a%20view.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/creating%20a%20view.gif)

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#this-line-chart-shows-that-sales-look-pretty-good-and-seem-to-be-increasing-over-time-this-is-good-information-but-it-doesnt-really-tell-you-much-about-which-products-have-the-strongest-sales-and-if-there-are-some-products-that-might-be-performing-better-than-others-let-us-see-what-else-you-can-find-out)_This line chart shows that sales look pretty good and seem to be increasing over time. This is good information, but it doesn't really tell you much about which products have the strongest sales and if there are some products that might be performing better than others. Let us see what else you can find out._

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#refining-the-view)Refining the View

Let us delve deeper and try to find out more insights regarding which products drive more sales. Let's start by adding the product categories to look at sales totals in a different way.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-2)`Steps`

> 1.  From Dimensions, drag  `Category`  to the Columns shelf and place it to the right of  `YEAR(Order Date)`.The view updates to a bar chart. By adding a second discrete dimension to the view, data changes into discrete chunks instead of continuous. This creates a bar chart and shows the overall  `Sales`  for each  `Product`  category by year.
>     
>     > `Learn More`
>     
>     > 1.  To view information about each data point (that is, mark) in the view, hover over one of the bars to reveal a tooltip. The tooltip displays total sales for that category. Here is the tooltip for the Office Supplies category for 2017:
>     > 
>     > [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view1.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view1.png)  
>     > 2. To add data point information as labels to your view, click  `Show Mark Labels`  on the toolbar.
>     > 
>     > [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view2.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view2.png)
>     > 
>     > 3.  To display the bar chart horizontally instead of vertically, click Swap on the toolbar.
>     > 
>     > [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view3.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view3.png)
>     

> 2.  The view above nicely shows  `sales`  by  `category`  i.e furniture, office supplies, and technology. We can also infer that furniture sales are growing faster than sales of office supplies except for 2016. Hence it will be wise to focus sales efforts on furniture instead of office supplies. But furniture is a very broad category and consists of many different items. How can we identify which furniture item is contributing towards maximum sales?
> 
> #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#to-help-answer-that-question-we-decide-to-look-at-products-by-sub-category-to-see-which-items-are-the-big-sellers-for-example-for-the-furniture-category-you-want-to-see-details-about---bookcases-chairs-furnishings-and-tables-double-click-or-drag-the-sub-category-dimension-to-the-columns-shelf)**To help answer that question, we decide to look at products by  `sub-category`  to see which items are the big sellers. For example, for the Furniture category, you want to see details about bookcases, chairs, furnishings, and tables. Double-click or drag the Sub-Category dimension to the Columns shelf.**

> #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#the-sub-category-is-another-discrete-field-it-creates-another-header-at-the-bottom-of-the-view-and-shows-a-bar-for-each-sub-category-68-marks-broken-down-by-category-and-year-however-it-is-a-lot-of-data-to-visually-make-sense-of-in-the-next-section-we-will-learn-about-filters-color-and-other-ways-to-make-the-view-more-comprehensible)**The sub-category is another discrete field. It creates another header at the bottom of the view and shows a bar for each  `sub-category`  (68 marks) broken down by category and year. However, it is a lot of data to visually make sense of. In the next section, we will learn about filters, color and other ways to make the view more comprehensible.**

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-3)`Hands On`

[![Alt text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/getting%20started/Refining%20the%20viewgif.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20viewgif.gif)

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#3emphasise-the-results)3.Emphasise the Results

In this section, we will try to focus on specific results. Filters and colors are ways to add more focus to the details that interest us.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#adding-filters-to-the-view)Adding filters to the view

Filters can be used to include or exclude values in the view. Here we try to add two simple filters to the worksheet to make it easier to look at product sales by sub-category for a specific year.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-3)`Steps`

> In the Data pane, under Dimensions, right-click Order Date and select Show Filter.Repeat for Sub->category field also.  
> [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/Adding%20filter.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/Adding%20filter.png)
> 
> #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#filters-are-card-types-and-can-be-moved-around-on-the-canvas-by-clicking-on-the-filter-and-dragging-it-to-another-location-in-the-view)**Filters are card types and can be moved around on the canvas by clicking on the filter and dragging it to another location in the view**

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#adding-colors-to-the-view)Adding colors to the view

Colours can be helpful in the visual identification of a pattern.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-4)`Steps`

> In the Data pane, under Measures, drag Profit to Color on the Marks card.
> 
> [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/adding%20color%5C.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/adding%20color%5C.png)
> 
> #### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#it-can-be-clearly-seen-that-bookcases-tables-and-even-machine-contribute-to-negative-profit-ie-loss-a-powerful-insight)**It can be clearly seen that Bookcases, Tables and even machine contribute to negative profit i.e loss. A powerful insight.**

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-4)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/adding%20filter%20and%20color.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/adding%20filter%20and%20color.gif)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#key-findings)Key Findings

Let's take a closer look at the filters to find out more about the unprofitable products.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-5)`Steps`

> 1.  In the view, in the  `Sub-Category`  filter card, clear all of the check boxes except  `Bookcases, Machines,`  and  `Tables`. This throws an interesting fact. While in some years, Bookcases and Machines were actually profitable. However, in 2016, Machines became unprofitable.
> 2.  Select  `All`  in the  `Sub-Category`  filter card to show all sub-categories again.
> 3.  From Dimensions, drag  `Region`  to the  `Rows`  shelf and place it to the left of Sum(Sales). We notice that machines in the South are reporting a higher negative profit overall than in your other regions.
> 4.  Let us now give a name to the sheet. At the bottom-left of the workspace, double-click  `Sheet 1`  and type  `Sales by Product and Region`.
> 5.  In order to preserve the view, Tableau allows us to duplicate our worksheet so that we can continue in another sheet from where we left off.
> 6.  In your workbook, right-click the  `Sales by Product and Region`  sheet and select  `Duplicate`  and rename the duplicated sheet to  `Sales-South`.
> 7.  In the new worksheet, from Dimensions, drag  `Region`  to the  `Filters`  shelf to add it as a filter in the view.
> 8.  In the Filter Region dialogue box, clear all check boxes except South and then click  `OK`. Now we can clearly focus on sales and profit in the  `South`. We find that machine sales had a negative profit in 2014 and again in 2016. We will investigate this in the next section
> 9.  Lastly, do not forget to save the results by selecting  `File > Save As`. Give your workbook a name, like  `Regional Sales and Profits`.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-5)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/key%20findings.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Emphasize%20the%20Results%20/key%20findings.gif)

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#4map-view)4.Map View

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#creating-a-map-view)Creating a Map View

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#map-views-are-very-helpful-when-we-are-looking-at-geographic-data-the-region-field-in-the-current-example-tableau-automatically-recognizes-that-the-country-state-city-and-postal-code-fields-contain-geographical-information)**Map views are very helpful when we are looking at geographic data (the Region field). In the current example, Tableau automatically recognizes that the Country, State, City, and Postal Code fields contain geographical information.**

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-6)`Steps`

> 1.  Create a new worksheet.
> 2.  Add  `State`  and  `Country`  under Data pane to  `Detail`  on the Marks card. We obtain the map view.
> 3.  Drag  `Region`  to the  `Filters`  shelf, and then filter down to the  `South`  only. The map view zooms in to the South region, and there is a mark for each state.
> 4.  Drag the  `Sales`  measure to  `Color`  on the Marks card. We obtain a filled map with the colors pointing to the sales in each state.
> 5.  We can change the color scheme by clicking  `Color`  on the Marks card and selecting  `Edit Colors`. We can experiment with the available palettes.
> 6.  We observe that Florida is performing the best. Hovering over its mark reveals a total of 89,474 USD in sales, as compared to South Carolina, for example, which has only 8,482 USD in sales. Let us gauge the performance by  `Profit`  now since Profit is a better indicator than sales alone.
> 7.  Drag  `Profit`  to  `Color`  on the Marks card. We now see that Tennessee, North Carolina, and Florida have negative profit, even though it appeared they were doing good in Sales. Rename the sheet as Profit Map

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-6)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Map%20View/creating%20a%20map%20view.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/creating%20a%20map%20view.gif)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#getting-into-the-details)Getting into the details

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#maps-are-great-for-visualizing-the-data-broadly-in-the-last-step-we-discovered-that-we-discovered-that-tennessee-north-carolina-and-florida-have-a-negative-profit-in-this-section-let-us-draw-a-bar-chart-to-explore-the-reason-for-the-negative-profit)**Maps are great for visualizing the data broadly. In the last step, we discovered that we discovered that Tennessee, North Carolina, and Florida have a negative profit. In this section let us draw a Bar chart to explore the reason for the negative profit.**

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-7)`Steps`

> 1.  Duplicate the Profit Map worksheet and name it Negative Profit Bar Chart.
>     
> 2.  In the Negative Profit Bar Chart worksheet, click Show Me and then select horizontal bars. Show Me highlights different chart types based on the data you've added to your view.
>     
> 3.  Multi-select the bars on the left by clicking and dragging your cursor across the bars between Tennessee, North Carolina, and Florida. On the tooltip that appears, select Keep Only to focus on those three states.
>     
>     > **`Learn More`**
>     > 
>     > **Creating Hierarchies**  
>     > Hierarchies come in handy when we want to group similar fields so that we can quickly drill down between levels in the viz.
>     > 
>     > 1.  In the Data pane, drag a field and drop it directly on top of another field or right-click the field and select
>     > 2.  Drag any additional fields into the hierarchy. You can also re-order fields in the hierarchy by dragging them to a new position. In the current viz. we will create the following hierarchies: Location, Order and Product.  
>     >     [![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Map%20View/Hierarchy.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/Hierarchy.gif)
>     
> 4.  On the Rows Shelf, click the plus icon on the  `State`Field to drill-down to the  `City`  level of detail
>     
> 5.  That's a lot of data. We can use  `N-Filter`  to filter to reveal the poorest performers. From the Data pane, drag  `City`to the Filters shelf. Click By field and then Click the  `Top`  drop-down and select  `Bottom`  to reveal the poorest performers. Type 5 in the text box to show the bottom 5 performers in the data set.
>     
> 
> **We now see that Jacksonville and Miami, Florida; Burlington, North Carolina; and Knoxville and Memphis, Tennessee are the poorest performing cities by profit. There is one other mark in the view—Jacksonville, North Carolina—that doesn't belong, since it has profitable sales. This means there is an issue in the filter we applied. We will take the help of Tableau Order of Operations.**

> 6.  On the Filters shelf, right-click the Inclusions (Country, State) (Country, State) set and select Add to Context. We find that now Concord, North Carolina appears in view while Miami, Florida disappears which makes sense.
> 7.  But Jacksonville, North Carolina is still in the view which is incorrect. On the Rows shelf, click the plus icon on City to drill down to the Postal Code level of detail. Right-click the postal code for Jacksonville, NC, 28540, and then select Exclude.
> 8.  Drag Postal Code of the Rows shelf. This is the final view.  
>     [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Map%20View/getting%20into%20details.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/getting%20into%20details.png)

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-7)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Map%20View/getting%20into%20details.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/getting%20into%20details.gif)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#key-findings-1)Key Findings

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#let-us-now-focus-only-on-the-loss-making-entities-ie-the-products-and-also-let-us-identify-the-locations-where-such-products-are-sold)**Let us now focus only on the loss-making entities i.e the Products and also let us identify the locations where such products are sold.**

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-8)`Steps`

> 1.  Drag Sub-Category to the Rows shelf.
> 2.  Drag Profit to Color on the Marks card. This enables us to quickly spot products with negative profit.
> 3.  In the Data pane, right-click Order Date and select Show Filter.It seems that Machines, tables, and binders don’t seem to be doing well. So should we stop selling those items in Jacksonville, Concord, Burlington, Knoxville, and Memphis? Let's verify.
> 4.  Go back to the Profit Map sheet tab.
> 5.  On the Data pane, right-click Sub-Category and select Show Filter.
> 6.  From Measures, drag Profit to Label on the Marks card.
> 7.  On the Data pane, right-click Order Date and select Show Filter to provide some context for the view. Clear Binders, Machines, and Tables from the list on the Sub-Category filter card in the view.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-8)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Map%20View/key%20findings.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/key%20findings.gif)

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#5-dashboard-1)5. Dashboard

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#a-dashboard-is-a-collection-of-several-views-enabling-one-to-compare-a-variety-of-data-simultaneously)**A dashboard is a collection of several views, enabling one to compare a variety of data simultaneously.**

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#creating-a-dashboard)Creating a Dashboard

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-9)`Steps`

> 1.  Click the  `New dashboard`  button.
> 2.  Drag  `Sales in the South`  to the empty dashboard
> 3.  Drag  `Profit Map`  to the dashboard, and drop it on top of the Sales in the South view. Both views can be seen at once. To be able to present data in a manner so that others can understand it we can arrange the dashboard to our liking.
> 4.  On Sales in the South, right-click in the column area under the  `Region`column header, and clear  `Show`  Header. Repeat the same for  `Category`  row header. This helps to show only what is needed and hiding the unnecessary information.
> 5.  Right-click the  `Profit Map`  title and select  `Hide Title`. Repeat the same for  `Sales in the South`  view.
> 6.  Select the first  `Sub-Category`  filter card on the right side of your view, and at the top of the card, click the  `Remove`icon. Repeat this step for the second  `Sub-Category`  filter card and one of the  `Year of Order Date`  filter cards. Click the drop-down arrow at the top of the  `Year of Order Date`  filter, and select  `Single Value (Slider)`.Now let the magic unfold. Try selecting different years on the Year of Order Date filter and see how the data is quickly filtered to show that state performance varies year by year.
> 7.  Drag the  `SUM(Profit)`  filter and drag it at the bottom of the dashboard below Sales in South.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-9)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Dashboard/creating%20dashboard.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Dashboard/creating%20dashboard.gif)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#adding-interactiveness)Adding Interactiveness

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#in-order-to-make-the-dashboard-more-interactive-like-viewing-which-sub-categories-are-profitable-in-specific-states-few-changes-need-to-be-done)In order to make the dashboard more interactive like viewing which sub-categories are profitable in specific states, few changes need to be done.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-10)`Steps`

> 1.  Select  `Profit Map`  in the dashboard, and click the  `Use as filter`  icon in the upper right-hand corner
> 2.  Now if we select any state in the map, the Sales in the  `South chart`  updates to show just the sub-category sales.
> 3.  Select the  `Year of Order Date`  filter, click its drop-down arrow, and select  `Apply to Worksheets > Selected Worksheets`.
> 4.  In the  `Apply Filter to Worksheets`  dialog box, select  `All`  in the dashboard, and then click  `OK`. This is done in order to apply the filter to all worksheets in the dashboard that use this same data source.
> 5.  Now explore and experiment. In the viz. below we will filter  `Sales in the South`  to only items sold in North Carolina, and then explore year by year profit.
> 6.  Rename the Dashboard to  `Regional Sales and Profit`.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-10)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Dashboard/adding%20interactiveness.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Dashboard/adding%20interactiveness.gif)

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#thus-selling-machines-in-the-north-carolina-did-not-bring-any-profits-to-the-company)**Thus, selling machines in the North Carolina did not bring any profits to the company.**

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#6-story-1)6. Story

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#a-dashboard-is-a-cool-feature-but-tableau-also-offers-us-to-showcase-our-results-in-presentation-mode-in-form-of-stories-about-which-we-will-discuss-in-this-section)A dashboard is a cool feature but tableau also offers us to showcase our results in presentation mode in form of stories about which we will discuss in this section.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#building-a-story)Building a Story

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-11)`Steps`

> 1.  Click the  `New story`  button.
> 2.  From the Story pane on the left, drag the  `Sales in the South`  worksheet onto your view.
> 3.  Edit the text in the gray box above the worksheet. This is the caption. Name it as  `Sales and profit by year`.
> 4.  Stories are quite specific. Here we will tell a story about selling machines in North Carolina. In the Story pane, click  `Duplicate`  to duplicate the first caption.
> 5.  In the  `Sub-Category`, filter  `select`  only  `Machines`. This helps to gauge sales and profit of machines by year.
> 6.  Rename the caption to  `Machine sales and profit by year`.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-11)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Story/Buildign%20a%20story.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Story/Buildign%20a%20story.gif)

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#making-a-conclusion)Making a Conclusion

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#it-is-clear-that-machines-in-north-carolina-is-leading-to-loss-of-profit-however-this-cannot-be-demonstrated-by-looking-at-profit-and-sales-on-the-whole-for-this-we-need-regional-profit)It is clear that machines in North Carolina is leading to loss of profit. However, this cannot be demonstrated by looking at Profit and Sales on the whole. For thi,s we need regional Profit.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-12)`Steps`

> 1.  In the Story pane, select  `Blank`. Drag the dashboard  `Regional Sales and Profit`  onto the canvas.
> 2.  Caption it as  `Low performing items in the South`.
> 3.  Select  `Duplicate`  to Create another story point with your Regional Profit dashboard. Select North Carolina on the bar chart.
> 4.  Select All the years.
> 5.  Add a caption, for example,  `Profit in NC, 2013-2016`.
> 6.  Select any year like 2014. Add a caption, for example,  `Profit in NC, 2014`  and then click Duplicate. Repeat the same for all the remaining years.
> 7.  Click on the presentation mode and let the  `story`  unfold.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-12)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Story/making%20a%20conclusion.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Story/making%20a%20conclusion.gif)

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#now-we-have-an-idea-about-what-products-were-introduced-to-the-north-carolina-market-when-and-how-they-performed-not-only-have-we-identified-a-way-to-address-negative-profit-but-have-also-successfully-managed-to-back-it-with-datathis-is-the-advantage-of-story-in-tableau)Now we have an idea about, what products were introduced to the North Carolina market when, and how they performed. Not only have we identified a way to address negative profit, but have also successfully managed to back it with data.This is the advantage of Story in Tableau.

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#7-tableaus-integration-with-r-python--sql)7. Tableau's integration with R, Python & SQL

Apart from the various visualization advantages that Tableau offers, it also has an amazing out of the box connection capabilities. Tableau can easily integrate with languages like Python and R and also with DBMS like SQL. This offers increased advantages in terms of functionalities and comes in handy for Data Scientists who are used to working in Python or R. They can directly import the R and Python scripts in Tableau and take advantage of its visualisations which are far more superior than that of these languages. Also the visualisation capabilities of tableau are easy to use and very intuitive, thereby saving a lot of time for the Data Scientists.

In this section, we will see how we can connect Tableau with these external sources and the advantages of these connections.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-and-r)Tableau and R

R is a popular statistical language used to perform sophisticated analysis and predictive analytics, such as linear and nonlinear modeling, statistical tests, time-series analysis, classification, clustering, etc. Using Tableau in conjunction with R has the following advantages:

-   Gives Tableau users access to a rich, ever-expanding collection of statistical analysis and data mining libraries to help them gain deeper insights from their data.
-   Brings Tableau’s fluid data exploration experience and broad connectivity options to R users.
-   Enables consumers of Tableau worksheets and dashboards take advantage of R, simply by interacting with the visualization or widgets without the need to have any knowledge of the language.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#how-does-tableau-integrate-with-r)How does Tableau integrate with R?

R functions and models can be used in Tableau by creating new calculated fields that dynamically invoke the R engine and pass values to R. The results are then returned back to Tableau for use by the Tableau visualization engine.

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#setting-up-tableau-desktop-with-r)Setting up Tableau Desktop with R

-   **Download and Install  `Rserve`.**

You will need to download and install  `Rserve`  package for Tableau to connect and utilize the R script functions. In the R console, enter the following commands:

```
install.packages(“Rserve”) 
library(Rserve) ` 
Rserve() / Rserve(args = ‘ — no-save’)

```

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#connect-tableau-to-the-r-server)Connect Tableau to the R Server

Once  `Rserve`  is installed, open Tableau Desktop and follow the steps below

1.  Go to the  `Help > Settings and Preferences and select Manage External Service Connection`  [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Tableau%20with%20R/connection1.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Tableau%20with%20R/connection1.png)
    
2.  Enter a server name of “Localhost” (or “127.0.0.1”) and a port of “6311”.
    
3.  Click on the “Test Connection” button to make sure everything runs smoothly. You should see a successful message. Click OK to close.
    

[![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Tableau%20with%20R/connection2.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Tableau%20with%20R/connection2.png)

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#start-using-the-r-scripts-in-tableau)Start using the R scripts in Tableau

Upon successfully accomplishing the above steps, we will be able to create new calculated fields in Tableau Desktop that utilize the SCRIPT_* functions to make R functional calls.

Let’s get to work and see how we can use tableau capabilities with R.We will utilize the inbuilt Sample Superstore dataset to calculate Profit both by using R script and by Tableau ‘s drag and Drop feature. We will then compare both the results.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-13)`Steps`

> 1.  Open Tableau workbook and connect to the sample superstore data.
> 2.  Connect to Rserve. Once tableau desktop is connected to Rserve it can invoke R engine through calculated fields.
> 3.  We will now create a calculated field called Expected Profit.
> 
> There are four functions that are available for use with R and they all  
> begin with the word  **script.**  The functions are:
> 
> -   SCRIPT_REAL: returns Real numbers as results
> -   SCRIPT_STR: returns string
> -   SCRIPT_INT : returns integers
> -   SCRIPT_BOOL: returns booleans
> -   For this example, we are going to use the SCRIPT_REAL function. We are going to create a simple  `linear regression`  in Tableau.
> 
> 4.  Open up the calculated field and insert the following script.

```
SCRIPT_REAL("fit <- lm(.arg1 ~ .arg2 +  .arg3 + .arg4)
 fit$fitted
 ",
 SUM([Profit]),  AVG([Sales]),  AVG([Quantity]),   AVG([Discount]))

```

> The script above pertains to the linear regression model in R. This model will have one  **dependent variable(arg1) and**three  **independent**  variables(arg2, arg3, arg4)**. These arguments are just placeholders and when the script gets passed back to R, the arguments will be replaced with the tableau columns that they correspond to. 5. Input the tableau fields that correspond to each of the variables. The dependent variable here is profit so we’ll put  `SUM(Profit)`  first since that corresponds to argument 1. Similarly, we will use the  `average unit price, average order quantity`  and  `average discount`  for the other three arguments respectively.
> 
> 6.  These inputs will now all be pulled into the model for determining expected profit levels. We are now ready to use this calculation within Tableau visualizations. Drag category over onto the rows and then  `Profit`  onto columns. Now drag  `Expected Profit`  over onto the columns.
>     
> 7.  We can now analyze the model to see how the  **Expected profit calculated in R compares to the actual profits**. We can continue to analyze this further by pulling customer segments over onto the colors and now we’ve created a stacked bar chart can also utilize ordered dates to break out the data by years or by quarters.
>     

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-13)`Hands On`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Tableau%20with%20R/Tableau%20with%20R.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Tableau%20with%20R/Tableau%20with%20R.gif)

One might wonder all the above calculations could have been done in Tableau without using R. So, why should we go through the process of downloading and configuring Rserve in Tableau and write scripts? R is a very powerful language because of its power to easily forecast, utilising widely-used libraries that contain well-known algorithms.Imagine how nice it would be to make predictions for our business in Tableau, by calling a simple R script and then being able to incorporate it into Tableau's visualisations.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-and-python)Tableau and Python

Python is a widely used general-purpose programming language, and a large number of Python libraries are available to perform statistical analysis, predictive models or machine learning algorithms. Connecting Tableau with Python is one of the best approaches for predictive analytics. Tabpy is a package developed to do the same. Tableau can connect to the TabPy server to execute Python code on the fly and display results in Tableau visualizations.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#how-does-tableau-integrate-with-python)How does Tableau integrate with Python?

When we use TabPy with Tableau, we can define calculated fields in Python, thereby leveraging the power of a large number of machine-learning libraries right from our visualizations.

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#setting-up-tableau-desktop-with-python)Setting up Tableau Desktop with Python

**Download and Install  `Tabpy`.**

Running Python code within a Tableau workbook requires a Python server to execute it, and the TabPy framework gets the job done. Download TabPy from Github at the following  [link](https://github.com/tableau/TabPy/)  .Alternatively you can follow the steps below:

```
conda install -c anaconda tabpy-server

```

Then cd to the directory containing the downloaded tabpy server and run

```
python setp.py

```

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#connecting-tableau-with-tabpy)Connecting Tableau with TabPy

The next step is to connect Tableau with TabPy. This can be done  `in Help > Settings and Performance > Manage External Service Connection:`

[![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Tableau%20with%20Python/Tabpy%20connection.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Tableau%20with%20Python/Tabpy%20connection.png)

Test the connection and you should get a “successfully connected” prompt.

#### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#start-using-the-python-scripts-in-tableau)Start using the Python scripts in Tableau

This new Python integration in Tableau enables powerful scenarios. For example, it takes only a few lines of Python code to get the sentiment scores for reviews of products sold at an online retailer. Then one can explore the results in many ways in Tableau.Let us see this with an example

**Sentiment Analysis with Tabpy**

We will be using the mobile reviews dataset which can be downloaded from  [here](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/Data%20Visualisation%20with%20Tableau/reviews.csv).

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-14)`Steps:`

> 1.  Import the dataset into Tableau Desktop
> 2.  Connect to Tabpy. Once Tableau desktop is connected to  `Tabpy`  it can invoke Python engine through calculated fields.
> 3.  We will now create a calculated field called  `Sentiment`  as follows: `

```
SCRIPT_REAL("from vaderSentiment.vaderSentiment import  SentimentIntensityAnalyzer  
vs = []  
analyzer  = SentimentIntensityAnalyzer()  
for i in range(0,len(_arg1)):  
    a = analyzer.polarity_scores(_arg1[i])['compound']  
    vs.append(a)  
return vs",ATTR([Reviews]))`

```

> We are using the  `VADER sentiment analysis`  tool here. It is a lexicon and rule-based sentiment analysis tool that is  _specifically attuned to sentiments expressed in social media_.To use to this tool you will need to install it first.Please read more at their  [github page](https://github.com/cjhutto/vaderSentiment).
> 
> 4.  Now, drag  `Reviews`  onto rows and  `Sentiment`  onto  **Text and Color Marks card**  and see the magic happening. We get the sentiment analysis of the review done without any hassle. Also it gets super easy to visualise the results too .The positive reviews are in increasing order of green while the negative ones are in red.  [![](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Tableau%20with%20Python/Sentiment%20analysis.png)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Tableau%20with%20Python/Sentiment%20analysis.png)

Thus, we have seen how it takes only a few lines of Python code to get the sentiment scores for reviews of products sold at an online retailer. Then we can explore the results in many ways in Tableau.We might filter to see just the negative reviews and review their content to understand the reasons behind them or we might visualize overall sentiment changes over time.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-and-sql-server)Tableau and SQL Server

There is a hidden value in our Microsoft SQL Server data which lies buried under the standard reports and complex business intelligence tools.  **Tableau delivers insight everywhere by equipping anyone to do a sophisticated visual analysis of SQL Server data.**  We can connect Tableau to SQL Server live for tuned, platform-specific queries, or directly bring data into Tableau’s analytical engine to take the burden off the database.

Tableau provides an optimised, live connector to SQL Server so that we can create charts, reports, and dashboards while working directly with our data. As we dig into our analysis, Tableau recognises any schema used in SQL Server so we don’t have to manipulate our data.

Let us walk through an example depicting how to connect SQL server database to tableau Desktop and then use it to create visualisations.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#steps-15)`Steps:`

> 1.  Login to the SQL Server
> 2.  Open Tableau Desktop and under Servers, connect to MS SQL.
> 3.  Paste the server name in the dialog box that opens and click ok. This connects Tableau to the SQL Server. Select the database of choice.In this example we choose the salesDB. We can then select from a list of TABLES too eg Sales Log. The table gets imported into the Tableau environment .Now we can choose to extract the entire data or the portion of it to new worksheet. We can even specify the number of rows to extract.
> 4.  In the new worksheet we have the extracted data from MS SQL, From here we can work with it like any other Tableau Worksheet.

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#hands-on-14)`Hands On:`

[![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/raw/master/%20images%20and%20gifs/Tableau%20with%20SQL/Tableau%20with%20SQL.gif)](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Tableau%20with%20SQL/Tableau%20with%20SQL.gif)  This is how we can easily connect SQL Server to Tableau and extract the data directly into it . Tableau enables the users to toggle connections with a click to apply in-memory queries to a larger dataset.

# [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#8-saving-the-work-1)8. Saving the work

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-desktop)Tableau Desktop

To save a Tableau workbook locally, Select File > Save. Specify the workbook file name in the  `Save As`dialog box. Tableau saves the file with the .twb extension by default.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-public)Tableau Public

With Tableau Public all the views and data is made public and anybody on the internet has access to it.  `Select Server > Tableau Public > Save to Tableau Public`  and enter the credentials.

## [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#tableau-server)[Tableau Server](https://www.tableau.com/products/server)

In case the data is confidential and the story needs to be shared with the entire team, Tableau Server comes in handy. To publish a story to Tableau Server, Select  `Select Server > Publish Workbook`  or  `click Share`  on the toolbar. But make sure to create an account first.

----------

### [](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/README.md#thats-all-we-need-to-create-a-good-visualization-in-tableau-although-one-might-find-doing-a-lot-more-revising-in-each-stage-than-we-did-here-so-with-experimentation-and-practise-tableau-becomes-a-lot-more-familiar-and-will-unleash-amazing-features-to-help-us-analyze-and-present-data-please-comment-below-in-case-of-any-queries-or-questions-and-happy-visualising)That's all we need to create a good visualization in Tableau although, one might find doing a lot more revising in each stage than we did here. So with experimentation and practise, tableau becomes a lot more familiar and will unleash amazing features to help us analyze and present data. Please comment below in case of any queries or questions and Happy Visualising.





