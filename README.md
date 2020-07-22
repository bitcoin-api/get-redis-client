# get-redis-client

[![npm version](https://badge.fury.io/js/get-redis-client.svg)](https://badge.fury.io/js/get-redis-client)

Get Redis Client


## About

Redis helper function to get Redis client. Useful in combination with [do-redis-request](https://github.com/bitcoin-api/do-redis-request).


## Set Up

`process.env.REDIS_URL` needs to be set to your Redis URL


## Example

```.js
'use strict';

const getRedisClient = require( 'get-redis-client' );


(() => {

    const redisClient = getRedisClient();

    redisClient.quit();
})();
```