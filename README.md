# My Database interaction sсheme.

# 0. TASK: Store and separated data (NDA) and get it from remote database located on other Data Center in other country (DC).
First implementation of task, with using Postgres_FDW module. 
The main **disadvantage** that is when remote DC is anavaliable, all tables that connected to remote DC is **unavailable**.
This scheme implemets store and separate data in DATABASE layer.
![Aplication Layer Scheme](https://github.com/wwwork/dataBase/blob/master/FDW%20-%20remoteDbWithTempTable-main%20Schema.jpg?raw=true)

# 1. TASK: Store and separated data (NDA) and get it from remote database located on other DC.
Second implementation of task, when main requirments of Aplication conception was changes after it was developed.

This scheme implemets store and separate data in aplication layer
![Aplication Layer Scheme](https://github.com/wwwork/dataBase/blob/master/remoteDb%20Api_gateway-main%20Schema.jpg?raw=true)


# 2. TASK: Store/separated data (NDA) and reduce development time and prevent data from disappear if DC is unavailable.
It's the second implementation of a task, the main GOAL of this task its to reduce development time and prevent data dasapear if DC is unavailable.
This scheme implemets store and separate data in DATABASE layer.

This objects code name is **"SGUSHCHENKA"**  is because scheme draiwins like "condensed milk with sugar"
![Aplication Layer Scheme](https://github.com/wwwork/dataBase/blob/master/remoteDbWithTempTable-main%20Schema.jpg?raw=true)

