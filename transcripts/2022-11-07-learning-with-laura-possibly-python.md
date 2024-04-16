---
showLink: "https://www.youtube.com/watch?v=aYJRn6qf28U"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-with-laura-possibly-python"
title: "Learning with Laura: Possibly Python"
publishDate: "2022-11-07"
coverImage: "https://i.ytimg.com/vi/aYJRn6qf28U/maxresdefault.jpg"
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

[00:00] Hello, hello, beautiful humans. Welcome to Mondays, which is Teach Gen Tech
[00:08] and Learning with Laura. Yay.
[00:11] And we talk about a lot of random stuff. We do.
[00:15] We do. That's why I love Mondays.
[00:17] They're random. Yep.
[00:20] Yeah. And especially when the cleaning fairy
[00:23] comes in the middle of the night. It's like Brain Dump Monday.
[00:28] Ooh, I like that. I feel like it's such a good way to start the week too.
[00:33] Yeah, I mean, yeah, for sure. I dig it, I dig it.
[00:38] So just going off of my memory, we are thinking a little bit of Python,
[00:47] a little bit of, I don't even know what the, what is it called?
[00:51] Mastodon? Mastodon, see, I don't even know what it's called.
[00:56] And then maybe some Arc. And eventually we might look at flashcards, y'all.
[01:04] We haven't actually finished that one, but hey, that's okay.
[01:10] This is Brain Dump Mondays. Yay.
[01:14] Oh, Stream Elements is telling people that we are live. That's fun and interesting.
[01:22] I don't think I know Stream Elements. Whoa.
[01:28] Ryan set it up where it does like auto commands and stuff. And that's why I'm gonna try to use OBS
[01:35] is Stream Elements, you can create like an overlay and put it into OBS.
[01:41] And then OBS, like to get the people in OBS, you use ping and then you stream it to switch,
[01:50] switch to Twitch. So.
[01:55] - Okay, right. - It does something, I don't.
[01:59] - Yeah, cool. Things occur.
[02:02] - Yes, yes. It is the thing I'm currently working on.
[02:07] But which one would you like to start with of our random things of the day?
[02:15] Which I need to start making notes. I did finally paste notes from last time
[02:20] of what we were talking about in the show notes. So that way I know what to tell people
[02:26] we're actually talking about. - You know, this, I've seen tweets from people
[02:33] calling out how podcasters will spend like the first 15 minutes of their podcast talking about
[02:42] not whatever the topic is and how that's super annoying. And I was like, oh no, is that me on the stream?
[02:49] - I'm totally, as for like the, I mean, as somebody that has a podcast too,
[02:57] I just dive right into that shit. Like we literally are like,
[03:00] hey, thanks for coming on the show. Please introduce yourself and the shit you wanna talk about
[03:04] and like go right in and like, this one I just feel is like so fun and chill.
[03:09] So I think it really matters who we're doing this for. - Are we doing this for us or are we doing it for them?
[03:19] I feel like this is for me because I just like hanging out with you and we learn a lot of cool stuff
[03:28] and you know, people can always fast forward. - Works for me.
[03:32] - Could fast forward. Maybe that's something too.
[03:35] I will start writing down time codes of when we do stuff. Maybe I'm going to go back to pen and paper.
[03:42] - I mean, yeah. And we can set it up too, because the streams
[03:47] only live on Twitch for like a week or. - Yes, they do live on YouTube forever.
[03:52] - They get forwarded to YouTube, exactly. And YouTube does the chapters.
[03:55] And so we can like add chapters. Like here's where we actually talk about the Python.
[04:02] Here's where we're just brain dumping on whatever. Here's some learning theories.
[04:09] Here's some neurodiversity. - It's true.
[04:13] We do that too. - Oh, and the other thing that I forgot to do
[04:17] that I got to do really quick before we dive into whatever fun stuff is telling people that we're live.
[04:23] I've been trying to like reshare the message and normally have it up on my screen.
[04:31] So that way I can just be like, click, send, and it's done. But I didn't have it set up.
[04:38] So now I have to go find the tweet and post and quote tweet and say we're live.
[04:46] It's a much more complicated process, post. Oh, I just reposted, okay.
[04:54] Share your thoughts. We're live.
[04:57] It's going to be really annoying about it on LinkedIn. That's fine, cool.
[05:08] Yay, okay, done, done and done. So.
[05:15] - Okay, good. And then we can talk about things in whatever order
[05:17] do we want, 'cause we'll add the chapter stuff later. - Yes.
[05:25] - I find that very freeing. - I'm also writing down our topics so I remember.
[05:32] - Oh, cool, cool. - I'm a pen and paper kind of person.
[05:36] It's not great for the environment. I have tried Rocketbooks, yet I hold on
[05:43] to all of my old notebooks, all of them that I've ever had. And I like going through them from time to time
[05:51] and I'm like, ooh, this is fun. - I do the same, except it's on an iPad.
[05:57] Like I also like to write notes by hand 'cause I'm writing it with, you know, it's my hand.
[06:07] But I can search. - Ooh, I did try Remarkable, I think it's what it's called.
[06:15] It's like a tablet that you can, that literally all it does is write.
[06:19] - Yeah, and you can't search. I know, because my boss uses it and then is like,
[06:25] oh, but I have these notes, but now I can't find anything in them.
[06:28] And I'm like. - Cool.
[06:31] So does it do, does the iPad do it pretty well going from writing to text?
[06:39] - Yes. I might be able to show you.
[06:42] Let me see if I have, so the app that I use is called GoodNotes.
[06:46] I don't know if I have it installed right now. Do I?
[06:49] On the Mac. Do I, I know I have it on that tablet,
[06:54] but do I have it over here? Yes, I do.
[06:56] Okay. And it might need to update
[06:59] 'cause I haven't opened it in like a year. - So you can actually have them sync between the two
[07:07] so you can. - Oh yes, oh yes, oh yes.
[07:10] - Does it sync automatically with your, yeah, your iCloud notes?
[07:18] - Oh, no. - Okay, it, no.
[07:23] - I keep it in my iCloud. Like that's where the data lives.
[07:29] - Okay. - It's not running properly.
[07:35] Let me try that again. Yeah, and so it's just,
[07:39] it's completely separate from the Notes app on the phone or the tablet or whatever.
[07:48] I also use that because that's how I do like scans. But okay, so the app is not happy
[07:59] and I strongly suspect it's because I need to update it on the Mac.
[08:05] But, oh, you know what? They probably have a website.
[08:07] We're on the internet. Let's just look it up. - We got this.
[08:11] - Yeah. - We got this. - And so it's called GoodNotes, all one word.
[08:15] - Cool, I will look it up and verify that I can find it. - They probably have a demo.
[08:22] I wonder. - Ooh.
[08:27] It says right outside the lines. I like it.
[08:33] (Hallease humming) I got that going in our Notes.
[08:48] Maybe I'll set up some GoodNotes and it might be magic. - They might even be collaborative now.
[08:55] I kind of think that's a thing that happened. - I kind of think so.
[09:03] That that's been like an update, maybe. Well, okay, that's really disappointing.
[09:16] I really cannot get this app to run at all and it does not say that it needs to be updated.
[09:20] So this is a great endorsement for me where I'm like, I literally can't even run it.
[09:24] It's awesome. - That's what happens when you're using Drive.
[09:28] It's just like, it's inevitable. - Yeah, but so yeah, I'm not sure what the issue is
[09:34] at the moment because I use this app. When I was teaching, I used it all the time.
[09:40] I use it less now or almost not at all now, like on the Mac, I use it on the iPad all the time.
[09:46] - Got it. Well, I am now looking at it and-
[09:50] - Share my iPad screen. - Ooh.
[09:53] - Yeah. Do you want to share your screen, the browser tab
[10:00] for the GoodNotes? I'm going to grab my iPad and see if I can.
[10:03] - I know how to do it on Zoom. (humming)
[10:08] - Ta-da! Very excited about this.
[10:23] I just started downloading it. - Yeah.
[10:25] - Open. - I don't know if you have an iPad.
[10:30] - I don't, it is on my to-do list once I have a real job. It's a real job.
[10:38] - Understood. - Oh, I can do screen mirroring.
[10:51] I wonder if that like translates to over here. I don't know.
[11:00] Okay, well, I'll figure that out another time, I suppose. Anyway, yes, I can, I can, the,
[11:08] oh, oh, oh, it's finally, oh, I think it was just like, wait, what?
[11:14] - Did you get it working? - Maybe.
[11:18] That's fascinating. What's it doing?
[11:20] - Oh, I can make a new- - I was such a dork.
[11:23] It's yours. - Is it mine?
[11:25] - It was looking at where it was like, hey, it's displaying, but why isn't it responding to my cursor?
[11:32] It's like responding to somebody else's cursor because it's literally not mine.
[11:37] And I am absurd. - It's cool, it's cool.
[11:40] You know, this is, let's do ruled. Let's change the cover.
[11:47] This is, this is where I get stuck in life is I wanna look at all the covers
[11:53] and see if there's anything. I'll do, this one's fuller, solids.
[12:02] Yellow! - Great.
[12:05] And you can choose paper that's not yellow if you prefer. And.
[12:17] - And y'all might know better than I do, but I wish they had a pen to use on my MacBook.
[12:28] Like it doesn't require the screen, but like if I wrote on like anything,
[12:36] it would like just show up here. - Something would have to have a touch screen then.
[12:43] - Would it? 'Cause I, hello, homie.
[12:47] What up, pseudo? But like, what about if it was like, you know, the pen?
[12:56] I think they have something like that out where the pen can be read by a computer
[13:04] without a touch screen and you can write anywhere. It's gotta have that out.
[13:08] - Oh yeah, maybe. I don't know if it would work as well, but maybe.
[13:17] Um, but maybe. - To write on any surface.
[13:29] Um, apparently they do. - Yeah, it's super cheap too.
[13:37] - Yeah. Yeah.
[13:39] So let's try this link just because I'm looking and homie, yeah, that's what Laura was saying.
[13:48] We're gonna skip over the video. I don't want to.
[13:50] Okay, so apparently not. One day I will get myself an iPad
[14:01] and this will make it easier. For now, we will work with this.
[14:06] It will be right. - Sounds good.
[14:08] - All right. Thanks for going down that rabbit hole with me.
[14:11] I enjoyed it very, very much so. And I believe I can type.
[14:17] Can I type? Okay, I can type.
[14:18] That's good. I'll try doing this now on this notepad.
[14:23] It'll be fun. - See, Rocket Books.
[14:27] I don't know Rocket Books. - I still have my Rocket Books,
[14:31] but A, they actually are really annoying and take forever to dry after washing them.
[14:41] Just a sec. Please stand by.
[14:43] This thing is full of notebooks. - Oh yeah.
[15:05] - But somewhere in here, I'm pretty sure is my Rocket Book. I've had two.
[15:11] And they're pretty cool. It's, I don't know.
[15:15] It just wasn't the same for me. Same with the Remarkable that I used.
[15:20] Where'd it go? Oh, apparently I wanted to put it somewhere else.
[15:27] That's cool. But that's a big reason why I don't like it though
[15:32] is because A, it doesn't translate very well for writing. And then also it does,
[15:41] the pens aren't very great and you have to use specific pens
[15:48] and it can't pick up all colors. So.
[15:52] - Okay. I may have just worked out how to share my iPad screen.
[15:59] What I can't tell is whether it's gonna work. - This is why it's called Learning with Laura
[16:07] because you just learn a lot of random stuff. - Okay.
[16:12] So at the moment, I'm just gonna share the whole screen. And so we're gonna have an Inceptions.
[16:19] Everybody close your eyes for a second. And now, okay.
[16:24] Can you now see? - Look at that.
[16:27] - It's working. Okay, cool.
[16:31] So, would you like to see some of my notes from grad school? - Yeah.
[16:39] - Cool. - That just sounds fun.
[16:41] - Yeah, okay. So this is from my Mathematical Logic class.
[16:46] And these are my lecture notes. I will go to, say, I'll just go to the beginning.
[16:53] Okay, so these are notes I took by hand on, oh my God, is it November 10th today?
[17:01] No, it's the 7th. But this is almost, let me see if I have,
[17:04] I don't have the 7th, but that's funny. Anyway, these are notes that I took by hand
[17:08] six years ago almost today. And so we can zoom in and I can search.
[17:15] So say I wanna look for, let me just highlight a word here. So, oh, this was not a good example
[17:26] 'cause too many of these words are not words that are gonna show up in an English dictionary.
[17:31] Let me choose a different notebook. Um, um, um, not this class.
[17:38] So let's try, uh. - Your notes are so like well put together.
[17:44] Like, do you, my notes don't look like that. - Well, these are my notes from class.
[17:52] I'm sorry? - Oh, these are to present to the class, right?
[17:56] - No, no, no. These are like notes that I took during class.
[17:59] - Yeah, my notes never look like that. - Oh, okay.
[18:04] And yeah, and so like I used this, like I would color something green
[18:12] if I wanted to flag to myself that that was something that we, the professor told the students,
[18:18] like, okay, you need to do this outside of class or like convince yourself that this is true
[18:25] or something like that. And so here we were supposed to generalize
[18:28] that this function F was continuous for all elements in the, in the real numbers and stuff.
[18:36] So we can search. What is it?
[18:43] It's been. - I am still listening.
[18:46] I'm trying to find one of my notebooks that show my type of notes.
[18:52] - Comments, there are comments now. This is totally collaborative now, that's awesome.
[18:58] - Right, handwriting is so nice. Your handwriting is so nice.
[19:06] - Oh, thank you. Actually the professor of this class,
[19:10] when he saw my notes said that he wanted to do a, write a book with me and have me like hand write it
[19:19] instead of like typing it or whatever. - I would love that.
[19:25] - Unfortunately, you can't actually see my whole screen because like you're not seeing right now the text box,
[19:34] but I'm going to search for the word measure in here because it's going to show up all over the place.
[19:42] So I just typed the word measure and it totally found it in my handwriting.
[19:46] - That's fascinating. Y'all, I need to get a real job
[19:52] so I can get a one of these. - And here's another one.
[19:55] So like, I'm just like rolling through the search results for the word measure right now.
[20:01] - Don't. - And it highlights it as well.
[20:08] So I love taking notes by hand and especially because I can use colors
[20:18] instead of having to have like seven different physical pens, you know,
[20:23] I have all these colors and I can do all these shapes and I can make super straight lines.
[20:29] Like I can just go, you know, like here's a line. It's not going to start out straight.
[20:34] Oh, hang on. I need to choose the straight line tool.
[20:37] Here's a line and it's just going to become a straight line. - Dude, that is actually really cool.
[20:46] I'm grabbing a couple of different notebooks because they're like, my notes, literally y'all,
[20:53] I'm just like, okay, so this is, I don't even know what these are.
[21:03] Like my, me taking notes, I honestly sometimes have no idea
[21:07] what I'm actually talking about. Oh, here we go.
[21:11] Like, do you just see how all over that is? - I think at least I can't see you
[21:18] 'cause I'm sharing my screen, like my whole screen. - I mean, let me go this, like it's just mumbo jumbo,
[21:25] very colorful mumbo jumbo, but there's arrows. There are arrows to things.
[21:35] I'm like, your notes are so nice. - Oh, well, I mean, thank you.
[21:44] - Would you be like a professional note taker? Like, that sounds weird.
[21:49] I don't know. I just want to see you write things.
[21:51] Like, this is what your stream could be on. You could just write things.
[21:56] I think we would all. - Let me, this is about to be like the thing
[22:03] that made GoodNotes like a killer. This, I would not leave for all of graduate school
[22:11] because this, being able to do this was also huge with the colors because I could write.
[22:19] So this is a proof of a theorem and I could correspond my colors in my drawing
[22:28] to like where that shows up in the proof. So like, here's this, oops.
[22:40] Here's this like yellow thing going on right here. And then I can instantly see in the proof
[22:47] that that's showing up in these three places. - Wait, do that one more time.
[22:54] - Okay, so in the diagram that's helping me visualize what's going on in the proof, I have this yellow thing.
[23:03] - Yeah. - And then that corresponds to stuff in the proof itself.
[23:10] So that I can keep track of like where the, where the concept comes from in the diagram.
[23:17] Like there's where the yellow thing came from and here's a pink thing.
[23:24] And I can show, I can explain to myself where that came from.
[23:30] Like, why is this true? Oh, because it's over here.
[23:36] - Y'all, a couple of different things. Oh, it is only for Mac.
[23:43] I was looking and I was hoping that it would be for like Android as well.
[23:47] And that would have been really cool, but no. - It's probably 'cause it's also only for iPad.
[23:51] Like the good notes app, the original product is only on iPad.
[23:57] - And Sudo had a really good idea of streaming mock interviews.
[24:03] Streaming mock interviews and interview prep stuff. I'd be so down if anybody wants to come on
[24:11] and do that with me. 'Cause that's not my forte.
[24:15] - You know who else does that kind of, or at least interviewee preppy stuff is Ian Douglas.
[24:24] - Yes, yes, yes. I catch his streams a few times.
[24:28] He's been on the show too, but maybe, ooh, maybe he'll come on the show to do this.
[24:35] - Ooh, that would be fun. - Good idea, Sudo.
[24:37] And let me know if you think of anybody else that I should have on about that,
[24:41] because I feel, I'll just ask if anybody wants to come on the show to do it.
[24:47] It'll be fun. But yes, I think we talked about that
[24:53] for like 20-ish minutes, 15 minutes, like that? - Yeah.
[24:59] - Yeah, yeah, okay. So chapter one is a good notes and it's about five.
[25:04] - Note taking. - Minute, yes.
[25:06] And this is a big thing, y'all. I know this started out as being Python,
[25:12] but I've learned so much of how to learn. Like seeing these types of like notebooks and things
[25:19] is not something that I ever would have thought about. And seeing that, seriously, Laura,
[25:27] since you started streaming with me, I'm just like, dude, there's so much more I can do
[25:31] with my life and make it more organized. So, really, it's true.
[25:37] No, no, it's true. Yeah, no, this is 100%, 100%.
[25:42] So if we give a round of applause for Laura, because it's amazing.
[25:47] - Well, I have a note taking mentor. And so I'm gonna have to just,
[25:55] her name is, well, she is now Dr. Tydenne Bradley. - Dang.
[26:02] - Let me find that. But we were grad students at the same time,
[26:06] which means I feel like I know her and she does not know me.
[26:10] (laughing) You know how it goes.
[26:13] - Y'all, let's go find her on Twitter and see if she'll be on Learning with Laura's show.
[26:22] - Oh, that would be super fun. So in fact, like somebody, when we at work,
[26:29] well, at work, we're remote, but folks were having a chat once about
[26:35] what would you do if you could go back to university? And I said, I would get a PhD in category theory
[26:43] and I would have Tydenne Bradley as my thesis advisor. So, yep, this is a dream for me.
[26:52] I'm gonna share my screen so that we can see her. Yeah.
[27:00] And so, let me see, categories. - She looks like a real human.
[27:09] - Right? - I never know to like--
[27:12] - She sure sounds like one. - Yeah.
[27:16] - I mean, I like, just from reading her writing and hearing her on podcasts and things like that,
[27:21] she seems like-- - Can you send me that link really quick
[27:24] so I can drop it in the-- - Sure.
[27:27] It's mathrema.com, so M-A-T-H-3-M-A. I know you asked me to send you the link, but--
[27:38] - I dig it, I dig it. - It's a short one.
[27:42] - It is, it is, and you spelt it out for me, so it doesn't sound as complicated
[27:47] as I thought it would be. - I'm trying to find, oh, here we go.
[27:51] Is this it, where she's got notes? - Oh, her notes look--
[27:56] - National Handwriting Day. (laughs)
[28:01] I love it. And yeah, her notes are all handwritten.
[28:03] Actually, her thesis has her handwritten stuff in it. Her thesis, here we go.
[28:14] - Dude, that's crazy. - Just click this.
[28:22] Are we gonna download? Oh, PDF, there we go, haha.
[28:28] Eventually, it'll load someday. It's a really long PDF is what's happening here.
[28:44] It's like 100 and something pages. (sniffles)
[28:50] Wow, this really is taking a long time. Anyway, yeah, so she has a post on her blog
[29:06] about how she takes notes or took notes in grad school, which influenced my note-taking philosophy.
[29:18] As it were, there we go. Yeah, at the interface of algebra and statistics.
[29:24] But she's got, see these, we like, can I zoom here? Yeah, little like things that she drew by hand.
[29:36] It's so cute. And do, okay.
[29:45] Yeah, anyway, so lots of just drawings and handwritten notes going on here.
[29:54] And she really tries to make her content really accessible, which I think is the mark
[30:04] of a truly excellent mathematician. The idea that the better you can explain something,
[30:15] the better you understand it. If you can't understand,
[30:18] I think there's a quote that's attributed to Richard Feynman, but all kinds of stuff
[30:22] is attributed to Feynman that wasn't really Feynman, but we'll just go with that.
[30:26] That's something like, if you can't explain it, and I think it's where the explain like I'm five thing
[30:31] comes from, that if you can't explain it to a five-year-old, you don't understand it well enough.
[30:44] I may or may not be writing the tweet to her right now. Ooh.
[30:49] Staring off on my second screen. And then I'm gonna ask all of you
[30:56] that are currently watching us to retweet it as well. So give me a second.
[31:03] Tweet, that was exciting. I would fangirl so hard, it would be embarrassing.
[31:10] Yeah, I awkwardly have gotten like people on the show by doing this.
[31:15] Some say yes, some say no, some just ignore my existence, which I'm okay with that too.
[31:20] Yo, what's up? You are on, where's street?
[31:30] Okay, you're on YouTube. Most of everybody watching is over on Twitch.
[31:35] Did you ever get your Twitch fixed? Up for the challenge is someone I met on an ADHD group
[31:43] and they said that they were like, Twitch deleted their accounts or something.
[31:47] It was like, yeah, what would happen? Interesting.
[31:52] Fully locked out of Twitch. Fully locked out.
[31:56] That is not cool. Like, anyway, anyway.
[32:01] Okay. I'm glad we streamed to YouTube too.
[32:04] Well, everyone, please go retweet this tweet. I can't talk.
[32:10] So that way we can get her attention to go be our friend and maybe be on the stream
[32:18] because that would be really, really cool. And I would die.
[32:21] We got to do it for Laura. We'll just keep bugging this person.
[32:26] All right. Oh, that kind of locked out.
[32:30] Okay. You just can't log in.
[32:35] That, that's okay. Yeah.
[32:37] That was a lot less dramatic than, than what I was imagining,
[32:39] which was like Twitch had like launched a full scale, like barring the doors to you.
[32:45] And I was like that, whoa. Ooh, politics.
[32:54] I love politics. Yeah.
[32:56] Well, so they, he just doesn't have access to them. Like they, it's a glitch
[33:03] that they can't get him access to his accounts. So the accounts are there.
[33:08] So like he can't log in or something, but then he would lose all of his followers.
[33:15] It's true. But if you can't actually utilize it,
[33:19] then you're still losing all your followers. Now we're just going to talk about what you're doing.
[33:27] What are you doing for the chat? I don't even know if I know your real name.
[33:32] Like I've talked to you, but I don't know if I know your real name.
[33:35] Anyway. - Yes. - Yeah.
[33:36] - But- - All right. Okay, so it's 34 minutes into the podcast
[33:43] and we've talked about several things that we weren't going to talk about.
[33:46] - Yes, yes, yes. - Or maybe just one big thing
[33:50] that we weren't going to talk about, which is, which is cool. We are allowed to brain dump Mondays.
[33:58] - Yes, yes. Brain dump Mondays.
[34:00] - I actually kind of think that we should, we should maybe just rename.
[34:05] - Yeah, that's what we're going to call it. I like it.
[34:10] Because I feel like it also gets the Mondays out of Monday. 'Cause it's like no pressure.
[34:17] I do feel like I should probably have you be like my teacher though.
[34:24] And like, be like, look, I got my Python homework done. Especially since we're not really doing it
[34:29] on the screen anymore, but that's okay. I thoroughly enjoy this.
[34:35] - I'm about to be, what I'm about to say is ridiculous. - Oh.
[34:41] - But we could have two streams. We could have brain dump Mondays
[34:43] and a learning plan on stream. - I'm not mad with it.
[34:48] I'm not mad with it. I'm not mad about it.
[34:50] Because I feel like that's the hard part is I'm like, but I want to talk to you about all these random things.
[34:55] - Right, right. It's like catch up time.
[34:58] I mean, I'm literally sitting here with my coffee and you know, it's like, yeah, we could do that.
[35:04] - Because a lot of the learning part of it is like outside of it.
[35:09] So yes, so everybody calls him up. I'm cool with that.
[35:14] So up and up says that we should do it. I mean, let's talk, let's talk.
[35:21] Any suggestions on days y'all? I mean, other than Wednesdays,
[35:25] 'cause that is neurodiversity and tech day. So if anybody else has any suggestions.
[35:32] - It's gonna have to be Fridays then. That's actually.
[35:34] - We could do every other Friday. - Wednesday and Friday are the only other ones.
[35:38] - Yeah, I wonder. - I say that because.
[35:42] - 'Cause we have started doing it every week because it's hard to remember stuff.
[35:47] - Yeah, but I have. - From two weeks ago.
[35:49] - I have to type script every other Friday. - So we'll figure it out.
[35:54] - We could do the opposite. Opposite Fridays.
[35:57] So like every week we're learning going back and forth, which it's crazy.
[36:01] But for me, as long as I associate it with a person or like a day or something,
[36:06] I can go into that mode of learning it. Where is it?
[36:11] Because people are like, how are you learning all these languages or frameworks?
[36:14] And I'm like, they all kind of go together. - And when we were doing the Python every other week,
[36:22] we were also doing the brain dump Mondays at the same time. And so it was harder to make progress
[36:30] if we're measuring progress in like a linear way, because we were also doing the other stuff.
[36:36] And that, so now if we do it every other Friday, if we start to head off on a tangent,
[36:41] we can just write it down and be like, we'll talk about this on Monday.
[36:46] - Yes, yes. - Okay, let's do that.
[36:53] Cool. - This is exciting.
[36:55] This is exciting. Okay, something that we did talk about.
[36:58] So last week y'all, we didn't stream because it was Tyler's birthday weekend.
[37:03] We went to the zoo where I hobbled around with my very, very swollen ankle.
[37:09] And yeah, I fell. It was pretty funny.
[37:13] - Off a stool? - Colorado Springs, sorry?
[37:18] - Off a stool, you fell, I think? - Yeah.
[37:20] - Something like that? - Yeah, yeah.
[37:24] It's still, it's I guess a bone bruise. So it's gonna take a lot longer for it to heal.
[37:31] Like the bruising itself is gone, but there's still like this giant bump.
[37:35] No, it is not broken. I've had x-rays.
[37:38] It is literally just didn't take time to heal. But Colorado Springs Zoo in Colorado is spectacular.
[37:46] We got to feed the giraffes and see lions like right next to each other,
[37:56] like the glass and on the other side of glass, they were just chilling.
[38:00] It was crazy. - Okay.
[38:03] 'Cause I was like, okay, that sounds really dangerous for the giraffes.
[38:07] - No. - I was like, wait, you were feeding the giraffes
[38:12] and then the giraffes were feeding the lions. - I mean, they could, that is like, it's a circle.
[38:21] I think that's what would happen. - Not when it doesn't sound like the most peaceful way
[38:29] to spend a weekend. - No, but if you wanna go see the kind of stuff
[38:37] that I posted about, it's over on my TikTok. It was really cool.
[38:42] Anyway, so the week before that, we were talking about Twitter and we love Twitter,
[38:51] but Twitter, well, let's not go into too much detail about Twitter
[38:55] 'cause there's a lot of processing for people, all that, but there is a social media network
[39:00] that so many people are talking about. I don't even know how to say it.
[39:04] I don't, Mastodon? - Mastodon.
[39:07] You know the, well, not, I mean, well, prehistoric. Sure.
[39:14] The ancestor of the elephant, right? The Mastodon, big tusks,
[39:22] and they lived here on this continent. You know, you know, I know you know,
[39:30] and you'll see like a picture and be like, "Oh yeah, of course, a Mastodon."
[39:33] - I'm just really excited that that's what it is. - Yeah, yeah, it's super cute.
[39:45] And things ought to be super cute. That's like a sticking point with me,
[39:50] that things ought to be super cute if they possibly can. Hi, Abdullahi.
[39:56] - Yeah, what up? I should also write down this time code
[40:01] of knowing what time we actually started talking about this, which was like 40 minutes-ish.
[40:06] - Dudes. - Dudes.
[40:11] They were around until like pretty recently in history from up over on YouTube.
[40:19] - Yeah, that's why I was stumbling over whether to call them prehistoric, because it's so close.
[40:26] - Okay. - That it's like, are they strictly speaking prehistoric?
[40:29] And I decided they were, because I think we usually refer to things as prehistoric
[40:34] if they are before written history. I think that's how we delineate
[40:39] what's prehistoric and what's not. - Okay.
[40:43] - And look, look, look at that. Look down there, little to the right.
[40:53] Look at that. Yeah.
[40:56] Isn't it adorable? - See, I think I always thought they were called mammoths,
[41:02] and I never, that's why I never got really excited about this new-
[41:06] - Oh, like woolly mammoths. - Yeah.
[41:09] But now that I know, it's like, y'all, I love it. Oh, another thing about the zoo.
[41:13] They're put away for the winter. That sounds weird, but they actually have African elephants,
[41:20] where a lot of the zoos in the U.S. only have Asian elephants and they have African ones there.
[41:27] And it's really expensive, but someday I'm going to do the like,
[41:32] you get to hang out and feed the elephants there. And they have African elephants.
[41:37] And then I'll just do like a video with it and show you guys.
[41:39] - Yes. Yeah, our local zoo also has African elephants.
[41:44] Actually, I don't even- - I don't even remember where you live.
[41:47] - Have Asian elephants. I live in the Bay Area,
[41:49] San Francisco Bay Area in California. - Oh, I haven't gone to the zoo there.
[41:52] I only went, I've been to San Diego, and at least each time that I've been to San Diego,
[41:56] they only had Asian ones. - Okay, yeah, this is the Oakland Zoo.
[42:00] And they, at least this was true like 10 years ago. Their elephants mostly don't live at the zoo.
[42:13] They have a like giant habitat up in Northern California. And that's where they live most of the time.
[42:23] And then they rotate in a few at a time to come spend a couple months living at the zoo.
[42:29] So most of their life is not actually in a zoo. I wonder if San Diego does the same thing.
[42:37] 'Cause now that you're saying this, it sounds familiar. - It feels like correct behavior to me.
[42:45] Like I have very mixed feelings. I mean, mostly not mixed,
[42:50] mostly pretty negative feelings towards zoos. But that seems like,
[42:58] especially because these are elephants that were rescued. They were not like snatched from their native habitat
[43:06] to come and like be looked at. You know, these are elephants
[43:09] that were rescued from a circus or whatever. But they get to live much more natural lives
[43:18] most of the time. And they also, even within the zoo,
[43:22] there's like the space where you can look at them and they can leave and go to like the space behind that
[43:30] where there are people staring at them. And they are free to just come and go.
[43:35] I love that. And in October, they eat pumpkins.
[43:40] Which is so cute. They just like pick up an entire pumpkin and go like.
[43:51] - Y'all, we're going to the open zoo in October next year. We're going to do a Learn with Laura,
[44:01] Teach Gen Tech meetup at the zoo. - I get what you say about like disliking zoos.
[44:13] I think for myself, it's a lot of like, are they doing things to actually help these animals?
[44:25] Where do the animals come from? What do their grounds look like?
[44:32] Their areas. - Their living space, yeah.
[44:34] - Yeah, so I think a lot of it, because I love zoos because it's a very educational space,
[44:39] but I also understand like, if they're just doing it to keep animals in captivity,
[44:45] not as a rehabilitation, that is where I like cross the line.
[44:50] But I absolutely love zoos. My grandmother called Tyler on his birthday
[44:56] and he was like, yeah, we're going to the zoo. And the first thing my grandma says is he's like,
[45:00] or she said, she was like, did Jenny ever tell you that we used to go to the zoo
[45:07] every time we had to see her when in Phoenix and we rode on the camel?
[45:12] So my grandmother's 90 now. And she was so excited to tell Tyler
[45:18] that she and I rode on a camel in the Phoenix zoo when I was like five.
[45:24] - I just want to quickly acknowledge Abdullahi asking what we think of Ruby Rails versus Python in 2022
[45:32] and say that we are super sorry for the false advertising today.
[45:36] We actually decided midstream that this is no longer a Python stream.
[45:43] This is a Braindump Mondays stream and the Python stream is going to be on Fridays.
[45:48] 'Cause we have too much to say to each other that is not Python at the moment.
[45:54] - Yes. - So just going to call that out.
[45:57] We're sorry. - I also want to call out your next comment,
[46:03] which is come to Africa in the desert. You'll see animals live without a zoo.
[46:09] And yes, this is on my to-do list. I don't know if this is possible
[46:17] and this is something that I really do need to do research on.
[46:20] And I definitely need to own this is I really want to
[46:25] actually work at a elephant rehabilitation or like actually go be able to spend months there
[46:35] or like take a year off. It's extremely hard work,
[46:39] but not just go and visit as a spectator, but to actually help save elephants
[46:49] because they've been hunted for so long. And so, yes.
[46:56] And you said, I'm gonna probably butcher it. You said their name, right?
[47:07] How did you say their name? - Oh, I have no idea.
[47:08] I didn't get confirmation. I said, Abdullahi.
[47:11] - You said it right. They said that you said it right.
[47:13] They said, thanks, Laura. They love that you said their name.
[47:18] So say it one more time so I can say. - Abdullahi.
[47:22] - Abdullahi. Yes, Abdullahi, we 100% like want to just say
[47:30] thank you for showing up today and hanging out with us 'cause you were so right.
[47:36] And I keep trying to show up comments 'cause nobody else can see them but us.
[47:43] There isn't a park in Thailand. That's where a lot of people go.
[47:50] But I really, really want to be able to work with African elephants instead of Asian elephants.
[47:56] I know that their size is different. Their ears are different.
[48:00] I've done research on it before, but this is a story for another time
[48:05] because I will just go on like wanting to go research elephants nonstop.
[48:08] So I'm gonna click share my screen so we can actually look at this thing
[48:18] that people are telling me about. Mastodon.
[48:22] - Thanks for the high five, Ben. - Yay.
[48:32] So we can create account. Do you want to go over?
[48:37] - And I'm gonna go on a tangent again first. - Okay, cool.
[48:41] - 'Cause I don't want to forget. - Or we could write it on your list.
[48:44] And then talk about it later. - I mean, might as well go.
[48:47] I think tangents are fun. This is where I get my ADHD brain gets to thrive.
[48:52] So might as well. - So on the topic of name pronunciation,
[48:58] I got better at pronouncing names from cultures to which I did not belong because of my students
[49:09] when I was a math professor. And I used to have my students,
[49:15] and this got way better when we pivoted to remote and that will be clear in a second.
[49:22] I had them on the first day, I would link to like a YouTube,
[49:29] like how to pronounce Laura and ask all students, even if they thought that their name was,
[49:37] it was obvious how to pronounce their name. Not everyone comes from our culture either, right?
[49:46] And we had a lot of international students. And so I said, everybody needs to post a link
[49:51] to how to pronounce their name. And so I could, and then some students,
[49:54] their name, they couldn't find one. And they made me a little recording
[49:58] and I put them in my Anki deck. So I had an Anki deck for each one of my classes
[50:05] that I was teaching. And I had a card for each one of my students
[50:09] that had like what their name, it looks like on my roster, because that's how I would see them.
[50:16] And then how to pronounce their name. And you can actually embed YouTube videos
[50:22] and audio files in Anki cards, which is a total superpower.
[50:29] And then like their pronouns and like anything else about them, like, oh, they have a kid named,
[50:39] whatever, and this is their cat. And these are like things that are important to them.
[50:42] This one plays the sport and things like that. So that I could really quickly get to a point
[50:50] where my students felt like I knew them and I cared about them.
[50:55] 'Cause I did, I mean, care about them, you know? And it like really accelerated the relationships.
[51:01] - That is really, really cool. - In the classes.
[51:06] I learned how to side benefit of, I learned how to pronounce a lot more types of names.
[51:11] - I really like that. And that's, maybe we could start seeing if,
[51:15] see, Ryan, I like that you posted that. It's something that I do,
[51:22] that wouldn't make any sense to me. And this is why I get really nervous
[51:26] of saying people's names. This is so important.
[51:30] I think you bring up a really, really great topic of pronouncing people's names
[51:34] because that is discrimination when you like, if somebody is constantly correcting you,
[51:41] that is discrimination against them if you're not doing your best to do so.
[51:46] I, one of my best friends to this day, I still don't pronounce her name right.
[51:55] That is not something I'm proud of. I say this as,
[52:01] even when she says it and I try to repeat it, I still can't say it right.
[52:05] I don't know why. - So if you record her and you put it in an Anki card,
[52:13] you can practice it. If you want.
[52:19] - That's a good idea. - Just an option. - That's a good idea.
[52:27] - I Anki kind of all the things. - We do need to do another one of these someday on Anki.
[52:33] That's a really good idea. 'Cause she, like she's,
[52:39] she's cool with it in the fact that like, she knows I'm trying yet at the same time,
[52:47] it's not fair to her. - And how would you introduce her to somebody?
[52:52] - I say her name as Inas, it's I-N-A-S. And a lot of people say it that way.
[52:59] She, it's not the way she says it, but the way that she's described it to me before
[53:06] is she's from Libya and then went to Germany and then went to Canada and then went back to Germany.
[53:15] So the way she pronounces it, it can be a bit different than like,
[53:22] let's say somebody from Germany specifically or from Canada specifically.
[53:28] So I think that's a big reason that she's open to it. And now, can I give it a shot first?
[53:37] 'Cause you're really good at it. So I kinda wanna give it a shot.
[53:41] - I mean, go ahead. I don't know.
[53:43] I haven't actually seen this name itself, but I will infer from other names I have seen
[53:49] that were sort of similar. - I would take a gander at Abderrahman,
[53:55] Abderrahman, Abderrahman? - So I would say Abderrahman, very similar, Abderrahman.
[54:03] - Your sounds like a-- - I would assume that it would be a soft A,
[54:12] like ah instead of ah. - Yeah, yeah.
[54:16] - And that the M-A-N at the end would be like men, not man. - Ooh, yeah.
[54:24] - Yay, I did it. - Yay.
[54:28] - I'm like having a party for myself over here 'cause I'm a nerd.
[54:30] - Do it. - Do it.
[54:32] And that's actually something that's great call out because there was someone I used to work with,
[54:41] his name, I'm gonna say it wrong, is everybody would say,
[54:48] now I'm typing it. I'm putting it in the chat for everybody.
[54:56] It's, now I'm on, like we would all butcher it. I'm purposely butchering it.
[55:02] So the way that I like taught myself to say it better was Neumann is more properly said.
[55:11] And, but nobody at the company actually pronounced it right until we started correcting it and saying it.
[55:18] So that way, and he worked there for many, many years. So it's just kind of bananas how so many people
[55:24] have to put up with that. And it's practice.
[55:29] It is practice. And I like the idea of Anki, Anki, Anki, Anki.
[55:35] - I say Anki. - Anki.
[55:39] - I don't know actually. Ha, ha, I've never actually looked up how to pronounce it.
[55:44] - I get frustrated doing it. - Bye Ryan, thanks for joining us.
[55:47] - See you next time, Ryan. Thank you.
[55:50] I get frustrated with all of it, but yes. So we've got chapter one is good notes.
[55:58] Chapter two is name pronunciation and some elephants in there.
[56:04] We might put the elephants in there at 40 minutes. Oh, there we go.
[56:07] We can do elephants. - Names and elephants.
[56:09] - We got some chapters going y'all. We are getting the chapters.
[56:15] All right, do we want to. - Mastodon?
[56:22] - See, I waited for you to say it because this, I am horrible at sounding things out.
[56:27] Like this is just something I always struggled with. So now I'm just like, I hate reading out loud.
[56:33] I hate it with a passion. But hey, so it's so cute.
[56:43] Is it mastodon, mast? - Sure.
[56:47] - How did you say it? - Mastodon.
[56:51] - Mastodon, mastodon, okay. All right, do you want to explain to us what this is?
[57:00] - Sure, okay. - As a happy scroll.
[57:03] - I think it makes the most sense to explain it as we do it. - All right, then let me.
[57:13] - Because otherwise it's all just like a bunch of terms flying.
[57:18] And I think that that makes it sort of overwhelming. Okay, so the first thing that is different
[57:24] about mastodon from say Twitter. Oh, you know who has a really great explanation
[57:31] about how to think of mastodon is, oh, just a second, I'm gonna have to find her.
[57:42] Okay, well, so while I'm looking for this, you can search for a server by,
[57:49] just a second, I lost you tab. Okay, so, all right, so you've already got language,
[57:57] English, all regions. Okay, and so you can just choose.
[58:03] It sorta doesn't matter, sorta doesn't matter which server you choose.
[58:11] It totally doesn't matter in the sense that you just choose one
[58:15] and then you can choose a different one later and everything will be fine.
[58:19] So let's go with that, it totally doesn't matter. So let's just go through and see what there is.
[58:40] Oh, well, while you're scrolling through and seeing what there is,
[58:42] I will look for that super awesome explanation. And the problem is that I can't remember her name.
[58:50] So how am I gonna find her? Oh, I think I've retweeted, well, boosted.
[58:57] (Emmy humming) Discord.
[59:10] It's funny, my company used to have our work comms on Discord and so like the Discord sound makes me go,
[59:25] oh, somebody needs something. - Yes, and I still haven't like gone in and muted it.
[59:32] Like I said that I would go do this soon, but okay, I'm gonna find just a random one I can join
[59:45] that I don't have to apply for. - I'm gonna drop a link to this user's,
[59:52] this person's profile on (indistinct) with a super fabulous thingy.
[60:02] Oh, search, you could, have you already chosen a server? - No.
[60:09] - I think IndieWeb is full. So you can search, I think if you scroll up,
[60:15] oh, on the other tab, on the servers tab, I think if you scroll up,
[60:19] you can search more up. - Yeah, I'm just making sure I cleared out everything.
[60:25] - Oh, okay, cool. Oh, nope.
[60:28] Eek. - Well, do you know what topics there are?
[60:32] - There should be a search bar. I'm not, it's, I don't think so.
[60:36] These servers are like special, specially picked ones. Okay, try just going to the web address,
[60:47] fostodon.org, and then that's FOSS, as in F-O-S-S, free open source software,
[60:56] to-t-o-don.org, there we go. And--
[61:06] - It's currently down. - Oh, okay.
[61:09] Yeah, they were up yesterday. Okay, so this is everything in the Fediverse,
[61:17] which is Feddy's Federation, and that's not super important at the moment.
[61:21] At the moment, all we need to know is about Mastodon. Everything is run by volunteers.
[61:25] It's not owned by, you know, some billionaire or whatever. And so, and they've experienced massive influx
[61:36] from people fleeing Twitter. And so people have been putting in so much work,
[61:44] upgrading their servers to deal with more people, and like making sure that things are staying safe
[61:49] for everyone, because that's a really important ethos on Mastodon, is that everybody needs to stay safe,
[61:57] and so on. So there are a lot of servers that are like,
[62:03] they're just saying, okay, we're done for the moment. We need to fix some stuff.
[62:08] Okay, so, okay, so not this server, I guess, any other server, just pick one, doesn't matter.
[62:16] Yeah, I was just gonna pick a random one that, can I, no, legal structure?
[62:25] No. Instant.
[62:30] Okay, we're going back over here. Oh, I think I have, oh, yes.
[62:36] - Look at that bottom left one. Question others to teach ourselves a STEM-oriented server.
[62:43] Boy, does that sound like the place for you. (laughing)
[62:47] - I dig it. - Yeah, at the very least, it's a great place to start.
[62:53] - Okay. - I have to remember all my stuff, so hold on just a sec.
[63:04] (typing) And I agree, and I am human.
[63:19] Oh, I have to click images that contain a cacti. So in the sand, cactus in the sand,
[63:27] that is very specific for, okay. I got all my cacti in the sand.
[63:35] All right, and we go to Gmail, 'cause I have way too many tabs open.
[63:43] Bet that's how everybody lives. And verify.
[63:54] - I think ARC is going to have to be in like the next Brain Dump Monday,
[63:58] but speaking of everybody lives in a million tabs, that's not really what happens in ARC.
[64:04] - Oh, okay. - Any of you have Brain Dump Mondays to come?
[64:10] - Me. - All right.
[64:14] - All right, so sure, we'll allow notifications, why not? Welcome to the Fediverse.
[64:22] - Fediverse? - In a few moments, you'll be able to broadcast messages
[64:25] and talk to your friends across a wide variety of servers, but thisserverquota.org,
[64:35] Q-O-2-O-T-O, wow, .org is special. It hosts your profile, so remember its name.
[64:43] Get it. Home, posts from people you follow
[64:49] will appear in your home feed. You can follow anyone on any server.
[64:53] Local, public posts from people on the same server as you will appear in the local timeline.
[64:59] Federated, public posts from other servers of the Fediverse will appear in the federated timeline.
[65:06] I do love their graphics. It is really fun.
[65:09] - Right? - And then reply, you can reply to others
[65:14] and your own toots, which will chain them together in a conversation.
[65:20] Boost, you can share other- - So toots are like tweets, right?
[65:24] That's like a post on Mastodon is a toot because of the trunk, like, dude.
[65:31] - I like that. So we can boost them and you can favorite them.
[65:36] All right, oh wow. - Boosting is like retweeting.
[65:40] However, there is no quote tweet. And that is a very purposeful design decision,
[65:50] design choice, because it prevents pylons. So it's a safety thing.
[65:59] - What do you mean by pylons? - Like that's, so that's what happens on Twitter.
[66:06] So say you post something that says, Elon Musk is a fuckhead, 'cause he is.
[66:16] And then somebody searches, somebody, some Elon Musk fan is searching Twitter
[66:25] for anybody who says anything negative about Elon Musk, and then finds your post, your tweet,
[66:34] and then they quote tweet it saying, everybody go tell Jen that she's a horrible person
[66:41] because she thinks that Elon Musk is a fuckhead. And then all those people show up and they pylon.
[66:47] - Got it, got it. - That's what it is.
[66:51] - I've experienced that, which I feel fortunate for, so that makes a lot more sense.
[66:56] - Yeah, I am too tiny and boring on Twitter. And also, you know, I'm a white woman,
[67:07] so people are a lot less likely to pylon me, right? I'll just own that.
[67:14] - I just went to like being a 13 year old kid, so I'm just gonna keep moving on and say,
[67:24] so what do I do here? - Okay, okay.
[67:27] So everything is, your home timeline is empty because you haven't followed anybody.
[67:34] So I am going to paste my mastodon, so I can be your very first friend on mastodon.
[67:45] Where are we? Here we go.
[67:50] So if you copy and paste this, including the first at. - Insert.
[68:08] So it's kind of like discord with that. - There you go, there's me.
[68:13] And you click the like person plus, so you have now added me.
[68:18] - Now is it something? - Good.
[68:25] - Is it like Twitter where you can just like follow anybody or is it where you have to?
[68:34] - I'm really surprised to see that cancel follow request button,
[68:37] because I do not have... So you can make it there, like in preferences,
[68:42] you can change it so that people have to request to follow you.
[68:46] Oh, okay, it's disappeared. So I think that what it was doing was,
[68:49] it was processing your follow request, but I don't actually have that like wall turned on.
[68:57] Like there's no gate to follow me. So it just finished and now it's all good.
[69:04] Here we go. - So that wasn't the hardest thing to do,
[69:10] to set up. Where are people not liking this?
[69:19] I mean, it's not as pretty, I'll give it that. - The having to choose, oh, well, you know what though,
[69:23] that depends on which server you're on. So when I said like, it doesn't super matter,
[69:28] but then it really doesn't matter 'cause you can switch, the way that the UI looks depends on choices made
[69:37] by the admin of your server. So the first server that I joined,
[69:41] I didn't really like the way that it looked and it didn't have that nav bar on the right side.
[69:49] And I liked it. So my server is purple and stuff.
[69:59] It otherwise is identical, but it's purple instead of white,
[70:03] but it's also closed at the moment. So, yeah, that's a thing.
[70:10] - Interesting. - But yeah, so then the way that you find people
[70:17] on Mastodon is by searching for hashtags. So unlike Twitter, you can follow hashtags
[70:29] on Mastodon. - Kind of like all the,
[70:35] y'all I'm just setting this up while we're here as we're here.
[70:38] And then my avatar, I don't even know if I have a photo of me in here.
[70:44] It used to, they're gonna be somewhere. Cool, that's my D&D character.
[70:49] In case anybody wanted to know. - You can be a hippo on Mastodon.
[70:55] It looks like a hippo. - I can. The only reason I did it is because,
[70:59] oh, this is me trying to like figure out what photos. We'll do that one.
[71:02] That one looks nice. - I would recommend for the moment,
[71:05] for like the next few weeks at least, to use the same photo as you have currently on Twitter.
[71:11] So that people will recognize you. - That's a good point.
[71:17] And for anybody watching, that's a good branding point in general.
[71:21] That is the same. Like having the same photo everywhere
[71:25] does make it a lot easier for people to it. Make sure that know that you're you across platforms.
[71:32] And I am going to my Twitter profile really quick to go copy and paste it for my bio.
[71:40] That was super exciting. It may not look great, but hey, it's there.
[71:47] - You might wanna change the @ shit to talk about because that's a Twitter @ and so it won't go anywhere.
[71:54] Maybe I need to do it for here. Host of, that's a good call though.
[71:59] - You could probably just hyperlink that link to your podcast.
[72:15] - Probably will, but we'll do it later. This works.
[72:22] List the account directory, recommended. - Sure.
[72:27] - Profile metadata. Like.
[72:33] - So you can put in your website. Polly work, I have my Polly work.
[72:42] What else do I have? My Twitch.
[72:45] GitHub, I think I have GitHub. I like that.
[72:52] I'm just like, here, I'll just put all those in there.
[73:03] So give me a moment, please. - So the way that that verification thing on the right works
[73:11] is you have to be able to edit the HTML of something in order to do this verification.
[73:18] And so for me, the only one that I could edit the HTML for was my personal website,
[73:23] but you don't have to do the verification thing right away. You can later.
[73:32] - I just realized. - And so that's how verification works on Mastodon.
[73:39] Nobody can verify you except you. - Nice.
[73:44] All right. Oh, guess what?
[73:48] I'm going to be emceeing next week. Or the, let me copy and paste that one really quick.
[73:58] For Next Nation is the conference and I'm either emceeing both days or just the second day.
[74:15] I'm not sure which yet, but it's free.
[74:19] So y'all should go and come hang out with me. It would be fun.
[74:24] - Cool, cool. - And we are almost done.
[74:27] All right. Save changes.
[74:46] And we have to continually remind ourselves that, what doesn't it like?
[74:57] - Oh, must be less than two. - Oh, your header file was too big
[74:59] or your avatar or something. Both of them.
[75:04] - Both of them or just the second one? - Looks like it's both.
[75:09] - Oh, okay. - I don't know.
[75:12] At least the header one has a broken image icon. - Yeah.
[75:17] - Please stand by while I work on doing this, but please continue.
[75:20] - We have to continuously remind ourselves that these servers are under unprecedented pressure
[75:30] and maintained by humans who don't get paid to maintain them.
[75:36] And so sometimes stuff is really slow. It's getting better.
[75:44] And the way to help that is to donate because servers cost money.
[75:49] So, yeah, sometimes stuff's slow. - That is a good reminder.
[75:59] That is definitely a good reminder for us. - We need to grant grace to these humans
[76:05] who are putting in all this effort to make this thing for us.
[76:13] - I'm making my photo smaller. Please stand by.
[76:19] Wee, Snagit, yay. Snagit is an amazing app if anybody wants to know.
[76:33] - Cool. - It is an app I use all the time.
[76:38] Where's my desktop? There it is.
[76:40] Oh, you're still 2.7. Oh my God, okay.
[76:46] File, edit, export. - In case anybody wanted to know,
[77:04] this is the really exciting part of it all. - You know what you could do that might be a shortcut
[77:10] is if you go to your own Twitter profile and then just right click on your avatar on Twitter
[77:17] and save that and use that, I'll bet it's already small. - Sweet.
[77:23] - And so here's a really good question. I don't know if I can like elevate that.
[77:30] Can I? Ooh, I can.
[77:33] Who are the admins of the Mastodon servers? Are they private citizens or companies?
[77:36] They are private citizens. So, and they own their server.
[77:42] And so what they say goes. And so different servers have different rules.
[77:47] Like some servers will have rules about you can't talk about Nazis on here, for instance,
[77:53] and other servers may not. However, as a group, the Mastodon part of,
[78:02] at least the Mastodon part of the Fediverse did actually get together a few years ago,
[78:09] as I understand it, when some alt-right types tried to come in and like make servers.
[78:15] And they were all just like, "No, this is a Nazi-free zone.
[78:19] "In fact, goodbye." Are servers connected
[78:26] or is every server a closed community? Okay, and so this is where that middle tab, Dr. Casey,
[78:37] Fisler one is handy. - Repost in here.
[78:43] - If you scroll down, she may have it. Oh, she doesn't have it pinned.
[78:53] Darn. Okay.
[78:56] - Is it a tweet or a video? - Oh, try that, the thread reader app, I think.
[79:04] - Okay. - So this is a really great, not super short explainer,
[79:13] but the TLDR is imagine, so like if you go to school, you can be, say you're a freshman in,
[79:27] you're a year nine or whatever student, and then you can join clubs
[79:34] and those clubs can have students from other years. Like you might have year 10, year 11, year 12 students
[79:40] all in the same club together. You do have to be a student at that school
[79:45] in order to be part of any of these clubs. So you, and the sort of analogy,
[79:51] the Mastodon part of the analogy is like, you have to have an account on a Mastodon server
[79:57] in order to connect with people on other servers, but you can connect with people on other servers.
[80:04] You are not restricted just to the server to which you joined.
[80:08] Just as if you are a year nine student, you are not allowed, it's not the case
[80:12] that you are only allowed to be friends with other year nine students.
[80:15] - I think that makes sense. Discord really helped me understand.
[80:27] I think that's why it makes a bit more sense to me is because Discord, in Discord you have to join
[80:35] a specific server to be a part of that like group, but you can still DM people if you know their full server,
[80:43] username and server. So it's, but okay.
[80:49] To my mind, it is completely the inverse of Discord because like when I go into Discord,
[80:59] in order to see updates, I have to look in each server one at a time.
[81:08] I'm only ever looking at one server. I'm not looking at like, here's everything
[81:11] from all of the 27 Discord servers that I belong to. That's Mastodon.
[81:18] - Oh yeah, I agree. I think I just don't look at each server like ever.
[81:26] I just do my DMs to people because I'm like, oh, I know where to find you now.
[81:31] Is it like IRC, it's IRC. - It was a, well, is a chat, like internet chat thing.
[81:43] Internet relay chat it might be. I'm sure that this IR is internet relay
[81:49] and I'm not actually sure about the C, but I kind of, I want it to be to chat.
[81:52] - Well, you explain, I will Google. - Oh yeah, yeah, yeah.
[82:01] So Mastodon is federated. That's why it's called the Fediverse in fact,
[82:04] because it is federated exactly, sudo. So internet relay chat, I got it right, right.
[82:11] Yeah, so it is kind of like that in the like federation sense, yeah.
[82:20] - Huh, huh, all the learning. - Yep.
[82:26] Did you have ICQ a thousand years ago? Okay.
[82:36] - What's ICQ? - Oh look, there it is, ICQ, the little, little,
[82:40] it's there actually. It's the one with the little green, yeah.
[82:46] - You still remember your number, sudo? Oh, that's cool.
[82:49] I don't, I don't know mine, ICQ. - I don't think I ever really...
[82:58] I think a lot of it is also, okay, let me think. What would a, because this would not be like AOL chat.
[83:16] This is more. - No, AOL chat, AOL instant messenger would be like Twitter
[83:23] because you had to be, you had to have a, like an AOL account.
[83:28] Like you had to be in the AOL world. - Okay.
[83:34] - And you could not talk to people who didn't, who weren't in AOL world.
[83:38] - Where? - On Twitter, you can only talk to people on Twitter.
[83:42] - Where IRC, you can talk to anybody even if they don't have IRC?
[83:47] - Well, it's because IRC, like ICQ is a client that I think was, I think it was an IRC client.
[84:02] But anyway, it's like, it's, if you think about like email, like if you have Gmail,
[84:08] you can email somebody who has Outlook. - Yeah.
[84:12] - And they can email you. It's not the case that you can only email people
[84:17] who have Gmail. - Okay.
[84:22] - Whereas with AOL instant messenger, you could only talk to people
[84:26] who were on AOL instant messenger. - So would these be like, no, because chat rooms,
[84:32] you would still have to have a like a name or account with that chat room to use it.
[84:40] ICQ changed the content ownership policy at some point where everything you wrote on the platform
[84:48] would belong to the platform. That's when a lot of people quit.
[84:53] That totally makes sense. I think I'm a little lost because I was more in chat rooms
[85:00] and AOL than this. I didn't even know this was really a thing.
[85:06] - Sure. So you can just think about it as like email.
[85:11] In order to email, you have to have an email client. Like you have to have,
[85:16] you have to be registered on somebody's email server, right? But you can email people whose emails are on other,
[85:25] whose email accounts are registered on other servers. Yeah.
[85:30] - Okay. - That's what Mastodon is like.
[85:35] You have to be registered on somebody's Mastodon server, but you can still talk to people
[85:42] who are on other Mastodon servers. Like me, you and I are not on the same Mastodon server
[85:47] and we connected. - And then, oh, that's where, okay.
[85:57] I was going in, look, I have it, yay. I just posted mine in here too.
[86:05] And then I will post Laura's in here. So y'all can go Mastodon it up.
[86:15] Oh, I just pasted it back to you. That doesn't really help.
[86:19] Wrong, you know, there we go. I would say that I've gotten a lot of knowledge drops today
[86:28] and this is why I absolutely love that we have our Mondays now
[86:32] because even though it's very, very random, I always learn so much.
[86:38] - Yep, yep. So couple more points.
[86:42] So just like if you're going to email somebody, you have to put like their username at their email client.
[86:51] - Right. - Like I'm, you know, me at Gmail or whatever.
[86:56] You can't just say like, I'm going to email Laura Langdon. - Right.
[87:01] - It'll be like, cute. Same thing.
[87:04] If you are looking for somebody who's on your server, you can find them with just their username.
[87:11] But you can't find someone on another server with just their handle.
[87:17] It has to be the whole, like that thing adds server's name. That's one thing that people trip over.
[87:25] - I think that's why I still relate it back to Discord 'cause you can't just find someone with their name.
[87:32] You have to friend them. You have to have their server number too.
[87:37] And that's why I think I keep associating the two is just that one aspect.
[87:42] - Yeah, whatever works. Yeah, everyone has different mental models of stuff.
[87:47] - That is true. - So that's one thing that people find confusing
[87:51] because on Twitter, there is only one server from that perspective.
[87:57] So you can find somebody because you're only looking on Twitter
[88:01] and nobody can have the same username on Twitter as somebody else.
[88:05] But just as there could be someone who has like Laura Langdon at yahoo.com, and that isn't me.
[88:16] Actually, that was me a million years ago. But anyway, that's the same idea.
[88:21] You can have somebody else, like the same username as somebody else
[88:24] on a different Mastodon server. - And that makes sense.
[88:29] - That's why you have to include the server name. - And Hi Vive and Sudo asked,
[88:37] what happens when my original server goes offline? Can they still log in to Mastodon?
[88:45] - Mastodon. I don't actually know,
[88:49] but there are all kinds of fabulous Mastodon explainers out there.
[88:54] Actually, if you go to fedi.tips, F-E-D-I.T-I-P-S, that website is full of answers to all of these questions.
[89:07] Fedi being short for Fediverse because of federation. - Dope.
[89:18] - Okay, so that's one thing that people trip up on. - Okay, wow.
[89:22] - Another thing that people trip up on is Mastodon, if you search for a word on Mastodon,
[89:28] it does not search text. So it's not going to be searching,
[89:34] like if you search for Python or whatever, it's not going to find everybody who has posted containing,
[89:43] has written a post containing the word Python. However, you can search for hashtags.
[89:49] And so people use a lot of hashtags in their posts on Mastodon, if they want people to be able to find them.
[89:56] And if you don't want people to be able to find them, you just don't put in hashtags
[90:01] and then people can't find them. So it'll only be visible to like the audience
[90:07] that you select. - Sweet, that one, I feel like that's kind of how I write
[90:13] my tweets, 'cause I'm like, I don't go search for it. But then I realized like Squarespace,
[90:20] I didn't tag them in something, I just used the term Squarespace
[90:23] and they actually replied to my tweet, even though I didn't tag them or hashtag them.
[90:28] - Because they were looking for the word Squarespace. - Yeah, so, okay, cool.
[90:33] I'm pretty excited about this 'cause apparently my mind-- - So you can search for hashtags,
[90:36] which means it actually has to have the hash, right? The like pound sign, hashtag symbol.
[90:44] That's another thing that people trip over. The third thing that people really have trouble with
[90:50] is signing up on mobile. - Ooh, okay.
[90:56] - Because when you download a mobile client and there are different ones,
[91:03] there are several different ones for iOS and there, I think Tusky is the one that people,
[91:09] that's the one I see that recommended the most often for Android.
[91:12] Capital T-U-S-K-Y. What was I gonna say?
[91:22] Oh, a lot of them say like, it looks like you have to rejoin.
[91:28] It'll say like, join a server and you're like, but I already joined a server,
[91:32] why are you asking me to do this again? You just search for the server name
[91:37] that you're already on. And so in your case, that's what, Q-O-T-O dot something?
[91:45] - Dot org. - Dot org, okay.
[91:48] And so you would search for that. And it'll start, like sometimes it'll start,
[91:53] my husband ran into this yesterday. He's on Fostodon.org and he started typing Fostodon.
[91:58] It started off like auto-populating the search results and then they all just disappeared.
[92:05] And he was like, oh, okay, so I guess it's not here. But if you actually just press enter and like do the search,
[92:11] then it found it. - Got it.
[92:14] - So you do have to actually search for the server that you just joined.
[92:17] And then you can log in and everything's like normal. But those are like the three, I think,
[92:21] things that people find the most confusing. - That is good to know.
[92:25] And I wrote these down. So I'll include them in the YouTube description.
[92:32] And y'all, we put in a hashtag TeachGenTech. So you guys can search it later.
[92:38] And also, I'm also kind of rushing y'all 'cause I really have to pee.
[92:45] TMI for everybody, but I'm like, I drink a lot of water. So I'm like, let's go.
[92:52] We are also at our time, which is pretty exciting 'cause that works out.
[92:56] And yes, as y'all heard, we are just gonna do as homey put Manic Monday or Brain Dump Monday,
[93:04] or this is just like a chill, get the week started with us. And every other Friday, we will be doing
[93:13] Learning with Laura, specifically Python. And not--
[93:17] - Is that starting this week or next week? - Next week.
[93:20] - Okay. - This week is TypeScript with Josh.
[93:26] And you know what will be really cool is I felt, see, I feel like Laura's gonna do this someday.
[93:32] - Laura, you will. Josh has a TypeScript book.
[93:36] (both laughing) So we are going through books.
[93:38] - We are already Python books. - You're gonna write something that I'm gonna be like,
[93:44] let's learn about it. - Yeah, I have to write a book
[93:47] because it's like a rule in my family, but I'm not sure what it's gonna be yet.
[93:52] - That's okay. I have a feeling it's gonna be something about math.
[93:55] - It could be. - It could be a math student, a math professor.
[94:01] A mathematician. That could just be the character.
[94:06] Or it could actually be-- - Oh, like a novel.
[94:08] Oh no, I don't think I'm writing any fiction. - It could be an autobiography.
[94:14] You're a mathematician. You math better than I do, so I'm gonna go--
[94:21] - I'm not like a practicing mathematician. But--
[94:25] - I like Suda's idea. - Oh.
[94:27] (both laughing) - Teaching tech.
[94:30] - Yeah. - Yes, because learning with Laura
[94:33] has truly helped me with learning techniques. This is stuff that I never learned growing up, so.
[94:40] - Oh, and the same. It's all stuff I learned as an adult too.
[94:43] - Yes, and thank you. - Thank you for sharing the wealth.
[94:46] - So y'all, until next Monday with Laura. And this week, I don't have as many guests this week.
[94:55] Who do I have on the show? We had a couple cancellations, which is cool,
[95:00] 'cause that is the cool thing about streaming is, oh, the next guest is gonna be on Friday,
[95:07] which is with Josh on TypeScript. But I will be streaming tomorrow and Thursday
[95:13] about a couple of projects I'm working on. - Yay.
[95:16] - So I will be here. - But y'all are too kind.
[95:18] - Thank you, everyone. - Thank you.
[95:20] - I gotta go find somebody to rate to, and then kill the stream.
[95:25] I always forget about that. I'm like, you know, rating to people is just,
[95:30] you find cool people. - Oh, while you're looking, I'll say one other thing.
[95:37] - Do it. - There is etiquette on Mastodon,
[95:41] which you can also find on the Feddy.tips site. There are like ways that it's nice to behave on Mastodon.
[95:55] Yeah. - It's different than, I don't know,
[96:00] just being a nice human. - There are some fairly specific things,
[96:07] like alt text, for instance. Mastodon had alt text for images like years ago,
[96:14] whereas Twitter only got it like sometime in the last, maybe 18 months.
[96:19] There's a very strong alt text culture. - Cool, I like that.
[96:25] - You don't just write like, oh, this is a picture of, you know, like you're maybe writing a paragraph.
[96:32] You're not just writing like a few words about what is in the picture.
[96:34] You're really describing the picture. - Yay.
[96:38] - Yes, yes. And also content warnings are a big thing.
[96:44] And they actually, if you use content warnings, that's actually like a feature,
[96:48] not just like you type CW and then, you know, whatever. It's like a button on a post.
[96:55] - That's cool. - And it will actually, like,
[96:58] it's not visible unless you click it. Like you opt in to see what's behind the content warning.
[97:07] And there are content warnings for things that you might not expect, like politics.
[97:11] It is not polite on Mastodon to talk about politics without putting it behind a content warning,
[97:17] which I would never have intuited. - That's pretty cool.
[97:21] - I needed to be told. I mean, I read it, nobody yelled at me, but yeah.
[97:27] And people are nice on Mastodon. Like the default is that people will be kind to each other
[97:34] and not like snarky or mean or whatever. It has a 100% different feel from Twitter.
[97:43] I was super sad about Twitter. And now I'm like, it was good time.
[97:49] And this is kind of a better one. - I dig it.
[97:53] And on that note, I'm gonna click the rate now. So y'all are getting rated, but we have the content.
[98:01] It will be on YouTube. And on that note, I'm ending our stream.
[98:06] So thank you, Laura. Thanks, Jen.

