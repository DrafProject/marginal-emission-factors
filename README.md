# marginal-emission-factors
This directory provides updatable supplementary data to a journal paper which will be referenced here as soon as it is published.

## Data description
| Column name   | Data type | Unit            | Description     |
| ------------- |-----------| --------------- | ----------------|
| T             | Integer   | Hour            | Hour of the year starting with `0`. |
| residual_load | Float     | MW_el           | Average residual national load. |
| total_load    | Float     | MW_el           | Average total national load. |
| marginal_fuel | String    | -               | Fuel type of marginal power plant. One of `lignite`, `coal`, `gas`, `gas_cc`, and `oil`. |
| efficiency    | Float     | -               | Efficiency of marginal power plant between 0 and 1. |
| marginal_cost | Float     | € / MWh_el      | Marginal cost of electricity generation. |
| MEFs          | Float     | kg_CO2eq/MWh_el | Marginal emission factors. I.e. the carbon emission intensity of electricity generation of the marginal power plant. |
| XEFs          | Float     | kg_CO2eq/MWh_el | Average electricity grid mix emission factors. |

## License
Data is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0).

## How to cite this data
Coming soon.
