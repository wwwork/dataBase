# My Database interaction sсheme.

# 0. TASK: Store and separated data (NDA) and get it from remote database located on other Data Center in other country (DC).
*Because there some law regulation and restricts users data access in some customers countries.*

When the data of users  profiles cant store in customers DC, but might be the part of  single data.


The first implementation of the task, using Postgres_FDW module. 

The main **disadvantage** that is when remote DC is unavailable, all tables that connected to remote DC are **unavailable**.

This scheme implements store and separate data in the DATABASE layer.

![Aplication Layer Scheme](https://github.com/wwwork/dataBase/blob/master/FDW%20-%20remoteDbWithTempTable-main%20Schema.jpg?raw=true)

# 1. TASK: Store and separated data (NDA) and get it from remote database located on other DC.
The second implementation of the task, when the main requirements of Application conception were changes after it was developed.

The main **disadvantage** of this scheme is very large developing and debugging time.

This scheme implements store and separate data in the application layer.
![Aplication Layer Scheme](https://github.com/wwwork/dataBase/blob/master/remoteDb%20Api_gateway-main%20Schema.jpg?raw=true)


# 2. TASK: Store/separated data (NDA) and reduce development time and prevent data disappear if DC is unavailable.
The main GOAL of this implementation its reduce development time (up to 6 month) and prevent data to disappear if DC is unavailable.
This scheme implements store and separate data in DATABASE layer.

This objects code name is **"SGUSHENKA"** is because scheme drawings like "glass of condensed milk with sugar"
![Aplication Layer Scheme](https://github.com/wwwork/dataBase/blob/master/remoteDbWithTempTable-main%20Schema.jpg?raw=true)

