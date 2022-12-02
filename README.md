
# Customer Acquisition

With this project my aim is to create Customer profile as well as understand market mix or positioning of products which can be further utilized by marketing teams to curate marketing campaigns

## Roadmap

#### Segmentation

- Understand the data (Correlation,)

- Pre processed the data (scaling)

- Best cluster selection: 

        - Hierarchical clustering
        - Elbow method
- Applied K-mean clustering

- Look at cluster characterstics and name each accordingly

- To improve the cluster quality, I used PCA

- Components of PCA reduced the clustering features

- Understand the components vs clustering features through a heatmap

- Applied Kmean clustering on PCA results 

- Look at cluster characterstics and name each accordingly

- Visualized the result 

Result: The results produced have a clear customer Segmentation which can be used to curate campaigns.

#### Positioning

Helps in answering 3 questions:
1. Purchase probability
2. Brand choice probability
3. Purchase Quantity

### Purchase probability

- Applied cluster model on purchase data to understand customer Segment 

- Calculate visits per customer and purchase instance for each visit, further calculate purchase probability of each record (Purchase instance/ visit)

- Calculate purchase percentage for each Segment

- Check for homogeneity of each segment

### Brand Choice probability

- Between 5 brands, calculate which segment prefers which segment 

- For each segment, how much revenue is produced by each brand

- To check the purchase probability of a brand, I calculated Purchase elasticity

Purchase elasticity

Price Elasticity of purchase probability is the % change in purchase probability in response to a 1% change in price

- Applied Logistic regression on independent variable : Price and dependent variable : Incidence (0: Not purchased, 1: Purchased)

- Calculate percentage elasticity for each price Positioning for each segment

- If elasticity value < 1 than its inelastic

    General rule:
    
    - For inelastic values, general recommendation is to increase the price as it would not cause a significant decrease in output variable (purchase probability)

    - For elastic values, we should decrease our prices

- Now we know for which segments we can increase the price of the brand without loosing customers, and for which we need to decrease price to attract more revenue

- Elasticity exercise is tested against Promotions and without promotions

- Own brand effect: How modifying the price of your brand effect your brand

- Cross brand effect: How competitors modifying there price effect your brand

### Purchase Quantity

- Calculate Purchase elastictity using Quantity metrics
