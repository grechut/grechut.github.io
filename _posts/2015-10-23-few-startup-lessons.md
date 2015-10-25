---
layout: post
title:  "Few startup lessons"
date:   2015-10-24 23:16:29
categories: general
---
I have been into the startup world for the recent 2 years. Definitely, it was the most interesting and challenging part of my software engineering career. During this period I have learned a few great lessons that I would like to share (some of them are already well known). These are my personal observations so they might not apply to your case.

**Recruit proper people.** In most cases, you need to hire few people that will be working with you. Picking up the right people is extremely important. Few wonderful tips presented in the [Aaron Schwartz's article](http://www.aaronsw.com/weblog/hiring). Generally you want to hire people that are smart, get things done and you would like to work with them. You should not hire a person that does not meet all the criterias. People that are not able to deliver won’t create any value. Unfriendly people won't create a great startup atmosphere. But if you happen to fail in this area...

**Don't be afraid of stopping working with bad hires.** Hiring a bad person happens. There are various factors that cause this mistake. Often as the project goes on you might realize that somebody's skillset does not match your needs. Or that somebody does not fit into your startup culture. Probably both sides will be happier if they go their own path.

**Hire a good designer.** One that can write quality CSS. You don't want to be stuck in the trap of having designer that will give you a ton of PSD designs (no PSD movement). You want to have a guy that can quickly materialize the design ideas. This will make your development move much faster. Quality design is essential. Not only being beautiful matters. It increases the credibility of your product (people tend to trust more in the things that look good).

**Time box your meetings.** When the meeting is time boxed, attending people tend to have better focus. Of course, you need to time box to the sensible amount of time. Too short limits will stress people too much. Too long will not bring any effect because even with many distractions and being verbose, the team will manage to finish on time. When bigger or unexpected topics are raised, arrange a separate discussion for them. Also remember about preparing well for every meeting.

**Pick up a good github workflow.** The one that will support code reviews, being able to deploy any time and being able to QA properly before releasing new version. [This one](http://nvie.com/posts/a-successful-git-branching-model/) from Vincent Driessen is perfect.

**Have regular retrospective meetings.** Your team and developent process need to continuously improve. Especially in the early phase of the development, there will be few bottlenecks that might hurt your velocity. Discuss those obstacles regularly but not too frequently. Every 2-4 weeks is fine. At the end of such meeting, pick 3-4 most relevant ones and really commit to overcoming them.

**Understand the problem before jumping directly to possible solutions.** Frequently people start brainstorming through technical challenges even though they are not needed. Deeply understand what the user needs and how you can simplify it before starting coding. Ask other people directly to demonstrate their understanding of the problem. It helps in sharing the understanding of the problem and clarifying things. Don’t forget to understand how the problem fits into the big picture of your startup.

**Cut the amount of work and prioritize properly.** Use the [Pareto principle](https://en.wikipedia.org/wiki/Pareto_principle) every day. Most of the features that you can think of seem to be urgent. Most of they really aren't. Value your time high and keep in mind that polishing one feature for too long would mean not doing other features. It's better to work on 2-3 essential things and do them properly instead of struggling with ten of them.

**Use [Slack](https://slack.com/) for the team short term communication.** Create channels per specific features / areas of the project. In these channels only relevant people should be involved. Also, the discussion will not be mixed with other topics.

**Be patient.** Especially at the beginning of the project. It takes some time until the team gets the whole process right. With the core software infrastructure ready and knowing how to work with other team members, the development will increase velocity. Fail frequently, learn from failures, apply fixes and iterate again.

**Have an experimental area** if your project is heavily based on research or has many unclear requirements. This idea was borrowed from [a great article](http://agilefocus.com/2009/06/22/the-3-kinds-of-code/) written by William Pietri. Separate place for the experimental code will help you in distinguishing between the production ready code and the experimental stuff. It will allow you to keep both high code quality and being able to move on rapidly with research / experiments. In the experimental part, you can have lower quality standards. Spending time on writing the experiments fully properly and then throwing them away would be a waste of time.

**Refactor continuously.** Your codebase is evolving all the time. Gradually you are learning which parts worked well and which didn't. Also, if you move fast, then you are likely to create a lot of technical debt. It's not bad to have it. If you want to keep high speed of development, you need to regularly refactor your code so that you can easily extend / add new features. That's one of agile core principles.

**Master debugging tools.** In the ideal scenario you will not have any bugs. But this ideal scenario does not exist. Always some smaller or bigger bugs are likely to occur in your product. What you need is being productive when it comes to debugging. In the modern world there are plenty of tricks and extensions to your development environment that can make the debugging easy. Learn about them properly. Also, you should have a helpful way of logging in your production version so that within a few seconds you can understand what went wrong. One of good logging services that I was happy with was [Rollbar](https://rollbar.com/).

**"Adapt what is useful, discard what is not."** You need to make your process support your needs. Often people might criticize you that 'you are not fully using agile methodologies'.
Do not take agile as a dogma. Firstly, try to understand your needs. If your team is productive without detailed estimations, then you can proceed without them. Recently [GROWS](http://growsmethod.com/) method is describing a very similar attitude.

**Try 'JSON driven development'.** That's the name that we use at Portent.io for the way of starting the feature by sketching the sample API response (in our case JSON format). With such JSON, backend developers clearly know how the backend output should look like. On the other hand, frontend can immediately start work using mocked response with faked data from that JSON. Generally, this idea can be applied to any case where many developers work together within explicit boundaries. Most popular example of such boundaries is backend - frontend. Starting with designing the integration point allows both sides to proceed without blocking the other part. Once you know what you should produce / expect, you can quickly jump into work. Otherwise you can spend lot of time, waiting for the other side’s decision about how you’re going to integrate your parts.

**Use profilers.** Memory leaks or performance bottlenecks are usually not harmful. Until you receive a big traffic on your production version and things crash. Understand deeply how your code is working. Profilers can be an invaluable help here.

**Use databases properly.** Use indexes, reduce access to the database and cache when possible. It's often convenient to just fetch data. Often we do this without understanding how many database calls we are making in total and what it takes database to process each of them. Most of the databases are good enough if we use them properly. Analyze how many calls you are making and how they are executed. Discover bottlenecks and fix them.

**Have fun, smile and be kind.** We are all humans. Having fun almost always makes the work nicer. Appreciate other people. Everybody is unique. Smile is for free.
