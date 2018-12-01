# ansible-ubuntu-image

Ansible-playbook that downloads cloud version of ubuntu and starts an instance on openstack.

To use it you must first have devstack stacked, then download the RC file from the horizon dashboard
to get the url to connect it to.
After getting that information, you must enter vars.yml and change the url to the os_auth_url shown on that file.

Such url has the following structure: <ip>/identity/v3.
  
After that, you must start the playbook with:
  ansible-playbook launch.yml
  
