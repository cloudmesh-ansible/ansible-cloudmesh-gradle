Ansible role which installs [Gradle](http://www.gradle.org/)

#### Requirements & Dependencies
- Ubuntu
- tested on ansible 2.0.1.0


#### Variables

```yaml
gradle_version: "2.13"             # The version of gradle to install
gradle_install_path: "/usr/local"  # Path where to install gradle
```

#### Example

```yaml
--- 
- name:	Install gradle on monitor nodes as root
  hosts: monitornodes
  remote_user: root
  become: yes
  roles:
    - gradle
```

#### Author
Hrushikesh Dhumal (hrushikesh.dhumal@gmail.com)
