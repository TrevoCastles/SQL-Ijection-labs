# 🧪 Portswigger-Labs-Writeups

# 🎯 What we will learn in this report
 ## 💻 Why you must learn SQL first
- The Foundation: Understanding how databases communicate is the key to breaking them
- Query Logic: You need to know the original query structure to inject your own code effectively
## 📋  Bypassing the Login Page
- Authentication Bypass: Using SQL logic to login without a valid username or password.
- The OR logic: Exploiting the ' OR 1=1 -- payload to force a "True" response from the server.
## 📊 UNION-Based SQL Injection
- Data Leakage: Using UNION SELECT to retrieve sensitive data from other tables.
- Combining Results: How to merge the original query results with our malicious output.
## 🔍 Enumerating Columns & Datatypes
- Column Counting: Using ORDER BY to find how many columns the query returns.
- Finding Strings: Identifying which columns can hold and display text data.
## 🌿 Fingerprinting Database Versions
- Syntax Variety: Different payloads for MySQL, Oracle, and PostgreSQL.
- Database Identity: How to ask the server "Who are you?" using specific SQL functions.
## 👀 Blind SQL Injection
- No Visual Output: Exploiting vulnerabilities when the page doesn't show any data.
- Blind SQL Error: Using database errors to confirm if our logic is correct.
## 💡 Data Exfiltration Without Prior Knowledge
- System Tables: Querying the information_schema to find table and column names.
- Mapping the DB: Reconstructing the database structure from scratch.

> [!WARNING]
> ## ⚠️ Disclaimer: All information in this report is for educational purposes only. I am practicing these labs in a controlled environment [PortSwigger Academy](https://portswigger.net/). to improve my security knowledge.

> [!important]
> - OS: Kali Linux / Windows
> - Proxy: Burp Suite Professional / Community
> - Browser: Firefox with FoxyProxy / Browser Burpsuite

# labs 
## Lab 1 : SQL injection vulnerability in WHERE clause allowing retrieval of hidden data [Lab-1](SQL-Ijection-labs/blob/main/Report-lab1/lab-1.md)
