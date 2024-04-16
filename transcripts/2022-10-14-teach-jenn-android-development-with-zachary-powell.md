---
showLink: "https://www.youtube.com/watch?v=TL4xVhz83nA"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-android-development-with-zachary-powell"
title: "Teach Jenn Android Development with Zachary Powell"
publishDate: "2022-10-14"
coverImage: "https://i.ytimg.com/vi/TL4xVhz83nA/maxresdefault.jpg"
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

[00:00] - Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:06] And today we have Zachary here, yay. Thank you for joining us.
[00:11] And Zachary, please introduce yourself and what you'll be teaching us today.
[00:15] - Sure, yeah, hi, everyone. So I am, well, where to start?
[00:21] I've been an Android developer for about 10 years. It's probably the easiest way to sum it up.
[00:26] In a more recent life, I was an Android developer advocate and I'm actually now a manager in developer relations.
[00:34] So I kind of split my time between being someone that advocates for developer relations in general
[00:40] and managing people, and then also someone who absolutely loves Android and continues to try
[00:45] and be an Android developer in what little free time they have.
[00:49] That's kind of me. - That's a good explanation.
[00:53] And I'm excited because I've been, and so the last two weeks,
[00:59] everybody has definitely heard me complain about being back on a Windows machine
[01:04] because I was running to a live stream and I had my laptop in my arm and a cup of water
[01:12] and I ran into a door. Like the door just like, I wasn't spatial,
[01:17] whereas it just didn't work. And I ran into it and it spilled water and fried everything
[01:22] like right before my live stream. So I had to cancel it.
[01:26] And luckily my partner has a Windows laptop. He wasn't, he doesn't use for work.
[01:31] So I have that to use and I was like, I can't do it. I love all Apple and Mac things.
[01:37] It just, my brain does not function like this. And I bring that up because in my journey
[01:44] of like understanding OSS and open source and also talking about it and realizing,
[01:53] and I think in fact it was like a conversation with, it was a conversation with you or BDougie
[01:58] that was like, oh my gosh, I've been talking about open source way longer
[02:03] than I knew what open source was because in, yeah, it was probably 2007 when Androids and iPhones,
[02:12] 2008, Androids and iPhones started really coming out. I worked at Verizon mobile company here in the States
[02:19] and everyone, I remember the first Motorola that came out, it was like a slide up and had a full keyboard
[02:26] and I absolutely loved it. And it was like, yet I kept crashing it
[02:32] because the apps didn't always play nice with each other. Then we got iPhones and what up, Ryan?
[02:40] Then we got iPhones. And so I was like, what's the difference?
[02:44] I learned it's, I would say closed sourced, that's how I explained it.
[02:48] And I was, and I just was like every, to explain it to a customer,
[02:54] Android is where it was so customizable, you can change everything,
[02:59] you can really make it what you want, yet there's no guarantee that all the apps
[03:03] will get along together. And then you have an iPhone where you can't customize
[03:09] a ton of it unless you jailbreak it. And yet it's gonna be much more reliable
[03:16] because you can't customize it that much and it just comes as it is.
[03:21] And it was ever since that, that I've never turned back to go back to Android
[03:29] or Windows, they are not the same everyone. So please know, I'm not saying they are the same thing.
[03:35] They're just much more customizable and not Apple that I associate them together.
[03:42] But I loved Android in the fact of so much of it was customizable and it was a lot easier
[03:51] to do a lot of things, change things. From my memory of them and also like a lot of my friends
[03:57] and family have them is, it also made it a lot easier to customize the,
[04:06] like, what are they called? Like the, on the homepages,
[04:11] but they are like the bigger versions of them. - Widgets.
[04:14] - Widgets, thank you, widgets. iPhones didn't have widgets for a really long time.
[04:20] (laughs) And Ryan is looking forward to your call,
[04:25] a chat on Tuesday, yay. - I'm assuming that's a coffee tech chat.
[04:31] - Nice, nice, I'm excited. - Continue to do those, that's very good.
[04:36] But yeah, no, you're completely right. You're completely right on Android
[04:40] basically being the open source mobile operating system. And I think today really what I want to do is kind of,
[04:49] when we talk about Android development and being an Android dev,
[04:52] most people associate that with being an app developer for Android.
[04:57] But I'd like to kind of go through the other side of it first today,
[05:00] which is actually looking at the operating system, actually looking at what Android is
[05:03] and how you might develop in the operating system, how you might actually customize the operating system.
[05:10] That's something that I did for many years and it's kind of not something
[05:13] that so many people have exposure to. So I think it would be quite fun to look at.
[05:17] After that though, I think we then should look at the Android app side of the world.
[05:22] And I know that we've got another live stream in the future where we will actually
[05:26] then build an app as well. So I think hopefully by the end of this,
[05:31] at the end of today, you'll have kind of an idea of where we're going.
[05:34] And then next time we can kind of really dig into building something fun.
[05:38] - Everyone can probably see that the light is changing. So I'm totally looking up something at the same time
[05:48] of the versions because I'm trying to see what version I got to before.
[05:58] Yeah, I stopped working at Verizon by the time it got to Froyo.
[06:06] - Oh, okay. Yeah, so quite early on.
[06:09] - It sounds like your mic might be doing something. Kind of.
[06:13] Ryan, do you hear that too? I'm just, I don't know if it's like my headphones
[06:20] or something. It just sounds like it's like a weird connection.
[06:27] - Hmm, it might be something interfering. - Oh, that fixed it.
[06:33] Whatever you just did so far. Yeah, it sounds like clicking.
[06:37] Yeah, so far you sound great. - Yeah, I think I had a phone too close to my microphone.
[06:44] I was probably trying to get a text or something. I'm gonna move my many mobiles out of the way.
[06:49] - Yeah, it was, I mean, I might've been there. Okay, I was still there for gingerbread.
[06:54] I'm looking at yours now and honeycomb. Okay, apparently I was there for ice cream sandwich too.
[07:01] And jelly bean. Okay, I just don't remember it.
[07:05] Maybe that's when I switched over to iPhone was, you know, before I...
[07:10] - And the thing is as well, like Google for a long time didn't really kind of publicize the version numbering
[07:18] or anything like that. It wasn't a very public facing kind of thing.
[07:22] It was just this runs Android, which caused a lot of issues, which I'm sure we'll get into.
[07:26] But because, you know, all these different versions running all these different kind of environments,
[07:34] they didn't work together, but yeah. But yes, yes, it's been around, like I say,
[07:40] it's been around for a long time. It's been around since kind of 2007 publicly.
[07:45] But I will sort of give you a little bit of a history lesson.
[07:50] And I will also actually say that if you're ever interested in really digging into Android history,
[07:57] there's a book called "Androids," which is by Chet Hayes, who was one of the kind of quite early Android developers
[08:04] actually at Google working on it. So I will plug his book because it's an incredible book
[08:10] that really goes into detail about how Android was built from nothing.
[08:14] - And what was his name again? - Chet Hayes.
[08:18] I will pop it in the Twitch chat. - Great.
[08:21] I was like, "I'll Google it." - He has, you know, I know there is like a PDF version
[08:27] and all that sort of fun stuff as well, but it's a very good book.
[08:30] So I will plug that slash, because that's kind of one of my primary sources,
[08:34] 'cause, you know, a lot of this information wasn't publicized until very recently.
[08:39] - Oh, wow, okay. - And so basically, if we go right back
[08:44] to when Android started, Android started as an idea to build a new operating system for digital cameras.
[08:52] - Oh, I never knew that. - The two people that kind of invented Android,
[08:58] they didn't like the systems that existed for digital cameras.
[09:01] They were rubbish, and they were rubbish, and they probably are still quite rubbish.
[09:05] And actually, a lot of cameras do now use Android, which kind of is a bit strange.
[09:10] But anyway, this was the original idea. This was the original plan.
[09:14] They were gonna build an operating system for digital cameras that were gonna make
[09:17] them much more user-friendly and much more feature-rich. And at the same time, Google was starting to look
[09:23] at how they were gonna build an operating system for this brand new things called smartphones.
[09:29] You had the BlackBerrys and-- - PalmPilots.
[09:33] - PalmPilot, there was rumors that Apple were gonna be bringing something.
[09:38] There was all these kind of things in the air, and Google wanted in.
[09:42] So they actually ended up talking to these two guys who were coming up with Android,
[09:47] and said, "Hey, we really like what you're doing, "but can we, instead of doing it for cameras,
[09:52] "can we do it for mobile phones?" Which is a bit of a segue, but they did.
[09:58] And they said, "Yeah, maybe." And basically what they did is they came up
[10:03] with a prototype of how this might work in JavaScript. - Okay.
[10:07] - It was literally just a web application that they built as like a little demo UI thing
[10:13] of how an operating system might work. Yeah.
[10:16] - Okay. - And that's what Google bought was a JavaScript demo.
[10:22] That was all there was. They had no code, there was nothing behind it.
[10:29] It wasn't anything. So Google bought this,
[10:32] and then the founders of Android realized we actually have to now build an operating system.
[10:37] So they went about building the whole mobile operating system essentially from scratch,
[10:45] from just this idea. And it was obviously an awful lot of work.
[10:49] And as we'll say, the book goes into great detail about how kind of, then over, this was like 2005.
[10:56] So then over the course of the next two years, they spent this time building out this operating system.
[11:01] And what you'll see is, if I can share my screen, you might remember that the first Android device
[11:09] was the HTC Dream or the T-Mobile G1 in the US. But what we had was this test device,
[11:17] which was the first device to run Android. And this is a very early version of Android as well.
[11:23] It looks an awful lot like a BlackBerry. This is what they were thinking smartphones were gonna be.
[11:29] And then the iPhone released. - Yes.
[11:35] - And suddenly everyone went, oh no, that isn't what people want as a smartphone.
[11:42] So within the space of less than a year, they released this instead.
[11:47] And this was the first actually publicly available Android device.
[11:51] And they basically had to take a complete like right-hand turn to include a touchscreen,
[11:57] to build an interface around that and do something completely different to what they planned.
[12:02] And so the early days of Android were very rocky. It wasn't a very well-polished thing at all.
[12:10] It was quite bumpy. It was very limited.
[12:14] There wasn't a whole lot you could do, but what it did have was integration into Google services.
[12:20] So things like you could use Google Maps, you could use Google to search,
[12:25] and you could, it has an app store, which actually the iPhone didn't at the time.
[12:31] - Oh, really? - The first iPhone had no app store.
[12:35] So Android was the first platform to kind of actually open itself up to developers
[12:41] in that sense. But the other thing which was massive
[12:45] was that they didn't just open up the platform for allow app developers,
[12:49] they opened up the whole operating system and they released all the source code,
[12:53] fully open source and said, "Anyone can use this if they want to."
[12:58] - This is like so bizarre to me in the fact like you're explaining like so much of it
[13:04] that I didn't, just being somebody that was like a salesperson of this
[13:14] or customer service and like having to fix so much of it, or like having to take it apart,
[13:20] like because back then we had like the actual like tech area to fix phones and this is like so surreal,
[13:29] like learning about it beforehand with the knowledge I have now, this is weird.
[13:34] And really cool. And hi, homie, just to catch up on everything.
[13:39] Interesting, okay, so... - So it was a big, yeah.
[13:46] It was a thing that existed and it really was quite rocky to start with.
[13:53] It took a few releases, a few versions of Android before things started to get stabilized
[13:59] and kind of the market started to grow. But the biggest thing was the fact
[14:04] that it was fully open-source and it's still open-source today.
[14:09] And for anyone that doesn't really know what that actually means,
[14:13] it literally means that you can go to this website, android.com/android,
[14:20] and you have all of the code that makes up Android. Everything is here in lots of directories
[14:29] and there's lots of code, there's millions of lines of code. But everything you need to actually build a version
[14:36] of Android yourself is publicly freely available for you to use.
[14:41] And that was kind of unheard of across all mobile platforms. Back then, of course, things like Nokia's stuff
[14:50] were still huge and they had an operating system, but it was much simpler.
[14:54] But this was just like completely unheard of, brand new territory.
[14:58] But what it did mean is phone manufacturers didn't have to build their own operating system.
[15:04] The likes of Samsung, HTC, Motorola, they could focus on building the hardware
[15:15] and they didn't have to invest thousands and thousands or millions in software developers
[15:20] to build the operating system. They just needed a small team.
[15:24] - Is HTC still a thing? - Oh, yeah.
[15:29] I mean, technically as a company, there is a company exists that's called HTC,
[15:36] but it is nothing like it used to be. And I think that's one of the very sad parts
[15:42] of Android history is just how quickly... Like HTC was the first company.
[15:48] They manufactured that prototype device I showed you. They manufactured that HTC Dream.
[15:54] And yet over the course of the years, Samsung just grew and grew and grew
[16:00] and kind of just completely dominated the market. Partly because...
[16:06] - Oh, go ahead. - No, I was gonna say partly because even Google
[16:09] kind of sided with them really. - Yeah, because even in Motorola was pushed out
[16:15] because Motorola was some of the very first ones too. - Yeah, yeah, they were.
[16:21] It was basically, it was HTC and then Motorola very quickly behind.
[16:25] - Samsung was actually quite late to the game, a few years down the road.
[16:29] And yeah, it does, it's sad to me because a lot of very cool HTC devices were created.
[16:37] - Interesting. And I'm also like thinking back to,
[16:42] and this is just like experience with these devices of like which ones worked well or which ones didn't.
[16:50] And because like, that's how we would have to advise people on them.
[16:54] And it's so weird to me, because especially now knowing more of
[17:00] that the manufacturers only had to work on hardware instead of the software,
[17:05] I'm really seeing how much of that was when we would talk about battery life.
[17:10] And Motorola, this is going off of memory, definitely not facts,
[17:18] but it was, from what I remember, it was like Motorola did so much better with battery life
[17:23] than HTC or like the touch. HTC, at least from what I remember,
[17:28] we didn't sell a lot of them because like the touchscreens would stop working
[17:33] and that type of thing, which is interesting to me, especially if they're the ones who came out first
[17:38] and that being pushed out from everyone else. So very interesting.
[17:47] - Yeah, and I think the thing is what happened is that in Google's perfect world,
[17:52] so this was an open source project that anyone could use, anyone could use freely.
[17:57] However, if they wanted access to Google services and namely they wanted access to the Android marketplace
[18:04] or what's now the Play Store, you had to sign an agreement with Google.
[18:09] So you had to kind of conform to Google's requirements, wishes, whatever it might be
[18:15] to become a certified device like that. And so what that meant is in Google's mind,
[18:20] they wanted everything to kind of be the same. They wanted the same feeling,
[18:24] the same operating system across whatever device you bought, because that would be easier for users.
[18:29] Like what you'd be picking is the hardware. Did you want a physical keyboard?
[18:35] Did you want a better camera or a better battery? But actually what happened is manufacturers didn't like that
[18:43] 'cause it meant that their phones all looked very much the same.
[18:45] And from a branding point of view, that didn't work. So you get this fragmentation
[18:50] where they take the operating system 'cause it's open source and freely available
[18:55] and they start customizing it. They add their own theme.
[18:58] They add their own like pre-installed apps. - Yes.
[19:02] - And it's these things that started to really slow down Android,
[19:07] really kind of bug things down because it just, yeah, it didn't work well.
[19:13] - And a homie asked that, this is crazy. So you could still today really tinker
[19:20] and make your own Android OS essentially. - Exactly, exactly.
[19:24] You can definitely still do that today. Getting it running on a device is a little harder,
[19:31] like an actual commercial phone, because you kind of have to root the phone
[19:37] and like bypass the protection that manufacturers have installed, but you can do it.
[19:42] And you can definitely still do it and you can definitely do it in more like developer devices
[19:49] and stuff that you can buy online, 100% possible. - Developer devices, now I'm Googling that really quick.
[19:55] - Google actually used to, you do arrange themselves, called, they were the Nexus devices.
[20:01] So Nexus S, Nexus One, there was loads of them. And those were like Google sanctioned developer devices.
[20:11] Unfortunately, they stopped doing those and started to focus on the Pixel devices.
[20:15] But there are a lot of kind of developer platforms and stuff out there, but you can still do it.
[20:21] It does still happen. And there are still ways that you can like root your phone
[20:26] and then install your own stuff on it. It's just kind of stuff gets a bit more locked down
[20:32] these days. - Like when I remember hearing it for Android,
[20:40] I would hear things like root your phone, that type of thing.
[20:43] But when it's going to iPhones, I would always hear like jailbreak.
[20:48] Is there a difference? - Yeah, so there isn't a particular difference.
[20:54] Both of them is about gaining control over your device and doing what you want with it.
[20:58] The reason why in Android we call it root is actually because Android was built
[21:06] on top of a thing called Linux. So Linux is an operating system.
[21:11] It's an operating system that kind of more traditionally runs on either servers or desktop,
[21:17] or actually it can run pretty much anywhere. It's essentially kind of that low layer of the code
[21:24] that sits between the actual hardware and like actually on the processor.
[21:30] So it's what's converting your nice code that you're writing in JavaScript or something
[21:36] into something that a processor actually understands as binary information, the memory understands it
[21:43] and the kind of the hardware level. So it was built on top of this thing called Linux
[21:47] and Linux has this idea of users. So just the same way as like your computer,
[21:53] you can have a user on your computer. So you might have a user with your programs installed
[21:59] and then someone else might have their own user with their programs installed
[22:05] and you don't have access to each other's programs. - Right. - Like you've got
[22:08] this own area, yeah. So Linux has this idea of users
[22:11] and it has a special user called root and root has access to everything.
[22:17] That's kind of like your admin or your kind of full permissions user.
[22:22] So on Android, we say root your device because it's literally gaining access to that user
[22:29] that has access to everything. 'Cause then from there, you can delete stuff,
[22:32] you can edit stuff, you can do whatever you want. And you have full control over the system.
[22:37] - Is a developer device then just a getting to the root and it just comes pre-set up like that
[22:47] instead of having to do it yourself? - Yeah, so essentially it'll either just come pre-set up
[22:53] and you'll have direct access to root. Or the other thing that these manufacturers of phones do
[23:01] is they do think they lock the kind of boot up process. So when the device is turning on,
[23:08] you don't have control of saying which user you want to access.
[23:12] It just automatically logs you straight into the user environment that's safe for the phone.
[23:18] Whereas if you think about a desktop computer, it'll take you to a login screen and ask you.
[23:24] So what you might find is actually on a development device, you kind of essentially get that login screen.
[23:31] It's not as pretty as an actual login screen, but that's the point.
[23:35] You can select how you turn your device on so that you can then boot it into the root user,
[23:42] do whatever you want to do. And then maybe you want to boot it into a different user
[23:47] 'cause you want to test something else. - This is like, so you're answering all these questions
[23:53] that I had when I was working in the industry that no one could ever answer
[23:59] because by the time it got to the stores, it wasn't like we had developers around
[24:04] to be able to explain what was going on. But like, I remember on different Android devices,
[24:12] how it would be like, if something really broke, it would be just like a screen of code.
[24:17] And back then I had no idea like how, what it said or how to read it,
[24:22] that it would just be like an almost automatic, we're just going to swap your device as a bed.
[24:28] And I've been Googling over here of like different developer Android phone,
[24:34] and I'm going down a rabbit hole. So I'm going to stop looking at that
[24:37] because now I really want to find one and see what I can do with it.
[24:41] So putting that on the side. Now, when is, and you mentioned this earlier
[24:49] that Android was originally built with JavaScript. Is it still JavaScript?
[24:57] - No. - Okay, I didn't think so, but.
[25:00] - So essentially what they did is when Google bought it, the guys that came up with this,
[25:06] threw that demo in the bin and got rid of everything that they'd done.
[25:09] So literally threw away what Google actually bought and started fresh.
[25:14] And, you know, I'm not entirely sure at the time how much like the execs at Google were aware
[25:20] of what was actually, what they'd actually bought. And I think it was much more conceptual
[25:24] and much more like, is this idea that we have? And yeah, we can totally make it.
[25:29] We don't know how we're going to make it, but we can totally do it.
[25:31] So no, that was all thrown away. - Okay.
[25:35] - And what you actually have now is most of, so the Linux layer, the low level,
[25:41] that's all written in C. - Okay.
[25:44] - Which is a very low level programming language. And then everything on top of that is a mixture of C++.
[25:52] So that's kind of, C++ is basically a language that's still quite low level.
[25:57] That's why it's called C, but it uses, it allows you to do things like objects
[26:02] and it has like, it's an object orientated language. - Can we pause really quick for a funny story?
[26:09] - Yeah. - So I'm giggling at C++ because when I was like,
[26:16] I'm going to be able to get my computer science degree and this is going to be awesome in school.
[26:22] I took the class and it just didn't click. It did not click whatsoever.
[26:27] And, but I really needed to pass the class. So I just started skipping class.
[26:33] And the instructor was like, you can pass the class if you catch up
[26:37] on all of your homework. And I was like, okay.
[26:41] So I went to Craigslist and found someone who understood what was being asked
[26:52] and just purposely made mistakes in them. So that way it wasn't perfect,
[26:58] but did all my homework for me. Not the smartest move,
[27:04] just, and I'm not suggesting this for anyone, but that was my introduction to programming.
[27:11] And I always felt like, because I was dyslexic, I didn't know I was dyslexic back then,
[27:16] but once I learned I was dyslexic, I was like, oh, that's probably why I couldn't understand it.
[27:21] And I never knew how to start understanding the theory behind it
[27:29] to be able to understand the coding going on. So now that you're talking about that,
[27:34] it's like different layers and that it's C and then C++ and what you'll continue with.
[27:41] I'm like, I wish I understood that back then. At least now I have funny story.
[27:48] - Yeah, exactly. So yeah, so that is what actually makes up
[27:54] the Android operating system is C and then C++. Then what they did to like, so they built this thing,
[28:03] they built this operating system. It worked, but then they had this issue of,
[28:08] well, how do you build applications for it? It's a completely new form factor.
[28:13] It's a completely new world. And at the time they actually had,
[28:18] the guys that built it actually had experience using Java. So they'd built like Java applications
[28:27] on like old style phones. So you had like these Java mini games.
[28:32] I don't know if you remember them. It definitely dates me, but they existed.
[28:36] And- - Like what?
[28:39] - I'm trying to think of some names of them now. It was like, it was after Snake
[28:44] and it was kind of like, you know, the next level. - I'm not gonna lie.
[28:48] I went from Snake to Brick Breaker. And I'm like, but that's like, you know,
[28:53] the really, really old school phones to BlackBerry. I'm like, were there any other ones?
[29:00] I don't remember. Anyway, please continue.
[29:03] - No, no, no. So they just kind of leveraged their experience
[29:07] and they thought, well, right. We will allow developers to build apps in using Java,
[29:13] which is a programming language. And the specific reason for that is Java,
[29:17] when you write your code in Java, not to be confused with JavaScript,
[29:22] they are completely separate. When you write your code in Java,
[29:26] it actually then runs in like a virtual machine. So your code has no idea about the outside world, basically.
[29:36] It doesn't know that it's running on an Android device. The idea there is you could write an application in Java
[29:45] and it would work anywhere that has a virtual machine. So it used to happen a lot on old websites as well.
[29:54] There'd be a lot of Java on websites. You'd have to install plugins to get it to work
[29:59] and keep those up to date and they'd never work. And it was quite popular at the time,
[30:04] like early, like 2008, 2009. And so they decided to go down this route
[30:09] because it meant that there was a security element there. If your Android app didn't know what was going on around it,
[30:18] it couldn't do anything bad, was the theory. You couldn't do anything malicious.
[30:23] It couldn't like read the information from another app. You wouldn't want some malicious app
[30:29] to be able to read your banking information from your banking app, for example.
[30:33] So there was this idea of built-in security. It didn't work very well, but it was that idea.
[30:41] - Is that what the, just to repeat back, I might have missed this part,
[30:47] of why certain phone manufacturers had their additional software in it?
[30:54] - Yeah. - Okay. - Yeah, so that's the layer where they started
[30:57] installing these additional things. So basically, coming all the way around,
[31:02] Android ended up with these three layers. You had Linux at the bottom,
[31:07] actually interacting with the hardware. The C++ that was the actual operating system,
[31:13] like the actual code, like the code that converted your SMS text message
[31:19] to a signal that your radio and your device understood and sent it, you know, that kind of level.
[31:24] And then on top of that, you had Java. And that was where you could actually
[31:29] then build applications. - Okay.
[31:33] - And that was what was built up and decided as this was gonna be what we release,
[31:39] and they released it. And it worked well-ish.
[31:46] But as you explained, we kind of had these issues where that's at the point where actually
[31:52] manufacturers started installing their own applications. Their own applications that weren't particularly well-made.
[31:58] They were consuming a lot of resource. They would run a lot of background things
[32:04] and they would absolutely slow down the device to basically unbearable speeds.
[32:09] And it caused a lot of issues. - You really are like just bringing back memories.
[32:18] There was this phone, I was so excited about it. It was an HTC phone and it was called the Rhyme.
[32:28] And it was purple and I was so excited about it. And then I got it and HTC put so much on top of it
[32:36] that it would run really, really slow compared to a Motorola device.
[32:42] This is like, okay, so weird. - And you had an even layer even above that
[32:47] because not only were manufacturers putting stuff on it, but the carriers were also putting stuff on them.
[32:53] - Oh yeah, because they would have like the default Verizon app.
[32:57] This is why we didn't get a lot of, I say we, because I was, you know, Verizon back then.
[33:03] We didn't get a lot of the capabilities that they wanted. As in like, it took years before Verizon
[33:12] was allowed to sell the iPhone actually. And Verizon wouldn't get a lot of the phones
[33:19] that AT&T did because of them wanting to have a specific control over the phone.
[33:27] - This is so weird, like so fun, but it's like so weird bringing this all background.
[33:35] Okay, so we got all three layers and then, you know, the manufacturer and the carrier would put extra apps on it.
[33:45] - But all those apps were running, they were all Java and they were running within that kind of third layer.
[33:52] - Okay. - Now the problem with that, of course,
[33:56] was the fact that they were taking up a lot of resource. These apps would run in the background.
[34:01] So they were just permanently taking up space. And that was a problem.
[34:05] And throughout the years kind of Google did a lot to try and stop that happening.
[34:11] It's definitely not so much the case anymore. And, you know, I'd say essentially for about 10 years,
[34:18] if you wanted to build an Android app, you were writing Java code, which was fine.
[34:25] The problem with that was the Java code you wrote for Android was not at all the same as the Java code
[34:32] that you would write for other platforms. So they had this big idea that you would be able
[34:38] to use Java, which meant you could write it once and use it everywhere, but that never worked out.
[34:45] Android never supported like the whole language. It never supported everything
[34:51] that you could normally do in Java. So they kind of ended up with their own programming language
[35:00] that just had the same syntax as Java. So if you looked at the code, you'd say,
[35:08] yeah, that's Java code. But if you Googled, how do you do this thing in Java?
[35:14] The answers you got wouldn't work. You had to Google, how do I do this thing in Android?
[35:20] - Oh. - Precisely.
[35:24] So as a developer, it was a nightmare. And it was especially a nightmare if you perhaps,
[35:29] like early on, there was a lot of people who had already been, who were already Java developers.
[35:35] Maybe they were making desktop applications. They were doing web stuff.
[35:39] They were doing whatever it was. And they saw this new platform and thought, oh, great.
[35:43] I can start being an Android developer. And then they'd get into it and they'd realize
[35:48] that it was some hellish mutation of the language they knew. And it was, you know, not great.
[35:55] So this was a problem for a long time. And on top of that, Android had its own way of making UI.
[36:05] Like you had Java on the code doing the logic, doing your code.
[36:13] But basically how you presented that on the screen was all done using XML layouts.
[36:21] So XML, it's kind of, I'm not sure if it's something that you've come across in your learnings.
[36:29] But it's a lot like HTML in that it's a markup language. And so you have like, if you think HTML,
[36:40] it's the same sort of thing. You have tags, which, you know, you open and close,
[36:45] you kind of nest things and all that sort of stuff. XML is just kind of more arbitrary.
[36:53] Like you can define your own tags and you can kind of build your own system around it.
[36:58] - I'm Googling while you're explaining. And isn't the other, maybe I'm getting this wrong,
[37:10] but isn't there an XML file for like Excel files too? - That's XLS, slightly different.
[37:21] But if you actually open a spreadsheet file in like a text editor as just raw text,
[37:30] it is actually XML as well. - That's probably, so no, I haven't gone into it,
[37:35] but I'm like, I know I've seen this somewhere and I never know what to do with it.
[37:40] - When we start looking at it sort of probably next time, you'll definitely recognize it
[37:44] because it is like ubiquitous across development. It pops up a lot.
[37:52] So on top of Java, they're not supporting the real Java. They also had their own way of creating UI using XML.
[38:02] So it was really difficult to get into because basically you had to throw away
[38:08] everything you already knew. So in 2017, basically Google said we've had enough,
[38:16] we're building, well, we're changing programming languages. We're gonna use Kotlin instead.
[38:25] And that kind of solved a lot of the issue because Kotlin was new
[38:32] and it worked a lot more like JavaScript. Like when you look at Kotlin code,
[38:37] it looks quite a lot like JavaScript. And it was also its own,
[38:42] it was literally its own language. So now when you Google, how do I do something in Kotlin?
[38:48] It will work in Android as opposed to the issues they used to have.
[38:51] So that is a very whistle-stop tour of the history of Android.
[39:02] And the structure of Android. - I'm Googling again, if you couldn't tell.
[39:09] And I'm not doing just like what it came up as, like I did Kotlin Java and it has questions like,
[39:24] is Kotlin harder than Java? Is Kotlin replacing Java?
[39:32] So if I understand correctly, then Kotlin is, is that now only for Android still?
[39:40] - No, so you can use Kotlin elsewhere. Essentially, when you build a program
[39:47] that's written in Kotlin, it actually generates a Java program.
[39:54] So you can still use it in other places that you would normally use Java.
[40:00] And in fact, you could actually go as far as to have some Kotlin code in your Java application.
[40:06] It's a little confusing and a bit weird, but the two are replaceable, basically.
[40:10] - Would that be, and this is just me not knowing all, like the languages break down enough yet in the ecosystem,
[40:19] but could it say that Kotlin is almost like a framework of Java?
[40:25] Kind of like TypeScript is to JavaScript? Or React is to JavaScript?
[40:32] - The concept is definitely very similar. I think if you publicly say
[40:37] that Kotlin is a framework of Java, people are gonna get very angry.
[40:41] - Good to know, good to know. - But if you're purely thinking in concepts, yes.
[40:46] Essentially, Kotlin is a new way of writing code, but actually under the hood, when it gets built,
[40:54] you end up with Java and it runs in the Java environment. Now, there's another thing to add more confusion,
[41:02] 'cause this whole talk is just pure confusion. - Yay.
[41:07] - There is another thing called Kotlin Multiplatform, which actually allows you to then write in Kotlin
[41:15] and then build it into iOS code. So you can build for iOS in Kotlin
[41:22] and also into JavaScript. It will convert it into JavaScript
[41:26] so you can build for the web as well. So they've essentially come up with this whole thing,
[41:32] this whole build process that would allow you to, as the name kind of suggests,
[41:37] write Kotlin and it be built for multiple platforms. - What are iPhone apps built within?
[41:47] - So iPhone originally was built in Objective-C and now it's built in Swift.
[41:53] - The iPhone itself or the apps? - The apps.
[41:57] The iPhone itself is a much more convoluted mess because it's closed source.
[42:01] We don't, we can't see it. - Yeah, yeah, yeah, okay.
[42:03] - So we only really know what people have kind of publicly said,
[42:07] and much like with all Apple things, it's a mix match of lots of bits and pieces.
[42:13] - Homie just asked a good question of, Kotlin seems super flexible.
[42:21] Why do you think it's not more widely used? I just read that in a different way
[42:26] than you actually typed it. Thanks, dyslexia.
[42:29] - It's all good. Don't worry.
[42:32] I read it in a completely different way as well. So there we go.
[42:34] - Cool, yay. - Why do I think it's not widely used?
[42:39] Well, it's still quite new. So it really was only like 2017
[42:43] that it started to take off. And it only really took off because Google said,
[42:47] right, we're gonna use it for Android. And the other issue is,
[42:51] especially with the multi-platform side of things, convincing developers to move away
[42:56] from their native platforms, convincing JavaScript developers
[42:59] that Kotlin is better to do, and convincing iOS developers
[43:03] that it's better to use Kotlin over Apple stuff. That's like near impossible.
[43:08] So it's taken a lot to kind of convince people to start using it.
[43:15] But also it's just not a very mature thing. If you think about the fact that Java has existed
[43:20] for about 30 years now, something that's only existed for five years
[43:25] is, you know, much less of an attractive thing when you're deciding what, you know,
[43:31] your super important, super reliable application, you want something that's kind of reliable.
[43:38] But it's expanding. I really think that we're gonna see
[43:41] a lot more of Kotlin in the future. And I'm a big fan of it.
[43:45] - I have been enjoying my Googles during our stream today. In the fact of just like,
[43:53] it's helping me piece it together a lot more. And also being able to look at the histories
[44:01] of these languages and like what they influence and when they came out,
[44:07] really helps to go along with the story as well. So I appreciate that.
[44:14] Okay, so we've been mainly talking about the operating system thus far, right?
[44:20] - Yep. - How are apps built?
[44:23] - Yep. So as we've kind of said,
[44:27] let's, and we'll kind of focus on how they're built now, because the other thing is just as much
[44:32] as Android itself has changed, the apps themselves have changed significantly
[44:36] as well over the years. And there's been lots of like ways of building things
[44:41] that are just completely disregarded now. So there'd be no point in learning them
[44:44] because you would never use them. So in terms of the app side,
[44:48] we definitely wanna focus on Kotlin and how we build from there.
[44:56] Essentially you have, your app is immediately split into two parts.
[45:00] You have the UI and then you have the, what we'd call the business logic,
[45:05] the actual code behind it that's deciding what to do. So when a user presses this button,
[45:12] what should that button do? You've separately, you've got,
[45:15] well, how does that button look? How does that button feel?
[45:19] You know, that sort of thing. And then you've got, well, what happens when you press it?
[45:23] So that gets split down and you can still use the XML layouts.
[45:27] That's still very much something that exists. And it's probably what we'll do in our sort of future app
[45:33] because it's definitely the easiest, it's the most established,
[45:38] but there are new ways of doing that as well. So you can actually write your UI in Kotlin
[45:44] using like a framework called Jetpack Compose, which allows you to do a lot of really cool stuff.
[45:50] But again, that's a very new thing. It's evolving, you know, it's not there yet.
[45:55] So apps are built in Kotlin and they're built using an IDE,
[46:02] an integrated development environment called Android Studio. There are other ways that you can build apps,
[46:11] but this is kind of the, definitely the Google approved way of doing it.
[46:16] And so what you would do and what you can do, whether it's now or after this,
[46:24] is you download Android Studio and that gives you a piece of software
[46:29] that looks a lot like this. It is an IDE, it's actually made in joint with IntelliJ.
[46:36] - Okay. - And they do other IDEs as well.
[46:39] So if you're familiar with their products, it looks very similar.
[46:43] But again, a lot of people have very opinionated views on what is the right IDE to use,
[46:50] whether it's visual code or whatever it might be. That's probably the one plus side of Android development
[46:56] is you don't really have that. You have the one IDE that you use and everyone uses it.
[47:03] And this provides a lot of different kind of tools, not just your code editing,
[47:09] but also has an emulator built into it. So you can actually run a Android emulator on your computer
[47:17] and see what it would look like when you're running your app
[47:23] and you can interact with your app live. And that is actually emulating an Android device,
[47:28] which is pretty cool. - That's really cool.
[47:31] - And that obviously makes it much easier to develop because A, it removes that barrier of entry.
[47:36] You don't actually need an Android phone to build with an Android app.
[47:40] It also means that you don't always have to have your phone connected to your computer to do it.
[47:45] You can just kind of iterate, make a change, run it on the emulator, make a change,
[47:50] that sort of thing. And then it's got all the other sort of normal things.
[47:54] So what we can actually do, I think the easiest way would be to download Android Studio on your side.
[48:03] And I'll walk you through kind of getting that set up. And if we have time, maybe we'll open up
[48:11] their sort of template "Hello World" application. - I'm downloading, you guys can't see it,
[48:27] but I will get there. I'm just very concentrated on it today.
[48:33] - That's all good. - Share screen, this one, share.
[48:39] There we go. - Cool, I'm gonna bring you up a bit bigger
[48:59] so I can see your screen as well. (laughing)
[49:04] - There we go. - You're gonna open?
[49:13] No, okay, fine. - Yay.
[49:32] - Cool, so you don't need to import any settings 'cause you've never used it before.
[49:36] - Sweet. - And we will open Android Studio,
[49:38] which is the latest version is codenamed Dolphin. So basically what we do is it takes you through
[49:45] quite a nice setup wizard, which is actually quite pretty straightforward.
[49:48] So we'll, you know, the other thing probably to mention at this point is, you know, at this point in history,
[49:56] now Android isn't just for your phones. Android, you have Android tablets,
[50:01] you have Android, you know, wearables like watches, Android in your car, you have sort of that system.
[50:10] So all of these systems use the same coding language and the same setup.
[50:16] So you can do it all within this IDE. So this will just kind of go through
[50:20] and basically download everything that you need. You'll need to click on the Android SDK preview license
[50:27] as well and accept that as well. And that'll then basically download the emulator
[50:35] and all the other sort of gubbins that build it together. This was all, this all used to be much less straightforward.
[50:44] I must say, this is probably a very good time in history to be starting Android development
[50:49] 'cause you have things like this that just download it for you.
[50:53] - Yeah, this is cool. And now going back to what we were talking a bit
[51:01] about earlier is how Kotlin has something that will also make an iPhone app too.
[51:15] Will this help with that? - So not really.
[51:20] That kind of is something that, that's why they kept it as a separate project.
[51:25] That's why it's that specifically called Kotlin Multi-Platform
[51:28] 'cause it's kind of another layer on top. So you would still use Android Studio for your Android bit,
[51:36] but then actually when you're building an iOS app, you would use Xcode and they just then share a lot of code.
[51:43] It's all, again, it's probably something we could specifically talk on for about 10 years
[51:50] just on that. But it is pretty cool how they've managed to do it.
[51:55] - Okay, interesting. It's, I put the link in as well
[52:00] because I think it's definitely something. It's interesting because since I've started the show,
[52:08] people have asked me when I'm gonna start niching down into one specific area and I'm like, how can I?
[52:15] I don't know everything that's out there. It's all so cool.
[52:19] So I'm going to start doing a hundred days of code in JavaScript just so that way I have it built out
[52:28] in a proficient in one language. Yet I'm loving the show of like,
[52:33] there's so many different things to learn. - Yeah, excellent.
[52:37] So here we go, yeah, and we can hit new project and this gives you loads of template projects
[52:43] that you can kind of get started with. So let's go with the login activity, actually,
[52:50] that's on the right there. That's quite a good one
[52:52] 'cause that gives you a bit of an idea of what's going on. And then you can literally,
[52:56] gives you the helper to name your application and set all these sort of things up.
[53:06] There's the minimum SDK thing is quite interesting. So I don't know if you've,
[53:12] you might've actually heard about it when you were sort of on the retail side,
[53:16] but this whole like fragmentation of different devices running different versions of Android.
[53:21] So as a developer, when they release a new version of Android,
[53:27] you obviously want to use those new features. They'll bring in some new, cool new things.
[53:32] However, those cool new features only work on the new version.
[53:37] So if your users aren't using the new version, you can't use those cool new features.
[53:42] So this is where you have to kind of set a minimum SDK to say, my app will only run on devices newer
[53:48] than whatever version. And it gives you a little prompt there that says like,
[53:54] you've selected API 21, which is a lollipop. Your app will run on 98.8% of all devices.
[54:02] And that's fine. And you can kind of go all the way up
[54:07] to the latest versions. And like you say, yeah, the latest version,
[54:13] there aren't any really any devices yet. And it's definitely interesting to see how segregated
[54:19] and like split out Android still is, which is a shame, but it's part.
[54:25] - This is interesting, okay. Which one were we, lollipop, there we go.
[54:31] - So it's something as well that like iOS developers don't really have to deal with
[54:36] because Apple are better at keeping the momentum forward. So everyone always wants to get the new iPhone.
[54:46] And because there's also only one iPhone, they support like four or five old iPhones,
[54:54] keep them updated. And then when they release a new one,
[54:56] they just remove the oldest and it keeps that momentum forward.
[55:01] Whereas with Android, because you as a manufacturer can select whatever version of Android you want,
[55:07] you do still get devices that are being produced brand new that actually you're running versions of Android
[55:12] that are four years old. And that's just because they haven't internally updated.
[55:21] They don't have a developer to do that or whatever it might be, and that causes a lot of issues.
[55:27] - That is so interesting. And so like to use the legacy support ones
[55:33] would make it so that way, if it's using like old stuff, so if we, I'm guessing for the minimum SDK,
[55:40] if we did that, it would be using like Jelly Bean, which would make it before they had the App Store, Play Store.
[55:48] - Yeah, yeah, exactly. So you can definitely-- - Interesting.
[55:51] So don't click that. - No, there's no, yeah, definitely.
[55:55] And again, Google's done a lot of work to try and make it easier by like backporting changes.
[56:01] So older versions get updates through the Play Store, but it's still very, a fragmented mess, to be honest.
[56:09] But yeah, so we've, this is just gonna kind of compile. - My, are you already having issues?
[56:17] - You can just close that. It's fine, it's fine, I'm sure it's fine.
[56:20] It's still building, yeah, it's doing the thing down the bottom right-hand corner.
[56:25] - Oh, I'm like, why are you still like, I just got you. This is so cool.
[56:31] Like this will, what up, Akari? I'm definitely getting some type of Android
[56:42] by next week now. - Sounds good.
[56:45] - 'Cause I want it. Will it make much of a difference
[56:47] if I get a tablet instead? - Not really.
[56:51] We can definitely explore, you know, the UI difference of having a big screen
[56:55] versus a small screen and the headache that that causes. (laughing)
[57:00] But yeah, yeah, we, functionally, pretty much the same. - This is, apply the code set up, yes.
[57:10] - So it's, so it's now just kind of pulling in everything to build the template application
[57:17] that we've asked it to build. And I think just 'cause it's the first run,
[57:22] it does take a moment. - And so would it be possible,
[57:29] do we have to use this IDE or could we use like VS Code instead?
[57:34] - So you could, but the problem is when it comes to actually building the app
[57:40] and making it into a file that people can install, you kind of now have to use Android Studio for that step.
[57:47] - Oh, interesting, okay. - So there are ways you can do it from the command line.
[57:53] You can like directly run the programs that actually do the building and stuff
[57:57] that's like under the hood, but they've really tightened down on saying that,
[58:03] no, this is the only way we officially support. So it can be a pain.
[58:09] Like, yeah, I would, this would be the only thing I'd recommend.
[58:13] - And this is another thing is I don't even know where it's saved this to.
[58:20] I can fix that, but just as a, I'm newer to GitHub and need to working on it,
[58:28] but as long as I save it to like my code folder, it'll still be the same as uploading for,
[58:34] I can upload a repo for it. - Yeah, you can actually even do that
[58:38] within Android Studio as well. - Okay.
[58:41] - So along the top menu, you've got one that says VCS.
[58:44] - Oh, yes. - And that's your version control.
[58:48] And so you can create a Git repository. You can share the project and get help.
[58:52] You could do all of these things. It'll probably ask,
[58:55] just then ask you to log in and do all that sort of fun stuff, but.
[58:59] - Oh, why would you need GitHub Enterprise? Whatever.
[59:07] I'll look at it later. - There we go.
[59:09] It has set up. So on the left-hand side now,
[59:14] you see there's a directory called app. And if you click on that,
[59:20] that'll expand out to the different areas of the app. - Oh, I didn't mean,
[59:25] well, that was fun. Not what I meant to click, but that was fun.
[59:29] - No, that works. - I was gonna see if I can just make it bigger.
[59:34] It doesn't appear. - You should be able to just,
[59:38] I don't, yeah, don't, don't. You should be able to just drag.
[59:41] Oh, you might like physically, yeah, yeah. You can change the UI size,
[59:45] but it is a little bit of a pain. - Yeah, like it doesn't do it like VS code or in a browser.
[59:50] - For next time, we'll get you set up with being a little bit more happy
[59:55] for people that are actually watching. 'Cause yes, I appreciate it's quite small.
[59:59] - So everybody's gonna squint. This is why I have to use my glasses while streaming.
[60:03] 'Cause I'm always like, I can't see it. We will get there.
[60:08] We will get there. But this is, oh, wow.
[60:11] - So this is the project that's been generated. Yeah.
[60:15] And what you did is kind of expanded everything, which is cool because we can now see it.
[60:22] And there's a lot going on here. So I guess the question is,
[60:26] do you wanna go through this now or should we save this as a surprise?
[60:30] - I kinda wanna save it because I think it'd be good to, we got it installed.
[60:35] We got there. So we don't have to wait for that next time.
[60:39] And we got the history. I think actually going through this
[60:43] is gonna be more helpful as we're building it. So we don't have to recap it again next week.
[60:49] Oh, this is so fun. Oh my gosh.
[60:53] This is so cool. Way cooler than I originally thought it was.
[60:58] - Well, that's 'cause if I say Android development is cool, people just laugh at me.
[61:05] - Well, I think a lot of it is, it's been hard for me to conceptualize
[61:09] and how it goes from point A to point B. Like I can understand like people doing the code,
[61:17] but then how to actually create and run it, especially on a device is like something that I'm like,
[61:27] I know it exists. I know it's possible.
[61:30] I've just never done it. So it's harder for me to go,
[61:33] oh, that was actually way easier, way cooler than I thought it was.
[61:36] And now I'm starting to see that too. - Yeah, I think that's the thing
[61:40] is these things have come on a long way. It is a lot easier.
[61:43] And it's a really fun way to develop because you can physically get it on your device
[61:48] as you're building it, test things out, actually interact with it.
[61:51] And there's a very kind of tactile element to that compared to like maybe doing web development
[61:58] or backend development, where it's just, you're looking at code
[62:00] and running it and hope it works. So yeah, it's definitely something that I really enjoy.
[62:07] - Interesting. Well, thank you so much for coming on the show today,
[62:10] Zachary. So everybody look forward to next Friday
[62:15] because that's when Zachary I think is coming back on. Pretty sure it's next Friday.
[62:20] I'm gonna go double check my calendar now so I don't lead anyone astray.
[62:25] I don't know why. Y'all, I made my life confusing
[62:33] with all these calendars, but yes, it's next Friday, the 21st.
[62:37] Ooh. And the day before that, I'm learning about Kafka.
[62:42] - Ooh. I think you probably know as much as I do, to be honest.
[62:48] - I like getting into sticky situations with the show of not knowing what I'm talking,
[62:56] like even an idea of it. So this is gonna be quite enjoyable
[63:02] learning how to do that. And I am excited because if I remember correctly,
[63:06] you said Kotlin is a lot like JavaScript. - Yeah, I think so.
[63:11] And it's very similar in terms of its structure and kind of what you're looking at.
[63:16] And I think when we start getting into some code, it'll kind of resonate.
[63:20] - Cool, cool. And then Homie did say
[63:26] that he thinks it's a little intimidating, but this helped him understand a bit more
[63:31] and it's very interesting. - Good, I'm glad.
[63:35] - Thank you. - It's always nice when other people think it's interesting.
[63:39] - Yes, not just. I really do, like I think this,
[63:44] I also think that I'm partially like really into learning about it
[63:48] because I used to work in the field. So I'm like, I'm finally gonna be able to answer
[63:55] all of these questions. - Yes.
[63:57] - And see what it takes. - It's 10 years too late. - Yeah, exactly.
[64:00] Yeah, because I actually quit at Verizon in 2013. So almost 10 years, almost exactly 10 years.
[64:09] So that is, that's pretty crazy. And then because we're using Android Studio,
[64:16] do I need to download, download, download, download Kotlin? - No, so everything will have been pulled in for you.
[64:25] It's all in there now. That's, again, that's a perk of using it.
[64:28] Like if you want to go down the route of using a different IDE, it takes a lot of setup.
[64:34] It's just not worth it. It's all bundled in, you can get started and yeah.
[64:38] - Yay, awesome. Well, thank you so much for your time today
[64:43] and coming back next week. I'm excited.
[64:46] You might also get stuck being requested even more because I'm like, but there's more we could do.
[64:51] There's so much more. - Yeah, there's a lot more we could do.
[64:55] - Awesome, well, thank you for your time, Zachary. - Bye everyone. - Bye everyone.

