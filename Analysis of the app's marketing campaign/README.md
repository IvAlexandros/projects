# Description of project "Analysis of the marketing campaign of an entertainment application"
The dataset for the project is provided by the Yandex Practicum educational service. The project was carried out during the studying the profession "Data Analyst" in the Yandex Practicum.
## Brief description, goal and tasks of the project
Datasets for analysis were provided by the educational service Yandex Practicum.\
Brief description: despite huge investments in advertising, the company has been suffering losses for the last few months.
The goal is to understand the reasons and help the company to come in positive.\
We have data about users attracted from May 1 to October 27, 2019:
- server log with data about their visits,
- data about their purchases for this period,
- advertising expenses.

The following tasks are to be solved:
- find out where do users come from and what devices they use,
- how much does it cost to attract users from various advertising channels;
- how much money does each client bring,
- in which case the costs of attracting clients pays off,
- what factors hinder the attraction of customers.
  
## Decomposition of the work
- Step 1 - Data preprocessing
  - Downloading the data, studying what is presented there. Checking data types, bringing the column names to one style. Also exploring gaps in data.

- Step 2 - Calculation of marketing campaign performance indicators\
  Setting functions for calculating the necessary indicators of marketing campaign analysis: LTV, ROI, retention and conversion rate.\
  These are functions for such metricks:
  - get_profiles() — to create user profiles,
  - get_retention() — calculation of Retention Rate,
  - get_conversion() — calculation of Conversion Rate,
  - get_ltv() — calculation of LTV
  
  As well as functions for plotting:
  - filter_data() — for smoothing data,
  - plot_retention() — for plotting Retention Rate,
  - plot_conversion() — for plotting conversion,
  - plot_ltv_roi — for LTV and ROI visualization.

- Step 3. Exploratory data analysis
  - Creation of user profiles. Specification of the minimum and maximum dates for attracting users.\
  - Finding out from which countries users come to the application and which country accounts for the biggest number of paying users.\
  - We will build a table reflecting the number of users and the share of those who are paying from each country.\
  - We will find out which devices are used by customers and which devices are preferred by paying users. Let's build a table reflecting the number of users and the share of those paying for each device.\
  - Studying the advertising sources of engagement and determining the channels from which most of paying users came. Building a table reflecting the number of users and the share of payers for each engagement channel.

- Step 4. Marketing
  - Let's calculate the total amount of marketing expenses.
  - We need to find out how the expenses are distributed by advertising sources, that is, how much money was spent on each source.
  - Then we build a visualization of the dynamics of changes in expenses over time (by weeks and months) for each source.
  - Also we will find out how much it cost on average to attract one user (CAC) from each source.
  
- Step 5. Evaluation of the payback of advertising\
  - Analysis of the payback of advertising using LTV and ROI charts, as well as charts of the dynamics of LTV, CAC and ROI.
  - Checking user conversion and the dynamics of its change. The same for user retention. Building and studying conversion and retention charts.
  - Analysis of the payback of advertising by device. Plotting LTV and ROI graphs, as well as LTV, CAC and ROI dynamics graphs.
  - Analysis of the payback of advertising by country. Plotting LTV and ROI graphs, as well as LTV, CAC and ROI dynamics graphs.
  - Analysis of the payback of advertising, broken down by advertising channels. Plotting LTV and ROI graphs, as well as LTV, CAC and ROI dynamics graphs.
  
- Step 6. Final conclusions
  - The reasons for the inefficiency of attracting users.
  - Recommendations for the marketing department.
