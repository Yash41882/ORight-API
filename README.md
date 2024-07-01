# ORight-API

This Project Takes an excel file and store its data in table, Table Schema is simple
Id - INT AutoIncrement (PK)
CliendId - INT NOT NULL
FAT - DECIMAL NOT NULL
SNF - DECIMAL NOT NULL
RATE - DECIMAL NOT NULL
Send client ID and FILE through POSTMAN while storing data.

URL FOR 1st API to store data in DB-
POST http://localhost:5000/api/upload?clientId=3

URL FOR 2nd API to fetch the stored data in DB-
http://localhost:5000/api/getPrice?clientId=1&snf=10.2&fat=11.1

For Brownie points:
In rateChartRepository.cs - Instead of writing records in DB for each record record. Send them in batched or store them in a Data Structure and Write at the end of Process, this will reduce the time significantly for POST Call.
And For GET CALL set up indexing in DB over ClientID, Fat and SNF for faster retrival.
