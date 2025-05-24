# 📘 DB_Labs268_271_summary

This repository contains summaries and terminal steps for AWS Labs 268 to 271, focusing on using MySQL/MariaDB from an EC2-based Command Host. These labs simulate real-world scenarios involving database setup, inspection, and conditional querying.

---

## ✅ Lab 268: Introducing MySQL and CLI Tools

- Connected to a Command Host EC2 instance via AWS Systems Manager (Session Manager).
- Switched to root and verified system setup.
- Installed MariaDB client and server.
- Logged into the MariaDB shell with:

  ```bash
  mysql -u root -p
Verified basic configuration with:
SHOW DATABASES;
✅ Lab 269: Importing and Inspecting the world Database

Checked for the presence of the world database.
world database was not pre-installed and access to RDS was not provided.
Skipped actual import due to lab constraints, but prepared system for it.
✅ Lab 270: Performing Conditional Searches in SQL

Practiced conditional queries using:
WHERE
AND
BETWEEN
LIKE
LOWER()
Aliasing with AS
Aggregation with SUM()
Example queries:
SELECT Name, Capital, Region, SurfaceArea, Population
FROM world.country
WHERE Population BETWEEN 50000000 AND 100000000;

SELECT SUM(Population) AS "Europe Population Total"
FROM world.country
WHERE Region LIKE "%Europe%";

SELECT Name, Capital, Region
FROM world.country
WHERE LOWER(Region) LIKE "%central%";
✅ Lab 271: (To Be Completed)

Placeholder for next lab steps.
🧠 Key Takeaways

MariaDB is a drop-in replacement for MySQL in most labs.
Using EC2 Command Host with Session Manager allows secure, direct access without SSH or RDS exposure.
Core SQL topics practiced: filtering, aliasing, text pattern search, and aggregations.
🗂️ Folder Structure

DB_Labs268_271_summary/
│
├── README.md
└── (add future notes or screenshots as needed)
🚀 How to Run

# From your local terminal
ssh -i your-key.pem ec2-user@<your-ec2-public-ip>

# Inside EC2
sudo su
mysql -u root -p
📅 Date

Work completed between May 22–24, 2025.