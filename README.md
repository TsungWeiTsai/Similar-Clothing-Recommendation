# Similar-Clothing-Recommendation
A method that identifies similar products based on low dimensional product representations and the ensemble learning 


# Motivaiton

### Possible applications/scenarios of similar clothing/product recommendaitons:
*	Recommend similar products to users on the e-commerce platforms such as Taobao and Amazon based on their browsing history or explicit queries.
* Able to conduct market/competitor analysis on a specific product and its similar products which often target same groups of customers. 


### Main features of the method:
*	Word embedding
  - Trained a set of low dimentional Chinese word representaions based on millions of Weibo posts
  - Complemented Bag-of-Words model by capturing syntactic and semantic meaning

2.	Negative sampling: most of the item pairs are not similar
the original item pairs cannot represent the population as the distribution differs
because of its small size and the sampling bias generated when we built the data set (to save time and money)
3.	EasyEnsemble
Deal with imbalanced data, make good use of information we dropped 

4.	Using NLP: 常见平台上图片不是那么标准 如同一搬论文中的那嬷干净 常常会有很多人像 街景 …等遮蔽/干扰，用NLP可以忽视/弥补这个劣势 (from practical perspective)???

