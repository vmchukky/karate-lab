## Hello World, really?#@!
Every feature will have a name, and one or more Scenarios
```
Feature: Hello Karate

Scenario: demonstrate JSON assertions
```
A Scenario can have `Given`, `When`, `And`, `Then` 
``` 
# as expected is the prefix for comment lines
* def theTestTool = 
"""
{
  what: 'yet another web-service test automation tool',
  BUT: 'we already have curl, postman, rest-assured, cucumber, spock, jmeter/gatling (perf), <what-ever-other-tool> why one more',
  YES: 'it is by-far the simplest tool to stitch a sequence of web-service calls and assert responses',
  features: {
    languageNeutral: {
      syntax: 'simple to deal with HTTP, JSON, GraphQL or XML',
      vocabulary: ['Given', 'When', 'And', 'Then'],
      example: "
        Given url 'https://duckduckgo.com'
        And param q = 'intuit karate'
        When method GET
        Then status 200
      ",
      betterExample: 'is at https://gist.github.com/ptrthomas/d5a2d9e15d0b07e4f1b46f692a599f93'
    },
    reuse: 'call other test cases (features), javascript functions, Java code',
    config: 'easy to switch environment specific configuration',
    assertions: 'simple but powerful (beats json-schema), support for jsonpath, xmlpath, regex',
    data: 'supports dynamic driven tests',
    mock: 'test-doubles'
  }
}
"""
```
how about some #ignore, #notnull, #object
```
Then match theTestTool contains 
"""
{
  BUT: '#ignore',
  YES: '#notnull',
  features: '#object'
}
"""
```
for the love of #regex?
```
And match theTestTool.features contains 
"""
{
  assertions: '#regex .*beats json\\-schema.*',
  mock: '#string'
} 
"""
```
finally what good is a hello world without printing some message
```
And print 'Awesome karate simple example:', theTestTool.features.languageNeutral.example
```