---
showLink: "https://www.youtube.com/watch?v=U09MGASHjFw"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "oss-thursdays-with-distribute-aid"
title: "OSS Thursdays with Distribute Aid!"
publishDate: "2023-01-19"
coverImage: "https://i.ytimg.com/vi/U09MGASHjFw/maxresdefault.jpg"
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

[00:00] And we are live. Hey, Taylor. Hey, how you doing Ramon?
[00:09] I'm doing very well, thank you. How are you? Yeah, just peachy. Had a really exciting kind of strategy session with our full-time team last week.
[00:21] And I'm finishing up a 50-page document, but we've got so much cool stuff going on this year. And one of the things we realized was, so many great people working on different parts of DA,
[00:36] but it's kind of lived in our heads how all these different pieces fit together. And so this document really looks at what are we going to be doing over the 2023 year,
[00:46] but also how does that complement each other? Because there's lots of moving parts across our different teams, right?
[00:53] A good example is the needs assessment. Our logistics coordinators use the needs assessment survey tool and send that link. They build the survey out, they send that link to our frontline receiving groups, right?
[01:06] Get responses in. Then they do data cleanup. And then we pull it into the landing site to show it off in the new needs kind of visualization that we just launched.
[01:16] And so I think that works really well and people understand how tech integrates with their other efforts on that pathway. But there's so much more that we can do.
[01:26] So just good to get everyone aligned, feeling really good about our goals for this year. And yeah, excited to get into it.
[01:37] Love it. Love it. Well, let's take an opportunity to do that. We need to do that. So we are, just to give everybody a little bit of context as to what's going on,
[01:46] you might be watching on one of our several, we are streaming to several platforms at the moment. We're streaming to Jen's Twitch. We are streaming to Distribut8's Twitch.
[01:59] We're streaming to my Twitch. And you might be watching right now and you might be watching and thinking like, hold on a minute, where's Jen?
[02:10] Not to worry, Jen's running a little late, but she's going to join in. Because if you did miss the stream last week, Jen's going to be joining the Distribut8 stream.
[02:21] Or I guess we're combining forces. I don't know. Yeah, it feels like we did the crossover episode last year and that feels like an ongoing mashup or something.
[02:33] Yeah, we've signed all the deals, all of the, what is it? The volunteer agreement and stuff, yeah.
[02:42] Oh yeah, but I also, sorry, I was sticking to the television metaphor. What is that called? When you have a crossover, you need to sign off on it?
[02:52] You know, the companies need to sign off on it? I don't know, Ramon. I live in like a very informal grassroots world.
[02:58] I make million-dollar A deals with like a WhatsApp handshake, you know. This like signing documentation and stuff is like, I don't want my name on there.
[03:09] Fair, fair. So, well, good to have you here, Taylor, as always.
[03:15] And, you know, since, you know, now that we're streaming with Jen, we're going to be having a lot more eyes on the streams, which is fantastic.
[03:23] Thank you, Jen, for bringing those folks our way and like, you know, exposing to what we're doing at Distribut8.
[03:31] And, of course, for your incredible contributions to not just the Champions program but also Distribut8 as a whole.
[03:39] Taylor, shall we take a moment to sort of reintroduce folks to what Distribut8 does, what it is, and what we're up to?
[03:49] What is our Open Source Thursdays all about? Definitely.
[03:54] So Distribut8 is a grassroots humanitarian aid nonprofit, and we focus on connecting communities through supply chains to support each other.
[04:06] So a great example is like we're the team that solved Brexit for humanitarian aid, and we kept our UK collection groups connected to their frontline partners
[04:17] in northern France and kind of were able to continue to maintain support, you know. And then, of course, we organize the shipments and we deal with customs and all of this.
[04:29] So we really help smaller organizations that want to do good in the world interact with like a very big and difficult-to-navigate global supply chain
[04:38] and work together to achieve efficiency at scale, right? Yeah. It's really cool.
[04:46] Most of the aid that we send is like very environmental. We're preventing waste, right?
[04:52] So it's secondhand items that people gather from their communities. It's for in-kind donors program.
[04:59] A lot of the stuff we send would otherwise be destroyed. It's overstock. It's a misprint, something like that.
[05:05] So I feel like people have human rights, like you deserve to live a life of dignity, which means they're basic items that you need.
[05:14] And if we can, you know, like get people and meet those needs as cheaply and efficiently as possible using the resources we already have,
[05:23] you know, that's like not only are we solving immediate needs now, but we're really trying to build kind of systems and processes
[05:32] that meet these needs for everybody in the future, right? Like what we do today is awesome,
[05:37] but it's really like how are we going to support each other? What does community-driven support look like 20 years from now
[05:44] as the climate crisis worsens, you know, as different things happen, right? So in the short term, meet needs today, and we operate across Europe,
[05:53] including sending support to Eastern Europe for Ukraine response. We send aid to Lebanon, and we're ramping things up in the U.S. right now.
[06:00] You know, but also like how, you know, not even how does distribute aid help connect these communities in the future.
[06:07] How do communities get connected? Can we open source everything? Can we build the tech tools?
[06:12] Can we build the documentation and knowledge sharing so that anybody could do what we do?
[06:19] That's awesome. And I think to that point, the open source component,
[06:26] which is what you see here today, you know, if you're tuning into OSS Thursdays. So this is something that Taylor and I have been doing for, gosh, a year and a half?
[06:37] Almost two years, yeah. It's been a while, and so what we're doing here is we're tuning in every Thursday
[06:43] just to hack a little bit on our open source stuff. Our big objective here is to make all of this more approachable,
[06:52] especially for folks who are looking to get started in open source software development or even making contributions or whatever they'd like to do,
[07:00] and do so in a way that is sustainable, not just in a physical sense, but also in a way that brings as much benefit to contributors as it does to maintainers,
[07:13] which can oftentimes go one way or the other. Really what we want to do here is provide an environment for folks
[07:23] that they can come in, make their contributions, and stick around. Of course, if they want to.
[07:29] Eventually making this a self-propagating kind of thing where you can help out, be in charge of guiding others
[07:36] through specific parts of the code base. Well, that's the whole goal, right?
[07:40] We had a great success. We've really worked very hard to make it super easy to check out the code
[07:45] and work on your first PR and get involved, and we host code jams and these live streams,
[07:51] but we want to help people level up in open source. So we're big believers in mutual aid, which means that if you're contributing
[07:58] to helping someone out, you should also be benefiting from that, right, and not like a transactional exchange, but there is an exchange.
[08:05] And so I think we're so excited for this new Dev Champions program that Jen will be building out because it lets us be more intentional.
[08:14] It's not just like, "Hey, show up to the code jam and pick an issue and work on it."
[08:19] We're going to be creating pathways that people can go through to develop their skills in different areas of web development,
[08:26] of project maintenance, of testing, a lot of these different tracks. And it will be a structured approach, right?
[08:32] So it's not just like pick up an issue, get it done, and kind of feel good about that, but really here's a larger stream
[08:38] of things that you can work on and have a larger impact by owning that as a whole.
[08:44] And then hopefully, like you said, Ramon, people get inspired by going through that.
[08:48] It's like, "Cool, that was a great three months, and if you want to call it a day, that's fine."
[08:53] But if you want to, after kind of going through that program, you know, be a maintainer, be a leader, right?
[09:00] Like own the section of the codebase and help other people contribute towards it.
[09:04] I think that's what you were getting at with the self-propagating, you know, like, yeah.
[09:10] - Yeah, be the change you want to see, essentially. So let's, you know, again, just in case you're tuning in, folks,
[09:19] and you're wondering, "Hold on, where's Jen?" Don't worry.
[09:22] Jen's still here. We haven't taken over her channel.
[09:25] She's just… - Hackers.
[09:30] - Jen's going to be joining us as soon as she's done with other things that she's doing, but she should be here.
[09:36] - Y'all were talking about me? - Oh, yeah.
[09:39] - How is that fair? - Did you say Jen three times on stream and she shows up, you know?
[09:44] - It might be a thing. It might be a thing.
[09:47] And also, I may or may not have had to redo that video, like, seven times because…
[09:54] - Do you want to give us a little context into that? What are you talking about?
[09:57] - What I'm doing? - Yeah.
[09:59] - I am unseeing View Nation next week on January 25th and 26th. You can get your free tickets at viewjsnation.com.
[10:11] Sign up now. - The reason I'm wincing and smiling at the same time is because I know what
[10:18] making those videos is like, and it is so difficult. It is so difficult, especially for me because I get excited.
[10:26] I go off script. I mangle words in my mouth as I'm trying to get them out.
[10:30] It's hard. - I 100% did all of that, and I also just, like, struggle bust.
[10:38] And then so this is a very silly thing. I definitely, I love makeup, and I got the wrong shade of foundation.
[10:52] And I am, like, recording, and I'm like, I can see all of the missed colors that I tried to blend earlier,
[11:01] where when you're streaming, A, I don't care as much because I'm like, it's live, people don't care, whatever.
[11:07] But it's a lot closer, and I'm like, oh, my God. So I had to fix that.
[11:11] So thanks for your patience. I'm here.
[11:14] - Well, your makeup looks on point. - Oh, thank you.
[11:17] Thank you. Yeah, I got one of my handy-dandy, like, moisturizer things.
[11:22] It was like, blend, blend. - Yeah, I got to figure out how to do eyes.
[11:29] Like, I got some nail polish for Christmas, which is so much fun. But it's so intimidating.
[11:34] Like, I don't, as a guy, like, walking into a makeup store, and I'm just like, show me all of the, like, eyeliner.
[11:40] And it's like, no, it's broken down by brand, and I have no idea. - Let me know if you have questions.
[11:45] If you want to have a chat about makeup, I will talk too much about it. I love makeup.
[11:51] And it's something that I think is, like, so empowering to be able to change the way you look as, like, a canvas.
[12:02] And so there's, like, days where I'm just like, yeah, fuck it, I don't feel like doing anything.
[12:06] And then there's days where I'm like, I want to go all out and, like, literally have, like, the fake lashes on and everything.
[12:14] And so I feel like all people should do this. If they're interested, I should say that.
[12:22] I don't feel like all people should. Like, anyway.
[12:25] - Not to go too off topic, but on my 2023, I don't call it goals. On my 2023, things I want to do, bingo, that I do.
[12:37] - Oh, I like that. - Oh, it is fantastic.
[12:40] It's the best thing. Like, resolutions are long, a thing of the past for me.
[12:44] But, like, things I want to do, bingo, that's fun. I did get a bingo last year.
[12:48] - Yay. - And on that was trying, like, experimenting.
[12:54] Like Taylor said, like, experimenting with these kinds of products. And on two occasions this year now, you will have -- you have so far on some corner of the internet seen me wearing foundation.
[13:10] - Oh. - And I get it.
[13:15] - So to -- and I know I'm taking, like, continuing this off-topic conversation. I'm very passionate about it.
[13:24] So there are a lot of things that go into foundation. And this is something that I wish I could comprehend when I first started liking makeup is there's different coverages and different -- I like to say it's different layers that you can look at.
[13:46] Of -- because skin care is so important to be able to take care and have your canvas look good and actually absorb product. But then there is primer, which is literally just, like, this layer that says, hey, makeup, stick to me.
[14:04] And -- but then there's also, like, different types of foundation of, like, I'm probably going to get totally the terms wrong, but there's, like, tinted moisturizer and BB cream and CC cream and full coverage foundation. And I have played with them all, and I would love to learn with you guys because I, like, know about them, but I don't know their full terms.
[14:29] And, like, what they all are. So if we decide that we want to do a makeup stream, just sign me up or talk offline, whatever.
[14:38] I am there for it. That's all I got.
[14:41] I dig it. >> Cool, well, Jen, just to catch you up on what we were talking about up until now, we were, you know, given that we are now, you know, you are -- you and are so kind to lend us not just your streaming powers to be able to stream to multiple places, but also your platform so that we can, you know, widen open source Thursdays reach.
[15:09] We were just briefly reintroducing folks to what DistributeAid does, and I think just when you came in, we were starting to have a look at our open source efforts, mainly being this, our DistributeAid.org website. >> Sweet.
[15:28] >> Yay. >> So, Taylor, how do you want to take it from here?
[15:33] >> Totally. So I think that maybe we want to do a quick run through of, like, some of the tools that we use and just show people how to easily get started.
[15:44] I feel like there's, you know, new year, new folks paying attention, right? >> Oh, yeah, totally.
[15:49] >> So, you know, let's look at, you know, let's click that get pod link, let's look at, like, the read me and some of the code C maps, let's show folks how to run our tests and run the dev server and check out storybook and things like that. And then after that segment, I wanted to do a bit of, like, a maintenance-focused approach.
[16:09] So maybe look at some, you know, issues that might be resolved, right, that we need to, like, go close out or adjust. >> Adjust this.
[16:19] >> Yeah, and one of the things I really want to do is, like, we just pushed a whole bunch of code out the door. I want to maybe start building some code C maps, right, and have those aligned roughly with, like, different types of contributor pathways, which Jen might be implementing in the future as she builds out the dev champions program.
[16:40] So not to, like, constrain you or anything, Jen, like, take that the direction you want to take it in. But there's some natural things like visualizations.
[16:48] Can we show folks, if you want to make a visualization on the landing site, like, where to look, how to get the data in there, you know, how to, like, where's the front end live, where's the example code to follow? You know, same thing with testing, same thing, you know, different things like that, right?
[17:06] So, you know, I think this is a great opportunity, because you mentioned, Taylor, this dev champions program. I just want to -- because some folks might be watching and being like, a dev for what now?
[17:18] I just want to quickly highlight one thing, if I may, which is that there is -- Jen is going to be lending us her incredible expertise in building out this pathway, this -- pardon me, this roadmap for impactful, long-sustaining, open-source contributorship in the form of a champions program, which you'll see in lots of other companies, like the Microsoft MVP, the Auth0 Ambassador, and so on and so forth.
[17:52] So here is where you come in, folks, because the goal is to build this out in public. The goal is to make this an open-source project from the very core, which I'm so excited about.
[18:03] So I'm just going to go ahead and very cheekily put a link into the chats. Please, we're building this for you to make it, like, easier and better, and, you know, to contribute to Distribute Aid, so absolutely want that feedback.
[18:31] You know, think about, like, what's it going to take to get you involved and keep you involved, but also how can you benefit by going through this program? You know, everybody that works with Distribute Aid levels up their career, and I think that's, like, a very fair tradeoff we can make as a grassroots organization driven by volunteers, right?
[18:48] It's like, you know, use this to show off your skills to the world, to learn new skills, you know, and to make an impact and have a great story, right? And then take that to, you know, get the first tech job or, you know, get that promotion or get us, you know, do your first tech talk, right?
[19:08] Go get flown to a conference and do a speech about, like, you know, the module you built out or something like that. So, yeah, what's exciting? Like, what structure do you need, you know, to contribute over, like, a three-month period and kind of level up through that?
[19:23] And what's going to be the most impactful, you know, as our way of saying thank you? Yeah, I mean, so much so, you know, all of this. And again, it's all there for everyone to have their say. So, in fact, we've got, you know, issues on, for example, naming.
[19:41] Hop on in. Give us your opinions. I said, we have a proposed name, but it's not final. Same goes in discussion. Have a look at discussions. Like, for example, we've got one here. What can we learn from other championship programs?
[20:01] Please feel free to add others. This is where your voice comes in, folks. Like, please feel free to hop in. Exactly.
[20:11] And feel free to type it in case you have to be like me and on mute because my dog won't stop whining. Yeah, we do pay attention to that chat. But definitely, like, I'm so glad to have Jen's expertise here. I'm not an expert.
[20:26] Like, I don't know anything about these champion programs, you know, and it's going to take a collective effort. So, like, one thing that you could do right away is, like, go look at those links in that discussion.
[20:35] Check out the GitHub stars or the Mozilla tech speakers and, you know, what do you like about those programs, right? What looks realistic for, you know, kind of a grassroots open source project and, you know, what's, like, going to cost $5,000 to put on a conference or something like that that we probably can't do, you know?
[20:55] Yeah, because like Ramon said, a lot of big companies have these and by building it out in the open, we're trying to make it easier for smaller projects, open source projects to provide a structured experience for their contributors. And, you know, kind of welcome new people through that. So, we're not going to be able to do everything the big orgs do, but we can do the things that matter.
[21:20] I love that. And I think -- yeah. Cool. Should we run through some of the code base? Like, how do people start contributing, Ramon? Maybe we can do kind of an end-to-end, you know, show it off. And I do have one small fix that we can make as an example there.
[21:42] Before we go into that, and I mean, you'll be using these tools for it, but can we go in -- if I miss this, that could be an issue, too, and I could go back -- of what is Gitpod and CodeSee? Because we talk about them a lot. And I'm like, so I get it. But I don't get it. And it definitely throws me off. And then the other part, especially if we're going to be contributing something today, is the process of creating an incomplete pull request.
[22:18] Because that one definitely threw me off quite a bit, because not a lot of other companies do that. So, if we have beginners, because a lot of, like, 100 devs join us for this, as well as, you know, like, 100 days of code, like, a lot of newbies take a look at this. And if other people are doing something different, it can be kind of hard to be like, yeah, I want to do that, but I don't get it.
[22:45] Yeah, it's like, why are we doing it this way instead of the standard thing? That makes a lot of sense. And maybe this is some stuff that we should, like, think about writing down in the readme at some point, as well. Ramon, do you want to -- oh, go for it.
[22:59] No, I said -- I was just going to say I love that. I love the idea of, like, having a "what are all these things" section to our documentation. Totally.
[23:11] What are the things? What are the things? What are the things, Ramon? What's Gitpod?
[23:16] Oh, I might -- okay, cool. So, Gitpod. Gitpod is our -- I would say our platform of choice, especially for the streams, for collaboratively coding across different machines. Or on the cloud, as you will. Yeah.
[23:33] So, Taylor, you are in North America right now. Is that correct? Mm-hmm. I am.
[23:38] I am in North America. I am in Europe. Jenny, you're also in -- you're in the -- closer to the -- Different parts of North America.
[23:45] Yeah, yeah, yeah. Exactly.
[23:47] Yes. So, we're at widely different parts of the world, at least relatively. What Gitpod lets us do is have an environment where we can -- and this is a key term here -- environment that lets us collaboratively code without needing to do complex screen sharing, without needing to do complex setting up servers, without needing --
[24:14] You don't have to install something that lets you, like, remote-access each other's computers, which just sounds like a huge security issue. You don't need to restart your browser because Apple is forcing you to go into your system preferences to give it permission to do X, Y, Z. And it's like, well, now that you've done it, you've got to restart. Yeah. I come from a time when Apple didn't do that.
[24:36] So, quick question on that, then. What about, like, VS Code is so popular and VS Code does have a plugin that does, like, live sharing and you can share that way. Is this -- is the big difference between, like -- it sounds like VS Code live sharing is, like, doing it together at the same time, even without screen sharing, where the Gitpod lets you do it, like, async? >> I think one reason we're going with Gitpod is that we don't want to assume that every one of our contributors uses VS Code. Like, on my local machine, I use Sublime Text. I would love to upgrade to VS Code, but, you know, that's going to take an afternoon to make that happen.
[25:21] And so what I love about Gitpod is, like, you just click the button from our README, and you do have a VS Code-like interface. Like, I feel like this is very similar, you know. >> It is. >> Yeah. >> I think it's very similar because it is VS Code running on the browser.
[25:37] >> And I know I've seen people do this before. I don't do this, but you can -- when you open up the Gitpod, there's an option to have it, like, you know, basically do the Gitpod thing, but in your local VS Code, right? >> Yeah, where is that? >> Yeah.
[25:51] >> I know what you mean. Sorry, carry on, Taylor. >> Yeah, no, but that's a great question, Jen. And I would say, like, we're just trying to put options out there. So this is, like, the most inclusive, easiest option. Click the button, get the Gitpod going, and you can start contributing right away.
[26:07] But, you know, especially as you're building out that Dev Champions program, I'm hoping to get a couple of people that, you know, kind of, like, are on the same track, right? Who can back each other up, who can collaborate for each other, who can do reviews for each other. And if they both have VS Code and want to use the VS Code sharing, like, more power to you, right? >> One thing that I like about having this running in the cloud, as well, is that -- and Taylor mentioned this kind of briefly -- I don't need to worry about what Node version I'm running, what NPM I have installed.
[26:43] I don't need to worry about, like, oh, I'm coding on FreeBSD. Do I need to -- you know, like, a different operating system that is not very commonly used. Do I need to, like, you know, get super stuck because, I don't know, one part of Storybook, which is one of our dependencies, does not work on FreeBSD. Like, this sort of thing. >> That's actually a very real thing I'm dealing with. Like, we need to upgrade our Node version from 16 to 18 or something in order to get the latest version of Gatsby. Right now, a bunch of pull requests from the box to, like, update our dependencies are piling up, and I can't do that.
[27:23] I'm on elementary OS, which is based off of, like, Ubuntu 18 or something, and that version of Node does not work unless you have Ubuntu 20. Right? So, like, locally, I basically am looking at an OS install, you know, and, like, wiping out my system, backing it up, installing it in order to, like, bump my Node version up. But the nice thing is, like, I don't actually have to do that. Right? I can open up Gitpod. We can have it, you know, use the right operating system, use the right Node version, and I can still make forward progress on the code. I just can't code locally in that case.
[28:02] So, I think it does, you know, getting an online environment, like, lets us standardize things. It gives us a chance to say, like, we support Gitpod, which means we support VS code and kind of standard stuff, you know, and hopefully that works on your own local environment. Because, like, if you need to set something up, like, that's cool, but I'm not, like, IT support for your computer. Right? You know, but if it doesn't, and, like, it doesn't work on my local environment right now, like, you can go back to this kind of standard thing. You know what I'm saying?
[28:34] That definitely makes sense. So, I'm stoked to see that, and definitely even as we're doing this in something that I think is really cool of doing this together, and also, like, for everyone, just if you're wanting to learn how to do something, observing others is a great way of doing that. >> I'm going to put this up in stream elements. I'll bug Ryan to see if he can help me with this. Is I was watching Theo's stream for a while, and yesterday, and something that he did is he'll record live, like, his full video, like, and I'm totally digging, and he would just say, like, some type of command that would tell him where they are, so I'm writing time codes.
[29:17] But I'm saying this in the fact that I'm going to clip it and put it where we are in our, I can link it in our readme when people want to go back and be able to understand it. Like, we can use the transcript and be able to put the video, which is really, really helpful for those who learn very differently. >> I dig that. I dig that a lot.
[30:00] >> I dig that a lot. >> I dig that a lot.
[30:34] >> I think it's really important as developers. I think if we shoehorn everything into the same way of doing things, we overlook people who have different setups, people who have different situations, and the homogeneity, is that the right word, of the browser, I find is -- I'm not going to say homogeneity. But the right word of the browser is pretty much the same everywhere you go is really, really handy for creating these streamlined experiences where you can be like, look, you can clone it if you want, you can do all your Git stuff, you can do all of your NPM, or if you want, just open this up.
[31:12] I think one of the benefits it has is that we can tell you, hey, instead of messing around with, you know, yarn and installing yarn install, like, why not tell Gitpod, and this is a feature of theirs that I really like, why not tell Gitpod, like, hey, when you open, do all those things that you usually have someone do when they start up. Why not tell Gitpod, install some, some NPX stuff, and then just start it up. Same goes for Storybook. Why not set up Storybook? Why not open the browser right away, since you're going to be working with that browser? And I find those parts, this, there's a, there's this sort of ephemeral feel that I, that I find is coming to the, to software development that I find really compelling, which is just like,
[32:05] instead of having an environment that you kind of like, lug around with you like a heavy suitcase, why not just have a thing that you just like, open up, pop in, do the things you need to go and then pop back out, because we're human beings, we're busy, we're jumping around projects. And I find that really compelling about a tool like this. It definitely goes back to options, though, right? Because there are people that maybe don't have the best internet connection, who should still be able to contribute to DA, it's better for them to download everything at once, you know, work offline, and then, and then, like, re upload it or something like that. So I think that the flexibility, I also want to caution folks, you're not going to get away from running the commands on on Gitpod, but it is a really nice way to get you started and get you in the zone, right?
[32:53] But if you change your branch, and there's new dependencies installed on the branch you're working on, like, yeah, you'll have to kill the server, run yarn, install and rebuild the server. And that's fine, right. But in terms of just a jumping off point, this has been the, the easiest way. And the collaboration features are really cool. Although I did not realize that VS code had similar stuff. So thanks for pointing that out, John. Cool. So should we show folks Ramon, like, like, I know that it's nice that that Gitpod does a lot of this for us. But do we actually want to like kill the server and kind of show them the commands we use to, you know, do the installs, clean out the cache, build it just kind of run through like, what do those normal kind of dev process look like?
[33:41] Yes. Also, may I put it out there? Jen, would you like to drive? Actually, no, thank you. I say that because being able to actually take notes and where things are to reference back to it is not, I could say a luxury that I normally have.
[34:08] Yeah, that being said, and also, I'm in charge of the dog right now. And this is why you see me go off camera is she's going bananas randomly. And I don't want to be able to take away from that. But I do appreciate it. And I will call dibs on the next one. Yeah, totally. Listen, just to just to be super clear, not putting on the spot, more like, I don't want to hog all the fun.
[34:34] Oh, no, I actually and this is something that I was thinking when you came on the stream on Monday is I love that you were running stuff. I was just like, have fun. So yes. To be clear, to give context, I was showing I was showing Jen and Laura how to use OBS, you know, open broadcasting software. And yeah, I just kind of took that and ran with it.
[35:03] And I appreciated it. It's something that I really, really appreciate of you. It was good fun. Awesome. Okay, well, let's let's let's do what what day Taylor recommended. So we've got, you'll see here some running terminals. So Taylor, you were saying get pod test to node, this can be shut down.
[35:28] Yep, that's where the server is running. Let's go and shut down storybook. Let's just shut it all down and show people from scratch. If you're checking this out locally, or sometimes like it pod does, you know, one of the commands times out or something when it's doing it set up, so you need to do this too. So the first thing that we're going to do to reset our dev environment here, Ramon, is we want to do a yarn install, right? If you change branches, you know, things like that always good to just run on yarn install, make sure you have the latest. Yeah.
[36:01] Fabulous. Let's do that then. So we will do. You said yarn install. Mm hmm. And most of these commands are documented in our readme. You can also look for them at the end of our package dot JSON. Let's let me says, Yeah. So we've done yarn or yarn install. What's the difference between yarn and yarn install? Um, I feel like it might just be a shortcut. Honestly, I'm not sure what happens when you just run yarn by itself.
[36:36] I think it is as well. But good to know. Okay. So we've got yarn and then run the dev server with yarn dev. Right. But what we're going to want to do here since we've already ran the dev server, like let's again, you're changing branches or something, go ahead and throw a yarn clean in there, right? So that'll clear out Gatsby's cache. Usually it's fine to have that cache if you're just kind of doing iterative development on the same branch. But sometimes if you're working at the Gatsby layer and changing how the data is formatted, or if you're changing branches or something like that, you're going to want to clean that cache out and rebuild it so that you have the latest and greatest.
[37:15] I've definitely had some highs and bugs pop up. And I'm like, why isn't this working? Or why is it giving me the old data? It's like, well, it's because it was cached. And, you know, Gatsby didn't update that cache. So a yarn clean is, you know, great troubleshooting step there. If you're like, why is stuff not showing up the way I expect it to? And now we can run that that yarn dev remote, definitely. Perfect.
[37:47] So what's going on now, Taylor? Um, so what it's going to do is compile everything, then Gatsby is going to source the data. So we have data that's included in the repo itself, we use forestry, which is our content management system that commits directly to Git. So there's a content folder with a bunch of markdown files in there. We also pull in data from external API is like our needs assessment surveys, we have a database on a server there.
[38:17] And we can pull data from that. So this is kind of like sourcing all the data, running the data transformations and building the Gatsby GraphQL API is that first bit, once that's built out, it's going to build our bundle, right. So this is the static site that it generates to serve, you know, either in production or in your local browser. So basically, takes that Gatsby API, you know, and that's what powers our react side, right, it plugs in all of that data into these react components, pre builds everything, and then you just have a static site that is served up.
[38:55] Great. And I can see it's still so it's still building, right? Yep, the dev bundles a little bit slow, but this will update. So as you're making changes and stuff, especially in the front end, if you're making front end stuff, it'll auto update. If you're changing the Gatsby kind of data layer, changing the structure of that GraphQL API, things like that, you're going to need to kill the server and restart it.
[39:21] Yeah. Good to know. Good to know. Thank you. How?
[39:33] Well, what happens now? Yeah.
[39:37] Yep. So so let's go take a look at what's available in the browser, we have two main views that the server offers us. The first one is just the, you know, the dev website itself. And the second one is the GraphQL Explorer. Cool. Which, which one do we want to open when we're developing?
[39:59] Both of them, probably. Okay, so so we can open that first one there, that'll be like the front ends that you see, right? I'd love to offer a caveat, if I may, if you're developing in, in, in Gitpod, and you try to open up localhost like this, as it says, it's going to give us an error saying that localhost refused to connect. So what's going on here, and here's a caveat of using a tool like Gitpod.
[40:27] Gitpod is running on the cloud, meaning that it doesn't know nor have access to localhost 8000, which is usually an address reserved locally on your computer, hence the name localhost. So if you want to open this, I would recommend, this is something that you can do in VS Code as well, is if you see a URL or a link like this, you can hold down Command or Control and click on it.
[40:53] Now what that's going to do is open up and you're going to, you can't quite see it because it's, or I hope the font size isn't terribly small here. But you'll see it made an automatic URL with 8000 at the beginning for this specific Gitpod instance, meaning that we now have access to be able to run the server, look at the front end as Taylor described, running on the cloud. And here's what's cool, because it is a public link, right, it means I can go ahead and paste it in the chat. I'm going to do that now.
[41:32] I just pasted that link into the chat. Now, if you're watching this live, you can go ahead and open it. I hope, I think.
[41:42] Let me confirm that. I don't want to be spreading wrong information. I think it should.
[41:49] I'm not so sure. If anybody's watching and can confirm, that would be amazing. Thank you.
[41:57] This page is not working. Ah, that's because it's not open to the public. I apologize.
[42:03] If I were to share, so sharing this workspace with others also means sharing access to your repository, everybody with access to the workspace you share can commit in your name. So, if I were to share this with all of you, you would be able to do that.
[42:16] The reason I'm not going to share it now is because I just don't want you all, you know, helping on our instance and like making, because this is tied to my GitHub, so you could make bogus commits. Not that I don't trust you, just making sure we're all on the safe side. I think that's fair, right, Taylor?
[42:35] Yeah, yeah, absolutely. You know, but it's cool that you can share this like with people you're collaborating with, or what I find is really good for like working with non-technical contributors, right? Because we're often building things, you know, like for the people running the needs assessment or for people running logistics, right?
[42:54] Is I can spin up a Gitpod instance and do some real-time collaboration where I share that front-end URL with them, right? And so it's like, hey, let me go make a change, refresh the page, and then take a look at that.
[43:09] So that can be cool as well. Exactly. Cool. So we've got that running now. What do I do next, Taylor?
[43:20] Yep. So let's open up the second link there, the GraphQL Explorer. So this is really handy when you're both doing kind of like the, I'm going to call it the middle ends, right?
[43:34] When you're working on sourcing data in Gatsby or transforming that data, and you want to make sure that, you know, the data is coming out okay. Like obviously you can write tests and stuff, and we do encourage that.
[43:43] But while you're hacking it together, exploring the GraphQL data here can be quite handy or figuring out, you know, how to structure that. And then, of course, for the front ends, when you're trying to build the page queries to get the data that the page needs, this is a really good kind of way to do it.
[44:04] So, for example, Ramon, let's say we're working on the region pages. Do you want to like click through and just source some data, you know, from all DA region there and kind of use that to explore, you know, our region data?
[44:19] So here you have different commands and stuff, like you can filter, you can group. What we usually do is if you click on nodes there, that'll be the actual data.
[44:30] So if you're just exploring, I recommend clicking on something, then clicking on nodes. >> There we go, yeah.
[44:39] >> There we go. And now this is like, you know, what is a region kind of data object look like?
[44:46] So we might want like the slug and the name. You know, we can probably skip a lot of the text-heavy stuff.
[44:53] But you can see that we also have this hooked up to subregions. So because those are linked, we can get a region and a subregion.
[45:03] So, Ramon, maybe you'll select slug and name for both region and subregions. And this would be an example of a query that you'd want, you know, for something like a menu.
[45:15] If you wanted to build a menu, you know, a static menu that just lists the region and the subregions, right, this would be an example here. And you can get all of that through GraphQL.
[45:26] So if you're new contributors, I highly recommend exploring the data in this GraphQL tool, you know. And the best way to do that is through, you know, clicking on one of those data objects and then clicking on nodes, right.
[45:40] And if you hit run, Ramon, we'll see our regions and subregions pop up. And there we go.
[45:47] >> I have a question, Taylor. For those that are watching and perhaps not familiar with this, because you mentioned GraphQL and a query, what is GraphQL?
[45:58] >> Ooh, Jen, do you want to take this one? You got real excited there.
[46:01] >> No, I was just like, this is such a good question. I'm not great at explaining GraphQL, but I'm excited to hear you explain it.
[46:09] >> Okay. So GraphQL is like -- I might be mixing up some of the technical terms here, so feel free to jump in.
[46:19] But essentially it is a graph database. So I'm sure folks are familiar with relational databases like MySQL or Postgres where you have tables, you know, which kind of model your data in a structured, repeatable way.
[46:35] And then you can link those tables together, and you can do joins to pull multiple data sets. Graph databases are nodes and arrows, right?
[46:45] So here we have a region node in our query, and then we have arrows connecting that region node to the subregions. That means that when we say, hey, give us all of the regions and their subregions, it creates this nested kind of JSON structure as a result, where it's like here's an array of all of the regions, and then inside of those region objects here are their subregions.
[47:10] But it's very flexible and powerful. We can basically pull data, you know, using this kind of like graph-driven relationship modeling.
[47:18] So we could just pull the subregions. We could also pull, hey, give me a subregion and what's its region, right?
[47:25] And I really like it for complex kind of data modeling spaces like the ones we have at Distribute Aid where there are lots of links between things. It's a much more natural way to say, like, I want this data and then I want this other data, right, rather than trying to, you know, do that through all these joins.
[47:44] So in one query we could get, you know, here's like a region and everything associated with the region. You'll see this on our very large page queries.
[47:52] We're like, hey, what's the region? What are its subregions?
[47:55] What are the needs for that region, you know? And so we can create the total, you know, current needs, you know, things like that, which like if I were to write that in, you know, like a relational database, like that might be one massive join or more likely a series of different database calls where I have to get the region and use the region ID to get all the subregions and get all the needs data, you know, and then stitch it together.
[48:25] So here it kind of does that stitching based on those relationships for us and we just get one large data response formatted in the way that we structure the query. Does that cover it, Ramon?
[48:37] I feel like I might have left some bits out there, but that's -- I think it's a good introduction and like just to add to what Taylor said, this -- what I like about this GraphIQL, which is GraphQL with that little I for interactive, is that it lets us mess around with it without fear of breaking everything.
[48:57] So that's -- the key here is -- the key part here is query. When you're asking for something, you're not modifying anything.
[49:04] You're just querying. That's not the whole picture, but I think in this context of like trying to get that data, I find it really, really handy.
[49:16] So what we've done here, for example, is query the entire graph of regions and their subregions, which, by the way, in case you're curious, I'm just going to take us to the website real quick, is what you see is the data that we have here. The regions we support at Distributed, in case you're not fully familiar with Distributed, they provide support to these regions.
[49:44] And then each of those regions you'll see here, the Balkans region, is made up of Serbia and Bosnia as subregions, Lebanon, Beirut, Beke Valley. Greece is made up of Eastern Islands, Southern Greece, Northern Greece as subregions.
[50:00] How's that? How am I doing?
[50:02] >> Yeah. Yeah, exactly.
[50:04] >> And there you go. And so, like, what we're doing here is querying that data and messing around.
[50:09] So these are, like, the two tools that you'll be working with when you're developing for the Distributed website. >> Absolutely.
[50:19] So I want to go back to Gitpod now, Ramon, and I want to show folks, you know, especially if, like, this is the first time you're checking out the code base, I'd recommend doing a few things to get familiar with our commands and kind of investigate. So one of those is not everything has tests, but we are starting to work tests in more and more to new development and could certainly use some help going to write tests for the kind of early hack-it-together stuff.
[50:47] But should we run through our different types of tests here, Ramon, so people can see those commands? >> Absolutely.
[50:54] So what do I do? >> Right.
[50:56] So leave the dev server running. Let's go to one of the different terminals there.
[51:03] And we can go look at the README again. There should be something farther down.
[51:09] There we go. You see, like, yarn clean documented.
[51:12] Here is our different types of tests. So one of them is code formatting, right?
[51:18] We want our code to be consistently formatted so that it's readable and understandable and, like, we don't have different personal styles, you know, kind of, like, conflicting with each other. This is almost automatic, right?
[51:29] If you use, like, printify or something like that in your VS code, it will automatically update it as you're working on the code. But we use a precommit hook to automatically printify our code.
[51:43] If you happen to write messy code like I do and want to kind of clean it up while you're working on it, though, you can run yarn pretty and that will do a printification pass, you know, through your kind of in progress stuff. So she'll run yarn pretty real quick.
[51:57] >> As a side note, just because we're using one screen to share right now, and I'm saying this because when I was watching streamers, I'd be like, oh, well, they do it in one screen, so I should do it in one screen. And half the time it's so much easier for me to have them side by side to remember the things I need to do and have multiple screens.
[52:20] So just saying that for people like me that are like, oh, yeah, that is an option. >> Are you saying, like, the terminal and the editor there or what's side by side?
[52:34] >> Well, I would say you can do it with the terminal, the editor, but I mostly meant, like, having the read me separate because then you know what to go back through and check and being able to do them side by side instead of constantly having to go back and forth. Because the back and forth really causes me to forget to do things.
[52:54] >> Yeah, that makes a lot of sense. >> I think that just kind of highlights that diversity, you know, like, diversity of approaches, point Ramon was making earlier, too, is, like, we got to provide a base layer that works, like, has one happy path that we, like, guarantee support for, like this Gitpod, but make it easy for people to, you know, adapt that workflow to their own.
[53:18] And, you know, like, just jump in and do it your way, and that's, you know, we appreciate the contribution. >> Yeah.
[53:28] >> You want to run Yarn Pretty, Ramon? >> Let's do it.
[53:32] >> Let's do it. There we go.
[53:36] So we don't have any changes right now. It's pretty fast.
[53:40] Exactly. And it will run every time you make a commit.
[53:44] So I think there's some, like, edge cases with Yarn Pretty where, like, if you have a partially staged file, like you're trying to -- in a single file there's some changes you're trying to commit and not others, then it doesn't know what to do, right? And so the thing to do in that case, if it's like, hey, my commit failed because of Yarn Pretty, just reset everything to head so your changes aren't staged, do the Yarn Pretty there, and then kind of re-add the changes that you do want to commit, including that partially changed file, and make your commit, and it should pass because there's no changes to make.
[54:22] So just want to throw that out there, if you do complex git commit stuff like Ramon likes to do. All right.
[54:32] On to tests. Should we run our unit tests, Ramon?
[54:36] >> Yeah. Do you want to tell us a little bit about unit tests and what they are?
[54:42] >> Totally. So unit tests, there's a couple of different types of unit tests.
[54:46] There's more of like, you know, the pure function testing. That's something you'll see in the Gatsby directory where we're kind of just saying, hey, data in, does the function transform it, so, you know, the right data out.
[55:00] We also have unit tests at the UI level where we want to render React components and then kind of like make sure that certain properties of that rendered component exist. So, for example, when we are testing images, we want to make sure that we can take that kind of blob of rendered HTML and find a specific alt text in there as a representation that, like, the image is available on the screen, but also that the image has alt text for accessibility purposes.
[55:32] Right? So pure function testing, you know, there's the kind of component level unit tests that check the properties of that component, make sure it's working fine.
[55:44] That's what our unit testing does. Yeah.
[55:50] We can also do some cool stuff. So I believe we're using Jest, Ramon.
[55:54] If you go to the Jest commands, you can add stuff there. I think if you do yarn test dash dash coverage, that will give us some code coverage stats as well.
[56:04] So we can maybe identify where some of the holes are. This might be my feature request of the stream for Code C. Code C, if you're listening.
[56:16] How cool would it be to take something like, you know, code coverage, right, at the file by file level, and then automatically apply that to a Code C map so you can see, like, where your tests are, where your tests aren't, and use that to plan future testing work. That's awesome.
[56:36] Yeah. I like that idea a lot.
[56:40] There's a lot of things. I dig that we're going, like, all the way down.
[56:44] Like, what are all our things? Let's start with what is Jest?
[56:48] Question. Is that the clown in a court during the medieval era?
[56:58] Oh, sorry, I meant the tool Jest. No, no, I was making a joke.
[57:02] I like the -- so is it a Jest or a Joker? Like, what are they?
[57:10] No, I'm not going to claim to be an expert here. Oh, puppers.
[57:20] Very annoying doggy. What up, doggy?
[57:24] What's your name? I'm not going to claim to be an expert here.
[57:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[57:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[58:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[59:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[60:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[61:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[62:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[63:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[64:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[65:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[66:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[67:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[68:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[69:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:24] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:28] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:32] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:36] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:40] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:44] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:48] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:52] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[70:56] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:00] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:04] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:08] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:12] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:16] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:20] I'm not going to claim to be an expert. I'm not going to claim to be an expert.
[71:24] I'm not going to claim to be an expert. TypeScript is compiled to JavaScript.
[71:31] Compilation is a step where you take a language, run it through a program--
[71:36] this is called a compiler-- that translates it to JavaScript.
[71:43] So what about our own types? Well, that's where doing things like
[71:47] defining types, interfaces, classes, sub-- no, that's JavaScript.
[71:53] Doing all of this typing helps us make sure-- we're essentially protecting ourselves from ourselves
[71:59] when we're writing code. So where does testing types come in, Taylor?
[72:07] Right, so basically when you declare your types, like, hey, this function takes a string.
[72:17] Let's say it takes-- actually, let's do a different example.
[72:21] It takes two numbers, it adds them together, and it spits out a number, right?
[72:25] And you can declare that as a type. You can say, here's the input types,
[72:29] here's the output type, right? Kind of define a function type there.
[72:34] And then let's say there's a different part of your code where you call that and you're taking some entry
[72:38] on a web form to add with another number, right? And maybe you made a mistake and said
[72:45] the input is a string input, it's not a number input, right?
[72:50] TypeScript will catch that for you. And so it'll say, hey, you're taking something
[72:54] that's a string and trying to put it in this function which accepts two numbers, right?
[72:59] Not a string and a number. Now, it's not going to, like, stop the code from running.
[73:04] It doesn't get in your way and break everything, right? But that's why we have our TypeScript checks.
[73:10] We want to make sure that types are defined as, like, a courtesy to the other contributors, right?
[73:17] And that there's no type issues, you know, that you've introduced as you're kind of, like,
[73:22] writing code and stringing functions together. So, again, it's one of these things that, you know,
[73:28] like, really is designed to keep things safe, to keep things normalized throughout our code base, right?
[73:35] Like, let's not just, like, hack it together and throw any types in there.
[73:39] There's, like, an any type. We want to avoid that. We want to have things explicitly typed.
[73:43] And let's make it easy for you to understand, like, you know, hey, like,
[73:47] this is why this part of my code isn't working. Like, the types aren't lining up.
[73:50] And so when I add the string three and the number one, I get 31 instead of, you know, as a string,
[73:57] instead of four as a number, right? And so it'll prevent that.
[74:03] Because JavaScript will coerce 31 into a number in different circumstances, right?
[74:08] So it can be very confusing if you get something that, like, looks like a number to JavaScript in its untyped form.
[74:13] And then, you know, like, it can be a number, but it's the wrong number because you've added a string
[74:19] and a number earlier on, right? - In fact, you can do that here in the console.
[74:24] - Yeah. - So what is it? Three, the string three.
[74:30] Oh, my goodness. I cannot type today. All right. I don't remember how to do a quick recap.
[74:39] Three plus one. You'll see JavaScript's already being like, "Oh, 31."
[74:44] But--oopsie--what happens if I say, "Is three plus one bigger than five?"
[74:55] No, wait, smaller than--oh, yeah, smaller than five. - Yeah, smaller than five. Yeah.
[75:01] - It's false. But is it bigger than five? - Exactly. - True.
[75:05] Why? Because what's happening here is that it's saying, like, "All right, let's course this string back into a number."
[75:13] So now we're checking that the number 31 is bigger than five. So this is, like, a really good, like, case
[75:20] for using something like TypeScript to protect your code. - Yeah, and so I find often, like, I want a command that,
[75:27] you know, lets me check my types as I go, or you can even hook it up to Visual Studio to do that for you.
[75:34] And so we can run yarn test colon types, and it'll run through the type checking.
[75:43] I've also introduced--and we might want to relax this in the future. I don't know, Ramon, but I added the TypeScript test
[75:51] to our pre-commit hook. And what I noticed was that a lot of people were, like,
[75:57] you know, sending code that had broken types but would otherwise work.
[76:01] And then the CIBC server was, like, catching that, and that was a bit frustrating.
[76:06] So what this does is it, like, won't let you commit stuff with broken types, which, like, might be a frustrating point, right?
[76:14] But it'll also, like, give you that heads up early. And so what we might want to do is, like,
[76:19] remove it from the pre-commit hook if it's too restrictive, but still have that command exposed.
[76:26] If you run yarn test colon types, you can, like, double-check that yourself
[76:31] before you push something up if you want. I don't know. We'll see.
[76:34] And we're very open to feedback, so please, y'all, if you're contributors, let us know.
[76:38] Like, if you're running into something that's stopping you from making forward progress, we're happy to change things up.
[76:46] - Love this. - Cool. All right.
[76:51] So I think I want to end here. We got about 15 minutes left, and there's, like,
[76:55] a real quick change we can make that I want to push out to production.
[77:00] And we can use this as an example for a draft PR. And so what we're going to be doing is we're going to be
[77:09] adding units to show what units different items are on on our new needs assessment visualization.
[77:19] How's that sound, Ramon? - Fantastic. - Awesome.
[77:23] There is not an issue for this up. Usually, we'd have an issue and work off of that,
[77:28] but I don't think -- unless we want to make one real quick. I'm not sure if we have time.
[77:32] - Let's do it. Let's make an issue. - Let's do it. Let's do it. Okay.
[77:36] - It's our stream where we do all of this live, so, like, why not?
[77:41] - Why not? So let me --
[77:47] - So what am I doing here? - Well, I have some stuff on Notion about this,
[77:53] so would it make sense for me to make the issue? - Yeah, yeah, go for it. I will unshare.
[77:59] And then when you're sharing your screen, we can bring yours up.
[78:10] - Okay. And everyone -- oh, this is one of the -- I wanted to show folks.
[78:14] We sent a whole bunch of stuff to Ukraine. There's a lot of oat milk for people that are lactose intolerant.
[78:22] So we usually don't share these beneficiary-facing photos on our social media, but most of these folks have masks on,
[78:31] and it's like, you know, they're obviously Ukrainians, like, not in a great position,
[78:35] but I don't think people can, like, identify where they're at. So just wanted to highlight, you know, some impact of our work.
[78:42] We also sent two machines to produce more milk, which I think is hella cool.
[78:46] Like, how do you get people in crisis supporting themselves? Because they want to do that.
[78:50] You know, it can be very tantalizing sometimes if everything's just done by the aid workers or whatever.
[78:57] Yep. But I got our issues here real quick. I'll smash that new issue button.
[79:04] And this was the priority feedback from the launch. So we want to add units on data visualizations for relevant items.
[79:14] This is going to be a feature request. You know, what I love about this is that it's a really good insight
[79:21] into how all of this grassroots work happens. You know, you're using Notion, you're bringing that over to GitHub,
[79:30] making all of that super, like, as open source as needs to be so that folks can contribute as is necessary.
[79:38] And just a quick reminder, folks, like, if you've been watching us going on and on about all the tools we use,
[79:43] we didn't even get to Code See today, our kind sponsor of the show. If you're interested in contributing, let this be a reminder.
[79:56] You're not alone. If you need help with anything, if you want to tackle an issue,
[80:02] speak up in one of these issues. Hold on. Let me, let me, let me, let me,
[80:09] while Taylor is doing all that good stuff, just put a link here to the repository.
[80:15] And, you know, remember, voice your interest, and one of us will be around to either guide you
[80:23] or at least get you up and running, all that good stuff. Because, like, how did you put it, Taylor?
[80:33] Mutually, mutual benefit here? No, how did you put it? - Mutually. Mutually. - Mutually.
[80:39] The idea that, like, by helping other people, you can also help yourselves.
[80:43] That could be, like, direct. We don't want it to be transactional, you know,
[80:47] but it can be direct, like, "Hey, I contribute to Code to DA and participate in the Dev Champions program,
[80:52] and I get, like, a LinkedIn shout-out, and, you know, like, have a great story to tell,
[80:56] and can use it to advance my career and learn things." Or it can be indirect, like, "We support refugees
[81:02] because that's a fundamental human right, and if we ever find ourselves in that situation,
[81:06] we want someone to support us. And if we don't, by making a more welcoming environment
[81:11] for people that are, you know, fleeing to our countries, like, will they get integrated in society faster
[81:17] and just kind of help, you know, our society and be a part of that," right?
[81:21] - Yeah. - Cool. So I have the issue up here.
[81:26] There's a few caveats, right? So we want to highlight this unit,
[81:30] but if things aren't broken down all the way, like, in some of the graphs, we're just looking at things
[81:36] at, like, more of a summary level, then we're not going to be able to do that.
[81:42] And the example they've done here is when you hover over the graph, right?
[81:48] And I can pull this up on our live website. You know, it shows you some more information.
[81:56] I might decide to take a different approach, though, right? So if I hover over here, it's like,
[82:01] here's the total number of, like, kind of items, right? But if we want to...
[82:07] let's go ahead and look at... we want to filter to hygiene,
[82:13] and we want to index by item. Right? So here, this is, like, the same item.
[82:22] This would be, you know, for liquid soap, that might be something in milliliters,
[82:27] like, how many 100-milliliter bottles or 100-liter bottles or something, right?
[82:33] So we want to highlight it there. Yeah, it just kind of depends on what the view is.
[82:41] So it might be a bit tricky. What I might recommend, Ramon,
[82:45] is instead of adding it to this kind of, like, hover-over sort of thing,
[82:49] what happens if we just include it on the item-specific? So if you break it down and you're showing, like,
[82:55] her item here, right, then we would show it next to the item name.
[82:59] If you're showing, like, her region or country, more of a summary view or something like that,
[83:03] you know, then maybe you don't care that some of them are, like, items of clothing
[83:07] and others are, like, 250-milliliter, you know, soap bottles, right?
[83:12] Right. Cool.
[83:16] I love it. Yeah.
[83:19] No, go for it. No, I was just going to ask, like...
[83:24] it's interesting how interacting with all of this data sort of brings out these needs that we have
[83:32] in order to tweak how this all looks in order to present it better.
[83:37] And, like, I think that really speaks to... like, Jen and I talk a lot about...
[83:46] holding ourselves back from releasing things just because we want to make sure
[83:51] that everything's looking great and perfect and all that, but, like, how by putting it out there?
[83:55] How by trying things out? And this is something that I find very...
[84:00] for lack of a better term, magical about open source is that we have the flexibility to experiment.
[84:06] And people can just tell us. Like, you have a forum right there,
[84:09] like a forum by which I mean a GitHub issue where you could just be like, "Hey, do you know what?
[84:13] I think this would be better as you saw." Because I believe, Taylor, you did change this.
[84:18] Now the graph is on top. The options are at the bottom.
[84:21] Yes. Yeah, exactly.
[84:23] It's only the share link on top and then the graph and then if people want to get more advanced with it, you know.
[84:28] But we also do some cool stuff. Like, if you go to regions, right?
[84:32] You want to look at France. Like, when you click that needs tab,
[84:35] it takes you to, like, a preset graph, you know. So we're using the combination of, like,
[84:40] here's all the options and then you can encode those options in the URL.
[84:44] You can get the share link right here. Allows our team to make these graphs
[84:49] but also has anyone to go in and, like, make their graph that they care about
[84:53] and then share it, like, on Facebook and people can come back and see what they were looking at, right?
[84:57] Yeah. Yeah.
[84:59] Yeah. So here's another example.
[85:02] We are... Oh, I wanted to index by subregion.
[85:09] Oh, that's right because I changed up. We're looking at Greece here.
[85:14] There we go. So this is, like, the subregion breakdown.
[85:17] You can see there's a lot more need in southern Greece than in the other places, you know.
[85:21] But we're grouping by category. So here it wouldn't make sense to have, like,
[85:25] item versus 250 milliliter. However, if we grouped by item, right,
[85:32] then that might make sense. Like, here's disposable razors, sanitary pads, you know.
[85:38] But there might be some liquid soap or something. You know, toothpaste, right?
[85:42] How many milliliters of toothpaste because they come in all sorts of different sizes.
[85:47] And I think that what we can do is just by changing how the item name is generated and including that unit,
[85:54] that'll make it happen both here and in the graph, right? So I want to switch it over.
[86:06] And to make sure we can get through this efficiently, does someone want to drive?
[86:11] And I'll help navigate the code base because I'm very familiar. We can just kind of go in and, like,
[86:15] do the thing that we need to do and use this as an example for the work in progress pull requests and then call it a day.
[86:22] - Sounds good. How are we for time? Because I know we usually have allotted an hour and a half.
[86:28] Jen, I want to be respectful of your time too. You got some time or, like, feel free to drop as well,
[86:34] like, as you wish. - I'm good because I'm trying to stay as concentrated as I can
[86:41] with the dog. - You are fine. Just want to give you the space.
[86:47] - As long as you guys are okay with me being on mute and randomly going away, we're good.
[86:53] - Just having you here is a joy, Jen. And know that you can interrupt us and ask questions at any time.
[86:59] I'll happily drive. - Thank you.
[87:02] - Yeah, totally. Hold on. Let me get my window. Got the wrong window. There we go.
[87:08] I am now in Chrome. Cool. So what am I doing, Taylor?
[87:14] - Right. So first thing, let's go ahead and open up our issue there.
[87:19] - Yeah. - Cool.
[87:23] And we can go ahead and make a new branch, right, based on that issue number.
[87:32] - This one here? - Yeah. - Go back to Gitpod.
[87:37] Submit checkout. Feature. Defeat or feature?
[87:43] - Do you need a -b in there? - I do.
[87:48] Branch. My mistake. So the issue number is -- that is not my issue -- this one.
[87:56] 929. - 929. So this is how we keep our branches in sync.
[88:01] Not every branch is tied to an issue, but if there is an issue, we usually do feat/,
[88:07] you know, the issue number, slash or dash, you know, like a short description for the branch name.
[88:13] So now we have our new branch. We haven't changed any code.
[88:16] We're not checking out an existing branch, so, like, our yarn install and everything should be good.
[88:21] And, yeah, so to get the work-in-progress pull request, we do need at least one commit.
[88:29] You know, you can push this branch up right now if you want, but, Ramon, let's go ahead and make that first commit
[88:34] just so we can get that pull request going. You're gonna want to look in -- oh, boy.
[88:42] I want to say source/components/viz/needsassessment. Needs bar chart. There we go.
[89:04] And that would be the -- Yep, and then we can open up our data helpers, I want to say,
[89:13] because I feel like that's where a lot of this is getting pulled from, is that we have these kind of functional things.
[89:19] So you can see at the bottom there that select item, key selector, that gives us the item for the left-hand side, right,
[89:27] where it's not just the item name, but it includes, like, you know, gender, like, size, style breakdown, so we can separate, you know,
[89:34] men's T-shirts from women's T-shirts and track those as different needs. So I feel like if we just add one more bit there to the end of that string,
[89:44] right, you see where it says product item on line 25? And then what we can do is have, you know, brackets,
[89:51] like space and then, you know, curly braces. Yeah, exactly. That's great.
[89:56] Parentheses, that's the word I was looking for. We want to do product.unit.
[90:03] Like this. Right. Yep. Let's make sure that works.
[90:07] So let's go ahead and load up our needs assessment tool there. Yep, we can just click on needs.
[90:18] No, data explorer. Yep. Great.
[90:22] And so we're not seeing any changes in this graph view. Let's go ahead at the bottom and index by item instead of category.
[90:32] Oh, interesting. Okay. And then if we scroll back up, now we can see, like, hey,
[90:39] T is measured in kilograms. Most of these are measured in items, right?
[90:47] You know, I guess there's also, like, euro palettes for T, which is weird. We might need to do some normalization here.
[90:54] Some of the data might not be normalized. But that's a cool way to discover this, right?
[90:58] Because it used to be combining T as an item with T as a palette and T as kilograms, right? Those numbers do not mean the same thing.
[91:06] So I think this is a really good step in the right direction, and it has let us discover we need some normalization there.
[91:13] Got it. So I think that this is a good, like, step forward.
[91:20] Let's go ahead and commit this. This solved one of our issues, right, where if items were listed on the left-hand side,
[91:26] we wanted to show, you know, basically, like, you know, what unit they were using. Yeah.
[91:35] Okay. So I think it's a good point to commit.
[91:38] And then we can get that work in progress branch going and do the second half of this in another commit.
[91:47] Display. Units for items.
[91:55] How's that? Yeah.
[91:59] On the left-hand axis, maybe, or something like that, like, where are we displaying it? That looks great.
[92:07] Let's go ahead and commit that. So this is, like, a great example where the TypeScript checking, if that --
[92:14] if, you know, product.unit did not exist, like, there was no unit field there, the TypeScript check would catch it.
[92:21] And it looks like you forgot to add the -- I did.
[92:31] I'm usually good with that. I know, I'm just being silly.
[92:37] Cool. So just let that TypeScript check run,
[92:41] and then we want to push this branch right away. So we're not done.
[92:44] We've just made the first commit, right? And that's okay.
[92:49] Hit push origin, and then we're feet. Great.
[92:53] So now let's go to GitHub. And remote is, like, the contributor here.
[92:58] Kind of view me as the maintainer. So I'm making a new pull request.
[93:08] Yep. And don't forget, Ramon, to add the issue number.
[93:12] If you could do number 929. Exactly.
[93:18] That way it will automatically link them up. If it's just in the title or the branch name, it won't.
[93:22] And now instead of hitting create pull request, you want to select create draft pull request, right?
[93:28] Now what this does is Ramon is communicating to me by making this draft pull request, hey, like, I was assigned that issue.
[93:35] I'm working on it. Here's where I'll be working on it, right?
[93:38] So now I have a workspace. I'm like, oh, like, what's going on with this issue?
[93:42] I can see the progress Ramon has made. It's also a good place -- it gives us a place to discuss questions about the
[93:48] implementation, right? So rather than have all that comment on the issue, Ramon's like, hey, Taylor,
[93:54] does this look good? Am I done?
[93:56] I might be able to say, like, no, can we add one more thing, you know, where items are broken down, like, in the graph to that hover over thing.
[94:05] You know what I'm saying? So I feel like, you know, this is like a good way to facilitate that dialogue.
[94:11] If Ramon runs into trouble, right, I can see his code, you know? So if he has a question, I'm like, hey, why isn't this working?
[94:18] He needs some more project context. I can't do that much, you know, if it's just a blank box, right?
[94:25] But by pushing up the latest and greatest on this draft pull request, I know it's not -- I'm not going to accidentally merge it in too soon or
[94:32] something like that, right? We can have those conversations.
[94:35] We can have that Q&A. I can check out Ramon's code if I need to step through it to figure out what's
[94:40] wrong, right? It's just a much more collaborative way to work.
[94:45] Yeah. >> I have a question, Taylor.
[94:48] How do we mitigate -- how do I -- sorry, I need to stop using words like that. One counterpoint I've seen people make to draft pull requests is that when they
[95:05] drag out a little long, changes made to a main branch can create merging conflicts.
[95:15] >> Yes. >> How can we minimize that danger?
[95:19] >> So I think two things, right? I think, you know, like hopefully supported by the Gen Step Champions program
[95:26] here, we want to give people like the structure to get through contributions. So we try to keep our issues smaller, right?
[95:34] So like small issues means -- >> I like that.
[95:37] >> Pull requests, you know, and just be realistic with yourselves if you're contributing.
[95:42] Like, you know, if you have time to work on an issue, pick that issue up. If you don't, right, like, you know, then like just leave it and it might still
[95:48] be there in two weeks when you have more time or there will be another issue available, right?
[95:52] So I think part of it is like do you have time to make this contribution, right? There's no time pressure.
[95:58] But as you said, we want to keep things moving along. We want to keep our issues small.
[96:02] And the last thing is like sometimes, you know, a lot of the work that I do is like larger ranging.
[96:07] I'm adding like, you know, the beginnings of a new section to a site that then other people can like, you know, fill out with small issues.
[96:13] I sometimes just have to do a lot of rebasing. You know, I have to basically say like this is going to be a longer living
[96:19] branch, and I'll bite that bullet and keep rebasing our main branch, which is called Saga, into this one so that I make sure that my code doesn't have
[96:28] conflicts and works with other people's code. Good question, though, Ramon.
[96:34] No, thank you. I love that.
[96:37] I really love that because it shows that, you know, we're thinking about this stuff.
[96:41] Yeah. Cool.
[96:43] So I will click on draft pull request. Yep.
[96:47] And the cool thing is like this gets all the fully featured pull request stuff.
[96:51] So code C is going to generate a pull request map so that I can get an overview as a maintainer of like what files have changed and things like
[96:58] that. It will run your CI/CD, you know.
[97:01] So like I often don't run the end-to-end tests while I'm working on something, but it's nice that like by the time I'm like, oh, should I make
[97:09] this a real pull request? I can see if those end-to-end tests have passed or if they have issues, I
[97:14] got to go, you know, fix them up, right, or change my code or something. That is a really interesting point, Taylor, speaking to the merits of draft
[97:26] pull requests. Why run those tests myself if I can just push them and keep going?
[97:34] Exactly. Like it will catch it if there's an issue and you can go back and fix that,
[97:38] you know. Yeah.
[97:40] But yeah, I basically only run tests when I'm like, hey, this thing is working and it shouldn't be, and then I'll run the unit tests, you know, to
[97:46] see like how I broke something, you know. But if I'm not actually blocked in my dev flow, I'll just let the CI/DC
[97:51] server take care of that. And if I got to go in and make a few changes at the end, that's fine.
[97:56] Love it. Love it.
[97:59] Cool. I can see we've got a map here that Taylor can use to review, branch not
[98:04] deployed yet, and we can see stuff is running. It'll also create a preview URL through Netlify, which is invaluable because
[98:15] that means that our non-code contributors can go look at how it works. So like let's say like we wanted to ask for feedback, you know, from the
[98:23] people driving this issue, which is not me. That's our needs assessment team, right?
[98:28] You know, hey, does this look like y'all want it to look? Here's the Netlify preview URL.
[98:33] They can go check that out on their own time and get back to us, right? Yeah.
[98:38] But hold on a minute. Looks like something failed.
[98:43] Uh-oh. Do we got time for having a look at what failed?
[98:47] Yeah. Yeah, I think we do.
[98:50] So let's see. Nine tests failed.
[98:55] And it seems that has to do with our -- the new code we just wrote. So these labels.
[99:04] Exactly. So basically, we have some test data here in some of our tests that, you
[99:10] know, are like, hey, it should display this label with this list of items, you know, that are going to be included on the data side, right?
[99:18] And so we changed the code that governs those labels. We saw that reflected in one implementation, which is the landing site,
[99:25] but we didn't update our tests. So that's fine.
[99:29] And that's a case where like the unit tests prevent regressions. We're making forward progress.
[99:34] So now we want to update our unit tests to work with this. All right?
[99:39] Sounds good. So let's -- I can see that here.
[99:43] Options, helpers, test.ts. And it even -- it should.
[99:48] I would expect it to. What we got -- oh, yeah.
[99:53] What we had and what we got instead? No.
[99:57] Oh, yeah. Yeah, right there.
[99:59] Awesome. Let's go and fix those.
[100:01] So that's options, test. Options, helpers, test.
[100:08] It's going to be on the needs bar chart one. Yeah.
[100:12] We can see what line that was on when it failed. So that was 522.
[100:17] That's a lot of tests. Yeah, well, that's a lot of functions in there to test.
[100:22] 522. So this should be item.
[100:28] Yep. Items with an S?
[100:33] Let's find out. It is -- it is item.
[100:39] Okay. That's fine.
[100:41] That's fine. Yeah.
[100:44] And then I think we can also, like, have our tests. We might want to change up the tests so they're not both items.
[100:50] Like maybe we want to make the unit for bar soap 100 grams instead of the size style there. Right?
[100:57] So we can go look at our test data. Okay.
[101:02] Where do I do that? Where are we getting that?
[101:06] Options, helpers, test. So that data is going to be coming from -- if you scroll down -- this might break -- actually,
[101:14] this might break more stuff. I'll do this later.
[101:17] Let's just get the tests to pass and I can work in units more later. Yeah.
[101:22] Were there other tests that were failing? There's nine of them, especially search for women T-shirt.
[101:27] Maybe that's popping up somewhere else. Okay.
[101:30] Women -- actually, I'm going to go with T-shirt. Oh, filtered needs.
[101:41] I guess it would be all of these, huh? I'm not sure, but, yeah, I think it would be all of them.
[101:47] Yeah. Let's give it a try.
[101:50] And I saw one here. And one thing we might want to do is just run these tests so that we don't have to run the entire test suite.
[102:03] Let's run them locally and just -- yeah, just this file. I see what you're saying.
[102:07] Yeah. Let's fix them here so we don't have to -- so that's -- how does that work?
[102:12] Is it -- So if you do yarn test, right, and then you just do a partial.
[102:18] It doesn't even have to be the full path. You can just type in, like, options-helpers, you know, or options-helpers.test.ts, like, however you want to do it.
[102:27] It should -- it should -- There it is.
[102:30] Yep. Brilliant.
[102:36] Nice. All right.
[102:39] And we just have one more here. Huh.
[102:48] That doesn't look right. Does it?
[102:54] Received one. Should filter the needs.
[102:58] So that makes sense if our filter is off, right? So can you scroll to the bottom and see what we actually got there?
[103:04] So we got an empty array, right? And that probably has to do with what we're passing into our filter there.
[103:12] So let's just go look at this test online, 160, and see -- you know, it might not be the output we need to change. So our filter's there.
[103:25] And that's because the item, right? So 156, we need to change the item name on that filter.
[103:33] Hmm. Ooh, that's tricky.
[103:39] I understand. Now it should work.
[103:42] Okay. Great.
[103:51] Awesome. And can you just show me the UI again real quick, Ramon?
[103:54] I want to see how this changes, like, the item filter label. If we scroll to the bottom there, to our filter -- sorry, not the bottom, bottom, but just the filter section.
[104:07] There we go. And we select item.
[104:10] That should also show up with the units now. That's really cool.
[104:13] Yeah, that actually makes a lot of sense, too. I dig it.
[104:17] Great. Great.
[104:19] Okay. So I think we got those tests passing.
[104:22] Let's do one last thing here as we're fixing this up. I want to take a look at if we group by item, right?
[104:31] So if you scroll down, maybe let's, like, index by region, but then group by item. Cool.
[104:42] Right. So it also shows up there.
[104:45] So changing that one part of the code, yay, Taylor wrote good code and made it easy for future work. Yep.
[104:54] So this is a great example where, like, we went in to change one thing. We found out it changed it everywhere we needed it to be changed, and we just had to fix up the tests.
[105:03] So, Ramon, you can make this fix commit here, and then we can move the draft PR to a, like, ready-to-review PR. That was quick.
[105:15] Cool. Yep.
[105:18] Okay. That's running.
[105:29] So that's a fix. Pass.
[105:37] >> Update test data or something, yeah. >> I think that makes sense.
[105:44] >> That's great. Well, nope, nope, nope.
[105:49] Don't want to -- I keep wanting to close that tab, but then I try to -- that, of course, tries to close my browser tab. >> Okay.
[106:01] Cool. So should I share my screen now, and we can -- I can close out the PR?
[106:07] >> Let's do -- well, first, before you -- >> Actually, first, you need to mark it as not a draft.
[106:13] >> Yeah, I mean, I think before that, we've got to make sure everything's working. >> That's actually okay, right?
[106:20] So if you feel like it's ready for review, even if the tests are running or something, like, you can be like, hey, it's ready, you know? And then if the tests fail, there might still be some collaboration that happens.
[106:31] But I think the point of this, like, work-in-progress PR, like, it lets us do that collaboration while the code is being written, you know, before you get to, like -- and I think that makes open source more approachable, right? Especially if it's your first project.
[106:44] Like, so many projects are just, like, give me work-in-valid -- you know, working-valid code with tests that meet this issue, and I'll look at that as a chunk. I get it.
[106:53] If you're an overwhelm maintainer and you just want to, like, work with the folks that, like, can deliver you, you know, some functionality or something, but we want to be a more open and accepting open source project. And like we've been talking about, how people level up through their work here, and that means that we can be more involved, like, while people are writing the code, you know, and extend the collaboration to that process.
[107:17] >> Cool. >> So you can go ahead and share your screen now, and I will -- wait excitedly for my review.
[107:29] >> There we go. And I'm just going to speed run this.
[107:33] Okay. Cool.
[107:37] So we can show off one Codesy thing. We'll do more Codesy maps next week and some maintenance stuff, Ramon, maybe.
[107:43] >> Sounds good. >> Yeah, next week I'll be unseen Vue Nation, so I will not be around.
[107:48] >> Yep. >> I mean, but today -- oh, my gosh, y'all.
[107:52] I just -- I put Kiana in Tyler's office, because that's where she wanted to go. And I was like, oh, my gosh.
[108:01] And then she just started barking really loud, and he's like -- it's a bit different for him, because he has like a lot of like really big calls and stuff where, you know, live streams to me are like, it's life. You know, it's like --
[108:14] >> It's chill. >> It's chill.
[108:18] And so I'm just like -- she was just barking really a lot. And I'm just like, oh, my God.
[108:22] Just -- this is why he goes to the office. >> Do you remember that -- do you know that picture of the dog, like, staring in from outside the -- what is that called?
[108:31] The porch door? Being like, please, let me in so I can go back out.
[108:35] >> Yes. Yes.
[108:39] That is her today. She is just being very, very sassy.
[108:43] But I've been trying to pay attention. But it's interesting, even though I couldn't, like, fully go through a lot of this and ask questions as we were going today, there are things that just being a part of the community that I'm like, ooh, we really need to do a video on X that is just walking someone through this, this, and this.
[109:08] And it's already giving me, like, content ideas of how we need to structure this, just getting someone started in the community, let alone doing -- you know, going through the open source academy. So -- can we call it OSA?
[109:34] >> Open source academy. OSA.
[109:40] >> Well, I want to be careful, though, because, like, the point of this is not to teach people necessarily. I got to draw that line.
[109:45] Ramon does great work with, like, free code camp and stuff. So I'm very open to names.
[109:51] But I want to set the right -- >> Ambassadors.
[109:55] Now I just want to come up with something that's an A. Ambassadors.
[109:59] Evangelists. No, evangelists is an E.
[110:03] >> Okay. Ramon, I have approved your pull request, but we still have some tests failing.
[110:09] That's on us for -- what we should have done there is run the individual tests that we thought were failing, but then run all the unit tests at once to see if there were, like, other files. But I think that's good enough.
[110:24] Like, we showed the draft PR process. You know, we can wrap this one up pretty easily.
[110:28] We can make some more of those adjustments in the test files, and then we can merge the PR in once that check passes. So I'm feeling good.
[110:38] >> Same here. >> Yay.
[110:42] >> Cool. >> We covered a lot.
[110:46] We did a lot. I'm, like, go team.
[110:50] >> Y'all did a ton. >> I think this is great.
[110:54] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:00] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:04] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:08] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:12] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:16] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:20] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:24] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:28] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:32] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:36] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:40] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:44] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:48] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:52] >> I think we're going to wrap up. >> I think we're going to wrap up.
[111:56] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:00] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:04] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:08] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:12] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:16] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:20] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:24] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:28] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:32] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:36] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:40] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:44] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:48] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:52] >> I think we're going to wrap up. >> I think we're going to wrap up.
[112:56] >> I think we're going to wrap up. >> I think we're going to wrap up.
[113:00] >> I think we're going to wrap up. >> I think we're going to wrap up.
[113:04] >> I think we're going to wrap up. >> I think we're going to wrap up.
[113:08] >> I think we're going to wrap up. >> I think we're going to wrap up.
[113:12] >> I think we're going to wrap up. >> I think we're going to wrap up.
[113:16] >> I think we're going to wrap up. >> I think we're going to wrap up.
[113:20] >> I think we're going to wrap up. >> I think we're going to wrap up.

