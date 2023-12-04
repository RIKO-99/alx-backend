##### Installation

1. Clone the repository:
   ```bash
   https://github.com/RIKO-99/alx-backend/tree/master/0x03-queuing_system_in_js

## Node Redis
This project utilizes the node-redis library for interacting with Redis. Below are some key points about node-redis:

Installation:

npm install redis
Connecting to Redis:

const redis = require('redis');
const client = redis.createClient();

client.on('connect', () => {
  console.log('Connected to Redis');
});

client.on('error', (err) => {
  console.error(`Error connecting to Redis: ${err}`);
});

## Basic Operations:

Example of setting and getting a value:
javascript
Copy code
client.set('key', 'value');
client.get('key', (err, result) => {
  console.log(result); // Outputs: value
});
Handling Errors:

client.on('error', (err) => {
  console.error(`Redis error: ${err}`);
);
