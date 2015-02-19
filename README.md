[![Stories in Ready](https://badge.waffle.io/emptyslate/slate.png?label=ready&title=Ready)](https://waffle.io/emptyslate/slate)
# slate
a customizable CommonMark editor and previewer, written in ClojureScript
---
slate is an attempt to make a beautiful, elegant, customizable, modular, and free/libre CommonMark editor and previewer. It's also probably a generic text editor, but that's not end goal.

#### Beautiful
slate and slate based projects must be a joy for the end user to use. The editor must be fast, low latency, and responsive (not in the browser window sense, necessarily). Too many web editors are hard to use on less powerful devices. Ideally, slate based projects should work on a Raspberry Pi, although that is currently impossible due to hardware constraints. So slate based projects should run on a 2012 Samsung Chromebook and be just as snappy as on the Darth Vader Apple Can Desktop.

#### Elegant
slate must be a joy to code for. It should exemplify current and evolving ClojureScript and JavaScript best practices. It should facilitate thinking at higher levels of abstraction than are fashionable in programming today. And it should do so transparently, guiding developers to programming Nirvana. Every tool and resource that has been factored into slate's design has been chosen for its ability to facilitate this goal. Someday, slate may be *the* project that sucks new users into the clojure fold. No promises, only ambitions.

#### Customizable
slate must solve **our** problems, not just my problem. There are a few ways to do this, but by far the most sustainable way is to build slate to do one thing really well, and allow other code to hook into the machinations that make that possible. We don't yet know what those abstractions are, but they should fully encapsulate the complexity of a text editor such that they don't leak and force you to waste time hacking a workaround.

The best way to do this is by starting, from day one, with thinking about the design goals and create example projects which require these interfaces to operate. slate was actually created in order to rebuild Hackster.io's editor, but it became obvious that this tool needs to be open source and highly available or else it will suffer too many bugs to be useful.

#### Modular
slate is the culmination of lessons learned in both functional and object oriented programming. It harkens back to the smalltalk style of OOP: objects should be huge and few. The goal is to grow these objects from tiny thought seeds, and have them internally work in as functional a way as possible.

This style of programming leads quite naturally to modular, easily refactorable designs. Every object does one thing. Data pipelines from one object to the next. Objects can be swapped out and replaced, as long as they fulfill the same contracts. The dependency graph becomes a circularly linked list, or a directed acyclic graph (ok, it has one cycle).

Both FP and OOP are incredibly valuable tools in our toolchest. Scala experiments have proven that they can work together, abstraction on top of abstraction, to fight valiantly against the horrors and pains of complexity. But it takes rigor and meta-abstractions and the knowledge that it's OK to do dirty hacks, as long as the end mission is fulfilled.

For more information on what modules are currently in development, please check out the wiki. (Todo mrnice me@niceguys.co: Flesh out wiki)

#### Free and Libre
Valuable products should be paid for. You can pay for slate with your time and energy if you don't want to share your money. But, because this is entirely unenforceable, we're happy if you can use slate to get things done faster, sleep more and live your life better. So please: extend, fork, crucify, alter, fold, mutilate, spindle slate. And if you can, share your lessons back :)

## contribution guide

### Getting in touch with the community
slate is a community driven product. It will die and be useless unless it is able to attract fantastic developers who want to work on an interesting and (more importantly) useful project. Because of this, we are attempting to make working on slate the most pleasant and pleasurable coding experience possible. In order to do this, we have invested heavily in robust code tooling and community organization tools.

#### Communication and Organization
* Discourse website
* Waffle.io
* Github wiki
* Email `me@niceguys.co` for a slack invite
* Someone please set up a slack auto inviter please please please
* Freenode type mirror of slack so that everybody can get involved

#### Community tooling and continuous integration
* Travis
* Selenium performance regression testing (Gotta keep it beautiful for our users)

### Writing Code
* style guide
* general workflow
* differences between core projects and extensions

#### Code Tooling
* Vagrant + Docker based development environment (Todo: Rapid start instructions to reduce friction)
* Leiningen project management
* Lein-npm for awesome npm modules
* lein-figwheel for hot reloading for development and debugging
* Running tests
* Profiling and debugging

#### Code sharing
* Making everything npm installable: http://www.matthewstump.com/misc/2012/06/04/writing-nodejs-modules-in-clojurescript/

#### I know JavaScript, what can I do?
* Why clojurescript (Expressive, functional + oop, great community, good tooling)
* Up and running with clojurescript resources
* Pros and cons of fragmentation of codebase
* Core projects should stay clojurescript, extensions should be in any compile2js language

#### I'm a designer or devsigner, what can I do?
*Oh you wonderfully beautiful flower*, reading all the way through this long and boring document to arrive here. If you truly want to help slate become a beautiful project, there is a lot that you can do to help.

* Create use cases and mockups for slate consumers. We don't yet know all of the ways people will want to use slate and integrate slate into their projects. If you're feeling wonderfully artistic or want to take a crack of highly specific User Interaction and User Experience design, we would love to see your prototypes and designs and your concerns, so that we can, together, find better code abstractions to support your art and artistry. Although the market might not understand it yet, you are truly what makes or breaks a product.
* Help create instructional material. slate is necessarily complicated. Your ability to convey and share knowledge in am empathetic fashion is a great strength. slate will be as simple as possible, but no simpler. You, as a designer, have the ability to explain visually, with space and with color and with symbolism, complicated concepts and make them familiar, warm, and approachable. Please email me@niceguys.co if you want to help make beautiful instructions.
* Support the website and community. I (mrnice) cannot handle creating pixel perfect designs, so I take free ones which are available and bend them to my will. This, sadly, makes the posterboard funnel for the project boring and unappealing, and seem unmaintained or cared for. I beg that you help slate overcome my personal shortcomings.
* Learn clojure. It's a gorgeous attempt at minimalistic programming. Even if you've given up before, you can definitely do it if you start with JavaScript and slowly move to ClojureScript. slate wants to be as welcoming as possible to all skill levels. And from a professional point of view, being able to both design beautiful interfaces *and implement them* will make you a white-hot item that companies will fight over. I believe in your ability to transform and rework your own mind. I believe in you.
