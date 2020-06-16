## Day 1 Activity File: Red Team

Today, you will act as an offensive security Red Team to exploit a vulnerable Capstone VM (`192.168.1.105`).

You will need to use the following tools, in no particular order:
- Firefox
- Hydra
- Nmap
- Metasploit



### Instructions

Complete the following to find the flag:

- Discover the IP address of the Linux server.
![nmap](images/nmap.png)
- Locate the hidden directory on the server.
![hint1](images/hint1.png)
![secret_folder](images/secret_folder.png)
- Brute force the password for the hidden directory using the hydra command:
![xHydra](images/xHydra.png)
![hydra](images/hydra_result.png)
![secret_folder_hacked](images/secret_folder_hacked.png)
![secret_folder_hacked2](images/secret_folder_hacked2.png)
- Break the hashed password with Crackstation website.
![secret_folder](images/hash_cracked.png)

- Connect to the server via WebDAV.
![webdav](images/webdav_open.png)
![webdav_opened](images/webdav_opened.png)

- Upload a PHP reverse shell payload.
![msfvenom](images/msfvenom.png)
![drop_payload_dav](images/drop_payload_dav.png)
![msfconsole](images/msfconsole.png)
![webdav_firefox](images/webdav_firefox.png)


- Find and capture the flag.
![webdav_firefox](images/meterpreter.png)
![found_flag](images/found_flag.png)
![cat_flag](images/cat_flag.png)


After you have captured the flag, show it to your instructor.

Be sure to save important files (e.g., scan results) and take screenshots as you work through the assessment. You'll use them again when creating your presentation.

---
© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
