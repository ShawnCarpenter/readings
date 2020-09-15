# Redis
Redis is an in memory data store.
It offers something called HyperLogLogs which proves that programmers really aren't that good at naming things.
In all seriousness it looks interesting as a way to store data that is quickly retrievable.

# Queues

Queues are lines, but British. When a person or item enters a queue they enter at the end. The first item in the queue is dealt with first, then the next. Items are added at the end and dealt with one at a time.

# Task Queues
Task queues are a way of organizing tasks so that the oldest tasks get attended to first.

# Bull
Bull is a javascript library for dealing with task queues using redis.
