# Project respository for SP2021.T81.INFO.577.01 - Applied Data Science for Practitioners

### Here is the explantation of folder strucure:
- src: Stores source code (python, R etc) which serves multiple scenarios. During data exploration and model training, we have to transform data for particular purpose. We have to use same code to transfer data during online prediction as well. So it better separates code from notebook such that it serves different purpose.
- test: In R&D, data science focus on building model but not make sure everything work well in unexpected scenario. However, it will be a trouble if deploying model to API. Also, test cases guarantee backward compatible issue but it takes time to implement it.
- model: Folder for storing binary (json or other format) file for local use.
- data: Folder for storing subset data for experiments. It includes both raw data and processed data for temporary use.
- notebook: Storing all notebooks includeing EDA and modeling stage.

### About database I used:
- [PostgreSQL]: The World's Most Advanced Open Source Relational Database(https://www.postgresql.org/)

### Interact with Windows Powershell:
- Start the server
    pg_ctl -D "C:\Program Files\PostgreSQL\13\data" start
- Stop the server
    pg_ctl -D "C:\Program Files\PostgreSQL\13\data" stop
- Restart the server
    pg_ctl -D "C:\Program Files\PostgreSQL\13\data" restart    
- Connect database with username
    psql --username=postgres

### About psql prompt after connect
- List all databases
    \l
- Connect to a specific database
    \c t81577
- List all tables
    \dt
- Show content of a tables
    select \* from cities
    

