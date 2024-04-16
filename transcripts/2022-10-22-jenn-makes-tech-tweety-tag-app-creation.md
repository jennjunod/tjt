---
showLink: "https://www.youtube.com/watch?v=SYp004VhmWM"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "jenn-makes-tech-tweety-tag-app-creation"
title: "Jenn Makes Tech: Tweety Tag App Creation"
publishDate: "2022-10-22"
coverImage: "https://i.ytimg.com/vi/SYp004VhmWM/maxresdefault.jpg"
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

[00:00] What's up beautiful humans, I am rando streaming, probably going to be doing this a lot this weekend.
[00:11] Even if I only have like an hour to work on this, I definitely want to, because today I was planning on streaming earlier today, but I spent like the entire day getting my
[00:24] foot and ankle checked out because I am a silly goose and I use something that is not a chair for a chair and I shouldn't have, we'll just go with that, we will go with that.
[00:43] So I will be streaming D&D here in about an hour, not on my channel, but on another channel on Jacob's channel, but I can link that in, but today I have made some progress on my
[01:00] project. Let me bring that up, give me a second.
[01:11] And today's music, we are trying the not loop thing to see if that'll work. Did not bug people as much, but we will see, okay.
[01:39] So for whoever is joining the party tonight, I have made a Twitter, I want to make a Twitter space tagging app.
[01:53] I get that it's probably already exists, but I'm just seeing if I can do it. So the outline of what I want to get done is I'll work backwards.
[02:02] Look at this new doc of every week I host a mental health and Twitter space or mental health and neurodiversity Twitter space in tech, like about how it shows up in tech.
[02:16] So what I'm wanting to do is I always say, Hey, here's the Twitter space. Second tweet is always literally a copy and paste it.
[02:27] And then for everybody that signed up to be tagged, I put them in there and I'm like, Hey, this takes me like way too much time and thought process.
[02:35] And I do it every single week. So this is why I was like, you know, I really want to get a challenge that I learn everything
[02:45] that I've learned, use everything I've learned on teach gen tech thus far. So I am using a, I want to be able to enter a Twitter handle and the, uh, the Twitter
[02:58] space link and then combine them and have an auto post and hello, Ryan, what up? And Ryan's already heard all of this, but just in case, um, I am going to be doing it
[03:13] as a react JS web app, which I did work on mostly yesterday. And then I'm going to look into getting at least Prisma set up and then using my SQL
[03:24] and then Prisma and then the Twitter API to auto post. You're going to see how this goes because the plan keeps changing.
[03:32] And my goal is to get this done by Sunday. So I will probably be streaming on again, off again tomorrow in the fact that instead
[03:41] of streaming today, I, uh, good call, Ryan, good call. I, instead of streaming earlier today, I was hanging out at urgent care and getting x-rays,
[03:55] but my foot and ankle are fine. They're just super bruised.
[03:59] And anybody wants to see that go to my Twitter. It's there, not the proudest moment, but that is okay.
[04:07] So this is also giving me great practice in being able to go find my stuff and let's see. Oh, it didn't even loop it.
[04:25] So it doesn't keep going. The music doesn't keep going if it doesn't loop.
[04:30] Oh, that's dumb. Well, I'm going to loop eating the ducks because it's my favorite one.
[04:38] If somebody could look into new music for me, because you'll have to like have like specific things for like copyright issues and stuff, uh, that would be awesome because
[04:53] I like need something else. And so it was probably everyone else, but I will paste this in here in case anybody
[05:04] else feels like looking it up and looking into it and, you know, providing the stream new music because yeah, I'm, I got enough to worry about, so, okay.
[05:23] This is also getting me in the habit of coding every day, but also like how to properly import and export.
[05:31] So I did do a stream for teach down tech earlier today. It was for, um, a, to be able to create a Android app and I actually have bought an
[05:43] Android and everything to an Android tablet. And I'm actually not, not uploading that to get hub right now because it wasn't doing
[05:52] what we wanted it to do. So Zachary will be back on the show later on after I get this all figured out and we
[05:59] will be basically taking this app that I built and now make it an Android app and we'll put that on get hub, but this one, not so much so, and I know I need to clone it and working
[06:13] through this. So this one is named Twitter tagging because I'm a genius and didn't know what to name
[06:22] it as a heads up. I have had a cat named Blackie, like it's, I named things as I, they are, it's not, not
[06:34] the best at it. That's okay.
[06:36] Do you, do you, do you, we have not updated our read me yet, which yesterday I can go through what we did, but we are going to see if I can do this, right?
[06:59] What up homie? Oh dude.
[07:01] I don't know if you saw my tweet, but my foot. Okay.
[07:07] Good news. I do not have any like broken bones.
[07:12] Yay. This is great news.
[07:14] I do all though have a ton of bruising from my, my little spill earlier this week. And then also I have, uh, yeah, I fell really hard on Wednesday.
[07:32] I basically was standing on something that I shouldn't have been standing on and I fell off of it and then on top of it.
[07:39] So my ankle foot is really, really messed up. Um, and today's day two, which the, the way that, uh, urgent care explained it is that
[07:52] it, the swelling may go up, but we did do x-rays, nothing's broken. I may have some torn tendons.
[08:02] I don't know. We'll find out.
[08:05] Um, but I basically can't walk anywhere and I have a cool boot on, so I guess I could go look that up for you guys really quick on my, on my tweeter, on my tweeter.
[08:19] It, it was, you know, I've been doing really good in the last like month, uh, yeah, you know, people have, people definitely have.
[08:34] And I feel like I should like tell people this, but I don't know if they'll ever believe me.
[08:40] I am that person that like, how to say this. You would think I would have learned this lesson when I was like 12 when this first
[08:53] happened. So I don't know if these even, uh, like exist anymore, but like roller rinks, I was at a
[09:01] roller rink with my friends and with my roller blades on, and I'm going like back and forth with my roller blades while I'm on a chair.
[09:10] And it's so funny. Ha ha ha.
[09:12] I fell off. Everybody's laughing, but then telling me not to do it, which is so right.
[09:18] You know, like you don't want to do that. You might fall off.
[09:21] Um, so well, maybe me, even at a young age, I'm like, Oh, it'll be fine. And I do it again.
[09:31] Uh, but this time instead of falling to the side, I fall forward and there, I mean, I'm blind as can be, but I actually have a scar through my eyebrow because I fell forward.
[09:44] Huge, huge. This is, you can be in this chat or you can be on Twitch.
[09:55] So yes. Come over to Twitch.
[09:58] I need the link. Let me find my link.
[10:01] Where's the link? Where's the link?
[10:06] Because I need to get this project done and I have like 45 minutes to get it done or like to get it.
[10:13] Then. Yeah.
[10:15] I like, okay. So thank you.
[10:17] Thank you. Call me.
[10:19] Um, I have 45 minutes to get it done or like get progress on this because I spent all day at urgent care because it was like super, super fun thing to do and here, I will give
[10:34] you the link here as well. So it goes over there.
[10:39] This is me posting about my wonderful experience. Yeah.
[10:45] Oh, yay. Okay.
[10:47] Then yeah, I don't know how many times I've posted this, but that is the story about what I did and the photos of what I did because I'm very, very talented in volley is what
[11:02] I was telling everyone about and why I'm streaming. I will be, um, playing D and D here in like 45 minutes, so I'm like, I'm going to be at
[11:15] the computer. Let me at least like do something.
[11:19] So I need to make sure I actually copy this and I need to gear to the right folder. We didn't change content folder to something else.
[11:53] No, we're not. Well, maybe, but not now.
[12:00] What children's, uh, Oh, got a hot date. Yay.
[12:07] And like, Oh no, like, I mean, it's, I find it funny. I hope the comment at least like came across that.
[12:18] I found it funny that this kept happening over the garden wall. Does that have anything to do with like the secret garden over the garden wall?
[12:30] Y'all we are taking a quick, not ad break, a quick ADHD break to find out what over the garden wall is.
[12:43] But it's a movie, not a series as a movie. Okay.
[13:02] Let's see if we can look back and forth. Oh, geez.
[13:25] Okay. I will look at this more later.
[13:27] It looks interesting. I hope you enjoy your movie and hot date.
[13:33] What up? Bakari.
[13:35] Yes, I am awkwardly coding on a Friday night before I play D and E because it's, it's cool. And homey, you always make me laugh.
[14:00] What about like spirited away? I get, I mean, I like all those movies, but I can't say like, I don't know, like princess
[14:12] Mononoke, all those are all my go-to's, but I need to look up more. What am I doing?
[14:21] Okay. I have to minimize this.
[14:23] I don't know what my timeline is open. I'm going to exit this.
[14:28] All right. Here we go.
[14:30] We have it open. All right.
[14:41] So how many of you are doing trick-or-treating this year? Like either taking your kids or friends or just going yourself or like having candy for
[14:51] trick-or-treaters? Do you guys like actually like that stuff?
[14:54] I'm like, I'm, I'm gauging because I, I grew up super religious, so I don't know how it actually goes and I need Prisma, which I think, yes, oh, you need JavaScript.
[15:24] Oh, okay. That's cool.
[15:30] I hope you guys have fun. Oh.
[15:33] Oh yeah. Cause next weekend, Halloween is on a Monday.
[15:37] I forget that people do like Halloween parties throughout the entire month. I honestly don't think I've been to a Halloween party in like six years.
[15:50] Let me think about this. Yeah, probably not because Tyler's birthday is the day before Halloween and we go horse
[16:00] riding instead. It's a lot of fun.
[16:05] So we don't normally Halloween. Okay.
[16:08] We are going to figure out these silly relational databases and oh yeah, then yeah, I forgot that you said you have a conference or that you're going out there for the week, like
[16:34] uh, and then famine chill, huh? Many sneaks.
[16:43] I almost said sneakers, snickers, snickers. I hope you're not eating sneakers, but I mean, you could.
[16:51] Wow. Ryan.
[16:53] Wow. Okay.
[16:55] Y'all like, this is so weird. So I, um, Ryan sent me a connection on LinkedIn and he lives where I used to live and live
[17:05] there for like a year and worked at a casino and he lives there and it's like, How crazy is that?
[17:13] Like small world. Right.
[17:15] Oh. And then, yeah, I've been meaning to tell you, uh, Janica also lives in this area and
[17:22] we need to all hang out. I told Janica about it, Janica is down and I keep forgetting to tell you, as you know,
[17:28] I am horrible at remembering to tell people that I need my SQL server live in. Let's see if it's set up and if I can log back in.
[17:49] Yeah, but you worked at the casino at like, I think 10 years before I got there. Ooh.
[17:58] It's running. Yay.
[18:01] Okay. Y'all, I am showing this for this tutorial.
[18:07] Just know when I'm done, I am hiding all the shenanigans from you. Like I'm changing it, changing all the shenanigans.
[18:15] So ding, ding, ding. Okay.
[18:25] So I have a database. I don't know what I'm supposed to do with it, but I have it.
[18:31] Metrics? No.
[18:33] Databases. Create a new, I don't need a new database.
[18:41] It's got me as a member. Yeah, I don't know what I'm doing for all of this.
[19:11] Oh, that makes two of us. I'm working on it.
[19:13] Venya, I will show you my very cool Miro board that I'm very proud of. Okay.
[19:25] So Venya, you know how every week I like to tag everyone for my Twitter spaces. I literally put like the same post, just whatever the Twitter space link is, everybody.
[19:40] And then I tag everyone. And then I was like, I need to stop doing this.
[19:48] I need to do it, like automate it because it takes me forever. And then I forget to do it.
[19:52] So I want to make it so it enters the Twitter handle and enters the Twitter space link combined and voila, it spits it out.
[20:03] It's what I'm working on. So I came up with this one, I need to scoot down.
[20:09] This is like going to be in like a while. This is nowhere, nowhere soon.
[20:15] That to do all of this, I think this is what I need to do. I don't know.
[20:29] I think it's possible. We're going to find out probably, but I'm also using this as a good reason to see if
[20:39] it works, to learn it of what does and doesn't work. So this is one I'm very great at, Tyler will tell you I'm very great at it, of I will listen
[20:52] to other people's advice and then not take it, but not in the fact that I think I'd know better.
[20:59] So that doesn't click. I do want to own that, but other times I'm just really stubborn and want to see if I
[21:05] can figure it out. So that's kind of where we're at for this because I know it's definitely possible.
[21:18] Okay, I don't know. I probably can do a lot of random things that I don't know what I'm doing, but yes, I am
[21:58] trying to figure this out. I will ask you how to do that once I figure this out, because you're probably right, but
[22:15] I need to get this figured out. It's going to be great.
[22:17] It's going to be phenomenal. I think, Oh, I also have to, um, yes, I click on a lot of things and try to
[22:35] break a lot of things, which is probably very apparent as my foot is in a keep it safe boot. Maybe, maybe, guys, this boot, I don't even know what I'm doing.
[23:13] I don't even know how I would access this externally. Resources, so at this point, just so y'all know the
[24:05] part that I'm working on is Prisma is telling me prerequisites of it is that I have to have my Microsoft, uh, SQL server set up and that's what I'm using Ivan for.
[24:19] And I'm just trying to see if there's something else I need to look at, which I should probably just put this in my mirror board.
[24:37] Then yeah, I know I totally owe you an email reply. Did you reply to my tweet yet or tweet text tweet?
[24:48] We have too many ways of communication. I need like people to just like use one.
[24:52] Can I like say, Hey, only use like X because I feel like I lose people's conversations all the time.
[25:19] Are we even discord friends yet? I don't know if we're discord friends, that's an added complication.
[25:28] I just want to say you guys, when Venya and I first became friends, I was so awkward. I was like, yeah, so I don't know how to get ahold of you cause you said you don't check
[25:41] your DMS and that's the only way I know how to get ahold of you. I was really awkward.
[25:47] It's cool. I make friends in awkward ways.
[25:49] So it's going to be really fun. All right, Venya, I'm going to send you a, so we can be friends there too.
[26:08] It's going to be great. And Ryan, which are you asking, like which one Venya prefers, I'm guessing a discord
[26:25] where my friends, my friends had a new friend. Let's be friends based.
[26:36] Are you asking me, Oh, I'm discord. I would prefer discord because I forget to reply to emails and LinkedIn and DMs discord.
[26:49] I at least like, because it can do more, like I can add other people and stuff. I'll put my discord.
[26:58] People can add me on discord. I'm cool with that.
[27:00] Doggo, what are you doing? Where are you going?
[27:02] Go hang out with your dad, Doggo. Okay.
[27:04] I don't know. I guess I put it in YouTube.
[27:19] That's fine. YouTube can have it as well.
[27:22] Oh, uh, then, yeah, I always do it to YouTube too, so I don't have to download the video and upload it.
[27:28] I'll give you the money if it goes to both. I will say, uh, Oh, bye Vanya, have a wonderful time.
[28:16] Isn't Vanya lovely. She's such an incredible human.
[28:34] Uh, Oh, look like they're suggesting Python application. I'm like, we have Python on Mondays.
[28:43] Oh, y'all, if we become mean girls, like we wear pink on Wednesdays, ew, I get that Python is Mondays, but that's different.
[28:56] Right? I don't want to be a mean girl.
[28:59] Maybe I will be one day, who knows. Okay, well, I think I got it started, um, you are, Oh, do I have a connection you are
[29:21] up to this URI? I think that's it.
[29:37] Please hold while I yell at my dog. All right, that was fun.
[29:59] Okay. She likes to hurt herself.
[30:07] She has really bad allergies, so she looks to death. Um, all right, so learn to an existing Node.js or texture project.
[30:33] Y'all I'm staring at this because I'm realizing that I have that part set up as a react, not, but isn't all of, um, we're going to find out.
[31:03] We're just going to try it. Try it.
[31:05] Do we have packin.js? Pretty sure we do.
[31:12] Yes, yes we do. Okay, cool.
[31:17] We are there. I don't know if you guys can see this.
[31:59] I'm blind. I'm blind as a bat.
[32:30] Let's see what happens if I just force everything to be fixed. Why not?
[32:45] Oh, I'm blind. Oh, wow.
[33:36], I'm blind. If you couldn't tell, I definitely learned best by breaking it.
[34:22] I'm going to take a screenshot of this one because it is asking me to do, um, I'm going to, um, fix this in my Git ignore, but at the moment I'm going to ignore that and get
[35:02] back to it later and see what I can figure out then. Set the database URL and the dot EMB file to point to your existing database.
[35:17] If your database has no tables yet, read this getting started. Oh, I'm blind.
[36:09] Okay. Let's minimize these, these, uh, let's see, go.
[36:41] Okay. So I need Prisma and then schema dot Prisma.
[37:02] I don't know. Oh, we've got Prisma.
[37:08] I'm honestly just installing these because I'm like, that would make sense. You would want them a hundred percent.
[37:13] Don't know what they do. Great way of learning things.
[37:17] But these two look like they're from Prisma proper, so might as well get them. So definitely don't need all of these open still last time.
[37:29] Let's go back here. We're going to go to the schema.
[37:32] Oh yes. It looks great.
[37:34] Okay. So database, I need SQL server and my URL, database URL, which, yeah, it's a service
[37:58] URL. I got 15 minutes y'all.
[38:32] I need to like, actually, uh, How do I?
[39:19] I'm running out of CLI. Okay.
[39:52] Well, I do have an error, which is actually kind of cool. I'm going to go back to my, my, my, my.
[40:50] Oh, let's see if that will work. Hmm.
[41:47] Error in SRC report web vitals and tax error. I'm going to go back to my web vitals.
[42:28] Between line three and four. Okay.
[42:58] So I'm going to go back to my web vitals. Hmm.
[43:29] I don't know. Import syntax errors may only appear at top level.
[43:57] Hmm. And this is a JS file.
[44:27] Syntax, I like that cheat sheet. Oh, this is cool.
[44:48] This is also a lot. Oh, is it saying top level?
[45:19] Okay. Give me all these.
[46:03] Let's Google. Oh, that's a, a SRC index.
[46:28] Oh, are you trying to tell me one of your imports aren't working? Import.
[46:37] Error in. SRC report web vitals.
[46:57] I don't think this will solve it, but. Hmm.
[47:30] Oh, I'm now on Bakari. You know, you're always welcome back on the show. This is frustrating.
[47:49] Okay, we're going to Google this. Into the Googles you go.
[48:27] Hello. Hello. How's it going?
[48:33] I'm having fun. Working on whatever this error is.
[48:53] Oh, yes, Ryan. He is tagging the. Get repo that I am working on.
[49:03] Because I am working on building a nap. That there. Yes, there may be other ways to do this yet.
[49:09] This is me trying to figure it out just to see if it's possible. And to go through these frustrations myself.
[49:16] I am working on. Getting a react web app to work with Prisma to work with my SQL.
[49:25] To get to this. Possibly Prisma to the Twitter API to auto post a thread.
[49:33] Yeah. And my goal is to get this done by Sunday. We'll see.
[49:39] Okay. It looks like my DND crew might be running a little late.
[49:51] So I'm basically just waiting for them to tell me when I need jump. So.
[49:59] I'm on a schedule of, I just want to have a deadline. And if I don't view.
[50:06] It's going to be Friday night. I play D and D on Friday nights, Ryan.
[50:13] So I'm waiting for. The DM to let me know when.
[50:20] I need to hop from my screen and go on his screen. Yes, exactly.
[50:26] And. I streamed and I don't know how to say your name.
[50:34] Can I call you? Can I call, you know, or like,
[50:42] can you tell me where I'm supposed to like. The pronunciation.
[50:45] I'm so sorry. I'm bad at these.
[50:47] I. Also just, I've had this stream.
[50:58] Teach gen tech for three and a half months. And I keep doing stuff with people on the stream and not by myself.
[51:03] So. I can't do anything myself.
[51:07] I know I can. I just like to ask for help and get unstuck faster.
[51:17] Which does not mean I retain the knowledge. It's just frustrating.
[51:24] Yeah. It's.
[51:48] Okay. Now I'm really stuck on a name. Is it.
[51:56] Then new Cooney or new. Or anywhere close to that.
[52:02] Anyone else want to give a guess? Because.
[52:04] I have done it for free. New Coon.
[52:11] Is that it? Yes.
[52:19] I'm so bad. Yes. I think your name was one of the easiest names.
[52:31] Because you have a really cool name too. And, but you like the Cardi, the Kari, like, you know, the two put together.
[52:36] I always think of it. Yes.
[52:41] Yeah. Almost four months ago.
[52:51] And I've been live learning three to four times a week. I live stream.
[52:55] At a regular time. For this project,
[53:01] I'm just streaming whenever I can to get this stuff done and to hold myself accountable to get it done.
[53:05] And. It has been, it is.
[53:08] Yeah. Close a brace.
[53:16] On a lot of these. Oh, no. What is that?
[53:21] I want to know. Oh.
[53:31] Okay. Tell me.
[53:45] I don't even know what email address that is. I mean, it's definitely videos like this is yes.
[53:52] This is totally me trying to make videos. But it doesn't tell me what email address it is because my actual,
[54:00] my YouTube channel. Has like.
[54:04] No subscribers. Huh?
[54:18] Oh, it's not even going through. An existing.
[54:25] YouTube channel. So weird. I like Ryan. I totally.
[54:42] Don't know. I don't know. Okay. Whatever. Sorry.
[54:53] Okay. So I started this project almost four months ago and yeah,
[55:02] I was a dev rel consultant for. Three of those four months.
[55:08] And one of the biggest things that I needed to work on was the tech side of things.
[55:12] And I'm like, I can talk to anybody. I got this. And I love learning, but I did not have the tech.
[55:17] I didn't have the tech, but I did have the tech. So I was like, I need to make videos. I need to make videos.
[55:24] I need to make videos. And I was like,
[55:26] I need to make videos and I was like, I need to make videos and I was like,
[55:28] I need to make videos and I was like, I need to make videos and I was like,
[55:30] I need to make videos and I was like, I need to make videos and I was like,
[55:32] I need to make videos and I was like, I need to make videos and I was like,
[55:34] I need to make videos and I was like, I need to make videos and I was like,
[55:36] I need to make videos and I was like, I need to make videos and I was like,
[55:38] I need to make videos and I was like, I need to make videos and I was like,
[55:40] I need to make videos and I was like, I need to make videos and I was like,
[56:10] I need to make videos and I was like, I need to make videos and I was like,
[56:12] I need to make videos and I was like, I need to make videos and I was like,
[56:14] I need to make videos and I was like, I need to make videos and I was like,
[56:16] I need to make videos and I was like, I need to make videos and I was like,
[56:18] I need to make videos and I was like, I need to make videos and I was like,
[56:20] I need to make videos and I was like, I need to make videos and I was like,
[56:22] I need to make videos and I was like, I need to make videos and I was like,
[56:24] I need to make videos and I was like, I need to make videos and I was like,
[56:26] I need to make videos and I was like, I need to make videos and I was like,
[56:33] I need to make videos and I was like, I need to make videos and I was like,
[56:35] I need to make videos and I was like, I need to make videos and I was like,
[56:37] I need to make videos and I was like, I need to make videos and I was like,
[56:39] I need to make videos and I was like, I need to make videos and I was like,
[56:41] I need to make videos and I was like, I need to make videos and I was like,
[56:43] I need to make videos and I was like, I need to make videos and I was like,
[56:45] I need to make videos and I was like, I need to make videos and I was like,
[56:47] I need to make videos and I was like, I need to make videos and I was like,
[56:49] I need to make videos and I was like, I need to make videos and I was like,
[56:55] I need to make videos and I was like, I need to make videos and I was like,
[56:57] I need to make videos and I was like, I need to make videos and I was like,
[56:59] I need to make videos and I was like, I need to make videos and I was like,
[57:01] I need to make videos and I was like, I need to make videos and I was like,
[57:03] I need to make videos and I was like, I need to make videos and I was like,
[57:05] I need to make videos and I was like, I need to make videos and I was like,
[57:07] I need to make videos and I was like, I need to make videos and I was like,
[57:09] I need to make videos and I was like, I need to make videos and I was like,
[57:11] I need to make videos and I was like, 
