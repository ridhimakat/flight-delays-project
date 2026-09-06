# U.S. Flight Delays — Exploratory Data Analysis

Analysis of one month of U.S. domestic flight data (June 2026) from the Bureau of Transportation Statistics, looking at what drives departure delays and where a traveler or airline could focus to reduce them.

## Data
U.S. DOT Bureau of Transportation Statistics — [Reporting Carrier On-Time Performance](https://www.transtats.bts.gov/) (Table 236), June 2026. ~500K domestic flights. BTS counts a flight as on-time if it departs or arrives fewer than 15 minutes after schedule.

## Tools
Python · pandas · NumPy · matplotlib · seaborn

## What's in the notebook
- Loading and inspecting the raw BTS extract
- Data cleaning — handling cancellations, nulls, HHMM time parsing, and carrier code mapping
- Feature engineering — airline names, time-of-day buckets, delay flags
- Exploratory analysis across airlines, time of day, routes, and delay causes
- Findings and recommendations

## Key findings
- Delays are heavily right-skewed — the median delay is about 1 minute, but a long tail pulls the mean higher.
- On-time performance varies widely by airline, from Alaska (8.5 min avg) to American (~27 min).
- Delays build through the day — morning flights average 7.3 min of delay, evening flights 29.1.
- Late aircraft and carrier issues are the top causes, far ahead of weather. Most delay is operational, not weather-related.
