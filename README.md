# SkillCraft1

By Xin (Alex) Guo, Jan 2018

## Overview

In computer game StarCraft, there is a certain relationship between the League that a gamer can get into and his/her screen movements when playing the game. This project is trying to find the best model and features to predict the gamer's League based on his/her screen movements.

## Dataset

The dataset used in this project is the [SkillCraft1 Master Table Dataset](http://archive.ics.uci.edu/ml/datasets/SkillCraft1+Master+Table+Dataset) from [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/datasets.html). It aggregated screen movements into screen-fixations using a Salvucci & Goldberg (2000) dispersion-threshold algorithm, and defined Perception Action Cycles (PACs) as fixations with at least one action. 

There are 3395 observations and 20 variables. As below,

1. GameID: Unique ID number for each game (integer) 
2. LeagueIndex: Bronze, Silver, Gold, Platinum, Diamond, Master, GrandMaster, and Professional leagues coded 1-8 (Ordinal) 
3. Age: Age of each player (integer) 
4. HoursPerWeek: Reported hours spent playing per week (integer) 
5. TotalHours: Reported total hours spent playing (integer) 
6. APM: Action per minute (continuous) 
7. SelectByHotkeys: Number of unit or building selections made using hotkeys per timestamp (continuous) 
8. AssignToHotkeys: Number of units or buildings assigned to hotkeys per timestamp (continuous) 
9. UniqueHotkeys: Number of unique hotkeys used per timestamp (continuous) 
10. MinimapAttacks: Number of attack actions on minimap per timestamp (continuous) 
11. MinimapRightClicks: number of right-clicks on minimap per timestamp (continuous) 
12. NumberOfPACs: Number of PACs per timestamp (continuous) 
13. GapBetweenPACs: Mean duration in milliseconds between PACs (continuous) 
14. ActionLatency: Mean latency from the onset of a PACs to their first action in milliseconds (continuous) 
15. ActionsInPAC: Mean number of actions within each PAC (continuous) 
16. TotalMapExplored: The number of 24x24 game coordinate grids viewed by the player per timestamp (continuous) 
17. WorkersMade: Number of SCVs, drones, and probes trained per timestamp (continuous) 
18. UniqueUnitsMade: Unique unites made per timestamp (continuous) 
19. ComplexUnitsMade: Number of ghosts, infestors, and high templars trained per timestamp (continuous) 
20. ComplexAbilitiesUsed: Abilities requiring specific targeting instructions used per timestamp (continuous)

where `LeagueIndex` is the label and other variables are features.

## Usage

Open the Jupyter Notebook [analysis.ipynb](https://github.com/alexguoxin/SkillCraft1/blob/master/src/analysis.ipynb) in the `src` directory for the analysis. Just hit `Cell` and then `Run All` to run the whole notebook.

Report is the [Report.md](https://github.com/alexguoxin/SkillCraft1/blob/master/doc/Report.md) in the `doc` directory.

## Dependencies

- Python
- Jupyter Notebook
- Python Packages:
	- `numpy`
	- `pandas`
	- `matplotlib`
	- `sklearn`