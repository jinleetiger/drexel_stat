# Soccer Data Analysis and Visualization

This project analyzes soccer data using the API-Football API to create insightful visualizations about team performance, player statistics, and match outcomes.

## Setup

1. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. API Key Setup:
- Sign up for an API key at [API-Football](https://www.api-football.com/)
- Replace `YOUR_API_KEY` in the notebook with your actual API key

## Usage

1. Start Jupyter Notebook:
```bash
jupyter notebook
```

2. Open `Soccer_Data_Visualization.ipynb`

3. Run the cells in sequence to:
- Fetch soccer data from API-Football
- Generate visualizations for team performance
- Analyze player and team statistics

## Visualizations Include:

- Points distribution across teams
- Goals scored vs. goals conceded
- Win-Draw-Loss distribution
- Team performance analysis
- And more...

## Note
Make sure you have a valid API key from API-Football to fetch the data. The free tier has limited requests per day.
