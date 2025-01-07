# Hoop-Metrics

## Overview
This project is a  NBA data analytics that uses Python to scrape and analyze NBA statistics data from [NBA.com/stats](https://www.nba.com/stats/). The project focuses on understanding trends in player performance and team strategies over the last 12 years (2012-2024) and how has the game changed over the years.

Part 1 involves scraping NBA statistics data from the official API, while Part 2 focuses on cleaning, analyzing, and visualizing this data to uncover interesting insights about the game of basketball.

---

## Features
### Part 1: Data Scraping
- Utilizes **Python requests** to scrape data from the NBA stats API.
- Processes regular season and playoff data for all players over 10 seasons.
- Stores the scraped data in a **pandas DataFrame** and exports it as an Excel file (`NBA_PlayerData.xlsx`).
- Implements lag times and randomization to prevent API blocks while scraping.

### Part 2: Data Analysis and Visualization
- **Data Cleaning:**
  - Removes unnecessary columns (e.g., "Rank" and "Efficiency").
  - Standardizes team names and creates a "Season Start" column.
  - Differentiates between regular season (RS) and playoff (PO) data.
- **Analysis Highlights:**
  1. Player stat correlations, such as the relationships between three-point shooting and rebounding.
  2. Distribution of player minutes during regular seasons and playoffs.
  3. Changes in gameplay trends over the last 10 years, including the rise of three-point shooting and pace of play.
- **Visualization:**
  - Heatmaps of stat correlations using **plotly**.
  - Histograms and line charts for exploring distributions and trends.
  - Side-by-side comparisons of regular season and playoff stats.

---

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/nba-stats-analysis.git
   cd nba-stats-analysis
   ```
2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Download and save the scraped data (optional):
   - Use the `NBA_PlayerData.xlsx` file provided or run Part 1 to generate the data.

---

## Usage
### Part 1: Scraping Data
To scrape NBA data:
```bash
python scrape_data.py
```
The scraped data will be saved as `NBA_PlayerData.xlsx` in the project directory.

### Part 2: Analyzing Data
To analyze and visualize the data:
```bash
python analyze_data.py
```
This will generate:
- Correlation heatmaps.
- Visualizations comparing stats between seasons and playoffs.
- Insights into gameplay changes over the last decade.

---

## Examples
### Stat Correlation Heatmap
![Heatmap Example](heatmap_example.png)

### Minutes Played Distribution
![Minutes Distribution](minutes_distribution.png)

---

## Key Insights
1. **Stat Trends:** The NBA has seen a significant rise in three-point attempts and makes, indicating a strategic shift toward perimeter shooting.
2. **Playoff Differences:** The playoffs feature tighter player rotations and increased physicality, as evidenced by higher foul rates.
3. **Efficiency Improvements:** Despite faster gameplay, true shooting efficiency has steadily improved over the years.

---


## Contact
For questions or suggestions, feel free to reach out:
- **Name:** Haider
- **GitHub:** [haiderali077](https://github.com/haiderali077)

---

## Acknowledgments
Special thanks to [NBA.com](https://www.nba.com/stats/) for providing access to their stats data.
