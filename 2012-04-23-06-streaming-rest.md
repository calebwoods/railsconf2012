# Monday Session 5: Realtime web applications with streaming REST

## Presenter: Brad Gessler

### State of apps

* had REST for server backend
* Backbone.js and Ember.js made cosuming REST API easier

### Solutions

* long pulling
  * using setInterval and cahce
  * doesn't work when you are dealing with large data streams
* streaming

### Picking a streaming layer

* Socket.IO
  * Issue with latency
  * Routing only on channels not urls
* Meteor
  * new and tightly coupled

### Firehose.io

* idea was to push resources
* pub/sub server using curl
* URL's are the exchange
* security
  * proxy with Goliath[https://github.com/postrank-labs/goliath] that hits Rails app

### Take aways

* Look at replacing mySQL with Postgres
* Git process standardization, Git-flow http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/
