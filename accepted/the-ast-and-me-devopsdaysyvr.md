Title:
------
The AST and Me

Conference:
-----------
DevOpsDays Vancouver
April 20-21, 2018
Vancouver, B.C.

Abstract/Elevator Pitch (max 300 characters):
---------------------------------------------
Get under the hood and learn about Python's beloved Abstract Syntax Tree. We'll discuss the AST's role in Python's compilation process, how it affects Bytecode, and how you can use it's optimizations to improve your code's speed at runtime. Write better code!

Talk Format:
------------
Talk - 25 minutes

Audience Level:
---------------
Intermediate

Description:
------------
Python is a wonderfully accessible language for novice and veteran programmers alike. Understanding how Python works can be a key step in writing better code.

Ever wonder how Python code is run? Overheard people arguing about whether Python is interpreted or compiled? In this talk, we will delve into the lifecycle of a piece of Python code in order to understand the role that Python's Abstract Syntax Tree plays in shaping the runtime of your code. Utilizing your newfound knowledge of AST optimizations, you will better understand how Python code is compiled in order to write better code.

Outline:
--------
* Intro (1 minute)
    - Quick introduction of me and my motivation for giving this talk
* Why should you care about Python internals? (2 minutes)
    - Why a bit of knowledge about Python internals goes a long way - from code speedups to understanding tracebacks
* A brief overview of compiling a piece of Python code - from source code through bytecode and execution, focusing on the role of the AST. 5,000-foot overview. (3 minutes)
    - Build an understanding of the broad steps it takes to compile a piece of Python code
* Current optimizations built into the AST (and ones that could be) (3 minutes)
    - What does one gain from optimizing the AST?
    - How is the AST optimized?
    - Constant folding, dead code elimination, copy propagation. (Easy, quick descriptions of each)
* Using the AST module to inspect a piece of code (4 minutes) (*This section will go through some trial and error when preparing and it may be best to simplify for brevity. Less code with better understanding is better, using `dis` may muddy the waters)
    - Code examples of:
        - Using the built-in AST module to inspect a few small piece of code
        - Using dis to inspect the bytecode from the example
        - Running the dissected code
* How the AST affects your bytecode, and how your bytecode affects your runtime (5 minutes)
    - Spoiler alert: it creates those *.pyc and *.pyo files! And those contain bytecode.
    - Mention the difference between *.pyc files and *pyo files.
* Motivating examples of ways to optimize your code to take advantage of AST and other compiler optimizations (5 minutes)
    - Ways to write code differently to generate the most optimized AST and, therefore, bytecode
    - Reasons to inspect the AST instead of bytecode (and why your bytecode still matters)
* Conclusion/Next steps/Resources (2 minutes)
    - Mention Victor Stinner's FAT Python project and PEP 509-511 - super exciting things for the future of Python internals


Notes:
------
* Please note: I plan on giving this talk locally at events, but this would be my first time speaking at a larger, regional conference and I would love a speaker mentor!

Bio:
----
Emily Morehouse-Valcarcel is the Cofounder and Director of Engineering at Cuttlesoft, a custom software development company that loves Python, puns, and cuttlefish. After living in the humid Florida for most of her life, she's now in a love affair with the Colorado mountains. A graduate of the Florida State University, Emily holds bachelor's degrees in Computer Science, Criminology, and Theatre.