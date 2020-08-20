
# README for using the Elections Performance Index data

#### MIT Election and Data Science Lab

#### Jack Williams

The data file `epi_indicators-all_years` contains all of the non-normalized indicator scores for the [Elections Performance Index](https://elections.mit.edu/) (EPI). These scores are produced through a large data collection and cleaning effort as part of the overall development of the EPI. More information on that process can be found in the [EPI Methodology Report](https://elections.mit.edu/2016-epi-methodology.pdf).

The data file `epi_index_2018` contains the EPI scores for 2018. Calculations before 2016 were conducted by the Pew Charitable Trusts and can be found on on the [EPI website](https://elections.mit.edu).

Contact [Jack R. Williams](mailto:jackrw@mit.edu) for any questions or to report errors.

## Codebook for `epi_indicators-all_years` dataset
The variables are listed as they appear in the data file.  


### `state_abbv`
 - **Description**: state abbreviation

 ---------------

### `state_fips`
 - **Description**: State FIPS code

----------------

### `year`
 - **Description**: election year corresponding to EPI indicators

---------------

### `website_pollingplace`
 - **Description**: Can you look up your polling place online?
 - **Source**: MIT Election and Data Science Lab coding of state policies
 - **Coding**:

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |

----------------

### `website_reg_status`
 - **Description**: Can you look up your voter registration status online?
 - **Source**: MIT Election and Data Science Lab coding of state policies
 - **Coding**:

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |

----------------


### `website_precinct_ballot`
- **Description**: Can you see a precinct-level sample ballot online?
- **Source**: MIT Election and Data Science Lab coding of state policies
- **Coding**  

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |

  - **Note**: This was not measured in 2008.


----------------

### `website_absentee_status`
  - **Description**: Can you check your absentee ballot status online?
  -  **Source**: MIT Election and Data Science Lab coding of state policies
  - **Coding:**  

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |

  - **Note**: This was not measured in 2008.

----------------

### `website_provisional_status`
  - **Description**: Can you check your provisional ballot status online?
  - **Source**: MIT Election and Data Science Lab coding of state policies
  - **Coding:**  

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |

  - **Note**: This was not measured in 2008.

----------------

### `reg_rej`
  - **Description**: Registration rejection rate
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[0, .67197359]` | Numeric |


----------------

### `prov_partic`
  - **Description**: Percent casting provisional ballot
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.00001733, .13130152]` | Numeric |


----------------

### `prov_rej_all`
  - **Description**: Provisional rejection rate
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[0, .01916237]` | Numeric |


----------------

### `abs_rej_all_ballots`
  - **Description**: Absentee rejection rate of all ballots
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[0, .01335678]` | Numeric |


----------------

### `abs_nonret`
  - **Description**: Absentee non-return rate
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[0, .51564848]` | Numeric |


----------------

### `uocava_rej`
  - **Description**: UOCAVA rejection rate
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[0, .25336698]` | Numeric |


----------------

### `uocava_nonret`
  - **Description**: UOCAVA non-return rate
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.01302932, .88048917]` | Numeric |


----------------

### `eavs_completeness`
  - **Description**: Percent completeness on key questions in 2016 EAVS survey
  - **Source:** [EAC Election Administration and Voting Survey](https://www.eac.gov/research-and-data/election-administration-voting-survey/)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[0, 1]` | Numeric |


----------------

### `post_election_audit`
  - **Description**:
  - **Source:** MIT Election and Data Science Lab coding of state policies
  - **Coding:** Post-election audit required

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |


----------------

### `nonvoter_illness_pct`
  - **Description**: Percent non-voters because illness/disability
  - **Source:** [Voting and Registration Supplement to the Current Population Survey](https://www.census.gov/topics/public-sector/voting/data/tables.html)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.03416906, .26005191]` | Numeric |


----------------

### `nonvoter_reg_pct`
  - **Description**: Percent non-voters because registration problem
  - **Source:** [Voting and Registration Supplement to the Current Population Survey](https://www.census.gov/topics/public-sector/voting/data/tables.html)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.00745624, .13933808]` | Numeric |


----------------

### `online_reg`
  - **Description**: Can you register to vote online?
  - **Source:** MIT Election and Data Science Lab coding of state policies
  - **Coding:**  

| Value | Description |
| --- | --- |
| `1` | yes |
| `0` | no |


----------------

### `wait`
  - **Description**: Wait time from SPAE and CCES
  - **Source:** [Survey of the Performance of American Elections](https://dataverse.harvard.edu/dataverse/SPAE), [Cooperative Congressional Election Study](https://dataverse.harvard.edu/dataverse/cces)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.406409, 61.502129]` | Numeric |

  - **Note**: This was not measured in 2010. Additionally, data was imputed using CCES, due to no SPAE in 2018. See methodology update for more information

----------------


### `residual`
  - **Description**: Residual vote rate
  - **Source:** MIT Election Data and Science Lab
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.0000391, .03168843]` | Numeric |

  - **Note**: This is only available for presidential election years.

----------------


### `pct_reg_of_vep_vrs`
  - **Description**: Residual vote rate
  - **Source:** [Voting and Registration Supplement to the Current Population Survey](https://www.census.gov/topics/public-sector/voting/data/tables.html)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.64003599, .93633616]` | Numeric |


----------------

### `vep_turnout`
  - **Description**: Turnout as a percent of VEP
  - **Source:** [U.S. Elections Project](http://www.electproject.org)
  - **Coding:**  

| Value | Description |
| --- | --- |
| `[.28341606, .78102571]` | Numeric |


----------------

## Version
- 20200820
