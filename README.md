# Ecommerce-Product-Recommendation-System-using Machine Learning on Amazon & Home Depot's Dataset

A well developed recommendation system will help businesses improve their shopper's experience on website and result in better customer acquisition and retention.

The recommendation system, I have designed below is based on the journey of a new customer from the time he/she lands on the business’s website for the first time to when he/she makes repeat purchases.

The recommendation system is designed in 3 parts based on the business context:

The datasets are from
  1. Amazon product ratings by multipe users, Data Source: https://www.kaggle.com/skillsmuggler/amazon-ratings
  2. Home Depot's Product and description:  https://www.kaggle.com/c/home-depot-product-search-relevance/data
 
The recommendation system is designed in 3 parts based on the business context:

When a new customer without any previous purchase history visits the e-commerce website for the first time, he/she is recommended the most popular products sold on the company's website. Once, he/she makes a purchase, the recommendation system updates and recommends other products based on the purchase history and ratings provided by other users on the website. The latter part is done using collaborative filtering techniques.

Strategy/Techniques used:

**1) Product popularity based recommendation system targeted at new customers:**

Popularity based are a great strategy to target the new customers with the most popular products sold on a business's website and is very useful to cold start a recommendation engine.

**2) Model-based collaborative filtering system:**
Recommend items to users based on purchase history and similarity of ratings provided by other users who bought items to that of a particular customer.

A model based collaborative filtering technique is closen here as it helps in making predictinfg products for a particular user by identifying patterns based on preferences from multiple user data.

**3) Item-item based collaborative filtering system:**
For a business without any user-item purchase history, a search engine based recommendation system can be designed for users. The product recommendations can be based on textual clustering analysis given in product description. Predictions done based on other products from the same cluster (based of text analysis of product description) on key search words.
