File Structures and Permissions


			d rwx r-x r-x  3 thirumal thirumal 4096 Dec 19 15:18 Desktop
			1  2   3   4   5    6        7       8     9          10

1 -> can be a directory,file or a link.
(d,-,l)


r-read(4), w-write(1), x-execute(0), - means denied permission.

x- has two functionalities.
for Files -> it tells that it is an excutable file, so the user or group can execute the file if they have the permission.
for Directories -> It tells that whether we can go inside that directory or not.


2-> user Permissions
3-> Group permissions
4-> Other - means everybody else(public)

6-> userName

7-> groupName 


if we want to give or revoke permissions, we can use chmod command.
for ex:
chmod u+x myFile.txt
chmod g-w myFile.txt
chmod o-r myFile.txt

Or we can use numerical expressions to grant or revoke permissions.
chmod ??? myFile.txt

?      ?	?
user group other

for ex: chmod 770 myFile.txt    which means 111 111 000
		chmod 526 myFile.txt    which means 101 010 110


Inorder to change ownership on a file or a directory, we use #chown command.

sudo chown kurni Desktop/     -> user
sudo chown kurni:kurni Desktop/ -> group 



About 5 and 8 we will learn in processes and inodes.
