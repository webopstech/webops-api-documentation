## Username and Password

WebOps Admin shall provide the following for each client setup:

- Username
- Password
- Manufacturer ID (manufacturerId)

Each call to WebOps API must be initiated via basic access authentication. Before initiating a request with any available WebOps API end point, designated username and password must be passed to inbound token service as a request header in a Base 64 encoded string.

## /token

Token API in return will give client an access token (Access_token), which must be passed to each WebOps API inbound service. This token will expire after a designated period of time.

### Examples

#### Request Header

**Key**|**Value**|**Description**|
-|-|-
Authorization|Basic|Base64(Username:Password)

#### Response Header

|**Key**|**Value**|
|-|-|
|Access_token|Value to be used in each subsequent inbound service to WebOps API|