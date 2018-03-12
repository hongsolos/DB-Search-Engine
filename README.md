# Search Engine

CSCE 470 Team project - Solr Search Engine

## Authors

* **Juan Duran** - *Contributor* - [Juan's Github](https://github.com/hueytlatoani)
* **Anh Nguyen** - *Contributor* - [Anh's Github](https://github.com/harryluffy)
* **Han Hong** - *Contributor* - [Hong's Github](https://github.com/hongsolos)


## Background

This project's goal is to build a data crawler program to retrieve data from Steam website. These data will be kept in our form of a database, and will be used by another program to build a search engine. 

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

#### Review Data Crawling
First, all review urls from crawled products must be extracted and exported to a text file using split_review_url script in script folder. Once generated a url text file, we can then call scrapy to start crawling reviews data.
```
scrapy crawl reviews -o review.jl ...
```

## Timeline

* 02/05/2018 - Project Initiated
* 02/18/2018 - Project Proposal Submitted
* 02/18/2018 - Data Crawler Completed - Data Retrieved

## Built With

* [Python 3.6](https://www.python.org/) - Python Development and Environment

## Acknowledgments

* Big thanks to [ANDRE PERUNICIC](https://github.com/prncc/steam-scraper) for making the crawler available for reference. 
* Scrapy Tool
* Steam


