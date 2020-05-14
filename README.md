# Assertible test

![Assertible tests](https://github.com/mbarnach/assertible_test/workflows/.github/workflows/main.yml/badge.svg)

This repository is used to test the `oneOf` feature on the [Assertible](https://assertible.com/) service.
The `db.json` file is a DB for [My JSON Server](https://my-json-server.typicode.com/) which creates automatically the endpoint `https://my-json-server.typicode.com/mbarnach/assertible_test/ids`.
The endpoints return the content of the `db.json` file for the entry ids:
```json
[
  {
    "id": "bc98c020-09df-4d60-904a-2fb5cbb637ea"
  },
  {
    "id": ""
  },
  {
    "id": "806E80F7-4C4C-44EA-9F0D-E6CE1F0A5DD7"
  }
]
```

With the OpenAPI schema `assertible.json`, a web service can be created on Assertible, and a single test is made to evaluate the `oneOf` feature of the schema validator.

The OpenAPI schema has extended to test:
- the security scheme
- the default parameter for a query
