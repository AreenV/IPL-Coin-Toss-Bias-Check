# Does Winning the Toss Win the Match? (IPL 2008–2024)

An exploratory data analysis project checking whether winning the coin toss actually gives a team an advantage in the Indian Premier League.

## About the Project
Commentators and captains often treat the toss as a huge factor in T20 cricket, with teams overwhelmingly choosing to field first. This notebook analyzes 17 seasons of IPL match data (2008–2024) to test if winning the toss leads to more match wins, and whether that changes based on batting vs. fielding first, venues, or match stages (league vs. playoffs).

## Dataset
- **Source:** [IPL Complete Dataset (2008–2024) on Kaggle](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020/data?select=matches.csv) (`matches.csv`)
- **Size:** 1,095 total matches across 17 seasons (1,090 completed matches used after dropping 5 no-result games)

## Key Results
- **No overall toss advantage:** Toss-winning teams won **50.83%** of all completed matches (95% CI: 47.86%–53.79%), which is essentially a 50/50 coin flip.
- **Chasing advantage faded in recent seasons:** From 2008 to 2018, teams choosing to field first won **55.47%** of the time, suggesting a chasing edge. However, from 2019 to 2024, that rate dropped to **51.56%**, back in line with random chance.
- **Batting first:** Teams choosing to bat first won **45.74%** (2008–2018) and **44.44%** (2019–2024) of their matches.
- **Match stage:** League matches matched the overall baseline at **51.00%**, while playoff/knockout matches had too few games (42 matches) to draw a solid conclusion.

## Tools Used
- Python
- Pandas & NumPy
- Matplotlib / Seaborn
- Jupyter Notebook

## How to Run
1. Clone this repository and download `matches.csv` into a `data/` folder.
2. Install the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
