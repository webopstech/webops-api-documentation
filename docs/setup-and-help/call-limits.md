## Default Limit

By default, API requests are capped at 5 requests every 2 seconds. Exceeding this limit will return the following error:

```json
{
  "messageId":null,
  "code":1105,
  "message":"Call limit is reached. Please wait.",
  "timestamp":"2018-04-26T15:05:24-04:00"
}
```