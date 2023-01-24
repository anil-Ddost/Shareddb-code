# Shareddb-code
this repository will be available for code for Anil/Devendra
______________________________________________________________________________
## Connect to Postgres database using Jupyter notebook

pip install psycopg2

import psycopg2

con = psycopg2.connect(
database ="dawaadost-dev",
user = "Postgres",
password = "Daw@@d0$t",
host ="34.93.78.248",
port ='5432'
)

cursor_obj = con.cursor()

cursor_obj.execute("SELECT * FROM medicines LIMIT 5")

result = cursor_obj.fetchall()

display(result)
