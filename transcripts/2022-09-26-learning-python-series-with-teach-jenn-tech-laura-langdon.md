---
showLink: "https://www.youtube.com/watch?v=glEpZhXTfH0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learning-python-series-with-teach-jenn-tech-laura-langdon"
title: "Learning Python Series with Teach Jenn Tech & Laura Langdon"
publishDate: "2022-09-26"
coverImage: "https://i.ytimg.com/vi/glEpZhXTfH0/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech with Laura.
[00:07] Laura is one of our first series that we've been doing. She's been teaching me Python.
[00:16] I haven't really been coding in the last two weeks. I think I had two other episodes the week you and I talked,
[00:24] and then last week was conference week, so I have to get re-into this world now.
[00:30] I'm like, "Re-adjust. Time to re-adjust."
[00:34] I'm excited that we are back and somewhat back to normal. I feel like everybody knows,
[00:48] but I am horrible at social media. I'm posting live now on Twitter right now
[00:57] because I forgot to auto-schedule things. >> I did a minute ago too and tagged you, so I think.
[01:06] >> Sweet. >> We're not totally silent.
[01:10] >> Yes. Well, hopefully our friends still show up today, but I totally get it if they don't,
[01:15] and we don't do this just for them. We do this for the learning,
[01:19] and people can always watch it post, which is really nice being able
[01:27] to do that because that's what I had to do. Have you ever re-watched one of the videos that we've done?
[01:35] >> That we've done? >> Yeah.
[01:39] >> Yeah. I mean, I've re-watched parts to make sure that I didn't say anything too stupid.
[01:44] You know how it is. >> I do. I do. All right.
[01:50] >> But I watch other people's streams after the fact all the time.
[01:54] I almost do it like co-working, where they'll be working on something,
[02:00] and I'll be half listening and half doing what I'm doing, and then they'll say something that's
[02:06] particularly relevant and whatever, and I'll be like, "Okay,
[02:09] now I'm just going to watch you for 15 minutes or whatever." >> I get that.
[02:15] >> It's like study hall. >> Yes. Oh, that's such a good way of saying it.
[02:20] Hello, Ben. Hello. >> Hey, Ben.
[02:24] >> I upgraded my mic since last time, so hopefully this sounds better.
[02:29] Wow. I can't talk. The mic's not going to fix that at all.
[02:33] That's just, that's all me. Yay. I'm glad to hear it.
[02:39] It's a Blue Yeti, but it's like an old-school one,
[02:42] but I'm really excited because the way I have my setup, it's not really in the shot.
[02:47] I've never been more excited. The mic is in my shot.
[02:52] I don't know why. It's kind of, I feel like it's a little silly, but.
[02:57] >> This one, it's a little bit in the shot, but I could get it, I could lower it,
[03:01] but then it wouldn't sound quite as good, or I could change my camera angle,
[03:06] but I really like the pictures over my head, and so I don't. >> I like your camera angle,
[03:11] because I always compliment you for your background, and what up, homie?
[03:15] Or should I say, Ben and Ben. >> Oh, really?
[03:20] >> Yeah, but thank you for commenting the upgrade. My boss over at Gravity actually was like.
[03:30] >> I can't hear you now. Did something happen on my end or yours?
[03:38] Actually, it looks like you're muted. >> Can you hear me now?
[03:43] >> Yes. The mute symbol is gone. >> Is it the same quality? Maybe.
[03:50] >> I'm not very good at that. >> It just said that my mic went offline,
[03:55] and I'm like, I didn't even do anything. But I wonder if it did.
[04:01] >> You know what? It's its first day at work. >> It is. For all those who do conference life,
[04:08] I feel like you probably really, really understand coming back and having to readjust.
[04:16] It's not always the easiest. Yay. What up, Yara? How's it going?
[04:24] Yara was episode number one, which was like three months ago,
[04:29] which is mind-blowing to me. Can't believe it's been that long.
[04:34] I've been slowly, well, totally procrastinating on talking,
[04:42] but I've been working on trying to clear my screen so I can actually share it,
[04:46] how to move everything to the other screen. >> It's a thing.
[04:50] >> It is a thing. Anthony would always yell at me about that too.
[04:57] I'm really glad I have learned my lesson. But yes, we have a very, very blank screen.
[05:03] Yes, Yara, it has been three months, which is so crazy to me.
[05:09] I want Visual Code Studio. Yes, you can subscribe now.
[05:17] Ben and Homie really helped me out figuring that out, and Homie was my first subscriber.
[05:25] Subscriber. See if we can talk. Hey, we still have the document open.
[05:31] Yay, because I honestly haven't done anything since then, which is sad but true.
[05:42] Although, I don't know what y'all think of on going to conferences, but I loved meeting so many new people.
[05:55] It was fun. What up, Ace? >> Welcome. This is episode number 4?
[06:04] >> I think so. >> I think so. You are more than welcome
[06:09] to check our older episodes on YouTube. We do have a playlist.
[06:18] I feel like I should just call this the Laura playlist, but it's technically called the Python playlist.
[06:25] >> It's a little bit more of an informative name. >> But come on, they both work.
[06:31] >> We can do Python with Laura, and then we've got both of these.
[06:35] >> That would work. >> That was totally self-serving.
[06:38] >> I dig it. Ace, still hang out and ask your questions.
[06:45] I'm not saying go back, you have to watch those. No. I have to go back and figure out half of it as well.
[06:54] Also, thank you for being a subscriber. Thank you. But what we're getting back into,
[07:06] and Laura gave me the option last time, is do I want to do the quiz then,
[07:20] or do I want to do the quiz when we come back? Past me was very,
[07:27] very wanting to do it now. Future me, present me.
[07:34] We're going to see it because I went back to, here is also Ace.
[07:44] This is what we've been using is a website/book called Automate the Boring Stuff.
[07:51] It's been written for newbie programmers, so not even just new to Python,
[07:56] it's new to everyone. I just sent you what we're working on,
[08:05] which is Chapter 1, but there is an intro chapter
[08:08] that helps you download everything. I don't think it showed setting up Python and VS Code.
[08:18] >> No. >> I think we had to figure that one out,
[08:20] but that's in our last video. >> We just followed exactly what the VS Code instructions were.
[08:28] We just googled Python VS Code and VS Codes docs were precisely correct, which is always nice.
[08:37] >> Yes. I know Jay will be excited to hear that, that they were correct since he works on VS Code.
[08:45] I am scrolling all the way down. All this stuff, we did all of it.
[08:51] We are to the quiz. >> For anyone who geeks out about learning theory,
[08:58] like the theory of learning and so on, spaced repetition is the way to go.
[09:04] Doing the quiz, the practice questions here, two weeks later, probably a few days or a week would be optimal,
[09:15] but we don't live in the optimal world, we live in the real world and we do this every two weeks,
[09:19] and so it's going to be two and that's fine. Doing it like this will help really cement
[09:27] that learning much better than if we had just done it at the end of the last show.
[09:32] >> Ace, I see you downloaded PyCharm. >> I love PyCharm. PyCharm is my IDE of choice for Python.
[09:43] >> Sweet. Ace, ask us questions as we go along. I am going to see which of
[09:52] the following are operators and which are values. I'm pretty sure hello, negative.
[10:11] Wait, are values only numbers? I'm cheating, I'm going back up. I don't remember.
[10:20] >> The teacher in me is like, "Wait, don't do it yet." >> Okay. This is why I appreciate that she's a teacher.
[10:28] >> I guess I never introduced myself on this stream. Hi, I'm Laura. I'm a technical writer
[10:35] at Suborbital Software Systems. Until December though, it's less than a year ago,
[10:41] I was still a math professor, and I thought I was going to be a data scientist after that,
[10:47] so I was learning Python and so on, and then I ended up deciding to go into DevRel instead.
[10:51] But I still love me the Python. It's still my favorite language to code in.
[10:58] Here we are. The teacher in me says, "Students don't trust themselves."
[11:04] The moment when we're in student mode, and this is true for me too,
[11:09] the moment that we're like, "I don't know, is that correct?" Our instinct is to go find out,
[11:15] like ask someone who knows, you know what I mean? But also in terms of the theory of learning,
[11:23] the struggle to make the connections, those are the connections.
[11:29] That's what we're here for. If the way that we make the connection is by going back
[11:35] and looking at what's just casting our eyes upon the answer rather than figuring out what would make sense here,
[11:43] we are depriving ourselves of the learning that we think that we're here to do,
[11:49] and we're also not trusting ourselves because usually students know a lot more
[11:54] than they think they do. Off soapbox.
[11:59] - I want to add to your soapbox. Yeray said, "Hi, Laura.
[12:04] Glad to see a teacher in DevRel and hear sharing knowledge about learning theory too."
[12:10] Yes, I agree with all of that. And this is where I personally just want to add in.
[12:18] I, how to say this? I have a love-hate relationship with people like Laura.
[12:26] We'll say it that way. - That's fine.
[12:28] - In the fact that I get really frustrated and I'm like, "I want to do the easy way."
[12:33] Yet when I have people around that are like, "Nope, we're just going to do it."
[12:39] And even when they suggest I do it, not necessarily like they're telling me
[12:43] or anything like that, I'm like, "Okay, cool, I'll do it this way."
[12:48] And also as to the part about the trusting thing, I personally, personal opinion over here,
[12:56] think a lot of it has to do with school in the fact that if we failed a test,
[13:03] it wasn't a learning opportunity, it was an opportunity to be punished and reprimanded.
[13:09] - It was a learning opportunity in my class, just for the record. - Yes.
[13:12] - But anyway. - So I appreciate the call out and I completely agree.
[13:17] So, and I know for you, it is a learning opportunity, not a moment for punishment.
[13:24] And if y'all make fun of me for these, I'll just boot you off our stream.
[13:30] - Yep. - Well, I mean, most people don't really make fun
[13:34] of each other here and I really appreciate that. It's a really safe space to learn, but all right.
[13:41] Well, if I remember the following are, which of the following are operators
[13:46] and which of the following are values? I would say operators are the multiplication,
[13:54] symbol, the star, the subscription, the divide, and the plus, and the rest are values.
[14:02] - Why do you think that? - Because they're in the order of operations.
[14:06] - Yeah, okay, sure. - Not the proper order of operations.
[14:12] - No, no, no, I know what you mean. Yeah, not in the order of the order of operations,
[14:16] but they're in the like capital O order of operations. - Yes, yes.
[14:21] - Yeah, right, okay, so that's completely true. They could have been different operators
[14:28] that weren't in the capital O order of operations, but when we think about the word operator,
[14:33] like it means a thing, right? Operators, they operate on something, right?
[14:41] They do something to a value. So when you're multiplying two numbers,
[14:49] you're doing something to them. If you are printing a string,
[14:54] you are doing something to that string, right? If you are subtracting, if you're dividing,
[15:00] if you're adding, you're doing something. You're operating upon, operators operate upon.
[15:06] So it's not just because these happen to be the symbols that we use for mathematical operations.
[15:15] I mean, some of the symbols that we use for mathematical operations,
[15:18] but also because they actually operate upon. And the others have to be values because they can't,
[15:26] like hello, the string hello, can that operate upon anything?
[15:31] - No, but I was gonna say, can it be a value since it's not a number?
[15:36] - So the quest, the wording of this question, I think is strategic and brilliant.
[15:47] Because it prompts the reader to ask exactly the question that you just did.
[15:54] Can a string be a value? Because like in colloquial English,
[15:58] we think of values as numbers. Although we also think of values
[16:03] as like things that are important, right? In English, we use value in multiple ways.
[16:09] - Mission statement, values, personal mission. Yeah, all that. - Absolutely.
[16:13] Yep, it's something that is sort of, yeah, sort of considered important or whatever.
[16:19] But yeah, so here they say, which of, he says, Al Swigert, who wrote this and is brilliant,
[16:25] says, which of the following are operators and which are values?
[16:28] So there are only two possibilities for each one of these things.
[16:32] It's either an operator or it's a value. And so we feel pretty intuitively confident
[16:38] that the two numbers, those are definitely values. And then we ask ourselves exactly like you did,
[16:44] but hello, is that a value? Well, is it closer to being a value
[16:51] or is it closer to being an operator since it has to be one of those?
[16:55] - I still say value because it's not gonna operate on something.
[17:03] It's not a doctor. - Exactly. Exactly, it can't do something to something else.
[17:08] And so then that's why this is such a great question because it sort of prompts us to think about
[17:17] what is a value in like a computational sense because to the computer,
[17:22] in fact, the string hello is a number. Right, 'cause everything to the computer
[17:30] is all zeros and ones. - Yeah, that's gonna hurt my head too much.
[17:38] But real quick, Ben said more examples of programmatic operators. - Programmatic.
[17:45] - Programmatic, see, this is why I hate reading out loud. Not you correcting me, this is totally fine,
[17:50] but I'm like, I hate reading out loud in general. So this is such a great opportunity to do it.
[17:56] Ramon has always pushed me to read the comments out loud and I'm like, oh, I love it.
[18:00] Programmatic operators that aren't in the order of operations percentage
[18:07] get the remainder from a division, plus plus add one to the variable
[18:11] and save the new value to the variable less than. And this is when we were talking about Legos, right?
[18:21] - Yeah, that's the one. - This, Ben, so that way you know how I learned this
[18:25] and the way Laura taught me and I really want Legos now is if we have, let's say 20 Legos
[18:36] and we're doing the remainder from a division, it would be like, how many times can eight go into 20 Legos
[18:44] and if-- - Groups of eight. - How many groups of eight can go into Legos
[18:50] and only two groups can go into 20 Legos and then there would be four Legos left.
[18:57] Or for the plus plus is when only two variable or only two groups of eight could fit in 20 Legos.
[19:08] - That's actually not the plus plus. That is integer division.
[19:15] It's also called the floor, but that's the one where that's like, it's slash slash.
[19:22] It's like division sign, division sign. - Oh, okay.
[19:26] - The plus plus, just like Ben said, is add one to the variable
[19:30] and save the new value to the variable. So if you had like X equals five
[19:35] and then you said X plus plus, that means add one to whatever value is stored in X.
[19:41] And so if five is the value that's originally stored in X, then X plus plus would add one to five, which is six,
[19:49] and it would save that to X. So now X equals six.
[19:52] That's the plus plus. - Okay.
[19:56] And what up, Ramon and thank you, homie. I appreciate it.
[20:01] And something that I just like realized is we are up to 70 followers and 15 subscribers.
[20:09] Congratulations. Crazy dance.
[20:14] So, and starting in next-ish month, I'm hoping to also be creating more smaller videos
[20:25] by myself doing some of these and a quicker recap of all of these videos,
[20:30] because not everybody wants to watch the full live stream. Okay.
[20:37] - And that's spaced repetition, right? So we're gonna feed two birds with one scone, right?
[20:44] - Yes. Oh, I like that.
[20:47] - It's not mine. I got it from someone on Twitter and it's the bestest.
[20:51] - Feed two birds with one scone. I like this.
[20:56] I like this. Because I am completely comfortable being a snowflake
[21:01] who doesn't want to say killing the birds with the stones. I want to feed the birds with the scones.
[21:05] - I mean, I really like seagulls. Plus they go, "Mine, mine, mine."
[21:10] - Oh, I actually hate birds, but I still don't want to stone them.
[21:13] - Oh, okay. No birds for you.
[21:16] All right. Which of the following is a variable and which is a string?
[21:21] This one is easy. A string has the quote marks.
[21:25] - True. - Name three data types.
[21:30] - Resist, resist, resist the urge to scroll. - Oh, I was just putting it at the top of the page.
[21:40] - No, I know. - Data types.
[21:45] Integers. - I don't remember what whole numbers are and...
[22:00] - Whole numbers are integers. Well, I mean, so in terms of Python,
[22:07] like Python doesn't, in mathematics, we distinguish between whole numbers and integers
[22:12] where whole numbers don't have negatives and integers do and also have zero.
[22:15] In programming, we don't distinguish between whole numbers and integers, particularly.
[22:21] I mean, there's like signed and unsigned, I suppose, but they're like, they're just integers,
[22:26] especially in Python. They are just integers.
[22:29] - I just remember integers. That is the only one.
[22:32] Like, I know others exist but... - It's gonna be in there somewhere.
[22:35] It's gonna be in there somewhere. Okay.
[22:37] So what comes in the number 5.3? Right?
[22:45] What's the word that I said after five? - .3, point?
[22:51] - Point. There's a data type that has the word point in the name
[22:58] and it means that point. - Pointager?
[23:02] - That should totally be it, right? That should totally be it.
[23:06] But it refers to the fact that it can move. It can sort of float.
[23:13] - Pointerina? - Floating point.
[23:18] Floating point. - Floating point.
[23:19] I mean, that would make more sense. That would make more sense, but...
[23:22] - Floating points. But in Python, as in many other languages,
[23:26] they're referred to as floats. So they're like ints for integers
[23:29] and float for floating point. And there's also, what did you call the spam
[23:34] with the quotes marks? - Oh, strings?
[23:37] That's considered a data type? Huh.
[23:40] Okay. All right.
[23:45] What? Oh, wait.
[23:50] I scrolled. I remember.
[23:51] - Oops. Sorry.
[23:53] I didn't mean to click on that, Ramon. Sorry about that.
[23:56] But I am so glad that you're good, Ramon. (Ramon laughs)
[23:59] And I am good too. - We are...
[24:03] Ramon, we copied you, and we're both streaming to both of our Twitches.
[24:09] Twitch Eye. All right.
[24:13] What is an expression made of, and what do all expressions do?
[24:18] I feel like we're gonna be spending the entire time doing this quiz.
[24:21] - Oh. Oh, what is an expression made of?
[24:25] A smiley face, a sad face, a frowny face. Maybe a grin.
[24:34] - So this is as opposed to an equation. What do we have to have in order to have an equation?
[24:44] - Orders of operations? - Nope.
[24:51] It's actually in the word. Almost all of this is in the word equation.
[24:56] - Equals. - Equals.
[24:59] We have to have an equals. In this case, that's sort of like an assignment,
[25:03] or we're saying like something equals something, or it gets a particular value.
[25:08] That's an equation, or in programming, either an assignment or an assessment, I suppose.
[25:15] But if we don't have that, it's an expression. Just like in math, actually.
[25:22] X plus five is an expression, because it has no equals sign.
[25:28] X equals five is an equation. And that's all there is.
[25:34] - What do they do? I don't get that part.
[25:41] - What do they do? So in programming, if you use an equals sign,
[25:47] you can give a variable a value. Like in number six, actually.
[25:56] So bacon equals 20. We're saying that we're giving the variable bacon
[26:00] the value of 20. - Okay.
[26:04] - If we said like bacon plus 20, we didn't give it a value.
[26:12] We didn't assign it anything, and we didn't, it can't return anything either.
[26:17] Like it can't say like, it's not like an equals equals, where that's like, does something equal something?
[26:23] We'll get to that further on. But anyway, an expression is a string,
[26:28] like a bunch of code that doesn't have an equal sign, more or less.
[26:34] It could also be a- - Okay. - For the moment, we're just gonna say
[26:36] it doesn't have an equal sign. - I'm gonna pause, continue past that one,
[26:41] even though it still hurts my head. This chapter introduced assignment statements
[26:46] like spam equals 10. What is the difference between an expression
[26:50] and a statement? And an expression,
[26:55] I think this goes to me not understanding number four too, but a statement is like what it said, spam equals 10,
[27:07] but an expression would be like, five plus five equals 10?
[27:15] - But it has, well, I mean, so sort of like that, that would still be a statement,
[27:24] because it can still be either true or false, or like it equals something,
[27:27] or it doesn't equal something, because it has that equal sign in it.
[27:31] We're gonna play with more of these. Let's keep going through the quiz,
[27:38] and we're gonna do lots of these things, and then it'll like start making more sense.
[27:43] But these questions are good for just sort of like keeping little like squirrels in the back of your mind
[27:47] to go like, hey, wait, was that a statement or was that an expression?
[27:51] - Yeah, what does the variable bacon contain after following code runs?
[27:58] Bacon is 21 or 20, because I feel like it wouldn't run this.
[28:07] - Oh, no, it's 21, because if bacon equals 20, bacon plus one would equal 21.
[28:13] - Your second intuition was correct. - Yeah.
[28:22] - That because the first one, it says bacon equals 20. So we are assigning bacon the value of 20.
[28:28] And then what we said was bacon plus one. But like in the same sense as like in English,
[28:36] bacon equals 20 is a complete sentence. But bacon plus one is not.
[28:40] There's no conclusion. Like if somebody said to you bacon plus one
[28:45] or something like that, like bacon and lettuce, you'd be like, bacon and lettuce.
[28:49] - Potatoes. - Right, like what's gonna come next?
[28:55] Nothing changed about the bacon. - All right, and what should the following two expressions
[29:05] evaluate to? Spam plus spam spam and spam times three.
[29:16] So the first one, wouldn't it be spam, spam, spam? And then, yep.
[29:33] But the bottom one would be, wouldn't it be the same?
[29:39] - Yes, it would, yes. - Okay, all right.
[29:42] Why is a valid variable name while 100 is invalid? 'Cause it doesn't say what 100 is assigned to or doing.
[30:00] - So the word variable contains or almost contains the word very, right?
[30:06] It means that it can change. Can 100 change?
[30:10] - No. - Nope, not a variable.
[30:13] And so what that means is that we can't assign, we can't use 100 as a variable
[30:23] because it's like the computer would be like, no, you can't do that because 100 has to mean 100.
[30:29] You can't decide that 100 means something else or else everything will be fucked forever.
[30:36] - Yeah, okay, that makes sense. That makes sense, all right.
[30:39] And then, let's see. What three functions can be used to get the integer,
[30:47] floating point or string version of a value? I'm gonna ask this question in a different way.
[31:01] - Okay. - If I gave you the number five,
[31:07] for some reason on this stream, my favorite number is five.
[31:10] I don't know why, 'cause it's not like in other contexts. - I dig it, I dig it.
[31:14] - It's five. So if I give you the number five,
[31:17] what data type is the number five of those integer? - An integer?
[31:26] - It's an integer, right. What if I gave you the number five,
[31:31] but you needed it to be a floating point number, which means you needed it to be 5.0, okay?
[31:38] Then you could use a function and they all work the same way.
[31:47] So I'm gonna tell you how the first one works and then you can extrapolate from that
[31:51] what you would do for the second two, okay? So I'm gonna say, if we have the number five
[31:56] and we want to make it a floating point number, then what we would type is float,
[32:01] and then in parentheses, five. And so the float with the parentheses,
[32:05] that means this is a function that takes inputs and turns them into floating point numbers.
[32:13] So if I give it the number five, it would say, okay, well, that's an integer,
[32:17] but the decimal version of that integer, the floating point version of that integer is 5.0.
[32:23] So here you go, here's 5.0. (silence)
[32:29] - So it would just be like integer equals the number or? - It would be more like if you wanted it like,
[32:38] if you like to stick with these variables, like if you said spam equals five,
[32:44] but then what you wanted was the floating point version of it, then you could say spam equals float
[32:50] with five in parentheses. And then if you printed the value of spam,
[32:55] it would be 5.0 instead of the integer five. - But if I did like spam equals five,
[33:05] that's the integer five. But if I wanted spam equals or five equals string of spam,
[33:12] can you do that? - So you can't, but strictly because of the question
[33:21] that came before this, where five can't be a variable. We can't say five equals something that's not five.
[33:28] - So spam equals five or like a string of print spam plus five in a string will show the print of that string.
[33:40] - Spam plus five equals three, yeah. So that would be, you'd have to use a different function,
[33:48] not the float function because float takes integers and turns them into floating point numbers.
[33:53] So what you were just saying is you want something that takes integers and turns them into strings.
[34:00] - Yeah. - And so that one is a different one and that's string,
[34:06] except that it's abbreviated to STR. And we're gonna use these
[34:11] and then it'll feel much more intuitive as we're using them.
[34:15] This in programming, this is called casting. And I like it because it evokes like casting,
[34:22] you know, a spell or whatever, like you turn a prince into a frog, right?
[34:26] So you cast an integer as a floating point number. And so you wave your wand and you say abracadabra,
[34:33] you are now a floating point number. - Got it, okay.
[34:38] Last, why does this expression cause an error? How can you fix it?
[34:44] - String plus 99 plus string. I mean, couldn't we fix it by adding variables above it
[34:58] of I have eaten equals two and burritos equals three. So when adding this together, it would make 104.
[35:13] - 104. So I love that.
[35:17] So you solved a problem that was a different one than Owl had in mind,
[35:23] but is a totally valid solution to the problem that you were interpreting this as.
[35:28] So what you were saying was, I can't, like this is gonna cause an error.
[35:36] Why? So what you said was you were gonna set variables
[35:40] for like the string I have eaten equals, what was it two? - Yeah.
[35:45] - Okay. And then the string burritos was three?
[35:48] - Yeah. - Why does that solve the problem?
[35:54] - Because then they have the number assigned to them. So it's mixing, it doesn't mix integers and strings.
[36:01] - Data types, yeah. - Data types.
[36:04] - There we go. Okay, what's another way that we could solve it
[36:09] so that we would still end up with a string? - Something about the F strings that I was learning about
[36:20] that we technically haven't learned about yet in this? - No, actually you would still have to do something else
[36:28] inside the F string that would work here as well without an F string.
[36:32] We don't need an F string to solve it. So what you were saying was the problem is
[36:37] that I have eaten is a string. 99 is an integer and burritos is a string.
[36:42] So thinking maybe back to question number nine, what can we do to the number 99, the integer?
[36:49] What can we do to make it a string? - Just put quotes around it?
[36:56] - Yes, but what is another way that we can do it thinking about question number nine?
[37:08] - Put STR in front of it? - Cast it.
[37:11] You are now a string. - All right.
[37:20] - Right. - That just gave me a headache.
[37:23] No, it's just like, I'm glad I'm doing it. It's just like difficult to do.
[37:30] I probably would have given up like 20 minutes ago. So I'm glad I'm doing this live with you
[37:36] because then I can't. And I like that Homi said, "Go team, even learning extra."
[37:44] - Absolutely, yep. - Okay, I'm skipping extra credit.
[37:49] I'm not an extra credit kind of person. - I think that's a good idea.
[37:52] - Hey Bakari, what up Bakari and what up? I haven't eaten plus string plus burritos.
[38:01] See, that makes sense. - That's exactly what you said.
[38:06] - Yeah, they typed it the same time I said it. - Yep.
[38:09] - And hello, hello. - Hi.
[38:12] - Is it, what would we say LFEND or EIF or IFEND? I don't know how to say their name.
[38:20] - I hate fonts that don't distinguish between a capital I and an L.
[38:24] - Right. - Which.
[38:28] - I'm always like, I don't know. I don't know if it is, but thank you.
[38:32] I appreciate the help on it. All right, so we are now going to IF, okay.
[38:39] Is it IFEND or IF, I don't know how to say your name properly. I will get stuck on this, so I'm gonna keep scrolling
[38:56] because I will like try to do this way too long. All right, so we are talking about flow control now
[39:04] and I know for myself, just for everybody as a heads up, I can only go until 10 after the hour.
[39:11] So we're just gonna see how far we can get in 30 minutes. And you're not irrelevant, FYI, you are a beautiful human
[39:22] that's showing up to hang out with us. I just know that I'll get stuck on trying to say names.
[39:28] So that's the only reason, but you are not irrelevant. All right, so.
[39:37] - I think the last sentence of the first paragraph is most of what we need to know here.
[39:48] - Flow control statements can decide which Python instructions to execute under which conditions.
[39:56] - And it works exactly like a flow chart. - All right. - Which is what we have here.
[40:01] - And this made sense. So when I was like, as a heads up y'all,
[40:06] something that I've learned to do is work on, I learn best by listening as audio instead of reading it.
[40:15] As you can see, I'm not great at reading out loud either. And so I listened to the audio version of this
[40:22] before we get started. And one thing I've noticed
[40:25] is this really made a lot of sense. But then further on in the chapter,
[40:30] it goes to the text version and I'm like, it's not visual. I don't get it as much.
[40:37] - We can make it visual though. We can try it out.
[40:40] We can totally do that. - Okay.
[40:42] But before you learn about flow control statements, you first need to learn how to represent
[40:51] those yes and no options. And you need to understand
[40:55] how to write those branching points as Python code. To that end, let's explore a boolean.
[41:04] - Boolean? - Boolean values comparison operators
[41:08] and Boolean operators. - Named for a mathematician named,
[41:13] I think it was George Boole, B-O-O-L-E. - Oh, we got George right here.
[41:22] All right. - Hi, George.
[41:25] Yeah, and literally all that means is true or false. Like that's all that we need to take away from that.
[41:32] Booleans are ultimately things that are either gonna be true or false.
[41:38] - Okay. Okay, this is actually, I just wanna point out,
[41:45] and this is something that I really, really appreciate with learning with you, Laura,
[41:50] is the fact that I do get really frustrated in this because especially during the times
[41:55] where it does not click very easily because that's how a lot of things just kinda work for me
[42:02] and it's very convenient. Yet, struggling through this kind of stuff,
[42:07] I get really frustrated because it doesn't click. And I appreciate the fact that you help me either go,
[42:15] okay, cool, we'll get back to it because something in the future we'll go through it,
[42:19] or no, we're gonna sit here and duke it out with a book. So it does make sense when you say
[42:27] that it equals true or false. That's kinda what I was getting
[42:30] when I listened to it earlier. So spam equals true.
[42:37] So if we just type spam, it equals true. A traceback, which...
[42:45] - So this is because of the in number two of like one line above where it says
[42:51] if we just type true, then it says the name true is not defined.
[42:58] That's not about, it's not like run together from the first one, just for clarification.
[43:04] - Okay. And true can't equal two plus two
[43:08] because that's not a complete thing. - That makes no damn sense.
[43:13] - Yeah. Okay, but could you do true equals four?
[43:19] - No, because it's... Okay.
[43:22] - Right, because then it would be like truth is equivalent to the number four, which would be odd.
[43:30] Not in the mathematical sense of odd. That would be weird.
[43:36] - Anyway, that would be even, but... Okay, like any other value,
[43:43] Boolean values are used in expressions and can be stored in variables.
[43:48] One, you don't, if you don't use the proper case, two, or you try to use true and false for variable names,
[43:56] three, Python will give you an error message. And then we got comparison operators,
[44:04] also called relational operators, compare two values and evaluate down
[44:11] to a single Boolean value. - Okay, I feel like these are pretty common, luckily.
[44:20] - Yep, yep, that double equals, I think that's just about universal.
[44:25] So that means is equal to, or is like equivalent to, the exclamation point equals,
[44:35] that isn't universal to all programming languages. Some programming languages do it with like equals
[44:41] and then slash equals to mean not equal to. I like this, I mean, it's fewer characters
[44:46] and also because I like calling it bang. - Just, I just wanna double check.
[44:58] Ace, if you're still here, let us know if you have questions so far as we're going through this.
[45:05] - Absolutely. - I know that you're just getting started with Python,
[45:08] but I do want to suggest that you can go through and ask us questions at any point.
[45:15] And that goes for everyone, so not just Ace. Ace was just the one that mentioned
[45:21] that they were a bit newer. All right, so this makes sense.
[45:28] So it says 42 is equal to 42, true. 42 is equal to 99, false.
[45:35] Two is not three, equal to three, correct. Two is not equal to two, false, it's not.
[45:43] Because if that equation doesn't compute because they are equal, there we go.
[45:50] - In inequality, it's not inequality because then it would be true.
[45:55] Equations have to be true. - Got it.
[46:02] - Otherwise they're inequalities. - Okay, okay.
[46:07] - You're either equal or you're not equal. - All right, well, we will try to--
[46:13] - Statement, if we want to say, if we want to use like a single word
[46:19] that isn't inequality, we can say statement. The statement two is not equal to two is false.
[46:25] - Oh yeah, okay, so the statement, got it. Okay, so the statement.
[46:31] And then we got, you might expect equal equal is equal to evaluates to true
[46:42] when the values of both sides are the same and not equal to evaluates to true
[46:47] when two values are different. The equal and not equal to operators
[46:54] can actually work with values of any data type. All right, and these are all making sense
[47:02] because the second one is false because one letter is capitalized.
[47:07] Um, oh, it did catch that 42 and the integer of 42 are the same.
[47:16] - Right, the integer of 42 and the floating point. - Yeah, the integer and the floating point are the same.
[47:23] And these are not the same. 42 equals quote 42 because it's in a quote.
[47:30] So it would technically create it, it would mean it's a string.
[47:33] - That's right. - Oh, groovy, all right.
[47:37] Which this just said all the same stuff we said. And then this is where I get mixed up
[47:45] is greater than or less than floating points, so. - So the big end of the thing
[47:54] points toward the bigger number. - Okay.
[48:00] - So if we're looking at like 42 and 100, like just to remember like which direction
[48:06] do these things need to face. - Yeah.
[48:08] - The little end is pointing toward the 42 and the big end is pointing to the 100.
[48:13] - Okay, so that's why when the shark is eating the smaller number, it's false.
[48:20] Maybe go into that. Okay, a count equals 42.
[48:31] And then I'm confused why the second line is a count is less than or equal to 42.
[48:42] So it's the same those two ones because it's less than or equal to.
[48:49] - It's the or equal to, yep. - Okay, and then my age is 29.
[48:54] My age is greater than or equal to 10. True.
[49:00] - Yep. - Boy.
[49:02] - Okay. - The difference between the equal equal
[49:07] and equal operators. You might have noticed that the equal equal operator,
[49:13] equal to, has two equal signs while the equal operator assignment has just one equal sign.
[49:20] It's easy to confuse these two operators with each other. Just remember these points.
[49:26] The equal equal operator, equal to, asks whether two values are the same as each other.
[49:32] The equal operator assignment puts the value on the right into the variable on the left.
[49:40] To remember which is which, notice that the equal equal operator, equal to,
[49:44] consists of two characters, just like the exclamation point equals operator,
[49:51] not equal to, consists of two characters. - Right, so one of them is like equals,
[49:58] one equals sign, or equal to, two words, two equals sign. - Cool, makes enough sense.
[50:06] All right. I'm gonna go to Boolean operators.
[50:13] The three Boolean operators, and, or, and, not, are used to compare Boolean values.
[50:22] Like comparison operators, they evaluate these expressions down to a Boolean value.
[50:29] Binary Boolean operators. - And we remember binary, it's just meaning two,
[50:36] means there are two things. So we're just comparing these two things.
[50:40] - Okay. The and, and, or, operators
[50:48] always take two Boolean values or expressions, so they are considered binary operators.
[50:55] That's how we got two. Okay.
[50:58] And the, and, bleh, the and operator evaluates an expression to true
[51:06] if both Boolean values are true. Otherwise it evaluates to false.
[51:11] Enter some expressions using and into the interactive shell to see an action.
[51:19] Let's scroll down a bit, 'cause I feel like these aren't necessarily
[51:24] the most informative. Let's just get a sense for all these operators.
[51:31] There we go. So here we are.
[51:33] So we're mixing the Boolean and comparison operators, which is the thing that we could do, you know?
[51:38] So we have four is less than five, and five is less than six.
[51:41] So and works exactly like we want it to do too. If you say, like,
[51:47] Laura is a technical writer and Laura knows Python, like it has, that's only a true statement
[51:55] if both Laura is a technical writer and Laura knows Python are true.
[51:59] - Can, can you use Boolean operators for strings as well as numbers?
[52:15] - Not without bringing in some functions maybe, because like it wouldn't,
[52:22] like if you said Laura and Jen, there's sort of no way to assess
[52:29] whether that's true or false, right? If you said Laura and Jen have met in real life,
[52:37] you know, then that's something that you can assess. But the, and in that sentence is not,
[52:46] in the, is not, I mean, yeah. I'm not saying that super well,
[52:54] but like it's, that's, you'd have to bring in something else.
[52:57] You have to add something to it. - Okay.
[53:02] And on that point. - So, or is at least one of them has to be true.
[53:12] - Yeah. So, and it's saying that the two is equal to two.
[53:19] - Right. At least one of them has to be true.
[53:25] - Okay. And then--
[53:27] - It can both be true, that's okay. - Okay.
[53:30] - But it has to be at least one of them. There is something else called an exclusive or,
[53:34] which means either this or that, but not both. - Okay.
[53:40] - But we're not, we're not worrying about that at the moment. - Okay.
[53:43] I feel like this is like the, what I've always hated about trying to figure out Excel.
[53:51] Just in case anybody was curious. - Absolutely.
[53:54] - This is, this is what I did not like about Excel. But like, it makes sense,
[53:59] but then it doesn't make enough sense. But this is teaching me.
[54:02] This is teaching me the ways. All right.
[54:05] So if four is less than five and five is less than six, then it's true.
[54:16] - Yeah. Both of those are true statements.
[54:20] Four is less than five and also five is less than six. So that's true.
[54:25] - So we wouldn't, I guess like I get that there, that this is an image to like describe it,
[54:32] but I feel like this true and five is less than six makes it very confusing.
[54:39] Like, why did that one drop down, but the first one didn't drop down.
[54:42] So if I just like skip this line, it's true. - Yep.
[54:49] - Okay. Which makes sense.
[54:50] - Because that's the, so what he says is, you can think of the computer's evaluation process.
[54:55] It's literally because the one that the computer is going to consider first,
[55:00] is the one that is written first on the left. Four is less than five.
[55:04] So it's going to consider, is this true? Because if it's not, we can stop here.
[55:09] We don't even need to consider the second one if the first one is false.
[55:15] - Got it. - Even if it were an or, because or is at least one,
[55:18] but and is both. So if the first one is false,
[55:22] we don't even care whether the second one is true or false. - Got it.
[55:27] And I'm going to paste this in here. This is the link we're using
[55:32] for anybody that wants to follow along. I know we're going through a lot of theory
[55:36] before doing it on coding. And yes, yes, I agree.
[55:43] It's important to understand how the computer will interpret the code.
[55:47] - Yep. - It's definitely something that I think,
[55:55] yeah, you're all right. It's just not the way my brain like read it very easily.
[56:01] - Right, yeah. It's because we're not reading all of the words
[56:05] that Al wrote. - Yeah.
[56:07] - 'Cause if we had read the words that Al wrote, then we would be seeing.
[56:09] - Yeah, that's true, that is very true. That is very true.
[56:13] - This is not Al's fault. - No, no, not at all.
[56:16] And I do want to say that I appreciate the way we're going through this
[56:20] because me trying to read from a textbook is, I find it very, very difficult.
[56:26] Like even when I had, like if I listened to this beforehand,
[56:30] it's a lot easier to comprehend even if I don't comprehend it all then.
[56:35] So I totally get that. You can also use multiple,
[56:42] now I forgot how to say it, Boolean. - Boolean.
[56:47] - Boolean operators in an expression along with comparison operators.
[56:53] So. - Let's skip this part.
[56:57] - Okay. Sounds good to me.
[57:01] I dig it. But I mean, I do think this makes sense
[57:06] just as apparently I don't want to skip it. I really want to just say,
[57:09] it does make sense in the fact that in my mind, you would have to do like the first group of numbers,
[57:17] the second group of numbers, the third group of numbers.
[57:21] And do they equal, does the first group not equal the second group
[57:29] and does it equal the third group? - So yes, but not strictly
[57:41] in the way that I'm hearing the words. - Okay.
[57:47] - Because it's not that we're asking if two plus two is equal to four,
[57:53] if that is equal to the second group or if that is equal to the third group.
[58:01] I mean, we sort of are in the sense that two plus two is equal to four,
[58:04] that evaluates to the value true. And because it's asking and not the second group,
[58:13] which is false, so true and false and true, and so it's just, that's sort of why.
[58:23] It's not that we're asking so much if the first group is equal to the third group
[58:26] or the second group, so much as we're just trying to string together,
[58:31] is the first statement true, the second statement false and the third statement true.
[58:37] - Got it, okay, okay. - And if that's the case, then this whole thing is true.
[58:41] Yeah. - I will say,
[58:44] and I noticed we only have like 10 minutes left. I feel like, would this be a good breaking point?
[58:53] The elements of flow control? Just trying to.
[58:57] - I think we can do the if and the else, but I want to start with that flowchart.
[59:05] - Okay. - And go backwards, or maybe even go backwards.
[59:09] - Let me go to the scrolls. - Yeah, so the flowchart says,
[59:13] so the if statements clause. So if we just read this without any other context,
[59:19] we who have learned how to read flowcharts, we say, we go to start,
[59:28] and then what would be the next word that you would say? - Yeah, after start, go to, does name equal Alice?
[59:39] - Yeah, so if name is equal to Alice. - If name is equal to Alice, okay.
[59:48] - Yeah, then. - Then print, hi, Alice.
[59:57] If not, print, or false, don't do any. - Yeah, and so in code, if not is else.
[60:05] So if name is equal to Alice, if that is true, then we're going to print, hi, Alice.
[60:13] Else, stop here. - Okay.
[60:19] - And those are if-else statements. - Okay.
[60:23] - And that's where a lot of the flow control is gonna happen.
[60:26] If this, then that, else, other thing. - Okay, and that makes sense.
[60:37] - Yep, so let's keep going. So we just basically covered the if and the else.
[60:43] So let's, we're gonna just live on the edge. - Else statements, yeah, so else, print, hello, stranger.
[60:51] I like it, all right. So that's where they put, if name is equal to Alice,
[61:01] is true, print, hi, Alice. If false or else, print, hello, stranger.
[61:13] And then end after both of those. - Right, exactly.
[61:17] - Okay. Elif statements.
[61:23] - Else if, which is abbreviated Elif. - Elif.
[61:28] - Or Elif, or whatever. - Elif.
[61:31] - But we read it out loud as else if. - Else if, that's like OSS.
[61:37] It's like, if you say it, you say open source, but if you type it, it's OSS,
[61:45] which is open source software. Why, why?
[61:50] I don't know, whoever comes up with naming conventions, like, please, please explain to me.
[61:56] Okay, so else if statements. While only one of the if or else clauses will execute,
[62:04] you may have a case where you want to have one of many possible clauses to execute.
[62:11] Let's see it in the code. Or in the flowchart, even better.
[62:18] - Yeah, okay. Like, I get what this is doing.
[62:31] The reason I'm a bit, like, confused. If name is Alice, or equal to Alice is true,
[62:40] print hi, Alice. If false, if age is
[62:45] less than 12, true, print you are not Alice, kiddo.
[62:55] And I guess I'm a bit confused because those two, like, don't even go together.
[62:59] - Okay, so let's change it in our minds. So if name is equal to Alice is true, print hi, Alice.
[63:06] Else if, in fact, I bet there's gonna be a different else if if we scroll down where it's like,
[63:12] nope. - Granny, okay, like, it does make sense
[63:21] in the fact that, like, it's doing, like, having it go through.
[63:26] And this is something that I was kind of talking about with Excel.
[63:30] It's like, it's doing an else if. Like, it just decided to put numbers with the name Alice,
[63:37] which, that's fine. It's just kind of, so you can keep doing else ifs.
[63:42] - Yeah, and so what this is saying, this is saying is, in the first one,
[63:46] if name is Alice, then we print hi, Alice. But then we're considering some possible ways
[63:54] that someone could be not Alice. So if the age is less than 12,
[63:58] then that person is not Alice, and they are a kiddo. Right? - Yes.
[64:05] - If the age is greater than 2,000, then they're not Alice,
[64:09] and they are an undead, immortal empire. - I dig it.
[64:13] - If they are not Alice, and their age is greater than 100,
[64:17] then you are not Alice, granny. It is probably a granny instead of a grandpa,
[64:25] because women live longer than men. But what we notice, what's important here,
[64:29] is this flow chart, right? So what is the, it's important that we asked
[64:36] about the age being greater than 2,000 before we asked about the age being greater than 100.
[64:42] Because if the age is greater than 2,000, it's definitely greater than 100, right?
[64:49] - Okay. - And so, but if the age is greater than 100,
[64:53] it's not necessarily greater than 2,000. If we had reversed the flow of these,
[64:59] if we had said, if age is greater than 100, print you are not Alice, granny,
[65:05] and then put the, if age is greater than 2,000, print, unlike you, Alice is not an undead, immortal empire,
[65:13] then we would be printing both of those things if someone were 3,000 years old.
[65:17] - Oh. - Right? We'd print both.
[65:24] And so we have to think about the order in which these questions need to be asked.
[65:29] Because if somebody were 3,000, then they would fall into that,
[65:34] that if age is greater than 2,000 group, and then we would print the thing
[65:41] for the age greater than 2,000, and then we would proceed directly to end.
[65:45] But if somebody were 500 years old, it would say, if age is greater than 2,000, no.
[65:54] Else, if age is 500, is that greater than 100? Yes, so then you are not Alice, granny.
[66:00] But if we had reversed those, then someone who was 500,
[66:04] it would ask first about the 100 and then the 2,000. But if somebody were 3,000, it would print both.
[66:11] - Got it, got it, and that does make sense. Couple comments from our beautiful humans.
[66:21] Maybe if you think of it as a maze, and you're trying to get to the end,
[66:26] each evaluation tells you which way to turn on your way to the end.
[66:33] - Yeah. - Agreed. - It's kind of a choose-your-own-adventure.
[66:35] - Yes, and I also agree, we'll be doing typing the codes next week, or next time,
[66:41] which is in two Mondays, 'cause I gotta end in like three minutes.
[66:46] Normally we do, this has been a lot of theory, which we normally aren't as theory-heavy.
[66:54] Normally it's like a side-by-side. If you catch the other ones we've done,
[67:00] and I believe I have that playlist right here. So let me, ah, what did I do with my Twitch?
[67:08] So many options, there are so many options. Laura comes on the show, it is Python with Laura,
[67:19] and she comes every two weeks, and we go through the beginning stages
[67:26] of bare basics of Python. So I would definitely check those out,
[67:30] and also put that on your calendar if you're liking the Python side of things.
[67:35] The rest of the time, I'm learning a bunch of theory and JavaScript.
[67:40] - Yep. - So. - Yeah. - Although I do think
[67:43] I have a Kubernetes coming on soon, and Kafka. - I'm working on the Kubernetes.
[67:53] - Yeah, I think I also have a Kafka. I'm trying to think who else.
[67:57] I might have some, I'm debating. I have a guest that's coming on Friday,
[68:04] and they're like, "Hey, we'll go through whatever you want." And I'm like, "He told me he knows Go."
[68:09] I'm like, "I don't even know what Go is or does." So I'm kind of debating just being able
[68:16] to see a little bit about that. - I started learning Go a couple months ago.
[68:20] - Yay, let's go. - Yes. (laughs)
[68:26] - So yes, very cheesy, I know. And for all of those joining today, thank you so much.
[68:31] I will be back again tomorrow, same time, 9 a.m. Pacific, 12 p.m. Eastern,
[68:39] and 1600 UTC, I believe. And yes, make sure to follow-
[68:48] - 1700, I think. - 1700?
[68:51] Is it 1700? I don't know.
[68:54] I need to keep, go update that, make sure it's right. But thank you all for joining today.
[68:59] I will see you again tomorrow, and make sure to follow Laura on Twitter and Twitch,
[69:05] and be back soon. Bye.
[69:08] - Bye. 
