# SQL with Tableau
### In this tutorial, you will learn how to how to connect Tableau to a Microsoft SQL Server database and then analyse the data to get insights.


Data is an important part of the lives of Data Scientists. Right from the sales and Profit of a company, to passengers in an airport, everything constitutes data. Now, all this data is recorded and most of the times stored in files called databases and an important task of a Data Scientist is to be able to access data from databases and then analyse them. Most of the ETL tools that tend to help in the cleaning part are actually running SQL commands under the hood. SO having some knowledge of SQL can be quite a valuable resource for a Tableau user.


## Objective

Apart from the various visualization advantages that Tableau offers, it also has an amazing out of the box connection capabilities. Tableau can easily integrate with DBMS like SQL. This offers increased advantages regarding functionalities and comes in handy for Data Scientists who are used to working in SQL_._ Tableau provides an optimized, live connector to SQL Server so that we can create charts, reports, and dashboards while working directly with our data.

## Pre-requisites

This article assumes some familiarity with Tableau, its properties and how it is used to do the analysis. Since this article will be focused only on SQL with Tableau, it is suggested to go through the following existing tutorials which serve as an excellent primer to both Tableau and SQL:

[**Data Visualisation with Tableau**](https://www.datacamp.com/community/tutorials/data-visualisation-tableau)

[**SQL Tutorial: How To Write Better Queries**](https://www.datacamp.com/community/tutorials/sql-tutorial-query)


##  Table of Contents
-   #### [1. Tableau](#tableau)
-   #### [2. Relational Databases: A Quick Overview](#relational-database)
-   #### [3. Connecting to SQL Serve](#sql-server)
-   #### [4. Importing SQL data into Tableau](#importing)
-   #### [5. Custom SQL](#custom-sql)
-   #### [6. Data Source Filters](#data-source-filters)
-   #### [7. Analysis in Tableau](#analysis)
-   #### [8. Conclusion](#conclusion)


# <a name="tableau"></a>1. Tableau

[Tableau Software](https://www.tableau.com/) is an American computer software company headquartered in Seattle which generates interactive data visualization products focused on BI. The main products offered by tableau are Tableau Desktop, Tableau Public and Tableau Online. You can read more about them [here](https://www.datacamp.com/community/tutorials/data-visualisation-tableau). For the purpose of this tutorial, we will be working with the **Tableau Desktop**(14 days trial available), since the free Tableau Public version doesn’t provide the SQL connectivity.

## Installation

Download the Tableau Desktop edition from the [official website](https://www.tableau.com/products/desktop). Follow the installation instructions and if the following screen appears on clicking the Tableau Icon, you are good to go.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/1.installation.png)


# <a name="relational-database"></a> 2. Relational Databases: A Quick Overview

The [Database management system](https://medium.com/analytics-vidhya/programming-with-databases-in-python-using-sqlite-4cecbef51ab9) (DBMS) is the software that interacts with end users, applications, and the database itself to capture and analyze data. The DBMS used for Relational databases is called **Relational Database Management Systems(RDBMS).**

A Relational database consists of one or more **tables** of information. The **rows in** the table are called **records** and the **columns** in the table are called **fields or** **attributes**. A database that contains two or more related tables is called a **relational** database i.e interrelated data. The major RDBMS are Oracle, MySQL, Microsoft SQL Server, PostgreSQL, Microsoft Access, and SQLite.

**_The main idea behind a relational database is that your data gets broken down into common themes, with one table dedicated to describing the records of each theme._**

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/2.relaitonal%20Database.png)

[Source](https://www.guru99.com/relational-data-model-dbms.html)

## SQL

SQL or the structured query language is a language that has been designed for the purpose of RDBMS. It is a declarative language for manipulating data, to access the database. SQL is used for insert, modify, update and query data in the databases. SQL can be regarded as a **language for database**s.


# <a name="sql-server"></a> 3. Connecting to SQL Server

There is a hidden value in our Microsoft SQL Server data which lies buried under the standard reports and complex BI tools. **Tableau delivers insight everywhere by equipping anyone to do a sophisticated visual analysis of SQL Server data.** We can connect Tableau to SQL Server live for tuned, platform-specific queries, or directly bring data into Tableau’s analytical engine to take the burden off the database.

Let us walk through an example depicting how to connect SQL server database to Tableau Desktop and then use it to create visualizations.

## Sample Database

For the demonstration purpose, we will be using a publicly accessible SQL Server instance on AWS and a database which has been created based on the Tableau’s built-in **Superstore** dataset. It contains information about products, sales, profits, etc. Our aim as Data Analysts is to analyze the data and find critical areas of improvement within this fictitious company. This SQL server instance has been hosted by [Ken Flerlage](https://www.blogger.com/profile/03698843288892226027), who regularly writes blogs for Tableau users.

## Accessing the sample database

-   Install the [SQL Server Management Studio](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-2017)(SSMS). SSMS is a free and integrated environment for managing any SQL infrastructure. With SSMS one can deploy, monitor, and upgrade the data-tier components used by your applications, as well as build queries and scripts.
-   Once downloaded and installed on to your system, you will see the following screen asking for certain credentials.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/3.MSSQL%20main%20screen.png)

Enter the following credentials:

    Server Name: ec2-52-14-205-70.us-east-2.compute.amazonaws.com
    
    Authentication: SQL Server Authentication
    
    Login: SQL
    
    Password: SQL

You will now be granted a ‘Read Only’ access to the ‘**SuperStoreUS**’ database.

![Alt text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/4.MSSQL%20credentials.gif)

For our example, **ec2–52–14–205–70.us-east-2.compute.amazonaws.com** is the name of the instance, **SuperstoreUS** and **Test** are the databases, and **Orders**, **Customer**s etc are the tables within the **SuperstoreUS database**. Thus there can be multiple instances and each instance can further contain multiple databases which can further have multiple tables.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/5.%20MSSQL%20explore.gif)



# <a name="importing"></a>4.  Importing SQL data into Tableau

#### Setting up the connection

Open the Tableau Desktop and navigate to the start screen. Here the connect pane offers a lot of choices in terms of the data sources that can be connected to Tableau. We will connect to the [Microsoft SQL Server](https://en.wikipedia.org/wiki/Microsoft_SQL_Server).

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/6.%20Tableau%20SQL%20connection.png)

On Clicking the `Microsoft SQL Server` option, a new screen will open up which will ask for the Server to which we want Tableau to be connected to. Enter the details and a familiar looking Tableau workspace opens up.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/7.%20TAbleau%20SQL%20credentials.gif)

Now, We can select from the list of available databases. Here we will select the SuperStore US database.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/8.%20Tableau%20SQL%20accessing%20tables.gif)

You can now click and drag the desired table on to the view. Let’s drag in the `orders` table for further analysis. The preview pane gives us options of `Update Now`, which loads the preview manually, or `Automatically Update`.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/9.%20Orders.gif)


## Getting data from multiple Tables from the same database

It is also possible to get in data from more than one Table in Tableau, through **joins**. Joining is combining the tables which are related by some common fields. For instance, it is possible to join `Orders` and `Returns` table since they have a common column called `Order-ID` . Join simply creates a virtual table by adding columns from different tables side by side.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/10.%20join.png)

