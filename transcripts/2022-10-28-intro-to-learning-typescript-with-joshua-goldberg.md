---
showLink: "https://www.youtube.com/watch?v=wROPI2E5u5c"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "intro-to-learning-typescript-with-joshua-goldberg"
title: "Intro to Learning TypeScript with Joshua Goldberg"
publishDate: "2022-10-28"
coverImage: "https://i.ytimg.com/vi/wROPI2E5u5c/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:05] Yet, day one of a new series that we are doing with Josh. Josh, who are you?
[00:13] What do you do? What series are we doing? >> Great questions. Hi, everyone.
[00:17] I'm Josh Goldberg. I am a TypeScript person.
[00:21] I'm not on the team, but I authored and through O'Reilly released a learning TypeScript book.
[00:27] I'm also a maintainer on TypeScript ESLint, which is the tooling that lets you run ESLint on TypeScript code.
[00:32] The series we're going to be going through is Teach Gen Tech,
[00:36] the learning TypeScript edition, where we'll go through the learning TypeScript book.
[00:39] Gen will explore TypeScript and all its fun and quirks, and we're going to have a great time,
[00:45] and I hope you all will too. >> Yay. Yes.
[00:50] For everyone tuning in or watching this post, today is just setting up.
[00:57] What are we talking about? How can you follow along?
[01:00] Because this is definitely for all of us to be a part of, not just me getting value out of it,
[01:05] but also how to go through the book. I grabbed the book today,
[01:09] and I've started going through it and everything, and I'm like, how did I already make it messy?
[01:14] I don't even know. It's not shiny and new anymore is basically what I'm saying.
[01:20] I'm like, I've used it. For those who have been following my journey,
[01:27] I'm very excited because I've been working on this Tweety tag app thing in Prisma,
[01:35] and they use TypeScript, and it's been a lot of Googling,
[01:41] which I feel like is my entire coding experience, but I'm excited for this. Thank you.
[01:48] What up, homie? It's one of my favorite things to say when homie joins the streams.
[01:54] >> One of my faves as well. >> Yay.
[01:57] >> Hi. >> Yes. I listened to,
[02:01] is it called preface or preface? Which is a proper way?
[02:05] >> You brought this up pre-stream. I was wondering, I truly don't know.
[02:09] My guess, and this is not informed, is that to preface is a word and the preface is also a noun,
[02:16] but I've heard that you could preface something and I don't know.
[02:18] It's a great question. >> All right. Maybe I'll Google this later.
[02:22] I realized without thinking about it, getting ready for the stream today,
[02:26] that I'm just going to blend in with my background. It's okay. There's just going to be floating hands.
[02:30] It's Halloween. It'll be great. I really liked it because it set up a why you got into it,
[02:39] and then also that it's going to be broken down more than having the assumption
[02:46] that people know all about this already. I'm going to see if I recap this well,
[02:53] and you can let me know. I just want to skip forward.
[03:00] Let me think about this. How did you get into this? I'll just ask you and then I can wait and skip forward.
[03:05] >> Sure. How did I get into TypeScript as a whole? Yeah, I really like JavaScript.
[03:12] I actually learned first Java in high school and then C++ in college. I was a four-year CS degree.
[03:19] Those languages are fun, but I really like the speed and rapidness of doing things on the web.
[03:25] I like how you can slap some, in my case, terrible code onto an HTML page,
[03:31] maybe add some CSS or JavaScript, and it just works and you can publish it on a website.
[03:36] My first big project using those fun ideas of just getting it out there, was a remake of Mario called Fullscreen Mario that went viral,
[03:44] got taken down by Nintendo, and was, I'm proud to say,
[03:48] the worst project code I've ever written. It was about a dozen files with hundreds of global variables,
[03:58] all sorts of bugs all over the place. It was terrible. People on the Internet told me, "Hey,
[04:02] you should look into things like ESLint," which is a linter. It looks at your code and complains about it for you.
[04:08] Then later on, I got into TypeScript because TypeScript is like the ultimate linter. It both finds bugs in your code for you
[04:15] and lets you describe how your code is supposed to run, which then in turn tells TypeScript more about your code and makes it easier for
[04:22] you to read your things that you wrote six months ago and have completely forgotten about since.
[04:26] I'd say through pain and tribulations, have I gotten into TypeScript.
[04:31] >> Yes. I love this because it's always like how you explain like, "Hey, what did you write a while ago?"
[04:39] I love this because it's literally on everything. But one of my favorite parts of the preface,
[04:47] we'll go with that for now, is you were like, "Nah,
[04:52] I don't like JavaScript." Then you did your project and you were like, "Yes, this is amazing."
[04:57] I loved that. My other favorite part and this is something that I feel like,
[05:05] especially with Teach Gen Tech, I have gone from knowing like people just throw projects at me, which I love.
[05:13] This is how I learned, this is why I learned it this way,
[05:16] this is why Teach Gen Tech is the thing. I do not do very well going through step-by-step normally,
[05:23] but it's also really, really useful to go step-by-step.
[05:28] There's a reason. There's a reason, y'all. The reason that I'm looking for.
[05:36] Yes, y'all, we will be having a information on how you can get yourself a book so you can take notes and things.
[05:45] Because I only listen to it, I use an app called Natural Reader to be able to take pictures or read books.
[05:54] I use that, but now I have my pen. I really like that TypeScript is four things;
[06:02] programming language, type checker, compiler, and language service.
[06:08] I was like, I didn't know what a compiler was. I've heard people explain it,
[06:14] but I was like, a program that runs the type checker reports
[06:19] any issues and then outputs equivalent JavaScript code. I was like, "What?"
[06:25] I was mind-blown that it was actually written out. That's a big thing that I'm really enjoying about just barely getting into the book.
[06:36] First off, hi, Ben. >> Hi, Ben.
[06:40] >> Yay. As we're going through this book, we can definitely go through the examples of chapter-by-chapter because y'all,
[06:51] I'm not going to lie, actually, it's really helpful because it's like you put the index in the chapter,
[06:58] instead of people having to go to the back and look at the index of everything. I'm totally just going to awkwardly show.
[07:07] It's like, "Hey, this is chapter 1. This is what you'll learn in it."
[07:11] >> O'Reilly actually has some pretty nifty automations. That's all automatically generated from the headings.
[07:17] >> What? Y'all, I'm showing you more because I get really excited about this because I'm like,
[07:24] it organized the way my brain wanted to look at things instead of what I struggle with with most books.
[07:31] If you're telling someone about TypeScript for the first time, do they need to know JavaScript beforehand?
[07:44] >> That is a debate in the TypeScript community. There are some people who've had some successes
[07:51] teaching just TypeScript to someone who doesn't know JavaScript. I personally, I'm in the camp that it is often and
[07:57] perhaps a majority of the time preferable that they know JavaScript first. I'll tell you what, I'm a really big proponent
[08:06] of the learn one major thing at a time strategy. The idea that it's not easy to learn a bajillion things at once.
[08:13] A lot of people when they start learning, say, programming, they learn HTML, CSS, and JavaScript all at the same time.
[08:21] They have to learn three things, the concept of the markup language,
[08:23] styling those things, JavaScript, which is like a whole shebang and I really don't like that.
[08:28] I think the brain works best when it can contextualize a solid single area of new knowledge against what it already knows.
[08:35] If it needs to make new core knowledge, core memories, then it can do so in an individual way for them.
[08:43] I really like teaching the concept of type theory, what is a type annotation,
[08:48] a type checker, those four things you were looking at, on top of already knowing the core fundamentals of JavaScript.
[08:54] Can you imagine teaching someone both the more difficult parts of TypeScript, the less easy ones, at the same time that they're learning
[09:01] about scoping in JavaScript or this? Those are both things that you really want to focus on.
[09:08] >> That does make sense and I'm curious about it because I feel like that's how it is for a lot of people yet at the same time.
[09:17] Y'all, I'm doing the opposite of what Josh suggest. >> You're just doing it all at once.
[09:23] >> Yeah. In the fact that I'm learning Python on Mondays, we have learning with Laura on Mondays,
[09:30] which I absolutely love. But that's how, and I've learned this about myself is,
[09:36] I am very ADHD. If I don't have different buckets going at the same time,
[09:41] I'll disengage with something. I'll be like, "Yeah, no, I'm done with that."
[09:46] Where I will say comparing different languages has helped learn more about JavaScript.
[09:55] While I've been learning Python, I've learned a ton more about JavaScript.
[09:58] While I'm building things, I learned more about how I would do something in Python compared to
[10:03] JavaScript and why each is good or bad, the pros and cons of them.
[10:11] I say that in the fact of y'all just for all the beautiful humans that are watching through this process
[10:18] is learning how you learn best. That is a difficult process yet it's also like getting into coding.
[10:31] Yes, you are Ben. Ben just said. >> That's right.
[10:37] >> It's Ben. I'm a beautiful human. Yes, you are.
[10:41] It's a lot of just getting used to and finding things of ways of learning. I am not a learn by the book person.
[10:52] I wish I was. But if I don't have someone that can say,
[10:57] "Hey, Josh, how does this compare to Python on XYZ?" It was actually harder for me to comprehend not knowing any of it from zero,
[11:10] then being able to compare it to something, which is the point that you had of at the very beginning,
[11:15] having a solid understanding of something to be able to compare it to. It's all different ways that we do things,
[11:23] but today is all TypeScript. >> I really like the idea by the way of jumping between things,
[11:31] say doing TypeScript on a Friday and Python on a Monday. I'm perhaps slightly less ADHD, who knows.
[11:37] But for me, my thing is, I can focus really intently on a short period of time on one thing,
[11:44] and then I move on to something else. I really like learning one thing intently in that short time,
[11:49] because if I have to learn four things or whatever, then it takes one, I get distracted.
[11:55] But yeah, strong plus one that the understanding of how each person learns that that person gains over time is both incredibly difficult to
[12:04] gain quickly and also super valuable as you get it. I'm glad you learned about yourself. It's good.
[12:10] >> Yeah. Teach Gen Tech has really, first off, it sounds weird when I say my name in it,
[12:16] but I really associate it separately. Homie says that they agree with your perspective.
[12:24] They like how you explain teaching Type Theory as opposed to biting it off as a whole TypeScript.
[12:31] The question is, where's your course? >> I wish I had the time to make one.
[12:36] First of all, thank you, Homie Coder. Always good to see you again. Second of all,
[12:40] I would love to make a course the way like Shonday Person or Matt Pocock have, both of which, by the way, I would recommend as
[12:45] course instructors if that's what you're looking for, both of whom. But yeah, I'm trying to do this open source thing and promote the book,
[12:53] and family stuff, and friends stuff, and there are too many things in this world to do.
[12:58] Maybe eventually, but not this year. >> To that point, that's a big reason that we're doing this,
[13:04] is to flush out to be able to help make the course later. Because since we're going through all this stuff,
[13:12] it's going to be recorded for him to use. You can literally use it whenever you want
[13:17] and also see what other people are struggling with. We're here for questions.
[13:24] It's something that is making it a, I don't want to say more.
[13:29] I'm missing words, but I'm going with accessible. Because since not everybody learns from the book,
[13:36] but we would all love Josh's knowledge and Josh loves to teach. That's why we're doing this. Also, thanks to Ben.
[13:47] It's weird that it's Ben and Ben in our chat and I'm totally digging it. But Ben Myers for introducing us.
[13:54] >> Yeah, that's right. Oh my God, thanks for reminding. I forgot it was Ben.
[13:59] Ben is great though. Y'all should subscribe to Ben's stream. >> Yes, exactly.
[14:05] Yes, homie, you do need to get this book. Homie and I are working on a project and we're going to be using TypeScript.
[14:16] I'm nervous, but we'll figure it out. It'll be great. Lots to learn there.
[14:24] If you were to break down the way the book works, how would you say overall what the book looks like and then how we break it down?
[14:34] >> Sure. There are three sections of the book. The first section is the most important,
[14:40] I think, to answer that question. The third section is fun miscellaneous stuff that's useful,
[14:45] but you would not need to know to truly understand, or to say that you know TypeScript.
[14:49] The second section of the book is how TypeScript works with each of the features of JavaScript that you would commonly use,
[14:56] functions, arrays, classes, etc. But the first section is where the real teaching, I think, happens,
[15:02] the core fundamental foundational stuff. That's split into, first,
[15:08] I explain in the book what TypeScript is, those four things you mentioned.
[15:12] It is a compiler which takes TypeScript syntax and outputs the equivalent JavaScript syntax, text-to-text.
[15:19] It is a, well, I guess we'll get into that later.
[15:22] Then I go over some of the syntax that TypeScript adds to JavaScript, like these little type annotations which help inform it.
[15:32] I think actually before that and then also after that, I explain how TypeScript reasons about your JavaScript,
[15:37] how the type checker, the thing that looks at your code and understands it,
[15:41] takes a look at variables, the way that they're assigned,
[15:45] the way that they're changed, and lets you know when, say,
[15:48] you assign a string somewhere that's supposed to be a number or some other mistake. Does that answer the question you're looking for?
[15:55] >> It does. Then I do want to share this to share screen and go to this screen.
[16:04] Yay. This is also something really cool. This is the website. It is linked in the YouTube video and everything.
[16:14] I will go copy and paste that here in a second with everything from today. It's also something that each of these chapter,
[16:24] I think it's by chapter or is it by section that we're going to have projects to go through?
[16:28] It's by chapter, right? >> Yes. Each chapter has a corresponding group of projects.
[16:33] >> Yeah. It's going to be at learningtypescript.com. This is pretty exciting because this is what we went
[16:43] through earlier on when Josh joined us a while ago. This is what happens as people join and then they're like,
[16:51] "Hey, I want to come back. That was fun." We ran this and then we ended up talking about it a lot more to see if I understood it.
[17:02] At the moment, I totally don't remember what we did. I remember that it was really cool because I was like,
[17:09] "Oh, this is a way to con. I'm getting theory and I'm getting practice."
[17:14] Where that's something that I really struggle with. If somebody is talking theory,
[17:18] then I'm like, "Okay, yeah, no." I'm very excited that we will be going through these as well.
[17:29] By we, I mean me and the audience and show Josh. If we finally got it and ask him questions.
[17:39] >> I'm here to help. I'm very excited about this. >> Definitely check out this website and get the book.
[17:45] We will be sharing ways to get the book too probably by the next time we stream. It is, we are going to stream every other Friday.
[17:59] This is, I will have a calendar out eventually. It will be a thing. It will be.
[18:06] I'm not sure when, but it will be. Is there things like, of course,
[18:10] like we can get the book, we can read through the book or we can watch your live streams.
[18:16] We can also watch your YouTube or are there things that we should do outside of that to prep for going through this course with you?
[18:26] >> Good question. I would say my live streams might not be great prep material. I live stream my work in open source,
[18:34] but it's a lot of stuff that deals with TypeScript static analysis, which is not great if you don't know TypeScript yet.
[18:43] It's great if you just want background coding or if you're interested in that stuff once you've read the book.
[18:48] I'd say it never hurts to read ahead or to take another course. I personally find that it often takes me two to three different things,
[18:58] whether that thing is a video or a Codecademy tutorial or projects to understand something.
[19:05] I'd say try reading ahead. Also, definitely, it's useful to recap your JavaScript fundamentals.
[19:12] Knowing how functions work in JavaScript, like first-class functions, storing them as variables.
[19:18] Classes, once we get to them, although I don't personally use those a lot in JavaScript,
[19:22] some hard architecture opinions over there. >> I'm just going to say, classes and I just have not clicked.
[19:31] I stopped taking a LinkedIn course because a lot of courses you have to finish X to be able to continue.
[19:38] I'm still stuck on classes. I'm like, I don't know why I'm so stuck on them.
[19:44] But it's not computing. As a heads up, that might be something I struggle with when we go through that.
[19:52] >> Well, the classes chapter was one of the more difficult ones to write. I'd say if you don't understand it,
[19:59] classes and types you're finding in a bit, that's totally fine because if you don't use classes,
[20:03] it won't affect you at all, so yay. >> Yes, yay.
[20:08] Cool. We can also tag those different things later on. I can put it in the YouTube video notes.
[20:16] Yes, Ben. Well, yes and no. He said that accessibility appearances have been very theory so far.
[20:30] I'm like, I don't know, Ben. Let's see, the first one we actually were going through
[20:38] and actually looked at colors and you showed me the contrast thing. That one wasn't very theory.
[20:47] Trying to remember the second one. I think I'm mixing it up with the first one too.
[20:52] But this is why they are recorded, because we might get messed up on them.
[20:59] Yeah, today was honestly just to get us set up and go through this. Do you think we should start with chapter 1 today or do you think we
[21:10] should wait till everybody gets their time to get their books and set up on start on next time?
[21:16] >> I'm down to wait. If anyone has any particular questions they want to ask about TypeScript or
[21:23] personal anecdotes about when it or JavaScript has given them great joy or pain, would love to hear it. But yeah,
[21:30] I defer to you and the audience. >> My dog is trying to talk to us.
[21:38] I don't know if she's like for continuing or for waiting, but she is, how fun is that?
[21:49] Sorry, Ryan and Homie have been setting up stream elements. That is actually really cool.
[22:01] Can you do the, for Josh's? Do you go by Josh or Joshua?
[22:08] I feel like it's been, I keep going between the two. >> It's Josh. I put Joshua K Goldberg
[22:14] because it's the only one that's been consistently available, but I really wish I'd been born
[22:19] a couple of years earlier and gotten Josh Goldberg everywhere. There's actually a verified Joshua Goldberg on Twitter
[22:25] who is not into tech and it's been real annoying. Also, there was a terrorist Josh Goldberg down in Florida,
[22:31] but he hasn't been on the news in a while, so I've beaten him in the yes or no game.
[22:35] Take that, Joshua Ryan Goldberg. >> That is funny. Ben did say they built
[22:45] a JavaScript bot for D&D resources a while ago. They also rebuilt in TypeScript and dang,
[22:54] it feels so much nicer to work in. >> Yay. Ben, where is this D&D resources?
[23:09] I feel like I need that in my life because later tonight, I will be playing D&D.
[23:14] I'm pretty hilarious at trying to use my character, especially when it comes to knowing what I
[23:23] can make damage with when it's my turn. It's awkward. In case anybody wants to stream on that one,
[23:31] it is on Jacob's stream. But really quick, sorry,
[23:43] I'm trying to multitask and I'm putting this in here of ways to connect with Josh and learning TypeScript.
[23:51] I just want to make sure I had it. Awesome. Well, then we will pause until next time.
[23:57] Today's was a quick stream just to set us up so everybody knew what was going on,
[24:01] what the plan is, and get excited for it because I'm excited.
[24:06] Goodbye, everyone. Hit us up when you want to learn more beforehand and we will be
[24:14] promoting it a lot more as coming up. See you in two weeks.
[24:19] Bye, everyone. Thanks for coming. 
