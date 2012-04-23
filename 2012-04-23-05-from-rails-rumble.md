# Monday Session 4: From Rails Engines to 50,000,000 results

## Presenter: Mikel Lindsaar

### Focus of Talk

* how to get a startup going on the side
* lessons learned from when things go wrong and servers crashed

### Still Alive - Production Testing

* smoke tests for your application
* does that app work even those the site is up

### Feature Scaling

* start simple
* set hard deadline and release on that date

### Focus

* focus on core features

### Communication

* engage with customers as much as possible
* don't implement everything that people want, choose the highest value features

### Performance Scaling - monitoring

* User Experience Alerts
  * Is the app down or query taking too long to load
* System opperation alerts
  * Done with cron to check server stats and alert if broken
* System Analysis Alerts
  * DB logs
  * Exception alerts

### Performance Scaling - database

* Indexing
  * Explain analyze is your friend in Postgres
* Concurrent Indexing

### Performance Scalig - queueing

* origianlly used DelayedJob
* replaced with ZeroMQ

### Process Scaling

* Dedicated staging environment
* Application Deployment
  * continuous deployment with zero downtime
* Application Configuration
* Standardization

### Take aways

* Look at replacing mySQL with Postgres
* Git process standardization, Git-flow http://jeffkreeftmeijer.com/2010/why-arent-you-using-git-flow/
