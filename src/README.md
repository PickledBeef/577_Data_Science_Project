- preparation: Data ingestion such as retrieving data from CSV, relational database, NoSQL, Hadoop etc. 
  We have to retrieve data from multiple sources all the time so we better to have a dedicated function for data retrieval. 
- processing: Data transformation as source data do not fit what model needs all the time. Ideally, we have clean data but I never get it. 
  You may say that we should have data engineering team helps on data transformation. However, we may not know what we need under studying data. 
  One of the important requirement is both off-line training and online prediction should use same pipeline to reduce misalignment.
- modeling: Model building such as tackling classification problem. 
  It should not just include model training part but also evaluation part. 
  On the other hand, we have to think about multiple models scenario. 
  Typical use case is ensemble model such as combing Logistic Regression model and Neural Network model.
  
- "prediction.ipynb" combines all the code files of the three directories.