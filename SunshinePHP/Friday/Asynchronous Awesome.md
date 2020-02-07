# Asynchronous Awesome

Eric Mann
[@EricMann](twitter.com/EricMann)

## Naive Approaches to Async

### Pseudo-cron

Wordpress checks if a cron should be run when your site is hit.  If your site doesn't get hit, the cron doesn't run.  Still living in the request/response lifecycle

### Mechanical Turk-like job systems

A bunch of people that do jobs manually.  Fakes scheduled tasks.

### Using another language entirely

Node has a long running event loop, as do other languages. Multi-threading in some languages.  PHP doesn't, so people will use another language.

## Parallel vs Concurrent

* Concurrent: Two queues, one coffee machine
* Parallel: Two queues, two coffee machines
* Concurrent Parallel: Two lines for two different things

## Tools available for Async

* Gearman
 * Job queue server
* RabbitMQ
 * Message queue
* Amp (promises)
* pthreads - extension for php that provides multithread support

Job Queue: Remote invocation of a task on another server - can be bidirectional
Message queue: Just sending messages back and forth - mono-directional

### Gearman

Workers register with a server.  Clients can ask server what workers exist.
Client connects to server, passes a job to it.
Workers don't have to be in PHP, but they can be

### Rabbit MQ

Client publishes a message onto the queue server
Workers are polling the queue server
Worker consumes a message from the queue
Can be made bi-directional by using two queues, one for app -> receiver, and one for receiver -> app

### Promises (AMP)

A promise represents the eventual result of an asynchronous operation
JQuery deferred empowers the AMP library, not the standard promise pattern

### pthreads

PHP must be compiled with a command flag (zts) for thread safety (it's not by default)
It consumes a lot of CPU resources to fan out over multiple threads/processes


AMP supports pthreads

## Why use any of this?

Empowers things like pdf conversions, video transpiling, slow things
Allows you to hit single-endpoint API's for multiple people without being so slow



