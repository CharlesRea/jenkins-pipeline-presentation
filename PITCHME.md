# Jenkins Pipeline

## Or why your CI should be in code

---

### What is Pipeline?

* Configure your Jenkins builds using code
* Groovy DSL
* Source controlled build config

---?code=Jenkinsfiles/1-HelloWorld&lang=groovy&title=Hello World
@[2](Specify where your builds will be run)
@[3-4]
@[5-7]

Note:
Show on Jenkins. Show on Blue Ocean. Source: Jenkinsfiles/1-HelloWorld

---
### Random notes
* Parallel
* Blue Ocean
* Declarative vs scripted
* Multibranch

---

## Why use it

* Code reviews of changes
* Easily keep changes in sync across branches
* Avoid duplication of jobs
* Easy to view history, diff, blame

---

## Reasons not to use it

* Longer to get jobs set up
* Documentation isn't great
* Plugin support is usually good, but often not perfect

---

## Others
* Teamcity - Kotlin DSL
* Gitlab - YAML DSL
* Travis CI
* Pretty much everything