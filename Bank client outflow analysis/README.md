# Description of project "Analysis of the outflow of bank customers"
The dataset for the project is provided by the Yandex Practicum educational service. The project was carried out during the studying the profession "Data Analyst" in the Yandex Practicum.
## Brief goal and tasks of the project
Datasets for analysis were provided by the educational service Yandex Practicum.\
The purpose of the study is to identify activities that can be carried out retain those who may leave and possibly to bring back departed customers.\
Main tasks:
- segment customers into compact homogeneous segments;
- identify segments of customers who tend to leave the bank;
- form recommendations for retaining customers and returning those who have left.
## Decomposition of the work
1) Examining general information: what kind of data is presented and what information is available to us.
2) Data preparation:
* Investigate data types and replace them if necessary;
* Encode categorical variables in the column with the city and gender using the one-hot method.
* Study the column names and bring them to a single style;
* Explore gaps: if possible, replace the omissions, delete or leave as is, depending on the type of omission:\
  -- Research how columns with omissions correlate with the available data;\
  -- MСAR omissions can be left or filled in with values that will not harm the distribution of column values.;\
  -- MAR - we can fill in with the average/median for each group associated with a omission, taking into account the number of gaps;\
  -- MNAR - it is impossible to fill in or delete omissions without additional justification, in such case the omissions will have to be left without intervention.
* Examine the data for explicit and implicit duplicates and delete them if allowed.
3) Exploratory data analysis:
* Examine the distribution of values of each column;
* View indicators of descriptive statistics for columns;
* Based on the average value, median, fashion, look at a typical customer in the context of high-quality and non-high-quality customers.
* Correlation analysis:\
  -- Calculate and analyze correlations of data of all columns with a column with a sign of outflow using the phik coefficient;\
  -- Graphically display the correlation using correlation matrices with a color scale for visual analysis;\
  -- Select those parameters where the correlation score is higher than 10%.
* Study of portraits of outgoing clients:
  -- Compare quantitative portraits of clients, i.e. indicators of typical clients.\
Take the appropriate statistical value and calculate for each characteristic by how many percent this number is greater (less) for outflow clients compared to the non-outflow. What will be less than 10% modulo can be checked by stat. criterion for reliability.\
  -- For the selected continuous values, plot the probability distribution density for the outflow and non-outflow clients to determine the ranges where the outflow is stronger than for the dataset as a whole.
4) Test hypotheses:
* For continuous variables use the Student's t-test or the Mann-Whitney u-test. Justify the choice. For the proportions test use the z-test for proportions.
* Test the hypothesis of income differences between those customers who are ready to leave and those who remain.
* Test the hypothesis of differences in average scoring numbers.
* Test the hypothesis of the difference in the average age of leaving and non-leaving clients.
5) Interim results and segmentation:
* To put together the results of the analysis and indicate which signs have the strongest effect on the outflow of clients and what values or ranges of values they take.
* Divide clients according to the criterias: the size of groups from 300 to 2000 people, the share of leaving clients in the group is at least 1.3 times higher than the average for the dataset.
6) Conclusions:
* Specify customer segments that tend to leave more often than others.
* Generate recommendations for returning customers and retaining customers who are inclined to leave.

