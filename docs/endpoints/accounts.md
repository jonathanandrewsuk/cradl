---
layout: default
title: Accounts
parent: Endpoints
nav_order: 3
---

# Accounts

* Accounts can be created and associated with users, provided they have the correct KYC permissions.
* Account creation requests will be passed onto the core

## Create Account
<div class="code-example" markdown="1">
Post
{: .label .label-blue }

`https://api.cradl.com/v2/accounts`

**Request**

| Key        | Description        |
|:-------------|:------------------|
| user_id | id of the user that will be associated with the account|
| account_type    | the type of account to be created  |

**Response**

| Key        | Description        |
|:-------------|:------------------|
| id           | unique account id |
| error_codes           | array of error codes related to request (if any)  |

</div>
