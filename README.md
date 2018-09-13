# Hyperledger-installation
Description of the installation of Hyperledger for the Block-chain Systems Architecture class

Before we start, we need to verify that we have the following pre-requisites installed:
1) git
2) curl
3) python
4) node
5) Go
6) Docker and Docker Compose
Next we downoad and install Hyperledger Fabric. 

To finally launch the network, we follow the following steps:
1) cd <work directory>
2) Generate the required certificates and articates for your first network
  $ ./byfn.sh -m generate
  # ./byfn.sh is a fully annotated script that leverages these Docker images to quickly bootstrap a Hyperledger fabric network. 
3) To see the generate certificates use the following command:
  $ cd crypto-config
  $ ls
4) Create your first network using the following command
  $ ./byfn.sh -m up
5) Check the generates images and running containers using the following command:
  $ docker images
  $ docker ps
6) To bring down the created network executed the following command
  $ ./byfn.sh -m down
7) You can check the created images have been removed using the following:
  $ docker images




