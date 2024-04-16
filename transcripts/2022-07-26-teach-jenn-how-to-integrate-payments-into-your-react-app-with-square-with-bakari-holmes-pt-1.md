---
showLink: "https://www.youtube.com/watch?v=HwpLKadAeus"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-how-to-integrate-payments-into-your-react-app-with-square-with-bakari-holmes-pt-1"
title: "Teach Jenn How to Integrate Payments into your React App with Square with Bakari Holmes Pt 1"
publishDate: "2022-07-26"
coverImage: "https://i.ytimg.com/vi/HwpLKadAeus/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome back to Teach Gen Tech.
[00:06] It has been a hot minute. I had a guest I think last Monday
[00:11] and doing co-working with Jen by myself was just really awkward, especially because I've had to work on
[00:18] podcast stuff that I didn't do the last few days. Thank you everyone for your patience.
[00:24] I'm very excited because today, we have Bacari on, not Bacardi, Bacari.
[00:30] >> That's right. >> Which is just a really cool name, by the way.
[00:33] >> Yes. Thank you. >> Do you know the origin of the name or was it
[00:36] just like something your mom was like, "That's cool." >> Yeah, they were reading the ingredients on the back of a bottle.
[00:44] Bacari. No, seriously, it's an African name. It is Swahili.
[00:52] My full name is actually Bacari Ayinde Holmes. >> Wow. Okay.
[00:58] >> Yeah. I think Ayinde is Yoruba, and Bacari is Kiswahili,
[01:03] and it means of noble promise. Yes. That's where that comes from.
[01:10] Ayinde means praise. >> A noble promise praise. I dig it.
[01:18] >> It doesn't really go together. >> It can today.
[01:24] No, I'm just kidding. I'm just saying that because it's your full name. Because it's your full name,
[01:29] but well, thank you for letting me go off on that total random side note. Please introduce yourself and what you're teaching me today.
[01:39] >> As you said, I'm Bacari Holmes. I am a full-stack front-end leading developer.
[01:47] I'm also a musician, content creator, physicist, teacher, dad, a whole bunch of stuff.
[01:55] Today, we are going to be going over integrating Square. You guys have seen Square.
[02:06] >> It's the payment thing, right? >> Yes.
[02:09] >> I feel like I know what Square is because I've helped a friend on a coffee truck before and she had the little app.
[02:18] But if you had to explain Square to somebody who had no idea what it is, how would you explain it?
[02:26] >> I would say Square is a whole bunch of things, but what we're going to be dealing with today is
[02:32] software that makes it very easy for you to take payments on the go. Let's say if you had a website,
[02:40] say me, say if you're a musician and you wanted to sell merch to people, and you wanted to add that ability to take payments for that merch,
[02:52] Square offers some APIs that make it pretty simple to add that. I have today a way of doing that,
[03:04] that allows you to build it without having to use Python, Django, and then React,
[03:12] and then something else for your back end. It's all one thing, one framework.
[03:19] We're going to do it in one framework. >> I feel like I am going to ask you a difficult question as soon as we go.
[03:29] When I worked at Stoplight and I was learning from the engineers about more, what is an API and what Stoplight specifically
[03:39] does to get ready for their learning services stuff, I was asking everyone,
[03:44] what is an SDK and the difference between an API and an SDK? So many individuals had different answers to the question.
[03:53] >> I'm probably going to have a different answer. >> Yeah. I'm curious, how would you explain what an SDK is,
[03:59] by itself, and then how would you compare the two? >> An API can be something as simple as you have an endpoint,
[04:09] which basically an endpoint looks like a URL. It has this address.
[04:14] When you go to this address, this address typically does one thing.
[04:18] It returns you some JSON, JavaScript Object Notation, and this JSON has a response.
[04:26] You say, "Hey, I want to know how many people are a part of this band." Then an API returns and says,
[04:36] "Here's a list of the people in this band. It's this person, this person, this person, this person."
[04:41] Or you could say, "Hey," there's another endpoint that says, "Hey, who's the drummer?"
[04:46] You just add, so that's an API. What an SDK does,
[04:53] an SDK is meant to allow you to build an app or integrate some technology into your existing app quicker.
[05:05] It's called a software development kit. You can think of it like a tool belt.
[05:11] You can add these tools to your existing skill set or to your existing code.
[05:17] In this case, we are going to take some React components that are built on top of Square's SDK,
[05:28] and all we have to do is add these components to our project and we can add payments with a little bit more code.
[05:36] Then we don't have to leave JavaScript at all. I love times apps like that,
[05:41] that you don't have to leave JavaScript. >> That is very cool. I know when I was working with Ramon last week,
[05:50] and he's been on the show twice, we actually worked on not only building an API,
[05:56] and I believe we were using Express, but then we also used Mongo and MongoDB to build the database,
[06:05] and we did it as kind words. If I add comments that people have given me,
[06:11] so that way, I have a happiness spurt. That way, if I'm feeling down,
[06:18] I can look at them all, where it would actually start listing them out as the endpoints.
[06:23] That was really cool being able to see that, and after being in the API world for so long,
[06:30] actually see how a bare basic API can be built. Because I was like, "Oh,
[06:35] it's not as hard as I once imagined." >> No. An API can be one endpoint.
[06:43] It can be a whole bunch of endpoints together, and then you call that an API.
[06:48] An API is really wherever you want to draw the line. There are huge complex APIs that deal with cybersecurity.
[06:58] There's APIs that deal with traffic to maybe a group of websites. There's APIs that you call them and they just return,
[07:08] like I was talking about, you call them and they just return one thing. At its most basic level,
[07:13] I like to explain an API that way. I feel like those more complicated APIs are
[07:18] just a more complicated version of something that's very simple. >> That's something that Mishko was talking about when he came on to go over
[07:27] Quick was especially and he told me that he was telling his kids this, of you just learn the basics and
[07:36] all these fundamental things that are all pretty basic and then build upon them. I was like, "When you think about it like that,
[07:44] it's not as daunting getting into the coding and tech world. It's just looking big picture like wanting to understand
[07:53] why we need to scale and create governance in APIs. It's very big picture, it's very needed,
[08:00] yet daunting at this level. >> Right.
[08:04] >> Thank you. I appreciate the explanation. >> Yeah, no problem. Let's jump into my little deck that I have here.
[08:13] If you want to do that right now, unless you have a comment or anything.
[08:17] >> No, I'm learning the clicky-clicky on StreamYard. Got to learn how to use all that.
[08:23] I know how to use it, but I never am doing it on time.
[08:27] >> Yeah. This is [MUSIC] >> Sorry, I always do sound effects and stuff.
[08:35] >> Yay. >> I think that's fireworks.
[08:42] >> Okay. >> That one reminds me of Star Wars.
[08:48] >> Don't get me started. >> But no, the old-school Star Wars,
[08:55] not like the ones that have been made in the last 20 years, but the old-school ones.
[09:00] >> Yeah, definitely. >> Yeah, we are going to go,
[09:05] and I didn't mention, but we are going to use Next.js. That is a React full-stack framework.
[09:11] It is owned by Vercel. I don't know if it's made by Vercel,
[09:15] but it's owned by Vercel. Someone from Vercel can probably correct me on that.
[09:22] But we're going to just build a demo. This is really going to be,
[09:25] it's not going to look pretty, but it's going to be functional.
[09:29] Again, it's going to be the simplest thing we can build in Next.js that has the square integrated into it.
[09:37] Then from there, later on, you can build on it, you can add to it.
[09:43] Then we'll have payments attached to it. >> That's really cool. I'm almost starting to wonder
[09:48] because Anthony taught me how to, and it was very much front-end of
[09:54] how to create a React app with Vite and Vercel, and then Ramon taught me how to do the API with,
[10:04] as I said, with Express.js and Mongo. Then learning this, I'm like,
[10:13] eventually I'm going to get to the point where I can mush them all together.
[10:16] >> Yeah. There's going to be some overlap with, I can't remember the name of the gentleman that was
[10:23] talking about quick. >> Mishko.
[10:27] >> Mishko. There's going to be some overlap with that and the API and the React.
[10:32] This actually, in some ways, is going to bring those things together, hopefully,
[10:36] because we are going to be building a full stack by just going createNextStack.
[10:44] I'm getting ahead of myself, but I'm really excited because Next allows you,
[10:49] it looks like it's front-end code, but it's actually full stack.
[10:52] There's just a whole bunch of stuff that's abstracted away from you.
[10:56] In other words, it's there, but the way that it's built,
[11:01] it's a really nice experience and all you have to do is type some JavaScript,
[11:06] and then you run your server and boom, everything is there. There's a server, we can build an API.
[11:14] We're going to be doing that. Here's the situation. My parents went to wait on a week's vacation.
[11:21] The situation is, and I think I already explained this.
[11:28] I'm thinking of a use case, and the use case for me is I'm a musician.
[11:33] I actually have a band page, and on that band page,
[11:36] I can't sell merch, but I want to be able to sell merch,
[11:39] and I want to be able to take payments for that. In my mind, I'm like, "Okay,
[11:44] I really like JavaScript LAN. I like staying in JavaScript LAN."
[11:48] What is the least number of frameworks? Because we could use an endless number of frameworks.
[11:53] We could use something for CSS, we could use something for HTML,
[11:56] we could use something for our front-end JavaScript, we could use something for our middleware like
[12:01] Express, our middle layer, and then we could use like Node,
[12:07] so we can continue to multiply. We want to do testing,
[12:12] we can introduce frameworks for testing. But what's the least number of frameworks
[12:17] needed to build a square app in JS? >> When this question is appropriate,
[12:23] I'm not sure when, I'm curious what would be the perks of doing this
[12:31] compared to something that's a bit less technical of like an iframe?
[12:38] >> An iframe? >> Granted, that is HTML,
[12:46] and iframes don't always work in general, and I'm going to Google it because I know what an iframe is,
[12:54] and I'll work on describing it, but then I'm going to Google it and see if it tells me what it is.
[13:00] Actually, iframe is where it can take a portion of an app or a website and you can embed it into another website using HTML,
[13:10] meaning that it is just a frame of a selected area. >> Right, so what I would guess,
[13:20] and I'm not the expert on this, actually, the Square folks are,
[13:24] and I don't work for Square. >> Yeah, maybe someday, come on Square.
[13:29] >> Maybe, we'll see. Are you guys watching? Did you hear that? >> We'll tag them. We'll tag them and be like, "Yo, Square."
[13:38] >> Yo, Square, what up, y'all? >> Square block. In case you don't know,
[13:45] I am looking for a job right now. That was the plug.
[13:50] I can't even remember what I was saying. >> The difference between an iframe,
[13:55] having it as an iframe and. >> When we finish, we're going to have an app,
[14:01] and what Next.js is going to do, it's actually going to create HTML,
[14:08] it's going to add event listeners, it's going to have all of the things
[14:12] that a typical website would have. We could take an iframe from that website,
[14:20] we've built a portion of it, and we could display it somewhere.
[14:25] For instance, it could be like a payment box, and we could use that iframe somewhere else.
[14:30] Yes, we could use an iframe, but you need the HTML.
[14:35] Either way, you're going to need the HTML, and then from that HTML,
[14:39] you can take that frame and put it somewhere or display it. >> It's not going to necessarily
[14:44] do exactly what we want it to do. We're building it into the site with Next.
[14:50] Yeah, we're on Next right now. Sorry, I was getting my frameworks all funky.
[14:55] It's going to be able to display what we want it to display. I'm thinking it's probably going to be more reliable.
[15:02] >> I'm not sure what. I haven't worked with iframes a ton.
[15:08] I've worked with them a little bit, but if I were to venture a guess,
[15:14] then I would think that iframes are a little bit more limited in their functionality and what they're able to do.
[15:23] Now, I'm not trying to hate on Apple. I'm just saying that particular technology
[15:28] is made for a specific use case. Whereas Next is made for a wide,
[15:37] general-purpose, full-stack programming purpose. Anything you want to build, essentially, that's full-stack.
[15:48] >> I dig it. >> Yeah. Anyways, the answer is one.
[15:55] Do we have a clap thing? >> Yeah.
[15:58] >> All right. We're doing ghetto. We clap on ourselves. If you use Next.js, in my opinion,
[16:07] building this way will lead to a better developer experience because developers that already know Next or know React,
[16:14] which there's a lot, they'll be able to quickly spin this up. Again, it supports full-stack React,
[16:23] optimizations, easy API design. We actually are going to build an API today.
[16:28] It's only going to take 20 lines of code, but we'll build an endpoint in Next in a folder.
[16:36] It's so cool. Oh my gosh, I'm so excited. >> Yeah.
[16:39] >> It's really easy to spin up. It's wildly popular, so that's why I'm doing it this way.
[16:45] This is just the justification for why it's being built this way.
[16:50] Between the Square API, which we just talked about,
[16:54] between the Square Web Payments SDK, so within all of the Square APIs,
[17:00] there's APIs that are specific for web payments. That's taking payments on the web.
[17:06] There's like mobile and there's all these different other ones. Actually, I don't know them all.
[17:13] >> You'll learn them all. It'll be good. >> Yeah, I will. I've been poking around their docs, actually.
[17:19] I've just been hanging out in the web payments. >> I dig it because you can tell you're passionate about it.
[17:27] Just as like a side point, because that is something that I really love about this show,
[17:32] is people always come on to talk about what they're passionate about.
[17:36] Thank you and please continue. >> Within those Square APIs,
[17:46] there is the Web Payments APIs, and they took those Web Payments APIs
[17:54] and wrapped them up in a Web Payments SDK. If you use this Web Payments SDK,
[18:00] you can, again, more easily build an app. You can make the Square API calls and all of that stuff.
[18:09] You can have that functionality that Square affords you. We want to use React.
[18:15] We want to use the component-based architecture that React has, and also the API endpoints.
[18:24] Between all of that, there's lots of complexity.
[18:27] Let's try to simplify this down so we have happy campers like that. >> Yes, they do look very happy.
[18:38] >> Yes, they do. These are actual satisfied customers. Yes, they are. What I have here is
[18:46] a picture of Next.js and it's all one code base. Then in your Next.js are different folders.
[18:59] What we're going to do is a group of folks. I think they are international.
[19:08] A group of folks actually took the Square SDK and they created what's called a React wrapper.
[19:15] Essentially, they took the Square SDK and they took that logic and they stuck them in different components.
[19:20] Then they put them on GitHub and they said, "Hey, world, use these."
[19:23] It makes it even easier because now all you have to do is import those components to your Next project and then you can use
[19:31] those components to build and add payments to an app. Essentially, all you're doing is once you have installed it,
[19:42] the wrapper and the SDK, then you can just import it.
[19:49] Now we're down to just React Square Web Payments SDK, which if you Google that,
[20:00] you'll come up with the GitHub and we're going to actually add it at our CLI, our command line.
[20:09] Next.js, we just have those two things. We'll stay in a React context.
[20:20] You can quickly integrate. >> Okay.
[20:25] >> There's so many nerdy references in here, like one framework can rule them all.
[20:30] >> I mean, see, I'm so new that I didn't even know. >> That, I believe, is Lord of the Rings.
[20:41] >> Oh, okay. >> One ring to rule them all.
[20:44] >> Oh, yeah, that does make sense. I'm actually been working through watching all of them,
[20:48] re-watching them in the last month, so I probably should have known that one.
[20:52] >> Yes. We will get off on so many tangents. In React context, there's actually a feature in React called context,
[21:06] and I was using the word context, so that was really nerdy, double-speak.
[21:12] >> I dig it. >> There's probably a couple of React developers going, "Oh, I got it."
[21:19] >> I'm glad they are because I'm learning all of this. I get excited when I get one reference,
[21:28] and I'm like, all the other ones got over my head, but I got that one.
[21:32] >> This slide here, I like to go over this because this is going to try to solidify.
[21:39] It's just another visual way to explain the architecture of what we're actually building.
[21:45] Because we're going to type a few lines and it's going to be like, boom, it's already there. Sometimes it can feel like,
[21:51] well, how do we do that? There is the next JS.
[21:59] We are going to npm install that SDK, React Square Web Pay payments SDK,
[22:08] and also the Web Payments SDK. We're going to npm install that.
[22:12] Within that, there are a couple of components. There's ACH, which is like,
[22:19] I think direct debit, and then credit card pay. >> Yeah.
[22:23] >> There's those two types that we're going to use. >> Okay.
[22:29] >> Add to our project. Some of the benefits specifically for Next.js,
[22:38] it allows for, and I'm not going to go a lot into this because I know you already had someone come on and talk about this,
[22:44] but server-side rendering and static site generation. It affords you that out of the box.
[22:53] Once you do create Next app, you've already got it. Pre-fetching. Pre-fetching allows you,
[23:02] if you have a link or a route or if you have a fetch call, sometimes it can actually get that data before you make that call.
[23:13] Then when you make that call, the response comes really quickly.
[23:17] >> Okay. >> It improves your, again,
[23:23] the purpose is to optimize or to speed up how long it takes for you to spin up this app,
[23:33] or to render it on the screen, to render it or paint it,
[23:37] where's the first paint or the second paint on your browser. Optimizations like code splitting,
[23:44] I'm going to slow down with this. Code splitting is you take your JavaScript and essentially,
[23:49] it's divided up into modules or pieces, and instead of loading it all at once,
[23:55] it's loaded in chunks. >> That's like what Quick does,
[24:01] because Quick only loads it when you need it, instead of, for example,
[24:07] loading an entire page at the beginning, it makes it so that way it does render a lot quicker.
[24:12] >> It is that, what you just said. You got it. >> Yay, learning.
[24:18] >> Gold stars. You blew up the Death Star. I can just keep going here.
[24:26] >> I dig it. >> Then tree shaking.
[24:30] Tree shaking essentially looks at your code and sees if there are any dead pieces of code that are no longer needed,
[24:38] and then removes them. Then again, if a reload needs to happen, it happens faster.
[24:47] >> Real quick, I'm just going to say, "Hi, Rizel." >> Oh, Rizel's here. What's up, girl?
[24:55] >> For anyone watching, you have to follow Rizel.
[25:00] She is just one of the coolest humans in the world. >> Yeah, that is true.
[25:05] >> I know that I follow most people on Twitter. She is the GitHub Dev Advocate,
[25:12] so follow her on GitHub too. Seriously, just a legit human.
[25:18] >> That is right. She's part of our RenderATL crew.
[25:22] >> Yes, and I like that I keep hearing about it without meaning to. I just keep meeting people that I've gone to about it.
[25:29] I'm like, "Yes, that's cool." >> That's right.
[25:33] Webpack. I'm not going to go deep into Webpack, but it's essentially, she said,
[25:46] "Yeah, you're in your ATL crew, shout out." Shout it out. Webpack is a system that allows you to take your modules,
[25:55] and your dependencies, and all these different things, and bundle them up into some nice JavaScript,
[26:01] HTML, and CSS. That Webpack system is built-in.
[26:06] I believe it's Webpack 5 at this point that Next.js is using. All of these features are all built-in to Next.js.
[26:13] You see what I'm saying? >> Yeah, this is cool.
[26:16] >> Yeah. Next.js, you can entirely build this essentially in React components.
[26:22] >> Okay. >> You don't need to fool around with HTML.
[26:26] I think there's a very small amount of HTML, but it's essentially a 100 percent React components almost.
[26:35] Then when you're building a React app, you use create React app.
[26:41] With Next, you use create Next app. Similar to your base-level scaffolding for create React,
[26:51] you're going to build base-level scaffolding for Next. We're going to do that on the command line.
[26:58] Let me see if we're going to do that now. Let me see what was. Yes, we are.
[27:03] What I want you to do is go ahead and go to your command line.
[27:11] >> All right. I don't think that I can keep both of our screens up, so I'm going to start sharing my screen,
[27:18] and then you can tell me what to type. >> Okay. Sounds good.
[27:22] >> Voila. I'm going to make this giant. Wrong page. Here we go.
[27:28] That one's back to normal, and this one is so much bigger.
[27:32] Yay. Then I don't believe I've installed Next yet. I think I have React, Express.
[27:45] >> Yeah. >> Yes. Then let me go to shoot.
[27:52] This is when it's not a good thing that I haven't done it in a week, because I'm like, "Wait, what do I do?"
[27:58] I need to go to. >> I was just going to say you can do LS to see what's in your directory.
[28:07] >> Thank you. >> It's just list.
[28:11] I don't know where you have your coding projects. Rizal could probably school us on how to organize
[28:21] your folders using some fancy Git thing. >> Probably. I'm not even going to lie.
[28:29] >> So much to learn. I'm in the proper folder now. >> Got it. What you're going to do is you're going to npm install,
[28:39] so npm install, and then dash, dash, save. >> Dash, dash, save.
[28:48] >> Yeah. Then it's going to be React. Actually, you know what? I'm going to send this to you.
[28:54] I can put it in. I can't put it in the comments. >> You should be able to put it in the comments, I would think.
[29:01] >> I can put it in the private chat, but there's no. >> All right. Well, it'll show up on the screen, so they'll see it.
[29:07] >> Okay. So it is react-square. Let me make sure I spell this right.
[29:16] React-web-payments-sdk, then I'm just going to type the whole thing, so we're not going back and forth.
[29:32] React-web-sdk, then next-transfile-modules, and then square. All right. So that whole thing.
[29:54] >> All right. Give me a second. >> Oh, geez. Okay. Then it's the same thing, right?
[30:04] >> Yeah. It's going to go and do the magical NPM install. So this is the magic.
[30:12] We're taking that third-party React library that was created, that has the Square SDK built into it, into the components.
[30:30] Then we need Square SDK, Web SDK, we need the next-transfile-modules,
[30:35] and we need overall square. So we can do certain functions.
[30:39] >> Got it. >> Let me see. I can't really see, but did it?
[30:43] >> Yeah. Let me make it bigger. I have to wear my glasses for these live streams,
[30:51] because I'm like, "I can't see." >> Yeah. All right.
[30:55] >> Awesome. >> One package is looking for funding.
[30:59] Run NPM fund for details. >> Yeah. So you could actually do that.
[31:04] But some of these are like open-source projects that they need money to run.
[31:12] >> Yeah. This is telling us to go to GitHub to find it. >> Yeah. Again, Rizal knows all about open-source.
[31:21] Shout-out to OpenSauce. Is it OpenSauce or OpenSauce?
[31:25] That is BDougie has a great open-source. BDougie is at GitHub as well.
[31:32] >> Nice. >> Just a little plug there.
[31:34] See? Just plug in my friends here. >> That's what we have these platforms for,
[31:40] is because we got to shout out other people. >> Yeah.
[31:46] >> That's what community is about. >> Yeah, that's right. Now we have
[31:50] those packages and what we want to do is, I want you to actually now open up your VSCode.
[32:02] >> Okay. I'm going to see if it does it. Is it, what is it dot code to normally open up?
[32:09] >> Code space dot. >> I don't think it'll do it.
[32:13] Yeah. I actually got the instructions how to update that in the shell commands.
[32:22] I just haven't done it yet. >> Oh, okay.
[32:26] >> I basically put in this, and then file, new text file.
[32:34] We'll just do this and then leave it, shift command P, and voila.
[32:46] >> It just takes like seven more steps. >> Yeah. We need to generate
[32:52] the next scaffolding, so from your shout out to open source, yeah.
[33:04] We just need to do create dash next dash app. >> Is there any spaces in there?
[33:17] >> Nope. It's all one. Oh, I forgot. >> Oh, wait a minute.
[33:22] >> I might have to install next. >> I think so, yeah.
[33:26] Let's go to just Next.js. Look, I'm Googling it right now.
[33:31] Actually, why don't you Google it on your screen so people can see it. >> I was going to say, let me bring this over and make this bigger.
[33:38] My profile because Rizal told me to set it up, so it did. Okay. We want to install Next.js.
[33:52] >> There you go. >> Get it started with Next.js.
[33:55] >> Get it started. There it is. >> Automatic setup, create app Next.js.
[34:06] It would be? >> Oh, I forgot. It had to have NPX in front of it.
[34:14] >> What is the difference between NPX and NPM? >> I believe NPX takes
[34:22] something if you don't have something and installs it for you. I had to look that up,
[34:28] but I'm pretty sure NPX is like a dynamic thing, and NPM takes the latest version and then installs it.
[34:36] >> What is your project? Oh, that's nice.
[34:44] >> But it does. Oh, I can't use capital letters. [inaudible]
[34:53] >> Car is dope. This is sometimes true.
[34:58] >> There we go. See, I'm remembering how to do this from when Ramon created a project name
[35:06] and you had to go through each of the steps on Express. See if I remember all of them.
[35:13] >> This has a bunch of like if you can see all of the stuff, React DOM, React scheduler,
[35:21] source map, TS library, Next environment. You see all those direct dependencies?
[35:29] All of those are built into Next. V8 Compile Cache.
[35:33] Yeah, it's a whole bunch of cool stuff. >> We can move this one back over.
[35:37] So we have this. Now I should be able to do code space dot.
[35:43] It has it right here. I guess that works. >> There it is.
[35:54] >> Yeah. >> All right. There's a few places we want to look.
[35:59] Go to Pages, please, and expand that. So there's API there.
[36:05] >> Okay. >> We're going to use that later.
[36:08] But if you can expand API and Hello.js, I want you to change that to pay.js.
[36:17] You change the name of that. Oh, sorry, P-A-Y. >> Oh, I heard hey and I was like,
[36:26] all right, let's do hey. I like it. >> Actually, we could do hey.
[36:31] >> But yeah, let's do pay. >> Okay. Then we're going to need index.js, of course.
[36:39] We're going to need something called next.config.js, which is down a bit.
[36:45] >> This one? >> Yeah, right there. Let me pull out my,
[36:53] this is going to be a bit. Can I show you my screen?
[37:02] >> Yeah, sure. >> I'm going to switch back over.
[37:08] >> Can you make yours bigger too, please? >> Yes, I can. I just saw it on the screen.
[37:15] I was like, "Hey, there it is." >> Thank you.
[37:17] >> Okay. You're going to do a couple of things. One, you're going to create a variable called withTM.
[37:29] It's going to be require, which is there's import and require,
[37:36] which do really similar things and they have some small differences in import versus require.
[37:47] Typically, require is used on the back-end and import is used on the front-end.
[37:51] That's not a good way to explain it, but that's typically where they're used because of
[37:56] the Node.js environment versus the browser environment. Whether the browser can recognize
[38:02] require and whether it can recognize index.js, some newer browsers might be able to
[38:08] recognize that now, so that might not be true. But I think typically that's where I've seen require.
[38:15] You're going to put in there, you're going to put three things.
[38:19] You're going to put this next transpile modules. Remember, we NPM installed that?
[38:24] What we want to do is in our code, we want to actually import that in.
[38:31] >> Yeah, we did that with having to use Express like we had to tell it to use Express.
[38:37] >> Yeah. This next transpile modules just has to do with the way that next translates
[38:44] one version of JavaScript into another version of JavaScript. Like say, if a browser can only run ES5,
[38:51] which is the 2014 or 2013 version of JavaScript. It can translate different versions
[39:02] of JavaScript in the next environment. It can also translate,
[39:09] like say, something's just a file in a folder, it can actually translate it to actually be a full endpoint.
[39:15] It does a lot of that work for us. Then also we want square web SDK.
[39:21] >> Okay. >> Here, at square dash web SDK and then comma.
[39:27] We want this in require and then open paren, not bracket, open paren,
[39:35] and then open quote, next dash transpile dash modules.
[39:41] >> Okay. >> Then close quote and close paren.
[39:48] >> Can you do me a favor? It's not at the beginning of the line, is it?
[39:56] >> This is line 2. This is just a comment. >> Yeah. Okay. It's const.
[40:01] That's what I couldn't see. >> Oh, yeah.
[40:03] >> I wanted to take a look. >> This is just a constant.
[40:06] We're not going to be reassigning with TM to anything else, so we can use const.
[40:12] Let me see here. Now, see here.
[40:18] Okay. Here, I just sent that line to you. >> Now, I should be looking at that,
[40:37] but now I'm just seeing if I can actually type it right. >> Oh, okay. You get the constant with TM?
[40:46] >> Yes. >> Okay.
[40:48] >> Well, go back to the very beginning. Let me just make sure with TM.
[40:53] Okay. That's where? >> Yeah. TM is capitalized.
[40:57] >> Cool. The reason I want to do this is just to ensure that I'm starting to remember all of the steps and
[41:08] not skipping over something because I'm not used to typing it. I've been really bad at commas.
[41:17] Commas have not been my friends. >> Commas are very important.
[41:22] >> Yes. >> In JavaScript, if you have an object,
[41:25] if it doesn't see a comma, it's going to either freak out and yell at you.
[41:30] If you have a linter, you know what a linter is?
[41:36] >> Yes. >> If you have a linter,
[41:39] the linter is going to scream at you, or if you have some build system that uses a linter to check,
[41:44] it will yell at you as well from your command line, or your code will just break and it won't work, which will be very sad.
[41:55] >> Can you scroll the rest of the way? >> Yes, I can. Which over here?
[41:59] Yeah, -xk and close record. Well, I think I'm close.
[42:11] I might have something a little different. Let's see. Where am I getting that I have a?
[42:22] That's where. Okay. >> I just realized we also didn't set you up
[42:27] a square developer account. >> Yeah, we got to do that too?
[42:34] >> Yes. >> All right. I will share my screen and get to that point.
[42:40] >> Yeah, these were things I had set up before. >> Can you just tell your linter to fix it automatically?
[42:53] That's actually a really good question. >> There are, so can I address this one?
[43:00] >> Yeah, for sure. This is Anthony. He's the one who helped me on the React app with Vite and Vercel.
[43:10] >> Yes. To a certain extent, the linters they're starting to make are getting really,
[43:17] really smart and if you're making an object and you start to make an object, it'll actually put the structure there for you.
[43:28] There's things like Prettier, there's certain code editing and
[43:35] beautification tools that will actually help you write code. It'll make it easier. It's not going to, well, actually,
[43:44] I don't know, some of the things that GitHub is creating, maybe it's going to replace us all together.
[43:49] We won't need coding. I don't know. Maybe Rizal can answer that.
[43:55] But yes, to some extent, yes, your linter can fix things automatically or it can give
[44:02] you suggestions about how to fix what you just wrote. It's maybe saying, "Hey,
[44:07] your comma is missing," or "Did you mean this?" Suggestions.
[44:12] >> His reply. >> He said, "I should use a linter, but I don't."
[44:16] "My code is already beautiful, how dare you?" >> That's funny.
[44:23] >> I got the account set up. I'm just making sure it's not going to make me verify my account.
[44:29] >> Yeah. We are going to need a sandbox. We're going to need sandbox values,
[44:34] so go ahead and create an application. >> Yay. Do I name the application same as what I named the files?
[44:44] >> Sure. >> Because it's Beccaria's Dope,
[44:50] of course, you can name it that. >> Yeah.
[44:53] >> I need a pat on the back as much as I can get it these days. >> Anthony, you got to be back on the show because I've
[45:01] started naming it after my guests and it makes it a lot easier to remember. Anthony, you have to come back on the show. Just saying.
[45:11] >> Yes. Especially if he writes beautiful code that doesn't need a linter. >> Yes.
[45:16] >> He should be back on the show. He should replace me right now.
[45:19] >> Well, no, because I definitely want him back on the show when we get into Web 3. In fact, he was like one of the people that I first met and he was like,
[45:30] "Don't even pay attention to Web 3 or any of that yet. Just no." >> Right.
[45:36] >> No, I'm not just calling it Tuesday. No.
[45:41] >> That's funny. >> It is an improvement.
[45:44] >> I didn't know what to do. You are like my second guest ever.
[45:47] >> He's leveling up. >> All right. I got my Sandbox account.
[45:53] >> Okay. Sandbox test account. What does it say there on the screen about Sandbox?
[46:01] That's what we want to use. >> Okay. Default test account, open.
[46:06] >> What does that add? >> Add another Sandbox account, I think.
[46:12] >> What is that? It said, "Sandbox seller account show you." It just says, "Learn more." Let's click "Add."
[46:20] Account name. You can name it whatever you want. >> Okay. Whoa. Automatically create authorizations.
[46:42] I guess that's a yes. >> Yes. We're going to need an authorization code.
[46:47] >> All right. >> Now, the reason why we're doing all of this is we don't want to put
[46:52] a real credit card in there and real names and real addresses that have to be authenticated by Square.
[46:58] Because they're a serious company. If you say this is a credit card and it's like
[47:03] the real production version of the API, it's going to charge the credit card.
[47:07] >> Yeah. Don't want to do that. >> We don't want to do that.
[47:10] We don't want to be putting that information up on the screen. >> Yeah. Anthony has taught me lots about not using
[47:19] Twitter because a lot of times it'll keep your DMs open or your calendar or anything.
[47:24] I'm getting better at that stuff. I like the call-out.
[47:28] >> Yeah. >> Open Square SDK learning.
[47:34] >> There's three values we're going to need. >> Something went wrong with your app arrangement.
[47:48] You can continue to use these apps as normal or refresh and try again. >> We'll do that.
[47:58] >> We'll do that. >> You try to refresh?
[48:00] >> No. Sure. >> Dammit.
[48:02] >> All right. Let's go to home. I think that's home. Then let's go to account and settings.
[48:27] There's nothing there. Let's go back to the hamburger menu. Here we go. Let's go to payments.
[48:44] Down there, Payments, Voices, Virtual Terminal, Subscriptions.
[48:51] Somewhere there is, oh, you know what? I can do it on my account.
[48:59] >> What are we looking for? >> We're looking for the place where the authorization token is.
[49:08] There's also an app ID and a location ID that should have been generated for you.
[49:15] >> Square Developer Dashboard. >> Do you have a sign-in?
[49:30] >> App integrations, maybe. >> Try that.
[49:37] >> Sandbox. Let's say that. There's permissions.
[49:46] >> I think it's the same thing. >> Actually, you know what? There's a dashboard.
[49:51] Let me see here. I'm going to sign into mine. >> Now, I'm just honestly clicking through
[50:03] everything to see if I can find it. Because as again,
[50:09] Ramon and Anthony and so many keeps telling me to actually do like read the documentation.
[50:19] I'm like, "No, I just want to click through it. I want to find it myself."
[50:22] Where it takes like half the time to do that. Anthony just said,
[50:27] "This is a good way for me to learn getting an API key, try and navigate docs is like
[50:32] half of what you do with services like this." >> Yeah.
[50:36] >> I will say, I do want to say that I have set up API keys with Zapier and Monday.com,
[50:45] and I got really excited being able to do it. >> Yeah.
[50:49] >> It's a very silly one, but I was very excited. >> We're going to get it. I just sent you a URL.
[50:58] That should help speed up. I'll put it in the private chat.
[51:06] It's going to ask you for your login likely. Whoa, page not found. That's not good.
[51:17] >> Developer dashboard. >> We were just there.
[51:30] >> Let's open your application. >> This one? The one up above?
[51:35] >> Yeah, the one you created. There we go. I think that's what we need right there.
[51:43] Macari is dope, and if you scroll down. >> Yay.
[51:49] >> Application ID, you're going to need that in our app. Then the access token we're going to need.
[51:57] Then there's also a location ID, which if you on the left-hand side,
[52:03] yeah, you see where it says locations? Yeah. You see that location ID?
[52:12] Let's have you copy those three values. You can put it on a notepad or however you organize your information.
[52:24] >> A lot of times, and I don't know if this is the best practice, but especially if I know that I'm going to be using them somewhere in a document,
[52:32] I like to put them up at the top so that way I can refine them again. I mean, I could actually start using a notepad.
[52:44] >> Yes. Just a note here for security purposes. Things like your location ID and things like this,
[52:57] like your authentication token, those aren't things that you want to leave in your code base.
[53:03] >> Got it. >> Even if you're on a live stream,
[53:06] that's typically not a good practice to display those things. Those are the things you want to keep hidden.
[53:16] I understand these are sandbox values, and this is for the purpose of learning,
[53:21] but I'm just saying if this were like a- >> Yeah. I've known that in the past,
[53:27] but I'm just curious, what could someone do with the location or an API key if they don't? Anthony said we can cover it.
[53:43] We're getting results, yeah, it's bad. You would get in trouble, you put those in a config file,
[53:52] and then you use get ignore. It's not very hard to set up,
[53:58] but once you do it once. >> Yeah.
[54:03] >> If we set up dot env, yeah. I don't know what that is, but cool.
[54:10] >> Then environment, yes. They're talking about environment variables,
[54:13] which actually one of those is going to be an environment variable or what's
[54:18] going to be the value for an environment variable. >> Yeah.
[54:21] >> Which actually is on this page. >> Sweet.
[54:25] >> But we needed the values first. >> Let me get my actual notepad,
[54:32] which I'm just going to move over. It was my cover letter to someone for a job.
[54:40] >> There you go. >> Exciting news for a hot minute that anybody wanted to take screenshots.
[54:50] >> You got that first line, right? >> Yeah. I'm getting the other one for my credentials.
[55:00] >> Yes. You can see that Square really takes the access token seriously,
[55:09] because they don't even show it to you. >> Yeah.
[55:12] >> They just have a bunch of dots. I think you can just copy it and paste it somewhere.
[55:19] Just in case I moved it off the screen. Get in the good habit. All right, cool.
[55:27] I got all of that set up. >> For now, we are going to continue with the config file.
[55:37] Can you show my screen, please? >> For sure.
[55:45] >> I'll show you slowly. >> Yay.
[55:49] >> All right. The next thing we're going to do is, now, look, I have this little note.
[55:54] It's like what I was just saying. I just didn't follow my own advice.
[55:58] I put it in a config file, but I didn't get ignore it.
[56:02] Please don't shoot the messenger. But you're going to do module.exports,
[56:10] and then equals withTM, and then open parens and open curly brace.
[56:18] You're essentially going to create an object inside of withTM, and you're going to wrap that object with the withTM.
[56:27] >> I feel like I'm going to need to clean up my code a little bit, but I want to make sure to have you look at it before I delete anything.
[56:45] I will do that in a moment. >> Okay. Notice this env,
[56:53] this is your environment variable. Someone was just talking about envs.
[57:00] This is a way that you can create an environment variable in Next. Then again, if you are committing this to say a GitHub repo,
[57:14] GitHub, GitHub, GitHub, you would want to get ignore this. You don't want to include that in what you're committing.
[57:23] But you want to keep that locally. >> This is how you get the token to be read, right?
[57:32] >> Yes. Without this, you cannot access the Square API.
[57:36] They won't let you make calls and get responses. I mean, you can make a call, but you won't get a response.
[57:43] >> Got it. I'm getting there, promise. >> Now, I guess the only exception to what I just said,
[57:56] sometimes APIs have read-only endpoints, that you don't need any security or authentication
[58:05] because you're just reading information and it's publicly available information.
[58:11] Or information they don't deem needing to be behind a security wall. >> I just realized you're using Next.
[58:32] You're going to learn a lot of React frameworks on the show, I bet. >> Yeah.
[58:39] >> Yeah, probably. >> Yes.
[58:41] >> Yes, probably. I will say, since last time I had someone on the show,
[58:50] I had the Denver API meetup, and I was really excited because one of the questions from the guest was,
[59:00] what is something that web developers don't build themselves, like when they're using stuff?
[59:08] I was like, "Frameworks. Frameworks, they do not build their own frameworks."
[59:13] I was really excited. >> Yeah. There was a time when a lot of these frameworks didn't exist though,
[59:17] and you would code things. >> Well, we would use jQuery.
[59:22] But there was a time there wasn't any jQuery. That's like before my time.
[59:27] But there was a time when people coded on the web without jQuery, which I don't know how they did that.
[59:36] I would go crazy. >> Redwoods is the best, of course.
[59:41] I'm guessing we're not talking about actual trees. That's a framework?
[59:48] >> Yeah. I haven't heard of it. >> Dude, how many frameworks are there out there?
[59:55] No wonder this is so complicated. >> This is a question we never ask.
[60:03] >> Especially when somebody is just getting into it and they're like, "Hey, I want to learn about this stuff."
[60:11] There's so much to learn, especially if you don't know what you want to learn yet.
[60:17] >> This is why we were having a conversation about this offline. But this is why I was talking about it.
[60:23] It's really a good learning strategy is to take something like for instance,
[60:31] building a React with Node or building a Next app. Learning that vertical all the way and learning it thoroughly,
[60:40] and then being able to transfer that knowledge to something else. Pick places like Free Code Camp or some people can go to boot camps.
[60:52] I actually did the crazy route and I did a CS degree, and then I did a boot camp,
[60:58] and then I kept learning on my own. >> Anthony went to a boot camp,
[61:05] I believe. Pretty sure. There's five that are important React frameworks.
[61:12] Next, Redwood, Remix, Gatsby, and Blitz. Is Gatsby what WordPress uses?
[61:24] What is the one WordPress uses? >> I think WordPress may use Gatsby.
[61:29] >> I think it's Gatsby that WordPress uses. That's something I really want to learn because I think
[61:35] that's something that I'm really confused about still is like, there's WordPress and you need to know stuff to be able to build your site,
[61:42] yet how is WordPress made as well? I know that I have somebody coming on the show to talk about
[61:50] Kafka and that kind of stuff and I'm like, maybe this will start teaching me the behind the scenes.
[61:58] But the part that I was going to ask you about if I still needed it here was line 5-10.
[62:06] I don't see it on your file. >> I took that out and replaced it with.
[62:12] >> I didn't think so, especially since we made another model exports. >> What's that red?
[62:20] >> I think it had to go with the other one maybe. Hey, you're there. Why are you red?
[62:28] >> You have an open paren and then open curly brace. >> Yay.
[62:38] >> Anthony, I'm hosting my first Twitter space about mental health and neurodivergency.
[62:53] It's at 9 AM Pacific, 12 PM Eastern. >> 9 AM Pacific, yeah, and I will be there.
[63:02] >> Yes. Okay, let me see. >> This one has.
[63:07] >> Your brain too. You should hang out. >> I don't know where this other closing one is.
[63:18] It's supposed to be. >> React, strict mode, true, experimental.
[63:27] >> Is there supposed to be one right here? >> No. There should be.
[63:37] Oh, yeah. Yes. >> Yes.
[63:40] >> It typically goes on the next line. >> I have one on the next line,
[63:47] but that's closing this one. Would I not have one here?
[63:51] >> No. If you go to loose at the end of loose. >> Yes.
[63:58] >> You go inside of that curly brace. >> Yes.
[64:01] >> You just hit "Enter". >> It should automatically indent.
[64:05] Actually, it didn't automatically indent. What is your indentation, ENV.
[64:15] Let's clean up some of your code. >> Please. Thank you.
[64:19] >> Typically, I do like four spaces and there's actually extensions you can
[64:25] install that will do this automatically for you. It's not a linter, it's I guess the step before a linter.
[64:32] But if you go to ENV. >> Okay.
[64:36] >> You want to indent that four spaces. >> One, two, three, four.
[64:43] >> You can do one tab or four spaces. >> Okay.
[64:48] >> Typically, your tab is four spaces, I think by default. >> Yeah.
[64:52] >> Then again, square access token, you want to indent that.
[64:55] >> One or two? >> One tab or four spaces.
[65:03] That's the rule, is when you have an opening curly brace on the next line,
[65:10] whether it's a function, whether it's an object,
[65:14] the next line should be indented. >> Really quick, I just want to say I
[65:21] appreciate that we're starting to have these conversations because Dan was
[65:26] talking about neurodiverse refers to a group, neurodivergent refers to an individual,
[65:32] and I just think that's really cool that we're starting to have these conversations,
[65:35] so I'm excited about talking about it tomorrow. >> I'm a little bit scared because I haven't in
[65:42] a public setting talk about my challenges with that. >> Worst case, if you don't want to talk,
[65:55] you can ask the rest of us a bunch of questions, or I'm pretty sure most people have
[65:59] learned that I just can talk a lot. Worst case, I'll just ramble.
[66:04] But I don't know, I think it's going to be really,
[66:09] really interesting to learn about who we have joined and talk about it
[66:15] because I've learned a lot from Wesley Faulkner. He's not going to be available tomorrow.
[66:21] He'll be on another one, and he has just taught me so much
[66:27] of also believing that I can do this because being dyslexic and a coder,
[66:33] I've always been so afraid to do it. You don't stick HasBipolar or Twitter on your resume.
[66:43] I don't blame you, but most people can look up my podcast and it says all the shit I have.
[66:49] I just roll with it. Is this curly bracket supposed to be here, up here?
[66:56] >> Yes. >> That's that curly bracket.
[66:59] >> Kind of strange syntax, but yeah. >> Then that doesn't have a curly bracket.
[67:05] This one has a curly bracket. >> Square access token still needs to be indented.
[67:17] >> This or one more like that? >> Right there. There you go.
[67:22] Square access token, you see where the square access token colon,
[67:28] there should be a space right after that. >> I think there is.
[67:33] >> It's just nice. >> There's a space there.
[67:37] >> Really? >> Yeah.
[67:39] >> Okay. >> Right? That's where my cursor is.
[67:42] Yeah, there's a space there. >> Can you go over one?
[67:45] >> Yeah, so there needs to be, yeah, there you go. >> That's two spaces.
[67:52] Cool. Then the React mode, that one doesn't have a curly bracket,
[68:06] but since it's part of this top curly bracket, I would do a tab? >> Actually, no, it's right after a comma, so that's fine.
[68:20] Then the experimental, yes, ESM externals is already indented,
[68:26] and then that curly bracket you want to indent. >> This curly bracket is indented.
[68:33] >> Yeah. >> Then would this curly bracket be indented then, like that?
[68:37] >> Which one? >> This line 8?
[68:41] >> No. >> Okay.
[68:45] >> That is the closing of the ENV. >> I forgot a comma. Is there a comma at the end one?
[68:54] >> No. >> No.
[68:55] >> No comma. ESM externals, yeah. Yeah, I think that's pretty good,
[69:05] so you can hit "Command S" or "Control S". I'm assuming you're on a Mac.
[69:12] >> Yes. >> It's yelling at us for something, that module.exports.
[69:18] Let's see what it's saying. You see the red line underneath module.exports?
[69:29] I'm just curious as to why it's yelling. Oh, a comma is expected?
[69:38] Const module any? Moot woot just recommended reading the access token in
[69:52] a form a.env.local file when using Next.js. >> Yes.
[70:02] >> Dan, no, we haven't talked about using Square versus Stripe. >> Actually, Moot woot, he worked for Square.
[70:12] >> Yay. >> He is the man.
[70:16] >> Well, thank you for joining Teach Gen Tech. I am total new about this stuff,
[70:23] so I appreciate Bakari coming on and teaching me all the things. As you said, he was helping me clean up my code.
[70:31] Cool. Then I'm going to learn what was this, is it because? >> He's right. We should have a local environment local file.
[70:48] >> I'm just going to retype this, see if it. Sometimes I like to think that it's going to be my friend if I do that.
[70:58] >> All right. Well, it is saved. >> We'll see if that presents a problem later.
[71:09] >> Okay. >> I mean, it doesn't look like it should.
[71:13] >> Because I don't know why. >> The other thing we can do is look at the end of the line before it.
[71:20] >> Parsing error for Babel. >> I'd be curious about the stripe versus square discussion as well.
[71:37] Oh, we're going to start a holy war here. >> I mean, for this one,
[71:41] MuteWude, you want to come on and help us talk about this? Because we can put this on pause and totally change it,
[71:49] because I am so much knowledge drop, and Bakari is definitely coming on the show again.
[71:56] >> Okay. >> Let's look at the end of your with TM.
[72:11] >> Okay. >> You can scroll over.
[72:14] >> Let's make sure that. >> It's saying that I have an extra.
[72:22] Look, that's why. >> There you go. Bam.
[72:28] >> Let's see. I'm going to put this on screen. You can create a file named.env.local,
[72:38] then create a variable in there called square_access_token and copy that string over there into,
[72:47] then you can call the process to read the access token in. >> We were going to do the second half of what he said,
[72:58] which is doing process.env. But yeah, he's right. We can just create a local file.
[73:09] >> When I create a local file, new pair, do I create it here in our folder for a local file?
[73:18] >> Yeah. You can just create it at the top level. >> Env.local, and then take that square_access_token,
[73:30] what we put in the config file. >> Where did my config file? Okay, there we go.
[73:36] >> Here it is. >> Take all of this?
[73:39] >> No, just the square_access_token. >> Okay. Do I take the env2 or just the square_access_token?
[73:45] >> Square_access_token and equals that. >> Then we're going to copy that.
[73:50] >> Then go to my env file, and then just call it. >> Save it.
[74:07] >> Then you can just call process.env. >> Does that mean?
[74:18] >> We haven't gotten to that yet. >> Okay.
[74:21] >> But later on, we are going to call that access_token, so we should be able to take out the env now.
[74:31] >> Save. >> Change that too and remove the quotes.
[74:45] >> You ready for the next part? >> Yeah, I'm also was just reading what Moot just said too.
[75:00] >> I couldn't see it. >> Here, I'll put it on screen.
[75:07] >> Change that dot to an equal and remove the quotes and space in there. That's right.
[75:17] >> Equal and remove the quotes and space. Would it be like this then?
[75:32] >> Typically, you want to have a space after an equals. >> Okay. No spaces.
[75:44] Okay. Is it because this isn't a const? >> Yeah.
[75:51] >> Okay. >> Because it's not a JavaScript file.
[75:54] >> Okay. >> It's a JavaScript file.
[75:57] It's just a [inaudible] >> Okay.
[76:02] Well then, okay. With everybody here, I'm going to question you all.
[76:14] We have the const with PM, and I've seen it with a lot of them,
[76:18] like even with Express and stuff like that. There's spaces around it.
[76:24] Do you not do spaces around the equals on this kind of stuff, or do you do it with spaces?
[76:30] >> Typically, if you're in a JavaScript file, I've always had spaces.
[76:40] It just looks too crowded to me. Yeah. He agrees.
[76:47] JavaScript files keep the spaces. But in that environment local file particularly,
[76:53] you don't want that spaces. >> I'll get it.
[76:58] >> I believe it will be a parsing thing, because that file has to be parsed.
[77:05] >> Does that mean there's this parsing error? Do we need to be concerned about this?
[77:14] >> I cannot find next babble. I think that should be fine.
[77:36] >> Thank you, Mutlu. That makes sense. >> Why? No spaces there.
[77:44] Okay, cool. I'm ready for the next step, and if this parsing thing is an issue,
[77:48] we can come back to it. >> We can come back. Right. It shouldn't be.
[77:52] You want to show my screen. The next thing we're going to build is we're
[78:02] going to build the payment form, and first, actually before we do that,
[78:10] we're going to import three things from React Square Web Payments SDK.
[78:18] Here, I'll just send this to you. Those are three different payment types.
[78:33] The payment form encapsulates or wraps the credit card and ACH type. The payment form also has
[78:45] some important logic in there and some of those values that we got from our sandbox,
[78:52] those go inside the payment form. Essentially, if you can think of an actual form, you'd fill out.
[79:00] There's certain information that the Square API needs from in that form.
[79:09] Some of the pieces of information are on my screen here. Of course, there's the actual payment form component,
[79:19] but there's this application ID. There's also the location ID down here.
[79:27] Everything that's currently in the index.js file we don't really
[79:33] need because we're redoing everything in there, right? >> Yes, exactly.
[79:37] >> Because with all of that, it was giving me an error for my import.
[79:43] >> For your import? Can you show your screen? >> Yes.
[80:05] >> Okay, could you please go away, mister? >> It was already showing this where it's all grayed out.
[80:12] That's why I wanted to delete it. I just clicked it and all this information came up.
[80:20] >> Okay, where did all that come from then? Welcome to, oh, create next step.
[80:38] I see. Your index.js already had some. >> I just deleted it.
[80:49] >> You could leave on there, there was a footer,
[81:00] it was a nice footer, you know, [inaudible] yourself.
[81:02] But actually, can you put that back? >> To deleting it all?
[81:09] >> Yeah, the next stuff and let's keep importing. But let's actually try something.
[81:19] Go ahead and save that. >> Okay.
[81:23] >> What we're going to do is actually we're going to run from your command line.
[81:27] We're actually going to run the development server. In order to do that, we are going to say npm run dev,
[81:34] and it should be able to be accessed from localhost 3000 unless there is an error.
[81:44] It said success. Missing script dev.
[81:53] This happened to me before. Npm run.
[82:09] Let's try npm run dev again. >> We're done.
[82:31] >> Let's go to your package JSON, and make sure that.
[82:39] >> Look at that. You both said the same thing, I dig it. >> You said what?
[82:45] >> Moot just said, you can check your package.json for runnable scripts available.
[82:50] >> See, we're twins. >> How do I do that?
[82:55] >> Yeah, just go to your. >> It's right here. Got it.
[83:02] >> There's a whole bunch of them. On next, there's one at almost each level.
[83:08] But yeah, scripts is dev, next dev, next start.
[83:18] >> Then Anthony is suggesting npm start. >> The thing is,
[83:30] I don't want to do that. I want to do npm install.
[83:36] >> Interesting. Let's try running npm install. We just ran that,
[83:42] but let's try that, npm install. >> Anything after it?
[83:50] >> No. >> I need to go. Okay, hold on.
[83:56] I see what you guys are talking about. >> Oh, you're in the outer folder.
[84:04] >> But I don't remember not being into that one. >> The thing is, when we did create Next App,
[84:13] it actually created a whole bunch of folders and folders within folders.
[84:21] In order to run this next project with that command, you have to be inside that project.
[84:35] You are a level above that project. >> Then Anthony is suggesting
[84:42] that I need to reinstall the dependencies. >> Just npm install.
[84:51] >> Strain node models. >> Then React Square.
[84:59] Actually, MootWoot just said it, the React Square Web Payments SDK.
[85:14] >> Hey. >> All right. Now, looks like you got some kind of an error.
[85:33] >> Well, it was saying the WebPaymentPackage.JSON, and then we just reinstalled it.
[85:41] If I redo this one, I'm still getting an error for the next.config.js.
[85:51] >> Here, next transpile modules. >> Sorry. I was just comparing the files.
[86:01] >> I can't read because the uneducated here, I'm trying to resolve.
[86:10] >> It's trying to resolve React Square Web Payments SDK. React Square Web Payments SDK or payment.
[86:21] Let's look at your config. Yeah, let's try that.
[86:29] >> With payments or payments? >> I think it's Web Payments SDK.
[86:33] >> I did that, and Anthony, I did rerun the run dev and it still gave us an error.
[86:44] >> Yeah, we're still getting that error. >> Yeah, even after it.
[86:47] >> Next.config error. Failed to load next.config.js.
[86:51] See more info here. Next.js org docs messages next.config error.
[86:57] Next.transpile modules and unexpected error happen when trying to resolve next React Square Web Payments SDK.
[87:05] Let's go to your NPM config. I'm sorry, your next.config.js.
[87:13] >> Is that in VS Code or in terminal still? >> Yes, that's the file that we worked on together.
[87:20] >> Okay. >> That's NPM.
[87:22] >> With TM, you see that? Okay, now go all the way to the end.
[87:28] >> Oh. >> Yes, there. There we go.
[87:34] It was trying to resolve that. It was like, "I'm looking for this package
[87:39] all across the Internet and I can't find it." >> I appreciate everybody's help with this and
[87:50] also because this is a big reason why I want to start typing these because I've been missing
[87:55] commas or something like that rather than just copy and paste, because it's teaching me where to look while for them too.
[88:04] Yeah. Okay. It should be live. Does this mean that I should be able to do local host to go look at it now?
[88:18] >> You can try that. I have a suspicion that it may not be done, but I'm not sure because it usually actually
[88:25] says live running on local host 3000. >> Oh, yeah.
[88:29] >> When it's done. >> Too many taps.
[88:32] >> But it looks like it was just sitting there. >> Because I don't see.
[88:40] I know when we were, oh, yeah. >> Okay. Got it.
[88:47] >> I know Anthony says, he knows I don't want to read docs,
[88:54] but you should get in the habit of writing docs because you realize very quickly that you don't want to have written docs,
[89:01] that you will want to have written docs. >> That's very true.
[89:06] >> That does not compute for me yet. >> Basically, what he's saying is you just want to make sure that,
[89:14] like for instance, when we got that error and it said, it had a URL that pointed to the next.js docs for your next config file.
[89:25] It's good to get into the habit of taking that URL, going to the docs, looking up the docs,
[89:31] looking up what they say about how to configure your next.js in that, or docs about anything else,
[89:40] particularly when you're troubleshooting errors. >> At least for writing your own docs,
[89:49] what do you-all use for your own docs? Because when I worked at Stoplight,
[89:55] their docs were really easy to use and it auto-generated as using creating API specs.
[90:05] >> Yeah. There's OpenAPI, Swagger. That's one of the, yeah,
[90:14] there's the readme.md files in your repo. But if you have a larger organization,
[90:22] then sometimes, yes, they have those auto-generated docs. There's, for instance,
[90:32] if you go to the Square documentation, there's API reference.
[90:37] Then there's actual documentation. We were looking at the documentation to figure out
[90:42] how we needed to set up a Square account, how we needed to create these different values,
[90:50] so we could actually do a charge to a fake credit card. But there's a ton of tools out there
[91:02] that have different levels of automation in creating your docs. One of the big industry standards is the OpenAPI, Swagger.
[91:19] The idea is that you think API first, and then those docs can be generated
[91:27] from a particular file that you create when you're writing your API initially.
[91:34] >> Okay. >> Do it in a YAML file or a JSON file,
[91:38] and your Swagger docs can be. Then Swagger has a bunch of standards as well.
[91:46] >> Yes. Anthony, let's do it, because I think docs is one of the most confusing things ever,
[91:52] at least what each of them do. >> Maybe. I like Stoplights,
[92:01] because it did describe what your endpoints were, but that was back when I didn't understand APIs as well.
[92:09] Maybe it would be cool to create an API spec in Stoplight, not because I want to promote Stoplight for everything,
[92:16] but that's where I've been to slowly start understanding it all. But okay, my local host is working.
[92:25] Yes, and you have generated the XJS, the development page that we created.
[92:40] >> Yay. Then Mootoot says, "That's where generate our docs off of an OpenAPI spec."
[92:48] >> There we go. Bam. What did I just say? I think we're twins. I really think we're twins.
[92:54] >> You should see a picture of him and a picture of me right next to each other.
[92:59] >> On a serious note? >> No.
[93:01] >> Okay, because I don't know what anybody looks like, so that would have been really funny.
[93:06] >> We both do have the Oakland connection, so I guess I'm grasping for straws at this point.
[93:15] >> Mootoot, I know that you're from Square, so either way, you need to hire Bakari,
[93:23] because he is patient enough to teach me all this stuff, and if he's a devrel,
[93:27] this is what devrels have to do, is go on all these shows and teach us stuff.
[93:32] I'm just saying, he's really cool. Anyway. >> Awkward.
[93:37] >> You're welcome. I am that person. I am very awkward.
[93:43] My bad. You can ask Anthony, I do this stuff to him all the time,
[93:48] and Rizal, and Ramon, and Yeray. >> I know it's 10.35,
[93:57] and I know you sent me a message here saying that we're going to. >> Yeah, we totally went over time,
[94:02] which I'm down to continue or pause. >> I do have something to throw out.
[94:19] I would be totally down to continue this later this week, if not tomorrow or something.
[94:26] Tomorrow is our Twitter space or maybe the day after, because I think breaking it up,
[94:31] it makes it a lot more consumable, because anybody watching these later on,
[94:36] I think having just the fact that we ran into errors, it's something that a lot of people are going
[94:43] to really benefit from of learning how to do that. Then Anthony, I think it would be dope to have
[94:50] you show me how to do documentation, maybe using this as a reference,
[94:57] and then having you back on the show. Moot Moot, I still want you on the show.
[95:02] Let's talk about why Square over Stripe. Seriously, I think we should just do it.
[95:10] >> Sounds good to me. >> Are we at a good pausing point though?
[95:15] Because I know you got to go. >> Yes, we are. We just generated.
[95:19] It's like this is a really good stopping point because we just generated our boilerplate Next.js page.
[95:30] >> Yeah. >> I think this is a good place to pause.
[95:36] On our next episode, we will actually import some.
[95:43] >> Well, okay, put it this way. You got to be on the show and teach me something, Moot Moot.
[95:50] Because just expanding and learning from different people, I think is something so awesome.
[95:56] Anthony, AJC, WebDev, he's been on the show. He's also been watching these.
[96:02] We've all been learning from each other, and it's helpful to be able to learn from a starting point
[96:09] of being able to see a previous show, so they know where my knowledge is at.
[96:16] I've actually been able to start to re-teach this to people, which is like [NOISE]
[96:22] >> He just said DM me on Twitter. >> You got it. Cool.
[96:27] On our next episode. >> On our next episode,
[96:31] we will be importing some components and building out our integration.
[96:37] We'll also are going to build a quick and dirty endpoint in Next.js,
[96:44] so we'll have a full stack app running. >> Yes. I know that we went through a lot of theory today as well,
[96:51] which I appreciate because learning the theory along with the actual practice of building these really
[96:58] helps with getting the information to stick. >> Yeah.
[97:03] >> Oh my God. >> Reminds me of my garage recording studio when I was in a band.
[97:10] I actually, this is my recording studio. [LAUGHTER]
[97:14] Legit, this is my recording studio. >> Because I just have fun blasting everybody's coolness.
[97:22] Bakari, if you go to his Twitter, he has his link to all of
[97:27] his music that he currently has out, a couple of singles. At some point with everyone that's in band,
[97:34] can we do a live stream of bands, different people playing stuff?
[97:38] I feel like that would be cool. >> I think I might.
[97:43] I'd be open to that. The thing is over a live stream,
[97:47] it's really hard because of the latency. >> Yeah, that's what I was just thinking about.
[97:52] >> Places. But if you have people that are in a certain geographical area maybe.
[97:56] >> I don't know. You're in California and we got Anthony's. Yeah, I'm going to leave it there.
[98:08] >> Oh, sweet. >> Like Anthony, we talk about your podcast or your live stream.
[98:15] Twitter space, there we go. This, dope.
[98:20] I like talking about people, it's fun. Y'all do cool stuff.
[98:24] >> Well, thanks for having me on. >> Yeah, for sure.
[98:27] Thank you. Thank you for the knowledge drop. Thank you. Yes, Anthony and people are dope.
[98:34] Thank you all for joining and commenting and see you tomorrow at our Twitter space.
[98:41] >> Yes, I will be there. >> See you later. Bye.

