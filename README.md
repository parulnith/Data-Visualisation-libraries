# <a name="dashboard"></a>5. Dashboard


#### **A dashboard is a collection of several views, enabling one to compare a variety of data simultaneously.**

## Creating a Dashboard

### `Steps`
 
> 1. Click the `New dashboard` button.
> 2. Drag `Sales in the South` to the empty dashboard
> 3. Drag `Profit Map` to the dashboard, and drop it on top of the Sales in the South view. Both views can be seen at once. To be able to present data in a manner so that others can understand it we can arrange the dashboard to our liking.
> 4. On Sales in the South, right-click in the column area under the `Region `column header, and clear `Show` Header. Repeat the same for `Category` row header. This helps to show only what is needed and hiding the unnecessary information.
> 5. Right-click the `Profit Map` title and select `Hide Title`. Repeat the same for `Sales in the South` view.
> 6. Select the first `Sub-Category` filter card on the right side of your view, and at the top of the card, click the `Remove` icon. Repeat this step for the second `Sub-Category` filter card and one of the `Year of Order Date` filter cards. Click the drop-down arrow at the top of the `Year of Order Date` filter, and select `Single Value (Slider)`.Now let the magic unfold. Try selecting different years on the Year of Order Date filter and see how the data is quickly filtered to show that state performance varies year by year. 
> 7. Drag the `SUM(Profit)` filter and drag it at the bottom of the dashboard below Sales in South.

### `Hands On`
 
 ![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Dashboard/creating%20dashboard.gif)  
    


## Adding Interactiveness 

#### In order to make the dashboard more interactive like viewing which sub-categories are profitable in specific states, few changes need to be done.


### `Steps`

> 1. Select `Profit Map` in the dashboard, and click the `Use as filter` icon  in the upper right-hand corner
> 2. Now if we select any state in the map, the Sales in the `South chart` updates to show just the sub-category sales.
> 3. Select the `Year of Order Date` filter, click its drop-down arrow, and select `Apply to Worksheets > Selected Worksheets`.
> 4. In the `Apply Filter to Worksheets` dialog box, select `All` in the dashboard, and then click `OK`. This is done in order to apply the filter to all worksheets in the dashboard that use this same data source.
> 5. Now explore and experiment. In the viz. below we will filter `Sales in the South` to only items sold in North Carolina, and then explore year by year profit.
> 6. Rename the Dashboard to `Regional Sales and Profit`.


### `Hands On`
    
![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Dashboard/adding%20interactiveness.gif)   


#### **Thus, selling machines in the North Carolina did not bring any profits to the company.** 

