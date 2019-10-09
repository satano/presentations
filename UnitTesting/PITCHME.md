# Unit Testing

---

@snap[north span-100]
## Auto-tests
@snapend

@snap[midpoint span-100]
- Unit tests
- Integration tests
- Performance tests
- Penetration tests
- ...
@snapend

+++

@snap[north span-100]
## No integration tests
@snapend

@snap[midpoint span-100]
![No integration tests](https://miro.medium.com/max/300/1*SLmk-xp-dv7aS8XLabqlwA.gif)
@snapend

---

@snap[north span-100]
## Why unit tests
@snapend

@snap[midpoint span-100]
- More confident that the code is correct
- Later refactoring is easier
- Sandbox for using new features
- Testing without waiting for others
@snapend

---

@snap[north span-100]
## Unit tests are
@snapend

@snap[midpoint span-100]
- Fast
- Isolated
- Independent
- Robust
- Maintainable
- Purposeful
@snapend

+++

@snap[north span-100]
## Fast
@snapend

@snap[midpoint span-100 text-08]
A unit test should run very fast. Having fast unit tests means they can be run often. This is a very important quality, especially in the refactoring process, where instant feedback is crucial. Slow unit tests will cause them to be run seldom, making them next to useless as a refactoring tool.
@snapend

+++

@snap[north span-100]
## Isolated
@snapend

@snap[midpoint span-100 text-08]
A unit test should test its assigned unit of functionality in isolation. What this means is that the unit should be isolated from other units of functionality during testing. Stubs, mocks and dummy components should be used in place of any dependency the unit might have.
@snapend

+++

@snap[north span-100]
## Independent
@snapend

@snap[midpoint span-100 text-08]
A unit test should be self sustained, and not depend on any other test in order to be able to run. There is typically no guarantee on the execution order of unit tests, so any introduced causality between tests can be harmful.
@snapend

+++

@snap[north span-100]
## Robust
@snapend

@snap[midpoint span-100 text-08]
A unit test should be designed as robust as possible. It should produce a deterministic result which is independent of external concerns. No matter how many times the test is run, the time of day it is run, what locale and environment it is run in, or any other influences, the test should give the same result.
@snapend

+++

@snap[north span-100]
## Maintainable
@snapend

@snap[midpoint span-100 text-08]
A unit test should be easy to maintain. In the same way that production code is refactored, unit tests also have the need to be changed and improved. If the unit test is well written and easy to understand, it will make the task of maintaining it much simpler. As a general rule you should strive to have the same code quality in your unit tests as in your production code.
@snapend

+++

@snap[north span-100]
## Purposeful
@snapend

@snap[midpoint span-100 text-08]
A unit test should have a clear purpose. It should test a small piece of functionality, and it should test it well. When writing a unit test you should know what the preconditions are, what you want to test and what the expected result should be. Using a sensible naming standard for unit tests will help in expressing the purpose of a test, and will make it easy for other to understand what the test does.
@snapend

---

@snap[north span-100]
## Code Coverage & TDD
@snapend

@snap[midpoint span-100]
- **Code coverage:** How much source code is covered by tests.
- **TDD:** Test Driven Development. First tests, than code.
@snapend

---

@snap[north span-100]
## Unit tests myths
@snapend

@snap[midpoint span-100]
- They slow down development
- They are expensive
- They are difficult
- 100 % coverage means no bugs
@snapend

---

@snap[north span-100]
## Hard to test code
@snapend

@snap[midpoint span-100]
- Static properties, fields and methods
- Singletons
- The `new` operator
@snapend

---

@snap[north span-100]
## Testable code
@snapend

@snap[midpoint span-100]
@size[5em](**S O L I D**)
@snapend

---

@snap[north span-100]
## @size[0.9em](Anatomy of a test (AAA))
@snapend

@snap[midpoint span-100 text-09]
- **Arrange:** Create and setup system under test (SUT).
- **Act:** "Run" the SUT (usually invoke some method).
  - Test "standard" cases.
  - Test edge cases.
- **Assert:** Check result, state, expected side effect...
@snapend

---

@snap[north span-100]
## Tools
@snapend

@snap[midpoint span-100]
- Testing framework ([xUnit](https://xunit.net/), [NUnit](https://nunit.org/), [JUnit](https://junit.org/))
- Mocking library ([NSubstitute](https://nsubstitute.github.io/), [Moq](https://github.com/moq/moq4))
- Assertions library ([FluentAssertions](https://fluentassertions.com/))
@snapend

---

@title[Questions]

# @size[2.5em](@fa[question-circle])
