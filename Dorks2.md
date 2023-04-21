 
# FTP PASSWORD GOOGLE DORKS
 
1.) ws_ftp.ini configuration file search:
 
intitle:index.of ws_ftp.ini
 
2.) ws_ftp.ini configuration file with “Parent Directory” search:
 
filetype:ini ws_ftp pwd
 
3.) Variation:
 
”index of/” “ws_ftp.ini” “parent directory”
 
4.) Variation:
 
+htpasswd +WS_FTP.LOG filetype:log
 
5.) Variation:
 
(Substitute vulnerablesite.com with your site you want to search)
”allinurl: “Vulnerablesite.com” WS_FTP.LOG filetype:log”

 # XSS GOOGLE DORKS
 
1.) cart32 executable file.
 
allinurl:/scripts/cart32.exe
 
2.) Cute news php file.
 
allinurl:/CuteNews/show_archives.php
 
3.) phpinfo.php file.
 
allinurl:/phpinfo.php
 
# PHP GOOGLE DORKS
 
1.) config.php file search:
 
intitle:index.of config.php
 
2.) PHP file contents search:
 
intitle:”Index of” phpinfo.php
 
3.) download.php directory transversal vulneralbilities:
 
inurl:download.php?=filename
 
4.) upload.php search:
 
intitle:index.of upload.php
 
inurl:upload.php
 
# SQL PASSWORD DUMP DORKS
 
1.) SQL dumps saved to database search. (Some of the more common passwords for you):
 
a.) ”123456″ = hashed password
ext:sql intext:@gmail.com intext:e10adc3949ba59abbe56e057f20f883e
 
b.) ”654321″ = hashed password
ext:sql intext:@gmail.com intext:c33367701511b4f6020ec61ded352059
 
c.) ”password” = hashed password
ext:sql intext:@gmail.com intext:5f4dcc3b5aa765d61d8327deb882cf99
 
d.) ”12345678″ = hashed password
ext:sql intext:@gmail.com intext:25d55ad283aa400af464c76d713c07ad
 
e.) ”iloveyou” = hashed password
ext:sql intext:@gmail.com intext:f25a2fc72690b780b2a14e140ef6a9e0
 
2.) Variation of above search:
 
a.) ext:sql intext:”INSERT INTO” intext:@gmail.com intext:password
 
b.) ext:sql intext:”INSERT INTO” intext:@yahoo.com intext:password
 
c.) ext:sql intext:”INSERT INTO” intext:@hotmail.com intext:password
 
d.) ext:sql intext:”INSERT INTO” intext:@att.net intext:password
 
e.) ext:sql intext:”INSERT INTO” intext:@comcast.net intext:password
 
f.) ext:sql intext:”INSERT INTO” intext:@verizon.net intext:password
 
3.) SQLi
 
allinurl:/privmsg.php
 
# WORDPRESS GOOGLE DORKS
 
1.) Asset Manager Plugin Exploit – Unprotected Remote File Upload Vuleralbility.
 
inurl:Editor/assetmanager/assetmanager.asp
 
2.) Timthumb Plugin Exploit – Attacker can attach a shell to a image file and upload the shell. (It has been patched, but there are still a lot of webmasters who have NOT updated!)
 
inurl:index.of thumb.php
 
inurl:thumb.php
 
3.) Search for plugins directory:
 
inurl:wp-content/plugins/
 
4.) Search for themes directory:
 
inurl:wp-content/themes/
 
# PASSWORD FILE GOOGLE DORKS
 
1.) Search for Microsoft Excel data file:
 
”Login: *” “password =*” filetype: xls
 
2.) Search for auth_user_file:
 
allinurl: auth_user_file.txt
 
3.) Search for username/password saved in Microsoft Excel files:
 
filetype: xls inurl: “password.xls”
 
4.) Search for login pages:
 
intitle: login password
 
5.) Search for “master password” page:
 
intitle: “Index of” master.passwd
 
6.) Search for backup directory:
 
index of /backup
 
7.) Search for password backup file index:
 
intitle:index.of passwd.bak
 
8.) Search for password databases:
 
intitle:index.of pwd.db
 
intitle:”index of” pwd.db
 
9.) Search for /etc/passwd/ index:
 
intitle:”index of .. etc” passwd
 
10.) Search for plaintext password file:
 
index.of passlist.txt
 
inurl:passlist.txt
 
11.) Search for hidden documents/password files:
 
index.of.secret
 
index.of.private
 
12.) Search for PhpMyAdmin files:
 
”# PhpMyAdmin MySQL-Dump” filetype: txt
 
13.) Hidden Superuser (root) data files:
 
inurl:ipsec.secrets-history-bugs
 
inurl:ipsec.secrets “holds shared secrets”
 
14.) Find the information files:
 
inurl:ipsec.conf-intitle:manpage
 
15.) Search for a stored password in a database:
 
filetype:ldb admin
 
