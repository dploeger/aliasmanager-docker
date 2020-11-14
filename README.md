# Aliasmanager

## About the project

The Aliasmanager consists of a Frontend and an API-Server that manages 
specific attributes in an LDAP server.

When integrated in an MTA (like Postfix), these attributes can be used
as aliases for the main E-Mail address.

## Introduction

This repository holds the docker-compose configuration.

The frontend based on [Vuejs](https://vuejs.org) can be found at
https://github.com/dploeger/aliasmanager-client.

The API-Server based on [Nest](https://nestsjs.com) can be found at
https://github.com/dploeger/aliasmanager.

## Usage

To use the aliasmanager, download this repository, copy .env.template
to .env and configure. 
(Check out the [API-Server readme](https://github.com/dploeger/aliasmanager/blob/master/README.md#configuration)
for configurable environment variables)

Additionally, with EXPOSE_PORT you can set the port where the
frontend will be available.

After that, run 

    docker-compose up -d

to start.
