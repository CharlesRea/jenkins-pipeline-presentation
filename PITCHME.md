# Jenkins Pipeline

### Or why your CI should be in code

---

### Pipeline?

* Configure your Jenkins builds using code
* Groovy DSL
* Build config in source control

---?code=Jenkinsfiles/1-HelloWorld&lang=groovy
@[2]
@[3-4]
@[5-8]

Note:
* Declarative v Scripted.
* Show on Jenkins. 
* Show on Blue Ocean. 
* Source: Jenkinsfiles/1-HelloWorld

---?code=Jenkinsfiles/2-ParallelStages-ShortExample&lang=groovy
@[5-18]

Note:
Source: Jenkinsfiles/2-ParallelStages

---?code=Jenkinsfiles/3-Multibranch-ShortExample&lang=groovy
@[10-12]

Note:
* Source: Jenkinsfiles/3-Multibranch
* Show ECP builds.

---

### The good parts - CI as code

* Put build changes through code review
* Easily propogate changes to all branches
* Single source of truth - no manually duplicating jobs per environment
* Easy to view history, diff, blame

---

### More good parts - Pipeline
* Use all your favourite Jenkins plugins (well, most of them)
* Execute Groovy code within build - programatically alter your build across environments
* Easy credential management
* Durable
* Blue Ocean

---

### The bad parts

* Learning curve
* Longer to get jobs set up
* Documentation isn't great
* Plugin support often not perfect

Note:
Requires trial and error to get started.

---

### Others
* Teamcity - Kotlin DSL
* Gitlab - YAML DSL
* Travis CI
* Pretty much all CI solutions

Note:
* YAML is easier to get up and running, but offers less flexibility.

---

### Should you use it?

Note:
* On any decent sized project, yes. Benefits of keeping build maintainable outweigh initial setup cost.
* We've been using it on Sanctuary and gone from 12 environments with 3-5 builds down to a single pipeline.
* Setup cost will only decrease as you get used to it.
* On smaller projects, you may be able to get away with manual config. But more lightweight CI solutions would be worth considering.