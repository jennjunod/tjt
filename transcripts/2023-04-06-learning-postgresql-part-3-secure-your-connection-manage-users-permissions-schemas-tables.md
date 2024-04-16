---
showLink: "https://www.youtube.com/watch?v=06Iw4IO76_I"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-postgresql-part-3-secure-your-connection-manage-users-permissions-schemas-tables"
title: "Learning #postgresql part 3: Secure your connection, Manage users/permissions,  schemas & tables"
publishDate: "2023-04-06"
coverImage: "https://i.ytimg.com/vi/06Iw4IO76_I/maxresdefault.jpg"
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

[00:00] Welcome to another episode of Teach Gen Tech. Today is day three of working on setting up Postgres.
[00:08] It's been interesting, it's been a learning journey and I appreciate everybody that has come along
[00:17] this journey with me. For those new to Teach Gen Tech,
[00:21] please click follow if you are watching along on Twitch, if you are on YouTube, subscribe, like all those things
[00:31] and for all the beautiful humans that already do, thank you, I appreciate it.
[00:36] And I'm here to either find the question or answer to the question, go find it,
[00:43] find someone who can help me through it and learn live so that way you can see what other people struggle with
[00:49] and ask your questions when I have experts on the show. Yay, all right, so I need to put these in the chat.
[00:58] You remember this. So if you're looking to check out previous episodes,
[01:06] here it is and what up, Anthony? Yes, that was the longest face ever.
[01:14] I was like, I gotta go do my stream. So I've got to drop and for those who don't know,
[01:23] Anthony is a host of JavaScript Jam. Owner, person, I don't know what your title is.
[01:34] You're a human of JavaScript Jam. JavaScript Jam.
[01:41] Oh, wow, oh, that's fun. Oh, that is fun, ask Anthony anything.
[01:54] I like it, I like it. That was a very, very long space.
[02:00] Did it just end? 'Cause I looked at it like right before I started streaming
[02:06] and it was still going, which is kind of bananas to me. Oh, oh, I bet Ryan did
[02:21] because you were joining the stream so often earlier, I think, I don't know, I don't know.
[02:30] Ryan shows up, we can ask him or Homie. Oh, I miss Homie, Homie might've made it.
[02:36] But yeah, you had a lot of like good conversations in it. I dig it and I hope that people learned a lot
[02:47] about how to handle going to a conference 'cause they're scary and difficult.
[02:53] Oh yeah, it probably was both of them together. Did I actually, no, I didn't paste it.
[03:09] Okay, I gotta paste this, paste. All right, so Anthony, I know you know
[03:17] where to find my content, but in case anybody needs to know,
[03:20] that is where they can go find it on YouTube. What I went through last week
[03:26] and what we're gonna see if I can figure out or this week, there's a lot to figure out.
[03:36] Yeah, yeah, I still have to like figure out how, yeah, yeah, there's a lot, there's a lot.
[03:48] I love my new job, it's so fun. It is, it definitely keeps me busy
[03:53] and there's so much to learn, which is great and scary. Ryan, did you know we were just talking about you?
[04:04] Is that like why you were like, yo, I'm gonna show up, like I wanna talk, I know they're talking about me.
[04:09] I feel like that, oh yeah, oh yeah. Anthony has a cool command and we don't know who made it.
[04:18] Okay, hi, this is my to-do list. I should move like what we did last week.
[04:31] Hey, let me just do this. Yeah, yeah, yeah, I thought that was so cool.
[04:43] I'm so happy, thank you for making it 'cause I do ask Anthony a lot of random things.
[04:48] Probably the other out of, I do like the Kiona ones, but I feel like the other really cool command
[04:57] is the clicking one. I don't even remember what the command is,
[05:03] but that I clicked too much or I click, I don't even remember what it's called,
[05:09] but it always makes me giggle when I see it. Okay, moving this here, move these up here
[05:16] and change the pen color. Oh, Anthony, I don't know if you saw this last week.
[05:26] I finally got my iPad and I can use it here. I'm pretty sure you did
[05:31] because anybody that was joining any stream, I was like, yo, you have to see this.
[05:35] But I'm really excited about it 'cause it makes me a lot more productive.
[05:41] And not look so weird online. And last week, okay, we'll do,
[05:47] ooh, not that, not that twice, not that twice. Go back, go back.
[05:51] Oh, good luck, Ryan, but yeah, like chime in if you hear anything you want to know more of.
[06:09] Oh yeah, I'm not great at always watching other people's streams.
[06:13] Like I try to go to them when I can, but like it's a lot of times where I'm like,
[06:21] you may not see me for months then. Let's see, so week one was set up local.
[06:38] Equals, nah, cool, that was cool, yay. Week two is, how many do you attend normally?
[06:51] Like how many do you see per week or go through? And for everybody joining, I am setting up Postgres.
[07:02] I'm gonna continue setting up Postgres, but I'm working on writing out what I have done
[07:09] and what I'll be doing today. And I like to share my notes on my iPad
[07:13] so I don't look so weird just looking down and talking to myself.
[07:17] Everyone else can see it too. Anthony, there's like, oh, yes, yes.
[07:24] No, I'm like, oh, yay, what up? Jonah, how's it going?
[07:35] Jonah Fado, Joe, Jonah, how would you like me to say that? 'Cause I like defaulted to Jonah,
[07:43] but I'm not 100% sure. And yeah, Anthony, like how many streams a week
[07:51] do you try to attend? 'Cause yes, I feel like I can almost always find people
[07:57] that I know that are streaming or podcasting or have new videos out, and I don't catch up enough.
[08:06] Last week, what did we do last week? I need to write this down.
[08:12] We set up Docker, yay, and, oh, no, that, yeah, okay. I installed, anybody's curious,
[08:30] I keep wanting to put like two S's in Postgres SQL. Jonah Fado, Jonah Fado, Jonah Fado,
[08:54] why is it if I still try to spell it out that I'm horrible at it?
[08:59] Jonah Fado, I hope that is close. And Anthony, oh, that's fair.
[09:10] Oh, yeah, I'm still bad at like even doing two or three, but I cut back on my streams,
[09:25] so I think I'll have more time for other streamers because I definitely burnt out on as many as they were
[09:33] going on and trying to keep up with all the content I had going on.
[09:40] Thank you, John. Yeah, that is something that I wish I was better about,
[09:49] is saying people's names properly. I have a dear friend who, to this day,
[09:55] I still say her name wrong, even no matter how much we practice it,
[09:58] and it's, you know, a work in progress. Oh, Anthony, that's smart, that is smart.
[10:11] I like it, putting them on in the background. And last thing we did was,
[10:23] wow, PG Admin, helps if I can. Client, okay, cool.
[10:38] And it sounds weird, but even if people aren't replying, it does make me, I feel like,
[10:48] a better streamer when I at least see numbers there, so I know that I'm not talking to myself.
[10:56] I don't know if that's how it is for anybody else. Okay, week three, I don't know what color that was.
[11:05] I think this color. Sure, why not, we'll do a bright color for this week.
[11:18] All right, so let's see how well I remember what I did last week.
[11:24] Okay. Yeah, there is something.
[11:38] - I'm curious, for those who are here, those who are lurking, when did you first start using Docker
[11:49] and what did you first use it for? Like, what was your first experience with it?
[11:55] - Oh yeah, let's do an update, yay, that was exciting. - Oh, Anthony, you're doing a nice job.
[12:05] - Yeah, I'm doing a nice job. - Okay, all right, let's see what else we have here.
[12:12] Oh, there's a couple of questions. Oh, that's great, that's great.
[12:17] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:20] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:21] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:23] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:25] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:26] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:28] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:30] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:31] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:33] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:35] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:36] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:38] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:40] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:41] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:43] Oh, there's a couple of questions. Oh, there's a couple of questions.
[12:45] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:14] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:16] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:17] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:19] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:21] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:22] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:24] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:26] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:27] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:29] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:31] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:33] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:34] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:36] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:38] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:39] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:41] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:43] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:44] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:46] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:48] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:49] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:51] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:53] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:54] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:56] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:58] Oh, there's a couple of questions. Oh, there's a couple of questions.
[13:59] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:01] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:03] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:04] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:06] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:08] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:09] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:11] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:13] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:14] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:16] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:18] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:19] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:21] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:23] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:24] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:26] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:28] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:29] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:31] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:33] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:34] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:36] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:37] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:39] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:41] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:42] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:44] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:46] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:47] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:49] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:51] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:52] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:54] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:56] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:57] Oh, there's a couple of questions. Oh, there's a couple of questions.
[14:59] Oh, there's a couple of questions. Oh, there's a couple of questions.
[15:01] Oh, there's a couple of questions. Oh, there's a couple of questions.
[15:02] Oh, there's a couple of questions. Oh, there's a couple of questions.
[15:04] Oh, there's a couple of questions. Oh, there's a couple of questions.
[15:06] Oh, there's a couple of questions. Oh, there's a couple of questions.
[15:07] Oh, there's a couple of questions. Oh, there's a couple of questions.
[15:09] Oh, there's a couple of questions. Which is definitely like a learning in its own right.
[15:15] It can be very, very frustrating for other people to see this because they're like,
[15:21] dude, just follow the instructions. I don't blame them.
[15:24] I 100% do not blame them for getting frustrated with it. For myself though, it's like,
[15:30] I wanna see if it's intuitive and then see how I get to the next step if I get stuck.
[15:36] Because I will remember things longer if I do it that way than if I follow instructions.
[15:43] And a lot of times with video, I do watch videos for other things outside of the tech world.
[15:53] Like if I want to, what's the thing that I've... Oh, seeing if different ways of running Genshin Impact,
[16:03] if I can, and doing walkthroughs there. I do that a lot.
[16:09] If y'all haven't played Genshin Impact, it's addicting. And I just bootcamped my other computer
[16:15] so I can play it on my computer. I'm excited to do that tonight.
[16:18] Anthony, it's useful to do the, just seeing if it's intuitive,
[16:26] messing around if we can figure it out. If you already have context,
[16:30] but it can waste a lot of time if not actually teach you anything.
[16:34] If you just go down a rabbit hole on a bug for hours, 100%, 100%.
[16:42] Last week, I was sharing a Miro board about all the steps that I'm going through.
[16:48] And one of the first steps of things to try to do to set all of this up,
[16:55] let me actually share this on the screen, was to set up Postgres local.
[17:03] One of the hardest things about doing that for myself was going to Postgres site and just trying to like,
[17:10] you know, figure it out and install it. And what I didn't know is that you still need to have,
[17:17] you need to install it locally. And then you still, so you need your server
[17:21] and you need your client, which was like, okay, cool.
[17:28] And, but I purposely didn't do any research before these streams.
[17:33] Yes, they will take me longer and it is frustrating. Yet, I'm also wanting to learn and get into
[17:42] how to learn these things. Because I think that's a big thing about breaking into tech
[17:50] is people get really stuck and don't know how to get unstuck based on their learning styles.
[17:59] (laughs) - Anthony, you're not wrong about it.
[18:06] I do have feedback for them. I will write it out.
[18:10] Maybe I'll blog it like, hey, if I knew this, this is what I would do if I were just setting up Postgres.
[18:16] But hey, it was a start. I did some things and I wasted like an hour and a half
[18:22] doing that because it wasn't the right direction I wanted to go, yet it wasn't a waste
[18:30] because I learned, right? I needed to learn.
[18:35] And last week was me clicking around Docker for a while, which was really awkward.
[18:42] And we had some really dope people join the stream last week and like, I think two of them were like sys admins
[18:50] and they were like, what did you do? They were experiencing the, I break shit
[18:57] and then I tried to figure it out and other people are like, what did you do?
[19:02] So we actually got these set up and now I have to remember what,
[19:09] I think it's this one. We got it set up.
[19:27] Let's see if I remember this. No.
[19:34] Anthony, this is why you write blog posts 'cause the official docs are missing a ton of steps.
[19:44] Your Docker blog posts is more thorough than anything in Docker docs.
[19:51] It's just an end-to-end tutorial. And I think that's a good call out.
[19:55] Like in my opinion, docs are not very accessible but it's also totally opinion.
[20:06] Hey, okay. No, I don't wanna change it
[20:18] because yes, I do want to save it. And I don't remember what we did.
[20:26] We had it working last time. Fair enough.
[20:39] I think Anthony, that's something that I need to clarify is I don't think it's necessarily who writes the docs
[20:48] but it's the fact that they're written because I may not always have the opportunity
[20:53] to do text-to-speech to help me comprehend it because it does take longer than a lot of people
[21:00] that can scan and do things, like scan through the text, find it really quick.
[21:05] I skip so many lines or discombobulate the words that it makes it really hard to use docs in general,
[21:15] like blogs in general, no matter who writes it. I struggle with that.
[21:19] And one thing that I've learned that has become incredibly helpful
[21:24] is like if I'm like reading one of your blogs of listening to it while I'm reading it.
[21:31] So that way, especially for tools like natural reader, they will highlight the word while it's being read to me.
[21:39] So I can actually learn it a lot easier. And I just wish I knew that back in like high school
[21:46] 'cause I would have known so much more and not felt so dumb.
[21:53] I feel, well, it's definitely not that, oh no.
[22:03] Yeah, that is very true. And it's all about stories.
[22:14] I really did like how y'all, and for those who are just joining,
[22:20] I was at a Twitter space earlier with Anthony that is a JavaScript jam.
[22:30] And they were having everyone from React, not everyone, but a lot of people from React Miami joined.
[22:38] And it was pretty cool because we were able to hear from a lot of the speakers.
[22:44] And I really liked Ryan's and talking about how storytelling is so important.
[22:52] Cora, I think it's Ryan Magoon. We're gonna go with, maybe that's how you say it.
[23:01] I will put their Twitter too. I live as Twitter as my default,
[23:07] but yet you can always Google them somewhere else. And if you want an introduction, let me know.
[23:13] I don't know all these people, but I can. All right, now I have to remember things.
[23:22] What did I do last time? Yeah, let's inspect some stuff.
[23:27] Okay, we got that going. I don't need that.
[23:32] Okay, well, I think I need to reset it up because I don't see my server in here anymore.
[23:39] Oh, it is, I just had to find it. Okay, that was exciting.
[23:47] I don't know if that was exciting for any of you, but this was exciting.
[23:51] This is my first time looking at this 'cause last time I was streaming last week
[23:59] about Postgres, we just wanted to get PgAdmin working and we were there for like two hours
[24:06] trying to get this thing figured out. And once we got it working, I was just like,
[24:10] "Okay, yay, done." Because I was so brain dead at that point.
[24:15] So this week I'm actually gonna go look for it, look at it.
[24:21] That means I can make this small, all small. And maybe we can make this small.
[24:30] We can do that, there we go. (humming)
[24:35] Okay, cool. So that way y'all can still see my notes.
[24:40] What up, Mr. Robot? How's it going?
[24:45] Thank you for joining. This is our to-do list this week
[24:50] is secure the connection, manage users and permissions, and create schemas and tables.
[24:57] I gotta be able to read my own handwriting. Wait, ooh, there's lots of databases.
[25:05] This is fun. If y'all had to choose a database,
[25:12] what database would you go with as your first database and why?
[25:16] I'm curious. Ooh, and something that I asked last time,
[25:29] you know, don't worry about like asking too many questions. What?
[25:35] Postgres on Railway? But then you would have to know Railway.
[25:39] Oh no, because that's another way of deploying it. Do you not need to have a client on?
[25:48] You don't have to do that. What?
[25:55] Oh, this is crazy. And Mr. Robot, I am doing good.
[26:01] Thank you. I am excited about working through this
[26:05] because I need to start making my how-to videos. Ooh.
[26:10] Okay, this is just gonna hardcore distract me. So we're gonna go back to this tab.
[26:20] Anthony, stop trying to distract me. I need to come through this.
[26:24] (silence) Oh, hey.
[26:54] I'm back. I don't know what just happened.
[26:57] Am I alive for y'all? Because everything just froze out and glitched on me.
[27:08] So hopefully it's still working. I'm gonna go with it's still working.
[27:15] I don't know what happened, but okay. Okay, yay.
[27:23] Well, at least I'm back. Oh, Anthony, I think you missed it last week
[27:27] of Josh joined my stream like half an hour into it. And I had no idea that I did not have audio
[27:36] for the first 30 minutes of my stream. That is talented.
[27:41] So, yay. And thank you for the follow.
[27:50] Okay. Not getting distracted by links that Anthony sends me.
[27:55] Oh, hey. So there is login and group roles.
[28:03] That is manage users. I'm guessing it might be over there.
[28:07] Create schemas and tables. Guessing table spaces.
[28:11] Or schemas. Okay.
[28:19] And again, for anybody that is joining, I am definitely, I'm gonna click around
[28:25] until I can see if I can figure it out. If not, then I will look things up.
[28:31] So feel free to give any feedback or like ideas or anything. I will Google the things soon.
[28:44] We got properties. Security.
[28:48] Just by clicking. This is exciting.
[28:54] Clicky, clicky. Okay, so I need to actually write down the steps.
[29:00] This is not something I did last time of writing down the steps I actually took,
[29:05] which is annoying because you should always document as Anthony says, you write a readme as you're doing it,
[29:11] and then you don't have to go back and watch it later. Anthony, look, I do listen to you.
[29:16] Now I just need to implement it. So we need to initiate Docker.
[29:44] I'm not great at documenting what I'm doing, but yes, it has.
[29:48] I actually work on writing down the steps I do or what I need to do better.
[29:54] So it would save me time if I implemented it. I don't always do that.
[30:06] So initiate Docker. So that's what we did first.
[30:15] And then second, we ran. That's actually a good question.
[30:26] What is this called? We ran the containers.
[30:31] Played the containers, ran the containers. We're gonna say ran.
[30:34] Postgres. Postgres.
[30:38] And PgAdmin. Oh, y'all can't see because I'm blocking stuff.
[30:51] That would help. PgAdmin.
[30:55] Container. And then three.
[31:06] Okay. Well, I don't know if I actually needed to run this.
[31:22] Because I did. Three.
[31:33] Click. PgAdmin.
[31:38] Quartz. And log in.
[31:47] Four. Was.
[31:52] We did the things. We went to Star House.
[32:01] On the lifts. Under servers.
[32:08] Shows. That one.
[32:20] Set up last week. Wee.
[32:28] That's gonna be a one word now. Dot, dot, dot, dot, dot, dot, dot, dot.
[32:32] Maybe this command helped. Yay.
[32:40] I don't know if this command was actually helpful or if I just ran it and it was just happened
[32:46] to be timing before I found server. But I just wanna make sure in case
[32:51] I need to go back to this and forget. So, maybe this command helps.
[32:57] And, oh, I should probably make sure that I can just read what that says.
[33:06] Command. There we go.
[33:08] Which was. Docker.
[33:13] Inspect. (mumbling)
[33:23] (mumbling) Okay, cool.
[33:43] Yay. That gets us caught up on what I previously did.
[33:48] Which is, oh, we did not want that. We want that.
[33:52] Okay. Okay, cool.
[33:54] So, with this, we, I went clicking around up here. Dependencies.
[34:07] What if I found it up here? (laughing)
[34:13] My next solo stream? I don't know, I've kind of been like very hit or miss.
[34:18] I know next week, oh, y'all should be excited about next week.
[34:22] I got setting up APIs with Postman and then like the basics of APIs.
[34:30] Like I know how to run APIs, but I don't always remember what stuff is called.
[34:33] So, I'm really excited about that one. And then also going further into the basics of data.
[34:39] And that's on Tuesday and Wednesday. So, I don't know.
[34:46] I might stream Monday or Thursday or the weekend. I'm just basically streaming on these ones when I can.
[34:53] So, if you want to come on and talk about Docker, you just let me know, Anthony.
[34:58] We will figure it out. 'Cause I could always use some help with Docker.
[35:02] It is very confusing. Like, I know you're getting off the screen,
[35:06] but I do wanna show you this. Oh, Norpie is a cool person that helped last week.
[35:11] And so did Vardahoff and Firefixity. They were all super dope.
[35:17] But like, if you are gonna come onto the stream, Anthony, these are some of the questions like containers,
[35:25] images, volumes. What are they all?
[35:29] What are they? What are all these things?
[35:34] So, excited for you to join sometime and we'll schedule that later.
[35:40] So, thank you. There we go.
[35:44] (silence) Well, yeah, but you know me.
[35:55] I like to like know these things. So, we'll talk.
[35:58] We'll talk. We'll figure it out.
[36:01] Okay. So, step five.
[36:05] 'Cause Anthony is always distracting me with other things going on, which happens.
[36:09] And I appreciate it 'cause you always like teach me new things.
[36:14] Okay. That is fair.
[36:18] Okay, bye. Okay.
[36:21] So, I feel like I figured this out and now I have to find it again.
[36:25] Nope. Nope.
[36:27] Nope. Nope.
[36:29] Nope. Okay, that is definitely, where did I find it earlier?
[36:32] Okay. It's because I didn't have the server correct.
[36:39] I got it. I got it.
[36:43] But now I don't. Damn it.
[36:46] (mumbles) (silence)
[37:12] Yes, I know y'all. I am probably annoyingly clicking through these again,
[37:33] but I was like, I thought this was super easy to find and now I can't find it again.
[37:38] So, I am doing what I thought I did earlier. But.
[37:46] No. Nope.
[37:56] Nope. How did I find this so well earlier?
[38:00] It was like super easy. Oh.
[38:03] Sure, let's like reset the layout. No, no, let's not do that.
[38:13] Just kidding. Yep.
[38:26] Not that. Sweet.
[38:28] (silence) Page of session details.
[38:36] Security. It was under, oh, it's because I have this clicked
[38:42] and it doesn't have security. I had database clicked and it doesn't have security.
[38:47] But if I have Postgres clicked, it has security. So, that is something worth going into.
[38:57] So. I don't like how close that is.
[39:07] It is. Go down.
[39:09] Thank you, thank you. So.
[39:12] On the left. After.
[39:26] After. PG.
[39:30] Is. Selected.
[39:34] Under. Server.
[39:41] Click. Database.
[39:48] And. Click.
[39:57] Postgres. Under.
[40:09] Second top menu? Sure, we'll go with that.
[40:26] Second. Top.
[40:28] Menu. Click.
[40:34] Properties. Sure.
[40:41] We're gonna go with, that is the instructions I have so far.
[40:44] I'm gonna forget to do this. Y'all feel free to yell at me
[40:48] if you need me to move my screen. I don't feel it would just be easier to do it like this.
[40:52] Ooh, I'm gonna get very giant. But.
[40:56] Move my coffee. It is four o'clock in the afternoon
[41:00] and I'm drinking coffee. I don't think I'm technically supposed to do this,
[41:03] but hey, it keeps me awake. I'm down.
[41:06] All right. So we have security.
[41:16] And we have default table privileges. Can't do anything with this.
[41:25] Okay. Dude.
[41:31] Like, thank you for not judging. I gotta go to bed at 8 p.m.
[41:37] 'cause I gotta wake up really early, but you know, it's 4 p.m. here.
[41:40] And I'm totally, it's kind of funny that you joined because I was going to send you a message at some point
[41:47] and be like, yo, I'm gonna hit you up later because my Chrome.
[41:51] But I can't do D&D and stuff either. Like, it doesn't let me do Forge.
[41:57] It tells me a bunch of errors. If anyone is curious of the randomness I'm talking about,
[42:05] there is, oh, there are a lot of notifications on Twitter and I don't know why.
[42:10] Oh, because Anthony. Anthony.
[42:16] That is normally what happens is because of Anthony. He's always, he's my favorite person to blame.
[42:23] I did it 'cause of Anthony. So this is what my browser randomly just does
[42:29] or doesn't do. It's super fun.
[42:32] But then also, y'all should, if you're curious about where I go to hang out
[42:43] is there's a really cool Discord server. And we play D&D and stuff.
[42:49] It's fun. Dylan Seuss Read Guild.
[42:56] Y'all should just go follow the Twitter 'cause it's cool. And Nick, just as a other random thing,
[43:09] I posted last week because Roy was trying to help me out with this
[43:16] and I posted in the light of Araxis. Channel of like all the issues I was having.
[43:26] So I will ask you about all of this later. 'Cause at the moment, it lets me do my thing.
[43:32] We'll see if it doesn't later. Okay, so this is very giant.
[43:38] Can I move this? Yes, yes I can.
[43:40] Thank you. I appreciate that.
[43:51] You've always been so helpful. Nope, nope, nope, nope.
[43:58] Okay, so that is, oh, pencil. Okay, okay.
[44:05] I'm really glad I'm writing directions 'cause that would be funny.
[44:13] That would be interesting. So see you then.
[44:16] Okay. Click pencil.
[44:26] I'm using Notability and I'm still learning how to like actually connect the,
[44:40] like to do emojis and stuff. I drew an emoji the other day.
[44:46] It was pretty funny. Okay, so we click the pencil
[44:50] and we're gonna go to security. Oh, this isn't too hard.
[44:57] All right, let's roll this over. Okay, so we are, ding, ding, ding, ding, ding, ding.
[45:09] We are, ding, ding, ding, ding, ding, ding, ding, ding. Let's see.
[45:22] Secure connection. Well, secure connection, okay.
[45:31] Guarantee. Oh, okay.
[45:34] Grantee, not guarantee. These are public.
[45:39] Maybe it's Postgres? All?
[45:44] I don't know. So everybody's still hanging out.
[45:59] What are you up to on this lovely morning, evening, night, afternoon,
[46:04] whenever you are hanging out with us? What's with the question mark?
[46:22] Ooh. Database dialog to define or modify database.
[46:31] To create, you must be a database super user or have create privileges.
[46:37] The database dialog organizes the development of a database through the following dialog tabs.
[46:47] General, definition, security, and parameters. Use the database field to add descriptive name
[46:58] to the database. Okay.
[47:01] Okay. So.
[47:14] Huh. And now we Google.
[47:24] Now we Google. Because I'm seeing like this would work for privileges
[47:29] and security for like if we wanted to make it for a user, but it's not.
[47:40] Security label, what lights you up? Why is that an auto?
[47:47] I don't know. But I'm not seeing like how you would secure the connection
[47:57] and like other IP addresses. So, and now we Google.
[48:01] Okay. So.
[48:04] PG admin. Secure.
[48:16] Secure connection. Server dialog.
[48:28] Connecting to a server. Establish SSL connection.
[48:32] Oh, that does make more sense, which I believe, no, that was SQL.
[48:40] Yay, Jen, for being dyslexic. I totally thought that said SSL.
[48:47] You know, there's things. So, let's go back to the Googles.
[48:54] Establish secure connection to Postgres. Let's click this one.
[49:00] No, I'm just gonna hit X. Theirs looks much different than mine,
[49:15] so let's go out of that. Documentation.
[49:18] Postgres. Secure connection.
[49:30] So, it does seem that it's for securing the connection for an SSL,
[49:47] which does make sense. So, that being said,
[49:51] I kinda wanna go look around for something else then. Okay.
[50:00] Hmm. I think that just takes us, yeah.
[50:24] Definition, security. Advanced, schema restriction.
[50:32] No, okay, cool. Back to the Googles.
[50:42] Oh. Oh, okay.
[51:02] So, this is saying that I'm gonna go move this over here as we figure it out.
[51:10] So, let's get a new color. And we will call this.
[51:35] Okay, so this is saying that Postgres has a native support using SSL connections
[51:46] to encrypt the client server communications for increased security that requires
[51:51] an open SSL installed on both with the SSL support compiled.
[51:59] And the Postgres server can be started with SSL-enabled by security parameter
[52:07] by setting the parameter SSL on on Postgres. Interesting.
[52:15] And for those who may be newer to this world of like the techie world,
[52:27] like if you're just coming to hang out and you're like, dude, I don't even know what an SSL is
[52:30] or what Postgres is, that's fine. I'm working on learning how to Postgres
[52:37] and what the processes are because for work, I will be creating how-to videos.
[52:44] And so, I'm kind of just figuring out how does it go? That being said, I'm familiar with an SSL
[52:53] because I used to work at GoDaddy, which sold domains. So, if you wanted to get like gengenod.com,
[53:02] I went to GoDaddy and was like, yo, I wanna buy that domain. That domain needs to be mine.
[53:07] It was available. So, I bought it and I built a website.
[53:12] We'll use my website for an example. So, I bought it and I built a website, which is cool.
[53:19] I really like my website. It's on Astro if you wanna look it up.
[53:22] And, but people may get like an alert saying that my site's not secure.
[53:28] That is when this little padlock thing is not here. Connection is secure, yay.
[53:34] So, if it wasn't secure, you would get an error. So, side note, that's my understanding
[53:43] of an SSL secure socket layer. There is a lot more going on there
[53:47] that I don't necessarily understand, but I need to stay on task and not go down a rabbit hole.
[53:53] It is difficult. It is very, very difficult not to go down rabbit holes.
[53:58] So, by some parameter, SSL on in the PostgreSQL and .conf, the server will listen
[54:16] to both normal SSL connections in the same port and negotiate anything within the client.
[54:26] How to set up the server to require SSL. Okay, the server reads system load,
[54:35] open SSL configuration file. By default, this is named openssl.cnf
[54:41] and it's located in the directory reported by OpenSSL version D.
[54:47] Okay. Yo, this is why you don't like reading them.
[54:53] Like, what? Okay, this is, there's things going on here.
[55:00] So, let's see if I can find other things that help explain what I'm doing.
[55:07] All right. And if I'm going to anybody, like,
[55:14] yes, there's companies that create it, but like this one is like from someone individual,
[55:21] Nicholas, it looks like. Hi, Nicholas, is these are never like personal,
[55:28] like, hey, I don't like this person did something horribly wrong.
[55:31] This is like more of a, no, I don't get what they exactly said.
[55:35] So, please know that these resources aren't helping me, but that doesn't mean that they won't help you.
[55:40] Okay, an SSL is a security measure that encrypts data sent between two devices.
[55:47] At least they explained it better than I did. That makes more sense than what I said.
[55:53] And they don't, hey, look, here's a video. Wait, what to which part?
[56:00] There was a lot of said, a lot said in the last while. Oh, fair enough.
[56:12] No, look, this person's named Nicholas too. I feel like it would be weird to call you Nicholas.
[56:19] Like, I didn't register that. Because you always go by Nick.
[56:24] You always go by Nick. Like, it'd be weird to call you Nicholas.
[56:29] Do you ever go by Nicholas? Is your proper name, your first name, proper name, full name?
[56:37] I don't know how you say that, but does anybody else call you Nicholas?
[56:45] 'Cause I can tell you if somebody calls me Jennifer, I don't register that anybody said,
[56:52] if somebody says Jennifer in like a waiting room, I have no idea that they're talking to me.
[56:57] And if someone says Jenny, it doesn't register either. Unless it's my family, they still call me Jenny.
[57:03] Oh, I mean, that is fair. We were talking to John earlier who was like super dope
[57:12] and they tried to spell their name out for me. And yo, I'm horrible at it.
[57:18] And I feel so bad. Like, why are Americans taught how to like
[57:23] talk different languages from birth so that way we can actually say other things
[57:29] than just English? I will one day learn another language after coding.
[57:35] This has been a journey on itself. Okay, prerequisites.
[57:48] Okay. Oh, I do like that they put prerequisites.
[57:51] That is a good way of writing a blog. I dig that.
[57:55] Well, we don't have that. We don't have that.
[57:59] Well. So, let's look up
[58:08] Postgres secure connection docker.
[58:17] Enabling SSL, Postgres and Docker. Okay.
[58:25] We got a gist, gist, gist. How do you guys say it?
[58:34] Do you say it like with a G like gist or with a J like gist?
[58:38] I feel like that's the same as giffy or jiffy. Yay.
[58:46] What up, Daniel? I know I'm not saying that to anybody on the stream
[58:50] if your name is Daniel, also hello, but also talking to the Daniel that wrote this.
[58:56] Oh, I like that they wrote, what is Docker? What's Postgres?
[59:02] Oh, this is fun. I like this.
[59:05] Because OpenSSL is quite complex to use, we'll use certstrap for generation of certificates.
[59:13] Oh, y'all. Oh, damn.
[59:19] This is like very, very multi-step. Not gonna lie.
[59:30] I was kind of like, oh, it's probably gonna be easy. This one, not so much.
[59:36] I don't know if I have the brain power for this. Because I also want to see
[59:44] if there is a certain secure connection or IP restriction that was requested
[60:07] on my list of doing things. So I will, questions, questions.
[60:14] Connection, name, SSL, there it is. Wow.
[60:40] Let's try typing or writing. A specific (mumbles)
[60:46] Huh. I would also say like something I'm working on learning
[61:07] and I'll be doing this as part of my like tests as well. Would this be needed for Ivan too?
[61:15] Because eventually I will be trying to set it up with like the products that my company uses.
[61:20] Yet at the same time, I'm like, cool. Would they need to do it too?
[61:27] Or is this just because we did it with Docker or we didn't do it?
[61:31] Like maybe because earlier we had Anthony on the stream talking about doing it with Railway,
[61:40] setting up Postgres with Railway. So in my mind, I'm like,
[61:43] does that mean that we would need PgAdmin and the secure connection with those as well?
[61:51] So I need clarification from this. And they're all asleep in Europe right now.
[61:59] So they're not gonna be around for me to ask right now. So would Ivan need secure connection?
[62:08] And then also, let's see. What about Railway?
[62:34] Cool. I'm gonna bookmark this.
[62:44] Now I'm gonna go back to this earlier. Let's do, I have too many bookmarks.
[62:52] No, I need that out still. Oh, we can put that one in there.
[62:59] We can put that one in there. Let's do that one in there.
[63:05] We'll do that one in there. That one's good too.
[63:10] I don't know what that one actually is. Oh, it's my GitHub.
[63:17] Do I have it twice though? Why do I have it twice?
[63:21] That's dumb. All right, so we got rid of that bookmark.
[63:25] And we have Postgres, how to set it up the SSL. We got that bookmarked.
[63:30] So we're doing good. Let's go look at my notifications.
[63:32] Oh, look, lots of people. Lots of people that I follow on DevToo.
[63:38] Oh, hey. Why are you saying there's still?
[63:45] Oh, okay. Stop telling me that there's notifications.
[63:50] It always annoys me when it tells me there's notifications.
[63:53] I'm like, no, bro, go away. All right, so we are putting Secure Connection on hold
[63:59] until I verify some things. I'm just gonna move this over here.
[64:15] It's doing connection. And when it's ready.
[64:19] And when it's ready. On hold.
[64:26] Cool, that's cool. We got some things going on.
[64:32] What is an Indus server or should I say data plane? That is a solid question.
[64:44] I will say, and thanks for joining DC. I am new to setting all of this up.
[64:52] I actually just randomly started downloading Postgres without any information about it.
[65:00] Yet I have people coming on the stream next week, next Wednesday, I have somebody coming on
[65:07] to talk about the bare basics of data. They are also one of the most genius people I know
[65:13] and talking about all sorts of data infrastructure. So it's always really fun to get the experts
[65:20] to break down the basics. Yet, DC, are you on the Twitters?
[65:29] Yes, I called it the Twitters. That totally made sense.
[65:34] It's cool. But are you on Twitter?
[65:38] 'Cause what I can do is ask about this and get it back to you tomorrow.
[65:45] (murmurs) What up, Max?
[65:55] Ah, Twitter is too fast for you. Well, if you follow on here on Twitch or on YouTube,
[66:03] I will answer it next week when I have Ben on the show. I'll see if he can help me answer that.
[66:10] And I'm happy to see if we could tag you or something to like let you know.
[66:16] But let me, 'cause we have questions from last week. Because Norah Pye, Varda Hoth and Firefix
[66:28] were all like hanging out and doing stuff. So I have them.
[66:34] That's why they're yay. But let me write down your questions.
[66:38] Oh, you know, I always forget. You can yell at me when I'm not sharing the,
[66:44] I am also, if anybody's curious, I am doing this from my iPad.
[66:49] This is the way I learn is I write notes and they're always all around.
[66:53] But a lot of people weren't able to follow up like what I was talking about.
[66:58] So luckily, hey, I got a job, yay. And the first thing I did was get a tablet
[67:04] so that way I can share the experience with y'all. And you're not like, what are you doing, Jen?
[67:09] So I will put that down that notes. (humming)
[67:14] Do you see Raid Boss? Oh my gosh, we're just going a little crazy right now.
[67:30] (humming) I will answer that once I'm done writing these down.
[67:42] And server. And I'll just say data plane, cool.
[67:54] I started working at a company called Ivan. Hey, we can go check them out.
[68:02] We can like go stalk them really quick. They are a data infrastructure company.
[68:08] They are based out of Finland, which is really cool. I got to go to Finland.
[68:12] Our team's offsite happened to be three days after I started, so that was an experience.
[68:19] And oh, as what position? I am a developer advocate.
[68:25] So my main focus is helping those new into tech be able to get an understanding of all of these platforms.
[68:36] This is a big reason why I started my show, Teach Gen Tech. And then also one of the reasons I got hired at Ivan
[68:44] is I live learn, I learn live. And it's part of what I wanted to do.
[68:52] I already thought databases were fascinating, even though I don't know too much about them.
[68:56] You know, learning about what the different databases do and how to set them up.
[69:03] And I'm starting with Postgres. And thank you for the follow, Max.
[69:08] I appreciate it. So yeah, Postgres is first.
[69:16] And then I'm gonna learn some Redis. And then my SQL.
[69:21] And then I really, I really don't know what I'm gonna do next.
[69:31] I have worked on learning some Kafka. Like there were times I've had streams
[69:35] about people coming on about Kafka. And I'm just like,
[69:40] I don't even know what you just said to me on a lot of it. So starting with something that makes a bit more sense.
[69:47] And then, you're trying to learn and get off the business side
[69:55] of the company into data engineer analyst. That is pretty cool.
[69:59] - Yeah, it's, what do you use mostly? Because like I work with some of the most
[70:07] insanely intelligent people on like as developers and things that I am happy to like ask them questions
[70:16] and follow up. You might be further in your journey than I am.
[70:20] Yet it's like, that's why I'm so excited for Ben to come on the stream.
[70:25] Oh, that's, oh, this is like, is it doing it?
[70:29] I don't know if you guys saw it. Did it do it?
[70:32] That's not gonna do it. My Chrome glitch is out.
[70:36] So I was just seeing if it showed up for anybody else, but I don't think it's gonna do it again.
[70:40] Let me, and thank you for the follow DC, yay. Let's go Google Ben.
[70:53] Oh geez, I will pass it along. I will pass it along.
[71:06] Max, I will definitely pass that along. And then DC, you mainly use your Terra data
[71:16] as my SQL solution, some Postgres, Python for cleaning and wrangling, some analytics, then Tableau.
[71:24] Tableau, wow, I haven't said that word in Tableau. There we go.
[71:30] I'm like, I haven't said that word in a really long time. I will tell them as well, Max, like I just said.
[71:36] Is this, I haven't even looked at it to see which one their heading is.
[71:42] I'll look at it later. I need a look, I keep listening to it.
[71:45] I like that it will tell me which one's the headings and stuff.
[71:48] Um, that is something that I think is interesting is like, I still need to learn more about like Terra data
[72:00] and like what each of these are for. I currently am learning Python every other Friday
[72:09] using, actually, y'all can go see this. Like, let's go look.
[72:15] So, not now, not now, not your turn. So, right now I'm working on my Postgres stuff,
[72:24] but I'm learning Python and TypeScript as well. So, I actually have the books in my Notability,
[72:33] which this Notability does not sponsor me. I just really like this tool because let's say that,
[72:45] why do I have this book marked? I don't really know why, but that's okay.
[72:50] We'll go down here. But let's say that I have questions
[72:54] and I can be like, yo, what? Because it's a virtual book.
[73:01] But I, and this is the cover of it in case anybody wants to see.
[73:07] Learning TypeScript, I can show you a bit more. The author of this book actually comes on the show as well.
[73:16] And these are some notes of last week's stream. This is what I do is I just like run up
[73:22] and ask some questions, it's super fun. That being said, Teradata is like, I'm like, look,
[73:30] I know what my SQL is, cool, or Azure SQL Solution. And I'm like, but what are all the differences with SQL?
[73:39] Why are there so many? 'Cause I've heard of KSQL and I'm like, what is that?
[73:43] And then also the, I still really don't understand how you move
[73:53] the different types of data, but that's a big reason that Ben has been coming,
[74:00] is coming on the show and has been on the show of talking about how to,
[74:10] like breaking down the types of data and working on all of that
[74:17] because it is, can be incredibly confusing. And we'll just go like LinkedIn stock 10.
[74:25] That's fine, let's go LinkedIn stock 10. We can do this together.
[74:29] Got mad skill. So he's worked in data for so long
[74:37] that he's one of the people that have been coming on the stream and then also,
[74:44] oh, I should go grab the YouTube. Where's the YouTube set at?
[74:48] Let's go find the YouTubes. Oh yeah, I created a playlist.
[74:57] This is exciting. All right, it is, here is the playlist,
[75:04] but it currently only has one video with Ben. And you can kind of see more of where we're at for that.
[75:13] Although, I like to do things at the same time of,
[75:21] let's talk about really, really complicated things and really basic.
[75:24] So that is more of the basics side of things. And I am going back over here.
[75:35] Okay, cool. Oh, hey, my dog's here.
[75:38] I noticed the door opened and suddenly appeared a dog. So we have got Postgres, Postgres, okay.
[75:49] I am also putting Teradata because I wanna ask him about it now.
[75:53] Let's see. Let me go here.
[76:00] I am currently going to put on hold security connection. So let's do manage users and permissions.
[76:11] Where to start? I don't know.
[76:21] That is fair. What are you, I guess,
[76:32] there's so much that goes into it. Is there a specific thing that you're wanting to do
[76:40] or could you tell me more about where to start? I don't know.
[76:44] That is a complex spot to be in. I forget what I was putting on,
[76:56] manage users and permission. [76:58],
[77:01] and one through seven is the same. Get there.
[77:20] Yay. Same, same.
[77:23] Same. One through seven.
[77:29] Cool. So we'll do eight.
[77:32] Let's see. Okay.
[77:43] So we're here. I'm gonna go properties, go to pencil.
[77:47] I feel like it would be privileges, but at the same time,
[77:53] definition, parameters, let's do the Googles. The Googles.
[78:08] I feel like this needs to be stronger. Wow.
[78:23] I hope this is still, I did not want you to go that back.
[78:26] Thank you. Okay.
[78:28] Wow, I'm so fucking slow. Permissions.
[78:41] CD admin. User management dialogue.
[78:51] Roll, login group, roll dialogue. Okay.
[78:56] I like the YouTubes. That is a good way to learn.
[79:06] Database roles. And if y'all can hear my dog, I am sorry.
[79:13] Hope she's not too noisy. Please let me know if she bothers you too much.
[79:19] Open link in new tab. Okay.
[79:25] Database roles, attributes, role membership, dropping roles, predefined roles.
[79:32] Function security. Okay.
[79:36] Okay. We'll see if she chills out
[79:51] or if she's gonna make me get up and walk away. We will find out.
[79:56] Access permissions using concept of roles. A role can be thought of as either a database user,
[80:08] a group of database users, depending on how the role is set up.
[80:13] I am trying to make a new folder, not folder. Postgres set up.
[80:32] Sweet. We need, oh, I wonder if this would work.
[80:37] Yeah, that should work. Probably a little better.
[80:47] So I stopped cutting this off. And we're gonna put this in here.
[80:51] Yay. So, more questions.
[80:57], look like that. We'll go back to it.
[81:27] Oh, wait, no, that's not what I wanted. So let's just do,
[81:34] that one's user. User management dialogue.
[81:41] Okay. When invoking, that's for PG admin though.
[81:49] So let's do Postgres. Postgres manages permissions through the concept of roles
[81:59] with roles or it's noticing distinction between users and groups.
[82:04] Roles are more flexible than the traditional unique system of users and groups.
[82:09] For example, a role can act as a member of another role inheriting its permissions.
[82:15] Interesting. I feel like that just answered my other question.
[82:22] Let's see. Oh, okay.
[82:29] Let's bookmark this one too. How to list users and permissions
[82:46] and using psql command. Hmm.
[82:55] Interesting. I kind of want to try this now.
[83:09] All right. I think this.
[83:20] This needs to be all of this. Yeah, all the way to the down.
[83:30] I'm spilling my coffee everywhere. That's cool.
[83:38] Not what I want to do. Oh, that's rude.
[83:45] Hmm. Fine.
[84:03] We will use this user. Hmm.
[84:09] A connection to server on socket. See, this is the issue.
[84:21] Helps if I read and not just try to do passwords a million times.
[84:33] Oh, doo, doo, doo, doo. Oh.
[84:43] Interesting. This is a very old one.
[84:51] Hmm, okay. That's why.
[85:00] That answers the question, yay. So, no, we do not need this.
[85:06] We're not gonna talk about that because that does not help us.
[85:11] Neither does AWS. This one looks more aligned with the words I used, but.
[85:25] Let's see. - Also, older one.
[85:31] - Y'all, we may not be streaming for a minute. The doggo is freaking out.
[85:38] Like, she's going a little bananas. So, let's take a look and.
[85:45] Oh yeah, I'm totally like gonna see if my partner is gonna be home soon
[85:53] or if I gotta go take care of her. Which is okay.
[85:57] You know, you know. Oh, thank you for the follow.
[86:01] I appreciate it. And yes, please let me know when y'all have questions.
[86:07] Stacey was asking some great questions that I'll be following up with next week.
[86:12] No, he's still at work. Oh, we might have to go take care of the doggo.
[86:27] Well, this was not everything I wanted to do today. But we are gonna look like this one.
[86:34] We have made progress, yet not where I want it to be. Tell him to use just instead of unbuntu.
[86:52] Yeah, yeah. That is, can you all actually hear her?
[86:57] Do you hear the whining in the background? I'm just curious.
[87:00] 'Cause it is really loud for me. Just curious if you guys can hear her.
[87:07] She's grumpy. She's a 13 year old doggo.
[87:12] I don't know if my crayon still works. Let's see.
[87:14] Oh, I'll try to work through it. You know, see if it, I think, yes, no.
[87:27] I don't remember what the command that Ryan set up for this is.
[87:41] I'm so bad at this. Like, I'm like, oh yeah,
[87:44] I forgot all of the commands that are possible. This is cool.
[87:47] I need to write them down. I need to add that to the channel.
[87:53] That would help. All right, well, I'll get that figured out next week.
[88:00] That is something that, oh, that's what it is, is it's, okay.
[88:06] Oh, it's Kiona. It's with a K.
[88:09] Ayo. Kiona, Lady Kiona is 13 year old bulldog.
[88:20] (silence) Oh, hey.
[88:25] Oh, this is so cool. Yo, can we just like give a shout out to Ryan?
[88:31] I am the one who set this up. I am, you know, I'm great at talking to people,
[88:38] learning, learning the things, following through with the,
[88:43] going and setting up stuff for my own channels. Not the best.
[88:48] (silence) Oh, this is so happy.
[88:52] Yay. Okay.
[88:55] Oh yeah. Okay.
[89:03] I am definitely A bookmarking this for channel commands and
[89:10] (silence) Yay.
[89:19] (laughs) That is so funny.
[89:28] Okay. Well, the doggo is absolutely driving me insane.
[89:33] So I'm really glad y'all can't hear her because she is not happy at the moment.
[89:40] Doggo. Let's see if you guys can see her.
[89:46] I don't know if the lighting will work. You're gonna move a little bit.
[89:51] Sorry if anybody sees sick. That is Kiona.
[89:55] She is really annoying me. So, I am going to take her out.
[90:09] I need to put my BRB. Ma'am, I'm trying to talk.
[90:17] I'm so glad you guys can't hear her. She is a lot.
[90:21] (humming) (laughs)
[90:27] All right. So I will be back.
[90:41] Hopefully y'all will still be here. I'm gonna go take her on a walk and I'll be back.
[90:47] So, please hang out BRB soonish, soonish. Soonish.
[90:52] (upbeat music) (upbeat music)
[90:58] (upbeat music) (upbeat music)
[91:03] (upbeat music) (upbeat music)
[91:08] (upbeat music) (upbeat music)
[91:13] (upbeat music) (upbeat music)
[91:18] (upbeat music) (upbeat music)
[91:24] (upbeat music) (upbeat music)
[91:29] (upbeat music) (upbeat music)
[91:34] (upbeat music) (upbeat music)
[91:39] (upbeat music) (upbeat music)
[91:44] (upbeat music) (upbeat music)
[91:50] (upbeat music) (upbeat music)
[91:55] (upbeat music) (upbeat music)
[92:01] (upbeat music) (upbeat music)
[92:06] (upbeat music) (upbeat music)
[92:11] (upbeat music) (upbeat music)
[92:16] (upbeat music) (upbeat music)
[92:21] (upbeat music) (upbeat music)
[92:27] (upbeat music) (upbeat music)
[92:32] (upbeat music) (upbeat music)
[92:37] (upbeat music) (upbeat music)
[92:42] (upbeat music) (upbeat music)
[92:49] (upbeat music) (upbeat music)
[92:57] (upbeat music) (upbeat music)
[93:05] (upbeat music) (upbeat music)
[93:13] (upbeat music) (upbeat music)
[93:21] (upbeat music) (upbeat music)
[93:29] (upbeat music) (upbeat music)
[93:38] (upbeat music) (upbeat music)
[93:45] (upbeat music) (upbeat music)
[93:53] (upbeat music) (upbeat music)
[94:01] (upbeat music) (upbeat music)
[94:09] (upbeat music) (upbeat music)
[94:18] (upbeat music) (upbeat music)
[94:26] (upbeat music) (upbeat music)
[94:35] (upbeat music) (upbeat music)
[94:42] (upbeat music) (upbeat music)
[94:50] (upbeat music) (upbeat music)
[94:58] (upbeat music) (upbeat music)
[95:06] (upbeat music) (upbeat music)
[95:14] (upbeat music) (upbeat music)
[95:22] (upbeat music) (upbeat music)
[95:31] (upbeat music) (upbeat music)
[95:38] (upbeat music) (upbeat music)
[95:46] (upbeat music) (upbeat music)
[95:54] (upbeat music) (upbeat music)
[96:02] (upbeat music) (upbeat music)
[96:10] (upbeat music) (upbeat music)
[96:18] (upbeat music) (upbeat music)
[96:27] (upbeat music) (upbeat music)
[96:34] (upbeat music) (upbeat music)
[96:42] (upbeat music) (upbeat music)
[96:50] (upbeat music) (upbeat music)
[96:58] (upbeat music) (upbeat music)
[97:06] (upbeat music) (upbeat music)
[97:14] (upbeat music) (upbeat music)
[97:23] (upbeat music) (upbeat music)
[97:30] (upbeat music) (upbeat music)
[97:38] (upbeat music) (upbeat music)
[97:46] (upbeat music) (upbeat music)
[97:54] (upbeat music) (upbeat music)
[98:02] (upbeat music) (upbeat music)
[98:10] (upbeat music) (upbeat music)
[98:19] (upbeat music) (upbeat music)
[98:26] (upbeat music) (upbeat music)
[98:34] (upbeat music) (upbeat music)
[98:42] (upbeat music) (upbeat music)
[98:50] (upbeat music) (upbeat music)
[98:58] (upbeat music) (upbeat music)
[99:06] (upbeat music) (upbeat music)
[99:15] (upbeat music) (upbeat music)
[99:22] (upbeat music) (upbeat music)
[99:30] (upbeat music) (upbeat music)
[99:38] (upbeat music) (upbeat music)
[99:46] (upbeat music) (upbeat music)
[99:54] (upbeat music) (upbeat music)
[100:02] (upbeat music) (upbeat music)
[100:11] (upbeat music) (upbeat music)
[100:18] (upbeat music) (upbeat music)
[100:26] (upbeat music) (upbeat music)
[100:34] (upbeat music) (upbeat music)
[100:42] (upbeat music) (upbeat music)
[100:50] (upbeat music) (upbeat music)
[100:58] (upbeat music) (upbeat music)
[101:07] (upbeat music) (upbeat music)
[101:14] (upbeat music) (upbeat music)
[101:21] (upbeat music) (upbeat music)
[101:27] (upbeat music) (upbeat music)
[101:33] (upbeat music) (upbeat music)
[101:39] (upbeat music) (upbeat music)
[101:45] (upbeat music) (upbeat music)
[101:51] (upbeat music) (upbeat music)
[101:57] (upbeat music) (upbeat music)
[102:03] (upbeat music) (upbeat music)
[102:09] (upbeat music) (upbeat music)
[102:15] (upbeat music) (upbeat music)
[102:21] (upbeat music) (upbeat music)
[102:27] (upbeat music) (upbeat music)
[102:33] (upbeat music) (upbeat music)
[102:39] (upbeat music) (upbeat music)
[102:45] (upbeat music) (upbeat music)
[102:51] (upbeat music) (upbeat music)
[102:57] (upbeat music) (upbeat music)
[103:03] (upbeat music) (upbeat music)
[103:09] (upbeat music) (upbeat music)
[103:15] (upbeat music) (upbeat music)
[103:21] (upbeat music) (upbeat music)
[103:27] (upbeat music) (upbeat music)
[103:33] (upbeat music) (upbeat music)
[103:39] (upbeat music) (upbeat music)
[103:45] (upbeat music) (upbeat music)
[103:51] (upbeat music) (upbeat music)
[103:57] (upbeat music) (upbeat music)
[104:03] (upbeat music) (upbeat music)
[104:09] (upbeat music) (upbeat music)
[104:15] (upbeat music) - Anybody up to anything fun now?
[104:21] (upbeat music) (upbeat music)
[104:26] (upbeat music) (upbeat music)
[104:32] (upbeat music) (upbeat music)
[104:38] (upbeat music) (upbeat music)
[104:44] (upbeat music) (upbeat music)
[104:50] (upbeat music) (upbeat music)
[104:56] (upbeat music) (upbeat music)
[105:02] (upbeat music) (upbeat music)
[105:08] (upbeat music) (upbeat music)
[105:15] (upbeat music) (upbeat music)
[105:21] (upbeat music) (upbeat music)
[105:27] (upbeat music) (upbeat music)
[105:33] (upbeat music) (upbeat music)
[105:39] (upbeat music) (upbeat music)
[105:45] (upbeat music) (upbeat music)
[105:51] (upbeat music) (upbeat music)
[105:57] (upbeat music) (upbeat music)
[106:03] (upbeat music) (upbeat music)
[106:10] (upbeat music) (upbeat music)
[106:15] (upbeat music) (upbeat music)
[106:21] (upbeat music) (upbeat music)
[106:27] (upbeat music) (upbeat music)
[106:33] (upbeat music) (upbeat music)
[106:39] (upbeat music) (upbeat music)
[106:45] (upbeat music) (upbeat music)
[106:51] (upbeat music) (upbeat music)
[106:57] (upbeat music) (upbeat music)
[107:04] (upbeat music) (upbeat music)
[107:09] (upbeat music) (upbeat music)
[107:15] (upbeat music) (upbeat music)
[107:21] (upbeat music) (upbeat music)
[107:27] (upbeat music) (upbeat music)
[107:33] (upbeat music) (upbeat music)
[107:39] (upbeat music) (upbeat music)
[107:45] (upbeat music) (upbeat music)
[107:51] (upbeat music) (upbeat music)
[107:58] (upbeat music) (upbeat music)
[108:03] (upbeat music) (upbeat music)
[108:09] (upbeat music) (upbeat music)
[108:15] (upbeat music) (upbeat music)
[108:21] (upbeat music) (upbeat music)
[108:27] (upbeat music) (upbeat music)
[108:33] (upbeat music) (upbeat music)
[108:39] (upbeat music) (upbeat music)
[108:45] (upbeat music) (upbeat music)
[108:52] (upbeat music) (upbeat music)
[108:57] (upbeat music) (upbeat music)
[109:03] (upbeat music) (upbeat music)
[109:09] (upbeat music) (upbeat music)
[109:15] (upbeat music) (upbeat music)
[109:21] (upbeat music) (upbeat music)
[109:27] (upbeat music) (upbeat music)
[109:33] (upbeat music) (upbeat music)
[109:39] (upbeat music) (upbeat music)
[109:46] (upbeat music) (upbeat music)
[109:51] (upbeat music) (upbeat music)
[109:57] (upbeat music) (upbeat music)
[110:03] (upbeat music) (upbeat music)
[110:09] (upbeat music) (upbeat music)
[110:15] (upbeat music) (upbeat music)
[110:21] (upbeat music) (upbeat music)
[110:27] (upbeat music) (upbeat music)
[110:33] (upbeat music) (upbeat music)
[110:40] (upbeat music) (upbeat music)
[110:45] (upbeat music) (upbeat music)
[110:51] (upbeat music) (upbeat music)
[110:57] (upbeat music) (upbeat music)
[111:03] (upbeat music) (upbeat music)
[111:09] (upbeat music) (upbeat music)
[111:15] (upbeat music) (upbeat music)
[111:21] (upbeat music) (upbeat music)
[111:27] (upbeat music) (upbeat music)
[111:34] (upbeat music) (upbeat music)
[111:39] (upbeat music) (upbeat music)
[111:45] (upbeat music) (upbeat music)
[111:51] (upbeat music) (upbeat music)
[111:57] (upbeat music) (upbeat music)
[112:03] (upbeat music) (upbeat music)
[112:09] (upbeat music) (upbeat music)
[112:15] (upbeat music) (upbeat music)
[112:21] (upbeat music) (upbeat music)
[112:28] (upbeat music) (upbeat music)
[112:33] (upbeat music) (upbeat music)
[112:39] (upbeat music) (upbeat music)
[112:45] (upbeat music) (upbeat music)
[112:51] (upbeat music) (upbeat music)
[112:57] (upbeat music) (upbeat music)
[113:03] (upbeat music) (upbeat music)
[113:09] (upbeat music) (upbeat music)
[113:15] (upbeat music) (upbeat music)
[113:22] (upbeat music) (upbeat music)
[113:27] (upbeat music) (upbeat music)
[113:33] (upbeat music) (upbeat music)
[113:39] (upbeat music) (upbeat music)
[113:45] (upbeat music) (upbeat music)
[113:51] (upbeat music) (upbeat music)
[113:57] (upbeat music) (upbeat music)
[114:03] (upbeat music) (upbeat music)
[114:09] (upbeat music) (upbeat music)
[114:16] (upbeat music) (upbeat music)
[114:21] (upbeat music) (upbeat music)
[114:27] (upbeat music) (upbeat music)
[114:33] (upbeat music) (upbeat music)
[114:39] (upbeat music) (upbeat music)
[114:45] (upbeat music) (upbeat music)
[114:51] (upbeat music) (upbeat music)
[114:57] (upbeat music) (upbeat music)
[115:03] (upbeat music) (upbeat music)
[115:09] (upbeat music) (upbeat music)
[115:15] (upbeat music) (upbeat music)
[115:21] (upbeat music) (upbeat music)
[115:27] (upbeat music) (upbeat music)
[115:33] (upbeat music) (upbeat music)
[115:39] (upbeat music) (upbeat music)
[115:45] (upbeat music) (upbeat music)
[115:51] (upbeat music) (upbeat music)
[115:57] (upbeat music) (upbeat music)
[116:03] (upbeat music) (upbeat music)
[116:09] (upbeat music) (upbeat music)
[116:15] (upbeat music) (upbeat music)
[116:21] (upbeat music) (upbeat music)
[116:27] (upbeat music) (upbeat music)
[116:33] (upbeat music) (upbeat music)
[116:39] (upbeat music) (upbeat music)
[116:45] (upbeat music) (upbeat music)
[116:51] (upbeat music) (upbeat music)
[116:57] (upbeat music) (upbeat music)
[117:04] (upbeat music) (upbeat music)
[117:10] (upbeat music) (upbeat music)
[117:16] (upbeat music) (upbeat music)
[117:22] (upbeat music) (upbeat music)
[117:28] (upbeat music) (upbeat music)
[117:34] (upbeat music) (upbeat music)
[117:40] (upbeat music) (upbeat music)
[117:46] (upbeat music) (upbeat music)
[117:52] (upbeat music) (upbeat music)
[117:58] (upbeat music) (upbeat music)
[118:04] (upbeat music) (upbeat music)
[118:10] (upbeat music) (upbeat music)
[118:16] (upbeat music) (upbeat music)
[118:22] (upbeat music) (upbeat music)
[118:28] (upbeat music) (upbeat music)
[118:34] (upbeat music) (upbeat music)
[118:40] (upbeat music) (upbeat music)
[118:46] (upbeat music) (upbeat music)
[118:52] (upbeat music) (upbeat music)
[118:58] (upbeat music) (upbeat music)
[119:04] (upbeat music) (upbeat music)
[119:10] (upbeat music) (upbeat music)
[119:16] (upbeat music) (upbeat music)
[119:22] (upbeat music) (upbeat music)
[119:28] (upbeat music) (upbeat music)
[119:34] (upbeat music) (upbeat music)
[119:40] (upbeat music) (upbeat music)
[119:46] (upbeat music) (upbeat music)
[119:52] (upbeat music) (upbeat music)
[119:58] (upbeat music) (upbeat music)
[120:04] (upbeat music) (upbeat music)
[120:10] (upbeat music) (upbeat music)
[120:16] (upbeat music) (upbeat music)
[120:22] (upbeat music) (upbeat music)
[120:28] (upbeat music) (upbeat music)
[120:34] (upbeat music) (upbeat music)
[120:40] (upbeat music) (upbeat music)
[120:46] (upbeat music) (upbeat music)
[120:52] (upbeat music) (upbeat music)
[120:58] (upbeat music) (upbeat music)
[121:04] (upbeat music) (upbeat music)
[121:10] (upbeat music) (upbeat music)
[121:16] (upbeat music) (upbeat music)
[121:22] (upbeat music) (upbeat music)
[121:28] (upbeat music) (upbeat music)
[121:34] (upbeat music) (upbeat music)
[121:40] (upbeat music) (upbeat music)
[121:46] (upbeat music) (upbeat music)
[121:52] (upbeat music) (upbeat music)
[121:58] (upbeat music) (upbeat music)
[122:04] (upbeat music) (upbeat music)
[122:10] (upbeat music) (upbeat music)
[122:16] (upbeat music) (upbeat music)
[122:22] (upbeat music) (upbeat music)
[122:28] (upbeat music) (upbeat music)
[122:34] (upbeat music) (upbeat music)
[122:40] (upbeat music) (upbeat music)
[122:46] (upbeat music) (upbeat music)
[122:52] (upbeat music) (upbeat music)
[122:58] (upbeat music) (upbeat music)
[123:04] (upbeat music) (upbeat music)
[123:10] (upbeat music) (upbeat music)
[123:16] (upbeat music) (upbeat music)
[123:22] (upbeat music) (upbeat music)
[123:28] (upbeat music) (upbeat music)
[123:34] (upbeat music) (upbeat music)
[123:40] (upbeat music) (upbeat music)
[123:46] (upbeat music) (upbeat music)
[123:52] (upbeat music) (upbeat music)
[123:58] (upbeat music) (upbeat music)
[124:04] (upbeat music) (upbeat music)
[124:10] (upbeat music) (upbeat music)
[124:16] (upbeat music) (upbeat music)
[124:22] (upbeat music) (upbeat music)
[124:28] (upbeat music) (upbeat music)
[124:34] (upbeat music) (upbeat music)
[124:40] (upbeat music) (upbeat music)
[124:46] (upbeat music) (upbeat music)
[124:52] (upbeat music) (upbeat music)
[124:58] (upbeat music) (upbeat music)
[125:04] (upbeat music) (upbeat music)
[125:10] (upbeat music) (upbeat music)
[125:16] (upbeat music) (upbeat music)
[125:22] (upbeat music) (upbeat music)
[125:28] (upbeat music) (upbeat music)
[125:34] (upbeat music) (upbeat music)
[125:40] (upbeat music) (upbeat music)
[125:46] (upbeat music) (upbeat music)
[125:52] (upbeat music) (upbeat music)
[125:58] (upbeat music) (upbeat music)
[126:04] (upbeat music) (upbeat music)
[126:10] (upbeat music) (upbeat music)
[126:16] (upbeat music) (upbeat music)
[126:22] (upbeat music) (upbeat music)
[126:28] (upbeat music) (upbeat music)
[126:34] (upbeat music) (upbeat music)
[126:40] (upbeat music) (upbeat music)
[126:46] (upbeat music) (upbeat music)
[126:52] (upbeat music) (upbeat music)
[126:58] (upbeat music) (upbeat music)
[127:04] (upbeat music) (upbeat music)
[127:10] (upbeat music) (upbeat music)
[127:16] (upbeat music) (upbeat music)
[127:22] (upbeat music) (upbeat music)
[127:28] (upbeat music) (upbeat music)
[127:34] (upbeat music) (upbeat music)
[127:40] (upbeat music) (upbeat music)
[127:46] (upbeat music) (upbeat music)
[127:52] (upbeat music) (upbeat music)
[127:58] (upbeat music) (upbeat music)
[128:04] (upbeat music) (upbeat music)
[128:10] (upbeat music) (upbeat music)
[128:16] (upbeat music) (upbeat music)
[128:22] (upbeat music) (upbeat music)
[128:28] (upbeat music) (upbeat music)
[128:34] (upbeat music) (upbeat music)
[128:40] (upbeat music) (upbeat music)
[128:46] (upbeat music) (upbeat music)
[128:52] (upbeat music) (upbeat music)
[128:58] (upbeat music) (upbeat music)
[129:04] (upbeat music) (upbeat music)
[129:10] (upbeat music) (upbeat music)
[129:16] (upbeat music) (upbeat music)
[129:22] (upbeat music) (upbeat music)
[129:28] (upbeat music) (upbeat music)
[129:34] (upbeat music) (upbeat music)
[129:40] (upbeat music) (upbeat music)
[129:46] (upbeat music) (upbeat music)
[129:52] (upbeat music) (upbeat music)
[129:58] (upbeat music) (upbeat music)
[130:04] (upbeat music) (upbeat music)
[130:10] (upbeat music) (upbeat music)
[130:16] (upbeat music) (upbeat music)
[130:22] (upbeat music) (upbeat music)
[130:28] (upbeat music) (upbeat music)
[130:34] (upbeat music) (upbeat music)
[130:40] (upbeat music) (upbeat music)
[130:46] (upbeat music) (upbeat music)
[130:52] (upbeat music) (upbeat music)
[130:58] (upbeat music) you

