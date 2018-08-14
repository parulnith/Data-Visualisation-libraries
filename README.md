## Refining the View


Let us delve deeper and try to find out more insights regarding which products drive more sales. Let's start by adding the product categories to look at sales totals in a different way.

###  `Steps`


> 1. From Dimensions, drag `Category` to the Columns shelf and place it to the right of `YEAR(Order Date)`.The view updates to a bar chart.By adding a second discrete dimension to the view, data changes into discrete chunks instead of continuous. This creates a bar chart and shows the overall `Sales` for each `Product` category by year.
>
>   `Learn More` 
    
    1. To view information about each data point (that is, mark) in the view, hover over one of the bars to reveal a tooltip. The tooltip displays total sales for that category. Here is the tooltip for the Office Supplies category for 2017:
    
     ![](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view1.png)
     2. To add data point information as labels to your view, click `Show Mark Labels` on the toolbar. 
    
       ![](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view2.png)
    
    3. To display the bar chart horizontally instead of vertically, click Swap on the toolbar.
    
     ![](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20view3.png)

> 2. The view above nicely shows `sales` by `category` i.e furniture, office supplies, and technology. We can also infer that furniture sales are growing faster than sales of office supplies except for 2016. Hence it will be wise to focus sales efforts on furniture instead of office supplies. But furniture is a very broad category and consists of many different items. How can we identify which furniture item is contributing towards maximum sales?
> 
> #### **To help answer that question, we decide to look at products by `sub-category` to see which items are the big sellers. For example, for the Furniture category, you want to see details about   bookcases, chairs, furnishings, and tables. Double-click or drag the Sub-Category dimension to the Columns shelf.**
 
> #### **The sub-category is another discrete field. It creates another header at the bottom of the view and shows a bar for each `sub-category` (68 marks) broken down by category and year. However, it is a lot of data to visually make sense of. In the next section, we will learn about filters, color and other ways to make the view more comprehensible.**

### `Hands On `  

![Alt text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/getting%20started/Refining%20the%20viewgif.gif)

