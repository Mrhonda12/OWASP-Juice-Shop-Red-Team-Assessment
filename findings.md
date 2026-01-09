# Findings – OWASP Juice Shop

## Finding 1: Broken Authentication (Testing Phase)

### Description
The login functionality was tested for improper input validation using common SQL injection payloads.

### Payload Tested
' OR 1=1--

### Result
Testing is ongoing. Initial input handling behavior observed.

### Impact
If exploitable, this vulnerability could allow an attacker to bypass authentication and access user accounts without valid credentials.

### OWASP Category
OWASP Top 10 – A2: Broken Authentication

## Finding 2: Reflected Cross-Site Scripting (XSS)

### Description
The application search functionality was tested for reflected XSS vulnerabilities by injecting client-side JavaScript input.

### Payload Tested
<script>alert('XSS')</script>

### Result
[Describe exactly what happened]

### Impact
If exploitable, this vulnerability could allow attackers to execute arbitrary JavaScript in a victim’s browser, potentially leading to session hijacking or phishing attacks.

### OWASP Category
OWASP Top 10 – A7: Cross-Site Scripting (XSS)
