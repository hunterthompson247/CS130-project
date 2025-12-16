# Methodology

## Data Source(s)
- The dataset was found in FiveThirtyEight's github repository that contains data from previous articles and graphics that they have done.
- The file used was `historical_projections.csv`, which contains projected outcomes for NBA draft prospects. The file contains many different different draft classes, however I decided to focus on 2015.

## Data Preparation/Cleaning
- The original CSV file contained improperly broken rows that split player names across multiple lines. This was first thing I had to clean up
- Rows were reconstructed by joining lines until each row contained nine fields. This made it easier to read the data.
- All data was filtered to include only players from the 2015 NBA Draft. I originally wanted to include multiple drafts, but the amount of data would have been overwhelming.
- Numeric columns, including Projected SPM, Superstar, Starter, Role Player, and Bust probabilities, were converted from strings to floating-point values.

## Assumptions
- Probabilities for Superstar, Starter, Role Player, and Bust outcomes were assumed to be mutually exclusive and collectively exhaustive.
- Projected SPM was treated as a comparable metric across all positions.
- The projections were assumed to represent expectations prior to the players’ NBA careers.

## Limitations
- The dataset does not include actual career outcomes, only projections.
- The methodology used to generate the projections is not fully documented. You have to take a lot of what you see at face value.
- Player development, injuries, and team context are not accounted for in the data.