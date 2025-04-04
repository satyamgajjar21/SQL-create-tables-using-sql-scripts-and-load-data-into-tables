# 🧪 Hands-on Lab: Create Tables using SQL Scripts and Load Data into Tables

**🕒 Estimated time needed: 30 minutes**

---

## 🧰 Software Used in this Lab

In this lab, you will use **IBM Db2 Database**, a Relational Database Management System (RDBMS) from IBM designed to store, analyze, and retrieve data efficiently.

To complete this lab, you will utilize a Db2 database service on IBM Cloud.

**Note:** If you haven't completed the previous lab where you sign up for IBM Cloud and create the Db2 service instance, make sure to do that first.

---

## 🗃️ Database Used in this Lab

The sample HR database schema used in this lab consists of **5 tables**:

- **EMPLOYEES**
- **JOB_HISTORY**
- **JOBS**
- **DEPARTMENTS**
- **LOCATIONS**

Each table contains a few rows of sample data.

---

## 🎯 Objectives

After completing this lab, you will be able to:

- **Create tables using SQL scripts**
- **Load data into tables from .CSV files**

> ⚠️ Make sure that you are using the CSV file and datasets from the same instruction file.

---

## 🧩 Exercise 1: Create Tables Using SQL Scripts

Instead of creating each table manually, you’ll run a SQL script with multiple `CREATE TABLE` commands.

### ✅ Steps

1. **Download** the file: `HR_Database_Create_Tables_Script.sql`
2. **Login** to IBM Cloud and go to the **Resource List**.
3. Locate your **Db2 service** under **Services** and click **Go to UI**.
4. Click on **SQL** > ➕ icon > **From File**.
5. Open the script file `HR_Database_Create_Tables_Script.sql`.
6. Click **Run All** to execute all table creation statements.
7. View the **Result** section on the right side to check for errors or successful execution.
8. Click on the **Data** icon and then the **Tables** tab.
9. Select your **Schema** (usually your Db2 userid).
10. You should see the following tables:
   - **DEPARTMENTS**
   - **EMPLOYEES**
   - **JOBS**
   - **JOB_HISTORY**
   - **LOCATIONS**
11. Click on any table name to view its **Table Definition**.

> 💡 **Note:** Some errors may appear related to dropping pre-existing tables. You can **ignore** those.

---

## 📥 Exercise 2: Load Data into Tables

Instead of inserting data row by row, you’ll upload data using `.csv` files.

### ✅ Files to Download

Download the following **CSV** or **TXT** files:

#### CSV Files:

- `Departments.csv`
- `Employees.csv`
- `Jobs.csv`
- `Locations.csv`
- `JobsHistory.csv`

#### TXT Files (for Firefox issues):

- `Departments.txt`
- `Employees.txt`
- `Jobs.txt`
- `Locations.txt`
- `JobsHistory.txt`

---

### ✅ Steps to Load `Employees.csv`:

1. In the Db2 Console, click on the **☰ menu icon** > **Load** > **Load Data**.
2. Ensure **My Computer** is selected and click **Browse Files**.
3. Select `Employees.csv` and click **Open**.
4. Click **Next** (bottom right corner).
5. Choose your **Schema** and select the **EMPLOYEES** table.
6. In the Table Definition tab, choose **Overwrite table with new data**.
7. Turn off **Header in first row** (since the CSV has no column labels).
8. Click **Next** and then **Begin Load**.
9. After the load completes, check for success or any errors/warnings.
10. Click **Tables** > select **EMPLOYEES** > click **View Data** to see the table contents.

---

### 📥 Load Remaining Tables

Repeat the above steps to load the following tables:

- **LOCATIONS**
- **JOB_HISTORY**
- **JOBS**
- **DEPARTMENTS**

> 🔁 Use the "Load More Data" option and repeat from Step 3 for each table.

---

## 🎉 Congratulations!

You’ve successfully created all tables and loaded sample data into them. You're now ready to move on to the next topic.

---

## 👩‍💻 Authors

- **Rav Ahuja**
- **Sandip Saha Joy**
