---
showLink: "https://www.youtube.com/watch?v=VLSfoBxWFgg"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-python-basics-with-guest-laura-langdon"
title: "Teach Jenn Python Basics with Guest Laura Langdon"
publishDate: "2022-08-29"
coverImage: "https://i.ytimg.com/vi/VLSfoBxWFgg/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome back to Teach Gen Tech,
[00:06] and we have a guest coming back. Laura is teaching us about Python.
[00:13] I'm not as scared as I was last time, which I'm pretty excited about.
[00:18] Now, Laura, can you introduce yourself and give us an idea of your path and what you work on with Python?
[00:27] >> Yeah. I'm Laura. I'm a Technical Writer at SubOrbital Software Systems,
[00:32] and before that, I was a math professor. I don't actually work with Python professionally at all.
[00:41] We don't do Python at SubOrbital. I am learning Go for what we do at SubOrbital.
[00:48] But before I became a technical writer, I thought I was going to become a data scientist.
[00:54] So for that, I definitely needed to learn the Python. There are lots of different things you can do with Python,
[01:03] and one of them is data science, and another is you can do web apps.
[01:08] You can deploy web apps with Python through Flask and Django and so on.
[01:12] I don't know anything about that. I know about it from the data science side of things.
[01:16] There are probably more things besides that you can do with Python,
[01:20] but I know about it from the data science. >> I just linked your video in the comments,
[01:26] but I'm also going to link another video that I did later that week
[01:33] on why build in JavaScript versus Python. In my head, that means why would you choose each one?
[01:42] What it came out as when Ian came on is he's like, "I don't know why you would build in
[01:47] JavaScript instead of Python." I'm like, "I get that's what I wrote,
[01:52] but that's not what I meant. I meant what do you use each for?"
[01:56] So that video is also going to be commented. There we go.
[02:03] But it was really insightful seeing how there are other things that we can use Python for,
[02:10] and that Python and JavaScript can do a lot of the same things now where in the past,
[02:16] it wasn't really as well-known as what they could do, from my understanding.
[02:22] >> Okay, sure. >> Which I think is pretty cool, but all right.
[02:27] Well, I know that last time as a quick recap, let me share my screensol.
[02:38] That's not a word, but I'm going to go with it. >> Works for me.
[02:42] >> We started using Automate, the boring stuff with Python.
[02:47] How do you say Al's last name? You said it so well last time you were like, "I got this."
[02:52] >> I mean, I made it up, but I think it's Swigert.
[02:54] >> All right. I dig it. We started through the,
[03:00] I'm just quickly scrolling up. What up, Akari?
[03:05] >> Hey, Akari. >> The first one of just like,
[03:10] "Hey, we're going through this. What's this book for?"
[03:13] Then, "What is programming? What is Python?"
[03:17] It says you don't need to do math, but we got to part like Chapter 1,
[03:22] and I freaked out because there's a lot of math. But we got a math teacher here,
[03:26] so I feel like we'll be okay. We got to installing Python.
[03:33] I think it's, yeah, downloading and installing. What up, Noel?
[03:40] >> In downloading and installing Python, I got really stuck on never realizing that NPM was for JavaScript,
[03:50] PIP is for Python, and then y'all in the chat,
[03:57] what other programs have their installs? What are their names? Do you know what they use for Go, Laura?
[04:06] >> Actually, no. I haven't gotten as far as installing any non-native libraries for Go.
[04:15] But for Rust, it's Cargo, and I thought that that was super cute,
[04:21] like you're loading cargo. There were names, I can't remember,
[04:26] it's been a couple of months, but there were names for things and it was like,
[04:30] it just totally worked for me, the idea of loading cargo into a truck or on a train or whatever,
[04:37] because that's exactly what you're doing. You're picking the thing up and you're putting it in what you're working with.
[04:42] >> Yeah, and I remember Ramon talking about Rust and Cargo, and I did not realize that those were a thing for all different languages,
[04:57] and now that I'm comprehending that a bit more, I'm like, "Okay, Python isn't necessarily weird,
[05:03] it's the fact that I'm learning my first new language." >> That's right.
[05:07] >> Those were some revelations from the last one, and we went and downloaded and installed Mew,
[05:19] and we installed Idle. I know we did, I don't remember what Idle does,
[05:25] but we did install it and we're going to go to the next chapter because that was a lot of texts to go through.
[05:36] >> Yeah. >> Another thing that I did for my own learning process,
[05:40] which I think is just a great call out for others, is I personally do not read text very well.
[05:48] Yes, teachers do roll. She was a math professor.
[05:52] >> Indeed. >> Which is cool. We talked about how algebra,
[05:57] last time we talked about how algebra, like so many people had to take algebra in college many, many times.
[06:04] >> Including math teacher. >> I'm very grateful for that.
[06:08] One thing I learned is that I myself do not read very well. It's very hard for me to really comprehend it if I read it.
[06:19] Meaning that when we were going through this last time, I'm trying to read it to find the directions and I'm getting lost and embarrassed.
[06:29] A lot of it is because I'm staying so focused on making sure that I read the right line and I'm reading the word that I'm not comprehending what I'm reading.
[06:39] Today, I got through a lot of this and did my text-to-voice on here. That way, I could learn,
[06:52] get a head start on comprehending a lot of what we go over. That way, I'm not trying to hide the fact that I'm reading this while we're live.
[07:03] I'm failing at reading it. I got mew going.
[07:10] Then it looks like it loaded the file that we had. I'm pressing F5.
[07:21] Now, I think this was a part that I was stuck on, is we were also using,
[07:29] was it idle that we were using? That's like in the browser, it's like inspect.
[07:37] >> I can't remember. I don't personally use idle and I can't remember what it is.
[07:45] >> I think it was this. >> Yeah, rebel, the read,
[07:51] evaluate, print loop, I think. Yeah. >> Yeah. Okay. This is where I was getting confused because yeah,
[07:58] it's rebel that we can do in the browser and hey, Jay. I like tag Jay on this one on LinkedIn
[08:15] because he does Python and I was watching his stream last week, and I was just like, I have no idea what's going on.
[08:26] But is this, anybody else experience this when you watch one of your friends that are live streaming?
[08:31] It's like calming because I'm like, oh, I can do my work too,
[08:35] but they're there if something catches my interest and I can ask a question.
[08:39] >> Totally. >> I don't know if that's everyone,
[08:42] but that was a cool experience last week. Okay. Now, into interactive shell,
[08:52] we have to hit "Run" or press F5. >> Okay.
[09:00] >> So it divided it out. We got three windows going.
[09:06] Well, that's fun. Yeah, I honestly don't even think we got to this point last time.
[09:13] >> I mean, sort of. We were working in the rebel.
[09:17] >> Yes. >> Right. Rebel, from last time,
[09:21] we learned that rebel is not a Python thing, it's an everything thing.
[09:26] >> This is a rebel. >> Yeah, that's what I want to see.
[09:35] It gave the solution down there at the bottom. It is, this is a rebel.
[09:40] It's not called, I don't think I ever would have known that in case somebody told me,
[09:45] because it's called inspects, and it says rebel nowhere.
[09:50] >> Yeah. I mean, I don't know if this would actually be called inspect so much as this is
[09:56] how you get to it by clicking "Inspect". But I wouldn't say the name is inspect.
[10:04] >> Yeah. >> It's name would probably be console.
[10:08] >> Interesting. All right. >> So we got that far and then expressions and operate, okay.
[10:25] >> Yeah. >> And errors are okay.
[10:27] I know we talked about this quite a while. Then this is where I started going.
[10:34] I don't even really understand the first three. >> Okay.
[10:39] >> The next four, I'm like, "Hey, I actually get that."
[10:43] But the first three, I'm like, as soon as we saw it last time, I was like,
[10:47] I think I understand like modulus remainder. Like what I'm guessing that one is,
[10:57] what is eight percent of 22? >> No. You would think so because it has that percent symbol,
[11:06] but modulus means remainder. So 22 mod eight,
[11:15] that's how you would read that example. That means that if you divide eight,
[11:24] or if you try to fit eight into 22, you're going to end up having six bits left over.
[11:34] So if you have 22 of a thing, 22 pieces of Lego,
[11:41] say we got 22 bits of Lego, and you want to divide them into groups of eight.
[11:49] So we grab eight of our 22 pieces of Lego. We've got one group of eight.
[11:55] >> Okay. >> Okay. We still have some leftover.
[12:01] We can grab another group of eight. We've got two groups of eight now, that's 16.
[12:07] But there isn't enough for another group of eight because there are only six pieces of Lego left.
[12:18] >> That's making sense. That totally makes sense.
[12:23] Instead of turning it into a fraction or a decibel, it's just like what is the remainder?
[12:30] >> Yeah. >> I like that. That one's easier to comprehend.
[12:35] The other ones don't make sense to me for exponent and integer. >> So an exponent, what's two squared?
[12:48] >> Four? >> Yes.
[12:50] >> Okay. Hey, I remember. That's exciting. >> Yeah. So that's an exponent.
[12:54] In that case, the exponent was two. It's a bad example because there are two twos,
[13:02] two is the base and two is the exponent. But it's the one that people can remember using almost like muscle memory.
[13:09] Don't even have to think about it, two squared is four. That's the one I start with.
[13:13] But two cubed is the example here. So that means if you multiply two by itself,
[13:19] so you've got two times two times two, that's three twos. Two times two is four,
[13:25] four times two is eight, two cubed. The reason that we call it a cube is because that's how you get,
[13:37] if you multiply three numbers together, like if you think of a rectangle,
[13:41] it has a length times a width times a height, it's three-dimensional. What is it?
[13:50] It is a cube. So that's where the word cube comes from.
[13:58] >> So this would be two cubed three. >> Two cubed is eight.
[14:06] >> Two cubed is eight. >> Yeah. Two times two times two is eight.
[14:11] >> Why do we put the three here? >> So it's because you're multiplying the two three times.
[14:22] If you were multiplying the two 72 times, it would be two star star 72.
[14:30] >> So like this one over here that I did is seven star star three. So seven cubed is three, three, 43.
[14:40] >> That's right. So exponents are just shorthand, right? It's so that especially if you have an exponent that's bigger than two or three,
[14:52] it would start to get really tedious to write them all out. >> Yeah. Okay. So I'm starting to get that.
[15:01] Yeah. An exponent is cubed number, no. >> Cube is an example of an exponent.
[15:09] >> So like this one, so if I do like seven star star seven,
[15:16] that one's not cubed, it's seven. >> The seventh power. Yeah.
[15:20] >> Okay. Then is the integer the opposite of modules where eight can go into 22 twice? >> Yes.
[15:33] >> Yes. >> You got it.
[15:35] >> Do you remember something in math? >> Yeah.
[15:37] >> All right. This is very, very exciting. >> Yeah. So if you've got your 22 pieces of Lego,
[15:43] and you want to put them into groups of eight, you can do that two times with six leftover.
[15:50] So the integer division means what is the integer part, the whole number part, that's two,
[15:58] and the modulus is what's the other part, the remainder, that's six.
[16:03] >> So I'm just saying if you ever want to start a live stream, which is like teaching math,
[16:09] especially if you use Legos, like big Legos, I would definitely pay attention.
[16:15] >> Yeah? >> Yeah. I would watch that.
[16:18] I would definitely watch that. So thank you because I was staring at those,
[16:23] and I shut down last time we were streaming. I'm like, "Nope. Nope.
[16:28] Nope. This is too weird. This is too different.
[16:31] I can't do it." Well, and that's such a big thing about learning,
[16:36] and I love learning live because it's like, I get to set my own pace, for example,
[16:44] but school doesn't really do that. If I'm going, "Oh my God, it's overwhelmed.
[16:48] I don't understand." Not all classes or teachers
[16:52] are set up to be able to break this down, or is someone so self-aware to be able to go,
[16:59] "I don't know where I'm lost." >> Yeah.
[17:01] >> So thank you again for doing this. I think I did a lot of
[17:08] these just by getting excited while you were talking, understanding it.
[17:13] This is definitely where my dyslexia and I did not get along in math,
[17:22] which now I'm curious if I remember my order of operations. So you can do the five minus one,
[17:33] which would be four, and then you would do your seven plus one,
[17:37] which is eight, and your three minus one is two,
[17:41] and then you would do eight divided by two, is three, and four times three is 16.
[17:49] >> Wait, wait, wait. >> No, I'm doing it out loud.
[17:52] >> Why did you do the division first? >> After doing the three minus one?
[17:59] >> Because it's these parentheses, the big parentheses.
[18:04] >> Oh, sorry. Yes, you are totally right, and I was just staring at them.
[18:16] You are totally right. I'm sorry. >> Cool. But that also means that I'm learning
[18:21] something and somewhat paid attention in math class. >> Right. They're nested parentheses. Yeah.
[18:28] >> That's what they're called. >> All right.
[18:30] >> Yeah. >> I will say talking about this.
[18:31] >> Just like matryoshkas, like the little Russian dolls, right?
[18:35] >> Yes. >> Yeah.
[18:37] >> I like it. >> I come up with toy examples
[18:39] for everything in math apparently. >> I think it's a great way of learning it.
[18:43] It is. All right. So if we do these long ones,
[18:53] this just shows how it breaks it down compared to if I were to have to break it
[18:59] down myself like we just talked about. >> Exactly. It's showing you what you just did,
[19:03] what you already knew. >> All right. Well, I'm going to type this,
[19:07] so that way we can see it running. I think this is a good question to ask.
[19:15] I get that we have our REPL, and that one's showing us the numbers,
[19:21] and then we have our file itself. What I'm not getting is,
[19:28] why are these two plus twos not showing up? Is it because we don't have a print there?
[19:34] >> Yes, it is. >> Okay. So print, but this isn't going to,
[19:45] oh, it's syntax error. I like syntax errors.
[19:48] Errors are great. >> Yeah.
[19:51] >> Oh, so if I knew it'd be this way. Oh, it just put four.
[20:02] >> Because they're living there in those parentheses as integers, not as strings.
[20:16] So if what you wanted it to do was print the characters two plus two,
[20:22] you'd have to tell it, this is a string,
[20:26] not a math problem. >> I'm just curious if this is going to work.
[20:32] I don't know where my one is. That didn't work, so I would need [inaudible]
[20:44] >> Well, we'll get an error, and that's totally cool.
[20:47] Let's see what the error is. It's probably just going to be the same invalid syntax.
[20:52] Yeah. Okay. So what it doesn't like is that these are apples and oranges.
[21:02] We've got the string two plus two, and then also actually outside of the print parentheses.
[21:10] So print has parentheses around it, the print command. So what the computer is reading is it's saying,
[21:17] okay, what you want me to do is print this string two plus two, and then after that,
[21:22] we've got another two plus two, but I don't know what to do with this,
[21:26] because it's attached to the print statement, but it's not in the print statement.
[21:32] So it's like there's an orange glued to my apple and I don't know what to do with this.
[21:39] >> Yeah. >> If that makes sense.
[21:41] >> Yeah. >> So if you take that two plus two in parentheses off the end,
[21:49] it'll be happy. >> But then I won't show my two plus two.
[21:59] >> So then you would create another print statement. >> Can you do them on the same line?
[22:06] >> Yes. So that's called string concatenation. So like sticking them together,
[22:11] you can actually, well, okay. So what do you, let me think, what do you, okay.
[22:18] So this is, yeah, you would need to put it on a new line.
[22:24] If what you're trying to do is just say, actually, I'm not sure what it's going to do.
[22:27] Let's see what it's going to do. >> Oh, yeah, I don't like it.
[22:30] >> This wouldn't be the Pythonic way of writing this. Yeah, I think it probably wants it on a new line.
[22:40] So Python is unlike some languages. Like in JavaScript, you have to stick
[22:46] semicolons everywhere to say this is where my line ends. In Python, you don't have to do that.
[22:53] Instead, it infers that stuff by putting something on a new line or whitespace.
[23:03] So it'll actually, like indentation is going to matter. >> Okay.
[23:09] >> But we'll get there. >> Is there a way to put these all on one line?
[23:15] >> Yes, but they would need to be two strings. >> I will ask that later because, oh, hey,
[23:31] I'm just not doing things grammatically correct. It's talking about, okay.
[23:37] So this is where it starts talking about, I believe, like you can't do like,
[23:52] because these two, I'm reading out loud and comprehending. Indentation matters.
[24:01] You can do some goofy math from Jay. Jay, you were working on, oh gosh,
[24:11] it was a time, like date and time. >> Oh, like Cron?
[24:20] >> I don't know. What were you working on last week, Jay? Do you remember?
[24:27] It was your first live stream, not your second one. I couldn't check out the second one.
[24:34] >> Yeah. So what Jay is showing here is a printf statement. So that's like formatting.
[24:41] So that's sort of like a fancy way to print. >> Okay.
[24:45] >> You can print fancy stuff. >> I have to, like, this is probably
[24:50] the one thing I don't like about StreamYard is, I can't copy and paste from there.
[24:57] I have to go to actually go to Twitch and go copy and paste it. >> That's goofy.
[25:06] >> I also don't know how to run other than opening and closing. That's a fancy way.
[25:14] He was doing some date and time manipulation. >> Very cool. Yeah, it seems complicated.
[25:26] I was just having fun like going, "Whoa, that is even possible?
[25:29] That is cool." >> Yeah. So there are some projects,
[25:34] I think, in this book that do dates and times and stuff. It's been a minute, so I'm not totally sure, but I think so.
[25:42] >> That reminds me, I need to post this in the chat, the book we're using.
[25:48] >> Thank you for that reminder. We definitely ran into our syntax errors,
[25:55] which thank you for helping me go through this because I think that helped conceptualize it a bit more.
[26:02] You can also include all of it in a print string. Wait, include all of it in an F string.
[26:11] There we go. See if I can talk. Print F. I think this is the cool thing about programming,
[26:23] is if you can see how somebody else did it, then you can be like, "Oh,
[26:32] that's what I need," and then copy and paste it to try to learn how to do it yourself.
[26:38] >> Yeah. There are usually multiple ways to do all the things. >> Yes. I think that's a really cool part about,
[26:48] you know the author, Jay? Jay.
[26:55] >> Oh, neat. Yeah. Al seems like a super awesome human.
[27:01] >> I feel like we need to get Al on the stream. >> That would be exciting.
[27:08] >> That would be so cool. >> Yes. Everybody go follow Al.
[27:15] >> I said this last time that I ran into a question and DMed him on Twitter and he wrote back in 20 minutes.
[27:24] >> That is so cool. I think that is the really cool thing about Twitter.
[27:30] Yay, thank you, Jay. >> Oh, exciting. Thanks, Jay.
[27:34] >> It is the fact that there's so many people I would have never met if it were not for Twitter.
[27:43] In fact, I'm going to start playing D&D this week. I'm very excited.
[27:51] I don't know if we're live-streaming this week, but we'll be live-streaming next week,
[27:55] I think on Jacob's channel. Once I know when we start, I'll start posting it.
[28:00] >> This is so fun. I have Internet friends. >> Yay. We've got these data types,
[28:10] and these are the same data types that you already know from JavaScript.
[28:14] We have integers, those are like whole numbers, but also with zero and negatives.
[28:21] Floating point numbers, more or less, we can just map floating point to decimal, has decimal.
[28:29] >> Do I need to remember what these are called? >> I feel like that's a part of the way I've learned JavaScript,
[28:37] is I may know how to use all of these, but I never knew that they necessarily had a name.
[28:45] >> I'm trying to remember. In JavaScript, do you have to declare types?
[28:50] Because I think maybe you do. If you're declaring a variable,
[28:55] and it's going to be the number 5. >> Yeah. We don't have to write integer.
[29:01] You don't have to do that in Python either. Python is dynamically typed,
[29:05] and so it will infer from whatever you give it. If you say x equals 5,
[29:13] then it'll say, "Ah, then x is an integer." But in the very next line,
[29:17] you can say x equals gen in quotes, and it'll be like, "Oh, okay, cool."
[29:25] Now, x means a different thing, and that's because in Python,
[29:30] everything is a pointer. I don't know if you're familiar with pointers.
[29:36] >> No. >> Okay. A pointer literally is exactly what it sounds like.
[29:45] It tells you, what it says is, x points to this place in memory.
[29:51] It means I stuck this over here. X is like a flag saying, "It's over there."
[29:58] If you say x is 5, then it'll say, "Okay, it's pointing to
[30:01] this place in memory where it's 5." Then if you then say x equals gen, it'll say, "Okay.
[30:08] Now, we're going to point to a different place in memory, where it says gen," or like,
[30:11] "I've rewritten that place in memory, and that says gen." Yeah.
[30:16] >> I think I'm starting to get it. Bakari, you are on YouTube,
[30:21] so not everybody can show this. See this, can show this,
[30:25] can see this, see if I can talk. Jay said, "No, can do it.
[30:32] Don't need to do it in JavaScript." But Bakari said, "Only in TypeScript."
[30:38] Then Jay also said that, "You do it in TypeScript,"
[30:44] which I am learning later this week. I'm a little nervous.
[30:48] You can include types in Python to provide context. >> Yes.
[30:54] >> You don't have to provide types in Python, but you can if you want.
[31:02] Say you've got a function and it's going to return some value,
[31:06] you can specify the value that this function returns must be an integer,
[31:11] so that you can't accidentally have this function return a string,
[31:16] which would make no sense. So you can tell Python,
[31:21] this thing must be of this type, but you don't have to. Options.
[31:27] >> Okay. Jay also added, or if you're using a Python convention
[31:35] that expects you to add a type like data classes, like data classes, we're just going to end it there.
[31:41] Also Bakari, Jay says, "Hi." He probably didn't say it like that,
[31:47] but I like to paraphrase everybody and put a gen spin on the transition.
[31:55] I'm really bad at telephone. >> Oh, yeah.
[32:00] >> Thank you, Jay. All right. So Python programs
[32:13] also have text values called strings or strs.
[32:23] What is the difference between a string or a str? Are they the same thing?
[32:27] >> Nothing. It's just that when you are telling Python that something is,
[32:31] just like you've probably seen programs where in order to tell the computer
[32:37] that something is going to be an integer, you write int, I-N-T as shorthand for integer.
[32:43] In Python, str is the shorthand for string. So there's no difference.
[32:49] >> Got it. >> Str is just the shorthand for string,
[32:52] and float is the shorthand for floating point numbers. So it means exactly what you might want it to mean.
[33:01] >> Oh, goodness. All right. We're getting into it joins words together.
[33:11] >> Yes. >> So what I'm taking from this
[33:16] without grueling over all the text that tells me what it is, if you type two strings that are letters,
[33:27] then it will like Alice plus Bob equals Alice Bob. That makes sense. But if you do Alice plus 42,
[33:35] it's just going to go, what did you just do?
[33:39] >> So it's not because they're letters, it's because they're both strings.
[33:43] If that 42 had quotation marks around it, it would be fine. >> Okay.
[33:49] >> So let's try that. >> Now, do I need to do, okay.
[33:56] I think I know. >> 57. We need this and we need this.
[34:11] Then we need to find a better way to run it, but F5 is happiness,
[34:16] so we need print. >> That's right.
[34:20] >> Print. >> Print. Does it have to have the parentheses around it?
[34:26] >> Yes, it does. >> It does join it.
[34:37] >> Because they're both strings. So it's not a letters versus numbers situation,
[34:44] it's a string versus not string situation. >> Got it. Bukari came back over to Twitch and says, "Hi, Jay."
[34:56] >> No, but Jay just jumped to YouTube. >> Did Jay go to YouTube?
[35:01] >> Oh, dear. >> Oh, no. Everybody come to Twitch.
[35:04] Twitch is where it's at. It's a party on Twitch.
[35:07] As a heads up, and I think that is a great call-out, I will not be live-streaming to LinkedIn starting next week.
[35:17] I will only be live-streaming to Twitch and technically to YouTube, but that's only because I don't want to re-upload it.
[35:26] To get the word out there, I was definitely streaming to every platform.
[35:30] But as of Wednesday, Teach Gen Tech is two months old.
[35:36] >> Yay. >> It's birthday.
[35:38] >> It's his birthday. Oh, yay. All right.
[35:43] We got Jay and Bukari in the same chat room. >> Yay.
[35:48] >> It's okay. That is totally okay, Jay. That's what I was doing while you were live-streaming.
[35:55] Then I don't know if Noelle is still here. If Noelle, you're still here,
[36:01] hello again to you. Oh, you can multiply Alice's.
[36:09] Yes. Wait, now I have a more complicated thing that I'm going to copy. Wait. Yes, maybe.
[36:23] No. We do print. [inaudible]
[36:57] I need to multiply it times five. Would I still use this type of string if I want
[37:03] to add their names together and then multiply it by five? >> You could.
[37:11] I don't start people with F-strings. That's what that's called.
[37:23] Just because, at least for me, it took me a minute to wrap my head around
[37:30] formatted with formatting as opposed to just print exactly what's here, just works better in my head.
[37:37] But if the F-strings are working better in your head, that's cool too. >> I think the only reason they're working better in my head is because I know what I
[37:46] wanted to say and being able to understand where to get to that point. If I'm reading this one right,
[37:59] it's the F-string is two plus two is what the word is saying, and it's what that word is calculating whatever this equals.
[38:12] >> Yeah, the result of two plus two. >> This makes sense.
[38:18] I guess the part that I'm curious about on an F-string, which I guess I can just try to do things myself.
[38:26] Instead of asking questions to see if I could get it to work, I just think that always just takes so long.
[38:32] >> It is the most effective way to learn, I think, is just try shit and see what happens.
[38:40] >> I don't necessarily need it to have a word. I just need it to do, let's see.
[38:55] Let's see what happens. Yeah. Okay, let's try this.
[39:23] Times five. Oh, no, that is not time. It's going to hit that shift button.
[39:29] I don't know, but I can concentrate on that one. >> No. Do you want to talk it through?
[39:45] >> Yeah. Also, I looked down away from my code and said, adding the equal inside the braces
[39:52] will print the thing plus its results. >> Yeah. Here, what you,
[40:03] I think, were trying to do was say print this thing five times. >> Yeah. I want to do the Alice thing,
[40:08] but with Bakari and Jay. >> Let's break out a for loop.
[40:14] >> Okay. What is that? >> A for loop?
[40:21] >> Yeah. >> Have you done them in JavaScript?
[40:24] >> Okay. If I just say for loop, what immediately comes to mind?
[40:40] >> Me failing CSS and trying to tell it to make the box. >> Okay.
[40:48] >> That is probably not at all what you're talking about, but that is what first comes to my mind.
[40:53] >> Yeah. No, that's super helpful information for me. That's why I always ask my students when I was a math professor,
[41:03] what immediately comes to your mind when we say these words so that they can tell me where they're coming from and then I can be like,
[41:12] "Okay, so now we're in the same place." This is how you get from where we are in your head to where we're going,
[41:20] if that makes sense. >> Yeah. I think it's really cool because I know as I've been learning,
[41:26] there are a lot of things that how I was telling you, I know what I can figure out my way of doing it in JavaScript,
[41:34] but I don't necessarily know what it's called. >> Yeah, sure.
[41:39] >> Okay, cool. We are going to do a for loop. >> Yeah. Jay was pointing out you can do this without a for loop.
[41:49] For my head, I feel like it makes more sense to start from the for loop and then show how you can do it shorter with the f-string.
[41:59] But this isn't about what's in my head, it's about what's in your head.
[42:02] So we can do it either way. >> We can do it both ways.
[42:07] Really quick because I said that I was going to take notes and I didn't. I'm going to say really quick before I forget,
[42:18] an exponent is a first number power number. >> Yeah.
[42:32] >> Right? So 72 power of whatever, and then an modulus is leftover Legos.
[42:46] >> That's right. >> 22 Legos and sorted into eight or Lego piles of eight.
[43:05] >> Groups of eight, yeah. >> Would have six Legos left over and in a 22 Lego set,
[43:32] two piles of eight can go into it. Okay. Thank you. I just realized that part.
[43:41] All right. Back to for loop. >> You know what? We're probably going to get there pretty soon in this chapter.
[43:50] So maybe we'll hang on to that thought for a minute and come back when the book says it.
[43:57] >> All right. Then I'm going to copy and paste just what Jay said, because I really want just to see the magic.
[44:04] >> Yes, definitely. >> I will say that's the hard thing on,
[44:10] I don't know if anybody else gets this way, but I'm like, I just want to figure this out because I want to see it.
[44:15] Then it's like, I can't move on till I figure that one piece out. >> Oh, absolutely.
[44:21] >> It irritates me because I'm like, why? That doesn't help anyone.
[44:25] That just takes me forever. But now I can see it,
[44:28] and thanks for the answer. I can move on now. >> Yeah.
[44:33] >> All right. So, oh, Tracebacks. Alice Times Bob.
[44:47] Though this is like a very complicated way of saying what we just did. >> Yeah. I mean, sure.
[45:02] So if you don't have the benefit of doing something live in a conversation,
[45:11] it's harder to make it not feel complicated. >> That's true. I'm just looking at this and I'm like, what's a Traceback?
[45:21] Why am I putting it in a file? >> So it was in the previous chapter,
[45:24] what a Traceback is. >> Okay.
[45:27] >> I'm giving credit to Al for actually being super wonderful. >> Yeah. I'm definitely not saying it's me and books.
[45:33] It's not anything against Al. >> No, no, no. It's all good. Yeah.
[45:35] So basically that means, so it says most recent call last.
[45:38] So what it's saying is, this is where shit fucked up. >> Okay.
[45:46] >> That's basically, yep. >> Good explanation of it. Okay.
[45:55] Now I'm picking up what you're putting down and the book is putting down
[46:00] because scroll back up. We have what integers, floating point numbers, and strings are.
[46:07] Then if we go back down here, it's saying can't multiply sequence by non-integer type of float.
[46:19] Then can't multiply sequence by non-integer type of str, and okay.
[46:27] >> Yeah. It's saying, if you want to multiply a string, what that means to me,
[46:33] the computer, is you want to print that thing however many times. But if what you give me,
[46:42] if the number of times you give me is actually a string, it's not a number.
[46:49] It might as well be a word or a letter. Like the number five,
[46:58] if it's in quotes, that's a string. It might as well be the letter M.
[47:04] Saying Alice times M, what does that mean? The computer says that means nothing to me.
[47:13] Please revise and resubmit. >> Yeah.
[47:15] Similarly, even though mathematically, 5.0 and the integer five,
[47:24] are the same, they have the same value. It doesn't want you to give it floating point numbers
[47:32] because it's not going to know what if that said 5.1, then it would be saying,
[47:39] do Alice 5.1 times, and then it has to make a decision about what is 0.1 of Alice.
[47:49] I can't do 0.1 of Alice. That's why it's saying,
[47:55] please don't give me a string because that means nothing to me. Please don't give me a float because God knows what that means.
[48:03] Please just give me an integer so that I can just do the thing. >> All right. That is starting to make sense.
[48:13] Hello, do I say your name, Ugar? Hello, hello, and thank you for joining.
[48:20] Let us know if you have any questions. We also are getting streams in from Twitch.
[48:25] If things we're saying may not make sense from the comments, that is why we're streaming to both places.
[48:32] This makes sense. In my head at first, I was like, there's five there,
[48:38] there's five letters. A fifth of it could be letter A,
[48:43] but it's not going to know where the fifth is, which letter is fifth?
[48:48] >> It's more like it's because of the decimal. It's entirely because of the decimal.
[48:54] >> Okay. >> Saying, I don't know what to do.
[48:56] If that decimal were anything other than zero, it would have a problem because what is 0.1 of Alice or whatever.
[49:05] It's saying, please just give me a whole number to multiply this by. >> A variable is like
[49:18] a box in the computer's memory where you can store a single value. If you want to use the result of
[49:27] an evaluated expression later in your program, you can save it inside a variable.
[49:35] I think this might be me getting mixed up on both JavaScript and Python. Aren't variables not necessarily a sign because they're a variable,
[49:53] like they can change? >> Yes. In our example from a few minutes ago,
[50:00] first we can say x is five. Then on the very next line,
[50:05] we can say x is gen or x equals gen. We're assigning the value five to x.
[50:13] Then we're saying, never mind. Now we're going to assign the value gen to x.
[50:19] >> For clarification, it will just read the second one or is it going to say x could be either five or gen?
[50:29] >> It'll read them in order. At first, x is five and then not even a split second later,
[50:38] because computers work through things really quickly, then it'll be 42.
[50:42] But what will happen, or not 42, sorry, I'm just looking at what's on the screen, gen.
[50:46] First, it'll store the value of five to x, and then it will say, never mind.
[50:53] Now I'm storing the value gen to x. That totally helps.
[51:00] If I do, just using this example right here, and for me to do this,
[51:11] I don't need to use spam equals. I want to put you two next to each other. Thank you.
[51:21] I don't need to put the spam equals 40 in print, because I don't necessarily need to print that.
[51:30] If I want print. Now, I do this because would it be print spam?
[51:46] But then it did it. >> Right, it printed the value.
[51:56] >> But it didn't type the word because I didn't do the quotes. >> That's right. You've got it.
[52:02] >> It's basically, if you're giving a name, a number to a name and a name to a number,
[52:15] that's what we're talking about next is? >> It doesn't have to be a number.
[52:24] >> Okay. >> Right? You could have spam equals the string gen.
[52:34] Sure. Or pizza equals the string spam or whatever you like. Right? Then if I do print pizza.
[52:53] Then, so the only time it would need to be numbers is if we want it to total a number like this.
[53:08] >> Yeah. It only needs to be a number if you want it to be a number.
[53:12] >> Okay. Cool. Then we literally just did this. Yay. All right.
[53:22] >> Yeah. >> You talked about how if we name it,
[53:27] it's automatically going to update it within a few seconds. That is totally making sense.
[53:33] >> Not even a few seconds, like from a human perspective, it's instantaneous.
[53:37] >> Yes, and that is so cool. All right. Variable names.
[53:44] I'm going to make this bigger again. Imagine that you moved a new house and
[53:52] labeled all of your moving boxes as stuff. You'll never find anything.
[53:56] Most of this book's examples and Python's documentation use a generic variable names like spam, eggs, and bacon,
[54:06] which come from the Monty Python spam sketch. Does this mean that there's killer rabbits in Python?
[54:16] >> I have not yet encountered a killer rabbit in Python. >> Jay, are you still there?
[54:23] Are there killer rabbits? Because I'm like, if we're talking about Monty Python,
[54:28] can we do it and the Holy Grail and have the killer rabbits? >> I mean, we sure could.
[54:33] >> Now, it'd be a little bit tricky because the rabbit doesn't have a name in Holy Grail.
[54:43] >> That's true. >> But we could do any of the others that do have names.
[54:50] We could do the castle. >> Yes. I did read that part that
[55:02] the Python is named after Monty Python and not the snake. I first saw Monty Python in the Holy Grail when I was 13, I think.
[55:15] >> Yeah, good age. >> There's another one. Monty Python has a couple of them, don't they?
[55:21] >> Sure. Yeah. The feature length ones are Holy Grail, Life of Brian, and-
[55:25] >> Oh, Life of Brian. >> -completely different.
[55:28] >> Okay. Life of Brian is the other one I saw. Now, you guys are making me want to watch them all.
[55:33] Thanks, Al and Python group. >> That's a good use of time, Monty Python.
[55:39] >> Though you can name your variables anything, not everything, you can name them almost anything.
[55:49] Python does give some naming restrictions. Table 1-3 has example of legal variable names.
[55:58] >> Oh, I think these are pretty similar to JavaScript. They're like, would you say that these are
[56:09] pretty accurate for all programming languages? >> That's pretty standard.
[56:16] >> Yeah. Okay. This book uses CamelCase.
[56:24] Cool. I know what that one is. Instead of underscores.
[56:31] Some experienced programmers may point out that official Python code style is
[56:40] pep8 says that the underscores should be used. Al unapologetically prefer CamelCase and point to
[56:50] the a foolish consistency is the Hobgoblin of little minds.
[56:57] >> Goblin. Hobgoblin. >> Itself. Yes.
[57:01] Okay. There's a program, but we're at the top of the hour.
[57:08] >> So pep8 is a style guide. Just like if you've written an English paper,
[57:14] you probably used MLA style or like Chicago manual of style, that kind of thing.
[57:20] So pep8 is the MLA guide for Python. >> So I feel very fortunate
[57:31] that programming and learning these languages, it tells you there's error messages
[57:39] because when you write an English paper, it does not tell you if you're creating
[57:44] error messages unless you're using Grammarly. >> Grammarly does help.
[57:49] >> That's right. >> Honestly, we're halfway through this.
[57:57] >> Yeah. So I wouldn't worry about pep8 at all right now. Just like when we're teaching kids to read and write,
[58:06] we don't break out the MLA guide. That's for way later.
[58:12] >> I think this definitely could probably be a good break point. Just because as I'm getting into this,
[58:24] I'm like, "Oh, let's keep going." Then I don't think we're going to end in half an hour.
[58:27] We're going to end way too far past that. Real quick though, Jay said,
[58:35] pep8 is a standard. It's not enforced unless you are using a linter,
[58:40] but ultimately as long as people know what to expect with your code and how to read it, you're good.
[58:46] Even couldn't you also program a linter to tell you to not use pep8?
[58:56] I don't know if that makes sense. >> Yes. You can tell a linter.
[58:59] Just like there's MLA style and Chicago Manual of Style, there are other style guides besides pep8.
[59:09] Pep8 is the most common one. But you could tell your IDE VS Code.
[59:16] I can't even remember the names of any of the others because pep8 is the one.
[59:21] But you could use a different style guide. >> Jay says, "Yes, that's black."
[59:31] It's black style. Now I'm going to Google it.
[59:36] >> Yeah, I'm not sure what that means either. >> [inaudible]
[59:49] >> Oh, nice. Yeah, because there are things that I don't love about pep8.
[59:57] Actually, I'm with Jay. I really like CamelCase as well more than underscores.
[60:04] >> All right. Here we go. Thank you, Jay, for the link.
[60:12] Interesting. I think this is definitely something that is interesting, that's what I'm going with.
[60:26] But just a reminder for myself, I'm using Mew but I could use VS Code for Python and use something.
[60:44] I don't know if anybody knows this and I can go look this up afterwards, but is there a run in VS Code?
[60:55] Because every time I've used VS Code, I always end up using localhost.
[61:00] >> Yeah, so you mean like a REPL. Is there a REPL in VS Code?
[61:04] >> Yeah. >> So Jupyter actually is,
[61:11] and I think maybe toward the top of the REPL somewhere, it mentioned Jupyter with a Y instead of an I.
[61:18] There's a Jupyter plug-in for VS Code. I have never used it.
[61:26] Yeah, but we could do that. >> Well, Jay, disclosure,
[61:32] I feel like you haven't been on the show yet, and you got to come on the show at some point.
[61:38] So might as well be for VS Code. >> I've used Jupyter,
[61:45] sorry for clarification, I've used Jupyter, but not as a plug-in with VS Code.
[61:50] I've used Jupyter tons, just not in there. >> Yeah, I get that.
[61:56] I think Jay said that they've heard a ton of good things about Jupyter.
[62:03] Jay, I will be sending you the link to get on the show, because I would say I love doing these and I'm starting.
[62:12] I'm debating on still streaming of LinkedIn, because a lot of people see them and
[62:19] they do get something out of them. It's just harder to track if they are.
[62:23] It doesn't say if they're watching it or not. >> Interesting.
[62:29] >> The Jupyter VS Code extension, my colleague Sarah has a lot more knowledge on that.
[62:39] Okay. We got options. >> You know what? We are almost to the end of this chapter.
[62:46] >> All right. >> So totally up to you,
[62:49] whether you want to stop here and then do the end of this chapter. >> I feel like this is a lot of scrolling.
[62:55] We're only halfway through. I got to find out where we were.
[63:02] >> We were down at your first program. >> Yeah. I mean, I'm down. Let's give it a shot.
[63:11] >> Okay. >> We might go over.
[63:12] >> I mean, I don't want to pressure you if you're burned out. >> No, I'm not.
[63:16] I don't have a hard stop, but it's hard for me to go, "Yeah,
[63:19] let's keep going," when I need to be cognizant of my guests. >> Oh, sure. You know what?
[63:25] Today is suborbital day, so we have the last Monday of every month as a day off.
[63:31] >> Fancy. All right, well, all right. >> Yeah. I was wrong when I said I was looking at the wrong spot.
[63:40] I was looking at summary or something when I said that we're almost done.
[63:42] We're not quite almost done, but I would be good to do the first program now or next time.
[63:50] >> All right. Then whichever is good for you. >> Yeah. Well, the interactive shell
[63:58] is good for running Python instructions one at a time to write entire Python programs.
[64:04] You'll need instructions to type instructions into the file editor. The file editor is similar to text editors.
[64:13] >> Okay. Open a new file in Mu and then click on the "New" button. Well, we got a new button.
[64:25] The window appears to contain a cursor, but it's different from the interactive shell which
[64:31] runs Python instructions as soon as you press "Enter". I guess we should have been doing it in the interactive shell.
[64:40] >> There's no should. >> Okay. Type your both options.
[64:45] >> Good call. That is another thing that I really got to work on is because that puts unnecessarily pressure on all of us.
[64:55] >> Yeah. They're both useful. The REPL is great for when you just want to see like, "Okay,
[65:01] if I did this, what would the output be without running your whole file?" >> All right. I should probably name this one.
[65:13] Here we go. We're just going to write on [inaudible] When the file editor window opens, enter the following.
[65:35] The hashtag, I did not need that. When it's a hashtag like this,
[65:44] goodness gracious, that means it's just notes, right? >> It's a comment.
[65:50] >> It's a comment. Okay. >> Yeah. Just like in other languages,
[65:54] you might use two slashes. >> Yeah.
[65:57] >> Slash and that's comments. Yeah. >> Or yeah. Okay. Cool.
[66:02] Print, "Hello world." Print, "What is your name?"
[66:06] Ask for their name. Well, this is easier.
[66:11] Oh, it did the indent. >> Yes. It would get mad if it didn't have the indent.
[66:19] >> That is good to know. My name is Input. We will fill in the blanks.
[66:26] It is good to meet you. >> Actually, in this case,
[66:36] it wouldn't because that's not actually, the white space there is not part of the program.
[66:41] It's for ease of reading. We'll see what it does.
[66:48] It might actually get mad that the white space is there. We'll see. >> I feel like this one didn't need to be.
[66:58] I got to put some spaces in here because. I'm starting to learn where spaces go in JavaScript.
[67:13] But this one, it's all squished together. But I do like this idea.
[67:20] >> These spaces are for the benefit, like the line breaks,
[67:26] like creating vertical white space, is for the benefit of the humans reading the code.
[67:33] The computer is not going to care. >> Right. All right.
[67:37] Let's just see if I got this thing to, even though it's not going to have anything.
[67:43] Indentation error. It doesn't like one of my indentations. >> Unexpected indent.
[67:48] What it's going to say, right above, you can see there's a little caret under
[67:52] the P in print for what is your name. It's saying, this is where there's an unexpected indentation.
[68:00] That's where I was saying, and that's the other thing,
[68:04] is that it's going to stop when it reaches the first error. It's going to be upset about all of those
[68:10] because indentation means something, like horizontal white space,
[68:14] that means something to the computer. It means a nesting situation.
[68:19] >> Yeah. How does it know not to go past Hello World, what is your name? Just because this input is blank?
[68:34] >> That's right. Well, the input, it's not that it's blank,
[68:39] it's that it's a function. That function says, get user input.
[68:46] So it's paused, it is politely waiting for you to enter your name. >> All right. Hello, Ben.
[68:57] >> Hello, hello. Oh, no, I mean. >> Down below?
[69:04] >> Yeah. It's waiting for your input. >> This got way more exciting.
[69:18] Y'all, I'm old. >> Okay. So notice, it said,
[69:24] it's good to meet you, Jen, and then it said the length of your name is five.
[69:28] Why does it say five? >> There must be a space there?
[69:36] >> That's right. >> Okay. Well, let's see.
[69:39] >> So if you run this again, and you put in Jen with no space. Yeah.
[69:47] >> Interesting. I'm a little confused. Thank you, Jay, and y'all go watch Jay's.
[70:06] I feel like we might be streaming at that point, so I'll attempt to read into yours, Jay.
[70:13] Jay, are you going to be doing it on your stream or somebody else's? >> I think on their stream.
[70:20] >> Okay. I guess I don't understand the bit about why do I want the length of my name?
[70:36] >> I mean, maybe you don't. But in the file,
[70:42] we have below where it says print, it is good to meet you space plus my name.
[70:50] It says print the length of your name is, and then it's going to find out the length of the name and then print that.
[70:58] So if you don't want to know the length of your name, you can just take those two lines out and it won't do them.
[71:06] >> Then it just knows that it's doing the length. >> That's right. That's the length function.
[71:14] Means you give me a string and I tell you how many characters are in the string. >> Okay. Interesting.
[71:34] >> Do you want to change what's in there a bit to see how changing it, well, changes. >> See how making changes changes things.
[71:46] >> Yes. >> Yes. Because this isn't life and I don't have to sit patiently waiting for things.
[71:52] I don't know why that cracked me up today, but it did. All right. I don't know.
[72:01] What's the length of something else it could do? I don't know. Okay. If I wanted this to,
[72:11] so I didn't get rid of it, but I wanted to make it whole.
[72:17] That's exciting. >> Yeah.
[72:21] >> I don't know why I'm so excited about this, but it's exciting. >> Yeah.
[72:32] >> All right. Then this is a stir or a string, an integer of your age,
[72:42] and then plus one in a year. I could do minus one last year.
[72:53] Well, that didn't do minus one. Could I do my age?
[73:04] Is there a way to do the year that it automatically can pull what year it is? >> Yes. We would need to import a library for that.
[73:21] I'm not sure which one. >> Okay. We're not going to do that.
[73:25] But the integer is my name. >> You know it would be an easy way to do it though,
[73:32] would be to just declare a variable called this year equals 2022. >> Cool.
[73:50] >> Then I would do int 2022, like this. >> It depends on what you want it to do.
[74:04] >> What is your age, and then have it do the input,
[74:08] and then it will say, you were born in X year.
[74:12] >> Okay. Let's start with the string part first. Instead of saying you will be,
[74:22] you can change it to the you were born in. >> Yeah.
[74:27] >> Then maybe you don't need the string at the end, the space in a year.
[74:40] So what that function there is saying, yeah, we can take out the ones.
[74:50] This function is saying whatever, so the number that the user gives for their age,
[75:01] that's going to be an integer, and we need to convert it to a string,
[75:07] so that we can add it to the string that's in front of it. So that's called casting.
[75:16] So we're going to cast this integer as a string. So that means consider this number as a string.
[75:29] >> So I'm excited that I'm about to be a magician. >> Yes.
[75:35] >> This is Ramon and I have talked about it, and we both really,
[75:40] really like the sparkle emoji. I don't know why, but it makes me think.
[75:47] So in this string, can I put two integers or do I have to create?
[75:56] Well, I guess instead of just asking you, I could try it because that's how you learn things.
[76:01] >> Sure. >> Is year me whole.
[76:11] >> You're telling me a bunch of stuff that I can't even see. I feel like there's more.
[76:18] >> Object, string, string bytes, or buffer encoding is created.
[76:24] >> I feel like this is the complicated stuff that- >> It's okay. So scroll down for a second,
[76:30] and then put a plus in between the int this year plus int my age. We're going to need to do this string consideration,
[76:48] or hang on a second. Wait, I said plus,
[76:51] but it shouldn't be plus, right? Yes. So maybe since we're doing a calculation,
[76:59] we're going to break this up into three lines. We're going to add an extra line maybe,
[77:05] just for the sake of it being super clear what the code is going to do. >> Okay.
[77:12] >> So let's make a new variable underneath my age input, make a new line.
[77:21] Let's create a new variable called birth year. >> Okay.
[77:32] >> It's this year minus my age. >> I guess we could have just said 2022 minus my age and not done the this year.
[77:42] >> Yeah, I'm okay with it. This year minus my age.
[77:50] >> Okay. Then where we have the string int this year blah blah, we can just make that be take out the this year and put birth year.
[78:02] >> You said put birth year, right? >> That's what he's actually suggesting down
[78:14] there because you've already declared that variable. So it's saying, hey, you're starting to type
[78:18] the name of a variable that I already know about. >> Right.
[78:22] >> Then we can just take out the whole minus int my age thing because we're done with it.
[78:28] We already did that above. >> Okay.
[78:34] >> Let's run it. Unexpected. EOF is end of file,
[78:41] so it's telling us that that happened on line 17. Do we have enough parentheses?
[78:51] I don't think we do. So if we're looking at our print statement.
[78:54] >> Oh, yeah. I see it. It didn't match this one.
[79:00] My name is Yen. What is my age? 34.
[79:11] >> Now, we're finding another error. We've got birth year equals this year minus my age,
[79:18] unsupported operand types for int and string. What happened was that my age,
[79:27] the input type was string. When we use the input function,
[79:33] the input that it's getting is going to be in the form of a string. Instead, we need to cast that as an integer.
[79:42] We can put int and then parens my age. >> Would I do this for year 2?
[79:51] >> This year is already an integer. Here we go. >> Then do I need bigger spaces here like the equals,
[80:03] or do I put them together? >> The computer doesn't care.
[80:08] In terms of style, it is more common to put the spaces just to
[80:16] increase readability for the humans. You got it.
[80:26] >> Yay. >> Yay. You wrote your first Python program.
[80:39] >> This was exciting. >> You didn't just write your first Python program,
[80:43] you also changed it to make a new Python program. You actually wrote your first two Python programs.
[80:49] >> Oh, this was exciting. >> Yeah. This is the note I was more excited to end on.
[80:56] >> Yeah. This was legit. >> Right. Yeah, we have accomplished.
[81:02] >> We have accomplished. I should probably take a look at my notes and see what I did or did not write on my notes to make me.
[81:10] I remember an exponent, a modulus, an integer, and then so I would put what is this thing called?
[81:26] A PEP 8 is default? >> It's the currently most common style guide.
[81:39] >> It's especially in the data science world, you would definitely use PEP 8.
[81:48] Maybe you use a different style guide in the web dev side of things. Just like in English departments and so on,
[82:02] you use MLA style, but in psychology, for instance,
[82:07] you might use Chicago Manual of Style instead. Each discipline has its own style guide or not its own style guide,
[82:15] but each discipline gets to decide which style guide it's going to use. That's a better way to say it.
[82:21] >> I know I'm over here like all quietly. >> No worries.
[82:31] >> I'm taking notes. If I go back to Laura is cool,
[82:41] we change this to make it. That is called an F-string.
[82:56] The goal was to add the Kari and J to create Kari J, and have it print or have it duplicate five times.
[83:25] >> Or just from a picky math teacher. >> You write docs,
[83:37] so I would love to hear it. >> Duplicate means two.
[83:43] If you duplicated something five times, you'd make 10 of them.
[83:47] If that makes sense. >> How would you say that?
[83:53] >> It makes sense. I'm not going to like points. >> Printing it five times.
[83:57] >> Have it print five times. I needed to change five outside of curly brackets.
[84:19] That's what we're going to go with. >> I'm trying to put why this one worked,
[84:26] but the other one didn't. I personally feel like this spam equals 40 thing is
[84:31] pretty self-explanatory because it's just defining a variable. >> Well, they're your notes.
[84:38] >> Well, I'm trying to create them for other people, but also for myself because it's a read me.
[84:45] >> Yeah. I mean, but it's not immutable. >> You used a big word.
[84:57] >> If something is immutable, you can't change it. If it's immutable, you can change it.
[85:04] You can keep changing your read me. Your read me doesn't have to be perfect.
[85:09] You can get the notes in there that are like the ones that are helpful for you,
[85:13] like the things that you think of today. >> Yeah.
[85:15] >> Then if in future you're like, "Oh, you know what? Maybe I really should go back in and add
[85:20] some more notes for other people who aren't me," you can do that. >> All right. I dig it.
[85:26] Then I'll grab these just in case I talk about variables. But it is called, just so I know, defining variables?
[85:48] >> Defining or assigning. >> That was pretty sweet.
[85:59] I feel like we did a lot, but I will say reading it first,
[86:05] I think really, really helped because I was like, and I wasn't even looking at the screen when it was reading it to me,
[86:12] I was just listening to it when it was getting ready. While I was getting ready,
[86:17] and I think it's really cool in the fact that I remember what the words were saying.
[86:22] I get the gist of it a lot easier that I'm like, "Okay, cool. There is a lot of words here,
[86:28] but it'll remind me what I already heard, so I don't have to read every single word."
[86:35] >> I do the same thing. When I was doing online courses,
[86:41] I would usually listen to them while I was doing something else with my hands,
[86:46] because that helps me actually focus on what I'm listening to. Then I'd listen one time,
[86:53] and then I would listen a second time, and that time I would be taking notes.
[87:00] I have projects for work this week that I'm digging your style and think I'm just going to copy you and do that.
[87:12] >> It can feel inefficient, like, "Oh, but then I have to listen to the whole thing twice."
[87:19] But if that means that when you have listened to the whole thing twice and done your notes you actually understand stuff better,
[87:26] then it's worth the time, right? >> Yeah.
[87:30] >> That's what I have to keep reminding myself, this is worth it. >> Yes. Even though it's not what everybody else's process is,
[87:38] doesn't mean that it's wrong. >> That's right.
[87:40] >> Really quick, Ben, you just made a clip of that. It's way more interesting now that we made a program.
[87:48] Very excited about this. >> Neat. Thanks, Ben.
[87:52] >> I got to figure this out, because that was just cool that you made a clip.
[87:59] I didn't even know you could make clips. I'm pretty excited about that one too.
[88:04] >> I can see it on my end on Twitch. There's a little button at the bottom that says clip.
[88:11] >> Okay. Well, I think we have wrapped up for today, but I'm not going to let us go yet.
[88:19] I'm going to figure out how to read, maybe. Maybe I am.
[88:25] I'm clicking a bunch of options, so don't mind me while I'm.
[88:36] I could show it. We could live stream me trying to figure out how to read. I'm okay with that.
[88:43] You just might see yourself multiple times. I know it's in my stream manager,
[88:48] and suggestion box, quick actions. No. Oh, clip that.
[88:57] Okay. I do have a clip that. That's cool. I don't know.
[89:07] No. I think everybody left us to streaming tools. No. I'm just going to Google it.
[89:27] How to read on Twitch. Oh, type raid.
[89:43] Start a raid for such read followed by the name of the channel. All right. Well, let's go here.
[90:06] Yes. What happened to everybody's chats? I think that's his channel, maybe.
[90:25] Okay. So, KJ Miller. And see if the magic happens. Raid channel. Raid has been created.
[90:53] Oh, that's exciting. And raid now.
[91:01] And we will stop the live because Twitch all went over the hits. And let me end this broadcast.
[91:12] And thank you, everybody else for joining. That's exciting to raid.

