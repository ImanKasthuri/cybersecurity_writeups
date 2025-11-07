# Group Policy Lab

## Learn how to use Group Policy to control settings for users and computers.

### What I did
- Created two separate Organizational Units for Workstations and Servers.
- Moved all laptops and computers to the Workstations OU.
- Moved all servers to the Servers OU.
- Tried to change the password — confirmed that the new password must be at least 10 characters long (Password policy from default domain policy)
- Created another GPO called Restrict Control Panel Access to block non-IT users from opening the Control Panel (Management, Marketing & Sales OU).
- Created a new Group Policy called Auto Lock Screen to lock computers after 5 minutes.(Set to all Computers).
- Used gpupdate /force command on poweshell to activate the Auto Lock Screen. 
- Logged in remotely using Remote Desktop (RDP) windows machine with a normal user account.
- The Auto Lock Screen Policy worked, the computer locked automatically.
- Tried to access the control panel as a normal user made sure that normal users cannot open it.

Screenshots Below

  <img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/group_policy_management/screenshots/Screenshot%201.png?raw=true">

  <img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/group_policy_management/screenshots/Screenshot%202.png?raw=true">

  <img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/group_policy_management/screenshots/Screenshot%203.png?raw=true">
 
<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/group_policy_management/screenshots/Screenshot%204.png?raw=true">

<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/group_policy_management/screenshots/Screenshot%205.png?raw=true">

  

