---
layout: blog_post
title: How to rescue failing programs
permalink: /thoughts/blog/how-to-rescue-failing-programs/
redirect_from:
  - /blog/how-to-rescue-failing-programs/
content_type: BlogPosting
image: /img/blog/rescue_failing_programs/rescue.svg
image_description: A firefighter standing on a large computer that's caught on fire and is using a firehouse to try to put it out.
image_display: true
order: 1000
tags: [delivery management, procurement, robert read]
excerpt: To rescue a failing program, you must protect the four freedoms of enterprise system development.
authors:
  - Robert Read
date_published: 2017-09-23
date: 2017-09-23
---
"Never give up." "Don't switch horses in midstream." "Quitters never win, and winners never quit." "When you're going through hell, keep going." We can all think of additional aphorisms that argue against changing course when a program is failing.

Here are some others: "When you're in a hole, quit digging." "Don't throw good money after bad." "Don't beat a dead horse." These sayings also capture essential truths and argue that you should make radical changes when a program is in trouble. The government IT leader faced with a failing project needs courage, calm rationality, and a set a best practices. This article can only provide the last.

A large, failing project clouds our thinking for several reasons:

- Nobody wants to cost the taxpayer money, and nobody wants to be blamed for costing the taxpayer money.
- Large projects tend to have many components, each of which requires a certain amount of effort to understand.
- A history grows up around all projects, and the story, which may be complex, can become more vivid than the state of the system, which should be simple. People start to let all that has happened obscure the fact that the software is just software.
- People in long-term relationships develop an inertia that makes them not want to accept the uncertainty of changing those relationships.

The fundamental principle that the IT leader must employ is: **always be attempting to increase your options rather than decrease your options**. The same lesson may be learned from the game of chess. In chess, how you got to a board position is irrelevant; it's a sunk cost. You only have to make the best move based on the position of the pieces as they stand when it's your turn. When beginners play chess, the outcome is determined by blunders. When you're good enough at chess and you're losing, it feels like being slowly buried alive. You lose freedom of movement. You lose control of squares on the board. One by one your options are snuffed out by an inexorable stoppage of our stratagems. Eventually you have no move left to you at all: that's called a checkmate.

Running a large IT project can feel like playing multi-dimensional chess while blindfolded &mdash; but it should not. The taxpayers will benefit the most if you protect four freedoms of enterprise system development:

1. **Freedom of What:** Do you have the freedom to choose what module you'll in invest in? Is your system a monolithic monster that must be treated as a whole, or is it modular, affording you the ability to prioritize which modules will be invested in at present? Have you accepted, perhaps with your own complicity, the idea that your project is a PERT chart of dependencies that force you to work on modules in a certain order?
2. **Freedom of When:** Has your project fallen into the trap of having a single "done" date? Or do you have the ability to make many releases, each of which enhances functionality, perhaps based on learning from previous releases? Do you have the freedom to watch the system grow and make adjustments in releases based on what you learn?
3. **Freedom of How:** Do you have the freedom to decide how a module will be implemented? Can you take advantage of improving technology? For example, can you easily take advantage of a responsive frontend library to make your project mobile-friendly? Can you choose to use either a SQL database or a NoSQL storage solution without undue expense? If an open-source technology makes a proprietary solution obsolete, can you take advantage of it and add the savings to your budget?
4. **Freedom of Who:** Can you choose whom will work on your system? Are you forced to have only one firm work on it, or can you have multiple firms work on multiple modules, or even the same module? If you have to have only one vendor, how high is the energy barrier and cost of changing that vendor?

In a perfect world, you'd design your project (through its growth and its planned final solution) to maximize each of these freedoms.

Modern agile software methodologies and related technologies can assist you with these freedoms, but there's one additional thing you'll probably need, unless you can do it yourself. You don't have to have a staff full of technology superstars, but you must have one trusted person on your staff that can fully understand the technical aspects of your program, while you manage the less-technical aspects of it. If you don't have an architect, or someone who can a comprehend the whole system, you'll be at the mercy of people pushing self-interested agendas rather than the truth. It must be your highest priority to obtain at least one such person and empower them to fully understand your system, even if they aren't designing it. This may require you to rearrange duties so that an appropriate person can play that role for you. If your system can't be understood by one person, you're doing something wrong. We don't mean that every line of code must be understood by this person. Here is a touchstone test: do you have one person who can draw a diagram (it may be a big diagram) of every component of your system and explain it to an outside technical expert in less than an hour?

