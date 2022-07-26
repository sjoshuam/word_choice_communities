# word_choice_communities
Using word choices to predict group membership

## DESCRIPTION

This project trains machine learning models to predict group affiliation from
social media word choices.  As a test case, the project uses Tweets from Republican and Democrat members of congress as a test case, and uses tweets from Canadian members of parliament for comparison.

## TASKS

This project is organized into three stages with 9 components per stage.

#### Stages

+ D1 – Draft code: Identifying technical challenges and basic code contours.
+ D2 – Rewrite code: Improving efficiency and incorporating D1 hindsight.
+ D3 – Optimize code: Reduce code's time and resource footprint.

#### Components

+ Port – Build entry to showcase the project on portfolio website
+ Plan – Plan project tasks for each stage
+ Hand – Gather Twitter handles for congresspersons and comparators
+ Pull - Pull Twitter data from the API
+ Mung - Process Twitter data to format suitable for modeling
+ Mode – Find best hyperparameters for each model and fit models
+ Eval - Analyse model performance and interpret models
+ Pptx - Generate briefing visualizations for key results
+ Topi - Cluster terms and associate clusters with parties
+ Show - generate poster visualization of the results
+ Test – Formulate tests to confirm code works as intended.

#### Stage x Component Task Tracking Matrix

|   | D1| D2| D3|
|:- |:- |:- |:- |
Port| / |   |   |
Plan| X | X |   |
Hand| X | X |   |
Pull| X | X |   |
Mung| X | X |   |
Mode| X | / |   |
Eval| X |   |   |
Pptx| X | N | N |
Topi| / |   |   |
Show|   |   |   |
Test|   |   |   |
----|   |   |   |
Task|8.0|5.5|1.0|
Weig| 50| 35| 15|

KEY:
/ = Task partly complete.
X = Task fully complete.
N = Task N/A

## Percent Progress (D1 & D2)

((8.0 * 50) + (5.5 * 35)) / ((0.50 + 0.35) * 11) = 63%

#### Misc. To-Dos and Notes
+ NOTE: Data collection will need to be parallelized before it can be recycled at scale
+ TODO: clean up EVAL03
+ TODO: fix EVAL04 to use a dictionary instead of a list

## SOURCES

+ Project builds on the ideas in RAND working paper WRA1008, but takes a
different approach to the problem – using off-the-shelf machine learning
components instead of developing a new flavor of machine learning from scratch.

+ Twitter data is from the Twitter API via Python's Tweepy package.

+ US Congressperson handles from their public websites as listed in: senate.gov
and house.gov

+ Canadian parliamentarian handles from their public websites as listed in: ourcommmons.ca and sencanada.ca

## DIRECTORY LAYOUT
Project directories are lettered to indicate sequences, and code scripts are
numbered for the same reason.
+ A_Input - Original input data.  It should be read but never written.
+ B_Progress - Contains intermediate data as needed.  Generally, these files
facilitate data hand-offs between scripts.
+ C_Output - Tables and visualizations that are the project's final products.
+ Z_Admin - Documentation as needed to provide guidance and context for the
project. Most significantly, this directory contains any supplemental planning material.
