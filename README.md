# java-cli-maven-sybase-index

## Description
Creates a small database table
called `dog`. This table, `dog`, has 2 non-clustered
index and has been normalized to 3NF.
All output normally
seen in a terminal will be in `java-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

## Tech stack
- docker-wait
- java
- maven
  - log4j
  - sybase driver

## Docker stack
- maven:3-openjdk-17
- datagrip/sybase

## To run
`sudo ./install.sh -u`
Creates java-srv/log

## To stop
`sudo ./install.sh -d`
Removes java-srv/log

## For help
`sudo ./install.sh -h`

## Credit
- [Sybase driver and connection example](https://razorsql.com/docs/help_sybase.html)
