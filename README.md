Customization of Kapacitor alerts
=================================

This repository provides a demo for my answer to the Stackoverflow question [How to define Alerts with exception in InfluxDB/Kapacitor][so:op].

Requirements
------------

* Docker
* docker-compose
* a web browser

Usage
-----

1. Clone this repository
   ```
   git clone https://github.com/mwmahlberg/so-influxdb-sideload.git
   cd so-influxdb-sideload
   ```
2. Pull the required Docker images
   ```
   docker-compose pull
   ```
3. Start the containers
   ```
   docker-compose up [-d]
   ```
4. Wait a few minutes and then visit http://localhost:8888/sources/0/alerts

Caveats
-------

The alert flaps because the chronograf database gets created. #helpwanted

[so:op]: https://stackoverflow.com/q/56972799/1296707