[Join](https://onlinehelp.tableau.com/current/pro/desktop/en-us/datasource_plan.htm)

![](https://cdn-images-1.medium.com/max/800/1*eknlrmoVT364J7sWPjOYvQ.png)

In case, the analysis requires working with data from multiple sources, it is called **Data Blending**. You can read more about blending [here](https://www.datacamp.com/community/tutorials/spreadsheets-tableau#data-blending).

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/11.%20blend.png)

[Blend](https://onlinehelp.tableau.com/current/pro/desktop/en-us/datasource_plan.htm)


# <a name="custom-sql"></a>5. Custom SQL

Custom SQL gives the users control over the data that they want to bring into Tableau. This feature is not particularly about writing SQL queries but mainly about defining the data set. The process of defining a new custom SQL is as follows:

-   Click on the custom SQL Tab on the left side of the screen, and a dialogue box opens up.
-   Write the custom query that you want to execute in the dialogue box
-   Update the results and what we get are only orders where quantities are greater than  4.
-   Now move over to your worksheet and start exploring with Tableau.

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/12.%20custom%20sql.gif)

This was a simple query since the data is limited. However, you can even execute complex queries too to specially choose the data that you want to analyse upon.


# <a name="data-source-filters"></a>6. Data Source Filters

Just like Custom SQL, it is also possible to get some specific data into Tableau with **Data Source filter**s. Let’s see how to work with these filters.

-   Drag the `Orders` tab on to the view. The orders table contains a field called `Region` signifying four regions in the U.S where the products are sold.
-   Let’s say we want the orders only pertaining to **West** and the **Central** Region. Go to filters in the upper right-hand corner and click `Add`, and `Add again`
-   A list of fields gets populated. Select the `Region` field or any field of your choice.
-   Now, what we see is a list of probable values for the field we selected. Select the desired ones and click OK.
-   This returns the filtered data from the connection level.

_Keep in mind that both_ **_custom SQL Query_** _and the_ **_Data Source Filter_** _methods should be used only for specific use cases. The best option would be to first connect the data to Tableau and then use the filters within Tableau._

![Alt Text](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/13.%20data%20source%20filters.gif)



# <a name="analysis"></a>7.  Analysis in Tableau

After getting the data from the SQL server into Tableau, it can be easily analysed in Tableau. Let’s analyse the data that we have in our worksheet in multiple ways:

-   We could analyse the State-wise sales

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/14.%20analysis%20in%20Tableau1.png)

-   Or we could find those States where Sales figures are more than 5000.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/15.analysis%20in%20Tableau2.png)

-   Another point of analysis could be Sales vs the Profit scenario.

![](https://github.com/parulnith/Data-Visualisation-libraries/blob/master/Data%20Visualisation%20with%20Tableau/SQL%20with%20Tableau/Images%20and%20gif/16.%20analysis%20in%20Tableau3.png)

Thus, the analysis in Tableau after getting the data from SQL Server is pretty straightforward just like any other normal analysis.


# <a name="conclusion"></a>8. Conclusion

Using SQL and Tableau together takes the data analysis to the next level. We can easily connect the SQL Server to Tableau and extract the data directly into it. Tableau enables the users to toggle connections with a click to apply in-memory queries to a larger dataset. SQL is a pretty useful tool and when leveraged with the expertise of Tableau can help to make the analysis more powerful and insightful.

----------

### References

-   [Microsoft SQL Server — Tableau](https://onlinehelp.tableau.com/current/pro/desktop/en-us/examples_sqlserver.htm "https://onlinehelp.tableau.com/current/pro/desktop/en-us/examples_sqlserver.htm")
-   [Programming with Databases in Python using SQLite](https://medium.com/analytics-vidhya/programming-with-databases-in-python-using-sqlite-4cecbef51ab9)



