---
showLink: "https://www.youtube.com/watch?v=2XGpHFmgrAQ"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-2-the-type-system"
title: "Learning TypeScript Chapter 2: The Type System"
publishDate: "2023-02-03"
coverImage: "https://i.ytimg.com/vi/2XGpHFmgrAQ/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech,
[00:07] and we are currently working on, I feel like I always need to do this when I talk about it,
[00:13] of learning TypeScript with Josh. >> Hi.
[00:18] >> It's very exciting and I have, that was confusing. I was going in Inception mode,
[00:25] I had YouTube up just in case I needed something there and I was like, I'm hearing myself talk, this is really weird.
[00:32] It is very weird and very distracting. Yet, hello.
[00:38] For those who are new to joining us, welcome, welcome. Josh wrote a really cool book that I was trying to show you of learning TypeScript.
[00:49] What? I feel like I almost want to ask at the very beginning of every time we meet of how would you describe TypeScript?
[01:01] >> The answer is going to change every time as I learn and grow like a human. I'd say TypeScript is a superset of JavaScript,
[01:10] meaning that's the technical term. The human term is TypeScript is like JavaScript,
[01:15] but it adds a lot of really useful features that let you describe what your code is supposed to do,
[01:20] which means it can both help you write code and also let you know when you're messing up.
[01:26] >> I like it. You just reminded me that at some point, I want to write a blog or do a video of what is a meta-framework,
[01:41] a framework, a superset, and then a compiler because all of those terms,
[01:47] I'm still like, okay, cool. I mostly know what I'm doing,
[01:51] like talking about, but at the same time, I'm like, yeah, no, I got to look all of this up.
[01:56] >> Let's add transpilers, linters, formatters, language services.
[02:00] There's just a bajillion terms that people throw around, and they all have reasonable meanings.
[02:04] It's not like any real rocket science, but on their own, you got to learn them,
[02:09] you got to understand where they come from. You have to do that three or four more times until it really sinks in,
[02:14] if you're me or many people. It's just stuff to learn.
[02:17] >> That is a great call-out too. The way I understand linter is it's something that will tell you,
[02:26] it's prettier in VS Code in the fact that it tells you if you have something that's incorrect or not a specific format that is a defined rule.
[02:38] Would TypeScript be a linter? >> You've activated my trap card, as they say.
[02:44] There are three tools that roughly fit into the description you said, and you are right. They look at
[02:52] your code and they let you know if something is wrong, and they all blends together.
[02:56] A formatter is the simplest of them. A formatter just looks at the stuff that doesn't change the meaning of your code,
[03:02] white space, tab spaces, end lines, semicolons. All that stuff should not change how your code runs,
[03:08] and a formatter just helps you write the code that's pretty and consistent. Hence the name prettier. In VS Code,
[03:15] a lot of people do what I do, which is they make it so that prettier runs on
[03:19] save whenever I hit "Save" it formats the file, and if I hit "Save" and the file doesn't format,
[03:22] I know I've messed up my syntax somewhere, which is actually really useful when you're learning a language.
[03:27] >> Yeah. >> The next step is linters.
[03:31] Linters operate with a large set of rules. Things like don't have an unused variable,
[03:36] don't name things in all caps or whatever. You can get some pretty advanced lint rules,
[03:41] especially when you have custom things that people write for their own projects. Linters should not work on formatting because the formatters do that.
[03:49] Linters aren't going to do it as well. They're slower, they're more powerful,
[03:52] so they're not as good at the edge cases of formatting. But they are really nice and configurable because in most linters,
[03:59] you can toggle rules on or off, change their severities.
[04:02] A lot of rules have options. You could allow unused variables that match a specific name or whatever.
[04:08] That's linters. I'll pause there because that's a big point of contention and confusion at
[04:13] least to the JavaScript TypeScript community of use prettiness for formatting and eslint for linting and it's a lot of [inaudible]
[04:21] >> I think that's a good call-out of just the examples of what they do, because I totally thought prettier was a linter as well.
[04:33] Ben just joined. Hi, Ben. What do you think?
[04:38] >> [inaudible] >> We're talking about that.
[04:42] I was like, "Okay, so a linter." Oh, my light just fell.
[04:46] That's cool. It can stay there. We're going for a new motif.
[04:52] Is TypeScript a linter? That's where the entire conversation got started here.
[05:01] We have prettier is an example of a formatter. Eslint is an example of a linter which does not
[05:08] actually do formatting such as spacing, but a linter does capitalization or incorrect.
[05:17] Would you say syntax for that one or is that syntax prettier? >> That would be the language.
[05:24] I will note that eslint can do formatting, but it can't do it well.
[05:28] Every linter maintenance team that I've ever seen, including the eslint JavaScript team
[05:34] and the TypeScript eslint team that I'm on, strongly recommends don't use a linter for formatting.
[05:39] Another rule example would be like in TypeScript eslint, we have rules that verify using
[05:46] the right TypeScript or JavaScript syntax for things. We can tell you don't use
[05:50] this specific type of loop over an array because that's unsafe. Use this other type of loop and it will prevent some bugs.
[05:57] But then the third tier then is, yes, the language. The language makes sure that things
[06:03] are correct in both syntax and in TypeScript case typings. If you say a variable is a string and then give it a number,
[06:11] the syntax might be correct, but TypeScript will yell at you saying,
[06:15] "No, you said it's a string, don't give it a number." >> That's a great example of how TypeScript does it compared to,
[06:22] I honestly thought that prettier or eslint actually did that, not that it was TypeScript that did that,
[06:33] to tell it that it's a wrong variable. Is that how I would say it?
[06:39] >> Depends how technically precise you want to get. Someone who worked on the language could probably give you
[06:45] a better answer than me on the very specifics of it. But yeah, that's what I would say.
[06:50] >> I would say, this does bring to all my questions for Chapter 2. Y'all, I'm going to show this really quick,
[07:02] we're going to see if we can show this, of how I end up studying before we do this
[07:08] and where Josh ends up coming in is, let me add to stream.
[07:17] You're not going to be able to read my handwriting because I think it puts it backwards and upside down. Let's try.
[07:25] Yeah, here we go. But I actually take notes in the book and I use
[07:33] a screen reader to read the book to me because I'm dyslexic, but this helps me remember what parts I was getting stuck at.
[07:41] That's currently what we're going to be working on today. If anybody wants to see the notes I'm taking,
[07:49] happy to do photos or show you again, but that's really, really awkward.
[07:55] It is not going to be permanent and let's see. We got a comment on, let's see,
[08:09] Cancer IMAX, is that anywhere close to right on your name? Would it be fair to say that a linter gives you a list of things to fix,
[08:19] but a formatter will actually fix them? >> That's a good question. I'll verbally say what I said in the chat.
[08:26] A formatter will basically always fix it for you and do it very quickly and in a standardized way.
[08:33] A linter allows a list of rules to run. Each rule may produce complaints and each of
[08:39] those complaints may have a fix available. Like in ESLint, there's a really popular plug-in,
[08:45] ESLint plug-in simple import sort that I like, that sorts your imports.
[08:49] It has an auto-fixer that can sort your imports for you. But other things like, hey,
[08:55] you used a function in a place that you should have just made it a class or vice versa.
[08:59] That might be more complex and the rule might not be able to quickly or easily suggest a fix for it.
[09:05] >> Very cool. Thank you. Something else that I do want to shout out that I
[09:12] actually didn't scroll to the beginning of Chapter 2, is I will also bring this up on screen so everyone
[09:21] can see at least what area we're in on the chapter. I'm getting there. Share this screen.
[09:36] We are on Chapter 2, the type system. I would say question number 1,
[09:44] tell me why this chapter, what was your intent to
[09:51] this chapter and why you created it, please. >> Sure. You're very polite. I appreciate you.
[09:59] I will also note that I'm in my brother's house, hence my potato quality camera,
[10:03] and he has two small children, so I am eating granola bites and will soon,
[10:08] all while muted, be enjoying a little bit of unsweetened apple puree.
[10:12] >> Nice. As another side note, it is on your Twitter,
[10:17] so hopefully I'm not crossing the line saying this. If anybody notices that Josh may look up,
[10:24] and there's a really red eyeball, he's okay. Please explain.
[10:30] >> Yeah. Sorry. Thank you for bringing this up. I was going to and I forgot.
[10:34] Content warning, not very much. I had LASIK, which is a now rather standard eye surgery
[10:40] that makes it so you don't need glasses or contacts anymore for the most part.
[10:44] Apparently, until you're in your 40s, I need reading glasses like everyone else,
[10:47] so I've got to look forward to. But the side effect of LASIK,
[10:51] it's pain-free, totally fine. It's just your eyes get red,
[10:53] especially if you have a really strong flinch/blink instincts like I do.
[10:58] If anything goes near my eyes, I'm just all over.
[11:01] Now my eyes look like a vampire or zombie costume, which is great. I have been wearing
[11:08] sunglasses indoors so that people don't look at me and think, "Oh no, I'm now that guy."
[11:13] If you ever see someone wearing sunglasses indoors, they might have just had LASIK two days ago,
[11:17] but pain-free, totally fine. Check out my Twitter for some cool pics.
[11:21] >> We did double-check that Josh is okay to stream today. >> Oh yeah. Jenna was real nice about this.
[11:28] I was like, "Oh, let's do this. I'm so excited." The type system.
[11:33] >> Thank you for that caveat. What is the type system? Why did you make this chapter?
[11:38] Tell us a little bit about it, please. >> Sure. It all started when I tried to learn TypeScript.
[11:45] I think a lot of explanations of TypeScript either assume people already understand what
[11:50] a type system is from another language like C# or C++, or they gloss over the concept of
[11:57] a type system and then jump into more syntax things. But I don't like that because I think if you're
[12:02] going to understand how TypeScript works, you should really understand how TypeScript works.
[12:07] What is it looking for in your code and why does it give the errors that it gets?
[12:11] In this chapter, I cover the foundation of the logic that TypeScript uses to look at your code,
[12:17] understand the code, and then maybe yell at you about the code. The type system refers to the understanding that TypeScript
[12:25] builds up of all the things that exist, variables, functions, etc, and the types that they might be,
[12:31] like string, number, etc. Does that sound good so far?
[12:36] >> Yeah. I don't know why I just decided that I was going to show it on the other screen.
[12:40] But yes. Something that I didn't realize, and this is a great reminder as well for everyone.
[12:48] I am still learning JavaScript. I'm still learning programming languages.
[12:53] I have built my own site. I can figure out a lot of it.
[12:57] But things like what we'll go through later on is like, what do you use null or undefined for?
[13:04] Questions for another time. That being said, if some of the questions I asked seem like they're not TypeScript related,
[13:12] they're JavaScript related, that is why. Also, I had no idea that TypeSystems happened outside of JavaScript.
[13:23] I didn't know that C++ or C# both used it as well. >> Oh, yeah.
[13:28] >> I didn't know that. >> JavaScript is a good one.
[13:30] >> Oh, really? Okay. >> There are three main popular languages out of quite a few,
[13:35] but three main popular ones people use that for the longest time did not have any concept of types or TypeSystem built in.
[13:41] JavaScript, Python, Ruby. I guess PHP is there,
[13:46] but it had some really small ones many years ago. There are also other languages,
[13:50] but those are the three main ones. All three of these main languages in terms of how many people use in the industry,
[13:57] now have very popular TypeSystems available for them because they're so gosh-darn useful. But almost every other language out there,
[14:07] C, C++, Rust, Go, Java, all these really popular languages have TypeSystems.
[14:15] One of the big flaws in JavaScript that gets mentioned in Chapter 1 of the book is that because it doesn't have
[14:20] a definitive way to describe what stuff is supposed to be, when you have hundreds or even thousands of files,
[14:28] it can get really difficult to manage your code. The TypeSystem is something that lets you manage your code because
[14:34] you have good ways to describe what stuff is supposed to be. >> Got it. Thank you. Can I just say your mic is
[14:42] really good because it literally heard the bag and I'm impressed. I'm impressed with the mic though.
[14:49] We have another question. Sometimes TypeScript can infer what you mean,
[14:55] and other times you have strictly to type. I'm not sure I understand that yet.
[15:03] Does that make sense to you, Josh? >> It does. The way Tech Twitter works is someone will make a joke about something,
[15:13] someone else will notice the nugget of truth or lie in the joke, normally truth, and then make an insightful comments about it,
[15:21] and the people will repeat this over and over, joke, comment, joke, comment,
[15:24] until it's a full-blown meme for the duration of one week. We are currently in that cycle about,
[15:29] I think two days in, maybe three at most, of people debating about the right way to indicate types of the TypeScript type system.
[15:38] We'll learn in this chapter that in many cases, TypeScript can just read your code and understand what's supposed to happen.
[15:44] But in some cases, you need to or can opt into being more explicit. >> Tech Twitter is all ablaze about it.
[15:54] People are posting everywhere. It's this whole thing. It'll die down in a week.
[15:58] I actually recorded a video for it. I've never waded into these stupid discussions before.
[16:03] Apologies. It's not a stupid discussion. The topic is very smart.
[16:07] The way people are discussing it is stupid. This particular question, I quite like and I really appreciate you asking.
[16:11] Thank you. Thank you, Cancer. >> Yay. Okay, cool.
[16:16] >> But yeah, we'll see later in the chapter more nuance around it. >> I am posting also really quick.
[16:30] For those who want to stay along, even if you can't join on the Fridays that we stream,
[16:35] I just linked the repo and that will keep track of all of our streams, all the dates, as well as any projects when I get to them.
[16:47] They'll be in there. We talked a bit about what your plan for this, a bit about what a type system is or how it might be used.
[17:00] But it's something that you said right here and I'm just like, I thought this was interesting in the fact of a type
[17:08] is a description of what JavaScript value shape might be. By shape, I mean which properties and methods exist on
[17:17] a value and built-in type of operator would describe it. I thought that was a good way of visualizing it.
[17:25] Also, to anyone that doesn't like learning from books, I am one of those people.
[17:33] Josh is a really good writer and actually made it funny, which I appreciate it.
[17:39] As someone that likes to just wing it and figure things out, I found that this one is actually worth reading.
[17:47] I'm having fun finding more and more books like that. In this example, you said when you create a variable with an initial value Aretha,
[18:00] let Singer equal Aretha, you also go in and I know I'm going to be skipping around a little bit
[18:08] of that let a first name be Whitney. Those, I'm just going to pause on it,
[18:15] confused me a little bit. But I think it might have to do with,
[18:22] I wonder if I can get, oh, I can, okay. Like the seven basic kind of primitives in JavaScript,
[18:30] and then which ones TypeScript understand. I get Boolean string number,
[18:39] and I feel like null, undefined, bigint, and symbol are things that I haven't
[18:47] really run into very much or aren't connecting the dots. Could you help explain those a little bit or examples?
[18:55] >> Sure. Yeah. I will say that the only one that actually matters in the vast majority 99.99 percent of
[19:02] JavaScript code is the difference between null and undefined. Bigint and symbol are things you will almost never use.
[19:09] I can't remember the last time I've used symbol. I don't think I've ever actually used bigint.
[19:14] I wrote a game engine before that was available. Bigint is like number, but it doesn't round.
[19:19] So it's really good for math, it goes. >> Oh, okay.
[19:25] >> It's not like a floating point number, like one point. >> Okay. Because y'all on opposite Fridays,
[19:33] I'm also learning Python from the bare basics as well. We just went over that,
[19:38] now I'm spacing what it's called, but there's a different number instead of,
[19:42] I think it's actually called int, if I remember correctly. >> Yeah. Python has what, ints and double floats?
[19:48] >> Yeah. >> Variants like that?
[19:49] >> Yeah. There is a variant of what is basically like a whole number and then what can be like fractions.
[19:57] Interesting. That's a connection for me. >> Symbol, we can just ignore it.
[20:04] It doesn't matter, it's not relevant in this book. We don't even need to have gone over bigint,
[20:09] I just think they're cool. Yeah, Ben, I feel like they're good for having the code type stuff.
[20:14] There are projects that use them. There's a reason why the JavaScript people work on them,
[20:21] but we won't get into that in the book. >> Now, I feel like I want to tweet that up,
[20:26] then like, who's actually used these things? >> Yeah. Every language has the concept of something like null or nil.
[20:37] What does Python call it? I always forget, nil, null. >> I don't know if I'm that far in Python,
[20:44] so I'll keep you posted. >> They call it none with a capital N,
[20:49] thanks Python, the only one. You have a variable and you don't assign it an initial value.
[20:55] Let's say you just write the code like let singer semicolon, no equals Aretha or Whitney or anything.
[21:01] What is stored in that variable before you give it a value? The answer is undefined.
[21:07] In JavaScript, the default, there's nothing here, is called undefined.
[21:12] JavaScript also has another thing that is basically the same idea, there's nothing here, called null.
[21:19] It is incredibly annoying to me and many people that JavaScript has two ways to describe there's nothing here.
[21:26] People get into these heated debates about when you should use one or the other.
[21:30] Undefined to many is when there's nothing there and no value. Null is when there is a value and it's nothing.
[21:36] The difference between those two makes no sense to me or most, but some of us prefer.
[21:43] I'd say language mistakes in JavaScript is having two things that mean almost the same thing.
[21:49] >> To just say that back to you, even though they're both confusing,
[21:55] it's like this example of let singer equal Aretha, and if Aretha was missing,
[22:01] it would come up as undefined. >> Yes. There are a lot of
[22:06] old browser APIs that return null, not undefined, when there are no results for something.
[22:13] For example, document.querySelector searches the browser document or the page for something matching a query,
[22:20] and if no DOM elements are found, it returns null, not undefined.
[22:26] That's just the way we live our lives. Preach.
[22:35] >> What up, Rivet? Haven't seen you for a while. I should talk about this. Y'all,
[22:42] for anybody that's in Denver, Genghis Khan is at the end of the month,
[22:46] and it's a tabletop conference. I always forget that Comic-Con is probably like a comic conference,
[23:00] but I'm very excited, and I'm going. It's going to be really awesome.
[23:06] The TTRPG convention. >> Tabletop convention?
[23:13] >> Yeah. >> Cool.
[23:15] >> It's going to be dope. >> Is it bad that I really despise playing most board games?
[23:20] I had a friend group that kept playing them over and over, and I hope one of them is listening so they feel shame about this,
[23:25] and it really ruined it for me. Now I have once a month tolerance for it.
[23:29] Unless it's Catan, I can tolerate Catan. >> I don't think I've ever played.
[23:35] I was in a Twitter space where they were talking about it. The D&D crew was talking about it.
[23:40] I've heard really boring things, not a lot of people really like Catan.
[23:46] >> It's objectively not the best of them. It's older, it's classic, it's good,
[23:52] but we've had innovations and more exciting things. People play Catan for hours,
[23:56] and it doesn't have hours of content in it. I also used to play Magic the Gathering,
[23:59] and I still really like that game. >> I play D&D, but we do it online.
[24:06] I mean, it's still a tabletop game, but we just do it virtually,
[24:11] and I definitely there's more games that I want to look into. I feel like Ribbit Hearts MTG.
[24:22] >> Magic the Gathering, heck yes. >> Yeah. I used to play,
[24:26] but everybody let me borrow their decks to play, to help them compete against themselves,
[24:32] so I'd have really good decks, but that was many moons ago.
[24:39] TypeScript. That was really helpful, so thank you. This was definitely something that also,
[24:48] I think really helps to know, is this something that I need to go down a rabbit hole to research more?
[24:55] Knowing me, I would have been like, I need to go figure out what a symbol is for,
[25:03] why I would use a symbol, that kind of thing, and it may not be something that's actually useful.
[25:08] Okay. Scrolling, scrolling, and y'all, you can buy this book online if we're going too fast.
[25:15] This is just review, give you some ideas of what each chapter is,
[25:19] and answer any questions that we have, and y'all are welcome to continue asking questions,
[25:26] so I'm really happy that cancer has been, so thank you. All right. The next questions.
[25:33] So this one goes with the Aretha part that I had in here of the error is, take the following snippet in which TypeScript is emitting
[25:52] a type error about a member property being erroneously called as a function. Erroneously.
[26:06] I have, for all that may not know, I am very, very,
[26:11] very dyslexic, and part of a lot of dyslexia for people is not knowing how to break down words to sound them out for streaming.
[26:19] So streaming and reading out loud is really fun and not fun. Fun. All right.
[26:28] So let first name equal Whitney. I know I'm not using all of the symbols and things.
[26:33] First name dot length with the brackets, and this expression is not callable,
[26:41] type number has no call signatures. So all of these answers totally made sense.
[26:51] What I was a bit confused on is, would it be like first name with the brackets and quotes to be proper?
[27:10] >> I'm going to nitpick you and I apologize in advance. It's going to help me.
[27:15] You're saying brackets. I would call it parentheses.
[27:18] >> Parentheses. Okay. >> As we get into arrays where we have both brackets and parentheses on the line,
[27:24] it helps me having the right internal monologue for things. I don't know about you, but I'm one of the people that has
[27:29] a very omnipresent internal monologue and that's how I think. >> Yeah. No, I love that because we all learn so
[27:37] differently that it's very helpful to have these conversations. Thank you for the follow.
[27:43] I don't know how to say your name, but I'll show it on here.
[27:48] >> Agribenia. Thank you. All right.
[27:56] >> It's a very mild typo. I'm noticing, just noticing now.
[28:00] The book's not wrong. There should be a period on that second line of the comment type number has no call signatures.
[28:06] The first line has a period, the second line doesn't.
[28:09] These are the things you notice when you write a book, wait a few months and then come back to it.
[28:15] Anyway, so the problem is in JavaScript, if you want to get the length of a string,
[28:21] it's just the thing.length. It's not a function, it's a member property, a field.
[28:28] Adding in the parentheses is wrong. One of the flaws of TypeScript,
[28:34] the big things they've been trying to work on last few years is that a lot of its error messages are too technical.
[28:39] They are accurate and precise, but not super clear.
[28:43] What it's saying here is type number has no call signatures, meaning I, TypeScript,
[28:50] have not been told that there's any allowed way to call length, which those things are called signatures, a call signature.
[28:58] Because there's no call signature, I don't think this can be called as a function,
[29:02] i.e. it is not callable. Those four steps are how we got to that conclusion.
[29:09] >> Thank you. I'm hoping this makes it a little easier, something I probably should have started doing earlier,
[29:15] so you can see where we are on the screen. There we go. That part makes sense.
[29:27] I'm going kinds of errors, and I think you just went through it.
[29:37] This is fun, I just will auto-do it. Syntax and type, that made sense of syntax errors are,
[29:49] if they're missing the quotes, and a type error is if it's not the correct type.
[29:58] In my mind, it made sense. This one didn't necessarily make sense to me,
[30:06] but we did skip that exercise and go, never mind. Because it had classes and me and classes don't get along yet.
[30:14] This one is for type errors, it would be like if I try to use a number instead of a string.
[30:23] >> Yeah, that type of thing. A syntax error is something that stops
[30:28] the runtime from being able to execute your code in the first place. If you have lots of something like that.
[30:33] A type error is, your code is syntactically valid, but TypeScript is pretty sure you screwed up.
[30:39] >> Cool. Now, what? Y'all, I just ended up,
[30:48] in the last couple of weeks, I was like, I need a job, I need a portfolio.
[30:52] I started building a site with Astro, and they are a JavaScript meta-framework,
[31:00] and it uses TypeScript and Tailwind CSS. I started up using TypeScript.
[31:09] We'll be going into that as we go. I mentioned that because I realize the assignability,
[31:18] and I think I tried assigning stuff in my website, which is exciting. Assignability, this made sense of let first_name equal Carol,
[31:32] first_name equal Joan. It followed along because they are the same type.
[31:38] It doesn't need to be the same string, but they are the string.
[31:42] They don't have to both say Carol, they can, and that it follows along meaning that, okay, cool.
[31:49] If we do let first_name be Carol, that's a string. First_name equal Joan, that's a string.
[31:55] Let last_name be King, that's a string. Last_name equal true, no.
[32:02] >> Not allowed. Because everything was a string until you added a Boolean in there,
[32:07] and TypeScript does not like mismatches. >> Yeah. All of that made sense,
[32:12] and you can change types around and that type of thing. All this made sense,
[32:22] and this is a big place where type annotations, and not needing to have doing too much on,
[32:46] I'm just making sure I didn't actually write a note for this, but I'm like, I feel like this is
[32:51] something I was supposed to write a note for. Because this is to say here assigning,
[32:59] I'm highlighting what I'm reading. Here, assigning the evolving any variable rocker is first assigned as string,
[33:06] which means it has a string methods such as to uppercase, but then evolved to a number.
[33:13] Could you explain this area and what's going on a bit more, please? >> Sure. We declare this variable rocker, rock on.
[33:25] Fun fact, the rock on sign is the sign of the horns, like the devil horns, that's where that comes from.
[33:31] Cool piece of trivia. We declare this variable rocker,
[33:36] and TypeScript doesn't know what's supposed to go in it. We haven't indicated to TypeScript what it's supposed to contain.
[33:42] To start, TypeScript considers it to be type any, which is a type that'll keep coming up and I'll
[33:47] get more and more angry towards as the book goes on. Any says, I don't know,
[33:51] just let me do whatever I want. Anything. >> Okay.
[33:54] >> When we, on the next line of code, assign a string to rocker,
[33:59] TypeScript knows, okay, they have assigned a string. Rocker is now type string.
[34:02] You can call methods like to uppercase that exist on string. >> Okay.
[34:07] >> But a variable that is what's called an evolving any, meaning it wasn't given an initial value or type,
[34:13] so it's just been assumed to be the type it was given, is allowed to be a new type or given a new type of value.
[34:22] Rocker equals a number is totally fine. At that point, TypeScript evolves its understanding.
[34:27] It switches it from string to number because it sees, we never said what it's supposed to be,
[34:32] and now we've switched it from string to number. Does that answer what you're looking for?
[34:39] >> Yes. To compare, let's see if I can actually make this smaller.
[34:47] This might be hard for everyone to see, so we're just going to do it this way.
[34:54] The reason this one didn't end up being any and it has to stay a string is because it's let first name equal something,
[35:04] and that's why it's associating with it, so it can't be changed.
[35:08] But if it was let first name, would you put equal any or just let first name?
[35:14] >> You're skipping ahead. You're asking how to give it a particular type to a variable.
[35:20] If you don't have an initial value, there is a syntax that you can use to
[35:25] tell TypeScript what is supposed to go in the variable, and that syntax is called type annotations,
[35:30] and it comes up in the [inaudible] >> Okay. That's where we got here.
[35:36] There we go. Of let rocker, and let rocker is not assigning to anything.
[35:43] Therefore, instead of saying the equals, whatever it equals, and for that example.
[35:49] We technically don't need to put that it equals a string. We could tell it that it equals
[35:54] a word and therefore it knows it's a string? >> Yes.
[36:01] >> This one says let first name equal Carol, it doesn't need to be let first name equals string.
[36:09] >> That's correct. >> Because Carol is a string.
[36:12] >> The way that you tell TypeScript the type of something isn't with an equals,
[36:15] it's with a colon if you don't have a value. You can either say let first name equals
[36:20] Carol or let first name colon string. Both of those things would tell TypeScript
[36:26] that first name is supposed to be a string. I'm going to bring this up for rivets,
[36:33] but I'm writing that down really quick. >> Yes. I would say that evolving any variables
[36:42] are generally bad-ish. I don't think we actually have
[36:48] a lint rule against them in TypeScript vs Lint. I personally try to avoid them.
[36:52] I honestly just try to make variables consts whenever possible.
[36:56] Even if I'm not in a project that uses the const syntax overlaps,
[36:59] I generally try not to mutate variables over time because it then gets hard to keep track of them.
[37:05] Most of the time I end up not having evolving anys. I'm hesitant to say no,
[37:12] it's bad or yes, it's good or whatever because
[37:15] it's not something that people end up doing a lot, so we don't have too many hard feelings on it.
[37:20] But eventually there will probably be some week-long Twitter flame war about it,
[37:23] and then we'll see who really cares. >> To see if I recap that to understand,
[37:29] even though that's technically possible, is it considered bad to change types on a variable?
[37:37] Is what Rivet asked. What you're saying is,
[37:40] even though we can, we don't necessarily always want to use it as a moving variable.
[37:50] We want to have it as we're going to define it, such as let first name equal Carol,
[37:56] just so that way it's defined as a string and we don't have to worry about it moving or changing.
[38:03] >> Yeah. Just keep your code simpler, easier to understand. It's hard enough to understand code as it is,
[38:10] let's not make it harder for our developers. >> Yes. Ben just said,
[38:16] so tired of the flame wars. >> Yeah.
[38:19] >> I mean, lucky enough for being a beginner is, I am still learning it all,
[38:26] so I don't get them when they're there. Some of them I'm starting to get,
[38:30] which is exciting. Let me scroll down here so that way y'all can see where I'm going.
[38:44] We have let rocker colon string, and we're still talking about the type annotations.
[38:51] Then the unnecessary annotations, which I think is very interesting.
[38:59] This also helps, this is where I was, this connected what I was asking about at the beginning with Aretha.
[39:11] I'm like, you answered it throughout the chapter, that was fun.
[39:15] Yet, what I'm wondering, and would love to show you what I was doing with my site,
[39:25] so give me a second because I'm not used to how to do this with so many screens. No. Now, we're just going to do this.
[39:39] Come on. There we go. >> I'm using rectangle for that.
[39:42] >> I am using rectangle. Yeah. I'm just not used to it yet.
[39:49] I got rectangle, which y'all, it's a really great app.
[39:52] You should definitely check it out. But then I also got Arc, the new browser.
[39:56] Between the two, I don't know what I'm doing. It's very awkward. But before we go into what my questions are going to be,
[40:04] Cancer asked, when building a function for the first time and it takes some parameters, do you start with type any and work backward towards stricter typing?
[40:14] >> I'll answer it in the general of when I write code in general, such as functions or variables,
[40:23] such as parameters, functions, variables. Do I start with type any and work backwards?
[40:28] If I need to. Generally, when I write code, I try to first think in my head what type is stuff going to be.
[40:34] There is eventually going to be a term someone comes up with like type-driven development that
[40:40] doesn't have the same acronym as test-driven development. But I try to think in terms of what are my values,
[40:46] what types can they be, and then how do I represent that in the type system?
[40:50] If I know the type of something, I will write it. Even if it's slightly wrong,
[40:54] I'll write it, get the code to have correct syntax, and then fix the type errors.
[40:59] But if I don't know the type, yeah, totally reasonable to write any.
[41:02] You can say colon space any as a type for something rather than colon string or colon number.
[41:07] If you don't know the type yet, it is better to say any and just know that as a to-do for yourself
[41:12] later than to freeze and not write your code at all. Totally fine to use any during development.
[41:19] I just would not recommend allowing them to persist in your code base. >> I was listening and then forgot what I was going to write down.
[41:28] What did you say was parameters again? I think you said like string or something?
[41:37] >> This question is specific to function parameters, but my answer is the same for function parameters,
[41:44] variables, anything that might need a type annotation. >> Okay.
[41:48] >> Fun fact, arguments are what you give to a function. You give a function an argument.
[41:54] Parameters is when the function declares what it takes in. They're not the same term.
[42:01] >> No one ever remembers that. >> This is why coding is so confusing.
[42:06] But at the same time, it's like when you finally start getting it,
[42:09] it starts to make sense. It just takes a while. What we are looking for, yay.
[42:19] >> Yay. >> Yay. Thanks to Josh.
[42:23] >> My pleasure, Cancer. It brings me joy every time.
[42:29] I built a site and I got a theme to start it off from Astro, which is a meta-framework.
[42:37] What I was doing is, so I will go a little backwards,
[42:44] is they have all of these components and I was like, I really, really like this code component.
[42:51] But it doesn't have anything in here that I can change and manipulate what's showing up on the screen.
[43:00] I was like, okay. I had to go find where this was. This is when I started figuring out the imports.
[43:06] I was like, okay, so we go to data, we go to code,
[43:10] and then we have our code.json, and they're in a very specific format.
[43:16] I'm like, okay, cool. Well, I'll just keep doing this, whatever.
[43:20] It has this index file. I'm like, okay, so I figured out enough that
[43:29] it's the importing the code site from types, and that there's sites data from code.json,
[43:41] and it exports as Git code. I'm like, okay, I feel like I understand this enough,
[43:49] but this does not help me put the dates. I really wanted my stream schedule to
[43:54] have the dates and to give y'all a visual, because that's always helpful for me.
[44:03] I go to portfolio, code. This is what it looks like. It looks beautiful.
[44:14] I really wanted it everywhere. I was like, cool, I'm going to make more of these.
[44:20] We have writing, we have speaking, all look great. These were very easy to duplicate.
[44:24] They all do the same thing. They're all the same sizes. Awesome.
[44:28] >> Very nice. >> Thanks. But for my live stream, I want dates.
[44:36] I really want dates. They need dates,
[44:39] and it didn't let me do dates. I was very agitated.
[44:46] In case anybody wants to know how I code, a lot of it is me yelling at my laptop.
[44:52] This is why I'm like, I don't know if I can actually do
[44:56] live coding instead of just learning, because I just yell at my laptop.
[45:00] What ended up happening is I followed. I was like, oh, there is a type.
[45:09] I'm going to go investigate. This is what goes through my head.
[45:15] I'm like, oh, look at all of these types. They do things and they do things.
[45:20] I actually created a thing of export, interface, stream site, and I added date.
[45:31] I got it to work. It clearly works. I'm very excited about this.
[45:35] I'm so excited that I figured out how to make it work. But I don't actually know what I did in
[45:41] the fact that we end up going through. We're going to see if I can make both of these big
[45:46] enough to ask my next question. Let's see if this works now.
[45:52] No. Do we want to do this? No. I don't know how I did that,
[46:02] but that is really cool. It's done. >> I would like to know what shortcut you
[46:08] just pressed because it looks really useful. Is that an on-screen magnifier, accessibility thing?
[46:13] >> Yeah, but I think it was from view. I don't know.
[46:28] Oh, show magnifier. It is the thing next to the one.
[46:35] >> Tilda? Is that Tilda? >> Yes.
[46:37] >> I actually never know if I'm right about that. >> I think it's called Tilda. You are right.
[46:41] >> Cool. >> I think. I don't know.
[46:42] That's what people have told me. This is fun.
[46:46] >> Look at that. >> I feel like we. My question is,
[46:52] so we got type shapes coming up, but we also have modules.
[46:57] I know you said there's some that aren't that important in here, and I'm really glad that we're talking about this,
[47:03] but I'm like, so there's type shapes, there's modules. I also have in here components,
[47:09] and I did something here with my TypeScript JSON index file into my component to make it work,
[47:19] and I don't actually know what all these separately mean, or if they're connected.
[47:26] >> It's funny because Chapter 7 is what covers interfaces, and I believe we're on Chapter 2 today.
[47:33] >> Yes. >> Jumping ahead.
[47:38] >> I will also note that the difference between a script and a module in JavaScript is not useful in most of the book.
[47:48] It's not something that comes up more than once or twice. I forget whether I've mentioned in the book that this is not
[47:54] something that you need to pay a lot of attention to, but it's just barely useful enough that we have to include it.
[48:01] A module is a file that imports or exports, I believe. I think that's a technical definition.
[48:08] If there's an import statement or an export statement, it's a module. >> Would that mean that my,
[48:16] let me go back up here to index. It imports and it exports.
[48:24] >> It's definitely a module. >> Rivet calls the tilde an eyebrow or the eyebrow,
[48:34] and Ben said that the magnifying glass is especially nifty for streams. I agree. I just don't know which way we're going on this,
[48:45] but it only works in PDF, I'm pretty sure. Let's magnifier.
[48:53] It doesn't go all the way over to my, so it's just for this,
[49:00] but that's still pretty cool. >> The index file is like a module because it has an import and export.
[49:10] >> Sure. All you need is one of them to qualify as a module. Any file that has an import and/or an export is considered a module.
[49:22] >> Nifty. Cool. >> Then you also asked about components,
[49:29] which is like a totally separate concept. A component is an idea in a lot of UI frameworks,
[49:38] where it is a single area of your view that takes in some information and renders UI output.
[49:48] Your header would be a component. >> Right. I'm understanding what you're saying,
[49:57] but I'm like, I don't know how to write that for notes. >> Sure. I do like the way that React does its description of components.
[50:08] I realized that this is like the fifth flame or I might be entering here. But in React, a lot of components,
[50:14] the most common way to describe them now is with a function. It takes in some information and literally returns a description of the HTML,
[50:23] that is output. Now, that's technically inaccurate.
[50:27] In some cases, it was like React for a native level, but in reality, it's like you take in some information and you
[50:34] return the description of the DOM. That is a result. That is a really common way to think of and describe a component.
[50:44] >> Okay. Cool. I like that. Then we also talked a bit about, where did I get this?
[50:57] Hold on. I have a reason to use a magnifying glass. Now, let me, I guess I should just actually use the tilde.
[51:07] A module is a file with the top level export import. That makes sense. A script is every file that's not a module.
[51:21] >> If it doesn't have an import or an export, it's a script. >> That's all the other files.
[51:31] >> This.json is technically a script because it doesn't say that it's importing or exporting anywhere.
[51:42] >> It's neither. I guess modules and scripts. >> Because it's a database?
[51:46] >> I don't know if I actually say this in the book. Modules and scripts is only referring to code files,
[51:54] like JST. Code.json is just some file on your system that is not part of the JavaScript understanding.
[52:04] Now, they're adding in ways to the language to really nicely interact with data files like JSON.
[52:12] But this is not JavaScript code. This is data or database, like you said.
[52:17] >> Okay. I'm trying to think. I probably don't have anything that doesn't import.
[52:25] >> Yeah. Most codebases, basically every file is a module. Scripts are really mostly from older codebases.
[52:33] Mostly, not completely. Not JavaScript.
[52:39] >> It's marked down. >> It's just a random file on your system
[52:41] that someone else might interact with. >> It's only for JavaScript, you said, right?
[52:47] >> Yeah. JavaScript and languages like TypeScript that poop out JavaScript.
[52:52] >> Interesting. Okay. That's all making sense.
[53:04] I think that was actually the bit that wasn't the end of the parts that weren't making sense.
[53:16] Although I do think if you could, is there something, and I have a feeling it might be more about
[53:26] like type shapes or the annotations or unnecessary annotations. You answered all of my questions.
[53:34] Thank you. Are there parts that you think that a lot of people may miss or you
[53:39] really want to drive home that we should talk about? >> Yes. Cancer at 12.18, my time.
[53:46] Messaged something that I like one-third answered, and then we said we'll get to later.
[53:51] Sometimes type, I don't have the ability to focus on the thing, but sometimes types you can infer what you mean,
[53:57] and other times you have to strictly type. Can you talk about that if it's not
[53:59] outside what you're already talking about? That's very much.
[54:02] >> Okay. Cool. Do you want me to show something in the book?
[54:07] >> Yes, please. We're working well. We're on the same web link. I was about to ask.
[54:12] >> Yay. >> There's the section on unnecessary type annotations.
[54:17] I think a little earlier. >> I have.
[54:20] >> Yeah. This is a good example of, we are telling TypeScript something that
[54:27] it already can figure out on its own. It's like me telling you, okay,
[54:31] I'm going to tell you a string. The value is Tina,
[54:34] like you know it's a string, so there's no need to tell TypeScript this.
[54:39] There are cases where it's useful to use explicit type annotations such as
[54:45] variables that don't have an initial value. As you go through the book,
[54:48] we'll see some places where it is anywhere from somewhat useful to tell TypeScript to type,
[54:54] arguably debatably, to totally necessary, you should really do it.
[54:58] In general, the rule of thumb is use explicit type information or annotations,
[55:07] like explicitly type the stuff out as little as possible. >> Give me just a second.
[55:15] >> Sure. >> I will be right back.
[55:18] >> I'll do crowd work. What's the deal with the bees?
[55:24] Anyone up to anything fun this weekend? If you hear a child yelling,
[55:33] it is my niece Liel. She is very serious.
[55:36] I'd like to take this moment to give a shout-out to, maybe looking at home it's going to say Mastodon.
[55:46] Ooh, what are you looking for? I am like a year and a half.
[55:50] Board game night. Ben, you're killing me.
[55:52] We covered this. No, that sounds lovely.
[55:57] Thank you, Cancer. I'm glad it was worthwhile for you.
[56:02] Yay. >> I've been trying to get my wife into Magic the Gathering.
[56:07] It's been really slow. She already plays D&D,
[56:10] so it's not like I don't like nerds thing. It's just like this specific game.
[56:15] Takes a while for her to get into. She doesn't like math, like the small numbers.
[56:19] Good. No friendships ruined. That game has a reputation.
[56:24] What are you going to play? Oh, hi. >> Hi. I just want to say sorry, everyone.
[56:30] My Grams went into surgery this morning and my mom was like, "Okay, I'll text you when she's done,
[56:38] just to let you know everything's okay." I'm like, "Okay, cool."
[56:41] Then it comes up that my mom's calling me. I'm like, "Oh my God, what happened?"
[56:45] My mom's like, "I forgot I said I would text you." >> Great.
[56:53] >> Everything's good. Y'all, we're good. But apologies for the interruption.
[56:58] Good news, my Grams is okay. I'm happy to see that you guys are going back to
[57:03] the D&D magic and canton conversation. It's always a fun one. My audio broke before I even heard you finishing this.
[57:20] Did you have anything else to add about the [inaudible] >> Yeah. I get that annoying Bluetooth thing
[57:29] where if a call comes in, everything stops. But yeah, final conclusion.
[57:33] In general, use as little explicit stuff as possible. Get away with it as much as you can,
[57:41] letting TypeScript infer everything because TypeScript is normally at least as smart and often smarter than you.
[57:48] Then there are cases where if you use what seems like a reasonable explicit type annotation,
[57:53] you will just be reducing TypeScript's understanding. You'll be telling it something more general and
[57:58] less specific than what it would have thought. But know the cases when it is useful to tell TypeScript
[58:04] something explicitly because sometimes it is better. We will see a few cases,
[58:09] one or two per chapter maybe, as we go through the book. Right now, the tech Twitter flame war thing is on function return types.
[58:17] When you have a function, should you explicitly tell TypeScript the type of what it returns?
[58:21] The answer, not my answer, the answer, the correct answer, he says,
[58:26] knowing he's going to get yelled at, is only what it benefits you.
[58:31] >> Okay. I like it. Also something that I realized
[58:40] that we might have glossed over a little bit, that maybe I'm going to ask you to do the recap of it,
[58:51] of type shapes because we didn't actually spend time on it. I think that's actually the only part of the chapter that I was like,
[58:59] "Oh, this actually makes sense." But I would like you to explain it so I could see if it actually made sense.
[59:06] >> Yeah. TypeScript knows not just whether you are a primitive type. By the way, the word primitive is very
[59:14] important because later on we'll see things that are different. A primitive type is like string, number, and so on.
[59:20] TypeScript also understands object shapes. If you have an object,
[59:24] TypeScript will make sure you're not accessing members or properties of it that don't exist.
[59:30] The example in this code, the second one, let's share equals firstName, lastName.
[59:36] If you try to say share.middleName, TypeScript will yell at you because it knows you declared
[59:40] an object that only has firstName and lastName, not middleName. Similar to how TypeScript can do
[59:46] assignability checks like Boolean versus number, it also does property existence checks.
[59:52] Does middleName exist on share? Is that what you were looking for?
[60:01] >> Hold on. >> Are you now looking for a file where you can try to find an object,
[60:08] and do object.asdf, asdf to see if it triggers anything? >> No. What you're saying makes sense more of,
[60:16] these are things that I don't necessarily know exist or why they exist. I just know how to make it do what I
[60:24] needed to do because I messed around with it enough. But since you have just these brackets that were already called for,
[60:35] this is why dates weren't working, because it was outside of the shape.
[60:43] You are putting words to what I learned. I can actually talk about it and know how to Google it.
[60:49] >> Yay. >> Because I didn't know these were called shapes.
[60:54] >> I don't know how many people call them shapes. I think the technical term is typically object types.
[61:04] >> Well, the shape would be all three of these together that was written out that I named TypeStream, or GitStream.
[61:18] I named it down here. It says export code site.
[61:23] It had these three, so this is a shape. But my date didn't fit in the shape,
[61:31] so I created a new shape that has all of these types in them. >> All the properties.
[61:42] >> Sweet. TypeScript is actually starting to make sense, and we're only on Chapter 2. I'm excited.
[61:48] >> I mean, you're on Chapter 7, but you know. >> We're on Chapter 2.
[61:54] This is something that I've definitely learned for myself in my own learning style, is if I have to just stick with the bare basics,
[62:04] it doesn't make sense yet. Because unless I can see how it fits into the big picture for myself,
[62:11] I'm just like, "Okay, cool. This doesn't make any sense yet."
[62:14] We're bouncing back and forth, where if I were to read all of Chapter 7,
[62:19] probably won't make sense because I don't understand Chapter 1-6. But this one part, it really does help with putting 2 and 2 together.
[62:28] Now, is there anything else that you wanted to cover before we wrap up today? Let me go down to the summary.
[62:39] I think that would also help to see if anybody else has any questions. I don't think the magnifying glass is big enough.
[62:47] >> It's adaptive. Very nice. >> Here we go. That is the summary for today.
[62:54] If anybody has questions or something you want us to go into more detail, I know we talked previously about doing the projects
[63:03] online once my mouse is done being over here. I will link them because I feel like it's going to be more important to go
[63:12] through the chapter and ask questions. Next week after I do the homework,
[63:19] if I have questions, I'll ask questions. But not necessarily that something that we need to do on stream.
[63:26] But if you-all have questions, I would really like to make sure that we get those answered
[63:32] because I know having access to a human to answer questions is so valuable. >> Yeah. No, this all sounds good to me.
[63:43] I got nothing else. I'm just reading through the book on the side to make sure I haven't missed anything, but sounds good.
[63:49] >> Great. Awesome. Then let me go back to our normal screen.
[63:56] I also want to make sure that we re-share the GitHub repo because it has all of the links.
[64:05] That way, you can know where to look at all of the book, where to get the book, the chapter projects, chapter summaries.
[64:14] It is all in one area. Also, if you did not catch chapter 1,
[64:20] that will also be in there. There we go.
[64:30] Just want to say shout-out to everybody who joined today, and thank you so much for asking questions,
[64:38] because these are questions I may not know to ask either, because I am coming from more of a beginner point of view,
[64:44] and TypeScript, I've found, is hard for a lot of people,
[64:48] no matter where they are in their coding journey. It's been very-
[64:55] >> I think it's good to have people learning in public like the way you're doing.
[64:58] I think it really helps. It helps show off the learning,
[65:02] and it also just helps show off different ways of learning, which I think is really crucial.
[65:07] >> Thank you. Next week is going to be regular scheduling of Monday, is Ms. Monday with Laura,
[65:18] where we literally just hang out and talk about random tech things or life, or just so many random things.
[65:26] Then Tuesday is going to be probably whatever I'm working on or no stream, because that's what I like to do on Tuesdays.
[65:33] Wednesdays is the mental health and neurodiversity Twitter space, and Thursday is open source with distribute aid.
[65:44] Last but not least, next Friday is Python, because we do it every other Friday of learning a language,
[65:52] TypeScript and Python. This is something that I am very,
[65:57] very proud of putting on the site that I got it figured out. The entire reason I started looking more into the TypeScript stuff,
[66:05] if you would like to know the stream schedule. Yeah. Ben's going to think about getting into streaming on Tuesday.
[66:15] That's what everybody should be doing on Tuesday. >> Do it.
[66:19] >> If you're not doing it yet, that's what you should do on Tuesday.
[66:23] Yes, please. Yes, yes. All the questions.
[66:35] I think this is, Ben, we've talked about questions I've already had for you too.
[66:44] I have so many questions already. I will be writing the list.
[66:50] Also, if you want to stay up-to-date with this stream schedule, there is that.
[66:57] I'm reading it and I'm like, yes, yes, yes. >> Okay.
[67:08] >> Yes. All right, y'all. You are about to get raided because that's always important.
[67:17] Rizelle is currently streaming from GitHub and that's amazing. She is doing open source Fridays.
[67:26] That is something she's always done. This month, I love the fact that she is making sure that
[67:31] it is black maintainers for Black History Month. Something really dope, make sure you go support.
[67:40] What? It says I'm unable to raid. Well, I wanted to raid.
[67:47] Maybe I'm not going to be able to. Rude.
[67:50] >> I really like the window there. >> I know. I'm also clicking the wrong link as we go over there.
[67:59] I'm hitting the plus sign. Well, I guess, I wonder if they have raids off.
[68:07] Okay. Well, we will raid into the alt F4 string. Pretty cool over there.
[68:16] If you don't like it, go check out GitHub.
[68:19] That's what we'll go with. All right, y'all. Thank you so much.
[68:25] Let's see if this raid goes through. It says it's going to go through.
[68:30] Thank you again and have a wonderful weekend and we'll see you next week.
[68:36] [BLANK_AUDIO] 
