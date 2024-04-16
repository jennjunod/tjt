---
showLink: "https://www.youtube.com/watch?v=iU2SLljSy-k"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-python-with-jay"
title: "Learning Python with Jay!!!"
publishDate: "2023-02-10"
coverImage: "https://i.ytimg.com/vi/iU2SLljSy-k/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome back to another Teach and Tech.
[00:08] Instead of learning with Laura Python, we have a new guest.
[00:13] >> I'm not new, I've been here before. >> Yeah, but you haven't been here for Python.
[00:18] >> Which is weird, because Python is what I do. It's funny because I've done two VS Code things,
[00:24] and both times I've had to preface with I just like VS Code, I use it, like yes,
[00:30] I get paid to talk about it from time to time, but ultimately Python is the space that I'm in.
[00:36] >> Yeah, and it's so funny because there's a specific people that I think about for Python,
[00:41] and you are one of them, and yet at the same time,
[00:45] you've never been on the show for Python until today. >> I'm happy to fix that.
[00:51] >> Let's see if I remember all the details about Jay. Not all the details, of course,
[00:55] but Jay is a developer advocate over at Microsoft and on the VS Code team?
[01:05] >> No, I'm on the Cloud team. >> On the Cloud team.
[01:10] >> Yes, I am a Cloud developer advocate or senior Cloud advocate, which our focus is mostly Azure or Azure products.
[01:24] With a little bit of sprinkling into some of those other spaces, like you said, VS Code,
[01:31] the things that you might use to develop things to go into Azure, but then also we're big proponents of open-source,
[01:38] so working to help create open-source projects, help maintain them when we can,
[01:44] and get more people involved in Python. >> What do you do in the Python world?
[01:53] That's really cool, and how you promote it? >> I do a little bit. Most of my focus is around community,
[02:00] so I wind up, I am one of the organizers for the San Diego Python User Group.
[02:07] I'm also the host of Python Community News, or one of the hosts of Python Community News.
[02:12] My co-host, John and I, we do a show once a month now.
[02:15] Used to be weekly, now it's monthly because weekly was a lot. We talk about the non-programming side of Python, the community.
[02:26] The Python community is one of those really weird things that people tend to not know as much about.
[02:34] It's like the iceberg principle where you're a Python developer and you see the tip of the iceberg,
[02:41] which is like the PSF, and PyCon US, and some of these other conferences.
[02:45] But what you don't see is this gigantic mass underneath that is like, here are all the other organizations that help make Python run,
[02:54] like the Euro Python Society, and the DSF, and Defna,
[02:57] and around the Django space, and all of these other communities that exist,
[03:02] and initiatives, and fundraisers, and there's a lot that happens.
[03:08] Since Python tends to be more, I guess, asking of community participation and community support,
[03:21] and it's very, very volunteer ran. Where some JavaScript frameworks
[03:27] will have an entire company behind them. >> I was just thinking that.
[03:32] >> Yeah. You don't get that as much. There are some, there's Anaconda,
[03:38] and a lot of the data science stuff, and even then that's very loosely based,
[03:42] and that some of those projects are like company-driven products. But a lot of those are even like,
[03:49] there's a non-profit like NumFocus that helps with a lot of
[03:54] the scientific community and a lot of those open-source projects. It's good to have something that talks
[04:01] beyond the code to help understand how all of these things are duct-taped together to make what is a very vast Python ecosystem.
[04:11] >> Thank you for that explanation. I think that is such a good point.
[04:16] When I first started coding and granted y'all, this is only like seven months ago,
[04:22] which is bananas to me. I'm like, "Yes, I'm doing this for seven months."
[04:25] >> That's awesome. >> Closer to a year now.
[04:28] I learned JavaScript because it was what was presented to me, I guess it was more like I asked people what I wanted to learn,
[04:40] what should I learn, and a lot of people said, "Python," if I wanted to go into data science.
[04:47] Other people said, "JavaScript," if you want to just be able to do everything.
[04:51] We're not even talking about the frameworks in JavaScript, just vanilla, and it was always like this thing,
[05:00] I knew about Python that I was like, but I want to learn Python.
[05:06] What up, Aaron? Hello. Aaron, what languages do you know?
[05:13] >> I know Aaron. Hi, Aaron. >> Yay.
[05:18] >> Aaron is one of the coolest people I've ever met in the tech industry. When it talks about learning community things,
[05:27] Aaron is the person to talk community with. >> Aaron is amazing. Thank you.
[05:35] I appreciate that. I actually never,
[05:38] I don't know if Aaron and I have ever talked about languages. >> If you ever catch Aaron out on the streets,
[05:44] just get her on a bird scooter and you'll have a blast. >> I am glad to see that Python is greater than JavaScript.
[06:00] Wait, what? We're going back. Yay. We're all the J people.
[06:07] I just take the first letter, like his name, and then I take that first letter and just keep it going.
[06:14] >> I like it. >> It works. What I was wanting to say though,
[06:20] really quick, is a lot of people have this idea that Python is only for data science. I've learned quite a bit about JavaScript because people are just like,
[06:31] "Hey, this is what we're going to do." I'm like, "Okay, this is cool, whatever."
[06:35] Where Python is what I'm learning from the bare basics of coding. Laura and I have been going through this book,
[06:46] which I will show here. Automate the Boring Stuff with Python,
[06:55] which is from Al Swigart. I believe that's how you say his name.
[07:01] We've learned a lot. I've learned how I learn better.
[07:07] Now we're going chapter by chapter, going through it, and Laura wasn't available this week,
[07:12] and Jay said he would come on. I'm very excited about this because,
[07:16] and knowing now that Aaron can too, we could just learn Python from everyone,
[07:22] just have different guests on for Python, which is fun. Aaron, you're funny.
[07:34] They let you on a bird scooter and supervise. You're uncoordinated. Yeah. I've heard that about you, Aaron.
[07:43] We had to get to food. I get that. Let's figure out how to.
[07:52] I don't know how to get people. Okay. It's going to stay there because I don't know how to remove it.
[07:57] I can't do anything on my side. Yeah. Please ignore the first-time chatter of Liz Bot,
[08:05] because I'm still learning how to block people. Let me go ahead and present my screen so we can go into the Python-y stuff.
[08:17] I'm going to go back a page really quick and post this here. Make sure that's close.
[08:29] >> Yeah. I second what Aaron is saying in the chat of like, automate the boring stuff is one of those books.
[08:35] I think that like what you were saying earlier, where like the Python community is so vast that people tend to
[08:42] forget that there are so many areas of Python. My journey into learning Python was somewhat centered around web development,
[08:57] but commercially, I was a horrible employee and didn't like sitting at my desk and working,
[09:05] so I just started automating all of my job. It was like, updating user accounts in Active Directory, automated.
[09:14] Sending out scheduled e-mails when we had little task things, I was like automated.
[09:20] My job was I had everything running into a spreadsheet of different things that needed to get done that day,
[09:25] that was automatically being pulled in from a help desk system. All the stuff that was really basic,
[09:33] like literally it just read the spreadsheet and then said, "Oh, well, there's a script that does that.
[09:39] Plug these values into that script, run. Now it's done. Now send that e-mail off.
[09:44] Okay, cool. Everything is done." I would just hit "Okay" and then walk around the building.
[09:50] I used to get in trouble so much because they were like, "Why are you not working?" and it was like,
[09:55] "Because I am working and it's easier for me not to touch my computer and let my computer do the work
[10:03] than it is if I'm not at my desk." Yeah, Python definitely is not just for data science,
[10:13] is not just for web development, is not just for back-end,
[10:16] is not just for all of those things. You can do a lot with Python.
[10:24] In fact, if you're just like, "I'm sure I could write a program that does this,"
[10:28] usually there is a way to do it in Python. May not be the fastest way, but there is a way,
[10:32] and it should be pretty fast. >> This is probably something I am most excited about,
[10:39] is Chapter 17 and 18. Because helping build communities
[10:43] and learning the back-end of that, I was like, "I just want automated e-mails."
[10:49] Yet you can only learn so much in different direction all at once. I'm very excited to be able to go through that later
[10:56] on and start building that out because it's something that I could see really does help,
[11:01] and you don't have to stick to one language. Aaron joined in.
[11:07] They started on the data side in data journalism, cleaning up datasets,
[11:13] now doing more app stuff with Python and some machine learning stuff which is new.
[11:20] Then they didn't even know until a year ago that you could build apps in Python.
[11:26] Not going to lie, I don't think I've seen too many apps yet. >> Usually when you're working with something like that,
[11:33] it is you are writing Python to a translation layer that writes it in some other host language.
[11:40] But you can do the underlying things in Python. A lot of the UI might be in some other language,
[11:49] but then it's calling your Python scripts to run in the back-end. As we talk about things like PyScript,
[11:55] PyScript allows you to just run Python in the browser. I want this Python code up on the screen,
[12:04] and I wanted to do Python things. It's not HTML and CSS,
[12:11] it is just full-on Python. To me, it's awesome and it's still really early,
[12:18] but we're going to see a lot of development and growth in the WebAssembly space for Python in the next few years.
[12:26] In fact, there are actually some Python enhancement proposals or PEPs which I'm sure you'll hear about.
[12:33] If you continue learning Python, you'll hear about the PEP system and all of that.
[12:36] There are a few PEPs out right now that talk about increasing support for Wasm WebAssembly.
[12:46] Kind of the same thing. I don't remember what all of the S and the M are,
[12:52] but WebAssembly is, when you hear Wasm, be thinking like WebAssembly in that case.
[12:59] >> There is a lot to break down there. First question that comes to mind is,
[13:09] and this is me not knowing my tools yet, and I call that out because Jay and I started late today,
[13:15] because I was asking a lot of questions about the learning processes.
[13:23] This is something that's pretty cool that we've been doing a lot with Laura,
[13:26] yet I'm excited that we're doing this with a ton of other people, is does DevTools tell you what language things are in?
[13:36] You just talked about being able to see it in the browser, and I'm like, I don't remember DevTools saying that,
[13:42] but I don't know if it does. >> Not right out of the box.
[13:47] There are extensions that you can use. I don't know if there is a PyScript extension, but.
[13:59] >> Because for example, I'm going to go to some random one I have.
[14:05] In GitHub, it will show you the languages people are using, which I have found really helpful.
[14:12] Yet, if I just go to inspect the page and go look at something, it doesn't really tell me that much.
[14:20] That's why I was curious if it's something like those can complement each other,
[14:25] or if it's something that there was a plug-in for. >> There are usually plug-ins.
[14:31] There's the React. That's the one that I always think of is React
[14:36] basically builds your website inside what's called a virtual DOM, or Domain Object Mapper thing.
[14:46] You can see the footprint or the fingerprint of those things in the HTML that it creates.
[14:56] When you are able to see those things, it allows you to be able to go and pull information from it.
[15:04] You do have extensions that'll say like, "Oh, this is built with Vue.
[15:09] I know this is built with Vue." I can then give you access to
[15:14] the layer that is Vue or the layer that is React, and use that as a way to pull that information out.
[15:21] Document Object Model. Thank you. I'm not a JavaScript developer.
[15:26] >> That's what JavaScript uses. Yet, is there something like that for Python?
[15:32] >> I don't know. I don't know entirely how. I put a link to the PyScript project.
[15:37] I'm not entirely sure how it's generating it, but I'm pretty sure there's some WebAssembly embedded layer.
[15:44] They have a Python runtime that's embedded in each page that it pulls from and then goes.
[15:51] But again, there's a lot happening with that. The next step in that space is how do
[16:01] you extract that and be able to show it to other people. But again, if you want to be in this area,
[16:13] this is a whole thing. This is the direction that a lot of active development is going in.
[16:20] How do we do more Python in more places? Again, I love how this is Python with JavaScript,
[16:28] a bidirectional communication between Python and JavaScript objects.
[16:31] You can write JavaScript and then pass out the results of that JavaScript into your Python and
[16:36] then do Python things with it and vice versa. Don't try to wrap your head too much around it.
[16:45] >> Well, it's reminding me of Bedrock. Bedrock does your CSS in your HTML.
[16:54] That way, and it just reminded me of that because it does the two together instead of.
[17:03] >> Okay. Y'all, I know that I am asking way too many questions and going off on a tangent,
[17:10] so to bring us back around. >> Really quick, Erin had some questions.
[17:16] >> Yes. >> You use Docker or a Jupyter Notebook or Kaggle when writing Python.
[17:22] GitHub is like, I'm not sure if you do Python things. Until I did a tech skills test with a recruiter,
[17:31] they're like, is there a way to make that more visible in GitHub? I don't really know.
[17:43] That's a good question. I think that there are definitely ways that you can take
[17:49] your project and if you're working in Docker, don't just have that image in
[17:57] Docker Hub and then the underlying code not in GitHub. Put that underlying code in GitHub,
[18:02] that way, people can see it. Now, if you're using someone else's Docker project
[18:06] and you're doing a bunch of stuff and they're running in that, honestly, that's more valuable than writing the Python yourself.
[18:12] You know what to write and what to let other people write for you, and I respect that.
[18:17] In terms of Jupyter Notebooks, this is the whole recruiter versus engineer type thing.
[18:31] If the recruiter is like, I don't see you do a lot of Python things and use it,
[18:36] say, I have all these Jupyter Notebooks over here that have Python in it.
[18:40] They're like, well, that's not Python, then just be like, it depends.
[18:46] If you know the engineering team, cool. Just be like, sure,
[18:50] whatever, I talked to so-and-so and this is a valuable skillset or this is a trait,
[18:55] or just explain to them that it is and if they, my guess is this is possibly a cis white dude that's like,
[19:09] yeah, I go to Python meetups all the time and it's like, yeah, I'm not here to bash recruiting.
[19:16] Recruiting is a job just as much as engineering is a job. They have their skillsets and they have the things
[19:23] that are blind spots in their skillsets, both of them. How do we get beyond
[19:33] those blind spots just so that we can get to the people that we want to be interacting with?
[19:38] >> Follow-up questions on this, and this is something that we talked about with Laura
[19:45] last time about Jupyter, Jupyter Notebooks. Y'all, again, I am still learning
[19:53] a lot of the theory of the coding first. It took me a while to wrap my head around Boolean.
[20:02] Just so that way you know where I am, I'm working on a lot of theory.
[20:05] I haven't done a lot on typing or writing it out. Would you not or could you not put
[20:18] your Jupyter Notebook on a repo for backup? >> Yeah, of course you can.
[20:27] You can absolutely take, if I have a Jupyter Notebook and I want to
[20:33] just throw the whole Notebook in GitHub, yeah, absolutely, you can do that.
[20:37] Actually, GitHub has a pretty good interface of presenting that. >> Great question from Fakai.
[20:50] I feel like I haven't seen you for a while, so I'm excited to see you back.
[20:54] Doesn't the source code of the Notebooks count as Python? Sounds like a GitHub bug, to be honest.
[21:00] >> I wonder if there is, yes, Ann. You may not actually want to include all of
[21:09] the embedded Notebook source code stuff into your repo, so that wouldn't be visible to GitHub.
[21:18] My guess is you would have a requirement.txt file that has all of the pip install Notebooks and all of that stuff,
[21:29] and you wouldn't want to include your virtual environment that has those Python libraries.
[21:38] >> How do Jupyter Notebooks back up then? >> Because it would store an actual file,
[21:48] and then when you run the Jupyter Notebook, it will just read that file and say, "Oh,
[21:53] I know how to present this inside of a Notebook." Because that's why it's an IPYNB file,
[22:02] like Interactive Python Notebook file. That file just has all of
[22:08] the markup that your Notebook "server" will read, and from there, it generates
[22:18] that visual layer that people are used to. It goes, "Oh, let me see this file.
[22:23] Okay, cool. Add some stuff." Then when you type into it,
[22:26] it writes to that file. If you've ever tried to look at an IPYNB file,
[22:32] it is definitely not just Python. It is like Python and a bunch of markup.
[22:41] It should even say, I'm pretty sure GitHub recognizes IPYNB files,
[22:49] and it says, "Oh, you do Jupyter Notebook things." From there, to me,
[22:56] if I'm looking for someone with Python knowledge and they see Jupyter Notebooks in
[23:01] your repo as the type of language that you're using, they should be able to look at that and tell like, "Okay,
[23:08] this person probably does some Python things." Not to say that you
[23:12] only do Python things in Jupyter Notebooks, you can do a lot of different languages in Jupyter Notebooks.
[23:18] But for the most part, Python tends to be the language that a lot of people use.
[23:24] If you're using something like a PYNB file, then you are 100 percent doing Python.
[23:30] Unless you're just doing all markdown or text, but it seems like a lot when you can just do that.
[23:36] >> You answered my question, but I don't think I said what I meant.
[23:41] >> Okay. >> Which is, if you're not backing it up a file on GitHub,
[23:47] does Jupyter Notebook back it up somewhere else like a GitHub? >> Oh, no.
[23:52] >> I guess, is it just saving it on your computer instead of backing it up somewhere?
[23:58] >> Okay. >> Yeah. I'm sure someone has some app somewhere that's like,
[24:08] "Oh, store all your Jupyter Notebooks here." But I'm not going to say GitHub,
[24:14] I'm going to say that is some type of version control system running in the background,
[24:20] specifically designed for scientific notebooks or Jupyter Notebooks. >> Okay.
[24:26] >> Yeah. >> It's not something that automatically happens.
[24:29] >> No. >> It's something that, okay.
[24:31] Cool. Because those who may not know Anthony, I like to call him my internet big brother, Campolo.
[24:43] I still call him Anthony AJC Web Dev. This is how I call him.
[24:52] That is his last name, not his official last name.
[24:57] With him being one of the first people that taught me about just process in general,
[25:07] he told me about going through and as soon as you're done with something, you upload it on as a repo and then you delete it from your computer.
[25:17] That's where I think I was just going like, "Wait, what? What's going on?"
[25:22] >> That's one way to do it. Yeah. I mean, storage is cheap.
[25:27] I have most of my projects still sitting on my computer somewhere, but I think the focus there is yes,
[25:35] have some form of Git layer, like some form of workflow that you use that puts
[25:43] things not just on your computer and gets them on GitHub. But of course, with that,
[25:49] there is also the do it in the way that's safe and also do it in a way that's not going to add a bunch of unnecessary components to it as well.
[26:04] You don't want, and then we talked about this like a Git ignore. You don't want your environment file with all of
[26:13] your keys and passwords and all of those things in there. You absolutely 100 percent don't want that.
[26:20] You don't want it to include every single piece of your Python virtual environment.
[26:28] Instead, you want just your code. Then if you have things like
[26:34] a certain environment that you want to enforce, you do something like a dev container that
[26:40] tells the person that's going to look at your code what they need and even give them a way to quickly add it,
[26:47] but doesn't include it in your repo. Otherwise, what you might be doing is every time you go to add something to GitHub,
[26:57] you're adding megabytes and megabytes and megabytes, and as things change,
[27:02] Git has to track all of that. Eventually, your project becomes this unwieldy beast that takes
[27:08] forever to load and get off the ground. Containers are, yeah.
[27:17] >> I don't even, what? Y'all, I get that we were going to talk about Chapter 2.
[27:23] We may not get to Chapter 2. I have so many other questions.
[27:26] >> We can do Chapter 2. We can get all in there.
[27:29] I can come back anytime and talk about all the fun stuff. >> Yes. This is something that I'm learning a lot.
[27:37] This is one of the difficult things with learning to code. It's also a lot of project.
[27:47] I'm calling it project hygiene. I don't know if that's the proper way of saying it.
[27:52] What do you do with your content? >> What are learning containers?
[27:59] >> Oh, sorry. Just containers. This is a topic that I am not prepared to talk about.
[28:09] >> I know. Aaron, what are you doing? Are you going to jump on the stream with us,
[28:13] talk about containers because I'm curious. >> Containerization is one of those things that you,
[28:21] I feel like at this point, you will learn. There are a few.
[28:30] Oh, I like that. It's like a mini space. It's like a mini space. Yeah. Think about that.
[28:37] Think about where you live. Think about your home.
[28:42] Your home has a bunch of different rooms in it that do different things.
[28:48] But they all have a few things in common. They have four walls,
[28:53] they have a ceiling and a floor, and probably a door so that you can get in and out of it.
[28:58] >> I'm going to go back to what Fokai said, but just to keep on the conversation we're going with.
[29:06] >> It's like a Sims neighborhood. I'm trying to keep the analogy really small here.
[29:12] >> But you don't want to fuck up the other Sims. >> Yes.
[29:16] >> I find this really funny because I never got into Sims. >> You should.
[29:22] >> I got so agitated at Sims, and so that's why I was like,
[29:26] this is really funny. But it's like a mini space,
[29:31] so let's go back to the apartment version or house version. >> Yeah. Think of an apartment or a house or whatever.
[29:35] A bathroom has certain things in it. It has a toilet, it has a sink,
[29:40] it has a bathtub or a shower. All of those things are included in a bathroom.
[29:47] Then when you get another bathroom, what do you do? You make sure that you have a sink,
[29:54] a toilet, maybe a shower or a bathtub. You don't have to think about like,
[30:00] every time I need a bathroom, let me go think about the concept of a bathroom from scratch.
[30:10] All over again, you go, no, these bathrooms are a thing, so we're just going to copy and paste bathroom, boom, there.
[30:15] Bathroom has been copy and pasted. That is ultimately what a container is in many cases.
[30:22] It is, if I have a Python project, there are certain things that I need for my Python project to run,
[30:29] and that scale. If I have a Django project,
[30:33] which is Django is a Python web framework, that I need to have all of these things for my Django project to run.
[30:41] If I have this web idea, this web project that is two databases,
[30:53] the web framework, the API layer, the JavaScript front end,
[30:57] those are five different servers that all have to run, and I now need to replicate that across to another project.
[31:05] I don't want to have to build all of that from scratch. Luckily, there may be a container already that has all of
[31:12] those things included that I can go, let me just grab that. Then that's there and I give it the things that do make it different.
[31:20] The wallpaper, maybe how the sink looks, maybe what you actually put in the cabinet.
[31:28] But ultimately, it's all the things that you needed to make this an effective space or an effective project.
[31:38] >> Yay. We will have content to follow up on. Thank you, Aaron. Rolling it back some of learning containers.
[31:58] We are still talking about containers like Docker? >> Yeah.
[32:01] >> Okay. Can you find containers that could be like
[32:11] a template like what you were just talking about? >> Yeah. That's your image.
[32:16] Docker requires you to create or pull from what's called an image, and that image is that template.
[32:26] You might say, I want to operate within a base image that is just Python 3.11,
[32:34] Alpine or Python 3.11. What's the one that we're supposed to use now?
[32:39] Bullseye. That is like, if you're developing and you just need a clean Python space,
[32:51] that is this image here and you just pull that image. >> Okay. Then when you're using containers,
[33:05] you don't need something like GitHub because the container is virtually backed up.
[33:12] >> I mean, it has to live somewhere. Docker Hub is a place and it is effectively
[33:22] like the space where all the Docker images that people decide to put there go to live.
[33:31] I want to call it the Docker Senior Community Center. That's just mean on me though.
[33:42] >> Okay. >> Yeah. You can store images in GitHub.
[33:50] There's a GitHub container registry. You can have your own special place for things like disclosure.
[33:58] Again, I work for Microsoft. My job is to promote Azure.
[34:02] If you have your own set of images that you want to be the basis for your big project.
[34:10] Think about how important this is for things like banking or businesses where you often
[34:19] are spinning up and tearing down servers because they need to serve a purpose.
[34:25] Hey, I have the "Big game" or whatever is coming up this week, and now you have all these companies that will
[34:36] put out commercials and they're going to go to a website. The website is going to crash because
[34:43] billions of people are going to go visit it. What you do is you have
[34:47] this scalable containerization project that is like the thing that serves my website is an image,
[34:54] and it is in this container. If I need more of those containers
[34:58] to serve that website to more people, I don't have to rebuild it all the time.
[35:04] I just say, "Give me another one of those,
[35:07] and then give me another one of those, or give me 15 of those."
[35:11] There are even technologies that you'll hear about eventually, like Kubernetes, that gets really involved in
[35:21] managing the adding and removing of those containers as needed.
[35:26] >> I was going to say, Aaron, I know you just said you're going to
[35:30] reach out to Jay for a collab, but when y'all collab at some point,
[35:38] it would be really cool for y'all. I have another person, Trevor,
[35:44] who does a lot of work with this too, it would be really cool if y'all could just write
[35:49] out or do a stream on Azure versus PowerShell, versus Kubernetes, versus Docker, versus AWS.
[35:57] >> What are these terms? >> Because aren't they all just server?
[36:05] Well, Azure and AWS are serverless, and then the other three are computers?
[36:12] >> No. Azure and AWS are just Cloud. Think of those as just Cloud providers.
[36:21] Ultimately, they do a lot of the same things. They might just do them different ways,
[36:27] and they're backed by different companies. Azure, obviously, is the Microsoft arm.
[36:31] >> What about Cloudflare? >> Cloudflare probably doesn't do as much as AWS or Azure,
[36:37] but probably does some similar things. Cloudflare probably gives you their CDN layer.
[36:46] They'll have some CDN stuff, which is for site reliability.
[36:50] They'll also have some- >> I'm learning that they do more than I thought they did.
[36:56] Because I thought they just did the CDN and I'm like, every time I've talked about one of these,
[37:00] one of the engineers are like, "No, it's also Cloudflare."
[37:05] >> Yeah. They do CDN, they do web hosting, they do DNS.
[37:09] They do a lot of those things. But when you look at something like an AWS,
[37:16] which has 200 some odd services, they do so many things, it's ridiculous.
[37:24] Azure as well. I focus on the quickly deploy Python projects in Azure,
[37:33] but if you wanted to go into other spaces of Azure, they totally exist. Also, most of
[37:40] these companies partner with other companies. If you want to have,
[37:44] I used to work at Elastic, that's where Aaron knows me from.
[37:47] If you want to host your Elastic infrastructure on AWS, you can do that.
[37:57] If you want to host it on Azure, you can do that. It's all the same product,
[38:01] it's just where that product lives. There are multiple ways that you can do that.
[38:06] You can go through Elastic's Cloud offering, that just focuses on what they do, and say, "Hey,
[38:13] let me do all my Elastic stuff over here, but store all of my stuff in Azure,
[38:18] or store all of my stuff in GCP, or store all of my stuff in AWS."
[38:22] Or you can go to AWS or Azure or GCP and say, "Let me spin up an Elastic Cloud layer,"
[38:32] and they'll do it that way too. That's something that I don't think you can go to
[38:37] Cloudflare and be like, "Yo, how do I get this entire application
[38:44] that's running Kubernetes on the back-end, but has been obfuscated so
[38:47] the end-users don't have to worry about that, and how do I put that on Cloudflare?"
[38:52] You don't. That's the answer, is that you just don't. >> I like this answer of Cloudflare has similar things,
[39:00] a very high focus on routing, CDN, proxying, but lately focused a lot on
[39:06] running your own projects on every server park. Yes, Aaron, I definitely want to go do things.
[39:15] But this hosting part, and this is something that took me a very long time,
[39:24] and added to this question that I probably shouldn't have asked, but I'm glad I did.
[39:30] Because I used to work at GoDaddy, so we did hosting there.
[39:36] It started to make sense, servers, all of that. But then you have Netlify and Vercel,
[39:43] and it's like, you can host things very easily? What? It's like, what?
[39:52] >> So think of all of these providers as often services that
[39:59] ultimately do the same thing but slightly different, and being really good at doing one particular thing,
[40:05] one or more particular things. AWS just has a lion's share of the space.
[40:14] So if you want to go work at a lot of companies, just understanding how AWS not even works,
[40:24] but the space in which you're doing your job, understanding how you do that in AWS
[40:30] is probably a thing that you should have some knowledge of. Then again, I think the more foundational knowledge you have,
[40:37] the easier it is to take that one thing and then go somewhere else.
[40:41] If you're talking about a Netlify or a Vercel, like Aaron said, a lot of Netlify and Vercel is,
[40:50] I have this JavaScript project or I have this static web app and I want to host it extremely cheap,
[40:56] or I have a very simple project that is doing a thing that I don't want to pay a lot of money for.
[41:02] So when you talk about Cloud providers, one of the things that becomes a challenge is,
[41:08] how do I set this up in a way that I'm not going to be spending hundreds of dollars?
[41:12] Because when we think about this, it's a scale problem. Azure has to be able to operate and
[41:20] handle Walmart's website and shopping platform and things like that.
[41:27] Your website doesn't need all of that. So when you go to something like an Azure,
[41:34] and this is the thing that we're trying to make better, and this is why they hire people like me,
[41:38] is we want to make it so that it is as easy as using a Vercel or a Netlify.
[41:44] But at the end of the day, a lot of the thing that we're doing is,
[41:51] we have to worry about both sides of that coin. Vercel and Netlify focus more on the smaller projects.
[41:57] Then once they start scaling to beyond what Vercel and Netlify are comfortable with,
[42:03] what you start seeing is that bill, it goes from $5 to whole, that's a lot of money.
[42:12] Then from there, you're like, "Okay, wait a minute. I'm trying to do this thing in
[42:17] a service that isn't really designed to do that thing." They want you to do that thing there
[42:20] because that's how they make a ton of money. But maybe it's easier to move it over to one of
[42:26] the larger Cloud providers that are going to have different pricing options and
[42:33] different scalable tiers and things like that. >> This is a great explanation,
[42:42] but one of the Netlify or Vercel uses Cloudflare underneath for all of their services.
[42:48] A lot of higher. It's definitely like this is a. >> It's abstraction. I like the word as abstraction of Wiki.
[43:00] That's a really good way to talk about it. It's like, "Hey, Cloud is hard.
[43:06] We recognize that Cloud is hard. Would it just be easier if I could
[43:10] just give you my file and it works?" Then some service comes in and says,
[43:15] "Yeah, you can do that here." Then they build the piece that moves things over.
[43:21] >> I'm writing myself notes. >> You bring me over for Python and then we
[43:30] start talking about Cloud-native, which I'm not an expert in in any way, shape, or form.
[43:36] When I think of containers, I think of dev containers,
[43:39] which uses containers, but is on the development side,
[43:44] not on the production side. >> I think these conversations are great.
[43:50] It doesn't offer you much control as you would get. This is the crazy thing and I think one of
[44:00] the hard things is when you're learning something new, at least for myself,
[44:05] without understanding the big picture, it makes it very, very difficult for me to learn the basics.
[44:12] Especially for some people that may have a little bit of knowledge in areas,
[44:24] like I used to work at GoDaddy, so I want to compare everything to GoDaddy or WordPress,
[44:30] and I might know something there. >> No, that's actually a really good way to look at it too,
[44:37] because GoDaddy and a lot of those, these were like VPSs.
[44:42] These are like the early day web host providers of like, you have to, we will give you a plot of land,
[44:49] I like Aaron's reference, and then you now have to build your entire house.
[44:56] What WordPress did was like, "All right, cool. We're going to basically give you a model home,
[45:03] and then you just decorate the inside." Then what these other services said were like,
[45:10] "All right, we're going to give you a container home, and if you want more space,
[45:14] you just add more containers." It is ultimately that same space.
[45:22] It's just how we've handled it. As someone who used to be a sysadmin,
[45:28] I appreciate this a lot because I hated having to build a website,
[45:35] and then think about all of the stuff that goes into building a website that is not the website of like,
[45:41] "All right, I need to spin up this Linux server, then I need to set up all of the security stuff on that,
[45:48] and then I got to keep that server up-to-date, and then if I need another server for another thing,
[45:53] I have to do all of that stuff again, which is a nightmare."
[45:57] Then people were like, "Oh, containerization. Now you just pull these templates out,
[46:03] and now you just have to focus on keeping the template up-to-date,
[46:06] which is fine because it's a lot easier to do." Then there's NGINX configuration, which never works,
[46:13] and then you got to figure out WSGI and asynchronous WSGI and so many other things,
[46:20] and it's a lot of stuff that you don't want to have to deal with, and it becomes really expensive.
[46:27] When you can say like, "Oh, like this stream, we can just have a bunch of people that know
[46:34] Python and they just write Python code, and then they commit their Python code to the Cloud,
[46:41] GitHub or wherever, and a bunch of automated systems take over and
[46:48] make sure that that produces some big project." That's where we're trying to get to,
[46:55] and that's where we are now. >> Maybe we'll get to Python Chapter 2 because this
[47:03] is all questions that do lead to it too. Going back a little bit before talking about
[47:12] these learning containers was the project hygiene, which you were talking about you may not need to
[47:25] upload to GitHub or something like that or you can. I get that there's .ignore and .env
[47:38] files that you put a lot of your codes into, and you do the .ignore so they don't upload.
[47:45] What do you do with your .env file? If you delete it off your computer
[47:52] because you uploaded it on GitHub, there's no way of really getting it back
[47:55] or upload to GitHub, but it's not public. >> No. You do not upload your environment file to GitHub.
[48:02] That is the recipe for a bad day. If you delete your .env file,
[48:09] you have deleted your .env file, you need to recreate it.
[48:12] There are ways that you can put secrets in places that are there but you're not like with GitHub.
[48:26] GitHub has a whole secrets space. We're like, I mean, I can show you this.
[48:31] Let's see. Wait, what screen?
[48:39] Screen? Yeah. No, wrong screen. Other screen. >> So many screens. I get it.
[48:46] >> So many screens. Yeah. Move that over.
[48:47] >> Add to stream. Yay. >> All right. So let's just do.
[48:55] You go up there. Thank you. Okay. I'm trying to go
[49:18] to one that I know I don't have secrets on. Actually, let's just do this one
[49:21] because this is just my profile. This is just my read me, whatever, super clean.
[49:25] >> Can you zoom it in a little bit, please? >> Absolutely. Better?
[49:29] >> Yes. Thank you. >> Awesome. So if I wanted to
[49:33] have some secret here that I'm pulling from, I would just go to settings.
[49:38] I would go to, whoa. Security? No. Do I not have secrets enabled on this?
[49:49] Secrets and variables. Duh, snake would have bit me. Go. There we go.
[49:57] Secrets and variables. So let's say that I want to spin this up in a code space,
[50:02] and I want to make sure that some secret environment variable is available in that code space.
[50:10] So I want to say genskey, whatever. I don't know why I started to spell supercalifragilisticexpialidocious.
[50:20] Why would I do that to myself? This is a secret.
[50:25] I can put that there and that's there now, and that's where I would.
[50:32] Now when I open up a code space for this project, this key is available.
[50:40] This might be a key that's in my environment file locally, but now I don't need to
[50:47] upload my environment file because it's in this space. This space is only here.
[50:52] As you can see, you can't see it unless even if you're in here, you can't see it now.
[50:57] It is no longer visible to the world. Nobody knows what this key is.
[51:01] It is not usable. The way that you do that is you might use it for something like an action.
[51:08] I didn't realize I had all these keys in here. So these are things that they haven't been used in
[51:16] several years and they haven't been updated in several years, which, no, one second.
[51:26] Yeah. Having all of these keys in here means that apparently when my website, oh, this is because my old website used to deploy from here.
[51:50] So yeah, I have all these keys in here from when I used to deploy my website from this repo.
[51:56] So you might start building a thing and then all of a sudden it's like, oh, hey, I need that key.
[52:01] What's that key for this? Okay, here it is. But there's no way as I'm deleting these now on stream,
[52:07] there's no way for me to view what these keys are. Honestly, most of these websites don't exist anymore.
[52:13] So it's not even like even if you saw them, you're like, whatever. But yeah, like ImageKit.
[52:20] ImageKit was a way that I would auto resize images on my website, but I needed a key to do that.
[52:31] So it was like, okay, hey, run this code, but here's my key and it's in here.
[52:35] So that's how you move things. If you need to access them,
[52:40] you definitely don't put them because as I mentioned before, I can go here.
[52:46] You can't see what this key is. I can't see what this key is anymore.
[52:50] Once I add it, it's there. I can change it, but I can't actually view what it is.
[52:55] They protect me from myself and my live streaming apparently. You can also just do regular variables too.
[53:01] So these are ones that you might want that are perfectly fine to see. You have different environments,
[53:08] those environments might have different variables and things like that. But what you don't want is to have some file over here,
[53:16] and there's probably more stuff in here than it should be in all honesty. Not to a dangerous level,
[53:23] but you say, hey, here are all the things that I don't want to exist in my GitHub repo.
[53:31] By no means are you to ever load any of this stuff. A lot of this is build stuff that just takes up clutter.
[53:42] We were talking about earlier with Jupyter Notebooks and IPython configuration files and things like that.
[53:49] But we also see things like pip file, lock files, Python version files,
[53:56] celery, schedule, things like that. Then you have this entire list of
[54:00] environment files that you don't want included. The way that I generate this is I don't do this manually,
[54:13] because that would be a nightmare. What is this? Let's get rid of that.
[54:20] Let's just do something completely new. Then we'll do an open and we'll make
[54:30] just another test folder, gen stream, get ignore IO. I've got you. This is a different way to do this.
[54:42] Open up your terminal. I know this is really small.
[54:47] Is there a way? Yeah, make that bigger. Make it really, really big.
[54:55] >> Thanks. >> Now, I've got to figure out how to move.
[54:59] Okay, I can't make it that big. It doesn't like it when it's that big. There we go.
[55:03] In here, you just do mpx get ignore Python. Then what that does is that just builds a get ignore file that I
[55:17] can then look at that has all of those things. There we go.
[55:30] Well, now you, Anthony and Rizal, because she's GitHub, are all going to get tagged
[55:44] on asking the interwebs what their best practices are for
[55:50] what you do with this content if you don't want to keep it on your computer.
[55:53] But you need to have it backed up somewhere. I'm just curious what everybody has to say.
[55:58] But this actually makes it very tangible. Yet at the same time, I'm like,
[56:03] I feel like so many different people may have different ideas of
[56:08] this and their own ways of doing things. That is one thing I absolutely love about
[56:16] the interwebs is everyone does something different. >> Let's do some Python stuff.
[56:24] Now that I've got this folder here, let's do some Python stuff.
[56:29] >> Well, I think a lot of the Python stuff is actually just probably bare basic questions.
[56:37] >> That's fine. >> Let me, I'm going to switch us and I'm going to go to mine.
[56:44] Zoom this in one more. It's Chapter 2, Flow Control.
[56:53] One of the first things that this chapter is talking about is Boolean values and then comparison operators,
[57:03] which if I scroll down, pretty self-explanatory.
[57:11] I've seen this before, didn't seem too confusing.
[57:15] Remembering that it has a name, probably is going to take a little bit,
[57:21] but that part is helpful. The part that I was,
[57:28] first thing that would be helpful to talk about more is, you have the double equals and then you have the equals,
[57:38] and one means equal to and one means the assignment. I guess that seems confusing to me
[57:49] because does the assignment of it mean that it's going to be like a string or a value instead of a,
[58:01] I'm working on how to put this into words. I'm comparing it to something in Chapter 2 or Chapter 1.
[58:17] Like, scroll all the way down. There we go. 40 is assigned to spam,
[58:36] but 40 is not equal to spam. >> Let's pull up something to write code in,
[58:46] whether it's VS Code or Jupyter Notebook or whatever. >> What was that you're yelling about?
[58:57] >> That it was made to force quit. >> Okay.
[59:02] >> Which I can't say is wrong of it. I probably did something. I like to overload it.
[59:10] It gets mad. This file still does not update to this day. >> Still doesn't?
[59:20] >> Still doesn't. I'm just like, it's just not going to happen.
[59:25] I know. >> You can either do a new file or we could do a new notebook.
[59:30] Yeah, I would just prefer a new notebook. It's easier. Which I think,
[59:38] isn't there a way that you can do? I don't operate in notebooks mostly.
[59:43] Open up the command palette and yeah. Oh, you got it. There you go.
[59:50] >> We got something here. >> Let's try this. You want to say spam is equal to 42, right?
[59:58] That's what we're saying? >> Yeah. Spam, but if we do spam equal.
[60:04] >> Let's assign spam to 42, sorry. >> Let's assign 42 to spam.
[60:10] Now, if you do spam equal equal 42, you're going to get true.
[60:23] >> My keyboard is starting to go under my computer. Spam equal equal 42.
[60:33] >> You should get true. We want to run that block there.
[60:40] We got to get you updated on Python a little bit. You're running 3.9, we need to get you into 3.11 land,
[60:54] but that's for another day. There's a whole conversation about Python environments,
[61:01] that's a whole hour. >> Yes.
[61:09] >> You can install the latest version of Python. The easiest way to do it is go to
[61:13] python.org and then just install it. >> Here we go.
[61:17] >> You probably don't want to do that in the long-term if you're going to do Python development over a long period of time.
[61:24] >> Fair enough. It came back as true. >> Why did it come back as true?
[61:30] >> Because, to figure that out, I'm going to do this really quick.
[61:45] Hold on. Because it is a variable.
[61:57] I don't know what literal means. >> Literal just means that's what it is.
[62:02] Occasionally, if you're doing things like type printing, what you might say is,
[62:09] I have this value, this value should be any of these things,
[62:16] and it can be a list of different values. To say literal just means spam literally is 42.
[62:28] >> But spam cannot equal string 42 because it's a string. >> Yeah. If you try,
[62:35] does the string of 42 equal the integer of 42? >> I'd have to do 42.
[62:46] Because I can't put those the other direction, can I? Do you put a string equal an integer?
[62:53] >> I mean, in most cases, the answer will be no, or sorry,
[62:58] that in most cases, the answers will be false. But yeah, you can say,
[63:02] does a string equal this? You can say, does anything equal anything?
[63:08] Yeah, so that's still false. >> If I were to do spam equal 42,
[63:25] so spam equals 42, will it also assign 42 to spam?
[63:40] Will it assign and equal it or will it be like, I then have to assign it to equal it or to use it again?
[63:49] >> If you try to change the value of spam to equal the string of 42, it will no longer equal the integer of 42.
[63:59] A variable assignment can only be assigned to one thing. Now, that one thing could be maybe a list of things.
[64:09] You could say, let's do spam. I mean, you've already assigned it now,
[64:18] so once you've assigned it, it'll still, because it's holding that value in memory.
[64:26] You'd have to reassign it to something else or you'd have to destroy this notebook and create a new one.
[64:35] If you do, it equals 45, it's going to say no.
[64:38] It doesn't equal 45, yeah. >> What?
[64:42] >> Because spam is held in memory, so the value that you've assigned is still assigned.
[64:49] It's not running everything again. That's why what you can do,
[64:54] you can have a notebook that has multiple code blocks. You say, in code block 1,
[64:59] I want you to assign this value to this. In code block 2, I want you to get
[65:02] that value and do something else with it. It's still, that thing exists in memory.
[65:08] Until you remove the memory of it, then it will always be that thing.
[65:16] Restart, where did you go? We're in the block where it's, yep.
[65:23] Can you make that a little bit bigger? >> For sure.
[65:28] >> I'm sorry, the window itself bigger. >> Yeah. I like the explanation we got of literal,
[65:38] so just give me one second. >> Yeah.
[65:40] >> Hit show on screen. >> I would say it is literally.
[65:45] >> Okay. Interpret it as literal data. >> Where does the thing go? There was a thing that said,
[65:54] hit the little three dots next to clear outputs of all cells, little three dots there, and hit "Restart".
[66:02] >> Yep. >> Restart.
[66:05] >> Yep. Now hit "Run" on that and what you'll get is, yeah, spam isn't defined.
[66:13] >> Oh, so it won't. >> Yeah.
[66:18] >> But if I do this and do you run all? >> Yeah.
[66:27] >> It tells me true, but then if I comment this out. >> It'll still be true.
[66:32] >> Comment, comment, comment. Well, you know what, that's still.
[66:38] >> That works too. >> Comments it out.
[66:40] >> Yeah. It's still true. Because once you've assigned it,
[66:43] you've assigned it and it has that assignment in memory. When you restarted the Notebook server,
[66:52] you cleared the memory of it. All of your assignments went away.
[66:58] >> What you're saying makes sense. Now, also thinking about it to JavaScript,
[67:08] is JavaScript doesn't do that. So this just got cooler and also more confusing, but cooler.
[67:17] >> That's just a trick of Notebooks. If you were to do this inside of just a regular Python script,
[67:25] it would not work. It would just do the JavaScript thing. >> Okay. So if I were in VS Code instead of in Jupyter,
[67:34] it wouldn't remember. >> Right.
[67:38] >> It's a Jupyter. That's cool. This makes more sense.
[67:45] >> The trick with that though is make sure that if you're doing a thing that you don't leave something in or think that you've removed it,
[67:56] and then it's still there. It comes with its own trade-offs there.
[68:01] Because I used to do that a lot with when I would do data stuff, I would import CSV files and
[68:09] then store the value of the CSV file in a variable, and then I would go to do something else,
[68:13] and I would have a reference to that CSV file still, and then all of a sudden now it's pulling up this data,
[68:18] and I'm like, where's all this coming from? It's because I did everything inside of
[68:22] a notebook and didn't get rid of the stuff. >> But yeah. Does that answer the question on this thing equals this other thing?
[68:44] >> Yes. It does answer that question. I don't know if we'll need to go back there for this next question,
[68:53] but let's find out. >> The scrolling too.
[68:59] The next part is the operator's truth table, and just talking that through a little bit,
[69:06] like expression and what it evaluates to, and I'm like, wouldn't false and false be true?
[69:15] >> Everything on here until the final one makes sense. >> Yeah. There's this Python thing
[69:30] that I'm sure you will learn about eventually called any and all, and that's how I like to explain this.
[69:37] Let me see. Go to VS Code again. >> VS Code. Here we go.
[69:47] >> All right. Let's just create another block. This is easier.
[69:52] >> Hey, new code. >> Yeah. There you go. Let's make a list called options.
[70:02] Options equals and then a Python list. Oh, sorry. The list is the bracket thingies.
[70:20] I mean, we can use that. Yeah, that's what I was referring to,
[70:25] but we could also do the other thing, and there are times when you want to do that instead of that,
[70:29] but don't worry about that. Let's put true and false as options.
[70:38] True, false. Sorry, true, false.
[70:40] I keep forgetting that words have meaning in programming. What is the value of true is it's true, right?
[70:51] >> Oh, yes. >> The value of false is false, right?
[70:57] >> Sure. >> Yeah. The value of false is false.
[71:04] False equals true. >> Yes.
[71:06] >> True equals true. >> Okay.
[71:08] >> There's this concept called any and all. Next line, let's do print and inside of the.
[71:23] >> Is it print like that or just? >> It's print in parentheses, like that.
[71:29] There's no space in between them. There can be, but there typically isn't. There you go.
[71:34] Now we're going to do any in parentheses. >> Wait, not parentheses.
[71:47] Okay. Yes. Sorry. I'm like, why am I forgetting words?
[71:50] Okay. Any. >> No, you're going to want to put another set of parentheses there.
[71:56] >> Okay. >> Because any is a method.
[71:59] Nope. On the end of any. >> Do this. I'm going to get there.
[72:05] >> Right there. >> So like this.
[72:07] >> Perfect. >> Wait, I got one extra.
[72:09] >> Yeah, and then options inside of that one. Perfect. All right. So the any says,
[72:21] inside of this list of things, is there one, any one of them that equals true?
[72:29] >> Okay. >> So what do you think the answer is going to be when you run this?
[72:38] >> That, options, any of that. Well, based on what we just looked at,
[72:50] it'd be true-true is true. True-false or false-true is false.
[72:58] But I guess because false is false, that's why false and false is still false.
[73:04] Yet, it's like a double negative, wouldn't it make it positive?
[73:12] >> That's why I prefer using any and all, because any and all make more sense in my brain than and and or.
[73:20] So yeah, like I said, looking at options, we have one that equals true and one that equals false,
[73:24] and any says, is there any one of these that equals true?
[73:30] >> So looking at what you have in your options would, do you think that this would print true or false?
[73:38] If it's just looking for one that's true. >> True.
[73:44] >> Let's run it. >> Wait.
[73:47] >> No, let's run it. Let's just run it and find out. >> Because true and true would be true.
[73:56] >> No, because or, in this case, means any. It doesn't matter how many are true or how many are false.
[74:05] If there's one that is true, then the answer will be true.
[74:10] By the way, any and all are just ways of saying and and or, but you can do it with more characters.
[74:26] You can have 100 of these options, and then you'd be like true, true, true, true, true, false,
[74:34] false, false, false, true, false, false, true. If you do any, then if one of them is true,
[74:39] then the answer is true. If one of them is false,
[74:43] it doesn't matter because if one of them was still true, the answer was true.
[74:47] Then if you do all, then it says everything has to be true. >> I'm taking notes, just a sec.
[74:59] >> You're good. >> Any means that anything, basically anything, and then.
[75:14] >> I look at any as anyone. >> If any one is true,
[75:23] then I'm going to return true, and then all would be every one,
[75:30] like any one and every one. Like Vicki says, not overthinking,
[75:45] but it's saying, is any of them true? Now, let's do the same thing where we do in options,
[75:54] change true false to false false. Now, do you think it's going to return true or false?
[76:05] >> True. >> Why?
[76:10] >> Because at least one of them are false. >> No, because remember,
[76:17] any is looking for at least one to be true. >> Since it's not using the word true,
[76:25] therefore it's not true. >> Exactly, it's false.
[76:29] I mean, we can run this and see. >> Like what you're saying makes sense.
[76:38] I think it's just like saying true, there will be a false there.
[76:43] >> Yeah. >> That is truthful. >> Yeah.
[76:46] >> As in like language? >> Add a true to this, to options.
[76:53] So it's like you have false, false, true. All right, is that going to equal true or false?
[77:00] >> Probably equal true because there's at least a true. No.
[77:06] >> Just run it. Let's run it, let's find out. Yeah, you're right.
[77:12] >> Because it's looking for any one. If you think about it from any one and everyone,
[77:19] like if any one of you are true, then I'm going to return true.
[77:23] So now let's change any to all. >> That still makes sense.
[77:31] It's just the idea of getting around the verbiage. >> Yeah. >> Let's say it, I don't know.
[77:43] >> That's why I don't like and or. >> It is truthful that there is a false, yet.
[77:54] >> You can write that out and but that's not what it's asking. If you said are all of these false,
[78:10] and you only have false and false, then you would get true.
[78:14] But that's a lot to check for, and in many cases, we don't do that.
[78:24] These are like Python anti-patterns in many ways. What you're checking for is often,
[78:32] and this is where I don't want to pick on Al, because I like Al, Al is a friend of mine.
[78:36] But to say true or true, you're probably not going to ever do that.
[78:44] You're not going to do true or false. You're not going to do false or true.
[78:47] You're not going to do false or false. You're going to say, I have some things,
[78:51] and what I want to know is, are these things true?
[78:57] Are these situations happening? Or are these things going and doing something that I don't expect?
[79:06] Because what you're not going to do is have false, true, true. Instead, you're going to have a bunch of computer logic that says,
[79:14] what does this computer logic do? Or what does this computer logic equate to?
[79:20] An example of you might have a data class, which I mean, don't worry about what a data class is.
[79:29] But you might have a data class which is just an object, and that object is called person.
[79:35] Our person, we're going to assign called Jen. We say, okay, Jen has accessories, eyes, nose,
[79:46] mouth, hair, and these things can equal different things. Maybe eyes, nose, and mouth are just, do they exist?
[79:57] Do they exist on Jen's face? The answer is yes.
[80:02] Then you might have, okay, what about accessories? Glasses might be an accessory.
[80:08] Now, if we want to compare, does Jen have eyes, nose, a mouth, and glasses?
[80:15] All of these things could be true. But then we also might have hair,
[80:20] and hair might be hair color or we might call it hair color. We say, okay, maybe we're building
[80:29] a design app that says like, hey, given a picture, we're going to give you an outfit that matches your style.
[80:38] When you look at, does this person have eyes, nose, and mouth?
[80:44] If not, then we're not looking at a human being so that our app doesn't work.
[80:49] Or we're not looking at their face at least. Maybe that's something there.
[80:56] But then you say, okay, what is the hair color?
[80:59] You might have one shirt that is neon green. You're like, okay, we're going to match this with
[81:07] hairstyles that are blue, hairstyles that are blonde,
[81:12] but we're not going to match it with hair that's just black or hair that's purple.
[81:17] Then we might say, instead of just true or false, we'll say eyes, nose, mouth, hair color.
[81:27] Is the hair color blue or blonde? If yes, sure.
[81:36] If your hair color being purple, we're going to go true, true, true, false.
[81:42] The hair is purple, it's not blue or blonde.
[81:46] Therefore, we're not going to provide this option. This is why when we talk about
[81:52] the idea of what is true and what is false, I hate it when we boil it down to simply,
[81:57] is it true or is it false? Because nobody is going to do that in code.
[82:01] No one's going to be like, I have this true thing here, I have this false thing here.
[82:05] It's like, I have some code that ultimately results in something being true or false.
[82:15] >> You're going into questions that I had, but I'm going to skip ahead to go.
[82:22] Possibly, we may go back. Let me find this graphic.
[82:28] >> I should also mention I am not a teacher like Laura is. I am a person who
[82:34] gets angry at the Internet and builds things. >> I feel like that is fair.
[82:40] >> That is my teaching language, is like, this makes me angry.
[82:45] I'm going to talk about it. >> Later on in this chapter,
[82:49] we go through ELIF statements, which do make sense to me.
[82:55] Your examples were totally making sense based on knowing this part is coming.
[83:02] I think what I was a little stuck on is, could you have an ELIF statement
[83:12] and then another ELIF statement? Kind of how you were just explaining,
[83:19] is their name or do they have eye, nose, and a mouth?
[83:25] Yes. Do they have purple hair? Yes, no. This mapping we'll go with can flowchart,
[83:41] can expand more than just these basic true/false. >> Okay.
[83:47] >> Right? >> I mean, let's build it. We can build this out.
[83:53] >> Really quick. It's better to give examples.
[83:58] They get the temptation to introduce Boolean logic from a teacher point of view,
[84:03] because it's a knowledge distilled and abstracted, but learning is so much easier from examples.
[84:10] >> Agreed, 100 percent. >> Let's build it. I'm all about the building of it.
[84:18] >> Before we go there, because I do want to build it,
[84:25] I just want to go over the stuff really quick that I skipped over to make sure,
[84:30] just to make sure they don't go into these things. >> We'll build all of that too.
[84:35] >> Let's see. Wait. Okay. Honestly, this actually made a lot of
[84:44] sense of mixing Boolean and comparison operators. I was like, "This part makes sense."
[84:50] Not the true/false, that one took a lot to get my head through, but this one I'm like, "Oh yeah, this totally makes sense."
[84:56] I think it's also because Laura had to go through this graphic in the last chapter to help me break down the graphic,
[85:06] because it didn't have colors and I'm like, "What are they doing?"
[85:09] Then we got into that entire conversation about order of operations. >> I always say I don't read,
[85:17] I just try things and see what works. >> That is how I learned a lot of this.
[85:24] But since doing this, it's a lot easier to read through this beforehand and
[85:31] then ask specific questions when they don't click. But I know that not everyone may have the opportunity to,
[85:38] so if you-all ever need the opportunity to join our streams, ask all the questions, learn with us.
[85:44] Condition versus expression. >> Sorry.
[85:50] >> Yeah, you're good. >> We have things happening in.
[85:58] >> In the real world? >> Yeah.
[86:03] >> If you got to go, you got to go. >> No, we're good.
[86:07] Speaking of Python, I always call it the gathering of the juggalos because that's where my brain is.
[86:20] Are you familiar with what that is? >> No.
[86:27] >> That's okay. Don't worry about it. >> Okay.
[86:30] >> The collection of a bunch of nerds. Hey, James, what's going on?
[86:38] James, thank you for the raid. >> Hi, James. Thank you for the raid and welcome everyone.
[86:42] >> You just walked in as I compared PyCon US to the gathering of the juggalos,
[86:47] which is some people are going to get that, and some people are going to be like, that's wild.
[86:53] >> Really quick, we are going through this book, Automate the Board and Stuff, Chapter 2.
[87:00] >> Eventually, we'll get there. >> Eventually, we're going through it.
[87:02] We're also learning the slow roll of getting explanations behind everything.
[87:09] Thank you, Jay, for joining and what a seabed too. >> That is a great book.
[87:15] >> Yes, it is a great book. >> I have a follow-up book here. This is the sequel.
[87:22] >> Let me make it bigger again. >> Where's my camera at? There's my camera.
[87:26] >> There, yeah. >> Beyond the basic stuff,
[87:28] I call it Automating the Boring Stuff to Electric Boogaloo. But yeah, PyCon US is the largest gathering of
[87:39] Python developers on the planet normally. People come from all over the world
[87:47] to hang out and do stuff and I'll be there. If you see me, say hi.
[87:53] >> I'm trying to hold the book and clap, but it was hard.
[87:57] >> That's what we're talking about. Now, we're always doing things. >> Yay.
[88:04] >> Awesome. >> Thank you, Seabed2.
[88:06] Yes, I started coding seven months ago, six months ago. Jay has been a big part of that journey and I'm
[88:16] learning Python and TypeScript at the same time. >> I just get distracted and then yell at
[88:23] the chat and be like, "That's not what it is." >> Yes. We were about to go through
[88:34] what conditions versus expressions are. I was scrolling down because a condition,
[88:43] this if statement came up and it's like a condition that is an expression that evaluates true or false.
[88:51] I was like, "Did that just answer the question I had on the previous page?"
[88:55] >> Possibly. Let's see it again though because I can't see it. >> Okay. Yeah, that would help if I share my screen. That would help.
[89:07] The question came up from under, let me scroll back a little bit.
[89:15] Y'all, I have the paper book with me as I showed on the video, but we're going through it on
[89:24] the website as well because that makes it more accessible, which is amazing. Where am I going?
[89:30] >> Your question got answered right there. Wait, a little bit more right there.
[89:41] You're asking, could you nest if LF statements inside of each other? It's like if I have an if statement,
[89:48] then I do some more if statements. Then if I have an if statement,
[89:51] can I do an LF statement and then do some more LF or if statements? Yeah.
[89:57] >> Interesting. I appreciate you saying this because I think, at least for myself,
[90:03] it doesn't always register that that might have answered the question because we went from flowchart to code.
[90:10] >> Yeah. >> I was going with flowchart in my mind still. That is crazy.
[90:15] >> I still say we just build it out and see what it's doing. >> I'm down for that.
[90:21] But basically, what's the difference between a condition and an expression?
[90:25] I don't know where it went on here, but it says that
[90:30] Boolean expressions you've seen so far could all be considered conditions, which are the same thing as expressions.
[90:39] Condition is more specific name in the context of flow control statements.
[90:45] I'm like, what? I don't know what that means. >> I don't know what that means.
[90:50] Hearing that, what I'm guessing is, okay, I found it. >> Let me try to find it so
[91:02] everybody else can know what I'm trying to say. >> It's elements of flow control conditions.
[91:07] >> It's right here. There we go. >> Conditions always evaluate down to a Boolean value.
[91:13] The Boolean expressions that we've looked at are like true is true, true is false, false is false, all those things.
[91:24] What we're doing conditions is we're questioning the truthiness of a thing. A condition is like in our earlier question around spam,
[91:35] does spam equal 42? Well, we told spam that it does equal 42.
[91:41] The condition is if we were to do a whole bunch of things, and we just wanted to check,
[91:51] is all of this stuff greater than or less than 42? That's the condition.
[91:56] Then what it does is it'll boil down to, no matter what we write,
[91:59] it'll boil down to whether or not it's true or false. When we do an if statement,
[92:04] that's all it's checking for. It doesn't care what the code itself is.
[92:10] All it cares about is, does the thing that we're telling it,
[92:14] does it boil down to true or false? Can we build it now?
[92:31] >> I'm 90 percent sure that there are no more further questions before we got to that point.
[92:38] >> Okay. >> I think that was the last of the questions before.
[92:41] I skipped ahead to the elifs. The elifs on the elifs.
[92:48] >> The elifs. Well, I don't know if your elifs can have elifs,
[92:53] but your elifs can have if elifs, which are like a whole thing.
[92:58] But let's build some stuff out. Let's have some fun with it.
[93:02] Let's create, we're going to do some higher-level Python stuff
[93:13] just to make it easier for us to talk about this a little bit more. Let's create a class.
[93:19] We're just going to type in class. We're going to call that class person.
[93:23] >> You said that it doesn't mean- >> Class space person.
[93:28] >> No, just class space person. Just for the sake of you're writing Python code,
[93:34] let's make that person with a capital P. You don't necessarily have to,
[93:40] but that is convention. Then instead of a comma, we're going to do a colon.
[93:46] Now we're going to do a new line. Let's tab over again.
[93:53] I don't know why it only tabbed over two. That's weird, but that's fine.
[93:58] We're going to say i is equal to. Well, i is equal to.
[94:10] >> Probably don't. >> I mean, for some people they don't, that's fine.
[94:16] Then we're going to do nos equals one. We're going to say, let's just do mouth equals one,
[94:33] and then ears equals two. Now we're going to go a couple of lines down.
[94:50] Let's de-dent. Now let's make gin. Gin is equal to person.
[94:57] Well, gin equal person. >> Wait, am I signing it?
[95:02] >> Yeah, that was my fault because what I said was gin is equal to, and that would be double equals,
[95:08] but we would say gin equals person. Hairs equals one million.
[95:12] [LAUGHTER] >> Okay. Actually, yes.
[95:18] Let's go back up there and let's add hairs. You can just throw a random number in there.
[95:25] Horace. What you would really do is say like, has hair and make it a blue.
[95:34] >> Horace, yes. Y'all, I am horribly dyslexic and I like that you even said it.
[95:40] I was like, what are you talking? >> We're going to create an instance of person.
[95:46] You're going to add, just open and closing parentheses there. Now, this isn't what you would do with a normal class.
[95:57] This isn't the way you would do a normal class, but this serves a purpose.
[96:00] This does what we're trying to do. Now we're going to create an if statement on a few lines below.
[96:09] We're going to say, if gin.eyes is equal to two. >> Equal to?
[96:30] >> Is equal. When I say is equal, that's like the equal equal.
[96:35] >> Okay. >> Yeah. Add a colon and then on the next line,
[96:45] let's tab over again. Can you change your tab settings somewhere?
[96:53] Because that's going to bother me. >> I would think that it's probably using prettier, but.
[97:00] >> Well, it shouldn't be. >> Something, I don't know.
[97:04] >> Go down to the little bracket in the bottom right corner. The brackets in the bottom right-hand corner, is that it?
[97:12] Okay, never mind. Don't worry about it. I'll just deal with it. All right.
[97:16] If gin.eyes is equal to two, then we're going to do print.
[97:24] The print has the parentheses. There we go. Then in quotations,
[97:37] because we're going to make a string, that's fine. Gin has two eyes, glasses are an option.
[97:43] Let's just run this just to make sure that everything's working. What we should see, because you have two eyes,
[98:02] and then we should see the glasses. >> Yeah. I have ads on my stream.
[98:09] If it gets too annoying, let me know. I put them there because they actually do
[98:13] start to make a little bit of money. But I'm not full-time, tons of subscribers yet.
[98:22] >> Yeah. >> I've just been gauging on the audience how annoying they get.
[98:25] Jay tells me, he's like, "I think one time you told me on one of the streams." >> It makes me subscribe using Twitch Prime.
[98:31] >> I'm like, "I haven't given my Prime sub yet, so congratulations, here's five dollars."
[98:35] >> Prime sub. There we go, so you don't have to view them.
[98:40] >> Exactly. We got it to read. It checked, it said, "Gin has two eyes,
[98:46] glasses are an option." Now, what we want to do is we want to say,
[98:51] what if Gin didn't have two eyes? What happens next?
[98:58] This is why I was saying that we normally wouldn't define it like this. But instead, you wouldn't want to do
[99:06] multiple if statements because you only want to access this if the first thing isn't true.
[99:12] This is where that elif comes in. We could do if else.
[99:20] If else, maybe we go. >> Or we do elif.
[99:28] >> You can do elif, yeah. >> I'm looking at this too.
[99:33] >> You throw a colon. >> Give it a colon.
[99:36] >> Sorry, you wouldn't give it a colon. You would add your logic and then give it a colon.
[99:41] >> Elif does not equal. Wait, is that does not equal?
[99:48] >> You would need to define what you're comparing now. >> Elif doesn't understand
[99:55] that we're probably thinking about Gin's eyes because we may not be. If Gin's eyes equal,
[100:04] well, you could say, yeah, if it doesn't equal two, that's an option. I mean, yeah, you could do that.
[100:11] I was going to just say elif if Gin's eyes equal one, we say Gin only has one eye,
[100:17] maybe we get a monocle or an eye patch. Those are options as well.
[100:24] Sure. Again, someone might have lost an eye in the war. >> We'll have them double-check.
[100:44] Since we're talking about Gin, I'm going to go with myself.
[100:49] But if I do, would I put input here?
[100:56] >> This is where I was going to say, because we're doing a class thing,
[101:02] maybe let's just reassign Gin's eye count. We just say Gin.eyes equals three because Gin secretly,
[101:13] no, not there, that's our comparator. Just underneath Gin is equal to person,
[101:21] just create a new line, and do Gin.eyes equals just a different number.
[101:31] Yeah, there we go. Now, we've changed your eye count to three.
[101:36] Again, don't worry about the class of it all, it just makes it easy for us to change these values quickly.
[101:42] There is a correct or I guess more Pythonic way to do it, which I hate that phrase,
[101:49] so I vomited a little as I said it, but it's okay. Let's run this, and what we should get is, are you sure?
[101:58] Yeah. >> Because it did not equal two,
[102:02] but if I change this to two, then it'll say, "Okay,
[102:09] new question for you," especially going back. This remembered that spam equals 45,
[102:17] so why did this not remember that's Gin.eyes equals three? Is it because it's not part of the class?
[102:26] >> No, because you physically change the value. If you put all of the Gin.eyes stuff in
[102:35] another block and you just ran that block, it would remember what you last had it assigned to.
[102:41] But since inside of this block, you physically change what that value equals,
[102:46] it was like, "Yeah, no, we're not going to keep that other version." Faki, yeah, you're right.
[102:52] You're right. I don't even want to say idiomatic. It's a way of saying like,
[102:59] there's this thing called the Zen of Python, and one of the things in the Zen of Python,
[103:03] it says there should be one and only one way of doing things. I have learned in 10 years of doing Python that that is not the case.
[103:11] There is always more than one way to do it, and the answer it depends happens way more than it should.
[103:18] When people say things are Pythonic, what they're saying is, this is the way that I subscribe to doing a thing,
[103:26] and that might be the way in many cases. But there are also very,
[103:32] very many times where Python as a language moves in a different direction. The way that we should have set this up was as a data class,
[103:42] but we don't need to import data classes, define data class, and do all this other stuff.
[103:47] None of that is important right now. You're just trying to learn Python.
[103:50] Worrying about things like being Pythonic or not is like the biggest headache when it comes to beginners of like,
[104:00] hey, I'm learning the language. I want you to get the successes of I wrote some code and it did the thing.
[104:07] I don't want you to get tied up into like, well, what's the exact right way to do this?
[104:14] Because as you grow as a developer, there's going to be more than one way,
[104:20] and it will become apparent what is the right way once you're in those situations.
[104:28] >> You also just gave me an idea to like, I don't know if this is going to work,
[104:34] so I'm just going to try it. >> Yeah. I think I see where you're going.
[104:39] >> [inaudible] >> Run.
[105:00] >> Yeah. >> Now, let's try this.
[105:07] Let's add ears into this because in order for glasses to be worn, they need to hook around something.
[105:18] There are a few ways that we can do this. We can nest our if statement or we can just combine it into one line.
[105:25] We're going to do the first one first and then we'll go back and we'll make it cleaner.
[105:29] If Jen's eyes equal two, now we need to check to see if Jen has two ears.
[105:37] How do you think you would do that? >> I don't know the actual programmatic way of saying it,
[105:56] but like and Jen got ears equal to two. >> Yeah. Set your eyes to two above it so that you can test that and see.
[106:20] >> Run. >> Now, let's change your number of ears to.
[106:33] >> Like this, that's three, and then run. >> Well, let's change the value of your ears too,
[106:45] because right now, not in person, just in Jen. >> Like how you have Jen eyes equals two,
[106:53] just do Jen ears equals three. >> Ears.
[107:00] >> Jen has three ears now. Now, when you run that, what happens?
[107:07] >> But if I do. >> Well, first, let's address nothing printed.
[107:18] >> Because it didn't match this, so it didn't print anything.
[107:23] >> Yeah. But then what would it do next in your logic chain? >> It would say, does Jen have one eye?
[107:31] It didn't have one eye, so no. Does Jen have four eyes?
[107:36] No. If I say, how would you say Jen eyes and ears equal anything?
[107:50] Wait, wait, wait, Jen is equal any? >> I mean, no.
[108:00] I mean, you could do that. I think what you're trying to do is,
[108:05] what's the catch-all after that, and that's where else comes in.
[108:11] >> Else is the, all right, we have concluded that none of the things above are true.
[108:20] Therefore, this is what we're going to do. You want to add a colon to the end of the else statement.
[108:27] Yeah, right there. >> Yay.
[108:42] >> This is making a lot more sense. >> Here's an interesting piece.
[108:51] What if, let's add a value to our class at the top. Also, I know that we've been going for some time,
[109:00] if we need to stop. >> I was going to say.
[109:03] >> I'm good. I've got nothing planned today. I can do this all day.
[109:06] >> I can keep going, but I need a bio break, y'all. >> Yeah, let's do it.
[109:09] >> I will be, we will be whatever, however we want to do this,
[109:14] BRB, I'm going to put you on mute. >> Oh, I was just going to say,
[109:20] this is a great time to do a, hey, Jay's here, AMA.
[109:24] Hi, I'm Jay. I do things, ask me questions. I will be sipping my water.
[109:31] It is water. Happy to answer any questions. I don't know how many people,
[109:40] I can't see how many people are in the stream or whatever, but can use this as an opportunity to talk about myself.
[109:50] I think as we mentioned at the beginning of the show, I am a Cloud advocate over at Microsoft.
[109:59] Just got here, Camomile. I'm doing great. How are you doing?
[110:03] Jen will be back. We are going through some Let's Learn Python stuff.
[110:08] I have been, I think I said 10 years. I don't think that's accurate.
[110:12] I think I've been using Python for eight years. Eight years, yeah. I've been a Python developer for eight years.
[110:22] I'm in San Diego, home of the amazing San Diego Python.
[110:28] How long have I been using Python? Just answered that.
[110:32] My favorite modules in standard library. That's a good one.
[110:38] I am a fan of the, only because you said standard library.
[110:46] I'm a fan of IterTools. I have, like I said, I used to be an automator.
[110:51] That's how I got started with Python was automating my job as a system administrator back in the day.
[110:56] A lot of functional programming happened there, so you use a lot of iteration tools,
[111:02] which is why when we're talking about doing if-elif and all that stuff, I love that.
[111:06] Do I love or hate match statement? I haven't found as many uses for match statement that I would like.
[111:19] I do think that where Jen is at now, where she's trying to do pattern matching stuff,
[111:24] I do think match statement would be good for this. But also, I feel like teaching
[111:30] someone that doesn't know a lot of Python, the match statement is like giving a toddler a hammer or
[111:37] a chainsaw and being like, "Hey, do chainsaw things." Very dangerous.
[111:43] Match statements are great for what they're supposed to be used for. Most people don't use them properly.
[111:52] If you want to know how to use them properly, there is a talk that my boss gave at PyCon.
[111:59] You love the case like A, B, C. Match statement is very much for pattern matching.
[112:11] What you'll often get is someone tries to use match statement to shortcut a bunch of logic,
[112:17] and that's not what it's designed for. That's actually slower than just doing if statements.
[112:22] >> Yeah. If you're doing a long and deep if else chain, that sounds like a refactoring question.
[112:35] I would even say probably don't want to use match statements for that either.
[112:39] You probably want to do some refactoring of code. But yes, if you have a bunch of different cases like what we're doing,
[112:48] the match statement would actually be really great for this, but we're not there yet. We'll get there.
[112:54] >> What did I miss? >> Just answering questions.
[112:59] >> Nice. >> Yeah.
[113:00] >> I feel like we should have AMAs, like guests. Yet, I am starting a real job,
[113:09] actually pay me job soon and I'm like, I don't really know what's going to happen with my life after that.
[113:15] I hope I get to keep streaming, but I know that I will have to cut back on some things.
[113:21] >> Mondays and Fridays are usually like my, Monday is like I just need to figure out,
[113:26] I need a slow start to the week. That's when I do stream on Monday.
[113:30] It's like I want to work on something that I want to work on, so let me just dedicate some time.
[113:34] Then Fridays are Saturday for my boss, so I'm very much like this is me doing my job,
[113:43] this is me being in the community. I call it Fridays like community Fridays.
[113:47] I also work Saturday morning because I, again, I work for Microsoft,
[113:54] so we sponsor the user group that I'm a part of, so it's my job to be at that user group.
[114:01] It gets fuzzy, so I borrow time that I'll make up on the weekend and
[114:10] other places as a part of my job and my job responsibilities. >> I love that because it's definitely like with the job I'm starting,
[114:18] they were like, "Hey, have office hours so people know when you're probably going to be there."
[114:23] Yeah, if you've got a book time, book time. If you're most creative not during that time,
[114:28] don't worry about it. I'm like, "Okay, that works." >> That's the biggest challenge for
[114:35] developer advocates is that it's like how do I get my work done, but also figure out where do I do my community stuff?
[114:49] The answer is your community stuff is also your job. If you have to go to a meet-up later that day,
[114:56] you go to work late the next day or you leave work early and make that time up. That's how you prevent people from feeling a lot of burnout, which is a pain.
[115:10] >> Yes. Y'all, just for an update, I got a job. Yeah. I'm not announcing where yet until I start next Thursday,
[115:18] so I will share the details then. I can say it is as a developer advocate.
[115:24] >> Yeah. >> So it's what I've been working on the last seven months.
[115:28] Yeah. Thank you, Camomile. It's definitely something I'm excited about.
[115:34] It's been a lot of work. I've done a lot of work towards it before I started streaming just in my career progression,
[115:43] yet the visibility and learning tech has only been the last seven months that I've been working on that.
[115:50] It's pretty cool. I'm stoked. Anyway, we have been doing stuff to our if statement, if else.
[116:00] >> We've been doing programmatic body modifications here. There was a thing that came up in the chat
[116:10] about using a match statement instead of if and elif. I want you to know that this is a thing that exists.
[116:16] We are intentionally not talking about it right now, because we really want to understand you're going to use if,
[116:24] you're probably going to use if and else more than anything else. >> Okay.
[116:29] >> Elif comes into play from time to time. But I don't want to overload you with like,
[116:39] there's this other thing that does a thing, and it is very similar to this thing,
[116:46] and it could work in our case. But let's get a real good grip on like how we would make this work.
[116:55] >> I'm just looking really quick. Do you think it might be under lists?
[117:06] Lists might do matching? I'm just thinking I'm putting a note and saying, okay.
[117:11] I'm just going to say. >> It's actually because it's new.
[117:14] It's only been around for two years, three years, so it may not even be in this book.
[117:21] But just know that there is another thing. Well, I'm not sure if Al has updated the book lately.
[117:28] I know he writes a lot of books and he also does them on stream. >> Yeah. He does have newer versions,
[117:37] which that's reminded me that things in the website may not match my book. >> Go support Al Swigert. He's very good.
[117:49] He's actually speaking at a couple of conferences in the next few months. He's speaking at Python web conference and I think he's speaking at PyCon.
[117:59] He'll be at PyCon. >> I will say at one point his Twitter was private,
[118:05] so I tried following during that time and it's public again. >> He's probably on like Mastodon doing Mastodon things.
[118:13] I don't know. >> Yeah. I'm just trying to see what version.
[118:18] >> I have no idea. It's probably at the bottom.
[118:23] >> I have the second edition, but maybe I saw it on one of his streams.
[118:34] It really could be what I'm thinking of that he was talking about like I thought version 4.
[118:44] >> Yeah. There may be a third edition getting reviewed. >> Yeah.
[118:51] >> Then that means he's probably already started working on the fourth edition. >> Something that I found as a newbie coder and as my own learning processes,
[119:03] especially with being dyslexic is yes, there's a website version but I also have the hardback so that way I can take
[119:12] notes with where they are and be able to use text-to-speech and that's how I learn. Suggestion for everyone because that's how I'm learning
[119:21] both Python and TypeScript and also keeping them organized in my brain. >> Yeah. Some services will let you,
[119:29] it'll just give you all the versions if you want them. If you buy one, they'll let you have multiple versions.
[119:36] Back to our code. >> I did want to say when we're done with this,
[119:45] I think the next part just in case this helps knowing it is loops. >> Yeah. We're going to get there.
[119:55] There's going to be more than one person. >> My goodness. There's going to be more than one?
[120:02] >> Yeah. Let's clean up our class a little bit. Let's go up to the top.
[120:09] We're going to change a few things. This is a glasses company now.
[120:17] They just specialize in glasses and eye accessories. No, this is still a person.
[120:22] Our person, we'll just call them a customer or something like that. But we don't need to worry about the mouth.
[120:28] We're doing glasses things. Mouth is not necessary here.
[120:33] Hair. Let's change hair to hair length. We're going to make it a string and we're going to say that string is long.
[120:46] We're going to hair_length. With Python, we use underscores.
[120:53] JavaScript, they do the camel casing. >> Al does camel casing too.
[121:00] >> Al does camel casing because Al came from a different language. We talk about that. I give Al so much crap about doing stuff like that.
[121:11] It's like, okay, you can stop at that anytime. >> What is this called?
[121:17] I forgot what casing this is called. >> Kebab casing. That's kebab case.
[121:22] >> What is this one called? >> That's snake case because it looks like a little snake.
[121:28] >> I'm just writing these down really quick because it's a question I keep asking.
[121:35] >> Actually, well, no, never mind. I can't show you that one.
[121:39] Not because I can't show it to you, just because it'll only confuse more than it helps.
[121:44] Because my boss has a GitHub repo that has all the cases, and some of them are silly and should never be used.
[121:53] That is intentional. >> Then the other one was called kebab.
[121:58] >> Yeah. >> Kebab. Because it looks like a kebab.
[122:02] >> Then you have camel case, which is lowercase frontend and uppercase,
[122:11] every word in the middle, which is what you do with nothing in Python,
[122:16] or you should do with nothing in Python. But there are some things that exist from
[122:19] a long time ago that were like that, so they stay like that.
[122:23] Let's change our hair length. We're just going to make it a string,
[122:29] and we're going to make that string long, short, or bald. >> Give me a second. I'm thinking.
[122:40] >> Let's just assign it as long for now. >> I'm just saying that it's going to be the ones that we check for.
[122:48] >> Is that? >> Yeah.
[122:52] >> Okay. Thanks. >> All right. We don't have to change any of this stuff.
[122:57] Maybe let's remove the ears issue here. As our glasses company,
[123:08] we have a few options. Let's just write these out.
[123:15] We don't necessarily need to know what they are. You can even put them in comments.
[123:21] Let's say we have glasses, are for people with two eyes,
[123:31] two ears, and a nose. Also nose, let's just make that true or false.
[123:43] So nose, we're going to just set that to true. Capital T. All right, cool.
[123:56] Anybody that has two eyes, two ears, and a nose can wear glasses.
[124:07] We have monocles, which are for people who have one eye. >> I have no idea how to spell monocles.
[124:21] >> I think it's M-O-N-A-C-L-E-S. That's fine. We know what you're talking about.
[124:30] But yeah, for people with one eye, and we don't care about nose or ears
[124:37] because you pin the monocle to your shirt. >> I think I just named some,
[124:44] this is actually just a, what I just named them is a bad guy in a game.
[124:52] I'm going to leave it there as a bad guy because we also have, what was the octa?
[125:01] >> Octothorpe? >> Yeah, octothorpe.
[125:05] >> Yeah. >> We're going to add an octothorpe.
[125:09] >> That works. There's an E on the end of octothorpe, I believe. It has one eye and a nose.
[125:27] >> You don't need a nose for a monocle. It just sits on the eye right there.
[125:32] >> Yeah, but how does it stay if it- >> Yeah, squint really hard.
[125:36] >> Okay. >> It's supposed to rest in your eye socket.
[125:39] >> Okay, then we have an eye patch, which is for? >> For the other bad guy or just?
[125:51] >> An eye patch is for someone who has one eye and at least one ear. >> Well, I mean, okay.
[126:18] No, this is good logic. What other eyewear is there?
[126:24] I feel like that is it. >> What do we do for the octothorpe?
[126:29] >> I don't know. Maybe he'll be our bad guy. He'll be our villain. He'll be one of the customers.
[126:38] Oh my goodness, steals off the glasses. Sure, I like it.
[126:44] This is LensCrafter's new computer matching eye program. Let's start with, first of all,
[126:57] you have a customer, so we have our person. Our person is Jen. Jen is that person.
[127:00] Jen says, "Hey, I need eyewear." I'm glad you mentioned the 2020 vision thing,
[127:06] because that means we can have things like sunglasses that are non-prescription.
[127:10] Let's start our logic here. We say, if eyes,
[127:20] go up to your person class, add an attribute there that is called prescription.
[127:32] >> I think that's how you spell it. I'm going to go with yes.
[127:40] >> That's fine. That's just true or false. They either need a prescription or they don't.
[127:47] If you went into LensCrafters, the first thing that they would ask you is,
[127:54] do you need a prescription or do you need non-prescription?
[127:59] How would you check for if Jen prescription? I said it there.
[128:20] I'm glad you wrote it that way so that I can tell you the "Pythonic" way to do it.
[128:28] If you were to just write Jen.prescription, you would get true or false.
[128:36] Remember, an if statement only cares about if a thing is true.
[128:43] >> You wouldn't need this? >> You don't need that. You can just say,
[128:46] if Jen prescription. That's it. >> What about the colon?
[128:52] >> You still need the colon. >> Okay. Then I could say print.
[129:02] >> Well, let's not do a print yet. I guess you could do a print,
[129:11] but maybe we'll use the prints for the logic. That's fine. I'd pick
[129:20] needs prescription as a variable name just so that if statements read nicer.
[129:24] Yeah, you could do that. You would also maybe in the future,
[129:33] there would be a bunch of composition happening and then needs prescription would be like a method that
[129:39] says takes eye test or whatever. But yeah, you could change it to needs prescription,
[129:45] you can leave it at prescription, just whatever is going to work for you.
[129:50] >> Just on that, would it just change to this? >> No, it would be if Jen.needsprescription.
[130:00] Then you want to change the prescription attribute in
[130:09] the person class to needs prescription. >> Okay.
[130:15] >> Perfect. >> Like that.
[130:20] >> Sweet. >> Okay. That makes more sense.
[130:22] >> Yeah. >> What up data dev?
[130:28] >> You say great. Now if they need a prescription, then we know that we have
[130:34] to eliminate eye patches from the table, and we have to eliminate
[130:40] non-prescription sunglasses or designer frames. Again, these are all things that we could build
[130:46] later on that we're not really accounting for. Right now, we're just eliminating
[130:51] eye patches from our selection. But if they need a prescription,
[130:56] that means we need to give them either a monocle or glasses. What do we need to check for that
[131:03] to determine whether or not we need a monocle or we need glasses?
[131:08] >> I'm trying to think of how to put it into one statement, but it sounds like.
[131:18] >> Well, no. I'm just asking, what is our thing that we're using to,
[131:24] like we wrote it up above. >> Yeah. If gen.eyes equal to.
[131:40] Wait, I see what I'm doing. I don't know how to write this.
[132:04] If eyes equal two, then glasses, if eyes equal one,
[132:11] then molecule, whatever it's called. But do I do it here?
[132:21] I would do it underneath. >> Here, you fell for my trap card, which is great.
[132:30] Right now, your second if statement is on the same level as your prescription.
[132:37] We want to put that if statement inside. >> Yeah. Can I delete all these other ones?
[132:43] >> Absolutely. >> You can do whatever you want.
[132:48] >> I want this to go inside of here. >> Yeah.
[132:54] >> Which would be like this? No. See, it corrected me.
[132:58] >> Right there. >> Thank you.
[133:00] >> I mean, again, I don't know why they're only doing the single thing, but that's fine.
[133:05] It is what it is. Actually, no, it does look like it is four.
[133:07] Okay, never mind. This is fine. >> One, two, three, four.
[133:11] >> Yeah, perfect. Spacing is weird. This is where like monospace fonts are nice
[133:17] because then everything is the same width and then stuff lines up pretty.
[133:24] Now, we're checking for eyes, but we also need to check for ears.
[133:32] This is where we could do an and statement. We could say if gen i is equals to
[133:42] and gen ears is equal to two. >> Yeah.
[133:51] >> Then we would print glasses are an option for you, or like prescription glasses are an option.
[134:06] >> There you go. Also, just so you know, these are how decision trees get made.
[134:26] Like those little chatbots that you talk to that are not chat GPT or whatever that are like, "Oh, hey,
[134:34] can you put in your number?" Then it puts in your number and it goes,
[134:39] it checks for that number. Does this person have an account?
[134:42] Cool, this person has an account. Which do you want to choose from?
[134:46] Then you just check that value. That's how those chatbots get made.
[134:50] It's like this nested chain of these things. [LAUGHTER]
[135:23] >> There you go. I like it. That is what it's going to be named.
[135:26] >> This is actually an interesting thing that this is where that Pythonic question comes into play.
[135:36] You can do this one of two ways. What you've written will 100 percent work the way that it is now.
[135:46] Having two if statements, one just being false,
[135:49] you decide to do a thing or you just skip over it, and then you just have another if statement to check.
[135:55] However, if you have two eyes and two ears, that already means that you don't only have one eye.
[136:10] You can do an else, you can do an elif statement so that it skips that check.
[136:20] You can do, actually, that's it. That's all you can do, is an elif statement,
[136:25] or you can leave it as two if statements. >> I feel like I shouldn't have deleted what I
[136:34] wrote earlier because now that is gone. I'm like, "Wait, I really want to say,
[136:39] if neither of these work, talk to an associate."
[136:45] >> That's where you have, there's three flows that you can go through.
[136:53] You can just have, if a thing is true, do something. >> Yeah.
[136:58] >> Then the otherwise is do nothing. You're either doing something or you're doing nothing.
[137:04] You can also do if else. Then you can do, if this is true,
[137:11] then do this, otherwise, do this other thing. Then you can do if elif else,
[137:19] which is, if this is true, do this thing. Otherwise, check to see if this other thing is true,
[137:26] and then if it's true, then do this thing. Then if none of those things are true,
[137:30] then go to the else statement. >> Okay.
[137:47] >> But then if I want to keep building this out, I could do, that needs to go there.
[137:56] But if I wanted to continue, so if Jen needs prescription, great.
[138:03] But if not, would it be an else? >> Yes. You also have a small little bug here.
[138:17] Right now, you have an if else, which means the first if
[138:24] isn't going to generate an else statement. I think what you want to do is,
[138:29] as Vicki says here, an if elif else. Because the else statement only works
[138:39] on the last if that was there. There you go. >> Please explain, because I get the words you're saying,
[138:49] and I can change it, but I'm not computing why. >> We're going to look at the camera for this one.
[138:57] You have your if statement right here, right? >> Okay. Yes.
[139:02] >> Then if you have an else statement underneath it, it goes, is this true?
[139:10] If it's true, we ignore this, this goes away. If this is false,
[139:18] then do this thing here. That's if else, right?
[139:23] >> Yeah. >> Then you have if elif else. Is this true?
[139:32] If this is true, these go away, and it just does this thing.
[139:37] >> Okay. >> If this is false, is this true?
[139:43] If this is true, then this goes away. If this is false and this is false,
[139:52] then you do this thing down here. That's if elif else.
[139:56] The thing is, you can have if elif elif elif else at the bottom, and that works.
[140:04] >> Okay. >> Now, if you just do just if, if goes away.
[140:11] If you have two, I can't do two ifs.
[140:14] I don't know. If and if, if this is if and this is if,
[140:18] and you have an else statement here, this if statement has nothing to
[140:23] do with this if else relationship. If you have if and that's not true,
[140:31] that doesn't change any of this relationship. It'll still check for both of these values.
[140:37] If you have if and elif, then this being true means that this is false,
[140:43] or not that this is false. If this is true, that means it doesn't worry about this.
[140:46] That's why if you do if, if else, the first if doesn't matter anymore.
[140:54] Because it's never going to say, otherwise, go do this other thing.
[140:58] But if you do if elif, it only checks the elif if the first thing wasn't true.
[141:04] Then if nothing in between those are true, then it'll go to the else statement.
[141:09] >> Okay. I'm going to read this first and then ask this next question because it may answer it.
[141:17] You basically only want one of these cases to run with an if, elif, else, then only one of them will trigger.
[141:27] If you have an if, if else, then the first one will run,
[141:31] then the second if else is checked. You could potentially do
[141:38] the first thing and the second thing, or the first thing and the last thing.
[141:42] >> Yeah. >> Could I have written this,
[141:48] since it's also nested, but if this is nest,
[141:52] could I have written this first if in elif instead of an if? Could I just elif the entire world?
[141:59] >> We can't see the code, by the way. >> Just kidding. Thanks.
[142:03] I just want it to switch in my head on screen. But if I wanted to,
[142:10] could I put just elif, elif, else? >> No. It needs to be if.
[142:16] If is the only one that's required. You can have if without elif or else,
[142:21] but you have to have if before you can have elif and else. There is another thing that you can do that like
[142:33] else statements you'll see in other areas of Python. But in this case,
[142:38] if is the only one that can exist on its own. >> What you're saying makes sense,
[142:47] yet I don't understand yet new to programming. I'm like, that doesn't logically make sense.
[142:54] Why can't you do an elif, elif, elif? It makes sense. It's just, you know.
[142:58] >> Because you can't have an elif, because remember elif means else if.
[143:04] >> Okay. >> In JavaScript, there is no elif.
[143:08] JavaScript has else if. >> Okay.
[143:13] >> At least I think JavaScript doesn't have an elif. I'm pretty sure it doesn't.
[143:18] >> If I wanted to do elif here. >> What would be the thing that you're checking?
[143:29] Do you have? Never mind, I forgot. You're in a notebook, so I don't know if you can
[143:35] even fold. Can you fold text in a notebook? Yes, you can.
[143:41] >> Okay. So I would just do else now. >> Note that if else is not actually one thing, it's two things.
[143:55] Yeah, that's what we're saying. It's if and then if else, yes.
[143:59] That's what we were trying to break down altos. >> Hello, altos. This is me having fun learning programming concepts.
[144:11] I actually built out my website. I'm very proud of my Astra website.
[144:15] >> I like the Astra website, it looks nice. It looks better than my website.
[144:19] >> Well, thank you. But at the same time, I'm like these core fundamentals,
[144:25] I'm just like really grumpy. >> Don't worry, a click will happen at some point.
[144:32] If not today, it'll happen at some point. You'll just be like, it makes sense now.
[144:38] >> This is why I'm doing it because I'm like, you know what? If I want to be able to do this,
[144:43] I got to take time and learn and practice and also not get frustrated that it doesn't work yet.
[144:49] All right. So going back to the first if statement, we did not, the Pythonic way,
[145:01] Pythonistic way, the way Python likes it is you don't have to say is true because it just knows that.
[145:11] >> Yeah. That's what it's checking for. Anytime you see the word if,
[145:17] what it wants it to say is, is whatever you are about to tell me eventually equate to true.
[145:25] >> So what I say else, or what I say else if Jen needs prescription?
[145:32] If I wanted to go through non-prescription. >> You're saying, so if it's not true, then it's false.
[145:42] Else is just the, this is not true,
[145:45] so then you do something else, right? >> Yeah. If I wanted to do it that way,
[145:54] because the else would have other if statements. It would be if in the else if,
[146:02] I have to look at this one just to see what else we asked. >> Yeah.
[146:07] >> Like this, I'm just going to copy and paste it. >> This is the fun part of programming
[146:14] because there is more than one way to do this. There are several ways in which we can do this.
[146:24] >> I don't know why it's yelling at me, but I'm going to do a print here too,
[146:30] just to make it this groovy. If Jen has print.
[146:43] >> The fun part is then to argue that your way is best. >> See, this is where I don't subscribe to one way,
[146:54] I subscribe to just like, how did someone do a thing?
[146:59] Occasionally, there are data science reasons for doing something differently,
[147:07] but most of those are like, what's going to be easiest read,
[147:12] and then what's going to be more performant, and then you have that balance,
[147:18] that dance in between them. In most cases now,
[147:24] performance for what Jen's doing will not be important unless we're doing some file automation stuff,
[147:33] and then we absolutely want that to be because I've fallen into that trap.
[147:37] My claim to fame in Python, and this was the thing that made me want to become
[147:44] a professional developer while Jen's typing things out. I mentioned before I was
[147:49] automating myself out of a job quite literally, and the company that I worked for acquired another company,
[147:56] and it was my job to add their products to our online e-commerce platform database thing.
[148:05] They had 40,000 items that needed to be added, and it was in a spreadsheet,
[148:11] and the spreadsheet matched to files in a system, and each one had its own thing,
[148:20] and there was a whole lot of stuff. In that case, you can do a iterate through
[148:28] the spreadsheet and then go find the file and then do some file things.
[148:38] But it's actually faster to do it the other way around. Start by iterating through the file,
[148:46] identify inside of your one spreadsheet where that file is and get the rest of the information.
[148:55] That's where it's like one of those things where like doing it one way versus the other.
[149:01] I started doing it the first way, and it looked like it was going to take about,
[149:07] I think it was like 32 hours to go through these 40,000 items and do a bunch of stuff.
[149:13] The other way around took six hours. You literally cut five-sixth of the time.
[149:24] I don't know what that is math-wise, that's like a bunch of percentage,
[149:29] like 85 percent of the time off by doing it one way versus the other.
[149:35] That's when it's like, sure, it is performance definitely more important in that case,
[149:41] but even then it was a thing to do. Jen, you wrote some stuff.
[149:49] Let me, what did we write here? >> I need to put my prescription in here. Hold on.
[150:00] I did not put everything in here yet. >> This is where the thing.
[150:09] Do me a favor at the top of this, the very top, right there where it says class person,
[150:17] go above that, add some more lines. You're going to need some more lines here.
[150:24] We're going to just make this a little bit easier to read. Import data classes.
[150:30] It's not terribly important that you understand what this is doing.
[150:36] It's just going to make it a lot easier to build multiple people in a faster format.
[150:42] Now, above class person, you're going to do an at sign, ampersand.
[150:48] You're going to do, no, ampersand is the other thing. You're going to do @dataclasses.dataclass.
[150:55] Yeah. We've got to get you using those. Yeah, there you go, .dataclass.
[151:02] Yeah, perfect. Now, we have to define some type values on this.
[151:07] I's is an integer. You're going to do I's colon.
[151:13] No, you're good. Go to where it says I's equals 2. >> Oh, I's colon.
[151:20] >> You're going to do I's colon, int, boom. >> Int?
[151:27] >> Yeah, like that, int. >> Okay.
[151:29] >> Yeah, perfect. Do me a favor. Do you have the Python plug-in for VS Code?
[151:41] >> Hold on. We're going to save this really quick. >> The Python extension? Yes.
[151:44] >> Let's save this first, just a sec. >> Okay.
[151:50] >> It needs to go into the cold field there. >> The LensCrafters story.
[151:57] The Lifetime series LensCrafters. >> We're just going to call it glasses.
[152:05] Glasses. >> That's fine.
[152:07] >> Glasses. Then you want it. Wait, wait, don't tell me.
[152:12] Because we went through this. >> You have some custom icons.
[152:17] Extensions. There you go. >> Extensions. I was like, I have to remember.
[152:21] >> Do you have emoji file icons? Interesting. >> It's installed.
[152:29] >> Okay. It's installed. Good. >> Wait, why is this one no longer?
[152:31] >> No, that's fine. No, you don't need that. Go into the settings.
[152:36] Sorry, the Microsoft person. No, don't install the thing that is in Microsoft.
[152:40] My bad. That wasn't my intent. >> It's okay.
[152:43] >> Okay. Go into settings. >> Not this settings or a different settings?
[152:49] >> No, settings. Just the actual settings. >> No, wait, we could do it down here too.
[152:55] There's multiple options. >> There are. Settings.
[152:59] >> Settings. >> Settings option. Then I made a video about this last year.
[153:06] Type hints, t-y-p-e, space hint, h-i-n-t. Cool. Now scroll down.
[153:21] Scroll down. >> Not JavaScript ones, not TypeScript ones.
[153:28] How about some Python? Astro Python. >> Here's what we're going to do.
[153:36] No, that's not it either. Just type in space Python after type hint,
[153:45] just so we can see. Just there we go.
[153:53] Type in add inlay to that as well. There's a lot of things here.
[154:02] You're missing some. >> The emoji icons make me happy.
[154:13] They make me not as mad at staring at it. >> Get rid of the phrase,
[154:16] type and get rid of Python and get rid of type. There we go. Change it from on to often less pressed.
[154:32] Now, go back to your notebook file. Now, hold the Control and Option key.
[154:47] >> Control and Option key. >> What?
[154:54] >> It's not getting anything. >> It did not work. It's supposed to work.
[154:59] >> I wonder if it doesn't work in. It must not work in notebooks.
[155:06] Darn it. Can I show you my screen? >> Yeah. It also doesn't mean that it doesn't work for my computer.
[155:19] My computer just does it like this file. If anything is changed there, it doesn't like it.
[155:27] I'm curious to see when I get my work laptop if I have the same issues, if I just broke it somehow.
[155:34] >> I could see what's going on here. If you're in a regular Python file,
[155:44] you can do coordinated classes. Sorry, I'm cheating.
[155:50] I have co-pilot on. Actually, I'm not even cheating. I have co-pilot on.
[156:00] I'm just going to say that. Eyes, ear. No, not encoding warning.
[156:05] Ears, nose. You don't need a mouth. Now, when you have this,
[156:14] by default, we don't have any of this stuff. Actually, we're going to get rid of that too.
[156:18] If we just said eyes equals two, ears equals two, nose equals one.
[156:24] Yeah, you're supposed to be able to do that. You're supposed to be able to hold down control and option,
[156:30] and it will make them magically appear. The type hints will appear,
[156:34] and you can double-click them and it will insert them, which is nice. That's what I was trying to get yours to do,
[156:41] but apparently, we can't have fun things. But also, I wonder if it's because it's a data class,
[156:48] and in order to set up the data class, it has to have these.
[156:52] Maybe it was yelling that. Yeah. That's what it was.
[156:56] Do this. Go back to yours. >> I may or may not have.
[157:05] >> No, you're good. >> I started a Python file
[157:09] just to see if it would make it any better. >> No, I don't think it will. Go to your notebook.
[157:15] >> Okay. Hold on. How do I get back to my notebook? We're going to figure this out.
[157:20] >> Do this. >> Somewhere.
[157:24] >> Use the command panel, the command palette. It's your friend.
[157:32] Hit "Command P". >> Okay. There we go.
[157:38] >> Just type in. >> This one.
[157:43] >> There we go. >> That is the hint that I tell everybody.
[157:48] If you can learn one thing, learn that the command palette exists,
[157:51] and it is your friend, and you should use it. >> The only time I use command palette is to.
[157:58] Actually, I wonder if I'm using the. I do the shift command.
[158:06] >> That is the actual like to do an action thing. If you just do "Command P",
[158:11] it puts you in a file search. It's the same bar and you can even move it by
[158:16] just adding the greater than sign. We'll just remove data class on that top part.
[158:23] No, not that part. Go down to right there. Just comment that out.
[158:28] >> This entire line? >> Yeah. Now hit "Command" and "Option".
[158:35] Is it still not doing it? >> Yeah.
[158:39] >> Just delete that line. >> Because if that doesn't work,
[158:44] then it's a notebooks thing and I want to report that. >> I'll try it over here really quick.
[158:51] >> Just copy and paste it. >> I just have to do the first one, right?
[158:56] Import data classes? >> You don't even have to do import data classes,
[158:59] just copy and paste the class. >> You're doing "Control" and "Option", right?
[159:13] Or do I say "Command Option"? Okay. "Control" and "Option".
[159:17] >> Yeah. I think it's a My Computer thing. >> That makes me sad.
[159:23] >> Because My Computer doesn't do a lot of things it's supposed to do.
[159:27] >> Well, the reason I was checking that, because if that's a bug with notebooks,
[159:32] that's a thing that I can report, and then we'll get that figured out.
[159:38] If you-all are still here, you should try this and let us know if it works for you,
[159:46] because it really could be My Computer. That's why it's hard to say.
[159:52] If you use VS Code, please try yourself and let us know.
[159:57] I'm going back to my notebook. Nope. It looks like it's an issue in data classes.
[160:10] I'm checking it now. You did your thing. You got your thing here.
[160:23] You're going to need to add the @DataClass.DataClass thing.
[160:30] That's a Boolean, B-O-O-L. Also, yeah, it looks like
[160:39] InlayTypeInts do not work in Jupyter Notebooks. Need to check with my.
[160:52] Did I misspell it? I probably misspelled it.
[161:07] >> What is this Boolean? >> It's just Boolean. It's B-O-O-L.
[161:33] Sorry. You got me. >> You were typing. I was like,
[161:37] "This is not working." I got a string one.
[161:41] I remembered string, but. >> Yeah. Then you need to add,
[161:45] get rid of the space between the @DataClass.DataClass in person.
[161:50] Right there. Yeah. Boom. Okay. Now, when you go to person,
[161:58] where it goes gen equals person, go in between the parentheses
[162:06] there and make a new line. Yeah. Now, you're going to just do
[162:22] needsPrescription equals true. >> Oh, so instead of these things?
[162:29] >> Yeah. >> Okay. I'm just going to
[162:33] copy and paste all this and then change it. >> That's not really going to work like that.
[162:43] >> Oh, yeah. Because it has the int. >> Yeah. Also, what we did is we set some defaults there.
[162:49] If you don't set it, you only need to change the things
[162:52] that you're going to actually change, which is why we built this as a class to begin with.
[162:58] I just want to say the entire reason that this makes sense, what you're talking about right now,
[163:07] is I've been working on learning TypeScript. They're very similar because of that type system.
[163:15] >> Yeah. If you tell that to someone who uses Python, they might get upset with you because, of course,
[163:22] type hints are polarizing thing in the Python community. Because in type hints,
[163:28] the types actually are enforceable. If you put the wrong value,
[163:33] then it's going to do some ugly stuff. It's going to be like, "Hey, no, you can't do that."
[163:38] In Python, the type hints are mostly just so that editors like VS Code can understand how to work with code.
[163:48] Also, for the user, which to me is the most important thing.
[163:52] But then also, data classes is one of the few exceptions where that is an enforceable thing.
[164:05] >> I will say it's because though learning them side-by-side, that it does make more sense.
[164:12] Now, as for enforcing the type system, and if it's going to be like strict TypeScript, for example,
[164:24] I comprehend the idea. I haven't done it yet though.
[164:29] >> Strict typing is, here's my super spicy take.
[164:35] Strict typing is the devil. >> All right.
[164:40] >> Vicki mentioned types are better in TypeScript than in Python. I strongly disagree because I think,
[164:50] so Python has this philosophy of duck typing. If it looks like a duck and quacks like a duck,
[164:56] it's probably a duck. I think that, yes,
[165:01] in most cases, you want to be explicit in your typing. But TypeScript takes it to way overboard.
[165:11] TypeScript is like if you have a dictionary and you haven't assigned that dictionary to a thing,
[165:19] and you haven't typed that dictionary out to be that thing, and if you haven't pinpointed what each of
[165:24] those individual dictionary values have to be, then I'm going to yield an error.
[165:29] Or you do what Altos just mentioned in the chat. You cheat and you say,
[165:35] I'm going to type everything as any, which if you're going to do that,
[165:39] what's the point in type hinting. >> But that's actually so when,
[165:45] and I'm paraphrasing, so do not hold Josh to this because I could also be misunderstanding.
[165:52] But that was actually a question that was asked on Josh's stream. Josh Goldberg, he wrote this book, Learning TypeScript.
[166:00] These are the two books I'm learning from at the moment. Josh is coming on the stream,
[166:04] is somebody actually specifically asked, and he said, well,
[166:09] if you're not sure what types you're using and the way you want to set it up, start with any and then go back and change it.
[166:16] That way it doesn't cause you to stop and start throughout the entire thing and getting stuck on that.
[166:22] In my mind, that totally made sense because I was just like, okay, cool. Once you're further along in your project,
[166:29] then it'll help you set up for success. But if you're just starting a project,
[166:33] that could be the death of everything as you just mentioned. >> Here's my alternate idea.
[166:43] Type it with what you know it will be typed as, unless it truly will be anything,
[166:50] unless it truly can handle anything, in which I have some code questions about that
[166:56] because I feel like that's where security vulnerabilities happen, or also performance issues.
[167:03] >> Y'all, just because I just went through the type systems area, this now has so many questions here.
[167:13] >> Yeah. >> The types that are these the same in,
[167:21] I guess I should Google. Y'all, we're going to go to Google really quick.
[167:24] Hold on. Where did it go? >> Yeah. Any is when you are handling things that you
[167:31] do not know what you are going to be handling. Even then, I argue that I think that you want to create
[167:37] an interface and you want to make sure you pass that interface in. Then if that interface is like something that is beyond your control,
[167:48] then you at least know that it is a reference to that interface. The reason I'm passionate about this is,
[167:58] I've been building my own static site generator for the last three years. The thing that is interesting about this is that I've been working at,
[168:13] it's been like my long-term project as a way to stay fresh in Python, continue to provide modernization ideas,
[168:20] and to have a playground to try these things in. Recently, I started adding the ability to create plugins for it.
[168:30] The thing that broke me was that because I didn't type hint my stuff, and I was assuming that I was always going to be working with text,
[168:45] I have completely bricked the plugin system because one of my plugins works with a dictionary and not with a string.
[168:54] Sure, I could stringify that dictionary and then add a bunch of unnecessary logic in,
[168:59] or I could have just type hinted everything and said, this is expecting this type,
[169:04] you're going to run into this issue. This idea of adding this really small feature set has
[169:10] taken now two months to implement because of bad typing, and bad initial design.
[169:21] That's why when people are like, "Oh, just give it the type of any and then keep it moving," that's great.
[169:28] Until three years later, you're like, "Why in the hell did I do this?"
[169:32] Because now I'm fighting with my previous self because of decisions that I made. >> I'm going to go with,
[169:42] I have no idea. I understood what you just said,
[169:45] but I don't know enough about the two. It would be interesting to have you and Josh on just to talk about type systems.
[169:56] >> Yes. >> Because I think that is,
[169:58] I'm looking further in the book. Between, y'all can't see all the things I'm holding.
[170:04] >> All the books. >> All the books and the website.
[170:08] In TypeScript or JavaScript, I should say, they have types of null, undefined,
[170:16] Boolean, string, number, big int, and symbol. >> Yeah.
[170:21] >> Which Josh told me even the last two don't really get used. He's like, "But you got to list them."
[170:27] I'm like, "Okay. Cool." Where this one, we have the Python data types.
[170:34] I'm like, "Okay, cool." We got same, same.
[170:37] We have data types, cool. But I don't even know where in the book,
[170:43] it talks about data types and automate the boring stuff. I'm wondering, A, is it worthwhile to explain in the beginning,
[170:53] or is it something that people learn data types in Python later on? >> Data types or type hinting is a thing that has not existed for very long.
[171:07] >> It's probably just not in here like matching. >> Yes. But my argument is there was a rift,
[171:17] there was an infinity war, or I guess a civil war,
[171:20] if we're talking about the Marvel movie universe, Marvel Cinematic Universe or whatever.
[171:26] In the civil war, there was this thing of we really want type hinting, type hinting is going to be great,
[171:32] we should totally do type hinting. Then there were half the people were like,
[171:35] "But no, Python is a duck type language. We don't need type hinting.
[171:38] Type hinting is going to be the death of Python as we know it." What eventually happened?
[171:49] Yes. We're talking about type hinting or type annotations, not necessarily data types.
[171:58] I think Jen understands the concept of this is an integer, this is a float, this is a Boolean value,
[172:04] what those different values are and what they look like. >> Yes.
[172:08] >> We're talking about the express annotation of these objects. >> I just learned last week in TypeScript.
[172:16] >> Yeah. >> I'm very excited about this because
[172:19] it was a whole chapter in type systems. >> This is where I'm amongst of those people that says,
[172:29] if you truly don't know what the type is, leave it blank until you know and keep it moving.
[172:40] I do agree with that. Assigning any is a declaration
[172:46] that this can handle absolutely anything. The reason I say leave it blank instead of giving it
[172:53] any is that if you're using a tool like VS Code, and you're in the situation where I reached out to my team,
[173:02] and they said that it should work, but it obviously isn't working,
[173:05] so maybe this is a bug. If you're using a tool like VS Code,
[173:12] you can keep writing the code and then go back and ask what types have been used in this. Do you have to go?
[173:19] >> Yeah, I'm totally 90 percent sure that I have my psychiatrist appointment right now.
[173:27] >> Oh, snap. Yeah, go do that. >> I'm three minutes late.
[173:33] >> That's okay. >> I'm three minutes late.
[173:34] >> This is great. This has been fun. >> This has been fun. Yeah,
[173:38] it totally started three minutes ago. I'm going to drop. Goodbye, everyone.
[173:43] Jay, if you want to stay on for a minute to finish that thought, you're welcome.
[173:47] >> Yeah, it's fine. >> Okay. Goodbye, everyone.
[173:50] >> If people are interested, just follow me on Twitter or something and then ask me and we'll figure it out.
[173:55] >> Yes. Follow me on Twitch. >> Get to your appointment.
[174:01] >> We'll be back. >> That's more important.
[174:02] >> Okay. Thank you all. Bye. >> KJAYMiller at everything.
[174:08] GitHub, LinkedIn, all of those things, even YouTube. KJAYMiller, that is the thing.
[174:16] She left it running, so I'm going to finish my statement here. If you're using VS Code and you write a bunch of code,
[174:24] you can use type hints to then go back and Apply the actual types that you're.

