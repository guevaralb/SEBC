Luis4
i-03f4076823b2d608d
m4.4xlarge
us-east-1b
ec2-54-204-183-201.compute-1.amazonaws.com
54.204.183.201
August 4, 2017 at 8:49:23 AM UTC-5

Luis1
i-05582de36d7801b06
m4.4xlarge
us-east-1b
ec2-54-157-31-236.compute-1.amazonaws.com
54.157.31.236
August 4, 2017 at 8:46:17 AM UTC-5

Luis2
i-0977ce016b28286ea
m4.4xlarge
us-east-1b
ec2-54-152-7-139.compute-1.amazonaws.com
54.152.7.139
August 4, 2017 at 8:47:56 AM UTC-5

Luis3
i-09a358dce99823684
m4.4xlarge
us-east-1b
ec2-34-228-219-36.compute-1.amazonaws.com
34.228.219.36
August 4, 2017 at 8:47:56 AM UTC-5


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

