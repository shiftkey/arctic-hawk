arctic-hawk
===========

## About

This all started on a plane flight home. Technically, it started after a pairing session recently on some WPF code where I lamented "Oh WPF you crazy bastard, I missed you". Anyway, I was frustrated by some work stuff and started pondering on a simple question:

### How can I demonstrate the disruptions I face when I'm in the office?

I've been getting a lot of visitors to my desk at the moment and would love to easily capture a bunch of data about when I'm productive and when I'm not. There's many [pomodoro](http://www.pomodorotechnique.com/) style apps out there but I was looking for something I could tailor to my use case.

So I started bashing out a simple WPF app to do the job and got midway through before I paused.

### What else have I got on the backburner that I could tie into this app?

There's things that I've been meaning to make time for over the past few months that I feel bad for the people I've promised stuff to. In particular:

 - I owe [@xpaulbettsx](https://twitter.com/xpaulbettsx) some feedback on [Shimmer](https://github.com/github/shimmer) - perhaps I can use it as an installer for this app rather than WiX/ClickOnce/etc.
 - I've got an idea for a Windows 8 app (or perhaps something Mono-related?) along these lines - how should I use the Portable Class Library tools, how can i structure this app for maximum portability, how far can I push this etc etc
 - I've been playing around with [event sourcing](http://martinfowler.com/eaaDev/EventSourcing.html) concepts but would like to see how it fits within the context of this app.
 - I don't have the spare time for Code52 that I'd hoped for, but perhaps I could write up some posts on my learnings from building an app at this time.

So of course this needs a rocking name...

### Arctic Hawk - What Does Building a Cross-Platform App in 2012 look like?

I have *The Distance* by Cake stuck in my head. Don't hate on the 90s, man.

#### Part One - Off and Racing

`Reluctantly crouched at the starting line, engines pumping and thumping in time.`
`the green light flashes, the flags go up. churning and burning, they yearn for the cup.`

This section will entail taking the concept and building the first version of the app (many people refer to this as the [minimum viable product](http://en.wikipedia.org/wiki/Minimum_viable_product). Emphasizing speed and features while keeping the codebase relatively simple at this point, I want to see just how quickly I can build it (with tests, because even I have limits).

Goals:

 - release a version of the app that people can download and play around with
 - app should auto-update so that users don't need to go back to the site

#### Part Two - Coding for Reuse

`They deftly maneuver and muscle for rank, fuel burning fast on an empty tank.`
`Reckless and wild, they pour through the turns. Their prowess is potent and secretly stern.`

So we've gotten something out the door and people have started playing around with it, but I need to change direction and target a different platform. How do I do this? How should I do this? How do I juggle multiple apps using the one codebase?

Goals:
 
 - structure the codebase into a portable core and frontend which is platform-specific
 - sketch out plan for targeting next platform and how it will differ from the current platform

### Part Three - World Domination Awaits

`As they speed through the finish, the flags go down. The fans get up and they get out of town.`
`The arena is empty except for one man, still driving and striving as fast as he can.`

Goals:

 - ship an app for a second platform (Windows 8/iOS/iPad) reusing the same codebase and a more suitable front-end
 - back-port features from new platform to current platform
 - be able to push out a release for both platforms from the same codebase in one step (crazy?)

### Part Four - TBC

`The sun has gone down and the moon has come up, and long ago somebody left with the cup.`
`But he's driving and striving and hugging the turns. And thinking of someone for whom he still burns.`

