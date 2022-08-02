Fork this repo to your own github account, create the playbook described below, and commit your changes back to your fork.

Given the ansible inventory file `myinventory` create an Ansible playbook that: 

1. Copies the contents of myapi to the destination host in /srv
2. Installs the required python dependencies for myapi
3. Starts the application listening on port 5000 in the background
4. Installs haproxy via yum (or apt)
5. Configure HAProxy to redirect incoming traffic on localhost:80 to localhost:5000 (using the variables frontend\_port and backend\_port in the inventory)
6. Install mysql via yum (or apt)
7. start mysql service
8. Prompt the user for a schema name and create that schema in the mysql database
