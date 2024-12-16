# 0x03. Queuing System in JS

## Overview
This project focuses on implementing a queuing system in JavaScript using Redis, Node.js, Express.js, and Kue. It covers essential concepts of job queue management, Redis operations, and asynchronous processing.

## Technologies
- **Back-end:** JavaScript (ES6)
- **Database:** Redis
- **Framework:** Node.js, Express.js
- **Queue System:** Kue

## Learning Objectives
By completing this project, you will learn:
- How to run a Redis server on your machine
- How to run simple operations with the Redis client
- How to use a Redis client with Node.js for basic operations
- How to store hash values in Redis
- How to deal with async operations with Redis
- How to use Kue as a queue system
- How to build a basic Express app interacting with a Redis server
- How to build a basic Express app interacting with a Redis server and queue

## Requirements
- Ubuntu 18.04, Node.js 12.x, and Redis 5.0.7 environment.
- All files should end with a new line.
- Code should use the `.js` extension.
- A `README.md` file at the root of the project folder is mandatory.

## Installation
1. **Install Redis:**
    ```bash
    wget http://download.redis.io/releases/redis-6.0.10.tar.gz
    tar xzf redis-6.0.10.tar.gz
    cd redis-6.0.10
    make
    src/redis-server &
    ```

2. **Verify Redis Installation:**
    ```bash
    src/redis-cli ping
    # Should return PONG
    ```

3. **Clone the Repository:**
    ```bash
    git clone https://github.com/alx-backend/0x03-queuing_system_in_js.git
    cd 0x03-queuing_system_in_js
    ```

4. **Install Project Dependencies:**
    ```bash
    npm install
    ```

## Usage
1. **Start Redis Server:**
    ```bash
    src/redis-server &
    ```

2. **Run the scripts:**
    - To connect to Redis:
        ```bash
        npm run dev 0-redis_client.js
        ```

    - To perform basic operations:
        ```bash
        npm run dev 1-redis_op.js
        ```

    - To handle async operations:
        ```bash
        npm run dev 2-redis_op_async.js
        ```

    - To store and display hash values:
        ```bash
        npm run dev 4-redis_advanced_op.js
        ```

    - To use publisher and subscriber:
        ```bash
        npm run dev 5-subscriber.js
        npm run dev 5-publisher.js
        ```

    - To create and process jobs:
        ```bash
        npm run dev 6-job_creator.js
        npm run dev 6-job_processor.js
        ```

## Tasks
1. Install Redis instance.
2. Create a Node Redis client.
3. Perform basic and async operations with Redis.
4. Store and retrieve hash values.
5. Implement publisher and subscriber with Redis.
6. Create and process jobs using Kue.
7. Track progress and handle errors in job processing.
8. Implement a stock management system with Express and Redis.

## Resources
- [Redis quick start](https://intranet.alxswe.com/rltoken/bD8ATSAVbine9-zEXenwyw)
- [Redis client interface](https://intranet.alxswe.com/rltoken/vFJSkoXkIvLqHzQgx8DVcw)
- [Redis client for Node JS](https://intranet.alxswe.com/rltoken/mRftfl67BrNvl-RM5JQfUA)
- [Kue documentation](https://intranet.alxswe.com/rltoken/yTC3Ci2IV2US24xJsBfMgQ)
        _**N.B:** Kue is deprecated but still used in the industry_
