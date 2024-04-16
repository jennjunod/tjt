---
showLink: "https://www.youtube.com/watch?v=XxVIDhLhtjk"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-robust-rudiments-with-philip-gannon"
title: "Teach Jenn Robust Rudiments with Philip Gannon"
publishDate: "2022-07-28"
coverImage: "https://i.ytimg.com/vi/XxVIDhLhtjk/maxresdefault.jpg"
---

This is a transcript with timestamps of a technical conversation.

Write a one sentence summary of the transcript and a one paragraph summary.
  - The one sentence summary shouldn't exceed 180 characters (roughly 30 words).
  - The one paragraph summary should be approximately 600-1200 characters (roughly 100-200 words).

Create chapters based on the topics discussed throughout.
  - Include timestamps for when these chapters begin.
  - Chapters shouldn't be shorter than 1-2 minutes or longer than 5-6 minutes.
  - Write a one paragraph description for each chapter.
  - Note the very last timestamp and make sure the chapters extend to the end of the episode

Format the output like so:

    ```md
    One sentence summary which doesn't exceed 180 characters (or roughly 30 words).

    ## Episode Summary
    
    tl;dr: One paragraph summary which doesn't exceed approximately 600-1200 characters (or roughly 100-200 words)

    ## Chapters
    
    00:00 - Introduction and Beginning of Episode
    The episode starts with a discussion on the importance of creating and sharing projects.
    
    02:56 - Guest Introduction and Background
    Introduction of guests followed by host discussing the guests' background and journey.

    ## Transcript
    ```

TRANSCRIPT ATTACHED

---

