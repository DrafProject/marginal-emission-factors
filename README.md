| Tool | Paper | Data |
|-|-|-|
| [DrafProject/elmada](https://github.com/DrafProject/elmada) | [![paper doi](https://img.shields.io/badge/DOI-10.1016/j.apenergy.2021.117040-blue.svg)](https://doi.org/10.1016/j.apenergy.2021.117040) | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4718362.svg)](https://doi.org/10.5281/zenodo.4718362) |

# marginal-emission-factors

This directory provides updatable supplementary data to the journal paper [Fleschutz et al. (2021)](https://doi.org/10.1016/j.apenergy.2021.117040).

The data was calculated using the tool [DrafProject/elmada](https://github.com/DrafProject/elmada), see [make_MEF_data.ipynb](make_MEF_data.ipynb).

The time series were calculated in hourly resolution (`data/60min`), and were additionally converted to quarter-hourly resolution (`data/15min`).

## Data description

| Column name   | Data type | Unit            | Description     |
| ------------- |-----------| --------------- | ----------------|
| T             | Integer   | Hour/Quarterhour| Hour/Quarterhour of the year starting with `0`. |
| residual_load | Float     | MW_el           | Average residual national load. |
| total_load    | Float     | MW_el           | Average total national load. |
| marginal_fuel | String    | -               | Fuel type of marginal power plant. One of `lignite`, `coal`, `gas`, `gas_cc`, and `oil`. |
| efficiency    | Float     | -               | Efficiency of marginal power plant between 0 and 1. |
| marginal_cost | Float     | € / MWh_el      | Marginal cost of electricity generation. |
| MEFs          | Float     | kg_CO2eq/MWh_el | Marginal emission factors. I.e. the carbon emission intensity of electricity generation of the marginal power plant. |
| XEFs          | Float     | kg_CO2eq/MWh_el | Average electricity grid mix emission factors. |

### Time zones

The data is in local time since the [Draf Project](https://github.com/DrafProject) focuses on the modeling of individual energy hubs.
Standard time is used i.e. daylight saving time is ignored.

The time zones are:

| Country | UTC offset | Time zone |
| ------- | ---------- | -------- |
| AT | UTC+1:00 | Europe/Vienna |
| BE | UTC+1:00 | Europe/Brussels |
| CZ | UTC+1:00 | Europe/Prague |
| DE | UTC+1:00 | Europe/Berlin |
| DK | UTC+1:00 | Europe/Copenhagen |
| ES | UTC+1:00 | Europe/Madrid |
| FI | UTC+2:00 | Europe/Helsinki |
| FR | UTC+1:00 | Europe/Paris |
| GB | UTC+0:00 | Europe/London |
| GR | UTC+2:00 | Europe/Athens |
| HU | UTC+1:00 | Europe/Budapest |
| IE | UTC+0:00 | Europe/Dublin |
| IT | UTC+1:00 | Europe/Rome |
| LT | UTC+2:00 | Europe/Vilnius |
| NL | UTC+1:00 | Europe/Amsterdam |
| PL | UTC+1:00 | Europe/Warsaw |
| PT | UTC+0:00 | Europe/Lisbon |
| RO | UTC+2:00 | Europe/Bucharest |
| RS | UTC+1:00 | Europe/Belgrade |
| SI | UTC+1:00 | Europe/Ljubljana |

## License

Data is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0).

## How to cite this data

If you use this data, please consider citing the open access journal paper [Fleschutz et al. (2021)](https://doi.org/10.1016/j.apenergy.2021.117040).
