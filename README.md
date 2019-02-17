# Trantek - A simple dataanalytics platform for engineers

Version 0.9

This is a setup of an analytics platform for the NordicWay II project. The platform supports data storage, analysis and presentation of results. The project relies on external queing services like the NordicWay II interchange or equals for data ingestion. Hence the Docker stack does not contain queuing functionality.

The setup is for running on a that the user uses SSH to logonto and create tunnels. All ports are only exposed to the local host for security reasons. Hence all data on the move is moved in an encryptes SSH tunnel. 

## Docker config

The Docker compose functionality is used to create a stack of applications that together becomes the Trantek analytics platform. All containers except for PostgreSQL uses volumes for mounting the data. After practical testing on geographic data mocing the storage for the database is moved to SSD storage on the server (/media/ssd/docker_PG11). The rest works like magic :) Just go into the logfiles of trantek-jupyter to find the access token. 

## Port and web access after using an ssh-tunnel
- Jupyter lab: **http://localhost:7002/lab**
- Jupyter notebook **http://localhost:7002**
- NodeRed: **http://localhost:7001**
- Postgresql: 7004 at localhost - 5432@ trantek-postgres
- Mongodb: 7003 at localhost 
- Mongodb express **http://localhost:7005**
- PGAdmin4 **http://localhost:7006**

## Default passwords 
(for this single user engineering stack localhost security is used)

PostgreSQL
- user: trantek
- password: svv123svv

PGAdmin 4
- user: trantek@npra.io
- password: svv123svv

To enable per application security go into the Docker-compose file and configure therafter.

20190217 Tomas Levin
