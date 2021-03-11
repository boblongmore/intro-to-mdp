# intro-to-mdp

## Working with Pyang 

pyang -f tree 

pyang -f 


## Working with Yangsuite
### installing yangsuite in the Programmability Foundations Lab

Reserve an instance of the [Programmability Foundations Lab](https://www.wwt.com/lab/programmability-foundations-lab)

On the jumphost, install python for windows ([Version 3.8](https://www.python.org/ftp/python/3.8.8/python-3.8.8-amd64.exe) or lower, python 3.9 is not yet supported)

Use pip to install yangsuite core: `pip install yangsuite[core]`

To start yangsuite, simply type: `yangsuite`

You'll be taken through setup wizard.
Specify a directory, I chose `./yangsuitedata`

Leave the default port of 8480

You can allow remote access, but you don't need to in this lab.
Enter in the superuser credentials and your email address.

Open up a browser on the jumphost and go to <http://localhost:8480>

Accept the EULA and you should be at the yangsuite home screen.


### getting started with yangsuite

To get started we need to some setup:
1. Add device(s)
2. Add Yang model repository
3. Create Yang model set

To add a device go to setup -> Device Profiles, create a new device.
* Populate IP address and credentials, under the NETCONF section, 
* enable NETCONF and click to bypass SSH Key validation
* Save and check connectivity

To create a Yang model repository go to setup -> Yang files and repositories
* Click new repository and give it a name
* You can download the models from the device by clicking on NETCONF, selecting the device profile, then clicking the get schema button
* filter and select, or select all modules to download

To create a Yang model set, got to setup -> Yang module sets
* click create new yang set
* add a name and choose to associate the Yang repository created earlier
* choose which modules to add to the module set



