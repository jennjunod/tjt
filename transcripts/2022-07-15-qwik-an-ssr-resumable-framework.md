---
showLink: "https://www.youtube.com/watch?v=tdEelSqDj0E"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "qwik-an-ssr-resumable-framework"
title: "Qwik, an SSR resumable framework"
publishDate: "2022-07-15"
coverImage: "https://i.ytimg.com/vi/tdEelSqDj0E/maxresdefault.jpg"
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

[00:00] - Hello, beautiful humans. Thank you for joining Teach Gen Tech.
[00:05] Today we have Misko joining us, and I'm very excited 'cause this is a brand new concept
[00:12] to me as I've been learning about JavaScript and frameworks. So Misko, please introduce yourself
[00:19] and what we're gonna talk about today. - Hi Jen, thank you for having me.
[00:24] We're gonna talk about today about this thing that I'm creating called Quick.
[00:28] A little bit about me, let's see. I did this thing called AngularJS that got kind of popular,
[00:32] so that's my prior life. Currently working as a CTO at Builder.io,
[00:37] and at Builder.io we're making a very cool, we're re-imagining the way headless CMSs work.
[00:43] So that's kind of what I work on these days. But Quick is my passion right now,
[00:47] and Quick is a framework for building web apps, but it's very different than existing frameworks
[00:52] in that it really focuses on, or rather, let me preface it with,
[00:57] existing frameworks usually download all the JavaScript eagerly,
[01:01] and then the application runs. And what Quick does is it goes the other way around.
[01:05] It tries super hard not to download any JavaScript until it absolutely has to.
[01:11] And for small applications, obviously it makes no difference,
[01:14] but once the applications gets large and big, it makes a huge difference in terms of performance.
[01:19] - Interesting, and to take it back a bit, I've started to learn a bit about formats
[01:30] and different ways that JavaScript can be. There's vanilla JavaScript that can't do,
[01:37] or it's the bare basis that everything's based off of, and then there's, I've done some work in React,
[01:45] I've done some work in Express. If I remember correctly, we built a web app,
[01:53] and it was much more of the front end, where when we were doing Express,
[01:58] it was much more of the back end. And eventually, those two are gonna be on the show together
[02:04] to help me go from making a full app, it's gonna be fine. So where does, to take it a step back,
[02:12] I know we're focusing on Quick, but where does Angular and Quick go into that?
[02:17] Are they similar to either of those, since those are the ones- - Yeah, yeah, they are.
[02:21] So I think the category is front end, right? So on the end of the day,
[02:26] you need to render something on a screen, right? You have to put characters and colors and boxes
[02:30] or whatever on the screen. And so you could do it manually, you just pure vanilla JS,
[02:35] but you're gonna discover pretty quickly that that's just a lot of boilerplate boring code.
[02:41] And for that reason, people create frameworks, and there's AngularJS, Angular, Swelt, Vue, React, Solid,
[02:50] just name a few, there's gazillions, bajillions of them. And they all basically try to solve this particular problem
[02:56] by saying, "Hey, let me give you tools so that you can have easier time making things,
[03:03] painting things on a screen. And more importantly, easier time updating it."
[03:09] 'Cause it's one thing to just paint something, quite another thing to be like,
[03:11] "Okay, now I have to go update it." Because now you change something, you click on something,
[03:15] or you added something to a shopping cart, right? And so the bread and butter of what frameworks care about
[03:22] is how do I show you stuff, and then how do I update stuff based on your interaction?
[03:26] - Got it, got it, yay. I feel like this is gonna be,
[03:32] this is something that I've learned since joining the, working more on the backend of the tech world.
[03:41] And I'm saying backend of tech world, not just like backend developer, not there yet,
[03:45] but I've been in sales and in marketing and learning services.
[03:49] So it's much more teaching about the technology after the technology is developed
[03:54] is very different than being part of building the technology and updating.
[04:00] And it's definitely something that it's, I've been on this journey for maybe a month now
[04:10] where I started working on learning JavaScript and then I've always wanted to become a DevRel.
[04:17] And so while I was working on finding out more of how to be able to do that,
[04:21] everyone's like, "Yo, you got the personality, but you don't have the tech or content."
[04:25] And I'm like, "Oh, well, we're gonna do teach gen tech and get both."
[04:29] So I love that it's, they all build on top of each other. And it's so similar yet different.
[04:39] And also something that I really do wanna call out of thank you for being human.
[04:45] I know we touched on this very, very briefly, but I was very nervous about this.
[04:50] And I feel like this is something that so many newbies getting into tech are like,
[04:55] "Oh, I don't understand the tech." And there is a big comparison of what,
[05:02] not all people can break it down or want to break it down. That's something I've learned on the podcast I also have
[05:10] of like putting that intellectual burden on people. It's not something that's made for everyone,
[05:15] yet there are so many kind people in this world that are definitely willing to break it down for you.
[05:21] And so thank you again for joining. - So what you're describing is this thing
[05:27] called curse of knowledge, right? Like once you understand something,
[05:31] you have a really hard time imagining what it is not understanding something.
[05:36] And this is a general problem for people, for humans, right?
[05:39] Is that once they understand something, it's like, it's obvious.
[05:42] Of course it's obvious. Like, how are you so dumb not understanding something?
[05:45] Well, it turns out before you understood this, you were also on the other side
[05:50] where it wasn't obvious at all. - How long did it take you to build Angular
[05:57] and then now Quick? Is it something that you did pretty quickly,
[06:00] like six months or- - No, it takes a long time.
[06:02] So let me back up a little bit first. And I wanna point out that I feel like anything in life,
[06:10] including software, right? It's not that it is complicated.
[06:14] Like every single part of it is pretty simple. It's just, there's a lot of it, right?
[06:20] So if you've been doing something longer, it's not really that you understand.
[06:25] I mean, things build up on each other and become complicated, right?
[06:28] But like the thing I really wanna get across, and I always tell this to my kids as well,
[06:32] is that it's just jillion small things that are in themselves pretty simple
[06:37] and straightforward, right? The difference really comes down to is just,
[06:40] there's just so many of them. And because it's so many of them,
[06:43] it really just comes down to like the amount of time you spend on it, right?
[06:46] So it is just like, you have to spend a lot of time on it to kind of go through it and learn all these things.
[06:52] But individually, they're all pretty straightforward. - I love that.
[06:56] - So you asked me how long it took me to build AngularJS. It's pretty long time actually,
[07:01] because I didn't know what I was doing, right? It's a learning experience for everybody.
[07:05] I think AngularJS took about two years, but I mean, that was a long time ago
[07:09] and I can't quite remember. With Quik, it was much, much quicker, ha ha, quicker.
[07:14] It was only about a year, maybe a year and a half. We kind of knew already what we wanted.
[07:22] And so we were able to just go straight after the particular goal.
[07:25] But Quik is also a lot more ambitious than what AngularJS was trying to do.
[07:30] AngularJS was one of the first ones in this particular space.
[07:34] I think the way you think about it is, it kind of went through stages.
[07:37] You know, at the very, very beginning, browsers didn't really even have JavaScript, right?
[07:43] They were not really interactive. And so you just showed static documents.
[07:47] And so on a server, you would generate the HTML, send it to the client, the client would show it,
[07:51] and that would be that. And at some point we added JavaScript.
[07:54] And so we're like, oh, now we can make it interactive. And the first kind of interaction we added
[07:59] is that servers still produced HTML. And then after the fact,
[08:03] we sprinkled JavaScript on top of it. So we generated the content
[08:07] and then we made the content interactive. - Okay.
[08:12] - And the problem with that approach is that you kind of have to do it twice.
[08:15] You do it once on the backend, like, oh, I'm generating a, whatever, a clock, right?
[08:19] So I have to generate the clock. And then you go to the client and you go like,
[08:22] oh, right, the client has to update. So now I have to write code
[08:25] that is pretty much identical for updating the clock, right? And so creating the clock and repainting the clock
[08:31] end up being two things that you write in two different locations
[08:35] and two different languages and it gets annoying pretty quickly.
[08:38] And so people were looking for kind of the unified answer to this particular problem.
[08:43] And the answer came in this component-based frameworks, I guess you could call them.
[08:48] And I like to think that AngularJS was one of the first. But the idea of component-based frameworks
[08:55] is that you write a component and then that component runs both on a server
[09:01] and on the client. Originally, that wasn't the case.
[09:03] Originally, they only ran on a client, but then we kind of realized like,
[09:07] oh, if it just runs on a client, then it takes a long time for the page to be painted, right?
[09:15] So you navigate to a page and you just see a blank page, right?
[09:18] Like just whiteness. And then the page says,
[09:22] oh, you need to go get the JavaScript and the framework and the application and everything.
[09:26] And so you go fetch all that stuff and then you go and execute all that stuff.
[09:29] And so at some point, like a couple of seconds later, everything executes and downloads and runs.
[09:33] And like, now you have your clock painted, right? And so there's a huge delay between like,
[09:38] I navigate to a page and then I see something. And that's kind of the problem with like
[09:43] the first generation, like you wanna call generations of frameworks.
[09:48] And so people came up with this idea of server-side rendering, right?
[09:51] And the idea is like, well, what if we ran the code on the server first,
[09:57] it's JavaScript, right? So we could do that.
[09:59] And then we can get a static snapshot of what the page will look like,
[10:04] send the static snapshot over to the client. And then in the client, you would run the code again,
[10:12] but instead of just staring at a blank page, you're now staring at the actual application.
[10:18] Of course it doesn't work, right? It's just like a painting.
[10:21] - Okay. - But you have like, oh, at least I'm recognizing,
[10:25] oh, it's a clock. What can I do over here, right?
[10:27] I'm gonna think about it. Hopefully by the time you kind of figure out
[10:30] like what I wanna do. No.
[10:33] - I have to go. - Okay, you go buddy.
[10:36] Sorry. Hopefully by the time you figure out what you wanna do,
[10:40] the page was able to initialize and run all that stuff and become interactive, right?
[10:46] So we went from like white page to like wait two seconds to having an interactive thing to, you know,
[10:52] having a painting of the thing that you want, wait two seconds and then have an interactive thing.
[10:58] And so that's an improvement. And so collectively we call that the service side rendering.
[11:04] - And thank you for explaining that. I think that's something that like I've had,
[11:08] I've worked at, previously worked at GoDaddy. So when I was in the hosting department,
[11:14] that was a big thing was, you know, load time on websites that helps SEO, all of that.
[11:19] - Yes. - So I never knew all of this went into it.
[11:24] So it's definitely very cool to learn about. And hi, Dan, thank you for joining.
[11:29] And I think Mishko is definitely no longer gonna be a mysterious white void 'cause he's joining today
[11:38] to talk about it. - Why was I a mysterious white void?
[11:41] - Because nobody like, you've done this cool thing. And so like nobody, it's, I think this is something
[11:48] that happens a lot in any industry where people that have accomplished something or is well-known,
[11:56] people are like, oh, well they're, yeah. Or they're untouchable, like, oh, we'll never hear from them
[12:03] or something like that. It's something that I've heard from a lot
[12:07] of different platforms. And it's like, no, like it's just harder to get them
[12:11] because they get so many messages. - Yeah, but like, I mean, I understand how it could go
[12:19] to your head, right? Like, but I think at the end of the day,
[12:22] most people are pretty down to earth. It is, just comes down to like, you know,
[12:26] people get a lot of messages. And so he's trying to juggle everything.
[12:30] But I, you know, at the end of the day, people want to have fun anyways.
[12:33] And so like, it's nice to come on a show and talk about things.
[12:35] And like, oh, this is my relaxing time, you know? - And thank you for that.
[12:40] And just for all of the humans that have joined as a heads up, Misko does know that he's gonna have
[12:47] to break it down quite a bit for Teach Gen Tech. Like, we're not 100% there.
[12:53] And Misko, I really appreciate you breaking down a bit of the, I could almost say the theory behind it,
[13:00] or you know, the-- - Yeah, that's the theory of it, yeah.
[13:02] - Yeah, the theory of it. It really helps learning the theory to understand
[13:06] what we're gonna be going into. - Okay, so since I already gave you three quarters away
[13:11] on a theory, so let me just finish the story. - Perfect.
[13:14] - So like, you know, think about the stages, right? Stage one is everything is just server-side rendered
[13:20] and there's no interactivity in the client, you have static pages.
[13:23] So obviously we're like, hmm, that doesn't work very well, we want interactivity.
[13:26] So stage two would be like, okay, server-side rendered, but then you sprinkle JavaScript on the client
[13:32] to make it interactive. This was kind of like the jQuery days.
[13:35] And the problem there is like, you're duplicating work and it's kind of hacky.
[13:38] It's ad hoc, it's not like, it doesn't scale very well, basically.
[13:42] So then people are like, okay, I have an idea. We'll do everything in JavaScript.
[13:47] And so you have the client-side frameworks that are borned. And then the problem becomes,
[13:51] yeah, but it's slow before it interacts, right? There's this white void before like I can work it.
[13:58] And so the server-side rendering is the answer. It's like, ooh, we'll pre-render on a server,
[14:02] send you the image, snapshot, right? It's not interactive, it's dead.
[14:08] You can't do anything with it. But hopefully by the time the JavaScript wakes up
[14:11] and does its stuff, we have made it interactive and you won't even notice the switcheroo
[14:16] and then you can play with it. So that's kind of where we are.
[14:19] This is the kind of the status quo. And so the thing that's different about Quik is that,
[14:26] well, let me back up a second. The problem is that there is this delay
[14:32] between like, you think you have a page, like imagine somebody- - Really, Quik,
[14:37] it's sounding really robotic all of a sudden. - Oh, no, is it me?
[14:42] - I hear it when you're talking. - Now you're muted.
[14:46] I can't hear you. I cannot hear you.
[14:54] - I don't know what all my mics and stuff are trying to do. This is when we have backup.
[15:04] (mouse clicking) - Okay, I think your mic is working and I can hear you now.
[15:12] (mouse clicking) (mouse clicking)
[15:17] While we're waiting, I think I can tell bad computer jokes. That's my favorite thing.
[15:45] I like dad jokes and I tell dad jokes to my kids. - That would be great too.
[15:51] - So do you know where I keep my dad jokes? - No, where?
[15:55] - In a dad-abase. Okay.
[16:04] - Okay, cool. And apparently it was just me.
[16:07] So, you know, Bluetooth headsets are amazing, but not always your friends.
[16:11] So, you know, got to go back to the old, sturdy plugin. - Yeah, so Bluetooth is, well, let's not go there.
[16:19] It's a complicated thing. Okay, so where were we?
[16:23] We were talking about kind of how we went through stages developing our applications, right?
[16:28] And so currently we're in this stage where, you know, you're on Twitter,
[16:31] somebody sends you a link and it's like, I don't know, shoes, you want to buy shoes, right?
[16:34] You click on the shoes and you immediately see the shoes and there's a buy button, right?
[16:39] And you try to click the buy button and it doesn't work because it takes like, I don't know,
[16:43] 10 seconds for all this JavaScript to kind of wake up and do its thing, et cetera.
[16:47] And finally the thing works, right? And so people are like, you know, screw it, you know,
[16:51] I don't even need the shoes that much, and so they leave. So there is a need to have the applications
[16:59] that just come on instantly, right? The problem is that we kind of don't have the technology,
[17:06] right, like the technology we have is server-side render, HTML, which is a static snapshot, right?
[17:13] Send it to the client. While the person is looking at the static thing,
[17:17] we download all the JavaScript, all the behavior, and then we re-render everything.
[17:23] And when you do this, like switcheroo, where we're like switch you the interactive one
[17:26] for the static one, and hopefully you don't want to even notice.
[17:28] And then you can do stuff. And the problem is on a mobile device,
[17:33] that could be like 10, 15, even 30 seconds, right? It's like.
[17:38] - I have like, I don't know if I can still imagine that. Like everything loads so quickly.
[17:43] - It depends. Like, so, you know, if you have an iPhone
[17:47] and if you have a 5G network, it's not so bad. It could be like a couple of seconds.
[17:52] If you on the other hand, have like an old, super old Motorola device, right?
[17:56] And you're like in 3G, then yeah, it can take a long time. Okay. - Yes.
[18:00] - So QUIC is basically what we, I like to think of it as a next stage
[18:05] of this particular game. And what the QUIC tries to do, it says,
[18:08] you know what? Instead of sending you static snapshot, you know,
[18:15] and then trying to spend all this time trying to figure out where the,
[18:20] so let me back up a second. Like what makes a HTML static, right?
[18:25] And the answer is, well, it's the lack of listeners, right? You didn't attach any behavior to it.
[18:29] So you have the tree, you have everything rendered, but there's nothing attached to it.
[18:34] And because there's nothing attached to it, like, you know, clicking the button doesn't do anything, right?
[18:38] Because you didn't tell the computer or the browser, like what should happen when I click this button?
[18:43] And because you didn't tell that to the browser, obviously browser won't do anything, right?
[18:48] Like you're clicking a button, nothing happens. - Right.
[18:51] - And so the problem is like, well, how do we figure out what listener goes where?
[18:59] And the answer to it is this process we called hydration, but basically just means just run the damn application
[19:06] from the very, very beginning and whatever it produces, that's for your listeners, right?
[19:11] - Got it. - Running it from the very, very beginning
[19:14] is huge amount of expense that we would like to avoid. So Quik has kind of coined the term called resumable.
[19:22] And the idea behind Quik is that you want to run the application on a server, get it to a particular state,
[19:28] serialize it into the HTML, including the listeners, send it to the client and the client can just continue
[19:35] exactly where the server left off, right? And so because of that, you get rid of that time,
[19:42] this delay, right? So Quik is kind of weird and hard to explain
[19:46] because we usually, when you look at different frameworks, you are comparing the developer experience.
[19:53] Like, do I use templates? Do I use JSX?
[19:57] Do I, you know, like how exactly am I gonna tell the computer what to do, right?
[20:02] And some people like one, some people like the other, and like, you know, we have debates about what's better,
[20:06] like whatever, right? And at the end of the day, it doesn't really matter.
[20:09] You're just really telling the computer, like, I want this to happen.
[20:12] - Right. - So the thing that's different about Quik
[20:15] is not how you tell to the computer, but actually what Quik does underneath
[20:20] so that it can skip this step, right? And so when you start looking with, playing with Quik,
[20:27] you look at it, you go like, this looks just like React. And the answer is, yep, that's kind of intentional.
[20:30] Like, you know, the fact that it looks just like React is not a coincidence.
[20:34] But what's different, what's unique about it is what actually happens.
[20:39] Now, for a small Hello World app, you know, the difference is kind of trivial and not really interesting
[20:43] but if you get like into a large application, the fact that Quik can skip hydration is pretty cool.
[20:50] Maybe I'll tell you one more thing and then we jump into maybe some coding.
[20:55] - Cool. - Are you familiar with virtual machines?
[20:59] - Like virtual servers or? - Yeah, like, so VMware came out like maybe 20 years ago
[21:07] and they had this crazy thing that was kind of mind-blowing when I first saw it, where you could open up a browser,
[21:14] oh, sorry, open up like another computer inside of your computer.
[21:17] - No, yeah, yeah, yeah, yeah, yeah, okay. - And so the main computer is called the host computer
[21:22] and the thing that you're opening inside of it is called the virtual computer.
[21:25] And it was kind of like, like, what? The craziness is this.
[21:31] So the thing with the virtual machines is that you are, for example, running on a Windows
[21:36] and you boot up like Linux inside of it, right? Inside a virtual box.
[21:41] And then the boot up process is slow, like in old computers,
[21:45] like it takes several minutes for it to come up. And then once it boots up,
[21:50] the crazy thing you can do with the VM is you can, let's say you open up like a Chrome browser,
[21:55] you can save it and it saves it to the disk and then you can take that file
[22:00] and you can give it to your friend and that friend can like just resume the file
[22:04] and they skip the boot up process, right? They don't go through boot up and opening up Chrome,
[22:11] they literally just open it and they're like, Chrome open, application running, you know, system booted.
[22:16] Like, what? - That's cool, I didn't know that.
[22:18] - How did you manage to skip the stuff in between? - Yeah.
[22:22] - Well, that's because the VM fully saves everything into that file so that it can just resume where it left off.
[22:30] And this is what we mean by resumability. So the thing with QUIC that we're trying to do
[22:37] is we wanna make the web resumable. So we want the web to be just like the VM machine
[22:42] where the boot up process, right? That is called the hydration or like the thing
[22:47] that figures out where the listeners go and grounds the application and all that stuff.
[22:51] We wanna skip that part, right? We wanna go straight to like,
[22:54] okay, the application is running, go, okay? And so that's kind of the magical bit behind QUIC
[23:02] is it's not that it's trying to build the app differently or like in a different style
[23:07] from a developer point of view, it's that what happens underneath is different.
[23:13] And the result is that instead of forcing the browser to download all the JavaScript ahead of time
[23:19] and then execute all the JavaScript ahead of time, which is expensive,
[23:22] we figured out a way to do it the other way around where like the browser doesn't really download anything.
[23:27] And then when you start interacting with the page, then we only download that very specific thing
[23:32] that's needed for that interaction, right? So like, if you look, think about a large application,
[23:37] like Amazon app, right? You could have like code
[23:40] for like adding things to shopping cart, code for like looking at the product from a different angle,
[23:45] code for like commenting on the product, code for like sending a review,
[23:50] code for asking for refund, code for like navigating,
[23:53] like there's a bajillion things you can do, right? - Right.
[23:56] - But you don't do all of those things at once. You only do one of them, right?
[24:00] Like I wanna look at the product from a different angle is just a tiny sliver of what the application can do.
[24:07] And so instead of downloading everything ahead of time and then running everything ahead of time,
[24:13] which is expensive, Quik basically says,
[24:15] "Actually, you only want to just look at the product from a different angle.
[24:18] So I'm only gonna download that particular piece of code." - So that answers my actual follow-up question,
[24:25] which was gonna be, what is the difference of that compared to caching?
[24:29] And how you explained that it only loads that particular piece,
[24:33] that's gonna be a lot different than caching where it previously loaded
[24:37] and tries to cause it to go a bit faster. - Yeah.
[24:44] So, I mean, caching is a very complicated term in terms of like,
[24:48] it could be used all over the place, right? So like not exactly sure what you mean by it.
[24:51] Like in the case of HTML, when you render the HTML on a server,
[24:57] we definitely cache that on a system that's called a CDN content delivery network.
[25:02] And so CDN is basically the thing that actually serves up the file.
[25:08] And so, yes, you can definitely cache it at that layer so that when you navigate to the sneaker, for example,
[25:15] the CDN can instantly just be like, "Yo, here's the file, go."
[25:19] - Yeah, I'm thinking more like browser caching because if we're on the browser side,
[25:25] we wouldn't necessarily need it to be cached because quick is made to load
[25:30] when just for a specific part, it doesn't need to previously,
[25:35] like it'll load faster from the very beginning instead of having to have it cached
[25:40] on the browser side to be able to load quicker. - Yeah.
[25:43] So caching is about faster delivery of the content. But there's a second problem,
[25:49] which is when the application starts up on the client, it has to execute the application, right?
[25:59] And browsers don't really know how to cache the execution, right?
[26:04] The execution is actually code running that has to happen, right?
[26:07] - Okay. - So even if you somehow deliver
[26:11] all the JavaScript quickly to the client because it's cached and whatever,
[26:15] you're still paying for the cost of like running it all. And so in a way,
[26:20] you can think of a quick as a way of caching it. So quick basically figured out a way
[26:26] to run it once on a server, cache the result in such a way
[26:32] so that on the client, the client, the browser can continue
[26:37] from where the server left off rather than going all the way to the beginning
[26:42] and redo all that work. - All right.
[26:46] I think like it sinks in enough. This is something that I've definitely had to learn
[26:49] where I'm like, it makes enough sense, yet it's going to be something that I got a noodle on
[26:54] and knowing my luck, I'm going to have like a question for you
[26:57] in like two weeks and being like, okay, cool. I will tweet you and see if I can get this answered.
[27:03] - You know, this is a hard concept because like we've been actually struggling with it
[27:08] to explain it to the people on Twitter of like how different it is
[27:12] because people are used to looking at the world in a particular way.
[27:17] And so if you come with something different, they're like, so it's just like this other thing.
[27:20] It's like, no, no, no. So it's just like that thing.
[27:22] It's like, well, no, right? And so it is a different enough thing
[27:28] that it's not immediately obvious why it's different. - Okay.
[27:33] But I think I enjoy being newer to it because I'm like, okay, cool.
[27:38] Like I do, like we all do need to compare it to something because it's kind of hard to conceptualize
[27:44] yet at the same time, I'm like, I feel like I'm new enough
[27:47] that I'm like, I don't have a ton to compare it to. - Okay.
[27:51] Let's do some coding and let's see if examples will help it. So, okay.
[27:56] You have a new thing here. Excellent.
[27:58] The magical command to get started with Quik is NPM, create Quik at latest.
[28:06] Quik at. - Latest.
[28:11] - There you go. So that should download and install things.
[28:17] Yep. And sure you can start with that folder name.
[28:24] - Okay, that works. - And so you want to do Quik City?
[28:29] Yep. Express sounds good.
[28:33] Prettier sounds good. - I do like prettier.
[28:38] It makes me happy. - Yeah.
[28:40] So now you can follow those steps. So city into Quik app and then do NPM install.
[28:46] And then we should probably get the visual studio running inside of that folder so that we can look around.
[28:52] - This is a very, very random thing to appreciate, but it's pretty and it has emojis.
[28:59] It makes it easier to comprehend as somebody that's newer to this,
[29:07] as someone that is, I'm also horribly dyslexic. So it'll take me a while to like re-read things.
[29:13] Having the different icons and like next steps and those types of things makes it a lot easier
[29:19] to go look at it and go, okay, cool. This is what I've done so far.
[29:23] These are next steps. So compliments on that.
[29:26] - Thank you. I will let Adam and Manu know.
[29:28] Adam and Manu are the two people who are working on it most of the time.
[29:33] - Yes, please thank them. I'm so getting used to this keyboard.
[29:40] I'm used to typing on my laptop itself. And since having to do two screens,
[29:45] I'm like, wait, this is a new keyboard. - I type fast on a keyboard, except when somebody's watching
[29:52] and then I can't type to save my life. - Well, I'm glad that it's not just me.
[29:58] - It's the moment somebody's watching. You're like, well, I can't type.
[30:02] - Yes. And for those that are watching,
[30:08] do you have any questions so far? I feel like a lot of you are
[30:12] on the more technical side as well. And we went through theory of some basics,
[30:19] which I really appreciate. So anyone else have any questions so far?
[30:25] - Before you type npm start, if you type code dot, it should open up the VS code in that folder.
[30:31] It's code space dot, sorry. - Yeah, you're right.
[30:34] - Ah, nevermind, okay. - Well, it's my VS code doesn't--
[30:39] - That's okay, that's okay. I'll just click on the open button over there
[30:42] and then we can just open the folder. - I need to remember where it is.
[30:50] It's supposed to be in here, but I didn't move it into there, so it's over here.
[30:55] - Quick up at the top, here we go. Yep, there we go.
[30:59] - Yay. - Okay, so if we just do npm start over there,
[31:07] it should open up the VS code in that folder. It should open up the VS code in that folder.
[31:13] - Okay. - And yep, if you open up localhost 3000,
[31:18] usually if you do it in Cognito window, it's kind of nicer because we can make sure
[31:23] there's no third-party extensions adding JavaScript, which happens often times.
[31:34] Okay, so here's your hello world of Quick City. This would be identical to just about any framework
[31:43] you would open up, right? That is not kind of the interesting bit.
[31:47] So I want to show you the interesting bit. So if you right click on it somewhere
[31:51] and go open up the developer tools, go to the network tab.
[31:58] - Let me get this bigger. It like went into a very weird--
[32:03] - Okay, and refresh this page again. Okay, and let's see.
[32:11] So if you click on JS, you have it on the top, it says fetch code, it says JS.
[32:17] Fetch XHR and JS CSS, it's a-- - Yes.
[32:22] - To the right of it. No, the JS one.
[32:23] So I only want to see the JavaScript that's coming down. Okay, so we're in a dev mode.
[32:29] And because we're in a dev mode, we're using this thing called beat.
[32:32] Beat is like a server for refreshing your thing. And one of the things it does
[32:36] is called hot module reloading. Anyways, beat is a dev mode only thing,
[32:40] and it would not be available in production. So we're only seeing it.
[32:45] So you see where it says filter, you can type in beat, and then there's a check mark that says invert.
[32:50] And then click on the invert check mark. Okay, and the thing I want to show you
[32:56] is that you have no JavaScript downloaded onto the page. - Okay.
[33:01] - Because Quick kind of figured out, looked at it and says like, well, this is a static page.
[33:07] There's no need for JavaScript in here anywhere. And so it didn't send anything down.
[33:11] If you were to use any other framework, like whether it be, it doesn't matter,
[33:17] like whatever framework you would choose, the existing frameworks basically can't do this.
[33:24] They would be like, oh, code. Let's send it over to the client,
[33:27] whether you need it or not. Now there are ways to disable JavaScript,
[33:32] like in a page where it's completely static, like, of course you can disable on any framework
[33:38] sending them the JavaScript. But what we're going to show you in a second is like,
[33:41] what happens when some things are interactive and other things are static?
[33:45] Then like you can't just disable JavaScript, right? And the thing is that existing frameworks,
[33:51] they can't differentiate. And so they always send all the JavaScript to the client
[33:56] and they always execute it, right? And I imagine in a normal setting,
[33:59] what you were having here is a situation where, you know, you send a static page to the client
[34:07] and then you send the JavaScript and the JavaScript like redoes everything
[34:10] and then repaints the static page only to come to the exact same state,
[34:14] which was completely pointless. But the reason we did that is because we didn't know
[34:18] what if there was a behavior over there? What if there was a listener that we needed to find?
[34:22] And because we don't know, we had to do it. And so QUIC, because it works differently,
[34:28] can be intelligent about it and be like, actually, I looked at it
[34:31] and I decided that there's no behavior and so there's nothing that I need to do.
[34:35] - Everything you are saying makes sense. I think something that I'll have to try later on
[34:45] is doing this exact same thing with like what I built with React
[34:49] and then what I built with Express, because it's like what you're saying makes sense,
[34:55] yet a visual, I think is gonna be really good to do later on.
[34:59] I'm not too worried about it right now. I'm just excited that I got the hello worlds going on.
[35:04] - Okay, so let's open this file up. So I think if you go to your code, your VS code,
[35:12] and if you open up the source folder, and then inside of the source folder-
[35:17] - This is source folder, right? - Yep, it should be routes.
[35:21] And look for a file called index.tsx. And so this is your component, right?
[35:27] You can see welcome to quick city, the meta framework for quick,
[35:31] and this is exactly what's rendered. There's also a, what we call a layout.
[35:35] Layout is basically the banner on the top and the footer at the bottom.
[35:39] And that's controlled by the layout file in here. We don't have to worry about it just yet,
[35:43] but let's go back to index.tsx. So let's add some behavior, right?
[35:47] Because like as of right now, this doesn't do anything. And so it's not really that exciting.
[35:53] So let's say we want to allow you to click on the welcome to quick city title.
[35:58] So we can add a listener to it. So after H1, before the closing tag,
[36:04] you can just say on click, dollar sign, and the C is capital.
[36:09] - Unclick? - Before, sorry, before H1.
[36:14] So it's a bracket, H1 space, on click, close bracket, right? So before the greater than sign.
[36:22] - Okay, sorry. - Right there, yeah.
[36:24] So space, on click. No, on, on, as in like, yes.
[36:30] - On click? Okay, dollar sign.
[36:32] - It's trying to complete it for you over there. And so in here, there's going to be an arrow function.
[36:38] So open, close parentheses, fat arrow. And then let's do something simple, like alert hello.
[36:46] Yep, and so open, close parentheses, fat arrow means equal sign, greater than sign.
[36:53] - Equal. - Greater than, we call it the fat arrow.
[36:59] - Okay, see, these are the terms, like I'm like, I'm not used to hearing out loud,
[37:04] which is really helpful now that I'm learning all of that while doing these videos.
[37:09] - So now you can type in like, alert, and in parentheses, you can say, you know,
[37:15] hi, or something in quotes. It's alert, parentheses.
[37:20] - Like this? - Yeah, open parentheses, alert, open parentheses.
[37:26] - Okay, alert, open parentheses. - That's a quote, right, what you have on there.
[37:33] Open parentheses, there you go. And now quote.
[37:37] - Now quote. - Now hi.
[37:41] - Okay, here. - All right.
[37:44] - This is what I always type. - That sounds good to me, all right.
[37:49] So because Vite is running, when you save this file, it should automatically refresh the page,
[37:55] so there's nothing for you to do, okay? So now if you click on welcome to Quick City,
[38:00] it will send. - Oh, yay.
[38:03] - Okay, so the thing we're demonstrating here is that we have interaction now.
[38:08] And so while at the beginning, you could say like, oh, no JavaScript needs to be sent to the client,
[38:14] now you can't do this, right? You can't just like blindly not send any JavaScript
[38:19] to the client, because you wouldn't have the interaction. So now the problem becomes is that
[38:24] all the existing frameworks are like, well, you have to have JavaScript behavior,
[38:28] and so they would send all of it down. What I mean by all of it is,
[38:32] all of it that you see on a page, meaning including the header, the footer, the text,
[38:39] everything that you see on a page would be sent. So if you hit OK, and if you click on a network tab again,
[38:46] obviously we have network tab, okay, refresh this page. And again, notice the network tab is empty, right?
[38:54] Meaning no JavaScript got sent to the client. Now go and click on your welcome to Quick City.
[39:02] Notice that JavaScript downloaded and executed. Now hit OK on that.
[39:09] And if you click on the code that's downloaded, again, if you click on response,
[39:16] okay, notice that the only thing that downloaded is just your alert, right?
[39:25] The file you've wrote, if you look at the file you wrote is much longer, right?
[39:29] It's multiple lines of code, it has all kinds of stuff in here.
[39:32] And yet the system kind of looked at it and said, yeah, but the only thing you really need
[39:37] is just the alert and nothing else. - I'm curious just to see
[39:45] like the difference on the console. And Http, inspect.
[39:58] Then we were in network, right? - Yeah, so if you refresh here,
[40:03] you'll see tons of code download. Although-
[40:05] - Oh, wow, that is so cool. - Google search is not the best example
[40:14] because Google search is actually also one of these frameworks
[40:16] that knows how to lazy load JavaScript. But if you would go to,
[40:22] what's a good example? I don't know, go to like Target
[40:28] or one of those e-commerce stores, it doesn't matter. And so if you look at-
[40:32] - Oh. - Yeah, see all the insane JavaScript that's coming down.
[40:37] - And then is Builder.io, is that built with Quik? - Our homepage is built with Quik, yes.
[40:45] And we are working on to allow other people to do this as well.
[40:48] So Builder.io is CMS system. CMS means content management system.
[40:54] - Okay. - Yeah, if you look at view page source,
[40:58] if you look at the network, oops, I'm sorry, not view page source.
[41:02] - Wrong one. - Inspect.
[41:03] - And network. - And if you do network and yeah, refresh this.
[41:09] So there are some JavaScript loaded, but not a lot. So the thing you're really looking for is the size of it.
[41:17] Party Town is another technology we have for moving third-party code off the main thread,
[41:21] but you know, for another day. - Yeah, I'm like, that's for another time,
[41:26] but it's really cool seeing how different- - Yeah, so the thing we can do is
[41:30] if you open up a new tab and in a new tab, you also go to Builder.io,
[41:34] but this time add question mark, render equals next. But add on the URL, just say question mark,
[41:42] at the end of it, just say question mark, render equals next.
[41:47] So this is gonna render using Next.js, which is a React system.
[41:50] And now go to inspect. And now look at the network and refresh this page.
[42:00] And look at all the code that's being done. - Oh, wow.
[42:03] - Right, and now compare that to the other page you had, which just has two items in there.
[42:11] Now, of course, if you interact with the menu, right? Like if you hover over the menu,
[42:14] you will see more code downloads. - Yeah.
[42:16] - Some more code downloads as you- - Or if I scroll because we're looking at different things,
[42:20] like this is interactive. - Right, so notice the difference, right?
[42:23] The difference is in classical system, like everything is front-loaded,
[42:28] whereas here everything is, it's push versus pull, right?
[42:32] Like in the old system, like everything is pushed to the client eagerly,
[42:37] and now we're flipping it around and say, actually, let me just pull on the stuff that I need.
[42:41] And it's not the same amount of code in front of you versus behind you.
[42:45] It's like all of it in front of you, or just the tiny sliver of the things that you need
[42:51] to get the thing that the user actually asked for, right? So if I say add to the shopping cart,
[42:56] then I'm only gonna download the shopping cart code and not the commenting code, right?
[43:00] If I'm commenting on something, then I'm only gonna download the commenting code,
[43:03] but not the shopping cart code, or the menu code, or the return, or feedback code, or whatever, right?
[43:08] Like there's a gazillion things you can do on a website. - Something that I just wanna point out is it even,
[43:15] for while I'm scrolling and having to gain more content, it only loaded in 546 milliseconds,
[43:24] where like the JavaScript version was 1.3 seconds, and then Target was 3.56 seconds.
[43:34] - Yes, and now you can. - Yeah, this is something that also would
[43:38] tremendously help with SEO too, to be able to talk to marketing or small businesses.
[43:45] Now, can I ask you like a totally random thing about builder.io? - Yeah, go for it.
[43:50] - 'Cause I was looking at it. So is builder.io, is it a website builder then?
[43:55] - So this is where it kind of gets hard to explain. In a way, yes, but it's a very particular
[44:02] kind of website builder, right? Imagine you're Target.com.
[44:07] You cannot run Target.com on something like Wix. So Wix is a builder, right?
[44:15] Because there's just like so much complicated things that they need specifically to them.
[44:19] So website builders are kind of targeting, I guess, mom and pops, like small businesses
[44:28] that don't really have a lot of complicated stuff in there. Something like Target, like it probably has
[44:34] a hundred engineers working on this thing, complicated shopping cart, like all kinds of stuff.
[44:39] There's no way you can run it on a basic builder. So what builder.io is, is kind of a builder,
[44:46] but for like enterprises. And specifically the thing over there
[44:50] is that enterprises have their own technology stack and builder integrates with the technology stack
[44:56] versus something like Wix basically says, we are the technology stack and take it or leave it.
[45:01] So the difference is like, do you play with whatever the customer already has?
[45:07] Or do you say, no, no, no, this is it, right? And that's kind of the difference.
[45:12] Most website builders are like, this is it, take it or leave it.
[45:16] You cannot modify things inside of it. Whereas builder.io is really meant for enterprises
[45:25] that have complicated needs. And we can work with whatever existing technologies
[45:31] they happen to have. - That's really cool.
[45:33] I went to Verizon because I used to work for this company back in the day
[45:38] and the website would always take forever to load. So I was just curious, but it's still saying,
[45:45] you know, 729 milliseconds. - So a better thing to look at is not load.
[45:50] So load means how long it took to download all the code. The blue one, it says DOM content loaded.
[45:57] That is a better number. So that's also says 500.
[46:01] So really to look at it properly, actually let's go to builder
[46:05] because builder has it built both in Next.js and on Qwik, right?
[46:10] So this is the Qwik version and the other one over is the other one.
[46:14] So let's do this experiment. Click on a performance tab inside of the dev tools
[46:19] and click on the next, whatever, the recycling, the arrow with a pointing to itself.
[46:27] You see in the left? Yeah, that thing, yeah.
[46:31] And just let it do its thing and just wait. Okay, good.
[46:36] And then do the same exact thing on the Next.js website. So it's the same exact website.
[46:40] - And that one was under performance, yeah. - Yeah, it's under performance.
[46:43] Yeah, click that button and just let it do its thing. And okay, because these are different sites,
[46:54] they'll be scaled differently. So it's important to kind of look at it,
[47:00] but look at all the yellow stuff that you see at the top. - Yeah.
[47:05] - Or you can see the JavaScript at the bottom, the pie chart, it says 1.281 milliseconds.
[47:11] So 1.2 seconds, right? Was the JavaScript time for it to come to life.
[47:16] And all the yellow is basically JavaScript running on the client.
[47:20] And so you can see that on your modern device, we're talking about 1.5 seconds of JavaScript
[47:27] hammering your device, right? And this is a desktop device versus if you have a mobile,
[47:32] this easily could be three, four, five, even 10 times longer, right?
[47:36] Because it's a mobile device, which is not as powerful. Now go to the quick version of this.
[47:42] And you are, sorry, you need to scroll to the top because you scrolled, scroll to the top.
[47:48] Here we go, now do the button again, the performance button, recharge.
[47:53] - Yeah. - Okay, just give it a second.
[47:56] And we should see a similar kind of graph. Notice how much less yellow is in there.
[48:05] - Yeah. - Not only how much less yellow,
[48:08] but look at the summary, the scripting, it's a 67 milliseconds versus 1,280 or something.
[48:15] 1,281, right? Like huge difference.
[48:21] I'm sorry, it was 67 milliseconds versus the other one was 800, I think,
[48:27] not 1000, that thing was the overall system, I think. The was 821, sorry.
[48:31] - Yeah. - So we're talking huge difference
[48:35] of the amount of JavaScript that got downloaded to make this page interactive.
[48:41] And so what QUIC is about is not about a different way of building your site
[48:49] in terms of the user developer experience, it's about different way of delivering the content
[48:55] to the browser so that the browser doesn't choke when we first navigate to a page.
[49:00] - This is very, very cool. And I feel like now that,
[49:07] where it's gonna help, like I'm like excited about it,
[49:12] yet I'm working on formulating my questions. Because it definitely,
[49:16] I can see how this would really help with websites and those type of things on.
[49:26] Now, because I've noticed in like, if I'm doing something in HTML or CSS or JavaScript or React,
[49:36] there's slightly different variations on how to do something.
[49:40] With your experience, and I'm not sure the best way to ask this,
[49:48] is it much different from being able to do it? You said it's very comparable to React
[49:59] in the way you build something? - Yep.
[50:02] - Okay, so those who know React, it may be a bit easier for them
[50:06] to use Quik compared to those who know Express, for example. - Well, Express is a backend technology, right?
[50:17] So let's build a counter, let's say in here, and maybe if we have a few more minutes,
[50:24] and then maybe we can call it a day. 'Cause it's about an hour, right?
[50:28] - Yeah, yeah. - Okay, okay.
[50:30] So let's make a new component. So I think if you go at like line 12,
[50:35] you can type in component, and I think it should auto-complete if we got this right.
[50:41] Yeah, component dollar, see what it says, component dollar? And just hit, sorry, you clicked on the first one,
[50:47] you were supposed to click on the second one. The one with the box, the empty box, the second one.
[50:52] - Okay, oh, cool. - Oh, it generated a lot of stuff in there.
[50:57] Maybe, okay, that's okay, we'll just use this. So just call it a counter,
[51:00] so just type counter with a capital C. - Where?
[51:04] - Just start typing right now without doing anything, just type counter, capital C do.
[51:08] Okay, so no space, delete the space, perfect. Okay, so what we did is we created a new component,
[51:21] and the component is called the counter. You can see it on line 16.
[51:25] There's the counter props, we're not gonna use any props, so it's unnecessary, you know,
[51:29] the template generated all this extra things that is unnecessary for us.
[51:32] Line 17 has used store, it's red, so I think you have to click on it
[51:35] and hit Control + Spacebar, I think, to auto-complete. And call, yeah, second one.
[51:42] And yeah, sorry, you added some extra stuff, but it did import, so like,
[51:48] just make sure it says store, delete the extra. - Yeah, that's weird.
[51:51] - There we go. Did it not do an import?
[51:55] Yeah, sorry, you know what? I think it's Apple or Control and then period.
[52:03] I don't know if you have a Mac or Windows. - Yeah.
[52:08] - Apple one is in the Mac. Apple, period.
[52:12] - Yeah. - There we go.
[52:17] And add missing function to, no, no, no, not, update import, that's what you want.
[52:22] There we go, now it's in. - Yay, okay.
[52:24] - Okay, so we have a button, and the button is line 23.
[52:30] You can see that there is a button, and it has an onClick behavior,
[52:34] and the onClick behavior updates the count. And on line 24, we just print the value.
[52:43] And then the only thing we have to do is now refer to the counter from the main example, right?
[52:51] So if you go to line eight and a half. - You do, yes.
[52:57] - So in line eight and a half, we would like to say counter with a angle brackets, right?
[53:02] - So on the same line? - So eight and a half is my way of saying,
[53:08] insert a new line between eight and nine. - Okay, that's what I was thinking,
[53:11] but thank you for the clarification. Okay, I'm sorry, what did you say we were inserting?
[53:17] - Counter, so angle brackets. So open, what is it, a less than sign.
[53:23] There we go, counter, perfect, you just hit enter on it. And then backslash, so that'd be set, close it,
[53:29] and then closing angle bracket, there you go. And why is it complaining?
[53:34] Oh, because, oh, it wants a step, sorry. So in there, counter, put space, step equals one, step.
[53:42] So that's like a parameter to it, right? And I think the one has to be a number.
[53:51] So yeah, perfect, exactly, you got it. So now if you go to our quick tab, we have a counter.
[53:59] - Oh, yay. - And again, look at the bottom, there is no JavaScript.
[54:03] - Yeah. - And if you click on the counter,
[54:06] JavaScript downloads and it updates the count, right? So now notice this, you click on a counter,
[54:14] it downloads some JavaScript. And then if you click on the welcome to Quick City,
[54:18] it downloads more JavaScript, right? So instead of having a world
[54:26] where all the JavaScript is eagerly delivered to the client, and for Hello World, it's trivial, it doesn't matter,
[54:32] but for large websites, this becomes a problem. We have this other world
[54:37] where instead of delivering everything at once, we actually deliver just the bit that you need
[54:42] to perform the operation and nothing else. - Yeah, this makes sense, this makes sense.
[54:48] Now to one day, I do need to work through remaking all of these myself,
[54:56] which has been interesting to say the least, but this is really cool how it does that
[55:03] and with much less load time. And now I'm curious when you've said
[55:08] that you're explaining this to people that it can be kind of hard to explain,
[55:13] do you normally show them the network load times? Is that how you normally explain it?
[55:18] - Yeah, network load times is usually what I focus on. I think that the reason is that,
[55:22] people have preconceived notions of things. And so, if somebody already knows Angular, React and Vue,
[55:30] they have a very clear idea of what a framework is. And when you come up with it with Quick,
[55:38] the difference is not necessarily of how it looks like, but what it does underneath it.
[55:43] And my argument is that all the existing frameworks, they do it by eagerly pushing JavaScript to the client.
[55:51] And so to even suggest that you could flip this around and have this lazy is,
[55:58] I think it just doesn't fit into people's mental model. And because of that,
[56:02] people are just having trouble understanding it because they look at this thing and they go like,
[56:06] well, it looks just like React. So like, why do we need another framework
[56:09] that looks just like React, right? And what they're not really,
[56:15] or rather what I'm failing to explain, or what's not really clicking,
[56:19] is that it's not about the developer experience. It's not about what you as a developer write,
[56:25] it's about the end result of what gets fed to the browser. So Quick is a new kind of framework
[56:33] that has a developer experience similar to React, and React is loved developer experience
[56:38] by a lot of people, right? So we think we have a good developer experience there,
[56:42] but it's not about that, right? It's about the fact that when you have large websites,
[56:47] you will end up suffering the fate of too much JavaScript being downloaded eagerly.
[56:53] And what Quick aims for is to make sure that that doesn't happen, right?
[57:00] That instead of eagerly downloading JavaScript, it becomes lazy.
[57:04] And instead of like downloading all of the JavaScript, it becomes download just the bare minimum
[57:09] that you need to get the job done. So it really kind of flips
[57:14] the way code is delivered to the client. And as I said, for small websites, it makes no difference.
[57:21] It's when you get big, right, that like it makes a huge difference.
[57:25] - And I think this is gonna be a very not related, but possibly related question.
[57:31] When I worked in hosting, and it was at GoDaddy, and people were comparing load times,
[57:40] a lot of it was with WordPress, but WordPress, you wouldn't be able to use
[57:46] something like Quick because it's built with- - Yeah, because WordPress is its own way of doing things.
[57:51] - Yeah, that's what I thought, okay. - So, and essentially it competes with Quick.
[57:54] - Okay. - And not really 'cause it's a different thing, it's-
[57:56] - Yeah, yeah, yeah, yeah. - But it controls the rendering pipeline.
[57:59] Like, I guess WordPress, they could migrate on top of Quick, and then they would get these benefits.
[58:06] But like, that's such a complicated and a huge effort that nobody's gonna do that.
[58:10] - Yeah, but it makes sense. Thank you for helping close that loop for me
[58:13] because I was like, this is where most people, but I get like WordPress is like
[58:18] a more technical website builder kind of thing with that type of format.
[58:23] And Daviko is saying, "Could go headless." - Yeah, so that's Builder.io, right?
[58:34] Builder.io is a headless CMS. So WordPress is hosted CMS,
[58:38] I think that's what the term is for it, right? So CMS being content management system, right?
[58:42] Like you have some content that you wanna tell your readers and you wanna change it all the time.
[58:47] And so that whole headless thing is the, I wanna modify content without
[58:54] having engineers involved in the process 'cause like the last thing engineer wants to know is like,
[59:01] oh, you wanted 10% sale last week, but now you want a 15% sale, really?
[59:04] Like that's what my job is to change the percentages. - Got it, got it.
[59:10] Okay, cool. Well, I think that I've definitely gotten
[59:14] a lot of knowledge drop from you. Anything else that you think we should know
[59:19] before letting you go today? - No, just, I love coding
[59:25] and I think it's just the amount of time you spend on it. So like, I would like to just encourage you
[59:30] to just not give up on this and just, and the more, it's like everything else in life.
[59:36] The more you know about a particular topic, the more enjoyable it becomes, right?
[59:39] - Definitely. - That's what I always tell my kids.
[59:41] It's like, the only reason you're not enjoying this thing is because you don't know enough about it.
[59:46] - Yes, and it's horribly, on days that I don't have a guest,
[59:49] I've been doing co-work with me, like co-work with Jen, and it's really embarrassing when I'm working through it
[59:55] and people are joining and they're like, Jen, we did this instead.
[59:59] And I'm like, I'm trying. - I just don't get it.
[60:03] - There's millions of different ways of doing things and it just takes time.
[60:07] So don't give up. - Thank you.
[60:09] Thank you for that. And we hope to keep you in the loop on this journey.
[60:14] I know you have lots of shows to be on, but thank you for your time today.
[60:17] We appreciate it, Misko. - You're welcome.

