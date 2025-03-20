Here’s a professional and technical GitHub README for your cricket World Cup centuries data visualization project:

---

# 🏏 Cricket World Cup Centuries Analysis using Python

## 📊 Project Overview
This project analyzes **Cricket World Cup Centuries** data using Python and popular data manipulation and visualization libraries like:

- **NumPy** 🧮  
- **Pandas** 📚  
- **Matplotlib** 📊  
- **Seaborn** 🎨  

The dataset contains columns such as:  
`No. | Player | Runs | Balls | 4s | 6s | S/R | Team | Opposition | Venue | Date | Result`

### 🚀 Objective
The goal of this project was to gain insights from the dataset by performing various operations and creating meaningful visualizations. This project was part of my **Winter '24 Training Program** at college, where I explored multiple visualization techniques to analyze and interpret cricket match data effectively.

---

## 📂 Dataset
> **CSV Link:** <a href="https://drive.google.com/file/d/1-DanDyAOQyW0-Ntv15YsrkRBFd8LADzE/view?usp=drive_link">Link to Dataset</a>  
The dataset consists of information about centuries scored in Cricket World Cup matches, including details about runs, balls faced, boundaries hit, and match results.

---

## ⚡️ Key Operations & Visualizations
### 1. 🎯 Basic Operations
- Printing unique values from columns.
- Counting unique teams and plotting a bar chart.
- Filtering data by batsmen’s S/R (Strike Rate) greater than 150.
- Dropping records while filtering simultaneously.

### 2. 📊 Statistical Analysis
- Sorting top 5 highest runs scored.
- Matches played by **Rohit Sharma** and venues where he scored centuries.
- Analyzing team losses and plotting win/loss/tie distributions.
- Runs scored over 170, boundaries (4s & 6s) analysis.

### 3. 📈 Data Visualization
- **Scatter Plot:** Runs vs Balls  
- **Bar Plot:** Count of unique teams  
- **Histogram:** Balls faced and S/R greater than 120  
- **Box Plot:** Distribution of runs and S/R  
- **KDE Plot:** Distribution of runs and boundaries  
- **Violin Plot:** Comparative analysis of strike rates and runs  
- **Pair Plot:** Visualizing relationships between multiple features  

### 4. 🏆 Advanced Filtering
- Displaying only winners and analyzing their S/R greater than 100.
- Removing winners with runs above 100.
- Analyzing S/R above 100 for all winners and plotting against the respective players.

---

## 📌 Code Highlights
### 👉 Top 5 Highest Runs Scored
```python
top_5_runs = df.sort_values(by='Runs', ascending=False).head(5)
print(top_5_runs[['Player', 'Runs', 'Team', 'Opposition']])
```

### 👉 Bar Plot of Unique Teams
```python
team_counts = df['Team'].value_counts()
plt.figure(figsize=(10, 6))
sns.barplot(x=team_counts.index, y=team_counts.values, palette='viridis')
plt.title('Count of Centuries by Team')
plt.xticks(rotation=45)
plt.show()
```

### 👉 Filtering by S/R Greater Than 150
```python
high_sr = df[df['S/R'] > 150]
print(high_sr[['Player', 'Runs', 'S/R']])
```

---

## 📝 Results & Insights
- Teams with the most centuries scored.
- Players with exceptional S/R in high-scoring matches.
- Distribution of runs and boundaries across different venues.
- Performance analysis of key players like **Rohit Sharma** in various matches.

---

## 🛠️ Technologies & Tools
- Python 3.x
- Jupyter Notebook / Google Colab
- NumPy, Pandas, Matplotlib, Seaborn

---

## 📚 How to Run the Project
1. Clone the repository:
```bash
git clone https://github.com/your-username/cricket-worldcup-analysis.git
```
2. Navigate to the project directory:
```bash
cd cricket-worldcup-analysis
```
3. Install required libraries:
```bash
pip install -r requirements.txt
```
4. Run the notebook:
```bash
jupyter notebook
```

---

## 📊 Sample Visualizations
### 🎥 Runs vs Balls Scatter Plot
![image](https://github.com/user-attachments/assets/4f7a9bd5-1c9c-4efe-aec9-edd0690fbb58)


### 📊 Win/Loss/Tie Plot
![image](https://github.com/user-attachments/assets/4d4132ad-4a90-447a-9f8b-650f57bec4c7)


---

## 🎁 Future Improvements
- Adding interactive visualizations using Plotly.
- Implementing predictive models for player performance analysis.
- Exploring more advanced statistical techniques for deeper insights.

---

## 🤝 Acknowledgements
This project was part of my **Winter '24 Training Program** at my college, where I explored and applied various data analysis techniques on real-world sports datasets.

---

## 📧 Contact Me
email: safalyaroy9463@gmail.com
Feel free to reach out if you have any questions or suggestions!

---

✨ _If you found this project helpful, give it a ⭐ and contribute to future improvements!_ 🚀
