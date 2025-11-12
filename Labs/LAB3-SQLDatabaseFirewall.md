# LAB 3 – Provision Azure SQL Database & Configure Firewall (AZ-305)

## 🎯 Objective
Create an Azure SQL Database, configure firewall rules, and run queries.

---

## ⚙️ Steps

### Step 1: Create SQL Database
1. In Azure Portal → **Create a resource → SQL Database**
2. Configure:
   - **Resource Group:** `rg-az305-lab3`
   - **Database Name:** `az305db-firewall`
   - **Server:** 
     - Name: `az305sqlfw`
     - Admin Login: `sqladmin`
     - Password: `P@ssword12345`
     - Location: Central India
   - **Pricing Tier:** *Basic*
3. Click **Review + Create → Create**

---

### Step 2: Configure Firewall
1. After deployment → Go to your SQL Database
2. Click **Server name** under *Overview*
3. Go to **Networking / Firewalls and virtual networks**
4. Click **+ Add client IP**
5. Click **Save**

✅ This allows your current computer to connect via port **1433**.

---

### Step 3: Run SQL Queries
1. Open **Query Editor (Preview)** in Azure Portal
2. Login with your admin credentials
3. Run:

```sql
CREATE TABLE Departments (
  DeptID INT PRIMARY KEY,
  DeptName NVARCHAR(50)
);

INSERT INTO Departments VALUES
(1, 'Sales'),
(2, 'Engineering'),
(3, 'Finance');

SELECT * FROM Departments;
