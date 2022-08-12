## Algae Harvesting Optimization Description
#### project description
SVDC R&D department has a major pain point that at what level of cell density, what frequency, as well as harvest amount would result in the maximum yield. This project uses various optimization and visualization methods to deliver the optimum harvesting scheme. 

#### Use Case Pain Points (pp):
1. SVDC only has un-cleaned data recorded by sensors, which cannot be transferred into usable information.
2. Three factors during the harvesting process (density level at harvesting, volume extracted for each harvest, and time interval between each harvest) require optimization to reach theoretically highest possible yield.

#### Solution:
Solution for pp1: Data preprocessing and winsorization are performed to detect and eliminate outliers in original dataset. Only data without external interference are kept for further modelling.

Solution for pp2: Growth versus Density plot is obtained from daily record of density. This relationship simulates a piecewise function between density and time, leading to a Monte Carlo optimization of the harvesting procedure. The best combination of harvesting conditions (density level at harvesting, volume extracted for each harvest, and time interval between each harvest) are obtained from a 3d heatmap.
