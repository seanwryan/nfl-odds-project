Overall Summary
---------------

-   **Data Preparation:** Combined and cleaned three seasons (2022--24) of NFL odds into one consistent table, extracting numeric scores, spreads, and over/under lines.

-   **Feature Engineering:** Created flags for wins, covers, and overs, plus computed point differentials and spread deviations.

-   **Team‐Level Insights:** Calculated each team's win%, cover%, and over% per season and visualized the top and bottom five cover teams against a 50% baseline.

-   **Probability Model:** Trained a logistic regression on point spreads to produce implied cover probabilities (`Implied_P`) for 2024 games.

-   **Calibration Check:** Verified average model prediction (48.5%) vs. actual cover rate (53.3%) to confirm slight underestimation of cover likelihood.

-   **Value‐Bet Analysis:**

    -   **Edge Calculation:** Identified games where empirical cover rates exceeded implied probabilities by more than 5%.

    -   **P/L Simulation:** Simulated $1 flat bets on those value games; wins outpaced losses roughly 2:1.

    -   **Team Performance:** Chargers and Broncos delivered the highest profits, followed by Lions, Ravens, and Bengals.

Sources
-------

-   **SportsBettingHistory.com** --- historical NFL spreads & odds data.
-   **chatgpt.com** --- structuring python notebook.
