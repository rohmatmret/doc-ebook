# Authentication

> Developer Guide

In Order to Use API You must request by email gramedia digital Then we will then grant you access to a client_id, and client_secret.

# Request Details
|Environment |Method|	URL|
|- | -|-
|Sandbox |	POST|	https://api.sandbox.ebookdigital.com/|
| Production|	POST|	https://api.ebookdigital.com/|

# SOAX 

- Create a new Books
- Update AX ID 

## Update AX ID
- endpoint: baseurl/soax 
- Method : POST
- Headers : x-soax-client-key : base64(your client_id)
- x-soax-signature: SKU + SECRET_KEY
- body

```sh
 {
    "ax_id":7824938943,
    "sku":"SCOOPG34763",
    "approval_date":"2021-02-01"
 }
```