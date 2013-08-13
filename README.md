openvzpackages
==============

centos6 binaries of libvirt compiled with openvz support


INSTALL OPENVZ
==============

wget -P /etc/yum.repos.d/ http://ftp.openvz.org/openvz.repo

rpm --import http://ftp.openvz.org/RPM-GPG-Key-OpenVZ

yum install -y vzkernel vzctl vzquota

reboot to boot into openvz kernel

INSTALL libvirt with openvz support
==============
git clone https://github.com/ianjw11/openvzpackages.git

cd openvzpackages

yum localinstall -y *.rpm
