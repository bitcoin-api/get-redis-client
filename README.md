# get-redis-client

[![npm version](https://badge.fury.io/js/get-redis-client.svg)](https://badge.fury.io/js/get-redis-client)

Get Redis Client


## About

Redis helper function to get Redis client. Useful in combination with [do-redis-request](https://github.com/bitcoin-api/do-redis-request).


## Installation
```
npm install get-redis-client --save
```


## Set Up
Your Redis URL can be set using the environment variable `process.env.REDIS_URL`. The default Redis URL is `127.0.0.1:6379`.


## Example

```.js
'use strict';

const getRedisClient = require( 'get-redis-client' );


(() => {

    const redisClient = getRedisClient();

    redisClient.quit();
})();
```