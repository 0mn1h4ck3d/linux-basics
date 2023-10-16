# Kali Linux Commands Cheatsheet

## 1. System Commands:

- **pwd**: Print current working directory.
  - Example: `pwd`

- **ls**: List files and directories.
  - Example: `ls -l`

- **cd**: Change directory.
  - Example: `cd /path/to/directory`

- **mkdir**: Create a new directory.
  - Example: `mkdir new_directory`

- **rmdir**: Remove a directory.
  - Example: `rmdir directory_name`

- **cp**: Copy files/directories.
  - Example: `cp file.txt destination_folder/`

- **mv**: Move or rename files/directories.
  - Example: `mv file.txt new_location/`

- **rm**: Remove files/directories.
  - Example: `rm file.txt`

- **chmod**: Change file permissions.
  - Example: `chmod 755 file.txt`

- **chown**: Change file owner and group.
  - Example: `chown user:group file.txt`

- **ps**: Display information about running processes.
  - Example: `ps aux`

- **kill**: Terminate processes using process IDs.
  - Example: `kill PID`

- **top**: Display and manage running processes.
  - Example: `top`

- **df**: Show disk space usage.
  - Example: `df -h`

- **du**: Display file and directory space usage.
  - Example: `du -h file.txt`

- **uname**: Display system information.
  - Example: `uname -a`

- **date**: Display or set the system date and time.
  - Example: `date`

- **man**: Display the manual page of a command.
  - Example: `man ls`

## 2. Package Management:

- **apt-get update**: Update the list of available packages.
  - Example: `sudo apt-get update`

- **apt-get upgrade**: Upgrade all installed packages to the latest version.
  - Example: `sudo apt-get upgrade`

- **apt-get install [package]**: Install a new package.
  - Example: `sudo apt-get install nmap`

- **apt-get remove [package]**: Remove a package.
  - Example: `sudo apt-get remove nmap`

- **apt-cache search [keyword]**: Search for a package.
  - Example: `apt-cache search text-editor`

- **dpkg -i [package.deb]**: Install a Debian package.
  - Example: `sudo dpkg -i package.deb`

- **dpkg -r [package]**: Remove a Debian package.
  - Example: `sudo dpkg -r package_name`

## 3. Networking:

- **ifconfig**: Display network interfaces and their configuration.
  - Example: `ifconfig`

- **iwconfig**: Configure wireless network interfaces.
  - Example: `iwconfig wlan0 essid "SSID" key "PASSWORD"`

- **ping [host]**: Send ICMP echo requests to a host.
  - Example: `ping google.com`

- **netstat**: Display network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.
  - Example: `netstat -tuln`

- **nc**: Netcat - versatile networking tool to read and write data across network connections.
  - Example: `nc -l -p 1234`

- **traceroute [host]**: Display the route that packets take to reach the host.
  - Example: `traceroute google.com`

- **wget [URL]**: Download files from the internet.
  - Example: `wget http://example.com/file.txt`

## 4. Security and Penetration Testing:

- **nmap [target]**: Network mapper; scans ports and services on a network.
  - Example: `nmap 192.168.1.1`

- **nikto -h [target]**: Web server scanner.
  - Example: `nikto -h example.com`

- **hydra -l [username] -P [password-list] [target] [protocol]**: Password-cracking tool.
  - Example: `hydra -l admin -P /path/to/passwords.txt ftp://192.168.1.1`

- **john [hashfile]**: John the Ripper; password-cracking tool.
  - Example: `john hash.txt`

- **aircrack-ng [file.cap]**: Wireless security cracking tool for Wi-Fi networks.
  - Example: `aircrack-ng capture_file.cap`

- **sqlmap -u [URL]**: Automatic SQL injection and database takeover tool.
  - Example: `sqlmap -u "http://example.com/index.php?id=1"`

- **msfconsole**: Metasploit Framework; penetration testing and exploitation tool.
  - Example: `msfconsole`

## 5. File Encryption and Compression:

- **gpg -c [file]**: Encrypt a file using GPG.
  - Example: `gpg -c confidential.doc`

- **gpg -d [file.gpg]**: Decrypt a GPG-encrypted file.
  - Example: `gpg -d file.gpg`

- **tar -cvzf [archive.tar.gz] [directory]**: Create a compressed tarball.
  - Example: `tar -cvzf backup.tar.gz /path/to/directory`

- **tar -xvzf [archive.tar.gz]**: Extract files from a tarball.
  - Example: `tar -xvzf backup.tar.gz`

## 6. Miscellaneous:

- **locate [filename]**: Quickly find the location of a file.
  - Example: `locate myfile.txt`

- **find [directory] -name [filename]**: Search for files and directories.
  - Example: `find /home/user -name *.txt`

- **grep [pattern] [file]**: Search for a specific pattern in a file.
  - Example: `grep "error" log.txt`

- **ssh [user]@[host]**: Securely connect to a remote system.
  - Example: `ssh user@192.168.1.1`

- **scp [file] [user]@[host]:[destination]**: Securely copy files between systems.
  - Example: `scp file.txt user@192.168.1.1:/path/to/destination/`
