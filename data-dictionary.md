# Data Dictionary — Alzheimer Latin America Dashboard

**Dataset DOI**: [10.7910/DVN/UVHABW](https://doi.org/10.7910/DVN/UVHABW)  
**Last updated**: 2025  
**Coverage**: 8 Latin American countries, 2000–2050

---

## Files

| File | Description |
|------|-------------|
| `alzheimer_data.csv` | Main longitudinal dataset |
| `policy_index.csv` | Dementia policy scores by country |
| `caregiver_burden.csv` | Caregiver burden indicators |
| `projections_2050.csv` | WHO-based prevalence projections |

---

## Variables

### alzheimer_data.csv

| Variable | Type | Unit | Description | Source |
|----------|------|------|-------------|--------|
| `country` | string | ISO 3166-1 alpha-2 | Country code (AR, BO, BR, CL, CO, MX, PE, VE) | — |
| `country_name` | string | — | Full country name in English | — |
| `year` | integer | YYYY | Reference year | — |
| `prevalence_rate` | float | % of population 60+ | Alzheimer's prevalence rate | GBD 2021 |
| `prevalence_cases` | integer | persons | Estimated number of cases | GBD 2021 |
| `incidence_rate` | float | per 100,000 | New cases per year per 100,000 | GBD 2021 |
| `mortality_rate` | float | per 100,000 | Deaths attributable to Alzheimer's | GBD 2021 |
| `dalys` | float | DALYs per 100,000 | Disability-adjusted life years | GBD 2021 |
| `population_60plus` | integer | persons | Population aged 60 and over | UN WPP |
| `gdp_per_capita` | float | USD (current) | GDP per capita | World Bank |
| `health_expenditure_pct` | float | % of GDP | Total health expenditure | WHO |

### policy_index.csv

| Variable | Type | Unit | Description |
|----------|------|------|-------------|
| `country` | string | ISO alpha-2 | Country code |
| `year` | integer | YYYY | Reference year |
| `policy_score` | float | 0–10 | Composite dementia policy score |
| `has_national_plan` | boolean | — | National dementia plan exists |
| `care_infrastructure` | float | 0–5 | Care infrastructure score |
| `awareness_campaigns` | integer | count | Number of awareness campaigns |

### caregiver_burden.csv

| Variable | Type | Unit | Description |
|----------|------|------|-------------|
| `country` | string | ISO alpha-2 | Country code |
| `year` | integer | YYYY | Reference year |
| `informal_caregivers_pct` | float | % | Share of caregiving by informal caregivers |
| `caregiver_hours_weekly` | float | hours/week | Average weekly hours of care |
| `economic_cost_usd` | float | USD millions | Economic cost of informal care |
| `caregiver_depression_rate` | float | % | Prevalence of depression in caregivers |

---

## Country Coverage

| ISO Code | Country |
|----------|---------|
| AR | Argentina |
| BO | Bolivia |
| BR | Brazil |
| CL | Chile |
| CO | Colombia |
| MX | Mexico |
| PE | Peru |
| VE | Venezuela |

---

## Missing Values

Missing values are represented as empty cells in CSV files (not as `NA`, `NaN`, or `NULL`).

## Data Sources

| Source | Description | URL |
|--------|-------------|-----|
| GBD 2021 | Global Burden of Disease Study 2021 | [healthdata.org](https://www.healthdata.org/gbd/2021) |
| UN WPP 2022 | UN World Population Prospects | [population.un.org](https://population.un.org/wpp/) |
| World Bank | World Development Indicators | [data.worldbank.org](https://data.worldbank.org/) |
| WHO | World Health Organization | [who.int](https://www.who.int/data) |

## License

This dataset is released under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/).
Attribution: de la Serna, Juan Moisés (2025). Alzheimer Latin America Dashboard. Harvard Dataverse. DOI: 10.7910/DVN/UVHABW
