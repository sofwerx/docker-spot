# **Apache Spot (Incubating)**   

Apache Spot is open source software for leveraging insights from flow and packet analysis. It helps enterprises and service providers gain insight on their compute environments through transparency of service delivery and identification of potential security threats or attacks happening among resources operating at cloud scale.

While current threat intelligence tools help, identifying unknown threats and attacks remains a challenge. Apache Spot provides tools to accelerate companies’ ability to expose suspicious connections and previously unseen attacks using flow and packet analysis technologies. 
<br><br>

## **Project Structure**

Each project sub folder is intended to be the source for the [Apache Spot organization](https://hub.docker.com/u/apachespot/) on the [Docker Hub](https://docs.docker.com/docker-hub/)

### *spot-dev*

The spot-dev image is a full development virtual machine that contains the following:

* Development Dependencies
* Working CDH distribution
* links to synthetic data

### *spot-demo*

the spot-demo is the source for apachespot/spot-demo

## **Prerequisites**

* docker
* docker-compose

## **Build**

This is an optional step that forces a build:

    docker-compose build

## **Run**

It should be as easy as:

    docker-compose up -d

Now try to open this URL in your browser:

- http://localhost:8889

Navigate to the ipynb/ folder by clicking on it.

Under the dns/, flow/, and proxy/ folders there are `*/Edge_Investigation.ipynb` and `*/Thread_Investigation.ipynb` for each. Open these up and click Run to start running those notebooks.

Now you should be able to visit the web pages for each by directly on each:

- http://127.0.0.1:8889/files/ui/flow/suspicious.html#date=2016-07-08

## **Needs**

* Automation scripts to download code from git repository at build time
* Automated builds
