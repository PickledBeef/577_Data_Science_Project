# Project respository for SP2021.T81.INFO.577.01 - Applied Data Science for Practitioners

### [Business problem from Kaggle](https://www.kaggle.com/sumithbhongale/american-university-data-ipeds-dataset)
- Most American institutions (that are not necessarily the top 10-20) that provide undergraduate education face a challenge i.e. what kind of students they will make an offer for admission so that they can maintain a good performance in terms of number of students completing their courses in time. They also need to predict how the current batch of intake will perform. The universities cannot relax the entry criteria too much as that way the quality of education that they provide gets diluted. At the other hand, they have to make offers to the candidates who are not only having appropriate profile but are also most likely to accept the offers.
On the other side, the students have a challenge deciding which colleges they should apply i.e. the colleges that provide best performance at a minimal cost given their own profiles. The student profile is determined by not only the performance in examination such as SAT and ACT, but also other data points such as their ethnicity, immigration status, gender etc.
We will be interested in answering three main questions for an institute i.e.

(a) What will be a likely enrollment rate?
(b) What will be a likely graduation rate?
(c) Which are the most lucrative colleges for students in terms of pass rate and cost?

- Dataset for this problem:
<br/>[“American University Data” IPEDS dataset](https://public.tableau.com/s/sites/default/files/media/Resources/IPEDS_data.xlsx)
<br/>Enrollment rate and graduation rate using machine learning and IPEDS dataset .

### Here is the explantation of folder strucure:
- src: Stores source code (python, R etc) which serves multiple scenarios.<br/> 
    During data exploration and model training, we have to transform data for particular purpose.<br/> 
    We have to use same code to transfer data during online prediction as well.<br/> 
    So it better separates code from notebook such that it serves different purpose.
- data: Folder for storing subset data for experiments. It includes both raw data, processed data and final output.
- notebook: Storing all notebooks includeing EDA and modeling stage.

### About database I used:
- [PostgreSQL](https://www.postgresql.org/): The World's Most Advanced Open Source Relational Database

### Interact with Windows Powershell:
- Start the server
<br/>`pg_ctl -D "C:\Program Files\PostgreSQL\13\data" start`
- Stop the server
<br/>`pg_ctl -D "C:\Program Files\PostgreSQL\13\data" stop`
- Restart the server
<br/>`pg_ctl -D "C:\Program Files\PostgreSQL\13\data" restart`    
- Connect database with username
<br/>`psql --username=postgres`

### About psql prompt after connect
- List all databases
<br/>`\l`
- Connect to a specific database
<br/>`\c t81577`
- List all tables
<br/>`\dt`
- Show content of a tables
<br/>`select * from cities`
    

