# Database Server

> The project lab hosts a database server with MySQL and [Microsoft SQL](https://go.microsoft.com/fwlink/?linkid=866662) server installed and for use with in-class projects like internal assessments.

## General Information
For now, this server can be accessed locally from any of the IT labs, however there are future plans for the server to be made remotely available.

To gain access, speak to a computer science teacher and a set of personal credentials can be created for you.

## Connecting to The Database Server 
Once you have a set of credentials and a database created for you, you can either connect using `Beekeeper SQL`, by following the guide below: 

### Beekeeper SQL Guide
```pdf
    _media/SQLServerConnectionInstructions.pdf
```

## Python Connections
Or to access with a python project follow the set of instructions below. 

1. Make sure you are on a machine that has python `pip` support (if you are not sure what this means then ask Mr. Krishna).
2. Ensure your machine has the `SQL OBDC Driver` installed (this should have been done over Summer of 2022), if not, the link is [here](https://go.microsoft.com/fwlink/?linkid=2186919).
2. Open a powershell terminal and run the following command: `pip install pyodbc`
3. Now in your python project you can establish a connection to the database, by importing `pyodbc` and using the following code sample, changing relevant values.

```python
import pyodbc

server = "172.17.102.110"  # IP of the project rooms router 
database = "your username" # name of your database (your username)
uid = "your username"  # your username, first initial + last name
pwd = "your password"  # your password

# Specifying the ODBC driver, server name, database, etc. directly
cnxn = pyodbc.connect('DRIVER={ODBC Driver 18 for SQL Server};SERVER=' + server + ';DATABASE=' + database + ';UID=' + username + ';PWD=' + pwd)

# Create a cursor from the connection
cursor = cnxn.cursor()

# run a query that selects user_id, user_name from the users table <- change this to whatever query you want
cursor.execute("select user_id, user_name from users")
row = cursor.fetchone()
if row:
    print(row)
```