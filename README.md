# Amazon_Vine_Analysis
## Analysis Overview
This module was us to analyze Amazon Vine program and determines if there is a bias toward favorable reviews from Vine members.\
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics. The data set selected for teh review was that of Books. https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Books_v1_02.tsv.gz\

## Resources
- Data Source: [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Books_v1_02.tsv.gz), [Books Review dataset]
- Software: Google Colab Notebook, PostgreSQL 11.9, pgAdmin 4, AWS-RDS 

## Results

### How many Vine reviews and non-Vine reviews were there?
- Vine reviews
      <img width="306" alt="1" src="https://user-images.githubusercontent.com/76264061/115157549-8cf85680-a0a7-11eb-9eee-59b238f85b44.png">

- Non-Vine reviews 
    <img width="549" alt="2" src="https://user-images.githubusercontent.com/76264061/115157098-fb87e500-a0a4-11eb-9e61-df387f149d5f.png">

### How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
 - Vine reviews 
    <img width="518" alt="3" src="https://user-images.githubusercontent.com/76264061/115157163-5a4d5e80-a0a5-11eb-963a-7215ce24564a.png">

- Non-Vine reviews 
    <img width="553" alt="4" src="https://user-images.githubusercontent.com/76264061/115157179-69cca780-a0a5-11eb-813a-b9c8b25a3b39.png">

### What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- Vine reviews ( Since the paid reviews were 0, The same was not a divisible number)
      <img width="561" alt="5" src="https://user-images.githubusercontent.com/76264061/115157205-9a144600-a0a5-11eb-9e82-062fe4bd26b3.png">

- Non-Vine reviews 
      <img width="560" alt="6" src="https://user-images.githubusercontent.com/76264061/115157214-a39dae00-a0a5-11eb-8ac6-911cabaffeec.png">

## Summary
Clearly there were no paid reviews in the Vine program and all 5 stars reviews were non biased reviews. There was 60% of unpaid 5 star reviews, so we can know and can trust that the reviews were not biased in anyway. This describes a positivity bias for reviews in the Vine program.

### Side Note for the grader
This challeneg was rather interesting and not at all complicated. But what took me over 7 hours is loading to datasets to RDS. It took me forever to load the datasets. I had to switch between 3 datasets to complete the deliverables on time. Requesting you to accept my assignment.  
