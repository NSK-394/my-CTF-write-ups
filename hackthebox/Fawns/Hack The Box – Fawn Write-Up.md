Hack The Box – Fawn Write-Up
Objective: Gain access and retrieve the flag

1. I began by scanning the target machine using Nmap:

nmap -sV 10.129.18.155

The scan revealed that Port 21 (FTP) was open and running vsFTPd 3.0.3.

2. FTP Access

I attempted to connect to the FTP service:

ftp 10.129.18.155

Because many misconfigured FTP servers allow anonymous access, I tried logging in with:

Username: anonymous
Password: anonymous

The login was successful, confirming that anonymous authentication was enabled.

3. Flag Retrieval

After gaining access, I listed available files:

ls
I discovered a file containing the flag. I downloaded it using:
get flag.txt

Then viewed the contents locally:

cat flag.txt

This revealed the flag.