16.) Search for admin.php file:
 
inurl:search/admin.php
 
17.) Search for password log files:
 
inurl:password.log filetype:log
 
18.) Search for Hkey_Current_User in registry files:
 
filetype: reg HKEY_CURRENT_USER username
 
19.) Search for username/password file backups:
 
”Http://username: password @ www …” filetype: bak inurl: “htaccess | passwd | shadow | ht users”
 
20.) Search for username/password files:
 
filetype:mdb inurl:”account|users|admin|administrators|passwd|password” mdb files
 
21.) Search for Microsoft Frontpage passwords:
 
ext:pwd inurl:(service|authors|administrators|users) “# -FrontPage-”
 
22.) Search for SQL database Code and passwords:
 
filetype: sql ( “passwd values ****” |” password values ****” | “pass values ****”)
 
23.) Search for e-mail account files:
 
intitle: “Index Of”-inurl: maillog
 
# MISC. DORKS
 
1.) WebWiz Rich Text Editor (RTE) – Remote file upload vulneralbility:
 
inurl:rte/my_documents/my_files
 
2.) EZFilemanager – Remote file upload vulneralbility:
 
inurl:ezfilemanager/ezfilemanager.php
 
3.) robots.txt – See directories hidden from crawlers. Also sometimes you can pull off a directory transversal with this:
 
inurl:robots.txt
 
4.) Serial Numbers – Look for software serial numbers
 
”software name” 94FBR
 
# FIND FREE SWAG
 
1.) site:*.com intitle:”Thank You For Your Order” intext:Click Here to Download
 
2.) site:*.net intitle:”Thank You For Your Order” intext:Click Here to Download
 
3.) site:*.co intitle:”Thank You For Your Order” intext:Click Here to Download
 
4.) site:*.org intitle:”Thank You For Your Order” intext:Click Here to Download
 
5.) site:*.biz intitle:”Thank You For Your Order” intext:Click Here to Download
 
6.) site:*.tv intitle:”Thank You For Your Order” intext:Click Here to Download
 
7.) site:*.co.uk intitle:”Thank You For Your Order” intext:Click Here to Download
 
8.) site:*.org.uk intitle:”Thank You For Your Order” intext:Click Here to Download
 
9.) site:*.eu intitle:”Thank You For Your Order” intext:Click Here to Download
 
10.) intitle:Thank you for your purchase! intext:PLR OR MRR OR Package OR Bonus
 
11.) intitle:Thank you for your order! intext:PLR OR MRR OR Package OR Bonus
 
12.) intitle:Thank you for your order! intext:PLR OR MRR
 
13.) intitle:Thank you for your Purchase! intext:PLR OR MRR
 
14.) inurl:/thankyou*.html intitle:Thank you for your order!
 
15.) intext:Click Here To Download
 
16.) inurl:thanks intext:”Thank You For Your Order!” “Click Here” filetype:html
 
17.) intitle:Thank You For Your Order! intext:Private Label
 
18.) intitle:Thank You For Your Purchased! intext:Private Label
 
19.) intext:”Thank You For Your Order” intext:PLR
 
20.) intitle:”Thank You For Your Order!” intext:download
 
21.) intitle:”Thank You For Your Order” intext:Click Here To Download Now
 
22.) intitle:Thank you for your purchase! intext:Click Here to Download
 
23.) * thank you for your order download
 
24.) * intitle:Thank you for your Purchase! intext:PLR OR MRR OR Package OR Bonus
 
25.) * intitle:Thank you for your order! intext:PLR OR MRR
 
26.) * intitle:Thank You For Your Purchase! intext:Click Here to Download
 
27.) * intitle:Thank You For Your Order! intext:download
 
28.) inurl:index.of .mp3
 
29.) inurl:index.of .mov
 
30.) inurl:index.of .iso
 
31.) ?intitle:index.of? mp3
 
32.) ?intitle:index.of? mov
 
33.) ?intitle:index.of? iso
 
34.) inurl:”insert filetype”:iso+OR+exe+OR+zip+OR+rar+OR+gzip+OR+tar
 
35.) intext:”parent directory” intext:”[EXE]“
 
36.) intext:”parent directory” index of:”[EXE]“
 
37.) intext:”parent directory” index of:”[RAR]“
 
38.) intext:”parent directory” intext:”[VID]“
 
39.) intext:”parent directory” index of:”[VID]“
 
40.) intext:”parent directory” intext:”[MP3]“
 
41.) intext:”parent directory” index of:”[MP3]“
 
42.) intext:”parent directory” index of:”[Gamez]“
 
# WEBCAM GOOGLE DORKS
 
1.) inurl:/view.index.shtml
 
2.) inurl:/view.shtml
 
3.) intitle:”Live View / – AXIS” | inurl:view/view.shtml^
 
4.) inurl:ViewerFrame?Mode=
 
5.) inurl:ViewerFrame?Mode=Refresh
