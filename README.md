# MS-SQL-Server-
MS-SQL Server Installation and Tools


How to install MS-SQL
# First method 
1.	Install  SQL Server Developer 2019
https://www.microsoft.com/en-us/sql-server/sql-server-downloads
*	Download the Developer edition (SQL2019-SSEI-Dev.exe)
*	Execute the SQL2019-SSEI-Dev.exe, choose Download Media at a specified location
*	Use ISO packaging, mount and install
*	After checking your computer, make full installation, select all options, and proceed using default settings
*	Add current user in all cases
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
2.	SQL Server Management Studio or Azure Data Studio
Download SQL Server Management Studio (SSMS) from the link below
https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15

or Download Azure Data Studio from the link below
https://docs.microsoft.com/en-us/sql/azure-data-studio/download-azure-data-studio?view=sql-server-ver15
