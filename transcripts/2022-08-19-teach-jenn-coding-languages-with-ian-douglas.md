---
showLink: "https://www.youtube.com/watch?v=rPlh0H2PRvU"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-coding-languages-with-ian-douglas"
title: "📚 Teach Jenn Coding Languages with Ian Douglas 📚"
publishDate: "2022-08-19"
coverImage: "https://i.ytimg.com/vi/rPlh0H2PRvU/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Thank you again for joining Teach Gen Tech.
[00:05] Today, we have an awesome guest from Postman, Ian. I'm very excited about this because you are
[00:11] like the one DevRel that I have met in person. I'm like, "Yes." We met at the API Denver meetup last month.
[00:21] Ian, please introduce yourself and what you're going to be teaching us today.
[00:25] >> Sure. Hey, everybody. I'm Ian Douglas. I'm a Senior Developer Advocate at Postman and I'm on the clock,
[00:31] so I'll be here for a little bit. But yeah, shout out to my employer
[00:38] that lets me do crazy things like this. Let's see, I've been in the tech industry a long time.
[00:44] I joke, I'm an old dinosaur in the industry. I've been doing this for 26 years,
[00:51] and I've had people on my live stream and people in my classrooms that are like, "Dang,
[00:56] you've been coding longer than I've been alive." It's like, "Yeah, thanks."
[01:00] Actually, this month, August, is the 40th anniversary of when
[01:06] my dad came home with a Commodore 64 computer. I was eight years old and that's when I learned how to code.
[01:11] I basically taught myself the basic programming language. Technically, I've been coding for 40 years,
[01:17] which is ridiculous to think about in and of itself, but professionally, I've been doing it for 26.
[01:23] It's been a lot of fun just seeing all the different programming languages and
[01:28] seeing the different technologies and things like that over the years,
[01:32] especially over the last 10, 15 years. So much has changed in the past decade especially.
[01:37] What I wanted to go through today is, I know Jen's been learning some Python
[01:43] and also had some curiosity around JavaScript. What we're going to talk about today is,
[01:50] what are some use cases for Python and JavaScript and how do they work together and so on.
[01:55] I've got a handful of things to show about how I use Python and how I use JavaScript.
[02:01] It's not just for JavaScript in the browser and it's not just Python for back-end code and stuff like that.
[02:09] So I thought we'd dive in on a few of those things. I'll share my screen and walk through some of
[02:14] the little bits of code and stuff that I've been doing, maybe some stuff that I've been coding for work.
[02:19] Yeah, we'll have some fun with that. >> I do have a question just because when people say back-end,
[02:28] I feel like a lot of people can conceptualize what front-end is because
[02:35] it's mostly set about websites and that kind of thing. But when somebody says back-end,
[02:42] is that talking about, let's say, it's what's run on a server
[02:49] or how would you explain back-end to somebody that has no idea what it is?
[02:54] >> That's a great question. I would typically classify it as code that runs on
[03:00] a server where you don't necessarily have a user interface, something like in a browser that
[03:09] someone is directly interacting with. When we work in the browser,
[03:13] we're generally interacting with the HTML, which then interacts with the JavaScript.
[03:20] But then the JavaScript, if it has to read and write things to a database,
[03:24] that JavaScript isn't directly talking to a database usually. It's going through some other software
[03:31] and then it's going to the database from there. It'll ping some other bit of software,
[03:38] which is what we call the back-end of what we do. The front-end is like
[03:42] the customer-facing or the user-facing software, and the back-end is what's behind the scenes.
[03:47] We can almost use an analogy of a restaurant where we have what we call front-of-house and back-of-house.
[03:54] Front-of-house is all the serving staff, where the back-of-house is all the people cooking your food.
[04:00] The people that you interact with as a patron of the restaurant, you're interacting with the servers,
[04:08] and so you're dealing with the front-end of what happens in the restaurant.
[04:12] Then they go and play a liaison between you as the customer
[04:19] and what actually needs to happen in the kitchen, so that you have a good user experience at the restaurant.
[04:24] They go and they'll take your orders to the back of the restaurant where they cook your food,
[04:29] and then they bring the food back out to you and bring you back that result.
[04:33] When I talk about back-end code, I'm usually talking about the folks in the kitchen who
[04:37] are preparing all of that food or data in order to give back to
[04:43] the front-end code to then give back to the user in some way. If you fill out a form,
[04:50] the JavaScript front-end might be processing that in a way that it can transfer that data efficiently to the back-end.
[04:57] The back-end then is going to look through that data, maybe do some validation on it again,
[05:02] and then save that in a database, or if you're trying to retrieve something,
[05:05] it's going to go get it out of the database, but it has to package that back up in a way to send to the front-end.
[05:10] But the front-end, we generally don't want to show you just raw data, we want to format it in a way that presents well and looks nice and so on.
[05:19] The front-end code will usually take that raw data coming from the back-end and format it in some way so
[05:25] that it shows up as a nicely formatted list and so on for the user. >> Very cool. I like the explanation.
[05:31] I also know that restaurants are also used very often as a way to explain APIs, so I feel like that is something that we can build upon another day.
[05:44] >> Yeah, for sure. >> You said that you have some examples because I think that's another thing of,
[05:52] first off, explaining what front-end and back-end is, but understanding when you would use them and why.
[06:02] Granted, the way I wrote the title on this was like, why use JavaScript versus Python?
[06:10] I meant it as when do you use each? I think that's a really cool thing of,
[06:18] yes, JavaScript is used very often and can a lot of people consider JavaScript easier to learn?
[06:26] A lot of people say Python is easier to learn. I would say no matter what,
[06:30] the first language is easier, the second language is really hard,
[06:34] and then the rest of them are easier. Because it's like you're comparing it to what you know on your second one.
[06:41] >> Yeah, that's a good way to think about it. Some people think about programming languages a lot like spoken language,
[06:48] where the first one that you learn, that one is going to come easier to you because you have a lot of
[06:55] coaching around like learn to say your words and then people help you enunciate and how to put the grammar and the structure together.
[07:02] When you learn that second language, you're on your own and you're right,
[07:06] it is that comparison of if I do it this way in English, I need to say it this way in Spanish.
[07:12] But then once you learn a couple of languages, if you're in that same family of languages like Latin-based languages,
[07:22] if you learn Spanish, you're probably going to learn French and Italian much
[07:27] easier because the grammar structure is the same and a lot of the actual words are very similar.
[07:35] You'll start to spot those similarities and go, "Oh, if I do it this way in this language,
[07:41] I do it this way in this other language." So it also translates well into programming languages
[07:46] where JavaScript and Python and Ruby, they're what we call high-level languages.
[07:52] They're interpreted languages, which means it gets loaded by some processor that's then interpreting
[07:58] everything line-by-line in order to go run those instructions. Where compiled languages, they tend to do what we call strongly typed,
[08:07] which means if I make a variable, I have to define it as a particular data type.
[08:12] This variable is going to be a string and this variable is going to be a floating point number.
[08:17] This variable is going to be an array and that array is of integers. That variable can only store that type.
[08:25] Where in JavaScript, we could say var whatever, and we can assign it a value of five,
[08:33] and later we can assign it a value which is a string, and later we can reassign it again as an array,
[08:38] unless we make it a constant. But if we make it a var or a let,
[08:41] then it becomes this fluid data type that we can change whenever we want. Python is the same way, Ruby is the same way.
[08:48] So some of these high-level languages, they don't lock you into a type when it comes to how you declare a variable.
[08:56] That allows for a lot of flexibility. But in these compiled languages,
[09:01] usually you have to set a data type saying this variable can only ever be a string, and if I need a variable to hold a number,
[09:07] I've got to make a whole new variable. So it's good and bad because it forces you into
[09:15] a better way of thinking about how you're actually organizing and storing your data. But then as you learn a couple of compiled languages,
[09:23] learning other compiled languages, it's just like, "Oh, yeah, okay.
[09:27] I need the data type and the variable and integers are integers, and floating point numbers are going to be floating point numbers."
[09:34] It's just this programming language calls it int32 or int64 for how many bits you're storing in that number,
[09:43] where something else is going to literally spell the word integer, and another language might just say int for integer and short form it a little bit.
[09:53] But at the end of the day, it's like you can glance through
[09:57] that code and have a pretty good understanding of what it's doing. So if you're learning JavaScript,
[10:02] looking at other high-level languages, you're going to grasp probably 75 percent or more of what it's doing,
[10:09] because the structure of it is going to be the same, and the syntax and the grammar of what you're looking at is going to be roughly the same.
[10:17] So all these languages have the same kinds of instructions, like how to iterate over an array,
[10:25] map, and filter, and things like that. >> What are some compiled languages?
[10:30] Because you mentioned the other ones, but I just want to think of-
[10:34] >> Yeah, for compiled languages. Yeah, I would think of like C++,
[10:37] Java, Go, Rust, things like that. Where with an interpreted language,
[10:44] like when I go run a Python script, I have to say, "Hey, Python interpreter,
[10:48] go run this script." The first thing it does is it opens that thing and it scans
[10:52] through and make sure the syntax is going to actually execute properly. So it does a quick scan for syntax errors,
[11:01] and then it goes through and it actually runs the code line by line. In a compiled language,
[11:07] it does that interpretation one time and then compiles it into machine code so that later you can say, "Hey,
[11:15] just go rerun that machine code." Something already scanned it and made sure that it was going to work properly,
[11:21] and then you end up with just an executable file instead. Then you can just go run that executable file as many times as you'd like.
[11:28] So the initial time it takes to open the file or multiple files and scan through everything and check all that syntax
[11:37] and make sure that everything is structured well, that only has to happen one time in a compiled language.
[11:43] Where in an interpreted language, every time you want to run that script,
[11:46] you've got to say, "Hey, Python, go run that script again."
[11:48] It's got to open that file, scan all the instructions,
[11:51] make sure it's valid, and then go execute it. But the nice thing about it is you can go in and you can change that script at
[11:57] any time and then the next time I say, "Hey, Python, go make my lights blink in the background,"
[12:03] it's just going to go update that and blink my lights in the background. But in a compiled world,
[12:08] I've got to go change that source code, run the compiler process again,
[12:12] and that could take anywhere from seconds to minutes. So it's a little bit slower process of getting that executable.
[12:19] Now that I have that executable, it's going to run really fast all the time because it doesn't have to
[12:23] go through that interpreter work again and again. >> Interesting. So if I'm just comparing Java to JavaScript,
[12:32] Java would have to change the source code and be recompiled every time, where Java is much more lenient in letting us
[12:43] change things a lot faster and a lot quicker. >> So JavaScript on the second one.
[12:51] >> Yeah. JavaScript. What up, famous yak? Yes, the lights are so cool, aren't they?
[13:00] I heard you talking to me last night about wanting to put a warning on there.
[13:08] I'm like, "Yes, I totally get that. But at the same time, they're so cool."
[13:14] >> It is pretty fun. But yeah. So what I was saying on my stream last night is I want to either make
[13:20] them less bright when they blink or slow down how quickly they blink, or maybe just pick random ones to more twinkle,
[13:30] as opposed to all 43 of them on the wall, all coming up with these random patterns just for seizure trigger warnings.
[13:37] >> That's smart. >> I'm probably going to do some combination of all of them where I dim it a little bit,
[13:42] and then slow it down and not flash all 43 at the same time. Because right now it's actually going through and it's saying,
[13:49] "Hey, all 43 lights, pick a random number from 0-255 for red, green,
[13:55] and blue, set that panel to that color, and now go set all of them,
[14:00] and then do that again, set all of them, do that again, set all of them."
[14:03] That's why you get this really rapid, pretty wild blinky thing. That's all done in Python.
[14:10] >> Yeah. I think that's a really cool thing that that's an actual way that we can use Python where before teach-in-tech journey,
[14:21] I'm like, "Yeah, I know you have to code it somehow." Just like it never really computed how to get started on that or anything.
[14:30] I know you have some things to show us today. Where would you like to start?
[14:35] >> Let's see. Let's start with, well, let's talk a little bit about the differences between Python and JavaScript.
[14:44] Then maybe not in the history of them, but where they're commonly used right now.
[14:50] We'll start with that basis. I think most people understand,
[14:55] or if you've done some amount of programming, or if you've been looking into programming,
[15:01] you've probably seen or might have heard JavaScript is used very heavily, obviously, in browsers.
[15:10] It came to be back in the 90s, I think late 90s, early 2000s,
[15:18] where JavaScript was invented as a language in 10 days. They literally wrote the JavaScript language in only 10 days,
[15:26] and released it in the world. It quickly became picked up in the browser as like, "Hey,
[15:32] if you want code to actually execute in the browser, there's this JavaScript code."
[15:37] Now, they borrowed from the Java name because then they're like, "Maybe we'll get some more adoption."
[15:43] Because back then Java was coming up as a very popular language. Everybody was learning Java.
[15:49] If we call it JavaScript, then everyone's going to think it's related and they'll want to use it.
[15:55] That's honestly where it got a big chunk of its popularity. >> Are they similar?
[16:00] >> Stealing a name. No, not at all. They're not related whatsoever.
[16:04] >> Bakari says that JavaScript is his jam. I loved having him on the show too.
[16:11] I feel like I could have Googled it, but knowing that's how JavaScript got its name.
[16:20] 1995 is when it became first released. It was integrated in Netscape Navigator 2.0.
[16:30] >> Yeah. Really, really old browser. It's not even around anymore.
[16:34] Bakari, strawberry. Strawberry is my jam.
[16:38] That's how JavaScript got its start. Python has been around just as long.
[16:44] Python has been around for quite a while. The guy that invented Python actually
[16:48] modeled it after another programming language called ABC, which was built to teach kids how to code.
[16:54] His whole methodology of coming up with a Python language is, it needs to be easy to read,
[16:59] it needs to be easy to interpret and understand how it works. We want to make it as easy as possible to get other people into that ecosystem.
[17:11] So he spent a lot of time just making Python a very readable, easy to understand kind of language.
[17:19] If anyone remembers the old TV show, are you smarter than a fifth grader kind of thing.
[17:24] His whole mentality was like, everybody should be able to look through
[17:28] a Python script and have a pretty good idea what it's doing. There were other interpreted languages in the day like Perl,
[17:36] spelled like the precious stone without the A, P-E-R-L. It stood for Practical Extraction Reporting Language.
[17:46] Perl was a very fast language. It could read through text files and crunch through data really,
[17:52] really quickly, but it was very hard to read. Guido is the name of the guy that invented Python.
[17:59] He wanted something that was going to process and handle things just as quickly,
[18:04] but also be readable. So Python has been around for a long, long time as well.
[18:11] >> February 20th, 1991. >> Yeah, it's been around 31 years now, 31.5 years.
[18:20] Yeah, it's been around a while. I've been using Python professionally for a little over a decade.
[18:26] I've been doing JavaScript since the Netscape days back, not quite 1995. I think I started learning JavaScript in 1998 or so.
[18:35] >> Okay. I feel like this is where I get confused. It's like one of the popular questions on Google is,
[18:41] Python built on C, and the response is Python is written in C.
[18:45] Actually, the default implementation is called CPython. I'm just like, how do you write something on something else?
[18:55] Like it's a language on a language. >> Yeah. So if you think about,
[19:01] like if you had to sit down, and I'll be a good example of this.
[19:06] If you wanted to write some code that translated a piece of text from English to French,
[19:15] you would need to open that file, and you'd need to read it word by word,
[19:19] and understand the grammar of what it's trying to do, and then figure out, okay,
[19:23] what's the equivalent for each of these words? Now, how do I reconstruct that grammar and syntax in French,
[19:31] and then rewrite that file? That's effectively what they're doing with C,
[19:37] is they've got the C software. So C is a programming language,
[19:41] it's been around much, much, much longer since the '60s maybe,
[19:47] maybe '70s, I think '60s. It's been around a really, really long time.
[19:53] Basically, what it's doing is they're writing instructions saying, "Hey, when Python interpreter opens a file,
[20:00] and it sees these instructions, this is what we want the equivalent machine level code to do."
[20:06] So they wrote the Python language using the C programming language. It's basically, how do we write this interpreter,
[20:14] where we're looking at the instructions piece by piece, to try to understand what the programmer is trying to do with Python.
[20:23] >> Interesting. Hey, what up? Do I say your name?
[20:31] [inaudible] I hope that is close to right. Hello, hello, and thank you for joining.
[20:42] Bakari said, "Ogres have layers?" >> Ogres. Ogres have layers.
[20:49] >> Ogres. >> Yeah, it's a reference to Shrek.
[20:51] >> Ogres have, oh, okay. That's how you spell ogres?
[20:57] >> O-G-R-E-S. I didn't see how they typed it, yeah. >> If you click "Comments",
[21:03] you should be able to see all of their comments too. >> Oh, they're there.
[21:07] >> Okay, cool. Then I looked up the oldest programming language, which is, do you know what it is?
[21:14] >> The oldest one? >> The oldest one.
[21:20] >> I feel like I should know it, but I don't recall off the top of my head.
[21:24] >> Fortran. >> Fortran. Yeah, I learned a little bit of Fortran in college.
[21:29] >> What? >> Yeah.
[21:31] >> Okay, that's just cool. SQL is one as well,
[21:42] and that's just crazy. You are absolutely right.
[21:45] On C, it was released in 1972. You said the '70s.
[21:50] >> Yeah. >> This is just cool also learning about the background of it.
[21:55] >> Yeah. A lot of people started using Python for
[22:02] more system-level programming when it first came out, and just general programming of let's make a little game,
[22:09] or let's figure out how do I look through my file system and get a list of files and do something interesting.
[22:15] There's going to be a lot of system-level things that you'll see historically in Python.
[22:28] The main library that you see happening within Python is going to have a lot of different things.
[22:38] Somebody just did something on my system, which is why all my lights went a little haywire there for a moment.
[22:44] But for JavaScript, the default things that you're going to see in
[22:50] JavaScript are here's how to do things in your browser, here's how to interact with a button,
[22:54] here's how to fill out a form, or how to interpret things that somebody has typed into a form,
[22:58] and it's not necessarily the default, but this is where we most commonly use this language.
[23:07] Python got its roots in system-level programming, but of course, it's used in so many things now,
[23:12] it's heavily used in machine learning and data science, and it's also used quite a bit for back-end servers.
[23:21] But if you need a back-end code that's really, really performant, you'll start with a prototype in Python because it's very quick to write.
[23:31] But then you're probably going to rebuild it in a compiled language which is going to be more performant,
[23:37] depending on your needs. Some people will write something in Python and leave it in
[23:41] Python forever and it'll work just fine. Not everything has to be built at what we say Google scale,
[23:47] or scalable to millions and millions of users. Chances are pretty good if I write a dad joke API,
[23:53] it's not going to be used by millions and millions of users, it might be used by dozens.
[23:57] >> I don't know. I would share that one a lot. I definitely would share that one.
[24:02] >> Yeah. There are some that are very, very heavily used. But again, if it's a dad joke database,
[24:10] you don't necessarily have to build that out at Google scale using compiled languages and whatever
[24:16] because it's just a static list of jokes. When somebody calls the endpoint saying, "Give me a joke,"
[24:22] you're just going to give it back something that you've probably already holding in cache memory.
[24:27] It doesn't even have to be really that performant, as far as how you build up that code.
[24:35] Python today is being used for a lot of data science, and number crunching, and machine learning,
[24:42] and stuff like that, and it's very, very effective in those roles.
[24:46] JavaScript, on the other hand, has worked its way out of the browser,
[24:51] and you can also do some interesting things with that language as well.
[24:54] A lot of these programming languages nowadays are really general purpose languages.
[25:00] I can do system level stuff in JavaScript. I can do web-based stuff in Python now.
[25:06] Someone actually wrote an interpreter in JavaScript to interpret Python code,
[25:11] and so now we could actually be writing Python code in the browser to do what JavaScript is doing, and that's all I did.
[25:21] Similar to how the original developers of Python wrote it in C, someone else has done that work in JavaScript.
[25:28] Now I can write a chunk of Python code, and it'll actually translate it
[25:33] into JavaScript for the browser to actually execute. Very similar to what the C Python is doing,
[25:39] where it builds that Python interpreter and compiles it down there. They've basically done that in JavaScript.
[25:45] Now it does add another layer of complexity, because when I write Python code,
[25:49] it's got to go through that interpreter, and then into JavaScript, and then to the browser.
[25:53] There's a lot of extra steps, and so it's not going to be as fast as writing native JavaScript.
[25:58] Just like writing Python code isn't going to be as performant as if I wrote that code in C.
[26:03] >> Is it something that if they're writing it in Python, that after it's compiled and put into JavaScript,
[26:13] that they could copy and paste the JavaScript and just use the JavaScript? That way it runs faster instead of making it more complex?
[26:20] >> Maybe. There are tools out there that will do something like that, and we call it not really compiling,
[26:27] but we call it transpiling, where we're taking something,
[26:30] we're translating it and compiling it at the same time, and then we have some result at the end of it.
[26:35] As an example, TypeScript is another form of JavaScript, which is getting into that strongly typed language
[26:43] that we were talking about earlier, where TypeScript is going to basically compile down and
[26:50] transpile down into the actual native JavaScript that the browser needs. There's been a lot of work around how do we build
[26:57] the libraries and so on to actually build TypeScript, that when we compile it,
[27:01] it's actually compiling down into JavaScript to then run in the browser. You're writing it in TypeScript and it's
[27:07] going through all the interpreter stuff, but the browser is not reading and executing TypeScript.
[27:13] It's got to be rebuilt into JavaScript. In that case, you could actually go look at the resulting JavaScript.
[27:22] I'm pretty sure with this Python version though, it's actually just running all in the browser,
[27:28] and it's not actually compiling down in a way to actually then go view that JavaScript.
[27:32] It's just interpreting the instructions and building the equivalent JavaScript instructions instead.
[27:37] It's looking at the code going, if they do a for loop,
[27:40] then I also want to do a for loop that looks like this. >> Interesting. That is complex yet simple at the same time,
[27:51] and this is where I keep getting stuck in learning programming. Things can be very complex and simple.
[27:57] It's a thin line because it's like if you think about it more, the more complex it can be,
[28:04] even though the bare basics are pretty simple. Also learning so much of the time of
[28:12] when these languages came out and also building upon each other. I see that you have your screens. Let me bring that up.
[28:20] I've got a handful of different bits of code that I can show, like how I use JavaScript and how I use Python
[28:26] just for some of the stuff that I do on a regular basis. This first one is a little API that I wrote,
[28:33] and this also has a bunch of Python code in here as well. This is a little jukebox voting app that I built.
[28:40] Basically, what it allows you to do is it's an API. Well, there's two parts of it.
[28:46] The back-end is actually an API that you can hit where you can say, "I want to vote for a particular genre of music,
[28:52] as well as a decade of music." While this code is running,
[28:56] it's capturing people's votes over an API. I wrote this because we were doing
[29:01] a partnership event with this company called Infobip. They were traveling around the United States and they
[29:09] wanted some way of showing off what their software is capable of. They're a little bit like a Twilio where they can do
[29:16] SMS and chatbots and e-mail and all this stuff. I'm like, "I like chatbots.
[29:21] Let's build a chatbot in Infobip." What it allows people to do is you can go in and using an SMS chatbot,
[29:29] you can say, "I want to vote for rock in 1990," and it would register that vote.
[29:33] But then I wrote a front-end for it that basically queries the back-end saying, "Give me all the votes."
[29:41] It'll actually start playing a song based on which vote is winning. It sounds a little bit like a radio tuner
[29:51] where someone's hitting the button to play a different song. Whichever song is winning,
[29:57] it starts playing a fragment of that song. If somebody else's vote starts to,
[30:02] they got more votes for say pop music in 2010, it'll skip from playing Journey from 1980 to Taylor Swift in 2010,
[30:11] and it'll actually change the song at that point. >> It reminds me of a play now on the jukebox.
[30:17] >> Yeah. It's basically what it is. But imagine if you're driving in
[30:23] your car and you're just changing the radio station, and people can't agree on which radio station to listen to.
[30:29] When you hit that button, you're going to go back and listen to that other song,
[30:34] but time has progressed and so the song has also skipped ahead, and that's basically what this code is doing too.
[30:39] >> Okay, that's cooler. >> It's effectively starting all the songs at the same moment,
[30:44] but then as one vote. They're all playing at the same time,
[30:47] but right now, Journey is winning, and so it's playing Journey.
[30:51] Then later on if Taylor Swift wins, it changes as if somebody hit the button on
[30:56] the radio to change to the Taylor Swift at that point. >> So if you're two minutes into Journey,
[31:00] you're two minutes into Taylor Swift. >> You're two minutes into Taylor Swift.
[31:03] Yeah. It was really fun. Yeah. The API that I built out is literally just go collect some votes,
[31:12] and so it's storing everything in a Redis database. But they can call an endpoint to just say,
[31:20] go get the list of instructions where I'm saying, here are the list of genres and the list of decades.
[31:26] I can zoom in on that a little bit more. >> Thank you.
[31:30] >> Yeah. It's looking at how I've set up my music for this so if I have music
[31:38] set up in a particular way where I've got rock music and pop music, I can go run my jukebox player using that structure.
[31:45] If one of my co-workers is doing an event and they want hip-hop and jazz, they can set up the song structure that way.
[31:52] The front-end player is basically looking at how you set up your music structure here. In this case, I had rock music and pop music,
[32:01] and so you set up a folder structure saying these are the songs, and then it goes through and it takes that song and
[32:08] it actually breaks it out into all these three-second segments. When that vote changes,
[32:13] what it's doing is it's saying, "Okay, well, we're 30 seconds in,
[32:16] so that's 30 divided by three is 10, so I need to start playing fragment number 10 of this particular song."
[32:24] So the front-end is basically just going through and it's constantly pulling that API to say who's winning,
[32:32] and then it goes and plays that fragment of whichever song is winning. So the back-end is literally just storing the votes.
[32:39] So if we come back over here and look at what's happening here, I can go in and I can reset all those votes,
[32:44] and this is all written in Python. So this is a library called Flask,
[32:48] and it's just the back-end code of how do I receive a vote, and then how do I go get all this stuff out of the database to give this data back.
[32:57] So if they call just whatever my host name is with a slash, it's going to give them back the instructions on how to use the API.
[33:05] If they vote, this is an endpoint to actually go get a vote. They have to give us the genre of music,
[33:11] so rock or pop or jazz or hip-hop or whatever, and then the decade of that music as well,
[33:17] and then it registers both of those votes in the database. Then later on, it'll say, "Okay,
[33:22] go get all the results, who's actually winning the vote?" All it does is it goes out to the database and grabs
[33:27] that data and it just gives all that back. So on the front-end then,
[33:31] or what I'm calling the front-end is just a command line script that I run. This is going through and saying, "Okay,
[33:38] let's go set all this stuff about where to actually go find the fragments of the songs."
[33:46] Then let's see, somewhere in here, I'm actually calling the API.
[33:53] So this is just doing the setup of like, go figure out which fragment of which song to play.
[33:59] Doing some Postman authentication as well because we're doing all this stuff in Postman.
[34:04] So this is where it's saying, "Okay, go figure out who my current winner is."
[34:08] So this line of code in Python is using a library that says, "Hey, just go call this API or go call this web endpoint.
[34:16] Just give me back the results of what you got." So it does all of the hard work of how do I connect to that server?
[34:22] How do I send that request over? How do I get data back and put that in a result object?
[34:27] Then I say, "Okay, well, that result is JSON. Now go figure out who the winner is."
[34:31] Based on what the winner is and the decade of what's winning, go figure out that MP3 file and start playing that next.
[34:41] So it's queuing up all these three-second segments. It's pretty fun. You go to a meetup and you're like, "All right,
[34:47] everybody start voting for your music and we're going to start playing it as we go."
[34:51] It would start playing all these little fragments of music. Then people are like, "I don't want to listen to Bon Jovi.
[34:57] I want to go back to Whitney Houston, 1980 pop music or whatever."
[35:03] As they vote that over and over and over, that vote count starts to climb.
[35:07] As soon as that one starts winning, it'll switch to that song.
[35:11] So it's really fun. The first couple of seconds is like, "Okay. Well, everybody's voting for Journey."
[35:15] But like, "Oh wait, it just changed to something else. Wait, now it's back to Journey.
[35:19] Now it's back to something else." So it hits this critical mass of people who are just like,
[35:23] "No, I want to vote over and over and over and over and over." So it was a lot of fun to build this out.
[35:29] So this is just a command line Python script, which is going out to the file system and saying,
[35:35] "Go get that MP3 file that I've got on my file system somewhere and just start playing an MP3 file."
[35:40] That's all just done in Python code. So it doesn't have to be what we consider back-end.
[35:46] This is just system code. I think that's maybe just like the part
[35:54] that I may not comprehend yet, is when people say like Python command line.
[36:01] Yeah, just like when you put it in your terminal, I don't know where I'm necessarily getting mixed up.
[36:13] But so command line is written in many different languages, not just like a Bash language, I'll go with that.
[36:26] >> So when we open the terminal, it's running a shell and that shell is an interpreter,
[36:34] very similar to a Python interpreter or a JavaScript interpreter. It's basically watching all these commands that I'm typing,
[36:40] like the word source and behind the scenes, it's interpreting what I'm writing and it's actually going to
[36:47] go do some things at a machine level to say what is it that Ian's trying to do here.
[36:53] In this case, I'm trying to activate a virtual environment. So Bash, in this case is my shell terminal,
[37:01] is just an interpreter. It's watching the instructions that I'm
[37:05] manually typing in and saying, "Okay, you type the word source."
[37:09] That means that whatever follows, I need to actually go execute that code.
[37:13] That code is basically saying, go set up my Python virtual environments
[37:16] that I can actually come in here and say, now I want to run my Python interpreter to go do
[37:22] my jukebox player and I can say Python 3. Now this would actually be playing
[37:37] my jukebox player at this point and connecting to that API and trying to figure out who's winning.
[37:42] Then it starts playing the MP3 files in the background based on who's winning.
[37:48] I don't know if you can hear the audio. I don't know when it shares my screen,
[37:52] if it shares the audio or not. But what it's doing is it's basically going through saying,
[38:01] let's see if I can stop it here. It went through and basically it was running through and
[38:09] figuring out who was winning and then playing the audio segment of that file.
[38:14] >> Very cool. Interesting. >> That just runs in a terminal,
[38:18] and so the actual player just runs in the terminal. The back-end code that I wrote,
[38:23] the actual API is actually running on Heroku. It's a hosting platform where you can
[38:28] send back-end code and front-end code. They're actually running that API for me over at Heroku.
[38:35] My code started up, it pinged over to Heroku going,
[38:38] "Hey, are you awake over there? Go tell me who's winning the vote,"
[38:41] and then it started playing the audio. I could hear the audio on my side,
[38:44] but I guess it wasn't being shared. That's one example of how I do Python code.
[38:50] I use it for back-end APIs. I also do a lot of system-level programming.
[38:55] Another thing that I do quite a lot is my Twitch chatbot. If anybody ever comes and follows me on Twitch.
[39:02] >> It's so fun. >> I've got all kinds of stuff written in here.
[39:07] This is my static content. Just let me go find static responses, for example.
[39:15] If you ever come over to my Twitch stream, and you type exclamation point A-N-O-N,
[39:21] it'll basically give you back this instruction in chat saying, "Hey, if you ever want to ask a question on my channel,
[39:26] and you want to ask it anonymously, here's what you need to do."
[39:30] Or if you want information about my audio podcast, you just do exclamation point podcast,
[39:35] and it'll give you back the static response. If you want a funny greeting,
[39:40] you do exclamation point hello, and it'll randomly pick one of these and send it back.
[39:45] This is all Python-based code, and it's using someone else's library to actually connect to
[39:51] Twitch and watch the chat for somebody typing in these commands. Then it's also interpreting what people are writing.
[40:00] I wrote my own interpreter inside of this as well. If I go pull up my actual chat bot,
[40:07] let's see, it's my prod bot. I'll show you an example here.
[40:13] What would be a good one to show? A good one is going to be when people want to change
[40:25] my lights here to a different color. You can actually come into my chat bot,
[40:31] and you can redeem channel points to say like, set this to a particular type
[40:35] of pattern or whatever animation on the lights. What it's doing in here,
[40:46] see if I can find it, let's see. Where does it actually get interpreted?
[40:57] Here it is. It's actually calling this blink. If they try to make it blink,
[41:08] otherwise, it's interpreting what they type in. I'm actually breaking their command down into
[41:13] multiple pieces to say, what is it that you're telling me to do?
[41:17] If they're typing in the word random, then I say, okay, I'm just going to go set it to
[41:20] one of these random effects. If you don't give me a list at all,
[41:25] it'll give you a list of the effects that you could set it to. I'm basically breaking this down piece by
[41:30] piece to say, what is it you want me to do here? I've basically built my own interpreter into
[41:35] my chat bot so that when you're typing things in, it can interpret what you're trying to do.
[41:40] This is all written in Python. >> Did Nanoleaf come with
[41:46] anything that described that you could do this or how? >> They have a public API.
[41:54] Then there are people that have written Python libraries for how to interact with that API.
[41:59] I don't have to figure out how do I talk directly to Nanoleaf. I'm going through another Python library that someone else has
[42:07] already done that work and tested that everything's working properly.
[42:10] I just connect to that library with an IP address saying, this is the IP address of my Nanoleaf thing on my home network.
[42:17] Then it knows how to send all the instructions back and forth. >> Very cool. Everyone, I just linked Nanoleaf in the chat
[42:25] because this was one of the biggest things when Ian and I first chatted.
[42:30] I love that I was so captivated by these last time we talked, and now seeing how a practical use case for Python.
[42:41] Since I've been mainly focused on JavaScript, that it's really cool to see the difference
[42:48] and looking at a lot of the different code. Even though at this point,
[42:53] I'm like, I can guess what everything does. >> Yeah.
[42:58] >> But it would definitely be helpful to have the documentation with it or something like that.
[43:05] >> That goes back to what I was saying at the beginning of the stream.
[43:08] Once you learn a couple of high-level languages or even one high-level language,
[43:12] you can look at this and you can probably guess what all of this stuff is doing.
[43:16] I'm doing the same imports here that you might do in JavaScript where you're importing a third-party library,
[43:23] and then I'm running some instructions here. This is how I'm connecting to my Nanoleaf.
[43:27] Then I'm telling it, make sure everything gets powered on, so it'll actually turn on the panel
[43:31] of lights if it's not already on. >> Okay, that's cool.
[43:34] >> This is just me watching old settings and things like that. Then guess what it does.
[43:41] It sets the brightness to a value of 34 of 100, and do that over the course of one second.
[43:48] >> If we're looking at this and we wanted to change, you said to put the lights in a slower speed,
[43:58] would we be changing it right there in one second? No, you haven't done that.
[44:04] >> Yeah, that's happening somewhere else. This is the code that actually says,
[44:09] go find a random red, green, or blue value, and then send
[44:14] that back as a data structure that we call a tuple, which is like an array of red value, green value,
[44:21] blue value, and it's got all the values between 0 and 255. I can set each one of these individual panels
[44:28] to a combination of red, green, blue. What's basically happening, this is
[44:34] the script that runs when I hit a button on my stream deck that says, go blink the lights.
[44:38] The timer here is really a count of how many times it's flashing.
[44:43] But basically saying, we're going to count down those 60 cycles and then say,
[44:48] okay, for every one of those panels, go pick a random color,
[44:52] and then I want to set that panel ID to be that color. Then it's saying, okay, now that we've told
[45:03] all 43 of those panels to get ready to set itself, I want to go synchronize that and boom,
[45:09] they all turn that color. >> That's cool.
[45:13] >> Now, to slow it down, all I need to do is add something in here that says,
[45:17] I want to sleep half a second in between each of these. If I save that and I try and run that now,
[45:24] it's actually a little bit slower on that blink. >> What happens if you did sleep,
[45:32] would it be a 10 to make it that much slower, or would the 10 make it faster?
[45:37] >> It would make it slower, so that's telling it like how many seconds to wait.
[45:42] In that case, I don't think it actually ran that one. >> So far, I know we've had a few people in the chat.
[45:57] Anyone have any questions? Because this is just answering my curiosity.
[46:02] >> No, it's all right. Notice how much slower they're blinking now. That's because I've introduced that timer saying,
[46:07] after setting them all to a random color, sleep half a second,
[46:11] and then go do all that again, and it's doing that 60 times.
[46:15] So what was happening really fast is now taking much, much longer to run.
[46:20] But these are all the different effects that I could set it to as well.
[46:23] So I'm actually querying my Nanoleaf saying, how many panels are there?
[46:29] What was the current effect? It was this Nemo effect,
[46:32] which is just the orange and white in the background. So what happens is it goes through that process of like,
[46:37] go make them all blink here, and then set it back to the old effect,
[46:42] and whatever the original brightness was. So again, what I was talking about at the beginning of the stream is,
[46:48] I want to tone down the brightness if I do make them flash. So it's not like this really bright,
[46:53] vivid thing because I could come in here, and I could set this brightness to be a value of 100.
[46:59] If I go run this again, you're going to notice these lights are like it's going to
[47:04] be wildly bright in the background. Like to a point where it becomes hard to see through
[47:10] the camera what color it actually set. But it's reflecting off a painting and stuff back here,
[47:16] like it's really, really bright in here. So if I wanted to be more sensitive to the folks on my stream,
[47:23] I would say, "Okay, well, let's tone it down. Let's do a 20 where it's going to be a more muted color."
[47:30] So now we see that it actually faded down quite a lot more. So understanding like, "Hey,
[47:35] I want these lights to flash when someone comes in and follows or something, but I don't want it to be this huge overpowering thing."
[47:44] Well, now that I've slowed it down, doing 60 cycles of all those colors takes a long time.
[47:51] So maybe I'll bring that down to only 10 color changes instead. If I can come over here, I can stop the script.
[47:57] I can run it again just to see what effect that's going to have. Five, six, seven, eight, nine,
[48:03] 10, and then it stops and it goes back to what it was when it last ran. Well, when it last ran,
[48:08] it was set to some random color. So that's why it'll be left on that.
[48:12] So now I've basically, I've slowed it down and I've made the colors more muted,
[48:19] and it won't take as long to flash either. >> That is so cool.
[48:25] Bakari said that Python is such an elegant language. >> It is. Like I said,
[48:31] the guy that invented the language wrote it to be easily readable and easily understandable.
[48:37] There's a whole team of people at Python that are basically looking at changes that people want to make to Python,
[48:49] and they make a decision as to whether or not, yes, this is a good change to make to Python around
[48:54] this whole idea of there should be one way to do a thing. There can be multiple ways of looping over an array,
[49:00] but really we want everybody to use this one way to do it. So that way when you look at other people's Python code,
[49:06] you have a pretty good idea of what it's doing because everybody does it the same way.
[49:10] Now, you can go off and you can write it your own way and wild, wild west the thing.
[49:14] But they really do want everybody to write Python the same way, so that anybody else reading the code
[49:20] has a pretty good idea of what's going on and what's happening. >> Does Python have frameworks like JavaScript does?
[49:29] >> Yeah, it certainly does. >> Like on Anaconda?
[49:34] I don't know why I'm saying that word so weird right now. >> Anaconda? Anaconda is,
[49:38] I believe that's one of the data science, data processing, data analytics libraries.
[49:43] So it'll do a lot of the heavy math from what I recall. So the API that I wrote for
[49:49] the jukebox player is written on a framework called Flask, and it's a very lightweight framework,
[49:55] and it's used a lot with APIs. If you want a full-blown web application,
[50:02] you can use a framework called Django, which starts with D-D-J-A-N-G-O.
[50:08] It's a full-blown, it'll build out admin panels and let you talk to databases and pull up.
[50:18] It's really quick to prototype, I've got this database structure,
[50:22] how do I make a form out of that database structure? It'll interpret what you've got defined in your database,
[50:28] and it'll automatically build forms for users to input data and things like that.
[50:32] It's a very powerful framework. It's got a pretty steep learning curve,
[50:35] but once you learn it, it's very, very effective. So yeah, there are frameworks as well.
[50:41] Then on my stream, I do a lot of Q&A around my career prep and interview prep and things like that.
[50:49] So I've got all these other Python scripts and shell scripts of how do I go do all these other things to then process
[50:56] my video files into smaller videos for YouTube and stuff like that, or how do I go extract the audio to actually go then
[51:02] upload MP3 files for the podcast audio stream and stuff like that. >> That's cool.
[51:08] >> Yeah, and so that's all Python and shell script. But what I wanted to show is that we can also use JavaScript for non-browser things.
[51:19] So what I wanted to show you here is how I use JavaScript on one of my websites. So this is my techinterview.guide website that I do my live streaming about.
[51:29] So if you go find IanDouglas736 on Twitter or on Twitch, you're going to find this website.
[51:35] It's basically my career prep advice. But one of the things that I do on here for transparency reasons,
[51:44] I want people to know when I've last updated something on my website. So for example, if I go over to here,
[51:51] if I go to techinterview.guide, I have a changelog on here.
[51:56] What this changelog is, is what have I last changed on the website. So the last time I actually pushed something in this,
[52:04] I was updating my financial transparency because all the money I make as a streamer, I put into a diversity in tech fundraiser and then I match that money.
[52:11] So I wanted to make a changelog that could people go see what I'm actually doing on the actual website for career advice.
[52:20] So in the past, in the changelog, it's been like I was working on the actual book format and things like that,
[52:28] or I put all the cover letter and resume notes in the wrong spot. This was mostly so that people could say,
[52:35] I haven't been to Ian's website in a while, has anything actually changed?
[52:38] Do I need to go through these chapters and look at anything new? So what I wanted to do is find a way of,
[52:44] could I grab all of my Git commit messages and build that into a web page? >> Oh, that's cool.
[52:50] >> So this is in JavaScript, and that was partly just to stretch myself a little bit.
[52:55] So I have this markdown file called changelog, and this is where it's going through and it's actually
[53:01] building and it's fetching all of my Git commit messages and building this as markdown,
[53:07] and then that compiles into HTML using another process. But what I have in here is I've got a script called changelog.js.
[53:17] So when I go run this on the command line, it's basically building an intermediate version of it,
[53:26] where I said I wanted some transparency about when I was actually changing something tangible about my website,
[53:33] and then it's going through and saying, "Okay, well, go find all of my commits as of basically November 2019.
[53:41] Stop looking at any commits older than that." So if I really wanted to say,
[53:45] only grab the last 50 commits or something like that, then I could set a date or something,
[53:51] or I haven't really tangibly changed anything since this date. But otherwise, this is going through and it's saying,
[53:57] "Go get all of my Git commit messages." So let's walk through what this is doing.
[54:01] So the child process is basically saying, I want to be able to go out to the shell and go run
[54:07] some shell command and then give me back that result. In order to do that, I also need access to the file system,
[54:14] and so I'm requiring in some JavaScript libraries for this. Then I'm just going to go call git log.
[54:21] I can literally come in here and I can just call that command myself on the terminal and
[54:27] see what my JavaScript is going to get back. So when I call git log with that,
[54:32] let me pull this up here, it'll actually show me here my commit messages,
[54:37] and then showing me the date with this delimiter, and I'm basically forcing it in there so that I can
[54:41] parse things a little bit easier with a known delimiter value, that I can go in and extract these strings basically.
[54:49] But here's my git log with all of these delimiters in here. So I wanted to basically take this whole git message
[54:58] here and say, "Okay, I want that to show up on this changelog."
[55:03] I say, "Okay, we'll go run that as a child process. Go do all of this,
[55:09] give it back as this UTF-8 character type." So there's different ways that we can interpret
[55:15] characters and things like that as strings. Then saying, "Okay, now in all of that output,
[55:21] I want to split it on that delimiter, and then I want to map over all those results,
[55:25] and I want to figure out the message and the actual date of that message."
[55:29] I build that into a data structure, and then I iterate back over that data structure to say,
[55:34] "Okay, now I want to go read this file, and how do I then go over all of those commits?"
[55:42] Then say, "Okay, well, if it started with this, so this is what I was doing is I was
[55:47] actually saying as soon as I see a commit with this date, I throw an exception that says, "Stop working."
[55:55] This is as far back as I want to go in my Git log. Otherwise, if I have
[56:04] a commit message that starts with the string, like rebuilding the site,
[56:07] it won't put that in there. Otherwise, it's going to go build all this stuff as markdown,
[56:13] and then if there was anything to change, then it goes and it creates
[56:18] that changelog file that we looked at a moment ago. It pulls this one up as a early processing version of it,
[56:28] and then ultimately writes it into this changelog file here,
[56:32] which is all written as markdown. Then I run another process that says,
[56:37] "Hey, go through all these folders, find all these markdown files,
[56:40] and convert them all into HTML." Then I upload that to the website.
[56:44] Whenever I do a Git commit, I then run this command here.
[56:48] I can come in here at any time and I can say, node changelog.js, and it just went through,
[56:55] and you notice it changed something in here. >> That is so cool.
[57:00] I like what Bakari said, "Wow, what a guy." Yeah, you've built this out pretty cool.
[57:05] I will say like imposter syndrome, I'm like, "Dude, I can never do that."
[57:10] Ian did share that it's taken him a while to get this done. >> Yeah, and part of doing
[57:19] this changelog in JavaScript was to stretch myself of like, I want to see if JavaScript can do system-level programming.
[57:25] I actually wrote this script long, long time ago and I haven't had to change it, thankfully.
[57:31] But JavaScript can be used for non-browser code and Python
[57:36] can be used for a lot of different kinds of things as well. It's mostly going to be used as
[57:40] back-end code and system code for Python. But now in JavaScript,
[57:44] we can also do system-level code. You can do back-end code if you
[57:48] use a framework like Node and Express. You can also build out full API back-ends as well and
[57:54] talk to your database and process data and all that stuff as well.
[57:58] There's lots of frameworks out there that you can go do this stuff with.
[58:02] The nice thing about these high-level languages is you can use them for a lot of different purposes.
[58:07] You shouldn't have to feel like, "Oh, if I'm learning JavaScript,
[58:10] I can only do stuff in the browser." It's like, "No, you can certainly
[58:13] do stuff in the terminal here as well." There's lots of ways that you can use
[58:17] this code and interpret this code to go run and execute. Now, is JavaScript the best tool for this?
[58:23] No, not necessarily. I could have probably done most of this just in
[58:26] regular shell script coding as well. But like I said, I wanted to stretch
[58:31] myself into how can I do this with JavaScript. It may not be the best tool for the job,
[58:36] but for me, it was a learning experience. I've been a big fan of learning in public and
[58:42] seeing how I want to do things and how things actually run and execute,
[58:49] and it expands my appreciation for what goes into the JavaScript language by building a script like this,
[58:56] to where I can say, "Oh, this isn't just about go interpret these values on a form and do a fetch
[59:02] and process stuff in a browser." JavaScript can do a lot more than that.
[59:08] >> I love that. I was looking really quick just to see what the documentation would be.
[59:16] It doesn't let you see very much before logging in for Nanoleaf. But I'm like, I almost want to get Nanoleafs and be able to see
[59:23] if I can program one in JavaScript and then program one in Python just to compare the two in the process.
[59:32] >> I'm sure somebody has written an NPM package for that. >> That's what I was just about to look up because I was like,
[59:40] well, it's not really letting me see it, so I'll look it up later.
[59:44] >> Yeah, you want to search for something like Nanoleaf client or something like that.
[59:48] >> Okay. >> Now, I'm not necessarily endorsing that one,
[59:51] but that's effectively what you want to use. You want some client-level software to talk to your Nanoleaf.
[59:57] But Nanoleaf EJS looks like API client and command line tool. Now, that's specific to one particular Nanoleaf.
[60:06] Let's go look at this Nanoleaf client one real quick. >> Nanoleaf isn't sponsoring this either,
[60:11] but I mean, if you-all do one point, please reach out.
[60:15] I will have more lights everywhere. I will completely redo my background for Nanoleaf.
[60:22] >> This one operates very similar to my Python script where it can try to
[60:27] discover what is the IP address of your Nanoleaf. But it should probably have a way of like,
[60:34] because this can actually take a little while. If you've got a lot of things on your network,
[60:38] it's going and pinging all of them, going, "Do you know how to talk Nanoleaf?
[60:42] Do you know how to talk Nanoleaf? Oh, you do know how to? Okay.
[60:45] This is the IP address I need to use." But if you've got multiple Nanoleafs,
[60:48] which one does this actually talk to? Like if you've got several of them,
[60:52] then you want to be able to talk to each one. So you would have to know the IP address.
[60:55] But otherwise, it's the same thing. You have an auth token,
[60:58] and then you can go get information about it. You can get the orientation,
[61:04] which is literally like how they're sitting on the wall, and things like that.
[61:09] You can get the saturation value, turning it on and off, setting your brightness,
[61:13] setting the duration of like fading that brightness in and out that we saw.
[61:18] Getting and setting the hue, which is basically a single color value,
[61:22] or setting, you know, the effect, like the Nemo effect that was just the orange and white
[61:28] in the background. Or you can set like an actual like RGB value or HSL.
[61:34] I forget what HSL stands for. But then they give you full examples of,
[61:38] yep, here's how to talk to your Nanoleaf on an IP address, given your auth token.
[61:44] And then based on that, you know, go get your information
[61:48] and then go run those other commands. So I mean, if I were going to do this again in JavaScript,
[61:53] I'd probably use this library. This one looks pretty well documented
[61:57] and, you know, pretty straightforward to use. - Thank you for joining Bakari, good luck.
[62:02] He just said that he has an interview. - Oh, awesome, good luck.
[62:04] Yeah, I hope it goes great. Let us know how it goes.
[62:07] - And this is so cool. You've taught me so much in such a short period of time
[62:11] of just like everything that can be done. - Yeah.
[62:16] - Like the possibilities. I feel like that's a hard thing for newbies
[62:18] of seeing the possibilities, where I liked that you,
[62:24] I don't know where I saw it, if it was on your Twitter
[62:27] or you actually talked about it yesterday, of suggesting that people can reach out to you for ideas.
[62:35] - And I'm like, for like something to program, for like-
[62:38] - Oh, for project ideas and stuff, yeah. - Yeah.
[62:40] - So I have a- - That's so smart.
[62:42] - Yeah, I have a Discord community and actually somebody posted in there last night going,
[62:45] I've got to build my 100 hours project for 100 devs and I don't have a project idea.
[62:50] And I'm like, here's what I would do as a project. And basically what I told them,
[62:56] I can pull it up here real quick. What I suggested to them is here,
[63:03] like the general concepts of what you should build out that will make you stand out as a candidate
[63:08] is you want something with authentication, maybe form data processing.
[63:13] And so I came up with an idea of like, just make a simple, you can log in,
[63:18] you can build a profile for yourself and you can go visit other people's profiles.
[63:22] And if you're not logged in, then what you see on the profile is very limited in scope.
[63:26] And so this teaches you all about authentication, like who are you so that you can build your own profile.
[63:31] And then it talks about authorization, which means if I go look at your profile,
[63:35] I shouldn't see the edit profile button, only you should see that when you're logged in.
[63:40] And if neither of us, like if no one's logged in and they go to your profile,
[63:44] maybe they just see like your name and your profile picture and they don't see all of the other content
[63:48] that I would see if I'm logged in, because if I'm logged in,
[63:51] I'm more trusted with that data or something like that. And then maybe for your profile,
[63:55] have a way to like upload a picture. And then where do you store that picture?
[63:59] Like, do you put it in an Amazon S3 bucket or something like that?
[64:03] These teach you some very fundamental things about web development and how the internet works.
[64:11] And so having a project that sort of encapsulates all of those things
[64:17] makes for a really good project, because then you can expand that out
[64:20] to whatever you want it to be. You could build like your own little newsfeed
[64:23] and make your own little social network kind of website or whatever, but by having the login
[64:29] and having the profile page and having that authorization of what are you allowed to do on that page,
[64:35] you could build out a search where you say, okay, we'll go find users who have Ian in their name
[64:41] and only show me them. Well, if I've got thousands and thousands of Ians
[64:46] on my website, I don't wanna list all of that on one page. So what if we did pagination
[64:51] and we only show you like 10 or 20 at a time? Well, that's also teaching you about database operations
[64:56] and how do we only grab like a little bit at a time. And so the concepts of building a project like that,
[65:04] which you can then expand out into whatever you want. You could turn that into a shopping cart website.
[65:09] You could turn it into like a book lending, between friends kind of site.
[65:15] You could build that into like whatever, like let's plan a road trip
[65:18] and go see what the weather's gonna be like when we get there.
[65:20] Like you can do all those things of like, here's Ian's profile
[65:23] and here are all the road trips that he planned. Those kinds of things.
[65:27] Like you can expand that idea out into whatever else you want.
[65:31] But these are the kind of the core fundamentals, I think that will really stand out
[65:36] as opposed to, you know, I made a to-do list application. It's like, okay, that's good
[65:41] because it still shows that you can write a user interface and you can store things in a database.
[65:45] But if I need somebody to be logged in on, you know, at my company,
[65:51] like our customers have to log in to do something. If you don't know how to do that,
[65:54] I've got to teach you all that authentication and authorization stuff.
[65:58] If you've already got a project where you've walked through that
[66:00] and you have that understanding, that's one less thing I have to train you on.
[66:04] And that makes you look like a better candidate for that job.
[66:07] So by building a project where you've got some of those core fundamentals in place,
[66:12] it makes you like sort of a better candidate overall as far as like me wanting to hire you.
[66:20] 'Cause I've got fewer things that I have to sort of train you on
[66:22] once you start on the job. - I totally get that.
[66:26] And there's just so much that goes into it. And I think that's the exciting yet overwhelming part
[66:34] of the tech world in general and coding and all of the possibilities.
[66:40] But any last things you want to go over before we end today? 'Cause we've gone through a lot of like
[66:47] when Python and JavaScript both came out, how they originated,
[66:52] just going through a lot of the differences as well as seeing some use cases on both.
[66:59] - I think the biggest thing, the biggest piece of advice that I give to folks
[67:02] who are just learning technology and learning about programming
[67:06] is study one thing and know it really well. So if you're learning JavaScript,
[67:12] learn how to do all these things in JavaScript. Learn about how to run things in a terminal,
[67:17] how to like connect to internet of things, lights. I mean, if you can get like a $10 light bulb on Amazon
[67:24] and learn how to control that through internet of things libraries like Nanoleaf,
[67:28] you don't have to go buy a Nanoleaf in order to do that. There's much cheaper alternatives out there
[67:33] where you don't need to buy a whole panel of these lights 'cause you can't really just buy one Nanoleaf.
[67:37] You have to buy like a whole set of them and they're maybe hundreds of dollars.
[67:41] But you can go buy like a single light from a company called Govee, G-O-V-E-E.
[67:47] And they're very inexpensive and you can get literally just a light bulb
[67:51] and you can interact with that API that way. And use Postman for that.
[67:54] We've got all kinds of fun stuff in Postman that you can interact with these libraries.
[68:00] But when you're learning a new concept, it's easier on your brain to learn one language
[68:07] and learn that really, really well. And then figure out later on in your career,
[68:13] like, okay, I've learned JavaScript, excuse me. I can do all this stuff in JavaScript.
[68:20] I wanna go a little bit deeper. What else should I learn?
[68:22] Excuse me. And so at that point you can make a decision on,
[68:28] okay, now I think I wanna go dabble in some Python or Ruby or Go or Rust or whatever.
[68:34] But I think what holds a lot of people back in tech is they see these job posts and they're like,
[68:40] oh, I can't even apply for that job because I don't know all 15 or 25 of the things
[68:44] that they're asking for. So I need to go learn all 25 of those things.
[68:49] Well, by the time you go learn all those things, that job post isn't even around anymore.
[68:52] And now when you go look at somebody else's job post, it's a completely different list of things.
[68:57] And you're like, well, now I gotta go learn all that stuff. And so you never really feel ready
[69:00] because you feel like you've always gotta learn something before you can even go apply for that job.
[69:05] Where if you just go really deep on a particular technology stack,
[69:09] then you can say, okay, I know JavaScript really well. I'm just gonna go do JavaScript.
[69:13] I'm gonna go do that interview in JavaScript. And yeah, maybe I need to go learn Python
[69:19] to actually get that job, but I understand the programming concepts
[69:22] and I understand how to do all these different things in JavaScript.
[69:26] I just need to go figure out how to say that in Python. And so again, if you learn Italian
[69:33] really, really, really, really well, you're gonna be able to understand some bits of Spanish
[69:39] and you'll be able to pick up the Spanish language really quickly.
[69:42] And then once you learn Italian and Spanish, picking up French, you'll pick up French in like a week
[69:48] because a lot of that grammar is the same and a lot of the words are the same.
[69:52] You just have to learn how to... Maybe there might be a few differences here and there.
[69:58] Same thing with a lot of Germanic languages and so on. As you learn German, you'll learn Czech
[70:05] and some of these other languages. They're not identical,
[70:09] but the structure of how those things get put together are gonna be very similar
[70:12] and it'll be the same way with programming. But I would say early in your career
[70:17] when you're just learning this stuff, focus on fewer things.
[70:22] And so I talk about breadth of knowledge and depth of knowledge.
[70:25] As a hiring manager, I would rather hire somebody with a depth of knowledge
[70:28] than a really broad breadth of knowledge where you only know things a very shallow amount.
[70:35] Like if the only thing that you can build in JavaScript is a to-do list application,
[70:40] then if I say, go build me an app in Python, you're like, I'll go build a to-do app
[70:44] 'cause I know how to do that. And then if I say, go do it in Ruby,
[70:47] you're gonna go build another to-do app because that's all you know how to do.
[70:51] But if you go really deep and you build a bunch of projects in JavaScript
[70:56] that do all different kinds of things, then you've got more experience
[71:00] that you can then apply to other languages, other technologies, other frameworks.
[71:04] So go really deep on fewer things early in your career. As you get that job,
[71:09] then you've got time to explore and learn and go do all that stuff.
[71:12] But to go get a job, focus on like one language, one framework,
[71:16] and just be your own expert. You don't have to be the expert
[71:20] or an industry level expert, but be really good at what you know.
[71:26] Like to where you're confident, like I've done several projects in this language
[71:30] or in this framework or using this technology. I know it really, really well.
[71:33] Now I'm gonna go interview. And I'm just gonna tell them at that interview,
[71:36] I'm gonna use these technologies. I'm gonna go learn whatever else you need me to learn
[71:40] on the job, but this is what I know really well. And just impress their socks off
[71:45] with what you know really well, instead of trying to,
[71:47] oh, they want me to know Python for that interview. Now I gotta go learn Python.
[71:52] It's like, well, you're not gonna become a Python expert enough to pass their interview in a short amount of time.
[71:57] So just go interview in JavaScript and say, I know JavaScript, it'll translate fine into Python.
[72:03] And go from there. So fewer things,
[72:07] but go deeper on those fewer things to start. - I dig it, I dig it.
[72:11] And I feel like our listeners will definitely be able to learn from that as well.
[72:17] And in a way that I've heard this as well is being, there's a difference between being an inch deep
[72:25] and a mile wide, then a mile deep and an inch wide. So that is something that has really stuck with me
[72:32] over time. So I really appreciate your time today, Ian.
[72:36] - Yeah, happy to help out. - Yay, so much to learn.
[72:40] - Yeah, there's a lot to learn, but like I said, like focus on fewer things.
[72:45] There's also something that we call a T-shape engineer. So if you think about the T-shape,
[72:51] it's very much like what you just said. You can go wide on things to a shallow amount,
[72:56] but on one thing, you're gonna go really deep and know that one thing really well
[73:00] where everything else is shallow. And so be that T-shape engineer early in your career.
[73:05] Like you can go learn like, okay, there's a database called Mongo
[73:09] and there's a database called Postgres and there's a database called MySQL
[73:12] and there's a database called Redis, but you don't have to know them all really well,
[73:15] but you know what, I'm gonna do everything in Mongo. So I'm gonna learn Mongo really deep.
[73:20] And now there's all these other programming languages and I can kind of read through them
[73:24] and understand prints and console logs and puts and whatever for all these different languages,
[73:30] but I'm gonna go really deep on JavaScript. - Okay, I did that.
[73:33] - And so be that T-shape engineer and just go really deep on fewer things.
[73:39] - I did that. And thank you again for the advice
[73:43] and all the learning and teaching. And I hope we get to have you back again someday
[73:49] to learn more about Postman too. - Yeah, we'll dig into what APIs are
[73:54] and how they're used and how they hold the world together. - Yes.
[73:57] Yes, I'm excited about APIs. All right.
[74:00] Well, happy Friday, everyone. We'll see you next time.

