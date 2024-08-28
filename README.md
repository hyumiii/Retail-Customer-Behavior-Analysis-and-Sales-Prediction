# Online Retail Sales Data Analysis

(See "Segmentation_and Prediction_Model.ipynb" for the full code)
<br>

## Introduction
This project aims to analyze an online retail sales database to identify customer segments and predict sales levels for each segment. By leveraging machine learning, the model aims to enhance business strategies through targeted marketing, optimized inventory management, and improved customer satisfaction.

## Approach 

The project is divided into two main components:

1. **Customer Segmentation**: Clustering algorithms were used to segment customers based on demographics and purchasing behaviours. This segmentation allows for targeted marketing campaigns, personalized customer experiences, and efficient resource allocation.

2. **Segmented Sales Prediction**: After the customer segments are identified, prediction models are implemented to forecast sales levels for each segment. The Random Forest model was selected for its superior performance in capturing non-linear relationships within the data, outperforming other models such as Linear Regression. This model allows for improved inventory forecasting, planning, risk management, and optimization of spending. 

<br>

## Results and Recommendations


#### 1. Customer Segmentation Model
- **Clusters Identified**: The unsupervised learning model identified four optimal clusters based on customer demographics and purchasing behavior (see Figure 13), as suggested by the elbow method (see Figure 12). Each cluster represents a distinct segment of the customer base, characterized by age groups and product category preferences:

- #### **Cluster 0 (Ages 51-87):**  
  - **Findings:** Preference for beauty, personal care, and home products, with a focus on self-care, comfort, brand loyalty, and less price sensitivity. They value quality and reliability.
  - **Insights:** Emphasize product reliability and health benefits through traditional media and targeted online campaigns. Develop products that focus on ease of use, ergonomics, and health-oriented features.

- #### **Cluster 1 (Ages 31-50):**  
  - **Findings:** Interest in home and food products, driven by the balance of family life and career, with a focus on value, convenience, and quality.
  - **Insights:** Highlight product efficiency, family benefits, and cost-effectiveness, especially during key seasons. Develop multi-functional or eco-friendly home products and time-saving meal solutions.

- #### **Cluster 2 (Ages 21-40):**  
  - **Findings:** Strong inclination towards electronics and food, driven by tech-savviness, convenience, and trend-following, with less brand loyalty and a preference for online shopping.
  - **Insights:** Utilize social media, influencer partnerships, and highlight trendy product features. Innovate in smart home tech and health-oriented convenience foods.

- #### **Cluster 3 (Ages 0-30):**  
  - **Findings:** Interest in electronics and beauty/personal care products, with a focus on innovation, personal image, price sensitivity, and strong social media influence.
  - **Insights:** Focus on visually appealing ads on social platforms, use promotions and discounts. Develop affordable, trendy electronics, and eco-friendly beauty products.

**Overlapping Age Groups**: For the model going forward, the clusters were consolidated from 4 to 3. This decision was due to overlapping age groups. Cluster 2 has age groups that overlaps with Cluster 3 and Cluster 1. This approach is to streamline the model and focus on distinct segments that exhibit unique purchasing patterns.

<br>

#### 2. Sales Prediction Model
- **Model Performance**: The Random Forest model outperformed Linear Regression in predicting sales levels across all segments. This model is recommended for ongoing sales predictions due to its ability to handle complex, non-linear relationships within the data.
- **Cluster 1**: Young and youngest demographics show significantly improved prediction accuracy in the Random Forest model, likely due to the model's ability to handle the variability and complexities of younger consumer behavior.
- **Cluster 2**: The middle-aged segment also demonstrated better results with Random Forest, suggesting that this model is more adept at forecasting for groups with varied product interests.
- **Cluster 3**: The oldest demographic showed the most substantial improvement in prediction accuracy with Random Forest, underscoring its effectiveness in dealing with segments that may have more stable but diverse purchasing patterns.

<br>

## Setup

To get started with the project, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/hyumiii/Retail-Customer-Behavior-Analysis-and-Sales-Prediction.git
   cd Retail-Customer-Behavior-Analysis-and-Sales-Prediction
   ```

2. **Install Required Packages**:
   Ensure you have Python installed, then install the required packages using pip:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Model**:
   You can run the model using the following command:
   ```bash
   python main.py
   ```

4. **View Results**:
   Results, including customer segmentation and sales predictions, will be displayed in the console and saved as output files in the `/results` directory.
   
## Future Work

- **Explore Alternative Predictive Models**: Investigate advanced models like XGBoost, LightGBM, or neural networks for potentially improved accuracy.
- **Continuous Model Tuning**: Periodically reevaluate and fine-tune models to adapt to changing customer behaviors and market conditions.
- **Dashboard Development**: Develop an interactive Tableau dashboard to visualize consumer behavior and optimize business strategies.
- **Implement Tailored Marketing Strategies**: Use segmentation insights to precisely target marketing efforts, boosting engagement and sales conversions.
- **Optimize Inventory Management**: Use predictive insights to align inventory with demand, reducing both overstocks and stockouts.

    #### Future Questions to Explore
    - How do external factors such as economic changes, market trends, and seasonal effects influence customer purchasing behaviors and model predictions?
    - How does brand loyalty vary across different customer segments and how can this influence new product launches or rebranding efforts?
    - How do our products perform in comparison to competitors within each customer segment?
    - Can we track changes in customer behavior over time to predict future trends more accurately?
    - What improvements can be made by integrating real-time data feeds into the prediction models to capture up-to-the-minute trends and behaviors?
    - Can analyzing customer feedback and sentiment provide deeper insights into the effectiveness of current marketing strategies and product positioning?
        
    By acting on these insights and exploring these questions, this online retail business can not only enhance its operational efficiency and drive better customer engagement but also maintain a competitive edge in a rapidly evolving market landscape.

<br>

## Next Steps

The next phase involves developing an interactive Tableau dashboard to:
- Visualize Consumer Behavior
- Optimize Marketing Spend
- Manage Inventory
- Implement Targeted Discount Strategies
- Enhance strategic decision-making and operational efficiency

This dashboard will streamline operations, enhance strategic decisions, and contribute to sustained business growth by providing a comprehensive overview of key business metrics.
[Visit Dashboard](https://public.tableau.com/app/profile/yuting.hu5191/viz/Project_17246389172000/Dashboard1)
