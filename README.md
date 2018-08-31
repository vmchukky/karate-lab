# karate-lab
Material that can be used for a karate hands-on lab/workshop

## [karate](https://github.com/intuit/karate):
An open source framework for web service testing (err.., for any/A-to-Z testing, I can dream right).  If you are still not sold on karate, here is some good reading material:
- First and foremost [beautiful documentation in karate README](https://github.com/intuit/karate)
- Easy assertions even for complex json schema: [no problem](https://pbs.twimg.com/media/DDLHXlQUIAEKKP8.jpg)
- [Data driven testing](https://github.com/intuit/karate#data-driven-tests) again the README
- Want to mock (before dev team implemented) a service: [World's Smallest MicroService](https://github.com/intuit/karate/tree/master/karate-netty#the-worlds-smallest-microservice-) 
- For all BDD purists: want to highlight [karate is not true BDD](https://medium.com/@ptrthomas/yes-karate-is-not-true-bdd-698bf4a9be39) (also mentioned in README)

Enough already, show me some code:
- [say hello to world](hello-world.md)
- [who cares about a hello world show me something real](README.md): See `Background`, `variables`, `request`, `header`, `params`, `response`, `status` (TBD)

## Exercise 1
- Stitch a sequence of API calls as one test case (Scenario)
- JUnit/TestNG integration 
- Code reuse, mix and match features, with javascript and java code

(TBD)
## Exercise 2
- json/xml first class citizenship, read/write from/to files
- how to keep secrets out of tests
- Switch configuration/profile (stage -vs- production)
- Pick and choose (test cases, test suites and all that jargon): want to run only smoke tests -vs- full regression 

(TBD)
## Exercise 3
See the power of karate 
- complex assertions
- data driven testing
- flexible logging

(TBD)
## Exercise 4
Didn't I promise karate for A-to-Z?
- performance testing: karate-gatling
- UI testing: karate-selenium
- mocking services: test doubles

(TBD)
## Demo
karate UI
(TBD)