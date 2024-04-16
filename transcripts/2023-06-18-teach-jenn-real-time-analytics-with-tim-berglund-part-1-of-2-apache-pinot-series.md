---
showLink: "https://www.youtube.com/watch?v=HZdklP6ttyg"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-real-time-analytics-with-tim-berglund-part-1-of-2-apache-pinot-series"
title: "Teach Jenn Real Time Analytics with Tim Berglund Part 1 of 2 Apache Pinot Series"
publishDate: "2023-06-18"
coverImage: "https://i.ytimg.com/vi/HZdklP6ttyg/maxresdefault.jpg"
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

[00:00] Welcome to another episode of Teach Gen Tech. And today we have Tim.
[00:05] Yay. Tim, who are you?
[00:07] Hi, Jen. Hi, everybody else.
[00:09] What are we talking about today? Who am I?
[00:13] I'm Tim. We got that far.
[00:15] I run developer relations at a company called StarTree. StarTree makes a fully managed cloud version
[00:25] of Apache Pino, which is a real-time analytics database. And what we're talking about today is real-time analytics.
[00:35] And to get to that, a lot of history and a lot of just like, what is even analytics.
[00:41] Yay. Thank you.
[00:43] And I remember something, Tim, I don't know if you remember this, when we met via Twitter.
[00:54] And before going into that story, I will say one thing that I started with
[00:58] is, the reason I would want to work with Apache Pino is so I can carry around a bottle of wine
[01:04] with me while going to events. No, that's on brand.
[01:09] And I'm actually contractually obligated to drink only Pinot Noir for the duration of my employment.
[01:15] Not a lot of people know that. And I would be totally OK with that.
[01:19] That is my favorite wine. Right, it's like, if you're having some chicken,
[01:26] it's kind of lighter. If you want to go red, you can still do it.
[01:29] But it's still got some body. Why not?
[01:30] It's just perfect. Yes, 100%.
[01:34] And so talking about that, though, do you remember how we met?
[01:40] I do. I do.
[01:42] We came to follow each other on Twitter. And you were looking for a developer advocate role.
[01:48] And I was looking for a developer advocate. I was like, oh, hi.
[01:52] It was. It was a fun conversation.
[01:55] Yeah, and we got on a call and talked. And the way that call went, I was looking for somebody
[02:07] more senior, like that role that I was trying to fill. I needed somebody who had been around a little bit.
[02:13] And it was a senior-level developer advocate role. And that wasn't you.
[02:16] But I remember very clearly that you-- I mean, that's just where you were in your career.
[02:21] You weren't that. But I thought, this person absolutely
[02:25] has what it takes to succeed as a developer advocate. And this is a tricky way to say it.
[02:30] But you have the personality. You have the communication skills.
[02:34] You have the curiosity. This was a year ago, wherever it was.
[02:39] I'm like, yes, this person. And if you look at what you're doing here,
[02:43] just a meta, talking about teach gen tech, this is what-- when I'm able to hire somebody who hasn't had the title
[02:56] developer advocate, and maybe a senior engineer or something who wants to make the change, I'm
[03:03] looking for people for whom developer advocacy is what comes out of them when they're not paying attention.
[03:11] It's just like you prick them, and they bleed teaching people things and wanting to explain things.
[03:16] And I don't know. Seems like this show we're on right now
[03:20] is an example of that, right? This is what you do.
[03:24] It's not enough for you to learn tech topics, but you're going to do it in public in a way
[03:29] that other people can learn too. And that's like--
[03:32] It's interesting. It's interesting.
[03:34] The heart of the teacher and the kind of person who wants to share is the core skill set, the tech skills
[03:43] you can learn. And they change all the time anyway.
[03:45] They do. Oh, you're always learning your tech skills.
[03:48] Thank you for answering that. And I promise I didn't set it up just
[03:51] so that way I could get some fluff in my feathers. It's because I really want people
[03:56] to hear two parts of just because you've never been in a role doesn't mean you can't get there.
[04:05] And also, you can learn so much by interviewing and also create a network.
[04:13] It's kind of weird, but people I interviewed with, like you, I'm like, hey, can I follow up with you sometime?
[04:21] And yeah, it's a bummer for not getting a job, but it really helped expand my network.
[04:26] And that's something that I really want to call out to others to not give up hope
[04:33] because it can be hard to break into any industry. I think it's difficult to break into DevRel,
[04:41] especially if you have an engineering background or not being able to merge the two and showcase that.
[04:49] It's like a different learned skill. Yeah.
[04:54] Oh, OK. We do have quite a few in the audience that I promise y'all
[04:57] I'm not ignoring you. In the background, I used to do--
[05:02] Akari. Oh, hey, man.
[05:03] Yeah, I used to do these streams with my iPad, and at the moment, it's not working.
[05:08] So I'm going to stop paying attention to that and say, what up, Lerner and Francesco and Bakari?
[05:16] Yay. And yeah, Bakari--
[05:19] Francesco, I owe you an email. I know.
[05:21] I'm sorry. I'm kidding.
[05:22] It's been rough. There's a lot going on in June for me.
[05:27] It's all my fault, Francesco. Sorry.
[05:31] Yes, tell us about what's going on because you do have a lot going on this month.
[05:35] I do. I do.
[05:37] I have lived in Denver since 1995. Prior to that, it was '77 to '90, so literally 80% of my life.
[05:47] And in Italy, you're pretty relaxed with timing. That is the reputation.
[05:55] And that is why Italy is such a glorious place. Anyway, yeah, I've lived in Denver 80% of my life.
[06:01] And last week, last week at this time, I was boxing up my apartment and loading up a U-Haul.
[06:09] And we drove Wednesday, starting Wednesday night through Friday night.
[06:13] I arrived in Mountain View, California on Friday. I am now a California resident doing all the residency
[06:20] establishing things. And in 11 days from the time of this stream--
[06:26] it is June 13th today-- on June 24th, I am marrying an absolutely fantastic
[06:34] and amazing woman currently named Rachel Stark. In 11 days, she'll be Rachel Berglund.
[06:41] And I'm super excited about that. Yay.
[06:44] And y'all, apparently I didn't pay attention to the memo that for the last 2 and 1/2 years,
[06:54] Tim and I lived in the same area. Yeah.
[07:00] I'm going to be back every couple months. I still have family that I have a grandson, their daughter.
[07:07] I'll be back. I'm moving to Phoenix at the end of the month.
[07:11] Well, there you go. In roughly two weeks, I'm going to Phoenix.
[07:15] But hey, we're going to have-- I've been trying to have a meet up in San Francisco.
[07:22] How far is Mountain View from San Francisco? Aren't they next to each other?
[07:25] Yeah, it's Bay Area. It's a half an hour in low traffic
[07:30] and an hour in crappy traffic. OK, because we're going to--
[07:35] I don't know if Ivan and StarTree want to do a joint meet up because you
[07:38] guys go to ClickHouse. But we love you.
[07:42] It's the open source data infrastructure. So it's when we get to be friends.
[07:49] Yes, yes, love it. And we're friends anyway.
[07:52] That's true, that's true. And hello, Anthony.
[07:57] Yeah, so let's get into it. Sorry, y'all, you won't be able to see my notes
[08:02] during the stream because my computer just doesn't want to do it.
[08:06] But I will still take notes. And let's-- everyone is Tim's friend.
[08:13] Is everybody Tim's friend? Are you just friends with absolutely everyone?
[08:17] I aspire to be friends with everybody I meet. It doesn't always work out.
[08:20] But those are a small fraction of cases, so yes. I like it, I like it.
[08:25] I feel like I always-- it's kind of fun because for some reason,
[08:31] I don't see a lot of your posts except when you reply to somebody's selfie Sunday.
[08:38] OK, that is a friend who is not in tech at all. I can say her name.
[08:45] Her name is Courtney Sexton. She's not in tech at all.
[08:47] She's a friend of Rachel's and mine. Her husband is a mid-career boot camp guy.
[08:53] So he just graduated boot camp and is looking for his-- Dave Sexton is his name, looking for his first boot camp job.
[08:59] Or first junior developer job out of boot camp. Super sharp guy, like he has taken to this stuff.
[09:05] So can you, y'all. Bakari, you're-- OK, you're moving?
[09:11] Oh, dude, I was going to say, I need to have you over dinner. But I can't do that in the next week and a half.
[09:17] Yeah, Bakari, you're moving to Atlanta. Atlanta?
[09:22] I think it's Atlanta. I feel like you're winning.
[09:25] I'm glad to be here, but I still feel like you're winning. Yes.
[09:31] Oh, yeah, that's true. Bakari's going to sell his house here and buy
[09:34] a palace in Atlanta for cash. That's how it goes.
[09:38] Even the cost of living from Denver to Phoenix is like, we're getting a much bigger house in Phoenix.
[09:47] Good, good. Yeah, yeah, it's gotten rough recently.
[09:51] I don't know, I'm still paying about 2x here relative to what I was paying in Denver for rent, but yeah.
[09:58] Yeah. Yeah, but you got to do what you got to do.
[10:03] And all right, so let's get started. What is real-time analytics?
[10:10] Because I-- and for context, because I know a lot of us, a lot of people are joining because it's Tim.
[10:16] And welcome. And I'm totally going to do a self-plug of make
[10:20] sure you follow, subscribe if you want. That would help too, but follow, because I need followers.
[10:28] I am a developer advocate at Ivan, which is a database management company that we--
[10:38] oh, wow, I don't even know how many-- Francesco, you're here, so how many databases
[10:44] do we help out with? Because I know Postgres, MySQL, Kafka--
[10:51] 600 of them. By the way, hi, Robert.
[10:54] I just saw your shout out, sorry, in the chat. Yeah, it's like 600 of them that you guys post, right?
[11:00] Yeah, there's a lot. And a lot of what I do is I work on getting people started
[11:07] with these different products. That's the content I'm working on with Ivan,
[11:11] as well as meetups. And then I'm still learning about databases
[11:16] with teach and tech. Because as you-- if you check out YouTube,
[11:21] you'll see streams of what is data, and intro to databases, and the difference between SQL and NoSQL.
[11:29] And we're getting there. We've done a stream on Kafka, and I still
[11:34] don't understand it. But that's OK, I will get there.
[11:38] Yeah, so that is the background of why I ask about what is real-time analytics.
[11:47] There you go. And with respect to all that stuff,
[11:50] this is teach gen tech. The conversation goes, where Jen wants it to go.
[11:54] And so whatever-- if Kafka comes back up this week, that's great.
[11:58] It might-- we're going to do this again next week and talk more specifically about Apache Pino.
[12:05] And so that could be a-- might talk about Kafka more there.
[12:09] We'll see. But can I just back up?
[12:13] Before we talk about real-time analytics, it makes no sense to talk about real-time analytics before we
[12:18] talk about analytics. And I have been--
[12:21] and maybe this is like a thing that a middle-aged person does. I've just been thinking about the things
[12:29] in their historical context a lot recently. And I think that helps clarify just what analytics means.
[12:39] Because, Jen, you're interested in databases. But if we would just rewind back to the beginning
[12:44] of commercial digital computing, that's the mid to late '40s, the first computers that we would call mainframes
[12:52] are being developed and sold. We think of them as IBM.
[12:56] There are a few other companies who are in that act. And these are single-threaded batch machines
[13:06] that compute analytics. That's the purpose.
[13:09] Commercial computing begins with analytics. The modern story of analytics begins with, at the same time,
[13:16] commercial computing. And so you had a bunch of data.
[13:19] And there had been in the decades-- by the way, I live in Mountain View right now.
[13:23] And just up Shoreline Boulevard is the Computer History Museum. And you can actually see some of these things
[13:29] that I'm talking about. And I don't want to be weird.
[13:33] I literally weep sometimes in some of those exhibits. It's just really affecting to me.
[13:37] It's amazing, the stuff that's there. But you had, in the decades before that,
[13:42] mechanical tabulating machines where there's data on punch cards.
[13:45] And it's doing basically adding of things. But then the first mainframes are
[13:52] taking data in batches on punched cards and running software.
[13:57] You could write arbitrary programs on these things. And they're doing batch analytics.
[14:03] And it's so difficult. And those machines are so expensive. And the model-- IBM leased them.
[14:09] You didn't buy these things. You leased them for--
[14:12] if you make the inflation calculation, it's hundreds of thousands of dollars a month.
[14:17] And-- So expensive.
[14:19] Right, right. Without even adjusting for GDP and all that stuff,
[14:23] it was a smaller world back then. But they were so expensive that only the largest scale
[14:31] businesses could justify the expense, OK? The auto shop down the street is not going to have a computer.
[14:42] We know that, right? And so large scale businesses and governments--
[14:46] we're talking banks, airlines, utilities, things that operate at that nation scale, governments
[14:52] by definition-- they're buying computers and they're doing batch analytics.
[14:56] And so it's such an expensive thing to do that only these very high status
[15:00] leaders in these very large valuable organizations are able to do analytics.
[15:05] And there's a big separation in time between the events happening out there in the world and someone encoding
[15:14] the events in punch cards and then writing a program, ingesting, blah, right?
[15:20] So-- Quick questions from the audience real quick was,
[15:27] that building used to be Silicon Graphics. SGI, yeah, boy.
[15:33] And then also, is that the same place Adobe and Netscape co-founders worked at together?
[15:40] I don't know. Adobe's founding might have been contemporaneous
[15:45] with early days of SGI. Netscape-- I just don't know the answer to that one.
[15:52] But Bakari is-- I mean, he's lived here longer than I have, so he'd know.
[15:58] But yeah, that's the former SGI headquarters. And it's-- anyway, if you're in the area,
[16:03] if you're coming to my wedding, it's on the list of things to do on the site, on the Knot.
[16:09] So yeah. Anyway, that's the start, right?
[16:15] It's very expensive. It's very difficult. You have to be
[16:17] a status leader in a very valuable, large organization to be able to do analytics.
[16:22] And then we chip away at that. That's the late '40s.
[16:26] By the early to mid '60s, you've got the System 360. And this is a mainframe that is the first kind of thing
[16:35] that we would recognize as a computer, kind of like we think of them.
[16:40] Because it has an operating system that runs on it, and you write software that runs on that operating system.
[16:47] And that operating system is going to get ported to other models in the same product line.
[16:52] Like you have OS X, and it runs on various Macs, and they're all the same, and you write the same program,
[16:57] and they're all there. That's the way we think of the world.
[17:00] So you get there, right? And people are still doing analytics.
[17:04] But now, all of a sudden, computers are fast enough that it's not just a bunch of punch cards
[17:09] in and some punch cards out with smaller numbers on them, but now you connect terminals to them.
[17:15] And so computing is powerful enough to be able to handle transactions, OK?
[17:24] So when we talk about analytics, there are these two kinds of databases in the world.
[17:28] There's transactional databases, and there's analytics databases, OLTP databases,
[17:32] and OLAP databases, those two terms, OLTP and OLAP. And OLTP, transaction processing,
[17:38] wasn't even a thing until mainframes got going for a little bit.
[17:42] And they were fast enough that you could hook up terminals and do this stuff.
[17:46] And so now, by this point in the '60s, it's commonplace to have terminals connected
[17:51] to computers and multiple people doing multiple things. And so now you have some kind of knowledge worker
[18:00] doing their job accessing data on a computer. And that's not analytics happening there.
[18:10] That's transaction processing. So usually what that program did,
[18:14] and that's the old green screen kind of life is what they had then.
[18:19] And basically what they're doing is crud over entities, right? There are things in the world, and they're
[18:24] using the software to create them, read them, update them, delete them.
[18:29] And that's most of the software that's been written in the two or three human generations
[18:35] since that started. You've got these transactional databases
[18:41] with people just accessing entities and looking at them on their screen
[18:47] and making them and changing them. And so there's--
[18:49] Really quick. --interactions out in the world.
[18:51] OK, go ahead. I'm talking a lot.
[18:53] Interrupt me. No, you're good.
[18:53] You're good. I'm just like, I know I'm going to forget this question.
[18:58] OK, so you got transactional, which is OLP. And then you have--
[19:03] OLTP. OLTP.
[19:05] OLTP. O-L-T-P.
[19:08] Cool. Online Transaction Processing, O-L-T-P.
[19:13] Which-- I'm just going to write these definitions down so I don't forget.
[19:16] Online-- There, very good idea.
[19:18] Actional, that-- you know, I hopefully can read my own handwriting.
[19:28] Program? Sorry, what was P?
[19:30] Online Transaction Processing. Processing, thank you.
[19:35] And then the other one was analytics? Online Analytical Processing, OLAP.
[19:43] Yeah, OLTP and OLAP. It was the thing that I'm like, I'm pretty sure that was it.
[19:54] But OK, cool. And then I like how you gave the example of CRUD.
[19:59] You explained it, and I'm like, I think this is the first time somebody has said it out loud
[20:05] that it actually clicked, of what CRUD meant. Because I-- so I wrote it down really quick.
[20:10] I'm like, I don't think I ever clicked that it was create, read, delete.
[20:15] Yeah, I was like, what? What?
[20:17] OK, thank you for getting those there. And yes, please continue.
[20:25] Awesome. So while we're-- and by the way, I
[20:28] love talking about stuff at the super fundamental levels. This is-- I think this is important, because we don't--
[20:33] even people who have been around the block for a long time and we think we know all this, you don't always think, wait,
[20:40] what does that really mean? What's a transaction?
[20:43] Because if you know transactions, you're like, well, you've got commit and rollback,
[20:47] and you've got two-phase commit, and blah, blah, blah. Nobody cares, right?
[20:51] What's a transaction? Well, what does a business do?
[20:55] A business exchanges things with people. You have-- you make something.
[21:00] It's a valuable thing, and you give that to your customer. And what does your customer do?
[21:05] Well, your customer is so happy that you gave them that thing that they give you money.
[21:10] And people do it voluntarily, and it's wonderful. And so there's this exchange of value that's happening.
[21:17] Fundamentally, that's like what a business does. And that's modeled in account.
[21:22] You see that in double-entry accounting, that idea. That's what we're talking about.
[21:26] So fundamentally-- and there are other ways to use OLTP databases, but when you're
[21:32] talking about the activity of a business, those exchanges are happening, and you are
[21:37] recording them in the database. That thing happens out there, and you keep a record of it.
[21:42] Or-- hi, Graham. Hi, Graham.
[21:47] You are keeping a record of a thing, like I'm a user of a system, and I'm doing all these address
[21:54] changes right now. So all of the update operations--
[21:58] I want to go read my account. Show me my address right now.
[22:01] OK, edit, click, new address, update. So you're either recording transactions,
[22:06] or you're keeping track of the state of things out in the world.
[22:09] Fundamentally, that's what transactional databases do. And the point I'm slowly making here
[22:15] is that computers had to get fast enough to where that was even a meaningful thing to do.
[22:24] And then they did, and there are all these terminals, and if you look--
[22:29] I travel a lot. If you ever look at the screen of the airline person
[22:35] at the ticket counter, you ever wonder, why are they typing so much?
[22:41] They're typing all of this stuff so fast. It's really strange, but they're using a terminal emulator
[22:50] on a modern computer that's this interface software closely related to the stuff that was developed literally
[22:57] before I was born, and I'm turning 51 in two days. Happy birthday, and happy congratulations, and yay move.
[23:07] I'm going to keep finding new ones. It's a big two weeks, that's right.
[23:11] So is that a big reason why-- and I'm just trying to think of a real life example of what
[23:18] happened with Southwest during COVID, or last year, I think it was, where all of their flights
[23:26] and things crashed because from what I remember, it was more about their software couldn't keep up with it,
[23:34] and so things got crisscrossed, which in turn makes me-- I don't know any details.
[23:40] I don't know any details of why that went down. In general, I wouldn't blame the platform.
[23:46] I mean, airlines run on mainframes, and a lot of travel deep under the covers.
[23:52] There's still mainframes doing that stuff, and that stuff can scale, and be reliable, and run,
[23:57] and you can screw it up. So I think that had to do with--
[24:02] and last Christmas, there was the big crazy thing because there was lots of travel, and then some weather,
[24:08] and that's just kind of airline instability because there's not a lot of slack in that system,
[24:12] and when one bad thing happens, it-- yeah, but mainframes started as analytics machines.
[24:19] Now they're doing transaction processing, and analytics, or what we then called reporting,
[24:26] was just a feature of the software because all the data is right there.
[24:30] It's one database to rule them all, one database to find them, one database to bring them all, and in the darkness,
[24:39] bind them, and then you've got software and application running around that database.
[24:44] So the transactions, the analytics, they're all the same. It's all fine, right?
[24:47] And so we're bopping along through the '70s, and then in the '80s, some things
[24:52] happen, which is basically PCs. So now we're good enough at making computers
[24:58] that you can make a sufficiently powerful computer that it can do a lot of that knowledge work stuff locally.
[25:07] You can actually have programs running on that thing. Maybe it's still a crappy green screen,
[25:11] and life sucks in 1982, but it's fast enough that it can actually run programs that you can use.
[25:21] And people start connecting those computers on networks. There's this big revolution happening in the '80s called--
[25:28] people talking about LANs, local area networks, and open systems.
[25:32] And now we've got little database servers. Oracle starts as a company in the 1980s.
[25:40] And you take one of those PCs, maybe a bigger, beefier one, and you put Oracle on it.
[25:47] Maybe it's not a PC. It's a Unix workstation, whatever.
[25:49] But now there's this server on your network that holds your data.
[25:52] And you've got all these PCs networked to it, each running their programs, talking to that data.
[25:58] And that's an interesting new approach because it's cheaper to build out,
[26:02] and it's easier to change. And so it revolutionizes the way business computing happens.
[26:08] Now everybody's got a PC in front of them, gradually. And there are these database servers
[26:14] on the network, new terms. And it's not just one database server.
[26:20] So in my department, I get some budget for my own database server and my own application.
[26:26] And in another part of the business, they want to do their own thing.
[26:30] They're tired of being controlled by the mainframe priesthood.
[26:33] And so they get their own database server and their own application developers,
[26:36] and they're building their own stuff. And so now, all of a sudden, instead
[26:40] of this centralized tower controlled by a priesthood, you've got local control and this flowering of innovation.
[26:48] But oh, crap, your data is everywhere. So what used to be, all of my transactions
[26:54] were done in one database, and I could just do reports in that one place, now the data is everywhere.
[27:00] And so how do I know what's going on in the business? So there's this revolution in application architecture
[27:07] that happens in the '80s. Instead of everything's on the mainframe,
[27:13] we go to a paradigm called client-server, where the client is the PC.
[27:17] There's software running on the PC. The server is the database server
[27:21] somewhere on the network. That's a completely different way to write software,
[27:25] and that breaks the way that we've done analytics. I have questions about this.
[27:33] I also want to catch up on the chat. Graham said, "Southwest was something to do with a storm.
[27:40] Caused a delay. The software couldn't actually handle all the updates
[27:47] to the schedule and crashed." OK.
[27:49] Yay. True story.
[27:51] Both of my daughters were visiting Denver from out of town.
[27:55] No, sorry, one of them was trying to take a trip to visit her in-laws on the East Coast.
[28:00] The flight just got canceled, and they're like, no, we can't have a flight for another week.
[28:04] That didn't happen. The other daughter was trying to fly back to San Diego.
[28:08] They ended up driving. It was crazy.
[28:10] Anyway, go on, sorry. Yeah, no, you're good.
[28:12] And Parasocial can get a database with $5 a month with PHP hosting.
[28:20] Yeah, they're pretty cheap now. Yeah, yeah.
[28:23] And I feel like I'm getting there. So I liked the way--
[28:29] I wish my iPad was working to stream. I'll have to figure this out later.
[28:33] The visual of that Oracle was like the local network database, and then the LAN to everything else,
[28:41] because that also helps why Oracle started. And then the way you said it was a client server,
[28:48] meaning that they ran the software on their own computer but was still asking the database
[28:55] from the local network. Yes, yes.
[28:58] OK. That was the new paradigm.
[29:00] Instead of all of it centered around the mainframe, and you've got a terminal that connects to the main--
[29:06] I mean, we complain about monoliths now. The original monolith was the thing
[29:11] that came before client server. And I was a nerdy teenager in the '80s reading Byte magazine.
[29:18] Anybody of a certain age in the audience will just feel waves of warm nostalgia right now.
[29:25] And at that time, this was the thing that the wild-eyed revolutionaries were
[29:31] carrying the banner and calling people to the barricades to tear down the tyranny of the mainframe
[29:37] and replace it with PCs and LANs and client server. It was really a big thing.
[29:42] It was a revolution in application architecture and in the economics of computing, which is itself
[29:50] is cool. And since we're telling the story of analytics here,
[29:54] it broke the way analytics worked. With that transition, the tools that we had
[30:02] didn't work anymore. And I'm going with context here.
[30:08] And again, this is probably my favorite thing about the show is I will ask what I think are the most simplest questions.
[30:16] And I'm like, I'm actually going to ask them now instead of just hiding and being like, I know it.
[30:22] No, I don't. Mainframe.
[30:25] Is that just the big computers before they went to home computers?
[30:31] Or how would you describe it? Yeah, yeah, yeah.
[30:33] Yeah, it was-- I mean, at first, they were the computers that we were able to make.
[30:42] And they were big and heavy and required special power and everything.
[30:46] And the first digital computers that human beings figured out how to make were large and expensive and physically heavy
[30:56] and needed three-phase power and cooling and all that stuff. So it was the best we could do.
[31:01] And that paradigm of the one giant machine is just the paradigm that we carried forward
[31:07] for about 30 years and just got better and better at it. Like we went from vacuum tubes to transistors, transistors
[31:13] to integrated circuits. We became more modular.
[31:17] And IBM with System 360 and the work of Fred Brooks, the late Fred Brooks, he finally passed away last year,
[31:25] a common operating system that would persist over different versions of the hardware,
[31:30] all that stuff. But the basic idea of a computer is a giant thing
[31:36] that goes in a special room. And you need to cool it and order special power
[31:40] connections, that was the mainframe. And that was the paradigm that just got carried forward
[31:46] for 30 or so years. And Graham said, ha ha, yes, you can.
[31:53] But through input, not scale of tens of thousands of users, this is why we have such complex infrastructure.
[32:02] Yeah, that was, I think, responding to parasocial about the $5 a month.
[32:06] Like that $5 a month database with shared hosting, that works, solves a lot of problems.
[32:11] But some problems it doesn't solve. And this is why you have other systems, yeah.
[32:15] And which is really ironic as now we are going back towards thin clients.
[32:23] Yeah, yeah. And I'll get later on in the story
[32:27] to what I think is happening with application architecture now.
[32:30] I mean, the web disturbed what we meant by client, but we'll get there.
[32:36] And Lerner said, Univac time, and I feel like you did go through that.
[32:42] Was Univac what-- Yeah, yeah.
[32:43] The different-- OK. Wasn't the first mainframe, but it was an early one.
[32:48] Yeah. OK.
[32:49] And then Lerner's just mentioning they didn't know much about computers until middle school,
[32:55] but that's really way after all these machines. I will say I was in the '90s.
[33:02] I was fortunate enough that my dad bought all the latest and greatest things
[33:09] and tried to tinker with them and break them apart. So I got to see a lot of it.
[33:13] But I didn't ask a lot of questions back then. But it's starting to piece together
[33:19] as I have people on the show. I'm like, oh, that's what that was.
[33:23] Or why people would go play StarCraft at a LAN-- Party.
[33:31] Yeah, LAN party cafes, computer cafes. They used to be a thing.
[33:35] But OK, so we got to the point where we have the client server and it still connects to the database on the network.
[33:44] Yeah. And client server is--
[33:49] Graham, I-- Prince of Persia. This is good.
[33:55] This is good. Maybe we'll go there.
[33:59] I don't want to play the I'm old enough game just yet. But client server was compelling economically and technologically
[34:08] and was winning. But the problem now is that all of your data that describes--
[34:13] remember all those transactions happening in the world? And they used to be reflected in that one database.
[34:18] And reporting was just a feature of that program. Now there's dozens of databases that all those transactions
[34:25] for different business units and departments are in with all those different business leaders wanting
[34:31] control over their own application and their own data and having it now because computers are cheap enough
[34:36] and they can put PCs on desks. And so how do you have one view of what's going on?
[34:40] Well, this is where the data warehouse enters. This is a late '80s, early '90s technology.
[34:46] OK. And the idea was, OK, fine, you've
[34:52] got all these departmental databases with all these different transactional schemas
[34:57] all over the place. We're going to write a program that at night--
[35:03] because again, this is kind of a pre-globalized world. And so you do business during the day
[35:09] and then computers sleep at night. At night, we're going to go read all of the transactions that
[35:15] happened in the previous day from all of those databases. They're all in different formats.
[35:19] Everybody's got a different view of the customer, different schema.
[35:23] And we're going to take all that, mush it together, try and unify all the different views of things,
[35:29] and transform the way the data is structured, and then load it all into a completely separate database.
[35:37] That database is called the data warehouse. So you've got all of these departmental databases.
[35:43] We're going to suck all the changes from yesterday out of all of them, transform them into a new format,
[35:48] and dump them into the data warehouse database. Now, that data warehouse database
[35:52] was still like Oracle or whatever. It was another relational database.
[35:57] We're not talking about database technologies in this. But by this time, everything is SQL.
[36:01] Everything is relational, pretty much. That's really starting to win by, say, 1990.
[36:09] But that data warehouse is rising right about then, right around the time of the first Gulf War,
[36:17] if that helps put it in any kind of perspective for anybody. And that now becomes this generation-long paradigm
[36:28] of the way analytics is done. And we had to develop that because of the change
[36:33] in application architecture. People are doing client-server now.
[36:36] There's all these databases, and we need to do this thing to get all that database into one place.
[36:41] So now I can write reports on that. And it's still a batch process, right?
[36:46] It's running at night. I can see what happened yesterday in this morning.
[36:52] I see what happened yesterday. And at that time, this is all oriented
[36:56] around a printed report. So somebody is designing a report
[36:59] in report-designing software, and it gets printed out on a laser printer.
[37:03] And it's still pretty expensive at this point to do all this. So you're still a pretty high-status business leader.
[37:09] Now, lots of different kinds of companies can have computers now.
[37:12] It's not just airlines and banks and utilities and governments.
[37:16] Any even medium-sized business is doing this. But you've got to spend a lot of money.
[37:21] And so you're not doing this for everybody. You're doing this for senior leaders in the organization.
[37:26] They're getting printed reports about what happened yesterday. And that sounds slow by modern standards.
[37:32] But at the time, again, these are wild-eyed revolutionaries blazing a trail, saying, I can get you all that data back
[37:41] that, for the last 10 years, has been locked up in these departmental databases that we've all
[37:45] been getting so excited about. Now I can show you what happened in your business yesterday.
[37:50] And this really sets the tone for the modern era of analytics.
[37:55] This is 30-plus years ago, but we've spent those 30 years working through that paradigm.
[38:05] So I'll pause there for a second. Take us to the modern world.
[38:10] I don't know if you've got questions. I don't know if I have as much questions as much as this
[38:19] is really helping understand a lot more about databases, but also about how we went from just--
[38:35] words, Jen. So I've had different guests on the show
[38:39] to talk about the different types of databases. Or Ben Gamble, who's also from Ivan,
[38:45] he came on the show to talk about just data in general, like from the computers to going all the--
[38:51] so that really helped. And a lot of what you're saying is just
[38:55] piecing these things together. But then also-- and I'm curious to see how analytics were
[39:03] built up and how it's become much more real-time analytics, which we're going to talk about.
[39:09] Because when I worked at GoDaddy, the analytics were still delayed.
[39:16] And when I think about analytics, I think about probably more on the client side of Tableau.
[39:22] Is that what it's called, Tableau? I think so.
[39:24] Tableau, yeah, yeah, yeah. Yeah, so I'm curious to hear more about how that evolves,
[39:34] because why those were still delayed. Are they still delayed?
[39:38] I haven't worked at GoDaddy for five years now, so a lot of things could have changed in the last five years.
[39:44] I'm pretty sure it did. But that's where my head's at right now.
[39:48] And we do have a question from Anthony of, why did Postgres win Relational?
[39:57] I don't have a good answer there. I mean, Lerner, that's true.
[40:02] But MySQL was open source, and it had years of development. And I mean, I think MySQL is how the MySQL folks say it.
[40:12] MySQL might disagree, but I mean, I would agree that Postgres is kind of the de facto choice.
[40:20] So yeah, parasocial, define win. I mean, fair enough.
[40:24] I think it's fair to say that Postgres is the de facto go-to open source relational database.
[40:32] It's not the only good one. But Francisco, I love your thoughts in chat.
[40:38] Seems like you need to, for professional reasons, would want to be thinking about this yourself.
[40:45] So I'm not sure. I'll just say I'm not sure.
[40:49] I feel like Anthony asked that because he knows. So for those who are curious, Anthony
[40:55] is who I like to call my internet big brother. He is the one that--
[41:00] the third person I talked to, and was like, dude, you should live stream, and was my second guest
[41:06] on Teach Gen Tech, so that was lovely. And he likes coming on the streams
[41:11] and asking really difficult questions, which I always find pretty funny.
[41:19] And Francesco is my colleague, but also my own mentor and helping me understand a lot of this,
[41:26] because this is a lot of shit to learn. And then also comparing it to where I work,
[41:33] it's very helpful to be able to balance the two. And yes, there is so much more going in.
[41:41] And I'm glad Francesco loves Postgres, because that is the first one I am tackling.
[41:46] But also, it could also be just because their logo is an elephant, and I love elephants.
[41:53] I feel like that's not a good enough reason, but I'm going to stick with it.
[41:56] It's difficult not to love elephants, Jen. I think that's fair.
[42:02] So we have data warehouses, and we are just on the cliff before we jump off into the web now.
[42:12] So the early to mid '90s, the web starts to happen and changes everybody's life.
[42:18] And we're completely reimagining the ways that we buy dog food and kitchen utensils and deodorant
[42:26] and e-commerce is a thing and the dot-com boom. A lot is happening in terms of the way computers
[42:35] are connected, in terms of the way we access information, blah, blah, blah.
[42:39] Not much is happening in terms of application architecture. The web is hugely transformational,
[42:46] but we are still essentially building client-server systems.
[42:49] The stuff that we learned how to do in the '80s, when the web hits in the '90s, we use all those same tools.
[42:55] And now we build client-server systems. And suddenly, because client-server was small,
[43:01] remember, the whole idea was, I can build something just for my department and have control of it
[43:06] and not the whole company-wide mainframe. Now we're using that paradigm to build websites, some of which
[43:13] become huge. And that's an interesting story, and it's kind of not
[43:20] our story right now. But there's some strain on the client-server paradigm
[43:28] starting to show by 2000, 2005. We're seeing that not always handle everything so well.
[43:35] And the reason why-- you mentioned GoDaddy, Jen, I meant to get to that-- but the analytics were delayed
[43:42] is because everything is a batch process at this point still. You have what happened yesterday, and it's nighttime,
[43:49] and then you load it into the system that lets you see it. So there's transactions happening here.
[43:54] Next day, analytics can happen here. And it's very much a batch world.
[44:01] It was a batch world in 1947, and it's a batch world in 2007. There's not a lot of real-time--
[44:08] I mean, every time I say, real-time analytics is a new idea, if I go tweet that, six people will say,
[44:15] well, I was doing real-time analytics. Yes, of course.
[44:19] People built special things, but it was not a mainstream practice.
[44:23] Analytics was a batch operation. And the strain on the data warehouse--
[44:30] remember, the data warehouse is you collect all this data, you put it into the system.
[44:34] Well, now what we're seeing is not so much that there are lots and lots of systems,
[44:38] but we're back to there's one big, giant website sometimes, and we need to do analytics over all that data.
[44:46] And suddenly, the volume-- it's more common to collect a very large volume of data.
[44:52] You don't have to just be a utility, or an airline, or a bank, or a government.
[44:56] There are these internet startups. There's the dot-com boom and crash.
[45:00] But into the 2000s, still, there are big web companies. And they're seeing that this loading all your data
[45:07] into Oracle to run reports on Oracle just doesn't work. And so Hadoop is born.
[45:15] What a bird? Hadoop is a product, a system, an open source
[45:21] system called Hadoop. OK.
[45:27] Francesco replied to you, and then I'm going to ask you more about Hadoop.
[45:32] I love Postgres, and currently assisting to fast growth in usage.
[45:38] He believes that it's very easy to use. It has a very deep set of extension,
[45:42] covering a wide set of functionalities, and a big, healthy community behind it.
[45:48] I like it. All right, all right.
[45:52] And I'm 100% not going into what the rest of you are saying, because I don't understand it yet.
[45:57] So y'all have fun. And I would sooner--
[46:07] I'm going to let the JavaScript-- I will not enter into a JavaScript debate
[46:13] in a live stream. I mean, every comment is yours.
[46:16] They can have fun. I'm going to leave that, and it's not out of disrespect.
[46:19] It's out of not being qualified. So in about 2010, we have Hadoop, H-A-D-O-O-P.
[46:30] Its logo, Jen, also an elephant. Yeah, yeah, yeah, yeah.
[46:37] And it's not a going concern anymore, OK? It flowered for a couple of years,
[46:42] and we are now dealing with kind of third generation Hadoop's grandchildren.
[46:49] But basically what it did is it said, we can't have just one computer being a database anymore.
[46:54] We have to spread our data out over a cluster, arbitrarily scalable cluster of computers, and then
[47:01] we'll spread our computation all over all those machines. OK.
[47:08] And Parasocial, I love how you are-- you are-- what's the word?
[47:21] You are dropping the hot takes like you don't care. And I love it.
[47:25] Parasocial will post the spiciest stuff. This is the third time-- so first it was databases,
[47:34] then JavaScript, and now you're like, no SQL's over. I mean, I happen to agree that no SQL's over.
[47:39] But I like the spice. I like it a lot.
[47:42] Please continue. Yeah, MapReduce was the future.
[47:46] MapReduce was the future for like five minutes. And it was also a terrible way to live.
[47:53] And I don't want to get into MapReduce. It's to some degree not the point.
[47:58] But nobody used that. Layers developed on top of that.
[48:02] Which, Parasocial, what was the common one? It was Hive, which is--
[48:07] I'm sorry, what's the language that that is again? Oh, yeah, SQL.
[48:11] So yeah, no SQL didn't really-- wasn't really a thing.
[48:19] It was an important movement in database technology. But the attempt to get away from the relational model
[48:23] and from SQL failed. Anyway, slight distraction.
[48:26] I want to stay focused on analytics, because we only have a little bit of time left to get to real time.
[48:30] So this new revolution, these are still batch technologies, just like they
[48:37] have been since commercial computing started in 1947. All right, ish.
[48:42] So Hadoop is now, instead of one big computer that's a database, we have 200 small computers that
[48:50] are acting as a giant database. But you still take your transactions
[48:55] from a little while ago and then load them in. And then you write reports.
[49:03] We're doing the same thing. We're just doing it bigger.
[49:08] Yeah, so that happens. Hadoop itself doesn't survive very long as the technology.
[49:13] But that paradigm, I mean, it's an incredibly fruitful idea. It just gets improved upon in Spark.
[49:21] And now you've got the other things in that whole ecosystem that are all this idea of,
[49:30] the data is going to be out there, and we'll do a bunch of computation on the data
[49:36] out there in S3 or out there on these computers or wherever it is.
[49:40] So around the same time as Hadoop, and for some reason, this just feels like a cheesy thing to say, but--
[49:54] Do it. Mobile devices become a thing, right?
[49:59] I think you just wanted to show the cute picture of you two because you're getting married in 11 days.
[50:04] It is a cute picture. OK.
[50:08] But around that same time, smartphones-- not mobile devices, but smartphones become a thing.
[50:12] And so we're now in a world where we're constantly always connected.
[50:16] You don't go home to get online. You're there, and we get accustomed to the fact
[50:22] that a notification makes the thing in our pocket wiggle when something happens out in the world.
[50:30] So more and more of our social lives and our commercial lives are mediated through computers that are constantly connected.
[50:36] And we develop the expectation that stuff happens instantly. And this also goes into protocols.
[50:47] And when we had POP3 and IMAP on how quickly things were grabbing the information as well.
[50:57] Yeah. I mean, POP3 would be an example of a batch in IMAP.
[51:03] I mean, those are batch technologies, right? Your email client, every so many minutes,
[51:10] has to go check and get stuff and bring it back. So that's like a batch way of doing it.
[51:16] OK. Yeah.
[51:20] And so, yeah, parasocial apps on phones, by implication, notifications in apps on phones.
[51:27] And so we're becoming accustomed to the fact that stuff happens right away.
[51:31] You don't know about something the next day. You know about it right now.
[51:37] Yeah, Graham, we're just about there. I know it's taken a long time, but I like telling the story.
[51:45] Thank you for sticking with us. It's helpful.
[51:47] So y'all, thanks for sticking with because this is going to help me learn and be
[51:51] able to tell other people about it. This is teach gen tech.
[51:55] Jen's taking notes. All right.
[51:59] And remember, I said that that client server paradigm, when the web happened, that's how we built things.
[52:04] So we just kept using that. Well, that's under more and more and more stress.
[52:08] As you get into 2010, 2015-- 2005, 2010, people start complaining in about 2010
[52:17] about this one giant application. You've got this database and this big, giant, complex
[52:23] application that does everything. It's one code base.
[52:28] You deploy it all together. And it's super hard to change and all that.
[52:33] And we start using a negative word for application, that application architecture.
[52:38] We start calling it the monolith. And a monolith is bad.
[52:43] It's the most mustachioed, twirling villain all of a sudden.
[52:48] Around the same time that Hadoop is happening, this paradigm falls out of favor.
[52:52] It's just another way of saying big client server application. But it becomes bad.
[52:59] And so people start breaking their systems apart into small programs that talk to each other,
[53:07] which we call microservices. So--
[53:13] Wait. You've heard the term.
[53:16] Oh, this is weird. Like when something finally starts to click.
[53:23] Oh. Yeah.
[53:25] It kind of made my head hurt. Well, I hope in a good way.
[53:29] Because the reason was, it was too hard to scale and deploy and change and think
[53:35] about the giant monolith. So if you can break that into lots of small programs
[53:41] that are small enough to fit in your head, then each developer can kind of understand the whole thing.
[53:49] And parasocial. I would not-- I would not co-sign that.
[53:56] I would say there are lots and lots of stateful microservices. And well, yes, less state always means your head hurts less.
[54:03] State always has a cost. But the problem is that--
[54:08] and this was a problem when people started making the first microservices systems,
[54:11] that state was really hard to deal with. And so I'm going to go a little teeny bit into Kafka.
[54:16] Just a teeny little bit. Around this time at LinkedIn, this is kind of 2010, 2012,
[54:23] they're making this migration to event-driven architecture, breaking applications into little pieces,
[54:30] wanting data pipelines. And they actually build a system that
[54:34] ends up being called Kafka, because one of the guys who wrote it was a literature minor in college.
[54:40] I never knew that. And just like-- yeah, Jay Kreps is a literature minor.
[54:44] He wrote-- I never knew it was LinkedIn that built it too.
[54:48] Yeah, it was absolutely LinkedIn. Same thing with P&L. So like this
[54:51] is my second company in a row that's LinkedIn infrastructure.
[54:53] But yeah, and he wrote a system before that called SAMSA, which was the surname of I think the guy in Metamorphosis,
[55:01] the guy who turned into the cockroach, Gregor SAMSA. I don't know.
[55:04] I don't know my Kafka, the writer, very well. But anyway, point being, they build Kafka
[55:10] as a way of getting services and data pipelines to exchange messages with each other in a more scalable way.
[55:19] So now you've got big program broken apart into lots of little programs that are shipping events
[55:26] back and forth through logs. And what we have there is another massive change
[55:38] in application architecture. I emphasized this back in the '80s
[55:42] at the client server stuff. We had the mainframe.
[55:46] And now all of a sudden, PCs and a departmental database on the LAN.
[55:50] And I said this was a totally different way of writing software.
[55:53] The internet happened. That didn't even change it.
[55:56] Well, now finally, the internet happened to us hard enough that we start to transition to this event-driven architecture
[56:04] or these little programs exchanging events with one another.
[56:08] You could just call that microservices if you want. And difference-- briefly, parasocial-- difference
[56:17] between queues and logs like Kafka is the log is persistent. Yeah, Robert, I skipped over SOA because I
[56:24] don't want to use bad words. No, I did.
[56:27] That was an attempt to get there. And if I wanted this to be 2 and 1/2 hours long,
[56:32] you're right, I did. I mean, if you want to go into it, I'm down.
[56:37] But I think he's just setting it up that one of you need to come on the show and talk about it now
[56:43] and give a history lesson. And thank you, Owen, for the subscription.
[56:48] Oh, it was from Roy. You're gifting them.
[56:52] Thanks. I appreciate it.
[56:54] Yay. SOA was an early and ultimately failed attempt
[57:01] to do what happened later with Kafka and microservices. And what happened with Kafka and microservices
[57:08] is now, instead of one giant program centered around a single database, we can have lots of little programs
[57:15] that each do a small part of the work and talk to each other through event logs.
[57:21] Now, that's a hugely pregnant statement, and I'm going to mostly just leave it.
[57:25] That's a whole other episode that, honestly, Jen, I could recommend some people who would do a great job.
[57:30] I was going to say, I feel like I need, at some point, someone to be like, OK, you've had people on about each
[57:38] of these, so now what's the difference between event-driven and real-time analytics, even though they're different,
[57:45] but why are they different in those cases? Yeah, yeah, yeah.
[57:48] I'm going to call it right now, Chris Jenkins. You should get Chris Jenkins on event logs.
[57:52] Chris was supposed to be on the show at one point. OK, well, there's a lot of things Chris could talk about.
[57:58] Like, you want-- Please remind Chris.
[58:03] Everybody go remind Chris that he needs to be on the show. And now, Chris, I'm going to insult you.
[58:08] Are you Haskell or Erlang? I get my small population of user purely functional
[58:18] languages confused. That was shade, everybody.
[58:22] Chris is a good programming language guy. He'd be a great guy for event-driven architecture.
[58:26] So anyway, OK, so now microservices. And this is another paradigm change, actual large
[58:46] disruption in the way we build applications. And now I'm talking to people, many of whom
[58:52] have gone through this. So if you were building monoliths for a few years
[58:56] and loving life, and now, all of a sudden, you're refactoring to microservices.
[58:59] You're like, why does life stuck? I don't know how to do this.
[59:02] That's because it's just a different way of doing things. And we're experiencing that together now.
[59:07] And we're making our way through that paradigm shift, like being a mainframe programmer in 1975,
[59:13] and then in 1985, having to be a client server programmer and making that change after years of experience on the job.
[59:20] So it's happening again. And it's a good thing.
[59:24] And it's compelling. And it's going to continue.
[59:27] And you don't all have to do it, but it's happening. And it's a good thing to learn and surf the wave
[59:36] rather than let it crash over you. But what happened last time we had a major change
[59:41] in application architecture? That upset the analytics apple cart.
[59:46] The way we were doing analytics didn't work anymore, which gets us, finally, to real-time analytics.
[59:54] So what's going on here? These two things happened.
[60:01] One, we transitioned to this event-driven microservices application architecture, different way
[60:08] of writing programs, lots of little programs that do one small thing and consume their work from an input
[60:19] log and do things and maybe put an event in an output log. And that's this network of services talking to each other.
[60:27] That's the modern application architecture now, right? And we're building systems that respond right away.
[60:34] They don't just record transactions in a database so somebody can print out a report on a laser printer
[60:41] tomorrow, OK? Yeah, I think 182 was on the radio the first time
[60:48] when that was happening. That's just not what we do anymore.
[60:54] I mean, they just went on tour again. I know.
[60:57] I know. That's why I said the first time.
[60:59] But the tickets are so expensive. Journey is still touring.
[61:04] It's different lead singers. Yeah, yeah, Robert, we turned the database inside out.
[61:11] I like that phrase. That's fun.
[61:13] I like that. It's super great.
[61:14] It's now like you're building your own special purpose database, that's what your system is.
[61:18] And Kafka is the event substrate. And the ways we've been doing analytics, which
[61:27] were now Spark, Snowflake, the data lake, all of these things that are just
[61:36] evolutions of the data warehouse. They're all still ways of taking all of these data sources,
[61:42] dumping them in this central location, and then running reports on it as a batch process.
[61:49] The specifics, the difference between an early '90s data warehouse and a contemporary data lake
[61:54] are meaningful and large differences. I'm not saying that they're really the same thing.
[61:58] But they are essentially both batch technologies and this way of centralizing that data.
[62:06] So what we need now, now that increasingly instead of transactions being stored in a database,
[62:13] transactions are stored in these events in a log that our services are emitting, we
[62:18] need a way of looking back on that log and seeing what's happening.
[62:22] And it can't be a batch process anymore, because all this stuff is happening in real time.
[62:27] So this and LinkedIn built Kafka. And then in 2015, they said, well, it's
[62:36] time for us to build a real-time analytics database, because we've got all these events.
[62:40] And we're not trying to run reports on them. We're not trying to power a dashboard for a leader to see.
[62:47] We're trying to take what's happening in the system right now and expose that to people in the user
[62:56] interface in real time. So what real time means is I load a web page,
[63:01] I click on a thing, I tap on something on my mobile device. Oh, cute picture.
[63:07] And I am kind of synchronously waiting for it to respond. I type in a search term, show me hamburgers near me
[63:17] because I'm hungry. I want to know the average delivery
[63:20] time of the five burger joints within a mile. I'm not going to wait 15 seconds for report processes to run.
[63:28] It needs to be alive and happen right away. So LinkedIn built the original first version of Apache Pino,
[63:35] we'll talk about next time, to be an analytics database that could ingest streaming events and answer
[63:44] queries in, on average, under 100 milliseconds. All of the previous generations of things--
[63:50] and I know I kind of skipped over the data lake. I didn't dwell very long on Hadoop and everything.
[63:54] But it's just a big scalable data warehouse. All of those were designed to power dashboards, which are
[64:01] just reports in a web browser. And if it takes 15, 30 seconds for a query to run, who cares?
[64:08] I just need it to update every once in a while. That's fine.
[64:13] It used to be overnight. At least it's not overnight anymore.
[64:15] It's OK if that process is pretty slow because I'm just an exec looking at a dashboard.
[64:22] But once we're taking data inside the business and exposing it to users in a user interface,
[64:28] now it needs to be fresh, not seconds old. Latency on queries can't be 10 seconds.
[64:37] It has to be 50, 75 milliseconds. And I don't have 15 execs refreshing a dashboard.
[64:49] I have 100,000 users of my application looking for hamburgers right now.
[64:55] And so you've got this massive amount of concurrency. So the shift here--
[65:00] and this happened because of the second pivot in application architecture.
[65:06] We had mainframed client-server, and now we are experiencing client-server to event-driven.
[65:12] Those same things are pushing us in the direction of needing these databases that can handle many,
[65:23] many more concurrent queries than the previous generation, much lower latency, and much fresher data.
[65:30] There is no batch process. You've got your Kafka pipelines.
[65:34] The data has got to come into the database and be available. So there you go.
[65:41] Ah, Robert, that Pat Helland quote. I need to get that guy in my podcast
[65:45] and email him right now, or after we're done. Anyway, that's why real-time analytics.
[65:54] Yeah. Did you see grams of the difference
[65:59] between a data warehouse and a data lake? Yeah, yeah.
[66:04] Right, right. So if you're a data infrastructure person,
[66:10] data warehouse is like saying monolith, right? You're a little embarrassed by it, and you kind of look down,
[66:16] and you know you're supposed to fix it, and some shame, right? That refers to the '90s technology
[66:23] of the one relational database that your ETL process is populating.
[66:30] And maybe it's not overnight, right? Maybe it's every hour.
[66:32] We've got those cycle times shorter. But it's still this batch process,
[66:36] and it's still that old thing. And then you put a BI tool like Tableau or something
[66:40] on top of that. So data warehouse refers to that.
[66:44] It's under the covers. And you know what?
[66:48] You might get people giving you slightly different answers to this, but this is a reasonable answer,
[66:51] and it's my answer. Under the covers, it's a relational database
[66:54] with that star schema version of your enterprise's data in one place.
[67:00] Data lake is-- originally, with Hadoop, it was an HDFS cluster, which was a distributed file system
[67:10] technology. These days, it's probably a bunch of stuff in S3
[67:13] or Azure Blobstore or Cloud Blobstore of your choice. But it's just a bunch of stuff that you
[67:23] dump into that sump of storage, and you don't do a lot of transforming before you put it there.
[67:32] So in the data warehouse, you had this very specialized, carefully thought out process of transforming
[67:37] the transactional schemas in everybody's departmental transactional database
[67:41] into the analytical schema. I said star schema before.
[67:46] You might hear the term snowflake schema into this fact dimension pattern that, again, it's
[67:52] this specialty of doing that transformation. And you're very carefully making that schema translation,
[67:57] writing code to do that, into the data warehouse. In the data lake, you just say, nope, here's the transaction,
[68:03] and there you go into a Parquet file or whatever. You just kind of dump the thing into the lake
[68:09] and worry about transforming the schema later on if you have to. That's the difference between ETL, extract, transform, load,
[68:18] and ELT, extract, load, transform. I think that distinction is a much less revolutionary one
[68:27] than some people have argued, but that's the difference between a warehouse and a data lake.
[68:31] With data lake, you just dump stuff in. You figure it out later.
[68:35] That totally went over my head, but I'm going to come back to it, and I know I can refer back to it.
[68:40] And this was very eye-opening and connecting a lot of the dots, I will say, next week,
[68:50] because you said that we'll have to refer to some of it with Kafka.
[68:55] And maybe you can answer this really quick, because I've asked a lot of people this.
[69:01] Is it Kafka or Kafka? Well, it depends on the accent with which you speak English.
[69:09] And I'm going to say for your accent, which is the same as mine, you are an American speaking standard
[69:15] spoken American English, Kafka. If you're basically anywhere else in the Anglosphere--
[69:22] well, no, if you're like an Aussie or a Kiwi or a Brit, they tend to say Kafka, and it sounds perfectly natural.
[69:28] But for us here in the States, it's Kafka. I actually made a whole video when I was a confluence.
[69:34] It was only internal, but there were these three things. Because some people said confluent,
[69:38] like people from the Midwest and the Great Lakes area, they said confluent.
[69:42] And then the name of the company was Confluent. And so I made this enablement video
[69:47] that said Kafka, confluent. Anyway, it's Kafka.
[69:50] Well, I'm going to probably end up going back and forth, because almost the majority of my colleagues are European.
[69:59] So I hear Kafka, or I don't know, now I need to figure out how to write that down.
[70:06] But that aside, I really like-- I mean, give them that.
[70:11] They get to say it how they want. Yeah, yeah.
[70:15] I like how we talked about going from mainframe to client server to event-driven to real-time analytics.
[70:21] Next week, something that I think would be really helpful, probably already on the plan,
[70:26] is understanding event-driven a bit more. Like, what's an event?
[70:32] Because it makes sense, but not enough, that I think that would be really helpful to build on.
[70:42] Because the rest of it really made breaking this down so much easier and understanding it.
[70:50] So that's definitely something to look into next week. And y'all, next Wednesday, same time, same place.
[70:58] So come join us next Wednesday. Make sure you follow, so that way--
[71:03] and Ryan, thank you for pinning Tim's Twitter account. I appreciate it.
[71:10] And Lerner, thanks for staying awake. And Lerner is, I believe, in India.
[71:18] So it's like 1:30 in the morning. Yeah.
[71:23] Have a good night. Keep learning.
[71:26] Oh, jeez. Thank you, Francesco, for joining today.
[71:31] And yes, everyone, let me see who we should raid to. Oh, Josh is streaming.
[71:38] We're going to go to Josh, because it's always fun to raid to Josh.
[71:41] So y'all are going over there soon. And come back next week, because raiding always takes forever.
[71:50] And I like to make funny noises and looks when I'm waiting. There we go.
[71:54] And-- 
