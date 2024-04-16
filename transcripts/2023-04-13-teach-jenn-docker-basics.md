---
showLink: "https://www.youtube.com/watch?v=FjUCeyIdTn0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-docker-basics"
title: "Teach Jenn Docker Basics"
publishDate: "2023-04-13"
coverImage: "https://i.ytimg.com/vi_webp/FjUCeyIdTn0/maxresdefault.webp"
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

[00:00] >> Well, welcome. Wow, Anthony, you're like our very first episode.
[00:07] I totally butchered saying hello as well. Can I blame you for this?
[00:12] >> Must have jinxed you. I guess I'm cursed. >> Well.
[00:15] >> I can introduce you. >> Yes.
[00:18] >> Welcome to Teach Gen Tech with Jen Janot and Anthony Campolo. Jen's a Developer Advocate at Avon where she teaches
[00:25] people about databases and APIs and even Kafka. >> My name is Anthony Campolo.
[00:30] I'm a Developer Advocate at Egeo where we deploy sites that are fast.
[00:35] >> I am keeping that clip forever. That was marvelous. Thank you, Anthony.
[00:45] >> I'm tired of Scott too much. He's rubbing off on me. >> Oh my gosh. He is so good at doing like the-
[00:52] >> Bringing the energy. >> Yeah.
[00:54] >> Yeah. >> The radio voice.
[00:55] >> Yeah. >> Always bringing it up during the streams or during the Twitter spaces.
[01:02] >> The spaces, yeah. >> Damn. You're good.
[01:04] >> Yeah. It's his primary job. We call them the station breaks.
[01:08] You have a specific term for when you stop the conversation, you let everyone know you got to follow the people who are on
[01:14] the space and that we're talking about this and that if you're a beginner, or you're just in the crowd and you want to chat, come up and chat.
[01:19] You always hit those three points every single time in a station break. >> I like it. Station breaks.
[01:25] I dig it. >> Yeah, super smart.
[01:28] >> Okay, y'all. We're doing things today. We are learning about Docker,
[01:35] which is funny and I keep doing this of doing things very backwards. I will learn about something,
[01:46] try to do something really technical, like Anthony's of my first stream was making a React web app.
[01:54] >> On Vercel. >> On Vercel, where I barely had any idea what JavaScript was.
[02:02] >> Yeah, but you had a site at the end of that stream. That's the most important part.
[02:07] >> I did. Today, we are going over the basics of Docker. I set it up on my computer about two weeks ago
[02:16] as I've been learning about Postgres, and then we also for the rest of this week,
[02:24] I have Ben coming on tomorrow, Ben Gamble, and we're going to be talking about the basics of data.
[02:30] I like that this week we're taking a step back on two of the streams, and then Friday is TypeScript day. I like TypeScript day.
[02:38] >> You have TypeScript day every week. >> Every other week.
[02:41] >> Every other week, yeah. >> Yeah, TypeScript days are fun.
[02:45] You know more TypeScript than me right now then? >> No.
[02:50] >> No, I'm serious. I've gotten away from not writing TypeScript my entire career.
[02:55] It's been a rare privilege of being a dev rel who creates his own templates and projects is that I just
[02:59] built everything in JS and no one can tell me otherwise. >> Okay. I'm typing this out to you for the chat.
[03:09] >> People right now are hearing me and they're like, "I hate this guy.
[03:11] How dare he try JavaScript and force others to deal with his JavaScript?" I'm like, "How dare you force people to deal with your TypeScript?"
[03:18] That's what I would say to that. >> I really like,
[03:20] I think, surprisingly, and Josh knew this, Josh Goldberg, for those who may not know,
[03:28] is the author of this book. >> He's been on my podcast, technically.
[03:32] The episode is not aired yet, which I feel terrible about since it's been a really long time,
[03:35] but it will air soon in the next month or two. >> Everyone, please excuse my sniffles because they're not going away.
[03:44] It is very springy here. Yeah, this week, we actually get to start going over part 2, Functions.
[03:54] >> There you go. Functions is the most important part because that's going to map a lot closely to what you do with a React app,
[04:00] where you have a bunch of functions that you're tossing around. You want to make sure they're type-safe.
[04:04] >> It's very, very cool doing this because, Josh, the questions I ask,
[04:10] Josh knows that it's from when I don't know JavaScript that well, or I know it in JavaScript,
[04:18] yet I don't know the name of it. That's been a huge piece of going through this with him has been,
[04:25] "Oh, I do know how to do this." It's just, I didn't know.
[04:30] >> It's slightly more complicated and with a couple extra steps. >> No. A lot of times, it's been something I've done.
[04:35] I just had no idea that's what the name of it was. >> Interesting. Do you have an example of that?
[04:43] What a thing was that you didn't know the name of? >> A module.
[04:47] >> A module. Yeah. Okay, cool. Yeah, that's an important one.
[04:52] >> If I understand a module, it's basically where it's like a little subsection
[04:58] that it uses your information and that you get types from. It can be a list.
[05:06] I was using it in one of my Astro Layouts websites that already had TypeScript set up,
[05:15] and it had a list of all of its types, and each section of them are a module.
[05:20] >> A module is more general than types at all. A module is just a chunk of
[05:25] JavaScript code or TypeScript code in one place, you want to import into another place.
[05:30] You could have a JavaScript module with no types whatsoever being imported from one file into another file.
[05:37] That's the general definition of module, but in terms of what you're talking about,
[05:42] importing types one place to another, that's like a use case of a module.
[05:46] I don't know if that makes any sense. >> It does. That is one of the parts that I found so
[05:53] interesting of my podcast that I was interviewed on. They were like, "Hey,
[06:00] so what type of tech do you do?" >> You do databases and event queues,
[06:07] and JavaScript is what you do now. That's your answer. Embrace it.
[06:12] >> I know some TypeScript and some Python. >> You should tell people that you're the inventor of Postgres,
[06:21] is what you should tell people when they ask you. >> No.
[06:26] >> Then they'll be so confused, they won't even know what to say like,
[06:29] "I'm kidding, but I work for a database company." >> Yeah, which is yes.
[06:34] It's a lot of like, oh my gosh, I can't believe it's been almost a year.
[06:40] We are two months away from it being a year since Teach Gen Tech is launched, which is bananas.
[06:47] >> The date, Teach Gen Tech. >> It started July 1st.
[06:52] >> You were on July 5th? >> That was nine months ago.
[06:59] >> Was it the 5th? >> July 5th, 2022.
[07:03] >> Oh, sure. >> Good times.
[07:05] >> It's only because I remember you were my second episode, and it was on Friday the 1st,
[07:17] and then you are on Tuesday. That's the only reason I remember that.
[07:22] >> That's funny. >> It's crazy because that goes into
[07:25] the language that I'm learning to say because the last year I've been like,
[07:29] "Oh, I'm learning X, Y, Z." Well, at one point you
[07:33] learn and then you can actually talk about it. So you actually know it,
[07:37] you're not just learning it. I didn't know how to talk about that, but that is okay.
[07:42] Well, we can move in to the Dockerness. >> Let me drop this in a couple of discords real quick,
[07:52] in case anyone wants to come hang out. I feel lonely, there's no one in the chat right now.
[07:57] >> Well, I think it's because everyone else decided to stream at the same time.
[08:03] BDuggy is streaming, Rizal is streaming, Ramon is streaming, Josh is streaming.
[08:09] >> How dare BDuggy stream right now. >> We are all streaming at the same time,
[08:15] and this is one of the best and worst parts about being friends with streamers.
[08:22] Is nine times out of 10, you have something to go watch.
[08:25] >> I'm especially bummed because I would be watching BDuggy stream right now.
[08:28] He hasn't streamed and he's been very spry, can last like three months.
[08:31] His was the first stream I ever watched. I started watching BDuggy stream two years ago.
[08:35] It was the first Discord I was ever into. >> That's crazy. I love how with Discord,
[08:41] you just end up, what are the things you did? >> I was trying not to overwhelm me with Discord.
[08:48] >> I heard if you do one Discord every couple of weeks. >> Yeah. I'm not very active in any of them.
[08:55] >> But they're there now, and you have resources if you need them.
[08:59] That's the important part. >> But I'm only active in one Discord,
[09:03] and it's the Open Source Raid Guild. >> Jacob's Discord.
[09:09] I'm in that one. I'm not active at all in it though. >> Yeah, that is my go-to.
[09:14] I always ask questions there. >> Yeah. I have mine ranked honestly,
[09:20] which is because it's top to bottom. You rank it whether you are realizing it or not.
[09:25] My ranking is, I go RedwoodJS, so it's going to be on top even though
[09:29] I really don't hang out in it very much. Then LunchDev, then Theo's Discord,
[09:35] then Swix's Discord, then OpenSauced, Brian's Discord,
[09:40] then ShowMyChat, which is not super active, but has the best collection of streamers,
[09:44] tech streamers that exist. >> It does.
[09:46] >> Yeah, that one's going to blow up one day. Then NickTaylor's Discord,
[09:51] irondeveloper.com. >> Wait, NickTaylor has a Discord?
[09:53] >> He does. I'll send you an invite. Then Learn, Build, Teach,
[09:57] which is JamesQQuick's Discord, and then UnicornUtterances,
[10:01] there's a new one I just joined, we'll see, on Corbin's Discord, Corbin Crutchley.
[10:08] >> Corbin has a Discord too? >> Then Trash's Discord,
[10:11] and then FriendHorse. I feel bad because FriendHorse used to be up seven places,
[10:15] but the conversations are not fully what I'm into these days, so I don't spend much time in Friend's Discord anymore.
[10:22] But I love Alex Trost, he's the man. >> Corbin and I just became friends a few weeks ago when we
[10:30] had a Friday night stream that had 12 people on stream at once. >> Yeah. I hopped in for five minutes on that one.
[10:39] It looks super fun. >> I was coding and everybody else was bullshitting,
[10:44] and then I would just interrupt to ask questions. Oh my gosh, BigDouggy, you're here.
[10:49] >> Yeah, he probably just popped in to leave a message before he starts his stream.
[10:53] >> Yeah. >> Yeah, I'm trying to get a secret sauce episode going with Brian.
[11:01] Have you watched any of his secret sauce interviews? >> Yes. They're so good.
[11:07] >> Yeah. Have you watched one with Ryan Carniato? >> No.
[11:10] >> Watch that one. That's probably my favorite one he's done. >> Can you link that one for everybody?
[11:15] >> Yes. >> If you have that up. I would say if you,
[11:19] I don't know if anybody else has this, but there's people that make an impact on
[11:24] your life and your career that you don't talk to often. That would be BigDouggy.
[11:29] >> Because he has an impact on everyone's career and not everyone has, he doesn't have enough bandwidth to talk to everyone all the time.
[11:37] >> It's weird because if I were to be like, hi, I wouldn't know what to say to them.
[11:45] >> Well, just because with people like that, if you have things to do,
[11:48] I only message Brian if there's like, I want him on my podcast,
[11:52] I think I could be on his podcast. There's a collaboration we can do.
[11:55] I would just message him in the random day like, "Hey, how's it going, buddy?"
[11:59] >> That's true. >> He's a busy dude. He doesn't have time for those messages.
[12:03] >> Yeah. >> But as long as you can find,
[12:06] you've had him on Teach Jet Tech. That's a good example of a time you get to collab,
[12:11] and you would be a good guest for The Secret Sauce. Because he would love to talk to you about
[12:15] your journey through streaming and getting into this stuff. You'd be a great guest for that.
[12:19] If you're ever in San Francisco, you hit him up and be like, "Hey,
[12:21] can I get on The Secret Sauce?" He'd be like, "Sure."
[12:24] >> That actually reminds me, when he was supposed to be on my stream,
[12:29] is when I dumped water on my laptop. >> Yeah, I remember that.
[12:35] >> It was heartbreaking. >> You eventually got him on.
[12:39] I'll drop a link for that one too. >> Yes. He did come on the show.
[12:45] He was so kind. It's one of those people that whenever I get really nervous,
[12:51] because I've had to postpone them or life happens, I get more nervous about the stream.
[12:57] Then I'm like, "Oh yeah, it's not that bad. Okay, cool." >> Are there only six videos showing up on the Peach Gen Tech YouTube page?
[13:06] >> Because they're all live streams. I'm slowly going to be downloading them from live streams.
[13:11] >> This is confusing. I really hate that YouTube does this. >> That's a big reason I started doing it where this is only going to Twitch,
[13:20] and then I download it and upload it to YouTube. It actually does better that way than it does with the live streams to YouTube.
[13:27] >> I say that again, you upload it to where and to where? >> I stream with Twitch,
[13:32] so I can download it from Twitch, and then I manually upload it to YouTube.
[13:38] >> We're not streaming on YouTube right now? >> Right.
[13:41] >> Okay. I do that the same way with mine. Then sometimes I spend a month putting off uploading the YouTube video like I just did.
[13:50] Here it is. You don't have Brian Douglas's name or open sauce in the title of this video.
[13:57] It took me forever to find it. >> This is why I need to go back through and do them.
[14:03] Also one of the reasons why I'm like if I download them as well from a live and move them to that,
[14:09] which I can change the dates they were recorded. >> I have a lot of ideas of what you should do with
[14:15] your archive to make it a little simpler to go through and sort catalog and things like that. >> Yes, please. Send over my way.
[14:24] I also have my websites to do. >> That's the thing though. It will combine with the websites.
[14:29] The website should be the source of truth. The website should have a page for every single episode,
[14:34] and every single episode should have a page with links to everything that happened, including the video, and the repo,
[14:39] and description, and information about the guests, and timestamps. Those are the hour you click out.
[14:45] Yeah, that's the thing. >> There's only like 77 streams and six videos.
[14:53] There's only like 80. I think I have roughly the same for my podcast.
[15:00] You know, that is all on the to-do list. Yay. But yes, everybody is streaming right now,
[15:09] which is great, and we will send this after it's uploaded to YouTube, so they can watch the recap of how to set up Docker, which.
[15:20] >> We should probably start doing. >> Yeah, we should probably start doing that.
[15:24] Oh, yeah. Yeah, we should. >> So let's talk about Docker.
[15:28] I can tell you my history with Docker because it's fun. Docker is an extremely confusing,
[15:34] but useful, and now ubiquitous tool in programming. It took me an extremely long time to figure out how to use it,
[15:41] which is why I wanted to hop on here, just like walk you through an example that's not incredibly complicated.
[15:48] It will take you nine hours to figure out, because it took me multiple hours to write
[15:52] this five-minute tutorial that we're going to go through, because the resources for Docker are so awful,
[15:58] or they're just out of date. But all we're going to do is we're going to create a node express server
[16:03] that's going to return a web page with a single H1 on it. That's all it's going to do.
[16:08] Then we're going to containerize that server, and then run that container on your computer.
[16:14] We're not even going to deploy it anywhere. The main thing that I think this example shows
[16:19] is that you can use Docker in lots of different ways, because you're using Docker right now for a database.
[16:24] This is not going to be necessarily what you're going to do with the Postgres stuff,
[16:29] but it's going to give you a better conceptual example of what people mean when they talk about Docker,
[16:33] and they talk about running their application in Docker, or deploying their website with Docker.
[16:39] Because when you just run a Postgres database, that's really just for testing purposes.
[16:44] Some people will actually deploy their Postgres databases in a Docker container,
[16:48] and those people are setting themselves up for a bad time in the future,
[16:51] because you should not put your database in an ephemeral server that is running in a container
[16:56] that can be wiped out at any time. Some people do it anyway, though.
[16:59] I do it with a bunch of my railway applications. That's because they're kind of demo apps.
[17:03] But for the most part, if you're running a database, you usually want to actually run that database
[17:07] on a database server, which is not using Docker. What Docker is doing is it's taking that database
[17:12] and it's creating kind of like a virtual version, self-contained version of it
[17:17] that can just run on your computer in a way that makes it simpler to access and to work with
[17:22] than if you're actually running Postgres on your computer. 'Cause you've gone through this whole struggle
[17:25] of trying to download and run Postgres on your local computer,
[17:30] which is something I actually think developers should not do. I think that that is not something-
[17:35] - Oh, yeah. It was just the experience of seeing if I could do it,
[17:38] and that was- - Yeah, you should do it to learn how to do it,
[17:41] so you can know why you should never do it again, is what that exercise is.
[17:45] So what more people do is they'll run it in a Docker container,
[17:49] which is what you're kind of learning to do, or they'll go one step even further.
[17:53] What I do is I just deploy a Postgres database on Railway, which is running in a Docker container on Railway,
[17:59] but then it's not running on my machine. It's already over a network,
[18:03] because then if you're gonna have weird network errors, you can debug that
[18:07] by working with a live database in production. It's just a live database in production
[18:11] that you can blow away at any point in time. So that's mostly what I recommend,
[18:16] but as I was saying, what we're gonna do today has nothing to do with any of that.
[18:18] We're just gonna run a Node server just to kind of figure out what's it like to use Docker
[18:23] to build and deploy a very, very small, tiny application. - And I realized that I probably should have prepped you
[18:31] for these questions. - You shouldn't have.
[18:35] I'll get better answers if you don't. - Okay, well, then I will ask them when we get to it.
[18:40] So let me go ahead. I've already, so once we get done today, y'all,
[18:45] I will have a readme to share. This is something I've been working on doing,
[18:49] and Anthony is a big reason why. And, oh, I do want to share this.
[18:56] It's not an official readme. It's very similar, but I had to start doing this
[19:02] so that way I could get help on my Postgres project. So this actually, me, me, me,
[19:12] which this will be very easy to put into a readme. So share screen, entire screen, yay.
[19:24] All right, so this is basically a giant readme because it's--
[19:34] - But you wrote it in a Google Doc because you hate yourself? - No, because I need other people's feedback
[19:40] and to be able to change it very easily. - If only we could collaborate on a readme
[19:44] in a GitHub repo. - Sir, sir.
[19:49] - I just hate Google Docs. I understand why lots of people use it.
[19:53] - But it's a lot easier to collaborate just this. - That is, you can leave comments
[19:57] and you don't gotta open a PR, I understand. - So it was really helpful.
[20:03] And this is why I was so excited because, yes, you make fun of me for having to use my tablet
[20:08] to write it down and then upload it. - I don't make fun of you for that.
[20:11] I'm telling you, you're adding an extra step to your workflow and that's like, that's okay.
[20:15] But if you spend more time practicing, typing out your thoughts in a readme,
[20:19] it may be harder now, but you'll get better at it as you do it more.
[20:22] That's all I'm saying. Like you can do what you wanna do
[20:24] in whatever you find easier right now, but you can develop skills by practicing them.
[20:29] That's my point. - I agree with that.
[20:32] And also people have different learning techniques and sometimes they do take extra steps, which is annoying.
[20:41] But I was so excited- - I have an education degree, I'm a teacher.
[20:44] Like I understand that, but I would also still recommend you try multimodal stuff
[20:49] because even people who excel at a certain kind of learning should do other types of learning that are harder for them
[20:55] because they will learn in a different way, which in the grand scheme will be useful.
[20:59] I know it feels uncomfortable 'cause people don't wanna do that
[21:03] 'cause learning is actually hard. - Learning is hard, but it is fun.
[21:08] And thank you for the follow. Yes, yes, we have a lot to cover today.
[21:14] - Hey, CM Griffin. I'm CM Griffin.
[21:16] I mean, I know he's a streamer. Can't say I know him super well,
[21:19] but appreciate you being here. Thank you.
[21:21] - Yay. It's definitely something that I feel like we are,
[21:26] there's so much that goes into this. And y'all, if anybody's wondering
[21:30] why I may come across as mean or give Anthony funny faces.
[21:36] - You come across as confident in your own decisions. And that's a good thing.
[21:43] And you shouldn't apologize for it. - That's good.
[21:45] Well, I was just gonna tell them like you're my internet big brother.
[21:48] That's all I was gonna say. 'Cause that's like-
[21:51] - But you shouldn't apologize for pushing back on my own advice.
[21:54] 'Cause that's fine. You should have pushed back,
[21:56] but you should also take it into account. - Thank you.
[21:58] Thank you. I do appreciate that.
[22:00] Okay. So we have the GIFs up for today of Tchen Docker.
[22:06] And then we have Docker up, which I did already download.
[22:11] So we will go through that. And CM Griffin, I need to check out your content now.
[22:19] Let me go follow back. So that way I can check out mean streamers.
[22:25] I like mean streamers. That would be fun.
[22:27] - The meaner, the better. - I mean, I feel like, I don't know.
[22:33] I don't think Theo's mean, but I do say that's why he makes funny content.
[22:38] But I can't say he's mean. I don't know if that's the right word.
[22:45] - He's mean to some people sometimes for reasons that he thinks justifies him being mean.
[22:50] And I think more often than not, he's correct. But right now that he is a little mean,
[22:55] but that's because he has a confrontational- He has a confrontational-
[22:59] - Oh, that's a good way of saying it. - Yeah, I would say he's mean,
[23:02] I would say he's confrontational, which some people interpret as mean.
[23:06] So it kind of depends on whether people are used to dealing with confrontational people.
[23:11] I can deal with confrontational people and I choose not to be confrontational most of the time
[23:15] because there's a certain percentage of people who get very, very turned off by conflict.
[23:20] And that's why there's like a subset of people who extremely dislike Theo.
[23:24] But I think it's fine. It's just, you're walking a fine line when you do it.
[23:29] - That is true, that is true. Okay, so we have a to-do list, which I am excited about.
[23:36] And for those who also want to know something kind of funny is while I was applying for jobs
[23:45] and having to like get help and approval from whatever project I was working on,
[23:51] half the time it was Anthony cleaning up my readmes and restructuring them.
[23:56] So they look pretty like this. - Just polishing them, you know?
[23:59] - Polishing them, polishing them. All the content was there.
[24:03] Just making it a bit more readable. And I dig it.
[24:06] Ooh, CM Griffin, same. I am nice mostly, but I don't mind an argument.
[24:15] It's a good, it's good practice. - Right, because most people are very set in their opinions
[24:21] and it's good to have them challenged and force you to actually defend them.
[24:25] 'Cause then you may find that your opinion is not as firm as you might have thought it was.
[24:31] - Touche. Okay, before we get too far,
[24:35] because one thing I have learned since starting Teach Gen Tech
[24:40] is when there's something that I've given of a to-do list or something like that,
[24:45] I start to just kind of glance over the entire thing so I might know where I'm going.
[24:51] - You should, that's why there's an outline at the top. - Yeah, yeah.
[24:54] Now, I'm very excited because it might be in your article. Let's open your article in a new tab.
[25:02] Okay, I'm not seeing it here either. - What were you hoping would be in it?
[25:10] - List of images, run an image that is close. Create a, build a container.
[25:16] - What are you looking for? - What is a container?
[25:19] Like a definition, what is a container? What is an image, and what is a volume?
[25:24] - Volume will not be in that blog post. It's not doing anything with volumes,
[25:28] but the other ones are defined within them once they are first introduced.
[25:32] So for container, create and build a container is where the title would probably be.
[25:37] Let's see. Yeah, that's a good question.
[25:43] Actually, I don't know if I actually give specific definitions of those two terms
[25:49] within this blog post, 'cause the point of this blog post
[25:51] is kind of to explain each of the steps and what they actually are.
[25:55] And by the end, you'll understand what an image and a container is,
[25:58] 'cause I found that giving the baseline definitions don't actually make any sense,
[26:02] but the difference between an image and a container will make sense once you build an image
[26:06] and then run and you build it. You create an image, you build a container
[26:11] and you run a container. So where an image turns into a container
[26:16] will make more sense once you've done it. So that's why I could give you the textbook definition
[26:21] of both those terms right now. They wouldn't mean anything to you.
[26:24] And then we'll go through the exercise and then we can kind of go back to them.
[26:28] So let's just do that. Define, actually, let's,
[26:31] chat GPT, this is a good use case for chat GPT. Let's ask chat GPT to define a Docker,
[26:37] what's the difference between a Docker image and a Docker container.
[26:40] - You are such a chat GPT advocate. - 'Cause this is gonna give a better answer
[26:46] than any explanation written in the entirety of the Docker docs.
[26:49] I know because I've read the Docker docs and they're trash. So people should use chat GPT for this.
[26:55] - I will say the Docker docs were easier than the Postgres docs.
[27:01] - Postgres is the only thing that is worse than the Docker docs.
[27:05] Postgres, just installing Postgres is so fricking hard. Not even the docs, like installing should be
[27:10] before you even need to read the docs. You can't even figure that part out.
[27:14] It's incredible. It's the most important piece of software like ever invented
[27:18] and it has the worst website ever. - It was tough, it was tough, but that's okay.
[27:24] Well, we moved through it and we'll make articles and blogs about it.
[27:28] It'll be good, it'll be good. All right.
[27:31] - All right, here we go. So I'm dropping these in the chat.
[27:33] The Docker image is a lightweight standalone and executable software package
[27:37] that includes everything needed to run a piece of software, including the code, runtime, system tools,
[27:42] libraries, and settings. So that's a lot of words.
[27:46] It's actually not that complicated of an explanation. It's just a big, such a big explanation.
[27:52] It almost becomes meaningless. It's technically correct though.
[27:55] - I feel like where I was getting confused when I set it up was, I will ask you after a container.
[28:05] There you go. - So a container is a running instance of a Docker image.
[28:10] So that's why I said, we'll create an image and then we'll build and run a container.
[28:15] So that's what it means right here. A running instance of a Docker image.
[28:18] When you start a Docker image, it creates a container. See, that's great.
[28:22] That's such an awesome way of explaining. I've never heard that explanation before.
[28:26] (laughing) - So, and that makes sense.
[28:29] Like the container itself makes sense. And running a container makes sense.
[28:35] What, going back to the image one of where I think is hard for myself, maybe others was, okay,
[28:45] so when we create a project and it goes on GitHub, it has its own main folder that you go into
[28:56] to be able to make all these changes and things. And so in my mind, that's what I was comparing an image to,
[29:05] but it's not the same folder structure. - Yeah, it's close in the sense
[29:09] that the image you can think of as a bunch of code that's going to exist in a GitHub repo.
[29:14] That's what we're gonna be creating in this example. But the important part is what is like the Docker file?
[29:19] The Docker file is what explains how to build the image. And that's the vast majority of what this tutorial about
[29:25] is about what are the steps of the image itself? And the steps are going to be,
[29:30] it's gonna take your node project and do kind of what you do on your computer,
[29:35] where you like have a package.json, you install dependencies.
[29:38] If you have that dependencies, you can run your server and you run your server with a certain command.
[29:43] So those are the steps that are going to be in our Docker image.
[29:46] - Makes enough sense. - Yeah, and this is why I say a lot of these terms
[29:52] don't make sense until you've already done it. So that's why I'm saying we shouldn't get too hung up
[29:56] on definitions right now. We should do the thing
[29:59] and then kind of talk about what happened. Unless you have other questions,
[30:05] which are totally fine if you have more questions, I could talk about this.
[30:08] - No, I can't type at the same time. I can't talk and type.
[30:13] And I just wanted to post every year blog. - Cool, cool.
[30:17] - Because I will-- - This is a good blog post.
[30:19] This is one that was one of the first that took me a long time to write.
[30:23] And I had to research something I knew absolutely nothing about.
[30:26] And I was able to create a resource for myself that I have continued to use for like many years,
[30:30] like this tree being a good example. And I was learning it because I wanted to figure out
[30:35] how to containerize Redwood because Redwood was talking to all these companies
[30:40] that were running containers. We were trying to figure out how to get Redwood
[30:42] to run on a Docker container. And I was like, I don't even know how to frickin'
[30:45] run a basic node server in a Docker container. I'm not gonna be able to figure out
[30:48] how to do it with Redwood. So as I was seeing that conversation play out,
[30:51] I created this as a resource for myself and exercise for myself to learn
[30:56] what a frickin' Docker container is and how to work with it.
[30:59] And I feel like that's pretty battle-tested. I just ran through it today.
[31:02] Even though it's two years old, it still works as expected. So we'll see how it goes with you.
[31:08] - Let's find out. Okay, so we, yo, how's it going?
[31:16] - It's got style, Aggie. - I'm not gonna lie, I don't think I ever,
[31:22] me and last names, your last name is super easy and just you're AJC web dev.
[31:30] To this day, you are AJC web dev. (laughing)
[31:33] - That's good, yeah. I don't know if my last name is necessarily that simple.
[31:36] Some people find other ways to pronounce it. And based on just looking at,
[31:39] it can even be a couple of things. Yeah, it's whether it's camp or comp
[31:43] is what people get confused about. Some people say compolo.
[31:46] - Yes, that is how he taught me. - Camping and polo, that's right.
[31:51] It's like camping and water polo, campolo. - Yeah, well, we got there.
[31:55] We got there. - And we got Elyon, what's up?
[32:00] When are you coming on the show? Keep talking about it, Elyon.
[32:03] Elyon, Elyon? - Yeah, I'm not sure, so.
[32:07] But I know that they're on the Astro team. - When you come on the show,
[32:12] you can correct us on how to say your name properly, which I should probably follow up about.
[32:18] But hey, we're not working on Astro today, for one. Okay, so.
[32:26] - All right, so the first steps in the create project section
[32:29] are just going to create a folder, initialize the package.json,
[32:34] and then create three files, a JavaScript file, a Docker file, and a Docker ignore,
[32:39] the Docker ignore being much like a Git ignore. - Well, because I have to do this in terminal
[32:49] because since I don't have a container yet, I can't do it on Docker, correct?
[32:53] - Correct, we're eventually going to run some commands that are going to do stuff
[32:57] that will affect your Docker desktop thing, but that's not until later in the exercise.
[33:02] We're gonna start by just creating a regular JavaScript project.
[33:05] - I'm gonna, I was so against this when I first started, and I'm like, I'm not even going to try
[33:14] to retype all of these. It's just gonna be--
[33:17] - Yeah, you should copy paste each command and do them individually.
[33:20] That's very important. Oh man, lunch devs, Michael Chan's even live right now.
[33:25] - Damn. - That's funny.
[33:28] I'm gonna go water. I'll be back in just like 15 seconds.
[33:32] - I'm counting. Yes, I love how like everyone is streaming today.
[33:40] Everyone, all at once. How many streams are y'all watching at the same time?
[33:46] 'Cause I know that you wanna like check in on all of us and make sure we're doing good and support us all.
[33:52] So how many are you watching at once? (silence)
[33:57] Okay, I'm back. (humming)
[34:04] - Yay. Okay.
[34:13] - Pop that, pop that baby open and then drop that JavaScript code in there.
[34:18] So if you-- - What code?
[34:21] - So you used Express with Ramon on your very first episode. So that's what this is gonna be.
[34:26] What we got to say. - Okay, cool.
[34:29] That, I finally got CodeDot to work. - Hey, what's up?
[34:35] - Okay. - You're a senior developer.
[34:37] - This is why. And it's because when it installed,
[34:43] it installed in download still. For some reason, it did not auto install to applications.
[34:49] I had to manually move it to applications where most things when they download
[34:53] and you know, you drag and drop to install it. They auto move to applications.
[34:58] It did not. - They don't auto move it.
[35:00] They usually pop you up with a little window where they have your applications folder right next to it
[35:04] and say drag it from here to there. So they basically stick that step right in front of you
[35:08] so you don't forget it. - Yes, except--
[35:12] - Yeah, you don't want anything that was in your downloads. So it was in your downloads folder.
[35:16] Yeah, so check your downloads folder every day and make sure there's nothing in there
[35:21] from whatever you were doing. This is gonna be a source of confusion
[35:24] for the rest of your life. - Yeah, I am much better about checking that now.
[35:31] And-- - If you want a fun story about a thing being in a folder
[35:35] that you didn't know, so your whole life was destroyed. I once had a node modules folder in my root directory
[35:43] that I didn't know about. So that anytime I would download a project,
[35:46] enter it and then run a dev command, nothing would happen. So I was unable to run a dev server on my computer
[35:54] like the first two months of my bootcamp 'cause no one could figure out the problem.
[35:57] So I wrote everything at a code sandbox and then I would fork the code sandbox into a Git repo
[36:04] and then I would deploy the Git repo on Netlify. So I deployed my project every single day
[36:10] to show it to my teacher. So I actually learned how to deploy projects
[36:15] like three months before everyone else because I couldn't run it on my computer.
[36:20] - Isn't that incredible? (laughs)
[36:23] - Is that why you like wanted me to use Vercel as like my first one, so I could show that--
[36:30] - Exactly. - Thing that I built? - Exactly.
[36:33] (laughs) - It didn't make sense until like a couple months,
[36:37] probably like two months ago, I had a interview with a company and they were like,
[36:43] "Hey, talk about why you love Astro." By the way, this interview was not with Astro.
[36:50] It was just, they were like, "Hey." - I had an interview with Astro once.
[36:53] - And it was, I compared why people deploy on Netlify or Vercel, just the experience itself.
[37:01] And I was like, I really like Vercel, like just the way it works.
[37:08] And thank you, Scott, for the follow. Ooh, ooh, that's actually,
[37:14] that is what you should come on the show. - No, I feel like Dan should complain.
[37:18] - Complain? - Complain, get it out of there, explain.
[37:22] Like that. Okay, anyway, I got it, it's showing.
[37:27] Let me go back now. Why did you--
[37:30] - No, we gotta change that to say, "Teach Jen Docker." - Yeah, okay.
[37:35] - That's good, you always gotta change something or else it's not a tutorial.
[37:44] - And I actually know what we're doing now because-- - You got a port, you got a host,
[37:50] you got a thing and the stuff. - And this is like new.
[37:56] This is not something that I knew how to do back in the day. I'm so proud.
[38:04] - Yeah, cool. So the next part is gonna be the actual Docker file.
[38:10] Yeah, look at that. - That's true, you need to turn and restart your server
[38:15] 'cause I don't even include NodeMod in this example. Although apparently Node 18 has a way to do that.
[38:21] - Well, I already restarted the server. - Right, which you normally have to
[38:26] because Node itself does not watch for changes. But I think Node 18 might have a way to do that
[38:32] if you pass it the right flag. I don't know how to do it right now,
[38:35] but I'll look that up later. Anyway, let's go to the next steps.
[38:38] This is where the Docker stuff actually starts. - Oh, I should probably install the extension.
[38:43] - Install, install. Oh, that was exciting.
[38:50] Thanks for the install. Okay, so then we're going to copy paste.
[38:56] - Yeah, so let's copy this, the whole thing, and then I'll talk about kind of line by line.
[39:00] There you go. Yeah, it's just a watch flag, if that makes sense.
[39:04] - I can say, y'all, in case anybody was curious, if you want to see me struggle with Node versions,
[39:12] especially because we were talking about VDougie earlier, that episode, I struggled with Node versions.
[39:20] It was interesting, to say the least. - And this is why I use Volta,
[39:25] 'cause Volta makes it really easy to manage your Node versions.
[39:28] You should open your window up so we can see the whole thing.
[39:32] - All the things, okay. - At least top-wise.
[39:39] Yeah, there we go. Okay, so let me just kind of walk through this real quick,
[39:43] and then you can ask me questions about individual things, if any of it confuses you.
[39:47] First step defines, we're using Node, where it's Node 16, and we're running it in Alpine.
[39:55] So Alpine is a Linux operating system. So if we left off Alpine,
[40:02] then you would not download the same bundle of things, because this is running Linux, and it's running Node.
[40:12] So you can choose to run different kinds of Linux, 'cause different kinds of Linux have different dependencies.
[40:17] So this ensures that your Docker file ends up small and lightweight.
[40:21] It's gonna be like 100 megabytes, instead of like two gigabytes.
[40:25] So that's the only reason why we're using Alpine, specifically.
[40:28] For someone who's new to Docker, this is totally not that important,
[40:31] but just for the record, for people who are watching this
[40:34] and are confused about what this means, there's your explanation of why we're using Alpine.
[40:38] It's just a way to run Node in a very small Linux operating system.
[40:43] - And this also helps, because you don't know if you'll get,
[40:46] we receive questions from, you know, nine months later. Yay. - Yeah, totally.
[40:53] Okay, then workdir. This is like the working directory for your project.
[40:58] So it spins up a Linux server for you with a file system. That file system is /usr/src/app.
[41:07] And the code of our project, which is just a single JavaScript file,
[41:12] is gonna be plopped in that kind of working directory. - Cool.
[41:18] - Then we're copying over the package.json and the package lock.json.
[41:24] That's why there's a star after package before the .json. And that is so when we run this server,
[41:32] it will have the dependencies. So what's happening here is kind of what happens
[41:36] every time you run a JavaScript project on your computer. You create a directory, you have a package.json.
[41:42] That package.json has some dependencies. You install those dependencies,
[41:45] that pulls a bunch of code onto your computer. Then you can actually run the project on your computer
[41:51] 'cause it has all those dependencies. So we need to first copy over the package.json file.
[41:56] We then need to run npm install, this command you've run tons and tons of times.
[42:02] Then after you run the install command, you copy the dependencies into it.
[42:07] So that's why you first copy the package.json. You then run the dependencies.
[42:11] You then do another copy step. Then you expose your node on a certain port.
[42:17] So you expose it on 8080. And then you say, hey, we're gonna run a terminal command.
[42:22] That terminal command is going to contain two blocks, the word node and then index.js,
[42:29] which is what you ran when you first were testing out the thing.
[42:32] So basically this is a way to take the whole process of sticking your current repo and the code in it
[42:39] into some sort of container that will download dependencies and then run the thing.
[42:44] So this is the image. This is the image that we're creating
[42:48] that will be built into a container. - It makes enough sense.
[42:56] It does make enough sense. - That's an explanation
[42:59] that you'll have to go through a couple of times. This is why it took me weeks to write the blog post
[43:05] because I took each of these steps and had to research the word,
[43:09] figure out what the Docker definition was, explain how that definition maps
[43:12] to this project in particular, and then find the words to actually explain it.
[43:15] So I had to actually write this down step-by-step, go through it many times,
[43:20] understand what it was conceptually, and then figure out a way to explain that to other people.
[43:24] And it's not simple, but once you get it, you'll be able to look at something like this
[43:28] and it just instantly makes sense. And it's actually an extremely concise way
[43:32] of putting this into a reproducible thing. - Without you saying what all of these were,
[43:42] I would have gotten that it was node, but I would have had no idea what Alpine was.
[43:49] - Work directory, now that I am seeing it, but I would have been like Workdir,
[43:56] I don't know what Workdir is. - Like Mikdir, Mikdir, Mikdir where you get your burgers.
[44:03] - It might've been hit or miss. The copy package.json, package star json, yes.
[44:10] Run npm i, I think I always do npm install, so I don't know if I would have gotten it.
[44:17] - I is the short form for install, and you could change that to just say install
[44:21] and it would still work. - I'm gonna do that, so that way I remember it.
[44:26] We'll just do it, we'll leave it the way it was and then put it in the notes, and then copy work.
[44:43] I wouldn't necessarily have known what it was copying. - Yeah, that's the step that could be a little confusing
[44:50] because you have to think of it from the perspective of this is a computer you're loading code onto
[44:57] and then you're installing those dependencies just like you would on your own computer,
[45:01] in which case you have that fat node modules folder in your project.
[45:04] - And then expose 8080, if it was a different port number, I don't think I would have gotten this.
[45:11] Because it's 8080, it makes sense to me. - Classic port.
[45:16] - And then command node and index.js. Totally makes sense.
[45:22] Save, yay. All right, let's put you down.
[45:26] - And then the next step is your docker ignore, which is like a get ignore.
[45:30] So this is to basically ensure that stuff doesn't end up in your docker image that doesn't need to be.
[45:37] So it doesn't really need like your get information and the node modules because you're basically
[45:46] it will figure out exactly kind of what dependencies you need.
[45:50] This is the step that John should understand that well, so we don't need to talk about it too much,
[45:54] but it's not gonna mess with anything. So just copy and paste that over.
[45:56] Let's just go build the image. - Yay, okay.
[46:00] So we got it saved. Everything's set up there.
[46:04] Okay, yay. So.
[46:07] - All right, so now we've got these five docker commands. These are the only five commands you're gonna need to know
[46:10] for an extremely long time. So it's gonna do everything you need to do.
[46:14] The first one is gonna build the image. So this is where it's gonna go from an image
[46:18] to a built container that can be run. And this is just something that's gonna happen
[46:24] inside your computer. You'd have docker running right now,
[46:26] but it looks like I see it up top. - It is, it is.
[46:30] - So you're already good. So that needs to happen before you can run this next step.
[46:34] If you don't have docker open, you run this step, it's not gonna work and you'll be very confused
[46:37] until you start running your docker program. That happens to beginners all the time.
[46:42] Very frequently it happened to me like at least five times. - I feel like I'm gonna write that down really quick
[46:47] because, yes, I know you always are like, hey, you probably don't need to write that down.
[46:55] - I never say that. You should write down everything.
[46:58] - Because you were like, hey, they may not like need that in the future if I was writing it for someone else.
[47:05] And that's when I clarified, I'm writing it for me, not necessarily for a specific audience.
[47:10] - Right, yeah. For the most part though, you should just write for yourself
[47:14] and assume that there's others like you as your audience. So whatever it was that I was saying you shouldn't write down
[47:19] was probably fine to write down 'cause it's very hard to include
[47:23] too much information I've found. Almost everyone includes not enough information.
[47:28] - Okay, build and run docker, okay, cool, yay. And so we'll go here and let's see these.
[47:46] - I think this is Alexis in the audience with Peachy Lex. She was asking Scott if it's their first time
[47:56] learning about docker. It's her first time learning about docker.
[47:59] So, and this is, you started learning docker like two weeks ago, you said?
[48:04] - Yeah, like I knew, well, let me link the first time I ever looked into docker.
[48:15] It was, we talked about Kubernetes at the same time and PowerShell.
[48:20] It was intense, but I definitely feel like it was worthwhile because it was a lot of high level content
[48:30] that was made what I'm working on now make more sense. - That's all, yeah, and that's why it makes so much
[48:40] more sense to do those after you've already actually run through a tutorial.
[48:45] It's just to get you something working 'cause every time you talk about something theoretically
[48:49] ahead of time, it won't make sense. And then you'll do the exercise
[48:53] and then it'll kind of make sense. But you could have just done the exercise
[48:55] before even worrying about the terms. - Yeah, but, yeah, yeah.
[49:01] - It depends, certain topics are worse than others. For this one, docker in particular,
[49:05] the terms were so confusing and the definitions were so opaque to me
[49:08] that they were just completely useless until I had actually done something.
[49:13] So you built the thing. And if you actually, let's stop right now for a second.
[49:16] And if you look in your terminal, you can actually see it ran each individual steps.
[49:22] Yes, it's two out of five working directory, three out of five copy, four out of five run.
[49:27] So it takes each of those steps and runs them individually. So if at a point in time you tried to install
[49:34] your dependencies and you had a package.json with a misspelled dependency, it would error.
[49:39] And it would say, "Hey, this broke at this step." If your dependencies were all fine,
[49:43] but then you try to run the server at the end and there's an error in your JavaScript code
[49:47] and it crashes, then it would tell you on this step that there is an error.
[49:50] So right now, 'cause I gave you working code that is gonna work flawlessly, there is none of that.
[49:55] But when you're doing this, you will frequently get errors within individual steps that you need to be like,
[50:01] "Okay, why did it break on this individual step and how do I fix that?"
[50:05] - Fair enough. I feel like just to something that you were just talking
[50:11] about on being new to tech, if you're doing self-learning, for myself,
[50:17] it was really helpful to understand theory of Docker and Kubernetes specifically, just because not understanding
[50:26] the big picture, I struggled with understanding why am I doing what I'm doing?
[50:32] And I see that- - So what was the big picture from your point of view?
[50:37] - A lot of it was what is Docker and Kubernetes and why is one used over the other?
[50:45] - Right, so how would you define that right now? I'll be curious.
[50:49] - Okay, so I know it's not a virtual machine to explain Docker, but it's easier for me
[50:54] to conceptualize it as that. Because it's like, okay, cool.
[50:59] Like you're going to, you're basically building on a little container in your computer,
[51:05] but it's not just on your computer. It's something that if you'd put it
[51:09] onto the Docker website in your- - People couldn't run it yet.
[51:13] - Yes, exactly. Where locally you can't do that.
[51:18] And it's not going to be set up exactly the same way as if you do a GitHub project.
[51:25] - Totally, yeah. And then Kubernetes, how does that relate to Docker?
[51:29] - Kubernetes, this is the way I explain it in my own head. Not necessarily how I think it works for everyone.
[51:37] Kubernetes is like, you could say, almost like Docker on steroids.
[51:41] Because instead of there being like one container, there's a bunch of containers that are connected
[51:46] to each other that can be set up as all duplicates of each other.
[51:52] Like if one fails, something else will pick it up. Or they can all be different containers.
[51:57] And one of the key parts of using containers and like Kubernetes is the fact that
[52:05] you can expand your own resources much easier and do more like pay-per-use
[52:10] rather than having to do like a virtual server that will just have X amount and you're stuck with it.
[52:16] - Totally, yeah, that's a great. That's a, so it's not like you got a good handle
[52:20] on what they are then. 'Cause for me, the big unlock is like Kubernetes
[52:24] is a bunch of Docker containers talking to each other for whatever reason you want,
[52:28] which is understand that it's important 'cause you need to understand you don't,
[52:32] you really should not even think about Kubernetes until you understand how to just work
[52:36] with a single Docker container. Because like what that even is
[52:39] and how it works with other Docker containers in this larger system is going to be extremely confusing
[52:45] until you at least have some handle on what a Docker container is.
[52:48] So that's why once I went down this rabbit hole of creating this article,
[52:51] I realized I could spend years learning about just Docker and never touch Kubernetes at all,
[52:55] which is exactly what has happened. I've never, I have never used Kubernetes.
[52:59] I tried to install a bunch of Kubernetes tools and figure out Kubernetes, hello world.
[53:03] And it was even 10 times harder than the Docker documentation.
[53:06] And I knew I was not going to be actually working with it anytime soon.
[53:09] So I have still never actually used Kubernetes, but you'll, everyone, every dev will use Docker
[53:15] probably a lot. Certain developers will use Kubernetes
[53:19] at their work for certain specific reasons. But a lot of devs will,
[53:23] there's really no reason to use Kubernetes. And if they are trying to use Kubernetes,
[53:27] but they don't need it, then they're going to have an even worse time
[53:30] than someone who does use Kubernetes and actually needs it. - Yeah, yeah.
[53:35] And it's definitely something that, Lex, if you go look at the video that I posted earlier,
[53:43] it is very complex, yet it helped me at least start thinking about things.
[53:49] This, and I'm glad my explanation helped. So that, I'm really happy about that.
[53:53] And I also wrote a blog of some of the things that helped me break it down of like a server,
[54:01] a hard, like a bare metal server to a virtual machine to a, I will show you.
[54:11] I have a cool graphic. I was very excited about my graphic.
[54:20] And I had to write this for a possible blog for someone else, but they didn't want it.
[54:27] And I was like, sweet, I'm going to keep it. Thank you.
[54:31] Yay, Canva. And Josh, I'm so glad you're still here.
[54:35] So yes, let's, we got it deployed. Let me go back.
[54:40] And we, did I run images yet? I don't think so.
[54:45] Did I? No, okay, cool.
[54:47] - Yeah, so run images. So this is gonna do is this is gonna show you the image
[54:51] that you just built and probably a couple others. So open that up wide ways so you can see it a little clearer.
[54:56] - Here we go. - There we go. So the one we created is at the very, very top.
[55:02] And you can see actually when each of these, when you created them, it'll tell you
[55:05] when you created them and how large they are. - Which is interesting because-
[55:10] - So you already did a Docker tutorial and you already have an Alpine thing.
[55:16] - And I was like, what those were some of the defaults that they talk you through,
[55:21] but it didn't really make sense to me while I was doing it. - So hopefully this makes more sense.
[55:28] So what this is gonna do now is it's going to run your container and it's going to take port 8080
[55:35] and pipe it into 49160. So now we're not going to access 8080 anymore.
[55:41] We're gonna access a different one. So that's why you have two port numbers here.
[55:44] And then you're just, you're running it in, there's a dash D there for a flag,
[55:50] which just means you're running it in a detached mode. So it's not going to like hang with like a server on it.
[55:56] Your thing is just going to kind of kick off and it'll be running in a background port.
[56:01] So if that doesn't make any sense, you'll see, you'll be able to just run the commands.
[56:06] - It's actually, I'm thinking about it because with Postgres, we were,
[56:12] because we were doing it with Docker and then we wanted to put pgadmin on it.
[56:17] It, we were running into a lot of port issues. So I'm wondering.
[56:23] - Another reason why running Postgres on a railway and grabbing the connection string is great
[56:27] 'cause you don't have to worry about conflicting with ports on your computer.
[56:30] - There we go. I don't know why that came up, but sweet.
[56:34] And then. - Okay, so now we're going to see the list
[56:36] of actual running containers. So you have a long list of images you've already created,
[56:41] but right now there should not be a lot of running containers.
[56:45] So we only have one. - That's the one we created.
[56:47] - Exactly. And it will tell you the name of the image
[56:50] and it'll tell you the command that's being run, which is not the node index command.
[56:55] It's like the Docker entry point command. So it's kind of one level abstracted.
[56:59] Most of this information is not super important except for the actual ports and the container ID.
[57:05] So you can see the ports it's running on, which I already kind of explained.
[57:08] But we're going to do this and you're going to grab the container ID
[57:11] that is spit out there and plug that. Yeah, you got it.
[57:14] - I was trying to copy and paste them out of order. Why don't you ever do that?
[57:20] I feel like it does a lot of really cool things. - And so make sure to get rid of the brackets on the end.
[57:25] - Oh. - Great, so that's how we know it's running.
[57:34] So now we need to open one of these. - Could we use the name?
[57:39] Like angry L back yawn? However you want to say that.
[57:46] Can we use that instead of the container ID? - Possibly, I'm not sure.
[57:52] Either way, you would have to run a command to look that up. So to me, it doesn't really make a difference.
[57:58] - Well, if it's like right here, that's why I'm wondering. Oh, you get it.
[58:08] - Look at you go. - That's fun.
[58:10] It's also the name. - Now we should actually open this in a browser
[58:13] so we can see our beautiful website once again. And so it's not 8080, it's 49160.
[58:18] - Yay. - And it should be the exact same thing.
[58:30] You did it, you're running a Docker container. - Yay.
[58:33] And then something that you have at the very, very end. And I feel like I always forget, what does cURL do?
[58:40] - So cURL is a way to basically hit a URL and just get the text input that the browser is interpreting.
[58:47] So do it and you'll see what happens. - Okay.
[58:51] - And I'm also including the headers as well. So it includes like the content type
[58:54] and the eTag and things like that. And then below that is the HTML
[58:58] that the browser is receiving, which is just a single H2
[59:01] that your express server is giving you. - Okay, and then, so I'm in Docker--
[59:07] - And then you'll see it there running at the bottom. You should bump up your font on your Docker desktop.
[59:12] - There you go. - Okay, there you go. So you can see it's running right now
[59:18] and you can go inspect it. So click it, see what happens.
[59:19] I don't use Docker desktop super often, but it'll give you a whole bunch
[59:22] of other information about it. - So this is something that I had to learn
[59:26] as a newbie looking at this. You can't, it's not the image or the ports.
[59:31] - It's the container, yeah. - I actually have to click on the name.
[59:34] - Yeah. - It's very annoying. - Totally, so try inspecting it or terminal.
[59:41] Yeah, just go through all of them, yeah, see what-- - Yeah, so you can do commands within it.
[59:46] You can see its files and stats about it. - There you go.
[59:51] - Pretty cool, I think. - Okay. - And I still don't understand the difference between,
[59:58] like I get it, but I don't get it. It's gonna take me a bit to understand
[60:01] like the difference between images and then like a project or something.
[60:07] I will get there, I will get there. - Image is a squishy word, 'cause it's just the code
[60:13] that represents the thing that you're running, which is contained entirely within the Docker file
[60:18] and the Docker ignore. So the image is like a series of steps
[60:22] that reproduces an artifact. So it's gonna be different for every project
[60:26] depending on what your dependencies are or what your node server does and all that kind of thing.
[60:31] But once you have it and you have the images created, then anyone can take that image
[60:36] and run a container based on an image. So the image is what takes a long time
[60:40] for an individual person to create so that lots of people can run that image
[60:44] without needing to think about it very much. - Very cool, and then something that's not on here
[60:51] is like the hubs, and the hubs is how it's set up to save to your Docker account,
[61:00] because right now-- - That's my blog post actually, so there's steps after this
[61:04] where I explain how you would publish this onto Docker Hub if you're so inclined.
[61:08] - Yay, let's do it. - I didn't include those in the gist here, 'cause it would have taken,
[61:11] we shouldn't do it, 'cause it's gonna add a whole lot of time. - Yeah, no, that's totally fine.
[61:15] - That's like a whole separate episode. - Yeah, that's totally fine.
[61:18] I mention it because right now, even though I put this, this is using Docker,
[61:23] it's local only, it's only on my computer. It is not-- - But I'm actually,
[61:27] well, I recommend before you even do that, though, right now what you should do is you should commit this
[61:31] to a Git repo and save it. - Well, you know what, y'all?
[61:37] I'm not gonna do it with CLI, because I always forget-- - I can tell you how to do it.
[61:42] Do you have the GitHub CLI? - Yeah, but look, I can initialize a repo here.
[61:47] - Hey, that's fine, too. Getting it onto the actual GitHub website is the main thing.
[61:52] Oh wait, actually, sorry, we need to create a gitignore before we do this, don't do that yet.
[61:56] Don't commit anything. - Oh, okay.
[61:59] - Create a .gitignore file. And then just put node_modules, that's all you need,
[62:08] and .ds_store. (laughs) - And what, .-- - Not,
[62:14] and then all capitalized, ds_S and then all lowercase after that, the word store.
[62:22] So, sorry, get rid of the extra S. There you go, yeah, 'cause then otherwise,
[62:29] when other people clone it down to their Apple, they get this stupid .ds_store thing.
[62:32] It's super, super obnoxious. (laughs) - Mm-hmm, mm-hmm, mm-hmm.
[62:38] New repo. Commit.
[62:41] Yes. Publish branch.
[62:47] Okay, that's fine. - Make it public, not private.
[62:51] - Well, I can go back and change it. Open on GitHub.
[62:54] - Oh, this is fun. - Yeah, no, you should make it a public repo
[62:57] 'cause the whole point of these things is it's a learning exercise for others as well.
[63:01] - I wasn't against making it public. I was against not clicking it.
[63:07] (laughs) - You're against not clicking the first option
[63:11] it gives you reflexively without reading the instructions. I know, it's a strong urge you have, I understand.
[63:19] - Yes, it is something I do on everything. And I don't even remember how to make it public.
[63:25] - Yeah, this is why you can never work in crypto. - No, no.
[63:29] - You would click the thing and then you would lose all your money
[63:31] and you'd be like, "Oh, I was supposed to click that thing. "Can I have my money back?"
[63:34] No. (laughs) - That is what would happen.
[63:38] Okay, see, we were just really wanting me to learn how to make this public.
[63:45] Maybe, pushes. Change visibility, change to public.
[63:55] I want to make it public. I have read, make it public.
[64:00] - Oh, oh. - This is why you should have done it
[64:06] from the thing in the first place. Unintended consequences.
[64:10] - Oh, okay. Yeah, this is why you don't always clicky clicky.
[64:19] But hey, I remembered my password. So we're good.
[64:23] It is now public. And we can do this.
[64:29] - So do one more thing now. Add a read me and just copy paste my entire gist.
[64:34] - Oh my God, I was just about to do that. Yay.
[64:37] - I was hoping you would do that. Yeah, just go to raw.
[64:40] Just copy paste that whole sucker. I can fill in my contact details and other stuff later.
[64:49] - Yay, look at us, we did it. Oh, actually, we can do one more thing.
[65:00] Although I should definitely put alt text with this, but. I'm almost done.
[65:13] I'm looking up the alt text that I put on other posts. So that way I don't have to rewrite whatever I'll.
[65:31] (indistinct) - Dude, why is it so hard to see alt text on?
[65:43] Like if you open the image on Twitter, you have to like reclose it.
[65:50] And I'll text. - Yeah, I don't know.
[65:54] - Come on. Hey, it's our faces.
[66:01] - Oh my God. - That was fun. - Did the thing.
[66:05] - Yay. Yay, we did the thing.
[66:08] And to take a page out of Scott's book, please make sure that you follow on Twitch
[66:16] and subscribe on YouTube. Make sure you follow everybody
[66:20] that is currently in the audience right now. You can find me on Twitter @jenshaw.com
[66:25] and you can find Anthony @ajcwebdev. Yay.
[66:31] (indistinct) I mean, like Scott, like I want to do that.
[66:37] Like you do such a good job at it. Oh, yay.
[66:42] Enjoy dinner. And yes, everyone, thank you for the stream today
[66:48] and coming in and hanging out. And tomorrow, oof, I have a stream
[66:54] during your Twitter space, but y'all they always have JavaScript Jam.
[67:00] Is it Jamstack? Why do I always get the name wrong?
[67:02] - JavaScript Jam. 'Cause I also do the FS Jam podcast,
[67:06] so it's easy to confuse them. But it's just JavaScript Jam.
[67:09] And yeah, you should leave that section saved so you can come hang out
[67:14] and just do your stream before or after. Like obviously I'm not saying reschedule the one you have,
[67:18] but for the future. - Normally I don't have streams on Wednesdays.
[67:23] Normally I'm pretty good. - Nah, that's even better.
[67:25] - Yeah, normally I just go stream. - Yeah, except you're usually there.
[67:28] - Yeah, but it might get over by then. I don't know.
[67:34] - Cool. - No, it's like during the end of it.
[67:37] If you guys have a two hour-- - We'll be talking about just some React Miami talks,
[67:40] Will, his Okta talk on web auth, and Anri, who will be talking about web page test
[67:47] and React performance stuff. - Nice.
[67:50] - We'll be talking about that, it'll be fun. - Yay, well, thank you everybody.
[67:55] And ooh, let's, I can do this. Yay, I'm excited.
[67:59] I will raid somebody once I figure out where I actually put my Twitch page,
[68:06] which is always really annoying. I don't know if any other streamers do that.
[68:10] I always like lose where I put Twitch itself. - Haha, let's see, who should we raid?
[68:19] My Twitch is not opening right now, but if BW's still going, you should definitely raid him.
[68:24] - Yes, he is, yay. Start raid.
[68:31] Y'all are gonna go watch a great stream, yay. It's thinking, why does it take so long to raid?
[68:40] I never get it. Well, y'all are ready now, bye.
[68:44] And yay, they raided. [BLANK_AUDIO]

