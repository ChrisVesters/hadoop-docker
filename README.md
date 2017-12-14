Overview
========

This repository contains all the required Docker files to create a Hadoop Cluster.

How To Use
==========

Create the base Hadoop Docker Image:

	docker build general/ -t hadoop:2.9.0

Deploy the cluster with Docker Compose:

	docker-compose up -d --scale datanode=5

To destroy the cluster:

	docker-compose down


