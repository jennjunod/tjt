---
showLink: "https://www.youtube.com/watch?v=dsYLNcRQtck"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-databases-with-christian-glassiognon"
title: "🎥 Teach Jenn Databases with Christian Glassiognon"
publishDate: "2023-08-17"
coverImage: "https://i.ytimg.com/vi_webp/dsYLNcRQtck/maxresdefault.webp"
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

[00:00] (upbeat music) (upbeat music)
[00:05] (upbeat music) (upbeat music)
[00:10] (upbeat music) (upbeat music)
[00:15] (upbeat music) (upbeat music)
[00:20] (upbeat music) (upbeat music)
[00:26] (upbeat music) (upbeat music)
[00:34] (upbeat music) (upbeat music)
[00:42] (upbeat music) (upbeat music)
[00:50] (upbeat music) (upbeat music)
[00:58] (upbeat music) (upbeat music)
[01:06] (upbeat music) (upbeat music)
[01:15] (upbeat music) (upbeat music)
[01:22] (upbeat music) (upbeat music)
[01:29] (upbeat music) (upbeat music)
[01:37] (upbeat music) (upbeat music)
[01:45] (upbeat music) (upbeat music)
[01:53] (upbeat music) (upbeat music)
[02:01] (upbeat music) (upbeat music)
[02:10] (upbeat music) (upbeat music)
[02:18] (upbeat music) (upbeat music)
[02:26] (upbeat music) (upbeat music)
[02:34] (upbeat music) (upbeat music)
[02:42] (upbeat music) (upbeat music)
[02:51] (upbeat music) (upbeat music)
[02:58] (upbeat music) (upbeat music)
[03:08] (upbeat music) (upbeat music)
[03:13] (upbeat music) (upbeat music)
[03:34] (upbeat music) (upbeat music)
[03:42] (upbeat music) (upbeat music)
[03:49] (upbeat music) (upbeat music)
[03:58] (upbeat music) (upbeat music)
[04:06] (upbeat music) (upbeat music)
[04:14] (upbeat music) (upbeat music)
[04:22] (upbeat music) (upbeat music)
[04:30] (upbeat music) (upbeat music)
[04:39] (upbeat music) - Well, hello, hello, beautiful humans.
[04:58] Welcome to another episode of Teach Gen Tech. And today we have Christian to talk about
[05:07] queries and databases and all the fun things. And we became friends because of Jacob's Twitter spaces.
[05:15] And I think actually Theo is saying that you would be a good person I should talk to
[05:20] about databases. - Yeah, I think so.
[05:23] Can you hear me by the way? - Yeah, I can.
[05:26] - Okay, sweet. - All of you here, Christian.
[05:28] That's the more important part. - Yeah, I think we were both in Twitter spaces
[05:34] where I usually hang out. And you're just like there, bubbly,
[05:40] like excited to talk about databases. And I was like doing database stuff at the time.
[05:43] So yeah, it's like good. I think I met you and I was just like running around
[05:49] San Francisco going to work and then just like sat down and have like an awesome conversation with you,
[05:53] like made my day and then like watch the stream. So yeah, it's pretty cool.
[05:58] It's good to finally be here. - Yes, yes, it has been.
[06:05] Also, everybody calling me out and I love that so many have about like actually like showing up on time
[06:11] and like having consistency. Because I would like not have anyone on the show for a while
[06:18] because I'd like forget or like just life. And now I'm like, oh, I actually have to make this priority
[06:24] of on time so people know when to show up 'cause that's kind of hard.
[06:28] And thank you everyone for joining. We got Lerner and is it Ariel?
[06:36] I feel like I'm looking at it weird. Is that how I say your name?
[06:39] I feel this is like the hardest part about like streaming is I'm always like, me and names.
[06:46] Even if it's like a normal name, I'm gonna be like. And Nick and there should be a leaderboard
[06:55] about starting streams on time. Hey, the stream wasn't on time, but it was,
[07:02] did not burn your ears from how loud the music was gonna be on the countdown that I was so excited I got working.
[07:10] - Yeah, the countdown was pretty loud. - I am glad you saved everybody's ears.
[07:18] And also, so yes, we met on Twitter spaces. You're in San Francisco area.
[07:25] You used to live in Denver, right? - Yes, yeah, I was born and raised in Denver.
[07:30] So that's like, that's still very much like, I guess like home for me in a way.
[07:35] - And it's just funny because between you and Tim Berglund, you both used to live in Denver.
[07:43] When I was in Denver, I didn't realize it. - Yeah.
[07:49] - Until like shortly after you both moved. And I was like, oh.
[07:53] - Yeah, yeah, and then I think you just, do you talk about where you live, by the way?
[07:58] I'm not sure. - Oh yeah, I'm in Phoenix now.
[08:00] - Okay. - Yeah, I'm in Phoenix now, nice and toasty.
[08:04] - Yeah, yeah, so you just like moved. Yeah, so like all the, like us being in Denver
[08:08] at the same time, it's like almost lined up, but just like didn't quite, which is, yeah.
[08:12] - Are you going to Denver Startup Week? Like that's a good time to just get home.
[08:16] - No, I'm not doing any traveling for a while. I'm on a very, yeah.
[08:22] Once, I like, I call my mom sometimes and she's like, oh, like when are you visiting home next?
[08:27] And I'm like, I have no idea. I have no idea anything for like the next three
[08:32] or four months and then everything will settle out and I can like potentially travel again, but yeah, so.
[08:38] - I'm going for Denver Startup Week. One of my talks got accepted.
[08:42] And so I'm very excited to visit again, but at the same time, I'm like,
[08:47] I'm really glad I have a cool job that lets me travel. And you know, I get a, my talk there is for mental health
[08:55] and neurodiversity and tech. And I'm like, I'm very fortunate that work takes care
[09:01] of that for me. And it's pretty cool to be able to talk about Ivan there.
[09:06] But then also since learning about databases, I don't, why do so many people,
[09:12] I feel like databases get a bad rap. - Yeah, I think generally they're like,
[09:20] they're just a very like hard problem. Like they're just, they're incredibly hard.
[09:25] And like, even for me, I've like scratched like the surface of like seeing how like things work.
[09:31] And it's just like an incredibly tough problem. I think only very recently has like the experience
[09:36] around that gotten a lot better. And I think part of that is just like developers
[09:43] have been like wanting it to get better. And so companies are just like sprang up and like,
[09:47] hey, we're gonna make this better. But yeah, they, yeah, they definitely get a better app.
[09:52] And there's also like a lot of like infighting between what is the best one,
[09:55] but that's like with every developer tool. So there's like, you know, like grand factions
[10:01] of like all the people who like Postgres or MySQL or who are like NoSQL and are doing like MongoDB
[10:06] or Dynamo or something like that. Everybody has very strong opinions, so.
[10:10] - So that is probably the one that, and for anybody like in the audience,
[10:16] please also chime in on what are the big differences between MySQL and Postgres
[10:22] and why would one be considered better? I'm still struggling with that one specifically.
[10:28] - Man, I wish this is where I need like a way better understanding of database architecture,
[10:39] but I think the sum of it is MySQL has the potential to be a lot more scalable.
[10:47] And I think when you talk about scalable, it's like, these are the things
[10:50] that like big companies worry about or like big enterprises worry about.
[10:54] Like if you're on a personal project and you're like, should I pick MySQL or Postgres?
[10:57] It's like, you know, honestly you can pick either and you'll probably be happy like with either one
[11:02] unless your project somehow scales super highly. You know, I think at that point, like what provider you pick,
[11:08] how much is it going to cost is like way more important to you than like the actual underlying
[11:14] database management system. But once you start getting to scale,
[11:17] things like how do you shard your database or like how do you,
[11:21] if you decide scale like horizontally or vertically, horizontally meaning you just add
[11:25] more and more database servers and the vertically meaning you just scale,
[11:28] I believe the compute of those servers, like deciding how to do that
[11:32] becomes more and more complicated. - Okay, so this is me like not being in it.
[11:40] What's sharding again, because it's not about your pants and somebody having a bad day.
[11:47] - No. No, so sharding I believe is like,
[11:52] you split your database into sort of multiple different parts
[12:00] and you run them on just different servers, right? So you're just like, you're like, okay,
[12:04] typically databases, not typically, but like when you start off,
[12:07] your database will run on like one server, just one box, and it's all good.
[12:10] And as your service sort of gets bigger and bigger and bigger you need to split it out across multiple different servers
[12:15] in order to make sure that like you can scale properly. This is why like, I'm gonna do my plan scale shilling
[12:22] and I hope I do it properly. Otherwise Sam is going to DM me and be like,
[12:25] ah, you're wrong. But the reason why I'm playing-
[12:28] - And Sam will just have to come on the stream and like, you know, do something as well.
[12:33] - Yeah, I need to do my planet scale shilling properly 'cause I want a database hat.
[12:37] I still have not got a database hat yet. And I just, I need to like email Sam and be like,
[12:41] hey, I want my database hat. - Come on, Sam.
[12:44] Let's do this. - Yeah, so the thing that makes like planet scale
[12:48] at least very nice is that it handles all of the sort of like charting of the database for you,
[12:54] where it'll say, okay, like this database has like reached a certain amount of like load
[12:58] and it will just like split the database up in a way where that load is sort of handled
[13:02] across multiple different servers instead of one server. The hard part about that is just making like,
[13:08] if your data is in multiple different places instead of one place,
[13:11] finding it becomes very difficult, right? Because you need to like orchestrate queries
[13:15] across multiple different servers instead of one server. And so, you know, companies like YouTube
[13:21] who have like reached such a high scale to spend, you know, 10 years building out technology
[13:27] that allows like this to be done efficiently, allows the database to be run like super fast.
[13:32] So it's like databases are just, they're just, they're very, very hard problems.
[13:36] And I've probably butchered like half of these explanations because like I still like understanding
[13:42] how exactly all of this works is still super tough, but yeah, hopefully that's a good overview.
[13:47] - Yeah, yeah, and I appreciate you coming on here because I feel like this is something
[13:54] that Jacob will ask me. And for those who haven't met Jacob,
[14:01] you need to like stop what you're doing and go follow Jacob and go show up on his Twitter spaces
[14:07] 'cause he's also just super fun to poke fun at, but he is, and tell him how lovely of a human he is.
[14:15] But he also is someone that challenges me the most and it drives me bananas 'cause he'll be like,
[14:21] Jen, why are you learning Postgres? Why Postgres?
[14:24] Why SQL? Why not know SQL?
[14:27] And I'm just like, I don't know yet because I don't understand,
[14:31] but having him ask me these questions helps me quite a bit with like understanding
[14:38] and realizing that it may make sense if somebody explains it to me,
[14:42] but it doesn't always make sense explaining it to others, which is a challenge.
[14:48] So I totally appreciate you going through that. Oh, geez, I don't think I want to ask that, Nick.
[14:57] You ask him. (Nick laughs)
[15:01] Oh, geez. Okay, well, anyway.
[15:04] So how did you get into databases and data morality? - I still feel very, very new to all of it, to be honest,
[15:14] but basically I was at, I worked at a company called Courier, which I left in May.
[15:22] And while I was there, we were sort of like working on launching a new product.
[15:26] We were going and just like changing a bunch of how the database works.
[15:29] So I was just going and like learning how DynamoDB worked and reading like over AWS documentation.
[15:37] And AWS is like very, very, they're very thorough with their documentation,
[15:41] but like, you know, you have a week to ship a feature or we were running out of time to ship a feature.
[15:47] And it was like, okay, I need to learn how DynamoDB works and all of its complexities and how to scale it properly
[15:52] and, you know, how to design it properly. So I don't like hot key a table
[15:57] and hot keying a table just means that there's a certain like set of data that you're trying to access.
[16:03] Dynamo just has a bunch of specific design patterns where if you break a few of the rules,
[16:07] your entire database slows down. Dynamo is also connected to other parts
[16:13] or other services in AWS. So if you slow down Dynamo,
[16:17] you end up slowing down like other services as well, which is fun.
[16:20] So you have like a very fun cascading effect. But I was trying to learn how to do all of that
[16:26] in like a very short amount of time. And when I sort of like looked to see if there were
[16:31] like any tools to like solve this problem for me, it was just, and yeah, it is a,
[16:37] it's not necessarily a document database, but it is like a NoSQL database.
[16:46] I think like a document database is like a little bit different.
[16:51] Learner, sorry, just talking to chat. But anyway, so yeah, I was like sort of going through
[16:55] and doing all of this. I was looking for a tool that would solve this problem
[16:59] and then I just didn't find one. And then I sort of realized like a lot of like the way
[17:04] that you design databases is in code. And there's this sort of like weird bridge
[17:07] between like the code that you write in your database and like where your database is actually hosted.
[17:11] So I started like trying to learn all of this and solve these problems.
[17:14] And then eventually like left Courier, like started a company to like do all of these things.
[17:21] To solve, wow, reading chat and talking is super difficult. Respect to all the streamers.
[17:25] I'm sorry, I'm just realizing this now. - You're good, you're good.
[17:29] But really quick, I wanted to ask what was the database called?
[17:32] 'Cause I look at- - Oh, it's called Dynamo. - And I was like, is that dinosaur?
[17:36] So I'm just kind of like pause really quick and make sure Dynamo, Dynamo, hey, I can, I can.
[17:43] So this is what we are talking about. I will link it.
[17:49] Yeah, I dropped it in the chat. So it's, yeah, it's most commonly used,
[17:57] I think by people who are like doing a lot of serverless stuff on AWS.
[18:03] It's a fantastic database, super scalable. You just basically, if you set it up properly,
[18:08] you never have to worry about scale ever. But you also, when you do set it up,
[18:14] it is very, very hard to change in certain ways. So you get the scale,
[18:21] but you also just like can't mess with it at all, which is very fun.
[18:24] - And yes, having so many streaming and replying and typing and yes, it's a lot of fun streaming.
[18:37] And this is why I'll be like delayed. I feel very fortunate 'cause Learner will just
[18:42] like ask me a question again, if I like forgot, like spaced replying or I'll just like cut off
[18:49] what I'm doing and like cut someone off to reply to it. And I'll be like, oh yeah, there we go.
[18:54] This is good, this is good. So you're doing great and replying
[19:00] and thank you for putting it in the chat. Okay, now, if it's a NoSQL,
[19:07] how and why did you learn SQL queries? - So for me, when I was sort of thinking
[19:14] about like what I should build or the problems that I should solve,
[19:19] initially it started off just being like, okay, I'm going to build like a really good DynamoDB studio.
[19:24] And then I just sort of thought, well, like all of the customers for that
[19:28] are like super limited and also, well, they're not necessarily super limited,
[19:32] but there's just like a very limited subset of people using Dynamo and sales process
[19:37] and all that stuff is hard. But I eventually just like went
[19:41] and I had been like familiar with using PlanScale, I use it on a bunch of like my personal projects
[19:46] and sort of when I was like explaining the idea of like what I wanted to do,
[19:50] like talk to a bunch of people. And I was like, okay, I'll make,
[19:54] PlanScale like makes migration super easy with Prisma. So I'll just build you like a way
[19:59] to do database migrations in SQL, because that seems to be something
[20:03] that is like really hard to do. So you can like look at your SQL schema,
[20:06] understand it and like make changes to it. And then I just got suggested,
[20:10] I'm pretty sure by Theo to just start with PlanScale, which ended up being like a very good decision
[20:16] for a multitude of reasons. It's why I like, I bring up PlanScale a lot
[20:20] when I talk about databases, but I like genuinely love that product.
[20:23] It's very good. It just solves like a lot of different problems.
[20:27] I better get this database hat. I'm gonna send this entire stream to Sam
[20:31] and I'm gonna be like-- - Do it, do it. - I better get that hat.
[20:35] - And then well, just Sam, so that way you know, Christian's doing amazing.
[20:39] And now Sam, you need to be on the show as well. - Yeah, yeah, that'd be fun.
[20:43] Sam's pretty cool. - Because that's actually happened
[20:46] when Bakari was on my show. At the very beginning, he was talking about,
[20:52] shit, Square, I think Square. And so somebody from Square actually joined in
[21:01] and came on the stream after him too, because it was cool seeing the progression of it.
[21:05] So yeah. - Yeah, yeah.
[21:08] So yeah, that's sort of like why like SQL I guess is just because, yeah, there's just,
[21:14] there are definitely problems in NoSQL land and actually I might end up building some tools
[21:20] for those databases, but just in SQL land, it's like a lot of the problems were there.
[21:28] Also, when I was talking to a lot of people, a lot of people were moving to Drizzle
[21:38] and Drizzle at the time didn't have a studio. They didn't have a studio, which is pretty cool.
[21:42] And so it was just sort of like building for that because again, I had also missed
[21:45] like having Prisma Studio around. Like going and like having one place
[21:51] where your data is easily accessible is like so nice. I've like out of, so I've worked at like three companies,
[21:58] which is not that many companies, but I started off actually being a software tester
[22:04] and I worked at a company called Maxar as a contractor. And so I, with them, I was like doing testing
[22:12] for their image ordering service. They do satellite imagery.
[22:15] And so I just like have to go and like see a bunch of logs, find all like the data within those logs.
[22:20] That was always like a fun process, like tracking down IDs and then sticking stuff into,
[22:25] it wasn't Insomnia, but Insomnia's competitor. I don't know why I'm forgetting their name,
[22:30] but just like finding and like hunting for data was all they did there.
[22:33] And then when I left and I went to the first startup that I worked at, Hyper, it was like,
[22:38] again, doing the same thing. - Postman?
[22:39] - Yeah. - Yeah, okay.
[22:41] - It was like going in, finding data, updating data. And they, we were using a tool called Compass
[22:47] and like Compass was fine, but it was like slow to start and a little buggy and had all these issues.
[22:51] And then even going to Courier, it's like we have their notification infrastructure service.
[22:57] So, you know, we would go through and like, if you sent a message tracing,
[23:01] like how that message went through all of the services in the database is like hard to find.
[23:05] So they're just like all of these problems with like finding data.
[23:09] And it's just like mildly frustrating enough for me to be like, all right, we're gonna do this
[23:14] and like solve this problem. And SQL just happens to be like a really good place
[23:17] to do it, I think so. Or doing it for relational database, it's just like, yeah.
[23:22] - Very cool. And to fill in some gaps to make sure also my understanding
[23:28] is PlanetScale is my SQL and they're built upon MySQL,
[23:36] where like Mongo and some other ones are actually not built on top of like Postgres
[23:44] or MySQL or anything. They are their own like Mongo.
[23:47] They're their own type of databases. And so like Ivan uses all open source platforms
[23:55] like Postgres or MySQL or Redis and Kafka and lets them build upon each other.
[24:02] Where like Confluent is Kafka only, StarTree is Pino.
[24:08] And so that's something that was very hard for me to understand was,
[24:15] and like ClickHouse is ClickHouse. All these databases and they all do different things
[24:21] is realizing that sometimes a company is building upon a certain database
[24:27] rather than its own specific database. If that made sense out loud.
[24:34] - Yeah, yeah. So yeah, MongoDB is just like pure MongoDB.
[24:40] I'm not honestly sure. I don't fully understand how they work,
[24:44] but yeah, they're like their own separate database. Whereas like you said, Ivan hosts MySQL
[24:51] and they host Postgres and they host like Redis databases and whatnot.
[24:55] And then yeah, PlanetScale is in this weird, PlanetScale and like NEON and other providers.
[25:01] NEON is in this weird, like they're building their own infrastructure.
[25:04] PlanetScale uses MySQL, but they're like built on top of Vitesse,
[25:11] which is this like database charting sort of orchestration thing
[25:15] where they like let you host your database and like scale it very highly.
[25:18] So yeah, there's all these sorts of ways. There's like your database management system.
[25:23] So Postgres and MySQL on the relational side at least. And then there's like where you host it
[25:29] and there's a bunch of intricacies there or the technologies you build on top of it.
[25:33] So yeah. - And as a heads up for all of our new joiners,
[25:39] first off, definitely click follow because I talk about databases a ton.
[25:42] Like that's a big part of the show because, and the reason I say that is I work at Ivan.
[25:49] So I started working at Ivan, which is the open source data platform for everyone.
[25:55] And I'm working on getting it down. And a lot of my learning is,
[26:03] I'm curious about databases in general. A lot of what I learn about, I compare.
[26:08] So that way to Ivan, so that way I actually understand
[26:11] what the company I do does better. But that is to say that like,
[26:17] I'm still forming my opinions to understand the tech. It's so vast.
[26:22] Like we just talked about so many different databases that six months ago I would have been like,
[26:27] what did you just say to me? That would have been like almost all of it.
[26:33] So linked in the chat has been all the resources we've talked about, all the tools.
[26:41] Nick, you put, I don't even know how to say it. HTTP IE.
[26:48] Is that like, does it have an actual name? Like, do you say it like that?
[26:55] Hipty, hipty? - I have no idea.
[26:59] - Oh, this is, I think he was talking about like postman competitors.
[27:05] - Yeah. Can you link those in there just so that way
[27:07] we have the links if we want to? - Yep, there we go.
[27:12] - Oh, hey, thanks. That works.
[27:14] Very cool. Okay, so we've talked a lot about background.
[27:17] We've talked about some theory. We've talked about like how you got there.
[27:21] As a quick one for everybody else, I ended up working at Ivan throughout
[27:30] like with Teach Gen Tech. This stream, it's been around a little over a year.
[27:34] And I was kind of going wherever people showed up on this show.
[27:38] I was like, teach me all the things 'cause I don't know what to learn.
[27:40] And I was applying for jobs and I had an interview with the team at Ivan.
[27:48] And I was just like, why are databases so cool? Like, it's the first thing I got excited about.
[27:54] And I was like, I don't understand why databases are so cool.
[27:56] And then I realized that a lot of people don't talk about databases
[28:01] and they don't like databases. They find them very boring as well.
[28:05] And I'm like, but they're so fascinating and they store all your stuff
[28:08] and they do all the things. And so, of course, that in turn came to falling in love
[28:15] with databases, specifically Postgres for myself. That one was because A, it was the first one I learned,
[28:22] which I feel like a lot of us fall in love with a lot of our first loves.
[28:26] And also it's an elephant. I love elephants.
[28:30] They're my favorite, absolute favorite. So that was an easy one.
[28:34] And between that and Josh Goldberg coming on the show like once a month to do TypeScript,
[28:41] my land fell into falling in love with Postgres and TypeScript.
[28:44] But they don't go together unless there's a lot of things in between it.
[28:48] And yeah, I don't know queries very well. And here's probably gonna be the,
[28:54] like, I feel like this is the simplest yet hardest question.
[28:57] What is a query? - So, best way to answer this is,
[29:07] so SQL is called like the structured queried language, query language, right?
[29:12] It's like a standard that's used across a bunch of different databases.
[29:15] It's like a, I believe it's an ANSI standard. Don't ask me what ANSI stands for.
[29:19] But it's like, it's a standard that is established by like one of the governments.
[29:23] And it basically is like a bunch of, like essentially a bunch of different words
[29:29] used to talk to the database, right? And you can do there,
[29:36] every database does it a little bit differently, right? So there are certain commands available in MySQL
[29:41] that are not available in Postgres. But generally there's like a bunch of like standard statements
[29:48] like the select statement, like a select statement will always work
[29:51] like basically with every like database that you'll ever run into that runs a SQL.
[29:56] So SQL is not, by the way, your like underlying database. It's just the language you use to talk to your database.
[30:05] So you can have like a relational database that speaks something that is not SQL,
[30:11] but they're not very common. - I'm pasting along the way,
[30:16] as you're explaining things, I'm Googling. I'm pasting them in here.
[30:20] - Sweet, yeah. Yeah, so that's--
[30:25] - That's not a, Learnr, Learnr, you're gonna have to be on the show someday,
[30:28] especially 'cause you stay up so late. Y'all, it's like midnight in where Learnr is.
[30:34] Anything with SQL that's not a procedural block is a query. - Yeah, oh, and he links the anti-standard suite.
[30:42] - Oh, hey. - That's cool.
[30:48] - Yeah, so. - I'm looking at it really quick.
[30:56] Okay, we got an idea of what a query is then, and it's, and using SQL is,
[31:05] the way that it's been explained to me, and I'm not sure if this is accurate,
[31:10] is that it is a language then, because it's a way it's talking to a database.
[31:17] - Yes. Yeah, it's,
[31:19] yes, it's a language that is actually very nice to work with, I believe.
[31:26] When I went and reviewed all of this, 'cause I spent a little bit of time yesterday,
[31:29] it's based on some sort of math. I didn't have enough time to dig into it deeper,
[31:33] but it's very, it's pretty interesting. Also, the reason why it's nice, it's,
[31:38] yeah, it's very English-like. Also, it ignores whitespaces.
[31:41] So do you have, I guess I could pull one up. If you have a SQL editor,
[31:45] and you type in a SQL command, right? You can make it,
[31:50] you can make it multiple lines very easily, which makes it very, very readable.
[31:56] Yeah, so it ignores whitespaces, which is pretty nice. - The Googles and I, I don't have one.
[32:07] If you have one that you may suggest. - Can I share my screen, is that possible?
[32:12] - Yeah, for sure. It should be down. - It's giving me a warning.
[32:16] Okay, is there anything on my computer I don't want people to see?
[32:19] No. - Oh, that's good, I'm glad it gives you a warning.
[32:23] - Yeah, it's like, this is done best on two monitors. I'm like, ah, okay.
[32:27] - Really funny for everyone. When I first started streaming, I shared my screen,
[32:35] and I shared, I didn't realize Twitter was up, and I'm new to Twitter, so I don't even know
[32:40] that Twitter's even that cool or anything. And all my DMs were open.
[32:45] So luckily, back then, only it's like, A, I didn't actually have real conversations like I do now,
[32:52] or privacy and things like that. And I'm like, oh, okay, now I know.
[32:57] And I won't do that in the future. - Yeah. - Ooh, okay, cool.
[33:02] - Sweet, so yeah, so this is my SQL editor and whatnot. And the thing I was trying to say is the nice part
[33:12] is this command works the same way. So if you have a very long query,
[33:18] because it ignores white spaces, you can just make it very big
[33:21] and add a bunch of stuff under it, and it will still work properly.
[33:24] So very English-like, very easy to work with. Used in a little bit like SQL Fiddle, kind of, yeah.
[33:32] So yeah, it's very easy to work with, works across a bunch of different things.
[33:38] And it works, this is not only for, so databases like Postgres and whatnot,
[33:48] you might think of them as like, oh, I can only use this to sort of work with data
[33:54] in production for an application. But SQL's also used a ton
[33:58] in data warehouses and all that stuff. So learning it as a language is actually very useful.
[34:04] I will tell you, when I was at Queryer as well, we had to go and figure out
[34:13] what users were using a specific feature we'd just built. And so we would go and use SQL to query data
[34:19] in our data warehouse that came from no SQL databases as well, which is fun.
[34:23] So you'll pipe it in, transform it into something that can be stored in a relational database system,
[34:28] and then use SQL to query it. That is how good of a sort of language
[34:33] it is to work with data. - Very cool.
[34:37] And just to take a pause really quick, y'all don't get to know what this is yet,
[34:43] but what we're seeing right now, Christian will be on later on to talk about it.
[34:48] And I'm very, very excited. And I have a feeling, Christian may not know this,
[34:54] but that he'll need to be on the show more often to talk about this kind of stuff, but we'll see.
[34:59] So that's very cool. And thank you for explaining this as well,
[35:05] because when Lerner said that it's very English-like, I didn't quite know what that meant.
[35:13] Especially because even earlier today, I was talking to someone from the women in Postgres team,
[35:22] and she was talking about how it's hard for a lot of engineers to learn SQL, Postgres,
[35:31] or MySQL, or any of them, because they are not as much like a computer language
[35:37] as they are like a spoken language. - Yes.
[35:42] Yeah. Yeah, and it's super, English is a very funny language.
[35:45] So it's like having an, yeah. It definitely is a lot more of a spoken language.
[35:50] My face lit up too, because I have a hat, a Postgres hat that is somewhere in my stuff
[35:57] that I haven't unpacked yet. And I'm pretty sure I got it
[35:59] from potentially the person you talked to. I forget her name as well, which really, really sucks,
[36:04] but yeah, thank you for that hat, if she somehow ever sees this.
[36:07] - I will tell her, I'll be like, hey, look, I'm learning. I'm learning, 'cause I'm gonna apply
[36:13] for Postgres Europe, Postgres Conference Europe to see, and I'm like, really excited,
[36:21] 'cause I don't know these texts yet, and that's something that I heard a lot of people do,
[36:25] is they'll apply for conferences about tech they wanna learn.
[36:28] - Yeah. - And I'm like.
[36:31] - One thing too is, yeah, one thing too is syntax, or I guess the syntax of SQL,
[36:37] that when I was sort of doing a summary review, I thought it was like a good way to explain it is like,
[36:42] generally your SQL commands will follow like what you want to do.
[36:45] So like select, update, delete, insert, and then sort of like on what piece of data.
[36:52] So from like what table, and then it'll go to like limited by what.
[36:58] So it'll be like, I want to update these rows that match this specific requirement.
[37:04] And then if you're like selecting rows, if you're getting a bunch of rows,
[37:07] it will also have the option of like, how do you want to organize them?
[37:10] So do you want to group rows by the specific ID? Do you want to sort of order rows by a specific thing?
[37:19] That's like a good way to like sort of think about that. So it's like, what do you want to do?
[37:24] On what sets of data do you want to do it on? Do you need to limit it by anything?
[37:29] And then how do you want to like, if you are getting rows of data,
[37:32] how do you want to like organize this data? - Okay.
[37:36] Here. 'Cause I've done this before in the past where like,
[37:47] let's see if it'll come up. I need to start doing it a different way.
[37:50] So that way like everybody can edit it, but. So like you said that there's three parts.
[37:57] It's, I hope I put my pen the right way. There's, what do you want to do?
[38:04] Do you want to do? To do, we can finish writing.
[38:13] What data? Is that the second one you said?
[38:18] - Yeah, on what data or sort of like, where do you want to do it?
[38:23] So like what table basically? - Okay.
[38:26] What table, AKA where? And then what was the third one?
[38:34] - I have such short memory. Limited by what?
[38:39] - Okay, what does that mean? One more time.
[38:48] - Okay. - So limited by what meaning?
[38:52] If you run like a SQL command with no limits, it will run on every single row of your table.
[38:59] So there's a very, actually can I share my screen again? We can show this.
[39:04] - Yeah, for sure. - Okay.
[39:05] I really need a dummy database, but it's okay. I'll do it on a table that doesn't matter.
[39:13] So if I go, we can go. Okay, so we have like all of these sort of rows
[39:27] in this sort of table that I have just to do experiments. So if I say like delete from,
[39:35] so delete is just like your SQL command. From is just the sort of,
[39:43] the word used to, why am I having such a hard time explaining this?
[39:50] Like delete from is- - The word to remove something?
[39:54] - No, it's the word. It's basically like when you're saying from is like,
[39:59] you were saying where you're going to do this action. So delete is the command and remove is the sort of thing
[40:05] saying, okay, I'm going to do this on this piece of data. Does that make sense?
[40:12] Hopefully, I'm like butchering this explanation. - No, you're good, you're good.
[40:16] I think this is, I'm also processing on like- - If I say select from, the next word after from
[40:26] is generally the name of the table that I'm getting things from.
[40:29] - What is the star? And are the stars always needed?
[40:36] 'Cause I feel like I got very stuck on stars and question marks lately.
[40:41] - Yeah, so no, the stars are not needed. The reason why it's there is it's to say
[40:49] that I'm selecting every single column from the table. - Okay. - So I can select
[40:55] specific columns. I think you do have to specify what you want.
[41:00] So like you either have to have the star, I believe, or you have to specify the column names.
[41:04] So I can say, if I just wanted the IDs from this table, I could like run this command
[41:10] and it would give me only the IDs from the table. And then- - And then alpha
[41:17] is the table, right? The table name?
[41:19] - Yep. - Okay. - So yeah, so select is like,
[41:26] by the way, I write all of these things lowercase, but SQL is not case sensitive with its commands.
[41:36] So like these two things, these two statements, same statement.
[41:45] You might see like SQL written in all caps or you might see it written lowercase.
[41:51] I write it in lowercase just because, yeah. Sometimes it's nice to write it like fully uppercase
[41:57] just to like have, to sort of like see the statements be a little bit different from the data
[42:04] that you're actually using, right? So it's like, let's say if you had like
[42:07] a really long SQL query, like select alpha from where ID is one.
[42:13] And you like this, we're gonna go on and on and on. Sometimes it's nice because then you can see the things,
[42:19] like the pieces of data you're actually working with versus like the SQL that you're writing,
[42:23] if that makes sense. - Yes.
[42:27] You should add a syntax highlighter. Okay. - Yeah.
[42:34] - Yes. - And a learner says they prefer to keep keywords
[42:41] in uppercase as they've seen that used in most places, including work.
[42:46] And I've seen it that way too. I think for myself, I probably will end up,
[42:53] I ended up putting them lowercase because for some reason until today,
[42:58] it didn't really distinctly stick that it's not the same as a coding language,
[43:04] like JavaScript, for example. 'Cause you know how JavaScript, you don't always,
[43:08] like half the time words are smooshed together and or have like quotes around them or a bracket.
[43:16] And I'm like, and to say this is like English, which it is, there's spaces, it's full words.
[43:23] I'm like, this makes my head, it's like, it's easier that it makes my head hurt more.
[43:28] - Yeah, yeah, yeah. Okay, so select ID, name from.
[43:38] Is name another column or a row or? - Yeah, so I forget, let me do describe.
[43:48] So MySQL has a command called describe where you can like describe a specific table.
[43:55] And so this table has four columns. It has a column called ID, column called name, age, object.
[44:03] And then it will give you the type of the column, right? And it will say, okay, like this is int,
[44:10] so it's an integer or a number. This is varchar, which is a variable amount of characters.
[44:18] So this is like in JavaScript, this would be a string, but you see it has like 50 here,
[44:26] it's limited by 50 characters. So if I were to, if you were to try to add a value
[44:33] into a row, into the name column that was over 50 characters, it would like reject it.
[44:40] And you do this to like save space in your database. And also like smaller sets of values
[44:50] are like also easier to search. They're more easily indexable as well, all that fun stuff.
[44:54] - And then Nick just said, are those code points just like JavaScript strings?
[45:04] And Lerner said, not code points, but sizes. - What are?
[45:12] - Does this all make sense to you? - Are those code points like in JS strings?
[45:18] Oh, not fully. Oh yeah, okay, I see what they're saying.
[45:27] No, no, this is like, yeah, this is in the number of characters.
[45:33] JavaScript, I don't think is, JavaScript is never strict in like
[45:37] what size something should be, unless it's, no, it's not strict, I don't think anywhere
[45:42] for like what size something should be. You can like make something like a thousand.
[45:46] Like you can make a very, very long string in JavaScript and it would just be fine.
[45:51] Whereas in here, like you have to define what size everything is.
[45:56] - And we're, right now we're doing everything in MySQL, right?
[45:59] - Yes, and even for Postgres, it's the same way. The data types for Postgres are a little different.
[46:04] - I was gonna say, I think the data type for Postgres is text.
[46:08] - Yes. - And that's why I was asking,
[46:12] 'cause I was like, I get it. And I think it's a little different
[46:15] just because I've been doing a lot of my stuff and like PgAdmin as my tool to be able to view everything.
[46:24] Oh, for example, an emoji is one chart with multiple code points.
[46:28] Oh, yeah. No, this is just in like number of characters.
[46:35] I wonder actually what size an emoji would be if I stuck it into a database.
[46:40] But I think emojis are, forget how these work,
[46:45] but like emojis and special characters are, like when they're represented in certain places
[46:51] end up being like that sort of four character starting like with an ampersand
[46:56] and then the sort of like set of numbers that you have representing that special character.
[47:05] Yeah. - This is all making sense.
[47:12] - I hope so. - Yeah, yeah, yeah.
[47:15] It's also just like a lot of like processing as well in the fact that,
[47:21] and you have this up on another screen and I just wanna call out,
[47:26] this is something, and I appreciate you going through this with me,
[47:29] is it is pretty easy to Google SQL queries and like what you wanna do,
[47:36] but actually understanding what you're typing and what each section is not as easy,
[47:42] especially when it's like, you mentioned earlier that if you wanted to write
[47:46] like a really long query, what is a time that you've had to write really long queries
[47:53] and can you give us an example around that? - Yeah, so generally all the queries that I use
[47:58] like in my application are pretty small. The longest query that I've had to write
[48:05] was that query that I had to write at Courier, which man, that did a lot of things,
[48:12] at least for me, because I just had never had to do it before.
[48:16] So at Courier, I wish I could draw this out somehow. So at Courier, we were trying to figure out
[48:22] how many people had used a specific version of a product of the previous products that we were building.
[48:31] So I helped to build a product called Preferences at Courier. Let's say you get an email sent to you
[48:36] and you want to unsubscribe from it, Courier handles all the unsubscribing logic,
[48:41] handles all of the behavior around that. And so we had a few different versions of it.
[48:47] We were launching the newest version, V4 Preferences, and we wanted to go see how many people
[48:52] had used the previous versions. So in order to do that,
[48:55] because it was in multiple different places, I had to like make a query that went to our users table
[49:01] and I wonder, yeah, this should be okay to talk about. I shouldn't get emailed about this.
[49:06] Went to our users table and then like searched for a specific property
[49:10] in the users table. That property was in JSON.
[49:13] So I had to like take that JSON and break it out and do like snowflake supports,
[49:18] searching within JSON objects, I believe, or like filtering within them.
[49:22] So like I had to like go, like take that piece of JSON, break it out,
[49:28] search for a specific property in that piece of JSON, join it with another table.
[49:33] And then I think I had to join it with one more table after that.
[49:36] And so doing all of that was a bunch of lines, but once it was done, it was done.
[49:43] - Yeah. - What?
[49:48] I think that's a great call out of like, why would somebody put JSON into a database?
[49:58] Because I'm like, isn't JSON kind of like its own database? - JSON is really just a way of like structuring data.
[50:11] So it's just a bunch of keys and then a bunch of values. This sort of pattern is mirrored in a lot of databases,
[50:19] right? So like, for example,
[50:21] Cloudflare has something called workers KB and it's a key value store.
[50:25] Dynamo is a key value store. So you just have like a piece of sort of something
[50:30] to identify the data and then the actual value of the data.
[50:34] - Okay. - And then JSON is just the specific sort of notation
[50:40] that it uses because it's like human readable and all that fun stuff.
[50:44] - Interesting. Okay.
[50:48] 'Cause I was like, for some reason I always thought they were pretty similar.
[50:52] - Yeah. - Almost like the same thing that,
[50:56] and I always got very confused on why somebody would want to put it in there.
[51:02] - Yeah. It's similar in terms of like the way that you store things,
[51:07] just different in terms of like what you do with it.
[51:11] The reason why we had JSON in our database and there's JSON even in my database.
[51:16] Well, in courier's case, courier was using DynamoDB.
[51:21] And so all of the values were stored in JSON. They don't necessarily have to be stored in JSON,
[51:27] but we were using JavaScript and it's sort of like a good pairing there.
[51:31] And so when we were taking that data and putting it into Snowflake,
[51:35] Snowflake is our data warehouse that I use to like query all of these things.
[51:40] It was just like JSON in a SQL database, which is okay in that aspect.
[51:48] If you're doing like, if you're using,
[51:50] if you're storing JSON and you're using it for an application,
[51:53] like it's like less good because SQL databases don't handle JSON very well.
[52:01] It tends to be a lot of data in sort of one place. And you want to split that out to make it,
[52:08] like easy to query, but yeah. Hopefully that answers your question.
[52:12] - It did, it did. And I think that's something that I'm like, okay, cool.
[52:16] Like that is something to start to noodle on and think on because I,
[52:23] we'll see if you sign up for this or not. I know I might get one more Ali stream out of you,
[52:28] but to go into more detail, because this has helped a lot
[52:33] with like just getting on stuck on some of the,
[52:37] what each of the areas mean, because I think it's very difficult to know,
[52:43] like, for example, the first part is a command.
[52:50] Okay, cool. I wouldn't have known that to know,
[52:53] oh, I need to Google and figure out what command I need to use.
[52:57] Or, you know, the same with like the asterisk is calling out the column name,
[53:03] which might sound a little silly, but Ilyan, Alian, E, Diddy.
[53:11] I'm gonna just like try to come up with so many different names for you
[53:18] until you're on the stream. So that way I actually call you the proper name.
[53:23] Oh, it's gotten bad. Like every single time he joins,
[53:28] I'm always like, your name changed again. I'm not great at names as we've talked about in general,
[53:34] but yes, I'm very excited. If it helps, I can send you some new dates as well,
[53:43] because I don't know if it shows them all yet. But all right, we talked a lot about the basics
[53:51] and I know we got to like the column name kit. Do you have an example where we could be like,
[54:00] ooh, yay, some juicy Astro three, version three content. What, I'll say it like this.
[54:14] If somebody has a blog and you know, they have like categories or tags
[54:20] or they want to add more information. Sorry, I'm hitting my mic now.
[54:24] What, like how would somebody query something like that properly?
[54:29] If they want to search specific categories or if they want to only do something from like X date.
[54:38] I feel like that's kind of confusing and putting it into like real usage.
[54:45] - Yeah, let's see if this dummy database has that sort of data.
[54:51] It sort of does. So based on that, it would sort of be like the same process
[54:59] of saying like, what, like, okay, sweet. So how do I explain this?
[55:06] So if you have like a blog and you want to like get it from categories,
[55:11] it would really depend on like how your database is set up. But like, let's say, let's use sort of this dummy database
[55:18] as an example, because it's here. And like, let's say you had, you have a bunch of actors.
[55:24] What's a good one that we can show a joint off. Okay, okay, here's a good one.
[55:29] You have a bunch of addresses and let's say you want to get every address
[55:37] from a specific city, right? What you would do is you would like say, okay,
[55:45] well, I know that all the addresses are stored in one table. So you would say like select,
[55:50] and then you would sort of figure out what information you need or what columns you need
[55:54] and specify that. If you need all of the columns,
[55:56] you would just sort of have the asterisk. And then you would say, where do I want to get this from?
[56:01] I want to get it from the address table. So even though this query won't work,
[56:05] let's just like write it out. Right. - Oh, okay.
[56:12] So select from address, and then what if I wanted the district column,
[56:15] it would be select district? - Yeah, so if you wanted only the district column,
[56:21] you just say select district. District, there you go.
[56:26] From address. And the district column looks like it gives you,
[56:33] oh, I scrambled all the data here. So it looks silly,
[56:36] but usually this would be like some sort of actual district.
[56:40] Let's say you wanted the actual data. Oh, okay.
[56:45] Does that make sense, by the way, before I like move on to like how you would like find
[56:48] or like join this data? - Yeah, because it would be select column
[56:55] or like command column table. Is that the way you would say it is command column table?
[57:01] - Yeah. - And then learner said select asterisk from address
[57:10] where city underscore equal ID question mark, where question mark is your city instead?
[57:18] - Yeah. Yeah, so that would be like the sort of full thing
[57:23] that you do if you wanted to get just the, if you wanted to get it based on just a specific city ID.
[57:30] Right, so the sort of where is the thing that I said when I said limited to.
[57:38] So this is get all of this data, but only if these conditions are matched.
[57:44] So in this case, like it'd be city ID is like 300. So if I wanted to show,
[57:52] let's do this for a table that you can actually see. I'm gonna need to refresh this page.
[58:00] Cool, so let's say you only wanted to get this first row and we know that the ID in the first row is one.
[58:10] So you'd say select ID from alpha where ID equals one. And then I have this weird formatting here
[58:18] where it just like shows one row as a different table or a different table format,
[58:26] but it does the same thing, right? It just only gets the first row.
[58:29] So let's say I wanted to get it based on like the user ID. You just change sort of the column here from name to this.
[58:44] This, sweet, and it would get the same row back. - Now you had multiple that I think had the age of like 20.
[59:00] How would you pull them back if they all equal 20? - You just get all the rows that match that.
[59:07] I think there's only, no, there's a few that had different ages.
[59:14] There's a bunch that had the age. Yeah.
[59:18] So yeah, these are all the rows that have an age of 22. And this is very jank formatting that I haven't fixed yet.
[59:30] - That's totally fine. This is still super helpful.
[59:32] So I could do select from like select all columns from a table where column is whatever I wanna have it show.
[59:45] - Yeah. - Okay. - Yep, so like if you had a post and you were like,
[59:59] I want to get all the posts with this specific category ID, you would do like the same thing.
[60:03] As long as you have the category ID stored in your post table.
[60:07] If you didn't, you would have to do, you'd have to make sure there's some piece of data
[60:15] like in the post table that is also in the categories table so that you can make a query that sort of links the two,
[60:23] if that makes sense. - Oh, Nick brings up a good point of where is like filter?
[60:36] - Where, yeah, where is like a filter, yeah. - Is like a filter, okay.
[60:41] - There is, there's actually a, I guess a statement in SQL called like, where it sort of, it does,
[60:50] I guess, I'm not sure if you'd call this fuzzy searching, but it is, yeah, it's SQL will like help you find things
[60:57] that are like other things. I wonder if this would actually work.
[61:03] Like where age, like to, nope. There are no rows here for that.
[61:11] But yeah, there's actually a statement in SQL called like, where you can do searching that is like a little bit,
[61:17] that is not like exact searching, if that makes sense. - Like is?
[61:22] - Searching with wildcards. - Okay.
[61:24] - Yeah. - It's like an array of conditionals
[61:28] that return true or false in the end. You only get to see results that return true.
[61:34] - So you can also, like if I wanted to say, I think you can do this as well, where age is not 22.
[61:45] And you would get all the rows whose age is not 22. - Okay.
[61:51] Underscore matches one of any character and percentage matches multiple of those.
[62:03] - Gotcha. Yeah, I forget all of the wildcards for like,
[62:07] I actually have to implement them like today or tomorrow. So.
[62:13] - For the like operator. I think this is a big part
[62:16] where I'm getting stuck learning them, is I'm like, cool, I can see something.
[62:22] And I'm like, okay, this is starting to make sense. I'm getting it.
[62:24] And then all of a sudden, nothing makes sense again, because I'm like, I don't know which part of the query
[62:30] I need a Google to replace. - Which part of the query you need Google to replace, yeah.
[62:37] - Like, let's say that I gathered from looking at this query.
[62:41] I'm like, you did exclamation point equals 22. And I'm like, oh, if 22 is what's being queried
[62:50] and it's not showing 22, I can see that that is not 22. But off of looking at it, I wouldn't necessarily know,
[63:00] well, what if I needed to do the same thing with a different table?
[63:06] Or not a different table, but a different column. I wouldn't have known just by looking at it,
[63:12] because it's an asterisk, that it's a different, that's the column name.
[63:15] - Yeah, this asterisk is just saying you want to return all the columns, right?
[63:22] So if I only want to do like one column and I still want to have all these other conditions,
[63:26] like you can still have, you can still say I want to take name
[63:29] and have a sort of filter on the age, right? So this still works properly.
[63:36] - Right, but I wouldn't have known that by looking at it. - Gotcha, yeah, yeah.
[63:41] - There's a lot of, I've noticed there's a lot of JavaScript as well, that is very apparent
[63:48] by looking at it, but it doesn't necessarily make it easy to change or know which parts to change.
[63:56] Because as Roy and, okay, Anthony, who else do I get to name?
[64:04] Jacob, Josh, basically lots of people like to yell at me for not reading the documentation.
[64:12] And yesterday I was so excited, I went and I read the documentation
[64:16] and I was getting somewhere and I told Roy, I'm like, I'm lost again.
[64:19] And he's like, how, you sent me the right doc. And I didn't realize that I went and clicked something
[64:25] in the doc to go search it, so I would understand it. And then I got lost there
[64:29] and didn't go back to the original one. - Yeah.
[64:32] - I was like, oh, I got lost in the docs. - Yeah.
[64:37] - It takes talent. - Just, yeah, I would, there's a,
[64:42] man, when I was first learning SQL, this was not, this was maybe a year or two ago,
[64:47] I forget what resource I used, but there's like, there's a bunch of SQL games
[64:52] that I actually really liked doing. I don't remember where they are
[64:54] and I'll have to find them later. But like, it basically will just run you through like,
[64:58] okay, like, this is what you need to do in order to like query a bunch of things.
[65:01] And it will just sort of like, it's almost like a typing test for SQL, which is fun.
[65:06] - Oh, that's cool. - Like write the statement and like,
[65:09] see if it matches the data that you need to get out. Yeah.
[65:15] - And Alien, yes. Writing docs, I completely agree.
[65:19] And it's so worthwhile and I'm so glad it's out there. What I've learned a lot about myself is,
[65:28] docs don't always give, it's not as easy to pick up context
[65:33] or see what else somebody is doing with it. So if I don't understand a word,
[65:39] I have to go search that word and then I get lost trying to get back
[65:42] to the original document of remembering what I was originally doing.
[65:46] Which is just, that's me in general. But then it's also something that I've learned
[65:54] quite a bit about that I don't know if it's everybody or just like a weird thing that I do of,
[66:01] I don't always know the word that I want to search. So even though the docs are there,
[66:07] I don't know what I'm looking for based on, like I haven't learned that terminology
[66:12] or don't remember that terminology. And again, context can't be written.
[66:19] I feel like it's not possible. - Yeah.
[66:23] - Where watching somebody's tutorial, you could normally see where they might've gotten something
[66:28] or how they typed it to be able to get to that same spot. - Yeah.
[66:32] - No, no. - Yeah. - That's good.
[66:35] I am challenging myself to get better at docs. It's there.
[66:41] There's sites like SQL Bolt and select star SQL. I will check those out.
[66:53] I will definitely check those out. - Yep, anything after where is what data points
[66:59] you want to include based on conditions. Yeah, that and then like how you want them.
[67:05] Yeah, anything after where is that based on conditions. And then there's commands like order.
[67:10] - Ooh, so it's order. - How to sort them. - What is ordered?
[67:16] - Ooh, we're going to challenge my very tired brain and it's, so order is just like sorting basically.
[67:24] I wonder, I believe it's like order by and then I should be able to do like ID.
[67:38] And then you also specify how you want them to be sorted. Okay, there you go, wow.
[67:45] Okay, so this is basically saying, I want to order this by this column
[67:53] and then the direction you want to order them by. So in this case, it's easy for the ID column, right?
[67:59] Because five, like I have IDs one through five for all of my rows and then D-E-S-C is short for descending.
[68:07] And so it'll order it from, it'll order it descending, right? And then you can do A-S-C, which is ascending
[68:14] and it'll order them by ascending. I believe, I might be wrong about this,
[68:21] but at least for numeric columns, right? Everything is ordered by ascending by default,
[68:31] but don't quote me on that. - Okay.
[68:35] - I'd actually have to look that up and just double check, but yeah, generally all of these things
[68:41] are ordered by ascending. There's also group by, so same thing or similar thing.
[68:48] Group by, you can group by a specific ID. I'll do age in this case.
[69:00] Oh, I need to, there's always another step that I need to do with group by
[69:05] that I always forget to Google. Yeah, but group by will let you sort of group
[69:13] all of these things together. So you can have like all the 22 ages close together,
[69:19] if that makes sense. - Hmm, that's pretty cool.
[69:24] - It's how you entered them by default. Okay, yeah, that would make more sense.
[69:29] - Interesting. - Yeah.
[69:34] If you have an ID, so, okay, this is, I think the thing that I was trying to explain, but failed.
[69:43] So if you have, I think this table, anytime I insert a row, the ID will auto increment.
[69:51] So anytime I insert a row, I never have to think about what ID I need.
[69:55] It will just like add it to, it will just like see what the last ID is.
[70:03] And then the next row will have an incremented row. There you go.
[70:07] - That's pretty cool. I've been using Strapi,
[70:15] which is something new that I've never used, but it's actually pretty cool.
[70:20] It builds the database content, like you can visualize it a lot easier.
[70:25] Let me see if I can bring it up, which is interesting in the fact
[70:33] that it's the first time I've seen more of a visual version of this.
[70:44] Let's see. And one of the big reasons
[70:54] that I'm wanting to learn more about queries as well, A, I'm also doing it for work and making videos for it.
[71:01] I'm like, I should probably actually understand them. I don't know why I just like totally spaced,
[71:13] but I was like, am I doing NPM or NPX? And I've always done NPM.
[71:18] So for some reason, I don't know why I suddenly was like, let's do NPX.
[71:22] Do you, do you, do you? Oh, why didn't you just, okay, whatever.
[71:28] There we go. So it's pretty cool because like,
[71:32] you can build your content types and it creates your database for you.
[71:38] And like, you can connect it to like Postgres or anything. But then as I'm creating things,
[71:47] like I can create the category, the description, and see all of my content in here where,
[71:54] and being able to do this as like a very simple way of doing things.
[72:00] I was like, this is really easy to, you know, go back into where having to remember to insert something
[72:08] and remembering all the things I need to insert to check all the boxes is really difficult.
[72:14] - Yeah, yeah, I have, yeah. It's, even for me, it's not necessarily like,
[72:22] I can do it in SQL, but it's also just nice to have like a UI that's there
[72:27] that also just tells you all the things that it's like, yeah, okay, this is like, it's, it's dummy proof.
[72:33] - Yes, yes. - Like it's just like, yeah, it's very dummy proof.
[72:36] I like things where it's like the amount that I have to think about how to do things is very low.
[72:41] - Yeah. - And the more I have to think about it,
[72:44] like it's fine, I can do it, but I'm also just like, I'd like to not think.
[72:48] - Yeah, and I think a big part of it is also just what a visual learner as well,
[72:56] like that is our learning types all together. And this is something that's a very visual
[73:04] goodness we'll go with. - Yeah.
[73:07] - Well, awesome. This has answered all of my questions that I had today.
[73:10] Was there anything that you wanted to go over before we wrap up?
[73:17] - I don't think so. This is a very good exercise for me too,
[73:23] to like review what stuff I always have, like I spent some time yesterday sort of like thinking
[73:27] about like what I wanted to sort of like teach. And I always have a hard time like getting the knowledge
[73:35] 'cause I never know what I don't know. So this is like very good review to do it.
[73:38] Okay, like this is, these are all the things that I don't know, so.
[73:42] - And then Lerner, there's a bunch. I know Superbase has in terms of tools
[73:48] that can like let you diagram out how your DB works. Superbase has one now.
[73:52] I also have one, but it is very jank. And I'm working on like making it look a lot better.
[74:00] It uses your Prisma schema to do it. There's like, yeah, there's a bunch of tools that do them.
[74:06] I know there's one for Prisma as well that does it. So yeah, like being able to--
[74:12] (indistinct) - Christian's gonna be back.
[74:15] - Yes, yes, I will be back at some point, yeah. - Yay, well, awesome.
[74:22] Thank you so much again today. And let me figure out who we will,
[74:29] you know, raid you guys too. So thank you all.
[74:33] Josh, Josh is live. Bam.
[74:39] - Sweet. (indistinct)
[74:43] [BLANK_AUDIO] 
