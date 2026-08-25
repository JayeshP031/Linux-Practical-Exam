# Linux Practical Examination

## Q1
**Commands:**
```bash
mkdir linuxexam
cd linuxexam
touch student.txt course.txt result.txt
pwd
ls
```
**Purpose:** Create the exam directory and required files, then check the current location and files.

## Q2
**Commands:**
```bash
cp student.txt student_backup.txt
mv course.txt linux_course.txt
rm result.txt
mkdir backups documents scripts
mv student_backup.txt backups/
tree
```
**Purpose:** Copy, rename, delete and move files, create directories, and display the directory structure.

## Q3
**Commands:**
```bash
cat student.txt
cat linux_course.txt
head -3 student.txt
tail -2 linux_course.txt
wc student.txt
```
**Purpose:** Display file contents, view selected lines, and count lines, words and characters.

## Q4
**Commands:**
```bash
sudo useradd -m student01
sudo passwd student01
su - student01
id student01
pwd
getent passwd student01
su - student01
```
**Purpose:** Create the user with a home directory, set its password, check UID/GID, check the home directory and switch to the user.

## Q5
**Commands:**
```bash
sudo groupadd linuxbatch
sudo usermod -aG linuxbatch student01
sudo useradd student02
sudo usermod -aG linuxbatch student02
grep linuxbatch /etc/group
```
**Purpose:** Create the group, add both users to it, and verify the group members.

## Q6
**Commands:**
```bash
cd linuxexam
touch project.txt
chmod 754 project.txt
ls -l
chmod 640 project.txt
sudo chown student01 project.txt
sudo chgrp linuxbatch project.txt
ls -l project.txt
```
**Purpose:** Create the file, set the required permissions, then change and verify its owner and group.

## Q7
**Commands:**
```bash
mkdir public private shared
chmod 777 public
chmod 700 private
chmod 770 shared
ls -ld public
ls -ld private
ls -ld shared
```
**Purpose:** Create the three directories, set their access permissions, and verify each permission.

## Q8
**Commands:**
```bash
sudo yum update -y
sudo yum install httpd -y
httpd -v
sudo service httpd start
sudo service httpd status
sudo systemctl enable httpd
```
**Purpose:** Update Amazon Linux packages, install Apache (`httpd`), check its version, start and check the service, and enable it at boot.

## Q9
**Commands:**
```bash
cd /var/www/html
sudo nano index.html
sudo service httpd restart
```
**Purpose:** Edit the Apache webpage in the document root and restart `httpd` to apply the changes.

## Q10
**Command shown:**
```bash
sudo service httpd status
```
**Purpose:** Check whether the Apache `httpd` service is running and view its process/PID information.

## Q11
**Commands:**
```bash
nano students.txt
grep "a" students.txt
grep -i "a" students.txt
grep -ic "a" students.txt
sort students.txt
find . -name "students.txt"
find . -name "*.txt"
```
**Purpose:** Search student records, perform case-insensitive matching, count matches, sort records, and find text files.

## Q12
**Commands:**
```bash
hostnamectl
hostname -I
ip link
ip route
ping google.com
```
**Purpose:** Display the system hostname, IP address, network interfaces and routing table, then test network connectivity.

## Note

The commands above are based on the commands visible in my practical screenshots and use the commands I actually used on Amazon Linux. Apache is managed as `httpd` on this system.
