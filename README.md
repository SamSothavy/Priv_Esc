# Privilege Escalation  

## Objective

The main objective of this lab is to gain elevated privileges on a compromised system by identifying misconfigurations, weak permissions, or security flaws that allow escalation from a low-privileged user to root or administrator access.

## Skills Learned

- Enumerate system information for privilege escalation opportunities.
- Identify misconfigured file permissions and sudo privileges.
- Detect weak service configurations and insecure processes.
- Analyze system users, groups, and access rights.
- Apply Linux privilege escalation techniques in a controlled lab environment.
- Understand the difference between user-level and root-level access.
- Verify privilege escalation paths safely in a test environment.

## Tools Used

- Linux terminal commands
- Manual enumeration techniques
- LinPEAS

## Steps
project setup or commands go here
bash
```
https://github.com/SamSothavy/Priv_Esc_Lab
```

Next, we attempt to brute-force SSH credentials in the lab environment.

<img width="1702" height="253" alt="Screenshot 2026-07-02 154642" src="https://github.com/user-attachments/assets/33d8098f-3b5a-47fe-b664-adbfcba8b156" />

<img width="1695" height="297" alt="Screenshot 2026-07-02 154800" src="https://github.com/user-attachments/assets/49c8195d-bbfe-4e60-b72d-783f668caf67" />

We access the server through SSH.

<img width="1696" height="624" alt="Screenshot 2026-07-02 160522" src="https://github.com/user-attachments/assets/0b5f144e-489e-4246-8e47-55dd13440a0d" />

The low-privilege user has restricted access, but `/usr/bin/vim`, `/usr/bin/find`, and `/bin/bash` can be executed without a password.
 
<img width="1711" height="580" alt="Screenshot 2026-07-02 163541" src="https://github.com/user-attachments/assets/a5d9a060-c7ae-4fd5-95ec-8a88d771d9aa" />

We use **vim** to edit files related to user configuration.

<img width="1702" height="948" alt="Screenshot 2026-07-02 170618" src="https://github.com/user-attachments/assets/dbace703-caf0-4d4d-984e-784f9287e93b" />

<img width="1716" height="425" alt="Screenshot 2026-07-02 171950" src="https://github.com/user-attachments/assets/8b71d775-ab63-4a3d-ba56-190c127ea6f8" />

<img width="1708" height="946" alt="Screenshot 2026-07-02 172137" src="https://github.com/user-attachments/assets/1a0f63ca-934a-4e14-9eb6-e08cefe35145" />

<img width="1704" height="783" alt="Screenshot 2026-07-02 172426" src="https://github.com/user-attachments/assets/f2e0db6f-84e3-4f77-ac84-21022f4c0220" />
