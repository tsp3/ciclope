
import sqlite3

#this short function allows you to run queries by just passing the query through the function once youÕve altered the name of the file in definition

def qq(query_):
	resulting = sqlite3.connect(Ôyour_file_name.dbÕ).execute(query_).fetchall()
	return resulting 


# example - 
t1 = 'select Major from recent_gradsÕ;
print(qq(t1))
