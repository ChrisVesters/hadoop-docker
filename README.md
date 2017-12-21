Overview
========

This repository contains all the required Docker files to create a Hadoop Cluster.

How To Use
==========

Create the base Hadoop Docker Image:

	docker build general/ -t hadoop:2.9.0

Deploy the cluster with Docker Compose:

	docker-compose up -d

To destroy the cluster:

	docker-compose down

Currently the created cluster consists of a namenode and a single datanode.
Adding the '--scale datanode=5' is currently not supported due to hostname and port binding issues.
