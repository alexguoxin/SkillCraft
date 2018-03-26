# SkillCraft

DSCI 573 Lab 2 Exercise 4 Mini-project

By Xin (Alex) Guo, Jan 2018

## Overview

In computer game StarCraft, there is a certain relationship between the League that a gamer can get into and his/her screen movements when playing the game. This project is trying to find the best model and features to predict the gamer's League based on his/her screen movements.

## Dataset

The dataset used in this project is the [SkillCraft1 Master Table Dataset](http://archive.ics.uci.edu/ml/datasets/SkillCraft1+Master+Table+Dataset) from [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml/datasets.html). It aggregated screen movements into screen-fixations using a Salvucci & Goldberg (2000) dispersion-threshold algorithm, and defined Perception Action Cycles (PACs) as fixations with at least one action. 

There are 3395 observations and 20 variables, where `LeagueIndex` is the label and other variables are features.

## Usage

Open the Jupyter Notebook [analysis.ipynb](https://github.com/alexguoxin/SkillCraft/blob/master/src/analysis.ipynb) in the `src` directory for the analysis. Just hit `Cell` and then `Run All` to run the whole notebook.

Report is the [Report.md](https://github.com/alexguoxin/SkillCraft/blob/master/doc/Report.md) in the `doc` directory.

## Dependencies

- Python
- Jupyter Notebook
- Python Packages:
	- `numpy`
	- `pandas`
	- `matplotlib`
	- `sklearn`