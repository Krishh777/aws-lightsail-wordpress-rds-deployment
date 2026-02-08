# AWS Lightsail WordPress Deployment with RDS

## Overview
This project demonstrates deploying a WordPress application on AWS Lightsail and integrating it with AWS RDS (MySQL) as the backend database. The setup separates the application layer and database layer, following basic cloud architecture best practices.

## Tech Stack
- AWS Lightsail (Linux/Unix)
- WordPress
- AWS RDS (MySQL)
- Apache Web Server
- PHP
- MariaDB/MySQL client

## Architecture
User requests are handled by a WordPress application hosted on an AWS Lightsail instance. The WordPress application communicates with an AWS RDS MySQL database for data storage and authentication.

User → Lightsail (WordPress) → AWS RDS (MySQL)

## Steps Performed
1. Created an AWS Lightsail instance using the WordPress blueprint
2. Accessed WordPress via public IP and configured admin access
3. Created an AWS RDS MySQL database
4. Configured RDS security group to allow MySQL access (port 3306) from Lightsail
5. Updated WordPress configuration (`wp-config.php`) to connect to RDS
6. Created WordPress database inside RDS
7. Verified deployment via WordPress installation and dashboard access

## Security Considerations
- Database access restricted using security groups
- MySQL port (3306) allowed only from Lightsail public IP
- AWS-managed RDS service used for better reliability and security

## Outcome
The WordPress application was successfully deployed on AWS Lightsail and integrated with AWS RDS. The setup was verified through successful WordPress installation and admin dashboard access.

## Author
Krish Bagga  
