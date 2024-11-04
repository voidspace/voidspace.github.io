---
layout: post
title: 'Python Knowledge Sharing Videos Online'
---

{% include youtube.html id="O25ro9U2Br4" %}

I've been teaching Python in one hour knowledge sharing sessions, some of which I've put online on youtube.

This is the link to the playlist of the sessions:

* [Python Knowledge Share Videos on YouTube](https://www.youtube.com/watch?v=O25ro9U2Br4&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&ab_channel=MichaelFoord)

The slides for each of the sessions, along with some example code, can be found in this github repository:

* [https://github.com/voidspace/talks](https://github.com/voidspace/talks)

So far there are seven one-hour sessions (with more planned) on:

* [Python Core Object Model](https://www.youtube.com/watch?v=O25ro9U2Br4&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=1&ab_channel=MichaelFoord)
    * Python objects
    * Slots
    * Attribute lookup and the MRO
    * Inheritance, multiple inheritance and super
    * Inside Python objects and classes
* [Closures and decorators (functional programming)](https://www.youtube.com/watch?v=koannusBFGU&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=3&ab_channel=MichaelFoord)
    * Functional programming: higher order functions and functions as objects
    * Lambdas
    * Closures: functions that build functions
    * Variable scoping: global, local and nonlocal
    * Decorators: functions wrapping functions
    * Decorator factories (decorators that take arguments)
    * Class decorators
    * Decorator order and using functools.wraps
* [Generators and Iterators](https://www.youtube.com/watch?v=yadfyn6-TzE&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=4&ab_channel=MichaelFoord)
    * The iteration protocol
    * Stateful iteration with generators
    * Adding iteration support to objects
    * References, assignment and mutability
    * Identity versus equality
    * Call by object
    * Object copying
* [Unicode, Floats and regex](https://www.youtube.com/watch?v=X3RBs0zau2w&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=5&ab_channel=MichaelFoord)
    * Floating point numbers
    * Unicode, encodings and strings
    * Regular expressions
* [Concurrency (async, threads, processes, the GIL)](https://www.youtube.com/watch?v=fwb1u-V81sk&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=2&ab_channel=MichaelFoord)
    * The history of concurrency from AmigaOS to a multi-core world
    * Python and the Global Interpreter Lock
    * I/O bound and CPU bound tasks
    * Threads and processes
    * Async programming (green threading, coroutines)
    * Concurrency with threads
    * Concurrency with multiprocessing
    * Looking to the future (Python 3.13): optional GIL (PEP 703) and subinterpreters (PEP 554)
* [Testing with pytest](https://www.youtube.com/watch?v=ZgfpAXAB_0Y&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=7&ab_channel=MichaelFoord)
    * virtual environments and pipenv (installing pytest)
    * pytest command line for collecting and running tests
    * Simple test functions and asserts
    * Test fixtures and conftest.py
    * Testing exceptions
    * Test parameterisation for test combinations
    * Test marking for running test subsets
    * Principles of testing (unit tests versus end to end testing, building test helpers etc)
    * Mocking and patching
* [Modules and Namespaces](https://www.youtube.com/watch?v=VuKWsoDogq8&list=PLzeg33w0Au4wgaHk3-hyGIXNU_WRBMgvq&index=8&ab_channel=MichaelFoord)
    * Import syntax variations
    * namespaces and variable lookups
    * sys.modules and the import cache
    * Module objects
    * Module level functionality: \_\_dir\__ and \_\_getattr__
    * Packages and the filesystem
    * Relative import syntax
    * Module reloading (how to do it and why not to do it)
    * Circular imports, avoiding and fixing
    * Executable modules and packages

## Other Talks

A selection of some of the talks and interviews I've given on Python and software engineering across my career.

* [UK Health Security Agency Software Development Practise Conf 2024](https://github.com/voidspace/talks/blob/main/healthsecurityagency/ukhsa.pdf)
* [PyCon MEA 2022 How Python Took Over the World](https://www.youtube.com/watch?v=gv8VA1KugWk&ab_channel=GlobalDevSlam)
* [Test and Code Podcast Episode 145: For Those About to Mock](https://testandcode.com/145)
* [PyCon Belarus 2020 How Python Took Over the World](https://www.youtube.com/watch?v=EFJzsKvi8lU&t=17s&ab_channel=SPACE)
* [PyLondinium 2019 The Python Object Model](https://www.youtube.com/watch?v=qqW4QYTeD40&ab_channel=PyLondinium)
* [Interview on Podcast.\_\_init__ on testing, Mock and the Python community (2018)](https://www.podcastinit.com/michael-foord-on-testing-mock-tdd-and-the-python-community-episode-171/)
* [The Role of Abstractions: Lightning Talk PyCon US 2018](https://youtu.be/c-I0md_3fbQ?t=275)
* [Best Practises for Software Development and Testing (2017)](https://opensource.com/article/17/5/30-best-practices-software-development-and-testing)
* [PyCon UK Panel 2015](https://eventil.com/presentations/L1see4-michael-foord-the-pycon-uk-panel)
* [To the Clouds: EuroPython 2015](https://pyvideo.org/europython-2015/to-the-clouds-why-you-should-deploy-to-the-cloud-even-if-you-dont-want-to.html)
* [Automated Deployments with Juju: PyCon UK 2014](https://pyvideo.org/pycon-uk-2014/repeatable-automated-deployments-with-juju.html)
* [Python and Pythons: PyCon NZ 2013](https://www.youtube.com/watch?v=IWB_pQacuw4)
* [Testing with Mock: PyCon US 2011](https://pyvideo.org/pycon-us-2011/pycon-2011--testing-with-mock.html)
* [New and Improved unittest 2: PyCon US 2010](https://pyvideo.org/pycon-us-2010/pycon-2010--new--and--improved--coming-changes-to.html)
* [Michael Foord on IronPython: Hanselminutes 2009](https://player.fm/series/hanselminutes-fresh-talk-and-tech-for-developers/ironpython-with-michael-foord)
* [Michael Foord on IronPython: TechEd 2007](https://www.youtube.com/watch?v=aSYT52Q8Mf4)
