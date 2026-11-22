# Cricket Player Performance Dashboard | Power BI

An interactive Power BI report that shows career statistics for individual cricketers across three disciplines: **Batting**, **Bowling**, and **Fielding**. Pick a player from the dropdown and the page updates with that player's key numbers, so you can review and compare performance quickly without searching through raw tables.

## Dashboard Preview

**Batting**
![Batting dashboard](images/batting_dashboard.png)

**Bowling**
![Bowling dashboard](images/bowling_dashboard.png)

**Fielding**
![Fielding dashboard](images/fielding_dashboard.png)

## Business Questions Answered

- How many runs, boundaries, and centuries has a batter scored, and how fast does he score (strike rate)?
- How effective is a bowler: wickets, average, economy rate, and best bowling figures?
- How much does a player contribute in the field: catches, stumpings, and dismissals per innings?
- What is a player's career span and how many matches and innings does it cover?

## Dataset

Three tables of player career statistics, with each column described in `Column_definitions.xlsx`.

| Table | Rows represent | Key columns |
|---|---|---|
| **Batting** | One batter's career | Player, Span, Mat, Inns, NO, Runs, HS, Ave, BF, SR, 100, 50, 0, 4s, 6s |
| **Bowling** | One bowler's career | Player, Span, Mat, Inns, Overs, Mdns, Runs, Wkts, BBI, Ave, Econ, SR, 4, 5 |
| **Fielding** | One fielder's career | Player, Span, Mat, Inns, Dis, Ct, St, Ct Wk, Ct Fi, MD, D/I |

## Data Collection

The data was collected by **web scraping** the player statistics pages of [ESPNcricinfo Statsguru](https://stats.espncricinfo.com/) for batting, bowling, and fielding. The scraped tables were then organized into three datasets and loaded into Power BI.

All statistics belong to ESPNcricinfo. This project is for learning and portfolio purposes only and is not used commercially.

## Report Pages and Metrics

### Batting
Span, Matches, Innings, Not Outs, Runs, Highest Score, Balls Faced, Batting Average, Strike Rate, Fours, Sixes, Half Centuries, Centuries, Zeros.

### Bowling
Span, Matches, Innings, Overs, Maiden Overs, Runs Conceded, Wickets, Best Bowling Innings, Bowling Average, Economy Rate, Strike Rate, Four-Wicket Hauls, Five-Wicket Hauls.

### Fielding
Span, Matches, Innings, Catches, Stumpings, Catches as Wicketkeeper, Catches as Fielder, Match Days, Dismissals Involved In, Dismissals per Innings.

## Key Metric Definitions

| Metric | Meaning |
|---|---|
| Batting Average | Runs scored per dismissal (Runs / Outs) |
| Batting Strike Rate | Runs scored per 100 balls faced |
| Bowling Average | Runs conceded per wicket taken |
| Economy Rate | Runs conceded per over bowled |
| Bowling Strike Rate | Balls bowled per wicket taken |
| Dismissals per Innings | Catches and stumpings divided by innings |

## Features

- **Player slicer** on every page to switch players instantly
- **KPI cards** that put the most important numbers up front
- **Separate pages** for batting, bowling, and fielding, each with its own layout
- **Custom design**: consistent color theme and cricket illustrations as page backgrounds

## Tools Used

- Web scraping (data collection)
- Power BI Desktop
- Microsoft Excel (column definitions)

## Repository Structure

```
.
├── cricket_data.pbix          # Power BI report (open in Power BI Desktop)
├── Column_definitions.xlsx    # Description of every column in the dataset
├── ESPN.pdf                   # PDF export of the report
├── images/
│   ├── batting_dashboard.png
│   ├── bowling_dashboard.png
│   ├── fielding_dashboard.png
│   ├── Batting.png            # Page background
│   ├── Bowling.png            # Page background
│   └── Fielding.png           # Page background
└── README.md
```

## How to Use

1. Download or clone this repository.
2. Open `cricket_data.pbix` in Power BI Desktop.
3. Choose a player in the **Player** slicer at the top right of each page.
4. Read the KPI cards. Use `Column_definitions.xlsx` if you are unsure what a metric means.

## Possible Next Steps

- Add comparison visuals to put two players side by side
- Add trend charts of runs or wickets by year
- Add ranking tables, for example top run scorers or best economy rates
- Add a format or team slicer if the data is extended

## Author

**Samarth Degaonkar**
Power BI Data Analyst | SQL | Python
[LinkedIn](https://linkedin.com/in/samarth-degaonkar-a76471168) | degaonkar.sam98@gmail.com
