# Video Game Sales Analysis: Clustering and Classification 🎮📊

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/Python-3.8%2B-green.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Clustering%20%26%20Classification-orange.svg)

Welcome to my project submission for the **Belajar Machine Learning Pemula** course by Dicoding! 🚀 This project focuses on analyzing video game sales data using **clustering** and **classification** techniques. The dataset used is **Video Game Sales with Ratings**, which includes sales data and ratings from Metacritic. Let's dive into the details! 🕹️

---

## 📁 About the Dataset

### **Context**
This dataset combines video game sales data from **VGChartz** with corresponding ratings from **Metacritic**. It includes information about game titles, platforms, genres, publishers, sales across different regions, and critic/user ratings. The dataset contains approximately **6,900 complete cases**.

### **Features**
Here are the key features in the dataset:

1. **Name**: Name of the game (e.g., "Wii Sports", "Super Mario Bros.").
2. **Platform**: Platform or console where the game was released (e.g., "Wii", "PS4").
3. **Year_of_Release**: Year the game was released (e.g., 2006, 1985).
4. **Genre**: Genre or category of the game (e.g., "Sports", "Action").
5. **Publisher**: Company that published the game (e.g., "Nintendo", "Electronic Arts").
6. **Sales Data**: Sales in millions of units for different regions:
   - **NA_Sales**: North America
   - **EU_Sales**: Europe
   - **JP_Sales**: Japan
   - **Other_Sales**: Other regions
   - **Global_Sales**: Total worldwide sales
7. **Ratings**:
   - **Critic_Score**: Aggregate score from Metacritic critics (0-100).
   - **Critic_Count**: Number of critics contributing to the score.
   - **User_Score**: Aggregate score from Metacritic users (0-10).
   - **User_Count**: Number of users contributing to the score.
8. **Developer**: Company or team that developed the game.
9. **Rating**: ESRB rating (e.g., "E" for Everyone, "T" for Teen).

---

## 🎯 Project Goals

The main objectives of this project are:
1. **Clustering**: Group video games into clusters based on their features (e.g., sales, ratings, genre).
2. **Classification**: Build a model to classify games into clusters using supervised learning techniques.

---

## 🛠️ Methodology

### **Clustering**
I used **K-Means Clustering** to group the games into **3 clusters** based on features like sales, ratings, and release year. Here's a summary of the clusters:

1. **Cluster 0**:
   - **Average Release Year**: 2008
   - **Low Critic and User Scores**: Critic Score: 56, User Score: 4.9
   - **Dominant Genre**: Action
   - **Dominant Platform**: X360
   - **Analysis**: Games in this cluster have low sales and ratings, targeting a general audience (Rating: E).

2. **Cluster 1**:
   - **Average Release Year**: 2006
   - **Moderate Critic and User Scores**: Critic Score: 71, User Score: 7.6
   - **Dominant Genre**: Action
   - **Dominant Platform**: X360
   - **Analysis**: Games in this cluster have higher sales and better ratings, targeting teens (Rating: T).

3. **Cluster 2**:
   - **Average Release Year**: 2006
   - **High Sales and Ratings**: Critic Score: 69, User Score: 7.6
   - **Dominant Genre**: Action
   - **Dominant Platform**: PS2
   - **Analysis**: Games in this cluster have the highest sales and quality, dominating the North American and European markets.

### **Classification**
After clustering, I used the cluster labels to train two classification models:
1. **Random Forest**:
   - Achieved **99.88% accuracy** after hyperparameter tuning.
   - Precision, Recall, and F1-Score: **99.88%**.
   - Robust and generalizes well to new data.

2. **Decision Tree**:
   - Achieved **99.88% accuracy** after hyperparameter tuning.
   - Precision, Recall, and F1-Score: **99.88%**.
   - Simple and interpretable but prone to overfitting.

---

## 📊 Results and Insights

- **Clustering**: The games were successfully grouped into 3 clusters based on sales, ratings, and other features. Each cluster represents a distinct market segment.
- **Classification**: Both Random Forest and Decision Tree models achieved **99.88% accuracy**, demonstrating excellent performance in predicting cluster labels.
- **Recommendations**:
  - Use cross-validation to ensure models generalize well to new data.
  - Explore other algorithms like Gradient Boosting or XGBoost for further improvements.
  - Analyze feature importance to understand which features contribute most to the predictions.

---

## 🚀 How to Use This Project

### Prerequisites
- Python 3.8+
- Libraries: `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/NovrianPratama/video-game-sales-analysis.git
2. Navigate to the project directory:
   ```bash
   cd video-game-sales-analysis

## 🤝 How to Contribute
Contributions are welcome! If you'd like to contribute:

1. **Fork** the project. 🍴  
2. **Create a new branch**:  
   ```bash
   git checkout -b feature/your-feature
3. **Make your changes and commit:**  
   ```bash
    git commit -m "Add some feature"
4. **Push to your branch:**  
   ```bash
    git push origin feature/your-feature

## 📧 Contact
If you have any questions or suggestions, feel free to reach out:

- Novrian Pratama - novrianprtama2@gmail.com
- GitHub Profile: NovrianPratama


### Key Sections:
1. **Project Structure**: A clear directory structure to help users navigate the project.
2. **How to Contribute**: Step-by-step instructions for contributing to the project.
3. **Contact**: Your name, email (placeholder), and GitHub profile link.

Let me know if you need further tweaks! 😊
