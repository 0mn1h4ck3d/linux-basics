# Linux File System Cheatsheet

## 1. Root Directory ("/"):

- **`/bin`**: Contains essential binaries (commands) required for all users to execute basic commands and perform system tasks.
- **`/boot`**: Contains boot loader files and the Linux kernel; crucial for the system's boot process.
- **`/dev`**: Contains device files representing hardware devices, allowing interaction with components like disks, terminals, and USB devices.
- **`/etc`**: Stores system-wide configuration files controlling system behavior, services, and installed applications.
- **`/home`**: Contains user home directories; each user has a subdirectory to store personal files and configurations.
- **`/lib`**: Contains shared libraries essential for programs in `/bin` and `/sbin`.
- **`/media`**: Provides mount points for removable media devices like USB drives and external hard disks.
- **`/mnt`**: Offers temporary mount points for manually mounted devices or network shares.
- **`/opt`**: Used for optional software packages and add-on applications; some third-party apps are installed here.
- **`/proc`**: Virtual filesystem offering detailed information about the kernel, processes, and system resources; used for debugging and monitoring.
- **`/root`**: Home directory of the root user, the system administrator; has superuser privileges.
- **`/sbin`**: Contains essential system binaries (commands) primarily used by the root user for system administration tasks.
- **`/srv`**: Contains data directories for services provided by the system; often used by web servers and network services.
- **`/sys`**: Virtual filesystem exposing kernel parameters and other kernel-related information; used for interacting with the kernel at runtime.
- **`/tmp`**: Provides a location for temporary files accessible to all users; typically deleted when the system reboots.
- **`/usr`**: Contains user programs, libraries, documentation, and files essential for normal system operation and maintenance.
- **`/var`**: Contains variable files, including logs, databases, spool files, and other files that may change in size and content as the system runs.

## 2. Important Files:

- **`/etc/passwd`**: Contains user account information, including usernames, user IDs, home directories, and default shells.
- **`/etc/fstab`**: Specifies file systems, devices, and mount points for system boot.
- **`/etc/hostname`**: Contains the system's hostname used to identify the system on a network.
- **`/etc/resolv.conf`**: Configures DNS resolver, specifying DNS servers for domain name resolution.
- **`/etc/hosts`**: Maps IP addresses to hostnames, enabling hostname resolution without querying DNS servers.
- **`/etc/ssh/sshd_config`**: Configuration file for SSH server, specifying security and connection settings.
- **`/etc/network/interfaces`**: Configuration file for network interfaces, specifying IP addresses, gateway information, and network settings.
- **`/etc/sysctl.conf`**: Configuration file for kernel parameters, allowing customization of various kernel settings.
- **`/var/log`**: Contains system log files, recording events, errors, and system component information.
- **`/var/spool/mail`**: Contains mailbox files for user emails; incoming emails for users are stored here until read.
- **`/var/run`**: Contains process ID (PID) files of running processes, used to track and manage processes.
- **`/var/tmp`**: Provides a location for temporary files preserved between system reboots; files here are not automatically deleted on reboot.
- **`/etc/shadow`**: The `/etc/shadow` file in Linux systems stores encrypted user passwords and related security information, such as password aging policies. It contains password hashes using cryptographic hash functions, ensuring the security of user passwords. Accessible only by the superuser, it is used to manage user authentication and enforce password policies. Common commands related to managing passwords include passwd, chage, and usermod. Modification of this file requires careful handling to prevent system authentication issues.

## 3. Types of Files:

- **Regular Files**: Most common type of file on the system, containing data such as text, images, and programs.
- **Directories**: Containers for files and other directories, organizing the file system hierarchy.
- **Symbolic Links (Symlinks)**: Pointers to another file or directory, similar to shortcuts in Windows.
- **Device Files**: Represent hardware devices; two types - block devices (for storage) and character devices (for input devices like keyboards).
- **Sockets**: Communication endpoints used for interprocess communication on the same or different systems.
- **FIFOs (Pipes)**: Named pipes allowing one-way communication between processes.
