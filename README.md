![](img/Map copy.png) 

## Bakerloo Line Extension Station Location Analysis
This document summarizes the key findings and methodology of a research project using linear programming to analyze optimal station locations for the Bakerloo Line Extension (BLE) in South London.

### Motivation:

South London residents lack adequate public transit access, limiting job opportunities and commute options. The proposed BLE aims to improve accessibility and revitalize the area. This project aims to inform the BLE's station location planning process by identifying optimal station locations that minimize walking time to stations. A benchmark of 10 minutes is used to evaluate the results.

### Methodology:

Two linear programming models were used for the same purpose, but with different objective functions and constraints formulation:

- _Location Set Covering Problem (Problem 1):_ Minimizes the number of stations needed to cover all demand within a set walking time Y).
- _Adapted P-Median Problem (Problem 2):_ Minimizes the total walking time to stations given a number of station k.

<img src="img/formulation.png" alt="formula" width="500"/>

### Results:

- Problem 1 has no feasible solutions that are close to the 10-minute walking time benchmark.
- Problem 2 finds optimal solutions for all numbers of stations between 3 (min) and 31 (max). An optimal solution with 586 seconds (~10 minutes) average walking time is reached when having _7 stations_

### Recommendations:

When reconciled with TfL proposal, the recommendation is to build 6 new stations along the BLE, two more than TfL's current proposal (see map)
Consider using the model's insights to inform further studies incorporating:

- Transit usage propensity and future demand.
- Local political considerations.
- Engineering feasibility of station locations.
- Different routing services for walking time calculations.
