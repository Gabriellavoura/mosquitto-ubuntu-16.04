# mosquitto-ubuntu-16.04
How to install mosquitto broker on ubuntu 16.04.

## Update - (28/06/2016)

#### 1º - Add the mosquitto-dev PPA to your repositories list :

  > $ sudo apt-add-repository ppa:mosquitto-dev/mosquitto-ppa
  
  > $ sudo apt-get update
  
###### _If the command “apt-add-repository” is not recognised, it can be installed with:_

   > $ sudo apt-get install python-software-properties
   
#### 2º - Install mosquitto from PPA :

   > $ sudo apt-get install mosquitto
  
###### _Now it's possible run the command below, in the terminal, to check if is everything ok._
  
   > $ mosquitto -v
 
###### _If everything is ok, you'll see something like this:_
 
 ```
 mosquitto version 1.4.10 (build date Thu, 25 Aug 2016 15:32:03 +0100) starting
 Using default config.
 Opening ipv4 listen socket on port 1883.
 Error: Address already in use
```
 

#### 3º - Install mosquitto-clients from PPA :
   > $ sudo apt-get install mosquitto-clients
  
  _Now you can run commands like mosquitto_pub and mosquitto_sub._
  
  _**That's all folks!**_
  
#### Offical Documentation:

For a Getting started guide and API docs, check out this docs!

+ Official mosquitto docs: https://mosquitto.org/documentation/
+ Official PPA: https://launchpad.net/~mosquitto-dev/+archive/ubuntu/mosquitto-ppa
+ Command mosquitto_pub: http://manpages.ubuntu.com/manpages/wily/man1/mosquitto_pub.1.html 
+ Command mosquitto_sub: http://manpages.ubuntu.com/manpages/wily/man1/mosquitto_sub.1.html 
+ Command mosquitto: http://manpages.ubuntu.com/manpages/wily/man8/mosquitto.8.html
+ mosquitto-clients: https://launchpad.net/ubuntu/wily/+package/mosquitto-clients

