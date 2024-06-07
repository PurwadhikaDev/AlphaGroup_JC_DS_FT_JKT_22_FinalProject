### **DATA SOURCE:**

[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## **Background**

### **Company Overview**

Olist is a Brazilian-based e-commerce platform that connects small and medium-sized retailers with large online marketplaces. Founded in 2015 by Tiago Dalvi, Olist aims to democratize online selling by providing tools and services that help businesses scale and reach a broader audience. The company's mission is to empower entrepreneurs and retailers by simplifying the complexities of e-commerce, thus enabling them to compete more effectively in the digital marketplace.

This project focuses on exploring, cleaning, and analyzing the Olist Public E-commerce Dataset to support customer segmentation efforts. Leveraging machine learning clustering techniques, our objective is to extract actionable insights from the data, predicting customer satisfaction levels and the likelihood of repeat purchases. By doing so, we aim to equip Olist with valuable business insights to optimize growth opportunities, enhance sales performance, and further empower entrepreneurs and retailers within the competitive digital landscape.



### **Business Model**

Olist operates on a B2B2C (Business to Business to Consumer) model, providing a comprehensive suite of services designed to simplify the e-commerce process for retailers. Key offerings include:

- **Marketplace Integration**: Olist allows retailers to list their products across multiple marketplaces through a single platform, increasing their visibility and sales potential.

- **Logistics Solutions**: The company offers end-to-end logistics support, including warehousing, packaging, and shipping, ensuring timely and reliable delivery to customers.

- **Customer Service**: Olist provides customer service support, handling inquiries and issues on behalf of retailers to maintain high customer satisfaction levels.

- **Marketing Tools**: The platform includes marketing and analytics tools that help retailers optimize their sales strategies and track performance metrics.



### **Problem Background**

In the competitive e-commerce industry, customer churn—where customers stop doing business with a company—ranges from 20% to 40% annually. High churn rates typically signal problems with customer satisfaction or service quality.

Olist, despite its innovative services and comprehensive support, faces a significant challenge with a churn rate of 70.41%. This rate is considerably higher than the industry average, indicating a critical need for strategies to enhance customer retention and satisfaction.

Customer churn is closely tied to customer loyalty. Loyal customers are less likely to switch to competitors and more likely to make repeat purchases, directly impacting a company's revenue. Olist's comprehensive services, including excellent customer support and efficient logistics, aim to boost customer loyalty.

Customer loyalty is crucial for sales performance. Loyal customers contribute to higher revenue through repeat purchases and referrals. By using advanced analytics and machine learning to understand and enhance customer satisfaction, Olist can further reduce churn and increase sales, supporting its mission to empower entrepreneurs and retailers in the digital marketplace.



## **Problem Statement**

Despite Olist's innovative services and comprehensive support, it faces a critical challenge with a churn rate of 70.41%, significantly higher than the industry average. This indicates a pressing need for strategies to enhance customer retention and satisfaction. A key issue exacerbating this problem is Olist's lack of an accurate predictor for identifying customers at risk of churning.


## **Goals**
To reduce Olist's churn rate from 70.41% to below the industry average by implementing advanced predictive analytics to accurately identify customers at risk of churning. This will enable the development of proactive strategies to enhance customer satisfaction and loyalty, leading to sustained business growth.



## **Analytical Approach**

Analytical Approach:

1. **Data Collection and Preparation:**
   - Gather comprehensive customer data including purchase history, frequency of purchases, recency of purchases, monetary value, demographic information, and interactions with customer support.
   - Ensure data quality and integrity through cleansing and validation processes.

2. **RFM Analysis:**
   - Utilize RFM analysis to segment customers based on their Recency, Frequency, and Monetary value.
   - Identify high-value customers who are at risk of churn despite their monetary contributions.
   - Determine patterns and trends among different customer segments to understand their behaviors and preferences.

3. **Churn Prediction Modeling:**
   - Develop predictive models using machine learning algorithms to forecast customer churn probability.
   - Incorporate RFM metrics along with other relevant features such as customer interactions, product preferences, and satisfaction scores.
   - Validate and fine-tune the models using historical data to ensure accuracy and reliability.



## **Assumption & Limitation**

**Assumptions**

- Assume datasets accurately represent Olist's operations.

- Assume data is a representative sample.

- Assume relatively stable market conditions.

- Assume the price and sales income use the Brazilian real, the official currency of Brazil.

**Limitations**

- The datasets contain information from 2016 to 2018 and may not capture recent changes.

- Dataset may not cover all aspects of operations.

- Analysis focuses on the Brazilian market.


## **Evaluation Metrics**

For this classification task, we have chosen the F1 score as our primary evaluation metric. The F1 score is particularly suitable for imbalanced datasets, which is a common scenario in churn prediction where the number of churned customers is usually much smaller compared to non-churned customers. The F1 score is the harmonic mean of precision and recall. It provides a single metric that balances both Precision and Recall. 

By focusing on the F1 score, we ensure that our model maintains a good balance between correctly identifying churned customers and minimizing false alarms, making our predictions more reliable and effective for business interventions.


# **Conclusion & Recommendation**

### **Conclusion**

**Conclusion:**

Based on the insights derived from the provided data on customer churn across various segments, payment types, product categories, cities, and states in Brazil, here are the conclusions:

1. **Segment-specific Insights**:
   
   - **Champions and Loyal Customers**: These segments exhibit high loyalty and engagement, with a significant majority not churning. They represent stable revenue streams and should be prioritized for retention strategies.
   
   - **Potential Loyalists and Promising**: These segments show promise with a balanced mix of potential loyalty and churn possibilities. Targeted efforts can convert potential loyalists into long-term customers.
   
   - **Need Attention and At Risk**: These segments have higher churn probabilities and require immediate attention. Proactive retention measures are crucial to mitigate further losses.
   
   - **About To Sleep, Cannot Lose Them, Hibernating Customers**: These segments show critical signs of churn or inactivity. Reactivation strategies for dormant customers and intensive retention efforts for high-value customers are necessary.

2. **Payment Behavior Analysis**:
   
   - **Credit Card Dominance**: Across most segments, credit cards are the preferred payment method, indicating convenience and widespread acceptance.
   
   - **Boleto Usage**: Varied adoption among different segments suggests a need for flexible payment solutions tailored to customer preferences.
   
   - **Debit Card and Voucher**: These methods show varying degrees of usage, with potential growth opportunities in segments showing lower current adoption rates.

3. **Product Category Preferences**:
   
   - **Popular Categories**: Categories like "Bed Bath Table," "Health Beauty," and "Sports Leisure" attract significant customer interest but also experience higher churn rates. Enhanced customer engagement strategies could improve retention.
   
   - **Niche Categories**: Categories such as "Telephony" and "Auto" attract fewer orders but may indicate specialized customer needs that could be targeted with niche marketing strategies.

4. **Regional Insights**:
   
   - **City-level Analysis**: Cities like Sao Paulo and Rio de Janeiro exhibit both high order volumes and substantial churn rates, suggesting competitive markets requiring robust retention strategies.
   
   - **State-level Analysis**: States like Minas Gerais, Paraná, and Santa Catarina consistently show high churn rates, indicating regional trends that may require localized approaches to customer retention.

5. **Best Churn Predictor Model:**
   
   - After performing grid search cross-validation, the Random Forest model was selected based on the F1 score, which is crucial for imbalanced datasets. The model demonstrates an F1-score of 97.22% after tuning, indicating robust performance in predicting churn accurately.



### **Recommendation**

1. **Champions**:
   
   Offer exclusive incentives like additional discounts or early access to new products to enhance their membership value. VIP loyalty programs can strengthen long-term brand relationships.
   
   Actions:

   - Continue to facilitate transactions with credit cards (80%) and offer exclusive cashback rewards or discounts on their preferred categories like "Bed Bath Table" (66.96% of the segment's transactions).
   
   - Implement free shipping on all orders or provide expedited shipping options to enhance their shopping experience and maintain loyalty.

2. **Loyal**:
   
   Develop personalized communications and relevant content to maintain engagement. Offer bonuses or discounts based on their purchase history to encourage repeat transactions.

   Actions:

   - Maintain their loyalty with ongoing discounts and rewards on credit card transactions (72%), focusing on categories such as "Health Beauty" (91.12% of the segment's transactions).
   
   - Offer free shipping on orders above a certain value to incentivize higher purchase volumes and reinforce their loyalty.

3. **Potential Loyalist**:
   
   Improve the buying experience with superior customer service and fast delivery. Special onboarding programs or product trials can help them discover added value.

   Actions:
   
   - Encourage initial purchases with flexible payment options including credit cards (60%) and boleto (40%), coupled with discounts on categories like "Furniture Decor" (55.78% of the segment's transactions).
   
   - Use free shipping promotions to convert potential customers, particularly on their first purchase, to increase conversion rates.

4. **New Customers**:
   
   Provide proactive follow-ups after their first purchase, such as product guides or exclusive offers for subsequent purchases. Focus on a positive customer experience from the outset.

   Actions:
   
   - Simplify their first purchase with popular payment methods such as credit cards (55%) and boleto (45%), offering introductory discounts on categories like "Housewares" (54.37% of the segment's transactions).
   
   - Provide free shipping on their initial order to reduce barriers to purchase and encourage repeat shopping.

5. **Promising**:
   
   Use purchase behavior analysis to offer relevant product recommendations or cross-selling to increase basket value. Regular discounts or exclusive benefits can maintain their interest.

   Actions:
   
   - Engage frequent purchasers with rewards and discounts on credit card transactions (68%) for categories like "Bed Bath Table" (60.47% of the segment's transactions).
   
   - Offer free shipping on orders exceeding average purchase values to stimulate larger transactions and foster repeat business.

6. **Need Attention**:
   
   Proactively identify and address customer concerns or issues. Offer problem-solving solutions or deeper customer service to improve satisfaction.

   Actions:
   
   - Regain their interest with targeted promotions on credit card payments (62%) and discounts on categories they favor, such as "Sports Leisure" (60.36% of the segment's transactions).
   
   - Provide competitive shipping rates and occasional free shipping offers on selected products to win back their purchasing commitment.

7. **About To Sleep**:
   
   Activate reactivation campaigns with special offers or incentives to encourage repeat purchases. Review customer lifecycle and consider targeted strategies to re-engage them.

   Actions:
   
   - Activate reactivation campaigns with discounts on credit card transactions (100%) for categories like "Health Beauty" (100% of the segment's transactions).
   
   - Reinforce incentives with free shipping promotions to prompt their return to active purchasing.

8. **Cannot Lose Them**:
   
   Prioritize retention by identifying any dissatisfaction or issues they may have. Offer VIP treatment, exclusive discounts, or priority service to retain these valuable customers.

   Actions:
   
   - Preserve their loyalty with significant discounts and exclusive offers on credit card payments (100%) for categories they consistently purchase, such as "Health Beauty" (100% of the segment's transactions).
   
   - Ensure seamless transactions with free shipping on all orders to solidify their continued patronage.

9. **At Risk**:
   
   Follow up promptly to identify potential churn reasons and offer relevant solutions or improvements. Use strong reactivation strategies with exclusive offers or discounts to influence their decision to stay.

   Actions:
   
   - Retain these customers by offering compelling discounts on credit card transactions (100%) for favored categories like "Sports Leisure" (100% of the segment's transactions).
   
   - Implement time-sensitive free shipping promotions to re-engage their interest and reduce the likelihood of churn.

10. **Hibernating Customers**:

   Activate reminder or stimulation campaigns to rekindle their interest. Provide incentives for repeat purchases or offers on products relevant to their previous purchases.
   
   Actions:
   
   - Revive their interest with discounts on credit card payments (100%) for categories they previously purchased, such as "Furniture Decor" (100% of the segment's transactions).
   
   - Offer free shipping incentives on their next purchase to encourage them to resume shopping with your brand.

By tailoring both payment type and freight value strategies to match the preferences and behaviors of each customer segment, the company can effectively enhance customer retention efforts. These personalized approaches not only cater to specific segment needs but also aim to increase customer satisfaction, loyalty, and lifetime value.
