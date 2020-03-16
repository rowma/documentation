---
id: database
title: Database
sidebar_label: Database
---

inmemory database and mongodb are the possible choises for database of ConnectionManager.

## Inmemory Database (Default)
Rowma stores Application and Robot information into arrays by default.

This storage is volatile, so you can use it only for test usecases.

## Mongodb
Mongodb is supported in Rowma and can be switched easily from an environment variable.

```bash
# For your local development environment
$ docker-compose up -d
$ ROWMA_DB=mongodb npm start
```

Also, you can use an external managed mongdb by specifying the URI.

```
$ ROWMA_DB=mongodb MONGODB_URI=mongodb://root:rootpass@mongodb.example.com:27017 npm start
```

(TLS feature to access Amazon DocumentDB is coming soon)
