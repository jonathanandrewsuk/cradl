---
layout: default
title: Users
parent: Endpoints
nav_order: 1
---

# Users

* Register user information in the schema needed for account creation in the core
* Retrieve user information such as name, address and references to their KYC status, and any financial products they have enrolled in.



<div class="code-example" markdown="1">
Get
{: .label .label-green }

**Get A User**

`https://api.cradl.com/v2/users/user_id`

Response

| Key        | Description        | 
|:-------------|:------------------|
| id           | unique user id |
| kyc_id | id of associated kyc object   |
| phone_number           | phone number, used for MFA      |
| first_name           | users first name |
| last_name           | users last name |
| account_ids           | array of associated account ids  |
| error_codes           | array of error codes related to request (if any)  |

</div>
