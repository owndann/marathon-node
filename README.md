# Marathon Node.js Client Library

Node.js client library lightweight for Marathon's REST API. ES6

## Install

Install using npm or yarn

```shell
$ npm install marathon-node-library
$ yarn add marathon-node-library
```

## Config

```javascript
const marathonClient = require('marathon-node-library')(MARATHON_API_URL, {
  // if you have basic authentifiaction in you marathon API
  auth: {
    user: MARATHON_USER,
    pass: MARATHON_PASSWORD,
  },
  // Or Accestoken auth
  headers: {
    'Authorization': 'token=MARATHON_AUTH_TOKEN'
  }
});

```

## API Methods

### Apps

- /v2/apps GET

```javascript
marathonClient.apps.getList(query)
```

- /v2/apps POST "Create App"

```javascript
marathonClient.app.create(body)
```

####  Insipred on [marathon-node](https://github.com/elasticio/marathon-node) of [@elasticio](https://github.com/elasticio)

# License

MIT.
