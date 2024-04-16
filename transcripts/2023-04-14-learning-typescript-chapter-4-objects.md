---
showLink: "https://www.youtube.com/watch?v=5m-VKKjzNJk"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-4-objects"
title: "Learning TypeScript Chapter 4: Objects"
publishDate: "2023-04-14"
coverImage: "https://i.ytimg.com/vi_webp/5m-VKKjzNJk/maxresdefault.webp"
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

[00:00] to another episode of Teach and Tech, Learning TypeScript with Josh. Yay! Josh came to the save earlier this week while I was streaming, learning how to
[00:13] create, download Docker. Download Docker? Use Docker with Postgres and PgAdmin. And the first 30 minutes of it, I had no audio until Josh showed up and was like, "Yo, dude. I can't
[00:32] hear you. Oh, shit. Well, that would be helpful." So, yay, Josh! And for those who don't know, we'll see if I can remember it, Josh is the -- is a TypeScript maintainer. Is it official
[00:49] TypeScript or is it the linter that you're a maintainer? My job title is, well, nonexistent and very confusing because I work -- I'm one of the people who works on TypeScript ESLint,
[01:01] which is neither TypeScript nor ESLint. It is a tooling that lets you run ESLint and also prettier on TypeScript code. But I do contribute to TypeScript once in a while.
[01:11] Okay. Okay. Because I was always like, I don't know exactly, but I end up explaining that I'm like, yeah, Josh wrote a book about TypeScript and maintains something about TypeScript and
[01:26] is a TypeScript guru. That is my explanation of you. Thanks. Yeah. I like TypeScript. It's good. It's very fun.
[01:36] Yes. And so, I will share my screen really quick because this is what the book looks like. Yay! Everybody should go get the book. It's amazing. I have thoroughly enjoyed learning and
[01:51] there's funny and punny things in here that make it all worth reading. And also, it's definitely builds upon itself, which I'm seeing, of course, we're on chapter four. It's taken us a while to
[02:04] get here, but we are. We are moving. And I'm doing this for those who are curious. I am streaming from my iPad so everyone can see what I'm working on as well. But also, if I go to chapter four,
[02:21] I bookmarked it. Y'all can see my notes. I'm also still learning my iPad. It doesn't really get any bigger than this unless I zoom in on the iPad itself. So, if you want to see my notes,
[02:39] I can zoom. But before we get there, Josh, we are on chapter four, objects. Yes. What went into building this and what's your
[02:53] overall like why is this chapter four and what do you think is the most important pieces of this? Quizzing you before we go look at the summary. >> Objects are really important in JavaScript.
[03:07] One of the really important things in JavaScript for everyone is writing all sorts of objects all over the place. And because people do all sorts of wild and wacky things, which I'm learning
[03:19] these days is one of my favorite phrases, with their objects, TypeScript has to be able to represent them super flexibly. But when you get down to it, in JavaScript, an object or an object
[03:28] literal, curly brackets, what's stuff inside, is a set of key and value pairs. That's what it is. So, in the type system, TypeScript lets you describe what those key and value pairs are
[03:39] going to be. Each of which might have their own type. You can have an object with key is the string ABC, the value is number typed. And then this object stuff just keeps going
[03:50] into different ways of representing different key value pair types. So, an object in like short, so object, is a key and a value.
[04:02] And it's in the curly brackets or regular brackets? >> I call them curly brackets or curly boys or squiggly bracket boys or squiggly wigglies. >> You sound like you were on Jason's stream
[04:18] because he always calls them like curly bracket or curly boys. I think he has a shirt about it. That is my representation of it. That's probably not great. Please don't judge. My drawing.
[04:30] Okay. So, me being the super noob, for everyone who is curious, I am figuring stuff out as I go. Like, I'm like, I want to do this project. Let's go learn it. Which has its struggles. Or
[04:50] is really awesome because then you live stream with like 10 other people that all know what they're doing. And you're the super noob who's sharing your screen asking questions about CSS.
[04:59] You know, that does happen too. >> That was a great stream, though. >> I had so much fun because I was not paying attention to like anything else anyone was saying.
[05:10] And I was so grateful because Jacob was like running the stream. And then I was just focusing on my code. But I could ask questions when I got stuck. It was phenomenal. For anyone who is
[05:23] curious, I would highly, highly suggest if you're ever wanting to learn stuff, make friends and just live stream it. It's a lot of fun. Okay. So, the reason I went into that is so I'm trying to
[05:40] think of how to explain this. Of a value I'm going to go back a couple pages because I tried writing this out. A value is different than a variable. But whatever, no. No. This isn't I was thinking
[06:05] I was putting pieces together and I wasn't. Which is a little sad. So, I'll just ask it instead of me trying to what's a key and what's a value. So, that way I stop trying to guess and look
[06:21] really awkward. >> So, in JavaScript, every object is a set of key and value pairs. Could you go earlier in the page? I wonder if
[06:31] I have an example here. Okay. No. Next page, then, if you don't mind. Trying to get an example. >> Yeah, for sure. >> All right. Here we go.
[06:38] Top of the page, poet equals. Then, poet equals an object with two key value pairs. Born is a key. 1935 is a value. The value's type is number. So, then, TypeScript would understand
[06:51] that poet variable to be type object that contains a born number and a name string. Is that what you're looking for? >> Let me see if it is. And I'm going to
[07:05] so, this defines variable. Variable. Sure. That's how it's going to be spelled right now. And then, okay. This is an object. And then, we're going to change colors because we've got
[07:35] too much going on here. Let's do purple. Sure. And then, I feel like so, this wow. That didn't work very well. Is a key. And this one's a key, too. But it wouldn't be the value is
[08:04] 1935 or the value is a number. >> Yeah, run time in the run time area of understanding. Yeah. Poet.born is the number 1935. But in the type system, TypeScript
[08:19] would consider it to be type number. So, you can later do like poet.born equals 123. That would be allowed because poet.born is considered to be type number. Kind of like how a let variable. If you
[08:32] said let born equals 1935, that's type number. You can assign it a different number. Keep in mind, in JavaScript, a const variable can't be reassigned. But you can do whatever the heck
[08:43] you want to its properties. So, you can do like poet.born equals negative one. Even though poet is const. >>
[08:49] And I hear what you're saying. I'm trying to think of how to like conceptualize this. So, I remember going back to it. >> Sure.
[09:01] >> So, would you say the key can be a type number, type string, whatever, and then the value is what is ever declared in the key? Because then like 1935 can always change.
[09:23] But in this example, it's 1935. >> Yeah. The key stays the same. The value can change if you want. >> Okay. Okay. I just see this.
[09:34] Can change. And these are the values. And the keys create like example. Poet.it would be poet.born, right? And that would be a number. Or would it be poet.
[10:06] Yeah. It's an example. Perfect. This is what I want. And I'm going to point to it. Yay. >> Yay. >> Yay. Cool. See, this is why I really,
[10:18] really wanted to get Catabolist. Because I'm like what you're saying makes sense, but it doesn't always make sense in my head. Because I need arrows.
[10:29] >> Sure. The arrows are key. >> Yes. So, I'm going to go back a page on so, we're talking about object types now. And I know at least on and thank you for letting me
[10:47] ask you questions and being aware of my Astro projects. Because that does help put it to reference. In at least my first Astro project, it was all of the type declarations were in another
[11:03] file. Are they always in another file or are they normally within the same file? >> By default, people normally put them in the same file. But if you have types that are used
[11:12] in multiple files and aren't strongly associated with one particular component or thing, then, yeah, it's not unheard of. It's not uncommon to put them in a dedicated types file.
[11:23] It's kind of like when you declare constants. If it's only used in one place, yeah, just keep it in that one file. But if you use it in a few different places, maybe put it in a shared,
[11:39] you know, separate file. >> Yeah, we'll go back and write that one. Cool. Yay. That totally made sense. Now,
[11:51] if we skip a little further, which guys we're going to, y'all, we're just going to scroll. Because it's like the fastest way to get to the summary. >> Real far. >> Yay. All right.
[12:05] >> Oh, right. Yep, yep, yep. >> We talked about this a little bit. And I kind of like going through the summary first. Because then I'm like, okay, I know what I'm
[12:17] going to be learning and what to look out for. Which that works for some people for learning. Other people are like, no, dude, I got to go from the beginning. So, I think this was really helpful
[12:30] of how TypeScript interprets types from objects type literals. Describing object literal types, including nested and optional properties. Which nested totally made sense to me. And then
[12:44] optional didn't. And I was like, why? Why? It's frustrating for me. Declaring, inferring, and type narrowing with unions of object literal types. And >> Discriminating unions and discriminants.
[13:04] What a concept. Going to have to read the chapter to get that one. >> And combining object types together with intersection types. So, a lot of this,
[13:17] and I really like that you always reference, oh, I got a pointer, guys. We got pointers. >> Pointer boys. >> That you always put where we'll
[13:29] cover it more. Or you link back to where it was previously covered. That being said, I don't think anybody wants to go through that again of me scrolling a ton. So, what's that one?
[13:46] Yeah. All right. Go into section two. Declaring object types. Some of these notes may be in here because I'm just working on remembering what we previously were talking about. So,
[14:04] if we are declaring object types, which this might make it easier for everybody to see. A little easier? I feel like it lets us show text and that. So, we're declaring object types. So,
[14:19] I was like, I need to remember what the types are. Which is null, undefined, Boolean, string, number, big int, and symbol. >> Those are the primitive types.
[14:32] Not the object types. The two terms are different. >> See? This is why we're fact checking myself. >> Cool. Everything you said is right, except if you cross out object and write primitive,
[14:45] then it will be completely right. >> Sweet. Yay. And okay. Okay. Because they're primitive types because an object type, an object needs to have a key and a value.
[15:09] Right? >> Yep. Basically, everything in JavaScript is either a primitive or an instance of a class,
[15:22] which we haven't gotten into yet, or a function, or an object. Basically, everything. >> Okay. So, these.
[15:41] >> Okay. Cool. Yay. That totally makes more sense. And what we were talking about further on. Yo, it's Ryan. Hello, Ryan. I love that Ryan always does that. Ryan is the best at
[16:15] posting stuff. I love talking to people, but live streaming and managing the chat and stuff, I'm always like, okay, hold on. Let me do this. I just realized something, though, y'all. Let's see
[16:32] if I can just do the window to make it easier for all of us to see. Hey! There we go. >> Awesome. Also, just got a really good backstretch. >> Nice. Nice. That is always
[16:48] important. So, okay. Declaring objects. What would you say is a short summary of declaring objects? >> You can create a new object in JavaScript. And so, actually, sorry. I misinterpreted. When
[17:06] we say declaring object types, it's similar to how you might say that a variable will eventually be or only ever be, like, a string or a number or something. Here, we're saying it will only ever
[17:17] be an object with these particular keys and values in it. So, on this example that you're showing on the screen, poet later, we're saying poet later the variable will only ever be assigned
[17:28] an object that has born, number, name, string. Technically, I should have said it's only ever going to be assigned a value that has those things, but that's semantics.
[17:40] >> So, I think this is a part that leads to my question later on of, like, error type string is not assignable to this. Because, like, what this alone makes sense
[18:00] when we go to when you're adding extras, that's where I'm, like, wait a second. So, cool. Aliased object types. This one made sense. And especially because we talked about aliases
[18:20] earlier. What I was curious about was you answered this one already. Yay. So, we don't need to go through that one. So, just because we were talking about, like, const let and those
[18:40] types of things, if let wasn't added here, could you just do poet equals instead of poet later equals? Right? >> Like the poet from earlier?
[18:55] >> Well, no. It says type poet. And that's the object. And then you say let poet let poet later be poet. And then you use let poet. But do you need to have let poet later declared for to use
[19:16] poet as a or could I say? >> You don't. You could say, like, let poet colon capital B poet equals the type. They all work the same as with primitive or
[19:31] literal types or type unions. You can slap that type in a place even if it doesn't seem necessary. >> Cool. Okay. >> Yeah.
[19:39] >> And this I was, like, okay, cool. This totally made sense. And this was another way of showing that you couldn't just put, like, with the error of just Emily Dickinson because it's missing
[19:56] information. >> Yeah. Like, in theory, Emily Dickinson, the string, has some properties on it. It has, like, length and, you know, two string and stuff.
[20:09] But it does not have born and it does not have name. So it doesn't work. >> And that one made total sense to me. Anything else you would want us to know about aliased
[20:22] objects types? >> Aliases are used for all sorts of things. But the concept of an alias itself is actually really small as a concept.
[20:31] It's just whatever I say this word, I actually mean whatever's to the rights of the equal sign. So whenever I say poet, I actually mean object that has born and name. That's all.
[20:41] >> Okay. Okay. And then structural typing made sense to me. Oh. Let me see if I can find this. I like that I made myself a note of it. Because this one talks about duck typing. And I remember
[21:05] on, like, our last string, I had to ask, like, it was the first time I heard of what duck typing was. And I was, like, what is this? And one night I came up with funny titles. And I was, like,
[21:23] so let me write this really quick. Y'all can laugh at it. It's totally okay. But I don't know if it applies. But, yeah.
[21:35] [ Reading from slide ] Okay. There we go. I didn't have my phone with me to put it earlier. But types of ducks,
[22:10] how having data types help your ducking code. >> I like it. >> I want to do a talk on that someday. Inspired by our stream. So, thanks.
[22:22] >> Let's do it. >> I was, like, is that a little too silly? Or does it actually work? >> I like it.
[22:30] >> What? >> The only problem is that you put it at the, it's a little longer of a title and the funny part's at the end. I'm wondering if there's a
[22:38] way to move the ducking code, like, the joke to earlier in the title to emphasize it more. Were you worried that I was about to criticize it?
[22:44] >> No. I didn't know. Like, I was, like, I'm pretty sure these pieces of it make sense. But I was, like, wait. If duck code is without types and is just, like, going with the flow,
[23:02] does adding data types actually help? Because then it's no longer duck typing. So, I was more, like, overanalyzing that part of things.
[23:14] Then word structure and stuff like that. But we could say let's change the color. Purple. Sure. Help your ducking code. >> This reminds me of one of the
[23:36] greatest Simpsons gags of all time. Ever seen the picture of Sneeds Feed and Seed? >> No. >> Formerly owned by Chuck.
[23:45] >> Oh, my gosh. >> It's a joke. Anyway. >> I don't think I've ever
[23:52] actually watched a full episode of The Simpsons. >> It used to be a lot better. >> I haven't seen a lot of TV. It's kind of sad, kind of boring, but that's okay. So,
[24:05] what do you think of this one, though? Help your ducking code with data types. >> I like it. Yeah. Good. >> I'll work on it. I'll work on it.
[24:12] >> Work on it. >> I was just excited that it's a concept. I woke up in the middle of the night and all these, like, title ideas came to mind.
[24:23] >> Yes. >> And I'm, like, why does it have to come to me at, like, 1 a.m.? Why can't it come to me during the day when I'm awake?
[24:30] So, it was one of those. That's why I'm, like, no hard feelings if it doesn't make sense. >> Do you keep, like, a whiteboard or pen and paper by your bed or anything like that?
[24:39] >> I send them to myself in a message. >> Nice. I found that super useful, like, having a message or paper or whatever. >> Yeah. Yes, that is true, Ryan. That is so true.
[24:54] Ryan said it's because you're more relaxed, i.e. shower thoughts. That is why so many people remember things or have ideas. I actually, since I started using the tablet, I started going to
[25:09] sleep with it next to me. So, I can just put this in a notebook and actually start having them together. >> Nice. Yeah, plus one of the driving. I've written, like, verbally dictated written a
[25:21] lot of blog posts in the car. >> That's a good call. That's a good reminder because if we are moving back to Phoenix in July, it'll be a 14-hour drive. So, you know,
[25:37] I'll just, like, be really productive and write things. >> I'm expecting you to have your own TypeScript book by the end of that drive. >> Yes. Yes. Like, TypeScript for people who
[25:47] don't know JavaScript. Okay. So, usage checking. This one also completely made sense to me. I was just like, oh, it's just checking that, like, yeah, that one was easy. What would you say is
[26:08] the summary of that one? >> I'm glad it made sense to you because I have to look back at what I'm doing right here. But it makes sense for you. Yeah,
[26:18] yeah. You tell me. >> Okay. The way I understood it is usage checking is when basically it's like, hey, we had first name, last name. You entered the first name,
[26:32] but, hey, last name's not here. So, it's still wrong because last name's not here. >> Yeah. Exactly. Yeah. >> If you wrote last name. So, you used an
[26:43] example earlier of how you can use somebody's, like, you can put the poet's information as a string. But if you don't put names and their name in the string there, it's not going to know it
[27:02] because it's not reading it correctly. So, but excess property type, there is a what for a reason. Because I was like, the other one made sense. Totally made sense. Stuff is missing.
[27:21] But going to excess property type, if I go to the next page, I was like, I was looking at the error and I'm like, I'm not it's not clicking. >> Sure. So, TypeScript tells you when
[27:43] the thing you did, the value, does not match what you previously said it should be. You declare a variable and you say it's going to be a particular type that has two things. And the initial value
[27:55] for the variable has three things. Wow. So, the complaint there, the second indentation level of two says an object may only specify known properties. If you say it's going to be a
[28:07] particular type, you can only specify properties mentioned in that type. And activity does not exist on type poet. So, TypeScript is telling you, hey, you said it's going to be this thing,
[28:17] but it's actually more than that thing. You added excess things you weren't saying you're going to. >> Okay. So, y'all, I know this is on two pages. So, bear with me for going back and forth.
[28:28] But oh, actually. >> Does it not have like a side by side? >> It doesn't, but it does have this kind of creepy thing that I can do.
[28:38] >> Creepy is my middle name. >> Paste image. This is what we have from the other page. Okay. I guess that'll work. Okay. Let me like zoom this in since it's a little
[28:58] smaller. So, we have and I think this does help, at least for me, being able to see them on the same page. So, we said the type is poet and that object includes born and name. And then we have
[29:19] the const poet match is poet. That's an alias. And so, the keys are born in name. Values are the year and name. And that's all that's in our object. That's it. Voila. We're done. But if we say,
[29:36] well, hey, our poet is walking, has an activity going on, it's not going to work because it's never assigned. Okay. That really makes more sense. Thank you.
[29:51] >> Cool. Yay. >> Yeah. I think it was just that it was on different pages. >> I know. That's one of the real
[29:57] drawbacks of books like traditional page oriented books. I wish it could be like I wish the PDF view of it was like the O'Reilly online platform or you could do it as one long thing.
[30:10] >> Do it like a seamless view like this. >> So, get the little page breaks, right? >> Yeah. So, like this one, I'm just like if I didn't have this here, it still doesn't
[30:26] entirely make sense. But they are closer together. So, it's something. It is something. Which I guess I'll just keep it here. >> Sure.
[30:38] >> So, nested types totally made sense to me. I'm trying to scroll down. So, it's like you have an object within an object. Right? >> Yeah.
[30:50] >> So, if we look at these ones are still I'm going to put Twitter. And then so, this is
[31:08] object. Wow. Object. I can spell, guys. No, no, no. There we go. Object 1 is poem. And then oh, sorry. I don't know if you guys heard that but I just made a beep a lot on me because
[31:31] my elbow hit it. And then author is object 2. Right? >> Yeah. Objects in an object. >> Cool. That one made sense to me.
[31:46] And it's still going to have the same issues if you don't have them lining up properly and enter the right information. So, gravy. This one is good. We don't need to go through that one. But
[32:03] optional properties. So, just to make sure that I understand, it's basically saying that earlier we talked about if stuff is missing, then we're going to get an error. But sometimes you
[32:19] don't always need a name and a date. Sometimes you just need a date because you don't know or you need the name because you have no idea when they were alive.
[32:29] >> Or it's a blind date and you just need to know when to meet them. >> Yeah, exactly. Exactly. So, all of that being said, just to break it down for myself
[32:39] on this last one. Okay. We're going back to the other view. Let's go. There we go. >> Stretched a second. >> Yeah. So, typewriters is string
[32:50] with a line and then undefined. And editor is question mark with a string. So, is this saying it could be either one of those or I need to do the line. I'm just going to rewrite it now in not
[33:06] pink. So, I would have to do the line, which is or, and then undefined. >> I'm not sure what you meant in the question. Can you rephrase, please?
[33:20] >> Does this mean the same as this? >> It does not. Author colon versus editor question mark colon. The question mark says this property does not have to exist.
[33:37] When there's no question mark, the property must exist. Even if its value is undefined. Because there's a difference between the property not existing and the property existing but having
[33:47] the value undefined. >> Okay. Okay. And I think it's so they would have to type undefined. It couldn't stay blank.
[34:15] >> Yeah. If they so this is most commonly done when well, actually, it's not super common. A lot of the time people will put the question mark. It's easier to type. Why would you want this? Let's
[34:28] say you have a function that returns string or undefined or something. Or you have a variable that's only sometimes given a string. You might want to explicitly have that value in the object
[34:39] even though it might be undefined. You might do author colon mark. This might be my author, maybe. The variable, maybe. I don't know if that helped or just made things more complicated.
[34:52] But what you said was right. >> No, it helped. >> Okay. That totally makes sense now. And then we get to unions. And I kind of struggled with
[35:13] unions in the last chapter. Not my favorite. But could you go over, like, what you were planning with, like, unions of object types and inferred object type unions and kind of go into
[35:32] that process behind that? >> It's all based on the concept of unions. So, we should get you and make sure you're solid on unions in general before we
[35:43] overcomplicate it with objects. So, can you describe what you think of unions as for me? >> I'm trying to remember. I think that's a big reason that I keep writing. Like,
[35:59] earlier I wrote what the values or what the on the other page, I wrote the seven that were there. >> Sure. The types? >> Yeah, the types. There we go. Thank you.
[36:12] The types because I'm like I feel like I'm going to forget what types are. I think union is the same way where I'm like I'm not used to the word. So, I'm not used to the definition. Because I
[36:23] still associate it with English language instead of coding. So, if I were to do this and I want to show everybody instead of just, like, asking you for the answer. Because, I mean, don't get me
[36:39] wrong. It is really easy just to ask everybody for the answer. But then I'm not going to be great at Googling things. Okay. Well, Siri wanted to answer but didn't understand. So, this is back
[36:57] in chapter three. Unions are expanding a values allowed type to be one or more possible types. Okay. So, this is when we said
[37:10] mathematician is a variable but it could be undefined or Mark Goldberg but it would have to be Mark Goldberg the exact string or it just could be
[37:27] undefined or a string. >> You tell me. It's a let variable. Is it string or undefined or Mark Goldberg or undefined? >> Mark Goldberg is undefined. Wait.
[37:37] >> A let variable is allowed to be reassigned. So, this is going to be string because it would be annoying to not let people assign any other strings to a let variable.
[37:55] So, it would be string or undefined, the union type. You look unhappy with this. >> No. It's just one of those things that are, like, going to take longer to, like, sink in.
[38:08] It's repetition, not what you're saying. >> Sure. >> So, that is, I think, one of the hardest parts of learning is it doesn't always
[38:25] whatever. Yes, we want to do this all. Because when it's referred to in another area, it's kind of hard to remember to go back and where to go back to.
[38:43] So, I appreciate you asking me. Do I know what it is? Because then I'm, like, that is a solid question. I don't know. I don't know if I remember what it is. I was going to say union as in it
[38:58] puts two and two things together. So, kind of. Okay. Let's paste this right here. Paste image. I can hang out over here. So, I at least know where I got it from.
[39:15] All right. That is making more sense, then. Because inferred object type unions is just saying instead of it being, like, a mathematician can be undefined or a string, it just means that
[39:33] there's two different type of objects that it could be. Right? >> Yep. It's either the one with pages or the one with rhymes. Exactly.
[39:40] >> Okay. So, or okay. Yeah, yeah, yeah. But would it still have to both have three in them? >> It does not. Note the type that's in the comment there. Both of those two options
[39:54] have an optional that was poor choice of words. Both of those two potential types, the technically constituents, but the two potential type objects, they both have named
[40:04] string and they both have pages and rhymes. But in each of them, one of those latter two are optional. Yep. So, in the first one, it says if you have a rhymes property,
[40:13] it's undefined. Like, it's not there. But you do have pages and names. That question mark is very key. >>
[40:25] But that being said, I could do one that is just to make sure I'm following along of, like, one type is name string and just has the one. And then another one could be name
[40:49] and rhymes as both required. So, they both don't have to have two keys to be a union. >> Yeah. Like, if you had removed pages from the first one, yeah.
[41:03] >> Yeah. This might make more sense. Give me a second. Oh, the back buttons. Oh, the back buttons. So, I just wanted copy. Paste. And this one to be copy. Paste.
[41:28] >> You're having a great time, I can tell. >> It makes so much more sense finally
[41:56] being able to, like, be, like, okay, cool. Like, I kind of get what you're saying. But I don't. So, can I, like, at least write it out? Which helps when I don't necessarily want to write it out in
[42:09] code. Because then I'm more worried about, like, the errors there. I just want to get the, like, understanding. Like, could I do this? Because they're all required. But the first one has
[42:22] one key and the second one has two keys. >> You could totally do that. >> Okay. >> I will note. So, first of all,
[42:31] yes. You're absolutely right. I'm not trying to correct any understanding because I think yours is perfect and good and great. I will note, though, something interesting. Because I think
[42:39] it's cool. The specific type you just wrote where they both have a name and only one of them has a pages could be represented as an object. It would be equivalent to, say, an object that has,
[42:50] oh, hello, that has a name, colon, string, and pages as an optional number. That's equivalent to basically the same thing. >> Oh, yeah, yeah, yeah. Okay.
[43:00] >> And the fact that you just said, oh, yeah, yeah, yeah, is great. Because you understand why that's the case. And that makes me happy. >> Yeah. So, I could have just done the question
[43:07] mark for pages. But if I did name, rhymes, and I just couldn't think of anything. Don't need to have the same number of keys. I actually understand what keys are. What up, Alien? Hello,
[43:26] hello. I do need to work on my website soon. I really should hit you up. We could do a stream for that. Just like hanging out, making fun of me, work on my site. And FYI, it was really fun,
[43:39] though, when we did it on Friday. Because I learned a lot. And Alien, I did try to tell everyone that I could have broken everything. That it's not because I got it from the theme. It's I could
[43:52] have done it myself. Because I copy/paste and try to make things work. So, okay. Yay. Oh. So, basically, what I was just trying to ask you is explicit.
[44:11] Object types. >> Yeah. What you wanted was the next thing. And that's just a prettier way of thinking about it. Rather than inferring
[44:24] something with these weird question mark undefined things. If that's your data structure, it's nice to represent it in the type system. And we're actually getting all excited. Excuse me.
[44:36] We're starting to think in TypeScript land. Before, TypeScript was letting us annotate all the stuff that's supposed to happen. But here, you are in this snippet describing in the type
[44:47] system how your code is thinking about things. The way your data is structured. And then you're just writing values that adhere to that format. I think it's a really pretty thing. And as you
[44:58] go through the book, you'll get to more and more of these, like, the data is based on the types, not the other way around kind of moments. >> Aww. Yay.
[45:08] Maybe I'm too excited for most people here. But I think it's really cool. >> No. It is really cool. Because I'm starting to enjoy learning about it more. Because
[45:22] it's starting to put these pieces together. Where at the very beginning, and it is frustrating. Because you asked me about unions. And I was like, dude, I don't know. I don't know. And a
[45:33] lot of it has to do with the fact that if somebody is going to ask me what's an explicit object type, I'm going to be like, dude, I don't even remember what unions are. Because the names don't associate.
[45:47] But if I were to go try to do this, oh, yeah. Okay. Yeah, yeah, yeah. This is I know I can make this work. I'm just not going to remember the name of it. Which is annoying. But it's also needed.
[45:59] You need to remember the name so you can know what to Google. >> Yeah. The Googling is key. Or as the kids now do it, chat GPT or whatever.
[46:08] >> Not going to lie. I did do that for if we moved to Phoenix, we got to find somewhere for my father-in-law to transfer his assisted living. And I was like, I don't even know how do you do
[46:19] that out of state. No idea. And chat GPT came up with my list. I was very excited about this. Okay. Narrowing is doing oh, I know it. I'm going to go read it again because I put it up here.
[46:38] Reducing a values allowed type to not be one of the more possible types. But isn't is this would narrowing object types only be in an if and? Because if an object says, yo,
[46:57] I don't know, let's say that it has the key of name and that is the only thing in the object, it doesn't need to be narrowed anymore, right? Or is it just because these are if else's?
[47:16] >> Is narrowing only for if else's? >> Yeah, trying to think of how to answer that right. It is not only for if else's. There are lots of cases in code where you end up using
[47:30] narrowing. Sometimes just surprising cases. Other places I think have already come up in the book are ternary statements like question mark colon. While loops and for loops can perform narrowing.
[47:44] But it's easiest to most common to say if statements and easiest to think of small code snippets that use them. Let's say that a variable is something or undefined and you say
[47:56] while that variable inside the while loop, the variable will be narrowed to anything that's truthy. >> Okay. Okay.
[48:04] I think I need to just practice more with narrowing types to understand them better. So that one, I will give you that. You told us that we would have to read the chapter to get
[48:19] to discriminated unions. So I feel like I should just like skip over this. >> Well, wait, wait, wait. It is my favorite thing in TypeScript. And you have personally
[48:31] hurt me. Just kidding. >> Whatever. I just didn't get to it. I'm sorry. I'm like, in reality, we could pause here and I will go through it. And then we can
[48:42] come back to it. >> Honestly, one could do an entire stream on discriminating unions and discrimination in TypeScript. And before anyone gets their ears
[48:52] perked up on the words I just said, it comes from the mathematical concept of separating things, discriminating on values. And it is not an HR nightmare. Which is a caveat I have to give
[49:05] always because the word discrimination has multiple meanings and only one of them is commonly used. >> Okay. So we're going to say separating.
[49:13] I like that. That makes a lot more sense even just looking at it. >> You were thinking, oh, no. What is happening? >> I was like, what are we discriminating against?
[49:28] Like what are we saying we're going to be mean to or something? >> It's those React developers. We're all on solid now. Am I right in the chat?
[49:36] >> Oh, that does bring up the great point that we were going to ask about. What is the latest drama on TypeScript? This is my favorite question to ask because I don't -- 99%
[49:50] of the time I do not realize anything is going on unless I hear about it from Dan. Which on Dan's stream we wrote a letter to an author. In a very kind way about some feedback Dan received from his
[50:06] thread. And then like from you or Jacob and Roy afterwards. That is how I find out about the drama. >> Yeah. I actually don't think there's very much TypeScript drama. They are making a TypeScript
[50:20] documentary. Fun fact. Same people who made the React documentary, I think. >> Oh. I didn't even know there was a React documentary. >> I haven't watched it, actually. I've
[50:29] been meaning to. Seem like a couple snippets. Actually, don't quote me on that. There might be two popular documentary teams happening. Yeah, I don't know. I don't know of any recent drama
[50:39] since the last stream. Which is kind of good. Yeah. Right. Dan actually asked an interesting question while we were chatting about this before the stream. Do TypeScript wizards like Pocock and
[50:50] me -- just going to subtly put myself on the same level as Matt Pocock. Do we compete with each other? Is there competition? I have never felt that is the case. Maybe technically we do. One
[51:03] could choose amongst our different offerings to learn TypeScript. But like it's not a competitive area. We're very friendly and supportive of each other. >> Okay. That's good. >> I was actually
[51:16] asking if you could help me with an analogy. The analogy I thought of was like local coffee shops or kombucha things or breweries in a very hipster, gentrified neighborhood. Have you thought of a
[51:27] better analogy than that to describe this loving area? >> I would -- I think this came to mind because of your code examples of authors. Authors like normally don't compete in having the better
[51:47] thing. Because they normally don't write the same stuff. Or it would be copywriting. Where they may compete in I must be the best version of myself because then I'll get more sales in my book.
[52:03] Like it needs to be like I need to level up. But it doesn't mean that I'm tearing anybody else down. >> Yeah. Exactly. Agreed. Like I have so many TypeScript books on my shelf. I've got
[52:16] this one. I've got programming TypeScript. A reference I'd recommend in mind. A rising title. We love each other. It's great. We're too small of an area to have infighting, I think.
[52:31] >> Yeah. Yeah. Well, okay. I'm glad we got, you know, whatever the drama was out. That's always fun. And so, discriminating unions. Is typed objects in JavaScript and TypeScript is you have
[52:53] a property on the object indicate what shape the object is. Oh, I don't think we've talked at least okay. You might have. I do need to clarify this. You might. I don't remember going over what a
[53:10] shape is. What shape it is. I don't remember this. You might have gone over it. It doesn't mean that it's stuff. >> I did go over it briefly,
[53:18] but not deeply. If you search for the word shape, it should only come up with a few matches. And the first like the first or third or something like that. One of the first few will be
[53:28] the description of like what is a type? It's an object shape. >> I don't know how to do that yet. I know I can. I just don't know how yet. >> Command F by default. Yes.
[53:38] >> Okay. And I was looking for shape? >> Yes. What an interesting search interface. I just used like the normal PDF viewer, like the default one.
[53:50] >> Oh, yeah. It searches all of it. >> Can you not just search units? >> It searches all of them. But it only found shape in the one I have highlighted.
[54:02] >> What? >> I don't know if that's accurate. >> Okay. Oh, it's a section in chapter 2 of the type system, page 24, type shapes.
[54:14] >> I wonder why it only took that one, then. That's good to know. Oh, see, it's searching all pages right here. Oh, it says 44 results. I don't know why it -- you saw the other page
[54:27] said only one. This says there's 44. >> I'm guessing it meant only one book or PDF. >> Okay. Maybe. Okay. >> That's a guess.
[54:36] >> That does make more sense. Okay. So you said that it was -- I don't think I can zoom in on these. That's annoying. Chapter 2. >> Yeah. Type shapes is the section. If
[54:54] you go to the table of contents, actually, it should be clickable links in the PDF. >> Oh, really? >> Yeah.
[54:59] >> That's fantastic. Okay. That means I need to -- oh, it is -- right. Let's bookmark these. And type system. Type shape. >> Also, if you open a PDF in Chrome,
[55:13] on the left side, there's, like, the mini menu. And then you can also view -- actually, wait. Yeah. On your right side, there are those three symbols above where it says all pages underneath
[55:24] the plus, top right. You're on the left of the three. What happens if you go to the middle of them? >> What do you mean?
[55:31] >> You see where it says all pages in the top right of your application? There's that bookmarky thing on top of it? Is that bookmarks? Oh, man. Because in Chrome, there's a view that shows you
[55:42] the table of contents from the headings. And you can, like, expand into subchapters and stuff. >> No. But you just gave me the idea that I do want to do this to the table of contents.
[55:53] >> Yeah. >> But your table of contents is not clickable. >> Well, it seems like a you problem.
[56:01] I'm clicking it just fine. >> Like, you do have other ones that are clickable. I'm trying to -- like, not even, like, these ones. But let's see.
[56:11] >> Well, anyway. >> I don't know. >> All of this to describe that -- when I say object shape, what I mean is the stuff that is
[56:21] known to exist on a type or value. So, like, a string is known to have length, two uppercase, two lowercase, and so on. >> That's chapter 1. Let's scroll to
[56:34] chapter 2. Okay. Say one more time what you thought it meant. Because I was highlighting. >> Sure. Yeah. I spoke at an inopportune moment. >> I was not listening the best I could have.
[56:50] >> Sure. When we say object shape, what we mean is the list of stuff that is known to exist on an object or on a value, rather. For example, strings are known to have a bunch of stuff like
[57:03] length, two uppercase, two lowercase, slice, and so on. >> Oh. Look, I found it. So, a type is a description of what a shape -- okay.
[57:16] Yay. >> The reason why I don't just say object shapes is because the concept of a type shape also applies to primitives,
[57:26] like the strings having length and so on. >> Okay. Which properties and methods exist on a value and what is built in the type of operator
[57:44] would be described as. Okay. Well, back to chapter 4. And so, that means that when we're talking about discrimination, shape scrolling, that it's --
[58:08] >> Can I propose, rather than have you read through the long -- because it is kind of verbose text, can I share a screen of mine and go through the playgrounds?
[58:18] >> Please. Yes. 100%. >> We end up doing this, like, on average, once a stream. >> I like when you do this because it's, like,
[58:28] it can make sense, but then I still struggle with it. So, this gives it more of a way of understanding it without, I guess, also being put on the spot. Because I'm like, you want me to type
[58:41] this too? That's scary. >> I'm going to be wet. Because it really is, like, very difficult to type or write and learn, right? Let's say we have type fruit equals name
[58:55] string. And then maybe some of our fruits are juicy or can be measured in terms of juiciness. And maybe some of them can be measured in terms of roundness. So, let's say we have, like,
[59:11] wet fruit equals 50% chance of being apple. Or banana. You know what? I don't like apple and banana and juicy round. Let's call it brown. Or what are some properties? I need one that only
[59:37] applies to apples and one that only applies to bananas. >> Red, yellow. Color. >> Interesting.
[59:48] You're making it a little more difficult for yourself. I love this. Let's do it. Color. >> Yay. I'm so excited. >> All right. So, let's say the
[59:57] apple color is another random. You know what? Let's do fruit. I'm going to separate it out just to make it a little more readable. So, in this case, it's an apple. Fruit equals
[60:14] color math.random. Red or yellow. Then name apple. Otherwise, in this case, it's a banana. Else, fruit equals name banana. And because we told TypeScript previously that it's a fruit,
[60:39] TypeScript is yelling at us because we don't have color. So, let's say color yellow. Yeah. So, that's cool. We, however, could get a little more specific in our types.
[60:53] What if we wanted to say that it's either an apple or banana? >> Oh. >> By the way, this is not yet
[61:03] discriminating. Sorry. Discriminating types. This is just normal things. What if -- you know what? I'm going to make it a little easier. What if curved is an applicable property only for
[61:15] bananas? Because apples don't care about whether they're curved. But bananas, let's say there's like a 50/50 chance it's a banana that's curved. 50/50 chance it's
[61:28] not curved. So, now we have this weird object type where it describes a fruit that's either an apple or banana and it has a property that we only care about if it's a banana. In theory,
[61:38] someone could put in like curved true for an apple and that makes no sense. >> Right. >> The fact that this makes
[61:44] no sense but is allowed by TypeScript makes sense to you. Cool. So, what I actually want to do is have my own types. Apple, color, string, name, apple. And I want banana. Name, banana, curved.
[62:00] And then, you know what? For now, let's just say color string, but later on we can do some funny stuff because bananas are only ever going to be yellow. I guess yellow-brown. Anyway, here,
[62:12] instead of having our own separate fruit type, we would say let type fruit equals -- instead of having a fruit object type, we'll say fruit is apple or banana because the fruit is either an
[62:24] apple or banana. So, if the name on the fruit is apple, then we know that curved makes no sense because curved doesn't exist on the apple type. So, I'm going to put the errors here so you can
[62:37] see the squigglies complaint at the same time as the code. Come on. >> Okay. >> So, this name property is what's called a discriminant. If name is apple, then TypeScript
[62:54] is able to deduce, oh, it must be the apple type. Otherwise, if name is banana, TypeScript is able to deduce, oh, it must be the banana type. Does that make sense? >> Yes.
[63:07] I'm also looking at this then. Okay. So, with discriminated unions, then is it easier to describe with the if/else or is it only if/elses? >> An if/else is the easiest way to describe
[63:34] narrowing. I'm just using it as a toy example to force narrowing to happen. But this example we have here doesn't actually need an if/else. I could just comment it all out and say fruit equals
[63:45] this. And it's just, oh, I see you have name apple. So, curved true. No, don't do that. >> Okay. I'm looking at this example, too, to see if I can
[64:00] it makes sense. I'm just, like, trying to think of how to write it down for future making sense, but it's okay. You know, worst case, I'll have to come back to it.
[64:14] >> This is a two-parter, and I'm waiting to do the second part until I get confirmation from you. >> Okay. Okay. I'm ready. I'm ready. >> Awesome. So, let's say that we are
[64:24] doing the randomization logic, and we don't mess it up. We don't put curved true. So, I wish I could show both at the same time. What I'm going to do is I'm going to have two tabs open
[64:36] with the types of playgrounds. Here we go. And on the left, you'll see the type definition, but it's the same code area. And on the right, you'll see stuff after declaring the fruit.
[64:54] So, just know that, like, this is the same code. >> Yeah. >> Using the fruit, a discriminated union value that is a type of whatever. Doesn't matter.
[65:13] Anyway, so, here we can check if fruit dot by the way, look at this. Fruit dot. Color and name. TypeScript knows it doesn't necessarily have curve because it might not be a banana. It might be
[65:23] apple. And it knows that the name discriminant is only ever apple or banana. But it knows it's either apple or banana. It is the union type, apple or banana. I don't know if you can physically
[65:36] see on the screen. So, I'm going to do fun fact on the type of playground. You can do these little called two slash queries. It just adds a little indicator of what the type is. So, fruit dot name
[65:49] is the union apple banana. If fruit dot name equals apple, then fruit dot well, fruit doesn't have a curved. But if you do fruit dot name is banana, then fruit dot curved does exist.
[66:08] The curved property can only exist if the banana sorry, if the name is banana. We have narrowed our object type using its discriminant property.
[66:24] >> Because we said it was banana, therefore, it can have an additional property. >> Yes. And just to show like what if we could add like crispy Boolean to apple. And then in
[66:39] the else statement here, let's say we do like fruit dot crispy. And I have to add it in this code because it doesn't sync. >> What up, Firefix-y?
[66:49] Hello, hello. Firefix was one of the humans helping me on my Docker situation earlier this week. That's what I'm going to call it, Docker situation. We're working on TypeScript. I
[67:10] am learning Josh wrote a book called Learning TypeScript and has been coming on every other week. And we go through a chapter, which Josh is also very patient because he knows that I don't
[67:22] know that much about JavaScript, which I feel like I know I'm learning a lot more. I just don't always put the words with what we're actually talking about. I'm like, oh, yeah, I do know that.
[67:33] Oh, that's the word that goes with it. So. And we're talking about discriminated unions, which is like separating out like, hey, this thing may not go with this thing.
[67:54] So, you have the look of someone who is still processing. And this is a topic that tends to take a little while to process. So, my proposal is I will copy and paste the Playground URL that
[68:06] I'm using in the chat. Crispy fruit. Because this shares the code. Let me just yeah, there we go. I'll paste it in the chat. And if any of y'all want to mess around with it, you can. But it's
[68:25] totally reasonable. And I think a lot of people, myself included, just need to sleep on this, on the discriminated union stuff. Yeah. And the link's too long, so I can't share it. Oh, well.
[68:38] Try can you tweet it to me? And then I can just like, well, I don't know. I'll look at it later. I'm going to go to my screen really quick, since we're looking at the notes.
[68:52] Because I think the part like, what you're saying makes sense. And I don't know why I only did that. What I'm struggling with working on putting into my own words is basically, if I'm going with this
[69:16] poem with pages, it knows that there needs to be the type pages. And this one knows that it needs to have the type rhymes. So, if it doesn't have that in there, it won't know that it's poem
[69:31] with pages or poem with rhymes. Unless we add it in later on. Yeah. All it knows is in the circled area is that anything that's a poem is one of those two types. So, it's going to have a name.
[69:47] It might have a pages or rhymes. And it has a type that's either pages or rhymes. And if pages sorry, if the type is pages, then it has pages. If the type is rhymes, then it has
[69:57] rhymes. >> You know what? Something that I don't think I realize, it may be something in the code that is used often but is throwing me off
[70:15] are these. Because in my mind, it would have been something like a comma and then the next one. Or like a it could have been like an or type of thing. But we have the colon and the question
[70:32] mark which just means does that mean the question mark means this one isn't included? Or it's a possibility of both? Or either? >> See, this is a very core fundamental
[70:44] thing that would be good for me to have gone over. This is a ternary. And whenever I do a math dot random in the code, in the snippets of code, that's I'm just using it to say that it's some
[70:55] random chance of using one or the other. Doesn't matter. And this is a ternary saying it's a 50% chance of the first thing, the one after the question mark. And a 50% chance of the second
[71:04] thing after the colon. That's all. >> I don't know what color to put this in. And what did you say this was called again? >> Ternary. I'll put it in the chat.
[71:21] And I'm finding the or conditional operator. So it's three things. It's the only operator in JavaScript that has three parts instead of two.
[71:35] It's some condition, the thing to do if it's true, the thing to do if it's false. Okay. Cool. That helps. Because I think that was also a thing that I was getting stuck on,
[71:54] of just like, okay, cool. But the rest of it makes sense. Now, if I were to go type it myself, this is something I do feel like I would still be struggling with. But for the most part, it really
[72:06] does incoming it makes sense. So I'm glad about that. Intersection types. I would think just based on context means that it could have that type in both of them. >> Sorry, can you say that
[72:29] again? >> So if I go back up here, like, it could have pages and rhymes in both. So we don't know which one it would be. That's context. Not what it actually is. >> Okay. Yeah. And now you're
[72:47] looking at intersection types, which have combinations of things, yeah? >> Okay. Okay. >> Okay. >> This makes sense. I'm just going to type in something weird. There we go.
[73:12] Combinations. And danger of intersection types. Anything you want to go through here that's super important that we should know? >> Yeah. TypeScript is super powerful. You can
[73:29] do a lot of stuff in the type system. Probably don't. It is difficult to debug things when they're very complicated in general, not specific to TypeScript. And a lot of people end up getting
[73:41] all hyper about what they can do in TypeScript and overcomplicating things. So try to keep your types simple just as you would in any area of code. Try to keep things simple so it's easier
[73:52] for you to read, understand, and modify over time. Yeah. Keep it simple, stupid. K-I-S-S. >> Okay. And then -- oh. Intersection types are easy to misuse. I can see that.
[74:20] Okay. >> By the way, I'm just going to clap myself on the back here because we're at the end. The never type is actually an important type in TypeScript, but it's not important until you get
[74:30] to the more fancy stuff. And I wanted to introduce never, but I didn't want to wait until the very end to introduce it because there was no one good place to put it. So putting it here actually really
[74:42] saved my butt in the layout of the book. The structure and ordering of things. I just remember being really pleased about realizing, oh, it's perfect. It's natural. You know how when some
[74:52] stuff just clicks when you're coding, you're like, oh, my God, that's how it has to be. Yeah. >> We'll just put yay. >> Yay.
[74:59] >> And I just -- I don't know if y'all can see this, but whenever I plug in my tablet, it still shows the wrong time at the very top. So I was thinking at the top upper corner that
[75:15] it's just been like chilling there. And no. No. A lot of time is fast. And I have the webinar I wanted to go to in like seven minutes. So I'm glad you're paying attention to time. Because I was
[75:27] like, how is the time not moved? >> Well, we're going to the container store at 3 o'clock, so you bet your butt I'm out of here by then. Love the container store.
[75:37] And yeah. What up, fuzzy? Okay. We have gone through a lot. And it's always -- >> I feel like we've hit our flow. We're good. >> Yeah. We finally figured it out. Took us a few
[75:54] times. But yeah. We got it all done. And we started a little late. I had to eat food, y'all. I was starving. Is it British summertime yet? Is it really? >> I'm looking it up.
[76:10] Oh, the time zone. >> Oh. >> During the British summertime, civil in the UK advanced one hour forward of GMT.
[76:21] >> I thought it was standard time, not summertime. But summertime makes way more sense. >> I thought it was BTS. >> Oh.
[76:31] Yay. I'm glad you saw the one with Dan. I reposted it on Twitter, and then I realized it was yesterday, not next Thursday.
[76:45] >> No. We're going to do another one. In the next one, we might actually do the types of compiler stuff that we were advertising we would do. But thank you. That was a fun stream.
[76:55] >> Yay. I adore Dan. He's so fun. He's so funny. I told him, I was like, I want to be on the stream. He's like, what do you want to talk about? I'm like, I don't know. I just want to be on your
[77:06] stream. >> Yeah. >> So that was my -- well, thank you again, Josh. And thank you, everyone, for joining us.
[77:15] We will be back in two weeks on chapter -- oh, my gosh. We're going in a new section. We're going in part two. >> Yeah. You've established
[77:26] the foundations. You're good to go. You could leave and be totally fine. >> No, we should probably go through functions, not going to lie.
[77:32] >> Functions are good. >> Because learning functions in Python was kind of a struggle. They make more sense, but I'll take it. I'll take it. And yes. So,
[77:48] well, thank you, everyone, and see you later. Bye. [BLANK_AUDIO]

