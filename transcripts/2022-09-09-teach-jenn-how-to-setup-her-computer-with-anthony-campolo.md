---
showLink: "https://www.youtube.com/watch?v=xXmHbiYW1Uo"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-how-to-setup-her-computer-with-anthony-campolo"
title: "Teach Jenn How to Setup her Computer 😂 with Anthony Campolo"
publishDate: "2022-09-09"
coverImage: "https://i.ytimg.com/vi/xXmHbiYW1Uo/maxresdefault.jpg"
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

[00:00] - Hello, hello, beautiful humans. Welcome back to Teach Gen Tech
[00:05] and one of our returning visitors, Anthony, who is, is this your third time being on the show?
[00:13] I think so. - Yep, yeah. Yeah, are there any others who've,
[00:16] I'm sure Ramon's probably been on three or four by now. - Yeah, yeah, yeah.
[00:23] Well, we paired up doing some stuff with Taylor from Distributade and that was pretty fun.
[00:29] And then Laura will have her third time on, on Monday. And then yesterday I was just like,
[00:38] Ben, you need to come on like once a month, just so that way.
[00:41] I think accessibility is such a deep topic, but not something you can necessarily like consume
[00:47] really, really quickly. - You also have to fill four episodes a week.
[00:51] So that requires a lot of people. So you, if you can have people who can come on
[00:56] kind of regularly, then you can fill the slots a lot more easily.
[00:59] - Yeah, but like, I actually just talked to Mike over at Stripe.
[01:05] He's the one that I like to call, "Hey, you're not square." 'Cause I totally did that the first time we met.
[01:12] And it's something that, what up, Yare? We're setting up my computer today
[01:21] 'cause I just hard reset it. So I have Chrome set up so far,
[01:26] Discord, Snagit, Slack, and I definitely need to do my Bluetooth.
[01:34] But Mike from Stripe just gave me the idea to do like look up people's tutorials and do them.
[01:43] - Oh yeah, that's a great thing to do. - Although this is something I need to figure out
[01:50] about StreamYard is how to allow sharing the audio. And, but not something I have to figure out today.
[01:59] - What do you mean? - Like yesterday's with, with Ben,
[02:04] nobody could hear the accessibility stuff from the audio on the computer.
[02:11] Like Zoom, you know how Zoom's like, "Hey, share screen."
[02:14] And then, yeah, so. - Yeah, that's overall a good default
[02:19] 'cause the vast majority of the time you don't want your computer sounds bleeding in,
[02:22] but that's one case where you'd actually want to be able to do it, yeah.
[02:25] So I don't know. - Yeah, neither do I, but we'll figure it out.
[02:30] And let's see, I am uploading the overlay because I completed it.
[02:36] Vim, I don't even officially know what Vim is. Is Vim?
[02:41] - Yeah, so Vim is like an older editor. So you can kind of think of it like VS Code,
[02:48] but like a more pared down version that was more based around having specific key bindings
[02:54] to navigate around. So the thing that makes Vim different from most things
[02:58] is that there's times when you can move the cursor by pressing the keys,
[03:02] and times you can actually write stuff to it while you're typing.
[03:06] So there's like two modes that you can be in, partly because you're gonna navigate around a lot
[03:10] and when you work in like large files. So people build a lot of muscle memory around it,
[03:15] but it's also like takes a long time to learn and actually get proficient at.
[03:20] And now VS Code is just like so awesome and does so many nice things for you anyway
[03:25] that not as many people use Vim, but it was kind of like,
[03:28] if you wanted to be like a "serious programmer," you're like, I wanna learn Vim.
[03:33] - Yeah, okay, that makes sense. And Yeray, I like how you say that you're just trolling.
[03:39] And I'm like, it could have been a serious question that I didn't know yet, but you know.
[03:43] - Yeah, you should assume 90% of the time when people are talking about Vim, they're trolling.
[03:47] - Okay, good. And I'm almost ready to share my screen.
[03:52] And once I get my screens set up in the proper order. - Yeah, it's all good.
[03:58] - They are not, 'cause we are literally setting up my computer.
[04:04] It does not have like anything. Like I don't even have my Bluetooth keyboard paired.
[04:10] So it's, okay, did I do that right? Let's see.
[04:21] Oh, I hate this. Oh no, you are.
[04:27] I wish I could share my screen on this one, but it like goes to the actual screens.
[04:33] - So I can talk about what I was going to show you today. So I can fill some air while you're doing this, yeah.
[04:39] - While I'm just staring at my screen and no one can see it.
[04:41] Thank you, thank you. - Yeah, well, the thing that we had talked about,
[04:47] Mike brought this up, Mike Havalier on his next episode about just like useful snippets and like stuff
[04:53] that will kind of make your life easier and more productive. So it's gonna be partly that
[04:58] and partly just getting you this stuff installed to allow you to have these useful snippets.
[05:02] 'Cause some of these are using like the GitHub CLI, which you need to install.
[05:06] And to install that you need Homebrew, so you need to install Homebrew.
[05:09] And so I have a gist that has a couple little formulas that will run through.
[05:14] And then when we're done, 'cause I might edit it along the way,
[05:17] you're gonna fork it. And then anytime you install anything else,
[05:20] you're gonna write it in that gist. So then you will have a record
[05:24] for how your machine is set up. If every single programmer in the entire world did this
[05:28] for everything they installed, everyone's dev machine would be perfectly reproducible
[05:32] every single time. That to me sounds like utopia.
[05:36] - Interesting. All right, so I am pretty sure I got my screens
[05:40] at least set up properly. Really?
[05:46] - I don't want it to twitch actually. - No, I don't wanna leave the site.
[05:50] I need to update my system preferences. Oh my gosh.
[05:54] - And so some of the snippets will also will be like initializing a Git repo and then like pushing it up
[06:03] to a GitHub repository with like a single command or like setting up a Postgres database.
[06:08] These are things that you probably don't have a lot of, some things you won't have a lot of context
[06:13] on like why you'd need it yet. But in like a month or two,
[06:16] you're gonna be in a situation where you're gonna have to spin up a Postgres database.
[06:19] And you'd be like, wait, Anthony told me how to do this in the real life.
[06:22] - And that's probably the thing I'm really excited about is like when you talk to people that are like,
[06:27] "Hey, I'm gonna get up and running and I wanna start coding."
[06:31] It's like, what do they need on their machine? Because that is something that I have found
[06:36] it was really, really confusing. - Have I told you the story of when
[06:42] no one could get my dev machine working when I was in my bootcamp?
[06:46] This is actually a ridiculous story. My node was like so broken that
[06:51] we couldn't figure out how to like run local dev, like local host, like on my computer.
[06:56] Like you would run NPM start or like Yarn start and then nothing would happen
[07:00] and there'd be no error message and everyone was baffled. And this went on for like two months.
[07:05] And then eventually I realized what it was. I was messing around with this stuff
[07:09] before I knew what anything was. So I kind of knew to my machine before I even got there.
[07:13] I had a single node modules folder, like a stray one in my like root, like user directory.
[07:19] So every time I'll be in a project and try to run a command node would get confused
[07:23] 'cause it would try and find the original node modules 'cause it like does this hierarchy thing
[07:27] to like find the node modules. And so by deleting the node modules
[07:31] in the root of my computer, then I was able to all of a sudden use it.
[07:35] And like, it was so specific and so ridiculous and like multiple people at the bootcamp looked at this
[07:41] and tried to figure it out. Like, I don't know.
[07:44] So what I did was I used code sandbox, like you've been doing.
[07:47] I would code a code sandbox, put it in a Git repo and then deploy that Git repo to Netlify.
[07:53] And then that's what I would show for like when I used to turn it in.
[07:55] 'Cause most people, they would like share their screen and they would run on their computer
[07:58] and they would kind of like click through it where I'll be like, I have a link.
[08:01] And so it's like, it actually was better 'cause it meant I had like a deployed website
[08:05] and other people didn't. But it was like a really crazy way to get there.
[08:08] - I honestly like appreciate so much because Yeray was the one that introduced me
[08:16] to code sandbox. And I'm just like, dude, that is actually really cool
[08:21] how you can see it so quickly without having to like go through and download it all.
[08:30] I think it was really hard to, and it's hard for a lot of newbies
[08:35] to be able to see that and like understand what they're actually doing.
[08:39] - Yeah, 100%. Yeah, there's like multiple good online IDEs.
[08:45] Now you should try out StackBlitz next. It's like a newer kind of more modern version
[08:50] of code sandbox and it's really great. - I'm just still having problems sharing my screen.
[08:59] - So what exactly is the problem? Like what's happening?
[09:04] You need to use your words, you can't show me. - It wants me to restart Chrome,
[09:12] which will end the live stream. - Can you make me like the co-host or something
[09:18] so it stays on? - I don't know.
[09:21] - 'Cause I think if someone stays on, hold on, let me first see if I can be--
[09:27] - 'Cause it won't end the stream. I just, I need to restart Chrome.
[09:31] - I mean, only one way to find out. You can also open it in a different browser.
[09:36] - I tried that. Well, I tried, well, let's try Safari.
[09:42] Maybe, I can't use that. - What was the other one?
[09:45] Did you try Firefox or what other browser did you have? - I tried Incognito instead.
[09:52] - Oh, cool. That means you weren't logged in.
[09:55] Yeah, so that would, yeah, no, don't do that. - Yeah, yeah, yeah, I'm, you know, thinking about this.
[10:00] Um, oh, set up shareability is so amazing. I'm like late to the show.
[10:07] Uh, Gary, I, Gary, what do you wish that you knew when you first started coding?
[10:14] Like, I don't think I ever asked you that when you were on the show.
[10:18] I don't know. That was, can you believe that was two months ago?
[10:22] Like, seriously, that is crazy. - But crazy time flies when you're coding.
[10:30] - Fucking code. - I mean, I had named tons of things
[10:34] that I wish I knew earlier. I wish I had learned more about HTTP
[10:38] and like what a GET and a POST are. That would have been super useful.
[10:43] And I wish I had actually learned the Fetch API instead of using Axios 'cause Axios is like a library
[10:48] that's really nice and like kind of wraps the Fetch API. So it kind of hides most of it from you.
[10:52] So you don't really know what the heck's going on. - Please stand by because I need to download Firefox
[10:59] because StreamYard does not allow, does not work with Safari.
[11:07] - I mean, it doesn't work with Brave either. So it doesn't surprise me.
[11:10] - This is the episode of me struggle busing setting up my computer.
[11:16] - Does that mean you searched for answers on Yahoo? - That is pretty good.
[11:25] - I guess you would search like bulletin boards back in the day.
[11:29] - Forums, all that. - You really need to find something.
[11:33] IRC chat. Things that existed before I was alive.
[11:37] - All right. So let's try this again.
[11:46] We are going to go to StreamYard. - We haven't crashed yet, so that's good.
[11:53] - That is good. We are at least getting in the right direction.
[11:57] (heart beating) - And this is something that I was told quite a few times
[12:06] that people actually love about, like live streams is when people mess up.
[12:14] And I'm like, y'all, I'm messing up. You just can't see it yet.
[12:17] We'll get there. - Yeah, this is not as much, this is not as reverting
[12:20] 'cause they're not seeing like a debugging process. That's more so what people find interesting.
[12:26] - Agreed. Okay.
[12:28] - 'Cause then you can see how people think through like what happens when you try and actually build something
[12:32] that isn't like something that someone already built for you or like kind of chart a path out for you.
[12:37] - Exactly. Okay.
[12:39] We are... I remember.
[12:41] Okay. Okay.
[12:45] Mute this one. Stop the camera on this one.
[12:53] Okay. And I think this one will still work.
[13:02] - Cool. Okay, well you dropped off but it survived.
[13:15] - Yeah, I'm on Firefox now. - Sweet.
[13:21] - So, oh. - Feedback.
[13:25] - I mean, if I can just get it working from here, I'm gonna do that but I think we're gonna find out.
[13:32] - I'm gonna share my little gist in the chat so people have something to look at while this is going on.
[13:40] - So they have something to do other than just listen to. - Yeah, but I'm also gonna get your whole Node deal set up
[13:48] 'cause I'm gonna have you install Volta, set your Node version, install Yarn and PMPM.
[13:56] So then no matter what project you get thrown at you, you will have the tools necessary
[13:59] to run that stupid JavaScript project the way that particular dev decided to make you do it.
[14:04] - Oh, well, Yare, have a wonderful day at work and thank you for sharing.
[14:10] - Yeah, thanks for stopping by. - And after all of that, it took me 15 minutes
[14:16] just to share my screen. Safari just started sharing it instead of Chrome.
[14:22] So I'm just gonna stay in Safari for now and I can do stuff in Chrome if needed.
[14:26] I still need to set up my fucking Bluetooth. It's okay, it's okay.
[14:32] All right, so you said that you shared the gist already? - I'm about to, just making sure the outline links all work.
[14:42] Oh, that one's not there. - All right.
[14:54] - All right, there it is. And I shared this on Twitter when you tweeted this.
[15:00] - Sweet, let's see if I can recalibrate to the proper, all this stuff going on.
[15:10] (computer whirring) Oh my gosh.
[15:16] And I hate that like StreamYard. Okay, I'm not just trying to bash on StreamYard right now,
[15:20] I'm just struggle bussing. You also can't like copy and paste things from StreamYard.
[15:28] You have to go through, yeah. - You can from the comments thing on the right.
[15:34] - It won't, it'll just, it won't copy and paste, it'll just let you show it or not show it.
[15:41] It might be different for you since you don't have access to showing and unshowing.
[15:46] - Yeah, maybe. I feel like I can write comments.
[15:51] You said there's no input, like where you can type text. Are you on private chat or comments?
[15:57] - On comments, on comments you can't copy it. On private chat you can.
[16:04] Will you paste it in the private chat instead of me trying to go find it since I can't?
[16:09] Because my Twitter's not logged in either, and neither. - Just type it out.
[16:15] - Obviously, it's a perfectly reasonable URL. - I am struggling this morning, y'all, if you couldn't tell.
[16:21] All right, so. - It's okay, what we're actually gonna do
[16:25] is you're just literally gonna run a bunch of commands that I've already written for you
[16:28] to see if it's the least stressful thing you could ever do. - Yes, all right.
[16:33] And hopefully we also get VS Code working to actually open the--
[16:38] - Yeah, we should do that before any of this. - Okay, so I haven't even downloaded VS Code yet.
[16:43] Like, it's literally-- - All right, well, you gotta download that then, right?
[16:46] Right now, don't download brackets. - I think, does brackets come default or, no.
[16:54] Oh, if anybody wants a really good hairdresser, Brandy is it, so.
[17:01] But no, I don't have brackets yet, so that's good. - Yeah, 'cause it's just, there's no need.
[17:05] Like, you're never gonna use another, it's highly unlikely you're gonna use
[17:09] another editor anytime soon. Unless you meet some WebStorm people
[17:17] and they really convince you. - Maybe one day, you never know.
[17:21] Maybe one day. Elise, while that's downloading,
[17:31] I can do all the really annoying stuff of-- - Bluetooth it up.
[17:35] - I got the Bluetooth going. Now I just need to remove all this stuff
[17:39] from my dock that I don't use. - I always get so confused when I use someone's computer
[17:46] that has the dock on one of the sides. So I'll go down, like, why doesn't it work?
[17:52] - Yeah, no, I hate it being at the bottom. Oh, no, I just, options.
[17:58] Move from dock. Chrome's good, those are good.
[18:01] It's so small right now, it's like sad. It's like all the icons are so big because of,
[18:07] I don't have all the stuff in there that I normally do. - Yeah, I find a more amenable dock keeps you saner.
[18:16] - Probably, probably. Well, for everyone that's gonna be watching this,
[18:23] we are downloading and installing VS Code, which I just Googled VS Code and got to the download.
[18:31] - Yeah, so that's one thing I could include in this gist, but right now I don't.
[18:36] There's no links or really any kind of, these are just straight instructions,
[18:41] but I'm kind of assuming that people either know what these are or I'm gonna explain them
[18:45] as we go, so if anyone's particularly curious, this will be a good record of.
[18:50] And these are things that I do every day, super-duper common things, so yeah.
[18:56] - I do think it should be where. - You're gonna need to make that way bigger.
[19:03] - Yeah, that you show getting VS Code going and then installing Prettier,
[19:12] 'cause that's also something that a lot of people forget, is installing Prettier and that kind of stuff.
[19:18] - So there's a thing here with, when you're using a CLI to like Prettier,
[19:22] you don't need to install Prettier on your computer. You can have Prettier just inside of a project,
[19:27] like in the Node modules, and run it with NPM or Yarn, and I think you should do that for the vast majority
[19:34] of the CLI tools you use. So like, I even do that with Netlify and Vercel's CLIs.
[19:40] So there's only like a handful of ones that I'm gonna show you, that's because they're not like
[19:45] things you just put in an NPM project, they're more so like, they're just more complicated,
[19:50] but so you need to use Brew, but for the most part, if you're globally installing NPM stuff,
[19:57] you wanna think hard about that, and here's the reason why, 'cause then,
[20:01] one, if you assume someone else has that on their computer, they may or may not, whereas if you put it in the project,
[20:06] everyone who clones that repo gets the same dependencies every time,
[20:10] and then you also don't have to worry about having to update the CLI on your machine,
[20:15] 'cause every time there's a new version, your CLI stays the same,
[20:20] there's not like automatic updates usually, so you have to like manually upgrade these things,
[20:25] but if you're just creating new projects and putting it as a dependency,
[20:28] every time you download it as a dependency, it'll pull the latest version.
[20:32] - Got it, okay. I wonder if everybody does that?
[20:38] - The global versus dev, so it's a hot topic, people have different opinions about each,
[20:45] most people will agree that using it as a project dependency is just like more stable and just like more dependable,
[20:51] because it's like, it cuts out the variability of developers' machines, which is like, for me,
[20:58] I think always a good thing, because as we're seeing here through this process,
[21:01] there's a lot of steps to set this stuff up. Everyone sets up their machine differently,
[21:05] everyone has different opinions about even how they should set their machine up.
[21:08] So if you make the project have to decide that, then it's all self-contained and you clone a repo
[21:14] and the things are there you need, you don't need to worry about installing
[21:16] these extra CLIs on your machine. - I will say, I am very, very grateful that
[21:26] like your tokens, if you have like something on your phone to do that, they're not messed with.
[21:31] - You're waiting by your tokens on your phone, like for a two-factor?
[21:36] - Yeah, for two-factor. - Yeah, well, you can do two-factor
[21:40] through your one password, and I think that's a really bad idea,
[21:43] 'cause then if your one password ever gets hacked, your passwords and your two-factor are both screwed.
[21:48] - That is also something that needs to be on somebody's to-do list of best practices,
[21:54] because I don't even have that set up, and that's something that I talk about for a long time.
[21:59] - If you just stop everything you're doing right now, you need to get a password manager.
[22:02] - Yeah, I will, I will. We'll add it to the to-do list,
[22:05] but I don't wanna take up that much time, 'cause we only got like 40 more minutes.
[22:10] - Dude, do you know how long it takes to install one password?
[22:13] Like five seconds. - Fine, I'm going.
[22:22] - What up? - Nice.
[22:25] - Okay, I'm doing it on like the DL over here on my extra screen, 'cause--
[22:29] - Yeah, no, don't show anything for the password. - Y'all don't need to see that shit.
[22:34] - And from now, we will refer to it as LastPass, just to really mess with people.
[22:39] But yeah, this is gonna, you want this to be in your workflow now,
[22:46] because you're gonna have so many things you gotta sign up for with so many passwords,
[22:49] and you're also gonna have API keys, and you're gonna have, eventually,
[22:53] probably multiple emails attached to different things, and you can also keep your credit card information
[22:57] in one password and use that to fill out forms when you're buying stuff online.
[23:02] It's like, that's super sweet. Also, there's like, this doesn't matter to you,
[23:05] there's tons of crypto wallet functionality too. So one password is one of the most amazing pieces
[23:11] of software I've ever used, and it's transformative. - I used it before at a previous company,
[23:20] but I never used it at the same time. - And that's the thing, is you have to actually
[23:27] get in the habit of using it, 'cause it also will autofill data on most websites.
[23:32] You should always assume 10% of the time, one password's just not gonna work,
[23:36] 'cause they can't make it work with every website on the entire internet, but most of the important ones,
[23:40] you just will click it, and it'll say, all right, I can autofill this for you,
[23:43] and then you click it, and then you log in, so. - Yeah, it was really convenient with things
[23:50] that were like, shared passwords. I thought that was really cool.
[23:58] - That's exactly what Nate's saying right now, is that I also, we also, I got my partner on 1Password too,
[24:03] so that we could share a bunch of stuff, and share like, you know, like Hulu accounts,
[24:07] and things like that, you know? And you just put like, straight up taxes in there
[24:12] if you want, put anything, like environment variables, like if you have environment variables
[24:17] for a certain project, it's a good place to save that as well.
[24:20] Just make sure you keep, so you're gonna have to create a master password though,
[24:26] and this is important, you're gonna wanna like, write it down on a piece of paper,
[24:30] and then put that in a safe deposit box somewhere. - Yeah, I was just about to say, I better write this down,
[24:35] 'cause I'm not gonna remember what I just created. - What's cool though, is that they prompt you
[24:39] to always have to do it at least once every two weeks, so you don't go six months without ever doing it,
[24:44] and then forget it for the rest of your life. They kind of force you to have some sort of like,
[24:48] repetition so you don't forget it, which is very smart. - Yeah, I found my, I found the sticky notes.
[24:55] - Is that your Arnold? - Yes, yes.
[24:59] - I mean, it was good, I could tell, so. Successful impression.
[25:05] - Yes. - I would just say, "Get to the chopper."
[25:10] - Okay, now I have to actually type it properly. (keyboard clicking)
[25:19] I think this is truly though, like people don't think about this,
[25:24] or like know where to start with this. It's something--
[25:28] - This, referring to password management, or just setting up your machine?
[25:32] - Both. - Yeah, no, totally.
[25:34] Yeah, I think password managers are starting to become a little more mainstream for some people.
[25:39] Like I know a lot of people who use like LastPass, and things like that,
[25:42] and if they're not necessarily developers. But I also know a lot of people that are like my dad,
[25:49] who like every one of his accounts had like one password, which was like his mother's maiden name,
[25:54] and like two numbers. So it was like the easiest thing to hack ever.
[25:58] And if you use it for all the same things. Actually, have you ever checked,
[26:01] have I been pwned to see if you're in any data breaches? - No.
[26:07] - Yeah, this is a really useful website. They actually integrate with a one password,
[26:11] to where if like a company's whole thing gets hacked, and it gets like posted in like a data dump,
[26:17] they will notify you if yours is in that record, and let you know, hey, you should change your password.
[26:24] - Oh, that's dope. Okay, I finally have one pass set up.
[26:29] - Awesome. - Okay, so now that that's done,
[26:33] I have VS Code, I got my terminal up. I know we need to create a folder as well on my desktop,
[26:40] to make that the default. - Not on your desktop.
[26:43] - Don't recreate the bad default, I've already been telling you to change.
[26:47] - Why do you think I like double checked with you beforehand?
[26:50] - So before we do that though, we should figure out the... Actually, yeah, let's do this.
[26:55] So make a directory right here, that is one word code, all lowercase.
[27:01] - What's the command for creating a directory? - MKDIR, you're making a directory.
[27:11] Yep, and just code one word, all lowercase. Okay.
[27:16] - Enter. - Now, every time you open your terminal,
[27:18] you will type cd code and you'll be there. You won't do cd desktop, cd code folder
[27:24] with capital C, capital F and a dash in between. - If y'all couldn't tell,
[27:31] I've been frustrating Anthony with my strings. - But now you're gonna understand why now,
[27:37] and every time you're gonna open your terminal and you're gonna thank me.
[27:40] - Yes, yes. I am a little sad because I was thinking about
[27:45] backing up all my projects, but I was like, at the same time, I'm like,
[27:48] you know, if I really wanted them, I'm gonna go watch the stream and recreate it.
[27:53] - This is also why you should get in the habit of every time you have a project,
[27:56] push it up to a get repo, like at the end of the day, and then just delete it off your computer.
[28:00] Like, I don't keep any projects on my computer 'cause then I'll lose work and do stupid stuff with it.
[28:05] So I always push stuff to a get repo, straight up delete the repo,
[28:08] and then when I wanna work it on again, I clone it down again and then work on it.
[28:12] Which seems like tedious, but it's like, for me, it's infrequent enough and saves me the headache
[28:18] of having to track projects on my computer. So yeah, that's also 'cause I don't do projects
[28:24] with like 20 environment variables, which would be kind of a different story.
[28:27] - This is also something that I'm gonna put as my best practice written down.
[28:34] (computer beeping) What's the best practice that you're writing down?
[28:43] - The upload to get hub, upload your repo. - Ah, right, yeah.
[28:49] And that's one of the things I'm gonna show you how to do. - Yay!
[28:53] These are things that I definitely have not been doing. And I'm kind of sad 'cause I just realized
[28:57] that I never went back and I think uploaded two of them that I actually should have kept, but that's okay.
[29:04] - Yeah, for me, I ended up not having, actually, no, I still have my Lambda stuff,
[29:08] but I kept it all hidden away and it's not public. But for the most part, like once you become intentional
[29:15] about using a get repo, you'll like think more about like when a project is actually like in a state
[29:21] where it can be pushed to a get repo. So it's a good thing to do.
[29:24] And then you'll just start to like have a collection. 'Cause also you're gonna have a repo for a lot of episodes.
[29:28] So you can have like, what Ben does for semantics is every episode has its own page on the semantics website
[29:34] that then has links to all the stuff they do that includes the repo and if they built a thing.
[29:39] And so that's also really useful. - Yeah, I'm still trying to get used to like balancing
[29:44] all of that too, so yay for best practices from everybody else.
[29:49] All right, what are we doing now? I guess I'll just go.
[29:53] - Okay, so now go into your code folder. - Okay.
[29:56] - And then pull up that gist. - Do, do, do, do, do, do, do, do, which went somewhere.
[30:03] So to do this, and I haven't done this very much. So that's gonna be like the hard thing to remember too
[30:11] is what up? - So bump it up like two and then also shrink it in.
[30:18] So it's not taking up your whole monitor. 'Cause you're gonna want to kind of keep this on the side
[30:23] while your other stuff is happening. - Cool.
[30:26] - So it can be like maybe just like 30% of the screen. - Yeah.
[30:30] Sure. - That's good.
[30:34] And then I would do the terminal kind of up to the very top left and take up like 20% or so.
[30:41] And then your code editor takes up the rest. Yeah, I would shrink your terminal down a bit
[30:51] from a height wise, if you're gonna need more space to kind of see code usually.
[30:58] - I think this is like what everybody would be a lot happier with for.
[31:06] - You could probably bump up the gist another one. And so you see here, I have an outline for you.
[31:12] So if you click any of these links, they'll send you to that part, but don't do that yet.
[31:15] Let's just look at the outline. So there's gonna be setup scripts to like install stuff.
[31:21] And those are gonna be first homebrew, which is the thing that lets you install
[31:25] most of the other things. And then a couple of these like JavaScript CLI things,
[31:30] you've already used NPM and you've already used Yarn. There's another one PNPM,
[31:35] which you may encounter at some point. So I'm just gonna put it on your computer.
[31:40] So it's not gonna break anything or do anything if you don't use it.
[31:43] - Thank you. - And then we'll install the GitHub CLI.
[31:47] So that's like really useful for, as you see, like when you do get now, you do like get in it
[31:52] and you create the repo and all that stuff. And then you go to github.com, create a repo
[31:56] and then do this whole dance where you try and figure out how to actually get it up on there.
[31:59] Like you've done that a couple of times now, right? Yeah, and everyone does.
[32:04] 'Cause the GitHub CLI didn't even exist until like two years ago.
[32:08] So they're like, wait, let's just build this. So now there's a single command you can run
[32:12] that will do the entire thing all at once. - Oh, okay, cool.
[32:16] - Yeah, and then there's, I'm gonna give you the Railway CLI 'cause it's like the dopest deployment platform ever.
[32:23] And it'll be a way for you to run containers, no servers, Postgres databases, other kinds of databases.
[32:30] Like you're gonna encounter many projects throughout your entire career that are gonna be,
[32:35] Railway will be useful for. And then fly, which we won't actually do anything with today.
[32:40] That's another one might be worth learning kind of down the line.
[32:44] - Okay. - That's pretty much it.
[32:46] And then two kind of like small utilities I like. One is HTTP stat, which lets you run basically
[32:53] like a request for a website. And then it gives you like the times of like when you do,
[32:59] like when you do your dev tools and you're like looking at how long is it takes
[33:02] for a website to like load and show up and that kind of stuff, right?
[33:05] It gives you kind of a nice clean visualization of that. And so that's a good one.
[33:10] And then tree, which allows you to just write the tree command and it prints out the directory structure
[33:15] of your projects that you're in. - Oh, that's cool.
[33:19] - Yeah. - Dope, okay.
[33:21] So to do this though, I'm gonna, no, I'm just gonna click through this.
[33:29] I'm not gonna create the gist into my own yet. - Don't do that yet.
[33:32] Yeah, yeah, we'll do that at the very end. Yeah.
[33:34] - The setup scripts. - Yeah. - Yay.
[33:36] - So you're gonna have to kind of copy that whole first line and nothing else there.
[33:41] 'Cause there's three commands here and you gotta run them each one after the other.
[33:47] So this is running the install script for homebrew. - I'm gonna make sure it doesn't show.
[33:55] I don't think it will, but you know, just to. - Yeah, that should be fine.
[33:59] - Okay. Done.
[34:06] - That's great, enter. And this might take a second.
[34:12] So go ahead and just copy the middle one. That can kind of tell you what's happening with that.
[34:19] Kind of just scroll over a little bit so people can see it.
[34:21] - Yeah. - So this one, this is setting your port, I think.
[34:30] Get mine up. - So just so everybody knows,
[34:36] like Anthony had me install a lot of this before my first live stream.
[34:41] Like he just sent me these and he was like, "Just go install these."
[34:44] And I was like, "I don't even know what these are." So I like that we're like finally talking
[34:48] about what I was installing. - No, this is good 'cause if I tried to explain this stuff
[34:52] to you at the time though, you would have had no context. You would have been more confused.
[34:57] - Yes, yes, definitely, definitely. - Yeah, 'cause what this is also doing right now
[35:04] is this downloading. I see how it says downloading command line tools for Xcode.
[35:09] So this is like, and this is why if you check out my gist, if you scroll to the very top of the gist
[35:15] where there's the title of the gist, I'm very specific here with this title
[35:18] 'cause this is very important information. All of these things and whether they're gonna work or not
[35:22] has to do with the fact that I am on one, a Mac OS, two, I'm on a specific version, Monterey,
[35:28] and three, it's an M1 chip. So it's a new chip that a lot of like some things
[35:33] just break for, break because it's so new. - Do you think it's backwards compatible?
[35:37] - What do you mean? - If it's the old chip.
[35:42] - Are you, so you're on a non M1 computer, I'm assuming? - Yeah.
[35:46] - For now, what we're doing, it shouldn't matter. It would matter more if we were doing Docker,
[35:53] but we're not. - Yeah, 'cause it is something that I'm on the Intel.
[35:59] - Okay, nothing I'm doing should be specific to that specifically.
[36:03] It's the only times I really see it become a problem is like I said, with Docker 'cause Docker builds binaries
[36:10] based on your operating system. So they had to basically rebuild everything
[36:14] to work with the new chip. And so stuff like Prisma will break
[36:18] and just like Docker itself, like you need to use this like build X command
[36:22] and pass in like an extra variable to tell it which architecture you're on.
[36:25] So it's just another thing to kind of have to worry about. But if you are someone with an M1,
[36:30] you get to like QA everyone's tool, make sure it works on M1 and then let them know
[36:36] when things break 'cause that's kind of fun. - So you're actually the first one I've really heard
[36:42] that uses Windows. Almost everyone else.
[36:45] - There's more of them than you think. They're more of a silent majority type.
[36:50] - Oh, like almost everybody's been like, "Oh yeah, I have a Mac too."
[36:53] And I'm like, "Oh, okay." - That's because you talk to a lot of successful
[36:57] and well-paid developers. - There are dozens of us.
[37:01] - There's a selection bias here 'cause with Windows it's just cheaper.
[37:06] And so a lot of people are just gonna buy a Windows computer automatically
[37:10] 'cause they have less money. And it has been like a dev thing forever,
[37:16] like Windows and DOS going back decades. So it makes sense.
[37:21] The problem is so many, like you were saying, so many people who do like dev rel kind of stuff,
[37:26] like we all have like apples. There are people who are on...
[37:29] Like if you have an open source project and there's 10 people on the team
[37:32] and all 10 of them have Macs, no one will know if things break on Windows
[37:36] until a user who's not on the team uses it on Windows. And then it says, "Hey, why is this broken on Windows?"
[37:42] Like, "Well, we didn't test it on Windows." - Yeah, that makes sense.
[37:46] And Windows is fine either one, install WSL or two. - That's Windows system or subsystem Linux.
[37:56] - Oh, WSL two and install stuff with... - Windows subsystem for Linux, yeah.
[38:04] - Wingit, I was trying to say... Like Win ET or something.
[38:13] - Yeah, so Wingit, let's see. That's a Windows package manager.
[38:18] So that's, I would assume fairly similar to what you're doing right now with Homebrew.
[38:22] Homebrew is a Mac OS package manager. Oh, look at that.
[38:26] That's what Nikki's saying right now. - So I do have like just a random curiosity question
[38:33] for everybody while this is installing. A, do you drink coffee?
[38:40] Because I only started drinking coffee again like a month ago because coffee used to make me
[38:46] so sick to my stomach, I couldn't drink it. And now I can drink it again.
[38:49] - Have you ever tried caffeine pills? - Yes, yes.
[38:54] And well, that works. And if you drink coffee, what do you put in it?
[39:02] - One cream, no sugar. - Okay, okay.
[39:08] I put dandy blend and cacao powder in mine. - Cacao, that sounds like something other gen,
[39:16] or your other gen, I guess. But I think-
[39:19] - Your gen, your gen would. Yes, I adore your gen.
[39:23] She's the best. - Indeed.
[39:26] Okay, this is still downloading. Are you sure?
[39:28] - It's still installing. - Scroll down and make sure.
[39:31] Yeah, I guess the Xcode takes a very long time. So let's kind of, we can do some other stuff
[39:36] in the meantime. Let's scroll down to the, let's go to the GitHub one.
[39:41] - No, no, no. - Yeah, right there.
[39:44] You scroll past it. Yeah, so create and push a public GitHub repo.
[39:49] So can you zoom in actually? And then just open your thing up
[39:53] so people can kind of see it while this is still installing.
[39:57] - Wait, what? - Yeah, exactly, yeah.
[39:59] 'Cause that's why I wanna talk through this, 'cause there's the thing,
[40:01] I'm doing a lot of stuff in that GitHub. There's a single GitHub CLI command happening here,
[40:06] but I'm passing it like six flags. So it does all the things I want it to do.
[40:10] This is my proudest moment writing a command that did exactly what I want it to do.
[40:15] So if you look at gh-repo-create, so that's like the base part.
[40:19] You're saying, I'm gonna create a repo, and then you give it a name.
[40:23] So you could just do that. You wouldn't need to do anything else in this command,
[40:27] and then it would kind of walk you through questions of, do you want it to be public?
[40:30] Do you want the source to be your current project? Do you wanna set a description for it?
[40:35] Do you wanna set the remote? And then do you wanna push it?
[40:37] So you could answer those five questions, or you can already know ahead of time
[40:41] what the answer to those questions are gonna be, fill it in, and run this one command to basically create it,
[40:47] set the remote, create a description, and then push it all at the same time.
[40:54] - Okay. - So does that make any sense at all?
[40:56] - I think where I'm lost is, so when this is done, it's gonna.
[41:04] - So it'll spit out a link for you. That is github.com/jenjanad/github-cli-example,
[41:13] 'cause that's the name you gave it. So since you're giving it a name,
[41:18] you already know what the URL is gonna be. It'll spit it out for you anyway in the terminal,
[41:22] so you just click it, but you can know ahead of time. Actually, it's always just gonna be your username/
[41:28] the name of the repo, and you're creating the repo.
[41:30] The first thing you do is you give it a name. So that's the URL.
[41:33] - Oh, that's cool. - And I also use that as the name
[41:40] of the project on my computer, the name of the repo, the URL,
[41:44] and then the URL for the subdomain on Netlify or Vercel when I deploy it.
[41:48] So there's a consistency across those three things, and I don't confuse myself
[41:52] by having three slightly different names for everything. - That's the other thing,
[41:56] is I really do wanna name everything like, you know, X person is cool,
[42:01] but I do need to start naming them the actual project name. - No, you need just the topic.
[42:04] You can put the name and the topic. - Ooh, question for you, Anthony.
[42:11] How do you backdate on GitHub? - I mean, you shouldn't for the most part.
[42:18] Ideally, if you use like Git and GitHub the way they're intended,
[42:23] you're always just saving history and not like rewriting history.
[42:26] So if that's what you mean by backdate, like how do you like change dates on stuff
[42:30] or maybe put things that weren't originally on GitHub, but were in like a Git repo?
[42:35] Okay, he's saying, I'm not sure what he's saying. He's saying yeah, too.
[42:39] So I do not mess around with like rewriting Git history and stuff like that.
[42:44] It's a thing you can do, and like technically anything you see in a Git repo,
[42:49] the history and the commits could all be entirely made up. There's nothing stopping you
[42:53] from just like writing whatever you want and just text files.
[42:55] But for the most part, and especially if you're using like GitHub
[42:59] and you're authenticating with the CLI, there's like, you have like authentication
[43:04] associated with every commit. So that's stuff where you kind of just want to just like,
[43:09] just get into your workflow. If Git were magic,
[43:13] changing history is considered a forbidden spell. That's a very good way to put it, yeah.
[43:18] Yeah, you can do it. You probably shouldn't.
[43:19] So just make sure you have a really good reason to do it. - Yay.
[43:26] - Yeah, and then let me just see real quick if I can actually find the command on that.
[43:29] So it would be, here's a stack overflow.
[43:34] For you, Git commit amend, no edit date, bam. Why don't I post that in the chat?
[43:40] I think that is what you're getting at. Okay, it looks like it's still going, still downloading.
[43:52] This is also because you're streaming actually. When you're streaming, you download way slower,
[43:57] but this is okay. So let's go back to this.
[44:00] - I was just showing a bit of what he just posted, what you just posted.
[44:05] Whoever I'm talking to, that, the link. - So we can start making this project
[44:11] and go all the way up to the GitHub command at this point. - Okay.
[44:17] - Nikki is actually, you should show Nikki's link up on the screen.
[44:21] This is why you need a chat overlay. - Yep, probably.
[44:27] - Yeah, I mean, lots of people need chat overlays, so. But what I do is I actually open the Twitch chat
[44:33] while I'm screen sharing and then have it in the corner. So it's just, it's like having a chat overlay,
[44:38] but it's just like a browser window. So it looks tacky, but the chat is there, you know?
[44:42] - Oh, interesting. I really do.
[44:46] - So do you know how in Twitch you can do forward slash chat after someone's name to just get the chat pop out?
[44:53] - Oh, no. - Yeah, so let me,
[44:56] this is really useful knowledge to have about Twitch. So I'm gonna drop this in where I am, where I met her.
[45:04] So if you follow that link, you will get to the chat and just the chat.
[45:08] So then you could bring that-- - It's magic. - You could bring that onto your screen now if you wanted.
[45:19] - Yeah, okay, hold on. - Especially people dropping links and stuff.
[45:25] It's good when people are watching these things back to be able to actually reference what's happening.
[45:30] - This is happiness. - Yeah, well, I'll make it a lot bigger.
[45:34] - I'm getting there, I'm getting there. Please stand by.
[45:39] - Yeah, and what I usually do is then I would have that be like the bottom right,
[45:44] and then the gist would be most of the top. So which one's on top or bottom
[45:50] isn't particularly important. - All the fancy things, all the fancy things.
[45:56] - Well, this is just me trying to figure out a way to do this and like without having to actually build a chat overlay
[46:01] and maintain that and like work it in 'cause it's not straightforward at all with StreamYard
[46:06] or even possible as far as I know. - I don't know how, I wanna get rid of these.
[46:11] - Oh, yes. - Yeah, go to kick the back button, I think.
[46:18] So you're looking at your GIF subs right now. Here, open it up for a second
[46:21] so you can kind of see what's happening. - Yeah, I did.
[46:25] It's just not going away. - Okay, well, try refreshing.
[46:28] There you go. - Okay, no, see, it comes back to me.
[46:41] - So this is what you can do, this is what you do. Okay, scroll your thing up, open the window up
[46:46] and then just have the browser above it covered. - Oh, bam.
[46:49] - They're windows, you can do anything you want with them and you put them anywhere on your screen, any combination.
[46:57] - All right, so we got the hello from the streams and what's the point of deleting stuff?
[47:07] Oh, got the big brain going. Just started using, let me go back to the first one.
[47:14] Now I got too many going on. That's the point where I go deleting stuff in DevTools.
[47:21] Does that work? - I've never tried to delete anything.
[47:25] If he means Chrome DevTools, yeah. Oh, I think he means just take it, kill it from the DOM.
[47:32] I'm curious then for this, this person just left this comment Zergling Soup, it sounds like they play StarCraft.
[47:42] Were you using another editor previously or is this just like the first time
[47:47] you're using a code editor? - I'm giggling at the fact if you were using brackets
[47:53] because you missed it. I have been called out many times
[47:56] that my default coder was brackets on my machine. - Well, it's just that like no one uses,
[48:04] I don't even, I'm not sure what, it's a, I think it's more. - I don't know, I have no idea.
[48:10] - Yeah, so when it comes to editors, you have 90 to 99% of developers use VS Code now.
[48:16] You have like 1% who use WebStorm and will like emphatically tell you over and over again
[48:22] why it's better and they don't manage to convince many people as far as I can tell.
[48:26] And then some people who use Vim, but you can use, you can do Vim stuff.
[48:31] You can configure VS Code to be like Vim. So a lot of people, they're still just,
[48:35] even if they used Vim, they'll set up VS Code so it's like they're using Vim
[48:39] and they kind of like emulate it. So that's why very, very few people do anything
[48:43] except VS Code. But I don't think that's gonna be the case necessarily
[48:47] forever 'cause it's still pretty new and there's always new things coming out.
[48:52] - And we got. - Okay, cool.
[48:55] Yeah, they said they'd use PyCharm. I use PyCharm once or twice.
[48:58] I tried to learn Python before I learned JavaScript actually, but it didn't go very well.
[49:03] - Join on every other Monday. So this coming Monday, I am learning Python.
[49:07] - Oh, yeah. - Yay.
[49:10] - Yeah, Python's fun. - It is pretty interesting.
[49:13] And I feel like, y'all, we only have 10 minutes left. I'm really sad 'cause this is like the one day
[49:20] I actually like have to end my stream, like have to end my stream on time.
[49:26] - Okay, let's do this. Let's stop talking.
[49:29] Go back to your terminal and open a do command tab to command T, I mean.
[49:34] - I was just gonna say command tab. - Sorry, no, command T, I meant.
[49:40] - You should just come back on on Tuesday, just saying. - Yeah, we'll see how far we get through this.
[49:47] This is the important one though. - In 10 minutes, we're in the rush.
[49:49] - So go back to the Git repo just, and close those up a little bit so they're both,
[49:55] so they're not overlapping on each other. Yeah, and so you're in your code folder.
[50:00] You're good to go. This is gonna be your first project in your code folder.
[50:03] So follow along with those. Here, you create a directory and then go into it.
[50:07] Yeah, and the dictionary pop-up thing is not super tight. - I just wanna turn you off.
[50:19] Turn off, turn off. - Oh, Grammarly, I see.
[50:24] - You know, Grammarly is really helpful for all of my articles and tweets.
[50:28] It is not helpful for this. - Yeah, Grammarly is, I think, an awesome tool.
[50:33] Imagine there's going to be a lot of writing, helping-like tools in many different ways.
[50:40] Okay, so then now this command is just gonna create a readme.md file with a single H1 that says,
[50:48] GitHub CLI example. So this command's a little complicated actually.
[50:52] So echo will take whatever is inside those parentheses and then add it to a file called readme.md.
[51:02] - Hmm. - So now if you go, so open this project now.
[51:06] Or actually, now we need to do the code period thing. - Well, oh, I don't think it'll work.
[51:12] - We can set that, it takes just two seconds. So. - Yeah.
[51:15] Well, I still-- - But we haven't set it up yet though,
[51:20] so it's not gonna work. So go to, let me look it up again real quick.
[51:24] - It's Command + Shift + P. I've had to do it many times. - You've done it so many times.
[51:28] - I've done it so many times. - So just do it, see what happens.
[51:31] - I don't remember which one it's called. - Hold on.
[51:35] - So y'all, just as like an update, my terminal would not open up the project in VS Code.
[51:44] Even though it was activated, I kept having to go back in VS Code
[51:48] and activate it each time beforehand. So that's why I remembered.
[51:51] But cool thing about VS Code is it remembers what you last used.
[51:57] So that's why I was like, oh, it's this one. - Okay, so you're gonna type shell and hit Enter.
[52:01] - Okay. We're gonna see.
[52:07] - And so close it out. - It'll probably work now. - Like, no. - We just won't, huh?
[52:12] - Well, okay, go for it, see what happens. - It opened. - There you go.
[52:17] - Now, is it-- - Yeah, and this trace is gonna have the same problem it did last time
[52:19] where it's not gonna work if we close everything down, but let's not worry about that now, let's keep going.
[52:23] - Yeah, I was gonna say, we'll try it next time, we'll find out.
[52:26] - Ah! Yes, I trust?
[52:31] - Yes. - That's random. - No, that's good, so did you, yeah, don't look.
[52:38] - I said yes, I said yes. - But did you check the box?
[52:41] - Yes, well, I think I did. I don't know. - Yeah, it was a little laggy.
[52:45] Okay, so now you can actually go look at the readme.md file. And then, so that's your H1.
[52:55] I'm not entirely sure. Nikki, I try not to mess too much
[53:02] with Zish and Bash config files and profile files, so I'm not super hip to all of that,
[53:09] but it's doing something, here, let me drop this. This is where I got-- - I'm also laughing.
[53:14] Anthony has literally been there seeing some really random shit.
[53:19] - So I went into Bash commands and broke, broke it, I completely broke it,
[53:26] that I was doing a live stream by myself. Anthony had to come on to help me figure it out.
[53:33] So I think this is technically your fourth time hanging out because-- - That's true, yeah.
[53:37] Three and a half, okay, let's-- - Three and a half, okay, okay.
[53:39] - Let me do the git init, git add command. Then you also know how to actually see
[53:47] a red markdown file in VS Code. So on the readme, where it says readme.md,
[53:56] to the right, there's the two panels with the magnifying glass at the bottom.
[54:02] Yeah, that one, click that, bam. - Yay! - So if you're ever writing
[54:07] a markdown file, you can see what the markdown's actually gonna look like,
[54:10] which is especially useful for links and images and syntax code, syntax highlighting
[54:14] and all that kind of stuff. - Oh, that is really cool.
[54:17] Okay. - Yeah, you have an entire markdown editor built into VS Code for you.
[54:21] - Okay, so I got the-- - Oh, let's do this also. So grab that command, git config-global init.default-branch.
[54:31] It's just the thing right in the middle. - Oh, okay. - Yeah, grab that whole thing.
[54:38] Sorry, starting from git config, though that's gonna copy-paste too much.
[54:44] Yeah, and then you're gonna delete name and write main, but without the brackets.
[54:51] No. - Yeah? - Yep, yep.
[54:58] - Yay! - So this will ensure now that every time you create a new repo,
[55:02] it's gonna be main automatically. - Oh, sweet, yay.
[55:06] And then now do I do git add? - Just real quick, just to make sure,
[55:10] do git branch-m and then main again. - Okay.
[55:16] - Make sure there's a space in after. So git branch space-m and then don't do it yet,
[55:24] I'm not done, then main. Yeah, there you go.
[55:30] Bam, okay. Now you can add and commit.
[55:33] And run git status in between so you can see what git status does.
[55:44] Yeah, so right now it's telling you you've added this file to the staging area
[55:48] and it is ready to be committed. So now you're gonna commit it.
[55:52] You're gonna do the thing. Yeah.
[55:58] And now run git status again. So now you see you have a clean branch, so that's good.
[56:07] You'll wanna run git status frequently when you're doing this stuff
[56:11] or else you'll get confused very easily. Let's see if you're still downloading Homebrew.
[56:15] Oh, it's so close, 100%. Unless there's more lines. - It's getting there.
[56:23] It's getting there. All right, and then do I need to do this one?
[56:29] - Hold on, so that's what we need to install, but you install it with...
[56:36] Okay, there's another way to install it. Okay, so go to cli.github.com.
[56:41] (keyboard clicking) And then click Download for Mac.
[56:50] I have no idea what this is gonna do, but click it and see what happens.
[56:56] - Do it. (mumbling)
[57:01] - Okay, cool, yeah, so it's just like... - Yeah, so I was afraid it was gonna do.
[57:13] - Okay, so we basically have to wait for this to do the next step and...
[57:18] - Well, there's another way we could possibly do it. Let's try 'em.
[57:21] - So we have like three minutes, so... - Last thing, it's last thing.
[57:25] - All right, all right, sudo. - Sudo and then port.
[57:31] - Is this how you spell sudo? - I just, let me drop it in.
[57:35] - Like, I feel like there's, it's so weird. Okay, sudo port install g8.
[57:41] - I'm gonna have to show you how to uninstall this and install it with Homebrew later,
[57:48] but this is good enough. - Command not found.
[57:51] - That means you probably need to download Mac ports. I never use Mac ports, so I thought it might have been
[57:58] built in, but it's not. - I will pause here because I feel like
[58:04] this is gonna be the best spot to leave it at, especially with this still installing and everything.
[58:11] - Yeah, so we essentially didn't do anything in the gist, so yeah, we'll definitely have to do another episode.
[58:17] - It's fine, it's fine. We'll just redo stuff in...
[58:21] - Well, we talked about all the things we're gonna do, so hopefully that was useful.
[58:26] - We did talk about all the things. I think it is...
[58:28] - And you gotta, and the GitHub part, all you have to do is once you install,
[58:30] you'll run literally brew install gh, that's all you gotta do.
[58:33] Then you'll have it, then you'll run that GitHub create repo command.
[58:37] - Yeah. - And it'll do the entire thing for you.
[58:39] It's a foolproof command, you can't mess it up. - All right, all right, cool.
[58:44] Well, thank you everyone for joining today and all the ideas and examples and all the things,
[58:51] all the things. - So many things.
[58:55] - So many things. So thank you once again, and we will see you next week
[59:01] and convince Anthony to come in on Tuesday. That's what I'm working on.
[59:06] So, thank you everyone. 
