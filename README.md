Ansible Role: Couchbash
=========

This role is used for install NoSQL database system [Couchbase Server](https://www.couchbase.com/)

## Requirements

Make sure these requirements need before the installation

| **Items**      | **Details** |
| ------------------| ------------------|
| Operating system | CentOS7.x Ubuntu18.04|
| Python version | Python2  |
| Python Components |    |
| Runtime |  |


## Related roles

This Role does not depend on other role variables in syntax, but it depend on other role before

```
  roles:
    - {role: role_common, tags: "role_common"}
    - {role: role_template, tags: "role_couchbase"}
```


## Variables

The main variables of this Role and how to use them are as follows:

| **Items**      | **Details** | **Format**  | **Need to assignment** |
| ------------------| ------------------|-----|-----|
| template_applications | True, False | Boolean | No |

notes: 

1. ×××××××
2. ×××××××

## Example

```
- name: Memcached
  hosts: all
  become: yes
  become_method: sudo 
  vars_files:
    - vars/main.yml 

  roles:
    - {role: role_common, tags: "role_common"}
    - {role: role_cloud, tags: "role_cloud"}
    - {role: role_template, tags: "role_template"}
```

## FAQ

1. What versions does Couchbase include?
Couchbase Server is available in several editions: enterprise, community, and open source.

2. Is community edition free?
Free, but sell, license, sublicense, distribute, offer or provide the Community Software on a standalone basis  
refer to [COUCHBASE, INC. COMMUNITY EDITION LICENSE AGREEMENT](https://www.couchbase.com/community-license-agreement)
