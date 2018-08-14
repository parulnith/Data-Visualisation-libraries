### `Steps`

> 1. Duplicate the Profit Map worksheet and name it Negative Profit Bar Chart.
> 2. In the Negative Profit Bar Chart worksheet, click Show Me and then select horizontal bars. Show Me highlights different chart types based on the data you've added to your view.
> 3. Multi-select the bars on the left by clicking and dragging your cursor across the bars between Tennessee, North Carolina, and Florida. On the tooltip that appears, select Keep Only to focus on those three states.
> 
>    > **`Learn More`**  
>    >
>    > **Creating Hierarchies**   
>    > Hierarchies come in handy when we want to group similar fields so that we can quickly drill down between levels in the viz.
>     >
>     > 1. In the Data pane, drag a field and drop it directly on top of another field or right-click the field and select 
>     > 2. Drag any additional fields into the hierarchy. You can also re-order fields in the hierarchy by dragging them to a new position.
>     > In the current viz. we will create the following hierarchies: Location, Order and Product.  
>     > ![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/Hierarchy.gif)
>     >
> 
> 4. On the Rows Shelf, click the plus icon on the `State `Field to drill-down to the `City` level of detail
> 5. That's a lot of data. We can use `N-Filter` to filter to reveal the poorest performers. From the Data pane, drag `City` to the Filters shelf. Click By field and then Click the `Top` drop-down and select `Bottom` to reveal the poorest performers. Type 5 in the text box to show the bottom 5 performers in the data set.
>     
> __We now see that Jacksonville and Miami, Florida; Burlington, North Carolina; and Knoxville and  Memphis, Tennessee are the poorest performing cities by profit.
There is one other mark in the view—Jacksonville, North Carolina—that doesn't belong, since it has profitable sales. This means there is an issue in the filter we applied. We will take the help of Tableau Order of Operations.__  

>  6. On the Filters shelf, right-click the Inclusions (Country, State) (Country, State) set and select Add to Context. We find that now Concord, North Carolina appears in view while Miami, Florida disappears which makes sense.  
>  7. But Jacksonville, North Carolina is still in the view which is incorrect. On the Rows shelf, click the plus icon on City to drill down to the Postal Code level of detail. Right-click the postal code for Jacksonville, NC, 28540, and then select Exclude.  
>  8. Drag Postal Code of the Rows shelf. This is the final view.  
>  ![](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/getting%20into%20details.png)


     
### `Hands On`

![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/getting%20into%20details.gif)
     
     
