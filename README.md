# Sports Data Analysis and Visualization

A comprehensive data analysis project covering three major sports: Baseball, Basketball, and Soccer. This repository contains detailed statistical analyses, visualizations, and insights for historical data and player performance metrics.

## Project Overview

### 1. Basketball Analysis (`Basketball_data_analysis.ipynb`)
- **Historical NBA Trends (1990-2023)**
  - League-wide statistical evolution
  - Pace of play changes
  - Scoring patterns and efficiency metrics
  - Three-point revolution analysis

- **Michael Jordan Era Analysis**
  - Career progression and statistical dominance
  - Championship vs non-championship seasons comparison
  - Performance relative to league averages
  - Comparison with contemporary legends (Magic, Bird, etc.)
  - Advanced metrics and efficiency analysis

- **Visualizations Include**
  - Time series of league trends
  - Jordan's performance scatter plots
  - Championship season highlights
  - Comparative radar charts
  - Era-adjusted statistical analyses

### 2. Baseball Historical Analysis (`baseball_historical_analysis.ipynb`)
- **Historical Trends Analysis**
  - Batting average evolution
  - Home run patterns
  - Pitching statistics changes
  - Team performance metrics

- **Player Performance Analysis**
  - Career trajectories
  - Statistical comparisons
  - Era-adjusted metrics
  - Hall of Fame probability analysis

- **Visualizations Include**
  - Historical trend lines
  - Player comparison charts
  - Performance distribution plots
  - Statistical correlation matrices

### 3. Soccer Data Analysis (`Soccer_Data_Visualization.ipynb`)
- **League Performance Analysis**
  - Team rankings and points distribution
  - Goal scoring patterns
  - Win-Draw-Loss distributions
  - Home vs Away performance

- **Team Statistics**
  - Scoring efficiency
  - Defensive metrics
  - Possession analysis
  - Season-by-season comparisons

- **Visualizations Include**
  - League standings charts
  - Goal distribution plots
  - Performance heat maps
  - Team comparison radar charts

## Setup and Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd sports-data-analysis
```

2. Create and activate virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## Dependencies
- Python 3.8+
- pandas >= 1.3.0
- numpy >= 1.20.0
- matplotlib >= 3.4.0
- seaborn >= 0.11.0
- jupyter >= 1.0.0
- nba_api (for NBA data)
- requests >= 2.26.0 (for API calls)

## Usage

1. Start Jupyter Notebook:
```bash
jupyter notebook
```

2. Navigate to the desired analysis notebook:
- `Basketball_data_analysis.ipynb` for NBA analysis
- `baseball_historical_analysis.ipynb` for MLB analysis
- `Soccer_Data_Visualization.ipynb` for soccer analysis

3. Run the cells in sequence to generate analyses and visualizations

## Key Features

### Basketball Analysis
- Comprehensive NBA historical trends (1990-2023)
- Michael Jordan's career analysis and comparisons
- League evolution metrics and visualizations
- Player efficiency and performance analytics

### Baseball Analysis
- Historical MLB statistics and trends
- Player performance metrics and comparisons
- Team success factors analysis
- Advanced statistical modeling

### Soccer Analysis
- League performance metrics
- Team statistics and comparisons
- Scoring and defensive analysis
- Season-by-season trend analysis

## Data Sources
- NBA: Official NBA API and basketball-reference.com
- MLB: Baseball statistical databases and historical records
- Soccer: Football-Data.org API and league statistics

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
- NBA API for basketball statistics
- Baseball statistical databases
- Football-Data.org for soccer data
- Various sports analytics communities and resources

## Notes
- Some analyses may require API keys for data access
- Historical data availability may vary by sport and era
- Performance metrics are era-adjusted where applicable
