# Amazon_Vine_Analysis
---
### Overview

The purpose of this analysis is to use PySpark to perform the ETL process to extract one of the datasets from Amazon reviews written by members of the paid Amazon Vine program. To accomplish this I transformed the data, connected to an AWS RDS instance, loaded the transformed data into pgAdmin, and then used PySpark to determine if there was any bias towards favorable reviews from Vine members in the dataset.

---

#### Deliverable 1: Perform ETL on Amazon Product Reviews
 
<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/1.png"  width="70%" height="70%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/2.png"  width="60%" height="60%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/3.png"  width="80%" height="80%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/4.png"  width="80%" height="80%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/5.png"  width="80%" height="80%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/6.png"  width="80%" height="80%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/7.png"  width="80%" height="80%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/8.png"  width="80%" height="80%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/9.png"  width="60%" height="60%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/10.png"  width="60%" height="60%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/11.png"  width="60%" height="60%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/12.png"  width="60%" height="60%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/13.png"  width="60%" height="60%">

<img src="https://github.com/Tifarahani/Amazon_Vine_Analysis/blob/main/Resources/Img/14.png"  width="60%" height="60%">



#### Conclusion:
36% of records that were part of the Vine program(paid) gave a 5-star rating.
47% of records that were not part of the Non Vine program(unpaid) also gave a 5-star rating.
There were significantly less records that had Vine than those records that did not had Vine,
so there is less possibility of bias in the Vine/Star-Rating reviews.
After reviewing the results comparing the Vine vs. Non-Vine reviews, there is not a bias for reviews in the Vine program. As seen in the images above, 42% of Vine members reviews were 5-star and 47% of Non-Vine reviews were 5-star. The number of Vine reviews total in comparison to Non-Vine reviews is significantly less though.

In order to confirm the Non-Vine customers actually purchased the item from Amazon or that it wasn't gifted, we can also filter based on the verified_purchase column. After rerunning the calculations on this new dataframe, 48% of Non-Vine members reviews were 5-star and verified that they purchased the item.
 
---
#### Resources:
- Google Colab (to run PySpark)
- Jupyter Notebook
- AWS S3 and RDS
- PostgreSQL
