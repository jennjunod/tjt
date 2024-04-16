---
showLink: "https://www.youtube.com/watch?v=I_E0WlZNtoE"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-how-to-setup-postgresql-pt-1"
title: "Learning how to setup #postgresql pt 1"
publishDate: "2023-03-22"
coverImage: "https://i.ytimg.com/vi/I_E0WlZNtoE/maxresdefault.jpg"
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

[00:00] Hello, hello beautiful humans! Welcome to another episode of Teach Gen Tech and today's first episode of Using OBS. So, with that in mind, please let me know if
[00:16] something's not working, if you can't hear me, if the screen's not working well because I need to learn how to use it too. And today, it's just me. I don't have a
[00:28] guest today. I am also nervous, but that's never gonna change. That is something that is great about live learning and doing things live is, well,
[00:42] it's just what's gonna happen. Everybody is just gonna see me awkwardly go through things. But today is gonna be about learning Postgres, Postgres SQL.
[00:56] I've heard. I like it bro-nifty. Fuck it if we're doing it live. Yeah, that's it's basically my my philosophy in life. I've done an entire talk about it. Hello,
[01:13] hello. Yeah, we are setting up a Postgres SQL database today. I've never done it. I have a to-do list of things to check out and try to do. So, let me grab that. I
[01:35] totally have it on a Google Doc just so I remember what I'm doing. Yay! Okay, so yay. And hey Chrissy, what's up? I'm so excited that I actually have
[01:55] the chat up here because I feel like I would forget to say hi to people and now the other people can say hi to each other. So, yeah. And one of the coolest, not
[02:07] coolest, I'm not really sure mattering on your perspective of doing this is, so getting started, is we kind of have to figure out where to go get Postgres.
[02:22] Postgres SQL. Okay, SQL. Yay! So, we're going to the website. Sweet. Oh, there's options. I also will say that I totally chose like Postgres as the
[02:39] first one because if you didn't know this, I love elephants. Love elephants. I have a ton of elephants. One day I want to take time off to go to Africa and
[02:51] spend time helping elephants, which I don't know if anybody knew, but if you ever go to a rescue like that or somewhere that does the rehabilitation,
[03:04] at least from what I've seen, is it's like a ton of work. Like you're working like 14 hours a day, six days a week, and one day I'm gonna be able to afford that.
[03:15] I'm very, very excited. Okay, well, we got a couple different ways. So, we can local, of course, Ivan's where I work, so we do have options on doing it through Ivan
[03:26] too. Just gonna see where it goes from here. I'm gonna make this smaller, though, so people can see what I'm doing. I think that makes it so I can fit most.
[03:42] Elephants like peanuts. I mean, I don't know if they actually do. Do they? Download! We're on Mac.
[03:56] Wait, so this is me just like thinking, okay, cool, so it does have a, can be installed through Homebrew. I was just thinking that. I was like, wait, can't you
[04:17] do it through CLI? Oh, there's also the Postgres app. That's kind of fun. What do you think, y'all? How should we install it today?
[04:38] Any thoughts on what we should do? Because I'm kind of thinking that this Postgres app looks kind of fun. But I am open to suggestions, and I won't play
[04:57] music for all of you, sorry. I don't know if it's going to be royalty-free, but it's really weird just sitting here in silence listening to myself, so we're
[05:06] gonna have some music for myself. Look at the cute little elephant!
[05:26] It's a full-featured installation package. Hmm.
[05:54] Okay, I know I totally said it that way, but now, now I'm backing out. I'm backing out. I'm going to Homebrew. Does that mean I already have it installed? If we're doing
[06:25] documentation. Oh, this lets me check it. Hmm, let's monitor it then. "Check if Postgres is installed with Homebrew."
[07:13] I'm asking this because I've done a lot of things, like with installing on Homebrew, and I am not to the point yet where I know exactly what's installed. I
[07:29] know that it's installed a lot of things that many use often, so I need to figure out if it's actually been installed. Okay, so we can, that's on Windows, that's not
[07:52] helpful. That checks the status. Hmm. I'll just assume it's. I see Homebrew, and that's
[08:21] cool. Okay, so we're not gonna try Homebrew. Homebrew installs, uh, look at what. I still don't know. Is it bro-nifty or bro-nify? Bro-nifty. Like, how do you say
[08:36] it? Which way? "Homebrew installs it on its own directory, then symbolic link directs it to your path." "gg is going to be easier to use from Docker."
[08:54] Brother-nifty. Okay. Brother-nifty. Bro-nifty. Then, uh, I'm just gonna go back to the first one on the installer because, well, it is the first one that it gives, and I
[09:11] just, like, looked into all the other complicated ones. Yay. Yay. Okay. Yes, open please. Move this over here so y'all don't see it. Not like you can see
[09:37] what I'm typing, but, you know, you never know. I'm open to just trying to get it to work. Just, if it's, whether it's through a client or, um, server, just seeing if I
[09:58] can get it to work. I'm thinking right now, because I know that I set up a code folder, so thinking
[10:13] if I should, we're gonna say we're gonna put it in the library. Yep, we're, we're gonna do that, and it gave me my command link. Oh, I'm gonna take that one off
[10:26] screen, too. [laughs]
[10:31] [music] And we're gonna go with the default port, because that's what it gave me, and for
[11:08] all of those joining, I am working on setting up Postgres, and I've never done it just by itself, and nor completely understand it, so we're just kind of going
[11:22] step through step, and seeing what I can figure out. Yeah. Yay. Yay. I am curious for everyone joining, and, uh, Bro Nifty, do you prefer when streamers have
[11:51] background music, or when they're, it's, like, just them talking? I've been very curious about this, because I've heard both, especially when people want to go
[12:00] back and actually watch the stream. [music]
[12:26] Yay. Um, music is vibe. Yeah. I feel like I'm gonna have to figure that out for next week. The nice thing about StreamYard is it just did it by itself, and I'm
[12:41] taking notes over here off screen. Y'all can't see it. This is something I'm actually working on getting fixed. Uh, I ordered a tablet that I am hoping, we're
[12:54] gonna see when I get it, that next week, uh, that you'll be able to see my notes, um, having it as an additional screen from, on screen as well. So, you can see
[13:05] what I'm writing down, what notes, my way of thinking, because I know for myself, that's a big way that I've been able to pick up on better ways for myself to
[13:15] learn, has been other people's experience. So, we're gonna see if this works, but some things that I didn't know going into Postgres, there are a lot of options to
[13:26] install. We haven't even tried, like, Ivan. We're still just trying local, but there's a lot of options on which one to choose to download. And then also, uh,
[13:46] downloading different things that may not, like, make sense. And I know a lot of people that watch the show, yes, we definitely have a ton of beginners that
[13:59] come on and ask questions. There's a lot of people, and a lot of my friends, so thank you, that come to listen that have actually done this before, and they, they
[14:08] get it. They're like, yeah, done that a million times. Yet, one thing I feel like many people may forget is, it doesn't always make sense to somebody looking at
[14:20] it for the very first time. And that's something that I need to remember, and I'm working on taking the notes for. So, Stack Builder is something that I wasn't
[14:32] expecting. Well, that's cool. We're not doing enterprise. Ooh. Remote server. We're gonna click this one, and see if we can make this bigger. Okay. I will say
[14:54] one of the best parts of streaming is that it's recorded. So, if I forgot to write down something, fine. I can go back and look at it. Okay. I would think that
[15:14] if I do categories, it does it all. Nope. You gotta select at least one. Well, okay. Database server. Ooh, there are options. That one's installed. Okay, cool.
[15:38] Postgres database server with PgAdmin. Here. I guess I'm just gonna do that one, because I don't know what the rest of
[16:11] these necessarily mean. We don't need enterprise. That's cool. And we'll figure out the rest of them. If not, I'll go back. We are actually not gonna do that
[16:27] directory. Oh. That is a good thing to go fix. Well, BRB as I fix my Apple settings. And, bro nifty, I will get music going for next time. What up,
[17:05] Sebastian? Sebby? See, this is the weird thing. Sebby, why do you put your name like the full Sebastian everywhere when you go by Sebby? Makes me want to call
[17:19] you Sebby. Or Sebastian, all at the same time. Okay. CF. Ooh. Okay, cool. Desktop. Code. We are gonna do a new folder.
[17:48] [BLANK_AUDIO] [BLANK_AUDIO]
[18:08] [BLANK_AUDIO] [BLANK_AUDIO]
[18:28] [BLANK_AUDIO] [BLANK_AUDIO]
[18:48] [BLANK_AUDIO] [BLANK_AUDIO]
[19:08] [BLANK_AUDIO] [BLANK_AUDIO]
[19:28] [BLANK_AUDIO] [BLANK_AUDIO]
[19:58] [BLANK_AUDIO] [BLANK_AUDIO]
[20:28] [BLANK_AUDIO] [BLANK_AUDIO]
[20:48] [BLANK_AUDIO] [BLANK_AUDIO]
[21:18] [BLANK_AUDIO] [BLANK_AUDIO]
[21:38] [BLANK_AUDIO] [BLANK_AUDIO]
[21:58] [BLANK_AUDIO] [BLANK_AUDIO]
[22:28] [BLANK_AUDIO] [BLANK_AUDIO]
[22:58] [BLANK_AUDIO] [BLANK_AUDIO]
[23:18] [BLANK_AUDIO] [BLANK_AUDIO]
[23:48] [BLANK_AUDIO] [BLANK_AUDIO]
[24:18] [BLANK_AUDIO] [BLANK_AUDIO]
[24:48] [BLANK_AUDIO] [BLANK_AUDIO]
[25:08] [BLANK_AUDIO] >> I feel like I'm gonna start here.
[25:15] So let's go find some hyper. I guess we will do some updates.
[25:21] Yay. I do use hyper and they are great.
[25:30] Again, those are preferences. I personally just really like them because it makes it colorful and
[25:35] easier for me to read while I'm doing things. [MUSIC]
[25:45] What are they? Yay.
[25:53] I like when I can, oh yeah, that would help. No tab, I didn't hit the tab.
[25:59] [MUSIC] Okay, okay, so.
[26:20] So what I did and I'm checking out is we're looking at a, like how to connect to Postgres.
[26:34] Like that is my next thing. So in my mind, I'm like, okay, cool.
[26:39] I found this document that says that it's a thing. Here's how to go look at it.
[26:46] And that there was a help. And granted, I am not someone that's great at reading through every single line.
[26:54] I am definitely a scroller, see if I can figure it out. Watch videos, those types of things to work on figuring it out.
[27:04] And that is why I was going to go to the help first. Yeah, that didn't work.
[27:12] So I think I am definitely missing a step. Probably opening the connection.
[27:23] [MUSIC] Using the post, is that this one that I, the dollars?
[27:33] Well, the PSQL-U Postgres? I think.
[27:38] Yes. Okay, cool, yeah.
[27:40] Thanks, Abby. [MUSIC]
[27:47] [INAUDIBLE] Okay.
[27:58] [MUSIC] Hey.
[28:02] [MUSIC] Well.
[28:08] [MUSIC] Let's go back to see if, why are we not seeing?
[28:18] [MUSIC] Oh.
[28:27] So there's a different client. I did install some things.
[28:33] But we will, I will install that, Google that, install that. I will Google it too.
[28:44] Isn't that confusing though? Like I went to the Postgres site and, oh, I literally copied it.
[28:50] But hey. How'd she run?
[28:53] Now I want to install. [MUSIC]
[29:06] Oh, I installed the server, not the client. [MUSIC]
[29:12] So if I'm taking a look at this in my like to-do list. So to set up, part of the setup on local is install the server.
[29:24] And then install the client. [MUSIC]
[29:30] These are all things that are somewhat annoying to learn. [LAUGH]
[29:40] [MUSIC] Okay.
[29:45] [MUSIC] Okay, well, there we go.
[29:50] We got our brand installed. [MUSIC]
[29:56] I don't know why I cheated and put my hyper to just do, go to my default folder. So a lot of times.
[30:07] I'll make sure nothing else needs to be done. Oh, of course you do.
[30:11] Of course you do. There's so much.
[30:15] Brew update. So this is like a side quest to make sure you can install things with Homebrew.
[30:23] I will work on explaining those a little later. There is a lot to know to get even just at this point,
[30:32] especially if somebody doesn't have experience with Terminal. So please comment if this is something that you want to know more about,
[30:43] because I can definitely go into more of any of this. Yay, all the installing.
[31:06] Okay. Okay, and we may need compilers.
[31:15] Interesting. [MUSIC]
[31:48] And then finally semi-link pSQL and other libpq tools into user local bin. I did do something similar of this of how I set up my terminal to be able to go
[32:06] to my home folder. So I will be -- this part makes most sense to me doing it through the actual
[32:18] finder, I'm going to do that off screen really quick. [MUSIC]
[32:48] Okay. [MUSIC]
[33:29] Just kidding. I just realized I could have done that.
[33:36] And for some reason I was still thinking that I had to semi-link pSQL. If you need to have the -- well, we're going to put that pin in this one.
[33:50] See what happens. If something breaks, we'll find out.
[33:54] Okay. And just so that way everybody knows what I used, as Sebby said, Google it.
[34:09] This is the link I used for today. Okay.
[34:13] Yay. So we're going to go back to and -- what's that do?
[34:24] Oh, yay. It worked.
[34:35] Sweet. Look at that.
[34:37] We got Postgres up. This is exciting.
[34:46] Okay. Yay, yeah.
[34:50] Thanks, Sebby. Okay.
[34:56] So we are connected locally. That is progress.
[35:10] So we installed it. We are connected.
[35:43] Interesting. And there's also like create databases and such.
[36:10] I'm going to first actually make this a bit bigger. I don't think that's necessarily what I want, but we'll find out.
[36:42] Because -- Okay.
[37:03] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- Okay.
[37:12] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[37:46] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[37:55] Okay. I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:01] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:27] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[38:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[39:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[40:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[41:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[42:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[43:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[44:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[45:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[46:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[47:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[48:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[49:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[50:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[51:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[52:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[53:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[54:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[55:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[56:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[57:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[58:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[59:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:23] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:29] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:35] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:41] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:47] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:53] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[60:59] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[61:05] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[61:11] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- I'm going to do my own documentation because I feel like this is going to be complicated if I try to just --
[61:17] I'm going to do my own documentation because I feel like this is going to be complicated if I try to just -- [ sub by sk cn2 ]
[61:20] you 
