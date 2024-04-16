---
showLink: "https://www.youtube.com/watch?v=xoPuU1YONwY"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-how-to-setup-postgresql-pt-2-with-docker-pgadmin"
title: "Learning how to setup #postgresql pt 2 with Docker & pgAdmin"
publishDate: "2023-03-30"
coverImage: "https://i.ytimg.com/vi/xoPuU1YONwY/maxresdefault.jpg"
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

[00:00] (silence) Yay! Apparently, um, setting up the second camera because I was like, "Oh, do I want
[00:12] my normal camera? Or, like, my background?" And, yeah, there were, like, two voices or just two, like, yeah, like, look, look, there's, like, different sides. It's crazy! But when
[00:27] I was like, "Nah, I don't want to do that side. I want to do this side, the one in front of me." And, um, yeah. I guess I'm just really for all those non-makeup-y people, I'm still
[00:42] gonna show you. Because I feel like this is a perfect, uh, okay, let's see. No, we'll try this camera. Okay. It's called Gemini, and I'm a Gemini, so having the two on here
[00:57] isn't that just kind of fun? It's like, there's two of me, and I'm a Gemini. Okay, yes. Thank you for the call-out, and I am happy there is sound now. There is sound. There is sound.
[01:13] Yes. Thank you. I wonder, like, that is so funny. I'm really glad that you joined and said something, Josh, because I've been streaming for, like, 30 minutes. So, it's always good
[01:31] to check on your friends and see if they have audio when they're streaming, even if you can't hang out the entire time. So, yay. Okay, well, as a quick recap for everybody, but
[01:49] also for myself, so I can go back and look at this. And, Josh, this is exciting. I'll show you, Josh, because we can use this for our stream later this week. So, over here
[02:06] that my docker is blocking is, I have my iPad connected, and I have the book. And, okay, I'm trying to just go to, like, this page, and then I can zoom in all the way about just
[02:32] the part I'm talking about. And, like, let's say I want to go to a certain page. We'll just scroll down here. Like, I can favorite the chapters, which I should probably do,
[02:47] but, and that's chapter two. That's fine. But, then I can hit my little pencil and be like seven, and then circle these to not really used. Maybe used. Ah! Undo. Used. Yay! Dude,
[03:18] streaming is hard. Like, I have a lot of work to do, but I am so excited about having the tablet to show my notes. Like, this is a very, I feel like, I'm very excited about it. And,
[03:35] I'm hoping it shows people the type of notes that I take. And, the really, really cool thing is, is like, let's say, I have to, like, copy my notes over, but, like, let's say,
[03:57] okay. So, I put what, but it's in my handwriting, and that may be really hard to read because, you know, I can type it out, but what I've found that's faster, oh, no, I didn't get
[04:14] it all. There we go. We can go in, and we can convert it to text, and then it converts to text. And, then I can say convert it, and it does the font I want. I can style it, and
[04:28] I can make the font really big or really small. Okay. I got really excited about this with y'all here. This is what I'm, like, so excited about streaming now is having a tablet to
[04:42] do this. But, anyway, thanks for the side note of being able to show you that I can write on your book digitally instead of physically. Because, yeah, that's how I write notes, and
[04:59] now I can share them. Okay. Well, anyway. And, my Postgres pre-stream stuff is earlier on in stream, I shared a bunch of tags for people because Trevor was on the show earlier.
[05:20] It was super fun. This was back in, like, October. Oh, my gosh, you guys, I've been streaming for almost a year. This is mind blowing. And, Ben, I am so excited that you're
[05:32] streaming again. I saw a little bit of it yesterday. Yesterday was a rough day. So, I just didn't really do much yesterday. But, I liked how it was talking about, was it typography
[05:46] with multiple languages? And, I was, like, dude, this is actually really cool. But, I did not have the bandwidth. And, anybody else, I'm just, like, curious for all streamers
[06:00] or those in, like, the tech field, anyone else struggle with the fact that, like, hey, I'm going to, like, do all this tech stuff. It'd be cool to do, like, some, listen to
[06:14] some podcasts and continue learning them. And, I'm like, nah, bruh. I cannot just, like, consume anymore. I need to, like, just listen to The Secret Room, which just tells a bunch
[06:29] of people secrets or other random podcasts to keep my mind off of it. Ah, yes. Oh, I'm back. Oh, Ben, I have news for you, too. Oh, my gosh. Oh, my gosh. Ben, yo, I used ShowMyDotChat
[06:51] in OBS. I got a little overwhelmed with OBS and trying to use all of this. So, today, I just used DreamYard because it was easier. But, I do have it set up. So, if you go check
[07:06] out Postgres 1, I am using ShowMyDotChat. And, anyone that streams should use ShowMyDotChat so you see the chat in the window. And, I'm so glad you guys came today because I would
[07:23] have forgotten to tell you all this stuff that I was excited about to tell you. And, let's see. I am I'm just pulling up this video to show y'all. I'm not I won't show, like,
[07:38] the entire video because last week was a lot of me super struggle busting because I didn't even know where to start. Oh, this is one of the best parts about being a streamer is
[07:51] when you freeze frame yourself on the most awkward things. It's real. It is real. And, you kind of just get over it. Because it's going to happen. But, this little box right
[08:04] here is is ShowMyDotChat. Yeah. So, this is the first one I went with. I really liked it. But, I couldn't figure out the spacing. And, for some reason, the spacing being right
[08:18] next to the edge was driving me insane. So, if I go back to my channel, and we go to videos, and then I used it day two, maybe. I thought I did. Oh, yeah. There we go. I used a different
[08:41] one because I thought the spacing was a little better. I don't think anybody actually stayed around to chat much. There we go. So, I liked this one a bit only because the spacing wasn't
[08:54] driving me insane. Okay. Cool. But, y'all, go use ShowMyDotChat because it is so fun and really easy to set up. So, these are my examples. Okay. Enough with the YouTubes and
[09:10] getting excited because I haven't talked to you guys in a while. And, yeah. You support your friends. But, they don't always know you're supporting your friends if you don't
[09:18] tell them because they might not see it. Which is okay. Anyway. So, I am sharing my iPad, taking notes. Super cool. What I previously streamed with Trevor Sullivan who works for
[09:35] a company called CBT Nuggets which does streaming or learning and a bunch of trainings. And, he came on this stream and taught me about like the differences between or like a high
[09:49] level review of Kubernetes Docker and PowerShell. I really listened to it. It's still pretty confusing. But, one thing that he was saying at the end of it back in October, mind you,
[10:09] was you kind of just have to do it. You kind of just have to go set it up. And, I never did because I never really had a use case. And, that was actually something that I was
[10:17] talking about when I was on stream with him until today. And, today, I have a reason to go set up Docker. So, before the stream, I also signed up for a free Docker account.
[10:30] And, to do all of this, I realized with my audio not on, I went to pull this command and I didn't have a Docker. I didn't know what Docker was, which is totally fair. So,
[10:48] I was like, oh, okay. You probably have to go install it. And, I installed it with the Apple chip because work computer has an M1, which is exciting. And, this is basically
[11:00] where we got to of clicking through stuff because that's what I'm best at is just randomly clicking shit and seeing where I can figure things out to get there. So, that is a very
[11:14] quick update since the first 25 minutes of my stream had no audio. And, yeah. So, I'm going to stop this one. I'm guessing I don't really need those to be there. And, yeah.
[11:32] I'm just going to say, this is something that looks really, really scary, like TypeScript used to. Now TypeScript is starting to make sense. But, yay. I don't know if I love it
[11:54] or hate it yet. It's starting to make so much more sense with TypeScript. You were there on Friday when I tried to explain it, which was interesting. That was such a fun stream.
[12:09] For those who are curious, somehow we ended up with like ten people on stream while I was like learning to code. Okay. I wasn't learning to code. I was live coding and fixing
[12:20] things on my website, trying to get it up and ready. So, okay. If we have a repo here, we're going to create a repo. Okay. And, that's good. Here. And, again, I am doing what you're
[12:41] not supposed to do and probably drives Josh more than anyone insane. And, I say it that way because, Josh, you wrote a book on how to do things. And, yet, I still just kind
[12:52] of click things. Pro tip. You can push a new image to this repo using the CLI. Okay. Make sure to change the tag name to your desired repo. Okay. So, push a new tag to this repo.
[13:26] Then I saw in this setup that it had a CLI in here. Okay. That is not where I wanted to click. So, exit. I don't think it's volume. I'm just going to go here. Let's go here.
[13:52] Let's hit paste. And, we're going to rename it. Oh, I have to scroll all the way back. New repo. It helps if I have it all on the same. And, I realize by me doing this, it
[14:23] might be trying to just redo what I just created. That's what it's going to do. That's what I'm going to learn. Enter. An image does not exist locally with a tag new repo. Okay. Let's
[14:52] see. Can't be. Oh. Yay. Image does not. Push refers to repository. An image. I need to figure out what an image is. This is something that I feel like it's a lot harder to learn
[15:24] this stuff when you're not like learning it from someone. You're just learning it by yourself. So, let's write down some questions. We need a better font that people can see. Nope. Nope.
[15:47] I like that color. So, stream. Cool streams. And, I'm writing this down because I feel like if I don't understand something, I'm going to forget while I probably find out
[16:04] something else I don't understand. Which is kind of the fun of learning is you find a bunch of stuff that you don't understand. Okay. Just putting this over here so y'all
[16:16] can see it, too. What is an image? Or, also, what is an image? What did this call it? Oh, but it has something here. What is this? Oh, it's a tutorial. It's that, but it's here.
[16:53] It's an image. What? Okay. So, I think I know what a container is, but we're going to write it down. Thank you, Josh. Talk to you later. See you Friday. Okay. Cool. Let's make sure
[17:12] I write down. So, what is everybody else up to? Like, are you guys doing anything fun? Working on any fun projects? Images. Um. Okay. So, I think I'm going to go ahead and
[17:52] skip. Oh, fun. And this is going to be the weird thing of going back to StreamYard. Not everybody can see that, but I am just streaming to Twitch now, even though it can stream to
[18:11] both, because I'm like, I feel like I need to make sure people can see the chat. And if I do YouTube as well, that would be complicated. I have my skip level once a month. So, my
[18:25] skip level is on Monday. Yeah. And I'm excited for it, because it's always cool to hear, like, the big level stuff. Oh, there's also a hub. I think local and the hub is online.
[18:40] So, we should put that as something we knew. I don't know if this color is going to show up. Yeah. Give me another color. Oh, damn. Skip levels are yearly. I mean, that's fair.
[19:00] You also work for a much larger company than I do. We have... I don't know how many employees I have. I just know it's definitely not as big as yours. Okay. So, local is local computer.
[19:25] And then hub is Docker online. Hello, hello. And Ben is amazing. So, I do hope that you recognize them. And what up, Firefox? Hello, hello. Thank you for joining today, everyone,
[19:57] with my let's learn... Okay. Yeah. I'm like, it looks weird on the... I'm using my tablet to take notes. So, if y'all are like, yo, I can't see something, just let me know. I
[20:11] am working on setting up Postgres on Docker, which does seem to be the easier option. Last week I tried setting it up local and that was kind of a shit show. So, but to do this,
[20:27] I kind of need to learn what Docker is. And that's what I'm doing. Let's see. How to create an image. That one has an image. Tags. Read me. Builds. Nope. Tags. Okay. Let's find out
[21:05] what a Docker image is. Oh. Hey. I'm guessing this will... No. You started the container for this tutorial. Let's first explain the command you just ran in case you forgot. Here's
[21:30] the command. I don't think that's going to help me add an image. Let's see. I'm catching up on y'all. I was like not looking at the chat. Varda just finished a .NET course that
[21:54] included Docker. Yes. It seems like it will be easy once I kind of like figure my way around. And then Firefix. I mean, let's do it. Yes. You guys can see all the random shit
[22:09] that I've searched in here. Session has expired. I don't know if it's going to work. Log in. Log in with Google. Yes, you guys can see all that. That's fine. I got a lot of email
[22:22] addresses. I do have Docker desktop running. When I'm looking at it though... Go back over here. So, I created the repo on Docker Hub and local... It doesn't see it locally. It
[22:48] only sees... Docker push for the tag name that they gave me. The push refers to a repository. An image does not exist with the tag. As to me wondering, what is an image? Yeah, I don't
[23:11] know what an image is. So, I figured I should probably find that out. So, let's... Oh, by the way, y'all can like Google so much random stuff. Like Google Postgres. Postgres? Wow.
[23:25] Chat. Chat GPT. That's not as easy to say as like Google. You can GPT it? I don't know. Let's see what they say. What is a Docker image? What is it, bro? You guys read that
[23:51] okay? We can make this bigger. Let's see. Docker image is a lightweight standalone executable package that includes everything needed to run an application, including the code, system
[24:09] tools, libraries, and settings. Ooh. Yes. To both of you. Something that just made it click was I originally tried... Let's go back a file. Back a page. Or another one. Excuse
[24:32] me. Okay. You're not going to show it to me. Fine. Where like at the very beginning in it, it suggested a bunch of them. And I did Postgres, but the Postgres one didn't work
[24:48] because I did not have it yet. And this is what I used. Oh. Interesting. So... Hmm. Okay. I don't think this is going to fix it. Like just comparing to what you just posted. But
[25:35] okay. I don't know what just happened. And this is the very annoying thing that I love and hate, is I like just kind of figuring it out. Which is not always great. But did
[25:58] that put it in the right folder? I don't think so. Let's look at some folders. Unity code. Okay. I think it did. Maybe. Okay. Looking at what you said, and that does make sense,
[26:33] especially with like what they were saying here of like the Docker run. So I wonder if I do... Go into it. Make sure I know CD, Postgres one. And then I would think I would
[27:05] need to run it. But it wouldn't be getting started. Would it? Maybe. Hmm. Join five. Postgres. Unused. Hey. Hub. What are you doing? You just got the Docker tutorial. Okay. So...
[27:52] I think I got Postgres on there. Oh, okay. Docker. Oh, hey. I got an image. Okay. I'm done. Cool. Images. Oh, I got two images. Yay. Well, I guess I will run it. What happens?
[28:43] You're going to click it? Let me go back over here. Especially since I didn't have audio the first like while. This... Yes, I am still learning how to use my iPad to do this stuff.
[29:11] So please bear with me. This was what I was originally like... Hey, I am going to move this really quick. So you guys can see it without my face being in the way. This is
[29:25] what I was originally like... Hey, Jen, let's do some like how to set up videos. I was like... I got to know how to set that up. So last week I tried local. Let's just say it was
[29:40] a bit rocky. It was really rocky. And that's as far as I got in the entire like hour and a half I streamed of learning that I had to install the server and then I had to install
[29:56] the client. But to install the client, I also had to install something else for like Post SQL, PS SQL. And yeah, I was supposed to get to secure connection and I was like, no, that's
[30:13] going to be rough. And then also if we do the how to videos with those, then we need to specifically do it for each operating system. So other people suggested they were like and
[30:26] here is my really cool mind map of it. I've like set up Postgres of... Hey, if I do local, there's a reason nobody does it. So let's try Docker. Cool. And then eventually I will
[30:43] get to try an Ivan. Ivan is where I work and that is where I first set it up and it was the easiest. But I don't know if that's actually true. So that's why I'm trying the rest of
[30:57] these and Kubernetes is here just so that way I know it exists. And OK, let me get back on my note screen so you guys were able to see all this and then I will read what you
[31:08] put in the chat. OK. If you have to, if you have to configure a Docker file for port forwarding, file mounting and other stuff, you have to configure. Oh, yay. I'm so excited. I'll put
[31:31] that on the notes of things. You left set up notes in your project. You can share them if I'd like. That would be dope. That would be dope because I'm definitely learning them
[31:44] and I will put a bunch of... Let's do pink. And if any of these colors are difficult for y'all to see or you need me to move my note screen around, please let me know. And so
[32:03] I'm just going to put this. I'm putting your username, so actually remember if like, yo, who told me this? Because I have questions at some point. But configure Docker file for
[32:36] port forwarding. Yay. And file mounting. Oh, yay. This sounds so exciting. Oh, thank you. OK, cool. I will grab that info real quick. And as Varda Haas, is that how I say your
[33:08] name? I am not always great at like going through things, but I think it will help. So I will get back to you on that. Happy link address. Go to the link address, please. I'm
[33:27] doing it off of screen just now. Cool. I have access. Let's start it. So I remember it. I have started. Thank you. I will look into that. Let's put that on my to do list. And
[33:46] for those who may not have been here, like when Josh joined earlier, because I didn't know I had my audio off. That's a thing. There is a way that if you're like, Jen, how are
[33:59] you going to read your handwriting later on? I can actually go in and tell it to convert my handwriting. Like I have to like double check it, but then I can convert the section.
[34:11] Bam. But then I'm able to like go in and look at it later. But writing it out helps me remember it way faster. So if you're wondering why I'm writing it all, let's oh, I guess I have
[34:32] green up right now. There we go. Sweet. Put notes. Yay. Well, that's good. That's good. It was something that I don't know if anybody else ever had this as punishment growing up.
[34:54] My dad would like make me write sentences. It was rough. So, okay, there we go. Got that going. We got this doing something. And go back one. So I had in Postgres, let's go back
[35:14] to images. I saw Postgres. And I hit run. And there's optional settings. Okay. Yay. Sure. More things to learn. Oh, that is a fair statement. If you want to make your Postgres
[35:48] database work, read documentation of your Docker image. That is very fair. That is very fair. I should. You are 100% right. I am definitely that person that I click my way through it
[36:04] and break shit until I can't figure it out. And then I go read the documentation. Because the documentation doesn't really sink in if I try to read it the other way around. But
[36:13] also a big part of why I've learned to do it kind of vice versa, which can be very frustrating for other people, is I'm really, really dyslexic. So reading documentation is hard for me in
[36:27] general. And yes, I can use the text-to-speech. But that doesn't always work out very easily. That's a big reason why Josh comes on. Like, luckily I was able to set up learning TypeScript
[36:42] with Josh, who I was showing this a little earlier. I'll show it again. Like, we go through this book. Oh, you guys can't even see it. How rude of me. We go through his book together.
[36:57] And where I can actually take notes and ask him questions as, like, my own -- I'm going to the very beginning so you guys can see the book -- of, like, my own way of this is
[37:07] the best way that I learn things. Right now, since I just got the tablet, the notes aren't in there. But hang tight. It's actually going to be Friday's stream. It's going to be exciting.
[37:22] But there are -- which camera am I using? This one. Notes in my book that help and then going through it. So it's all kind of just, like, figuring out our own, like, learning
[37:37] styles. It's frustrating. I never knew my learning style before I started to stream. That was awkward. Learning while streaming. It's fun and also very nerve wracking. Okay.
[37:54] So I guess we're running this as a new container. And it gives me errors, which is probably good. Because it gives me something to look at. What? KevScript only took you two weeks
[38:11] to learn? Oh, I'm so jealous. So jelly. Josh would be so happy to see that. If you don't -- oh, I should just, like, do the shoutout. Okay. Hold on. We will -- because if you don't
[38:29] follow what Josh does in his streams, like, definitely something you guys should do. Okay. And copy. And paste. Yay! I dropped my pencil. So would highly, highly suggest following
[39:00] him in his content. Because he is on the -- what is it? Maintainer? He's one of the maintainers of some of the work they do. So super, super cool. Okay. Now back to this. Okay. Database
[39:22] is uninitiated and superuser password is not specified. Okay. Well, that is delightful. I will say this is a bit easier to understand than all the clients I was trying to do with
[39:41] the local setup. It's definitely -- it's definitely going to be difficult. But then it's okay. And if I get too exhausted or confused by doing this, then I can always switch over
[39:56] to working on my website. That is my default that I'm going back to. So that's a logs. And then we got inspect. Oh, interesting. Oh. Interesting. Okay. Oh, it does. And the
[40:29] container files. And it didn't because of that. Okay. Got it. There. Oh. Okay. Okay. Hmm. Database is uninitiated. Super must specify user and a nonempty value. For example
[41:17] -- well, what did I -- I think go back to images. Okay. There is one local. But -- okay. Yeah. Is it that space? All right. There. Oh, it just went to the original. Okay. Yeah.
[42:12] I got that. I'm also -- where I -- I guess I'm looking right now to like talk out loud of where I'm looking. I'm like, okay, cool. So I didn't set up my password. Let me go
[42:25] do that. But where I got a little stuck on was -- I'm going over here just because it's going to make a bit more sense for me to look from here. Is on my code folder, it set up
[42:48] like locally, it set up my Postgres 1. And it hasn't put it up to the hub. And I'm like, oh, cool. So I have two different areas that's saving content. And I'm like, so where is
[43:04] Docker saving stuff? Because if it's local, it had to go somewhere, right? Yeah. But where is it sharing locally? Yeah. I guess a better way of asking it is -- okay. So this is saying
[43:46] I have a local Postgres. And it's just called Postgres. But it's on in my code folder where I normally put things. So where did it go so I can update this Dockerfile? Okay. So
[44:13] let's see. Okay. Give me a second. We will share it on stream really quick. Right. Yeah. Right. You have the Dockerfile. But it's within your reactivities file. So basically what
[44:55] I'm trying to say that I'm a little lost is if this Postgres file folder is somewhere. Where's the project? Or do images not get projects? I think that's where I'm a little
[45:10] lost. Okay. Then... Funniness. Okay. So I'm going to go ahead and create a new project. Okay. That will make sense. But then how do I go into this Postgres to do the fix if I
[45:56] can't go into it here in my terminal? Or how do I go into it in my terminal? Because I can't run it because of the issue. I think that is where I'm like... Images are stored
[46:19] in the Docker desktop folder. But you can't access an image like a folder. You need to build container from that image. So would that mean that I need to delete this image
[46:35] to be able to start from scratch to be able to put a password in it? I'm going to get that. Well, I guess I should probably go back to my code folder. Or at least desktop folder.
[47:11] When I try to run this image, which this has been me just clicking stuff around. So that's why, as a heads up, I did miss something. But when I go into... Because both of these
[47:22] are executed. And then... Okay. We'll just run... Whatever. I don't have a password set up. So that's why I was like... Do I have to go into like a project or a folder to go
[47:40] set up a password so I can do that from terminal? Because I was like... Oh, let me go to terminal here. But you can't execute commands from here. Because I can't run the container. I'm
[47:57] glad you think so. My first time using Docker. Yay! I am glad that it is common enough that people are like... Yeah, dude. It's so easy. Okay. I'll get there. I will get there. Okay.
[48:24] So... Yes. Supported tags. File issues. Docs repo. Oh, this part. Okay. Oh... Okay. Okay. Wait. What? Good news, I haven't run anything yet. Ah. This one. Okay. Okay. Okay. Okay.
[49:19] I'll do it offline real quick, y'all. Okay. Okay. Okay. Okay. Okay. Okay. Okay. Okay. I honestly don't know. I feel like these are always the things that I'm like... Yeah, I'll
[49:53] set it to something. It's going to be exciting. Okay. Okay. Okay. Okay. Okay. Okay. Okay. Oh, whatever. I'll close it. If you guys really want to go through it, you can. It's not going
[50:39] to be that exciting. How do passwords set? Okay. I did run the command. I ran the command that was in here, not in just yet. Click on the containers. Okay. And then Varda Hoth,
[51:19] I will or in Firefox, I will look at the stuff you guys sent in just a second. Okay. Oh, there we go. Got it. Got in it. There we go. Yay. Okay. Teamwork, y'all. Teamwork. We got
[52:05] in it. We are running it. That was interesting. Oh, that's a good call. I like the names of them all. Yes. Believe forever. We're good. This one's running. Yay. Okay. Whatever. Yes,
[52:46] I totally get that. Click on the name. I'm glad that you kind of saw what I was like getting grumpy about because I'm like, why? Yay. Okay. Yes. Yes. And then terminal and
[53:04] you can make some magic. Yeah. We got this going. Okay. So we have it running. That is a start. And as a reminder, now that we have this running, which took a while, but hey,
[53:29] we got there, is there we go. Now I need to find out if I actually need to set up to something like PSQL, SQL. That is going to be. I have a to do list and we are making moves. Thank
[54:03] you all for your help. I didn't say thank you. So thank you. I appreciate it. So it's ready to connect to database system is ready to accept connections. Okay. Oh, that's a
[54:26] good way of understanding it. PgAdmin is just a GUI for Postgres. So. Okay. We'll use it to run SQL queries directly to the database. I feel like that's kind of like one of the
[54:53] confusing things of getting into like the database world is in my head. I'm like, I just want it to look like Excel. This is very naive of me, you could say, but it's definitely
[55:07] something I need to get over. Yeah. Oh, see, that is smart. That is smart. I have. Yeah. That's everything I'm going to be working on. I'm learning. Yeah. Yeah. I recently started
[55:34] working for a company called Ivan and they do have data infrastructure and it's really cool because I'm like, I get to learn about all of this. It gives my show a bit more of
[55:46] a focus. Yeah. At the same time. I'm just like, dude, I get video. I can talk to like anyone I got you. You want me to go do a talk? I can do. I got that. Understanding databases.
[55:58] So thank you. Thank you. I it's so fun. I've been there about a month and a half. So and I need to start making these videos and that means I need to learn more. Okay. One of the
[56:18] best parts in case anybody has ever thought about like starting a stream or wanting to learn live is you can it records it for you. So if you have questions about the work that
[56:30] you're doing, it's a lot easier to go back and it's, I don't know, not as awkward as if you learn by yourself, you're not always talking out loud about your processes where
[56:44] if you learn in life, you kind of have to explain to people what your thought process is and why you might be going a certain direction. And so if you need to figure out why you did
[56:54] something, you're saying it when you learn in life. It's a lot of fun and also very nerve wracking, especially when things just don't click. Okay. So we set this up. And one of
[57:18] the tools that I used last week, let me grab that really quick. Figure out what I did with it. Yay. Aha. I know I'm totally looking at a different screen. Hold on, y'all. Be there
[57:59] for a second. I might be able to see myself in there. I just need to be able to click. Okay. These directions that were sent, that I found last time is all for local from what
[58:33] I understood, but I feel like it gave a pretty good breakdown of like what you do with it afterwards. So I feel like I need to just look up setting up a Postgres. Doctor, what
[58:58] do you do with it? Oh, hey, they have three easy steps. Oh, we logged into chat GPT and now it's chat GPT. What it does. That's fun. Okay. Varda Hoth, you did a coding bootcamp
[59:18] five years ago and you did one hour whiteboard sessions talking through your thought process with something you had practice on. Oh, yeah. I guess perks of me being an only child. I
[59:31] don't know. Maybe I'm just like a weirdo, which is a hundred percent possible. I just talk out loud to myself a lot in general. My partner has walked in the room and I'm
[59:43] like singing something like, oh, I got my little cup. I got my little cup and now I need to go get some water. And he's just like, what are you doing? You singing to the cup?
[59:56] Yeah, yeah, yeah. I'm enjoying the cup. So, yeah. At least learning live was very similar. But like, what do you do with it after you set it up in Docker? That is a good way of
[60:20] saying it. Okay. I am scanning. Because that is. Start a Postgres instance. Database configuration. Okay. That was a lot of scrolling. So. And this is something that we have on next on
[60:56] the to do list was like users and permissions and things like that. But. Let's find out what is vSQL for. Frontend. Okay. I feel like I need to write this down. I'm going to forget.
[61:31] So, do, do, do. [silence]
[61:41] Is terminal... Um...
[61:51] [silence] [silence]
[62:01] [silence] Terminal...
[62:11] [silence] Um...
[62:21] [silence] [silence]
[62:31] [silence] [silence]
[62:41] [silence] [silence]
[62:51] [silence] [silence]
[63:01] [silence] [silence]
[63:11] [silence] [silence]
[63:21] [silence] [silence]
[63:31] [silence] [silence]
[63:41] [silence] [silence]
[63:51] [silence] [silence]
[64:01] [silence] [silence]
[64:11] [silence] [silence]
[64:21] [silence] [silence]
[64:31] [silence] [silence]
[64:41] [silence] [silence]
[64:51] [silence] [silence]
[65:01] [silence] [silence]
[65:11] [silence] [silence]
[65:21] [silence] [silence]
[65:31] [silence] [silence]
[65:41] [silence] [silence]
[65:51] [silence] That doesn't sound complicated whatsoever.
[66:01] [silence] [silence]
[66:11] [silence] [silence]
[66:21] [silence] [silence]
[66:31] [silence] [silence]
[66:41] [silence] [silence]
[66:51] [silence] [silence]
[67:01] [silence] [silence]
[67:11] [silence] [silence]
[67:21] Okay. [silence]
[67:31] Interesting. [silence]
[67:41] [silence] [silence]
[67:51] Interesting. So it looks like
[68:01] this is a container deployment.
[68:11] PGAdmin can be deployed in a container using the image at this. There are various tags you can select from to get a version that you want.
[68:21] Okay. More questions. [silence]
[68:31] [silence] [silence]
[68:41] [silence] [silence]
[68:51] [silence] [silence]
[69:01] [silence] [silence]
[69:11] [silence] [silence]
[69:21] [silence] Oh, I'm in.
[69:31] [silence] [silence]
[69:41] [silence] [silence]
[69:51] [silence] [silence]
[70:01] [silence] [silence]
[70:11] [silence] [silence]
[70:21] [silence] [silence]
[70:31] [silence] [silence]
[70:41] [silence] [silence]
[70:51] [silence] [silence]
[71:01] [silence] [silence]
[71:11] [silence] [silence]
[71:21] [silence] [silence]
[71:31] [silence] [silence]
[71:41] [silence] [silence]
[71:51] [silence] [silence]
[72:01] [silence] [silence]
[72:11] [silence] [silence]
[72:21] [silence] [silence]
[72:31] [silence] [silence]
[72:41] [silence] [silence]
[72:51] [silence] [silence]
[73:01] [silence] [silence]
[73:11] [silence] [silence]
[73:21] [silence] [silence]
[73:31] [silence] [silence]
[73:41] [silence] [silence]
[73:51] [silence] [silence]
[74:01] [silence] [silence]
[74:11] [silence] [silence]
[74:21] [silence] [silence]
[74:31] [silence] [silence]
[74:41] [silence] [silence]
[74:51] [silence] [silence]
[75:01] [silence] [silence]
[75:11] [silence] [silence]
[75:21] [silence] [silence]
[75:31] [silence] [silence]
[75:41] [silence] [silence]
[75:51] [silence] [silence]
[76:01] [silence] [silence]
[76:11] [silence] [silence]
[76:21] [silence] [silence]
[76:31] [silence] [silence]
[76:41] [silence] [silence]
[76:51] [silence] [silence]
[77:01] [silence] [silence]
[77:11] [silence] [silence]
[77:21] [silence] [silence]
[77:31] [silence] [silence]
[77:41] [silence] [silence]
[77:51] [silence] [silence]
[78:01] [silence] [silence]
[78:11] [silence] [silence]
[78:21] [silence] [silence]
[78:31] [silence] [silence]
[78:41] [silence] [silence]
[78:51] [silence] [silence]
[79:01] [silence] [silence]
[79:11] [silence] [silence]
[79:21] [silence] [silence]
[79:31] [silence] [silence]
[79:41] [silence] [silence]
[79:51] [silence] [silence]
[80:01] [silence] [silence]
[80:11] [silence] [silence]
[80:21] [silence] [silence]
[80:31] [silence] [silence]
[80:41] [silence] [silence]
[80:51] [silence] [silence]
[81:01] [silence] [silence]
[81:11] [silence] [silence]
[81:21] [silence] [silence]
[81:31] [silence] [silence]
[81:41] [silence] [silence]
[81:51] [silence] [silence]
[82:01] [silence] [silence]
[82:11] [silence] [silence]
[82:21] [silence] [silence]
[82:31] [silence] [silence]
[82:41] [silence] [silence]
[82:51] [silence] [silence]
[83:01] [silence] [silence]
[83:11] [silence] [silence]
[83:21] [silence] [silence]
[83:31] [silence] [silence]
[83:41] [silence] [silence]
[83:51] [silence] [silence]
[84:01] [silence] [silence]
[84:11] [silence] [silence]
[84:21] [silence] [silence]
[84:31] [silence] [silence]
[84:41] [silence] [silence]
[84:51] [silence] [silence]
[85:01] [silence] [silence]
[85:11] [silence] [silence]
[85:21] [silence] [silence]
[85:31] [silence] [silence]
[85:41] [silence] [silence]
[85:51] [silence] [silence]
[86:01] [silence] [silence]
[86:11] [silence] [silence]
[86:21] [silence] [silence]
[86:31] [silence] [silence]
[86:41] [silence] [silence]
[86:51] [silence] [silence]
[87:01] [silence] [silence]
[87:11] [silence] [silence]
[87:21] [silence] [silence]
[87:31] [silence] [silence]
[87:41] [silence] [silence]
[87:51] [silence] [silence]
[88:01] [silence] [silence]
[88:11] [silence] [silence]
[88:21] [silence] [silence]
[88:31] [silence] [silence]
[88:41] [silence] [silence]
[88:51] [silence] [silence]
[89:01] [silence] [silence]
[89:11] [silence] [silence]
[89:21] [silence] [silence]
[89:31] [silence] [silence]
[89:41] [silence] [silence]
[89:51] [silence] [silence]
[90:01] [silence] [silence]
[90:11] [silence] [silence]
[90:21] [silence] [silence]
[90:31] [silence] [silence]
[90:41] [silence] [silence]
[90:51] [silence] [silence]
[91:01] [silence] [silence]
[91:11] [silence] [silence]
[91:21] [silence] [silence]
[91:31] [silence] [silence]
[91:41] [silence] [silence]
[91:51] [silence] I'm seeing if it shows me, like, somewhere over here,
[92:01] like, what the port -- aha! Okay. So,
[92:11] run a new instance. So, when the container is
[92:21] running, I need to stop the container and rerun it. Is that what run a new instance means?
[92:31] [silence] Or restart it?
[92:41] [silence] We'll find out.
[92:51] Okay. Stop it. Change the command to run it, and run it then.
[93:01] [silence] [silence]
[93:11] Okay. Okay. So, it's
[93:21] Docker...yes, y'all, I don't remember what it was, and I should have written it down. That would have been happy.
[93:31] Docker run. Okay. [silence]
[93:41] To set up Docker with Postgres, I use command name...
[93:51] ow. Okay. run Docker.
[94:01] Let's just set the password. Nope.
[94:11] No, that's pull it, not run it. I had it there. Oh, great. Yay.
[94:21] No. I'm just gonna try that one. No. Oh, well, that's why.
[94:31] Y'all, if you hack this stuff, enjoy.
[94:41] It's not gonna have anything cool in it. This is it, right? It just had the dollar sign in front of it.
[94:51] No. Grand. Okay.
[95:01] [silence] Okay, cool. It's all there. We got it.
[95:11] [silence] After password.
[95:20] [silence] [silence]
[95:30] [silence] [silence]
[95:40] [silence] [silence]
[95:50] [silence] [silence]
[96:00] No. Okay. Oh.
[96:10] [silence] I wasn't kidding when I said I was dyslexic.
[96:20] FYI. I annoy myself sometimes.
[96:30] It's fun. And then, does it need the username? If so, where would I be putting it? Would it just be
[96:40] Postgres user at the very end? Or this should work.
[96:50] Who didn't hit enter? Hey.
[97:00] [silence] Rename some Postgres
[97:10] container. You have to remove and rename that container. [silence]
[97:20] So, essentially, I just delete it. I read that one right. That is exciting.
[97:30] [silence] [silence]
[97:40] Oh. Well, I like clicking things so we can leave it and then if I need to I'll go back and rerun it.
[97:50] [silence] Find address already in use. It's created.
[98:00] And then, here? No. Okay. Oh. No. Never mind. Go away.
[98:10] [silence] Yes.
[98:20] [silence] [silence]
[98:30] [silence] [silence]
[98:40] Oh. Actually, good call out. Because that's what I was working on last week.
[98:50] [silence] [silence]
[99:00] Give me a second. I'm trying to think. [silence]
[99:10] Okay. Hold on. [silence]
[99:20] Yeah. [silence]
[99:30] Let's make this bigger. [silence]
[99:40] [silence] [silence]
[99:50] [silence] [silence]
[100:00] Well. Yeah.
[100:10] [silence] Okay. Hold on. I will go delete it.
[100:20] And yes, I'm going like the old school way. Or the not new way. I think it is because I tried setting up
[100:30] a Postgres instance last week locally. And so it would make sense that it would be showing now.
[100:40] [silence] Give me a second and I'll rerun this after I delete it.
[100:50] Oh. Well, I can rename it though. Can't I?
[101:00] [silence] [silence]
[101:10] [silence] [silence]
[101:20] [silence] [silence]
[101:30] [silence] [silence]
[101:40] [silence] [silence]
[101:50] [silence] [silence]
[102:00] [silence] [silence]
[102:10] [silence] [silence]
[102:20] At least I have a cool -- they give us cool names.
[102:30] Heuristic Blackburn. And a lot of people --
[102:40] I don't know. If nstat is a command.
[102:50] [silence] [silence]
[103:00] [silence] [silence]
[103:10] [silence] [silence]
[103:20] [silence] Oh, y'all are funny.
[103:30] I dig it. I feel like also something that's interesting is I'm going into my library and
[103:40] it's also not seeing that, which is annoying.
[103:50] [silence] [silence]
[104:00] That is so funny. So I actually have dual monitors.
[104:10] So it is at least fixed now. [silence]
[104:20] [silence] [silence]
[104:30] [silence] [silence]
[104:40] [silence] [silence]
[104:50] [silence] [silence]
[105:00] [silence] [silence]
[105:10] [silence] [silence]
[105:20] [silence] [silence]
[105:30] [silence] [silence]
[105:40] [silence] [silence]
[105:50] [silence] [silence]
[106:00] [silence] [silence]
[106:10] [silence] [silence]
[106:20] [silence] [silence]
[106:30] [silence] [silence]
[106:40] [silence] [silence]
[106:50] [silence] [silence]
[107:00] [silence] [silence]
[107:10] [silence] [silence]
[107:20] [silence] [silence]
[107:30] [silence] [silence]
[107:40] [silence] [silence]
[107:50] [silence] [silence]
[108:00] [silence] [silence]
[108:10] [silence] [silence]
[108:20] [silence] [silence]
[108:30] [silence] [silence]
[108:40] [silence] [silence]
[108:50] [silence] [silence]
[109:00] [silence] Just in time. Goodnight fire. Thank you for joining and hanging out.
[109:08] And I think you already do, but make sure you follow and come back and hang out with us. This was fun and I appreciate it.
[109:18] And y'all, I gotta, before I forget, I got told that I'm going to get food on the way home.
[109:28] My partner is going to be late coming home, which is fine, but said, order food. They'll pick it up on the way home, which is exciting.
[109:38] So please stand by. I have to order quickly. [humming]
[109:48] [humming] [humming]
[109:58] Reorder. Release.
[110:08] [inaudible] [inaudible]
[110:18] [inaudible] The perks of always ordering the same thing
[110:28] is I just had to hit reorder and it knew exactly what food I wanted. Okay, I need to put my desk to standing because I've been sitting for a while.
[110:38] So please stand by. Yay for standing desks. And for those who may not know, these are things I'm definitely
[110:48] not used to having that are huge things that are very, very helpful in streaming, but then also
[110:58] just my work in general. But these are definitely perks that I've worked hard for. But it feels weird yet knowing that maybe not everybody can have the same
[111:08] things, I guess is the way I'm saying it. Anyway, okay, and that's not working.
[111:18] That is the thing. [inaudible]
[111:28] [inaudible] That's fair.
[111:38] It's true. It is true. There are many, many DevOps people that I very much so appreciate.
[111:48] Oh, it did something. Or it didn't do something and didn't give me an error. So let me go up a million times and then rerun this.
[111:58] Right? Or am I just trying to do, rerun this? All right.
[112:08] I'm going to delete you. [inaudible]
[112:18] [inaudible] Invoking remote Docker start container error.
[112:28] It's not available. Okay.
[112:38] Hold on. Go back down. Go all the way down.
[112:48] Okay. Do you want it to work now?
[112:58] I'm going to try deleting it and rerunning it just to see
[113:08] the Docker container. Okay, fine. Hold on. I'm going to go up a million.
[113:18] [inaudible] God damn it. Okay. So remove this, rerun it.
[113:28] Okay. And it is running.
[113:38] Y'all, we got it running. Now, let's see if I can get this. I'm just going to click out of it.
[113:48] That's where we're going, right? The PG.
[113:58] I'm going to copy this because I don't feel like retyping it. So we're going to close this. Because it doesn't let me resave. I mean, I can try to reset.
[114:08] Yeah, it does the same thing. Okay, we'll reset it. I'm going to name you PG.
[114:18] [inaudible] Port 443 because we updated the port in the last one.
[114:28] [inaudible] Hmm.
[114:38] [inaudible] [inaudible]
[114:48] [inaudible] Hmm.
[114:58] [inaudible] [inaudible]
[115:08] [inaudible] [inaudible]
[115:18] Okay. Maintenance database. I'm just going to update the full username.
[115:28] It's not giving me that error, but you know. It doesn't like anything.
[115:38] [inaudible] Okay. There you go.
[115:48] That is my Docker desktop. Hold on. Let me move this down some. Move this up some.
[115:58] [inaudible] No, that is definitely not what's supposed to happen.
[116:08] Give me just a second. I'm just going to. I think it's what.
[116:18] [inaudible] I get that it's supposed to be by default by admin, but if I change something,
[116:28] then at least we can make sure this didn't. I get we may not need it now.
[116:38] It's probably. Okay. Whatever. That's fine. [inaudible]
[116:48] Oh, okay. Go to your terminal and enter Docker inspect.
[116:58] [inaudible] [inaudible]
[117:08] Oh, goodness gracious. It shows the port correctly.
[117:18] I don't know how far this goes up. Okay. Stop. Tell me where to stop. [inaudible]
[117:28] There's a lot here. Okay. I'm going to stop with config.
[117:38] And then let me know if you need me to keep going. The IP address. Okay. Let me see if I see it. And then if not network settings.
[117:48] Bridge port. Oh, host IP is zeros. For the port. So just update that to zeros maybe.
[117:58] [inaudible] Keep going down. Okay. Oh, no. Gateway.
[118:10] [inaudible] Let me know if you.
[118:27] [inaudible] Save.
[118:37] [inaudible] Kept saying that it was hello.
[118:47] So fine. Be hello. [inaudible]
[118:57] Oh, Jesus. Okay. This isn't it. This isn't it. Let me steal this.
[119:07] I don't think you're going to copy and paste, but if you do. Oh, yeah, you did. [inaudible]
[119:17] [inaudible] I'm doing this one, right?
[119:27] The IP address 172.17.0.12. Okay. Data password. Okay.
[119:37] Oh, fabulous. Thanks. Okay.
[119:47] Well, yay. At least it's a new error, right? [inaudible]
[120:09] Okay, fine. I will delete you. Please stop and.
[120:21] Delete forever. Rerun.
[120:25] Okay. Hey, we are running.
[120:30] And we're going to just reject this. Just in case.
[120:37] And we're going to hit save. No, it's not.
[120:48] Okay. Literally is what I put.
[120:55] Copy you. And paste.
[121:03] Okay. I think it showed it in here.
[121:21] Status, status. Name.
[121:46] That's a username. Okay. Please be my friend.
[121:54] Please be my friend. Jesus.
[121:58] Never. We did it.
[122:02] Yay. Thank you.
[122:09] Yay. Oh.
[122:21] Oh, I like this. I like this a lot.
[122:24] Okay. And.
[122:36] Oh, I've got to end the stream soon anyway the dog is like, dragging me insane to go out. But, hey, we got it connected we got to step two, which was a little crazy. Because, okay, so we got steps to next, next stream when I work on this.
[123:06] How long did I. Did I try it. Did I try it. Did you try it. Did I try it.
[123:26] Well, this, this part of the process, locally, took like an hour and a half, and I did not get it connected properly. Well I think I did but I'm not entirely sure and it was a really hot mess. And it didn't make enough sense.
[123:32] So that when I ended really early. Thank you for the thank you and thank you for the follow is, it's definitely something that I love. This is group participation and learning.
[123:49] Oh, that is very true that is very true. Are y'all on Twitter like I'll tag you when I go live next or you're at least going to see what happens with the adventure. But, yeah, this is a, we will put that on my to do list of.
[124:15] So I'll just. Yay.
[124:20] I don't want brown anymore. Colors.
[124:28] Trucker. We'll go with coral.
[124:36] We'll go with coral. Yay.
[125:00] We're going to talk about like drawing so you guys will get fancy things that way. Yay. Well, hit me up.
[125:10] Oh, I can give you guys the discord and I'm going to stop sharing my screen though because just like looking at that thing is. Nope, nope, nope. I want this one. Yay.
[125:26] Where's my discord. There we go.
[125:37] I thought I would copy it. There you go.
[125:44] Add me and I'm totally gonna put you in a group chat. Um, it is something that a lot of people have been like john do you have discord and I'm like, Hmm.
[125:54] Yes, enjoy your time. Thank you all for joining. I'm gonna see. Oh, hey, because of y'all, we hit followers.
[126:06] And I'm going to see if there is anybody to read to. That's cool. So if you guys feel like you know, sticking around you at least get somebody cool to watch but I don't think I follow anybody that's streaming right now.
[126:20] Oh, but there's a remix react full stacked with somebody named dollar dojo. They sound fun.
[126:30] Right, we're gonna follow them. And if y'all feel like hanging out so I'm gonna read you over there.
[126:38] That sounds fun. Maybe, maybe I will.
[126:43] I always feel like it's hard to tell if somebody has their rates on or not. Yay.
[126:57] Do you do because we gotta wait for ready to raid. I don't know how people multitask this and do it. Okay, bye. Bye.
[127:07] Bye. Bye.
[127:09] [BLANK_AUDIO] 
