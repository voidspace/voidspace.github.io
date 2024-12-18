---
layout: page
title: Advanced Python
permalink: /advanced/
---

Advanced Python is a modular course that can be tailored to the clients needs. Typically taught as a three day hands on course that will take you deeper into the Python programming language and ecosystem. This course will take delegates from beginner/intermediate level in Python to Advanced Python experts. The course provides a solid overview of the Python language including some low level details essential to working confidently and fluidly with Python. The focus is on practical programming and the skills learned here can be applied in any field where Python is used.

This course is taught by Michael Foord. Michael has been teaching Python for over a decade and has over twenty years industry experience as an application developer. Michael is a Python core developer and the creator of [unittest.mock](https://docs.python.org/3/library/unittest.mock.html) in the Python standard library, and is the author of [The Absolute Minimum Every Python Web Application Developer Must Know About Security](https://opensource.net/essential-python-web-security/).

In this course delegates will learn a great deal of Python, from an essential foundation like how assignment works to taking advantage of multicore systems with multiprocessing. Included is networking, from API clients to understanding sockets and how servers work - the request response cycle of the REST API model, language features like closures, generators, context managers and the whole Python object model along with testing with pytest.

For smart programmers this course provides a solid foundation for working with Python along with many advanced language features and concepts and powerful libraries for tackling many common programming scenarios. As well as learning and discussion every section is backed by lab exercises.

Full list of modules available:

* Exceptions and the Call Stack
* Closures and Decorators
* Concurrency
* Context Managers and \_\_init_subclass__
* Iterators, Generators, References and Assignment
* Imports, Modules and Namespaces
* Networking
* The Core Python Object Model
* Testing with pytest
* Floats, Unicode, and Regular Expressions
* List Comprehensions and Generator Expressions
* Advanced Python OOP

An additional optional module "Data Science Overview" is available on request.

To add:

* New module on functions coming soon
* Module on datetime handling

# Modules

## Exceptions and the Call Stack

A section covering the full Python exception syntax and behaviour, including best practises around exception handling and the new ExceptionGroup language features. In order to fully understand exception handling in Python we have to understand Python as a running system with stack frames and local variables, which we can explore with a debugger.

* Exception type and message
* Basic exception handling syntax
* Exception objects
* Avoiding over-broad exception handling
* Best practises for exception handling
* The exception type heirarchy
* Creating and raising your own exceptions
* Full exception handling syntax:
    - Handling multiple exception types the same
    - Multiple except blocks for different types
    - Re-raising the current exception
    - Exception chaining
    - The else block
    - Resource management with the finally block
    - Context managers as an alternative for finally
* Exception handling best practises: which exceptions to handle
* Launching code with `python -i`
* The pdb debugger and pdb.pm()
* Stack-frames, local variables, stack traces
* The traceback module
* ExceptionGroup and handling multiple exceptions

## Closures and Decorators

Learning the functional aspects of the Python programming language, like higher order functions and closures, and then putting it to practical use with decorators.

* Functional programming
* Higher order functions
* Functions that take functions
* Lambda functions
* Partical application
* Closures: functions that return functions
* Variable scoping and nested scopes
* The closure machinery
* Closures and nonlocal variables
* Decorators: functions that wrap functions
* Decorator syntax
* Decorators and metadata: functools.wraps
* Decorator factories: decorators that take arguments
* Decorator order and the built-in decorators
* Class decorators
* Class decoration via inheritance with \_\_init_subclass__


## Concurrency

A section on executing multiple tasks in parallel, based on an understanding of the underlying hardware (CPU and operating system), a brief history of concurrency, and working with async (asyncio), threads and multiprocessing. With a discussion of the Global Interpreter Lock, free threading, interprocess communication and shared memory, plus best practises via the actor model (CSP - Concurrent Sequential Programming).

* Concurrency basic principles
* Multitasking on a single CPU; context switching
* True concurrency
* I/O bound and CPU bound tasks
* Processes and the operating system
* Use processes and not threads
* Python and the Global Interpreter Lock (GIL)
* Python 3.13 and free threading
* Async and the event loop
* Await and coroutines
* asyncio.gather and true concurrency with asyncio
* async generators
* Threading and the main thread
* The threading module
* Launching a function on a new thread
* Thread joining, thread cancelling
* Race conditions and mutex locks
* Thread coordination with events, flags and sempahores
* The threading APIs
* Thread pools
* Concurrency with multiprocessing
* Process lifetime management
* The actor model with queues, processes and object passing
* Shared memory with multiprocessing

To add:

* Verify thread pool content
* Thread local variables
* Free threading with C/Cython/Rust extensions
* Launching processes with the subprocess module
* Interpreters as a third party module
* Distributed systems with task queues (RabbitMQ and celery)
* The pre-fork model with gunicorn and uvicorn (WSGI and ASGI)

## Context Managers and \_\_init_subclass__

Context managers and the with statement are a powerful and integral part of Python. Even basic file I/O uses the with statement. This section explains how context managers and the with statement work, how to write your own context managers, and the tools available in the `contextlib` module to help.

\_\_init_subclass__ is a reasonably recent addition to Python and an amazing tool for customizing class creation. Particularly useful for frameworks that need just a little bit of magic, \_\_init_subclass__ can be used for many of the things that previously required metaclasses. An advanced feature of Python object orientation with practical uses.

* Try/finally for resource management
* With statement for file I/O and locks
* Context managers and exception handling: `pytest.raises(...)`
* Context managers returning a value: `mock.patch(...) as mock`
* The context manager protocol
    - \_\_enter__
    - \_\_exit__
    - Returning a value
    - Handling exceptions
    - The full Python equivalent code
    - \_\_aenter__ and \_\_aexit__ for `async with`
* `contextlib.contextmanager`: context managers written as a generator
* \_\_init_subclass__ method
* Keyword arguments and class construction syntax
* Example with class level caches

## Iterators, Generators, References and Assignment

* The iteration protocol
* \_\_iter__ and \_\_next__ methods
* Delegating to builtin iterators (like listiterator)
* The builting in `next` and `iter` functions
* Stateful iteration with generator functions
* Coroutine behaviour: suspend and resume execution, yielding values
* The `yield` keyword
* Adding iteration support to objects
* References, assignment and mutability
* Names not variables (references not pointers)
* Mutable objects and multiple references
* Identity versus equality
* Call by object
* Object copying

To add:

* `yield from`

## Imports, Modules and Namespaces

Modules and packages are the larger units of abstraction that Python provides, along with functions and classes, for building systems with. Much of the state of a running system lives in the global namespaces of imported modules, the `sys.modules` import cache. We'll look at import syntax, the import machinery, the importance of namespaces and factoring code into modules and packages.

* Import syntax variations
* namespaces and variable lookups
* Global variables
* sys.modules and the import cache
* Module objects
* Module level functionality: \_\_dir\__ and \_\_getattr__
* Packages and the filesystem
* Refactoring modules into libraries
* Refactoring libraries into packages
* Relative import syntax
* Module reloading (how to do it and why not to do it)
* `__import__` and the `importlib` module
* Circular imports, avoiding and fixing
* Executable modules and packages

To add:

* Package distribution and installation
* pip, uv and pyproject.toml

## Networking

Web scraping and API clients use HTTP client code whilst API servers live on the server side and we'll cover both sides of the equations and the request -> response cycle that API clients and servers are built on top of.

* HTTP request response cycle
* The requests module
* HTTP clients for REST APIs
* pip, requirements.txt and venv for project management
* Sockets
* TCP/IP
* TCP and UDP, IPv4, IPv6
* TCP server / client
* UDP Server / client

To add:

* Update from requests to httpx
* Update based on networking section from "Essential Python Web Security"

    - Network Layers
    - Application Protocols
    - Sockets
    - DNS
    - Request Response Cycle
    - Basic Authentication
    - WebSockets
    - Network Interfaces, Routers and Firewalls
    - Running and Exposing an App Server

## The Core Python Object Model

A look at the whole Python object model from attributes to inheritance to super and the method resolution order. Perhaps the most important module in the course this module describes the behaviour of all Python objects, inside and out.

* Objects as abstractions, for thinking
* Objects, methods and instantiation
* The class statement
* The explicit self
* The initialiser method \_\_init__
* Bound methods
* Attributes and the built-in attribute access functions
* Class attributes
* Class methods
* Properties
* Private attributes
* Single inheritance
* Inheritance to extend and modify the parent
* The use of super
* Cooperative multiple inheritance
* Mixin Classes
* Attribute lookup and the method resolution order
* The type system: isinstance and issubclass
* Inside Python objects and classes
* The instance dictionary
* Slots
* Class dictionaries
* Composition over inheritance
* Magic methods and Python protocols
* Operator overloading
* The string representation protocol
* The container protocols
* Implementing custom containers

To add:

* Inheriting from collections.abc.MutableSequence
* Python protocols
* Abstract Base Classes
* Alternative approaches:

    - named tuples
    - `typing.NamedTuple`
    - dataclasses
    - type as a class factory

## Testing with pytest

* virtual environments and pipenv (installing pytest)
* pytest command line for collecting and running tests
* Simple test functions and asserts
* Test fixtures and conftest.py
* Testing exceptions with `pytest.raises`
* Test parameterisation for test combinations
* Test marking for running test subsets
* Principles of testing (unit tests versus end to end testing, building test helpers etc)
* Mocking and patching
* Testing API servers with Flask and pytest test client

To add:

 * More detail on testing principles
 * Update to uv instead of pipenv

## Floats, Unicode, and Regular Expressions

The minimum every developer must know about floating point numbers, unicode, and character encodings. Along with a fast paced but in depth look at regular expressions. The exercises illustrate a Test Driven Development approach with unittest.

* Floating point numbers
* Unicode, encodings and strings
* Regular expressions

## List Comprehensions and Generator Expressions

* For loops and iteration
* Tuple unpacking, multiple iteration variables
* Keeping track of iteration with `enumerate`
* Combining iterators with `zip`, iteration over pairs
* Building dictionaries with zip and item, value pairs: `dict(zip(keys, values))`
* List comprehension syntax
* How to read list comprehensions (from the middle)
* List comprehensions with filters
* List comprehensions and query like syntax
* Eager versus lazy: list comprehensions versus generator expressions
* Generator expressions as one shot iterators
* Ordered dictionaries
* Ternary expressions

To add:

* The `safe` argument to `zip`
* Nested list comprehensions
* Dictionary and set comprehensions (in the exercises already - verify)


## Advanced Python OOP

An module on some advanced features of the Python object model. Useful for building larger systems, a full understanding of the Python object model, and the creation of frameworks or understanding the mechanisumes used by frameworks.

* Two phase object creation
* Weak references
* Destructors
* Metaclasses

To add:

* \_\_getattr__ and customising attribute access
* The descriptor protocols
    - The magic behind methods, properties, slots and classmethods
    - object.\_\_getattribute__
    - Writing custom descriptors
