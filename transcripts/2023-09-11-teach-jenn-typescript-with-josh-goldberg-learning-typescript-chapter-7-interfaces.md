---
showLink: "https://www.youtube.com/watch?v=U2szfBQjE3U"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-typescript-with-josh-goldberg-learning-typescript-chapter-7-interfaces"
title: "🎥 Teach Jenn TypeScript with Josh Goldberg; Learning TypeScript: Chapter 7 Interfaces"
publishDate: "2023-09-11"
coverImage: "https://i.ytimg.com/vi_webp/U2szfBQjE3U/maxresdefault.webp"
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

[00:00] It erred out and then it didn't erred out. Yay.
[00:03] Welcome to Teach and Tech, where we break down tech barriers to make it accessible
[00:09] and have super duper cool guests on, like Josh, who wrote a book called "Learning TypeScript"
[00:15] and does cool things. And we have a fun series about learning TypeScript.
[00:21] This is chapter seven. I'm actually,
[00:23] I like that we haven't streamed for like two months. And I'm like, you know, we're slowly,
[00:31] this might take us like two years to get through the book. - Yeah.
[00:34] I mean, we're getting through it, honestly. It's happening.
[00:37] - We are, and I love it. But hello, everyone.
[00:41] My name is Jen, host of Teach Gen Tech. And this is Josh.
[00:45] As I said, the author of "Learning TypeScript," but you also do a lot of other things.
[00:49] And what have you been up to? I haven't asked you conferences
[00:52] or what you've been doing lately. - Yeah.
[00:55] It's been a little while. I've been a little calmer at the last few months.
[00:59] I think my most recent conference was Seattle JS Conf, which was fantastic and wonderful.
[01:04] Actually going to a wedding in France, leaving tomorrow over the weekend.
[01:07] Real excited about that. - Yay.
[01:10] - Shout out, Nod and Remi. But yeah, no, I've got a busy year.
[01:14] I think you and I are sharing a conference pretty soon. TS Congress coming up later this month, right?
[01:20] - I'm actually at a conference. Well, I'm at that conference.
[01:25] Because for those who don't know, TS Congress, TypeScript Congress is a virtual conference
[01:32] and you should join. It's going to be fun.
[01:34] We're talking. And so is Daniel Rowe, which I like hardcore fangirled.
[01:40] I was like, I'm actually talking at a conference that he's, what?
[01:45] That was a mind blowing. And yes, it's also weird to think
[01:53] that I'm actually going to be at a conference that you're talking at too.
[01:56] - Oh, I'm not talking at the conference. I'm just hosting like a Q and A or two.
[02:00] - Yeah, but still, you're you. And really quick, before I forget,
[02:04] Nate, I've been meaning to reach out to you because you need to come on the show.
[02:08] And my spaciness has not reached out. So while I see your name, I need to tell you that.
[02:15] So thank you for the pause. Anthony just got married.
[02:19] - Congrats, Anthony. - Woo!
[02:24] - I'm really excited. I wish I could have made the wedding.
[02:27] Oh, it looked so beautiful. I saw photos and I'm just so excited.
[02:31] I love his new wife. Well, his fiancee, I love, now new wife.
[02:35] How would I, is that? Anyway, she's amazing.
[02:39] - Grammatically speaking, I think what you're saying. - Yes, and anything else you've been up to?
[02:45] - I've actually been working on a fun project called Create TypeScript App,
[02:52] formerly Template TypeScript Node Package. You can see why we need it to create TypeScript App.
[02:57] It's like a good getting started thing for TypeScript repos. It sets up all the linting and building and testing
[03:03] and coverage among contributors and everything that you could possibly want
[03:06] in a generic TypeScript repo. And that's, I'm taking, I learned a term yesterday,
[03:11] prep-tember. So like September preparing for Cracktoberfest.
[03:14] - Oh yes, Cracktoberfest. Yes, yes.
[03:17] I need to talk to, reach out to Brian. See if he wants to be on the show for prep-tember.
[03:25] - Yeah, yeah, that's a good idea. Yeah.
[03:29] Yeah, rolling out Create TypeScript App for all my repos. And it's got like a bunch of like repo automations
[03:38] and documentation and stuff to make it easier for people to contribute.
[03:40] So I'm pretty excited. - Yay, and what up, Roy?
[03:45] Yes, Roy, I think you'll be very excited about this news as well.
[03:50] Since something for everyone that doesn't know, I am part of the OSRG Raid Guild,
[03:59] open source Raid Guild. Yeah, there we go.
[04:01] It's where I currently hang out and it's super fun. And all my friends there are all huge TypeScript fanatics
[04:10] and also are like, Jen, you do a lot of the theory stuff. You don't actually code enough.
[04:17] I'm like, heh, heh, heh, heh, okay. So Roy has been helping me learn how to get unstuck
[04:25] on certain things and building what I want when I have the time to do it.
[04:29] And I think he will be very excited to hear that. I am gonna go through and do all of the chapter assignments
[04:39] that from Josh's book as well to learn too. - Awesome.
[04:44] - Because we haven't done the assignments, which again, because of time, but also like we should.
[04:48] And yes, Nate. - Yeah, I just had a bunch of good first issues on it.
[04:56] So I've had it. - Yay.
[05:00] Do you wanna tell us a bit more about PrepTember so that way people are prepped and ready to go contribute?
[05:08] - Yeah. I just learned the word like this week,
[05:13] but in general, Hacktoberfest is a yearly celebration of open source sponsored by some big companies
[05:20] in open source. I always forget who's doing it.
[05:23] DigitalOcean I think was the thing. Maybe, I don't know.
[05:25] Anyway, the idea is if you get a certain number of merged pull requests, so code contributions,
[05:31] or I'm sorry, not code. Contributions such as code or documentation
[05:35] to open source projects in the month of October, I think it's like five is the threshold.
[05:40] You get a free shirt or you get to plant a tree. Is the new website, this year's website up?
[05:45] - Yeah, it's presented by DigitalOcean Ilacloud? How do you?
[05:52] I don't know how to say that in AppRight. - Ilacloud.
[05:56] - I feel like I was at Cloud Next last week and they're doing cool things with AppRight,
[06:02] with Google Cloud Next. And they did some cool announcements.
[06:05] And also we followed each other on Twitter that there's a new DevRel there
[06:13] that I should make friends with and see if they wanna come talk about Hacktoberfest.
[06:17] - Cool. - We'll do.
[06:19] - I was talking to one of their DevRels. Tessa was really cool.
[06:21] Shout out. - Oh, I don't know if like, Tessa Tessa.
[06:27] That's so cool. - Shit, if I got the name wrong, that's embarrassing.
[06:31] No, it's Tessa. Anyway, yeah, no, that's really cool.
[06:34] Thanks for, I forgot to check. I didn't like, didn't even think to check.
[06:37] Like, oh yeah, hacktoberfest.com, it's September. They probably have it up.
[06:39] So yeah, it's really exciting. Anyone who's interested in like getting into open source,
[06:44] whether you've never done it before or like you've tried but like never really contributed
[06:48] to anyone else's library. There are a lot of great tools that people will talk about
[06:51] for finding like what's called a good first issue, something that's welcoming and friendly
[06:56] for someone who might not be like super experienced, which I think is really exciting.
[07:00] I like the idea of Preptember. This is a kind of a new thing
[07:05] where when they first rolled out Hacktoberfest, it was just any repo anywhere, go contribute.
[07:09] And that was chaos because not everyone was ready to receive contributors.
[07:12] So now we're prepping maintainers such as myself to make sure that our repos are ready.
[07:17] We've got dev documentation. We've got getting started guides.
[07:19] We've got good first issues, all that good stuff. - And one that I am very excited about
[07:28] that I mentioned about BDougie coming on the show. I think I'm also partial to it
[07:33] because Ben Myers helped me figure out how to commit it. But I did my first PR with OpenSauce.
[07:41] So it has a special place in my heart. - That's awesome. - And yes.
[07:48] Gotta make five PRs with the most minor doc fixes ever. One thing that to make sure to mention
[07:59] that I'm mentioning, want to remember, is you wanna get these done as soon as possible.
[08:05] Because there's a lot of shirts but not as many shirts as we may want.
[08:10] I didn't get a shirt last year, but I did get the cool hologram thing on my GitHub.
[08:16] - I think I did a tree last year. I've got too many dang shirts of these.
[08:22] - Yeah, there are. I mean, for some people, the shirts,
[08:28] I just really wanted one last year for my first year. Now that it's my second year, I'm like,
[08:33] that could be cool, that could be cool. Let's see.
[08:36] Y'all, we're gonna hopefully not share like too much of my screen today.
[08:43] Let's see it. Share, share, share.
[08:47] Hey. - Here it is.
[08:51] - This is my GitHub. And it does, you get your achievements.
[08:56] I think there's achievement here too. Oh, hey, I'm the sponsor.
[08:59] That's a quick draw. That's cool. - Thanks.
[09:03] - I'm like, I don't even know what all of these are. This is fun.
[09:06] But I was going for the app rate, this participant, and these two.
[09:13] It's from last year. Very exciting stuff.
[09:16] But I know that everybody joined to like hang out with us and hear what we're up to.
[09:23] And that is some of the fun. But we actually also have what we've been learning
[09:32] and your book. So please tell us about what your book is
[09:38] and what we've been going through on this. I feel like it's, you're a good explainer.
[09:45] I was gonna say explanation. You're a good explanation.
[09:48] - Explain-ator. Yes, learning TypeScript.
[09:51] Enhance your web development skills using TypeScript.
[09:53] It's a book that I wrote, published with O'Reilly, through, with, by.
[09:57] It takes you from, I just know JavaScript, or in Jen's case, I haven't coded in JavaScript before,
[10:03] to TypeScript. So what is TypeScript?
[10:06] Why do we like it? How does its stuff work?
[10:08] Like the type system. What is a type system?
[10:10] How does that work? And then all the most common features
[10:13] that most developers are using in TypeScript, like interfaces, arrays, tuples, functions,
[10:18] type narrowing, unions. A lot of good stuff in there.
[10:22] - Yes. And this was something that was fun on,
[10:27] that we started with, is the fact that I,
[10:34] Josh and I met when I didn't even, I'm still learning JavaScript.
[10:38] If you ask Roy, I still don't know the differences of all of them.
[10:41] It's like, I can figure stuff out. I just don't always know their names,
[10:45] which is currently what I'm working through. And I promise Roy, I will reply on,
[10:50] I was supposed to be replying on. But, we are on chapter seven, interfaces,
[10:56] which is kind of crazy that we've, almost that we've made it this far,
[11:00] but then also that it's taken us this long to get here. - Yeah.
[11:05] - I'm not sure which. - I think we're at the bell curve of information.
[11:09] We're like, we are now hitting the point where like you could get to most TypeScript co-bases
[11:14] and be generally fine. Like there are no major new things we're introducing.
[11:19] - That's fair. I see that a lot more in,
[11:22] so we have the book. I am sharing my iPad,
[11:27] in case anybody's curious how I'm doing this. And this is a big reason why,
[11:31] when I was asking about like external monitors, a lot of people were like, just use your iPad.
[11:37] I'm like, I can't, I can't use my iPad 'cause I do things on my iPad when I stream.
[11:44] So, but I do believe, (indistinct)
[11:49] There's a pointer. Okay, that was fun.
[11:54] Let's do the great. So, going through it,
[11:59] something we've done in the past is going to the summary, which I will get there.
[12:06] I did not go through all of, get through the entire chapter this time
[12:11] because I personally am working on catching up with Josh. If y'all didn't know,
[12:18] Josh does like conferences and live streams and creates cool new things
[12:23] and is always busy and somehow balanced. And I'm like,
[12:26] I did a conference last week and I had a 4 a.m. call yesterday.
[12:32] And I'm just like, I will get there. I will get there.
[12:37] It's getting better. - You got this.
[12:41] - Yes, yes. Okay, so the summary.
[12:45] We talked about using interfaces instead of type aliases to declare object types.
[12:53] That one part mostly made sense. I like the references in them.
[12:57] Various interface property types, optional re-only function and method
[13:03] also mostly made sense, at least for me. And then where I didn't get
[13:08] is apparently the second half of the chapter, which is awesome, of using index signatures
[13:14] for catch all object properties, reusing interfaces and using nested interfaces
[13:20] extends inheritance. That's just a hard sentence to say.
[13:25] And how interfaces with some same name can merge together. - Wow.
[13:32] - And hello. I was so ecstatic.
[13:37] I caught some of Parasocial's stream yesterday and I realized that Parasocial,
[13:43] I feel like you kind of stream like Theo. You make your videos as you stream, which is smart.
[13:50] I use it as a talk show, I feel like, where I'm like, I get to talk to everybody
[13:55] and it's hard to clip things. We'll get there.
[14:00] It is all learning. Outside of this, and I'm curious
[14:04] while I'm looking at the summary, what was the idea behind this chapter
[14:09] or why is this chapter so important in our building blocks? - Yeah, a couple of reasons.
[14:14] One, the least important is that every programming language has its equivalent
[14:20] of tabs versus spaces. And in TypeScript, I think the biggest one
[14:26] is types versus interfaces, using object type aliases versus interfaces.
[14:30] So now that you've read this chapter, you can engage in that discussion
[14:34] by screaming on Twitter about it. There are small differences.
[14:38] They don't really matter most of the time. The real juice in this chapter though, I think,
[14:41] is that it introduces a lot of concepts around how to declare more rich object shapes,
[14:46] whether it's with type aliases or interfaces, things like that second list item,
[14:51] optional read-only function versus method properties. So now you're not just writing code
[14:57] and then writing little shapes in the type system to describe it.
[15:01] You're getting more deep into the type system. You're really getting used to describing rich stuff in there
[15:07] and thinking of the type system as a major part of your code.
[15:10] Does that sound right to you? - Yeah, and it does make sense.
[15:16] And something that I, we're gonna scroll all the way back up to the chapter,
[15:22] beginning of the chapter, maybe, maybe. Keep going.
[15:26] Is something that I really liked about the beginning of this chapter
[15:35] is, let me, I have to find where I put it, or where it is.
[15:44] I know that I highlighted it, but the fact that it makes it faster to read as well
[15:51] when you're using interfaces instead. And I was like, that was interesting to me because,
[15:58] let me, ah, I did highlight it. It's these two points right here.
[16:04] It's speedier for the type script checker. And I was like, that's interesting to think about
[16:12] how fast it takes to go through all of that and generate. - Yeah, I will note that that's less of a concern
[16:20] this year than it was when I was writing the book. They're constantly doing perf improvements in TypeScript.
[16:25] So I had, I can't remember the last time I had to switch from type to interface for perf performance,
[16:32] but I know there are cases when that still happens. I just don't remember what they are for their edge.
[16:38] But yeah, it's really cool. And actually there's a really good talk,
[16:40] and I'll link in the chat from Alexandra Sikora on TypeScript performance that has been flowing around.
[16:48] Let's see, what was that? Oh yeah, BEJS, and that's really good.
[16:57] I don't remember if that's what Alexandra was speaking on that type of converse actually, but another chat up there.
[17:03] - Ooh, yay. And I did like this example and I highlighted it
[17:10] because that's how my brain works is making sure that there's different colors to pop out
[17:17] that you call out that the syntaxes are so similar. And like for this example of the type aliases
[17:28] versus interfaces, it's the actual like the semicolon. Wow, took a second to figure out.
[17:38] I'm like that symbol, that symbol right there, the one. And I feel like that's something that I was like,
[17:45] oh, it's not as difficult as I thought it was gonna be. And not as, I feel like it's not gonna be as many names
[17:55] as like something like the, how to say it? Like all of the things that like event streaming has,
[18:14] they have logs, they have so many names for the stupid stuff.
[18:17] - Oh yeah, the text is actually not that big. - Yeah, so I'm like, yay, there's not gonna be a million
[18:24] names about the same thing and I'm very excited about that. And cool, and did we wanna take a quick look at her talk
[18:35] or just make sure that we all go watch it later? - I would suggest to watch it later, it goes deep.
[18:42] It's really cool. - Yay, I'm excited.
[18:44] I always love to see new resources. All right, so, I'm gonna do each of these.
[18:54] Wait, Roy said they don't think that they've seen that. - Yeah, so the phrasing here, I'm actually kind of proud of
[19:12] and I'm gonna hone in on the little gecko squirrel, whatever, squirrel.
[19:17] Within the spectrum of types of developers who do prefer semicolons, myself included,
[19:23] we do put them after object type aliases because it is analogous to declaring a variable
[19:30] or declaring a thing. So it's type X equals whatever, semicolon.
[19:36] If you don't use semicolons, then you don't need a semicolon there, it's the same.
[19:40] But an interface is more of a declaration rather than a statement, which is two very nippy terms
[19:49] that are often used interchangeably, but within the language design,
[19:53] referring to the different technical terms for all these things,
[19:57] there is an actual difference between the two. Sparkle emoji.
[20:02] - I did put kind of sparkle emojis on the graphic, so. - Yay.
[20:11] - I updated our graphic. We'll figure out graphics at some point
[20:16] and the YouTube hacks, and oh my gosh, so much there. So most of, excuse my dog if you can hear her.
[20:25] We'll mute real quick. She's hard of hearing, like she can't hear anymore.
[20:38] So even if I were to like yell at her, she can't hear me. So it's more of just a, just waiting, waited out.
[20:46] And I really like that in this chapter so far, like you're referencing back to a lot of items
[20:56] that we've already talked about or where we will talk about it.
[21:00] Like this one's, as we'll see in the next chapter, there's a reference to chapter 13 coming up as well.
[21:08] And I was like, okay, cool. As I want to learn more information,
[21:11] I know where to go for it. And I really appreciate that.
[21:15] Something that, and this one I feel like is, was more of a, for myself than for everybody else
[21:25] on the highlights of the differences between interfaces and type aliases were just to remember that,
[21:33] that what we're doing for the rest of the chapter and this book is going to be based on interfaces
[21:42] in these two bullet points. More of like a point of reference for myself.
[21:48] But, oh, y'all, I'm doing a talk at TypeScript Congress and I'm going to use this quote.
[21:57] At least, at least maybe like the last sentence. TypeScript provides a set of--
[22:04] - Set of types. - Yes, you do it, you do it.
[22:07] I'll clip it. You do it.
[22:09] - I thought we were doing it in unison. - I'm not that, I don't know.
[22:12] - It's like a cult situation. - Okay, well, TypeScript provides a set of type system tools
[22:19] for interfaces to help model, help us model the wackiness.
[22:27] - That was great. Love it.
[22:32] - That is going in the talk, just as a heads up. It's going to be amazing.
[22:38] - Great. - This is, and one of the reasons I really like that
[22:44] is because with the talk, I'm talking about learning live and how learning TypeScript and learning,
[22:51] especially with having Josh on this show consistently and having the consistency has helped build more structure
[23:00] in my learning as well. And in my code, as I'm learning all of it
[23:04] because I'm learning TypeScript and JavaScript at the same time, it's fun.
[23:09] Although I don't always know the differences that something is TypeScript and not JavaScript.
[23:14] It makes it fun, it makes it fun. All right, optional properties.
[23:24] This made a lot of sense to me. Anything that, if I explain, see if I can,
[23:32] wait, what? - So there's actually a typo on the page,
[23:41] like a pretty glaring typo in this code snippet, which has been bugging me.
[23:45] The error message says that a property author is missing in type.
[23:48] Missing, I flipped it somewhere in the editing between pages and author.
[23:53] So this sample is fine. Pages is required, author is optional.
[23:57] So this sample is just wrong. - Okay, I was just going to say,
[24:01] because of the question mark, it's just saying that it's optional.
[24:05] - Yeah, so const missing book is totally fine because it has pages, which is required,
[24:10] and it doesn't have author, but that's okay 'cause author is optional.
[24:12] If you were to say const missing book equals and then an object had an author without pages,
[24:16] then you'd be in trouble because pages is required. And if you don't have pages, then it's the wrong thing.
[24:21] - Right, right. Now, if we put both, are you able to put both as optional?
[24:28] - Yeah, and this is fun. You can declare an object
[24:32] that has entirely optional properties, one of them, two of them, 20 of them,
[24:36] and then every object, everything that is not null or undefined
[24:40] is assignable to that object. Because you're just saying it's a shape
[24:44] and it can have any of these properties, but they're optional.
[24:47] So as long as you give it something that doesn't have a different type
[24:49] for one of those properties, if it's missing all of them, who cares?
[24:52] It's fine. - Okay, but this one did make a lot of sense.
[24:58] So this one, I was like, cool, yay. I didn't get super stuck on.
[25:02] Read-only made a lot of sense. I liked the fact of,
[25:10] oh, really quick, I'll go through this in a second. Parasocial asks, "Josh, what's your take on pages?"
[25:18] I'm just gonna put it on the screen instead of having to read it on this.
[25:23] - Great question. What's your take?
[25:28] - I also love the JavaScript. What's that?
[25:31] Yeah, so those two are not the same. They're commonly used similarly,
[25:34] and they work similarly, but there are subtle differences.
[25:38] The first page's question mark string is saying you may have a page's property.
[25:43] If you have that page's property, which you don't have to,
[25:47] then it must be a string. Not string or undefined.
[25:49] If the property exists, it must be a string. Which is different from saying
[25:55] you must always have a page's property, and then the value under that property
[26:00] is either string or undefined. And then, yes, that third one,
[26:04] page's question mark string or undefined, is saying you may have a page's property.
[26:07] If it exists, it may be either string or undefined. Now, TypeScript actually has a configuration option,
[26:13] which I can never remember the name. There it is, exact optional property types.
[26:18] I'll post that in the chat, which makes it a little more strict around this,
[26:23] because most of the time, who gives a crap? Like, either the property is there with a thing,
[26:27] or it's undefined. Like, why do we care about this?
[26:29] But there are some cases where people really want to be strict
[26:31] about whether the property exists. Because there is a difference
[26:34] between a property existing and having an undefined value, versus a property not existing at all on an object.
[26:41] Does that make sense and answer the question that we were going for?
[26:44] I'm also asking you, Jen, because this is your stream, and I want to make sure
[26:52] you're feeling good about all this. - It makes enough sense, but again, it's gonna be...
[27:00] One thing I love about all of these is it's something that I can go back and reference
[27:03] when that knowledge builds, because something that may go over my head
[27:08] to not force learning that one part. And cool, you answered Kevin's question as well,
[27:18] which I'm gonna put it on screen just so that if people don't have access to the chat,
[27:24] they can see this. How zone property works differently
[27:29] between the two, right? And yeah, also in the in operator.
[27:36] Yay. All right, cool.
[27:42] And so, what was I gonna go through on this one? (Jen humming)
[27:49] I'm thinking, I'm thinking, seeing what... I think with this one, it made a lot of sense,
[28:03] and I like that you called out that it doesn't have to be read only
[28:07] for the entire part of it, for the entire object. - Cool. - And I think that's--
[28:15] It's just saying anything that, any place where you told me that the type I care about
[28:20] is this page thingy, I'm not allowed to touch text. Wherever it came from, I don't know,
[28:27] but specifically here, don't modify text. - Cool.
[28:32] Anything that we need to go through separately here that you'd wanna call out?
[28:43] - I have another typo named from page-ish to messenger-ish, really annoying me.
[28:49] The editing process was crap towards the end in my mind. I just rushed through it
[28:53] and didn't get a lot of proofreading done. So that was unfortunate.
[28:56] This is what happens when you talk to an author. They just like nitpick their material aggressively.
[29:03] Yeah, honestly, most of this chapter is just expressing different ways
[29:07] you can declare different things on properties or methods of object types with interfaces or type cases.
[29:13] Like it's just a bunch of cool facts, really, for the most part.
[29:18] - And I dig that, so thank you. There was something that was part of functions and methods
[29:26] because you can provide, TypeScript provides the two ways of declaring interface members as functions
[29:40] with the method and property. This is the only thing I hate
[29:50] about going through these later on is I'm like, I had a question about it,
[29:53] but I didn't write it down, so therefore that doesn't help. - But you have a fancy highlighting situation
[30:00] to write down things. - I know, I know.
[30:04] But I was like, oh, I'll remember. No, I don't.
[30:07] - That's fine. That's fine.
[30:09] How would you briefly tell us about this? - Oh boy.
[30:14] See, Jen, this is one of the reasons why I don't recommend people learn TypeScript
[30:17] and JavaScript at the same time because this relies on a core JavaScript fundamental thing,
[30:22] which is that there's a difference, sort of, kind of, subtle differences
[30:25] between the two different ways to declare a thing, a field on an object that can be called like a function.
[30:33] One is a method declaration, which is like the class style.
[30:38] There's actually like some syntax sugar that you can use that makes this definition blurry,
[30:42] but generally the idea is you have a prototype-based instance of a class.
[30:47] The method is declared on the class, not the instance. Then separately from that, there's the property approach,
[30:52] which is a property, just like any other object property, and the value under that property
[30:56] just so happens to be a function. So if you look on the screen, it has both function types.
[31:00] Those are the two ways of declaring that syntax. The functional result is almost identical.
[31:05] It's a thing you can call by its name and it's a function, but TypeScript lets you explicitly say
[31:12] which of the two ways JavaScript allows you to declare it, that it was declared with.
[31:17] Yeah? - Yeah.
[31:23] I didn't realize I was muted. I mean, I was just shaking my head,
[31:27] but I was also like, yeah, okay. You know, come on, Josh.
[31:31] You just have to, like, nobody wants to be in my head. Just like, that would be very confusing for everyone.
[31:36] So, but sometimes I do wish that they could. And I do get the fact, and I appreciate the call out on,
[31:44] like, these are things that knowing JavaScript beforehand would help.
[31:48] There haven't, I feel like there's been a few, but not as many as I would have thought.
[31:54] - Yeah. - I think it's just enough to be annoying,
[31:57] but not enough to block you. - Yeah.
[32:01] Okay. And then this is where I, I didn't get to.
[32:07] - Oh, yeah. - Which, so what are call signatures?
[32:10] Because, okay, apparently I can't spell obvious. Obvious, obvious, obvious.
[32:19] - It looks right. - Is it, is that actually how you spell it?
[32:22] I'll be shocked. - Yeah, O-B-V-I-O-B-U-S.
[32:26] - Yeah, so what is a signature in code for functions? A signature is description of how something can be used.
[32:34] A call signature is a description of how something can be called.
[32:38] So I say that explicitly because there are actually two types of signatures
[32:43] that we refer to in this chapter. We talk about call signatures,
[32:47] and later we'll talk about index signatures. So before we get to index signatures,
[32:52] let's just talk about call signatures. A call signature describes how an object
[32:56] or a thing of value, a shape, can be called like a function. For example, interface call signature says,
[33:02] this is a shape and it can be called in this way. Pass it an input string, it gives back number.
[33:08] Functionally, that's basically the same as type function alias.
[33:12] The difference is the interface form allows you to add other properties onto it.
[33:19] Because it's really common in JavaScript for people to say, like, make a function
[33:22] and manually assign, like, dot version equals two, or whatever, like, random arbitrary properties on it.
[33:28] So TypeScript allows you to declare that an interface allows properties
[33:33] that are whatever, properties, functions, methods, whatever, and then also that the object itself
[33:37] is a function that can be called in at least one particular way.
[33:40] Does that make sense? - Yeah, yeah, and it also...
[33:50] (laughs) I'm currently stuck on,
[33:57] not on the fact of, like, what you just explained, but the fact that I'm going through
[34:03] so many names in my head for bumpy lumps, 'cause I'm like, wait, that's not it.
[34:11] But it's not Dreg, and it's not Tyler. Dude, what's your name?
[34:19] Because I'm spacing it, 'cause there's too many names. - Is it LuffySpacePrincess, is this the--
[34:23] - Alex, yes. He's on our D&D, not D&D, The Expanse,
[34:31] when we play The Expanse. But his username says one thing,
[34:34] and then he has two names in The Expanse, and then I just, like, couldn't get to their real name.
[34:38] 'Cause that's what happens when you learn their name in the game first.
[34:44] Anyway, thank you, Roy, for that, and Alex. What do you like about call signatures?
[34:51] I'm curious. But that was the whole thing to get to that question, yes.
[34:58] And is there... (laughs)
[35:05] - The perps. - That is fair, that is fair.
[35:12] Y'all, let's take a brief, yay, thank you for the follow.
[35:22] Let's take a brief break, because I think y'all will be amused by this.
[35:29] So if I take my hair down, you can see that I have purple hair.
[35:33] And I am quite a goofy human in general. And then if you take my character,
[35:42] which I will also link in here, so that way y'all can go follow Jacob,
[35:49] 'cause you should, in general. But we, I don't look like me.
[35:58] I look like a completely different person, and I'm really mean.
[36:01] - That's interesting. - It is.
[36:07] Oh, let's, this one won't work. (humming)
[36:14] Share screen, go to this one, go to this one. And that's me.
[36:23] - Oh my God, that's so different. - And I'm a meanie poo-poo head,
[36:28] who's really mean to everybody. That is me.
[36:32] - Gamora from "Avengers", but with hair vibes. The face things.
[36:38] - I'm a belter from "The Expanse", a mean belter. Well, she's not mean.
[36:45] She's just like, she's not, she's got a lot going on in life,
[36:52] is the best way to say it. She's got a lot going on.
[36:56] But yes, she is mean. She is mean.
[37:02] And it's so funny, because they'll be like, they'll be laughing about stuff,
[37:07] and I can't laugh, I have this very serious face. And I gotta like sit differently.
[37:12] Anyway, that is the, we don't need to go off on, we don't need to expand on "The Expanse".
[37:20] I'll talk about it nonstop. So let me go back to the book.
[37:23] But yes, this is why I couldn't come up with Alex's name. 'Cause yeah, too many names to go.
[37:34] But Alex, thank you, because you're a sucker for predictability.
[37:38] I think that's a good way of saying it. - It's a good value prop in general, a TypeScript.
[37:44] Call signatures and other parts, yeah. - Yeah, very true, very true.
[37:49] All right, so the next one that you were gonna talk about, which you said that you're like,
[37:55] there's two types of signatures, but now we have index signatures.
[38:02] - Yeah, a call signature describes how a thing can be called, like a function.
[38:09] Which by the way, if you ever see an error message like, it has no call signatures,
[38:12] that's because TypeScript's telling you it can't be called like a function.
[38:16] An index signature describes how you can index into it, or like look up properties dynamically.
[38:21] We've seen this very often in JavaScript code, where someone will just like put it up, make an object,
[38:27] and then like randomly assign properties to it. Like word counts, let's say,
[38:31] from the screen is a good example of that. Where I'm just putting whatever strings,
[38:35] or like whatever properties I want. Counts.apple, counts.banana, counts.cherry.
[38:40] And TypeScript is being told by us, well, let me do whatever I want, whatever keys,
[38:46] and as long as the value is a number, I'm okay with it. So that's an index signature.
[38:54] So you're just strongly typing what the keys and the values are, not what the,
[38:58] sorry, the types of the keys and the values, not what the specific keys are.
[39:01] Does that track seem reasonable? - Yeah, yeah.
[39:05] That one seems, I don't know.
[39:10] I feel like it clicks a little more, but like they both click.
[39:13] It's, yeah. - They're not big concepts.
[39:18] - No. - Regardless of whether they click or not,
[39:21] like there is not a lot of stuff to click with it. It's just, okay, this describes how you call it,
[39:25] that one describes how you index into it. The tricky thing actually comes from the latter,
[39:30] which is one of the fun little places where TypeScript is not truly type safe.
[39:34] The type system is more of a heuristic. Because let's say,
[39:38] and I'm just looking at the second example, dates by name.
[39:43] Let's say you declare an index signature and in doing so, you've said this object,
[39:48] any key is gonna give whatever, a date value. And then TypeScript is okay with you
[39:54] looking up any key on the object. 'Cause you've said any key in the universe,
[39:57] literally every possible string one could concoct in JavaScript gives me back whatever the value is.
[40:04] So that's not type safe. Much like how arrays,
[40:07] you can access things out of bounds and TypeScript's like, okay, this is fine by the default compiler options.
[40:12] This is, well, you told me it has the infinite set of strings as keys.
[40:16] So I'll just go with that. Thoughts?
[40:21] - Interesting. I think that's alluding to the mixing properties
[40:27] and index signatures too. But it also makes me wanna ask you
[40:35] why would you not do any when you start with anything TypeScript as your type?
[40:44] - You can think of JavaScript as just TypeScript with a lot of anys.
[40:48] Everything is any. And then as you onboard to TypeScript,
[40:51] you're replacing those anys with better things. So yeah, this is,
[40:57] well, this is better than an any, but maybe most of the time using the next signature
[41:02] is not what you want. Especially now that it's post whatever, 2015,
[41:07] and we have things like map and set built into JavaScript that are built for these operations
[41:11] of like getting arbitrary properties. So yeah, this is not ideal,
[41:16] but it's better than YOLO, any, let me do whatever I want.
[41:20] Thoughts? - Fair enough.
[41:23] Fair enough. All right.
[41:25] And I like that explanation. Anything else?
[41:29] Is there anything you specifically wanna cover in the mixing properties and index signatures?
[41:35] - Yeah. I found it difficult to write this part
[41:37] because it's actually not that, again, not that big of a concept,
[41:40] but I found it to be tricky personally. When you have an object like at the bottom
[41:44] between historical novels, hi, Eric. All you're saying here is two things.
[41:50] One, any key that's a string gives me back a number. And also I specifically know that I have Orinoco, the key.
[42:00] Like that must exist. So if I create an object that's missing that,
[42:04] let's say it only has OutMentor, types you could kill at me
[42:06] because although you said that any key in the universe is allowed to exist,
[42:10] you've also said that specifically that key must exist. Thoughts?
[42:16] - I like that. And also, Kitty.
[42:21] - Yeah, Jerry's hiding. He's been all over me today.
[42:25] It's been nice. - Hi, Jerry.
[42:27] Jerry, you're cute. - No.
[42:30] - Is he a full black cat? - He's got a little bit of gray up the chest.
[42:36] He and his brother. We think brother.
[42:39] We think he has ADHD because he gets very restless and very attention all over the place.
[42:45] He's really cute. - I like what Roy said of,
[42:54] they want a TypeScript book that is one page. Use any for everything.
[42:59] Thanks, Kay, bye. Just for the--
[43:02] - Yeah, you can self-publish. - But Roy, I see a future in writing for you and teaching.
[43:10] Roy's a great teacher and doesn't give me the answers. I get very stuck and then I just want to yell at him.
[43:19] Thank you, Roy. Oh, yay.
[43:26] So this part does make sense. And then, oh, we got numeric index signatures.
[43:31] - Numeric ones. - Yeah, fun fact.
[43:37] In JavaScript, so this is a JavaScript thing that TypeScript has to let us represent.
[43:43] Whenever you create an object and then ask for a dynamic property,
[43:46] like whatever the thing is, array index of some variable,
[43:49] that property can be anything and it gets coerced or turned into a string.
[43:54] I forget the technical term. There's like a fancy algorithm.
[43:57] So you can use numbers. So like this mixes numbers and strings thing
[44:02] is totally fine in JavaScript land. So now TypeScript index signatures
[44:07] can say not just I string, but also I number. That's why they have the type annotation there.
[44:11] It's not just I, 'cause it can be string or number. And number must be more specific than string
[44:16] because number keys get turned into string keys anyway, which again is a JavaScript thing, not a TypeScript thing.
[44:23] - I appreciate the clarification. Ooh.
[44:28] (cat meowing) - Did you hear that?
[44:32] - Jerry agrees. - Yes, he does.
[44:34] (cat meowing) (laughing)
[44:39] - This is the fun part about live streaming or calls or doing anything
[44:43] is you will probably have animals in the background. It is the best.
[44:49] Okay, nested interfaces, which I feel like we kind of talked about earlier
[44:58] because you could, in the read me part, because you could have things nested
[45:03] but not have the same requirements. - Yeah.
[45:09] Yeah. - Is there a big difference in this area?
[45:17] - No, just, it's the same stuff that you went over back in chapter four with objects
[45:23] where you can nest things, an object can have a property, that's another object.
[45:27] And here, in addition to being able to represent as like an object literal,
[45:30] you can ultimately call it an interface. So, yay.
[45:35] - This may be a very apparent answer, but I'm gonna ask it anyway of,
[45:44] can you nest object or interface? Like, can you switch back and forth?
[45:52] - You can mix and match, yeah. Nothing stops you. - Okay, thank you.
[45:55] - I also really like the way you asked that. A lot of people say phrases like,
[45:58] "This is a dumb question." And I really don't like that
[46:00] because I don't like encouraging the concept of questions being dumb.
[46:03] - Yes, of course. - Very few dumb questions.
[46:05] There are dumb questions, it's just very, very few of them.
[46:08] And no one who's concerned about asking a dumb question has ever actually asked a dumb question in my experience.
[46:13] So, "This might be apparent," I really like as a phrase,
[46:15] because to me, the person who wrote the book, it might be apparent,
[46:18] but to you, someone who's just reading it now, learning, it may not be so apparent.
[46:22] So, yay, plus one, I like that. - Thank you, thank you, thank you.
[46:26] I will say I learned that from someone at Cloud Next last week when I'm learning.
[46:32] I had questions about everything, and they were asking people that came up to the booth
[46:37] or getting to know them, like, "This may be apparent," or, "This may be something that I'm not seeing right now."
[46:44] I'm like, that's a great way of asking it, because it may not be apparent to everybody.
[46:51] Ooh, extensions, woo! What big, cool news do you have about adding to extensions?
[47:03] - Again, the same as what you saw before, just with a different keyword.
[47:08] - Yes! - Intersection, but differently named.
[47:12] Otherwise, it's basically the same. - So, basically, I'm hearing that this was a great week
[47:18] to have a shorter episode, even though I had it delayed a day. - Yeah, yeah, this is perfect.
[47:23] - Nice. Overridden.
[47:26] I don't know if we've talked about this. Oh, well, it does say new.
[47:30] In case anyone's curious, the stuff that I have, oops, as I hit my mic,
[47:37] this right here is notes of, is this a new concept or not? And apparently, this is new,
[47:45] so no wonder I had no idea about overridden properties. What is this?
[47:49] - Well, glad you asked. You can make things more specific
[47:58] in the derived or extending interface. For example, on the screen, we see with non-nullable name,
[48:06] which extends with nullable name. In the extended one, the one that extends, name is string.
[48:12] So, anything that's typed with non-nullable name, name is string, not string or null.
[48:17] So, we are taking in the with nullable name interface and getting a more specific, more narrow version of it,
[48:25] which seems kind of silly here because they all have the same property
[48:27] why we could just make a new interface. But if the base interface with nullable name
[48:30] had other things on it, it would still be really useful to be able to extend it,
[48:33] but then say that my name is more specific, more narrow. Does that make sense?
[48:38] Is that reasonable to you? - Yes.
[48:46] I'm going back to, because we're talking about extensions
[48:57] and this is something that I, with coding in general, of like extensions to narrow things.
[49:04] - Yes. Set theory is weird.
[49:10] Like the terminology is based on set theory. You are getting, you are extending the interface,
[49:15] so it's like a new thing. And you can add properties to make it bigger.
[49:24] You could also narrow existing properties and in that way make it smaller.
[49:29] - Mm-hmm. Yeah, yeah, yeah.
[49:35] That's why I'm like, it makes sense, but it doesn't make sense based on words
[49:41] that I've learned so far. So in general, not even,
[49:46] but what did you say this is based off of that I should go look up?
[49:50] - You don't have to set theory from like mathematics. So it's like a lot of TypeScript actually comes,
[49:57] a lot of type systems in fact, come down to set theory of like what are the set of allowed things?
[50:02] So like a union type, the concept of a union comes from set theory.
[50:06] It's two unions, you union them together. I don't introduce set theory.
[50:12] I don't think I've ever actually mentioned it in the book. I don't, because most people
[50:17] don't feel particularly comfortable diving into mathematical principles,
[50:21] but that is like a root of where a lot of this comes from. So if you do have like an affinity or prior experience
[50:27] or just an enjoyment of math, like that theory of math, it can be very useful for understanding TypeScript types.
[50:34] - We also have Laura and I haven't had Laura on the show for forever.
[50:39] It's been crazy. She is, was a math professor.
[50:44] - Oh yeah, Laura would love this stuff. - Yeah, we could just be like, yo Laura,
[50:49] you wanna come on and talk about set theory? And all right,
[50:54] Roy, think of extending the functionality of an interface versus extending the quantity of what's in the interface.
[51:06] And Alex is saying, they like to think of it as extending,
[51:11] like pulling out of the shapes, extending a part rather than making
[51:16] the original part bigger. - It's always fun seeing how people interpret
[51:23] these different things. Everyone has like a different personal thing
[51:25] that works for them. Yeah, cool stuff.
[51:28] - And I appreciate everybody sharing. 'Cause it's like, this is one thing about learning
[51:33] that if like, you might have to hear it seven times from three different people
[51:41] and four different ways for it to finally make sense. - Roy, we're all right here.
[51:50] All of us. - Different ways to make it click.
[51:53] Ooh, extending multiple interfaces is extending interfaces multiple times.
[52:03] - We've extended the extending, yes. - Okay, so that one seems pretty self-explanatory,
[52:11] but what about interface merging? - Yes, this is new.
[52:16] Hi, learner. Good to see you.
[52:18] - It's leaner. - Yeah, interface merging is the big thing,
[52:23] like the big thing that interfaces can do that object types can't, at least object types.
[52:30] Now, whether you want them to do this is separate from the question
[52:34] of whether they can do this thing. But if you declare two interfaces near each other
[52:39] in the same area, and they have the same name, it's as if you just declared one big interface
[52:44] with all the things from both of them. They merge together.
[52:49] To some people, that sounds horrifying. And in a way, it is horrifying,
[52:53] because what if you typoed? Why would it let you do that?
[52:56] That's weird. But it's actually really useful,
[52:59] because in JavaScript land, because JavaScript is weird and wacky,
[53:02] people actually do often merge together their things at an existing type.
[53:08] For example, the global window, or global this in different environments.
[53:12] People are constantly adding crap to the window, whether it's good stuff, like new polyfills for new APIs,
[53:19] or if it's bad things, like window.myCount equals zero, or whatever.
[53:23] So there's a global interface window that you can then also extend
[53:26] by saying interface window myCountNumber. - Okay.
[53:31] - And this is explicitly a thing that interfaces are used for.
[53:34] This is why many people use interfaces, even if they wouldn't prefer it normally,
[53:39] because they have to. Thoughts?
[53:43] - Currently swirling around the idea of how someone may learn that they have objects,
[53:55] even though they may want interfaces to merge, like how someone would maybe be able to identify that
[54:04] to get it to work that way, if they're newer. - Yeah.
[54:08] - So that's a good question. To get it to work that way, if they're newer.
[54:13] - This is not a common thing. If you are newer to TypeScript,
[54:19] you can probably just ignore it until it becomes necessary.
[54:22] If you are newer to JavaScript, definitely ignore it. I'd say there are very few,
[54:30] but very distinct and visible cases where this is useful. The most common one,
[54:36] the only one that I've actually got a memory of using this past year is process.env in Node,
[54:43] where in Node.js, you can set process environment variables and then run your script.
[54:47] And then the global process.env is an object with all those environment variables.
[54:50] And sometimes you want to say like, okay, I know the script will always run
[54:53] with some global process variables. So you can extend, you can merge.
[54:58] I forget the name of the interface you use for process.env. So that's like a case where the built-in types
[55:03] are not sufficient to describe the built-in global options, or in this case, the things that are declared
[55:08] in that type/memory, the type definitions for Node.js. Thoughts?
[55:15] - That does make sense. And I can see based on that example,
[55:22] why a newbie wouldn't be anywhere near that. Now, I like, Lunar just said like,
[55:30] interfaces versus types are something that they feel confused.
[55:36] And I know we've been talking about this a bit, but I'm curious if you could summarize that part.
[55:43] - Yeah, happy to. It's been a little while.
[55:45] It's been like, what, half an hour on the screen? An hour?
[55:47] Wow. Yeah, so it's at the beginning of the chapter,
[55:51] and there are like a million articles online. Yeah, there are a lot of different resources
[55:56] explaining this in slightly and sometimes maybe in different ways.
[55:59] But basically, there are very few interface versus type differences.
[56:03] They're almost the exact same. This, what's on the screen now,
[56:07] good, yes, plus one to showing this. The two are the same, basically,
[56:11] type poet versus interface poet. So for most of the time,
[56:15] not all, but most of the time, it's really just whatever you like the looks of more,
[56:19] or maybe like the underlying principles that you prefer. So don't be confused, they're the same.
[56:25] Now, there are some differences, which the chapter does mention.
[56:30] The main thing that interfaces can do that object type aliases can't
[56:35] is merge, which we were just discussing. If you have two interfaces,
[56:39] the same name and the same scope area, they just merge together.
[56:42] Object type aliases, on the other hand, can do unions, which interfaces cannot.
[56:50] Interfaces, there's no way to represent a union, like string or a number.
[56:55] That's a type alias thing. That's not an interface.
[56:58] Now, there are other subtle, small differences. Later in the book, we'll get into generics
[57:03] and fancy types, which lean much more towards type aliases, but that's later.
[57:09] It used to be the case, lastly, that object type aliases tended to be slower
[57:16] for TypeScript to compute and have worse error messages or type errors when something was mismatched.
[57:21] Nowadays, that's not really the case. I think there might be still edge cases,
[57:24] but it's really hard to find them. So for the most part, it's just,
[57:28] eh, they're the same, basically. - I like it, I like it.
[57:34] Okay. Are member naming conflicts just like if there's,
[57:42] if they can't merge, like you, or when you don't want them to merge?
[57:47] - Yeah, if they can't. If you have declared this, whatever,
[57:50] merge properties interface twice, and in one thing, you said that different
[57:55] takes in a string, and the other one, you said different takes in a number.
[58:01] Well, what is TypeScript supposed to do with this information?
[58:05] It's blatantly contradictory. So it gives you a type error saying,
[58:07] hey, if you declare two properties in the same named interface,
[58:11] if you want to merge them, they have to have the same type.
[58:13] Otherwise, I don't know what to do with this. - Got it.
[58:17] - It's like me telling you, my favorite color is blue, and then two minutes later saying,
[58:22] my favorite color is red. I have lied to you at least once, maybe twice.
[58:29] - Or you're a Gemini, and your truth changes. - My truth changes, true.
[58:34] TypeScript is definitely that. What zodiac sign does TypeScript do?
[58:38] (laughs) - Has someone done that yet?
[58:42] Like, what zodiac sign each language would be? That would be great.
[58:47] That would be a great TikTok. - Now you can phrase it that way, probably.
[58:51] - What zodiac sign does TypeScript do? - Now that we've gone through interface merging,
[58:57] we can finally understand the last bit of the chapter. Why are interfaces good drivers, Jen?
[59:03] - They're great at merging. - There you go.
[59:07] (Jen laughs) - Which I feel like a lot of drivers aren't,
[59:12] so that is a good thing. - God, I've been driving in New Jersey lately.
[59:15] These people are awful. TypeScript could be associated with the zodiac sign Virgo.
[59:20] Virgos are known for their attention to detail, precision, and practicality.
[59:23] - Oh. - Solid.
[59:27] (both laughing) - I need to figure out what language is Gemini
[59:34] because that's probably the one I'd get along with best. 'Cause our truth changes.
[59:40] Like, it's not like we're ever lying to people. Our truth changes.
[59:44] - I love it. - Because like, it could be like,
[59:47] I am so convinced that this elephant is my favorite elephant of all time,
[59:55] and this is the best elephant. But then five minutes later, these elephants appear.
[60:01] - Ooh. - And therefore, this is my favorite elephant of all time.
[60:07] And then I'll forget about this elephant and see this elephant, and therefore it changes again.
[60:11] It's really annoying. - I love it.
[60:15] - And that does remind me, I don't think we've talked since I went to AWS Summit,
[60:22] New York, and I survived New York. - Oh yeah, New York.
[60:26] How did that go? - It was good.
[60:30] Alex came to come hang out at the meetup, and thank you. Next time to give Alex more of a heads up
[60:35] so he doesn't just have to go. You came from Connecticut.
[60:40] I said goodbye to a couch. - What?
[60:48] - Oh, I did say goodbye to a couch. I did do that.
[60:51] Yes, I did do that. Did I freeze or did he freeze?
[60:56] Who froze? I do remember that now.
[61:04] Oh, he froze. Okay.
[61:09] Oh, his Mac is randomly restarting, so we'll just remove him from screen
[61:15] so he's not stuck in that frozen spot. Yay, I'm glad it was fun.
[61:21] And yeah, Aaron, I forgot that I, I was so tired and did not want to move
[61:29] that I said goodbye to a couch. And it was pretty great.
[61:39] It was really pretty great. Oh, I'm just replying to Josh in all caps.
[61:45] It's cool. Okay.
[61:51] Learner, you can do the virtual conferences, but one day I bet you'll go to in-person conferences.
[61:56] Someday. Someday.
[61:59] But yes, New York was fun. I wanted to tell Josh about it 'cause I survived.
[62:04] I took public transport into the city and then I took an Uber back to the airport.
[62:14] It was like a two hour ride. It took forever to fly to JFK, to get to JFK to fly.
[62:23] And yeah, well, while you're all here and we'll see if Josh can rejoin,
[62:29] make sure that you hit follow, subscribe if you like, and you know, keep hanging out.
[62:36] And also there is the, there's the thing. There is the link to open source.
[62:47] Open source Raid Guild, which is where you can come find out
[62:52] and hang out with the community, which I will link. If you want to know what's going on with Teach Gen Tech,
[63:01] come join here. There's it's own little bubble.
[63:04] And hello again. - Hi, sorry.
[63:09] I switched my assistant desk to sit from stand and I forgot the little outlet at the bottom was loose
[63:15] and it keeps jostling it out. So turned off my Mac.
[63:18] Sorry, how was New York? Did we already pass that point in conversation?
[63:22] - You just missed the fact that I said goodbye to a couch. Like I realized my shoes were too small.
[63:34] Like if you walk around a little bit in shoes, you may not realize that they're too small.
[63:41] Like they're like, they probably fit really well. But if you walk around a ton, your feet swell.
[63:47] And I did not know that I hadn't bought anything for all these trips.
[63:53] And my feet were in so much pain and so many blisters that I had to say goodbye to the couch that I was on
[64:02] because I was so sad I was leaving it because that meant more walking.
[64:06] So Aaron reminded me of that. - Yeah.
[64:14] - The subways were good. From JFK, I took the subway to my hotel in Times Square.
[64:23] And then I said, no more about this shenanigans. And I took a lift back to the airport when I had to leave.
[64:34] Aaron and Alex came to the open source data infrastructure meetup,
[64:41] which Aaron's gonna talk on at one of them sometime soon, someday, or the Boston one.
[64:47] I need to plan the Boston one too. And I need a plan when I'll be back in New York.
[64:52] And I survived. - Good.
[65:00] - New York was the first one. So New York was the hardest one.
[65:06] Chicago was worse for other reasons. And then I just got back from San Francisco,
[65:16] which went really well. And I'm like, so there's progression
[65:21] of preparedness on these trips. And I have Denver in two weeks
[65:26] and then San Jose the week after that, so. - Hell yeah, that's a good amount of tripping.
[65:33] - Yes, yes. And I find out soon if I'm going to a conference
[65:38] in Portugal later this year, that's a big conference. And I'm hoping I am.
[65:44] I don't know yet. - Good luck.
[65:48] Oh, shout out in the chat, Aaron, Strangeloops is a great conference.
[65:50] I don't think I'm going this year, but I really like going there.
[65:53] I think I was there last year. I met a few cool people, saw some awesome talks.
[65:57] They're really nice. Great time.
[66:00] - And y'all go follow. We'll also follow, well, we'll do Aaron
[66:05] and then I gotta wait for a little bit. Aaron, when are you streaming?
[66:09] Okay. This is a big reason in case anybody's curious,
[66:17] Josh also streams on Tuesdays and this is why I moved my stream earlier on Tuesdays.
[66:22] But yesterday just wasn't gonna happen. I was so struggling.
[66:28] I wake up at four and start work at five. I can handle that.
[66:32] That is routine. That is something I do.
[66:35] Waking up at three to be to work till at four, it screwed up my entire day.
[66:42] I struggled so bad with it. So thank you.
[66:46] Thank you. Okay. Yes.
[66:48] Go follow Aaron so we can watch her stream and also go follow Josh because they're fun.
[66:57] - Yay. - I have to do the @ symbol.
[67:01] Your streams are fun. They're very, like, it's easy to ask you questions.
[67:07] - Thanks. - Oh, I have to wait another minute
[67:11] before I can shout you out. Yay.
[67:18] Lerner, that's a big reason though. Like I was like, I might as well do it earlier
[67:22] 'cause then other people can join and Lerner, you're regular.
[67:26] You count. So I'm glad.
[67:31] And then Aaron and I had a big discussion on when she should stream
[67:34] because no matter what, when you make friends with streamers,
[67:38] you're gonna overlap with somebody. There's no way to not overlap.
[67:43] - We have a weirdly small community, programmers, streamer people in our space.
[67:48] - We do, we do. But yes, it is a fun crowd
[67:54] and you can always learn something. Aaron and anybody else that wants to get
[68:00] into live learning or streaming, I will share my talk because it will have,
[68:07] if you were to start doing this tomorrow, slide. Oh, I almost shouted out Aaron again
[68:14] just because she just replied and that's not what I'm trying to do.
[68:19] Aaron, I already shouted you out. For me, there we go.
[68:23] It finally worked. But yes.
[68:27] Yay. Awesome.
[68:34] Well, all right. So on that note,
[68:39] is there anything that I'm missing, Josh? - I'm scrolling back to the contents.
[68:49] Also finding people on Twitter. I don't think so.
[68:54] I think interfaces and classes are like the chill middle part of the book.
[68:58] Like you've absorbed a lot of information. - I was gonna say classes.
[69:01] Classes is the next one and I'm so not excited for classes.
[69:06] - I mean, I would just skip it, honestly, for you because you would have to learn JavaScript classes.
[69:12] And I think that that is the JavaScript feature that is most like not intuitive in TypeScript.
[69:19] - Well, we could do our own separate... Maybe I'll try to have somebody come on
[69:23] and see if they can help me figure out what classes are and actually understand them.
[69:29] - Yeah. The nice thing about TypeScript and classes
[69:36] is that TypeScript adds very few things to them. There are like a couple of like weird things it adds
[69:41] that people don't often use. But there are very few things.
[69:44] It's mostly about just like type declarations, like declaring what the type of the classes should be,
[69:48] as you would expect, based on literally everything else in the book.
[69:51] It's just around types. - Yeah.
[69:54] - The bad thing about attaching classes is that it's classes and that's a controversial topic in TypeScript.
[69:58] Some people love them and use them for everything. Some people hate them and avoid them like the plague.
[70:02] I'm personally like closer to the avoid, but I don't avoid it like the plague.
[70:06] I just like only use it when it's really useful. - Who do we know that loves classes?
[70:12] I need to find them and I will make a tweet later and please retweet and tag people that you think love classes
[70:19] and would like to teach about them because I want to punch them in the face.
[70:25] And you did say that we could skip this chapter, but I feel like it's one of those things
[70:30] that I'm gonna have to learn it at some point, even though.
[70:37] - Unclear. I would say, I would prefer to skip it,
[70:41] but like I understand if you want to go through, that makes sense.
[70:45] Angular in particular, out of the like the big common frameworks
[70:49] is like a big class proponent and like has a lot of good reasons
[70:53] going for using classes. So if you know anyone in like the Angular-y areas
[70:57] or like the, I think Vue has like class in Texas. That's like, that's still a thing people do.
[71:02] I haven't. - I mean, we had Mishko on the show,
[71:08] but that was when he was doing more quick things. So it could be kind of weird to be like,
[71:13] "Hey, do you want to come back on the show and teach about classes since you made Angular?"
[71:19] - Yeah, that might be overkill for that, but I could do.
[71:24] - See if he says yes, just to see. I don't know.
[71:28] That could be kind of funny. But also at the same time,
[71:32] I'm like probably should save that one for something more technical down the road.
[71:36] 'Cause he was my fifth stream ever and having to explain things
[71:43] without even knowing what Hacker News was was probably painful enough.
[71:47] - It's good practice for him, though. I think anyone who's super like big experience, et cetera,
[71:52] should regularly, if possible, if they have time, do things with people who, say,
[71:57] don't yet know what Hacker News is. Like it's really, really useful for us to stay grounded.
[72:02] Us being like people who've been around in the industry for a while have like written a book
[72:05] or made a framework or whatever. - That's cool.
[72:08] No, I'm glad. I'm glad.
[72:10] It's definitely fun to have to have others on.
[72:15] So, all right. Well, on that note,
[72:20] I am going to rate us. It looks like, let's see.
[72:30] Finite Singularity. I think, you know, I've hung out with them before.
[72:37] I've seen some of their streams or somebody on one of their streams.
[72:40] So, let's go say hi to them. - Let's do it.
[72:44] - And thank you everyone for joining today. And we will see you next week.
[72:51] Okay, I'll see you. Josh, we'll be rating Josh on Tuesdays is the goal.
[72:56] So, it'll be like a double feature. - Okay.
[73:03] - All right, see y'all next week. (audience laughing)
[73:09] [BLANK_AUDIO] 
