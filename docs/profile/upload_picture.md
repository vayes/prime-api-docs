## Upload profile picture

### <request type="post"></request> /api/{version}/user/profile-picture

Uploads profile picture for current user.

<!-- tabs:start -->

#### **Parameters**

[parameters.md](../_parameter/media/_generic.md ':include')

#### **Auth**

- Requires: `AuthToken`
- Permission: `None`

#### **Request**

```json
{
  "name": "profile_picture.jpg",
  "height": 200,
  "width": 200,
  "mime": "image/jpeg",
  "dataUri": "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEBLAE....",
}
```

Here is a sample base64 image to test in API calls:

```json
{
  "dataUri": "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEBLAEsAAD/2wBDAIVcZHVkU4V1bHWWjoWeyP/ZyLe3yP////L/////////////////////////////////////////////////////2wBDAY6WlsivyP/Z2f//////////////////////////////////////////////////////////////////////////wAARCADIAMgDASIAAhEBAxEB/8QAGAABAQEBAQAAAAAAAAAAAAAAAAECAwT/xAAhEAEBAAIDAAIDAQEAAAAAAAAAARECMSESQVEDMmEiE//EABYBAQEBAAAAAAAAAAAAAAAAAAABAv/EABYRAQEBAAAAAAAAAAAAAAAAAAABEf/aAAwDAQACEQMRAD8A5AoIoAYq+b9Ivqgv/PbDNlnLc3a9SwHJudrjVMY4Qa4Ms2UnQNZSdpK3FCRbhZGdgSXCXejF5Qb95PTGTIJb2CKKZQBciAKAAAACgigARrXS11mkgOUy3jp0xFBx8rI6YMAzCrhMAxYxdb9O2HO2yoOeBv1fo9T5ijA3/n6S6z4oMjXn+nmgyLZZyAgAAoAABHXXT7TTX5reQXhcsXZPYOmRj0uQaMpkBVRQTBdZZwoDjvrY5vVZmPPvr5oMgAGaAHIAAqAAAsma3NMYZ0/Z3szAZYuy7dOduQXORBFaEAblXLCwG8rlhVRvKucrcvQLGPya5jcL3AeYWztAAAAABpEEFAI7SuU5ayDpcXly30xem5TKjiOu2kvDnZhFAAFRQXJllQVdayQHaVWJWvhUct5/plveds2AgAAANI0iCCgEZ3vbbnt+wLN8LN2Ez/BXabLcVxlWbKjXyJkiKsi4WWLKDGKYdYdBriO2J9J5/gJq2kiqjH5OGG/ycMACiDIoDQCACgztcOfy3t9sRVDr5XBgEkkRrCYAi1cdM0DLU2YspMg7TZuV55cNzbAOplj3D3FRvIzLloGd2V27qIAoCAA0AgAA578Mxr8nLKq0IAWrEWAtRayBj6MqoM4yNYQEWI1rAb1N9sTpm7Y6Z5oNRUUQBAAAaEEFABy3/ZF35RVVcLIoOdixrpAT1c8KuFwDDUZqiqggK1rwy3r+ojG3K6wsy1gABEQBQAAyM5XINDLUgMbpry3t2zrBWmN7Z1HRzoMTatTdMHkHTXeXpcuXntvHyC2Mtzhm8gigKsmW8dJJhoZZwoIIKKIACCgOcalxzGI1MA0ZpJlqddQGbwmrVZ4oNXhix0+Ewo54HSxnCKiwwSAs4SqlBF15Za1nQNTlpnXlq8CMqggoAAAAAOMrprrb3W9fxzXlrpRn4xE4mI1twyCJVAXXgSXFaURML8gJgawgJeGK6TtmxFYaNZ2XqhWtF2TThN72IDOVyDQzlcgqs5UFEAdLEwAJtemYAKgAi67Y5AGwFCFgAnnFW65AGbrjhi90EHTWdOe0t2BQmtbmgAvj+pfx0AYuZyZBAyAD/9k="
}
```

#### **Response**

> 201

[_uploaded_profile_picture.md](../_response/media/_uploaded_profile_picture.md ':include')

<!-- tabs:end -->
