# Redis_in_c/cpp
# Key-Value Store Server

This project implements a simple key-value store server in C++. It provides functionality to handle various commands like GET, SET, DEL, and more, along with support for zset operations.

## Overview

The key features of this server include:

- **GET**: Retrieve the value associated with a key.
- **SET**: Set the value for a key.
- **DEL**: Delete a key from the store.
- **ZSET**: Operations for a sorted set including adding, removing, querying, and scoring.

The server is implemented with non-blocking IO and supports multiple concurrent connections using the poll() system call. It also includes a thread pool for asynchronous operations.

## Dependencies

- C++ compiler with C++11 support
- GNU Make


# Simple Key-Value Store Server

This will compile the source code and generate the executable file kvstore.

## Usage

To start the server, run the following command:


./kvstore
# Simple Key-Value Store Server

By default, the server listens on port 1234. You can modify the port in the source code if needed.

## Commands

The server supports the following commands:

- **GET**: Retrieve the value associated with a key.  
  Example: `GET key`

- **SET**: Set the value for a key.  
  Example: `SET key value`

- **DEL**: Delete a key from the store.  
  Example: `DEL key`

- **ZADD**: Add a member with a score to a sorted set.  
  Example: `ZADD zset score member`

- **ZREM**: Remove a member from a sorted set.  
  Example: `ZREM zset member`

- **ZSCORE**: Get the score of a member in a sorted set.  
  Example: `ZSCORE zset member`

- **ZQUERY**: Query members in a sorted set based on a score range.  
  Example: `ZQUERY zset score member offset limit`

- **KEYS**: Get all keys in the key-value store.  
  Example: `KEYS`
