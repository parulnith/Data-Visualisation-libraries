# <a name="map-view"></a>4.Map View 

## Creating a Map View

#### **Map views are very helpful when we are looking at geographic data (the Region field). In the current example, Tableau automatically recognizes that the Country, State, City, and Postal Code fields contain geographical information.**

### `Steps`

> 1. Create a new worksheet.
> 2. Add `State` and `Country` under Data pane to  `Detail` on the Marks card. We obtain the map view.
> 3. Drag `Region` to the `Filters` shelf, and then filter down to the `South` only. The map view zooms in to the South region, and there is a mark for each state.
> 4. Drag the `Sales` measure to `Color` on the Marks card. We obtain a filled map with the colors pointing to the sales in each state.
> 5. We can change the color scheme by clicking `Color` on the Marks card and selecting `Edit Colors`. We can experiment with the available palettes.
> 6. We observe that Florida is performing the best. Hovering over its mark reveals a total of 89,474 USD in sales, as compared to South Carolina, for example, which has only 8,482 USD in sales. Let us gauge the performance by `Profit` now since Profit is a better indicator than sales alone.
> 7. Drag `Profit` to `Color` on the Marks card. We now see that Tennessee, North Carolina, and Florida have negative profit, even though it appeared they were doing good in Sales. Rename the sheet as Profit Map


### `Hands On`

![Alt Text](https://github.com/parulnith/Data-Visualisation-with-tableau/blob/master/%20images%20and%20gifs/Map%20View/creating%20a%20map%20view.gif)

