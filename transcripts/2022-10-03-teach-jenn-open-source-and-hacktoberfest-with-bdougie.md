---
showLink: "https://www.youtube.com/watch?v=5q8l5eDJyoQ"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-open-source-and-hacktoberfest-with-bdougie"
title: "Teach Jenn Open Source and Hacktoberfest with bdougie"
publishDate: "2022-10-03"
coverImage: "https://i.ytimg.com/vi/5q8l5eDJyoQ/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Thank you for joining another episode of Teach Gen Tech.
[00:07] Being very patient with an episode that I was very stoked for, and then I spilled water all over my laptop.
[00:14] It happens, and we were scheduled for today, so welcome, BDougie. I appreciate your patience as well and flexibility.
[00:22] Please introduce yourself and what we're talking about today. >> Yeah, my name is BDougie.
[00:28] Brian Douglas is my actual given name, but BDougie is what I go by on the Internet.
[00:32] Yeah, I'm going to talk about open source. I'm passionate about open source and getting people
[00:37] involved and happy to do that today with you. >> Yay. That really does.
[00:44] Hey, Ben. It is cool people. We are cool people.
[00:48] That brings up a great question, and as I've talked about in these shows before,
[00:54] but also when I've watched your streams of open source is like a thing, and I know that open-sourced is based on open-source.
[01:07] What is open-source, but what is also open-sourced? >> Yeah. Open-source, it's just that.
[01:15] It's code that the source code is viewable in public. Now, there's a couple other things that people
[01:22] put labels on top of open-source, like licenses.
[01:25] Can it be open-source without a license? Legally, yes, but also no,
[01:31] because there are some licenses, there are some assumptions that can be made unless they're not viewable.
[01:37] Just like it being open-source, you can see the code, having a license also helps that.
[01:41] Most stuff gets MIT license, which means that all responsibilities are remissed for the maintainer or creator,
[01:49] and you use it at your own risk. There are other licenses like Apache 2 or is it BDFL or something like that?
[01:56] Anyway, there's a bunch of licenses that are out there that apply to open-source and slice and dice what it is,
[02:02] but at the end of the day, it's open and viewable public source code.
[02:06] A lot of open-source is on GitHub, so it's easy to make that assumption.
[02:10] If it's on GitHub, it's public, it's open-source. But yeah, I would say use at your own risk
[02:16] is the assumption when it comes to open-source. Using your projects for work or your bootcamp or whatever.
[02:22] Open-sauce. Open-sauce is a project I built back in 2016, started a little CRM tools like a sales product,
[02:32] like Salesforce to manage your sales, I guess, pipeline. I built something for open-source to manage my open-source contributing pipeline.
[02:40] That's what I originally came out the gate with it. Two years ago, I actually built a login.
[02:47] I was the only one that could use it up until two years ago. Then we started building a community two years ago, Discord,
[02:55] folks logging and also tracking their contributions. Then we expanded into other things.
[03:00] The broader vision is empowering the best developers who work in open-source,
[03:04] is what we're aiming towards. Today, as of Saturday,
[03:07] we launched a platform to track Hacktoberfest contributions. Then we have some other stuff that we're planning on in the future.
[03:14] >> I am awkwardly staring at my other screen to grab the link to it because I didn't think
[03:20] about grabbing the link to the Discord to talk about it. I'll just go to the website and grab the website because-
[03:29] >> Yeah, that works. >> -such good content and y'all just need to go
[03:35] follow BDuggy and open-source because you are also very, very patient with asking questions and trying to figure that out.
[03:44] If for all of those that are looking to get into your Hacktoberfest, which we'll go through that in a minute,
[03:51] or new to coding, open-source is like the place to be.
[03:56] I'm not going to lie. I'm blind, this is why I wear my glasses.
[04:03] Homie Coder, you said BDuggy knows OSS, and that O didn't look like an O when I first looked at it.
[04:12] >> I'm a purveyor in lots of things, including OSS. >> Another way that I actually realized that clicked for me,
[04:24] coming from the mobile device world, I used to work at a cell phone company for
[04:30] many years when Androids and iPhones came out. I just realized a week ago that I would always explain it to
[04:37] customers as iPhone has to go through a lot of rigorous testing, to be able to go onto the App Store and be approved,
[04:46] where Android is open-sourced so anybody can contribute to it. I was like, wait,
[04:53] I used to say that like seven years ago and I had no idea. But it's the same thing.
[05:01] >> It's just a talking point, yeah. >> It's open-source software.
[05:06] When you say it, people will say open-sourced. When you type it, it's OSS.
[05:13] That confused me at the very beginning. >> Years ago, I don't know how long you've been tinkering computers.
[05:20] I guess you've sold Androids. But back in the day, open-source,
[05:24] I don't think it actually got extremely popular until the last 15 years. It has been around for a while, before my time.
[05:32] But there were things like shareware, where shareware is like, "Oh, you can have it,
[05:37] host it, anybody can use it." But there was some sort of attachment,
[05:40] like you had to pay either the license fee. Like Adobe, it's very popularized,
[05:48] the way they operate with Creative Cloud and stuff like that, how they walk down a DRM and everything.
[05:53] Open-source is like the response to that, where you had to get a cracked version of Photoshop back in the day,
[06:00] at least when I was in college. I'm outing myself, the FBI is going to find me.
[06:05] But you find the cracked version or you find license keys. What I'm getting at is open-source is kind of says,
[06:14] "You know what? Everyone can use this." It actually makes the entire industry better by just giving this away for free.
[06:20] I think of StreamYard is currently what you're using. OBS is like the underlying technology for a lot of streaming services,
[06:27] and OBS is open-source. What OBS has done is they've taken a complicated, expensive streaming
[06:34] and television software and made it free and open to anybody who wants to use it. Also, free and open to anybody who wants to build a business on top of it.
[06:42] Actually, StreamYard, but what's the other one? >> Bing? Theo? I'm like Theo and Bing, that's where I go.
[06:51] >> Yeah. Theo, he's building this whole other thing. But yeah, the fact that Theo can build on top of
[06:57] open-source protocols and streaming directly and have a business around that. It's like a testament for open-source,
[07:03] where now you don't have to start from zero in all the bits and bytes. You can start from open-source libraries to get started.
[07:09] So CSS Bing, I was talking about Tailwind before we hit live, but the fact that I don't have to think about how to structure
[07:16] my CSS and I can just build a product, just move forward. Now we can start not one from step 0,
[07:22] now we can start from step 2 or step 3. So now it's like the rising tide is raising all boats.
[07:29] So that's what open-source is really doing for everybody. So when you can find a library to do X, Y,
[07:33] or Z and not have to build it, now you can work on harder problems at that point.
[07:39] >> I dig that. Ben also brought up another one. >> StreamLabs. I kept looking at StreamYard in my browser URL.
[07:48] I wanted to say StreamLabs. StreamLabs is a business built on top of OBS directly.
[07:54] >> I know. I'm curious and this is something that we can talk about another day.
[08:00] Yet, when I think about open-source, I think about more complicated,
[08:05] meaning that for somebody that's new to it, it may not be as easy to use.
[08:10] I'm comparing OBS to StreamYard. StreamYard is very quick and easy to go.
[08:17] Multiple people have been like, "Jen, use OBS." Then I'm like, "I don't want to learn that too."
[08:24] That really does lead into Hacktoberfest, because there are good first issues that you don't have to
[08:33] worry about the high-level complications of it. But can you explain as a maintainer,
[08:42] and y'all, a maintainer is, and please BW, please let me know if I'm explaining this right,
[08:48] is where you have an open-source project and a maintainer is someone that owns the open-source project?
[08:58] >> Technically, and this is all depending on the license. So Python, instead of BDSL, whatever it is,
[09:07] it's like the Benevolent Dictator, which Guido Rossin, the creator of Python,
[09:14] created this. I don't know if he created it, but the way it is, he gets to say
[09:18] what the roadmap is going. So yeah, he owns the roadmap for Python.
[09:22] I think Guido actually might have stepped down. Someone else, keep me honest.
[09:25] But what I'm getting at is, own the product. If it's MIT licensed,
[09:30] then technically you don't own it. You're using it, you're directing it.
[09:35] As a maintainer, you have access to publish and cover releases. But at the end of the day, if someone can clone that repo
[09:42] and go run off and do something else they want to do with it. It's like hotopensauce.pizza,
[09:47] which is our discovery engine for finding projects. That's MIT licensed.
[09:51] So if someone wants to take anything that we've built and say, "You know what? I'm going to make it better.
[09:56] I'm going to take all their code and produce a better version." They can do that based on the MIT license.
[10:02] So yeah, technically, code owners. >> That's scary.
[10:07] >> Yeah, it's scary, but it's also the thing, it's almost like,
[10:12] I don't want to say it's like plain chicken or something like that, where you roll the dice and you say,
[10:16] "Yeah, if you can do better, take it, steal it, do whatever you want."
[10:19] But at the end of the day, the movement we're seeing right now is stable diffusion and open AI,
[10:24] where they're pushing forward machine learning and what you could do, and generating art, audio, video.
[10:32] That would not have happened if open AI didn't open source all their stuff. Because now everyone's starting from like,
[10:39] "Okay, they solved a bunch of stuff for us. We're going to start here. Now we're good."
[10:42] You see it in the blockchain too as well. Once people started sharing the blockchain and the Ethereum,
[10:48] like the Web 2 or whatever it is. Sorry, Web 3. I don't know why I said Web 2.
[10:53] Web 3 stuff, some people would have come at me in the comments. What I'm getting at is, you don't have to start
[11:00] from zero and create your own blockchain from scratch. There are services and tools and open source projects where you could start.
[11:05] So no one owns it unless it's explicitly said. Usually, if it's like a Facebook,
[11:11] they had a lot of pushback years ago with React. Because React, in their licenses said that you could never sue
[11:17] Facebook for if you use React, like you can't. Yeah. But it was pretty expansive that it sounded like if you use React,
[11:26] you can't sue Facebook for anything. So Facebook was coerced and forced to change
[11:32] their license to be more explicit to can't sue them for React problems. Interesting. That is like a whole rabbit hole we can go down with licensing.
[11:44] I think that would actually be really great. Put that on my to-do list of videos to create.
[11:50] Now, with Hacktoberfest, and Hacktoberfest started two days ago,
[11:59] and how would you explain Hacktoberfest and what do you look for as a maintainer? Yeah. So Hacktoberfest, it's a month-long hackathon.
[12:12] It's like the biggest open-source hackathon in the world on the Internet. The focus is for mainly first-time early contributors,
[12:21] early devs to make contributions to open source. So that's the encouragement, that's the focus.
[12:27] Now, everyone's got their own story around Hacktoberfest, whether it's good or bad for them.
[12:31] But for Hacktoberfest, what they did a couple of years ago is they opted in.
[12:34] So your repo needs to opt in to be part of Hacktoberfest. If somebody creates four,
[12:40] I think it's four PRs in the month of October to an opted-in repo that's been accepted. So please don't do spam,
[12:47] but try to do quality contributions. Then you get a T-shirt or you get a choice to plant a tree.
[12:52] So that is Hacktoberfest as a whole. It's really just around encouraging people to be aware and to do open source.
[12:59] I forgot your second question. Oh, what are maintainers looking for?
[13:04] >> Yeah. I would say specifically you because you have open-sourced and that is quite the project and how do people find the projects,
[13:16] get involved, and what do you look for for somebody to submit a PR to get approved? >> Yeah.
[13:23] >> Complicated question, complicated. >> It is complicated, but luckily,
[13:27] we have a lot of automation and tooling to coerce people to do it the right way.
[13:30] So what I'm personally looking for, hands down, look at the growth of the community.
[13:35] We're not really looking for heavy-hitting features or we do take some low-hanging fruit contributions, which is totally fine.
[13:43] But at the end of the day, if you're going to come contribute open-sourced, the hope is that you come join our Discord,
[13:48] you come find out more about the project, and it's not just a one-off,
[13:52] you're just trying to get the T-shirt. I think as a whole, Hacked Over Fest should be approached that way,
[13:56] where I don't care how low-hanging fruit or the typo that you change or you fixed in my repository.
[14:04] But if you're interested in coming along for the ride and hanging out with us and having conversation about what we're building,
[14:09] that's what I'm looking for, to be honest. So we have a lot of automation and tooling.
[14:13] So all Hacked Over Fest contributions in my projects require an issue attached to it. The reason for that is a lot of some unsolicited stuff comes all the time,
[14:24] as much as I want to convert everything into TypeScript, which we already did that last year, to be honest.
[14:28] But there's some other TypeScript conversions, I think back in 2018 with the popular,
[14:33] like people would just try to convert one file to TypeScript, which doesn't work. But anyway, what I'm getting at is I'll take your ideas.
[14:41] I'd like the respect of you opening up an issue first, and us having a discussion on whether this is needed in the project.
[14:48] And I think overall, most maintainers would like that as well. So open up the issue, be diligent about what you're actually proposing
[14:56] and what is actually a bug, and then wait for a response. We tend to automate the process of how you can assign yourself to issues,
[15:04] but also automate the process for releasing through GitHub Actions to make it easier for people not to have to understand
[15:09] how to do every single piece of open source contributing, which we can talk through in a moment.
[15:16] Yeah, so for that reason, we try to keep it easy and approachable. Because at the end of the day, like, oh, we had,
[15:23] some of my contributors actually had been around for a while, came through Hacktoberfest, and have stayed consistent with us,
[15:27] and like, will participate in conversation about the future of what we're trying to build.
[15:33] That brings up a question for myself of, so in many streams, I've talked about Anthony,
[15:40] and he's like my big brother, he's AJC web dev, because he's really, like, hard on me to get stuff done and figure it out,
[15:49] yet one of my biggest supporters, which I so appreciate him, yet he said that he actually got into a lot of this stuff
[15:56] because he found open source. And I'm curious, like, did that happen through Hacktoberfest,
[16:04] or like, how do people find first good issues? Like, how do you get involved?
[16:10] Yeah. Yeah, so like, Anthony's an interesting story, because we actually met on a podcast first.
[16:15] He had reached out to be on my podcast to talk about Redwood. And I was like, oh, cool, I haven't had a conversation about Redwood.
[16:21] We had the conversation, I think I followed up with like, hey, we'd love to stay connected, join our Discord.
[16:28] We happened to be joined, like, creating a Discord around that time, or maybe it was like a couple months old.
[16:33] So he joined, and as our Discord was growing, he was a part of it, and started this sort of coercing him, asking him questions, getting feedback.
[16:42] And he hasn't been like a huge, like, code contributor. But as far as like a awareness contributor, conversation starter,
[16:50] like, he's like, very excitable. And I think he's in quite a few different Discords, I highly recommend.
[16:55] So like, for finding good first issues, repos, like, we've been trying to solve that problem with open source.
[17:01] So originally, I created the tool, which is app.opensource.pizza. Like, that's the original tool.
[17:07] I created that about five years ago, 2016. Six and a half years ago, I don't know, time's off.
[17:14] But what I'm getting at is, like, I created that for myself. It was really for me to track repos, and that's what it did.
[17:20] And then up in the upper right, I don't know if you can share this on your screen,
[17:24] but I had the idea to like, recommend good first repos for people to contribute to. So the, yeah, if you, oh, this is a hot repo, yeah.
[17:36] Yeah, so if you go to opensource.pizza, the actual URL. - Move this, we're just, there we go.
[17:47] - Yeah, and you put the word app in front of it, app.opensource.pizza. We, I just recently took this down.
[17:54] Sorry, I took it off the main page, mainly because we're focusing on some other things.
[18:00] So I want to recreate these features in our new product. But it just got to the point where I just,
[18:05] we couldn't keep up with the legacy stuff. So here you basically, there's an onboarding
[18:10] to essentially get to the point where you can have a dashboard. And in that dashboard. - Oh, cool.
[18:15] - In that dashboard, so like, this is what I built originally. So if you click sync repos,
[18:20] this will actually authenticate you to GitHub. Hopefully, hopefully it's not broken.
[18:26] This is the, I haven't gotten to the onboarding myself in quite some time.
[18:34] - I'm guessing it's synced. Create a database.
[18:36] - Oh yeah, if you've logged into GitHub, I guess it will work.
[18:39] Yeah, so create a DB, which then create the repo for you. It'll take you to GitHub, then tell you,
[18:44] hey, this is what we're going to do. My recommendation is to select repositories.
[18:51] So you want to install this on everything. You just want to install it on this repo
[18:54] called opensauce.goals, or opensauced, open-sauced goals, yeah.
[19:03] So it's that second one right there. So what you did was syncing repos,
[19:07] and we created a repo for you. So your entire database is a GitHub repo.
[19:12] And I did that because I didn't want to pay for a database tool,
[19:16] 'cause I didn't have that much money when I created this thing.
[19:18] So if you click accept, I think, or whatever that green button is, install.
[19:22] Excellent. Now it's installed, and this is a GitHub app.
[19:30] So GitHub apps are like integrations you can build inside of GitHub
[19:33] to do cool things on people's repos. What we've done is we created a repo for you,
[19:38] and we installed it on that repo. So if you go back to the tab with opensauce,
[19:42] it should advance you to the next section. Yep, there you go.
[19:45] And then it gives you an option to select repos that you want to add to your list.
[19:50] So if you click on the first one, I think that's the way that works.
[19:55] Oop. Oh, okay. - Oh, yeah.
[20:00] Okay, got it. Yeah, yeah, yeah.
[20:02] - Sorry, that UI is maybe not as intuitive, 'cause I forgot how it works.
[20:06] - That's okay. We figured it out, and we will add.
[20:11] - Yeah, so the way this works is, yeah, so the way this works is you add any repo you want.
[20:19] So if you wanted to add Tailwind or Gatsby or Next.js, you can add it in that list,
[20:25] and then you start tracking the repos. So if you click on the list there,
[20:30] yeah, I guess if you click on open source in the list, it'll take you to the page that will then tell you
[20:35] more of like good first issues. It'll give you insights on, well, not much insights here.
[20:40] Anyway, I don't know why we're in this rabbit hole. Basically, this is the old product.
[20:46] We're moving away from this, but as I was building this,
[20:48] I wanted to create a recommendation engine to recommend projects for you to click on.
[20:53] So we hard-code three repos for you to choose from. But the goal really is we want to discover
[20:59] where open source is happening, which is why we created HotOpenSauce.pizza.
[21:03] So HotOpenSauce was just gonna be a feature on this platform, and it turned to its own app, essentially,
[21:10] because as we were building it, it was like, oh, this is cool, we should do this, we should do that.
[21:15] And this didn't make sense to inject it here. It also gave us an opportunity to create a new application,
[21:21] which is a React app built on Vite. That is now, all of our open source happens
[21:28] around HotOpenSauce.pizza at the moment. - Few questions.
[21:33] So, first off, I do need to say this. On the Discord, there are pizza pics that you can post,
[21:41] and I just remembered that I took pictures of pizza to post there, and I forgot to,
[21:46] so I'm gonna have to post some pictures of pizza. Also, so, and I think this would matter
[21:54] to each open-sourced projects and for who it is, but what languages do people need to know
[22:06] to be able to contribute to open-sourced? - Yeah, that's a good question.
[22:10] Yeah, so at the moment, we are primarily JavaScript. Also, TypeScript is the other language.
[22:19] Yeah, so the majority of the stuff we're doing right now is TypeScript, so we kind of like moved,
[22:23] we've moved into the TypeScript land. I think it's like a pretty popular move at the moment
[22:31] for most folks, but yeah, JavaScript's a 100% necessity to contribute to open-source in particular.
[22:38] - I can, A, this keyboard does not work, and it double-clicks everything.
[22:44] - I'm gonna move the TypeScript. I can type script.
[22:53] I'm posting the video that we did with Josh last week on Josh Goldberg on foundations of TypeScript,
[23:03] and he's actually gonna be a regular on the show of working through his book,
[23:08] so definitely something cool that I think would really help anyone trying to learn TypeScript
[23:14] because it is really cool and can be really complicated to learn at the same time.
[23:21] So all right, we've got here, this is like the old area, and now if we wanted to go,
[23:30] they would go to here to find out more on their GitHub. - Yeah, so-- - If we just go here.
[23:40] - What in particular are they looking to find out, finding projects in particular?
[23:43] - For Good First Issues? - Yeah, so we do have Good First Issues.
[23:47] We don't have a sort of centralized database for all Good First Issues, and mainly because,
[23:53] so we can talk about our Good First Issues specifically for open-source,
[23:58] but also there are some other cool tools like goodfirstissues.dev.
[24:02] There's also a Twitter account, which is @goodfirstissuesbot
[24:06] if you're looking to source issues or make contributions in random places.
[24:11] Also gonna shout out our Discord has a Good First Issue channel as well,
[24:15] which is, I believe it's still called Ketchup. - All right, I am slowly getting these linked in
[24:25] to our chat. So Good First Issues.
[24:30] - We do have a Good First Issue channel. It used to be called Ketchup,
[24:34] now it's called Good First Issues, 'cause it was, I guess Ketchup was too,
[24:38] the open-sauce thing was too much on brand, I guess. - (laughs) All right.
[24:46] Oh, I don't know about ketchup on pizza, but I don't know if I could do that.
[24:55] I don't know if I could do that. - You know, I would say that I wouldn't recommend it,
[25:00] but also those like Lunchable pizzas sometimes can hit pretty well.
[25:04] So, which is basically like putting ketchup, mozzarella sauce, or marinara.
[25:10] I said mozzarella sauce, that doesn't make sense. - It is technically tomato sauce, but it's not the same.
[25:19] It's not the same. - Yes. I think ketchup has sugar and vinegar is the difference.
[25:25] - Okay, okay, that makes sense. And we got the Discord linked.
[25:32] That's this lovely one right here for the actual Good First Issues,
[25:39] and then .dev and the Twitter account. So those are all linked now.
[25:45] And where we started was, if I go back, ta-da, Good First Issues that we have right now.
[25:56] Goodness gracious, I can talk. - Yeah, so we can talk through the Good First Issues.
[26:03] And actually philosophy-wise, like I'd love to mention the way I approach
[26:07] Good First Issues, which is why we don't have so many, is that every Good First Issue
[26:11] should have an answer inside the issue. I don't think they should be tongue twisters.
[26:15] I don't think they should be challenging things to accomplish.
[26:19] And the reason for that is Good First Issues exists to bring more people into the community.
[26:24] So it's like something that you could do yourself as a maintainer or something,
[26:28] it would take you 10 minutes to do. Realistically, for someone new to the project,
[26:32] it should only take them a couple hours to approach and complete,
[26:37] or else you haven't scoped it properly. So you gotta break down the issue in the smaller chunks
[26:42] or approachable problems. And then if it's longer than that,
[26:46] it probably isn't a Good First Issue. So that's the philosophy I sort of stand on.
[26:51] So for that reason, we don't have a lot of Good First Issues 'cause when I do put the time in to put a bunch of issues up
[26:57] that have answers in them, they end up getting taken. So we can really quickly talk through
[27:02] what the first one is, which I just assigned the Janie this morning.
[27:07] This is, as it says, rename everything from post to repo. So we started the HotOpenSauce.repo project,
[27:14] or HotOpenSauce.pizza project. And I didn't actually write up the files,
[27:19] but someone put, like, name everything post. One of the contributors named everything post.
[27:24] But what we're actually submitting are repos. So I just found that it kind of annoying to,
[27:30] not annoyed by the contributor, but annoyed that every time we look up something,
[27:33] I'm like, oh, it's a post, it's a post, it's a post. Can we rename these to repos?
[27:37] So the actual ask is take the files that are called PostGrid.js or PostWrap.js
[27:44] and make it RepoWrap instead. So for whatever reason, this one's been,
[27:49] it's basically been open since last month. No one's picked it up.
[27:53] And I'm not sure if it was too confusing or it was too easy.
[27:58] But so I just asked somebody this morning that, actually, honestly, we were gonna do this one on Friday,
[28:03] but I was like, oh, I was talking to a contributor and was like, oh, I got an easy one for you.
[28:07] Here you go. So I just assigned this to Janie,
[28:10] who's gonna handle that one. But I do have another issue that we can work on today.
[28:13] But I just wanted to call out that it's just as simple as that in our project.
[28:17] We wanna make sure it's approachable. There's like a CSS fix or there's like a word change.
[28:23] Like, that's most of our good first issues are things to, 'cause what usually happens
[28:27] is once you do that easy thing, the hard part is always getting it up into a PR
[28:31] and then understanding how to keep your branch up to date and doing all the other stuff after the fact.
[28:36] That's when it gets interesting. And it's not that hard,
[28:39] but you just have to open up a PR to learn it. So the goal for Janie, as I was talking to her,
[28:46] is I want her to learn how our process works. So like, here's an easy issue.
[28:49] Now you'll learn how the actions run and how this works and how that works
[28:52] and how we cut releases. But we do have someone who did actually respond,
[28:57] say, hey, can I take the issue? And this during Hacktoberfest,
[29:00] it's a constant problem of like everyone asking if this is still available, is it still available?
[29:05] And my ask is, yes, it's available if no one's assigned to it.
[29:11] And the way to assign yourself to it, as I comment right here,
[29:16] there's a link there on ContributingMD that tells you how to assign yourself to the issue.
[29:21] And the reason for that is I want people to walk into the ContributingMD and read it,
[29:27] 'cause that's the other challenge. So the good first issue, again, it's not about the code,
[29:30] it's not about the problem at hand, it's just about learning how to contribute to our project.
[29:34] So here's a doc site and it has triage. Actually, there is, there should be a link about,
[29:40] oh, there you go, first line, .take. So if you type in .take into the issue,
[29:46] it will assign you to the issue. - Okay.
[29:49] - And the reason for that is like you can't assign yourself unless you're an org member into a project.
[29:56] So it becomes like a sort of a hurdle for anybody who wants to contribute,
[29:59] you have to be a member of the org to assign, or you have to ask me.
[30:02] And the challenge is that if you have to wait for me, then it's just gonna be slow.
[30:08] Like, 'cause I'm gonna have to like go through all this. So I've created a get of action that basically,
[30:13] if you write that word, the action will assign you on my behalf.
[30:16] - So, and we do have a comment real quick. Yes, agree on the good first issue point.
[30:25] That's a really good way to get people set up the repo. Wow, locally, when you know that effort won't be wasted,
[30:35] you're way more likely to do other stuff later instead of even set up a repo to start with, agreed.
[30:42] And Mo, just to give you a heads up, we are actually talking about Hacktoberfest
[30:50] and how to find good first issues because since people aren't,
[30:55] a lot of people in Hacktoberfest is made for those who are new to coding,
[31:00] is we're going through how in open source that we contribute to a first issue.
[31:04] So that way you get points to Hacktoberfest. And that being said,
[31:10] I do wanna take a step back really quick. How do I know that this would be good for Hacktoberfest
[31:19] or approved for Hacktoberfest? - Yeah, so if you click on the, go to the,
[31:24] I guess the readme, the landing page of the repo itself. And up in the right hand corner,
[31:32] most, now it's not required, but if you wanna opt in to Hacktoberfest,
[31:37] it needs to have the topic Hacktoberfest in the repo. And that makes it easier for every,
[31:42] the node it's been opted in. Now there are maintainers that will not put that topic there
[31:47] but will accept Hacktoberfest PRs. So the other half of it is just asking the maintainer
[31:53] if they can add the Hacktoberfest accepted label, and then that will also get accepted.
[31:58] 'Cause some maintainers don't want all the contributions to be associated to Hacktoberfest,
[32:01] but if there's someone already contributing, and there's like a good first issue they sort of captured,
[32:07] they can then go ahead and ask the maintainer to add the label,
[32:12] and then it'll get accepted into the Hacktoberfest system. - Sweet, and I clicked the label and this came up,
[32:19] which it looks like a place to start. So I'm gonna go back
[32:25] because I love the community that you've built. So that way it's easier for us to know what to do with it
[32:32] instead of just like all general. Because I know for my first issue,
[32:38] I definitely... Is my first issues.
[32:45] Now I have to go back. Okay, fine.
[32:49] - Back, back. - Yeah, if you also go to any repo, do /contribute.
[32:55] So right now it's open/hot in your URL. Take out everything after hot and then type in contribute.
[33:04] This is a quick sort of Easter egg to get to just good first issues.
[33:11] Good first issues and docs. So it's the same filtered list,
[33:17] but there you go. - Right, private repos, I wouldn't think so.
[33:28] Private repos are not a part of Hacktoberfest. - Yeah, Hacktoberfest is focused on open source.
[33:34] And by default, if your project is private, it's not open source.
[33:40] So it negates even the reason for having a contribution submitted.
[33:45] Also, if it's private, it probably doesn't want people alerting
[33:48] what their contributions are in the code. - That is true, that is true.
[33:52] And what up, Anthony? We were talking about you earlier and you weren't here.
[33:57] All right, so we talked about... So I'm gonna go to the feature Tailwinds and...
[34:05] - Yeah, so this is the issue that we had where we had a contribution, quite a few contributions,
[34:11] and we found that we were introducing anti-patterns. Tailwind is a framework to build CSS.
[34:17] And when you use the framework, it is beautiful. When you start writing...
[34:23] Anytime you have a framework and you start writing code that doesn't belong,
[34:27] or you start writing your own libraries on top of the framework,
[34:30] it becomes a maintenance nightmare. So someone called it out.
[34:33] So we ended up going through all the files and identifying where we need to clean up the actual CSS.
[34:39] The example that I have here is the class name. Anywhere where it's hard-coded pixels,
[34:43] we wanna change it into the Tailwinds, like the number framework, basically,
[34:50] which just attaches a rim that's... Anyway, we don't have to get into details about Tailwinds,
[34:54] but basically it's just consistent across multiple browsers and browsers like window sizes and stuff like that.
[35:01] So it's better to use the second pattern than to use hard-coded pixels.
[35:04] So it seems like we only have one issue open that needs to be addressed.
[35:09] So if you wanna click on that one, you can actually, in GitHub, you can link issues
[35:13] inside of issues. So what we had previously was a tracking issue,
[35:19] and then the tracking issue has the last one that's ready to get accomplished.
[35:23] - So on that note, would I want to take both of them, or would I just take the one within the one?
[35:32] - Take the one within the one. Yeah, 'cause so the tracking issue is really set up so,
[35:36] and multiple people can work on the same problem, just in different places.
[35:41] One person could take all of them, but if someone takes like six issues,
[35:45] I usually unassign them, because you're being a ball hog, basically.
[35:50] Like we wanna share the wealth. Like this is not really meant for you to,
[35:54] and a lot of times some people can get in their head of like, oh, good first issue, I'm gonna grab another one.
[35:58] But the thing is like, if you've grabbed the good first issue already,
[36:03] after a couple of them, they're not good first issues anymore.
[36:06] It's just basically you're cherry picking some easy stuff to do.
[36:10] So my ask is like, hey, why don't we go try another problem or a harder problem?
[36:14] 'Cause at this point, you already know how the repo works. You know how to clone it.
[36:17] You know how to do PRs. You know how to interact with us,
[36:19] us as in the contributors to open source. So let's move on to like something a little more challenging.
[36:25] - I dig that. And so like they did their take on it.
[36:31] It looks like it was, let's see. - Yeah, so- - They disappeared.
[36:39] - Yeah, so Alex basically, he got a little busy. He had some family stuff come up.
[36:44] He also, it failed in review. So there were some things that we had to get updated.
[36:50] But Alex currently, I don't know if he's gotten his first job yet already,
[36:53] but he was either on the hunt for work. So I'm gonna assume he got busy.
[36:58] So I went ahead and unassigned him. But if you write .take,
[37:02] I do wanna do some automation, which if somebody wants to build this for me,
[37:08] I need some automation to basically go through anything that gets stale after being assigned
[37:12] and go ahead and unassign people. 'Cause we do get a lot of folks
[37:15] who assign themselves issues and they just, you get busy.
[37:18] - I think I've done one. I've done one of them.
[37:21] I assigned myself, I think like two months ago and forgot. - Yeah, and it happens.
[37:27] And like, we wanna be respectful. Like, hey, I understand like, you know, family comes up.
[37:32] It is all like free time you're giving to the project. So my assumption is like, there's no deadline.
[37:38] Just like within a month, probably at that point might wanna unassign them
[37:43] because then we're gonna have someone else take it. So you initiated the .take.
[37:48] We should, we just got to see you're assigned. We saw the action below go live.
[37:53] - Yep, okay, so we gotta wait for, ah, okay. - Yeah, so this GitHub action,
[37:59] and we can actually talk about the action if you want and then jump on the clone.
[38:02] - Yeah, for sure. But the action itself, it just assigns you to the issue
[38:06] on behalf of me. So that's what's happening to GitHub action spot does that.
[38:10] We also alert you that we have a Discord. So the hope is that you go in the Discord and ask questions.
[38:16] So that's like our sort of pipeline. Like, I talked to a lot of maintainers when I worked there.
[38:20] I used to work at GitHub. I don't think I actually mentioned that.
[38:22] Spent four and a half years working at GitHub. Talked to a lot of open source maintainers and contributors.
[38:28] And a lot of folks wanna know, like, how do you get your projects like noticed?
[38:31] Or how do you get contributors? And it's by doing things like this.
[38:34] Like if someone has a good experience, they're gonna talk about it.
[38:37] So all you had to do is type .take, you assign the issue. Now you're an open source contributor.
[38:43] Like your name is somewhere in someone else's project. To make that process as easy as possible
[38:49] is how you grow community and how you grow interest. And not everyone's built for community management.
[38:55] Not everyone's built to be sort of an open source maintainer but we all grow into it essentially.
[39:01] So like as long as we like do the smallest baby steps, if you care to do them,
[39:06] you'll see growth in your community. You'll see attention and traction.
[39:09] And that's, at the end of the day, that's how it all works. Like all the larger projects got some sort of backing
[39:14] behind good community managers or good folks who know how to engage community and stuff like that.
[39:19] And that's how they get traction. It wasn't, like no one's gonna find your project
[39:23] organically, just magically, just by searching on GitHub. You kind of have to talk about your project
[39:29] and you have to also make sure when people will show up like they can help out
[39:33] or they can at least use a thing too as well. - That brings up,
[39:37] I'm gonna actually move my Discord over here because one thing that has always like,
[39:45] that I get stuck on and I don't know if anybody else does this,
[39:49] but it's the fact that I'm like, oh, I got a good first issue, I'm ready.
[39:54] I don't know where to ask questions 'cause I'm like, does it go here?
[39:58] Does it go here? Does it go here?
[40:01] And then in turn, I DM Ben and ask him, how do I do this?
[40:06] Because I really wanna do it, but I don't wanna make an ass out of myself.
[40:10] So how do I do this? Or Anthony, like instead of doing it in the community
[40:15] where others can learn with it, because I'm like, I don't know.
[40:18] So good first issues is where an issue is posted and you can go like assign yourself.
[40:27] But then I'm looking at them too. Where would I put it?
[40:37] No. - As far as the question.
[40:40] So I would start, it says a section called start here.
[40:45] And this, it should have explanation on where, I don't think we actually have explanation
[40:52] on where to actually have open source, open source questions,
[40:55] which is a good, it's actually a good catch too as well.
[41:00] If we don't, I'm actually reading it right now. Okay.
[41:06] I'm gonna type this in here because it should be here. Here we go.
[41:16] Now, everyone who comes here after now will know that's where I ask open source questions,
[41:22] which would be that. - Yeah, this channel is just for everyone to,
[41:28] so Takanomi, he's had a couple of contributions. If you have specific questions on the approach
[41:33] or if you need reviews, or if you had a review requested,
[41:37] or so you had changes requested and it's ready for review, this is the place to go to.
[41:41] So yeah, this channel is in particular, specifically for, I wanna contribute to open source
[41:49] or I'm a contributor to open source, this is where we hang out.
[41:53] Everyone who's just here for just having conversation or hanging out, we have a hanging out channel.
[41:59] We have a free stuff channel. We have the pizza pigs channel, jobs channel.
[42:02] So like all that stuff is for those specific reasons, but if you specifically want questions answered,
[42:10] like that's the place. - Sweet, thank you for that because I was,
[42:14] I mean, any community that I join, I'm really, really bad at commenting or being a part of them
[42:20] because I'm like, I'm overwhelmed. There's so many options.
[42:24] So thank you for adding that in there. And all right, so we, the GitHub action,
[42:31] thank you for explaining that, assigned me to the issue.
[42:37] And now I need to go to context is on the tracking issue here.
[42:47] Okay. - Hold on. So you're good here.
[42:50] - Okay. - What we're doing is basically there's a one file called the hero TSX.
[42:54] That file has the anti-pattern in it, and we just have to replace the anti-pattern.
[42:59] So we could do, we do a couple of different things. I don't know, do you have code spaces enabled?
[43:05] And that might actually be easiest to do that in the browser. - Make that, yeah.
[43:10] - I'll show you how you can check. So if you go to the file itself,
[43:15] if you hit the word, the letter T on your keyboard. - Okay.
[43:21] - Oh, you know what? You actually have to be the main, sorry.
[43:24] Go to the landing page, the code, code tab. There we go.
[43:32] Now hit T. - T. - And then type of the word hero.
[43:36] So click that first one. And then if we scroll down,
[43:46] we should see like square brackets and pixels. Literally throughout the entire code base.
[43:51] It should be at the bottom where the JSX starts. Oh yeah, line 144.
[44:01] So if you scroll over, so see that dash X dash? So all that like five PX, we have to replace all that.
[44:09] - And like this one, that's 130, okay. - Yeah, so it's just littered throughout the entire section.
[44:16] So the way, you know, actually we can't do it. We'd actually have to clone this locally
[44:22] 'cause we have to run a server to see this work. So a couple of things, we're gonna,
[44:28] do you have Git already installed on this machine? - Solid question.
[44:38] I say that because this is not my computer. - Yeah, so you have VS Code.
[44:42] So we'll probably, we can do this in VS Code. - Okay.
[44:46] - So that will get you out of the way there. The, I will struggle with the,
[44:51] getting the CLI to work in Windows, but if you go to cli.github.com,
[44:55] we'll do it, we'll basically approach just the easiest way possible.
[44:59] And honestly, I think using the GitHub CLI to make your first good first issue contributions
[45:04] is probably the good way to start 'cause it does a lot of the forking and dancing for you,
[45:10] which I'll explain what I mean by that. So yeah, good news is that there's a executable
[45:16] for the Windows. It looks like you have a, now an installer to install.
[45:22] So yeah, the GitHub CLI, it's a tool built by GitHub to interact with GitHub.
[45:28] So most people are familiar with the Git command line interface, where you can like Git add
[45:32] or Git commit or Git push. The GitHub CLI basically adds more interactions.
[45:38] So you type in like gh-clone or gh-fetch, like you can grab data from GitHub directly.
[45:45] Okay, okay, I am staring at it on my other screen, waiting for it.
[45:52] Oh, yes, yes, I do. There we go, finish.
[45:57] Okay, and it's installed. So I just wanna see if there's something
[46:09] we need to do for-- - Yeah, you shouldn't have to.
[46:13] - Yeah, if you just do gh-auth-login, you might have to open a new terminal.
[46:18] I'm not sure how it works on Windows, but yeah. - This keyboard is going to--
[46:26] - Yeah, so you have to close the command prompt and open it up again, 'cause I think the way it,
[46:34] it should load everything that's been installed. Me, I'm like trying to use a Windows computer is difficult.
[46:46] Okay, gh, what was it again, gh-- - Auth, A-U-T-H.
[46:54] Oh, you gotta log in after. Yeah, so this is basically taking,
[47:03] connecting you to GitHub from your command line. So gh-auth-login.
[47:09] (keyboard clicking) Cool, github.com is the one you want.
[47:15] Just hit Enter, and you wanna click SSH as well. And there's a reason for that, and you wanna say yes.
[47:23] You don't have to put anything here. Just hit Enter, and hit Enter again,
[47:32] and I'll explain to you what you're doing too as well. So log in with a web browser.
[47:35] So basically, normally to set up SSH is a little more complicated than we could do on stream,
[47:41] 'cause I'll mess you up, and you'll mess it up. But with the GitHub CLI, it will actually give you access
[47:47] to your GitHub account directly through your command prompt. So when you clone, you don't have to type in your password,
[47:52] 'cause now you're basically saying this, I trust this, hopefully you trust the machine you're on,
[47:57] but you're basically telling GitHub, I trust this machine enough that I'm gonna add a SSH key,
[48:01] which is a secure shell protocol, to basically go back and forth between GitHub.com
[48:07] and your Windows computer. - And I'm creating a new one, maybe.
[48:18] - Creating a new one? - SSH key, 'cause I don't currently have any.
[48:22] - Oh, yeah. Well, you should be able to do it from the command line.
[48:28] - Oh, okay. - Yeah, so the CLI will do it all for you.
[48:31] - So on this-- - So just hit Login with Browser.
[48:35] Just hit Enter. - Okay.
[48:40] - Are you focused on the command prompt? I don't know if it's a...
[48:48] - Let's see. - There you go.
[49:01] - So that number, you should be able to paste in the browser that opens up.
[49:05] - Oh, okay. - Yeah, so normally you would manually create a SSH key,
[49:11] you would copy and paste that, throw it into your root folder,
[49:15] hope for the best, and then it works. A lot of times it takes a couple tries.
[49:20] It's really challenging for beginners, so I always point people to the CLI to do this for you,
[49:25] so that way you don't have to worry about how we used to do it in the old days.
[49:31] - Cool, so now what it's done is basically it's created a SSH key, it's put it into your root.
[49:37] It also logged in tgentech, which I assume is your GitHub. - Yeah, it's not supposed to be, but yeah, yeah.
[49:47] That's it, that is it. - Well, we'll roll with this one.
[49:51] - Yeah, okay, there we go. All right, so we are logged in.
[49:58] - Yeah, if you wanted to change it, we could've reset it if you wanted to log into your other account.
[50:03] - No, I don't have access. I'm currently waiting for GitHub to get back to me
[50:07] because it was associated with an old work email, and I didn't realize to change the email address
[50:15] before I was let go, so I'm asking them for access, being like, "Please, can I please have my username back?
[50:22] "That's all I want. "I don't want the content.
[50:24] "I just want the username, please." But we'll see.
[50:28] All right, so I am in here now, so I can... - Yeah, so here's the nice little,
[50:38] because now you have everything connected to GitHub. You're now, you're a wizard, Harry, basically.
[50:44] Sorry, bad joke, it's out of date. If you go back to your homepage for the hot repo,
[50:50] we wanna clone it. You're a wizard.
[50:54] You wanna clone the repo by just going to the Code tab. - Okay, let me make this bit bigger again.
[51:01] All right, you said Code tab? - Yeah, yeah, 'cause we wanna get the green button
[51:07] on the right that says Code. - Oh, so I need to do this entire thing, and...
[51:16] - Well, the beauty is that you can click on the CLI and then copy that, and then that should clone it locally.
[51:23] The good part about doing it this way for folks listening at home
[51:26] is that it also sets up your remote. So you could also, oh, you know what?
[51:31] To be honest, we should fork it first. - Ah!
[51:36] - Oh, and we have to install Git for Windows as well. - Okay, well, we're just gonna close that for now,
[51:44] and Git for Windows. - This is, you know, honestly,
[51:54] I did set up my Windows machine to code on. I've never coded on it, but for times like this,
[52:04] I have it set up in case I have to use the Windows machine. - Well, now it'll be set up so that way,
[52:11] if I do ever need it, again, it'll be already set up on this laptop.
[52:19] - I am very, very fortunate that Tyler is letting me use his Windows laptop.
[52:25] But I did find out that I have AppleCare, and so it was only a $300 replacement
[52:32] instead of like a new, completely new computer. So-- - That works.
[52:41] - There is good news in that. There is good news in that.
[52:44] All right. Install.
[52:50] So many install options. Okay, and then.
[52:54] I have too many tabs now. This isn't good.
[53:01] I always hate too many tabs. Exit, exit, exit, exit.
[53:06] Yeah, okay. - Yeah, so we do wanna fork this repo,
[53:11] 'cause I realized we're gonna clone the upstream, so that would have been challenging
[53:14] to contribute back up to that. So up on the right, we have a fork button.
[53:19] So when doing open source, open source really starts from getting a copy
[53:23] of the version, so you could work on. So by clicking that fork button,
[53:27] that's how we get started with that. - So just click fork.
[53:32] - Yeah. Yep, you know, everything should be good.
[53:36] You just go ahead and create fork. This is a new screen.
[53:39] Back in my day, we used to just get the fork, and that was it.
[53:44] Oh, they took out the copying machine? There's a nice little animation
[53:47] where they were copying the code base on a copy machine. I guess they took that out.
[53:52] Sad days at GitHub. Cool, so now we have the fork.
[53:57] We wanna go ahead and clone using the CLI, so go back to the green button.
[54:01] We also might have to open a new command prompt tab, because git might not be recognized,
[54:08] and I'm not sure how to do this. And you might, well, I'm not sure if this is bash or not.
[54:13] I'm not even sure why you're local. We shouldn't have to do this.
[54:15] - It is bash. - Is it?
[54:18] Yeah, I mean, we should be able to do... There is a trick, but...
[54:23] Yeah, if you type in the word... Yeah, I'll type in what you can type in
[54:26] to refresh your bash. - Okay.
[54:29] This is fun. - Your name is Jim.
[54:36] Oh, you know, actually, we'll do it this way. Let's see if this works.
[54:41] Source bash RC. That actually reloads your bash RC.
[54:47] And then it will... Yeah, it will then hopefully update your command prompt,
[54:54] but if it doesn't, then I'm all out of Windows options. - Yeah, no, it doesn't like me,
[55:02] so it's not typing anything. I'm just gonna close it.
[55:08] We're gonna close it. - We'll just use this.
[55:10] - Okay. And can I use it in here too, to refresh the bash?
[55:18] - Yeah, possibly. I don't know how the command prompt,
[55:22] if it's connected to bash, or you actually have to use the bash thing,
[55:25] but it looks like your keyboard is unplugged or something. - What the heck?
[55:31] I don't... Me and this computer, it's better than nothing.
[55:38] It is better than nothing. It's frustrating.
[55:42] All right, well, I still restarted my command line, and zoom all the way in.
[55:51] - Yeah, can you type in this window? - Let's see.
[55:56] Yes. - Okay, so you should be able to use the gh command
[55:59] for cloning. - Okay.
[56:03] - Just copy it from the browser. - Yeah.
[56:05] Y'all, I am definitely struggle busing with this compared to my Mac.
[56:14] - Cool. All right, we are now...
[56:18] (indistinct) Yeah, this would be...
[56:20] - Ah, well, sure. Okay.
[56:23] So... Do yes, just...
[56:28] Not find... - Can't find the fingerprint.
[56:34] Oh, it failed. Do it again, because you should have typed in yes.
[56:39] I think it got canceled when you're moving the screen. - Yay.
[56:44] - Yeah, so type of yes here. There we go.
[56:55] - There we go. Yay.
[56:57] - GitHub trust this computer forever now. - Yay.
[57:01] - Cool. So now we have the repo.
[57:04] So we should be able to... It should be at the change directory into the hot repo.
[57:09] Okay, so... CD...
[57:16] - Yeah, CD hot. - So the keyboard also, the T doesn't work.
[57:22] It either double types it. This has been interesting, to say the least.
[57:29] Okay, cool. So I am in the repo.
[57:33] - Yep. So this is where all the work happens now.
[57:35] So we should always start with a new branch, 'cause you'll get to the point where you're like,
[57:40] "Oh, I'm gonna fix the thing." And I'm now, I'm still in the main branch.
[57:43] It's not looked or frowned upon, at least in the open source community,
[57:47] if you contribute from your main branch, but it's always nice to have separate branches,
[57:52] 'cause if you don't contribute from a separate branch, then you have to nuke the entire repo start over,
[57:57] and you shouldn't have to do that. So if you do git checkout -b.
[58:00] (keyboard clicking) - B? - Yeah.
[58:10] - Right? - Yeah. And then your name of your branch.
[58:11] I'll just call this what you're gonna be working on. I actually, in the contributing MD,
[58:17] I ask people to put their issue number in the branch name. It's always easy to look up later
[58:23] if your issue number is in the branch name. I already forgot what it was.
[58:29] So if you click on opensource-hot, just below your name. Yeah, right there.
[58:36] Going into, back into the issues. - Mm-hmm.
[58:44] - So I just do, I just type in 315 as your branch, and then tailwinds anti, or hero anti-pattern.
[59:00] - Okay, enter. - Yeah, you'll have to do dashes in between the spaces,
[59:16] 'cause the, it looks like, it's assuming that it's extra commands after 315.
[59:21] There we go. Now we have a branch.
[59:26] - Okay. - Cool.
[59:28] So now, the first step for the contributing MD, you should be able to npm ci,
[59:35] just to make sure you have all the packages local. - Like that?
[59:42] - Yeah, also, I wonder if we're not gonna have npm. Nope.
[59:47] - Ooh, my gosh. - So we're actually, we'll have to install node.
[59:54] This is a, I guess we both came in a lot of assumptions before starting this.
[59:59] The other, I guess there is, I mean, there's tons of other options we can use
[60:03] besides setting up your entire environment, but we might as well just go ahead and do it.
[60:08] - We're here now. - Yeah, and Vortex is saying that it's easy.
[60:13] Oh, Anthony's, he helped you with this last time. - Yes, yes, and then I get to set all of this up
[60:21] when I get my new machine again. Yay.
[60:24] - At least you'll, it'll be in recent memory, so it'll be really quick.
[60:29] - Yes, okay, so I need to install node. This, in case anybody, I just Googled it,
[60:43] but I don't think I Googled right. - Yeah, you can just go to nodejs.org
[60:48] and download it from there. (keyboard clicking)
[60:53] - Smarter, much smarter than what I was doing. Okay, download that one.
[61:01] Maybe. What up, Vortex?
[61:14] And yeah, this is, we are really showing someone how to like,
[61:19] really get started with all of this, like step-by-step. - They're questioning why you're not using 18.
[61:25] 18 is the latest one. Yeah, we'll probably download 18,
[61:31] mainly because you're gonna have to, I mean, I'm not sure how much code you're gonna be on.
[61:36] Oh wait, now Anthony's saying don't use 18. - He always tells me not to use the current one
[61:41] because it's gonna be buggier while I'm learning. - Okay, well, we'll just install one of them,
[61:48] it doesn't matter. 'Cause like what we're doing, either is gonna work.
[61:54] I don't know what this .msi is though. - I think the install for it, I don't know.
[62:00] Yes, it's preparing, we're doing 18 now. We just, we just, I went for it.
[62:07] 18 is what's being installed. - Yeah, we don't have any Lambdas to worry about.
[62:18] - Yes, install. It's really fun installing screen.
[62:29] - I'll take your word for it. Yeah, so there are a couple other options
[62:36] that I'd probably mentioned for folks you are contributing. Like Codespace is a really good option
[62:40] for folks who wanna contribute to open source for the first time, but don't have all this set up,
[62:45] or you're like maybe on a Linux machine, don't know how to get all that set up.
[62:49] Codesandbox is another good option. It's kind of like a watered down version,
[62:52] gives you an environment to run the shell locally. For what we're doing, Codesandbox
[62:57] would be like more than enough. StackBlitz is another one, Replitz is another one as well.
[63:02] Those are tools that will give you an environment with Git, Node, everything installed right away.
[63:08] And you just sort of get on your way to start changing the code up.
[63:11] (silence) And it's still installing stuff.
[63:21] - Yeah, it's gonna take some time. While this is working, can we pipe over
[63:31] to the Insights product that we can talk about finding open source projects?
[63:38] - Yeah, was that the... - Yeah, so if you go to opensauce.pizza.
[63:43] Cool, and it's like start now is the... - Start now.
[63:53] I like the pizza loading screen. - Yeah, I like it too. - I'm happy.
[64:00] - Yeah, so this is, we had mentioned around Hacktoberfest, and the one thing that I will question
[64:08] Vortex, Vortex is working with me on this. It seems like all of our contributions
[64:12] are bunched up to the day. I'm pretty sure we had contributions yesterday,
[64:15] but basically this is like Eagle Eye's view of what's happening at Hacktoberfest.
[64:20] So if you like went to repositories on that tab, you'll see a list of Hacktoberfest repositories.
[64:27] - Oh, cool. - And these are projects that are opted in.
[64:30] This is a contribution that what's happening at the moment. And if you go down to the, if you click on the filter,
[64:35] you can go to recent, and the recent will then give you, see where contributions are happening.
[64:41] So good chance if they're actively getting contributions, they'll probably have good first issues
[64:47] that you can also work with as well. - Click.
[64:55] - Oh, just a little bit to the left. I think the click area is actually too small.
[65:00] - Ah, so recent. - Yeah, it's a bug. - Yes.
[65:05] So yeah, if you wanna contribute to, I don't know what all these are.
[65:11] Open API generator, Lava Link, Gotham. Not sure what any of these projects are,
[65:17] but they're all enabled at Hacktoberfest. - Oh, this is really cool.
[65:24] Yay, we gotta get open sourced on page one. - We will, once you merge your contribution,
[65:36] we'll be popped up to page one. - Once I--
[65:40] - Once you install Node. - Okay, really quick, it's to check
[65:47] and see if it installed the rest of it. It's Node-V? - Dash-V, yes.
[65:53] - Y'all, that is how, oh, I probably have to go out. I don't know.
[66:00] - Yeah, your path might, you might have to close the prompt again, yeah.
[66:05] - Yeah, let's just close it and-- - Yeah, there is a way, there is a command to do that,
[66:10] to refresh it, but to be honest, it'll take me longer to Google that too as well.
[66:16] - We'll just close, it'll be great. All right, so we have-- - Unless someone
[66:22] already mentioned it on the chat. Doesn't look like.
[66:27] - Yay, it's installed. - Okay, now we should be able to,
[66:32] now we can run npm install now, or npm ci, 'cause we have a lock file.
[66:37] - Npm install. Oh, I was supposed to do, oh, whatever.
[66:50] - I don't know what this is. - Am I supposed to do npm install ci?
[67:00] - No, you have to go into the hot folder. But yeah, ci-- - Okay, that makes, okay.
[67:05] - Ci would be better 'cause it'll be a little faster. - Okay, npm install ci.
[67:14] - Oh, just ci, it's one or the other. So I believe it's probably just gonna be installing.
[67:25] There's an error message. - I don't know what this means.
[67:31] This is, you have the wrong node version. Oh, it won't actually work with 18.
[67:40] Okay, there's a way around this, but we won't be able to contribute this up.
[67:47] Can you open up VS Code? I don't know what would be easier,
[67:51] to install a specific node version on top of what you already have,
[67:54] or just to change the package.json? So like what we're doing, we actually,
[68:06] in the package.json we're actually requiring specific versions.
[68:09] Yeah, we probably should use Volta, but I feel like that's a scope creep at this point.
[68:15] So go to the package.json and there's gonna be three different versions of node.
[68:21] We'll just add your version to the list. And then we'll get by.
[68:26] Yeah, we specifically require specific versions to unbreak people.
[68:29] - Where do I go for that? - Click out of this getting started page.
[68:37] And then I would go to open folder. - Oh, and open the hot, okay, got it, got it.
[68:42] - Yeah. You just scroll down, scroll up a little bit.
[68:47] Up, there you go, right there on the right. - Oh, thank you.
[68:52] - And select this, yeah. Always trust.
[69:02] Always trust the open source. - All right, and then we need to go to--
[69:08] - Package.json. And then on the bottom, you had these engines.
[69:16] So line 22, we can change that to 18. - Is it 18.0.0?
[69:26] - I honestly don't know, but it should tell you right there on the bottom.
[69:34] If you scroll all the way down, 18.10. It's in the error message.
[69:40] Yep, so now if you run that same command, just do it with just CI.
[69:51] All right, sorry, npmci. Nope.
[70:08] It said, oh, I guess that's not how we can change that. All right.
[70:17] This will be interesting. We might have to punt and just grab a Repl.it clone instead.
[70:24] - Can I just install the other nodes so both of them are on here?
[70:29] - I guess you can install the 16. Oh, Vortex is saying if you just do npm install,
[70:35] don't do CI. I guess that makes sense, okay.
[70:43] (keyboard clicking) Oh, okay, that makes sense.
[70:51] It's because the lock file that we're running from, actually, that's not great.
[70:56] That is not what it is. Sorry, I'm explaining it.
[70:58] Oh, and then the shrink wrap. Okay, so we have to edit it in the file
[71:04] above the package.json. You have to change that version as well.
[71:09] - Mm-hmm. (keyboard clicking)
[71:14] - So line 79. (keyboard clicking)
[71:39] All right, well, we can comment out the pre-install script. So if you look for the word pre-install.
[71:45] (keyboard clicking) Nope, in the, oh, sorry, package.json.
[71:57] There we go, just comment that line. If you do command backslash, yeah, there we go.
[72:07] You're good. Perfect.
[72:10] Yeah, having the good first issues is like this is the pathway to really learn
[72:19] what you're doing, which is, again, this kind of hammers down the point
[72:22] of why it's less about the focus of like what code you're actually fixing
[72:26] and more about just getting a bunch of people to go through the processor.
[72:30] JSON doesn't have, oh, you have to delete it. - Oh, yeah, okay.
[72:36] - Technically, that's not a comment. It's just breaking it.
[72:39] (keyboard clicking) And we'll just make sure not to commit that.
[72:43] This is quite an experience. Also, anybody who's watching
[72:47] who wants to do documentation updates, we're clearly finding some edge cases in documentation
[72:54] that would be perfect to contribute back upstream. - Still a no-go.
[73:01] - Yeah, it's literally the same error message. And it's mainly 'cause we're enforcing these versions
[73:09] are higher than node 16, but it's weird that node 18 won't work
[73:16] 'cause that technically is higher. But, hmm, change the engines, too.
[73:22] We did that. (keyboard clicking)
[73:32] (laughing) Bugs on bugs.
[73:44] All right, we could just delete all the engine, all the references to engines.
[73:49] - So, just delete this one? - Yeah.
[73:52] Yeah, you want that 729, line 729. Oh, yeah, we're in the wrong, sorry.
[74:02] Undo this one. We should do this in the packside.json.
[74:06] The shrink wrap itself, this is the lock file that comes out of the install.
[74:12] Yeah, you want line 24, as well, or line 22. All right.
[74:23] Moment of truth. (keyboard clicking)
[74:29] Yeah, it's like, yeah, this will be something that we should probably just open issue on.
[74:39] Could you, actually, you know what the thing is about finding good first issues?
[74:44] The best good first issues are the ones you find. So, could you open an issue in the hot repo?
[74:50] And we'll talk through that. Unfortunately, we'll have to punt
[74:54] on making this contribution. - Yes.
[74:56] - Even though it was extremely, just double check to see if you're in the right folder.
[75:02] Oh, yeah, you are. Okay.
[75:03] Let's just open an issue around node 18, and then we'll address this upstream in the repo.
[75:11] - Okay, give me just a second. - Yeah, 'cause I don't know if we have a hard stop.
[75:17] - That's more up to you. I'm good for the moment, but.
[75:25] - Yeah, I do have a meeting in 15 minutes. - Yeah.
[75:29] So, we'll come back to this later on. You'll just be back on the show.
[75:36] Okay. - Yeah, so if you just click on new issue,
[75:41] this will give the opportunity to talk about some other stuff.
[75:43] Yeah, so I'm a strong believer, not only that good first issue should have issues,
[75:50] like sort of have the answer in it, but also it should be dead simple to also open up issues
[75:55] because like we clearly hit a roadblock trying to install this on Windows.
[75:59] If we were using like a sort of like MVM or Volta, like we easily just install another version,
[76:06] but I don't know if that will work for us and how we can install an older version from the binary
[76:13] without deleting the previous one. Anyway, it becomes more of like a maintenance nightmare
[76:17] to do it that way. So, if you just click on bug report,
[76:21] I would just create a new bug that basically says node 18, node V18, not supported.
[76:28] And I'm curious, have you seen the issue forms before? - No, this is something that,
[76:49] I think these were pretty easy, but something that I do wanna comment on
[76:54] when we do fix the bug and the check mark is like it's in markdown,
[77:01] so I was totally doing it wrong last time. So, I'm like, I was planning on mentioning this one.
[77:07] This one seems pretty easy. (keyboard clicking)
[77:15] (keyboard clicking) To clown and create branch on Windows machine.
[77:25] (keyboard clicking) (keyboard clicking)
[77:46] (humming) - Do you have the engine error message?
[78:12] When you did npm install, there was like error message that came out.
[78:16] If you scroll up just a little bit. Oh, no, sorry, it's in the bottom.
[78:24] I see it. So, where it says red error,
[78:26] I'd copy just a couple lines above that. - I'll just get all of these.
[78:32] Then it's on. - Yeah.
[78:35] - Anything, you guys will have it. (keyboard clicking)
[78:42] - Yay. Oh, should I have put it in the code version?
[78:47] - It makes it a little more easier to read. That works.
[78:53] - Steps to reproduce. Watch.
[78:57] - Watch the stream. - DOD of stream.
[79:02] Affected services. Hot.
[79:09] - Yeah, that works. - Hello?
[79:13] Chat. I'm breaking stuff.
[79:16] It's fun. Browsers.
[79:21] Chrome. In a new environment.
[79:24] - Yeah, technically, we can just leave this blank because this is more of like a contributing bug
[79:33] than an actual bug in the UI. - I agree.
[79:37] I agree. Submit.
[79:40] - There we go. - Yay.
[79:45] That was fun. - Yeah, so the beauty of open source is even if we fail,
[79:51] we win by opening up issues. - All right.
[79:54] All right. So we have created issue number 350.
[79:59] This is exciting. - Yeah, we had a good run.
[80:03] - There was quite a bit that we went over today. And as a heads up, I will be creating shorter videos
[80:11] talking about how to, what open source is, how to find projects, those type of things to kind of recap.
[80:19] And then we'll be Dougie, you're invited to come back again. So hopefully I'll have my normal computer
[80:27] and it'll be working. So that way we can actually go through and see what it says
[80:33] and go through the issue. It's a good first issue.
[80:38] - Yeah, sounds good. - Yay.
[80:41] All right. Anybody have any questions that you want us to follow up on
[80:44] before we end the stream today? Because I know we had quite a few more people.
[80:51] What up, Cynthia? Thank you for joining.
[80:55] Vortex, I did say hi to you while I was like slightly panicking going through all this.
[81:02] Rizal, I need you back on the show. Like we need to talk about some Git actions
[81:08] and so much more. And yeah, this is everybody that I've been missing.
[81:16] Oh, and Ramon. I'm literally scrolling up and catching up on all of this.
[81:20] So hi, Ramon. And let's see.
[81:26] Oh, Mo, let me know what questions you have and we can work through getting those put
[81:35] into the next stream and/or the videos I'll create. So yes.
[81:44] And we're also trying to get Cynthia to come on to talk to me about apps for Discord
[81:51] 'cause she knows how to make them. Very exciting.
[81:55] All right. Well, goodbye, everyone.
[81:59] I hope you have a lovely rest of your Monday. Thank you, BDougie for coming on today.
[82:04] And yes, Mo, it is going to be on YouTube. Let me grab that link for you.
[82:13] And eventually I will have enough subscribers on YouTube to be able to have the actual proper name on here.
[82:23] - How many subscribers do you have? - On YouTube, 59.
[82:30] - 59, all right. - Anthony is fast.
[82:35] - Gonna make it a 60. - Yes!
[82:38] Yes! Thank you, Vortex, for helping.
[82:44] Well, thank you for subscribing. And thank you, Vortex, for your input.
[82:50] I appreciate it. And everyone, have a lovely day.
[82:53] We will let you know when we continue this conversation. So thank you.
[82:58] Bye. 
