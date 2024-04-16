---
showLink: "https://www.youtube.com/watch?v=6gZZyBCG_8E"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-apis-with-ian-douglas-from-postman"
title: "Teach Jenn APIs with Ian Douglas from Postman"
publishDate: "2023-04-19"
coverImage: "https://i.ytimg.com/vi/6gZZyBCG_8E/maxresdefault.jpg"
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

[00:00] of Teach Gen Tech. And today Ian is teaching me about APIs
[00:06] because he's also from Postman. And that's about the intro you got from me
[00:12] as Gen, your host. Ian, who are you and what are we learning about today?
[00:17] - Hello everybody, I'm Ian. I'm a Senior Developer Advocate at Postman.
[00:21] Postman's an application that folks use to test APIs, like use APIs and build APIs as well.
[00:28] It's been around for, gosh, like a decade. We got like 20 million plus people using the software.
[00:33] And yeah, I get to do fun stuff like build workshops and teach people how to use Postman effectively,
[00:40] but also educate people on like, what the heck is an API in the first place
[00:44] and what kinds of different APIs are there out there and things like that,
[00:49] just to help on the education side of it, just to help make everybody a little bit better
[00:53] at what they do. - Yay, and I love that because this is a big reason, y'all,
[00:58] that we are doing this stream today. Because for those who don't know,
[01:02] about two years ago, I was working for an API design spec company.
[01:10] Wait, API, yeah, spec design company. That is a good way of saying it.
[01:16] It is, I worked for a company named Stoplight and they make it, it's pretty easy to build an API with them
[01:23] and I could build APIs with them, which is great.
[01:25] And it built documentation, which is awesome. And I have on the show, we've built APIs, great.
[01:32] And I am also one of the co-organizers of the Denver API meetup.
[01:38] It's actually where Ian and I first met. And yeah, if you ask me the parts of an API
[01:43] and what an API actually is and what it stands for and anything about the actual API itself,
[01:48] is what I got. So I'm very excited that we are going to the basics,
[01:56] back to the basics, relearning it, and really working towards growing our vocabulary
[02:03] and remembering what each of these mean. At least that's my own goal.
[02:07] So my hope is other people will be able to understand that as well.
[02:12] And yeah. - Awesome.
[02:15] - I'm excited about our intro. I always get nervous about the intros.
[02:18] I don't know why. I'm always like, I'm gonna butcher them every single time.
[02:22] - It's all good. It's all good.
[02:24] It's your stream. You can do what you want.
[02:26] You be you. - That is what I work on doing.
[02:30] That is what I work on doing. But for some reason, it's like every time I'm like,
[02:34] that excitement. And then I'm like, oh yeah, we're streaming.
[02:37] It's no big deal. But it happens every time after,
[02:41] I think I have like 80 screens now. So for anybody, it still happens.
[02:46] It still happens. All right.
[02:50] So Ian, what is an API? - What the heck is an API?
[02:54] So the letters API, when we talk about like, what's the, if we look at this up in like a tech dictionary,
[03:01] what does API actually stand for? Stands for application programming interface,
[03:07] which is a whole bunch of like syllables. What does that even mean?
[03:13] Like what's an application programming interface? When you think of interfaces,
[03:18] you could think of like plugs. When you think of programming,
[03:22] a lot of people are like, oh no, this has to do with code. Like they suddenly get a little bit scared.
[03:26] I think to explain as simply as possible, what is an API?
[03:36] I wanna use a word, abstraction. Have you ever heard abstraction?
[03:40] Like when it comes to programming or anything like that, or like how to abstract an idea, abstract painting.
[03:45] - I was like painting. Painting comes to mind.
[03:48] - So the idea of like an abstract painting is like, it kind of looks like a thing.
[03:53] But when we talk about abstraction, the example that I like to give is
[03:58] when my kids were little, we'd go up to their room and it'd be like,
[04:02] okay, well, let's take these clothes out of the laundry basket.
[04:04] Let's fold them, let's put them away. Let's pick up your toys, put them in a bin,
[04:08] put the bin in the cubby on the wall. Let's pick these books up off the floor,
[04:11] put them back on the bookshelf. And we call that cleaning your room.
[04:15] And so now when I tell you, go clean your room, I expect you to fold your laundry, put it away,
[04:21] put the toys in the bin, put the bin in the cubby, pick up the books off the floor, put them on the bookshelf.
[04:25] So I'm abstracting that instruction to my kids saying, go clean your room.
[04:31] And hopefully they remember, not always, but if I had like a list on the wall of like,
[04:38] to clean your room, do the following things. That's basically what we call abstraction.
[04:44] When you wanna use like the blender in your kitchen, there's a button on there to say,
[04:51] blend, change the speed, blah, blah, blah. That's also kind of an interface
[04:56] to how the blender actually works. How fast is it running?
[05:00] Is it pulsing? Is it just blending at super high speed?
[05:05] What speed is it blending at? It's an abstraction.
[05:08] It's not you in there like turning the motor. You're pushing a button to have something else
[05:13] do that thing for you. And so there's a lot of this kind of idea of abstraction
[05:19] all around us when it comes to something, yeah. - Would you say abstraction is like what to do,
[05:28] but not necessarily how to do it? - It could be, it could be, yep.
[05:36] Normally when we talk about APIs though, we're basically saying, I want you to go do this thing.
[05:42] How you actually do it, that's up to you. We'll get into a little bit of that.
[05:47] - Okay, cool. - So when we talk about programming and APIs,
[05:53] there are two kinds of different APIs. So the first kind of API when we get into coding
[05:58] is what is my programming languages API? So if you work in Python or JavaScript or Ruby, C#,
[06:07] even Java, C++ and C, like all the lower level languages, we're still kind of abstracting
[06:15] what we want that programming language to tell the computer to do.
[06:18] So no matter what programming language you're writing your code in,
[06:24] you're basically giving the computer an instruction like go print the words, hello world, in my terminal.
[06:30] That's abstracting all the way down to machine level of the binary ones and zeros that actually tell the CPU
[06:41] and your computer, like actually go do these things to send the instruction to the video card
[06:45] to like print this thing out on the screen that says hello world.
[06:48] And so we're not down at the hardware level, like turning the electricity on and off these wires
[06:56] for the ones and the zeros, the CPU does that. The CPU gets machine level code,
[07:02] which comes from the programming language level code. And then these programming languages
[07:06] are all kind of written in one another too. So for example, C++ is written in C and assembly.
[07:13] Assembly goes down into the machine code of like how the CPU actually works, right?
[07:19] But then C and C++ are used to write languages like Python and Ruby and JavaScript.
[07:25] And so we call JavaScript and Python, for example, we call those high level languages
[07:32] because we're not necessarily getting into all the nitty gritty of like,
[07:36] go allocate this chunk of memory to make an array of strings.
[07:40] We just say, we want an array of strings and Python kind of tells the interpreter like,
[07:46] okay, these are the actual instructions to actually go do. And so when we talk about APIs,
[07:52] we could be talking about what is our programming language API,
[07:57] which is still just an abstraction of, hey, I need an array of strings
[08:01] that the programming language then knows, oh, I need to go allocate memory in a particular way
[08:06] and do a particular kind of thing in order to actually make that happen for you.
[08:10] So when we get into, so that's the primary thing
[08:19] that we talk about when we're coding, when we talk about APIs,
[08:22] but there's another kind of API and that's where kind of Postman comes in
[08:26] and that's where I've spent a lot of my career is when we talk about how do we get information
[08:33] or send information somewhere else. So for example, there are a lot of APIs out there
[08:40] to do things like, oh, go get the weather. I've got an API that I can hit a button
[08:45] and it makes these lights behind me blink. That's all done over APIs.
[08:49] And it's still just an abstraction of go make these lights blink
[08:54] or go get the weather in Denver or go find a dad joke or whatever.
[09:00] There's lots of these APIs out there. - Really quick, everyone,
[09:04] we just need to pause for a second and just look at Ian's lights
[09:07] because that is the level I want to get to someday. That is the goal of someday
[09:14] being able to get really cool lights like Ian's. Literally, since Ian's my first,
[09:18] he's been on the show before quite some time ago. I think we ended up talking about Python versus JavaScript
[09:26] because it was when I first started that. And so ever since then, I'm like,
[09:32] you know, one day I want to get my light game up and you mentioned it.
[09:36] So it was the perfect time to say so. All Ian's fault.
[09:39] - I'm glad I can be a bad influence when it comes to visual purchases.
[09:47] So even the idea of sending and receiving information to other computers, other servers somewhere,
[09:58] that's still an abstraction of those instructions where I say, "Hey, I want to get the weather in Denver."
[10:04] There's still a list of software instructions somewhere, whether that's running on my computer
[10:09] or some other computer out on the internet somewhere where I'm saying like,
[10:13] "Hey, go get me the weather for Denver." Something out there is following a list of instructions
[10:17] to go look up that information. Some other computer is actually reading sensor data
[10:22] and storing that somehow. All I'm doing is I'm doing an abstraction
[10:27] of go get the weather or go make these lights blink or whatever.
[10:32] Like when I hit a button on my little thing that says go blink my lights,
[10:36] that's a whole list of instructions. And some of those instructions are,
[10:39] well, how many lights are there on the wall? Let me make a list of all of those.
[10:43] Let me go pick a random color for each of those, set the lights,
[10:48] send that packet of light instructions to all the panels. And then repeat all of that over and over several times
[10:57] so it looks like this random flashing kind of pattern. It's all just an abstraction where I'm not in there,
[11:02] running that what, 50 times or whatever for each of the lights that I have on the wall
[11:09] and doing that 50 times or however many times I wanna make these lights blink.
[11:13] And so the idea of abstraction is you're coming up with a high-level instruction
[11:19] to do a bunch of low-level instructions. - Ooh, I like that.
[11:23] - And then those instructions are also being interpreted as software kind of like we talked about.
[11:30] So if I'm running a little Raspberry Pi with a temperature sensor and I say,
[11:37] what's the temperature in my workshop right now? That's still running a list of low-level instructions
[11:43] of go read the hardware, go interpret that information into a temperature,
[11:47] send that temperature back to however Ian's calling it. And then Ian gets just a number of it's 68.2 degrees.
[11:55] - I didn't know you could do that. And that is really cool because when I get back
[12:02] from this work trip next week, I should be coming back with Raspberry Pi
[12:07] to build it to do something and I've never done it. So I'm very excited and I'm gonna do it live.
[12:14] That's pretty obvious, but I'm excited. So that's a cool, another idea that you can do
[12:20] with a Raspberry Pi, yay. - So strictly speaking, the letters of API
[12:25] stand for application programming interface. I like to think of it as like the A is kind of
[12:29] the abstraction of programming and interaction. So, but I wanna be careful, like the proper terminology
[12:39] for API is application programming interface. But I sometimes think of it as like the A
[12:44] is abstracting things, P we're still programming things, but the word interface sometimes sounds a little weird.
[12:52] And so we can think about like, how are we interacting with something,
[12:56] but we're abstracting it in a way that's sort of high level that we can just say, hey, go clean your room.
[13:03] And hopefully my kid is gonna follow all the instructions. Where the computers are generally a lot better
[13:10] at following the list of instructions that we give it. And so we're gonna spend most of today
[13:16] talking about like, how do we access and send information to an API
[13:22] where that's not necessarily like code that I'm running on my computer.
[13:28] We'll talk about like, how do we send stuff over the internet and so on.
[13:32] One of the things- - What did you say the I was? - Like an interaction.
[13:38] - Interaction, okay. - Yeah. - I like that.
[13:40] That's why I put it down here, you know, it's not gonna- - But the proper-
[13:47] - It's hidden. - But the proper terminology is application programming interface.
[13:51] I wanna make sure everybody's walking away with good terminology here.
[13:54] It's application programming interface. But I like to think, me personally,
[13:58] I like to think of the A as abstraction just 'cause that helps me realize like,
[14:02] oh, I'm taking a really high level instruction and somebody else is handling
[14:06] the low level instructions for that. So we're gonna spend most of our session today
[14:11] talking about, you know, how do we communicate with these APIs?
[14:15] What does that actually mean? 'Cause it's a little bit different from like writing Python
[14:18] and then writing the Python interpreter. When we talk about APIs, there are different ways
[14:24] that we can send that information over the internet to actually go communicate with these servers
[14:29] to do different kinds of things. So we'll get in and kind of break that down bit by bit.
[14:35] - Really quick y'all, something that is also really good to know is that Ian used to be a instructor
[14:43] at Turing, that's what it was called, right? I always forget.
[14:50] Are you still there at all doing anything or? - I'm a mentor for the students.
[14:57] I still help a lot with career development and like interview preparation and things like that.
[15:03] Resume reviews, that sort of thing. - And that's something that Ian is amazing at
[15:07] and really helped me realize a huge missing part on mine, which y'all, for those who may not realize,
[15:17] I was job hunting for a very, very, very, very long time, over a year before I got my job at Ivan.
[15:23] And this was, Ian caught the mistake, that really helped. So I'm posting Ian's Twitter.
[15:32] Yeah, like you can, there's so much to go to, go follow him on Twitch, he can do a shout out.
[15:39] - I use the same, yeah, I try to use the same username, IanDouglas736 on Twitch, Kick, LinkedIn, Twitter,
[15:48] like all those platforms, Instagram, all that kind of stuff. Yep, so Sundays I live stream about like career preparation,
[15:57] interview preparation. Tuesdays, like Tuesday night, I tend to do like live coding
[16:02] of some kind, I'm gonna be building out chatbots and so on, which use a lot of APIs.
[16:07] And then Thursdays, I tend to get a little more crafty. Lately, I've been getting into like airbrushing
[16:13] and stuff like that. So I've got like some cool 3D printed dragons
[16:16] that I'm airbrushing. So I'll be doing that on Thursday nights.
[16:19] So I do kind of a variety of things, but it tends to stay around like a technical nature.
[16:26] - Yeah, okay, let's see if you remember. Do you remember the mistake that my resume had?
[16:31] - Um, I'm trying to remember if it was how the PDF file was generated that it wasn't like pulling
[16:37] the text in properly. - That was it.
[16:41] - Was it? Yeah. - So basically y'all, what happened is I generated
[16:45] my resume with Canva. It looked gorgeous.
[16:49] I exported it into a PDF. It still looked gorgeous, it was fine.
[16:54] But when Ian got it, he just went to like copy and paste something and there was spacing
[17:01] between all of them. And like, and it wasn't necessarily like a space
[17:07] between every single letter. It was like half of the word.
[17:10] So it would be like, if we're talking about APIs, it would be app and then a space and then the L
[17:18] and then a space and then I-cation. And it wasn't something that was obvious
[17:24] just looking at it. It was something that he found copy and pasting it
[17:28] and something that I guess happens to a lot of people. - I catch it from a lot of folks that ask
[17:34] for resume reviews. It's like, well, that's one of the first things
[17:36] that I look at. It's like, what made that PDF file?
[17:39] And then we can kind of debug from there, so. - Yes, Lex, yes.
[17:45] I would say at least from this reference, I now had, I had to, and even when I was trying
[17:50] to copy and paste everything from Canva, it wouldn't go into my Google Sheet very well.
[17:55] So I actually rewrote the most boring looking resume ever. But I was like, you know what?
[18:03] If it's readable, it's there. - Well, the thing with resumes is it's gotta get past
[18:08] three things. The first one is the automated applicant tracking system,
[18:12] which is actually what's scraping all the words and putting that in the database so that when the HR people
[18:16] say we're looking for a JavaScript programmer that your resume is gonna pop up.
[18:20] The second thing that it has to pass is the HR person has to look at it and go, okay, I can actually read this.
[18:28] It's organized well. And then it goes to a hiring manager or a technical manager,
[18:31] in my case, for doing programming and so on of, you know, do they find what they're looking for quickly
[18:39] and easily as well. So generally the resume is about like,
[18:42] what's the value I bring to the company? But you've got to present it in a way that's gonna get past
[18:47] the applicant tracking system, as well as HR, as well as the hiring manager in order to get
[18:50] that phone call. But that's a whole other screen we can do
[18:54] on career prep. But that's the kind of stuff that I do on Sundays
[18:57] is help people understand like how to build resumes, what goes into a resume,
[19:01] how to talk about the value you bring and so on. - And 3D printing on Thursdays.
[19:07] - On Thursdays, yep. And then Tuesdays I do coding, yep.
[19:10] So later tonight I'll be doing some live coding and working on some chatbot stuff.
[19:14] - Yay, Ian does lots of cool stuff. - Yep, I try to dabble in all the things.
[19:21] I mean, for me, it's like, I wanna go learn something and then teach it to somebody else.
[19:24] I get more satisfaction out of the fact that I'm teaching you about APIs and now you're gonna go do
[19:28] something cool with APIs than the fact that I know how to do something with an API.
[19:32] I get a kick out of like teaching that to other people then watching them go succeed.
[19:36] That's what drives me. That's my intrinsic motivation.
[19:39] So, if I can fumble around with airbrushing and somebody picks up a tip that they never thought
[19:45] about before and then they go do something cool with airbrushing, it's like, sweet.
[19:48] Now I had like a tiny little piece to play in that. - Yes, yes.
[19:52] - Like the cool lights you've got behind you now. It's like, I had a little part to play in like convincing--
[19:56] - You did, you did. Like, Ian complimented my lights when I turned them on
[20:01] 'cause, you know, of course I was running late and I was like, yay, I almost forgot to tell you
[20:06] that you influenced my light purchase. So, that is exciting.
[20:10] Yes, okay. - So, let's get into APIs.
[20:14] So, this is a lot of what Postman does. This is a lot of like the workshops that I do,
[20:18] a lot of the conference talks and going to meetups like the API meetup in Denver and just helping educate
[20:25] people on like, what are the different kinds of APIs and then how do we communicate with those?
[20:30] So, what I'd like to do is I wanna talk about kind of the most popular type of API,
[20:36] but there are different kinds of APIs about, and these are really how do we communicate
[20:41] with these other servers on the internet? At Postman, we talk a lot about how APIs
[20:47] kind of run the world. When you think about what's happening on your phone,
[20:50] like my mobile phone, for example, like every app on here is connecting over the internet
[20:55] to go get information. So, whether I'm like looking at the weather,
[20:58] pulling up my calendar, checking my email, those are all making like API calls to some server somewhere
[21:05] to like send and retrieve data. And so, there's this, the most popular type of API
[21:12] that we talk about is called REST. And REST was actually developed back in like the 2000 era.
[21:21] And to back up a little bit, a lot of how we communicate over the internet,
[21:28] if you ever look at the browser address bar, you'll see like HTTP or HTTPS.
[21:34] More recently, you're gonna see HTTPS everywhere where the S just means it's secured.
[21:40] But HTTP stands for Hypertext Transport Protocol. And we kind of have to talk about this a tiny bit
[21:48] before we get into REST. So, Hypertext Transfer Protocol.
[21:53] And this is basically, how do we send these blocks of text information for like a webpage?
[22:00] And that's HTTP. With HTTP, somebody came up with the idea of,
[22:05] okay, well, how are we gonna send and receive that information to where it's not like a webpage
[22:10] in a browser, but can I just get the computers to talk over HTTP?
[22:15] And so, somebody came up with the idea of REST. And the reason is with HTTP,
[22:21] the way that the protocol is made, and it's kind of this communication protocol.
[22:26] When I contact a web server saying, "Hey, go get me iandouglas.com as a website,"
[22:35] that server doesn't remember who I am. Like we use cookies and things like that to say like,
[22:40] "Hey, this is who I was last time, this is who I am again." But inherently within HTTP, there's no recognition.
[22:49] And so, we call that a stateless protocol because it doesn't remember the state of who you are.
[22:55] And so, for example, if you wrote some code that connected to a database,
[23:02] you authenticate to that database, and then that connection stays open.
[23:06] And as long as that connection stays open, you can do all kinds of things back and forth
[23:09] with your database because it knows who you are. But with HTTP, it's stateless
[23:15] because every time you connect to it, you say, "This is who I am, this is the information I want,"
[23:21] it gives you that information, and then you close that connection.
[23:23] Well, the next time you wanna talk to that server, you gotta go through this whole like magic handshake
[23:29] all over again of, "Hi, I'm Ian, these are my credentials, "can I please have this information?"
[23:35] And then it hangs up again. And so, the idea of coming up with REST,
[23:39] REST actually stands for a representational state transfer. So, the R-E is representational,
[23:48] and then the S is state, and then T is transfer. And this is to kind of make kind of like a stateful
[23:59] sort of feeling because of HTTP is stateless. - Okay, and you said earlier for HTTP, it's stateless what?
[24:13] - It's a stateless protocol, which basically means it doesn't remember from one connection to the next
[24:19] who you are, because you're just coming from some IP address, it doesn't know who you are.
[24:24] Like, there's no inherent trust in the protocol itself. The protocol is pretty dumb.
[24:31] It's like making a phone call, and I call, and I say, you know, like maybe I know your phone number.
[24:36] So, I call and say, "Hi, Jen, I'm Ian. "I'm this developer from Postman.
[24:42] "I got a question for you. "Can you give me some information?"
[24:44] Okay, cool, and we hang up. The next time I call, so imagine like way,
[24:49] way back in the day, I don't know if you're old enough to not remember a caller ID.
[24:53] - Yes, I do, I do. - Way, way back in the day, the phone would ring,
[24:56] and you would just pick up the phone because you didn't know who it was that was calling.
[25:00] - Or as my family would say, "Hi, thank you for calling "the Genov residence.
[25:05] "How may I help you?" - Right. - Yeah.
[25:07] That is how my parents told me to answer the phone when I was like six.
[25:11] - Right, but that's also kind of how these protocols work. Like the server's gonna answer,
[25:16] and then there's this little like handshake chitchat back and forth of this is who I am, this is who I am.
[25:22] Here are my credentials. Okay, I accept those credentials.
[25:25] Like there's this whole back and forth thing at a really low level.
[25:28] And so, back in the day, there was no caller ID. You would just call, and I would have to explain
[25:34] all over again, "Hi, Jen, I'm Ian. "I'm this developer from Postman."
[25:38] Now, you as a human, you'd be like, "Oh yeah, I remember you.
[25:40] "You just called me a minute ago." - Right. - But the computers are dumb.
[25:44] HTTP is kind of dumb in that sense. It doesn't remember who you are
[25:49] because there's no kind of like a caller ID kind of thing of like you're just coming in from an IP address.
[25:56] And so, it doesn't remember who you are. And so, that's why we call it a stateless protocol.
[26:02] And so, then we've got to go through this whole handshake every time I connect saying, "This is who I am."
[26:08] And you check my credentials and say, "Okay, you're allowed to ask me
[26:13] "for certain kinds of information." I can say, "Cool.
[26:17] "What's your favorite color?" And you tell me that, and I'll be like,
[26:19] "All right, cool. "Got that, written it down.
[26:21] "Thank you." And we hang up.
[26:23] And then I have to call you back, "But by the way, what's your favorite boy band?"
[26:28] Or something from the '90s. And you tell me that, "Okay, cool."
[26:30] And we hang up, and then I call you back, and, "What's your favorite food?"
[26:33] And you tell me that, and, "Okay, cool." And then we hang up.
[26:36] But every time I call you, I have to go through the whole, "Hi, I'm Ian.
[26:39] "I work at Postman." We've got to do that handshake every single time
[26:44] to kind of mimic the state of this is who I am, and so on. So, HTTP is kind of a dumb protocol.
[26:55] It doesn't remember this state. And so, the idea of REST is we wanted to kind of
[27:02] add a layer of state on top of HTTP, where we can kind of pretend that we know
[27:10] what you're talking about and what it is you're trying to do.
[27:13] So, when we fetch a webpage, for example, you've got the domain name, like google.com,
[27:19] but then you've got the path after that, like /something, /something.html, or whatever.
[27:25] And the rest of that path is what we call the resource. And that resource is something
[27:31] that we're trying to interact with. And so, the idea with REST is we use that path
[27:36] where you might have like an ID value of I want to go get user number 15,
[27:42] or I want to go get the weather for Denver. And so, those components are going to be part
[27:48] of the overall URL that we're trying to interact with. And so, the idea of REST is that we're using
[27:55] a combination of that path as this is the resource that I want to interact with to kind of mimic a state of,
[28:04] hey, you know who I am, but under the hood, we still have to go through this whole handshake
[28:10] of hi, I'm Ian, I work at Postman, here's my credentials, and all this kind of stuff.
[28:17] Really quick, something that is... That, wow, words, Jen, words.
[28:29] I'm going to write it out because I don't know how to verbalize this.
[28:34] - No, no worries, no worries. - And then...
[28:45] Good tech, I can write my own domain name. So, you were talking about how it calls this resource.
[28:54] And the reason I'm showing both of these, y'all, is again, if you haven't caught on,
[29:01] I was taught from shared hosting world. There was not as much out there in the world
[29:06] as I thought that I found out there is. And that has caused me to go, wait, you're saying this,
[29:13] but is this the same? Because from what I understand is the forward slash blog
[29:21] in this example, that would be the resource, and that could be a folder or a file within...
[29:27] - Within the server, yeah. - Within the server, where blog dot could be the same thing,
[29:34] or it's specifically a subdomain that could point to anything.
[29:38] - So the blog dot is what we call a subdomain on your teachgentech.com domain name.
[29:45] So teachgentech.com is your domain name. The dot com is what we call a top level domain.
[29:50] And so we kind of break them out right to left. So dot com is the top level domain,
[29:55] and then it's your domain after that, which is teachgentech.
[29:59] And then anything to the left of that becomes a subdomain. - Okay.
[30:04] - That's a whole other thing we can do. - Yeah, it was more about you needed a refresher.
[30:09] - That will be important to kind of go through with the APIs, but the slash blog is the resource.
[30:14] But when you call just blog dot teachgentech.com, that's still asking the server, like,
[30:21] "Hey, I want to get a resource at this path." In this case, it would just be slash at the end.
[30:27] And so you're just saying like, "Hey, I need to go get the resource found
[30:29] at blog dot teachgentech.com slash." And then it's up to the server to try to figure out,
[30:36] "Is that a resource I can even give you? Or do I give you a 404 error?
[30:40] Or do I have to ask you for credentials?" You know, things like that.
[30:45] So when we- - You just helped collect something.
[30:49] Sorry, I know I'm going off. - No worries.
[30:52] So the resource that you're interacting with on the first line, teachgentech.com slash blog,
[30:59] slash blog is the resource. - Yes, so let me go put this in my random notes area.
[31:05] - No worries. So it's using that path as,
[31:11] "This is the resource that I want to interact with." Now, when you pull this up in a browser, excuse me,
[31:16] when you put this in the address bar of your browser, the browser is saying, "Okay, I need to go fetch this."
[31:22] And so HTTP has a number of methods that it can operate on, which is how it's sort of sending and receiving information.
[31:31] And when we connect to a server saying, "Go fetch this resource,"
[31:36] we're saying, "I want to go get this resource." And so there's an HTTP method called get.
[31:41] And so if we were to actually look at the low level, like what actually gets transferred to the server,
[31:47] the first word that gets transmitted is the word get. And we say, "I want to get teachgentech.com/blog."
[31:55] And so we've got these HTTP methods, and we're going to talk about five of them.
[32:00] There are five most common ones. There are others, but they're not going to be,
[32:04] they're not as readily used by people who do programming. There are a lot of different ones out there,
[32:14] but we're just going to talk about the five most common ones.
[32:17] And by far the most common one that we're going to interact with is just a get,
[32:22] where I'm saying, "I want to get some information." So for the longest time, since HTTP was created,
[32:28] get was the very first method in the HTTP protocol of I want to get some information from the server.
[32:35] - Okay. - And so we use this for what we call fetching of data.
[32:44] So get, fetch, it's all kind of the same thing. Like you're going to gather something.
[32:49] So we use the word get. The second one that was created back in the day was post,
[32:56] which is basically I want to send some information to the server.
[33:01] And so get is where we're fetching information. Post is where we're sending information.
[33:05] In early HTTP days, if you had like a form that you were filling out,
[33:12] like on a webpage where you're filling in all the different fields and you click a submit button,
[33:16] that was being sent over a post operation. So the browser kind of behind the scenes
[33:22] knows how to do a post, but when you type an address, like a URL in the address bar,
[33:27] that's only ever going to do a get. And so the browsers were kind of dumb.
[33:31] They could only do a get and a post. Once we started getting into JavaScript,
[33:36] then JavaScript had access to some of these other methods that we're going to talk about
[33:40] and sort of what they're used for. But this is where the REST and the RESTful API
[33:47] kind of adopted these HTTP methods saying, I want to use these methods on these resources.
[33:54] So now I don't need a browser to do this stuff anymore. I want to use a combination of the HTTP method
[34:02] and the path of the resource that you're trying to interact with.
[34:07] So in this case, /blog, I want to get /blog. And we could make that an API call to say,
[34:13] go get that information. If you've used WordPress,
[34:19] like a very default installation of WordPress as a blog engine, when you make a blog post,
[34:25] it would have like /blog/1. And that number one is like your blog article number one.
[34:31] Well, when you pull that up in a browser and you send that to the server,
[34:33] the server's like, okay, I need to go fetch blog article number one,
[34:37] and it returns all of the HTML and so on. But when we call that sort of resource from an API,
[34:43] we're saying, hey, I just want you to go get whatever the data is there for resource number one from blog.
[34:51] And so REST is using that path of /blog/1 as the state of this is the resource
[34:58] that I want to go interact with. And then it looks at the HTTP method
[35:02] for how we want to interact with that thing. Do I want to get it?
[35:05] Do I want to post a /blog? Do I want to delete that blog entry?
[35:12] So there's all these other methods that we're going to talk about,
[35:14] but they will interact with the path of your URL. (murmurs)
[35:20] Okay, would this be a proper way of saying it, is it would find a resource to interact with
[35:47] via the domain path? - So I would change two words in here.
[35:50] I would change the word find to be, we want to identify the resource
[35:59] because finding implies that we're trying to get something, but we might be trying to manipulate what's already there.
[36:08] So we're using that path to identify the resource that we want to interact with.
[36:13] And then I would change the word domain to be URI. So there's URL, which is everything,
[36:24] the protocol, the domain name, and the path. But when we talk about just the path of /blog/1,
[36:30] that's what we call the URI. It's a universal resource identifier
[36:34] where URL is universal resource locator. The identifier is, so just, I would just write in the URI.
[36:43] Yeah. - But I am going to put universal resource...
[36:50] - Identifier. - Instead of locator, locates.
[37:03] That makes sense because I'm, okay, cool, cool, cool. Thank you.
[37:08] - Yep, no problem. So REST is, it was a very rigid set of rules.
[37:14] Like this is exactly how we're going to make this sort of REST API thing happen.
[37:21] It has to follow these exact rules. Well, as soon as you tell a programmer,
[37:25] you have to follow these rules. Every program is like, I want a little bit of wiggle room.
[37:29] I want to kind of do it my way. And so people are like, well,
[37:32] do we have to do it exactly that way? Like, can we have a little bit of flexibility here?
[37:37] And so around 2005, somebody actually proposed, well, let's just call this REST full.
[37:44] So it's not strict REST, it's a REST full API. So it's still kind of following the theme
[37:52] of using these HTTP methods, as well as the URI path to identify our resource
[37:59] in order to interact with that resource. But we're not holding very super rigidly
[38:05] to this set of rules that was proposed around the 2000 era. - 2005-ish.
[38:13] And I am writing down dates. And for everyone watching,
[38:19] a big reason why I'm also writing down dates is, again, I am learning things out of context
[38:25] and trying to understand things with other contexts I know. And part of when I worked at Stoplight,
[38:32] it was like learning about like open API and things like that.
[38:36] I don't wanna go down that rabbit hole, but that is why I'm like, okay,
[38:41] eventually I'm gonna have a timeline and connect all of these things at some point.
[38:46] Okay, so- - 2005-ish, we wanted some flexibility
[38:51] and that flexibility is where we came up with REST full API.
[38:55] So in modern days today, when you hear somebody talk about a REST API,
[39:01] they really mean they're doing it REST full. Very, very few places are actually very rigidly holding
[39:08] to the original REST API specification. Everybody's kind of doing REST full.
[39:15] I used to joke at one job that I used to call our API, our insomnia API, because it wasn't very REST full.
[39:22] - Oh, geez. - You're trying to conform to even a REST full idea
[39:26] of what an API was, but we were like really mangling it at the time.
[39:30] And so I joked internally that we were calling it our insomnia API, it wasn't REST full.
[39:34] - Oh, geez. - So this is where the idea of REST full came about.
[39:40] And because of this flexibility, it made this kind of API access
[39:44] between servers extremely popular. And to this day, by far,
[39:49] if you're interacting with an API where you're like sending
[39:53] or retrieving data over the internet, chances are really, really good,
[39:56] it's gonna be a REST full API. - Cool, cool, okay.
[40:00] So I wanna recap really quick 'cause I feel like I'm getting it,
[40:04] but at the same time, I'm like, wait a minute, what? So when we were talking about REST APIs,
[40:11] they were only using HTTP protocol, or HTTP protocol is saying protocol twice like ATM machine.
[40:19] - Right, yeah. - But for some reason,
[40:21] it makes sense saying that it's a protocol. So because it was like,
[40:28] hey, if we just do it based off this regular protocol, it's stateless,
[40:33] meaning that it's never gonna remember anything. We have to reauthenticate every time.
[40:38] It's gonna take forever and a day, and there's not enough.
[40:42] It's gonna take forever, so we're not gonna do it. So then they were like,
[40:46] yo, let's make representational state transfer. And so it's still, is it still using,
[40:55] it still uses HTTP, but instead of it having to reauthenticate every time,
[41:03] it is identifying the resource it wants to interact with? - No, it still has to do that handshake
[41:10] every time it connects. - Okay.
[41:13] - But the idea of state is really, like what is it that we're trying to manipulate?
[41:20] So when we think of like, I wanna, I want Python or JavaScript or whatever
[41:24] to manipulate or connect to a database and interact with that database,
[41:30] you authenticate one time and you just have, you've got that open pipe to the database
[41:35] and you can just manipulate whatever you want as long as you're allowed to.
[41:38] With the idea of HTTP is that you, because by its very nature, it makes a connection.
[41:48] You send, like I send a request, you send me a response, and then we hang up.
[41:53] The next time I connect, we've gotta, you've gotta make sure that I'm still allowed
[41:56] because I'm just showing up from some IP address. You don't necessarily know who I am.
[42:01] - Right. - And this is why we came up with things like cookies
[42:04] and stuff like that. So even on a webpage, for example,
[42:07] when you say, I wanna go get this webpage, when you make that request,
[42:09] it's actually sending you all of the cookies for that site to the server saying,
[42:14] by the way, these are all the cookies that you told me to save last time
[42:18] that may indicate to you who I am. And so that's why when you log in at, say, Amazon
[42:23] to do some shopping, and then you close your browser and tomorrow you go back to Amazon,
[42:28] Amazon still remembers who you are. The dumb HTTP protocol just says like,
[42:33] hi, I need the homepage for Amazon. By the way, here's all my cookies.
[42:37] Amazon looks at those cookies and goes, oh, it's Jen. Jen's back to do more shopping for more cool lights.
[42:43] And it sort of, it kind of remembers who you are. It doesn't remember it's because we're sending
[42:49] that information to say this is who I am. And so there's still an authentication,
[42:54] but the idea with REST is that you're identifying, like REST is using the HTTP method plus the path
[43:03] in order to mimic a state of this is the resource that I wanna interact with,
[43:08] and this is how I wanna interact with it. So the HTTP methods are how we wanna interact
[43:16] with the resource that we're trying to, yeah. So get it, get them post, yeah.
[43:21] And we're gonna talk about three more. - Yeah, I feel like it's starting to make sense,
[43:25] but at the same time, I'm like, something is still missing, but that is okay.
[43:30] This is, I've learned, it's taken me a while to learn that it doesn't need to click right away.
[43:36] It clicks enough so I can continue, but it's okay if it doesn't like quite stick yet.
[43:41] - Yeah, it's okay. - We're gonna go from stateless to REST,
[43:47] intellectually and learning, okay, anyway. - So HTTP is always stateless, no matter what.
[43:55] REST is kind of like the next layer up where we're trying to mimic some idea of state
[44:01] and what it is we're trying to interact with by using that path, as well as the HTTP method
[44:08] to kind of combine those two things as far as like, this is how I wanna interact
[44:13] with this resource. And then REST full is basically,
[44:18] we wanted some flexibility there where it wasn't this rigid set of rules
[44:23] that we had to follow very explicitly. We wanted a little bit of flexibility on,
[44:27] does it have to be slash blog slash one? Could it be slash blog slash hello world?
[44:32] Can we still go find that as our identifier? Like, does it have to be a rigid integer identifier?
[44:39] Does the path have to, you know, et cetera? And so the idea of REST was a very rigid set of rules
[44:45] where REST full, we as programmers kind of rebelled a little bit and we're like,
[44:49] nah, dude, we want some flexibility here. And that's where we came up with REST full.
[44:54] So we don't have to follow those rules exactly, but we still kind of stay with the theme
[44:58] of we're gonna use those HTTP methods to interact with a resource,
[45:02] but we've got a little more flexibility as far as like how we do that
[45:06] and the status codes that come back that indicate whether it was successful or not
[45:10] and so on and so on. - Would you say being able to use a string then?
[45:29] So that way it's like blog slash Ian? - Yep, and so nowadays when you set up WordPress,
[45:38] it'll typically come up with like a URL friendly version of whatever title of your blog post is.
[45:44] So you don't see slash blog slash one, it'd be like slash blog slash welcome dash to dash my
[45:51] dash blog exclamation point or something. And when you tell the server, hey, I want this resource,
[45:58] it looks at that title and it tries to figure out, okay, which one does this actually match in the database?
[46:03] And then it goes and retrieves that for you. - We're just gonna say teach gen tech API.
[46:15] So it'd be teach gen tech API as my example today. Yay. - That's good.
[46:26] All right. - Okay, cool. Thank you.
[46:27] - So that was where we kind of came up with the idea of RESTful
[46:31] is we just wanted a little more flexibility on how we use these HTTP methods and paths to do a thing.
[46:37] But we still like, even in 2023, we still just talk about them as REST APIs,
[46:43] but if you hear RESTful, we basically mean the same thing.
[46:47] Very, very few places are actually very rigidly holding on to REST and saying,
[46:53] no, this is a proper REST API. Those kinds of companies are very pedantic about it
[46:59] and so on, but very few companies are actually very strictly conforming to REST.
[47:04] Pretty much everybody that does a REST API is really doing a RESTful API,
[47:09] where it's following the theme of it, but it's good to know,
[47:15] but it's also bad because that means every company has a slightly different way of building a REST API.
[47:22] And so how you might interact with one REST API, REST API, which is RESTful API,
[47:30] is gonna be slightly different as far as how do we authenticate,
[47:33] how do we, like, what's the path of that resource, because every company is gonna be a little bit different
[47:38] in how they implement it. It can add to a little bit of confusion
[47:42] to people who are trying to build, or rather consume APIs in the first place,
[47:47] as an end user of, hey, I wanna go get the weather. Well, is it slash, you know, weather slash Denver,
[47:53] or is it slash weather slash 642, because that's the city code for Denver?
[47:59] Like, you know, because it's not strictly REST, you know, and so every company wants to do it slightly differently.
[48:05] It may not even be slash weather, you know, it could be, you know, several path levels deep
[48:10] or whatever to basically interact with that API. And so it's good and bad.
[48:18] It's good for the company and for the programmers at the company,
[48:20] because they have flexibility in getting to do what they wanna do.
[48:24] It's bad for the end users, because now every REST API looks
[48:27] and feels a little bit different. And they're, you know, it's all kind of,
[48:31] okay, I've got the, you know, I've got a method and I've got a path.
[48:35] But aside from that, like how I actually interact and authenticate and, you know,
[48:40] what kind of protocol am I using? Like it made it very, very different.
[48:44] The other downside is with REST APIs, the server doesn't,
[48:55] sometimes it doesn't have a lot of control over what the end user is trying to do.
[49:02] So for example, if I said, "Hey server, I wanna send you some information.
[49:05] Like I wanna do a post operation on this resource." And the server comes back and says,
[49:09] "Okay, I got you. Fam, what you got?
[49:12] Send me whatever data you wanna send." And I start sending like terabytes of data.
[49:16] The server has no way of saying like, "Hold up, hold up, hold up.
[49:19] That's way too much data. You can't send me that much data."
[49:22] It has to wait until the whole thing finishes before the server can respond and say,
[49:26] "Nope, I can't handle all that data that you sent me. Sorry, you just spent all that time
[49:30] transferring all that data and I can't even handle it." - So, okay, you say that.
[49:35] And again, for anyone joining us for the first time today, Ian is from Postman and understands APIs very, very well.
[49:45] And I have been, had teach Gen Tech streaming for almost a year now.
[49:51] And I am definitely piecing things together. And as you're saying with the pulling information
[50:00] off the server, no matter how large it is. I started working at Ivan,
[50:06] which is a data infrastructure company about two months ago. And we, part of my new role is learning about Postgres
[50:15] and which is a database. It's a relational database,
[50:18] which I don't quite know what that means, but I will someday.
[50:22] Anyway, when they do a query on a database, is that technically using an API because it doesn't,
[50:30] since it's just gonna pull no matter how large of an amount, or is it only an API if a web,
[50:36] like something else is pulling the querying it from the outside?
[50:40] - Great question. So at the very beginning of the session,
[50:42] we talked about the idea of abstraction. So when you're interacting with a database,
[50:48] you're still abstracting the instructions of storing and retrieving data.
[50:52] So technically that is using some kind of API. You've got some sort of language and protocol of,
[50:57] this is how we're gonna send and receive information from one another.
[51:00] So that's still using a type of API. It's not the same kind of like restful API.
[51:07] Like you don't connect to a database with a get or a post. You're, it's gonna have its own communication protocol.
[51:14] That's not HTTP. - Interesting.
[51:18] It's starting to click. Really quick, just to,
[51:21] I am putting this down here in my like other notes for REST API downfalls.
[51:26] Of all companies do it different. And you said that it's with security and what else?
[51:32] - For things like authentication and- - Authentication, thank you.
[51:37] - And like how they basically build the API. Like everybody builds their API slightly differently.
[51:42] Some people, you know, do you have like query parameters? That's where you have like the question mark on the URL
[51:49] and the questions, you know, where you've got the parameters there.
[51:52] Some people want those things in headers where you're sending the headers instead of parameters.
[51:56] Some want both, you know, how do you send that API key? Is it a query parameter?
[52:02] Is it a header? How do you indicate what kind of content you wanna get back?
[52:06] Do you wanna get it in JSON format? Do you want it in XML format?
[52:10] Do you want plain text format? Like, can you even tell the server
[52:13] how you're gonna get that data back? Or does the server, is the server rigid
[52:17] that it can only give you back one kind of data? So if you connect to a server and say,
[52:22] give me the weather information in XML format. And it says, sorry, I can only do JSON.
[52:27] You know, now you've got kind of this miscommunication. So every company is doing things slightly differently,
[52:31] which ends up confusing people who are new to interacting with APIs.
[52:37] - And then you said that the other REST API is when you do call something,
[52:43] there's no way of stopping the data limit because it's just gonna load everything that you ask for.
[52:48] - Yeah, so a good analogy would be like, hey, Jen, you know, I call you on the phone and be like,
[52:53] hey, Jen, can I read you a story real quick? Can I read you a story?
[52:58] - Sure. - All right.
[53:02] Well, Prince, Genoa, and Luca are now nothing more than appendages of the Bonaparte family.
[53:08] I warn you that if you don't tell me we're gonna have war, if you still allow yourself to condone all the infamies,
[53:14] all the atrocities of this antichrist, on my word, I believe he is an antichrist.
[53:18] I will not recognize it. It's war and peace, right?
[53:21] You're not gonna sit and like wait for me to read the entire story of war and peace.
[53:25] You'd be like, hey man, like it's lunchtime, I gotta go. The server has no way of interrupting a client
[53:31] when the client says, hey, can I send you some data? The server's like, yeah, okay, go ahead and send it.
[53:36] It has to wait for the client to send all of that data to go, dude, you just made me sit through war and peace.
[53:42] Like, I thought you were gonna read like a poem that your kid wrote.
[53:44] And so the server has no way of interrupting with a typical REST API.
[53:51] It has to wait for the client to send everything to the server for the server then to say like,
[53:57] hey, all that time and effort you just spent sending me all that data, I just dropped it on the floor.
[54:01] I can't deal with all of that. I can't even, right?
[54:05] It's got no way of like stopping that interaction in the process.
[54:09] So these are kinds of drawbacks that servers have. And it's partly from HTTP and it's partly
[54:16] from just how we build software. But so there are benefits and disadvantages
[54:23] to all these different kinds of APIs that we're gonna talk about today.
[54:26] So, like I said, the most popular kind of API is a RESTful API, which is typically I call,
[54:34] like I call Jen and I say, hey, Jen, I got one question for you.
[54:39] What's your favorite food? And you tell me your favorite food is?
[54:43] - Pizza. - Cool, thanks.
[54:46] And I hang up the phone. And the next time, hey, Jen, what's your favorite topping
[54:52] to put on a pizza? - Cheese.
[54:55] - Okay, cool. And then I hang up the phone and then I call,
[54:59] hi, Jen, I'm Ian at Postman. We go through this whole authentication.
[55:02] What kind of cheese do you like to put on your pizza? - I don't know.
[55:07] I just like gluten-free cheese pizza. - Okay.
[55:11] - That's not the response you were looking for, no. - Unknown, all right, cool.
[55:14] And I hang up and I call back again. You know, hi, I'm Ian from Postman.
[55:19] Jen, what's gluten-free mean? You know, and then, you know, you have that.
[55:24] I mean, that's a whole other conversation. And we have, so the idea with a REST API
[55:28] is it's a single transaction. I make a request, you send me a response,
[55:33] and then we say, bye-bye. And the next time we got to jump through
[55:36] all those authentication hoops every single time. And so with a RESTful API, you connect to the server,
[55:42] you make a single request, you get a single response, and then you hang up.
[55:48] So when we talk about like, how do we load a webpage? So you imagine you go to something like a Pinterest page
[55:56] and you say, okay, I wanna go get pinterest.com. Well, what the server sends you back
[56:04] is just the HTML of the page. It doesn't send you anything but the HTML.
[56:11] What your browser has to do then is interpret everything in that HTML to say,
[56:14] okay, well, there's this CSS, you know, style sheet I have to go fetch.
[56:19] There's some JavaScript I have to go fetch. I've got all of these images of all the coolest crafts
[56:24] and whatever the people are putting on Pinterest. It has to go back to the server every single time.
[56:29] Hi, I'm Ian from Postman. Can I please have this image?
[56:32] Cool, thank you, click. Call back again.
[56:35] Hi, I'm Ian from Postman. Can I have this image?
[56:38] Cool, thanks. Click. - That would take forever.
[56:40] - Hi, I'm Ian from Postman. Can I please have this or that?
[56:43] Well, the browsers are pretty good at sending multiple requests at a time,
[56:47] but each one of those is an individual request going, hi, I'm Ian, can I please have this resource?
[56:52] Because REST is a single transaction of, I want a single, here's my single request,
[56:59] I want a single response, and then we hang up. So it's inefficient
[57:07] if you want multiple pieces of information. And so most REST APIs, when they work on HTTP,
[57:17] they're using HTTP version one, or version 1.1 is more common.
[57:22] And version one is the single transaction of single request, single response.
[57:28] - Request, and then a single response. Okay, and that makes sense.
[57:46] - Yep. - So that was all fine and good.
[57:49] And for most APIs, that's all we need. Like, hey, go get me the weather in Denver.
[57:53] Go fetch my latest list of new emails. Go get my, you know, the newest things
[57:59] on my Twitter timeline. Go get, you know, whatever.
[58:02] We're making a single request, we get a single response of data,
[58:05] and then our software interacts with that. - But if we, for a single request and a single response,
[58:12] can that request have, like, how you were asking about pizza of like,
[58:19] hey, what's your favorite crust? What's your favorite topping?
[58:23] What's your favorite cheese? Those are all different requests
[58:26] instead of one request with sub requests. - Sometimes with APIs, the developers would be like,
[58:32] let's just take in a whole structure of, you know, what the user actually wants,
[58:36] and we'll try to figure out some way of packaging all that up and sending it all back.
[58:39] But that's kind of moving away from the idea of REST, which is, I want to interact with a single resource.
[58:47] So that would be like, you know, I wanna go register as a user and pull up my profile page
[58:55] and send you a profile image. Like, I'm trying to do a bunch of instructions
[58:58] all at the same time. And that generally kind of moves drastically away
[59:02] from the idea of a RESTful API, where it's like, I'm interacting in a single way
[59:07] with a single resource. Now, even in the case of like our pizza example here,
[59:12] I'm asking for a lot of information about pizza. So that might be where we put in query parameters.
[59:17] Like, I wanna interact with gen.com/favoritepizza, and then I start sending in query parameters
[59:25] of favorite crust, favorite cheese, favorite topping. - Query parameters would be like the sub requests
[59:31] that I'm calling it. - Maybe, yeah.
[59:33] Or just, you know, while you're fulfilling my request to go get favorite pizza details,
[59:40] I specifically want these details or something like that. And so that's where sometimes we'll get
[59:44] into query parameters on, you know, instead of going and getting every pizza,
[59:50] you know, topping out there, I wanna get just, you know, send me 10 at a time
[59:54] and we can get into like pagination and things like that. Where I could say like, just give me,
[59:59] like however many pizza deals you got, just give me five pizza deals at a time.
[60:03] And if I want more than five, I'll ask for the next five pizza deals.
[60:07] Kind of thing. And so that's where we get into query parameters
[60:09] where we can kind of filter things down a little bit. But again, it's up to the programmers
[60:13] for what we want to build and how we wanna build that API interaction.
[60:18] And does that strictly follow, you know, kind of our best practices and industry norms.
[60:26] And again, this is where it's good and bad because for the programmer,
[60:31] it gives us all the flexibility that we want, but it's bad for the end users
[60:35] because now that pizza API acts drastically different from some weather API where you're also trying to say,
[60:42] go get me the weather for the following cities. Maybe they do it completely differently.
[60:47] So there are a lot of good and bad things about using a RESTful API in this sense.
[60:54] So yeah, there are ways that we can ask for more than, you know, one bit of information at a time,
[61:00] but that also kind of drifts away from, sort of what the intention was behind building an API
[61:08] around interacting with a single resource at a time. - So I just said, just like the request of,
[61:26] what is your favorite pizza? That would be a one request,
[61:29] but then in the query, it could be the five most recent responses,
[61:34] you know, favorite crust or like favorite topping. - Yeah, so some APIs will allow you to interact
[61:41] in a way that says like filter the results in some way or like, you know, go get me all the authors
[61:48] that you have in your library, sort them alphabetically
[61:50] and just give me the first 10 authors or something like that. Like you can sometimes interact with APIs
[61:55] if the API developer has actually built those kinds of controls.
[61:59] And they may not have, you know. - Are those types of controls and those filters,
[62:05] those are always after they call the information or request the information.
[62:10] - It's part of the request. It's part of the request.
[62:12] Because again, when I connect to you and say, hi Jen, I'm Ian from Postman.
[62:16] I would like this information. That's all I'm allowed to say.
[62:20] I have to then wait for your response and go, okay, cool, thank you.
[62:23] And I hang up. Whether that response was actually valid or not,
[62:27] I had to make my request all in one shot. And so that's where you would send the path
[62:31] and the query parameters and the headers and cookies and things like that.
[62:34] You send all of that as your request and then you wait for a response to come back.
[62:40] - So some people could be like, okay, I think I get it.
[62:48] I'm good. - It'll probably get more clear
[62:52] like as we talk about it a little bit more as we go. - Cool.
[62:56] - So this was all fine and good if we had a single request and we expect a single response
[63:01] and that's the end of it. But we started to realize as an industry,
[63:05] it's like, well, that's a little bit limiting. What if we want to ask for multiple things?
[63:10] And so this is partly where HTTP/2 came into play, where in the new version of HTTP/2,
[63:17] well, I mean, it's not really that new. It's actually been out for a number of years now.
[63:22] But with HTTP/2, we can actually make a connection to the server and say,
[63:26] I want the following list of resources. And then we get a response back
[63:30] which encapsulates all of those responses. So I can say, I can make a single request going,
[63:36] give me pinterest.com's homepage. And it gives me back that HTML.
[63:40] Now my browser can go through and I can break out, okay, I need this CSS page, this CSS page,
[63:45] these 10 JavaScript script files, the ads and all of the images.
[63:51] And then it can reconnect to the server and say, here's a list of things that I want you to give me back.
[63:56] And now the server can send all of those things back in a single response.
[64:00] And so that was one workaround instead of saying, can I get a list of crusts and pizzas and whatever.
[64:07] HTTP/2 now will allow for, here's a bunch of things I want you to give me
[64:13] and it comes back. But that's still a single request of I want this information
[64:21] and a single response of, here's a package of that information.
[64:25] So HTTP/2 will allow you to request multiple resources, but it's still a single request for all of those resources
[64:34] and a single response of all of those resources. - Okay.
[64:40] I think that makes sense enough. And what up B1 mind?
[64:45] I'm trying to reply to people while you're talking so I'm not interrupting.
[64:49] 'Cause I'm like, I also like really want to learn this. - Well, I'm watching Twitch kind of on the side as well.
[64:56] So folks have questions about APIs, like feel free to drop that stuff in Twitch chat.
[64:59] I'm not sure what other platforms you're streaming on other than Twitch.
[65:02] - Just Twitch now. I just stream on Twitch and then I upload to YouTube,
[65:06] which surprisingly doing that gets more YouTube views because it's a video and not a stream.
[65:13] - Well, but it hangs out longer and people can watch asynchronously.
[65:17] They can watch at their own pace and so on. - Really quick, y'all.
[65:22] Ian is also very, very technical. We are going through the basics right now,
[65:28] but if you're like, hey, I have a question that's a little higher
[65:30] than what we're doing right now. This isn't a troubleshooting stream.
[65:34] I do have to say that, but a lot of times it is something we can help out
[65:39] and figure out. And thank you, Sahay, for the follow.
[65:46] I appreciate it. And okay, so we are-
[65:49] - Yeah, so if folks have questions, feel free to drop it in chat.
[65:52] We'll try to address like API questions as well. I've got kind of a list of things
[65:56] that I wanna work through, but if it's part of that,
[65:58] then I'm happy to jump around and answer stuff too. - Yay.
[66:02] Thanks, Ian. - So HTTP/2 will allow us to request multiple resources
[66:07] and get a response back with multiple sort of resources in that single response.
[66:14] But HTTP/2 also allowed for what we call streaming requests and streaming responses.
[66:22] And that's where we're gonna talk about a little bit different kind of API here in a minute.
[66:26] - Okay, let me go back, because something just clicked as you were saying that,
[66:31] that I'm like, okay, my brain's not ready to move on. When we were talking about multiple resources,
[66:36] it's like talking about how over here, we're talking about resource.
[66:41] So does that mean like, instead of having to only call this resource,
[66:47] it could call /blog/pizza/ like different areas. It doesn't have to be one specific area.
[66:57] - It's gonna be a different structure of that request, but yeah, it's basically sending a single payload
[67:03] to the server saying, hey, Jen, I've got the following questions for you.
[67:06] What's your favorite number? What's your favorite food?
[67:08] What's your favorite sports team? What's your favorite boy band?
[67:10] What's your favorite pizza? Give me all that information back.
[67:12] And you're gonna go grab all that information and say, here's my response.
[67:16] My favorite number is blah, blah, blah. My favorite food is blah, blah, blah.
[67:19] And you're gonna give me all of that back as a single response.
[67:21] And then I say, cool, thanks. And then we hang up.
[67:23] Because that's the typical RESTful kind of approach is we make a single request, we get a single response,
[67:30] and then we close that connection. Now that single request over HTTP/2 can say,
[67:36] I wanna get a whole bunch of things. And that way I only have to do
[67:40] that magic authentication handshake one time. I can request a whole bunch of things.
[67:45] The server can process whether I'm allowed to actually get those things
[67:48] and then send them back as a single response, kind of all bundled up of like,
[67:52] here's this collective response to all of those things that you requested.
[67:56] - I know this is very simplified, but for my visualization,
[68:11] I'm gonna say V1 is forward slash blogs. And that's the only place that can get content.
[68:18] And V2 could be blogs. - And images. - HIV.
[68:25] - And CSS and JavaScript. - Images. I'm gonna say pizza.tss.
[68:35] Dot TSX, right? Like it could do whatever the, what it wants to do.
[68:40] It could be, you know, yay.js. Okay, cool.
[68:49] That gives me. - Yep, yep. You got the idea there.
[68:51] - Yes. Thank you.
[68:53] - So we realized like, hey, this HTTP/2, like that actually opens up a whole other thing
[68:59] that we can do because HTTP/2 also gave us some flexibility about do we have to hang up after we get that response back?
[69:08] Like, can we just hold this connection open, you know, a little longer so I can call you up and say,
[69:15] hey, Jen, what's your favorite phone number or your favorite number?
[69:21] And you tell me that number and say, hey, while I got you on the phone,
[69:24] what's your favorite color? And you tell me that and say,
[69:26] hey, while I got you on the phone, you know, and so on. Or we could do something where it's like,
[69:32] sorry, I need to take this. - Yeah, go ahead.
[69:38] - Nevermind, I missed the call. If they call back, I have to take that call.
[69:43] - No worries. - So there's,
[69:47] there's some flexibility in HTTP/2 that says like, hey, once I get that response back from you,
[69:57] we don't have to hang up. Like we can stay on the phone for a little while longer.
[70:01] And this is where we came up with the idea of having things that we call like webhooks or websockets.
[70:10] If you've heard of webhooks and websockets, these are using HTTP/2 to basically say,
[70:14] hey, I want to hold this connection open for a little while so that we can kind of interact more long-term.
[70:22] And generally what's happening over like a webhook or a websocket is I make a request to you saying,
[70:28] my request is I want to hold this connection open so that the server can stream back information to me
[70:36] about things that happen. So for example, if you're on say Discord, right,
[70:42] you can set up a webhook for Discord saying, hey, if something happens,
[70:47] can you interact with my Discord on my behalf? So for example, on my Twitch chat,
[70:54] there's a way that you can interact with my Twitch chat that will actually post your Twitch comment
[70:59] on my Discord community over a webhook. And so I have a Python script running on my computer
[71:08] that basically watches my Twitch chat and when something particular happens,
[71:11] something very specific, my Python script says, hey, I want to use this connection
[71:17] that I'm holding open to Discord so that I can say, hey, Discord, can you put this in my Discord community?
[71:24] And I make an API call and it shows up in my Discord community.
[71:28] And then I hold that connection open. So it's kind of like I call Jen and one time I say,
[71:37] hi, Jen, it's Ian from Postman, here are my credentials. And you're like, okay, cool, we can chat.
[71:42] And now I can say, can you go do this thing while I got you on the phone?
[71:47] And we hold that connection open for a long period of time. Not indefinite, not a forever kind of connection.
[71:54] Like internet interruptions happen. Sometimes the server will say like,
[71:58] hey, you can hold this connection open for like an hour or a couple of hours,
[72:02] but then we got to close it up because I need you to re-authenticate
[72:05] because your authentication is only good for a certain amount of time.
[72:08] And so after a certain amount of time, we might as well just hang up the connection
[72:12] 'cause you're gonna have to re-authenticate anyway. So it's really, there can be some sort of communication,
[72:19] protocol communication between the client and the server to determine how long that connection is gonna stay open.
[72:23] But it's pretty much, it's gonna stay open for these webhooks.
[72:28] This allows for what we call server-side events or server-side push where the server wants
[72:34] to push information to you to say, hey, this thing happened. For example, if you hang out on Twitter
[72:40] and you load up the homepage of Twitter and it starts loading your timeline or whatever,
[72:47] if you just stay on that page long enough, you'll notice after a little while up at the very top,
[72:53] it's gonna be like, hey, there's 50 new tweets and you can click on that and it shows all of those tweets.
[72:58] That's because there's a web socket connection that stays open that's saying like,
[73:04] while you're browsing that timeline, I'm gonna like, the server's actually gonna push
[73:10] that information to your client saying, by the way, there's another tweet,
[73:13] there's more recent tweets. There's other things that we wanna push to you
[73:17] as an event that has happened that we wanna alert you to. And so it allows for the streaming of data from the server.
[73:25] And so we can make a single request to the server saying, like, hey, let me know if like anything happens
[73:30] that you wanna alert me about like notification systems. Like on Facebook, for example, if you're on Facebook
[73:35] and you see that little notification bell, if I tag you in a post on Facebook,
[73:40] that thing automatically kind of blips and it's like, hey, Ian tagged you in a post.
[73:44] That's all happening over a web socket or a webhook. - Is that what event streaming is?
[73:51] - Yeah. - That's exciting.
[73:58] So, and it's basically kind of like the server pushes information.
[74:09] - The server is pushing information to the client, yeah. So the client, so it's still doing like a single request
[74:15] to the server saying, hey, I wanna like hold this connection open for a little while.
[74:19] And sometimes like kind of under the hood, there's like this little, like, are you still there?
[74:23] Sort of keep alive ping, as we call it. There's like a keep alive or like a heartbeat
[74:29] of like, I'm still connected, I'm still connected, I'm still connected.
[74:32] That kind of goes back and forth. So the client and server know
[74:34] that they can still communicate, but it allows the server then to keep sending information
[74:39] back to you. 'Cause when you think about what happens,
[74:42] like when I'm on my computer here, I've got firewall software on my computer,
[74:47] I've got firewall software on my wifi, I've got firewall software on my router.
[74:52] And so nobody on the internet can push information directly to my computer
[74:56] because it can't get through three different layers of firewalls.
[75:00] But if my computer initiates a connection and holds that connection open,
[75:05] then whatever I've connected to can send information back to me.
[75:09] And so you kind of think about like, you know, I'm drilling a hole in the dam
[75:12] or whatever to, you know, purposely let a certain amount of,
[75:16] or a certain kind of information in. And so that's basically how web sockets work,
[75:21] is I'm saying over the web, I wanna hold this socket connection.
[75:25] If you know about TCP, it's basically sockets. It's a really low level of how the internet
[75:34] actually like connects and communicates, but- - We'll put that on my one date.
[75:38] - Yeah, so it's using something called sockets. And that's where we get the idea of a web socket
[75:43] is your webpage is making a socket connection to say like, I wanna hold this HTTP connection open
[75:50] to be able to get information back from the server. Well, as long as I've got that connection open,
[75:56] the server can push information to me. I don't have to, otherwise what would normally happen
[76:01] in older RESTful APIs is I would call you up and say, "Hey Jen, is there anything for my notification feed
[76:08] you need to alert me about?" And you say, "No."
[76:10] Okay, cool. And then we hang up, but then I've got to connect again
[76:13] like every minute and go, "Hey Jen, it's Ian from Postman. Do you have any notifications for me?"
[76:16] "No." Okay, cool.
[76:18] And we hang up and a minute later, you know, or seconds later, that makes it for a lot of traffic
[76:23] for me to have to initiate that connection just to get no response
[76:28] and then to have to close that connection. So it's a very chatty kind of way of what we call polling.
[76:34] And so the idea was web sockets is, hey, I'm just going to hold this connection open
[76:40] specifically for this notification feed. So anytime there's a notification,
[76:44] you can just push that back to me and my software is going to say,
[76:48] "Oh, hey, something came in from the server and now we can interact with the UI
[76:52] to actually make that notification bell light up." - So when we go to the web hook and web socket,
[77:00] it's no longer part of RESTful? Or it is like- - It's not RESTful anymore.
[77:04] - It's not RESTful anymore? - Yeah, it's now what we call an asynchronous API
[77:09] because things are happening asynchronously. Things are happening on the server
[77:15] asynchronous to what I might be interacting with on Facebook or Twitter or Instagram, whatever.
[77:20] But when the server says like, "Hey, you get some new notification,"
[77:24] that's getting pushed down to my mobile device or my web browser to where it can like little ping
[77:32] or send a notification or whatever to say, "Hey, Jen liked that new airbrush dragon photo
[77:38] that you posted on Instagram," or something like that. - Yeah.
[77:41] - And so that's how these things happen. So this is all part of asynchronous APIs,
[77:46] which are different from RESTful APIs because now things can happen asynchronously
[77:51] because I'm not polling, polling, P-O-L-L. I'm not polling you for that information.
[77:57] You're able to asynchronously send me that information because we're holding that connection open.
[78:03] - Okay. And polling, like, say that, spell that one more time.
[78:09] - P-O-L-L, not polling, P-U-L-L. I'm polling, P-O-L-L.
[78:15] - Because you're checking or you're, okay. - Yeah.
[78:18] So in the old RESTful times, I would have to make a connection,
[78:21] do all the authentication magic handshake just to say, "Do you have anything new for my notification feed?"
[78:27] And you say, "No," and I hang up. And then, you know, responsible software developers
[78:31] would wait a few seconds and then connect again and say, "How about now?"
[78:35] And, "No, okay, cool," and we hang up. And then I call back a few seconds later,
[78:38] "How about now?" "No, okay, cool."
[78:40] So like, you know, let me call you up and say, "Hey, Jen, can you bake me some cookies?"
[78:44] And you say, "Sure." And then I hang up and I call back and say,
[78:48] "Chocolate chip, please." And you say, "Sure," and we hang up.
[78:51] But then I call you back every 30 seconds going, "Are the cookies done?
[78:54] Are the cookies done? Are the cookies done?
[78:56] Are the cookies done? Are the cookies done?"
[78:58] That gets very repetitive and very chatty. Wouldn't it be better if we could just say like,
[79:03] "Hey, Jen, can you make me some cookies? I'd like chocolate chip."
[79:05] And you say, "Yeah, okay." I'll let you know when they're done.
[79:08] And I just sit on the phone and I wait. And then you say, "Hey, cookies are finished."
[79:11] I'm like, "Sweet, send them over." And you send me those cookies.
[79:14] That's a better interaction. It's a lot less chatter over the internet.
[79:18] Because I'm not constantly calling you to say, "Are the cookies done?
[79:23] Are the cookies done? Are the cookies done?
[79:25] Are the cookies done?" We've kind of, we're holding this thing open
[79:28] to now where asynchronously you can tell me, "Hey, Ian, alert, the cookies are finished."
[79:34] And now I get freshly baked chocolate chip cookies. - Yum, yay.
[79:40] - Subtle hint to make me some cookies. Just kidding.
[79:42] Just kidding. - Right? I was like, you were saying that and I was like,
[79:45] "I think I'm gonna go make some oatmeal cookies when we get done now.
[79:48] That sounds delicious." - Oatmeal raisin? Oatmeal raisin?
[79:50] - Actually, no, maybe oatmeal cranberry. Oh, that's what I'm gonna make.
[79:55] Oatmeal cranberry. I'm probably gonna make them now.
[79:58] - Craisins? Cranberry raisins?
[80:00] - No, they're- - Regular cranberries? - Just regular, they're frozen.
[80:04] So I gotta defrost them, but. - So anyway, so that's how asynchronous APIs came to be
[80:10] is because we wanted a way of saying, like there's gotta be a better way
[80:14] than like constantly pinging the server or asking for this over and over and over again.
[80:18] So we come up with this idea. Now there are downsides to that too,
[80:22] because servers, the way that TCP works, they can only have 65,000-ish connections at a time.
[80:31] And so imagine if you're Facebook and you've got, what, a couple of billion users
[80:36] on your platform. Every server can only have 65,000 connections maximum.
[80:41] That's a lot of servers that you're gonna have to spin up to allow all these connections from all these users
[80:47] who may be on multiple devices. I might have multiple browsers open.
[80:52] I might have a mobile phone and a tablet and maybe a smart TV all connecting to Facebook.
[80:58] So maybe me as an individual user, I've got like 30 of these WebSocket connections myself,
[81:04] multiply that by billions of users, right? And so TCP only allows for 65,000-ish connections.
[81:11] And so we needed a way of... So that's the downside to WebSockets
[81:18] is you're basically holding open one of those connections for a long period of time.
[81:23] Where with RESTful APIs, as soon as I get that information, I shut down that connection between me and the server
[81:31] and now somebody else can connect to the server instead. So think of it like an actual phone line
[81:35] where I call you on the phone, nobody else can call you until we hang up our phone call.
[81:40] Then people can call you and have that conversation. Yeah, there's no idea of call waiting here.
[81:45] - Kids these days, they don't know what they missed. - They're missing out on what that little beep
[81:50] in the background was. Or even back in the day, we didn't even have call waiting
[81:53] to get that beep. You just get a busy signal, right?
[81:55] - So TCP was only 65,000 connections per server, did you say? - Per server, yeah.
[82:03] - Okay. I don't know what it-- - And so, you know where--
[82:07] - Go ahead. - Sorry, go ahead. No, you go ahead.
[82:09] - I was like, TCP, I should look into that one time. - Yeah, so the idea with WebSockets and Webhooks then
[82:18] is you're holding that connection open long-term. So the benefit of REST is that as soon as that connection,
[82:25] or as soon as that communication is finished, you close that connection, which frees up a connection
[82:30] for somebody else. Where asynchronous, you're holding that connection open,
[82:35] which blocks somebody else from using that connection. And there are advanced ways that we're mitigating that
[82:44] and rotating things around. But at the end of the day, there are these limitations
[82:49] that are happening because of asynchronous. So there's, like I said, there's advantages and disadvantages
[82:56] to all of these technologies. - Okay, cool, yay.
[83:09] We've gone through a lot already. I'm kind of excited that I'm also still so far
[83:18] following along, so that's exciting. - That's good.
[83:23] So these are the two, like these are the two most popular kinds of APIs.
[83:28] REST by far is like a huge portion of the API market. When you're interacting with APIs,
[83:35] it's probably gonna be a RESTful API. But more and more, we're seeing a lot more
[83:39] of these Webhooks and WebSockets and whatever using this asynchronous API pattern of,
[83:46] let's hold that connection open a little bit longer so that you can send me data or I can stream data to you.
[83:52] And so it's holding that connection open a little bit longer so that we can stream data
[83:56] back and forth, which is a different sort of mechanism than what REST was meant to be a single transaction.
[84:04] So even though HTTP/2 is like, here's a bunch of things I want,
[84:07] you can send me back a bunch of things, it's still like one transaction
[84:09] and REST will still hang up at the end of that. With asynchronous, it's the same thing.
[84:13] If I make that WebSocket connection, I have to authenticate,
[84:16] but we're gonna hold that connection open for a period of time.
[84:19] But if that connection ever closes, I've got to reauthenticate again the next time I call
[84:23] because it's still using HTTP at the end of the day. So HTTP is stateless, it's kind of dumb.
[84:30] So I have to do that authentication every time, no matter what.
[84:33] And the people working on HTTP protocol, they're trying to find better ways
[84:39] and different ways of authentication. And how do we handle these things
[84:42] to make that a little bit easier, make it less chatty over the internet?
[84:45] Are there other sort of ways of doing this? So they're actually already working on an HTTP/3,
[84:50] even though HTTP/2 has only been out for a couple of years and isn't fully adopted,
[84:54] they're already working on HTTP/3 because they realized like,
[84:58] hey, even with the cool stuff that we introduced in version two,
[85:01] we can still do even better. And that's kind of the nice thing about tech
[85:05] is there's always something new to like go and learn and explore and see how things are being built and done.
[85:11] - Yes, I will say that is like one of my favorite things 'cause I will never learn,
[85:17] run out of topics for Teach Gen Tech ever. - Cool, so I do wanna back up a little bit
[85:23] so that we can talk about kind of these HTTP methods 'cause we really only talked about GET and POST.
[85:30] So GET was fetching data, POST is sending data, but there are a couple of different ways
[85:35] that we wanted to interact with data. And so this can even come into play a little bit
[85:40] with asynchronous API calls as well for how we wanna interact with the resources that we do.
[85:47] Because like I said, at the end of the day, these are all happening over HTTP.
[85:51] And so we have access to these HTTP methods to interact with the resources that we're trying to access.
[85:59] So we have GET and POST, and I wanna talk about three more.
[86:05] So we have DELETE, which says I want you to actually destroy
[86:12] some kind of resource. And again, you wanna make sure
[86:14] you've got good authentication in place because you wanna make sure that person's allowed
[86:19] to delete that blog post, or they're allowed to delete that image
[86:22] or something like that. - That's not scary at all.
[86:24] - Not scary at all, even a little. But there are security concerns around authentication
[86:31] and also what we call authorization. So authentication is who are you,
[86:35] authorization is what are you allowed to do. I could do a whole thing just on auth sometime.
[86:42] So we have authentication and authorization. And so if you ever hear somebody say auth,
[86:51] like just A-U-T-H, it's like, well, which, like, are you talking authentication
[86:55] or are you talking authorization? Because they're two different things.
[86:58] - Authentication is who are you. What can you do?
[87:06] - Authorization is your permission, basically. It's like, what are you permitted to do?
[87:10] And typically you would do authentication and then authorization.
[87:13] So now that I know who you are, what are you allowed to do?
[87:18] So with the delete operation, it's exactly what it sounds like.
[87:22] You're trying to delete or destroy some kind of content or resource.
[87:27] And so you have to make sure that you're properly authenticating
[87:30] like who the person is that's trying to delete something. And so nothing more really needs to be said on that one.
[87:37] The other two are a little bit analogous, but they are meant to be a little bit different.
[87:43] One is called put and another is called patch. Both of these are meant to change a resource
[87:51] in some varying amount. So a post is, I wanna go create a brand new blog post.
[87:58] And when you create that blog post, it would come back and say,
[88:01] okay, we've created post number five. When you do a put operation,
[88:07] you're basically saying like, hey, remember that blog post number five?
[88:10] I actually wanna change everything about it except for the ID value.
[88:13] I wanna change the title. I wanna change the body.
[88:15] I wanna change like everything that you're storing about that thing.
[88:18] So typically a put is saying, I wanna keep the ID the same,
[88:22] but I wanna change everything else about it. Where a patch is like,
[88:27] I just wanna change the title of the blog post. I just wanna tweak part of that resource.
[88:33] Where a put is like, I wanna keep the ID the same, but I wanna change everything about that thing
[88:37] other than the ID. So for example, a post operation could be,
[88:44] I wanna create a work outfit. So certain kind of pants, certain shirt, and so on.
[88:52] Maybe I'm going for a really corporate job. And so I've got really nice slacks and a button down shirt.
[88:56] Maybe I wear a tie. That's why I don't work at corporate entities
[89:00] 'cause I hate wearing a tie. And so, maybe I go work that corporate job
[89:05] for a little while and I'm like, okay, I'm gonna change my job.
[89:07] I'm gonna go hang out on in the stream and find out how to build a resume.
[89:10] And then I need to change everything about what I'm calling my work outfit
[89:15] to now I'm working at a startup so I can wear jeans and a hoodie.
[89:19] So I wanna change everything about it, but I still wanna call it work outfit.
[89:23] So the ID of this outfit is the same, but all of the content of that outfit is different
[89:31] because I'm changing everything about it. And so a put operation is I wanna change everything,
[89:37] but the ID stays the same. Where with a patch, a patch is like,
[89:43] I wanna change the sweater. Maybe it's not quite startup, it's not quite corporate,
[89:51] but kind of this large-ish kind of company. Maybe they're not really into hoodies.
[89:56] So maybe I'll wear like a button down shirt, but I'm still gonna wear jeans.
[90:00] I'm still gonna wear my sneakers, but maybe I'm gonna wear like a polo shirt
[90:03] or something instead of a hoodie. So put, we're still gonna call it a work outfit, but-
[90:10] - But we're changing everything about that outfit. New shirt, new pants, new shoes, new belt.
[90:16] Everything is different. So put is changing everything, but the ID.
[90:20] - Okay, let me, and hi, Ramon. I don't wanna forget to say hi.
[90:30] I hope we're still co-working tomorrow, Ramon. I really enjoy those.
[90:35] Okay, so put is... - Change everything about the output,
[90:42] but the name of the work outfit. Now, it's important to differentiate here
[90:51] that when we're calling it work outfit, that we're using that as the ID of the resource
[90:57] and that it's not just part of the resource itself. Like when we would talk about a blog title, for example,
[91:03] or like a blog post, the title is part of the blog post that gets stored in the database.
[91:09] But when we're talking here, like I need to go sort all of my outfits or something.
[91:15] So outfit number one is my work outfit. And so every time I interact with outfit number one,
[91:21] it's always gonna be my work outfit, that kind of thing. But maybe the name of it is like,
[91:26] maybe like the actual words work outfit is actually part of the resource itself.
[91:32] So I just wanna be clear here that when we're saying, I'm gonna go create an outfit,
[91:36] I'm calling it my work outfit. And then when I do a put on that resource,
[91:41] I'm changing everything about it, but I'm still referring to it as the same identifier.
[91:45] For the analogy of it, we're calling it a work outfit, but the actual text of the work outfit
[91:51] could be part of what we're storing in a database. - Okay, and Papa Smurf, hello, hello.
[91:56] Haven't seen you for a bit. I know my streams have been inconsistent.
[92:00] Update all resource attributes or fields based on ID. - So the put is saying,
[92:07] I wanna change everything about that work outfit, the shirt, the pants, the belt, the shoes,
[92:12] like everything about it is changing except for the identifier.
[92:16] Where the patch is saying, okay, well, now that I'm in my jeans
[92:20] and my band T-shirt and my hoodie, maybe a patch is like,
[92:26] okay, company would prefer that I didn't wear Marvel character T-shirts and a hoodie,
[92:33] so I'm gonna just change my shirt, but I'm still wearing my sneakers or my flip-flops,
[92:38] I'm still gonna wear my blue jeans, maybe wearing the beanie or the ball cap is still okay,
[92:44] but they want me to change my shirt. So I'm only gonna change part of my outfit,
[92:49] and that's where we would do a patch operation. Now, some people will use put and patch interoperably,
[92:58] and they'll say like, oh, either one is fine, they're both changing some amount of data,
[93:02] 'cause nothing really would stop you from a patch to say, I wanna change my pants and my belt and my shoes
[93:08] and my shirt and whatever I wear on my head. Nothing would stop a patch operation
[93:12] from actually changing everything in there, and then effectively it is a put.
[93:16] Where a put in its nature was meant to be, we really do wanna change all of the attributes
[93:22] except the ID, where the patch is like, oh, we only wanna tweak some of it,
[93:25] but nothing would stop a patch from changing all of those attributes.
[93:29] - And I put it in more gen terms of changing the lipstick color,
[93:35] 'cause that is what's gonna actually register, where if it's changing a shirt,
[93:41] then I'm like, is it a formal shirt or is it an unformal? How is that not in the outfit reference?
[93:48] - Yeah, so kind of the analogy I was using is like, if my original work outfit was corporate
[93:53] where I'm wearing a suit and tie, where my next job, I'm still calling it work outfit,
[93:59] but now I'm working at a startup, so I'm gonna go to jeans and a hoodie
[94:03] and like a beanie or something, but then maybe I need to change it again
[94:06] 'cause they don't want me to wear a hoodie and a beanie, but it's still okay to wear jeans and sneakers,
[94:12] but they want like a button down shirt instead. So that would be a patch operation
[94:14] where you're changing part of your outfit, but not changing everything about it.
[94:19] - I like what you said, Papa Smurf. (mouse clicking)
[94:26] Resource, attributes. Cool.
[94:42] And I'm gonna put it by Papa Smurf. (mouse clicking)
[94:55] Which works out because I am using blue. It's not quite Smurf blue, but hey, we're close.
[95:02] So this is making a lot of sense. And I love that Ramon is here, was here,
[95:08] because that was the first API that I built on stream. - Nice.
[95:13] - Way back in the day, we did it. If Ramon's here, hopefully he'll correct me.
[95:19] I believe we did it on ExpressJS. Wait, why am I suddenly, is Express a thing?
[95:27] For some reason, I haven't said ExpressJS in a really long time.
[95:30] - Express is the backend framework for Node.js that actually builds out an API in JavaScript.
[95:35] - Okay, why did I forget that? That's a thing.
[95:40] Yeah, I haven't used that term in a while. All right, cool.
[95:46] - So a post sends and creates, or and/or. - A post is meant to create a resource.
[95:54] So with a post operation, you're not gonna send an ID. It's up to the server to assign an ID.
[96:03] It's very, very atypical. It's not a typical thing for you to try to create something
[96:12] and give it an identifier at the same time, because that identifier might already exist.
[96:17] And so if I was connecting to an API to say, "Go store this blog post,"
[96:22] I would say, "Here's the title, here's the content, "here's other metadata about it."
[96:26] And then it would be up to the server to tell me, "Okay, that's blog post number 12."
[96:30] And then I can interact with blog post number 12 with a put or a patch to say, "I wanna update the title,"
[96:37] or, "I need to fix a typo in the content," or something like that.
[96:40] Or, "You know what? "I wanna delete that one completely."
[96:43] And I just delete blog 12 where the create, you're creating everything but the ID.
[96:51] And so you're creating something and the ID is assigned to you.
[96:54] And then I would say on the post, yeah, create a content and get an ID,
[97:06] 'cause that's a typical thing that would happen with an API. You're gonna create something
[97:10] and you're gonna get an ID back. - But you get an ID back with your get or just like--
[97:17] - No, with a post, with a post. - Okay, cool.
[97:20] And I'm just gonna say create content and receive ID. I'm like, if I use the word get, I'm gonna get confused.
[97:31] - So with a get operation now, we've got two additional ways of doing a get
[97:38] where we can say, "Go get me all my blog posts," or, "Give me like a paginated list of my blog posts,"
[97:42] or, "I want to get blog post number 12." So with a get, depending on the path,
[97:48] you can say /blog and that'll get all your blogs or you can say /blog/12,
[97:52] and that'll give you just that one resource. So depending on what you're telling the server
[97:57] you want to get, it's up to the server to determine and up to the API to determine,
[98:01] am I giving you back one thing? Am I supposed to give you back a list of things?
[98:05] And so along with kind of this idea of REST and what a RESTful API is,
[98:11] if you're calling a resource without an identifier, you're generally asking for a list of things to come back.
[98:18] So if I say, "Go get/blog," I'm typically going to be asking for a list of blog posts,
[98:25] where if I say, "Go get/blog/12," I want just that one blog post.
[98:31] So if I had a library and I do get/books, I should get a list of books.
[98:36] But if I say, "Get/books/12," I should get just book number 12.
[98:42] So with REST, if you provide an ID, you're getting one thing,
[98:47] or you're interacting with one thing. If you're interacting with a resource
[98:53] where it's just kind of the name of the resource and not a specific one of those resources,
[98:59] then you're generally saying, "I want to go get all of them,"
[99:02] or "I want to create a new one of them." So with a GET and a POST, you would call /blogs,
[99:10] where a GET is going to get you all the blog posts. Doing a POST to /blogs would create a new POST.
[99:16] But if you give it an ID value, then you're saying,
[99:21] "I want to interact with that one specific ID." Papa Smurf also said in chat,
[99:34] "Some web frameworks will send patch rather than put, but if they do, you probably don't need to worry about it."
[99:40] Yeah, I agree. So again, with patch,
[99:43] there's nothing stopping a patch from updating all of those attributes,
[99:46] but a put is generally meant that you want to change all of those attributes
[99:51] other than the ID. - Oh, goodness, okay.
[99:55] What y'all are saying makes sense. It's just also at the same time,
[100:00] I'm just like, "Okay, I'm gonna get there. I will get there."
[100:05] - So let's wrap up with this. Let's go, I'm gonna share my screen,
[100:09] if you want to activate my screen. What I'll do is I'll show you in Postman,
[100:16] 'cause I work at Postman, for those that don't know me. And Postman is just a way
[100:20] that we can kind of interact with an API. So this API is just something I've got local,
[100:24] and it's a little to-do list application. And so I've got this endpoint called /notes,
[100:30] which is just my to-do list. And inside the body here,
[100:35] I'm gonna have a title with some content and whether that thing is completed or not.
[100:38] So this is the information that I'm sending. So when I do a post operation to /notes,
[100:46] with a RESTful API, I'm saying, "I wanna go create one of this kind of resource."
[100:51] So notes is a type of resource on my API. So I'm saying, "I wanna go create a note."
[100:57] - Okay. - And so when you do a post to a resource name,
[101:03] I'm not saying I wanna go post to notes six, because that's not valid,
[101:09] because I can't create number six. It's up to the software, the API,
[101:15] or whatever to assign that ID. So I'm gonna say, "Okay, I wanna go walk my dog,
[101:19] and I'm gonna send that over to the server." And the response that I get back here says,
[101:24] "Okay, I gave that ID number one." It was for user number one,
[101:31] and here's all the content and whatever. So the server is giving me a little bit more context
[101:35] about what it created on my behalf. And so it assigned an ID value back to me here.
[101:41] - Okay. - So now I can use that ID value
[101:45] for all of these other methods. I can patch it, I can delete it,
[101:48] I can fetch one of them, or I can say, "Go get all of my notes."
[101:52] So when we were talking about get and post on /notes, this is where I would say, "I wanna go get /notes."
[102:01] Now I should get back a list of all of my notes. So if I send this over,
[102:06] we see this comes back as an array of objects here. If you understand JSON,
[102:11] the square bracket means you're getting back a list of something.
[102:15] And so when I say, "Go get /notes," it's saying, "Oh, you want a list of things."
[102:19] Even though I've only got one thing in here, it's still giving me a list of all of the notes
[102:24] that I have on the system right now. That actually might cause us to go onto a tangent
[102:33] yet at the same time. I feel like it's a little important.
[102:37] I can get what, at least conceptually, when somebody says an XML or regular text,
[102:48] I'm like, "Cool, XML." I can visualize it at least enough
[102:53] because you can open it in Excel. So it does do some things.
[102:58] Like it's a little easier to visualize. Where when somebody says JSON, I'm like, or YAML,
[103:07] I'm like, "Those are things? Yeah, those are things.
[103:10] Those do exist. I know they do.
[103:14] And I know they go to APIs. Other than that, I have no idea what they are."
[103:18] Is this a good- - That's a whole other topic.
[103:22] - Bananas. - I'll give you like the five,
[103:28] well, I'll give you like a 30-second intro. So JSON, do you know what JSON stands for?
[103:33] - Isn't it JavaScript- - Object notation.
[103:40] Yeah, and so this would be a way of defining an object in JavaScript.
[103:46] Basically saying I've got an object. That's what the curly braces are sort of wrapping.
[103:50] And inside of that, I have an attribute called data. And inside of that, like that attributes value is an array.
[103:58] That array is an array of JavaScript objects. And that object has an attribute called ID,
[104:06] user ID, title, content, and so on. And so JSON is just a way of structuring data
[104:12] that you can pull it into JavaScript. And actually now you've got actual JavaScript objects.
[104:17] So it's just a text representation of what a JavaScript object is under the hood.
[104:23] But we as a community, we kind of adopted that going, oh, that's actually really easy to read compared to XML
[104:29] and compared to other things that were a lot more verbose. JSON is a much more compact amount of data that we send
[104:38] at the expense of losing identification around, well, this field can only be an integer.
[104:44] This field can only be a string or this field could be a string or an integer.
[104:48] JSON doesn't have the idea of data types. And so you can't say like,
[104:53] oh, this field has to be an integer where XML can define those kinds of things.
[104:58] - I'm literally writing to like ask, so Josh Goldberg who wrote "Learning TypeScript"
[105:06] comes on my show every other week. And I was literally writing,
[105:09] asked about JSON versus TypeScript. And you just said it, JSON does not assign data types.
[105:17] - Yeah, well, TypeScript and JSON are two different things. So JSON is just a way of expressing an object
[105:26] modeled in just text that we as humans can read. And so now, so the idea that we're kind of coming to here
[105:36] in Postman was when we do a GET or a POST on just the name of the resource,
[105:42] when we do a POST we're saying, I wanna create one of those resources.
[105:45] When we do a GET on that resource name, we're typically in a RESTful API.
[105:50] We're saying, I wanna go get a list of all of those resources.
[105:53] So now that I got, I know that I've got an ID of one, now I can go in and I can change, I can fetch that one.
[106:01] I can say, go get note number one. And when I send this over,
[106:05] it kind of looks like the last payload that we got, but this is only a single object.
[106:09] It's not an array of these objects. 'Cause I said, I wanna go get that one resource.
[106:14] So if we give it an ID as part of that path, what REST is saying is I wanna go get that one resource.
[106:21] And then it gives me back that one resource. Same thing, I can do a patch where I can say,
[106:28] okay, well, I wanna change this up. I can't change the ID, that's invalid,
[106:34] but maybe instead of saying, walk the dog, I wanna change the title to say, I wanna feed the dog
[106:40] and maybe I have completed that. And so I can change that value to true
[106:44] and I can send that over. Can't change that, I wasn't trying to change the ID.
[106:49] Okay, something broke on my software, but if I were to go back and fetch that one,
[106:55] it would have changed the title to like feed the dog and completed would have been true.
[107:00] So I've got a bug in my software apparently though, I'll go fix.
[107:03] But the patch, because we're giving the patch an ID value, it's saying, I wanna go change this one resource.
[107:10] Now it's not a typical RESTful endpoint say, I wanna go patch all of the things.
[107:16] That would typically be an invalid kind of instruction because I wouldn't necessarily have access to say,
[107:23] go change everything in the database to go change all of the titles
[107:27] 'cause you wouldn't wanna change all the titles to one thing.
[107:29] You wouldn't wanna change the completed status to all be false.
[107:33] You would wanna go through those methodically and say, go get a list of all those resources
[107:36] and then iterate over that and change the flags or change the titles appropriately.
[107:40] And then I can go in and I can delete that one note. So this comes back with nothing,
[107:46] but the status code here of 204 basically indicates that worked,
[107:50] but it had nothing more to tell me about that. So now if I try to go get all of my notes,
[107:56] it comes back as an empty list because I said, I wanna go delete that one resource.
[108:00] So when I do a get or a post on the resource name only, I'm saying I either wanna create that resource
[108:07] or I wanna get a list of all of those resources. But if I give it an ID value, like slash one,
[108:14] I'm saying, go get me that one resource. Now, if I try to go fetch this, I get a 404.
[108:18] Well, again, with a software, I need to be able to tell it to send me back a 404,
[108:23] but typically this will come back with a 404 saying, I don't have that resource.
[108:27] Or if I'm not authorized to see it, I might still give back a 404 going,
[108:32] I don't know what you're talking about, dude. Where if I say,
[108:34] oh, you're not allowed to see resource number one. It's like, oh, there is a resource number one.
[108:38] Let me try and hack into your system because I know that there's something there
[108:41] 'cause you just told me I'm not allowed to access it. And so a better security way of writing an API
[108:47] if somebody tries to access something they're not authorized to,
[108:51] is to give them back a 404 saying, I don't know what you're talking about,
[108:54] that doesn't exist here. And then I'm less likely to try to break in and say,
[108:59] well, I'm sure there must be an ID of one. So yeah, there are security implications
[109:05] about how to build APIs and so on. But I wanted to kind of show,
[109:07] like these are those five methods you've got to get to put in a patch, like we said, are kind of analogous.
[109:14] And then we've got the delete. But in this case, I wanted to show the difference
[109:17] between fetching one of something or just saying fetch all of something.
[109:21] There is a little bit of a different flavor on this. And this is where, you know,
[109:26] everybody that writes an API does it a little bit differently.
[109:30] Here's a dad joke API where I can just call this API and it's gonna go fetch a single dad joke.
[109:36] But I'm not saying which dad joke to get. I'm just saying, go get me a dad joke.
[109:42] And so in this case, I'm, you know, this might be better where I had like,
[109:47] go get jokes, you know, sample, you know, where I pass in like a size of one or something like that.
[109:53] Like that might be a better restful path where I'm saying this is what I wanna go get
[109:58] as opposed to just go call the domain name because now it's up to the software to go,
[110:02] oh, you're hitting the domain name. You only want one joke.
[110:05] So it's not as flexible, but this would be a way of, you know,
[110:10] a different way of writing a restful API where I do a get operation on this endpoint
[110:14] and I get one joke coming back. But a better restful path would be something like,
[110:20] I wanna go get a jokes resource and I wanna get a sample of that.
[110:25] And that sample size is gonna be like one joke or maybe I wanna get back five dad jokes or something.
[110:30] That would be a better way of structuring that restful path.
[110:35] But again, this is where as programmers, we wanted the flexibility of being able to write these APIs
[110:40] any way that we wanted to. But for the end user, it's like, well,
[110:43] but my expectation, if I call that endpoint, I should have gotten back like a whole bunch of stuff.
[110:48] And so it can create confusion for people that are trying to actually go use APIs
[110:53] for like, how do I use your API? Because yours is gonna be different from their API.
[110:57] And it's gonna be different from their API because we don't rigidly follow restful practices
[111:02] on how these things should work. So yeah, anyway, Postman will also work
[111:07] with asynchronous APIs. You can open up web sockets
[111:10] and watch data transfer back and forth and so on and so on.
[111:13] - Really quick y'all, I'm gonna be right back. I need to use my inhaler really quick.
[111:22] - Yeah, no worries. If anybody's got questions about APIs
[111:27] or anything like that, feel free to drop it. So yeah, Papa Smith,
[111:31] I've been working at Postman for a little over a year. I started last January
[111:35] and I have a blast. I'm on the developer relations team over there.
[111:38] So I get to do all kinds of really fun like workshops and tech conferences and videos and blog posts
[111:44] and all kinds of content around API education. And I actually met Jen at a local Denver area API meetup
[111:53] and we got chatting. She's like, I would love to learn more about APIs.
[111:57] So I'm like, why don't I come on your stream and we'll chat about APIs.
[112:00] So we kind of coordinated a little bit on what we're gonna talk about.
[112:04] And there's like so much more we could get into with different kinds of APIs and so on.
[112:09] But yeah, good to see everybody. So at the very beginning of the session,
[112:13] we were talking about like how APIs kind of run the world right now.
[112:16] Like there's so many things that we control over APIs. Like pretty much everything on your phone
[112:21] is gonna be communicating over these kinds of APIs. Maybe not for getting dad jokes,
[112:27] but for like fetching the weather and things like that. These all interact over APIs.
[112:31] Like all these lights I have in the background, those all connect with an API
[112:35] where I make an API call saying, go get the identifier for each one
[112:39] of those individual light panels and then go set all these random lights
[112:42] so I can hit a button. And it makes them all blink and flash
[112:45] because software's fast to actually go interact with those APIs to go make all those lights appear to blink
[112:53] when really it's just sending random patterns of like turn this light on or off.
[112:57] And if it's on, set it to this random color and then wait half a second and do it again.
[113:04] And then do that like a bunch of times. And so we use these APIs to interact
[113:08] with a lot of different things in the world. So like your smartwatch, your phone,
[113:14] those are all using APIs for things like banking, email, calendars, notification events,
[113:19] like all those are happening over APIs. - And thank you.
[113:23] I will say this is a perk of, you know, when you have another streamer on your show,
[113:30] they just can like handle themselves if you disappear for some reason.
[113:34] I will say, I am very, very surprised that after like 80 plus streams,
[113:40] that is the first time I've had any asthma issues on stream. But it was because I started like choking on something,
[113:47] which made me cough, which made my asthma. And I was like, I'm not gonna be able.
[113:52] So thank you. - I thought I was just getting you really worked up
[113:55] about APIs, that's all. - Well, I am really excited about APIs
[113:59] because it was something that is very difficult for people to explain in very basic terms.
[114:08] This is a lot of tech in general is it's difficult to explain the high level.
[114:14] And I know, especially for those who are very, very technical,
[114:19] which I get because you're like, I don't know, like you just do the thing.
[114:24] And this is why I do really appreciate you coming on the show because it's like, for myself, at least,
[114:32] if I don't understand all the things that the theory behind it,
[114:37] it makes it really difficult for me to actually implement what I'm doing.
[114:41] Where other people are just like, oh, this works with this, cool.
[114:45] I'm like, okay. - Or it tends to be like, go do this, go do this,
[114:48] go do this, and it magically works, but you don't understand the why.
[114:51] Like, how does that actually work? So that's why I wanted to kind of go into like HTTP
[114:54] and talk about these different kinds of protocols, like B1 mindset, coming back to modern web,
[114:59] I thought all APIs were REST APIs. I mean, most of them are.
[115:03] Like most of the APIs that you interact with are going to be RESTful APIs,
[115:06] but we're seeing a bigger shift into the asynchronous APIs where we're getting into web hooks and web sockets
[115:12] because we can have more of that interactive kind of thing where there's less chatter over the internet
[115:17] of constantly like, hey, Jen, are those cookies done yet? Are they done yet?
[115:21] Are they done yet? Now, you know, I'm still waiting for those cookies.
[115:24] Like I don't have to pull the server over and over and over again,
[115:28] waiting for a response that says, you know, some task that I gave it is finished.
[115:33] And so we're starting to see a lot more asynchronous APIs happening.
[115:37] And they've actually been supported for a number of years in browsers to actually connect over HTTP/2
[115:43] for web socket connections. That's actually been around for a while.
[115:46] We can build REST APIs on HTTP/2, but it's less common.
[115:51] REST is still kind of in the 1.1 version of HTTP where it's like single request, single response,
[115:57] because that was kind of the nature of REST. It was meant to be, hey, I want to interact
[116:03] in a single way with a single response or a single request. And I get a single response telling me
[116:08] whether it worked or not, and that's all I need. So I don't know if REST is ever
[116:12] actually going to move to HTTP/2. There aren't any real strong advantages
[116:16] to moving REST to HTTP. I mean, there are some things about the protocol
[116:20] that would make it a little bit faster, but there's not like a big like,
[116:27] oh yeah, if we moved HTTP/2, REST is going to be like a gazillion times better
[116:31] because it would mean changing a lot about what REST is, and it would actually shift more
[116:37] into what we're already doing with asynchronous APIs. So I have a feeling that REST APIs
[116:41] are going to kind of linger on like older versions of HTTP for a while, where all the asynchronous stuff
[116:47] and the more performance types of APIs are getting into HTTP/2 and starting development on HTTP/3.
[116:55] But yeah, going back to like what we talked about at the very beginning of the stream,
[117:00] gosh, it has been two hours. - Yeah, I was like, I'm writing notes
[117:04] to bug you about later. - Yeah, no worries.
[117:06] Is the whole idea of abstraction, like we use APIs to abstract like,
[117:09] hey, I need to go do a thing. I need to go perform some kind of operation.
[117:14] It's not like I know all the different steps to go store that blog post in the database.
[117:18] So I just need to go tell a server like, hey, here's some details about a blog post.
[117:22] Can you store that, please? And the server's like, yeah, I got you, fam.
[117:26] Like, no problem. We got that handled.
[117:28] And it's kind of the same thing when we write code in JavaScript or Python.
[117:31] We're just saying like, hey, I need an array of strings. We're not in there manually manipulating the memory
[117:37] and like telling the CPU how to talk to the RAM. Like it's all abstraction at the end of the day,
[117:42] whether we're talking to an API, like a weather API or a dad joke API,
[117:47] or whether we're using our programming languages API, it's all an abstraction for, I want to go do a thing.
[117:54] And something else knows kind of the underlying instructions of how to actually make that happen
[117:58] and then return back a success or a failure. - Oh my goodness, me and my coffee.
[118:04] I will say like just future things I'm curious about, of course, is like digging in deeper to this
[118:12] and something that I know that I'll be working on and a big reason y'all that timing just happened
[118:20] to be really great of, since I've been learning Postgres is I'm going to need to set it up on my website.
[118:29] And that's gonna involve working with something like Prisma, which will then need an API to be able to do all of that.
[118:37] So this is great timing, as well as really starting to understand
[118:43] where we use APIs is something that I'm very, very grateful for,
[118:49] because I like, I know that they connect everything, but actually being able to see them in action
[118:55] is something new to me in the future. And this is something that I completely forgot about
[119:02] until you were the very end. Soap versus rest, because I'll,
[119:10] that's what I hear a lot about, which is interesting because it's,
[119:14] you also said asynchronous, which cool. Events streaming, because that seems to be all the rage.
[119:24] And I'm like, okay, cool. Which events streaming is just asynchronous, right?
[119:35] - It tends to be, yeah. - Okay, JSON and XML in more detail,
[119:42] and TCP, which none of the, at any or all of these might be a you questions,
[119:51] or just in general, I need to find somebody to talk to me about them.
[119:55] Those are- - So I can cover SOAP in 30 seconds or less.
[119:59] - Ooh, yay. So SOAP actually stands for Simple Object Access Protocol.
[120:06] So you're still interacting with a single resource. So you're saying, I wanna go manipulate a simple object.
[120:14] So you're interacting with an object, but they wanted to call it like,
[120:19] we're gonna call it the simple protocol. And so it's a simple object access protocol.
[120:25] And when it was created, it was pretty much primarily only using XML.
[120:33] XML looks a lot like HTML. It's still a markup language,
[120:37] where XML is a very verbose structure of the data where you're defining fields
[120:43] and what data types they can have. And if it's a number, what range can that number be?
[120:49] But it made it very, very verbose. And so even sending back like,
[120:54] here's my to-do list with go walk the dog and so on, and whether it's completed or not,
[121:00] might be 10 times as much content actually being transferred back.
[121:05] Well, back in the day when SOAP started, like SOAP has been around for quite a while,
[121:10] it started in sometime in the late '90s. I wanna say like '97, '98 maybe,
[121:17] where REST kind of came into play like shortly after that, 'cause people are like,
[121:21] "Surely we can do better than SOAP." But SOAP is still around.
[121:26] Even Salesforce, folks that are familiar with Salesforce, even Salesforce APIs were on SOAP for the longest time.
[121:33] - Interesting. - But doing things over XML,
[121:38] because it was so much information, so much content, what we didn't have back in the day
[121:42] was a way to compress that data before we transferred it to a server.
[121:46] Where now browsers, if you ever look at the user agent string
[121:49] of like what identifies your browser, you'll see the letters GZ or GZIP,
[121:55] and that's basically saying like, "Hey, while we're talking,
[121:58] "like while we got this communication channel open, "by the way, I can compress this data.
[122:02] "Can you also compress data when you send it back?" And so it actually crunches that data down a little bit
[122:07] in transit. And so we're not sending these massive gluts of text anymore.
[122:11] They do get compressed. But XML compressed is still larger than compressed JSON,
[122:17] because JSON just takes up less room overall. And so XML is still a very verbose way of explaining things,
[122:25] kind of over explains things, but there are benefits to it as well.
[122:29] Like the data typing of this field can only be an integer from one to 10.
[122:34] And this field has to be a Boolean and it can only be true or false.
[122:37] And if it's not set, we're gonna default it to false and things like that.
[122:41] Like XML is a very descriptive kind of markdown where JSON is just like,
[122:46] "Here's a field, it's set to false. "Hope that's good with you."
[122:49] And then it's up to the server to actually validate that what the user sent over actually validates properly
[122:55] of like, "Wait, you sent me a one. "It's supposed to be a Boolean.
[122:58] "Am I supposed to interpret that as a true, "like a one or a zero?
[123:02] "Or did you accidentally send me an integer?" And so there ends up being a lot more confusion
[123:07] about actually sending the right kinds of data over JSON. There are binary versions of JSON called BSON.
[123:16] It's a binary structure of that. And then there are other mechanisms
[123:21] that can use like binary payloads of data and different kinds of APIs
[123:25] that actually maintain that data type. But SOAP back in the day was just XML
[123:31] and it was a very, very verbose. And so a lot of people just once REST kind of came out,
[123:36] they're like, "Okay, we don't need to use SOAP anymore." And so SOAP quickly fell off by 2005,
[123:41] like very few APIs were SOAP anymore. And then it still took like another decade
[123:45] for most of the other SOAP APIs to go away, but they're still out there and they still use XML.
[123:52] But SOAP was one of the first ways of actually interacting over the internet
[123:56] 'cause the internet was still relatively new back then. The internet really only came around like '93, '94,
[124:04] as far as like a public internet, 'cause that's kind of when HTML started being invented,
[124:09] was around '93, '94. And then SOAP kind of came in to play around like,
[124:14] "Hey, can we just get the computers to talk where it's not everything has to happen through a browser?"
[124:18] And so that's where SOAP kind of came to be. And then SOAP got kind of overtaken by REST.
[124:25] REST is now still very, very dominant, but we're starting to see like Webhooks and WebSockets
[124:31] kind of like catch up a little bit, but not nearly as much. And then we're seeing other kinds of APIs
[124:36] that are like gRPC and so on that are more performant. They're faster at doing their things,
[124:41] but that's a whole other... That's where you're getting into like performance tuning
[124:47] of like, "I need the fastest possible way of like sending this data."
[124:51] - Yeah, I wrote it down. That is something that I'm...
[124:54] I'm running. So, oh, I just double wrote it, whatever.
[125:02] But gRPC and like finding out more about that and like event streaming and those things specifically
[125:10] would be interesting to learn about. I think those are also more of my own curiosity
[125:17] because companies I've worked for use those terms a lot and I never understood them.
[125:24] That has driven a lot of my curiosity. - Yeah, knowing how to interact with Webhooks
[125:30] is actually a really cool part of being in programming these days
[125:34] because it does get into that event-driven architecture and the event-driven kind of internet of,
[125:40] "Hey, a thing happened. I'm gonna let you know where you don't have to call me
[125:43] and find out if those cookies are done. I'm just gonna let you know
[125:45] when the cookies are finished baking." And so it allows for a lot more flexibility
[125:50] and power around like when things actually happen, you get notified instead of having to go request
[125:57] whether something is finished or not. So it allows for a lot more kind of cool things
[126:03] to happen on the internet. But like we said, there are disadvantages too
[126:07] of like holding those connections open and that means maybe other people
[126:10] can't connect to that server. So now as the service, as Facebook or Twitter,
[126:14] now I need even more servers, which uses more electricity
[126:18] and more resources from the planet and, you know. - There's a lot that goes into it.
[126:23] - That's a whole other soapbox. That's a whole other soapbox we can get into.
[126:26] But yeah, there's a ton that goes into it that a lot of people don't really understand
[126:30] like how the internet actually works and how these things communicate.
[126:33] But the starting point is like the internet kind of runs on APIs
[126:38] and knowing how these things actually work is good. And I think from here,
[126:42] we could start to go down a lower level and start getting into like,
[126:45] how are these things actually transmitting over the wires? And like, how does that actually route around the internet?
[126:50] What if my ISP goes down or what if whatever it connects to goes down?
[126:55] Is there still a way that I can get that data if something breaks on the internet?
[127:00] - Yeah, that's a big thing that I'm definitely looking forward to as well.
[127:06] So y'all, I just gave Ian a shout out on the channel. Go make sure you follow his Twitch as well.
[127:14] And thank you, Ron, for the follow. I appreciate it.
[127:18] We definitely have gone through a lot. I'm kind of like, I'm totally wrapping things up.
[127:24] Sometimes I'm a little awkward about it. And I say that because I'm starting to get mushy brain
[127:28] where I'm like, you're saying things and I'm curious but they're not computing as well.
[127:33] And this is what I like to call like mushy brain or I'm just like hit my saturation,
[127:38] whatever you want to call it. Everyone go bug Ian to be back on the show
[127:44] because there is a lot we have left to learn. - You don't have to bug me to come on this show.
[127:49] - Yay. And then also make sure to go hit them up
[127:54] on Twitter and LinkedIn, especially for anyone looking for work.
[128:00] Like I honestly, especially in the tech field, Ian is so good at resumes and helping with job searches
[128:08] and teaching about all of this. And you're gonna ask really interesting questions
[128:13] or when it doesn't click, he's very kind about it. I say that as coming from someone that did do that.
[128:19] So, and thank you again. Ian, anything you want to say before we,
[128:26] I go read them to somebody. Albedo is saying links.
[128:30] - Links, yeah, I'll drop some links. So I tend to use Ian Douglas 736 on all platforms.
[128:38] So like Twitter, Twitch, Instagram, Linktree. I use the same username on all those.
[128:45] - Yeah. - Yeah, except my YouTube channel.
[128:47] My YouTube channel is just Ian Douglas. And I've got a lot of like free videos.
[128:53] You can go to iandouglas.llc as a website and that'll kind of branch you off
[128:56] on all the different things that I do. Like the live stream and the 3D printing stuff.
[129:01] And all that kind of stuff, that's all through there. The techinterview.guide, all my career advice, it's all free.
[129:07] I've got newsletters you can sign up for on there, all that kind of stuff.
[129:10] So go check out iandouglas.llc as a website. And you can go find me
[129:16] on all the different platforms from there. But yeah, it's all free.
[129:19] So there's no paywalls. The only thing that you would ever need to register for
[129:23] is like the newsletters. If you want to get tech newsletters
[129:25] about like how to get ready for interviews and why we ask the kinds of questions
[129:30] that we do in interviews. I kind of approach it from a hiring manager's mind.
[129:34] But yeah, I'll be streaming in about five hours. I'm going to do some live coding tonight using APIs.
[129:40] We're going to be building some chatbot stuff. So feel free to drop by the live stream
[129:44] if you want to hang out and nerd out some more. If you've got questions about other stuff,
[129:48] I love taking questions on the chat, so. - Yes, and definitely, again, y'all follow both of us.
[129:54] I go through mostly like new tech as I'm learning and developing, I bring everyone with me.
[129:59] It's not always with a guest, even though sometimes I like it more with guests
[130:03] because then it's like, they are, you know, they can help coach me through it,
[130:08] where when I'm streaming by myself, I get stuck and then I get really frustrated.
[130:12] But luckily, there's been some amazing people in the crowd when I've been learning Postgres.
[130:16] So thank you, everyone. And let's go raid Chris.
[130:23] See, Griffin, really dope human, always. I believe he might be working on something new.
[130:32] It always takes a few minutes for the raid to go through. So thank you again, everyone.
[130:37] And this video will be posted later this week on YouTube and will be shared out too.
[130:44] Bye. - See ya.
[130:47] [BLANK_AUDIO] 
