## **What is a Test?**
- code you write to verify the behavior of your application

## **Why Test**
- tests are specifications for how your code should work
- it's DOCUMENTATION for the source code
- consistency 
  - verify that best practices and conventions are being followed
- comfort and confidence!

## **Jest**
- test framework
- provides certain tools:
  - test runner
  - assertion libary
  - utilites for mocking

## **Types of Tests**
(From highest overview to most specific)
- End-to-End
  - simulate user behavior
  - kind of like a robot performing a task in your app
  - Integration
    - verify that multiple units work together
  - Unit
    - verify the functionality of a single function/component
  - Static 
    - catch typos and errors while writing code
    - like ESLint

> want to have a very tight feedback loop and as few dependencies as possible

## **Basic Test Example**
```js
const expected = true
const actual = false

if (actual !== expected){
    throw new Error(`${actual} is not ${expected}`)
}
```

## **A Jest Test**
```js
const expected = true
const actual = false

test("it works", () => { // test runner
    expect(actual).toBe(expected) // the assertion libary provides this
})
```
