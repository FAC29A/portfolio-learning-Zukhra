# Learnings on Automated Testing

## Overview

In weeks 7 to 9 of the learning program, I delved into the crucial aspect of software development - testing. This period focused on understanding how to ensure the correctness of code through the creation of automated tests.

## Topics Covered

### Introduction to Testing

The initial phase provided an introduction to the fundamental concepts of testing in software development. This laid the groundwork for the subsequent workshops.

### Workshops

#### 1. Build a Testing Library

The concept of testing code is often introduced with complex libraries. This hides the core of testing: writing some code that runs your other code and tells you if it’s wrong. This workshop introduces the concept by slowly building up a useful and reusable function that helps you test your code.
```javascript
// Testing function to check if two values are equal
function equal(actual, expected, message) {
  if (actual === expected) {
    const defaultMessage = `Expected ${expected}, and received ${actual}`;
    console.info("Pass: " + (message || defaultMessage));
  } else {
    const defaultMessage = `Expected ${expected}, but received ${actual} instead`;
    console.error("Fail: " + (message || defaultMessage));
  }
}

// Testing function to check if two values are not equal
function notEqual(actual, expected, message) {
  if (actual !== expected) {
    const defaultMessage = `${expected} is different from ${actual}`;
    console.info("Pass: " + (message || defaultMessage));
  } else {
    const defaultMessage = `${expected} is the same as ${actual}`;
    console.error("Fail: " + (message || defaultMessage));
  }
}
````

#### 2. Unit Testing Workshop

The unit testing workshop was dedicated to understanding the principles and practices of unit testing. Practical exercises allowed for the application of these concepts to real-world scenarios.

**Unit Testing Description:**
Unit testing involves testing individual units or components of a software to ensure they perform as expected. 

#### 3. Integration Testing Workshop

Integration testing, a critical aspect of ensuring components work together seamlessly, was explored in this workshop. Practical examples provided a deep understanding of integration testing methodologies.

**Integration Testing Description:**
Integration testing focuses on testing the interaction between different components or modules of a system.

#### 4. TDD Workshop

Test-Driven Development (TDD) was a central theme of this workshop. I learned how to approach development by writing tests before implementing features, enhancing code reliability.

**TDD Description:**
Test-Driven Development is a methodology where tests are written before the actual code. This promotes a clear understanding of requirements and ensures that the codebase remains maintainable. 


## Key Takeaways

- **Understanding Testing Fundamentals:** Acquired foundational knowledge about the importance of testing in the software development life cycle.

- **Building a Testing Library:** Developed a hands-on understanding of creating a testing library, a valuable skill for implementing effective testing strategies.

- **Unit Testing Mastery:** Explored the intricacies of unit testing, mastering techniques to validate individual units of code.

- **Integration Testing Expertise:** Gained expertise in integration testing, ensuring components work seamlessly together.

- **Test-Driven Development (TDD):** Embraced the TDD methodology, learning how to write tests before implementing features for more robust code.

