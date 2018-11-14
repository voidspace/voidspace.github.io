---
layout: page
title: Effective Testing with unittest and mock
permalink: /effective-testing/
---


Learn practical testing techniques for both unit testing and end-to-end testing using standard Python testing tools. A two or three day course.

This exercise driven course covers the mechanics of writing tests and a test framework, practical tips for writing test support code, common testing patterns and anti-patterns and an in-depth example driven exploration of both [unittest](https://docs.python.org/3/library/unittest.html) and [mock](https://docs.python.org/3/library/unittest.mock.html).

### Syllabus

* Testing Styles

  TDD, BDD, test first, functional tests, integration tests, unit tests. Tests as specification. The what and why of testing; different styles and basic terminology.

* unittest introduction

  unittest basics, test modules and test cases, test discovery and test suites. Assert methods and running tests. Structuring your test system. Set up and tear down and friends.

* Unit testing

  Test to the unit of behaviour and not the unit of implementation. Seeing your tests fail first. Why code structure matters. The standard principles of unit testing with Python. 

* Functional testing

  Techniques for the automated end-to-end testing of systems and discussion of particular difficulties of functional testing and the trade-offs between issues like test isolation and test run time. Test plans and owning product quality. Testing web applications with Selenium (or Nightwatch).

* Testing performance and other tips

  Performance testing has its own particular challenges. Along with discussion of other useful testing tips like avoiding voodoo sleeps.

* Mocking, how and why

  Why use mock objects at all? Good mocking and bad mocking.

* Mock and MagicMock and friends

  How to use, and how not to use, the mock objects provided by the unittest.mock module.

* The patch decorator and context manager

  How to wield patch for effective testing with mock objects.

* mock tips and tricks

  A good collection of common gotchas and common patterns for testing with mock objects.

* Workflows and Infrastructure

  Is CI/CD (Continuous Integration/Continuous Deployment) possible or appropriate for your situation? Is it something to work towards. What about smoke tests and gated check ins, issue management, kanban boards? Managing your test project and support libraries, including supporting multiple versions of a product or system under test.

* Other Tooling

  Code coverage, how much value is this and how do we integrate it? Linters, PEP 8 compliance and code quality checking tools.

* py.test comparison and equivalents (Optional)

  An optional section showing the equivalent testing techniques using py.test instead of unittest and demonstrating some of the additional capabilities of py.test like test functions and fixtures.

