# Amazon_Vine_Analysis

[Big_Data_Amazon_Vine_README.docx](https://github.com/mmh926/Amazon_Vine_Analysis/files/6627716/Big_Data_Amazon_Vine_README.docx)

# Big Data - Amazon Vine Analysis README
# By:  Monica Holmes
# June9, 2021


##The purpose of this analysis is to access a dataset and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. From there, I used PySpark, in Collab, to determine if there is any bias toward favorable reviews from Vine members in your dataset. Finally, I wrote a summary of the analysis for Jennifer to submit to the SellBy stakeholders. 

I utilized PGAdmin to create four Tables within the Challenge / Vine database:

![image](https://user-images.githubusercontent.com/78371845/123721528-8e3ac200-d854-11eb-832a-36dea742f376.png)


Review ID Table output:

![image](https://user-images.githubusercontent.com/78371845/123721577-a3afec00-d854-11eb-891d-6cbf4a3a5dac.png)


Products Table output:

![image](https://user-images.githubusercontent.com/78371845/123721661-c9d58c00-d854-11eb-98ef-e8b4a63d629f.png)


Customers Table output:

![image](https://user-images.githubusercontent.com/78371845/123721715-e7a2f100-d854-11eb-88da-baa7326f699b.png)


Vine Table output:

![image](https://user-images.githubusercontent.com/78371845/123721760-fab5c100-d854-11eb-8609-57d3e3debb59.png)


Analysis: I will answer the following questions:
1.	How many Vine reviews and non-Vine reviews were there?
2.	How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
3.	What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Results: Below are my answers to the above questions:
1. There was a total of 27,009 reviews in the Shoe Dataframe. Of that, 22 were Vine reviews and 26,987 were non-Vine reviews. 

![image](https://user-images.githubusercontent.com/78371845/123721806-11f4ae80-d855-11eb-8a07-1f9c4c56c21f.png)

![image](https://user-images.githubusercontent.com/78371845/123721821-191bbc80-d855-11eb-90aa-0862697e78f2.png)

![image](https://user-images.githubusercontent.com/78371845/123721832-1faa3400-d855-11eb-908e-d2843b0fc7fd.png)



2. There were a total of 14,488 5-star reviews.  Of that, 13 paid Vine reviews were 5 stars, while 14,475 non-paid Vine reviews were 5-star. 

![image](https://user-images.githubusercontent.com/78371845/123721857-2df85000-d855-11eb-8f92-fade7b3c7866.png)

![image](https://user-images.githubusercontent.com/78371845/123721871-33559a80-d855-11eb-96b4-caf4d534bd1f.png)

![image](https://user-images.githubusercontent.com/78371845/123721882-38b2e500-d855-11eb-9df0-640de2effa0c.png)


3a. 59.09% of paid Vine reviews were 5-stars

![image](https://user-images.githubusercontent.com/78371845/123721916-48322e00-d855-11eb-8245-849747c8c1ed.png)


3b. 53.64% of unpaid non-Vine reviews were 5 stars.

![image](https://user-images.githubusercontent.com/78371845/123721953-60a24880-d855-11eb-94a7-fa7f38cab91c.png)



###**Summary:**###
Analysis of the Shoe data output indicates there is no bias in the Vine dataframe as the majority of total 5 star reviews (14488)  were non-Vine (unpaid) reviews (14475), equating to about 99%.
An additional analysis comparing the count of all the star ratings to non-Vine (unpaid) reviews is consistent with the previous analysis. Also, this is applicable to every star rating category. 

![image](https://user-images.githubusercontent.com/78371845/123722021-80397100-d855-11eb-8b7d-6f3b755476a4.png)

![image](https://user-images.githubusercontent.com/78371845/123722038-8596bb80-d855-11eb-877a-693dde2c372d.png)







