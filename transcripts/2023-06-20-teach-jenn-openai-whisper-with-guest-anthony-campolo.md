---
showLink: "https://www.youtube.com/watch?v=O4yrFmySAI4"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-openai-whisper-with-guest-anthony-campolo"
title: "Teach Jenn OpenAI Whisper with guest Anthony Campolo 🎥✨"
publishDate: "2023-06-20"
coverImage: "https://i.ytimg.com/vi/O4yrFmySAI4/maxresdefault.jpg"
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

[00:00] to another episode of Teach Gen Tech with my internet big brother, Anthony.
[00:05] Hi. - Hello. - What's up? - How's it going?
[00:07] - Happy to be here. I shaved this time,
[00:09] so I look like a hobo on the "Docker" episode. (both laughing)
[00:13] - Well, good, good. Good for you.
[00:15] What have you been up to lately? Who are you?
[00:18] Because I know you, but everybody else doesn't know you. - Yeah, so I am a developer advocate at Edgio,
[00:26] which is a deployment platform. I say it's like a combination of Netlify and Cloudflare.
[00:34] We have the power of Cloudflare, but the DX of Netlify is what I like to say.
[00:38] And yeah, I have been on this stream, I think this will be my fifth time.
[00:44] If you count that one time, we tried to install a bunch of stuff, but didn't,
[00:47] 'cause there was the Vercel episode, the "Set Up Your CLI" episode,
[00:51] the "Read Me, Driven Development" episode, and then the "Docker" episode.
[00:55] So now we got five in the can. - Yeah, yeah, that sounds about right.
[00:59] That does sound about... I feel like we need to plan for July 5th,
[01:05] like if you're available. - What, your anniversary? - Yeah, be like, "Hey, we streamed a year ago today."
[01:11] But I'm like, at the same time, I'm like, "Eh." I, mm-hmm, it'll work out.
[01:15] - We could do a watch party of our own stream. - Oh, it just sounds so cringy to think about like what...
[01:22] - You'll see how far you've come in a year, like way farther than most people.
[01:29] - Oh, geez. That's because I have people like you and Jacob
[01:32] that go, "Yeah, you could do better." (laughing)
[01:37] - Blame it on you. - It's good to have people who can help you accelerate.
[01:41] - It is, it is, and y'all have, and I appreciate it. Okay, so what are we learning about today?
[01:50] - Yeah, I'm not sure how this came up, but we were talking on a very recent stream
[01:55] about transcriptions, and I had mentioned that I've been playing around with OpenAI's Whisper model,
[02:02] and this is like a tiny sliver of a much larger story that's happening right now with AI.
[02:09] So we can kind of zoom in on a couple different levels here. The main thing is that there's this company called OpenAI,
[02:15] which most people know of now because of ChatGPT, which is this chatbot that is smarter
[02:20] than any of your college professors. It's a very strange experience to talk to a robot
[02:25] that is so freakishly intelligent. It makes stuff up every now and then,
[02:28] and that's kind of what a lot of people are- - I was gonna say, it might lie to you.
[02:31] It might lie to you, but it is pretty smart. - Never lied to you?
[02:35] - Yeah, but you at least can blame them and get away with it.
[02:40] ChatGPT, not so much. - Well, I mean, so I look at it this way.
[02:44] ChatGPT guaranteed will lie to you somewhere between, I would say like one and 10% of the time,
[02:49] depending on what you're doing and what you're kind of asking it.
[02:52] Some people will lie to you 100% of the time though. - This is true, this is true.
[02:57] And for y'all that aren't aware or never used the ChatGPT, I like to say the chat
[03:05] because apparently it's a millennial thing and I'm just gonna embrace it.
[03:10] That's what's gonna happen. - Yeah, I add that to lots of things,
[03:13] but me and Scott call it homie GPT. - Homie GPT?
[03:17] - 'Cause it's the homie. It does all our work for us.
[03:20] - All right, so we can ask it, ooh, and what is- - Make sure to switch to GPT-4.
[03:28] - Oh, yes. So if you want to go check this out,
[03:33] I'm actually paying for my ChatGPT because I'm needy and I need responses right away.
[03:39] So- - And GPT-4 gives significantly better answers.
[03:43] Like it actually does make a difference. - I wanted to ask it, what is AI?
[03:51] It's giving me a very long answer. So I'm gonna say, explain in one sentence.
[03:59] - What I like to say is I say, write that again, but make it half as long.
[04:02] That's one thing I do. Explain in one sentence is good too, though.
[04:06] This is how you can tell you've been using this thing for a while because a lot of people don't understand
[04:13] that when you get a response from ChatGPT, you can ask it to make the response better.
[04:17] So people just ask it and they get a response back and like, this response kind of sucks.
[04:22] ChatGPT sucks. I'm never gonna use this thing again.
[04:25] And it's like, you gotta work with it. - It's just like a conversation.
[04:31] If Anthony is not gonna tell me the answer, I have to ask seven different ways to be like,
[04:35] tell me the damn answer. Just kidding.
[04:38] But artificial intelligence, AI, is a field of computer science dedicated
[04:44] to creating machines that mimic human intelligence, such as problem solving, learning,
[04:49] and language understanding. - Yeah, and that's pretty good.
[04:53] And that's not like, and the important thing here is that if you were to look up,
[04:58] like if you were to Google define AI, it would give you a dictionary definition.
[05:03] And that would not be this exact wording. This is not, it didn't go to a dictionary
[05:07] and look up a definition and then hand you the definition written in a dictionary.
[05:11] It actually wrote its own definition to define it. - Yes, and the Google answer is.
[05:19] - AI is artificial intelligence. - Yeah, that's sort of-
[05:23] - This shows actually how ChatGPT understood, you were asking for a definition of AI,
[05:27] not what it's an acronym for, and Google did not. So this shows right now how on the first response,
[05:34] you got a more complete and comprehensive answer from ChatGPT than you did from Google.
[05:40] Now this one's gonna be interesting 'cause this might be too new.
[05:43] - Yeah, it's too new. - It's too new.
[05:46] So this is the perennial problem with ChatGPT that you can't ask it questions about things invented
[05:51] after September, 2021. - It's annoying.
[05:55] - Very frustrating, but something you could do instead is you could take the blog post about Whisper AI,
[06:03] copy paste it and say, summarize this article. And then it would write you a summary of what Whisper AI is
[06:07] by being prompted with the blog article. You don't need to necessarily do that right now.
[06:12] - If it's not too many characters. - Yes, it could take a lot.
[06:16] It could take, I think, up to at least a thousand words, so. - 4,000 characters.
[06:22] I may or may not have messed with this a bit too much to know that.
[06:27] - I summarize articles every single week for my newsletter using ChatGPT.
[06:31] If you read javascriptjam.com, there's always a story of the week
[06:35] that's usually 90% written by ChatGPT. - I like it.
[06:39] I like it. I use ChatGPT a lot for ways to start things.
[06:45] And if you check out the video I did with Josh Goldberg a while back,
[06:51] we took a look on how to create talk information, which I need to go work on later.
[06:59] But, yay. - Yeah, there's all sorts of,
[07:01] lots of little things it can do. I mean, there's, I feel like people get really hung up
[07:07] on what you can't do with it. And like really harp on its limitations.
[07:11] And like, it's important to know what those are. Once you know what those are,
[07:15] you avoid those or mitigate those and find the things it actually can do.
[07:19] 'Cause the things it can do is actually quite striking if you kind of get into it.
[07:22] You're thinking about the sum total of every little task you do in your day-to-day, you know?
[07:27] So I think, I say like, pay attention to what AI can do
[07:30] more than what it can't do. After you learn what it can't do,
[07:33] that's really all you need to know. Just move on, understand that the models will get better
[07:38] and things it can't do now, it may be able to do in the future,
[07:40] but you shouldn't worry about that. You should worry about what it can do today.
[07:44] So-- - But Anthony.
[07:46] - Yes. - Won't AI take our jobs?
[07:49] - I mean, so many people, this is a pat phrase by now, but people say, "AI won't take your job."
[07:57] A person with AI might though, so. - Oh.
[08:02] Isn't it gonna like become and take over the world and make it really scary to live here?
[08:09] - Um, this is a great question actually. This is what got me into AI back in 2015
[08:13] is what's called the AI safety problem. Which is, will AI, it's called the AI safety problem
[08:20] or the alignment problem, there's a couple different terms for it.
[08:22] Basically, will AI, once it's smarter than humans, decide to kill us all or create a utopia?
[08:29] 'Cause it has to do one or the other. For some reason, that has to do with math.
[08:34] That they won't explain to you. (laughs)
[08:38] - And what up, Brian and Laura? Hello, Laura.
[08:41] Hello, Ryan. Only one or the other, not, you know.
[08:46] - And I'm being ironic there because there's this term called the singularity.
[08:53] And the idea with the singularity is that once you build something smarter than yourself,
[08:58] by definition, you're unable to predict the future because you can't know what it's going to do
[09:04] if it's smarter than you 'cause you don't actually have the ability
[09:07] to understand its mental model. So there's, what's this term of like understanding
[09:14] that other people have like independent consciousness from you?
[09:17] There's this theory of mind. Like we can't have a theory of mind
[09:22] about a thing that is smarter than us because by definition, it's beyond us.
[09:27] So by that definition, we can't say whether it's gonna kill us all
[09:31] or that it's gonna build a utopia definitively one way or the other,
[09:35] or that might do something totally in the middle, or it might just decide to leave.
[09:39] Like that's what happens in "Her" if you've ever seen that movie.
[09:41] So the people who worry about this worry because the fact that we cannot,
[09:47] by definition, predict what's going to happen, we can't say for sure that it won't kill us all.
[09:53] So it might decide to kill us all and we won't be able to prove that it won't,
[09:59] but it doesn't mean it guaranteed will kill us all. It just means it might.
[10:03] So that's why people are kind of super worried about it. - Laura, you gave me my first,
[10:12] I had to approve your message. That was fun.
[10:16] Yeah, yeah. And that is the downfall of AI
[10:22] is it could make a lot of systemic issues that we already have worse.
[10:28] - Yeah, and this is a good point from Laura is that part of the alignment problem
[10:32] isn't necessarily align it so it doesn't kill us all, it's align it with actual good morals and ethics
[10:39] and actually understand how to treat humans fairly. And it's hard to actually define that mathematically
[10:47] and in a guaranteed way. So that's why these models have to constantly be watched
[10:52] and double-checked by humans and corrected and slowly made less and less racist.
[10:58] So yeah. - And yes, Laura, I know because we already have our,
[11:06] what is it called when the face detection? There we go.
[11:13] And those types of things. There are a lot of things in technology already
[11:17] that is not just AI that already has racist issues. And so with Whisper, explain Whisper.
[11:27] - Yeah, so Whisper is a transcription model. So a lot of the current issues we're talking about
[11:36] aren't really that pressing here because you don't have to worry about it
[11:40] hallucinating something and you don't have to worry about using it to decide how long someone
[11:46] presses a sentence is gonna be. Like those are the things where all these societal issues
[11:50] start to come in. This is, you give it text and it outputs,
[11:53] you give it audio and it outputs text from that audio. So there is some issues in the sense that
[11:59] it's gonna be better at English than other languages 'cause it's trained overall on English data
[12:05] and certain types of voices. So I shouldn't say that that doesn't entirely
[12:08] come into play here. I'm saying that it's a different set of issues.
[12:12] These things are always gonna come into play. But for what you're doing,
[12:17] you're someone who is recording audio with nice microphones for the most part, and you speak English,
[12:24] and you are someone who will be able to benefit from this technology, thankfully.
[12:29] So that's an example where you are going to be kind of on the cutting edge here
[12:35] in terms of understanding what you can do with these models. Now, this isn't necessarily to say
[12:41] that you can't do really nice transcription with the current tech, but you have to pay for it usually.
[12:48] Like if you're using something like Descript, like Descript's expensive.
[12:51] So if you want to be able to transcribe a lot of audio and have it be very accurate and very fast,
[12:58] you usually have to pay a bunch of money. Whereas I'm gonna show you how to do this
[13:02] entirely with open source models. - I'm looking forward to it.
[13:07] And this is also what got us to where we're at is for those who've been hanging out for a minute,
[13:14] know that I've been working on getting my website back up and running and automating some shit
[13:19] because I can't do it as a one person show. And so that's where the transcript came in.
[13:26] And also we may be working on this a little bit later in the stream, if we have time, we'll find out.
[13:33] Okay, so. - So we should not talk about anything else
[13:37] until we start running a command. 'Cause this command I think is gonna take
[13:40] at least five minutes, if not longer. So we should run this.
[13:44] And then while it's running in the background, continue on with our conversation.
[13:48] 'Cause part of what I'm showing you here is that there's gonna be a way to do this in Python
[13:51] and a way to do this in C++. And the way to do it in C++ is a little more complicated,
[13:56] but that's because it's gonna be way faster. It's gonna take like 10 seconds instead of five minutes
[14:00] to transcribe a minute of audio. - Okay, I'm glad Laura's around
[14:05] because she's like the Python queen. - Yeah, we're doing Python today.
[14:10] I learned how to install something with Python specifically to do this.
[14:14] - Okay, okay, so I will share my screen. And then let me share this gist.
[14:21] Throw this up on the screen just very quickly. - Yeah, I'm going to the one that is not,
[14:30] because if I try to copy and paste it, it doesn't want to. But if I do it here, it will.
[14:35] There we go. Ta-da!
[14:38] - Yeah. Great, so if you scroll down a little bit,
[14:43] we've already done some of these steps. So keep going down to where the commands start.
[14:52] - We've done all of this, except this bottom one. - Yeah, so you installed FFmpeg.
[15:00] That's a tool that's gonna allow us to convert because for the Whisper model, it needs to be in WAV format.
[15:07] So you need something, a tool that can convert things from like MP3s to WAVs or whatever kind of file you have.
[15:14] So that's why I'm giving you FFmpeg here. And then with Python, we installed the OpenAI Whisper.
[15:22] So let's go up to the very first section and the third command here.
[15:28] - This one. - Yeah, so with this, there's,
[15:32] and you see I have a comment written there. That's because there's a couple different sized models here.
[15:39] There's like the tiny, base, small, medium, large, and then large V2.
[15:44] Basically, the larger the model is, the more accurate it is, but the longer it takes to transcribe.
[15:49] So I don't want to sacrifice any quality of transcription because it already is not gonna be 100% accurate.
[15:58] So I want it to be as close to 100% accurate as possible. So I'm always gonna go with the largest possible model
[16:03] they can give me 'cause that's gonna be the most accurate. The problem is that means it would take me like four hours
[16:08] to transcribe like an hour long podcast, or actually even longer than that,
[16:12] probably five or six or seven hours. So it is frustrating from that respect.
[16:19] Now, I gave you a one minute audio clip. Do you have that on your computer?
[16:23] - Yes, yes. - Yeah, so you're gonna have to run that command
[16:26] in whatever directory has that file. - Give me a second 'cause I'm gonna move the file actually.
[16:36] - Yeah, I would just drop it, plop it right in your code folder
[16:38] if that's where you're currently, your terminal is right now.
[16:42] - That is, yay. - Yeah, I can see 'cause it says code on here.
[16:47] - But should I put it in code? Well, yeah, because it does show there.
[16:50] Okay, cool, convert. - Let's actually, let's do this.
[16:53] Let's make a directory called whisper in your code folder, and then let's do everything in there.
[17:00] - Okay, 'cause there's a whisper.cpp in here. I'll show you guys.
[17:05] You guys can see my folder structure. So we'll do a new folder and call it AI Whisper.
[17:13] Whisper, we're doing it that way since there's a whisper one already in there.
[17:19] - Yeah, cool. - And copy this after I go into that folder.
[17:26] - So not that command. So go into this folder. - Don't want to go
[17:31] into this folder. - Do go into this folder,
[17:34] but the command you copied is not the right command. So scroll up.
[17:39] So I want, so this is, so that's all the whisper ccp, cpps.
[17:43] So first I want to show the Python one. - Oh, okay.
[17:47] - Yeah, exactly, yeah. So grab that Python command.
[17:49] So you've already done that. You already did brew ffmpeg,
[17:52] and you already did the pip install, I believe. So you can skip those ones.
[17:56] So you're grabbing, exactly, yeah. And then just delete that stuff after the hashtag.
[18:02] - Now I'm curious. - I'm curious.
[18:05] - I don't. - Okay, so.
[18:12] - Yeah, I didn't like it because I had all this stuff in there.
[18:15] - Yeah, yeah. So let's see, that should, hopefully that'll work.
[18:20] - No. - Okay, so run the command right above it again
[18:26] and make sure you actually installed it. - Yeah.
[18:30] - Okay, and now try the other one again. Just bump up.
[18:40] You can just go up on your keyboard in the terminal. - Yeah, I'm like, I thought I was clicked in the terminal.
[18:46] I wasn't. Yeah, it's that one.
[18:48] There we go. - Okay, so you have an issue with your Python.
[18:57] Python, come on, we can be friends. - So I would have no idea how to fix this.
[19:03] So I would copy paste that whole error into chat GPT and ask it to fix it unless Laura knows what to do.
[19:08] 'Cause it looks like it's something to do with your version of Python.
[19:22] It's saying, is this example on purpose? It says URL lib3 version two only supports open SSL 1.1.1,
[19:32] currently SSL modules compiled with LibreSSL. Yeah.
[19:37] - Well, chat GPT, see if you can figure out how to fix this. Click the plus sign.
[19:45] - Make sure you use four. - How to fix this error.
[19:49] And what were you saying about the quotes and stuff? Because I can do a single quote and it figures it out.
[19:54] - Okay, then that's fine. Then just, it's smart.
[19:57] - I was like, so confused by it. Like I can do this and it's like happy.
[20:01] - Open up your, let's see. This means your Python environment has thing about,
[20:16] yeah, it's, and this is, I know this is the issue is the question is how to fix it.
[20:20] Okay, that's one thing. All right, that's another one.
[20:29] Okay, let's try option one. - Oh, yay.
[20:40] Well, hopefully it doesn't end up being, you know, a 45 minute stream of yay, it was quick.
[20:55] Okay, so we are going to do. - There was another step though.
[21:00] - No, it said option two. - Nope, there's two steps there.
[21:03] - It's not gonna work. At least, maybe this one it will.
[21:12] It is a different computer. - Before you run this, you can't run this right here.
[21:15] Hold on, or actually maybe you can do it. See what happens.
[21:18] - There, it ran. - Then restart this terminal as well.
[21:24] Just to make sure that takes hold. How do you like hyper?
[21:31] - I like it. I can actually see things.
[21:34] It's nice. Okay, so let's see, CD, AI, Whisper,
[21:42] and we're going to do this one. No.
[21:53] Okay, so try option two. And if it doesn't end up working,
[21:59] it's not the end of the world if we can get the C++ one to work.
[22:01] 'Cause the only thing I wanted to show is that this would take five minutes in general.
[22:06] Oh yeah, that might be good. And in general, the C++ one
[22:12] is the one you're actually going to want to use. So this is more of an example that I wanted to show
[22:15] to show why not to do this. So if we can't get it to work,
[22:18] it's not the end of the world. But is it?
[22:23] I'm just going to try it. - Try that one, yeah.
[22:27] - Sure. - You got two commands there.
[22:29] So you should copy each of them independently, yeah. - Yeah, I don't have pip.
[22:34] - Yeah, and this is, I don't know, Python virtual environments and stuff like this.
[22:40] So that's why the commands I had are like that, where they have Python three stuff in there.
[22:47] So you're still not Python conversant enough yet to get a virtual environment.
[22:51] - Well, I had to stop on Python to stick with something. And I did sticking with TypeScript.
[23:03] - Let's see what happens with this. - We'll find out.
[23:08] Probably tell me no pip. Oh!
[23:10] - Yeah, so this is what getting a virtual environment set up. So now let's see if the command actually works.
[23:16] - Well. - Yeah, just try running that command again.
[23:23] - I'll try installing. - That's, you need to go all the way back
[23:28] to Python three on the line above. - Ah, thank you.
[23:32] Hey! Okay, so let's go back to.
[23:47] - One more time. Nice one.
[23:52] Hey, I didn't get an error. - Yeah, but that's not correct though.
[23:56] That should have started transcribing, so. - Okay, well, let's try this.
[24:04] - I think you're installing Python inside a Python virtual environment now.
[24:17] I'm not entirely sure. We'll see.
[24:21] - Well, that's fun. And then we'll do this and see if it actually.
[24:27] - Don't forget those extra things on the end. - Oh, damn it.
[24:32] - I don't think those actually matter though. - Well, I don't like it.
[24:36] - Yes, it's the same error. - Enter.
[24:42] Yeah, no, okay. - Okay, so let's just do the whisper one then.
[24:46] So take, so go back to your folders and open up. Yeah, in your Finder.
[24:55] So grab that MP3 and then drag it into Whisper CPP. Yep.
[25:03] And then open Whisper CPP and then drag it into samples specifically.
[25:09] Yeah, and if you look at samples right now, there's a file called JFK.
[25:17] That's the example they get, but I want to have a cooler Teach Gen Tech example
[25:21] we can transcribe. - You didn't want to do, is this the one?
[25:27] No, it's not the one that you did a funny intro. - No, it's not.
[25:34] That probably would have been better, but this is our first interaction on stream.
[25:38] It's cute. So now you want to get into that Whisper CPP directory.
[25:44] Specifically. - Okay, so CD, no, whisper, whisper.
[25:51] And then samples, right? - No, so I only wanted for that in the commands.
[25:59] So then go back to the gist. - Okay, let's, I feel like we can put these
[26:04] side by side again, yay. - So grab that whole FFM.
[26:09] So we did all, all four of those steps should already be done, right?
[26:13] Did you do these already? - Yeah.
[26:15] - Okay, great. So then do this one.
[26:17] And with that, oh, that's, sorry. To do that command, you need to be in the samples directory.
[26:27] So go into samples now. Yeah, exactly.
[26:32] So then run that. Yep, and then pop back out.
[26:35] Just do CD, period, period. Great, and then run that big command,
[26:43] the next one in the gist. And what this is gonna do is this is gonna output
[26:46] a whole bunch of different formats. So hopefully this works.
[26:52] Not screwed. - Well, it'll think about it.
[27:00] And hey, Chris, we might work on some database stuff today too.
[27:03] - Great, okay, so open that up wider real quick. - Oh, it's when I couldn't like say.
[27:10] Oh, look at how adorable it was. - Yeah, and so, and you see how this is taking,
[27:18] that took like less than a minute, you know? If we'd done it with Python,
[27:22] it would have taken about five minutes. So that's why I say I like,
[27:25] if you're transcribing hours and hours of text, like you're talking about an hour
[27:31] versus 20 hours of time to do that. So you don't need to copy paste this.
[27:35] It dumped this into files. No, you're gonna ask.
[27:38] - It to remove the time codes. I'm just curious.
[27:41] - That's what I'm saying, it printed a bunch of, it made a bunch of files for you already.
[27:46] - Oh, that's cool. I still want to know if it can do it.
[27:49] Now I'm just curious if it can do it. Like if it's smart enough to do it.
[27:55] It is! - Yeah, it's good for these kind of data munching tasks.
[28:03] - Look at that, that was fun. So if we actually look at what it's outputting,
[28:08] you will notice it's making one big mistake here, which is that it thinks gen is gen, G-E-N instead of J-E-N-N.
[28:15] But what's nice is it does that consistently. So you can do a find and replace to fix all of those at once.
[28:21] But then aside from that, we see some of these terms here. It knows what Redwood JS is.
[28:26] It knows to capitalize Redwood JS. It knows what React is.
[28:29] It knows to capitalize React. It got first cell wrong, which is kind of interesting.
[28:34] But this is almost entirely accurate. And if you've ever used transcription,
[28:39] like free transcription services in the past, especially for technical content,
[28:45] usually it's much, much worse than this. So the first time I used this,
[28:49] I was pretty shocked by just how little modification it required if you compare this to something
[28:56] like YouTube automatic captions, it's a night and day difference.
[29:04] - The teach gen shit. But I'm not surprised that I probably said that.
[29:09] - I said that. - Oh, you, okay.
[29:11] Well, you know, whoever. - That's why I asked, is this a swear friendly stream first?
[29:16] - Oh, well, yeah, yeah. Oh my gosh, I can't believe it's been 11 months today.
[29:23] 11 months, oh my gosh. That's so fun.
[29:28] And I think I'm gonna hit over a hundred episodes. I think. - That's sweet.
[29:34] - This is bananas. Okay, so if I, I'm just curious.
[29:40] - So I tried something fun 'cause I ran this beforehand and transcribed the same thing.
[29:50] And then I asked ChachiBT to summarize it. And it wrote this summary.
[29:56] If you wanna put that on screen. - Look at that.
[30:03] - So then, so this is where it's pretty cool. And you start to see some of the workflows
[30:06] you can start to create is that once you can take your video and dump a large scale transcription,
[30:13] even if there's kind of like some small mistakes in there, you can still generate summaries
[30:18] and you can take chunks of it and compress it down to smaller chunks.
[30:22] And so it gives you just the ability to create a much larger content farm
[30:27] and ability to put out lots of content based on a single video or podcast.
[30:33] If you're just an individual by yourself, 'cause there's like some podcasts
[30:36] where there's like whole teams of people that are going through podcasts
[30:40] and like taking clips and like transcribing it and then writing little, creating little short videos
[30:45] or creating TikToks. And so there's like, there's so much stuff you can do
[30:49] with audio content or streaming content that just requires time.
[30:54] And this really can allow you to take huge chunks of this content and create lots and lots
[31:01] of different smaller pieces of content off of it. - I am gonna go test again.
[31:12] ♪ Do, do, do, do ♪ But it probably doesn't like spaces.
[31:18] So I'm not gonna do spaces. I don't wanna delete letters though.
[31:23] ♪ Do, do, do ♪ Another trucker.
[31:29] Okay, we're just gonna- - It's also worth pointing out though
[31:31] that in this summary that I provided, since it's getting a fairly small amount of context,
[31:37] it's actually confused about what we were saying. It thinks that when I said you combine the two,
[31:43] it would have been teach gen shit, not teach gen tech. So it doesn't quite understand that reference,
[31:48] but that's probably because it's like trying to parse like us making like humor with each other.
[31:54] Robots don't quite understand the jokes yet, but I can get chat GBT to detect irony,
[32:02] which I find to be super fascinating. So I gave it a phrase where I said,
[32:10] I made some comment on Twitter once. I was like, how dare you?
[32:14] Hold on, I have this written down exactly in a gist somewhere.
[32:22] So I said, how dare you discredit my unjustified slander? So obviously that's a joke 'cause slander by definition
[32:32] is something that should be discredited because it's slander.
[32:35] And so it says, when someone says, how dare you discredit my unjustified slander?
[32:40] It's important to note that the statement can be taken seriously or sarcastically.
[32:44] In a serious context, the person might genuinely feel offended
[32:47] that you questioned their false accusation. In a sarcastic or ironic context,
[32:51] the person might be admitting that their accusation was baseless
[32:54] and acknowledging that you have disproven them. So that was, I was just reading chat GBT
[32:59] basically responding to that. So I found that really fascinating
[33:03] that it actually is able to detect things like irony and kind of get into like,
[33:08] what do people mean by things they say? - I did, I think I did the wrong thing.
[33:15] - What are you trying to do right now? - I didn't correct the wave form in it.
[33:20] I need to. (laughing)
[33:24] - Yes, yes. That is probably true.
[33:28] I need to change the file. And I forgot to change the file.
[33:32] I guess I could just, there, okay. Get up and do, do, do, do, do.
[33:40] And I, can you let me type right here? Do, do, do, do, do, do, do.
[33:48] So if I already have it in a wave file, I don't need to do the first step, right?
[33:54] - Correct, yeah. Yeah, that, the FFmpeg stack step
[33:56] was specifically just for that. Make sure you got the exact same.
[34:03] - Oh, no, it's, it is the exact same name. It's not the right folder.
[34:09] - Right, yeah, if it's not in the samples folder, then you gotta fix that.
[34:14] - I will get that. What folder did I call it?
[34:17] - Yeah, this is not the most DX suite kind of exists. It's like, you, since we talked about this,
[34:24] this kind of ran on me off the cuff. Like, this is a blog post I'm like 20% complete with.
[34:29] So there's a lot more stuff I was gonna do to make this kind of nicer and make it simpler.
[34:35] But for now, these are just like the raw commands. If you wanna understand what's going on,
[34:40] start playing around with this yourself. - Okay, so I should look how long this stream is.
[34:46] How long was the stream that I picked? - Upbeat music.
[34:52] - An hour and a half, roughly. - Yeah, so that could take--
[34:58] - I'm curious. - At least my time. But, and it looks like you start
[35:00] with no one saying anything for a little bit. - Five minutes.
[35:05] - Five minutes, okay. So it's gonna be playing upbeat music for five minutes.
[35:08] - It was like the window, the window that, or you know how it does a countdown?
[35:12] - Yeah, so what do you, what did you feed it? - One of my videos from like two weeks ago.
[35:18] - Okay, cool, which one? - Well, one of the audio from one of the videos from two weeks ago.
[35:22] - Which one? - Sniffles.
[35:27] Jen makes tech queries for my database. Queries for my, it was-- - By yourself?
[35:35] - Yeah, it was on Twitch, but I don't know if I ever uploaded it to YouTube.
[35:38] - So there's another thing worth pointing out. You will have noticed when I gave you the example,
[35:42] it's us, it's two people talking, and that is represented nowhere in this output.
[35:46] So that's kind of an issue, and there's already, in the gist I provided,
[35:51] there's a whole bunch of other services and other open source libraries
[35:54] and stuff we're not gonna look at that are kind of trying to,
[35:57] there you are, hello, hello, beautiful humans. So it's weird when you get-- - I don't ever say that.
[36:02] - Yeah, you'll see, you'll start to like visually see things you say all the time
[36:06] when you start transcribing lots of your own texts. It's a very surreal experience.
[36:10] But-- - Oh my God. So we're gonna do that first. - For you by yourself,
[36:15] this can be very useful because it's just you talking, stream of consciousness, so you don't need to worry about
[36:22] being confused about who's saying what and things like that. Also, I never showed you how this was creating
[36:27] a whole bunch of different files. So-- - I looked at it.
[36:31] - Yeah, so we can talk about this briefly. I'm not an expert on this.
[36:36] If someone like Ben Myers ever is on your stream again, he can explain these way better than I could.
[36:41] There's specific files for things like captioning software. Or if you wanna-- - S-R-S-P.
[36:47] - Yeah, yeah, so that's where stuff like that is. And then also gives it to you in a text file,
[36:51] gives it to you in a JSON file. There's a whole bunch of different formats.
[36:54] I just have it right now set to give you all of them. Most of them are probably not gonna be useful to you.
[36:59] It's just depending on what you are doing this for, what you want the text to eventually be.
[37:04] And then you can kind of figure out which format is gonna make the most sense for you.
[37:07] There's a, this gets back into this being new tech, that is still getting all the kinks worked out.
[37:14] You can't edit all of them at once. Like this is such a huge issue.
[37:19] If you wanna fix things in the transcript, which you're going to have to do,
[37:23] and you want it to still be in all these multiple file forms,
[37:26] then you gotta edit each of those individual files. So people need to take these open source models
[37:31] and actually build services on top before it's really gonna become
[37:35] like a super duper useful transcription tool. But if you're someone who has a bunch of audio,
[37:41] like raw audio that you need transcribed, and it's just like, you just want it dumped out,
[37:45] like what you're doing right here, this is the use case it currently is
[37:49] really, really well suited for, and will give you really high quality results
[37:54] for no money whatsoever. So I'm glad you picked this specifically.
[38:00] - Is it proof that I'm going to talk to myself? Oh, this is when GitHub was down.
[38:08] I started streaming and I needed my website and GitHub was down.
[38:15] I was like, oh, well, I guess we're gonna work on something else.
[38:20] Well, yeah. Yeah, I don't, I mean, it's moving right along.
[38:27] It's been what, like four minutes? Yeah, and so that's why I,
[38:32] for a while I used to do this just with Python. I did like 10 or so FHM episodes
[38:36] and I used to just kick it off before I would go to sleep. And then I would just go to bed, come back,
[38:42] and then five hours later it'd be done. So this is why I wanted to show you Whisper CPP,
[38:47] C++ in particular, because the Python version
[38:51] is really kind of a massive bottleneck unless you're transcribing very, very short clips.
[38:59] - Can you make a GUI for it? - So let me go look at some of the ones
[39:05] that I have actually in here and see. So Buzz, Buzz looked kind of nice.
[39:11] - You can share your screen if you want. - No, let me just shoot this over to you.
[39:16] Just a link to a site. There's nothing interesting to see here.
[39:21] (mouse clicks) Interesting.
[39:30] And-- - Yeah. Yeah, so I haven't used any of these yet.
[39:40] So this is why I say this is a blog post I'm like 20% done with.
[39:44] So I have a bunch of references here. I know that these are things
[39:47] that are using Whisper under the hood. I have not vetted any of these tools,
[39:52] but just if people want to learn more, these are the ones that I know about.
[39:55] If you know of others, please share them. I'm like very interested in learning more about anything
[40:00] that's currently trying to push this stuff forward. - I think Parrot also does that.
[40:06] - Okay, great. - I don't think I want to go to the app.
[40:11] Let's do just Parrot AI. - And as far as I know,
[40:16] Descript now is using OpenAI stuff under the hood. But again, Descript's very expensive.
[40:23] And so I'm not a point where I can pay like 20, 30, $40 a month to do this
[40:29] because I'm not making any money off of my podcast. But I want high quality transcriptions
[40:34] 'cause that's important to me. - Yeah, I can't, y'all I'm blind as a bat
[40:42] since I rearranged my desks. Stuff.
[40:48] - So this is Parrot.ai. - Yeah, so with Parrot, I checked it out.
[40:56] I liked it. It's still also kind of weird.
[40:59] I've had to delete stuff and re-add it because web components.
[41:06] So if I'm looking at this. - Are you on the free or paid version?
[41:14] - I'm on the paid one. - Technically they're the same at the moment.
[41:20] - This says there's a personal plan for $30 a month. - Oh, do they have pricing on them now?
[41:29] - Yeah. - Oh.
[41:31] - And this is like, this is someone, so let's go get Descript's pricing.
[41:34] - I don't know. Maybe I got in on time.
[41:39] Don't tell them to take it away from me. - Descript's actually 12 bucks a month for Creator 24.
[41:46] Yeah, see like Creator 12 bucks a month is 10 hours of audio a month.
[41:50] Like that's not a lot. - I was like, I'd go through that in like a week.
[41:53] - I know that that's barely anything, yeah. - The only problem I've had is I keep saying,
[41:59] change all to speaker one and I'll not unclick that. And I'm like, oh shit, oops.
[42:05] So let's change this one to Jen. And speaker two is, don't change all the speaker two.
[42:12] Speaker two is Kiss. - Yeah, and I should mention that like there's.
[42:20] - You get to do all. - There's dozens of transcription services out there.
[42:24] And the links I gave, those are ones that are using OpenAI Whisper in particular.
[42:28] There's been many transcription services that already existed and may or may not have adopted
[42:34] these tools under the hood. It's really hard to say for a lot of them.
[42:39] Like as far as Parrot goes, like I can't really find any information
[42:42] on what's actually happening in the model. - So apparently I am on the free version now.
[42:47] - There you go, yeah. So the vast majority of the transcription services
[42:49] you're gonna pay for won't really tell you what they're using under the hood.
[42:52] You kinda just have to use them and find out whether they're good or not.
[42:55] - Yeah. - I find that kind of frustrating.
[42:58] And this is why I like that now there's an open source tool that we can use.
[43:02] And if something's built on that, I know there's a baseline of transcription quality
[43:06] I'm going to get from it. So I'll be more inclined to wanna pay money
[43:09] for a service that is building on top of that. That's kind of where I'm at right now.
[43:15] So yeah, this whole thing is something that I've been like researching for like three years now.
[43:22] And it's like so frustrating. There's like just not really many great tools that do this
[43:28] 'cause it's such a huge problem. So many people have transcribing podcasts,
[43:33] like some of the biggest podcasts in the world don't provide transcripts and it's bad.
[43:37] - It's annoying and hard to do. - Yeah.
[43:41] - And okay, so. - It's already a half hour in, that's pretty good.
[43:47] - Apparently I was talking about Jacob and his Twitter space.
[43:50] - Yeah, but you're talking about all sorts of things. - I am, I'm talking to myself basically.
[43:58] It's fun. Okay, so I feel like this is pretty cool
[44:03] and we got a solid, like figured this shit out. We can let this go on in the background.
[44:09] - Yeah, and now anytime you wanna run some transcriptions, you now have the ability to do that for free.
[44:15] You don't gotta necessarily go out to a service. How much utility you're actually gonna get out of this
[44:19] will kind of vary depending on what you need these transcriptions for.
[44:23] I don't think this stuff is fully baked technology by any stretch of the imagination.
[44:28] And if you're someone who is not trying to go really deep in like running these models on your own computer,
[44:34] you could probably look towards just paying some money and having them do it for you.
[44:38] But for me, as someone who has this issue, I want to know about what the cutting edge open source stuff
[44:44] can do and how to use it. So I found this very useful for me to learn personally,
[44:48] but your utility will vary for others. - Yeah, I say make friends with smart people.
[44:57] 'Cause they'll just tell you when this stuff happens. Like for example,
[45:03] instead of following all of these tech influencers, I just like follow people that are my friends
[45:12] that follow them, that retweet important information. - You got a powerful network by now.
[45:17] And I told you this was gonna happen when you first created this stream.
[45:22] And now we're a year in and you can see the fruits of your labor and your powerhouse.
[45:26] - I'm very fortunate for that. I am very fortunate for that.
[45:31] And thank you. I have such cool people.
[45:34] Oh, by the way, I don't think I've told you this. You should look at this.
[45:37] Hold on, hold on. Let's go to Twitch and go to Jacob's stream.
[45:43] - Never show my Twitch home screen on stream. - I'm not, oh.
[45:50] - Yours is fine. - I was like, I don't even pay attention to them.
[45:56] - Yeah. There's some stuff.
[45:59] - What do you watch? - Oh, don't worry about it.
[46:01] - I don't wanna know. Okay, okay.
[46:06] Look at this. Look at this.
[46:08] Hold on. Look at us.
[46:14] - Wow. - And that's Chris's wife, Sarah.
[46:19] She plays with us now. And yeah, but look, I like dressed up as my character
[46:23] and it's really fun. And she is so mean.
[46:25] - That's you, I was like, which one are you? Okay.
[46:28] - I am so mean. - Wow. - So mean.
[46:32] It's very exciting. It's really funny. - That's awesome.
[46:38] - You should watch it sometime. I'm gonna share this with all of you.
[46:41] Not that you really were ever gonna watch it, but if you want to, it's really cool
[46:47] 'cause I'm like the opposite of me as my character. It's so fun.
[46:52] Okay, that aside. Okay, we should go look at my websitey things
[47:00] that I got stuck on. I think I still have it here.
[47:04] - Yeah, I did not go back and watch the stream. So we'll kind of just have to talk out
[47:07] what exactly is happening and what the issue is. - Yeah, what exactly?
[47:11] Oh yeah. Chris, like I got even meaner.
[47:16] I got even meaner. I'm still like, Chris watched last week's.
[47:23] I was like, dude, you're the opposite. I'm like, I know.
[47:25] - Which Chris are we referring to? - You haven't met this Chris yet.
[47:30] This Chris is Database Chris, which I met at Denver Startup Week.
[47:35] It was a lot of fun. - Or she, is it he, she?
[47:38] - Chris does not have Twitter. Chris, why don't you have Twitter?
[47:44] I feel like it's, you should have Twitter, but I have no justification other than
[47:52] everyone should have Twitter now. There's no really.
[47:56] - Twitter, Twitter's what you make of it. You know, it's, and we talked about this
[48:01] on my very first episode, actually. I think that if you're intentional about Twitter,
[48:06] you can be some cool people, but like you don't need like a Twitter following
[48:12] unless you're optimizing for that for specific reasons. You know?
[48:16] - Like your role. There's Link.
[48:19] It was fun. It was a very fun stream.
[48:22] Taught me a ton about like relational and non-relational. - Oh, this is the person I told you to ask
[48:30] whether MongoDB is web scale. - Oh, yeah.
[48:35] Well, now you two have kind of like introduced yourselves. This is Anthony, my internet big brother,
[48:41] who also kind of likes to troll my streams and my guests. - Yeah, I do.
[48:45] - There you go. And Chris is like one of my go-to database people
[48:53] because he knows how to break it down, but also in like a really good way of understanding it
[48:58] with real life things. And I think that's been difficult for other people
[49:03] because databases can be difficult to understand. - Yeah, they're highly theoretical,
[49:09] but also highly practical because so much of what we do on the internet
[49:14] ultimately lands in a database at the end of the day. I think you don't want it in a database
[49:20] or in a lot of databases. - Okay, cool.
[49:25] So this should be up to date, but let me show you guys what I was up to
[49:31] in my last stream. This one will...
[49:33] And we did talk about code first versus database first. I did my databases first so I would understand them,
[49:42] not that it actually needed to be built first, but... - I mean, it's like, do you build your API
[49:50] before you build your front end? It's all the same at the end of the day.
[49:54] You arrive at the same thing. - It will reconnect.
[49:59] Thank you for reconnecting. Did I put you in?
[50:03] Yeah, I did put you in default. And go to my tables.
[50:08] Wow. Okay, cool.
[50:11] Okay, so I created four tables and they're the format that Chris and I talked about.
[50:23] So that way, the channel and the show can go into... - Can you just click on the channel
[50:33] so I can see what is in there? Can you visualize it?
[50:38] In terms of like the data that's actually in it? Can I see it like it's an Excel spreadsheet?
[50:44] So that's the point of PGAdmin, right? - No.
[50:47] - Is there data in here already? - No.
[50:50] - Oh, okay. Then there, that's okay.
[50:51] - But it only has... Well, it does ID and name and then...
[50:57] - Right, 'cause that would be the first thing I would say, like, regardless of what we're doing,
[51:01] you should have your data, some data, at least a couple pieces to work with.
[51:06] - Right, and I can... Let me open a new tab.
[51:12] - Yes, I'm broken in your ZRC, by the way. - Why?
[51:31] Why do you say that? - If you look at the very first line.
[51:35] - Oh, well, that's new. - Yeah, that's 'cause you ran that ZRC command earlier.
[51:43] - Yeah, I'm like, that's new. - That command was questionable, so that doesn't surprise me.
[51:48] - Okay, so I can add data in here, 'cause I do have it connected to Prisma.
[51:56] Yay. - What Prisma Studio does is broken, though.
[51:59] - Okay, so if we wanted to add some data, let me go back and look at this.
[52:06] - Like, I would at least have an episode in there, you know? - Okay, add a record.
[52:15] We have episode one, name. Hold on.
[52:25] Let me not do it this way. This card changes.
[52:30] No, I'm... - Yeah, so there's a couple questions here,
[52:34] which is that, how are you even gonna get all this data into this database in the first place?
[52:41] - Well, that's what I was trying to do, so... Well, go here, go here.
[52:50] Okay, so I have-- - You need the data in some sort of structured format,
[52:56] unless you wanna write a whole bunch of SQL. - No, hold on.
[53:03] - Yeah, no, don't do that, yeah. - Okay, let me just go put an episode in.
[53:08] Please stand by. - Yeah, I'm still not entirely sure what your issue even is,
[53:14] so I should just shut up and let you-- - I was gonna show you, but you distracted me.
[53:19] But we will do this. We will do that the channel,
[53:25] this is ID one, this is Teach Gen Tech. And then Save Changes, okay.
[53:38] And then we're going to do, oh no. Just kidding, that wasn't right.
[53:46] This is the bad thing about when you're working on it for so long, and then you haven't touched it in a while.
[53:55] Show ad record. This one, then, aha.
[54:05] Okay, give me a second. I have to remember how I set this up.
[54:29] I'm just gonna work backwards. Add a record.
[54:32] It's gonna be episode one. What is the name of the episode?
[54:39] It is AJC Web Dev. It has a hashtag of Anthony.
[54:53] - Tell me that was the second episode, but this is okay. - And it pulls the information from show.
[55:04] So see how we were filling this out, it needs to know show ID.
[55:09] So the show is, if I filled that one out, add a record, it's one--
[55:18] - Honestly, if you didn't work for a database company, I would tell you not to use a database at all
[55:23] to build this website, but this is fine, 'cause this is gonna be a useful thing
[55:27] for you to have to do. - I know.
[55:30] - And just what I mean by that is that what I would do in this example for your website
[55:37] is I would just have a bunch of markdown files. Every time you have a new episode,
[55:40] you create a new markdown file with all the information and a link to the YouTube, and that's all I would do.
[55:46] - Do you know that I have 70 episodes on the podcast and over almost 100 on Teach Gen Tech?
[55:53] That is a lot of data to try to keep track of. - No, I would say you wouldn't keep track of it.
[55:58] I'm saying every time you have a new episode, you make a new markdown page,
[56:02] and then you just do that every time you make a new episode. So if you wanted to do all of that in one go,
[56:08] there's ways you could do that, but the point is what I'm saying is that
[56:11] I would want to think of this in terms of pages, not in terms of rows in a database.
[56:18] Now, not to say one is wrong or one is right, like there's a good case to be made for both,
[56:23] I'm just saying. That's how I would do it.
[56:26] So anyway, okay. So I don't remember exactly how my database is structured.
[56:30] That's fine. I can figure that out again.
[56:32] - So what's the issue you have with that? - That is not what I was stuck on.
[56:36] I did know this when I was streaming earlier, but VS Code. Okay, so I have my schema Prisma.
[56:46] Okay, this actually makes more sense looking at it this way, but I got my schema set up.
[56:52] The way that, let me actually show you the page itself. (indistinct)
[57:02] So, last time I was working on this,
[57:21] I was able to use the template to get the six blog posts like set up,
[57:26] like this is the template. Cool, yay.
[57:29] And I got the top of it set up. I was very excited.
[57:33] We are making progress. And so that's the Teach Gen Tech version.
[57:38] This is the full default version with blog. And I was so proud because-
[57:43] - And I have seen these websites, yes. - Yeah, and I was so proud.
[57:47] I'm like, yes, I got this figured out. I am on the right track.
[57:53] Intel. So, to follow blog,
[57:59] what we just looked at is the blog list. This is the blog list.
[58:05] - Yeah. - Okay, well,
[58:08] let me look at blog content. Okay, it's in content.
[58:16] It's using, all right, I'll figure this out later. And then we got a blog summary card.
[58:22] And I'm just like- - So your question right now is
[58:27] what are Astro content collections? That's the question you need to ask right now.
[58:33] - Okay. - That is what is happening right now.
[58:35] And this is something where only an Astro core team member can truly help you with this
[58:42] because this is an Astro specific convention. Astro created their own thing to manage content.
[58:48] This is not something that was built for databases. This is something that was built
[58:52] for pulling in content from markdown files. So this is why my approach would work very well with Astro.
[58:59] And I have an Astro website myself that I already do this with.
[59:03] What you need to do is you need to get Ben Holmes and Sabin on a stream together
[59:08] to explain how the hell you would do this. 'Cause as far as I know,
[59:11] I don't know if anyone's actually used Astro content collections to pull in stuff from a database.
[59:16] It's a very interesting project. The fact that you're hitting this issue is quite fascinating
[59:21] and both of them will be very interested to hear this. So I'll say that first off.
[59:25] I don't know if I'll be able to make a lot of good progress with you right now on this,
[59:29] 'cause there's a knowledge gap here, which is that you have a template
[59:35] that's using something called Astro content collections and you don't even know what that is.
[59:38] So figuring out how to get that to work with an ORM is actually quite a challenging thing to do.
[59:45] So you wanna get the right people in the room to actually ask the questions
[59:49] of what you even need to be thinking about to get this to work in the first place.
[59:52] So that's what I would kind of recommend. And I can make those introductions
[59:57] if you don't know those people. Those are two good friends of mine,
[59:59] so not very hard to get them in a conversation. - I'm tweeting them right now
[60:05] and saying we're talking about them. And I'm specifically saying that you're saying
[60:09] that they need to be on the show. - Yes, say that.
[60:12] - I would also, actually let me shoot Ben a question right now.
[60:18] Hey Holmes, Deb. I said, yo, has anyone wired up
[60:35] Astro content collection with Prisma? He'll know exactly what I mean by that.
[60:42] I did Prisma with my other, I think I did, I don't,
[60:46] I feel like I did at some point. - Like you did what?
[60:54] - I don't know, now I have a lot of websites. I have to think about this.
[60:59] Let's go, let's go stalk my GitHub. - Let's do this first
[61:04] so people understand what I'm talking about here. Go to Google Astro content collections.
[61:09] 'Cause I'm using that term. I'm sure most people probably don't even know
[61:12] what that is. So let's talk about that first.
[61:13] 'Cause that's how your site is set up. It's using this content collections.
[61:18] This is a way to manage and author content in any Astro project.
[61:23] And it's to organize your documents, validate your front matter.
[61:28] So the fact that it's validating front matter at all should clue you into why this is made for Markdown
[61:33] and provide automatic TypeScript type safety for all your content.
[61:37] So in my website, what this does is it would be able to say, hey, your meta description and your OG tags
[61:46] is too short or too long. That's the type of thing it can do.
[61:49] It can type, it's like, so go back to TypeScript. TypeScript can type check.
[61:54] This can type check a Markdown file. But you're trying to use a database, not a Markdown file.
[62:00] So that's a whole different thing. - So it would skip this content collection
[62:08] to be able to work with Prisma and go to the database. - Yeah, you could query the database directly
[62:13] and just display it on your page, but you would be bypassing what your template
[62:18] has already set up. 'Cause your template is now using
[62:20] content collections right now. So you could trash all that,
[62:25] just have a raw Astro project and start making database queries
[62:28] and then figure out what to do when you get that data back. That's something you can do.
[62:33] I don't know if that's advisable or not. And this is why these are kind of questions
[62:37] that need to be asked to both Astro and Prisma team members kind of in concert with one another.
[62:42] - I feel like you'll need to be able to be on the show too, to like translate what I'm trying to do.
[62:48] Be like, I'm here to translate Jen. 'Cause it doesn't always make sense.
[62:53] - I think it's a super interesting question. Ben Holmes is like, how would you expect that to work?
[62:59] Which basically means I have no idea what you're talking about.
[63:05] Please tell him I tweeted that he's, they're gonna be on the show.
[63:09] Well, that at least makes me feel better that. - Okay, display this quote I just grabbed from Ben.
[63:17] So we only support file-based collections of the MoE to write to files, manual and rephrase.
[63:22] So content collections are not made to work with databases. Which is why you weren't able to figure it out.
[63:28] So you should feel good about that, that you're trying to do something impossible.
[63:31] So you shouldn't have expected to be able to figure it out.
[63:34] - Okay. But I don't get why it doesn't work.
[63:40] Like, why wouldn't it work? Why like?
[63:42] - It's because this is an Azure specific convention that was created specifically to work with Markdown files.
[63:47] That doesn't mean you can't use Prisma and Azure together, but that means the template you selected
[63:53] is not designed well to do what you want to do with it. - Okay.
[63:57] That's all I got. - Well, let me ask them now,
[64:11] do you know of any Astro Prisma examples at all? That'll be the next question.
[64:17] 'Cause so this is what you wanna do, which as I say, you are for a database company.
[64:21] It makes sense for you to build a ridiculous project just for the sake of your work.
[64:26] So you can learn things. I do it all the time.
[64:28] - It is, it really is. - It's how I've learned the vast majority of things
[64:31] I've learned in tech. I'm building projects I probably shouldn't have.
[64:34] So don't be discouraged by that. But what you need is you need a starter
[64:38] that already has Azure and Prisma connected in a way that's kind of ergonomic
[64:43] and that isn't using content collections. Which is good.
[64:51] These are important things for you to know and understand. So we are making progress right now.
[64:56] This doesn't feel like progress. This feels like we just went backwards,
[64:59] but we're making progress here, trust me. - I know I always say his name wrong,
[65:04] but I just tagged Elian in the tweet as well, because this is his theme.
[65:11] And I love this theme. I don't wanna get rid of the theme.
[65:14] I like the theme. I'm very attached to this theme.
[65:18] - Oh, the main response to this tweet. You didn't put a whole lot of context in there.
[65:26] - Yes, please fill them in. Chris said, "If you really want a good, bad idea,
[65:31] "you could write something to pull from your database, "have it generate a Markdown file."
[65:35] - Yeah, that's exactly what I'm thinking. This is the type of starter I'm looking for.
[65:42] - Well, this is a great moment to ask, because I was thinking that it would query everything
[65:51] and put it into a Markdown file with the queries. And then could I,
[65:59] could I put, where would I put the transcripts? Because can the transcripts go into the database?
[66:07] And if they're in the database, will they actually output correctly
[66:12] with the paragraphs and stuff? - Well, so once you've got something in a database
[66:19] that you're gonna be querying and displaying, you should think about it as just like strings of text
[66:24] at the end of the day, because that's what you're gonna be shoving
[66:28] into Markdown files or into HTML. So you're gonna lose a lot of the structure
[66:34] once you start doing that. But because you have Prisma,
[66:37] you can kind of write your query the way you need to, so you can get the data you want.
[66:43] This is actually, this is where GraphQL would actually be really useful.
[66:47] This is partly why Gatsby kind of had this problem solved and did it without needing a database at all, really.
[66:55] But again, this is just like, most people who create websites like this,
[67:00] they don't have a database with all their stuff in it. They have like,
[67:05] they think about things from the pages level. So this is just, it's partly,
[67:10] it's like a different kind of mental models that you need to think about.
[67:13] Like what is, what are your database queries? Like what is gonna be the query
[67:18] you're gonna write in Prisma that's going to get the data you need?
[67:22] And then how do you display that on the page? So there's a lot of ways to do that.
[67:28] And what I would do, if I were you, I would start, so if I were Jen right now, this is what I would do.
[67:36] I would first actually get all my data in a database so that I understand what the data is
[67:41] and what I'm actually working with. - I mean, I can do that.
[67:45] I was stuck earlier and that's why I was like, "Oh, I need to figure this out first."
[67:49] So that's definitely something I can do. - So that's what I wanna do
[67:52] because once all the data is in the database, then I can start working with it
[67:55] and figure out how I actually wanna display it on my page. Because until it's actually in the database,
[67:59] or at least just an example, like a dummy example, as long as it's structured correctly in the database,
[68:06] 'cause then I would wanna query the database and I would wanna just grab a JSON blob of each episode
[68:13] and throw that on the page. Then I would take that JSON blob,
[68:16] I would turn it into a component that looks the way I want it to look,
[68:20] and then I would iterate over that array to display each component in the way I want it to look.
[68:25] - So I need to go back and look at this in my database that I did set up, but the way it's set up is,
[68:36] so I have the show table, which just has A, which show are you doing this on?
[68:42] Teach it in tech or shit you don't wanna talk about. And then we have a channel table,
[68:47] which is, is this going to YouTube, Twitch? Like, where is this from?
[68:54] Where do I watch the video on demand, basically? So also like Spotify, Apple Podcasts, blah, blah, blah.
[69:03] And then the episode would be taking the information from the show,
[69:09] and then what is the name of the episode? So if this is Teach Gen Tech,
[69:16] I would have, it would grab the show, Teach Gen Tech for show ID, whatever this ID is,
[69:22] and then the name of it would be building a React web app with deploying on Vite and Vercel,
[69:32] and then we would take that information and put it with the channel
[69:36] so we know where it's going with the channel. So that is the database I set up.
[69:42] I just didn't, this is my pretty coloring of it, didn't know how to explain that
[69:47] without looking at it on my web diagram. - Okay, so Ben just gave me a link to an Azure starter
[69:56] that uses Prisma. There's a huge issue though, which is that it's using MongoDB,
[70:00] which is not a relational database. So your whole database deal becomes irrelevant
[70:04] as soon as you use it. So this was Chris's episode, SQL versus non-SQL, right?
[70:09] Yeah, so you're working with a SQL database right now. She got relations and stuff.
[70:15] So the starter he just gave me doesn't actually get us entirely to where we want to go,
[70:20] but we could just rip out the schema entirely and replace it with your schema,
[70:27] and that might kind of work after some effort. I feel like you should just put them in a group chat
[70:36] and be like, look, let's do this really cool collab on doing this
[70:42] because Jen needs to learn how to use Postgres and really wants us to work with Astro and Prisma.
[70:51] - I mean, I've wanted Astro to have nice full stack examples. If we used Redwood,
[70:57] it would actually make everything a lot simpler if I was there,
[71:01] but that's only because I know how Redwood would fit into this whole equation.
[71:05] Most people would say that would make it more complicated, but...
[71:08] - I was like, I barely, no. - I'm just giving you a solution here.
[71:14] You take it or leave it. - I mean, the solution would be like,
[71:17] I really could be like, hey, does somebody want to build my website for me?
[71:21] I'd really appreciate it. That could be really cool.
[71:23] And then it would magically be done, but that's not gonna help.
[71:25] And I don't want to learn Redwood on top of all of this. Although I will say,
[71:32] it finally dawned on me that Redwood came out of San Francisco.
[71:37] - Kind of. It was built by a dude from South Africa in Berlin, actually.
[71:44] But yeah. - Really? But isn't it like mainly you?
[71:47] Then why is it called Redwood? 'Cause I was thinking-
[71:50] - Yeah, so that's correct. That's because, so there's two people.
[71:53] There's Tom, there's Peter. Tom's the figurehead.
[71:56] He's the guy who lived in Marin and has these Redwood trees like in his backyard.
[72:01] He built it with Peter. Peter wrote most of the code.
[72:04] Peter's the South African who lived in Berlin. They worked together on an app called Chatterbug,
[72:10] which was a language learning platform that was using Ruby on Rails
[72:14] as a backend GraphQL API to a React front end. And they realized that this was so painful
[72:20] that they needed to build an entire framework to make it a nicer experience.
[72:24] So then they spent five years building Redwood and they named it Redwood
[72:30] because the first name, Chainsaw, was too violent. The second name, Hammer, was already taken.
[72:37] And the third name had to fit with the explanation Tom already wrote for Hammer.
[72:42] - Okay. Okay.
[72:48] I'm still going with it's San Francisco. - Ben is saying that there's a remix example
[72:54] you should use and translate a remix to Astro. I don't know if that's a good idea for you to do
[73:02] 'cause you don't know how to use remix yet. So that's simple for Ben to do--
[73:06] - Can you just tell him, I really, really want him-- - That would not be simple for you to do.
[73:09] - Can you please just tell him, I really want him to come on my stream with whiteboards.
[73:13] Like I need more whiteboards in my life. - He just said, I assume you're on stream right now.
[73:19] I saw the SOS on Twitter. (laughing)
[73:23] - We're gonna tell him we're not gonna figure this out right now, but that she wants you on the stream.
[73:30] - Yep. That's a good way of saying it.
[73:33] That is a good way of saying it. Yeah.
[73:36] Yeah, it would be fun. But hey, I figured out how to make Whisper do its thing.
[73:46] And it's done. Oh, it tells you the total time.
[73:51] Is the encode time or the decode time its full time it takes to do it?
[74:06] - Okay, so same as asking where the database needs here. So I'm gonna say you have a database
[74:18] with episodes of a show. It's a relational database.
[74:26] - I'm gonna take a screenshot of my pretty thing and just be like, look, it's not gonna make any sense.
[74:33] Very excited about this. - Ooh, here we go.
[74:44] Prisma, Planscale, and Astro. This is what you need.
[74:48] This is the blog post. This is one of those things where
[74:52] there's probably only one person out there in the world who's actually created content
[74:55] for this specific problem you have, but this looks like the person.
[74:58] - Yay. What up, Aus?
[75:04] What time is it there? I feel like it's probably like the middle of the night.
[75:12] (Hannah vocalizing) I haven't looked at that yet.
[75:24] I am very concentrated on resizing stuff on my Miro board. Okay.
[75:33] (Hannah vocalizing) (Hannah vocalizing)
[75:44] Sure, that'll work. So I'll need to write an article eventually
[76:01] on how to do it with Ivan. Yay.
[76:04] - No, this is actually, that's gonna be great quality content because Astro is blowing up right now.
[76:11] You should be on the Astro train in creating this type of content for Ivan.
[76:16] So this is like, this is great stuff. - Oh, it's already like, I'm focusing
[76:21] because I'm like, Prisma talks about Ivan, but Ivan doesn't talk about Prisma.
[76:24] And I'm like, what? We need more Prisma in our life.
[76:29] Prisma is happiness. - Everyone needs more Prisma in their life
[76:31] until Drizzle takes over. (Aaron laughing)
[76:35] - Okay. I just responded to Sabin and Ben.
[76:48] Yeah, I'm not sure if Sabin probably won't be able to help too much 'cause the issue more so
[76:58] is once we have the Prisma queries written. - Well, yes.
[77:03] Would you know how to write a Prisma query that would return the episodes?
[77:10] - I mean, that's gonna be easy enough to Google and figure out how to pull the information
[77:18] to query the information. - Yeah, 'cause that's what Sabin could help with.
[77:23] And then actually displaying it on the Astro stuff, that's where Ben would come in.
[77:28] And Ben has used Prisma, so we probably don't necessarily even need Sabin
[77:33] on the stream at all. - Yeah, but we now have said it,
[77:35] and Sabin already said he'd be on the stream someday, so. - Well, yeah, you can have Sabin on regardless.
[77:41] I'm just saying for this specific problem, you might not necessarily need him.
[77:46] - Yeah. - Great, he says, "Dope, I'm here to help if you hit a snag."
[77:50] Oh, I know you are, Sabin, 'cause he's Sabin the world. - He is.
[77:55] - That's his email, Sabin the world. - Good.
[78:00] Yes, yes, so many dope humans. But yeah, so I have homework to do, that's fun.
[78:10] - You do. - Damn it.
[78:13] - So is homework to do. - There is, I will get my website finished eventually.
[78:20] Eventually. - And then once you have it,
[78:22] you'll have that huge maintenance burden of the website. - That's worth it, though.
[78:29] You need to have your own website. Anyone who's actually like a DevRel
[78:34] kind of deserves it to themselves to go through the process of building their own website.
[78:39] - Well, not just that, I need somewhere to put all my content.
[78:42] - Yeah, yeah. - And blogs and show notes.
[78:46] - Notes for the show. - Just, and transcripts.
[78:52] And I just decided to make it the most complicated thing ever.
[78:56] - Yeah, that's what happens when you add a database into the mix.
[78:59] - Well, I want to make sure that I understand the databases and I want it to work the way I want it to work
[79:08] and it may not, but I'm gonna really understand why. - Yeah, no, I think this is a great exercise.
[79:14] Yeah, even though, like I said, I would not build a site like this.
[79:18] It makes sense for you to, for all those reasons. Well, that works.
[79:28] Yes, gotta have all the bases covered, yes. Well, hopefully we get to have a stream soon
[79:37] where Anthony comes on to translate with Sabin and Ben. We're just gonna have a party.
[79:47] - Yeah, let me know if you get either of them on. I don't think you need to get them both on at the same time.
[79:52] - Dude, that would be really funny. - Yeah, ideally you would want to get Sabin on first
[79:56] so you could write the queries. Then you'd want to get Ben on
[79:59] so that you could then just take those queries and then get them into the Astro project.
[80:04] That's how I would probably do it. 'Cause otherwise, Ben's gonna have,
[80:07] if you get Ben on first, Ben's gonna have to figure out how to write the Astro queries with you
[80:10] or have to figure out how to write the Prisma queries with you.
[80:13] And then there'll be nothing for Sabin to do. - All right, all right.
[80:19] Well, that's fine. - Or you could just have me build it in Redwood
[80:26] and then we wouldn't need either of them. - I like Astro.
[80:32] - No, you'd still be using Astro. Astro would be querying a Redwood API.
[80:36] - Oh. - But actually, yeah, let's not do that.
[80:44] But the next time I come on, I will just show you Redwood in the abstract
[80:49] and show you how to connect that to Ivan. And then you'll have a Redwood Ivan example.
[80:53] - How about we do that on July 5th? - Yeah, that sounds great.
[80:59] - I actually do have to check my schedule. I'm not sure.
[81:01] I moved that week, so we'll find out. But--
[81:04] - It's a Wednesday, so I will be doing JavaScript jam, but I can fit it in.
[81:09] - All right. And I'm gonna be in a new time zone.
[81:12] Oh, that's gonna be confusing. - You're gonna be in Pacific?
[81:16] - Pacific, yeah. - Specific time zone. - I'm gonna get
[81:19] all sorts of confused. - All right, y'all.
[81:22] I'm gonna raid you over to Chris Griffin, 'cause he's a dope soul.
[81:27] And, dude, Phoenix time is weird. Phoenix time is really weird.
[81:34] I agree. - I like the Phoenix. - Yeah, it's gonna be nice and toasty.
[81:39] - Need to hang out with Lucia. I think she's in Phoenix.
[81:41] - She is! I'm so excited, yes.
[81:44] And bye, y'all. Thanks for coming to hang out.
[81:49] - Bye. (computer mouse clicking)
[81:54] [BLANK_AUDIO] 
