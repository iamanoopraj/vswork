<<<<<<< HEAD
Readme created.
import os

import pandas as pd
import numpy as pd
import mysql.connector 
from dotenv import load_dotenv

load_dotenv()
host = os.getenv('HOST')
username = os.getenv('USER')
password = os.getenv('PASWORD')

connection = mysql.connector.connect(host=host,
                                     user=username,
                                     password=password,
                                     database='swiftmarket')

cursor = connection.cursor()





def queryToDataFrame(query):

    cursor. execute(query)
    rows = cursor.fetchall()
    df = pd.DataFrame(data=rows,columns=cursor.column_names)
    return df

def shoeTables():
query = """SHOW TABLES;"""
cursor.execute(query)
rows = cursor.fetchall()
df = pd.DataFrame(data=rows,columns=cursor.column_names)
retrun df

def describeTable(tablename):
query = f"""describe {tablename};"""
cursor.execute(query)
rows = cursor.fetchall()
df = pd.DataFrame(data=rows,columns=cursor_names)
return df

=======
# Header level 1
## header level 2
#### header level 4
-
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

This data was colected from [Kaggle](https://www.kaggle.com/datasets/mhadani/predictive-maintenance-aircraft-engine).
--
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

* This is star
* Another star

1. This is number
2. Another number

- This is dash
- Another dash
  


The following code does this....
```python
def showTables():
    query = """SHOW TABLES;"""
    cursor. execute(query)
    rows = cursor.fetchall()
    df = pd.DataFrame(data=rows,columns=cursor.column_names)
    return df
```
The above code does this...

|Names|Designation|
|------|-----------|
|DevA  | Developer |
|DevV  | CTO  |


![Image](https://th.bing.com/th/id/OIP.qJblymcwhKgizHC0Grbx1AHaE7?w=251&h=180&c=7&r=0&o=5&dpr=1.3&pid=1.7)

>>>>>>> 1ed44a7229cbedd83bb3765291cb629f7a385909
