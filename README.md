# Installing tools and programs required for this project:

1. Create a folder project
`cd ~` // go to your user path
`mkdir project` // create a folder
`cd project` // move to inside folder

1. Updating system urls
`sudo apt-get update`

1. vim
`sudo apt install vim`

1. Installing basic programs
`sudo apt-get install vim git wget

1. Installing `mongodb`

	1. get the key
`wget -qO - https://www.mongodb.org/static/pgp/server-4.4.asc | sudo apt-key add`
	1. Create a liste file for mongo
`echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-4.4.list`

	1. Update package
`sudo apt-get update`

	1. Start Mongodb process
`sudo systemctl start mongod`

	1. Check if running
`sudo systemctl status mongod`

:::info
if python 3.11 is required:
1. `sudo add-apt-repository ppa:deadsnakes/ppa -y`
1. `sudo apt update`
1. `sudo apt install python3.11`
:::

1. Installing anaconda from [here](https://repo.anaconda.com/archive/Anaconda3-2024.02-1-Linux-x86_64.sh)
`chmod +x Anaconda3-2024.02-1-Linux-x86_64.sh`
`./Anaconda3-2024.02-1-Linux-x86_64.sh`
> Restart the operating system

```python
# 1. Installing pip
# `sudo apt install python3-pip -y` 
> Around 83 Mb.
```

1. Installing pymongo
`sudo pip3 install pymongo`

1. Installing jupyter notebook
`pip3 install jupyterlab`

1. Installing jupyter core
`sudo apt install jupyter-core`

if this error occurs:
`pip3 install --upgrade setuptools`

1. Install jupyter notebook
`pip3 install notebook`


1. Clonando reposytorio
`git clone https://github.com/mjacker/bigdata.git`

1. cd into repositoryo
`cd bigdata`

1. Run Jupyter lab
`python3 -m jupyterlab .`


# How to run this project.

1. Run the ipynb file
2. Change password and username
* client = pymongo.MongoClient('mongodb+srv://group2:(PASSWORD)@cluster0.7cwggsq.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0')

