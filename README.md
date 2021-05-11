# Project respository for SP2021.T81.INFO.577.01 - Applied Data Science for Practitioners

### [Business problem from Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/overview)
- **Description:**<br/>
Ask a home buyer to describe their dream house, and they probably won't begin with the height of the basement ceiling 
or the proximity to an east-west railroad. But this playground competition's dataset proves that 
much more influences price negotiations than the number of bedrooms or a white-picket fence.<br/>
With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, 
this competition challenges you to predict the final price of each home.

- **Goal:**<br/> 
It is your job to predict the sales price for each house. For each Id in the test set, you must predict the value of the SalePrice variable.
 
- **Dataset for this problem:**<br/>
https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data<br/>

### Explantation for folder strucure:
- src(notebook): Stores source code (python, R etc) which serves multiple scenarios.<br/> 
    During data exploration and model training, we have to transform data for particular purpose.<br/> 
    We have to use same code to transfer data during prediction as well.<br/> 
    So it better separates code from notebook such that it serves different purpose.
- data: Folder for storing subset data for experiments. It includes both raw data, processed data and final output.

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
    

