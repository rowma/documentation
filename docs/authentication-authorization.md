---
id: authentication-authorization
title: Authentication and Authorization
sidebar_label: Authentication and Authorization
---

Rowma supports authentication and authorization by using an external authenticator server.

```
$ npm run build && AUTHENTICATOR_URL=http://localhost:1323/api/v1 ROWMA_DB=mongodb npm start
```

In addition, you should use `connectWithAuth()` function in a SDK.
