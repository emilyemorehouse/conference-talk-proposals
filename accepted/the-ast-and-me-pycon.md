Title:
------
The AST and Me

Conference:
-----------
PyCon 2018
May 9-17, 2018
Cleveland, OH

Talk Format:
------------
Talk - 30 minutes

Description:
------------
Get under the hood and learn about Python's beloved Abstract Syntax Tree. Ever wonder how Python code is run? Overheard people arguing about whether Python is interpreted or compiled? In this talk, we will delve into the lifecycle of a piece of Python code in order to understand the role that Python's Abstract Syntax Tree plays in shaping the runtime of your code. Utilizing your newfound knowledge of Python's AST, you'll get a taste of how you probably already rely on ASTs and how they can be used to build awesome tools.

Who and Why (Audience):
-----------------------
This talk can spark interest in people in many different ways, from a desire to understand how Python's internals work at a high level and how that can inform better code, to using an AST to lint code or build new tools (with Python or many other languages). Many talks have used Python's bytecode and code objects to delve into Python's internals, but you don't have to go that far! The AST is an excellent bridge to understand how your code works and the optimizations applied to your code at that level.

I expect audience members to have a working knowledge of Python in order to understand the code that's being used (code for simple print statements, if/else statements, for loops and lambdas are dissected into their AST and bytecode, and audience members should not be caught up on what a lambda is, for example). It would be ideal for audience members to have an idea of how an interpreted language is structured and how compilers work, but I'll go through the highlights of crucial knowledge for this at the beginning of the talk. For these reasons, I would consider this talk to be geared toward "Intermediate" individuals.

The audience should walk away with a better understanding of how Python and its compiler works, how to interact with and visualize their code in new ways, useful knowledge about Python's optimizations, and a variety of applications of using ASTs to build cool tools.

Outline:
--------
* INTRODUCTION AND OUTLINE                      (2 minutes, 2 total)
    - Quick introduction of myself
    - Outline of what will be covered and what you will learn
    - My motivation for giving this talk
* WHY?                                          (1 minute, 3 total)
    - Why should you care about Python internals?
    - Why a bit of knowledge about Python internals goes a long way
* OVERVIEW                                      (4 minutes, 7 total)
    -  Is Python interpreted or compiled?
    -  What is an Abstract Syntax Tree?
    -  Life cycle: a brief overview of compiling a piece of Python code - from source code through bytecode and execution, focusing on the role of the AST. 5,000-foot overview.
    -  Build an understanding of the broad steps it takes to compile a piece of Python code
* TOOLS FOR WORKING WITH ASTS - PART 1          (6 minutes, 13 total)
    - Primary (built-in to Python): AST and DIS modules
    - Secondary (third party): astor, meta, codegen
    - Code examples to walk through how the AST and bytecode are represented and accessed:
        - Using the built-in AST module to inspect a few small piece of code
        - Using dis to inspect the bytecode from the example
        - Running the dissected code
    - Side-by-side comparisons of the visualization of an AST and its bytecode for a few simple pieces of code
* CURRENT COMPILER OPTIMIZATIONS                (4 minutes, 17 total)
    -  Current optimizations built into the AST (and ones that could be)
    - What does one gain from optimizing the AST?
    - How is the AST optimized?
    - Constant folding, peephole optimizations - easy, quick descriptions of each
* TOOLS FOR WORKING WITH ASTS - PART 2          (6 minutes, 23 total)
    - Examples of how constant folding and peephole optimizations can affect your AST and bytecode
* AST -> BYTECODE -> RUNTIME                    (2 minutes, 25 total)
    - How the AST affects your bytecode, and how your bytecode affects your runtime
    - Spoiler alert: it creates those *.pyc and *.pyo files! And those contain bytecode.
    - Mention the difference between *.pyc files and *pyo files.
* PRACTICAL/OPTIMIZATION EXAMPLES               (3 minutes, 28 total)
    - Motivating examples of ways to optimize your code to take advantage of AST and other compiler optimizations
    - Applications within Python:
        - Improve and speed up your code
        - Debug errors
        - Change the Python grammar
        - Round-Tripping
        - Code generators
        - Alternative interpreters
    - Applications outside of Python
        - Code analysis
        - Code linting
        - Tools such as Post-CSS and Babel
* CONCLUSION / NEXT STEPS / RESOURCES           (2 minutes, 30 total)


Additional Notes:
-----------------
By the time PyCon 2018 rolls around, I will have given this talk to at least two local meetups and one smaller regional conference.

I've been working on delving into CPython source code for over a year with the mentorship of some of Python's core developers and have been particularly interested in the internals of its compiler and optimizations.

Bio:
----
Emily Morehouse-Valcarcel is the Cofounder and Director of Engineering of Cuttlesoft, a digital product development agency focused on creating beautifully designed and highly scalable custom software. Her passion is driven by the unique blend of empathy, strategy, curiosity, and human-centered design. When she isn’t leading Cuttlesoft, Emily is an avid Open Source Software contributor and constant learner with side projects focused on automating the mundane, improving daily life, and shedding light on the complexity of the human experience. A graduate of the Florida State University, Emily holds bachelor's degrees in Computer Science, Criminology, and Theatre.
