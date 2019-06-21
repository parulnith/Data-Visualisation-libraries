
## Quadrant Analysis in Tableau

#### Learn how to analyse data in the form of a dynamic quadrant chart in Tableau.

Exploratory data analysis forms the backbone of any data science project. Before proceeding with the model creation and training the dataset on any machine learning algorithm, it is essential that the dataset is explored nicely to get an overview of what’s in it.

Consider the famous Superstore dataset. The data is that of a United States Superstore and contains information about products, sales, profits, and so on that you can use to identify key areas for improvement within this fictitious company. The first step would be to import the dataset and explore it. You can download the data from [here](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/Sample-Superstore%20.xls).

### Python for EDA

Let’s use Python to import the dataset and explore it.

 

    import pandas as pd  
    import numpy as np
    superstore_data = pd.read_excel('Sample-Superstore .xls',header = 3)  
    superstore_data.head()
    
![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/df.head%28%29.png)

The dataframe shows the first five rows of the dataset containing different attributes. We can also see if there are any missing values and the different columns:

    superstore_data.info()

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/df.info%28%29.png)

The information above shows that there are no null values and a total of 9994 records. Visualisation is also an important part of EDA since it gives a better perspective. We could create a scatter plot between Sales and Profit but what if there was a way to further modify the existing scatter plot to give us more information? One such way of visualising information is through a **Quadrant Chart**. Let’s understand more about it in the next few sections and create one of our own.


##  Quadrant Analysis Chart

If you are a part of the Data Science ecosystem, you must have heard about the [Gartner’s Magic Quadrant](https://www.gartner.com/imagesrv/research/methodologies/magic_quad_faq.pdf)(MQ). These MQs are a series of reports containing the market research and analysis of several technology companies. As a matter of fact, they are one of the most anticipated and awaited reports in this space. Here is the [2019 Magic Quadrant](https://www.qlik.com/us/gartner-magic-quadrant-business-intelligence) for Analytics and Business Intelligence Platforms which shows that Tableau and PowerBI are leading the way.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/GartnerMQ.png)


A Quadrant chart is technically a scatter plot that is divided into four equal sections or quadrants and hence the name. A Quadrant Analysis chart helps to represent the data in separate quadrants so that it becomes easy to locate which data points are similar and which are not, based on certain characteristics.



## Creating Quadrant Charts in Tableau

[Tableau](https://www.tableau.com/) is a great data analytics and visualization tool used widely in the industry today. Tableau’s ease of use comes from the fact that it has a drag and drop interface. As a result, it makes it very easy and intuitive to create a plethora of plots and quadrant charts is one of them.

#### Pre-requisites

This article assumes some familiarity with Tableau, its properties and how it is used to do the analysis. In case you are a complete beginner, it is suggested that you go through the following article which serves as a good introduction to Tableau:

[**Data Visualisation with Tableau**](https://www.datacamp.com/community/tutorials/data-visualisation-tableau)


## Tableau Environment

In this tutorial, we will be working with [**Tableau Public**](https://public.tableau.com/en-us/s/)  which is an absolutely free offering from Tableau. Download the Tableau Public edition from the [official website](https://public.tableau.com/en-us/s/). Follow the installation instructions and if the following screen appears on clicking the Tableau Icon, you are good to go.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Tableau%20Environment.png)

## Connecting to Data Source

We’ll use the same Superstore dataset that had been described earlier. In case you haven’t download the dataset, you can find it [here](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/Sample-Superstore%20.xls).

-   Import the Data into Tableau workspace from the computer.
-   Under the Sheets Tab, three sheets will become visible namely Orders, People, and Returns. However, we will focus only on the Orders data. Double click on `Orders` Sheet and it opens up just like a spreadsheet.
-   We observe that the first three rows of data look a bit different and is not in the desired format. We shall use Data Interpreter, also present under Sheets Tab, to rectify this. By clicking on it we get a nicely formatted sheet.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/connecting%20to%20data%20source.gif)


## Creating a Scatter Plot

Let’s say we want to see how Discount is related to Profits of the Superstore and which products are more profitable than the other. The first step is to create a simple scatterplot between Discount and Profit Ratio. `Profit Ratio` gives a better sense than the field Profit alone and since it doesn’t exist in the original database, we shall create one.

-   Open up a new worksheet and create a new calculated field called `Profit Ratio` by using the formula mentioned below.

    ```sum([Profit])/sum([Sales])```

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/creating%20scatter%20plot.gif)

-   Drag `Discount` to Columns  and  `Profit Ratio`  to Rows. Finally, drag the `Sub Category`on to the Colors Shelf. Convert the Measure of Discount to Average from Sum. You get a scatter plot which is coloured by the different products.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/creating%20scatter%20plot1.png)


##  Creating Parameters

Now that we have a basic scatter plot, it’s time to create the two parameters which will act as the basis on which the Quadrants will be calculated. In our case, we shall create a `Discount Parameter` and a `Profit Ratio Parameter` which will be derived from the Discount and Profit Ratio Fields respectively.

#### Discount Parameter

Click on the Discount field > **Create** > **Parameter** and fill in the values as shown in the figure below. Set the Current Value to **the point of the data of your choice** (in this example 0.2).

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/creating%20Parameters.png)

