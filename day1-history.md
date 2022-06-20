less anaconda-ks.cfg
more anaconda-ks.cfg
cat anaconda-ks.cfg | grep timezone 
cat anaconda-ks.cfg | grep timezone | grep -v "#" 
cat anaconda-ks.cfg | grep timezone | grep -v "#" -n 
cat anaconda-ks.cfg | grep -e timezone -e rootpw
grep -e timezone -e rootpw anaconda-ks.cfg 
grep -e timezone -e rootpw anaconda-ks.cfg > /tmp/timezone.txt
vi /tmp/timezone.txt 
grep -e timezone -e rootpw anaconda-ks.cfg >> /tmp/timezone.txt
vi /tmp/timezone.txt 
grep -e timezone -e rootpw anaconda-ks.cfg > /tmp/timezone.txt
vi /tmp/timezone.txt 
su - student
vi test
cat test
vi /etc/ssh/sshd_config 
cat /etc/ssh/sshd_config | grep -v "#"
cat test 
grep -i alma -A 1 -B 2
grep -i alma -A 1 -B 2 test 
grep ^test test 
grep ^/ test
vi test 
grep ^/ test
vi test 
grep ^/ test
man find 
find / -name test
find / -name -type f test
find / -type f -name test
touch testFolder
find / -type f -name *stFo*
find /home/student -type d -empty
find / -type f -name *stFo* -exec mv {} /tmp/ \;
ls -la /tmp/
cat test 
sed 's/file/folder/g' test 
sed -i 's/file/folder/g' test 
cat test
sed 's/\bfoo\b/linux/g' test 
sed 's//bin/bash//bin/sh' test
sed 's|/bin/bash|/bin/sh' test
sed 's|/bin/bash|/bin/sh/' test
sed 's|/bin/bash|/bin/sh/g' test
sed 's|/bin/bash|/bin/sh|g' test
sed 's@/bin/bash@/bin/sh@g' test
sed 's/\b[0-9]\{3\}\b/number/g' test 
sed 's/\b[0-9]\{3\}\b/number is &/g' test 
tail /etc/passwd > passwd
tail /etc/passwd
head /etc/passwd
vi passwd 
head -2 /etc/passwd
tail -2 /etc/passwd
cat /etc/passwd | wc -l
cat /etc/passwd | grep : -n
cat passwd | grep : -n
cat passwd | cut -d : -f 1
cat passwd | cut -d : -f 1,6
cat passwd | cut -d : -f 1,5-6
vi test 
cat test 
cat test | grep bash
cat test | grep bash | cut -d " " -f 1
cat test | grep bash | cut -d "," -f 1
cat test | grep bash | cut -d "," -f 1 | cut -d " " -f 1
cat test | grep bash | cut -d "," -f 1 | cut -d " " -f 1 | head -1
alias
which vi
vi
vi test 
vi nowyPlik 
mkdir test1
mkdir test2 test3
ls -al
rmdir test3
touch test2/testfile
rmdir test2
rm -rf test2/
touch test1/test
rm -r test1
ls -la
mv nowyPlik nowy
ls -la
pwd
mv nowy /tmp/nowyPlik
ls -la /tmp/nowyPlik
ls -laZ
cp -rp /tmp/nowyPlik 
ps -ef
ps --help
ps --help simpl
ps -efd
man ps
ps -ejH
ps aux 
ps axo pid,user,comm
ps -eL
ps -C "bash"
ps -efC "bash"
ps -C "bash"
ps -U student
ps -U student -u student
ps -u student
ps -U student -u student
ps -u student
pgrep httpd
pgrep bash
pgrep gdm*
pgrep gdm* -l
pgrep gdm* -l -u student
pgrep gdm* -l -v -u student
ps -ef
ps aux
ps -efl
ps -efl | tail -20
clear
ps -efl
vi skrypt.sh 
chmod 700 skrypt.sh
./skrypt.sh & 
ps -efl | grep -i skrypt
ps -efl | grep -i skrypt | grep -v grep
renice +10 4775
ps -efl | grep -i skrypt | grep -v grep
renice -500 4775
ps -efl | grep -i skrypt | grep -v grep
nice -n 5 ./skrypt.sh 
nice -n 5 ./skrypt.sh & 
ps -efl | grep -i skrypt | grep -v grep
nice -n -15 ./skrypt.sh & 
ps -efl | grep -i skrypt | grep -v grep
ps -efl
ps aux
kill -l

