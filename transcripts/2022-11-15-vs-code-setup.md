---
showLink: "https://www.youtube.com/watch?v=GD8GVIBA4GY"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "vs-code-setup"
title: "VS Code Setup"
publishDate: "2022-11-15"
coverImage: "https://i.ytimg.com/vi/GD8GVIBA4GY/maxresdefault.jpg"
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

[00:00] There we go. We're live. We're live! Hello, hello, beautiful humans. Welcome back
[00:06] to another Tuesday with Jay. And whoa, whoa, Twitch is going on a different, different tab and scared the bananas out of me
[00:18] hearing myself talk. Keep the bananas in the peels.
[00:22] Okay, I am alive. Scared me but we're here and we are doing this. Today we are talking with Jay about VS Code. And I'm
[00:36] pretty excited about this. But Jay, for those who are new to haven't seen you on the show, and also to VS Code, could you
[00:44] introduce yourself and what we're talking about today? Yeah, I'm Jay. I'm a senior cloud advocate at Microsoft. I
[00:53] mostly do Python things every once in a while. Jen and friends get me to do some TypeScript things, and I'm not
[01:01] good at TypeScript. I'm just saying that now. But my job is to mostly talk to developers about things Azure and things
[01:11] VS Code. So when Jen said, "Hey, I want to talk things VS Code." I was like, "Sweet, let's let's do my job, I guess."
[01:19] Yay. And yes, hello, homie, first off, and then yes. So y'all, VS Code can do a lot of cool shenanigans. And all I use
[01:33] it for is like out of the box, other than like installing Python to it.
[01:37] I was just talking to someone about this yesterday about one of the things I like about VS Code is that if you don't have
[01:46] time to make it yours, it works right out the box really well. Yeah, and you can take the time that you need to slowly make it
[01:56] more and more yours. And if things go away, or things are no longer needed, you can continue to modify it without having to
[02:05] like completely rebuild the wheel every time. But even if your wheel is just the basic editor itself, that's probably
[02:12] good enough in many cases. Yay, and Yere is joining us from YouTube and said, "Glad to make
[02:24] it in time for their lunchtime. See if I can talk." Wow, words. Words, Jen, they are a thing. And what up, Anthony? Yay, we
[02:36] got a crew today. Now, I will say that it's like all of the originals. So my very first stream was with Yere, and then
[02:48] my second stream was with Anthony. And I'm pretty sure it was Anthony who talked me through how to download VS Code.
[02:54] And then I kind of sort of added things since then. But again, it's been like, to do Python.
[03:00] And just as I know that I've grown that I can Google this, but just in case other people are looking at this for the very
[03:11] first time as like, "Hey, what is VS Code? And we should look at it." I'm going to share my entire screen once I figure out
[03:22] what screen I want. There we go. And maybe, maybe. VS Code. That's basically how I've learned about as a developer or
[03:41] dev rel or anybody in tech. The key part of your job is learning how to Google, and Google well. And my Google-ness
[03:51] is getting better. But half the time I'm reaching out to actually one of you that are here today going, "Hey, how do I
[03:58] Google this?" My words don't make sense. Yeah. Well, let's, I want to, I want to first get a good
[04:07] understanding of where you are with VS Code. So VS Code is, well, actually, here's a quick quiz. One question quiz. Is VS
[04:17] Code a code editor and IDE? Both? Neither? Or Jay, what are you talking about?
[04:25] Okay, I feel, so it's, it's both. Although I feel like I want to hear your explanation of it. So I'm not going to do the
[04:36] correct answer and say, what are you talking about? Okay, well, it, the answer is it depends. That's, that's always
[04:45] the answer. Especially in dev rel, the answer is always it depends. Because can it be set up to be an IDE? Absolutely. Is
[04:59] it considered an IDE by Microsoft? No. An IDE is an, yeah, nevermind. Google says that they're integrated
[05:08] development environment. IDEs traditionally give you all the tools that you need to run, test, build, deploy, all those
[05:16] things for your code. VS Code, by design, is not an IDE. It's a code editor. It was meant to just give you a place to write
[05:28] code. The big brother of VS Code, Visual Studio, is an IDE. Out of the box, it has a lot of the tools that you need to run,
[05:37] test, develop, deploy your code, mostly C# or C, those, those type of things, traditionally. Also, if there's anyone from
[05:46] Microsoft watching, and I'm getting any of this wrong, feel free to correct me. I just pretend to know what I'm doing.
[05:52] Or come on the stream and come hang out with us. You know, we can do another episode.
[05:57] That being said, one of the things that VS Code has that has kind of become the standard nowadays is a rich extension
[06:10] ecosystem. You said some things about setting up VS Code for Python and things like that. VS Code has one, I don't want to
[06:24] call it a weakness, because I think it is a strength. But I think that the people that don't use VS Code or specifically
[06:31] don't like VS Code always don't like it for the same reason. And that's because VS Code has to be as much as it can be for
[06:41] all the languages, C#, Python, JavaScript, Rust, you know, all those things. It can't dive deep. It can't be a T-shaped
[06:51] developer where it's like general for most things and then really good at one thing. It has to be kind of medium, like
[06:58] breadth for everything else. I'm giggling because I feel like you just described a dev rel.
[07:04] Yeah, I mean, that's, that's actually, that's really, it's really astute observation there. I like that.
[07:12] Like VS Code is a dev rel. You got, you kind of have to be good at good or decent at everything. And then, you know,
[07:21] find the people that are really good at something to figure the rest out.
[07:24] Yeah, I do think that developer advocates are like, you know, folks, folks in dev rel in general can kind of have that
[07:31] T-shape. Like if you're really good at testing, my good friend Andrew Knight, like, he's a developer advocate, but he's
[07:39] like, really good at testing. So all of his stuff is focused in the testing space, but he still has to have all those other
[07:46] really good skill sets. Like for me, I would say my, my most deft, depth, most deft, that's an artist, but most depth is in
[07:59] like Python and like automation hacking and like tinkering and things. So anything that is DevOps or, you know, integrated
[08:09] systems or anything that's, that's pretty low level, I am going to have to lean on other people a little bit more. But
[08:16] when it comes to like, hey, I built this little package that does one thing and does it really well, I'm really good at
[08:23] that. And that's the area that I like to be in or API hacking. Oh, hey, I found some API and I want to get the most out of it.
[08:30] Or I want to build a wrapper around it. Like these are things that I have kind of built my career on is like, Oh, hey, this
[08:38] thing has some API, let's dive deep into it. And let's use that to get our job done. VS code is a lot like that. It's out of the
[08:46] box, it's going to let you just write your code, it's going to give you all of the good benefits of a code editor. But
[08:53] then when it comes to doing all the specialty things, that's when you're going to have to lean on those extensions. And
[09:00] the extension ecosystem is so it's, it's surprisingly vast and narrow at the same time, like, there are so many great
[09:08] extensions out there so many great themes out there. But when you need it to do a very, very, very specific thing, you tend to
[09:18] like, either miss or there tends to be something that wasn't maintained, you know, for a while. And that that can be a
[09:25] problem when it comes to relying on extension ecosystems, which is why, you know, when we talk about things like Python, or
[09:33] Rust, or like these, these really big ones, Microsoft just develops the the extensions themselves, because they can
[09:39] actually hire a team to manage them, like the the team that manages the Python extension is like, I think it's like eight
[09:46] people. And that's what they do is they develop VS code extensions, and they interact with the VS code core team to
[09:55] make sure that things run the way that people expect them to. So to repeat some of that back to you. It's like, VS code can,
[10:10] it's kind of like wants to be friends with everybody and do a little bit of everything, which makes it really cool. Yet,
[10:18] installing a theme and defining theme theme is just where the way it looks, or does that change the way it interacts?
[10:27] Just the way it looks, a theme specifically will only change things like your color palette, background fonts, font types,
[10:36] font colors, all those things. I'm pretty sure that's the case. There are some extensions that will VS code gives you access to
[10:47] certain areas of VS code when you're an extension developer, and your extension can insert objects inside of those areas
[10:57] but ultimately, you can't really manipulate them without, you know, manipulating the core level code, but you can add your
[11:06] code to it, which VS code is an Electron app, I believe it's an Electron app, almost certain it's an Electron app. But what
[11:15] that means is like, if you've ever worked with JavaScript, Electron is effectively JavaScript. So the way that you
[11:22] add things to it, you add them like you would JavaScript, you say, hey, I want this thing to exist, insert it in this
[11:30] particular area. And that area is almost like a div. So you can say, hey, I want in this div there to be this component that
[11:36] does these things. Right. And the big difference is that, you know, in a lot of this is additive, you can't just say,
[11:43] hey, obliterate this div, I never want to see it ever again. But you know, you can you can definitely say, hey, add my
[11:49] logic or add my code to it. Which, you know, means that they have, again, playing with extensions playing with themes,
[11:57] there's always a danger of bloat or doing too much. So even once you get it set up, I would, I would definitely suggest take
[12:08] inventory of what you're using, take inventory of what you're not using. Just because over time, you need stuff, you try it
[12:15] out, it works for a while, then all of a sudden, you determine you don't need it anymore. And then now you're like, well,
[12:21] it's taking up key commands, it's taking up, you know, real estate that can be devoted to other things. If I don't need
[12:29] it, then I'm not going to use I'm not going to remove it, you know?
[12:32] Yeah. And, and that makes sense. I, I would say, this goes into like a deeper conversation at some point of, like, if you were
[12:45] to get a brand new computer, what would you set up, we have had a stream like that with Anthony, although it took
[12:52] forever for I think we were installing node. So the entire stream was just waiting for node to install. But I feel like it's
[13:01] kind of similar to when you have your extensions and things like that, because then you learn what you always don't realize
[13:07] you may use. And yet, at the same time, if I never needed to touch Python, again, that would be an extension that I don't
[13:15] necessarily need to have anymore, or download that language. If it was, I downloaded specifically through
[13:22] VS code, because there is a extension on there for it. Yet something that comes to mind that I think it was actually
[13:31] your stream that had you did like a chat within VS code for Twitch. Yeah, there's like the coolest. Um, so that's kind of
[13:43] how I like differentiate, like maybe like an extension to a theme, because an extension is something that adds to it where
[13:52] a theme just changes the look. Yeah, 1000%. And that extension, the the Twitch chat theme thing,
[13:58] like, that's just because I'm really bad at checking chat. So I have chat literally up next to me while I'm coding. Like that
[14:05] just makes life easier. I get it. I get it. It's true. I luckily my setup is I see my
[14:13] chat when I'm like looking at the person. But as soon as I start coding, or doing stuff, I'm like, Oh, wait, I forgot
[14:19] about chat. Luckily, a lot of the guests are also streamers. And they're like, Jen, you haven't replied to anything.
[14:25] It's not bad. That's cool. Alright, so now that we have like a better understanding of what? Well, yes, we have a
[14:38] better understanding of what VS code is yet at the same time. I didn't know that Visual Studio was a thing.
[14:44] Depending on depending on what industry you're in, or what language you work with, it may not be a thing. That's like,
[14:52] it's like, what's the X code? Not? Is it? Yeah, X code for like, Apple, like iOS and Mac, Mac OS app development and stuff.
[15:02] Like, the only reason I think about it is because when I have to install Python, it's like, Oh, you usually need to run like
[15:11] X code setup tools or whatever to get it to work properly. But other than that, like, I don't I don't go into it. And I think
[15:19] I've used Visual Studio like once in my life. That was when I was asked to do some C sharp development. I was like, I do
[15:28] not do C sharp development. I'm sorry. So yeah, it's it's not a requirement. You don't have to know Visual Studio to know
[15:35] Visual Studio code. Absolutely not a requirement. That is good to know. Because I honestly had no idea that even
[15:41] existed until you just said it. I'm like, Oh, interesting. Okay, net friends are probably like yelling at me. Don't tell
[15:49] them that. Yeah, yeah, there I will say there is so much more that we
[15:56] can have on teach gen tech and we will have on the future yet. Oh, we just said, Jane, Jay summed up a good piece of what
[16:06] code is it. It just makes life easier. I dig it. I dig it. And alright, so I already have VS code installed. I have dropped
[16:20] in the chat earlier on how to like the link to install it. So go back to my share screen. If we were installing it, I would
[16:33] download Mac universal, but I already have it installed. So do you have an M one device? No. Okay, you still have the Intel
[16:43] Mac? Yeah. Okay. Once I get a job, I will. I'm at least guessing that's the type of laptop that they'll give me is
[16:50] an M one. Probably. We're in M2 land now. So maybe that would be great. Um, okay, I feel like I have an extension that reload
[17:03] required. Okay, well, we can look at those. But where would you like to start with VS code? Um, I mean, let's let's start
[17:11] with like, what you have, go ahead and do that reload. I mean, it takes no time at all. required. And then yeah, we'll
[17:20] see what you have installed. And we'll kind of go from there. So let's, you can minimize that recommended. I don't, we might
[17:29] be in there. I don't know how long we'll be in there. We probably won't be in there. Go ahead. And there you go.
[17:35] Perfect. All right. So what do we have? Um, all right. So yes, let that that's probably smart. You're doing JavaScript stuff.
[17:44] So having a linter for it, go. If you're doing go stuff, then I had go, but I, I feel like they're not going to be on the
[17:53] show again anytime soon. So we'll just uninstall that one. You can always install things again. And this isn't a like,
[17:58] let's clean up extensions. I'm more just trying to figure out what's there. It says you have 20 extensions installed. So you
[18:05] know, that's, that's always nice. HTML lint. I'm seeing this migrate button. Just hover over it. Don't click migrate hover
[18:11] over the it's deprecated. Use the HTML a different Oh, went from HTML hint to HTML. And okay. Um, what is this? I don't
[18:26] know what this is. I don't know what it is either. I will say I definitely installed some random things when I first got started
[18:35] because I didn't know what they do. Um, we'll come back to that. Let's just keep going. We can probably remove this. Yeah, I'm
[18:42] gonna remove it. And if I miss it, I'll bring it back. That's the beauty of it. Alright, so we got Jupyter stuff. If you're
[18:48] doing Jupyter things, I definitely recommend Jupyter. Are you familiar with Jupyter notebooks?
[18:54] Really quick, just to make sure I remember what Jupyter is. Jupyter is for the
[19:00] goodness gracious for Python. I know. Yes, yes. Um, Jupyter notebooks have kind of blossomed
[19:14] out of Python. I do believe you can use Jupyter notebooks with other languages. But the basics of it are Python. And maybe
[19:23] maybe that's even wrong. But Jupyter Yeah, like Jupyter is designed to work with Python. But then there's there's other
[19:37] there's other versions of Jupyter that allow you to do other languages. So yeah, you're ultimately Yeah, that's that's
[19:46] probably what you downloaded it for was to do things with Python.
[19:52] Okay, a live server. Well, you have live server and live share live server launch development local server. That's I mean,
[20:07] again, I don't know what any of these are. Let's just keep going. I know live share live show. Okay. Live share audio and
[20:13] things like that. I didn't know. They got they got that that deep into it. But yeah, you can just do audio like we can live server.
[20:23] I from what Anthony said, live server runs an HTML page really easily. Okay, so it's it's okay. It's whatever. We can keep
[20:34] going. Markdown lit. Cool. prettier. Cool. Prisma. Okay, Prisma. I've done probably be back on the show. So I'll just
[20:45] leave that one. Okay, cool. Um, pylance, Python, stylants, or style, I don't know, style, but okay, interesting. And then you
[20:59] have spell. Okay, cool. So it seems like you have your base language things, the things that you're you're using to make
[21:08] working with the language easier Python being a big one spell. I forgot one of the ones up there. I mean, you had go, but that's
[21:16] gone. And then you had yes, which is good. Oh, it's the go live button in the status bar. Oh, yay. So what
[21:27] is the go live button? It shows you it will like pop up an HTML and show you what it looks like. Okay, that's just so more live
[21:36] server stuff. Yeah, that's what the live Oh, that's what live server does is you hit go live and then it just pulls up a
[21:43] little browser window. I do Python development, which means that I wound up running my server, like Python dash m HTTP
[21:52] dot server and then you're up and running but or using flask or whatever and it does it for you. So yeah, that's, that's
[22:00] fine. I think I actually have that installed. It might be one of those things that I like you, I just installed and was like,
[22:05] okay, cool. Um, what themes do we got rocking right now? I didn't see any themes. Um, well, real quick. What up Bikari?
[22:16] Thank you for joining today. And to be honest, I don't even know where you go to themes. Just type theme. I don't I probably
[22:26] don't have a theme because yeah, now go up to the little filter icon up there. Right there. And I thought there was one for
[22:37] installed. Interesting. Go to the three dots. All right, well, easy enough. Let's I'm gonna open up VS code and figure out
[22:51] why that didn't do what I thought it did. Could it be just because I don't have any? No, installed?
[22:59] No, there's like a there's an actual filter for things that are installed. But I can't remember what it is. There's
[23:09] also another way to do this, it's probably a little bit easier. Going back into that little filter icon, go to
[23:15] category. And then you have themes down there at the bottom, which, again, that's a thing that if you're not sure about,
[23:24] you can definitely like, filter in and do things. That that being said, a lot of there it is at installed. I knew there was
[23:34] a thing just to add installed and then category at category themes. It's probably going to overwrite it when you do that.
[23:43] But you can. Yeah, just add. Can I add just add installed afterward?
[23:50] Yeah, you can. Yeah, so no themes. Yay.
[23:54] All right. Thank you, homie.
[23:58] So at this point, the so you got no themes. That's I mean, again, that's fine. Out of the box. It's not bad. The next
[24:10] thing that I want to ask you about is do you know what the command palette is?
[24:13] The thing that never works. Okay, hit Command Shift P.
[24:19] I have to do this every single time because it does not like me.
[24:28] That's all I know about this is it does not work. Huh?
[24:36] It does not work. So that's the only reason I even know that that commands a thing.
[24:42] That's how you know the command palette is there. Yes.
[24:45] Interesting. Go to terminal.
[24:48] Oh, no, don't do that. No, I'm just showing you. If I go to CD, desktop, code. And
[25:02] I'll just see if I could open this folder. No command found.
[25:07] I mean, I do that. Do I do that? Watch. And then this is this is magic. If I do this.
[25:17] And then click it. Oh, yeah. And I hit OK. Yeah, then it works.
[25:22] It's magic. But this is a the only reason why I know that thing is there is because I have to click it every single time.
[25:32] And and are you familiar with? Okay, that's why. Sorry.
[25:41] I did try to fix it once. And then Anthony had to come on my stream because I really broke stuff.
[25:50] That's okay. All right. So we're gonna we're gonna throw down the command palette really quick. And we're going to just type in
[25:57] theme. And what do we get? We should get some options there. Sorry, I keep jumping off.
[26:09] There you go. All right. So you can you can now start moving in doing things that you want. If you go to like preferences,
[26:20] toggle between light and dark themes. Retina, retina burning warning. Sorry, God. Yeah. Yeah. Okay. So how would you how would
[26:29] you change that? There you go. How do I go back? Oh, my God, that really hurt. I should have
[26:38] given myself the warning of like, it's going to the light theme.
[26:41] Yep, yep, yep. Oh, hi, Dali. Yes. Hey, Abu Dhali. And yes, Bakari my eyes that hurt. I'm
[26:53] struggling with that. So a lot of this a lot of this stuff is going to be going
[26:58] through like, we're going to do something and then we're going to use the command palette to make some changes. Okay, so I
[27:05] just wanted to make sure that we know what that is. And that you understand that if you click the wrong thing, your eyes will be
[27:10] burned. That was a mean joke. And I'm sorry. So I mean, I do overclick things. I go clicky clicky when I'm not supposed to.
[27:19] So I mean, it serves me right that at some point, it was just going to blind me.
[27:22] There we go. All right. So the next thing we got to figure out is, how's your how's your appetite for keyboard shortcuts?
[27:31] If I write them down, they're happy until they come to memory. But until then, I never forget it. Remember anything? Although
[27:39] wait, wait, wait, wait, is it? Yay. Okay. It's Command J. Oh. Oh, interesting.
[27:50] Command J goes to your terminal, turns it on and off. It goes to my debug console. That's I was like, if you do
[27:59] control tilde, it'll also yeah. That was fun. That's another thing. We're gonna we're gonna have a lot of little things
[28:13] today like that. The reason I'm asking is, as we as we move things, some things we might want back and the easiest way to
[28:20] get them back isn't to hunt for them. It's to know the command key. Like for extensions, it's going to be I got to remember
[28:26] this now. Because if I don't do it, that I will get it wrong. Command Shift X. Yes. So Command Shift X will will do that.
[28:41] Okay, so we got y'all I am totally writing writing these down. So you'll have to give me a minute. The reason I'm doing
[28:51] this, though, is because, for me, there's a difference of writing it and typing it. If I write it, a lot of times I
[28:58] remember it, whereas if I type it, probably not. Yeah. So a lot of a lot of this stream is going to be just
[29:04] getting you familiar with where things are, how to get to them, how to get to them quickly, how to remove them, and how to bring
[29:11] them back. And I'm also having to like, bring up my own VS code window just to see where things are. Because there's, I'm like
[29:26] looking at your screen. Oh my god, where is this thing? Also, what is that thing? What is the thing underneath the extensions
[29:32] icon that looks like a notebook? Just hover over it. You don't have to click it.
[29:36] Oh, I think it's juniper. Jupiter. Okay. I don't even know what it does. It's there.
[29:42] Okay, that's fine. And this is how we get rid of it. Right click hide.
[29:46] Thanks. Now it's gone. And then something else will take its
[29:51] place. And this this is exactly the that's fine. You can hide that one too.
[29:57] No, I like the live share that one. Because we use that. Wait, do we use live? We didn't. Yeah. Right. Yeah. Yeah. So I like
[30:07] live share because that was where I was getting really lost is because that other button was there.
[30:11] Yeah. So Explorer is another one that you're going to need to remember just Command Shift E. I click it. I don't. I don't hit
[30:20] Command Shift D usually unless I'm trying to hide it, which is kind of funny. Because you have to press it twice. If it's not
[30:28] like the main window, you have to press it twice in order for it to hide. Actually. Oh, wait, no, it doesn't hide. Nevermind.
[30:35] I lied to you. So you have to click it anyway. So yeah, you want to hide it?
[30:40] Yep. I just have to click it to hide it. I thought you could hide it easily. My bad. And then find, are you familiar with
[30:49] the different finds that are there? No, no, I was reaching for that one. You know, I'm like, do I
[31:00] remember that? No. All right, let's just pull up some code, any code, the code
[31:04] itself doesn't matter. Open recent.
[31:10] There we go. Open some recent. I like it. Uh, this one is, I can. Thank you, homie.
[31:20] All right. So if, if you're looking for the word Tweety tag, and I know that it's at the very top, how would you find Tweety
[31:32] tag? Yeah, apparently typing. Um, well,
[31:37] without clicking on it. Out of curiosity, though, if does JavaScript do this too? Or
[31:46] is it just TypeScript, where if you go to go to definition, it actually like tries to find the original?
[31:53] Um, I don't know if JavaScript does it. I'm sure it does. Python does it as well.
[31:58] Oh, okay. Um, I don't know. I'm gonna try command find. No. Unhighlight it. Unhighlight it.
[32:05] No, that's because you you selected it. You hit command F, which brings it in there for, you know, good feelings.
[32:15] Yeah. All right. If you tap down things. Oh, it's replaced. That's fine.
[32:22] Yep. So now what if you wanted to find, uh, let's do something that will be, will exist a lot. Uh, what if you wanted to find
[32:31] it, uh, tweet, just the word tweet, but you wanted to find it in all of the documents in your project?
[32:39] Okay. Okay. That was just a solid guess of, uh, because everything else is command shift. So I'm like, let's just
[32:51] try command shift F, see if this works. Another just random click, see if it works kind of magic.
[32:56] I like it. That that just means that it's intuitive. I just searched for Prisma because I don't know how often I
[33:06] actually said tweet in it. Perfectly fine. Um, and then do you know what the buttons on the
[33:11] side of that search window do? Also, there's an echo. I don't know if that's me or you.
[33:16] Oh, that's new. Give me a second. Is that any better?
[33:26] Um, nope. Thank you, Mike. Thank you. I appreciate this.
[33:33] Um, let me go grab my headphones BRB.
[33:40] Okay. Hey, chat. How's it going? Happy to sit here. Oh, now it's gone. Interesting. I think I think she has StreamYard like
[33:51] echo cancellation on and it is canceling. It's not canceling because she's typing or talking. So therefore, all the echo is
[34:03] popping up. But yeah, chat. What's how you been? How's life treating you? Happy to have this here in chat. By the way, I
[34:11] guess I should I should mention, I know I haven't streamed personally in a while. That's not because I don't want to
[34:17] stream. That's because it's been busy. Am I always so chill? Um, I think so. No, not really. Sometimes I'm, I'm an anxious
[34:30] mess. But when I'm on, I'm pretty chill. That's, that's kind of my brand. But that's something that that's something
[34:39] that I think Jen will learn. Getting into DevRel a lot is that there's a difference between being on and you can you
[34:49] get? Yeah, I just hit my knee on the desk. And it's like everything
[34:54] shook. Please continue. I was listening. Yeah, so we're talking about homie asked, Am I always so
[35:02] chill? And I was like, Oh, no, not really. But when I'm on stream, yes. And when I'm on stage, absolutely. It's it's not
[35:11] a gimmick. It's it's this idea of what's called being on. And when you're a developer advocate, you have to I don't
[35:23] want to say masking because masking is kind of a negative thing. But I can't bring all of my anxiety and all my concerns
[35:32] and all of my like quirks to everyone when I'm working. So you have like a default and your default is what we call Yeah,
[35:43] it's like getting into character. It's like I'm not like, I am being my authentic self. But I am also just not
[35:51] letting people see the things that are going to cause them to like, you know, freak out, which again, for me, is a little bit
[36:01] easier to do, because I am relatively open about having anxiety, having some mental health things. And, you know,
[36:09] that kind of liberates me to be able to just be like, yo, if I don't know, I'm not going to pretend that I know. And that's
[36:15] that's what I mean by like, trying to be authentic of like, I try to be chill, but I try to be chill for like myself. And I
[36:20] try to be chill while I'm teaching. Because if I'm like, no, don't do that. No, no, stop that. Like, like, all that's
[36:26] gonna do is cause the person that I'm working with to get anxious. So I just try to just try to keep it relaxed. You
[36:34] know, when I'm off stream, when I'm off camera, I'm listening to chill music and stuff like that. But I'm often like, cursing out
[36:43] my monitor because, you know, the outcome wasn't what I expected. I may or may not have thrown my phone before getting
[36:55] mad. That costs money. Don't do that.
[36:58] I mean, luckily, I've learned that the hard way. And also I, I grew up, I say I grew up in the cell phone industry. It was like
[37:08] my first job for seven years. What is that? It's, well, sorry, camera. It's like a little fidgety thing. But
[37:14] the nice thing about it is one, it makes noise. But then also, you can drop it and it's flexible until you get really
[37:22] angry and you just want to break it. And I'm apparently I can't break it right now. Because it's one of those little puzzle
[37:29] things. And they breaks into a bunch of little pieces. Yeah, like that. So
[37:34] yes. And I think that's a big thing of like, in general, even if you're a live streamer, and not like a devil or anything is
[37:45] like you figure out, like getting into character, but you also see who your character is. And I feel like that's so
[37:54] different for many of us where if I'm not on, I am actually like hiding under the covers and don't want to move and just want
[38:03] to sleep all the time. Where when I'm on, I am very energetic. That's naturally who I am. Yet it's more amplified
[38:12] when I'm around other people, because I'm like, okay, cool. Like, if I can be in, like a hype mode, I know that it will
[38:20] hype everyone else up. Exactly. And that's so yes, that's such a big thing. When
[38:27] you're streaming when you're on stage, like, Oh, yeah, I know those things. Yeah, when you're when you're presenting, you
[38:38] don't want to be a downer. Like, especially like, for me, like, I, a lot of my topics are hard topics. So I don't want to be
[38:48] talking about, like, super challenging topics, like, you know, systemic racism, and like data collection and things like
[38:57] that, which are talks that I've done, while also being super, like, melancholic, and like, extremely, I don't even know the
[39:08] right adjective there. But just being like, Okay, well, we're gonna talk about this, I guess, and that it like, nah, I'm
[39:15] gonna, I'm gonna let my excitement and my passion kind of bleed through. Because what that does is that tells people
[39:21] that one, I'm going to be talking about difficult topics, but I not doing it from the like, let's burn it all down and
[39:28] start over. It's like, no, this is the thing that I care about. And I want you to see that care. I want you to see the care that
[39:35] I took to prepare this. But I also want you to see the importance to me in the topic itself. So that's, that's where
[39:45] like, I tend to think being chill. And you know, for me is kind of the thing. There it goes. I'll put it back together.
[39:52] Finally, took me a second. But you got to like being chill is great, because being chill kind of sets the tone. If all of a
[40:01] sudden, I am like super hype, and I'm like, really driving it in. That means it's something that's really important. But if
[40:08] that's my baseline, it's really hard to set those differences. And like, I love how I'm basically the opposite. Hype is
[40:19] like my default mode, but especially with like the podcast. And for those who may not know, I have a podcast
[40:25] called shit you don't want to talk about. And to Jay's point, I've talked about systemic racism on there. And it's
[40:34] definitely, you learn to be a storyteller, and where your, your natural character, your natural abilities come through,
[40:48] where yes, default is my hype. But when I slow down, and I get quieter, people know to take me more seriously, because it's a
[40:57] serious topic. And it's not something to be brushed aside. Yet, I am really hype. And I do get louder, because I like to
[41:06] live in the world of everything's going to be great. And we're going to be in a perfect world. And I'm going to
[41:10] convince everyone of it, even if by the time I get home, I will be completely drained and don't want to talk to anyone. And I
[41:15] hate people. I love humans. And I hate humans. It's a very weird thing. So it's like this weird, like dynamic that we all
[41:23] end up having to learn about ourselves and being in the public eye.
[41:28] Yeah, by the way, that little puzzle thing, I think I found it like Barnes and Noble one time. Then I was like, Oh, little
[41:36] little puzzles. And then yeah, I just, I was like, Okay, cool. Something to fidget with that. If ultimately I'm having a bad
[41:43] day, it breaks into a million pieces, or at least six. Let's let's jump back into some VS code stuff.
[41:51] Uh, I will, I just started googling it for the round puzzle. And let me let me just like move this over here,
[42:00] because I'm very, very, very confused. I'm on this as Yeah. Oh, no. Yeah, there you go. That $25 one is still
[42:16] overpriced, but that's a little bit more. That's a little closer to what I paid. I think it was like $10 is more like that
[42:24] jungle wooden puzzle. Again, that was really cool. Yeah. Oh, that lion is pretty dope. I like that. But yeah, um,
[42:32] anyway, super ADHD brains over here. And it's fun. So VS code, we are over here and we searched.
[42:44] But you search for Prisma, you don't know what the buttons do. Okay, now. So the buttons are, I mean, if you hover over them,
[42:50] they tell you and there are shortcuts for them. I don't know those shortcuts. There's a lot of shortcuts. That's that's a
[42:56] lot. So the the capital A lowercase a matches case, the bar underneath the A and the B matches the entire word. So if
[43:09] you click on the match entire word Prisma client should not show up. Boom. Well, it still shows up in this case, but
[43:19] that's because of something else in the line, not because of it itself, which is good to know when you're searching for
[43:25] something like if, if you're searching for tweet and not Tweety tag, using that will kind of clean up some of the stuff.
[43:33] And then that that dot and asterisk there. Do you have an idea of what that is?
[43:39] Okay, I didn't even get a chance to look at it. In my head. It means something like it. Or like, I honestly have no idea.
[43:50] It's it's for regular expressions or basically like a pattern matching. Let's let's try this. I want to find
[44:00] something special. Okay. Let's see if we can find all URLs. Yeah. Oh, yeah. You can select more than one. You want to find
[44:15] all URLs. Mm hmm. And we'll do like a rough all URLs. Well, that's cheating because the word URL was there. Yeah, but how
[44:28] would you search? Oh, like it would have Prisma in the URL. No, just we're looking for any and every URL that pops up. What
[44:38] what do what does every URL start with? Oh, HTTP. Like that. Okay, good start. Um, all right, then probably also the colon
[44:53] colon black backslash. So that would probably do it. But what if we had like, trying to think of? Oh, here's a good one. Okay,
[45:07] what if we just want Miro and GitHub? And that's it. So we don't have to remove HTTPS. We can leave that in. Now let's try
[45:15] this. You're going to do an open bracket. Bracket. Yeah, I have a space in there. By the way, you might
[45:25] want to get rid of the space. Yeah. All right. Now you're going to do Miro Miro. Oh, sorry. Put Miro in parentheses.
[45:39] Yep. And then you're gonna you know, this is cool. You're gonna need your bracket still. It's bracket parentheses Miro. Yep,
[45:59] then close, then close your parentheses. Now you're going to do open parentheses, GitHub, close parentheses.
[46:04] It did some things wrong. I was like wondering if it did the Miro one. What happens if I
[46:20] get rid of these? No. So ultimately, this is this is why a lot of people don't work
[46:31] with regular expressions, because they're not easy. They're not the easiest thing to do. That being said, they are a
[46:40] good tool to know if you know them. But the reason I the reason I wanted to show you that you should be able to do
[46:53] something like this, I'm going to type in the private chat. Interesting. Okay, you should be able to do something like that
[47:11] and have it basically give you either GitHub or Miro and those things, but that didn't seem to work. I don't know why it didn't
[47:19] work. I more than anything, I wanted to show you that there are like actual patterns that you can use for searching
[47:25] things. Like if you want to find every single time a number is used, you would use something like one of the slashes.
[47:33] Anthony's here. So yeah, like I said, I don't know why that's not working. But that could be something that I did wrong. If
[47:43] you do was that backslash forward slash one of the slashes, this slash, if you do that, in this search, it'll give
[47:53] you every number that is in your other slash. This one. There we go.
[48:05] Oh, yep. Now if you do that, add a plus sign to that. It's going to
[48:15] give you where there's one or more. Okay, remove the plus sign, add a curly brace, and then the number two, and then
[48:24] another curly and the closing curly brace. And that'll give you everywhere there's two of them. So these are these are
[48:35] really powerful search tools that you may want to, again, there will be times when you need these things. And like
[48:44] understanding how to actually get them is is really important. By the way, these options also appear in your single file
[48:54] search as well. So you can do all those things. But then yeah, like I said, you can, you can also just turn that off. And it
[49:02] won't. It won't cause problems. Yeah, anything says use regex one on one.com. That is a good one. There are also some
[49:11] applications that you can use like expressions. And there's a lot you can also, well, you're not using Copilot. Sorry, I keep
[49:18] forgetting that I use Copilot. So like, if you use Copilot, which I'm not going to tell you to because you're you're balling
[49:25] on a budget right now. And you don't need a monthly subscription. No, I don't. But you can actually say like, give
[49:35] me a regular expression that does this thing. And it usually will give it one give you one, which is kind of cool. All
[49:42] right, my copilot is like hitting one of you up. Exactly. What am I trying to say? No, that's that's fine. All right.
[49:52] So you know what Explorer is, you know, where your find window is, do you know the the Git navigation window? This one,
[50:07] that's it. All right. So I can't give you a lesson on Git. Git is confusing. And there's a lot that would have to go on and we
[50:15] don't have enough time for that. But if you're dealing with source control in VS code, you can use this window, you can
[50:24] also just use the terminal and do all the good stuff in there. Microsoft owns GitHub. So there's kind of some built in
[50:32] support for GitHub. Like that exists. I think there might be like, there's also the GitHub app or the GitHub extension. I
[50:43] would encourage you to use that too, if you're doing GitHub things. But again, I wanted to just make sure that we know what
[50:51] each of these do. So this is going to be where you, again, you, you commit, you push, you pull, I don't. Is this a project
[51:00] that's in GitHub? It is. And this is where like, I've had to, when I've created
[51:09] something, like I edited the readme in GitHub online, and then did something here, it was really dumb, of having to create
[51:17] a new branch. So that way, I could upload it to something. And then, yeah, so homie, and I have had a lot of fun doing
[51:28] this, specifically in this app, or this project, because I had to figure out all of this. And he's reminded me often to
[51:40] remember to pull the project, even if I have it up. So it's definitely a good reminder to always pull the project instead
[51:51] of just going for it. Yeah. And I mean, it won't let you push until you've pulled,
[51:58] but pulling first allows you to avoid conflicts. There is also a setting that I probably wouldn't recommend, which is like always
[52:10] pull first, because you get sometimes you pull stuff, and then stuff could get redacted. And that could be a problem. And
[52:19] a lot of, again, I just I wouldn't recommend it. But yeah, if you're working on something, pulling first isn't necessarily
[52:28] the worst advice that someone's given. And it's actually really good advice, and you should do it. Um, okay, so debug, do you
[52:36] know what the debug icon there you go. debug is one of those that's not everyone uses it. I use it only when I'm developing
[52:48] VS Code extension stuff. There are other options for doing some of this stuff. And I kind of like them better. So that said,
[53:03] we've kind of gone through all the things right click on, let me make sure I do this right. Oh, this is these are all the
[53:12] buttons that you have available to you in this moment. Oh, no, you don't go to the go to like that blank space under live
[53:20] share and right click there. Oh, all right. So these are all of the extensions that you have set up that you can move, remove,
[53:34] add, reduce all those things. So if there's one that you don't like, or you don't use, you can get rid of it, boom, it's gone.
[53:40] I mean, okay. I was just, you know, looking at it. So you know, you know how
[53:47] it goes, how it goes. Um, okay. This is cool. I will say, I'm going to be learning about more of the debugging with Anthony,
[54:07] he was on your show a while ago. That's a very descriptive way of saying someone because I'm horrible at names. And I just
[54:13] remember how I like met them normally. On my show.
[54:18] Nick, yes, Nick, Nick is gonna come on my show and talk about debugging and console and all of that.
[54:29] Oh, cool. Very nice. Yeah. I am. I am definitely not. I don't do debug. Like I said, unless I'm doing like, PS code extension
[54:40] testing. But I do testing. So that's kind of a different thing. All right. So we were talking about setting this up
[54:48] for Python development? Question mark? Sure.
[54:54] Okay, so the extensions that I have, let me see here. Um, I have 109 extensions installed. You have 18. You don't need 109.
[55:08] 109 is definitely more than necessary. Um, but there are some that and I'm going to run through this and just make sure
[55:23] I'm not giving you ones that we that you shouldn't have. Let's do one called to do highlighter.
[55:31] Stop one. Yeah, that's it. Install. This is a great little
[55:45] she have ADHD. It's a great little thing. Go go back to your little document there. What any of your documents, it doesn't
[55:54] matter. We're going to delete this right after we create it. So you can just go to a license is fine too. It doesn't matter.
[56:01] Just type in to do in all caps. Anywhere, anywhere. Oh, all caps. All caps.
[56:09] At a sorry at a Yeah, see how it now stands out a little bit of like, hey, this
[56:19] is the thing that you need to do. Put it on the same line. By the way. Now, right click that to
[56:34] do. I don't think this does it, but it might know on the actual to do part. Oh, okay, good. Hasn't doesn't do it yet. All
[56:46] right, by the time we're done with that to do it, we'll do something. So the next thing we're going to install is the
[56:51] GitHub pull requests and issues. There we go, install that.
[57:01] This is going to give you access to pull requests and issues inside of the project. So now go back to that to do
[57:07] right click it. Oh, sorry, hit the little yellow, but yellow light bulb
[57:17] there. Oh,
[57:20] so that's fun. You can also now highlight all of that and then click the little light bulb. And it's going to give you a bunch
[57:31] of different things that you can do. This is HTML lit, you don't want to do any of those things. Click on a line. So hit number
[57:38] six. Boom.
[57:45] Okay, it's still doing the thing. So what you can now do is if you highlight everything with that highlight everything
[57:50] with it to do in itself, that whole paragraph. Well, yeah, I was gonna say like, all that.
[57:57] Right click. Right. No, sorry, you're right. You're right. You're right. Hit the little light bulb. I wish I went away. Yeah, I
[58:07] wish there was a way to to get there we go. Oh, yay. Yeah, go ahead and create that issue. I
[58:14] just want to show you what it looks like. So you have that. That would just be what that looks like there. Let's hit that
[58:22] little there's no enter create the issue. Yeah. I hit enter. That's okay. There's no excited about that. There's no remote
[58:30] setup. So it didn't do anything. Go ahead and hit that create issue again.
[58:35] Hit the little pencil looking icon in the top right, right there. And what you see is it kind of does this thing to where
[58:47] now you have all this stuff that you can go in and add, you could add, you know, if you want to do that, I think you have to put
[58:54] the at symbol in front. I don't fully remember. Oh, it says either username or probably just their name. So that's good. And
[59:05] then label. So if you have labels, you can add them there. I think it will create new labels if you don't, they don't
[59:13] exist. But the nice thing here is you also have a link to where that exists in the code. So when you create that issue, you're
[59:26] going to have all your context. And underneath this, yeah, you could add whatever you want any description that you want after
[59:31] that. But it's also going to show where in the code that problem is. Okay. And can this go away?
[59:43] Yeah, hit Control F again, I think. Command F. Do it again. No, okay, it doesn't go away. It goes away. I don't know. I'm
[59:53] only seeing I'm not seeing all of your screen. I'm only seeing like, two thirds.
[59:58] Oh, sorry. We'll just do this. There. It should be the entire screen now.
[60:06] Yeah, hit the X on that bar. Oh, there we go. Yay. I must have been hiding the X from
[60:12] myself. So then if you hit that checkmark in the top right
[60:16] corner, it would create this issue. Again, you don't have a remote so it can't create it. You can just close this out. You
[60:23] don't have to do anything with it. How do I get a remote?
[60:27] You'd have to push this code to GitHub. I didn't pull it first. So probably not the best idea.
[60:39] Okay. And then yeah, let's what, Pomi, what is this thing that I keep hearing about?
[60:50] Oh, the manager? Oh, I was that was going to be the big, big ending, but since someone decided to ruin it. So the
[61:01] manager is this really cool extension that was created by homie coder. I actually, I actually have it installed on
[61:09] mine as well. That allows for streamers to show what theme and what font set they're using, which is really good. So you're
[61:24] using default dark plus, let's change that. Let's, let's find you some fonts that you might like. You can just, it'll go
[61:32] away if you will. I was wondering if it like, clicked. Okay, cool. Yay. Yay.
[61:37] Okay. Okay. So up in the extension, we're in the extension search
[61:43] window here. Let's try Studio Ghibli. G-H-I, it's G-H-I-B-L-I. I, I.
[61:59] Okay. Remove studio. Oh, there it is. Studio Ghibli inspired themes.
[62:08] Cool. Install. All right. I'm not sure how, how your, your Ghibli aesthetic is. I tend to
[62:22] like Kiki's delivery service personally. Okay. So now how do we change our theme? Well, yeah, like that. Good job.
[62:34] I got excited. Set theme color. Black. Okay, not that one. I don't like that one. I like Kiki's.
[62:44] Kiki's is subtle. But I really like the Spirited Away one. Set theme color. Go to
[62:51] Spirited Away. Okay. There. Okay. Yay. Oh, and then it's down here. Look at that.
[63:01] I see a bug in, in the code because it didn't update when the theme updated. But that's something that we can handle
[63:09] later. Don't bug like that. Bug fix already. So instead, let's do this. Let's, let's
[63:21] actually force it to update. Well, maybe we can force it update. I don't know if this will work or not. Open up the
[63:25] command palette again. Command shift p. And let's type in theme manager. Whoa, did we find another bug? Okay, type in
[63:46] current theme. And theme.
[63:50] Whoa, I think we found another bug. Okay, so I don't think it's going to update until we restart the client, which is. Oh,
[64:00] you're in file search. Wait, wait, wait, wait, wait, wait, nevermind. Cancel. Did you I think you did command P do
[64:05] command shift P. Command shift P.
[64:09] There you go. Now type in theme manager. There it is. Okay, display current theme. Oh, bug. Bugged. Okay, so we found a bug.
[64:27] That's okay. Because we can we can help make it better. That's what we're here for.
[64:32] We'll file an issue later. Or maybe homies already. I'm curious. I'm gonna don't save.
[64:41] Yeah, don't save. Did it update now? It updated. Yeah, it updated.
[64:51] Yeah. So currently, it's only checking it at application start. You might want to have it refresh anytime, maybe anytime
[65:02] an extension is full. It's like there's a theme change and things like that. Totally an option. Let's try some other
[65:10] ones. Let's go and add Dracula. These are just some of the themes that I like. So there's and this is one of the this is
[65:24] one of the the pain points of working with themes is there will be better versions. There's Dracula official, you can check
[65:32] Dracula at night, which might make it a little bit darker. There's Evan dev Dracula Dracula refined. Basically, everyone
[65:40] has their own opinion about which Dracula theme is the best. Ultimately, just find one that you like and you're good or you
[65:50] can slowly modify an existing one and then make it your own theme and then there will be another Dracula existing one.
[65:59] But I like the purple and pink. Oh, you're signing in. Oh, the same settings. Yeah, just to sync my settings. Okay, that
[66:09] works. And it's interesting. That is interesting. I was thinking it's like maybe a sink or something would help it. I
[66:18] don't think so. I think it if you did like a reload maybe is can you reload from the command palette?
[66:23] Oh, yeah, develop a reload window. Command R. Let's see that work. Yeah. Oh, yeah. Command R worked. Yeah.
[66:40] So that does the thing. Alright, so we've added our theme. The theme is fun. It gives us a little bit more personality into
[66:50] our code. Again, if it doesn't work, you can manually change each of these things. You're still using Menlo font. That's
[66:57] fine. If the fonts okay with you, then it's okay with me. There are other fonts. These fonts you don't install through
[67:07] the extensions, though. Do you do it through the computer itself? Yeah. Okay. And
[67:18] we will see if I can remember how my Google's up. Download dyslexic font. Open dyslexic. Download. Download. I can read
[67:36] this. I mean, there's another one. I don't know if open dyslexic is
[67:42] what you need. Like cool. Open dyslexic to me is a little too too much. Try open dyslexic mono. See that one.
[67:54] I also need to be able to make it readable by other people. So yeah, there is also there's also comic mono. Comic mono is what
[68:14] what it sounds like on the tin. It's Comic Sans, but it is a little it is a little do comic mono, not Comic Sans. So comic
[68:31] mono is actually it is actually easier, apparently for dyslexic folks to read. And there is there you go.
[68:44] Y'all talking about dyslexic, like, I've, in the last two weeks, I started writing like my dreams in the morning and like
[68:53] nightly, like how I've been doing because I have a lot of medical issues going on that I'm like, I need to start tracking
[68:58] all of this. And something that I've realized is I just skip letters. Like I'm like, have I always done this? Like, I'll be
[69:08] like, writing and I just skip the first three letters and I'm like, how am I supposed to know what I meant?
[69:15] So do you see what it looks like on the screen? Yes.
[69:18] That's what it looks like. Yeah. Okay. If you wanted that you would download comic mono. So download that TrueType font,
[69:25] you're going to install that TrueType font. And that is
[69:30] just double click, double click it from there. Okay.
[69:34] It installed it. I'm not used to it being that easy. I'm doing both. So I have the bold too.
[69:43] I did might actually have Yeah, yeah, because it's all that you had both of them in there.
[69:49] Oh, that's isn't that so nice. Okay, so if I were to guess, I would preferences. Maybe keep going. File icon keyboard
[70:06] shortcuts. Why am I skipping it? You did skip it, by the way.
[70:13] Keyboard. Wait, no. I'm just gonna go to settings. Okay.
[70:18] Oh, yay. Now type in. Well, well, yeah, I mean, you can do that. Here's
[70:30] the thing. If it's not installed, if you you have it syncing, right? So if you don't have comic mono on another
[70:37] computer, it's going to wig out because it needs default. That's why there are multiple options. Menlo it like checks for Menlo
[70:44] if Menlo exists, then it gives you Menlo. And you kind of keep going. The other thing is you can actually set different fonts
[70:53] based on a profile. Comic Mono. It's not Comic Sans. Thank you.
[70:59] And also you want it at the front because it's going to check from the front going back.
[71:03] Good call. I don't know what happens if you leave a thing there by itself.
[71:14] Alright, so now go to some go to some code and see what happens. Oh, yo. Open recent. Tweety tag.
[71:26] Oh, you're in that new issue. You got a This is just happiness, y'all.
[71:44] This would have made life so much easier. Like, I can actually see stuff and read it. Yeah.
[71:53] Thank you, Jay. This is amazing. There you go. There's another one that's it's like JetBrains
[72:04] font, but Comic Mono to me is nice. It's soft. It's not. It's not too difficult to read. Some characters. I don't like the
[72:19] I don't like the caps personally, because I think the caps are a little too wide. But again, I don't have dyslexia.
[72:23] So like, if if it helps, if it's what's helpful, then I would just say, Hey, there you go. If not, there are there are other
[72:30] tools that you can check out. But y'all, I'm literally just clicking in random stuff. So I
[72:35] can see how pretty it is. Yeah, we have we have more extensions to go with.
[72:42] Okay, we got more extensions. And Ryan asked. Oh, yes, I did click on something else again.
[72:51] I don't know what Indent Rainbow is. Let's check it out. Indent Rainbow. Every time I hear it,
[72:58] I immediately say reading rainbow, which in my mind goes to the song. Butterfly in the sky. Okay, anyway, Indent Rainbow.
[73:11] And then I'm just going to click it. And oh, it does the dots. Is that what it does?
[73:19] Well, it highlights the dots, the dots will exist, but it'll just show you what level of what it'll show you the indentation
[73:28] levels by putting them in different colors. And you can change the color settings red, white and blue. No, that's
[73:36] that's, that's really bright. But yeah, okay. So that's if you're dealing, especially if you're dealing with code where
[73:43] indentation matters, or you're if you use indentation, something like this is very good, because it'll help you
[73:49] identify where, where you are in the stack in your indentation. It'll also help you find bugs really quickly when you're like,
[73:59] Oh, no, that's supposed to be indented. Why is it not indented? And then you can just indent it.
[74:04] Oh, well, we'll try this one. And what are the other extensions?
[74:10] There's indent guides as well. I don't know what indent guides I don't use either one of these, but I actually I'm probably
[74:16] going to I'm going to download Indent, Indent Rainbow. Yay!
[74:22] Because again, every time I hear it now, I'm going to immediately sing the reading rainbows theme song.
[74:27] So another one that I use is called tab out. Very, very nice. Tab out is nice, but can possibly break your brain. So
[74:38] be careful with this. Have you ever been in like, a bracket, and you need to get out
[74:48] of the bracket and go to the next thing? You can use tab out to do that. And then you just hit tab, and
[74:55] it takes you out of the bracket. Again, if it's something that your brain can can do, very cool
[75:03] because it helps speed up. Like a lot of the moving navigating through your code. But if it breaks your brain, I don't want
[75:16] to break your brain. Well, thank you. Thank you. I mean, it's pretty it's it's
[75:22] pretty resilient. So luckily, I have witnesses to this. So if I get really stuck on it, I've, I feel like either I'll realize I
[75:32] don't know why this isn't working and I'll get frustrated with it and realize it or someone else will, or I'll just
[75:38] really like it. So you have another there's another extension. It's a really
[75:44] important one. It's called add code of conduct. Oh, yay. Yeah, that is a good one.
[75:50] Yep. You should you should totally do that one. Yeah, sadly, you got it. We're not popular enough. You got to actually type
[75:58] the whole thing in to get it. And y'all, this is actually like super, super dope. And the
[76:06] project that Jay was on for last week that Jay homie and sorry, I just flicked myself from my straw because I got excited and
[76:13] my pen hit the straw. Just got water all over me. Um, yes, yes. See, this is what happens is I get really excited about stuff.
[76:22] Um, and it adds a code of conduct. It's really cool. Yeah, it's all I got. Uh, are we using a non relational database for
[76:37] this project? I don't know what this project is. If you're talking about for
[76:42] the community standards project, then no, we're not using any database because no database is required.
[76:50] If if you're on Tweety tag, I mean, I could see I could see a non relational database working. Are you using a database for
[77:00] Tweety tag at all? Yes, we were using um, why am I blanking right now? data MySQL
[77:11] and for relational database. Um, but it was more of just for my experience of it, not for the exact setup. Um, I'm kind of
[77:22] putting Tweety tag on pause because not everybody likes to be tagged in it. But at the same time, I'm like, Okay, maybe I'll
[77:27] stop tagging people. But I mean, that's a good reason to have the application because then you can
[77:34] just say I don't want to be tagged in this anymore. And then yeah.
[77:38] So I'm kind of putting it on pause. But it's like, if somebody needs something to work on when they're on the show,
[77:45] then I got it. And I'm excited to make progress on it. So yes, code of conduct is definitely something Oh, hey, Ryan, because
[77:56] I think you're still here. Can you help me figure out the shortcut to make this a shortcut, please? Because this
[78:05] is something that I would like to tag more often is the community standards because it also in the organization, it has
[78:14] the VS code, add code of conduct, VS code, add code of conduct.
[78:21] So we've got a couple more. And then after that, I kind of got a jet. It's about 1030. Yes. So we've, we've personalized this a
[78:34] lot. But what we haven't done is changed our icon sets. Yeah, go to your icons, go to go to your file explorer there. On the
[78:46] side. See how they're just little logos and little folders and little icons. Yeah, we can we can judge that up a little
[78:56] bit. Let's go into our extensions. And let's do let's do bearded bear. bearded bear is actually a I want to say he's a
[79:06] streamer. Yep, there you go. And do bearded bear icons. Why am I like you're bearded? It's the second one. Okay. He also has a
[79:20] theme. I don't I don't know what the theme is, is like I haven't checked that out. But yeah, let's set those bearded icons.
[79:26] And now let's take a look. Oh, those those are kind of nice. They pop more. I can see stuff better. Exactly. Yay. That's
[79:34] what we do. So and you can also if there's an icon missing, you can just say, hey, there's an icon missing and then create an
[79:42] issue and add it. So yeah, I like bearded icons. There are a few other icons sets. Let me see what I have installed. I have
[79:55] material theme icons, which are okay. Material theme is okay. bearded icons are okay. I have. Well, I think SETI is like the
[80:05] default. And then like VS Code. I don't know SETI icons is not the default. That's a different icon set. SETI's are also kind
[80:14] of pretty, but I feel like not all of them exist. So yeah, bearded icons is kind of cool. And again, more than welcome to
[80:21] come through here and you know, do some digging around. We do yes, Thunder client. Yes. You do a little bit of API stuff. Yeah.
[80:31] So yes, your client is one. I think there's another one that James quick talks about a lot that I haven't. Oh, he's gonna
[80:44] come on the show eventually. I don't know when we have talked about it. And then thank you. Do I? How do I say your name? Is
[80:56] it? API? Nick? Yeah. Your result? Nick is your y'all I'm horrible at names and I need to start googling it like like
[81:11] Laura suggested, but I will install this one. And this is a great call out because we are actually having an API Denver
[81:20] meetup, which I'm a co organizer for tomorrow. Oh, and also, everyone. Next JS. The conference is the next two days.
[81:30] I'm unseen. Come hang out with me. It's online. It's free tickets. Do it.
[81:34] So yeah, the the one that James uses is rapid API. I think there's like stuff involved with that Thunder client is just in
[81:47] VS code, so you don't have to add anything else to it. Thunder clients pretty lightweight, it does add a
[81:52] little thing. So go into the little three dots on the sidebar. And by the way, Nick said that his name is just Nick.
[82:04] Oh, thank you. So let's do a new request. Um, actually, let's, let's do a
[82:12] request for Okay, so yeah, you can just do the the welcome. So if you want to actually just type in a request here to see
[82:20] what output you get, instead of having to write the code, you can just use Thunder client to say like, Oh, if I type this in,
[82:25] what do I get? And then you get the output. This is also good for local testing. So if you build a web application, like a
[82:31] Django app or a flask app, you can save your requests in these in like collections, and then just test, you know, what you
[82:41] want to happen. And you can even have it as a test runner. I would not suggest using it as a test runner, because it's there
[82:50] actually have test runners for that. But if you need a quick test of what's this going to do when I run it, just run it and
[82:56] then type it in here and you're good. And you get the response in here.
[83:02] Yeah, um, I do have to go as well. Are there any that we missed that I need to go install later? Or can I just say, Hey,
[83:12] we need to have Jay back on the show to probably like finish this up. And then we can also talk about, you know, the
[83:17] community standards stuff. Yeah, I'd be happy to come back on at another time. And you
[83:23] know, we can we can talk about it. And I mean, again, there are always new extensions and things like that. If you have
[83:28] new extensions, you can tell me about them. My social media stuff is right here. I'm on Twitter. I'm only on Twitter.
[83:34] I'm also on Twitch, you can follow me on Twitch. I will be streaming again soon. Right now. I've got conferences, like my
[83:43] last conference of the year is like next week. And then I've got like some user group stuff that I'm working on. So once
[83:49] all that's done, I'll be back to streaming again. Yay. Yes. And as y'all know, on the daily, you get rated into
[84:01] a really cool channel, which I actually have, as I'm doing this, coding garden seems really, really cool. So maybe
[84:11] one day they'll be on the show. So if you guys are going to go hang out with them, tell them to come be on the show. They're
[84:17] also in Denver. So I told them to come to the API Denver meetup. So come hang out with us again. We will let you know when Jay
[84:26] will be back on the show after conferences, and go enjoy coding garden. So thank you, everyone. Bye.
[84:35] Adios! 
