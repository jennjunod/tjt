---
showLink: "https://www.youtube.com/watch?v=1dOw4v-IDzY"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "dynamic-experiences-using-netlify-edge-functions"
title: "Dynamic Experiences Using Netlify Edge Functions"
publishDate: "2022-11-18"
coverImage: "https://i.ytimg.com/vi/1dOw4v-IDzY/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:07] I know I've been a bit MIA this week with NuxNation, so welcome back.
[00:13] Today we have someone that is pretty well known in the tech community, streaming community, Twitter, all the things, Jason.
[00:22] Jason, please introduce yourself in case people don't know who you are. >> Yeah. Hi, I'm Jason Langsdorf.
[00:28] I am the host of Learn with Jason, which is a show here on Twitch,
[00:32] and also at learnwithjason.dev. I also teach a lot of folks how to build for the modern web over at Netlify.
[00:41] I've been doing developer experience for a long time, and prior to that, I worked in product engineering for a very long time.
[00:50] I'm just trying to find ways to goof around on the Internet and have fun, and see if we can all make this place a little bit less bleak every day.
[00:57] >> Yay. Thank you, especially with everything going on. I feel like that's to everybody going on with tech layoffs right now.
[01:05] I adore you. Please stay positive. I've dealt with that too,
[01:09] so hopefully this gives you a little bit of fun for the day. What up, Anthony? Thank you for joining.
[01:17] Anthony, along with a few other people, were how I found out that Jason existed.
[01:25] Because Anthony was the third person I talked to and was like, "Hey, you should just start streaming Learn with Jason."
[01:36] I'm like, "Who's Jason?" This happened again, and again, and again.
[01:43] There were multiple people that finally I was like, "I should probably reach out to this Jason person,
[01:51] because everybody likes his style and knows who he is." Y'all, I'm pretty sure my first message to him,
[01:59] which I'm still surprised he replied was like, "Hi, I'm starting my stream tomorrow,
[02:04] so you should come on the stream sometime." Yeah, that I think was my awkward way of saying it.
[02:13] People don't believe me how awkward I am in the DMs. I honestly just say,
[02:21] "Hey, can we be friends?" I'm also pretty sure that is how Yarey and I ended up hanging out.
[02:28] Oh, yeah. Y'all are hearing the echo too. >> Uh-oh.
[02:35] >> Let me try swapping mics, see if that helps, because I hear it on my end for myself.
[02:44] >> Yeah, I don't hear it. >> All right, y'all. Is this any better?
[02:53] >> I hear my echo still. >> Well, that's annoying.
[03:02] >> Is this any better? >> No, I still hear myself.
[03:10] >> Is it annoying so much that we got to figure it out, or do we think we can deal with it?
[03:21] >> Wait, it might have gone away. I think it went away.
[03:26] >> Are we good? >> I think so. I'm not waiting.
[03:30] >> You can probably go back to your other mic then. >> Okay. Yay.
[03:35] >> All right, y'all. How is this? >> Check, check.
[03:44] >> I think we're doing better, hopefully. Yarey, let us know if you still hear it.
[03:49] >> Yarey is tuning in from YouTube, just because I auto-stream over there.
[03:56] Thanks for the great pause. Yes. Today, we were going over the history of me being
[04:04] awkward and reaching out to people because that is how I also met everybody that said hi in the chat today,
[04:09] also being awkward because y'all were there from the beginning of the journey. Thank you.
[04:15] >> I will say that in terms of awkwardness in the DMs, you're maybe middle of the road.
[04:22] >> Sweet. >> I get some extremely strange DMs.
[04:27] >> I keep hearing about people getting asked for laptops. >> Yes. That one's a little bit sad.
[04:36] People can't afford laptops and they think that getting a laptop will get them into
[04:41] tech so that they can get a better life, so they just ask for a laptop.
[04:45] >> That makes sense. I guess I just don't understand. Y'all, I've been on my journey of DevRel
[04:53] for almost five months now, but I've been unemployed since January.
[04:59] If people ask me for a laptop, I'm like, mine died. I don't even have the money to afford mine,
[05:04] but that's why I think it's interesting, but you're so right. It's like that dynamic of
[05:09] reading more into it and being able to help more. Or the hellos.
[05:15] The hellos are always fun. The hey. >> Those ones I just have to ignore at this point.
[05:20] If somebody sends me a message with no context, it's stressful enough when it's at work,
[05:26] where you get the DM from somebody on your team that's just like, "Hey, you got to give me the rest of the message."
[05:33] You can start with, "Hey," but then say the rest of the thing, please. >> Yes. Y'all, again,
[05:41] this is how you, what not to do. But yes, my message was literally,
[05:49] "I'm stoked to be on my journey of DevRel, following in your footsteps of a bit,
[05:53] but from being a total noob, I'm going to start Teach Gen Tech."
[05:57] Then three days later, Yeray was the first guest. Thanks, y'all.
[06:02] Thanks, Jason, without even knowing it, inspiring me to do this.
[06:07] >> Happy to play some small part in this journey. >> Yay. Now, if we're talking about Netlify today,
[06:18] and I'm actually pretty excited because people have talked about Netlify from the beginning,
[06:24] and I'm like, so it's hosting, is what I've gathered, and I'm worked at GoDaddy,
[06:29] so I'm like, okay, hosting. Same, same, I think.
[06:33] But yet, it still has not clicked. I even watched the intro video and I'm like,
[06:38] why is this not clicking? Why are things like Netlify not clicking?
[06:43] How would you describe it? >> Netlify is a little bit tricky to describe because
[06:48] it is built of component parts like hosting, or Cloud Functions, or DNS management,
[06:57] which are all commoditized things that are clear, you understand those.
[07:02] But what we do that's different is, it's like a workflow platform,
[07:09] and the idea is that we're not selling you infrastructure, we're selling you efficiency and productivity.
[07:17] So the value of Netlify, what you get when you choose Netlify as your platform,
[07:22] is a faster feedback loop from idea to something live. Whoa, Twitch just unmuted itself,
[07:35] and I started hearing myself talking to myself. You get a faster feedback loop
[07:41] from having an idea to seeing that idea live on the Internet. The way that we do that is by
[07:47] making it faster to deploy your sites, so that you can get them up and hosted,
[07:51] so we manage the CDN for you, so that they are faster.
[07:55] It's less likely to hit problems if you get a lot of traffic really fast.
[07:59] We automatically deploy and scale serverless functions. We give you tools like
[08:05] redirects and proxies that make it easy to set up an API-like thing if you want
[08:10] your site to have a slash API slash episodes. For Teach Gen Tech, for example,
[08:15] you can do that with a serverless function and a redirect that will give you
[08:19] the ability to stand up this API in a few minutes, instead of having to figure out how to set up a Node server,
[08:24] and then where does that Node server run, and how much does that cost,
[08:27] and how do I get the Node service plugged into my website service,
[08:30] so they're both on the same domain? All these things that are tricky.
[08:35] With Netlify, you just get to have these ideas and do them very quickly,
[08:39] and they're up and running. We also offer local development tools so that you have
[08:43] the ability to get our CLI, for example, and you can run Netlify Dev.
[08:47] We'll auto-detect which framework you're using, we'll start it in local development mode,
[08:51] and also we'll be running your serverless functions, your edge functions, anything that you're running there,
[08:56] and we'll pull in your environment variables so that you can set the environment variables once,
[09:01] and then they're available locally, they're available in staging,
[09:03] they're available in production. You're not dealing with.n files,
[09:06] you don't have to figure out how to ignore them locally so they don't go into GitHub, but still use them,
[09:12] and then you have to put them somewhere else so that they get loaded in production,
[09:15] and all that kind of dance of trying to keep things secure. There's all of these just little things.
[09:21] So maybe the biggest pitch is, what Netlify is doing is it's removing
[09:26] what I've started calling undifferentiated labor. So if you think about the amount of work
[09:33] that you have to do to build a website, there's your actual idea.
[09:37] So there's the design, the logic, the interface. That's the valuable part.
[09:42] That's the piece that you need to create because it's unique.
[09:46] And then there's all the stuff that has zero difference from every other website on the internet.
[09:51] You need a CDN, you need hosting, you need it to be up and running,
[09:53] you need it to be deployable, you need to make sure that the CI/CD starts
[09:57] whenever you make changes. All of that boilerplate and all of that configuration,
[10:01] it's undifferentiated. It works basically the same for every website.
[10:04] So there's not really any value in you doing it yourself, right?
[10:09] And when you hit an edge case where you need to do it yourself, great.
[10:13] But for the vast majority of use cases, it's just not worth your time.
[10:17] And so that's where Netlify becomes value is it saves you from having to do all this stuff
[10:22] that's the same every time. So you can focus on building the unique value
[10:26] of whatever project you're working on. - Interesting, 'cause it almost,
[10:32] because I think like so many of us like, okay, in the new world, even more new than me,
[10:37] I don't think a lot of us knew like how to set up a website. And even when in the GoDaddy world,
[10:44] 'cause that's what I compare a lot of it to, is going to be like, oh, hey, like this is,
[10:52] you know, if we're gonna build hosting, I'll probably do WordPress.
[10:55] You know, that's where like so much of it went to, like that was kind of like the slightly more technical,
[11:01] but y'all just for now, so you know, my websites are totally built on Squarespace
[11:05] because I was like, I needed something quick and I don't want to think about all of this,
[11:10] but as I'm building up my own technical knowledge, homie, which I'm guessing will be here at some point,
[11:17] if not, you'll just have to hear this in the recording. It's reminding me that I need to start doing
[11:23] a real developer website, not a, you know, plug and play website, so.
[11:29] - Yeah, and I would, I mean, especially as you're pretty early on,
[11:33] I would really encourage you not to use words like real developer, just because it,
[11:39] like if you built something for the web, whether you used Wix or Squarespace or whatever,
[11:44] you're a real developer. You're making something for the web.
[11:47] And like, 'cause the pitfall of making that distinction of like what's real development, what's not,
[11:54] is that there's always an abstraction under the abstraction. Even somebody who's writing like C-sharp on the backend
[12:01] and, you know, doing like ultra low level stuff, they're not, you know, they could go deeper.
[12:06] They could understand how the byte code works. They could understand how the binary works.
[12:10] They could understand how the actual hardware on the circuits works.
[12:13] You could get all the way down until you're talking about how do we teach rocks to think back in the day, right?
[12:18] And that whole piece, the trick is, is that it becomes a moving goalpost.
[12:23] And the reason I think it's important to not frame things that way is,
[12:29] I think one of the major challenges for so many people is that as soon as they've learned something,
[12:35] they assume that that thing is no longer valuable. And they think, because I could figure this out,
[12:40] it's not hard, it's not real. Only the stuff I don't understand yet is hard or real.
[12:45] And then they hold themselves back from ever giving themselves credit as being capable,
[12:50] despite the fact that like they built all this stuff. Like how many people out there have,
[12:54] they don't even know how to get a website up on the internet even if they have a tool like Wix
[12:58] or Squarespace or whatever. And they would look at you as like,
[13:01] dang, you're a web developer. And that's true, you are.
[13:04] And I think that's the, it's important to recognize the value of what you can do,
[13:08] even if it's not like what you've seen somebody else do. - And I so appreciate that because it really is something
[13:16] that we all need to remember. And Wesley Faulkner was the first person I met
[13:22] on this whole like DevRel journey of me awkwardly replying to people in Twitter.
[13:27] It was really, really awkward on this thread. Many of you were part of this awkwardness.
[13:31] So it was, I was talking to Wesley and first he was like the first person that was like,
[13:38] yeah, you can be ADHD and dyslexic and be a coder. Like you totally can.
[13:42] I'm like, you can? And so there's a lot of tools that I'm learning for that.
[13:50] But one thing that he said that really matches what you said was the fact he's like,
[13:55] many, many people will say, if it's easy for me, it's not a skill.
[13:59] If it's hard for me, it's a skill. And I'm like, damn.
[14:06] I feel like you just like said that in a very, very different way.
[14:09] Yet we had a Twitter space yesterday with, about DevRel's actually,
[14:16] really, really good Twitter space. And we were talking about how advocacy is like really like
[14:24] just doing streams or blogs or Chad from Tech is Hiring. We were like, yeah, you're a DevRel.
[14:30] Literally advocate for people to find jobs. Like you were doing the work.
[14:34] And I think it is that mindset that you're talking about of, yeah, it might not be the level I wanna be,
[14:41] but you're right. Further than I was even four months ago.
[14:45] - Well, and that idea of like, if I can do it, it doesn't feel like a skill.
[14:48] Like I got this put into perspective pretty sharply a while back where I got the chance, I was in Las Vegas,
[14:56] and through just a friend of a friend, I'm connected to the personal trainer
[15:01] for the Cirque du Soleil folks that run O at the Bellagio. And so I got invited to go backstage at O
[15:07] and kind of see how the show runs and meet some of the performers and all this stuff.
[15:11] And for the people who are in Cirque du Soleil, that is the most mind bending thing to me.
[15:18] These are people who are, they're doing flips a hundred feet in the air.
[15:22] They're doing these incredible stunts and to them, that's a job.
[15:28] It's not hard. It's not exciting.
[15:30] It's not scary. They do three shows a day and they're just,
[15:33] it's just a boring job. They're looking forward to their weekend.
[15:36] They wanna be done. And so no matter what the thing is,
[15:41] no matter what the skill is, if you do it often enough, it ceases to have a like personal challenge
[15:47] because it's now a thing that you've gained a high level of skill at.
[15:51] And it just turns into like the boring thing that you do before you get to your weekend.
[15:56] And so I think that's a, that was really good framing for me
[16:00] when I saw that like somebody would be at Cirque du Soleil, they're up on stage, do some wild stunt,
[16:05] and then they like do their performance, flounce off stage, and then they get behind the curtain
[16:10] and they just light up a cigarette and look bored. (laughing)
[16:15] And it kind of like blew my mind that that is, you know, you would think, right?
[16:19] I would think that they would get off stage and they would stay in peak performance and like, okay,
[16:22] must practice, must be like paying attention. And nope, nope, not at all.
[16:26] They're like, they're texting, not paying, they're complaining about, oh, I gotta work tomorrow.
[16:30] I gotta cover for so-and-so. Like, it's wild, absolutely wild.
[16:34] - And I just love the fact, so y'all, I don't know if any of you have emceed or done anything,
[16:41] like a lot of speakers will like go on stage and then you're like one and done.
[16:46] As an emcee, you're constantly having to go on stage. And I just relate so much to what you just explained
[16:51] 'cause as soon as somebody else was talking, I was like. - It's like that Ben Affleck meme
[16:56] where he's like standing outside his front door just like with a cigarette.
[16:59] (laughing) - Yes, 'cause like, I was just like, okay, we're done.
[17:03] And I had somebody on the other screen and they were just like, yeah, you can relax now, it's cool.
[17:09] I'm like, okay. So I'm really excited that Cirque du Soleil
[17:13] does the same thing. And yes, they make it look so easy, it's true.
[17:18] But I'm excited 'cause I think I'm gonna use this opportunity to also maybe start setting up
[17:24] my website again. I feel like Tommy would be so happy
[17:26] 'cause he keeps bugging me to have a real website. Okay, there is a real website.
[17:32] It's a more technical website. There we go, a more technical website.
[17:37] - All right, so here's what we can do today. We've got another like 40 minutes, right?
[17:42] - Technically if you wanna go for the full 90, we have-- - Oh, full 90, okay, yeah, let's do it.
[17:49] - An hour 10, but if you wanna do 40, we can do whatever. - I know, okay, so here's what I think we can do
[17:55] within the span of the next hour 10. We can get you set up with a local repo.
[18:04] We can get local development running. We can get it deployed to the internet with some basic text
[18:09] and make it so that whenever you make changes and push, it will update the site.
[18:13] - Ooh, okay. - And I think we can, yeah.
[18:17] And depending on how that feels, we can also look at doing some personalization stuff
[18:22] or some kind of fancy, like we'll call it jazz hands for the website.
[18:28] (laughing) But yeah, so do you wanna just kind of dive in here?
[18:34] - Yeah, I definitely do. And real quick, just catching up on a few of the chats.
[18:41] Is that like the full Monty? I'm not gonna lie, I totally missed what this one was for.
[18:49] So yes, sure, why not? And thank you for the compliments on the emceeing.
[18:57] I'm glad to see that you are here and definitely ask us questions.
[19:03] It was a fun couple of days. And oh, yeah.
[19:07] Ooh, I like that full Monty being the full 90. I get it, I get it now, thank you.
[19:12] Okay, so getting started, I'm guessing I need to go to Netlify.
[19:18] - Yes, so this is kind of where we're actually starting. So if you want to sign up,
[19:26] you can sign up with your GitHub account. - Sign up, GitHub, yay.
[19:32] - Make sure I have my phone here. - What this will do is it gives Netlify
[19:38] the ability to list your repos and also listen for changes on them.
[19:41] So this, is it gonna let you, you might be able to skip this
[19:48] or you can just kind of like power through it. - Oh yeah, we'll just, we're doing this for work.
[19:55] - Here we go. - Yeah, I'm a, we'll say web designer.
[20:01] I like it. Company of me.
[20:04] My first product will be marketing your company site. I just said, other.
[20:13] All of you. - That's right, that's right.
[20:17] - I'll just say everyone. And name of my, oh, let's see if I can type.
[20:26] Name or company is teaching tech. Oh, you didn't auto do it.
[20:30] I hate that sometimes I don't know when it's actually gonna auto do this stuff, so.
[20:35] - You guys teach Jen, teach. - Oh, did I really?
[20:39] - It's all right, you can fix it later. - All right, well that's good at least.
[20:44] - Okay, so you can skip this step for now because we're gonna set up from local.
[20:51] So up at the top, there's a skip link. And this is your dashboard, okay?
[20:56] So if you want to fix your team name, you can go to team settings at the top right
[21:01] under that upgrade button there. - Thank you.
[21:05] And y'all, I didn't put in my contacts today, so I'm also really blind.
[21:10] Because I don't know if anybody's ever done this, but you're like, hey, I have 30 minutes to get ready
[21:17] and do stuff, so I'm gonna do it really slow. And then the next time you look at your phone,
[21:21] it's time to start. And I'm like, oh shit, and ran to my computer.
[21:24] So I don't have glasses, I don't have anything. I'm just like, I can see.
[21:28] I'm gonna squint at the computer a lot, but all right, I'm gonna,
[21:31] thank you for telling me how to fix that. All right.
[21:36] - This is actually all you need to do for right now. So do you have a terminal that you prefer?
[21:42] - I actually think that, I've been needing to come up with a reason
[21:47] for James Quick to come on the show. Like we've talked about it,
[21:52] and I think this is why I'm gonna ask him to come on the show.
[21:55] They're like, I keep meaning to do this, and his is like so cool.
[22:00] - Yeah, there's some really fun stuff you can do with a terminal.
[22:03] Do you have Node installed? - Yes.
[22:05] - Okay, so do npm install. And we're gonna do netlify-cli.
[22:15] And do a -g with a space before the -g. And what that's gonna do is it's gonna install
[22:27] the netlify-cli globally. So that you can just type the netlify command.
[22:32] And so there's the full command, which is netlify, or there's a shortcut, which is ntl,
[22:37] if you wanna use fewer characters. And so this is gonna give us the ability
[22:42] to set up new sites. It's gonna let us do local dev.
[22:47] We can manage environment variables. We can do a whole bunch of things from here.
[22:51] So do you have a preferred place to keep sites? Actually, do you already have a site
[23:00] that you're working on right now? - Solid question.
[23:06] - If you wanna-- - I found glasses, I'm very excited.
[23:10] - If you wanna start from scratch, it's actually like that'll, you know, that's even fewer--
[23:13] - Yeah, let's just start from scratch. - Okay, so make a folder wherever you want it to be,
[23:17] that's gonna be your website. - Oh, I should've known.
[23:24] ♪ Do, do, do, do, do, do, do, do, do, do, do, do, do, do ♪ I have to think, is it M-D-I-R to make a folder?
[23:35] - M-K-D-I-R, so make the-- - M-K-D-I-R. (laughs)
[23:38] - Yeah. - I always forget, and I'm just gonna call it this,
[23:41] 'cause then-- - Okay, so then move on in there.
[23:44] - Yay! - And do a git init.
[23:50] So we're gonna set this up as a new repo. - Okay, and then do you have a preference
[23:58] on like what you wanna build with? Do you wanna use plain HTML?
[24:01] Do you wanna use React? Do you wanna use Framework?
[24:06] - I feel like maybe I should do stuff like React, only because it's like what I started learning with Anthony,
[24:16] but then there's Next, with Next Nation kind of stuff, and it's like--
[24:20] - How about this? Let's not force that decision today.
[24:23] We'll just do a plain old HTML, and then you can switch over
[24:26] to whatever framework you want later on. So right now, do you have VS Code?
[24:33] - Oh, I don't think this ever got fixed, but let's see if it did.
[24:37] No, no, you didn't. - You have not found code, okay.
[24:39] - It likes to do that. If I just go manually do this really quick,
[24:43] it'll reopen, so just a sec. This is something...
[24:49] I have to do this manually every single time. Not sure why.
[24:54] - Yeah, that's... - It's a thing.
[24:56] It's cool. Ta-da!
[25:00] - Okay, so let's create a new file. And let's just call it index.html.
[25:11] Okay, and then if you type an exclamation point, it should let you auto-complete with all the...
[25:22] There you go, hit Enter. - Ooh. - All right.
[25:25] So that's an eminent abbreviation for a blank HTML document.
[25:29] So on line seven, let's edit document to teach-gen-tech. Okay, and then on line 10, let's add an h1
[25:46] and put teach-gen-tech in there as well. - So I don't know if Yare is still here,
[25:53] but this, everything you just said, when I first started,
[25:58] I wouldn't have understood anything you just said. - Well, you just killed it.
[26:03] You just did great. - So, Yare, it's been four months, almost five,
[26:08] and I've learned a lot, so thank you. - Excellent.
[26:11] All right, so save that. And then let's go back to your terminal.
[26:16] - And could we just do it in here? Is it, what is it?
[26:20] - We definitely can. I think it's a Control-Backtick or Control-Tilde.
[26:26] - Here we go. - There it is. Ooh, that's fun.
[26:30] - Yeah, look at it. - Let's do a... Just, let's see, we're in that folder.
[26:34] Yeah, so let's do ntl space dev. - Ntl space dev, what is this?
[26:43] - What happened? - Is it the font?
[26:46] But the rest of the fonts are good. - Yeah, it looks like something weird happened.
[26:51] So it's gonna try to open a tab. That's gonna be your dev site.
[26:54] - Okay. I don't know why it didn't do it on that one,
[26:58] but there we go. - All right, so this is your running site.
[27:02] So if you wanna make this one like half the width and then make VS Code the other half the width,
[27:08] then we can kind of work in here-- - Never, you know, like, do something,
[27:13] something, you know, that makes it easier for all of us. That would be way too fun. (Ben laughs)
[27:18] Good call, good call. All right. - Okay, so then if in here
[27:22] you wanna add like a, you know, a little paragraph that just says like, "Hey, everyone,"
[27:25] or something like that, just any change you wanna make. Okay, and then if you save that,
[27:42] you can reload the page on the right. - Yay!
[27:48] - Okay, so this is because we're using plain HTML. There's no hot reload or anything
[27:53] 'cause there's no framework to actually set that part up. But as you're building now, this is functional.
[27:59] It's working. So this, I think, is a great start.
[28:04] Let's go ahead and deploy this site. So if you wanna go into your terminal
[28:07] and hit the Control + C to stop the process, okay, then do a git status.
[28:16] - I'm not gonna lie, I'm going back over here 'cause I don't-- - Yeah, something weird
[28:22] is going on. - (laughs) - Okay, so then you can just git add -A
[28:31] to put all those files into git there. We just need the two.
[28:35] - Git add with a capital A or just git add? - Git add. - Okay.
[28:42] - And then a dash capital A. - Dash capital A, great.
[28:45] - Yeah, so that's like, the capital A is a flag that says add everything, add all.
[28:51] - Okay, okay. - So then if you run git status again,
[28:53] you'll see that they're ready to commit. - Yay! - Okay, so then
[28:57] we can do a git commit and whatever message you want. So -M and then, you know,
[29:02] I usually just call it initial commit or something. But yeah, perfect, okay.
[29:07] So then the next thing that we need to do is we need to create a repo on GitHub.
[29:11] Do you have the GitHub CLI or do you work from the UI? - I don't remember. - Do vh dash v, gh.
[29:24] - Vh dash, I mean, that would make sense. - And then a space before the dash v.
[29:28] - Yay, I do. - You do have it, okay. So do a gh space repo space create.
[29:39] And this is gonna create a new repo on your site. You wanna push an existing.
[29:48] Oh, yeah, you can create an... Actually, you know what, it's easier if you don't.
[29:52] So hit Control + C and start again. And do the existing.
[29:58] - Here we go. - And you want this one, so you can just hit Enter.
[30:04] - Yay. Yes, right. - Okay, you do wanna
[30:11] add a remote, yep. - That's fine. - And that's default.
[30:16] And you do wanna push the commits up. - Yay. - Okay.
[30:21] So there are two ways that you can create a site on Netlify. So let's go with probably the most visual one.
[30:28] So go back to your browser and go to your Netlify dashboard. And let's make this bigger.
[30:33] You can go to Sites and Import from Git and use GitHub. And this is just gonna check that you are allowed
[30:49] to look at all of those things. Okay, and then configure on GitHub.
[30:56] You might have said it could only have no repos and you've gotta flag 'em individually.
[31:02] So hit gengenod, all repos. - There we go. - Yeah.
[31:06] And so you have a choice here. You can either do it like if it's a company org on GitHub,
[31:14] you can choose one repo at a time so that you keep security locked down.
[31:18] For me, because I pretty much put everything on GitHub, it's a shortcut to let it see all repos.
[31:24] And I'm not putting anything out there that, nothing goes on GitHub that I'm worried
[31:30] about other people seeing. I think all of my repos are public.
[31:32] Okay, so now that you got that, you can, there it is. And all the defaults are good.
[31:43] So you can just go down and hit Deploy. - And hi, Sudo.
[31:50] And yeah, maybe it is permission things to binary. I broke my computer doing that once,
[31:58] trying to fix it with Bash. So I just haven't messed with it in a while, but yes.
[32:04] Okay, we got this going. - All right, so it's deploying your site.
[32:08] If you scroll down a little bit, it's going to, you can click into that deploy
[32:13] or actually even a little bit lower, you'll see the actual deploy happening right there,
[32:19] where it says building. So you can click into that one there that says building.
[32:28] And this will kind of show you what's happening. Actually, it's already done.
[32:31] So you can open your production deploy. - I was like, they didn't have a lot to do, so.
[32:38] - And there you go. You now have a deployed site.
[32:40] And so this one, there's a couple things to note. Netlify will do a like published production deploy,
[32:50] and then it will do a tagged deploy for every Git commit. So that what you're able to do is you can like review work,
[32:58] you can go back in time and see how your site's evolved with every commit.
[33:02] - Oh, that's cool. - And then we also do something
[33:06] where if you open a pull request, we'll build the pull request.
[33:09] So you can see the live production site and what it would look like if you merge the pull request
[33:14] and review before you make that commitment. - Oh, that's very cool.
[33:20] - And that allows things like you can add comments on deploy previews, and that'll sync back to your GitHub.
[33:25] So that if you want to send it to somebody for feedback or something, like you said, you work with a designer
[33:29] for your images, if they were uploading those to your site, you could actually go and like take a screenshot of it
[33:35] and draw arrows and say like, I don't know about this. And then that would go back to GitHub
[33:39] or wherever you're tracking work to do that. So lots of ways to do the collaboration and stuff.
[33:46] Again, this is kind of what I'm talking about with Netlify trying to like remove work.
[33:50] It's a workflow tool, not necessarily just infrastructure or kind of the raw pieces.
[33:57] - Random question. And this is just making me think of like, you know,
[34:04] moving external work away because, you know, having jumped through hoops trying to figure that out.
[34:10] Canva, very random thing, but I use Canva a lot for like my GitHub for our like readmes and stuff.
[34:19] I love using Canva to make it look a little easier to read than just the text.
[34:24] - Sure. Is there anything that does like where people can use Canva
[34:28] or something like it within Netlify or is that still gonna be very external?
[34:32] - So what you can do is there are tools like Cloudinary or Imgix that will allow you to kind of use a template
[34:43] and then slot text in. So if you look at the way that like I learned
[34:49] with Jason thumbnail is actually generated programmatically using a serverless function in Cloudinary.
[34:55] And so I upload the details of an episode or actually I don't even upload the details.
[35:02] I have a Calendly that people book to choose a date for learn with Jason.
[35:07] And then that invite goes to my team. I have an administrative assistant
[35:13] and then Aiden will take that and enter it into Sanity. And then the details from Sanity get used
[35:19] to update learnwithjason.dev, to generate image assets, to update the overlay on the stream
[35:25] so that it's got the right episode title and guest name. All of that happens--
[35:30] - I need to do that in my life. (Jason laughs)
[35:32] - Like I said, I mean, we talked about this before we went live.
[35:35] This has been a slow accumulation of things. So I did it manually for a long time.
[35:40] And then when I realized that I had a process that worked, then I automated the process.
[35:45] And then the parts that I couldn't automate, I hired help for because my job doesn't let me do,
[35:52] I have no time. So. (laughs)
[35:54] - Yeah, that's why I'm like, there's so many people I've been like, oh, I haven't replied to them
[35:58] or the podcast I have has been put on pause 'cause I'm like, there's only just me.
[36:03] - Yeah. - So I get, oh, I'm like even more excited about this now.
[36:09] - Yeah, so many fun things that you can do, right? So let's go back into the dashboard.
[36:16] And go, click on the superb send all. And what this is, so we auto-generated this,
[36:25] but it's kind of hard to remember. So if you go to site settings there,
[36:29] we can change the name of the site to be something better. So scroll down a little bit.
[36:35] And actually, if you make your window wider, that will become a sidebar
[36:38] instead of pushing everything down. - Oh, sweet. - There you go.
[36:41] - There we go. - And so if you wanna change the site name,
[36:44] then you can change this to tjt.netlify.app or teachgentech or something like that.
[36:51] Somebody already grabbed that one. So these have to be globally unique
[36:56] because they're on the .netlify.app space. And then later, if you do decide to make this your main hub,
[37:04] you'll be able to set a custom domain for this as well. - Oh, sweet, okay.
[37:08] - And you can do that through Netlify. There's a domain management option there
[37:11] on the left-hand side. - Which is here, which I probably will end up doing soon.
[37:16] So yay. - So now if you go back up
[37:18] and go to your main details there, you see how it's changed the site
[37:22] to teachgentech.netlify.app? So if you click on that,
[37:26] now you're hosting live at teachgentech.netlify.app. So let's make an edit and we'll see how this all changes.
[37:34] So go back to your VS Code. - And close out of this 'cause you're not my friend.
[37:44] - (laughs) And let's add anything. If you wanna, we can do some styles.
[37:50] We can add more text. We can do, you know, we can add a work-in-progress caveat
[37:55] here or whatever you wanna do. - We'll do it.
[38:01] Let's do that. - Okay.
[38:05] - Yeah, we can do this. - Okay.
[38:08] Oh, I should hyperlink this. Oh, did you already hyperlink it?
[38:31] - Oh, it's helping. - Oh.
[38:33] - Now I know I did something super weird. (laughs)
[38:35] - I was like, did it just, what did you just,
[38:38] now I'm just curious what it just did. - That is, that's an eminent abbreviation.
[38:44] So if you do like a dot something tab in VS Code, it treats it like a class.
[38:51] So basically what just happened is you did teachgentech.com and it was like, is this a tag?
[38:57] And so it thought it was the, it thought it was like an element called teachgentech
[39:02] with a class of, yeah, see, it's trying to do it again. I'm like, now I don't want to think that hard
[39:07] on how to make it, to link it because I don't remember off the top of my head.
[39:13] Yes, Bakari. - I can help if you want.
[39:15] It's an A tag. - Okay, so.
[39:21] - So right before the T, do an opening bracket A space href is the inside the A tag.
[39:29] You'll want to do space and then H-R-E-F. But like inside that first A tag.
[39:38] - Oh, okay. Space href.
[39:40] - Equals. And in here, you're gonna do the HTTP.
[39:48] Yeah. - Oh, not om.com.
[39:56] There we go, Dan. Come on, do it, do it, do it.
[39:59] There we go. And then this will be named, oh, go back.
[40:03] (Dan humming) And that'll need to go inside the A tags there.
[40:13] So you'll want to move that closing one. Yeah, just right in there.
[40:20] Perfect. Okay, so.
[40:21] - Beat, take the assist. - You save that.
[40:23] Now we can go back to the terminal. We can commit these changes.
[40:26] And the shortcut I always use is git commit -am, which is like git commit everything.
[40:33] And then a message. So like add a link or something.
[40:38] - And yes, Bakari, this is. - Oh, you have to quote the.
[40:46] - Add link, added link. - Yeah, yeah.
[40:49] - Go back. Bakari, this has been many months in the making.
[40:53] I actually first talked to Jason before I. - And then git push.
[41:01] - Oh yeah, damn it. Why, I just wanted to all do it at the same time.
[41:06] - You can, if you do have James come on and you talk about terminals,
[41:11] have him talk to you about aliases because you can make shortcuts for yourself.
[41:15] - Okay, 'cause I will say I started using it in here instead just by like as a way to like just check myself
[41:25] because it'll error out a little definitely. But yes, yay.
[41:30] Okay, so. - Yeah, okay. So then if you go back to your Netlify dashboard,
[41:34] when you look at your deploys. So you can see now the site is already building.
[41:45] It deployed in four seconds, so it's already live. So if you go back to the teachgentech.netlify.app
[41:49] and reload. - Yay. - There you go, right?
[41:55] So this is the workflow. This is why I get so excited about Netlify
[42:02] and why I'm always telling people to try it out is you've got this local dev workflow
[42:07] where you build locally, you try things out, you see that they're working,
[42:11] you commit them to GitHub and push and they just go live and things just work.
[42:15] So then the next piece here that we can do is really whatever you want.
[42:23] There are a few things that we can start looking at. There's, we can build an API
[42:27] using some serverless functions. We can look at doing some personalization.
[42:34] We can show what city people are visiting your site from. There's, yeah, a lot of options.
[42:42] - I feel like, I would say the API and then if we have time,
[42:48] then the city that they're tuning in from. - Great, let's do it.
[42:52] So let's start by going into VS Code and open up your file browser again.
[43:01] And we're gonna create a new folder and call it Netlify.
[43:09] And then inside that folder, create another new folder called functions.
[43:17] Not the .NET, yeah, sorry, that one. - Okay, I just wanted to make sure I was like,
[43:20] wait, did that just suddenly appear? - The .NETlify is like caching and stuff that we do
[43:25] to make sure that it's hooked up to the right site on app.netlify.com and stuff like that.
[43:33] But that's, it gets, get ignored and everything. But yeah, if you've never seen it before,
[43:37] it can be a little confusing. - Yeah, I was like, wait, what?
[43:39] Okay, so what was the folder though? Because I was very distracted by that.
[43:42] - Functions. Okay, and then inside here,
[43:48] let's start like everybody does with a hello world file. So do hello.ts.
[43:53] Okay, and so the way that a serverless function works is you are going to get a request made
[44:07] to the serverless function and it needs to return an HTTP status code,
[44:11] which is like whenever you load a website, it sends back a status code usually of 200,
[44:16] which means, okay, everything worked. You can also send back,
[44:21] like if you wanna redirect somebody to another page, that's status code 301.
[44:25] If you can't find the page, that's 404. You may have seen the 404 pages.
[44:30] And there's a bunch more, but really what we care about in this case is 200.
[44:35] So we are going to export. So you can just write export const.
[44:44] Handler. Equals.
[44:49] And then we're gonna make this an async function. So the word async.
[44:56] And then a space and then do parentheses, open and close. - Wait, parentheses is--
[45:06] - Round boys. - Okay, I'm like,
[45:08] why am I suddenly forgetting what a parentheses is? - And then outside of those,
[45:13] like to the right, we're gonna do a fat arrow.
[45:16] So equal sign and then a greater than sign, and then curly boys.
[45:22] - Yay. - And inside of this,
[45:26] so this is the body of a serverless function. Like this is kind of the structure
[45:32] that you need for one to work. So hit enter.
[45:34] And what we have to return for one of these to work is so use the return keyword.
[45:43] And then set up some more curly boys. You wanna put a space after that return, I think.
[45:53] And then inside there's gonna be two properties on this object that we're returning.
[45:59] So the first one is gonna be status code with a capital C. And do a colon and then 200.
[46:09] - Mm-hmm. - And a comma.
[46:14] And then body is the next property name, a lowercase.
[46:19] - Body. - With a colon.
[46:22] And then in quotes, you know, hello or hello world or something.
[46:27] - I can type, y'all. I promise I can.
[46:35] (laughing) There we go.
[46:36] - Okay, so save that. - Mm-hmm.
[46:39] - And next, go back to your terminal. - Doo-doo-doo, and--
[46:48] - And run netlify dev, ntldev again. - Okay.
[46:51] I always forget it. It does not let me just slide and delete everything.
[46:57] (sighing) Netlify dev.
[46:59] - Mm-hmm. And so now what it's doing is,
[47:07] because we created a netlify folder, it knows that there is serverless function.
[47:12] So if you go back into your terminal and scroll up a little bit,
[47:15] we can see that, see where it says now, it loaded function hello,
[47:23] and the function server is listening and setting up a local development server.
[47:27] So that URL next to hello, that's where you'll test this function.
[47:32] So you can copy paste that out and put that in your browser.
[47:37] - Yay! - Great.
[47:40] So you've now built an API, technically. So somebody is sending a request
[47:45] and you're returning a response, right? So typically what'll happen
[47:51] is an API is gonna return JSON. So that way you can send back multiple pieces of data.
[47:57] So like, you know, a message and an ID and stuff like that, right?
[48:01] So let's go ahead and upgrade this to send back JSON. So go back into VS Code.
[48:06] And what we're gonna do is for this body, let's make a variable like above line two
[48:16] and let's call it response. So do, let's, yeah, var works,
[48:23] or you can do const is kind of the standard that I've seen most people do.
[48:27] And let's give it a, so a space, not a colon, and let's give it a name of response.
[48:35] And equals, and then let's do some curly boys. And now let's make the property message.
[48:45] So you can hit, yeah, and a colon. And then in quotes, we can send,
[48:53] we can just move the hello beautiful human into there. - I feel like this should be my goal
[49:02] of the stream for now on is how, can I get other people to say hello beautiful human?
[49:07] Like if I can get them to say it, I have succeeded. I feel like that should definitely be what the new goal is,
[49:14] but so I can delete the body then, right? - You're gonna still need the body,
[49:19] but we're gonna change the way that it works. So get rid of the quotes.
[49:21] And so now what we wanna do is we wanna send back JSON, but you can't just send a JavaScript object,
[49:28] you have to send a string. So we're gonna use JSON, all caps.
[49:34] Dot stringify, and it's gonna auto-complete, yep. And then put the response inside parentheses.
[49:46] - Parentheses exists. - Yeah, and just put response in there.
[49:53] So we're using that variable that we set. And then I don't know if you can put a space,
[50:02] Chat, do you know if a space between a function call works? I don't know, I never do.
[50:07] Like after stringify, I wouldn't put a space there, but I don't know if it actually works or not.
[50:13] I don't know if that's like a style thing or like an actual functionality thing.
[50:17] - I guess we'll find out. - Yeah, save that.
[50:19] And then go back to your browser and reload. - Okay.
[50:25] - And there you go, you're sending back JSON now. - Yay.
[50:31] - So as you get into more and more APIs, you'll have more details that you wanna send.
[50:37] Like you'll want the episode date and who the guest is and what time it started and all those sorts of things.
[50:42] And now they can all go into these responses and you would just kind of add like an ID, date,
[50:50] title, image, whatever. - I was doing this a bit when I was using Prisma
[50:56] to try to build, I was calling it a TweetyTag app. - Yeah, yeah, yeah.
[51:01] - And I was using Ivan's MySQL and then using Prisma to set it all up.
[51:07] I'm still working on it, but I kind of put it on pause because I was like,
[51:10] I don't think everybody wants to get tagged anymore. So maybe I'll just pause that.
[51:15] But this actually gives me an idea to further work on the actual structure.
[51:22] So I could put, well, I'm thinking this out loud at the same time.
[51:27] So I'm like, of course it would be able to have a database because Netlify wouldn't be as cool
[51:32] if you couldn't have a database, so. - Yeah, so you can actually use Prisma
[51:36] in a serverless function. - Okay.
[51:38] - So there's, yeah, there's lots of ways that you can pull this stuff all together.
[51:41] And this is one of the things that I love is we're giving you the raw tools
[51:45] and then you can bring in whatever platforms, whatever additional tools you want.
[51:49] You can work with whatever framework, whatever database system.
[51:51] The only limitation is that like serverless means that you don't get long running stuff.
[51:58] So if you wanna do real-time or like GraphQL subscriptions or something,
[52:02] that won't work in a serverless function, but just about everything else does.
[52:06] So, and honestly, by the time you get to GraphQL and real-time and all those sorts of things,
[52:12] like that's, yeah, it's not. - I'm like, I'm gonna just pretend
[52:16] like I know what you're talking about and blankly stare at you.
[52:20] But I am excited 'cause like with the space that everybody's replying with.
[52:25] - No, everybody's really, we're all blown away by this space working.
[52:28] (laughing) - I mean, leave it to me, y'all.
[52:31] Come teach me something. And I'm really excited.
[52:33] Nick's gonna be on the show next week of like- - Oh, nice.
[52:37] - I'm a clicky person. Like literally, I think there's a,
[52:42] somewhere somebody made a command that how many times I click something
[52:48] when I'm not supposed to click something. It's what I like to do.
[52:50] I get excited. I'm like, enter, click.
[52:53] Oh, shouldn't have done that. But it's a way to break things and learn, so.
[52:58] - For sure, yeah. - Yay, okay.
[52:59] - Okay, so the next thing that I wanna do though is if we go back to this URL, like in the browser,
[53:05] like this is great, but I want it to look more official. I want it to look like it's the actual API.
[53:11] So I want the URL to be /api/hello, right? - Okay.
[53:17] - And so to do that, I would need to, I don't know, like there's a whole bunch of things that you'd have to do,
[53:24] except we've kind of shortcut this in Netlify. So if you go back into your VS code
[53:29] and next to index.html, create a new file. - Why am I suddenly being very blind?
[53:38] Okay, there we go. - Yeah, and call it underscore redirects.
[53:43] - I almost typed underscore. - This is my whole life.
[53:49] I do this all the time. So what we wanna do is we want people to be able to hit API
[53:55] but have it actually use the functions that are located in .netlify/functions.
[54:00] So type /api/star, like the actual like asterisk star character.
[54:11] (laughing) All good.
[54:14] And then add like a couple spaces so that there's some differentiation between the thing
[54:20] and then do slash .netlify/functions/ and then you're gonna do a colon and splat.
[54:36] - Is that actually a word or? - That is actually a word.
[54:41] - Okay. - So this confused me and I think the reason is
[54:48] if you look at the asterisk, it kind of looks like a splat, like if you would like squished a bug or something.
[54:54] And so I think somebody was like, yeah, it's slash splat. And then we just decided to say the whole word.
[55:00] So then add another couple spaces there. - I dig it.
[55:05] - And we're gonna do 200. Okay, so what this does is it's saying
[55:11] if someone visits the URL/API with anything following it, take that URL and instead serve slash .netlify/functions
[55:22] and whatever was in place of the star. So we're rewriting this whole URL
[55:29] and then we're saying serve that as a 200 so that the URL doesn't change.
[55:34] 'Cause by default, if you leave that blank, it would redirect you to the new URL.
[55:38] So like if you had an old site and a new site, you would say like slash old URL to slash new URL
[55:43] and it would just change it in the browser. And usually that's good, but in this particular case,
[55:49] I want slash API to be the URL people use. So I don't want that to change in the browser.
[55:53] So by sending a 200, we say use the slash API but serve this other thing underneath it
[55:58] as what people actually see. - This is really, really weird
[56:03] because like part of working at GoDaddy was working with the DNS,
[56:08] but it wasn't on like this further technical side. It was on just like, oh, you wanna add it to a forward
[56:14] and then it automatically goes in or sometimes it was a redirect within the index.html file.
[56:20] And so this is just kind of like really surreal, like weird. Like, I don't know how else to say it.
[56:27] Like, it's like such a weird feeling, but I'm like, oh. - And the reason that we do this, right,
[56:33] is because this is one of those really common things that really is not fun to set up on your own.
[56:39] And so by making it something as simple as it can be, we're trying to reduce the amount of, again,
[56:46] undifferentiated labor. Your goal is to work on value, not on configuration.
[56:51] So if you save this and then go back to your terminal, 'cause we just created this.
[56:56] So I can't remember if we have to stop and restart or not. Scroll down, reloading redirect rules from, okay, good.
[57:03] So it picked it up automatically. So go back into your browser
[57:07] and replace that .netlify functions with, let's change it to API.
[57:13] Slash hello. - Oh yeah, okay.
[57:20] 'Cause it has to read the file. Got it.
[57:22] - And there you go. You've now set up an API with a clean URL.
[57:27] And this, like, this is the stuff that I love about this. Like, it just, it starts to feel magic.
[57:33] And the other thing too- - It does, and real quick, we do have a question in here of,
[57:39] can you reverse the single linked list on a N-O-N? I'm hoping that makes sense to you.
[57:47] - I don't really know what the, I kind of feel like this might be trolling.
[57:53] - Oh, okay, well. - I'm not sure. (laughing)
[57:58] - I hate that about it though, because I'm like,
[58:00] I never know if it's like a very technical question or if it's trolling.
[58:04] - Well, so this is talking about complexity, right? So when you're talking about the complexity of a program,
[58:09] there's like O, big O notation is what this is called. And so the, like, O of one is ideal
[58:17] because that means that it runs once. And then O of N means that it runs like one time
[58:23] for every item in the list. And then it can get worse.
[58:27] Like it can be O-N squared or O-N, you know, whatever. And so you, so the, you want lower complexity.
[58:35] And, you know, when you'll hear people talk about this stuff.
[58:38] However, I'm gonna say I've actually never been able to pass an algorithms interview
[58:44] because I don't have a computer science degree. I'm self-taught.
[58:47] So I didn't learn like the really deep algorithm stuff. I've never had to reverse a binary tree
[58:54] or do like any of this kind of stuff. And I don't, I mean, would it make me a better programmer?
[59:00] I'm sure it would. I think learning anything makes you better at things,
[59:02] but it hasn't prevented me from having my career. So I, I try not to, I try not to stress too much about it.
[59:09] - Got it. It wasn't trolling.
[59:11] It was a joke, but I feel like it went way over our heads. - So I forget, I forget which, I forget which chat I'm on.
[59:18] My chat only trolls me lovingly. And so when I, when I say trolling,
[59:24] I mean more like teasing lovingly. - I was like, people, I think just realize
[59:30] that I don't always get the stuff. So they try to like say something funny.
[59:33] And I'm like, I don't know yet, yet. I will get there.
[59:38] I will get there. All right.
[59:41] So we got it. So that way it actually says it with the proper URL.
[59:45] - Yeah. So we've got the URL.
[59:48] - Yeah. - And the other cool thing here is
[59:51] we actually have two distinct systems running on the same URL.
[59:55] So you, if you notice you're at localhost 8888. And so our API, which is a serverless function
[60:02] is running here. But if you remove the slash API slash hello
[60:06] and go to that site, this is your index.html.
[60:14] So this is another thing that you don't have to think about because these are two independent systems.
[60:20] Like serverless functions are deployed and hosted and managed in one place.
[60:25] The static website, the HTML file is deployed and hosted and managed in a second place.
[60:30] But Netlify automatically puts together so that it works on the same URL,
[60:34] so that they're all kind of talking to each other. You don't ever have to think about that.
[60:38] And this is one of those things that like, if you try to set this up on Amazon, you can,
[60:43] but you're setting up like CloudFront and Route 53 and API Gateway and S3.
[60:51] And suddenly you're like really looking at a lot of moving pieces
[60:55] that all end up with the same result, which is that you want your functions and your site
[60:59] and your CDN and all these pieces to run on the same URL. So again, it's just, we're trying to keep it simple
[61:06] and as uncomplicated as we can. So let's see, we've got, how much time left?
[61:13] We got like another 30 minutes, is that right? - Yeah, basically.
[61:16] - Okay. Let's see if we can personalize this a little bit.
[61:23] So the next thing that we wanna do is I want to set up an edge function.
[61:29] And if you look at, so like edge functions themselves, if you, let me drop a link in the chat here.
[61:39] And what these will do is edge functions are set up as, all right, I ate an everything bagel earlier
[61:54] and I have like a seed in the back of my throat that won't go away.
[61:57] And it's really, it's driving me up a wall. - I'm sorry, I'm giggling because this weekend at Costco,
[62:03] I guess it was last weekend. It's already Friday.
[62:06] Okay, sorry, that aside, that aside, I bought like a giant bagel seasoning and I'm so excited.
[62:13] (both laughing) - Everything bagel everything.
[62:16] - Yes, I hope it gets better soon. Maybe you'll talk it out.
[62:21] - Yeah, yeah, we'll just, I'm gonna power through it. Okay, so for some context,
[62:27] let's talk about how the internet works. And I swear I'm not trolling you.
[62:31] (both laughing) - I love learning about it, so I dig it.
[62:35] - When someone makes a request for a website, you're in a browser, you type a URL into the browser
[62:41] and you hit enter. So the browser is gonna send off a request
[62:44] with a bunch of headers that say like, I'm looking for this URL, this is the type of browser I am.
[62:49] I accept these types of responses, et cetera, et cetera. And that request then gets to the origin server
[62:56] or the CDN node or wherever the content's gonna come from. And that node says, okay, you've asked for this thing.
[63:03] I do have that thing, so here it is. And it sends back just like our serverless function,
[63:09] an HTTP status code of like, yes, I have it 200, it's fine. And here's the actual content along with more headers
[63:16] like it's a HTML file or this is JSON or whatever it is and the size of it and some other details.
[63:23] And then the browser gets that back. It reads what it's got.
[63:27] It's like, oh, they sent me HTML. I can understand HTML, so I'm gonna take the body of this
[63:31] and format it on the screen the way that it's supposed to be.
[63:34] What an edge function does is it lets us jump in between the request to the edge node
[63:41] and the response to the browser. And it lets us modify things.
[63:45] So we can do things like looking to see if the browser has a cookie set that has permission
[63:52] to see the thing they're asking for. And then we can like redirect them somewhere else
[63:57] if they don't have permission. Or it lets us see if the browser is modern
[64:03] and can support an advanced image format like WebP or AVIF.
[64:08] And then we can replace on the fly, if they requested a JPEG, we can say, hey, actually,
[64:14] you can take a WebP, which will be less size, less transfer, and send that back instead automatically.
[64:23] And you're saving your own bandwidth costs and you're saving the user download time.
[64:28] And then you can do things on the other end where you get the response that's gonna go back
[64:33] and you can transform it. You can say update with the local time.
[64:37] You can update to say, if it's winter, I want this store to show the winter products like coats.
[64:43] And if it's summer, I wanna show the flip-flops and swim trunks.
[64:47] And that, so it's a way that you'll hear this described as middleware.
[64:53] It kind of happens in the middle of the request. So what's really cool about this is it means
[64:58] that we can do things like somebody can request a static HTML site and we can say, hey,
[65:06] how's the weather in whatever city they're in, right? So let's add that functionality.
[65:13] So the first thing that we wanna do, oh, go ahead. - Great question.
[65:17] Because of thinking about how you also have this set up for your site for streaming,
[65:24] instead of using weather per se, could you do it as, hey, this is what the site,
[65:28] like have it change the site based on date and it be a rolling date?
[65:35] - Sure, yeah. Yeah, you can do all sorts of things.
[65:39] Like for example, you could have your site check whether or not it's your streaming window
[65:47] and either show a link to your schedule or show a link to go watch because you're already live.
[65:52] - That is so cool. But, and it could do that, but then it can also do it,
[66:01] like let's say that I set the stream up then or like my schedule up because I've been horrible
[66:08] about that, that's why nobody knew you were coming on this stream until yesterday.
[66:12] 'Cause y'all, that's what I do in my life. I hope people find out in time.
[66:16] But if I made it, like, let's say I did schedule out this entire week, they would see,
[66:24] it would work where I could say, hey, yes, we're going live on Friday.
[66:28] And then when Friday hits, they'd go, could it have it auto switch to the YouTube video too
[66:36] from, can you do stuff like that? - You definitely could.
[66:42] I think in the use case that you're talking about, I would almost do something like we have another thing
[66:48] that you can do on Netlify where you can schedule jobs where you could basically say, rebuild my site every day.
[66:53] And then in the build process, figure out what the next episode is, put that in the next episode slot.
[66:57] Most recent episode, put that in the most recent episode slot.
[67:00] And then you're not doing it with edge functions because you definitely could.
[67:05] But at that point, it's so much that it feels like it would make more sense as part of the site itself.
[67:11] Like what I really like is I think of edge functions as like the sprinkling of personalization.
[67:18] But if it's the same thing for every person, then I'd probably want to reach more
[67:22] toward either a serverless function or there's straight up part of the build.
[67:28] And in the case of a site like yours or mine, where it updates usually once a day,
[67:32] I would probably run a build at like midnight or something to just update for the next day.
[67:38] - That is so cool. Okay, thank you.
[67:41] Thank you for connecting all those dots. Back to, you know, let's get the weather going.
[67:47] - Absolutely. Okay, so let's start by making a space
[67:51] for this to live on the page. So we're going to go into VS Code
[67:58] and go into your index.html. And we can, let's see.
[68:07] Let's do a paragraph tag underneath line 12. And let's say, let's just put the text weather here.
[68:26] (Jason laughs) Or even, you know what?
[68:33] I don't wanna, I think we're gonna run out of time to go get an actual weather API.
[68:36] So let's instead say location here. We'll just show the location.
[68:39] And so what we're going to do then is we're going to
[68:48] save that. And inside that Netlify folder,
[68:56] so not the functions folder, but the Netlify one, create a new folder
[69:00] and call it edge-functions. Okay, and inside, let's add a new file
[69:13] and we'll call it location.ts. And the name doesn't matter.
[69:19] It's whatever you want it to be. So these ones are similar,
[69:24] but a little bit different from a serverless function. So the format for these is gonna be to export default.
[69:30] So the word export space default. - Oh, default, there we go.
[69:41] - Async. And then a space, do some curly boys,
[69:47] or sorry, round boys. A fat arrow.
[69:53] - On the outside, right? - Mm-hmm.
[69:55] And then some curly boys. And let's just start by doing a console.log.
[70:04] Dot log. - I don't know why. I'm like, why am I suddenly blanking this?
[70:11] Console.log and-- - And then inside parentheses,
[70:16] in quotes, do like edge function running. (mouse clicking)
[70:21] Okay, so save that. And then in the root folder next to index.html,
[70:32] create a file called netlify.toml. - Toml?
[70:42] - Dot toml. - Okay, yay.
[70:46] - And inside of this, we need to tell Netlify which pages
[70:53] should run this edge function because we can run it on the whole site,
[70:57] which is probably, actually, we'll just do it on this one URL.
[71:02] But if you wanted to, you could say like, on every blog post, I wanna run this edge function,
[71:06] or on my entire shop, but not on the homepage or something like that.
[71:11] So what we're gonna do is two square brackets. (mouse clicking)
[71:18] Okay, and then edge underscore function. You got a missing n after the u there.
[71:29] - Thanks. - Okay, and then on the next line down,
[71:34] you can indent, that's kind of the standard with this, and then do function equals.
[71:42] (mouse clicking) And in quotes, we'll put in the name
[71:50] of our function, location. And then on the line below that, path equals.
[72:00] And in quotes, we'll do forward slash, so just the main page.
[72:06] Okay, so save that. And I think, let's go back to the terminal.
[72:11] I think we have to stop and restart for this one to pick up.
[72:14] Yes, so Command + C, and then Netlify Dev again. And now, if you scroll back up in the terminal output,
[72:29] you'll see that it also picked up the edge function, so keep on scrolling up.
[72:37] And let's see, where does it show it? And go down a little bit.
[72:43] It shows it somewhere in this output, and I'm not sure. Keep on going down.
[72:49] Little bit more. Command for local development.
[72:56] Oh, there it is, loaded edge. It was right at the bottom.
[72:58] Loaded edge function location. And then you can also see, look, it logged our thing.
[73:02] So the edge function is running. And at the moment, it's not doing anything,
[73:06] because we haven't actually told it to do anything. But what we wanna do is we want to update
[73:15] some of that content. So I want to...
[73:20] Let's start by just logging this stuff. So the first thing we're gonna do is go back
[73:29] into the Netlify edge function that we have in VS Code. And we're going-- - Is that one?
[73:38] - Yes, this is the one. And so we want a...
[73:44] Let's get some autocorrect here. So above line one, let's do an import.
[73:49] And it's gonna be import, and then in some curly boys, space before the curly boys.
[74:01] Capital C context. And after the curly boy, do from.
[74:10] - Would it be on the same? - Yeah, same line, but yeah, lowercase from.
[74:17] And then in quotes, do HTTPS colon slash slash. And it's edge.netlify.com.
[74:31] And the reason that we're importing from a URL is because edge functions run in Deno.
[74:37] And so this is very similar to Node in the terms of the way that we'll write it,
[74:42] but it's the Deno runtime, which has some different rules, including packages live at URLs
[74:47] instead of in imported packages. So now that we have that, we can use it.
[74:54] So inside the parentheses on line four, we're gonna get two pieces of data.
[74:59] The first one is request. And because we're in TypeScript,
[75:05] it's gonna want us to type these, so do a colon. And then capital R request.
[75:11] And this is built into the browser, or built into the runtime,
[75:16] so you don't have to import that from anywhere. And then comma, context, lower C context, colon.
[75:24] Yes. Josh is coming on our show and teaching me TypeScript.
[75:33] - Nice. - He's the one that wrote this book. - Nice, nice.
[75:35] - So he comes on every other week and teaches me some TypeScript,
[75:38] so I'm excited for YouTube. - Excellent. All right, and we got a rogue C in context there
[75:43] instead of an X. Okay, so then the next piece is let's replace on line five,
[75:51] instead of edge function running, let's log context, and no quotes on this either.
[75:57] - Okay. - .geo.
[76:02] - And-- - G-E-O. - G-E-O, okay.
[76:09] And thank you, Nick, for posting those, I appreciate it. - All right, so save that.
[76:15] And then reload, and let's take a look in the terminal. See, you gotta reload in the browser too.
[76:24] Oh, sorry, yeah, you actually, it'll automatically reload those,
[76:27] but so start your server again, Netlify Dev. Okay, now, if you look in the console there.
[76:40] - It did it. - It did it. So it's showing your city, country code,
[76:45] your latitude, longitude. This is pretty exciting stuff.
[76:49] And so what we'll be able to do now is we wanna take that geodata
[76:53] and actually put it into the text. So let's make that happen.
[77:01] And I want to do that through. Yeah, this'll be good.
[77:07] So let's do, let's go back into the edge function. And we're going to get the,
[77:19] get const response, so we can get rid of line five. And instead, we can write const response equals,
[77:28] and then we're going to await context.next, and put some parentheses after next.
[77:44] It's a function call. Okay, so what this does, when you call context.next,
[77:50] is we've requested the homepage, right? So context.next goes and gets the content of that homepage,
[77:58] and now we have it in the response so we can do stuff with it.
[78:01] So what I wanna do is I want to replace the text on it. So let's get the text on the next line.
[78:10] So const text equals, await, response.text with parentheses.
[78:21] It's a function call again. And then I want to, on the next line down,
[78:32] we need to return a response. And so what we wanna do with the response
[78:36] is we're gonna use the built-in response object. So return new, capital R response,
[78:44] capital R response, and inside parentheses, let's do text.replace, and this part we might have to,
[78:56] little trial and error on this 'cause I always get replacers wrong.
[79:04] So we're gonna do the, I'm just doing a quick check in my own console
[79:12] for how this works. Text.replace, and we want to do,
[79:18] the first one is gonna be a, it's a function, so we're gonna put parentheses there.
[79:25] - Wait, within text.replace or outside of it? - Inside the parentheses, replace itself is a function,
[79:37] so we're gonna add some, okay. And then we're gonna use a regular expression
[79:43] like anarchists, so do a forward slash. And then, do you remember what we wrote in the HTML file
[79:53] for, was it like location here or something? - Yeah, I think it says location here.
[79:58] - We want that text. Then a forward slash.
[80:03] - Okay. - Comma.
[80:06] And then let's do a space and context.geo. And then open up your terminal again.
[80:18] I wanna, I can't remember what it was. It was .city.
[80:24] Okay, so save that. And reload your page.
[80:36] Oh, we need to max, we need to match the caps there, so capital L, capital H.
[80:46] - Yeah. - Okay, so save that.
[80:53] Okay, so see how it did a replace? - It did, it put Denver. - That's great.
[81:01] But it's not interpreting as HTML anymore because we just converted it all to text.
[81:06] So we can work around this if we go back into the edge function.
[81:10] And as the second argument, so on line seven, between the blue and pink parentheses,
[81:20] do a comma at the very end there and add response. Sorry, just like the word response.
[81:30] - Oh, just the response, yeah. I was like, wait, I had to think about that one.
[81:34] But is it capital response or lowercase response? - Lowercase, it's the one that we created on line five.
[81:39] So save that. And what this'll do is it'll carry over the headers
[81:48] and the other details that were necessary there. - Yay! - And there it is.
[81:53] So now you are telling people where they're requesting the site from,
[81:58] which is kinda neat, it's a little personalization touch. But so you could now make something
[82:05] like in your index.html, you could change that to be, how's the weather in, and then have location here.
[82:14] So in your index.html there. - Yeah, I'm just, but I could also do like context.geo.land.
[82:24] Like want to know your latitude and longitude and put that in there.
[82:33] - Yeah, or you could like update a map. So I have an example if you want to see it.
[82:39] It is in here. I'm dropping it in the Twitch chat.
[82:47] So this one is an example of updating the location and then using that on a map.
[82:54] So it shows the current air quality where you are. And this is done using an edge function.
[83:01] It looks at your request, uses that to go get your latitude and longitude,
[83:07] and then updates a map and goes to the air quality index to pull the air quality for the given area
[83:15] and does that as an overlay on a Google map. So this is like one way that you can do this.
[83:20] And everybody watching, if you click this open, like for Jen, it's showing Denver,
[83:24] for me, it would show Portland, for you, it would show wherever you're at.
[83:28] And this is really relevant to me in the Pacific Northwest because during fire season,
[83:32] there are days when we just definitely don't want to go outside.
[83:34] So I can open this site up and see if it's a purple day and I need to just like hide in my basement.
[83:39] - Yeah, and that actually is really helpful because like with the fires here too and all the smog,
[83:45] but I feel like we definitely went through a lot and y'all, I just finally figured out
[83:50] how to put chapters in YouTube. And now I need to go do it, but I have figured out how.
[83:56] Okay, more of Twitter, somebody posted on there and then I learned and yeah, but I know now.
[84:03] And I know we had a few more minutes, but I'm a little mind blown.
[84:08] We have so much fun. And I feel like this actually does give me
[84:11] a really good basis to build off of to be able to build this site.
[84:15] - And oh, the last thing to do would be to just deploy that. So if you just git commit everything, push it,
[84:20] it'll all go live and then everybody who's watching can try it as well.
[84:23] - And I will do a really great job. - And so, yeah, so that, I mean, this is one of the reasons
[84:30] that I get very excited about like web dev today is that tools like this are available
[84:35] and it doesn't require you to, oh, I have an idea for an API.
[84:41] So now I need to go get like, figure out where to put a Docker image.
[84:44] And then I got to figure out what Docker is and how it works.
[84:47] And then I got to figure out how to put that up somewhere that doesn't charge me, I have a side project idea.
[84:53] I don't want that to cost me $9 a month. The thing I want to be up for fun,
[84:58] but like four side projects later and suddenly I'm spending a lot of money
[85:02] that isn't ever going to pay back because it was just for fun.
[85:06] And so this, everything that we did today on Netlify is on the free tier.
[85:11] And so you can build as many of these as you want. And unless one of them gets really, really successful,
[85:17] you're not gonna end up paying any money for it. So this is a really, really good way to experiment,
[85:23] to play, to learn, to try a bunch of stuff, to bootstrap a business,
[85:27] whatever you're doing in a way that lets you stay, you don't have to pay
[85:32] until your business starts making enough money that you have actual business requirements
[85:36] that would merit paying. And so for me, this is really exciting
[85:41] because I get to think about what I want to build, not how to get it on the internet.
[85:45] I get to try things without having to put a credit card down. I get to really, really rapidly experiment.
[85:51] If I break something, like yesterday, when I went on my stream,
[85:54] I found out that I'd broken my site and I was able to fix it and push a fix
[85:58] in the five minutes before we went live so that I only started like two minutes late.
[86:03] - Nice. - And it's this whole thing
[86:05] where I never ever could have done that when I was still running like a WordPress site
[86:11] on DigitalOcean and I'd have to like SSH into the remote server and like restart the thing.
[86:17] It just, it took forever. - Yes, yes.
[86:18] - I could never get it done. So it reduces this barrier for experimentation and learning
[86:25] that I no longer have to spend my whole half day Friday that's my learning time trying to set up the project.
[86:33] I can spend the whole half day actually building the thing that I'm interested in building.
[86:37] And I think that's, to me, that's really exciting. - I'm now starting to get like wet netlified up.
[86:43] I say starting to because there's still so much to learn, but I at least have an direction of how to play with it
[86:51] and get started. And instead of just going, Netlify is a thing.
[86:56] - Yeah, yeah. - I now know more about what the thing does.
[87:00] Yay. And thank you, Jason, for coming on the show
[87:04] for all of you that like don't know Jason. I feel like that's weird only because like,
[87:09] I feel like so many streamers or those in the dev world or in the tech world or know about Netlify.
[87:16] So that's why I say that it would surprise me, but thank you for being on the show.
[87:22] Next week, Nick will be on the show and we've had Brittany on the show.
[87:26] We've had a lot of the Netlify team, just we've all been talking about other things.
[87:30] So thank you again for talking about all of this. And any last questions for Jason before we end?
[87:37] We gotta thank you. And also Netlify has the lowest bar and clearest way
[87:45] of getting stuff going. Yes.
[87:49] - All right. - And excitement from Anthony, so.
[87:53] - Anthony, always appreciate you being around. Yeah, so if anybody wants to find me,
[87:59] I love talking about this stuff. So I'm @JLangstorf pretty much everywhere.
[88:05] I'm on Twitter, Twitch, on YouTube, I'm Learn With Jason, so you can find that there.
[88:11] Or just jason.af/links is where I've put everything. So if you want to hit that up,
[88:20] you can find all my links to all my things. And thanks for having me, this was a lot of fun.
[88:24] - Yes, and thanks. Make sure you follow both of us on Twitch
[88:29] because this is where we learn live and you get to ask all the questions and make it some fun.
[88:33] Thank you, everyone. 
