---
showLink: "https://www.youtube.com/watch?v=bU-zAAd5FyM"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-how-to-deploy-a-react-app-with-vite-and-vercel"
title: "Teach Jenn how to Deploy a React App with Vite and Vercel"
publishDate: "2022-07-06"
coverImage: "https://i.ytimg.com/vi/bU-zAAd5FyM/maxresdefault.jpg"
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

[00:00] Hello, Anthony, thank you for joining. I almost said my podcast.
[00:07] Yeah, is this a swear-friendly stream? I'm going to say yes because my podcast is called "Shit You Don't Want to Talk About,"
[00:15] so it's going to be very hard to transition to teach gen tech without swear words. To teach gen shit.
[00:23] Yes, yes, teach me the shit that, you know, you don't want to talk about. That's what my two shows combined are.
[00:30] Thank you for joining Teach Gen Tech. There we go.
[00:35] Gotta get used to saying that. Please introduce yourself and what you're going to teach me.
[00:39] Yeah, hello. My name is Anthony Campolo.
[00:42] I am a developer advocate at Quicknode, and I am also a member of the Redwood JS Core team, which is a JavaScript framework.
[00:50] I won't be talking about that at all because it's a little more high-level, but today I wanted to teach gen here how to deploy a React application, and we'll be using a couple tools
[01:02] to do that. We'll be using a specific build tool called Vite and a specific deployment platform called
[01:07] Vercel, and we can break down both of those and kind of explain what they are a bit from here.
[01:13] But yeah, I want to make a call out for some of my -- one of my friends is already confused about this.
[01:18] My partner gen is not this gen. This is a different gen that I met on the internet very recently, and you had reached
[01:24] out asking about how to get a DevRel job, and I love helping people get into the industry and especially helping people launch streams.
[01:33] I helped one of my friends, Ben Myers, launch a stream about a year and a half ago, and so yeah, I was super excited that you reached out, that you wanted to do this, and it's
[01:43] going to be really fun. I think this content is so valuable to beginners and to other DevRel people who want to do
[01:49] stuff like this, so yeah, and it's like you already got like -- you got like, you know, title cards, you got graphics, you got a little logo right up there, you got all sorts of
[01:59] stuff. So this is very, very cool.
[02:01] Thank you. Thank you, and the only thing I don't have figured out, just because I think it is a
[02:06] great call out, is the fact that my ring light hits my glasses, but people can't see me without it and I can't see shit if I don't wear them, so they do show up in these, and I love the
[02:18] fact that your partner's name is Jen. Like that, she must be amazing.
[02:22] She's pretty cool. Yeah.
[02:24] Her name is Jen. She would never do a text stream, though.
[02:26] Definitely not. I did set her up with a Hashnode blog, though, because she's a writer.
[02:30] I'm going to pretend like I know what that is so far. Yeah.
[02:34] It's a -- so that'll be -- next stream, I'm going to show you how to create a Hashnode blog.
[02:37] Hashnode is like a very, very cool blogging platform. If you go to ajcwebdev.com, which is my home page, you'll see a blog and that's a Hashnode
[02:45] blog, whether you realize it or not. Very cool.
[02:49] Very cool. Well, at least I know that you'll be returning, and I will say I think a lot of people are
[02:54] excited to just see the growth and like for the opportunity for me to ask them questions in like six months where they're like, "You've learned so much.
[03:03] You're not as much of a noob." Totally.
[03:05] Yeah. I mean, I'm someone who created a podcast before I had my first tech job, so I really
[03:11] saw a lot of parallels between my story and your story and what you're doing here, and for me, I was interviewing people who were so far beyond where I was and trying to ask
[03:22] the questions that I thought would help contextualize things for me, and then that ended up having a knock-on effect of creating really good content for others who were like, "I want
[03:29] to learn this stuff, but I don't know how to get into it," and when people talk about it, they're using all these terms that are just talking past me, and I can't really wrap
[03:37] my mind around it. So having a beginner ask the experts the "dumb questions," and there are no dumb questions
[03:44] here is so valuable, and it allows people who are also having those same questions the ability to sit in on those conversations and be like, "Okay, that's what I wanted to ask,
[03:53] and that's the explanation I needed for it to click for me." Yeah, and thank you for mentioning that because since ... I'm also brand new to Twitter.
[04:03] I've had a Twitter account. I think I deleted it and then restarted this one in 2020.
[04:09] I think I've sent a total since 2011-ish, maybe 10 tweets ever. I didn't understand the concept of Twitter and how to use it and how to make sense of
[04:22] it, and looking into the developer relations roles and then seeing Adam's post and thread, I was like, "Oh, this is actually starting to make sense."
[04:34] And even two weeks ago, I was asking people on the feed, on the thread, how to get in touch with them instead of just DMing them.
[04:44] So it's like brand new to Twitter too, and I see what people post and the people I'm starting to follow, and I'm like, "I got like half of that," or like-
[04:54] It could be scary. It could be scary because in one sense it can be conversations that are really complicated
[04:59] and you don't quite understand. It can also be scary because people will be very aggressive, and you'll meet some incredibly
[05:04] rude people on Twitter. And don't ever feel bad about blocking or muting someone on Twitter because many of
[05:09] them deserve it. That's a good call.
[05:11] That is a good call. If you find the people who are open to have genuine conversations and who are looking
[05:16] to help you out, Twitter is the most incredible professional network you will ever find. I think far better than LinkedIn personally, but there's some people that swear by LinkedIn.
[05:26] It's fine, but I've met so many people on Twitter and connected with so many people on Twitter, and once you kind of put yourself out there as someone being part of the conversation
[05:34] and putting out your own content, people will start to see that. And then when you do reach out to someone as like a "cold message," they'll know you
[05:42] even if you've never talked to them because there's a decent amount of people doing this, but there's not like thousands of DevRel people, I would say, in terms of a specific niche.
[05:51] We're just looking at kind of like the JavaScript front-end world, at most, there's maybe 1,000, 2,000 DevRel people who are like active, working at a company, doing it, and then if you look
[06:02] at things like DevOps and data science and like Web3, then you'll add in like thousands for each of those kind of niches, but you'll find very quickly that there's only so many
[06:13] people you need to meet to kind of meet all the DevRel people, you know, we're fairly like a small, tight-knit group.
[06:19] Sweet. I got added to a, what are they called, a list, a Twitter list, and I was so excited.
[06:27] I was like, "I made the big times, I made it, I'm on a list." Yeah, and a good list, "I'm on a list I want to be on."
[06:35] Yeah, and I was just like, "I don't even know these existed, that's cool, I'm still learning that."
[06:40] And thank you so much because I think also how you're mentioning when with Twitter, like putting out content and those type of things, I started in my journey of Twitter, the last
[06:50] two weeks, I started following Coding Therapist, and Africa is absolutely phenomenal in the fact she posts a lot about also like stretching and yoga and in, which seems like so not related
[07:06] yet at the same time, I realized even now I'm like sitting at my desk all the time that I think you're absolutely right because when you're posting that stuff, you don't even
[07:15] realize how much of an impact that may be making on others yet. Yeah, the health aspect and staying healthy while you do this is really important and
[07:25] under discussed topic for sure. I just followed her, that's super cool.
[07:30] Yeah, it's like you got to stay active and you got to make sure you're not on screen all the time.
[07:35] It's like once you get into this, you start really enjoying this kind of work, you just like sit down, just like crank out like hours and hours of work, and it's like really invigorating
[07:42] and cool stuff. And then all of a sudden, you're like, "Why does my neck hurt so much?"
[07:47] And I've noticed that with editing, I interned as a video editor for my podcast, I'm like, "Oh, I've been like seriously sitting here for like four hours, I need to get up.
[07:59] I need to move around." But thank you again for volunteering yourself too, like you were the last conversation that
[08:08] I was like, "Okay, I'm committing, I'm doing this." And we booked a date and then somebody else booked a date and I'm like, "This is like
[08:14] real. What?"
[08:16] So- - Now you can't stop it.
[08:18] - Yeah, now you can't tell it's a date. - We're going to start reaching out to you and asking to be on whether you want them
[08:21] to or not. - It's going to be cool.
[08:23] It's going to be cool. Okay.
[08:25] So, it's React app with Vite, Vite? - Vite, yes, because it's French, yes.
[08:32] So the reason why it's Vite and like, this is just fun minutiae, it's not really important is that it was from the creator of a framework called Vue, which you can kind of think of
[08:40] as like a competitor or alternative to React. And Vue is also a French word, even though they don't use the French pronunciation because
[08:49] things are never simple when it comes to naming. So Vite is a French word that means fast because it's what's called a build tool, which basically
[08:56] means that when you build a JavaScript project, like the JavaScript project you did on the coding, the code sandbox one, that was one where it was kind of like vanilla JavaScript.
[09:07] I don't think you were really using like a framework at all. And with something like React, it's kind of, it's almost like a different language from
[09:17] JavaScript. It's not entirely, but it's using something called JSX, which basically requires a compiler
[09:24] to transform it back into JavaScript. So you kind of need like a program to take your program and rewrite the program into
[09:31] something the browser actually understands. What's great though, is you don't have to know how to do that.
[09:35] Like that's what the tools do that for you. - Okay.
[09:39] - So usually you would use something like Webpack and Webpack would be the thing you would use to kind of turn your JSX into JavaScript.
[09:48] But the problem is Webpack is super slow and kind of obnoxious and Vite is basically like a faster, sweeter tool.
[09:54] So if you use kind of older React frameworks that use Webpack, you'll find that as you're doing it, you may like make a change and you'll save it.
[10:02] And then you'll look at your browser and you'll be like, wait, you'll be like 1, 1,000, 2, 1,000, 3, 1,000, and then it'll change.
[10:08] And then you'll see it, because it'll have to do that transformation. It takes time.
[10:12] Whereas with Vite, you'll save and then it changes and it's like instant. And so that's why it's more like a code sandbox in that respect, where it's like, as you're
[10:20] making changes, it's just automatically updating. And so that's what makes Vite like super duper sweet.
[10:25] There's a ton of other stuff about like the internals and how it relates to the evolution of JavaScript as a language.
[10:30] And like, that's not really into the scale, I didn't totally confuse you. - Okay.
[10:35] - But that's the important thing is that Vite is like the tool you're going to use to develop with.
[10:39] - Okay. Let's see if I can summarize this and if I got it.
[10:43] So and seeing if this all makes sense, JavaScript is front end. So it's like what the browser actually reads.
[10:52] React is a format of JavaScript, but it's more on the backend. And then you need something like Vite or the web one that you mentioned to compile it and
[11:04] move it from the React format back to JavaScript so it can be read by the browser. - That was all perfect.
[11:12] Just remove that word backend from there. So there's no backend involved here.
[11:15] This is all still stuff happening entirely on the front end. - Okay.
[11:19] - But if, yeah, so the backend stuff is like, when I teach you Redwood JS, we can talk about the backend because that's where you have like a server and a database and all that
[11:27] kind of stuff. - Okay.
[11:29] - None of that is going to be involved here. - Why would someone use React instead of vanilla?
[11:33] Like that part, I'm not quite following. - Yeah.
[11:37] You could do a whole episode on that question itself. So I would say, because it's going to give you certain conventions for doing things that
[11:47] you're going to do all the time in JavaScript and makes it a little bit easier. So when you're using JavaScript, you have things called events.
[11:56] So an event could be a click. You can have an event that says, when you click this button, I want something to happen.
[12:02] And then you will write code to make sure that the thing you want to happen when you click the button actually happens.
[12:08] Now what React does is it gives you the ability to do that with less code and with less understanding of how JavaScript and the browser actually works.
[12:18] So that's part of it is it allows you to do lots of frequently common tasks within JavaScript. And then it also gives you the ability to create components.
[12:29] And basically that just means if you want that button to be a self-contained piece of code that you can easily insert into, say, different pages or different parts of your
[12:39] application, you can contain it within something called a component. And then that component is literally just like a single tag with like a single word
[12:46] in it. And then you just got to import that wherever you want it, and then you can put it wherever
[12:50] you need it. So those are the main reasons why things like React exist.
[12:55] And this is the same thing with Vue. This is the same thing with a lot of other frameworks.
[12:59] They're all kind of based around this idea of components and containing your logic and functionality within these components.
[13:07] OK. And this will make so much more sense once we actually look at the project.
[13:16] Yes, yes, yes. So I'm going to say, I was just about to say, I think it's like when I get mixed up with
[13:21] classes. And also it makes me think of how Google lets you color code tabs now and put them in groups.
[13:30] So but cool. Here's also a nice thing about React.
[13:34] You can write it with classes or without. So you can completely ignore classes for the rest of your life if you start writing React.
[13:41] I bet that sounds nice. That sounds pretty exciting, at least thus far.
[13:46] That's where I started on this journey of teaching myself all of this, because I got really stuck.
[13:52] So I know we talked about this, but we need to have, you said, Terminal and VS Code, right? Yes.
[14:03] Yes. So let's start with, we're going to generate our project.
[14:08] Now this is going to be using something called Yarn, which I already made sure you had installed. Yarn and NPM are both just like command line tools to help you do common JavaScript-y kind
[14:22] of things. And they're all using Node under the hood.
[14:25] And we don't need to get into Node, but that's kind of like another important piece of the whole JavaScript ecosystem and understanding where Node sits within things is something
[14:34] you're going to have to understand at some point. But don't worry about it now, because Node is like a huge beast onto itself.
[14:41] OK. So listeners or everyone out there, if you want to come on the show and explain Nodes
[14:47] at some point, you're welcome. DM me.
[14:50] Let's do this. Let's make the font bigger in your Terminal first off, so you can just do a command plus.
[14:58] See? OK.
[15:00] I told you, I haven't really touched this in so long. I've just barely knew what Terminal was.
[15:08] Let's talk about the Terminal real quick. The Terminal is something that scares new developers for good reason, because it's like
[15:15] a blank prompt. And it's like, tell me to do something.
[15:19] And it's like, well, what do you want me to tell you to do? And you need to kind of know that ahead of time.
[15:24] But what's cool about the Terminal is it allows you-- once you kind of figure out the commands and the things you need to do, you can just tell your computer to do things, and it will
[15:32] do it. And this is actually-- there used to be a time before we had GUIs, graphical user interfaces,
[15:39] like this nice desktop we have, where the Terminal was a computer. There was no other way to interact with a computer except with the Terminal.
[15:46] So the Terminal is kind of the more long-standing way of how programmers used to work with computers. So I would say embrace the Terminal.
[15:54] Once you kind of wrap your mind around it, it's actually really powerful to use. And you're going to find that it's like, if you try to always avoid the Terminal, you
[16:01] end up doing all these weird kind of workarounds just to avoid the Terminal. But if you kind of embrace the Terminal, it's going to be very, very useful for you in the
[16:08] long run. I would say that this is-- my time at Media Temple is definitely why I'm not as scared
[16:15] as Terminal, because when we had to fix customer servers and things like that-- and yes, you're probably right, my tech leads probably did totally just go search for the answer, because
[16:27] I didn't know how to do that back then. We would have to go through Terminal to their server.
[16:32] And A, that was really hard to conceptualize and do, yet at the same time-- shout out to Ahmed.
[16:40] I actually texted him out of the blue after like three years of not working there. And I was like, dude, I'm not scared of Terminal, and we're doing stuff on this thing I'm doing.
[16:48] And I actually somewhat know what you used to tell me now. I was really excited.
[16:52] So yay, Terminal. Super cool.
[16:54] OK, so what we're going to do-- and I'm just going to tell you exactly what to type here. So first, write the word "yarn," and then do a space, and then write the word "create,"
[17:09] and then do a space, and then write "beat," B-I-T-E, space. And then now we're going to give our project a name.
[17:18] So what would you like to call our project today? Tuesday.
[17:21] Tuesday. All right, not a very descriptive name, but we'll go with that.
[17:27] Let's make it all lowercase, too. OK.
[17:33] Does it need to be all lowercase, or does it need to be camelcase? So this is going to eventually be a Git repo.
[17:41] When I'm naming Git repos, I will do all lowercase and dashes in between the words. OK.
[17:48] Yeah, so I'm going to do Tuesday, July 5th. I'm going to do 05, not a five.
[17:55] Why four? Huh?
[17:58] Just because? Just because it's cool?
[18:00] Or why? Well, because what if you wanted to, say, sort it by the date?
[18:05] And if you do that, it's going to go 1, 10, 2, 22. It'll do it like that.
[18:12] So that's why you want the 0 in front. Groovy.
[18:16] Yeah. OK.
[18:18] So that's great. And then do space.
[18:20] And then you're going to do two dashes, and then the word template, great, space, and then the word React.
[18:33] And so what's happening with that is we're saying we want to create a Vite project, and we're doing that with the Yarn CLI, and we want to create that project, and we want to
[18:43] name it Tuesday, July 05. And then because Vite doesn't need to necessarily be used with React, you could use Vite with
[18:50] View, because I already said it's from the creator of View. You could use it with Svelte, which we haven't even talked about at all.
[18:55] We don't need to. You can do it with just straight-up vanilla JavaScript, which would also be a good thing
[18:59] for you to do at some point. But we want to tell it specifically, when we generate this project, we want it to be
[19:05] a React project. So that should be all we need to do.
[19:08] If you hit space-- or if you hit-- not space-- return, then that should generate our project. And really quick, you mentioned CLI.
[19:17] And for a very long time, I did not know what CLI was. I don't know why.
[19:22] I knew that it meant typing something like this, but I never knew that it was command-line interface.
[19:29] Yep. And a command-line interface is what you do on the terminal.
[19:34] So the command line is the terminal. Those are essentially synonymous terms with each other.
[19:39] Yeah. When I saw something, I was just like, oh, that's so cool.
[19:43] Mm-hmm. Yep.
[19:45] Awesome. So you should be able to find that project now in your VS Code.
[19:51] So actually, before we do that, real quick, I want to just try something. In your terminal, write the word "code," yep, and then do a space, and then write the name
[20:01] of your project that you just created. Yeah.
[20:07] And then see what happens when you do that. OK.
[20:10] So we would need to configure that first. So this is a nice kind of thing that lets you just immediately open your project from
[20:16] VS Code. But for now, you should be able to just go find it within your VS Code.
[20:21] OK. I barely know how to use VS Code, so this will be fun.
[20:27] Yep. So let's see.
[20:29] First, actually, just close that out entirely because you're already in a project. So yeah.
[20:37] Just close that out. Hit the red.
[20:39] Oh. OK.
[20:41] And then go to File. I didn't know that actually closed it.
[20:44] Oh, that's fancy. Look at that.
[20:46] Yeah. That's how you close them out.
[20:48] All right. Yeah.
[20:50] So you want to go to File and then Open Workspace from File, I think. Let's see.
[20:57] I can do Open. I never do this.
[21:00] I had to figure out how to do this real quick. Open Folder is what you want to do.
[21:06] There you go. Yeah.
[21:08] Oh. OK.
[21:10] So cancel out of that and then hit the red again. So go back to File and then Open Folder.
[21:18] Got it. Thank you.
[21:20] There you go. Yep.
[21:22] And then that would have been generated in, like, your gen genod folder. Yep.
[21:29] Yep. There we go.
[21:31] And then hit Open. Don't do anything else.
[21:33] Yep. Just that.
[21:35] Bam. Cool.
[21:37] Great. OK.
[21:39] Yeah. So now let's go back to your terminal.
[21:44] And now what we're going to do is we're going to do CD, which is change directory, and we're going to enter that project.
[21:50] So give it your name again. I can't click back.
[21:55] You've got to move back. CD?
[22:00] Yep. Just like that.
[22:03] Great. And then do just the word "yarn" and then execute that.
[22:09] And what that's going to do is that's going to install your dependencies. So any time you're doing a JavaScript project on your computer, the JavaScript project is
[22:19] usually made up of a bunch of code other people wrote. So like you didn't write the code for Vite, you didn't write the code for React, but we're
[22:26] going to create a project that's using those dependencies is the term. So we have to first download those from the internet onto your computer.
[22:33] So that's what's happening with this step. OK.
[22:37] And so just to make sure I'm following along, because we opened it in Visual Studio, that's the reason why we were able to change directories to it, because we were able to show that it
[22:51] existed by opening it? So the Visual Studio code part is completely decoupled from what we're doing right now.
[22:59] So your terminal always has kind of like a state that it's in. And so if you see right now on your command line, you see how it says Tuesday, July '05.
[23:09] It didn't say that before. That's because you're like inside that directory.
[23:14] And so the code you're looking at on Visual Studio code is just because you have that code on your computer and you opened up an arbitrary folder over there.
[23:22] You can open a terminal inside VS Code. I like to kind of keep them separate, because I also use a specific terminal that is called
[23:29] Warp. And it gives you a lot of really nice stuff.
[23:32] So I tend to keep them separate. You could have opened your project in Visual Studio code, generated it, and done that all
[23:39] through the terminal in Visual Studio code. But right now, the two are kind of separate.
[23:44] But they're both doing things on your computer, if that makes sense. Yes.
[23:49] I just wanted to get a bit more detail on it, because I was like, I'm following along. But I don't know if anybody else would that hasn't been here yet.
[23:57] Yeah. This is the type of stuff, it's just getting into the workflow of how do you open a project
[24:04] and work with it. It's like, this is why I really do highly recommend people start with things like Code
[24:09] Sandbox. Because you didn't need to know any of this to do Code Sandbox.
[24:13] You just opened up a browser and started writing code, and it had your whole development environment set up for you.
[24:18] So that's great. But at a certain point, you got to learn how to do it locally, you know?
[24:23] Yeah. There's a lot of reasons why, but it's just something you've got to eventually learn to
[24:27] do. And then you'll be glad you did.
[24:29] But there's-- Yeah.
[24:31] That's a big reason I'm also excited about Yare going through and doing a code review. Because I'm like, I'm pretty sure I wrote it in HTML.
[24:39] Yeah. Your font sizes are still a little too small.
[24:42] That work? Or you want a big--
[24:48] Do one more on the terminal, and then go back to-- and then close that up a little bit. Yeah.
[24:54] Yeah. Cool.
[24:56] And then open up your VS Code a little bit more, and then bump that font up like three times.
[25:01] Yeah, that's pretty good. Cool.
[25:03] And then you can also X out of that get started thing. Yeah.
[25:10] Sweet. And so you also see how now you have that folder called node_modules.
[25:16] That is what was downloaded when you ran Yarn. So open it.
[25:19] OK. And then close it, and never look at it again.
[25:22] Cool. I like that.
[25:24] It'll just scare you. Don't ever look at your node_modules.
[25:27] It'll stress you out. Because there's like hundreds of packages in there that you have no idea what they're
[25:32] doing. And if you try to look at the code, you're having no idea what it's doing.
[25:35] One day-- That's exciting.
[25:37] You will have to go into your node_modules and actually change something, and that will be the day you will know you're a senior developer.
[25:42] I'm so excited. Don't worry about that.
[25:44] I'll get there. Don't ever look at-- that's good advice.
[25:49] Remote load knows what I'm talking about. OK.
[25:53] Awesome. OK.
[25:55] Now, here comes the magic. So now what we have to do is we've generated our project.
[26:00] We have some code. Now we need to actually run it locally on our machine.
[26:04] So the way we're going to do that is we're going to type Yarn space dev in our terminal. Yep.
[26:12] And then hit that. And then it's going to tell you that this is now running on localhost 3000.
[26:17] And I'm assuming you probably don't know what localhost is. Localhost means it's only updating to your computer.
[26:25] It's not actually pushing it out to anything because it's not connected to HTTPS or anything. That was a great answer.
[26:32] That's exactly what it is. Yes.
[26:34] Don't-- like, I'm still really stuck on, like, understanding going from, like, browsers from-- I'm guessing you want me to open this in Chrome or not.
[26:45] Yes. Yeah.
[26:47] Because I'm assuming you don't have Brave. I don't even know what you just said to me.
[26:50] Brave is a more crypto-native browser that has, like, crypto wallets and stuff built into it.
[26:56] We already talked about this. I'm not allowed to look at that stuff until I understand this.
[27:00] Yeah. Exactly.
[27:02] And that's a good thing. So now here you are.
[27:04] So this is your React app. You have created a React app.
[27:07] You are now a React developer. And now just to make sure that that count does something, you got to click the Count
[27:13] button. That's part of the ritual.
[27:15] Wow. That was exciting.
[27:17] I know. Right?
[27:19] I have no idea how-- well, like, hmm. OK.
[27:21] I understood a lot of it. Yeah.
[27:23] So now we're going to look at the code, actually, because we haven't looked at any of the code yet.
[27:31] So that'll kind of help us out here. So what you should do now is you should rearrange your windows so we can have all three of these
[27:36] on screen at the same time. Yeah.
[27:39] I would say you could move your React app so it's kind of just below your terminal. Because your terminal, you only need a little bit of screen real estate right now.
[27:50] Yeah. That's pretty good.
[27:52] Perfect. Yeah.
[27:54] And then just keep-- don't touch your terminal at all. That's just set and forget that for now.
[28:00] And then, yeah. And then you could even probably move that up even a little bit more and just have it
[28:04] on top of there. Yeah.
[28:06] That's great. OK.
[28:08] Cool. So now you want to go to the src folder in Visual Studio, and then go to app.jsx.
[28:16] So you notice how it's not a .js file. It's a .jsx file.
[28:20] So that's what I was talking about, how this is kind of JavaScript, but not exactly. This is something called JavaScript extension language.
[28:28] And the reason why is because right now what you're going to be looking at is you're going to be looking at a combination of JavaScript and HTML at the same time.
[28:36] So you have a JavaScript function, and that JavaScript function is returning a bunch of HTML.
[28:48] I comprehend the words you're saying. Yeah, right.
[28:51] It is-- So here's what you're going to do.
[28:53] You're going to go into that file, and everything under Hello Vite plus React, delete that. Oh.
[29:02] Yeah. So from there, and then go down a little bit, down a little bit more, and then-- yep.
[29:11] Keep going. Keep going.
[29:14] Keep going. I can't see entirely to the bottom.
[29:16] And then the div, and don't delete the header. Yep.
[29:22] Delete all that. OK.
[29:25] That was fun. And then scroll through a little bit.
[29:27] Great. And then save.
[29:29] And now you saw the change on the left. And also, part of your screen is being blocked right now by the header of your streaming
[29:37] setup. Oh, yeah.
[29:39] I can turn that off. Give me a second.
[29:43] Hey, now we know that I need to make it smaller, or in a different spot. There we go.
[29:49] Or just account for it with how you position the windows on your screen, however you want. So now what we want to do is, where it says the p tag, change that to just say, "Hello
[30:01] from Teach Gen Tech." Great.
[30:04] And then save. And then you'll see that change in your window.
[30:18] So that's what I mean. So that's HTML.
[30:21] That's a p tag. So you've written a tiny bit of HTML before, right?
[30:25] A tiny bit. Yes.
[30:27] Yeah. So that should make sense.
[30:29] You'll see there's an image tag there. And there's a div, right?
[30:32] Yes. Yeah.
[30:34] So that is the HTML part. But then above that, you have the function app.
[30:39] And so that's a function. And so that's not HTML.
[30:41] You can't write functions in HTML. You write functions in JavaScript.
[30:44] So that's why I say this is a JavaScript function that literally returns HTML. I think this is going to be something that, like, everything, again, you're saying is
[30:54] making sense. I think it's like, when I go through last week's training in more detail, because we
[31:03] wrote some things in JavaScript and some things in HTML, and now I'm, like, stuck on-- I get what you're saying.
[31:10] What's what. Yeah.
[31:12] Yeah. Yeah.
[31:14] So that's easier for you. If anything, it's going to be a little more complicated for a while, because you're going
[31:16] to be mashing it up all together. OK.
[31:19] But the two-- Yari is going to have more questions later on.
[31:23] Like, got it. I'm learning.
[31:26] I'm following for the moment. And then we're going to delete one more thing where it says const count setCount useState.
[31:32] Delete that. That was for our counter.
[31:34] We're not going to worry about that too much. That's going to be your React 102.
[31:37] We'll be learning useState. But for now, we're good to go.
[31:41] And then just for my sanity, delete line 6, and then line 11. Would you delete line 15, or because--
[31:54] No. Because you want to have a space in between your imports and your function, and in between
[31:59] your functions and your export. Not because it's going to break anything, but just because that's the standard.
[32:03] It's going to look weird if you don't do that, because there's always going to be three pieces here.
[32:09] There's going to be the imports, which is the stuff you need to make this component work.
[32:14] And then there's going to be the component itself, which is going to have a name. And then there's going to be-- you need to export the component.
[32:20] So that's so you can bring the component into another file. So let's also delete the import useState at line 1, because we're no longer using that.
[32:29] And again, you don't need to worry about useState at all at this point. And then save that.
[32:36] And now, just to explain what I mean about this being exported, now go to main.jsx. So here you see, on line 3, we're importing the app from the app file.
[32:51] And then we're having the app displayed in our react.dom.createRoot. This is another React-ism that you don't need to worry about really understanding right
[33:01] now. The point is is that all of your components basically get smushed together into this one
[33:07] kind of like uber component. And that component is then your entire app.
[33:12] So any time you're trying to trace back an issue, you can always be like, OK, where is this component?
[33:19] And how does it sit in what's called the component hierarchy? This is more React terms.
[33:24] That is going to take a little while to sink in. But the point is is that every file has a component.
[33:29] It exports a component. And that component can be imported into other files.
[33:36] >> On if you're exporting it into other files, if you update the original one, will it update everywhere else without having to go to backtrack it?
[33:46] >> Yeah. And that's why when you were updating it in app.jsx, you were changing things, and you
[33:51] were saving it, and you were instantly seeing the change. You didn't have to go into your main.jsx and do anything else.
[33:56] Right? >> OK.
[33:58] Cool. >> Yeah.
[34:00] Go ahead. >> Is there anything outside of going into the individual files that are going to tell
[34:06] us the hierarchy? >> There's what are called the React dev tools, which will give you kind of more visibility
[34:14] into the component hierarchy. So that's the thing that you'll probably want to get into at some point if you plan on becoming
[34:21] like a React dev. This is the thing, though.
[34:23] You don't necessarily need to ever write React. I think it's an important thing for developers to learn because it's kind of becoming the
[34:30] standard in a lot of ways, and it's what a lot of front-end devs are expected to know. But if you want, you could write Svelte, and Svelte doesn't have the same kind of hierarchy
[34:39] idea. It's a little bit different.
[34:42] There's similar things, but it's not exactly the same. So for the most part, you're going to get deeper into some frameworks, and you're going
[34:51] to install tooling that's going to give you better visibility into them, and you'll build mental models around them that are kind of unique to them.
[34:57] So for now, it's just like we're kind of just doing a high-level overview, and the point of this whole stream was not really necessarily to teach you React, but to show you how to
[35:07] get a React app online. That's really going to be the cool part here, because right now, you don't have a website.
[35:13] You have a thing sitting on your computer running on localhost, and that doesn't help anybody.
[35:17] So for me, the thing that I think is really cool is that now we're at a point where you can get this onto a Git repo, and then log into something like Vercel or Netlify, and
[35:27] you can click a button, and it's going to deploy it for you. And so first, let's make sure that we can get this onto a Git repo at all.
[35:35] So I should have asked this before. Actually, do you have a GitHub account?
[35:39] Yes. Great.
[35:41] That's very important. So yeah, let's go to GitHub.
[35:44] And actually, before, let me show you a cool trick, actually. Let's type "repo" -- actually, first, go back into your terminal and hit Control-C.
[35:59] That's Command-C, right? Control-C, not Command.
[36:01] Yeah. Oh, Control-C.
[36:03] There we go. Yep.
[36:05] So that did -- that killed our development server, so now it's no longer running. So if you go refresh in localhost 3000, your React app will no longer be there.
[36:12] Yep. There you go.
[36:15] And that's good. Because right now, our app is done.
[36:18] You've written the entire app. We're finished with it.
[36:21] It's so exciting. I feel like I can mess things up very well there.
[36:25] I'm excited. So now go back into your browser and just go to "repo.new" and then bam.
[36:37] So remember that one. That's cool.
[36:41] Yep. So give your repository name the same name as your project.
[36:47] Okay. Cool.
[36:51] And then we want it to be public and keep all that exactly the way it is. Don't change anything.
[36:58] And then hit "Create Repository." And what's cool is they're going to give you a set of instructions to actually get this
[37:07] on there. So you can see the instructions.
[37:10] Don't do the echo because you already have a -- or you technically don't have a readme, but let's skip that instruction anyway.
[37:16] Go to -- start with "git init." Yep.
[37:19] And then do that. And then don't --
[37:25] Aw. I got excited.
[37:27] That's fine. That's not an error.
[37:29] That's good. So it's letting you know you -- this is something that we should do later is configure things.
[37:37] So it uses "main" instead of "master" because people don't use the term "master" anymore. They use the term "main."
[37:42] But there's a step within this flow that will change it to "main" for you. So next, do "git add."
[37:51] So "git" with the "i." Oh, yeah.
[37:53] I got -- you know, just, like, hearing it and typing it. Right.
[37:58] Yeah. Totally.
[38:00] Going to get used to that one. Yep.
[38:02] Yep. So "git add."
[38:04] And then do "space" and a "period." And so what that's going to do is that's going to put all of your changes into the staging
[38:12] area. This is also "git speak."
[38:14] Don't worry about that too much. And then now copy the "git commit -m" command from the browser.
[38:22] Yep. Perfect.
[38:28] So that committed everything. Now do the "git branch," and that's going to change your branch from "master" to "main."
[38:37] Cool. And then do the next one.
[38:39] This is going to set the "remote." So this is what's going to actually connect your current project to this online GitHub
[38:47] repository online. And then the last one is actually going to push your project up into this repo.
[38:54] Yes. And you will do-- OK, so you're going to have to log in.
[39:06] It should hide it for you. I don't know if it necessarily will.
[39:08] You might want to pull it off screen just in case. I would say go off screen just in case.
[39:11] It should hide it for you, though. I don't even know what I-- yeah.
[39:17] Also get a password manager if you already have one. I pay one password, and it's actually like a piece of software I pay for because it is
[39:25] extremely nice and it's going to save you hundreds of hours of your life just to pay for it.
[39:30] So I would recommend getting a one-password account. It'll change your life.
[39:37] "Please use a personal access token." Hold on.
[39:45] Oh no. That's not good.
[39:51] OK, so that's weird. OK, there's another kind of stupid hacky way I think we might be able to do this.
[40:03] Let's see, actually. Let's try logging in to-- wow, this is funny.
[40:16] Friggin' Git, man. Every time.
[40:18] Yeah, try from the VS Code terminal instead. OK, and is it sign in to sync settings, that one?
[40:29] No, no. So do command J. Great.
[40:36] And then run that last command, again, the git push origin main. I don't think-- I think you're going to have to log into GitHub through VS Code for this
[40:43] to work. So let's first see what this does.
[40:46] It's going to probably give you the same thing. I'm teaching Ramon all sorts of stuff over here.
[40:52] Oh, yes, that's perfect. OK.
[40:56] This is what's nice about the fact that all these companies are now owned by the same company.
[41:01] So GitHub is owned by the company that makes VS Code. Yeah, you just got to remember your password.
[41:12] Do you not know your GitHub password? No, I just set up all these accounts, and I made them all different passwords.
[41:24] So-- Yeah, this is-- and you don't have a-- so why are you saving your passwords?
[41:28] Are you just trying to remember them all? You know what?
[41:32] I would have prepared. I didn't even think I'd have to log in.
[41:36] Yeah, no. This is totally fine.
[41:38] Yeah, you're getting a lot of password manager, definitely, for sure. I would say, if you need to, you can go reset your password right now, and that will--
[41:46] I'm going to try. --take you a bit or two.
[41:48] Oh, hey. Oh, is that it?
[41:50] I think Chrome might have saved it. There you go.
[41:53] Sweet. But I can't really-- I'll reset it after this.
[41:59] Cool. Yes.
[42:01] Yay. Yes.
[42:03] Great. OK, and then close that other window.
[42:06] OK. OK.
[42:08] Go back to the-- yeah, close that one out, too. Uh-huh.
[42:13] Close that one out, too. And then hit Refresh.
[42:16] On this one? Yeah.
[42:19] Mm-hmm. There's your project.
[42:22] Yay. Excellent.
[42:24] Great. The next step should be very simple.
[42:28] Just go to Vercel.com. Vercel, right?
[42:36] Yep. Yeah.
[42:39] There we go. Cool.
[42:41] And then let's open this up just to be the whole thing, because this should be all you need right now.
[42:46] And then also, bump your font up a couple times. Yep.
[42:50] That's perfect. And then hit New Project.
[42:55] Yep. And then--
[42:57] Import Git. So add GitHub account.
[42:59] Yep. Thank you for staying logged in.
[43:01] I appreciate you. GitHub.
[43:03] And click out of that, and then Import. And then notice, there's something very cool happening here.
[43:05] You see how it says Vite already? Yes.
[43:07] So Vercel can literally look at your project and tell what it needs to build. So this is incredible.
[43:09] Yeah. Yeah.
[43:11] Yeah. So you see Redwood Deus is in there?
[43:32] Yeah. That's the team I'm on.
[43:34] So there's like all of these. I know the creators of probably about half of these frameworks, so if you're ever looking
[43:40] for more guests, I can personally introduce you to a lot of these people. But this is what's really, really cool about Vercel is that you don't have to configure
[43:48] your project to tell Vercel how to build it and how to put it on the internet. It literally looks at your project and lets you just click a button, and it's going to
[43:57] put it on the internet for you. OK.
[44:00] Yeah. So just click out of that, because you're already all set up.
[44:06] And then hit Deploy. Now, I'm just curious what these are, though.
[44:10] Cool. Yeah.
[44:12] I mean, I can explain this. So when I was talking about how you need to build it, that's the transformer here from
[44:16] the JS, JSX to the JS. So it's going to run npm run build, which is running the vbuild command.
[44:23] And you could do that on your own computer, too, and kind of see what that does. I skipped that step just for kind of time's sake.
[44:30] Yeah. But what it does is it takes your entire project and then bundles it together, and it puts
[44:35] it in a folder called dist. So that's the output directory.
[44:39] And then the output directory is now where your project lives. And so when you're coding on localhost, that's the thing that I was saying takes Webpack
[44:49] a long time. It needs to take your code.
[44:51] It needs to turn it into this other thing that's in a different folder with completely different code.
[44:57] And then it needs to take that code and actually run it in your browser. So there's all those steps involved that Vite is kind of doing for you.
[45:03] But when you're deploying it, your code isn't changing, hopefully. Your code should stay the same once it's done and you want to deploy it.
[45:11] So it just takes that. It does the build step once.
[45:14] And then your project is built, and it's in this dist folder. And then that is the thing that actually gets shipped to the server that runs your website.
[45:22] I'll ask you about that again after I learn more. But this is what's awesome about these platforms, is you don't need to know any of this stuff.
[45:31] This is stuff that's important to know, because at a certain point, stuff's going to break and you're not going to know why, and you need to know how to debug it.
[45:37] But at this point, all of this is going to be done for you. You don't need to really understand any of that.
[45:42] I deployed like two dozen websites to Versaille before I understood that a project was being built and put into a dist folder, you know, because it just does it for you.
[45:51] All right. Click actually the building little arrow.
[45:56] And then you can... Oh, too late.
[45:58] It's already done. Yay!
[46:00] So go to your dashboard, and then go to domains. Yep.
[46:07] And then click that, and then drop that baby in the chat so everyone else can see your wonderful new website you just created.
[46:14] Yay! Cool.
[46:16] You did it. You deployed a React app to Versaille with Vite.
[46:23] Cool, right? It is.
[46:27] It is. I'm also thinking how I'm going to remake one of these.
[46:34] Totally. And dude, this is what I do for my job.
[46:38] I create little example apps, and then I deploy them to a deployment provider. And then I have an example app, and then I can show it to people.
[46:46] This is what I just showed you. This is my actual workflow for actual projects.
[46:51] That's because I'm a dev advocate. Like, obviously, if you're building a whole production app, you're not usually spinning
[46:56] up lots and lots of new projects and deploying lots and lots of projects. You're usually working on a single project that was built 10 years ago and is only deployed
[47:04] in one area. But for what you want to do, you want to be in DevRel, you want to be a dev advocate,
[47:09] you're going to do this 100 times in the next year, minimum. I'm letting it soak in.
[47:18] Okay. So for homework, a few questions.
[47:24] Just to keep the same theme on every single one of them, I will write my three or four favorite podcasts just on this instead.
[47:34] So if I want to change the logo, would I just upload another SVG file? Do I just Google it and see if I can figure my way out of it?
[47:48] You could do that. You could literally just take what's written in the logo.svg and rewrite that because then
[47:53] you wouldn't have to worry about importing a different thing back into your app.jsx. Or you can create a new file with a new SVG, then you're going to figure out how to import
[48:02] that. That'll be another step.
[48:04] So yeah, there's so many different ways you can do stuff in React and so many different avenues of how you can start actually building this out into your own custom app.
[48:14] So yeah, that'll probably be for the next episode, though. Okay.
[48:18] So now I have my homework set up for me. Yeah, and Ramon was saying there may be some CSS wiring you'll have to do.
[48:29] Right now it's set up where you have an index.css and app.css, so those should already be set up.
[48:36] But CSS and how CSS kind of comes into the picture is kind of its own separate complicated question because everyone has opinions on how you should do CSS.
[48:45] Some people want to write regular CSS, some people want to use something like Tailwind and you have to actually bring out a CSS expert to talk about CSS because I don't know.
[48:53] I don't write CSS at all. Not because I think CSS is beneath me, because I think CSS is too complicated for me.
[49:01] Okay, that's going to be a lot of fun. Yeah.
[49:06] Yeah. Okay.
[49:08] And okay, this might be a very, very silly question, but I'm going to ask it anyway. So what makes this an app compared to just a regular website like a .com?
[49:22] That's a great question. So most people would say the difference between a website and a web app is that a website
[49:30] is static content. So a website would be, say, a blog post that you can read, whereas a web app has a button
[49:40] that has a counter on it that you can click to make it change. That's kind of the...
[49:45] So if you think about it, like, when you have a blog or if you have... Imagine like a restaurant's menu.
[49:52] So you have a restaurant, you can have a menu, you can read the menu, that would be a website. If you could also buy the food on that site and actually order it and pay, then it would
[50:02] be an app. Does that make sense?
[50:06] It does. I'm working on converting it in my head to something that will stick.
[50:11] Yeah. So basically, is it interactive or not?
[50:13] Can you actually interact with it and do stuff with it, or is it just like a thing you're reading?
[50:18] It's just like content. That's kind of the distinction that most people make between a website and a web app.
[50:22] But there's also lots of people who will argue about the semantics of those two things and where the boundaries are between.
[50:29] For me, that's a nice, clean boundary that I think is pretty comprehensible and most people will agree with.
[50:34] Okay. So does that mean most web apps by non-techs are called websites, even though they're web
[50:42] apps? Yeah.
[50:44] I mean, like Twitter is not a website, Facebook is not a website, any social network is not a website, because by definition, if you can't interact with it, it's not a social app.
[50:52] So the vast majority of things we do on the internet these days are apps, but the vast majority of things on the internet are websites.
[51:01] Because if you think about it, there's these large companies with these very small number of apps that we interact with on a regular basis, but that's actually a tiny, tiny, tiny
[51:12] fraction of the entire internet. The vast majority of the internet is like these small little mom and pop shops and people's
[51:18] personal websites and things like that. So most of those are just websites with just some content that people want to put out that
[51:25] people can read. But the things that people actually do on a day-to-day basis when they're using the internet
[51:30] are almost entirely web, because you go to the internet to do stuff, you know? An RSS feed.
[51:41] An RSS feed is a way to get content. So a podcast has an RSS feed, and then every time someone puts a new podcast episode out,
[51:55] that is added to the feed, and people who are subscribed to that feed get that new episode pushed to them.
[52:01] So you can do that with a blog, you can do it with a podcast. So is that a web app then?
[52:05] RSS is neither a website or a web app, it is probably what you would call a protocol, I would guess.
[52:14] Oh. Yeah, that would make sense, like HTTPS or IMAP or...
[52:19] Yeah, Wikipedia calls it a web feed. Oh.
[52:23] So I would say you could use RSS within a website or a web app. Most of the time an RSS feed is kind of something that people will put on a website so that
[52:36] web apps can consume it. Okay.
[52:40] Okay. Yeah, that's true, you get HTML from an RSS feed, so RSS feeds, or is it actually XML
[52:50] technically? I think it might be.
[52:56] I'm like stuck in processing mode. Yeah, no, we're starting to talk over each other and talk back, so don't...
[53:03] No, no, no. I think it's good.
[53:05] I think it's good because it's giving me examples of... And this is something that I love about having teach Gen Tech is I'm able to ask for things
[53:16] that go around it, because I may be stuck on what normally makes sense as the next step, but I'm still stuck on how this works with it, so I'm not understanding the next step.
[53:26] Yeah, and you're still building mental models around all of these terms, and the technology is just really, really the hardest thing, and this is why, for me, listening to podcasts
[53:35] was really useful because I got to hear people constantly speak in these terms and speak with each other about it.
[53:42] So yeah, the feed itself is XML, but a blog post inside would be HTML. Yeah, exactly.
[53:49] So the RSS feed itself is HTML that embeds, or is XML that embeds HTML in it, kind of the way that React embeds HTML in JavaScript, so that's kind of one way you can think about.
[54:01] XML is a very old programming language that is kind of baked into things like RSS, but you will almost certainly never write XML, or hopefully you won't have to write XML anytime
[54:13] soon. Well, Ramon, you know what I'll be working on before our Teach Gen Tech next week, so
[54:20] that'll be exciting, and then I have Rizal the next day teach me about GitHub. I feel like, by then, I'll have a more solid understanding, but I will-
[54:35] With Rizal and GitHub, so much of the stuff you're going to do is going to be based around GitHub.
[54:40] And the more you can learn about GitHub up front, the better, because- I'm so excited.
[54:45] It's like, as you saw, that was the connection point between our project and the deployment provider.
[54:50] And this, what's really cool, is that if you wanted to change your project, what you need to do is you need to change something, and then push it up to your Git repo, and then
[55:01] Vercel will automatically deploy that new change for you. So that can be your homework, is make a change, and then push that change to your Git repo,
[55:10] and then see it update on your Vercel site. I was going to say another thing that I think is very confusing to have answered at some
[55:19] point would be... So Stoplight is my main point of reference when it comes to GitHub, is we would be able
[55:30] to create new projects just like we did today, and it would sync to GitHub. I think the part that is most confusing, though, is going from VS Code to GitHub to update.
[55:48] Like, I don't know. I'm going to ask it after Vercel.
[55:51] And this is why I say getting comfortable with the command line, because the command line is where you can do the commands to do stuff with Git.
[56:00] You can also... Visual Studio Code itself has Git functionality built into it.
[56:05] There's also the GitHub desktop app, which... You're going to be able to figure out three or four different ways to get a GitHub project
[56:14] up on the internet. Everyone has their preferences on which ones they prefer.
[56:19] Some people stick with the terminal. Some people like having a more visual kind of desktop app way to do it.
[56:24] Some people like having it just in their code editor already. I used the GitHub desktop app for a little bit, and then eventually kind of just stuck
[56:31] with using the terminal and VS Code by itself. But you should play around with all these things, because then you can kind of form
[56:38] your own opinions about how you like to do stuff. Okay.
[56:42] And just remember, it's all part of the process. You don't need to learn this all at once.
[56:47] You'll take in a new tool at a time, and it'll start to accrue, and before you know it, you're going to have 20 of these things, and you're going to be a pro at all of them.
[56:56] So it's all part of the process. I've been doing this now for...
[56:59] I first started learning to code in 2018, and then I did a boot camp in 2020, and I've been working professionally in tech for a year and a half.
[57:10] So that may seem like a long time, it may seem a short amount of time. It kind of depends on your perspective, you know?
[57:15] So yeah. Thank you, and thank you for your time.
[57:19] You definitely taught me quite a bit, and I'm still stuck on the processing side of it, because I'm like, "Okay, cool.
[57:27] I think I should have questions," but I'm like, "I need to process it." It's a lot to take in.
[57:33] The most important thing is you should have a question when something breaks. So when something breaks, it's like, "Well, how do I get to the next step?"
[57:40] Because you had a goal. The goal was to create a project to get that project onto the internet.
[57:45] As long as you have that goal, then along the way, you can worry about where the questions come in, because you'll be stuck at a certain point, and then you'll have a question, you
[57:54] know? So I would say that's the main thing, is start with a goal, and then work through that goal,
[57:59] and then as you're going, questions will naturally arise. Yes.
[58:03] Yes. And I will be getting this done before next week's Teach Gen Tech.
[58:10] Yes. I could see the rabbit holes, because- So many.
[58:14] Yeah. I have so many questions, too.
[58:16] Yeah, that's why there's a lot of times where I would start explaining something, and I'd be like, "Don't worry about that," because you got to stick to the goal you're trying
[58:24] to do, and you could fall down a week- or a month-long rabbit hole with so many things along the way.
[58:29] So, yeah. And this is why I really like just creating content and blogging, because then I can pick
[58:34] a rabbit hole, and I can go down it, and then when I come out of that rabbit hole, I have a blog post to share with the world.
[58:39] Yeah. That totally makes sense.
[58:41] That totally makes sense. And thank you for answering so many questions.
[58:46] Yeah, this was super fun. Yeah.
[58:49] Homework is going to be where it's at. I'll do this anytime.
[58:51] Don't worry. Happy to come back.
[58:53] I'm excited. I'm having you back on the show and be like, "Wait.
[58:55] There's so many questions. Just so many questions."
[58:57] Yeah. Yeah, this was super, super fun.
[58:59] Thank you for having me. Yes.
[59:01] Thank you. And, Ramon or Yeri, do you have any other questions?
[59:03] Thanks for hanging in the chat, Ramon. Yes.
[59:05] We'll see you here. Yes.
[59:07] Agreed. Yeah, me and him have been following each other on Twitter for a while.
[59:09] I haven't interacted with each other a ton, though. Yay.
[59:11] Ramon is so cool. We ended up having like a two-hour conversation like a week ago.
[59:31] Yeah. Yeah.
[59:33] I see him out in the community doing cool stuff for sure. Yeah.
[59:35] He was the first one that taught me about what peer programming was. So he was going to have me teach me something and then I talked to you and a few other people
[59:45] and then I'm like, "I'm just going to do my own show. That's just what's going to happen."
[59:51] You are. You are.
[59:53] We see you. Awesome.
[59:55] Well, thank you so much, Anthony. Looking forward to having you on the show again.
[59:59] Yeah, for sure. [BLANK_AUDIO]

