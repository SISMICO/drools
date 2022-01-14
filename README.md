# Drools

## How to run
``` bash
docker-compose up

docker run --rm -p 8080:8080 -p 8001:8001 -d --name drools-workbench jboss/drools-workbench-showcase:latest
docker run --rm -p 8180:8080 -d --name kie-server --link drools-workbench:kie-wb jboss/kie-server-showcase:latest

```

## Default Users for Drools
```
USER        PASSWORD    ROLE
*********************************************
admin       admin       admin,analyst,kiemgmt
krisv       krisv       admin,analyst
john        john        analyst,Accounting,PM
sales-rep   sales-rep   analyst,sales
katy        katy        analyst,HR
jack        jack        analyst,IT
```

## Default User for Kie
- Username: kieserver
- Password: kieserver1!
