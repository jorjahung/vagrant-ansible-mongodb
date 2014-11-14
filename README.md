First, pull the submodule and update it:

      git submodule init
      git submodule update

If you want to have a Vagrant VM with MongoDB locally:

      vagrant up

If you want to run the playbook on a host. First change the host file (you can see an example in the hosts folder), then run

      ansible-playbook playbook.yml -i ./hosts/mongodb