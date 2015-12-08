# znc-baseserver
An ansible setup to create a multi-user znc server

## Why?
Needed a simple method to setup a znc server that a group of ppl can use and not worry about setting
up their own server & configuring everything. Also wanted to use this as a reason to learn some ansible.

## How?
1. Create a VPS server
2. Create username znc
3. sudo apt-get insstall python-apt python-pycurl
4. If you are installing locally, edit /etc/ansible/hosts and add the below line
  * ```localhost ansible_connections=local```
5. Run the playbook. This will install znc
6. Run ```znc --makepass``` & edit the znc-setup.yml file with the respective data
7. Run setup again

YES, the above is not the cleanest and it sucks in many ways. But it worked on the first run. I will fix
it more as and when i get some time. Any contributions and criticisms are welcome

##Anything Else?
Have some bugs here and there. Check the issues list.
