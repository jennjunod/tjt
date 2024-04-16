---
showLink: "https://www.youtube.com/watch?v=EEe8N2jbnsc"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-1-from-javascript-to-typescript"
title: "Learning TypeScript Chapter 1: From JavaScript to TypeScript"
publishDate: "2022-11-11"
coverImage: "https://i.ytimg.com/vi/EEe8N2jbnsc/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome to the official, official,
[00:06] official start of learning TypeScript. See if I can put it in the frame.
[00:12] Yay. We have Josh, who's the author of this lovely book,
[00:17] going through this with us every other Friday-ish. >> Very exciting.
[00:26] >> We also have resources for those who are joining along with us. We, helps if I copy and paste it already,
[00:38] have the website and also my favorite part that I just found, but is also in my new favorite part of,
[00:50] it's very organized. I think that's why I like it so much.
[00:54] Now I'm like, oh, this makes sense. I will be adding this in as well.
[01:04] But before we get started, even though I got really excited about both of those.
[01:10] Who are you, Josh? What's TypeScript? >> Who am I? What am I doing here?
[01:16] What is love? Hi, I'm Josh. >> Follow me in love.
[01:19] >> Yes. Love is when you really like something. Speaking of which, I really like TypeScript.
[01:26] TypeScript is a cool language. It is a superset of JavaScript.
[01:29] It adds types, meaning the ability for you to say what your code is supposed to do or look like and then it will let you know if you mess it
[01:36] up and gives a lot of really nice developer tooling. I have done a lot in the TypeScript ecosystem.
[01:44] I've given talks, I wrote the Learn TypeScript book. Sometimes I contribute to TypeScript itself once in a while.
[01:49] But most notably and mostly, I work on TypeScript VS Lint,
[01:52] the tooling that lets you run VS Lint or prettier on TypeScript. Although you may not have used or heard of these things,
[01:59] if you're an enterprise, if you're a company that uses TypeScript,
[02:02] you almost certainly use something that I work on. >> Yay.
[02:05] >> Let me know how I can help. >> For those who may be super noobs,
[02:11] which I say that with a lot of love because I still consider myself a super noob, and yet we're all learning together.
[02:23] I feel like a few things to break down is VS Code is a code editor or an IDE, which I'm like, what's an IDE?
[02:35] Now I'm trying to think what an IDE is. >> I can say it, but let me know.
[02:41] >> I'm Googling it, so you can say it. >> Sure. Integrated Developer Environments,
[02:46] I believe. Let me know if I'm wrong. >> You are 100 percent right.
[02:50] So an IDE, the way I think about it is, it basically lets you see what you're working on.
[02:58] So you can run it locally before it goes out to the world. That is probably the best breakdown for some of what we're talking today.
[03:11] If you're wondering what the subscript or more about JavaScript, I do have videos on that.
[03:17] Hit me up, let me know and I can give you those. Today, we are starting through the book and working our way through it.
[03:26] So I will share my handy-dandy screen. I don't know why, but ever since I started this stream,
[03:34] it makes me think of Blue's Clues. >> The handy-dandy reading chair.
[03:40] I was just thinking that. Used to watch that when I was a kid.
[03:44] That's a great show, classic. >> Like mail song.
[03:48] [inaudible] Anyway, these are the things that I bring up and also have talked about in D&D.
[03:57] So I'm just a millennial nerd. So for those joining us,
[04:02] we've got TypeScript, learning TypeScript in the website itself.
[04:06] If you're wanting to go through this yourself for a book we'll be posting the resources there to buy the book,
[04:14] as well as your digital copy. I personally really like the digital copy
[04:18] because I can have the computer read out loud to me. But then also, I can show you guys things.
[04:25] It makes it a lot easier because I don't think, I don't know. You can tell me Josh, do you think people can read it if I just go like this?
[04:33] >> I think they can and I think they won't. >> Yeah, so we like the digital version.
[04:41] The way we're going to be doing this is going through the digital version of it together and
[04:50] not reading word for word because that would be really annoying. But we are going to be talking about it overall,
[04:57] what they mean, a faster pace of it. So that way you have an auditory version of it with the book itself and
[05:04] maybe have watching live or asking questions. You know where you can ask these questions if you're watching the video on
[05:14] demand or live with us, so let's get started. And this book is broken down into four sections.
[05:28] I'm scrolling down because I don't remember the last section. >> I honestly also keep forgetting, which is embarrassing.
[05:34] But yeah, four sections or parts and a total of what, 15 chapters, I think. >> Yes, yes.
[05:41] Okay, we're doing good. So we're going to go backwards because this is where I am in the table of contents.
[05:47] So after, and we may not go all the way to part four. Just as a heads up, y'all, this is a series.
[05:55] We are going through the majority of the book. Maybe not extra credit, though.
[06:00] Because those are more of experiences for us as individuals to go through and research, but we got to get the understanding up until that point.
[06:12] And scrolling, keep scrolling. Part three is usage.
[06:18] So how are we going to use it? Is that kind of what we're going with?
[06:21] I'm guessing that's what we're going with. >> Yeah, parts, everything before that are about the language features,
[06:28] like how it works, why it does things. This is more of how you can use the language effectively.
[06:33] Like you were talking about IDEs before. IDEs give you a lot of really nice tools that make it easier to develop.
[06:38] They can assist you. They can show you every place a certain thing is used.
[06:43] Or they can help you rename something, and then all the places it's used are also renamed.
[06:48] So this goes over, for example, how to use TypeScript in an IDE to help yourself. Which I think is really useful, and you don't need that to know the TypeScript
[06:56] language, but it's so nice as a TypeScript programmer. >> Agreed, agreed, and I think that's going to be really handy.
[07:03] Because after, before that is features, and then I believe, yeah, concepts and features.
[07:10] That's probably where we're spending is going to take the longest time. Because getting the understanding of it to be able then to use it.
[07:19] So yes, we are chapter one, have a quick, I guess I could read chapter one. But the table of contents, but the quick way I understood it.
[07:33] Because y'all, I definitely, I need to listen to things to read it. It's how I learn best, so I've already listened to the chapter.
[07:44] And going through it, it made me just think, okay, here's the history of it. Here's what TypeScript is, and
[07:52] here's what we're going to be doing in the future. So it's the perfect setup of the book.
[07:59] That's normally what a first chapter is. And as we keep going, the type system, unions and literals.
[08:10] >> That's the fun stuff. >> Okay, I'm glad because I'm not there yet.
[08:13] So I'm stoked that we're going to be learning about that and objects. I will tell y'all, let's see,
[08:19] what chapter is this that I'm not looking forward to? Chapter eight, chapter eight, and I am not looking forward to it.
[08:28] >> You can completely skip chapter eight if you never use classes in JavaScript and don't want to learn them for this, totally fine.
[08:35] TypeScript doesn't have an opinion on whether you use classes or functions or whatever, as long as you're writing some code, TypeScript will look at it.
[08:41] So if you hate classes, ignore them. >> I think it's honestly like it just hasn't clicked yet.
[08:48] So maybe by the time we get to chapter eight, it'll click. And y'all, beautiful humans watching can let us know if we should do it or not.
[08:56] Because if it's up to me, I might want to skip it, but let's keep going, yay. And y'all can read the preface.
[09:07] >> We still don't know how to say. >> Yeah, we watched the intro last week.
[09:11] This was a huge thing we weren't sure of how to do, so we're skipping this. We're skipping right through this, read it yourself, go get the book.
[09:21] I do think navigating this book is smart. Look, we could have gone right here to, should have remembered that, me.
[09:28] Dang it, Jen, whatever. And yay, okay, concepts.
[09:41] >> So every chapter starts off with a haiku and ends with a pun before you ask. And I say before you ask to imply what you were going to ask, but
[09:49] really this is me bragging. I'm really excited that they let me do that.
[09:54] >> What's your favorite haiku, which chapter? >> I don't know.
[10:00] I think the one at the very end brought me a lot of joy, the last chapter. So that's something to look forward to, chapter 15.
[10:07] >> Okay. >> But actually, I also really like this one.
[10:10] >> I don't even know if I know how to read a haiku properly. Like with like the right pauses and cadence.
[10:21] >> I don't know that there is a right way. >> I don't know, I'm not a poetry person.
[10:26] But JavaScript today supports browsers decades past. Beauty of the web, done.
[10:36] That was the entire video. We are done.
[10:37] We know what we're doing. Okay, bye.
[10:39] >> Perfect. >> All right, so, and not reality because that would be very, very confusing.
[10:51] How would you describe in like a quick overview of what, like the history of JavaScript and how TypeScript was created?
[11:02] >> Sure, JavaScript was created quickly and it was never intended to be the ubiquitous everyone user for everything language that it is today.
[11:11] Also, JavaScript, because it is the language used in web browsers for web pages, which need to always work forever and ever the same way.
[11:20] It's a very inflexible language in that way. You can't break JavaScript.
[11:26] You can't break the web. So for example, there are two null or undefined values in JavaScript.
[11:31] Null and undefined, and thousands upon thousands of developers, myself included, would really like it if we just had one because it's confusing to have two.
[11:40] Other languages might have been able to fix that mistake in some new version. JavaScript can't.
[11:45] So the beauty of the web is that you can always look at old web pages. You can go to the like 1990s, whatever, Space Jam websites, and it'll work.
[11:53] But that also means that although we can add a lot of great stuff to JavaScript, which has happened, we can't change the things that are already there in a breaking way.
[12:02] Does that feel reasonable to you and match your expectation? - Yeah, that does make sense.
[12:06] And skipping ahead because to start and the entire reason we decided to do this series is Josh came on the show and we went through one of the exercises, which will be a part that we'll talk
[12:21] about later today, of how you can actually change something everywhere. And that was something that I thought was really cool in the fact of as I've been working
[12:34] on more projects, I'm finding the difficulty of not knowing everywhere I'd put something. - Yes.
[12:44] Oh, yeah. You made something and then you can never touch it again because any little push will just collapse
[12:50] the whole thing. That's a very good segue into some of the pitfalls of vanilla JavaScript,
[12:55] which is actually kind of a bad term because vanilla is a legitimate good flavor on its own. But people say vanilla JavaScript and mean just the plain.
[13:03] When you just have JavaScript, you don't have anything else. You can do whatever you want.
[13:06] You can YOLO it, but then it's really hard to change stuff later on. And there's no way, for example, in vanilla plain JavaScript to tell JavaScript what something
[13:17] is supposed to look like. You can't say that this function takes in a string and a number or whatever,
[13:22] and then later on, if you pass it something else, have anything tell you, "No, you did it wrong."
[13:26] That just doesn't exist, which is real bad when you have, like, thousands upon thousands of lines of code.
[13:33] - Very true, very true. And now, this next part, what did you mean by, like, loose documentation?
[13:43] - Yeah, so there's nothing in the language itself to say, "This is a string. That's a number."
[13:48] So people have added one in, sort of. They've added what's called JSDoc, which comes from Javadoc.
[13:53] And I like to joke, if there's one thing we should know about things about JSDoc, is that it comes from Java, which is an insult.
[14:01] I'm insulting it right now. But these are these kind of semi-formalized comment syntaxes,
[14:08] like a way to write comments indicating that, like, okay, this one parameter is a string, or this other parameter is some shaped thing we're going to call painting.
[14:17] But there's nothing that enforces you doing those rights. There's no, like, one exact syntax.
[14:22] Like, sometimes people put two spaces or four or whatever in certain places. So it's very loose.
[14:27] It's very kind of hand-wavy. - And, y'all, as we're going through this, as a heads-up, on every other Friday that
[14:38] Josh and I aren't learning TypeScript, Laura and I are working on Python. Because Laura and I started on Mondays to do Python, and then we realized that it's
[14:50] just way more fun to bullshit and just, like, get all of the random learning things out.
[14:56] So that's what Mondays became. And I say that because a big part of understanding JavaScript, for me,
[15:08] was learning Python. Because as I'm learning something else and how it works and comparing it to
[15:15] something, I'm like, "Oh!" So when you're talking about, you know, how loose it is, I'm like,
[15:23] "Doesn't necessarily make sense." But as you're explaining it, you have to put, like, in at least what I've learned
[15:29] so far in Python, like, there's certain parts where you have to put that it is a string or it is, you know, an integer or something like that.
[15:37] And it makes you, it's very concrete where now that I'm thinking about it, I'm like, "Oh, I guess when you declare something, it can be a lot more open."
[15:50] - Yeah. I like that strategy of bouncing the two languages off each other.
[15:54] - Yeah, yeah. It's definitely something where you and I talked about this a bit last week.
[16:00] A lot of people, and I don't suggest this for everybody to go back and forth between languages.
[16:06] It does get confusing. It's also something that I do it on certain days.
[16:11] Like, it would be very difficult to do it all in the same day or studying at the same time, but I associate a lot of it with people.
[16:19] So, like, for example, I know Josh is TypeScript. Days I talk to Josh, it's going to be TypeScript.
[16:25] When I talk to Laura, she understands. Her main language is Python.
[16:30] She's also very much, she's been a math professor, very much about, like, learning and learning techniques.
[16:38] So, I mostly do it, all of that, with her. So, it's very different of who, like, I just associate people with topics.
[16:48] Not sure why, but that's, it helps having that structure in a specific day that I talk to people too.
[16:55] So, yeah. - Makes sense.
[16:58] Now, this was something that I found really interesting, and, yes, y'all, I highlighted it.
[17:05] It made me very, very happy to highlight it, of JavaScript is four things. So, a programming language, and I'm not, like, reading, reading these because I
[17:16] want to talk about them, the programming language makes sense to me because it's a language you use to create things.
[17:25] - Now, you're talking about TypeScript, right? - Yeah.
[17:27] - Yes, TypeScript is four, cool, cool, cool, yes. - Yeah.
[17:30] And then, a type checker, and I'm wondering if, like, this example would work outside of programming to kind of, like, conceptualize it a bit easier of,
[17:44] instead of, like, if you have a bunch of apples, they could be named anything, like, you have Gala apple or a Fuji apple.
[17:58] But if you call something a Clementine apple, a type checker might say, "Clementine isn't an apple.
[18:06] That's not an apple. That is something else, but it's not an apple."
[18:10] And so, when we talk about type checker for TypeScript, is that kind of what it's doing is saying, "Yes, this is..."
[18:19] - Yeah. It takes a look at, for example, your labels and it shows you the ones that yells
[18:26] at you about the ones that are incorrect. Or if you call something a Clementine apple or a blue apple or something.
[18:33] Oh, my, hi, homie coder. Yeah, AppleScript, that's a good analogy, I like that.
[18:37] - I like it, homie. I like it, homie.
[18:39] And hello, homie. All right.
[18:42] And then, a compiler, which I'm not looking at the definitions. They're on my other screen, so that's why I'm like, "Over here."
[18:50] A compiler is where the... I always get mixed up with compilers, and I don't know why.
[18:57] But it compiles all of the content and then spits it back out as JavaScript. - Yes.
[19:06] I personally, I don't know how many of you folks listening are like this, but I personally like knowing where words come from because I remember things
[19:14] visually, and I remember things when they're stories. So, for me, a compiler, I visually see as like a compilation CD or set of books,
[19:23] like on the old "Whose Lines Are Anywhere" sketches when they're selling compilations, or like when you compile a bunch of books together into a series.
[19:30] So, a compiler takes an original thing and compiles it into something new. In this case, we oftentimes have a smaller output and not a bigger,
[19:39] but that's just this one particular compiler, TextScript. - So, we could say that we are making a composite of learning TypeScript,
[19:53] the book, because we are doing a series on it. - Yeah, that works.
[20:00] Let's go with it. Whatever gets the impression across that it's taking something and creating a
[20:05] new thing from it. - Okay.
[20:09] Homie said, "Facts. They, like Jen, need to know what the words mean."
[20:15] Yes, yes. And then, "Language service."
[20:20] This one I don't have a good guess on, so I'm reading it. "A program that uses the type checker to tell editors, such as VS Code,
[20:27] how to provide helpful utilities to developers." Like, that probably makes sense to people that know, like,
[20:35] languages and things, but what? - It's a service.
[20:39] Think of it, let's say a programming language is a description of your apple pie recipe.
[20:45] Content warning, food, for those who are into, are. The apple pie is describing a programming language.
[20:53] The type checker will look at your recipe and say, "No, you don't need clementines.
[20:56] Everything else is good." The compiler takes your recipe and turns it into an actual apple pie,
[21:00] and the language service is the server who brings you that apple pie. It's something that helps you use the thing.
[21:08] It's the thing that, like, when you start typing in C-O-N, will suggest, "Oh, did you mean console?
[21:13] And if so, did you mean console.log and so on in your editor?" Does that kind of help?
[21:21] I'm guessing no. - No, no, no, it is, it totally is.
[21:29] For myself, it's a bit of, you know, y'all, on Teach Gen Tech, we talk about a lot of really random things.
[21:36] And one of those are, I've also seen a high-level glance of Go, and I remember a lot of tabs to be able to autocomplete.
[21:47] That's why I was just, like, thinking about things. It was, like, taking me a second to, like, conceptualize.
[21:54] But, so language for service is a fancy way of saying, the official way, probably not just fancy, the official way of saying,
[22:04] if you hit tab, it'll autocomplete and give you the option to autocomplete. - Yes, exactly.
[22:10] Autocomplete, find all references, rename, all that stuff is language service. - Okay.
[22:16] I never knew it had a name like that. That is probably the reason that I was, like, "Oh, okay."
[22:25] And now, and what up, Travis? What, like, when you're talking to somebody that is just getting into this,
[22:39] you talk about, oh, I can do the check mark now, yay. You talk about the TypeScript playground in here.
[22:47] For people that may already know JavaScript, that are, we'll say, like, employed developers, I'm going to use that as a term only because some
[22:56] people, like, you know, you have to have a verified scope. I don't know how to say that properly.
[23:00] Do it in real life? - Professional?
[23:04] - Yeah. - Because I'm not actually employed myself.
[23:07] - Yeah, then I don't know what the term would be. You know, people that actually know the coding languages more than me,
[23:15] would you say doing it on TypeScript playground is going to be better than doing something like, you know, VS Code or something that people are used
[23:27] to using on a regular basis? - I would not say that.
[23:32] Side note, I like what building bedrock layout just said. It arose by any other name because that implies that there are thorns
[23:38] in development, which is true when we have bugs. I say whatever is most comfortable for you is totally fine.
[23:45] I personally use VS Code and then sometimes dip into the TypeScript playground for quick things.
[23:50] Honestly, VS Code and the TypeScript playground actually use a lot of the same components to show you, like, editing in TypeScript.
[23:58] It's called Monaco, the text editor that they both use. Monaco is open source.
[24:02] It's extracted from VS Code. So I just suggest the playground because it's a really easy website
[24:07] for people to visit. You don't have to set anything up.
[24:09] It just works. But if you already have VS Code locally and you're used to it, sure, yeah.
[24:14] It's all the same. - Sweet.
[24:16] - TypeScript is gloves. I like this, the analogies.
[24:20] I'm reading the chats. - Yeah, do it because that's a bit…
[24:24] See, I like having other streamers on because if I'm not paying attention to the chats, sometimes they just get really ignored.
[24:33] So I definitely appreciate. And then I am just looking up the playground.
[24:41] So, well, this is not the playground, what I post first. This is just TypeScript to be able to get it.
[24:52] Script. Wow, I can spell.
[24:55] I can spell. I promise.
[24:58] Spell or type. And then this is almost…
[25:09] TypeScript playground. Yay.
[25:18] And Bedrock says, "TypeScript helps removes those thorns or at least gives you gloves to work on so it doesn't hurt as much."
[25:28] Ooh, I like that reference. And, ooh, using playground as a quickly think through type of in isolation.
[25:40] Interesting. Interesting.
[25:42] I feel like we're going to get more into types as we go because, like, I get it but I don't get it.
[25:48] Like, I think that's the hard part is I'm like, "I understand what you're saying, yet at the same time, I can't visualize it."
[25:55] And that is why we're doing this. So that way if other people are like me, hopefully, this will help start getting it.
[26:02] All right, so I am scrolling through this a bit more because of that we'll be going through different things to be able to show later on.
[26:12] I do want to say thank you for your first, "Figure 1-1 is about Lizzo." - Yeah.
[26:22] - I don't know if I can say this enough. I think I would cry or pass out.
[26:28] There are two people that, like, I think I would melt, like, literally just, like, melt if I ever met, and that is Lizzo and Arlen Hamilton.
[26:39] And I'm like, if I met either one of them, I'm pretty sure that I would just, like, combust or melt or, like, cry, probably all of the above.
[26:50] And so I was very excited about it, being Lizzo. Anyway.
[26:56] So freedom through restriction. What?
[27:00] - Yeah. This was something that took me a little bit to feel comfortable about when I first
[27:07] got into TypeScript. TypeScript actually restricts you a little bit, but in a good way.
[27:11] It's like the little gutters when you're bowling on the side or little training wheels on a bicycle.
[27:18] TypeScript will let you know when you've messed up because it also allows you to describe what you're trying to do.
[27:23] So if you want to change a bunch of stuff, and you, like, let's say you have five, ten things you got to get through, and you only change one of them, it'll let you
[27:31] know about the other nine of them. So although it restricts you, that allows you to make big changes because you have
[27:37] these guardrails, these little training wheels on that will let you know about the things that are broken when you change something.
[27:44] Freedom through restriction. - Okay.
[27:51] All of that made sense. I just started thinking about types again, and I'm like, "I'm going to keep scrolling.
[27:57] We're going to get to that." I don't know if it just clicked or not, and I'm just not going to confuse myself
[28:05] more. So precise documentation.
[28:10] That one is just giving us an example of how it's actually saying that this is going to be a string, so therefore it has to be a string.
[28:19] - Yeah. I don't cover that exact syntax it's using for a little bit, but yes, the theory,
[28:23] yes. The syntax is showing that you can describe that, let's say if you want to call
[28:29] something a painter, like a particular object, anything that you want to call painter has to have these three things, finish, or whatever.
[28:37] So if you were to say that a place is supposed to receive a painter, and then you pass in, like, a number or something, TypeScript would yell at you.
[28:44] Or if you pass in an object that doesn't have those three properties, or if it does but they look different, TypeScript would yell at you, which is good because it
[28:51] stops you from messing up. - Okay.
[28:54] And that makes sense. And I can see how it would, by default, build stronger developer tooling.
[29:02] And hey, yay, it's the tabs. Not probably the proper way of saying it, but the tabs.
[29:10] The language services. The tabs.
[29:13] - Yeah, the tabs. Whatever works.
[29:16] I mean, we all have different slightly inaccurate terms. Like, there's no one specific correct term for any of this stuff.
[29:22] So if I call it the tabs in my head, you can call it the tabs in your head, too. No shame there.
[29:27] - Yes, the tabs. The tabs.
[29:30] And we will be going through a lot of this as, instead of just these theory pieces, we're just going through theory to start.
[29:41] A, because that's how we do a lot of the show anyway. And because knowing a bit of the theory can help us practice the hands-on.
[29:52] So we will be doing both. And what up, Jay?
[29:56] And Bedrock said that documentation in your code, instead of having to go look at the docs site.
[30:06] - Yeah. - I dig it.
[30:08] I dig it. Okay.
[30:12] And coding syntax. Compiling syntax.
[30:16] See if I can read, y'all. Compiling syntax.
[30:20] This one, I got nothing. What is compiling syntax?
[30:24] - Do you remember what a compiler is? - It takes something and makes something else.
[30:29] - Yes, exactly. So now we're talking about it for your syntax.
[30:33] We take in your TypeScript source code, the text, we call it sometimes the syntax, and it outputs your JavaScript syntax.
[30:42] So in the photo of the playground, TypeScript on the left, JavaScript on the right. The compiler took the left and created the stuff on the right.
[30:49] - So can you reverse compile? Can you take a JavaScript file and make it a TypeScript file?
[30:57] - You can kind of guess. And actually, the open source project I spend the second most amount of time on is a
[31:04] project that does that. But it's quite difficult.
[31:06] Because you lose information when you go from TypeScript to JavaScript. TypeScript allows you to document all these things, which then mysteriously disappear
[31:14] when it becomes JavaScript. Because they're TypeScript, not JavaScript.
[31:17] So trying to guess at those things is quite difficult, and you're not always going to get as good.
[31:21] It's like if you annotate in the side margins of your book, and then you try to create a new book from it, you can only guess what you would have written in the side margins
[31:31] of the book. - And that makes sense.
[31:35] And -- oh. And for those who may not know what Bedrock is...
[31:43] Yay! Bedrock uses TypeScript.
[32:00] Yay. I was getting there.
[32:04] I was very slowly getting there, Travis. So Travis was on the show -- oh, goodness.
[32:12] It's been a few months now. But it was really cool, because Travis was showing us how we can build things in HTML,
[32:23] and then we can build things in CSS. Or with Bedrock, it puts the two together.
[32:28] Instead of having to guess and make changes in multiple places. It was really cool.
[32:34] But that actually makes sense on TypeScript, too. Weird.
[32:41] When stuff starts to click, it's like this really cool and yet really confusing how it works.
[32:49] Are you going to come back on the show? I feel like we could do it again.
[32:53] I'm just not -- I don't think I've really talked -- done too much CSS since then. It's been mostly TypeScript, JavaScript, and Python.
[33:08] Yay! I am excited about that.
[33:11] Okay. So we got Getting Started Locally, which this is definitely a good walkthrough.
[33:19] And again, y'all, highly, highly suggest getting the digital book so you can just copy and paste things.
[33:25] Okay. Don't do it the way I'm trying to do it, though.
[33:29] And Running Everything Local, which we will be showing through as we're going through things.
[33:35] But Editor Features of creating a tsconfig.json. Say what?
[33:46] Yes. That -- every programming language tool, whatever, has a config file, or any one that can
[33:54] take in different config options, configuration options. And the TypeScript one is called tsconfig.
[34:00] Short for TypeScript Configuration. So we don't need to cover what's in a tsconfig now.
[34:05] That's actually one of the much later chapters. TypeScript is super configurable, because people use JavaScript in a lot of weird and
[34:11] wacky ways. But if there is a tsconfig file, TypeScript will look at it for your settings.
[34:17] Yay! Okay.
[34:20] So I feel like I appreciate that you put this in here. I feel like other people would be like, "Why are you saying this?"
[34:30] But it is really helpful to, again, know what your guardrails are, and what it is, and what it is not.
[34:37] So what TypeScript is not? How would you explain that?
[34:41] I would say TypeScript doesn't have opinions. It's only about correctness, not about doing it a right way.
[34:48] Oftentimes, there is no one right way for a thing. So TypeScript won't stop you from doing bad patterns, like copying and pasting the same
[34:57] function 20 times instead of reusing it. That's fine.
[35:00] It's type-safe. It's correct.
[35:02] It's just humans might hate your code. TypeScript also won't enforce using whatever, class-based, object-oriented programming,
[35:09] versus functional, versus just a whole bunch of random stuff. As long as it's type-safe, as long as you don't mess up your types, TypeScript doesn't
[35:17] care what you use. Which is why I was saying earlier that you can totally skip the classes chapter if you
[35:21] never use them. All right.
[35:25] So if I'm thinking about TypeScript, it's kind of like Grammarly. Grammarly will tell you if the structure is wrong, but it's not going to tell you if
[35:41] it's not, I don't know, spelt wrong, or something like that, or used wrong. You can think of, I would say TypeScript is like Grammarly, or like the spell check in
[35:52] Google Docs or Word. It'll tell you whether you've spelled your words right, and if the grammar is correct.
[35:56] And Grammarly will even give you phrasing suggestions, like, "Oh, you might want to remove these words."
[36:02] But if you're writing an op-ed, an essay about how, I don't know, I'm going to make a sports analogy here.
[36:08] I never, "The Red Sox are better than the Yankees." It's not going to tell you, yes, they are, or no, they aren't.
[36:14] You might be totally wrong in your opinions. But as long as your sentences are well-structured and the words are spelled correctly, it's
[36:20] okay. I don't know if someone's going to get upset about what I just said about the baseball
[36:26] teams. I couldn't think of anything more good than that.
[36:29] No, it works. It works.
[36:32] It works. And Travis came up with, Grammarly is a great example because you can also tell Grammarly
[36:39] to ignore things. And I like that because I think that's a good way of going back to it, too, because it's
[36:48] like you can, it'll tell you something's wrong, but it's not going to stop you from running it.
[36:53] So, you know, you can say that the Red Sox are bad, but it's not going to prevent them from playing.
[37:00] I just thought of a better analogy. I hate using sports analogies.
[37:06] They're not appropriate for me. Okay, because I was like trying, I call it like sports balls.
[37:11] So although the Chargers, like if anybody wants to know, I'm a Chargers fan because Tyler's from San Diego.
[37:19] He's a diehard Chargers fan. So they're playing on Sunday.
[37:22] Yay. Fun fact, that's actually a laptop's favorite sports team.
[37:26] The Chargers. Okay.
[37:32] Anyway, I won't think anybody, I'm going to go ask him now. What's a laptop's favorite sports team?
[37:39] Yeah, he probably won't know. I like know the answer and it's going to be really exciting.
[37:43] Thanks for helping me with getting some points. I appreciate it.
[37:46] There you go. An analogy I was thinking of is you might describe a recipe, like we were talking about
[37:52] apples before, Grammarly, Word, Spellcheck, whoever, they can tell you if the recipe is well structured, if it like contains real ingredients, but it's not going to tell you
[38:01] that like, oh, your recipe is terrible and this is going to taste bad. There's no way for it to know that.
[38:05] So, oh, oh, okay. Since we were talking about apples earlier and TypeScript will tell you that a clementine
[38:15] is not an apple, it's not going to prevent you from putting clementines in the pie. Yes.
[38:21] There you go. We made it and-
[38:26] Which actually might be good. I don't know.
[38:27] I've never tried that. I think they would be too watery because it's like you can't-
[38:31] Has anybody tried dried like orange chips? Are those a thing?
[38:37] Can you have them as a thing? Because I don't think-
[38:41] Bars will have them for like mocktails and cocktails. Oh, yeah.
[38:44] I've seen them at Trader Joe's. And yes, Jay, I feel that's how he feels too.
[38:55] And he's like, he's going to, no matter where we move, Tyler will always love the Chargers, which I love the Chargers.
[39:03] Yay. Bolt up.
[39:04] He doesn't like it when we went to a Broncos game because I live in Denver, y'all. I promise I'm almost done with these stories, but it was a Broncos Chargers game.
[39:15] And I kept wanting to like, be like, see it. Every time I saw a Chargers person to be like, bolt up.
[39:20] And Tyler's like, please don't. I don't need us to get in a fight with someone because they hear you being a Chargers fan
[39:28] really loud. Okay, fine.
[39:32] Anyway, back to actually TypeScript. Extension to JavaScript.
[39:42] How does it not do that? Sure.
[39:46] This is a really important delineation distinction. For the most part, and there are unfortunately a couple asterisks there, TypeScript does
[39:55] not add new runtime syntax. JavaScript lets you define things like variables, functions, arrays, whatever.
[40:01] TypeScript just, for the most part, puts type annotations around those. You create a function in JavaScript and then use TypeScript to say that the function takes
[40:09] in a string and a number or something like that. So a lot of times people will ask, oh, can we add something to TypeScript that's a runtime
[40:18] feature, like a new way to write a function? And for the most part, no.
[40:21] TypeScript does not change JavaScript. Its goal is to be a superset that just adds type stuff.
[40:26] And that's because if we add new runtime things in TypeScript and then later on the JavaScript language also adds an equivalent to that thing, now you've got competing versions and one
[40:37] will not be compatible to the other. So that would be really bad.
[40:42] Unfortunately, very early on, TypeScript added a few runtime things, JavaScript extensions, which I cover at the end of the book.
[40:51] For the most part, people try to avoid them. So I don't need to cover them until the end of the book.
[40:56] We don't need to learn them for a while. But just know that although they never do this anymore and for the most part do this,
[41:02] early on there were a couple things that were just so gosh darn useful that they didn't. And then Travis just said, "Example is lowercase private in TypeScript versus official
[41:18] capital private fields." So this is actually a really interesting one.
[41:23] TypeScript. So this is classes.
[41:25] Trying not to explain needing to understand classes too well. But you can-- each instance thing, like if there's an Apple class, each individual Apple
[41:35] can have some private members that no one else can access. There's a way in TypeScript to describe that in the type system that isn't a runtime thing,
[41:43] like it's not reflected in the runtime JavaScript. And later on, many years ago, now recently, JavaScript added a syntax, like a hashtag
[41:51] syntax, to describe that something is only available to itself. No one else is allowed to see or touch it.
[41:56] But fortunately, the TypeScript syntax is just in the type system. It's just I'm saying that this is the way it is.
[42:02] It doesn't actually exist in the output JavaScript. So that one is-- we're safe.
[42:08] We're allowed to use it. It's not an extension to JavaScript, even though it does a similar thing to a later
[42:12] on JavaScript feature. Everything you're saying makes sense.
[42:17] I will say something that, again, is one of those things that I'm like, I feel like I should know what this means.
[42:26] I kind of know what it means in runtime. But please remind me or in context of what runtime is.
[42:34] Like, it means how long it takes to run. I'm guessing that's, you know, runtime.
[42:39] But like, when a browser, like, could you-- what? Runtime?
[42:46] Runtime is an unfortunate word, because it means two things. It means what you just said, like how long does it take something to run, the literal
[42:53] time. But it also means like stuff that gets executed in the browser.
[42:56] Could you do me a favor and actually open the TypeScript playground? So we can see it.
[43:03] Because I think it's really easy to show it visually while describing. Yeah.
[43:08] So if you could, like, let's say create a variable. Just say, like, let value equals true or something like that.
[43:16] And just delete everything else. Yay.
[43:24] Cool. Like, I don't remember.
[43:28] Is this-- yay. Like, I did it.
[43:33] In Python, it's a capital T, and that always trips people up going back and forth. Yeah.
[43:37] Yeah. All right, cool.
[43:39] So on the left is the source TypeScript. On the right is the output JavaScript.
[43:43] You can ignore that use strict string. That's just like a safety measure.
[43:45] It's a whole other shebang. We don't need to worry about it.
[43:47] So really, they're basically the same thing. Let value equals true becomes let value equals true.
[43:52] But if you were to put next to the word value, just to the right of it, between it and the equal sign, type in colon space Boolean.
[44:01] Yay. So now we have a difference.
[44:09] Now on the left in the TypeScript code, you have created a variable, which is all JavaScript. And in TypeScript land, the type system, you have said this variable is only ever going
[44:18] to be a Boolean. That colon Boolean exists only in the TypeScript understanding of the code.
[44:24] When you output JavaScript, when you compile to JavaScript, which is what you get on the right, anything that is only in the type system gets removed.
[44:32] Notice no colon Boolean. So that's what I mean by type system code versus runtime code.
[44:38] I get it, but I don't get it. But I mean, it makes sense.
[44:49] And thank you, Will. Will is over on YouTube and says a fair runtime question.
[44:58] So thank you. I feel like it's something that, again, it needs to be noodled on.
[45:05] And actually, I'm -- and then Travis just said, runtime code means the code that the browser actually sees.
[45:16] And so, Travis, how are you on classes? Because -- and y'all, I'm particularly annoyed at classes because before Teach Gen Tech was
[45:31] created, there was a course on LinkedIn about JavaScript, and it had classes. And I could not conceptualize classes.
[45:43] I got so stuck. And I was like, I'm never going to learn how to code because I hate classes.
[45:49] Because it's just not clicking. So it's like one of those things that I -- like, even as you said, Josh, a lot of people have
[45:54] said this to me, that they don't -- like, you don't really need to know classes. Like, you can get around without using classes.
[46:01] I'm like -- but I couldn't figure it out. Now I want to know what it is.
[46:06] Because it stumped me. So yeah, we'll just, you know, keep going.
[46:13] And that also makes sense why slower than JavaScript. And finished evolving.
[46:18] Yeah. JavaScript is still evolving.
[46:22] TypeScript is still evolving. None of this is sedentary.
[46:25] They're all changing over time. Fun fact, the TypeScript repository is one of the most active repositories on GitHub.
[46:32] Lots of features and bug fixes and performance improvements. >> It's not, like, the most.
[46:38] But it's definitely, like, upper echelon of activity. >> All right.
[46:42] All right. And Travis replied to me.
[46:48] Thank you, Travis. Travis typically writes functional styles.
[46:52] So no classes. But depending on the code, they might still need to use it.
[46:56] I need -- I feel like there are a few things that we really need on the show. So if anybody knows anyone is -- so we're going to say classes is one.
[47:06] But two, protocols. All the protocols.
[47:11] All the protocols. That's a confusing life.
[47:16] Anyway. So we are to the summary of chapter one.
[47:21] Ayo. Yes, we got a brief history of how we went from Vanilla, got some TypeScript in the world.
[47:32] Pros and cons of both. And also how TypeScript tells you if you have Clementine -- trying to call an apple a Clementine
[47:41] apple and will still let you cook with Clementines, but it will at least warn you that a Clementine is not an apple.
[47:49] And if you do not get that reference, please go back about 40 minutes and it will make more sense.
[47:58] And the advantages of TypeScript. And I do see how -- if I'm -- I'm going to work on sticking with this apple reference
[48:09] each of our -- of our videos. So that way hopefully, you know, it sticks and makes sense for us.
[48:16] If we are talking about, you know, is it Fuji or Fiji apples? Fuji apples?
[48:28] Fuji, I think. Yeah, Fuji apples.
[48:30] We're talking about Fuji apples. And we have a bunch of Fuji apples in so many different areas in our code.
[48:38] One of the things TypeScript does do is if I wanted to change it from a Fuji apple to a Granny apple.
[48:47] Granny something apple. Granny Smith apple.
[48:50] See, I don't even know all my apples. I just -- what popped in my head.
[48:53] We could do that with TypeScript. And it will change all of them.
[48:57] Oh. And you got to go -- if possible, apple picking is a lovely activity.
[49:06] And this is why I think -- at least I and perhaps also Bedrock are real up-to-date gal apples.
[49:12] See, I really like Pink Lady. Those are fine apple species, whatever.
[49:17] I -- like I knew Macintosh was an apple because that's why it's called apple. But like has anybody eaten a Macintosh apple?
[49:28] Is that actually a real thing? Like it's --
[49:31] Yeah. Oh, wait.
[49:32] I was -- I'm Latham. I'm from Latham.
[49:34] Shout-out upstate New York, near Troy, near Albany. That new one's great for apples there.
[49:40] We get all sorts of apples. Green, red.
[49:43] All the colors. Saratoga Springs!
[49:46] Oh, my God. Neighbors.
[49:48] Yes. No, this is perfect.
[49:52] As you join our live stream of TypeScript, you will learn about apples and also more about upstate New York.
[50:01] I've never actually been to New York. It's a very weird thing to say.
[50:04] Like people go to, you know, the states to see New York. I'm like, I've never been.
[50:09] I don't know why. The city is fine, but the state is beautiful.
[50:13] Yes. I'm going to pause us because we've already gone through so much.
[50:18] But there is something really cool that I want to go through on -- and then let me copy and paste this really quick -- is there are different projects, practices?
[50:38] Projects, yeah. Projects that we can go through that I'm giving up that says homework, y'all.
[50:44] And we'll go through it next time we meet up. So in two weeks of the typinator.
[50:53] I do like that you have punny things. It does make it a lot more amusing.
[51:00] So although sometimes I stare at them and I'm like, how am I going to say this? But for everyone, we're going to do the chapter one assignment.
[51:11] Assignment is the word I was looking for. Assignment.
[51:14] It is a project, but an assignment of homework. So go test this out.
[51:21] Comment on the YouTubes if you get stuck. And I will be sharing that.
[51:26] And on Monday, we will get the link to everything and also see how everybody's doing as a homework check.
[51:33] And I -- what is in two weeks? Two weeks is Black Friday.
[51:39] Oh, is that already? Is it?
[51:43] Is it? I think it is.
[51:44] That makes sense. Yeah, yeah.
[51:45] Because that's 14 plus 11 is 25. Yeah.
[51:50] Are we -- are we meeting on that day? I mean, I'm down, but I just want to check.
[51:57] Like, I don't know if we are. I don't think I should take a meeting on Thanksgiving weekend.
[52:05] Let's say I don't think I can make that. Okay.
[52:08] Okay. So it might be a little bit before we meet again.
[52:11] Or we'll just figure out another day for us to do this. And yes, thank you.
[52:19] Thank you, Coco, for even after working in TypeScript for a while, it's always good to brush the dust off.
[52:29] Yes. Yes.
[52:31] And TypeScript is -- having different people try to explain it. I've heard so many different versions and ways.
[52:40] And luckily, the way Josh explains things lets me ask a lot of different questions and also try to come up with Apple analogies that Josh, you follow along with.
[52:52] So it works really well. And thank you for that, because I get lost if I don't have an analogy to go with.
[53:00] So -- and anyone have questions for Josh before we end chapter one today? And if you want to get the book, we will have links on Monday-ish of where you can get the
[53:15] digital book to follow along with us. Also where to get the real book.
[53:19] And yes, I am talking of the book a lot, because Josh is spending a lot of time with us. So -- and I like -- it's books like these that I don't learn very well by just reading
[53:29] them, but it's -- I like having physical books, because then I can -- I can do this. And write.
[53:38] Oh, no, the book! Just kidding.
[53:39] That's great. That's a good way to learn.
[53:41] Sorry, bro. It's not your book.
[53:43] It's my book now. I bought it.
[53:45] Got it. Everybody go buy your book.
[53:47] Because I like being able to write and keep notes, such as I will be adding in a compiler and a language service, because of apples and all of that.
[54:01] So that is why -- wait. Plus books on your shelf self makes it look like you know how to read.
[54:13] Yes, this is true. I actually don't have a lot of books in the house.
[54:17] Like, we only have like a handful of books. And it's because -- and I used to have so many books.
[54:24] And it's because I don't read. I listen to audiobooks.
[54:27] You want me to listen to an audiobook on double or triple time? I got you.
[54:31] I've read a lot of books this year. And podcasts.
[54:36] But physical books and I -- this is my favorite one for the year. 2022 version.
[54:44] Right here. Yay.
[54:46] Yay! I appreciate you saying that, Jen.
[54:49] Yeah, I appreciate you going through this. Because it's -- no, seriously.
[54:54] Learning a language or learning TypeScript is something that I think has bad rap. Because I think it's hard for people to conceptualize.
[55:03] And if we can make it so that way people can understand it and conceptualize it and can use it, it's well worth it.
[55:09] Because it is a tool that a lot of us could really use. Absolutely.
[55:13] Thank you, everyone. And we will see you in a few weeks.
[55:18] We'll announce when. And next week you will have the information on the YouTubes of how to use it all.
[55:26] Jay just said don't worry. TypeScript push types will make TypeScript more approachable.
[55:36] I don't know if I understand. You neither.
[55:41] Sorry. But I like making TypeScript more approachable.
[55:46] That's good. I will say -- so Jay is -- Jay and Homi are the ones -- oh, I will show you guys this.
[55:53] Josh, you're getting stuck on a stream for a little longer. That's okay.
[55:58] It's what we were talking about earlier. The project that I'll be asking you questions about.
[56:06] JavaScript is talking about adding more type support. Oh.
[56:13] Nice. They're adding in the ability -- so they're talking about it.
[56:18] Even if it does happen, which is not certain, it will take several, several years. But they're adding in the ability for you to put in little annotations in your JavaScript.
[56:27] They're equivalent to comments but with a nicer syntax dedicated to describing types. Looking very similar to how TypeScript does things.
[56:34] That would be -- it would just be super convenient. But it doesn't -- it's not adding in a type system.
[56:40] It's letting you run your own type system such as TypeScript. It's just making it easier to annotate your code for type systems.
[56:48] Interesting. And Jay, I don't know if you were here earlier when I was comparing it to
[56:54] TypeScript is like how Python makes you say that it's like a string. Is how I was conceptualizing it earlier.
[57:03] But all right. Oh, no.
[57:05] Come back. Add to stream.
[57:07] There we go. So, y'all, GitHub community standards, come hang out with us over here.
[57:16] Jay and Tomi created this. I technically am hanging out here and doing stuff, too.
[57:23] I say that because it's still going over my head. So, what we're doing is when you start a new repo, there are certain things that you need
[57:37] to make it accessible for the community. And GitHub shows us what those community standards are.
[57:45] One of which is a code of conduct. And Jay made the fancy code of conduct and donated his code to our project to be able
[57:53] to show it. But that's cool.
[57:57] And we're a step in the right direction. But it still makes a lot of it confusing for everything else.
[58:03] So, if we go into the GitHub community standards, we can scroll down. Love that image.
[58:10] Thank you. Thank you.
[58:12] This is why they keep me around is I like graphics. Is these are what a community standards require.
[58:21] Is your description, your readme, your code of conduct, contributing, license, security policy, issue templates, pull request templates, repository, admins, except content reports.
[58:34] And yet it doesn't show you the health of all of it just by looking at it. It, like, shows you just this bar.
[58:43] And it doesn't really always give you access to where you can find all of these or examples. And that's what we're building.
[58:50] And we are using TypeScript to do it. And also, Jay and Homie, please add in anything else that I am missing.
[59:00] Because Jay was doing some really, really cool things. And I wasn't 100% understanding them the other day.
[59:09] But we were doing some cool stuff on Tuesday's stream. So, come hang out with us and do that when we have Jay and Homie on the stream again.
[59:21] I love how everybody is, like, overlap. Like, all of my streams start to overlap with each other.
[59:29] It all flows together. Blends in, like, a nice plate of Indian food.
[59:34] All the flavors seeping in together. You've gotten me really hungry for this whole stream because of all the Apple stuff.
[59:39] >> You're welcome. Yay.
[59:42] And yes, yes. And I would say...
[59:46] Okay. So, Homie said this about Jay.
[59:48] I'll also say about Homie. Because Homie's my homie.
[59:52] Okay. Yes, yes.
[59:54] Homie has a real name. But I still call him Homie.
[59:59] Because it's fun. And Jay just said they have no idea what they're doing in TypeScript.
[60:08] They just pretend to do things while furiously searching for things. Yes.
[60:12] And this is what we did the other day. Yet there is a huge difference of knowing the concepts of programming in general versus,
[60:25] like, just learning a new language. And there's a lot of leveling there.
[60:29] So, that's why we have Teach Gen Tech. So, that way we get to do all this stuff together.
[60:34] And because you cannot rush... Oh, I just thought of this the other day of what I was trying to say.
[60:40] Consistency. You cannot rush consistency.
[60:43] Consistency takes time. That is what I was...
[60:50] Yay. I finally got to say it out loud.
[60:51] I'm excited. Well, beautiful humans, you know where to head us up.
[60:56] Oh, yes. >> Sorry.
[60:56] I've got one more thing to add. I'm going to do this after every chapter.
[61:00] There's one part from the chapter that's very important that you missed. Why did the string and the number break up?
[61:05] >> They weren't each other's types. >> Yep.
[61:10] They weren't each other's types. >> I had to think about it because I'm like, I read this.
[61:14] I read this. I read this one.
[61:15] I read it. Yes.
[61:19] Yes. Now, for next times, y'all have to figure it out.
[61:24] Today I got it. But next time you have to.
[61:27] Yay. Bye, everyone.
[61:31] - Bye. 
