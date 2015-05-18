Salesforce APIs
===============

Tech writers = members of scrum teams
A good tester is a strong customer advocate, and a good tech writer is a strong customer advocate
We're an advocate for our customers when our customers aren't around

Initial job: question requirements

gold nuggets: things to look out for (these are the things that are hard to find and take a lot of collaboration)

API Design Review Board
-----------------------
In order to be exposed in API, a feature had to be approved by review board
Now cornerstone of API - where docs start

3 stages:
1. Doc template (dev fills out - explains resources, how they work, how people use them)
2. Posts to chatter group
3. Review (1x week) - 30 min for each feature, approve or rework

What's great about the design review board: 
- gives writer and tester chance to give input early on in design cycle (error codes). 
- Makes tech writer's job easier; full seat at the table with devs & product owners to make API as easy as possible to learn.
- Testers and devs more living in code base; we advocate for external names and docs.

API Quality
-----------
Universal Definition File - complete picture of API.
Trust means existing clients aren't going to break with new resources
If a client is in version N, version N is frozen - needed to enforce in testing

Simulating the real works
-------------------------
Tech reviews! Just a starting place, lucky if you catch some mistakes, maybe a best practice.
see who's interested in docs and thinking like a customer
Code Samples - How do we get to them? collaborating with as many people as possible 
Instead of saying 'what's the use case' saying 'why would a customer use this'? and zooming out until you have a persona in mind

Dogfooding: eating your own dogfood, using your own product before it gets released
Blitzing: coordinated activity on a certain part of the code 

Working in the Real World
-------------------------
- direct exposure to customers of at least 2 hours every six weeks made a difference in UX
- See what has been answered - can it be linked to doc? 
- If content isn't there, file a doc bug

Let's Tell a Story: Scenario-based documentation
================================================
Every topic has feedback forum
Customers communicate via IRC, twitter, support/sales/customer service divisions
Feedback is mostly for doc improvement
Most people want to have simple documentation for complex tasks
A chasm that must be bridged! Intermediate to Expert.. connect the dots

Getting started in an enterprise software: What's in there? What should I pack? How do I get there? Are there monsters?

Tutorial: good for a start, doesn't do much more than getting them familiar with the basics
Or: conceptual overview (historical context, diagrams of big picture view, important locations, links to more detailed info) ...
Procedural docs: how to ... how to ... etc w decent TOC, people can piece together tasks they need to carry out on whatever task they need

All these are too detailed or too broad or not relevant

Senario or use-base case will come in handy!
Instructional story: Similar to tutorial but goes further - useful prerequs, assumes some basic knowledge, useful tips and tricks to avoid distress. takes into account threatening variables

table top role playing games!
D&D Manuals = scenario-based docs
- users embark on an epic journey
- accomplsh anazing feates

D&D lives and dies by how playable it is. 

Railroading: If you provide them w enough choices or heremy the appearance of enough choices, they don't even realize it's happening
The trick is coming up with stories that are worth coming up with a railroad for
Document well defined use cases to help them down the road
then take them there on an express train to awesometown!
inlike D&D, customers don't like surprises

Scenario based doc is for people who finished tutorial. tutorial got them to hello world state with product
come up with scenario based documentation to get them to where they really want to go

What do you need to do?
What is the end goal?
  You want to create a dashboard that displays... blah blah blah
Break down project into easily digestible features 
Obvious railroad but positive this is good for users

Scenario-baased Docs: Best Practices
------------------------------------------
- Know your customers! If you don't know, talk to support, sales, edu services
- Develop customer profies
- Don't write a tutorial (not to get started, about solving big problems)
- Don't write a Marketing case study (prove your product can do what marketing says it does)
- Simple procedure for a complex process (chunking)
- Don't waste time explaining what goes on under the hood unless you need to
- Use video strategically and as a supplement; keep it short! Customers should NOT need to watch video to know how to do a thing
- have fun with it

How to write documentation for users that don't read
====================================================
Why people don't read your documentation
-----------------------------------------
bc:
-no one reads aything on the internet
- Users scan in F-shaped pattern (lots of text is just ignored)
- meaningful text and images
- links, bullets
- shapes more important than text

transgresssion: fixed with text
solution: use markdown, bold, headers

People tend to skip over things that look like ads
transgression: many fixations per line
text is 65-90 characters wide = lots of fixations on left side

transgression: search failure
link to next page is same size as small stuff - make content all in one page, indexable

observance: breaking up content
short, big headings, buttom is expandable content (hidden by default), ordered (step 1 headings)

Users are awful at searching!
-----------------------------
Users try 1 query and give up
Stackoverflow used to close duplicate questions - theres a benefit to having multiple subtle variants of a question as people tend to ask and search using completely different word, and the better our coverage, the better odds people can find the answer they're looking for

Helper Libraries, Client SDKs, API SDKs, library bindings, language-specific wrappers
Look through support queries, look through google analytics on what terms they're using
solution: add verbs

No one reads anything above/below code snippets
everyone just does copy/paste

Sometimes copy and paste can go a little too far ($ gem install rails) - people pasted in $
separating out input vs. output - but this is tricky

Every user failure is a potential job to be done

Docs behind a wall! NOOOOOOOOOO
Downoad pdfs to get access to docs = 50% of your traffic you're just throwing away
if you're big enough, wikihow will steal your traffic!

Validation as documentation
bad: confusing error messages
good: did you mean? etc
You can fix these confusing error messages!
Strings are easy to find/change - good way to get started with code base

make documentation readable
----------------------------
- break up text often
- first 3-5 wwords of every paragraph are most important
- 6590 good
- meta description should match content
- URL should describe content
- every page = landing page
- your documentation should always win
- etc etc - read the Google Guide
- Why your awesome docs aren't solving user problems
--------------------------------------------------

- look at your product from a user/task perspective
- users shold hire things you contrl for most faulures
- make error messages explain how to fix the problem
- better yet, solve the problem for the user

A Developers Approach to Documentation: From Passive to Dynamic
===============================================================
English is ambiguous (API = simple vs. consumer language = complex)
Pollyanna principle: machines should work. People should think.

Four types of documentation: separation of duties
-------------------------------------------------
- Reference (low level, dictionary-esque)
- Examples (tutorials, walk you through use case)
- Guides (topical, higher level 'why you want to use this', point is to get people to buy into mindset)
- Support (important, some stuff is inconsistent. Best online documentation has a huge support component)

Mental model for division of labor:
-----------------------------------
- Generated: reference, examples (in different languages)
- Humans: examples (for humans to curate), guides 
-   A snippet of code without context is just a snippet of code
- Community: guides, support

Problem with Documentation
--------------------------
O'Reilly-ification of documentation: problem is that everyone (novices to devs) get the same guide
Has to cover all use cases and skill levels
once you know stuff about the user, you can start tailoring documentation to them

MVC: minimum viable call
------------------------
Get people doing an action as quickly as humanly possible
Ex: onboarding flow (know language, etc), installation, MVC (first call to get them to do something)
After MVC: congrats, everything is set up. Next, let's... blah blah blah

Things taht don't seem like doc but are
----------------------------------------
touches all parts of an API
- Interactive playgrounds
- Error Messages (ex: angular JS error takes you to the module error online and tells you what's up)
- API SDKs
- Support section (his company vs. stack overflow). Biggest threat to documentation is support. Not someething to fight but something to bring in. 


