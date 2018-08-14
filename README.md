## Creating a View

We will start by creating a simple chart. In this section, we will get to know our data and will start to ask questions about the data to gain insights There are some important terms that we will encounter in this section.

| ` Dimension`      | `Measures`          | `Aggregation`|
| -------------     |:-------------:      |  -----------:|
| Dimensions are qualitative data, such as a name or date. By default, Tableau automatically classifies data that contains qualitative or categorical information as a dimension, for example, any field with text or date values. These fields generally appear as column headers for rows of data, such as Customer Name or Order Date, and also define the level of granularity that shows in the view.     | Measures are quantitative numerical data. By default, Tableau treats any field containing this kind of data as a measure, for example, sales transactions or profit. Data that is classified as a measure can be aggregated based on a given dimension, for example, total sales (Measure) by region (Dimension). | Row-level data rolled up to a higher category, such as the sum of sales or total profit. Tableau does this automatically so you can break data down to the level of detail that you want to work with. |

###  `Steps`

> 1. Go to the worksheet. Click on the tab `Sheet 1` at the bottom left of the tableau workspace.
> 
>  ![](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/creating%20a%20view.png)
> 
> 2. Once, you are in the worksheet, from Dimensions in the Data pane, drag Order Date to the Columns shelf.
>
> *When you drag Order Date to the columns shelf, Tableau creates a column for each year in your data set. Under each column is an Abc indicator. This indicates that you can drag text or numerical data here, like what you might see in an Excel spreadsheet. If you were to drag Sales to this area, Tableau creates a cross-tab (like a spreadsheet) and displays the sales totals for each year.*
> 
> 3. From Measures, drag Sales to the Rows shelf.
>
> *Tableau generates a chart with sales rolled up as a sum (aggregated). Total aggregated sales for each year by order date is displayed.Tableau always generates a line chart for a view that includes time (in this case Order Date)*




### `Hands On `  

![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/creating%20a%20view.gif)

#### *This line chart shows that sales look pretty good and seem to be increasing over time. This is good information, but it doesn't really tell you much about which products have the strongest sales and if there are some products that might be performing better than others. Let us see what else you can find out.*

