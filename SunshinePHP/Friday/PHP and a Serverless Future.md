# PHP and a Serverless Future
Doug Steinberg
@doug_steinberg

[Slides](https://joind.in/talk/3e3f6)

## What is serverless?

A server managed by a cloud provider that runs some code and allocates resources for you based on some trigger

What triggers it? Could be anything. HTTP request, Queue events, DB events, scheduled events, etc

## Why would we want to use it?

* It's a good fit with PHP - both are stateless
* It's a good way to separate concerns
* Don't need to worry about maintenance/upgrades/etc
* Can reduce costs
* Scales easily and automatically
* Improve security
 * Can't hack a server that doesn't exist?
 * Functions can be given limited views

Cons:
* Vendor lock-in
* Unsuitable for long-term tasks
* Cold starts
 * Takes a bit to run a function that hasn't been run in a while
* Complexity and learning curve

## Vendors and Tools

* AWS Lambda (focus of this talk)
* MS Azure Functions
* IBM Openwhisk
* Google Cloud Functions/Cloud Run

AWS doesn't support PHP, but does have custom runtimes where you can set that up

Tools:
* [bref](bref.sh) takes care of that custom runtime
* [serverless](serverless.com) - helps you deploy to your serverless provider
* [Vapor](vapor.laravel.com) - takes care of everything for laravel apps