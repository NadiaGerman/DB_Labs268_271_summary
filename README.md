✅ Summary Structure
Here's a suggested format for your README.md:

# 📘 DB_Labs268_271_summary

This repository contains summaries and command-line steps for AWS Labs 268 to 271, focusing on MySQL/MariaDB database tasks using the Command Host EC2 instance.

---

## ✅ Lab 268: Introducing MySQL and CLI Tools

- Connected to Command Host EC2 instance via Session Manager.
- Installed and verified MariaDB.
- Logged into MariaDB shell using:
  ```bash
  mysql -u root -p
Ran basic commands:
SHOW DATABASES;
✅ Lab 269: Importing and Inspecting the World Database

Verified absence of the world database.
Installed necessary MariaDB packages.
Database import skipped due to lab constraints (RDS access unavailable).
✅ Lab 270: Performing Conditional Searches in SQL

Practiced filtering using:
WHERE
AND, BETWEEN, LIKE, LOWER()
AS (aliases)
SUM()
Sample query:
SELECT Name, Population 
FROM world.country 
WHERE Population BETWEEN 50000000 AND 100000000;
✅ Lab 271: (Next Step Placeholder)

(To be added after lab is completed)
🧠 Key Takeaways

MariaDB vs. MySQL: interchangeable for most CLI tasks.
Connecting via EC2 ensures security without direct public DB exposure.
SQL syntax learned: filtering, aliasing, aggregation.
🗂️ Folder Structure

DB_Labs268_271_summary/
│
├── README.md
└── (any additional notes or screenshots if added)
🚀 How to Run

Connect to EC2:
ssh -i your-key.pem ec2-user@your-ec2-public-ip
Launch MariaDB:
sudo mysql -u root -p
📅 Date

Work completed between May 22–24, 2025