## Distributed serving data-science models

### Description

This repository consists of a bunch of microservices which were deployed as a cluster in Kubernetes (OpenShift)

The aim of this project was to prototype a system which will be agnostic to data science models, and will cover data 
science models deployment, management and inference.

As pillars, I selected TensorFlow Extended, Kafka as technologies and service choreography as architectural pattern.


### Structure
As I mentioned above project consists of microservices orchestrated in event messaging system.
Every service can produce specific type of events, as well as sign and listen on another type of events.
The next services included:
- Monitoring service
- Scanner service
- WEB API service
- Compute service

Every service has it's own documentation stored in own folder.

Small front end application implemented also.


### How to add submodules
You can clone and setup every Kofer project alone or use monorepo.
If you would like to use monorepo, follow next commands:

1. Clone Kofer repository
2. **cd** into kofer and clone submodules
   
```bash
git submodule add https://github.com/adyachok/kofer-web-api.git kofer-web-api
git submodule add https://github.com/adyachok/kofer-scanner.git kofer-scanner
git submodule add https://github.com/adyachok/kofer-trinkets.git kofer-trinkets
git submodule add https://github.com/adyachok/kofer-monitor.git kofer-monitor
git submodule add https://github.com/adyachok/kofer-fas.git kofer-fas
git submodule add https://github.com/adyachok/kofer-facade.git kofer-facade
git submodule add https://github.com/adyachok/kofer-ds-artifacts.git kofer-ds-artifacts
git submodule add https://github.com/adyachok/kofer-compute.git kofer-compute
```    

    


### Mode information
More information you can get from the presentation attached to this repository.
  