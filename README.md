# Database Schema Testing using SQL

## 📖 Project Overview

This project focuses on **Database Schema Testing** using SQL queries in MySQL. The objective was to validate the database schema against the expected design by executing SQL queries and documenting the results.

The testing was performed on the **customers** table, and all test cases passed successfully.

---

## 🎯 Objectives

- Verify table existence in the database.
- Validate table naming conventions.
- Check the number of columns.
- Verify column names.
- Validate column data types.
- Check column sizes.
- Verify NULL/NOT NULL constraints.
- Validate primary and key constraints.

---

## 🛠️ Tools & Technologies

- MySQL
- SQL
- MySQL Workbench
- Microsoft Excel
- Git & GitHub

---

## 📋 Test Cases

| TC ID | Test Case | Expected Result | Status |
|--------|-----------|-----------------|--------|
| TC001 | Check table presence in database schema | Table should exist | ✅ Passed |
| TC002 | Validate table naming conventions | Table name follows naming standards | ✅ Passed |
| TC003 | Verify number of columns | Table contains 13 columns | ✅ Passed |
| TC004 | Verify column names | Column names match database design | ✅ Passed |
| TC005 | Verify column data types | Data types match database design | ✅ Passed |
| TC006 | Verify column sizes | Column sizes match database design | ✅ Passed |
| TC007 | Verify NULL constraints | NULL settings match database design | ✅ Passed |
| TC008 | Verify column keys | Primary/Key constraints are correct | ✅ Passed |

---

## 📝 SQL Queries Used

### Check Table Presence

```sql
SHOW TABLES;
```

### Count Columns

```sql
SELECT COUNT(*) AS NumberOfColumns
FROM information_schema.columns
WHERE table_name = 'customers';
```

### Verify Column Names

```sql
SELECT column_name
FROM information_schema.columns
WHERE table_name = 'customers';
```

### Verify Data Types

```sql
SELECT column_name, data_type
FROM information_schema.columns
WHERE table_name = 'customers';
```

### Verify Column Sizes

```sql
SELECT column_name, column_type
FROM information_schema.columns
WHERE table_name = 'customers';
```

### Verify NULL Constraints

```sql
SELECT column_name, is_nullable
FROM information_schema.columns
WHERE table_name = 'customers';
```

### Verify Column Keys

```sql
SELECT column_name, column_key
FROM information_schema.columns
WHERE table_name = 'customers';
```

---

## 📊 Test Summary

| Metric | Result |
|--------|--------|
| Total Test Cases | 8 |
| Passed | 8 |
| Failed | 0 |
| Overall Status | ✅ Passed |

---

## 📂 Project Structure

```
Database-Schema-Testing/
│
├── README.md
├── Database_Schema_TestCases.xlsx
└── SQL_Queries.sql
```

---

## 💡 Skills Demonstrated

- Database Testing
- SQL Query Writing
- Schema Validation
- Manual Testing
- Test Case Design
- MySQL
- Information Schema Validation
- Quality Assurance (QA)

---

## 🚀 Conclusion

This project demonstrates the process of validating a database schema using SQL queries. It verifies that the database structure complies with the expected design by checking tables, columns, data types, constraints, and keys. All eight schema validation test cases were executed successfully, confirming that the **customers** table meets the specified requirements.

---

## 👤 Author

Nafeel Sarook

GitHub: https://github.com/NafeelSM
