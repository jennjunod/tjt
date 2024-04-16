---
showLink: "https://www.youtube.com/watch?v=KvANdTwjvGM"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-typescript-with-josh-goldberg-the-beginning"
title: "Teach Jenn TypeScript with Josh Goldberg: The Beginning"
publishDate: "2022-09-27"
coverImage: "https://i.ytimg.com/vi/KvANdTwjvGM/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome back to another episode of Teach Gen Tech.
[00:07] We apparently have the green crew here right now because you're wearing green, I'm wearing green.
[00:14] Also, your mic was green at the moment. I love those color-changing ones.
[00:19] Yes, we are here for another episode with our guest, Josh, and he's going to be teaching us foundations of TypeScript.
[00:28] I'm going to give this another shot. So many people reached out about
[00:31] the other episode and was like, "Jen, don't give up on TypeScript."
[00:35] I don't know. I want to. Josh, please introduce yourself
[00:42] and a bit more about what we're going to be talking about today. >> Absolutely. Hey, everyone.
[00:48] Excited to be here. Thanks, Jen, for having me on. My name is Josh Goldberg.
[00:53] I'm a full-time open-source maintainer in the TypeScript ecosystem. That means instead of working for
[00:58] a company and making real money like a good tech person, I work on shared open-source tools and beg for money on the Internet.
[01:05] If you might have seen me floating around, sometimes I contribute to TypeScript itself,
[01:09] sometimes I contribute to random other projects. Most notably, I work on TypeScript ESLint,
[01:14] which is the tooling that lets you run ESLint on TypeScript code. I really care about people learning TypeScript,
[01:21] which is incidentally the name of the book that I wrote to teach TypeScript. I'm excited for Jen to give a second attempt here for TypeScript.
[01:30] I actually really respect that you're ready, willing, and able to do that so quickly.
[01:34] I think most people with most tech, it can take them a time or two or three to learn it,
[01:39] and sometimes you just got to keep powering through until you find an Nth strategy iteration that works for you.
[01:45] >> It's not always my favorite, and I appreciate that you do say that,
[01:48] but a lot of it is me being very, very stubborn as well.
[01:57] Yes, shout out to Ben connecting us. Hi, Ben. >> Hey, Ben.
[02:04] >> I would say something that I really, really appreciate about the tech Twitter,
[02:15] tech world is that that's how I met so many amazing humans and built a community. I'm very grateful for that,
[02:24] and I am slowly going to be adding all your info into Twitch very slowly, because it says you cannot post over the $500 character limit.
[02:41] It can be $500. Come on, if we get enough subscriptions for that,
[02:46] $500, that would work. Awesome. Well, yay, and yes,
[02:54] Ben is actually the one that was like, "Yo, here's somebody that can reteach you or teach you more about TypeScripts."
[03:02] That is the world of networking. I know I talk about that a lot,
[03:06] but networking is your friend, even though learning all the tech and things.
[03:12] What is your background? >> I'm moving to Philadelphia from Brooklyn on Thursday,
[03:20] which is why it's this dilapidated half dead wall. But this is a poster I'm terrible with.
[03:27] This is a poster that was drawn by Craig O'Connor, the Halo Community Lead.
[03:33] I won it at a charity auction a few years back. It is a Mr. Chief poster,
[03:37] which is like a parody of Master Chief from Halo that he's done a bunch of. Superimposed on a Marathon poster,
[03:45] which is a Marathon is one of the game series Bungie made before Halo. It's a deep cut mixed with a slightly deeper cut.
[03:56] >> I dig it. I love the idea of how it's like the options of art in the world, but there's so much that we could unpack there in video games.
[04:10] That's a conversation for another day, because I have to remind myself to not completely derail all the time.
[04:18] How do you become an open-source full-time open-sourcer? >> That's a great question.
[04:28] >> Is that a term? What do you call yourself again? >> I call myself open-source maintainer,
[04:34] but I don't know that that's the easiest set of words to regurgitate quickly. I like open-sourcer.
[04:39] >> I've seen open-sourcerer out there. >> I like that one.
[04:43] >> That could be me. I'd say it's not something that is easy to dive into at the very beginning of your career.
[04:51] I just happened to do a lot of open-source stuff more and more over time. Where at first I would publish a project or two,
[04:59] I had one that went viral and for a brief period of time had attention and then stopped. Then I just kept doing work in random open-source libraries
[05:08] until earlier this year, really late last year. I realized what I was really passionate about,
[05:14] the tooling that I want to work on is all open-source. I wanted to work on TypeScript ESLint and my libraries
[05:20] that do other static analysis for TypeScript and TypeScript itself. I've accumulated enough money and I have a spouse with health insurance,
[05:28] so I can make that risky jump and just do open-source full-time. >> Yeah, that is very cool.
[05:35] To unpack this just a little bit, but also to quiz myself.
[05:40] Open-source is technically open-source software, but everybody says open-source,
[05:47] but if you type it, it's normally OSS. Open-source means that anybody can contribute to it
[05:53] and anyone can use the code elsewhere as well. >> That's right. Technically, there's also open-source hardware.
[06:00] You might have hardware schematics like 3D printing stuff that's open-source. That's why people use the terms interchangeably.
[06:06] But yeah, I personally just deal with open-source software, which is stuff that anyone can look at,
[06:11] anyone can send suggestions over to, and anyone can use. >> Dope. Then also,
[06:18] if we talk about linting, linting is how something will go through and find errors,
[06:28] or set an idea of, hey, this is how something's going to be done,
[06:32] so like a spell checker. >> Yeah. The analogy I like to use is that in traditional JavaScript land,
[06:41] there's nothing that tells you whether your stuff is working until you run it. Yeah, a spell checker, a little blue or green or whatever,
[06:48] red squigglies in Word, that's a good analogy for something that looks at your code,
[06:52] doesn't actually run it, it doesn't say it out loud, but it just knows,
[06:56] hey, this is probably a mistake here. >> Dope. Then before I start sharing my screen and going through all of that,
[07:04] I do want to put some stuff on screen with this is where to, down there, is where to follow Josh.
[07:15] Also, go check out the book, and that's where to follow on Twitter as well.
[07:22] Then we are using a plug-in that I didn't know existed, so I wanted to share the knowledge here that it can share, it's live share.
[07:36] I'm like, dude, this is cool, and I'm still in VS Code.
[07:41] That gets everyone caught up and share my screen. Please definitely share any questions that you have while we're doing this too.
[07:55] I don't know if the chat will make it too small for everything, but well, that's a little too big.
[08:03] Is that easy enough to see, everybody? Sweet. We'll see if anybody else.
[08:12] >> That's good to me. >> Dope. Please talk us through what you have magically set up for us.
[08:21] >> Let's start from scratch, actually. Suppose you have a variable.
[08:26] On the left is the source file that we're going to be working with. What I want to show here first is writing code in TypeScript,
[08:35] and that it gets compiled to JavaScript. The first thing you got to understand about TypeScript is
[08:40] that it is a language a lot like JavaScript. Instead of having JS files,
[08:44] you have TS files, but they're basically equivalent to
[08:47] the JS files you would have written in JavaScript. I have in my terminal,
[08:52] you can ignore the errors. I have in my terminal tsc-w running,
[08:57] which is a TypeScript compiler, and that takes files that end in TS and turn them into the equivalent JS file.
[09:06] As you may have noticed, the let my name equals gen variable on the left
[09:12] looks the same as the let my name equals gen variable on the right. As we go through types of things,
[09:18] we're going to add features and see places where TypeScript can fix and find issues for us.
[09:24] But the really core concept is that you're writing code that looks a lot like JavaScript and behaves basically the same as it would in JavaScript.
[09:31] Does that make sense and seem reasonable so far? >> Yes. Just to double-check.
[09:42] First off, it will not auto-translate to JavaScript. It's because you used something in your terminal to auto-share.
[09:56] Then we just got a question as well, so I'm going to interrupt myself.
[10:04] Just looked you up a question in your course. Do you teach bracket generics?
[10:11] >> Yes. That's a feature. I don't think we'll have time in the stream today to go into it.
[10:15] But yeah, in the book, I do have a whole chapter on generics. It's my least favorite one,
[10:19] but it was also a good chapter. >> Well, we'll need Josh to come back on,
[10:25] so we'll just bug him for that and get him back on the show again. It's my hope. Everybody ask lots of questions, play nice.
[10:33] I'm more saying that to myself, so don't scare anybody away.
[10:39] That's how we're translating it over to TypeScript to JavaScript. Then I'm trying to think of a really good comparison,
[10:53] and my grandmother is coming to mind of TypeScript versus JavaScript. If back in the day,
[11:07] anyone that was a secretary had to create shorthand, which looks crazy, did the same thing.
[11:16] It was because they had to take notes so quickly because transcription didn't really exist back then.
[11:21] But it technically was the same information. It was just in a very,
[11:26] very short version of it to make it easier to take notes and still make everything as pretty.
[11:34] Is that a good way of comparing these? >> You know what? It is a good analogy,
[11:40] except for one thing, TypeScript code is a superset of JavaScript code. Meaning, I think that was on the last stream too, that term.
[11:50] TypeScript, the language includes all the stuff in JavaScript, the exact same as JavaScript, along with other things.
[11:56] Shorthand, it's a good analogy in that, yeah. They mean the same thing, they just look differently.
[12:02] My one gripe there is that it's the other way. It's that the TypeScript code will have more stuff than the JavaScript,
[12:12] and the only difference between the TS and the JS is that anything TypeScript developer time-specific
[12:17] gets removed when it gets turned into JavaScript. >> Maybe another analogy would be TypeScript would be like,
[12:28] if you're writing an essay and you have a lot of notes from a proofreader in there, like a little arrow here,
[12:35] like, "Hey, this word looks bad," or, "Hey, that's a really good sentence there."
[12:38] But then when you turn that into the output PDF, all those little side arrow things get
[12:44] removed and it just looks like the words itself. Does that feel like an equivalent analogy to you?
[12:50] >> It does. I don't know if I asked this in the last stream, as well as straight up asked you,
[12:58] why would somebody use TypeScript compared to JavaScript? >> Great question. Let's look at variables.
[13:08] Here, I'm just going to close on my end. Let's say that you have this myName variable.
[13:18] TypeScript keeps track of the types of all your values, of all your things. If you were to hover your mouse, and actually,
[13:25] could you please hover your mouse over the variable myName in your TypeScript file? Yeah. TypeScript sees that it's type string because its initial value is gen.
[13:35] Later on, if you do myName equals Josh, that's allowed because Josh, the string is a string.
[13:42] But if you were to do myName equals undefined, TypeScript would yell at you, and if you hover your mouse
[13:48] over the myName that has the red squiggly, it would complain that, "Hey,
[13:53] you initially set up the variable as string, but now you're trying to give it undefined. That's not allowed."
[14:00] TypeScript keeps track of the types of all your things and yells at you if you put something in a place that doesn't match the type,
[14:07] which can be really useful if you have code that expects, say, a variable to be a string and not undefined.
[14:13] Well, how does that feel? >> Very simple and complicated at the same time,
[14:21] which is like all of text. I'm going to say cool,
[14:25] and let's keep moving because it'll probably click later on. >> Okay. TypeScript is one of
[14:33] those things where it really is most beneficial when you have a few files or more in a project.
[14:38] If you have just one file and it's like this little Node script you're writing for fun or something,
[14:42] maybe don't use TypeScript. But if you have, say,
[14:45] a whole bunch of functions and objects and classes and stuff all working together, it's really nice having TypeScript tell you what everything is expected to be.
[14:53] Because then as you change stuff, it'll let you know what you need to update to account for the new shapes.
[14:59] >> Okay. >> We can keep going. But does that context make sense and seem reasonable so far?
[15:04] >> Yes. Thank you. >> Cool. The first concept that we'll see that's TypeScript specific,
[15:11] is the concept of a type annotation. I'm just going to comment these things out and keep going.
[15:18] My name delayed. This is a variable and we don't know what's supposed to go in it.
[15:25] We could give it a name, we could give it a Boolean false.
[15:32] This is all allowed. TypeScript lets you say on your variables, if they don't have an initial value,
[15:37] I will later assign a particular value type to them. Later on, I'm only ever going to put a string in this container,
[15:44] which means that line 3, name delayed is Josh, is allowed.
[15:47] But assigning false is not allowed because, well, you said it would be a string and a string is not a Boolean.
[15:54] Make sense so far? >> Yes. Thank you.
[15:57] >> Awesome. There are two things, actually three things that I want to call out here.
[16:01] One is that, this is why I asked you to have a JS file open on the right at the same time.
[16:07] That colon space string does not get pooped out to your output JavaScript. It's just a TypeScript thing.
[16:13] If you were to try to copy and paste the TypeScript code in the browser, it wouldn't work because JavaScript has no idea what a type annotation is.
[16:20] >> Got it. >> That's what we mean when we say it's a superset,
[16:26] that it's JavaScript plus things like type annotations. But if you turn it into JavaScript,
[16:30] those type annotations get removed. The reason that we would want to do it with
[16:37] a type annotation is because it will help define it as a string and not do, but we could still do multiple strings like my name delayed could be Jen.
[16:50] It's starting to make sense. But if we left it undefined,
[17:02] undefined, there we go, that's the word. Then it could have been anything.
[17:10] >> The type terminology would be something like untyped or implicitly typed. But the technical term for this specific scenario is
[17:21] actually the perhaps slightly convoluted name, evolving any. Meaning the variable starts off as the type any,
[17:30] which means any type in the universe. I have no idea what it is.
[17:33] That's the TypeScript term. Then later on, as you assign values to it,
[17:38] TypeScript will know what type it is. If you were to hover over it on line 8,
[17:42] TypeScript would know that it's type string. If you were to hover over it on line 12,
[17:47] it would know that it's type Boolean. It's an evolving initially any variable.
[17:53] >> What? Okay. >> TypeScript is smart.
[17:57] >> Okay. >> That's what I'm going with.
[18:03] Anybody in the beautiful humans watching and listening have questions? Also, hi, homie.
[18:13] >> Hi, homie. >> Yeah. In Simple Sphere,
[18:23] definitely let us know if you have questions because I may not know the questions to ask.
[18:29] If anything comes up, please let us know. Oh, look, it's Anthony.
[18:37] What up, Anthony? We were talking about you before we went live, just as a heads up.
[18:44] We were talking about a lot of you actually. Ben, we were talking about you.
[18:50] Homie, we weren't talking about you, but I talk about you a lot.
[18:54] I get excited when it's like return people. Because I'm like, "Yay, we're making a crew."
[18:59] We got the beautiful human crew. That's like everyone in the world,
[19:02] but we're slowly building out this crew. >> The cream of the crop, the best of the best.
[19:08] >> Exactly. Okay. We got one from Anthony.
[19:17] "How many types could a TypeScript type if a TypeScript could type scripts?"
[19:22] Wow. Thank you. >> Even if a TypeScript could type scripts,
[19:25] a TypeScript could type all the scripts that a TypeScript could type,
[19:28] but a TypeScript can't type scripts? I think that's the canonical answer to that question.
[19:34] >> I like Ben's answer too. >> Yeah. Ben said 12, maybe 42.
[19:43] Who knows? Okay, dope. This is definitely making a bit more sense now that we've used that.
[19:55] But where do we end up moving from here? >> I want to actually make that a little bit
[20:01] up to you and confirm with you. My guess, and please tell me if I'm wrong,
[20:05] is that you're starting to see how the type system works. TypeScript knows what types things are,
[20:10] you can say what type something is, and if you add a different type, it yells at you.
[20:14] But this isn't looking super useful yet. We haven't shown any bugs that would be caught.
[20:18] It's just, "Okay, I guess we can do that. Why would you bother?" Is that right?
[20:21] >> Yes. I think just knowing, seeing something that even if it may not make sense yet,
[20:33] where you would use it, but actually seeing how something may be made with it,
[20:42] other than just like, "Hello, world." >> Sure.
[20:46] >> The canonical first thing that a lot of people do with TypeScript is a greeter function,
[20:52] which takes in, let's say, a name. Then we'll like, "Hello, name."
[20:59] Like in a lot of the older TypeScript examples, they used to use greeter functions and greeter classes.
[21:04] Let's say we want to, who do you want to greet? Give me a name. >> Beautiful human.
[21:11] >> Beautiful human. Awesome. So right now,
[21:17] I have a TypeScript setting enabled called no-one-must-hit-any, which says you have to give me a type on
[21:22] anything that I wouldn't immediately be able to tell the type of. So just looking at the code,
[21:27] we're going to have to give a type to name the parameter. So just off the top of your head,
[21:33] what would you guess the type for a name to be? What would I put after the colon space?
[21:37] >> String. >> Yeah. Awesome. Just checking. That is correct.
[21:41] So let's say that we refactor this function. Let's say that instead of calling it greeter,
[21:46] which takes in a name string, we instead take in first name,
[21:51] string, and then it all splits across lines, then last name, string.
[21:58] Now, TypeScript is yelling at us because we've refactored our code, we've changed it, but not all the callers of that code are updated.
[22:06] Specifically, two places are complaining. One is that your console log still refers to name,
[22:12] which interestingly actually is a global variable that exists, but it's deprecated.
[22:18] So on my screen, it has a strikethrough on it, and I don't know why in yours it doesn't.
[22:22] >> It has the dots. Let's see. >> Oh, there we go.
[22:26] >> Oh, it is. Okay. This one, no, go back.
[22:33] >> There we go. So that's a TypeScript complaint. TypeScript is yelling at you,
[22:38] expected two arguments, but got one. So you can imagine if you have a function that's used in a lot of places,
[22:43] and you change the function signature, meaning what it's called with and/or what it returns,
[22:48] it would be real nice to know all the places that complain. So in this case, you can change it by,
[22:53] let's say, firstName, beautiful, lastName, human. Then firstName, lastName.
[23:01] Does that make sense? Seem reasonable so far?
[23:05] >> Yes. >> Cool. Also, I just want to emphasize on the right,
[23:11] it's the same code except no colon space string is anywhere in the JavaScript because that is a TypeScript thing.
[23:18] >> Right. >> I can see the wheels churning in your head. How does this feel?
[23:26] >> It's making enough sense, something that I've realized from the very beginning.
[23:32] I'm pretty sure Anthony has probably yelled at me to do, but I'm finally going to do it,
[23:37] is creating shorter videos of understanding it and redoing it myself. At the moment, it makes sense,
[23:45] yet in the big picture of things, not a 100 percent,
[23:51] but it makes enough sense to follow along. >> Okay. Cool. I want to bring up then a few topics that build on this,
[24:02] and then we'll also introduce something called a union type, which sounds weird and different,
[24:08] but it's actually really applicable and cool in programming. >> Yay.
[24:12] >> I'm going to make a variable let greeted, and then let's say that instead of greeter console logging the message,
[24:20] it const message equals, it creates the message,
[24:24] and then just also, let's say returns the message in addition to console logging it.
[24:30] TypeScript then knows that this greeted variable is type string. But we never actually explicitly told TypeScript
[24:38] anywhere that the function returns string, and then this variable is type string.
[24:43] TypeScript just knows this function happens to return string, and knows that by reading the contents of the function and seeing the return message.
[24:50] Then greeted is a variable whose value starts off as the result of that function. If you were to hover on line 10 over the name greeted,
[25:00] you again would see greeted string. Does it make sense that TypeScript would be able to figure that out,
[25:06] and that that would be a reasonable understanding? >> Is greeter a normal function?
[25:17] Therefore, that's why it's able to read it. Or if I said,
[25:22] is there another function we could use to replace greeter for another example for greeter and greeted?
[25:32] >> Sure. Let's say you wanted to do like let very greeted, or like name upper equals gen.toUpperCase.
[25:47] TypeScript knows that toUpperCase on the string is a string method that returns a string. The variable name upper would then be type string,
[25:56] even though you've never explicitly said, "I must put a string here."
[25:58] TypeScript just reads your code and understands. >> Got it. Then Ben said,
[26:04] "In really big projects, you'll often find yourself exporting files from
[26:09] one file and importing them and using them in other files. Because of that, you'll often have
[26:15] less visibility whenever the function signature changes." This red squigglefication is really good for seeing
[26:25] how changes propagate throughout the code base, so you don't miss any places you need to fix it,
[26:33] and then should be exporting functions from one file. Is TypeScript more helpful also in classes and that type of thing then?
[26:49] >> Side note, I like red squigglefication as a term. That's a really good-
[26:55] >> I do too. >> Yeah.
[26:56] >> I feel like we just need to keep that forever, what red squigglefication.
[27:02] See if I can even say it. >> Red squigglefication. It's a good one.
[27:06] >> Definitely. >> I won't say that TypeScript is more helpful when you have classes.
[27:10] I would say TypeScript is similarly or also helpful when you have a lot of classes.
[27:15] TypeScript doesn't care if you're using traditional object-oriented programming or a lot of classes,
[27:21] or if you're functional and use a lot of functions. It does the same logic no matter what.
[27:26] Classes, it lets you define what the members are supposed to be and what the methods are supposed to take in and return.
[27:33] Same thing with functions. You can say what their parameters are supposed to take in and be,
[27:37] and then you can also say what types variables are in both worlds. Either way, TypeScript red squigglefies whenever you mess up.
[27:44] >> Got it. Hello, Bernie. How's it going?
[27:53] Thank you for joining and let us know when you have questions. It's sinking in. It's sinking in.
[28:02] >> Okay. >> It's getting there. It's getting there.
[28:04] >> Cool. Let me show you a function then that is copy all or comment all this. Let me show you a function that has an optional parameter.
[28:13] Function greets name maybe, which takes in a full name that's supposed to be a string.
[28:23] Hello. Full name that to uppercase. Now, what if you're supposed to change this later on?
[28:37] Say it worked well for a while, but then later on we're refactoring it.
[28:43] We're supposed to be able to call it with undefined. Suppose this is intentional.
[28:49] Maybe this is supposed to, I don't know, to do different behavior if full name isn't provided.
[28:59] Well, per the red squigglefication, TypeScript is now bad at us because we expected one argument and got zero.
[29:08] There's a way in TypeScript plans. Oh, yes. Thank you. There's a way in TypeScript plans to mark a parameter as optional,
[29:15] and that is to put a question mark before the colon for the parameter that says, I might not provide it,
[29:22] but if I do, I should provide it as a string. But now we have a complaint here from TypeScript because we have said that,
[29:32] full name that to uppercase is going to happen, but full name might not exist.
[29:36] Could you actually do me a favor and hover over the full name that's got the red squiggly on there?
[29:40] Yeah. TypeScript is yelling at us, rightfully so, because it sees that we are calling a method on
[29:46] a value that might not be defined, it might be undefined. This is the concept of a union type.
[29:52] The full name parameter inside the function is either a string or undefined. If you were to hover your mouse over it,
[29:59] you would get the colon space string or undefined, which you saw when you're hovering over there.
[30:06] A union type is an either or, it's either of those possible things.
[30:11] TypeScript knows that if you call a method on a union type that includes, say, undefined, that might cause a crash because it might be undefined.
[30:19] >> Does that seem reasonable so far? You look happy. >> Yes. It's clicking more.
[30:32] It is clicking more. >> Awesome.
[30:36] >> What up, Bakari? >> Hello.
[30:40] >> Hello, world. One of the ways you can work around union types giving you complaints is by fixing the code.
[30:49] This code is legitimately broken. If you were to run this file,
[30:52] you would get a crash. Something like two uppercase of undefined or some complaints.
[30:58] What you can do is you can introduce logic in your code. Let's say if full name,
[31:04] otherwise do phone who this or something. Now, notice that here TypeScript is no longer complaining.
[31:12] Before the if statements, the if block, whatever you want to call it,
[31:16] full name is type string or undefined, but inside, it's just type string.
[31:20] This is because TypeScript is smart. It reads your code and it knows this if statements,
[31:25] if block, whatever that starts on line 4 is only going to get run, the contents are only happening if full name is defined,
[31:32] if it's truthy, which means there's no way that line 7 could crash
[31:37] because full name is definitely string and not undefined. We have narrowed the type,
[31:42] that's the key word, type narrowing to be just string. How does that feel?
[31:48] >> It's sinking in. It is sinking in. >> It's sinking in and full names in this function.
[32:04] >> I would plus one that. Hover your mouse over where full name is and see that inside
[32:09] the if it is string and then outside it's string or undefined. TypeScript has evolved a better understanding of the type,
[32:18] it's narrowed it down. >> Okay.
[32:29] >> Actually, if you hover inside the else statement, it would say string or undefined because that else still
[32:36] happens even if it's undefined or if it's the blank string. Fun fact, I actually have a pending pull request,
[32:42] an issue open against TypeScript so that it would say blank string or undefined in the else
[32:46] because that's technically more accurate, those are the only two values it could be.
[32:51] But it's blocked on, well, we don't know why this would actually be useful to anyone.
[32:55] If you have any bugs in your head that you can think of, let me know, but otherwise.
[32:59] >> Sweet. >> Still works.
[33:00] >> Thank you. >> That's a union type and
[33:06] type narrowing and optional function parameter, all rolled into one example.
[33:10] I will tell you that I have seen and caught legitimate production bugs in code when
[33:15] converting to TypeScript on this exact type of thing, where people assume that something is always going to be defined,
[33:20] but actually they sometimes provide null or undefined. This is so common in industry that it's actually got a term.
[33:27] This is what's called the billion-dollar mistake. Have you ever heard of this thing?
[33:32] >> No. >> Oh my God, I love it. It was coined by Tony,
[33:37] I don't know how to say his last name exactly, H-O-A-R-E, someone from the early days of,
[33:44] I forget if it's C or C++ or what. But the idea that you can provide a null value to something that's
[33:50] supposed to be taking in like a real thing, has caused so much pain and
[33:55] bugs in the industry that he thinks it's been over a billion dollars of damage.
[33:59] TypeScript actually solves the billion-dollar mistake. It doesn't let you provide
[34:03] undefined where you expect something like this term. >> Okay. Yes, maybe, yes.
[34:14] We do have a question. Why to put full name in line 2,
[34:20] and it's to call the full name in the above string, right? It's so that way it asks for this?
[34:28] >> I just put it there so that it's somewhere you can hover your mouse over.
[34:30] They don't actually do anything. We could comment them and it wouldn't change anything.
[34:35] >> Good question, Barry. >> Good question.
[34:38] >> Glad you asked. >> Yay.
[34:48] >> Okay. >> Now, I'm going to do it to the rest of it.
[35:04] So it'll still work if we get rid of all of these. >> Yes.
[35:10] >> I apologize for not explicitly calling that out. They don't do anything.
[35:14] >> Okay. Makes sense. >> Yay.
[35:20] >> Okay. >> Yay. So there are three topics that I think
[35:25] are the crucial important thing for understanding TypeScript. One is that it's a superset of JavaScript,
[35:31] that what you're working with here is JavaScript with a little extra stuff added on.
[35:35] But when you compile it down to something that gets run on your actual app,
[35:38] it's just the JavaScript contents. The second thing is the concept of type checking,
[35:45] that TypeScript knows what types things are, and it can form things called union types
[35:51] when something could be more than one value, which then lets it know to tell you to narrow it
[35:55] down before calling it as just one of the values. Do those make sense and seem reasonable so far?
[36:01] >> Yes. >> Cool. I like this also.
[36:04] That is a treasure trove of good phrases. I was going to put seasoning.
[36:10] >> All right. >> Awesome.
[36:13] >> Is this when things get spicy? >> This is when things get spicy.
[36:18] More seasoned developers using. The third concept is the concept of an interface or type,
[36:24] an object type. Let's say that you have a let my value or my poet. I shamelessly copy and paste it from my book,
[36:33] and my book each chapter is like a different name of things people do.
[36:37] >> Perfect. >> Let's say you have a poet and the poet's shape is,
[36:44] actually, I'm just going to copy a full variable, is this. TypeScript can then not just tell you when things are wrong,
[36:52] but also give you utilities in development time because it knows things about your code.
[36:56] For example, it knows that poet. It only be completed with born in name.
[37:02] Actually, can I ask you to type out poet. It's on a line so that we can see on your screen,
[37:09] the suggestions that it comes up with? There you go. This is another answer to why is TypeScript useful?
[37:16] Because TypeScript can help you develop. TypeScript knows that it just has born in name.
[37:21] Voila. >> Okay.
[37:29] >> Was that your next curiosity of does born have other things on it that TypeScript would know?
[37:33] >> This may be me not knowing JavaScript enough too. How would you put both there if you would just put poet?
[37:46] Never mind. I answered my own question. That's exciting at least.
[37:50] That does make sense. >> Cool. Actually, I like what you're doing before.
[37:55] Could you click or type period again? Yeah. TypeScript knows what exists on, say, numbers.
[38:02] Born is a number of poet of born is 1935. It knows that numbers just have these methods,
[38:08] most of which I have never used in my actual code, but two fixed is a thing you can do on numbers.
[38:14] Fun fact. If you do poet.name, it'll know that name has two uppercase to lowercase trim and so on.
[38:23] >> There's a lot of options here. >> Yeah. Fun fact, JavaScript strings actually have a lot of features,
[38:32] including things that turn them into HTML, or like return an HTML version of them.
[38:37] >> Yeah. Interesting. Okay. Yay. >> Awesome. Do me another favor though.
[38:55] Can you right-click on name on line 7? In the middle of that menu where it says "Rename Symbol",
[39:04] click that, and call it whatever you want, something other than name.
[39:10] When you're done, hit "Enter". >> That was cool.
[39:16] >> Yeah. Notice it did it in two places. It did it on the poet variable on line 3 and on line 7.
[39:23] >> Now I want to go try it here. >> Yeah, yeah. Go ahead.
[39:30] >> Okay. That works too. Look at you being fancy.
[39:38] Could I rename symbol? >> Yep. Fold gen.
[39:51] >> I was going to do it. I really was, but figured I shouldn't do that.
[39:59] Yay. Okay. That's actually really cool, and you can't do that in JavaScript.
[40:05] >> The thing that lets you do that is TypeScript. TypeScript reads in your TypeScript files
[40:11] and understands things, it understands where they're used, where they're declared.
[40:15] Actually, you can do it in JavaScript in editors like VS Code, but it's TypeScript powering that.
[40:21] It's more powerful and more reliable when you do it on TypeScript files,
[40:27] but to a limited extent, you can't do it in JavaScript.
[40:30] >> Interesting. I feel like this alone, it gets me way more excited about TypeScript.
[40:36] >> Yay. >> Like this one feature.
[40:40] >> I think people oftentimes get really hooked into the really cool powerful things you can do in TypeScript,
[40:45] but the actual benefits of TypeScript that are important and critical for day-to-day developments
[40:51] are that it will find your bugs for you, it'll give you utilities and
[40:54] helpful suggestions when you're writing code, and it enables a lot of really powerful automations
[41:01] from renaming things or refactoring code. I'm going to do a refactor here.
[41:08] You can't see it on your screen, but in mine, I just extract it to a function named log thing.
[41:17] That TypeScript just did that for me. I selected the line and I selected
[41:22] the refactor new function and it took it in. Yay, TypeScript. The language server,
[41:28] which is the tool that VS Code runs, gives us all these awesome things.
[41:32] >> Okay. Very cool. This is exciting. I like it. >> Yay, I'm glad.
[41:42] >> I feel like this is to you and anyone else that builds coding books. I get that a lot of the code,
[41:54] you actually have to read it and then do it on the computer. So not always would make sense as an Audible book,
[42:02] but I would really appreciate it as an Audible book because that's how I learn is to be able to hear it,
[42:10] and then it helps me stay along with it. I know that there are tools that you can actually have it read the specific page.
[42:24] I'm very lazy because then I have to wait for every page to go through and click it every minute.
[42:30] Anyway, I'm saying that in the fact that I have not read your book, even though I really want to,
[42:35] is there an exercise when we get through done today that you have in the book or that you would suggest as a good practice to follow up on these for next time?
[42:47] >> Yeah. Actually, two notes on that. One, I agree.
[42:51] Although I personally learn best for blog form, blog posts, and docs, and books.
[42:56] I know a lot of people are video-based. If you want a good recommendation for someone who has a video course,
[43:03] I'd say Matt Pocock. I will post that in the chat once I get my Chrome in order.
[43:10] There we go. This person has really good content, is one of my favorite TypeScript people.
[43:15] Highly recommend. They're awesome. That's one thing. I'm also a big believer in hands-on learning.
[43:28] I like the long-form blog posts, but then I also have to do it on my own.
[43:31] Otherwise, it's all theory and it doesn't stick. Every chapter in learning TypeScript,
[43:35] the book, ends with a note to go to learningtypescript.com, the website, and do one of the 1-3 practice projects on the website.
[43:43] I've got practice projects for every chapter on the book that exercises just what's in that chapter and maybe a little bit of
[43:49] what you've already learned prior to that chapter in the book. It's all intended for people who may not have any TypeScript experience prior to the book,
[43:58] but do know some foundational JavaScript. >> Ta-da.
[44:03] >> Yeah, that's the thing. >> That's the thing. It's actually funny enough,
[44:08] when I was going through this, prepping for our call and stuff,
[44:12] I was like, maybe it's on Amazon or maybe Google Play will read it to me. I was like, no go.
[44:19] Yet, I am very excited about this. Yay. There are the things.
[44:26] >> All thematically terrible. I apologize in advance for the themes.
[44:33] >> No, no, no. I really like the names. >> Yeah?
[44:37] >> No, I like these. I really like these because they're amusing. They are very amusing.
[44:47] There's a hub. Look at this. I'm also showing this as one thing that I really like
[44:57] about when people set up pages like this is I can still read it. It's not something that I have to get the physical book for.
[45:06] It's like, okay, cool. I can. Ben and I looked into screen readers,
[45:13] which as an update, Ben, I have used my screen reader when my text-to-speech decides to glitch out.
[45:22] Thank you for showing me that. But I'm excited to go through these.
[45:26] Now, do you think we've gone through enough to cover what's in the Typeinator? >> We do. We have. I do.
[45:39] The Typeinator doesn't actually introduce any TypeScript stuff. It just has you refactor things from old JavaScript to
[45:46] modern JavaScript in preparation for getting excited about what TypeScript gives you. I'd say the first TypeScript project is System of a Clown,
[45:54] one of my favorite themes. That one, I believe we've pretty much gone over enough of.
[46:01] Yeah, we could do that. >> Okay. Because I feel like we have two options,
[46:09] and I want to let the audience pick for us because we do have the time. Yet, should I do a video doing this and talking us through it just like solo,
[46:22] or should we do it now and hang out with Josh as I stumble through it? Votes for stumbling through it now or video later.
[46:33] Those are your two options, everybody. Josh, you can have a vote too because it is your content as well.
[46:41] Thank you. You read my mind. >> I'm doing it now.
[46:44] >> All right. >> There are enough projects there.
[46:46] You can always stumble through one now and also stumble through one on your own later if you want.
[46:52] >> Perfect. Okay, cool. I like it. I think I get embarrassed and shy about it because I'm like,
[46:59] I just want to listen to it really quick and nobody else, so I'm just going to awkwardly listen.
[47:04] But that's okay. It's fine. It's not very long. System of a Clown.
[47:17] Yes, I'm reading to myself because I don't want to read out loud. All of you, but the link, they have linked it.
[47:24] Thank you, Josh, for linking it. Look, you made it so easy.
[47:35] >> I got you. I will say though, that copy button is a UI bug.
[47:40] It should be floating off to the right and styled, and I can't figure out why it's so unstyled, but it still works.
[47:47] >> I thought it looked nice, but that could be.
[47:51] Hey, Anthony, are you still here? Because I just realized I think I have everything,
[48:02] for the most part, re-installed on my computer, but I don't know if I do.
[48:07] Do I have node and everything re-installed? Did I ever do that?
[48:16] Like when we did? For everyone that wasn't there for this very random day,
[48:24] I had a hard reset my laptop, and Anthony and I were re-installing stuff.
[48:32] Okay, I'll look really quick. I don't have node. >> That's the most annoying thing to have to
[48:37] go through and re-install everything. My condolences.
[48:41] >> Is this still going to work without node? >> Yeah, it should work.
[48:49] >> Okay. >> Yeah, you'll just have to do everything through VS Code,
[48:52] but you'll get the squiggles, the red squigglies if you mess up,
[48:56] or you'll have the red squigglies in places that need to be fixed. Yeah, it should all work.
[49:01] >> Okay. But I can still download it and everything through Git? I think so.
[49:09] >> Yes. >> What?
[49:10] >> Did it not, what? >> Oh, I don't know if it copied and I put red.
[49:17] No, it did red squigglification. >> That's unfortunate. Well, you only need to run the first two lines,
[49:25] I guess, that you can just copy manually, I guess. That's upsetting to me.
[49:31] >> Well, it was also pasting red squigglyfication. >> Yeah, I'm going to file a bug in my site.
[49:41] >> See, this is useful for me because now I'm just doing user research at this point.
[49:45] Next question will be, on a scale of 1-10, how likely are you to recommend this to a friend?
[49:51] >> To everyone. Okay. Change your terminal directory.
[50:01] Totally did it wrong. In the fact that I skipped a step, that I thought I didn't do NPNI.
[50:14] >> You don't have to do NPNI. That's okay. You can just open this in VS Code and it should be fine.
[50:18] I wouldn't worry about it too much. That would be nice to have those things running,
[50:22] but you don't need it. I can just walk you through it now.
[50:25] >> Okay. Let's see if code.works. >> What?
[50:32] >> You don't have code? >> Where did my VS Code go?
[50:38] Did I close it? Close it? I don't think I closed it. No.
[50:43] We might be back to where I was a while ago. This is fun. >> Yay.
[50:57] >> Yes, trust. >> Okay. We have the project.
[51:06] Steps. Notes. Don't import code from one step into another.
[51:27] We got this here. Let me make these bigger and then I will.
[51:39] Everybody should have the link to follow along as well. It was scrolling to steps. That's where we're at.
[51:51] [inaudible] repeatedly creates groups of five to 10 guests. Each group is directed to go to an activity,
[52:04] which can hold a certain number of them at a time. It looks like the clowns didn't change too much on this one.
[52:11] They mostly just removed a few type annotations and changed one value. Could you please add back missing type annotations,
[52:21] avoid implicit, and fix the wrong value? Fix the code here and then solution code.
[52:36] I need to go find the code to fix. I'm guessing it was this one?
[52:42] >> Yeah. >> Wait, wait. Come back, come back.
[53:12] I don't. Yesterday was with Laura about Python and she's a previous teacher as well.
[53:29] She loves to watch me struggle through these two. It's my love-hate relationship with teachers.
[53:35] Because of course, this is what I'm going to learn, but I'm definitely going to second-guess myself on all of it.
[53:41] >> Sure. What interaction mode are you looking for here? My default is to just be quiet until
[53:48] you yell at me that this is not making sense. Would you like me to be a little more proactive and give hints?
[53:53] >> No. I'm also thinking that it can't be applied to types, number, and string,
[54:02] which makes me think it can only be one or the other. I'm just going to struggle along and see what happens.
[54:14] >> Can I suggest going to where capacity is declared and seeing what it is?
[54:21] Which fun fact, you can do by right-clicking on it and then selecting "Go to definition" or "Command" clicking on your Mac.
[54:28] >> That's cool. I do something string.
[54:39] Equal string? Is it equal string? >> This is, if you've gone through like npm install,
[54:47] I think you might be getting squigglies indicating. Yeah, these lines 6-8 are where I would suggest starting.
[54:53] What types do you think each of these variables are supposed to be? >> Numbers, because we have a new comment coming in.
[55:15] Hi, by using TS, please don't use any.
[55:20] >> Yeah. In general, in TypeScript, you don't want to use any,
[55:23] you want to have more specific types. Sometimes they're like weird edge cases
[55:27] with wacky logic where it's hard to avoid any, but for the most part, yeah,
[55:30] it's better to have actual types, not the YOLO, I don't know what I'm doing, any type.
[55:35] But yeah, I liked what you said before. I think capacity being a number is totally reasonable.
[55:41] The syntax you're looking for is colon space number, saying eventually this will have a value,
[55:46] and eventually that value will be number. >> That one? No.
[55:54] >> Yes. But you added a semicolon instead of a colon, a semicolon.
[55:59] >> That would help, right? >> Yay.
[56:03] >> Which means these need to be fixed into numbers. >> There you go. Yay.
[56:17] >> Was that it? >> That's it.
[56:19] >> Yay. >> That was the most complex one. You did it.
[56:23] >> Okay. Exciting. >> Excited. Because this one I think would be string.
[56:35] >> Yeah. >> I don't know what the Boolean,
[56:47] is it called Boolean? >> Yeah, it's Boolean. In the book,
[56:50] it mentions there is number string, Boolean, null undefined, big int, symbol,
[56:58] and maybe that's all of them. Those are the primitive types in JavaScript,
[57:02] and thus also TypeScript. Yeah, I think that's the solution.
[57:05] I think you fixed the thing. >> Okay. Let's compare. I can just go double-click.
[57:14] That's sad. Oh, yay. Wait, this is mine.
[57:22] Other than my semicolons. >> Which don't matter at all.
[57:25] >> Bye, Ben. Do they matter in, I don't know. I struggle with my that and commas.
[57:35] I always struggle with it. Oh, yay. >> Oh, yeah.
[57:38] >> This is exciting. >> Actually, can I suggest a really cool VS Code command?
[57:43] I saw you know how to use the command palette. You did the install code,
[57:46] and a different command you can do from the palette is compare active file and the third one with dot, dot, dot.
[57:56] You're right now in index compared to solution TS. It'll show you a diff view between the two.
[58:02] Yep, you have no differences. This is a neat VS Code feature I learned about recently.
[58:17] >> Yeah. >> Oh, this is fancy.
[58:21] This is fun. Anthony said that there are seven primitive types.
[58:31] String number, big int, Boolean, undefined symbol, and null.
[58:40] What's big int? >> It's like a number,
[58:44] but they can't have anything like zero point, whatever. It's just integers.
[58:50] It's used for math primarily. >> Because Python has something integer like that,
[59:06] but it's for numbers. Cool. Actually, y'all,
[59:11] I just want to say that I learned about Boolean yesterday while learning Python.
[59:16] Yes, knowing what that was. I heard of it, but never did it.
[59:21] I'm excited about this. I feel like I can make headway on this now.
[59:29] You have the virtual version of the book, right? There's an e-book version?
[59:43] >> Yes. O'Reilly's platform has a native e-book thing, and I want to say you can also get
[59:50] it as an e-book on Amazon and Goodreads and stuff. Side note, I personally have been
[59:54] trying to do more independent bookstores, and it really pains me that for mainstream programming books,
[59:59] your local indie bookstore isn't going to have it. If anyone knows a way to get it that isn't
[60:02] through Amazon or equivalent, please let me know. But in the meantime, yes,
[60:07] Amazon, O'Reilly, et cetera, do have e-book versions. >> Because then I feel like I could do the next one, possibly.
[60:16] I'll struggle through it, because show up and hide it in the corner stores.
[60:23] >> Genius. >> There you go.
[60:24] >> Put a little request in. >> Yeah, I don't see a lot of bookstores that have,
[60:30] as you're saying, a lot of technical books. They normally have everything else.
[60:37] >> Yeah, I can't blame them. The cycle of books is pretty rapid.
[60:42] In two years, this book will either be out of date or need to have a second edition.
[60:46] There is already a new TypeScript feature coming out that satisfies keyword.
[60:50] That's something I would absolutely put in the book if this book had come out before or after that feature.
[60:57] >> Okay. >> Yay, software.
[60:59] >> Yay, and I have my homework, and I can't say that I exactly understand TypeScript
[61:07] in the fact of what are all the differences, but I at least see some cool features
[61:13] and have some exercises to work through and learn from, so thank you.
[61:19] I appreciate that. That is a big step in the right direction.
[61:23] Oh, we got TypeScript issues. >> That's the new satisfies keyword
[61:29] that's going to be in the next version of TypeScript. They just released a beta/release candidate for it, so.
[61:35] >> Nice, nice, and thank you, Anthony, for posting it, so that way everyone knows what's going on,
[61:44] and I think I'm good for today. Was there anything else you wanted to cover
[61:49] before we start wrapping up? >> No, I feel good about this.
[61:53] We've been on almost exactly one hour. I think what I normally do is I'll end with my summary
[62:00] and then also suggest that you rephrase it in the way that your personal brain works,
[62:06] so my summary of TypeScript is that there are three main things we looked at.
[62:10] We saw that TypeScript files get turned into JavaScript files, which are almost the same.
[62:14] Any TypeScript-specific syntax gets removed, but otherwise they're the same.
[62:19] The second is that TypeScript looks at your code and understands what types the values are supposed to be,
[62:24] so if you, say, make a variable and then later on assign a different type of value,
[62:29] number instead of string, TypeScript will yell at you, and that's really useful because if you have a function
[62:33] that took in one parameter and then you refactored it to take in two parameters,
[62:38] TypeScript will yell at you to fix all the places that call it, and then the third thing is that TypeScript
[62:42] has nice dev tooling, things like rename and refactor that it can do for you
[62:47] because it knows the types of all your values in code. Does that all kind of make sense and seem reasonable so far?
[62:53] -Yes. I will say for the first one, I logically get what you're saying about that TypeScript
[63:00] goes to JavaScript and translates. It makes sense, yet isn't completely computing.
[63:10] As, like, examples in my head, I'm not there. And then for the second one, that was the values
[63:21] or being able to rename things. -What was it? Third one was renaming.
[63:25] Second one was, oh, yeah, it'll yell at you if you mismatch. -Yes. I like that.
[63:31] That one, I thought, was a great example of showing how it will yell at you if you mismatch.
[63:37] And then so that actually worked out with the exercise of being able to see where it's going to yell at you
[63:44] and also going to the original one. And then third is the renaming part,
[63:51] and I thought that was really cool. That's just a fun feature that I'm like,
[63:54] cool, if I decide I want to rename all of them at once. I dig it. I dig it.
[64:00] And we know how people can follow you. We've got those linked in Go Get the Book linked up above,
[64:08] but how do, like, all of us help you in your open-sourceness? -I appreciate you asking that. Thank you.
[64:18] I'm just typing into the chat the three things because I'm already forgetting what they were
[64:22] in order, so, yeah, 1, superset, 2, red-tweakalification. Shout-out again, Ben, who's left for that term.
[64:29] And 3 is definitely features refactoring, such as renames and extracting functions.
[64:35] Cool. Yay. Folks can sponsor me on GitHub.
[64:38] I'm github.com/sponsors/JoshuaKGoldberg. You can also sponsor TypeScript ESLint,
[64:47] which some of that goes to me. Some of it goes to my fellow open-source maintainers.
[64:51] TypeScript ESLint is the tooling that lets you run ESLint, the standard JavaScript linter on TypeScript code.
[64:57] So TypeScript comes with a lot of really good checks, but it doesn't, say,
[65:01] let you define a custom rule that yells at you if you use a deprecated API or anything like that.
[65:07] Like, that would be what a linter does. Lastly, I'm also on Twitch,
[65:12] and I'm actually streaming in an hour and a half, a little bit less, later today.
[65:16] So I'm Joshua K Goldberg on Twitch, GitHub, Twitter. You can follow, like, subscribe,
[65:20] whatever, in all of those places. - Do it, do it.
[65:23] Subscribe to all the channels. Subscribe to his channel, subscribe to my channel,
[65:26] subscribe to them all. If only we could, right?
[65:31] I would totally dig it. Awesome.
[65:33] And I've already talked to Josh. Try to convince him.
[65:38] Come back again. Teach us all the things.
[65:41] Teach us all the things. I'm also excited to start working through the book, too.
[65:46] So, and yeah, I think that is it. Make sure to, thank you, Anthony,
[65:55] for putting up his Twitch. I always just figure people would just click on your bubble.
[66:00] I don't know if that's, like, a thing, if people click on people's bubble
[66:05] to, like, go see what they're up to. - I do that, but yeah, thanks, Anthony.
[66:09] Appreciate it. I forgot to. - Yes, yes.
[66:12] Agreed, agreed. And yes, so I will see all of you
[66:16] that are going to the Twitter space tomorrow for mental health and neurodiversity and tech,
[66:22] same time, just tomorrow, on Twitter. And last but not least, see you on Thursday.
[66:29] We are going through cool stuff that I don't remember, but I will be back on Thursday.
[66:36] So thank you, everyone. Bye.