ps aux | grep -i "Z"
kill -l
ps -ef
kill -15 5001
ps -ef
kill -15 5069
ps -ef
kill -15 5078
ps -ef
ps -ef | grep -i skrypt
ps -ef | grep -i sshd
kill -l
kill -19 5006
kill -18 5006
kill -15 5006
ps -ef | grep -i sshd
ipcs
lspci 
clear
rpm --help
rpm -qa 
rpm -Va
wget https://vault.centos.org/centos/8/BaseOS/x86_64/os/Packages/nano-2.9.8-1.el8.x86_64.rpm
ls -la
rpm -qa | grep -i nano
rpm -e nano
rpm -qa | grep -i nano
nano
rpm -ivh nano-2.9.8-1.el8.x86_64.rpm 
nano
rpm -qa | grep -i nano
rpm -Va 
rpm --help
man rpm
rpm -V nano 
ls -la
rpm -V nano-2.9.8-1.el8.x86_64.rpm
wget https://vault.centos.org/centos/8/BaseOS/x86_64/os/Packages/NetworkManager-1.32.10-4.el8.x86_64.rpm
ls -l
rpm -qa | grep -i networkmanager
rpm -qa | grep -i perl
rpm -ivh NetworkManager-1.32.10-4.el8.x86_64.rpm 
dnf saerch nano
dnf search nano
uname -r
dnf search NetworkManager
dnf info nano
rpm -qa | grep -i nano
rpm -e nano
rpm -qa | grep -i nano
dnf install nano
dnf remove nano
dnf repolist
dnf repolist all
ls
dnf remove nano
dnf localinstall nano-2.9.8-1.el8.x86_64 
dnf localinstall nano-2.9.8-1.el8.x86_64.rpm
cd /etc/yum.repos.d/
ls -la
vi almalinux.repo
dnf repolist all
dnf config-manager --enablerepo ha
dnf config-manager --enablerepo "AlmaLinux 8 - HighAvailability"
dnf config-manager --enable ha
dnf config-manager --enablerepo "AlmaLinux 8 - HighAvailability"
dnf repolist 
dnf repolist all
dnf config-manager --disable ha
dnf repolist all
ls -la
head 20 almalinux.repo 
vi myRepo.repo
dnf repolist all
ls -la
vi almalinux-ha.repo
dnf repolist all
rm myRepo.repo 
dnf repolist all
dnf config-manager --disable ha
dnf config-manager --disable ha-*
dnf repolist all
dnf config-manager --add-repo https://mirrors.almalinux.org/mirrorlist/$releasever/baseos
dnf repolist all
vi mirrors.almalinux.org_mirrorlist_baseos.repo
rm mirrors.almalinux.org_mirrorlist_baseos.repo
dnf grouplist
dnf groupinstall "Security Tools"
dnf groupremove "Security Tools"
rpm -qa | grep -i createrepo
dnf install createrepo
 mkdir localRpms
