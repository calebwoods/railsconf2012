# Tuesday Session 5: Stack Smashing

## Presenter: David Czarnecki @czarnecki
Slides: http://speakerdeck.com/u/czarneckid/p/railsconf-2012-stack-smashing-cornflower-blue

### Application Migration

* start internal
* end with external apps
* iteraction breeds abstraction

### The Unicorn

* from Thin to Unicorn
* wicked fast
* kernel load-balancing
* can do rolling restarts
* signal for capacity

### Service Configuration

* if a server fails does it make a sound?
* alias DNS to mysql server
  * no redeploys if DB server changes
  * shield from updating config when needed

### Sexy Capistrono

* sexy == DRY
* common functionality into a gem

### Application Monitoring

* it has to be visual
* it must be historical
* Munin
* request/sec, queries/sec

### Infrastructure Monitoring

* BDD on infrastructure using cucumber

### Continuous Integration

* Jenkins
* Build failure notification on build failure via email

### Contious Deployment

* Deploy only deploys if build is successful
* Deploy script same a manual deploy

### Review

* simplify as much as possible
* upgrade small to big
* alias services
* DRY
* monitor
* validate - test infrastructure
* integrate
