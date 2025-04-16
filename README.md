# Visualizing the Evolution of Formula One Performance Metrics (1950-2024)

By [Aritra Saharay](https://ari-s-123.github.io/Personal-Site)

Formula One (F1) stands as the pinnacle of motorsport, epitomizing the fusion of
cutting-edge automotive technology, driver prowess, and strategic team
management. Since its inception in 1950, the sport has undergone profound
transformations influenced by technological advancements, regulatory changes,
and evolving competitive dynamics. In recent years, significant developments
such as the introduction of hybrid power units in 2014, the implementation of
budget caps in 2021 to level the competitive field, and adaptations due to
global events like the COVID-19 pandemic have further reshaped the landscape of
F1.

The primary objective of this project is to analyze and visualize the evolution
of key performance metrics in Formula One (F1) over the period from 1950
to 2024. By examining metrics such as mean career win rates for drivers and
points per race for constructors, the project aims to uncover trends, assess the
impact of regulatory changes, and highlight significant shifts in team and
driver performances. These visualizations will provide valuable insights for
fans, analysts, and teams to understand the dynamics that have shaped the sport
over the decades

## Specific Aims

- Trend Analysis: Examine how drivers' and constructors' performance metrics
  have evolved over different eras of F1.
- Impact Assessment: Determine the influence of major regulatory changes and
  technological advancements on performance outcomes.
- Comparative Insights: Identify teams and drivers that have shown significant
  improvements or declines in performance.
- Interactive Exploration: Develop interactive visualizations that allow users
  to explore the data in-depth through various analytical lenses.

## Main Insights

- Mercedes has the best (lowest) mean finishing position in a given season of
  all time of 3.17 in 2017.
- Zakspeed has the worst (highest) mean finishing position in a given season of
  all time of 35.03 in 1989. Funnily enough, 1989 was also the last year they
  participated in F1...
- Out of the drivers with at least 20 race starts, Juan Manuel Fangio appears to
  be the driver with the best mean career finishing position of all time with an
  average finishing place of 4.79. However, it must be noted that the next best
  driver according to this metric is Lewis Hamilton at 5.02, a driver with a far
  greater total number of race starts at 356 compared to Fangio's 58.
- Out of the drivers with at least 20 race starts, Bernd Schneider appears to be
  the driver with the worst mean career finishing position of all time with an
  average finishing place of 28.5. Interestingly, he drove for Zakspeed in 1989,
  the same team that we previously identified as having the worst mean finishing
  position for a constructor in a single year...

## Data sources and abstraction

**Dataset Type:** The project utilizes static multivariate tabular datasets in
CSV format encompassing historical Formula One data from 1950 to 2024. These
datasets include comprehensive information on drivers, constructors, race
results, etc. This is an author-maintained dataset with a universal public
domain license from Kaggle, sourced from the Ergast F1 API updated for full 2024
results. I downloaded a snapshot of this data in April 2025. The results from sprint races and
Indianapolis 500 have not been considered.

**Data Description for Key Tables:**

- Drivers Table:

  - Variables: driverId, driverRef, number, code, forename, surname, dob,
    nationality, url

- Constructors Table:
- Variables: constructorId, constructorRef, name, nationality, url

- Results Table:
- Variables: resultId, raceId, driverId, constructorId, number, grid, position,
  positionText, positionOrder, points

- Races Table:
- Variables: raceId, year, round, circuitId, name, date, time, url, fp1_date,
  fp1_time

**References:**

- Primary Dataset:
  [Formula 1 World Championship - Kaggle](https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020)
- Regulatory Changes: Compiled from official FIA publications and reputable news
  sources.
