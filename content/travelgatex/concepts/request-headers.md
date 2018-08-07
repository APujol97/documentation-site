+++
title = "Request Headers"
pagetitle = "Request Headers"
description = ""
icon = "fa-plus-circle"
weight = 3
alwaysopen = false
+++

The following HTTP request headers are relevant to all request methods (GET, PUT, POST and DELETE) and are required on all API requests.


## Authorization (Required)

The HTTP Authorization request header contains the credentials to authenticate a user agent with a server, usually after the server has responded with a 401 Unauthorized status and the WWW-Authenticate header.	no

### Syntax

```
Authorization: <type> <credentials>
```

### Directives

`<type>`:
- `ApiKey`
- `Bearer`

`<credential>`: String

### Example
Authorization: Apikey q8ggx-poVDW76Kw9-18hwnnRvxlZm-AP2QZ

## TGX-Audit (Optional)

Force audit the request in TravelgateX systems.

### Syntax

```
TGX-Audit: <number>
```

### Directives

`<number>`:
- 0: The requester prefers to allow tracking on the target system.
- 1: The requester prefers not to be tracked on the targe system.

`<credential>`: String

## TGX-Tracing (Optional)

Performance traces alongside the data returned.

### Syntax

```
TGX-Tracing: <number>
```

### Directives

`<number>`:
- 0: Default value. Tracing not enabled.
- 1: Tracing enabled.

`<credential>`: String
