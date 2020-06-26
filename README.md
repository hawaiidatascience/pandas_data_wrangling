
![alt text](https://github.com/hawaiidatascience/pandas_data_wrangling/raw/master/images/hidsi-header.png "Hawaii Data Science Institute")
# Introduction to the Pandas Python Package For Data Wrangling


## Pre-requisites

* The creation of a Data Camp account and signup for the Data Wrangling with Python track from HI-DSI

This course builds on the introductions to Python from <https://www.datacamp.com/tracks/custom-data-science-institute-intro-courses-dr-stokes> so if you find yourself struggling to understand some concepts it might be helpful to review the "Introduction to Python" course and "Introduction to Data Science in Python: Getting started in Python" chapter.

## Module introduction.

Data Wrangling is the process of transforming your data from one form into another, usually with the intent of making it more suitable for analysis.  This is a vital part in the Extract, Transform and Load (ETL) workflow and is encompassed in the data transformation portion of that workflow.

Data transformation is the process of changing the format of data so that it can be used by different applications. This may mean a change from the format the data is stored in into the format needed by the application that will use the data.

### WHY SHOULD I CARE OR WANT DO THIS

If you have ever worked with a set of data in an Excel spreadsheet, Google sheet or CSV file you have probably has to modify that data in some manner to use it.  You probably have needed to add or remove columns and rows or do some summations or different arithmetic functions to the data.  Excel and G-sheets work just fine for simple data.  But what do you do when you have thousands and millions of rows of data?  Or what if you have a bunch of the same type of dataset and your want to apply the same steps to each dataset or repeat this in the future?  Manually doing this work doesn't scale nor is what you did reproducible or easily shareable with others.

So you using some of the tools presented here you will be able to scale, automate, document and reproduce your process of modifying your data as you move through from initial data to an analysis product.

Here you will learn the basics of using Python and the Pandas library for loading data into a “DataFrame” that can then be leveraged to perform transformations on the initial raw dataset to produce a data product that has been cleaned and formatted so that it may be used in further analysis and workflows.

## Module learning outcomes

<details><summary>More</summary>
<p>

4.0.  Understand what python libraries and modules are and how to load and use them, particularly the “pandas” library

4.1  Describe the “pandas” Series and DataFrame objects and perform loading plain text file data, handle missing data and writing data output to a file.

4.2  Describe pandas DataFrame attributes and methods and perform data subsetting and vectorized arithmetic operations on pandas DataFrames.

4.3  Perform data subsetting using boolean methods for pandas DataFrames, sorting of data by index or values and plot data as basic charts using the pyplot library.

4.4  Perform dataType inspection and modification on a pandas DataFrame, utilize string methods to manipulate text values, reindex a DataFrame and identify, filter and fill missing data.

4.5  Describe Global and Specific data processing and perform data splitting, grouping. aggregation,filtering and transformations.

4.6  Describe merging  DataFrames and Series using inner and outer-join functions and perform DataFrame concatenations and merges.

</p>
</details>

## Module Competencies

<details><summary>More</summary>
<p>

4.0  Use python the pandas python libraries and alias.

4.1  Read a text file using pandas and output a new file.

4.2  Subset data and execute vectorized arithmetic operations using pandas.

4.3  Subset and sort data by index or values and plot data with the pyplot library.

4.4  Manipulate string data values and identify, filter and fill missing data using pandas

4.5  Split, group, aggregate, filter and transform data using pandas.

4.6  Merge and concatenate data using pandas.

</p>
</details>

## Getting Started

To get started we will be using learning materials in two formats:

#### 1.) Jupyter Notebooks with sample datasets. (it is assumed you are familiar with Jupyter)


The Juptyer Notebooks contain self contained "chapter" explanations of the concepts and along with executable code examples that you can run and modify to explore how Python and pandas work. In addition to the "chapters" there are notebooks that have Exercise solutions from each "chapter" as well as Practicals for each "chapter" to bring all the concepts together.  In order to access the Jupyter notebook materials you can either use this URL <https://mybinder.org/v2/gh/hawaiidatascience/pandas_data_wrangling/master>  that links to a cloud hosted Jupyterhub workspace. NOTE that this is only a temporary workspace and will disappear once you disconnect from it.

OR

you can use Anaconda on your own computer and download the materials from this link  <https://github.com/hawaiidatascience/pandas_data_wrangling/archive/master.zip> - this avenue allows you to keep the changes you make to any of the notebooks as you work through the course at your own pace.

Do Note that when running code cells within the training materials you will need to run the cells in order starting at the top of a notebook since the operations can rely on the execution of previous cells as you get further down the notebook.  (so if you run into an error be sure you have run all the code cells that came before – especially the loading of pandas).



#### 2.) Data Camp courses.

<details><summary>More</summary>

The Data Camp track that compliments the Jupyter Notebook materials is "Data Wrangling in Python" (<https://www.datacamp.com/tracks/custom-data-wrangling-in-python>).  This track has four course that cover the same materials as the Jupyter Notebooks with short videos, slides and small Exercises.

The Data Camp materials may be more remedial than the Jupyter Notebooks so try them both to see what works best for you.

</details>

# Lets begin

### Introduction
  
Lets begin with the Jupyter Notebook 0_Introdcutions.ipynb to introduce the basic concepts of Data Wrangling and pandas.  

NOTE - if you downloaded the materials and are using Anaconda on your own machine you will need to install pandas as the materials instruct - if you are using the cloud hosted materials pandas is already installed.

---

### Pandas Data Structures
<details><summary>More</summary>
<p>
  
Open 1_pandas_Data_structures.ipynb.
This chapter introduces the Python pandas modules and its primary data structures the “Series” and “DataFrame” and how to manipulate these data structures.  These concepts and skills are necessary to working with and analyzing tabular data and provide the foundation for everything else in this module.

#### Outcomes:
* Learn about the pandas Series and DataFrames concepts
* Understand the difference between pandas Series and DataFrames
* Learner will be able to: Create Series and DataFrames, Index Series and DataFrames, Access data within Series and DataFrames, Modify data within Series and DataFrames, Add and Modify columns and rows in Series and DataFrames

</p>
</details>

---

### Data Loading and Storage
<details><summary>More</summary>
<p> 
  
Open 2_Data_Loading_and_Storage.ipynb
This chapter introduces how to load plain text data files into pandas DataFrames and how to handle common data integrity issues such as missing values or ignore rows or columns with irrelevant information.  These skills are important as the first step in any data workflow is to
load the information in order to analyze or manipulate it later.

#### Outcomes:

* Learn how to transfer data from plain text files (.csv) to pandas DataFrames
* Understand what a plain text file is.
* Handle missing data in a DataFrame
* Skip loading undesired data from a file into a DataFrame
* Writing DataFrames to a text file

</p>
</details>

---

### DataFrame Attributes and Arithmetic

<details><summary>More</summary>
<p>
 
Open 3_DataFrame_Attributes_andArithmetic.ipynb.
It is crucial to have a deep understanding of your data in order to draw meaningful insights from it. In this chapter we will see how to use the built in functionalities of pandas to begin exploring and transforming data. This will help identify patterns or potential flaws in the dataset and hopefully inspire or even answer some interesting questions.

#### Outcomes:

* Learn how to use a pandas DataFrame attributes in order to understand more about a dataset
* Learn common pandas DataFrame methods to inspect the dataset to understand some basic properties such as (min,max,mean,sum..)
* Learn how to view subsets of a pandas DataFrames
* Learn how to perform vectorized arthimetic operations on pandas DataFrames

</p>
</details>

---

### Jump to Data Camp  - Streamlined Data Ingestion With Pandas

To reinforce and augment the Jupyter Notebook materials or perhaps instead of them it is recommend that your complete the Streamlined Data Ingestion With Pandas - Importing Data From Flat Files section. https://www.datacamp.com/courses/streamlined-data-ingestion-with-pandas

---

### Subsetting and Sorting

<details><summary>More</summary>
<p>
 
Open 4_Subsetting_and_Sorting.ipynb
This chapter covers the basics of subsetting data within a DataFrame and basic sorting.

#### Outcomes:
* Learn to subset data using comparison and boolean methods for a pandas DataFrame
* Learn how to sort data by index or value within a pandas DataFrame
* Learn how to plot data using pyplot for basic charting using data within a pandas DataFrame

</p>
</details>

---

### Data Preperation and Cleaning

<details><summary>More</summary>
<p>
 
Open 5_Data_Preparation_and_Cleaning.ipynb
This chapter covers the basic use case of needing to prepare or clean a set of data for further analysis using pandas.

#### Outcomes:
* Learn to inspect and modify dataTypes in a pandas DataFrame
* Learn how to utilize the pandas Series ‘string’ methods to manipulate string data
* Learn how to reindex a pandas DataFrame
* Learn how to handle missing data (identifying, filtering and filling)

</p>
</details>

---

### Function Application and Mapping

<details><summary>More</summary>
<p>
 
Open 6_Function_Application_and_Mapping.ipynb
What we will learn in this chapter might be some of the most important concepts and skills that we will cover in this entire course. We will be tying much of what we have learned in previous chapters together, and the practicality will become clear as you read and work through the exercises.
Function application and mapping simply refers to processing the entries of a DataFrame to better suite your needs.

#### Outcomes:
* Learn Global and Specific processing
* Learn to split and group data
* Learn to aggregate, filter and transform data

</p>
</details>

---

### Combine DataFrames

<details><summary>More</summary>
<p>

Open 7_Combining_DataFramews.ipynb
In this chapter we will learn about four different strategies for combining data sets and the methods `pandas` has implemented to support them. The strategies we will cover will be powerful enough to handle almost all of the types of combining you will need to do in practice.

#### Outcomes:
* Learn how to merge DataFrames and Series
* Understand how to use inner and outer join functions
* Learn how to concatenate DataFrames and understand the difference to merge.

</p>
</details>

---

### Jump to Data Camp - pandas Foundations

It is recommended that your augment learning with the Data Camp "pandas Foundations- Data Ingestion and Inspection"  <https://www.datacamp.com/courses/pandas-foundations>

