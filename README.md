# MS-SQL-Server-
MS-SQL Server Installation and Tools


How to install MS-SQL
# First method 
1.	Install  SQL Server Developer 2019
https://www.microsoft.com/en-us/sql-server/sql-server-downloads
*	Download the Express edition (SQL2019-SSEI-Expr.exe)
*	Run the file SQL2019-SSEI-Expr.exe
*	Select the Basic edition, accept the license agreement
*	After checking your computer, make full installation, select all options, and proceed using default settings
*	If asked, add current user in all cases
*	Choose mixed mode authentication using the password Password: passw0rd


2.	Install  SQL Server Management Studio, SSMS 
Download SQL Server Management Studio (SSMS) from the link below
https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15

 
# Second method (using Docker)
1.	SQL Server (Docker image)
*	First install Docker and cmder from the links
https://docs.docker.com/docker-for-windows/install/
https://cmder.net/
*	Open cmder and run the following command:

```bash
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=admin!@#123" -p 1433:1433 --name sql1 -d mcr.microsoft.com/mssql/server:2019-CU3-ubuntu-18.04
```

*	A new SQL Server instance will be created, and you can access it using SQL Server Management Studio by using:
Server name: localhost
Authentication: SQL Server authentication
Username: sa
Password: admin!@#123


# Demo databases

Demo databases can be downloaded from 
https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms.
Download the files _AdventureWorks2017.bak_ and _AdventureWorksDW2012.bak_. Do not install these files, just keep them in an accessible location. These two files will be used during the course.
