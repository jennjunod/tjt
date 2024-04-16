---
showLink: "https://www.youtube.com/watch?v=GP0Rw_fnQkI"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-python-basics-with-guest-laura-langdon"
title: "Teach Jenn Python Basics with guest Laura Langdon"
publishDate: "2022-09-12"
coverImage: "https://i.ytimg.com/vi/GP0Rw_fnQkI/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome back to Teach Gen Tech. Another episode about Python, which I am excited, except I did a hard reset last week on my laptop because
[00:15] it was being super goofy. So we get, you know, Laura gets to deal with new extra things that we get to set up today. And Laura, please introduce yourself.
[00:27] >> Hello, I am Laura. I am a technical writer at Suborbital Software Systems. And I before that was thinking I was going to be a data scientist. And so I did a bunch of learning
[00:37] of Python. And so here we are to teach some Python. Before that, I was also a math professor. And so the teaching and the Python are sort of my comfort zone anyway. So it's nice to
[00:48] spend some time in here. >> Yes. And for all of those that are just checking out this episode, you'll be able to find if you're curious about Python, you
[00:58] will be able to find a playlist on YouTube of Laura's and my adventures with Python. In the fact that once I get that set up, they're all there. I just need to make a playlist.
[01:14] As y'all can probably tell, I have been a bit batty lately. And that's okay. Because that's what happens when life goes on. So I am putting we are still going with automate
[01:26] the boring stuff with Python. So that I have that in the chat, as well as we since I decided that it'd be really cool to delete everything without realizing that I deleted everything.
[01:42] It's like, I did, but I didn't realize that I didn't back up certain things. We're also going to set everything up on VS code instead. >> Yeah, which we were going to do at some
[01:53] point anyway. So this is a feature and not a bug. >> Yes. Ooh. I like that. I need to start saying things like that. Because that does
[02:05] sit home. >> I say it so much that, like, my children say it. >> That is like happiness right there. So when
[02:18] they don't do something, like clean their room, are they like, it's a feature, not a bug? >> Mostly not to like that extent. Mostly
[02:28] it's not like in a cheeky way. >> That's what I would do to my parents. I feel like they're lucky that I'm also very mischievous. So I would have found it hilarious.
[02:44] All right. So we need to, in this article, install Python. >> And so we found this by just searching for Python VS code, I think. Is that right?
[03:01] Read through. Okay. Quick install. Use Python.org and install the extension. Oh, yep. We still have to install Python. So all right. This is where I --
[03:15] >> Do that big yellow one up at the top. >> Oh. >> It just takes an extra pair of eyes sometimes, I find. You know how, like, when something's
[03:28] not working, you know, and you ask somebody for help and they come over and then they're like, oh, it's this thing. And you're like, oh, okay, right. I swear I have a brain. But
[03:39] anyway. >> Yeah. That was -- so y'all, just so you know, what I was doing earlier and got stuck on is I was scrolling down. It made it way
[03:49] more complicated. All right. So I am going to click on this, I'm guessing. >> Let's run back to the tutorial and make sure that there's not some kind of weird --
[04:01] >> For quick install, use Python and install the extension. Okay. So continue, continue. I feel like this is so much easier than some of the other languages I've installed.
[04:13] >> Really? >> Maybe. I think so. I think because I normally do them from, like, our first session that we talked about, I was doing them through
[04:27] Terminal and, like, npm install instead of, you know, pip install. There we go. And what up, homie? Glad to see you today. >> And look, there's our friend, Idle.
[04:41] >> Yes. Yes. The Idle. Okay. We can -- I don't know what we're doing here. So I have to install Idle, right? >> Let's just -- let's look back at the installer.
[04:53] So it's installing. It's done. Okay. And we can close. Cool. Okay. And then let's just proceed directly to the plug-in for VS Code. We're just going to follow the instructions
[05:07] exactly as they're written. >> I'm glad you're here because I'm not the best at doing that. I like to try to figure it out. If I figure it out, great. If I don't
[05:17] figure it out, then I'll go back and read it. >> I literally write the docs. It's my job. >> Well. It's definitely something I need
[05:32] to, you know, work on doing. So, okay. We -- for quick install, use Python and install extension from the VS Code Marketplace. I'm going to open that in a new tab. All right.
[06:00] And install. And I still don't have anything, like, prettier or anything like that. So if we need them, I get to go install them. >> Sure.
[06:19] >> All right. Sweet. >> What does that switch to? What does that want to do? >> Switch to pre-release version of this extension.
[06:32] >> No. >> No. I don't need bugs or features. I need to learn. All right. So, once you've installed it, activate using the Python select interpreter
[06:44] command. How do I know if it automatically did it or not? >> Okay. So, let's see. Python select interpreter command. Okay. So, let's look around at the
[07:08] options in your menu in VS Code. Like, if we close this extension -- oh, wait. That's okay. >> Oh. Jupiter.
[07:21] >> Oh, you already have Jupiter. >> Installed. >> Oh, maybe it came with Python. No, because they're listed separately. That's interesting.
[07:32] You have all this stuff. >> I have all this stuff that I didn't -- well, maybe it came with the extension. >> Maybe. They're listed as separate extensions,
[07:39] so that would be kind of interesting. Okay. So, yeah. Because I haven't done it -- so, for context for anybody who hasn't been with us the last couple episodes and is like, I
[07:58] thought you said you write Python. Why can't you do this? I used a different IDE. I used one that's specifically for Python called PyCharm from JetBrains. So, I haven't actually
[08:08] done this in VS Code before. So, this is a learning experience for both of us. >> And then the last couple times that we did it, it was we did it in Mew, which was
[08:19] a different editor. So, we're now doing it in VS Code, which I'm kind of excited because I use VS Code for JavaScript. >> Yeah, yeah. Getting you back in your comfort
[08:31] zone. I love it. So, okay. So, let's try looking at -- I just tried to click on the settings cog on your screen. >> Nice. Nice. Well, you know, I will go
[08:42] there. >> So, let's look at settings. Do we have like an extensions setting? Okay. And let's look at the Python one.
[08:58] >> Got Jupyter one. >> Yeah. I think, yeah. Let's do Python. Okay. And then there was a cog. So, okay. Is there an extensions -- oh, is that -- is there an
[09:15] separate extensions button in VS Code? I think maybe it's up a bit. Is it the squiggly one or is that branching? >> This one?
[09:25] >> That's branching. Okay. So, what about the boxes? The one with the like box -- >> That's how this came up. >> Great. Okay. Yay. Okay. So, let's look
[09:35] at Python in this view. And let's click that little cog and see if that gives us -- oh. Really? Extension settings? Because what I'm wondering is -- oh, default interpreter path.
[09:53] We found it. Scroll down. Okay. So, that doesn't look like -- it doesn't look like a path because it just says -- it's just one word. Right? But maybe it's secretly a path. Like it can
[10:20] just use that word, like VS Code can use this word Python to use it as a path. So, let's go back to the tutorial instructions for VS Code and see -- oh, sorry. In the -- yeah.
[10:34] There you go. Oh, wait. >> I just went to setting descriptions to see what it would say for this link. Python.Python path setting is no longer used by Python extension.
[10:47] >> Okay. Python.default interpreter path. So, I think that is what we just saw. Because what we were looking at was the heading was default interpreter path. And the word that
[10:58] was in that box was Python. So, I think that's -- that is what we just had. So, I think we're good. >> Groovy.
[11:04] >> But let's go back to that, yeah, Python in Visual Studio Code and make sure -- okay. Let's just try running something and find out whether we're good.
[11:14] >> Okay. So, run Python code using file explorer. So, I'll just open a new file and named it -- okay. Just making sure. I guess I'll open a folder. Code. Open. And I want a new file
[11:41] and I'm going to -- what am I calling it? I need to put these next to each other. Oh, by the way. So, I just learned something super, super nifty that I should probably bring up
[11:54] on screen. Which for all streamers out there, I thought this was really cool. It's definitely not like the really fancy setup that other people have. But I still thought it was cool.
[12:08] Let me do this one up here. There we go. And then let's see if I remember. Yes. So, if anybody does want to talk to us, other than Homie. Homie's still here. I'm not going to
[12:33] miss it because I'm not looking down at my other screen. I'll just show up here. Like, this is fantastic. And we'll just go like this. Cool. All right. So, I need to scroll
[12:45] down. Oh, scroll up. And I need to get a new file and call it hello.py. And then print. Okay. So, I think -- yeah. So, when you open up a new method, like print, it's going to
[13:17] show you off to the right. But it looked like it was on top of it just because it's so tiny. Yeah. It shows you like the documentation for that method. Which is super helpful. Except
[13:30] if what you're looking at is quite tiny, then it's like in your way. Got it. Yes, Homie. It is fancy. And I believe I can do it.
[13:45] Yay! It worked. It worked. I don't exactly know how I did that. But in a previous stream, I could see
[13:58] it live right here. So, if I made an edit and it was in VS Code that it was doing that, it was really cool. I just don't remember how to do it.
[14:11] Yeah. So, well, I'm not sure what that would look like in a Python context. I know what it would look like for Markdown. Like, Markdown where you're just editing files. Then you
[14:26] can do like a live preview and it'll show you what your file would look like. Maybe it was that.
[14:29] In a Python context, I don't know what that would be. Because there's nothing to display other than what it literally did display at the bottom down there.
[14:39] Yeah. Because you said print hello, beautiful human, and that is precisely what it did.
[14:45] Yes. But it's not like a web page or something where there's something to look at.
[14:51] Yeah. Yeah. And so, I think there's no preview because it would be like, well, what would you want
[14:57] that to look like? Yeah. All right. So, I'm in the right folder. Now I have to I'm going to Google this because
[15:08] I keep asking people and maybe this is why it's not sticking, but I have to download our old file. So, from GitHub, download my repo so we can use it. Right?
[15:21] Yeah. Oh, okay. Gotcha.
[15:23] So, I'm going to, and I'm doing this because I feel like I keep asking people and I've written it down, but it's not clicking. Download, get.
[15:31] Okay. So, don't use the word download. Okay.
[15:38] Clone. And I should probably see in CLI. On GitHub, files download.
[16:03] That's the one. Oh, there. Down a bit. Down a bit. Big green button. Yes.
[16:09] That's your friend. Okay. So, I need to go find it in my actual file. Got it.
[16:16] Actual repo. Yeah. Actual repo. Thank you.
[16:19] Sorry. I'm totally not trying to be pedantic, but just in terms of like, knowing the search terms and so on, it's helpful.
[16:28] Yes. I agree. I completely agree. So, I need to copy this. Right? Okay. And then, oh, wait. This does it even, all of it.
[16:42] That's in the GitHub CLI. Not in CLI on my computer.
[16:48] It could be if you install the GitHub CLI, but you can actually just, if you go back to the HTTPS one.
[16:56] Okay. Copy that.
[16:58] Yep. Okay. Go to your terminal. What word do you think you need to type first if we're talking
[17:05] to... Git clone?
[17:08] You got it. That's it. That's exactly it. You totally got it. Okay.
[17:13] And you're good. You did it. Okay. And then, if I want to open it, I need to do CD learning Python.
[17:21] Mm-hmm. Okay.
[17:23] Thank you for helping me because I'm like, I feel like I've done it enough and then code. We're going to see if it works now that I did the hard reset.
[17:36] It actually works! Yay!
[17:39] That was when, you know, you've been there since the beginning, Laura, of when it wasn't working.
[17:45] So... Oh, that's right. That's when we met.
[17:49] Yeah. And it's still, like, no matter what I did, it would not work. Now that I've done the hard reset, it worked. It's magic.
[17:56] Hooray. All right. So, I know that we are behind because... Well, I decided that it would be cool...
[18:05] Because this was a thing that we were going to do anyway. Yeah. But if I'm... And I'm kind of sad because Wesley was also hanging out with us and showed
[18:18] the... Is it called an F line? F string?
[18:22] F string. F string. Okay. He showed us the F string and I thought it was, like, the coolest thing ever created. Because we're on chapter 1. And this is probably really small for everybody
[18:32] because it's small for me, too. It looks good to me.
[18:36] Sweet. And then... Yep. We did the 2+2, clearly. We got this in VS Code. Yep.
[18:44] And I'm going to close this. So, we can move it a smidge more. Errors are our friends. Yep. Okay. Let's see. Let's see if I remember what these are. Exponent is, like, 2 cubed.
[19:07] That's right. 2 to whatever power.
[19:10] That's it. Okay. Remainder or modulus is... 8 can go into 22. Wait, wait, wait. No matter how many times
[19:22] 8 goes into 22, there's 6 left over. Yeah. And the next one down is the number of times that 8 can go into 22.
[19:33] Yeah. Sweet. The number of whole times. Yeah.
[19:37] Yeah. Yeah. I'm still thinking Lagos. Like, that is how... I'm so glad.
[19:42] Yeah. Lagos is helping. All right. So, we were doing different commands. Oh, yeah. For sure. Ta-da! Thank you, homie, for reminding me because this is, like, what I need in my
[20:00] life is when I'm not remembering things like that. So, we went through all... Order of operations.
[20:10] All order of operations. Hey, Jay, we were just talking about you. Hey!
[20:16] We're using VS Code now. Because I deleted what we were working on last time. Yep.
[20:22] Okay. Ooh. I kind of remember this. Integers... Numbers without decimals.
[20:37] Yeah. That was the only part, right? It was number without decimals, numbers with decimals, and then, like, words in a string.
[20:44] Strings. Or numbers or words in a string.
[20:46] So, any characters that you have strung together. Yeah. Because we were doing, like, Jay Bakari or something like that when I was trying to...
[20:58] That's right. Oh, yep.
[21:00] Doing string concatenation. Yep. All right. We got this far. And Jay, I totally ended up deleting my F string because
[21:10] I did a hard reset on my computer. So, I'm a little sad I didn't back it up first. But now I know.
[21:17] That's okay. Now I know.
[21:19] We'll be doing more F strings in the book. Don't know why. F strings are so exciting. But they are.
[21:25] They are very cool. All right. So, this is, I think, where we landed.
[21:32] Oh, we got way past this. We got way past this?
[21:35] Way past. Oh, yeah. Because we were telling them what they equaled.
[21:40] Mm-hmm. So, I could say spam plus cheese equals goodbye, hello.
[21:49] Mm-hmm. Okay. I feel like this... We looked at this and it was, like, the same for most coding
[22:05] languages? Yep.
[22:07] Okay. Yep.
[22:09] Oh, yeah. We did build our first... Oh, yeah! We did.
[22:13] Okay. I kind of want to build this again because we figured out how to change it. Mm-hmm.
[22:20] And I was really excited about this. So, now I'm going to see if I can... Yeah, I don't want... Do I want that version? No, I want this version. Okay.
[22:30] Do you want to try writing it without looking at it? Okay. I do. I just want to look at it one more time before...
[22:42] Sure. Input... What is your name? That's right. The imprint. Okay. We're gonna try this. We're
[23:01] gonna scroll. Mm-hmm.
[23:03] That's good. All right. At least the output will remind me. Can I look at the output? I feel like I can...
[23:10] Sure. Yeah. I think that's actually a really great way to learn. It's looking at, like, what do we want to get? And then figuring out how do we get it is totally solid.
[23:20] All right. So, we want print name. What is your name? And then we were doing comment of input of name. And then...
[23:43] Okay. Strictly speaking, is print an input or an output? It's both, right? Because they're gonna input it and then use the output of the name to
[24:02] say... And that just matters because in terms of keeping it straight in our heads, like, what
[24:18] we have done so far and what we still need to do, it just is sort of helpful. Okay.
[24:26] Also, I think it's pretty common practice to put the comments in after you're, like, mostly done. Because otherwise, at least for me, I would end up going back and, like, changing
[24:42] the comments because I'd be like, "Oh, no. I need to change this thing and, like, move it over there or whatever."
[24:46] Yeah. I probably would do the same. And so I'd put the comments in after.
[24:48] Yeah. I would probably do the same. Okay. So now I need my input. It'll be a function. So input is totally good. You'll need some parentheses. Because it needs
[25:19] to take what we call an argument. And yes. Needs to be name. But is it gonna object? What happens if you click outside of the parentheses? I'm curious to see whether it's gonna let
[25:35] you know that you have an issue. Oh, it's not. Okay. There is a problem with name. What is it?
[25:45] Do you think? It's not in parentheses?
[25:48] It is in parentheses. Oh, no. Sorry. It's not. Like, the text is perfect. You know what? Let's just keep going
[26:00] and see what it says when we run it. Okay.
[26:03] Yep. Because learning from the like trying to run it and then have it go... There we go.
[26:17] So it's saying built in function name. And so it's not happy. Because we're trying to use name as a variable. But we didn't declare a variable called name.
[26:28] Okay. Now I'm scrolling back up. Because I'm like... I don't even... Oh! So it's backwards. I just got it backwards. One more time. Because it's... Okay. So what's happening here in
[27:00] line 7? What do you think is happening? I'm telling my name to be a variable.
[27:07] Yep. And what are you assigning as a value for my name? Anything. Because it's open brackets.
[27:18] Yep. And in particular, what is it going to end up... I'm trying to figure out how to ask this question in a way that isn't goofy. How is it going to know what to put in my
[27:37] name? Is 100% possible that I'm not asking this question very well? No. So like how is it gonna know that I'm gonna write my name and then put out my name
[27:46] right here? You're gonna write it. Right? Yeah. So it's... What this is saying, line 7, is like... Okay.
[27:51] We have a variable my name. We haven't given you a value for my name yet. Because the user's going to give you that value.
[27:59] Right. So it's like... Hang tight. It's coming. The value for my name.
[28:05] Again, I'm gonna be print my name. Okay. I'm gonna... Yeah. No. It... Hang on. It's... Do you have two copies of this file open? Is that what we're looking at?
[28:47] Maybe because of this. Oh. Because it should be where... There. So I think if you just close... I think you have two sort of instances of this file open.
[28:59] Okay. And so when you clicked on the first one, it didn't do it right.
[29:03] So I can just hit play right there. Okay. Cool. Yeah. Yeah. You only need one.
[29:07] All right. Cool. So it said my name. And then... I want... Print. I want... I don't know. Okay. Let me try this. Let me try this.
[29:55] Yes. Yes. Yes. I'm sorry. I'm trying to do it like what we were doing last time. But I'm trying to do it off of
[30:01] memory. So... And then I need another input. Your age equals input. And then... Parent. You were born in... And this is where I know it's gonna get goofy, because I don't remember
[30:33] what it was. But it's, like... The year minus... Forever. Play. Okay. So we got some errors. And that's totally cool. Because we're just gonna figure
[30:54] it out. So let's look at the first error that it's identifying. Line 12. Oh.
[31:09] Yep. But I... Oh, wait. I only need singles. I don't know why I keep putting singles. It's actually fine for either one.
[31:21] Oh. Okay. It'll take this.
[31:23] And then... I want... I also want this. Print... I don't need that in. Okay. What's your name? Ah! Oh, but I didn't print the year.
[31:59] Okay. So let's see what's going on. So you've got... Right. 2022. Okay. So what might have happened? So we've got your age equals input. And then prior to that, you've said the year
[32:23] equals input 2022. So input is what we use when we want to get user input for something. Oh. So I just need to do...
[32:46] There you go. So let's, for the moment, comment... Oh, okay. Yeah. We'll get there. We'll get there. We're
[33:00] going to just take it one error at a time. Oh, I also need to say, "What is your age?"
[33:09] Okay. Well, we're getting closer. We are getting closer. And this is the best way for humans to learn is by making mistakes
[33:23] and then figuring them out instead of me telling you, "Okay. Now you need to do this. And then you need to do that."
[33:31] Okay. So let me also save these things, because I keep forgetting to save. All right. So lovely to meet you, new friend. Can I do it, like, on the same line? Or this is where you would
[33:48] need an F function? You can do it in two different ways. You can do it with string concatenation, where you're
[33:55], like, literally using, like, the plus symbol to add strings together. Or you can do it with F strings. But it would be all inside the same print statement. Sorry.
[34:10] Where did you go? Come back. We're still here. We're hanging out.
[34:22] Where is it? Oh, that's interesting. It, like, became full screen. And then I couldn't find you, because you were in, like, a different -- because Mac OS is weird that way. And so
[34:37] -- Oh, other than not having a space, eh?
[34:43] Uh-huh. Oh, wait.
[34:47] So why -- so right now it's saying, "Lovely to meet you, new friend, Jen." But it didn't say -- oh, no, sorry. Never mind. Go ahead. You don't actually need the parentheses on
[35:01] my name. But it's not tripping over them. It's not, like, an error. But they don't need to be there around my name in that print statement.
[35:13] But -- oh, okay. Okay. Okay. Yeah. Not hurting anything. But in terms of, like, readability later, it would be, like,
[35:29] wait, why are there parentheses around that? Is that supposed to be, like, an argument to a function and the function's missing? Yeah.
[35:35] Okay. And then going off of what you were saying, but also age equals input -- Yeah.
[35:42] -- into input? Let's not look at the solution manual yet. Let's just keep working at it, like --
[35:48] Okay. I'm putting it just as, like, separating them out so I can see answers. Absolutely. Yep.
[35:55] Okay. So, your age is input. And then I want to say print. And then if I were to do this to match --
[36:17] I'm going to need my plus sign. Plus sign. All right. Let's give that a save and run it
[36:25] and see how close we are to where we want to be. My name is -- click down here. My name is Jen. I am 34.
[36:39] Okay. So, got to awesome. You are 34. Yep.
[36:44] Cool. Yep.
[36:46] And then my last thing is not great. Okay. So, what it's doing is it's just printing exactly the string that you gave it.
[37:00] Mm-hmm. Right? And so, but what you wanted it to do was to --
[37:06] Line 18. Oh, I forgot my plus sign. Yeah.
[37:31] I forgot the minus -- or the commas or semicolons. My name is -- not there. My name goes down here. Jen. I am 34.
[37:48] Okay. And so, this is exactly what Jay was identifying would become a problem. That it's saying, "Hey, you can't concatenate. You can't stick an integer on a string. You can only
[38:02] stick a string to a string." So, it's not happy because concatenate, that's the plussing. That is just a really weird word to use, but okay. Okay.
[38:16] Yep. That's the plussing. And so, because when you got the input, the input is always going to be a string. So, when you said, "What is your age?" and your age equals input, that
[38:31] was 34. And that's why it worked in line 16. It said, "Awesome. You are plus your age." Your age was a string because if your age were a number, it would have been like, "Hey,
[38:45] I can't add a string to a number. That doesn't make sense to me." But your age was already a string. And so, it was fine. But then in line 18, it becomes a problem because it's
[38:57] not an integer or it is a string. And so, what you have to do is cast it as an integer. And that's that int input. So, you say or not, sorry, input. But like around your age
[39:14] in line 18, you put int and then in parens, your age. And you'll need one extra parens on the end. And so, that's a function which means take this string and make it an integer.
[39:34] This string that is a number. It wouldn't work if it were like the letter A or something. Did you save? >> I did. But I'm wondering if it's like
[39:46] I have to do the same thing with year. So, if it's >> Shouldn't need to. Because if you look at line 10. So, oh, oh, look at what else we're doing. We're still trying to do
[40:17] that thing. We're saying you were born in plus integer. So, we're still trying to act like it's an integer. Like we're concatenating these. And so, that won't work. And so, we'll
[40:31] need to do let's see. We can do this with left strings. And we can do it without. So, let's take out the plus. And let's just run it again. I'm trying to remember how this
[40:48] I haven't done this thing in a bit. So, okay. So, it's not like in that. Yeah. I think we probably need to just use f strings for this. >> And this is the problem is I deleted my
[41:03] f strings because I didn't save that one. >> Totally. This is kind of a feature instead of a bug as well. Because exactly. It's this. F string in Python. This is my students when
[41:24] I was a math professor, I would tell them, you know, it can be kind of frustrating. Because you know that idiom, if you teach a man to fish, he can eat for a day. Or no, if you
[41:35] give a man a fish, he can eat for a day. If you teach a man to fish, he can eat for life. And I would tell them, I'm never going to give you a fish. I'm going to teach you to
[41:43] fish every single time. Or if you're starving, I'll give you a fish and then teach you to fish. But like, you know, and so, I'm almost never just going to tell you just type this
[41:53] and then type that. It'll pretty much always be let's figure out how to find the information that we need. Just like this. >> I like that it's here at least. So that
[42:05] way I totally used what Jay said. But I could at least know I could find it. >> You can find it again, right? Without having to watch this live stream.
[42:17] >> Which has happened before. I have had to. When I hit play, I just expect to start typing down here. No, you still don't like me. >> So we don't have all of the components
[42:35] for an FString yet. Let's go back to that tab with the FString documentation. Okay. So looking at their example. So we say we have like F yeah. We have our string. And
[43:16] we need a variable name in there. So would it be yeah. So okay. Let's put back the int and parens around your age because we're still going to need that to not be a string in line
[43:46] 20. If we do it in line 13, we're going to have the same problem in line 16 where we're concatenating an integer and a string. The int and parens would need to go around your
[44:02] age. Actually, wait. Is it treating the year as it should be treating the year as an integer. Because if we look at line 10, we just declared the year is 2022. There we go.
[44:14] >> No, it still doesn't like me. >> We're going to get there. So scroll down in your tab on FStrings. >> Oh, I got to also get rid of the space.
[44:41] Oh, it was a space. Space is 34. I was born in 1988. We got it. Did it. That only took like 45 minutes to figure out. That's it. >> But you learned to fish. Right?
[44:58] >> Yes. Yes. >> You learned to fish. >> And I do think I will say this has been kind of fun with Python learning this kind
[45:08] of stuff, too. Because I like being able to learn both in different ways. We've talked about that before. But I'm learning Python from the ground up. And JavaScript, I kind
[45:23] of feel like I'm learning how to fly the plane while I'm flying it. So it's a great experience being able to do the balancing the two. >> Exactly. Yep.
[45:34] >> Okay. So now I'm going to hit save. And we are going to oh, oh. Jay said, ah, can't keep it up on the screen. There we go. I like that Laura teaches the fishing. I like to
[45:53] show then explain mostly to avoid the foils and troubleshooting. Python has a saying there should generally be only one way to do a thing. This is almost never true. I think we talked
[46:05] about that when we talked about using camel casing. Because like it's not like the Python way. But a lot of people do use camel casing. >> Right. Just because here I am going to
[46:22] be just a pedant. Because I think you're probably going to put this on in the GitHub repo. >> I'm totally going to do that next. >> If you scroll down, look at your last line.
[46:33] >> Yes. >> It says you were born in and 1988. >> Oh, oops. That's a good call. >> Just because otherwise it looks like something's
[46:43] missing. So, this is actually a different way of doing F strings than I have seen before. The way that I've seen before is the same way that Jay was talking about last time where
[47:09] you're actually using like a percent sign, the modulo looking operator. Which might just be further down in this. And so, this is another example of where it turns out there's more
[47:20] than one way to do F strings. You know what? We're going to get there in the book as well. >> Cool. Cool. >> And this is working.
[47:32] >> All right. Then I am going to see if I can use this terminal to upload. Let's see. I have to think about this. Get info? No. Get status. I just wanted to see if I could
[47:57] do it. It was modified. So, I want to add this to the current one. So, I think it would be get add. All right. >> And then you either need to specify a file.
[48:13] Like in this case, it would be Laura's cool.py. Or if what you want to do is add everything that you have just changed, then you can do that get add dot like you just did. That can
[48:25] be dangerous is too strong a word. But it can be something sub dangerous. Because you can end up adding files. If you just get into muscle memory habit of get add space dot,
[48:40] it's going to add everything. And sometimes you don't want it to add everything. And so, no, you're all good. You're all good. So, what this is saying is, please enter a commit
[48:50] message. >> Oh, yeah, yeah, yeah. >> Yep. Okay. And so, this is going to be doing it using Vim. Have you used Vim before?
[49:08] >> I've heard of it. I've heard it's not used very often anymore. Or something. I don't know. I don't know. I feel like I know. >> Okay. So, the bits of Vim that pretty much
[49:29] everybody needs to know, even if they're not planning on using Vim in their in most cases, is this much Vim. So, we're about to learn the like little base Vim, a few things. Okay.
[49:44] So, in order to edit using Vim, the you know how on keyboards, especially older ones, there will be a button that says insert? >> Yes.
[49:57] >> Yep. Okay. So, you want to insert text. And so, the Vim command for insert is I. And now you can type. You can type your message. >> Oh, but enter text.
[50:32] >> Oh, but enter didn't work. >> That's right. Because we're still in Vim. Okay. So, Vim has two different modes. One is editing mode. And the other is command
[50:48] mode. So, remember how we had to press I, the I command, in order to insert text? We need to get back into command mode. And you do that by pressing escape. Okay. And now
[51:07] the commands that we want to run, one thing that we want to do is we want to write this, which is like saving. We want to write this to the file. And we want to be done with this
[51:18] file. We want to quit. So, when we want to issue a command that's not like insert, we have to type a colon. Okay. And then the two things that we want to do are we want to write
[51:35] and quit. So, we're going to type W and Q. >> Together or space? >> Enter. We did it. We Vim-ed. There should be a badge.
[51:57] >> I don't know if I like Vim-ing. >> Yeah. I mean, it's a thing, right? Where like it feels like, why are you doing this to me? At least that's sort of how I felt
[52:07] about it. Yeah. So, my dad, because I grew up in nerd house, right? My dad says, used to say, I guess, about one of these. There are two things that you can get by life. You
[52:23] can almost get through life without knowing two things. One is how to drive a stick shift. And the other is VI. Vim is VI improved. That's where the M comes from. So, it ends up being
[52:36] super powerful. And I'm currently expanding my Vim knowledge because I'm starting to realize how incredibly powerful it is. It just feels like there's a learning curve. For sure, there
[52:53] is a learning curve. >> I feel like based on your dad's saying, I'm halfway there because I know how to drive stick shift.
[53:03] >> You are totally halfway there. You're ahead of me. >> So, we're getting there. Just, bleh. And thank you for the words of encouragement,
[53:12] homie and Jay. >> I actually mostly can't see them because I think they're underneath the browser. >> Oh, yeah, yeah, yeah. Here you go. I don't
[53:23] know how to get rid of this thing. No, I don't. I don't know. How do you get rid of it? I'm not sure. Yeah, maybe that'll get rid of it.
[53:36] >> If you look at that, yeah. >> There we go. Well, no, it's just still there. It just makes it bigger. >> Yeah, probably. Oh, Jay, is that NeoVim?
[53:47] I've seen NeoVim, but I haven't actually used it. Oh, and thank you. It means a lot coming from you about good teaching because I listen to your podcast, Jay, by the way. Sorry. It
[54:05] always feels stalkery to be talking to somebody that you've never met and be like, oh, I listen to your whatever. It feels weird. >> I met Jay without like I met people that
[54:20] knew Jay from Elastic and were telling me about him when I already had a meeting with him, not knowing that he was who they were telling me about.
[54:30] >> Oh, that's funny. >> And it was very weird because like halfway through the conversation, I was like, what? I know of you. Whoa.
[54:42] >> There's a super awesome game for learning Vim. I am working through it myself right now. It's called Vim Adventures. It might be like vim-adventures.com. I'm going to have
[55:04] to check out NeoVim. Okay. So where were we? >> I'm just trying to see if I could look at the Vim ones that we used because I think they're gone, though. So it was an input command.
[55:26] Well, it's command input and edit. >> Those are the two that you need to know. Yeah, I would have said that Vim has three modes as well, but I would have said it's
[55:43] command insert, which is also called no, command is also called normal mode. Insert is always called insert mode. And the third one that I know of is called visual mode. I would have
[55:58] thought of edit mode and thingy and insert mode as being the same thing. Or no, I mean, I guess edit and visual are kind of the same thing too. Yeah. Anyway, so what you have
[56:16] to know, anytime you find yourself in a Vim situation, the most important thing to know is how to get out. >> Yes. I think I've gotten stuck in it before.
[56:28] >> Right. And so the way to get out without accidentally saving anything or whatever is colon, Q, exclamation point. The colon is always there because if you're going to issue
[56:46] a command, you have to have the command colon. And then the Q is for quit. The exclamation point means quit, even though it's equivalent to exit without saving. It's like just quit.
[57:09] Even if I've made changes, don't be like, "Ah, you made changes. Do you want to save them or whatever?" Just get out, get out, get out. Colon, Q, exclamation point is just
[57:21] get me out of here. But what we did, we wanted to save. And so that was colon, right, right? >> Oh, W-S. Right, save. Oh, right was the save. So right, Q is, okay, right is save.
[57:49] I'm totally taking notes on a notepad, old school. And Q is quit. Okay. And then that helps for quit, quit without saving, right? Okay.
[58:01] >> In fact, it's super cute. Have you ever heard of Obsidian? It's kind of like Notion for like notes and stuff. >> No.
[58:11] >> Okay. That's super awesome. That's a whole other like podcast or stream. In fact, Nicole Vanderhoeven on YouTube does great streams for it. Anyway, if you want to enable the
[58:25] Vim plugin for it, it won't let you do it until it'll say, "We'll do this once you type in, how do you leave Vim?" And so you have to type in colon Q exclamation point, or it
[58:43] won't let you use Vim. And I just thought that was so clever. >> That is really smart because knowing me, I would get stuck in it and just be like cut
[58:51] my losses and close terminal. I've done that. I don't remember why I've done that, but I've done that. >> Oh, yeah. And Jay is saying that VS Code
[59:01] has a Vim mode extension. I literally use Vim in VS Code. >> I was going to say though, I don't know if I remember who Julia is. And Jay, can you
[59:12] give an introduction? Because you also said that you knew our friend here. What's his name? I don't remember his name. >> Al Swaggart.
[59:23] >> Al Swaggart. So I'm going to be hitting you up for some introductions and for... You got to still be on the show, Jay, because... Oh, no. Who's gone? Oh, okay. Julia, you're
[59:37] Laura. Laura, you're Julia. You're the same, same. Same, same. >> Oh, okay. Cool. >> So this next one.
[59:47] >> Oh, Jay says Al did catch our last stream. That's exciting. >> Really? Yay. What did he think? >> So, okay. So we were in your terminal in
[60:05] VS Code. We added the file. So we were like, okay, let's get this ready to go. And then we submitted it. Yes. >> What do we need to do next?
[60:32] >> I don't know. Push. >> Oh. Is it git push space dash M and then you put more comments? >> That's actually git commit. So there are
[60:46] two different ways, well, at least two, two that I know of, ways to write a commit message. So you can write git commit dash M and then you write your commit message. Or if you just
[60:57] say git commit, enter, then it'll pop you into that Vim window that we were in where you wrote your commit message. >> That's how I, okay.
[61:07] >> Yeah. So then, yeah, so those are two different ways of doing commit messages. >> That's where I was like. >> Ramon taught me the second one, the one
[61:21] with Vim instead of the dash M message thing. Okay. And so we can just git push. >> Okay. I'll do that in a second. Because Jay said that he's in Georgia right now. So
[61:39] he has oh, you're speaking on Thursday. Yay. Al said he was glad to see someone not familiar with Python doing a live stream with it because it helped him learn some new context about
[61:51] how to be clearer in updates. And Jay, I mean, if Al wants to be on our show, he is more than welcome to be on the show. He could join me and Laura. We'll do it together on a Monday.
[62:08] And then I do want to say just as we are speaking about Ramon and Jay's here, we are finishing up our discussion from last weekend, or last Wednesday, about one version of the way I
[62:26] was saying it for my CFPs was a develop Cato's guide to saying fuck it. But I will put this in the comments as well. It actually led me to writing a blog post to work on finding
[62:43] my voice on all of this. And we are finishing it up on Wednesday, same time, to do to learn how to actually submit CFPs. So we kind of like we really worked hard on like, you know,
[62:59] all the pieces about it. But now we need to finish the description and actually go apply places. Nice. So, but yes, get push. I am remembering a promise. I'll go back around
[63:14] to it. Yeah, you're all good. Oh, okay. So GitHub is protecting you because you wouldn't want anybody to just clone your repo, and then push to it as you. That would be bad.
[63:39] Yay. Yep. Thanks for coming, Jay. Thank you, Jay. See you later. Um, yeah, I totally want to like watch that stream later too. Hopefully I can catch some of it. Hey, other than getting
[63:58] myself very confused with Git commit without the dash M, I'm feeling pretty confident about this one. Yeah. Do you want to see it in your repo? Yeah. Link to stream for, uh, the previous
[64:16] one we did or the one on Wednesday? Um, homie. I wonder. Oh, I was interpreting it as for Jay's charity stream. Yeah. Okay. So I got that one on Twitter. I actually have his Twitter
[64:30] up. So let me copy the Twitter link. He, he, you should definitely follow Jay on Twitter anyway. And that is the status about with it to the link and everything like that. So
[64:50] definitely follow. And then, all right, we are going to GitHub over here and we're going to refresh. And Hey, we actually did it 16 minutes ago. And it's there. Yay. Okay. And
[65:16] then, okay, cool. I need to update the readme. These are old notes. I still have the notes from last time, but I definitely need to update notes. And I feel like this is definitely,
[65:36] it was harder than I thought, than it was going to be doing that by without using it as a cheat sheet. Using the, um, documentation as a cheat sheet. Right. Yeah. And that's
[65:51] another thing that I always used to, used to tell my students is because they, um, sometimes they would find it frustrating that in our classes, I would have them do a lot of group
[66:02] work. Like I would show them like an example of something and then have them do it themselves. And they would be like, no, because I learned better just by watching you do it. But it's
[66:12] a total myth that our brains believe very strongly that like we watch somebody do it. And we're like, everything that they're doing is making sense. Therefore, I understand this
[66:24] concept. But then when it comes time to actually do the thing ourselves, we're like, Oh, okay. I thought I had it. I don't got it. You know? Yeah. And that is definitely, and thank you
[66:41] for helping letting me kind of stumble my through way through, um, get as well. Yeah. It's painful. It's painful. Like I totally get like Jay was putting stuff in the comments
[66:53] too. And I'm like, dude, I get it. Like I get that way too. I'm just like, but here, here's the answer. Um, yeah, but also I, I do, I, Jay's not here anymore, but I'll still
[67:06] talk about him. Um, it was really helpful seeing how he was putting together the F strings as well, different from the F strings that we were seeing. And I will also put those
[67:19] in the chat just because I don't think, I don't know if I did. I can't remember. Is this a 90 minute thing or, uh, it's an hour to 90 minutes. Um, just because sometimes
[67:30] like an hour is not enough, but I try to keep them under an hour or around an hour just so that way people it's consumable still. Cause I think that's also another thing is
[67:41] when people are following along, it can be very, very overwhelming. Yep. No, I feel that. Um, yeah. Cause I think we're just about done with chapter one. There
[67:53] were like some review questions at the end, which we could, we could, I mean, three options we could do that today so that we're just like, we have checked off chapter one is done.
[68:05] And then we just go directly into chapter two next time. Or we use those review questions next time as like a warmup for chapter two or I almost feel like we should do that. No,
[68:17] I really liked the idea of doing them. I'm not great at them. Like if you were to like quiz me on them, I would feel the quits like no joke. But if it's like something I get
[68:26] to talk through, you understand comprehension and like, like I'm fine with that. So that's why I'm like, but I really liked that idea. So I am, we're going to start with chapter
[68:43] quiz on chapter one. Yeah. The review questions at the end. And I am putting that in our calendar invite that way. I also remember, I'm really excited about this. Like I feel like this
[69:03] is a good way to, and it was cool seeing it in VS code and also different ways I can see VS code. So thank you for that as well. Sure. Yeah. I mean, it may just, just in case later
[69:21] today, if, if your brain is like mine, my brain might be like, oh, we didn't, we didn't go any further than we did last time, but we totally did because we learned how to install
[69:33] it in VS code. We were working from like figuring out what was in our brains versus like where we were, where we wanted versus where we wanted to go and like how to troubleshoot all those
[69:45] error messages, which that's the skill, right? That's the job of a developer. And, and we did some Vim and we did some Git. So we did all kinds of stuff today. We did so much work.
[69:59] Yeah. The Vim was a little like, and I was not realizing I was going to go into Vim and for all of those watching, I have linked Laura's Twitter, go follow her on Twitter. Cause you
[70:16] do cool things and end up going on shows like this. And yeah, I think we're good. I think my, my brain is like, I get it and it's not fully mushy mush, but it's definitely where
[70:31] I'm like, I don't want to push it further. Cause I finally feel like I'm getting that, you know? Yeah. That makes sense. It does. Cool. Well, thank you all and talk to you
[70:42] soon. Bye beautiful humans. 
