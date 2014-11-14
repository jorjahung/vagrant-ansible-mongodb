First, pull the submodule and update it:

      git submodule init
      git submodule update

If you want to have a Vagrant VM with MongoDB locally:

      vagrant up

If you want to run the mongodb setup playbook on a host. First change the host file (you can see an `mongodb`example in the hosts folder), then run

      ansible-playbook playbook.yml -i ./hosts/mongodb

If you want to run the uptime setup playbook, set the correct host (`mongodb` is given as an example), change the username and password in `uptime.yml`:
      ansible-playbook uptime.yml -i ./hosts/mongodb