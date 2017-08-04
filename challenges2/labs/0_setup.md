AWS 

Luis4
i-022bb349bc84bfc50
m4.2xlarge
us-east-1b
ec2-54-173-57-43.compute-1.amazonaws.com
54.173.57.43
# cat /etc/centos-release
CentOS Linux release 7.3.1611 (Core) 


Luis3
i-0605f457ac6b6df1e
m4.2xlarge
us-east-1b
ec2-54-236-4-132.compute-1.amazonaws.com
54.236.4.132
# cat /etc/centos-release
CentOS Linux release 7.3.1611 (Core) 

Luis2
i-07aa31513f58df15c
m4.2xlarge
us-east-1b
ec2-52-90-69-13.compute-1.amazonaws.com
52.90.69.13
# cat /etc/centos-release
CentOS Linux release 7.3.1611 (Core) 

Luis1
i-0a05a762b777c73f3
m4.2xlarge
us-east-1b
ec2-34-230-24-146.compute-1.amazonaws.com
34.230.24.146
# cat /etc/centos-release
CentOS Linux release 7.3.1611 (Core) 
# Filesystem Luis1 :
# df -h
/dev/xvda1        80G   4,5G   76G   6% /
devtmpfs          16G      0   16G   0% /dev
tmpfs             16G      0   16G   0% /dev/shm
tmpfs             16G   332K   16G   1% /run
tmpfs             16G      0   16G   0% /sys/fs/cgroup
/dev/xvde         50G    33M   50G   1% /var/lib/mesos
/dev/xvdf        100G    33M  100G   1% /var/lib/docker
/dev/xvdg         50G    33M   50G   1% /dcos/volume0
/dev/xvdh         20G    58M   20G   1% /var/log
tmpfs            3,2G      0  3,2G   0% /run/user/1000
tmpfs            3,2G      0  3,2G   0% /run/user/995


# adduser --uid 2800 saturn 
# adduser --uid 2900 haley
# groupadd comets
# groupadd planets
# usermod  -aG planets saturn
# usermod  -aG comets haley

# cat /etc/passwd | grep "saturn\|haley"
saturn:x:2800:2800::/home/saturn:/bin/bash
haley:x:2900:2900::/home/haley:/bin/bash

# cat /etc/group | grep "planets\|comets"
comets:x:2901:haley
planets:x:2902:saturn

# yum repolist enabled
Complementos cargados:fastestmirror
Loading mirror speeds from cached hostfile
 * base: mirror.umd.edu
 * epel: mirror.cogentco.com
 * extras: mirror.atlanticmetro.net
 * updates: mirror.math.princeton.edu
id del repositorio                                                 nombre del repositorio                                                                         estado
base/7/x86_64                                                      CentOS-7 - Base                                                                                 9.363
cloudera-cdh5                                                      Cloudera's Distribution for Hadoop, Version 5                                                     146
cloudera-manager                                                   Cloudera Manager                                                                                    7
epel/x86_64                                                        Extra Packages for Enterprise Linux 7 - x86_64                                                 11.919
extras/7/x86_64                                                    CentOS-7 - Extras                                                                                 449
updates/7/x86_64                                                   CentOS-7 - Updates                                                                              2.130
repolist: 24.014

	