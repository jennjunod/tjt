---
showLink: "https://www.youtube.com/watch?v=NLbSYsgckd0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-backend-development-with-express-js-guest-ram-n-huidobro-pt-1"
title: "Teach Jenn Backend Development with Express.js guest: Ramón Huidobro Pt 1"
publishDate: "2022-07-11"
coverImage: "https://i.ytimg.com/vi/NLbSYsgckd0/maxresdefault.jpg"
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

[00:00] >> Thank you for joining Teach Gen Tech. I actually got it right this time, I'm pretty excited.
[00:05] This week, we actually have more than one guest this week, and today to start off our week,
[00:12] we have Ramon and it is all Ramon's fault of why I got into this, because he's the one who gave me the idea of
[00:22] learning live and to peer programming. Hello, Ramon. I deserve no credit for that.
[00:30] It was so lovely to having a conversation with you, Jen, and I just love your energy and the way you learn in public,
[00:38] because it's such a cool thing to do and such a cool reminder to all of us, that we're all learning at some point.
[00:44] With a lot of things in tech, it's an ongoing learning thing,
[00:47] so being able to do so in public and for me, one of my favorite things about streaming is I can do that in public,
[00:54] can't be perfect when you're live, so I'm going to make mistakes and people are going to take
[00:58] notice and just be like, "Huh, it's not just me that never remembers how to make an Espresso."
[01:05] >> Yes, and I love also just from a production side, you don't have to edit it because it's live.
[01:13] >> Absolutely. Exactly, there's no editing needed. That's also the best. Hey, we got a comment from.
[01:21] >> Yay. Yeray. No, we're done. Okay. Yeray, see, I totally butchered names.
[01:30] We've got more. Yay. Welcome, everyone. >> Love to see it. Hey, everybody.
[01:38] >> Yay. What are we talking about today, Ramon? Where are you from? What are you doing?
[01:46] >> Right. I got caught up in the excitement about streaming itself. Yes, hi, my name is Ramon.
[01:51] I'm coming to you live from Vienna in Austria. I'm originally from Chile,
[01:56] but I've been living here for pretty much all of my adult life. I'm a software, I've been developing software for 12 years,
[02:04] and just learning in public, teaching in public, all the good stuff,
[02:09] it's a joy of mine. My focus has been mostly on Mac OS and web software.
[02:16] Let's see, what am I working on? I'm working at a company called Suborbital.
[02:21] We do WebAssembly extensibility for your apps. I think that about covers me.
[02:29] >> That is awesome. Also, you have been one of the couple people that have just been keeping
[02:38] me in the loop of keep going, which has been really, really helpful.
[02:44] Oh, go ahead. >> No, I was just going to say that means so much.
[02:48] I think the best thing we can do for each other as tech folks is motivate each other.
[02:53] It's honestly that aspect of community that's kept me around. >> That's actually something that I found really
[03:00] surprising is the Twitter tech space, Tech Twitter. Okay, first off, only been on Twitter for
[03:07] a month of actually using it and now I'm addicted. But also, everyone, for the most part,
[03:15] is pretty friendly and I would say all dev roles or dev advocates, dev evangelist, there's so many names, are super dope.
[03:25] I love that because since that's what I want to get into, I'm like, "You're people, people,
[03:30] and you know the tech. This is exciting." >> Yeah, I'm glad. No, it's been wonderful and I have very few regrets.
[03:41] I see here that AJC Web Dev knows Suborbital and the founder, Conor. Yes, I'll send him your regards if I may.
[03:50] >> Yeah. >> Yay.
[03:54] >> Sorry. >> Go ahead.
[03:56] >> You know what? I got so caught up in myself, I didn't even talk about what we're doing today.
[04:02] Last week, I saw you live doing some React, which was super fun and I loved watching that.
[04:12] Immediately afterwards, sent you a message like, "We were originally going to do some intro to open-source stuff,
[04:18] but I got so excited I messaged Jen right afterwards like, "Do you know what we could do?
[04:22] We've done some front-end. What if we just dip our toes into some back-end?"
[04:27] That's what we're going to be doing today. Very gently, very fun, very easy.
[04:32] We're going to be checking out some back-end software development with JavaScript.
[04:37] Using a framework called Express.js. >> AJC web dev wants to know,
[04:46] are we going to deploy some Kubernetes pods? >> Not today. I still have to
[04:54] learn the ins and outs of Kubernetes first, in all honesty. >> I feel like at some point because that is something that I've been,
[05:02] I'm like, I'm going to work on that eventually because it's that, and Docker, and knowing people that I've worked at both,
[05:11] I'm just like, I'll get there. I will get there in time.
[05:15] >> Yeah. There is no rush. There is no optimal route.
[05:22] As AJC web dev says, don't ever learn Kubernetes,
[05:25] learn Docker really well. There you have it. >> Okay. I used to have a ton of Docker shirts
[05:32] because my second cousin used to work there. I didn't know what it was back then.
[05:38] I just really like the whale. >> It's a cute logo.
[05:41] >> But I would say that's probably something with gravity as well. They have new to the Graviton,
[05:46] so I'm like, I want to work there because their logo is, their mascot is so cool.
[05:52] I will say I am most excited about our chat today because you said that it also will have to be with APIs.
[06:00] I'm excited with being one of the co-organizers on the Denver API Meetup.
[06:07] That I used to work for Stoplight and never fully understood APIs and API specs
[06:13] and until very late in the game there that I'm like, yes, I'm finally going to get there.
[06:19] >> Yeah, no, that's awesome. Yeah, that's it. It's going to be gentle, it's going to be fun,
[06:25] and we'll get as far as we can until we either get tired or run out of time.
[06:29] >> Perfect. >> Shall we go ahead and share your screen?
[06:35] Oh, this looks lovely. Yeah. You've got here your React app from last week.
[06:46] >> Last week, yeah. >> Yeah. I think it would make sense to start a new project.
[06:53] >> I'm not going to lie. This was confusing. AJ had to help me through this last time.
[07:02] >> Oh, yeah. >> There we go.
[07:08] >> Wonderful. We're going to probably make a new folder. Yeah, where do we want to put that?
[07:17] Yeah, I think we're going to have to, I would actually do that from the terminal.
[07:21] How about we go back here. Do you have a folder where you normally do your coding?
[07:26] Do you have some folks have a dedicated code folder or a coding folder in their home folder,
[07:32] maybe on your desktop or something? I don't know where you put it, or documents.
[07:38] >> I will now. >> Okay, cool. Code folder, that's a good name.
[07:45] Let's go hop back on the terminal and we're going to navigate into that new folder.
[07:54] >> Talk me through it because I do not remember any of this from back in the day.
[07:59] >> We're going to do this step-by-step. We're going to cd or change directory,
[08:04] followed by a space. You can see there's a little next to gengenod@boss,
[08:12] there's a little tilde, a little squiggly character. That's the folder we're currently in at the moment.
[08:19] I like to think of the terminal as a finder window right there. Right now, we're inside a specific folder,
[08:26] which is the home folder. We want to navigate from there to the desktop folder.
[08:31] The desktop folder is always located inside the home folder. If you start typing desktop and then hit "Enter",
[08:38] terminal will like to access files in your desktop folder. >> Then cd code folder?
[08:48] >> Yeah. We're going to run into a bit of an issue here because it says string not in PWD code.
[08:57] This is the thing about the terminal that's a little bit wonky to get used to.
[09:02] You see, spaces between each, let's say, command or word are treated as a separate thing.
[09:11] We have two options. Either we rename our code folder to have no spaces in it,
[09:17] or we use quote marks around when typing C. >> Okay.
[09:23] >> It's totally up to you which one we use. >> Hey, Joe, real quick.
[09:29] We are focusing on Express JavaScript, but JavaScript is everything that I've been working on to start
[09:39] learning before I go into Python or GraphQL. >> Cool.
[09:46] >> Yeah. We can either rename it or go with quote marks. That works too. Now you're going to see we're inside that folder.
[09:57] Awesome. Express is a JavaScript library that uses Node. Yes. We're going to be doing some Node.js today,
[10:05] which did a little bit of last week. Is that correct? >> Yeah. Because I had to install it.
[10:12] I need to do homework for that still. >> That is what I'm going to be. No, we didn't do that last week.
[10:17] >> Oh, we talked about it. Sorry. >> What did I install then that was for the nodes?
[10:23] >> Oh, you probably did install the node. Yeah. >> I was like, AJ talked me through it.
[10:31] It was just before we got started. >> Yeah. Awesome. Yeah, exactly.
[10:36] We're going to be using that again, except we're going to be, yeah.
[10:40] So we didn't run any Node scripts per se. Node is also your local build tool.
[10:48] Yeah. We did a little bit of NPM stuff last week. Is that correct? I think so.
[10:59] I seem to recall you ran some NPM commands. NPM, short for Node Package Manager,
[11:06] lets us install and manage JavaScript packages locally on your machine. Good so far?
[11:15] >> All right. Yeah, we do have another question. In the naming, can we use a double quote or single interchangeably?
[11:24] >> I'm not sure. Do we want to try it out? You can always cd dot dot and try again.
[11:31] >> Is the dot dot the backwards? >> Like one out.
[11:35] >> Exactly. So we're back in desktop. Sorry. Do you know what?
[11:43] The single quote would be doing it without shift, I think, on the English keyboard.
[11:49] So it's not putting two double quote. So the symbol is called double quotes, right?
[11:55] The quote marks. >> Oh, yeah.
[11:58] >> Yeah. So if you type in cd, and then there you go.
[12:04] Let's give that a try. So that answers your question. That works too.
[12:11] >> Thanks, Joe. >> Yeah. I love these kinds of questions.
[12:14] Sometimes it's interchangeable, depends on the command you're trying to do. So I always go when in doubt,
[12:21] use double quotes for terminal stuff. I could be wrong and I'm happy to be corrected on that.
[12:29] But yeah. So we're going to create our own Node project. Do we want to cover what Node.js is and how it relates to JavaScript?
[12:42] >> Yeah. Especially since I got so mixed up with last week's. >> Yeah, sure. So I'm going to probably butcher this,
[12:55] but I'll give this to the best of my understanding. So Node.js is a runtime that is a program that lives on your computer,
[13:02] that all it does is execute JavaScript on your computer, right? It's a program to which you give some JavaScript and it'll say,
[13:11] "I got you. I'll run that JavaScript." >> Right. Because there's some front.
[13:20] I think this is where it also helps with like, is it something that Vercel does?
[13:27] Because it takes the front-end stuff to the back-end stuff. >> Kind of. As AJC Web Dev says,
[13:36] at its inception, JavaScript was meant to run in the browser, right? Each browser will have its own, what's it called?
[13:44] Runtime, right? Each browser runs JavaScript its own way.
[13:48] They are according to a pre-agreed upon standard across different browsers and technology vendors, right?
[13:56] >> Okay. >> Sound good? Right.
[13:58] >> Yeah. >> Some folks took that,
[14:02] brought it over to run locally on your machine, and said this is called Node.js,
[14:07] and all it does is run JavaScript locally on a machine outside of a browser. As AJC Web Dev says,
[14:15] Vercel runs Hella Node. So there you go. >> Or on a server, right.
[14:22] >> Okay. >> We good so far?
[14:26] >> Yes. >> Cool.
[14:28] >> It does look like we have one more question from the crowd. >> Oh, yeah.
[14:31] >> Does it compile as well or just a runtime for web framework? >> I'm not an expert on this, but I think it interprets JavaScript.
[14:42] That is, instead of reading all the JavaScript and giving you an executable file, like a.app file or something,
[14:50] to be like, "Hey, take this and you can run it," right?
[14:54] What it does is in real-time, it reads it and goes like, "Okay, done.
[14:59] Okay, done." It reads and interprets, that is, executes at the same time,
[15:04] each line of code. Sound good? >> Yeah. I'm seeing what AJC said.
[15:12] JavaScript is an interpreted language, but it doesn't compile like TypeScript or JSX.
[15:18] Okay, cool. >> Cool. We're going to go ahead and create
[15:25] our first local JavaScript file. Sound good? >> Yes.
[15:36] >> Let's open VS Code locally in this folder. What we can do is either do
[15:44] code space dot to open this folder in VS Code. Should we give that a try?
[15:52] >> Oh, wait. >> Command not found code, totally fine.
[15:59] What VS Code lets us do is install a little program that says, "Hey,
[16:02] open me in VS Code." But since we don't have that now,
[16:05] we can do one of two things. Either we can set that up or we can go by
[16:08] the open folder method from last week. Do you want to try and install that?
[16:15] >> Sure. >> Yeah?
[16:17] >> Yeah. >> All right. I think if you go to file,
[16:21] we're going to go down all the rabbit holes. If we go to file, let me see, file.
[16:28] I'm looking on my machine as well because I can never remember what the command is.
[16:32] It is under, is it edit? We're going to be opening up a little command tray,
[16:42] which I know as shift command P. If you go back to VS Code and put in
[16:49] the keyboard shortcut shift command and P. What this has done is opened up a little console that lets
[17:00] us run some VS Code specific commands. We have a little search bar,
[17:07] we're going to look up a specific thing, which is code, I think.
[17:12] >> I'm learning where to put my mic and my keyboard. >> Oh, yeah, you're good.
[17:19] >> Code, there we go. >> Oh, yes. You see where it says,
[17:22] shell command colon, install code command and path, that's us.
[17:28] >> Do I want to click the gear or just click "Enter"? >> I think you want to press "Enter" on it.
[17:32] Yeah. Shell command code successfully installed in path. Let's go back to our terminal, try it out.
[17:40] I don't know if that's going to work. Let's see. Hey.
[17:43] >> That's exciting. >> Yeah. Let's let it access file.
[17:47] What we've done now is anytime we want to open a folder in VS Code, we can do it from the terminal, which is pretty cool.
[17:53] >> Yay. All right. >> Awesome. We're one step ahead.
[18:00] Now, we're inside our folder now. Let's create a new file in this folder, shall we?
[18:07] You can do that here. I think there's a little icon a little bit higher up. Yeah. Let's call it app.js.
[18:14] That's A-double-P.js. This is our JavaScript file which we're going to execute
[18:21] with Node.js locally on our computer. Let's keep it nice and simple.
[18:27] Let's have it. Let's have it. Are you familiar with console.log?
[18:34] >> We've done it. >> Let's do a console.log.
[18:38] Let's do console.log and then we'll need some brackets for some arguments. >> I don't think I've done arguments yet.
[18:51] >> Parameters, I always mix up the terms. If I say parameters or arguments,
[18:55] I mean the thingies that go inside the brackets. >> Perfect.
[19:00] >> This is a function call that we're going to pass as an argument, a string, which is double quote marks.
[19:08] Inside that string, we're just going to enter some text that's going to show up,
[19:15] that is be console logged when we run our script. It can be anything. Let's say, I don't know,
[19:21] hello from teachgen tech or something shorter. Hello world is the usual go-to.
[19:29] I love hello, beautiful humans. Lovely. Awesome. Well, that's done.
[19:38] Let's go ahead and save that. >> It looks like we have two comments.
[19:45] Thank you, Joe. He said, externally, you both sound brilliant.
[19:50] >> Well, thank you. >> That is super exciting.
[19:54] I'm feeling imposter syndrome hardcore. >> You're sounding fantastic.
[20:00] >> I will say, Tiffany from the podcast will be very, very excited that I'm finally set up my mic.
[20:08] AJC said, arguments that actually, I forget that I can put these on the screen.
[20:16] >> You can click on it to highlight it. Yeah. >> Yeah. It's so exciting.
[20:20] Can I do it? >> Wait.
[20:21] >> No. >> I think you want the second one. Do the other, yeah.
[20:26] >> Arguments are the actual values passed to the function parameters or what the function
[20:33] defines as having the thing that gets passed through. >> Here, we're calling a function called log.
[20:47] We're passing to it arguments. But somewhere in another file,
[20:52] the function log gets defined, and to it, we declare
[20:58] what parameters we're going to be passing to it. We'll get there. But in this context,
[21:07] we're using arguments. Thank you very much for the explanation.
[21:11] >> That means I had to go all the way away. >> You're good. Actually, I think you can hide it, honestly.
[21:19] >> That's what I thought I was doing, but okay. Well, we'll see if it comes back. There we go.
[21:25] >> It'll come back. I think you can toggle it with that. I don't know why I'm pointing.
[21:28] You can toggle it with the two document icons at the top-right of the. >> Oh.
[21:35] >> No. Not top-right, top-left. Sorry. >> Okay. Well.
[21:39] >> You can close those other ones. >> I just really want to have as many of the same document open.
[21:45] >> That's totally fair. I think you can close that get started one.
[21:50] >> There we go. All right. >> If you click on the document icon at the top-left of your window,
[21:57] you can toggle it open and closed, which is nice. >> That was exciting.
[22:02] >> Great. We've got our console log ready. Let's run this on our computer.
[22:07] We'll hop back to the terminal. Now, yeah, exactly.
[22:12] Back in our terminal, we've got access. When we installed Node.js,
[22:16] we installed a couple of things on our machine, one of which being NPM,
[22:21] which I believe you used last week. NPM start, NPM other things,
[22:27] NPM install, you might recall. Maybe it was Yarn. Sorry.
[22:31] You installed amongst other problems. >> Yeah, we did Yarn.
[22:34] >> My bad. NPM, short for Node Package Manager,
[22:39] is a program very similar to Yarn in usage. Y'all should both start using PMPM though.
[22:47] We'll stick to NPM for now. NPM is a program that gets installed with Node.js.
[22:55] But another program that gets installed is Node. If you type in Node,
[23:01] try hitting "Enter". Let's see what happens. Now, we're inside Node itself. All good?
[23:12] >> Yeah. I was just hitting random things because I'm not used to my bike being here.
[23:16] >> I'm totally with you. Now, you can see it says, "Welcome to Node.js version 16.
[23:22] Type .help for more information." Right now, our terminal is running Node.
[23:27] No idea how this works. We're actually going to just exit out. Type in "exit" and give it some brackets.
[23:36] Sorry, type in "exit" and give it some brackets, some smooth brackets without the space.
[23:42] >> Oh, wait. This one, right? >> No. Sorry, the round brackets.
[23:48] >> I'm going to learn the difference to all of these. It's going to happen.
[23:52] >> Give it the other one. Now, hit "Enter". Do you know what? Press "Control D" on your keyboard.
[24:05] There we go. That'll kill the Node execution. We've got Node installed, which is fantastic.
[24:12] We can type in "node". We're just going to remember, is that JavaScript runtime?
[24:17] Give it a space. Now, we're going to give it the name of our file to run.
[24:22] We're going to say, "Hey, Node run" and now put in "app.js". Before you hit "Enter", let's hit it.
[24:30] >> I got excited. >> You're good. But check it out.
[24:34] You can see it printed out. You ran it and then it printed out,
[24:38] "Hello, beautiful humans." >> Yay.
[24:41] >> What does that mean? That means we have run "app.js" locally on our computer using Node.
[24:48] >> Got it. >> If we were to put this into a browser,
[24:52] we're not going to do that today. But if we were to put this exact file,
[24:54] "app.js" in a browser and run it there, it'll print it into the browser console.
[25:00] >> Okay. >> Because a lot of what Node and browser JavaScript do is,
[25:06] is it fair to say, mostly similar? They share a lot of things that they can do, the JavaScript.
[25:12] >> Okay. >> That said, we spent a lot of time on this.
[25:18] Let's actually start making some back-end code. First thing we're going to do is we're going to
[25:24] create an NPM project. To do that, we're going to use
[25:33] that other program that I mentioned that comes installed with Node.js, which is called NPM.
[25:37] If you type in NPM, give it a space,
[25:43] and now we're going to initialize our NPM project. We're going to type in "init".
[25:52] With this, once we hit "Enter", it's going to start asking us some questions
[25:56] to set up our project. Go ahead and press "Enter", we're going to see.
[26:01] Let's read it out. I like reading out the stuff. This utility will walk you through
[26:05] creating a package.json file. It only covers the most common items
[26:09] and tries to guess sensible defaults. See NPM help in it for
[26:13] definitive documentation on these fields and exactly what they do.
[26:16] We don't need that right now. Use NPM install and then the name of
[26:20] a package afterwards to install a package and save it as
[26:23] a dependency in the package.json file. That's a lot of stuff we just saw.
[26:28] Now it's asking us some questions. What would we like to call our package?
[26:35] Package in this context is referring to the project itself.
[26:39] Let's talk a little bit about that, shall we? My usual go-to back-end example,
[26:48] app example is something I like to call Kind Words, which is a little app that I use to
[26:56] save little quotes of nice things people have told me, so that when I'm feeling down,
[27:01] I can go back to it and have a look and have a nice little serotonin boost.
[27:05] We can do something similar to that or we can- >> I like that.
[27:09] >> Yeah? >> Yeah.
[27:11] >> Well then, let's call our package name Kind-Words. >> Okay. It's going to be NPM.
[27:21] >> No, no, no, sorry. >> No?
[27:23] >> No, no, no, sorry. See here, it's prompting us for a package name.
[27:27] We can just type in the package name. Right now, NPM is still running.
[27:34] I usually go with hyphenation. Instead of the capital W,
[27:41] give it a nice hyphen. Yeah.
[27:45] >> Enter, so it creates that package. >> Yeah.
[27:48] >> Yay. >> Now, it's asking us, "Hey,
[27:50] what version do you want it to be?" Now, the default is,
[27:54] you see the brackets there, 1.0.0. The convention is to have 1.0.0 be like the final released version.
[28:06] I would actually recommend that we go with 0.0.1. This will be like our beta or alpha in development mode.
[28:18] We can give our package a description. Actually, let's write it. What is it?
[28:28] REST API for Kind-Words. >> Is REST capitalized?
[28:37] >> REST is all caps. >> I was like, "I haven't typed this in a while."
[28:41] >> Okay. What did you say? REST API Kind-Words?
[28:46] >> REST API Kind-Words. Perfect. As AJC Web Dev says,
[28:51] "That would be a patch version technically semver file." It would? Is that a bad thing?
[28:57] Sorry, I'm super curious. You're good, Jen. You can keep going.
[29:02] >> I'm just grateful that all of you keep joining each other's. When I am going through them,
[29:09] you're like, "No, you don't learn that." Yes, you did. Okay, we'll find out.
[29:13] We'll figure it out. >> Yeah, we'll figure it out.
[29:15] Entrypointapp.js. You see it in brackets is making, "Hey, this is the default I'm proposing,
[29:24] but you can change it if you want." Yeah. Let's press "Enter" on that and leave it as is.
[29:33] >> All right. Thank you, Joe. >> Thanks, Joe. Have a good one.
[29:38] >> We got a reply from AJC. >> Right, major.minor.patch. Exactly.
[29:47] When you make backwards compat, oh, you're right. This should be 0.1.0 technically.
[29:56] Anyway, we can fix that. Let's leave that test command blank. >> Okay. Just hit "Enter"?
[30:05] >> Yeah. >> Groovy.
[30:07] >> Git repository, we'll leave blank for now as well. >> Sweet. Tomorrow is going to be all about Gits. I'm excited.
[30:14] >> Yeah. That's why I planned this so that it progressed naturally into that. >> Wow.
[30:21] >> Nice. Keywords, let's leave that blank as well. Author. Well, now, we need to put in your name.
[30:31] I think you can put in your, yeah, I like that. Perfect. License.
[30:41] Do we want to talk about software licenses? >> Is software licenses like either you could buy a Word from Microsoft?
[30:53] It used to be where you could buy it as a one-time software that you purchased, but most softwares now are software as a service,
[31:00] which means you pay a monthly service fee. Is that what it is or what is?
[31:06] >> I think that covers part of it. When it comes to open-source development, however,
[31:12] a software license also tells you how you can use that code. When you download a project from GitHub,
[31:20] it gives you access to that code. But this license is a piece of text,
[31:27] a piece of most of the time legal text that tells you like, okay, you have the code,
[31:32] here's what you're allowed to do with the code. Does that make sense?
[31:37] >> It does. But if you don't upload it to this same repository,
[31:46] will they really know that you didn't follow those license guidelines? >> That's a good question.
[31:53] >> What would happen? >> That's where a lot of arguments come from, actually.
[32:01] I'm not going to get too much into the nitty-gritty because a lot of it comes from things that I'm not very knowledgeable on.
[32:08] But, and I'm going to sound really naive when I say this and probably mis-sell it, but a lot of the times it's kind of an honor system.
[32:16] I hope that's not too controversial to say. So, you know, there are mechanisms for checking that people are complying with these licenses
[32:24] when they go like, hey, you're using my code, and you should be giving me, what is it called?
[32:34] Attribution? Is that the correct term?
[32:39] >> Okay. So just based on what you're saying and what AJC is saying, it sounds like it's kind of like when somebody else uses a logo or something,
[32:55] where they either will send a cease or assist or give us some money for using our stuff. >> Yeah, yeah, absolutely.
[33:05] And as AJC correctly says, the best default is MIT. So they're under license where it says ISC.
[33:14] The default is currently ISC. Let's change that to be MIT.
[33:19] >> What is MIT? Oh, I'm breaking stuff.
[33:23] >> You're good. >> What is MIT mean instead?
[33:27] >> I think it comes from Massachusetts Institute of Technology. It's a license that was created there that as AJC correctly says, it makes you not liable.
[33:41] So let's see. This little form we just filled out,
[33:48] I'm about to write to this file called package.json, where it says amongst other things,
[33:55] the name is kind words, version is 0.0.1, description is this, main is that,
[34:01] scripts, we're going to get to scripts in a bit, author TeachGenTech, and the license is MIT.
[34:06] Is this okay? I'm going to say yes. I know we want to change that version,
[34:09] so we'll get to that in just a sec. >> If I just hit enter though,
[34:14] because it already says yes in there, will it default to that?
[34:20] >> It should. It looks like it.
[34:25] And we can find out. Remember how I said we can toggle that file folder thing?
[34:30] >> Yes. >> In VS Code?
[34:33] >> Yes. >> Should I go and toggle it?
[34:35] >> And, hey. >> Now we've got a file in here called package.json.
[34:41] And let's take a second to take a closer look at it. So let's toggle that away.
[34:46] So let's see. This is a piece of JSON.
[34:49] Are we familiar with JSON? JavaScript Object Notation?
[34:52] >> I'm familiar with it from hearing it happen that in YAML when I worked at Stoplight,
[35:02] knowing what they mean, not so much. I just know they exist.
[35:05] >> Right. This is a way of storing data in the JavaScript Object Notation
[35:11] that we can then-- that, for example, Node.js will read this file
[35:15] and do its magic with it. This is a standardized convention
[35:22] of how to lay out JavaScript projects. >> Okay.
[35:27] >> Cool? >> Yes.
[35:29] >> And there you can see all of the things that we filled out, right? Name, version, description, main, scripts, author, and license.
[35:38] >> I'm clicking the debug thing. Oh, I clicked it.
[35:42] And now it did a lot. >> It did some stuff.
[35:46] Let's-- yeah, let's go-- there you go. Nice.
[35:53] We don't need that terminal right now. >> My closest.
[35:55] >> I think you can hide it. Or you can-- oh, you see that trash can icon on the right?
[35:59] >> Ah, yay. Okay, so don't click the debug.
[36:03] >> Yeah, not yet. Not for now.
[36:07] And as AJC correctly says, on the left, let's call it a column. You see, we have like string, colon, string, or string, colon, string,
[36:17] comma, string, colon, colon, string, and so on and so forth for each line? >> Yes.
[36:23] >> Right. The left-hand side is what's called a key.
[36:26] That is, we're setting, for example, the name to be. And then on the right-hand side of the colon, we've got the value.
[36:33] >> What is the difference between a key and a const or a variable or-- >> Ooh, I think-- I think the way I would say it is that-- yeah, as AJC correctly says,
[36:58] key is kind of like a-- is like a variable. Yeah.
[37:01] It's a different data structure. >> So it's just called something different because it's in JSON,
[37:09] or it's called something different because-- like, what do you mean by different data structure? >> I think because it's in JSON, because it's a JavaScript object,
[37:18] it's setting that-- it's having that different name. >> Got it.
[37:25] Okay. Thank you.
[37:26] >> It's a different way of going about structuring and handling that data. So we've got that.
[37:33] So now we've got this package.json file. And I kind of want to keep that open while we do-- while we do some stuff around it.
[37:42] So you remember I said we can install packages with npm? Remember it said-- yeah.
[37:48] Let's install Express.js. So let's type in npm, and then space install, space.
[38:00] And now we're going to type in the name of our package without the bigger than and smaller than. We're going to type in Express.
[38:07] Perfect. >> And then the name?
[38:12] >> Nope. We're good.
[38:14] So we'll press enter. Now it's going to be installing some stuff.
[38:21] So let's see. Added 57 packages and audited 58 packages in two seconds.
[38:28] I like reading this stuff. Seven packages are looking for funding.
[38:32] Found zero vulnerabilities. Always good.
[38:34] But look at how our package.json file changed. I don't know if you can see the difference.
[38:40] >> Yeah, with the dependencies in Express? >> Yeah.
[38:44] So npm automatically edited our file to say, hey, this project now has a dependency.
[38:50] And this dependency is Express. And the very specific version I have installed is 4.18.1.
[38:59] Sound good? >> Yeah.
[39:05] >> Like, you got to stop me and ask questions as well, please. >> No, I found that with a lot of this stuff, it's like just like consuming it.
[39:15] Because if you keep going, it'll eventually click where like, I may not understand exactly what's going on right now.
[39:22] But after going through it all, then towards the end, it eventually clicks what I was wondering or didn't quite understand beforehand.
[39:33] >> Yeah, totally. I mean, we can, you know, we have time.
[39:36] We can also take a look at this concretely. In the terminal, we told npm, hey, I want to install this dependency called Express.
[39:46] It went on the internet. It looked up and downloaded those files.
[39:52] And it also edited our package.json file to say, hey, this project has a dependency. And that dependency is Express.js.
[40:01] Um, okay, so that just like, taken aback some, it means that we made the app.js, which at this point was just a basically like a text file to view to name it something.
[40:20] And then we added package.json, which like told us more about app.js. And then we said, hey, cool, we have, we want, we have the dependency, which means
[40:37] we want to use Express.js in all of this. And that's what we just installed.
[40:42] >> Yeah, I'd say that's, I'd say that's, that's a pretty good assessment of what's going on. I think, I think to rephrase it, if I may, we made a file called app.js.
[40:54] This is a JavaScript file that we ran in our terminal using Node. >> Got it.
[41:00] >> Right? Independently of that, in the same file, we declared an npm project.
[41:05] >> Okay. >> Right?
[41:09] We said, hey, this project is called kind words. It's got this version.
[41:12] It's got this description. It's got a main JavaScript file, which is called the same as that file that we created.
[41:19] And this project also depends on Express.js. In fact, I'd love to take us down a rabbit hole, another rabbit hole, if I may.
[41:31] >> Yeah. >> And take a look at what was downloaded.
[41:33] So why don't you toggle that folder view again? Because a couple things happened.
[41:39] Oh, yeah, yeah, yeah. You found Node modules.
[41:41] Have you heard of Node modules yet? >> I've heard.
[41:44] And then I'm pretty sure AJC was the one that said just ignore them. >> I don't want to, like, completely distract you.
[41:56] I'm all for ignoring it as well. But one thing I want to see -- oh, there it is.
[42:00] There it is. Check it out.
[42:02] So one of these folders here is Express. And if you take a look at that, what npm did was essentially download Express.
[42:11] Now you've got all of the source code of Express.js in this folder. All of the framework.
[42:19] It's been downloaded right here. >> Huh.
[42:23] I'm letting that one soak in. >> All good?
[42:29] >> Yeah. >> AJC's saying, no, I said never look in there.
[42:34] Don't ignore. Actively run.
[42:35] Oh, gosh. I'm sorry.
[42:36] I'm going against those wishes. >> I think it's cool to see.
[42:43] I don't want to touch it. >> And you absolutely don't have to.
[42:48] And I don't want to cause confusion. I like to poke around.
[42:53] And what you see here, by the way, are all bunches of JavaScript code that Express needs to run. >> Oh, wow.
[43:03] Okay. >> Yeah.
[43:05] >> Okay. >> So we can clerk that and never look at it again.
[43:10] Absolutely right. >> So just to maybe solidify this in my head a bit.
[43:17] >> Sure. >> Because we installed all the nodes, it's not making us break down that code even further.
[43:26] Because it installed the nodes. Like, what would happen if it didn't have the nodes?
[43:32] Like, do we have to develop nodes or somebody has to break it down that far? >> Yeah, that's a good point.
[43:43] And I didn't cover that well. What we did was download a -- in JavaScript land, we call them packages -- a package of
[43:54] prewritten code. >> That makes sense.
[43:57] But what if we didn't have that prewritten code? >> A super valid question.
[44:00] And the answer to that is what would happen if you tried to -- I don't know. Let's say it's a tool.
[44:08] Let's use a metaphor of a tool. Let's say we tried to -- let's say with this project, we say, I don't know, I need a hammer.
[44:14] Right? And we don't have that hammer on our desk.
[44:19] I go to reach for it. What happens?
[44:20] I can't use it. It's not there.
[44:23] In the context of here, if we tried to use Express.js without having installed Express.js, our program would fail.
[44:36] And in case you're curious, we can actually make it fail by doing that. >> I might save that one for another time.
[44:43] >> Sure. >> But, like, I'll work on conceptualizing this.
[44:48] I'll work on that one. >> Totally.
[44:50] Maybe it helps if we try actually writing some Express now. >> Cool.
[44:54] >> Yeah. Why don't we go back to app.js?
[45:01] So and let's just run -- let's run our code again. Do you remember how to do it?
[45:07] >> If I don't, I can scroll up. >> You totally can.
[45:17] In fact, oh, here's a trick. If you press up on your keyboard, you can cycle through previous commands you've written.
[45:25] >> Is it this one? >> That's the one.
[45:28] >> Yay! >> Cool.
[45:30] So we've still got -- we've still got our app file that does the things. And now we're going to modify that file to turn into an Express server.
[45:44] More on that later. We're going to turn that into a backend.
[45:48] So let's hop back onto VS Code and start writing some stuff. So let's replace line 1 with declaring a const.
[46:00] And the name of this const will be Express. And its value will be what is returned by calling require.
[46:15] That's the one. It's a function, so it takes brackets.
[46:25] >> Which ones are brackets? >> Sorry.
[46:31] When I say brackets, I mean round brackets. Like not curly brackets.
[46:35] >> Okay. >> And you want to remove that space.
[46:38] It's the space between require and the brackets. >> Oh, okay.
[46:43] >> Yeah, nice. Parentheses, that's much better.
[46:48] Thank you, AJC. Yeah, parentheses.
[46:53] So require, and then we're going to give it a string. Which is denoted by quote marks.
[47:00] And now we're going to give it the name of the package that we want to require. So right now you've given the package name kind words,
[47:16] which is the one we're developing right now. >> Oh, so it's the Express one?
[47:20] >> Exactly. So what are we doing here?
[47:23] We're just telling app.js, hey, take all of the Express framework, all of the package. Sorry, I sometimes use these terms interchangeably.
[47:35] Take all of this package and make it accessible to me via this variable express. >> Got it.
[47:42] >> So if we were to save and run this, exactly, as AJC very correctly says,
[47:50] you have it in your project, but it's not in the app.js file. So we ran our app.js and...
[47:58] >> It didn't do anything. >> Well, exactly.
[48:04] So it didn't do anything because all we did was, hey, just import this package. We didn't actually do anything with it.
[48:12] >> Okay. >> So what we're going to do next is create a new variable called app,
[48:20] where we're going to put in our Express. We're going to start up a new Express app.
[48:24] >> Okay. Quick question.
[48:28] Why don't we have the squiggly line before this and how many spaces... >> Sorry.
[48:38] >> This one. This one.
[48:43] >> Oh. >> Like, well, let's see if I do it down here.
[48:49] It, like, creates it. Is it because it's a const?
[48:52] So it's out of it? Or...
[48:54] >> I'm not sure I understand the question. Sorry.
[48:58] Have you seen that sometimes we need those brackets? >> I've seen them.
[49:06] It doesn't mean I... Because a lot of it is also going from the LinkedIn learning that I was learning.
[49:16] But it was just very difficult to understand when we would or wouldn't use them. So I will ask that another time.
[49:26] Okay. And then for the next one, for the variable, do I do it as no spaces between it?
[49:32] What is proper, like, clean coding, I think is the term that I've heard. >> Yeah, I think.
[49:40] Yeah. And there are programs that will clean that up automatically for you.
[49:44] >> Okay. >> Which is kind of nice.
[49:45] But what we want to do is when we're declaring a variable, for example, we'll do const space, name of variable, space, equals, space, and then an expression.
[50:01] So we'll have, for example, const. And we're going to want to call this one app.
[50:05] And then the equals is going to be just calling express function. That is express with parentheses.
[50:18] >> They express in the parentheses or just parentheses? >> Express with parentheses.
[50:27] After them. After the express.
[50:31] Sorry. >> Okay.
[50:31] You're good. >> There you go.
[50:37] Cool. So, oh, check it out.
[50:38] Check it out. Wait, wait, wait.
[50:39] Go back. How did you do that?
[50:40] That was so cool. We had that little popover.
[50:43] >> Here we go. >> Yeah, let's read that.
[50:45] So creates an express application. The express function is a top level function exported by the express module.
[50:52] So it creates an express application, and that application gets stored in the variable app. Good so far?
[51:03] >> Yes. >> Awesome.
[51:06] That's the types. Awesome.
[51:10] So let's create a new line afterwards. And we're going to use -- we're going to have our app listen.
[51:24] So if we call app, let's write it out first, and then we'll cover what it does. App.listen.
[51:31] Then we'll open up some parentheses. >> Next to it or space first?
[51:41] >> Always next. >> Okay.
[51:43] >> So this -- and check it out. See?
[51:48] We've got a callback. So listen -- we'll pass in two -- I'm mixing the term up now.
[51:55] Arguments. Yes.
[51:57] Two arguments. The first one is the port number.
[52:01] So the port number is -- and you've probably seen this before where you do -- where you start up -- like the React app last week, where you had like local host colon and then a number.
[52:11] >> Yeah. >> We're going to define that number here.
[52:14] >> Oh, yay. Okay.
[52:17] As long as it's bigger -- let's say as long as it's bigger than 3,000, feel free to pick one.
[52:21] And keep it to four digits. Very nice.
[52:27] Three, three, three. >> We'll do a four.
[52:30] So just that way, you know, I feel like three, three, three is probably used. >> Sure.
[52:35] We can do that. So that's our first argument.
[52:39] Second argument is denoted by a comma. Sorry.
[52:44] That's still inside the parentheses. >> Oh.
[52:48] >> Perfect. And now we'll define what's called a function.
[52:57] A callback function. Have you -- wait, wait.
[53:03] We're not typing callback, though. Sorry.
[53:05] >> Okay. Just kidding.
[53:06] >> Have you done functions before? >> Uh-huh.
[53:12] Yeah. I think so.
[53:14] I'm vaguely pretty sure I have. >> Okay.
[53:18] Have you done them with the keyword function or what's called an arrow function? >> Keyword function.
[53:24] >> Let's go with that, then. So let's type in function.
[53:28] Then get some parentheses. And actually, we'll skip the -- so we'll go outside of that first parentheses.
[53:46] Yeah. And put in a space.
[53:52] And now we're going to write the inside of that function, which is done with curly brackets. So great.
[54:02] You've got some curlies there. And now hit enter.
[54:07] So now we're typing in that function. So how about we say -- let's do a console log.
[54:16] And we're going to console out saying -- now, this is going to be what the user -- well, what the developer will see once they've started up their app.
[54:32] So let's say "listening to port 3334." Don't forget, it's a string, so it needs quote marks.
[54:42] Cool. >> And really quick, a string, is that just saying because it's, like, text?
[55:02] That you see? >> So I -- it's a story that's related, I promise.
[55:08] When I was -- so I studied in university here in Austria. And the German word for a string is "Zeichenkette," which translates directly -- I know.
[55:18] Which translates directly to English as "character chain." Right?
[55:28] Because a piece of text, in this context, is a string of characters. >> Right.
[55:35] >> Like, everything between the quote marks is just text to be used as is. It's never to be interpreted as code.
[55:47] >> Okay. >> It's just like -- yeah?
[55:49] Does that make sense? >> Yeah.
[55:51] Yeah. That -- yes.
[55:52] Okay. Exactly.
[55:54] So that's what I suspect the etymology is. And I know German gets bad rap for having, you know, complicated words.
[56:02] But I got to give credit to it. "Zeichenkette" is -- I mean, it's long, but it's descriptive.
[56:08] I like it. Anyway, so yes.
[56:12] So we're printing out the string, listening to port 3334. >> Okay.
[56:18] >> So what we've done here in line 3 is we're telling our Express app, hey, just listen on this port.
[56:27] That is, just always be running -- waiting for this port to get a connection. And once it's started up, call this function.
[56:37] So once the app is ready to start listening, it'll call this function. Hey, console log, listening to port 3334.
[56:48] >> Okay. >> Let's hop on the terminal and run this and see what's going on.
[56:56] Ooh. AGC says -- and it's just arbitrary versus, like, numbers, which computer know our numbers
[57:03] and can do math with those. That makes sense.
[57:06] Okay. Cool.
[57:08] So you've run node app.js, and you can see listening to port 3334, but also you can't enter any commands right now.
[57:17] >> Because it's still listening. >> Yes.
[57:21] >> So I would have to do the control C? >> Correct.
[57:27] So what's going on here? Our app is running, and it's essentially turned itself into a server.
[57:37] And when you think of servers, you think of, like, big room full of computers that are, like, you know, super tall and wall-to-wall.
[57:46] But really, I like to think of a server as a program that runs on your computer, and all it does is wait for what are called requests, right?
[57:56] And you probably remember this from your rest -- from your API meetups, right? Where a server is just -- it just sits there and patiently waits.
[58:07] >> Yeah. >> It just waits to get together -- to get some kind of request.
[58:12] Usually, these are done as HTTP requests. You've probably heard of those.
[58:18] >> Yes. And that is something that I one day totally want to go into our protocols, because I get
[58:27] that so mixed up with my time at GoDaddy of -- >> Yeah.
[58:32] >> It's very confusing. >> Yeah.
[58:36] No, and I mean, it's a lot. So, yeah, this server is currently running and waiting for requests.
[58:45] >> Okay. >> But actually, I don't know what's going to happen.
[58:49] Let's do something. Let's run the program again.
[58:52] >> Okay. I'm writing notes, too.
[58:56] >> Oh, yeah. So now we've got a backend running.
[59:00] This is when you put your Express app on a server -- sorry, when you put your Express app into what's called production, that it's live to the public.
[59:09] It is essentially doing this. It's just running and being like, all right, like twiddling its thumbs, waiting.
[59:15] >> Right. >> So now we can actually -- we've got a server running.
[59:21] We can actually interact with it. Let's go to the browser.
[59:24] >> Should I go live from VS Code or just a regular browser? >> No, I meant a browser, yeah.
[59:33] >> Okay. >> Exactly.
[59:36] So you remember from the last stream, you know, you could access a server running locally on your computer with localhost, colon, the port number.
[59:46] We can do the same here. >> Oh, can we just, like, notice that part of my past Googles have been time in Austria?
[59:54] >> Yeah. >> Because it's -- I always have to Google what time zone everybody's in.
[60:01] All right. >> Yeah, time zone's all right.
[60:02] >> Localhost, and it's going to be 334. >> Cool.
[60:10] Now we've got an error. Cannot get forward slash.
[60:16] That's because our server is listening, but it doesn't know how to respond yet. >> Okay.
[60:24] >> Does that make sense? >> Yes.
[60:27] >> So what we're going to do next is tell it how to respond. But let's try something else just yet.
[60:34] Let's turn off our server. Let's turn it off by control C, and let's go and refresh our browser and see what we see instead.
[60:42] "Localhost refused to connect." AGC says, "Did you try turning it off and on again?"
[60:49] We're going to be doing that shortly. Cool.
[60:53] So, yeah, exactly. So this site can't be reached.
[60:56] Localhost refused to connect. There's no server running.
[60:59] >> Right. Because it's not listening to anything.
[61:04] >> Exactly. >> Okay.
[61:06] >> So what we're going to do next is tell it, "Hey, when you get a request at this path, this is how you'll respond."
[61:15] So let's do that. Let's create a new line between lines two and three.
[61:21] And we're going to define what's called a route, right? So we'll go app, and we're going to define what's called a route.
[61:34] So we'll go app.get. And it'll take two parameters.
[61:45] Yes, parameters. So when we say it takes parameters, first, we put in our parentheses.
[61:53] >> And then our string. >> It is a string, yeah.
[62:01] And the string is going to be the location where we'll be connecting to, the route. And, like, I don't know if you know, when you connect to a server and you just go localhost
[62:13] 3334, for example, it connects to what's called the root route. And that root is denoted to a computer as a forward slash.
[62:22] So if you put in a forward slash here, we're saying, "Hey, when somebody connects to this app with the forward slash, that'll be the root route."
[62:40] Sound good? >> Yes.
[62:44] >> You can also think of it as, like, a website. Yes?
[62:48] >> I'm kind of thinking of it, like, just as, like, a GoDaddy comparison is, on, like, cPanel was the backslash was always the root folder.
[63:00] >> Right. >> So I'm trying to pair it like that.
[63:06] >> Cool. Yeah, so when we go to localhost 3000, then we're going to tell it, "All right,
[63:11] when that happens, our second parameter after the string is going to be how we respond." And that's going to be a callback as well.
[63:18] So after the string, let's put in a comma. >> Oh, okay.
[63:23] >> After the string, not after the parenthesis. >> Oh.
[63:28] >> You're good. So after the string, let's put in a space.
[63:32] And we're going to define the-- >> Space comma or comma space?
[63:37] Okay, cool. >> Comma space, yeah.
[63:39] We're going to define a callback, right, which is a function that gets called automatically when the server gets hit with this route.
[63:48] And it'll be just like in line five. So we'll define a callback function.
[63:55] >> So is it app-- it wouldn't have app.listen, it'll just be a function, right? >> Yeah, it'll be function, exactly.
[64:04] And so one tiny difference-- well, one difference here is that this function actually does take arguments.
[64:17] By the way, I think in-- the function is missing the first n. >> Oh.
[64:25] That would help. Thanks.
[64:31] >> Cool. >> This is-- I am very, very grateful that I'm starting to hear that there are more dyslexic
[64:37] coders that I ever thought was out there because this has been a big reason I've never wanted to get into it because I'm like, "I miss entire words at times."
[64:48] >> And a lot of program interpreters do-- could do a better job at explaining those errors.
[64:59] You know what I mean? >> Yeah.
[65:01] >> Like, there's a programming language called Rust that I find does a pretty good job of being like, "Hey, you typed in this.
[65:06] Did you mean that?" And I very much appreciate that.
[65:11] Because it's not just-- it's also for folks who are-- for whom English is not their first language.
[65:16] >> Yeah. >> Like, that becomes a-- you know, like, the amount of time that I have lost to trying
[65:23] to tell CSS that, "I'm sorry. I meant color without the U in it."
[65:28] Yeah. A lot of time spent on that.
[65:32] >> And AJC, I will eventually listen to your podcast. I think between doing, like, these Teach Gen Tech Lives, and now I'm going to be doing
[65:42] them every day on-- like, just even doing my homework, same time, almost every day, that I'm like, "I don't know if I can consume more knowledge of it."
[65:57] Because it's, like, so hard and exciting. >> That's awesome.
[66:04] Oh, do please-- what's a podcast called? I'd love to-- maybe we can, like, put the URL here or something.
[66:11] >> Yes! >> But while we do that, yeah.
[66:15] So, our function now takes two arguments, right? So, the first one is called-- what is the first one called?
[66:28] Oh, nice, we have it. FSjam.org.
[66:32] Full stack Jamstack. Cool, thank you.
[66:35] I gotta take that. >> I'm going to leave that there for a few.
[66:38] >> Yeah, that's awesome. Yeah, so this one takes two arguments.
[66:44] The first one is called "request." We can give it any name we want.
[66:48] We're going to call it "request." And the second one, with a comma-- so, comma space, is going to be "response."
[66:58] So, you see, after that, we've got two closing parentheses? Between them, let's put in our curly brackets.
[67:05] >> Oh, another opening curly bracket? >> That's right.
[67:14] >> Right, okay. >> Give it an enter, so we can get some space to write some code.
[67:17] Cool. So, let's-- so, this function here is called "request."
[67:25] So, this function here is going to be called when we try to access the forward slash, which you remember is the root route.
[67:36] So, it's actually going to get called when you take your browser to localhost 334. >> Okay.
[67:43] >> Sound good so far? >> Yes.
[67:46] >> So, let's actually respond. And what we can do is take that response argument.
[67:55] So, into line four, we can type in "response dot." And we're going to call the function "send."
[68:05] And in parentheses, we're going to send in whatever data we want to send back. Because a server receives a request and responds with a response, right?
[68:22] >> Can we put a string here? >> Let's put a string.
[68:25] >> I need to learn how to type on this keyboard. I'm also not used to using an external keyboard.
[68:35] I'm always on my-- >> Oh, on the laptop.
[68:37] >> Yeah. And I'm like, "I need to get used to this."
[68:40] Okay. >> Perfect.
[68:50] So, let's save. And let's run our server again.
[68:55] So, you can see, listening to port 3334. So, if we come back to our browser and access that, let's see what happens.
[69:06] >> Yay! >> So, what happened?
[69:10] The server said, "Hey, I got this request at the root route. And I will respond with this text, which is BRB someday."
[69:18] So, then the browser says, "Hey, I got this text." When I get text, I usually just render it as is in the browser.
[69:26] >> Okay. >> Let's try something.
[69:29] Let's change "someday" to "tomorrow." Save that.
[69:45] And let's refresh our browser. Now, you'll notice it still says "BRB someday."
[69:53] That's because we did change our server, but the code that's being run is the old one. >> So, I have to close the server, restart the server.
[70:08] Okay. >> So, let's try something else real quick.
[70:15] Before we start it up again. Since we're just sending text, what happens if we make that response into some HTML?
[70:22] >> I was actually going to ask that if we could, like, add a header so it actually looks bigger. >> We totally can.
[70:30] So, do you know how to do that offhand? >> I can tell you that Yere first showed me how to do that kind of thing in, like, lesson day one.
[70:42] >> Nice. >> It exists, I don't remember how.
[70:45] >> Totally cool. I mean, that's how we learn.
[70:49] So, before the BRB, inside the string, before the BRB, we'll open a less than HTML tag. >> Oh, it's that easy?
[71:03] >> No, no, hold on. >> Because AJC is cheating.
[71:05] >> Sorry, just a sec. It's after the quote mark.
[71:10] >> Oh, okay. Because the HTML needs to be part of that content we're responding with.
[71:15] So, H1, yep. And then after tomorrow, forward slash H1.
[71:26] And that's it. Save that and run it.
[71:34] >> Yay. >> Not bad.
[71:44] Not bad at all. >> And then if I wanted, so, just as a refresher from my first lesson,
[71:50] if we want to change color or anything, that you have to do in CSS. >> Which, yes.
[71:59] >> Which you can technically write what's called inline. >> Let's not do that right now.
[72:06] I just wanted to double check that that was a possibility. Cool, yay.
[72:14] >> Yeah, no, you can totally, and honestly, what we've just done now is how, and I'm going to sound really, very likely wrong,
[72:24] but a vast majority of what browsers interact with servers do is this. What we've just done.
[72:30] When you go to, say, Twitter.com, they've got their own little, maybe it's not Express, I think it's Go.
[72:38] I could be wrong. They've got their own little server that's like, oh, somebody's like,
[72:42] like getting a whole bunch of, like they gather up a whole bunch of data, and they respond with some HTML, which we just did, some CSS, and some JavaScript.
[72:54] It responds to the browser, and the browser's like, I gotcha, and then it renders it accordingly.
[72:58] >> Okay. >> This is a big, big, big part of how the internet works.
[73:05] Mind you, mind you, this is, you might be thinking, well, this is fairly rudimentary, and I thought we were building an API.
[73:14] Let's do something a little more sophisticated now, okay? >> Okay.
[73:22] >> Now, I don't think we have time to start interacting with a database per se. Do we want to talk about what databases are?
[73:30] >> Yeah, let's just mention what a database is. I can, from what I remember at GoDaddy,
[73:38] and I would love for you to break it down from there. But in my head, a database is kind of like just Excel on steroids,
[73:50] where it's a bunch of tables that get, yes, that thing, if you break, you'll get fired. I totally see that.
[73:59] But it's basically where it's a table where if you take a look at, let's say, X will equal whatever the input for line four is, the column.
[74:17] I don't know if that actually made any sense out loud, but it did in my head.
[74:20] >> Mm-hmm. No, I think that's a good part of what a database is.
[74:28] I would say it's a program that stores data. It's got two functions.
[74:35] >> In rows and columns. Okay.
[74:37] >> Yeah. The pedant in me, it's going to say it's not always rows and columns,
[74:46] but most of the time it's rows and columns. >> What is, so just to get clarification here,
[74:52] so I can conceptualize what a database is, yet what is MySQL? Because that comes up a lot as well.
[75:03] >> MySQL is a type of database that stores data in tables. As AJC says, it's relational because tables can be related to one another.
[75:16] A user will have, let's say we have a user table, which will be made up of rows, one row per user, and columns, different types of data for that user.
[75:27] Name, last name, address, date of birth, email address, password, stored, encrypted, of course. >> Yeah.
[75:37] >> That sort of thing. An order will be a different table, right?
[75:40] Will be like, I don't know, product, date of purchase. >> So just to get a visual on it, for those that are visual, so it would be like,
[75:51] promo, and it could be like, job title. >> Yeah, totally.
[76:02] >> Address, and that's like a basic database, right? And then MySQL will just be able to find it if there's different sheets,
[76:18] because we may not want to do job title on the sheet, because there's different layers within job title.
[76:28] Or like, job title would be its own different sheet. Yeah, okay.
[76:32] >> Exactly. So MySQL is a program that stores these tables in its own way.
[76:39] >> Okay. >> So it wouldn't really interact with, wouldn't really interact with Excel.
[76:47] SQL is, MySQL, pardon me, is Excel in a way. >> Yeah.
[76:54] I was just using this as an example to view it. >> I think that's great.
[76:58] >> Okay. >> So usually your backend will interact, if you're storing data,
[77:05] you will interact with a database. But because we are lazy developers, and we're short on time, we will store our data,
[77:16] what's the word? As long as our program is running.
[77:22] >> Okay. >> Yeah?
[77:25] >> Yeah. >> So this is for the sake of exercise.
[77:31] It's not, let's say, the best way to temporarily, what's the opposite of temporarily? >> I would say we could always pause it and come back to this point.
[77:43] >> Totally. >> Because I feel like we've covered quite a bit today.
[77:48] >> Sure. >> And I know my homework later this week is going to be just getting to this point again.
[77:56] >> Yeah. >> And I personally would love to have you on the show again.
[78:00] And then we could just pick up for databases. >> Yeah, totally, totally.
[78:06] So then I apologize that we didn't get to do the rest part of the API, the rest of the REST API. >> It's a lot to break down.
[78:16] I think this is a really, really, this is the cool thing about breaking down tech to newbies, is you start to find out how many layers it is to doing this one thing to be able to understand it.
[78:29] >> Totally, totally. Yeah, we can come back to it.
[78:34] >> And yes, AJC, I do want to copy and paste, but I'm trying to learn it to what things actually do.
[78:43] So I'm like, I don't want to do that yet. I will say, though, something that I really, really want to thank you for, Ramon,
[78:49] is you were saying the word on what we were going through. So that way, I was learning what it does a lot better.
[79:00] So you would say, hey, we're going to do a function. So I would have to try to remember what a function is and then how to type it out.
[79:10] >> I'm a big fan of learning by doing. >> So I really, really appreciated it.
[79:17] I mean, I'm down if you have more time to do databases, but I know it's getting late there. So I don't want to, like, force you to do anything.
[79:25] >> We can, you know, I think getting our hello world that we've done just now, our hello world of backend, is a good stopping point.
[79:35] Also, like, because if we were to continue now, we might have to, like, stop at a, let's say, less convenient point.
[79:40] So if you'll have me, I'd love to come back. >> Okay.
[79:50] Well, I just said that you'll be back sometime in the next month. >> Works for me.
[79:54] Solidified on stream. Now I can't take it back.
[79:57] No, that sounds great. >> All right.
[79:59] Let's see if I got this refreshing with -- yay! >> Wonderful, because there's one last part to what we've just done that I wanted to cover
[80:11] with you that I didn't really get to, and that is on line three, we said app.get. >> Okay.
[80:16] >> And this is what's called an HTTP method. I think there's five of them.
[80:25] There's get. There's post.
[80:30] There's put. There's patch.
[80:32] And there's delete. >> Where does the -- I feel like I've also heard of pull.
[80:39] >> I think get -- with get you pull. >> Okay.
[80:44] Got it. >> Yeah.
[80:46] AJC says those are the most common ones. See, there's more than that.
[80:50] But, yeah, so -- and express lets you define how to respond not just to the path, to the route, but also to the method.
[81:01] Right? >> I was giving a funny face to what AJC said, because I'm like there's more.
[81:06] There's more. >> Oh, yeah.
[81:07] >> There's always going to be more. >> There is more options, Ned, I think are related to cross-origin something, something.
[81:15] Cores. >> Yes, the Mozilla.
[81:20] Let's see if I can actually copy. >> Oh, MDN.
[81:22] It's a great resource. >> Okay.
[81:27] >> But, yeah, so there's more. But the ones that you'll be interacting with the most are get, put, patch, get, put, patch,
[81:36] post, and delete. >> Okay.
[81:38] >> And these are a standard that web apps conform to. So what a browser does when you say go to localhost 3000, it's actually saying, hey,
[81:50] I want the forward slash. I want the forward slash, but it's also saying I'm doing a get request for the forward slash.
[82:01] >> Wait, what? Could you repeat that one more time?
[82:06] >> Sure, sure, sure. When you go to a website, your browser sends a get request to the server.
[82:12] >> Okay. >> And so we've defined how our server will respond to a get request in this route.
[82:20] >> Right. >> But when, for example, you're in a browser and you submit a form,
[82:26] that sometimes takes you to another website, sometimes doesn't. You've seen that, right?
[82:34] Like when you post a tweet, you don't go to a new website. You just --
[82:37] >> Right. >> It just shows up.
[82:38] >> Right. >> This is called a post request.
[82:42] >> Okay. >> So we're sending that request to the -- so it's kind of weird because you're sending --
[82:50] you're posting a request. That terminology always mixes me up.
[82:54] >> Yeah, that's why I'm kind of like giving you a funny face. I'm like, wait.
[82:57] >> Yeah, no, you're good because it's confusing. Yeah, so you're sending a post request.
[83:04] >> Okay. >> When you're editing a tweet, for example -- I know you can't edit tweets,
[83:11] but let's go with that for now. When you're editing a tweet, you're sending a put or patch request.
[83:19] You're telling the server, hey, I want to update this. >> Okay.
[83:23] >> If you delete a tweet, then you're sending a delete request. >> All of that makes sense, other than it's going to take me a while to get used to a --
[83:40] you said a put request? Yeah, yeah.
[83:45] That's going to just -- I got to wrap my -- like, I get what you're saying, but the words, I'm like -- okay.
[83:50] >> It's weird. It's super weird.
[83:53] But all you want to know is get is for asking for data. Post is for sending data.
[83:58] >> Got it. >> And we're going to -- when we get to the database next time,
[84:03] we've defined now how to get our stuff. But then we're going to be finding out how to send data to our server.
[84:14] >> Got it. >> And as AGC correctly says, we're dealing with something called CRUD,
[84:22] which is short for create, read, update, and delete. >> Okay.
[84:31] >> It's a lot. >> Yes, it is.
[84:36] >> We'll get back to it, and we can just cover whatever we need covering next time. And this is, like, something that I really enjoy.
[84:47] And for all the beautiful humans that are watching these streams or watching them, you know, as you're going through your journey later on, sometimes just finding -- even if it's on Twitter
[85:00] or in Stack Overflow or there's so many different resources, Reddit, that you can ask these questions that -- just being able to connect the two dots.
[85:12] Like, Ramon, I asked you a question so I could compare it to GoDaddy or to an Excel sheet or something that I'm familiar with.
[85:21] So that way I can build upon or change what I've already learned. And sometimes doing that of just doing coding by yourself, that can be very difficult.
[85:32] So please comment on these. Please reach out to all of us.
[85:37] This is how we're all going to learn, is by teaching and learning together. >> Absolutely.
[85:44] Learning is modular. We build connections between the different modules of knowledge we have in our heads.
[85:50] >> Yes, yes. All right.
[85:54] Is there anything else you want to cover? >> I think this is a fantastic stopping point for now.
[86:00] >> Okay. >> Let me reverse the question and ask, is there something we covered
[86:05] that maybe you want to just cover one more time? >> Ooh, let me -- I'm actually going to use my terminal for my recap.
[86:14] I actually wrote down notes of change directory. >> Cool.
[86:23] >> I believe you can create a folder from terminal as well. You don't have to use an existing one.
[86:31] >> Yes, you can type in the command mkdir, make directory. >> Okay.
[86:36] All right. Well, I'll write that one down at some point.
[86:39] And then we looked up Node, but we didn't use that. So...
[86:44] >> We used Node to run our app.js file. >> Okay.
[86:53] Yes. I think -- okay.
[86:56] And then we used it to install the package. And we used Express.
[87:04] Okay. And then that's where we named it.
[87:09] And we confirmed it. Yeah.
[87:13] Yeah. I think I have a handle on it.
[87:16] Yet it's definitely going to be something that is going to take practice. >> You're not alone, Jen.
[87:26] Any questions you have, you know, you can always DM me. >> Thank you.
[87:31] And so... Oh, wow.
[87:36] That AJC just said, "Maybe I need to have the two of you on at the same time to do that." We'll just keep inviting the -- you both on, and Jere, because he was great as well,
[87:52] of what AJC just said. >> I'd be totally up for that.
[87:57] >> If you connect by the React front end and the API, you would have a full stack application. >> And that's where this all just comes together.
[88:08] This, by the way, is called full stack development. >> Okay.
[88:13] Well, my homework later this week is to still do my homework from last week. Because I had a horrible migraine that it just didn't happen.
[88:21] And also do this. So for all of those who want to tune in to me doing live homework,
[88:28] I'll be doing that on Wednesday, Thursday, and Friday around this time. And...
[88:34] Okay. So apparently we'll do that, AJC.
[88:39] We'll do, you know, Ramon will come on again, and then we'll have the two of you on together. We'll get there.
[88:46] We will get there. >> It's added.
[88:48] >> And thank you again. And just so that everybody knows, if you want to reach out to Ramon,
[88:56] it is Ola_Soy_Milk. It is in...
[89:03] >> I'm so bad at this. >> Yeah, I like it.
[89:06] I like it. And mine, let's see if I can do it.
[89:10] I'm like on different... There we go.
[89:12] Yay. >> Look at you.
[89:14] Look at you having much better Hyundai coordination than me. >> Other than when I was typing and using this mic.
[89:22] So thank you, everyone, for joining. Please comment on the YouTube if you have questions or on Twitter or LinkedIn,
[89:29] and we will answer them another time. Thank you all.
[89:33] Bye. 
