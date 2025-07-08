# osTicket Lab - SOC Helpdesk Simulation

This project documents the setup of a real-world style ticketing system using osTicket in a home lab environment. It simulates SOC workflows such as incident tracking, escalation, and resolution documentation.

---

## Project Objective

The goal of this lab is to replicate a functional SOC Helpdesk system that mirrors enterprise environments. This setup supports the triage, tracking, and resolution of security events in a controlled, documented, and reproducible way.

---

## Repository Contents

- Step-by-step osTicket installation on Ubuntu
- MySQL configuration for osTicket backend
- Apache HTTP/HTTPS setup
- Troubleshooting and solutions for setup issues
- Password recovery via bcrypt and SQL
- Customization notes and plugin references

---

## Build Summary

This lab was completed on a VirtualBox VM running Ubuntu. A LAMP stack (Linux, Apache, MySQL, PHP) was configured to host osTicket. The web installer was used to complete the initial configuration, and password security was enforced using bcrypt hashing via Python virtual environment.

---

## Key Issues and Solutions

- **White screen after setup**: Resolved by correcting Apache SSL site configuration.
- **Admin login failure**: Fixed by querying the MySQL database and updating the password hash using bcrypt.
- **Pip install errors**: Addressed by isolating the environment using Python's virtualenv module.

---

## Technical Stack

- Ubuntu Server (VM on VirtualBox)
- Apache2
- MySQL
- PHP
- osTicket 1.18.2
- Python 3.12 with bcrypt (for password management)

---

## Status

The osTicket system is fully operational and accessible at:

https://localhost/osticket/scp/login.php
