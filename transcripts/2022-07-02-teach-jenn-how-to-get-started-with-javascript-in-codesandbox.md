---
showLink: "https://www.youtube.com/watch?v=Dc5t9w7GD50"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-how-to-get-started-with-javascript-in-codesandbox"
title: "Teach Jenn How to Get Started with JavaScript in Codesandbox"
publishDate: "2022-07-02"
coverImage: "https://i.ytimg.com/vi/Dc5t9w7GD50/maxresdefault.jpg"
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

[00:00] I'm excited. Hello, hello, beautiful humans.
[00:06] I'm totally new to this live thing. So we are-- I'm checking out and making sure it's actually
[00:11] showing up on the Twitters and LinkedIn and that kind of thing.
[00:15] Oh, it is. How exciting and creepy looking at yourself on Twitter.
[00:21] Yes, definitely mute your windows. Yes, and thank you, Jere, for joining us today.
[00:31] Please introduce yourself and what you'll be teaching me today.
[00:35] Yeah, happy to be here. My name is Jere Suikkula.
[00:40] I'm a developer advocate at a company called Mapped In. I've been a developer professionally,
[00:47] I would say, for four years or so, but I've always had that as a hobby.
[00:51] And today, I figured we'll take a look at Code Sandbox. That's an online coding environment
[00:59] where it's really easy to get started. You get to do visual stuff with JavaScript, HTML, CSS there,
[01:06] and you see the feedback immediately. So I feel like that's a really great way for beginners
[01:11] to start coding when they get to see the results of what they do.
[01:15] Yes, thank you. And as a bit of background, because this
[01:20] is how I've met so many of our upcoming guests, is I love public speaking, going to events,
[01:26] talking to everyone. And one role that I've really wanted to go into
[01:31] is developer relations, also known as dev role, or developer advocate, or developer evangelist.
[01:40] There are a lot of names for the role, and it's different at every company what it does.
[01:44] And you are one of the kind people that talked to me about it first.
[01:49] I'm curious, could you explain to everyone what you do with your role?
[01:54] Yeah. So in my role, and this really depends on companies,
[01:58] but my role is a lot of technical customer support, helping our customers use our SDKs.
[02:07] So we have a product that software developers use to put indoor maps on websites or applications
[02:13] on mobile. And my job is to help them make sure that they're successful
[02:19] on the technical side of things. So that also involves creating demos for our sales team
[02:25] to show off what our technology can do. And then, of course, putting content
[02:31] on our developer portal website that is aimed towards the developer audience of our customers,
[02:37] where they can see examples of the basic functionality of what you can do with our products.
[02:45] Very cool. Thank you.
[02:47] And for something that I've been seeing in the developer relations world is you've also done a bit of marketing.
[02:56] And there's a bit of so many of that human aspect as well. And I absolutely love that because it's like, cool,
[03:03] you know how to-- you've had to learn how to break it down for people, which
[03:08] I know can be a challenge even for myself. I'm like, I used to work at an API spec company.
[03:14] And trying to explain that to my mother is very, very difficult because what is an API?
[03:24] Application Programming Interface. What?
[03:27] You know, two softwares work together. It's great.
[03:30] And then a spec, I'm like, it's your blueprint. Think of your blueprint for the house.
[03:35] It's like the blueprint for this application you're going to develop.
[03:38] And yet, you mentioned something as well that I'm like, I don't even know how I would explain that to my mom of,
[03:45] what's an SDK? Yeah.
[03:48] And that's actually one of the questions that I also have to answer quite a lot when
[03:52] I try to explain what I do. So if I was talking to a completely very
[03:59] non-technical person, someone who can use a computer but not actually doing anything, building with it.
[04:05] So I would say an SDK is a library or contained piece of code that helps you do something specific with it.
[04:17] So for example, you want to use-- in this case, where I work, I always use that as an example.
[04:26] So you want to put those maps on your websites. But you don't want to build them from scratch.
[04:31] That's a lot of work. There's a lot of things that go into it.
[04:34] You have to figure out what your data looks like. What is all the data that you need for that?
[04:40] And then how do you render that? So when you take an SDK, that means some other developer
[04:47] has already done a lot of work to answer a lot of those questions for you, put them in a package.
[04:54] And then that's kind of like an abstraction that hides those details away from you
[05:00] and then gives you an API that you can work with on a higher level.
[05:06] So you don't need to worry about, how are things rendered? How does that happen?
[05:10] You just tell that that's what you want to happen. Interesting.
[05:16] I remember my time at Stoplight, and I had to talk to a lot of the engineers
[05:21] working on launching a training program and asking every single developer or engineer what
[05:30] is the difference between an SDK and a API. That was a lot of fun, hearing all the answers,
[05:37] because it's the same with developer relations. People are like, they're all different,
[05:42] mattering on the company, mattering on the team, mattering on what they're working on.
[05:46] And I think that is such a fun part of the technology world. Yet a giant reason is we're talking about JavaScript
[06:00] and you said that we're going to use it on Code Sandbox. Yet there are so many different coding languages.
[06:08] And while I was on my journey to go, OK, cool, I'm going to start learning to code just so I
[06:14] can get this job I really want. And people would be like, well, it
[06:19] matters if you're going to be a full stack engineer or not. And I'm like, a what?
[06:24] And so let's see if I can explain this right. So a front end developer or engineer
[06:31] are people that develop the websites the way-- make it look pretty kind of thing.
[06:38] And then a back end engineer is who creates the actual product. Is that a good way of explaining the two?
[06:47] Yeah, I think the front end is well explained. I think some front end engineers, though,
[06:55] might get offended that their part is not the actual product.
[07:00] My bad. Yeah.
[07:03] Because the back end takes care of the data and making sure things happen that need to happen.
[07:11] A lot of going to the database, modifying that data, making sure that it's fit to be displayed and all that.
[07:18] So there's a lot of that kind of work there. And I think that's also in motion.
[07:24] It changes what things happen in the back end and front end. But if we think about it really as technically,
[07:32] from a technical perspective, I would say front end is what is being run in your browser.
[07:39] And that is definitely the UI and all that stuff. But then nowadays with frameworks like React,
[07:45] a lot of that business logic on what is displayed there, like do you have a message box or something like that,
[07:54] or news feed of items using Facebook here as an example, because they came up with React.
[08:01] Those are very big pieces of code that have a lot of logic in themselves that are not just
[08:06] about how it looks like, but it's also about how to deal with that data.
[08:11] And then the back end is what happens on the server side. Got it.
[08:16] And to put the two together, that's what full stack means, is that someone that can
[08:20] do front end and back end. That's right.
[08:23] And there's a lot of these frameworks these days that make it easier to be a full stack developer.
[08:30] Of course, a lot of businesses and startups are popping up, and they want to get started fast.
[08:37] And how do you do that? Well, you hope that one person can do everything, right?
[08:43] So in order for them to do everything, they need to be able to do that fast on every place.
[08:51] So there are CSS frameworks that make it fast for you to do something beautiful on the front end side.
[08:57] And then on the back end side, there are frameworks like Next.js that we can have a look at later
[09:05] or put in the notes somewhere for people to look at. That makes a lot of things easier on the back end side,
[09:13] so you don't have to build everything from scratch. And that comes to the idea of SDKs
[09:17] as well, which is like an abstraction. Taking some big piece of code and making it
[09:23] so that the application developer doesn't have to worry about it.
[09:27] In this case, full stack developer doesn't have to be worrying about how
[09:33] to cache something, for example, or things like that that are very difficult to do,
[09:37] like difficult problems. I understood a lot of what you're saying,
[09:42] yet at the same time, if somebody were to ask me, I don't think I'd paraphrase it very well.
[09:47] So I appreciate that. These are probably questions I'm going
[09:52] to be asking again and again for a while till it sticks. I would say something that does come to mind with frameworks,
[10:02] and see if I explain this one right, is there is a-- so you have your coding languages,
[10:10] and then you have frameworks that can be put on top of those coding languages
[10:14] to make them faster. Like React?
[10:19] Yeah, so what happened with React, for example, is that it makes it easier for you
[10:25] to build interactive frontend applications and manage the state and the data that's
[10:32] there, easier than just doing with JavaScript itself. And that's why they exist.
[10:39] And so you kind of trade a little bit of freedom of doing whatever you want to do,
[10:46] however you want to do, for getting some pieces of the puzzle already pre-built for you.
[10:53] Interesting. OK.
[10:55] One day, we're going to have someone come on and talk about GraphQL, because during the API Days Interface
[11:01] Conference, when I was emceeing, they were talking about GraphQL.
[11:05] And I was just like, you're speaking another language to me. Figuratively, it is a coding language.
[11:13] But also, I just didn't even click what it did. So one day.
[11:20] I'll be watching that one, for sure. I've touched GraphQL a couple of times,
[11:23] but it's definitely not my expertise. So looking forward to that.
[11:28] I totally get that. All right.
[11:30] So into the nitty gritty of JavaScript on Code Sandbox, what are we doing today?
[11:39] All right, yeah. So like I said, Code Sandbox is an interactive online coding
[11:44] environment. And one of the best parts of that
[11:47] is that it's out-of-the-box. It's a multiplayer experience.
[11:53] So if you share your screen and start the Code Sandbox, you go to codesandbox.io.
[11:59] Code sandbox dot-- Now we can get started there.
[12:07] Ooh, pretty. Create sandbox, I'm guessing.
[12:12] Yeah, I think that works. Yeah.
[12:16] And then we want to be signed in, I think. Yeah.
[12:20] Because this might be a good idea to sign in. I'm not sure if you can share.
[12:24] I'll try. Let's find out.
[12:27] And I'm very excited, because we're going to have Rizal from GitHub come on at a time.
[12:33] And so that way, we can also learn about GitHub. Because that's been a confusing matter for me, too.
[12:40] Yeah, GitHub is one of those things that definitely are very helpful for developers to get a hang on very early
[12:50] in their careers now. We're just going to-- oh, wait.
[12:54] I need to invite someone. Oh, you're not going to let me.
[12:57] OK, we'll just exit out. Yeah, it was just pictures of what you can do.
[13:02] So create a sandbox. So what we actually see here is a whole bunch
[13:08] of different starters. So basically, these are templates
[13:17] that have already a little bit of code in them so that we can get started easier.
[13:20] You can see there's React, Apollo. What else do we have?
[13:25] ViewPress, p5.js. So all kinds of different things there that you'll eventually--
[13:32] I'm sure you'll run into most of these things. Yay.
[13:36] And definitely Go Exploring as well. That's part of the fun of being a programmer
[13:42] is that once you get more and more into things, you just learn by tinkering with things
[13:47] that you've never touched before. Today, though, we want to do vanilla JavaScript.
[13:56] And that starts something for us. Maybe.
[14:04] It takes a little bit of time. So what's happening, it's downloading a bunch of files.
[14:10] So there's a share link there. If you could-- yeah, this is sharing in terms of now
[14:18] you've built something cool after. And you're like, hey, everybody, look at what I did.
[14:23] So maybe afterwards, we post this on Twitter or whatever we end up putting on this web page today.
[14:28] Got it. And talking about Twitter, I'll just send you this link
[14:32] on Twitter really quick. Yeah, I think I might need another link, though,
[14:36] from the left side. So I'll explain that.
[14:39] So there is the two people icon on the left side menu. All right.
[14:45] So in order for me to join, I would need that link. And then both of us are there.
[14:54] And then because now some other people might see the link as well, I think
[14:58] we'll be in classroom mode so that you get to decide who can edit it.
[15:08] Oh, gotcha. Yeah.
[15:10] So now you can see me there. But if you make me an editor, then I
[15:13] can also edit the code in front of you so we can do that together in case there is something.
[15:20] Make editor, yay. Yes.
[15:23] All right. Now we're set up.
[15:25] So that was pretty fast. Now we have a full-blown coding environment here.
[15:32] In the left side, we have some options. And we can look at the files.
[15:38] We can search the files. Then there are some settings and configuration files
[15:45] that we don't need today. But these are the ways, for example,
[15:48] if you wanted to deploy this somewhere really later, for example, Netlify, which can host JavaScript and HTML
[15:56] projects with just a few button clicks, that would take care of that for you.
[16:01] GitHub, so if we wanted this to be on GitHub so that you can edit from there, do pull requests and all that,
[16:09] that's something to look at in the future as well. And here's the deployment part.
[16:14] Very cool. And then just like we were saying earlier,
[16:18] this is where we add new individuals. Awesome.
[16:23] That's right. So that's kind of the sidebar options there.
[16:27] In the middle, we have our code. So if you open the one with the files in it,
[16:35] that's probably the most helpful one of these. So here, I think the first thing we should do
[16:41] is go through the files and kind of see what's where and what feels familiar to you, what you've seen before
[16:46] and what you would guess that they do. OK.
[16:51] I will say I've seen an index.js. And that's, if I remember correctly,
[16:57] because I did start a JavaScript course, but only a few days in. But the index is what's going to--
[17:06] like, if you had different class files, different JS files, you would put them all in the index to call, I think.
[17:16] Index is usually what we call the starting or the first file or where things then go deeper from.
[17:24] So that's where you would import everything else that you're working on, like if you had classes or something
[17:28] like that. OK.
[17:30] And then I'm only guessing on styles.css, that's probably where we would put any colors
[17:39] or that kind of thing? Yeah.
[17:42] Text, yay. So here we can see for the HTML body,
[17:48] we put the font family to be Sans Serif font. That will take the Sans Serif front of your system default,
[17:56] I think. And then just display that one.
[17:59] System and browser default or something like that, and then display that.
[18:04] Do you want to change the color of that font already? Sure.
[18:07] All right. So just in there and a new line, and you write color.
[18:14] No use here, even though I am in Canada. Do have to write it with just the O.
[18:21] And then a colon, and let's see what happens. Oh.
[18:26] And it even has what they all can be used. All right.
[18:30] So yeah, there's definitely a lot of default colors that you can use.
[18:34] This is called IntelliSense. I think is the--
[18:40] I don't know if it's the brand name or whatever. But basically, it's telling you the options you have here.
[18:47] It's kind of giving you a hint of what you could put there. And right now, so just to--
[18:52] we're writing in HTML. Yeah, so this is CSS.
[18:57] OK, we're writing in CSS. OK, cool.
[19:01] Just making sure I'm following along. Yeah.
[19:04] And CSS is Cascading Style Sheets. And mostly, they are used-- and end the sentence
[19:11] with the semicolon at the end. OK, I will once I switch that color,
[19:15] because it was really hard to read. It was a bit too bright, yeah.
[19:19] Too bright, too bright. Let's go not so-- we'll go with the dark purple.
[19:24] Perfect. And then semicolon.
[19:27] That one? There you go.
[19:29] Sweet. And then hit Command Save on your keyboard.
[19:34] And that saves your changes. You're able to see that next to the file name,
[19:39] the style CSS on the top bar, it changes from a circle to an X. So that's how you know you have unsaved changes there.
[19:49] OK. Yeah.
[19:52] Just in CSS, if I wanted to, could I create another body and put the color in another section of the body?
[20:02] Or would I always have to put it next to other pieces of the body?
[20:07] Yeah, that's a good question. So right now, there is only one element on the HTML page.
[20:14] And that's the body. We can go have-- well, there's a couple of elements.
[20:18] But let's go have a look, actually. But definitely, you can edit other elements as well.
[20:28] The body there is called a selector. And that defines which elements your styles apply to.
[20:37] And in this case, this is now the HTML file. So if you look at it, you can find the body element in here.
[20:41] So this is kind of like a tree of elements. And there's the body.
[20:44] That's the end tag. And that's the start tag of the body element.
[20:50] So if we wanted to, we could add a head in the styles.css to change information on that piece of--
[21:00] yeah, head is metadata. So that's not displayed or rendered in any way.
[21:06] But maybe we'll add something here and then see how we can change how that looks.
[21:14] So underneath, we're in the body under the div ID app. So make a new line there.
[21:21] And let's do a button. So start with the--
[21:27] open a new tag and write button. So like this?
[21:32] Yeah. And then close it.
[21:36] Close that. And then you have to end that tag as well,
[21:39] same way as you've done with the div above. Now that we're in HTML land, we end things with--
[21:49] like you see in the line above. Oh, OK.
[21:53] Like this? There you go.
[21:55] And it's already suggesting-- auto-suggesting there, the option for you.
[21:59] OK. There you go.
[22:00] So we don't see quite anything yet. I think there might be maybe something there.
[22:08] But that's because we don't have any text inside the button. So no--
[22:12] OK. No--
[22:15] I was just going to try and move inside the button. Maybe click me.
[22:21] Yeah. Oh, yay.
[22:24] There you go. And now it appears there.
[22:25] I want to move you. It should move.
[22:28] Yeah, there you go. Yeah, there is a spot there to move.
[22:31] All right. So now we've created another element on the page.
[22:35] Save the index HTML. And then we can go back into the Styles page
[22:44] and see how we could edit. Now, if we wanted to edit that button,
[22:48] how we would edit a button. So would it be like this?
[22:52] That would be it. OK.
[22:55] Me. There you go.
[22:59] Can make this one a really annoying color. Oh, yes.
[23:10] Probably want to change the background color as well. So that would be background dash color.
[23:16] Maybe this is dark or-- Oh, OK.
[23:19] I like how this one helps you guess them. Yeah.
[23:25] So it knows what the valid values in many places in your code are and then suggests
[23:32] those valid values for you. And that is very nice.
[23:36] It helps you get started a lot faster. You don't have to be Googling what the valid values
[23:40] or options would be in many situations. Oh, this is so cool.
[23:45] Oh, and you can click back and forth up here too. And then if we wanted to have this hyperlink somewhere,
[23:54] I doubt it's going to let me highlight it and right click for link.
[23:59] How do you actually create a link so it could go somewhere kind of like the here?
[24:07] All right. Yeah.
[24:08] Let's create something underneath the button then. And it will be called an anchor tag.
[24:14] So that's just an a tag. That's right.
[24:18] I actually forgot that I can edit here as well. Yeah.
[24:22] Oh, then you go. All right, all right, all right.
[24:24] My turn. OK.
[24:26] So we will add an anchor tag here. And then we'll close it.
[24:32] Now, we don't see anything yet. All right.
[24:37] This is a link. Now, it's not clickable yet, right?
[24:44] Nothing happens if you click it now. So we need to make sure it's clickable.
[24:51] In order to do that, we give it a href. So where do we want it to link to?
[24:59] So in this case, I can put Google here. But maybe you put your website there or something like that.
[25:05] Right. Aha.
[25:13] It broke. All right.
[25:15] I think that's great. We found our first error message.
[25:18] Ended up with our first error message. So it looks like it wants us to add HTTPS there.
[25:23] Ah, OK. So it was kind of weirded out by the path choice we had there.
[25:31] It was interpreting it in a different way. So we wanted to have the HTTPS in the beginning.
[25:35] And if we go back to that error, is there something that I could have known that that was the error?
[25:43] Because I feel like that's something that I get really confused on is it's not saying it's just a module in path.
[25:53] It doesn't necessarily say, oh, it's because the HTTPS is missing.
[25:59] Yeah, I think in this case, it's not the perfect error. Like, it doesn't really--
[26:09] I'm just going to Google it. --really help with that.
[26:11] See if anything comes up. Because this is also, I think, very
[26:17] related to the environment that we're working in, in CodeSandbox, and the way it handles this type of situation.
[26:28] The reason I realized what was going on was because it should not be looking for a module path.
[26:37] And it's looking for something relative to index.html. So I realized that it's trying to find a relative path
[26:48] from our current file. So for example, if we had an other HTML file,
[26:55] let's say contact us page, contact us HTML, we could have that here.
[27:02] And that would then be contact us dot HTML. And then we would create one file here, over here
[27:15] on the site, contact us HTML. Interesting, OK.
[27:24] I guess in this case, it would be source, contact us HTML. And then if it's clicked, then that will open that page.
[27:34] It's making enough sense, yet at the same time, it's definitely going to take some practice.
[27:40] Yeah, there's a lot of things here that we're looking at right now.
[27:45] Because you've noticed there's CSS, there's HTML, and then there's-- we haven't actually even written
[27:50] any JavaScript yet. So we're just looking at elements on this page.
[27:56] And this is a big reason, and I appreciate your time today, because it's like, where do individuals start?
[28:04] When I asked everyone, I was like, hey, what language should I learn first?
[28:09] Yes, the majority said got to JavaScript, but so many of them were like Python, or even CSS.
[28:18] And I'm just like, I need-- I don't know.
[28:22] So I just went with JavaScript, since that's one of the more popular ones, and it has so many formats
[28:30] to go with it, with React and those type of things. So I was like, I'll start with JavaScript.
[28:35] And I learned that a big reason that it's called vanilla is because JavaScript now has so many of the formats
[28:46] that not a lot of people use the vanilla. But if you know the vanilla, you'll
[28:51] probably be able to figure out all of the other flavors we'll go with.
[28:56] Yeah, so everything else is built on top of that vanilla JavaScript, indeed.
[29:01] And yeah, that is actually-- that is one of the most difficult questions,
[29:05] because there's so many programming languages. There's so many resources available these days.
[29:11] Where do you get started? And somebody asked me that the other day,
[29:15] and I had to ask them, it depends what you're interested in.
[29:20] Do you want to make games? Do you want to call some existing APIs
[29:28] and pull some data about movies and then display them on a web page?
[29:34] What is it that you want to do? Because I think one of the most important things about programming
[29:39] is practice and doing it. So in order to practice, I think the easiest way to be motivated
[29:45] is to find something that you really want to do. Like, I need this application or something like that.
[29:51] I want to have this game or whatever it is. Or I want to do data science.
[29:56] I want to figure out what is the best height level in Minecraft to mine diamonds on.
[30:06] I didn't even know-- I think in the back of my head, yes, I
[30:10] knew you could do all of those things. But I think that's something that's been really hard
[30:14] for myself, is I want to learn it to get a job. And because in the API world, where
[30:22] I've been working the last year and a half or so, it's like, how do I learn more about APIs
[30:29] to know in what language supports those? But again, as you were asking, it
[30:34] matters where you are and what you want to learn about the APIs.
[30:38] Because a lot of individuals that do some data mining but also do back end, it's Python.
[30:45] They're like, that's the best one you should learn. And I'm like, I don't even know what
[30:50] all the options are to know. And that's why I really appreciate
[30:54] that we're going through this. Because it's like, cool, I'm just
[30:58] going to stick with JavaScript to get one started and understood.
[31:01] And then I will start working on a different language eventually.
[31:06] Yeah. And definitely, once you've learned one language,
[31:09] it's easy to learn other languages afterwards. I would recommend 9 out of 10 times, 8 out of 10 times,
[31:17] I would say start with JavaScript. If a person has no idea where to start from,
[31:22] I would say start with JavaScript. One of the big reasons is that the results
[31:27] are very visual once you start working on it, like on a web page or something.
[31:31] It's very shareable. It runs in your browser, so you can show it off to everybody.
[31:36] There's just so many resources about JavaScript. YouTube, for example, there's so many--
[31:43] you can learn anything about JavaScript online. And with other things like Python,
[31:53] they are a little bit more specialized. And JavaScript has gone from being
[32:01] a language that creates a little bit of interactivity in the browser to something that is now
[32:06] used for full stack applications and everywhere. So it is in the front end in our browsers.
[32:14] But it is also on the server side where we deal with databases and all that.
[32:21] So it's a good place to get experience in a language that can be used in a lot of places.
[32:28] And then once you have that, you can find out what's interesting to you from there.
[32:34] And then if there is a more specialized language that works for that area, you can go there then.
[32:39] I love that. And something that you mentioned is there's so much content
[32:45] online about this. And I'm like, yes, there is a lot of content
[32:49] about JavaScript. But I'm so stuck on something.
[32:52] And that's a big reason Teach Gen Tech was started. Because it's like, this gives me an opportunity
[32:59] to ask someone like you or people that are more experienced at it going, OK, I am really, really stuck here.
[33:05] And all the Googles and all the Stack Overflow and GitHub is just not making sense.
[33:11] Where it's normally just like, oh, I didn't think of it in the same logic
[33:17] because I haven't learned that logic yet to where it sinks in.
[33:20] And I think that's a big piece of everyone listening and watching this.
[33:26] Please comment your questions where you got stuck, where you're wanting help.
[33:30] Because this is why we're going to have so many different guests from different backgrounds.
[33:35] Like, we're going to have someone on for GraphQL or from GitHub.
[33:39] And I think that's one of the most exciting pieces is finally, in my mind finally, having the accessibility
[33:46] to people that already know this day in, day out. We're watching a ton of YouTube videos.
[33:54] I think I spent like four hours trying to figure it out. And I still couldn't figure out a piece of classes.
[34:01] So it was-- I so appreciate that you're on today.
[34:06] Yeah, it does become a problem kind of like of abundancy, kind of like an analysis paralysis and all that
[34:15] when you see everything. Like, there's so much.
[34:17] And you're like, so what? I need to learn this specific thing.
[34:21] How do I go about it? Because you kind of don't know what you don't know.
[34:26] And you don't know what you need to know in order to know that thing.
[34:30] So for that type of situations, I would recommend something like FreeCodeCamp, for example.
[34:36] Absolutely brilliant resource. There's so much there.
[34:40] Also in other languages. That kind of has like a curriculum
[34:44] that you can follow and go through the basic concepts of programming and then how to do those things in JavaScript.
[34:56] Because then that kind of teaches you the language you need to understand.
[35:00] There's a lot of-- and I don't talk about the programming language,
[35:04] but kind of the language of computer science. And then you can understand what do people mean
[35:12] when they talk about loops. Yeah, and just like how we've been--
[35:17] because the .js is our JavaScript file, right? That's right.
[35:21] OK, so we've literally looked at CSS, HTML, and each of them are so different on how you put something in, on how they're
[35:33] read. And I think that's something that's so beautiful, yet also
[35:37] makes it more complicated. Because it's like, OK, cool.
[35:40] I kind of understand HTML, yet-- wait, what?
[35:45] And you don't even realize you're making these mistakes. So like we were talking about with the error.
[35:51] And so I-- again, this is really exciting, being able to learn it.
[35:57] What are some things that we can create in our JavaScript file? Yeah, now that we've created a couple of elements in the HTML
[36:07] and CSS, I was thinking we could maybe create a couple of links using JavaScript.
[36:14] So first, maybe we make a list of your favorite websites, or maybe, let's say, your YouTube channel, and Twitch,
[36:21] and Twitters. And we render links for all of those.
[36:28] What if we do that? Let's see how we could do that from JavaScript.
[36:32] All right, that means I actually need to know all of my links, but I'm getting there.
[36:37] All right. All right, so if--
[36:41] because this other stuff is done, would I create a different--
[36:45] like go down a few and create a different one, or would I put it all within that semicolon?
[36:52] All right, so let's go through what's happening here first. And then we can figure out what we want to do.
[36:58] So the first line, import style CSS, that tells our bundler-- bundler is a special JavaScript program
[37:08] that runs before this is served to us, and it puts everything together.
[37:14] That's the name bundling, bundler. It puts everything together.
[37:17] So in this case, it makes sure that our styles are also part of the output.
[37:24] Then on line 3, we tell JavaScript to get the whole document, so the HTML document,
[37:31] and then find an element with an ID of app inside that document. OK.
[37:39] And then we modify that app element's inner HTML to be what's there right now.
[37:48] So if we copy pasted what's inside there right now, the purple text from line 4 to 9,
[37:56] let's actually cut that so that it doesn't stay there, but cut it from there.
[38:03] Could we also, just thinking about it, if we do these, does it make it into comments?
[38:10] Oh, no, it doesn't. OK.
[38:12] It doesn't. In this case, it doesn't.
[38:14] And that would be a comment in JavaScript. OK.
[38:18] However, what-- Because it's showing inner HTML, it's
[38:23] not going to work because it's HTML in the purple right here. Right.
[38:26] The purple is a string. OK.
[38:29] So it's like a string that we're putting in there. But if you cut that out and now go into the index HTML page,
[38:35] you notice it disappeared already. Right.
[38:38] And then go inside the div ID app that you saw before on line 9, inside there, leave that,
[38:46] but the tag itself there. So that's between the start of the starting tag
[38:51] and the end tag of that element. Oh, right here.
[38:53] Paste that there and see what happens if you save the file. We should.
[39:04] Is it because we have too many divs? No.
[39:09] Honestly, this is a very small amount of divs. OK.
[39:12] Once you get using these frameworks, you'll end up with a lot of divs.
[39:16] Let's save this. Oh, OK.
[39:18] I realize what happened. So go back to our index.js still.
[39:24] So this is actually a good exercise. So what we basically did, we moved that HTML
[39:31] into the HTML file, right? However, this JavaScript file is executed
[39:36] once that index HTML is first rendered. Then we execute this piece of code.
[39:45] And this code now says, put empty inside the app. OK.
[39:52] So we would have to delete-- would we delete this line or delete the inner--
[39:57] the dot inner HTML? And you were wanting to comment something,
[40:00] so now comment the line number 3. And then save that.
[40:05] So that is indeed how you do comments. Now that piece of code is not run, and our result is there.
[40:13] OK, because we moved it over to where the HTML file was. Exactly.
[40:21] So it was just rendered there using JavaScript. It was the exact same thing, but that
[40:25] was how JavaScript could modify the HTML of an element on that page.
[40:32] Got it. I'm going back and forth, because it's
[40:36] like it's starting to sink in of how we created app. And so it was using app and inserting it there.
[40:45] OK. As long as I don't have to recreate that and do something
[40:48] else, I think I'm starting to follow along. All right.
[40:53] Next, let's have a look how we create a list of things. So we're going to make an array in JavaScript.
[41:03] Is that familiar to you? No, I was working more with, at least as far as I got so far,
[41:12] was constants. Constants, all right.
[41:14] And not an array yet. All right.
[41:17] So what kind of constants did you have? You had numbers and strings and--
[41:22] Just numbers. Basically just numbers and a couple of colors.
[41:26] OK. So an array is also can be a const.
[41:35] And we say favorite websites here. And then we open it with angle brackets.
[41:46] I think they're called angle brackets. I'm not sure.
[41:50] So and inside here, we do a comma separated list. We do a comma separated list of strings in this case.
[41:59] So maybe you put your websites there now, like Twitch and YouTube links there in those spots.
[42:08] So this is now an array of strings, if you think about it. So there's multiple strings in a list there.
[42:16] OK. I'm going and finding the other ones because, of course,
[42:19] I'm like, oh, I don't know what they are off the top of my head. That's right.
[42:24] And I'll go to our index HTML page. And I'll add an element there where we will render those.
[42:30] OK. [CLICKING]
[42:33] [CLICKING] [CLICKING]
[42:40] [CLICKING] [CLICKING]
[42:52] So-- I'm grabbing the last two.
[43:11] That's good. Gives me a little bit of time to think
[43:17] about how we want to do this. As usual, in programming, there's many, many ways.
[43:23] We just have to find the way that's the best way for us today.
[43:28] So there's always trade-offs and all that. But--
[43:32] I think that's a big part of the paralysis, too, is it's like, if you start learning something
[43:38] and you're like, OK, so this teacher is showing you how to do it, yet they're talking at you
[43:42] because it's recorded. It's not virtual where you can learn with them.
[43:46] It's very difficult, because when you go to Google things, then they're like, oh, you do it this way, this way, this way.
[43:52] And it's not always-- at least from a beginner's standpoint, I'm just like--
[43:57] I don't know what you just said. I get that it might be a different way,
[44:00] but I don't know why and what it meant compared to what this specific lesson is talking about.
[44:06] Yeah. And that's-- I think that's one of the biggest
[44:09] challenges when you're self-learning, is understanding the why.
[44:13] And once you understand the why, then you can figure out, OK, this is the same thing but in a different way
[44:18] because of x, y, z. But if you don't really get that why just yet--
[44:23] and the most difficult part is to learn why we're doing things a certain way--
[44:29] then it's tough. And that's why I do prefer there are learning groups and things
[44:37] like that where people learn these things together, like in peer learning and all that type of stuff.
[44:44] I would recommend that type of things, not only does it help you motivate yourself,
[44:48] but it also gives you that peer support, peer feedback, and all that when you run into that type of questions.
[44:55] And it's really hard to Google answers, like why is this done this way?
[44:59] Why did this person on YouTube say this and not the other way that I saw on a website?
[45:06] And for the newbies that are listening and watching, feel free to hit me up and join me on one of these
[45:13] because I'll just hopefully hope the guest is OK with it and learn with me because, again, I
[45:19] think it's great idea what you just said of learning as a group because this may click with someone else that
[45:27] as they're saying it or as they're asking a question, I'm like, oh, dude, that does click.
[45:32] So I really appreciate it. It is something I do have a question, though,
[45:37] because when I was learning about JavaScript and the const, it used the squiggly bracket instead
[45:45] of the square bracket. Does that make a difference?
[45:49] It does make a difference. So let's look at different types of variables.
[45:58] So we can also have number of websites, and that is now four. So that's a number variable, and then we
[46:14] can do websites title, my favorite websites, and this is a string variable.
[46:25] So variables are something that you can refer to in many places in your code so that you don't have
[46:40] to write my favorite websites every time you use that word or that string or this number.
[46:48] And you can put anything in them. What is it called again?
[46:52] And I know I feel it's a really simple term, where specifically in JavaScript, I don't know if it's in other languages,
[47:00] that you type the first word lowercase and then instead of a space, the second word is capitalized.
[47:06] I think this is called camel case. Yes, that's what it's called.
[47:10] Thank you. And Python uses snake case, for example.
[47:19] So different languages have different preferences. OK.
[47:25] That is good to know as well. Most languages doesn't really make a difference.
[47:30] Some languages does, but yeah. Those are kind of conventions that you notice.
[47:35] You have it in languages, but then also when you go into frameworks, the frameworks
[47:39] have their own conventions about certain things. Not necessarily how you capitalize things,
[47:47] but maybe sometimes even about that. So for example, React components usually
[47:51] start with a capital letter. Oh, gotcha.
[48:00] OK. Yeah.
[48:03] But yeah, you were asking about squigglies. So maybe I'll show that quickly.
[48:14] So here's an object that holds more than one variable inside of it.
[48:30] And I think now is a good time to actually figure out what is a console.
[48:36] So while we're programming, it's sometimes hard to see what is inside which variables and where.
[48:42] So one way of doing debugging and understanding what's going on in your code is to do console log statements.
[48:49] So logging out what's happening in your code. So if you look underneath the white part of the page
[48:56] where you can see the web page, it says console. And it has a few notifications there for you.
[49:04] Let's see. There we go.
[49:07] And click that open. Clear those ones out of there.
[49:10] Those are, again, related to the environment earlier when we had trouble with the link.
[49:15] So you can clear them from the stop. Is that like a stop sign or something?
[49:20] Next to where it says filter. Oh, yeah.
[49:24] OK. There we go.
[49:26] And then the problems are-- this was another thing that kept coming up.
[49:31] It's not assigned a value, but never used. Yeah.
[49:37] Is that something that's kind of a clear message or-- It took a lot of Googles.
[49:44] And what I came up with is-- so what was it called?
[49:53] Log? Like guest?
[49:59] Console. Oh, yeah.
[50:01] So write console.log. And that is a function call.
[50:08] Console, let me jump in here. Console.
[50:11] So that's how we refer to that. Console.log.
[50:14] And then-- And then it was like--
[50:16] Yeah, there you go. Guest.
[50:19] There you go. And so it got rid of the one that's for guest.
[50:24] But I guess what I don't understand is when-- during the lesson that I was taking,
[50:32] it was like at the very beginning, the favorite websites, you could still look the right click
[50:40] and inspect it and see it. Yet as time went on, those were no longer--
[50:46] it just gave the error of never used. And I'm like, why was it working,
[50:51] and now it's not working? Yeah.
[50:54] I can explain what is it trying to say. I'm not sure what happened there like before.
[51:03] So in this case, the problems area is giving you helpful hints that you don't have to follow.
[51:11] Like nothing breaks if you don't follow. So it's OK that we're not using this variable right now.
[51:19] It's just giving kind of like a hint for us that we're doing something that doesn't kind of make sense.
[51:27] So we are assigning variable website title, but then we're not using it anywhere.
[51:33] OK. In this case, now guest is being used
[51:36] because we're at least logging it out. It's not being printed anywhere other than in the console.
[51:41] If you look at that now instead of the problems, you can see it now has the guest there.
[51:46] But at least the code now realizes that you're not only declaring a variable, which
[51:51] is what we're doing here on lines 5, 12, 13, and 15. We're declaring variables.
[51:57] So we're saying guest now holds this data. Got it.
[52:03] If we just declare that and never use it, why did we declare it?
[52:06] That's basically what it's telling us. OK.
[52:11] So it's kind of like, hey, you know that Microsoft Word used to have that paper
[52:17] clip that told you helpful things back in the day, and then it became a meme?
[52:21] That's kind of what's happening here. It's like, hey, I noticed you're doing something,
[52:25] and I'm going to help you a little bit. And that's why we have those yellow squiggly lines
[52:29] under those three variables now. So if you hover over them, you should see the same message
[52:36] there. Oh, cool.
[52:38] Yeah. So much learning.
[52:42] So much learning. OK, cool.
[52:44] Yeah. Click into the console underneath the page.
[52:46] So you should be able to see the guest there just to make sure that everything's working.
[52:50] That's the problems. And then the console.
[52:53] There you go. So now you can see that the guest is there.
[52:58] So when something's not working, it makes sense to try to console log things
[53:02] and see if things are doing what you expect them to. Got it.
[53:09] All right. So I created a new element inside the websites,
[53:23] and inside the index HTML. So I created a couple of new ones there.
[53:38] So let's first put the title in there using JavaScript, and then we'll put the websites underneath that.
[53:44] And I think that could be our goal for the day. OK.
[53:50] So would it be something kind of like the document that we did earlier for reading it because it's from HTML?
[53:58] Yeah. So now we want to hook into what is already in the HTML,
[54:02] just like we were doing before with the get element by ID and all that, and then the inner HTML.
[54:10] OK. So we called it websites title.
[54:15] We would want to do-- we're going to find out if I do this right at all--
[54:20] document, but get-- ah, lowercase. Yeah.
[54:27] Get element by ID, websites, dot title. No, dash.
[54:41] Dash title. Yeah.
[54:43] Title. And then dot inner HTML.
[54:51] I can click that. Make sure it's right.
[54:57] Equals. And then I would copy and paste this one down there,
[55:04] or I would put this above that one. Now we've declared already the variable, right?
[55:12] Now we want to use that variable. So in order to use the value inside that variable,
[55:19] we refer to it with its name, websites title. So that's what you would write here.
[55:25] You would just put websites title. So now that is the ID of the element.
[55:39] But we want to refer to the variable on line-- is that line 13?
[55:45] Oh, OK. Yay.
[55:54] There you go. Awesome.
[55:56] So now we are doing a couple of things here, if we maybe do a little recap,
[56:01] an unpack of what's happening. So we're first getting the website's title element
[56:06] from the HTML. And then we are assigning something to the inner HTML.
[56:14] And that's the website's title. So now we're using that variable that we declared earlier.
[56:22] Let's say you don't want the word "my" in there. How would you go about that?
[56:25] You don't want it to say "my favorite website." You could say "Jen's favorite website," for example.
[56:29] I believe it's editing line 13, because that's Jen. Yay.
[56:38] And see how fast it's already on the other side of your screen? Immediately, once you start typing there,
[56:47] it appears on the right side. And then-- oh, go ahead.
[56:54] Yeah, I said we have a comment on YouTube. Somebody is asking if this is a private class.
[56:59] Can I stay or leave? Please do stay.
[57:02] And you can ask us questions, see what you want to do. This is definitely something that's open for everyone.
[57:11] Yeah. Thanks for joining.
[57:13] Happy to have you here. That's why we are doing this online on YouTube.
[57:19] We are also on Twitch, right? Yeah.
[57:23] I should probably double check and make sure the rest of them don't have comments.
[57:28] I don't see any on Twitter. And I don't even know on LinkedIn how to look at it.
[57:38] I don't know about LinkedIn either. Well, just anyone on LinkedIn, maybe find us on Twitter
[57:44] or YouTube to make sure that we actually reply to you. That's right.
[57:49] OK, I'm not seeing any comments there either. OK, let us know if you have more questions later on,
[58:01] because we'll be doing this with all sorts of teachers and guests and going through, yes, very basic things right
[58:07] here, because I'm a complete noob. Yet, as the channel grows, we will be going
[58:13] into more complicated things. Abdul, do you have a topic that you're looking to cover?
[58:19] Yeah, I mean, today we're just getting started. This is the first time, right, for you to do this.
[58:30] So that's why we're looking at Code Sandbox, because it's kind of--
[58:34] I love it. I think it's a really great way to get started,
[58:38] because you immediately see what you're doing. And that is just magical.
[58:43] I think that is one of the reasons I've always been excited about programming, even when I was a little kid,
[58:52] because I was able to see what I was doing. Something changes.
[58:55] I write a piece of code, and something changes. I change a number.
[58:59] Now a color has changed. It's always been very exciting to me to see that visually.
[59:07] Well, thank you, Abdul, for stopping by to say hi. And if any questions come up on this or future ones,
[59:14] please hit us up and let us know. We love suggestions for topics, because this is number one.
[59:22] Now, so if I wanted to do favorite websites instead of-- so we're-- OK, words.
[59:34] We use document.getElementById for website's title, which is in the HTML.
[59:41] And we're using website title, the constant website titles. So if I go back, I'm going to go back to HTML.
[59:52] And you created one called Websites. Yeah.
[59:57] That is not a header, because H1 is header 1, right? That gives a bigger font, which is also another thing.
[60:06] Y'all, you'll probably need to go look that up at some point. But those ones, I feel like, are a little easier
[60:12] to use, because Google Docs does it, Word Docs do it. So I'm just going to copy that entire line.
[60:20] And it's called Websites. And--
[60:25] Oh, and something's already there. Yeah, because I didn't delete the item.
[60:31] So now I have to do Favorite Websites. Different?
[60:39] Oh. So how would I put those line by line
[60:46] instead of next to each other? Yeah.
[60:49] So let's first look at what was the tag that I used. So that was a UL tag.
[60:57] And if you wanted to know, you see a tag that you've never met before.
[61:02] Like, who is this? What goes inside here?
[61:07] Google, of course, is a great resource. But when I Google anything about JavaScript, HTML, or CSS,
[61:14] I look at something called MDN Web Docs. So what I would Google is MDN UL.
[61:22] What MDN UL? Yeah, space between the MDN and UL, yeah.
[61:29] OK. So MDN is Mozilla Developer Network.
[61:34] And that is a very comprehensive set of documentation about web technologies
[61:39] by Mozilla, creator of the Firefox browser. Oh, very cool.
[61:44] OK. So that explains what is a UL, Unordered List Element.
[61:51] OK. And inside that, it wants LI elements.
[61:58] So if you look at what's inside there underneath-- Oh, we need to do LI in front of each of them.
[62:04] Yeah. And it'll show us what it is for HTML
[62:08] and then what it is for CSS. Yeah, so here's some styles.
[62:13] They've applied a little bit of custom styles into this example. That's why there's the CSS.
[62:19] OK, so it's LI. So that means up here I would do the LI, right?
[62:24] Let's see. I don't know.
[62:27] I'll try it. I don't know if it'll work.
[62:29] That will not work in this case. And it's almost how you would do this in React, but not quite.
[62:40] So that's not going to work. If we think about what's going on here
[62:43] and why it doesn't work, like we talked about before, the why is always useful for future learning.
[62:50] So this is just a JavaScript variable, right? OK.
[62:55] So what we write here is JavaScript. And this is a list of websites.
[63:01] And by default, the way it renders a list of websites or an array in this array of websites,
[63:09] it puts them as strings and then a comma in between them. But we want to do something different.
[63:19] Now, I'm not sure if this is really like a day one lesson thing to teach.
[63:29] I've never tried teaching somebody programming in this way.
[63:33] But let's try. I think you might understand what's
[63:37] kind of happening here when we go about this. - Groovy.
[63:43] - Let's put a little bit of line breaks here. And then let's first put just 0.
[63:51] Let's see what happens. - Oh, it does the first one.
[63:55] Oh. - And then the second one and the third one.
[64:05] So this is the way we index into an array. So we pick out which element from the array we want.
[64:14] Now, in this case, we want all of them. But we don't want them to be just a comma-separated list.
[64:22] So in order for us to define how it looks like as a string, we use a method called join.
[64:33] And if we now put comma and a space here, it's not quite what we were looking for, right?
[64:44] But it's getting better. You can see something's changing.
[64:49] - Mm-hmm. - However, we want it there to be li-elements.
[64:59] Let me think. I've got to think about--
[65:13] so that would be a simple way to make it into strings. But now we want to make--
[65:19] we've got to use something called a map. And this defines how each single element is rendered.
[65:31] So instead, we want it to be li. We'll actually use backticks, because then we
[65:45] can do something called string concatenation. We can put variables inside here.
[65:54] Let's see if this works now. There we go.
[66:04] - Where is the comma coming from? - So the comma is actually-- yeah, that's--
[66:09] - Oh, I see it. It's up above.
[66:13] - It's coming from-- it's not that-- yeah, that comma--
[66:16] - It's not that. - We need that comma there, because that's
[66:19] how we define the variable. But it's coming because now we could maybe inspect.
[66:31] I can explain why. Because-- let's see.
[66:35] Let's actually pull this out of here. And we create another variable.
[66:44] This is kind of how you would end up doing debugging very often when you're coding.
[66:49] So you create another variable, and you maybe log it out and see what's in there and what's happening there.
[66:54] So const list is now this. And then console.log that list.
[67:05] And then we have to put a list in here as well. And now if you go into the console,
[67:11] you'll see what's there. So what's happening is it's taking
[67:21] each one of these favorite websites that we have in that variable, favorite websites,
[67:27] and it's wrapping that in li tags, right? - OK.
[67:31] - That's fine. That's great.
[67:33] That's almost what we want to do. However, because we are modifying the inner HTML,
[67:42] and if we put a list of things, like this has four elements. It still has 0, 1, 2, 3, 4--
[67:49] 0, 1, 2, 3 in it, right? It's not just a string.
[67:54] Like HTML itself is just a string. There's no lists in there.
[67:58] It's just a string of elements that are next to each other. So now we join it with nothing in between.
[68:05] Or we can do, let's say, a line break in between them. And now we hit Save, and the commas are gone.
[68:16] Because-- let's move this join over here. And now if you look at the console,
[68:25] you see it's rendering something different there. So it's not rendering a list of elements anymore.
[68:31] It's not 0, 1, 2, 3. But it's rendering a string that has those list elements in it.
[68:41] And I think that was a lot in ones. Maybe we'll unpack and see if you
[68:47] have any questions about this. - I think it's something that I--
[68:53] apparently, I'm just going to start doing some homework for myself off of all of these.
[68:57] Because what we went through definitely does make sense. And I think it's going to be something that
[69:07] is going to be where-- seeing it multiple times in a row,
[69:12] like seeing it from different people. And that's a big reason why having different guests,
[69:17] I think, is going to be great. Because I know for myself, it's like I can hear it
[69:22] from seven different people. But it's not till the eighth time
[69:25] that I realized my mom was right when she told me when I was six.
[69:29] And it's the type of thing that hearing it just repetitively-- I will say that I followed along probably
[69:37] until we made it pretty. But it makes enough sense that I think
[69:44] if I were to start my own project, I could do my favorite--
[69:51] as homework for myself, I will do my favorite podcasts and list them out and share that as my live learning
[69:59] as a follow-up on this one. Because it's definitely something
[70:02] that I feel like is going to take some practice. Yeah, absolutely.
[70:07] And we already went-- like I said, this is not a day one thing that usually gets
[70:16] taught, I think, when you start learning. So I think we're going really, really far here.
[70:24] So yeah, Abdul has a question. So the map method will return on array,
[70:30] and then we'll join all the elements in one string using the join method?
[70:35] Yeah, that is a very succinct way of putting what's happening.
[70:39] So you could actually look at what MDN says about JavaScript map.
[70:46] I think that is the best way you can get a little bit more into it.
[70:49] So there's-- yeah, there's search there. Map goes through an array, and then we
[70:56] can modify each element of that array, and then it returns the modified version.
[71:05] So that's why it still was an array. We went through an array.
[71:08] We went through each element of that array. We did something to each element.
[71:13] So we wrapped it in the li tags on both sides. And this is not what we're looking for, though.
[71:20] Yeah, I looked for map, and it didn't have it. So I'm just going to go back.
[71:23] Oh, write array.map, because it is a function on the array prototype.
[71:32] Oh, yeah, array.prototype.map. So if you go back, there you go.
[71:36] It's the first one now. Oh, OK.
[71:38] I wasn't even looking at it. Yeah, this is so popular, it was immediately first one there.
[71:44] And that's why I also decided we should use this, even though it's the first day.
[71:48] Because this is one of the basic things that you will be doing with arrays, for example.
[71:53] Yay. And a big thing.
[71:56] OK. Well, I will be working on doing this again, probably
[72:03] on sometime this weekend or on Tuesday, of figuring out how to do everything we just
[72:10] did as using a podcast list. I'm totally going to be cheating and using our code again.
[72:18] But it's definitely something that needs practice. And you did teach me a lot.
[72:24] So let's see if I can recap it well. We started with Codesandbox.io because it allows you to code,
[72:32] and then you can see it on the right side. So it gives us an instant visual, where something like--
[72:39] is it called Visual Studio, what people call VS? That one doesn't always give you the instant view.
[72:46] You have to actually have it open in the browser. Yeah.
[72:49] You have to have it open in the browser. And that's a little bit extra on top of this.
[72:55] And if we-- just for kicks and giggles, so people see the difference.
[73:00] And I really appreciate what we did. From using the Codesandbox, I was
[73:08] able to see that this is the temporary website of what we're building.
[73:12] So I went in to-- typed it into my browser.
[73:16] And I'm able to view it here, just like I did it in the other box.
[73:20] But I can go in and inspect it, like I was having to do with-- and click Console.
[73:27] And then I was able to see it like I had to do with VS. Yet this is saving me so much more time.
[73:33] Yeah. And this is a really easy way for us
[73:37] to do a multiplayer on a stream like this. It's possible inside VS Code as well.
[73:41] But I love how easy it is with Codesandbox. Definitely.
[73:45] And then, OK, so we went through. And on style.cs, we did create a button.
[73:52] And we were able to see that we could change the colors. And then on index.html, that is where our HTML lives,
[74:01] unless the JavaScript file is calling the HTML. But we originally deleted that.
[74:09] But then we recreated it on line 22, and making it so that way we could have the headers
[74:22] of Jen's favorite websites. And then also putting it in a regular font with line 26.
[74:31] And the part that I'm going to get a little messed up for, but I get that for we did the document.getElement
[74:45] by id.websites.innerHTML. And instead of having it be const list, which
[74:53] is where we did all the fanciness of making it look pretty, we could have done favorite websites again,
[75:00] which I'm just going to copy and paste this really quick to make sure I got this right.
[75:05] We can. It will paste.
[75:07] It just will not look pretty. And that is what I'm going to try on my own,
[75:15] is creating all of this again with it looking pretty, because that is something that is outside
[75:22] of the beginner wheelhouse. And I think that would just be fun to learn
[75:26] and see if I can duplicate it. Yeah, I'm looking forward to that.
[75:30] I think you're going to have a teach gen tech website up and running real soon.
[75:38] Yay. And thank you again for joining us and getting us all started.
[75:44] And for Abdul and everyone else listening, make sure to follow--
[75:51] I'm going to say your name wrong again. Why am I so bad at names?
[75:55] Yare? Yare.
[75:57] Yare, Yare. Thank you, Abdul.
[76:01] And make sure you follow Yare. And we are just starting, but you
[76:08] are welcome to re-watch this stream. We will have more streams next week with different guests.
[76:13] So you might be a little late for here, but make sure to tag us on Twitter
[76:18] or grab us on any of the other comments. And we'll make sure to see if we can get you your answers.
[76:25] And if you do that, please tag a time frame, a time code. So that way we can go and see exactly
[76:31] what you were asking about. But we are ending today's.
[76:35] And thank you so much for your time. Yare, is there anything else you wanted to go over before we go?
[76:42] No. I'm glad you're already thinking of what you want to do next
[76:45] and how you want to go about this. One thing I want to see when you've done this,
[76:52] make them links. Make them clickable, because we did
[76:54] go through how links look like. Go for that.
[76:58] That's like a rich goal right there. Yeah, it was a pleasure.
[77:04] Happy to be here, and looking forward to maybe teaching something else later on your journey,
[77:11] and having people join us, and having good chats, and figuring out how we can learn together.
[77:19] I think I just have to say, because I'm on YouTube, like and subscribe.
[77:23] Yes, like and subscribe. And we will eventually be going through Python as well.
[77:30] So give us a few weeks. I'm probably going to be focusing more on JavaScript,
[77:33] just to wrap my head around it. Yet we will definitely be having guests on about Python,
[77:38] because that is such an important language. If you hit either one of us up on Twitter,
[77:43] we may be able to put you in touch with someone that is really good with Python as well,
[77:49] and open to coming on a little sooner rather than later. And our Twitter names--
[77:58] me and Twitter just don't get along, it's hard to say. Our names are linked on our videos too.
[78:05] All right. Thank you very much.
[78:07] Thank you. Bye.

