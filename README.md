# 🏈 Clustering NFL QBs, RBs, and Receivers Based on 2024-25 Season Stats

This project uses unsupervised machine learning to cluster NFL quarterbacks, running backs, and wide receivers/tight ends based on their statistical performance during the 2024–25 NFL season. By scoping in on each position group separately, I seek to find unique player types and trends that go beyond raw box score stats.

## 📌 Project Goals

- **Identify player types** within each position group using statistical clustering  
- **Explore play styles** using PCA and visualizations  
- **Quantify performance** using modern metrics (e.g., EPA/play, yards per route run)  
- **Uncover hidden similarities** between players that may not be obvious from traditional stats (see Saquon Barkley and James Cook!)

---

## 📂 Project Structure

├── code-notebooks/ # all of my .ipynb files consisting of data preprocessing & modelling

├── filtered-data/ # data that I have processed in the `NFL-Player-Clustering-Data-Preprocessing.ipynb` file

├── pro-football-reference-data/ # all of the plain basic statistics pulled from [Pro Football Reference](https://www.pro-football-reference.com/)

└── README.md

---

## 📊 Data Sources

- **2024–25 NFL player statistics** pulled from [Pro Football Reference](https://www.pro-football-reference.com/) using their built in export feature
  - [Passing Stats](https://www.pro-football-reference.com/years/2024/passing.htm)
  - [Rushing Stats](https://www.pro-football-reference.com/years/2024/rushing.htm)
  - [Receiving Stats](https://www.pro-football-reference.com/years/2024/receiving.htm)

---

## 🧪 Methodology

### 1. Data Wrangling
- Separate datasets processed for QBs, RBs, and WRs/TEs  
- Position-specific feature engineering

### 2. Feature Scaling & Dimensionality Reduction
- `StandardScaler` applied to all continuous stats  
- PCA used to reduce high-dimensional stat space to 2D/3D for visualization  

### 3. Clustering
- `KMeans` applied to QBs and Receivers, `AgglomerativeCluster` applied to RBs
- Each player assigned a cluster label corresponding to their play style  

### 4. Visualization
- 2D PCA scatter plots with cluster coloring  
- Cluster summaries with median stats and archetype names (e.g., “Deep Threat WR”, “High Risk High Reward QB”)  

---

## 🔍 Results

Revisit with full findings 

---

## 📈 Key Learnings

- Clustering offers a way to explore performance and player characteristics beyond surface stats  
- Play styles often align more with usage and context within the team than pure efficiency  
- Proper feature engineering and data wrangling is the most important part of reduced dimensionality clustering 

---

## 🛠 Technologies Used

- Python (`pandas`, `scikit-learn`, `matplotlib`, `seaborn`, etc.)  
- Jupyter Notebooks  
- PCA, KMeans, Agg Clustering
- Advanced visualizations w/ Plotly

---

## 🚀 Future Work

- Incorporate *defensive matchups* and *game situations* into clustering - This would be consequential for players like Caleb Williams, Kyren Williams 
- Explore *season-over-season* clustering to identify development trajectories - This would be consequential for players like Saquon Barkley, Alvin Kamara
- Build *interactive dashboards* for exploring clusters dynamically - This would be useful for any user who wants to explore my findings

---

## 🙋‍♂️ About Me

Hi! I’m Jake Lukasik, a data science undergrad at Penn State, graduating Fall of 2025 passionate about sports analytics.
Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/-lukasik/) or check out my other projects!

**Other Projects:**
- [NASCAR Race Simulation](https://github.com/jake-lukasik/NASCAR-Race-Predictions)
- [UFC Fight Predictor](https://github.com/jake-lukasik/UFC-Fight-Predictor)
- [NFL O/U Betting Model](https://github.com/jake-lukasik/NFL-OU-Models)
---

## 📎 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
