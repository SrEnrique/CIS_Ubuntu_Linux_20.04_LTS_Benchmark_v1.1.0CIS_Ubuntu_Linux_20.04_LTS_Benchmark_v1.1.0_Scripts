# CIS-Benchmarchs Ubuntu Server 20.04

## Download
``` 
git clone https://github.com/SrEnrique/CIS_Ubuntu_Linux_20.04_LTS_Benchmark_v1.1.0_Scripts.git
``` 
## Usage

Run audit recommendation scripts
``` 
$ sudo sh run 
CIS Ubuntu Linux 20.04 LTS Benchmark
v1.1.0 - 03-31-2021

System information
hostname : neon
Distributor ID: Neon
Description: KDE neon User - 5.25
Release: 20.04
time : Mon 25 Jul 2022 05:26:04 PM MDT
=========================================
FAIL - 1.1.1.1 - Ensure mounting of cramfs filesystems is disabled (Automated)
FAIL - 1.1.1.2 - Ensure mounting of freevxfs filesystems is disabled (Automated)
FAIL - 1.1.1.3 - Ensure mounting of jffs2 filesystems is disabled (Automated)
FAIL - 1.1.1.4 - Ensure mounting of hfs filesystems is disabled (Automated)
FAIL - 1.1.1.5 - Ensure mounting of hfsplus filesystems is disabled (Automated)
FAIL - 1.1.1.6 - Ensure mounting of squashfs filesystems is disabled (Manual)
FAIL - 1.1.1.7 - Ensure mounting of udf filesystems is disabled (Automated)
PASS - 1.1.2 - Ensure /tmp is configured (Automated)
PASS - 1.1.3 - Ensure nodev option set on /tmp partition (Automated)
PASS - 1.1.4 - Ensure nosuid option set on /tmp partition (Automated)
PASS - 1.1.5 - Ensure noexec option set on /tmp partition (Automated)
PASS - 1.1.6 - Ensure /dev/shm is configured (Automated)
PASS - 1.1.7 - Ensure nodev option set on /dev/shm partition (Automated)
PASS - 1.1.8 - Ensure nosuid option set on /dev/shm partition (Automated)
FAIL - 1.1.9 - Ensure noexec option set on /dev/shm partition (Automated)
FAIL - 1.1.10 - Ensure separate partition exists for /var (Automated)
FAIL - 1.1.11 - Ensure separate partition exists for /var/tmp (Automated)
PASS - 1.1.12 - Ensure /var/tmp partition includes the nodev option (Automated)
PASS - 1.1.13 - Ensure /var/tmp partition includes the nosuid option (Automated)
PASS - 1.1.14 - Ensure /var/tmp partition includes the noexec option (Automated)
FAIL - 1.1.15 - Ensure separate partition exists for /var/log (Automated)
FAIL - 1.1.16 - Ensure separate partition exists for /var/log/audit (Automated)
FAIL - 1.1.17 - Ensure separate partition exists for /home (Automated)
PASS - 1.1.18 - Ensure /home partition includes the nodev option (Automated)
SKIP - 1.1.19 - Ensure nodev option set on removable media partitions (Manual)
SKIP - 1.1.20 - Ensure nosuid option set on removable media partitions (Manual)
SKIP - 1.1.21 - Ensure noexec option set on removable media partitions (Manual)
FAIL - 1.1.22 - Ensure sticky bit is set on all world-writable directories (Automated)
PASS - 1.1.23 - Disable Automounting (Automated)
FAIL - 1.1.24 - Disable USB Storage (Automated)

Results

Scored (Server)
==================
Server 1 = 12 / 21
Server 2 = 12 / 26

Scored (Workstation)
==================
Workstation 1 = 11 / 20
Workstation 2 = 12 / 26

Not Scored (Server)
==================
Server 1 = / 3
Server 2 = / 4

Not Scored (Workstation)
==================
Workstation 1 = / 3
Workstation 2 = / 4
```

If run a single recommendation scripts this show you a bit of help for the solve and know the problem with this recommendation 

```
$ sudo sh tester/1.1.10.sh
mnt_var: 
expecten: verify output shows /var is mounted
No Mount var
```

