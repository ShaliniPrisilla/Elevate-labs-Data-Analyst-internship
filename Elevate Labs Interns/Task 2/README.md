# Task 4 : Data Visualization and Storytelling

![data_story3_sq-1](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/c44e7c77-6134-432c-add6-1bf5a4ca17e7)

This repository is dedicated to the art of data visualization and data storytelling. In today's data-driven world, effectively conveying information through compelling visualizations and narratives is essential. Whether you are a data scientist, analyst, or anyone interested in making data more accessible and insightful, this repository provides resources and examples to help you master the craft of data storytelling.

## Introduction

Data storytelling is creating a narrative that explains the insights derived from data. It involves selecting and presenting data through visualizations, combining them into a coherent narrative, and effectively communicating your findings to your audience. This repository serves as a guide to help you create engaging and informative data stories.

## Why Data Visualization Matters

Data visualization is the cornerstone of effective data storytelling. It helps in:

- **Understanding Data**: Visualizations provide an intuitive way to grasp complex data.

- **Spotting Trends**: Patterns and trends become evident when data is presented visually.

- **Engaging Audiences**: Visual elements captivate the audience and make data more accessible.

- **Informing Decision-Making**: Data-driven decisions are more informed and effective.

## Tools and Libraries
These are the tools and libraries that we are going to use today.

- [Jupyter Notebook](https://jupyter.org)
- [Pandas](https://pandas.pydata.org)
- [Numpy](https://numpy.org)
- [Matplotlib](https://matplotlib.org)
- [Seaborn](https://seaborn.pydata.org)

## Data Understanding
### Source Data
![Amazon_Books_logo svg](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/688f3d54-a0fc-48a7-bb68-f1bc51b04828)

- [Amazon Top 50 Bestselling Books 2009 - 2019](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019/data)
- 7 Column
- 550 Rows
  
### Data Dictionary
Dataset on Amazon's Top 50 bestselling books from 2009 to 2019. Contains 550 books, and data has been categorized into fiction and non-fiction using Goodreads

- Name: Name of the Book
- Author: The author of the Book
- User Ring: Amazon User Rating
- Reviews: Number of written reviews on Amazon
- Price: The price of the book
- Year: The Year(s) it ranked on the bestseller
- Genre: Whether fiction or non-fiction

## Data Preparation 
The first step is to import the necessary library and load the dataset.

![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/24b6fe48-bf9d-4c2b-a0e4-9277b4b56f51)

## Data Cleansing
![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/68297357-d28b-4783-aefa-16035ddc9c9c)

The data is clean, with correct data types, and free from missing values and duplicates.

## Exploratory Data Analysis & Data Visualization
### Genre of the bestseller books

![image](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/f5eb5338-6598-47c0-9d40-f3691555d69d)

![image](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/34df8bc5-54c1-48a2-9ea9-f9f66cc973fe)

Based on the data, Non-fiction books dominate the reviewed book category, representing a substantial 56% share, while fiction books make up the remaining 44% of the reviewed books. This suggests that non-fiction literature tends to generate more reader engagement and feedback compared to their fictional counterparts.

### Distribution Of User Rating For Books

![image](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/c84ddcf4-95a4-4f7a-b97f-3e8d25f602d0)

![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/d9f4928c-d48f-448e-a786-ce492b0773f3)

In this dataset of 550 book user ratings, we can observe rating distribution on a scale from 0 to 5. The most common rating is 4.8, which accounts for approximately 23% of all ratings. Following closely, ratings of 4.7 and 4.6 are also quite popular, making up about 19.6% and 19.1% of all ratings, respectively. This insight provides a clear picture of the distribution of user ratings in the dataset over 81.7% of ratings are 4.5 or higher, indicating that users have positively rated majority of books in the dataset.

### Top 5 Author Who Wrote Most Of Bestseller Books

![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/2ab0e4e6-3f57-42a4-b39a-7b035347ca1b)

![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/696209ea-ea04-43dc-9e38-5549f6711e1e)

Based on the data for the top 10 authors with multiple book publications, we find that Jeff Kinney leads the list with 2.2%. Gary Chapman, Suzanne Collins, and Rick Riordan are in the same tier, each with 2% of the total books published. This suggests that Jeff Kinney may be a favorite among readers.

### Distribution Of Reviews Over The Years

![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/c03ce7a7-fab7-4c79-a855-4a775af6a319)

![image](https://github.com/Art1star/Data_Visualization_Storytelling/assets/70962598/1018c638-7167-46b7-956b-a1836650f63b)

Looking at the distribution data above, we observe that in 2015, the fiction genre accounted for the highest percentage of book reviews at 8.6%. Interestingly, this genre experienced only a slight decline to 4.6% in 2018. However, by the end 2019, it rebounded, representing 6.7% of the total reviews.

In contrast, the non-fiction genre peaked in 2018 with 5.4% of total reviews and remained steady at 5.1% in 2019. Nevertheless, it still lags behind the fiction genre regarding the total reviews.

### Total Profit by Genre Over the Years

![image](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/234ba437-1957-4a2c-a2a0-d7a449d80bbb)

![image](https://github.com/Art1star/Data_Visualization_Story_Telling/assets/70962598/e11781c9-2890-4879-8692-5794ae29301d)

In this dataset of book sale profits by year, we observe that fiction books consistently comprised a lower percentage of profits compared to non-fiction. In 2010, non-fiction books accounted for approximately 71% of total profits, whereas fiction books comprised about 29%. This trend continued in subsequent years. It is notable that while both fiction and non-fiction profits fluctuated annually, the dominance of non-fiction remained evident throughout the years, with a substantial 64.6% of total profits in 2019.

## Conclusion

Thank you for exploring this Data Visualization and Storytelling repository. We hope the resources, tools, and examples provided here will help you become a more effective data storyteller. By mastering the art of data visualization and storytelling, you can unlock the power of data to inform, persuade, and inspire.

If you have any questions or feedback or would like to contribute to this project, please don't hesitate to reach out. We value your input and look forward to building a vibrant data storytelling community.

Happy data storytelling! 📊📚📈





