# portia

Portia aims to automate a number of techniques commonly performed on internal network penetration tests after a low privileged account has been compromised
- Privilege escalation
- Lateral movement
- Convenience modules

Portia is a genus of jumping spider that feeds on other spiders - known for their intelligent hunting behaviour and problem solving capabilities usually only found in larger animals

## Videos (Will be adding more soon)  
Video that shows privilege escalation via impersonation tokens and running of post exploitation modules  
https://asciinema.org/a/45ry3g26devqcabpugwyz4to5  

## Dependencies

```
apt-get update
apt-get install -y autoconf automake autopoint libtool pkg-config freetds-dev
pip install pysmb tabulate termcolor xmltodict pyasn1 pycrypto pyOpenSSL dnspython netaddr python-nmap
cd /opt
git clone https://github.com/CoreSecurity/impacket
python setup.py install
cd /opt
git clone https://github.com/libyal/libesedb.git && cd libesedb
./synclibs.sh
./autogen.sh
cd /opt
git clone https://github.com/csababarta/ntdsxtract && cd ntdsxtract
python setup.py install
pip install git+https://github.com/pymssql/pymssql.git
cd /opt
git clone https://github.com/volatilityfoundation/volatility && cd volatility
python setup.py install
cd /opt
git clone https://github.com/SpiderLabs/portia
```
