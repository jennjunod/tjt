---
showLink: "https://www.youtube.com/watch?v=piWcBs9CTHs"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "jenn-makes-tech-integrating-twitter-api-with-prisma-and-mysql"
title: "Jenn Makes Tech: Integrating Twitter API with Prisma and MySQL"
publishDate: "2022-10-23"
coverImage: "https://i.ytimg.com/vi/piWcBs9CTHs/maxresdefault.jpg"
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

[00:00] what up what up beautiful humans here is day two of don't know how long I'm going to stream and to get all this work going I also totally slept horribly yesterday with like my leg
[00:19] healing and stuff and yeah so that's that's that's fun it's fun it's fun for some reason that any type of like painkiller and stuff makes me wide awake it's very very annoying
[00:36] but you know at least I was fortunate enough to be able to get rid of the pain for a bit so you know you win some you lose some and so for today's dream I will get you all caught
[00:54] up from yesterday we did a lot yesterday and not gonna lie I just worked on showing up today because I was struggle bussing very much struggle bussing and we're gonna hit
[01:14] the timer before we hit break and we're gonna hit break. So let's get started. I'm gonna start off with a little bit of a
[01:56] good morning. And good morning or good evening to all of you. I feel like this is really loud right now. I should probably turn this down. And I just realized that also my speakers
[02:16] are probably super loud and they don't need to be. Okay I'm feeling this is a good volume. All right. So we are going to try something new of just doing stuff through VS Code. So
[02:59] I don't want to run a bug. Go away. We're going to do a new poll just to make sure I have everything which I do. Yay. Oh hi Jay. Hello. I'm about to explain what I'm doing
[03:18] today too. So this is exciting. Okay. So for everyone to have all the links that I've been working with. My GitHub repo basically has everything. And Jay I feel like I haven't
[03:39] seen heard you in forever and I know it's been conference season. But I was like so happy to see that you're still doing the newsletters for Python because Pythons have been become
[03:50] weekly now on Mondays with Laura which is phenomenal. But I do. Yes. Doing some JavaScript and Twitter things. Yes. I am. I'm going to use my mirror board because it's like the
[04:06] easiest way for me to keep track of what I'm doing because I'm learning all of this. So yeah I want to auto tag people and have this auto toast auto post. And oh it actually is
[04:25] going to work now. This one. Of working on like what order I'm actually going to build things in. And how I think they're going to work. Well I'm glad things are slowing down.
[04:44] We still need to have you on the show. Yeah. This stream is just for me trying to get this project done. I still mostly just stream during the week. So that part hasn't changed at least.
[05:05] We are. I'm learning about databases which has been fun and difficult. But we've been missing you on Mondays because even Laura now when we're whenever we were referring
[05:21] to F tags or F F strings F. Now I'm trying to. I hope you know what I'm talking about but you may not. We refer to you though Jay. We talk about you. Just know that in good
[05:36] ways. Strings yay. I'm glad. What's the longest you've streamed because I've realized I need to like give myself a timer. Or I feel like I'm gonna be here like all day and not take
[06:12] breaks and get really really frustrated. Do you do anything like that. What am I doing. It's link everywhere. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah. Yeah.
[06:50] Yeah. What up Brian. And then one more week of insanity and then chill. Yay. OK. Yesterday I streamed for like five hours but I did like step away for a bit. Like I did like this
[07:17] countdown and then like took a half hour break and then came back. So my five hours doesn't include that but it was still like crazy. So I think yesterday stream just working was
[07:30] three hours but still at the same time even though I was like walking away I was still like thinking about everything which is just kind of crazy. Oh thank you Ryan. I am putting
[07:57] it on my LinkedIn once I find my post because I realized I said I would put it in the thread and then I didn't. Oops. But without planning it I also started 100 days of code. I've been
[08:12] meaning to. And I was like y'all I'm coding every day now doing this. So I'm just going to we're just going to start it. It's four days in now. So might as well. OK. So right.
[08:30] Might as well. Look up Twitter API stuff. I have not looked at this at all. So I have no idea how far I'll get or if it's going to cost anything or all that. Oh nice. Yeah.
[09:06] I'll be I'll be around. Feel free to read later and come back and hang out with us. Thank you for saying hi. This is going to bug me. I need to be the same size. This is
[09:37] going to bug me. Wait a minute. I need to actually read this. I don't think I need this. I don't think I need this. I don't think I need this. I don't think I need this. I don't
[10:32] think I need this. I don't think I need this. I don't think I need this. I don't think I need this. Good call Ryan. Good call. And y'all I'm like super struggle busting today.
[11:18] Like I'm not screaming for long and then coming back later because I'm so tired. I took a pain pill for my leg and then forgot how wide awake it makes me. So it was fun. It was fun.
[11:41] Where am I based? I'm based in the US. Scroll to views. Making a bot. I don't think I'm making a bot. Building tools for Twitter users. I think other people will Twitter use this.
[12:04] No, it's not a government. Sure. Sign me up for the latest. Let's do this. Oh, all the scrolls through all of the info. Yay. Okay. I will go verify my email. Oh, y'all I get
[12:37] to name my app. I'm so excited. It is literally going to be Tweety tag. Hopefully. And I feel like just as a sidetrack, I am going to Tweety tag. In case anybody is curious, I was explaining
[13:04] this in a, like what I'm working on. And I was trying to say Twitter and tweeting. And I said, Tweety. And I was like, you know what? Tweety tag. That is what we're going to name
[13:18] it. Oh, we're going to get some keys. Oh no. Somebody already has Tweety tag. I mean, now I'm just curious what they have. Oh, okay. Interesting. All right. Whatever. Let's come
[13:50] up with a Tweety tag app. That is my app name. That's exciting. All right. Yes, y'all, I am viewing. You can see all my stuff today. I will be changing this later on. I am letting
[14:16] people see the keys and things like that because I think it's really important to be part of the setup. Okay. The dashboard. Oh, okay. Fine. I will officially, officially. And yes,
[14:34] I will be changing them. So, please know that. Okay. Yes, I think. Yes. All right. This is as far as I'm going to get on the app at the
[15:17] moment. I'm thinking how I'm going to do this. Because I have my database. I have that all set up. But then. I don't know. Getting started. Tools and libraries. Tutorials.
[16:06] Docs. Fundamentals. Security. Tools and libraries. SQL. Oh, I unselected it. Oh, no. I want the opposite.
[16:48] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[17:48] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[18:46] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[19:43] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[20:40] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[21:39] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[22:20] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[23:17] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[24:14] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[25:10] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:07] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:31] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:33] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:35] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:53] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:55] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:57] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[26:59] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[27:57] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[28:55] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[29:49] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that.
[29:51] Okay. So, I'm going to go ahead and do that. Okay. So, I'm going to go ahead and do that. know how to google it. I'm just trying to think out loud like I have my Prisma like
[30:08] connected to my database. I got that done yesterday but now I'm looking and I believe I need to do a REST API to be able to connect it to the Twitter API. But then also I need
[30:31] to build the front end of it. And I don't know what I would look for that. I don't even know if that made sense out loud. Uh, hi Ryan. Um, I was just saying that like
[31:11] I think that I need to set up a REST API on my Prisma so that way it calls and does everything with the Twitter API. But then I'm also stuck on, um, what, how do I input and build a like
[31:37] front end web app to be able to do the input of everything. Yeah, like I
[32:21] need to have it go to the Twitter API, like at the end of the day, um, to be able to post on Twitter, but like building the front end would, I'm also struggling because I, it built
[32:49] in Node.js, I think. Because this just says JavaScript, but it doesn't tell me, waaah. (upbeat music)
[33:20] (upbeat music) (upbeat music)
[33:27] (upbeat music) (upbeat music)
[33:44] (upbeat music) (upbeat music)
[33:50] (upbeat music) (upbeat music)
[34:14] (upbeat music) (upbeat music)
[34:25] (upbeat music) (upbeat music)
[34:40] (upbeat music) (upbeat music)
[35:02] (upbeat music) (upbeat music)
[35:13] (upbeat music) (upbeat music)
[35:30] (upbeat music) - Thanks Ryan, at least for, you know,
[35:53] like thinking about it. I'm also asking random people I know
[36:00] to see if they maybe know too. (upbeat music)
[36:06] (upbeat music) (upbeat music)
[36:26] (upbeat music) (upbeat music)
[36:32] (upbeat music) (upbeat music)
[37:01] (upbeat music) (upbeat music)
[37:07] (upbeat music) (upbeat music)
[37:27] (upbeat music) (upbeat music)
[37:40] (upbeat music) (upbeat music)
[37:52] (upbeat music) (upbeat music)
[38:11] (upbeat music) (upbeat music)
[38:35] (upbeat music) (upbeat music)
[38:49] (upbeat music) (upbeat music)
[39:00] Hello, hello everyone that has joined. I am stuck on creating, so I probably,
[39:17] I've been having fun doing this probably entire project backwards.
[39:21] I am working on making a, an app that will auto post things for me on Twitter.
[39:31] Basically people enter their Twitter handle, I create the Twitter space link and voila,
[39:40] every week this will auto post for me. Now, to make this all go through has been interesting
[39:48] and I had to restart the project. So I am working on it again.
[39:57] And I'm thinking I should have started with Prisma on my front end,
[40:03] but I am looking to see if I can set up, install a Next.js project.
[40:13] Actually, let me help. Next.js web app.
[40:23] (upbeat music) Oh, I don't want Netlify.
[40:30] (upbeat music) (upbeat music)
[40:38] Thank you Ryan for posting that. Yes, I'm like such in like concentration mode,
[40:59] like trying to figure this out. (upbeat music)
[41:04] I have no JS. (upbeat music)
[41:17], actually. (upbeat music) (upbeat music)
[41:25] Actually. (upbeat music)
[41:44] (upbeat music) See, I don't wanna do that,
[42:10] but (upbeat music) install.
[42:24] (upbeat music) (upbeat music)
[42:29] (indistinct) (upbeat music)
[42:48] (upbeat music) (upbeat music)
[42:53] (upbeat music) (upbeat music)
[42:58] (upbeat music) (upbeat music)
[43:03] (upbeat music) (hums)
[43:30] (upbeat music) (upbeat music)
[43:36] (upbeat music) (upbeat music)
[43:41] (upbeat music) (upbeat music)
[43:46] (upbeat music) (upbeat music)
[43:51] (upbeat music) (upbeat music)
[43:56] (upbeat music) (upbeat music)
[44:01] (upbeat music) (upbeat music)
[44:07] (upbeat music) (upbeat music)
[44:12] (hums) (upbeat music)
[44:39] (upbeat music) Now I'm just concerned that if I like deploy
[44:46] or like install this web app, that it's gonna overwrite everything, but.
[44:51] (upbeat music) (upbeat music)
[45:22] But I think this is what I want. Think it is at least.
[45:27] I like that they have this, that. Oh, yay.
[45:33] Yes. (upbeat music)
[45:51] So I'm almost wondering if, (hums)
[45:59] 'cause I don't have a public folder. (upbeat music)
[46:05] (hums) (hums)
[46:13] (upbeat music) (upbeat music)
[46:18] (upbeat music) (upbeat music)
[46:24] (upbeat music) (upbeat music)
[46:29] (upbeat music) (upbeat music)
[46:34] (upbeat music) (upbeat music)
[46:39] (upbeat music) (upbeat music)
[46:44] (upbeat music) (upbeat music)
[47:12] (upbeat music) (upbeat music)
[47:17] (upbeat music) (upbeat music)
[47:22] I'm debating with Tyler about like food, and then I just found that I have granola bar in here.
[47:52] That is exciting. 'Cause I don't wanna stop working on this.
[47:56] I'm like, I feel like I'm getting somewhere. (upbeat music)
[48:01] (upbeat music) (upbeat music)
[48:06] (upbeat music) (upbeat music)
[48:11] (upbeat music) (upbeat music)
[48:16] (upbeat music) (upbeat music)
[48:21] (upbeat music) (upbeat music)
[48:26] (upbeat music) (upbeat music)
[48:32] (upbeat music) (upbeat music)
[48:37] (upbeat music) (upbeat music)
[48:42] (upbeat music) (upbeat music)
[48:47] (upbeat music) (upbeat music)
[48:52] (upbeat music) (upbeat music)
[48:57] (upbeat music) (upbeat music)
[49:03], I didn't think anybody wanted to hear me eat, so, at least y'all were on mute for a minute.
[49:13], I didn't think anybody wanted to hear me eat, so, at least y'all were on mute for a minute.
[49:42] Is anyone doing anything fun today? You know what's going, I'm going a bit out of order.
[49:52] Yes, all right, all right. What are you like building Jay?
[50:04] Like, what are you working on getting it to do? Oh, wait, I wanna do this.
[50:12] Oh, okay, that is always fun. [50:26], what is this cute little thing?
[50:40] Oh, okay, that is always fun. What is this cute little thing?
[50:45] (upbeat music) (upbeat music)
[50:51] Ooh. (upbeat music)
[51:10] Nice, I need to follow you on GitHub. I don't know why I don't.
[51:16] Well, I'll follow Python Community News and then I need to go follow you as well.
[51:22] I mean, join us on Mondays, we're learning Python with Laura
[51:28] and eventually one day Jay will be on here too. and eventually one day Jay will be on here too.
[51:38] Ooh, fun. Oh, I finally found your GitHub,
[52:02] there, followed. I hope employers don't look at my GitHub
[52:07] and I'm like, Jen, no one follows you. I'm like, well, I just got it back.
[52:16] So my old one, I had like three followers. Oh, nice.
[52:24] (upbeat music) I did the things, I did the things.
[52:39] I follow and do the things and the YouTubes and all of it. Yes.
[52:51] (upbeat music) On GitHub, oh, do I have one now?
[53:11] I should go back and look. Actually, I think I have GitHub over here.
[53:18] (humming) Does anybody ever like just clean up all the,
[53:28] I got a follower, yay, homie, thank you. Does anybody else like just clean up
[53:40] all of their repos at times? 'Cause I feel like I wanna do that at some point.
[53:46] (mouse clicking) I am in the proper folder.
[53:51] I don't know what this is gonna do. Need to install the, yes.
[53:57] Did it update it? Did it add it?
[54:04] Might take a moment, all right. (mouse clicking)
[54:18] Oh yeah, I was gonna do this, makes it easier to stream with and I forgot.
[54:25] Oh, damn, yeah, that makes sense. Oh, yes.
[54:42] So really funny, when Tyler gets swag, I just like opening boxes.
[54:49] It doesn't matter what the box is. If he gets a delivery, even if it's like medication,
[54:53] I'm like, can I open the box? But when he gets swag, I'm like a happy swagger.
[55:00] And yesterday he got a webcam cover. Very excited for this.
[55:05] I need to put it on my laptop when I'm done streaming today, yay.
[55:10] (mouse clicking) Okay.
[55:14] Did it not, oh, oh, you installed it in it, but I didn't want you, eh.
[55:27] (mouse clicking) (sighs)
[55:33] Mm. (sighs)
[55:49] (mouse clicking) (sighs)
[55:54] (sighs) (mouse clicking)
[56:22] Mm. (mouse clicking)
[56:46] Mm. (mouse clicking)
[56:49] Mm. (mouse clicking)
[56:54] Mm. (mouse clicking)
[56:57], mm. (mouse clicking)
[57:01] Mm. (mouse clicking)
[57:28] Mm. (mouse clicking)
[57:31] (thuds) (mouse clicking)
[57:52] It's good. (mouse clicking)
[58:00] This is frustrating. Do you all know if my web app is not in the same folder
[58:10] as Prisma, if, I'm gonna delete this, if it'll work, 'cause it didn't install it.
[58:27] It installed it as its own folder instead of putting it with everything else.
[58:33] And I need to connect the two now. Anybody know?
[58:38] I don't. Why I keep breaking stuff, I don't know.
[58:46] (mouse clicking) Oh, maybe it'll work.
[58:58] Pages. Mm.
[59:06] (mouse clicking) Okay, well, we will find out.
[59:16] (mouse clicking) (laughs)
[59:37] I know, I know. I actually have been, I looked at Jays
[59:42] as one of the examples, like straight up, it is on my notion board of like, Jays, one of the examples.
[59:48] But I got something on there at least. What page is this?
[60:03] (upbeat music) Is this the index file one?
[60:06] (upbeat music) [60:09], (sighs)
[60:14] (upbeat music) (sighs)
[60:39] Mm. (upbeat music)
[60:45] Oh. (upbeat music)
[61:12] I need that. (upbeat music)
[61:15] I need this. I don't want it though.
[61:21] (upbeat music) (sighs)
[61:33] (upbeat music) [61:35], (sighs)
[61:40] (upbeat music) (upbeat music)
[61:47], (sighs) (upbeat music)
[61:54] Ah, yay. (upbeat music)
[62:18] (sighs) (upbeat music)
[62:22] (sighs) (upbeat music)
[62:38] (sighs) (upbeat music)
[62:43] (sighs) (upbeat music)
[62:47] (sighs) (upbeat music)
[62:52] (sighs) (upbeat music)
[63:16] (sighs) (upbeat music)
[63:20] Hmm. (upbeat music)
[63:45] (upbeat music) Hmm.
[63:56] (upbeat music) (upbeat music)
[64:01] (laughs) I get what you were saying by like,
[64:25] as long as it connects to the database, then it should be fine that it's in a different folder.
[64:30] And I'm just not sure or seeing how to get the information submitted here
[64:40] to put into the database. Oh, wait.
[64:46] Is this it? No.
[64:55] Let me close this one, close this one, close this one. And.
[65:01] We were in the Prisma. No, we were in index.
[65:15] Yes, we were in index.js. And then I also have a,
[65:24] oh, here we go. Oh.
[65:32] So index.tsx is the web, the web app.
[65:44] And then index.js is, (upbeat music)
[65:50] Hmm. (upbeat music)
[65:53], (upbeat music) (upbeat music)
[66:01] (upbeat music) (upbeat music)
[66:24] (upbeat music) (upbeat music)
[66:52] (upbeat music) (upbeat music)
[66:57] (upbeat music) (upbeat music)
[67:02] (upbeat music) (upbeat music)
[67:07] (upbeat music) (upbeat music)
[67:35] (upbeat music) (upbeat music)
[67:58] (upbeat music) (upbeat music)
[68:20] (upbeat music) (upbeat music)
[68:25] (upbeat music) (upbeat music)
[68:31] (upbeat music) (upbeat music)
[68:36] (upbeat music) (upbeat music)
[69:03] (upbeat music) (upbeat music)
[69:09] Oh. (upbeat music)
[69:32] (upbeat music) (upbeat music)
[69:37] (upbeat music) (upbeat music)
[69:42] (upbeat music) (upbeat music)
[70:12] This is challenging and teaching me so much. That's what it's supposed to do, right?
[70:26] Is teach me the things. And we...
[70:33] (upbeat music) (upbeat music)
[70:39] (upbeat music) Async function.
[70:59] It is TypeScript in my project, but it was what imported,
[71:10] which I am glad that I'm starting to learn TypeScript and I feel like I can figure that out.
[71:15] But the part I'm on right now is where to... So this is get data from the form,
[71:29] but I don't know. Oh, hey, send the form data to our API and get a response.
[71:34] (upbeat music) Maybe reading this out loud to you, I found it.
[71:43] We'll find out. (indistinct)
[71:47] (upbeat music) Any other requests, Jason data was created up.
[72:05] Tell us over, we're sending Jason. (upbeat music)
[72:10] Is this your... (upbeat music)
[72:31] (laughs) Yes, future me will be thankful.
[72:35] Right now me is annoyed, but in like such a good way.
[72:40] It's so weird. Like, I don't know how to describe this to people.
[72:43] I'm like, I'm having so much fun, even though I'm incredibly agitated at it.
[72:48] Cast the event target in HTML form. Const handle submit is declared value number read async.
[73:06] Get data from the form. So I'm going to do this because it's going to be...
[73:29] LetterHandle. Well, TypeScript, we will have on the show
[73:46] every other Friday. I just don't see.
[73:58] Yeah, it's weird because people are like, you're learning all of this at the same time.
[74:03] And it's not like I'm meaning to, it's because just the stuff that's coming up,
[74:08] I'm like, yeah, this is cool. (upbeat music)
[74:12] (upbeat music) (upbeat music)
[74:43] Oh, for TypeScript, it's Josh Goldberg. Let me.
[74:51] Oh, yay. Yes, thanks, homie.
[74:56] That is exactly who. I was about to go grab his Twitter.
[75:00] So thank you. Okay.
[75:04] Oh. Doggo, stop licking yourself.
[75:12] (upbeat music) I see you, ma'am.
[75:16] This is not what I wanted. So I broke something.
[75:24] (upbeat music) (upbeat music)
[75:29] That should be fine. (upbeat music)
[75:50] (upbeat music) It's probably one of those.
[76:03] (upbeat music) Okay, so I need this thing.
[76:18] (upbeat music) I don't need this one.
[76:29] I don't need this one. Oh, you're not gonna work.
[76:36] This one? Nope.
[76:38] (upbeat music) (sighs)
[76:45] (upbeat music) (upbeat music)
[76:50] Oh, you're so funny. It's not because of that.
[77:08] It's she licks her paws raw. She just like has a ton of allergies and things like that.
[77:16] So she just is like so mean to herself that she'll like cause herself to bleed and stuff.
[77:23] So it's not because we like don't want her to clean herself. It's just because of...
[77:28] Dammit. Why?
[77:33] Not safe. (sighs)
[77:40] (upbeat music) I just told you to save though.
[77:51] Save. (upbeat music)
[77:54] (sighs) (upbeat music)
[78:01] Where's the last thing coming from then? (upbeat music)
[78:08] (upbeat music) Ha!
[78:20] We are getting further. I feel like I'm getting like way too excited
[78:27] when I figure one thing out. I'm like, yes!
[78:29] Oh, geez. (upbeat music)
[78:35], (sighs) (upbeat music)
[78:44] (upbeat music) (upbeat music)
[78:49] (upbeat music) (upbeat music)
[79:14] (upbeat music) (upbeat music)
[79:19] (upbeat music) (upbeat music)
[79:25] No, that was wrong. (upbeat music)
[79:51] (upbeat music) (laughs)
[79:58] Have fun working. I don't think that was it.
[80:06] Oh, it is. Yay.
[80:08] (upbeat music) (upbeat music)
[80:14] (upbeat music) (upbeat music)
[80:19] Yay. (upbeat music)
[80:47] Glad to hear it. First or last name that I found.
[80:54] (upbeat music) Yeah, you know I want to.
[81:07] Are you guys doing Hacktoberfest? I need to do my Hacktoberfest stuff.
[81:16] I had two PRs and then I fixed my things. I got my official GitHub name back.
[81:28] What is this? (upbeat music)
[81:33] Nice, yay. (upbeat music)
[81:41] (upbeat music) Where is?
[81:46] (upbeat music) First name or last name not found.
[82:05] (upbeat music) Oh.
[82:09] (upbeat music) What up?
[82:19] You are joining on YouTube and my stuff just goes to YouTube by default
[82:28] so I don't have to re-upload it. But if you wanna come hang out with everyone
[82:33] in the conversation, we are over on Twitch. Twitch, oh, that's kind of fun.
[82:42] Twitch, Twitch, Twitch, Twitch. This is the Twitch info.
[82:48] (upbeat music) And by that I mean hack with the coding.
[83:09] Feel free to subscribe while you're there, you know, like any subscriptions too, but.
[83:14] Okay, well I can. I don't need a link.
[83:24] I just need this to be. (upbeat music)
[83:29] (upbeat music) (upbeat music)
[84:01] Oh, that is a very, very large name. (upbeat music)
[84:09] (laughs) Jay, what is diffusion B?
[84:31] (upbeat music) (indistinct)
[84:45] Interesting. (upbeat music)
[85:01] I don't even know if I know what that is. That's how.
[85:05] Oh, okay. That's cool.
[85:12] Oh, I downloaded an app that does that. I don't know how good it is, but it's called Wonder.
[85:27] (upbeat music) It's entertaining to say the least, but it's on my iPhone.
[85:32] It's not something down like on the computer, but it is pretty entertaining.
[85:37] (upbeat music) (upbeat music)
[85:42] There we go. Let's see.
[86:05] (upbeat music) [86:08],
[86:08] (upbeat music) [86:12],
[86:12] (upbeat music) (upbeat music)
[86:17] Go, go, leave yourself alone. Just moving around the room
[86:44] doesn't mean I'm not gonna hear you. (upbeat music)
[86:48] Oh, I don't know what happens in four minutes if it's, 'cause I need to take like at least like a 10 minute break,
[87:02] just to get away from the computer and make sure my posture is good.
[87:06] I know, she is so sweet though. She's just our sassy old lady.
[87:12] She's 12. So, all right.
[87:18] Get tagged in the weekly Twitter space. Mental health and neurodiversity and tech.
[87:25] Twitter handle. Okay.
[87:29] Now how to get stuff. (upbeat music)
[87:39] Cue that. Bro, ma'am, whatever you wanna be called, stop it.
[87:51] I'll put a cone on you. Yes, the poor doggo.
[88:01] She's been like this her entire life too. (upbeat music)
[88:07] I wonder. Oh, that's a good idea.
[88:33] I think I could maybe even add that as a, I mean, I could make that one of those Twitter list things.
[88:42] I've like, I found so many dope people. Jay is one of them.
[88:48] So. (upbeat music)
[89:00] Async function. So.
[89:18] (upbeat music) (upbeat music)
[89:24] (upbeat music) (upbeat music)
[89:29] (sighs) (upbeat music)
[89:53] (upbeat music) (upbeat music)
[90:14] Ah-ha. So this is where,
[90:24] I don't need this. (upbeat music)
[90:40] (upbeat music) (upbeat music)
[90:45] (upbeat music) (upbeat music)
[90:50] (upbeat music) (upbeat music)
[90:56] (upbeat music) (bell rings)
[91:25] Oh, that's what happens when the timer goes out. Yes.
[91:50] Oh, wow. I don't wanna talk to you.
[91:55] That thing scared me. What, why are you giving me so many ads, bro?
[92:02] I don't know why we have. Okay, here we go.
[92:09] This one, no. Oh, we were doing 95 minutes.
[92:16] I'm just gonna go look for a new one. That's fine.
[92:22] Let's see. YouTube.
[92:24] Yeah, I'm probably gonna take like a, I don't know, probably a half an hour break
[92:33] because I went for an hour and a half this time. So.
[92:38] (silence) I'm looking for one.
[93:02] They're all like very chill music too, which I'm like, uh, that's not always good, I feel like, I don't know.
[93:10] But this one is cool. So I will do this one, even though it's super chill.
[93:27] (silence) Let me get that going.
[93:40] And so we are not to have music now. Present, share screen, Chrome tab.
[93:49] Share audio. And we get the banner.
[93:57] BRB break time. And I will be back in 30.
[94:02] So y'all have fun. See you in a bit.
[94:06] (soft music) (soft music)
[94:20] (soft music) (soft music)
[94:24] (soft music) (soft music)
[94:40] (soft music) (soft music)
[94:45] (soft music) (soft music)
[94:50] (soft music) (soft music)
[94:55] (soft music) (soft music)
[95:00] (soft music) (soft music)
[95:05] (soft music) (soft music)
[95:10] (soft music) (soft music)
[95:28] (soft music) (soft music)
[95:48] (soft music) (soft music)
[96:09] (soft music) (soft music)
[96:33] (soft music) (soft music)
[96:38] (soft music) (soft music)
[96:56] (soft music) [96:58],
[97:01] (soft music) (soft music)
[97:06] (soft music) (soft music)
[97:27] (soft music) (soft music)
[97:32] (soft music) (soft music)
[97:38] (soft music) (soft music)
[97:49] (soft music) (soft music)
[98:03] (soft music) (soft music)
[98:23] (soft music) (soft music)
[98:28] (soft music) (soft music)
[98:32] (soft music) (soft music)
[98:49] (soft music) (soft music)
[98:55] (soft music) (soft music)
[99:12] (soft music) (soft music)
[99:25] (soft music) (soft music)
[99:39] (soft music) (soft music)
[99:59] (soft music) (soft music)
[100:14] (soft music) (soft music)
[100:30] (soft music) (soft music)
[100:47] (soft music) (soft music)
[101:08] (soft music) (soft music)
[101:22] (soft music) (soft music)
[101:44] (soft music) (soft music)
[102:00] (soft music) (soft music)
[102:20] (soft music) (soft music)
[102:47] (soft music) (soft music)
[102:59] (soft music) (soft music)
[103:22] (soft music) (soft music)
[103:39] (soft music) (soft music)
[103:57] (soft music) (soft music)
[104:18] (soft music) (soft music)
[104:34] (soft music) (soft music)
[104:46] (soft music) (soft music)
[105:00] (soft music) (soft music)
[105:17] (soft music) (soft music)
[105:45] (soft music) (soft music)
[106:02] (soft music) (soft music)
[106:11] (soft music) (soft music)
[106:28] (soft music) (soft music)
[106:49] (soft music) (soft music)
[107:07] (soft music) (soft music)
[107:24] (soft music) (soft music)
[107:42] (soft music) (soft music)
[107:52] (soft music) (soft music)
[108:05] (soft music) (soft music)
[108:24] (soft music) (soft music)
[108:37] (soft music) (soft music)
[108:47] (soft music) (soft music)
[109:07] (soft music) (soft music)
[109:26] (soft music) (soft music)
[109:38] (soft music) (soft music)
[109:51] (soft music) (soft music)
[110:11] (soft music) (soft music)
[110:23] (soft music) (soft music)
[110:35] (soft music) (soft music)
[110:52] (soft music) (soft music)
[111:07] (soft music) (soft music)
[111:29] (soft music) (soft music)
[111:42] (soft music) (soft music)
[111:54] (soft music) (soft music)
[112:16] (soft music) (soft music)
[112:43] (soft music) (soft music)
[113:07] (soft music) (soft music)
[113:27] (soft music) (soft music)
[113:40] (soft music) (soft music)
[113:52] (soft music) (soft music)
[114:08] (soft music) (soft music)
[114:28] (soft music) (soft music)
[114:49] (soft music) (soft music)
[115:17] (soft music) - What up, y'all?
[115:29] I'm coming from Brock, Brock. I'm coming from Brock early.
[115:34] Coming from break early. So, get that music paused.
[115:42] I get everybody else may not be back, but I got my tea, basically.
[115:49] Like I'm gonna get tea and then I wanna get back to work. Weird how that goes.
[115:55] I honestly, in a million years, didn't like realize how much I would really enjoy coding
[116:03] and like figuring this out. Now that I have like an idea of what to make,
[116:06] I'm like, yes, hello again. How is your AI stuff going, Jay?
[116:17] Okay, I have a new music to do. And we go to share screen.
[116:26] This screen. This one.
[116:31] (soft music) I went with jazz this time.
[116:38] So, we'll. (soft music)
[116:43] I'm digging it so far. Yay.
[116:50] Are you gonna show us any of them at some point? Or like, how do we get to see them, Jay?
[116:55] - Okay. (soft music)
[117:01] - Yay. Yay.
[117:23] (soft music) [117:26], I'm gonna do this.
[117:28] time. (soft music)
[117:31] How do I do this? (soft music)
[117:52] (soft music) (soft music)
[117:57] (soft music) (soft music)
[118:02] (soft music) (soft music)
[118:07] (soft music) (soft music)
[118:20] (soft music) (soft music)
[118:33] (soft music) (soft music)
[118:38] (soft music) (soft music)
[118:52] (soft music) (soft music)
[119:02] (soft music) (soft music)
[119:18] (soft music) (soft music)
[119:37] (soft music) (soft music)
[120:04] (soft music) (soft music)
[120:09] (soft music) (soft music)
[120:15] (soft music) (soft music)
[120:39] (soft music) Oh no, I want.
[121:03] (soft music) (soft music)
[121:10] Sorry. (soft music)
[121:18] (soft music) (soft music)
[121:22] (soft music) (soft music)
[121:27] (soft music) (soft music)
[121:32] (soft music) (soft music)
[121:37] (soft music) (soft music)
[121:42] (soft music) (soft music)
[121:47] (soft music) (soft music)
[121:53] (soft music) (soft music)
[121:59] (soft music) (soft music)
[122:14] (soft music) (soft music)
[122:36] (soft music) (soft music)
[122:41] (soft music) (soft music)
[122:45] (soft music) (soft music)
[122:50] (soft music) (soft music)
[123:09] (soft music) (soft music)
[123:34] (soft music) (soft music)
[123:58] (soft music) (soft music)
[124:03] (soft music) (soft music)
[124:08] (soft music) (soft music)
[124:38] - Oh, I don't have a syntax here. (soft music)
[124:42] Okay. (soft music)
[124:48] Okay. That is okay.
[124:58] Oh wait, where'd it go? So.
[125:04] (soft music) I think it would just be here.
[125:26] (soft music) (soft music)
[125:31] Undefined? What is it?
[125:44] Oh. Why is it undefined?
[125:54] Oh. Well, bye, Jay.
[125:58] Have a wonderful day. Thanks for coming and hanging out for a bit.
[126:02] Hopefully I can catch your stream later. (soft music)
[126:07] Why is this undefined? You're getting it.
[126:18] Why is this showing up? Undefined.
[126:21] (soft music) [126:26],
[126:29] Oh, that's probably why. (soft music)
[126:46] Object, object. That's not what I want either.
[126:57] Oh. (soft music)
[127:01] (indistinct) (soft music)
[127:09] (upbeat music) Oh.
[127:29] (upbeat music) That's hard.
[127:32] (upbeat music) (upbeat music)
[127:37] Can you use response data there? (upbeat music)
[127:56] Oh, right. (upbeat music)
[128:01] (upbeat music) Oh.
[128:10] (upbeat music) (upbeat music)
[128:21] (upbeat music) Okay.
[128:49] I know this is wrong, but I wanna see what happens. (upbeat music)
[128:54] Rude. (upbeat music)
[129:02] Maybe this? (upbeat music)
[129:08] Do you like that better? No, you don't.
[129:09] Okay, cool. (upbeat music)
[129:13] (upbeat music) Okay.
[129:30] (upbeat music) (upbeat music)
[129:35] (upbeat music) (upbeat music)
[129:40] (upbeat music) (upbeat music)
[129:46] (upbeat music) (upbeat music)
[129:51] (upbeat music) (upbeat music)
[130:03] (upbeat music) (upbeat music)
[130:14] (upbeat music) (upbeat music)
[130:23] (upbeat music) (upbeat music)
[130:37] (upbeat music) (upbeat music)
[130:47] (upbeat music) (upbeat music)
[131:07] (upbeat music) (upbeat music)
[131:16] (upbeat music) (upbeat music)
[131:29] (upbeat music) (upbeat music)
[131:39] (upbeat music) (upbeat music)
[131:58] (upbeat music) (upbeat music)
[132:18] (upbeat music) (upbeat music)
[132:37] (upbeat music) So.
[132:50] (upbeat music) (upbeat music)
[132:55] (upbeat music) (upbeat music)
[133:25] Oy, progress. Progress is not progressing as much as I would like it to,
[133:34] but it is progress. Where I think I need to,
[133:55] (laughs) Yes.
[133:58] I'm just trying to figure out like how to put this into work together,
[134:21] which is becoming difficult. 'Cause this one.
[134:33] Ooh, I wonder if I could do, import index.js.
[134:45] (upbeat music) Index.js.
[134:49] Yeah, I don't think that'll work. (upbeat music)
[135:14] (upbeat music) (upbeat music)
[135:19] (upbeat music) (upbeat music)
[135:24] (upbeat music) Well, Prisma works with the rest of it,
[135:53] so why wouldn't this work with the rest of it? (upbeat music)
[135:59] (upbeat music) (upbeat music)
[136:05] (upbeat music) (upbeat music)
[136:10] (upbeat music) (upbeat music)
[136:15] (upbeat music) (upbeat music)
[136:20] (upbeat music) (upbeat music)
[136:25] (upbeat music) (groans)
[136:54] (upbeat music) So, if I did import type from index.js,
[137:09] import type, ah, from index.js, ah, from index.js, import, ah, from index.js, ah, from, ah,
[137:17] ah, index.js,
[137:23] import. (upbeat music)
[137:38] (upbeat music) (upbeat music)
[137:43] (upbeat music) Ah, um,
[138:10] (upbeat music) for it's, ah,
[138:19] (upbeat music) (upbeat music)
[138:26] (sighs) (upbeat music)
[138:42] (burps) (sighs)
[139:07] (upbeat music) I wonder, could I done?
[139:12] (upbeat music) (upbeat music)
[139:20] (upbeat music) (upbeat music)
[139:25] (upbeat music) (claps)
[139:46] (upbeat music) (upbeat music)
[139:51] (upbeat music) (upbeat music)
[140:10] (sighs) (upbeat music)
[140:21] (upbeat music) (upbeat music)
[140:26] (sighs) (upbeat music)
[140:37] (upbeat music) (upbeat music)
[140:55] (sighs) (upbeat music)
[141:15] (upbeat music) (sighs)
[141:20] (upbeat music) (upbeat music)
[141:25] (sighs) (upbeat music)
[141:52] (upbeat music) (upbeat music)
[141:57] (upbeat music) (upbeat music)
[142:02] (upbeat music) (upbeat music)
[142:07] (sighs) (upbeat music)
[142:32] (upbeat music) (sighs)
[142:47] (upbeat music) (upbeat music)
[142:52] (upbeat music) (upbeat music)
[143:16] (upbeat music) (upbeat music)
[143:21] (upbeat music) (upbeat music)
[143:27] (sighs) (upbeat music)
[143:52] (upbeat music) I don't hang out on a specific Discord,
[144:13] but I do have Discord. You can be my friend.
[144:21] Be my friends, it'll be great. Why am I so stuck on this?
[144:27] I just wanna let y'all know that I just asked Twitter if somebody knows this stuff really well
[144:38] and saying that I need an adult, 'cause I'm not feeling very adulty right now.
[144:43] (sighs) (upbeat music)
[144:51] I don't know. (sighs)
[145:01] (upbeat music) (upbeat music)
[145:16] (upbeat music) (upbeat music)
[145:21] (upbeat music) (upbeat music)
[145:46] (upbeat music) Twitter, please don't fail me right now.
[146:06] Yay! (upbeat music)
[146:15] (upbeat music) (upbeat music)
[146:20] (upbeat music) (upbeat music)
[146:25] (upbeat music) Okay, Discord is making me like fill out,
[146:57] asking me if I'm human. And it's putting in like pictures of ducks
[147:02] and I think geese together. And I'm like, wait, I need a...
[147:06] I feel like that's not fair. (upbeat music)
[147:14] (upbeat music) But we are friends.
[147:29] I don't know, whatever. All right, I'm gonna figure this out.
[147:37] Once I stare at this for a while and try to figure out why, how.
[147:46] (upbeat music) (upbeat music)
[147:55] Okay. Time for some more Googles in...
[148:25] (sighs) Connect, type, set form to database.
[148:44] Connect, type, set form to database. (upbeat music)
[148:54] (upbeat music) Prisma, maybe?
[149:02] (upbeat music) (upbeat music)
[149:07] (upbeat music) (upbeat music)
[149:12] (upbeat music) (upbeat music)
[149:20] (upbeat music) I don't like this area.
[149:50] Okay. (upbeat music)
[149:53] What if I did... Import.
[150:04] (upbeat music) Hmm.
[150:07] (upbeat music) Import something from...
[150:29] (upbeat music) Next, form app, forward slash.
[150:38] (upbeat music) Form.
[150:48] (upbeat music) Forward slash, AP.
[150:58] (upbeat music) Pages.
[151:02] (upbeat music) Forward slash, API.
[151:07] (upbeat music) Forward slash.
[151:10] (upbeat music) Oh, hey.
[151:19] Hello. Hello, hello, hello.
[151:25] Hello, everyone. Yay.
[151:28] Welcome to me figuring out some, lots of fun stuff. I feel like y'all probably need to know from the beginning
[151:37] and it gives me a minute to try to get unstuck. So give me just a second.
[151:45] Hope y'all are having a beautiful day. All right.
[151:51] So this is my first time working on building a... Oh, it's actually a different...
[152:03] I just realized that. Brian, that Git is actually the old one
[152:09] because yesterday I had to completely restart from scratch. It was so fun.
[152:15] So Raiders, we are looking at... I have never made an app before,
[152:25] like full, like front, full stack. And I really wanted to, and I have,
[152:32] and let me post this now. And I want to use my visual skills
[152:43] of being able to conceptualize it and put it into code. So what I do is every Wednesday I host a Twitter space
[152:51] for mental health and neurodiversity in tech. And so many people have been like, yo, can you like tag me?
[153:00] Make sure that, you know, I'm alerted for this. I'm like, yeah, sure.
[153:04] 'Cause I was new to Twitter like three months ago. So the way that I'm able to keep that going
[153:11] is by I wanted to make these both go together and then auto-tweet.
[153:18] So basically people put in their Twitter handle, I entered a Twitter space link and whabam,
[153:23] they go together. And well, that is not going as easily.
[153:30] As easily as I thought it would building this because I'm learning a lot of different things.
[153:37] And as a heads up, you are on the stream for Teach Gen Tech. I have been streaming for almost four months.
[153:46] So it has been a bit of, before that I barely knew what like HTML and CSS was.
[153:54] So now I'm actually going through and building this like full stack app that I'm.
[154:01] That was fun. That was super fun.
[154:24] No idea why that happened. It was just like, okay, bye, but I'm back.
[154:31] So hello again. All right, let's try re-explaining this.
[154:37] Share screen, StreamYard, that was not very friendly of you.
[154:42] (laughs) It was trying to get you to like get excited about it,
[154:50] but then go, oh God, what happened? Okay, back to this.
[154:56] Thank you for following by the way. And thank you all for the love and support
[155:02] because this is, thank you. Thank you.
[155:06] So now that totally threw me off though. I don't know what I was talking about.
[155:13] Oh, I built in this app and I've been doing it in Prisma to my SQL.
[155:18] So I have a database to the Twitter API to autopost. And then I'm trying to do the front end.
[155:23] Well, I realized that in the order of things, that doesn't really work.
[155:30] So I'm currently using, I did get Prisma working
[155:38] and I was able to query the database, but then I was like, oh, I need forms.
[155:45] So I made it. So that way we could get to install the forms
[155:53] app, but now I can't get that to connect to my database, which is where I have been stuck for a while,
[156:02] but I did get it prettier. Get tagged in the weekly Twitter space and you hit submit.
[156:11] And it still says undefined, undefined. And I have the index in the next format.
[156:20] And then I have also the index in the main file that I'm just,
[156:29] and I'm new to TypeScript that this has been a huge learning opportunity.
[156:37] And yes, thank you for all of the follows and love. And thank you for rating over.
[156:45] I feel like I'm also, is it shell? I feel like I'm gonna butcher your name.
[156:51] So I'm like, awkwardly not saying it. How do I say your name?
[156:57] 'Cause A, you're cool for coming over. B, you just, I like coding people and I wanna be friends.
[157:05] I'm gonna follow you back though. Shell, shell.
[157:19] This is like the thing that I hate about the fact that on streams, it doesn't have like the sounds.
[157:29] So that just means like one day, you'll just have to come on my stream and tell me,
[157:38] and you'll be on Teach Gen Tech sometimes. That could be cool, right?
[157:42] I think it would be cool. What do you mostly stream about?
[157:46] (upbeat music) Now I really wanna say not.
[157:57] I think it would be so cool to learn like beginner to Ruby. I like seeing like the differences.
[158:11] I just learned a bit about Go. And John, nice.
[158:19] Yeah, what is that, John? It's an object of something, of something.
[158:30] Well, I'm gonna go follow you on, I feel like you definitely shouldn't have said not Kale,
[158:38] because now I really wanna call you not Kale, just 'cause I think that's a really cool name.
[158:44] Interesting, where, where is the things? Oh, I've only been streaming for a few, yes.
[159:09] Yes, I've only been streaming for a few months now, and that is something that I think is so fun,
[159:21] is like when people have their pages set up, and I'm like, dude, I don't have mine set up at all.
[159:30] Like, look at this, look at the not, look at not Kale's set up.
[159:35] They actually have it all, all set up, and I love it. And I need to do that on mine sometime,
[159:42] so I will definitely get there. Okay, well, I,
[160:01] yeah, I was just, just thinking the same thing. Not gonna lie, y'all, I, I'm like, I don't know how to,
[160:25] mod mute people. I'm gonna get there, though.
[160:32] (gentle music) Oh my goodness, bro, like,
[160:39] I mean, you're definitely making me like level up. (laughs)
[160:46] You can tell I'm a newbie streamer, newbie streamer. I am, like, curious, while I work on doing this whole thing,
[161:02] what does everybody, what were y'all working on on the last one?
[161:08] You said that you were doing a, contributed to Casa by, that's pretty cool.
[161:17] All right, thank you. Thank you, that was fun.
[161:30] All right, thank you, Ryan, for helping me figure that out. Do any of you know TypeScript or Prisma?
[161:39] Because I literally just said on Twitter that I need an adult, which,
[161:45] just saying, I do, I do. 'Cause that is, I don't know,
[161:55] how long do y'all, like, get stuck on stuff? Since starting this, I'm like,
[162:01] I've been working on this for a few days now, but it is my first one.
[162:05] So I've been working on my Googles. I feel like, I don't know if it's TypeScript
[162:19] or just not knowing databases well enough, 'cause, like, yesterday we worked on
[162:25] the query and setting up the database, which was interesting in itself,
[162:33] and we were able to query it. Let me close these out.
[162:36] I have, like, too much going on at the moment. 'Cause I was able to set that up with Prisma
[162:42] and get it connected to MySQL, so it's definitely getting there,
[162:50] but it's way, way. Prisma, wait.
[163:03] Index as function, export default function. (playful music)
[163:20] Yay. Yes, we do work on TypeScript every other Friday.
[163:36] And for anybody that likes Python, we do that every Monday.
[163:40] So, not Kale. (laughs)
[163:43] That's why I'm excited to have you on, like, maybe about some Ruby,
[163:46] because that's gonna be pretty dope. Oh, the issue is,
[163:54] probably the way I did this, but I set up Prisma and in Node,
[164:04] which did let me use my database and set it up. So, set up the database.
[164:12] Then I was like, oh, I need a front end to be able to put this in.
[164:18] So, to be able to put into the database, and which I came up with the Next Forums app,
[164:26] and I got that working for the most part, but I don't have the two working together.
[164:31] Like, if I enter something on this get tagged weekly for Twitter space,
[164:36] it doesn't connect to the database. But I think that's because Next Forums
[164:44] came after the database. And I don't know.
[164:55] And what I was thinking of doing is trying to, like, combine this index.js
[165:02] with the index here, because that's what it was under.
[165:09] But I'm also not sure what order I would do that in. But give me just a second.
[165:19] Let me commit this, so that way people can actually go look at this
[165:25] without me going to so many different screens. And as a heads up, everybody,
[165:31] if you do go look at this, it is something that I do have a lot of,
[165:36] like the API information or keys public. Right now, I'm just learning.
[165:41] Once I actually get this fully up and running, I will make everything private
[165:46] and nobody will be able to see it. And you should be committing.
[166:04] And as soon as this does want to load, here is my GitHub.
[166:11] Why do you take so long? Although this likes to freeze.
[166:24] I might have to reopen it. Fine, fine.
[166:30] Fine. No, and I think that's why it tends to freeze
[166:38] when I don't do that. And I just started doing it through GitHub instead of CLI,
[166:43] but sometimes it gets me a little mixed up. (gentle music)
[167:15] It's a good thing I'm save happy. I will say that.
[167:19] (gentle music) (gentle music)
[167:24] (gentle music) (gentle music)
[167:42] (gentle music) (gentle music)
[167:50] I don't know how to respond to that message. You need our help desperately at this point?
[168:06] Well, you just barely said hi. That makes it a bit awkward.
[168:14] (gentle music) Maybe I waited too long to actually commit.
[168:23] (gentle music) Right?
[168:34] I will say, when people are committing to like their branches
[168:44] or like uploading stuff, is anyone like, is this a really old joke with, I'm just scared to commit?
[168:49] And yeah, quick, what's going on?
[169:02] Like, how are you? Who are you?
[169:07] Please tell us more. (gentle music)
[169:12] (gentle music) Anybody know what Delphi seven is?
[169:22] That is not something I'm familiar with. (gentle music)
[169:31] I don't know what everybody else uses for music, but I use countdowns to be able to
[169:45] make sure that I take breaks. So today's is, or at least this 90 minutes is jazz.
[169:55] I'm just kind of having fun with it. It's good music.
[169:58] Please commit, bro. I know you're grumpy at me.
[170:08] I'm sorry. (gentle music)
[170:12] (gentle music) (gentle music)
[170:18] Oh, that's surprising. (gentle music)
[170:47] Okay, Jay. Thank you.
[170:49] Would you go already? Okay.
[170:59] We'll just do this thing again and put you on a new branch. (gentle music)
[171:11] (gentle music) I would really appreciate you working.
[171:36] (gentle music) Oh, my goodness.
[171:44] (gentle music) (gentle music)
[171:59] (gentle music) Interesting.
[172:28] Side note, I finally got it uploaded on GitHub, if y'all want to take a look at the repo now.
[172:38] I finally did it, which is exciting. But,
[172:44] I don't know. (gentle music)
[172:53] Quick, what are you going to school for? (gentle music)
[173:05] (gentle music) (gentle music)
[173:10] (gentle music) (gentle music)
[173:15] (gentle music) (gentle music)
[173:22] (gentle music) (gentle music)
[173:38] (gentle music) (gentle music)
[173:45] Okay. I'm just gonna try some random stuff.
[174:12] It's gonna be fun. (gentle music)
[174:16] Let's see. I'm gonna leave that the same.
[174:27] (gentle music) So.
[174:33] (gentle music) Oh, okay.
[174:40] (gentle music) Oh, goodness.
[174:55] There's somebody I follow on Twitter that would probably be really, really good to reach out to.
[175:00] And of course, I hate when this happens, but I just like blank what their name is.
[175:06] (gentle music) Yay, I'm glad.
[175:23] Yeah, we try to keep it chill. (gentle music)
[175:32] I am J and Tuck, J Taylor. I've been on a few of his Twitter spaces.
[175:44] There's a delivery, y'all. Thank you, babe.
[175:52] Love you. It's cookies.
[175:55] Cookies. Gluten-free cookies.
[176:02] (plastic crinkling) I'm excited.
[176:05] Yay. Okay, well, cookies aside,
[176:09] J and Tuck has done a few Twitter spaces with about security and things.
[176:17] So he has a lot of different guests on for Mentor Mash, which would be probably a good one to Mentor Mesh.
[176:27] I don't know why I wanna say mash. Whatever.
[176:29] (gentle music) As you follow and come to hang out, you will learn.
[176:36] I can't talk and I get in trouble for clicking things too quickly.
[176:40] Ryan, I don't know if you've started a counter. I don't think I've done it as much today.
[176:48] It's been a lot more typing than click-happy. (gentle music)
[176:55] ♪ Do, do, do ♪ I'm just gonna...
[177:02] I knew this. ♪ Do, do, do, do, do ♪
[177:11] Copy. (gentle music)
[177:14] (playful music) ♪ Do, do, do, do, do, do ♪
[177:20] (playful music) (playful music)
[177:32] (playful music) (playful music)
[177:41] (playful music) (playful music)
[177:49] And y'all, I have no idea if this is working. I'm just literally just trying random shit,
[178:06] see if I can get it to work, which is kind of fun when it comes down to it.
[178:14] (playful music) Oh, I don't remember how to run it now.
[178:24] How do I run you? Is it NPM start?
[178:30] (playful music) No, of course.
[178:36] (playful music) (playful music)
[178:41] Twitter API stuff, you can go away for now. Yay.
[178:58] (playful music) Run, let's see if that works.
[179:13] (playful music) Shit, CD.
[179:21] (playful music) How does that NPM run?
[179:37] I don't like this one. (playful music)
[179:42] Oh, it does, yay. (playful music)
[179:46] Oh. (playful music)
[180:01] (playful music) I mean, that is a very, very good.
[180:15] Bro, go, go back on mute. Like, go away.
[180:22] (playful music) This is a good quote in the fact that like,
[180:30] but, yes, but it's frustrating. This is probably like one of the cool things
[180:39] of doing Teach Gen Tech is I have somebody on the stream with me teaching it about it
[180:43] so I can ask questions. And I love that, yet at the same time,
[180:48] I know I need to do stuff like this because then I don't have somebody holding my hand,
[180:55] basically. Although when I get really stuck,
[180:58] it takes me hours to get unstuck. Okay, so Prisma Client cannot be run in browser.
[181:08] Is it because? Oh, this one's set up.
[181:17] (playful music) Thank you, Ryan.
[181:25] (playful music) (playful music)
[181:30] Okay. So that doesn't make sense.
[181:46] We can't have these in the same file. Okay, cool.
[181:50] Well, we tried it. Oh, no.
[181:57] (playful music) Dammit.
[181:59] (playful music) Index TST.
[182:04] (playful music) Connect index.tsx
[182:10] (playful music) to index.
[182:17] (playful music) Yes.
[182:21] (playful music) [182:24], Oh.
[182:25] (playful music) (sighs)
[182:30] (playful music) Oh.
[182:52] (playful music) Oh.
[182:57] (playful music) Okay, y'all.
[183:03] I don't know if Jay is still here. I also am not gonna be mad if anybody wants to,
[183:12] you know, go check out his stream because he just sent me the coolest video for his intro.
[183:20] Like what he was just working on. Let's expand.
[183:23] So y'all can see it. (playful music)
[183:29] I don't know if it has sound, but how cool is that? He was doing it with this AI tool that creates images.
[183:43] That's just really cool. I should do this.
[183:53] That is another thing that I definitely will be upping my game on is my streaming setup.
[184:01] 'Cause right now I use StreamYard and it crashed earlier and luckily,
[184:09] it just goes back and forth. That's fine.
[184:14] Right? It's cool again.
[184:17] All right, back to jazz music. (playful music)
[184:24] (upbeat music) (playful music)
[184:29] (playful music) (playful music)
[184:34] (playful music) (playful music)
[184:39] Import. Next form.
[185:05] Form. Data.
[185:17] Wow. Data.
[185:18] Two. Configuring forms.
[185:31] (playful music) (playful music)
[185:36] (playful music) (playful music)
[185:41] (playful music) (playful music)
[185:47] (playful music) (playful music)
[185:52] (playful music) (playful music)
[185:57] (playful music) (playful music)
[186:03] (playful music) (playful music)
[186:08] (playful music) (playful music)
[186:32] (playful music) (playful music)
[186:37] (playful music) (playful music)
[187:04] (playful music) (playful music)
[187:09] (playful music) (playful music)
[187:14] (playful music) (playful music)
[187:20] (playful music) (playful music)
[187:26] (playful music) (playful music)
[187:55] (playful music) (playful music)
[188:01] (playful music) (playful music)
[188:18] (playful music) (playful music)
[188:42] (playful music) (playful music)
[188:54] (playful music) (playful music)
[189:05] (playful music) (playful music)
[189:32] (playful music) (playful music)
[189:51] (playful music) (playful music)
[190:05] - All right, y'all. I have pretty good news.
[190:17] My next guest is Anthony, who I like to call my internet big brother.
[190:24] He's the one who really helped me get my stream up and running and like get into DevRel
[190:30] and helped make sure I had guests on the show. He also knows I've been really stuck on this
[190:37] and I'm also very stubborn in, I don't want help in time.
[190:43] No, I want help, but I am not always great about like I wanna make my own mistakes to learn.
[190:51] You know, it can be a catch-22. I am stubborn.
[190:55] I 100% will admit that. But he just said that he is willing
[191:01] to go over this with me later. So thank goodness.
[191:06] But here is his Twitter. So y'all should definitely go follow him as well
[191:11] because he is a good cookie to know. Yes.
[191:19] So on that note, I am almost done on this timer and I feel like I'm going in circles
[191:26] that I need to like take some time away. So do stay up to date and follow me on Twitch
[191:33] to get the updates next time. Yeah, as Ryan said, that is my,
[191:43] the GitHub because this makes it super, super confusing when I'm like layering all of this.
[191:53] But yes, please follow me on Twitter. You know, check out the repo.
[191:59] See if you have questions, let me know. And I will be back later, probably the stream,
[192:06] but I also have some homework I need to do for something else. So may not be today, but I do stream four days a week
[192:15] at 9 a.m. Pacific, 12 p.m. Eastern, and 1600 UTC, Monday, Tuesday, Thursday, Friday.
[192:25] And on Wednesdays, I have my Mental Health and Neurodiversity in Tech, which is the entire reason I'm building this app, Twitter Space.
[192:34] So, so, see you later all. Bye. Thank you for joining.

