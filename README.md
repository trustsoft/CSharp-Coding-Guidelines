# About the Guidelines #

The guidelines provide a practical way of developing .NET applications using C# 3.0 or later depending on versions that applications are using.

# Rationale #

Coding guidelines are sometimes overlooked since they are considered as putting some unwanted burdens on developers. However, it has already been proved to worth doing because not all developers:

* are aware that code is generally read 10 times more than it is changed;
* are aware of the potential pitfalls of certain constructions in C#;
* are introduced into certain conventions when using the .NET Framework such as `IDisposable` or the deferred execution nature of LINQ;
* are aware of the impact of using (or neglecting to use) particular solutions on aspects like security, performance, multi-language support, etc; and
* know that not every developer is as capable of understanding an elegant, but abstract, solution as the original developer.


# Basic Principles #

In general, because this document cannot cover everything for each application's purpose, those two documents provided by Microsoft are the main starting points:

* [C# Coding Conventions (C# Programming Guide)](http://msdn.microsoft.com/en-us/library/ff926074.aspx)
* [Framework Design Guidelines](http://msdn.microsoft.com/en-us/library/ms229042.aspx)

Those principles have already been applied to Visual Studio. So, using the default settings can check most of our coding conventions. [ReSharper](http://www.jetbrains.com/resharper) that we are using checks our code in a more robust way so following its default settings would be more efficient.

In addition to them, this document provides guidelines with the following principles:

* **The Principle of Least Surprise** (or Astonishment) &ndash; you should choose a solution that does include any things people might not understand, or put on the wrong track.
* **Keep It Simple Stupid** (KISS) &ndash; the simplest solution is more than sufficient.
* **You Ain't Gonna Need It** (YAGNI) &ndash; you should create a solution for the current problem rather than the ones you think will happen later on (since when can you predict the future?).
* **Don't Repeat Yourself** (DRY) &ndash; you are encouraged to prevent duplication in your code base without forgetting the [Rule of Three](http://lostechies.com/derickbailey/2012/10/31/abstraction-the-rule-of-three) heuristic.


# How to Apply #

Developers are not forced to comply with this guidelines. However, they are encouraged to apply those guidelines. Each guideline is clearly labeled like:

* ![MUST](imgs/must.png): This guideline must be considered for coding.
* ![SHOULD](imgs/should.png): This guideline is strongly recommended for coding.
* ![MAY](imgs/may.png): This guideline can be applied for coding.

![NOTE](imgs/note.png) The terms &ndash; `must`, `should` and `may` &ndash; are defined in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt)


# Useful Resources #

In addition to the many links provided throughout this document, the following books, articles and sites for everyone interested in software quality are recommended:

* [Code Complete: A Practical Handbook of Software Construction](http://www.amazon.com/Code-Complete-Practical-Handbook-Construction/dp/0735619670) (Steve McConnel)

It deals with all aspects of software development, and even though the book was originally written in 2004, but you'll be surprised when you see how accurate it still is. I wrote a review in 2009 if you want to get a sense of its contents.

* [The Art of Agile Development](http://www.amazon.com/Art-Agile-Development-James-Shore/dp/0596527675) (James Shore)

Another great all-encompassing trip through the many practices preached by processes like Scrum and Extreme Programming. If you're looking for a quick introduction with a pragmatic touch, make sure you read James' book.

* [Applying Domain Driven-Design and Patterns: With Examples in C# and .NET](http://www.amazon.com/Applying-Domain-Driven-Design-Patterns-Examples/dp/0321268202) (Jimmy Nilsson)

The book that started my interest for both Domain Driven Design and Test Driven Development. It's one of those books that I wished I had read a few years earlier. It would have saved me from many mistakes.

* [Jeremy D. Miller's Blog](http://codebetter.com/blogs/jeremy.miller)

Although he is not that active anymore, in the last couple of years he has written some excellent blog posts on Test Driven Development, Design Patterns and design principles. I've learned a lot from his real-life and practical insights.

* [LINQ Framework Design Guidelines](http://blogs.msdn.com/b/mirceat/archive/2008/03/13/linq-framework-design-guidelines.aspx)

A set of rules and recommendations that you should adhere to when creating your own implementations of `IQueryable<T>`.

* [Best Practices for c# `async`/`await`](http://code.jonwagner.com/2012/09/06/best-practices-for-c-asyncawait/)

The rationale and source of several of the new guidelines in this documented, written by [Jon Wagner](https://twitter.com/jonwagnerdotcom).


# Table of Contents #

* [Class Design Guidelines](Class.Design.Guidelines.md)
* [Member Design Guidelines](Member.Design.Guidelines.md)
* [Miscellaneous Design Guidelines](Miscellaneous.Design.Guidelines.md)
* [Maintainability Guidelines](Maintainability.Guidelines.md)
* [Naming Guidelines](Naming.Guidelines.md)
* [Performance Guidelines](Performance.Guidelines.md)
* [Framework Guidelines](Framework.Guidelines.md)
* [Documentation Guidelines](Documentation.Guidelines.md)
* [Layout Guidelines](Layout.Guidelines.md)


# License #

This is released under **New BSD License**.