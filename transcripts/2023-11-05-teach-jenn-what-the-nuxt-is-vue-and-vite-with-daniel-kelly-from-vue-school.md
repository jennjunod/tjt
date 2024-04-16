---
showLink: "https://www.youtube.com/watch?v=IG1i9bmfp_4"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-what-the-nuxt-is-vue-and-vite-with-daniel-kelly-from-vue-school"
title: "Teach Jenn What the Nuxt is Vue and Vite? with Daniel Kelly from Vue School"
publishDate: "2023-11-05"
coverImage: "https://i.ytimg.com/vi/IG1i9bmfp_4/maxresdefault.jpg"
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

[00:00] Another episode of Teach Gen Tech. This is an exciting episode as, I don't know if y'all knew,
[00:07] I've emceed five conferences with Vue School. - Like a lot of conferences.
[00:15] - It's a lot of conferences in the last year. And you and I have done Vue Forge together,
[00:22] or is it Vue Forge? - Vue Forge, that's right, yeah.
[00:25] - Yeah, yeah, yeah, together for two over the summer. And we've been planning this
[00:30] and we're finally doing something for Vue School. So Daniel, who are you?
[00:36] What is Vue School? - Hey, Jen.
[00:39] So my name is Daniel Kelly, first of all. I am the lead instructor at Vue School.
[00:46] And what we do at Vue School is we produce video content in order to teach people about Vue.js
[00:54] and the Vue.js ecosystem at large. So everything surrounding Vue.
[00:59] And yeah, it's a really great, really great program. Of course, if you like to learn by video,
[01:07] we have courses that walk you through all that. - Yay, and that is a great explanation of it.
[01:15] And what up, Alex? Now, I am curious about specifically,
[01:22] because these are ones that I really liked where there's, now I have to count.
[01:28] I can do this. Four main conferences throughout the year.
[01:32] It's Nuxt Nation, Vue Nation, and then two Vue Forges, right?
[01:37] - Yes, yes. I think you know that better than I would.
[01:40] (both laughing) - Well, and if I understand correctly,
[01:44] of course, Nuxt Nation is about Nuxt. Vue Nation is about Vue.
[01:51] And then Vue Forge is actually workshops. Like two-day workshops.
[01:55] - Yeah, Forge is really different, actually. It's less of a conference
[01:59] and more like you said, like a workshop. I like to explain it kind of internally to people
[02:05] as a glorified workshop. I mean, it's really cool
[02:11] 'cause the attendees get to get hands-on. We have like exercises that they can do.
[02:17] And then we have professionals within the industry live code the solution to those exercises.
[02:22] So you get a feel for what the experts would do for such things.
[02:27] So it's pretty cool. But we also have just like a conference.
[02:31] We have a live stream. We have sponsors.
[02:35] We have all these other conference-like things that are intermingled with it.
[02:41] - Yes, and thank you. Okay, so the most exciting part.
[02:47] What the Nuxt is Vue and Vite? - Ooh.
[02:50] (both laughing) - Okay, so that's a loaded question, right?
[02:55] Well, let me start off just by very high level comparing the three, right?
[03:02] So very, very high level. They are all related, right?
[03:07] Because you see them at all the conferences and then Vue conferences.
[03:10] So they definitely are related, but they're distinctly different.
[03:13] So Vite essentially is the build tool that allows you, number one,
[03:20] it's kind of got two responsibilities. It allows you to start up this development server
[03:26] on your local machine with all the goodies in there, right? Things like the hot module reloading.
[03:31] So your previews can be shown live as you're editing, but also things like converting your TypeScript files
[03:40] into JavaScript, because the browser doesn't know anything
[03:44] about TypeScript, right? So at the build pool level,
[03:47] it's doing these kinds of activities, like converting your files to things
[03:52] the browser understands, and doing things like hot module loading
[03:56] and things like that. So that's Vite's job.
[03:58] And then when you run npm run prod or whatever the case may be to bundle your stuff,
[04:04] it's going to do things like minify your code and still take those TypeScript files
[04:10] and those files that the browser doesn't understand and turn them into files the browser does understand.
[04:15] So like even your .vue files, right? So all that kind of stuff is Vite's responsibility.
[04:20] Then Vue is the JavaScript that actually runs in the browser, right?
[04:30] So if you did any jQuery back in the day, I did plenty of it,
[04:35] Vue is kind of like the jQuery, just stick with me, don't hate me for that statement.
[04:41] Vue is like the jQuery, not in that the interface is at all the same.
[04:46] The API for jQuery and Vue are completely different, but it's what's going to handle
[04:50] that interactivity in the browser. Like this is the JavaScript
[04:52] that actually runs in the browser, right? And the whole difference between Vue and jQuery
[04:59] or vanilla JavaScript is just that it has a different API. You interact with the DOM differently, right?
[05:07] So you're not doing document.querySelector and then selecting a DOM element.
[05:11] Instead, you're using Vue's templating system in order to interact with the DOM element.
[05:17] And under the hood, it's actually doing that document.querySelector stuff,
[05:20] right? It's doing all that vanilla JS stuff under the hood,
[05:23] but it just provides this nice declarative syntax for us to do it in a more intuitive way.
[05:30] So Vite is the build pool, Vue is the code that runs in the browser.
[05:35] It's the JavaScript that runs in the browser. Nuxt is what's known as a meta framework
[05:41] built on top of Vue. So it uses Vue as its templating language.
[05:47] So you write all of your pages and things like that in your Vue templates, right?
[05:52] But it does several different things. The main one though is it renders this stuff on the server.
[06:01] So by default or just out of the box, Vue is nothing but JavaScript
[06:07] that gets sent to your browser and then your browser renders the stuff
[06:12] that Vue tells it to render, right? So if I were to look under the hood
[06:16] of just a vanilla Vue page, you'd see probably like a div tag with the idea of app
[06:23] and an empty body for the most part. That's it, right?
[06:27] Because Vue is just a JavaScript that runs and it inserts all that stuff into the DOM
[06:33] after JavaScript is finished running. So this isn't great for SEO.
[06:40] A lot of crawlers expect the content to be there inside of the HTML, right?
[06:45] Now, some crawlers can render JavaScript or run JavaScript and then crawl the page
[06:53] and things like that. But for the most part,
[06:55] you want your content to be in the actual HTML that's sent down from the server, right?
[07:02] - Right. - So that's kind of where Nux comes in.
[07:04] Nux actually renders that stuff on the server side. All the stuff that Vue would have done in the browser,
[07:09] Nux just does it on the server, sends it to the client,
[07:13] and then Vue takes over and does kind of the same thing inside of the browser.
[07:16] That's known as hydration. So yeah, that's kind of a high level difference
[07:23] between the three. That's a lot at one time.
[07:26] - It is, it is, but it is helpful. And I didn't want to interrupt too much
[07:29] because I was like, there are questions behind them and also comparisons that came up.
[07:34] I'm also curious to everyone watching like what you y'all use,
[07:41] 'cause I know at least those who are in the OSRG Discord, they almost all use TypeScript.
[07:48] I know that, which is cool, but I don't know if they all use React or what they use.
[07:55] So I'm a bit curious. So y'all please put that in the chat.
[08:00] And also, so one of my very first videos with, oh my gosh, wait, what?
[08:11] Oh, I'm reading Jason's reply. And I'm like, it made me think
[08:20] that you went to go have Taco Bell breakfast. And I'm like, Jason, that doesn't really seem like something
[08:25] Jason like posts on Twitter about like waking up at like 4 a.m. and have like so much done.
[08:30] And I'm like, there's days where I'm barely getting out of bed.
[08:33] Granted, I have to wake up that early too, but I would be very confused.
[08:37] - I don't know that I've seen 4 a.m. in a very long time. That's, whew, no thank you.
[08:42] - It comes early. It does come early, but okay, cool.
[08:45] That's good to know. So Jason's React.
[08:47] One of the first streams I ever did was building a React app on,
[08:56] and deploying with Vite and Vercel. So saying that out loud means
[09:04] that I used the framework of React and then Vite helped build everything
[09:12] and then it deployed on Vercel. - Yes, yes, exactly right.
[09:16] And so like while you were developing on your local machine, what allowed you to see your app
[09:20] in the browser was Vite, right? And then when you hit deploy to Vercel,
[09:25] when you see all those little logs that Vercel prints out and things,
[09:28] that's Vite working to build the project from your source code.
[09:33] Do you always need Vite? 'Cause my other experience is like working
[09:38] on building an Astro site and all that comes to mind is npm run build.
[09:48] And Astro just does its thing. So when we're doing something in React and Vue,
[09:54] it doesn't auto do the build with npm build? - That's right.
[09:59] Under the hood, it's using some kind of build tool. And the two popular build tools are Vite and Webpack.
[10:05] So yeah, you may not be using, I don't know what Astro uses.
[10:10] I think it is Vite. But it could be Webpack or it could be straight roll up
[10:17] or there's several build tools out there. But that requires basically anything
[10:22] that the browser doesn't understand out of the box, like Vue files or TypeScript files
[10:27] or you need that build tool in order to convert it. - Interesting.
[10:32] This is really helpful piecing it together based on like past streams and different pieces.
[10:38] 'Cause I think that's where I personally got really confused with what is Vite and what's the use of it.
[10:44] So that one is making sense. And so Astro-
[10:49] - Well, it's even more confusing, Jen, to be honest. I mean, like that is the main job of Vite, right?
[10:56] Is to like transform these files that the browser doesn't even understand.
[10:59] That's its main job. But because it exists at that build level,
[11:03] there's so many other little things you can plug into it, right?
[11:05] Like you can do things like optimize images with it. You can do things like, oh, I don't know.
[11:12] Basically anything that you wanna transform a file in some way, you could do it at that point.
[11:18] So there's all kinds of little applications that you can, not apps, use cases that you can have for-
[11:26] - Yeah. Okay, that makes a lot of sense.
[11:30] Now, my next like thought process, and I know you said you'll show us a few things,
[11:36] but just on the theory-based side of things, is because React is so popular
[11:44] and like somebody getting into coding brand new, like first off, like when people first get into
[11:52] like becoming a developer and coding, A, there's always so much to learn no matter what,
[11:57] but also it's like one of the first things I hear from newbies is, "Hey, what should I code in?
[12:03] Should I do Python? Should I do JavaScript?
[12:06] Should I do C++?" So they not only have to like figure all that out,
[12:10] but if they go with JavaScript, it's like, what free? - Yes.
[12:14] - So it's like an added one. So are there like off the top of your head,
[12:20] do you know what the major differences are between like, you mentioned it a bit earlier,
[12:24] but like Vanilla and I'll use React because it's so popular, but that and with Vue,
[12:33] like what the biggest differences are there? - Sure.
[12:37] I mean, so your biggest differences between, let's start with Vanilla JavaScript and Vue.
[12:45] So your biggest benefit with using Vue over Vanilla JavaScript is that you get this,
[12:51] what's called a declarative syntax. So essentially you weren't having to write
[12:57] document.querySelector and then choose your DOM element and then live in JavaScript world separately
[13:03] than HTML world, right? So in Vue, you've kind of mixed the worlds together
[13:08] where you can do your loops inside of the HTML. You can put your event handlers inside the HTML.
[13:15] You can do your conditionals inside the HTML. And it's called a declarative syntax,
[13:21] but it's basically just easier to think about. And so the downside with that is that
[13:29] you are going to have a little bit more complexity overhead in terms of getting that stuff to the browser
[13:39] because you aren't, if you're using just Vanilla JavaScript,
[13:44] then the browser already understands all that, right? But the browser doesn't understand your .vue files.
[13:49] So you have to use Vite to transform your .vue files into regular Vanilla JavaScript,
[13:55] and then the browser can understand that. So, but Vue,
[14:02] I threw Vite in that sentence, and I know you're like, what?
[14:06] - No, no, no, but that's like, no, no, no. I feel like that just started to click so many things
[14:10] because if it's a build tool that people are using, it's taking all of the frameworks to use it.
[14:18] Whatever framework, a build tool would put it back into Vanilla.
[14:21] - Right, right. That's essentially the idea.
[14:24] - Okay. - Yes, I taught Jen something.
[14:30] That's the name of this, right? - I feel like that is something that probably clicked,
[14:35] but okay. Y'all, I've been doing this over a year,
[14:39] and that just really helps. So thank you.
[14:41] Please continue. - Yeah, absolutely.
[14:43] So in terms of Vue versus React, it's really just a, you know,
[14:49] it's just a choice each individual developer makes, I think.
[14:54] There are a few major differences, like React uses JSX,
[15:02] while Vue uses the .vue files, the Vue single file components.
[15:07] And it's really just, at the end of the day, it's just a personal preference
[15:13] because a lot of the things are the same. - Okay.
[15:17] - So, you know, I mean, Vue came after React. It, you know, was able to learn
[15:23] from what React did in the beginning, and I think makes some really nice decisions
[15:28] that really kind of make it more intuitive to use. But yeah, at the end of the day,
[15:32] it really comes down to personal preference. React is obviously huge, right?
[15:37] I mean, that is a big benefit for React. There's more resources for React.
[15:41] There are more jobs available, honestly, for React. But Vue still has a really great resources
[15:49] and job potential as well. So it is a little bit smaller than that.
[15:52] So it just kind of comes down to really what your personal preference is.
[15:57] - I am very well-trained with the conferences because I was about to say,
[16:01] and go check out Vue jobs, because that's where, if you're a Vue developer,
[16:05] I'm like, oh my God, we're not in the conference right now, y'all.
[16:08] I really like the way you said that, and I think that's a great way to also talk about,
[16:16] this is something that I've wondered since I started with MCing with Vue School,
[16:21] is like, so why is Nuxt called Nuxt? And they said, from what I understand,
[16:26] it's because Nuxt is for React, so Nuxt is for Vue. And I like the way you mentioned that,
[16:35] how Vue developed and learned from what React had already made.
[16:40] And a great call-out that I think is a big reason why I personally suggest
[16:48] when people are looking into new languages or getting into tech, like which way they need to go,
[16:54] is what is around for tribal knowledge? So in my, like the Discord I hang out in most OSRG,
[17:06] majority of everybody uses React. So, and they use TypeScript,
[17:11] which has made it a lot easier for me to learn because that's what they use.
[17:16] Where with like Vue, now that I hang out with all of y'all too,
[17:20] and like go to the courses and stuff, it's easier to learn it
[17:24] because I'm around that network of people. - Yeah, this is very important
[17:29] when you're learning anything. I mean. - Yes.
[17:31] - Yes. (laughs) - Now, so that being said,
[17:38] can you go a bit more into what a meta framework is? So I'm getting, okay.
[17:45] So we can build like a framework and using like Vue, and then we have our build tool
[17:51] that turns it into regular JavaScript or vanilla JavaScript. And then you can deploy it on something like Vercel
[17:59] or Netlify, and that's what makes it go on the web. - Yep.
[18:03] - With like a meta framework, we talked a little bit before stream about what,
[18:11] can you just go over what a meta framework is and I'll ask from there?
[18:17] - Yeah, absolutely. So a meta framework is like a framework
[18:22] built on top of a framework. So these guys saw, hey, Vue is awesome,
[18:27] and we like what Vue does, but we don't think it does quite enough.
[18:29] We wanna make it do a little bit more. And so there are several different benefits.
[18:37] To Nuxt, the primary one though is the server side rendering aspect of things.
[18:44] So Nuxt was, or excuse me, Vue was primarily just a UI thing, right?
[18:56] So in other words, it allowed you to create a beautiful UI that had nice reactive elements,
[19:02] things that, it was easy to make an interface where there's a lot of user interactivity.
[19:08] But all that just happens in the client. So an app is made of more than just a client,
[19:15] it's also made of what's happening on the server as well. And so what Nuxt does is it combines the two,
[19:22] combines this wonderful interactivity on the client, and then it does some of those same kind of things
[19:28] and more on the server. So you're getting your HTML rendered from the server.
[19:35] So the browser receives content, like it actually receives something inside that HTML.
[19:41] It's not just an empty diff tag somewhere. But you also get things like server side API endpoints.
[19:48] So a lot of times when you're working with Vue, you're making requests to an API to get your data, right?
[19:55] A lot of times, some people where I used to work, we used Laravel to power that API.
[20:04] So we're making a request from our front end, our Vue app was a completely separate app
[20:10] than our backend API. But with Nuxt, I can do that in the same project, right?
[20:18] I can have my API endpoints actually defined inside my Nuxt project,
[20:23] and my front end defined inside my Nuxt project. So this is really nice.
[20:28] And it also allows Nuxt to do things like actually automatically type my API responses.
[20:35] So when I'm making a request to one of my internal API endpoints
[20:40] that I defined with Nuxt, in my IDE, my browser,
[20:44] my IDE knows what the payload looks like. So it can do things like autocomplete.
[20:49] It can do things like error check. Yeah.
[20:53] So other things like that are really nice. But yeah, it's also got a lot of conveniences built in,
[21:01] things like file-based routing, which means you just set up a file
[21:05] in order to create a route, instead of manually having to create your routes
[21:09] with a JavaScript mapping of, hey, this route goes to this file,
[21:13] this route goes to this file. It just has some conventions around
[21:16] what file matches what route, and allows you to just create the file, and that's it.
[21:22] It does other little things in there too. - Okay, this is,
[21:27] since we're talking to them all differently, which this is so helpful,
[21:31] I don't think I've looked at this stuff like a year to actually re-review the fundamentals.
[21:36] And I like to say fundamentals instead of the basics, 'cause these aren't basic things to comprehend.
[21:41] They are difficult to comprehend. Fundamentals, they're part of the beginning.
[21:45] So is, can you mix meta frameworks across different frameworks?
[21:54] So could Nuxt go on React? Like, I feel like I know the answer to this,
[21:58] but I'm gonna ask it anyway. - No, the answer is no.
[22:02] - Okay, cool, great. I'm glad we got that one figured out.
[22:08] Now, just 'cause we're also on these different stages of a framework, a build tool, and a meta framework,
[22:17] gonna throw you one for a loop. What is TypeScript?
[22:20] - What is TypeScript? - 'Cause it's not a meta framework.
[22:24] - That's right. - And I wanna hear how you would explain TypeScript
[22:27] with all of this. - I'm gonna go the safe route
[22:29] and quote the TypeScript website. I think they say they are a superset of JavaScript,
[22:36] I think is the term they use. But basically all it means is they are,
[22:43] anything you write in JavaScript is valid TypeScript, right? So underneath TypeScript is just JavaScript,
[22:52] but it's got an additional layer of the type system layer on top.
[22:57] So I don't know, the relationship is a little fuzzy, but essentially it just brings that type system
[23:03] to JavaScript. But that's why you need something like V,
[23:06] because the browser doesn't know anything about TypeScript. It's really just for your ID, yeah.
[23:13] - Okay, that's cool. And (laughs)
[23:17] Sarah, thank you for joining. And yes, so really quick on catching up on that.
[23:27] Sarah's husband, Chris, has been on the show before to talk about databases.
[23:33] So, and Sarah is part of our, we play a live streaming tabletop game called The Expanse.
[23:42] And Sarah is in that. And it's really funny because like if I see Sarah,
[23:50] like her username is not that. And then her user, like her, like character name is Maria.
[23:57] So every time I see her, I'm like... - What do I call you?
[24:04] - You have a name. And the same goes for Bumpy Lumps.
[24:06] He's also part of that tabletop game. And his name's Alex and his character's name,
[24:15] now I'm gonna space your character's name. I don't, I don't remember Alex.
[24:19] - I'm really sad, actually, that his parents didn't name him Bumpy Lumps
[24:22] because I don't know, that would just be amazing. - Yes, yes.
[24:28] And yes, Jason, I just wanted, I did link it in there for what the View School stuff was
[24:37] because they do have like everything, like from beginner to super advanced.
[24:44] This is something that they just, so they have Mastery Nux if you wanna do,
[24:49] because Nux 3 came out last Nux Nation in '22. And then they also have,
[25:00] what's, Pina, Pina just came out. Mastering Pina, which, what is Pina?
[25:08] - So Pina is a state management system. So if you're familiar with React,
[25:13] you could think of it as Redux. Redux is the React version of that.
[25:19] - Okay, I'm gonna not dive into that one. We'll have you on again.
[25:24] We'll just like, we'll deep dive on that one. But yeah, they have a lot of different levels
[25:29] and just, honestly, y'all, I just wanna say, since I've emceed so many of these,
[25:35] I also remember way more about them because they also have the View Certification,
[25:43] which I was like, that's cool. I didn't know that that's a thing.
[25:46] It is a thing, you can get certified. Also just telling you, 'cause it's all great resources.
[25:52] And they have trained me very well. - We've got you promoing us well, don't we, Jen?
[26:00] - Like not even meaning to, like not even, it's just like in my brain now.
[26:04] So now that we've kind of gone through all of these and thank you for helping me break down
[26:10] the fundamentals there, can you show us a bit of like what something would look like?
[26:18] Just like a basic deployment of a Nuxt app and then maybe what it would look like
[26:24] for the differences if you are a View app and if you use Nuxt or don't use Nuxt.
[26:29] And then also maybe what a build log looks like. So like, do people know that they're,
[26:35] like if I am building something in View and I'm like, okay, cool.
[26:38] I'm gonna go deploy this on Vercel. Am I gonna get blocked somewhere to know
[26:45] that I can't build without using VEET? - Sure. - 'Cause if I'm using,
[26:51] oh, Anthony, look, okay, sorry, y'all. Anthony's here.
[26:54] And Anthony was the one who had me build a React app on VEET and Vercel to confuse me.
[27:01] (Anthony laughs) - Thank you for doing that, Anthony, that's,
[27:07] we wanna confuse Jen, it's a goal. - Yes, yes, but Anthony, I'm finally following up
[27:11] to understand that, we'll see, let's see if I got the explanation to Anthony,
[27:17] 'cause he's been on Teach Gen Tech way too many times, or not enough, is that VEET is the build tool
[27:25] that takes any, and it can work with any type of framework to build it, to build the framework
[27:34] and then turn it into vanilla JavaScript so it could deploy on something like Vercel or Netlify.
[27:40] - Yep, that's the gist. - Yes, okay.
[27:44] See, Anthony, like I knew what, I knew VEET did something, I just couldn't understand why,
[27:50] especially since, Anthony, when you and I did our stream, it was like using React,
[27:58] and I built my site a few times with Astro, so I didn't really understand why,
[28:05] what VEET did in the middle, and why there was a build tool,
[28:09] because Astro just auto did it, so this is making a lot more sense,
[28:13] and Daniel's gonna show us some stuff. - Awesome.
[28:16] First, before I show you something, Jen, I do want to just mention, so the Mastering NUX course,
[28:24] if you are already familiar with VUE, I think the Mastering NUX course is a really great next step,
[28:30] it's taught by Michael Thiessen, he is huge in the VUE community,
[28:35] he taught me a lot when I first started working with VUE, and he's a really great teacher.
[28:42] If you're brand new to VUE, I don't suggest jumping into NUX necessarily right away,
[28:47] because you really need to get the basics of VUE first, but for someone who's brand new to VUE,
[28:53] we do have some really great courses on the actual VUE School platform that are VUE fundamentals,
[29:00] and a couple of those are even free, so I suggest you check out that
[29:03] if you're interested in starting with VUE. - And I just want to add to that,
[29:07] because I love how when the course first came out for Mastering NUX, so y'all, this is a year ago,
[29:15] for those who have been following me for quite a while, I don't know what any of this is,
[29:19] or who's who, or anything like that, and Michael Thiessen is very level.
[29:24] - Very. (laughs) - That's the best way I can say it,
[29:27] and you guys can tell him I said so, because he is, and then he came out with this video,
[29:31] and he's so excited about it, and I'm just like, I feel like I need to listen, 'cause what just happened?
[29:39] - That's great, yeah, I get that experience, I totally get that.
[29:44] - So thank you, that was a great call-out of going through the differences of them,
[29:50] but yes, anything else you want to add to that one? - Nope, nope, that's it for the resources there.
[29:57] Yeah, Jen, let me see if I can, so I'm gonna pull up a next site, give me just one moment.
[30:05] - Yeah, for sure, and yeah, Anthony, I didn't realize that until like,
[30:11] okay, yes, you've probably said it before, Anthony, and I call Anthony my internet big brother,
[30:16] because he's come on, I think he was my second or third episode, I don't remember at this point,
[30:25] and so, and he's been on the stream so many times throughout there, that helps fill in the gaps,
[30:32] so he just became my internet big brother, and it's been fun learning them,
[30:37] and then referring back to them, and be like, do these actually all connect?
[30:41] And actually having it sync in now, so. All right, let me get this on stage.
[30:48] Bam. - Awesome. All right, y'all, so this is the new Nuxt documentation
[30:55] they just released at this Nuxt Nation, which is pretty cool, so what I'm gonna do is,
[31:01] I'm gonna copy their bootstrapping command here, and open up my terminal, and just paste that in,
[31:10] and I'll just call my project teach gen tech, right? That's what we're doing.
[31:16] - But it's two N's. - Oh, it's always two N's, Jen, no, it's too late.
[31:23] - It's too late, we committed. - I'm gonna change your name now.
[31:26] - Dammit. - Okay, cool, so that's booting up here,
[31:33] and then we're going to open it in Visual Studio Code as soon as I get it open, so just a quick explanation,
[31:42] I'm gonna show you kind of what I mean by the server-side rendering.
[31:48] So this is gonna kind of show you the difference between a vanilla Vue project and a Nuxt project.
[31:54] - Adding to that question that you reminded me of a question I had earlier was,
[31:59] could you go over an explanation of like, when somebody says server, and then you have client-side,
[32:08] like what's the difference between the two? Like what's the, I know I've asked this question before
[32:13] for everybody that's been here for a while, but you know, sometimes you have to ask like seven times
[32:17] for it to say again. - Yeah, absolutely, so your server is the computer
[32:22] that the person deploying the website owns or is renting or whatever, right?
[32:26] So it's your, it's Netlify servers, or it's Versailles servers, it's Versailles computers,
[32:33] which probably under the hood is actually Google's computers.
[32:35] I don't know, but that's probably it. So the server is everything that exists
[32:41] outside of your user's computer, essentially. And it's the place where you can do things safely,
[32:46] it's the place where, you know, you can talk to your database,
[32:49] it's the place where you can store secret keys and all that, because your users never see that.
[32:53] The client is just the browser, that's all it is. Yeah, the client is just the browser.
[32:59] Or in the case of a, you know, an Electron app or a desktop app,
[33:04] maybe it's the app shell or whatever. So yeah, does that make sense, Jen?
[33:10] - Yes, yes, and this is probably one of the biggest things that I never get why, like tech in general
[33:20] has so many different names for things. And it's like, why don't we just call it the browser?
[33:25] We have to call it the client. - Right.
[33:27] - Please continue, this is just a rant I have about. - No worries, no worries.
[33:32] I mean, the reason they call it the client is because you could have other clients, right?
[33:37] You could have other things receiving the stuff sent from the browser.
[33:40] So like if I did curl and then I curled the next website, like in this case, my terminal would be,
[33:51] or I guess curl would be the client. But I can visit that same website in the browser
[33:56] and then the browser is the client, right? It's kind of weird, but yeah,
[34:02] you can have different clients. But the one that most people are using is the browser.
[34:06] Okay, so I started my project, right? So teach, yeah, there it is.
[34:14] So we're gonna open that up. And let me show you, let me get my presentation mode on here
[34:21] so I can, y'all can see a little bit better. - Yeah. - There we go.
[34:29] Okay, so what am I looking for? Let me start the dev server.
[34:36] So I'm gonna install everything with NPM. So to throw your one more difference in there,
[34:46] NPM is that other layer, right? That's your package manager.
[34:48] - Ooh, let's get really complicated. What's the difference between like NPM
[34:56] and then why am I blanking all the other ones right now? MPX or those other ones?
[35:03] - Yeah, so NPM, Yarn, Bun now, right? - That's what Bun is?
[35:11] I haven't paid enough attention to it. That's good, that's good to know.
[35:14] - Well, Bun is, yeah, it's more than that actually. Bun is a whole JavaScript runtime,
[35:19] but it has the package manager built into it, which is kind of cool.
[35:23] - And the package manager just installs all the things you need to use to make one of these projects.
[35:30] - Yes, exactly right, exactly right. Okay, so now I'm gonna start the development servers
[35:37] with NPM run dev and this is Vite working its magic, right? This is Vite putting that little development server,
[35:44] giving me the URL and then bundling all the, or compiling all my non-browser ready files
[35:52] to be browser ready. - Cool.
[35:55] - So then I can visit this in the browser and you're going to be able to see now
[36:03] kind of Vite in action. So let's look at the network tab, reload my page.
[36:09] - And y'all let us know if we need to zoom in more, please. - Absolutely.
[36:14] Let's see, welcome to the next, oh, I'm, here we go. So all the things.
[36:20] So there is a welcome component. And so you can see over my code in app.view right here,
[36:29] we have this next welcome component. Okay, this is a view component.
[36:33] So it's a file that ends in .view. It's not in my project, it's in the dependencies.
[36:38] So I'm not gonna go find it, but you can see here, this welcome.view file that my browser has loaded.
[36:45] So yes, it ends in .view. However, if you look at the content type here,
[36:53] we've got application JavaScript. So my browser is not reading the .view file,
[36:58] it's, this is just pointing, this is just to help me know which file
[37:02] this is actually talking about. It's reading the compiled file that Vite made for me.
[37:08] So Vite turned my .view file into a JavaScript file. And if you look at the response,
[37:14] like, this is not what I'm having to write. Like, I'm not in my IDE writing this crap,
[37:20] because that would be a nightmare. This is what Vite is creating for me, okay?
[37:25] So-- - Got it, okay. Is it possible to edit that then?
[37:32] Like, if I were like, hey, we're using this template, I don't, I like it, but I don't like it,
[37:37] I wanna go edit the template. Where, would I just delete the template
[37:42] and then start from scratch? Or would I, can I go edit the template somewhere?
[37:47] - Yeah, yeah, I would definitely go edit. So, like, this next welcome here comes from,
[37:54] at, shoot, how do I search this? At next, where are you?
[38:03] Is it at next here? - Yeah, so at next, probably UI templates, something?
[38:09] I don't know. - Yeah, so there's ways to go in there,
[38:15] and that's good to know. I was very curious about that one.
[38:18] - Yeah, yeah, yeah. Probably even a better example would be
[38:21] if I did a new directory here called components, and then I just did a, just a hello world component, right?
[38:28] So I did hello world.view, and then I would do a template of h1 hello world,
[38:36] something like this. And then I could just put that here
[38:40] instead of the next welcome. So hello world.
[38:44] Okay, so this is the exact same thing, just somewhere inside of next package,
[38:50] it had something like this, right? And so now you can see, this is, here's that,
[38:55] yeah, let me refresh. Oh, this should be hello now, yeah.
[39:03] So you can see, yeah, here's hello world.view, but under the hood,
[39:07] this is what the browser actually gets, okay? - Sweet, really? - I'm not writing that.
[39:12] - Really quick, I'm gonna pause you because we just got rated.
[39:15] Thank you, Jason. If y'all don't know who Jason is,
[39:19] it's Learn With Jason, Jason. Because for some reason, I never say Jason's last name.
[39:23] I don't know people's last names. I know their Twitter handles or like their projects.
[39:28] And so thank you everybody for joining. We are currently hanging out with Daniel from Vue School,
[39:35] learning the fundamentals of what the next is Vue and Vite. And we're currently seeing how Vite is the build tool
[39:48] that uses, that changes any type of framework to a vanilla JavaScript and showing us an example
[39:57] of how that shows up in the browser or the client side instead of the server side.
[40:04] Which the server side is the computer you're building it on. The client side is the browser for the most part.
[40:12] - For the most part, Jen. The server side is the computer you're serving it from.
[40:16] So I'm not necessarily serving it from my actual personal laptop.
[40:20] But if I deploy it to Vercel, they're servers or whatever. - Got it. - Yeah.
[40:25] Cool, cool, cool, cool. Thank you.
[40:27] - Cool. Jason, by the way, I've seen some of your stuff, man.
[40:31] I really like, I really like some learning with Jason. - Yeah, like I wanted to name it.
[40:37] Like I was gonna be like, maybe I should change my name or like start my show to be Learn With Jen.
[40:42] And I was like, no, there's Learn With Jason. So instead, since he gave me like the idea of it,
[40:47] I just said, "Hey, Jason, will you come teach Gen Tech?" And he did back when he worked at Netlify,
[40:52] which was awesome. - Awesome.
[40:55] Very cool. So yeah, so that's, I mean,
[40:59] that's the gist of what VEET is doing for you. - Very cool.
[41:03] - It's taking those files and transforming them. And I'm so glad I don't have to write this, right?
[41:09] - Yeah, like how do a lot of people end up writing that? Like, I guess. - No, nobody ever.
[41:17] No, no, no. - I was like, that would be a lot.
[41:21] - Cool. Yeah, what you would do, Jen,
[41:23] is you would come and edit this file and then you would need to make sure you have VEET
[41:27] transpile the file for you. So I couldn't just edit this
[41:31] and then send it to the browser. You would need to run your build step.
[41:34] - Okay, okay, that's making sense. - Awesome.
[41:38] Okay, so that's kind of how VEET plays a part. Let's talk about the difference now
[41:42] between VUE and NUX and show you that. So I'm not gonna start a brand new VUE project
[41:49] just for the sake of time, but I am willing to turn NUXT's SSR setting to false.
[41:55] So what this means is that I want my NUXT app to behave basically like a VUE app at this point.
[42:05] I want it to not do the server-side rendering, okay? So just imagine now this is a plain vanilla VUE application
[42:13] and for this demo, it essentially is. So if I do VUE page source,
[42:19] you'll see there's really nothing yet. - Can you zoom in a bit for us on this one?
[42:23] - I can, yeah, absolutely. - Sweet, thank you.
[42:25] - Better? - Yeah, thank you.
[42:27] - So there's really not a whole lot going on. And more importantly, if I look for my H1
[42:34] that said hello world, that doesn't exist in here. So the server didn't put that H1 tag into my HTML, okay?
[42:44] So, but I still have the hello world on the page. It's like, so what's going on?
[42:50] So what's going on is that the JavaScript is executing and putting the hello world in here.
[42:57] The HTML is just, where's the div? Just this div right here.
[43:03] This is where the JavaScript is. It's finding the div with the ID of NUXT
[43:08] and then it's injecting that into the div, which is fine for our end user, but for the crawlers,
[43:16] they don't necessarily always execute the JavaScript before crawling it.
[43:21] So like right here, if I go to, let's see, how do I turn off JavaScript?
[43:27] If I go to settings and then, where's JavaScript in here? Disable JavaScript, can I search this?
[43:37] Java, I thought it was in here somewhere. Ah, here it is, disable JavaScript, okay.
[43:46] So if I have my JavaScript disabled and refresh the page, yeah, you can see that the hello world isn't there.
[43:52] So it only exists in the JavaScript. Yeah.
[43:58] - If we have NUXT enabled though, even if we disabled the JavaScript,
[44:05] it would still be showing because NUXT will take it from that JavaScript into creating it as an HTML.
[44:12] - That's right, on the server. - Cool, on the server, therefore it will load faster
[44:19] because it's already been done on the server. - Yep, yep, and it does, the browser doesn't have
[44:25] to execute that JavaScript before it shows anything. Yeah, absolutely right.
[44:31] So I'll just disable that SSR fault. So now it's behaving more like a typical NUXT application.
[44:36] And now if I refresh the page, yeah, my JavaScript is still disabled, but hello world is there.
[44:43] And that's because it's in the, so here's the H1 and there's the hello world.
[44:50] So it's coming from the server. - So that's making sense on why that's like very important
[44:55] for like SEO and crawlers and things like that. What doesn't quite make sense to me is we've mentioned
[45:01] hydration and those types of things really quick before, if anybody wants a funny story of,
[45:09] we were talking earlier about my internet big brother, Anthony, he was like, hey,
[45:13] let's help you get more people on the stream. And he saw Mishko who created Angular post about that.
[45:20] He wanted to do streams, like to talk about quick. Fifth episode, fifth episode, Mishko comes on and he's like,
[45:28] he's like, hey, do you wanna like, do you like maybe like hacker news or something?
[45:34] And I'm like, what, that's a thing. So he basically spent the time like trying to explain
[45:44] what hydration is. And as I said, y'all episode number one of Teach Gen Tech
[45:48] was learning the differences between CSS, HTML, and JavaScript.
[45:52] So fifth episode being hydration, I was like, I don't know. - What is this hydration thing, right?
[46:03] - Yeah, so what is hydration and where does it go into all of these pieces?
[46:08] - So hydration is really just kind of the mixture of your view app on the client side
[46:13] and your view app on the server side. So Nuxt does its thing here, right?
[46:18] Where it renders it on the server, but with JavaScript off,
[46:23] so with JavaScript off, this is not really doing anything. Now I'm not actually doing anything inside the component.
[46:29] Let's do something like, I don't know, script setup and make it whenever I click the H1,
[46:36] we do an alert, why not? So I'm gonna define a function here called handle click,
[46:43] and then we're just gonna alert hello world, okay? And then we're going to call whenever we click this H1,
[46:54] we'll call handle quick, okay? With JavaScript turned off,
[47:01] this isn't going to do anything. I can click all I want and it's not gonna do anything
[47:04] 'cause we need JavaScript to handle event handlers, right? That's not something that can run on the server.
[47:10] That's something that only runs in the browser. But if I turn JavaScript back on and then click,
[47:16] we get the hello world. So the idea here is that this is the server side rendering,
[47:24] is getting that content into the HTML. The hydration is going and actually putting
[47:30] the interactivity kind of back over that regular old HTML. So we're actually getting the whole Vue app
[47:39] is up and running in this browser now. And because the whole Vue app is up and running,
[47:46] it can listen to the click and I can do things on the client side.
[47:49] I hope that helps. It's not super clear, but yeah.
[47:56] - You know, I think we'll get there. I think that is an added thing,
[48:00] like asking about what is TypeScript. But this is starting to make a lot more sense,
[48:07] like refreshing on the fundamentals and seeing how it actually works in action.
[48:13] Is there somewhere where we can actually see a bit more about what V does and the build tool?
[48:23] - Sure. - And how it builds things? Is there a way of seeing that
[48:27] or is it just like magically behind the scenes and you don't get to see any of it?
[48:30] - I mean, a lot of it's happening behind the scenes. I imagine you could probably pass a flag here.
[48:36] Let's see, this is kind of where Vite's doing some stuff. Like so Vite server had HMR for seven different files.
[48:46] Yeah, I'm sure there's like a flag we could probably pass to it
[48:49] to see what all Vite is doing under the hood. To be honest, I don't know what it is.
[48:55] - That's fair. - You know what, let's try one thing.
[48:59] So Next is a TypeScript-first framework, which means configuring it is super easy.
[49:05] So like I can hit Control + Spacebar in here and just kind of scroll through all the different options,
[49:11] which is really nice. - Oh, that's cool.
[49:13] - So I think there is a Vite option. There is, then I can Control + Spacebar again.
[49:17] And let's see if there's a way to tell it to like print out stuff.
[49:24] Experimental JSON legacy log level maybe, or maybe is there like a dev?
[49:30] I don't know. Let's see what log level does.
[49:33] So log level, and then I'm just... See, this is the TypeScript helping me out.
[49:40] Like all I'm doing is pressing Control + Spacebar and it gives me the autocomplete, which is, I love it.
[49:46] Let's try log level info and see if that gives me anything more.
[49:52] Um, so if I make a change here, paragraph, I don't know. HMR update, eh, it doesn't look like
[50:02] I'm really getting any more info, but yeah. - This is making a lot more sense.
[50:09] And I mean, y'all, we have had Daniel go through so much. Is there anything else you want to show us
[50:16] that you think we need to review today? - Let me show you one more thing.
[50:21] Let me show you this built-in server API endpoints. 'Cause I think this was a big difference
[50:26] between NUXT 2 and NUXT 3. NUXT 2 did not have this, and this was a huge, huge thing.
[50:33] So if I go to the server directory here and create a folder called API, okay,
[50:42] and then create a, no, just do the regular. Actually, let me do that.
[50:47] So I chose new API because I have a extension installed that kind of knows the default NUXT file types and things.
[50:55] And it's able to give me some boilerplate. So, okay.
[51:04] So now I've got return, hello, Nitro. Let's pretend, let's pretend here that I, you know,
[51:12] I connect to a database. I fetch, you know, I fetch all the blog posts
[51:21] from my database or whatever, right? And then what I can do is once I have
[51:30] all those blog posts ready, so that can look like, you know, this is all my blog posts from my database.
[51:36] And I've got a blog post with a title of, you know, hello world, and then I've got another blog post
[51:43] with the title of, yeah, I'm super not creative with these, Jen.
[51:47] - It's okay. - I've said hello world so many times.
[51:51] - Hello, beautiful human. There you go.
[51:54] That's what I write. - Hello, beautiful human. - That's what I write.
[51:58] - I love that, Jen. It's a wonderful shout out to being human.
[52:02] And I really appreciate that. Okay, so here's all our posts.
[52:06] So now we can just return our posts. Like we don't have to JSON stringify it
[52:10] or anything like that. Normally, if you're sending something from the server,
[52:13] JSON stringify it. It's still being JSON stringified.
[52:16] It's just being done on the web. But now if I were to visit localhost 3000/API/,
[52:23] was it hello world? What was the name of the file?
[52:31] Yeah, hello world. Okay, I get my posts.
[52:37] And so this is just like a server, a JSON REST API, right? - Okay.
[52:42] - And it's super quick to boot up. But the beauty of it now is that I can interact
[52:47] with this API endpoint from my components. So here, let's say I want to display all the posts.
[52:54] Well, up in my script section, I would just make a request
[52:58] with the built-in use fetch composable. Hit slash, and oh, why is the autocomplete not working?
[53:06] That's the best part. Is my server still running?
[53:14] It is. Let me restart it just to be sure here.
[53:17] So it should autocomplete this route for me. - Okay, that, I mean, in general, is just like live coding.
[53:26] It doesn't matter. It's like, I don't care what you're doing.
[53:29] It's gonna cause issues. - Absolutely it is.
[53:32] - That's live coding life. - Let me try this one.
[53:35] No, why is it not doing this? Let me get rid of that and let's just,
[53:40] let's cross our fingers. If this doesn't work, then we're moving on.
[53:45] All right. Still no.
[53:47] See, okay. But anyways, we can make a request to that API endpoint.
[53:51] Okay. And then we can, oh, it looks like it started to do it then.
[53:56] My apologies, Jen. I'm gonna make it work.
[54:00] I'm gonna make it work. It has to work.
[54:03] Still not working. - You're good, you're good.
[54:06] - Okay. I will say that is something that I really am so grateful
[54:10] about people that have a lot more experience coming on the stream and then this type of stuff happened.
[54:16] Not like I want anything to happen to other people, but I think that's one of the biggest things
[54:20] that beginners have in their mind. It's like, yo, everybody just gets it the first time.
[54:25] So like this just like really does make it show others. Like it doesn't matter how much experience you have.
[54:31] - That's right. - It can still happen.
[54:33] It's coding. This is the world of coding.
[54:35] - That's exactly right. Exactly.
[54:37] Okay, so now I can get my data and I think it's coming out of here like this
[54:45] or like this is all my posts. I have to remember which one it is.
[54:48] Yeah, some of the autocomplete stuff isn't working. So I don't know why that is.
[54:52] But so now I would want to loop over each of these. Why in the world is going on right now?
[55:02] It thinks I'm inside of, oh, this thing is up here. I bet that was the issue.
[55:08] No, ah, goodness gracious. You're right, Jim.
[55:15] This is totally live coding. Okay, so now when I do the LOI
[55:19] and I'm just gonna actually type it 'cause apparently my ID is freaking out right now.
[55:22] So we can loop over each of those posts. So for posts and posts.
[55:29] And then we can just like print the title of the post, right? Post dot, and this is where I really wish.
[55:36] The TypeScript was working. Oh, it's 'cause I didn't say lang equals TS up here,
[55:41] isn't it? Post dot, no, I don't know.
[55:46] - They saw it working earlier. They know it's a thing.
[55:49] It is a thing, we saw it. Everybody, I know we saw it.
[55:51] We did see it working earlier. - We totally saw it.
[55:55] Okay, so now if I go, let's go back to the actual page here. And I've got lots of, so let me look at Vue.
[56:05] So these are the Vue DevTools. And now I can see what post is.
[56:11] Okay, so post is a promise. So that's cool.
[56:14] I didn't actually await for it to finish. Okay, so that's a little better.
[56:19] And now post is this data object here. It has data error, blah, blah, blah.
[56:26] So yeah, this should actually be some extracting data from the return of this.
[56:32] And that data is the post. So yeah, there are the posts there.
[56:36] - Yay. - Yay, so it works.
[56:39] But the biggest benefit here is that you get like the auto-completion and stuff in TypeScript.
[56:43] And posts dot, yeah, I don't know why it's not working right now.
[56:50] - How does that, wait. Alex just said the HTML templating syntax
[56:56] kind of reminds them of handlebars. - Yeah, it's kind of the same.
[57:01] So, I mean, this is one of the major differences between Vue and React is React uses the JSX
[57:08] and us Vue people do basically anything that's legit HTML like we can put in here.
[57:13] But then we have these little Vue directives that we add in that do the Vue stuff.
[57:18] - Oh, and Anthony said really quick, VS Code may be restarting it.
[57:24] You know, I feel like that's the default answer. Hey, restart it.
[57:27] Did you turn it off and turn it back on? - That's right.
[57:30] - The best answer. And just wanted to say, thank you.
[57:33] Is it McNeely ad? We're gonna go.
[57:38] - Oh, here it is. Here it is.
[57:40] - Also shout out to, thank you for Mr. Noly. - Thank you everyone.
[57:45] I appreciate the follows. - Okay, keep going Daniel.
[57:49] - Yeah, sorry. Sorry, I zoned out there for just a second.
[57:52] Reloading my thing and I think it's working now. Apologies, interrupting you there for the shout outs.
[58:00] - No, giving shout outs. Like I gotta make sure people hear the appreciation.
[58:04] 'Cause I think that's one thing like a lot of people don't understand
[58:06] is like how much like liking and following and like watching people's content
[58:11] is what makes the algorithm work. And also like, I love hearing ideas,
[58:16] which by the way y'all, think of questions that we need to ask Daniel
[58:20] on the next stream. So start thinking of those that you've seen so far.
[58:24] So we know what to ask him for a follow up. - Absolutely, I love those questions.
[58:29] So yes, I think it is working now, Jen. And this is really what I wanna show you.
[58:32] So yeah, see how it auto-completes my API endpoint? Like--
[58:37] - That is pretty cool. - It's really nice.
[58:39] And not only is the API endpoint auto-completed, but it knows what the return,
[58:45] it knows what the response is. So you can see here, it's a,
[58:48] I'm pointing at my screen like an idiot with my finger 'cause y'all can't see that.
[58:51] - You're good, well, we'll imagine. - So you can see it's an array that it's returning
[58:57] of objects that have a title property. So this is really cool.
[59:03] Like now down here, I can say post. And it auto-completes title for me.
[59:07] So this is a disconnect. Like if I was using a Laravel API,
[59:12] or just a completely separate API from a Nuxt project, I wouldn't get any of this,
[59:17] or I would have to manually type this stuff inside my project.
[59:20] Now, just based on the return of my endpoint, I automatically now on the front end
[59:26] know what the shape of that data is. And so I can, it helps not create errors.
[59:32] I can code more confidently. - This is pretty sweet, thank you.
[59:37] I think that's definitely. And yes, Anthony, I'm really glad
[59:42] that Redwood GraphQL API has always done this. He's a very, very big into Redwood
[59:49] and GraphQL at some point, I know that. Okay, Anthony, maybe you and Daniel can chat
[59:59] and we can do a GraphQL Nuxt stream. Like you got to talk to Daniel though.
[60:05] Like- - That would be cool. - Come on together 'cause he,
[60:08] Anthony's been wanting to come on the stream to talk about GraphQL for like forever.
[60:12] So we got to go baby steps. - My personal experience with GraphQL
[60:17] is I've used it some. And I really do like the, I mean,
[60:21] like you have that type safety across your backend and your front end,
[60:26] which is exactly kind of what I just did here, right? So GraphQL pioneered that essentially.
[60:30] Like they did that first, absolutely. I'm just always more comfortable
[60:35] doing like regular REST API calls. So this helps me as the one who's comfortable
[60:39] with REST API calls, get that same kind of functionality, which is really nice.
[60:43] But I can do it without a GraphQL piece, which makes me comfortable.
[60:47] - All right, all right, that's good to know. Very cool.
[60:53] Well, I like that you showed us that. And we also got to see how to troubleshoot
[60:59] those types of things when they don't work. I think that's always very helpful for all of us too.
[61:04] Now, is there anything else that we have missed that you want to go over?
[61:08] - No, I think that's about it, Jen. - Yay, all right.
[61:13] So y'all either like, also go follow Daniel and View School on all the social medias, they're everywhere.
[61:22] Really big on X, formerly known as Twitter. And if y'all want to see how awkward it is
[61:29] saying that during conferences, definitely like know that this is something
[61:35] I struggle with all the time. We have a weekly stream sometime on Tuesday
[61:41] between like a few hours earlier to now-ish. I haven't gotten great at nailing down the time yet,
[61:48] but yes, y'all come back. Thank you for following Calvin and y'all.
[61:54] Make sure to click follow and ask us all the questions that we should have Daniel on the stream again
[62:00] for View Next. I'm gonna volunteer you for V2 or Pina,
[62:06] or like we'll figure out one of those things we need to learn more about.
[62:09] And thank you all, let's see where am I spacing anything that they need to follow up with and follow y'all on
[62:17] that I forgot to mention. Okay, and do y'all wanna go to Finite Singularity
[62:28] or ending with Ali, I almost said Ollie, Ali, because both are really great streams.
[62:38] So see if we have any preferences before I hit the raid button.
[62:41] I'm just gonna surprise y'all. You're just gonna have a random one.
[62:47] - What's it gonna be? We don't know.
[62:50] - Oh, Treat Bot, you're here and I'm leaving, but yes. Okay, y'all really quick before I go through all of this
[62:56] and raid you, we're going to get like Skittles where you guys can like do things and get your points
[63:04] and I'm gonna get Skittles. It's gonna be amazing.
[63:08] And cause he made all these like machines. It's really cool.
[63:12] All right, we are going to raid and thank you everyone. [BLANK_AUDIO]

