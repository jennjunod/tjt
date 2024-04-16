---
showLink: "https://www.youtube.com/watch?v=v3Ybkz-6o3U"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-database-basics-with-chris-martinez"
title: "Teach Jenn Database Basics with Chris Martinez"
publishDate: "2023-05-10"
coverImage: "https://i.ytimg.com/vi/v3Ybkz-6o3U/maxresdefault.jpg"
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

[00:00] humans. Welcome to another episode of Teach Gen Tech. Today is Teach Gen, not Data Basics, but Database Basics. We're adding to it. Database Basics with Chris. Hi, Chris.
[00:15] >> Hey, everybody. >> Who are you? >> I'm doing great. Yourself? >> Good, good. I've been trying to think
[00:27] about how I tell people that I met you. I awkwardly walked up to a bunch of people at Denver Startup Week. It was like, "Hi. You're cool. Let's be friends." I'm pretty sure that's
[00:42] how we met. Would you add anything to that? >> It was at that rooftop party. >> Oh, yeah. >> It was a rooftop party
[00:52] at Denver Startup Week. Yeah, there's just a circle of -- other than one person, everyone in that circle was a complete stranger to me to that moment. You picked a perfect one to walk into,
[01:03] because no one knew each other anyway. Yeah, Jen introduced herself and seemed cool, told me about the show. I really loved the concept. Jumped in and watched a few of them and
[01:19] had a bunch of commentary in the chat. Now here we are. >> Thank you. Yes. Thank you. That was the fun part. Y'all, in case anyone is curious,
[01:29] I think this is a key point. I still, to this day, get nervous about walking into a group of people and going, "Oh, I'm just going to be really weird and say hi." It's still something that
[01:42] happens. Having my podcast and having my show give me a really good excuse, because saying, "Yeah, I have a podcast called 'Shit You Don't Want to Talk About' and a show called 'Teach Jen
[01:53] Tech'," the first one lets me gauge if they're, like, going to be super judgy. Kind of gives me a temp check. And then also if they're going to be super judgy on being around a beginner.
[02:10] And now I get to add to it, I am a DevRel at Ivan. So there's more to why we are learning databases. And yes, Chris has joined a lot of them and had a great callout, which I am working
[02:23] on, everyone, of being consistent and having a schedule. That's on my to-do list. That is on my to-do list. They should be around this time, and I'm hoping to stick to Monday, Tuesday,
[02:38] Wednesday. So we're working on it. We're working on it. What are we learning about today? Like, exactly, because there's a lot. >> Yeah. So I'm going to try to distill
[02:53] 10, 15 years of database knowledge into roughly an hour and a half. But the biggest piece is that we are going to really just touch on the basics. If there's any
[03:08] DBAs or former DBAs in the audience today, you're probably going to have opinions that are contrary to a lot of what I say, and that's totally cool. Remember that this is how do you
[03:24] help someone who's never really worked directly with a database before get on their feet, not what's the best way to build a database that can handle 10,000 queries a second.
[03:38] And that brings me to another really big point. For whatever reason, in my experience, it has been that developers and technological people in general are the most opinionated about
[03:59] databases more than anything. I used to joke, if you ever want to see two developers get in a fight, have them design a database together. >> And I've heard that from multiple people.
[04:11] >> Yeah. And so, you know, if we come to blows during this, no hard feelings. >> That's good to know. I would say I'm fortunate in the fact that I don't know a ton about them
[04:26] yet. You've seen a lot of the ones that I've been doing with Postgres. And also, for everybody's knowledge, we're starting with Postgres not because it's like, "Hey, I'm just going to pick
[04:39] something random." It's because it's part of my real job. So I'm using my show to help me learn my real job. And part of that is creating videos to get started with Postgres, MySQL, and Redis.
[04:54] So there is the background to it of why you might be like, "Why are you asking just these ones?" So eventually, I'd love to expand, but that is kind of our starting knowledge base. So...
[05:07] >> Yeah. And last bit of disclaimer is, as I mentioned, people are incredibly opinionated about all aspects of database design, management, implementation, usage, et cetera. So remember
[05:27] that you are getting my highly-colored opinion on this. So look at everything we talk about today through that lens. If you talk to other developers over time, they're going to tell you different
[05:42] things. And it's not that necessarily either of us are explicitly right or wrong, unless they're telling you something that's technically impossible or dangerous. If they're like, "Oh,
[05:56] just expose all your ports to everybody. Everyone loves being publicly accessible. You don't need roles." Yeah. Other than that kind of stuff, every opinion is to an extent valid.
[06:11] >> That's interesting because one of the things that I'm working on grasping is why we would secure specific IP addresses or whitelist them, just as something that I'm like, in my own head,
[06:27] I'm having a problem. Wait, so would you do that? Because... Anyway, I will go through that later. >> Yeah, no problem. I have a fun story for when we get to that.
[06:37] >> We don't need to go through that one just yet. All right. So I will say we are going through... And just because I just love doing this on my iPad, so I'm going to share it really quick.
[06:52] It's my Notes app. We do have a whiteboard that we'll be working with as well. But this one is my Notes app. So give me just a second. We want this window. It's also not exactly even yet. Okay.
[07:08] No, it's not even. But it took me forever. But this does show us what we're going through. I have them based on size, not necessarily order, just so everybody knows. I'm excited to
[07:27] learn about what's relational and non-relational. The codeverse versus databaseverse. Basic SQL queries, which I'm very excited about. And database design. And hello, learner. Thanks
[07:41] for joining today. And yeah. So this is what we're going to talk about some parts on. And where do you want to start? Because there's a lot of different options.
[07:56] >> Yeah. So let's start with... For those who either haven't... This is your first time tuning in. Or like me, you don't always make it every week and aren't all the way caught up. Let's
[08:12] start with... And I recommend this process for any technology implementation. Let's start with talking about the problem that you're trying to solve. So talk about the website that you're
[08:26] putting together that drove you to want to have a database, want to implement a database. And then we'll start talking about the kinds of databases and move on from there.
[08:37] >> Yay. And just as you said that, I finally got the image even on my screen. Because that is the random stuff that drives me bananas. So ding, ding, ding. And for those who... I do need to bring
[08:53] up the Miro board, too, to try to explain this. So it's like double-sided of I want to do this because of my website. Because I want to make it a lot easier for everyone to actually be able to
[09:09] consume the content that we're working on. But then also to learn the new company and job I have. So it's great when they all work together. So I have a website.
[09:21] It's very exciting. Very original. And I want to make it where we don't need to worry about this Ivan one. That's something that's going to be built on Ivan. I'll just link to it.
[09:37] But we have Teach Gen Tech, which has over 80 episodes. But nobody would know it unless you go through YouTube. And going through YouTube is going to be not fun. Not fun at all. And then we
[09:51] have my podcast, which has probably 60-ish episodes. I paused it for a while. But again, people can't really search it unless they go to specific places. Because I took down their old
[10:02] websites. Because it was a lot to keep up with. And so in my head, what would happen is they would both have their own episode notes. Like, hey, I need these X amount of things to go into every
[10:26] page that I create for Teach Gen Tech. I need the YouTube, the episode description, the guest contact, any associated links, and the transcript. Okay, cool. The podcast needs a little bit more.
[10:42] It needs the Apple link and the Spotify link to that exact episode too. So it's a little bit more, but not like a ton more. And I'm like, I think I can do that with a database. I think. But is it
[10:57] just one database? Do I need multiple databases? Do I use a JSON file instead? Because last thing to show all of you is, let's go to Vercel. Not this one. No. Go to this one. Uh oh. Did I lose
[11:26] my stuff? Is it this one? Deployments? Maybe. Now I lost it. I'll just go to the GitHub. The GitHub will tell me. Okay. So this is what the old website looked like before I got hired.
[11:53] Which is great. I don't have to say hire me really big anymore. This is lovely. Thank you, Ivan. And under livestream, I would have the stream schedule. So this is one JSON file that I would
[12:06] have to update manually. And then I would go to portfolio, and code is a second JSON file, writing is a third JSON file, and speaking is a fourth JSON file. I'm not saying this is the
[12:20] proper way of doing things. I'm saying this is how I winged it and got it to work the way I wanted it to look to be able to go get a job. Not necessarily proper way of doing things. And also,
[12:32] not knowing what's when you would use a JSON file and why there are some items that you would put, like, I may be mixing up language right now, but I think I've heard that you can put JSON files
[12:47] within a database as well. And I'm just like, well, I don't know. But that's why I was like, so could I have had one database for even though they're all using different things?
[12:58] Or yeah. So that is the base knowledge that I'm at of yeah. I don't know. So part of the beauty of that example is it's an excellent segue into talking about the two
[13:17] main, like, super types of database, which are relational databases, your typical SQL based SQL flavored, although there are other kinds that we won't get into, databases,
[13:34] and then your non-relational, no SQL, which does not stand for not SQL or doesn't have SQL, it stands for not only SQL. >> Oh, I don't think I ever
[13:48] realized that. >> More of a piece of trivia than important to the current discussion, but what's called unstructured or semi-structured data.
[14:00] And what you had going there with your collection of JSON files sounds like unintentionally, but regardless, you basically had a rudimentary unstructured
[14:15] no SQL database that you built yourself out of raw JSON files. >> That's fun. >> There have been plenty of times
[14:24] where I just needed to stick data in a place for a minute and get it out real quick and not do a lot of crazy stuff to it, where I've just stuck some JSON files in an S3 bucket, and that was my
[14:40] database. Other more formal ways to use that unstructured or semi-structured data include things like MongoDB, that's the one everyone really knows. And yes, you can store
[15:04] JSON data as a data type, which we'll talk about when we get more into the databases within your Postgres. And also MySQL now supports storing JSON data type as well.
[15:22] >> Interesting. And this is something that I'm very excited about asking about. And I warned Chris that at one point I will ask this of like, what's the difference between Postgres and MySQL?
[15:36] Whenever we get there, I'm very excited about it because it's something that as I share my journey with others, that they're like, well, what's the difference? I've heard of MySQL. And I'm like,
[15:49] I don't know yet. I will get there. >> Yeah. And I don't want to get there just yet. Let's finish going over just the two super types. I don't believe that's a technical
[16:05] term, but that's the term I'm going to use. Super types of database. So the use cases for them and when and why there are two different types and when to use them does matter quite a bit. And that's
[16:22] where the first place for technological people to start fighting about databases. There are certainly people who have made reasonable arguments for using a NoSQL database for your
[16:42] entire application. And there's no reason unless you're a bank. That's the one example everyone gives where you always have to have a relational database. Where they say, oh, it's fine. Use
[17:00] MongoDB for your entire app. You don't need a relational database. Semi-structured or unstructured data is the best. And it does have plenty of upsides and advantages. >>
[17:16] I'm just realizing I am using -- I will say just for clarification, I'm not using the whiteboard we're supposed to do because I was faster and know how to do this one better for now.
[17:31] >> Okay. We can save the other whiteboard for when we start diagramming this. >> Okay. Cool. Because I'm like, that one's harder to -- is it non-relational? Right?
[17:46] >> Yeah. Non-relational or sometimes they'll be called semi-structured or just NoSQL. >> Ah, NoSQL I think is the word I'm looking for. >> Yeah. And sometimes, you know, things like,
[18:02] excuse me, my allergies would be profoundly inconvenient. >> I don't know what happens, but like streaming, it's happened to me on so many streams that I'm like, I'm fine all day.
[18:17] And then as soon as I get it ready to stream, I'm like, allergies. Can't do it. Okay. So, we got relational and non-relational. I'll just say unstructured, semi-structured.
[18:29] >> Yeah. And that's -- it's also important to understand that even in your NoSQL databases, there's still ways to relate data and entities to each other. It's just not as tightly coupled
[18:44] or as strong as with a relational database, which we'll get into. I don't want to spend too much time on -- especially because your technical requirements more or less require you to use
[18:59] a relational database. I'm not going to go too deep into the other type, other than to say it exists and you're going to hear -- you're going to hear about them. And it's good to have at least
[19:13] a basic knowledge of what they are. They're very, very good if you have a whole lot of data coming in and out that doesn't have to have a lot to do with other data in the system. So, for example,
[19:38] the classic use case that a lot of people use is if you have a social media app, all of a person's posts, they just need to, you know, fall under that person's bucket. So,
[19:57] like, when you use your Twitter and you send out a tweet or whichever one of those is the correct term, that probably is just stored as a piece of JSON somewhere. And every time you do it,
[20:15] there's another one. If I go and start a Twitter account and send one out, there is no need -- even if you and I worked together or even though we're friends, it doesn't matter. There doesn't need to
[20:35] be any relation between my bucket of tweets and your bucket of tweets. >> Okay. >> Now, compare that to this -- the whiteboard we're going to be using somewhere else. That's probably not
[20:53] exactly how they're storing it, but let's say we were making a whiteboard app and you and I work for the same company. Ivan decides they need more engineering managers and they hire me.
[21:07] And we both work for Ivan and we have this shared whiteboard that you and I are working in. So, now, you and I each have our own account. And that's stored in the database table somewhere.
[21:24] And there's this whiteboard which lives in its own table. But because we both work in the same organization, which is Ivan, and someone else over here works at Twitter and they have their own
[21:36] whiteboard, this whiteboard needs to know which organization does it belong to, who at that organization is using this whiteboard, who's allowed to see it. And that's where the tight
[21:49] relational entities and stuff need to happen. That's where things need to relate to each other. >> So -- >> Because otherwise,
[21:58] you have a pile of whiteboards laying around. >> And that's a good example. Thank you. So, you mentioned, like, the -- like, the NoSQL versions is like Mongo. Kafka?
[22:18] >> Admittedly, I'm not super smart on Kafka. I couldn't tell you much about it. >> Okay. But things like -- okay. I'm just -- this is my I don't know pile.
[22:32] >> Yeah. >> But, like, Postgres is over here. >> Very much a relational. Although Postgres will -- it's a little -- it's its own special
[22:42] animal, and we'll talk about that when we get into the difference between MySQL and Postgres. It's, like, it goes in the relational column, but you can, like, kind of put it close to the line.
[22:53] I'm pointing with my finger as though I'm able to point at your tablet. It's -- it can dance around in -- >> Just, like, kind of right on the line of, like, it's its own thing.
[23:06] >> But really, most people use it as a relational database that I know of. >> Okay. >> And feel free
[23:11] pitchfork-wielding commenters to tell me I'm wrong. >> Learner, I just looked down and saw your CouchDB and Redis. Is that on relational as well? I think they are. Because it has Redis,
[23:29] and I think Redis is relational. Unstructured. Okay. Cool. Thank you. I'm glad I asked. Like, there we go. So, that -- Couch -- yeah, there's so many that I, like, feel like I haven't
[23:49] heard of. Like, I -- this is something I need to look up, is, like, how many databases? Not, like -- >> There are tons, and they all have their own special job. Like, they have a reason to exist.
[24:05] Like, there's a reason why -- and, again, anyone tell me I'm misunderstanding, because I don't play too much in unstructured land. But Redis is good for, like, data warehousing where you have just a
[24:22] ton of data that you don't really need to -- you need to look at it, but you don't need to do anything with it, if that makes sense. Like, it doesn't change. It just lives there. Where Mongo
[24:36] might be, like, your app's main database and has a lot of in and out. >> And that's -- a lot of people have explained that to me as well for -- it does not help if I can't -- there. I'll just move
[24:52] you down here. And I'm going to put that for Redis is, yeah, a lot of people use it as their cache instead of its own, like, standalone. >> Yeah. Was Redis the one that lives,
[25:07] like, in memory? Am I -- >> So -- I like to hang out with -- oh, yes, yes, yes. Okay. Redis, lots of times, is used for cache. And I'm going to -- why am I,
[25:30] like, spacing how to spell cache? >> Yeah, you're right. C-A-C-H-E. >> Okay. Because I'm, like, that's -- >> Oh, you have a bonus C in there.
[25:39] >> Oh, that's why. Okay. That's why. There. We'll just make this a C. Cache -- or an E. There we go. Cache. And uses memory. Which is a whole 'nother thing that -- I like to hang out with our OSPO
[25:57] team, and, like, they mention it one time, and then I'm, like, I'm lost now. >> Okay. Again, anyone who knows better than me, tell me I'm completely wrong,
[26:07] because I might be. But I think Redis is, like, if you have a -- like, something that lives in a Lambda function or something that doesn't stay alive all the time, like a web service, Redis is
[26:21] what preserves your data where you might store a variable in session if you're on a always on web server. I think Redis sort of acts like that. >> Oh, in Firebase.
[26:39] >> Almost like a stand-in for session. But, again, anybody tell me I'm wrong. >> We -- I'll look that up later on. But relational, we have, like, MySQL,
[26:52] we got Postgres being its own, like, random thing. Any other big players? >> I mean, Microsoft SQL, or just SQL Server. You'll see it written both ways, like MSSQL or
[27:05] SQL Server. I think Oracle still has -- Oracle bought MySQL, but I think there's still, like, an Oracle SQL database somewhere. >> You know what? I never said I
[27:21] could spell by starting this, so we're just going to go with that. Oracle Server. >> Yeah. I will say that it's MS, like Microsoft SQL on the one above Oracle. No problem.
[27:34] >> Thank you. And then Maria. >> So, yeah. And Maria is, like, a flavor of MySQL. >> Didn't Maria come from -- I guess
[27:46] there's also, like, a lot of drama with tech is also what I found, is, like, tech has a lot of drama because they, like, break off from each other and go do something else. And Maria is like
[27:57] that. >> Yeah. Much like Activision, the video game company, was started by a bunch of disgruntled Atari developers, MariaDB was
[28:05] started by a bunch of disgruntled MySQL. >> I'm just going to put those together like this. >> And they're so not -- like,
[28:16] their differences are so superficial, it's not, in my opinion, in my highly opinionated database opinion, not worth learning why they're different. >> That's good to know.
[28:28] >> Yeah. >> There's DB2. Oh, my gosh, there's so many different -- >> Yeah. Well, and then, if you want
[28:37] to get wacky, Amazon has, like, all these things that are basically MySQL but not. >> I'll just put Amazon in general. >> Yeah.
[28:46] >> Okay. >> They're all, like, versions of RDS you can spin up, which is relational database or relational data storage,
[28:56] something like that. >> Okay. >> But what really is important here is to know that all of these that are written up here
[29:08] use some version of SQL. So SQL just stands for structured query language. And Postgres is going to have its own sweet extra cool features. And MySQL is going to have its
[29:24] features that the other ones don't have. And then T-SQL, which stands for transact SQL, it's got its own features and quirks, but they're all based on SQL. And if you just learn
[29:38] the basics of SQL, you will be able to get by. >> And I think that goes to another question of, like, a lot of people have told me that, like, SQL as a language may not be something that anybody
[29:56] really needs to learn. And but, like, don't all relational databases use SQL? Therefore, wouldn't you want to learn it? >> So there are a lot of frameworks
[30:10] and tools that generate SQL queries for you. >> Oh, okay. >> Or act as a stand-in for SQL. I come from a .NET development background, and .NET has
[30:25] something called Entity Framework that handles. And then there's also something called LINQ, and L-I-N-Q. And those are libraries that let the .NET framework talk directly to your database,
[30:38] and you never have to write one line of SQL. >> That's cool. >> On the Node side, there's Kinect. A lot of people use that. And same thing. It generates
[30:53] queries. It's spelled like the toy. >> Oh, wow. >> I will say those are incredibly useful tools. And there are some people who say never use them.
[31:06] And is it cool if I swear on here or no? >> I have a podcast called Shit You Don't Want to Talk About. So fuck it. Like, let's go. >> Okay. Some people will say, you know,
[31:20] don't ever use them and fuck you for even thinking about it. Only write SQL. And then there's -- I don't agree with those people. I think you should absolutely use them when it makes sense to,
[31:32] which is most of the time. However, I also am a firm believer that you should know SQL because there are going to be times when you're debugging or doing some kind of experiment in development
[31:50] where you're going to want to directly query your database and you're going to need to write SQL. And the other thing is, it's not that hard. It's not -- it's not -- you're not -- it's not like
[32:04] learning -- I'm not asking you to learn, like, another high level programming language. It's not like, all right, you know Python and Node. Let's tackle C# right now, Jen. >> No, thank you.
[32:18] >> No, it's -- it's -- it's very simple and very logical. The commands, they're -- in my opinion, I'm going to say that so much. In my opinion, there's no SQL command where you can't immediately
[32:40] tell what it's asking the database to do. >> Okay. And I saw that a bit when we streamed a few weeks ago. >> Yeah. >> Oh, my gosh. I can't believe that was a few weeks ago
[32:52] just because I've been traveling so much. I'm like, I streamed, like, yesterday. No, I didn't. It's been weeks. That's weird. But you said that during that and I was like, oh, okay.
[33:05] >> And there's -- there's going to also be times where it either doesn't make sense or you're working in a language or framework that doesn't support one of those query generators. And at
[33:18] that point, you're either writing your own from scratch, which is usually unnecessary, or you're just going to write SQL directly. >> Okay. >> So I am an advocate for using
[33:30] querying tools. I'm a huge advocate for leveraging frameworks that make it easier to interact with your database, but I also believe that anyone who wants to call themselves a full stack developer
[33:43] should know SQL. >> Good to know. Good to know. >> Yeah. >> All right. >> And by "know SQL," I mean be able to look at the references on W3Schools and know, oh, yeah, that's how I do that.
[34:00] >> Yeah. >> I don't think you have to have it committed to memory and be able to write a perfect SQL query without looking anything up, but you should damn well know what you're looking
[34:12] up. >> Yeah, and that's been a big struggle with being, like, self-taught, and I hear this from other self-taught people, is that you don't always know what to look up. >> Yeah. >> So it's like,
[34:27] I know I need to look up something, but I don't know the terminology of what I need to look up. >> Yeah. >> So -- and then really quick, just to get -- there we go. To -- I want to get this,
[34:41] see if I remember what it is, because it's JavaScript object something. >> Notation. >> Okay. JavaScript object notation. And
[35:03] I will ask more about that later. Okay. >> Yep. >> I just wanted to remember what it was. And then anything else you think we should know about, like, comparing the two?
[35:22] >> Probably not on this level. I think now we're ready to get into what makes MySQL and Postgres different, which I know you wanted to talk about.
[35:38] >> I'm just putting that so I remember that they can do. So many. So many. Okay. >> All right. Here. Can I -- do you mind if I drive for a moment? >> Yeah. I think you'll have
[35:57] to reshare your screen. It went away for me. >> No problem. >> But at least you don't have to get the browser to do it for you. Because that's why I always ask people to join beforehand.
[36:09] If I ever have to learn from another -- or, like, go from another browser, I'm like, oh, goodness. That -- I didn't realize I had to share it. Thanks, Apple, for making my life hard.
[36:22] >> I'm sticking this link in our internal chat that you can share with the -- >> Yay. Thank you. >> -- world at large. I think this is a good, well-written article that really
[36:34] highlights the difference between the two and doesn't come with a strong opinion about which one is better. It really says this is the use case for one and this is the use case for
[36:50] the other, where a lot of these types of articles will just be like, oh, Postgres is better all the time. Fuck MySQL and the horse it rode in on. But really, they have -- they both have their place.
[37:04] >> Okay. >> So the very short -- the short answer is more people know MySQL than Postgres because it's been around longer. It is potentially
[37:18] faster, but this article even talks about why that's not 100% of the time true. But it's worth knowing that if fractions of a second matter, which sometimes it really does
[37:32] in programming, MySQL can often give you an edge. But Postgres just does so many crazy cool things that MySQL didn't used to do. And you'll notice, like, a lot of the things in this chart,
[37:51] MySQL now does and didn't used to. They're both running into each other because they both -- I don't want to say they see each other as a threat because they're both open source, but they both
[38:04] definitely take the good things from each other. Like, for a long time, you couldn't stick JSON in a MySQL database in the same way that you could a Postgres database, which now you really can.
[38:18] And the other thing is you can write -- and that's probably another reason why there's some people saying you don't need to learn SQL, is Postgres will let you write in other languages. Let me go.
[38:34] >> Oh, so you can query in other languages. >> Yeah. And somewhere -- and MySQL does that a little bit, too. But in my -- in my opinion -- everybody take a drink every time I say that,
[38:49] and you won't be able to drive back to work. In my opinion, it's going to be quicker to just write the line of SQL to do your query than it is going to be to write your query out in one of these
[39:04] languages. So -- >> Yay. Okay. >> Still worth learning SQL, in my opinion. But, yeah, I recommend reading this article. We're not going to go in too much depth because it could take the whole -- it
[39:23] could take the whole session. But the big 1,000-yard view is MySQL does a lot of things. It -- the 1,000-yard view is MySQL is older, and so more people are familiar with it and have worked
[39:41] with it more. But Postgres is old enough now, that's not necessarily true. >> But also, like, doesn't -- and this WordPress is mostly on MySQL. >> WordPress is entirely built on MySQL, yes.
[39:57] >> Yeah, so -- and WordPress being so large is something that's considered easier than, like, a fresh website. Yeah, because -- >> Ooh, great, great example of why it's a real good idea,
[40:10] even if you normally use query generators or those kind of tools. Really great example of why it's important to know SQL is, say, you're working with a client who has their marketing
[40:27] website out on WordPress, and especially if you work in services, if you work at some kind of agency, if you do one -- it's been my experience -- I love to qualify everything -- it's been my
[40:46] experience that if you do a technical project for someone who does not have their own IT department, you become their IT department. >> Yes. Yes, we do. Yes. >> And so you built this really cool
[41:06] web app that uses Postgres and does all this cool, snazzy stuff for them, and suddenly their marketing website's broken, and they don't know who to turn to, they're going to come to you.
[41:21] So now it would be really handy to know enough SQL to go into their WordPress database and disable whatever plug-in and made it so you can't get into the WordPress back end, because nine times out of
[41:38] ten, that's what it is, is some fucked up plug-in. >> Yep. >> And just knowing how to write the SQL query that lets you disable that plug-in. >> And it's crazy, and this is a big reason why
[41:55] I appreciate so many guests coming on the show to learn these things, because the example you just gave me, I used to have to do when I worked at GoDaddy all the time. People would call in,
[42:06] something broke, even on Managed WordPress, or if they had it on their own server, because they wouldn't know how to get into MySQL to -- or the admin? SQL admin? >> Yeah. >> My
[42:23] admin? >> My admin, yeah. >> Thank you. I'm like, I don't remember what it's called, but we would have to go through and be able to do that, that it was really, really helpful being able to learn how
[42:34] to compare them, and y'all, just because this is such a -- was a really, really good example of it, I had Roy on the show, and we talked through the differences, because I was having a really hard
[42:53] time understanding all of the different -- like, Vercel versus, like, shared hosting. >> Yeah. >> And this video goes through this, so I definitely really appreciated that, and yes, please continue,
[43:10] because I was like, oh, yeah, I have done that. I forgot. >> Yeah. So, yeah, that's my example of why it's worth your time to learn SQL, even if you can spend the entire rest of your career using
[43:27] query generators. >> That's awesome. That is awesome. Thank you. Thank you. >> Yeah. No problem. All right. So, we talked about why Postgres and MySQL are different. We talked about
[43:44] relational versus non-relational databases. Now let's talk about code first versus database first, and sometimes you don't get a choice. >> Okay. Good to know. >> So, when you're making a database
[44:05] -- >> Oh, yeah, that's true. >> That's awesome. But, you know what? Still use a SQL. Still built on SQL at the end of the day. So, we will learn some basic SQL before the day is over.
[44:19] But when you're creating a database, everything in a relational database -- let me make that super clear. We're talking entirely about relational databases right now.
[44:34] Everything in a relational database is stored in tables, which, well, relate to one another, and we'll go over what that looks like and why and how later. But you can either come up with
[44:52] all of your entities, as they're called, or your tables, your things you're storing in the database and how they relate to each other, and you create them. That's a great way to put it.
[45:07] They do kind of look like a bunch of Excel spreadsheets that reference each other. But you map out all these things and define them, and then you have to go into the database,
[45:24] create the tables, define each of the columns, et cetera. And if you don't have -- if you're not working with a framework that supports a code-first database, that's just how you have
[45:38] to do it. A code-first database is where you go and you write out your classes, either your JavaScript classes or your C# classes. I believe Java also has some version of this.
[46:01] The one thing I actually like about Django is the way it handles code-first databases. So you write out your Python classes, whatever object-oriented language it is,
[46:16] you write out these classes, and then you run some kind of command that generates a database based on those classes. And it puts the schema together for you. You don't have to -- now,
[46:37] I like to go and look and make sure it didn't do anything stupid, because none of them are perfect. But a lot of the time, they work great. >> Really quick, I had a question.
[46:54] What was my question? Damn it, I forgot the question. Well, you know, if I think of it, we'll get back to it. >> And if given a choice,
[47:10] I prefer doing code-first -- yeah, someone, learner0418 is talking about ORM, which is, I believe, object-relational mapping software or library. The node one that I know of is called
[47:35] SQLize. >> And you use that on code-first? >> Yeah, to generate and update your database. That's the other really nice thing about using
[47:52] an ORM, is if you have to change something, if you have to change the properties in an object, because you just thought it was going to do something different when you first planned all
[48:04] that out, it's easier to say, hey, go update my database for me. Because otherwise, you got to change your object, then you got to manually go into your database and say, all right,
[48:19] I had to change my database so that it doesn't get pissed off that my object is different when I go to make my query. >> So I've been working on
[48:29] actually doing this, and it's really funny, because in case -- and Nami mentioned you want to learn Prisma for this. Well, I've been setting that up with -- I got
[48:46] challenged. I got challenged, like, in this group that I run with -- I feel like such a cool kid, a.k.a. just, like, my Discord server friends, that if I can create the T3 app,
[49:02] they'll answer more of my questions. And I'm laughing, because it has you connect a database and then push it and have it do code first, which I didn't realize that's what you were doing.
[49:21] It was code first, because you do with Prisma, once it's connected, it does NPX Prisma DB push, and it creates it for you, and it updates it for you. I got stuck on a different error,
[49:35] but it's interesting, because I wouldn't have realized that that was what I was doing. >> Yeah. >> So that being said,
[49:48] if I -- just to see if it's connecting dots or not. Let me stop this one and reshare for my entire screen. Window. Not that one. Entire screen. This one. I had to scroll up on my
[50:08] thing. This is it, in case anybody is curious about it. I'm only, like, halfway through it. But if I'm over here -- excuse you. Excuse you. If I made all of these first in the database,
[50:25] that would be database first. Because I'm like, I want all of these things. That being said, would that be the database, the schema, or the table?
[50:39] >> So the schema is what defines the -- what the tables are and what they look like inside of the database. So each of those things that are in your diagram there would probably be a table.
[51:03] >> Okay. >> And the schema would define what columns are in that table and how the tables relate to one another.
[51:13] And then eventually you can get into things like stored procedures and indexing and stuff, all the DBA shit that makes them go faster and be more efficient. But I would argue are
[51:29] not as important as learning the fundamentals, so we're not going to cover them here. But, yes. That -- >> So one schema can have multiple tables?
[51:43] >> Yes. Shitloads of tables. As many tables as you need. >> Can one database have more than one schema? >> Yes, but it's not common.
[51:56] Almost always it's going to be one schema per database. To the point of I can't -- even though I've like heard of it, I've never even seen it out in the wild. I just know that, for example,
[52:15] Postgres will absolutely do it. I'm not even sure MySQL will allow it, but Postgres definitely will, but I cannot think of a use case for it. >> I cannot write today.
[52:30] >> I would say if you need two schemas, you probably need two databases, unless somehow in some wacky world you have the exact same data, but you need two distinct ways to
[52:45] model it or map it. And I just can't -- if anyone comes up with an interesting reason why you would do that, let me know. >> I know I'm switching a little bit over
[53:01] here, so please bear with me. Do you -- because these are -- so if I have teach gen tech as one table and then like shit you don't want to talk about as another table,
[53:16] do I need to define the same things? Can I say like this is a string, this is -- I don't know, whatever. Like having -- >> So here's where the relation part of a relational database gets
[53:36] awesome. So both of your things have a YouTube embed, right? >> Right. Here. Let me see if I can put these by each other a little better. Okay. >> We're probably going to want to hop over to
[53:48] our shared whiteboard soon after this. This is where we start getting into database design. This is where the fighting starts. So you have shit you don't want to talk about and you have
[54:00] teach gen tech. But they both have a YouTube embed. >> Right. >> And there's probably not any reason for them to be different. A YouTube embed is a YouTube embed. It has a link. It has a
[54:14] thing. But you're probably only having one YouTube embed per show. I don't know why this episode of teach gen tech would end up on shit you don't want to talk about unless this conversation gets weird.
[54:29] >> That is a great way of saying that. Thank you. >> So what you would do is you would have one YouTube embed table and then you would have some way to relate that YouTube embed to the other show.
[54:46] Now, you could either have just one column that's like show ID that is either teach gen tech or shit you don't want to talk about. And that's one way to do it. And that's called a one to many
[55:07] mapping where one show, teach gen tech, has many YouTube embeds or shit you don't want to talk about has many YouTube embeds. But let's say this episode of teach gen tech does get really deep.
[55:25] We suddenly start talking about I don't know. I don't even want to try to come up with a topic. But something really deep. And we leave database world for a minute to work through that. And now
[55:39] suddenly we have a YouTube embed that we really do want in both places. So now we need a way to map it to where it could be associated with both. And that is where you have a many
[55:55] to many relationship where many YouTube embeds could belong to many shows. And that's done through a special kind of table that we'll go through when we start. >> Okay. I'm excited for
[56:13] the designing. Clearly. Because I'm like this is where I'm also really stuck on. Okay. This -- let me scroll out here. >> The other thing is it doesn't matter if you're going code first or
[56:27] database first. Making a -- I mean, there are some people that say a database diagram is a very specific thing. And if you're not drawing it a certain way, it's not a legitimate database
[56:45] diagram. I don't agree with that. If it's -- if the thing you write down is what makes it so you can create the database correctly, it's a fucking database diagram. >> Okay. >> So we're going to
[56:56] make a fucking database diagram. >> I'm really excited about this. Yet kind of nervous. Because I'm like it still doesn't click yet. But this is why I have the show. Because I got to learn this
[57:07] stuff. And I'm stuck. And I'm stuck. And I'm like -- and this is like just for all learners out there. I'm literally a learner because you're here. I like that you have that as your username.
[57:18] Is that we all learn very differently. And a lot of learning is finding out about a topic and learning about a topic multiple ways. Probably multiple mediums. And possibly multiple people.
[57:38] I say all of that to say I've had repeat customers -- repeat guests on the show. And I'm then like six months down the road, I'm like, oh, it finally clicks. I wish they did that more often.
[57:56] We're getting there. We are getting there. Okay. So do you want to -- yes? >> One of the comments, forgive me for butchering your screen name, wouldn't Code First also help with keeping
[58:11] track of database changes over time? Probably. If your migration history supports that. I know that the Code First tools associated with Entity Framework in .NET certainly do a pretty good
[58:32] job of it. I just don't have enough experience with things like SQLizer Prisma to say what they do. And yeah, someone commented storing logs is really good.
[58:52] A really good practice. Again, at least in Entity Framework, it keeps -- kind of keeps track for you if you look at -- go back and look at your code. And part of
[59:08] that is because you can always roll back migrations. A migration being just a change pushed out to the database. >> I'm slowly typing. I'm not a very fast typer. I've been talking to Prisma. They've
[59:31] been on the show before, but it was when I was actually interviewing with Ivan, and I didn't know what I was doing. Even more so than now. Let me look for that episode really quick just so that
[59:46] way you have it. But then also I'm talking to them about coming back on the show because it is something that I feel is a bit different conversation now. >> Yeah. I'm excited because I
[60:07] in comparison compared to the decade I've been working with .NET, Node is still comparatively new to me. And so I'm very interested in learning what kind of tools are out there in that ecosystem.
[60:25] >> Okay. Here is the Prisma stream that we had. It's like six months old. It does have to do with some Ivany things because it was when I was interviewing here. But we actually dealt with
[60:45] SQLite. So it's definitely something that... And if anybody feels like watching it and suggesting time codes for chapters, dude, I don't know what I'll give you, but I will give you a huge shout
[61:00] out. I'll send you a hat or something. I don't own hats, but I'll buy you a hat because I want to make hats. >> I want to teach Gen Tech shirt. >> I should, I should. Because it's like getting
[61:16] the... Dev, hello. Dev has yet to be on the show and I'm very excited. I don't know what we're talking about yet. But yeah, I'm going to put some stuff together. So just as a side note,
[61:31] we talked about this a while ago, but I am setting up my stuff within the OSRG Guild, which is the Open Source Raid Guild. And many of you know Jacob, who has been on the show and is
[61:51] also looking to come back on the show. So that'll be cool. Is he now has a store for all of his swag. And I'm trying to look for it really quick because this is like my third time losing it.
[62:05] How do I keep losing the store? Like the link. I just... I'm magic is what I've decided. Magic and losing shit. But anyway, I will share it later. That one already has a store and has swag.
[62:20] So that's a start. And then maybe one day he'll let me like put TeachGen tech stuff with it. So it's like they're together and that would be cute. Anyway, yes. Prisma, go check it
[62:37] out. Dev, do you want to be on the show for Clerc? That could be cool. Unless I'm like just forgetting where Dev just started working. And that could be really funny. Yeah. Wait,
[62:56] I just went to your... Is it your birthday today? Because I feel like I just got balloons. On your... Dev, is it your birthday? I'm going to very, very awkwardly. Yeah,
[63:11] I'm going to awkwardly sing you happy birthday really quick. Happy birthday to you. Happy birthday to you. Happy birthday, dear Dev. Happy birthday to you. Yay. And many more on Channel 4.
[63:27] Because I don't know why that's a thing. Because it rhymes. You are more than welcome to clip it. But yes, yes. Oh, that's so cool. Happy anniversary.
[63:46] Okay, Chris, because I now get to be friends with your wife too. How long have you guys been together? I'm curious. So we started dating in 2005. We got married in 2010. So we've been
[64:03] married for 13 years. And together for almost 20. Yeah. I'm like if I'm mathing right, right? Yeah. Yeah. Yeah. Okay. Like, am I mathing right right now? Yay. Congratulations. And for those who don't
[64:18] know, because I just have fun, on the OSRG Guild, his wife has joined us to play the Expanse. And it took me like, okay, it took Roy three hours on a call to teach me, help me work through my
[64:35] character development. But these are all things for another time. I'm really great at derailing. Sorry, Chris. That's all right. All right. On that note. Your third channel is Teach Jen
[64:49] Gaming Principles. I mean. Here's how to burn out a character really quick. Here's how to. I mean, trying to create a character, like, I can't, I don't, I don't know if I should share
[65:05] all of it. Like, Roy might get mad. But it ended up being three pages of a character background. Like, this brings me back to school. Three pages, no spacing, like single space. It's
[65:18] not even double spaced. And I was like, this is a freaking novel. But a really good experience. All learning. Okay. It also depends on the game system.
[65:29] That's true. That's true. I'm just, we're gonna, we're just gonna run down. We're gonna chase this squirrel for a minute. And once we, once we've caught it, we'll come back to databases. I was
[65:44] gonna say, because doesn't your wife do this? Yeah. So she works for a company called Pinnacle that makes a system called Savage Worlds. And their whole thing is called their, their tagline
[65:57] is fast, furious, fun. And if it takes you more than a half hour to build your Savage Worlds character, you thought way too damn hard about it. That is crazy. I've, I've, I've had someone,
[66:11] I've been running a Savage Worlds game at a convention, had someone walk up to my table and say, hey, do you mind if I make my own character? And you know, in a convention, you only have a
[66:20] limited amount of time to run your game. So with most systems, it's like, sorry, man, you either use one of my pre-gens or bring one you already brought. We don't have time for that Savage
[66:28] Worlds. I'm like, yeah, go nuts. Here's the book. By the time we're done saying hi's and everyone gets their drinks topped off, you'll have a character cranked out. That is crazy. That is
[66:38] completely crazy to me. Okay. Oh, that's where, okay. Sorry. I am, uh, setting up. I got Accelidraw on, on here. I just as, uh, I'm so excited for Sarah joining. A, it's also someone that really
[66:54] knows the Expanse. And for anybody that's wondering, I'm still haven't finished watching it. And I'm not going to start listening to the books until I finished watching it because,
[67:08] uh, the guys have been like, if you do that, you're going to get kind of confused. So don't do that, but it is a really cool show and book series.
[67:20] Let me see if I can find this in the amount of time it takes you to, uh, talk about the Expanse. But for Comic-Con one year, Sarah had us all dress as Expanse characters,
[67:41] and I'm trying to find the picture to share it really quickly. It's Jacob. Hi, Jacob. And then we can go back to talking about databases. We will get there. I mean, at least Jacob is also
[67:56] part of the Expanse crew. This is Sarah's wife, Sarah's husband, the other half of the crew. Um, yeah, we're going to get to database talk. We got one more thing to show.
[68:08] Promise. Dev, we had to take a break to sing you happy birthday as well. And well, here, while you do that, I will show everyone and catch them up and see what corrections
[68:24] we need. Because Dev and Jacob just joined. Okay. So we started talking about relational databases versus, like, unstructured. So SQL versus NoSQL. And Postgres is kind of like its
[68:51] own weird thing where it's mostly relational, but it can do a lot of crazy stuff. MariaDB came from MySQL because of some cool drama. And then Redis does a lot, a lot of times is actually used for
[69:11] caching, not necessarily as its own thing. And I don't remember where Kafka goes. So that's cool. And then there's no need to necessarily learn SQL, because, like, you know, there's so many
[69:29] tools out there that can do it for you. But to know, at least understand it enough to make your own commands so you know what to Google is one of the best things to do. And then we were comparing
[69:46] Postgres and SQL, which there's a link I sent out later. I will send it out later on. And it is comparing the two. And then I also need to put Roy's video as a bookmark because we
[70:01] talked about WordPress and it's a good reference. We talked about database first versus code first. And for Dev and Jacob, who weren't here earlier, I was talking about the T3 app, because in part of
[70:20] it, you have to push Prisma to push and create the tables within the database. And then we started talking about schemas and stuff. And I'm getting lost on database design. And we are almost there.
[70:39] When we went happy birthday, Dev, and a bit of gaming stuff. >> All right. Here we go. I'll show that picture and then we'll get back to databases.
[70:50] >> Okay. Share your screen one more time and I got you. And Dev, we can't go with Mongo. We got to start going with Ivan stuff.
[71:03] >> There we go. >> Oh, that's so fun. >> Comic-Con pictures and she's in her belter costume and I'm in my MCRN costume.
[71:12] >> That is awesome. That is awesome. Thank you for that. >> Yeah. >> Actually,
[71:19] a lot of people that I work with came from Mongo. So, you know, I got to learn them though. I got to learn them. No matter what, I have to learn about all the databases, no matter where I work.
[71:33] I need to understand databases. So, that brings us to the super fun Excel draw board where we are talking about design. I think we're on to design.
[71:45] >> Yeah. All right. >> Okay. We have design. >> Here we go. So, the other thing you're going to want to have open, not necessarily,
[71:56] you can put it on the other monitor or whatever, is your diagram that you had of your... >> My funny diagram. Give me a second. >> No problem. That's the one.
[72:09] >> If we do this, we can do this. And then we can do this. >> All right. >> There. And voila.
[72:18] >> All right. >> I don't know if I'll need that stuff, but... Really quick, just for those who have just joined, I feel like Jacob knows about a
[72:30] lot of this stuff because Jacob got stuck helping me with this website. This one. This one was such a pretty website that I killed because I'm no longer looking for work and I needed to update
[72:44] my website anyway. But it was a lot of really hard work. Thanks, Astro. I do appreciate you. I built a lot of JSON things. And this is my new website. And I want to be able to say, hey,
[73:00] everyone, go to my website. So, that way, people who are here for the podcast start looking at TeachGen tech stuff and TeachGen tech stuff will look at the podcast stuff and it will be fun and
[73:12] I can make them all the same processes because right now everything's frozen and I don't do anything with podcasts. That leads us to this page, which I should probably change the order
[73:21] of that. Oh, yeah, they're the same order. Yay. The TeachGen tech. I want these five things in every single one of them. Let's make this bigger. View to embed, episode description, guest contact,
[73:38] associated links, and transcript. Which we just found out about Whisper. So, I want to see if Whisper AI can auto transcribe and put it into the database. That is a question for another time.
[73:51] It sounds really cool. And then the second one, there's a little bit more needed because we need the Apple podcast link and the Spotify link also in the podcast one. But they also, to me, in my
[74:07] head, are two different shows. So, this is where we're at and Excel a draw. All right. So, a lot of times, and that probably isn't going to be the case here. So, people don't really need to be
[74:25] logged in to look at these things, right? There's no reason for them to be. So, we can ignore users and permissions and all that. That's usually where I like to start when I'm designing a database. But
[74:39] almost every app I've ever created has required some kind of there's been a reason to have users and accounts and things. We don't really have that going on here. So, we're just gonna go with
[74:56] starting on we just need to pick a place to start. Let's start with shows. So, right now, you have two shows. You have... >> I don't know why I don't have a D there,
[75:12] but it shows me a D. >> I don't see a D on my side. >> That's so weird. Well, we'll just have two Ds on mine. That's fine. Whatever.
[75:23] >> All right. So, the first thing is gonna be a show. So, we're gonna have shows. Because right now, you have TeachGenTech and you have shit you don't want to talk about. But what if you decide
[75:35] to spin up TeachGenGaming or Gen's Crazy Phoenix Adventure or... >> iRollToDev. iRollToDev. That will be another one. Anyway, please continue. >> Yeah. So, for now, let's say... And this may
[76:00] or may not be the case. That's the other thing. Is never let your database diagram become... Don't write a bad app because you made a... It's a plan to deviate from. Don't...
[76:19] This is not written in stone. It's written on a screen. It can be deleted, erased, updated. This is for getting our heads wrapped around this. I've seen too many times
[76:38] such dogmatic adherence to a database diagram to the detriment of the final product that I feel the need to express my warning about that. >> Ah. >> This is a plan to deviate from.
[76:55] >> Okay. >> So, here... With that... Because when you go to build this thing, you may decide it makes no damn sense to have a show table.
[77:07] Shows... You know, it can just be a field in one of these other things or something. But for now, let's say there's going to be a show table in the database. >> Okay. >> So, I... I'm going to do the
[77:23] first one just so you can kind of see what they often look like. So, I'm going to write show in tiny ass font. How do I make that bigger? >> I can, like, super zoom. Wow. That is, like, so small.
[77:41] >> I used the text tool instead of the writing tool. >> And that's fine. Look how much I can, like, zoom in. It'll be fine. >> Yeah. That's just... Yeah, that's a little wacky.
[77:53] >> And yes. That is something because Jacob, like, said in another way of what you said of, like, diagrams are only useful if they represent the needs accurately and needs change.
[78:14] >> Yeah. Love that. >> And I need to not... On a lot of this, I get, like, analysis paralysis because I'm, like, but what about this? But what about this? And I'm not going to think about this.
[78:26] >> That is where the fucknuttery of database design begins. >> Fair enough. Fair enough. I am... >> All right. So... >> There we go.
[78:41] Will you do that? I'm going to log in here to try to make this a smaller screen. >> There we go. I got an Excel font size. That's better. >>
[78:55] Log in. Yay! >> And this is something that we talked about earlier and I'm excited about learning more about is,
[79:12] like, what is the, like, what schemas can go into, like, how many schemas can you have? How many databases can you have? Or not... Well, yes, databases, but also how many tables. And so it is
[79:32] good to know. >> The answer to both of those questions is as many as your server can handle. Can have as many databases and tables as your server can. >> There we go. Yay. Okay.
[79:48] >> But that is a thing to look out for is overtabling. If a table only has one column and there's never going to be a reason why it would ever have a second column,
[80:03] it probably doesn't need to be a table. >> And the reason why we would have... And I think this is something that's going to help is the way that I visualize, like, the show
[80:18] and things is I'm, like, each show would be... I don't know. Now I'm having a hard time saying it. I don't know. I'm going to wait until you have that part done and... >> All right. So we've got
[80:35] a show. And every show, every thing, and some people don't write this down. They just take for granted. And that's up to you. Especially when you're in the beginning. I like to... And I still
[80:50] do it, frankly. Every show has an ID. >> Okay. >> And that's because... It's unlikely with show, but we're going to use it. What if there's somehow two shows called TeachGenTech?
[81:07] Or better example is maybe later we have, like, a viewer table of people who watch the show regularly. And maybe there's two people named Chris Martinez.
[81:23] So you need an ID to make damn sure that everything in your database is unique. >> Okay. >> And then Lerner just asked, is show as a super type? >> Yeah, I haven't even gotten into typing.
[81:41] Show is a table. In this example. >> Cool. >> So every show has an ID. And every show has a name. >>
[81:59] And a heads up, y'all. We are both using a tool that is a bit newer of the Excelidraw. I've used it before with Ben Gamble when he was on the show. So if we're both like, what? That's why.
[82:19] And thank you, Lerner, for joining. Yes, please get some sleep. And I will tag you when I post it on Twitter. So that way you get the notification. >> Yeah. All right. So every show has a name.
[82:39] Now, every show also is shown on a channel. So like this show is on Twitch. But it's going to be on YouTube later. And I think it might be live streaming on YouTube now. >> Actually,
[82:56] no. I'm just doing Twitch right now. But yes, I have before. >> So that means that a show can have many channels. >> Yes. >> So we probably should not have channel
[83:16] be a column because a show can be on many channels. >> Okay. >> And a channel also has an ID and a name. So now we could say, okay, does this channel have a list of shows?
[83:55] Well, yeah. More than one show can be on the same channel. But one show can also be on multiple channels. So we need a way to store that relationship. Because this is a relational
[84:08] database. So we're going to make what's called a many to many table. And it's going to be called show channel. And it's going to have a show ID and a channel ID. And that ID is going to come from
[84:46] here. I'm sure there's a way to make these curvy. >> And then Lerner just said same for podcast links. No need to have columns for iTunes and Spotify, which we may reach there. Oh,
[85:01] yeah. Because they would be a channel, right? >> Yeah. >> Like they would also be channels. Okay. >> Yeah. And so this you'll notice the show channel table does not have its own ID.
[85:15] It just has a show ID and a channel ID. And that's because that in and of itself will always make a unique value. You would never have two of the same show on the same channel. It's not
[85:30] possible. You can't have two unique teach gen techs on Twitch. And so by virtue of let's say we're using numbers for our IDs. Most of the time it's this long string of randomly
[85:46] generated crap. But we're going to say that it's a number because it's easier. And some people do still use numbers for IDs for certain things. So teach gen tech is show number one.
[86:01] And Twitch is channel number one. So the show channel table is going to have a one and a one. Shit you don't want to talk about is show number two. And Twitch is still channel number one. So
[86:17] you're going to have a two and a one that's a separate thing. So that denotes teach gen tech is on Twitch. Shit you don't want to talk about is on Twitch. Now we have YouTube as another channel.
[86:33] And we've decided that because of YouTube's algorithm, they won't even monetize a show called shit you don't want to talk about because they don't like the word shit.
[86:41] So we're not going to bother. We're not going to bother putting those on YouTube. They're only going to be on Twitch. So there's going to be another one for teach gen tech and YouTube,
[86:54] but not one for teach gen tech. And sorry, not one for shit you want to talk about. And YouTube. Does that does that make sense? Do you I can also like write out what it would look like with data
[87:07] in it, if that's helpful. Um, here, so go away. I'm doing it on my tablet really quick. I know nobody can really see me. But hey,
[87:25] so if it's like show ID would be like, so let's say it's this is a shorthand that I yeah, I guess maybe show me the first one because it's not 100% like clicking.
[87:47] No problem. So I'm going to write this on here, but I'm going to like delete it afterwards, just so it's not taking up space.
[87:56] I mean, we can zoom in and out. Look how much space we have. We have lots of space. It's not let me reword that. It's not that I don't want it taking up space. It's that I don't
[88:11] want it creating confusion later on. Fair enough. Fair enough. So, and it's gonna be ID one tech. And now we've got another show to let's see, let me look at the stream. Okay, yeah, it's on there.
[88:47] I'm looking at the whiteboard on a different screen that's covering up the stream. Make sure it was showing. Yeah. And now we've got, whoops, that's a dot, not a text.
[89:00] Channel ID one, two, and twitch. T-W-I-T-C-H. I don't know how to spell twitch. No, wait. Yeah, that's right. There you go. All right. So we got twitch, we got YouTube,
[89:43] we got teach gen tech, and we got shit you don't want to talk about. So now we need a way to denote teach gen tech on YouTube. Yeah.
[89:53] Channel ID one, channel ID one. There, I'm drawing them. Nice. I was like, this will make more sense because for some reason, as it's, you know,
[90:16] probably not that distracting for others, but I'm like, it's covering stuff. So I'm having a hard time paying attention to it. There we go. >> So this shows.
[90:40] >> So this is. >> That works.
[91:17] >> Come on, you little bastard. There we go. >> Right? Like, it's like, I'm going to have like a hard time with everything. It's cool. We will become Acceladraw masters eventually.
[91:38] >> Yes. If anyone is an expert at Acceladraw and wants to be on the show. >> That would be fun. And learner just said foreign keys already covered.
[91:54] >> Yeah. So that's what this is called. And I'll explain that once it's drawn out. That's where I was going with this is what a foreign key is. But I wanted to show the example first.
[92:04] >> That works because I'm like, I don't know what a foreign key is. So that's cool. All right. So in this
[92:41] nightmarish drawing, we have teach gen tech. And we have teach gen tech on YouTube, which is show ID number one for teach gen tech and channel ID number one, which is YouTube.
[92:58] Those show IDs and those channel IDs are called foreign keys. And it's saying, hey, I'm using the ID of another table to show a relationship. >> Does this make a new table then?
[93:17] >> Yeah. So these are and none of these things are tables. These are all rows in the table. So these are all the table. These are like the header names.
[93:30] And these are all rows if we're using an Excel spreadsheet as an example. So these are the names of the columns. And these are the actual values.
[93:40] So yeah, those now let's say we've decided, you know what, this multi channel thing is confusing. We don't ever want to do it. And I'm not saying that's true. But for the sake of argument,
[94:00] we've decided no show can ever be on two channels. But one channel can have multiple shows. So if we do all that, I'm going to move. Do you if you want me to save this, I'll save it.
[94:15] Let me see if it will let me move it. Yes. >> I think you should be able to. >> Okay. So. >>
[94:27] But if it's easier, I can. Oh, there you go. >> And I'm going to label this many example. >> Yay, thank you. >> Over here. We're going to have
[94:50] too many example. So in this one, instead of the show being able to be on multiple channels, it can only be on one channel. We have moved to syndication. In fact, I'll use TV shows as
[95:11] an example. You just got teach Gen Tech the TV show instead of the YouTube. >> Yes. All right. This is exciting. We're moving up in the world.
[95:32] Channel ID is one. And channel. Come on, you little bastard.
[96:00] Let me write. I will end you. There we go. I just had to threaten it. >> Sounds about right.
[96:08] >> So make another channel. So teach Gen Tech, because that's how the TV world works, can only be on one TV network.
[96:33] They don't play nicely together. So it won't ever be on NBC. So in that case, instead of having this one many to many relationship, we have one to many because
[96:45] CBS will have multiple shows, but each show will only be on CBS. NBC will have its own multiple shows, but each of those shows will only be on NBC. >> Okay. That's making sense.
[97:04] >> And I'll just write one more to drive the point home. And one more.
[97:36] So now you have two shows on CBS and one on NBC. So does that do a good job for you of illustrating the difference between a one to many and a many
[98:00] to many relationship? >> Yes. I think the next part that I'm stuck on is just like visualizing how I would write it out and actually create the databases.
[98:10] >> Right. And that's what we're doing up here. >> Sweet. And let me scroll up for everyone, too. >> Yeah. So this here is a many to many because multiple shows will be on multiple channels.
[98:24] >> Yeah. >> And if you want to drag all that other shit out of the way for a minute, this is about to get big.
[98:32] >> The top part? >> Yeah. >> Okay. Hold on just a sec. Look, it's going to be really far away. And I don't leave it. Sweet.
[98:43] >> It's there to get at later. All right. So we have our show table. We got our channel table. And we've got our show channel relationship table. So that covers our
[99:02] both, you know, our part that talks about teach gen tech and our part that talks about shit you don't want to talk about in your other diagram. That covers YouTube. Oh, so let's talk about more
[99:23] things that a show is going to have. And this is where someone might come fuck me up in the comments about how I like to do this. Every YouTube well, no. So that's an interesting question.
[99:51] YouTube embeds, those are all episodes, aren't they? They're not >> Yeah. I mean. >> It's not a link to your
[100:00] YouTube channel as a whole, is it? >> Right. Like I might want to do like a playlist later on, but mostly it's yeah. >> Okay. So now that brings us to yet another
[100:16] episode or another table. I said episode because I was looking at it. So we're going to have an episode table. And like all things, it is going to have an ID. Does it have a name?
[100:42] Do you name your episodes? >> I mean, like this one. Yeah, because I named this one like teach gen database. >> Yeah. YouTube makes you. Yeah. The video has
[100:54] to have a name. And it's got a link. >> Lerner, I don't know if I know what you mean by your comment. >> Let me see the comment.
[101:06] >> Sorry, design changes for episodes. >> Yes. Because the other thing was talking about the show as a whole, not about the individual episode. Now we're doing individual
[101:21] episodes within a show, which is also nice because it lets us illustrate a one to many relationship. >> I get what you're saying. >> So that's and that brings us to our
[101:35] previous question of do you and this is the part where do I risk painting myself into a corner? Because you could say show ID and say every episode only exists on one show. This
[101:59] live stream that we are doing will only ever be on teach gen tech. It doesn't matter what else we talk about. It will only ever be on teach gen tech. And in that case, we have a show ID column,
[102:13] and it's going to be the ID for teach gen tech. >> That's accurate. >> But do we ever think that the situation might arise where a show episode either because it's a
[102:33] very special episode of teach gen tech in which Chris learns to stop smoking or is it and that becomes an episode for both shows? Or is there no way in hell that's going to happen? And even
[102:49] if Chris learns about the dangers of secondhand smoke in this episode of teach gen tech, it is staying on teach gen tech, damn it. And neither thing is wrong. What could happen is we have
[103:04] over complicated, over designed our database for a scenario that will never happen if we make it a many-to-many table or we have shot ourselves into a foot and painted ourselves into the corner when
[103:18] we finally reach that day where the very special episode of teach gen tech happens and we wanted it to be on both shows. And that is a question that you just, there's not a right answer or
[103:31] wrong answer. >> But if I do that, I could just input it twice, right? One for teach gen tech and one for.
[103:38] >> You could, you absolutely could do it. >> Like if it is a one-off, because it wouldn't be a regular thing. It might be a one-off, but if I need them to show up on both,
[103:49] then I could just create it twice. >> And there's an example of why ID matters. >> Okay.
[103:55] >> Because those are both going to have the same name, but they're going to have a different ID and a different show ID.
[104:03] >> Mm-hmm, mm-hmm. >> And there are people who will tell you that the same name, but a different show ID is enough to differentiate. I don't personally like
[104:12] to work that way. I like the definite unique ID, except in my many-to-many tables where there is not a way for them not to be unique. >> Okay.
[104:24] >> All right, so this ID goes down here. Sweet. So we're going to do that then. And yeah, cool. If there's a very special episode, it will just get two entries, and that's totally acceptable,
[104:43] especially if you're not doing it a ton. Yeah, business decisions, that's exactly what you call these, where this, that. And it sucks because the one you really thought you thought out all the way
[104:58] is the one that ends up with this fucked-up edge case that happens all the time after some milestone, and you end up having to either refactor or have, like, dead columns in your
[105:13] database. And there's just no avoiding it. It happens to everyone. No one has ever, to my knowledge, in the history of humankind, ever designed a perfect database the first time.
[105:26] >> I wish. >> Everybody's got a database of dead tables or dead columns or un-normalized data. It's got to happen. And the quicker you can
[105:41] come to terms with the fact that it is going to happen, the, oh, you can bend these. Hell yes. >> That's amazing. That is amazing. >> What color is this?
[105:56] >> The green one? >> Yeah. >> I don't know. On my tablet, it just gave me color options.
[106:04] >> Oh, it didn't give you a hex code? >> Let me, hold on, hold on. >> Let's see if I can guess. Let's see if my design is still where I thought it was.
[106:12] >> Oh, okay. You guess, and I will tell you if you're accurate. >> Maybe just a little bit blue. Nope, that's too green. Oh, let me.
[106:32] >> Would you like me just to tell you what it is? >> Yeah. Wait, let me try one more time. >> Okay.
[106:38] >> Oh, that's closer. But yeah, go ahead and tell me. >> It's 087F5B. >> All right. Sweet.
[106:53] So there you go. You can apparently grab this little, like, knobby thing to bend them. >> Sweet. Now we know. >> Precision arrows. Sweet. All right.
[107:07] So now we would just go through and do these for all the rest of them. And there may be more attributes to an episode we decide later on. I'm just trying to show you,
[107:24] like, the basics. If we actually spin up a database today, I fully expect us to blow it away at the end of the episode. Like, not, this is, this is a four-hour exercise,
[107:38] if we want to completely. >> Yeah, yeah, yeah. But if we do, so we got the name, we got a link, we got a show ID. The link would be the YouTube embed?
[107:56] >> Yeah. It would be the URL to that episode. >> So would I then, instead of using, like, link, would I say YouTube embed? So that way I knew what that link was supposed to be.
[108:13] Especially, like, on the podcast one, there's more than one link. >> So if there's multiple links? >> Yeah, like.
[108:27] >> One episode. >> Yeah, let me, give me a second. >> Okay. So there's, there's a few ways to do that. And that's totally
[108:43] interesting. Because there's a, so you can either have a link table. >> I don't know if I like that. >> And it's going to be called, like,
[109:02] episode link. And it's going to have a URL and an episode ID. And you could have 500 of those. Because the internet gets real fucking weird in 10 years.
[109:15] >> Yeah. >> So that's option one. >> Okay. >> Option, and that's probably the,
[109:27] in my opinion, everybody take a drink. In my opinion, that's probably the best way to handle that. But I'm going to, I'm going to throw out some additional possibilities.
[109:40] >> Okay. >> While you're writing that all down. Another option is to make one field that's links and make them, like, comma separated or,
[109:54] like, pipe delimited. Or if you're using a Postgres database, maybe that's the time to use that JSON data type. That lets you stick some JSON in there. That's a bunch of links. I don't think
[110:06] any of those things I said are the best idea. But I want to make sure you know that those are options. When you start doing weird shit like that is when you're, like, trying to undo a
[110:17] mistake you made before. Like, you made link a single column and you made it to where it can't ever be empty. It's called a non-nullable column. So, there always has to be something in there.
[110:32] But later on, you're, like, shit, I want multiple links in these. That's when you're, like, well, fuck it. We're just going to comma separate them. But since we're nice and at the beginning,
[110:45] we're going to oh, sweet. I get what you're doing. You're writing an example. >> Yeah. Because I'm, like, I'm not piecing together exactly what you're saying. So,
[110:58] I think just getting it out. Because what I'm wondering is if, like, using I don't know what this is. Okay. There we go. Because, like, if I had it where it had the Twitch or whatever it
[111:16] would be and see, we're already changing things. Because I already thought of something that I forgot was Twitch date. Maybe these aren't the best orders. But and then description.
[111:38] So, I got let me zoom in on the stream. Is basically the I'm wondering, would I do it like this? Even though okay. >> Because maybe next year maybe you decide
[112:05] that you know what? I want to start offering my show on TikTok. Or Vine becomes a thing again. Like, do you want to have to add a column every time a new possible vector for a link comes out?
[112:25] And that's why having a separate table is a good idea. >> Okay. So, if I it would have a copy. Is there a copy option? Let me copy you, man.
[112:43] Oh, it's right there. Okay. Cool. >> And that so, that's interesting. So, maybe show and channel is not the relationship. Maybe it's episode and channels.
[112:53] And this is where database design gets extra fun and extra wacky and why it should always be a plan to deviate from and not a piece of concrete. Because now through, I'm starting to feel like
[113:14] definitely episode is going to have multiple channels. And that's also nice. Because maybe one episode didn't used to be on older episodes. Maybe they weren't offered on a certain channel
[113:33] back in the day. So, right now here's an example of where points of discussion or argument happened. In the comments we have
[113:43] learner suggesting make show and episode link to channel. And my thought process is at any point does it really matter now that we've talked this through that show and channel ever touch each
[114:03] other? Is it really only the individual episode that matters what channel it's on? And that's because a show is always going to be made up of several episodes.
[114:17] >> Yeah. >> Even if it's a very special episode. And so, my thought process is let's just make it let's just relate
[114:31] channel and episode instead of channel and show. >> So, that would mean that it would be episode ID and then it would be like
[114:49] within episode. >> Yeah. If we scroll back up to our other diagram. >> Yeah. Okay. Sorry. I was looking at it
[114:58] on my tablet. Go. Scroll. Scroll. >> All right. So, if we get rid of that arrow between show and channel, that green hand drawn one. And then we're going to rename that table
[115:13] episode channel. >> Show and channel. Get rid of the one between this one? >> No. No. >> Well, I'm going to redo it
[115:24] anyway. Because we found out that we can bend stuff. >> It's true. >> Okay. Let's see.
[115:31] >> There we go. Nice. Love it. Love it. So, we're going to rename that table episode channel instead of show channel. >> Okay. That one I'm going to do
[115:43] on my computer because it's not written. Okay. Episode. >> Yeah. And we're going to change show ID to episode ID. Now, instead of drawing an arrow from the show table to the show channel
[116:12] table, we're drawing an arrow from the... >> Like that? So, it's episode? >> So, I would draw the arrow going from the ID column of episode.
[116:25] >> Like that? >> Yeah. But make the arrow go the other way. >> Oh. Well, let's see. Hey. Not horrible. >> You can grab your middle. And I would draw
[116:41] the point of the arrow going to the episode ID column to make it clear it's the ID. It's the same value that's the ID of that episode. >> I get you.
[116:52] >> And we still also need an arrow going from the ID of the show table to that show ID column in the episode table. >> Oh, okay. That was not my plan.
[117:08] What are you doing? >> What the shit? >> That was not your plan whatsoever. >> We are learning a lot about... Today,
[117:20] I teach gen tech how to whiteboard and... >> We're learning. We're learning. All right. So, this ID... I could be a little better. Whatever. It works. Okay. This is making a lot more sense.
[117:41] And so... Then... >> So, yeah. Now we can start putting more attributes on that episode table. Like
[117:59] date is probably a good one. Air date or whatever. >> Yeah. And I figured if it shows future, people can see if it's in the future or in the past based on the date. Okay. So... I don't know
[118:14] why I'm having to do this. I have access. >> That's another piece of weirdness. So... >> You can move this. >> Let's really take a second to
[118:26] think about that. So, right... >> And the memes... Oh, sorry. Go ahead. >> Actually, never mind. I already thought through it. Because right now we're... I'll talk
[118:40] through the logic still. Even though it already resolved itself in my head. Right now we are streaming live on Twitch. It's happening right now. It's air date was May 9th. You can go back
[118:54] and watch things on Twitch. You know? Like we watched your guys' game last night. Even though it aired on Sunday. And we watched it on Twitch, not on another channel. >> Right.
[119:08] >> The air date was the same, though. When this gets put on YouTube, the date's gonna be different. >> I was still gonna put it the same.
[119:23] >> Okay. >> Because to have... And that might be something to put as a note. Like is... We'll do purple, sure. Is air date not published date?
[119:42] >> Yes. >> Okay. It's good enough. And then I don't necessarily want it to go for Twitch as an embed. Because Twitch
[119:53] video on demands go away. >> Yeah. >> Unless you make a shit ton of money on it and you can keep it for longer.
[120:00] >> Yeah. Oh, you know what else we should do is move that link over to that episode channel table. Because the link is gonna be different for each channel. The YouTube link is not the
[120:14] Twitch link. It's not the Spotify link. >> Say that one more time. Oh. Move this down there. >> Move this. Yeah. Get rid of that in the
[120:28] episode table. And move it to the episode channel table. Because it's episode channel link. >> Oh, yeah. Because it's doing a different table. Okay. Okay. I'm starting to get it.
[120:43] >> Yep. >> I'm starting to get it. I think. Sure. We're just gonna... Oh. >> Yep. There you go.
[120:51] >> Eh? >> Yep. >> Eh? Okay. So this would be link ID? >> Yeah. Probably just link. Because it's
[121:02] just the URL of that... That takes you to that episode, right? >> Yeah. But if they have multiple links... >> Right. But each link is gonna go... Is
[121:11] gonna belong to a different channel for that episode. >> Okay. >> So, here. I'm gonna write an example of one.
[121:22] >> Yes. Thank you. >> So... So, episode channel. Episode ID is gonna be... This is... Why did you say this is episode
[121:55] 9? Do you know what episode number this is? >> Probably, like, 87. We're gonna go with... >> 87. >> We'll go with 87 for now.
[122:02] >> Channel... >> Oh! >> I think in our example, we made YouTube channel 2.
[122:14] >> Yeah, I think so. >> Channel 2. Link. I know that's not really what a YouTube link looks like, but it is for the sake of...
[122:32] >> Fair enough. >> Just for fun, we'll write the whole damn thing out. And this is probably where date actually belongs. No. Date can... Well, no.
[122:44] Date belongs to the episode. Because you just said you want to use the same date no matter what channel it's on, right? >> Right.
[122:49] >> Yeah. So, these are the only things that belong in this episode channel. Date would still belong to episode. >> Okay. What you're showing me makes sense,
[123:05] because it's episode channel. What's not making sense now... And thank you, Lerner. Agreed. Now that we have this, and I'm like, okay, cool, I'm starting to keep it together,
[123:22] how would I visualize what I build? >> What do you mean? Like, how it'll look in the database or in your code? >> In the database itself. Like,
[123:40] just to go for my own brain at the moment of... Zoom out. Thank you. And we'll say... We will do orange for now. So, let me zoom back in for the orange. Because I think the other part
[123:59] that I'm currently stuck on is... We got boxes. We got boxes. We got a box. We got another box. Maybe we got another box. We got another box. And then we got another box. Let me move you.
[124:27] And then... So, it would mean that if it's show... Like, this is one table. Show ID is table. So, it's like... This is show ID. It's not a mind reader, Jen. Show ID.
[124:52] So, I would create three different channels or three different... Four different tables? >> Yep. These are all four unique tables. >> Okay. So, show... Okay. Hold on. I am
[125:11] basically rewriting what I already wrote, but in a way I can visualize it. >> Yes. >> Which feels very funny, but, you know,
[125:20] sometimes you got to do what you got to do. So, it would be ID. And then it would be whatever we have named. Yeah. Okay. This is making sense.
[125:33] >> And they're going to be written across the top. >> Oh! >> So, it would be ID and then name. And then
[125:42] I guess show is not a really involved thing yet. >> Okay. That is where I think I was getting a bit lost. So... And I feel like now that I
[125:56] kind of am visualizing it, I can just do it here. It's not something that I need to try to stay up to... Up to the speed of someone talking. That is normally why I write things out is because I'm
[126:11] like... I can't keep up with what they're talking and type. I don't want... I would like you to be a different color. Thank you. But I do need the typing. Oh, okay. So, we got show is one table.
[126:26] Channel. So, and then these would all just be one schema. >> That is... That whole collection of tables is a schema, yes.
[126:46] >> Okay. And do you create a schema... Like, do you have to make detailed directions of a schema or it learns it by creating the table? >> So, if you are doing database first,
[127:07] then as you create the table, it makes a change to the schema that says this schema now includes this table. >> Okay.
[127:19] >> And this table has all of these columns. And each of those columns has a data type. >> Okay. And is it... Is it queries that populate something that pulls the information from all of
[127:44] these? >> Yeah. Queries are what get the information out of the table or put information in the table. I mean, every thing in SQL is...
[128:02] Every, like, typed command in SQL is technically a query. >> Okay. >> Which is not a good, like,
[128:14] descriptive word. I should have called them commands. >> Yeah. But, hey. So, for... >> Actually, you know what? For funsies, since it was something you wanted to cover anyway,
[128:28] if you want to, because I know... I know we're getting at the two-hour mark, and I'm happy to keep going. I just want to make sure, A, that we cover everything you want to cover, and B,
[128:42] that we're respectful of your and everyone watching's time. If you wanted, since you wanted to cover some basic SQL commands and wanted to cover creating a database, we could go make a
[128:56] simple database with just these four tables really quick. >> Okay. >> We'll probably have to... It probably won't be a database we can, like, use in production
[129:06] later on. You'll have to blow it up and remake it later, but... >> It learns by table database first, but in code, that could be big. >> Yeah. Code first is, yeah, a different
[129:21] animal. >> Okay. So, y'all, you know I'm going to use Ivan, because it makes my brain properly... Oh. Back to dashboard.
[129:35] Hey, look, I made one five hours ago as an example. And I'm pretty sure I have PGAdmin on here. Still, yay. Maybe. Maybe. Please load. Please load. Yay.
[130:01] I don't know what that was. So... Oopsie. But good news is I'm just going to remove server group, because I deleted that one a while ago. Why? Why do you have to be a problem?
[130:20] Okay. Create server group. Sure. >> It looks like you have a server group, and you should be able to stick a database
[130:36] in that server group. >> Oh, okay. >> That's wonky. >> Right. Oh, wait. What was that?
[130:44] Deploy... Why? Refresh. No. Bro. I just wanted to delete everything. I just wanted to... Delete. No. No. Okay. Well, you know what? Hey, what's this? We'll just click random things until you
[131:05] do something. No. >> No. Let's... Fuck it. Let's start again. Let's make a server group after all. >> Well, it's... Oh. It's going to still put it
[131:20] under... What? Whatever. >> Yeah. Call it TJT. It'll be great. >> Yeah. And then connect now. Yes. Host name. Address. Must be specified.
[131:32] >> Go to connection there. Try typing local host. See if it'll let you do that. >> Local host. >> And that's just saying
[131:46] host this on the machine right now. >> Yeah. And then... Okay. Save. Crypt key is missing. Oh. Would you do that as the IP address for the... Is that the default local host?
[132:05] >> No. It might want something. And it's been a good while since I've made a Postgres database, not code first. So, forgive me for not being as sharp on this anymore. Crypt key is missing.
[132:27] Is it under that? >> I don't even see something called "crypt key." Connection. Go to advanced. See what's in there.
[132:49] Oh, we got comments. Maybe someone knows what the hell they're doing. >> Yeah. Learner. I was like, wait a second. Doing locally would be easier instead of all
[133:02] these off prem stuff. But if I do it this way, it shouldn't be too hard. Because this is just a service URI. Okay. Let's see if... I don't think you're gonna import everything for me.
[133:18] Quick connect. >> Oh, well, there you go. Use that. >> PgAdmin. >> Okay. Copy that JSON.
[133:28] >> And... Okay. No. That's not what I want. >> It's saying in PgAdmin, go tools, import, export, servers, and then copy that JSON file in there.
[133:50] >> Okay. So, we are going to do... Yes. We want to lose everything. Click on tools, import, export. That was exciting. File name. Oh, I still have to create the file.
[134:07] >> That's fine. Just save that as something.JSON. Just open, like, VS code or something. >> File. New text file. But not there. No, this is in a different project.
[134:40] >> Yeah. New window. That will open it in a new, like, space. >> Thank you. New file. Text file. >> There you go.
[134:53] >> We want to file save as. Thank you. This is today's. And we are going to put it in the right folder. Maybe we're going to put it in the right folder. I would like to put it in the right folder.
[135:10] There we go. Save. That was very exciting stuff. Here we go. Here's the JSON file. And next. And we'll put it in group test. Next. Finish. Okay.
[135:29] >> All right. Now click that dealio. And. >> I think. It should be this one. Oh. I didn't put the password in, I don't think. Connect server.
[135:54] >> There you go. And then put that password in there. >> Okay. No. Why are you. Yes. That's fine.
[136:08] Okay. Now we get that one. Save this password. Okay. Good news. We got it. We are good. We've got the database going. So, let me go back over here.
[136:30] Fantastic. So, we have our table spaces. Databases and table spaces. That's not confusing whatsoever. >> All right. So, let's make a new
[136:50] database. Excuse me. >> Create a new database. >> And call it whatever we want to call it, yeah. >> Okay. Do we need to go through any of these
[137:04] other things? >> Let's look at security and make sure it doesn't want a password right now. Okay. It doesn't care right now. Go ahead and save.
[137:10] >> Save. >> All right. So, now. Right. So, if you click on schemas right now, which is down there. And click the little arrow.
[137:23] Cool. If you go down to tables, there may or may not be a default table that it sticks in there. It doesn't. >> No.
[137:31] >> Sweet. So, we're going to make a table two ways. The first way is, yep, by doing create. >> Table. >> Yep. Cool. And pick one of those ones we
[137:47] want to create. >> I'm going to do them in the order that we do. Do I select a table space or anything? >> What are the options in there?
[137:58] >> PG default. >> Just leave it blank if it'll let you. All right. So, now we got columns. And this is where we start sticking shit in here.
[138:12] >> Okay. >> And have an ID. That's our favorite. So, click name ID. All right. And then data type is going to be if you want it to be a number,
[138:28] just have it be an int. Or it probably doesn't need to be a big int unless you're just getting crazy with it. Or a string. >> Oh, wow.
[138:38] >> Yeah. There's a lot of data types. >> It doesn't have a regular integer? >> Doesn't have it. >> Interval. Integer.
[138:47] >> Integer. That's the guy. Cool. >> Okay. >> And we want so, two things. Do you see those two little switches there?
[138:56] >> Yes. >> Not null. We definitely want that. We want to make sure that nobody can ever create something in there that doesn't have an ID.
[139:06] That would be disastrous. >> Okay. >> The next thing is this primary key column. Most databases and database tools will
[139:17] lose their mind at you if you don't call something your primary key. And it's typically the ID. >> Oh, yeah. It's the first column. >> The primary key is that column
[139:27] that identifies a unique entry. >> Okay. Cool. >> So, go ahead. >> And then the next one is name.
[139:39] >> Yeah. >> And that one is a string. >> It could be either string or text. It might be called text. Yeah.
[139:47] >> What's the difference between the one with a bracket and without the bracket? >> I have no idea what the one with the bracket is, if you want the truth.
[139:52] >> Okay. Because the other one had it. So, let's do that. And we don't want these blank. It is not the primary key. >> Right.
[139:59] >> Okay. So, there's -- >> Oh, it's apparently an array of text. Oh. Well, that'll get wacky. >> Well, let's see if I can get rid of it.
[140:08] >> Yeah. See if it'll let you -- if not, I'll show you how to change it. We'll learn about alter table. >> Properties. Columns.
[140:20] >> Sweet. >> We just want regular text. >> Yeah. >> Yeah.
[140:25] >> Maybe. Bro. >> Delete, like, all of it. >> I'm just going to -- yeah. I'll just delete -- yes.
[140:34] >> Oh, that works, too. >> There's nothing in there. >> Yeah. >> It wouldn't let me delete
[140:41] what was in there. So, I was either going to rename it something. We don't want it as null. We are going to hit save. >> Yeah.
[140:48] >> And then do the same thing for the other four or three. >> Yeah. So, the next one we're going to do by SQL command just to do it.
[140:58] >> Oh, God. Okay. SQL. >> Yeah. >> I'm guessing this is where I go. >> Yeah. All right. So, I just put in
[141:08] to the private chat, but you're welcome to put it in the public chat, a link to the W3Schools SQL reference. Honestly, like, as simple as it is, like,
[141:22] this is probably the best, easiest to understand SQL reference I know of. This is going to be generic SQL. It's not going to be anything Postgres specific.
[141:37] But it's going to work 99% of the time in every flavor of SQL you're going to come across. And, in fact, this is how 10 years ago I learned SQL is through this tutorial.
[141:54] So. >> Oh. >> Lerner, I miss that you said alter table implicitly. >> That's a command. We're not
[142:08] to that yet. We'll get to what all those things are. >> Okay. So, we are going to use select from customers? >> No. So, that's just an example of a SQL.
[142:22] >> Oh. Okay. Thank you. >> Can you make it bigger so your hamburger menu is expanded out? Or just drop your hamburger menu. That works, too.
[142:31] So, SQL create. Scroll down. Keep going. >> Great table. >> Yep. All right. So, let's talk about
[142:54] what each of these things in here are. >> Okay. >> So, create table is just the create table command. It's what you do when you make a new
[143:07] table. And you give it a name. You write the name of the column and the data type that it is. And this is the simplest way to do it. If you look in that SQL thing that's
[143:24] that was just there a second ago, Beck. >> Yeah. It wouldn't let me type. Like, I can't type anything. >> Oh, that's weird.
[143:33] >> That's why I was oh, but I think it's because I'm in the table, not the schema? Maybe? >> Right click on the database itself for a second.
[143:51] >> Database itself. Oh, there we go. >> There's okay. It's not in there. Go down to the table name and right click. >> I didn't right click. Oh, to tables.
[144:12] >> Yeah, right click query tool. That's what we want. Sweet. This will let you type. >> Yay. Okay.
[144:21] >> Whatever the hell you want. Sweet. All right. So, now we're going to create a table. All right. So, this one is over here somewhere. Channel. Channel.
[144:42] I'm going back to the reference. It is column one is ID. Column two is name. I need to change their data types. >> And we're going to add
[145:00] what are called constraints. It looks like it also stuck a bunch of dots in there that we don't want. >> Text. Bunch of dots. And yeah, how do I tell it which one? I bet it's in here.
[145:14] >> That is exactly the right question to ask. How do you tell it which thing is a primary key, which thing is a foreign key? So, let's go back over. >> I don't know. Can you look what
[145:29] learner just said? Before primary? Yeah. >> Chiger. Chintiger. I don't know what that means. It may not be in there. Oh, integer. All right. >> Oh. That makes so much more sense.
[145:55] >> Okay. So, it wants you to write out the whole word integer in Postgres. Okay. >> Thank you. >> That's good to know. Because
[146:03] I would have wrote int as well. All right. So, now if we hit another space after integer. >> Before the comma? >> Before the comma, yep. And type PK.
[146:14] It may make you capitalize it. But we'll try it without. And that. >> I was just seeing if it changed colors or anything. >> Yeah. And that tells you it's the primary key. And then if you
[146:32] hit another space, because we want the next thing is real important is not null. And I believe it's with a space. >> Not a dash?
[146:43] >> Not a dash. That is one kind of wacky thing is there's like a lot of places where spaces are okay. So, hold up. Oh, that's all right. Now we get to learn about. Okay. Apparently it's not.
[147:01] Oh, apparently you write primary key all the way. Oh, after commas. >> She's primary key. Oh, yay. It's pink. Oh, look. It's Josh. And hi, Josh and everybody.
[147:24] And for everyone curious, Josh is going to be on the show on Friday. What up, Chrissy? We are learning databases. We have done a lot. We have been streaming
[147:38] for a while. >> Okay. Apparently primary key goes all the way at the end. It's been a long time since I've written this out manually.
[147:47] >> Oh. Column type. Column one. Column two type primary key. How will it know the first one is primary key, then? >> See how it has ID in the like
[148:00] parentheses there? >> Uh-huh. That makes sense. >> Yeah. >> That makes sense.
[148:08] >> Let's make sure that text is or name is also not null. >> Okay. Yes. Learner, thanks for coming to hang out. Appreciate it. And good night. Especially
[148:21] because you were going to leave like an hour ago. I do enjoy that you were able to come. >> Sorry we kept you up. >> Yes. Yes. Not -- oh,
[148:31] I don't need caps. Not -- >> So you don't have to type caps, but that's generally like the convention. >> Is caps?
[148:38] >> You'll see that SQL -- like if you look how your create table is in caps, SQL -- no SQL thing that I know of gives a flying fuck about capitalization, but that's just like the
[148:52] convention that most people follow. >> Okay. Okay. Well. >> So now write primary key. >> Let's see. This one is in all caps.
[149:06] Primary key. And then -- >> And then a parentheses with ID. >> There you go. And that's telling it the ID -- it's saying create a table with an ID
[149:19] column that's an integer and a name column that is a text. Neither one can be null and the ID is the primary key. So now -- >> This is -- yes.
[149:33] >> Yeah. >> And let's run it. Yay. >> All right. So now if we go back and look in our tables, we may have to refresh.
[149:43] I think there might be a right-click refresh. >> Yay. Yay. Okay. So the PK style reminded learner of MS Access. I'm guessing Microsoft Access. >> Yeah. So Microsoft Access used to be
[150:08] like part of Microsoft Office. And it basically made like a weird ass like halfway SQL database that was like localized to your machine. And it was usually used by companies in place of like a
[150:24] CRM before they got popular. >> Yeah. >> Their own access databases with their customers and shit in them.
[150:31] >> I remember this now because I could never -- yes. Yes, Josh. Everyone knows Excel is the best CRM and database. >> You're right. It totally is.
[150:45] And just as a very quick update for everybody that has joined us, we're going to take a quick pause to be like, hey, what have we done so far? Because we've been streaming for a while.
[150:57] And oh, I need -- if we go back here and go over here, we have gone through a lot. We started with relational versus unstructured databases. And that like relational uses
[151:22] structured query language and unstructured or semi-structured is NoSQL. And then it's I don't even think I can like switch back and forth as well.
[151:38] With the structured query, the reason we're learning some SQL is so that way we can query things ourselves in case there's an error even though there is a ton of options out there in
[151:52] the world. And then we talked about Postgres versus MySQL. And there's a link that I will share later on about that one. Then we also talked about database first and code first.
[152:08] And right now we're creating databases first. Because talking about these schemas and define the columns and like what it takes, you technically can have more than one schema per
[152:29] database. But it's never really been done. But in theory you can. And so that got me to trying to understand what we are doing with designing things. Which is never a great way to go into
[152:45] things because then I got really stuck on this -- I won't confuse you with that. This is what my website looks like. And it's been built by Brutal on Brutal on Astro. And eventually I will
[152:58] have the creator that I'm not going to butcher his name today on the show. But I was like, I need these to be built out. We need to build these. This is cool. I didn't know they were all
[153:09] different colors. Anyway. So we go to our lovely Miro board. What did I do with my Miro board? Oh, I think it's in a different window. So many windows. Okay. There's probably another one on
[153:28] here. There we go. And we were talking about all the things we want to have in teach gen tech and shit you don't want to talk about. Because that's my podcast. And there's a bunch of shit that we
[153:41] need in both of them. And then we went to -- again, too many windows, gen. Too many windows. Why do I have to have so many windows open at once?
[153:53] Then we figured out that we need these four tables. This took a while because we also talked about one-to-many and many-to-many type of databases. And we'll go into that more later.
[154:17] But right now we are creating these so we can kind of see a visualization of them. And Learner, you are right. It probably will help me a lot. I also need to learn how to be ready to
[154:32] showcase where we're at. Instead of, you know, floundering because we had new people come in. Because it's always exciting when new people come. All right. And we are in PG admin and we created
[154:47] channel and show. Channel we created through SQL command. And show we created through right clicking and hitting create. Bam. I think that catches this up.
[155:02] >> Sweet. >> So I need to create two more tables. >> Yep.
[155:09] >> Which were on these ones. So -- >> All right. So now do you want to create the episode table through a command or do you want to use the table builder?
[155:29] >> I think the table builder is way easier. So that means I have to do it through the command or I'll forget how to do it through the command. >> All right.
[155:38] >> But now that this one is built, can I just replace it? >> Yep. >> Okay. Cool, cool, cool.
[155:45] All right. So we have episode. We need to do episode first because episode channel uses -- >> Yep, yep. >> Cool. ID, name, show ID.
[155:56] >> All right. And for those watching, I'm going to not tell her something critical so that I can show her how to do an alter table. So save your pitchforks and screaming.
[156:09] >> No. Can we just add it to reference it? >> Put it in there, yeah. >> It's not Twitter. But okay. Hold on. I need to name an episode.
[156:22] Episode. >> Yep. >> And then -- wait. I want -- maybe -- ah, damn it. Well, I haven't looked at it yet.
[156:40] I haven't looked at your comment yet. I'm going to do this and then see if I can create a database. Oh, wait. No, I want to reference.
[156:54] >> I will tell you this. Right now, if you run this command, which I do want you to do right now, after you finish giving it its data type and it's going to be an integer because that other ID
[157:11] is an integer. Now -- >> Well, then you can type. >> Yep. Here's another question. Can a show -- can an episode -- and I think the answer is no,
[157:24] but can an episode exist out on its own without being tied to a show ever? >> Yes. Because if I do, then it needs to be null. Because if I do an episode, like,
[157:39] to reference a show I was in, it should not -- >> So just -- there you go. Just integer. There you go. So now run the query. And it will run. And it will create a table. Cool. So now here's
[157:57] what we're missing. Is it does not know right now that episode and show are related. >> Right. >> That show ID is
[158:11] supposed to be calling for another table. And that's what I was telling everyone, hold up, that's why I didn't -- I intentionally did not tell her to make the foreign key.
[158:21] Because we're going to alter the table now. We're going to fix it. Or in this case, didn't know. And that's okay. >> Database. Table. Alter table.
[158:34] >> Alter this table to give it the foreign key. >> Okay. Alter table. So I would delete this, right? >> Yeah.
[158:44] >> It doesn't show delete, which is weird to me. Alter. And then we are going to episode. Episode. And then I'm guessing brackets. >> All right. And it's parentheses. Yeah.
[159:04] >> Parentheses. Okay. Are these parentheses? No, it's parentheses or dots. Which ones are parentheses? These are parentheses, right? >> Yeah. The smooth ones are parentheses.
[159:18] >> I do not know why that confused me so much. Job column. Would I do alter column? >> Actually, go in there to the -- on the right, scroll down more and find the one that says
[159:34] foreign keys. Back in your W3 schools. >> Foreign key. >> Yep. And then if you scroll down, there's an alter table example for making something a foreign
[159:45] key. >> Oh, okay. Let me make this bigger for everyone. And I will also copy and paste this one. Okay. So alter table. Add
[160:01] foreign key. Oh, so it's -- okay. Give me this. This is what I want. >> Yep. So we're going to change that to -- >> Show.
[160:18] >> ID. Yep. Show ID. Yep. References. And then it's going to be the show table. >> Show. And it knows that it's the table. >> So that inner part is the column name.
[160:35] So it should -- that inner part should be ID. And that should be the table name. >> Okay. >> And then there you go.
[160:44] >> I think -- wait. Would it be down there? Or would it be before the -- I'll try it. And then it will tell me if I got it wrong.
[161:01] >> Okay. It doesn't want those parentheses. Just delete them. The outer ones. There you go. >> Play. Yay. >> So now if you make the episode table,
[161:18] if you click the little thing, it'll -- I'm having to like lean in myself so I can see the -- >> Oh, let me see if it zooms in. Kind of. There we go.
[161:31] >> Okay. So scroll back down, please. >> Oh, it like jumped. >> And so now if you see, there's these columns. And if you expand that, you can see that. And if
[161:44] you click on constraints, I believe, and make that bigger, that talks about how there's the primary key and the foreign key that shows, hey, so now that shit is not that important unless
[162:08] you're getting really into it. The important part is you know that it's -- you know that it's referencing that other table. >> Yeah. I guess this is just
[162:22] me not knowing databases enough yet is I kind of guessed it would have like a pretty way to be able to see it. >> Well, we don't have any data in it yet.
[162:31] >> But it still won't show you as the columns or things just for creating the table? >> Click on the episode table itself. >> Oh, and -- okay.
[162:48] >> Yeah, this -- I don't see a good way to look at it without data in it. >> Okay. >> But let's throw some shit in there. Let's
[162:58] make a channel. Because channels are easy and they don't have a lot of crap going on. >> Okay. >> So go back.
[163:11] Right click on channel or one of the other tables and do query tool down. There we go. Yeah. That's one thing I don't like about the Postgres admin tool is that there's not a quick
[163:29] way to get a query like right the hell now that I know of. There may be one that I just don't know about. >> Like it might be like a key
[163:37] shortcut too. >> Yeah, it might be. But either way, let's throw a new channel in there. So we are going to use the --
[163:53] >> Our handy. >> We're going to use the update command. >> Update. SQL update. Okay. Well, okay. And we do this to put it all the way back.
[164:15] The table name is -- why do you keep scrolling back up? >> Oh, you're right. It is insert. Sorry, it's been a minute.
[164:22] >> Oh, yeah, because we're not updating it. >> Updating is when we change an existing. We got to insert first. >> Would it be insert into, I would think?
[164:33] >> Yeah. I don't think there is just insert. It's insert into. But most people, if you say insert, know what you mean.
[164:41] >> Yeah. Noob here. I'm like, oh, that's really what it is? No. No, it's not yet. Calm down. So we got channel. And -- >> So you can write down the names of
[164:59] all of the columns. That's really mostly only useful if you're doing some of them. >> Oh. >> If you're doing all of them,
[165:09] you don't have to do all that. Just delete that. And then insert into channel. And then values are going to be -- >> 27. And --
[165:23] >> So normally -- and this is where my reduced -- it's been a long time since I manually inserted something into a database like this. Normally it will -- okay. You have to tell it to automatically
[165:47] stick an ID in there, which we didn't when we created it. We'll save that for another day. But typically you're going to go one, two, three, four. But 20 sounds fine. It will take it as long
[166:01] as you never give something else the ID of 27 again. >> Okay. >> So go ahead and -- >> And run.
[166:09] >> Okay. I think it doesn't like -- >> Well, okay. Then we'll just do this, bro. Do this. >> Oh, you have to put -- sorry,
[166:19] you have to put single quotes around text. >> Oh, yeah, because it's a string. >> Not double quotes. Double quotes is every other programming language you've ever worked with.
[166:29] Single -- SQL, every flavor of SQL insists on single quotes. And -- >> Rude. >> -- whoever came up with that rule.
[166:38] All right. So now it worked. So now delete all that. And type select star from channel. >> Like this star or the other one? >> Yeah, that's the only star I know.
[166:58] And you've got to type from. So star. And star means get everything. So space from channel. >> And run. >> Yeah.
[167:10] >> Oh, hey! We got something, y'all. It made some things. We got some things and stuff. >> Yep. >> Ooh.
[167:23] >> So there you go. Now you can visualize what it -- what it looks like. >> I think -- I think we're doing good. And so now that I have episode -- I have episode,
[167:40] I have channel, I have show. So I would -- >> Make the episode. And let's do this one in the builder instead of doing it through a SQL query. Because,
[168:00] one, we're using multiple foreign keys. >> Can I just say that backwards? Episode channel? Episode channel. Okay. Cool. Columns. Oh, wait. Inherit from.
[168:23] >> I need to be able to put these side by side. >> See what that does. I've never used that. So I can't -- I can't promise what that's going to do.
[168:32] >> Fair enough. I can't promise what it's going to do either. But we'll give it a shot. I need episode ID. So we'll do that one first. Oh, that is not what we want.
[168:45] >> All right. Delete that. >> That was easy. >> Click the big black trash can. That should -- on the left. There you go. Does that make you
[168:55] happy? Yes. >> No. For that one. >> Oh, okay. >> There we go.
[169:01] >> All right. >> So add a row. Name. Episode ID. >> Data type.
[169:14] >> Integer. >> Integer. >> Yeah.
[169:22] >> And then not null. Primary key. >> It might do something. Don't have a default. Hit another row. Let's see if it lets us
[169:37] make a new row. You're good. Just make a second row. >> Okay. >> And make that one --
[169:43] >> Channel ID. And what's my last one? Link. Okay. Just so I can stop looking back and forth. Link. Link. And this one is going to be an integer. Integer.
[170:04] >> Yeah. >> And this one is going to be a link? >> No. It's going to be a text. >> String? Text?
[170:13] >> Yeah. You can also do Varchar. That's a different day's discussion is the difference between all the different text types. >> Oh, this is fun. Okay. I will stop
[170:29] clicking around. >> Everyone can save your pitchforks for later about which is the right one. We're just trying to get off the ground.
[170:36] So now make channel ID also primary key. >> Oh. >> It didn't bitch. Because the combination of those two is what makes the primary key.
[170:46] >> Ah, okay. I like that. But then -- >> So now we'll go over to constraints. >> Oh. >> And you want a foreign key constraint.
[170:58] >> Yep. >> Name. >> Is going to be -- >> I would create two, right?
[171:10] Episode ID and channel ID? >> Call it episode channel. I want to see what it does. No. Columns. >> Yeah. No. It's not let me -- so
[171:24] what did I just -- episode ID. No. No. Maybe. >> What happens when you click the pencil? >> Pencil. >> There we go. Now go to columns.
[171:42] >> Definitions. Columns. Local type is -- >> Episode ID. And then references. >> Episode ID. >> There you go.
[171:59] >> Okay. >> And then instead of calling that episode ID because that's the name of the other column, call it -- most of the time when it auto generates,
[172:12] it's going to call it like episode channel episode ID. It's like the name of the table and then the name of the -- yeah. It doesn't really matter as long as it's something unique,
[172:29] but it's one of those, like, conventions. >> Oh. Episode ID F key. >> Yeah. That's another -- but really it could be anything as long as it's unique.
[172:43] >> I like it. >> That looks as good as anything else. >> Okay. Specify. Oh. Episode ID. ID. At. >> Cool. So now click another one.
[173:05] >> Oh. >> Just, yeah. Delete. >> Delete. Delete. >> All right. Click the plus again.
[173:13] Or there it goes. Yeah. >> And then this one was -- >> Channel ID F key. >> F key. And then we're going to hit pencil.
[173:26] Go to columns. Local column channel. Local channel. ID. At. >> Yep. >> And.
[173:39] >> There you go. Now you should just be able to hit save and everything. >> I think I created this one as an extra. >> Okay. Yeah. Just delete that.
[173:52] >> Maybe? >> Yep. There you go. >> It's not letting me hit save still. >> Go back to general. I want to see if that
[174:03] -- oh, sorry, no. Under constraints there's multiple things labeled general. >> Oh, yeah. I think it deleted it. Like what -- but I -- what?
[174:19] >> See, this is why I like -- this is a good example of why I prefer code-first databases. >> Add. Okay. General. >> All right. Now go down to the
[174:35] next one and make sure we re-add that one. >> Channel ID. ID. Add. >> There we go. Now we save. >> Oh, yeah. Now it's on me.
[174:49] >> There we go. >> Wow. All right. >> There you go. >> Oh, I forgot link.
[174:58] >> No, we did link. But -- >> I think I ended up deleting it. >> So here's something kind of funny. >> Oh, I did. Okay. You're right. Okay.
[175:06] >> Do a select star from episode channel. >> Okay. >> Even though there's no data in it. Oh, no. Type episode channel. That's the name of the table.
[175:17] >> Oh, yeah. Episode. >> And it should. Go ahead and let it run. No. It does not like it when there's nothing in there. Some of them will give you just the
[175:32] column names when you do that. Some of them piss and moan because there's no data. >> Got it. Okay. So I think this is good at least for now. Like for everything that we were
[175:53] wanting to go over. Because we went over a lot. I mean, we did stream for three hours instead of two. And thank you for that. Thank you for that. This was extremely helpful. And I feel like
[176:06] now it's just a piece of me kind of figuring this kind of stuff out. Which is easy enough. Not easy enough. But like easy as in I can conceptualize it so I can work through it.
[176:19] Not easy like -- it's not easy. It takes time. So learner, you were supposed to go to bed like hours ago. No, you're not, too, chatty. I feel bad that it's so late there.
[176:34] I've appreciated all your comments. It's been really great having you here. Oh, see. This is good. This is good. I got to learn the sequels. The sequels. That's what I'll call it. Before
[176:46] you go to bed, learner, anything else you wanted us to cover that you had curiosities of? Or anyone else that's still hanging out with us?
[176:59] Maybe. Maybe. All right. Well, Chris, how do people reach out to you in case they want to reach out to you or anything you want to tell anybody before we raid everyone?
[177:13] I can throw my LinkedIn into the chat real quick. Sweet. Okay. Learner, we'll have to have Chris on again so you can ask him these questions.
[177:30] And let me grab this. So if anybody wants to reach out to Chris, here is his information. And we are going to raid the channel that I first did my very first PR many moons ago.
[177:52] Many, many moons ago during Hacktoberfest. So thank you all for joining. Enjoy B Dougie's channel thing. I'm a jig. And I'm going to hit end and
[178:05] [BLANK_AUDIO] 
