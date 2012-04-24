# Tuesday Session 3: Schemaless SQL — The Best of Both Worlds

## Presenter: Will Leinweber @leinweber
Slides: http://ssql-railsconf.herokuapp.com

### People love CoachDB and MongoDB

* Documents are fun
* Migrations are hard
* If you have big different between your data and your objects then it's hard to things in your head

### Why Postgres

* Builtin fulltext search
* Easy Geolocation with PostGIS
* knn, closest records
* pub/sub like functionality
* wal-e backup tool https://github.com/herku/wal-e

### hstore

* key/value store in a column
* can be used with joins
* support build into Rails 4
* demo heroku/hstor_demo
* log observations ryandotsmith/wcld
* bulkbag for storing extra in table
* constraints
  * only strings
  * no nesting

### plv8

* v8 engine in progress
* write js for functions
* documents
  * create index on any expression
  * postpres 9.2 will have json datatype
  * type checking with domain
  * run mustache in progres
* json:select()
  * css selector for json

### ruby

* use active record and dump data in a single column
* working on gem to make this work with json:select()
* don't be afraid of using advanced db features

### Postgres app
* postres.app http://progresapp.com
