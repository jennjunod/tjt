---
showLink: "https://www.youtube.com/watch?v=almMsIY-wvs"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-android-app-development-with-guest-zachary-powell-pt-2"
title: "Teach Jenn Android App Development with Guest Zachary Powell pt 2"
publishDate: "2022-10-21"
coverImage: "https://i.ytimg.com/vi/almMsIY-wvs/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:07] We are doing more Android stuff today. I am very excited for this,
[00:11] probably a little too excited. But Zachary, please introduce
[00:17] yourself and what we're going to be talking about today. >> Sure. Hello, everyone. I'm Zachary.
[00:23] I am basically now within DevRel, but I was an Android developer for 10 years exclusively.
[00:31] I still do Android development in my free time, and it's just something that's never going to get away from me.
[00:37] We're here today to have another look at an Android application,
[00:42] how we can actually build an app, and all that fun stuff.
[00:45] >> It's going to be great. As of right now,
[00:52] so that way you-all get caught up, I have a few things I need to post in.
[00:59] Hello, Ryan, that I need to post in the chat. Because we have last week's stream,
[01:11] then we have using tablet screen share, and also how to put debugging mode,
[01:31] which is pretty funny that it's from Verizon. >> Yeah, that was quite funny.
[01:36] It's a pretty generic steps like for any Android device. It's just that was the first one that came up and it was clear,
[01:44] so good job Verizon, I guess. >> I like it. That way everyone knows there are all of the fancy links,
[01:57] and working through the install at the moment, which happens to be taking forever.
[02:06] >> What we can do is we can start by looking at the code if you'd prefer, and then once that is all done and happy,
[02:15] then we can run. Just like that, it's finished. >> Yes, we have another one.
[02:22] >> Yeah, not that one. That was if you're using Mac ports.
[02:26] >> Oh, very cool. Very good. >> You should be able to just run screen copy and it should work.
[02:34] >> Let's find out. >> Assuming your tablet's plugged in.
[02:39] >> It is plugged in and it's getting the charge. >> Excellent. Of course.
[02:46] On the tablet, there should be a little pop-up that's come up. You might need to unlock it.
[02:52] It should say something along the lines of, "Do you want to allow this device to do things?"
[02:57] >> Oh, hey. >> There we go.
[03:00] >> Very exciting. Yes, I put my calendar as my home screen. >> You can actually also control it with your mouse.
[03:06] It works both ways. You can use your mouse to move about,
[03:10] click on things, and all that stuff. >> This is quite entertaining.
[03:14] >> I find this incredibly useful when I'm presenting. If I'm at a conference or something,
[03:19] it's just a lot nicer to be able to physically present something. I work with communication APIs,
[03:25] so being able to actually send a text message and show it come up on the screen and that sort of stuff.
[03:30] It's a really great tool. >> Yes, this is so fun.
[03:34] >> Like all good tools, it's also open source. >> Yes. It took us, what, 20 minutes to install on everything?
[03:43] We did get started, but these are the steps that we went through.
[03:47] That was just shared in the chat. Let me know, everyone, if you need us to re-share it.
[03:55] I will change all of my tabs. If I remember correctly, this was one that didn't want to zoom in.
[04:02] We are using Android Studio to be able to build our app. >> Yes, indeed. I think last time we did create
[04:13] this login activity project which we can open, and we can use that as our basis to have a look through.
[04:21] I think there's quite a lot that gets generated for you when you create a new project.
[04:27] I think it'll be interesting to go through and explain the different areas what built makes up an app,
[04:33] because there's quite a lot that makes up an app. >> Really funny, I just saw that I got a notification and I'm like,
[04:41] "Didn't I turn on do not disturb on this thing? How do I?" Y'all, this is what I find pretty funny is,
[04:49] as you guys can look at this with me, I don't care. How do I do all of this?
[04:58] Because I am an iPhone Mac user through and through. I have been for years.
[05:03] Catch the other stream if you want to hear why, and me trying to learn how to do this.
[05:10] But I'm like, "Didn't I put it on do not disturb?" Notifications. You are on do not disturb.
[05:18] Turn on. Yes, you are the Android gang. I dig it. I'm getting there.
[05:30] Just to make sure, this is the Android Studio that we were using, that we downloaded. I just want to make sure I relink it.
[05:39] So that way, everybody sees what we are using. Going back, so many tabs.
[05:53] >> Well, hey, I clicked it. That works. >> There you go.
[05:56] >> It just magically happened for us. >> Brilliant. So we'll just let it.
[06:04] There we go. Just get rid of that tip. Yeah, you can click that. That's fine.
[06:11] Yeah. So this is the whole hierarchy, the whole tree of files
[06:17] that's just been completely generated for you. What we can do, let's try and make it a little bit
[06:22] more streamer-friendly. So if you click on the Android Studio tab on the top menu,
[06:28] and then go to Preferences, there is a appearance and there is a, where is it?
[06:39] Yeah, use custom font. So if you tick that,
[06:49] and then you can increase the font size a little bit. That'll make it slightly more probably streamer-friendly.
[07:01] >> You will make a giant. >> This is probably actually my biggest annoyance.
[07:06] That might be a little bit. >> Maybe a little too big, maybe a little too big.
[07:11] >> This is actually, yeah, this is one of the big annoyances of, if I ever do any live coding on stage,
[07:17] trying to get this set up properly. I don't know, it's always an absolute nightmare to do,
[07:23] but we'll get that. Then yeah, it should be able to move it about a little bit,
[07:29] and then just drag that so it takes up a bit more of the screen. >> Yeah. Okay. We have been set up.
[07:35] I think it's because on VS Code, it is expanding with the command plus and minus,
[07:46] and on this app, it expands all of the folders and set. What up, Jeremy? Thank you for joining today.
[07:56] Jeremy is a fellow streamer we met on a Twitter space, because that's how I meet way too many people, I think.
[08:04] >> Yeah, without a doubt. >> All right. So we chose,
[08:10] I believe we decided to make this a tablet one. >> When we chose our options.
[08:17] >> Yes. So basically, this is what you're presented with any app that you make.
[08:24] You're going to have these A2 top-level sections. You've got the app, and then you've got
[08:29] the thing called the Gradle scripts. So we can have a quick look at the Gradle scripts,
[08:34] if you click on that and expand that side of it. What these files, these are just literally the build process,
[08:43] the scripts that control actually taking all your app code and making it into the file that people can install.
[08:51] >> Okay. >> So if you have a look at that,
[08:53] you've got two build.gradle files, and if we have a look at the top one,
[08:57] this defines basically the plugins that we're using, the top-level areas of code that we're using,
[09:10] which is a lot like in, say, Node.js or something,
[09:14] you'll have quite a high level, or if you're using React,
[09:17] you'll have the React component and then you'll have other third-party libraries and stuff.
[09:23] So here you can see we literally have a Android application plugin,
[09:29] an Android library, and the Kotlin library. So the real, just the absolute core bones
[09:38] of a system that we would need. Then in our other build.gradle file
[09:45] is then all the configuration about our app. So things like you've got the package name there,
[09:53] the namespace, so com.example.loginactivity for TJT, which we set up last time
[10:01] when you were creating the application, and other config informations like SDK numbers.
[10:07] So Android, one of the big issues with Android is there's lots of versions of Android,
[10:12] and these are broken down into SDK versions as developers. For end-users, they'd know it as like Ice Cream Sandwich,
[10:20] and Jelly Bean, and whatever. But for us, it's numbers.
[10:26] So we're saying we're going to target the SDK 32, which is the newest stable version,
[10:34] and we're going to require that the device we install it on has at least SDK 22, which I think translates to,
[10:42] I want to say Ice Cream Sandwich, but I might be wrong. - And as a pause really quick there, y'all,
[10:48] for those joining in on my journey of building my Twitter tagging thing,
[10:55] is what I'm calling it, Twitter tagging thing, is after I get it working with React,
[11:03] Zachary and I were actually talking offline about how I could replace React with the Android app
[11:11] to be able to make it an Android app later on. So I have found the app that I want to make
[11:17] as super complicated as possible, and make it in different ways.
[11:23] So I will be doing that later on. I just wanted to, you talking about the SDK
[11:30] reminded me that I'm like, oh yeah, I want to do this later on too.
[11:34] - So yeah, this is literally where we are going to set kind of all these kind of configurations things.
[11:43] And then we have the dependencies, which this section is basically the libraries
[11:50] that we're installing in our application. So these are all the things that we just kind of get
[11:55] for free that come as this config, but perhaps you're going to use some custom libraries,
[12:00] someone's created something, or maybe there's an SDK or something
[12:04] that you want to install. For example, at Vonage, we have an Android SDK,
[12:08] which you could use to then make phone calls and that sort of stuff.
[12:11] So this is where you would define that and say, I want to use this SDK.
[12:15] And so that all then gets pulled in during the process of actually building your app.
[12:19] - Okay. - And then the other files there,
[12:23] that again, they're just more config. There's a lot of kind of very technical things
[12:28] that a normal developer probably will never have to touch, certainly in like a personal project kind of thing.
[12:35] So, I mean, but definitely have a look at them if you fancy it, but you know.
[12:41] - I feel like that's like when I'm installing some type of JavaScript and it comes with the node folder
[12:48] and people are like, don't even worry about like looking at, just forget it's there.
[12:53] It's important, but don't touch it. - Oh, well, yeah, yeah, yeah.
[12:57] Only change things if you know what you're doing, I think is probably the thing.
[13:01] - That is the great way of saying it. - That's the Gradle section.
[13:06] And so Gradle is the framework that builds the app. There are a few different frameworks,
[13:12] but this is the one that Google said, no, use this one. This is the de facto way of doing it now.
[13:20] So that's that side of it. And now we can actually kind of look at the app side
[13:25] and probably the much more interesting side of code. So your code is essentially broken into three sections.
[13:32] You've got your manifest. And this is basically how you tell the Android,
[13:38] the operating system, how to use your app, what is available in your app, what can you do?
[13:45] And this is what the manifest is. It's like a table of contents.
[13:48] It's like, you know, that sort of, these are the things that are available.
[13:52] And what you'll see here is you've got, you define your activities, which we'll get into,
[13:58] but like see that as kind of a definable section of your app. So you might have an activity for the homepage,
[14:06] an activity for your login page, an activity for the registration process,
[14:13] those sorts of things. So you define these here to say,
[14:16] these are the things that are available in my app. And then also you're defining here
[14:22] some more details about the app itself. So you can see that you've got on line nine, Android icon,
[14:29] and that's the icon for your application. That's the, when you actually install your app,
[14:37] the icon that shows up on the screen. Your, I've got like other bits and pieces there as well,
[14:46] the label for your app. So what comes up underneath the icon.
[14:51] And yeah, I mean, there's a lot of config here. You also, if you scroll up to the top of this file,
[14:59] I just don't know if it's not, it hasn't got any in here, but this is where you'd also set like permissions.
[15:04] So, 'cause you're not really someone that's used Android so much,
[15:08] I'm not sure how much you know about permissions, but when you, I think it's on iOS as well.
[15:15] So for example, if an app wants to be able to use your camera,
[15:18] it has to ask you for permission to do that. - Okay.
[15:22] - I think there's normally like a pop-up. - Oh yeah, yeah, yeah.
[15:24] - Do you allow this app, yeah? So this is where you define the things
[15:29] that you want to be able to ask. So you might say, well, I know my app
[15:34] is gonna want to be able to use the camera, or maybe it wants to be able to use the microphone or GPS.
[15:40] And again, you'd add them here so that the operating system, Android knows,
[15:45] these are the things your app might want to use, and then can show the user that sort of pop-up.
[15:52] - Okay, that makes sense. And like, I noticed that when I clicked into here,
[16:00] was it this one or did I end up like, oh, it went to that one, okay.
[16:05] - Yeah, so what it's trying to do here is be a little clever, which as always, as we know,
[16:10] most of the time when computers try to be clever, they're not.
[16:13] And essentially what you see is the app string forward slash names, the app name.
[16:20] So that's actually a reference, like a variable reference to another file somewhere
[16:26] where the actual string is being kept. So when you hadn't clicked off it and it was gray,
[16:32] it was giving you the value of that string as like a preview. - Yeah.
[16:37] - And then you clicked on it and it shows you the actual, that it's confusing and annoying,
[16:44] but we will see where that file is shortly. - I'm like, now I'm trying to make it go back to it,
[16:49] by like clicking everywhere else. - I don't think you, again, this is the other thing,
[16:54] I don't think you actually can. I think you have to close the file and then reopen it again.
[16:58] - Oh, weird, okay, well. - Again, computer is trying to be smart,
[17:02] but it doesn't matter, we'll look out for that later and you'll be able to see it.
[17:06] So you've then got these two other folders, you've got Java and this is where
[17:11] your actual app source code is. - Okay.
[17:14] - So as we sort of talked about last time, Android apps used to be Java,
[17:19] they're now written in Kotlin, and this is kind of one of those oddities
[17:23] that's been left over, even though the code is Kotlin, it still goes into a Java folder,
[17:31] or has to go into a folder called Java. - Okay, and y'all, I will repost this again.
[17:39] What up, Huck? It's some things that we went through already of,
[17:49] Android Studio, of the first video that we went to, as well as the screen share, which my tablet is plugged in,
[18:02] the debugging, and then the studio that we're using to get y'all caught up,
[18:09] it will be in the YouTube videos as well. Oh, well, thank you, Ryan.
[18:13] Ryan's got my back, thank you, thank you, I appreciate it. And yes, please pause us and let us know
[18:20] if you have questions. Let us know if we have questions too,
[18:24] I mean, I will probably have questions and may not know how to say them,
[18:28] so please let me know if I have questions as well. And if you're wondering about the going from JavaScript
[18:37] to Kotlin, we did talk about that in last week's stream too. - Cool.
[18:48] So yeah, so in here is where all your source code is, and this is where things get a little bit kind of interesting
[18:58] shall we say, that until very recently, the Android community could never agree
[19:07] on how they should structure their apps, like how you should actually kind of have the directories
[19:15] and what you should call the files and how your app should be kind of structured
[19:19] in a meaningful way, and no one could agree. There was lots of different kind of ways
[19:25] that you could do this, with lots of different people that said
[19:28] they were the best way to do it until very recently, because until very recently, Google said,
[19:33] "No, we've finally decided this is the way you're gonna do it."
[19:38] So what you'll find, I kind of wanna touch on this because what you'll find is if you look
[19:44] at other Android apps, if you look at open source projects, they won't always look in the same structure.
[19:52] They'll sometimes have different naming conventions, there'll be different things going on,
[19:56] and that can be a bit of a stumbling block. So you're not losing your mind
[20:00] or thinking that I could have sworn this was done differently, 'cause it was,
[20:04] and there is lots of different ways. So every app will have their code in the Java directory,
[20:11] and inside that will be the name of the package. So we've got com.example, blah, blah, blah, blah,
[20:17] and that'll be different for each app. But then once you're in that, it can be, it's a free-for-all.
[20:22] The developer can decide how they want it to be. - That being said, I feel like, hey, homie,
[20:30] I feel like a lot of people use VS Code just as their regular go-to,
[20:36] like VS Code is a go-to thing. Is Android Studio the same way,
[20:43] which if it is, may give things more structure, or is there other go-tos?
[20:51] - Yeah, so I mean, it's basically the accepted. It's definitely Google's recommended IDE.
[20:58] You should use Android Studio, and I think generally it's the accepted way of doing things.
[21:03] So there is that kind of bonus that if you're gonna be an Android developer,
[21:09] you're gonna use Android Studio, and therefore there is some level of continuity
[21:16] compared to other like JavaScript or other sort of languages and frameworks
[21:20] that don't have a set IDE. So that is useful, definitely,
[21:27] but that's kind of where the usefulness ends. - Okay, okay, fair enough, fair enough.
[21:35] - But that's fine. So in this, in our package directory,
[21:40] in the com.example, blah, blah, blah, we have two subdirectories.
[21:45] We have data and we have UI login. So this app has taken quite actually
[21:52] to the point where I'm considering we start a new app because this is actually quite,
[21:56] they've broken it down in a very detailed way, which is good, but probably not good
[22:04] for your first look at an Android app 'cause there's a lot of files there
[22:08] and it's probably way more than you need to look at. So what we're gonna do is we're gonna close this
[22:14] and we are gonna start a new application. So if you just basically close out Android Studio
[22:20] and it should take you back to the pop-up. So we can go new project.
[22:27] And if we go to basic, use the basic activity template, so the one on the top right, yeah,
[22:36] that should give us a bit of a simpler example. - I'm making this name way too complicated,
[22:50] but I really, really wanted to name it that way. And then remind me,
[22:56] we don't always want to use legacy support libraries? - Yeah, we don't need to.
[23:01] We're not specifically interested in old stuff. So we'll do that.
[23:06] It'll now resort itself out and if we close the main activity, but when the panel on the left is loaded,
[23:16] you'll see that this is much simpler and will definitely be a better starting point.
[23:23] So this actually, this does come back to my point of different apps do things in such different ways.
[23:28] The app that we had previously was definitely looking at more of a in-depth granular way of building out an app,
[23:38] which is very good when you're building something for production and you're gonna have different people
[23:44] working on it. We're gonna be very user-friendly for a developer,
[23:50] but when we wanna just learn about apps, it's not so good. And so it's loaded and as you can see,
[24:00] there's only three files. - I'll show again, yay.
[24:04] And I found out that I can at least go make this part bigger. That's exciting.
[24:09] And yes, three files, that is exciting. Much, much, much, much easier to go over.
[24:16] So like I mentioned, Android has this concept of activities and activities are the easiest way to think about it
[24:28] is it's yeah, it's a self-contained piece of functionality. It's a self-contained thing that your app can do.
[24:38] And you would traditionally start with a main activity, i.e. the entry point into your app.
[24:45] What does the user see when they load your app? And this is what this file is, that is the main activity.
[24:56] And we are now looking at some Kotlin code. So Kotlin is an object-orientated language,
[25:04] which means we have this concept of classes. Again, I'm not sure how much you do and don't know.
[25:11] So if I'm reinventing the wheel, just yell at me, it's fine. But basically we wrap everything in classes.
[25:20] And this means that like, you can then create an instance of that class
[25:25] and do things with it. You can also, it also has this idea of inheritance.
[25:30] So a class can be the child of another class. (laughs)
[25:41] - I clicked something. - Yup, you did.
[25:43] It's okay. - Okay.
[25:45] - It's always interesting to see how people like interact with things.
[25:48] - I click things way too often or hit enter way too fast. - No, you've literally hit onto what I was talking about.
[25:58] So this idea of inheritance. So we have this main activity class
[26:03] and our main activity class inherits. So if you go back to the main activity tab
[26:10] on the, there, yep. If you scroll up to the top of the file,
[26:13] you have, it says main activity colon app compact activity. So we're inheriting the app compact activity class
[26:23] which inherits other classes. And basically the top class is this activity class
[26:29] that you just opened. So this other tab that we have open,
[26:33] and this is like the core of Android. This is one of the core components of an app.
[26:42] So you've got the same kind of, you've kind of gone to the very bottom of this.
[26:52] And the point is your activity has access to everything that it inherits.
[26:58] So you don't have to write out all of the like basic boilerplate getting started code.
[27:07] That's all given to you by inheriting another class. - Real quick, we have a question from Han,
[27:15] and thank you Han. Kotlin is single class inheritance like Java, right?
[27:21] - Correct. - Which would mean because Kotlin would export to Java
[27:26] and is part of, well, it's different, but kind of like-- - It's compatible.
[27:32] - Yes, okay. - It's probably the easiest way to say it.
[27:34] Like you, yeah, Kotlin is under the hood, underneath it all, it's basically just Java.
[27:41] So you can't do anything completely crazy that you could otherwise do in Java.
[27:45] So yes, single inheritance, which means it can only have one class
[27:49] that it's inheriting from. - Got it, okay.
[27:52] - So you have a parent class, but you can only ever have one.
[27:56] Unfortunately, they are all single parents. But you get this stack.
[28:04] And if you actually like go through the whole stack of what you're inheriting,
[28:11] you'll have lots and lots of classes stacked on top of each other.
[28:13] So when you click on that. - Yeah, this one does make me question
[28:19] because sources for Android API 32 platform not found. Does that mean, where would this activity.class file
[28:27] be hanging out? - So any file that's a .class file
[28:34] is actually compiled Java code. - Oh, okay.
[28:38] - What happened here is when you clicked on that, it couldn't find the source code
[28:43] because we haven't got it downloaded. So instead it decompiled that code
[28:48] and it gave you this file. It generated this file for you on the fly,
[28:55] which is kind of cool because it means you can access these things,
[28:57] but it's not actually anywhere, essentially. That file doesn't actually exist.
[29:02] It's just made it for you. - And yes, Ryan, I feel like I click something
[29:07] or I hit enter. It's like things I say way too often,
[29:12] meaning that I didn't meet. But I clicked one of these buttons.
[29:17] I'm not gonna click it now. But this is what I clicked, but like one of these.
[29:21] - Yeah, so what you clicked on is you, these are your functions.
[29:26] So we're saying we've got override. So on line 19, for example, override func onCreate.
[29:32] So by using the keyword override, we're saying we want to override a method
[29:40] that we've inherited from a parent. So somewhere in our stack of inheritance,
[29:48] that function onCreate has been defined. And when you clicked on that thing,
[29:54] it's taking you to where that's been defined. So in theory, you could look at it and go,
[29:59] well, actually, do I need to override it or is it already doing the thing I want it to do?
[30:04] - Now I want to click something else. Oh.
[30:08] - So, okay, yeah. So you've got all sorts of like things
[30:11] the IDE is trying to help you, to take you to different areas
[30:14] that you're implicitly-- - That's really helpful. And-- - Yeah, it is good.
[30:18] - We got another question from Han of what is, I feel like I'm gonna say it wrong, late in it?
[30:26] Late in it? - Yeah, that's late in it. So on line 16 and line 17, we have these.
[30:33] And these are two variables that we're defining. So we're defining a variable called appBarConfig,
[30:42] configuration, sorry, which is of the type appBarConfiguration.
[30:47] So that's the other thing about Kotlin is you can define types to your variables.
[30:54] And the reason why we use late in it is that's to say we haven't yet initialized that variable.
[31:01] So at the moment, that variable is null, but we will initialize it.
[31:07] So it's telling the system that at some point, it shouldn't be null.
[31:14] At some point, it should have a value. And if it never has a value, something's gone wrong.
[31:19] So that's one of these like helper things that Kotlin does that Java doesn't do.
[31:25] In Java, stuff is either null or has a value. And in most languages, that's the case.
[31:33] Like if you defined a variable, it's either gonna have a value or it's not.
[31:38] But this gives you a third option of it will at some point have a value.
[31:45] - Ryan asked like def some par pass like Python in Python? - I think so.
[31:57] My Python is very rusty and I think it's been about 15 years
[32:03] since I worked on anything in Python. - Ryan, join on Monday with Laura and let's ask her
[32:09] 'cause Monday is our Python day. So let's ask her to see if she maybe knows
[32:17] and we'll get her to watch this clip. - So there's no late equivalent in Java.
[32:27] No, there isn't. You have to either define a variable or it's not.
[32:33] You can't say it's going to be defined at some point. And I have no doubt there's some very weird witchcraft
[32:41] going on in the background to make this a possibility in Kotlin.
[32:45] But that's kind of what Kotlin is. It's just a lot of witchcraft on top of Java.
[32:49] So yeah, so we've got two variables that we're defining and then we've got this method on create
[32:57] which is a method that was being defined somewhere else. And when we clicked on it,
[33:02] it showed us it's being defined in activity. But we can actually override this
[33:08] and do something ourselves. And why might we want to do that?
[33:13] Well, an activity has this idea of states. So again, I'm not sure if states
[33:22] is something that you've looked at, but basically the system will tell this program
[33:28] that something has happened and that will change its state. So we have on create, which literally means
[33:36] when the application is created, we'll tell you. And when that application is created,
[33:43] so when, sorry, when the user has launched the application and this activity has been created.
[33:49] So the user is now coming into the activity and the system will say, look, this has happened.
[33:58] You can do something. And that would trigger the code
[34:02] that you write in this method. - Okay.
[34:05] - If you scroll down, there'll be others as well that we're overriding.
[34:09] So we do quite a lot of stuff in here and we'll go through this stuff,
[34:12] but there's other ones as well. So on create option menu.
[34:16] So when the menu is being shown, we can do something here. - Got it.
[34:22] - On options item selected. So when a user clicks on a button in the menu,
[34:27] this method gets triggered and we can then actually find out what item they clicked on and do something with that.
[34:36] So we have this whole kind of like engine of all these different things that can happen
[34:43] and we can capture those things and then do something with them.
[34:47] - Got it. - And that's basically the state engine.
[34:50] - Okay. - And there's a lot of them.
[34:52] There's like 30, 40 different things. - I like that it does create these by default
[35:01] just by us opening the program, opening the app, because I feel like this would be something
[35:07] that even as I'm building an app for myself, which is not an Android app, just a web app,
[35:15] there's enough things as a newbie to get confused on that it's very nice that they build this all for you.
[35:24] So that way you at least have the more tricky stuff taken care of that you can like focus on
[35:30] what you actually wanna build. - Exactly, exactly.
[35:33] So you know that basically, the onCreate is quite a key method
[35:38] because it's where you're gonna do any of your initialization, any of your setup
[35:42] in that kind of instant as the user is coming into your activity.
[35:48] So, and then if you, yeah, if you drill in, you can see that this is the onCreate method
[35:57] for the fragment activity. And then if you do it again,
[36:00] it will take you to the other app and there's a whole. I won't go down that rabbit hole.
[36:05] I just wanted to click it once and I'm gonna, oh, does this take us back to the other one?
[36:11] Oh, it does. Okay, that was cool.
[36:13] - So you can, and you can, this is one of the things that I think really makes it easy to learn using this IDE
[36:21] because you can actually spend time just poking about and getting to understand, oh yeah, okay.
[36:27] So that's linked to that, which is linked to that, which is, whereas in the past, you didn't have that
[36:32] and it was kind of like, you just had to read the docs and take for granted that you had access to these things.
[36:38] - And this is also something that I just observing is these ones are locked,
[36:43] which means I'm guessing I can't make changes and save it because these are like the hidden files
[36:50] that go into making this. So very cool.
[36:53] - Yeah, so these are the bits that are actually given to you by the operating system.
[36:58] So they're not really actually part of your app. They're just part of the framework that makes Android.
[37:05] - Very cool, very cool. - So yeah, so one of the first things we ever do
[37:11] when we're building an app is we're gonna do some initialization in our onCreate method.
[37:16] - Okay. - And there's a couple of different, again, there's a million ways
[37:19] that we could do this, but here what we're doing is we are setting, so in our onCreate method,
[37:26] we're giving the binding variable on line 22. We're giving that a value using this thing called
[37:35] activityMainBinding.inflate and then layoutInflater. So if we click on the layoutInflater variable,
[37:45] so the bit that's in the brackets, so you've got inflate and then layoutInflater on line 22.
[37:55] - Oh, yes, yes, yes. - Yep, and that should highlight--
[38:00] - Highlight. - Okay. - There we go, oh, let me move.
[38:05] And Ryan, just as a quick thing as I'm trying to get this, if you see these little doodads,
[38:13] it almost looks like a inject CD or inject CD. That is what I'm seeing as this.
[38:21] If you click this, he asked if those are just visible, how do you know to connect with them?
[38:27] If I'm paraphrasing this right, these are auto-connected. These are not something we would ever technically
[38:34] have to look at by using this IDE. Go to the top.
[38:38] Because they are part of the Android operating system. It's just to show you of like this little doodad
[38:48] linked into the fragmentActivity.java and then if I wanna go back, I can put the CD back in.
[38:55] Is how I'm viewing these. And we're back to where we were.
[39:00] - Yeah, so that's it. - And hopefully makes sense. But I need to make room for my layout inflater
[39:08] to show the description. Fetching documentation, yay.
[39:12] - I think, I don't know if you can hear my dog barking, but-- - Yes, yes. - Yep, yep.
[39:19] - But that's okay, that is-- - I'm just gonna close the door, he's fine.
[39:23] - I mean, he can always make an appearance if you want him to come on the show.
[39:26] - Okay, yeah, yeah, yeah, give me a second, I'll-- - Yes. - He's only small.
[39:31] - I love seeing everybody's pets. - I'll just mute myself so you don't hear.
[39:37] Where are we? - Yes, very excited for this.
[39:42] And for everyone out of the topic, let's see. Is there some functionality locked
[39:51] behind Jailbreak Android? Oh, Han, I will re-ask that when he gets back.
[39:59] I don't know. We will ask when he gets back.
[40:07] And thank you all for asking such good questions because this is a lot of the learning processes.
[40:14] I don't always know what questions to ask either. So, doggo, no doggo.
[40:21] - No dog, it was my wife coming home. So, unfortunately, she gets dog privileges.
[40:26] - Fair enough, fair enough. And Han asked a really good question again.
[40:32] Is there some functionality locked behind Jailbreak Android?
[40:37] Want something to cheat engine for Android? - So, this week, we kind of touched on this last week
[40:45] with routing Android. So, there are, yeah, essentially,
[40:50] there are certain things you can and can't do. And if you wanna do the things that you can't normally do,
[40:56] you have to route your phone to get access to them. So, yes, is the short answer.
[41:01] There is some functionality. - And also, last week, we talked about
[41:05] how jailbreaking normally, for some reason, refers to iPhone and routing refers to Android.
[41:12] - Yeah. - But they're doing the same thing.
[41:15] - Exactly. - So, it's very, I find that very interesting.
[41:19] - You can't possibly have standards in the United States. - No, no.
[41:23] With anything, iPhone or Apple? No, no, of course not.
[41:29] It has to be different than everybody else, including chargers.
[41:33] - Yes, very true. - But, okay, so if I go to layout.
[41:47] Yay. - So, this is a good example of
[41:53] how you can kind of access the documentation within your app while you're building stuff.
[41:59] So, this is what I wanted to show, is you highlight kind of a variable
[42:03] or something that's part of the system, and it's gonna give you an outline
[42:07] of the documentation about it. So, it's gonna tell you kind of
[42:10] when it was added to the system, and I'm gonna click on it and probably break things,
[42:16] but that's fine. - I clicked on it, and I'm laughing.
[42:20] - (laughs) Oh, no, that's embarrassing. - Let's try one of the other ones,
[42:28] and we'll just leave that right there, see if it will, okay, let's highlight.
[42:35] Oh, now it's like much longer. - Yeah, it's having a moment.
[42:43] We'll leave it be, we'll leave it be. But the point is, it kind of builds in
[42:48] the documentation into the system, so you're supposed to kind of get a bit of a hint again
[42:52] about what things are doing what. - And if it's not giving you the right information,
[42:57] wait a minute and click again. - Apparently so.
[43:00] - (laughs) That's like all things technology, so you never know, you never know.
[43:06] - But basically what we're doing here with all the code that's on the screen
[43:10] is we are setting up the UI. So we're creating a binding between the UI file,
[43:16] which we'll have a look at in a minute, and our activity. So we can then access the components that are in the UI,
[43:23] we can kind of change colors, handle button presses, do any of the kind of things
[43:29] that you might normally do in an app. And this is what this code does.
[43:35] And then if you scroll a little bit down to line 31, this is an example of where we're then doing something.
[43:43] So what we've done is we've created this binding variable, and this binding variable is what,
[43:49] I mean, as its name suggests, binds our app code to our UI. So we've got binding and then .fab.
[43:58] Well, fab will be a UI element that we've defined in our UI file, which we'll see.
[44:05] And we set it, so we can see that here it's saying that it's a floating action button,
[44:11] which I guess is where fab comes from. And we've set the onClickListener on that.
[44:18] So when a user clicks the button, it will trigger this code.
[44:27] And what we're doing here is making it say a message, replace your own action with your own action,
[44:34] 'cause this is just demo code to show you. This is where you'd put some code to run the button.
[44:41] So I think the best thing we do at this stage is run the app.
[44:45] So you can see that code happening. - Okay. - So up the top here,
[44:49] there's a nice green plus run button. And you'll actually see to the left of that,
[44:56] it says Samson SM, blah, blah, blah, blah. So it's already connected to your device
[45:01] 'cause it's plugged in. So if you hit the run and we bring up the tablet view
[45:07] that you kind of had. - Which is somewhere over here, once close all these, that's fine.
[45:13] Oh, I wonder if the device is connected. Let me make sure it's unlocked
[45:18] and then I will reconnect it and possibly run again. - And then if we just check, oh, hello.
[45:38] - Duplicate class found. - Oh, that's interesting.
[45:43] Just try running it again because no, no, it's just, oh, it's good job, Android, good job.
[45:51] That's probably gonna take, yeah, that's. - Navigate class include.
[46:01] (indistinct) - This shouldn't happen, but of course it's going to
[46:15] 'cause we're live and that is just the nature of it. Honestly, the easiest way might be to create a new,
[46:28] like delete this project, create a new project. - Okay.
[46:32] - As we're just purely just to get the thing running. - Yes.
[46:36] - So close out of this one. - And we'll go get a new project.
[46:42] - Create a new one and we'll use the same, it should still be able to use basic activity.
[46:46] I don't really understand what's happened there, but we'll do that and then click next.
[46:51] And. - We'll just name this one yay, make it really easy.
[46:57] - Sure, sounds good. - All right, let it install all the things.
[47:05] - Yeah. - Am I making sure my, where'd it go?
[47:13] Why did you disconnect again? Is it like making it disconnect by running it?
[47:21] - Oh, it might be. Well, we'll see, 'cause we can run it
[47:27] and then reconnect once it's installed on your phone anyway, that's the old tablet, that's not a problem.
[47:33] Just a bit weird. - I might've clicked buttons too quickly.
[47:40] This is something I do very often. - It's all right. - I clicked it.
[47:45] - It's a good stress test. - I clicked it, I clicked it.
[47:48] - If you, and it's done the same thing. - Oh, Google, why must you, why must you be like this?
[47:56] - Oh, well, that's cool. I'm glad alarms are off on my tablet.
[47:59] So the tablet is still working. - Yeah, yeah.
[48:03] No, there's definitely, we might have to, that might be something
[48:15] we need to kind of delve deeper into. So unfortunately we might not actually be able
[48:19] to run it right now, but we can finish, we can finish going through everything
[48:24] and we'll see where we get to. - And Ryan, I feel like you, we eventually,
[48:32] when I have OBS going in, it can do all the alerts, is people can like do a counter of say,
[48:38] of how many times I say I clicked something when I wasn't supposed to, that would be fun.
[48:43] - I like that idea, I like that idea a lot. - All right, I'm gonna try it one more time.
[48:48] - Yeah, there's no harm in trying. - No. - No, it's not happy.
[48:53] Something is obviously broken and we'll figure that out. So, but the point is, this is kind of our main activity
[49:02] and this is where you would enter the application. You would go through this life cycle of when the app,
[49:09] when that screen is created, do something, when a user clicks on a button, do something
[49:14] and you can define all these things. Now, the other thing we wanna look at is the UI,
[49:20] the actual, what would be displayed on the screen, which unfortunately should have been able to show you,
[49:25] but whatever. So, you can see on the left-hand side,
[49:29] you've got your Java folder, but then we had this res folder.
[49:33] So, further down that one, yep. And this is basically all of the UI stuff,
[49:42] all of the kind of, if you've got any like images that you want in your app, any kind of assets,
[49:49] all those sorts of things go in this folder. So, the Java folder is purely for the code
[49:56] and then this folder is for everything else, which I get, okay, in this apps instance,
[50:03] isn't gonna be a lot, but there's stuff in there. So, one of the things is you have is your layouts.
[50:09] So, if we go on the activity main.xml file, that will be the layout for your activity train
[50:18] and it will actually render that as something that you can see.
[50:22] So, we can have this kind of visual design type thing and it tells you like, oh yeah, there's a,
[50:30] so basically that button in the bottom right-hand corner of the screen, the green.
[50:37] - Oh, this one, the email. - Yeah, yeah, yeah.
[50:40] That will be your button that you were triggering with that replace with your own code,
[50:45] with your own activity thing. So, you've got the design and this is the design layout.
[50:50] This lets you kind of play around with all the settings for these objects.
[50:55] You can kind of play around with like rotation and yeah, so you break things as much as you like.
[51:02] - Oh, this is exciting. I wanna spend like all my time here.
[51:06] - Yeah, and this is obviously, and it's all drag and drop as well.
[51:09] So, like you can take the text view and then drag it into your app and place it down.
[51:17] And then kind of, you have to set up the like layout to make it understand where it needs to be
[51:23] and it gets a little bit broken, but because of the type of layout that you're using.
[51:29] Again, they've recently updated these sample projects and they're way more confusing than they need to be.
[51:37] But if we have a part three, we might actually build something from scratch.
[51:42] - I feel like we need to have a part three, especially once I get my app built.
[51:48] I feel like that would be a great part three to have that on the show 'cause-
[51:51] - And that would be a good way to build something from scratch and kind of-
[51:55] - 'Cause this is really cool. Just even just getting to this point
[51:59] where people could see like what they could do. - Yeah.
[52:06] - I don't know why I'm like very confused about this like layout.
[52:10] - This is because it's basically using relative layout. So it doesn't work so well in this view.
[52:15] So if you go to the top right-hand corner, you've got design split and code.
[52:21] If you go to split, this gives you the actual HTML file on the left-hand side
[52:28] and then how that looks when it's been rendered on the other side.
[52:34] So you've clicked on your thing and it's now taking you down to this edit text element.
[52:40] And that is literally the code for that element. Annoyingly, it's behind the action bar.
[52:51] So you can't see your edit, but if you were to click on the thing
[52:55] that says, "Hello, first fragment." - Then I can change that one at least, right?
[53:02] Ah, no. - Yeah, no, that's fine.
[53:04] That's fine. So this is an example of an embedded file again.
[53:09] So that layout is a separate file here. So this is a much more simple file
[53:17] which should work a bit nicer. So you can literally then click on
[53:20] and then it's gonna take you, I think, to another file. Yeah, so there's another fragment.
[53:29] I just try it. Yeah, just try clicking on the actual,
[53:33] the text or the button either works. There we go.
[53:38] You see, it's all kind of embedded in itself. And this is why I think it's very strange
[53:43] that they've made these basic activities so confusing 'cause there's a lot going on.
[53:48] But there we go. We've got down to the actual UI.
[53:53] And here you've got the actual view and it says like, "Here's your text."
[53:58] And you can actually, you'll be able to move these elements
[54:00] around on the screen as well because they're basically-
[54:03] - Oh, you're a string going somewhere else. - So we need to go find that file.
[54:09] - It doesn't do the cool thing that it was doing earlier.
[54:15] - So let's go find that file. Let's do that.
[54:18] So on the very left-hand side, your projects is kind of minimized,
[54:23] but we want to read. There we go.
[54:27] So you've got all these different directories for all these different types of files
[54:31] and it's the values one that you're gonna want to look into.
[54:34] So you've got layout. - Yeah.
[54:36] - And then there's a strings file, which is relates to that at string.
[54:41] And here's your text and where it's defined. Now you don't have to do this.
[54:47] You can actually write the text directly into that thing. But the reason why they recommend doing it like this
[54:54] is you can then do translations. So you can have a string file
[55:00] for each language that you want to support. And you've just got the one file
[55:04] that has to be translated as opposed to all the files. - Got it.
[55:10] So I got it to update. - Yeah.
[55:14] - And I don't think next was, oh, next is in here.
[55:18] I don't know. I just want to go see it now.
[55:32] - Yeah. - I'll take a second.
[55:36] But there you go. And that's kind of why they're splitting it out
[55:40] because then maybe you want to be able to support this app in Spanish or French or Chinese, whatever it might be.
[55:48] You would just have a separate strings file that has the correct translated text.
[55:54] - Interesting. Okay.
[55:57] So now I'm like, I feel like you have to be back on the show
[56:03] 'cause I have like this huge curiosity of wanting to like actually see something like go through
[56:10] and having it as an Android app, at least the project I want to make would be so cool.
[56:18] So is there anything else you want to show us in here before I kind of like.
[56:25] - I think that kind of gives you a good overview of all the sections that make up an app.
[56:31] And then, yeah, the next thing would be to actually build something.
[56:33] But that's gonna take a while. - Yeah, right.
[56:36] Well, that one might be like, you're hanging out with us for a bit.
[56:39] Might be multiple streams. Yesterday I had a two hour stream to get started on this.
[56:45] And the reason I am bringing it up is, so I made a visual of it,
[56:56] but what I need to update is I'm going to, I'm going to move this away
[57:05] because I think it'd be good to still keep different versions of what I'm learning,
[57:10] but and option. So if I have, oh, let's do this.
[57:19] I'm gonna use Prisma for the backend. And then, so if I want to do this with Android,
[57:30] it would just be instead of, I could keep the rest of this the same,
[57:37] except it would be using Android Studio. - Yeah.
[57:42] So you'd literally just replace, you know, what we'd call the front end of the application.
[57:51] The database, it would be the same database. It could be the same, everything else.
[57:56] - Okay. - And you said that it does work with Node.js
[58:01] because it would just be connecting to Node.js. - Yeah, we'd just have,
[58:05] we'd have like that API interaction. So yeah, completely possible.
[58:11] - Yay, this is exciting. I am very, very excited.
[58:14] And for those who are joining today, and also just 'cause I really want to show you Zach, Zachary.
[58:20] I feel like I go back and forth. I'm like, is it Zach, Zachary, Zach, Zachary, Zach, Zachary
[58:26] is everybody enters their, because right now the way it happens
[58:30] is I manually create these Twitter spaces on Wednesdays. - Yeah.
[58:36] - Every Wednesday, it's really annoying because I copy and paste it.
[58:40] And I'm like, what if someone doesn't want to go in there? So the overall goal is to enter Twitter handles.
[58:47] Like somebody can go on the website and enter it and say, cool, I accept.
[58:52] I entered Twitter space link. The database combines it
[58:55] and the Twitter API will spit out this and auto post. - Okay, yeah.
[59:03] - So this is yesterday we were working on the React JavaScript web app.
[59:09] And now next I'm gonna set up Prisma and then MySQL. I have a feeling there's gonna be something I need
[59:15] between MySQL and the Twitter API, but we'll- - Probably be Prisma again.
[59:22] - Oh, I'll put that as a question. - Yeah, you'd kind of have it coming back out
[59:28] from the database through Prisma to the Twitter API. - Okay, we'll find out, it's fine.
[59:35] This is a huge learning curve. So this is what we will be working on.
[59:42] So once I get the app built, then I will let you know. But I feel like we can definitely get it scheduled
[59:50] and all of that because that gives me a deadline as well. - Oh, yeah, sounds good.
[59:55] - Yay, this has been great. And thank you for coming on the show today, Zachary.
[59:59] It's so much knowledge drops. And before we end the stream today, y'all,
[60:05] anyone have any other questions? Yay for Zachary coming back later on
[60:10] because I honestly went to go get a tablet this week and I'm through and through an iPhone and Mac user.
[60:19] Y'all have heard that before, but I'm like, this is actually really cool.
[60:25] I now want to build an app, like really bad, a real one. Well, thank you, yay.
[60:35] All right, everyone have a wonderful day, night, evening, and weekend, buh-bye.

