# BHDS2010-Final-Project-
Repository containing files associated with BHDS 2010 Assignment 4


**Purpose:** 
The purpose of our Shiny app is to let users explore the Healthcare Access and Quality (HAQ) Index across 204 countries and territories from 1990–2019.
The app will provide interactive visualization of HAQ Index values, HAQ indicators (the 32 causes that should not occur under adequate care), and uncertainty intervals.
Users will be able to view changes over time, compare age groups, and examine HAQ performance across locations.

**App Layout**
<u>Inputs</u> 
* Upload dataset (default = GBD 2019 HAQ dataset CSV)
* Select country / location
* Select year 
* Select age-group type (overall, young, working, post-working)
* Select measure type (Index, MIR, RSD)
* Select indicator (optional for detailed drill-down)
<u>Outputs</u>
* Summary statistics table showing HAQ values and uncertainty intervals
* Visualization(s):
  * Bar plot comparing HAQ Index between 1990 and 2019
  * Scatterplot comparing HAQ Index vs MIR/RSD
  * Line plot (if user selects multiple years) to show HAQ change 
* text description summarizing the selection (ex: location + result interpretation)
* Optional CSV export of filtered output
<u>UI description text</u>
* At the top, include a brief description explaining what HAQ Index measures, why the 32 causes are included, and how the index reflects access + quality of care.

**Features**
* Load default GBD 2019 HAQ CSV or a user-uploaded file
* Filter by location, age group type, measure, indicator, year
* Display mean estimates and 95% uncertainty intervals
* Generate interactive plots (bar, line, scatter) to compare HAQ performance across time and groups
* Allow users to extract a subset of the data and download it
* Potential statistical additions:
  *compute absolute/percent change in HAQ from 1990 → 2019 
rank countries by HAQ score
map visualization (optional extension)
