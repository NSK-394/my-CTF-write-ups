# DVWA Command Injection (Easy)

## Objective
To execute system commands via user input.

## Tools Used
- DVWA
- Kali Linux

## Steps
1. Set DVWA security level to LOW.
2. Open Command Injection module.
3. Enter a normal IP to observe behavior.
4. Inject commands using separators.

## Payloads Used
127.0.0.1; ls
127.0.0.1 && whoami
127.0.0.1; pwd

## Result
Successfully executed system commands.
Output included:
- File listings
- Current user (www-data)

## Vulnerability
- No input validation
- Direct execution of user input