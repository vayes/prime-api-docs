## Login
 
### <request type="post"></request> /api/login

Returns a token to authenticate your next requests through bearer token.

!> This is the only API endpoint which you will fire with an bearer authentication token.

<!-- tabs:start -->

#### **Parameters**

```yaml
email: string [required]
password: string [required]
```

#### **Auth**

- Requires: `None`
- Permission: `None`

#### **Request**

```json
{
  "email": "name@domain.com",
  "password": "myPassword"
}
```

#### **Response**

> 200

```json
{
  "token": "f221dwqd.......4TTZnSk1qQ2FGdWZCWW"
}
```

<!-- tabs:end -->
