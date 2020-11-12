# PortFolioManagementSystem
A Web Application built on ASP.NET Core that allows users to check their networth and sell their assets. The application is built on the microservice architecture.

SOFTWARE REQUIEREMENTS :

* VISUAL STUDIO 2019
* MICROSOFT SQL SERVER MANAGEMENT STUDIO 18
* WEB BROWSER

STEPS TO EXECUTE:- 
1.  All the 4 APIs are hosted on Azure Cloud. Their respective IP Address are also provided.
  * DailySharePrice - http://52.146.55.16/api/stock/
  * MutualFundNAV - http://52.224.199.83/api/MutualFundNAV/
  * CalculateNetWorth - http://52.224.136.125/api/NetWorth/
  * Authorization - http://20.62.155.216/api/Auth
2.  Open the Customer Portal Soution and Change the connection string as per your SQL Server Management Configuration in appsetting.json file.
3.  Go to the NuGet Package Console and write "Add-Migration "initial migration" " command.
4.  Now Write "Update Database" command.
5.  Now run the Customer Portal. You will be taken to a page with URL - http://localhost:44327/Home/Login
6.  You can enter into the application by entering the correct PortfolioID and Password.
7.  Once you have entered the correct credentials you will be redirected to the Dashboard which contains the Net Worth as well as the list of Stocks and Mutual Funds.
8.  User also have the option to sell the stocks and mutual funds. If the Quantity he wants to sell is greater than the quantity he has then we will get a negative sale response Page.
9.  The application also logs the Sale Status along with the new calcuated net Worth and Portfolio ID into the Database.
