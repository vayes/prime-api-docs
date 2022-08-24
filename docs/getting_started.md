## Getting Started

### Localization

?> To localize your validation and error messages you need to add `?hl=en` to your endpoint.

```yaml
hl: string [optional] [default:"tr"]
```

### Error Responses 


<!-- tabs:start -->

#### **Auth Required**

```json
{
  "status": 401,
  "error": 401,
  "messages": {
    "error": "Unauthorized"
  }
}
```

#### **Auth Expired**

```json
{
  "status": 400,
  "error": "Firebase\\JWT\\JWT",
  "messages": {
    "error": "Expired token"
  }
}
```

#### **Auth Failed**

```json
{
  "status": 401,
  "error": "Login failed",
  "messages": {
    "error": "User not found."
  }
}
```

#### **Validation Failed**

```json
{
  "status": 400,
  "error": "Validation failed",
  "messages": {
    "name": "The name field is required.",
    "description": "You must enter a description."
  }
}
```

#### **Not found**

```json
{
  "status": 404,
  "error": "Not Found",
  "messages": {
    "error": "Page not found."
  }
}
```

<!-- tabs:end -->




