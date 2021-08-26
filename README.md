
#  docker-shibboleth-sp (container of shibboleth-SP)

docker-shibboleth-sp is a container of shibboleth-SP.

You can run shibboleeth-SP in a docker container.

( nginx-shibboleth連携図.pngか何かを適当に載せるかも


# Installation

## 1

prepare server.crt and 0701IDPmetadata.xml


## 2

edit shibboleth2.xml and supervisord.conf

## 3

build the Dockerfile.
If you failed building shibboleth-SP, check the version of softwares specified in the beginning of Dockerfile. 


## debug

Once you build image, you don't need to rebuild(if you use docker-compose.yml in 'test' directory).
When you 'docker-compose up', container automatically reload server.crt, 0701IDPmetadata.xml, shibboleth2.xml and supervisord.conf



# DEMO

refer to the test directory, and read [README.md](/test/REDME.md)

# Note

(書くべきこと何かあるかな

# Author


* Teruyuki Mishima
* procube
* website: https://www.procube.info


