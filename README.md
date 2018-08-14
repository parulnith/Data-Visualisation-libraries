# <a name="getting-started"></a>2.Getting Started


In this section, we will learn some basic operations in Tableau to get acquainted with its interface.

## Tableau Workspace

The Tableau workspace consists of menus, a toolbar, the Data pane, cards and shelves, and one or more sheets. Sheets can be worksheets, dashboards, or stories. The image below highlights the major components of the workspace. However, more familiarity will be achieved once we work with actual data.

![](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Tableau%20Workspace.png)


## Connecting to a Data Source

Before we can build a view and analyze our data, Tableau must be first connected to the intended data. Tableau supports connection to a wide variety of data, stored in a variety of places. For example, your data might be stored on your computer in a spreadsheet or a text file, or in a big data, relational, or cube (multidimensional) database on a server in your enterprise. Or, you might connect to public domain data available on the web such as U.S. Census Bureau information, or to a cloud database source, such as Google Analytics, Amazon Redshift, or Salesforce.

When you launch Tableau Desktop, the data connectors that are available to you are listed on the **Connect** pane, which is the left pane on the **Start page**. File types are listed first, then common server types, or servers that you've recently connected to. Click **More** to see the complete list of data connectors you can use. Under **Open**, you can open workbooks that you have already created. Under **Sample Workbooks**, view sample dashboards and worksheets that come with Tableau Desktop. Under **Discover**, find additional resources like video tutorials, forums, or the “Viz of the week” to get ideas about what you can build.


### `Hands On `     

	  
![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/connecting_to_dataource.gif)

For supported files and databases, Tableau provides built-in connectors that are built for and optimized for those types of data. If your file or database type is listed under Connect, use this named connector to connect to your data. If your file or database type is not listed, you might have the option of creating your own connection using Other Databases (ODBC) or Web Data Connector. Tableau provides limited support for connections that you create using either of these options


#### Connecting to the [Sample-Superstore data set](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/Data%20Visualisation%20with%20Tableau/Sample-Superstore%20.xls)

For convenience, let’s use the sample data set that comes with Tableau installation named sample superstore.xls.However, in this tutorial, we will download it from here and load it as an excel sheet. 
The data is that of a United States’ Superstore. It contains information about products, sales, profits, and so on that you can use to identify key areas for improvement within this fictitious company.