[00:00] - Hey, Philip. Thank you for joining Teach Gen Tech. Please introduce yourself and what you're going to be teaching us today.
[00:09] - Sure. Yeah. So, thanks for having me. Obviously, my name is Philip. I'm a lead engineer in a company called Wunderman Thompson MAP, super cool place to work. And generally, the kind
[00:20] of stuff I want to talk to you about today is basically the foundations or rudiments of software development. There's a lot of really interesting basics that people overlook
[00:29] because of the basics, but they set you up so well for the rest of your career that it's like only a fool would ignore them. So, I want to talk a little bit about that today
[00:38] and hopefully whet people's appetite about the topics. - I dig that because something that we kind of talked about too is creating theory Thursdays
[00:48] where it's not anything we're doing on screen, we're not peer programming, it is just talking about what goes behind the scenes of the code. Like, what do we need to know? What logic
[00:59] do we need to start thinking about? And for everyone watching, yes, I'm like moving around with my pen because I want to make notes of when we talk about each of them because it's
[01:10] definitely something that I know one of the ones you mentioned were solid, right? - The solid principles, yeah.
[01:19] - I was just like, I don't even know what that is. But since we're talking about different things throughout it, I need to take time because to remember where they're at. So,
[01:27] thank you again. I appreciate it. Where do you want to, well, before we get into it actually, how did you get to the point where you're at right now? Because you also have the podcast
[01:39] and you talk about like interviewing and soft skills and so much more than just engineering and the software. How did you get to that point?
[01:50] - It's a bit of a long road, a couple of years, but I mean like a big part of it, the tech community is giving back. So, you see people that do like amazing open source contributions
[02:00] and I mean like the majority of software we use as developers is open source, right? So, you can contribute that to yourself. We're building upon the wisdom of other people.
[02:08] And then of course, there's a lot of great people who do technical tutorials on like how to get started, how to build certain things and all the rest. And I kind of found out
[02:16] that there was a niche missing where people don't really talk about the other side of software, which is the soft stuff. So, that's like, you know, management, leadership, interviews,
[02:27] how to have a good work-life balance because work-life balance is a huge thing in the development world, right? Control your stress, control your workload, set boundaries, things like
[02:36] that. People weren't really talking about that. And I felt that like maybe the more technical aspects were well covered by other people, but that I could certainly speak about
[02:45] public speaking, leadership and all that kind of stuff and help people with that. So, my podcast is kind of a way for giving back with that to show people how to interview better
[02:53] and just how to have a successful career without focusing too much on the technical aspect. Does that make sense? It does. And I love that you're doing that
[03:03] because I would say that tech world is like its own species. Like you have to talk about it differently. You have to think about it differently. And whereas if you're talking
[03:15] to somebody in marketing for spacing, so we're going to say like a beverage, like they're not going to think about the same things as marketing in the tech world. And what up Kay,
[03:30] the Pringle one? How's it going? Thanks for joining. And so, I think it's really cool that you talk about those soft skills. And as somebody mentioned of like soft skills
[03:43] and core skills, I think that was Ramon. He was on the podcast a while ago. I like how you say that soft skills are core skills too. So, we will get into all of that one day,
[03:54] but can't go down that rabbit hole. Where do you want to start? I'll just start rambling and then you can stop me at any time.
[04:03] Perfect. I dig it. We can stop and start like that if that's okay. So, I guess like for the topic, we said robust rudiments. Rudiments is a really deliberate
[04:12] choice because if you think of something like maybe say drumming, for example, you have your rudiments and they are patterns that you practice continuously. I think there's
[04:20] a set of like 40 in total of combinations of left and right, left and right, left and right. And what they're designed to do is they're designed to build your muscle memory
[04:29] to help you build your coordination and also develop a sense of rhythm over time. And then as you progress further in your career as a drummer say, you will try different combinations
[04:40] of these. You'll swap your left and right for your kick and your snare or different toms or different cymbals. And that brings you to the musical aspect. Your playing becomes
[04:47] more automatic and more expressive and you've built this amazing muscle memory to work with. Can you be a great drummer without these things? Absolutely. But I find that maybe if you go
[04:59] through this system of building up these rudiments, you maybe become a more technical and better drummer overall. And it's kind of the same with programming that like you pick up the
[05:08] basics and you reuse them constantly. You're going to follow the same patterns all the time, but like there's a deeper theory to a lot of them. And we'll talk about things
[05:17] like say object-oriented programming and stuff like that, which for a lot of developers, they kind of know a little bit about, but if you get deeper into the headspace about
[05:25] it, you kind of get a little better at solving solutions. I think you put together more well rounded solutions and those neurons fire together and they wire together the more you do it.
[05:35] And you're building this mental muscle memory effectively where you can actually get some solutions out from your brain to your fingers, the keyboard much faster and much clearer.
[05:42] So I guess that's the idea of going through the rudiments. Right. Makes sense. It does. And I like that because I think I've thought about like rudiments abstractly, like
[05:54] I've never actually fully taken a moment to be like, what is rudiments? And I like how you explained it as, as a bit more of specific repetitions and how doing those repetitions.
[06:07] Yes. Like if I, with my other show, like shit, you don't want to talk about, we talk about a lot about therapy and a lot of therapy is rewiring our, our mindsets to have better
[06:22] connections. And that's like the same thing that you're talking about. And I love it. And what up Akari? Hey.
[06:31] So I really dig that. It really comes into our world in so many different aspects than just coding yet. I think the logical side of it is where many people get stuck because
[06:43] I don't know those or knew that they really existed with my natural Googles of trying to figure out JavaScript.
[06:49] Okay. Okay. Let me like Googling is, is the super rudiments, the core, core, core skill of every developer, right? You get that one down, your career is sorted. You don't have
[07:01] to worry about the rest, but okay. So talking about some of them I guess to tell a bit of a story, we see an awful lot of the drive towards data structures and algorithms. And
[07:13] it's, you know, a big thing in interviews where you have to do like these hacker rank tests or code wars and stuff like that. And they test your ability to maybe like balance
[07:21] a binary tree or do something with a LinkedIn, a list or whatever. And there's a lot of candidates who go for these interviews and graduates and stuff like that. And they will spend like
[07:29] six months full-time learning data structures and algorithms. They'll go through courses, they'll buy books, they'll do all the rest. These are super talented people, but they
[07:37] come out at the other end, maybe with a job or whatever happens, position. And while they're really good at writing algorithms, maybe they don't know how to join everything together
[07:46] properly in an application that makes sense. And especially when you join a company, you're usually joining a pre-existing platform. And usually there's a way to code is structured
[07:55] and they can't rock that sort of thing at the start, right? So maybe there's a leaning towards one side where it should be leaning towards the other. And that's towards these
[08:04] concepts like object-orientated programming to get better at that, the design patterns and then architectural patterns. And we can jump a little bit into them at the moment.
[08:13] So for object-orientated programming, I mean, you're using it at the moment. If you're using JavaScript, JavaScript can do it. And I'm sure anybody C#, PHP, all the rest, very common
[08:22] concept, which is a software paradigm where your solutions are based on objects instead of just pure functional logic. So if you think of like a script and the script is going to
[08:33] be like, I want to get from A to B, I want to take in my data, process my data and spit it out. That's very logical, concise, one-way sequence. When you think of object-orientated
[08:44] programming, you're actually describing things in terms of objects, the properties they have and the behavior they display and how they interact with each other. And maybe that sounds
[08:54] like super abstract and out there, but the general point is you're just, you're modeling your problem space. So if you have a system where it takes in some data and then it sends
[09:04] out an email, well, maybe you'll have an object, which is an email service and that handles sending of emails. So it's, once you kind of get to it, it's handy enough. Really does
[09:16] make sense because you're building basically bigger solutions and you're building whole systems where parts can interact with each other, but you can build them one piece at
[09:25] a time. And one of the core aspects of object-oriented programming as you build little units of code, you describe the behavior for each of these, and obviously it's chains of them working
[09:35] together. How do you interact with each other? It's your full system of how everything works. That's something that we had Mishko, who on the show that he created AngularJS and then
[09:49] he recently just launched quick. And that was something that he was talking about, like with his kids. And I love this, like a comparison to kids, because I'm like, it's basically
[09:59] what we all have to do is be a newbie and think of these all as bare basics that we're learning them for the first time. And he talked about how it's very, very small steps and
[10:12] very, very small projects and things that you learn them and then they all stack together. So when you think about like, I'm going to go with Twitter because that's where I meet
[10:24] like half the guests on here. It's been complexity built over time. It wasn't something that just automatically appeared like this. And so with object oriented, and I wanted to ask
[10:39] this to your previous, before we introduced object oriented, do most companies say they have a certain way of doing it or is it more like suggested instead of actually said?
[10:57] You pretty much know from the languages that they use. So I mean, like for the most part, if you're working in a C sharp.net shop, it is an object orientated world. Whereas if
[11:06] someone said, well, actually we do things in F sharp. I mean, that's a functional language. It's not an object oriented language. You wouldn't know. But I mean, like you would
[11:14] generally tend towards one or the other. So like people who work in JavaScript, sorry, Java or C sharp, or even JavaScript to a certain extent, it's pretty much just object oriented
[11:23] code all the way. You wouldn't really think about it. But then there are people who would maybe specialize in functional languages, functional solutions, and that would just
[11:31] be their whole jam for their whole career. Okay. I'm taking notes. Okay, cool. Thank you.
[11:42] Okay. So moving on from that, as you're writing your software, and as you said, a lot of these things are like you learn little bits over time. So like if anyone's listening and they're
[11:51] like, man, I don't know all of these things. Well, like, look, I've been doing this for 12 years. I don't know all of these things in in-depth detail, but you'll pick up little
[11:59] bits and pieces over time and you'll join the dots. And then you'll generally tend to take on what you need, right? So as your people tell you things or your Hill concepts, you'll
[12:08] do a little bit of Googling, and then you get a better understanding as time goes on. But based on the object orientated part, once you kind of get familiar with that, and once
[12:17] you kind of understand the core concept, which is your modeling, your problem domain, your solution domain, you start to deviate your code in particular ways. And then you come
[12:26] across what's usually called the solid principles. And these are five principles for just writing really good object orientated code. People dispute them, and that's fine. And people
[12:37] dispute the other, and that's fine. But I think just following them generally gives you just like a really clear framework of just good practices to follow. And solid actually
[12:46] stands for an acronym, which is really easy. So like five principles, and I'll jump through them and stop you at any time. The first is the single responsibility principle. So if
[12:56] you have an object or a class, you should really only do one thing. You shouldn't try and do two things. And when we say do a thing, that's like an abstract concept. You get to
[13:07] decide what that is. That thing could be, we talked a little bit in email service, right? So if you have an email service, the only thing it should do is send emails. It shouldn't
[13:15] send text messages. Shouldn't talk to people on WhatsApp. Shouldn't have artificial intelligence built in. It should just send emails. That makes it super easy to verify that the functionality
[13:27] works. It makes it easier to write it in the first place. And then it makes it easier to write tests against it. And then when other parts of your code want to do something, they
[13:34] know want to send an email, call the email service. Easy peasy. And you might have other parts within that. So obviously as your applications grow, they might delegate some of their responsibility
[13:47] to other objects and classes. So again, in our email service, you might have a particular class that says, well, we want to send it to an email address. Maybe we want to validate
[13:56] that email address before we send it. So you might have a validator class. It's one responsibility. It's just to validate that an email address is valid or not. So you break up your problem
[14:08] into lots of tiny little parts. And each part that processes part of that problem just has one little responsibility, which is that one particular part.
[14:17] Okay. Still with me?
[14:21] Still with you. Still following. Okay. So let's say yes. Solid. We went to the next one, which is the open and close
[14:29] principles. And this one, a little bit squiggly, but we'll try our best. Basically that your objects are open for extension, but not for modification. And we'll go back to our email
[14:41] service for a second. If your email service, you know, imagine somebody wants to extend the way that your application communicates. And they might say, well, right, we also want
[14:51] to be able to send WhatsApp messages. Your email service shouldn't do that. That's not its responsibility. So you wouldn't modify it in order to add this additional functionality.
[15:03] But you could extend it for value add functionality. So you imagine with an email, you say, okay, I wanted to send it to this person. And here is the HTML I want to send as part of that
[15:14] email. That could be one method. You might extend it and add another method and say, well, here's the name of the person I want to send it to. And instead of sending a big
[15:22] block of HTML, I'm actually going to send some plain text and maybe the name of an HTML template.
[15:30] So our responsibility is still to send an email. So that's okay. But we've just extended it as a kind of a value add kind of thing. There's another way to use it, but it still
[15:39] does pretty much the same thing, which is just send emails. Just you now have two methods of doing that.
[15:44] And what was that one called again? Open and close principle.
[15:47] Okay. Thank you. The next one in L, well, this is a bit tricky. The list cup substitution principle, which
[15:57] sounds much scarier than it actually is. Anything that can use a base class should be able to use a derived class. So you imagine you might have a shape class and your shape
[16:10] class has a meta that's like, well, get the area of a shape. And you think, okay, well, for a derived class that could be like, say, a rectangle. So rectangle's area is width
[16:20] by height. Or for a triangle, it's whatever, width by half the height or whatever. And then for a circle, you involve pi and all that kind of fun stuff. But if something wants
[16:29] to do something with shapes, it can say, I'll expect the shape or I'll expect any descendant of shape, which could be triangle, circle, or square. And I don't really know the difference
[16:40] and I don't care. All I know is it has a get area method and that's all I depend on. I don't really need to know about the details. Make sense? Or trickier?
[16:53] It doesn't 100% make sense. But I think one thing that I'm seeing within all of these frameworks is there's things within the frameworks that I need to look into and ask more clarification.
[17:08] I don't think I'm there yet. But it's giving me an idea of what to look up or what to ask later. That is one of the hardest lessons I've had to learn on this teach gen tech journey
[17:20] is it's not all going to make sense right away. Half the time it's going to be like somebody, I understand you're saying words, but I don't have a visualization or understand
[17:31] how it actually works. But there's things that I can look into to like, you mentioned two different phrases of how if you can do one thing, you should be able to do the other
[17:47] in the substitution. And it's the type of thing that I'm like, cool, I can really listen to that part and go look it up later. And then if I don't fully understand what those
[17:58] are, then I could have you or somebody else back on the show and be like, hey, can you explain this to all of us? Yeah, we can certainly come back and do another
[18:07] version with like code samples and all the rest. That's not a problem. But I mean, like you could go your whole career without even hearing the words this got substitution and
[18:14] have a very successful career and not worry about it. But it's just, again, you'll pick up little bits over time and you'll take the bits you need and you'll forget the bits you
[18:22] don't then that's fine. That is, again, that is life. That is how I feel like we get through all of life. So, okay, cool. And then what is I stands for
[18:33] interface segregation, which again, sounds an awful lot scarier than what it is. Basically, when you have objects that depend on other things, there's usually an interface between
[18:44] them and an interface is just like a contract. And the contract says, like, hey, I can do these things. I can provide this value to you. You don't really have to worry about
[18:53] the internals of how that happens, but just this is the value I provide to you. So, for an email service, that might have an interface that basically says send. Send a thing. And
[19:05] you might have different services that use the same interface that just say send. You don't really care what happens behind, but just that they say send. Interface segregation
[19:13] is kind of a thing where when you're giving a contract or giving an interface, you only want the bare minimum of functionality there. You shouldn't have, like, tons of extra methods
[19:24] just in case somebody might need them someday. Keep it as short and sweet as possible just to the things you want to implement. And that gives you less to implement and also makes
[19:34] it much clearer, again, part of the responsibilities of what you have an interface for, what it actually does behind the scenes. So, basically, just when you provide an interface, make that
[19:43] as small as possible, the minimum amount of value add you can get, if that makes sense. Yeah.
[19:50] For the most part. We're going for the most part. Okay.
[19:53] Like, you're explaining things well. It's the context beforehand, again. So, and this is what I love about it is I've had it when I first started. I could not comprehend what,
[20:04] like, the first three speakers were saying to me. And then, like, on my fourth guest, I was, like, oh, that's starting to make sense. Yay. So, it's definitely something I like
[20:15] how you mentioned that we learn some bits and then we forget some bits. But, you know, it's really cool how they always can stay in the back of our mind and then click later.
[20:25] Yeah, yeah. Exactly. So, the last one, the D, probably one of the more important ones for me. Dependency Inversion. And this is a really sweet one, if you can kind of get
[20:37] this one down in your career. It's a really nice one. Basically, depending upon abstractions and not concrete implementations. So, we talked about interfaces before, and an interface
[20:48] is basically just a contract of these are the things I do. If you think of something like, say, a file storage service, okay, that might have an interface that basically says
[21:00] here's a list of folders, here's how to get a file, here's how to save a file, and here's how to delete a file. So, that's the value that it adds. That's the value that it has
[21:11] available for other things to work with. But then when you think about it, it's like, well, what are the implementations of that? You could save to a hard drive. You could save
[21:20] to a CD-ROM, for people who are old enough to know what CD-ROMs are. You could save to your cloud storage on Azure Blobs or AWS or whatever. Or maybe you could store in memory.
[21:33] Whatever uses that interface, so say you have a service that's like a REST API that takes a file and says save the file somewhere. That service doesn't need to know about the internals
[21:43] of what happens, the actual concrete implementation. All it needs to know is to say, hey, there is an interface. It has a method, which is save a file. So, I'll just give it a file.
[21:56] It will tell me whether the save is successful or not, and that's all I need to know. I don't need to know where that's saved. I don't need to know how it's saved or how quickly it's
[22:03] saved or whether it's this planet or the moon. All I need to know is that it is saved. And then you would just give it the different implementation over time. So, say maybe a
[22:14] user has another option of save to the cloud or save to my drive. Again, your actual system would depend on the interface for that, and then behind the scenes is whatever implementation
[22:25] does whatever it's supposed to do. >> I will say, I'm just glad you didn't say floppy disk, because I feel like that is where, like, no one -- I mean, I knew they were out
[22:38] there when I was a kid, yet, you know, CDs are more of what I grew up with, but, you know, you also didn't talk about, like, A track or something. So, I think we're good.
[22:51] >> I think most people's reference for the floppy disk is just the save icon now, right? >> That is true. >> Most people, they've never held one, they've
[22:57] never used one, but it's the save icon, right? >> Yeah, that is so funny. It is. I just realized that. I didn't even put two and two together. That's funny. Okay. Cool. What is after solid,
[23:11] or are there ways that we can implement solid? >> Ways to implement solid is, as you're going through your code, and, I mean, like, you'll do an awful lot of exploration over time,
[23:20] you'll work on a lot of different projects and a lot of parts of projects, and over time, you'll start to see these pop up, and maybe you'll be working on your code, and you'll
[23:29] be, like, you know what? This class is doing two different things. Maybe I can get it to do one thing. Maybe I can make two classes instead, and that'll just be a little bit
[23:38] easier to deal with, and over time, you'll naturally lean towards less complicated solutions, hopefully, and that allows you to speed things up, because instead of thinking of just one
[23:48] massive class with, like, three or 400 lines of code, you might be able to break that up into three or four subclasses that each handle only little pieces at a time, and that actually,
[23:58] like, it's much easier to get around in your head space. It's much easier to explain to people, and then later on, when you're working in a team and doing things, it's much easier
[24:05] to maybe review that code or share that code or integrate it into other people's changes or your main branch or your platform. So just practice, practice, practice, and you'll start
[24:16] over time to see them, or you'll learn about them, and you'll say, "Hey, I want to implement that. I'll give it a try," and you'll go through it, but, again, some of them, you might not
[24:24] bother, so that's fine. >> Got it. And just to make sure, Bakari or Kay, do either one of you have any questions
[24:31] so far? They might be half-listening. I feel like that's what most people do with livestreams. They, like, half-listen and then go watch it later when they, like, something piques
[24:44] their interest. So it's kind of hard to pay attention to livestreams, I've noticed, because, like, I really want to, but I also learn really well by listening on double-time instead of
[24:58] listening, like, just normal. So I don't catch even a lot of speakers because I'm like, "Oh, it'll retain better if I'm doing it in a different way," like, while I'm doing dishes, listening
[25:10] on double-speed instead of watching someone talk, except if I'm actually in the conversation. If I'm in the conversation, then I'm good. >> I think if you're watching somebody, like,
[25:21] your attention span starts to drift after 15, 20 minutes, and then it's like you just peter off. >> Yes, yes. I will say that we've had a
[25:30] bit more success than I think a lot of technical channels do when you're screen-sharing with it because then they're able to see and/or guess what they're going to do next or they
[25:41] can work their way through it, which I think that's been pretty cool. All right. So we talked about implementing solid. What else do we have going on?
[25:52] >> So building upon that, and maybe on another abstract level, you're going to see a lot of things like design patterns. Again, design patterns, maybe there's something you're using
[26:01] already. Maybe you don't even think about it, and that's fine. But if you do start to do a bit of digging about it, you'll start to see particular patterns pop up all the
[26:08] time. There's 23 standard design patterns. They're categorized in three ways. Don't need to worry too much about that. You don't even need to know them all by heart. But some of
[26:18] them you'll start to see so frequently that you'll just recognize them on site. The rest you'll Google, and that's fine. Just knowing they're there and having a rough idea is more
[26:26] than enough. But generally what design patterns are, they're common ways to structure your code typically to solve a standardized set of problems. And as you go through making
[26:39] particular things, you'll come across the same ones all the time. And a really good example is, say you're making a desktop application like, say, Photoshop. And you might say, "Okay,
[26:48] well, I want to replicate Photoshop, and a big part of Photoshop is undo and redo." You'd say, "Well, how do I implement undo and redo?" And of course, being the software world's
[26:58] so varied, you're not the first person to do it. You would think about, "Well, maybe when someone clicks a button, that's going to make an action in a list. And every time
[27:08] they click a button, it's going to add more actions to that list." And then if they say, "Oh, shit, I made a mistake." Well, they'd hit undo. What does undo do? Maybe it takes
[27:16] the last one off the list, and then we can roll from that. And then when you see that kind of thing, well, you go, "Okay, well, that's the command pattern." So if you're
[27:26] doing GUI applications, or desktop applications, or applications where there's undo/redo, you're going to see the command pattern a lot. And it's something you'll implement, and it's
[27:34] something you'll recognize on site, and off you go. And like, say, other examples, really famous ones, the singleton pattern. You might have
[27:43] something that you only want to be implemented once in your code. And you might think of something like a caching service. So every part of your code, before they hit the expensive
[27:54] database or they go do a really long, tedious operation, they might go and ask your caching service, "Hey, do you have this thing?" But you don't want everything in your system to
[28:08] make new versions of the caching system. You only want it to be one existing version that they can all tap into. So the singleton pattern is like, "Well, we'll allow you to make this
[28:17] once, and then any time any other parts of your code tries to make it again, we'll just give them the existing one." So there'll never be a new implementation. They're all using
[28:27] the same implementation. And this is really handy when you're doing things like data stores and caching and stuff like that. But you'll find over time that the problems you tend
[28:36] to solve or the problems you come across usually can be solved with just one of the standard patterns. So you'll pick up a handful of them over time. You'll ignore the rest. And the
[28:46] ones you do use, I mean, like, you get very familiar with them as time goes on. >> Okay. I am -- okay. Something that I hate to admit, but I'm totally going to admit,
[28:58] is, like, classes don't always make sense. Like, abstractly, they make sense to me. Like, actually figuring out how to write them, they don't really make sense to me. Because is
[29:13] our classes -- and this has to do with singleton. I will bring it back around. Because I don't think they're connected, but I want to ensure. Because in classes, is it where it will create
[29:30] a template that you can use multiple times for different items? >> Yes. So a class is a blueprint for an object. So a class basically says, well, when we have
[29:42] an object, that object is going to -- you think of a user record. The user record is going to have -- it's going to have a user name. Maybe it has a password. Maybe it has
[29:51] their email address. Maybe it has their age. That's what your class is the -- as a blueprint defines so that every time there's a user in your system, that's an implementation of
[30:01] that class. That's an object. And then you know that it has these properties. So bringing back to object-oriented programming, you describe the attributes you want your objects to have
[30:12] and the behavior they have. So you think for your user record, you have a class, a user record class, and maybe that has some functionality. Well, maybe we store their date of birth, but
[30:26] we might have a method to calculate their age. Really simple example, but whatever. So that's the functionality that it describes, the blueprint that it says, hey, these are
[30:35] the things that this can do. >> Okay. And then so a singleton pattern wouldn't use a class, but it could use an object?
[30:45] >> It does use the class. So it uses that blueprint. It makes the object. But then it makes one object. And then any time any other parts of your system says, hey, super class
[30:58] for your whatever, I want to make another one of these to do things, well, it will say, hey, one of those already exists. So I'm just going to give you the existing object. I'm
[31:06] not going to make you a new one. >> Would that be like going back to the reference of users, like if I already have an existing account, would a singleton pattern give me
[31:17] my existing information instead of creating a new user? >> Well, user might not be a good example, but we'll stick with it. So if you say, right,
[31:26] I want to make a new user record, and I want to apply the singleton pattern to that, once somebody creates or some part of your system creates the first user record, if they try
[31:38] and create another, it's going to say, no, here's the one we already have. So if you make your first record and it's like, hey, the name is Jan, the password is whatever,
[31:45] my email is this and my ID is that, when they go and try and make another one, it will say, well, here's the one that already exists with the properties that it already has and the
[31:53] values that it already has. >> Okay. No, like it makes sense. I'm just trying to like -- >> So the user record might not be a good
[32:05] example. A really good example might be for singletons, like we said, like a caching class. So when somebody asked for something from the database, they'll say, hey, caching class,
[32:19] do you have this? And the caching class will say, no, I don't, but I'll ask the database for it, and then when the database comes back with that, I'll store it in my memory. So
[32:30] the next time someone asks me for that, I'm not going to go hit the database. I already have it in memory. But then when you're caching class or whatever, you only want one instance
[32:41] of that. Because otherwise, if you have multiple different instances, they have their own internal memory lists, and they don't jog up, they don't mesh together. Whereas you only want
[32:50] one instance that has one really big long memory list, and everything asks the same cache, hey, do you have this thing? >> Okay. That does make sense. So other than
[33:03] -- like I know we have 23 design patterns. Other than the singleton, what's another pretty popular one? >> I have to rack my memory now. Okay. So
[33:15] a really good one -- give me a second here. I have another one here in my notes. So you imagine that you want to make something like a chat room, okay? And a chat room, you would
[33:26] say, well, I have a list of messages, and when I send a message to the chat room, I want everybody to get that. So when you think about it, you say, well, that's a really good
[33:37] example of, say, the observer pattern. Because what can happen is you can publish a message to the chat room, whatever the chat room is, and then everybody that's subscribed to the
[33:51] chat room gets that message on their phone. And that's just like a -- generally when you look at publish and subscribe kind of things, you think, okay, the observer pattern is just
[34:00] the normal way that's done. >> Okay. And that makes sense. Real quick, Bakari did mention a good example of a -- is a listed favorite websites that are cached.
[34:15] Just to go back to the singleton one, I believe. >> Yeah, that's a really good example. >> And I just Googled it also to look at -- so you said that there's three different types,
[34:30] and it's credential, structural, and behavioral, right? >> That's correct, yeah. >> Okay. I'm going to copy and paste this
[34:36] into the notes as well. Because I think it's -- like, yes, you may not run into them very often. Like, you know, we're talking about singleton. But at the same time, just reading
[34:49] through it and knowing what they are, I feel like would be really, really helpful. And I'll share this on the screen. >> But even if, like, you go to Wikipedia,
[34:59] nice Wikipedia articles about this, and they actually talk about for each pattern, the typical use cases. So as you said, even if you have, like, a vague idea they exist, and
[35:09] then, like, as you go through, you're writing a problem, you're like, man, I'd really love to know how to write a chat room or whatever, right?
[35:16] You'll come across people online will describe, like, hey, the observer pattern is the best way to do this. You don't have to, like, magically know this from nothing. You'll just -- you'll
[35:24] see it over time. You'll develop your own heuristics as you're solving problems. Like, this sounds like it would be a really good way to use the observer pattern or to use
[35:32] a singleton. >> Yeah. And this is pretty cool that it has design pattern. I'm not -- this goes through types and things, as you said, with wiki.
[35:43] And then going to the one I clicked down here, through cs.lmu.edu, I like that it also shows, like, why study them, common themes. So there's definitely -- but this is really helpful to
[36:01] know that this exists. As you said, to, like, know what to Google. That's what I run into is I'm, like, I know this is a thing. I have no idea what it's called. So therefore it
[36:16] makes it really hard to Google. And I've had it from people I've worked with, my partner, he makes fun of me all the time. Because I have to ask someone, how do you Google this?
[36:26] I'm not the best Googler. That is something I have yet to master. But knowing key terms does really help that. >> This goes back to our first rudiment. Googling
[36:35] is the main skill you learn. >> I totally -- honestly, it's more of, like, knowing the terms to Google. Like, if I was looking at -- to think of something that keeps
[36:46] showing up again and again in code, I may not think of the word "pattern," for example. So that's where I really struggle with it. But I feel like I'm slowly getting better.
[36:58] >> You will. It's just -- it's a long journey. >> Yeah. Or I spend way too much time on Google. That too. Awesome. >> There was a thing about link that talked
[37:08] about, like, why you should learn design patterns. I mean, there's some really interesting reasons about that. I'll blunder through some of them now. Probably the one most important is that
[37:17] the code you're writing follows expected patterns and expected behaviors. There's a lot of developers out there who just kind of, like, they get an inkling of what they want. They DIY a pattern.
[37:29] And that's not to say that what you're doing isn't great and they're not talented people. But maybe they haven't thought about all the side effects. Maybe the way they're doing
[37:37] it isn't mature or battle tested. There's a reason why these 27 patterns are so ubiquitous throughout the software design world. Because they're mature. They're well used. There's
[37:48] multiple examples of them. People have pointed out the flaws, discovered the flaws and pointed them out and fixed them and all the rest. So, I mean, as you go through writing code,
[37:58] you know, you kind of say, like, okay, well, this is the normal way this is done. If you enter a new codebase, say you change your job and you're seeing new codebases, you will
[38:05] expect to see the same kinds of patterns pop up again and again and again. You wouldn't expect to see crazy ideas that people put together. So, it just helps to keep things
[38:16] consistent. It helps to keep things in an expected way for you that you know what to expect. And then for other people when they're looking at their code, because obviously software
[38:24] development is a team exercise, that they know what to expect. And they kind of have, you know, okay, we talked about publishing and subscribing earlier. The observer pattern.
[38:33] You wouldn't try and do some other crazy bullshit. You just use the observer pattern. >> Yeah, I think that's really cool about also teaching to not reinvent the wheel. Because
[38:47] that saves a lot of time. Although sometimes there's stubborn people like me that I've in other parts of life, I'm like, but I can do it this way. Even though my stubbornness
[39:00] leads to learn, it could be easier just using something that exists. >> Yes and no. Failure is a very important part of life. That's how we learn. And I think
[39:13] you have to get things wrong a lot of times in order to really understand the right solution. So, people should go off and have coding adventures and make all sorts of cool bullshit. Maybe
[39:24] they'll discover a new design pattern. Who knows? But as you go and do these things, and then maybe you have someone who's more advanced than you or more experienced or whatever,
[39:33] they can review your work. And they'll say, hey, actually, you've written a lot of stuff here and instead you could do a different solution. That's maybe 10 lines long. You're
[39:41] going to remember that more because it's based on a failure and a correction to a solution rather than if you just say, right, I'm going to read every single software development
[39:50] book out there and now I know everything. So, it's like as you're going through and you make mistakes and you learn and progress, people are going to correct you. You'll correct
[39:59] yourself over time. You'll go back to previous projects you had and you'll say, damn, I can't believe I wrote that. I do this all the time. I look at things and I'm like, what fucking
[40:07] idiot wrote this? And then it's like, my name's on it. It's like, okay. But, you know, you learn over time. You progress. And true failures, you have better successes later on.
[40:18] >> Very cool. Thank you. And I agree. And we do have a pretty cool comment that we're learning good principles. Learning the fundamentals in any profession are essential. Lots of good
[40:30] info here. And I don't have your name. So, you're currently a LinkedIn user. But thank you for the comment. I think it's so true. Because even to up until this part, I mean,
[40:43] I've only been in this world of really working on learning coding, becoming a dev role. I had no idea this stuff existed. Even when I started learning about like APIs when I
[40:53] was in Stoplight. Like, I didn't realize how much there was behind it to think about the big picture stuff when there's like Ian from Postman. He used to be an instructor and helped
[41:11] with code camps. And he talked about how I really want to think about theory things. And then I really want to think about like for scaling APIs. And he's like, not necessarily
[41:22] something you need to think about yet. And so, it's a lot of like learning what is good to learn this early on and what isn't. And that is a fun piece of failure. And also learning
[41:36] from so many different people. So, thank you, again, LinkedIn loser. I just said LinkedIn loser. Oh, my goodness. I cannot talk. LinkedIn user.
[41:47] I looked on LinkedIn and I believe it's Julie J. Oh.
[41:50] It's my mom. Okay.
[41:53] Thanks, mom. You're not a LinkedIn loser. If it's really not, it's probably my mom. But that's so weird because it normally does shows us who it is. Dang it. But all right. So,
[42:13] that is something Bakari says, hi, mom, too. And Bakari, you used to be an instructional and do code camps, too. So, what do you do you teach these type of things in code camps
[42:29] for more of this theory or design base, you know, behind the scenes to create the logic behind it? Let's see a few replies.
[42:42] Yeah. While you're working that, I guess, from my own experience, I don't expect people who had maybe just fresh graduates or fresh from boot camp, maybe they don't know this
[42:51] stuff offhand. And then, like, when they get to, like, two, three, four, or five years experience, they kind of get if they're going towards more pure software engineering kind
[42:59] of stuff, right, more hardcore, they would start to get more into this kind of thing around the four or five mark. They would have, like, their favorite patterns. They'd know
[43:08] the ones they'd use all the time. And they'd be aware of the other ones existing. Whether they know the implementation is another thing. But that's always something you can Google,
[43:16] right? Yeah. I like that. And Bakari just said yes and no. He thinks code camps need to focus
[43:24] more on the fundamentals before building full stack apps. And I think that's a good call because something that I've really thought about on being able to do when there's a lot
[43:38] more of these videos out there are putting them in playlists of, hey, if you want to use learn JavaScript, here's where might be a really good a place for you to start. And
[43:51] these fundamentals, honestly, I didn't even realize they existed, as I said. So it's like, this is so helpful to start digging into. And Bakari, just as a heads up, I told Ian
[44:03] the same thing. I'm totally hitting you up on going through this, too. And then, Philip, I'm going to dig into these fundamentals even more now. So are we missing any of the fundamentals
[44:19] that you wanted to go through? The last one I wanted to talk about a little bit was kind of building above that a level
[44:24] again, which is an architectural patterns. And these are kind of the patterns you would expect full applications or full services to follow. And the reason why we do this is,
[44:34] again, it's because you would have code in places where it's expected to be, where anybody can come along and say, well, I know why that's there, or I know where that is. I can jump
[44:43] in and do that. And I'll talk a little about, I do an awful lot of backend engineering and awful lot of REST APIs. So something we use a lot is the end tier architecture pattern.
[44:51] You might hear it called the tree tier pattern, the layer pattern, but that's basically what it is. And the idea is that you would divide your system up into separate layers that would
[45:01] have their own responsibilities. And the classes would then kind of loosely follow that responsibility. So if you think of a REST API, you typically have three layers. Your first is your top
[45:12] level layer where people talk to the API, your presentation layer. And that has a particular set of responsibilities we'll jump into in a second. You might then have a business logic
[45:21] layer under that. So that's the meat on the bones of exactly what your service does. And then underneath that, you might have like a data access layer. And that's maybe for
[45:30] getting stuff from the database and saving stuff to the database. And when you think about that loosely, it makes an awful lot of sense because if you then, you know, you
[45:40] join a new company and then you're given a bug to fix and someone says, well, you need to fix something related to a particular data model record. It's pretty, you know, obvious
[45:50] to say, well, that's in the data access layer. I know where that is. There's an expected pattern that's used here. I know where to jump in and get a start and do something.
[45:58] The same when you're like maybe expanding upon your code or you're modifying the existing platform, knowing the different layers you have and the different responsibilities they
[46:06] have, you would easily know then where I'm going to put this new code that does this new thing. Or for a new feature that happens, you'd break it into these smaller subtasks
[46:15] like we said before, and you'd pop them into different places. And each layer kind of dips down into the next layer. So your top layer talks to your business logic, which talks
[46:24] to your data access, which sends the results all the way back up. So it's a nice kind of clear expected pattern. And it's just kind of become an industry standard, right?
[46:36] Where my thought process is going right now is that, like, first off, I need to understand APIs better. That is just, you know, some, I feel like I'm stuck on that currently because
[46:49] I started in at Stoplight, and they're an API design for a spec company, and I'm like, I really just want to understand APIs because that's where I started. But I'm curious, is
[47:04] it possible to, because I've built an API with Ramon, and I know that we used ExpressJS, and I think where I'm starting to really get a bit lost is how to create, like, the difference
[47:24] between like REST and SOAP APIs, and then how these work, like, based in building an API, if that makes sense. Like, this kind of makes sense where I'm like, okay, like,
[47:36] code as a singular, like, doing it on my computer with VS Code and localhost, cool, like, that's making sense, but doing stuff as, like, open source, or creating a REST API, which you
[47:50] need to make documentation for, so other people can use your API, and I'm like, that is not, I know they go together. I know they do. I just don't know how you go from A to B. So
[48:02] as you're, like, explaining a lot of this stuff, I was like, how do you go from A to B? And I think that's something that I'm going to ask you back on the show for, to see what
[48:15] you want to explain, and if we could go through some of these, and Bakari was on the show yesterday, and will be on again tomorrow, which I'm pretty excited about, because it's,
[48:27] there's so much that goes into all of this, and I know that I keep saying that I need to code by myself, but with so many of these episodes a week, it's really cool, because
[48:37] it is repetition. - Repetition is one of the best ways to learn. If you want to do another session of REST
[48:43] APIs, I'm happy to do that. - That would be cool.
[48:45] - We can go through it a bit more in detail, because there's two parts to that, right? There's the whole concept of REST, and then obviously there's the actual implementation, where if
[48:53] you said you've used Express and stuff before, I usually use, like, csharpen.net, but, I mean, like, if you understand the concept of REST, you're really just fulfilling that
[49:01] concept through your implementation. We can think about that another time. - Yes. This is the cool thing, is that, since these are so complex, that we are creating
[49:12] so many, like, part one, part two, or going down, like, certain rabbit holes with a specific guest, because something that so many people have asked me, being a newbie, is, like, well,
[49:24] where do you want to go in this, like, what do you want to do? And I'm like, I don't know. I don't know what's out there. I don't know if I want to do, specifically, APIs. Like,
[49:36] I applied for a company that does API management, and I'm like, cool, if I work there, like, I'm going to learn more about that, because I work there, and I'm going to support it,
[49:46] because if it's helping people, I'm happy. And that's why I'm like, I don't know. I'm currently learning JavaScript. I have someone coming on the show next month in August about
[49:58] Python and starting to look into that. I got really curious about Kafka and what that is. And one day, I will ask more about Kubernetes and Docker and that kind of stuff. So, so
[50:12] many different rabbit holes to go down, and how they all intermingle. A lot of the things you've mentioned, like, you could spend your whole career focusing
[50:21] on a single one of them, and having a very lucrative career doing quite well. What I would say is, like, what a lot of juniors don't do, and maybe they should, is get your
[50:32] feet wet with everything. Try as much as you can. Write projects in Python, follow tutorials, write projects in JavaScript, follow tutorials. And then as you go through, you'll get a feeling
[50:42] for the things you like to do. And it takes a long while to get a sense of that. A really good example is that, for me, I've been doing this for, like, 12 years now. I was a full
[50:51] stack developer for 11 of those years, and I transitioned to being just backend within the last year. And it took me a long while to find that that's actually what I love doing,
[51:01] that's what I prefer to do, that's what I want to do. But it takes you time to develop that you have to try a lot of things, and then say, right, I don't like this, I don't
[51:09] like that, and that scares the shit out of me, I don't want to even look at that. And then over time, you develop this thing of, like, okay, these are the things I enjoy doing.
[51:16] This is the rabbit hole I'm going to launch myself into. Yeah, yeah, I really like that. And we will definitely get you scheduled back on the show.
[51:26] And I did bring up LinkedIn, because you just said it was Julie J. And I looked it up. It's my mom. It is totally my mom. She is like my number one supporter. It's it's so fun.
[51:38] But yes, so much goodness here. And I'll be putting time codes and resources in the YouTube link. And is there anything that we missed that you're like, we need to talk about today
[51:51] before we end today's show? Not so much missed, but something I'd like to reiterate that like, you can go through
[51:58] all of this stuff and have a very long, happy career without knowing any of it. Without knowing these exact concepts, the deal about software is software that you deliver and
[52:07] works and makes money and users can use is the best software. People might judge you for the quality of your software. And maybe there's a good reason for that they might
[52:15] judge you for the way that it's put together. But I mean, ultimately, it's delivered code that makes money is the best code, right? So I mean, like, if you don't know these things,
[52:22] no matter where you are in your career, you can pick them up over time, you can ignore them. But I think if you if you are interested in it, and you do start googling and start
[52:31] learning and you'll find different books and videos and Udemy courses and all sorts for it, whatever floats your boat, you do take a bit of an interest in it. Over time, you'll
[52:40] start to see yourself improve an awful lot. And between like reading code and writing code and finding mentors and getting that feedback loop going, you'll see yourself progress.
[52:50] So it's just take on the things you want to take on, ignore the things that you're not really interested in. As long as you're kind of keep moving and keep going. Like that's
[52:58] all good. Right? Yes, yes. And thank you for reiterating that. I think it is definitely something that I love how it might have even been before we started streaming. We talked
[53:10] about that we all learn so differently. Some people it's you know, going to the books documentation. This is something that I don't think Anthony's here today. You know, joining joined us today,
[53:22] but he always is like, Jen, you have to read the documentation. Do the readme. So I have a couple people coming on. So Anthony is one of them. And then another person coming on
[53:36] to talk about documentation, not only why it's important, but then also how to create good documentation. And it's it's definitely something that we documentation is not always
[53:51] where my mind goes. But it's really cool how with meeting people in this industry, how even though documentation is the way a lot of people read and what products need, that
[54:05] even though I'm dyslexic, I can there's much more screen readers that can tell me what's going on. And I can understand it and check my code. And I mean, a lot more coders that
[54:15] are dyslexic or are ADHD. And it's just really cool being able to see, yes, how many of these overlap and how many really once we learn what we're interested in or the way we learn
[54:28] or how to get around something, if we are neurodiverse, that there are topics and things out there. That's why I started on Wednesdays, we do a Twitter space about neurodivergency
[54:41] because I feel like so many people don't know how to function, especially in the tech world when it's not always as clear, I think is the best way to say it.
[54:56] Yeah, that's fair. I think a lot of people who write software are drawn to the aspect of logic and order and purity and all these great concepts within software. But those
[55:05] are like diametrically opposed to, like, say, people skills. You talk about writing documentation and stuff like that. People who are really good at writing code are often really poor
[55:14] at writing documentation because they're two totally different skills. And like with a lot of things, you just have to practice and practice and practice and practice and develop
[55:22] that skill over time to get it over. But yeah, people learn in different ways, try things in different ways. It's just the voyage of discovery to find what works for you, right?
[55:33] Yes, yes. And writing anything is not awesome for me. But if you want me to live stream something, create video, be a hype person, go to events and talk to everyone, and network,
[55:46] I'm your girl. And that's what I've been trying to explain as I've been going for dev role roles. They're like, you don't know how to write a plugin. I'm like, I can learn. But
[55:57] here's all my other skills that will benefit you. So it's definitely a lesson learned. And thank you again, Philip, for joining us today. And we look forward to having you on
[56:07] the show again. Yeah, looking forward to it. Bye. 
