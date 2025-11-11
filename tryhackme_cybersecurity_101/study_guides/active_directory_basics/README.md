# 🛡️ Active Directory (AD) Fundamentals Study Guide

This guide covers the core concepts of Active Directory Domain Services (AD DS), the central authority for managing users, computers, and security across a Windows network.

---

## 1. Core Active Directory Concepts

* **Domain Controller (DC):** This is the main server that manages all computers and users in a company or school network.
* **Active Directory (AD):** The big, central database running on the DC. It stores and controls all:
    * User accounts (usernames and passwords).
    * Computers on the network.
    * Security rules and settings.
* **AD Objects:** Every item stored in the AD database is called an Object (Users, Computers, Printers, Shared Folders).
* **Organizational Units (OUs):** Objects are grouped into these containers for easier management (e.g., Sales, Marketing, IT).
* **Machine Accounts:** These accounts represent computers. They are distinguished by a dollar sign at the end (e.g., `TOM-PC$`).

---

## 2. AD Management and Policy

* **Delegation:** The process of granting specific, limited control over an OU or object to another user (e.g., allowing an IT Support user to reset passwords).
* **Group Policy (GP) Update:** Changes to AD Group Policies usually take up to two hours to apply.
    * **Force Update:** Use the command **`gpupdate /force`** on a client machine to apply policy changes immediately.

---

## 3. Essential Management Commands (PowerShell)

These commands are used by administrators to manage user accounts and security settings.

* **Resetting User Passwords (Delegated):**
    * The **`Set-ADAccountPassword`** cmdlet is used by privileged users to reset lower-privilege user passwords.
    * *Example:* `Set-ADAccountPassword sophie -Reset -NewPassword (Read-Host -AsSecureString -Prompt 'New Password')`

* **Forcing User Password Change:**
    * The **`Set-ADUser`** cmdlet can force a user to reset their own password at the next login for security.
    * *Example:* `Set-ADUser -ChangePasswordAtLogon $true -Identity sophie`

---

## 4. Remote Access

* **Remmina:** A command-line tool used on **Linux** systems to connect to remote desktop services, including those running on Windows domain controllers.
