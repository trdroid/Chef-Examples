# Installation

### Ubuntu

```sh
droid@droidserver:~/scratchpad/Chef/ChefDK-0.19.6$ uname -r
4.4.0-42-generic
droid@droidserver:~/scratchpad/Chef/ChefDK-0.19.6$ uname -a
Linux droidserver 4.4.0-42-generic #62~14.04.1-Ubuntu SMP Fri Oct 7 23:15:48 UTC 2016 x86_64 x86_64 x86_64 GNU/Linux
```

```sh
droid@droidserver:~/scratchpad/Chef/ChefDK-0.19.6$ sudo dpkg -i chefdk_0.19.6-1_amd64.deb
[sudo] password for droid: 
Selecting previously unselected package chefdk.
(Reading database ... 707589 files and directories currently installed.)
Preparing to unpack chefdk_0.19.6-1_amd64.deb ...
Unpacking chefdk (0.19.6-1) ...
Setting up chefdk (0.19.6-1) ...
Thank you for installing Chef Development Kit!
```

```sh
droid@droidserver:~/onGit/Chef-Tryouts$ which chef
/usr/bin/chef
droid@droidserver:~/onGit/Chef-Tryouts$ chef -v
Chef Development Kit Version: 0.19.6
chef-client version: 12.15.19
delivery version: master (802e801d920ea6b6d48db735aa7c6e7a6194bea4)
berks version: 5.1.0
kitchen version: 1.13.2
```
