---
layout: post
title: 'The Role of Abstractions in Software Engineering'
---


This is a video and text of a lightning talk, a five minute presentation, given at PyCon US 2018 in Cleveland.

This is an abstract talk. There isn’t time to give examples but I hope that the application to the day to day challenges of the practise of software engineering is clear. The only theory worth a damn is the theory of the practise. This is a talk about the role of abstractions in software engineering.

Programming is all about the use of abstractions. We often say that the fundamental language spoken by the machine is ones and zeros. Binary. This isn’t true. Ones and zeroes are an abstract representation of the fundamental operation of computers. It’s a way of representing what central processors do in a way that can be understood by people.

The actual language spoken by computers is the electromagnetic dance across wires and etched silicon, choreographed by the beating of a quartz crystal at the heart of the machine.

Ones and zeroes are a representation of that dance, understandable by humans in order for us to reason about the behaviour of the system.

That’s a very low level abstraction. Very close to the actual operation of computers, but very hard to work with. The next step up is assembly language where we use mnemonics, symbolic instructions like JMP for jump, to represent these patterns of ones and zeroes. We can also use human recognisable labels for memory locations instead of numbers and allow the assembler to calculate offsets for us. Much easier.

Next we have languages like C and then right at the very top we have Python where each construct, a print statement for example, may correspond to as many as millions of the lowest level operations.

Computer programming is communication in two directions. Programming provides a language the computer understands, and is able to execute deterministically, whilst also communicating with humans so they can conceptualise the behaviour of the system. A programming language is a set of conceptual tools to facilitate that communication in both directions.

The art and craft of software engineering is taking the conceptual tools that programming languages provide and using them to solve real world problems. This is the difference between science and engineering. Science is the theory, engineering is the application.

In order to be able to do this we have to have an understanding of the problem domain. We conceptualise it. We think about it. Software is easy to understand and maintain when the abstractions you build map well to the problem domain. If the way you think about the problem is close to the way you think about your software then you have to do less mental translation between the problem and your code.

Joel Spolsky talks about the law of leaky abstractions. Any abstraction that maps to lower level operations in the system will leak. At some point something will go wrong and you will only be able to fix it by understanding the lower level operations too.

I’ve heard it said, and it rings true, that a good programmer can hold about ten thousand lines of code in their head. So if your system is less than ten thousand lines of code, even if it’s terrible code, you don’t need to build higher level building blocks to hold it in your head.

An all too common situation is that a system becomes too complex to reason about, so an engineer decides to create abstractions to simplify how they think. So they create black boxes, abstractions, in which to place the complexity. These type of abstractions conceal complexity. So now you don’t have to look at the mess you just made.

You can reason about your system with your abstractions, but in order to understand the actual behaviour (at a lower level) you need to go digging in all that dirt.

Instead of concealing complexity a good abstraction will explain and point you to the lower level operations. Good abstractions simplify and reveal complexity rather than concealing it.

We can also use this kind of reasoning to think about product and system design. What user experience are you providing, what’s the user story? Your users also think about the problem domain using conceptual tools. The closer the abstractions your software presents to your user map to the way they already think about the problem the easier your software will be to use.


And here we come full circle. If the way you build your software maps well to the problem domain then it will be easy to reason about and maintain. If the abstractions you present to the user map well to the problem domain then it will be easier for your users to think within your system and it will be more intuitive to use.



So abstractions matter. They’re the raw stuff of our world.



You can watch the presentation, from the Saturday afternoon lightning talks, four minutes into this video.
