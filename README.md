
# forti-srl

SRLinux EVPN Fabric with Integrated Fortigate

The steps to deploy the lab are:

Arrange a Linux host with 64Gig Memory - 32 vCore CPU ( Preferably Ubuntu )

1-) Install Docker  --> https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

2-) Install Containerlab --> curl -sL https://containerlab.dev/setup | sudo -E bash -s "all"

3-) Load FortiOS image to docker images --> docker load -i fortios-7.6.0.tar

4-) Pull this git repo to the local ubuntu machine --> git clone https://github.com/kkayhan/forti-srl.git

5-) Go to the git directory on the local machine and deploy the lab "clab -t forti-srl.yaml deploy "

Then you can ssh the nodes.

ssh fortigate
ssh spine
ssh leaf1 

