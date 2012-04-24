# Tuesday Session 4: Digging Deep with ActiveSupport::Notifications

## Presenter: Matt Sanders @nextmat

### What get measured gets managed

* production != development
* when problem happens you can already to be tracking the problem areas

### Performance Monitoring

* action controller request time
* total request vs slow requests

### SQL Monitoring

* check requests by model

### What to with data

* custom logging - adding things to logger - pappertrail
* custom event in New Relic
* StatsD
* KISS
* save data for later - postpone sql explains

### Performance

* all subsribers are run in same thread as request
* background slow subscribers

### Power Moves

* Conditional Instrumentation
  * rollout
  * turn on specific notifications for specific users
* Simplifying Repetitive Instrumentation
  * `extend Forwardable`
  * LogSubscriber

### Use Outside of Rails

* activesupport/notifications can be on it's own
* gems that use this
  * faraday
  * excon
* what else can you do
  * lograge
    * detactes existing log subscribers
  * harness
  * search rails for `.instrument`

### Discuss Conventions for team

* put subscribers in intializer
* don't use for core events use for notifications

### Take aways

* what are the important things for our apps
* what are our important metrics, what's the top 2
* student action notifications

