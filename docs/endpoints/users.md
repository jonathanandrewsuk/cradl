---
layout: default
title: Users
parent: Endpoints
nav_order: 1
---

# Users

**The users endpoint can be used in 2 ways during the onboarding process:**
1. **Without KYC**: User objects can be created for the purpose of contacting users who have partially completed applications
2. **With KYC**: User objects that have been created with KYC records associated are able to create account objects

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
| id           | unique user id |
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
| id           | unique user id |
| error_codes           | array of error codes related to request (if any)  |

</div>