For example, with the help of a sufficient staff and direct access to end-users, agile story-based development can give you the **Freedom of What** you invest in, guided by designers who are informed by direct user interaction. Modern JSON-based APIs are a valuable part of this strategy by enforcing modularity and testability. Test-driven development, or at least designing for testability, further free you to work whatever modules you deem most important by decreasing the risk of making changes to a module.

Continuous integration, and other software engineering techniques (further beyond the scope of this article) also increase your freedom to invest as you see fit.

The **Freedom of When** is summed up in an agile motto: Always be Releasable. From the first sprint, a project should be releasable. Note this doesn't mean "released." For sound social reasons, you may not want to release every sprint. However, it should be noted that the most admired companies on Earth do, in fact, release on a daily basis. Nonetheless the important thing isn't that it's "released" but that it's releasable.

Why does this matter if it isn't actually given to users? For two reasons. The first is an aphorism every high school athlete has heard their coach say: "you play like you practice." If you don't intensely and thoroughly practice the complete story, start to finish, you'll undoubtedly miss something important. The second reason is also embedded in the spirit of agile, but has been articulated by Eric Ries in his book <a href="http://theleanstartup.com/">*Lean Startup*</a>: to reduce risk maximally, you must learn as much as you can as early as you can, and the best way to do that is to get real software in front of real users, even if the users are carefully selected and the software is extremely limited compared to the planned final scope. The possibility of discovering something &mdash; which may in fact be something wonderful that no one had thought of &mdash; is an opportunity cost that no project can afford to throw away.

The beauty of this approach is that you fail fast &mdash; or rather, fail constantly, in small ways from which you may learn. Conjure in your mind the spectre of the last project of $300M or more that you heard of that was simply never turned on. Holding that image in your mind, ask yourself how much trouble it's worth to always be releasable, having a fully tested project that can be evaluated during the entire course of the project to avoid a catastrophic failure.

The **Freedom of How** hearkens back to Computer Science 101: if a module is truly independent, then you're truly free to change its implementation without disrupting the system. This is drilled into us as students. But the modern age of GitHub-based open source has made this even more <a href="https://18f.gsa.gov/2014/11/26/how-to-use-more-open-source/">important</a>. It's perhaps more apparent to professional programmers who code everyday than to executives, but the world of programming has changed. Programming is now largely about how to choose and stitch together open-source software to avoid work as much as possible. This is what Larry Wall called Laziness &mdash; a fundamental virtue of a programmer, and now a fundamental means of decreasing risk on a project and saving money for the taxpayer.

In order to take advantage of this wealth of work already done for you, your team must be partially aware of the world of free software. But additionally, you must have a well organized, modular project that allows you to test replacing major functionality with commercial off-the-shelf software (COTS) in a reliable fashion.

As in fictional multi-dimensional chess, there are indeed many dimensions of choice, or lack of choice. Ask yourselves these questions:

1. Do you have the freedom to deploy the project gradually, one component at a time, or have you been forced (perhaps with your own complicity) into accepting the idea that the project is an "all or nothing" launch? For example, in replacing a legacy system, do you have the freedom given you by the "<a href="https://www.martinfowler.com/bliki/StranglerApplication.html">strangler pattern</a>?"
2. Do you have the freedom to treat each major component independently? That is, if Congress suddenly mandated you spend three times as much as you have currently budgeted on one component and one-third as much as you budgeted on a different component, could you do that and still release a functional system?
3. Are you enslaved by a PERT or Gantt chart? That is, have you been told you have to get pieces done in a certain order, such that one schedule slip cascades into a schedule slip for the entire project? Or, are you using modern agile practices and can release a project, even if incomplete, at any time?
4. Do you have the freedom to distribute work on multiple modules to multiple vendors, or are you completely locked into a single vendor?
5. If you must have only one vendor, do you have the freedom to change that vendor?

Perhaps the most pernicious and common freedom for the government IT executive to lack is the **Freedom of Who**. Commonly, large projects are locked into a single vendor. Vendors may intentionally try to increase vendor lock-in. The IT leader must always be on guard against this. Here are several ways to prevent vendor lock-in:

1. Insist on clean, simple API-separating modules.
2. Make sure a technical architect works for you and can diagram the whole system and can explain each part.
3. The ability for anyone to deploy and host the system must be treated as an essential part of the deliverable. It isn't enough to have code that anyone could use, if the means of deploying it are kept secret or poorly documented.
4. Insist on architectural review and at least some code review by a party loyal to you, or by a third party if you don't have the staff for that.

