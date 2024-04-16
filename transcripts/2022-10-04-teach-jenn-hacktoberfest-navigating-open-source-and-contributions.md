---
showLink: "https://www.youtube.com/watch?v=FrWG0_FZlwc"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-hacktoberfest-navigating-open-source-and-contributions"
title: "Teach Jenn Hacktoberfest: Navigating Open Source and Contributions"
publishDate: "2022-10-04"
coverImage: "https://i.ytimg.com/vi/FrWG0_FZlwc/maxresdefault.jpg"
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

[00:00] [♪♪♪] Hello, hello, beautiful humans.
[00:05] I am going live to research Hacktoberfest stuff. I have literally written down everything that I put in the
[00:17] notes of what I was gonna do and I'm like, I have to research this stuff, so I'll stream it.
[00:24] And that'll help me have the content created so I can stitch it all together and hopefully make this easier for all of you
[00:32] to consume. This is my first Hacktoberfest.
[00:37] Hacktoberfest. For some reason, that's a really hard word to say.
[00:42] And it's something that a lot of newbies are doing yet and people that have been in, you know, the coding,
[00:54] developer, engineering realm have done for many years. They've been around for nine years from what I've seen.
[01:01] So, after we go through, like, what is open source, we'll go through what is Hacktoberfest and,
[01:07] like, how to contribute, how to find people, and we'll kind of, like, stack it all together because I feel
[01:14] like you can't really go into what Hacktoberfest is without open source, but that may make it confusing,
[01:20] so I'm switching it. We're going to what is Hacktoberfest.
[01:26] [humming] All right.
[01:33] Let's share my screen. And this is, like, my favorite song because it's called
[01:43] Feeding the Ducks, in case anybody wanted to know. So, the where I would look first.
[01:51] So, Hacktoberfest, yay. I was looking at this a bit earlier because I haven't even
[01:58] signed up yet and I didn't realize that you even needed to sign up for Hacktoberfest, so that's where we're at.
[02:06] So, I just Googled "Hacktoberfest." I am pretty sure that--well, I know they are on Twitter, too.
[02:17] So, let me bring that one up. And for everyone joining today, like,
[02:26] what have you done for Hacktoberfest? Why am I, like, struggling with this?
[02:33] Because they do have a YouTube--well, they probably do. They have a Twitter account, so we got that going.
[02:46] It's one way to also find this information. Yes, I am going live again, and hi, Ben.
[02:53] Hi, Laura. Yeah, so, I'm trying to find out, like,
[03:01] I--bDougie being on the show today just made me really think about how I don't know enough about, like,
[03:12] open source or Hacktoberfest, and I'm like, it's just, like, it clicks, but it doesn't click,
[03:17] so I'm just breaking it down today. And I'm gonna have to do the research anyway,
[03:21] so might as well record it with all of you and then piece it together.
[03:27] So, Hacktoberfest, starting with the Twitter. Aw, Venya, don't worry, it'll be VOD later.
[03:40] You can come hang out with us. And plus, Venya, I'm gonna see you tomorrow, right?
[03:46] I think, I think. I should probably double-check that.
[03:52] Ben, you haven't made any yet? Oh, you did?
[03:56] Okay, well, Ben, will you send me the link to your repo so I can share that with everyone or, like--and y'all,
[04:07] I don't normally stream on LinkedIn anymore, but I am today because I think it's really important to get
[04:14] more people involved in Hacktoberfest. So, I'm trying to put it in more places just so that way people
[04:22] can get this information, ask questions, and if they want to join the full conversation with all of
[04:29] you, then they can hop over to Twitch, but just to consume it, you know,
[04:34] hang out on LinkedIn and, yay, Venya and I are hanging out tomorrow.
[04:39] So, Hacktoberfest, back to that. So, this is the official account of Hacktoberfest,
[04:46] a month-long celebration for--of open-source projects, their maintainers, and the entire community of
[04:52] contributors. Yay, exactly why I--I'm gonna go a bit deeper into what is
[05:00] Hacktoberfest because going into open-source first I don't think will explain the experience and the importance of Hacktoberfest.
[05:11] So, we're--if I could, I would have it on, like, two channels side-by-side, but I think that would get
[05:17] really confusing, and y'all, to check out Ben's repo is in the chat, so please go check it out.
[05:28] It is a surprise stream. What up, Anthony?
[05:33] You keep saying that I need to, like, do my own videos to make sure, like,
[05:37] I learn how to do this. Yes, Ben's link, I can go post Ben's link.
[05:48] I needed to do the content, so I was like, you know what, I'm just gonna, you know,
[05:55] live stream me doing the homework. Oh, there you go.
[06:04] And Laura's talking about that she tried to get more involved with OSS outside the company's OSS stuff,
[06:13] but you usually get stuck trying to find an issue that you can actually get traction on.
[06:18] Yes, yes, so that is something that we are going to go through today, hopefully today, because I think--we tried to contribute
[06:30] to a project earlier today in my first stream, it did not go great, so I'm kind of breaking these two apart of,
[06:41] you know, let's go with Hacktoberfest stuff, you know, get the basis, get what OSS is,
[06:46] get, you know, how to find projects, and then when I have my computer back and it's all set up,
[06:53] we will go through how to contribute, 'cause my computer's not my friend at the moment,
[06:59] 'cause it's not my computer, I killed mine. And thank you, Anthony, thanks, Ben,
[07:08] for helping with my broken computer stuff. Everyone that works at Microsoft,
[07:13] I love VS Code, love VS Code, love VS Code. Not necessarily the operating system.
[07:20] Anyway, carrying on. So we went through their Twitter and now we are going to
[07:27] hacktoberfest.com, and registration's open, as Anthony always reminds me, it's never big enough.
[07:36] So, yes, I am--yeah, Ryan, yeah, like, what is open source?
[07:44] We are going to do that here soon, promise. So Hacktoberfest, registration is now open,
[07:53] and, like, I gotta say, like, for whoever's sponsoring these kind of things with, like, working on a community that
[08:04] isn't always profitable yet really contributes to humankind and getting us to get further in the world,
[08:13] that is a big reason I'm passionate about Hacktoberfest. As BDougie said it so well earlier,
[08:20] it's, like, open source is, like, instead of having to start from ground zero,
[08:25] if somebody else has made the content, it will allow you to, like, start at step two instead
[08:30] of step one. And so shout-out to DigitalOcean,
[08:35] AppRite, and Docker because they're making it happen for all of us.
[08:39] So definitely want to say a shout-out to them. Whoo.
[08:44] All right, so this is also just a very giant screen itself. Y'all can go to hacktoberfest.com so you don't
[08:53] have to be stuck on the same screen I am and go at my speed.
[08:58] You can go peruse yourself. So preparing to hack, it does talk about different ways
[09:05] to be able to be a part of the community. I do like this and will be joining the Discord here
[09:12] shortly because I want to go through all of this together. [laughs]
[09:18] Yes, yes. Go get on -- thank you, Anthony, for stopping by.
[09:25] Yes, this is all -- you know, I'm going to work on getting through this, but thank you.
[09:32] So -- oh, we can make an event. That's pretty cool.
[09:40] And then I'm going to click the "How to Participate" because participation.
[09:47] I also just want to say whoever built their website, I'm very entertained by it.
[09:53] Ooh, yay, values. Everyone is welcome.
[09:57] Yay. I dig that.
[10:01] Ooh, quantity is fun, but quality is key. For those of you who were able to check out the
[10:08] stream of contributing to open source this morning with the Dougie, this is something that a lot of
[10:14] maintainers talk about because they're like, "Yo, if somebody just wants to make small changes
[10:21] in Hackathon or Hacktoberfest," which -- some people will make just very, very small changes
[10:29] to try to get that check mark of a PR is approved. So we'll go through that a bit more.
[10:36] I would also highly suggest if you're, like, new to GitHub or what a PR is, I did a stream
[10:42] when I first started this Teach Gen Tech with Wiesel from GitHub.
[10:48] Let me actually go get that link really quick because it is a great way of seeing how
[10:58] all of this is broken down. Do-do-do-do-do.
[11:04] Yay. Oh, my gosh.
[11:06] I don't know if I can watch it, though. It was from so long ago.
[11:11] For all the other streamers out there, do you ever, like, see your old content and are like,
[11:16] "Oh, my God, I can't believe you did that," because that's what I do.
[11:22] But here is -- Yes, I'm so happy.
[11:33] Thank you, Ben. Thank you.
[11:35] Because I'm like, "Uh." Getting started with GitHub.
[11:42] There we go. All right.
[11:45] So, yes. Quantity is fun, but quality is key as a maintainer.
[11:51] Ben, I can only imagine that you agree. And then a big part of the open source community
[11:59] is the fact that, like -- how to say this? Because I know we're going to go to open source
[12:06] here soon, but short-term action, long-term impact. When people are first getting into the tech world
[12:13] or wanting to become an engineer, a developer advocate, like, so many different roles.
[12:19] If you're able to show that you're contributing on GitHub to open source projects,
[12:24] you're going to learn a lot and be able to contribute to a community that they'll definitely be able
[12:31] to get a lot farther because more -- this is like the one time that it's good to have
[12:36] more chefs in the kitchen or too many hands in the cookie jar because they can --
[12:43] you could say each cookie is built on top of each other. It is also something that it shows employers
[12:50] that you are working on improving your own knowledge and contributing to others, too.
[13:00] Okay. Here we go.
[13:02] These are the details. So here's what you need to know to participate
[13:07] and complete Hacktoberfest. Number one, register at any time between
[13:13] September 26th and October 31st. We are recording this on October 3rd,
[13:20] so plenty of time to get started. Make sure you go register.
[13:25] And I will go grab that link really quick for y'all. Okay.
[13:48] And y'all are just going to get stuck with seeing too many Ts or not a T somewhere.
[13:55] This keyboard and I do not get along, but it's not my laptop.
[13:59] So we are going to get through it. It's better than no laptop since I killed mine.
[14:04] All right. So number two, pull requests can be made
[14:09] in any GitHub or GitLab-hosted projects that are participating in Hacktoberfest.
[14:15] Look for the Hacktoberfest topic. I am going to segue into a reference.
[14:31] All right. So yeah, show my chat is registered.
[14:39] Thank you, Ben, for sending this to me. So when you go to somebody's GitHub or GitLab,
[14:45] their repository, you will be able to see that in here's where the topics are and it shows Hacktoberfest.
[14:55] Something you can also do to be able to find Hacktoberfest if there's different projects that you want to work on
[15:02] is you can actually click the topic and it will be able to actually go through
[15:11] and show you places that are participating or show you repos that are participating in Hacktoberfest.
[15:19] So thank you, Ben, for letting us use yours as an example. Y'all go contribute there too.
[15:30] All right. So project maintainers must accept your pull merge request
[15:35] for them to count towards your total. Got it.
[15:38] We will be going through that in a bit. And then have four pull merge requests accepted
[15:44] between October 1st and October 31st to complete the Hacktoberfest.
[15:50] Yes, Ryan. Yes.
[15:53] Streaming again. And I love, Ben, that you were able to join
[15:57] because, Ben, you were able to give us show my .chat. And I'm excited because there's quite a few friends
[16:04] that I have that are doing open source and are maintaining for Hacktoberfest.
[16:10] Yet, like, so many people to give shout outs to. Like, BDougie with open sourced.
[16:17] Ben with show my .chat. And then Taylor with distribute aid.
[16:22] So there's a lot of options I will post later on. What are some of my favorites?
[16:28] I've named at least three of them. So, all right.
[16:34] The first 40,000 participants, maintainers, and contributors who complete Hacktoberfest
[16:40] can elect to receive one of two prizes. A tree planted in their name or a Hacktoberfest 2022 t-shirt.
[16:48] So, guess what? Sign up sooner rather than later.
[16:52] Because if you wait until the end of the month, I have a feeling you'll probably be out of the 40,000.
[17:01] And there are a lot of resources for beginners. So, you can go through all of these links.
[17:08] I'll just open them in a new tab for us real quick. All right.
[17:20] DigitalOcean, thank you for posting this. They were able to -- they made a article on introduction
[17:28] to GitHub and open source projects. Probably go through that in a bit to research that one.
[17:35] How to contribute to open source. This is from opensource.guide.
[17:40] Yay. Another DigitalOcean one.
[17:45] What is open source? And DigitalOcean how to use Git, a reference guide.
[17:53] So, these are things that I will be getting to as well in this stream. Now, something that -- as a heads up for everybody,
[18:03] I have a hard time reading through them. I do use a text-to-voice.
[18:09] That really helps me be able to consume the content. I am horribly dyslexic.
[18:16] So, there are accessibility tools that really help me. And if you want to find more out about accessibility,
[18:24] Ben does streaming about all of that. And is like your go-to person.
[18:31] Actually wrote a blog that -- I should just go find this tweet really quick. And share that.
[18:38] Because accessibility is a big thing. Of course, I'm not going to completely derail the conversation.
[18:44] Just slightly. To share this post.
[18:51] Okay. I posted it on Saturday.
[18:53] Can't be that far down. Or maybe it is.
[18:57] Maybe it's just going to be nowhere. Oh, yay.
[19:04] I found it. I found it.
[19:16] All right. So, this link is going to show my experience with voice-to-text.
[19:23] As well as link you to the article that Ben wrote. Okey-dokey.
[19:31] Okay. So, this is pretty cool.
[19:34] Because start contributing. So, the big reason that I'm making this video.
[19:40] Is because a list of beginner repos. For up4grabs.net.
[19:47] And then GitHub repositories. First contributions.
[19:51] And then also awesome for beginners. And then they also have training kits.
[19:57] So -- and sharpen your skills. So, like, you know, training kit.
[20:03] Understand GitHub flow. Get started with GitLab.
[20:07] An introduction to open source. Y'all, I might actually end up doing all of these.
[20:12] Because this is pretty cool. I love the layout.
[20:15] And then it does show you on the main page. Like, pulling -- pull merge request details.
[20:21] Like, what is out of bounds. Okay.
[20:28] So, can't be anything private. That totally makes sense.
[20:33] So, what is out of bounds? So, what is out of bounds?
[20:37] So, what is out of bounds? So, what is out of bounds?
[20:41] So, what is out of bounds? So, what is out of bounds?
[20:45] So, what is out of bounds? So, what is out of bounds?
[20:49] So, what is out of bounds? So, what is out of bounds?
[20:53] So, what is out of bounds? So, what is out of bounds?
[20:57] So, what is out of bounds? So, what is out of bounds?
[21:01] So, what is out of bounds? So, what is out of bounds?
[21:05] So, what is out of bounds? So, what is out of bounds?
[21:09] So, what is out of bounds? So, what is out of bounds?
[21:13] So, what is out of bounds? So, what is out of bounds?
[21:17] So, what is out of bounds? So, what is out of bounds?
[21:21] So, what is out of bounds? So, what is out of bounds?
[21:25] So, what is out of bounds? So, what is out of bounds?
[21:29] So, what is out of bounds? So, what is out of bounds?
[21:33] So, what is out of bounds? So, what is out of bounds?
[21:37] So, what is out of bounds? So, what is out of bounds?
[21:41] So, what is out of bounds? So, what is out of bounds?
[21:45] So, what is out of bounds? So, what is out of bounds?
[21:49] So, what is out of bounds? So, what is out of bounds?
[21:53] So, what is out of bounds? So, what is out of bounds?
[21:57] So, what is out of bounds? So, what is out of bounds?
[22:01] So, what is out of bounds? So, what is out of bounds?
[22:05] So, what is out of bounds? So, what is out of bounds?
[22:09] So, what is out of bounds? So, what is out of bounds?
[22:13] So, what is out of bounds? So, what is out of bounds?
[22:17] So, what is out of bounds? So, what is out of bounds?
[22:21] So, what is out of bounds? So, what is out of bounds?
[22:25] So, what is out of bounds? So, what is out of bounds?
[22:29] So, what is out of bounds? So, what is out of bounds?
[22:33] So, what is out of bounds? So, what is out of bounds?
[22:37] So, what is out of bounds? So, what is out of bounds?
[22:41] So, what is out of bounds? So, what is out of bounds?
[22:45] So, what is out of bounds? So, what is out of bounds?
[22:49] So, what is out of bounds? So, what is out of bounds?
[22:53] So, what is out of bounds? So, what is out of bounds?
[22:57] So, what is out of bounds? So, what is out of bounds?
[23:01] So, what is out of bounds? So, what is out of bounds?
[23:05] So, what is out of bounds? So, what is out of bounds?
[23:09] So, what is out of bounds? So, what is out of bounds?
[23:13] So, what is out of bounds? So, what is out of bounds?
[23:17] So, what is out of bounds? So, what is out of bounds?
[23:21] So, what is out of bounds? So, what is out of bounds?
[23:25] So, what is out of bounds? So, what is out of bounds?
[23:29] So, what is out of bounds? So, what is out of bounds?
[23:33] So, what is out of bounds? So, what is out of bounds?
[23:37] So, what is out of bounds? So, what is out of bounds?
[23:41] So, what is out of bounds? So, what is out of bounds?
[23:45] So, what is out of bounds? So, what is out of bounds?
[23:49] So, what is out of bounds? So, what is out of bounds?
[23:53] So, what is out of bounds? So, what is out of bounds?
[23:57] So, what is out of bounds? So, what is out of bounds?
[24:01] So, what is out of bounds? So, what is out of bounds?
[24:05] So, what is out of bounds? So, what is out of bounds?
[24:09] So, what is out of bounds? So, what is out of bounds?
[24:13] So, what is out of bounds? So, what is out of bounds?
[24:17] So, what is out of bounds? So, what is out of bounds?
[24:21] So, what is out of bounds? So, what is out of bounds?
[24:25] So, what is out of bounds? So, what is out of bounds?
[24:29] So, what is out of bounds? So, what is out of bounds?
[24:33] So, what is out of bounds? So, what is out of bounds?
[24:37] So, what is out of bounds? So, what is out of bounds?
[24:41] So, what is out of bounds? So, what is out of bounds?
[24:45] So, what is out of bounds? So, what is out of bounds?
[24:49] So, what is out of bounds? So, what is out of bounds?
[24:53] So, what is out of bounds? So, what is out of bounds?
[24:57] So, what is out of bounds? So, what is out of bounds?
[25:01] So, what is out of bounds? So, what is out of bounds?
[25:05] So, what is out of bounds? So, what is out of bounds?
[25:09] So, what is out of bounds? So, what is out of bounds?
[25:13] So, what is out of bounds? So, what is out of bounds?
[25:17] So, what is out of bounds? So, what is out of bounds?
[25:21] So, what is out of bounds? So, what is out of bounds?
[25:25] So, what is out of bounds? So, what is out of bounds?
[25:29] So, what is out of bounds? So, what is out of bounds?
[25:33] So, what is out of bounds? So, what is out of bounds?
[25:37] So, what is out of bounds? So, what is out of bounds?
[25:41] So, what is out of bounds? So, what is out of bounds?
[25:45] So, what is out of bounds? So, what is out of bounds?
[25:49] So, what is out of bounds? So, what is out of bounds?
[25:53] So, what is out of bounds? So, what is out of bounds?
[25:57] So, what is out of bounds? So, what is out of bounds?
[26:01] So, what is out of bounds? So, what is out of bounds?
[26:05] So, what is out of bounds? So, what is out of bounds?
[26:09] So, what is out of bounds? So, what is out of bounds?
[26:13] So, what is out of bounds? So, what is out of bounds?
[26:17] So, what is out of bounds? So, what is out of bounds?
[26:21] So, what is out of bounds? So, what is out of bounds?
[26:25] So, what is out of bounds? So, what is out of bounds?
[26:29] So, what is out of bounds? So, what is out of bounds?
[26:33] So, what is out of bounds? So, what is out of bounds?
[26:37] So, what is out of bounds? So, what is out of bounds?
[26:41] So, what is out of bounds? So, what is out of bounds?
[26:45] So, what is out of bounds? So, what is out of bounds?
[26:49] So, what is out of bounds? So, what is out of bounds?
[26:53] So, what is out of bounds? So, what is out of bounds?
[26:57] So, what is out of bounds? So, what is out of bounds?
[27:01] So, what is out of bounds? So, what is out of bounds?
[27:05] So, what is out of bounds? So, what is out of bounds?
[27:09] So, what is out of bounds? So, what is out of bounds?
[27:13] So, what is out of bounds? So, what is out of bounds?
[27:17] So, what is out of bounds? So, what is out of bounds?
[27:21] So, what is out of bounds? So, what is out of bounds?
[27:25] So, what is out of bounds? So, what is out of bounds?
[27:29] So, what is out of bounds? So, what is out of bounds?
[27:33] So, what is out of bounds? So, what is out of bounds?
[27:37] So, what is out of bounds? So, what is out of bounds?
[27:41] So, what is out of bounds? So, what is out of bounds?
[27:45] So, what is out of bounds? So, what is out of bounds?
[27:49] So, what is out of bounds? So, what is out of bounds?
[27:53] So, what is out of bounds? So, what is out of bounds?
[27:57] So, what is out of bounds? So, what is out of bounds?
[28:01] So, what is out of bounds? So, what is out of bounds?
[28:05] So, what is out of bounds? So, what is out of bounds?
[28:09] So, what is out of bounds? So, what is out of bounds?
[28:13] So, what is out of bounds? So, what is out of bounds?
[28:17] So, what is out of bounds? So, what is out of bounds?
[28:21] So, what is out of bounds? So, what is out of bounds?
[28:25] So, what is out of bounds? So, what is out of bounds?
[28:29] So, what is out of bounds? So, what is out of bounds?
[28:33] So, what is out of bounds? So, what is out of bounds?
[28:37] So, what is out of bounds? So, what is out of bounds?
[28:41] So, what is out of bounds? So, what is out of bounds?
[28:45] So, what is out of bounds? So, what is out of bounds?
[28:49] So, what is out of bounds? So, what is out of bounds?
[28:53] So, what is out of bounds? So, what is out of bounds?
[28:57] So, what is out of bounds? So, what is out of bounds?
[29:01] So, what is out of bounds? So, what is out of bounds?
[29:05] So, what is out of bounds? So, what is out of bounds?
[29:09] So, what is out of bounds? So, what is out of bounds?
[29:13] So, what is out of bounds? So, what is out of bounds?
[29:17] So, what is out of bounds? So, what is out of bounds?
[29:21] So, what is out of bounds? So, what is out of bounds?
[29:25] So, what is out of bounds? So, what is out of bounds?
[29:29] So, what is out of bounds? So, what is out of bounds?
[29:33] So, what is out of bounds? So, what is out of bounds?
[29:37] So, what is out of bounds? So, what is out of bounds?
[29:41] So, what is out of bounds? So, what is out of bounds?
[29:45] So, what is out of bounds? So, what is out of bounds?
[29:49] So, what is out of bounds? So, what is out of bounds?
[29:53] So, what is out of bounds? So, what is out of bounds?
[29:57] So, what is out of bounds? So, what is out of bounds?
[30:01] So, what is out of bounds? So, what is out of bounds?
[30:05] So, what is out of bounds? So, what is out of bounds?
[30:09] So, what is out of bounds? So, what is out of bounds?
[30:13] So, what is out of bounds? So, what is out of bounds?
[30:17] So, what is out of bounds? So, what is out of bounds?
[30:21] So, what is out of bounds? So, what is out of bounds?
[30:25] So, what is out of bounds? So, what is out of bounds?
[30:29] So, what is out of bounds? So, what is out of bounds?
[30:33] So, what is out of bounds? So, what is out of bounds?
[30:37] So, what is out of bounds? So, what is out of bounds?
[30:41] So, what is out of bounds? So, what is out of bounds?
[30:45] So, what is out of bounds? So, what is out of bounds?
[30:49] So, what is out of bounds? So, what is out of bounds?
[30:53] So, what is out of bounds? So, what is out of bounds?
[30:57] So, what is out of bounds? So, what is out of bounds?
[31:01] So, what is out of bounds? So, what is out of bounds?
[31:05] So, what is out of bounds? So, what is out of bounds?
[31:09] So, what is out of bounds? So, what is out of bounds?
[31:13] So, what is out of bounds? So, what is out of bounds?
[31:17] So, what is out of bounds? So, what is out of bounds?
[31:21] So, what is out of bounds? So, what is out of bounds?
[31:25] So, what is out of bounds? So, what is out of bounds?
[31:29] So, what is out of bounds? So, what is out of bounds?
[31:33] So, what is out of bounds? So, what is out of bounds?
[31:37] So, what is out of bounds? So, what is out of bounds?
[31:41] So, what is out of bounds? So, what is out of bounds?
[31:45] So, what is out of bounds? So, what is out of bounds?
[31:49] So, what is out of bounds? So, what is out of bounds?
[31:53] So, what is out of bounds? So, what is out of bounds?
[31:57] So, what is out of bounds? So, what is out of bounds?
[32:01] So, what is out of bounds? So, what is out of bounds?
[32:05] So, what is out of bounds? So, what is out of bounds?
[32:09] So, what is out of bounds? So, what is out of bounds?
[32:13] So, what is out of bounds? So, what is out of bounds?
[32:17] So, what is out of bounds? So, what is out of bounds?
[32:21] So, what is out of bounds? So, what is out of bounds?
[32:25] So, what is out of bounds? So, what is out of bounds?
[32:29] So, what is out of bounds? So, what is out of bounds?
[32:33] So, what is out of bounds? So, what is out of bounds?
[32:37] So, what is out of bounds? So, what is out of bounds?
[32:41] So, what is out of bounds? So, what is out of bounds?
[32:45] So, what is out of bounds? So, what is out of bounds?
[32:49] So, what is out of bounds? So, what is out of bounds?
[32:53] So, what is out of bounds? So, what is out of bounds?
[32:57] So, what is out of bounds? So, what is out of bounds?
[33:01] So, what is out of bounds? So, what is out of bounds?
[33:05] So, what is out of bounds? So, what is out of bounds?
[33:09] So, what is out of bounds? So, what is out of bounds?
[33:13] So, what is out of bounds? So, what is out of bounds?
[33:17] So, what is out of bounds? So, what is out of bounds?
[33:21] So, what is out of bounds? So, what is out of bounds?
[33:25] So, what is out of bounds? So, what is out of bounds?
[33:29] So, what is out of bounds? So, what is out of bounds?
[33:33] So, what is out of bounds? So, what is out of bounds?
[33:37] So, what is out of bounds? So, what is out of bounds?
[33:41] So, what is out of bounds? So, what is out of bounds?
[33:45] So, what is out of bounds? So, what is out of bounds?
[33:49] So, what is out of bounds? So, what is out of bounds?
[33:53] So, what is out of bounds? So, what is out of bounds?
[33:57] So, what is out of bounds? So, what is out of bounds?
[34:01] So, what is out of bounds? So, what is out of bounds?
[34:05] So, what is out of bounds? So, what is out of bounds?
[34:09] So, what is out of bounds? So, what is out of bounds?
[34:13] So, what is out of bounds? So, what is out of bounds?
[34:17] So, what is out of bounds? So, what is out of bounds?
[34:21] So, what is out of bounds? So, what is out of bounds?
[34:25] So, what is out of bounds? So, what is out of bounds?
[34:29] So, what is out of bounds? So, what is out of bounds?
[34:33] So, what is out of bounds? So, what is out of bounds?
[34:37] So, what is out of bounds? So, what is out of bounds?
[34:41] So, what is out of bounds? So, what is out of bounds?
[34:45] So, what is out of bounds? So, what is out of bounds?
[34:49] So, what is out of bounds? So, what is out of bounds?
[34:53] So, what is out of bounds? So, what is out of bounds?
[34:57] So, what is out of bounds? So, what is out of bounds?
[35:01] So, what is out of bounds? So, what is out of bounds?
[35:05] So, what is out of bounds? So, what is out of bounds?
[35:09] So, what is out of bounds? So, what is out of bounds?
[35:13] So, what is out of bounds? So, what is out of bounds?
[35:17] So, what is out of bounds? So, what is out of bounds?
[35:21] So, what is out of bounds? So, what is out of bounds?
[35:25] So, what is out of bounds? So, what is out of bounds?
[35:29] So, what is out of bounds? So, what is out of bounds?
[35:33] So, what is out of bounds? So, what is out of bounds?
[35:37] So, what is out of bounds? So, what is out of bounds?
[35:41] So, what is out of bounds? So, what is out of bounds?
[35:45] So, what is out of bounds? So, what is out of bounds?
[35:49] So, what is out of bounds? So, what is out of bounds?
[35:53] So, what is out of bounds? So, what is out of bounds?
[35:57] So, what is out of bounds? So, what is out of bounds?
[36:01] So, what is out of bounds? So, what is out of bounds?
[36:05] So, what is out of bounds? So, what is out of bounds?
[36:09] So, what is out of bounds? So, what is out of bounds?
[36:13] So, what is out of bounds? So, what is out of bounds?
[36:17] So, what is out of bounds? So, what is out of bounds?
[36:21] So, what is out of bounds? So, what is out of bounds?
[36:25] So, what is out of bounds? So, what is out of bounds?
[36:29] So, what is out of bounds? So, what is out of bounds?
[36:33] So, what is out of bounds? So, what is out of bounds?
[36:37] So, what is out of bounds? So, what is out of bounds?
[36:41] So, what is out of bounds? So, what is out of bounds?
[36:45] So, what is out of bounds? So, what is out of bounds?
[36:49] So, what is out of bounds? So, what is out of bounds?
[36:53] So, what is out of bounds? So, what is out of bounds?
[36:57] So, what is out of bounds? So, what is out of bounds?
[37:01] So, what is out of bounds? So, what is out of bounds?
[37:05] So, what is out of bounds? So, what is out of bounds?
[37:09] So, what is out of bounds? So, what is out of bounds?
[37:13] So, what is out of bounds? So, what is out of bounds?
[37:17] So, what is out of bounds? So, what is out of bounds?
[37:21] So, what is out of bounds? So, what is out of bounds?
[37:25] So, what is out of bounds? So, what is out of bounds?
[37:29] So, what is out of bounds? So, what is out of bounds?
[37:33] So, what is out of bounds? So, what is out of bounds?
[37:37] So, what is out of bounds? So, what is out of bounds?
[37:41] So, what is out of bounds? So, what is out of bounds?
[37:45] So, what is out of bounds? So, what is out of bounds?
[37:49] So, what is out of bounds? So, what is out of bounds?
[37:53] So, what is out of bounds? So, what is out of bounds?
[37:57] So, what is out of bounds? So, what is out of bounds?
[38:01] So, what is out of bounds? So, what is out of bounds?
[38:05] So, what is out of bounds? So, what is out of bounds?
[38:09] So, what is out of bounds? So, what is out of bounds?
[38:13] So, what is out of bounds? So, what is out of bounds?
[38:17] So, what is out of bounds? So, what is out of bounds?
[38:21] So, what is out of bounds? So, what is out of bounds?
[38:25] So, what is out of bounds? So, what is out of bounds?
[38:29] So, what is out of bounds? So, what is out of bounds?
[38:33] So, what is out of bounds? So, what is out of bounds?
[38:37] So, what is out of bounds? So, what is out of bounds?
[38:41] So, what is out of bounds? So, what is out of bounds?
[38:45] So, what is out of bounds? So, what is out of bounds?
[38:49] So, what is out of bounds? So, what is out of bounds?
[38:53] So, what is out of bounds? So, what is out of bounds?
[38:57] So, what is out of bounds? So, what is out of bounds?
[39:01] So, what is out of bounds? So, what is out of bounds?
[39:05] So, what is out of bounds? So, what is out of bounds?
[39:09] So, what is out of bounds? So, what is out of bounds?
[39:13] So, what is out of bounds? So, what is out of bounds?
[39:17] So, what is out of bounds? So, what is out of bounds?
[39:21] So, what is out of bounds? So, what is out of bounds?
[39:25] So, what is out of bounds? So, what is out of bounds?
[39:29] So, what is out of bounds? So, what is out of bounds?
[39:33] So, what is out of bounds? So, what is out of bounds?
[39:37] So, what is out of bounds? So, what is out of bounds?
[39:41] So, what is out of bounds? So, what is out of bounds?
[39:45] So, what is out of bounds? So, what is out of bounds?
[39:49] So, what is out of bounds? So, what is out of bounds?
[39:53] So, what is out of bounds? So, what is out of bounds?
[39:57] So, what is out of bounds? So, what is out of bounds?
[40:01] So, what is out of bounds? So, what is out of bounds?
[40:05] So, what is out of bounds? So, what is out of bounds?
[40:09] So, what is out of bounds? So, what is out of bounds?
[40:13] So, what is out of bounds? So, what is out of bounds?
[40:17] So, what is out of bounds? So, what is out of bounds?
[40:21] So, what is out of bounds? So, what is out of bounds?
[40:25] So, what is out of bounds? So, what is out of bounds?
[40:29] So, what is out of bounds? So, what is out of bounds?
[40:33] So, what is out of bounds? So, what is out of bounds?
[40:37] So, what is out of bounds? So, what is out of bounds?
[40:41] So, what is out of bounds? So, what is out of bounds?
[40:45] So, what is out of bounds? So, what is out of bounds?
[40:49] So, what is out of bounds? So, what is out of bounds?
[40:53] So, what is out of bounds? So, what is out of bounds?
[40:57] So, what is out of bounds? So, what is out of bounds?
[41:01] So, what is out of bounds? So, what is out of bounds?
[41:05] So, what is out of bounds? So, what is out of bounds?
[41:09] So, what is out of bounds? So, what is out of bounds?
[41:13] So, what is out of bounds? So, what is out of bounds?
[41:17] So, what is out of bounds? So, what is out of bounds?
[41:21] So, what is out of bounds? So, what is out of bounds?
[41:25] So, what is out of bounds? So, what is out of bounds?
[41:29] So, what is out of bounds? So, what is out of bounds?
[41:33] So, what is out of bounds? So, what is out of bounds?
[41:37] So, what is out of bounds? So, what is out of bounds?
[41:41] So, what is out of bounds? So, what is out of bounds?
[41:45] So, what is out of bounds? So, what is out of bounds?
[41:49] So, what is out of bounds? So, what is out of bounds?
[41:53] So, what is out of bounds? So, what is out of bounds?
[41:57] So, what is out of bounds? So, what is out of bounds?
[42:01] So, what is out of bounds? So, what is out of bounds?
[42:05] So, what is out of bounds? So, what is out of bounds?
[42:09] So, what is out of bounds? So, what is out of bounds?
[42:13] So, what is out of bounds? So, what is out of bounds?
[42:17] So, what is out of bounds? So, what is out of bounds?
[42:21] So, what is out of bounds? So, what is out of bounds?
[42:25] So, what is out of bounds? So, what is out of bounds?
[42:29] So, what is out of bounds? So, what is out of bounds?
[42:33] So, what is out of bounds? So, what is out of bounds?
[42:37] So, what is out of bounds? So, what is out of bounds?
[42:41] So, what is out of bounds? So, what is out of bounds?
[42:45] So, what is out of bounds? So, what is out of bounds?
[42:49] So, what is out of bounds? So, what is out of bounds?
[42:53] So, what is out of bounds? So, what is out of bounds?
[42:57] So, what is out of bounds? So, what is out of bounds?
[43:01] So, what is out of bounds? So, what is out of bounds?
[43:05] So, what is out of bounds? So, what is out of bounds?
[43:09] So, what is out of bounds? So, what is out of bounds?
[43:13] So, what is out of bounds? So, what is out of bounds?
[43:17] So, what is out of bounds? So, what is out of bounds?
[43:21] So, what is out of bounds? So, what is out of bounds?
[43:25] So, what is out of bounds? So, what is out of bounds?
[43:29] So, what is out of bounds? So, what is out of bounds?
[43:33] So, what is out of bounds? So, what is out of bounds?
[43:37] So, what is out of bounds? So, what is out of bounds?
[43:41] So, what is out of bounds? So, what is out of bounds?
[43:45] So, what is out of bounds? So, what is out of bounds?
[43:49] So, what is out of bounds? So, what is out of bounds?
[43:53] So, what is out of bounds? So, what is out of bounds?
[43:57] So, what is out of bounds? So, what is out of bounds?
[44:01] So, what is out of bounds? So, what is out of bounds?
[44:05] So, what is out of bounds? So, what is out of bounds?
[44:09] So, what is out of bounds? So, what is out of bounds?
[44:13] So, what is out of bounds? So, what is out of bounds?
[44:17] So, what is out of bounds? So, what is out of bounds?
[44:21] So, what is out of bounds? So, what is out of bounds?
[44:25] So, what is out of bounds? So, what is out of bounds?
[44:29] So, what is out of bounds? So, what is out of bounds?
[44:33] So, what is out of bounds? So, what is out of bounds?
[44:37] So, what is out of bounds? So, what is out of bounds?
[44:41] So, what is out of bounds? So, what is out of bounds?
[44:45] So, what is out of bounds? So, what is out of bounds?
[44:49] So, what is out of bounds? So, what is out of bounds?
[44:53] So, what is out of bounds? So, what is out of bounds?
[44:57] So, what is out of bounds? So, what is out of bounds?
[45:01] So, what is out of bounds? So, what is out of bounds?
[45:05] So, what is out of bounds? So, what is out of bounds?
[45:09] So, what is out of bounds? So, what is out of bounds?
[45:13] So, what is out of bounds? So, what is out of bounds?
[45:17] So, what is out of bounds? So, what is out of bounds?
[45:21] So, what is out of bounds? So, what is out of bounds?
[45:25] So, what is out of bounds? So, what is out of bounds?
[45:29] So, what is out of bounds? So, what is out of bounds?
[45:33] So, what is out of bounds? So, what is out of bounds?
[45:37] So, what is out of bounds? So, what is out of bounds?
[45:41] So, what is out of bounds? So, what is out of bounds?
[45:45] So, what is out of bounds? So, what is out of bounds?
[45:49] So, what is out of bounds? So, what is out of bounds?
[45:53] So, what is out of bounds? So, what is out of bounds?
[45:57] So, what is out of bounds? So, what is out of bounds?
[46:01] So, what is out of bounds? So, what is out of bounds?
[46:05] So, what is out of bounds? So, what is out of bounds?
[46:09] So, what is out of bounds? So, what is out of bounds?
[46:13] So, what is out of bounds? So, what is out of bounds?
[46:17] So, what is out of bounds? So, what is out of bounds?
[46:21] So, what is out of bounds? So, what is out of bounds?
[46:25] So, what is out of bounds? So, what is out of bounds?
[46:29] So, what is out of bounds? So, what is out of bounds?
[46:33] So, what is out of bounds? So, what is out of bounds?
[46:37] So, what is out of bounds? So, what is out of bounds?
[46:41] So, what is out of bounds? So, what is out of bounds?
[46:45] So, what is out of bounds? So, what is out of bounds?
[46:49] So, what is out of bounds? So, what is out of bounds?
[46:53] So, what is out of bounds? So, what is out of bounds?
[46:57] So, what is out of bounds? So, what is out of bounds?
[47:01] So, what is out of bounds? So, what is out of bounds?
[47:05] So, what is out of bounds? So, what is out of bounds?
[47:09] So, what is out of bounds? So, what is out of bounds?
[47:13] So, what is out of bounds? So, what is out of bounds?
[47:17] So, what is out of bounds? So, what is out of bounds?
[47:21] So, what is out of bounds? So, what is out of bounds?
[47:25] So, what is out of bounds? So, what is out of bounds?
[47:29] So, what is out of bounds? So, what is out of bounds?
[47:33] So, what is out of bounds? So, what is out of bounds?
[47:37] So, what is out of bounds? So, what is out of bounds?
[47:41] So, what is out of bounds? So, what is out of bounds?
[47:45] So, what is out of bounds? So, what is out of bounds?
[47:49] So, what is out of bounds? So, what is out of bounds?
[47:53] So, what is out of bounds? So, what is out of bounds?
[47:57] So, what is out of bounds? So, what is out of bounds?
[48:01] So, what is out of bounds? So, what is out of bounds?
[48:05] So, what is out of bounds? So, what is out of bounds?
[48:09] So, what is out of bounds? So, what is out of bounds?
[48:13] So, what is out of bounds? So, what is out of bounds?
[48:17] So, what is out of bounds? So, what is out of bounds?
[48:21] So, what is out of bounds? So, what is out of bounds?
[48:25] So, what is out of bounds? So, what is out of bounds?
[48:29] So, what is out of bounds? So, what is out of bounds?
[48:33] So, what is out of bounds? So, what is out of bounds?
[48:37] So, what is out of bounds? So, what is out of bounds?
[48:41] So, what is out of bounds? So, what is out of bounds?
[48:45] So, what is out of bounds? So, what is out of bounds?
[48:49] So, what is out of bounds? So, what is out of bounds?
[48:53] So, what is out of bounds? So, what is out of bounds?
[48:57] So, what is out of bounds? So, what is out of bounds?
[49:01] So, what is out of bounds? So, what is out of bounds?
[49:05] So, what is out of bounds? So, what is out of bounds?
[49:09] So, what is out of bounds? So, what is out of bounds?
[49:13] So, what is out of bounds? So, what is out of bounds?
[49:17] So, what is out of bounds? So, what is out of bounds?
[49:21] So, what is out of bounds? So, what is out of bounds?
[49:25] So, what is out of bounds? So, what is out of bounds?
[49:29] So, what is out of bounds? So, what is out of bounds?
[49:33] So, what is out of bounds? So, what is out of bounds?
[49:37] So, what is out of bounds? So, what is out of bounds?
[49:41] So, what is out of bounds? So, what is out of bounds?
[49:45] So, what is out of bounds? So, what is out of bounds?
[49:49] So, what is out of bounds? So, what is out of bounds?
[49:53] So, what is out of bounds? So, what is out of bounds?
[49:57] So, what is out of bounds? So, what is out of bounds?
[50:01] So, what is out of bounds? So, what is out of bounds?
[50:05] So, what is out of bounds? So, what is out of bounds?
[50:09] So, what is out of bounds? So, what is out of bounds?
[50:13] So, what is out of bounds? So, what is out of bounds?
[50:17] So, what is out of bounds? So, what is out of bounds?
[50:21] So, what is out of bounds? So, what is out of bounds?
[50:25] So, what is out of bounds? So, what is out of bounds?
[50:29] So, what is out of bounds? So, what is out of bounds?
[50:33] So, what is out of bounds? So, what is out of bounds?
[50:37] So, what is out of bounds? So, what is out of bounds?
[50:41] So, what is out of bounds? So, what is out of bounds?
[50:45] So, what is out of bounds? So, what is out of bounds?
[50:49] So, what is out of bounds? So, what is out of bounds?
[50:53] So, what is out of bounds? So, what is out of bounds?
[50:57] So, what is out of bounds? So, what is out of bounds?
[51:01] So, what is out of bounds? So, what is out of bounds?
[51:05] So, what is out of bounds? So, what is out of bounds?
[51:09] So, what is out of bounds? So, what is out of bounds?
[51:13] So, what is out of bounds? So, what is out of bounds?
[51:17] So, what is out of bounds? So, what is out of bounds?
[51:21] So, what is out of bounds? So, what is out of bounds?
[51:25] So, what is out of bounds? So, what is out of bounds?
[51:29] So, what is out of bounds? So, what is out of bounds?
[51:33] So, what is out of bounds? So, what is out of bounds?
[51:37] So, what is out of bounds? So, what is out of bounds?
[51:41] So, what is out of bounds? So, what is out of bounds?
[51:45] So, what is out of bounds? So, what is out of bounds?
[51:49] So, what is out of bounds? So, what is out of bounds?
[51:53] So, what is out of bounds? So, what is out of bounds?
[51:57] So, what is out of bounds? So, what is out of bounds?
[52:01] So, what is out of bounds? So, what is out of bounds?
[52:05] So, what is out of bounds? So, what is out of bounds?
[52:09] So, what is out of bounds? So, what is out of bounds?
[52:13] So, what is out of bounds? So, what is out of bounds?
[52:17] So, what is out of bounds? So, what is out of bounds?
[52:21] So, what is out of bounds? So, what is out of bounds?
[52:25] So, what is out of bounds? So, what is out of bounds?
[52:29] So, what is out of bounds? So, what is out of bounds?
[52:33] So, what is out of bounds? So, what is out of bounds?
[52:37] So, what is out of bounds? So, what is out of bounds?
[52:41] So, what is out of bounds? So, what is out of bounds?
[52:45] So, what is out of bounds? So, what is out of bounds?
[52:49] So, what is out of bounds? So, what is out of bounds?
[52:53] So, what is out of bounds? So, what is out of bounds?
[52:57] So, what is out of bounds? So, what is out of bounds?
[53:01] So, what is out of bounds? So, what is out of bounds?
[53:05] So, what is out of bounds? So, what is out of bounds?
[53:09] So, what is out of bounds? So, what is out of bounds?
[53:13] So, what is out of bounds? So, what is out of bounds?
[53:17] So, what is out of bounds? So, what is out of bounds?
[53:21] So, what is out of bounds? So, what is out of bounds?
[53:25] So, what is out of bounds? So, what is out of bounds?
[53:29] So, what is out of bounds? So, what is out of bounds?
[53:33] So, what is out of bounds? So, what is out of bounds?
[53:37] So, what is out of bounds? So, what is out of bounds?
[53:41] So, what is out of bounds? So, what is out of bounds?
[53:45] So, what is out of bounds? So, what is out of bounds?
[53:49] So, what is out of bounds? So, what is out of bounds?
[53:53] So, what is out of bounds? So, what is out of bounds?
[53:57] So, what is out of bounds? So, what is out of bounds?
[54:01] So, what is out of bounds? So, what is out of bounds?
[54:05] So, what is out of bounds? So, what is out of bounds?
[54:09] So, what is out of bounds? So, what is out of bounds?
[54:13] So, what is out of bounds? So, what is out of bounds?
[54:17] So, what is out of bounds? So, what is out of bounds?
[54:21] So, what is out of bounds? So, what is out of bounds?
[54:25] So, what is out of bounds? So, what is out of bounds?
[54:29] So, what is out of bounds? So, what is out of bounds?
[54:33] So, what is out of bounds? So, what is out of bounds?
[54:37] So, what is out of bounds? So, what is out of bounds?
[54:41] So, what is out of bounds? So, what is out of bounds?
[54:45] So, what is out of bounds? So, what is out of bounds?
[54:49] So, what is out of bounds? So, what is out of bounds?
[54:53] So, what is out of bounds? So, what is out of bounds?
[54:57] So, what is out of bounds? So, what is out of bounds?
[55:01] So, what is out of bounds? So, what is out of bounds?
[55:05] So, what is out of bounds? So, what is out of bounds?
[55:09] So, what is out of bounds? So, what is out of bounds?
[55:13] So, what is out of bounds? So, what is out of bounds?
[55:17] So, what is out of bounds? So, what is out of bounds?
[55:21] So, what is out of bounds? So, what is out of bounds?
[55:25] So, what is out of bounds? So, what is out of bounds?
[55:29] So, what is out of bounds? So, what is out of bounds?
[55:33] So, what is out of bounds? So, what is out of bounds?
[55:37] So, what is out of bounds? So, what is out of bounds?
[55:41] So, what is out of bounds? So, what is out of bounds?
[55:45] So, what is out of bounds? So, what is out of bounds?
[55:49] So, what is out of bounds? So, what is out of bounds?
[55:53] So, what is out of bounds? So, what is out of bounds?
[55:57] So, what is out of bounds? So, what is out of bounds?
[56:01] So, what is out of bounds? So, what is out of bounds?
[56:05] So, what is out of bounds? So, what is out of bounds?
[56:09] So, what is out of bounds? So, what is out of bounds?
[56:13] So, what is out of bounds? So, what is out of bounds?
[56:17] So, what is out of bounds? So, what is out of bounds?
[56:21] So, what is out of bounds? So, what is out of bounds?
[56:25] So, what is out of bounds? So, what is out of bounds?
[56:29] So, what is out of bounds? So, what is out of bounds?
[56:33] So, what is out of bounds? So, what is out of bounds?
[56:37] So, what is out of bounds? So, what is out of bounds?
[56:41] So, what is out of bounds? So, what is out of bounds?
[56:45] So, what is out of bounds? So, what is out of bounds?
[56:49] So, what is out of bounds? So, what is out of bounds?
[56:53] So, what is out of bounds? So, what is out of bounds?
[56:57] So, what is out of bounds? So, what is out of bounds?
[57:01] So, what is out of bounds? So, what is out of bounds?
[57:05] So, what is out of bounds? So, what is out of bounds?
[57:09] So, what is out of bounds? So, what is out of bounds?
[57:13] So, what is out of bounds? So, what is out of bounds?
[57:17] So, what is out of bounds? So, what is out of bounds?
[57:21] So, what is out of bounds? So, what is out of bounds?
[57:25] So, what is out of bounds? So, what is out of bounds?
[57:29] So, what is out of bounds? So, what is out of bounds?
[57:33] So, what is out of bounds? So, what is out of bounds?
[57:37] So, what is out of bounds? So, what is out of bounds?
[57:41] So, what is out of bounds? So, what is out of bounds?
[57:45] So, what is out of bounds? So, what is out of bounds?
[57:49] So, what is out of bounds? So, what is out of bounds?
[57:53] So, what is out of bounds? So, what is out of bounds?
[57:57] So, what is out of bounds? So, what is out of bounds?
[58:01] So, what is out of bounds? So, what is out of bounds?
[58:05] So, what is out of bounds? So, what is out of bounds?
[58:09] So, what is out of bounds? So, what is out of bounds?
[58:13] So, what is out of bounds? So, what is out of bounds?
[58:17] So, what is out of bounds? So, what is out of bounds?
[58:21] So, what is out of bounds? So, what is out of bounds?
[58:25] So, what is out of bounds? So, what is out of bounds?
[58:29] So, what is out of bounds? So, what is out of bounds?
[58:33] So, what is out of bounds? So, what is out of bounds?
[58:37] So, what is out of bounds? So, what is out of bounds?
[58:41] So, what is out of bounds? So, what is out of bounds?
[58:45] So, what is out of bounds? So, what is out of bounds?
[58:49] So, what is out of bounds? So, what is out of bounds?
[58:53] So, what is out of bounds? So, what is out of bounds?
[58:57] So, what is out of bounds? So, what is out of bounds?
[59:01] So, what is out of bounds? So, what is out of bounds?
[59:05] So, what is out of bounds? So, what is out of bounds?
[59:09] So, what is out of bounds? So, what is out of bounds?
[59:13] So, what is out of bounds? So, what is out of bounds?
[59:17] So, what is out of bounds? So, what is out of bounds?
[59:21] So, what is out of bounds? So, what is out of bounds?
[59:25] So, what is out of bounds? So, what is out of bounds?
[59:29] So, what is out of bounds? So, what is out of bounds?
[59:33] So, what is out of bounds? So, what is out of bounds?
[59:37] So, what is out of bounds? So, what is out of bounds?
[59:41] So, what is out of bounds? So, what is out of bounds?
[59:45] So, what is out of bounds? So, what is out of bounds?
[59:49] So, what is out of bounds? So, what is out of bounds?
[59:53] So, what is out of bounds? So, what is out of bounds?
[59:57] So, what is out of bounds? So, what is out of bounds?
[60:01] So, what is out of bounds? So, what is out of bounds?
[60:05] So, what is out of bounds? So, what is out of bounds?
[60:09] So, what is out of bounds? So, what is out of bounds?
[60:13] So, what is out of bounds? So, what is out of bounds?
[60:17] So, what is out of bounds? So, what is out of bounds?
[60:21] So, what is out of bounds? So, what is out of bounds?
[60:25] So, what is out of bounds? So, what is out of bounds?
[60:29] So, what is out of bounds? So, what is out of bounds?
[60:33] So, what is out of bounds? So, what is out of bounds?
[60:37] So, what is out of bounds? So, what is out of bounds?
[60:41] So, what is out of bounds? So, what is out of bounds?
[60:45] So, what is out of bounds? So, what is out of bounds?
[60:49] So, what is out of bounds? So, what is out of bounds?
[60:53] So, what is out of bounds? So, what is out of bounds?
[60:57] So, what is out of bounds? So, what is out of bounds?
[61:01] So, what is out of bounds? So, what is out of bounds?
[61:05] So, what is out of bounds? So, what is out of bounds?
[61:09] So, what is out of bounds? So, what is out of bounds?
[61:13] So, what is out of bounds? So, what is out of bounds?
[61:17] So, what is out of bounds? So, what is out of bounds?
[61:21] So, what is out of bounds? So, what is out of bounds?
[61:25] So, what is out of bounds? So, what is out of bounds?
[61:29] So, what is out of bounds? So, what is out of bounds?
[61:33] So, what is out of bounds? So, what is out of bounds?
[61:37] So, what is out of bounds? So, what is out of bounds?
[61:41] So, what is out of bounds? So, what is out of bounds?
[61:45] So, what is out of bounds? So, what is out of bounds?
[61:49] So, what is out of bounds? So, what is out of bounds?
[61:53] So, what is out of bounds? So, what is out of bounds?
[61:57] So, what is out of bounds? So, what is out of bounds?
[62:01] So, what is out of bounds? So, what is out of bounds?
[62:05] So, what is out of bounds? So, what is out of bounds?
[62:09] So, what is out of bounds? So, what is out of bounds?
[62:13] So, what is out of bounds? So, what is out of bounds?
[62:17] So, what is out of bounds? So, what is out of bounds?
[62:21] So, what is out of bounds? So, what is out of bounds?
[62:25] So, what is out of bounds? So, what is out of bounds?
[62:29] So, what is out of bounds? So, what is out of bounds?
[62:33] So, what is out of bounds? So, what is out of bounds?
[62:37] So, what is out of bounds? 
