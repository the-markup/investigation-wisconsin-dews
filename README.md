# Data for our investigation into Wisconsin's dropout prediction algorithm

This contains the data we obtained through public records requests for the story ["False Alarm: How Wisconsin Uses Race and Income to Label Students 'High Risk'"](https://themarkup.org/TKTKTKT)

Wisconsin’s Department of Public Instruction maintains two predictive early warning systems for students. The Dropout Early Warning System (DEWS) predicts the likelihood that a student will graduate from high school on time. The College and Career Readiness Early Warning System (CCREWS) predicts whether students are ready for the ACT or college.

The “[DEWS_outcomes_aggregated](dews_outcomes_aggregated.csv)” dataset contains aggregate DEWS risk predictions from 2011 through 2021 broken down by academic year, district, grade, and student race.

The “[CCREWS_outcomes_aggregated](ccrews_outcomes_aggregated.csv)” dataset contains aggregate risk predictions from 2017 through 2021 broken down by academic year, district, grade, and student race.

Both datasets were provided by the Wisconsin Department of Public Instruction in response to a public records request. DPI redacted the aggregate student risk counts in some instances to preserve student privacy.

## Data dictionary for “DEWS_outcomes_aggregated”


| Column | Description |
| ------ | ----------- |
| SCHOOL_YEAR | The academic year the predictions were made |
| STUDENT_GRADE | The school grade level |
|DISTRICT_CODE | Wisconsin Department of Instruction’s code for the district |
| SCHOOL_DISTRICT | The name of the school district |
| STUDENT_RACE | The racial/ethnic group |
| STUDENT_RISK_OUTCOME | The predicted likelihood that a student won’t graduate from high school on time, designated as “Low,” “Moderate,” or “High” risk |
| STUDENT_COUNT | The number of students in a given racial/ethnic group assigned to a given risk category |
| STUDENT_TOTAL_COUNT | The number of students of a given race in a given year, district, and grade level |
| TOTAL_COUNT | This column is not used |


For more information, see [Wisconsin DPI's page on DEWS](https://dpi.wi.gov/wisedash/districts/about-data/dews).


## Data dictionary for “CCREWS_outcomes_aggregated”



| Column | Description |
| ------ | ----------- |
| SCHOOL_YEAR | The academic year the predictions were made |
| STUDENT_GRADE | The school grade level |
| DISTRICT_CODE | Wisconsin Department of Instruction’s code for the district |
| SCHOOL_DISTRICT | The name of the school district |
| STUDENT_RACE | The racial/ethnic group |
| TYPE | Which outcome is being predicted. Predictions about whether a student will enroll in a four-year college degree program are represented by “college.” Predictions about ACT readiness are represented by “3 of 4,” to indicate whether a student will meet the college enrollment benchmark in three out of four ACT subjects (English, math, reading, and science), or “4 of 4” to indicate whether a student will meet the benchmark in all four subjects. |
| STUDENT_RISK_OUTCOME | CCREWS’ prediction about whether a student will or won’t achieve the given outcome, designated as “ready” or “not_ready” |
| STUDENT_COUNT | The number of students in a given racial/ethnic group assigned to a given risk category |
| STUDENT_TOTAL_COUNT | The number of students of a given race in a given year, district, and grade level |
| TOTAL_COUNT | This column is not used |


For more information, see [Wisconsin DPI's page on CCREWS](https://dpi.wi.gov/ews/college-career-readiness).

