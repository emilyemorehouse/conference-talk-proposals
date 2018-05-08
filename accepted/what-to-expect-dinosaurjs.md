Title:
------
What To Expect When You’re Expecting

Conference:
-----------
DinosaurJS
June 21-22, 2018
Denver, CO

Abstract - Provide a concise description for the program limited to 600 characters or less:
--------------------------------------------------------------------------------------------
We all know we *should* be testing our applications, but testing is hard and *great* testing is even harder. Brush off your knowledge of different types of testing to hone in on exactly what you should test in your applications, and explore different approaches you can take in doing so. Take a deep dive into regression testing with a focus on visual regressions, and figure out what you should put in that `expect()` statement. Learn how to leverage modern headless browser libraries and automated diff-ing to get (and keep) pixel-perfect apps.

Talk Format:
------------
25-30 minutes


Details - Include any pertinent details such as outlines, outcomes or intended audience:
-----------------------------------------------------------------------------------------
## Outline:
* INTRODUCTION AND OUTLINE (1 minute, 1 total)
    * Quick introduction of myself
    * Outline of what will be covered and what you will learn
    * My motivation for giving this talk
* TESTING, WAT? (1 minute, 2 total)
    * We all know we should be writing tests for our code, but what does that really mean?
    * What does writing tests “in the real world” look like?
* OVERVIEW (3 minutes, 5 total)
    * Rapid-Fire Introduction to Testing - 20,000 foot view, short descriptions of different types of testing
        * Unit Testing
        * Integration Testing
        * Regression Testing
        * Functional Testing
        * System Testing
        * Performance Testing
        * Usability Testing
        * Accessibility Testing
        * Chaos Testing
        * Stress Testing
    * What kinds of tests are most impactful for different use cases?
    * Shout out to accessibility testing - it’s surprisingly easy to do and can point out oversights that are very easy to fix and are very impactful
* THE IMPORTANCE OF CONSISTENT REGRESSION TESTING (1 minutes, 6 total)
    *  [Change blindness](http://enacademic.com/dic.nsf/enwiki/1159161) - the human brain isn’t good at remembering minute details of stimuli, and therefore it’s much better to let a computer handle detecting changes, both visual and functional
    * The larger your application gets, the more existing features may (unintentionally) break as you add new code!
* ANATOMY OF A TEST (3 minutes, 9 total)
    * Ingredients:
        * Test environment (e.g., Mocha, Jasmine, Jest, Karma)
        * Testing structure (e.g., Mocha, Jasmine, Jest, Cucumber)
        * Assertions (e.g., Chai, Jasmine, Jest, Unexpected)
        * Mocks, spies, and stubs (e.g., Sinon, Jasmine, enzyme, Jest, testdouble)
        * Browser or browser-like environment (e.g., Protractor, Nightwatch, Phantom, Casper)
    * Process:
        * Generate, display, and watch test results
        * Generate and compare snapshots to make sure changes from previous runs are intended
        * Generate code coverage reports
* WHAT SHOULD YOU EXPECT? (3 minutes, 12 total)
    * Good tests mimic good bug reports:
        * What were you testing?
        * What should it do?
        * What was the output (actual behavior)?
        * What was the expected output (expected behavior)?
* APPROACHES FOR VISUAL REGRESSION TESTING (2 minutes, 14 total)
    * Developers maintain a set of “golden” images, whether screenshots or mocks, that represent what the application *should* look like
    * Tests are run that take screenshots of the current application and compare them against the “golden” set
    * Results can be received as either discrete pixel amounts or an overlay of screenshots with highlighted areas where they differ
* VISUAL REGRESSION TESTING IS EASIER IN 2018 (1 minute, 15 total)
    * Previously, visual regression testing was tied to manipulating an actual browser using tools like Selenium or PhantomJS
    * [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome) makes interacting with your browser much easier since you can control test environments without a visible UI
* WALKTHROUGH - TOOLS FOR VISUAL REGRESSION TESTING  (2 minutes, 17 total)
    * [Puppeteer](https://github.com/GoogleChrome/puppeteer) - Headless Chrome Node API
    * [Resemble.js](https://github.com/Huddle/Resemble.js) - Visual image comparison
    * Runner and assertion libraries of choice - we’ll use Mocha and Chai
* WALKTHROUGH WITH CODE SNIPPETS (this will have a companion repo on GitHub)  (8 minutes, 25 total)
    * Set up your test environment:
        * `before` - start your local server, make sure your directories to store screenshots exists
        * `after` - stop your server
        * `afterEach` - reload your Puppeteer browser
    * Set up a test:
        * Load the Puppeteer browser
        * Set your viewport size, or emulate a specific device
        * Take the screenshot
        * Compare your screenshot with the expected view
    * Example (I would include this as a demo, but this is cool to see the output that you get when your site changes):
        * Original screenshot of DinosaurJS site: ![original screenshot of DinosaurJS site](https://s3.amazonaws.com/dinojs/dinosaurjs.org_original.png)
            * Screenshot of DinosaurJS site with elements moved: ![screenshot of DinosaurJS site with elements moved](https://s3.amazonaws.com/dinojs/dinosaurjs.org_changed.png)
            * Image showing diff between screenshots: ![image showing diff between screenshots](https://s3.amazonaws.com/dinojs/dinosaurjs.org_diff.png)
* CONCLUSION (1 minute, 26 total)
    * Wrap up and call to action

Pitch - Explain why this talk should be considered and what makes you qualified to speak on the topic:
-------------------------------------------------------------------------------------------------------
As a mentor and lead engineer, I’m constantly asked questions about why testing is important, what you should actually be testing, and what testing looks like in the real world. I’m hoping that this talk can shed light on all of those questions to give clarity and confidence to developers when approaching testing. I’m also a huge fan of regression tests and believe that visual regression tests are key to maintaining well-designed and user-friendly sites.

I took care when writing this proposal to cover all audience levels. I find that it’s best to create a foundation with basic information and terminology to give all audience members a chance to understand a more advanced topic. I rely upon finding a happy medium of keeping information simple yet dense, to allow for broad topics to be described quickly so we can move quickly from “what is a test?” to implementing visual regression tests.

This talk will be…
… witty, but not cheesy.
… dense, but accessible.
… code-inclusive, but not code-heavy.

I have 6+ years of experience testing and building applications not only in the JavaScript world but in many other languages and frameworks as well. I believe that my wide range of experience can shed light on this topic and cross-pollinate my approaches to testing.

---

Private Info (revealed after rated):

Bio: (500 character limit):
----------------------------
Emily Morehouse-Valcarcel is the Director of Engineering at Cuttlesoft, a digital product agency focused on creating beautifully designed software. Her passion is driven by a blend of empathy, strategy, curiosity, and human-centered design. She's an avid OSS contributor and constant learner focused on building tools to automate the mundane and shed light on the complexity of the human experience. Emily holds degrees in Computer Science, Criminology, and Theatre from Florida State University.

Online recordings:
-------------------
cut.tl/ast-and-me
