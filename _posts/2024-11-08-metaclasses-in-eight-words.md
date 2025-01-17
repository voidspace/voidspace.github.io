---
layout: post
title: 'Python Metaclasses in Eight Words'
---

![Metaclasses]({{ site.baseurl }}/images/metaclasses.jpg)

Python metaclasses, considered advanced programming and Python "black magick" (*) explained in eight words:

*The type of a class is a class.*

Here's what knowledge of Object Oriented theory and type systems permit you to deduce from this:

Using the word "class", instead of "the type of a class is type" or even "the type of a class is a type, classes are types", implies that a user defined class can be a metaclass. This is indeed the case, and the point of metaclasses in Python.

The type is responsible for creating new instances. So if the type of a class is a class then we can write classes that create classes. Indeed this is the primary usecase for metaclasses.

(Deeper knowledge of Python, and the two phase object creation protocol, may lead you to deduce that this is done by overriding the \_\_new__ method. If you're familiar with "type" as a class factory you can probably even guess the signature and that you must inherit from type.)

If the type of a class is a class then the type system will permit a type check for the class against its class. And indeed isinstance(klass, metaclass) returns true.

(And deeper knowledge of Python will tell you that the magic methods, the protocol methods, are always looked up on the type. So we can implement behaviour for class objects by providing magic methods on the metaclass.)

All of this implies that classes are themselves objects. Which is true in Python for everything is an object in Python (and everything is a reference).

And so on...

* Type and class are synonyms in Python.
* type(type) is type

And to further round out the type system, these are also Python invariants:

* isinstance(object, object) is True # object is an object
* isinstance(object, type) is True # but also a type
* isinstance(type, object) is True # type is an object
* isinstance(type, type) is True # but also a type

(*) Like all black magick it is useful for understanding the world but never for actual use. Well, except perhaps in very rare circumstances if you know what you're doing.