#### Profit Ratio Parameter

Perform the same steps as above using the Profit Ratio field.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Profit%20Ratio%20Parameter.png)

A new heading called Parameters is now visible in the worksheet where both of our calculated parameters appear.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Parameters.png)


##  Adding Reference Lines

A Reference line in Tableau is simply a vertical or horizontal line in a graph that represents a point of reference. For instance, a reference line drawn on a Sales chart can easily differentiate between high and low sales points. We shall be creating two reference lines, one for each axis.

-   Right click on the `Profit Ratio axis` (y) and select **Add Reference Line**.
-   Set the Reference line Value to the `Profit Ratio` Parameter.
-   Leave the other fields with their default values and click **OK**.
-   Right click on the `Avg Discount` axis (x) and select **Add Reference Line**.
-   Set the Reference line Value to the `Avg Discount` Parameter.
-   Leave the other fields with their default values and click **OK**.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Refrence%20lines1.gif)


##  Assigning a colour to every Quadrant

We now have our four quadrants but the data points in every quadrant is randomly coloured which doesn’t help us in visualising which data point falls in which quadrant. We can write a simple calculation that assigns a colour to a data point based on their quadrant i.e UPPER RIGHT, UPPER LEFT, BOTTOM RIGHT or BOTTOM LEFT.

-   Click **Analysis** > **Create calculated field** and name the field as Quadrant **Color**.
-   Enter the formula as mentioned below:

    ```
    IF AVG([Discount]) >= [Discount Parameter]  
    AND [Profit Ratio] > [Profit Ratio Parameter] THEN 'UPPER RIGHT'  
    ELSEIF AVG([Discount]) < [Discount Parameter]   
    AND [Profit Ratio] > [Profit Ratio Parameter] THEN 'UPPER LEFT'  
    ELSEIF AVG([Discount]) >[Discount Parameter]   
    AND [Profit Ratio] < [Profit Ratio Parameter] THEN 'BOTTOM RIGHT'  
    ELSE 'BOTTOM LEFT'  
    END

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Quadrant%20color%20formula.gif)

-   The data points currently have been coloured by the Sub-category. However, we want to colour them with their respective quadrants. Simply drag the `Sub-Category` field on to the Detail card and `Quadrant Color` field on to the colour. Instantly all data points are now coloured with respect to the quadrant in which they fall. Change the `Shape` to circle to get filled circles and adjust the size and tooltip preferences accordingly.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Quadrant%20color%20settings.gif)

So here we have a Quadrant Analysis of the Discount and Profit Ratio of an American Superstore. It is pretty evident from the graph that products which lie in the `Bottom Right`are the least profit-making products while the ones lying in the `Upper Left` are the most profitable ones.


## Creating Dynamic Quadrant Chart

The quadrants in the above chart are fixed and can only be changed once we change the values of the linked Reference lines. What if we want to experiment with different thresholds to see how the products change their quadrants in real time? This is actually possible and is referred to as a dynamic quadrant chart and is achieved through the `Actions.`

#### Actions

Actions is a feature in Tableau that lets us add interactivity to the data. With the help of this feature, we can interact with our visualisation by either selecting, clicking or hovering on them. Actions can perform the following tasks in a visualisation:

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/actions.png)

Let’s now set up a worksheet action with the following steps:

-   Goto **Worksheet>Actions** and add `Change Parameter` action. This is because we want to create an action that changes the parameters accordingly.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/creating%20Parameter%20actions.png)

-   Next, we will name the action as `Update Discount Parameter` and select the corresponding `Target Parameter` and `Value` which in this case would be `Discount Parameter` and `AVG(Discount)` respectively.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Update%20Discount%20Parameter.gif)

-   Similarly, create another action called as `Update Profit Ratio Parameter`.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/Update%20Profit%20ratio%20parameter.gif)

Now as you click on a data point, it becomes the centre of the Quadrant. Thus what you now get is a dynamic Quadrant chart and you can easily see how changing the values of Profit Ratio and Discount changes the position of products in the quadrant.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/Quadrant%20Analysis%20in%C2%A0Tableau/images/dynamic%20quadrant%20chart.gif)



### Conclusion

In this article, we learnt how to convert a scatter plot to an interactive Quadrant Chart. Quadrant chart normally helps to have a general overview of data and understand how similar and dissimilar the objects are. From here you can proceed with the normal data analysis either in **R** or **Python to** further do some sales forecasting for coming months and analyse the data to identify important features in the dataset that actually drive the sales.

