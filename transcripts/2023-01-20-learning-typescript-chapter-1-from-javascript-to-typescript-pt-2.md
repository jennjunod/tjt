---
showLink: "https://www.youtube.com/watch?v=K710B5oMYAU"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-typescript-chapter-1-from-javascript-to-typescript-pt-2"
title: "Learning TypeScript Chapter 1: From JavaScript to TypeScript pt 2"
publishDate: "2023-01-20"
coverImage: "https://i.ytimg.com/vi/K710B5oMYAU/maxresdefault.jpg"
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

[00:00] - Hello, hello, beautiful humans. Welcome back to another episode of Teach Gen Tech.
[00:06] And hey, we are finally, finally, mostly because of me,
[00:11] going back and doing learning TypeScript with Josh Goldberg.
[00:15] All right, so it's been a hot minute since we have been streaming.
[00:27] Like, oh gosh, has it really been two months? - Two months. - I think it might be
[00:31] two months. - Yeah, it was like mid-November.
[00:35] - Oh, wow. - Give or take. - Yeah, and there's been a lot of learning since then,
[00:41] at least on my side. I mean, you already know all of TypeScript.
[00:44] You wrote a book. So I'm like, hey, you know a lot of this coding stuff.
[00:49] I feel like there's been a really, really big shift for myself, which was learning that I, A,
[00:59] don't do things offline very well at all. Like, if I have homework,
[01:08] I'm not always as keen to do it if, you know, I'm not streaming, which isn't a great feature of myself,
[01:19] but you know, it's a thing. At least I've learned.
[01:22] And the other part is learning how, and I put a lot of thought in this
[01:28] because we're gonna be starting the Python stream back again as well,
[01:34] is how are we gonna structure this to make it consumable? And for myself, that had a lot to do
[01:45] with how we approach this and really making sure that we break it down because I went through an experience
[01:57] where I was kind of shut down and I was like, I'm never doing this.
[02:05] And I hate that other people have been shut down and they may not know how to build the same relationships
[02:11] like I have, or always feel like they want to reach out to other people.
[02:16] So that being said, you are an expert in this field. And I'm curious, before we dive into like setting up
[02:25] everything for learning TypeScript itself, can you introduce yourself a bit more
[02:31] and also tell us like, what would you tell a newbie and how would you tell newbies to maybe approach this?
[02:40] Because I know that not everyone is like up in everybody else's grill going, hi, talk to me.
[02:48] Because I, and shout out to Ben, thank you again for another subscription, yeah.
[02:54] - Yeah, Ben. - Okay, Josh, all you now.
[02:58] - Cool, hi everyone, good to be back. Good questions.
[03:04] I'd say it's hard to get intent across correctly on the web and also some people aren't accustomed to that.
[03:16] So sometimes a very reasonable help request is incorrectly received as a, I haven't done any work,
[03:24] please tell me everything request. And I think it's on the person who is more knowledgeable
[03:30] in the area to try to assume like, okay, that's probably not what they're asking.
[03:34] Like maybe I should re-evaluate like what they're actually asking,
[03:38] which is my fancy way of saying, I think someone getting shut down for asking for help
[03:43] is a bad thing, I don't like that. - That is a great point.
[03:48] That is a great point because I know for myself, a lot of it has to do with not necessarily knowing
[03:57] how to ask the question. And which it may seem like I'm not,
[04:04] that I didn't do the homework. But a lot of times it's me going,
[04:08] hey, I don't know how to Google this 'cause I don't know the terms, but could you just like,
[04:12] I don't need you to do the work, I don't need you to necessarily like,
[04:16] explain the entire thing, but for example, I spent like three hours trying to update my terminal,
[04:27] like to my home directory. It's like four hours and I'm like trying all this stuff
[04:35] and I'm like lots of Googles and I'm looking for it on an app called Hyper
[04:40] and I'm looking at it for like Mac OS. And so I finally was like, okay,
[04:47] I'm gonna ask my D and D smarties because they know what's going on
[04:53] and they're in this world and the reply from Roy was, I'm pretty sure you're using, is it called,
[05:04] do you say it out loud as Zish, Z-S-H? He's like, I think you're using that and not Bash.
[05:10] He's like, just try these two things to ensure you're using this
[05:13] and then you should be able to Google it. He solved five minutes worth of knowledge.
[05:23] Like it took him probably two minutes to reply to this. The three hours it took of me Googling it
[05:29] and not getting anywhere. And he was able to see that I was just incorrectly
[05:34] trying to Google it because I don't know it. And that's, I think one of the hardest things to your point
[05:40] that people are like, yo, why are like, why are they asking?
[05:45] And it seems really overbearing. Like they're not doing the homework.
[05:48] And hello, homie, happy to see you. So how do you, would you suggest to newbies
[05:58] to maybe show that they're doing more of the work or also to people being asked that to be a bit more,
[06:08] I guess, kinder or empathetic when answering the questions to not be like, yo bro, you haven't done shit.
[06:16] So I'm not gonna answer you. - Those are two very good questions.
[06:20] For the first question, for newbies to show off that they've, show off, to show that they've done the work,
[06:28] it might help to give the high level summary of what you've looked at so far
[06:33] and how much time you've spent. In the case that you just described of,
[06:38] I can never remember how I like to pronounce this. Let's say ZSH or Bash.
[06:42] Say, okay, I've been trying to do this, whatever, upgrade Bash.
[06:46] I've Googled around these types of phrases. I have tried switching apps.
[06:51] I'm on whatever Mac or Windows, XYZ, Linux, and it's still not working.
[06:56] Here's how it's not working. Could you please help me?
[07:00] So especially when I worked at a corporate job and had people coming to me for help,
[07:07] I would always ask first, what is the stuff you've done already?
[07:10] Because I don't want to assume they've done nothing. I just want to know what they've done
[07:14] so I don't repeat myself. And also I've found for myself especially
[07:19] and anecdotally from other people, having to say what I have done so far,
[07:24] oftentimes makes me realize, oh wait, I haven't done this particular thing
[07:28] that I know I probably should now that I'm thinking about it.
[07:31] So it's both helpful for the person you're asking for help and helpful for you as the person asking.
[07:36] How does that all sound? - Yeah, and that totally makes sense.
[07:40] And something that Homie said, Googling is hard when you don't know exactly what to Google.
[07:47] A hundred percent. Like I was Googling Mac stuff
[07:52] and yeah, or hyper stuff. And to be honest, I thought I was Googling Mac,
[08:01] but it might not have been, but it didn't occur to me that there was something else
[08:06] like Bash versus DSH. Like I knew they were two things,
[08:12] but I figured it would just like, no. Google doesn't know, you have to break it down.
[08:17] And I think that's a really good call out of how to tell someone when you're asking for help,
[08:22] but also how to reply when someone was asking for help of just what have you done so far.
[08:32] - Can I say that? Because with my experience that I went through recently,
[08:36] I did put, I was really stuck on an image and I put, hey, I tried this article,
[08:43] but I'm still really stuck and I don't know why I'm stuck on this.
[08:47] And then replying back with the article that I already just tried.
[08:50] - That's just disrespectful. - That's not helpful.
[08:56] And I bring this up because I really want Teach Gen Tech show to become accessible for everyone
[09:03] and make it so that way people can learn and aren't like scared of asking these questions.
[09:10] And also for people to really learn that it's, yes, it can be very scary and frustrating
[09:18] and to be able to go and get into tech, but it is very, very, there are so many dope humans
[09:27] that want to be able to help. It is very time-consuming to help one-on-one.
[09:34] So how do we start changing these conversations from the very beginning?
[09:39] And what up Dev? Dev is joining us from YouTube.
[09:45] We're also streaming on Twitch, which is where a lot of the crowd is at.
[09:49] If you want to join us, I will figure out how to link my Twitch.
[09:56] I can do that. And then also Ben brings up a great point
[10:02] of accessibility or a great, yes. I did say accessibility,
[10:12] 'cause I think it's so important of not only captions, which by the way, y'all on our YouTube on MISC Mondays,
[10:25] oh, I'm clicking things. On MISC Mondays with Laura, we are talking about OBS
[10:30] and Ramon has been joining us to talk about doing live captioning,
[10:35] which I think is really great and something that would be so helpful.
[10:39] StreamYard doesn't have that as of right now. But anyway, with that side note over,
[10:45] let's move on to, so we have this really cool book
[10:52] and this cool project that we're gonna be doing together of going through your book
[10:56] and learning some things about TypeScript, which I'm very excited about.
[11:02] And I'm not gonna have us go through the entire book again of like what chapters are there or anything like that yet,
[11:08] because these are all, we went through it a few months ago. And what I really want to do is set up a repo in GitHub
[11:17] that has the readme, talking people through it, talk about why readmes are so important
[11:24] and then work backwards of, hey, so we're gonna try chapter one's project,
[11:33] see what we can do without knowing anything about it and then kind of pick apart the chapter from there
[11:40] because something that I've learned in my own learning is without live application,
[11:47] it's very, very hard for me to learn the fundamentals if I don't know where they go,
[11:52] which is very frustrating because this is why people tell me,
[11:57] I get why they responded, "It would help if you learn the code."
[12:01] I know it would. I want to, I want to learn the code.
[12:06] I just am not great at learning the fundamentals. I like doing big, really difficult things first.
[12:13] So how does that sound to you? - That sounds great.
[12:18] I think whatever way you approach it, whatever direction you come from,
[12:21] whether you're going from the foundations and applying them to the code
[12:24] or using the code as a way to figure out what foundations you need,
[12:28] these are all very valid, good ways of learning. So I personally am opposite from you.
[12:33] I try to do foundations and then apply to code when I'm learning a new language and I'm really excited.
[12:37] I think this is a good matchup that we're each coming at it from a different direction.
[12:41] - And yes, everyone, my dog is being really annoying again today.
[12:45] So I will be randomly trying to stop her from licking her paws.
[12:51] And yes, this is a conversation that Josh and I had a while back as well,
[12:57] because every other Friday is learning TypeScript. Every opposite Friday is learning Python
[13:08] with automate the more and stuff. And a lot of people would say,
[13:12] "Don't learn two languages at once." Yet learning two languages at once
[13:18] have really been helpful because then I can actually understand
[13:20] what the differences are, what's something that's in JavaScript or TypeScript
[13:24] or something like that compared to Python and when people talk about them.
[13:29] So it's, again, this is all for somebody, your own learning practice, the way you learn.
[13:34] I am curious for everybody listening, watching, or if you're watching afterwards,
[13:40] I would love to see this in the comments. How did y'all learn?
[13:45] Did you go fundamentals first? Did you just say, "Hey, I want to build a website.
[13:48] "So I'm going to just go figure it out as I go." How did you learn to code?
[13:52] And, okay, while we get that set up, I am going to get our...
[14:11] All right, so teach.yantek has an org now in GitHub. It's very, very exciting and somewhat new
[14:19] as of like earlier this week. And I will link that down here for us.
[14:26] Oh, that's such a good one. Coffee said, I had to look at that for a second.
[14:40] I'm like, there's letters and words. And I'm like, I know what this says.
[14:44] '80s computer bought at a garage sale and started playing. I love that.
[14:50] And Dev said, "Learned by practice first, "fundamentals later."
[14:57] All right, I dig it, I dig it. Okay, so I'm not going to go too much
[15:05] into like GitHub and things like that because those are, yes, if you want to learn more,
[15:11] we can do more videos on this. This is something we've done before.
[15:15] And it's always a balance of when making content, if anybody's curious about this,
[15:21] of how rudimentary you go. Like how beginner friendly do you go?
[15:31] Because if you don't build upon it, then people aren't going to be learning with you.
[15:36] If you go back to the very beginning every time. So I will link that line really quick
[15:42] of just some fundamentals of GitHub that I did with Rizal,
[15:48] who is one of GitHub's developer advocates. See if I can talk.
[15:54] Developer advocates. And this was when I was a baby learner myself
[16:06] because I am pretty sure this was my third or fourth stream. But you can also see what the differences are
[16:18] since I first started. All right, so we're gonna go into Teach Gen Tech
[16:24] and create a new repo, maybe, yay. And we're gonna call it Learning TypeScript.
[16:34] Curiosity, I don't know if it does this, but does anyone do camel casing on this?
[16:46] Does GitHub actually see camel casing? - I tend to do like uppercase letter firsts
[16:59] in languages that tend to do that. Or for like for some projects,
[17:04] and it will like know that that's the normal canonical URL, but it'll still work if you do the lowercase.
[17:11] So I've always been kind of nervous about that, of like, in what case will it not work?
[17:15] - Okay, okay. Oh, I didn't even know that had a name.
[17:21] GitHub saves capitalizations. Ben prefers kebacase, so Learning TypeScript,
[17:29] so the dashes. - Kebab, because it looks like a kebab,
[17:32] or the letters are the little, whatever vegetables on your stick.
[17:35] - I didn't know that was a thing. - Okay. - Makes me hungry every time.
[17:43] That's the only reason I wouldn't want it. And yeah, I still do it a lot.
[17:47] Plus one to kebab case. Also plus one to Ben as a human.
[17:51] Yes, yes. All right, and okay,
[17:56] something that I just am curious about for everyone. Some people have told me, like,
[18:02] you always add a gitignore. Some people have been like,
[18:05] nah, you don't really need to add a gitignore. Like, what's everybody's preference on this?
[18:11] - Privilege of being an audio live person. I can go first.
[18:21] I normally add a gitignore if there's anything that I know the repo is gonna build
[18:25] that I don't want checked in. Like if I'm doing TypeScripts,
[18:28] TS files become JS files, but you don't really need to check those JS files in.
[18:32] So, that. But if I'm just doing like a markdown repo,
[18:35] just like a bunch of markdown or text documents, eh, I'd bother.
[18:40] - Okay. So would we just do JS files or type, like,
[18:45] would we leave the JS files or would we leave the TypeScript files?
[18:51] - You'd leave the TypeScript files. Those are the source code.
[18:53] And then there are built outputs, which in this case are JS files.
[18:57] So if they have a TypeScript option in there, that would be nice,
[19:00] but I don't know. - Yeah, they don't. - Oh, well.
[19:04] - Hey, you should talk to GitHub about that, Mr. TypeScript. - I'll get right on it.
[19:11] I'll use all my high level network connections in the industry to affect this change,
[19:16] because that is something I can definitely do at this stage of my career.
[19:20] (laughs) Okay, we'll leave it blank for now.
[19:25] I'm gonna leave the license link for now. We can talk about that another time.
[19:30] And Coffee said, "Maybe depends on tooling,
[19:36] "like if I'm gonna use an IDE that will have junk "I don't want in the repo."
[19:44] Good point. And then also,
[19:47] I think maybe I'd spin up a repo and then add and get ignored later.
[19:52] That's what I've been doing a lot of, is adding a lot of this post,
[19:56] 'cause I'm just like, "I just need this to go right now
[19:58] "and I don't wanna think about all of that, "'cause I just wanna get going."
[20:03] What, whoa, homie coder, are we good? What are we good about or not good about?
[20:18] For those who don't know, homie is like one of the dopest people I've ever met
[20:22] or talked to. Do you say met if you haven't met them in person?
[20:27] I don't know. Josh, have we met or have we?
[20:35] - Oh. Oh, both to the chat thing.
[20:41] I'm guessing it was like a misclick. I don't know if we've met.
[20:44] If like, if what we have, if this constitute as meeting.
[20:47] I know people say nice to e-meet you in emails, which I've always been like, eh, as a phrase.
[20:54] - Oh. Yay, thank you.
[21:02] So as a total side note, I feel very, very fortunate to have people,
[21:09] especially those who are streamers, but also those who know how to deal with,
[21:16] like meanies or creepers. And so Ben and homie are both moderators
[21:24] and they were messing with the, you know, cool chat features that I barely,
[21:29] yesterday was the first time I had to block someone and it took me like seven tries
[21:32] to try to like figure out how to block them as much as I, so moderators are the best.
[21:39] And also to get back to what you were saying, I think that, I don't know,
[21:45] especially when you talk to someone a lot, like I'd be like, I feel like I know them
[21:50] 'cause I talk to them a lot. We just like literally haven't met in person.
[21:56] Anyway, enough of that. So I'm gonna set up this README to start with.
[22:04] And this is probably my favorite part about Markdown is it is very, very friendly
[22:14] at just drag and dropping images because I, and it does everything for it.
[22:23] And ta-da, look, our faces are on it. Coffee.
[22:35] Yeah, it was all you, coffee. You know, I'm just kidding.
[22:41] Wait, would it be if people didn't get enough coffee, maybe something was wrong?
[22:47] Eh, anybody, anybody? No, okay, you know, I like my cheesy puns.
[22:56] So biggest things that we are going to do, learn, learning, and y'all can totally make fun
[23:05] of my TypeScript, that may take me like seven times to figure out learning TypeScript.
[23:10] We need to get Goldberg, Goldberg. I'm not gonna lie, I have actually like had to go,
[23:25] and I might even do this right now, of going and looking and seeing how you spell your last name
[23:33] because I'm like, is it Goldberg? Is it Goldberg with a U?
[23:37] Is it, like, I second guess myself every single time when trying to figure out what to say.
[23:45] - I'll give you a tip that you will never forget that will help you spell.
[23:49] It is like iceberg, but gold. Which is, I'm told, so stupid of a tip
[23:57] that people remember it. - Or you're a golden iceberg.
[24:01] - That. Okay, so learning TypeScript.
[24:09] And biggest things we're going to do is, and for those who don't know,
[24:16] you can go back and forth from edit file over to preview to see how it's looking.
[24:23] And one thing that I just really want to link here, or put here, are all of the links
[24:30] that we use on a regular basis, which is going to be,
[24:37] yeah, is the website, which, I'm trying to think of how to put this.
[24:50] (laughs) That's what I was thinking about when he said it.
[25:00] (laughs) Ben saying, Josh Goldberg over here,
[25:08] like, "I'm going to sink the Titanic, but gold." Yes, yes.
[25:14] I dig this, I dig this. All right, so we will,
[25:21] I feel like I just want to link the, but there's the starters, the books, right?
[25:30] We'll do projects. I'm going to clean it up in a second, y'all,
[25:38] before you yell at me about my markdown. And then,
[25:43] what would you call this? - It's a page?
[25:57] Like a chapter landing page? I never really figured that out.
[26:02] - Yeah, 'cause I feel like this is a big reason that I want to put these as separate links in there,
[26:09] is because the one that I just used before this was where we're looking at the projects.
[26:16] But if we're at the homepage, I may not scroll down. That is just something that I know that I may not do.
[26:26] So I want to link the projects and have that, but this other one is just so helpful
[26:34] of just notes with the projects. Maybe notes or summaries?
[26:44] Learning modules? - Learning module makes me think
[26:49] of the way Codecademy organizes things, which is like lessons inside courses,
[26:55] inside modules, inside paths, which is also a reasonable way of doing things.
[26:59] But yeah, I like summaries, modules. Pubs.
[27:03] - How about I'll put the link as summaries, and then when I break it down into each of them later on,
[27:11] or next stream, who knows, I will put modules. So we'll do a little bit of both.
[27:18] (mouse clicking) - Everyone organizes path, module, course,
[27:28] hub, et cetera, differently. It's fun.
[27:30] - Oh, it's true. I have done it on multiple companies,
[27:33] and everybody does it differently. And you have to like notate which one,
[27:38] like what the string or path is. (mouse clicking)
[27:45] Breakdowns. I'm just putting that there, so I remember.
[27:52] Put it there. ♪ Dee, dee, dee, dee, dee ♪
[27:58] So I am curious, and this is me being like, I've been in coding for like six months
[28:04] to those who code like daily and get paid to do this,
[28:11] of do you go through and say, like do this, where you're like, I'm just gonna link it all
[28:18] and then go back and actually make it work, or do you make sure that you're putting in the links
[28:23] properly about like while you're doing it? - Personally, I think it's more efficient
[28:32] to do what you were doing. Just like put all this stuff there,
[28:36] and then later on fix it up, because you never know what you're gonna end up
[28:39] removing or changing. So figure out what you want
[28:43] and then make it nice and tidy. That's how I code.
[28:47] I get the logic to be generally what I think will work, and then I go through with an actual high for scrutiny
[28:54] and fix it up. - Fair enough, fair enough.
[28:58] That is actually something that I recently just, like, hmm, what am I trying to say?
[29:11] Y'all make sure you save stuff and actually upload it to wherever you're using,
[29:17] like GitHub, because if you don't do that and you just keep doing stuff and saving it,
[29:22] then you might end up undoing something important that you did because you didn't upload it.
[29:30] And I might've done that this last week. It was not pretty.
[29:35] I was very frustrated. And I feel like that's just, like, you know,
[29:41] a path you must take. Okay, cool, yay.
[29:46] We at least can commit changes. Okay, I want to go here.
[29:54] I want to go here and copy and do, do, do, do, do. Where am I going?
[30:05] Hyper, yay. Can y'all see my terminal or hyper well enough
[30:13] or do you need me to make it bigger? Yay.
[30:21] So, oh, I'm just going to shamelessly plug this because I'm very proud of it.
[30:26] It is also the first tech writing thing I did. And Laura helped me a ton with just making it
[30:37] even more proper of how to update your home directory or like what you want to use there,
[30:48] because this helped so much on realizing and not putting stuff in my desktop or in my user folder
[30:58] and actually putting them in my code folder. So, voila, I get to open it, yay.
[31:06] And then CD, learning TypeScript, fantastic code. This is one thing I haven't gotten fixed yet.
[31:20] We tried, we tried on a stream, Laura and I tried, and I'm just not determined enough to get there.
[31:30] So, I'll just go magically turn it on. Yay, it's installed for a minute.
[31:39] Fantastic, we have made progress. Now, if I want to do the chapters
[31:51] like we were talking about, 'cause we are going to do from JavaScript to TypeScript,
[32:00] is chapter one. And yes, like we have,
[32:05] and let me link this to everyone really quick so that way you can look it up yourself,
[32:10] is it's talking about just the overall, we did go through this in a previous stream.
[32:21] So, not going too deep into this, but a brief history of JavaScript, the pitfalls,
[32:28] what TypeScript is as a programming language. And it was really fun to ask Josh these in details
[32:37] of a programming language, a type checker, a compiler and a language service.
[32:43] I will at some point get those like probably chopped out of the first one and create a video based on those,
[32:50] because I thought those were really good and explanations of them, because it was always like,
[32:56] I don't think I ever thought of beforehand what a language service was or a compiler.
[33:02] And we really broke it down in that stream. And then TypeScript advantages,
[33:08] freedom through restriction. I feel like this is a very good one
[33:11] and really talks about the type of person when you're like learning of,
[33:17] I like to try to break everything and then learn it instead of having restriction,
[33:21] learning the rules and then breaking it. So we're going to try learning the rules
[33:26] and doing things better and faster. And then just getting started with everything.
[33:33] Now we have the typinator. So,
[33:38] going over here to be able to get it to store locally and have all of the projects.
[33:52] Quick question. And this is me not knowing GitHub actions well enough.
[33:59] Would you, is this something that if I add the repo with,
[34:07] words, Jen, words. Can I add this within the learning Python repo,
[34:20] clone it and decide the learning Python, art learning Python learning TypeScript repo
[34:25] and still be able to go into that folder and get it to load even though they are both GitHub repos?
[34:34] - You could try. - Okay.
[34:42] - I don't know. It's a good question.
[34:46] - 'Cause I feel like this would be a little easier for people to do than if I just like copy
[34:52] and paste things over. I just want them to be able to access it a little easier
[34:57] than trying to remember like, where did Jen do all this stuff?
[35:01] So let's find out. So we're in learning TypeScript.
[35:07] Let's paste. Oh, didn't I just hit copy to,
[35:17] - Clone it. - Are you trying to,
[35:21] did you mean like get clone paste? - Yeah.
[35:24] - I think you just pasted. - Yeah.
[35:30] What did, oh, it didn't copy the entire thing for the clone.
[35:41] - Yeah, it just copies the URL. - Oh, that's weird.
[35:44] Why did this one copy the GitHub repo clone when this one only copied the URL?
[35:56] - Were you in GitHub CLI when you copied? Like a little subsection?
[36:01] - I was just right here. See?
[36:04] - Yeah, that one's in GitHub CLI. - Oh, then why didn't this one go to GitHub CLI?
[36:10] - Oh. 'Cause I didn't manually like move this one earlier.
[36:15] It was just on it already. Interesting.
[36:19] Oh, that's a good call. Coffee.
[36:27] Coffee just called out first off that I was just pasting the URL, 100%.
[36:31] And then Afi also, wow, words, Jen. Maybe the clone does something.
[36:39] They haven't clicked it before. I use the GitHub CLI quite a bit,
[36:46] and I love that we are doing this live, even though I feel completely silly
[36:51] that I didn't realize that it was that. On, it definitely is small things like this
[36:59] that can really frustrate people, being me. I can get really frustrated
[37:06] when I don't notice those small things that make a huge difference.
[37:11] Like it probably could have taken me like an hour to do that, so.
[37:15] Code. Hey, we got projects.
[37:21] Yay. - Fine. - All right.
[37:23] So to hopefully make this a little easier on all of us. You don't need that one.
[37:31] We're going to put these side-by-side. Hopefully I make them big enough.
[37:36] - For maybe another time, there's a really good app called Rectangle for Mac
[37:42] that gives you really nice keyboard shortcuts and like snapping behaviors.
[37:45] You can like drag and drop a window to the left side of the screen,
[37:47] and it'll snap to 50% of your screen width. - Oh, that is. - Like the way it works.
[37:53] - I thought I closed a different one, but apparently I didn't.
[37:56] And it's a really nice app. It's called Rectangle for Mac.
[38:00] I thought I closed a different one, but apparently I didn't.
[38:03] And that is phenomenal. What is it called?
[38:11] - Rectangle. I am a big believer that although I have a bunch of Macs
[38:22] and like use Macs for developments because I have to, I really like the Windows desktop interface a lot more.
[38:27] Yes, that is. - I, yes, yes. I'm gonna add this to my to-do list y'all really quick
[38:33] because this is something as funny as it may sound. I had to put in my to-do list yesterday
[38:43] to reply to a lot of you because I was like, I haven't replied to homie.
[38:47] I didn't reply to Ben. Oh my God.
[38:52] So I'm just gonna put it on my to-do list so that way I remember later.
[38:57] Yay. And that's actually really exciting
[39:00] the way at least it sounds like it would work because especially while streaming,
[39:05] it can be really annoying to have to like manually do all of this.
[39:09] - Yeah. - Okay.
[39:12] So we, and y'all, if you didn't see it, this is already what I'm doing is
[39:20] I just went with step one and was like, oh, okay, let's do this
[39:23] without reading all of the steps or directions. So we're now gonna read the directions
[39:27] and see if this is what I missed. So, sweet.
[39:34] We went to the projects. Okay.
[39:44] And Ben is saying that there are, there's a few window manager apps
[39:54] in the rectangle camp. Def get at least one of them.
[40:01] I feel like this will like save my life. I'm so excited about it.
[40:03] 'Cause especially if I'm doing stuff from my laptop, it's so frustrating.
[40:06] Okay. So we need to go.
[40:11] Oh, so we didn't even really need VS Code. Oh, this is exciting.
[40:19] Something that we were talking about and I know not everybody was on this stream yesterday
[40:28] with distribute aid. What is a jest?
[40:34] - A jest is JavaScript testing. It's a library that you can run that runs your code tests
[40:47] and then lets you know how many tests passed or failed. Does that sound reasonable?
[40:54] - Yeah. That is something that I think
[40:59] when we were streaming yesterday, the dog and I were just not getting along at all.
[41:06] She was barking at everything. So it was a lot of me going on mute a lot,
[41:11] but they brought up, I don't even know if this is it.
[41:17] No. A website that also explained a lot of it.
[41:22] So maybe it was this. No, I'll look it up later.
[41:27] But that's a guess. Yo, my chair just broke.
[41:31] Well, something broke. And now it's wobbly.
[41:35] Oh, that's it. That's entertaining.
[41:38] All right, well, I'm still here. So we're good.
[41:40] So back to this one. All right.
[41:46] So in this, we are going to copy,
[41:53] but we first need to go into Learning Typescript projects.
[41:59] - So you've done things slightly different from the command, which is fine.
[42:05] This is gonna be slightly different words. You cloned it into a folder named projects
[42:10] instead of a folder named Learning Typescript projects. So you can either just go to the projects folder
[42:16] or rename the folder to Learning Typescript projects. Learning Typescript projects.
[42:21] - And I'm not gonna lie when it comes to this stuff. A lot of times I don't know if it's called cheating
[42:31] or just doing things differently. I'll actually just go edit it here instead.
[42:38] And a big reason I do that is this for folder structure, it still makes a lot more sense
[42:44] when I'm looking at it this way than folder structure going through terminal.
[42:48] So you have it. - That's totally reasonable.
[42:51] I do the same. - Named Learning Typescript projects.
[42:56] - In kebab case. Happy lunchtime, everyone on the East coast.
[43:01] - Cool. - That way we can actually go through the directions
[43:10] the way you have it said. So yay.
[43:15] All right. And then NPM I, is that installing something?
[43:22] - Yep, that's what the I stands for. - I was like, I know NPM does installing a lot of things,
[43:30] but... - No, I should fix that security thing.
[43:37] Make it stop yelling about that. - Well, let's run the audit fix.
[43:46] Yay! Is the code on the terminal VS code right now?
[44:03] Wait. I'm not sure if I know what you mean by that question.
[44:11] Coffee. This one I'm currently using hyper as my terminal right now.
[44:19] If that helps. I ended up somewhat watching
[44:27] James quick, like set up for terminal to make it look prettier.
[44:34] So this is what I ended up with. And what up she be?
[44:40] Thank you for the follow. And yes, we are like having fun
[44:47] having Josh break down TypeScript to very, very beginner friendly,
[44:52] which I think is a lot of fun. All right.
[44:57] So we fixed the vulnerabilities. We are going to CD into this.
[45:04] It's really fun to copy and paste. In one terminal run the TypeScript compiler
[45:12] via the TSC script within whatever step you're working on. For example, start the TypeScript compiler
[45:21] on the first step and watch mode. So basically at this point, I'm going to be honest.
[45:33] And I love that we're doing this at the beginning. I'm following directions,
[45:36] but I have no idea exactly what we're doing. - To you on how I should improve the site
[45:44] to explain this better one. - No, not necessarily.
[45:47] I'm saying that we're doing it backwards. Like remember how I said, I wanted to do the problems
[45:56] or the test before actually studying. - Sure.
[46:01] - So this is me going, hey, what is this? I wanna see if I can figure it out.
[46:09] - I would say, yeah, it probably does assume knowledge of NPMI or NPM.
[46:17] But this is a big thing. And why I asked Josh if we could do this
[46:22] is TypeScript is so commonly talked about when talking about JavaScript
[46:28] that I feel like a lot of beginners are like, hey, I wanna learn TypeScript.
[46:34] And where a lot of people previously, were like, yo, you gotta have very solid JavaScript
[46:44] knowledge to learn TypeScript. And so I'm going through it as,
[46:49] I got some JavaScript knowledge, a smidge, a smidge. So I'm gonna see if I can figure it out.
[46:54] And that I think is definitely not what TypeScript in general is normally the audience that gears towards.
[47:04] But also if we were to put some in between things, what would they be?
[47:09] And I think NPM is a caveat that we could put here of like, if you want to learn more about NPM.
[47:16] And I have a really fun error that I need to read. - You know what?
[47:27] I think this is a recent bug in the site where I shouldn't have been asking you to run that command.
[47:31] So I'm just gonna say, you can skip that. I'm gonna fix that now on the website.
[47:38] So just ignore the thing, the NPM run TSC, you can command C out of this, don't worry about it.
[47:44] Thank you for a beta testing for me post release. - Yes, if anybody needs me to beta test instructions,
[47:51] I'm here for it. I love learning.
[47:53] I also am really great at not using things the way they were meant to be used.
[47:58] So I break stuff to find bugs. It's a lot of fun.
[48:02] I would say also, oh, okay, I see what you're saying to copy.
[48:11] Okay, so we're gonna skip that one. That was fun.
[48:17] In another terminal run just via the test script on whichever step you're working on,
[48:22] for example, to start tests for the first watch mode. So let's do that.
[48:29] What? Oh, here we go.
[48:37] - And I should put a note in here that the test will fail at first
[48:44] and your job is gonna be to fix them. - Yay.
[48:47] Okay. So what do I have?
[48:58] Okay, so test suit failed to run. Reference error humanoid is not defined.
[49:08] And then the comments say C./original.js for their older JavaScript code.
[49:20] Module.exports.humanoid equals humanoid with a capital H and then model.exports.robot equals robot.
[49:32] And going through this, I can run the test again.
[49:39] And let's see what, and really quick, I'm going back over here.
[49:46] Coffee just said you can install TSC globally and run it without npm run.
[49:55] They think. Sheepy said, but if you can do npm run TSC,
[50:02] doesn't it mean you can do TSC fine too? They haven't gotten to cpkg.json though.
[50:09] I love having more, I don't wanna say more educated, more experienced people, because then I'm like,
[50:18] oh, that's where you would look for that? That is good to know.
[50:20] That would make sense, but. All right, so steps.
[50:24] I'm gonna look at this step number one. Prototypes to classes.
[50:30] I'm going to just try to fix it based on the error code 'cause I'm stubborn.
[50:39] And this is also, I'm not great at reading directions. As we can see, this is why Ramon,
[50:46] who is somebody that's been on my stream quite a bit, will tell me to read things out loud
[50:51] so I don't skip over them. - It does hurt me a little bit
[50:55] because I put effort into making all these chapter read-me's or project read-me's really flavorful and silly,
[51:02] but we can't go into that. - And I think that's a big part is there's so many different learning ways of learning,
[51:10] and this is something that, I can do this. I guess I'm just embarrassed to do it on stream
[51:18] and also something I'm not, I'm still getting used to the fact that I can do this.
[51:25] Of, for when they have steps like this, of making sure I use my text-to-speech
[51:32] to actually listen to them and comprehend them, where I honestly get a little embarrassed
[51:42] of doing it on stream 'cause I'm like, what are people gonna hear or think if I do that?
[51:48] And I think that is a big step of also not realizing that I can't do that until the last couple of years.
[51:56] So I'm so used to also just going, well, I have to just figure it out
[51:59] without reading documentation 'cause documentation has always been hard for me to read.
[52:05] - Makes sense. - So that being said, we're gonna do what Ramon said
[52:10] and y'all get to hear me read out loud. I'm very excited about this.
[52:15] All right, so we used for steps, we have step one and step two.
[52:21] And I'm going to scroll down to the readme that it linked to and step one is prototypes to classes.
[52:32] The first project for you to overhaul hails from before the time of class syntax.
[52:38] How primitive. Okay, I also reading out loud
[52:42] with like any like proper inflection is not gonna happen. So y'all try to say it yourself, but also, yes, Josh,
[52:50] you are much better at writing these than a lot of people because this is not how I write my readmes.
[52:54] My readmes are like, go here. - Yeah. (laughs)
[52:59] Yeah, it's hard. - Yours are much more comical. The original .js file contains the project's original code
[53:08] for robot and humanoid functions used as classes. Your job is to port that code to proper
[53:17] ES2015+ class classes. Specification, an index.js export to classes
[53:27] using ES2015 class syntax. Robot based on the robot function in original.js.
[53:36] Humanoid extending the robot class based on the humanoid function in original.js.
[53:44] Files, index.js, write your robot and humanoid function here.
[53:49] Index.test.js verifies robot and humanoid and solution.js is the solution code.
[53:55] So don't look at solution yet. Got it.
[54:00] - I also, that's a typo. It should say function plural.
[54:04] I just fixed that too. Index.js write your robot and humanoid function here
[54:11] should be functions. - Oh, I mean, Joe, like when I'm missing things,
[54:16] please like actually go make sure that I'm not just missing things.
[54:19] - No, no, no, to be clear, you said it correctly. I wrote it incorrectly and now I'm fixing it
[54:24] in the original repo. - Okay. - So thank you, good.
[54:27] You did nothing wrong. - You're welcome. You're welcome.
[54:29] And so that being said, and this is also me learning a bit of VS code
[54:37] and how this was, ooh, this is a great question from Coffee.
[54:44] Jen, does ES 205 classes mean stuff to you or would you like modern JavaScript classes
[54:51] to be more understandable? I'm gonna go with that.
[54:58] - Yeah, I meant it as ES 2015 because that's the technical, right?
[55:05] Like the technical-- - Oh, okay. - For like what edition of JavaScript they were added in
[55:08] because JavaScript gets new additions roughly every year now.
[55:13] But yeah, that's a good question, I think. Like, are you familiar with ES 2015 classes,
[55:17] aka just modern JavaScript classes? - Okay, yay.
[55:25] Thank you Bedrock for coming and hanging out with us and everybody over there.
[55:31] We are working on learning TypeScript and I am being the annoying student
[55:37] that is going through all of these lessons from Josh's learning TypeScript book
[55:46] and doing them as I would normally do them and also getting called out
[55:51] that I need to practice on reading out loud and learning more about JavaScript and TypeScript.
[55:58] It is pretty, isn't it? - It's a sun conure.
[56:05] I requested bird. I really like birds.
[56:07] They were kind. - I like the bird.
[56:09] I feel like without meaning to, I feel like the color of our background
[56:18] really compliments the bird. - I just assumed that was intentional.
[56:23] - It wasn't. It was you and I used one
[56:27] and then like I set one up for ours and then Homi made Laura's and my Monday strings similar
[56:36] that I was like, I don't want them to be associated. So I went and found a new one
[56:40] because I didn't want Homi to change that one 'cause I liked that one so much
[56:43] that I found this one and I was like, oh, they're pretty together.
[56:46] I like this. But that being said,
[56:51] Sheepy said lately they've been thinking about learning JavaScript or JavaScript TypeScript,
[57:00] helps if I can read properly in the last couple of months. They've been learning TypeScript and JavaScript
[57:06] by doing at the job and they've mostly been missing,
[57:11] missing most of the fundamentals, I guess. Well, that is where we're here
[57:17] and you can join us every other Friday 'cause that's what we're gonna be doing.
[57:21] Oh, Coffee just said to Sheepy, hope they are doing better than their last job
[57:32] when they started, they'd been doing TypeScript for years which meant they were using file extensions
[57:38] and running ancient style JavaScript code through their TypeScript compiler.
[57:44] All right, Bedrock, learned half of TypeScript on the job. All of that just kind of sounds terrifying
[57:58] but also I'm trying to like remember a bit of what Josh and I went through
[58:06] when we were streaming back in like November when we first went through this
[58:11] because there was like one thing and I, so to be very honest, y'all,
[58:16] I technically did this test back in November. I don't remember it whatsoever
[58:22] and something else was, let's see, if I go to the original,
[58:30] actually, I have to go find it, projects. What project are we in?
[58:35] The Typinator. - From JavaScript to TypeScript is the chapter
[58:39] so there's a folder for each chapter and then the Typinator is the project.
[58:45] - Ah, thank you. I was looking just directly for the Typinator
[58:48] 'cause it was the project name but it makes way more sense that it's in the chapter.
[58:57] Just not where I necessarily went. All right, so,
[59:00] in the index, right, robot and humanoid functions here and I'm just gonna,
[59:10] but to answer your question earlier, Coffee, about, yes, 2015, to say it properly,
[59:19] I don't think I knew that was really a thing. Like, I didn't necessarily know what, yes, 2015 was
[59:29] or that it was a thing or that it meant really anything. A lot of what I would have done would have been like,
[59:39] okay, cool, let's see if we can figure out the rest of it and may not have even registered what
[59:46] that JavaScript classes change and there's different versions of them.
[59:55] I just would have gone, oh, this is JavaScript class that TypeScript uses
[60:00] and end of the story. I think it's, and I would say definitely,
[60:11] and as a reminder, just on this one, is that I am going through this very backwards
[60:18] of just seeing if I can figure it out instead of going through the chapter.
[60:23] So it's definitely maybe something that he does point out. We should, you should go get his book.
[60:30] And it is something that you can also get the PDF version for Kindle and use text to speech.
[60:36] And a big reason for those who are like, Jen, you can't read very well, why are you,
[60:41] why do you have a physical book? And a big reason for that is 'cause as much
[60:47] as I need a text to speech tool, I am not good at keeping notes all digitally.
[60:55] I need to be able to physically look at things and in the order.
[60:59] And I use this, for example, this is something that we typed last time.
[61:04] Maybe, maybe, maybe we're gonna get there. 'Cause I can't see my, there we go.
[61:11] Is I write notes in the book and it really helps me remember things
[61:17] when I'm getting really stuck. So to me, books are for note taking.
[61:23] We're gonna go with that. Oh, interesting.
[61:33] That coffee said that they've seen people from a hundred devs learn JavaScript
[61:41] and sure they encounter class quite early. They may, and to catch everyone up
[61:48] because you may not know this. Ooh, so to someone maybe learning in the last few years,
[61:54] it might be harder to understand that class wasn't always something there.
[62:00] I'm paraphrasing it. Always there or something.
[62:03] This is also my problem of reading out loud or reading in general is I just put words there.
[62:10] It's really annoying. A big part that I will say that I got a little stuck
[62:17] on classes when I was trying to figure it out for JavaScript and it actually started make more sense
[62:25] when doing TypeScript. Yet I've noticed that it's not something
[62:32] that's used everywhere. Maybe it is, but, or I miss it,
[62:38] but I haven't seen like when I'm working on other projects that I have to create a class of something.
[62:46] Do you always have to create a class for something in JavaScript?
[62:49] Is this the thing that I just haven't stumbled upon yet? - You don't.
[62:55] I don't often use classes once in a while, but. - Okay.
[63:01] - It's a feature. - This was a big part of actually why
[63:05] this ended up working out really well, but I was on LinkedIn learning
[63:10] and classes were what I got stuck on. Like I was really having a hard time comprehending classes
[63:16] 'cause they wanted us to pause and go do classes to put them back into the code.
[63:21] And I'm just like, and they use a backpack as an example. So it just was not clicking.
[63:27] And then when I was like, hey, I want to be a DevRel. And everyone was like, you need to know tech
[63:35] and have content. And I was like, cool, I'll start streaming.
[63:39] And until we started learning TypeScript, I have not run into classes, which has given me more hope
[63:44] where this one course that I was stuck on, it specifically needed me to do classes next.
[63:52] And I didn't realize that you don't necessarily need classes. So I'm excited that we're doing it now.
[64:00] And well, let me come back to this one 'cause it was first of Bedrock said,
[64:07] classes are for a specific programming style. And Coffee said languages like C sharp.
[64:16] Is it C? - C sharp, yeah.
[64:24] - It was like trying to say seashells. Shelly, she's...
[64:30] - Sally sells seashells by the sea shore? - Yes.
[64:33] - Simply speaking. - Trying to say C sharp.
[64:37] Okay, and Java more forcing you to have classes versus like JavaScript and C++ where you can use them
[64:43] or not. Oh, I love this.
[64:57] This is just happiness. I don't see sharp, I wear glasses.
[65:02] That's just like the happiest thing for this Friday. Thank you.
[65:10] So, okay, going back to over here of re-reading all of this and talking about classes.
[65:21] Specification in index.js export to classes using ES 2015 class syntax,
[65:31] robot based on robot function in original JS humanoid, extending the robot class based on the humanoid function
[65:43] in the original just.js. So what I was doing when I was like trying to figure this
[65:50] out for a different project is I kept always selecting them and would go to definition, trying to find them
[65:57] or seeing if they have like references or things like that. And then also something that I started doing,
[66:04] and I'm also doing this out loud. So that way people can tell me if it's like
[66:08] not the proper way of doing things of like yours walks me through like where they actually are.
[66:15] But that's not always something that happens when you do a full project is I'll just start looking
[66:22] for it and search it and then go see if where the original might be and where I need to change things.
[66:29] And that can be very helpful or very overwhelming. So thank you for telling me where things are
[66:35] in the original.js. Okay, so and this.
[66:45] And this is where I'm totally getting stuck because instead of module exports,
[67:07] wouldn't it just be exports or no? - I think you could kind of ignore that part of it
[67:15] because either way works depending on like what system you're running in.
[67:19] I don't normally use this style of things like agile exports dot or module exports dot.
[67:29] This is called common.js modules. I normally use the newer like standard JavaScript modules
[67:34] called ECMAScript modules. Yeah, so this is CJS, I'm used to ESM.
[67:40] So yeah, if you could try removing the module dot from them and see what happens,
[67:45] but it should work the same either way. But either way, it doesn't really matter.
[67:53] Like it's the same code or the same result. Is that what you're asking?
[67:57] - I think so. And thank you for the follow, Mr. Software.
[68:04] Because when I was working on a different project, I thought it had more of like,
[68:12] yeah, it would be more just like this where it was export. But I thought it would be like export instead of dot robot,
[68:26] it would be just like export robot equals robot without the dot.
[68:31] But am I just maybe remembering incorrectly, which is definitely possible of what an export would be?
[68:39] - Yes. I think you're halfway between the style
[68:44] or the form of exports that's used right now in the repo and maybe like the new exports
[68:49] or like a different languages exports. - Okay.
[68:53] So step in the specification export two classes in the ES 2015 class syntax.
[69:02] So those are already done. And then in original.js.
[69:07] - So this is the... So honestly, you don't really need to go
[69:19] through this lesson, right? If you don't want to,
[69:21] this might just be a good exploration of how the projects are set up.
[69:24] But the intent of the lesson is that you have this old style of JavaScript code.
[69:28] And in the chapter, one of the things that covers is
[69:33] there were like new ways of doing things and old ways of doing things in JavaScript
[69:37] because the language has been improving over the years. And one of the like,
[69:41] there's an old way and there's a new way things as classes where this was the old way of writing classes.
[69:46] You didn't actually use the word class. You've made a function, excuse me.
[69:49] And then put stuff on the functions prototype, like robots.prototype.announce equals function announce.
[69:56] But if this isn't necessary for learning TypeScript, this is just like an exercise
[70:03] to get used to things ahead of time. So if you personally don't jive well with classes,
[70:08] you can just skip this. - Okay.
[70:11] - Up to you. - Yeah, and I think that is an interesting way
[70:17] of putting things in and could also be why I'm also struggling
[70:21] so much as with classes still, they just don't click.
[70:25] And Coffee said, they think many learners might start off with website code
[70:31] that isn't like library with exports. This is possibly another way
[70:36] to confuse learners in lesson one. And also I think, yeah, that's fair.
[70:44] They're not super into NPM, but have a vague recollection.
[70:49] Right? Recollection?
[70:52] Recollition? Right?
[70:54] - Close enough. - About like CommonJS still being recommended for reasons.
[70:59] - That's good feedback. I'd plus one it.
[71:04] Sometimes, yeah, CommonJS, the old style of modules, some platforms or like some libraries or frameworks
[71:10] haven't been set up to support the new version of modules. So sometimes you do have to use CommonJS.
[71:16] I think that's why I use it here. - Okay.
[71:19] - Yeah. - Okay.
[71:21] Cool. Like without even realizing it,
[71:25] like A, first off, I think this has been just like such a great exercise on how to say this,
[71:34] of like, cool. Like for people that aren't the best, like me,
[71:39] at following directions, this is a really good example of why it's important
[71:44] to go back and follow the directions. And also like a bunch of different ways
[71:50] that we can like Google things and set them up, but also like, because as a reminder to everybody
[72:00] that's been hanging out with us today or may tune in later on is I did not read the chapter.
[72:05] So I was just winging it. And I think that's very interesting
[72:11] because many, many people, I think, when tackling things nowadays, they do that.
[72:21] They just kind of like skip ahead. And also, or the directions are not as entertaining,
[72:28] which yours are entertaining. Oh, y'all, we need to talk about this though.
[72:33] This is like a really big reason why you should follow directions and not just skip ahead.
[72:37] Like, because is, there are funny things at the beginning of every one of them,
[72:46] every chapter, and you should read them is what. So chapter one is from JavaScript to TypeScript.
[72:56] JavaScript today supports browsers decades past beauty of the web.
[73:00] It's a haiku. Okay, well, I don't probably read it
[73:05] in the proper way of reading them, but everybody should. I like the haikus.
[73:12] And this also gave me more of a way that I think as, if I were to say to newbies of going through this,
[73:20] of like, hey, if you're just wanting to start learning TypeScript and things,
[73:27] and you don't wanna compare to JavaScript, because sometimes that's not always the easiest
[73:32] or wanna deal with classes, maybe skip chapter one. Because knowing me, if it wasn't for all the support here,
[73:40] and I really appreciate everybody is, I would have been like, well, this isn't clicking.
[73:47] So I may be like, okay, I'm not gonna learn it. Not because I'm like, oh my God, I can't like figure it out.
[73:54] But like a lot of times, since I'm so used to having to just like pick it up very quickly and move with it,
[74:00] I don't always know how to study or properly Google things. And I think this is such a good way of reminding people
[74:12] if a chapter doesn't make sense, and this is not to Josh's book,
[74:15] this is literally to anything. If one chapter doesn't make sense,
[74:19] you can go around it and go learn other things. And maybe that chapter will start to make sense.
[74:25] And that is a big thing that I wish I could tell all learners in any topic, because when I was building my website
[74:33] this weekend and trying to do things, I kept having to remind myself,
[74:37] I'm very stuck on this problem. There is no reason I need to do this specific problem
[74:41] right now, I will go try something else. Thank you for the Jen rant of,
[74:48] if something doesn't click, go do something else for a bit.
[74:50] And thank you, Josh, for being here and doing this, because I think this is a really good way of newbies
[75:03] also seeing that it's not something that may automatically click for people.
[75:12] Like, we had a lot of engagement from the audience, and thank you everyone that showed up,
[75:16] that was also asking questions, because TypeScript is a very,
[75:21] I don't want to say difficult, I want to say new thought process.
[75:27] Like, it's harder to put together the methodology and thought mapping into place to be able to comprehend it.
[75:38] And that takes time. It's more time consuming than anything.
[75:46] - There's a difference between difficult and different. - Yes, yes.
[75:53] And I would say that TypeScript is different, not difficult. At least when I've been able to use it
[76:01] in other projects, but it's definitely something I want to practice more,
[76:09] and this is really exciting, and I'm so grateful that Josh has come on to do this.
[76:14] And also, so with this being done every other Friday, and something that we have talked about for a while,
[76:22] but I really dropped the ball with the holidays, is even if Josh isn't available for TypeScript
[76:31] or Laura's not available for when we talk about Python, is I'm just gonna, you know,
[76:37] keep showing up and do it by myself. And we're going to see what happens.
[76:42] Might look a lot differently because I might try to skip through reading something.
[76:49] And then Josh will be like, I'll just have Josh's like voice in my head going.
[76:56] But I put effort into it and it'll be funny, not like everybody else's.
[77:00] That's my impression of me remembering that I actually do enjoy reading your writing
[77:06] instead of that is just a normal like textbook. - Word.
[77:16] - All right, y'all. I feel like this is a really good breaking point.
[77:22] And on the Read Me page for each chapter, I will be putting the link to the video stream.
[77:31] So that way, if you're like wanting to skip around or try it, you can go through that
[77:35] and look at the chapters. And also it will have a link to the projects,
[77:41] everything we've talked about. Please let us know in first off to everybody
[77:46] that's hanging out with us. Anything else you wanna ask Josh
[77:50] before we let him go for the day? And thank you for joining, Sheepy.
[77:56] I have questions. Josh, what headphones are you using?
[78:07] - Bose QuietComfort 35, some variant to them. The type, it's relatively new, they have USB-C.
[78:17] I tried the Bose noise canceling 700s and they were fine.
[78:22] Little, they're not cheap or flimsy, like a little less sturdy than these classics.
[78:26] And they had like the situation where the whole headphone was like a capacitive touch thingy.
[78:33] So like every time you like adjust it, you could accidentally turn the volume on or mute yourself.
[78:37] It's really annoying. - Ooh, I don't like that.
[78:40] - Yeah, but I really like the QuietComforts, that's a good line.
[78:43] It's like 45S or something maybe. - I don't know where my headphones are.
[78:47] I was actually looking for them. I have a very old school version of them.
[78:50] I have QuietComfort 35s from 2018, I think. So mine are still the micro USBs and very frustrating.
[79:02] So I've been going, okay, these are still really good quality.
[79:08] I cannot like convince myself to go upgrade. And for those who may have questions about streaming,
[79:16] feel free to join in and ask questions about that too, because Josh is a fellow streamer.
[79:21] And if you don't already follow Josh, go follow Josh on streaming,
[79:25] 'cause then you can ask questions there. And I don't know, shout out.
[79:32] How do you do shout out? Shout out, oh, hey.
[79:37] - My goal for the beginning of this year is to figure out stream elements.
[79:41] I just haven't even tried that till now. - Ooh, ooh, we might be getting somewhere.
[79:50] Josh Goldberg, okay. Yeah, so that took me like a full like minute
[79:58] just to get the shout out out. But go follow Josh.
[80:02] And that is it for my side. I definitely will.
[80:09] I'm scared of this journey because learning live, I will say like, as I grow in knowledge,
[80:19] learning live almost seems scarier because I'm like, I should be getting this by now.
[80:26] And I feel like other people see that and they're like, I should be,
[80:30] you should be getting that by now. And then I have to remember, Jen, it's okay, it's okay.
[80:35] You can still be a noob, still forever. And.
[80:43] - Opposition research. Yeah, plus one, it's okay to not know.
[80:48] Part of being a streamer for me has been being okay with other people
[80:51] seeing me flail and suffer, which I think is a good thing. - Yes, yes, I am.
[80:58] And good call, Coffee. You know, you can, but funny enough,
[81:07] you say you keep meaning to try. I recently gave a talk.
[81:12] Oh, Hank, Josh, I did my first talk. - Oh, congrats.
[81:15] - Yeah, I did my first conference talk. I'm very excited about this.
[81:19] And it was actually, I don't know if it's out there yet. And I'm gonna go look, hold on.
[81:29] Before I tell you guys the title, I want to tell y'all, I wanna see if it's live yet.
[81:35] 'Cause if it is, it has everything to do with if somebody wants to start streaming.
[81:41] Okay, that is definitely not. Come on, YouTube, I can do this.
[82:04] I can do this. Recordings will be available soon.
[82:10] Okay, well, I will just link to the website so you can go do it.
[82:15] But I gave a talk about saying fuck it, and it was extraordinary.
[82:22] And I say that in the fact of Coffee. You could always just say fuck it and, you know, do it.
[82:30] And it's scary and terrifying. And I will say not for everybody,
[82:34] because as I have talked before about not doing things live,
[82:39] unless I'm doing them live, I don't always do them, because I'm great at saying fuck it and just doing it.
[82:44] Nah, fuck it, we'll do it. It'll be fine, and we'll figure it out.
[82:48] Does not mean I'm great at strategy. There is that, and it is a very fine balance.
[82:55] And this is why I have a lot of people around me that are very strategic and do things very methodically,
[83:02] 'cause I'm the opposite. And that is just one big thing
[83:07] that if you need encouragement to do something, when this talk is out, you should watch it.
[83:14] Very excited, 'cause I had like three days to plan for it, too.
[83:17] - I look forward to watching it. Sounds great.
[83:20] - Yay! All right, y'all.
[83:23] And thank you, Chaos, for the follow. I appreciate it.
[83:27] Last but not least, let's go raid y'all to a channel. Ooh, I haven't seen them for a while.
[83:37] I feel like Trash Dev is really funny. So, oh, but Nick's online.
[83:43] Literally, his username is Nicky Online, and Nicky's online, so therefore we're gonna go to Nick's,
[83:50] 'cause Nick is the best. So y'all are about to get raided.
[83:56] And I don't know if anybody else announces it or just does it, but I'm not great at multitasking,
[84:00] so that's why I just tell people they're gonna get raided. Okay.
[84:05] Bye, everyone. [BLANK_AUDIO]