Ideally, a plan to limit vendor lock-in should be a part of every project, and vendor's compensation should be tied to it. If you have inherited a project, you may not be able to adjust the compensation structure to achieve this, but if you're re-baselining or starting a new project you should prioritize rewarding vendors for doing a good job allowing other vendors to work with their code.

Sadly, both human nature and the financial interest of existing vendors on a project press them not to dispel or even to increase this confusion. Here are some statements that you often hear vendors on a large, failing system make, and our suggested responses.

1. "The problem is you've changed the requirements." Response: "Modern software practice is about being agile in order to respond to change. The motto of agility is 'embrace change'. Start embracing!"
2. "This system is so complex, it'll take someone else years to understand it." Response: "It's the job of the computer programmer to create order out of chaos. Using APIs, unit tests, and clean interfaces, your efforts should be making the system simpler, not more complex."
3. "The code is a legacy of poorly-designed and complex code of great size. It'll be difficult for another vendor to work on it." Response: "It is your job to make the code simple, clean, and reasonably short. Possibly you have done your job poorly."
4. "It'll take other programmers a long time to understand this code." Response: "Code isn't magic unless it has been intentionally obfuscated. We expect professional programmers to be able to deal with a legacy codebase, and employ modern software engineering practices to help them do so."
5. "We have a long-term relationship, and now that we have gotten past our most recent problems, we're sure progress will speed up." Response: "We live in an unpredictable world, but the best predictor of progress next year is progress last year."
6. "We know we're behind schedule showing you what we promised, but if you give us some more time we'll give you a system even better than what you asked for." Response: "No." The heart of agile practice is to always be releasable, even if you have to compromise functionality temporarily to obtain this. If you're asked to give up getting your software tested by end-users as soon as possible, you must simply flatly refuse.

There are perhaps two major myths that make it harder to free yourself from the clutches of a vendor who's locked you in. The first is that code is somehow mystical, that it can't be understood except by the people who create it, and that there's a major expense to having an uninvolved person start working on the code. Like all good myths, this is based on truth, but distorted out of all proportion.

Good programmers write clear code that other programmers can understand. If the code is hard to understand, that reflects very poorly on the people who wrote it. After a time, say a year, a team of bad programmers loses the ability to understand the bad code that they wrote, even though they wrote it. So the unfair advantage they have compared to others turns out to not be so great as one imagines.

The second myth is that programmers are fungible; that somehow a project just takes X lines of code, like X tons of asphalt that have to be laid, and that it doesn't matter who does it. In fact, all experience shows that individual programmers differ by a factor of about ten in terms of how productive they are. In fact, although we have no studies that prove it, we believe good programmers can often accomplish the same functionality with one-tenth the code of mediocre programmers. We have argued [elsewhere](/blog/software-badness-quantified/) that lower number of lines of code in a system is a critical measure of system quality. It'll often be much more cost effective to pay more for a better team. A team that claims to be better should be able to demonstrate this quickly and effectively &mdash; let's say in a week or two. The use of an expensive team may expose an IT executive the risk of being accused of waste. To offset the risk, the executive should demand results from an expensive team be delivered much more quickly than the industry/government expectations. This delivery should justify the executive's decision.

By definition, if you have to rescue a failing project some sort of drastic action is called for. If a team with a current rate of $X has failed miserably, you should perhaps not seek a team of less than $X to replace them, or even one 10% more expensive. It may be appropriate to seek a team that's 50% more expensive. It is tempting to say "you get what you pay for." However, for social reasons we never pay good programmers 10 times as much as bad programmers, even if they're worth it &mdash; so you may get much more than what you pay for, if you can really find programmers who are 10 times better. Decreasing systemic risk to a project, which is somewhat difficult to place in a financial model, is worth almost any price when viewed in the context of the large number or completely failed large government IT systems. It is usually unrealistic and unnecessary to field a team staffed completely by all-stars, but the relative success demonstrated by 18F and the U.S. Digital Service by staffing a much higher percentage of experts than is typical for government is evidence that you should invest in the best team you can find.

Finally, the executive should not think in terms of "switching" vendors, in an all-or-nothing sense. The goal isn't to escape one prison to be incarcerated in another, but to gain the freedom to choose and evaluate vendors. It is typical of an abusive relationship that abuser seeks to curtail the knowledge and ability of the abused to choose other options. The IT executive should not seek to limit their **Freedom of Who**. In moving away from an abusive vendor to whom they're locked-in that has demonstrated cost overruns and incompetence, they should only move toward vendors who increase their freedoms, including the **Freedom of Who**. Human nature being what it is, the longer you stay in an abusive relationship the harder it can be to leave. Do not miss an opportunity to invest in freedom.
