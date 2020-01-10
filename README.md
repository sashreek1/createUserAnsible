# createUserAnsible
An Ansible program to create a new user in the system
  
# Steps to use
* Clone this repository
* Run this command ``` python -c 'import crypt; print (crypt.crypt("<your password>", "$1$SomeSalt$"))'```. The output of this command is your password
* After this run the yml file with this command ```ansible-playbook createUser.yml --become --ask-become-pass```
* It will then ask you for ```BECOME password:``` where you have to type in the root password
* when asked for username ```What is your username?: ``` write in the username of the user you want to create
* when asked for username ```What is your password?:``` write in the password that was created in step 2
* With this your new user has been created

### you may follow the steps from this asciinema as well : https://asciinema.org/a/ZcCadFDTZzawrRhegd9mstiqM

Here is a screenshot of the new user (logged in):
