# Instagram Influencer Dataset Analysis

## 📊 Dataset Overview

Instagram is a widely used social networking platform for sharing photos and videos, established in 2010 by Kevin Systrom and Mike Krieger, later acquired by Facebook Inc. Users can upload media, apply filters, organize posts with hashtags, and share content publicly or with approved followers. This network has grown into a powerful platform for influencer marketing, where users with large follower counts can shape opinions and influence purchasing decisions.

**Source:** Kaggle (https://www.kaggle.com/datasets/surajjha101/top-instagram-influencers-data-cleaned)

The dataset includes 200 entries of top Instagram influencers across industries, with attributes such as:

- **Influencer Name**
- **Influencer Score**
- **Follower Count**
- **Engagement Rate**
- **Average Likes**
- **Number of Posts**
- **60-Day Engagement Rate**
- **New Post Average Likes**
- **Country**

This data helps analyze factors contributing to influencer performance and guides brands in making strategic decisions for influencer partnerships.

## 🧠 Analytical Approach

### 🛠️ 1. Data Cleaning and Preprocessing

- **Handling Missing Values:**
  - Checked for null values using `missingno`, and confirmed no gaps in the data.

- **Data Type Conversion:**
  - Converted 'Posts' to a numeric format (e.g., '3.3k' → 3300).

- **Removing Redundant Features:**
  - Dropped the 'Rank' and 'Channel Info' attributes after using them for initial sorting.

- **Country Grouping:**
  - Ranked countries based on influencer density to simplify clustering analysis.

### 🔍 2. Exploratory Data Analysis (EDA)

- **Distribution of Influencers Across Countries:**
  - Visualized with a count plot, showing the USA, India, and Brazil as top influencer hubs.

- **Engagement and Influence Metrics:**
  - Histograms and KDE plots for influence score, followers, likes, and posts.
  - Marked means with vertical lines for better interpretability.

- **Top 10 Influencers by Key Metrics:**
  - Bar charts for the top 10 influencers in followers, likes, and posts.

- **Correlation and Outliers:**
  - Pair plots revealed positive correlations between likes and followers.
  - Boxplots displayed outliers, especially in follower and like counts.

### 🔑 3. Cluster Analysis

- **K-Means Clustering:**
  - Applied the Elbow method to find 4 optimal clusters.

- **Cluster Characteristics:**
  - **Cluster 1:** Mega influencers with high followers but lower engagement.
  - **Cluster 2:** Micro-influencers with small but highly engaged audiences.
  - **Cluster 3:** Balanced influencers with mid-level followers and steady growth.
  - **Cluster 4:** Outliers with exceptionally high engagement.

## 📊 Visualizations

- **Count Plot:** Distribution of influencers by country.
- **Histograms & KDE Plots:** Distribution and density of numerical features.
- **Bar Charts:** Top 10 influencers by posts, likes, and followers.
- **Pair Plot:** Feature correlations with regression lines.
- **Boxplots:** Outlier detection for each numerical feature.
- **Cluster Plot:** Optimal cluster selection with K-means and Elbow method.


## 📈 Key Insights and Business Implications

1. **Leverage Micro-Influencers:** Small, highly engaged audiences drive better interaction.
2. **Expand Global Reach:** Explore influencers in less saturated markets.
3. **Prioritize Engagement Metrics:** Focus on interaction rates over sheer follower counts.
4. **Target High-Engagement Outliers:** Use outlier influencers for viral campaigns.
5. **Category-Specific Strategies:** Tailor campaigns based on influencer niche.

## 🚀 Next Steps

- **Advanced Statistical Analysis:** Build regression models to quantify influencer success.
- **Predictive Modeling:** Use machine learning to forecast influencer performance.
- **Sentiment Analysis:** Analyze audience sentiment through post captions and comments.
