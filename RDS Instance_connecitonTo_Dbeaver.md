# RDS Instance in AWS
## AWS RDS (Relational Database Service) 
- is a managed service for relational databases, but it doesn't offer a "full environment" for running SQL queries in the same way Google Cloud's BigQuery does.

-   **SQL Execution:** You would need a client (e.g., MySQL Workbench, pgAdmin, DBeaver, etc.) or a programming language (e.g., Python, Node.js) to connect to your RDS instance and run SQL queries. It's more about accessing a database that you can use as a backend.
-  **Use case:** RDS is for applications that need transactional data, relational schema, and structured data with consistent SQL support. It's not designed for ad-hoc querying or analytics at scale (BigQuery excels here).

## 1. Navigate to RDS and click on Create a database 
 <img width="975" height="554" alt="image" src="https://github.com/user-attachments/assets/4c87b5b7-24d3-4ab5-9a27-55d91f8b587b" />

## 2. Select the Engine type and the dialect 
 <img width="1586" height="956" alt="image" src="https://github.com/user-attachments/assets/c5250365-e284-49cd-a8be-278f2f64dfb7" />

## a. Enable Public Access: 
 <img width="975" height="525" alt="image" src="https://github.com/user-attachments/assets/944408e8-9ba1-4726-ae28-d17adc3de7fe" />


## 3. Connecting Dbeaver to RDS instance (SQL Server)
## a. Open Dbeaver and select the database type 
 <img width="975" height="693" alt="image" src="https://github.com/user-attachments/assets/eea46a38-c46c-4203-93e9-a4e11d7c0196" />

## b. Enter the Connection Details:

After selecting SQL Server, you'll need to enter the connection details:
- **Host:** Enter your RDS endpoint (you can find this in the RDS console under your instance details, it will look something like mydbinstance.xxxxxx.us-east-1.rds.amazonaws.com).
-	**Port:** The default port for SQL Server is 1433, but if your RDS is configured to use a custom port, enter that.
-	**Database:** Enter the name of the database you want to connect to, or leave it blank if you want to connect to the default database.
-	**Authentication:**
>   - 	Username: Enter your master username (e.g., admin).
>  -	Password: Enter the master password you set when creating the RDS instance.
 <img width="975" height="641" alt="image" src="https://github.com/user-attachments/assets/8738a9d0-fa4f-44d7-b5ac-c21e623f1616" />

## 4. If seeing a Connection timeout error
 <img width="739" height="744" alt="image" src="https://github.com/user-attachments/assets/44b4e1aa-1ded-4775-a857-449a5d29d8fe" />

## a. Go to the security group of your instance 
 <img width="975" height="430" alt="image" src="https://github.com/user-attachments/assets/5421c2f9-602d-4ea8-9f9e-bf20609c9594" />

## b. To the security group (default in this case)add an Inbound rule with your IP address and the port of your connection. 

	<img width="975" height="270" alt="image" src="https://github.com/user-attachments/assets/f84264f3-5aaa-4823-98b4-b241ff9e622c" />

## 5. The connection is established. Can create datasets, tables, and data. 
<img width="807" height="710" alt="image" src="https://github.com/user-attachments/assets/ed1c8f66-78de-46d8-970a-f3631c1dce30" />



 
5. The connection is established. Can create datasets, tables, and data. 

 
