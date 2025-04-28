# Movies-Insights
Analyzed 20,000 movie and tv show titles to uncover insights and optimize recommendations using SQL and Python.

## Project Overview
- **Goal**: Identify high-quality content to recommend based on sentiment (High: ≥7, Neutral: 5.5–6.9, Low: <5.5).
- **Data**: ~19,000–20,000 cleaned records (`data_cleaned.csv`) with `title`, `type`, `genres`, `releaseYear`, `imdbAverageRating`, `imdbNumVotes`.

## Tools & Techniques
- **SQL**: SQLite queries (CTEs, window functions) for sentiment and genre analysis.
- **Python**: Pandas for EDA, Seaborn/Matplotlib for visualizations (pie, bar, heatmap).
- **Deliverables**: Jupyter Notebook , PDF, visuals.

## Key Findings
- **Sentiment**:
  - Movies: ~60% High, 25% Neutral, 15% Low.
  - TV Shows: ~50% High, 30% Neutral, 20% Low.
- **Top Genres**: Drama|History, Biography|Drama (~80–85% High ratings).
- **Trends**: Movies (~75%) dominate, led by Drama (20%). High-rated titles with high `imdbNumVotes` (>100K) are more popular.

## Recommendations
1. Prioritize Drama/Biography movies (~80% High ratings).
2. Expand Comedy|Drama TV shows.
3. Target Comedy/Action fans with user data.
4. Weight recommendations by `imdbNumVotes` to favor popular, High-rated titles (e.g., Drama movies with >100K votes).
