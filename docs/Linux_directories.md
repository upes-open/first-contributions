# LINUX DIRECTORIES
#### by [Ashutosh Gupta](https://github.com/m3tac1ph4r)

In this blog we will talk about directories in linux. Why binaries are kept /bin or /usr/sbin.

![image](https://static.thegeekstuff.com/wp-content/uploads/2010/11/filesystem-structure.png)

1. **/root** : As we know plant starts growing after the root , same in linux. Every single file and directory starts from the root directory. Only root user has write privilege under this directory. 

2. **/bin** **(User binaries)** : This directory contains binary executables. Common linux commands you need to use in single-user modes are located under this directory.
For example : ps,ls,grep,etc.

3. **/sbin (System Binaries)** : Just like /bin, /sbin also contains binary executables.
But, the linux commands located under this directory are used typically by system aministrator, for system maintenance purpose. For example: iptables, reboot, fdisk, ifconfig, swapon etc.

4. **/etc (Configuration Files)** : Contains configuration files required by all programs.
This also contains startup and shutdown shell scripts used to start/stop individual programs.
For example: /etc/resolv.conf, /etc/logrotate.conf,etc.

5. **/dev (Device Files)** : These include terminal devices, usb, or any device attached to the system.
For example: /dev/tty1, /dev/usbmon0.

6. **/proc (Process Information)** : Contains information about system process. This is a pseudo filesystem contains information about running process. For example: /proc/{pid} directory contains information about the process with that particular pid.

7. **/var (Variable Files)** : Content of the files that are expected to grow can be found under this directory.
This includes — system log files (/var/log); packages and database files (/var/lib); emails (/var/mail); print queues (/var/spool); lock files (/var/lock); temp files needed across reboots (/var/tmp).

8. **/tmp (Temporary Files)** : Directory that contains temporary files created by system and users.
Files under this directory are deleted when system is rebooted.

9. **/usr (User Programs)** : Contains binaries, libraries, documentation, and source-code for second level programs. /usr/lib contains libraries for /usr/bin and /usr/sbin
/usr/local contains users programs that you install from source. For example, when you install apache from source, it goes under /usr/local/apache2 . 

10. **/home (Home Directory)** : Home directories for all users to store their personal files. 

11. **/boot (Boot Loader Files)** : Contains Kernel initrd, vmlinux, grub files are located under /boot .

12. **/lib (System Libraries)** : Contains library files that supports the binaries located under /bin and /sbin

13. **/opt (Optional add-on Applications)** : Contains add-on applications from individual vendors.

14. **/mnt (Mount Directory)** : Temporary mount directory where sysadmins can mount filesystems.

15. **/media (Removable Media Devices)** : Temporary mount directory for removable devices.
For examples, /media/cdrom for CD-ROM; /media/floppy for floppy drives; /media/cdrecorder for CD writer

16. **/srv (Service Data)** : Contains server specific services related data.


### Reference:
https://www.geeksforgeeks.org/linux-file-hierarchy-structure/


                        Thank you for Reading!!