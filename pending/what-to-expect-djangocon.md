Title:
------
What To Expect When You’re Expecting: A Hands-On Guide to Regression Testing

Conference:
-----------
DjangoCon US
October 14-19, 2018 (Tutorials - 14, Talks 15-17)
San Diego, CA

Elevator Pitch:
---------------
We all know we should be testing our applications, but testing is hard and great testing is even harder. Take a deep dive into what and how to test your Django apps, plus learn how to leverage modern headless browser libraries and automated visual diff-ing to get (and keep) pixel-perfect apps.

Talk Format:
------------
Tutorial, 3-3.5 hours

Audience Level:
---------------
Intermediate

About This Tutorial:
--------------------
We all know we should be testing our applications, but testing is hard and great testing is even harder.

Take a deep dive into what types of things to test and how to approach testing them in your Django apps, plus learn how to leverage modern headless browser libraries and automated visual diff-ing to get (and keep) pixel-perfect apps.

We'll cover types of testing as a whole, plus practical applications and deep dives for testing in Django and visual regression testing with Javascript (whether for templates rendered by Django or for a standalone Javascript client application).

Tutorial Outline:
-----------------
## Outline:
* Introduction (10 mins, 10 mins total)
  * Introduction, outline, and expectations of what you should take away from this tutorial
* Foundational Knowledge for Testing (35 mins, 45 mins total)
  * Testing, Wat?
    * We all know we should be writing tests for our code, but what does that really mean?
    * What does writing tests “in the real world” look like?
  * Rapid-Fire Introduction to Testing: 20,000 foot view, short descriptions of different types of   testing
    * What kinds of tests are most impactful for different use cases?
  * The Importance Of Consistent Regression Testing
    * Change blindness
  * Anatomy Of A Test
    * Ingredients for successful testing
    * Process and workflows for testing
  * What Should You Be Testing?
    * Good tests mimic good bug reports
  * Approaches For Regression Testing
  * Approaches For Visual Regression Testing
    * Visual Regression Testing Is Easier In 2018!
* Walkthrough - Regression Testing in Django (1 hr, 1.75 hr total)
  * From a carefully crafted starter application, we'll walk through the important aspects of our application that must, could and should be tested. We'll also cover tips for scoping out areas that are more likely to have bugs introduced and ways to separate your code appropriately for the best testing approaches.
* Walkthrough - Visual Regression Testing Powered By Javascript (45 mins, 2.5 hrs total)
  * From our same carefully crafter starter app, we'll add visual regression tests using my test runner, test assertion, web driver, and image diff libraries of choice. (Yes, you CAN use Python for this, but there are some awesome JS libraries that make our lives even easier).
* Flex Time (remainder of time left)
  * Additional time for breaking things and putting them back together, questions, helping each other, etc.
* Conclusion
  * Wrap up, call to action, and suggested tools/resources

Audience Expectations:
----------------------
A foundational knowledge of Python and a web framework of choice is beneficial, as we'll dive right into testing an existing application. Starter code and code progressions will be provided, so you don't have to be a Django expert to grasp the content! Whether you love, hate, or have never used Javascript, you'll feel at home; our use of JS will be limited to leveraging libraries to gather data and screenshots for visual regression testing, whether for a JS client or a Django web app.

Notes:
------
As a mentor and lead engineer, I’m constantly asked questions about why testing is important, what you should actually be testing, and what testing looks like in the real world. I’m hoping that this tutorial can shed light on all of those questions to give clarity and confidence to developers when approaching testing. I’m also a huge fan of regression tests and believe that visual regression tests are key to maintaining well-designed and user-friendly sites.

I took care when formulating this proposal to cover all audience levels. I find that it’s best to create a foundation with basic information and terminology to give all audience members a chance to understand a more advanced topic, while making sure the information being covered is integral to the topic at hand. I rely upon finding a happy medium of keeping information simple yet dense to allow for broad topics to be described quickly so we can move quickly from “what is a test?” to implementing visual regression tests.

I have 6+ years of experience testing and building applications not only in the JavaScript/Python worlds but in many other languages and frameworks as well. I believe that my wide range of experience can shed light on this topic and cross-pollinate my approaches to testing.

---

Private Info (revealed after rated):

Bio: (500 character limit):
----------------------------
Emily Morehouse-Valcarcel is the Director of Engineering at Cuttlesoft, a digital product agency focused on creating beautifully designed software. Her passion is driven by a blend of empathy, strategy, curiosity, and human-centered design. She's an avid OSS contributor and constant learner focused on building tools to automate the mundane and shed light on the complexity of the human experience. Emily holds degrees in Computer Science, Criminology, and Theatre from Florida State University.