mv *.rpm localRpms/
cd
mv /etc/yum.repos.d/localRpms/ /root/
mv *.rpm localRpms/
ls localRpms/
cd localRpms/
ls -la
wget https://repo.almalinux.org/almalinux/8/AppStream/x86_64/os/Packages/createrepo_c-0.17.7-5.el8.x86_64.rpm
ls -la
createrepo --help
createrepo --database .
ls -la
cd repodata
ls -la
less repomd.xml
pwd
cd ..
pwd
dnf config-manager --add-repo [root@alinux8 repodata]#
vi /etc/yum.repos.d/root_localRpms_rootalinux8.repo
dnf repolist all
dnf clean all
dnf repolist
rpm -e nano
dnf install nano
dnf repolist 
dnf repolist all
yum repolist
which yum
ls -la /usr/bin/yum
ls -la /usr/bin/dnf
dnf module list
dnf module install php
dnf module install erl
dnf module install perl
dnf module install perl:5.32/minimal
dnf module install nodejs:14/minimal
dnf module list
dnf module remove nodejs
dnf module list
dnf module install nodejs:16/minimal
dnf module reset nodejs
cd
dnf module list 
dnf module install nodejs:16/minimal
dnf module list 
dnf history list
dnf history 15
dnf history list
dnf history 16
dnf history 14
dnf history undo 14
dnf history 
dnf history undo 15
dnf modele reset nodejs
dnf module reset nodejs
dnf history undo 15
rpm -qa > /tmp/BeforePatching.txt
rpm -qa | sort > /tmp/BeforePatching.txt
vi /tmp/BeforePatching.txt
mkdir git
cd git
git config --global user.email 'markuj5@gmail.com'
git config --global user.name 'Marcin Kujawski'
git clone https://github.com/mariano-italiano/lfs301_Jun.git
ls -la
cd lfs301_Jun/
ls -la
touch READEME.md
vi READEME.md
git status
git add READEME.md 
git status
git commit -m "Adding first file"
git status
git branch --unset-upstream
git status
git push
git push --set-upstream origin master
git status
git fetch
git pull
git fetch
git pull
git status
ls -la
git checkout v1.0 
ls -la
vi testfile.md 
rm READEME.md 
git status
git rm READEME.md 
git add testfile.md 
git status
git commit -m "Do some cleanup"
git push
history
history | awk '$1 > 113' | cut -c 8- 
history | awk '$1 > 113' | cut -c 8- > day1-history.md
vi day1-history.md
clear
cd
nmap
nmap 192.168.0.1/24
ip a s
nmap  192.168.1.80/24
nmap  192.168.1.80
nmap -p 80 192.168.1.80
dnf isntall telnet
dnf install telnet
telnet 192.168.1.80 22
telnet 192.168.1.80 443
telnet 192.168.1.1 443
curl -v telnet://192.168.1.1:80
dnf install traceroute
traceroute -I wp.pl
traceroute --help
\
traceroute -I wp.pl
ethtool -S ens33 
ip a
ip -s link
systemctl status firewalld.service 
netstat -vatunlp
nmap 192.168.1.80
ss -tulpna
dnf search netstat
dnf provides "*netstat"
iostat
df -h
lvs
vgs
pvs
netstat -i
vmstat -5
vmstat 5
sar
cd /var/log/ 
ls
cd sa
ls 
ls -la
vi /etc/cron.d
vi /etc/cron.daily/logrotate 
cd
lastlog
cd /var/log
ls -la
less kdump.log
less dnf.log
w
dnf install tuned
systemctl status tuned
tuned-adm active 
tuned-amd list
tuned-adm list
tuned-adm profile_info desktop
tuned-adm profile powersave 
tuned-adm active 
tuned-adm recommend 
tuned-adm profile virtual-guest
tuned-adm active 
date
date +%d-%m-%y
date +%d-%m-%yyyy
date +%d-%m-%Y
date +%d/%m/%Y
date +%d/%m/%Y-%H:%M:%S
date +%d/%m/%Y %H:%M:%S
date +%d/%m/%Y-%H:%M:%S
touch serverLog-`date +%d/%m/%Y-%H:%M:%S`.log
touch serverLog-`date +%d%m%Y-%H%M%S`.log
ls -la
date
hwclock 
hwclock ; date
hwclocl --help
hwclock --help
timedatectl 
timedatectl set-timezone Asia/Singapore 
date
timedatectl 
timedatectl set-timezone America/New_York 
timedatectl 
timedatectl set-timezone UTC 
timedatectl 
timedatectl set-timezone Europe/Warsaw 
timedatectl 
timedatectl list-timezones 
timedatectl set-ntp no
timedatectl 
timedatectl set-ntp yes
timedatectl 
systemctl status chronyd
systemctl status ntpd
cd
chronyc sources
vi /etc/chrony.conf 
chronyc sources
rtcsync
clear
systemctl stop chronyd
dnf install ntpd
dnf install ntp
dnf provides "*ntpd"
dnf provides "*ntp"
dnf provides "*ntpq"
dnf repolist all
vi /etc/chrony.conf 
chronyc sources
systemctl start chronyc
systemctl start chronyd
chronyc sources
cat /etc/services |wc -l
cat /etc/services | grep -i ntp
cat /etc/services | grep -i nfs
clear
cat /etc/services | grep -i nfs
cat /etc/services | grep -i samba
cat /etc/services | grep -i winbind
cat /etc/services | grep -i ssh
history
history | awk '$1 > 113' | cut -c 8- > git/lfs301_Jun/day1-history.md 
