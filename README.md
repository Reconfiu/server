# ReckonFIU - Server 

> Python server running on docker container, by running our server in a docker container we can easily change, upgrade and scale our server. In order to use docker, we install `docker-engine` and `docker-compose`. In case of Mac and Windows `docker-machine` with `virtualbox` must also be installed.   

## Requirements:

* **Python 2.7.10**
    ```
    For Linux run command:
        $ sudo apt-get install python
    Windows:
        Download from https://www.python.org/downloads/release/python-2711/
    Mac OS 
        Download from https://www.python.org/downloads/release/python-2711/
    ```
    
* **Docker 1.12.6**
    ```
    1. Linux: https://docs.docker.com/engine/installation/linux/
    2. Windows: https://docs.docker.com/docker-for-windows/
    3. Mac OS: https://docs.docker.com/docker-for-mac/
    ```
    
* **Docker-compose 1.10.0** 
    ```
    Follow these steps: https://docs.docker.com/compose/install/
    ```
    
* **Docker-machine (Windows/Mac users only)** For docker-machine to run we also need virtualbox. 
    ```
    docker-machine: https://docs.docker.com/machine/install-machine/
    virtualbox: https://www.virtualbox.org/wiki/Downloads
    ```
    After installing docker-machine create a docker virtual machine
    ```
    $ docker-machine create --driver virtualbox default
    $ eval "$(docker-machine env default)"
    ```
    
    Full guide: https://docs.docker.com/machine/get-started/
* **Important Note**
    To check if docker, docker-compose and python are installed run these commands
    ```
    $ docker-compose -v
    $ docker -v
    ```
## Setup:
 To set up our server with docker after all dependencies have been installed follow these steps:
 
 * **All platforms** 
    ```
    $ git clone https://github.com/reckonfiu/server.git
    $ cd server
    $ docker-compose up
    ```
    
 * **Note: for linux you might have to do**
    ```
    $ sudo docker-compose up
    ```
    
 In the browser go to `localhost:5000` "Hello World";   
    
    
