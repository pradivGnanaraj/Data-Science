# Mac Users 

## Virtualization tool : Docker 
Purpose : Install and use SQL server

(base) pradivgnanaraj@Pradivs-MacBook-Air ~ % docker pull mcr.microsoft.com/mssql/server:2019-latest
(base) pradivgnanaraj@Pradivs-MacBook-Air ~ % docker run --name SQLServer -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=12345OHdf%e' -e 'MSSQL_PID=Express' -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-latest

WARNING: The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested
63658ec3c58315a855eaafe03bb922eaaaadf5.....


Azure Data Studio is used instead of SQL Server Management Studio 

# Windows/Unix Users

SQL server express *.exe file works well.
