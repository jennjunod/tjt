---
showLink: "https://www.youtube.com/watch?v=7vUtd2JDU5Y"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-3-unions-and-literals"
title: "Learning TypeScript Chapter 3: Unions and Literals"
publishDate: "2023-03-18"
coverImage: "https://i.ytimg.com/vi/7vUtd2JDU5Y/maxresdefault.jpg"
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

[00:00] We're live. - Yay.
[00:02] Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:07] And today, if you haven't been a part of these streams yet, we are learning TypeScript with Josh Goldberg.
[00:14] Yay. - Yay.
[00:16] - And Josh, who are you? What do you do?
[00:18] What are the things and stuff you've been up to? - What is my name?
[00:22] What do I know? Do I know things?
[00:24] Let's find out. I'm Josh.
[00:26] Hello, I'm a full-time open source maintainer in the TypeScript ecosystem,
[00:30] which means instead of having a real job like you, I work full-time on open source tools.
[00:36] Most of my time is spent on TypeScript ESLint, the tool that lets you run
[00:39] a lot of standard JavaScript tools and TypeScript code like ESLint and Prettier, both great tools.
[00:43] And then I also run like a few smaller side projects that I'm trying to get bigger in my spare time.
[00:48] I also just became, by the way, a Microsoft MVP, which I still don't know exactly what that entails.
[00:54] It's for people who share with the community, do stuff like this, which makes me happy.
[00:58] So yay. - Nice.
[01:00] I was gonna ask what it means, 'cause I wasn't sure. I just was like, this seems prestigious.
[01:07] Yay. - I think it is.
[01:09] It's nice. I like a lot of people who are MVPs.
[01:11] They seem great. So I'm happy to be here.
[01:14] - We should ask Microsoft. Yo, what's it mean?
[01:17] Come hang out with us. Now, I will say something that I'm excited about
[01:22] is you mentioned earlier about some of the projects you work on.
[01:29] And for those who are wondering about the difference between linting and formatting,
[01:34] we talked about that on our last stream. Like we spent a solid while on that.
[01:38] So go check it out if you are curious. I can link it eventually.
[01:43] I do need to still put these in a playlist for us. I've been neglecting.
[01:51] Something that you asked about right before we went on stream was,
[01:57] how is the new job? - Yeah.
[02:00] - I got the job. - Belated again, congrats.
[02:02] - Thank you. Thank you.
[02:04] I currently now work at Ivan, which is a data infrastructure company.
[02:09] And it's interesting because I thought like, nobody specifically said this,
[02:18] but I thought I was gonna have to quit streaming for some reason.
[02:21] I just thought I was gonna have to quit streaming. I was like, I got a job.
[02:24] I gotta quit streaming. And they're like, no, Jen,
[02:27] you gotta continue to learn live. That's why we hired you.
[02:32] This is me paraphrasing by the way, but I was like, yes, this is great.
[02:37] Thank you, Bakari. And hello, hello.
[02:40] Yes. So I will be continuing to learn live.
[02:44] I will still, the biggest changes is that there's gonna be a lot more structure
[02:50] to teach Gen Tech. Other than, you know, MISC Mondays,
[02:56] Python TypeScript, and working with Distribute Aid on Thursdays.
[03:01] The other two days are basically all gonna be about data infrastructure
[03:04] and learning how to make, how to create Postgres.
[03:12] What is data? Like that's next week's stream.
[03:15] I'm actually really excited. This week, we went over Kafka,
[03:19] which is a database type that does some things and stuff.
[03:24] I say it like that because I'm like, I feel like this is how people feel about TypeScript
[03:30] because this is how I felt about TypeScript when I first started learning about it.
[03:34] It's using itself. So hopefully it'll get better.
[03:38] And yeah, and there's a kitty. - I'm not doing this intentionally.
[03:44] If I don't do this, he will cause ruckus. Yeah, Kafka is cool.
[03:48] I've been meaning to look into it. Is there like a TL;DR you can share
[03:52] of what Kafka actually is for people like me who know nothing?
[03:55] - There will be in the future because I don't quite understand it yet.
[04:02] Because this is something that I've realized I enjoy yet can be difficult when I'm doing the live streams
[04:08] is I do something very, very difficult that I don't get at all,
[04:12] but it helps conceptualize long-term. Just kind of makes it a little tricky
[04:17] if you are trying to start from scratch. And your cat reminded me that y'all,
[04:26] my doggo has a UTI at the moment. So she decides to wake up and has to go.
[04:31] I get to take her out really quick. So hopefully we don't have any of those interruptions.
[04:37] - I'll have to be making bad jokes and puns the whole time while you're gone.
[04:41] You don't want to have that for the stream. You'll lose all your followers.
[04:44] - No, I won't. That is why I, and actually this is a big reason
[04:48] why I like learning this book with you, A, because you answer my questions, but things are punny.
[04:54] And we have cat purrs in the background. - Your occasional growl of frustration.
[05:01] - Yes, and updates from last time, because we were supposed to have one stream
[05:09] between last time and this time, but I started the new job, so it didn't happen.
[05:14] But Josh's eyes are so much better. They're not red.
[05:18] - No more giant bloodshot. I look like I've been in outer space or something.
[05:24] Death looks, it's great. I can see without glasses.
[05:27] I don't need to constantly squirt I single use preservative free eye lubricant in there,
[05:31] which is surprisingly refreshing. It's good stuff.
[05:35] - How long did it take for the redness to go away? - Slowly over two, three, four weeks.
[05:42] Really, by a month, it was almost completely gone. - Interesting.
[05:46] I just happen to have contacts in today, but normally I have to have my glasses on.
[05:51] But I still, I don't wanna give up my glasses. I like my glasses too much.
[05:57] - I liked my glasses within the spectrum of having glasses, but within the spectrum of not having glasses,
[06:06] this is pretty great. I like waking up and being able to see fully.
[06:09] It's pretty great. - Fair enough. That is fair, that is fair.
[06:12] Well, onto the TypeScripty things, the TypeScripty of things and things.
[06:19] Really quick, y'all, just so that way I can bring this up and I want to go here.
[06:25] Okay, let's move this to the screen. Yay.
[06:28] So this link will be in our chat here shortly. This is where you can learn more about learning TypeScripts
[06:36] and you can buy the book, get this book. You have multiple choices on where to get the book.
[06:45] I also say this because like, as somebody that's scared of really big concepts,
[06:51] I can't say I'm scared, but like they make me grumpy. And especially when I'm like, gotta learn it.
[06:58] And then there'll be really dry and boring. Josh is funny and puts all of that fun humor
[07:04] and everything into his books and into the assignments and the projects.
[07:11] But something that is starters new or has starters always been there?
[07:17] - They've always been there. I just haven't changed them since the book came out
[07:20] since no one's asked for any new ones. So I don't know how useful they are to the majority,
[07:24] but I like them. - I feel like for some reason,
[07:27] today's the first day I noticed them, which maybe I was just super concentrated on the projects.
[07:34] But this is, you can also scroll down to get to the projects, but this is where you can get the book.
[07:41] I have the book, yay. And the PDF.
[07:49] So I will be using the PDF to share with everyone today. So that way you can tag along and, you know.
[07:58] All right, so we learned this really cool trick last time. Whoa, the Tilda.
[08:06] So did I until I was like watching last week's just to make sure I went to the right chapter.
[08:10] And I was like, oh yeah, that was a really cool trick. Although I can't use my mouse anywhere else.
[08:16] That's the only annoying part. But nothing is constant.
[08:22] Values may change over time. Well, except constants.
[08:25] Yeah, and today we are literally talking about unions. (laughs)
[08:34] What up, Papa Smurf? The Tilda, is that what we decided it was called?
[08:39] The thing next to the one. - I'm trying to find it.
[08:45] Yeah, that's the Tilda. My weird windows map keyboard.
[08:50] - I did this last time too. I don't know where it is, but I think it's this thing.
[09:01] (laughs) It's that thing.
[09:04] And we're on Mac just with this PDF viewer and it does this and it's really happy.
[09:09] It makes streaming a lot easier. But something that I do wanna get into,
[09:16] which I don't know if it's possible, using an iPad to do this.
[09:22] So that way I can write notes on the side of it and just stream my iPad.
[09:27] But then have notes that I write in the book next to it. I don't know if it's possible.
[09:34] When I get an iPad, we'll find out. We will find out.
[09:37] Hopefully by-- - I've never owned one. - Never owned, what, how about a tablet?
[09:42] - I have an e-reader, a Nook Glowlight 4E. - Okay, okay, that kinda counts, right?
[09:50] I'm gonna go with yes. - Yeah. - I'm gonna go with yes.
[09:55] Okay. (laughs) All right, so we debated a few
[10:01] before how we were gonna go through this chapter. But beforehand, I think it's gonna be smart of,
[10:09] so what are unions and literals and what made you make this chapter?
[10:17] And could you tell us a bit about it, please? - Sure.
[10:21] If by debated you mean angrily screamed at each other for 47 minutes,
[10:24] it was a horrifying experience. You were really mean.
[10:27] - Really personal. - Don't tell anybody. You're not supposed to.
[10:31] - Sorry. So this is in the concepts, the foundations part of the book
[10:37] which means it's not something that's like a specific thing you might use in some specific scenario.
[10:42] It's a core foundational. You end up seeing this in a lot of places.
[10:46] Unions are the concept of something that could be one of multiple possible types.
[10:51] Like a variable might be a string or undefined. Or an object could be like this shape of the object
[10:57] or that shape or that shape or dot, dot, dot. And that's really powerful because in JavaScript,
[11:02] you can do wild and wacky things. You can create a variable and then 3000 lines later
[11:06] then assign some value to it. What was its type before it was assigned?
[11:09] And then you have all sorts of fun. Ooh.
[11:14] - I tried to make it for you, but it made it on me. You were talking, ah.
[11:19] No, it doesn't work. Sorry, we're just gonna remove this
[11:21] so you can talk and explain the chapter things. Me and StreamYard, we don't understand.
[11:26] - No, I'm trying to figure out if I can do it. Cool.
[11:29] Yeah, so that's really good and useful, the ability to have stuff that's like one of possible types.
[11:34] And then TypeScript also gives you the option to narrow types.
[11:36] Like if you have an if statement, if some variable is defined inside that if statement,
[11:40] you know the variable is not undefined. Otherwise you wouldn't be inside that if statement.
[11:45] So you have the ability to both widen the types and then also narrow them,
[11:49] which brings up a whole other list of cool things you can do.
[11:52] Like things that are a specific number, like a literal zero instead of any old number
[11:57] in the universe. - Oh, that's cool.
[11:59] I didn't realize that. Okay, well.
[12:03] - This chapter goes over it. Yay.
[12:05] - I mean, it does. I feel like this is something that I would say
[12:08] to everyone learning is the best writers and teachers in the world.
[12:14] Things may not click the first time you see them, read them, learn them, go through exercises with them.
[12:20] No matter how many times people tell you about it, it might take a while to click.
[12:26] So I just wanna remind everyone of that. And I think I honestly,
[12:33] I am gonna skip a little bit because we, it's so stuck in my head.
[12:40] And yes, y'all, I'm scrolling, trying to get to this end really quick.
[12:44] - Do, do, do, do, do, do, do, do, do, do, do. Summary.
[12:49] Yay. - Summary. - So the reason we're going to the summary
[12:53] is when I was going through this chapter, I have chatter going on in my head of things
[13:02] other people have told me about TypeScript, which is not accurate or is accurate.
[13:09] I don't know. And it can be very hard for me to move forward
[13:13] with a concept if I don't deconstruct what I previously knew. So what we're going through in this chapter
[13:21] is union and literal types, along with how it's type system can
[13:27] deduce more specific, narrower types from how our code is structured,
[13:31] how union types represent values that could be one or more types,
[13:37] explicitly indicating union types with type annotations, how type narrowing reduces possible types of a value,
[13:48] the differences between cost variable, const. Damn it, I hate dyslexia sometimes
[13:54] 'cause I'm like cost, no, that doesn't make sense. Const variables with variable types
[13:59] and let variables with primitive types. One part I'm looking forward to hearing more about
[14:06] is the billion dollar mistake and how TypeScript handles strict null checking
[14:11] using explicit, undefined to represent values that may not exist.
[14:16] Explicit, implicit, undefined for unassigned variables and using type aliases to save
[14:24] typing long type unions repetitively. I got the numbers. - A lot of stuff.
[14:31] - Yes, all of that to say. So why is TypeScript known to like put any
[14:37] and that you can just put like any for anything and you could just move forward doing that?
[14:41] Why not do that instead of doing unions in literal? - That's a great question.
[14:48] And the question will probably come up in later chapters, especially the next one, chapter four, objects.
[14:53] Any is, to recap, any is the keyword in TypeScript that tells TypeScript to shut up,
[14:58] let me do whatever I want, don't type check me. And thanks, Ryan.
[15:02] That is good if you just need to get something done. If like you're working with some wacky old weird code
[15:09] and there's no way in your understanding of the type system in TypeScript features to describe to TypeScript what it is,
[15:16] or if you're just hacking some stuff together and you don't have time,
[15:19] or maybe it is theoretically possible in TypeScript. You just don't have the 20 bajillion hours
[15:25] to learn enough to get there. Like those are all valid reasons to just tell TypeScript,
[15:29] stop yelling at me, let me do whatever I want. So of course there are people
[15:33] in those legitimate reasonable circumstances and then people who just, for whatever other reasons,
[15:37] just sprinkle an any in there to get TypeScript to shut up and never go back to fix it.
[15:41] So, especially when we get into these more fancy, advanced even, parts of the type system,
[15:46] and I wouldn't, within the spectrum of TypeScript, this is not the advanced stuff.
[15:49] This is like the core foundational good to know. Sometimes it's just easier to use an any
[15:53] and maybe go back to it later once you know how to do stuff. And honestly,
[15:57] I think that's a totally valid learning strategy. You both get to get the code to work,
[16:00] which is oftentimes the most important thing, and you get to experience the pain
[16:04] of not having as good IntelliSense and other development features
[16:07] because you're using an any instead of proper types. - Yeah, and thank you for that.
[16:12] Because like going through this, when I first started reading this of like union types
[16:19] and then going through and then also looking at narrowing, one thing that like came out to me was
[16:32] if you could go into a bit more detail, we have, and I'll just,
[16:37] I keep forgetting that I can do the zoomy zoom. Oh. (laughs)
[16:45] - Yeah. - Thanks, Ryan.
[16:47] I was like staring at it and I'm like, who's cat? Oh, you mean Josh's cat.
[16:52] Got it. (laughs) Unions, expanding a values allowed type
[17:01] to two or more possible types and narrowing is reducing it. So that totally makes sense to me.
[17:08] What doesn't quite make sense, if you could go into more detail
[17:12] of helping me put like two and two together. If in this example, going back to the tilde.
[17:21] Oh, oh, like zoomed in more. - Zoomies of the zoomies.
[17:25] - Whoa. - Is it automatically doing that?
[17:28] - Yes. - What are you doing?
[17:30] - Nothing. I was just like, this is interesting.
[17:35] Okay, well, we'll take this variable. And you go into it that it is a string,
[17:43] but if we're telling let mathematician be math dot random, then I guess I'm a little lost on the difference
[17:55] between union types and strings and why you wouldn't just name it a string.
[18:00] Like it's a, you explain it, but it doesn't click. - Sure, what you're describing is in fact
[18:08] the thing you expressed interest in, the billion dollar mistake.
[18:12] Because, and you should feel good about yourself. The questioning you're giving now
[18:15] is the same questioning the industry has been doing for decades.
[18:18] Because a lot of languages don't make a difference. It is either undefined or string, let's just call it string.
[18:24] And that's actually how a lot of older languages and even still used today languages
[18:28] like C++ and Java work. And C# except they added a new set of settings to fix this.
[18:34] So in like traditional Java code, it's typical at the beginning of any function
[18:40] that takes in parameters to check. If this parameter is null, throw new whatever exception.
[18:46] If that parameter is null, throw new exception. I don't know if your variants of Python code
[18:51] that you tend to use do that, but I've seen that in like some Python code bases, not many.
[18:57] But in code bases in languages like Java that explicitly say like this is a string,
[19:02] that's annoying because if you know it's only ever going to be a string and not null,
[19:05] why do you have to check for it? And that's why union types are valuable.
[19:09] Because we now can explicitly say this is not string or undefined or null.
[19:14] This is only ever string. And those variables over there,
[19:16] those can be string or undefined. So you can explicitly say whether you have to check
[19:21] for something being undefined. And I see that doesn't click.
[19:27] Maybe this one extra cherry on top will click. If you take something that's allowed to be undefined
[19:32] and try to shove it in a place that's not allowed to be undefined,
[19:35] TypeScript will yell at you because it knows the thing that can be undefined might be undefined.
[19:41] So it won't work if you try to do things on it that only work on strings, like calling dot to uppercase.
[19:47] - Yeah, I'm just also trying to think of like my own work that I've been doing,
[19:56] especially the first site that I built for Teach Gen Tech was included TypeScript.
[20:03] And all of the types that they were assigning were strings. So that's where I'm also like struggling
[20:10] 'cause I'm like, but none of them said like something specific like this.
[20:15] And trying to put it into a practical manner, which we will do if we have time going into the exercises.
[20:22] So that part, I am looking forward to. Now, and I'm gonna skip along over here
[20:31] because we're not gonna go step-by-step on every one of these, but if, curiosity, it wasn't,
[20:39] do you think it makes more sense putting like the union and then defining the properties?
[20:45] Because I think declaring union types and union properties also got mixed up for me.
[20:52] - What do you mean? Sorry, by union properties?
[20:56] - These ones of declaring union types and then like the properties of it.
[21:00] And I was like, wait, is that just because of saying that it was the down here with the numbers in the strings?
[21:11] I think I was getting kind of confused there. - I think, this is good learner feedback.
[21:18] Thank you. Good reader feedback.
[21:20] In retrospect, I think a better name for that chapter might be properties of unions.
[21:25] 'Cause it's talking about the properties you're allowed to access on things that are type union.
[21:31] - Okay, okay. That's, it's weird, but that totally is clicking more
[21:39] on which I think is part of the narrowing and the, where'd it go, where'd it go?
[21:48] I have to think of it, where it went. Would it be kind of like putting through
[21:54] with type aliases then? I know I'm totally skipping like four pages,
[21:59] but like it makes more sense if you're putting properties and you know the properties, the aliases, I don't know,
[22:07] just maybe it's the way it's structured, which let me show everybody, which this is something
[22:12] that for those who watch, please ask the questions you have because not everybody is going to bounce around
[22:20] like my head does. And luckily Josh answers questions,
[22:24] even though I bounce around a lot. Because with the type aliases, this made a lot of sense
[22:30] on like raw data could be any number of these things. And so if we do let raw data be raw data, okay, cool.
[22:40] Raw data equals all of these, done. And for some reason, the way I'm visualizing it
[22:46] is for union type or union properties is kind of like showing here like,
[22:54] hey, these things could be properties and like a visual of it, I guess you could say.
[22:59] - I would encourage you to visualize type aliases, like type raw data as like a copy and paste
[23:06] or cut and paste operation, where whenever the code says one thing, raw data,
[23:11] it actually means whatever's aliased by that, like Boolean or number or string.
[23:15] Like literally if you copy and pasted the Boolean or number or string and so on
[23:19] into wherever the code referenced raw data as a type, it would behave the exact same.
[23:24] Like you might have slightly worse error messages, but that's literally what happens,
[23:28] give or take on the inside in TypeScript. Does that make sense?
[23:33] - What's the difference between type aliases and any? - And a type alias is a way to like copy
[23:43] and paste a description, like a cookie cutter template. And any is like a very foul smelling piece of matter
[23:50] in your cookie batter. You can copy and paste any if you want,
[23:54] but it's not normally something you want in your code. It's like a different way of doing things.
[24:00] It's like a different type that can be used. Whereas an alias is like how you describe types.
[24:04] I don't like what I just said. I don't think it's a very good explanation.
[24:11] - Well, let me bring this one up and then we can go back to it.
[24:14] So Papa Smurf asked or said, so if you have a string,
[24:19] you can call those string properties, but if it's undefined, it won't have those properties.
[24:25] - I'm gonna answer in the affirmative to what I'm interpreting that.
[24:31] And please let me know if I'm misinterpreting. If you have a variable that's a type string,
[24:36] say type string, then yeah, you can call any property on that variable
[24:39] that TypeScript knows exists on strings. Like two uppercase, two string, or two lowercase.
[24:43] If the string is known to be type undefined or is a type union that includes undefined,
[24:49] then you're not gonna be able to call those things because TypeScript knows it might not be a string.
[24:56] It might be undefined, which doesn't have any of those properties on it.
[24:59] So this is, in the case of undefined in your type union, this is TypeScript's way of making sure
[25:04] you're not gonna get a runtime exception, error cannot read blah of undefined
[25:08] because your variable value is actually undefined. Instead of some string.
[25:11] Is that what you meant? By the way, I'll also note that this is like relatively new
[25:17] as a concept in mainstream programming. Like most mainstream programming languages don't do this.
[25:21] So as an industry, we're still kind of learning how to explain and phrase the stuff
[25:25] around unions and narrowing. It's not just you folks who are going like WTF is all this.
[25:30] - I've been going WTF to like programming in general. And then it's been, gosh,
[25:38] eight months ago, Mishko, who created Angular was on Teach Gen Tech,
[25:45] talking about his newer language, Quick. And he was on Anthony Campolo's stream for JavaScript Jam
[25:53] or Java Jam? Damn, I don't know.
[26:00] JavaScript Jam, yeah. And I was like, I actually understand what they're saying.
[26:05] A lot has changed in eight months. - All your information is worthless.
[26:11] No, no, that's good stuff to know. - What will happen when I call it and it's undefined?
[26:18] - Great question. TypeScript is just a development time tool.
[26:22] So it can yell at you and say, hey, this is gonna be undefined
[26:25] and you're trying to call that two uppercase. This will crash,
[26:27] but it'll still compile the code to JavaScript and let you run it and let you see the crash,
[26:31] the maybe see a crash in real time if you want to. But all we're talking about is just theoretical,
[26:36] like little annotations in the code and then a language TypeScript,
[26:39] like it's corresponding program, the type checker looking at your code and saying,
[26:43] hey, I think this is wrong. But again, this is all development time.
[26:47] Your code will still run even if TypeScript is yelling at you about errors.
[26:50] - I think that's a hard thing to realize that even if TypeScript is going WTF,
[26:58] you can still run it. - Is it feasible for me to present using the Playground
[27:05] for like a quick two minutes? - Yeah, do it. - I found that
[27:07] to be a good, awesome thing. - Do it. - So the TypeScript Playground,
[27:13] I'll post it in the Twitch chat. - Thank you.
[27:16] - One of my few not cat related messages. TypeScriptlang.org/play, that's where I'm going.
[27:21] I'm gonna present, show screen, TypeScript Playground, boop. Ignore that horrible code I just showed.
[27:30] - Well, good news, I didn't show it to everybody yet. So there you go.
[27:33] - Nice. All right, you can ignore the use strict on the side.
[27:36] That's just some JavaScript crump that gets made for compatibility reasons.
[27:40] Anyway, so let's say you have a variable, like let name maybe,
[27:44] and you say that it can be string or undefined. Your type alias here,
[27:50] this is on the left TypeScript code and on the right JavaScript.
[27:53] That type alias is just a development time thing. The stuff that actually gets run is on the right.
[27:58] Just let name maybe. So I get this now when you and I first started
[28:05] and I think it was the first stream you showed me something like this.
[28:08] And I was like, what, what? It took me a long time to understand this.
[28:15] And I think one of the easiest ways that if I could go back and tell myself now is it's like,
[28:23] it's a good way of saying it. When you go to a coffee shop and you get a mocha,
[28:35] all you get is a mocha. You just, that's what they hand you is a mocha,
[28:38] but you don't only see the ingredients that go into it, which is, you know, the espresso, hot water
[28:46] and chocolate sauce and milk. And when, but you can see the mocha is done.
[28:53] And I think that's been a really hard way for me to comprehend what TypeScript does
[28:58] because it's still Java. Like it doesn't most of,
[29:05] at least that I've seen most languages, whatever you put in your, to type out will run.
[29:12] You know, like it's always same, same where TypeScript is more like
[29:17] you're making coffee behind the scenes. - Yeah.
[29:20] You're stepping behind that barista counter and learning latte art,
[29:23] which I actually am doing now, fun fact. - Oh, yay.
[29:26] - Send pictures, post pictures. - As soon as I can actually do it, I will.
[29:30] - Have you done the heart or a leaf? Those ones aren't too hard.
[29:36] - I've managed to do some rather inappropriate symbols, which will not be shared on the stream by me voluntarily,
[29:41] but eventually I'll do the leaf, yeah. - What milk are you using?
[29:49] - So far, I just use like 2%. - Okay.
[29:52] Because for those who want to know, because I did barista for a hot minute,
[29:57] that non-dairy milks are actually harder to be able to do latte art than regular milk,
[30:07] such as even skim milk is easier than non-dairy milks to do latte art.
[30:12] There you go. Okay.
[30:16] Please explain what we have on the screen. - Sure.
[30:19] I quickly typed it up in VS Code. So let's say we have previously declared
[30:22] that name maybe is allowed to be anything that's either string or undefined,
[30:26] which means we still can't put anything that's not one of those.
[30:28] We can't do like name maybe equals on three, three, seven. That's not allowed because that's a number.
[30:33] If you look at the TypeScript complaints. But the key thing with the union type
[30:36] is that it can be either of these two types, either or. So if we just do like a 50% chance,
[30:42] it's either gen or undefined, that's allowed because it can be either a string or undefined.
[30:50] But the really key useful thing in TypeScript land is that it will yell at us if we try to access something
[30:55] that only exists on some of the union types, not all, because name maybe is possibly undefined,
[31:02] which means this code has a 50% chance of failing. In fact, if I run the code, half the time it yells
[31:11] and half the, oh yeah, look at this, alternating. Okay, 50% chance it'll throw an error.
[31:17] So this is TypeScript telling us, hey, you might break. So really quick, can you comment out name maybe math down
[31:25] and then, yeah, line five, that would make more sense. Could you comment line five down
[31:34] and uncomment line three and run it? Because you said like, just so we can get a visual of it,
[31:41] of like, hey, what happens when you run something and it says.
[31:49] Sure, I'm trying to figure out how to clear, doesn't seem well, this window.
[31:52] So maybe I should like at the end, just like log name maybe. - Oh yeah, thank you.
[31:57] - Maybe is name maybe. Oh, TypeScript yelling,
[32:02] but it still runs and creates JavaScript code. - I think that is such a huge key to see and how,
[32:10] that is so important. This is a great example, thank you.
[32:17] I appreciate you showing us. And Papa Smurf, you were asking some of these questions.
[32:22] So if you're still here, is this starting to make a bit more sense?
[32:27] 'Cause I am curious. Now.
[32:31] - There we go. We got the TypeScript complaints.
[32:37] Oh my God, what is that? Jeez.
[32:40] We got the TypeScript complaints in the middle. The actual JavaScript output on the right.
[32:46] And. - I can't, we can't see the actual JavaScript.
[32:50] - Oh, you can't? Oh no, I was looking at the DevTools, oh well.
[32:53] I guess we can only see one of these at a time. You get the logs.
[32:56] - But Papa Smurf said PHP unions are similar and throw exceptions at runtime by the sounds of it,
[33:07] but are relatively new. Only difference is JavaScript will still try to run.
[33:13] - That's awesome. I did not know PHP had union types.
[33:17] Those people over there, the language folks for PHP, they're doing a good job.
[33:21] They've had a lot of good stuff. Because yeah, PHP is like a more traditional type system
[33:25] that is a runtime type system. You can reference and refer to the runtime types at runtime.
[33:31] Like in your code, you can say like, if the type this is being called with is something,
[33:35] then do some other thing. Whereas in TypeScript, vanishes after development time.
[33:41] It's just JavaScript output. - I have like a half thought question, give me a second.
[33:47] Something that I struggled with when first trying to comprehend TypeScript would be,
[34:02] so would someone use TypeScript to create something, but use the JavaScript it created
[34:10] to actually put it into a program? - Yeah, TypeScript is a tool
[34:15] for creating good JavaScript programs. It coincidentally lets you write something
[34:19] that looks a lot like JavaScript, but is actually a little different.
[34:22] Like it's got this new type syntax. But you can think of TypeScript as like the ingredients
[34:27] that go into the Mocha. And the ingredients may or may not look like actual Mocha.
[34:32] They might look like weird chocolate syrup powder and hopefully coffee beans,
[34:36] but maybe some sort of like weird pod thing. - Okay, okay.
[34:40] Yeah, because I guess I'm curious, like if somebody built a program with using,
[34:47] we'll say Astro using Tailwind CSS and TypeScript. If I deleted my TypeScript file, would it still run then?
[34:58] After everything is built, will it still run if I don't have my TypeScript file?
[35:04] - It should, if there's an output JavaScript file, some .js or .cjs or .mjs or whatever extension
[35:10] created somewhere. Yeah, you don't need a .ts file.
[35:14] It's like the Photoshop or Figma files after you've exported it to like an SVG or PNG or JPEG.
[35:20] - That's a great way of saying it. - Yay. - Oh, yay.
[35:24] Yay, okay. We're moving right along.
[35:28] Yay, okay. Now, I have to like rethink where I was at.
[35:36] For the rest of this, so I will- - Do you want me to stop sharing or?
[35:43] - I was just about to ask you the same thing. I'm like, was there anything else you'd want to show us
[35:47] on this to kind of like get to know the unions and literals? - Yeah, a couple more things.
[35:56] One is you can see that TypeScript gives a complaint here. If you try to call it to uppercase
[36:02] in something that might be undefined because it might throw an error.
[36:06] It might not. But narrowing is when inside a statement,
[36:10] TypeScript can deduce. It can narrow the type of something to be more specific.
[36:14] It can deduce that inside this if statement, if name baby is truthy, it can't be undefined
[36:19] 'cause then the body of the statement, line 12, would never be run.
[36:23] So inside this if statement, name baby is type string, which is why this code is not given
[36:29] any TypeScript red squigglies. Line 12 is fine.
[36:32] And we can see that it never throws an error when it's run, if I can get that to show.
[36:38] There we go. Does that make sense?
[36:43] - Let me read out Papa Smurf's and then I will reanalyze. And Papa Smurf, please do not apologize on this.
[36:58] I'm an absolute noob. So at least when other people ask questions,
[37:02] I can learn along with everyone. So say you have a DTO with like four types,
[37:09] how would you narrow that? - So correct me if I'm wrong,
[37:14] I'm gonna assume DTO is data transfer objects in this context, which is a fancy term
[37:19] for any object that's used to carry data like between two things,
[37:24] oftentimes like two programs or processes. It's like a standard term and yeah, like backend stuff.
[37:31] So you have a DTO with four types. We haven't seen how to rep, oh, awesome.
[37:37] Yay, I got it right. We haven't seen how to represent object shapes
[37:41] like JavaScript objects in the type system. But once we do, you will be able to mix those with unions.
[37:46] So you can have a union that's like apple shape or banana shape or cherry shape or dragon fruit shape,
[37:53] or maybe like fruit shape or vegetable shape or carb shape or something.
[37:57] And then your DTO can be represented as a union of it. Like, okay, it's one of these possible shapes.
[38:01] And each of those shapes can be like an object shape or string or undefined or something.
[38:05] - And guess what next chapter is? Object.
[38:12] - I wasn't gonna guess, I wasn't sure if you were asking me. - I didn't read ahead though, just so everybody knows.
[38:18] I did not read ahead, we're not gonna go there yet. I am like a, I will get it done just in time
[38:25] to learn things. I will say teach Gen Tech and we're University of Gen.
[38:30] I actually have learned more in the eight months of doing this than I did the multiple years
[38:37] I tried to go to school. So, but okay, cool.
[38:45] And I liked how you gave the example of narrowing as well. And this is all making a lot more sense now.
[38:54] - If you were a compiler, you'd be a just-in-time compiler. - This is true.
[39:02] Okay, just because I liked this part of the chapter and I feel like it'd be fun to have you go over it,
[39:13] whether you share your screen or you want me to share the chapter.
[39:18] The billion dollar mistake. Which is on page 36, let's get there so I can actually see it
[39:27] and I will share my screen so people can at least see what we're talking about.
[39:31] Entire screen, this one. Okay, so, Tilda, Tilda over here, get over, wait.
[39:41] Oh, there we go, we got the billion dollar mistake. Right, okay, is it fitting, maybe.
[39:49] It's kind of weird, it doesn't want to fit both. It doesn't want to fit both, oh, well.
[39:54] So, it was the invention of the null reference in 1965. This has led to innumerable errors, vulnerabilities,
[40:07] and system crashes, which have probably caused a billion dollars of pain and damage in the last 40 years.
[40:16] - Damn. - And given that that was just doing the math
[40:20] spoken in roughly 2005, imagine how much worse the damage cost has been given the exponential growth
[40:28] of the software industry now in like almost 20 years later. - Oh, thank you, oh, thank you.
[40:33] So, how does TypeScript, this one we got to share.
[40:43] - Papa Smurf said, "I make the billion dollar mistake "every time I write JavaScript."
[40:48] - Ba-dum-boom. - Well, hey, you're learning.
[40:55] How would you explain what the billion dollar mistake is as it relates to TypeScript
[41:03] and how it helps conceptualize it more? - Sure, first of all, thanks, Ryan, for the question.
[41:10] First of all, thanks, Ryan, for the link share. Second, I find that I like sharing these
[41:16] or explaining these with a playground, so if you don't mind, I'll just hop right back in.
[41:19] - Yes, yes, I am loving this, thank you. - Cool, so this code is always gonna crash.
[41:25] Function greets, we haven't gone over functions, but it's the same concepts as before.
[41:29] You can annotate that a parameter is a particular type, let's say string, and this one, oh, right,
[41:34] and let's say like your name dot to uppercase. So here we say that we're gonna greet somebody by saying,
[41:41] "Hi," and then your name in uppercase. And then we pass in null to greet.
[41:46] Do you think this code will crash, yes or no? - No, because isn't null like nothing?
[41:54] - Null is nothing, which means it will crash because you're not allowed to read properties off of it.
[42:00] Unlike in other languages, like Ruby, which allows you to do like fun shenanigans sometimes.
[42:05] Yeah, so this is always gonna run. And yet, there is no red squiggly here,
[42:12] which is weird because we have already been trained that if TypeScript thinks something is gonna crash,
[42:16] it should give us a red squiggly. And this is like five lines of code,
[42:19] so it should know that this is gonna crash. And the reason why- - I've had this happen.
[42:24] - You've had this happen? - I've had this happen.
[42:27] - Which this? - Just something didn't squiggle and it crashed it.
[42:32] And I think it was because of the TypeScript with a, but again, I say that because it was my first time
[42:40] learning TypeScript and I didn't put things in proper. Yeah, anyway, please continue, yeah.
[42:44] - Who knows then? So yeah, who knows?
[42:48] But in this specific case, this is the billion dollar mistake.
[42:52] The idea that you can provide something like null or undefined, in JavaScript they're like almost the same,
[42:57] which has annoyed me and everyone for years, to a place that does not expect it,
[43:02] that does not explicitly say this can be string or undefined, or it doesn't explicitly say string or null.
[43:08] And a lot of programming languages, that's just how things are.
[43:13] Like in C# prior to a few years ago and in Java, I think still now, like that's just how it is,
[43:18] which is why in a lot of code, you see like, if your name equals null,
[43:24] throw new error, your name is null. That's really common.
[43:31] And that's because a lot of old language didn't have the concept of union types,
[43:34] saying that something could be either, let's say string or null.
[43:38] They just were like, it's one type and then it could also be null.
[43:41] So the billion dollar mistake is corrected by a particular compiler option
[43:46] that TypeScript has, is it strict null checks, which says no, null and undefined are no longer assignable
[43:54] to all the things. This is no longer a null.
[43:57] You're not allowed to provide null or undefined to something that doesn't explicitly say
[44:01] it can be null or undefined. (mouse clicks)
[44:06] I'm gonna pause on that and read everybody else's stuff of, oh, we read that one.
[44:16] There we go. Fukai says, "Cannot read properties of undefined
[44:21] "is probably the most common error in all of JavaScript "if they had to take a guess."
[44:28] Papa Smurfs said, "They were going to mention "duck typing in Ruby, but it can be mind blowing."
[44:35] - Yeah, fun fact, TypeScript is like a halfway or like a intermediary step
[44:40] between duck typing and strict typing. Duck typing is do whatever you want at runtime.
[44:44] If it works, it works. If it quacks like a duck, it's a duck.
[44:47] Strict typing is no, we're gonna exhaustively check it before you run it.
[44:50] And then it has to be explicitly the thing you said it's gonna be.
[44:53] TypeScript is structural where you can say what stuff is supposed to be.
[44:56] And as long as we think it matches up, that's fine. So it's like duck typing in the development side of things.
[45:02] - What's an example? Like, so Ruby is duck typing.
[45:08] Are there any other languages that are duck typing? I don't know if I've actually ever heard of that term.
[45:16] - It's a fun term. If it looks like a duck and quacks like a duck,
[45:20] it's probably a duck. JavaScript is duck type, Python, Ruby,
[45:23] except for the fact that Python and Ruby are adding in type annotations in some native-ish form
[45:27] and we have TypeScript for JavaScript. So fun facts about duck typing.
[45:31] Everyone ends up just going to structural typing eventually or something better than duck typing
[45:36] because it's for all the reasons why TypeScript are good. - Sometimes I just gotta let this sink in for a minute.
[45:48] But this is making sense. Like what you just said about like being able to...
[45:53] Can you show us what it was called again? Where I should just like look in here
[45:58] for the null to be turned? Because you had to turn that on, right?
[46:04] For null not to work. - Strict null checks is a compiler option.
[46:08] By default, if you run TypeScript with no settings, it's not on for compatibility reasons.
[46:14] They didn't have it originally. But if you do the like friendly,
[46:17] create a TypeScript project for me in like any framework or TypeScript itself,
[46:22] like tsc --init, which creates a new TypeScript configuration,
[46:25] they'll turn it on for you. So the vast majority of projects,
[46:29] at least the vast majority of new TypeScript projects use strict null checks and other strict flags.
[46:33] - I'm adding this. - The way that I phrase this in the book
[46:38] is if you've never worked in a more traditional language like C++,
[46:41] this is probably weird and confusing to you. Like why wouldn't this null not allowed thing be the case?
[46:47] Like a billion dollar mistake seems weird. But if you've worked in those languages,
[46:51] it may seem weird to you that that's even a mistake in the first place,
[46:54] that we have another way. Like people get very entrenched in the mindsets.
[46:57] And I've seen both cases where like, why would it,
[47:01] like null is just another type in TypeScript and undefined,
[47:04] like why would it be that it's like some weird special case is how people think.
[47:08] So if you're looking at this going like, why was it not like that all along?
[47:12] Why is null somehow special case? You're right, it shouldn't be.
[47:23] - I am actually going into VS code and checking if mine is on.
[47:28] 'Cause I'm curious, but okay. This is totally making sense.
[47:32] And we talked about type aliases. And I liked how earlier you were talking about how,
[47:42] and I almost wonder if this is making more sense about the ducks.
[47:46] Because type aliases are not JavaScript. Almost made me think that it's not duck typing.
[47:54] Yeah, okay. Oh, I skipped, I skipped.
[48:02] Papa Smurf said you answered the questions they asked. Yay.
[48:10] And Sakai says duck typing is like, if an object has a duck quack method,
[48:19] then it is a duck. In a non-duck typing languages,
[48:23] you would have to say beforehand that the object is a duck. It's not defined enough.
[48:30] It's not enough to just be defined a duck quack method on something for it to be a duck.
[48:36] Or that's how I think about it at least. I'm actually really excited for objects
[48:41] because I feel really embarrassed saying this, but I'm like, when you start to learn,
[48:49] you're like, I know too much. I shouldn't not know this.
[48:52] Yet that's learning. Like you, it's gonna get more confusing
[48:57] probably before it gets better. And in Python last week, we were talking about functions.
[49:04] And for some reason it couldn't click what functions were. And I'm like, what are, no, what?
[49:09] Yeah, you literally use functions as part of everything. And yeah, that was,
[49:17] I feel like objects are probably the same thing, but at the moment they don't fully click.
[49:21] So I'm excited to be getting into objects in one of these streams,
[49:25] because it's gonna click like functions did and me not realizing how often I use functions.
[49:32] Cool, yeah. - It's awesome to see the learning process
[49:36] like live in real time over the months. - Oh my gosh, it's so frustrating though.
[49:41] I'm just like, I'm slowly going through my old streams to be able to create chapters.
[49:46] And I'm just like, oh God, Jen, young Jen, what are you asking?
[49:53] And I'm like, thank you for asking that, but geez, okay. - You have emotionally resonant,
[49:58] empathetic conversations with yourself. - That's why I'm just like, okay,
[50:03] if I could like help myself back then, this is what I would say.
[50:10] - And then your combining type aliases, that one seemed pretty standard to me.
[50:18] It didn't seem too confusing to me at least. Is there anything, I know we skipped around,
[50:23] so I do wanna ask, is there anything in this chapter that you're like,
[50:26] dude, we didn't cover and we need to cover? - I think so,
[50:30] but I might be wrong about the need to cover part. We didn't cover the difference.
[50:34] - I was just gonna say your opinion on it, it means we need to cover it.
[50:40] - Maybe, we'll see. The great problem of teaching
[50:45] is that as soon as you know enough to teach, you're no longer in that beginner mindset.
[50:49] There's this very difficult challenge. We didn't cover the difference
[50:53] between primitives and literals. A primitive type we've already covered in the book,
[50:58] string, number, actually number undefines, big ints that no one ever uses except for like special cases.
[51:05] So like string and number or boolean are really common primitives.
[51:10] But then you can have specific instances of those primitives like Hypatia is a string.
[51:17] But that philosopher variable, it's not gonna be just any old string in the universe.
[51:22] We know it's specific. Yeah, symbol, another great commonly used.
[51:26] Yeah, yeah. Yeah, well, what are they?
[51:30] See if I, I wrote in the book, we'll see if I know this off the top of my head.
[51:33] All the primitives in JavaScript are string, boolean, number, null undefined, big int, symbol, is it seven?
[51:42] - One, two, three, four, five, six. Yeah, I can go there really quick
[51:50] because I feel like I'm getting smart about using this on here because I'm like,
[51:56] oh, I can know the page number. Yay, that will help.
[52:00] All right, here are the, oh, oh, look, the seven. And we had to do special things
[52:08] to get that list all in one page. It would have folded by default,
[52:11] which would have been confusing. Yeah, so those are primitives,
[52:15] but each of those can have specific instances. Like if you say const philosopher equals Hypatia,
[52:21] that variable Hypatia is not just any old string. We know it's more specifically the literal Hypatia,
[52:27] which means you can do some clever, fancy things. Like VS Code, because of TypeScript telling it,
[52:35] if you hover over a variable that's declared as const, we'll give you the literal type,
[52:39] like Mark Goldberg, instead of string, if you hover over it. - Oh.
[52:43] Okay. I think, I want to look at both of these.
[52:52] No, no, oh, oh, I think we got it. - You got one figure caption.
[52:59] - Yeah, we'll just turn it off for now. So.
[53:05] - So this doesn't seem very useful yet, but it will probably be more useful later on.
[53:17] One example of where it's useful is you could have union types
[53:20] where some of the things are primitives and some of the things are literals.
[53:23] Like you could say that something is either a string or the number negative one to indicate failure.
[53:31] Some programs do this. So if you check whether the result of something
[53:35] is the number negative one, then you know it's like number negative one.
[53:38] And in the else case, you know, it's going to be a string. - Okay, so, and this is for everyone watching this.
[53:48] These are some of the really fun questions that I get to ask Josh,
[53:52] because I did not learn JavaScript first. Like I can make things happen.
[53:57] If I Google enough, I can make it work. Do I know what things actually mean?
[54:04] No, like what is the difference between const and let? - Great question.
[54:10] A const variable may not be reassigned to a different value. If you say const first name equals high,
[54:16] you're never going to have a different first name. - Okay.
[54:20] - A let variable can be reassigned to a different value. That's the only difference.
[54:25] - And is that TypeScript only or JavaScript in general? - JavaScript in general, yeah.
[54:30] - Okay, okay. - I thought so, but I'm like, hmm, hmm.
[54:33] Okay. So if it's const mathematician equals Mark Goldberg,
[54:43] then Mark Goldberg will always, like, if you want to look it up,
[54:48] it's going to show up as the mathematician equals Mark Goldberg.
[54:54] I'm trying to think of a way to say it back to you. That's not working very well.
[55:00] (laughing) When would you go back and look at this?
[55:13] Like, I guess, hmm. If I go search for Mark Goldberg,
[55:18] I'm going to find a string where, if I say let mathematician,
[55:24] where if I put const mathematician, I guess I don't really understand a way of saying this,
[55:30] even though I feel like I get it. - It'll be a lot more useful
[55:35] in the objects chapter, I feel like. When you have a property
[55:38] that can be one of specific set literals and which literal it is changes what, like, the type is.
[55:44] Which is actually tying back to the DTO, data transfer object suggestion earlier,
[55:48] where, like, sometimes people have an object where, like, the type property on that object,
[55:51] or, like, variant or something, if it's this one string, if it's root,
[55:55] then it has these properties. If it's this other string, like vegetable,
[55:58] it has these properties. That's where it comes in handy, oftentimes.
[56:01] And we'll actually see that in the next chapter, how to do that.
[56:08] Did that just click? - Well, I think I did that
[56:12] with my first Astro project for the website, is I think, because I was trying to ask you
[56:20] to compare them with modules, and they weren't quite modules.
[56:24] I think they were objects. - Okay. - I don't remember.
[56:29] But I will go follow up about that. - Hmm. - Hmm.
[56:34] And that is, like, one of the hardest things that I could say to anyone is,
[56:39] even if it doesn't make sense, keep going. It will click, probably, eventually.
[56:45] And then Ryan said, "And let is kept within a scope unlike var."
[56:55] What does that mean? Oh, yeah.
[56:58] So this is some dumb stuff. Dumb is the wrong word.
[57:01] Some silly stuff. There are three ways to declare a variable in JavaScript.
[57:05] Var, let, const. Let and const are the good ways.
[57:08] Var is the weird way. Var is how the language originally did it,
[57:12] and let and const are added later. But var had these weird rules where...
[57:17] Oh, I don't even know how to explain it anymore. It's been so long.
[57:22] Don't worry about var. The fact that I can't instantly remember how to explain it
[57:25] means it's, like, weird and convoluted. But the TL;DR is,
[57:28] it's an old way of declaring variables that has, like, weird shared rules
[57:32] where you can have, like, multiple declarations all over the place and declare things out of order.
[57:36] And it's confusing, and everyone hates it, and you should avoid it if possible.
[57:40] - So would be... Okay.
[57:43] And would it be, like, var became before let, and let, like, replaced var
[57:49] because you can reassign something with let? - Let replaced var, yeah, because...
[57:57] Well, there are some specific cases where var actually still is useful, unfortunately.
[58:03] Don't think we should go into them now. But yeah, the...
[58:07] Generally speaking, let has, like, become what people do instead of var.
[58:12] - Okay, so... - Satisfy you?
[58:23] - Mm, yeah, yeah. Uh, cannot reassign.
[58:30] So a const can reassign a... It cannot be reassigned.
[58:36] A let can be reassigned, and they're reassigning what's ever being declared,
[58:43] which is not necessarily a type. - Sorry, you lost me on that one.
[58:50] - Okay, so, like, what is this?
[58:54] I get that it's a string, but, like, it's... - When you say this.
[59:00] - Oh, yeah, you can't... I don't like when this doesn't highlight
[59:06] the way I want it to, so I could show you. - I know, it's so confusing.
[59:10] It's, like, the instincts there, right? - Okay, so Mark Goldberg.
[59:15] - Sure. - What is Mark Goldberg called?
[59:18] Would it just be a string? So if you const, like, const Mathematician Mark Goldberg,
[59:24] you would just say Mark Goldberg cannot be reassigned, or Mathematician cannot be reassigned.
[59:34] Mathematician is what? - I was just at a conference where there was a running gag
[59:40] that the theme of the conference was either pandas, 'cause someone referenced it in an early talk,
[59:44] or the phrase, "It depends." And in this context, another key thing from the phrase,
[59:51] was the context here is that it is either a string or the literal Mark Goldberg,
[59:58] depending on, like, what you wanna be more precise about, or, like, how precise you wanna be.
[60:03] So both are valid and correct answers. In these variables, Mark Goldberg is a string.
[60:08] More specifically, it is the literal string Mark Goldberg. - But Mathematician would be the variable?
[60:18] - Yes. - Or, like, the word Mathematician is a variable.
[60:22] So a const declares the variable, and a const makes the variable
[60:29] not being able to be reassigned. A let makes the variable be able to be reassigned,
[60:34] and bar does something to the variable we're not gonna talk about.
[60:38] - That's an excellent description, yes. - Yes, that is, yay.
[60:43] And this is one of the hardest things with, like, learning by your, like, doing your own stuff,
[60:48] is, see, like, it took me forever to figure out how to ask you what a variable was,
[60:53] because I didn't know the word. - What?
[60:57] - Okay, I have things from Papa Smith on here that I have missed, so let's go back.
[61:02] Thank you for your patience. Does anyone remember use strict in JavaScript with vars?
[61:09] Probably showing their age. - I remember.
[61:14] - So you would have a var and tell it to use strict, so it'd be kind of more like a const?
[61:20] - Now, newer developers these days don't know how weird JavaScript was,
[61:26] like an old Seattleite, a Brooklyner. JavaScript is so weird that they added the word use strict.
[61:34] Like, you could say at the beginning of a file, use strict, and that would make JavaScript slightly less weird.
[61:39] There are proposals to add even more, like use stricter, or like use strict to,
[61:44] or something to make it more and more strict, but they never went anywhere.
[61:47] So there's some, like, really wacky things in JavaScript that you could do that get disabled
[61:50] if you just put the string use strict at the top of your file, or in, like, a function or block.
[61:56] - And that was, like, ES6. Oh, this is, funny enough, Papa Smith,
[62:06] during, I think our first chapter, is when I got to learn about the versioning of these
[62:12] that I didn't know existed. That was a fun project. - Do you remember
[62:17] what ES stands for? Trivia question.
[62:19] - Ah, shit. I don't know.
[62:25] Let me see if I wrote it down. I honestly don't know if I wrote it down.
[62:30] I do know it's versioning, which I didn't know beforehand,
[62:41] but I don't know if I wrote down. No, I don't think I wrote down.
[62:45] Wait. No, I just wrote down ES length,
[62:50] compared to prettier when we were talking about it during types at the beginning of the last stream.
[62:57] But no, I don't remember what ES means. - ECMA script.
[63:04] Do you remember what ECMA stands for? - No, I don't know how we went through this.
[63:11] - I don't remember what ECMA stands for. I'm looking it up now.
[63:13] It's like the standards organization that runs, like, oh my God,
[63:18] European Computer Manufacturers Association. Okay.
[63:24] It's the standards body that runs a lot of things, including the JavaScript standard.
[63:29] But because Oracle, like a jerk, owns the JavaScript trademark and won't give it up,
[63:33] we have to technically call the language something else, hence ECMA script.
[63:37] There is shade, intentionally there. - By the way, they were hiring a developer advocate
[63:45] for those who are applying for jobs. They hit me up.
[63:48] I found a job. You can go apply there.
[63:51] I like my job. I don't know why people do this.
[63:53] When you get a job, they finally like reach out to you.
[63:55] And it's like, bro. - Always.
[63:59] - No, I like my job. Please go away.
[64:01] Okay. So it's called ECMA script.
[64:03] I will look more into that. And then, like I said,
[64:09] what they do is always use const. And then if I find out later that I need to mutate it,
[64:16] I change it to a let. That is good to know
[64:20] because I am rebuilding my site with, it is still with Astro,
[64:25] but it's with like, the theme isn't as defined, I guess is a good way of saying it.
[64:32] Like it's not as structured. So I can customize it a lot more.
[64:35] So I'm finding myself doing a lot more fresh coding instead of mutating their code.
[64:41] So it's good to know these. I'm going to go share what Helper Smith sent.
[64:49] And I just have to click it into a different tab. ♪ Do, do, do ♪
[64:54] ♪ Because StreamYard doesn't do that right ♪ Aha.
[64:57] Oh, this is good. Thank you.
[65:00] ♪ Do, do, do, do, do, do, do, do, do, do, do ♪ Yay.
[65:05] Okay. ECMA International,
[65:13] formerly European Computer Manufacturers Association. That is like a lot.
[65:20] But now we know. Now we know.
[65:26] Like reading "Rainbow," the more you know. Okay.
[65:33] Okay, anything else? Really quick, let me write this down.
[65:38] So all these define a variable. This is why I really want to be able to do this on an iPad
[65:58] because people then could actually see all these random notes that I'm doing
[66:02] instead of me just like staring down at my... - I am curious what's going on over there.
[66:06] By the way, I'm told from a mutual of ours on Twitter, Elian, that I should remind you
[66:15] or ask you if you like a particular Astro theme. Do you know which one is?
[66:22] - It's the one I'm using now. - You're using Brutal, I think it is?
[66:25] - Yeah. It's the one that I'm saying,
[66:27] I don't know if more defined is the right way of saying it or I'm just better at breaking this one.
[66:34] - Either way. - There really could be a...
[66:41] I just started using it. I got the colors to work fine.
[66:46] I can show you guys. I'm very proud of it.
[66:49] It just started. But because, and yes, Ryan,
[66:54] I probably should look at "Notebooks Camp," but that's why I'm trying to think if I can get the iPad
[67:01] because I also want an iPad. So I'm trying to find a business reason to get an iPad.
[67:06] I don't know if it's gonna work. Okay, so here is the layout so far.
[67:15] And I'm so excited about it. It's called Brutal, which let me grab the information.
[67:23] The end of automation. So this is my GitHub and you can see that it came
[67:34] from Elian, which is this one. And okay, so this is something I really appreciated
[67:45] that he did with, so this is the original theme, what it originally looks like.
[67:52] It's like, dude, this is dope. I need this in my life.
[67:55] But there's more. He also put his website.
[67:59] And I was like, dude, that gives me even more ideas. And voila, this is where we're at now.
[68:08] - Very nice. - And I'm excited about it.
[68:10] I'm like, this is so cool. But here is where it's not knowing me fix how of,
[68:16] it does not scale. - No, you have your little head.
[68:24] - Yeah, yeah, and it's like, and then look at these. - Lordy.
[68:30] - I don't know how to fix it. It took me long enough to get the colors to work
[68:34] the way I wanted to. So yeah, it's on pot.
[68:39] Well, I should be working on it, but I haven't adjusted to my new sleep schedule yet.
[68:43] And, but the way, the reason I did all of this instead of my old teach you on tech site
[68:48] is because now that I have a real job, it's kind of weird just telling someone
[68:54] to go to one of these. Instead of just being like, yo, I'm Jen Janard.
[69:00] I do all of these things. You should check out one of them.
[69:05] So yeah. - I've been meaning to update my site for the longest time,
[69:09] but I can't get rid of it. It's just so darn useful.
[69:11] Just as a landing page. - Oh, that's a different one though.
[69:16] Wait. I just mean like as a list of links,
[69:20] like it's good to have. And then also, yes, like it's a demo, et cetera.
[69:23] Yeah. - There's one that I think, I think it was yours.
[69:28] That linked to something that was not your actual website. Or it was like a page within your website
[69:34] that was like a funny image. - The Rickroll?
[69:39] - Yeah. - Oh yeah.
[69:41] On all my conference slides, I'd like to hi.joshuakaygoldweg.com.
[69:46] I think it's on Twitter. Yeah.
[69:48] 'Cause people kept freaking spam recruiter yelling at me. So yeah.
[69:54] Don't go to it unless you want to Rickroll everyone. But hi.joshuakaygoldweg.com is a Rickroll.
[69:59] - I do. And oh my goodness.
[70:02] Oh my goodness. We need to pause.
[70:05] - Hi Jacob. - Jacob is here.
[70:09] Jacob's amazing. Yay, it's Jacob.
[70:13] - We were learning TypeScript. Now we're learning how to construct a Rickroll
[70:17] in the era of modern web standards where you can't auto-play a video with sound.
[70:22] So you have to put an enter button to gain user intent. - So I wanted to show that to everyone
[70:31] because when I first like, Ben Myers was like,
[70:36] "Yo, you and Josh should be friends. "And you should reach out to him."
[70:41] And I go to like look at his site to like learn more about him.
[70:45] And this happens. (laughing)
[70:50] - So good. Sorry.
[70:54] - I know, but it does make me actually remember it a lot more.
[70:56] And it goes to your humor. And yes, for those,
[71:00] so this is first time, first time chatter,
[71:06] but not first time guest. Jacob was my first time of someone
[71:12] trying to explain to me what TypeScript was. And then we got stuck on him
[71:17] trying to explain what Headless is. Which I still don't understand,
[71:22] but I haven't, I don't even remember why it came up.
[71:25] Or Workers. - Workers.
[71:28] - Not Headless. What were we talking about?
[71:34] Server. Well, is Headless part of Serverless?
[71:45] - Class of their workers. So Kai says,
[71:49] "Josh reminds me of Richard Hendricks in Silicon Valley." - I'll take it.
[71:55] It's a good show. - All right.
[71:57] - I had a previous engineering manager/director called, say that I reminded,
[72:01] but not an engineer, some head of department somewhere or something called me.
[72:05] It was, it was maybe Patrick Bateman-esque or like some, like Ryan Gosling playing the,
[72:13] like some psychopath or something who was handsome. Fine, close enough.
[72:16] This is better. - Couple of things.
[72:23] Yay, Elyon, thank you for joining. And you should just come on our stream
[72:28] and could, you know, help with my site because you created the theme and I'm working on it.
[72:35] And thank you for the follow. And Jacob, yes, I am using StreamYard.
[72:40] And hello, Laura. Yes, yes, I am.
[72:45] I am going to have my OBS set up. - Oh yeah, you were gonna do that.
[72:54] Or you were interested in it and tentatively looking at it, right?
[72:57] - Some OBS, I'm thinking. Yes, I'm gonna set it up for the new one
[73:02] for working with work to figure out what we're doing on all of that.
[73:07] Because I gotta streamline my stuff and stuff. And yay, thank you for doing all the shout outs, Ryan.
[73:16] And yes, I'm building a new Astro site. And I can show you what it's supposed to do
[73:25] and what I did before I broke it. So this is what, not that, we can minimize that.
[73:32] That is what we were learning. Elyon made and it's pretty and it does things.
[73:40] And no, it's different, it's different. I'm building a new site.
[73:46] I still have the old site there. It's just not like public.
[73:49] But like, look, it works, it functions properly. And then the cool thing is Elyon also put their site here,
[73:57] which gave me more ideas. I was very excited.
[74:02] So, and then we have my site, which is getting there. And I even have different colors.
[74:10] I'm so excited about it. And like colors match my shows and my jobs.
[74:16] And I will show you in a second, Papa Smith, thank you for the call out.
[74:22] But what I did not do, because if we go back to Elyon's site,
[74:27] look, look, it actually does the things it's supposed to do and still fits.
[74:32] Like, it looks good. Mine, on the other hand, I broke.
[74:36] I don't know how, but it does that. Or I did this, but that's why I'm like,
[74:47] I don't know what I do. Elyon and everyone, Jacob will tell you,
[74:53] I break a lot of stuff when I'm trying to figure this stuff out.
[75:00] - Because I'm like, oh, that didn't work, let me go try something else.
[75:06] - Breaking stuff is one of the best ways to learn stuff though.
[75:08] I like this. - It matters how frustrated I get.
[75:14] - The more frustrated you get, the more you've broken things,
[75:16] the more you've learned, yay. - Yeah, and then it's like,
[75:19] I go to my D&D crew and be like, someone please help me get unstuck.
[75:23] I don't know what I'm missing. But yes, I break a lot of stuff
[75:30] and I do learn a lot. And this is actually why,
[75:36] oh, you guys, I'm really excited about this one. I'll show you this one.
[75:39] I built another Astro site that did not break. I'm really proud of it.
[75:45] It's just a landing site, but I built it without asking anybody for help.
[75:52] Yay. It was very exciting.
[75:55] - That's really beautiful. - Yeah, yeah.
[75:58] I don't remember which theme, but if you look at the GitHub,
[76:02] it will show you the theme. Yeah, yeah, they have it,
[76:05] but I was so excited. This one I made without breaking in 30 minutes
[76:11] compared to the ungodly hours I put on these sites. But yes, Astro is amazing, Papa Smurf.
[76:21] I will say, oh, this is something I meant to ask. Astro build, Astro dot build, I think.
[76:31] Yeah. Could somebody, and Josh,
[76:35] I feel like you are a good candidate on possibly explaining this, please.
[76:39] How? Something like quit couldn't be used with Astro
[76:50] and Astro can't use, because Quik also wouldn't be able to set up
[76:56] because Astro does its components. - You know what?
[77:02] I actually met Gillian at a conference wherein both Astro and Quik were demonstrated on stage,
[77:08] and I learned them and they were both really cool, but I don't think I could explain
[77:12] why one can't be used with the other, other than just they're both things,
[77:16] like Quik is its own framework. It's like a way to do very small,
[77:20] like super incrementally loaded stuff, and Astro like manages other UI libraries.
[77:26] I don't, I don't think that's a good explanation and I don't feel confident giving anything more than that.
[77:31] I'm sorry. - Oh, it's good.
[77:32] I mean, this is, and Jacob just said that, yes, most things can work in Astro.
[77:40] And to Papa Smurf's point, what is the cat's name again?
[77:47] - Jerry, I'm trying to get him out. - Hey Jerry.
[77:50] Oh, okay. Gillian says they're both trying to solve the same problem,
[78:00] but take another approach. I think what I'm curious about is like,
[78:07] I like Astro because I can find themes like this and be like, cool, let me see what I can take
[78:12] that they made that's really pretty and also make my own thing,
[78:17] where like with React and that kind of stuff, I'm like, that's a lot harder to find.
[78:23] And I don't know if that's because of Astro, but I also know that we have gone on a really far tangent
[78:31] from TypeScript. I don't even know how we got here.
[78:38] - Truly, I couldn't tell you. - Gillian said, in short, I would say that Astro
[78:45] is for content-driven websites and Quick is for the more real web application side.
[78:51] That is fair. I am see VueNation and NuxNation,
[78:57] and then also like learning about Quick, and then I just really like Astro.
[79:01] I'm like, I wanna learn something that I can build with all of them to compare them all,
[79:05] but I don't know. - All right, takes time.
[79:13] Back to learning TypeScript. - Yay.
[79:17] - Is there anything else that you would suggest we go over? - From TypeScript?
[79:22] No, I think we're good. Before all these nice folks talking about Astro
[79:28] came in and Quick, we covered union types, literals versus primitives,
[79:34] the billion-dollar mistakes for null checking, and type aliases, is that all?
[79:40] - Okay, let's see. I will see if I can summarize them.
[79:44] - See if you can explain it to the people in the chat, see if any of them don't yet know it,
[79:49] and see if those explanations click at all. That would be a fun challenge.
[79:53] - Okay, I will say I am cheating and looking at the summary
[80:01] because I have to think about how I would even put it into my own terms
[80:04] to say that I understand it, so. Okay, unions are where you,
[80:13] can unions be made with a const then, to go to my other question?
[80:19] - Yeah, if you say like const something equals then some condition, question mark, colon.
[80:25] Yeah, the turnaround. - Okay, so unions are where you can put
[80:31] two different types. So you can put that it's a boolean,
[80:35] and then the dashy thing, and then the other type which could be a string.
[80:40] - And it's, I call it a pipe. - Oh, that would make more sense than a dashy thing.
[80:49] - A dashy thing. There are a lot of dashy things.
[80:51] Also a lot of pipes. - That's true, that's true.
[80:53] And then, this will be indicating union types, typing in a question.
[80:59] This is also the hard thing I have about this is I'm like, I know we went through type annotations,
[81:10] and I remember going, the words just don't make sense to me,
[81:14] but it was in chapter two. Okay, I don't know how to,
[81:26] explicitly indicating union types with type annotations. - Yeah, so let's say you have a variable,
[81:33] and you don't immediately assign something to that variable.
[81:36] - Oh, is the listing undefined? - Yeah, it starts off undefined,
[81:41] but maybe you eventually wanna add a string or a number, maybe, either, who knows.
[81:45] So you could say let variable colon string or number, or like string or number or undefined,
[81:50] or something like that, to say that eventually I might add
[81:52] one of these possible types. - Okay, that makes sense.
[81:56] How type narrowing reduces the possible types of a value. - So it's like taking away the pipe,
[82:03] and leaving it as one. Cool.
[82:08] Difference between const variables with literal types, and let variables with primitive types.
[82:15] And primitive types are the seven that are indicated in chapter two,
[82:22] and it is null, undefined, boolean, string, number, big int, and symbol.
[82:29] And literal ones are like const mathematician equals Mark Goldberg.
[82:39] And because mathematician would be literal, because we're not telling it if it's a string or anything.
[82:46] - Yeah, yeah, because it's const, it can't be reassigned. So it's not gonna be any other string in the universe.
[82:51] It's only ever gonna be that one literal exact string. - Okay, and then the billion dollar mistake.
[82:58] Turning on script null checking, because null will not come up with a red squiggly line
[83:06] telling you that it's wrong. And you could break some shit.
[83:10] So you wanna turn it on. - Wanna break that shit, yeah.
[83:13] - Using explicit undefined to represent values that might not exist.
[83:18] I don't know if we actually went through that one. - I don't think we did, forgot about that one.
[83:24] Oh yeah, that was a thing. So let's say you declare a variable, let value.
[83:29] What type is that value variable? Or like let value colon string.
[83:34] And then the next line you do console.log parentheses value. It's gonna log undefined,
[83:40] because there's no value in that value variable yet. - Oh, so because it was blank,
[83:47] where like if we use implicit undefined, we actually put undefined in the quotes,
[83:54] not quotes, brackets. - In the type annotation.
[83:58] - In the type annotation, yeah. - Could I share the playground for this actually?
[84:02] This is like one of my favorite things. - Yeah. - Cool.
[84:05] - I like that you're doing this, because it is helping click more.
[84:07] Because sometimes like trying to talk about it, and then also trying to type it,
[84:13] can be very nerve wracking to also learn. - Yeah.
[84:17] So let's say you have a variable like let sup. Good variable name.
[84:21] Yeah, and then you do like console.log sup. What's in sup?
[84:23] It's undefined. But let's say you declare
[84:27] that sup is eventually gonna be a string. And then you wanna do like sup.to uppercase.
[84:32] Well, TypeScript knows this is implicitly, meaning you haven't explicitly said this,
[84:36] but like we know it's undefined, because you haven't actually assigned a value to it.
[84:41] So in reality, sup, the variable, is kind of like the union type string or undefined.
[84:47] Until you assign something, it's either a string or undefined, really undefined.
[84:51] And TypeScript's yelling at us, because it knows we're gonna crash, or shit gonna break.
[84:56] But then if we do like sup equals, hello, yay. Now TypeScript knows after this, sup is again, string.
[85:03] It's definitely defined, and it will not complain. TypeScript knows.
[85:10] - TypeScript does know. TypeScript yells a lot.
[85:13] - Yeah. Ultimately, you could do sup is string or undefined.
[85:17] Like that's allowed. And then the TypeScript error message says,
[85:19] well, sup is possibly undefined. And then you can instead, if you want to do,
[85:24] you can do like if sup. Let's say like, if math.random is greater than 0.5,
[85:31] sup is hello, yay. Then later on, you could check, like,
[85:33] if sup is defined, then we console.log. And this is type narrowing to recap,
[85:38] because inside this if statement in the block in line eight, TypeScript knows that this stuff would only be reached
[85:45] if sup is defined, if it's actually a string and not undefined.
[85:49] So inside the sif block, sup is actually type string. No crash.
[85:55] - It makes enough sense. I don't know if I'd be able to repeat that one back as much,
[86:01] but it makes enough sense to keep moving forward. And then using type aliases
[86:08] to save typing a long unions repetitively. That one was just, instead of let something
[86:17] be fully a number string null, you would just say, let it be.
[86:25] Oh, you would just name it type. I think it makes sense.
[86:33] Oh, I didn't mean to do that. If you were still sharing, I just hit the keyboard.
[86:39] - Yeah, it's like a copy and paste or like a cookie cutter. Like when I say maybe string,
[86:46] what I actually mean is string or undefined. By the way, to answer the chat,
[86:53] like we could do like, if sup not equals undefined, like TypeScript is smart enough to know that any area
[86:58] that can only be reached if sup is actually a string inside the area sup is a string.
[87:03] Like if type of sup is string, these would all work. - Yes, yes, so what Jacob said.
[87:14] There's so many types of checks. Yes, let's not confuse me.
[87:24] We haven't even gotten to objects yet. - That case we'll just stick with it.
[87:30] - Objects is in two weeks. Join us in two weeks.
[87:35] We'll be talking about objects. Lots to learn before then.
[87:40] Next week, I'll have someone on to talk about data. I'm very excited because that's a good place to start
[87:47] instead of Kafka. But old way of doing it was type of guards in JavaScript.
[87:56] There's so much to learn. - You have architectural, archeological history
[88:06] in JavaScript that like dubious usefulness nowadays, but like cool to know once you have the time.
[88:13] - Okay, I still have to catch up and start watching season three, "Critical Mass."
[88:20] So I have a pretty long to-do list and I have to get my website done.
[88:25] The website is a little, I got to actually really work on it. It's probably gonna be my weekend project,
[88:31] but I feel like we're good. At least getting my brain a little fuzzy
[88:41] and learning enough that by the time we get to objects, I'll be like, oh yeah, I do understand that.
[88:46] So on these closing notes, we have a, what are the closing ones?
[88:54] Are there haikus too? - Oh my God, I forget.
[88:58] I want to say they're just puns, right? - I don't know.
[89:01] - I know, they're just puns. - They're puns.
[89:04] Okay, let's see if I still have it up on here. I do, I do.
[89:08] Okay. - Yeah, why are const variables so serious?
[89:13] - Anyone have a guess before I bring it up on screen? - I've been meaning to watch "Critical Role."
[89:20] - Did I say "Critical Mass?" I think I did.
[89:23] - Oh, okay. - And that's close, right?
[89:27] Except for "Critical Mass," "Critical Role." - Oh, it's because they take themselves too literally.
[89:34] - Got 'em. - It's fun, it's fun.
[89:40] Well, thank you, Josh, for joining today and for coming to hang out.
[89:46] And what? Our thing was funny, Jacob.
[89:51] Our thing was funny. And Jacob, I am going to work on getting the OBS set up
[89:56] with the chat up. - Yay.
[90:02] - And everyone, please follow so you get notifications and go follow Josh.
[90:08] See if we can do a shout out. I try to do these.
[90:11] - I'm actually doing my own Twitch stream in half an hour, just working on some TypeScript stuff.
[90:15] People want a little more in-depth stuff. Although I am getting kind of tired,
[90:19] so it might be a chill stream. We'll see.
[90:22] - I did message you. I saw that tweet and I was like,
[90:25] "Dude, you're doing two streams?" You're brain dead.
[90:28] - I'm already brain dead. It's perfect.
[90:31] I just had a conference for a day yesterday. - Oh, yeah.
[90:35] - Great conference, by the way. Staff plus New York City, really, really good stuff.
[90:38] The Lead Dev Conference line is good. - Yes, yes.
[90:44] - Also, thank you for the shout out. - Yay.
[90:47] And please, yes, go follow Josh. Follow me.
[90:51] Come join us more often. I stream, oh God.
[90:55] Starting next week, I stream five days a week. - Woo, brain dead.
[91:02] - Follow Jacob. Yeah.
[91:04] I don't know if I'm playing D&D anymore, 'cause I don't know if we're switching to another thing yet.
[91:14] We were doing something. But we do play D&Ds on Friday nights sometimes
[91:20] and on Jacob's stream. So go follow Jacob.
[91:23] I'm a giant hippo. It's phenomenal.
[91:26] Her name is Hippity. Hippity Hop.
[91:29] Or we might start streaming some other game, but I don't remember what it's called.
[91:36] Yes, go follow. Go follow Jacob.
[91:42] The Expanse, we might be doing. And I'm trying to see if they'll do it on Sunday afternoons
[91:49] when I'm awake, 'cause I wake up at 4 a.m. now and 'cause my calls are early.
[91:56] Yay, working for a fitness company. I actually like, I like it.
[92:01] Yes. Yay, thank you, Ryan.
[92:03] Thank you for shouting out, everybody. Yo, like Ryan mods quite a few channels,
[92:08] but thank you for always modding mine, 'cause I'm always like,
[92:12] I don't know how to block someone. Please ignore these.
[92:14] I'm like a horrible streamer. I'm like, ugh, I don't know.
[92:20] All right, y'all, I am not going to raid you because if Josh is gonna be streaming in like half an hour,
[92:27] you should just like come back and watch Josh's. Do you have, well, are you, do you use OBS?
[92:34] - I do, yeah. - Do you have a countdown on it?
[92:37] - No, I don't have anything. - Oh.
[92:40] - I've been meaning to set up, I actually just set up stream elements.
[92:43] I've been meaning to set up like overlays and stuff. I just haven't had the time.
[92:46] - Okay. Jacob, how did you get your countdown?
[92:49] Did you start? How did you start yours?
[92:53] I'm more wondering if I need to, like create one.
[93:02] You use overlays? Like Google Twitch overlays or OBS overlays?
[93:08] - It's not. - Overlays. Yes, there's always more to do as a streamer.
[93:15] - It's too fun. Okay.
[93:20] Well, and goodbye everyone. Thank you all.

