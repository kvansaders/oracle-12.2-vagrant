# oracle-12.2-vagrant
A vagrant box that provisions Oracle Database 12c release 2 automatically, using Vagrant, an Oracle Linux 7.3 box and a shell script.

## Prerequisites
1. Install [Oracle VM VirtualBox](https://www.virtualbox.org/wiki/Downloads)
2. Install [Vagrant](https://vagrantup.com/)

## Getting started
1. Clone this repository `git clone https://github.com/totalamateurhour/oracle-12.2-vagrant`
2. Change into version folder (12.2.0.1)
3. Download the Oracle Database 12c release 2 binaries linuxx64_12201_database.zip
from [http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index.html](http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index.html)
4. Run `vagrant up`
    5. The first time you run this it will provision everything and may take a while. Ensure you have a good internet connection!
6. Connect to the database.
7. You can shut down the box via the usual `vagrant halt` and the start it up again via `vagrant up`.

## Connecting to Oracle
* Hostname: `localhost`
* Port: `1521`
* SID: `ORCLCDB`
* PDB: `ORCLPDB1`
* OEM port: `5500`
* All passwords are `password`.

## Acknowledgements
Based on @steveswinsburg's work here: https://github.com/steveswinsburg/oracle12c-vagrant

## Other info

* If you need to, you can connect to the machine via `vagrant ssh`.
* You can `sudo su - oracle` to switch to the oracle user.
* The Oracle installation path is `/opt/oracle/`
* On the guest OS, the directory `/vagrant` is a shared folder and maps to wherever you have this file checked out.

## Known issues


