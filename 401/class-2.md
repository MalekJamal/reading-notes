# express-middleware-demo

## What is middleware function?

> Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application's request-response cycle. These functions are used to modify req and res objects for tasks like parsing request bodies, adding response headers, etc.
> It's like a bridge.

- middleware levels :

1. Application level middleware.

> app, express..ect.

2. Router level mid.

> for speicifc route.

3. Error level handler.

> handle the errors, status code (400,500).
> 400 problem with the client, 500 server error.

4. Built-in level middleware function.

> express, cors..etc.

5. Third-party level packages | API.

> from external Api, cookies, body-parser, morgan, cors.

### 4xx Client Error

400 Bad Request

401 Unauthorized

402 Payment Required

403 Forbidden

404 Not Found

405 Method Not Allowed

406 Not Acceptable

407 Proxy Authentication Required

408 Request Timeout

409 Conflict

410 Gone

411 Length Required

412 Precondition Failed

413 Request Entity Too Large

414 Request-URI Too Long

415 Unsupported Media Type

416 Requested Range Not Satisfiable

417 Expectation Failed

418 I'm a teapot (RFC 2324)

420 Enhance Your Calm (Twitter)

422 Unprocessable Entity (WebDAV)

423 Locked (WebDAV)

424 Failed Dependency (WebDAV)

425 Reserved for WebDAV

426 Upgrade Required

428 Precondition Required

429 Too Many Requests

431 Request Header Fields Too Large

444 No Response (Nginx)

449 Retry With (Microsoft)

450 Blocked by Windows Parental Controls (Microsoft);

- [error](https://www.restapitutorial.com/httpstatuscodes.html)
