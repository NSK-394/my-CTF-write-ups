# DVWA Brute Force (Easy)

## Objective
To gain unauthorized access by guessing login credentials.

## Tools Used
- DVWA
- Kali Linux
- Burp Suite (optional)

## Steps
1. Set DVWA security level to LOW.
2. Navigate to the Brute Force module.
3. Attempt login using common credentials.
4. Optionally use Burp Suite Intruder to automate attempts.

## Payloads Used
admin:password
admin:admin
admin:123456

## Result
Successful login achieved using:
Username: admin
Password: password

## Analysis
The response length for the correct password was different from others, indicating a successful login.

## Vulnerability
- No rate limiting
- No account lockout
- Weak authentication mechanism

## Mitigation
- Implement account lockout
- Use CAPTCHA
- Enforce strong password policies