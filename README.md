# AirBnB-Project
## Introduction
*(This analysis was a part of case study based project for a business intelligence course during my masters degree)*\
Airbnb Paris, a service-based company, relied on customer satisfaction to drive revenue. To enhance their service quality and attract new customers, they turned to sentiment analysis of online reviews. By analyzing customer feedback, we were able to identify areas where their service offerings and operational processes could be improved. This data-driven approach provided valuable insights to help Airbnb Paris optimize their services and ultimately boost customer satisfaction and revenue.
## Exploratory Data Analysis(EDA) 
Once we gathered the data, we delved into a thorough exploration. Power BI was our tool of choice for visualizing and understanding the underlying patterns within the dataset.
![image-1](https://github.com/user-attachments/assets/e2af860b-7de1-437a-8b4c-cc475d741cd8)
## Data Cleaning 
Data Cleaning is one of the most vital step in data analysis. In order to clean the reviews, I did following steps
* **Translation from French to English**
* **Conversion into Lowercase**
* **Splitting**
* **Stopwords Removal**
* **Punctuation Removal**
  
After cleaning and preprocessing the review text, we were ready to calculate sentiment scores. The VADER library was employed to assign sentiment scores to each review. To visualize the overall sentiment distribution, we plotted a histogram, allowing us to identify areas where sentiment was predominantly positive, negative, or neutral.
![image-2](https://github.com/user-attachments/assets/55d828a5-67eb-4297-b616-d3cdd6d504ec)
## Cluster Analysis
As we can see from the histogram, most of the reviews were highly positive & few had a sentiment score little behind. We divided those reviews into clusters based on their characteristics. For this purpose, we used Elbow plot & Silhouette method to determine the optimal number of clusters based on the data.

![image-3](https://github.com/user-attachments/assets/600f74f0-b639-46ba-acac-ae77bc432068)
![image-4](https://github.com/user-attachments/assets/f5361bf8-142b-47a3-8a0e-c30ede73ec2e)

From both methods, we were able to dtermine the optimal number of cluster(2)\
There was a significant difference in average sentiment score for each cluster as evident below 

![image-5](https://github.com/user-attachments/assets/23bfba9f-4e2e-40ad-851d-b1b7d3f399d4)

## Findings
For a better performing cluster in terms of sentiment score 
1. Average price was low
2. Average Security deposit was low
3. Average Cleaning fee was low
4. Average number of beds were greater
5. Average number of baths were greater

So, In order to improve sentiment score, properties from the low performing cluster need to focus more on the points given above. This will eventually improve the customer service/feedback & revenue for AirBnb Paris.








