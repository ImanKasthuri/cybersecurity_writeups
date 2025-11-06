# Active Directory Delegation Lab

## A short lab to manage OUs and delegation control in Active Directory.

### Steps
- Added new Organizational Unit (OU) name Students under the THM domain.
- Disabled unnecssary user accounts from sales OU instead of deleting them, to preserve their data and permissions.
- Delegated passwords reset rights for the sales OU to Phillip User.
- Logged in as Phillip and used powershell to reset user Sophie's password.

### Commands used to rest password
- Set-ADAccountPassword sophie -Reset -NewPassword (Read-Host -AsSecureString -Prompt 'New Password') -Verbose
- Set-ADUser -ChangePasswordAtLogon $true -Identity sophie

### Lesson learned
- It's better to disable old accounts instead of deleting them.
- Delegation let you give limited permission without making someone an admin.
- can use powershell to manage user quickly as example resetting passwords.
- always test the changes by loggin in as the user.

  <img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/managing_users/screenshots/Screenshot%201.png?raw=true">

<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/managing_users/screenshots/Screenshot%202.png?raw=true">

<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/managing_users/screenshots/Screenshot%203.png?raw=true">

<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/managing_users/screenshots/Screenshot%204.png?raw=true">

<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/managing_users/screenshots/Screenshot%205.png?raw=true">

<img src="https://github.com/ImanKasthuri/tryhackme-cybersecurity-101/blob/main/active_directory_lab/managing_users/screenshots/Screenshot%206.png?raw=true">
    

        
