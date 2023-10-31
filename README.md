Ansible Collection - diademiemi.foreman
========================================
Documentation for the collection foreman.

This collection is NOT meant as a replacement for the upstream Foreman/Satellite Ansible collection. This is meant as a simple way to deploy a test environment for Foreman/Katello.

This collection will deploy a Foreman/Katello server and configure it for PXE booting clients. The default variabes will use the network the server is connected to as the PXE network. The default username and password for the Foreman/Katello server and PXE clients is `admin` and `admin` by default. Check the variables for every role for more information.

The default variables will produce a VERY insecure environment, if you want to use this, please change the variables to something more secure. This was made so I could practice for the EX403 exam.

This collection is tested on the following operating systems:
- CentOS Stream 8

But should work on:
- Ubuntu 20.04
- Debian 11

The Katello parts are only supported on CentOS Stream 8. Be aware that some defaults might assume CentOS Stream 8. (For example, the default hostgroups refer to content views)

Contents 
========

Roles
------
Role | Description | CI Status
--- | --- | ---

[diademiemi.foreman.install](./roles/install/) | Set up dependencies and run Foreman installer | N/A
[diademiemi.foreman.smart_proxy](./roles/smart_proxy/) | Set up Smart Proxy (Capsule server) | N/A
[diademiemi.foreman.configure_katello](./roles/configure_katello/) | Configure Katello resources | N/A
[diademiemi.foreman.configure](./roles/configure/) | Configure Foreman resources| N/A
[diademiemi.foreman.install_capsule](./roles/install_capsule/) | Install Capsule server (NOT FINISHED) | N/A

Click on the role to see the README for that role.  

