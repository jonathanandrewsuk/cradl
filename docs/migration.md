---
layout: default
title: Migration
nav_order: 5
description: "Cradl API"
---

# Migration

## Strategy

The V2 system will re-create all functionality in the V1 system and they will be run in parallel during the migration period. This means that we will be able to create a V2 front end experience that sits on top of our newly deployed V2 backend.

As the V2 system will be component based both front & back, each client will be able to migrate the user experience piece by piece, **avoiding a big switchover event in favor of a gradual transition**. If there are any issues we will be able to quickly rollback to the V1 system.

Only when the V1 system has been unused for sometime will it be retired.

## Migration Project Teams

Depending on the complexity of the migration a cross-company team should be assembled. This team should include business sponsors, product owners and engineers from both Cradl and the client company.

## Risks & Dependencies

* Clients are nervous about a migration and resist switching to V2
* Will client side developers be able to dedicated sufficient time to a migration project?
* Do some migrations require extensive custom development work, who will pay for this?
* A microservice may begin to error under heavy traffic, did we make the correct assumptions in our architecture planning?
