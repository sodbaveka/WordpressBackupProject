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

My project as a learner is to create an Ansible playbook to automate the installation of a wordpress website.

Running this playbook will perform the following actions on your Ansible hosts :
- Install aptitude, which is preferred by Ansible as an alternative to the apt package manager.
- Installation of the required LAMP packages and PHP extensions.
- Creation and validation of a new VirtualHost Apache for the WordPress site.
- Activation of the Apache rewrite module (mod_rewrite).
- Disable the default Apache website.
- Sets the password for the MySQL root user.
- Removal of anonymous MySQL accounts and the test database.
- Creation of a new MySQL database and a user for the WordPress site.
- Configure the UFW parameter to allow HTTP traffic on the configured port (80 by default).
- Download and unpack WordPress.
- Set the correct directory ownership and permissions.
- Define the wp-config.php file using the template provided.

Please feel free to message me if you have any questions.

Bye ;-)

### Technologies
***
A list of technologies used within the project :
* Linux Debian 10.8
* ansible 2.10.8
  * config file = /etc/ansible/ansible.cfg
  * configured module search path = ['/root/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  * ansible python module location = /usr/local/lib/python3.7/dist-packages/ansible
  * executable location = /usr/local/bin/ansible
* python version = 3.7.3 (default, Jul 25 2020, 13:03:44) [GCC 8.3.0]

### Installation
***
* Download :
```
$  git clone hhttps://github.com/sodbaveka/wordpress_installation_with_ansible.git
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
* https://wordpress.org
* ‘python for dummies’ :-p 
