# Similar-Clothing-Recommendation
A method that identifies similar products based on low dimensional product representations and the ensemble learning 


# Motivaiton

### Applications
*	Recommend similar products to users on the e-commerce platforms such as Taobao and Amazon based on their browsing history or explicit queries.
* Able to conduct market/competitor analysis on a specific product and its similar products which often target same groups of customers. 


### Main features of our method:
* Natural Language Processing:
  * It is common to encounter pictures that are not "clean"
  * As far as we know, there is no related researches on finding similar clothing based on natural language features, all of them extract     feature from pictures. 
  * Features based on product descriptions can complement those from computer vision. The proposed method can easily incorporate with         image processing approaches to create more robust recommendation system.

*	Word embedding:
    * Trained a set of low dimensional Chinese word representations based on millions of Weibo posts
    * Complement Bag-of-Words model
    * Strengthened the learned representation of product descriptions by using word embedding to capture semantic and syntactic
      patterns. Word embedding can effectively measure the similarity between words.
      
* EasyEnsemble
  * Originally from [Exploratory Undersampling for Class-Imbalance Learning](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/tsmcb09.pdf)
  * Exploit the information from majority class to deal with seriously imbalanced data
  * It is costly to get enough labeled dataset. EasyEnsemble enabled us to “reuse”existing minority class samples to certain extent.            However, we have to make sure that the minority samples are diversified enough to represent general features of similar product pairs

* Negative sampling
    * Due to the nature of clothing market, most of the random pairs of clothes are not similar item pairs. Hence, we can treat unlabeled item pairs as negative class (not similar) with low probability labeling a pair of similar products as negative case.
    

# Data

# Framework

# Performance

