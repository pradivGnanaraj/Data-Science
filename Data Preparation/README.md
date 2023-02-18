# Mac Users 

## Virtualization tool : Docker 
Purpose : Install and use SQL server

(base) pradivgnanaraj@Pradivs-MacBook-Air ~ % docker pull mcr.microsoft.com/mssql/server:2019-latest

(base) pradivgnanaraj@Pradivs-MacBook-Air ~ % docker run --name SQLServer -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=12345OHdf%e' -e 'MSSQL_PID=Express' -p 1433:1433 -d mcr.microsoft.com/mssql/server:2019-latest

WARNING: The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested
63658ec3c58315a855eaafe03bb922eaaaadf5.....

https://github.com/google/cadvisor/issues/2763

2023-02-18 13:15:43 /opt/mssql/bin/permissions_check.sh: line 4: [: : integer expression expected
2023-02-18 13:15:43 /opt/mssql/bin/permissions_check.sh: line 59: [: : integer expression expected
2023-02-18 13:15:43 /opt/mssql/bin/sqlservr: Invalid mapping of address 0x4003917000 in reserved address space below 0x400000000000. Possible causes:
2023-02-18 13:15:43 1) the process (itself, or via a wrapper) starts-up its own running environment sets the stack size limit to unlimited via syscall setrlimit(2);
2023-02-18 13:15:43 2) the process (itself, or via a wrapper) adjusts its own execution domain and flag the system its legacy personality via syscall personality(2);
2023-02-18 13:15:43 3) sysadmin deliberately sets the system to run on legacy VA layout mode by adjusting a sysctl knob vm.legacy_va_layout.
2023-02-18 13:15:43 
2023-02-18 13:15:43 SQL Server 2022 will run as non-root by default.
2023-02-18 13:15:43 This container is running as user mssql.
2023-02-18 13:15:43 To learn more visit https://go.microsoft.com/fwlink/?linkid=2099216.

Azure Data Studio is used instead of SQL Server Management Studio 

# Windows/Unix Users

SQL server express *.exe file works well.
