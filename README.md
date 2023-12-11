# Customer_Segmentation
Customer Segmentation with K-Means Clustering

After looking through several datasets on Kaggle, I chose this one focusing on Customer Personality Analysis (link below). This dataset looked like one you may receieve from a company asking for your analysis with several features to play around with. Dimensionality reduction may need to applied to this dataset and clustering may be a good approach to segmenting the customers in the data.

Here is the description of the features from the Kaggle site:

### People

* ID: Customer's unique identifier
* Year_Birth: Customer's birth year
* Education: Customer's education level
* Marital_Status: Customer's marital status
* Income: Customer's yearly household income
* Kidhome: Number of children in customer's household
* Teenhome: Number of teenagers in customer's household
* Dt_Customer: Date of customer's enrollment with the company
* Recency: Number of days since customer's last purchase
* Complain: 1 if the customer complained in the last 2 years, 0 otherwise

### Products

* MntWines: Amount spent on wine in last 2 years
* MntFruits: Amount spent on fruits in last 2 years
* MntMeatProducts: Amount spent on meat in last 2 years
* MntFishProducts: Amount spent on fish in last 2 years
* MntSweetProducts: Amount spent on sweets in last 2 years
* MntGoldProds: Amount spent on gold in last 2 years

### Promotion

* NumDealsPurchases: Number of purchases made with a discount
* AcceptedCmp1: 1 if customer accepted the offer in the 1st campaign, 0 otherwise
* AcceptedCmp2: 1 if customer accepted the offer in the 2nd campaign, 0 otherwise
* AcceptedCmp3: 1 if customer accepted the offer in the 3rd campaign, 0 otherwise
* AcceptedCmp4: 1 if customer accepted the offer in the 4th campaign, 0 otherwise
* AcceptedCmp5: 1 if customer accepted the offer in the 5th campaign, 0 otherwise
* Response: 1 if customer accepted the offer in the last campaign, 0 otherwise

### Place

* NumWebPurchases: Number of purchases made through the company’s website
* NumCatalogPurchases: Number of purchases made using a catalogue
* NumStorePurchases: Number of purchases made directly in stores
* NumWebVisitsMonth: Number of visits to company’s website in the last month

Data retrieved from: https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis/data?select=marketing_campaign.csv

## Conclusion


After going through the Exploratory Data Analysis on the raw customer data from Kaggle, scaling the data, using PCA to reduce the dimensionality, and finally applying KMeans clustering and visualizing the results, we've gained a good amount of insight from the data. With k set to 3, the clusters were not evenly distributed. Cluster 0 made up nearly 50% of the data, while cluster 1 and 2 were only about 28% and 25% respectively. 

### Cluster Analysis

#### Cluster 0:
* Mostly parents in mid 30s to 40s
* Almost all of them did NOT accept the offers
* Most had a graduate education and were 'together' with a partner
* They earned some of the higher income but also spent the least amount of money

#### Cluster 1:
* Mostly non-parents in mid 30s to mid 50s
* Most did not accept the offer but the distribution was closer than cluster 0
* Also highly educated with mostly graduate degrees and post-grad
* Most were together with a partner
* Much more spread out when comparing income to amount spent. Cluster 1 definitely spent much more than cluster 0 while earning a little more income on average

#### Cluster 2:
* Almost exclusively parents in mid 40s to upper 50s
* Most did not accept the offer, similar to cluster 0
* Also highly educated with most having graduate and post-grad
* Mostly together with a partner, by a wider margin than clusters 0 and 1
* Similar income range for cluster 1 but spent less on average than cluster 1
