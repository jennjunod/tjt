---
showLink: "https://www.youtube.com/watch?v=w-I60iANqCY"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-intro-to-python-with-laura-langdon"
title: "Teach Jenn Intro to Python with Laura Langdon"
publishDate: "2022-08-15"
coverImage: "https://i.ytimg.com/vi/w-I60iANqCY/maxresdefault.jpg"
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

[00:00] >> All right. >> Hello, beautiful humans.
[00:03] Thank you for joining Teach Gen Tech. Today, we have Laura here.
[00:08] Laura, please introduce yourself and what you'll be teaching us today.
[00:12] >> Hi, Jen, and hello, everybody. I am Laura.
[00:16] I am a technical writer at Suborbital Software Systems. But before I was a technical writer,
[00:23] I thought I was going to be a data scientist, and so I was studying Python and data science.
[00:28] Before that, I was a math professor. Actually, until December.
[00:34] All of those before that are short periods of time. >> Did you say a data scientist?
[00:45] What is that? >> It's like how computer science used to be this small-ish field,
[00:58] and maybe people specialized in little bits of things, but more or less, everything overlapped with everything.
[01:05] Then now, there's front-end and back-end, and there's this and there's that,
[01:08] and there's all kinds of stuff. Data science has gone the same way.
[01:13] At a super high level, it's the study of data and
[01:19] manipulating data and learning things from data and so on. It's a subset of artificial intelligence.
[01:27] They sometimes get used interchangeably. Machine learning is a type of data science,
[01:33] and of course, that is also associated with artificial intelligence. It's in that genre.
[01:42] >> Interesting. There's so much. >> I'm just realizing that my microphone is not in front of my face.
[01:48] >> Yeah. Your microphone sounds even better. >> Sorry.
[01:53] >> I am very lazy about my microphone, and so I use my cool little headphones because I don't like a microphone in front of my face.
[02:05] I don't know. I think that does make a bit of sense, because when I started this journey of Teach Gen Tech,
[02:15] which is not even two months old, which is bananas to me,
[02:18] almost two months ago, I heard from a lot of people that Python was
[02:25] more of back-end stuff and JavaScript was all front-end, and that was a big reason I started with JavaScript.
[02:36] Later this week, we'll have Ian on from Postman, and he's going to be talking about why you may choose one over the other,
[02:46] why you would use JavaScript or why you would use Python. I think perfect timing of it follows up for today.
[02:54] >> Is that Ian Douglas? >> Yes.
[02:57] >> Oh, I was just on his show two weeks ago. >> Yeah, he's so cool.
[03:02] He's going to be on, and I think that's a great opportunity
[03:06] since I am learning this from you today. Yet, I guess especially since I heard
[03:14] Python does more like data and data mining and that kind of thing, I'm scared about this one.
[03:22] >> Okay. >> Because for me, at the moment,
[03:27] maybe it's not going to be that complicated, but it's harder to conceptualize that code is doing that.
[03:36] I don't know. This has been a big journey for myself of like, oh yeah, that is how something is made instead of it just magically happened.
[03:47] So I'm excited about learning about it today also. We'll see how much it sinks in or not.
[03:56] >> Sure. I mean, you can use Python for all kinds of stuff. You can deploy apps to the web with Python,
[04:04] like with frameworks like Django and Flask and so on. So it's not exclusively a data thing.
[04:10] But it is, I think, one of the easiest programming languages to learn.
[04:16] I think it's maybe the best. I'm saying maybe because I have
[04:22] a math background and so I can't say definitively that something is the best, if there's any possibility that that might not be true for some edge cases.
[04:31] Basically, I think it's the best programming language for someone to learn because it's a lot less fiddly and we'll see how that works out.
[04:43] >> Okay. I dig it. >> I don't even know where to start.
[04:50] >> All right, cool. Let's see. Do you have that link or I can grab it for
[04:55] the book Automate the Boring Stuff with Python by Al Swigert? >> Do give me a second.
[05:01] I will grab that. I'm grabbing it off screen because I'm really bad
[05:06] at forgetting that kind of stuff and having to go back to Twitter, but I've got it here shortly.
[05:15] >> [inaudible] >> Yay.
[05:25] >> All right. Is that big enough? I always feel like I don't make my browser big enough.
[05:30] >> It looks good to me. >> Cool. All right.
[05:34] >> Yeah. When I started learning, the first programming language that I learned any of was HTML.
[05:44] Way back in the day, the GeoCities days, and then I learned some Perl,
[05:55] which is not very common these days, but it's Python-like.
[05:59] Then I learned C++ in a computer science class, and I could not believe how fiddly C++ was compared to Perl.
[06:09] Python was very refreshing to me because it felt more like Perl. It felt even better. I tried a bunch of different resources,
[06:19] including this one, and this one was my favorite for a whole bunch of reasons. Alice Weingart is really active on Twitter,
[06:28] and when I was working on one of the exercises in this book, I had a question, I DMed him,
[06:35] and he literally answered me in 20 minutes. >> What?
[06:39] >> We had a whole conversation. He is the tremendous bestest for this, I think.
[06:46] >> Okay. >> He's made this book available for free,
[06:49] so you can buy the physical book or an e-copy of the book, which I highly recommend to support Al's amazing community efforts.
[06:58] For today, we can just use the browser version though. >> That's interesting and good to know.
[07:05] I think something that you and I were talking about beforehand is, you learned from using this,
[07:12] and I'm like, this is probably one of the biggest reasons I never got into code before this.
[07:20] I think it was C# class in my many random tangents of university, and it never communicated because it was a lot of reading the text,
[07:43] to be able to create things, and this is probably almost probably 15 years ago.
[07:51] I wasn't getting it, but I needed to pass the class. So I ended up hiring someone off a Craigslist to do
[07:59] my homework and make the mistakes because it didn't make sense. I love now that there's applications that we can use for
[08:10] the tech and to screen readers or text-to-speech, that's helped so much. Then also learning my own learning styles,
[08:22] that's a big reason that I started teaching on tech is, I was trying to do like LinkedIn or Code Academy,
[08:29] and that's just not syncing in the same way, where when I get to learn about all this random shit,
[08:34] and then I get to go, "Teach me the things and let me ask you all the questions," because if I don't learn that how A goes to M and associates with Z,
[08:47] I'm going to get really stuck on it and then not be able to move forward. So I super appreciate you coming on the show and excited to learn about this stuff.
[08:57] >> It sounds like we have pretty similar learning styles, so perfect. Sweet. All right.
[09:04] What? We're going through here and I honestly didn't even look at it before today. >> No worries. Yeah, you can scroll past all the boilerplate.
[09:16] I think we don't necessarily need to read the introduction, although he does call out in the who this,
[09:23] sorry, if you scroll up just a little bit, like who this book is for and specifically says,
[09:30] "Countless books, interactive web tutorials, and developer bootcamps promise to turn
[09:34] ambitious beginners into software engineers with six-figure salaries. This book is not for those people.
[09:40] It's for everyone else." >> I dig that because yeah, that is.
[09:48] That's why I really like that this has been starting to build a community because being able to show people that they can learn no matter what
[09:56] their learning style is and also giving them an opportunity to ask questions and an outlet to ask questions.
[10:05] So now I love it even more. >> Yes. Okay.
[10:12] So if we keep going. Yeah. Since you already have experience with a programming language,
[10:25] I figure we won't necessarily talk about everything like this part, like what is programming and we basically know that.
[10:34] Anybody who wants to read that, of course, can follow the link and read all of this good stuff.
[10:39] >> Yes. To that point, I will put the link will be also added to the description,
[10:51] but it will also be commented right here. So it went to both YouTube and Twitch.
[10:59] What is Python? >> Yeah. So it does actually come from Monty Python.
[11:07] There was a great interaction once when one of the people from, I think it was maybe Michael Palin from Monty Python,
[11:19] saw the word Python trending on Twitter and was like, "Oh, haha, I thought it was going to be about us,
[11:24] but it was actually about the programming language." Then Guido, I can't remember his last name.
[11:29] Anyway, he wrote Python. He was like, "But it is actually about you.
[11:34] Also, hi, Mr. Monty Python person." They had this whole little like, "Oh, that's nice. Who are you?"
[11:42] It was just like one of those, "God, I love the Internet."
[11:47] >> Yes. I would say it's so cool because I think this is my 16th or 17th episode and everyone I have met,
[11:59] except Ian, Ian I met in person. Everyone else I have met through Twitter.
[12:07] >> Yeah. I actually don't know how to do a career without Twitter, and that's not an exaggeration.
[12:14] >> I didn't even know how to use Twitter before this journey. So I started using Twitter in June.
[12:26] Now I'm like, "It's so fun." >> Yeah. People are always like,
[12:32] "Oh, you need to be on LinkedIn for whatever." I'm like, "I guess."
[12:38] I mean, yes, you should have a LinkedIn profile, but should you be spending a lot of time on LinkedIn?
[12:43] I just, I don't really buy it. I think if you're going to spend time on
[12:49] a social media platform and you're looking for a job in tech, the one that you should be spending your time on is Twitter.
[12:57] Yeah. I dig it. I dig it. Okay. Hey.
[13:01] >> Then we've got. >> I feel like you know a lot of math,
[13:05] but I'm excited about this. >> Yeah. Since you've already done some programming,
[13:14] then you know that you don't need to know a lot of math in order to be a programmer. >> Why do you? I guess I don't know where
[13:23] that idea came from that you have to know a lot of math. >> I suspect it came from,
[13:33] I want to say two places, but maybe it's the same place in the end.
[13:37] The original computer scientists were mathematicians, full stop, like Alan Turing. What was his degree in?
[13:44] Math. Would he have referred to himself as a computer scientist? No. He was a mathematician.
[13:52] So it really arose from math. The other thing is that if you're doing a computer science degree at a university,
[14:05] you will be required to work up through probably calculus 1, and you'll probably have to take discrete math.
[14:14] >> I forgot about that because I did not realize that I was incredibly dyslexic, and me in school in general being ADHD and all that.
[14:26] But I would always fail math. I've had, "What up, Ramon?"
[14:32] I always had to take multiple math classes. I think I've taken Algebra 1 three times.
[14:40] >> Then you haven't taken it as many times as I have. >> What?
[14:44] >> True story. >> Yeah. Well, I still haven't passed.
[14:48] I just gave up on that degree. I was just like, "What up, Noelle?"
[14:52] >> I'm just saying. I took Algebra 1 a whole bunch of times.
[14:57] I took Calculus 1 four times, three times. I have graduate degrees in math.
[15:05] >> But you are reminding me why I also didn't continue down a computer science degree,
[15:14] because I would do the math like the right problem-solving skills, but I never realized how much I disposed my numbers,
[15:29] and even in the calculator. Even though if it was written right,
[15:35] it just makes me happy to hear, not happy, but happy that I feel very validated.
[15:41] >> It's interesting too. I feel like, I mean, this is way off topic,
[15:45] but I feel like we do math a huge disservice, because there's just so much stuff that's fun in math,
[15:53] like graph theory, which sounds like you're doing a bunch of making graphs and so on,
[15:57] but it's all nodes connected to other nodes, and you're actually drawing pictures of these nodes talking to
[16:05] each other and how they're connected and studying all of those things. I always say I like my math with as few numbers as possible,
[16:14] and people's minds are blown because they're like, "What is math without numbers?"
[16:18] But there's this whole world of math with symbols that aren't numbers. Yeah. Anyway, it's super cool.
[16:25] There's all kinds of cool stuff in there. >> Yeah. I feel like maybe one day I'll go back,
[16:30] but something that I'm realizing as an adult, that it's taken me a really long time,
[16:38] is to focus on one thing at a time and not to try to do everything at once.
[16:44] >> Sure. >> So I say that because I should probably get back to this,
[16:48] but also in the fact that I used to be like, "Oh, I can learn coding and to do math and to do baking."
[16:59] I don't know. I'm totally making this up. >> Okay. Sure.
[17:01] >> But you only do all of them half-ass unless you actually focus at one of them.
[17:06] >> I think it depends on the person. So I also have ADHD,
[17:16] and I feel like my brain has three channels. I have to have all three of them going at once,
[17:23] or else whichever one I'm trying to use, the other two will just start doing random stuff.
[17:30] I can either fill those channels with something intentional, or they will fill themselves,
[17:36] but they're not going to be empty, almost ever. So for me having actually,
[17:43] and this happens to you all the time when I was a math student, I would be working on a problem, I'd get super stuck.
[17:51] I had to go do something else. Then I'd come back and be like, "Oh, it's this."
[17:59] Why did not thinking about this for two hours suddenly mean that I figured out
[18:04] something that I had been thinking about for four hours and didn't get to the answer?
[18:09] >> I feel you there. >> Yeah. Maybe that thing is like, "Okay,
[18:16] I'm just going to go for a walk or I'm going to go make dinner," or something like that.
[18:21] But if you are fortunate enough, as I have been sometimes,
[18:27] to be able to devote a lot of your work time to studying. For me, if I spend all of that time studying one topic,
[18:38] I am going to get something out of it, but not as much as I would have done if I had
[18:44] spent that time studying three topics. >> I get you there. I feel very, very similar.
[18:54] I think when I mention it, it's more of mattering on the difficulty of what I'm learning.
[19:03] >> Totally. >> Baking is going to be completely different.
[19:06] I don't know anything about baking, so that's going to be completely different than coding.
[19:10] That is not using the same wavelengths. >> Yeah.
[19:14] >> Where I have my podcast, Shit You Don't Want to Talk About,
[19:18] then I have Teach Gen Tech, then I'm an API co-organizer for the Meetup here in Denver,
[19:24] and then starting a new part-time job. They're all on the same wavelengths,
[19:29] so it's a lot easier to conceptualize, where dude, I feel like this.
[19:36] You just got to join on Wednesdays because Wednesday, we do a Twitter space talking about mental health,
[19:41] neurodivergency, and tech. I feel like this is such an important topic.
[19:48] >> Yeah, love to. >> Yes. Yes. Yes, Noelle.
[19:53] I don't know why we take Algebra 1 so much, but I do like the fact
[19:58] that we're never too old to learn programming. I feel that. I'm 34.
[20:03] I feel like an old lady and I'm learning it. I'm excited.
[20:07] >> I do know why we take Algebra 1 a lot of times. >> Oh, do it, do it, do it.
[20:13] >> It's because it's the first time that you're pulling together all kinds of
[20:19] different things that you've been learning since you were four. You're pulling them all together to do them at the same time.
[20:25] Because previously, we were doing, right now we're doing multiplication,
[20:30] and then we're doing division, and then we're going to do fractions,
[20:33] and then decimals, and then long division or something, and then integers and so on.
[20:38] So we're doing all of these things siloed. Then in Algebra, we're bringing them all together for
[20:46] the first time which means that we're having to relearn the ones that we forgot.
[20:52] We're having to unlearn things we thought we understood that were incorrect.
[21:00] Having to use them altogether and use them to solve problems. It's like if you've spent all of your time learning how to
[21:17] use a hammer and you're just doing the hammer by itself. Then two weeks later, you're just doing the screwdriver.
[21:23] A few weeks later, you're doing the saw or something. Then you bring them all together to make an actual project.
[21:31] The project is not going to come out very well the first time. It may not even come out great the second time.
[21:37] By the third time, you're starting to get the hang of it.
[21:41] Algebra is a project. >> All right. Interesting.
[21:46] >> Learning new tools. It's both. It's like learning, it's using all the tools that you've been
[21:51] amassing for six years using those altogether, and learning some new ones.
[21:57] Of course, it's going to take some time. >> Interesting.
[22:03] >> The only reason that we feel like it's a problem is because we get graded on how quickly we can mash these things together.
[22:16] >> Have to repay for another semester of the same class. >> That too. There's shame involved in it and so on.
[22:23] Yeah. That's why it's not Algebra's fault. >> Okay. I like that.
[22:29] I like that. It's not Algebra's fault. Now, I'm so curious.
[22:34] If you said it was Swigert, if he's neurodivergent as well because making this book.
[22:48] But Al, if you ever hear this, come hang out with us. That's all I've got.
[22:53] >> Yes. We could tag him too. >> Done.
[22:59] >> Yeah. I can't speak for Al Swigert. I don't actually know Al Swigert personally.
[23:06] We chatted once like two years ago on DM. But anyway, I have a pet theory that is actually borne out by data,
[23:14] that neurodivergent people tend to have good vibes with other neurodivergent people.
[23:23] If a neurodivergent person likes somebody's vibes, the odds that that person is also neurodivergent are quite high.
[23:32] Cannot speak for Al. >> I dig it. Al, look,
[23:36] we've already tagged you on Twitter. I'm just going to tag you all the time now to check this out.
[23:42] So I'm going just to the overview. We got part 1, Python programming basics.
[23:52] Chapter 1 is the basics, covers expressions, the most basic type of Python instruction,
[23:59] and how to use Python interactive shell software to experiment with code. Chapter 2, flow control.
[24:08] I'm scrolling through this because there's a lot here. I know we are starting at the beginning,
[24:16] and anybody that wants to come check this out, they can.
[24:22] >> Yeah. So let's pause here. >> I was like, "Hey, this is what we're looking for."
[24:30] >> Yeah. So we definitely want to use Python 3 and not Python 2, because Python 2 is no longer supported.
[24:40] That's relatively recent, maybe two years ago, that Python 2 was unsupported.
[24:48] >> Okay. >> All right. So we'll go get Python.
[24:55] >> Then, hey, look, it's the latest version. >> I'm writing my reading in the other screen.
[25:16] >> Oh, sure. >> If I can get used to at least taking the notes while we're doing it.
[25:23] >> I used to do that, or I still do. I made them into blog posts,
[25:32] and it's literally how I got my job for the record. >> That's actually what I want to do is go back and start blogging about them.
[25:39] I wrote my first blog last week. I've never published a blog before.
[25:44] So that's a big reason that I'm wanting to pay more attention to my read-me's, because now that Anthony,
[25:52] who was on last week, started to explain it. I'm like, "Oh, that makes so much more sense
[25:57] to be able to get someone to be able to do it." >> Right.
[26:02] >> So I need to go into my code folder, which I should probably update.
[26:08] No, I should see where I'm at. At one point, I will make it so it's my default folder.
[26:19] I haven't yet. All right. I'm in the proper folder now.
[26:29] Warning, Windows Terminal. But we're not running this, right?
[26:37] >> We're not in Ubuntu. At least it looks like you're in Mac OS.
[26:41] However, Ubuntu is a flavor of Linux. It's a Linux distribution, and Linux is Unix,
[26:52] and Mac OS is secretly also Unix. Pro tip, if you find something that works in a Linux terminal,
[27:02] it also works in a terminal on Mac OS. >> I'm going to go back to this one because
[27:09] it doesn't look like it has the, that's for the system, let's see.
[27:21] Thank you for giving me a second to read through these and work on. >> Mac OS, download the file,
[27:28] double-click on it. Interesting. It just installs it like a program.
[27:38] A lot of them I've had to do NPM installs instead of like this. >> Yeah. It's not an NPM install because that's a JavaScript thing, right?
[27:51] >> It's not. There's pip install and conda install for Python. But if we're just getting started,
[28:04] we don't have to do those, so we'll just do this.
[28:09] >> Interesting. My goodness. I thought that was just like an install anything kind of thing,
[28:15] not necessarily a JavaScript thing. >> It's associated, it's part of Node,
[28:20] so it's not just installing JavaScript things, but it is a package manager for JavaScript things and related things.
[28:30] Then there's pip. Pip is the one that you use.
[28:34] If you are a Python person, then pip is your NPM.
[28:38] Pip is the one that you pip install this and you pip install that. >> Okay. Interesting.
[28:47] >> Hold on. >> Conda is another option,
[28:50] but I haven't used that one too much. >> Downloading and installing.
[29:04] >> Let's make sure we finished installing Python first. It looks like I see it in your applications folder,
[29:13] so I think that we are probably good there. >> Am I using the Python launcher?
[29:19] >> Let's see what it does. I have actually only used it through in a Conda.
[29:28] Is this a safer work stream? >> No.
[29:36] >> Okay, cool. Because I have a very not safe for work thing to say about this.
[29:41] The way that I first started interacting directly with Python was through a program called Anaconda.
[29:50] The instructor of the course that I was looking at at the time said, "Okay, Anaconda is great because it'll install everything for you."
[30:03] I had a little internal snicker at the word Anaconda. I get it because it's Python,
[30:11] it's a snake, but sir makes a lot, ha-ha. >> Yeah.
[30:15] >> Then he goes on and he says that the thing is about Anaconda, that it takes up a lot of space. It's pretty big.
[30:26] If you don't have room for the full Anaconda, there's another distro called Mini Conda that you can use instead.
[30:36] I was absolutely deceased. I am a ghost.
[30:43] I do not live anymore. I died three years ago.
[30:46] >> I feel like the creators of Python and Anaconda knew this, and they are having fun with everybody.
[30:55] >> I just cannot believe that he said it with a straight face. If you don't have room for the full Anaconda,
[31:01] you can install Mini Conda. >> I'm not going to lie, as soon as you said I want to install Anaconda,
[31:07] I'm like, "Yeah, that's all that just popped in my head." >> Yep. Right. Okay. Anyway, so let's close this for now.
[31:17] >> Easy peasy. >> Since you have already said that you would like to use,
[31:24] you want to do it in the terminal instead of in VS Code, we will proceed to Mew.
[31:35] >> Mew? Okay. >> Which I think is a,
[31:40] I have not personally used it. This is where we're going to be learning it together, and that's cool.
[31:46] I strongly suspect that it's going to. Yeah. We'll see.
[31:54] If this ends up being an IDE along the lines of VS Code, I think maybe we should just do VS Code.
[32:00] That's nice. >> Okay. Well, we're done.
[32:04] >> Sure. Let's do that. >> Sure. Interesting.
[32:12] >> Another way to do this is through VS Code by installing the plug-in for Python.
[32:23] Lots and lots of options. This is not actually going to be,
[32:28] I misunderstood about what Mew is, and I thought it was going to be a way that you
[32:33] can just write Python in the terminal. It's not. It's basically like
[32:37] a little mini IDE along the lines of VS Code. We can use it for VS Code, whichever you like.
[32:45] >> What is IDE? >> Integrated Development Environment.
[32:58] VS Code is an IDE. >> Is that like Code Sandbox then?
[33:04] >> Code Sandbox can be integrated into an Integrated Development Environment.
[33:14] It is an IDE in itself, sort of. >> Okay. Then click "Mew" and we install.
[33:31] >> You know what would be fun? We could do Mew this time, and since we've already decided
[33:36] that we would love to do this again, we can do it in different ways.
[33:41] We can do it in Mew this time, we can do it in VS Code sometime,
[33:44] and we can do it in the terminal. >> Yo, it's Ben.
[33:53] He said, I need to start looking at getting these on the screen better.
[33:59] I like to think about IDEs as editors with superpowers. I like it. There's so much to learn here.
[34:13] Ben, as a random update, because I tagged him in this,
[34:17] I had a very curiosity question of this weekend while this is installing of why GIFs don't come with alt text.
[34:31] >> Yeah, I think I saw that conversation. >> Yeah. I haven't started using my alt text yet like I should,
[34:39] but it's been in the back of my mind. I'm not typing them yet,
[34:44] but I'm like, "Is this what I should type?" So I just want to let you know, Ben,
[34:48] ever since you were on the show, now I'm stuck in my head thinking about it.
[34:56] The first time you run select a mode window will appear. Add a fruit, CircuitPython, BBC,
[35:12] Micro, PyGame0, and Python3. Select Python3.
[35:17] You can always change the mode later by clicking "Mode" button. Open. Interesting. I don't know why I'm so fascinated about this right now.
[35:43] >> Yeah, it's just fun. I haven't seen it. I haven't used it before. I love the little sneaky thing and its little friend.
[35:54] Was it a bird? It's gone now. It had a friend. >> Did it eat the friend?
[36:00] >> It didn't. It is a bird. >> I think this is also like I've been doing
[36:12] all JavaScript for like the last month and a half that now redoing this on Python,
[36:18] I'm like, "What is all of this? It's so different."
[36:23] >> Python3. Yes, that's the mode we want. >> All right.
[36:28] >> That was fun. All right. Make this, see if we can get these guys next to each other.
[36:36] Ben got us back on the alt text. Anthony did a great job tackling that.
[36:44] Basically, alt text is contextual and two people posting the same graphic might be doing so for
[36:51] different reasons and to different audiences. It's hard to specify one true alt text for everyone,
[37:00] and even if GIF keyboards did supply predefined alt text, they probably also need to support a bunch of languages,
[37:07] user might speak, etc. A really hard problem.
[37:12] >> Touche. >> Touche. I was also thinking about it like on,
[37:17] oh, really quick as not knowing the context of the GIF. Maybe that's just me not knowing
[37:26] GIFs, like how to use them properly. >> There are all kinds of GIFs that I
[37:33] don't actually know where they came from, but I've seen how they've been used.
[37:38] You see it used in the same context a few times, and so you get to understand what folks mean.
[37:44] >> Fair enough. What up, Anthony? >> Right. This book uses Mew as an editor and interactive shell.
[37:52] However, you can use a number of editors. The integrated development and learning environment software
[38:01] installs along with Python, and it can serve as a good second editor.
[38:07] >> Let's back burner idle since we have Mew running already. >> Cool. That's why I was like,
[38:14] wait, what? We got interactive shell. When you run Mew, the window appears,
[38:19] and it is called File Editor Window. You can open the interactive shell by clicking the Repel.
[38:27] >> It's pronounced Repel. >> Repel?
[38:30] >> It turns out, yeah. >> Button. A shell is a program that lets you type
[38:38] instructions into the computer like terminal or command on command prompt on Mac OS respectively.
[38:45] Do we need idle with Mew? >> Mew, it has an interactive shell,
[39:00] so we're looking at it right now because that's where it says write your code here.
[39:04] That's where you can type. >> Okay.
[39:07] >> That's the shell. >> Okay. Cool.
[39:13] >> We don't need to be looking at idle right now. Shall we hello world?
[39:27] >> Yeah. >> All right. In a Python context,
[39:33] to print, you just print and then in parentheses, you write your string in either single quotes or double quotes.
[39:41] This is something that had me messed up the other day for an hour and a half because I come from
[39:49] Python world where you can use single and double quotes depending on what you like.
[39:54] Single quotes are more common. I am currently learning Go,
[39:59] and you can't just use single and double quotes interchangeably, but it didn't want to tell me that that was what was wrong.
[40:07] I spent an hour and a half trying to figure out what the fuck was wrong with my code,
[40:11] and it was because I used single quotes and it wanted doubles. >> Yeah. That is something that I've also just learned
[40:19] Go actually exists. Then let's enter
[40:38] the interactive shell should display this prompt. >> Okay. Maybe let's try that.
[40:49] Maybe we need to configure it. Yeah, we need to save the file.
[40:57] >> [inaudible] >> What's everybody else working on today?
[41:08] Because this is exciting and yet really nerve-wracking doing this. Save as, Laura is cool.
[41:24] It worked. Anthony recorded a podcast about TypeScript. >> Nice.
[41:34] >> That is exciting. I'm going to learn about TypeScript in September. You've given computer instruction and it did what it told you to do.
[41:44] Well, this is where it talked about PIP, but we don't necessarily need to do
[41:54] installing third-party modules right now, right? >> At the last sentence of that paragraph,
[42:02] it says consult appendix A when this book instructs you to install a particular third-party module.
[42:07] Yeah, we can back-burner this and it will let us know when we need them. This is one of the reasons that I think that this book is exceptional.
[42:19] Because not very many books or courses teach you how to find solutions to your coding problems on the Internet,
[42:30] like actually teach you how to do it, and this one does. He gives this example.
[42:41] For example, let's cause an error on purpose. We're going to enter string 42 plus 3.
[42:49] So with nothing with it, which is going to be weird.
[42:55] String 42 plus 3, enter. >> What if you stop and then run it again?
[43:13] >> Click "Stop" and then run. There we go. Type error,
[43:22] it can only concatenate, and concatenate means put one in front of the other,
[43:29] a string, not an integer. It's saying, I don't know what on earth you mean when you say to
[43:36] stick this string to attach this string to this integer, this 42 string to this integer 3.
[43:44] Makes no sense. Then what do we do? This error message appears because
[43:49] Python couldn't understand the instruction and the traceback. That's important because if you end up on Stack Overflow,
[43:57] people will sometimes ask you, what's the traceback and knowing what that means is handy.
[44:05] >> Is a traceback like a trace route when you need to be able to find where something is not connecting,
[44:12] like a website is not connecting with the server or only connects to localhost or something like that?
[44:19] >> If you look at it, so it says traceback and then in parentheses,
[44:23] most recent call last, and it gives you the file.
[44:26] It tells you where that's running on your machine. Then he says, if you're not sure what to make of
[44:37] a particular error message, search for it online. You just copy and paste that whole traceback
[44:45] and then search for it in quotations. Let's just do that just to see what that looks like.
[44:54] That type error can only concatenate string not into string. Copy that whole thing and open up a search engine.
[45:07] Put and search for that in quotation marks. Yeah. The quotation marks matter,
[45:15] as you may already know, because that way we're searching for,
[45:19] we want these exact words in this exact order. That way we're going to find this exact error message.
[45:28] If you go back to automate the boring stuff and scroll down.
[45:38] He's got a little image of what that looks like, like we just found,
[45:46] and says that you'll often find that someone else had the same question as you,
[45:50] and some other helpful person has already answered it. Then he goes on to talk about how to ask smart programming questions.
[45:59] This is another mind-blowing moment, because this is almost the only time that I've ever seen it in a course or a book,
[46:07] where they actually teach you how to ask good programming questions. That's a total skill.
[46:14] We don't need to read all of this. I just wanted to call it out because I think that it's so exceptionally good,
[46:22] that when we're asking good programming questions, we want to explain what we're trying to do,
[46:29] what we've already done, exactly how it failed to do what we expected it to do,
[46:35] and all of that kind of stuff. This is a great, if we come up with a question,
[46:42] we can refer back to this page, and make sure that when we ask a question,
[46:47] we are asking it in the most efficient way. The more efficiently we can ask a question,
[46:57] the more likely we are to get our question answered. The friendlier people will feel toward us when they are answering our questions.
[47:06] It's a total thing. >> Interesting.
[47:11] >> Yeah. >> Okay. I can go through those all later.
[47:15] >> Sure. Yeah. I mean, we don't need to look at that specific error message, just that this is an example of how,
[47:24] say we found this error, this is how we could debug it by figuring stuff out for ourselves,
[47:31] by looking for answers online, or by actually asking questions like on Stack Overflow,
[47:38] or as he specifies here, he blogs, Alice Weigert does,
[47:44] and is on Twitter and Reddit. >> We made it through Chapter 1.
[48:00] >> Chapter 0. >> Chapter 0. We made it through Chapter 0.
[48:04] We're getting somewhere. >> Yeah. If we click that right arrow,
[48:09] then we'll be in Chapter 1. >> I don't know if everybody else is seeing this as,
[48:17] this is something that I don't need to use it right now because I don't think anybody will hear it with using StreamYard.
[48:25] But this is how I get through online text, is a plug-in called something.
[48:37] It is called Natural Reader. >> I use that too.
[48:44] >> Yeah. It helps so much. It's definitely something I highly,
[48:48] highly suggest if anybody has a hard time with this stuff. Because it used to be they didn't exist,
[48:53] which they do now. So you can catch up on everybody else,
[48:57] even if you're dyslexic. >> I'm not dyslexic,
[49:03] but I use it because with my ADHD, I'll realize I've read five paragraphs,
[49:09] my eyes moved over them, but I stopped paying attention
[49:13] to what my eyes were looking at two paragraphs ago. Whereas if I can listen and do something with my hands,
[49:19] I can actually retain all the information. The other thing that I use it for is when I'm writing,
[49:26] I have it read my writing back to me. >> Yes, 100 percent.
[49:31] >> Yep. Make sure that I'm not missing words, because that's a thing that I do.
[49:36] >> I have things that are fun to mess with while I'm learning other stuff.
[49:41] I totally get that. >> I used to work in a bookstore when I was a teenager,
[49:45] and one of my co-workers, her son-in-law was the guy who invented that.
[49:50] >> What? >> The hand thing that you're doing, the pin.
[49:54] Yeah. Ward something. Anyway, yeah, he invented that when he was like 19.
[49:59] >> They don't make it like the pins anymore. They don't make the metal pins,
[50:02] they make plastic now. >> Yeah.
[50:04] >> Made me very sad. I found this at a garage sale, and I was very excited about that.
[50:08] But they don't make these ones anymore. But it actually has
[50:20] a wide range of syntactical constructions. >> Yeah, so programming concepts, sweet.
[50:37] >> Yep. >> Interesting. Then we're using an interactive shell right now.
[50:49] >> Yep. >> Then it's called, you said, REPL?
[50:53] >> REPL. >> REPL, which is read,
[50:58] evaluate, print, loop. Python instructions at one time instantly shows you results.
[51:08] Cool. This is showing how to go into Mew and wants us to save an empty file.
[51:23] We started a file, so we're probably just going to keep it the same.
[51:27] But says, two plus two should work now. We do it like this.
[51:35] Does that mean he has spaces? Is it going to work if I do it like that?
[51:45] >> It will. It's conventional to use spaces in between for readability sake, but the computer will not care either way.
[51:59] Click "Stop". Is REPL grade out? >> No.
[52:19] >> Okay, there we go. Type it in there. Then I'm going to go back over here for,
[52:37] so what's the difference between REPL and run? >> Notice that when you ran your program right there,
[52:51] it was running everything. It printed, "Hello, beautiful humans."
[52:56] If we had written like x equals two plus two and then printed x, then it would have said x equals four and so on.
[53:13] But it would do everything. Everything that you wrote, it would do all of it.
[53:17] Whereas in the REPL, it's running one line at a time.
[53:23] >> You have to type the line here for what you want it to run? >> Yeah. A REPL is really handy for if you
[53:33] want to check your syntax without running your entire program, which matters a lot more when you have
[53:40] a really big program that might take a while to run, and then you don't want to have to run something that
[53:46] takes five or 10 minutes to go, to figure out whether you've got your syntax right or whatever.
[53:54] It's a nice little way of checking if stuff's working one line at a time.
[54:02] >> Give me a second. I'm adding this to my notes of run versus. >> Cool. I'm not going to lie.
[54:20] I mean, it's similar, but it's still awfully confusing
[54:24] compared to JavaScript at this point. >> When you're comparing Python to JavaScript, what do you mean?
[54:38] The typing two plus two is confusing compared to JavaScript? >> In JavaScript, there's going to be more in front of this,
[54:53] like telling it what it's going to do, and then there's the spacing.
[55:02] >> That's also weird. Then just being able to, that there is a difference of run versus repel.
[55:16] >> Repel? >> Repel.
[55:18] >> Okay. But repel is not a Python thing. It's an everything thing. You can do this with JavaScript.
[55:29] >> Yeah. That's not a difference between Python and JavaScript. I think maybe what you mean when you say that there would be
[55:40] stuff in front of this is you'd have a variable declaration and you're going to in Python.
[55:48] If in that top window, you would be writing it with the variables.
[55:54] In the bottom window, in the repel, it's letting you just test things super fast.
[55:59] It's almost like it's a scratch pad that you can execute if that makes sense.
[56:06] >> Yeah. Anthony just said that I haven't been using a repel, so I can do the same thing there.
[56:11] The browser console is a repel. Interesting. Code sandbox would be a repel, I would think then.
[56:21] >> I haven't used it, so I don't know. >> Press "Option Command I" and you'll see a JavaScript repel.
[56:32] Code sandbox is an IDE. >> Yeah.
[56:37] >> Okay. All the fun things. "Option Command I." Press "Option Command I".
[56:50] >> Probably within the browser. >> Okay. Now it's starting to click.
[57:04] >> Yep. >> We're getting there.
[57:06] >> Yep. Right down there in that console was the repel. >> Got it.
[57:10] >> Yep. >> Got it. Okay.
[57:13] It's clicking now. I'm picking up what you're putting down. It looks like just looking at this,
[57:20] is where we were just about to get to expressions. >> Right. This is going to work exactly the same way as it does in math.
[57:29] This is another, a lot of the programming constructs and expressions and so on come from math.
[57:37] Because the only way that computers can do anything that we think of as thinking is they're always doing math. That's it for them.
[57:46] In math, an expression is like two plus two. It's not an equation because an equation has to contain an equal sign.
[57:55] This is an expression. We would need to give that an equal sign, in fact,
[58:02] if we wanted to assign it to a variable. >> Okay.
[58:10] >> Yep. In Python, so the expressions always evaluate down to a single value.
[58:17] If you said x equals two plus two, then the value won't be like a string two plus two.
[58:25] It'll be the value, the mathematical value of two plus two, which is four.
[58:31] You can say x equals four and you can say x equals two plus two, and those will mean the same thing.
[58:38] >> Okay. >> All right. Okay, so let's keep going.
[58:45] >> Errors are okay. Yay, glad to see that. >> Yep.
[58:57] >> There is a good link for error messages, which I will put that in the chat too.
[59:11] I'm also putting it in my own notes. Then use plenty of other operators in Python expressions too, for example.
[59:32] >> Okay. >> Let's put a pin in this table because we'll come back to it.
[59:47] More or less, it's going to work the same way as order of operations do in math. There are some exceptions,
[59:54] mainly to do with division. >> Okay. I don't know.
[60:06] I'm feeling a little noodled on. I got a noodle on it because I think something that would help before next time too.
[60:15] Of course, it's like learning that they, how do I say this? A lot of times when I've been learning like check Flask.
[60:28] Anthony, what do you mean? >> Flask is a framework for deploying Python apps to the web.
[60:37] Another one is Django, D-J-A-N-G-O. >> Okay, and check those out.
[60:48] Okay, that could be it too. It definitely, they're a lot different.
[60:57] But also, I don't think that when I started learning JavaScript, it wasn't like I was really comparing it to too much of
[61:05] anything because it was the first one I learned. Where now I'm like, as you said,
[61:09] with algebra, you have to unlearn and relearn what you already know. I'm picking up what you're putting down,
[61:18] yet at the same time, it's not fully sinking in. >> Sure.
[61:21] >> But I think having, oh, go ahead. >> Yeah, I think that at least for me,
[61:28] I understood English better when I started studying a foreign language, because I hadn't properly thought about what a verb was and so on,
[61:40] and where it fits in a sentence relative to other things. Whereas when you started studying French and then eventually Spanish,
[61:48] it was like, "Oh, okay, right." All these things that I've intuitively,
[61:53] I've never really thought about these things and how they fit together, but I intuitively understand
[61:58] because I've been speaking English all my life or whatever. I think it works out to be the same thing with programming languages.
[62:05] You learn your first programming language, and then when you're learning your second one,
[62:10] you understand your first one better, because you can map all these things that you intuitively
[62:16] understood to a more formal infrastructure, if that makes any sense.
[62:24] Like here, you learn like NPM was just like, this is the command,
[62:30] you wave your magic wand, you say NPM, and then things install.
[62:34] But what is that? It's a package manager. That makes more, I understand NPM better now,
[62:40] because now I know about the existence of PIP, which is another package manager.
[62:46] >> I think it's also like, it does. I thought that all package managers were basically the same,
[62:53] like that I did not realize that NPM was specific to JavaScript. Yeah. Yarn. I was struggling with yarn.
[63:05] What do you mean you learn the metalanguage, Anthony? I don't know if I understand that.
[63:13] >> I'm going to speculate. Like if you're learning something meta,
[63:19] you're learning, instead of learning in a math context, like you can learn math,
[63:27] or you can learn about specific mathematical types of constructs. Or in a language, for instance,
[63:34] if you're learning, you can learn Spanish, or you can learn about this is a verb,
[63:38] this is a noun, this is conjunctive, or whatever. Those are meta, like those are characteristics of a language,
[63:48] or any language really, but not just characteristics of Spanish or English.
[63:55] >> Yeah. >> It's a level up.
[63:57] >> Yeah. Anthony said the metalanguage is how languages work, and then Jay said Python has PIPX,
[64:11] but isn't nearly as possible, but it does something similar to like NPX.
[64:19] He was mentioning NPX. That is still confusing for him.
[64:23] Okay. Yeah. I'm excited that Laura has signed up to be on the show multiple times.
[64:29] >> Me too. >> Because it's definitely very, very interesting.
[64:34] It's just also a little mind-boggling, because even the install process was
[64:41] different in not installing it through terminal, installing it through the Finder view,
[64:49] which you would think is just super simple. That's how I've installed all my other programs,
[64:55] yet when it comes to a language, I wasn't expecting it,
[64:59] because I've done everything else through terminal and I'm like, "Oh, that makes sense."
[65:04] It's just thinking it through. >> Yeah. A lot of the things that you can install through,
[65:12] say, NPM or Yarn, you can also go to their website
[65:15] and download it and install it that way. >> Okay.
[65:19] >> Yeah. >> Yeah. Great.
[65:28] It's definitely something that is going to take a bit to sink in, and I'll read through the next couple of chapters
[65:36] first before we have our next session. Because I'm like, this has taken me a minute to put two and two together,
[65:48] especially since there's stuff that is somewhat repetitive, but we may not need to use like,
[65:57] I'm trying to go back to it for an example. >> You're not sharing your screen anymore.
[66:04] >> Yes. Yes, I know. Not realizing what impromptu is?
[66:15] Is that what it's called? >> I'm not sure. Can you show me?
[66:21] >> I have to go back to it. I can't find it. >> Gosh.
[66:24] >> There we go. But it's also like learning the idle terminology, that kind of stuff is also been new,
[66:36] but REPL is new. It's also just like, I just haven't had a chance to learn them yet.
[66:44] So like you said, even though it's like I'm learning what a noun is. >> Yeah, exactly.
[66:51] >> Also mind-boggling where I'm like, "Oh, that's what it's called.
[66:54] I never knew that was a thing." >> Right. Exactly. Yeah.
[66:59] I guess I would hate for, sometimes if a person is struggling learning
[67:07] something because there are a bunch of other things that they need to learn along with it,
[67:12] it gets like a bad rep or whatever for being hard. Actually, math is one of those.
[67:18] So I would hate for it to come across as like, "Oh, Python is so hard because you have to learn all this stuff."
[67:26] All this stuff applies to all the programming languages. >> Yeah.
[67:29] >> Everybody can use a REPL and everything has expressions and so on. Assignment operators, all of that kind of stuff. All of them do.
[67:42] >> Yeah. I think this is a great start to learn what I know about another language already.
[67:50] So I think that is a great example to be able to explain it to others. >> Can you set up a GitHub repo and push your README?
[67:58] >> Yeah. Okay. Let me get back there. There we go. Let's see. Ramon says, "Eventually, those concepts will
[68:07] carry over with different names with experience," and that's a total thing. Just like people say, learning your first language is hard,
[68:14] and then it gets easier and easier because you get a sense for like, "Okay, how do I do this?"
[68:20] Instead of thinking like, "Okay, well, what is a while loop?"
[68:24] Then when you learn your second programming language, you say, "How do I do a while loop in this language?"
[68:32] >> Yeah. Anthony, it's just in notes, but I am making myself a README just to let you know I am doing that.
[68:43] I am learning and getting the repetition of that, even though I'm also writing it as a,
[68:51] "Hey, Jen, remember what the differences are." >> Okay. I don't remember how to make a repo.
[69:03] >> Let's go to GitHub. >> There are lots of different ways to do almost all of these things.
[69:12] >> Yeah. We're up there. There we go. I don't know why it's in white right now, but it's white.
[69:19] I said the other day that I made my first repo, and I guess I didn't.
[69:25] It was more of like, this is the first one that I've realized that I made.
[69:30] >> That's a thing. Sure. >> Didn't realize. I guess I could create a new repository.
[69:37] >> Absolutely. >> Sweet. Laura is cool.
[69:46] >> [inaudible] >> I would. Strictly to make it easier for you to find it in the future.
[69:56] >> I know. >> If you want to share it with anyone else,
[70:00] they won't understand why I'm cool. >> That's what I'll start doing the next.
[70:15] >> Add a read me. >> There you go.
[70:16] >> Yes. >> If you're going to make a read me,
[70:19] I would recommend that you make your repo public instead of private. Well, more like, I guess it's the other way around.
[70:27] Usually, a read me is for the sake of other people. I mean, it could be for the sake of you,
[70:33] but if you want other people to be able to see it, I would do public. >> I'm cool with making them public because if I
[70:44] go back here, we're going to go. Look, it's black now. It was white like two seconds ago.
[70:49] Anyway, go into my React app. What I did with Anthony last week is, yes,
[70:57] all of this up here is for others, but I put gen notes at the bottom because I'm like,
[71:05] I get that this is for everybody, but these are things that I got stuck on,
[71:08] so maybe other people got stuck. >> Yeah. Using this as a framework for putting together a blog post,
[71:18] eventually, makes a ton of sense. In fact, what is it?
[71:25] Jason Langster had a post last week, I think. Yeah, it was last week called How to Turn One Piece of DevRel Content into 10.
[71:37] >> Yes, I saw that one. >> This is along those lines.
[71:41] You can make your repo with your readme and then you can use that to build out your blog post,
[71:48] and this is a stream already, so that's three. >> Yes, and if I make clips of it and also the transcript,
[71:55] and yes, there's so much in it. We're not going to do a get ignore.
[72:02] >> You can always add one later. >> We don't need a license right now, right?
[72:06] >> I mean, there's no harm in choosing, usually, the most common are Apache and MIT.
[72:14] I genuinely have no idea what the difference is between those. I think I usually default to MIT,
[72:23] strictly because the first time I had to make that decision, I looked to see what some other group was using and it was MIT.
[72:34] I was like, "All right, I'm going to do MIT." >> Yes, if you click "License".
[72:40] >> Really quick, I'm just going to show this on here. This is the link to go find Jason's DevRel breakdown 1-10,
[72:52] and we will do "Licenses" and go to "MIT" and "Create". >> Okay.
[73:04] >> Yay. It's got two whole things. >> Yeah.
[73:09] >> Okay, cool. Then I will go into the README and
[73:15] create it from what we did so far today. >> It's already created.
[73:20] >> Yeah, but I meant like add my notes. >> Mm-hmm.
[73:24] >> Yeah. Now that I'm in here, I don't even know if I can.
[73:29] >> You can edit it here. >> Yes, absolutely.
[73:33] >> Oh, that's exciting. Y'all, I haven't done much in GitHub now that I'm learning it.
[73:41] Jay just said, "Also be sure to add a code of conduct as well if you're going to have folks contribute."
[73:55] I'm going to say, "Hey, Ramon on our live stream on Thursday,
[74:02] can we go over what the code of conduct for them are so I can see an example?" >> Ramon and I have in the past worked on a code of conduct for our companies.
[74:15] Ramon said, "Hey, you know where we should start? We should start with free code camps,
[74:21] code of conduct because they have an excellent one." >> Okay.
[74:25] >> So, yeah. AJ's linked to another one as well.
[74:33] >> Yeah. Oh, hey, this is cool. Jay, is this what you normally use for them,
[74:43] or do you use something else? I'm going to the second link.
[74:46] Oh, cool. In the other version of it. >> Oh, nice. I didn't know that, Jay.
[74:57] >> GitHub has a template built in as well. If you create a new file with the name code of conduct,
[75:10] it will make the file default. >> Thank you, Jay. That is awesome.
[75:15] >> Go find where I put this. Too many tabs, y'all. Too many tabs.
[75:21] Okay. If I go here and I add a file, create new file, and I want code of conduct.
[75:38] >> MD is the file extension for Markdown, for anybody who's wondering.
[75:51] >> Good call. Oh, and there's also a choose a code of conduct template right here.
[76:00] Mean words right now, y'all. >> It's a thing.
[76:04] >> Look at the right. Okay. >> Yeah. I think that's that code of
[76:09] conduct template button that you were just. >> Yeah. Jay, I feel like I need your help with VS Code
[76:16] because I try to open stuff in VS Code from terminal and it doesn't work.
[76:22] >> Oh, I know this one. Or we can wait for Jay. >> Well, you know how you sent me the link of how to fix it?
[76:30] I may have broke terminal. >> Can't have broken it.
[76:37] >> No, you couldn't do LS lookup or CD or anything. It's pretty entertaining.
[76:44] Yeah. Anthony, help me figure that out. But that's why I was like Jay.
[76:54] I need your help at some point. This is cool. This is actually really, really cool.
[77:02] If I go review and submit, you work with folks on VS Code Python experience.
[77:19] >> Score. Way more informed than I am then by far. >> Jay is so informed and super knowledgeable on all of this stuff.
[77:31] I will say all of you are. All of you are really cool and helping me figure this stuff out.
[77:36] I'm going to commit this file. Oh no, I did a new branch.
[77:42] >> That's okay. Then we can merge it. >> Okay. Pull requests, is that where you would merge it?
[77:52] >> Sure. Click the green one down there, create pull request. >> Okay. Now, if this had anything more going on,
[78:05] you'd want to maybe review it or well, since it's only you in here at the moment, you're good to go.
[78:15] But yes, so you can merge pull request. >> All right. Confirm merge.
[78:22] >> There we go. Now you can delete your new branch. >> Okay. Then go to, yay.
[78:34] >> Yay. >> I'm going to put that in my notes too because that was dope.
[78:42] >> Me too. Let's put this over here so I remember to put it in my code, in my notes. All right.
[78:53] >> I keep forgetting that VS Code is a Microsoft thing. Jay just got to Microsoft earlier this year and I was like,
[79:03] "Microsoft, why does that matter?" Because good morning Laura,
[79:07] VS Code is a Microsoft. >> Right.
[79:10] >> I swear I'm awake. >> Yes, Jay, come join the stream.
[79:14] I will give you a link later. >> Yes, thank you so much for coming. It's super helpful.
[79:19] >> This was, and so much knowledge drops and learning so much. >> One more thing.
[79:25] >> Yes. Oh, we're doing more. We got more. >> I just wanted to put your Python file into your repo.
[79:33] >> I mean, that would make sense. How do I do that? >> There are a few different ways we can do that.
[79:42] Let's start with maybe the GUI-oriented one, and then in a future stream,
[79:48] we'll do it from the terminal. >> Dig it.
[79:50] >> Okay, cool. Go into your repo and click "Add File", "Upload". >> I should probably make sure this is saved.
[80:11] >> Good call. >> Choose "File", and we went to "Desktop",
[80:19] "Code Folder", this one, "Open". >> We know this is the right file
[80:24] because the file extension is .py, so we know this is our Python file as opposed to
[80:30] any of the other things that could be there. >> We're going to direct it directly to the main branch
[80:37] because there's not an already existing file to go see the changes. >> True. If you had other people collaborating on this,
[80:52] even though there aren't any changes, you might want somebody to review it just because it's new.
[80:59] >> Got it. >> In that case, you would make a new branch,
[81:03] put it there, let them review it, and then assuming it's all good, then merge it in.
[81:07] >> Cool. All right. Hey, it's there.
[81:13] Yay. I don't know why I'm so excited about this, but it is there.
[81:21] It's a lot of good practice. That is why I love it.
[81:24] >> You have a Python file, and you have a repo, and a readme, and a code of conduct.
[81:31] >> Yeah, first code of conduct today. >> Yeah.
[81:35] >> I'm slowly building it up. Yay. Oh, we got a Python,
[81:42] and I have CSS in here. I also have multiple accounts that I don't know what to do with,
[81:49] which I will figure that out at a different point. Sweet. Thank you.
[81:55] >> I think we have hit all of our targets today and then some, which is pretty cool. Thanks to Jay for that.
[82:04] >> Yeah, we got the crowd going. This is the one thing I love about live streaming,
[82:08] is it's such like a community. >> Absolutely.
[82:12] >> So much learning. All right, cool. Well, everyone, thank you for joining today,
[82:18] and yes, all the green squares. Yes, with Ari, I get really happy about the green squares.
[82:25] I need to get more green squares, and I'm learning. I am learning.
[82:29] I have no idea what I'm doing for co-working tomorrow, but it's probably writing read-me's on stuff.
[82:37] >> Nice. >> Probably what I'm going to be doing.
[82:41] So thank you, thank you so much everyone, and we will see you.
[82:47] I'll see everybody tomorrow, but we'll keep you posted when Laura is coming back on.
[82:52] >> All right. >> Thank you. Bye, everyone.
[82:55] >> Thanks, Jen. 
