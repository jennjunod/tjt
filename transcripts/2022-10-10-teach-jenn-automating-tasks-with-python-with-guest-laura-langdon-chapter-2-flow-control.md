---
showLink: "https://www.youtube.com/watch?v=3VnyR6QARpU"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-automating-tasks-with-python-with-guest-laura-langdon-chapter-2-flow-control"
title: "Teach Jenn Automating Tasks with Python with guest Laura Langdon Chapter 2 FLOW CONTROL"
publishDate: "2022-10-10"
coverImage: "https://i.ytimg.com/vi/3VnyR6QARpU/maxresdefault.jpg"
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

[00:00] Hello, hello, beautiful humans. Welcome back to another episode of Teach Gen Tech and to the series of Learning Python with Laura. I feel like you should be like starting your
[00:16] own channel of learning with Laura and you could teach all the things. I have thought about it because there's stuff I want to learn too, but I didn't want to
[00:24] be like stealing your idea. No, it's like I feel like everybody has like a different way of doing things. Like learning with Jason is out there. Jason's actually
[00:39] going to be on the show sometime. Yay. That's exciting. It is. And I'm going to be learning from him. So it's all like, you know, even if we have
[00:51] the same ideas, we all learn so differently. So I would sign up. I'd be there. I would show up. So probably going to do that. Just saying. Just saying. And okay, y'all,
[01:04] just to start, we got to get this in the air elephant in the room out on the air is especially funny given what we're about to talk about. I know. Like, I don't know. Whatever. We may
[01:18] randomly end our stream today mattering on how Laura is feeling. Because, Laura? I went to Florence. Yesterday was my daughter's 16th birthday and we went to a Florence and
[01:33] the Machine show, which was her request because she's a super cool kid. And I had forgotten about all of the pot that gets smoked at shows and I am not opposed to the partaking of the
[01:46] pot. But I had pneumonia two years ago. Not COVID. Bizarrely not COVID. But it damaged my lungs. And I'm now like asthmatic or like I have highly reactive airways or like however
[02:01] you want to phrase it. Anyway, I'm broken. Lungs are broken. And like by the end of it, I couldn't even stand up anymore. I had to sit down. I couldn't speak. It was really
[02:12] unpleasant. And I wish that people would use vapes or edibles or whatever because it's a public space and you never know what people have going on and you can't tell to look at
[02:23] people that they have damaged lungs. Right? So, yeah. That would have been nice. So, I'm not totally sure how long I'm going to last today. It doesn't hurt anymore, but I can
[02:36] still feel my lungs, which is weird. Yeah. >> Fair enough. And thank you for sharing. And this is something that Laura and I were talking offline really quick of I'm very asthmatic,
[02:51] yet like weed and that kind of thing doesn't really affect me as much as vaping can. Because my partner does vape and it's a lot better than cigarettes, but it is something that
[03:10] there's times where it really affects me. But outside of that, it's normally just exercise induced. And, but my mom, like she smells anything like perfume, lotion, hairspray,
[03:25] and she's a goner. And I find this interesting to talk about because yesterday I was like, how do you explain to someone what it feels like to have to take your, use your inhaler
[03:40] and the jitters it gives you, and then the possible like headedness, and then you feel like really spazzy and then feel like you're going to fall asleep because it took your
[03:51] body all of this to heal your lungs. And that while I was cleaning the house yesterday, I experienced that. So, you are hidden close to home. I've had it my entire life though.
[04:02] I, um, so it's just second nature to me, but like getting it from pneumonia, dude, that's scary. Yeah, it's really weird, but you know. All right. Well y'all, um, I'm going to do
[04:19] most of the talking and probably most of the, uh, I'm going to go for today. And I feel like I need to do this anyway, that Laura is just going to be there for backup for today
[04:34] as we go through the next one, because I need to start doing a lot of it more on my own. Like I still don't remember all of the command line stuff. Um, so on that note, I used to
[04:50] tell my students, um, for anyone who's, who's tuning in for the first time, um, I used to be a math professor. I was a math professor at this time last year. And I used to tell
[04:59] my students, um, that the one who's doing the work is the one who's doing the learning. Because a lot of times, especially in math classes, students really just want to watch
[05:09] you solve problems and write them down because that's really comfortable, um, and safe. And they would get sort of, they would resist a bit when I would say, okay, I've done one
[05:20] now, you know, let's all like struggle through one together. And they'd be like, no, I really want to just watch you do it. I'm like, but the one who's doing the work is the one who's
[05:29] doing the learning. And I already know this stuff, you know? Yes. Yes. And hello, Ian. Ian has been on the show before, as well as he live streams
[05:41] and, uh, because, so I don't forget. And, uh, somebody was asking me about resumes and stuff, and I sent them your live stream. So you might have a random person reaching out.
[05:56] Also, I, as I'm part of the Denver API Meetup group, Ian's going to be presenting, which I'm pretty excited about. And also, Ian, because you're here and I don't want to forget, again,
[06:09] would love to have you on the show sometime and talk about Postman, because that would be dope. He is a DevRel over at Postman. And yes, Ian, I am learning the Pythons. I have
[06:23] not done anything with the lights yet. He has this really sweet back, like, like lighting situation. I was on Ian's show like two months ago.
[06:33] Oh, yes. Yes. Yes. I will. We're getting there. We're getting there. Um, so on that note, I will share my screen soon. There we go. Uh, okay. There we go. Yay. Yay. Isn't Laura
[06:57] great? I adore Laura. Laura's on the show every other week. Um, oh, by the way, Laura, we are, um, with your, you being the very, very first, uh, uh, series, we are going to
[07:16] have another series starting with TypeScript. Ooh, nice. Yeah. And it is somebody that wrote a book called Learning TypeScript. And I'm very excited. Josh, Josh Goldberg. Is that
[07:31] his last name? I think it's his last name. Okay. Well, so this week we do not have a quiz yet because we did not finish chapter two. I'm going to scroll for a while. We learned
[07:47] you want to clone your, your repo for this new machine. I will give me just a second, but good call. I do need to say a good call because that is, um, so I'm just kind of going
[08:02] through because we didn't really do too much coding last time. It was, uh, what up juice? I hope I said your name, right? We are learning about Python. And if you have questions, let
[08:15] us know. Um, oh, I should put this in the chat actually. Maybe, maybe we'll get there. We will get there. We are working on chapter two of automate the boring stuff from Al Swigert.
[08:42] Yes. I said it right this time. And I will be putting that in here. We also have, uh, the previous streams with Laura and I have a playlist for that. Let me go grab that.
[09:07] Python series. Yay. All right. So, all right. So, last time, uh, yes. Yes. Al Swigert does do a really dope live stream as well. I've joined, um, or at least like watched it. And
[09:36] the entire thing I did was, uh, talk about, like, try to get him to show the kittens because he had a lot of kittens. And so that was, he was fostering kittens. That was the entire
[09:49] thing that I was getting out of his live stream while he was like replying back to people. I was like, I just want to see the kittens and then I'll learn Python later. So, uh,
[10:00] getting back to today's Python, um, we learned about Boolean values, which are like, if I say it, it's the if and kind of thing. Like, is it true or false or is that the comparison?
[10:16] Yeah. So, the Booleans are the true false. The if and the else are flow control, which frequently involve, like, depend upon Booleans. Okay. Okay. Cool. And, uh, yeah, we just basically
[10:38] went through the majority of this, but I am going to figure this out without having to ask Laura how to do it. So, that way, hopefully I remember. I keep forgetting how to clone
[10:51] my repos and move them to the computer and re-upload them, especially with Hacktoberfest being here. It's, I'm like, I should know this. I should know, but I don't. So, I know,
[11:12] but all right. If I were to Google all the things, I would say in CLI create new folder. Uh, all right. So, we are going to go to so, CD is what moves it and we have folder names.
[11:36] Okay. But it is capital. What? Oh. Is it because I'm in on Windows? Um, the, the Windows doesn't use the Unix command line, which Linux and Mac OS do, but
[11:55] you can get one, which I would recommend. So, I would download Windows subsystem for Linux. There you go.
[12:10] And hello, Ramon. Okay. This makes so much more sense why I couldn't get this to work the other day. And for everybody, my Mac is still in, in the thing, at the repair shop
[12:31] again. Because it was not what? Elevation. That probably means you don't have the, like, admin permissions. So, you need to run as
[13:05] Windows. I haven't used Windows in a bit. So, yeah, command terminal, like, run, yeah, just a few. It's what I'm going with. I hope it was somewhat accurate. All right. Command
[13:36] terminal. Right click on run as administrator. Okay. Oh, pop ups. Yes. Yes. Oh, hey. Okay. I hope that is legible. Yeah, I mean, it's good for me anyway. Yay, it's installing.
[14:16] I didn't know this was a thing, but this is a thing. And glad to see that I can still use the commands that I would on Mac. Because then I am learning it for what I normally
[14:31] use. But this is, so, for everybody to know, I spilled water all over my Mac, like, two weeks ago. I brought it in. Oh, did it? Am I back?
[14:46] Yeah. Okay. I don't know why I froze. Well, that could make this stream very interesting as well. It's choppy. Well, okay. So, not actually your screen, but just your video.
[15:03] Just your camera. Your screen is totally normal. Your camera cuts in and out a little bit. I really want my computer back. Apple, if you can hear me, please give me my laptop
[15:18] back and working. Why did I just lose you? Oh. Frank, good call. Nothing wants to work today. My AirPods just disconnected. Just a second. I'm no longer
[15:30] using you. Oh, there we go. You're back. Okay. Default. Just leave the Ubuntu default distro. It's fine. I would say. So, then would I need to run it as an administrator
[15:55] again? What is the next, is there a next step in the install process? So, we don't need to change the thing. >> Yes. We definitely will. Now it's really
[16:30] big. Prerequisites. Install. I'm just going to see if it works now. >> No. Oh. Oh. >> Okay. Cool. Okay. So, do you wait. You're
[16:57] not actually in Windows subsystem for Linux, I think. Does it say on the in the browser how to run it? >> Change default Linux distribution installed.
[17:28] This can be changed using the D flag. >> Yeah. Just keep scrolling. We're good with the default. Okay. Best practices for setting up a WSL development environment. Oh, stop.
[17:48] Go back up. There we go. That link. Best practices. >> And in case anybody is wondering, this is okay. Oh, and a homey coder, Ola Soymilk is one of the master magicians at things and
[18:23] stuff. That's what I'm going to call it. Master magician of things and stuff. >> You can put that down, Ramon, as your job title. We've been having to figure out our
[18:37] job titles at Suborbital and like what's going to go on the website. So, now Ramon has a good one. >> I'm hoping. I am not. Let's put it out
[18:50] there. Good vibes. I am in the interview process somewhere. And it's going very well. And upon getting hired, I am hoping that they will let me use develop Cado as my job title. I
[19:06] don't know if they will. But all right. So, get started. >> You've already installed. So, we did that. >> Here we go.
[19:27] >> Oh. Once you open the distribution, start using start menu, you will for your Linux distribution. So, it might be under W for WSL or U for Ubuntu. I really haven't used
[20:02] Windows in such a long time. >> Yeah. This is just searching it. >> I've been using the start menu. >> Yeah.
[20:17] >> What shows up under apps? >> Under apps? Let me where do you see apps? I don't anymore. It's gone now. >> I think it was showing up because of oh,
[20:36] yeah. >> There we go. Up there in the top. Okay. >> Oh. >> That's not helpful. Oh, but the Frank Freeman
[20:46] suggests we should be able to find it under WSL.exe. Oh, wait. Go back. There it is. Run it again. Maybe. No, I think I was wrong. Sorry. My bad.
[21:07] >> Yeah. >> Search again. WSL. I don't need that. >> You don't have to restart, do you? >> If I do, that's going to be really annoying.
[21:21] >> Yes, it will. No. No. Okay. I thought I saw it install Ubuntu at the command prompt type. Okay. Yes. I'm highlighting it, and then I will go over here and actually copy
[21:54] it. Give me just a second. Go right here. There we go. >> Usage is the WSL. >> What if you just run, like, type WSL.exe
[22:46] in the command prompt? >> The same thing again. It's giving the arguments. I'm going to go to the first one really quick. And make this go up. There we go. When I did
[23:12] the dot dot list, it did the usage of WSL.exe. Oh, no space. Okay. >> You just want this? >> No. So, you want WSL and then a space and
[23:38] then dash dash list. There we go. Yeah. So, it's listing the distributions, or it's supposed to be, but if no options are specified, the recommended features will be installed along
[23:52] with the what happens if you do install again? Like, WSL space dash dash install. I don't know. Yeah. Okay. So, you're not running as admin again. Here we go.
[24:17] So, now what happens if you just run WSL? Like, just WSL enter? No? Okay. >> Yeah. It's just bringing up the same thing. I can try the install again.
[24:48] >> Yeah. We're definitely in admin right now. So, something should happen. Oh, we're going to go full screen, y'all. >> That's what I thought. Windows wants you
[25:11] to restart after every damn thing, I feel like. >> Yeah. >> So, you can make a new folder without using
[25:25] the command line. If you want. In order to not lose the stream. >> That's dumb. WSL. You kind of or Microsoft. >> No, that's it. It's Windows' fault.
[25:46] >> Yeah. Like, should make a folder. Okay. We're going to do regular, but we'll find out then I need to, like, figure out how to actually change folders. Change folders. CMD.
[26:19] >> Because it was objecting to that earlier. >> Yeah. And to show folder. >> Yeah. It was objecting to LS. >> Yeah. It was objecting to LS and objecting
[26:33] to CD. >> It totally was. Yeah. Okay. So, you might do okay. Yeah. Good idea. Okay. So, now it's fine. I don't know why it was itching earlier.
[26:48] Okay. You'll have to make oh, you've already got one. Never mind. >> This directory listing is a Unix fan. Oh, okay. There we go. We have to use
[27:02] >> Yeah. >> Okay. >> That's why I was trying to get us into WSL. >> All right. We are learning. We're
[27:09] getting there. So, MKIR. >> You've transposed the K and the D. MKDIR >> Oh, thank you. Ooh. Yay. And we will call this Python. Just in case I
[27:38] >> Oh. So, maybe not. Because you might also want to be able to have a directory for the Python programming language to live in. And it would probably be better for that to be
[27:51] called Python. This is within the code directory. So, it wouldn't have actually confused the computer, but it could confuse a human. >> Yeah.
[28:18] >> In the future. >> All right. We have made the folder and learned lots. Then I can go back to this. And y'all, I know I'm doing this a little
[28:28] slower than most people would probably want. It's because I keep getting talked through how to clone and download and upload. So, I am trying to do this for myself with, you
[28:47] know, assistance, but mostly, like, you know, doing the research myself. So, if I remember, I want this for to download it. And I'm in the proper folder. And I hit paste. Yay. And
[29:12] then CD learning Python. Ah. >> I don't think there's a yeah, you got it. I'll give you a bash shell. Oh. Nice. I did download it for Windows, I thought. Let's
[29:49] see. Yes. I did download it for Windows. And then it gave me this manual of, like, getting started with them. And >> And so, that's what you were literally
[30:05] using. Because what you had there was with the command that you ran, can you is GitHub repo clone. And I was thinking, wow, that's interesting. I've never seen that syntax before.
[30:20] I usually would use git clone and then the URL of the repo. So, that's why. >> And thank you, Frank, for the directory. Because then I was able to look that up for
[30:36] the DIR. But then CD learning Python. Okay. There we go. And then I want to do code space dot dot dot code. Right? Code dot space. Wait. >> Yeah. It would be code dot space. What
[31:02] the space and the dot do or rather what the dot does is it says everything in this directory open up in VS code. >> We made it. We have made it. Okay. So,
[31:18] that made sense for cloning it. So, we now have it on the computer. That took a bit. But we made it. Okay. And now we go back to this one. We could you oh, there we go.
[31:42] >> Oh, and just for the sake of knowing terminology that other people would be using and so on, we wouldn't refer to this usually as downloading or uploading. That is what's going on. But
[31:58] sort of in this context, we would refer to it as, like, cloning and pulling. You, like, pull from a repo or you push to a repo. >> The words you say make sense.
[32:13] >> Mm hmm. >> Would this then is this a branch that it created because I did the pull and clone? >> It created the branch when you created
[32:25] the repo. You can't really have a repo without a branch. It would be like a building without a door. >> That's kind of fun. Okay. All right. I
[32:40] feel like I have more questions on this, but I don't know how to ask them or examples to use. So, we're going to skip that question. But all right. So, when we left off last time,
[32:58] we were mixing Boolean and comparison operators. I am going to see if I can go to the last part. Because we were oh, there we go. Talking about the actual graphs first before we started
[33:17] trying to code any of it. So, that way flowcharts. Yeah. The flowcharts. So, that way it was understanding the concept and then going through to do the coding part.
[33:33] >> Right. Visualizing the flow control. >> Yes. And we went through values. Equal to, not equal to. And again, I'm going to post this in messages for anybody that's joining
[34:09] us now. Okay. So, this again is going through more this is what I like to call more theory based at the moment because we're learning the concepts instead of actually coding. And
[34:28] at the moment, I am working on just finding where we were last time. The difference between double equals and equals. The double equals equal to asks whether or not the two values
[34:42] are the same as each other. The operator assignment puts the value on the right into the variable on the left. That makes sense. And I know we went through that last time.
[34:56] >> Mm hmm. Still went through all of this. Do, do, do. Unlike the and, and, or, the not operator operates on only one Boolean value or expression. This makes it a unary?
[35:29] >> Like a unicycle is a one wheeled. >> Oh, yeah, yeah, yeah. The not operator simply evaluates the opposite Boolean value. So, not true is false. Not, not, not true
[35:46] is true. Okay. >> So, do you want to see why that is the case? >> Because there's four of them. So, they cancel
[36:02] out. But if there were five, it would be false? >> Mm hmm. If you have an even number of nots, they're going to not, not each other. You're going to be able to pair up two nots that
[36:13] are going to cancel each other out. But if you have an odd number, then there's always going to be one left. >> So, it would be the same as if there was,
[36:22] yeah. If there were five or one, if they're odd, okay. That part makes sense. We just talked about the not true is false and not false is true. And this is making sense. And
[36:51] then the way I believe this is kind of where we left off in this image right here of four is less than five. And five is less than six. So, it would only do the first equation. So,
[37:11] four is less than five. So, it's true. And then it does the second equation, five is less than six is true. So, true and true makes true. >> Exactly. >> All right. And then conditions.
[37:33] The Boolean expressions you've seen so far could all be considered conditions, which are the same thing as expressions. Condition is just a more specific name in the context
[37:44] of the flow control statements. Conditions always evaluate down to a Boolean value, true or false. A flow control statement decides what to do based on whether its condition
[37:59] is true or false. And almost every flow control statement is a condition. >> So, like in English, we often colloquially say, like refer to the conditions, like the weather as the conditions.
[38:18] What are the conditions? And it's like, well, if it's raining, then you want to bring an umbrella or something like that. So, if the condition is this, then blah, blah, blah.
[38:31] And so, we actually use that in human language all the time. And it's exactly the same thing. >> But an expression could be just, it is raining, where a condition is, it's raining,
[38:52] so bring an umbrella. >> A condition is something that can be true or false, like it is raining or it is sunny, that kind of thing. And an expression, like,
[39:12] so those are examples of expressions, but they're not the only expressions. That part's not too important about what is an expression and what's not.
[39:23] >> Okay. So, lines of Python code can be grouped together in blocks. You can tell when a block begins and ends from the indentation of lines of code. There are three rules for blocks.
[39:40] Blocks begin when an indentation increases. Blocks can contain other blocks. Blocks end when the indentation decreases to zero or the containing blocks indentation. Blocks
[39:55] are easier to understand by looking at some indented code. Oh. So, if that's the case, then we could come over here to the code that we had. And it would be indented here. And
[40:20] then. >> So, what is your goal for indenting some of these? >> So, I was all of the prints, I'm indenting
[40:41] why are you indenting twice? There you go. Indenting once. So, that way they know that they're part of this one down here. So, like, this is a start. This is the end. So, all
[40:56] these prints are within it. But these, my name, the year, and your age are all part of the print above. But it doesn't like that. >> So, the indentation is communication. So,
[41:14] like, there isn't because you don't need to nest those print statements beneath that first print statement. It's saying, please don't do this. Because this isn't communicating
[41:27] anything to me. It's a bit like in how does it work in Java? I'm trying to think of languages where it's not indentation dependent. But I think it is in JavaScript. So, if you look
[41:47] at the example in the browser, I'm pointing at it like that. Makes any sense? >> It worked for me. I was going to get there. >> So, we've got the first three lines are
[42:00] all at the same indentation level. Right? But then the next one, after if name is equal to Mary, then we have an indentation to say this print statement is part of that if conditional.
[42:16] So, if this is true, if name is equal to Mary, then we have some things that we can do with that. So, those are all part of that if statement. >> Yeah, because it doesn't like this either.
[42:33] So, it was correct beforehand. So, it would have no indents. >> That's right. All of these are at the same level of indentation.
[42:47] >> My mind doesn't like that. >> Okay. >> I understand what you're saying and agree. It's more of like if I'm thinking of it as
[43:00] like an email or something, you know, when you're like it's a sub of this. It's because your instincts are super spot on because what you're thinking of eventually
[43:11] we're going to make into functions. And it will indent exactly as you were sort of as you were intuiting. We're going to get there, just not there yet. But you are exactly that's
[43:22] exactly the way that we want to be thinking. That's the direction we want to be thinking in. >> Yes.
[43:28] >> Thank you. Okay. So, in the previous so, program execution in the previous chapters, hello.py program, Python started executing instructions at the top of the program going
[43:47] down one after another. The program execution or simply execution is a term for the current instruction being executed. If you print the source code on paper and put the finger on
[44:02] your finger on each line as it's executed, you can think of your finger as the program execution. Not all programs execute by simply going straight down. However, if you use your
[44:14] finger to trace through a program with flow control statements, you'll likely find yourself jumping around the source code based on the condition and you'll probably skip entire
[44:25] clauses. That makes sense. Like, if I wanted to do the, like, hello, beautiful humans, if your name was Mary, then it's lovely to meet you, Mary. If it's not Mary, bye, not
[44:46] Mary. >> Sure. Exactly. Yep. >> Okay. The most common >> We did actually read through almost all
[44:56] of this last time. I don't know if you want to be just reviewing it or if you want to finish this chapter today. What are your goals? And that's read as else if. It's an abbreviation
[45:09] for else if. >> I feel like it's bringing it all back. Yeah, because I remember the vampire one. And you explained why it had to be greater than 2,000.
[45:26] Okay. >> More like why the greater than 2,000 had to come first. >> Oh, yeah, because the greater than 2,000
[45:39] or like greater than 100, then you are not Alice, Granny. And then if you do greater than 2,000, you're an immortal vampire. That totally makes sense of why they had to come
[45:58] in that order. Now, I do not remember >> This is new. We didn't talk about while loops last time. >> Sweet. While loops, you can make a block
[46:10] of code execute over and over again using a while statement. The code in a while clause will be executed as long as the while statement's condition is true. And code a while statement
[46:26] always consists of the following, the keyword, the while keyword, a condition that is an expression that evaluates true or false, a colon starting on the line that is intended
[46:42] in indented block of code, cause the while clause. You can see that a while statement looks similar to an if statement. The difference is in how they behave at the end of an if
[46:55] clause, the program execution continues after the if statement. But if but at the end of a while clause, the program execution jumps back to the start of the while statement.
[47:09] The while clause is often called the while loop or just the loop. How would you turn off a loop then? >> So look at what they've got here. So we've
[47:33] got the same idea expressed in two different ways. We've got it using an if statement and we've got it using a while statement. So these are both totally legit ways of doing the same
[47:49] thing. So we start off with spam is zero. And then if spam is less than five, we're going to print hello world and then we're going to add one to spam. We're going to go
[48:04] back up to the top of our if statement. If it's less than five. So now what is spam? What's the value of spam? >> One.
[48:14] >> Yeah. So what's going to happen? >> It'll be, it'll turn in, well in the while it would turn into two. >> Both of them.
[48:29] >> How would this one know to restart at the beginning? >> Oh, sorry. Never mind. That's, that's, you are exactly correct. And I, what I said
[48:39] was exactly incorrect. So yeah, so this, this, the if statement does stop and the while does not. And so that's, those are like two different use cases for the same. What we can see is
[48:53] inside those indentations, we've got exactly the same code, but different things are going to occur. >> And how would the while one know when it's
[49:06] going to stop? >> What condition is it evaluating? >> Oh, while spam is less than five. So once it hits five, it'll stop.
[49:21] >> That's right. >> Oh, okay. Okay. This is making more sense. >> Yep. >> An annoying while loop. Here's a small
[49:36] example of a program that will keep asking you to type literally your name. Select a file new, open a file editor, and enter the following code and save the file your name.py.
[49:51] >> All right. Let's do, I want to do new. There you go. Oh, wrong, wrong button. Oh. So in general, I do recommend typing the code, like especially like if it's not, you know,
[50:25] live. I recommend typing it instead of copying and pasting it, because it helps get those neural pathways in your brain. >> I love Laura's teaching style, too. She's
[50:53] the first one that, like, I've done this with, like, I've had career coaches or, like, she does have the perfect podcast voice. She really does.
[51:05] >> Oh, this isn't my voice. This is my voice when my lungs are damaged. >> No, it's still your voice. It's a little bit raspier, but not, it's still, you have,
[51:18] like, the best deep, like, enriching voice. >> Oh, thank you. >> Yeah. It's, but you, you're one of the first people since being on the show that
[51:29] I can say I hate you or glare at you or give you a lot of mean pushback, and you're just, like, you're still going to have to figure it out, because you know that it's me being
[51:41] frustrated as a student, not, like, anything personal to somebody teaching me. >> Absolutely. >> And I love that, because you make me work
[51:52] harder, and then I remember it more. >> It's a thing. It's a thing. >> It is a thing, and I just want to, I agree with all of them, so thank you.
[52:04] >> You're welcome. >> Okay. And you answer a lot of the why questions, which I really struggle with. >> Same, and that's, that's, that's why we're
[52:21] compatible, because in a lot of ways, our brains work in the same ways. >> Oh, it invented it itself. >> Yes.
[52:30] >> Prettier for the win. >> That is probably, I'm going to guess that's not specifically because of prettier, but it's because you, it knows that this should
[52:42] be Python. Although we are going to need to select interpreter, but we don't have to do that at this moment. We can wait a minute. >> Why don't you go?
[53:04] >> Me and a Windows keyboard. I'm so excited when I get my laptop back. Hopefully it works this time. Oh, I love it. >> Yes. Way to go, Laura. Name, input, ease?
[53:38] Okay. And, no, that wasn't going to let me, I was seeing if it would like let me rename it from there. I want to name you. Oh, there we go. No, no, I don't remember. Ah! Could
[54:14] you, like, rude. Okay. Well, y'all, I'm taking it to another screen to type. Okay. Save. Okay. >> So, before you run it, and actually you
[54:40] can't run it yet because we haven't selected an interpreter. But before you run it, let's just talk through what's going on on these lines of code. So, we can predict, like, this
[54:56] is one of the best ways to learn is before we run the code and see what's going to happen, we see if we can correctly predict what's going to happen. If that makes sense?
[55:11] >> Mm hmm. And I'm guessing also by the way it wrote in an annoying while loop is that no matter how many times you enter your name, it's just going to keep going.
[55:26] >> So let's figure out, let's see if we can figure out why. Why that's going to be true. Because it doesn't have a stopping point. Like, the one up here had a stopping point.
[55:41] >> There is a way to make it stop. So, let's do the let's okay. I'm going to be pushy and I'm going to say we're literally just going to look at each line of code and we're going
[55:51] to examine it and see what's happening. Because there is a way to stop this. >> If we put a value in name? >> We will. So, on line 1, what are we doing?
[56:05] We're saying name equals >> Anything. >> Yeah. Actually, a very specific thing. An empty string.
[56:16] >> Wouldn't an empty string be anything, though? >> Well, no. Because, like, 5 is a thing. But it's not an empty string. >> So, an empty string would be like if it
[56:33] asks for your name and you just hit enter, that would give it an empty string? >> It would not change the fact that it's already an empty string. So, then on line
[56:47] 2, we're saying so while name is oh, you read it. Sorry. >> Yeah. Because you've got to save your voice. While name is not equal to your name, print
[57:08] please type your name. Name equals input. And which is open. So, then it will print thank you. So, oh, so are they saying that while your name is not your name? So, if you
[57:23] type your name, it will stop. >> Yes, it will. You got it. >> All right. So, I need to will this work? If I just do it right here?
[57:50] >> I don't know. Oh, yeah, yeah, yeah. Right. So, this is a way to run it in the browser. So, this isn't the code that you wrote. This is this the exact same program lives on this
[58:07] Python tutor.com. It was already saved here. So, it wouldn't matter what you had typed in your in VS code. This would still look exactly like this.
[58:23] >> So, he typed your name and it ended it. Whereas if he kept writing Al, it would keep going. No, this is a very useful tool called Python Tutor.
[58:44] >> So, that's because he's already saved this exact program here. >> Yeah. >> But if anybody like Jay always he has the
[58:55] like Python newsletter. If he wanted to write something to give a demonstration or something, he could use this. >> Sure.
[59:06] >> Ramon, oh, my God. OMG. I use this for visualizing JavaScript for the learners all the time. It's magnificent. >> What's really neat about this is that it's
[59:31] showing the green lines, the green, sorry, arrows show the line that you just executed. If you click start again, it's going to go through it. Interesting. Wait.
[59:51] >> Nope. >> Not that. Go back. Sorry, my bad. I told you to do the wrong thing. Yep. Where is it? Sorry. Next. If you click next. So, it will
[60:14] keep moving that arrow to show you which line is green line is being executed. The red line is the next one. And if we keep clicking next, it will keep showing us which line we're executing
[60:27] each time. So, first we executed the print, please type your name. And then put in L. And that is not equal to the string your name. And so, we go back through.
[60:43] >> It's weird that it has this here, too. Oh, Visual X, it says right here. I was confused why Ramon said he was using it for JavaScript. And it says right here you can use it for
[60:57] JavaScript. Okay. That totally makes way more sense. Oh. I like this. Okay. Okay. But let's try it again in your editor so that you can run it on your machine. So, we need
[61:23] to we need to select an interpreter. If you look at the bottom in sort of like a dark mustard. Yeah. Okay. So, okay. So, Python is not installed. That's because we installed
[61:37] Python maybe two streams ago, but that was on your Mac. And so, now we need to install it on Windows. >> This is such a weird process.
[61:52] >> Why? >> Like you have to know everything that you need to download and remember it all to go machine to machine. So, like what if you have
[62:04] like I guess like if you install if you're getting it from GitHub and like cloning it and then reuploading it, you can do it on two computers. But it would be like really
[62:18] frustrating if you don't. Yeah. >> Yeah. Your dev environment is what you're setting up right now. And yeah. So, that can be really frustrating moving from computer
[62:32] to computer. And there are ways of making that a bit less painful. As Ramon is saying that this is making a good case for cloud coding. So, if we were working in VS code
[62:49] in the browser, we'd be okay. We wouldn't need to be doing that. But the reason that I'm not saying, hey, we should just do that is because if you want to be able you know
[63:01] if you're going to be doing this as like for your job, then you have to be able to do it locally for most positions, I would think. >> Got it. Okay. And Ramon gave us some options.
[63:18] Gitpod, GitHub, Codespaces, StackBlitz, et cetera. I dig it. All right. So, now and then now I can hit play, right? Yeah. Run Python. >> Run. In this context, we would say run
[63:35] instead of play. But yes, exactly. >> I'm not giving you this. Look, I'm giving the developers. It's a play button. >> We're running the program.
[63:46] >> Yes. Okay. So, please type your name. And if I type Jen. And Nora. And Ramon. Ta da. And then if I say you're actually I'm going to do this just to see it. So, it doesn't
[64:10] do it. >> Right. So, what you were just doing was you were testing what we would call sort of not exactly an edge case, but it's something
[64:18] pretty similar to an edge case where you were checking, hey, will it be will it be really precise in looking for matching the case? Like uppercase versus the lowercase. And that
[64:31] is exactly the kind of instinct that you need for writing good code. >> Oh. Yay. Okay. So, we have gotten through here. And we figured out how to turn it off.
[64:51] And then a break statement. I just want to see this actually work. I like that these are starting to be in there. Because I feel like it's easier visualization than like not
[65:13] everyone is going to have a Laura. So, these at least help a bit. >> Absolutely. This scales and I don't. Not that I'm the only person who teaches Python.
[65:30] But, you know, you can for everyone, you could probably find a tutor or start your own livestream. I think everybody >> Read this book.
[65:41] >> Yeah, read this book. >> This is how I learned Python. >> Yes. Yes. You can tweet people like us and we will reply with answers if needed.
[65:50] What are you guys talking about? Locally would be great to use dot files in a repo. Good point. And, in fact, okay. There we go. And then good point. And, in fact, some of these
[66:10] are cloud platform support examples of VX code dot files. It's great there are so many tools. Oh, my gosh. Yes. It's very overwhelming. >> Yeah. So, we could we could talk about
[66:29] dot files, if you want. Or we could do that on a future stream, if you want to try to get to the end of this chapter today. >> Yeah. Let's do that. So, I'm going to ignore
[66:41] it for a second. But work on remembering it. So, I'm going through this kind of fast because I want to see what it does for the break. I don't understand.
[66:56] >> So, let's look at the difference between this program's code and the previous one. >> If name is equal to. >> So, here we have that condition. Instead
[67:12] of having that condition in up next to the while, like because in the previous program, it was while name is not equal to your name, do this stuff. And here it just says while
[67:29] true. So, if you have while true and you have no break statement, true is always true. And so, it would be what's called an infinite loop. Nothing would ever stop it.
[67:41] >> And if the name is equal to your name. >> Oops. Did my headphones disconnect again? What's going on here? Okay. We're connected again. Sorry about that.
[68:16] >> All good. You're at least having less computer issues than I am. So, I appreciate your patience. This one does make sense. So, this one is definitely and then because we entered your
[68:35] name, it broke the while and it printed thank you. So, that's what a break. Okay. And I'm going to keep going. Keep going. Continue statements. Like break statements, continue
[68:53] statements are used inside loops. While the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop and reevaluates the
[69:04] loop's condition. So, I'm guessing okay. Oh. So, like in this one, they're using a password. So, if they use the wrong password, it would continue to the front. Or continue to the
[69:22] beginning. >> Yeah. To the top of the loop. Yeah. >> But if they wanted to this is where they would add more to say like 3 passwords and
[69:36] it's wrong. Or like 3 attempts. They would add that here too. How would you add that, I think is my question. >> Yeah. So, you would need to create your
[69:56] while loop maybe instead of saying while true or like you'd have to say like you'd have to create a variable that would be storing the number of attempts. And incrementing that
[70:14] number of attempts with each attempt that was made. And then like while number of attempts is less than 4. Or usually because we do what's called 0 indexing. So, usually we start in
[70:30] programming we start our numbers or our counters at 0. So, in that case you would actually say while number of attempts is less than 3. Because the first one would be 0. And the
[70:46] second one would be 1. And the third one would be 3. >> That makes sense. And that's making me think of some React web apps that I've made.
[71:00] Has the counter automatically built in as the like default. So, and then being able to see what the counter does. And the counter it does count like just the page visits. But
[71:12] I can see the similarities of that to password attempts. Totally different code and I'm talking different languages. But conceptually. >> Exactly. Different ways to use the same
[71:27] concepts. Which is great. >> Nice. Wait. What is what are you guys talking about? Oh. Yeah. When she gets off her MacBook. Distractor mode off. Thank you, everyone.
[71:45] Thank you. All right. This is talking about what we just talked about. Truthy falsy values. I like truthy falsy values. That sounds way more interesting. Conditions will consider
[72:02] some of the value in other data types equivalent to true and false. When used in conditions, 0, 0.0 and empty string are considered false where other values are considered true. Okay.
[72:33] I feel like a lot of this now is they all generally kind of make sense. It's just gonna be more of I'm just scrolling down to see if there's anything totally crazy. No, that
[73:00] makes sense. Because importing modules, I'm guessing, is they're just importing built in functions. Okay. I've done that. I think in JavaScript. >> Very possibly. Yeah. I think
[73:22] of it like if you have you're putting together your toolkit or something and you're like, okay, I'm going to need today I'm going to be building something. So I need to bring
[73:36] my like building module. So I'm going to put that in my toolkit. But I'm also going to need to be doing some plumbing. So I need to bring like my plumbing kit. I need to put
[73:47] that in my toolbox, too. That kind of thing. Like different modules will be for different purposes. So you don't but you don't have to bring everything with you. Because that
[74:00] would be super heavy. >> Got it. Yeah, that makes sense. >> You only want to bring with you the stuff that you're going to use. >> I just want to agree with this. And this
[74:10] is why I named this project after Laura. I agree with that. Okay. >> So I feel like you're getting to a point where we can do what I like to do when I'm learning something is
[74:30] to just sort of skim exactly like you're doing. Skim like headings and see if anything sort of jumps out at me. But then otherwise I want to just go directly to the exercises. >> And
[74:45] I think that's where I'm at. But I really like that we were starting the exercises at the beginning of the next session. Because then it's like, do I actually remember it
[74:59] and build off of there? And then I get that it's taken us longer to go through the chapters that way. But I feel like I'm remembering a lot more of the previous one. So I am going
[75:17] to start wrapping us up, y'all. I have practice questions for next week. Does anyone have any questions? You can find Laura on her Twitter. Her Twitter is there. And her stream. Also,
[75:35] we are streaming to both places right now. And that is let me go grab your stream. To make sure that it's in here. There we go. Now I'm like, I need to make sure that I'm
[75:57] actually following you. Because that would make me sad if I'm not. Yay. Thanks, Frank. Come join us. We're here every other Monday. Laura, what is your stream? Apparently I don't
[76:29] know. I can't use the regular comments. I can just do private chat. Okay. Oh, that's why. I always forget that. Until I see it, like you're chatting in. And then I'm like,
[76:49] oh, yeah. That's what it is. All right, everybody. Here is Laura's info. Please follow both of us. Feel free to subscribe as well. And we will see you soon. This is very exciting that
[77:07] we have we are learning more and more about Python. These are things that we definitely want to know your questions to. So, either comment, you know, if you can't catch one
[77:20] of them here, please feel free to comment on YouTube or tweet us. We will do our best to get back to you. And thank you, everyone. Bye!
[77:33] Bye! 
