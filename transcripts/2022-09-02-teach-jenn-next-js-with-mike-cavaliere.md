---
showLink: "https://www.youtube.com/watch?v=jFAdQ8AkjJU"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-next-js-with-mike-cavaliere"
title: "Teach Jenn Next.js with Mike Cavaliere"
publishDate: "2022-09-02"
coverImage: "https://i.ytimg.com/vi/jFAdQ8AkjJU/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful human. My Twitches are doing weird things and I don't know what is happening.
[00:11] Just kidding guys, we're not going to go live yet because my Twitch is not working because I got to affiliate,
[00:21] which is very, very exciting, but now there's two-factor authentication.
[00:25] I don't know if I can do it while we're live streaming. Hopefully, I didn't know it would mess it up.
[00:32] Yes, for anybody that has been following along, I just got to affiliate yesterday and set it up today,
[00:43] not knowing that it would be doing this. Give me just a second.
[00:47] That's always a fun way to start a live stream. Hey, just kidding, I can't start.
[00:53] Okay. Authorize. Go live. Okay, cool.
[01:04] Well, thank you StreamYard for at least not making me end the stream and try to figure all of that out.
[01:10] I do really appreciate it. But now that we are actually on Twitch because it's updated to affiliate.
[01:16] Welcome, welcome, beautiful humans. Thank you for joining today on Teach Gen Tech.
[01:22] We have Mike here today. Please introduce yourself, Mike,
[01:25] and the stuff we're going to be talking about today. >> Hey, everybody. Good to meet you all,
[01:32] Jen's audience, Mike Cavalier. I am located in Brooklyn,
[01:37] which is actually sunny today. Who am I? I've been an engineer,
[01:43] full-stack engineer for quite some time, a couple of decades. Throughout my career, I've done the engineering freelancer role.
[01:53] I've worked for some startups. I've done consulting.
[01:56] I've been a CTO for a little bit. I've been a manager,
[02:01] a tech director of different sorts. Throughout my career, I've worked a lot with JavaScript.
[02:09] The reason I offered up to teach Jen some Next.js stuff, hope I'm not spoiling it because you didn't tell the top kit.
[02:15] But it's up there, so nobody's being spoiled. >> It's all you to introduce anyway.
[02:21] >> Awesome. I have the power. I've worked with a lot of JavaScript frameworks over the years,
[02:29] and Next.js is one that is near and dear to my heart right now because it solves a lot of problems that
[02:36] previously you had to do manual work for, and it just does them automatically for you.
[02:42] Throughout my career, I've seen that happen a lot of times. Back before PHP was a thing,
[02:51] Perl was a language that I wrote stuff in, and then PHP came along and it did
[02:56] things automatically that you had to do manually in Perl. Then Ruby and Rails came
[03:01] along and it did things automatically that I had to do in PHP manually. Next.js is one version of that for JavaScript.
[03:10] There's many JavaScript frameworks out now, but Next.js is one of the more popular ones.
[03:17] I think it's really good for a web engineer to know because you can do a lot of great stuff with it,
[03:24] pretty fast and without banging your head into the wall. >> Very cool. I think that's also a good place too
[03:35] because that is for everybody that is joining. See, Anthony's calling you out.
[03:43] You even have a book about Next.js, right? >> Anthony, I do.
[03:49] I do have a book out. It's called Cut into the Jamstack.
[03:54] Next.js is at the center of it, but it shows you how to build.
[04:01] You're building a full-stack software as a service application with
[04:07] Next.js and a bunch of other very popular libraries. Chakra UI is one of them.
[04:13] Prisma is a database interaction library. Deploy it to a server and you utilize the app.
[04:24] But Next.js, I write about it in the book and in blog posts. I talk about it a lot because I think it's really cool.
[04:33] >> Thank you for that. I think that is also. Hi, Ben. I haven't had a chance to say hi.
[04:39] Hi, Ben. It's definitely something that I love that this is where we ended up going when we connected and
[04:49] went with the show for Teach Gen Tech. I also really want to call out Mike because I thought this was
[04:56] really cool that he was also open to talking about the other show I have,
[05:04] Shit You Don't Want to Talk About. I love that because I think tech
[05:08] and mental health do really go hand-in-hand, which we can talk about that on the other show.
[05:14] I just wanted to call out that, Mike, I just thought that was so cool.
[05:18] Made me even more excited to have you on the show, Little Did I Know, how you and Anthony know each other.
[05:24] We connected over Twitter space. Y'all, Twitter is amazing.
[05:30] I feel so weird because I haven't used it more than a couple months, but I'm like, it's just so cool.
[05:37] Definitely check us out. Make sure to follow Mike.
[05:41] Where do you want to get started today, Mike? >> We're going to get started by creating Next.js app.
[05:49] Actually, you might have to talk with her. Do we both share our screens at the same time?
[05:54] >> I don't think we can. I can share my screen or you can share your screen,
[05:58] but we can do stuff on your screen and then switch to my screen and go back and forth.
[06:03] >> Let's share your screen and I'll see how much I could talk you through and we need to switch.
[06:08] We'll switch and I'm going to do it along with you. >> Sweet. Let me get to that point.
[06:15] Yay. >> All right.
[06:18] >> I know that I need to get into the right folder because as Anthony keeps telling me to go through and do,
[06:25] I have yet to actually just have it default to this. >> There's always to-do's.
[06:32] There's to-do's in code, there's to-do's in your brain.
[06:37] >> Yes. That is 100 percent. That's all I got, is yes.
[06:44] >> This makes me think, seeing this too like there's, we could probably do a whole stream on
[06:50] just shortcuts to make your life easier when developing. >> I feel like we should.
[06:57] We can just have multiple people on that. I feel it could be like a two-hour stream
[07:02] of just shortcut hacks. >> Yeah, or a series because two hours of it.
[07:07] >> That's true. >> You have one person on for
[07:11] a half an hour and then another half an hour, and then you meet again,
[07:15] and you're going to accumulate just so many time savers. It's just going to feel so much more productive.
[07:21] >> I do feel like you just volunteered yourself though. >> If I got to do it, I got to do it.
[07:27] >> I dig it. Anthony, can I volun-tell you
[07:34] because you now have to go on the show. Hello, Noel. Cool.
[07:42] I'm in the proper folder finally. >> Cool. Now, we're going to generate an app.
[07:49] The way you do that, actually, let me ask you, actually,
[07:55] you may not need to do this. Do you have NPM or Node installed on your system?
[07:59] I think you must already. >> Yes, definitely.
[08:01] That is the first thing Anthony had me do before his episode and he was episode number 2.
[08:08] I have Node and Yarn, even though I still have a hard time comprehending what Yarn is.
[08:15] >> It's NPM and Yarn are very similar. They are package managers for JavaScript.
[08:24] What that means is when you're building an app, you want to use open-source code to do
[08:31] things so that you don't have to invent the wheel each time. In this case, Next.js is
[08:39] an open-source JavaScript library that we want to use to build a web app. Under the hood, it's going to do all these other things for us.
[08:47] It's a JavaScript package that we install into our project that's going to do a lot of things.
[08:56] If you've ever run NPM install or Yarn install or Yarn add, when you say Yarn add some library,
[09:10] it's going to find some library in this package place in the Internet,
[09:15] and it's going to pull it into your project. It's going to copy all the source code so you can use it in your project.
[09:21] It's also going to make a note of it in this file that you've got, so that anytime you install this package on
[09:30] another machine or you reinstall it, it's going to know to pull in those packages automatically.
[09:36] >> Okay. >> Managing the packages.
[09:39] >> That makes sense. Two things really quick. What up, Ian?
[09:46] I do want to also put this on there. It's the node modules folder that Anthony said to never look in.
[09:55] Is it each time before you start a project that you have to reinstall it or if I already have Next.js on my machine,
[10:08] do I need to reinstall it, and if not, how do I double-check that I have it?
[10:13] >> You want to install it every time into the project. >> Okay.
[10:21] >> Well, actually, let's walk through the process because this will be a good example of me explaining it to you.
[10:26] Let's start. We're going to start by generating an app. Using what's called Create Next App.
[10:34] It's a project generator by the Next.js people. The way you do that is it's quite easy.
[10:45] In your terminal, let's use, which are you more comfortable with, NPM or Yarn?
[10:53] >> NPM is what I think I've used the most. >> Okay.
[10:57] >> Pretty sure that's what it is. There's a command called npx,
[11:01] which comes with NPM. It's like node package execute or something like that.
[11:08] Npx space, and let's see how it runs, create-next-app space.
[11:23] Let's see, what can we call it? Maybe we call it teach-gen-next-js.
[11:30] >> I get excited in, yes, proceed, right? >> Now, yeah, you hit "Yes" and it's going to install
[11:45] the create-next-app package on your system, and then it's going to run it.
[11:51] Oh, okay. It doesn't like the capital letters, which the convention for
[11:57] a lot of node packages is lowercase hyphenated. >> Okay. Well, we can just do next-js then.
[12:06] I at least was trying to do that, but well, let me do this.
[12:16] Initials of teach-gen-next-js. Cool. I don't know if I realize it uses Yarn by default.
[12:30] It looks like it used Yarn to install the packages, and you see it's just
[12:37] listing all the packages that it's installing. This is related to what Anthony was talking about.
[12:42] All these things that are listed in this tree view here, slash and string prototype,
[12:48] these are all in the node modules folder that you don't want to look in.
[12:52] But that's where all these useful single-purpose node packages are, the JavaScript packages,
[13:02] that do all kinds of different things that the library that you're using, next-js, depends on.
[13:08] You'll see this in open-source projects. The bigger your project is,
[13:14] you don't want to write code that does something, somebody else has done and better.
[13:21] You want to just use that code. These are all little things that people have
[13:27] done really well that just get pulled in. If you look at the contents of your folder,
[13:34] well, there should be a new folder called tjt-next-js. >> I'm going to cheat and just pull this up,
[13:42] so that way I can look at it next to it. >> Not cheating, it's doing it your way.
[13:46] >> It is, ta-da. >> As you see, there's the node modules, don't look there.
[13:52] It's going to generate a couple of things. This is the directory structure of a next-js application.
[14:01] But you'll see this with a lot of JavaScript applications. A couple of things that you'll always see, package.json.
[14:08] If you open that up, that file does a couple of things.
[14:14] It tells you all about your project. If you have a license for the project,
[14:20] it'll list the license, your name, the name of the author and such.
[14:25] >> But I honestly didn't know I had brackets on here. I think this is a conversation that I've had
[14:31] multiple times because when it just opened something, I'm like, "Oh, I have brackets."
[14:37] Let me- >> You can probably just drag it onto VS Code.
[14:42] >> Open my VS Code. Eventually, I'll make it a default.
[14:48] See, we're just going to have this shortcut hacker jam thing, to just shortcuts for everything.
[14:56] >> It's going to be great. This is your package.json, and this is a file to remember
[15:03] because it's like a manifest for your app. I mean, the name of the project is important,
[15:10] but most notable right now is dependencies and dev dependencies.
[15:15] Dependencies are what this project depends on. Your app is going to depend on Next,
[15:22] on line 12, because it's a Next.js application, and it needs the source code from
[15:27] the Next.js project to do anything. It also depends on React,
[15:33] because React, it's necessary for Next.js to run. It's a dependency of Next.js.
[15:42] These are just other libraries that come bundled when you generate a Next.js app.
[15:49] The important thing to know is that when you look at this file, these are going to be the things that your project
[15:55] directly depends on that need to be included here. If you were to save this code repository in GitHub,
[16:06] and someone else would pull it from GitHub and install it on their machine,
[16:10] they just need to run yarn install, and it'll see this package.json file,
[16:15] and it'll install all the things that it needs. Next, React, React DOM,
[16:21] ESLint, ESLint config next, all these things that you see listed here.
[16:25] Then those in turn will install their own dependencies. Does that make sense so far?
[16:30] >> It does. I'm also seeing a fact.
[16:33] I hate that I haven't fixed this yet. What up, homie?
[16:38] Anthony, you wrote a lot of stuff, so I'm trying to figure out.
[16:46] I will say this one is probably a big thing. I appreciate that you explained it,
[16:55] especially with what Anthony is saying here that we skipped over it. I think the part that I am still a little lost on is,
[17:05] when I was doing stuff with Square, it was a web payments SDK,
[17:14] I believe with Next.js with a React wrapper. Saying it out loud, other people seem to know what that means.
[17:23] I don't quite understand why would it have a React wrapper if Next.js needs React?
[17:35] >> I'm not sure the content of that episode, but Next.js is a React wrapper in a manner of speaking.
[17:43] >> Okay. >> React is a UI library or a library for user interfaces.
[17:51] Next.js has React within it, and it uses React for the user interfaces,
[17:59] and it adds much more around it. In a manner of speaking, it does wrap React.
[18:07] It might have been the other way around or they might have been saying something different that I don't know about.
[18:11] >> Okay. Anthony said that that was a Square SDK installed into a Next.js project.
[18:20] >> Got it. >> He also provided the links to look at it later.
[18:28] That is in the comments if anybody wants to go check it out. I am going to see if I can finally get
[18:36] code dot to finally open this. I did. Okay, cool. Again, something that I need to get fixed.
[18:45] Now, really quick because this is probably one of the parts that I struggle with.
[18:55] Can you create a new repository from here or do you need to create it on GitHub first to upload it to?
[19:04] >> You do not need to create it on GitHub first. In addition, when you run "Create Next App",
[19:12] it creates one for you. If you go into wherever you utilize Git,
[19:19] whether from the terminal or from here, you'll see that there's a Gitignore generated.
[19:25] If you were to run Git status in the terminal, you would see that there is a repository there.
[19:32] On branch main, nothing to commit working tree clean. That indicates that there's a branch main that you're on.
[19:43] If you run Git log, you should see that it committed the initial files for you too.
[19:49] There's the initial commit from "Create Next App". That's another cool thing about "Create Next App"
[19:53] is it gets you started on a good foot. It's another thing that you don't have to do manually.
[19:58] >> Okay. Then I like Anthony's response on my productivity episode. I feel like we could just do this once a week with productivity tips.
[20:12] >> Yeah, we could do that. >> Yeah, I think that's a really good idea.
[20:17] >> Yeah, that's a really good idea. >> I think that's a really good idea.
[20:20] >> Yeah, I think that's a really good idea. >> Yeah, I think that's a really good idea.
[20:24] >> Yeah, I think that's a really good idea. >> Yeah, I think that's a really good idea.
[20:28] >> Yeah, I think that's a really good idea. >> Yeah, I think that's a really good idea.
[20:32] >> Yeah, I think that's a really good idea. >> Yeah, I think that's a really good idea.
[20:35] >> Yeah, I think that's a really good idea. >> Yeah, I think that's a really good idea.
[20:39] >> Yeah, I think that's a really good idea. >> I was going to say, I don't even remember how you run it,
[20:44] but I know that localhost would be our next step after we run it. >> Yes. If you run the command yarn dev,
[20:53] and really quick, if you open your package.json on the right, you see under the scripts where it says dev?
[21:06] >> Yes. >> Line 5 and 6.
[21:09] >> Yes. >> This is where that dev command gets defined.
[21:14] On the left, find a command that you want to be able to run from the command line and on the right, you tell it what to do.
[21:23] >> Okay. >> Run yarn dev, yarn and then dev or npm run dev.
[21:29] It's going to run the command next dev, which is defined in this project.
[21:34] This is just one thing to know in the back of your mind, because when you want to create custom scripts
[21:40] that run things from the command line, that's where you would do it.
[21:44] >> If you want to be a hipster is pnpm. See if I can even say that.
[21:54] >> Anthony, you're distracting. >> He always is, but it's entertaining.
[22:01] Localhost, at least this one is 3,000. >> Yay, we have it.
[22:09] >> This is all generated for you. One of the cool things about it,
[22:13] one way I like to learn and I have since I was learning web development is to see
[22:19] something created and reverse engineer it. I like to look under the hood of the code
[22:26] a little bit and see how things happened. If you want to look at the anatomy of this page,
[22:32] let's take a look in your VS Code at the folder structure
[22:36] and see where things exist. >> I'm curious just because for
[22:47] some reason I'm totally went to pages, but I think it's because of something that I'm working on
[22:55] for open source with distribute aid that I went to pages,
[22:59] but I don't think that's actually where it is.
[23:03] >> Your intuition is right though. That is where you keep pages in Next.js.
[23:08] Anytime you create a JS file in the pages directory, it becomes a Next.js page,
[23:15] and we'll do that in a minute. But if you open up index.js,
[23:19] you'll see all the contents to this page. You'll see welcome to Next.js on line 16 inside of H1 tag.
[23:30] You'll see get started by editing pages in Next.js, like all the code for this page is here.
[23:37] >> I'm also looking at the documentation, because I like how they have it in the box.
[23:46] I was like, I don't think I've ever looked at or understood to look at it to go,
[23:51] oh, so I get that this is the link, and with the class name styles grid,
[23:58] that's how the style grid is how that was made. Then it's using styles grid that was defined earlier,
[24:06] and then styles card to know that it's a card. >> Yeah.
[24:10] >> Right? >> That's right.
[24:11] >> Yes, I am learning. It's been two months.
[24:14] I would never have known that two months ago, so that's exciting.
[24:18] >> Just to reiterate, this is why I like reverse engineering things,
[24:23] because it's like when I was a kid, I would get Legos and I would build them according to
[24:30] the description and then I would take them apart halfway, and then I would rebuild them my way.
[24:37] I always found that to be a very valuable way to learn. You look at what somebody built,
[24:43] and then you take it halfway apart and do it your way, and that's what we're going to do here.
[24:47] >> Real quick, Ramon, I was just talking about you, and hi.
[24:54] That's actually, so he's part of Distribute Aid and how getting into that open source,
[25:03] and we were working on, they wanted to create a template page that people could just copy
[25:09] and paste certain aspects of it, and that's a lot of where thinking of seeing
[25:16] like these style grids and stuff like that, were things that we were having to set up for them,
[25:20] even though I think they're using Tailwind and it's a bit different and all that,
[25:24] but it's like, cool. Hi, thanks. Now I can continue.
[25:30] I got excited that more connections. >> Very cool. I'll do a quick explanation of
[25:37] like how HTML works in React in general. Everything in React is a component.
[25:47] A component at its minimum is just a function that spits out some HTML.
[25:55] Can do a lot more than that, often does do a lot more than that,
[25:58] but that's the simplest form. In React, the HTML is augmented.
[26:07] It's not just plain old HTML, it's JSX, which is,
[26:12] there's definitely HTML in there, as you can see like the main tag,
[26:16] the H1 tag, the P tag, looks very much like HTML with the exception that
[26:22] class name is not an HTML attribute. Classes, but in React,
[26:28] we use this class name attribute. For reasons I won't even bother going into,
[26:34] I also don't remember why, but that's what you do in React.
[26:37] You can write any arbitrary HTML in here for the most part. But then when you pass in the class name,
[26:46] styles.description, that's where Next.js comes into play. Next.js automatically lets you use CSS inside React,
[26:56] which if you were to generate React in other ways, you might have to do an extra step to get that working.
[27:03] That's one of the things Next.js provides for you. If you were to look on their homepage,
[27:08] you'd see this as a thing that they advertise as one of the Next.js values.
[27:13] In fact, we should take a really quick look at it. It's good to have on hand as a reference of why we use Next.js,
[27:21] and it's Next.js.org. >> It auto-completed into something
[27:29] that I've looked up before. Yeah, okay.
[27:33] >> It's the React framework for production. If you scroll a little bit,
[27:37] image optimization, zero config, file system routing is something we'll
[27:45] probably touch on where do they have built-in CSS support. This is where the documentation would be for this,
[27:53] but we'll just do some simple stuff in here so that you can see how you can start to use CSS in a Next.js app and style stuff.
[28:02] >> Cool. >> To break that down really quick,
[28:07] you had noticed that in the divs, there's this styles.container attribute,
[28:14] styles.main, styles.title, and you had noted that styles was defined somewhere else.
[28:22] If you look at line 3, this is where it's coming from.
[28:25] It's importing this object styles from a CSS file. >> Yeah, I can make this. It's been a minute.
[28:40] >> That would have to be somewhere in here or installed somewhere. >> If we look at line 3,
[28:49] we can break down how this import statement is working. >> Oh, it's under styles.
[28:57] >> Just as a note, if you go back to that file really quick, and I would double-click it so you keep it open.
[29:08] >> Cool. Yeah, if you noticed, when you first click a file in VS Code,
[29:14] the tab home module CSS is italicized. That means you're just opening temporarily,
[29:21] and if you click another one, it'll replace it. But if you double-click it, it'll keep it open.
[29:26] >> Oh, this is exciting. Ramon, just volunteering you,
[29:33] we're going to do a productivity series of shortcuts that each developer uses.
[29:39] You'll have to be back on the show too. All right. Cool.
[29:46] >> Go back really quick to index.js. There's an important thing there.
[29:50] On line 3, when you go import styles from, I will leave the folder director view open.
[30:00] >> Okay. >> What I'm talking about. When you see the dot dot,
[30:03] import styles from dot dot styles. The dot dot means go up one directory.
[30:12] Index.js is in the pages folder. When I say import styles from dot dot slash styles,
[30:19] the dot dot says go one directory up from the pages directory, and then styles means go down into the styles directory.
[30:29] You're telling it the relative path, like where to go to find this file.
[30:35] >> At some point, I'm not ready to look into this yet,
[30:40] but I learned about that when working at GoDaddy and doing things with cPanel and Plesk.
[30:48] I mean, computers in general have that folder structure. But I feel like at some point,
[30:54] I do need to put two and two together of, what does this all do with that hosting stuff?
[31:00] Because I'm still a little mind blown there, but I like that it's so consistent to learn across all of them.
[31:08] Thank you for also explaining what the dot dots mean, because I don't think I knew that one.
[31:11] The rest of them I could figure my way around. >> Yeah, no problem. Now we can do something fun if you want.
[31:19] Let's look at the index.js and the home module CSS at the same time if you feel comfortable doing that.
[31:26] >> Yes. >> You already know how to do that. You're a master.
[31:31] >> But I do need to make my screen bigger. >> Yeah, and you can probably hide the sidebar if you want.
[31:39] >> Yay. >> All right. Now, in the import,
[31:46] you're importing just this one object. That's some Next.js magic that basically says,
[31:54] import everything from the CSS file and so on the right,
[32:02] everything with a dot, dot container, dot main. Those are CSS classes.
[32:07] They're called classes in CSS. When Next.js imports styles from this file,
[32:15] it says make every one of these top-level classes, a property of the styles object.
[32:21] At the top where you saw a dot container, dot main, dot title,
[32:25] if you look on the left, you've got divs class name equals styles.container,
[32:30] styles.main, styles.title. >> Okay.
[32:38] >> Like line 7 on the left? >> Yeah.
[32:42] >> Line 1 on the right. >> I think where my mind went,
[32:48] which just means I skipped ahead even though I wasn't supposed to, was where is the title to go look at that or the description or the grid?
[33:01] Just because those are mostly, it looks like they're used more often than just the container.
[33:08] >> Okay. Yeah, that's valid. Yeah, title is used.
[33:12] Well, let's see what's used the most. Title is used, description is used,
[33:17] grid is used, card is used. But they all correspond to stuff on the right side.
[33:26] So there's a dot card. >> Is there a way to turn this doodad off where you can skip around?
[33:33] >> Yeah, that's called the minimap. So if you go into either view or window,
[33:38] I'm sure Anthony is going to tell us before we do it. There you go. Show minimap,
[33:43] fourth one from the bottom on the left side. >> Oh, thank you.
[33:48] >> There you go. >> Yeah. Thank you.
[33:51] >> Tell me if that makes sense so far. >> It does.
[33:59] >> You want to try changing one of them? >> Yeah.
[34:05] >> So pop open your browser. >> Now I got to find it again. Please stand by.
[34:11] >> Do you want a Mac? >> Yes.
[34:15] >> If you hit a command tab, that's an easy way to jump back and forth between Windows.
[34:20] >> Yeah. I don't think because I have a ton of Chrome browsers open. How does it know which?
[34:28] That's actually a great question. So I have three monitors.
[34:33] How does it know which Chrome browser to go to based on? Does it know to do it based on monitor? I don't think so.
[34:40] >> No, I forget. I don't know what rule it uses, but I know how to tab between the Chrome Windows.
[34:46] >> Sweet. Let me get a little smaller for now. There we go. All right.
[34:52] >> So you can click the browser and then we'll just look at the browser. You want to pick something to change the color of?
[35:00] >> Yes, because I think it'd be cool to change the title colors. >> Title of these cards?
[35:07] >> Yeah. >> Okay. Let's do that.
[35:11] Actually, here's a good exercise in finding. If you go to the browser,
[35:18] this is a useful way to find what you need to edit. If you right-click on the titles of the cards,
[35:26] one of the titles, and you go inspect, boom, that's going to open up the Chrome debugger console.
[35:36] You might have to resize a little bit just to make some room to see there. You could probably hit the "Escape" button
[35:42] once and it'll close the console on the bottom. >> Oh, sweet. Okay.
[35:47] >> This is the Chrome debugger and it's extremely valuable tool. In this case, we're looking at
[35:54] the HTML structure that is generated for us, and you see that h2 documentation tag.
[36:00] On the right side, you could see all the CSS styles that are applied to it, and even toggle them on and off and edit
[36:06] them without actually saving any code. >> Is this a REPL, an R-E-P-L?
[36:15] I don't know what they're called. >> I don't even remember what the acronym means,
[36:18] to be honest. I have to look it up. R-E-P-L, I forget.
[36:22] I know that's an acronym, but I forget what it means.
[36:25] >> I think it is. Console is REPL, from what Anthony said.
[36:32] [OVERLAPPING] >> Very cool. Go ahead.
[36:44] >> I was going to say, the important thing to remember is you can toggle and edit all the CSS on the right side in real-time and see how it
[36:52] affects stuff without actually touching your code, so it doesn't save anything.
[36:56] If you refresh it, it'll all be gone. Let's try it in the browser because it's fun.
[37:01] >> I was going to say, I think that's one of the biggest things that I've really struggled with,
[37:05] is people have shown me how to do it in here. But then I'm like, but how do I go find this and execute it
[37:13] within the file structure if it is something I want to keep? Very excited about this.
[37:19] Here is my documentation and this is my H2. Now, this is probably why it's a little hard to translate.
[37:34] Scroll to the top of that window on the right. >> No, that's left. This is right. There we go.
[37:40] >> On the right side of this right window, it's listing the files which have the styles that you see on the left.
[37:52] What this window is, it's a list of CSS styles in
[37:58] order that are affecting the element you have highlighted on the left. The H2 that says documentation in it is affected
[38:07] by the style.home_cod blah, blah, blah H2, which is defined in home.module.css line 95.
[38:18] Then in turn, it's affected by global CSS and all that. If you click it, it takes you to the line in the file.
[38:26] You're darn tootin' row. >> That's cool. Now, I don't know how to go back to where I was, but.
[38:37] >> It's elements. >> Okay, cool.
[38:39] >> You can always right-click and inspect it again. It's easy to get lost when using this.
[38:45] But hopefully, this demystifies it a little bit. The reason I call it, it's CSS stands for cascading style sheets.
[38:56] The cascading comes from the fact that you can apply styles to the same element in different places in different files,
[39:06] and they cascade, they combine, and the end result is what you see.
[39:13] There's reasons you want to do that. I don't want to confuse you,
[39:17] but just know that you might be applying styles in different places that affect this element.
[39:24] >> Is that like with JavaScript, and I'm totally piecing together different parts.
[39:32] One of the Mishko, who created Quick, came on and was explaining,
[39:41] I know that with JavaScript, it reads from top to bottom,
[39:46] and with Quick, it only reads what the page needs to render. If CSS is cascading,
[39:55] I guess you could say on that, would that mean that it's read top to bottom,
[40:00] or it's read what's inside of something else, and that's why it's cascading.
[40:05] >> The cascading is not a matter of the way in which it's read. It's more in that multiple things.
[40:17] There's a cascade in the way in which CSS applied to an element. If you really got into it,
[40:27] you could apply CSS styles to an element through classes, you could apply it through the element name,
[40:39] you could apply it through the parent element. There's a weighting to each style you apply,
[40:48] and depending on the weighting, one will take presence over another.
[40:53] For example, you see how there's different CSS selectors on the right side in
[41:03] the screen that are being applied to the same h2. One is the h2 tag,
[41:08] one is an asterisk, and one is.homecardlpl1h2.
[41:16] Those are all called CSS selectors. Each of them has a different weight to it.
[41:21] If you apply the same style with different values, like color, for example,
[41:29] if you apply a red color with the h2 selector, a blue color with the asterisk selector,
[41:35] and a green color with the.homecardlpl1h2 selector, the top one will probably weigh out because of how specific it is,
[41:47] because there's a system of weights in that selector. That's a cascade, that's the cascade.
[41:53] >> Got it. Okay. >> It cascades in the way you apply the things,
[41:57] and there's a certain level of weighting to which one wins. >> Okay.
[42:06] >> For the most part, you don't have to know that, at least not right now when you're adding styles to stuff.
[42:11] That comes in handy when you're seeing styles applied at different places,
[42:17] but in a style system. >> This was too good not to clip.
[42:26] Anthony created a clip for us or from something else. But there is a clip.
[42:32] >> All right. I can't wait to check it out. >> It is. It was you. That's funny.
[42:38] We'll share it afterwards. >> All right. Can't wait. Let's add some color.
[42:45] Pick your favorite color and we're going to apply it to the h2. >> Okay. To apply it to the h2 because it is inside of both of the,
[42:57] I'm also saying this out loud to see if I registered what you were talking about.
[43:01] I would need to go to the home CSS online 95 to be able to change the color?
[43:08] >> Right now, you can try any of them and we'll see what happens. Right where you are now is fine.
[43:14] You're adding a CSS rule called color. >> Okay. I open it or not?
[43:22] >> Yeah, you don't open the file. I didn't actually tell you, so it's on me.
[43:26] Double-click in that area where the other styles are. >> Yeah, it's a little hokey with the double-clicking,
[43:33] but once there you go. Then you type in color,
[43:38] which is a CSS property, and then you hit "Tab" and you can enter a color value.
[43:45] Now, the ones that are auto-completing for you are all named colors, so you can put in one of those,
[43:51] and so we'll pick one that looks okay to you. >> Yay.
[43:57] >> Boom. Now, if you notice, it applied to all of the H2 tags here.
[44:04] >> Very cool. >> So what I was going to say is,
[44:13] what that means is we picked a good style in HomeModule.CSS to actually put into the code.
[44:20] If you were to apply a color to one of the others, it may or may not have the same effect.
[44:29] The H2, it probably would. But this one you can't even edit because
[44:33] this is a user agent style sheet. That means the browser style sheet.
[44:37] This is the browser has a style sheet. These are your browser settings.
[44:41] But this is a good one to apply it to. So if you look at HomeModule.CSS line 95,
[44:49] we could probably put in a color that you want in the NVS code in the editor itself
[44:55] and reload the page and it'll still be there. >> So we are going to go to Home.Module.CSS line 95.
[45:05] >> There you go, .card H2. You'll notice that the selector is
[45:12] a little different in the browser. I think that's because Next.js is doing
[45:17] some dynamic generation of these styles. >> But it still helped a ton knowing the line file.
[45:24] >> Yeah. >> I guess I'm curious to watch it change,
[45:30] so I'm going to try a different green. >> Sure.
[45:34] >> Apparently, this one also just only has certain colors. >> Well, if you delete that actually,
[45:42] you notice your autocomplete was giving you all different types of colors too.
[45:46] So in CSS, there are a certain set of named colors like green and aqua and all these other things.
[45:53] But if you hit "Space" or I think you probably hit "Control Space", it should give you some autocomplete options.
[46:02] There you go. You notice the ones with the pound sign? >> Yeah, the hex colors?
[46:09] >> Exactly. You have all these hex numbers as well, and there's an infinite,
[46:14] maybe not infinite, but a very large number of hexadecimal. >> So we could look up a hex number and put it in here?
[46:21] >> Yeah. >> That's actually really cool and that makes sense on
[46:24] branding too to understand branding and making sure that the colors are accurate.
[46:32] Because I love that debate. I've been on both sides of that debate of,
[46:36] yes, it is that color. No, it's not that color. Yes, it is that color.
[46:40] So entertaining. >> Now, you're getting a syntax error.
[46:49] >> I know why. Semi-colon. Damn semi-colons and colons.
[46:57] >> That's what errors are for. They can't learn a thing from us. >> It's the same thing. I do it every time.
[47:02] Now what? >> Did you save the file?
[47:11] >> I thought I did, but maybe I didn't save.
[47:17] >> Yay, and I changed the green. >> Sure did.
[47:22] >> Okay. That was fun. >> Cool.
[47:27] >> I don't know why that's so fun to change a color, but that was fun. >> Yeah. Here's another fun thing.
[47:32] This is another fun thing about Next.js. Change the color again and save the file,
[47:38] but don't reload the browser. Change it to something different like red or tomato.
[47:43] That's a cool little picker you got too. >> I got it.
[47:47] >> It was like control space? >> Yes.
[47:54] >> How about gold? Goldenrod? >> Goldenrod, beautiful.
[48:00] >> Sure. >> All right. Now you save that and now just click the browser.
[48:07] Don't reload it. Boom. >> That is pretty cool.
[48:10] >> That's the hot module reloading. Next.js, it will do that not just with CSS and HTML,
[48:18] it'll do that with JavaScript with your logic changes. You can completely change components in the browser,
[48:27] and it'll refresh that stuff without you having to reload anything, which is great.
[48:31] >> I feel like that makes it a lot easier. Anthony just said you'll hear most people call it HMR.
[48:41] >> Hot module reloading, yeah. >> Thank you. Wait, what was that again?
[48:47] >> When you hear people refer to it as that, it may ring a bell. >> It really does make me think about how easy it was to change colors,
[48:56] and it makes me think about Ben and accessibility and being able to make sure it has a high enough contrast.
[49:04] Ben, yes, I will look into stuff, look them up on the Twitters at some point.
[49:13] That was fun. Now, I am curious, so how would I add if I want to add another box?
[49:24] >> That's great. Well, let's see if you can answer this. What would you make the box out of?
[49:37] What type of code would it be? >> It would be in the JS file because it's already had
[49:46] all of the CSS modules created, so I would just need this stuff from the JS file.
[49:53] >> You're right. >> I don't know which stuff,
[49:55] but I can figure that out. Let's see if I can figure it out.
[50:02] Yeah, because it looks like each of these are their own. What's this one? That one doesn't have a name.
[50:16] This one does though. It's from the a tag, [inaudible] and then come up with a website,
[50:34] maybe do some Twitch. Well, this makes it a lot easier,
[50:41] seems to be a lot easier to build a website too. I don't know why it's suddenly clicking.
[50:49] Yeah, because it also makes more sense why I could never figure out classes.
[50:55] I was always so bad at trying to figure out classes. I don't know why. It just never made sense to me.
[51:03] >> It will eventually. We'll help you with that. >> Wait, that's not what I wanted.
[51:18] Goodness gracious, really? Copy, and then go here.
[51:29] I do not want all this. I'm just going to do some undos
[51:33] because I feel like I moved some other stuff too. There we go. That is highlighted.
[51:37] >> Command Z is your friend. >> Huh?
[51:39] >> Command Z is your friend. >> Yes.
[51:41] >> Okay. >> All right. Examples.
[51:45] >> Teach some brand new here. >> Discover and discover how to build.
[51:59] Discover examples. All right. >> Save.
[52:09] >> All right. Don't reload the browser. Boom. Look on the right.
[52:15] >> It's there. Yay. >> Click it. Make sure the link works. There you go.
[52:23] >> Yay. We can see ourselves. >> Oh, no. Inception.
[52:28] >> I'll look at this later. But I hate that it does a, oh.
[52:40] Anthony just said, "Remember when I said on the React episode you'll never need classes in React?"
[52:47] Dude, that was two months ago. Sure, but probably.
[52:53] Probably is the reason I kept going with this. >> I mean, it depends.
[52:58] >> Depends on what kind of project you walk into, unfortunately. But no, he does have a valid point.
[53:07] Yeah, go ahead. You sounded like you were going to ask a question. >> I guess, how do I say this?
[53:20] What is something else that we could do with this that isn't just making a pretty website.
[53:29] >> You want to make a new product. >> Yeah, I want to make it do stuff.
[53:32] I'm like, I don't know how to make it do stuff. But I do like making it pretty.
[53:37] >> Wait, sorry. You don't feel like making it pretty or you do? >> No, I do like making it pretty,
[53:43] but I want it to do stuff. That's more important thing because
[53:46] it needs to be functional, not just pretty. >> Let's do this. Have you ever
[53:53] used fetch in JavaScript? >> I've worked for API companies and being able
[54:07] to fetch and get or maybe they're not the same. But it's definitely, I think I've done it. I don't know.
[54:15] >> Well, we're going to try. We're going to do something that is going to add
[54:20] some React interactivity. It's going to have a couple of pieces
[54:26] that are going to be a little confusing. But we're going to work through it and
[54:30] pieces of it are going to start to make sense. I'll try and talk you through each piece as we do it.
[54:35] But it'll take a couple of pieces and then at the end of getting those couple of pieces together,
[54:39] we'll have some dynamic data in here. Sound good? >> Yes. Anthony, to your point,
[54:46] these shows can take up to an hour and a half. We normally try to keep them under an hour,
[54:51] but I schedule that extra half hour just in case we need it for stuff like this.
[54:56] If it's a good breaking point, cool. If not, let's keep going.
[55:00] So I'm guessing we won't need CSS anymore. >> Not right now. Anthony does have a point though.
[55:07] It is going to take more than five minutes, so it's up to you how you want to handle it.
[55:14] Do you want to keep going? >> Oh, yeah. I totally want to keep going.
[55:16] I'm like, I want to do stuff. I want to make it magic.
[55:18] >> All right. The first thing we're going to do, and what I'm going to do is I'm going to ask you in
[55:24] your browser to open up documentation on the different pieces so
[55:29] that you can reference this stuff later and start to understand it more.
[55:35] The first thing I want you to search for is, it's called UseEffect.
[55:40] It's one word, UseEffect. UseEffect is, there you go,
[55:47] UseEffect React, and click. Let's see. Hooks API reference
[55:53] is probably the one we want to reference for now, but later on you'll want to look at using the effect hook.
[55:58] >> Okay. >> If you click on,
[56:02] so midway down the page on the left, there's UseEffect. >> Why this one?
[56:11] >> Yeah. >> Okay. Yay.
[56:14] Now, I'm going to tell you a little bit of background. Number 1, UseEffect is what's called a hook in React.
[56:26] The simple thing to know about hooks is, we already have components.
[56:33] We know that components at minimum spit out HTML or JSX code to make things pretty, to show you content.
[56:41] Hooks are how we add any thinking to the component. That's just a very general statement.
[56:51] But that's all you need to know right now, is that hooks, number 1,
[56:56] they are how you add anything more elaborate than just rendering text out in HTML,
[57:02] and they also start with the word use. Use this, use that.
[57:08] It's just a convention. You know hooks.
[57:12] >> Oh, goodness. What was I trying to compare it to? >> Prepare to be confused, Anthony.
[57:19] >> I know that this would be considered a webhook then because? >> No.
[57:26] >> No. Okay. What's the difference? >> Webhook is a different concept entirely.
[57:30] This is a React hook. >> Okay.
[57:34] >> In the React world, there's this notion of hooks that
[57:38] add interactivity to your components. A webhook is like a server-side thing.
[57:46] It's like a piece of code in your app that listens for. >> That's exactly what I was
[57:52] thinking about and wanted a clarification because I was like, it doesn't sound like you're describing
[57:56] that but wanted to make sure. >> Yeah. Totally different.
[58:03] That's a good thing to make a note of in your own personal notes later.
[58:06] But React hooks, just for adding interactivity and all kinds of thinking.
[58:11] >> Okay. >> We're going to use UseEffect.
[58:15] UseEffect, the disclaimer I got to give you is, it's in a way one of the most basic React hooks,
[58:25] but it's also one of the most confusing. Just want you to remember that and
[58:31] try and remember how I tell you to use it. Because even the documentation is not super great on.
[58:36] It needs a lot of work. They're working to improve this in newer versions of
[58:41] React and there's better ways of handling this. But to do what we're trying to do,
[58:47] which is the simplest way to get some data and put it into the page,
[58:51] UseEffect is probably the simplest way to do it. That's what we're going to do. With that,
[58:59] let's write some code and we're going to do it step-by-step. >> Great.
[59:04] >> In your component, this is a Next.js page.
[59:10] In a Next.js page, they all say, as you see on line 5,
[59:16] export default function and the name of the page. Every Next.js page just exports a function and exports default.
[59:25] It's the default export. It basically spits out the HTML for the page.
[59:33] Now, if you want to add some interactivity to it, as you would any React component,
[59:38] you do it before the return statement. You see on line 6, the return statement
[59:42] is what spits out all the HTML. Any interactivity and any thinking
[59:48] at React hooks has to go before that. >> Can I ask you a quick question?
[59:53] >> Of course. >> Let me see if I can figure out how to ask this.
[60:01] If we wanted to do, because the index page is normally the homepage, I'm guessing.
[60:09] But if we wanted to be able to add an additional page, would we add a page here
[60:16] and just tell the index page to pull from that content? I know it's not necessarily what you're talking about,
[60:23] but just so I can fit it in if I wanted to build a new page and what to do with that.
[60:27] >> Building a new page is one of the easiest things in Next.js. In fact, we could do that really quick if you want to.
[60:34] >> That would be helpful. That would be helpful just to really visualize how that would be made.
[60:39] >> Yeah. That's one of the best things about Next.js, is that creating a page is super easy.
[60:46] In your pages directory, create a file and let's call it About.js.
[60:55] This will be your About page. >> Sweet. Okay. If I save that, it'll show up.
[61:04] >> Probably show nothing yet because you're not doing anything in there.
[61:07] You do need a little bit of code, but we can try it. Let's see what happens. I don't know
[61:10] what happens if you load a blank page. If you go to localhost/about, there you go.
[61:17] To give you this error, and this error is actually informative, the default export is not a React component.
[61:24] That's because if you look at your index, it's looking for a default export.
[61:31] Next.js is looking for you to export a default function for the page.
[61:38] What we're going to write in here is export default function about page.
[61:45] >> I'm just seeing if it's in there. Function about page?
[61:58] >> Yeah. >> It'll be one word, about page.
[62:03] Because it's the name of a function in JavaScript and they got to be one.
[62:07] >> Okay. >> Since you're defining a function,
[62:10] you got to put open and close parentheses at the very end of it. >> At the end of the about page, rather.
[62:20] >> Yes. Okay. >> You're going to need open close curly braces.
[62:31] This is all just JavaScript function definition. It'll probably still throw an error,
[62:38] but if you save it, it's going to be a different error. >> Okay.
[62:43] >> The error is probably going to show you blank content because we're not returning any content.
[62:51] Remember, in React, this is a component and every component,
[62:57] for it to show you any HTML, it needs to return some.
[63:02] If you just return an h1 tag. Really quick to catch up on comments and then I'll do that.
[63:14] Starting with Ben's, totally page building seems to be next core feature like the API makes it very clear what it's for.
[63:26] Bakari said, "We did something similar with the square integration." Anthony, "Yeah, this would have been a good intro episode to the square stuff."
[63:39] I got really confused with square stuff, but not at the same time.
[63:45] It was like I could comprehend it, but didn't know how to break down the individual pieces of it.
[63:51] Bakari, "When we created the simple back-end." That gets us up there.
[63:59] I'm wondering. Beautiful. I can spell humans and save.
[64:15] >> Now, why isn't it showing up? >> Because it has no CSS?
[64:21] I don't know. >> No problem. You have to return it.
[64:29] You have to put in the word return. >> Where?
[64:35] >> Right before the h1 tag. I'll do a little more explaining that in a second,
[64:46] so you have a little background. Probably need it on the same line,
[64:50] or probably reformatted if you've got code formatter. >> That?
[64:57] >> Yeah. >> Please explain the return
[65:06] because I think that could be something that I've definitely missed in a lot of this.
[65:11] >> Also, you're going to want to make a note to install prettier in VS Code.
[65:17] It'll format the code for you and it'll- >> It's installed.
[65:21] >> Interesting. It's not running? >> I thought it was.
[65:24] I'm having to look like what it says in the corner because my laptop covers that side.
[65:28] >> Okay. Well, no worries for right now. >> It's probably a part of our productivity stuff
[65:32] of setting up prettier at some point. >> Cool. What we have here,
[65:40] JavaScript functions, so there's JavaScript by itself, outside of React, outside of Next.js.
[65:47] Let me start simple. When you declare a function,
[65:56] if you just say the word function about page, inside of it, you can do whatever you want.
[66:01] In React, for it to render any HTML, it's expecting you to return something.
[66:07] A function in JavaScript can just do something like console.log or whatever,
[66:14] or it can return a value. What that means is when you call that function,
[66:19] either the function will just do something or you say, my variable equals,
[66:25] call that function, and that function will calculate something and return you a value.
[66:30] Functions or these component functions React for them to render HTML,
[66:39] they have to return HTML. It's just the convention used in React,
[66:44] it wants you to return it. The return statement is where you
[66:48] spit out the HTML for the page. If you look at index.js,
[66:53] it's the same thing. It says, "Export people," and then it's
[67:00] a big return statement with all these divs and stuff in it. >> Got it. I honestly think I was missing that every time.
[67:12] Anthony, I'm not sure what you mean by that. Next.js page hello world snippet,
[67:23] but I don't really do hello world, I do hello beautiful humans.
[67:32] I always say it, so I've got to be difficult with that. But make about page about for consistency.
[67:41] >> He's just talking about the naming conventions, yeah, and it is a stickler for detail.
[67:46] But if you see how we have our export default function home it's
[67:50] capitalized in the about page, you would name it just about with a capital A.
[67:58] Now, this is your convention. It's good to keep consistent across the files in the project.
[68:05] You should make that a capital A though. >> Oh, I thought I did,
[68:09] but yeah, I'll pick a different convention across
[68:21] a single project and try and keep consistent like homepage or something like that.
[68:25] I use the word page, but this is a good practice. Cool. Let's go back and try
[68:31] and see if we can get in some interactivity. Now you know how to create a page.
[68:35] >> How easy. Yeah, definitely. Thank you. >> No problem. But yeah, if you go back to the about.
[68:43] I'm sorry, if you go back to the end. >> Index.
[68:48] >> Yeah. Now, first we got to get the useEffect from React. >> I'm just going to take us back to the homepage really quick.
[68:58] >> Yeah. >> Okay. One more time, please.
[69:02] >> First, we got to get the useEffect hook from React. We got to import it.
[69:06] We're going to add another import statement. >> Would the import statement information be here?
[69:14] >> No. >> Under, okay.
[69:15] >> No. I'm going to tell it to you because this is a, I don't even know where
[69:23] documentation would be on how typically to do this. But typically, this is
[69:28] how we import stuff from a lot of open-source projects. You're going to import, but this time you're
[69:33] going to import with curly braces. If you open a curly brace right
[69:37] here and you type useEffect, lowercase u, capital E.
[69:44] Then outside the curly brace, move your cursor to the past the end curly brace.
[69:54] >> Okay. >> Space from, and you can do this all on one line.
[70:01] >> Okay. >> Do another space, add quotes, and React.
[70:10] >> Is it with a capital R? >> No, lowercase. Typically, or exclusively nowadays,
[70:21] when you're importing something from a package that you've imported into the project with yarn or NPM,
[70:28] they should be lowercased. >> Okay.
[70:31] >> If you notice at the top, we're importing from next/head, next/image.
[70:36] Those are all lowercase too. >> Then this is the value is never read,
[70:44] but this will change once we start building more in here, right? >> Correct.
[70:48] >> Okay. >> You can save it, but just to break down the statement,
[70:52] if you notice, I think you have a sense of what import does. It says upload from another file or a package into this file.
[71:01] The ones at the top are different. They don't need curly braces
[71:06] because you're pulling in the default export. When we create the homepage right here on line 7,
[71:16] it says export default. There's a default thing getting exported.
[71:21] When a file exports a default, you can import it without curly braces.
[71:27] Import head, that package does a default export. Import image, it does a default export.
[71:35] Use effect is not a default export. It's a export that you import by name,
[71:42] so you need to use the curly braces. I don't want to blow your brain up,
[71:48] but just know that the differences in the way you import are dependent on how the file exports them.
[71:56] >> That makes sense. All of that made sense. I think where I'm a little lost is,
[72:03] this is going off in memory, so I'm not sure where,
[72:06] but I thought I've used it in some type of file where it did import React and that's where I'm a bit like,
[72:16] if I imported React, would it have imported use effect if I imported React as a whole,
[72:23] or I would still have to do it by itself? >> It would, but I don't want to
[72:28] confuse you because it's not the same across different places you import from.
[72:33] Importing and exporting is probably a topic by itself, that if we had a couple of different files,
[72:39] we could show all different ways of doing stuff. Just know that when you see the curlies versus no curlies,
[72:45] there's a difference in how the file exports it. >> Anthony also said,
[72:52] import React was an older convention that is usually handled by the new version of React.
[72:58] >> Yes. >> Okay.
[73:00] >> Cool. Let's pop this use effect in. Now, this is where it's going to get interesting.
[73:05] Inside your function definition, but before the return statement,
[73:09] we're going to type in use effect. Now, we're going to open and close parentheses.
[73:20] >> How do I know if there's supposed to be right next to it or space between them?
[73:25] >> Usually prettier will tell you. But either it should be okay, I believe.
[73:31] But I usually put them right next to it. I think most people do.
[73:34] The parentheses mean you're calling this function. This happens to be a React hook.
[73:41] If you notice the definition that just popped up, there are two parameters that it's expecting.
[73:49] Effect and depths. Now, without confusing you,
[73:55] use effect is a confusingly named thing, but you can say that it's running like a side effect.
[74:04] A side effect is something that happens that isn't the main purpose of this component.
[74:12] Main purpose of the component is to render out something. A side effect is something that happens on the side,
[74:21] which is a very basic way of putting it. It's the least confusing way to tell you it right now,
[74:28] and I think it's sufficient for now. What it's going to do,
[74:33] it's going to run a side effect function, and the dependencies, we're just going to pass in a blank,
[74:42] and I'll explain why in a second. First, let's give it a function.
[74:45] You declare a function here. You can declare it as a arrow function,
[74:51] where you just put in another set of parentheses, or you could declare it as a,
[74:55] let's see, what's the easiest way to do this? Let's do it as a regular function.
[75:01] I typically don't do this, but put it in the word function, and open close parentheses,
[75:10] and open close curly braces. Sorry, after the parentheses.
[75:19] - After both, or just the first set? - Right there, yeah.
[75:23] So you're passing this function as the first parameter of useEffect.
[75:30] This is the effect function, okay? useEffect is looking for two parameters.
[75:34] It needs a function, and it needs an array, okay? - Okay.
[75:40] - Bear with me. - I know the words you're saying,
[75:44] it's that it hasn't fully solidified what they each do, so that's why I appreciate you're telling me what to type,
[75:52] because I'm like, okay, eventually I will learn that's what it means.
[75:56] - Yeah, and in this case, this one won't fully sink in, but just bear with me, and we'll get something working,
[76:02] and then you can understand it a little bit more as time goes on.
[76:04] After that ending curly brace, I want you to put a comma. - After the curly brace?
[76:13] - Yep. And you're gonna put open and close array brackets,
[76:18] square brackets. - Oh. - Oh, there you go.
[76:22] All right, now save that. This is gonna do nothing, all right?
[76:26] - Sweet. - But this is the framework
[76:29] for how to call a useEffect function. Now, inside there's curly braces, add a new line.
[76:39] All right, so what this useEffect says, what this one with useDefine says,
[76:47] is we're gonna run some code after the component initially mounts.
[76:53] It gets added to the screen, okay? And what we wanna run is a fetch function
[77:00] to a website that I'm gonna give you. So JSON Placeholder.
[77:05] If you Google for JSON Placeholder, J-S-O-N, placeholder. All right, should be the first result.
[77:16] And this is a fake API. It's an API with just a bunch of dynamic,
[77:20] randomly generated fake data. And it's really good for projects like this
[77:25] that you just wanna pull in some data for the sake of pulling in data and do something with it.
[77:30] It's a very useful tool to have. And so if you scroll down a little bit
[77:36] in their documentation, you're gonna see- - Oh, you can see the fetch.
[77:41] - Yeah, and if you run it, you'll see the JSON data that it gives you, right?
[77:46] Another way we can see, I wouldn't put, don't put this in your code yet,
[77:51] but if you see that URL right there, in the fetch, you can take that URL and you could paste it
[77:58] in another tab in your browser, and you'll see what the JSON response looks like.
[78:02] - Okay. - All right. - Okay.
[78:08] - And you see, this is dynamic data. If you refresh it, it's gonna be different, I think.
[78:13] Oh, actually, no, they stay consistent. But if you delete the one,
[78:18] in fact, delete the number altogether, and just go to to-dos,
[78:23] it's gonna give you an array of to-dos. - And they're all user ID one, interesting.
[78:30] - Yeah, I mean, it's not perfect. - Some of them are too, we just gotta scroll.
[78:34] Okay. - 'Cause it's different users,
[78:36] different fake users that created them. And so this is just something that you can paste in,
[78:41] and we can pull data from and do something with. Now, let me think really quickly.
[78:47] What the easiest way to do this is without it being crazy. Yeah, pop that in there.
[78:57] And what we're gonna do is save that. And if you look in your browser and open the console,
[79:07] you should see it logging out some JSON data. And so, oh, you don't have to refresh.
[79:12] You see that? It's spitting out those objects right there.
[79:19] So have a look inside your code again. And I would delete the number one in the URL.
[79:28] And you see how it spit out a 200 element object right there?
[79:37] And now you can just kind of page through it to see what that object looks like.
[79:41] And look at all that. You've got all these elements in here.
[79:44] So it's a big array of to-dos, like fake to-dos. And so you just fetch this data.
[79:51] So applaud yourself really quickly, 'cause you just- - Yay.
[79:54] - From an API into your Next.js project. Now, the thing you wanna do with it
[80:01] is put it into your code base. And so you can spit it out and render some cards with it.
[80:07] And now, this is where it gets a little interesting. There's certainly better ways to do it,
[80:14] but we're gonna do it a very basic way, simply because this is another building block in React
[80:21] that can be valuable, right? I'd like you to look up the documentation for useState.
[80:27] - State? - Yeah, Anthony did, useState, A-T-E, S-T-A-T-E.
[80:35] Although useState would be a great hook to have. - I'm just like, why, what, what?
[80:40] Okay, useState. - Yeah, and I'm teaching you things
[80:44] that this isn't necessarily the best practices way of doing it.
[80:48] This is a learning way of doing it. - And I appreciate that, especially with,
[80:53] I'm definitely in the API world and I can understand a lot of it.
[80:58] I just, I've been struggling with going with, okay, I understand a lot of the concepts,
[81:03] doesn't mean I know how to make it. So I appreciate this
[81:06] and just getting the experience with it. - Yeah. - So, all right.
[81:09] So we got useState. - Yeah, and so what useState does, it says,
[81:15] this one's a little more intuitive. It says that in my component,
[81:20] I want to keep track of something. I want to keep track of the state of something.
[81:24] So in the example they give you, there, it says const count setCount equals useState zero,
[81:32] right? What this is saying is I want to keep track
[81:35] of something called count, which has an initial value of zero.
[81:41] And I'm getting me a function called setCount where I could set it when the user does something, right?
[81:49] And so later the user clicks a button and it says, setCount, count plus one,
[81:54] it adds one to the count. And so rereading it back,
[81:57] that line that uses the useState says, I want to keep track of the state of something
[82:02] called the count. It starts at zero
[82:07] and I have a function to set the count anytime I want. Okay?
[82:12] So in our code, we want to keep track of the set of to-dos.
[82:18] Okay? So you could even copy and paste this definition here
[82:22] to work off of this, the count- - Yeah.
[82:25] - Format your code a little bit to make it neater so you can read it better.
[82:30] That's a good thing to do right now. - And then it would go right here, right?
[82:38] - No. You want to...
[82:41] So you can't really use hooks and side hooks in that way. Well, you can and you can't.
[82:46] - So we would just need to do it outside of this curly bracket
[82:49] and do the same thing after I import it. - Yeah, or you could do it beforehand.
[82:53] I would do it beforehand just for ease of readability. So before the useEffect, I would add another line.
[82:59] In fact, you kind of have to because you'll see why in a second.
[83:09] - But that's not gonna work. - You can add...
[83:13] So, okay. So this is another...
[83:14] This is a good opportunity. So this is another named export.
[83:17] So you just need... Exactly, you're doing it correctly.
[83:20] So you just say useState. Okay?
[83:24] - And then we want to useState and then bracket.
[83:33] Wait, wrong one. And then we need to give it a function.
[83:38] - Well, let's start over. So if you delete that line
[83:41] and take a look at the way we're using it in the documentation on the left.
[83:46] Now useState is a different type of function. And you remember some functions return value, some don't.
[83:52] - Okay. - useEffect doesn't return a value, useState does.
[83:56] So you gotta say something equals useState. So the way it would be here.
[84:03] - Okay. - It's got a particular way of defining it.
[84:06] So you just want that one line. Const blah, blah, blah equals useState.
[84:13] Oh, not that line. - Oh, okay.
[84:20] We don't need that function for it to work? - No, you're already in your component function.
[84:26] That's just an example component function. - Cool.
[84:29] - There you go. And so again, this says,
[84:33] I'm tracking a variable called whatever. And I'm creating a setter function for it,
[84:39] something that lets me set the value of it. So what we wanna track is to dos.
[84:45] So I would change count to dos. Sorry, in the first variable, undo that.
[84:54] So this is to dos, yep. And then the function, instead of setCount,
[85:01] we're gonna be setTos with a capital T. All right.
[85:08] And then inside useState, we're declaring the initial value of it,
[85:12] which is just gonna be an empty array. So square brackets.
[85:17] - Oh, okay. Square brackets inside of the?
[85:20] - Correct. - Okay.
[85:22] - Cool. Now let's read it again in our context.
[85:32] So I just said this to you like five times, so sorry for the like broken record.
[85:37] But I want you to understand what useState does. And sometimes repetition helps.
[85:42] - Yeah. - What this line says is,
[85:45] I'm declaring a variable called to dos, which is gonna track the list of to dos
[85:51] that I'm pulling from an API. I'm declaring a function that lets me set those to dos
[85:57] to any value that I'm getting from the API. And the initial value of it
[86:04] is the one I'm passing into useState. It's an empty array.
[86:07] - Okay. - So to dos will start as an empty array.
[86:11] And then when I call setToDos, it's gonna set it to whatever value that I pass to it.
[86:16] - Okay. - And so the place we're gonna do that
[86:20] is after I'm done fetching the API call. So inside of useEffect,
[86:26] we're saying that when the page loads, fetch from this API,
[86:31] then convert the response to JSON object on line 12. And take that JSON object and console log it out.
[86:41] But now instead of logging it out, we wanna call setToDos.
[86:45] So if you change that console.log call to setToDos, it's going to save that object
[86:58] that we returned from the API and put it in the to dos variable.
[87:02] So now the to dos variable will have that list of to dos in it.
[87:05] And we can access it within the HTML and spit it out. - So what our next thing to be,
[87:14] would we build the, if we're gonna put it in one of these like boxes,
[87:19] would we put a box up here so that way we understand that this is all together
[87:24] or would we put it down here with the rest of the HTML stuff or in CSS stuff?
[87:29] - You wanna put the HTML rendering with the HTML. You wanna keep the thinking code
[87:35] above the return statement and all the showing things code
[87:39] inside the return statement. - Okay.
[87:44] - Does that answer your question? - It does.
[87:46] So if I want to have it show, I would want this here.
[87:52] But the class name would be something to dos? - So let's take a step back and do it a little simpler.
[88:01] I would delete that chunk of HTML. And the first thing you gotta learn
[88:07] is that if you wanna put a variable and output its contents in the render world,
[88:17] in the return statement, you need curly braces to start off with, right?
[88:21] If you notice, like you see class name equals and it's got curly braces,
[88:26] that says evaluate this JavaScript object styles.card and give me the value of it and then render that out.
[88:37] And so let's try that, but I'm gonna give you something in the chat
[88:45] that is gonna prevent you from being too confused. I'm gonna give you in the private chat.
[88:49] So we're gonna render it like this. So let's see, dos.
[88:55] All right, so this is a little code snippet that I just sent in the private chat
[89:07] that you can just put right in there. And I'll explain why in a second.
[89:13] You can delete that, yeah. Boom.
[89:18] And now save that. (computer mouse clicking)
[89:22] Oh, I might need to do something else with that, but let's see if it breaks.
[89:26] Boom, look at that. So you've got just a dump of the data
[89:35] in your todos variable. So now you know where that data is stored.
[89:39] We just have to, because it's a big array of JSON objects, we have to navigate that variable
[89:46] to get to the parts that we want. Does that make sense?
[89:49] - Yes. Pause for a second of everyone in the chat
[89:54] is saying you're doing an amazing job, and I would agree.
[89:56] - Thank you. - And also the json.stringify.
[90:03] - Yep. So if you look back at your code,
[90:08] do you understand the concept of JSON, or do you need that little explanation?
[90:16] - I won't say no to the explanation again, because I'm like, I think I know, but I don't remember.
[90:21] It hasn't sunk in enough yet. - That's okay.
[90:24] JSON stands for JavaScript Object Notation. Can you open that browser tab where we,
[90:33] let's see, where we ran the API, so like the JSON placeholder URL?
[90:44] Oh yeah, actually, this is good too. So this is JSON.
[90:49] It's just a format of describing data. In this case, it's describing a list of to-dos.
[90:58] And basically JSON's a very simple format that a lot of APIs use for sending information
[91:05] across the web. And it basically, the reason they call it JSON,
[91:12] JavaScript Object Notation, is it's the same way you would declare
[91:15] an object in JavaScript, right? You got curly braces, and then inside the curly braces
[91:21] are a set of names of things and their values. So a user ID is a thing, value is five.
[91:28] A title is a thing, big chunk of text is the value. They're called key-value pairs, okay?
[91:37] A key is like, this user ID is a key. ID is a key, title is a key.
[91:43] It's a key to get a value out of the object, right? Without overloading you with too much detail,
[91:51] JavaScript Object Notation looks like this. It looks like curly braces and brackets and colons.
[91:58] And basically anything, any JSON object is gonna either describe just a set of names and values
[92:08] or a bunch of those in an array. - Okay.
[92:13] - Not too confusing? - This is something that I've learned
[92:17] that I may not understand it 100%, but it's something that will definitely click later on,
[92:24] so I'm not gonna stick on it. - Yeah, that's fine.
[92:27] In this case, this is a JSON object that describes a list of to-dos.
[92:31] This is the list of to-dos that I pulled from my API. - Okay.
[92:35] - We're gonna display in the page, right? So going back to what people were saying in the channel,
[92:40] if you look at your code, the reason I'm calling JSON.stringify
[92:44] is React isn't gonna spit out a JSON object for us and show us the contents.
[92:51] I need to convert it to text. I need to convert it to a string.
[92:54] - Oh, so, oh, I get that part, okay. - This is just so that we can see the contents of it
[93:01] without throwing in error, okay? - Okay, cool, that makes sense.
[93:04] - All right, great. Now, what we don't,
[93:07] now, that's not how we ultimately wanna do it. We wanna take each one of those to-dos
[93:12] and spit out something, right? So what we're gonna do is to-dos is an array,
[93:20] and arrays have a function called map, right? Which says take every element of the array
[93:26] and do something with it and give me the new version. So what we wanna do is take every to-do
[93:34] and we wanna spit out some HTML for it. Does that make sense?
[93:39] - Yes. - All right, so, delete that.
[93:43] All right, and let's do, open up another set of curly braces
[93:51] because we want React to evaluate what's in here. And then we wanna take to-dos,
[93:56] and we call it to-dos.map. So, evaluate, or I'll explain in a second
[94:06] after we type some, to-dos.map. Open curly braces.
[94:10] Oh, I'm sorry, open parentheses. All right, now, to-dos.map is a function,
[94:20] as you can see, that has one function called a callback function.
[94:25] And I'm gonna run whatever function we pass in here on every element of to-dos, all right?
[94:31] So every to-do is gonna run this function and return the result.
[94:35] So we're gonna declare another function like we did before, right in here.
[94:40] And we'll just say function. - And then is it--
[94:48] - Function, you got an extra. Although that sounds really cool, funcation.
[94:52] I need to take a funcation soon. Function.
[94:56] All right, and now you'll need an open and closed curly braces for this function.
[95:05] I'm sorry, I keep saying curly braces. Parentheses.
[95:08] All right, and then after the parentheses, you need the curly braces for the body of this function.
[95:14] Delete that one, and you'll need an opening one and a closing one.
[95:23] All right, now hit enter just so we got a little space in there.
[95:26] So recapping, the outside curly braces say, react, evaluate this and render the output.
[95:33] - Right. - To-dos.map says, I'm taking the contents
[95:38] of the to-dos array. And for each element in the array,
[95:41] I'm gonna run this function in here. Oh, and I forgot to mention, this is important.
[95:45] This function is gonna take one parameter, a single to-do. - Okay.
[95:51] - So in the function definition that we just created, in the parentheses.
[95:57] - It will choose just one. - Yeah, but I want you to put the word to-do in there.
[96:05] So this is the name of the parameter that's coming in, right? So what this says is every time this function runs,
[96:10] sorry, just to-do, singular. - Oh, okay.
[96:13] - Yeah, or we could call it anything. We call it T, whatever is easy for you.
[96:18] But all this is, I'm taking in a single to-do at a time, and I'm gonna return
[96:23] what I want that to-do to turn into. - For sure.
[96:27] - Okay. And so let's start really simple.
[96:29] Let's just take this to-do, and let's return the title. So-
[96:37] - Can we go to, I don't, that one didn't compute. - So this function that we just created
[96:45] is gonna take a to-do, which we're doing. We're taking the to-do in as parameter,
[96:50] and we're gonna return the to-do's title. - Okay.
[96:55] - So inside the curly braces in the middle, return to-do.title.
[97:00] All right, now it might throw an error because it's returning array,
[97:16] or I can't remember, it might work. So let's save that and don't refresh the page.
[97:21] Let's just scroll. Yeah, you did.
[97:26] All right, so these are titles, but you can't see that they're different.
[97:30] So let's make each one of them an H1 tag. So go back into your code.
[97:35] So wrap it in an H1 or H3, maybe. Actually, no, the cards were H2, so let's do H2.
[97:44] - Okay. - You don't wanna wrap the return statement though.
[97:50] - That's the to-do title? - Correct.
[97:53] - How did I just do that, and then I'm going blind? That is not good.
[98:07] - And now it may give you an error because right now it just thinks
[98:17] that you're asking it to render out the text to-do. It doesn't know it's dynamic data.
[98:21] So you gotta put it in the curly braces. So put to-do.title in curly braces.
[98:25] There you go. Boom. - Oh.
[98:35] Okay, that's cool. - Yeah.
[98:40] Now, if you take a look back at it, you wanna recap again and review this?
[98:47] - Yes. - So from outside to in.
[98:51] This is a good point from Anthony. This is 90% of all React development
[98:55] you'll do in the future, this process. And he's right.
[98:58] This is a lot of React development. Taking information in, state of a component,
[99:05] taking it in from somewhere, maybe from an API or maybe from outside somewhere,
[99:09] manipulating it, rendering it out. It's a core of it.
[99:13] It's a really important part of React development. - Okay.
[99:19] - And so looking at the curlies again, curlies outside say evaluate this
[99:24] and give me some kind of HTML. To-dos is an array, run map on the to-dos.
[99:31] So for every to-do in the array, transform it using this function that I'm giving you.
[99:38] Transform it, you take a to-do, you spit out an h2 tag with to-do.title in it.
[99:45] Boom. That's the whole thing right there.
[99:48] - So that's all making sense. And then if I wanted to make it into the cards?
[99:56] - You're gonna do that. So let's do that.
[99:59] And I think your instinct is leading you in the right place. So do you wanna just try it?
[100:03] - Yeah. - Do it.
[100:07] - Okay, so it's not gonna be clicking somewhere.
[100:15] So I don't think I need a link. So I'm gonna do this link.
[100:22] - Well, actually, taking a step back. If you delete that for a second,
[100:32] and let me see if I can guide your thinking a little bit. - Sure.
[100:36] - In this statement, we're saying do this for every to-do.
[100:45] So do you wanna put the HTML code outside this block or inside?
[100:55] Or in other words, do you wanna do all that HTML for every to-do
[101:00] or do this loop for every to-do inside the HTML? - I wanna take all of those to-dos
[101:08] and make them different boxes. - Right.
[101:11] - So all of these show up as boxes. - Right.
[101:15] So what you wanna do is you wanna take this, you know, big chunk of HTML, A, HREF, whatever,
[101:22] and you wanna do that for every one of the to-dos, right? - Yeah, but that sounds really hard.
[101:29] - To have that card, right. So take a copy of one of these HTML chunks,
[101:34] and you're gonna put it inside the return statement because you want it inside the map function
[101:39] 'cause that's happening for every to-do. - Oh, okay.
[101:46] So it's this. Wait, wait, wait, let me.
[101:49] - Oh, you're doing great. - Let me do some.
[101:52] So, I'm gonna, I'm gonna build it and then put it
[102:00] where it's supposed to be. - Absolutely great approach, too.
[102:04] - And so I want this inside of the HTML. I don't know why there's a rar.
[102:15] - That's a HTML character for like the little arrow, I think.
[102:21] - Oh, okay. And then we, ah,
[102:26] we can call this all of. (mouse clicking)
[102:33] Come on, what is this called? What line am I on, somebody?
[102:41] Use effect? No.
[102:45] Which one did we use for this? This was the use effect?
[102:50] - We used the use effect and a fetch. - Okay, which ones are these for?
[102:58] Was it for use effect or was it for a fetch? Was it for use state or use?
[103:04] - This is the result of the API call. I'm not sure what you're asking.
[103:08] - Trying to say that these are all of the use states or the use, like what we would have used them for,
[103:17] but that's okay. - These are all the to-dos.
[103:20] - Okay, we'll just leave it at that. That works for me.
[103:26] And then the class name is card. And then do I link this part to something?
[103:31] - If you want to. - But I don't need to link it to some,
[103:36] well, I guess I could link it to this. - You could leave it there just so,
[103:40] because they're already links and the links have the styles.card style on them.
[103:45] So I don't think it'll hurt to leave there for now. - Okay, and then I take all of this,
[103:52] delete it, and then I replace this with all of it? - I don't know, let's try.
[103:59] - Oh, where did you go? - Don't worry about that warning.
[104:11] I could explain that in another segment. - I just don't see, oh, it's right there.
[104:20] Okay, well, now I want to see what it does. Oh, it did it.
[104:23] - Look at that. - Okay, that was fun.
[104:29] I mean, there are some CSS things that I would definitely end up wanting to fix,
[104:34] but it did it. - You want to do one more thing?
[104:40] - If you have the time, sure. - One more thing, and it's going to be a fast one.
[104:44] Go into your code. Instead of making it say all the to-dos,
[104:49] let's make it have the to-do description. - Okay, and Anthony was saying I don't think,
[104:59] he doesn't think I have a useState mental model yet, so that's why the question is confusing.
[105:09] - I'm not sure which question he means, but I'm not surprised.
[105:13] It can be a little confusing, so. - Okay, and then we wanted to put all of their abouts, right?
[105:22] - Take a look at the JSON object that you pulled up there. Yeah, so what do they have?
[105:30] Oh, actually, you know what? There's no descriptions in there, I'm sorry.
[105:33] - But we could put their IDs. - Absolutely right.
[105:37] Go for it. - So if I wanted to do that, it would be,
[105:44] well, hold on. I would want to do this one here and their IDs,
[105:50] which would be to-do.id squiggly space or squiggly? Do I need space?
[106:13] Do I need space right here? - I don't know.
[106:16] Try it. - Okay.
[106:18] - Give it a break. - Yay.
[106:22] Oh, let's get rid of that arrow. That looks dumb.
[106:27] - See, now you can have fun with it and kind of like change it to how you want.
[106:35] - I think you created a monster. - Good.
[106:40] - We need more time. - Okay, I can leave it like that now.
[106:55] I was like, I did not like the yellow, but it was like a good.
[107:01] And then, so, would, have you heard of,
[107:10] and Anthony, I might need your help explaining this one because now I'm just trying to connect dots.
[107:15] Have you heard of Bedrock? Is it Bedrock CSS or Bedrock HTML?
[107:21] I'm not sure which it's considered. - I have.
[107:24] I don't know too much about it, to be honest with you. - Okay.
[107:27] The reason I'm asking is I'm just wondering if it would be something for the web layout
[107:33] to fix these boxes. - Well, that's a fork in the road
[107:41] because you can fix the layout with just CSS before you like add another framework or library for it.
[107:51] And it's up to you, you know? Like you can definitely figure,
[107:55] I believe you could figure out if you wanted to how to fix this with just CSS.
[107:59] The question is, do you want to learn more CSS or do you want to go in a different direction?
[108:05] And I'll leave that totally up to you 'cause I do have to jump off in a second.
[108:09] - Yes, so do I. I think it's more of this is,
[108:13] and let me make sure I save this before I take it back to us. It's more of just, I'm not fully seeing,
[108:22] like I'm very much enjoying learning each of these platforms and like different ways of doing things.
[108:29] It's I'm still not to the point with when you connect them, why you would connect them together.
[108:35] That I still struggle with. So that's why I'm wondering about Bedrock,
[108:38] not that I necessarily want to learn CSS, but oh, hey, I learned CSS.
[108:43] So would this be something that would go in here kind of thing?
[108:47] There's still so much learning, but this is exciting. And a lot of it made sense.
[108:54] I will say at some point, we're going to have guests on here to talk about APIs,
[109:00] but it might be from where I work. So that way they can explain APIs from their point of view,
[109:07] but we will see, 'cause I'm excited to talk more about APIs.
[109:11] I think this is my second or third time doing an API or an SDK.
[109:17] So it's definitely, seeing it actually happen seems completely different than just knowing about it.
[109:24] Spacing words now. But whatever, y'all get what I mean.
[109:32] It's been, my brain is definitely going to mushy mush now, but in like such a good way, there's,
[109:38] I'm really excited about what we built. Thank you.
[109:40] And knowing that there's a JSON placeholder. - Yeah, extremely useful tool.
[109:50] I use it whenever I'm proof of concepting something. So, but you did great today.
[109:55] Congrats to you, pat yourself on the back. You picked up some things really well,
[110:01] hopefully at a pace that's useful to you. And now you have something you can play with more.
[110:06] - Yes, yes, and thank you. And Anthony, really quick, just as a heads up,
[110:11] somebody from Postman is actually planning on coming on to talk about GraphQL.
[110:18] So, well, everybody, please leave us comments. Let us know what you think.
[110:24] If you want to hear more about a certain subject, make sure you click follow and share these.
[110:30] So, thank you all. Have a wonderful day, beautiful humans.

