# ML Final Project with PUBG Data

## Feature Elimination

We have chosen to eliminate the following features for a variety of reasons...

1. `maxPlace`, `numGroups`, `killPlace` - These are relevant to the data and not important for actual gameplay
2. `matchId`, `groupId` - There is too much data here to run efficiently timed comparisons per groups and we do not want the features to be weighted by these due to such little variation
3. `rankPoints`, `winPoints`, `teamKills`, `killPoints` - The description for these features is ambiguous, and also is reliant on the tifferent team types
4. `vehiclesDestroyed`, `roadKills` - These ones are so sparse that if the algorithm detects someone with one of these who also has a high win percentage, it may skew the data
