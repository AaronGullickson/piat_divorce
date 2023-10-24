---
editor: visual
---

# Data Source Description

The dataset we will use for this project is the [National Longitudinal Survey of Youth 1997](https://www.bls.gov/nls/nlsy97.htm). The survey was a representative national survey of adolescents in 1997. Since the original survey, these original respondents have completed 19 follow up survey, providing a wealth of data as these adolescents age into and through adulthood. We use a subset of data on individuals who have been married at least once in the data.

From the full data, I have extracted and recoded the following variables for our use as an analytical dataset. The dataset contains all individuals who have been married and were married at least five years or divorced within five years. To load this dataset in R, you just need to run the setup code chunk in the full_report.qmd quarto document. The name of the dataset in R is `nlsy`.

-   **divorce_five**: This is a TRUE/FALSE variable indicating whether the respondent was divorced within five years of being married. Individuals who report TRUE were divorced within five years, while those who report were not divorced within five years. This is the key dependent variable.
-   **high_grade**: The total number of years of schooling received by the respondent. This is the key independent variable.
-   **urbanicity**: This categorical variable is either "Urban" or "Rural" and indicates the respondent's urbanicity status in the survey wave after the marriage occurred.
-   **income**: This variable records the family income of the respondent in the survey wave after the marriage occurred.
-   **age_mar**: The age of the respondent when they were married.
-   **raised_two_bio**: A yes/no variable. If yes, this respondent was living with both biological parents in the initial survey wave.
-   **race**: The race of the respondent. The reference category of "Non-Black/Non-Hispanic" is heterogeneous but is mostly composed of white respondents.
