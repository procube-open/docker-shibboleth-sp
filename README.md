
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
If you failed to build shibboleth-SP, check the version of softwares specified in the beginning of Dockerfile. 


## debug

何か書く

# DEMO

refer to the test directory, and read [README.md](/test/README.md)

# Note

(書くべきこと何かあるかな

# Author


* Teruyuki Mishima
* procube
* website: https://www.procube.info


