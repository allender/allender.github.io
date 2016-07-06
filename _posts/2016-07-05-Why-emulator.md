---
title: "Why an Apple ][ Emulator"
excerpt: ""
date: 2016-07-06
---

I wanted to write an Apple ][ emulator as a side project to provide me a
project that I could work on outside of work hours.  Oftentimes I have
found that while I love game programming, there are a lot of things that I
__want__ to do, but don't have time to do.  Working on the emulator provides
me a way to do something fun and fairly educational at the same time.  I
have plans to work on other emulators in the future, mainly because they
are (in my opinion) pretty neat projects.

I had the follwoing goals for this project:

* Use C++11.  Love it or hate it, I use C++ every day and wanted to 
stay in this language.  I don't see game programming moving away from
this language anytime soon.
* Cross platform.  Several of the emulators that I have seen have been
mac only, or windows only.  I wanted to provide something that would
be useable on Windows, Mac, and Linux.
* Create easy to understand code.  Programmers have a tendency to get
fancy when there is no need to do so.  In reviewing other emulator projects,
many look fairly obfuscted in critical sections with not a lot of internal
documentation on how things actually work.  Code is self documenting, but 
that is not a good teaching tool.

In order to provide cross platform rendering, I settled on SDL as the
main mechanism with which to provide this functionality.  For reasons that
I will expand on in another post, this decision ultimatly means SDL + openGL
but it has worked out well, as I have gotten the benefit of event handling
(and soon audio) that SDL provides.

My intent here is to provide updates on the project and expand on how/why I
made certain programming decsisions. By no means is my code the most elegant.
My goal (as stated above) is to be readable.  Gone are the days of having
to make an Apple ][ emulator as fast as possible through arcane code
optimizations.  Modern hardware and compilers will ensure that this current
emulator won't need a ton of those tricks.

