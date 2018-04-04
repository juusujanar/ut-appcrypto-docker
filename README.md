# Docker for Applied Cryptography course

This is a Ubuntu 16.04 based Docker image, that includes Python 2.7 with required dependencies that are used in Applied Cryptography course in University of Tartu.

Included dependencies:
* dumpasn1
* python-crypto
* python-pyasn1

Updated applications: 
* openssl


## How to use?

#### Step 0 - Have Docker installed
MacOS: `brew cask install docker` or [here](https://docs.docker.com/docker-for-mac/install/)   

Linux: [Ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/)/[Debian](https://docs.docker.com/install/linux/docker-ce/debian/)/[CentOS](https://docs.docker.com/install/linux/docker-ce/centos/)   

Windows: [Check here](https://docs.docker.com/docker-for-windows/install/)

#### Step 1 - Run the Docker image
Use your course repo folder between quotation marks, leaving in `:/data` part.

On MacOS: 
`docker run -it -v "/Users/user/Documents/git/appcrypto:/data" janarj/appcrypto`  
On Linux:
`docker run -it -v "/home/user/appcrypto:/data" janarj/appcrypto`  
On Windows:
`docker run -it -v "C:\Users\user\Documents\appcrypto:/data" janarj/appcrypto`  

## Advanced: If you want to build it yourself

#### Step 1 - Clone the repository 
`git clone https://github.com/juusujanar/ut-appcrypto-docker.git`

#### Step 2 - Build the Docker image
You may need to include sudo for Docker commands on Linux.  
`cd ut-appcrypto-docker`  
`docker build -t appcrypto .`
