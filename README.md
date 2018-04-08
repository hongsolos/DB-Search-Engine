# Search Engine

CSCE 470 Team project - Solr Search Engine

## Authors

* **Juan Duran** - *Contributor* - [Juan's Github](https://github.com/hueytlatoani)
* **Anh Nguyen** - *Contributor* - [Anh's Github](https://github.com/harryluffy)
* **Han Hong** - *Contributor* - [Hong's Github](https://github.com/hongsolos)


## Background

As a continuation of Data Crawler project, the goal is to index of the crawled data into a search database. For this project, Solr will be used as the main building block and almost 90% will be done in Java.

## Installation Instructions

What things you need to install the software and how to install them

Installation of packages required for Solr
```
sudo apt-get update && apt-get upgrade -y
sudo apt-get install python-software-properties
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
wget http://www.us.apache.org/dist/lucene/solr/6.0.1/solr-6.0.1.tgz
tar xzf solr-6.0.1.tgz solr-6.0.1/bin/install_solr_service.sh --strip-components=2
sudo ./install_solr_service.sh solr-6.0.1.tgz
```

Getting Started & Accessing the Interface
```
sudo su - solr -c "/opt/solr/bin/solr create -c gettingstarted -n data_driven_schema_configs"
http://[YOUR_IP]/solr/
```

## Timeline

* 02/19/2018 - Project Initiated
* 03/12/2018 - Indexing and overall setup
* 03/13/2018 - Database building
* 03/18/2018 - Field Test

## Built With

* [Solr 7.2.1](http://lucene.apache.org/solr/) - Search Engine Platform

## Acknowledgments

* [How To Forge](https://www.howtoforge.com/tutorial/how-to-install-and-configure-solr-on-ubuntu-1604/) Solr tutorial
* Steam


