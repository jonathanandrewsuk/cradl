---
layout: default
title: Migration
nav_order: 5
description: "Cradl API"
permalink: /migration
---

# Migration

* The mico serviced based API (V2) should be backwards compatible to each of the endpoints currently served from the monolith (V1). 
* The V1 endpoints will he kept active as the V2 microservices are developed
* This means that as V2 endpoints are deployed existing customers are able to switch API versions in their staging environments and perform testing to confirm that all functionality has been replicated.
* Within each existing application the client will be able to switch one endpoint at a time. For example: They may start by switching to the V2 “Users” endpoint and keeping all other endpoints pointing at V1 apis.
