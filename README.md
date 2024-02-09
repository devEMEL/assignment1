## ASSIGNMENT

Your login name: altschool i.e., home directory /home/altschool. The home directory contains the following sub-directories: code, tests, personal, misc Unless otherwise specified, you are running commands from the home directory.

#### `sudo useradd -m myaltschool`

#### `su - myaltschool`

#### `mkdir code tests personal misc`

a.Change directory to the tests directory using absolute pathname

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ cd /home/myaltschool/tests`

b.Change directory to the tests directory using relative pathname

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ cd tests`

c.Use echo command to create a file named fileA with text content ‘Hello A’ in the misc directory

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~/tests$ echo "Hello A" > /home/myaltschool/misc/fileA`

d.Create an empty file named fileB in the misc directory. Populate the file with a dummy content afterwards

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~/tests$ touch /home/myaltschool/misc/fileB`

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~/tests$ echo "This is file B" > /home/myaltschool/misc/fileB`

e.Copy contents of fileA into fileC

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~/tests$ cp /home/myaltschool/misc/fileA /home/myaltschool/misc/fileC`

f.Move contents of fileB into fileD

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~/tests$ mv /home/myaltschool/misc/fileB /home/myaltschool/misc/fileD`

g.Create a tar archive called misc.tar for the contents of misc directory

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ tar -cvf misc.tar misc`

h.Compress the tar archive to create a misc.tar.gz file

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ gzip misc.tar`

I. Create a user and force the user to change his/her password upon login

##### `myaltschool@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ sudo useradd mydom`

##### `dominic@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ sudo passwd -e mydom`

J. Lock a users password

##### `dominic@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ sudo passwd -l mydom`

K. Create a user with no login shell
##### `dominic@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ sudo useradd -s /usr/sbin/nologin freddo`

L. Disable password based authentication for ssh

##### `dominic@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ sudo nano /etc/ssh/sshd_config`
##### set `PasswordAuthentication no`

M. Disable root login for ssh

##### `dominic@dominic-HP-ENVY-x360-Convertible-15-dr1xxx:~$ sudo nano /etc/ssh/sshd_config`
##### set `PermitRootLogin no`