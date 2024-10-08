# R-homework

## [EDA of Airline Transport Data](https://github.com/vittoriashch/R-homework/blob/main/hw1.Rmd)
### Overview
This project explores airline transportation data with a focus on exploratory data analysis (EDA). The primary goal is to identify key insights about passenger traffic, trends in transportation, and potential factors influencing air travel patterns.

### Features

* Data Cleaning: Removal of null values and outliers for accurate analysis.
* Descriptive Statistics: Overview of data distributions and basic statistical metrics.
* Visualization: Comprehensive data visualization, including time-series graphs, histograms, and correlation heatmaps.
* Hypothesis Testing: Statistical tests to validate assumptions about the data.
## Tools Used
* R: Main programming language for data processing and visualization.
* ggplot2: Used for data visualization.
* dplyr: For efficient data manipulation.
### Insights
Significant fluctuations in passenger traffic during specific seasons.
Correlation between passenger numbers and external factors like fuel prices.
Key routes and their traffic patterns.
* [Dashboard](https://github.com/vittoriashch/R-homework/blob/main/hw1_dashboard.Rmd)


## [Marketing Campaign Analysis](https://github.com/vittoriashch/R-homework/blob/main/hw2.Rmd)
### Overview
This project focuses on analyzing customer behavior in response to various marketing campaigns. Using a dataset from a marketing campaign, the primary objectives are to explore customer engagement patterns, identify factors that influence campaign success, and provide insights into customer retention and segmentation strategies.

### Objectives
Customer Engagement Analysis: Investigate whether customers who responded to previous campaigns are more likely to respond to future ones.
Socioeconomic Influence: Analyze the impact of household income and wealth on the likelihood of submitting complaints.
Consumer Behavior Prediction: Build a decision tree model to predict customer responses based on past behavior and economic factors.
### Key Research Questions
* Response to Campaigns:

Do customers who responded to earlier campaigns tend to respond to future ones?
Using Chi-squared tests, this question is explored to find correlations between previous responses and future behavior.
Complaints and Income:

* Are wealthier customers more likely to leave complaints?
Through hypothesis testing (t-tests), the relationship between income and the likelihood of leaving complaints is analyzed.

### Data
The dataset used for this analysis contains information on various customer interactions with marketing campaigns, including:

* Customer demographics: Income, household status, etc.
* Previous campaign engagement: Whether customers responded to earlier campaigns.
* Consumer purchases: Data on customer shopping habits (e.g., wine, fruits, meat).
* Customer complaints: Information about complaints submitted by customers.
  
### Methods
* Chi-Squared Test: Used to analyze the relationship between campaign responses and customer retention.
* T-Tests: Applied to assess whether income levels are associated with customer complaints.
* Decision Tree Model: A classification tree is built to predict customer responses based on variables like income, previous campaign engagement, and purchase patterns.
### Tools Used
* R: Primary programming language for analysis and modeling.
* ggplot2: For visualizations.
* dplyr: For data manipulation and cleaning.
* rpart: For decision tree modeling and pruning.
### Results
* Campaign Responses: A significant correlation was found between previous campaign engagement and future responses. Customers who had responded to earlier campaigns were more likely to engage again.
* Income and Complaints: There was no statistically significant relationship between customer income and the likelihood of leaving complaints, indicating that complaints are not influenced by socioeconomic status.
* Decision Tree: The decision tree model provided a reasonably accurate prediction of customer responses to future campaigns based on past behavior and economic factors.
* [Dashboard](https://github.com/vittoriashch/R-homework/blob/main/hw2_dashboard.Rmd)
### Conclusion
The analysis highlights key factors influencing customer engagement and behavior in response to marketing campaigns. These insights can be used by businesses to design more effective, targeted campaigns, improving customer retention and overall campaign success.



## [Company Communication Network Analysis](https://github.com/vittoriashch/R-homework/blob/main/hw3.Rmd)

### Overview
This project focuses on analyzing the email communication patterns between employees of a company, using a subset of the Enron email dataset. The primary objectives are to explore how employees interact through email, identify key players within the communication network, and provide insights into the structure and dynamics of the company's internal communication.

### Objectives
Network Structure Analysis: Examine the email exchange network between employees during March 2001.
Key Employee Identification: Identify employees who are central in the network and play a crucial role in communication flow.
Communication Patterns: Understand the types of connections (direct and indirect) within the company and visualize the network to spot patterns of engagement.

### Key Research Questions
* Who are the key communicators?
Identify employees with the highest number of connections (degree centrality) and those who serve as bridges in communication (betweenness centrality).

* What are the dominant communication paths?
Explore the most common routes for information flow and the strongest connections within the email network.

* How structured is the network?
Assess the overall structure of the network to determine whether it is hierarchical, centralized, or decentralized.

### Data
The dataset used in this analysis includes information about email exchanges between employees of Enron. Each data point represents a directed edge from one employee to another.

* Employee Data: Email addresses, names, and roles.
* Email Metadata: Timestamps, recipient types (to, cc, bcc), and topic classifications.
* Communication Network: Vertices represent employees, and edges represent email exchanges between them.
  
### Methods
* Network Construction: A directed graph is constructed where nodes are employees and edges represent emails sent between them.
* Data Filtering: Emails outside the target time frame (March 2001) and self-loops (emails sent to oneself) are removed.
  
### Network Analysis:
* Degree Centrality: Measures the number of connections an employee has.
* Betweenness Centrality: Identifies employees who act as communication hubs, connecting different parts of the network.
* Simplification: Removes multiple edges and isolates for clearer analysis.
  
### Tools Used
* R: Primary programming language for data analysis and network modeling.
* igraph: For building and analyzing network graphs.
* dplyr: For data manipulation and cleaning.
* lubridate: For handling dates and times in the email dataset.

### Results
* Key Communicators: Several employees were identified as central figures in the communication network, responsible for managing critical email exchanges across the company.
* Communication Structure: The network revealed a moderately centralized structure, with a few key individuals handling a majority of email traffic, while most employees had fewer, more direct connections.
* Information Flow: Certain communication paths were more frequently used, showing that some teams or departments had stronger internal communication, while others relied more on key intermediaries.

### Visualization
The email network was visualized using a graph, with employees as nodes and email connections as edges. The size of the nodes indicates their centrality, and different colors were used to represent various teams or departments.

### Conclusion
The analysis provides valuable insights into the internal communication patterns within the company. Identifying key employees and understanding how information flows can help in improving communication strategies, ensuring more efficient information dissemination, and recognizing potential bottlenecks in the network.

