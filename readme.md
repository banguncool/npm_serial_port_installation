# npm serialport installation

Link: https://www.npmjs.com/package/serialport

## Windows
Normally you can install Serialport by 
```sh
$ npm i serialport
```
But if you have problem installation try to install **windows-build-tools**\
Open cmd with administrator
```sh
$ npm install -g windows-build-tools
```
It will take long time, be patien. Until you found this message
```
Starting installation...
Launched installers, now waiting for them to finish.
This will likely take some time - please be patient!

Status from the installers:
---------- Visual Studio Build Tools ----------
Successfully installed Visual Studio Build Tools.
------------------- Python --------------------
Python 2.7.15 is already installed, not installing again.

Now configuring the Visual Studio Build Tools..

All done!
```
Then you now you can install normally
```sh
$ npm i serialport
```

## Ubuntu failed to install because make is not foud
Solustion install make
```sh
$ sudo apt-get update
$ sudo apt-get install -y make
```
### Other solusion install different version NodeJS, maybe versio 16 is fine.
### If still not fix then try to remove package-lock.json and node_modules in the directory


## Ubuntu
If you are using modbus-serial, try install individually with
```sh
$ npm i modbus-serial --unsafe-perm
```

or if you are using serialport
```sh
$ npm i serialport --unsafe-perm
```

then install all other dependecies

```sh
$ npm install
```
