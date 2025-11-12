# LAB 1 – Azure SQL Database Overview (AZ-305)

## 🎯 Objective
Understand what Azure SQL Database is and explore its basic configuration options.

---

## 🧠 Concept
Azure SQL Database is a **fully managed PaaS** (Platform as a Service) database that provides:
- Automatic backups
- High availability
- Scalability
- Built-in security

---

## ⚙️ Steps

### Step 1: Login to Azure Portal
- Open: [https://portal.azure.com](https://portal.azure.com)

### Step 2: Create SQL Database
1. Click **Create a Resource → Databases → SQL Database**
2. Click **Create**
3. Fill in the details:
   - **Resource Group:** `rg-az305-lab1`
   - **Database Name:** `az305db-overview`
   - **Server:** Click *Create new*
     - Name: `az305sqlserver-overview`
     - Admin Login: `sqladmin`
     - Password: `P@ssword12345`
     - Location: Central India
   - **Compute + Storage:** Select *Basic* tier

4. Click **Review + Create → Create**

### Step 3: Explore SQL Database
Once deployed:
- Go to **Resource → Overview**
- Observe:
  - Server name
  - Connection string
  - Pricing tier
  - Query editor option

---

## 🧩 Output
✅ Azure SQL Database created successfully.

---

## ✅ Check Yourself
1. What is the difference between SQL Database and SQL Server?
2. Where can you find the connection string?
3. What is the default port used for Azure SQL?

---
