# Shot Decision-Making

## Where and Whether to Shoot? Quantifying Intelligence in Shooting Decision-Making

This repository contains supporting materials for our research submission to the **MIT Sloan Sports Analytics Conference 2027**.

-- Vincent Lee

The proposed framework evaluates two related decisions:

- **Where to shoot:** comparing the observed shot target with counterfactual target regions on the goal.
- **Whether to shoot:** comparing the scoring value of shooting with feasible passing alternatives.


## Data Availability

The data used in this project are StatsBomb event and freeze-frame data. An open-source example of StatsBomb data is available through the [Hudl StatsBomb Open Data repository](https://github.com/hudl/open-data).

Importantly, the methodology does not depend on a specific or study-exclusive dataset. It is designed to operate on compatible StatsBomb event and freeze-frame data in JSON format. It can therefore be applied to other leagues and seasons where data are available in the corresponding structure.

For the empirical analysis in this study, we use English Premier League and La Liga data from the 2022/23 to 2024/25 seasons. These licensed data are used as the empirical sample for evaluating the framework, rather than as a dataset required by the methodology.

## Methodological Overview

For shot-placement evaluation, the framework maps the shooting situation onto candidate goalmouth target regions and estimates the scoring likelihood associated with each alternative. The observed target is then compared with its counterfactual alternatives to quantify the quality of the placement decision.

For the shoot-or-pass decision, the value of the observed shot is compared with feasible passing alternatives using teammate positioning, shooting value, passing-lane geometry, and interception risk.

The resulting measures are aggregated to evaluate shooting decision-making at the player level.
