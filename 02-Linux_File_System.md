## Linux File System

### /bin
Contains essential commands for system startup and control. Files that can be used by both users and system administrators can be placed here (unless it makes the root directory too bloated). Programs like init, getty, updatedb, which only the root user might need, can be located in /sbin or /usr/sbin. Examples of files found in this directory are cat, chgrp, chown, date, dd, df, ln, mkdir, mount, ps, rm, sh, su, sync, and umount.

### /dev
Contains device files for I/O. Every supported device in the Linux kernel has a corresponding file under the /dev directory. During installation, these files are created and can be recreated using /dev/MAKEDEV if they are accidentally deleted.

### /etc
Contains system configuration files. This directory should not contain executable files.

### /skel
Files in this directory are copied to a user's home directory when the user account is created.

### /rc.d
Contains configuration files referred to by the init process. These are also known as "rc files."

### /passwd
Stores the user database.

### /fstab
Lists the file systems to be mounted during Linux startup.

### /group
Similar to passwd, it stores the groups of users.

### /inittab
Configuration file for the init daemon.

### /motd
Contains the message displayed on the user's screen after logging in.

### /profile
File executed when a user logs in (for csh and sh-like shells).

### /shells
Lists the names of shells available in the system.

### /login.access
Configuration file for the login command. Used to restrict access to the system on a per-user basis.

### /home
Directory allocated for users. Unless otherwise specified, each user account uses this directory. In larger systems,
this section can be further divided (e.g., /home/ftpadm, /home/student, etc.).

### /lib
Library files.

### /mnt
Temporarily mounted file systems. It is dedicated solely for this purpose, saving time for system administrators.

### /proc
File system that holds process controls and other system information. This file system does not occupy disk space; 
all files can be considered extensions of the kernel.

### /cpuinfo
Reports the processor model, type, and performance.

### /devices
Lists the device drivers currently running in the kernel.

### /dma
Specifies which DMA channels are in use.

### /filesystems
Lists the file systems supported by the current kernel.

### /interrupts
Indicates which interrupts are in use.

### /iports
Specifies which input/output ports are currently in use.

### /kcore
Snapshot of the system's memory.

### /root
Home directory for the system administrator. If possible, configure this directory to be inaccessible to other users.

### /sbin
Vital system commands. Previously, these files were located under the /etc directory. Only commands necessary for the system 
administrator are found in /sbin or /usr/sbin.

### /tmp
Directory for temporary files. It should be cleaned periodically.

### /usr
Contains other important system files. This directory is usually the largest because all newly installed programs are placed here.

### /X11R6
Contains information about the window system.

### /doc
Holds documentation files, typically HOWTO and FAQ files.

### /lib
Contains some libraries.

### /man
Stores manual pages.

### /src
Contains some source files and the code that builds the Linux kernel (/usr/src/linux).

### /sbin
Contains executable system administration files that do not need to reside in the root file system.

### /var
Stores system information that constantly changes. Except for some exceptions, it is not shared with other machines.

### /adm
Logs related to system administration.

### /preserve
Location for preserving files that may be damaged after a system crash.

### /spool
Temporary storage for data that will be processed later (e.g., email).
