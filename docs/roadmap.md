---
layout: default
title: Roadmap
nav_order: 3
description: "Cradl API"
---

# Roadmap
<div class="code-example" markdown="1">

## Near Term
{: .text-green-200}

### Customer Groundwork

* Reach out to a small group of clients that have been requesting API access, get a sense of functionality priority.
* Reach out to key existing clients that may need to migrate their services in the future. If possible they should have input on the roadmap and migration plan.
* Draft a migration timeline e.g All KYC requests should be sent to the V2 endpoint by Q3 2020

### Technical Groundwork

* Finalize the functional plan for the API services
    * Which endpoints are needed to get the first version live?
    * How should the functionality be grouped? e.g. Should KYC and Users be contained in a single endpoint?
    * What are other endpoints to consider in the future? Lending etc
* Create architecture plan and micro-service template
* Create starting assumption for object shapes (User, KYC etc) and associated tests

### Users & KYC

* Stand up the first 2 endpoints in a staging environment, integrated with KYC partner
* Create "sad path" scenarios and run tests:
    * Key fields are not passed by the user
    * KYC partner is down, how would we handle this?
</div>

<div class="code-example" markdown="1">

## Medium Term
{: .text-green-200}

### Client Feedback

* Begin testing Users & KYC with small number of early adopting clients, this could be within their staging environment.
* Any changes/feedback should be considered by future work. e.g Is this documentation provided comprehensive enough?
* Begin to develop migration plan for existing clients

### Iterative Cycles - Accounts & Payments

* Bring up other endpoints in a similar fashion, getting basic functionality live and testing with key clients.
* Perform testing of the endpoints communicating with each other to perform more advanced tasks e.g adding KYC to a User.

</div>

<div class="code-example" markdown="1">

## Long Term
{: .text-green-200}

### Beta Release

* Release all endpoints to key clients
* Contact clients using the V1 product to kick off the migration process

### Long Term Retrospective

* How does the full set of endpoints compare to the V1 product? Stability, Cost and User Experience
* What could be done differently as we develop new functionality? e.g. Lending

</div>
