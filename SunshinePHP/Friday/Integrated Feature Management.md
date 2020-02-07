# Integrated Feature Management - Using Feature Flags
Dana Luther

[@danaluther](https://twitter.com/danaluther)

[Joind link](https://joind.in/talk/7b4f6)

## What are feature flags?

A variable that defines a condition.

 * [Feature Flags site](https://featureflags.io)

Helps to avoid long-running feature branches

Integrated Management: Defining your conditional such that you don't need to update your codebase to switch features.

For views, you can add conditionals around which view to render

## Why do we want to use them?

* A/B Testing    
 * Putting together two versions, and supplying them to two groups of users
 * Something as simple as button color/location for click-throughs
* Canary Testing/Rollouts
 * Sending out a new feature to a small percentage of userbase
 * 90% old version, 10% new version. Does it perform how we think it will?
 * Slowly start ramping the % on new version
* Maintenance Windows
 * Maybe the whole site is down, maybe portions are down
 * Flagging for third party API's that may be under maintenance
* Seasonal/Calendar driven content
* [More feature flag uses](https://featureflags.io/feature-flag-uses/)

Can automate turning them on/off with timers, or based on failures, etc

## How do we want to use them?

* [PHP libraries](featureflags.io/php-feature-flags/)
* [On packagist](https://packagist.org/), search for "feature flag", etc
 * [Swivel](https://packagist.org/packages/zumba/swivel)
 * Well build, so if there is no framework version for it, it's not hard to make one

### User Experience Groups

Cohorts of users that have the same experience.  Users are placed into "buckets", 10 buckets, each has 10% of users.

Look into [Google Tag Manager](tagmanager.google.com) as a way of telling Google Analytics what bucket a user is in

Once Google Analytics knows about buckets, you can assign groups for A/B testing.

### Implementing in your application

#### Scenario: Canary Release

Create feature slugs, then assign slugs to buckets

Decouple from code deployment: Tell tool (swivel, etc) what slugs lead to what behaviors, and go from there
- The order you add the behaviors is important if you put everybody in main bucket and some in test bucket

Based on analytics, can start adding users to buckets

#### Scenario: A/B Testing

Same setup as Canary Release, just starts at 50% of buckets having new version