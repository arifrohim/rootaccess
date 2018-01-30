# rootaccess
Root Access for GC and AWS
To get root access via putty without key is realy simple
Please login to browser console
Enter below command:

sudo su root

passwd root

(Create new root password and confirm)

mv /etc/ssh/sshd_config /etc/ssh/sshd_config.bak

cd /etc/ssh/

wget https://raw.githubusercontent.com/arifrohim/rootaccess/master/gcsshd_config

mv gcsshd_config sshd_config

sudo service sshd restart

cd

Now you can login to you VPS via putty as root with your password without any key
