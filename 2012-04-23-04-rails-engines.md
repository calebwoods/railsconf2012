# Monday Session 3: Rails Engine Patterns

## Presenter: Andy Maleh

### Benefits of Engines

* shared code across controller, models and views
* stored in gems

### Definition of engine

* has folder structure similar to app
* lib directory has engine file as it's gem

### Load Order

* load order - change so that engine loads first
* config railties order

### Ruby code customization

* based on load path app files can expand classes
* keeps only common code in engine

### View and Assest

* can't be expanded like Ruby class
* app will use either the app or engine file

### Typical dev process

1. made change in engine commit then get GIT ref
2. change git ref in Gemfile of all apps

### Improve Productivity

1. symlink engines to app directory with rake tasks or gem link to path
2. before deployment go through typical dev process

### Best Practices

* Name space all engine files to avoid name conflicts
* Prevent bi-directional coupling
* Avoid app specific conditional

### Pattern - Common Domain

* include base behaviour and assoiations
* in each add app specific code and behavoir

### Pattern - Expose Helper

* need to customize persentation for one app specific
* common helper in engine and redfine specific methods

### Pattern - Expose Partial

* extract parts of view that needs to be customize to partial and redfine in app

### Pattern - Extension Point

* problem multiple apps need to contribute data to view in different places
* add helper that reads partials from ext directory and insert based on file name

### Pattern - Configurable Features

* each needs different features in different location
* engine looks up config from YAML file and uses conditionals

### Cost of using Rails Egine

* setting up engine first time
* switching contexts for making changes
* adding ref to Gemfile

### Benefits

* resuse of code
* defined boundries for where app code and feature code exists

### Engine vs Service

#### Engines are better

* reusing small bits of MVC
* avoid network infrastructure and more code to interacte
* less over head to use as engine at first

#### Service are better

* better for large ammount of code
* information needs to be consumed by muliple laungages
* offload feature to it's own service

### Take aways

* Develop engine for Student Managment for myCP
* Possible replace theme gem with engine
