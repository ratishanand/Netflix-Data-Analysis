# Netflix-Data-Analysis -BY Ratish Anand

# 🎬 Netflix Data Analysis

<div align="center">
  
![Netflix](https://img.shields.io/badge/Netflix-E50914?style=for-the-badge&logo=netflix&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

*An exploratory data analysis project uncovering insights from Netflix's content library*

[View Demo](#-visualizations) · [Report Bug](https://github.com/ratishanand/Netflix-Data-Analysis/issues) · [Request Feature](https://github.com/ratishanand/Netflix-Data-Analysis/issues)

</div>

---

## 📋 Table of Contents

- [About The Project](#-about-the-project)
- [Dataset](#-dataset)
- [File Structure](#-file-structure)
- [Technologies Used](#-technologies-used)
- [Installation](#-installation)
- [Key Findings](#-key-findings)
- [Visualizations](#-visualizations)
- [Analysis Performed](#-analysis-performed)
- [Future Enhancements](#-future-enhancements)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🎯 About The Project

This project performs comprehensive exploratory data analysis (EDA) on Netflix's movies and TV shows dataset. The analysis aims to uncover patterns, trends, and insights about Netflix's content strategy, including content distribution, genre preferences, rating patterns, and geographical content production.

### Key Objectives:
- 📊 Analyze content distribution between Movies and TV Shows
- 🌍 Identify top content-producing countries
- 📅 Examine content release trends over the years
- 🎭 Explore genre and rating distributions
- 👥 Analyze cast and director patterns

---

## 📊 Dataset

The dataset contains information about Netflix's content library with the following features:

| Feature | Description |
|---------|-------------|
| `show_id` | Unique identifier for each show |
| `type` | Content type (Movie/TV Show) |
| `title` | Name of the content |
| `director` | Director(s) of the content |
| `cast` | Main cast members |
| `country` | Country of production |
| `date_added` | Date added to Netflix |
| `release_year` | Original release year |
| `rating` | Content rating (TV-MA, PG-13, etc.) |
| `duration` | Duration (minutes for movies, seasons for TV shows) |
| `listed_in` | Genres/Categories |
| `description` | Brief synopsis |

**Dataset Source:** [Kaggle - Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)

**Total Records:** ~8,800+ entries

---

## 📁 File Structure

```
Netflix-Data-Analysis/
│
├── data/
│   ├── netflix_titles.csv              # Raw dataset
│   └── cleaned_netflix_data.csv        # Processed dataset
│
├── notebooks/
│   └── Netflix Data Analysis.ipynb     # Main analysis notebook
│
├── images/
│   ├── content_distribution.png        # Movies vs TV Shows pie chart
│   ├── top_countries.png               # Top content producing countries
│   ├── yearly_trend.png                # Content addition trends over years
│   ├── rating_distribution.png         # Rating category distribution
│   ├── genre_analysis.png              # Popular genres visualization
│   └── duration_analysis.png           # Content duration analysis
│
├── src/
│   ├── data_cleaning.py                # Data preprocessing scripts
│   ├── visualization.py                # Plotting functions
│   └── analysis.py                     # Statistical analysis functions
│
├── requirements.txt                     # Project dependencies
├── README.md                           # Project documentation
└── LICENSE                             # License information
```

---

## 🛠 Technologies Used

### Programming Languages
- **Python 3.8+** - Core programming language

### Libraries & Frameworks
```python
pandas           # Data manipulation and analysis
numpy            # Numerical computations
matplotlib       # Static visualizations
seaborn          # Statistical data visualization
plotly           # Interactive visualizations
wordcloud        # Text visualization
```

### Development Tools
- **Jupyter Notebook** - Interactive development environment
- **Git** - Version control
- **GitHub** - Code hosting and collaboration

---

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Git

### Setup Instructions

1. **Clone the repository**
```bash
git clone https://github.com/ratishanand/Netflix-Data-Analysis.git
cd Netflix-Data-Analysis
```

2. **Create virtual environment** (recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

5. **Open the analysis notebook**
   - Navigate to `notebooks/Netflix Data Analysis.ipynb`
   - Run all cells to reproduce the analysis

---

## 🔍 Key Findings

### 1. Content Type Distribution
- **Movies dominate** Netflix's library with approximately 69% of total content
- **TV Shows** comprise about 31% of the catalog
- Netflix has been gradually increasing TV show content in recent years

### 2. Geographical Insights
- **United States** leads in content production (~40% of total content)
- **India** is the second-largest content contributor
- **Top 5 Countries:** USA, India, UK, Canada, France

### 3. Content Rating Patterns
- **TV-MA** (Mature Audience) is the most common rating
- **TV-14** and **TV-PG** follow as popular rating categories
- Majority of content targets adult audiences

### 4. Temporal Trends
- Significant increase in content additions from **2015 onwards**
- Peak content addition year: **2019**
- Slight decline in 2020 (possibly due to COVID-19 pandemic)

### 5. Genre Analysis
- **International Movies** is the most prominent category
- **Dramas** and **Comedies** are highly popular genres
- Growing trend in **Documentaries** and **Stand-up Comedy**

---

## 📈 Visualizations

### 1. Content Type Distribution
![Content Distribution](images/content_distribution.png)
*Pie chart showing the split between Movies and TV Shows on Netflix*

### 2. Top Content Producing Countries
![Top Countries](images/top_countries.png)
*Bar chart displaying the top 10 countries by content volume*

### 3. Content Addition Trends
![Yearly Trends](images/yearly_trend.png)
*Line graph showing Netflix content growth from 2008 to 2021*

### 4. Rating Distribution
![Rating Distribution](images/rating_distribution.png)
*Distribution of content across different rating categories*

### 5. Popular Genres
![Genre Analysis](images/genre_analysis.png)
*Top 15 most popular genres on Netflix*

### 6. Duration Analysis
![Duration Analysis](images/duration_analysis.png)
*Movie duration distribution and TV show season count patterns*

---

## 🔬 Analysis Performed

### 1. **Data Cleaning & Preprocessing**
   - Handled missing values in director, cast, and country columns
   - Converted date_added to datetime format for temporal analysis
   - Extracted year and month from date_added for trend analysis
   - Split multi-value columns (cast, director, listed_in) for detailed analysis

### 2. **Exploratory Data Analysis**
   - **Univariate Analysis:** Individual feature distributions
   - **Bivariate Analysis:** Relationships between features
   - **Temporal Analysis:** Content addition patterns over time
   - **Categorical Analysis:** Genre, rating, and type distributions

### 3. **Statistical Analysis**
   - Content growth rate calculations
   - Genre popularity scoring
   - Country-wise content contribution percentage
   - Rating distribution across content types

### 4. **Text Analysis**
   - Word clouds from descriptions and genres
   - Most frequent cast members and directors
   - Popular keywords in content descriptions

---

## 🔮 Future Enhancements

- [ ] **Sentiment Analysis** on content descriptions
- [ ] **Recommendation System** based on genre and ratings
- [ ] **Predictive Modeling** for content success
- [ ] **Interactive Dashboard** using Streamlit or Dash
- [ ] **Time Series Forecasting** for future content trends
- [ ] **Network Analysis** of cast and director collaborations
- [ ] **Comparison Analysis** with other streaming platforms

---

## 🤝 Contributing

Contributions make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📧 Contact

**Ratish Anand**

- GitHub: [@ratishanand](https://github.com/ratishanand)
- LinkedIn: [Your LinkedIn Profile](#)
- Email: your.email@example.com

**Project Link:** [https://github.com/ratishanand/Netflix-Data-Analysis](https://github.com/ratishanand/Netflix-Data-Analysis)

---

## 🙏 Acknowledgments

- [Netflix](https://www.netflix.com/) for inspiring this analysis
- [Kaggle](https://www.kaggle.com/) for providing the dataset
- [Python Data Science Community](https://www.python.org/) for excellent libraries
- All contributors who help improve this project

---

<div align="center">

**⭐ Star this repository if you found it helpful!**

Made with ❤️ by [Ratish Anand](https://github.com/ratishanand)

</div>
