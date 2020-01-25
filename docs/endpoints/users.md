---
layout: default
title: Users
parent: Endpoints
nav_order: 1
---

# Users

* Register user information in the schema needed for account creation in the core
* Retrieve user information such as name, address and references to their KYC status, and any financial products they have enrolled in.



## Get A User
<div class="code-example" markdown="1">
Get
{: .label .label-green }

`https://api.cradl.com/v2/users/user_id`

**Request**

| Key        | Description        | 
|:-------------|:------------------|
| user_id           | unique user id |


**Response**

| Key        | Description        |
|:-------------|:------------------|
| id           | unique user id |
| kyc_id | id of associated kyc object   |
| login | user login object, email & password   |
| phone_number           | phone number, used for MFA |
| first_name           | users first name |
| last_name           | users last name |
| account_ids           | array of associated account ids  |
| error_codes           | array of error codes related to request (if any)  |

</div>

## Create A User
<div class="code-example" markdown="1">
Post
{: .label .label-blue }

`https://api.cradl.com/v2/users`

**Request**

| Key        | Description        |
|:-------------|:------------------|
| login | user login object, email & password   |
| phone_number           | phone number, used for MFA |
| first_name           | users first name |
| last_name           | users last name |

**Response**

| Key        | Description        |
|:-------------|:------------------|
| user_id           | unique user id |
| error_codes           | array of error codes related to request (if any)  |

</div>

## Update a Users KYC Information
<div class="code-example" markdown="1">
Patch
{: .label .label-purple }

`https://api.cradl.com/v2/users/user_id`

**Request**

| Key        | Description        |
|:-------------|:------------------|
| user_id           | unique user id |
| kyc_id           | id of the associated KYC object|

**Response**

| Key        | Description        |
|:-------------|:------------------|
| user_id           | unique user id |
| error_codes           | array of error codes related to request (if any)  |

</div>
