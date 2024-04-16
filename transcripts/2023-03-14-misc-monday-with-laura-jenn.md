---
showLink: "https://www.youtube.com/watch?v=dm5YJZTT3cY"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "misc-monday-with-laura-jenn"
title: "Misc Monday with Laura & Jenn"
publishDate: "2023-03-14"
coverImage: "https://i.ytimg.com/vi/dm5YJZTT3cY/maxresdefault.jpg"
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

[00:00] - Hello, hello, beautiful humans. Welcome to another episode of Misc Mondays with,
[00:09] I don't know why I actually, where did I get music?
[00:14] Are you playing music? - I don't think so.
[00:18] - I just randomly hear music now. Oh, this is fun.
[00:23] This is the random stuff about live streaming is when music just randomly starts and you're like,
[00:30] I mean, it's pumping music, but, oh, I bet it's this. No.
[00:37] I have no idea what's playing it, but you know what? I will figure this out as we go, but it's Misc Monday.
[00:51] So welcome to Misc Monday. And yay, this is Laura and I'm Jen.
[00:58] - Hi. - And this is the best part about Misc Mondays
[01:03] is it could be all the random things, especially when I can't do an intro
[01:08] because music randomly plays in my background. Oh, I think I figured it out.
[01:16] - Yeah. - My Twitch was open in another tab and I heard the music
[01:20] and then I heard myself, so I think it was an ad. - Oh, gotcha.
[01:26] Yeah, that makes sense. - Yay, yay, figured it out.
[01:30] And Laura, do you want to tell them who you are? - Hi, I'm Laura.
[01:36] I am a developer advocate at Suborbital Software Systems, previously a math professor.
[01:41] I mentioned that just because it always ends up coming up. Anyway, I slept very badly last night
[01:49] and because of spring forward, my entire brain's just like, nope, being out on today.
[01:56] And I can't think of a single other thing to say. So you should probably introduce yourself now, Jen.
[02:01] - I mean, that's what I'm here for. And this is exactly why we do Misc Mondays though,
[02:06] because a lot of times it is Mondays are dreaded and there can be a lot of brain deadness.
[02:14] I know that I had almost complete back-to-back calls until now, which my day started at 6 a.m.
[02:22] and it's noon my time. So I had a lot of learning, lots and lots of learning.
[02:28] And to introduce myself, I am a developer advocate at Ivan
[02:34] and I am the host of where you probably might be seeing the show of Teach Jen Tech, where I,
[02:41] excuse me, my dog wants to interrupt in the background, where I learn about tech publicly.
[02:50] It's really embarrassing. It's super fun.
[02:53] It's very nerve wracking and it's very challenging. Yet it's way cooler than learning by myself
[02:59] because that's not how my brain thinks. I like to be able to interact with people when I'm learning.
[03:05] I'm gonna see while I'm talking if I can get my dog to be quiet.
[03:08] And I also am the host of a podcast called Shit You Don't Wanna Talk About.
[03:16] So basically, I learn live, talk about shit that's hard to talk about and I advocate
[03:22] about learning about database or data infrastructure. Ooh, that is a pretty good short synopsis.
[03:29] We might finally be there. Yas.
[03:33] And the fun thing about Mystic Monday is sometimes we have topics that we actually want to talk about
[03:41] and then other times we just show up. - Yeah.
[03:44] - Because we, Laura was the first person I started having
[03:51] more consistency of her being on the show. We started learning.
[03:59] She started teaching me Python with Al Swigart's Automate the Boring Stuff.
[04:06] And we tried doing that about every week and it ended up about--
[04:12] - First it was every other week. - Yeah.
[04:15] - And then it was every week. But then it was still taking us like forever
[04:22] and ever and ever and more evers to come because we kept going down rabbit holes.
[04:29] And so we finally just said, hey, you know what? We're just gonna have like rabbit hole day and Python day.
[04:36] - We should call this rabbit hole day. - Myst Mondays is rabbit hole day.
[04:43] - Yeah. - And a lot of times I really enjoy the fact that we do this
[04:48] because it's a way to digest a lot of what we've previously learned.
[04:55] What we're, we've talked about world events. We've talked a lot about,
[05:00] a lot of times I just tell Laura about things that I've been learning, if all else fails.
[05:06] Which today was, I learned a lot about OBS. - Ooh.
[05:13] - Which I think, because this has been a topic of conversation on this stream specifically,
[05:20] I do believe that I will have OBS set up in the next couple of weeks.
[05:27] I'm looking at getting some new gear. So once that's done, I think I will be set up.
[05:34] We will see, but one of my colleagues, Sebby, took time to go through all of it with me.
[05:44] And they have like this really cool document about OBS. And I'm like, dude, can we like add to this?
[05:51] Because it's really cool. So if it ends up being live, I will share with everyone.
[05:57] - Nice. - And we did functions on Friday.
[06:02] - Yeah, in Python. - Mm-hmm, mm-hmm, mm-hmm.
[06:05] - Oh, I have something I can show you. - And it turned out that you knew a lot more about functions
[06:10] than you realized you knew. - I didn't realize the name function, what it meant.
[06:15] Which is always a really fun thing of learning live, I would say, and also like being self-taught,
[06:24] is you don't always know that the thing you do has a name, or what it is named.
[06:33] I can show you what I've been working on this weekend, because this has been a interesting topic for us before.
[06:40] So share screen, I got a new website I'm working on. - Nice.
[06:49] - And the reason I show it is eventually, these will all link into their own subdomains.
[06:57] So people, I don't have to have three websites to keep up with.
[07:02] - Mm-hmm. - I'm very excited.
[07:04] But at the moment, it is just this homepage, and this actually took me a really long time
[07:08] to get to this point, so. - It's a thing.
[07:11] - Yeah, I did not realize. So when you started, I feel like I know the answer to this,
[07:19] but it's been a while. When you first started getting into tech
[07:24] and learning like Python and stuff, did you ever think about going to front end,
[07:30] or were you just like, yo, I'm gonna go to back end stuff? - Oh, so neither.
[07:36] I never, I mean, I, okay. So I was, as a math professor,
[07:45] I realized I needed to get a different job because teachers don't make any money.
[07:52] And the most obvious transition from math into tech was through data science.
[08:01] So not front end and not back end. Just no web, actually, it's like just not web.
[08:08] - Yeah, where I had it, I would have totally thought that that would be considered back end, but it's not.
[08:17] - Yeah, yeah, 'cause like, what's it behind, so to speak? I mean, like, yeah, it's between.
[08:34] It's actually between front end and back end, except it's like between it in a totally different,
[08:41] in a parallel universe. - I'm doing some Googles over here.
[08:47] - Yeah, like if you wanted to interact with, like, okay. So when folks are interacting with like chat GPT,
[08:56] they're interacting with it through a website generally. That website has a front end and it also has a back end.
[09:04] And what the website is like doing, I mean, I guess you could sort of consider that part the back end,
[09:13] but it's not just the back end of like the whole infrastructure.
[09:18] It's, I would say it's in the middle. It's the meat of the sandwich.
[09:26] (laughs) - Okay, I just, I have found a link.
[09:30] I shared it just in case anybody wants to look at it later on, because I feel like it at least gives us a start
[09:38] into data science and. - Oh, sorry, it's also not the case that like all data
[09:47] science would even have a front end or like a back end or whatever, 'cause you might just be doing
[09:55] your data analysis on your own company's databases. And the databases would have a back end,
[10:02] but the databases themselves are not the back end in like, to my way of thinking.
[10:06] - Right, right. - Yeah.
[10:08] - And that's interesting because especially with launching the data infrastructure series, I get to like dive
[10:15] into like so much data, data, all the data. What is the data?
[10:21] Which is very, very interesting. I feel like a new leaf has grown, turned over.
[10:28] I think the term is turned over. In the fact that I don't think I ever would have gotten
[10:34] this excited about data before, but I actually am like very intrigued about data infrastructure.
[10:42] And I'm stoked about Kafka tomorrow because a big reason why is I've heard of like event driven and those type
[10:50] of things, but for some reason, I just kind of give it a blank stare and go, yeah, that's a thing.
[10:57] Yeah, that does some things and stuff. Yeah, it just hasn't clicked yet.
[11:02] And I'm excited to have somebody on the show because this is, and you and I have talked about this
[11:07] many times, this is a big part about learning is it doesn't always click the first time you learn it.
[11:13] - No, or the third. - Very frustrating because I just want it to click.
[11:19] Yet, that's a big reason I enjoy doing less checking myself is 'cause at least others can learn along with me.
[11:28] I do have a follow up on this of what is a topic, if you're open to sharing with us,
[11:35] that took you a while to learn? Like I am by, I mean a while like to even conceptualize
[11:44] the concept of it. - There are so many candidates for this.
[11:51] I'm going to go with the one that I used to reassure my students, which is that I was a math professor
[12:01] who took calculus one, three times. - Okay.
[12:05] I don't think I've ever taken calculus. I think the highest I ever got was algebra.
[12:12] - Okay. - Yeah.
[12:15] - I don't know, I found out that I, this took up quite some time of I love learning,
[12:21] I hate school. So I did not make it very far in university or college.
[12:30] - Yeah, it's kind of the same for me. I love school when it's built for me.
[12:38] - Oh, that's a good one. And Fakai just said functional programming
[12:47] is slowly starting to click for them. It's been a long time in the learning process.
[12:52] Now I'm just going to go Google what is functional programming.
[12:57] - Yeah, yeah, that's one that I've looked into. And that's taking a while to click for me too, for sure.
[13:09] I'm copying and posting, copy and pasting a copy-paste of it of functional programming is an approach
[13:21] to software development that uses pure functions to create maintainable software.
[13:26] In other words, building programs by applying and composing functions.
[13:30] So we just basically talked about it the entire time on Friday.
[13:36] - Sort of. So I'm trying to remember what's the...
[13:40] I'm getting stuck on, like, there's a binary declarative or declarative programming versus imperative programming.
[13:55] And then there's functional programming versus, and I'm trying to remember the term for like,
[14:00] what's the other half of the binary for functional programming versus...
[14:08] I don't know, let me see what versus comes up with. Object oriented?
[14:14] - Okay. - Is what it's coming up with most.
[14:19] Which let's share this lovely, hopefully it's lovely. I haven't read through it, but there is a Medium post on it.
[14:33] Cassidy Williams. Cassidy is big into functional programming.
[14:39] And she always has nice explanations. I'm sure that the one that you just found
[14:44] is perfectly lovely. I just want to see if I can find...
[14:46] - It's from 2019, so it's a little outdated. - Okay.
[14:49] - I think that's definitely something that... Thank you both of you for sharing
[15:01] just like some things that you got stuck on because it's definitely,
[15:05] I think that's one of the hardest parts about changing industries is switching
[15:12] or like having to understand new concepts. It's like, after you can like understand the concept,
[15:21] you're like, yo, I got this, but before that. - Okay, here's one of Cassidy's.
[15:29] Oh, I should paste it in Twitch and on StreamYard.
[15:32] Oh no, wait, I should paste it. Wait, how does this go again?
[15:39] No brain. - Paste it in StreamYard.
[15:41] - Okay. - And then it'll go to all three.
[15:43] - Okay, okay. So the exact opposite of what I was thinking,
[15:46] which is awesome. - Yes, 'cause once I get OBS working,
[15:52] I can only stream to one spot. - Oh, why am I getting it as a Twitter link?
[15:57] That's so annoying. Twitter.
[16:00] - Yeah, yeah. I will say like, as we have people joining
[16:05] and thank you for stopping by and saying hi, is there any questions that y'all had for us?
[16:10] Because MISC Mondays definitely don't need to be just about what we come up with.
[16:15] It can definitely be what y'all wanna talk to us about, or we can always have them as being very short
[16:21] because we at least kicked off Monday hanging out for a hot minute and that's always fun.
[16:26] So it's very easy, go with the flow. I just wanna, since we don't have conversation today,
[16:33] if anybody else has some. - Yeah, okay.
[16:38] So yeah, the difference between, so you've got object-oriented and functional programming.
[16:44] And the thing that I get stuck on is that you still use functions
[16:49] in object-oriented programming. It's just not everything is a function.
[16:55] So in object-oriented programming, everything is an object. And in functional programming, everything is a function,
[17:01] but you can still have functions in object-oriented programming.
[17:06] - I'm still just stuck on the really pretty artwork. - Yeah.
[17:14] - Oh, this is cool. This is definitely something worth checking out.
[17:17] I would say, and this is the way my brain works, especially after so many meetings in the morning,
[17:26] I love that one thing that you and I have talked about and then, oh, Fukai just said,
[17:33] and you can still have objects in a function style. - Yeah, that's what I figured
[17:40] was that it was gonna go both ways. Just for extra confusion.
[17:44] - How do you explain it? How would you explain this to someone?
[17:48] - Me? - No, Fukai, how do I say your name?
[17:54] I do this every time. - I feel like maybe you said Focky, but I don't know.
[18:01] I have absolutely no reason to think that I am saying that correctly.
[18:07] - Okay, well, I was gonna say that one of the things that I really love about doing streams with you
[18:14] and meeting more and more people in tech is that makeup is a thing.
[18:22] - It makes me happy. - Yeah, makeup.
[18:26] - Makeup in what context? - That there's more people that wear makeup.
[18:30] - Oh, like literally cosmetics, okay. - Yeah, like literally cosmetics.
[18:35] Not like Markdown. And you don't mark down in makeup.
[18:39] Makeup from Markdown. - No.
[18:42] - That would be a really good stream name. - That totally is a really good stream name.
[18:47] Oh, we're gonna do another stream now, aren't we? We're gonna have a DevRel stream called Makeup Markdown.
[18:57] I'm gonna have to rename our makeup DevRel group on Mastodon.
[19:07] - Oh, yeah. Well, thank you, Bukai.
[19:14] And functional style is a big field, but the gist of it is like,
[19:21] use an Array.map instead of imperative style for a loop. All right.
[19:29] I dig it. I dig it.
[19:33] I feel like there's definitely, there's so much to learn out there in the world.
[19:37] I actually started a, I started in a sauna board and it's called Research.
[19:46] And every time I just keep adding stuff to this board to research, it's never ending.
[19:52] Like, I don't, I don't know. - Ooh, there's more.
[19:59] Yay. - Oh, I think we both clicked it at the same time.
[20:03] - And write lots of small functions that do just one thing without side effects
[20:08] instead of a couple of big objects. Bonus points if your functions take other functions
[20:13] as parameters or returns new functions. - And that's where it like,
[20:19] because when you, so Python is an object oriented programming language.
[20:25] And when you are learning how to write production level Python code,
[20:33] as opposed to just this code does the thing that I want it to do, you know,
[20:40] when you're making it better. A big principle.
[20:45] I mean, really with any programming language, a big principle generally is to write really small functions
[20:51] that do exactly one thing and then without side effects and work up, you know, from there.
[20:59] Like I learned that in my CS1 class, which was in C++, which is not, you know,
[21:05] it's very far from Python, but also has objects. So like, it's still, there's so much,
[21:15] there's so much overlap between philosophies and also declarative programming
[21:20] versus imperative programming. And so I think functional programming is maybe jives a bit
[21:27] with declarative programming, but it's not exactly declared. It's this, I am too tired for this today.
[21:35] - I was just about to say, I'm not quite computing what you're saying,
[21:41] but I do think it is something that we are definitely, we're a little out of it today.
[21:48] I feel like we both are. And maybe it's daylight savings.
[21:51] Maybe it's just getting into a new, you know, time. 'Cause we are streaming.
[21:57] We just started streaming later than we normally do. - Except it's earlier than it's supposed to be
[22:03] because of spring forward. - Yeah.
[22:07] - I hate daylight savings. I hate it.
[22:10] - I agree. I agree.
[22:12] And really confusing is Europe hasn't, I don't know how many other places
[22:18] in the rest of the world I just have talked to a few. - Yeah.
[22:23] - My company is, yeah. - Yeah.
[22:26] That's because we moved. So we used to spring forward in April
[22:31] and fall back in October, but then we squished standard time on both ends.
[22:37] So now instead of starting standard time in October, we start it later.
[22:40] We start it in November. And instead of finishing standard time in April,
[22:44] now we finish it in March. So it just got squished.
[22:47] - Oh, and hi, Ian. - Hey.
[22:52] - We are, we're misc Monday, Ian, but we're both a little brain dead.
[22:56] So our misc Monday, Ian, isn't going. I don't even know how to say that.
[23:04] - I don't know. I think, you know, miscellaneous Mondays, right?
[23:07] - Yeah. - So there are no rules.
[23:10] We're doing great. - No, there are no rules.
[23:13] There, I am glad that we're, you know, getting this out today 'cause tomorrow's,
[23:17] I actually need to be able to consume the content of Dita Kafka.
[23:27] - Doesn't Ramon have a, it's like Captain Pat Pat or something
[23:31] where you like pat yourself on the shoulder? - I don't know, but I want to do that right now.
[23:37] - I want to say to ping Ramon and be like, isn't that a thing?
[23:42] 'Cause I don't think I made that up. - Ian, I've been talking a lot about you
[23:48] and your lights in the background, in case you were curious.
[23:52] I will say there is something, especially because you two are Pythoners,
[23:57] you and Ian, of eventually, I want to see how much I can automate on my,
[24:05] to get it to do after I stream something. Like, I don't know if it's possible,
[24:11] but if I stream a video on OBS, so it like downloads to my computer,
[24:17] can it then upload to like, let's say- - Everywhere else.
[24:24] - Rev.com or something to translate it or to transcribe it and then somehow tell my computer
[24:32] or something to put it on YouTube and also put it on a blog post
[24:41] to translate and embed the video. I don't think this is possible,
[24:47] but it'd be really cool if it was. - I think it probably is possible,
[24:53] but I have no idea how to do it. - Oh, so Ian says,
[25:01] he has OBS recorded streams and upload to YouTube later, which also does transcription in various languages.
[25:12] Yeah, so YouTube does transcribe. - Yeah, I want to do it on its own,
[25:18] like almost blog post with the transcription in there. - Yep.
[25:23] Yeah, you can get that in OBS. You don't have to upload it.
[25:31] Ramon showed us how to get transcription. - That's closed caption and it doesn't transcribe.
[25:39] - Well, there's a button. - There's a button?
[25:42] - Yeah, so that you can download it. - Oh, but it's still a manual process.
[25:48] - No, like when you set up the- - It would auto download?
[25:54] - I think so. Basically, I'm realizing I need to automate my life.
[26:00] - Right? - I do a lot of stuff manually.
[26:04] It took me, this is so silly.
[26:08] It took me like three hours yesterday to create the graphics,
[26:15] write all of the like social media posts, then post on all of the social medias.
[26:25] And that took a really long time. - Chat does take forever.
[26:37] I mean, if you want to join on the stream, we'll send you the StreamYard link in.
[26:43] You're welcome to join us. Like you want to join this conversation.
[26:47] - Yeah, I really want to find a lot of APIs in my life. It's to the point I'm at
[26:56] as there needs to be more APIs in my life. - Yeah, I have been learning.
[27:06] Well, I have been preparing to learn, sorry. - Say the funny way.
[27:13] - Yeah, okay. Wait, you mean the one that I want to make a series for?
[27:20] - Uh-huh. - Okay, yeah.
[27:21] So I have been getting NeoVim set up, which is a fork of Vim
[27:28] with a better plugin ecosystem and some other improvements. And I need to learn how to use it.
[27:36] And so I'm going to do a series of, I don't know, I guess, probably both blog posts and streams called...
[27:43] Oh, and when you want to invoke NeoVim, instead of typing Vim, you type nvim.
[27:51] And so I want to have a series called Becoming InVimcible in which I learn NeoVim.
[28:00] - This is happiness. - Yeah.
[28:02] Yeah. But today I'm tired.
[28:07] - Yeah, today we're just not computing life. Alias, oh, alias by...
[28:18] - Vi equals nvim. - Mm-hmm, yeah.
[28:22] So Vim is Vi Improved. So Vi came first.
[28:29] And then Vim was Vi Improved. So it's already like a cute name, Vim is.
[28:40] And then there's NeoVim, yeah. - Oh.
[28:46] - There's also LazyVim or LazyNeoVim or, I think it's LazyEnvim.
[28:53] Anyway, there are a bunch of these things. Oh, yeah.
[29:00] So that alias that... What were you...
[29:08] How were you saying it? I'm just gonna try it the same way.
[29:10] - Akai. - Akai, and just try to be consistent.
[29:14] So this would be like an alias that you would put into your shell file.
[29:20] So like we, many streams ago, edited your .zshrc, your zshell configuration file.
[29:29] So this is something that you can put in there. So I have various aliases in my zshell.
[29:34] Things that make it faster to like get to particular directories
[29:40] or I don't have to type out like git checkout main, I can just type gm and stuff like that.
[29:47] And so, yeah, you can alias it, but that file is local to your machine.
[29:54] It doesn't follow you to whatever machine your fingers happen to be typing on a keyboard
[30:01] that is interacting with. And so you have to remember either
[30:06] you're gonna have to adjust the zshell or this would work in Bash too.
[30:12] As adjust your shell configuration everywhere, or you just have to remember like,
[30:16] oh yeah, these shortcuts aren't going to work here because we're not in Kansas anymore, so to speak.
[30:23] - Okay. Yeah, I'm not computing anymore, y'all.
[30:33] I'm blaming Daylight Savings. It's just what I'm gonna go with.
[30:38] - Daylight Savings is the worst. I mean, okay, I try to appreciate in my being
[30:45] that there are people for whom... Okay, so you know seasonal affective disorder, right?
[30:54] Where people experience more depression during the winter. For me, it goes the other way.
[31:04] My seasonal affective disorder means that I have more depression in the summer
[31:08] and I feel great in the winter. But it's interesting to me 'cause I feel like
[31:15] we don't have any data on how people experience their seasonal affective disorder
[31:21] separate from standard time. Because there are people who say like,
[31:25] oh, I don't like being on standard time because it makes me depressed, you know, whatever.
[31:32] But it's like, that also occurs when the season changes. Right, so how do you know that it's the standard time
[31:40] and not the season? Control your variables, you know what I mean?
[31:45] So like, there's that. But anyway, so some people like Daylight Savings,
[31:52] even if they don't have a seasonal affective disorder, they like Daylight Savings because they like
[31:57] having more sunlight at the end of the day. I don't, not only because I hate sunlight, not true,
[32:06] but like not only because I'm not a huge sunlight person in the first place, but because for me,
[32:13] like in the winter, I'll have an experience like, oh, the day's almost over.
[32:20] Oh, actually it's only five o'clock, yay. I have all this more time in my day.
[32:25] Versus in the middle of June, I'll be like, yeah, there's lots of time left.
[32:29] Oh, it's actually nine o'clock, damn. Fair enough, fair enough.
[32:37] That is something I'm still getting used to because in Phoenix, where I grew up and kept moving back to,
[32:47] there wasn't a Daylight Savings, like it just stayed. But the easier way of saying it is that it would move
[32:57] time zones and go to Pacific time half the time and Mountain time half the time.
[33:02] But technically, technically it stayed. And I think that's gonna be, it's hard because I've realized
[33:12] off and on again, I have been in Arizona majority of my life. So I've only been in Denver for two years,
[33:22] that it's been really hard for me to transition to Daylight Savings.
[33:29] And I don't think I thought of it beforehand of how much it really does affect me.
[33:34] - It's actually super unhealthy. The spring forward in particular,
[33:41] there's really interesting research. So because there's been,
[33:46] most people say that they dislike the time change and they wanna just stay on something all year.
[33:57] But I can't tell whether it's actually a majority of people who want to stay put,
[34:05] whether they want to stay on Daylight Savings or whether they're just louder
[34:11] than the people who want to stay on standard. I can't figure it out.
[34:15] So there's a law that federally a state is allowed to decide whether they want to do Daylight Savings or not
[34:27] you can decide I'm not doing Daylight Savings. Therefore I am staying on standard time year round
[34:33] like Arizona does, but you are cannot decide I am going to stay on Daylight Savings time all year round.
[34:40] So there's been this bill sponsored by Marco Rubio in Florida to make it so that states can decide
[34:52] to stay on Daylight Saving time. - I've only heard of people that want to just not change.
[35:01] Like there's not one or the other that they necessarily want to stay on.
[35:09] They just don't wanna change anymore. And Ian just post the state has to prove
[35:18] that it will negatively affect the economy making the change.
[35:24] And so Marco Rubio from Florida wants states to be allowed to say
[35:30] that they can stay on Daylight Saving time because there are a lot of golf courses in Florida
[35:37] and they want people to stay on Daylight Saving time because people golf after work, not before work.
[35:45] And so if there's an extra hour of daylight at the end of the day, they can make more money.
[35:51] - Weird. It's probably the opposite in Arizona
[35:57] and why they stuck to whatever they stuck with because it's too hot at the end of the day.
[36:01] - There's that. It's also, it's physically unhealthy
[36:07] because it fucks with your circadian rhythm to be on Daylight Saving time.
[36:12] And there's more cancer. - What are we on right now?
[36:19] Are we on standard time? - We just switched to Daylight Saving time.
[36:25] - And this is the one we don't, that fucks with you. - Yeah.
[36:33] - I like what Ian and Zen Hobbs said. Government bill that supports, oh, wait,
[36:42] that's I forgot the first one, but I think that's like a very fair statement.
[36:49] But Colorado approved a bill that only takes effect once the federal government decides
[36:56] to drop Daylight Savings. And then Zen Hobbs instantly against
[37:04] because CalPERS wants to do it. Don't blame you.
[37:09] - California has a bill. We approved as voters to stay on Daylight Saving time
[37:17] year round in 2018, but that only takes effect when the federal one takes effect.
[37:23] - And Fukai said, there was talk about getting rid of it in Norway, but apparently there's a lot of dispute
[37:30] which time to make it standard plus one or plus two. Because like the company I work for is in Finland
[37:37] and I think they're plus two. I vote that y'all go to plus one
[37:41] 'cause then you're less hours away. - Eight hours is easier to deal with than nine hours.
[37:48] It's a round number. That's a very silly reason why, but for some reason,
[37:53] eight hours has been a lot easier for me to figure out than nine hours.
[37:57] I don't know. Maybe just 'cause it's less an hour.
[38:02] I honestly don't know if it's that or just because it's a round number.
[38:05] - It's also exactly a third of 24. Like you can break 24 into three, eight hour segments,
[38:17] but 24 doesn't divide nicely by nine is a thing. - I need to turn off my ads.
[38:28] Like, whoa, people get that they're like on there to like, you know, help out and stuff.
[38:34] And that's why people subscribe. But like, I thought they would like run an ad
[38:42] like an ad. No, they run like five.
[38:47] - Yes, they do. Yeah, there'll be several ads
[38:50] and it's the same ones over and over again. - That's annoying.
[38:53] Like one ad is something. Okay, well.
[38:56] - I hate Twitch ads so much. - After this stream, I'll go figure it out.
[39:00] I feel like I can turn off ads now. I finally got a job and people can subscribe.
[39:05] Like, you know, it's been a minute, but I got a job. I don't need ads.
[39:11] But yeah. - So there's interesting, like a link between
[39:18] cancer incidences and time zones. - I'm sorry, I'm laughing because you started saying
[39:27] there's a link between cancer and there was a pause and made me think Twitch ads.
[39:33] (both laughing) - Yep, Twitch ads cause cancer.
[39:38] You heard it here first on miscellaneous Mondays. - So sorry, what you said is very serious.
[39:44] Put this over my head first. Like, I'm gonna go work on my Twitch ads
[39:52] to not cause cancer while you tell us about what's going on in different states.
[39:57] - Yeah, I'm gonna, let me see. I could share my screen with this and that might be useful.
[40:04] Is this gonna have like a nice map? Yeah, it is.
[40:11] Okay, and this is really what we want. Open this in a new window.
[40:18] - Can you hear my dog? - No.
[40:29] - That's good. Let me know if you can.
[40:31] - She sounds like a baby hippo. - Okay.
[40:39] - Or a cow. - Uh-huh.
[40:40] (both laughing) - So if anybody hears it, that's what it is.
[40:47] Oh, she left. No.
[40:50] Well, hi everyone. I'm still trying to find my Twitch settings
[40:58] to deactivate my, yeah, my ads and Laura left. Yay, Laura's back.
[41:10] - I closed the wrong window. Brain is very tired.
[41:14] Okay, what was I gonna do? I was gonna share my screen.
[41:18] Okay. Okay, and that is, where am I here?
[41:33] I'm here, yes. Okay, yeah.
[41:44] So we have this map. And so what you can see...
[41:53] Oh no, this isn't the right map. This is a map just showing the time zones.
[41:58] Hang on, let me find. What I wanted was the map that shows the incidences.
[42:03] Why don't they have the map here? Okay, let's try a different one.
[42:13] Um. - I'm kind of just like leaving myself not on mute
[42:21] to see when you tell me you actually hear her. - I heard something just now.
[42:26] Do we have, oh my God. Why are you not showing the map?
[42:42] There was like a... Right, okay.
[42:53] So people who live further west in a time zone, they experience fewer days with natural morning light.
[43:04] And that affects your body. And then that, come on.
[43:13] I'm going to close you so that I can open a different one. Is this one of the ones with the cancers?
[43:22] No, I'm sorry. Maybe we should talk about something else
[43:29] while I find this map because it's super fascinating. - Well, I would think that everybody probably
[43:37] stopped watching my stream 'cause of my hats. (laughing)
[43:43] So, I mean, I feel like we are just having a MISC Monday that is not motivational.
[43:53] This is why we do not call it Motivational Monday. - Indeed.
[44:00] - Which I am very grateful for 'cause, yeah, yeah. Yeah.
[44:10] - Oh, I'm so annoyed that I can't find this now. - Well, I can't find how to turn off my ads yet either.
[44:21] So between the two of us, we are doing great. - Yes, good, good, good.
[44:26] Okay, so let me try. Bye.
[44:36] Maybe it's in here. No, no, yeah.
[44:44] Plus, they only give me 11 cents. That is not worth giving everyone.
[44:49] Oh, you get really, really annoying ads. This is not worth it.
[44:55] - Okay, well, I'm just gonna go back to the same one that I linked to even though it doesn't have the map
[45:00] and that's really too bad, but let me make this bigger. Okay, so if you are further west in your time zone,
[45:09] because like the entire time zone, the sun will actually set later in the day for you
[45:28] if you are in the western part of the time zone than you are in the eastern part.
[45:35] Like the actual light will happen, the light change will happen at a different time
[45:40] even though you're in the same time zone because the earth is not actually cut up
[45:44] into those chunks, right? We made them up is the way that it goes.
[45:49] And so the alignment goes wrong with the circadian rhythms.
[45:56] So that's gonna be true like for time zones in general, but it gets way worse when you add in daylight savings.
[46:04] - Good news, I think I got them turned off. No more ads.
[46:19] I don't know, we'll find out. If people get ads, please let me know
[46:22] so I can think I turned them off. Is that, and Fakai, thank you for telling me 'cause 25,
[46:30] 20 and 15 is annoying. I thought it would be like maybe one,
[46:37] like let's say a 30 second one, but three in a row and you can't skip them.
[46:43] They're not like YouTube, you can't skip them. - Yep.
[46:46] Anyway, so yeah, our bodies are designed for standard time. Standard time meets our bodies, natural circadian rhythms
[46:58] and daylight savings time moves it. And that actually fucks with your health.
[47:05] And so to be, if we did move permanently to daylight savings time, instead of standard time,
[47:14] we would actually have more cancer, more heart disease. All of these things would be worse
[47:21] because we would be permanently on the time paradigm that fucks us up
[47:30] instead of permanently on the one that doesn't fuck us up. - That is crazy.
[47:35] That's bananas. - It's not like it just gets better once you adjust.
[47:40] Like it's not like jet lag where it gets better once you adjust.
[47:44] You may not, you don't notice that your circadian rhythm is wrong
[47:50] but your body knows. And so like over time, it increases your risk
[47:56] for various types of cancers and stuff. - The ad I got was actually for a shampoo ad
[48:09] that they already use. I like that, that is, you know,
[48:15] I get a lot of those ads of things I already use and I'm like, that's not,
[48:20] I mean, I'm not mad. At least I like that, but that doesn't help
[48:27] make you any money because I already use it. Although there are sparkly gold boots
[48:36] that I am not buying yet. I will probably buy them at some point.
[48:41] I wish they had sparkly gold Doc Martens. They do not.
[48:47] So eventually, eventually. But I figured I live stream more than anything,
[48:52] more than in-person events. So I can't really justify something for shoes.
[48:57] If they were glasses, I feel like I could have like justified that one,
[49:00] rationalized it. - Do you have to rationalize having shoes that you like?
[49:10] - Yeah, I have a lot of shoes that I don't wear because I work from home and I never leave the house.
[49:18] Well, as we talked about, I leave the house when I travel. And that's it.
[49:23] More of just like, and plus I don't know if they're comfortable.
[49:29] And I wish I could wear heels because they're pretty. They are very pretty.
[49:40] And I can't because they're not comfortable. So, okay, my dog is like yelling at me.
[49:48] I don't know why, she's an old lady. - I used to wear high heels a lot.
[49:58] And when I stopped wearing them, I developed some foot problems
[50:05] from no longer wearing high heels because my arches are really high.
[50:12] And so I switched, like when I stopped wearing high heels, I started wearing flats.
[50:22] And so there was nothing supporting my arches. I also have extraordinarily wide feet.
[50:27] I have hobbit feet without the fur. Like they're really not very long.
[50:33] They're almost square. I mean, not really, but like,
[50:38] they're really short and really wide. Oh, I think you're muted.
[50:44] - Oh no, well, I was muted because of the dog, but I'm over here laughing, don't worry.
[50:49] - My feet are a size seven in length and between a 10 and a half and 11 in width.
[50:58] - I'm horrible at sizes, so we're gonna go with, that doesn't sound great, but yes.
[51:04] - It's a huge difference. Like that's all you need to know, right?
[51:07] Is that that's like three and a half to four full sizes difference
[51:12] between the length and the width. - And an old boss had to have surgery, hip surgery,
[51:20] because she wore heels for so long that when she switched to flats, it caused hip issues.
[51:27] - Interesting. - Because your calf is not as long
[51:35] as it would be if you were in flats in the front of your leg, something like that,
[51:40] and it affected her hip. But I can tell you that I'm pretty brain dead for today.
[51:47] And I know we've been on repeat. So other than hobbit feet.
[51:53] - Anything else you wanna cover today before we start wrapping?
[51:59] - No, I gotta wrap anyway, I guess, because it's actually almost noon
[52:03] and I have a thing going pretty soon. - Yay, yay.
[52:08] Well, thank you Foucaille for joining us today. And if you're still here, thank you for joining as well.
[52:15] And I am ready to go take a nap, because I'm really brain dead
[52:20] and it's the perks of waking up so early to work with people and it's really early there.
[52:30] So we'll enjoy the rest of your day, and bye, everyone. 
