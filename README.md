# vagrant-Docker-Infrakit

This repo contains the [Vagrant](https://www.vagrantup.com) box which in turn contains a [Docker Infrakit](https://github.com/docker/infrakit) installation. It is built for testing purposes only, so the only provider for this box is [virtualbox](https://www.virtualbox.org).

You can run and ssh this box by executing the commands below:
```
mkdir Infrakit_test
cd Infrakit_test
vagrant init ivaquero/Docker_Infrakit
vagrant up --provider virtualbox
vagrant ssh

# You will find that infrakit tools are installed at 
# /go/src/github.com/docker/infrakit or you can access them
# via the environment variable INFRAKIT_PATH

cd $INFRAKIT_PATH # This takes you directly to infrakit main repo
```

This box is hosted on [Atlas by Hashicorp](https://atlas.hashicorp.com/ivaquero/boxes/Docker_Infrakit).
