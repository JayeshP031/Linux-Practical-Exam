# Linux Practical Examination

## Q1
**Commands:**
```bash
mkdir LinuxExam
cd LinuxExam
touch student.txt course.txt result.txt
pwd
ls
```
**Purpose:** Create the directory and files, enter the directory, and verify the location and contents.

## Q2
**Commands:**
```bash
cp student.txt student_backup.txt
mv course.txt linux_course.txt
rm result.txt
mkdir Documents Backups Scripts
mv student_backup.txt Backups/
tree
```
**Purpose:** Copy, rename, delete and move files, create directories, and view the directory structure.

## Q3
**Commands:**
```bash
cat student.txt
cat linux_course.txt
head -n 3 student.txt
tail -n 2 student.txt
wc student.txt
```
**Purpose:** Display file contents, show selected lines, and count lines, words and characters.

## Q4
**Commands:**
```bash
sudo adduser student01
id student01
getent passwd student01
sudo su - student01
whoami
```
**Purpose:** Create and verify a user, check UID/GID and home directory, and switch to the user.

## Q5
**Commands:**
```bash
sudo groupadd linuxbatch
sudo usermod -aG linuxbatch student01
groups student01
sudo adduser student02
sudo usermod -aG linuxbatch student02
getent group linuxbatch
```
**Purpose:** Create a group, add users to it, and verify group membership.

## Q6
**Commands:**
```bash
touch project.txt
chmod 754 project.txt
ls -l project.txt
chmod 640 project.txt
sudo chown student01 project.txt
sudo chgrp linuxbatch project.txt
ls -l project.txt
```
**Purpose:** Set and verify file permissions, then change the owner and group.

## Q7
**Commands:**
```bash
mkdir public private shared
chmod 755 public
chmod 700 private
chmod 770 shared
ls -ld public private shared
```
**Purpose:** Create the directories, set different access permissions, and verify them.

## Q8
**Commands:**
```bash
sudo apt update
sudo apt install apache2
apache2 -v
sudo systemctl start apache2
sudo systemctl status apache2
sudo systemctl enable apache2
```
**Purpose:** Update packages, install Apache, check its version and manage its service.

## Q9
**Commands:**
```bash
cd /var/www/html
sudo nano index.html
sudo systemctl restart apache2
curl http://localhost
curl -I http://localhost
```
**Purpose:** Create the Apache webpage, restart the service, access the page, and check the HTTP response.

## Q10
**Commands:**
```bash
ps aux
top
pgrep apache2
ps -p <PID>
sudo systemctl stop apache2
sudo systemctl status apache2
sudo systemctl start apache2
sudo systemctl status apache2
```
**Purpose:** View processes, find the Apache PID, check process details, stop Apache, and start it again.

## Q11
**Commands:**
```bash
grep "name" students.txt
grep -i "name" students.txt
grep -ic "name" students.txt
sort students.txt
find LinuxExam -name "*.txt"
```
**Purpose:** Search student records, perform case-insensitive searches, count matches, sort records, and find text files.

## Q12
**Commands:**
```bash
hostname
ip addr
ip link
ip route
ping google.com
curl https://example.com
nslookup google.com
ss -tuln
```
**Purpose:** Check hostname, IP information, interfaces, routing, connectivity, domain IP, webpage access, and listening ports.
