# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:


## OUTPUT:

![image](https://github.com/user-attachments/assets/97fb9560-c5bd-4daa-86be-9e67c04719a7)

POSTGRESQL msfdb :

![image](https://github.com/user-attachments/assets/95d538b4-5d92-49a1-8b78-aacb642a4c85)

## OUTPUT:

![image](https://github.com/user-attachments/assets/bdf3ba11-b267-4473-9d88-64b8b7d7444a)
Invoke msfconsole:

## OUTPUT:
![image](https://github.com/user-attachments/assets/b18346c4-fcac-48e9-9ee2-85538f157a85)

## OUTPUT:

![image](https://github.com/user-attachments/assets/a9447441-5b39-4c7b-9ede-b3135d7c2cd1)

Port Scanning:
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000). msf > nmap -sT 192.168.1810/24 -p1-1000

## OUTPUT:
![image](https://github.com/user-attachments/assets/7b2268c7-06ed-4d2e-b226-26121d8f2f53)

Step4:
use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later. scan the targets with the command db_nmap as follows. msf > db_nmap 192.168.181.0/24
## OUTPUT :

![image](https://github.com/user-attachments/assets/0c90a62f-89fc-49f7-8a42-cd8754de74dd)

## OUTPUT:

![image](https://github.com/user-attachments/assets/7f7b87b6-68a0-4787-8534-f39e9388b1e2)
## OUTPUT:
![image](https://github.com/user-attachments/assets/3bf2f8ee-6932-4ee8-a6a7-a3d9e63bb0a8)

## OUTPUT:
![image](https://github.com/user-attachments/assets/447762a0-977e-4424-a50a-bf27e1c5d6cf)
Before beginning, set up the Metasploit database by starting the PostgreSQL server and initialize msfconsole database as follows: systemctl start postgresql msfdb init
MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port. db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

## OUTPUT:
![image](https://github.com/user-attachments/assets/1123f937-5147-4941-a5e5-b6883fd2cea9)

## OUTPUT:
![image](https://github.com/user-attachments/assets/d550b36d-ab34-4289-b538-99f7351ee04e)

## OUTPUT:
![image](https://github.com/user-attachments/assets/70f2709f-2ebd-470b-87fb-ffcaa0fc81b0)

## OUTPUT:
![image](https://github.com/user-attachments/assets/640276d7-0c3c-4e5f-9671-79cfb8a5d862)

## OUTPUT:
![image](https://github.com/user-attachments/assets/9befe623-9588-4ddc-8d4c-ee9b420ff9cc)
set the PASS_FILE parameter to the wordlist path available inside /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt Then, specify the IP address of the target machine with the RHOSTS command. set RHOSTS Set BLANK_PASSWORDS to true in case there is no password set for the root account. set BLANK_PASSWORDS true

## OUTPUT: 
![image](https://github.com/user-attachments/assets/cc6c25a1-e523-4f19-b94a-804917f194a6)

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
