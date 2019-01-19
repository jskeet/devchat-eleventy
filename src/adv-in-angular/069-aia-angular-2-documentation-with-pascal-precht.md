---
layout: layouts/post.njk
title: >
      069 AiA Angular 2 Documentation with Pascal Precht
date: 2015-11-25 16:00:00
episode_number: 069
duration: 0:41:14
audio_url: https://media.devchat.tv/adventures-in-angular/AiA069Angular2Documentation.mp3
podcast: adv-in-angular
tags: 
  - adv_in_angular
  - podcast
---

Go check out [JS Remote Conf](https://jsremoteconf.com/)!

&nbsp;

02:14 - Pascal Precht Introduction

- [Twitter](https://twitter.com/PascalPrecht) 
- [GitHub](https://github.com/PascalPrecht) 
- [Blog](http://pascalprecht.github.io/)

03:03 - Getting Involved with the Angular 2 Documentation

- [thoughtram Blog](http://blog.thoughtram.io)

05:10 - Deciding Where to Contribute

06:16 - Contributors and Contributions

- Dependency Injection (DI)

15:41 - APIs

18:02 - Reactions to Trainings

20:15 - [ngUpgrade](https://github.com/angular/ngUpgrade)

- [@teropa](https://twitter.com/teropa) (Tero Parviainen)

25:34 - View Caching

26:53 - “Chapters” (Documentation Format)

- [angular.io/docs/](https://angular.io/docs/) 
- [Developer Guides](https://angular.io/docs/ts/latest/guide/)

29:26 - Giving the Broad Overview of Angular 2

32:02 - Approaching Documentation

34:18 - Contributing to the Documentation Project

- [wardb@ideablade.com](mailto:wardb@ideablade.com)
Picks

[Heart of a Dog](http://www.imdb.com/title/tt4935446/) (Ward)[Chrome Dev Summit codelabs](https://www.code-labs.io/chrome-dev-summit) (Aaron)[Toastmasters](https://www.toastmasters.org/) (Chuck)[Nexus 5X](https://store.google.com/product/nexus_5x?utm_source=en-ha-na-sem&utm_medium=text&utm_content=bkws&utm_campaign=nexus5x&gclid=Cj0KEQiAg7ayBRD8qqSGt-fj6uYBEiQAucjOwctZDpb9TTB_IExJeZLdS03BejwkI-beicFiOmZi6_EaAugW8P8HAQ) (Pascal)[@robwormald](https://twitter.com/robwormald) (Pascal)[thoughtram Blog](http://blog.thoughtram.io) (Ward)



### Transcript

**_[This episode is sponsored by Hired.com. Every week on Hired, they run an auction where over a thousand tech companies in San Francisco and New York and LA get on JavaScript developers providing to put the salary and equity upfront. The average JavaScript developer gets an average of 5-15 introductory offers and an average salary of over $130,000 a year. You just can either accept an offer and go right into interviewing with the company and neither with that any continuing obligations. It's totally free for users, and when you're hired, they'll also give you a $2,000 signing bonus as a "Thank You" for using them. But if you use the Adventures in Angular link, you'll get a $4,000 bonus instead. Finally, if you're not looking for a job but know someone who is, you can refer them to Hired to get a $1,337 bonus if they accept the job. Go sign up at Hired.com/AdventuresinAngular.]_****_[Ready to master AngularJS? Oasis Digital offers Angular Boot Camp, a three-day, in-person workshop class for individuals or teams. Bring us to your site or send developers to ours classes in St. Louis or San Francisco – AngularBootCamp.com.]_****_[This episode is sponsored by Digital Ocean. Digital Ocean is the provider I use to host all of my creations. All the shows are hosted there, along with any other projects I come up with. Their user interface is simple and easy to use. Their support is excellent. And their VPSes are backed on solid-state drives and are fast and responsive. Check them out at DigitalOcean.com. If you use the code “Angularadventures” you'll get a $10 credit!]_****_[This episode is sponsored by Telerik, the makers of Kendo UI. Kendo UI integrates seamlessly with both AngularJS 1.x and 2.0. It provides everything you need to integrate with AngularJS out-of-the-box bindings, component configuration and directives, template directives, form validation, event handlers and much more and yet Kendo UI tooling does not depend on AngularJS. So if you want to use it with Angular or not, that’s totally up to you. You could check it out at KendoUI.com]_ ****CHUCK:** Hello everybody and welcome to episode 69 of the Adventures in Angular show. This week on our panel we have Aaron Frost. **AARON:** Hello! **CHUCK:** I’m Charles Max Wood from Devchat.tv. I just want to remind you all to go check out JS Remote Conf – jsremoteconf.com. We also have a special guest this week and that’s Pascal Pretch – and I know I killed it. So you want to introduce yourself? **PASCAL:** It was indeed pretty good. Yeah, hello. **CHUCK:** I get credit for pretty good; I’ll take it. [Chuckles] **AARON:** Yeah. **CHUCK:** So you want to tell everybody who’s listening who you are, what you do? **PASCAL:** Yeah, sure. My name is Pascal. I’m from Hannover, Germany. It’s pretty great and rainy there today. I’m a software engineer and a trainer at thoughtram which is a company which I’m running with my buddy Christoph; we do Angular trainings, Git trainings. We work a little bit on the Angular 2 project here and there, do open source contributions a lot and that’s pretty much what we’re doing. **CHUCK:** I was going to say we brought you on – Lukas actually recommended that we bring you on and talk a little bit about some of your contributions to the body of work out there regarding Angular 2. So do you want to talk a little bit about what you’ve done and what’s out there as far as being able to learn Angular 2? Especially since we’re getting close to it going into beta. **PASCAL:** Alright. So here’s the thing – there are currently plenty developers working on the Angular 2 documentation, and it just happens that Christoph and I are also part of it. So it started all, from our side, basically with us writing a lot of technical articles or thoughtram blog. We started that last year when we started an article series on exploring Angular 1.3 [inaudible] wrote articles on the main topics, the main features that come into this release. We continued with that over the months by writing articles on Angular 2. It turned out that a lot of people are interested in Angular 2, of course, and a lot of people also like what we’re writing about. At some point, we basically reached out to Brad Green and we said, “Yo listen; we are writing these articles and the community seems to love them. How about we help out with the documentation? Because it seemed like there’s not – no one really working on it but there was so much working on under this project.” So we offered our help and they said that they like it. We started contributing to the documentation. We mainly worked until now on the dependency injection guides together with Ward Bell, who is currently not on this show but maybe he jumps in later. And we’re about to work on some other chapters for the documentation. **CHUCK:** Yeah. I know Ward’s been trying to join but I guess there’s a network issue or something somewhere; we’re hoping to get him on. So when you're looking at Angular 2 and you're trying to decide ‘okay, we need more documentation here or we’re trying to decide where to contribute to’, how do you make that call? What makes you go ‘okay, this is the place where we want to spend our time’? **PASCAL:** Well, regarding the documentation itself, it’s mainly Ward who is actually in charge of assigning chapters to the authors; we’re basically discussing the [inaudible] what is needed and then he – most of the time, he knows about it. He knows what is needed; he knows which gaps need to be filled. When we write our articles, we basically – we just think about some topics that we want to learn about, like something that we don’t know about yet then we dive into that topic and then we start writing articles about it. Sometimes, content from those articles also end up in the documentation, but it’s mainly really the core team that decide what chapters need to be written next or where more content needs to be written for. **CHUCK:** Ah, gotcha. **AARON:** So how many people are with you guys on this? How many people are helping Ward out? If you guys are included, how many additional people? **PASCAL:** Right. So I think we just started with Christoph and myself, and Ward. Then we extend it with John Papa and a couple of other guys. In fact, there were some planting new people popping up in the Slack chat or whatever we’re using there. I don’t know; I think we have about maybe ten people working on this now. **AARON:** What specifically are the pieces of the documentation that you're working on? What’s been assigned to you guys? **PASCAL:** Since we – I think one of the topics that we digged into the most was dependency injections. So we worked on the chapter on dependency injection and also advance dependency injection; everything from – starting with simple service injection and these kind of things to hierarchical injections. So there are basically two parts of the documentation right now that are covered for dependency injection but we still have to do some more work on that to be honest. **CHUCK:** What’s changed in the dependency injection? **PASCAL:** Everything changed. **CHUCK:** Oh, is that all? **PASCAL:** Yeah, just that. **CHUCK:** Okay. **PASCAL:** When the whole framework changes, so does dependency injection. In Angular 1, you have basically – you have a flat dependency injection system. Let’s say if you build your own application with your own Angular module and you're using a third party library which is another module and introduces some services that might have the same name that the service in your module has, then it kind of conflicts; the last one wins. This is because you only have one injection in your entire application. And this is fixed in Angular 2 – it’s actually fixed very well. In Angular 2, you have much as a single injector but you have multiple injectors. So when you build an application in Angular 2 or you start off with a component, then each component behind the scenes gets its own injector even if you don’t know it. There’s even a thing called platform injector which basically sets up injection bindings or providers for you that you can share across applications, because in Angular 2 you can also bootstrap multiple applications which is pretty amazing. So it’s very different in a sense that you don’t just deal with a single injector. You can really configure on a component level, how dependencies are created for your specific component. **WARD:** And that changes the way in which a lot of things are given to, say, a component for example. I think about in Angular 1, when you would write a link function or something like that and you have a fixed number of parameters and they would be tossed in; now they don’t have to do that because they can inject anything at any time. **PASCAL:** Yeah, that’s correct. You don’t have those parameters that you have in the link function anymore; you can inject everything everywhere because –. Originally, there were two injectors – you have the normal dependency injector for your mobile dependencies, and then you have this element injector. Technically, there’s still an element injector but this is an implementation detail. The point is that when you build an Angular 2 application, you have a component – let’s say you built a tabs component which has tab child components, then if you are in your tab components to ask for the tabs component, then you can just simple ask for it through dependency injection as you do with every other dependency as well. Basically, there’s nothing different really; it’s the same syntax, the same APIs which is pretty cool. **CHUCK:** Now when they – because you said you talked to Brad Green and they assigned you this area of expertise to write the documentation for, how do you go about figuring this out? Does the core team just explain it to you and then you write it down so that normal people can understand it or do you go dig into the code? **PASCAL:** Yeah, that’s – so actually, the letter is the case. So when we work on the documentation and also – Ward is also into this; he wrote tons of documentation for testing – it’s pretty much like this – we are in this Slack chat and we can totally ask the core team questions, but of course they have also a ton of work to do so they can’t always answer questions, or maybe it takes some time until you really get your actual answer. So what happens is that you have to start digging into the code or you start playing with the code and see what happens. When I started digging into dependency injection, I had the – it wasn’t easier for me because there was already some documentation for dependency injection in Angular 2 right into the repository because someone wrote it already. It was very, very technical and not super complete but there was something there, something that at least describes how the API works. This helped me to understand the system, and it helped me to getting started with it, to at least to play with it a little bit and then to explore how things work in this DI system. Once I’ve done that, I dig a bit deeper and I really check out the source code and look what’s going on there and then try out some edge cases because you always stumble upon some questions. If there’s no one you can ask, then you have only two options. You either read the source code and then you understand it, or you start playing with the code and trying to reproduce your question and then trying to find that answer. This is what we’re actually doing most of the time, but we have some help and guidance from the core team when we have questions. Ward, do you have some thoughts on that? **WARD:** Yeah, and I think you're doing the digging so that everybody out there doesn’t have to. The role of an author and a dev guy is not to prevent you from getting to the APIs, but if any of us have ever dropped into APIs before, it’s all like ‘how do I turn this screw and flip that lever?’ And Pascal’s job, the authors’ job is to make you get not just the nuts and bolts but to understand why, what good is it. So one of the things that Pascal’s doing in there is also telling stories about how you would use this things called the eye. The API will tell you how to flip things but Pascal’s going to tell you why you're going to need it, what problem you're going to solve – that kind of thing. I think that’s the fun part of your job, don’t you agree? **PASCAL:** Yeah, pretty much especially because this is an approach that I haven’t done before. When I wrote articles at thoughtram, I kind of start the other way around. I usually – I just started explaining the technical things like how you can do things and I’m super excited about it and I write about it. Then when I started working on the documentation with Ward together, he was reviewing my documentation content and then he said, “Yeah, this is all nice and everything but there’s still this question ‘why do you want to do it’?” And it’s like as soon as you start thinking about the why, like why do you need this feature and what is the motivation, and which use case do you really need it, you write your content totally different because you can also – you can leave out a lot of stuff. Whereas in our articles, we go very, very deep into the topic; wee cover some things that might never end up in the documentation because it’s too technical, it’s too low-level, and you might not ever need it. So Ward is really helping out in giving you the right feeling for what content should go in and which questions should be answered. It’s challenging, too. So when we started with the DI guides and the advanced topics, Christoph and I – we realized that if we want to cover a certain subtopic of this chapter, we really need to come up with a use case for it. It turned out that for some topics, we couldn’t really come up with something. Then we decided to just leave it out for now because if we cannot come up with a use case, well then it’s probably not needed for now; it’s not important enough or maybe it isn’t important enough but even we cannot come up with a use case, then how should ever – come someone up with something who’s starting with a framework. So yeah, it’s [crosstalk]. **AARON:** If someone else finds a need for it, they can do a pull request then get it in the documentation, right? **PASCAL:** That’s right. Exactly. **WARD:** The other thing that Pascal’s doing is when you look at these APIs, there’s a five or six different ways you come at it. But as a developer, there are certain things that feel more natural and feel more comfortable than others, and it’s Pascal’s job to find the ones that feel natural – at least feel natural for the use case. Since nobody has ever written Angular 2 apps before, that’s a voyage of discovery. **PASCAL:** Yeah, that’s true. What comes into play is that while the framework is still an alpha – we’re very close to beta now but APIs are still changing here and there. And when you write documentation, you also realize that some APIs are not – they're probably never going to be perfect but some APIs are not really – they don’t really fit what you're doing right now. Sometimes, we also just end up having discussions for I don’t know how long, talking about how this DI API should be called now so it’s a lot of energy that goes into that. **WARD:** But I think the consequences that you're helping make the product better, by acting in the role of the user and saying, “Hey, if this doesn’t make sense to me who’s spending all this time here, maybe the API has improved,” then we get into those discussions is what you're talking about. **PASCAL:** Yeah, that’s right. **WARD:** By the way – and mind you, you’ve been doing that for a very long time, long before you joined this project. **PASCAL:** Well, yeah. That’s right. We start with our technical articles almost a year ago but we started really digging into Angular 2 at the beginning of this year. The first things we did were also just getting started articles, like how to build a tabs component, how to build a zippy component or whatever then we dig deeper into other topics. But yeah, it’s indeed challenging but it’s also fun at the same time, you get great insights of the framework. If you are someone who’s teaching the technology to other people which is what I’m doing, then this is very helpful because when you dig so deep into this technology, it really helps you to provide better content for your classes like when you teach someone. **WARD:** You’ve been doing a lot of training recently on this kind of stuff. What are you finding people’s reaction? **PASCAL:** In general, it’s like this – we’re doing Angular 1 training currently – mainly. Here and there, we’ve done some Angular 2 trainings like getting started trainings, but it always happens that more and more people are explicitly asking for how do I operate to Angular 2 and what does that look like in Angular 2 and how do I do this in Angular 2, will this feature still be there in Angular 2, so there’s already a lot of interest of there. And in the Angular 2 trainings that we’ve done so far, it turned out that some things – most of the things turned out to be very clear to everyone. For example, when you build a component in Angular 2 and it’s really just an ES 2015 class with some decorators on it, it feels very natural to most of the users. They don’t have to learn directive definition object anymore, this huge thing that we’re using in Angular 1; that feels more natural to them. On the other hand, the dependency injection, like the new dependency injection where you have multiple injectors, this is something that a lot of people seem to struggle with because they really have to rethink how they can provide dependencies for their components, and that they can actually override dependencies in their component tree. This is like a new thing and I think people have to just let this sink in and understand that this particular part of the framework is indeed a bit more complex, but it’s also way more powerful and way more flexible. **WARD:** And to be fair, you can almost pretend that it’s flat if you want to. You can start thing up at the top if you want to and just pretend it isn’t [inaudible] and get away with that pretense for a while. But as you say, you're going to be tempted to find out what this is all about and then you're on that journey with you. **PASCAL:** Yeah, that’s very true. **AARON:** So are you guys also writing the documentation for things like ng-upgrade? **PASCAL:** Yeah, as far as I know, Tero – I can’t really pronounce his last name. **AARON:** It’s Teropa. Just call him Teropa. **PASCAL:** Ah, Teropa. Teropa on Twitter. So he’s working on a chapter on ng-upgrade and I think he just recently twittered that he upgraded the project successfully using ng-upgrade. So there’s surely something nice coming very soon. **AARON:** Yeah, I saw that tweet. That was actually kind of a confidence inspiring to see that someone like him would like to use it and he said it just worked which is actually gives us a hope in my work. **PASCAL:** Definitely. The interesting thing is that this year at AngularConnect, I gave a workshop on upgrading to Angular 2. During that workshop, we used the ng-upgrade module to take an existing Angular 1 application and then upgrade it into Angular 2. This time, the [inaudible] package wasn’t really a package, so you couldn’t really just use it right out of the box; you have to hard copy the source code into your projects so you can use it, but it worked out. It’s pretty cool; the APIs might still change at some point but it’s nice that it’s working. You can really – you can use Angular 1 and Angular 2 side by side and use – make Angular 1 and Angular 2 components into operating which is very, very cool. **AARON:** In the documentation, is there something that explains how am I going to use the Angular 1.5 component to upgrade more easily to Angular 2? **PASCAL:** I’m not sure if we planned to cover this one in the Angular 2 documentation to be honest, because the [inaudible] component helper is – it is indeed a helper in that sense that it’s kind of simplifying the directive API because it gives you some defaults and then you don’t have to configure everything when you build a component directive. But when it really comes to upgrading, I don’t think that this component helper will really help because technically, it doesn’t really help with the operator itself. It’s a nice API for you to make components, and of course, if you think in components then you are closer to Angular 2; that’s for sure. But I don’t think it’s really helping with an upgrade because when you upgrade, there are actually two things you can do or three things – you either really do a big bang upgrade which is really like rewriting the whole application which I think is what will happen for most of the applications out there as soon as – as long as they're not too big. So if you have a small Angular 1 application, you can totally rewrite in Angular 2; that’s probably the easiest thing you can do. The second option is you componentize you Angular 1 application by maybe using [inaudible] component, you can do it; you don’t have to but when it’s there then you can just use it. The point is that as soon as you really have components and you think in components then you can really take component by component and rewrite them in Angular 2. So really, it’s not like a big bang but you make a big bang on each specific component. The third option is to really run both frameworks side by side and then use ng-upgrade, then really make both frameworks communicate to each other. That’s upgrading for me where you really have to use both at the same time. **WARD:** It may be that the word ‘upgrade’ isn’t quite helpful because it suggests that it’s actually somehow transforming your Angular 1 things. It’s really help them either operate [inaudible] upgrade, don’t you think? **PASCAL:** Yeah, when you use ng-upgrade and – so maybe for those who don’t know, in an ng-upgrade you have a couple of APIs that allow you to make Angular 1 components work in an Angular 2 component and vice versa. But there’s one thing that is always true and that is when you have an Angular 1 application and you want to upgrade to Angular 2, you always have your Angular 1 module as a root component. So you always need that Angular 1 context and that means you always have to downgrade your Angular 2 components to make them run in your Angular 1 component or in your Angular 1 app. At the same time, you upgrade your Angular 1 components to make them work in your Angular 2 component. Sometimes it sounds a bit backwards but technically what happens is that in fact, when you upgrade an Angular 1 component, use it in your Angular 2 component, there are really some things that argues from the Angular 2 framework. I think as far as I know, the things like view caching for example, this is the thing that really comes from the Angular 2 framework even if you upgrade an angular 1 component, and even if it’s running in an Angular 1 module so you really get some benefits. **WARD:** Could you elaborate a little bit on that view caching for a second there, Pascal. I don’t know much about that; I’m not sure our viewers do. **PASCAL:** Well, I have no idea. It’s just a buzz word that I’m throwing around. [Laughter] But seriously, I read about it and I know it’s there, and I see Brad Green talking about it in his keynotes, but I have really no clue yet what it’s all about. There is this guy – Tobias Bosch in the core team. He is doing some crazy work on the compiler and on performance improvements. I’m watching the repository and I’m seeing all these commits and pull requests coming in that he’s doing. And when I see his pull requests and the stuff that he’s doing, I don’t understand anything. He’s like optimizing on a level that I can’t even think of and so I don’t think I have an answer for that. [Chuckles] **WARD:** Actually, that may be a great answer because who needs another term to worry about. It may just be another way of describing what we’ll all benefit from without even looking which is the work that Tobias is doing under the hood there. Because you're right; I’m listening in and it’s always ‘well, I think I can make this four times faster’, and then it goes off and [inaudible] things so it’s amazing. **PASCAL:** Yeah, that’s right. **CHUCK:** Yup. **AARON:** So when you describe the layout of the documentation, we’re calling it chapters; what is the chapter – I just want to understand how the documentation is going to end up being formatted. **PASCAL:** So I think things are still moving, but currently if you go to angular.io and then you go to docs, you can see on the left-hand side there’s this side bar, which is you have sections like tutorial with the tour of heroes tutorial which is mainly written by John Papa. It’s a great tutorial to get started. Then next to it, you have another section called Developer Guides and that’s basically – it’s not just one big guide; it’s rather really single sub guides. One of those guides for example is a guide about dependency injection. You have another guide about the template syntax or just about forms, but in this – in one particular guide, you can have different subsections that cover subtopics, isolated more or less. This might change at some point because you also have – next to a dependency injection, you have hierarchical injections which is actually part of dependency injections so we might have some nested structure there at some point, but I’m not sure what’s the state of this currently. Maybe Ward has some more thoughts on this? **WARD:** Well I have thoughts. It is thought to be – there’s a drill into the dev guide section; we tried to treat it as if each of those is a chapter. Now it maybe that one chapter lead to the next, so you have a dependency injection and an advanced dependency injection chapter right after it. And maybe, as you say Pascal, we may be able to get some depth there but let’s suppose that we didn’t; you should really think of those things as one chapter after another, and you could pick a chapter that you're interested in, a topic that you're interested in and go right to that chapter, but they do have a sequence. There is some intention that you’d be better off having read chapter three before you read chapter six, let’s say. Does that answer your question Aaron or am I missing something? **AARON:** No, that answers it. Thanks Ward. **WARD:** One of the challenges for the author is to both work as if you were going to parachute into that one chapter and not reading anything else, and try to make it work within the context of the other one’s around it and Pascal’s up to that challenge. **PASCAL:** Yeah. Not always easy. Actually, it’s more hard than easy. **WARD:** We’re going to keep throwing the hard things at you which is why – I’m going to put you on the spot here; we can always cut it out but I’m open that you’re going to take on the challenge of giving the broad overview of Angular 2 that would sit right at the front so that when Aaron opens up the dev guide and he goes to Chapter 1, he’s running into your chapter on the overview. So if you had to do that right now off the top of your head, ow would you sketch the architecture for me? What would you say so that they got it in about ten minutes? **PASCAL:** This is really tough. [Laughter] **WARD:** I told you I’d put you on the spot! Charles, we can cut it out! [Chuckles] **AARON:** It’s alright. **PASCAL:** So the thing is that – to be honest, I thought about exactly that. I thought about exactly that because Ward and I, we already chatted about this and he said that he wants this kind of chapter or we need that chapter and I thought, “Alright. If we’re going to do this one, we really need to think about how this – what this should look like and what should go in.” The problem with this topic – giving a general overview is that you really need to have an overview of it. You need to have the bird’s eye view picture of this whole framework in order to write such a chapter for the documentation. So I think that as of right now, I don’t think I know enough parts of the framework so that I can write such a chapter. Before I can tell you what this could look like or what I should about it, I would – the first thing I would do then is to go to the repository, and then compiling all the different parts of it as in very general, what kind of modules that we have in there. Trying to understand all the connections between all those different parts of the framework and then maybe come up with a sketch or something that gets you really – literally a picture that shows you what kind of parts you have. Then I might going to show it, Ward, and once we talked about it two and a half hours, you're probably going to throw it away and then he comes up with tons of better ideas and then I’m going to do a new sketch. Then maybe at some point, some designers, or someone is going to make it a really nice picture, then I’m going to start writing content about it. **WARD:** I think you're being too modest but [chuckles] I can’t think of nobody better than you did to do this so I know you’ll bring it off. **PASCAL:** Yeah, you just put some pressure on it now, thank you. [Laughter] **CHUCK:** So I am wondering a little bit with the documentation. It seems like you are looking for people probably to read it in a particular manner or even a particular order. So with the documentation, how should people approach it when they see it? **PASCAL:** Well, I think that it really depends. So if you start off with a framework like you haven’t done anything with it before – you just want to start learning it; the first thing as a user what you should do is definitely check out the Tours of Heroes tutorial because it gives you a run through the framework. It’s like using most of the important features of the framework and you build a little application without digging too much into detail, then you already get a kind of overview of what’s going on and how you built things. Then I think you can totally go into all the other chapters if you want to dig into some specific topics, because when you do this tutorial – Tours of heroes – there will surely be some questions that come up. For example, there’s one part where you generate a list of heroes using ng 4; it’s like the equivalent of ng-repeat in Angular 2 but it’s still different; the syntax is different. You have this asterisk symbol that you have to put ng template. There are some pointers in the documentation that say something like ‘if you want to read more about this particular directive, check out this chapter’; this probably already gets you there. If it doesn’t then at some point, you're probably going to check it out yourself. I think that’s pretty much what you can do; you should start with a tutorial and then questions will come up and then you will probably just dig into all the other chapters. If you're already kind of familiar with Angular 2 and you know everything that is happening in the tutorial then you probably just jump right into one of those other chapters. And if you know everything about that, then you should just talk to know me or talk to Ward so you can write some more documentation. **CHUCK:** Gotcha. **AARON:** So if someone in the community, they got a spot where they can dedicate serious amounts of time, maybe somewhere like [inaudible] or someone wants to put one of their employees to donate time to it, how do they get involved? Who do they talk to and how much of an effect can they have on this documentation project that you guys are working with? **WARD:** I think that’s a question for me and the answer is contact me and tell me what you want to do and we will work something out because we have topics that need attention. **CHUCK:** Alright. Let’s go ahead and get to some picks, ward, do you want to start us off with picks? **WARD:** I saw a crazy good movie last week that would not appear in your regular theatre. It’s called Heart of a Dog by Laurie Anderson, the multimedia artist that you may have heard about. Coincidentally, I just learned that her husband was Lou Reed who just died recently. But she stands on her own; I only knew her on her own and it’s this amazing avant garde film full of wit and depth on a troubling subject which is the death of the people we love. I know I sound like a real downer when somebody’s going to take me and say, “Oh great. A feel-good movie of 2015,” but the darn thing is really, really worth seeing. So dig it out and check it out. She is amazing. **CHUCK:** Alright. Aaron, what are your picks? **AARON:** I’m going to do one pick and I’m at the Chrome Dev Summit right now. They have some really cool codelabs online, and they break down and they get really easy to learn. Some new things coming out on the web like the physical web and Bluetooth, but they also 0have a tutorial for service workers and for a lot of us who haven’t maybe able to use one. It’s a really good tutorial to understand ‘hey, this is how it works’ and ‘this is how you turn it on if it’s available and turn it off if it’s not available. So the Chrome labs from the Chrome Dev Summit – my pick and we’ll have a little two minute show with it. Go check them out; it’s actually [inaudible] ten to fifteen minutes tutorials you can watch, [inaudible] you can watch to learn how to use some of these things that the Chrome team teaches us about. So that’s my pick. **CHUCK:** Alright. Tomorrow, I’m going to be giving a speech at Toastmasters. I know I’ve picked Toastmasters on here before but I’m just really excited because this is speech number ten out of the comp communicator manual to basically back that up a little bit so that non-Toastmasters people understand. The first level of speaking competency or the competent communicator is the competent communicator manual. It includes ten speeches, so since I’m giving my tenth speech, I’m about to complete my competent communicator and I’m really excited. So I’m talking to you about it on the show because yay me, right? But the other things is that if you're looking for a way to increase your ability to communicate or to lead because the other basic manual is the competent leader manual, I highly recommend you go check out Toastmasters. If you go to a club and it doesn’t seem quite awesome, try a couple others in your area. I’m finding that I lucked out and walked into one of the best clubs in the state where I’m at. Some of the other clubs are good but less awesome. So if you're looking for a way to level up that way, then by all means go check that out, and that’s my pick. Pascal, what are your picks? **PASCAL:** Well I have two picks. My first one is the new Nexus 5X; I got it a couple of days ago. I love it; it feels nice. It’s not too big, it’s not too small and something that I haven’t thought before is that I really like the fingerprint sensor. It works very well and it feels very good. I dropped the phone three days after I got it and now it’s damaged, but I’m going to get a new one so that’s nice. So that’s my pick; I like that phone very much. My second pick is since I really liked the Angular community, and there are plenty, plenty nice people out there that help you out everyday on different chats like Slack chats or Gitter, IM or whatever. There’s one guy who’s doing tons of community support, and he’s also very active on Twitter and he’s sharing his latest and greatest thoughts on Angular 2 and experiments. This is Rob Wormald, so you should definitely follow him on Twitter if you want to get some nice updates. He’s definitely out there to help you if you have any questions. **WARD:** I second that. Great. **CHUCK:** Alright. Well, thanks for coming Pascal and sorry for all the technical difficulties. **PASCAL:** That’s alright. Thank you for having me. **CHUCK:** I blame Skype. [Inaudible] that Microsoft. Alright, well if people want to follow up on what you're doing or get involved in any projects that you're working on, what should they do? **PASCAL:** There are a couple of things that they can do. So you can follow me on twitter which is just my name, Pascal Precht [chuckles] or you can follow thoughtram, and you can subscribe to our blog if you want. If you want to get technical articles on almost weekly then you can do that. **WARD:** Can I plug that? Can I plug the thorughtram blog? Because that’s a go-to blog for me. **CHUCK:** Yeah, how do you get to it? **PASCAL:** Oh, well it’s just blog.thoughtram.io. **CHUCK:** Awesome. **PASCAL:** I can give you the link [crosstalk]. **CHUCK:** Yup, put it in the chat [crosstalk]. **WARD:** I consider one of the most important resources that an Angular 2 person should be following. **AARON:** My [inaudible] with Victor [inaudible]? **WARD:** Absolutely. When Victor writes, it’s magnificent, but he doesn’t write as often in thoughtram so you should definitely follow. Follow them both. **CHUCK:** Okidok! Well let’s go ahead and wrap up. Thanks everyone for listening. Tell your friends about the show and check out JS Remote Conf and we’ll catch you all next week.**_[Hosting and bandwidth provided by The Blue Box Group. Check them out at bluebox.net]_****_[Bandwidth for this segment is provided by Cache Fly, the world’s fastest CDN. Deliver your content fast with Cache Fly. Visit cachefly.com to learn more.]_****_[Do you wanna have conversations with the Adventures in Angular crew and their guests? Do you want to support the show? Now you can. Go to adventuresinangular.com/forum and sign up today!]_**