# Monday Morning Session 1: Designing Hypermedia APIs

## Presenter: Steve Klabnik
Slides at https://github.com/steveklabnik/hypermedia-presentation

### Searching for the meaning of REST

* Rails REST is not rest
* Writing book on using lean idea
** Put up sign up page see if there was a response

### REST is over

* You can't change people's mind by telling them they are wrong
* Nobody knows what REST so let's invent a new buzz word "Hypermedia"

### Hypermedia

* Beyond just regular text
* Hypermedia APIs text documents with links to other parts of API

#### Possitive

* Decoupled
* Salable
* Logevity
* Independent evolution

#### Downsides

* Latency
* Not as efficient because it's text not binary

### Designing with Hypermedia

* Use http properly
* Use hypermedia to guide clients through business process
* Make short term decisions for that hurt us in the long run
* Web is the biggest information store that mankind has been

### 5 Steps to Hypermedia API design

1. Evaluate Business Process
2. Create State Machine
  * dot language
3. Eveluate Media Type needs
  * build a format on top of JSON (Collection + JSON, HAL are the popular ones)
4. Create Media Types
  * data elements
  * how does it link
5. Implement

### Links
* Future book: http://designinghypermediaapis.com
* JumpStart Lab Tutorials: http://tutorials.jumpstartlabs.com

### Take aways
* Do some learning of state machines and how that affects app/API design
* Openstruct for storing config parameters
