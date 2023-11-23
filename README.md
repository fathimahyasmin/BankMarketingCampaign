## **Business Understanding**

### **Context:**
Banks need to maintain their liquidity ratio to ensure that cash needs are continuously met. This ratio indicates a bank's ability to handle short-term financial responsibilities, which includes providing loans to consumer and business. The more cash reverse a bank maintains, the greater its ability to provide loans and generate profits. 

One way for them to keep this ratio in check is by offering term deposit investments to customers. **Term deposits are a type of investment where customers commit a certain amount of money to a bank or financial institution that cannot be withdrawn for a set period.** In return, customers receive a fixed interest rate on the amount they deposit. 

Portuguese banks conduct telemarketing campaigns to promote term deposit investments, contacting customers believed to be potential investors. To improve the effectiveness of these campaigns, the banks aim to predict which customers are likely to open term deposits. Accurate predictions enable the banks to focus on promising customers, thereby reducing the financial losses from misdirected campaign efforts.

### **Problem Statement:**
The Mass Funding Division plays a crucial role in securing the funds needed for the bank's everyday operations and its larger financial strategy. One way they do this is through term deposits. These are a reliable source of funds, offering low risk and steady returns. However, there's a challenge: term deposits require a long-term commitment and offer fixed returns, which makes them less appealing in a market where many people want investments with higher returns.

To tackle this, the division uses targeted telemarketing campaigns, involving repetitive calls to gauge customer interest. But this method can be time-consuming and costly if not done effectively. If the division just relies on manual methods to identify potential customers, it could lead to biased and inaccurate predictions. This means they could end up targeting the wrong people, wasting time and money.

To improve the effectiveness of their marketing efforts, a more strategic approach is needed. By using a precise classification model, the division can focus on customers who are more likely to open term deposits. This way, they can run more efficient campaigns and make better use of their resources.

By employing a classification model that not only prioritizes accurate predictions but also takes profitability into account, Mass Funding Division can strategically target customers who are more likely to open term deposits. This approach allows this division to optimize campaigns and resource allocation, ultimately enhancing their profitability. 

To develop a solution, we need to consider these key questions:

**`Key Questions:`**
- Which factor or variable should the Mass Funding division focus on to enhance term deposit sign-ups?
- How can the Mass Funding Division forecast customer likelihood to commit to term deposits?


### **Goals:**

The main goal here is to **create an effective classification model**. This model's job is to predict how likely it is that clients will choose term deposits. It's important that this model is good at predicting both clients that will say yes and they who will say no to term deposits.

Also, we want to **understand what makes customers decide to sign up for term deposits**. Knowing these key factors will help banks use their resources better, make their interactions with clients more effective, and ultimately, get more clients to agree to term deposits through their marketing.


### **Analytical Approach:**
We analyze the characteristics of potential customers who are likely to open a term deposit account and then build a supervised machine learning model, specifically a classification model, to predict which prospects are inclined to open a term deposit account. This way, these potential customers can be prioritized in the campaign, making the process more efficient.

### **Metric Evaluation:**

This analysis will focus on customers interested in investing in term deposits. The targets are defined as follows:

- **0:** indicates a customer who does not invest in a term deposit.
- **1:** represents a customer who invests in a term deposit.

Ensuring the accuracy of our model is crucial to avoid the financial repercussions of misclassification, which could come in the form of false positives or false negatives.

| **Error Type**     |**Explanation** | **Consequences** | 
|-----------------|------------|----------------|
| **False Positive / Type 1 Error**  |This occurs when the model incorrectly predicts that a customer will invest in a term deposit when they actually will not. In other words, the model's prediction is positive (1), but the true value is negative (0)| The bank will incur unnecessary marketing expenses by targeting customers who are not interested in investing in term deposits.|
| **False Negative / Type 2 Error**  |This happens when the model incorrectly predicts that a customer will not invest in a term deposit when they actually will. Here, the model's prediction is negative (0), but the true value is positive (1)| The bank will miss out on potential profits from customers who are likely to invest in term deposits.| 

