# Ecommerce-Product-Recommendation-System-using Machine Learning on Amazon & Home Depot's Dataset

A well developed recommendation system will help businesses improve their shopper's experience on website and result in better customer acquisition and retention.

The recommendation system, I have designed below is based on the journey of a new customer from the time he/she lands on the business’s website for the first time to when he/she makes repeat purchases.

The recommendation system is designed in 3 parts based on the business context:

The **datasets** are from
  1. Amazon product ratings by multipe users, Data Source: https://www.kaggle.com/skillsmuggler/amazon-ratings
  2. Home Depot's Product and description:  https://www.kaggle.com/c/home-depot-product-search-relevance/data
 
The recommendation system is designed in 3 parts based on the business context:

When a new customer without any previous purchase history visits the e-commerce website for the first time, he/she is recommended the most popular products sold on the company's website. Once, he/she makes a purchase, the recommendation system updates and recommends other products based on the purchase history and ratings provided by other users on the website. The latter part is done using collaborative filtering techniques.

Strategy/Techniques used:

**1) Product popularity based recommendation system targeted at new customers:**

Popularity based are a great strategy to target the new customers with the most popular products sold on a business's website and is very useful to cold start a recommendation engine.

**2) Model-based collaborative filtering system:**
Recommend items to users based on purchase history and similarity of ratings provided by other users who bought items to that of a particular customer.

A model based collaborative filtering technique is chosen here as it helps in making predicting products for a particular user by identifying patterns based on preferences from multiple user data.

**3) Item-item based collaborative filtering system:**
For a business without any user-item purchase history, a search engine based recommendation system can be designed for users. The product recommendations can be based on textual clustering analysis given in product description. Predictions done based on other products from the same cluster (based of text analysis of product description) on key search words.

**Recommendation system part I: Product pupularity based system targetted at new customers:**

**Product popularity based recommendation system targeted at new customers**

Popularity based are a great strategy to target the new customers with the most popular products sold on a business's website and is very useful to cold start a recommendation engine.

![popularity graph](https://user-images.githubusercontent.com/78776711/114181246-e7ced700-995e-11eb-83fb-7862bda8b2e1.PNG)

**Analysis:**
The above graph gives us the most popular products (arranged in descending order) sold by the business. For eaxmple, product, ID # B001MA0QY2 has sales of over 7000, the next most popular product, ID # B0009V1YR8 has sales of 3000, etc.

**Recommendation system part II:**

**Model-based collaborative filtering system based on customer's purchase history and ratings provided by other users who bought items similar items**

Recommending top 10 highly correlated products in sequence based on a customer's purchase history:

![top10_correlated_product](https://user-images.githubusercontent.com/78776711/114181478-2e243600-995f-11eb-8b83-c32ff227c9ec.PNG)

**Conclusion:**
Product Id #: Here are the top 10 products to be displayed by the recommendation system to the above customer based on the purchase history of other customers in the website.

**Recommendation system part III:**
Cold start problem for new businesses: When a business is setting up its e-commerce website for the first time without any historical data on product rating
For a business without any user-item purchase history, a search engine based recommendation system can be designed for users. The product recommendations can be based on textual clustering analysis given in product description.

**Visualizing product clusters in subset of data:**

![product_cluster](https://user-images.githubusercontent.com/78776711/114181489-32505380-995f-11eb-9be5-01b95a94f35c.PNG)

**Top words in the first 3 clusters based on text analysis and clustering techniques applied to product description:**

**Top terms per cluster:**

Cluster 0: m12 battery devices charge light fuel
 
Cluster 1: power air volt cutting watt cooling light

Cluster 2: metal water concrete use ft provides seal

**Recommendation Technique:**
Once a cluster is identified based on the user's search words, the recommendation system can display items from the corresponding product clusters based on the product descriptions.

**Summary:**
This works best if a business is setting up its e-commerce website for the first time and does not have user-item purchase/rating history to start with initally. This recommendation system will help the users get a good recommendation to start with and once the buyers have a purchased history, the recommendation engine can use the model based collaborative filtering technique.
