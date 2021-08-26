# Demo (test)

You can test the shibboleth-SP container with growi, nginx and some softwares.


# Installation

clone this directory.

# Usage

## 1

build the shibboleth-SP image, and name the image "pershib".
If you named it another name, edit docker-compose.yml

## 2

build the growi image.(Docker file is in test/editedgrowi) and name the image "editedgrowi".
If you named it another name, edit docker-compose.yml

## 3

pull the images of mongo:4.4 and procube/nginx.
Probably, you can use another version of mongo (edit docker-compose.yml )

## 4

Prepare fullchain.pem privkey.pem, and edit docker-compose.yml

## 5 

'docker-compose up'.

## 6

make SPmetadata.
for example, you can download SPmetadata, 
if you access https://EXAMPLE.com/Shibboleth.sso/Metadata.
EXAMPLE should be edited.

## 7

Upload the metadata to IDP.
You may have to edit SP-metadata before uploading.

## 8

Access https://EXAMPLE.com/secure .

If you can login, the test is complete.

# Author

* Teruyuki Mishima
* procube
* website: https://www.procube.info

