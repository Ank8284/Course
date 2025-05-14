# How to form connection with psycopg2 in python ?
    -> One has to Import psycopg2 library 
    -> Form connection with psycopg2 with " .connect() " ##this will make virtual enviorment for a python complier
    ## to perform certain command which is expilitvely available inside a DBMS server
    -> make a cursor so program can irritate within said virtual enviorment
    -> now write a desired command with ''' xyz.... ''' inside a variable
    -> now use variable connection from step 1 to commit the command by " .commit() "
    -> to get result use " .fetcall() "
    -> now close all by " .close() " \\ connection,cursor

# What are benefit of using Database with in a program ?
\-- within Database act as backend support for the python program, 
    it is used to store data in form of table which is vible solution for
    storing large number of dataset as in python creating table and then 
    storing data into those table is good approch for a new be but for a
    hardcore python progarm is nessary to relay on backend server like 
    this psycopg2 

# What is Syntax/Structure?
 ## Syntax:

    import os, sys
    import psycopg2 as pg

    conn=pg.connect(
        database = "Database",
        user = 'User',
        password= "Passward",
        host = "Host",
        port = "Port"

    )

In a nutshell :
install pyscopg2
create connection
create a cursor
execute the cursor
close the connection