

Advanced Market Segmentation Using Deep Clustering

Targeting Customers with Deep Learning
Data Preprocessing
I cleaned the dataset through several important steps:

Handling Missing Data: Missing values were addressed using forward filling, ensuring no gaps that could affect the analysis.
Correcting Shipping Durations: I handled cases where shipping durations were negative or unreasonable.
Normalization and Encoding: To prepare the data for model input, numerical features were normalized, and categorical features were one-hot encoded.
These preprocessing steps ensured a clean and consistent dataset, ready for feature extraction and modeling.

Feature Engineering
To help the model identify customer segments more effectively, I created new features:

Customer Lifetime Value (CLV): Measures the total value a customer has provided based on their purchase history.
Purchase Frequency: Represents the number of purchases made by a customer.
Profit Margins: Calculated as the ratio of profit to sales per order, helping identify more profitable customers.
Deep Learning Model
I used an autoencoder to reduce the high-dimensional data into a compressed, lower-dimensional form. This allowed for more efficient clustering of customer behaviors while retaining important features.

The autoencoder was able to reduce the dataset to eight essential features, which captured key aspects of customer behavior. These compressed features were then used for clustering.

Clustering and Results
After reducing the data dimensionality, I applied K-Means clustering to categorize customers into four distinct segments. The number of clusters was determined using the Elbow Method and confirmed with evaluation metrics like the Silhouette Score.

The Four Customer Segments:
Segment 0 (High-Value, Frequent Shoppers)

Contains slightly more than 3000 customers.
These customers tend to make frequent and high-value purchases, contributing significantly to revenue.
Segment 1 (Mid-Spending, Occasional Shoppers)

Consists of around 2500 customers.
This group is more selective and makes purchases occasionally, but with a higher spending capacity than some other segments.
Segment 2 (Price-Sensitive, Medium Engagement)

The second largest group, containing around 4500 customers.
These customers are more price-sensitive and often make lower-value purchases. However, they still engage regularly with the business.
Segment 3 (Low-Engagement, Low-Spending)

The largest segment, with approximately 5000 customers.
This group is characterized by infrequent purchases and lower spending, often opting for budget products or waiting for discounts.
Visualizations:
I used Principal Component Analysis (PCA) to reduce the clustered data into two dimensions for visualization. The resulting plots clearly showed the separation between the four segments, validating the effectiveness of the clustering approach.

These insights are critical for businesses, as they highlight different customer personas. Each segment represents a unique opportunity for targeted marketing and engagement strategies. For example, Segment 0 could benefit from loyalty programs, while Segment 3 might need price incentives to encourage more frequent purchasing.

Conclusions
This project successfully demonstrated how deep learning and clustering can be used to uncover customer segments in a real-world dataset. By segmenting the customers into four distinct groups, businesses can better understand customer behavior and develop more targeted marketing campaigns.

Future Work
In future iterations of this project, I aim to:

Experiment with Advanced Clustering Techniques: Techniques like DBSCAN or Hierarchical Clustering could provide even more nuanced customer groupings.
Incorporate More Features: Adding features like customer feedback, return rates, and web activity could provide deeper insights into customer behavior.
Develop Predictive Models: Using these customer segments as input for predictive models could help forecast future customer behavior, such as churn or lifetime value.





Installation

1. Clone the Repository

git clone https://github.com/your-username/your-repository.git
cd your-repository

2. Create a Virtual Environment

python -m venv venv
source venv/bin/activate   # On macOS/Linux
venv\Scripts\activate      # On Windows

3. Install Dependencies

pip install -r requirements.txt

4. Run the Application

python app.py


---

Usage

Train the Model: Run train.py to train the deep clustering model

Make Predictions: Use the API to segment new customers

View Dashboard: Open the frontend UI to visualize customer clusters






Contributors

Sujan J 

B K CharuKeerthy Reddy



