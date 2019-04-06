----------

## Data Visualisation with PowerBI

#### Learn how to analyze and display data using Power BI and make better, more data-driven decisions.

  
Our goal as Data Analysts is to arrange the insights of our data in such a way that everybody who sees them is able to understand their implications andacts on them accordingly.

[Power BI](https://powerbi.microsoft.com/en-us/) is a cloud-based business analytics service from Microsoft that enables anyone to visualise and analyze data, with better speed and efficiency. It is a powerful as well as a flexible tool for connecting with and analysing a wide variety of data. Many businesses even consider it indispensable for data-science-related work. Power BI’s ease of use comes from the fact that it has a drag and drop interface. This feature helps to perform tasks like sorting, comparing and analyzing, very easily and fast. Power BI is also compatible with multiple sources, including Excel, SQL Server, and cloud-based data repositories which makes it an excellent choice for Data Scientists.

#### This tutorial will cover the following topics:

 -  [ Overview of Power BI](#overview)
 -  [Advantages of using Power BI](#advantages)
 -  [PowerBI Desktop](#powerbi_desktop)
 -  [Getting Started](#getting_started)
 -  [Transforming Data](#transforming_data)
 -  [Report Creation](#report)
 -  [Building a Dashboard](#dashboard)
 -  [Power BI’s integration with R & Python](#r_and_python)
 -  [Saving and Publishing](#saving)
 -  [Conclusion](#conclusion)

----------

## <a name = "overview"></a>1. Overview of PowerBI

### Overview

[Power BI](https://powerbi.microsoft.com/en-us/) gives the ability to analyze and explore data on-premise as well as in the cloud. Power BI gives the ability to collaborate and share customized dashboards and interactive reports across colleagues and organisations, easily and securely.

![](https://cdn-images-1.medium.com/max/800/1*jWt7QPw7x86-BmiDMm3l_w.png)

[Source](https://docs.microsoft.com/en-us/learn/modules/get-started-with-power-bi/1-introduction)


### Power BI’s Components

Power BI consists of various components which are available in the market separately and can be used exclusively.

![](https://cdn-images-1.medium.com/max/800/1*QZ0k9tHvzI98YSCce8mSHQ.png)

[Content Source](https://en.wikipedia.org/wiki/Power_BI)

Choosing which component to work with depends mainly on the project or a team. We, however, will be working with **Power BI desktop** since this is component used mainly for Business reports generation and desktop creation. Also, all the other works normally begin with Power BI desktop, where the report creation takes place.

----------

## <a name = "advantages"></a>2. Advantages of using Power BI

Power BI provides certain advantages which makes it superior to the existing analytical tools:

-   Provides a cloud-based as well as a desktop interface.
-   Provides capabilities like data warehousing, data discovery and interactive dashboards.
-   Ability to load custom visualisations, and
-   Easily scalable across the entire organization.

----------

##  <a name = "powerbi_desktop"></a>3. Power BI Desktop

Power BI is a free application that can be downloaded and installed on the system. It can be connected to multiple data sources. Normally, an analysis work begins in **Power BI Desktop** where report creation takes place. The report is then published to **Power BI service** from where it can be shared to the **Power BI Mobile apps** so that people can view the reports even on mobiles.

  

![](https://cdn-images-1.medium.com/max/800/1*SZGJXc9mPw3P_EguKtiJUg.png)

Source: [https://docs.microsoft.com/en-us/learn/modules/get-started-with-power-bi/2-using-power-bi](https://docs.microsoft.com/en-us/learn/modules/get-started-with-power-bi/2-using-power-bi)

### Installation

Power BI only runs on Windows Machines. Mac users could spin up a Windows VM in Azure and load Power BI onto that or use [Turbo.net](https://turbo.net/run/powerbi/powerbi), which can stream Power BI to the Mac directly from the cloud.

Power BI can be used in two ways:

-   As an app from the Microsoft store and just sign in to get started. This is the online version of the tool.
-    [Download](https://www.microsoft.com/en-us/download/details.aspx?id=45331) the software locally and then install it. Make sure you read all the installation instructions.

Depending upon the choice of product, download the software on to the computer. After accepting the license agreement, verify the installation by clicking the Power BI Icon/App. If the following screen appears, you are good to go.

![](https://cdn-images-1.medium.com/max/800/1*9g4z7xVvx_6s6sMa0mXnEw.png)

----------

## <a name = "getting_started"></a>4.Getting Started

Let us now get an idea about working with Power BI Desktop. In this section, we shall explore it a bit to get accustomed to its interface.

### Power BI Workspace

The image below highlights the major components of the workspace of Power BI.

![](https://cdn-images-1.medium.com/max/800/1*T5vOMi8AaPcJB3spA870IQ.png)


### Basic VIews

-   **Report View** : This is the main view where the Dashboard is created

-   **Data View** : The data view gives a preview of the entire data.

![](https://cdn-images-1.medium.com/max/800/1*Oy9ySQTRw7325v05Iu6HvQ.png)

-   **Relationship View**: The relationship view displays the relationship between various objects.

![](https://cdn-images-1.medium.com/max/800/1*aKOGIbOkrTWRnmrX0K3A0A.png)

###  Connecting to a Data Source

Power BI can be connected to a number of data sources. the `Get Data` icon displays all the possible available options from where data can be imported into Power BI.

![](https://cdn-images-1.medium.com/max/800/1*-XzTx1lkwdqh9UwEzbjFJg.gif)

 Let’s look at a few of the most commonly used data sources:

-   **Excel data**

Let’s connect to an Excel data source. The workbooks consist of some fake financial data. Download the file from [here](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Power%20BI/Financial%20Sample.xlsx). Power BI Desktop  loads the workbook and reads its contents, and shows you the data in the file using the Navigator window.
![](https://cdn-images-1.medium.com/max/800/0*pCdHL-766l6dYsz4.png)

Once loaded, the data can be viewed in the **Fields** pane.

![](https://cdn-images-1.medium.com/max/800/0*MtIGb0UBc-XPMHxc.png)

-   **Web**

You can also simply use the data from the web. Here is a dataset which presents the best and the worst states for retirement in the U.S.

link: [_http://www.bankrate.com/finance/retirement/best-places-retire-how-state-ranks.aspx_](http://www.bankrate.com/finance/retirement/best-places-retire-how-state-ranks.aspx)

Simply select `Web` as an option in `Get Data` and enter the name of the url.

![](https://cdn-images-1.medium.com/max/800/1*8Qgwm-9BJmohX36KIlqTYA.png)

Try experimenting with other data sources too.

----------

## <a name = "transforming_data"></a> 5. Transforming Data

After the data has been loaded, it becomes  visible under the `Fields` Tab. From here, we can modify our datasets with the help of **Query Editor**. Query editor can be used for modifying datasets irrespective of their data source. We can do manipulations like renaming a dataset, removing a single or multiple columns etc in the query editor. The Query Editor can be accessed by clicking the `Edit Queries` button on the Home Ribbon.

### Creating a Custom Column

Using the same [Financial data](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Power%20BI/Financial%20Sample.xlsx), that we used above, let’s shape data to meet our needs. Let’s create a custom column called `New Manufacturing Price`, which is equal to:

    ([manufacturing Price])*3

![](https://cdn-images-1.medium.com/max/800/1*OPnVtNo5H5iIDZrPcd_4Ew.gif)

### Changing Column Data Types

The data types of the columns can also be changed easily. The `Units Sold` column has a floating point data type which can be changed to a whole number.

![](https://cdn-images-1.medium.com/max/800/1*bKNOebMFGn6tmRnJolwb5A.gif)

### Removing Columns

Removing columns is also easy. Simply select the column to be selected and choose the `Remove Columns` option, as shown in the following figure. Let’s get rid of the `Discount` column as it is adding no value to our dataset.

![](https://cdn-images-1.medium.com/max/800/1*5y8cAwK_bVVwSMEfkZUWXw.png)

Similarly, there are other multitudes of functions that can be carried out  like removing and adding rows, transpose, pivot and split which can be easily achieved through the query editor. Note that all the steps that you undertake to transform your data also appears in the `Query Settings` panel.

![](https://cdn-images-1.medium.com/max/800/1*-FKh_xAQ2Zu2GxoQxn6Thg.png)

----------

## <a name = "reports"></a> 6. Reports

Reports are a collection of visualisations that can be created on one or more pages. These visualisations are usually related to one another. 

![](https://cdn-images-1.medium.com/max/800/1*VzL1fKbFFsL8_NAJ5jRNYw.png)

----------

## <a name = "dashboard"></a>7. Dashboard

A dashboard is a collection of several views, enabling one to compare a variety of data simultaneously. Whereas the report can encompass various pages, a Dashboard is a single page interface.

### Creating a Dashboard

Once we have the dataset ready with all the manipulations done, we can proceed for **the Dashboard** creation process. A Power BI dashboard, also known as canvas, consists of many visualisations on a single page which helps to tell a story. These visualisations called **tiles** are pinned to the dashboard from the reports.

Let’s now try to understand what insights we can get using superstore data set:-

-   **Sales by Country**

![](https://cdn-images-1.medium.com/max/800/1*Scx2P5OqhhMjwip1R4eC3w.gif)

-   **Sales and Profit by Segment**

![](https://cdn-images-1.medium.com/max/800/1*jMkOIlsKFrkqDh9g9sBw8A.gif)

-   **Sales & Profit by Month**

![](https://cdn-images-1.medium.com/max/800/1*G_47evCEtV1C8Tw7OaRQxg.gif)

-   **Sales by Product**

![](https://cdn-images-1.medium.com/max/800/1*HQLNRH37AG8sso8ULFMxBg.gif)

-   **Profit by Discount Band**

![](https://cdn-images-1.medium.com/max/800/1*dLGe5YP-3prFe5GnZTwlmw.gif)

The Dashboard created is interactive which means a change in one tile affects the other.

![](https://cdn-images-1.medium.com/max/800/1*NbiVk0mtt2_5aWXvZUnfYQ.gif)

----------

## <a name = "r_and_python"></a>8. Power BI’s integration with R & Python

Apart from the various visualization advantages that Power BI offers, it also has an amazing out of the box connection capabilities. Power BI can easily integrate with languages like Python and R and also with DBMS like SQL. This offers increased advantages in terms of functionalities and comes in handy for Data Scientists who are used to working in Python or R. They can directly import the R and Python scripts in the workspace and take advantage of its visualisations which are far more superior than that of these languages.

In this section we shall learn how to work with Python and R scripts in R. For learning about **SQL’s integration with Power BI**, here is a detailed article on that:

-   [SQL with Power BI](https://www.datacamp.com/community/tutorials/sql-with-powerbi)

### Power BI & R

R is a popular statistical language used to perform sophisticated analysis and predictive analytics, such as linear and nonlinear modeling, statistical tests, time-series analysis, classification, clustering, etc. Using Power BI in conjunction with R  gives the users access to a rich, ever-expanding collection of statistical analysis and data mining libraries to help them gain deeper insights from their data.

#### Pre-requisites

Make sure you have the following installed and running on your local systems:

-   R
-  A separate R integrated development environment (IDE) like R Studio.

It is also important to note that:

-   Only data frames are imported
-   Any R script that runs for more than 30 min gets automatically timed out.

Verify that R and R studio are installed on your system. Launch the Power BI and go to `Options and Settings -> Options`

![](https://cdn-images-1.medium.com/max/800/0*4AIcsRgH4TrdNKxE.png)

Under `Options`, go to the `R Scripting` Tab and make sure you can see the correct R version.

![](https://cdn-images-1.medium.com/max/800/1*xvfLQZMf9IdVhh2qkB9ehQ.png)

#### Using R Scripts within Power BI

[Working with R Scripts in Power BI](https://www.red-gate.com/simple-talk/sql/bi/power-bi-introduction-working-with-r-scripts-in-power-bi-desktop-part-3/) is a very good resource on this topic. Below is an overview from the same source.

1.  **R scripts for Importing Data**

There may be times when you don’t want to import an entire dataset but a portion of it. You can write an R script to only select certain columns or rows from the entire dataset to be loaded into Power BI.

> For this demonstration, we will be working with the well known Iris dataset that is included with the CRAN distribution

![](https://cdn-images-1.medium.com/max/800/1*EFCmy418PKuuOLzvu_ay_A.gif)

Datasets can also be imported from files. Here is an example which shows how to **load a CSV file** into the workspace with the following script. Download the file from [here.](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Power%20BI/Iris.csv)

    iris_csv <- read.csv(file="C:/Users/Parul/Desktop/Iris", header=TRUE, sep=",")

![](https://cdn-images-1.medium.com/max/800/1*l9qWxeRivDmyrsJIk_pJfQ.gif)

Merely importing data with an R script doesn’t serve much of a purpose. The actual use is when we can manipulate data while importing. The following script uses the **summarize** and **group_by** functions available in the **dplyr** R package to group and aggregate the data before importing it:

Launch R Studio and install the following packages:

    install.packages("dplyr")  
    install.packages("data.table")  
    install.packages("ggplot2")

Now, use the following R script to import the Iris data. We will get a new dataset called iris_mean which contains the mean for each of the four measures, grouped according to the values in the _Species_ column.

    library(dplyr)
    
    iris_mean <- summarize(group_by(iris, Species),  
    slength = mean(Sepal.Length), swidth = mean(Sepal.Width),  
    plength = mean(Petal.Length), pwidth = mean(Petal.Width))

![](https://cdn-images-1.medium.com/max/800/1*fUSI2aKossJiQm5e5aU9XA.gif)

**2. R scripts for Transforming Data**

R scripts come in handy when we want to manipulate data that is already imported into the workspace. Let’s say we want to apply the `summarize` and `groupby` functions after the entire data has been imported. This can be achieved by running R Script in the Query Editor as follows:

![](https://cdn-images-1.medium.com/max/800/1*Q4uZg6drV4RPgbkQ_u7w0g.gif)

**3. R scripts for Creating Visualisations**

With the help of R scripts, you can create visualisations in Power BI. Simply type in the script and load in the necessary libraries and you get visualisations similar to the ones in any R IDE. Let’s go through the steps:

-   Import the Iris dataset into the workspace.
-   Click on the ‘`R script Visual`’ in the visualisation Tab and a placeholder R visual image appears on the canvas and a script editor at the bottom.
-   Select the fields that you want to include in the script. Let’s select `PetalLengthCm ,PetalWidthCm` and `Species`. The selected fields appear under the `Values` Tab and pre-populated R script appear in the R editor.
-   The script creates a dataframe named `dataset` with the selected columns. You can now write your script here or make changes in the existing one. Let’s paste the following code which imports **ggplot** library and creates a scatter plot.

```
      library(ggplot2)  
      ggplot(data=dataset, aes(x=PetalWidthCm, y=PetalLengthCm)) +  
        geom_point(aes(color=Species), size=2) +  
        ggtitle("Petal Widths and Lengths") +  
        labs(x="Petal Width", y="Petal Length") +  
        theme_bw() +  
        theme(title=element_text(size=15, color="blue3"))
```
  
![](https://cdn-images-1.medium.com/max/800/1*w-uiGNNOgfJpH_KqXiLCTA.gif)



### PowerBI & Python

Python is a widely used general-purpose programming language, and a large number of Python libraries are available to perform statistical analysis, predictive modeling using machine learning algorithms.

Microsoft recently made it possible to integrate Python scripts within PowerBI which enables running Python scripts and obtaining Python visuals within Power BI. Let’s look at the steps needed to do the same. But before that there are few pre-requisites :

-   Make sure that Python is up and running on your local systems.
-   All required packages and libraries should also be loaded such as pandas, matplotlib etc.
-   Currently, only pandas dataframe are supported.
-   Any Python script that runs for more than 30 min gets automatically timed out.
-   Python needs to be enabled before we can use it. Launch the Power BI and go to `Options and Settings -> Options`

![](https://cdn-images-1.medium.com/max/800/0*4AIcsRgH4TrdNKxE.png)

Under `Options`, go to the `Preview Features` Tab and enable ‘Python Support’.

![](https://cdn-images-1.medium.com/max/800/0*cvouQbY2CwXPP7Ts.png)

Restart Power BI and you get the Python icon both in visualisation as well as in the `Transform` tab.

![](https://cdn-images-1.medium.com/max/400/0*2-EIn5l2gUirvUaq.png)

![](https://cdn-images-1.medium.com/max/800/1*Ah6pI70DtlpzmtAJbGdFww.png)

There are multiple ways of running Python Scripts in Power BI

1.  **Running Python scripts exclusively**

Steps:

-   To run your Python Script, select `Get Data > More>Other > Python script` as shown below.

![](https://cdn-images-1.medium.com/max/800/0*qR1OympDDUw9EUGh.png)

Now, simply paste your Python script here in the window that opens. Select `OK` to run the script which and then imports the resulting datasets into the Power BI Desktop workspace.

![](https://cdn-images-1.medium.com/max/800/1*LiltJl-Ki-QmSV-KhobDNg.png)

**2. Creating Visualisations using Python**

-   Import the dataset into the workspace. Going with the same [Financial dataset](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Power%20BI/Financial%20Sample.xlsx), which  pertains to Financials of a hypothetical company.
-   Click on the ‘`Python Visuals`’ in the visualisation Tab and a placeholder Python visual image appears on the canvas and a Python script editor at the bottom.
-   Select the fields that you want to include in the script. Let’s select `Sales` and `Profit`. The selected fields appear under the `Values` Tab and the scripts also appear in the Python script editor.
-   The script creates a pandas dataframe named `dataset` with the selected columns. You can now write your script here or make changes in the existing one. Let’s paste the following code which imports matplotlib and creates a plot.
```
    import matplotlib.pyplot as plt  
    dataset.plot()  
    plt.title("Sales Vs Profit")  
    plt.show()
```
-   Run the script and the visualisation appears on the canvas. The visualisation appears as it would in any Python IDLE.

![](https://cdn-images-1.medium.com/max/800/1*7q0CusYGb-IK3c0uezOjGA.gif)

-   Next, let’s create a correlation plot. Select `Discounts, gross Sales,` and `Units sold` in addition to the previous fields and replace the script with this new script:
```
    import matplotlib.pyplot as plt  
    plt.matshow(dataset.corr('pearson'))  
    plt.show()
```

![](https://cdn-images-1.medium.com/max/800/1*N0PFYSXq3eIzAL3Cr9fH4w.gif)

-   We can also import other libraries. Let’s import Seaborn library but make sure it is installed on your system. The dataset is called the ‘Tips’ dataset which usually comes pre-loaded with seaborn. Download the dataset from [here](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Power%20BI/tips.csv) and load it into the workspace. Then paste the following code into the script editor and you will get the seaborn plots.
```
    import matplotlib.pyplot as plt  
    import seaborn as sns  
    sns.set(style="darkgrid")
    
    sns.relplot(x="total_bill", y="tip", data=dataset)  
    sns.relplot(x="total_bill", y="tip", hue="smoker", data=dataset);  
    sns.relplot(x="total_bill", y="tip", hue="smoker",col="time", data=dataset);
    
    plt.show()
```

![](https://cdn-images-1.medium.com/max/800/1*qi9rZFAKGsw3ZZANzzWDlQ.gif)

The Dashboard with all the Python visualisations will finally appear like this.

![](https://cdn-images-1.medium.com/max/800/1*ueQfl1qsBJRBXgnqlKK-Jg.png)

Python Dashboard

----------

##  <a name = "saving"></a>9. Saving and Publishing

### Saving and Exporting Files

You can  save your files as Power BI templates. The visualisations can also be exported as PDF files.

### Publishing

Data is only useful when it can be shared among people or organisation. The generated Dashboard or reports can also be shared by publishing it to the Power BI Service. We can then use the Power BI Apps to view or interact with the Dashboards/Reports.

![](https://cdn-images-1.medium.com/max/800/1*VySwsMlEjueEPXXHV_0fqw.png)

----------

##  <a name = "conclusion"></a>10. Conclusion

That’s all we need to know create a good visualization in PowerBI although, one might find doing a lot more revising in each stage than we did here. So with experimentation and practise, Power BI becomes a lot more familiar and will unleash amazing features to help us analyze and present data.

---
**References:**
* [https://docs.microsoft.com/en-us/power-bi/desktop-what-is-desktop](https://docs.microsoft.com/en-us/power-bi/desktop-what-is-desktop)


