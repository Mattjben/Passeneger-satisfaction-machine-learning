# **Due at the End of Week 6 (20%):**

- Data cleaning and preprocessing (dealing with missing values, dropping ID-like columns, data aggregation, etc.) as appropriate.

- Data exploration and visualisation (charts, graphs, interactions, etc) as appropriate.

## **REQUIREMENT: The green-highlighted texts below must be the Section headers in your Phase 1 report**

- **(Task 0.1) (2 points)** Please give your project a proper title. Example: "Predicting Melbourne House Prices" etc.

- **(Task 0.2) (5 points)** Please include a proper Table of Contents.

- **(Task 1) (28 points total) Introduction:** This section needs to include the following subsections:
  - (Task 1.1) (3 points) Dataset Source: Please explain your data source properly and provide a proper citation in a References section at the end of your report.
  
  - **(Task 1.2) (5 points) Dataset Details:** Explain in sufficient detail what the dataset is about. Also please report the number of observations (rows) and the number of features (columns) in your dataset. And please print 10 random observations (rows) from your dataset. Please make sure we can see all the columns by adding this code in your report:

  ```python
  import pandas as pd
  pd.set_option('display.max_columns', None)
  ```

  - **(Task 1.3) (18 points) Dataset Features:** Explain the features in your dataset that you will be including in your project in a table format. To be clear, please include only the features you will use in your project and leave out the ones you will not be using in your project. In your table, you need to have one feature per row with the following 4 columns:
    1. Name of the feature
    2. Data type (numeric, binary, nominal categorical, ordinal categorical, date)
    3. Units ("Unknown" or "NA" for Not Applicable are acceptable)
    4. Brief description
  - **(Task 1.4) (2 points) Target Feature:** This is really important: you need to clearly identify your target feature. That is, what is it that you will be predicting in your Phase 2 report? Also state if it is a numerical or categorical feature.
- **(Task 2) (7 points**) Goals & Objectives for modelling this particular data.
- **(Task 3) (15 points)** Data Cleaning & Preprocessing as appropriate (dealing with missing values & outliers & incorrect values (such as negative age), dropping ID-like columns, data aggregation if necessary etc). If your dataset is already clean and ready for modelling, you will get the full score for this task, our treat! For this section, you will need to add subsections as appropriate for better organisation of your work.
  - **Task 3 Clarification #1:** Please do not perform any one-hot-encoding or scaling in Phase 1. Thank you.
  - **Task 3 Clarification #2:** For this task, sampling is optional: you can perform sampling (for a smaller dataset for ease of computation) either in Phase 1 or Phase 2, or you may choose to skip sampling all together if you like.
- **(Task 4) (15 points)** Data Exploration & Visualisation as appropriate with proper explanation: charts, graphs, boxplots, numerical summaries, etc. For this section, you will need to add subsections as appropriate for better organisation.
- **(Task 4.5) (Advanced Submission Mode Only, 15 points)** Literature Review This section needs to report and explain existing closely-related research studies in the particular field of your project. Please make sure you include some recent references published in the last few years. This section needs to include a minimum of 10 journal articles and a minimum of 4 conference papers in a dedicated References section at the end of your report (with correct APA citation style). In addition, this section needs to be at least 600 words excluding the references.
  - **Task 4.5 Clarification #1**: For this task, 8 points will be allocated to the comprehensiveness and accuracy of your literature review itself. The remaining 7 points will be allocated to the correctness & appropriateness of your references.
  - **Task 4.5 Clarification #2:** Links to some websites do not count as a journal article or a conference paper reference!
    - **Example of a journal article & its reference:**
      - Yum, H., Lee, B., and Chae, M. (2012). From the wisdom of crowds to my own judgment in microfinance through online peer-to-peer lending platforms. Electronic Commerce Research and Applications, Vol 11, pp. 469–483.
    - **Example of a conference paper & its reference:**
      - Backstrom, L., Huttenlocher, D., Kleinberg, J., and Lan, X. (2006). Group formation in large social networks: Membership, growth, and evolution. In 12th ACM International Conference on Knowledge Discovery and Data Mining, pp. 44–54.
- **(Task 5) (10 points)** Summary & Conclusions of the first phase of your project: a comprehensive summary of Phase 1 and any insights you gained in this phase as they relate to your goals and objectives.
- **(Task 6) (REQUIRED, 3 points)** References For citing any book, article, paper, website, etc. in your report, you need to use the APA style (Links to an external site.).

## **Plotting Requirements**

The minimum number of different plots you need to include in your Phase 1 report for the data exploration & visualisation part as follows:

- A group of 3 members: at least 4 plots of each one of the following: one-variable plot two-variable plots, and three-variable plots (that is, minimum 4*3=12 plots in total)

### **Additional plotting instructions are as follows**

1. For plotting, you are free to use whatever Python module you like: Matplotlib, Seaborn, Altair, Plotly, etc.
2. Your plots must be meaningful and they need to make sense with respect to the goals and objectives of your project.
3. As long as your plots are meaningful and relevant, there are no restrictions on the plot types. That is, you can have a mix of box-plots, histograms, line plots, scatter plots etc.
4. For each plot in your report, you will need to label the x- and y-axes as appropriate and also add a meaningful title.

## **Clarifications**

**CLARIFICATION #1 ON ASSESSMENT CRITERIA:**

The above assessment criteria only apply to "proper" project submissions. If your submission is fundamentally flawed, you may receive a mark of zero regardless of whatever else is in your report. For instance, if you fail to disclose the source of your dataset or use a blacklisted dataset you will not get any credits for your project.

**CLARIFICATION #2 ON ASSESSMENT CRITERIA:**

In case of the following mistakes, you will automatically loose the entire points corresponding to the Predictive Modelling, Critique & Limitations, and Summary & Conclusions sections:

Your report does not contain any predictive modelling procedures.
Your project uses time-series data wherein the rows in your dataset are correlated. Why? Because a fundamental assumption in machine learning in general is that the observations in your dataset are random samples from the entire population of observations.
You use an ID-like variable in your model. Remember, ID-like variables that have a unique value for each row (such as customer ID, patient ID, record no, student ID, etc) must be removed during the data pre-processing step before fitting any models. Why? Because including an ID-like variable in an ML model is such a huge mistake that it will render all your results meaningless.
