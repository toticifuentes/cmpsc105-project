# Exploratory Data Analysis (EDA)
## Dataset Overview

For our project, we are using a dataset called `engineering_trends.csv`, which contains information about people working in programming and technology. The dataset has 30,903 observations and 212 variables, including education, employment, work experience, salary, job satisfaction, and AI usage. Our main goal is to explore the data and understand some of the relationships between professional experience, compensation, and the use of AI tools.

## 1. Data Ingestion & Cleaning — Jose

We started by importing the dataset into Pandas and looking at the first five rows to understand how the data was organized. We also checked the different data types, missing values, and duplicates. One thing we noticed was that there were a lot of missing values. In fact, 179 columns had more than 50% missing data. We decided not to replace these missing values with zero because some people might have skipped questions or certain questions might not have applied to them. We also checked for duplicates and found that there were no duplicate rows or response IDs. After that, we converted the numerical variables into the correct format and checked for negative values in experience and compensation. Our cleaned dataset still had 30,903 observations and 212 variables.

## 2. Summary Statistics — Alif

For this part, we calculated the mean, median, standard deviation, and missing values for some of the most important numerical variables. One thing that stood out was that the average professional work experience was 14.26 years, while the median was 12 years. For annual compensation, the average was around $106,535, while the median was $79,610. This difference suggests that some respondents with very high salaries might be increasing the average. We also looked at categorical variables such as education, employment, and country. Around 40% of respondents had a bachelor's degree, and about 65.6% were employed. Another thing we noticed was that some variables, especially the number of AI tools, had extremely high values that did not seem realistic. This is something we will need to consider when analyzing the data further.

## 3. Initial Visualizations — Jose

For this section, I created graphs to better understand the relationship between professional experience and compensation. The first graph was a histogram showing the distribution of professional work experience. This helped us understand how experience varies among respondents and identify the most common experience levels. The second graph was a scatter plot comparing professional experience with annual compensation. I wanted to see if people with more experience generally earned more money. I also excluded the highest 1% of salaries from the graph to make it easier to see the main distribution of the data. The third graph was a box plot comparing annual compensation across different experience groups. This helped us compare median salaries and see how compensation varies between people with different levels of experience. Overall, these graphs give us a better idea of how experience and compensation might be related, but we cannot say that experience alone determines salary because other factors, such as country, education, and job position, could also have an impact.

## 4. Dataset Quirks & Limitations — Sedan

One of the biggest challenges with this dataset is the amount of missing information. For example, more than half of the respondents did not report their annual compensation. This could affect our results because we are only analyzing the people who answered those questions. Another issue is that some variables have extremely high values. For example, the AI tool count variable includes values that are clearly unrealistic, which makes the average much higher than the median. We also have to consider that respondents come from different countries, where salaries and working conditions can be very different. Additionally, the data is self-reported, so we cannot guarantee that every answer is completely accurate. Because of these limitations, we need to be careful when interpreting our results and making conclusions about the technology industry as a whole.

## 5. Next Steps

For our next deliverable, we want to explore the relationships between work experience, compensation, and AI usage in more detail. We also want to look at how other variables, such as education, country, and job position, might influence these relationships. I think one of the most interesting things to investigate further is whether having more professional experience is associated with higher compensation and whether AI adoption differs depending on someone's experience level.
