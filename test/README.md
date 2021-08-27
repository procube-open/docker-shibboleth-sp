# Demo (test)

You can test the shibboleth-SP container with growi, nginx and some softwares.


# Installation

Clone this .

# Usage

## 1
 
Build the shibboleth-SP image,following [README.md](../README.md) ,and name the image "pershib".
If you named it another name, edit docker-compose.yml .

## 2

Build the growi image.(Dockerfile is in test/editedgrowi) and name the image "editedgrowi".
If you named it another name, edit docker-compose.yml

## 3

Pull the images of mongo:4.4 and procube/nginx.
Probably, you can use another version of mongo (edit docker-compose.yml )

## 4

Prepare fullchain.pem privkey.pem, and edit docker-compose.yml

Edit nginx.conf(in test/reverseproxy).

## 5 

'docker-compose up'.

## 6

Make SPmetadata.
For example, you can download SPmetadata by accessing https://EXAMPLE.com/Shibboleth.sso/Metadata.
'EXAMPLE' is example.

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

