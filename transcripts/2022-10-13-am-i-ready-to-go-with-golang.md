---
showLink: "https://www.youtube.com/watch?v=BUhAghCenHo"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "am-i-ready-to-go-with-golang"
title: "Am I ready to Go with @golang?"
publishDate: "2022-10-13"
coverImage: "https://i.ytimg.com/vi/BUhAghCenHo/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to a later episode and another episode of Teach Gen Tech.
[00:09] If anybody was wondering, I'm not always the greatest at communicating schedules,
[00:15] is really what it comes down to, but we may be changing times altogether.
[00:20] If this time works better for people, I don't know. Tell me what you all think.
[00:25] Today, we have Eddie on the show. Eddie, please introduce yourself and what you're teaching us today.
[00:31] >> Yeah. My name is Eddie Zaneski. I'm a software engineer at a company called Chain Guard.
[00:37] I'm a maintainer for the Kubernetes project and the SIGSTAR project, which are both pretty big Go projects.
[00:43] I'm teaching you Go. >> Yay. I totally forgot to change the background, y'all.
[00:50] You should definitely see that here in a moment, if I can click the right thing.
[00:56] That's actually, so y'all, Eddie was open to doing,
[01:01] here we go, learning about Golang. Eddie was open to teaching basically anything.
[01:08] He was just like, "Whatever, let's just do this." I know that I do a lot of JavaScript,
[01:13] also a lot of Python and different frameworks in JavaScript, yet I keep hearing about Go.
[01:22] I just keep hearing about it. Eddie was actually the first person to tell me about Go when we met at, oh, goodness.
[01:31] Was it the Orbit meetup? >> Yeah, it was.
[01:34] >> Yeah. The Orbit meetup in Denver. It was right when, this was probably three or four months ago,
[01:40] I'm trying to get into DevRel, and he was talking about Go and I'm like, "What's Go?"
[01:47] I didn't even know it was a language. There's a lot of languages I don't know that are a language,
[01:51] so I'm excited to hear about it because it's, I think I just heard of a company called Charm,
[02:01] and I think they build on Go too. >> Yes, they do.
[02:05] >> That's another reason why I was very curious about it because I was like, Charm looks so cool,
[02:10] plus they have the best names ever. I saw them on a live stream with GitHub with Roselle,
[02:15] and I'm like, "I want to be able to do that someday because they have the coolest names."
[02:21] That's how they got me caught, but what up, homie?
[02:26] Yay. Somebody was able to change their schedule. I know we talked about that we're going to work on doing this with VS Code,
[02:37] and then I completely forgot what the plugin was. Let me Google that.
[02:43] >> If that doesn't work, we can use my little editor thingy.
[02:48] >> Okay. Well, I will share my screen so people can actually see this happening. Y'all, I do think being able to Google is a skill,
[03:06] because me and my Googles don't always work, which I find pretty hilarious,
[03:11] but it's not always hilarious for everyone else. VS Code live share?
[03:23] That's what we're going to go with. Yay. Do you have the link in the Marketplace?
[03:36] This is Marketplace? This is Marketplace. Okay. I'm sending you this really quick.
[03:40] >> I'm installing VS Code. >> Oh, hey. Yeah, that's you.
[03:45] >> Just so everybody else knows, I asked to do it in VS Code still,
[03:53] even though there's other options. Because something that I've realized that does make it harder to learn,
[03:59] is having to always switch tools. Because then I'm learning the different tool,
[04:06] where a lot of other people have used the tools I use, it's just not their go-to tool.
[04:13] >> That's why I use Vim everywhere. >> Oh my gosh. Me and Vim.
[04:21] Yeah, I don't know. I don't know about that. >> All right.
[04:25] >> Laura, I was telling you about when she's on for Python, and I ran into Vim.
[04:31] I didn't mean to, I was very stuck. >> All right. Let's see. Live share.
[04:41] >> Okay. I'm installing that. >> Sweet.
[04:49] I need to make a folder and things and stuff. >> Okay. I have this installed.
[05:14] >> Sweet. Do you want to make the folder, or do you want me to make the folder?
[05:18] >> Let's have you make it. >> Okay. It's weird.
[05:21] I automatically went to terminal to go make a folder. I don't know if that's normal.
[05:25] >> That's what I do. >> I feel like enough people have been on that,
[05:31] they've like teach me how to do this, that I'm like, "Oh, this is weird."
[05:35] Okay. Code. Although I was just on a PC, and is it still MKDIR to make a new folder?
[05:50] >> Yes. >> Okay. We will call this.
[05:57] >> Nice. >> Then something that I was talking about last stream,
[06:11] was there is this fee. Well, I guess I should ask this because this screwed us up when I was
[06:22] learning a bit of spelt is, should I go ahead and create a repo here through command line first,
[06:30] or should I install and then make a repo? >> I would just do it locally first.
[06:41] >> Okay. Easy enough. I like that idea. All right.
[06:45] >> But fun fact, that CLI tool is actually built in Go.
[06:50] >> That's fun. >> Okay. What? Why?
[07:03] >> Exit. Okay. Yes. Oh my goodness. Yes.
[07:18] How do I share this now? >> I think it's at the bottom there.
[07:23] >> Oh, live share. Where it says live share? Yeah, that would be.
[07:26] What? Already signed in. >> Okay. I have to do that too.
[07:33] >> Authorize. >> What? It signed me in with GitHub and now I'm at GoDaddy Office 365,
[08:00] and I have Gmail. This is confusing.
[08:05] All right, let's see. Starting, signing in, cancel, go.
[08:14] We'll just start from scratch really quick. >> Do what every developer does and turn it off and on again.
[08:35] >> I think I have to have VS Code open for this, but we'll find out.
[08:43] >> Yay. Live share. We've signed in with GitHub.
[08:53] Oh, wow. Please be my friend. Okay. Copy.
[09:11] >> Paste. >> I'm going to click it and hopefully it gave me.
[09:19] I can continue right from the web browser. That's cool. >> Oh, hey.
[09:25] >> Let's see if this works. Am I connected?
[09:32] >> I think so. >> Yes.
[09:37] >> Hooray. >> Hey, we got there.
[09:40] Yes, homie, I totally think that my Mac just hates on me right now, because I just got it back yesterday.
[09:51] I spent many hours at the Apple Store the last two weeks. It's been fun, but I'm glad to have it back.
[09:59] I guess I need that back over here because I need to install it. >> Do you have Homebrew installed?
[10:08] >> Not yet. >> Okay.
[10:11] >> That was on my to-do list today. Am I going to need it?
[10:16] >> No. >> Okay. I don't know which.
[10:26] >> Do you have Apple Silicon or Intel? >> Intel.
[10:30] >> Then the x86-64 one. >> Okay. Thank you.
[10:35] >> At least it's letting me do this this way instead of over man-line since I don't,
[10:51] because you have to have, what does Homebrew do?
[10:56] Since you're here, I'm just going to ask you random questions as we go. >> That's fine. Homebrew is a package manager.
[11:02] You would normally just type brew install go, and it would do all of this for you.
[11:07] The best part about using a package manager to install things is when you want to clean them up.
[11:12] Package manager will keep track of every file that gets put anywhere on your system.
[11:16] If you decide, I hate go, I never want to do it again,
[11:19] you can brew uninstall go, and it will clean everything up.
[11:23] >> Interesting. How do I say the name? Canny is what we're going with.
[11:36] My bad if I totally butchered your name, said it's a really bad package manager.
[11:42] But Volta only does it for JavaScript and Node, but isn't that a package manager too?
[11:51] >> I've never heard of Volta before. Is that an NPM client?
[11:59] >> It is a JavaScript tool manager. >> Oh, okay.
[12:07] >> Sure. >> Yeah, you could consider that.
[12:11] That's very specific for Node it looks like. >> Yeah. Okay. Oh, yeah, that would be cool.
[12:19] Thank you, homie. Y'all, I did have a to-do list that I was going to do,
[12:24] and then Eddie and I figured out schedules and we're like, we're doing this today.
[12:27] But Anthony created a gist for me to be able to get started on all these installs today.
[12:39] I closed it, but I think Go is here now. >> Let's see. Can you open your terminal up?
[12:47] >> Yes. >> Type reload.
[12:55] >> That might be a different thing. Just close this and open a new one.
[13:01] >> Easy enough. >> Yeah.
[13:03] >> We'll do that. This was on my to-do list today too, was to actually,
[13:17] there's so many different versions that you can do with this. I was like, that's so cool.
[13:22] Then it won't be boring. >> All right. You want me to
[13:26] teach you lots of different things, right? >> Sure.
[13:30] >> One of the biggest tricks that I do a lot of mentoring for different code schools
[13:36] and I work with a lot of beginners. Typing out paths in your terminal
[13:41] is not something you want to spend your time doing. Just type CD for me, you hit "Enter".
[13:48] That's going to go back to your home directory. If you do CD and then space,
[13:54] hit "Tab" on the keyboard, and then type in DE,
[13:59] then hit "Tab", and then hit "Tab", and then CO, you may have to do D.
[14:07] Cool. Then tab again. Yeah, you got it. You want to tab complete everything.
[14:13] You want to type as little as possible in that terminal, and most commands will actually have
[14:19] tab completion to help you with the command that you're typing. It'll know the flags to pass it or it will know what it can do.
[14:27] >> That's cool. >> Yeah. That's looking in your path.
[14:31] It's a list of places to look for programs to call. That is showing you all the programs that you can call.
[14:38] Those are all named MK something. >> Yeah, I was seeing how it would come up with MK directory.
[14:45] Make directory. Yeah, this was fun. Then I'm trying to think of how would you check to see if Go installed?
[14:59] >> Yeah. We're going to type which Go? >> This which?
[15:04] >> That which. Which which? Cool. Which is a command.
[15:09] I mentioned that path thing before. If you type echo,
[15:13] space, dollar, capital path, dollar sign, all capital.
[15:21] This is going to show you your path. This is a list of folders on your computer.
[15:26] Now, whenever you run a command, it's going to search through starting from the left to the right.
[15:31] You see here, Go has actually been added to your path at the end. >> Interesting.
[15:39] >> The which command, so you can have conflicting programs sometimes.
[15:43] You can have multiple programs named Go, for example. Typing which Go will show
[15:48] you which command is going to be called when you type Go. >> All right.
[15:54] >> You can do which-a and it will show you all the programs named Go. I go on forever. But you have Go now.
[16:01] >> Yay, we can go. Let's go. >> Okay. Let's start with Go version.
[16:07] Just type that out. Make sure. Cool. That's the other way.
[16:13] We checked if the binary is there and now we're checking to make sure you have the latest version installed.
[16:17] >> Yay. >> We mentioned earlier,
[16:22] so one of the big differences between Go and JavaScript is going to be that Go is a statically typed language.
[16:28] Statically typed is, in JavaScript, when you write a function, you just say,
[16:32] "Hey, this takes in a variable." You don't really tell your program what kind of variable it's
[16:38] expecting and there's no enforcement. I could call your function and give it
[16:42] a string or a number or a Boolean, and it'll just take it.
[16:47] It could be what you're intending and it could be what you weren't intending.
[16:51] But it will call it and run it until maybe something breaks. That's what we call dynamic typing.
[16:57] Python is the same way. TypeScript is like
[17:02] a statically typed version of JavaScript that has some other features built in,
[17:06] and Python actually has some typings now that you can add in too. I did a lot of JavaScript back in the day
[17:13] and moving to a statically typed language, that just makes you feel better
[17:18] because your editor is going to do magic stuff for you, because it's going to know what your function is expecting to take
[17:25] in or return and can help you with more auto-completion. >> That being said, and I don't think
[17:32] these have anything to do with each other, but for some reason,
[17:36] it's stuck in my head as somehow connected of a compiler language, and I don't know what else there is.
[17:46] What is a compiler language? >> Yes. Go is a compiled language.
[17:52] When you're using JavaScript, for example, that's what we call an interpreted language.
[17:57] There's a JavaScript interpreter that will slurp in your JavaScript text file and it will read it and execute it,
[18:04] and it'll do all sorts of different parsing and all this jazz. But for that JavaScript code to run,
[18:11] you have to have a JavaScript interpreter. >> Right.
[18:14] >> Same thing with Python, you have to have Python installed. With a compiled language like Go,
[18:20] you can compile all of your code, your whole project down to a single binary.
[18:25] I can send that to you, and as long as you have
[18:27] the same architecture that I built that binary for. If you have a Mac on Intel.
[18:31] I can build you a binary, and you don't have to have Go installed actually.
[18:35] It'll just run because Go binaries have a runtime built in. But it's usually compiled to
[18:43] some type of machine language that something can run. Like Java, for example, is a compiled language technically.
[18:50] It compiles out to Java class files that a JVM will run. Then there's also the whole thing of transpiling,
[18:57] which is big in the JavaScript world, where you can transpile your new fancy JavaScript code
[19:03] down to older code that can run in older browsers. It's going from one thing to another.
[19:08] But compiled is just different parts of the compiling step or linking and all this other jazz.
[19:14] But it's just the idea that you can build down to usually a single binary or some byte code.
[19:21] >> That makes some sense. It makes sense, but it doesn't make sense.
[19:27] Then if I go back to, and what did you call that Go is,
[19:33] that JavaScript stunt again? >> A statically typed?
[19:37] >> Yeah. So static types. Going back to that just to repeat back is,
[19:43] that means that compared to also like Python. In Python, you can tell it to share
[19:53] or this exponent can or sorry, I'm trying to think back on what we're currently working on.
[20:02] We can make five equal a food, for example, or something like that.
[20:11] So it can be very open and to discretion where Go is not like that. >> Yeah. Go will be very strict.
[20:19] So when we declare a variable as a string, it can only ever be a string.
[20:23] >> Okay. I'm starting to connect. >> Yeah.
[20:26] >> I'm starting to connect. Okay. >> Let's do one more thing in your terminal here.
[20:31] Let's initialize a Go project, just like you would run like npm init.
[20:35] With Go, we're going to do go mod init. Then we're going to give it a project name.
[20:42] This is generally, most Go projects are just GitHub paths. So do like github.com/yourusername/letsgo.
[20:52] >> You said github.com/yourusername/letsgo. >> Most Go packages are URLs.
[21:05] Do slashes, sorry. >> Okay. Yeah, that makes more sense.
[21:11] >> So username and then do the project name. So whatever you want to call it.
[21:17] I'm still having fun with letsgo. >> That's great. Cool.
[21:22] >> That was fun. >> Yay. So now see we have that Go mod file.
[21:26] That's going to keep track of our dependencies and build our project.
[21:31] It's a lot better than how Go used to be. >> Okay. So that created the project?
[21:41] >> Yep. Look at me, I can type around in here. Yes. It's a lot of fun.
[21:48] I personally would have no idea where to go with this because I'm used to even in all the JavaScript frameworks that I've been learning,
[21:58] it would have way more files and a lot more content in it just to install something.
[22:04] >> Oh, yeah. Well, we'll get to dependencies at some point. One of the big differences is specifically between Go and JavaScript,
[22:11] is Go has a very large standard library built in. JavaScript is a very small standard library and API surface.
[22:21] Most Go developers will use the baked-in things because they're there. I don't have to go install a library to build a web app.
[22:31] I can just use the standard library because it's real feature packed. So you actually wind up using a lot less dependencies when you're writing Go.
[22:38] >> Okay. >> So let's create a new file.
[22:41] We'll just call this main.go and click that "Install" button there. This is going to install some Go tools and stuff.
[22:56] Yeah. Do you install all? Let's see if that works. Yeah, there we go.
[23:09] Oh, God. >> It's doing all the things.
[23:15] >> Yeah, that's okay. You need a C compiler, it looks like. >> I should really just start adding to the list of things I need to install.
[23:25] So any that you suggest, I will share with you what I already have suggested,
[23:30] and Homie has one for me now. So I'm like, I'm cursed with technology.
[23:38] So me and having to get a new laptop or hard reset my laptop is not a new thing. So I really should come up with a list that is like,
[23:46] make sure you do all of this, Jen, to make your laptop work for you.
[23:50] >> Yeah. Well, one day you'll transition to a point where you can get a new laptop, probably run one script and you'll have
[23:57] your full work environment set up because at least that's what I have. >> Oh, that's cool. Homie has a question.
[24:04] Wondering when you started, what influenced you to become a Go developer?
[24:09] Do you use JavaScript as well? >> Yeah. So up until,
[24:14] I don't even know when, 2016-ish. I would have considered myself a Node developer.
[24:22] I did a ton of back-end JavaScript. I also played around with React at one point.
[24:27] It made me learn a little bit more about front-end because React is a pretty fun thing to do.
[24:32] I started working in the containers and Kubernetes and Cloud Native World, and most of that tooling is all written in Go.
[24:39] So that just led me to learn Go and start working on things like Kubernetes and Terraform and some other big Go tools out there.
[24:48] Yeah, I love it as a language. I still love JavaScript as a language.
[24:52] It has its faults just like everything. You'll learn a lot of the Go faults pretty quickly.
[24:57] But yeah, when I was younger and immature, I was just like, "Oh, PHP is awful,
[25:04] JavaScript is awful," and then you just get to the point where you're like, "These are just tools," and the more tools you have in the toolbox,
[25:11] it's way better. For certain things, I would still write a web application in Node over Go,
[25:18] if I needed to prototype something much quicker. You'll feel the pain at some point.
[25:24] >> It's been cool where I think I've learned more. Yes, it can be very confusing as I'm getting started,
[25:34] but looking at Python compared to JavaScript, I'm understanding JavaScript better.
[25:40] I really hope you don't take 15 minutes. >> We can switch to probably mine if we need to.
[25:48] But on that note actually, one of my favorite classes when I was in school
[25:52] was called Principles of Programming Languages. The whole point of that class is it
[25:57] taught you how to learn programming languages, which is exactly what you just said.
[26:01] The more you learn, the easier it is to learn new languages. I did a Ruby many moons ago,
[26:09] and at one point I had to write some Perl, and I'd never done Perl before,
[26:13] but Ruby was inspired a lot by Perl, especially their syntaxes and variables.
[26:19] I was like, "Oh, now I get where Ruby got this from. This is familiar to me.
[26:23] I can figure this out." >> Yeah. Next week we're going to have,
[26:30] Brittany was on Tuesday talking about Svelte, and then Anthony who has been on the show quite a bit.
[26:38] I like to call him my Internet big brother. Maybe we should switch to your computer because mine is
[26:50] just struggle busing. So next week, they're going to compare and
[26:59] talk about React versus Svelte. I'm really excited because there's,
[27:05] oh, you might know this. Is there some type of platform
[27:11] that you're aware of for VS Code or something that tells you what language something's written in?
[27:18] Because in JavaScript, you'll have some HTML, you'll have some CSS,
[27:23] you may have TypeScript and JavaScript. It would be really helpful if a line just told you like,
[27:29] "Hey, if a line is this color or has this dot or something, then it's TypeScript."
[27:37] Just to learn because I'm like, I can read the code and figure out what it's going to execute,
[27:42] but then it's not always making sense that what languages are going into that.
[27:47] >> Yeah. There's parsers, there's syntax, highlighters, and other tools that will pick it up.
[27:52] You could probably paste it. There's probably a web app you could paste it in,
[27:56] and it'll tell you what language it is. >> Okay. That's cool.
[27:59] >> I'm getting this started. >> Cool.
[28:01] >> Sorry, what were you going to say? >> I don't know.
[28:06] That is the fun part of live streaming. It's like, I don't know, it's not going to be perfect.
[28:13] It's cool. It's cool. I do want to go back to-
[28:17] >> I sent you the link. >> Sweet. Is it going to open in my VS Code or my web browser,
[28:28] or what are you going to do? Yeah, I don't know. I'll just move it over here.
[28:34] Continue in web. Let's do that because now you want me to sign in again.
[28:41] >> Goodness gracious. >> This highlights a great pain point when it
[28:49] comes to getting started with developing. It's gotten so complicated.
[28:52] There are other tools that when I work with students, I usually use like REPL tools or like one-off editors,
[28:58] but getting a development environment set up is complicated. >> Right. I will re-share my screen here shortly.
[29:09] >> There we go. Yay. >> You in here?
[29:13] >> I believe so. Helps if I actually make the right screen.
[29:17] Now it's really big. Yay. >> What was your GitHub username?
[29:27] >> Jengenod. >> Jen.
[29:31] >> J-U-N-O-D. >> Let's go. I created this GoMod file.
[29:38] We should be on the same page. I see it.
[29:48] >> Oh, there we go. >> Hey, okay.
[29:50] >> Yay. >> I'm going to create that main.go.
[29:54] Open that up. The way Go does everything is with packages. Package is just going to be a folder in our case.
[30:06] It's like a folder of software. You get sub-packages and other complicated stuff.
[30:12] But for our point, what I want to say, a package is a folder.
[30:15] Our first package is going to be the main package. If you want to go type in their package main,
[30:21] and main is a special reserved package name. I see it even knows it.
[30:26] This is the entry point to your program. This will be like your index.js.
[30:30] This will be the file that all your Go code is going to start in. >> Okay.
[30:36] >> We also need to declare a function. To do that in Go, you're going to say func,
[30:43] and then space and call this main. Again, special function name.
[30:50] Open, close parenthesis, and a little curly brace. Outside the parenthesis, sorry.
[30:59] >> Like that? >> No, like you would in JavaScript,
[31:05] where you open it curly. >> Okay, there we go. I like
[31:10] how it auto-creates the other ones, but it doesn't auto-delete them.
[31:13] >> Yeah. I'll just clean this up a little. There we go. Cool. We got our func main.
[31:20] Let's see because my name is there. If we save this file and run it right now,
[31:27] it should actually just work. Actually, I don't think you have a terminal, do you?
[31:33] >> Can I open a terminal? >> Interesting.
[31:37] >> Let's see. >> No, no.
[31:46] >> How do I open a terminal in VS Code? >> I know in VS Code itself, but I'm, oh, there you go.
[31:59] >> Yay. Oh, yeah, you're using the real VS Code. >> Can you see that? Oh, you can. Okay, cool.
[32:06] The problem is a little messed up, but it'll work for now.
[32:10] Now, if we run go run on this main.go file. Oh, we didn't save it. We need to manually save it here.
[32:19] Cool. Go run is like your almost interpreter. It'll compile the program and then run that executable.
[32:30] We say go run and it just ran the file and didn't do anything yet.
[32:34] Let's make it print out Hello World as is tradition. The way we do that with Go is with the package
[32:41] called format or fmt fmt. If you inside that main function,
[32:47] and you just come down a line and then do fmt. >> Fmt, fmt.
[32:56] >> .println. Yeah, you use that tab completion that comes up. There you go. The Go tooling is really cool.
[33:06] It imported the package for you because it knew what you're using.
[33:10] If you open a parentheses now, it's going to tell you everything about
[33:15] this function and everything it takes in. This will take in anything,
[33:20] which is like a wild card type in Go. >> Will it automatically do the print because it's in here?
[33:26] >> Yes. >> That's not going to work. Can you guess why?
[33:37] Click away and let's save that. Let's see if your editor yells at you.
[33:44] I need to save it. Well, I have a squiggly red line
[33:49] under what's inside this function. Oh, because I didn't put these things.
[33:56] >> Yes. >> These things, that totally made sense.
[34:00] >> That's not going to work either, but I'm not going to expect you to guess this one.
[34:03] There's a difference between a single quote and a double quote in Go. >> I didn't know that. That's weird because the rest of them are pretty interchangeable.
[34:15] >> A single quote in Go is for what we call a rune, which is like a single character. It's like a char.
[34:22] >> Okay. >> Double quotes are for a string.
[34:25] Now if we save this and run it, we will see a message printed out.
[34:31] >> Yay. >> We can also do a Go build,
[34:36] and that's going to build us the file name there. You see let's go with compiled.
[34:42] It's that green tells you it's an executable in your terminal. I can run that and it'll run as the same.
[34:49] If I could actually send this to you, if I built it for Mac,
[34:53] I'm running on Linux, but I could build this for Mac, send it to you in an e-mail and you could download and run it basically.
[34:59] >> Interesting. >> Yeah. It's cool. Let's see.
[35:05] This is probably one of the smallest Go programs we can do. We can look how big it is.
[35:10] 1.8 megabytes, which is big, and that's one of the complaints that you hear about Go sometimes.
[35:17] Go does wind up with a little bit bigger binaries because the entire Go runtime gets compiled into your program.
[35:25] >> This is making sense. I guess now I just have a pure curiosity thing of actually seeing it in action.
[35:38] Other than something small like this, are you working on something that you may be able to show us
[35:50] and what some of the functions look like in Go that you're currently building?
[35:55] >> Sure. >> You can open up a project.
[35:59] >> You can share your screen and let me know. Because I feel like that would be really cool and something I actually
[36:05] should ask for more often is actually seeing how. Yes, we're starting to see how it looks
[36:13] like with the getting started with it, but how people are actually using it,
[36:19] especially since you said this is how they build Kubernetes. Homie, you said great question mark.
[36:28] Now you got me lost. >> All right. I think I'm sharing my screen.
[36:38] Hey, there we go. Oh, I think you're sharing yours.
[36:44] No, that is my screen. Hold on. What's going on?
[36:48] That's the wrong screen. Let me share my other screen.
[36:53] The perils of two monitors. >> Oh, yeah. I have two external monitors and my own,
[37:02] so I get mixed up all the time. >> I can show you some Kubernetes code,
[37:13] which is definitely a complicated code base, but it'll give you a good idea.
[37:21] KubeCTL, which I think you've used before, the command line tool for Kubernetes?
[37:27] >> Not yet. >> Not yet. Well, KubeCTL is the command line tool for Kubernetes,
[37:32] and that's what I primarily work on. The way this is structured is we
[37:37] have different sub-commands in here. I can see commands for creating something or deleting something.
[37:45] I can show you what the command for deleting looks like. We got all these imports.
[37:52] These are like your built-ins, so they have no URL in them.
[37:58] These are part of the standard library, and these are external libraries that we've pulled in.
[38:04] These are all the internal Kubernetes libraries that we use to build things.
[38:10] Let's see what's exciting looking thing. This is a type,
[38:18] this is a struct in Kubernetes. We talked about types,
[38:22] so you have your basic types of string. We have six different number types.
[38:29] We have integers that are 64 bits long, integers that are 32 bits long,
[38:34] I think there's a 8-bit integer, and then there's unsigned integers which can't be negative,
[38:41] but they can hold a much larger number because they're much longer. Then there's Booleans, and we have a whole bunch of other types.
[38:49] Another one of these basic types is what we call a struct. This is basically the closest you can get to
[38:54] the class you would use in JavaScript or Python. Python has some other conventions that you can use,
[38:58] but struct is like an object. It's like a JavaScript object.
[39:03] This is just declaring a type named delete options for the delete command here,
[39:10] and it is a pipe struct. Then this is declared with a field name.
[39:18] These are the fields that are in the struct, so it has a label selector field with the string,
[39:22] that's a type string. Delete is a Boolean,
[39:27] which is delete now, by all these different types. Integers, time is a duration.
[39:33] This is another type. This is how we represent time and go. Making sense so far?
[39:40] >> Yes. >> Cool. This is the constructor for that new delete command.
[39:49] When this gets added to the whole CLI and runtime, this is what it's called.
[39:54] It takes in this factory type here, so this is from another package,
[39:59] it's command util, and it is a factory, which is an interface,
[40:04] which is another type in Go. Interface is like a contract that your struct can
[40:12] implement and it can say it fulfills that interface. We don't have to talk too much about them today.
[40:19] Same thing here, this takes in a stream. This is your standard in and standard out.
[40:25] This is what your terminal will read in or print out. That's a struct.
[40:30] >> Interesting. That does make me think of another question. Can you show us side-by-side or an example
[40:42] of how Go makes you use those specific? You can't have the same type of variables
[40:53] or changes that you would in JavaScript and what those would look like?
[40:58] >> Yeah. Let's pop back to your editor here and make this bigger. Does that look okay?
[41:13] >> Yes. Thank you. >> Yeah. I can write a function here.
[41:22] You should be writing this, but we'll give you a pass now because of your editor situation.
[41:29] I'll just call this function greet. This is going to take in a name,
[41:34] which is a string, and it's going to return another string.
[41:39] That's it so far? >> Yes.
[41:44] >> This is how we declare the return type. This says my function must return a string.
[41:49] If you see here, it's pissed off because we're not returning a string yet.
[41:53] Missing return. If I go to return, let's say the number 3,
[42:00] it's going to be pissed off again because you cannot use 3 as an integer as
[42:06] a string because it knows it's supposed to return a string. Immediately, we can see the protection that's put in place.
[42:12] Now, let's call that and let's just say, we'll return, I'm going to join a string.
[42:20] We'll say, hello and your name. I'm going to pass that name there.
[42:27] This is like string interpolation. You can do this in JavaScript and Python.
[42:31] This just says, percent s says, "Hey, plug in a string value for this token here."
[42:37] Use name as that. S printf is going to return us a string.
[42:43] It's not popping up, but there you go. This is like, we call this like format string.
[42:54] Now, inside here, let's just call greet and we'll say, we'll put jet in there.
[42:59] That make sense so far? >> It does in the fact that it sounds weird,
[43:05] but it doesn't. It makes sense, but this is I think the cool thing about seeing
[43:12] something so new of it's going to take some time to sink in. This is one of my favorite things
[43:22] about learning this tech side of things, because it's so simple,
[43:28] it makes sense, yet at the same time, it doesn't make sense.
[43:31] I think that's a bit of where I'm at. Yes, it makes sense to,
[43:38] it doesn't make sense. >> Okay. Well, if we run this,
[43:42] you'll see it works, says hello, plugs in the name.
[43:46] But again, if I try to pass three into that function, it's going to be mad.
[43:52] It's going to tell me, you can't use three here, it's supposed to be a string.
[43:56] I'm not used to having to save a file. There we go. If I try to run it,
[44:02] it's going to give me that same error. Cannot use three, which is an untyped integer
[44:06] as a string value, the argument. >> Okay.
[44:10] >> This is a simple example, but you can see this is giving me protection.
[44:15] I'm not going to hit any bugs where my function is expecting a string and I give it a three,
[44:19] because it won't run. >> Now I'm curious. If we do that though,
[44:26] it'll still turn it to a string, so therefore it'll work.
[44:28] >> That'll be the string three, yeah. >> Okay, cool. Yeah, it makes sense.
[44:33] It makes sense. I'm getting there. >> Okay. Where do you want to go next?
[44:39] >> I don't know. I don't know what to ask, because it's like at the same time.
[44:44] This happened, so I told you how last week I started talking about Kubernetes and Docker,
[44:52] and it was way over my head. I definitely didn't have the questions to
[44:56] ask because it's so new, yet because of learning about that last week,
[45:02] and one of the speeches that I heard at Denver Startup Week, the way that when you were looking at
[45:09] all the Kubernetes stuff and it had all the commands for it, I'm like, "Oh, that totally makes more sense the way that's
[45:14] structured because it's for Kubernetes compared to, if you're coding and I wouldn't have put two and two together
[45:21] without this way of the overwhelm. Just getting an idea of something
[45:30] before actually going into it, what is something that you think we
[45:37] should know about Go that would interest people? >> Yeah. One of the things
[45:48] that trips people up a lot is what we call pointers. You've done JavaScript before and you know how we're,
[45:55] let's say we do this. Let me see if I can still write JavaScript.
[45:59] I'm going to say function main function do work or something.
[46:22] We'll call main down here. I'm going to create a new object, a JavaScript object.
[46:32] I'll say object equals name Eddie. Then this will take in that object.
[46:43] We'll say do work with object, and we'll print out that object afterwards.
[46:50] You're with me so far? >> Yes.
[46:55] >> In here, I'm going to say object.name equals gen. When I go to run this,
[47:05] you see what happened there? I declared my variable here.
[47:16] I said, this is a constant named object, and you're familiar with constants in JavaScript.
[47:22] I can't reassign that. But I print it out,
[47:27] I pass it to this function, and then I print out the same variable.
[47:31] I didn't give that other function my variable. I said I called it with it,
[47:38] but I didn't intend for it to do something to it. Is that expected behavior for you?
[47:45] >> Okay. >> Let's give another example.
[47:52] Instead of object, we'll say, we'll just call this like num.
[47:56] It's supposed to be the number 3. We'll do the same thing here.
[48:00] We'll print out num. Inside here, I'll say num is equal to 7.
[48:13] Cool. When I run this, what's going to happen? What's going to be the output?
[48:17] >> Well, I would have thought that I would have been the number 3.
[48:22] >> Both times? >> It is the number 3.
[48:35] Why was it different when we did it with an object? >> I don't know.
[48:42] >> You see the problem, right? You see what we ran into?
[48:49] >> Because of, oh, because. >> Oh, like this.
[49:00] >> I'm saying we'll say object.name equals gen. >> Why did it do the same thing?
[49:20] I reassigned the variable I was passed. >> It's saying that you've reassigned everything,
[49:28] but because the first one was the number 3, that's how Go makes it.
[49:32] It's going to make it stick to its guns no matter how many other times you redo things.
[49:38] >> This is where we get into another principle of programming where we say pass by reference or pass by value.
[49:45] Have you heard that term before? JavaScript has a mixture of both.
[49:53] This is pass by value. When I'm given a number 3,
[49:59] number is a primitive, so that is like an actual number,
[50:03] like the type of number is a value. When I pass that to a function,
[50:09] it gets a copy of that value. It doesn't get the original variable I gave it.
[50:15] But with an object, when I take this object and I call it with this,
[50:21] objects in JavaScript are passed by reference. This is actually taking in
[50:26] a reference to the original variable. But when I mutate that reference,
[50:33] I'm actually mutating the original variable. >> Your words make sense,
[50:39] but it's not sinking in yet. >> But that's why I'm like, it's so weird.
[50:45] Like it's not going to click now, but then later on somebody else will say something,
[50:49] I'm like, "Oh my God, I finally understood it." >> Yeah. This is a lot.
[50:57] What I'm getting at is there's two different types of passing a value.
[51:06] There's pass by value, pass by reference. JavaScript has a mix of the two.
[51:10] Objects in JavaScript are always passed by reference. When I call, when I hand it to another function,
[51:16] it gets a reference to the original object. When I pass it a number or a other primitive,
[51:23] if I just had a regular string, that's also a value. If I give that to a function,
[51:28] it gets a copy of that value. Where I'm going with this is when we do things in Go,
[51:35] I can create a variable here. I can be more explicit in how this works.
[51:41] I can say, var name string is Eddie, we'll do the same thing.
[51:52] >> Might be wrong. >> Declared but not used.
[51:56] Side track, Go is very strict on a lot of things. It's very conventional.
[52:01] There's basically one way to do things in Go and it checks. This is actually a check for an unused variable.
[52:08] This actually won't even run. It won't compile, it won't run,
[52:11] because you're not allowed to have unused variables in Go. There's a lot of those little safety features
[52:17] that help you write better code. It's going to be mad until I use that variable.
[52:23] I'm going to say name in here. Well, this is going to work as expected.
[52:29] We run that, we get hello Eddie. With me? >> Yes. I think something
[52:37] that is also making it click more now that you're doing it over here is with JavaScript,
[52:46] it would also, if we got the same type of error, we would have to use a console log or something like that if we
[52:51] haven't completed it out yet just so that way it compiled it too. >> Yeah. It would give you undefined warnings or other things.
[53:00] >> This is starting to click. >> That actually leads me to one of the pain points in Go that I find,
[53:07] is Go has no concept of undefined or null. >> Okay.
[53:13] >> Everything in Go has a default value. If I say var s string,
[53:24] the value of s here is going to be the default value of a string. If I go print this out,
[53:31] it's going to be an empty string. That's the default value for string.
[53:35] Let's say that s was actually an integer. What do you think the default value of an integer is?
[53:42] >> Zero. >> It is zero.
[53:45] >> Okay. >> The pain point I have here is when I'm working with this variable,
[53:55] I can't tell if it was set to zero or if it is the default value of zero.
[54:04] That comes around to bite you in very certain situations, where you're like, I'm not sure if I was passed.
[54:13] I work on CLI tools. If you say, do something,
[54:18] let's say you write a sleep command that'll just sleep for a number you give it.
[54:23] Let's say you give it zero seconds. I have no idea if you passed in zero or if it defaulted to zero.
[54:32] That leads to problems. Let's say that when it's zero, it should sleep forever.
[54:38] Well, if you say sleep zero, you want to sleep zero seconds,
[54:42] like it could wind up sleeping forever. >> Real quick. Homie asked,
[54:49] if I change a reference to a variable, I just change the variable that points to the value.
[54:55] When I change the value, I change the actual value. Is that correct?
[55:00] >> Change the variable that points to the value. Almost. The reference is pointing to the same value.
[55:15] If you change what it points to, you're changing the original pointer.
[55:22] I can actually reassign that object. Let me do this and go.
[55:28] It'll make a little more sense here. Where I'm going is,
[55:31] we have the string. If I do the same thing here,
[55:37] so let's say that I say, name equals gen and I return name.
[55:51] Then we'll just print out regular name in here. I'm going to call greet, pass it name.
[56:04] It's going to set name equal to gen and return name. But this is its own copy here.
[56:10] When I run this, it didn't reassign this variable to gen. It assigned this one, this here,
[56:19] because this is a value that got passed in. If I want this to be a pass-by reference,
[56:25] we use something called a pointer in Go. This is used in C and other languages too.
[56:30] I can say that name is actually giving me a pointer to a string. We declare that with the little percent sign here.
[56:37] I mean, the star sign. That's going to be more complicated.
[56:46] I'll just say string equals Eddie. This is inferred typing in Go.
[56:51] This colon equals, I don't have to declare the type ahead of time,
[56:55] it will just know from the right side that this is a string. This is what we wind up using usually.
[57:02] Now I have string. No, I shouldn't call that string, it's a name.
[57:07] Name equals Eddie. Inside of here, let's say I call greet.
[57:12] I want greet to take it a pointer to a string now. We'll do what we did before, print out name.
[57:24] Greet has to take in a pointer, I've said. The star says there should be a pointer,
[57:30] which is a reference. I can say, hey,
[57:34] pass a reference to this variable, that's where we use the ampersand.
[57:38] This actually gives it the memory address to this variable. Still with me?
[57:48] >> I am. Another thing that just hit me is the fact that I think this is where,
[57:58] especially for newbies, when you start in the coding world, people aren't necessarily explaining what language to start with,
[58:08] because when you start, they're all really complicated.
[58:12] But what you would use a language for and what logically makes sense to them, is where I'm getting. To some people,
[58:27] what you're doing right now is going to make so much more logical sense than what JavaScript does, for example.
[58:34] >> Absolutely. >> Yes. Because it's pointing to the second one,
[58:43] therefore, it's going to basically ignore the first one. >> Right.
[58:47] >> Even though the first one is the declared one. >> Right. Well, this actually is this one.
[58:52] They're the same one because I gave it this address of this one. It took in a pointer to that original variable.
[58:59] This is what we call a dereference. This just says, because this value named by itself,
[59:05] if I print out name in here, it's going to be a memory address,
[59:09] which you probably haven't seen before, have you? >> No.
[59:14] >> This is a hexadecimal memory address. This is how virtual memory is represented on your computer.
[59:21] Think of your RAM sticks. They're just like rows and rows and rows
[59:25] of addresses that can hold values. This is an address to one piece of your RAM stick in your computer.
[59:36] >> I don't know why I find this so fascinating, how confused I can get learning this stuff.
[59:43] But seriously, it's beyond me at the moment, yet at the same time, it slightly makes sense, which is so weird.
[59:52] >> This is complicated. I wouldn't call pointers the beginning of learning Go. Especially while you're learning programming in general.
[60:01] But this is one of the major characteristics of the language. Here I said, this is printed out the name,
[60:09] which is the address, that's what we got there. Then I say, I want you to actually change the value at that address.
[60:16] That's where that little dereference star comes in. That says, change the value of name to be gen.
[60:23] That actually changed this variable because we see it printed out twice. >> Interesting.
[60:29] >> You want me to downshift a little bit, so I'm a little easier?
[60:33] >> Yes, please. >> Okay.
[60:36] >> Homie just asked, the first print of gen was the main brackets due to the pointer.
[60:45] The second print was from the greet brackets, correct? >> Yeah, that's the return.
[60:53] I'm just returning that string. We could ignore that if we,
[60:57] I did it confusing, but yes, you get the idea. What do you want to build?
[61:07] You want to build something very simple? >> I would say most times when people
[61:12] are wanting to come on the show and want to build, it's normally like a web app.
[61:17] Just so that way it gives a reference to something to build and can edit. >> Have you done back-end web apps before or just the front-end part?
[61:29] >> Mostly, that's a good question. >> Have you done Node servers or Python servers?
[61:35] >> No. >> Okay.
[61:37] >> I feel like you need to come back on the show now. Because I'm curious about that stuff,
[61:43] but a lot of people have been doing much more front-end. >> Yeah.
[61:48] >> I like a front-end. I think it's really cool,
[61:51] but I would say even to what we were talking about earlier, if you're talking about actually question,
[62:00] my thought went from a statement to a question midway through. Because things like databases and APIs and
[62:08] that thing are going to be more back-end, not front-end. That's really where my mind goes,
[62:15] especially when, but it's not as easy to learn, is what I'm realizing as where I'm like.
[62:22] Because seeing how something is, I don't think not compiled like the languages,
[62:29] but a database is compiled and puts out to the front-end or an API is linked and put out to the front-end is really cool.
[62:40] But it is really more of I'm curious how stuff works. >> Yeah. I wouldn't say back-end is more complicated, it's just different.
[62:51] >> No, I don't think I've done a lot of back-end to actually say whether or not to compare the two.
[62:57] >> Okay. >> Interesting.
[62:58] >> I don't know whether to super overload you by doing that or we can pivot to something else.
[63:03] >> I would say we can pause. I would say we can pause because I think this is,
[63:08] it definitely is we went through the complexities, which oddly I really enjoy doing even when I don't understand it.
[63:18] Homie said front-end, so I'm guessing that means that majority of the things I've done are front-end.
[63:24] Because Homie has been here for, I want to say at least 25 of the 38 shows that I've done.
[63:34] It's definitely something that now I'm a lot more curious about. I think that I've only done something with MongoDB once, so.
[63:48] >> Can I show you one more thing before we bounce out? >> Yeah.
[63:51] >> I'll turn this back on. I'll just show you what a web server would look like in Go, just real quick.
[64:04] We use the HTTP library, and I'm going to type this out quick.
[64:11] This is what we call an HTTP handler. This is common for any back-end programming,
[64:20] so when you do some Node or JavaScript, this is how we approach building web apps.
[64:25] This is going to say, when a HTTP request, so when your browser makes a request to the root of the domain,
[64:31] so in your browser here, so if we have Google.com.
[64:39] Well, there's actually a magic hidden flash at the end of Google.com there. >> Right. That way, it may go to the index file,
[64:49] it may go to, and I think that is something that luckily,
[64:55] that file structure I learned from hosting at GoDaddy, when I worked in hosting there,
[65:02] but it is something that other than that, I'm like, "Okay, I get file structure, yay."
[65:09] >> Yeah. You understand that. That's the path. That would go to your file on the disk if there was index HTML.
[65:20] I'm just going to send back a message, and then I'm going to start up the web server.
[65:25] You learned what a port is yet? >> Yes.
[65:29] >> I'm going to say port 8080 here. This is like the basic Hello World of a web app in Go.
[65:36] Let me make sure it works. Browser Go. There you go.
[65:43] See, I got the Hello World printed back. >> Interesting.
[65:47] >> I just sent back the string Hello World. I could have done something wild,
[65:50] like we'll just say, HTML, body, H1, Hello World, H1, body.
[66:08] Do you know that look right? >> Enclose that one, right?
[66:17] >> Yeah. Thank you. >> All right. This came back as HTML.
[66:26] We can see in the H1. >> See, that's what I'm wondering.
[66:32] If there's an app that would go into what you just wrote, to be able to be like,
[66:38] this is HTML and this is Go. >> From like a website?
[66:42] >> Not from a website, but just looking at the coding.
[66:45] Because yes, I could tell that it says HTML in it, but when you're doing JavaScript,
[66:51] TypeScript, and HTML, it may not be as obvious.
[66:57] That's why I'm like, I wonder if there's an app somewhere out there that does that.
[67:02] >> That's fine. I have this Chrome extension that I really like. >> To do it more in VS Code or whatever I'm coding in
[67:12] compared to the web app. But I mean, that could be the same type of thing.
[67:19] >> Yes, for sure. Chrome extension is called Wapalyzer. Right here is a good example.
[67:29] This can look at a website or a web app and tell you the technologies that it's using.
[67:34] >> That's cool. >> Here you can tell Airbnb is using React.
[67:38] This is using Ruby on Rails, some other bits in here as Google Analytics on it.
[67:44] >> Interesting. >> Yeah. I like this extension a lot.
[67:47] You can get a few. Most days, things are just like a static HTML site,
[67:52] and so you can't tell what their back-end is, but sometimes it can detect from
[67:55] a header or something that this is Ruby on Rails. >> Got it. All right.
[68:01] >> It's just called Wapalyzer. >> Interesting.
[68:04] >> I don't know where the, there you go. >> Yeah. That's what a web app would look like in Go.
[68:14] You could build your React app and read that file from the disk and serve it here,
[68:21] or build it as a single string if you wanted to here. It's the same deal. This is just a web server
[68:27] serving something to a request. >> Interesting. Then Homi asked
[68:36] another question and did this answer it? That seemed pretty easy.
[68:41] Can you explain why you normally choose node over web server to build this?
[68:48] >> It goes back to the right tool, right job kind of thing.
[68:52] I think that node does something, do you know what a web socket is?
[68:58] Have you learned that one yet? >> I know what it is,
[69:02] but I don't know what it is at the same time. It's really annoying being a part of API stuff,
[69:07] because I'm like, I know what it is, but do I? Homi knows,
[69:12] and that's what matters because he's the one asking the question.
[69:15] >> Yeah. If I ever had to do anything with web sockets, I would probably just use node,
[69:19] because it's like socket IO and like the node JavaScript experience for
[69:23] web sockets is just such a good experience. That's the tool I would use for that job.
[69:29] At the end, Go is probably going to be more performant if you need a really performant web app
[69:34] just because it's a statically compiled language. Go is a concurrent language
[69:41] too which we didn't talk about a lot, so you know about the event loop in JavaScript.
[69:45] JavaScript is single-threaded. Right now, there's worker threads that you can do,
[69:51] but JavaScript is single-threaded, only one thing runs at a time.
[69:54] >> Right. >> With Go, we have a concurrency built into the language.
[70:01] If I want to do something concurrently to another thing, I can start two functions
[70:06] and they'll both run at the same time. That's actually Go's strong suit.
[70:11] Is anything to do with concurrency or distributed language types, distributed networking and server type stuff,
[70:17] that's where Go really shines. >> Okay, I'm going to have to doodle on what I'm thinking of.
[70:35] It's very confusing in the fact of when I'm learning this stuff and I'm like, wait,
[70:40] this question did make sense and then I'm thinking about it and it doesn't make sense.
[70:44] [LAUGHTER] I am enjoying the learning of all of this,
[70:51] and thank you for at least explaining a bit about more about why people talk about Go.
[70:57] I may not fully understand all of the things you were doing, but it's enough to be like, okay,
[71:04] now I understand why these are built with Go instead of with JavaScript or Python.
[71:12] I would say when I was asking people what languages I should learn, my first language, almost everyone was like JavaScript or Python.
[71:21] Those were the main two. Learning what Go does,
[71:26] or at some point it would be cool if I could learn what if they're even used,
[71:32] but C# or C++ or C even, or Java, what are those differences?
[71:37] Those are all things that why do we still use them, but nobody starts with them.
[71:45] >> Yeah. You saw a lot of it today. You don't want to have to worry about pass-by reference,
[71:52] pass-by value, pointers, types, all these other things. I agree completely.
[71:57] When people are learning Java to program, I tell them Python or JavaScript as well.
[72:00] >> Yeah. This at least is answering why and this is like something, I think, and you and I talked about this when we first met.
[72:08] I've talked about this before. I think I would really struggle going through a course because I don't always understand.
[72:16] I'm like, I need to know the why of why don't we do this? What does it do enough?
[72:21] That way I can go, okay, let me refocus on what I'm supposed to be learning.
[72:26] Because it's really hard for me not to just go down the deep end of wanting to go, okay, I'm suddenly going to go learn Go because it's
[72:35] cool and I don't know it. Why does everyone say no? >> Yeah.
[72:40] >> Thank you for at least solving that curiosity. Homie said, exactly.
[72:46] I feel like I have a better general understanding of where Go, Node.js fit into the tech eco.
[72:54] >> Yeah, of course. >> That's a great way of saying it is that's what I'm working on learning,
[73:00] homie, is like the tech ecosystem because I don't think that's explained really well anywhere.
[73:08] At least that I've seen. >> Yeah. Again, I work with a lot of students and beginners.
[73:14] Learning different languages is cool, but you definitely should get a foundation for basics of programming,
[73:20] which you have, you're learning and you're working on. Every language has an if statement,
[73:25] every language has some for loop or while loop. >> Actually, that's what we're working on in Python right now.
[73:33] It's been really cool to have Laura on this show because it's giving me some structure.
[73:39] We were going every other Monday, we're now going to do it every Monday.
[73:43] As we're going through the automate the boring stuff book, and it's cool because I don't think I could ever sit
[73:54] through a class or a course if it was just this. I would be like, I'm out,
[73:59] I'm done because I tried going to school for this. Yet now that it's like,
[74:04] I have this one dedicated day and I can learn about everything else. It really happily comes together.
[74:11] I don't know how else to explain it. I'm like, I can do the complex stuff and learn the basics at the same time.
[74:17] >> I don't know. >> Yeah. We had a summer intern and he spent a good chunk of it learning,
[74:24] and reading, automate the boring stuff, and yeah, I've heard great things.
[74:27] >> It is so cool. His books are also very funny. When I watch his live stream,
[74:34] I always just want to ask him to show the kittens that he is fostering at the moment. >> That's awesome.
[74:42] >> But yeah, Eddie, I think this is good for today. I definitely learned a lot.
[74:48] I know we have quite a few viewers, so if anybody has any questions before I see if I can
[74:55] raid you into DistributeAid's OSS stream. I have fun now that I've learned how to raid.
[75:05] I've done it twice before, I think, twice ever. >> Yeah. I'm definitely happy to come back.
[75:12] What I actually had planned, I didn't know where along you were in your journey so far,
[75:16] but what I had planned today was to build a URL shortener, like Bitly or something.
[75:20] >> That would have been cool. >> Yeah. I think that would be way too much right now.
[75:26] But when you're ready for it, I can come back and that's what we can do.
[75:30] >> Sweet. Are you aware of Quick.js and that framework? >> No.
[75:37] >> Well, Mishko, who built Angular and Angular.js has come out with Quick. He was on the show,
[75:47] I want to say one of my first five people on the show. He was like, "Let's do Hacker News."
[75:55] The person that I like to call my Internet big brother, Anthony, was like, "Dude, don't do that.
[76:03] You don't even know that Hacker News existed." It has been a lot of fun to learn all of this.
[76:13] >> Yeah. >> It definitely has been.
[76:15] >> That's what I tell beginners too is as you're learning, forget the basics first,
[76:20] and then as you're learning new things, pick a project that you're going to do in every language or framework.
[76:26] My project for learning a new language is I build a URL shortener. I use a little database called SQLite,
[76:34] and it touches everything. It has to write to the disk,
[76:38] it uses a database, it serves a web app.
[76:41] For front-end frameworks, when I was doing more front-end, I would build my own version of Giphy using Giphy's API.
[76:48] Which was really easy to do actually. You can use their search or the random API.
[76:53] That was my hello world for JavaScript frameworks. >> I will say that there is an app I really want to build,
[77:01] but I don't know what goes into it to even start. I don't even know if apps are anything,
[77:06] I just wanted to do something. Every Wednesday, I host a Twitter space
[77:11] that people can DM me and tell me that they want to be tagged every week. Basically, I just want something that I can paste the Twitter space into,
[77:23] and it takes all of the people and tags them and just creates it, instead of me having to copy and paste it.
[77:31] But I'm like, I get that I would probably want to use the Twitter API, and my guess is some type of database to be able to
[77:38] keep track of all of the people that have submitted. But I'm like, I don't even know where I would start,
[77:45] because I don't know what goes into doing something like that or even what to Google. >> Yeah. Well, when you're ready for that,
[77:52] we can absolutely do that. >> Because that is something that would be extremely helpful in my world.
[77:59] Because right now, I just have them in an Excel file and copy and paste it. It's a really fun thing.
[78:05] But cool. Well, thank you so much for being on the show today, Eddie, and we're going to see if I can actually do this raid.
[78:14] No, I didn't do it right. Let's see. I'm going to get here. I'm going to get it.
[78:31] Why is it saying invalid? Why? Why, Twitch?
[78:40] Why? I know I'm awkwardly causing people to stay here while I'm trying to do this. One of these days, I'm just going to know how to raid.
[78:58] This was, as I was telling you earlier, I was going to do all this random stuff
[79:06] earlier and it was going to be stuff like this, like learn how to set up my Twitch.
[79:13] Oh, there we go. Let's see. If it's working, you-all are about to be raided in 10 seconds.
[79:23] Two viewers, four viewers are ready to raid. Three, two, one. Okay, bye.
[79:32] I think they raided. At least I'm guessing they did. If they did, they did. Awesome.

