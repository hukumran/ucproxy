apt-get update && apt-get -y upgrade
apt-get install -y build-essential nano
wget --no-check-certificate https://pkgs.fedoraproject.org/repo/pkgs/3proxy/3proxy-0.7.tgz/b2a7b643d3e3d348ce97ed094075fc53/3proxy-0.7.tgz
tar xzf 3proxy-0.7.tgz
cd 3proxy-0.7
make -f Makefile.Linux
cd src
mkdir /etc/3proxy/
mv 3proxy /etc/3proxy/
cd /etc/3proxy/
wget --no-check-certificate https://github.com/benjamin74/3proxy/raw/master/3proxy.cfg
chmod 600 /etc/3proxy/3proxy.cfg
cd /etc/init.d/
wget --no-check-certificate https://raw.github.com/benjamin74/3proxy/master/3proxyinit
chmod  +x /etc/init.d/3proxyinit
update-rc.d 3proxyinit defaults
