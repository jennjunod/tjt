---
showLink: "https://www.youtube.com/watch?v=W0fkrUicn6o"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-5-functions"
title: "Learning TypeScript Chapter 5: Functions"
publishDate: "2023-04-15"
coverImage: "https://i.ytimg.com/vi/W0fkrUicn6o/maxresdefault.jpg"
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

[00:00] Welcome to another episode of Teach Gen Tech. And we are streaming chapter five
[00:06] of learning TypeScript with Josh Goldberg. Yay!
[00:11] - Yay. Chapter five.
[00:14] - And it's crazy. That means that we've done at least five episodes,
[00:21] but they're every other week. Dude, how many have we done?
[00:26] I really should look at this. - I think we repeated one.
[00:28] So is this like episode six or something? - I feel like we might've repeated two
[00:34] because it took us like a minute to get into the flow of everything.
[00:38] - Yeah. And then did we have like a prep episode before that?
[00:41] So is this like seven or eight or something? - I think so.
[00:44] I'm actually looking because actually I think this is nine. - Jeez.
[00:50] - I'm almost tempted to like delete the old ones. - It's not me anymore.
[00:58] I'd be like, oh, we finally got into the flow. What's the ones with the flow?
[01:02] And what up, Lex? Yes, pre-rolls.
[01:06] It's yeah. - Yeah, what is going on there?
[01:09] Is that a bug? Is that intentional?
[01:12] - I have ads turned off and people still get them. And I'm like, I don't know.
[01:18] I don't know. It's frustrating.
[01:19] It's really frustrating. So Lex, I appreciate you still showing up,
[01:22] especially when, you know, Twitch doesn't want to always be our friend.
[01:28] - Well, that is weird. - I regret going to the thing that lets you get paid.
[01:32] I get paid like a dollar a stream on average. And now people have ads, even though they're subbing.
[01:37] I don't want it. I don't want ads.
[01:39] Is that why I'm here? - I don't blame you.
[01:41] - Yay, TypeScript. - Yeah, yay, TypeScript.
[01:43] And I guess I should start announcing it to everyone. So I needed to narrow down like my focus on things
[01:52] and I focus as everybody. I will still have a lot of random stuff on the show
[01:56] that is not going to go away because that is my pure curiosity.
[02:00] Yet there will be more focus. And to no one's surprise,
[02:05] it's going to be Postgres because that's what I'm learning
[02:08] and I need to do something for work. And I'm actually really curious about it.
[02:11] They have Elephant as the database. And then we have Redis,
[02:17] which is another relational database, but it's like goes on.
[02:21] We'll go into that later. And then TypeScript, I'm excited.
[02:28] TypeScript has helped me understand JavaScript better. - Heck yes.
[02:34] Heck yes, it has. TypeScript makes everything better with JavaScript.
[02:38] - Yeah. And so for all of those who do not know,
[02:42] Josh is the author of, I have to see what I did with it.
[02:46] Oh, yay. Learning TypeScript.
[02:51] And has been coming on for, apparently this is our ninth episode
[02:57] since probably, I feel like we started streaming in like October, maybe.
[03:04] - Maybe October, maybe November. - Yeah, something like that.
[03:08] And we've gone through many of the chapters and worked through things.
[03:12] And we finally came up with our flow. And remind all of us
[03:17] because you are a maintainer on ES Lint. - TypeScript ES Lint.
[03:23] A project that is neither TypeScript nor ES Lint. - Okay, so TypeScript ES Lint.
[03:29] And can you drop a link to it? Because I feel like people have been curious
[03:33] and I always forget to ask about it. And I'm like, it's important.
[03:39] We need to learn about this stuff. Okay, cool.
[03:44] - The tooling that enables ES Lint and Prettier to support TypeScript.
[03:47] The whole naming thing is hard and this is the best we've got.
[03:51] But it's like a really critical piece of the TypeScript ecosystem.
[03:54] Like the vast majority, like more than 95% of projects that use TypeScript use us.
[03:59] Because if you use ES Lint or you use Prettier, that is how those tools that natively only work
[04:05] in JavaScript can support TypeScript code. - That's cool.
[04:09] I had no idea. Well, I think you've said it.
[04:12] And this is something that I've learned a lot about as been learning live,
[04:17] is people can say things, but without the other knowledge, it never made sense.
[04:22] - Yeah, it's just words, right? Oh, he does the ES Lint thing, yeah.
[04:26] - Yeah, yeah. That's probably what I told people too.
[04:29] And Lex, I am, you're loving a little TypeScript moment. Is there anything you're looking forward to learning
[04:36] or want to ask Josh before we get started? Just like a random, you can ask him,
[04:42] "Hey Josh, you just got volunteered for an AMA, thanks." - Oh, no.
[04:46] - I will, well, we can start with this in the meantime. - Features.
[04:57] So you've understood the core concepts of TypeScript. Like you've gotten through that part of it.
[05:01] All that's left now is like various ways that TypeScript represents different things
[05:05] using those core features. - I'm excited.
[05:09] - And Lex, you've been working for it for three months and now at a basic level, that is good, that is good.
[05:16] I feel like I'm at a, I don't know what level. I'm at a, I'm gonna figure it out level.
[05:20] That is where I'm at. I will say for myself and y'all,
[05:28] I know that I've mentioned this before, this will continue. There will be highlights writing and things like that.
[05:35] That hasn't changed. One thing that is really, really helpful
[05:40] is that we talk about like type annotations or unions and that type of thing.
[05:48] And I'm like, I know what it is, but I don't remember what it is.
[05:50] So to do so, I end up going and getting it and then putting it where I'm relearning it.
[05:57] So I don't have to go back many, many pages again. 'Cause for some reason to learn the words is not clicking.
[06:05] - Sure. Ooh, Lex, I feel like we need to hear more
[06:11] about your full stack apps. Like that is pretty exciting.
[06:16] - Yeah, plus one. - All right.
[06:20] So today we're learning about functions and I moved the summary up here,
[06:25] which I'm very excited about. So, oh, you guys wanna see something cool else
[06:30] that I learned? We can have a follow dot thing.
[06:37] So you can see where I'm moving the cursor. This is just kind of weird,
[06:41] but so we are gonna be learning about declaring function parameter types
[06:47] with annotation, type annotations, declaring optional parameters,
[06:52] default values, rest parameters, and change type system behavior.
[06:57] Function return types with type annotation, functions that don't return a usable value
[07:06] with void type and then, or any value with never type,
[07:10] and then using function overloads to described varying function call signatures.
[07:16] And half of this chapter really made sense. And then I went, what?
[07:23] And I feel like that is also, so for those who don't know,
[07:29] I also am coming into this, not fully understanding just regular JavaScript.
[07:36] So I've never taken a course. I have never like taken a bootcamp
[07:40] or anything like that. 99.9% of my learning has been live
[07:45] or me working on my own website or projects, but most of it has been here.
[07:51] Ilyan, hello. - Ilyan, hello.
[07:55] - Yeah, is it Ilyan or Ilyan? - Can I make a guess? - Yes, guess.
[07:58] - I heard dance. I thought I had it right.
[08:01] And then I heard Danji dance in a different way than me. So I apologize.
[08:05] I should have asked in private. I keep forgetting to.
[08:07] Anyway, I want to make a guess of where your feelings are for each of those list items.
[08:14] Can I? - Yeah, wait, wait, wait.
[08:17] Give me like two seconds. Let's highlight the ones that you think
[08:20] I'm having a hard time with. So go ahead.
[08:22] - I think the first three you're fine with. That's my guess.
[08:26] - Okay. - If I'm wrong, I'm wrong.
[08:28] The next two, so the void type and never type, you're like, okay, this kind of makes sense in isolation.
[08:32] I don't see why I'd use it. Or like, maybe it doesn't like quite click,
[08:35] but like it's kind of okay. And then the last one, you're just like, what?
[08:38] No, I don't understand. Is that, that's like a lot of people go through.
[08:44] So that's just like a general common case. Is that yours?
[08:48] - I would say, I think it's more parts of this one.
[08:57] I don't remember which parts because we'll scroll through and find out.
[09:00] And, oh, I just looked up. Thank you for the follow, follow stuff.
[09:07] I'm like, what words am I trying to say? And also their name at the same time, it doesn't work.
[09:12] Medeo, I'm horrible at names. So y'all can make fun of me for that.
[09:19] And also tell me how to say it and I will try to be better at it.
[09:23] But thank you for the follow. And so I'm pretty sure it is,
[09:31] I think, I'm also really bad at the names. I think it is these two
[09:38] because the, for void type and never type, I was like, I doubt I'm ever really gonna use these.
[09:46] So like, and they make enough sense that I'm like, meh. Okay, I know where to go back to get them,
[09:53] but I didn't like go, I really need to understand this. Oh, I know where it was, but we'll get there.
[09:59] We will get there. We're gonna see if I'm right based on my memory.
[10:03] - Okay. - We'll see, we'll see.
[10:06] All right. So please tell us a little bit about why is this the,
[10:13] like, why did you split out the, you know, the sections? Why is this the first chapter of the section?
[10:19] What was your mindset behind that? - Sure.
[10:22] So to recap, this is the first chapter in the features section of the book.
[10:27] It's core concepts, features, and then what? What did I call that third one?
[10:33] At this point, I forget. I'm a terrible author.
[10:35] Concepts, features, and extra credit, I think we've resolved.
[10:40] This was like a whole discussion. - Usage. - Oh, usage.
[10:43] Usage and then extra credit, that's right. I know what I wrote.
[10:46] It wasn't chat GPT who wrote it. This came just before that whole thing.
[10:51] So yeah, the reason why I split that up is in order to really use TypeScript effectively,
[11:00] you really want to understand the core concepts. You don't have to like truly know them completely.
[11:05] Like it's fine to be a little shaky, but like they're really useful.
[11:08] So just going over the core concepts of what's a type system? Why did he even want it in the first place?
[11:13] And then how a type system works with objects and unions and narrowing.
[11:17] That's the core of TypeScript. That's the juice.
[11:19] That's what sets it aside from other equivalent type systems.
[11:23] And I feel like it was a very interesting time because last week was, was it last week?
[11:30] I think it, oh, it was two weeks ago. I'm looking.
[11:33] Narrowing, narrowing, narrowing. Why am I being blind right now?
[11:40] Oh yeah, it was three. It's right.
[11:46] I want to do yellow. - Second subsection in three, yeah.
[11:51] - Thank you. If y'all can see it okay.
[11:54] I feel like yellow is really hard to see on screen. We'll go blue.
[11:58] How about blue? Blue.
[12:00] We talked about narrowing and I figured out what we were talking about.
[12:07] And now I went from any, and I'm starting to narrow my life.
[12:11] It's a really weird feeling. It's really weird.
[12:13] - You're widening your knowledge and narrowing your types. Good, good, good.
[12:18] That is definitely what is happening. So why functions as the first chapter?
[12:25] - Sure. So we've covered objects.
[12:27] That's like a core part of the thing. And the next thing I generally want to talk about
[12:34] is if I don't have any specific need going to be the next most useful thing.
[12:37] And functions are all over the place in JavaScript. The only core concept that happens more often
[12:42] than functions is objects, which is the previous chapter. Additionally, functions show up in a lot of other places.
[12:49] For example, when we cover interfaces, which is like another way of describing object types,
[12:54] there's a difference between how you represent different types of properties or methods that are functions.
[13:01] The difference between a method and a property that happens to be a function.
[13:05] So in order to explain that well, we really want functions first.
[13:09] - Okay, okay. And it was definitely interesting
[13:14] because we saw how the type annotations went into this and we ended up going down a bit of a rabbit hole
[13:24] of talking about variables and stuff, which was very helpful.
[13:27] Thank you. And I just went and added it over here
[13:32] of type annotations. And this really helped when we were...
[13:41] I think the second part of this that I did not bring over,
[13:46] but was, I like this example of like, let rocker be string and rocker equals Joan Jett.
[13:53] So they both equal, rocker equals Joan Jett and string equals rocker.
[14:02] Anyway, I liked it. It made more sense that way.
[14:07] And then function parameters, I highlighted that when you're taking it
[14:14] and I just wanted to verify on this one. Tell us a bit about function parameters
[14:20] before I just totally butcher this, please. - Yeah.
[14:24] Have we covered the difference between a parameter and an argument, the terms?
[14:32] - I don't think so. And it was funny because I was just thinking about that
[14:35] while I was going through this chapter. I was like, I don't think we did,
[14:39] or I don't know if the book does. Honestly, I don't know.
[14:43] - Oh boy. The book, I don't remember whether I explicitly say
[14:48] this is the difference between them. I'm looking it up now,
[14:51] but it's certainly in the glossary at the very least. Let's see.
[14:57] I'm just kidding. Anyway, an argument is something you give.
[15:05] Like both, that's how I remember it. An argument is something you give,
[15:08] like I'm giving my partner an argument or something. So like when you call a function,
[15:11] the argument is the value you're providing or the arguments are.
[15:15] So like if I say console.log string hello world, string hello world is the argument.
[15:22] Full stop for now. Does that make sense and sound reasonable?
[15:26] - Does it have to be, because when you say give, it makes me think input.
[15:34] Is it something that's input or is it something that if you just wrote string
[15:40] in the console log, it's fine? Or is it a, you have to like run the program
[15:47] and manually type it. - Here.
[15:53] Lex in the chat is a great idea. Let's give her an example.
[15:56] There we go. Cool, yes.
[15:57] Function parameters, you zoomed out. I'm also putting something in the chat.
[16:01] In this example, like to console.log, this template literal string singing song,
[16:07] that string is an argument. You're providing to console.log.
[16:11] You're giving to console.log. - So this part is an argument.
[16:19] - No, no, no, no, no. The next line is the argument.
[16:21] - Okay, that's what I thought. Okay, cool, cool, cool.
[16:23] - It's specifically not the whole line. The string, the template literal string,
[16:27] singing colon, then the interpolation, the shenanigan, that string, including the exclamation mark
[16:32] and last tick is the argument. - Let's go to the highlighter because it likes it better.
[16:39] - Yes, yes in the chat. Yes to Lex, PG Lex.
[16:46] So yeah, the thing you've highlighted is the argument. The argument is something you give.
[16:52] - Okay. - Does that make sense now?
[16:54] - Enough. I think I will say arguments and functions
[16:58] are something that are like thinking about annotations and unions.
[17:03] I'm like they're words. They mean something.
[17:05] Like I understand it when somebody explains it to me, but it takes a little bit to code.
[17:12] - That's okay. A couple notes.
[17:15] One, same. Two, no one ever remembers the difference
[17:19] between arguments and parameters unless they work in tooling that works with code ASTs,
[17:24] like the structure of the code the way people like me do. So like all over the place,
[17:28] you're gonna see people use the terms interchangeably, which sucks because they're getting it wrong.
[17:35] They're inaccurate, but it's also good to know that like it's totally fine
[17:38] to get it wrong. Like no one cares really.
[17:41] But anyway, I care. And the argument is something you give.
[17:44] The parameter is something that the function declares. So song would be a parameter in this written example.
[17:50] - Oh, I did a person. I want the whole thing.
[17:54] Maybe, good enough. So a parameter is what it calls.
[18:00] - A parameter is what the function calls the thing. In this case, song.
[18:04] - Okay. I'm going to something else
[18:18] to see if I can get a different example. - Yeah, sync to first and second are the parameters.
[18:28] - Okay. - By the way, we could just ignore this altogether.
[18:38] Like as if you don't want to spend time just like exhaustively detailing the difference
[18:44] between parameters and arguments, like you can totally understand this whole chapter
[18:47] without remembering the difference. It's intentionally done like that.
[18:49] But I do like that you're going into this. - I would say that it's something that I appreciate
[18:55] when people come onto the show is a lot of people can notice the nuances
[19:03] that may not be written in something. Ooh, as I throw my pen at myself.
[19:07] And there is context that may be needed that people don't have to begin with.
[19:11] And especially since we talked from the very beginning many months ago that I'm not going to be a JavaScript pro,
[19:19] this is something that I may not have asked, but is going to be very helpful.
[19:23] And a parameter is the value that a function requires to be passed
[19:29] because it's going to use that value somewhere in the function body.
[19:34] Ooh, okay. So.
[19:39] - That's a good definition. - Is it only song that is the parameter?
[19:44] - Yes, in this particular function, it takes in exactly one parameter named song.
[19:50] - Yeah, that can highlight everything. There we go.
[19:54] - Alexis is like, yes, nailed it. - I like this.
[20:01] Alexis, where have you been? Like you just like suddenly showed up in my world
[20:05] and I'm very happy about it. Like seriously, she was on like the JavaScript jam,
[20:12] Anthony's Twitter space. And then like, she's in Jacob's Twitter spaces
[20:19] and makes me really happy. And then she keeps showing up here and I'm like, yes.
[20:23] - Yes. - I like making new friends.
[20:25] Okay, cool. So this is making sense.
[20:30] - Oh, I'll see you in Miami then. Awesome.
[20:32] Shout out React Miami. - Yay.
[20:34] React Miami. - Wait, Jen, are you going?
[20:38] - I am not going. - Oh.
[20:40] - Yeah, no. Well, A, I didn't find out about it till like what?
[20:44] Last week. So that's one part.
[20:47] And B, it is the two days. Like it's what?
[20:54] Thursday, Friday. And Saturday, I have to leave for Portugal.
[21:00] So it would be a little too much because after Portugal, I'm going to Munich.
[21:05] It would just be, as I have to say in my world, I'm not Dan.
[21:09] Dan like is like magic. He's going to like all of these places
[21:13] and gonna be gone for a month. And I'm like, "Dude, me going for a week?"
[21:17] And I'm like, "No." Okay, let me.
[21:20] I'm going to copy and paste this really quick so I don't forget her answer.
[21:28] Okay, whatever. That works.
[21:34] Cool. I dig this.
[21:37] And then I highlighted it down here to see if I understood what it was.
[21:42] And without knowing it, I understood it, even though I couldn't put words into what I was learning.
[21:48] That is one of the hardest parts about learning is being able to repeat it back to someone.
[21:53] - Yep, for sure. - It might make sense to consume it,
[21:56] but to say, you re-say it, not so much. And then required parameters.
[22:04] Anything you want to say about this before I talk about a few things?
[22:09] - Yeah, I want to go back actually 'cause we kind of glossed over it.
[22:12] I just want to make sure it's solid. So a parameter can receive a type annotation
[22:17] similar to variables saying, whenever you give me something for this,
[22:21] whenever you give me an argument, it must be that type. If there's no type annotation,
[22:25] then TypeScript doesn't know what it's going to be in most cases.
[22:28] So any, YOLO. Same with a variable that starts off
[22:31] without a type annotation or initial value. But in Function Sing version two, later down,
[22:36] we say song is type string. So the parameter song is type string.
[22:41] And anytime you provide or give an argument, that argument must be assignable to string.
[22:46] 'Cause if you give it like a number or something, heavens only knows if the Sing function
[22:49] will work with that argument. Does that sound good to you?
[22:54] - That made sense. And I think this is where I get confused later on
[22:59] is because it infers different things. So we'll get there.
[23:08] But where we're at right now, totally makes sense. And yes, Lex, where does Theo live?
[23:16] Is he in Atlanta too? Because Dan's in Atlanta, right?
[23:22] I don't actually know where. Oh, okay.
[23:26] Yeah, I'm always like, where do people live? I don't know where anybody lives.
[23:33] Okay, so required parameters. This made sense in the fact that it was saying
[23:42] first is a string, second is a string. And so therefore it was two required parameters.
[23:50] And so I don't know how I keep doing that on my pencil when that pops up.
[23:56] So please. I thought Dan wasn't going to render.
[24:04] So maybe, I don't know. 'Cause I thought he was going to.
[24:09] I don't, I can't keep track of everybody. I can barely keep track of myself.
[24:13] I don't know what I'm ever doing. And then, so all of this made sense of like,
[24:20] hey, we only have one thing defined. So it's expected two arguments, but got one.
[24:26] And then we got two, which was okay. We got three of them.
[24:31] And it was like, no, bro, that's too many. And so in this, before we get to the text,
[24:38] I said, if I add a question mark right here, will this fix the error?
[24:45] And creepy, yes, it would. As an optional parameter in the next one.
[24:52] And optional cannot be first. It can only be the second.
[24:56] - More generally, you can't have any required parameters follow an optional parameter,
[25:03] because that wouldn't make sense. - Oh yeah.
[25:07] Okay, well, I'm just kind of leaving it back. It's like, it works for me.
[25:14] - Yeah, I mean, but what your intuition makes sense. Like what you're going for here is totally reasonable.
[25:19] I'm really, as I was saying before, I'm really excited that like,
[25:21] you're getting these intuitive punches. The question mark means optional.
[25:24] That's a TypeScript thing. And it means that for object types,
[25:27] and it means for function parameters. - And so this is what the optional parameters
[25:32] were saying is that, you know, we have the string as the first one,
[25:40] and then we have the singer with the question mark. And therefore that is why that it is optional.
[25:46] What doesn't make sense, which I don't know where I actually asked this.
[25:52] Let's scroll. Okay, yes.
[25:54] I will ask in the next one and then it'll make sense. But optional parameters totally made sense.
[26:01] It was, we talked about it a lot more in one of the previous streams
[26:05] about what the question mark means. And that was really helpful.
[26:09] So thank you. And then we go into default parameters,
[26:17] which tell us about this one. What were your thoughts here?
[26:23] - You know, I went back and forth whether I wanted to teach default parameters
[26:30] before or after optional parameters. It's a joke somewhere about optionality ordering.
[26:35] I see a default parameter as like the next step up from an optional parameter.
[26:39] Like an optional parameter defaults to undefined if you don't provide an argument.
[26:45] I'll say that again, because that's like really good usage of the words
[26:48] and I'm proud of myself. An optional parameter defaults to undefined
[26:52] if you don't provide an argument. A default parameter lets you customize
[26:57] what that default type is, or what that default value is.
[27:01] So like in this rate song function, instead of rating defaulting to undefined,
[27:04] it defaults to zero. - Because we said the rating equals zero.
[27:09] - Yeah. - Okay, cool.
[27:13] And that was put right here. Where I got lost,
[27:19] and I'm starting to get lost in this, is rating is inferred to be a type of number.
[27:27] - Is that because it's equals zero, therefore it knows it's a number?
[27:32] - Yeah. - Okay. - I don't think you're lost.
[27:33] I think you're doubtful. - Maybe. - But you know the truth.
[27:37] You're just not sure of it. - Yes.
[27:39] Okay. And then if five star says the highest number,
[27:50] it can be five. Yeah, is that due to the exclamation points?
[27:55] Because in this, in a lower one, it's like this one says 100,
[28:01] but it says-- - Oh, wait, wait, wait.
[28:03] Hang on a second. That exclamation point has nothing to do with TypeScript.
[28:05] That's inside the string. That's just me being clever and cute
[28:08] with how I console log. That exclamation mark is not syntax code.
[28:13] - Okay, that is good to know. I need to write that down.
[28:17] And only because that is the problem with not knowing the stuff beforehand,
[28:21] is you don't always know what is actual and not, so. - Yeah, we should cover this before going actually,
[28:30] 'cause I use template strings a lot. This backtick string is different from normal,
[28:36] like single apostrophe or double apostrophe, quote, whatever strings.
[28:40] And the only difference is that you can, it's more easy to like shove values into it,
[28:45] like concatenating strings. And that dollar sign squiggly, something squiggly syntax
[28:51] is like string concatenation. Well, I'm gonna show you,
[28:56] I'm gonna send a link in the chat for TypeScript Playgrounds real quick.
[29:00] So, Ponce. - Do you wanna share your screen?
[29:03] 'Cause I know we've done that in the past. - I totally forgot we do that.
[29:06] Yeah, yeah, yeah. That'll be easier.
[29:09] All right, sharing the TypeScript Playground tab. So, can you see the console log?
[29:13] Hello, world. - Yes.
[29:15] - Awesome. So, let's say you have a console first name equals Josh,
[29:20] and you do like a const value or const message equals, and I'm doing the backtick.
[29:26] My name is Josh. And his first name.
[29:32] And it is nice to meet you. And hello.
[29:37] Let's just say shorter message. So, on the left is TypeScript,
[29:41] on the right is the equivalent JavaScript. And if we down pile down to like old,
[29:46] oh my God, they switched it on me. Dang it.
[29:51] Well, in theory, this actually means my name is plus first name plus and hello.
[30:03] That's what the string means. These two lines do the exact same thing.
[30:12] And I just use this form, the second one, because it's a little less syntax.
[30:17] Like it's just shorter to type out. Does that make sense?
[30:21] - It does. Can you copy and paste that to me so I can like,
[30:26] I guess I could screenshot it really quick. - Or I could copy and paste the URL in the Twitch.
[30:33] - That works too. - Yeah.
[30:37] So, if you run it and then look in the logs, my name is Josh and hello.
[30:41] It's, this is called interpolation, which is like a fancy variant of concatenation,
[30:47] which is a fancy way of saying combining strings, like adding strings to each other.
[30:52] - Okay. Not language syntax.
[30:54] And this is the URL and it's, what did you call it?
[31:03] Concat what? - This is string interpolation,
[31:10] which is a variant of string concatenation, which is like a way to do string concatenation.
[31:19] String concatenation is combining strings, concatenating. - We'll add that in later.
[31:29] - This is not relevant to functions. Other than that,
[31:33] it's just a thing that I use a lot in this chapter. - And I think that goes to my last part of this,
[31:40] which is, that helps if you guys can see what I'm actually doing, huh?
[31:45] 'Cause I, yeah, I know. This is one problem that I keep doing
[31:50] is like people will have to remind me I'm not sharing my screen.
[31:53] And I'm like, damn it. My bad.
[31:55] - Life is hard. - So right here,
[31:59] I guess I'm going to use a little pointer. You use the backslash.
[32:04] Is it the same or different than the, than-
[32:10] - That's a forward slash. - Okay.
[32:13] - That's a thing that's irrelevant. It's just part of the string.
[32:15] - Okay, this and- - Oh, sorry.
[32:19] You're talking, that's the, like the vertical pipe. - Yeah, the vertical one.
[32:23] - Yeah, that's the type union thing. - Okay.
[32:27] - And then in the string, you have the forward slash, slash five.
[32:31] That's again, that's like the exclamation mark. That's just part of the string.
[32:33] That's just like three out of five, like three slash five. - Cool.
[32:37] Yay. - Yay.
[32:42] - Well, now I'm going to, I have a new follow-up question. If we did a console log on this,
[32:48] why didn't it show three out of five right here? - It would log five out of five.
[32:55] - So it just won't say, it won't type in. - It would say, well, first of all,
[33:02] you can copy and paste this into the Hexcode Playground. Like that's something I'd encourage you to do
[33:06] if you're ever curious what they do. But second of all, I can fast forward to the answer.
[33:10] That second rate song would say, Sapphire, the rain gets five out of five stars,
[33:14] exclamation mark. - Okay.
[33:18] I think that's where I was getting confused as I was expecting this to show that.
[33:24] And okay, that totally makes more sense. Yay.
[33:29] Yay. Thank you.
[33:30] Okay, cool. - Yay.
[33:32] - Now on to rest parameters. - Which if I remember it was basically
[33:44] doing the square brackets to show that it's gonna do an array.
[33:52] - Yes. The dot dot dot is a JavaScript feature
[33:55] that TypeScript now has to support. If you say that the last parameter
[33:59] in a function has dot dot dot before it, that means it's gonna be an array
[34:03] of whatever number of arguments people provide. So like you can see, sing all the songs.
[34:10] We can provide none or we can provide like three and that's okay.
[34:16] Either way, song is an array. - Is there a limit to an array?
[34:21] - Only whatever your runtime environment will allow, which is basically huge.
[34:27] Whatever thousands or millions. - I'll still put that.
[34:30] - Good question. I'm looking at stuff that drops you a max array size.
[34:38] A 4 million, wait, 4 billion? 4,294,967,295.
[34:47] I will quiz you on that number in seven months time. So be sure to memorize.
[34:52] - I'm just gonna be say this. Runtime, whatever runtime allows.
[34:59] So technically yes, but probably it's never gonna find it.
[35:02] - Billions. - Cool.
[35:05] And that made sense. And oh, this was my fact checking myself
[35:11] that if I added quotes to this, it would be correct because it would be a string
[35:17] instead of a number. That was exciting notes from the learnings.
[35:24] Okay, return types. Ooh, this was the first part that I got really stuck on.
[35:31] And I also figured out how to put an emoji in. I just figured that out today.
[35:37] I also just figured out today how to highlight and how to make boxes.
[35:41] So we're definitely lots of learning. - Hell yeah.
[35:47] - I am curious going back to the beginning. Reset parameters, return type.
[35:56] Neither one of us said return types. Neither one of us.
[36:00] - Oh, I said the first three. Like I thought, I assumed you'd be okay with return types
[36:04] or hoped, projected would be the right term. 'Cause everyone's different.
[36:09] Some large number of like, I don't know, 30 to 50% of people are fine with the first half
[36:13] and then the second half is where they start. But you know.
[36:17] - I know. I think return types are just like where,
[36:20] 'cause it does, this is one thing I really enjoy about reading your book is there,
[36:27] it does definitely build on top of itself. And that makes it really easy to start learning it.
[36:34] Although when I start to see that I don't get something, I'm like, I can get overall concepts,
[36:39] but it's not going to entirely make sense until I understand this first thing.
[36:43] - Yeah. That's the beauty and the terribleness
[36:46] of building on yourself. Like, yes, it means that you learn
[36:49] as little as possible at one time, but if you miss something, you're missing the rest, right?
[36:54] - Yes. So could you tell us a bit about return types, please?
[37:03] - Sure. So I will say that for the rest of the book,
[37:08] the building on itself and needing to know prior things, it's there, it's always there in every tome of knowledge,
[37:14] but it's less so now that we're doing random features instead of concepts.
[37:20] They do build on each other, like there is order, but less so.
[37:23] So this singsongs function, it returns something. Unless it crashes, like unless like, I don't know,
[37:32] some whatever weird thing happens, songs is undefined, somehow it'll return something.
[37:38] What would you say the type of that return value to be? And I'll give you a hint,
[37:44] it's one of the types that you copy and pasted on the right.
[37:47] - So I think this is where I was starting to get confused because like, I see how it's up here,
[38:01] it's talking about that it's a number. - Ignore that, that's cheating.
[38:05] I'm asking you a question that's answered in that line. Don't look at the line, just intuitively.
[38:09] Like if I were to tell you, oh, I'm calling singstongs with something
[38:13] and we're storing that results in a variable, what type of that variable be?
[38:16] - I would say a string. - The returned results from singstrongs,
[38:20] what type is songs.length if songs is an array? - If it's length, then it would be a number.
[38:26] - Exactly. This function returns a number
[38:29] because it has one return statement that returns statement returns something that's typed.
[38:33] Number. - Oh.
[38:35] And for Kai, yes. Yes.
[38:41] - Okay, so this makes sense. So,
[38:51] well, that didn't work very well. And plus that's not a very easily seen color.
[38:55] Let's try a bright pink, see if it helps. Probably not, but so songs.length
[39:02] is how I would find a number. I just want number.
[39:06] That makes way more sense. - Yeah.
[39:10] - Oh. - Yeah.
[39:16] - Okay, before I keep going, I also copy and pasted types
[39:21] because we talked about this earlier. It's what I like to do, copy and paste from past.
[39:25] But as we are learning other things that are not associated with TypeScript,
[39:33] do you know, are types the same in every language or thing? Like for Postgres,
[39:40] would Postgres be learning the same type of types? - I'm honestly glad you prepped me with this question
[39:46] like, whatever, 45 minutes ago. I'm glad you did.
[39:49] No, everything represents types in a different way. For example, JavaScript and TypeScript
[39:56] which we'll lump it together, they have things like strings and numbers.
[40:01] A lot of other languages like Java, C#, Python, they have more specific versions of number.
[40:09] They have like ints and floats and doubles and like different ways of representing
[40:13] the concept of a number. This is just how things are.
[40:18] Every language is built for a different set of purposes. And those sets of purposes dictate
[40:23] what design decisions they make. Like, do you have one unified way
[40:28] of representing numbers or two? Or do you have like 14?
[40:30] And as a result, it's a little annoying because now everything considers something
[40:35] to be slightly different, like a number in TypeScript. Well, if you just have a number in TypeScript
[40:40] and then Postgres represents things in like ints or floats or whatever, like it's not the same.
[40:44] So yeah, everyone does that slightly differently but the core concepts are all pretty similar.
[40:49] - I am saying that it's different terms and definitions because like number for the numbers example
[40:59] is in TypeScript is numbers, but as you said, it goes to int in Python
[41:06] and that does technically they're around the same thing but they're technically different terms.
[41:11] So therefore the terms may have similar but different definitions too.
[41:17] So I think this is a yes and no. Okay. - Yes and no.
[41:23] - Yes and no, that makes enough sense for them. All right, so.
[41:28] - Wait, yeah, let's actually stay on this page for just a little bit.
[41:35] I wanna look at this thing, getSongAt. Because a function, every function has one return type
[41:43] but that return type might be a union. Here we're saying getSongAt can return
[41:48] either a string or undefined. Does it make sense why that's the case?
[41:53] - I'm gonna stare at it for a second. - Sure.
[41:59] - Is it because the string is an array? - Why, 'cause songs is an array?
[42:14] Yeah. - Yeah. - So there are two possible things
[42:17] this function could return. It could either return songs of index,
[42:21] which is type string as you just alluded to, or it could return undefined, which is undefined.
[42:26] And the reason why is 'cause this is a ternary statement. It, are you familiar, have we gone over ternaries?
[42:31] Are you familiar with these things? - I don't think we have.
[42:34] - Cool, let's, how about I share? - Okay.
[42:38] - Take over these things. - So a ternary statement is like a,
[42:41] like a shorthand for using. - Can you share your screen real quick, please?
[42:45] - Yes, cool. So a ternary is saying const result equals if true
[42:52] or some condition, if true, if false. That's how ternaries are structured.
[42:58] It's like, if some condition, const if true equals array,
[43:09] if false equals. So in this code, we're saying result is either array
[43:16] or oh no, it will be array if some condition is true. And it will be, oh no, if some condition is false.
[43:25] - Okay. - It's another way of saying this would be like,
[43:27] let results, if some condition result equals if true, else results equals if false.
[43:37] These aren't quite the same because this is a let and not a const,
[43:43] but like generally these, this ternary is like a quick way of writing the if else.
[43:50] Does that seem reasonable? - Yes.
[43:55] And so because of the songs, the songs, yes and no.
[44:05] - Okay, so ignoring the function, the song stuff, the reason why that function is string
[44:16] or undefined is because of a ternary. Because here I'm gonna actually start a new here.
[44:23] So first I'll send this particular snippet in the chat. Ternaries makes conditions look pretty,
[44:30] a strong degree, that's why I use them. So let's say that you have a function saying songs
[44:34] or get song gap, what's it called? Which takes a song string and an index number.
[44:43] And we're saying if index less than songs dot length, return songs of i or index, otherwise return undefined.
[44:54] This is the same as what you saw in the book. It's just using an if instead of a ternary.
[45:00] Does this make sense? - Yes.
[45:04] - Ultimately we could say it's like else return undefined, but there's no need to use an else
[45:08] because we returned on this line. So we can just say if.
[45:12] - Okay, so it's, thanks Lex. That does make sense.
[45:22] And I feel like it's kind of like the other part that you were talking about earlier,
[45:29] the, when something is shortened. - The fact that sugar.
[45:35] - It's like another one of those areas that I'm like, oh, it's saying the same thing.
[45:40] It's just the way that I'm seeing it. It didn't make sense to me, but it's the same thing.
[45:45] - Refactoring syntax sugar, yeah. - Yeah, okay.
[45:49] - Cool. - Okay, cool. - So that's why get song gap is a function
[45:53] that returns string or undefined. Because in one return statement, it returns a string.
[45:58] And in another possible return statement returns undefined. So we don't know what this function returns
[46:03] between those two. It's either string or undefined.
[46:07] - Okay, okay. - Sound good?
[46:10] - Yeah, that one is making sense. So I'll just add mine back.
[46:15] - Good synchronization there. - All right, so explicit return types.
[46:24] I did like this because you were like, probably not gonna run into this often.
[46:31] - Sweet. - So I still read it.
[46:33] I was like, you know, let me understand. And recursive, I was like.
[46:41] - Don't worry about it. - I'll Google it at some point,
[46:46] but that's why I have it highlighted. And then, oh, this is the other question
[46:52] came up in this area. Is a language used inside of a database?
[46:56] - The answer is yes, you probably should use it as little as possible.
[47:03] I'm curious, what is your context for asking this question? - It was the count plus one.
[47:15] So if you had an episode number, it would do a count plus one
[47:20] and automatically add an episode number. - Okay, yeah, so that's,
[47:25] I believe that's called a procedure. Is that the term you're familiar with?
[47:29] - I haven't gotten there yet, but sure. - Yeah, so there's like,
[47:33] there's the concept of an auto incrementing index where like it automatically knows to use the next number
[47:41] or like a unique, another thing. Every time you add something new,
[47:43] you don't have to explicitly say this one's four, this one's five.
[47:46] But then there's also the concept of a procedure in databases where you can have some code
[47:52] embedded in the database that's run on some actions. So yeah, there is stuff,
[48:00] like there are languages you can use in a database. There are very limited cases where that's really useful.
[48:04] However, it can be very difficult to work with. So people try to limit the amount of procedures they use.
[48:11] Like there are very specific cases where procedures are awesome
[48:14] and will be great for performance and simplicity, but I don't know enough about them
[48:21] to be able to describe to you what those cases are. - That's totally fine and super helpful.
[48:27] And Elian, we were talking about that earlier 'cause Lex got pre-rolls and I don't know why.
[48:34] I turned it off and everything. I'll verify after this,
[48:38] but I will tag y'all and switch and see if we can get an answer.
[48:46] I might have something clicked wrong. I do not wanna just say it's Twitch.
[48:49] I think it is, but you know. And then what did you call it?
[48:53] Because I started procedures. - Procedures, yeah.
[48:56] Actually, I think I misphrased. I'm not saying they're always not a great idea.
[49:01] I'm saying there are very specific cases where they're a great idea
[49:04] and many other cases where they're a terrible idea. - Yeah, okay.
[49:11] Thank you. I mean, in all seriousness, though y'all is,
[49:16] I've only had a job for two months and after being jobless for a year,
[49:20] people are like, you can do all this stuff. Like Dan was talking about this and I'm like,
[49:24] dude, dude, no, I wish. I do wish, but yes, okay.
[49:34] - Before we move on, I wanna shout out Alexandra Sikora. It's a regular conference speaker.
[49:40] Alexandra gave a really good talk at Prisma Day 2022 that I linked in the chat
[49:44] that goes through all sorts of wild and wacky fun stuff you can do with database procedures.
[49:48] I think the talk's in SQL, but like the concepts are applicable in a lot of languages.
[49:53] - Yay, thank you. I'm gonna put that in my notes, watch video.
[49:58] Cool. Okay, so this was also another thing
[50:06] that it actually does kind of build on top of arrow function and lambdas and it was, yeah, like looking at all of this,
[50:17] I need to, I really need to work on like breaking these down, but there are, like I said, they're a bit surprised
[50:31] you have to do a, oh, now you guys are- - TypeScript know that the array might not be big enough
[50:45] in the, sorry, Jen, would you mind going back to the sing songs at, or get song at function,
[50:50] the one we were looking at before this stuff? So yeah, a couple of reasons why I used the condition,
[50:56] even though I didn't have to. For starters, TypeScript put the idea of knowing
[51:01] that accessing an element of an array could return undefined behind a flag,
[51:05] because most of the time that's real annoying. Like if every time you access an array of some elements,
[51:12] you had to manually check whether that index was inside the array.
[51:16] I mean, there's some code bases that that's legitimately useful and they want that on,
[51:19] but most code bases that would just be like a total pain. And this is an area where TypeScript's type system
[51:23] is actually not completely safe. 'Cause I could do, I could say like const names
[51:28] equals an array with like one thing in it and to do names of 9,001 and TypeScript would be like,
[51:33] oh yeah, that exists, that's fine. So this is covered in the arrays chapter, which I-
[51:39] - Which is next. - Next, awesome. - I think it's next.
[51:42] Let's see. See if I can see it enough because I booked mark 'em all.
[51:48] Oh, it doesn't get bigger, why? Let's see, yes, but arrays is next.
[51:53] I'm like having to like really zoom in on this, but yes, arrays is next.
[51:57] - Yes, cool. I will also say in just ignoring TypeScript,
[52:00] like in JavaScript in general, accessing elements outside of the size of an array
[52:04] is like a performance paper cut. Like most of the time it's fine,
[52:08] but like if you have a hot code path, meaning a code path that's like run repeatedly
[52:12] over and over again, that's hot, then that like does de-optimize the code path.
[52:16] So it's in a general situation, it's oftentimes better to be safe to check
[52:22] whether it's less than the array's length, but like that's not sound performance advice all the time.
[52:27] - Fair enough, fair enough. - I wrote a game engine and that was a performance hell.
[52:33] But great question, thank you for asking. Oh, something fun to tell all of you
[52:41] to as I've been learning data and we had Ben Gamble on the show
[52:46] talking about data basics and apparently Josh, check your discord,
[52:52] is that I will be building a raspberry pie to understand data more.
[52:59] I'm very excited. This will be sometime next month, but okay.
[53:06] I feel like these two need to have their conversation first. - Go on, please, I'm with you.
[53:16] - When are we gonna stream, Ilyan? When?
[53:21] I've been like holding off website stuff. I should show that.
[53:25] If you're still here when we're done with the chapter, I have stuff to show you.
[53:30] Well, to show both of you, but like show everyone 'cause I'm really excited about it.
[53:35] Okay, so lambdas and arrow functions. Those are the same,
[53:44] but this doesn't really make a ton of sense to me. - By the way, this is a JavaScript thing
[53:57] that there are two really more, but like two main ways of declaring a function.
[54:01] You can do what's called a function declaration where you say like function, some name,
[54:06] the things we've been seeing before. And then you can also do an arrow function,
[54:10] which is, this is like, that's what it is. Fun fact, people used to call them fat arrow syntax
[54:16] and I will let everyone spend about two milliseconds guessing why the term fat arrow syntax
[54:21] is no longer the common term for this core language feature. And I'm glad that we realized, no.
[54:27] (Ilyan laughs) - That was funny.
[54:31] - So yeah, arrow functions sometimes also called lambdas. It's just another way of writing a function.
[54:36] There are like some small differences, but they're not relevant in this book.
[54:39] - Okay, so, okay. So basically these two for the one right above it
[54:53] for a function declaration, it's basically two ways of saying the same thing.
[55:01] - There are some small differences. Yeah, there is a reason why we have two to three ways
[55:07] to declare functions in JavaScript, but right now, not relevant.
[55:10] They're just two different ways of doing the same thing. You could also do const variable equals function something,
[55:31] and that's called a function expression. And that's so nitpicky and nuance
[55:35] that I didn't even bother including it here. - Thank you.
[55:38] Thank you for that. Okay, so is returning a date.
[55:47] This made sense. This wasn't too tricky.
[55:53] (typing) Okay, so this one made enough sense.
[56:03] And then you have function types and this got a little hazy.
[56:11] - Well, so you have to be able to describe all sorts of things in the type system.
[56:17] If you have a variable, that's a string, you can say it's a string.
[56:20] If you have a variable, that's an array of things that are number or string or whatever,
[56:24] you have to be able to describe that, always. They're objects, they're arrays, all sorts of things.
[56:30] Well, what if you have a variable that stores a function, which is like a really, not all the time,
[56:35] but like a pretty common JavaScript practice. You have to be able now to describe
[56:40] the type of the function. Like if you have a function that takes in another function,
[56:44] like arrays.map, you have to be able to describe the type of the parameter that is a function.
[56:49] And here, I give you the way to do that. Does that make sense?
[56:56] - I'm reading it and I think it does make more sense. I think sometimes, and this is something
[57:09] that I love about your book. And there are a lot of teachers out there
[57:14] that do this too, like your book is a little more common language, I guess is a way of saying it.
[57:23] Yet there are gonna be some nuances that just even while reading it or looking at it,
[57:28] it just doesn't necessarily click. So I appreciate you going over that one.
[57:33] That one does make a lot more sense. - Cool, on that note, sorry to interrupt.
[57:40] On that note, I actually got dinged in a couple of Amazon for like elsewhere reviews for not having
[57:49] like everyday language. So like this is something that I'm actively
[57:52] or was actively working on, but this book is incredible. I highly recommend it if you're writing blogs,
[57:57] if you're streaming, if you're doing conference talks, if you're writing a book on writing well by William Zinser.
[58:04] It's like one of the standard things for writers that I did not know about until like most of the way
[58:08] through writing my book. Put it in the chat.
[58:13] Great book, honestly, fantastic book. Even if you just talk to people,
[58:17] it's really good about like clear, understand book, comprehensible language.
[58:22] Don't use like three random words that mean the same thing in a row.
[58:25] Keep your sentences short because each sentence is its own idea.
[58:30] So thank you. I tried to do that in the book, but I came in late.
[58:33] There are parts that don't do it as well. - Ooh, and it is,
[58:43] is it? Yay.
[58:46] It is on Audible as well. - Yes, yes.
[58:53] - So definitely go check it out. I am excited that it is on Audible as well
[58:59] because well, that's how I learned. - So, yay.
[59:04] Okay. I appreciated that you included the errors.
[59:09] This is why I highlighted them. So I see them and come back to them
[59:12] because it made a lot of sense what these errors would have been.
[59:16] And then, so we have- - Wait, sorry.
[59:22] I just don't wanna skip over these things 'cause the assignability errors are like,
[59:25] they're gonna keep coming up in TypeScript, no matter what you do.
[59:28] So does this concept of like increasing indentation for each level of specificity in the error
[59:35] jive well with you? - Yeah, well, at least in my visualization of it,
[59:42] 'cause y'all, I did not go on there and actually go test it out.
[59:46] Yet, it made sense because if I'm looking up here, at least at these ones,
[59:51] it's talking about the level of indentation right here to see where if it's something that's readable
[59:59] to know that it's associating with the top one or whatever's above it.
[60:03] - Yes, that is a big part of why they do it that way. - Yep, exactly, I love that.
[60:08] - Oh, yeah, yay. Go Lex, you got this.
[60:13] - Ooh. - Thank you, Lex. - Good luck.
[60:17] - Okay, cool. But yeah, that's, I think, why I skipped over it
[60:21] because I was like, this totally made sense, was the indentation part.
[60:25] But a big part of this is because Python really does that a ton.
[60:33] And if you don't have the right indentation, Python breaks.
[60:36] So that actually, yay for learning Python at the same time for a while.
[60:43] I do think I am going to put that on hold so that way I can focus on narrowing down what I do.
[60:52] I don't know. Okay, anything before we go to function type parentheses?
[60:59] - Nope, thank you for humoring me. - You're very welcome.
[61:02] I appreciate the fact checks. You'll make sure I know what I'm saying.
[61:07] And I was very excited because Anthony had me explain the difference between Docker and Kubernetes,
[61:16] and I did a decent job. I was very excited.
[61:19] So as people quiz me on things, checking my understanding, I get better,
[61:24] or I just totally flounder. Okay, so function types,
[61:33] maybe you place anywhere that another type would be used that includes union types.
[61:39] So I grabbed union types from the previous chapter. And from what I understand is it's just saying
[61:51] that if you use mathematician over here, if I'm using mathematician and it equals math.random,
[62:04] I can use mathematician later on instead of reusing this. And that's what a union is, right?
[62:12] - Yeah, a union is something that could be either one or another.
[62:16] So. - This is literally just no unformatting.
[62:34] It doesn't introduce any new concepts. It's just letting you know there's a difference
[62:37] between this thing and that thing. - Okay, the only, other than the, like what is letting,
[62:46] it's, I see an, is it an extra bracket? Oh, no, it goes over there.
[62:53] I wasn't seeing where it closed. Yeah, parentheses.
[62:56] I wasn't seeing where it closed and it took me a second. Got it.
[63:00] Okay, parameter types. - This is where it gets funky.
[63:05] - Okay. - And that, by the way,
[63:09] this is the third way to declare a function. This is called a function expression.
[63:13] It's like a halfway between a function declaration and an arrow function.
[63:19] And honestly, you can ignore that totally and just pretend that all the syntax looks the same to you
[63:24] and you'd be fine. - Okay.
[63:27] Oh, okay. I wonder if, what is my question?
[63:36] Is index inferred as a number due to it being after songs and not a string?
[63:42] - Ah, that is a built-in method to JavaScript. In JavaScript, the language, the runtime, whatever,
[63:51] every array has, among other things, a forEach method, a property you can call.
[63:56] And that forEach takes in a function and it will call the function with three things.
[64:02] It'll call it with each member of the array or each element of the array.
[64:06] It'll, that array's indexed and then the array itself. Fun fact.
[64:10] That's just a JavaScript thing. - Right.
[64:17] What would I look that up as? Array types?
[64:21] - Array forEach. - That blue is not gonna be able to see.
[64:28] - I'm just gonna show in the, I'll put my, what I would look up in the chat.
[64:33] Other people's mileage may vary, as they say. We all might use different things,
[64:37] but I would look up like array forEach on Google. And then the first thing would be MDN for me
[64:41] because I like MDN and they know that. - Yeah. - So they make it good.
[64:45] So it executes a provided function once for each array element.
[64:49] And the parameters to the function, the first one is a callback that receives
[64:54] elements index array for each of the elements. - Okay.
[65:00] And thank you, Alien. - I think it looks like poop,
[65:07] but that's because I look at my handwriting all the time. But something that I think is really cool is they,
[65:17] there are now, what is it called? A screen protector that feels like paper.
[65:27] So it doesn't like make me cringe when I'm trying to write. So it's a lot easier to just use.
[65:32] Yeah, it's paper-like. So it's really easy to write on the tablet
[65:38] because I'm not getting grossed out from trying to do. - Paper-like.
[65:48] - Yeah. - Wasn't there some other fancy new tablet,
[65:51] like Remarkable? I've been looking, or I've seen people talk about it,
[65:54] and you need to look into it. - That is, I personally didn't like Remarkable.
[66:02] I tried it a long time ago. Thank you for the follow.
[66:06] I tried it a long time ago, but a big reason that I didn't like it back then
[66:14] was, I don't know if you could tell, but I need colors in my life.
[66:19] And if I don't have colors, I get really lost on things. Everything is very color-coded,
[66:26] me trying to figure life out. It's how I associate things.
[66:31] So without the color, and I don't believe Remarkable did color.
[66:36] From what I remember. - Darn.
[66:41] Oh, well, there go my hopes and dreams. - Okay.
[66:46] So function type aliases. - Yes.
[66:52] - I don't. - Fun fact, this introduces no new concepts.
[66:56] It's just rehashes old ones. Your favorite part of these later chapters.
[67:01] Combines them in new ways. - I was going to say,
[67:04] I think it made sense because I didn't put any notes on it. - I have no idea.
[67:11] - Yeah. - What if in the book,
[67:13] each section explicitly says what it does with regards to new concepts?
[67:18] Like does it introduce new concepts and or does it rehash or like recombine old concepts?
[67:23] I feel like that would actually be like kind of cool. - That would be helpful because like,
[67:27] if this was like, like let's say that it said build.
[67:35] So it's building on something else, new or recap. - My mind just immediately auto completed to,
[67:47] build, deploy, first cell, but that's not correct. But yeah, something like that.
[67:51] - Actually, oh goodness. Sabin, is that how they say their name?
[67:57] Sabin at Vercel? I think Sabin's at Vercel.
[68:00] Anyway, I need to have someone from Vercel or Netlify on again to understand the differences
[68:09] between old school hosting and like GoDaddy or HostGator or something and how Vercel does things.
[68:18] So yes, this one made sense. And more return types, void returns.
[68:28] When in real life would somebody actually use this? - Void returns show up all over the place.
[68:36] The most common example is a console log. It's not just that you're explicitly
[68:45] doing something different. It's that by default, all functions return void
[68:49] unless you add an explicit return to them. (mouse clicking)
[68:54] - Okay, that helps. Is there a reason you would want it to return void?
[69:11] Like, I guess if it does it, cool, but is there a time you would actually like,
[69:18] be like, I need to make sure this does this? - Yeah, it's similar to other cases
[69:23] where you'd want an explicit function return type. You don't have to, unless it's recursive, ignore that.
[69:30] But if you have like a larger function and you just want to make sure that like,
[69:34] there's no random like return zero or something in there. Yeah, it can be useful just to make sure.
[69:38] And it's like, this is at the level of stylistic preference for the most part.
[69:44] (mouse clicking) - Sure, we're gonna go.
[69:57] I'm using it as an example. We'll see if I remember what it means.
[70:04] Oh, and then up next, note that although JavaScript functions all return undefined by default,
[70:13] if no value is returned, void is not the same as undefined.
[70:19] Void means the return type of a function will be ignored while undefined is a literal value to be returned.
[70:28] - At first, when I like first got into TypeScript deep, like not just learned it,
[70:36] but like started getting really into it, I started to convince myself, like, why do we have a void?
[70:40] It's just, just say the thing returns undefined. But then when I got even deeper,
[70:44] I realized, no, I was wrong. TypeScript is right.
[70:46] A feeling that a lot of people go through frequently when getting into TypeScript deep.
[70:51] Yeah, there is an actual reason why void is not undefined because a function, a function can return something
[70:58] and then be used in the location that says, ignore this thing's return.
[71:02] So like, void is saying, I don't care what you return. You could return whatever you want.
[71:09] I'm not gonna touch it. Does that make sense?
[71:13] - Yeah. We're going with yes for now.
[71:19] In the future, it may not. - Sure.
[71:22] And this here is, this records thing is a good example. Like fun fact about JavaScript arrow functions, aka lambdas.
[71:29] They, they're used because they return whatever that first line is.
[71:34] Like, like if the, if you scroll up just a little bit to the four each, if you don't mind.
[71:40] Yeah, so save records. Sorry, too, too far.
[71:45] - Too far. Okay, I was like, where did I go?
[71:48] - There is a save records function. - Oh no.
[71:53] - Should we check page 71, I think? Yeah, bottom of page 71.
[72:01] - Ah, there we go. - Cool, so fun fact, a couple of fun facts actually.
[72:07] For one thing, a question, are you, are you familiar with the concept
[72:10] that JavaScript arrays have a push method that you can call to push something
[72:14] at the end of the array? - No, but yay.
[72:18] - That's, that's how you add to an array in JavaScript. You can do like records equals empty array,
[72:22] records.push something, and that adds to the array. That's a thing.
[72:29] That push method returns a number. - Okay.
[72:39] Wow, can't wait. Okay.
[72:50] Oh, that's cool. - Yeah, so it returns a number.
[72:54] It returns the new size of the array, which means that that, this little arrow function,
[73:01] this little lambda record thingies, records.push record, that function returns a number.
[73:08] - And is that, so would that be considered part of a lambda then?
[73:15] - I would encourage you to use the word arrow expression because lambda like means a totally different thing
[73:22] in like server or serverless tech. But yes, it means that this lambda,
[73:26] this like record, records.push, that, that means because records.push returns a number,
[73:31] that whole function returns a number. Could I share my screen?
[73:35] Just brief. - Yes. - Yay.
[73:38] Let me go back to the TypeScript playground. So like const version arrow equals records string,
[73:47] records.push something. And then you have the same thing, version function,
[73:55] takes in records and returns records up or something. These two do the same thing.
[74:02] Just one is the arrow syntax. The other is a function declaration.
[74:07] Both are records string return number. So note that these functions don't return undefined.
[74:19] They return a number. And if I were to run calling version function on existing,
[74:31] it would return two and log two. (silence)
[74:35] Okay, that makes sense. If you run it again, would it go to three
[74:43] or would it keep two? - Every time I call it, it's a new array.
[74:46] So like, let's say const my stuff equals this, so like version function, my stuff.
[74:55] First call. - You want to guess what this will run?
[75:04] - I'm hoping to three, but you know, I would think that it's a first call, second call.
[75:08] It would go to three, but okay. - Yeah.
[75:11] - But it will always do first call, second call. So it'll always be two and three.
[75:15] - Every time I run it, it's new everything. I'll just refresh the page to make it a little more clear.
[75:22] And then at the end, it's console.log my stuff. So at the very end,
[75:25] now my stuff is existing something, something. - Okay.
[75:31] - Cool. - Does that make sense?
[75:33] - Enough? - Cool.
[75:35] So yeah, so these functions return number. So if I were to provide either of these
[75:40] to a location that says, I would take in a function that returns undefined.
[75:45] Like let's say I did like, let this variable is a function that returns undefined.
[75:50] Undefined, let's say, or like input is a string. And then I said like this variable, blah, blah, blah,
[76:00] equals version, either of them, let's say arrow. TypeScript would be mad because I said that this function
[76:08] returns undefined, but the thing I'm providing to it returns number and number is not the same as undefined.
[76:15] - That makes sense. - Does it make sense why TypeScript's mad in this case?
[76:20] - Yeah. - Cool.
[76:21] Void says, I don't give a crap. Just do whatever you want.
[76:26] So void is okay with this because whatever I call this returns void thing,
[76:34] I'm completely ignoring the returns value. It could be undefined, string, number, whatever.
[76:38] I don't give a crap. - So for your example earlier of like,
[76:45] if I'm scrolling and lean to the thing, maybe, was that like you might use void to
[76:56] help find if there were zeros somewhere, or like if it gave an error,
[77:01] how would a void do that compared to a undefined? Void will still run them and undefined won't?
[77:09] - Void just says, you can give me more permissive things. Undefined says it must be undefined.
[77:14] So like an example of something that takes in void is the like array for each.
[77:18] Array for each says the parameter returns void. I don't care what you give me.
[77:22] You can give me something that returns a number or a void or undefined or whatever.
[77:25] I don't care. - Okay.
[77:30] Okay. - You don't have to,
[77:34] this is not gonna come up very often. In my experience, people have a lot of trouble
[77:38] understanding the concept of void, but when it comes to using it in code,
[77:41] it just intuitively makes sense. Like, because it's a more permissive thing,
[77:46] if you just like console.log or like array for each, it'll just work.
[77:51] And then you don't have to really memorize like what void does.
[77:54] - Cool. And then, 'cause we talked,
[78:01] do we end up talking about the never returns? I don't think we talked about.
[78:09] - We haven't yet, but this one is fun. This one I actually found easier to understand personally
[78:13] than void. It never returns.
[78:16] It literally never does. You'd never continue after this function,
[78:19] the end of the line. - So it's the opposite of a loop?
[78:24] - It's an infinite loop. It's a, have you ever seen while true?
[78:30] - Yeah. - It's a while true.
[78:33] Whatever comes after that, you're never getting there. Unless you like break out or something,
[78:37] but like that's not happening. - Okay.
[78:40] That totally makes sense. Function overloads.
[78:46] And I really want to say function overlords, but it's overloads.
[78:51] I tried to get these out of the book, actually. I went back and forth.
[78:55] I wobbled a lot on whether I wanted them in the book. And then towards the end, I was like,
[78:58] you know what, no one uses this. Like this is not necessary.
[79:01] It's like the random edge cases that most people don't hit. But by then it was too late to take it out.
[79:06] So now we're stuck with it. - Okay.
[79:10] That, then I'm just going to skip it. - We can skip it.
[79:14] - Call signature. - Sorry, I didn't understand.
[79:18] - Sorry, you triggered me. - Well, that's okay.
[79:19] I don't either. So.
[79:21] - Google's learning TypeScript right with us. - Yay.
[79:25] - All right. This is a part of function overloads.
[79:32] - Oh, is it? Okay.
[79:34] - Yeah. You're done with it.
[79:35] - Oh, yeah. Yeah.
[79:37] This is one thing that on this PDF version, it's kind of hard to always tell
[79:43] because you can tell, like if I can get them in the same area
[79:47] that that's like an H1 and this one's an H2 or something like that.
[79:53] But when they're not next to each other, it makes it a little hard.
[79:59] So where did we land? I had a hard time with return types and voided never.
[80:07] And then we kind of skipped the last one. - I didn't think you had that hard of a time with never.
[80:17] Or maybe we just didn't dive deep enough to explore. - No, like never is gonna make sense.
[80:21] I was just seeing like thinking of what we, from the beginning,
[80:24] what we thought I would have issues with. - Cool.
[80:28] Yay. - So, that being said,
[80:31] I do have a question for you because next is a raise. When you get a second,
[80:39] 'cause I think this would be a fun challenge, is if we went with,
[80:43] does it build upon something? Is it new or is it a recap?
[80:46] So when you get a second, could you classify them?
[80:52] - For each of the chapters or the whole chapter as a whole? - I would say the headers.
[80:56] - Yeah. Do you want me to send you that now, later?
[81:00] - Later. - When we do the stream?
[81:02] Okay. - Yeah.
[81:03] Before the stream, if possible, but later. Like you have a little, probably bigger,
[81:11] wow, you have bigger than two weeks. That is verbiage.
[81:14] That is, you know, totally made sense. You have more than two weeks
[81:18] 'cause I will be on my way to Munich this time in two weeks. I think.
[81:27] I don't, what time is it? I'll already be in Munich.
[81:31] I'll probably be going to bed. - Cool.
[81:35] I got it. What are you going to Munich for again?
[81:36] You told me this, I forget. - So I'm going to Portugal for Crab Week,
[81:43] which is like our meetup. Not meetup, our offsite for the company.
[81:49] And then I am going to Munich afterwards because my friend Anas is from there
[81:55] and I haven't seen her in forever. - Hey, that's exciting.
[82:00] - So, and if we have time and let's see. Let's see, Elion, if you're still here,
[82:11] I will, I'll show everybody, but you know, since it has to do with brutal things,
[82:22] might want to know. Oh yeah, you are still here.
[82:24] Okay. - Yeah, I'm going to be rude and plug.
[82:29] Elion had a blog post that got retweeted. We published something on dev too.
[82:33] So the practical dev should not try to find the link. - Wow.
[82:43] Okay. As soon as this loads, I'll be able to show you.
[82:46] Yo, it's not loading though. Miro, are you like seriously not going to be my friend
[83:02] right now? - Rude.
[83:04] - Rude. - Very rude.
[83:11] - I just got that that logo was like an M. Oh my God.
[83:15] - Oh, huh. It kind of looks like the monster logo.
[83:21] - Yeah, yeah, it does. - But I mean, there's only so many.
[83:25] Oh, oh, oh. - The Gen Z rebrand of monster for Silicon Valley.
[83:28] - Okay. - Eh, eh, eh.
[83:32] - Yay. Okay.
[83:38] So we have progress. I am slowly, since I am learning Postgres,
[83:46] learning like what I want to do with the website and things. And look, I have,
[83:54] I think I included all the things that are in your theme. I did built with brutal theme on Astra
[84:02] and it's using Astra, JavaScript, you know, and TypeScript. And for the backend,
[84:08] I know that I want it to go to Postgres database, which I believe I need to connect with Prisma
[84:15] because going over here, these are my handy dandy links
[84:22] that will link to all my projects. They are for Ivan.
[84:28] They are making me like a virtual business card, like page. So that'll link there.
[84:35] But the entire reason I'm asking about this is I need to figure out how to see
[84:44] if I could use like Postgres and have two different like requirements
[84:48] in for like each page. So like, if it's on a teach gen tech thing,
[84:56] each page needs to be set up that it knows it needs to have the embed,
[85:01] the episode description, guest contacts, any links, and then the transcript
[85:07] where for my podcast, it needs a little more. And that's my goal to continue learning Postgres
[85:16] and finish studying at my webpage. - That sounds great.
[85:22] - And I think it can do that. I think it can.
[85:27] I'm like, I think I can. But yeah.
[85:30] So yay. That's what I wanna show you
[85:35] is I'm building this out all on the Brutal Theme because I love the Brutal Theme.
[85:39] And I will say that when we do stream, Elian, shit, I'm messing it up again.
[85:51] Sorry. - Elian?
[85:54] - Elian. - Oh, Elian, okay.
[85:58] Elian is that seeing how to customize a few of the other pages would be cool.
[86:06] 'Cause I'm always like, I don't know how to do that part properly,
[86:09] but I'm gonna figure this all out. It's gonna be great.
[86:13] And if you guys wanna see something really fun, 'cause I shared this on my stream last night,
[86:18] this is the life cycle of how to put out a podcast episode on here.
[86:28] It's everything I do for the podcast, which is from guest information
[86:37] to how many calls we have to actually why we have it.
[86:46] And then before we can even put it all out, the video and asset creation.
[86:51] It is fun. This took a really long time,
[86:54] but I'm glad it exists 'cause now I can make it better. But I'm also trying to do that with my website stuff
[87:02] because I think it's important for people to be able to see this side
[87:06] 'cause I didn't really understand it. And as to why I need to make friends
[87:12] with someone at Vercel so I can understand the hosting side of it,
[87:17] which will happen eventually. - Cool.
[87:22] So yeah, that is what I will be up to you later next week and this week.
[87:29] And what cool things do you have going on? Like who streams or what streams are you gonna do?
[87:34] - Me or the chat or? - Both.
[87:39] I was technically asking you, but I'm gonna ask everybody now.
[87:42] - I know there's at least one person in the chat who streams.
[87:45] Yeah, I've got a busy week actually. Today was fun.
[87:48] I did a game show with people around React Miami. That was a whole thing I won.
[87:56] I won a free React Miami ticket, which I'm really excited and super appreciative
[87:59] and I don't know if that came across in the screen. I kind of feel bad,
[88:02] but I don't know who to give it to. So yeah, the next week I'm in New York City actually
[88:09] for the first two and a half days 'cause there's a Codecademy event
[88:14] and a bunch of people who used to work there are coming over to hang out
[88:18] 'cause we have a very positive, uplifting, fun, friendly culture, us alum
[88:22] and the people who are still there. And then I'm in React Miami.
[88:25] Can I actually show a website design by the way that's also the Brutal theme vibe?
[88:29] - Never. Yes, of course.
[88:32] It's my favorite thing. - So yeah, I've been wanting to do this for a while.
[88:36] I just got it approved for the Philly JS club. It's like our JavaScript meetup.
[88:40] Not to be confused with the Philly JS user group, which is different.
[88:44] But yeah, this is the theme that we're gonna go with for the Philly JS website.
[88:47] It makes me so happy. It's so silly.
[88:52] For fun, I'm gonna be implementing it in Remix, which I've never used beyond like toy demos before.
[88:59] - Nice. Please tell us how it goes.
[89:03] - Yeah, we'll do. I'm excited 'cause it's like the simplest,
[89:05] by far the simplest of the designs that we looked at. Like we had like, I came up with a bunch of different ones.
[89:11] Like this one we're holding in case everyone hates the Brutal one.
[89:14] But like I made a parody of Vercel as a design, sun rays, the whole thing.
[89:18] And this one's simple and it just brings me joy. - I do like it.
[89:24] - Yeah, we'll fly you over on December 34th. Sounds good.
[89:26] Yeah. - That's funny.
[89:31] Do you tell, I almost forgot to ask you for this week. What Twitter drama or TypeScript drama is there going on?
[89:40] Because this really is a big part of it that I always forget to ask.
[89:47] But what, I would say, how did you come up with your colors first?
[89:50] I am curious about that. 'Cause you had a few different colors going on.
[89:54] - Let me show you something. The JavaScript logo.
[89:57] - Oh, I don't think I ever knew that. - Yeah, it's not black.
[90:02] It's like very dark, dark charcoal. The JavaScript logo is in a font called Nutraface,
[90:08] which is free only for personal use. So this website is in a font
[90:12] that looks very similar to Nutraface. So it's not quite the same,
[90:17] but it's like slightly more bold and like fillet-in. It's, I don't know, that's what we call ourselves.
[90:22] Yeah. Cool.
[90:24] - Interesting. - But the real exciting thing, it's again, not drama.
[90:28] You keep asking for drama and I'm sad to say I haven't delivered, but-
[90:32] - That's okay. - The TypeScript types for React and similar
[90:36] have been slightly inaccurate for quite some time. And the reason why is there needed to be like a new feature
[90:44] in TypeScript around how you describe JSX, like the syntax using like React, solid, and so on.
[90:50] And this lovely individual, Sebastian Silberman, got a PR approved and merged
[90:56] that has been open since October. And the next version of TypeScript
[91:00] is gonna be much better for describing edge pieces of JSX types.
[91:04] So yay. - Yay.
[91:06] - People will be very happy about this. - And anybody else working on anything cool?
[91:13] But before we forget, is your website using the exact same font?
[91:18] That to me, it's to you, right? Like-
[91:21] - That is to me, yeah. - Yeah.
[91:23] - It was, and then I realized for personal use doesn't mean you can use it on your personal site.
[91:27] It's for like stuff that you keep to yourself. So I switched to, from Nutraface to League Spartan,
[91:34] which is like another very similar font. And now I'm working on that personal site.
[91:39] Eventually I'll have it working. - Okay.
[91:43] - It's in Astro. - I feel like, are you all gonna be like streaming
[91:47] with Dan this coming week? Because he had this many streams this week.
[91:52] I was like, damn. He is like a powerhouse.
[91:54] Like he is always going. - Isn't Astro like Remix, but like slower?
[92:01] That's what I thought it was, right? Just kidding, just kidding.
[92:05] Every time he asks, I say something stupider, but I love that.
[92:09] By the way, this is such good marker research. Calling, calling out positively.
[92:13] Ask what your thing is to see what people say it is. Like, that's such a good way of learning
[92:18] how people view your thing. Like I asked people what TypeScript, BSLint is,
[92:22] and they have no fucking, pardon me, no effing idea. And it's very upsetting.
[92:27] - Oh no, you can cast on here. I was like, I have a podcast called
[92:30] shit you don't want to talk about. - Oh, that's right.
[92:32] Like, I will say that since I don't understand, didn't because this was a few months ago,
[92:43] understand enough of like why choose Astro and how to talk about it compared to something else.
[92:51] I had to do like a presentation on it. It was really difficult because it's still a little bit,
[92:57] but at the time it's like, I don't know, what's the difference between that
[93:03] and like starting up something as a React website. I don't know.
[93:08] I don't know. I know there's differences.
[93:11] So yes, there is still learning there to be done. - Still learning.
[93:17] And that's the fun part of it. There's always something else to learn
[93:20] and you can always feel like you're missing out because you're always missing out.
[93:23] And that's totally good because there's infinite content out there.
[93:27] - Yes, yes. - Yay, yes.
[93:32] Send those over. So down for that.
[93:35] And yeah, well, that is all I had today. Josh, anything else that you had for us?
[93:41] - No, no. - Go buy his book.
[93:45] - Yeah, that's, thanks. Buy my book, sponsor me on GitHub.
[93:48] Sponsors are sponsored by PPS link. Like and subscribe and follow me on Twitch, I stream.
[93:53] But no, I'm just excited to see your progression. Like you're clearly like instinctively getting things
[93:59] such as the question mark stuff. That's awesome, really pleased.
[94:01] - I really like it. I think the book is really,
[94:05] I will say it's the theory stuff that I always really struggle with
[94:08] and also putting words to things that I already figured out how to do,
[94:12] but I didn't know that it actually had a word to go with it or a phrase or whatever.
[94:19] And yay, I will check out this video. And any preferences who we should read to y'all?
[94:27] Any requests before I click the raid? 'Cause we got Chris Griffin.
[94:36] We got Ryan. Yeah, I was just about to say we got Ryan.
[94:41] - Ryan is a good one. - All right, we will go to Ryan.
[94:45] Please stand by. Y'all will raid when, I don't know why it takes so long.
[94:51] It's like ready to raid in. I'm like, what do you want me to say during this time?
[94:56] It's gonna be awkward. - I so strongly relate to what you're saying.
[94:59] My first few raids, I was just like, bye. 14 or like nine seconds later, like, what do you do?
[95:05] - Yes, well now I actually get to hit raid. So, okay, bye.
[95:09] And, and. care.
[95:13] [BLANK_AUDIO] 
