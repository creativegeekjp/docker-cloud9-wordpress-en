Cloud9 v3 Dockerfile with Wordpress installed
=============

This repository contains Dockerfile of Cloud9 IDE for Docker's automated build published to the public Docker Hub Registry.
Together with Wordpress v 4.5, ready to deploy

# Installation

## Install Docker.

Download automated build from public Docker Hub Registry: docker pull creativegeekjp/docker-c9wordpress-en

## Usage

The simplest way to run this is (Port 80: Worpdress, Port 8080: Cloud9 IDE)

    docker run -it -d -p 8080:80 -p 80:8080 -e PASS=c9pass creativegeekjp/docker-c9wordpress-en
    
You can add a workspace as a volume directory with the argument *-v /your-path/workspace/:/workspace/* like this :

    docker run -it -d -p 8080:80 -p 80:8080 -e PASS=c9pass -v /your-path/workspace/:/workspace/ creativegeekjp/docker-c9wordpress-en
    
