### Table of Contents
***
1. [General Info](#general-info)
2. [Technologies](#technologies)
3. [Installation](#installation)
4. [License](#License)
5. [Ressources](#Ressources)

### General Info
***
Hello World!

My name is Mickaël alias sodbaveka.
I created this repository as a lab to discover git, gitHub, Bash, Python and Ansible.

My project as a learner is to create a python (or bash) script to automate the saving of a wordpress website.
These scripts will be factored into Ansible modules.

Ansible will therefore have the following task:
- TO COMPLETE.

Please feel free to message me if you have any questions.

Bye ;-)

### Technologies
***
A list of technologies used within the project :
* Linux Debian 10.8
* ansible 2.10.5
  * config file = /etc/ansible/ansible.cfg
  * configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  * ansible python module location = /usr/local/lib/python3.7/dist-packages/ansible
  * executable location = /usr/local/bin/ansible
* python version = 3.7.3 (default, Jul 25 2020, 13:03:44) [GCC 8.3.0]

### Installation
***
* Download :
```
$  git clone https://github.com/sodbaveka/WordpressBackupProject.git
```
* Complete the path to utility classes :
  * In /etc/ansible/ansible.cfg, add the library/utils directory to the option 'module_utils'.

* Launch :
```
$ cd ../path/to/the/file
$ ansible-playbook -i inventories/mainInventory.yml -K mainPlaybook.yml 
```

### License
***
* Copyright: (c) 2021, Mickaël Duchet <sodbaveka@gmail.com>
* GNU General Public License v3.0+ (see COPYING or https://www.gnu.org/licenses/gpl-3.0.txt)

### Ressources
***
* https://docs.ansible.com/
* https://ldap3.readthedocs.io/en/latest/
* ‘python for dummies’ :-p 
