## Hands On Labs

- Oracle Code Sydney July 2017

### Installation of Postman

This section will help you deploy the Postman REST Client software that can be used to test the MedRec APIs.
Follow the steps for your operating system as per [Postman Install](https://www.getpostman.com/docs/postman/launching_postman/installation_and_updates)

### Installation of Postman on Ubuntu 16.04

These steps worked to get Postman installed on Ubuntu.

```
sudo wget https://dl.pstmn.io/download/latest/linux64 -O postman.tar.gz
sudo tar -xzf postman.tar.gz -C /opt
rm postman.tar.gz
sudo ln -s /opt/Postman/Postman /usr/bin/postman
```

Then simply run it from within the VirtualBox graphical view:

```
postman
```

It should open a new Postman desktop client in a new window.

* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)

<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center />
<hr />

