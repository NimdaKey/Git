Git
===
  Follows
How to use github
=================
第一步： 生成ssh key，使用命令 “ssh-keygen -t rsa -C "your_email@youremail.com"”，your_email是你的email		
		 
ubuntu@ubuntu:~$ ssh-keygen -t rsa -C your_email@youremail.com
Generating public/private rsa key pair.
Enter file in which to save the key (/home/ubuntu/.ssh/id_rsa): 
/home/ubuntu/.ssh/id_rsa already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/ubuntu/.ssh/id_rsa.
Your public key has been saved in /home/ubuntu/.ssh/id_rsa.pub.
The key fingerprint is:
87:94:19:04:1f:dd:d7:76:bc:77:81:be:52:c1:91:75 your_email@youremail.com
The key's randomart image is:
+--[ RSA 2048]----+
|      .o+. ...=+E|
|       . =. .=..*|
|        =   ....+|
|       . .   o .o|
|        S . . . o|
|         . . .   |
|            .    |
|                 |
|                 |
+-----------------+
ubuntu@ubuntu:~$ cat /home/ubuntu/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCbQLaYMQLaUsJkrfTfq6H+RxTcOOfRxKSPVDEniP4sU3E7wJe62IYUGFlJFl97ouqLLk5QIEan6jttkzvY5WfHbaXpP2W7A53ioqRx4unYH3mZK8ftzFc2wnA8j0k03U+bLQnvdAp1hlnAVha5Vz+dUDBvUnfLmNI4W511eDbPLKKrtnshSQMsJHIrq7qJ4KcU+17OOtUd52sOC/RoYvn9Y/epsn3ncVJn5TRxKD/n5WY884G/MoXWvxD3uQq4CuqOZRgi67E4hpbVoQ3XkPMW9m3YEXlHYsAYiopHN5U38OUniUGwWWhVpZxeZgsbI4e5qRGa4Yij0k1U4l5e+v0B your_email@youremail.com

第二步： 登陆github，进入Account Settings，左边选择SSH Keys，Add SSH Key,title随便填，粘贴public key。
第三步： 测试ssh key是否成功，使用命令“ssh -T git@github.com”，如果出现You’ve successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。
