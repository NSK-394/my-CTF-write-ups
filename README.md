# CTF & Lab Write-ups

Hands-on walkthroughs from practice labs and CTF platforms. Each write-up covers the objective, the tools used, the exact steps, and **why** the vulnerability exists and how to fix it.

> All targets are intentionally vulnerable lab environments (DVWA, Hack The Box Starting Point, OverTheWire). Never test systems you don't own or have written permission to test.

## Index

| Platform | Challenge | Category | Key techniques |
|---|---|---|---|
| DVWA | [Brute Force](DVWA/brute-force.md) | Web / Auth | Credential guessing, Burp Intruder, response-length analysis |
| DVWA | [Command Injection](DVWA/command-injection.md) | Web / RCE | Shell metacharacter injection (`;`, `&&`, `\|`) |
| DVWA | [CSRF](DVWA/csrf.md) | Web | Forged state-changing requests, missing anti-CSRF tokens |
| Hack The Box | [Fawn](hackthebox/fawn.md) | Network / FTP | Nmap service scan, anonymous FTP login |
| OverTheWire | [Bandit log](https://github.com/NSK-394/bandit-learning-log) | Linux | File discovery, permissions, SSH, encodings |

## Repo layout

```
DVWA/          Damn Vulnerable Web App modules (with screenshots)
hackthebox/    Hack The Box machine write-ups
```

## Related

- [owasp-nettacker-contribution](https://github.com/NSK-394/owasp-nettacker-contribution): my merged fix in OWASP Nettacker
- [kavach-loop](https://github.com/NSK-394/kavach-loop): detect → exploit → patch → verify pipeline for a real CVE
