# Send-CLOC-Report
## Objective
Scan a specified GitHub source repository with CLOC and send the output to a specified email address.

## Implementation
The Send CLOC (count lines of code) Report script works by first prompting the user for a sender email address and password. These account credentials will be used to login into the Gmail email service and send the CLOC report to a specified email address. 
The user is then prompted for a receiver email address for where to the send the CLOC report, the url of a Github repository, and a specified branch within the repository to scan.
The repository is processed with CLOC and the output is placed into a CSV file. This CSV file is sent as an attachment from the sender email address to the specified receiver email address.

## Requirements
 Python 3.7.4 or later
  - An interpreted high-level general-purpose programming language
  - Python 3 installation and documentation: https://www.python.org/downloads/
  - Python executable must be on system PATH
  
 Pip 20.0.1 or later
  - Package management system used to install and manage software packages/libraries written in Python.
  - Pip installation and documentation: https://pip.pypa.io/en/stable/installation/
  
 GitPython 3.1.10 or later 
  - A python library used to interact with Git repositories
  - GitPython installation and documentation: https://gitpython.readthedocs.io/en/stable/

Email Credentials
  - Sender: Gmail account credentials (email address and password)
  - Receiver: Any email service credentials (email address only)

## Usage
```
C:\Users\Sonali> python send_cloc_report.py
---Enter sender credentials---
Enter email: sender@gmail.com
 sender@gmail.com is not a valid email address. _*Output for invalid email address*_
Enter email: sender@gmail.com
Enter email password: 

---Enter receiver credentials---
Enter email: receiver@gmail.com

---Enter url of repository---
Enter url: https://github.com/AlDanial/cloc.git

---Enter branch name within repository---
Enter branch: master
```

