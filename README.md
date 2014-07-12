#modulename

####Table of Contents

1. [Overview](#overview)
2. [Module Description - What the module does and why it is useful](#module-description)
3. [Setup - The basics of getting started with [Bamboo]](#setup)
    * [What [Bamboo] affects](#what-[modulename]-affects)
    * [Setup requirements](#setup-requirements)
    * [Beginning with [Bamboo]](#beginning-with-[Bamboo])
4. [Usage - Configuration options and additional functionality](#usage)
5. [Reference - An under-the-hood peek at what the module is doing and how](#reference)
5. [Limitations - OS compatibility, etc.](#limitations)
6. [Development - Guide for contributing to the module](#development)

##Overview

Installs Bamboo on a server, with a local Postgres instance. By default, you get Bamboo 5.5.1, Postgres 9.3 and Java 1.7.

##Module Description

This module will install Bamboo 5.5 on your server. It also installs Postgres 9.3, and creates a database and user for you. Currently, it does not configure Bamboo to point to the database - you will need to do that yourself.

##Setup

###What [Bamboo] affects

* Java JDK
* Postgresql

###Setup Requirements

 This module requires the Postgresql module. Also, don't define your bamboo user separately, use this module to do it.
 
###Beginning with [Bamboo]  

Download the module, and at a minimum, set the following parameters:
* password
* pgpass

##Reference


##Limitations

This module has only been tested on Centos 6.5, but it should be ok with Ubuntu too.

At the moment, this module will not setup any additional Bamboo addons. I hope to add this functionality in the future!

##Development

Pull requests are welcome. Please use a feature branch.
