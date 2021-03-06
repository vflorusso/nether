# Count Event

## When?

## Why?

## Request

### JSON Body
```json
{
    "type": "count",
    "version": "1.0.0",
    "clientUtcTime": "2016-09-07T13:37:00",
    "displayName": "enemiesKilled",
    "value": 1,
    "gameSessionId": "A3A22EE1-563A-4697-9EDF-B69B998CD214",
    "properties": {
        "country": "Germany"
    }
}

```

Element name       | Required | Type   | Description
------------------ | -------- | ------ | -----------
type              | Yes      | String | Specifies the type of event being sent. Has to be "game-start".
version            | Yes      | String | Specifies the version of event, based on how much information is being sent.
clientUtcTime      | Yes      | DateTime | Specifies the UTC timestamp of the client.
displayName        | Yes      | String | Entity which is being counted, e.g. magic sword found, number of enemies being killed
value              | Yes      | Int    | Quantifying the displayName
gameSessionId      | Yes      | String | GUID that uniquely identifies the game session
properties         | No       | String | Option for the developer to integrate more information, e.g. country, colour, etc.