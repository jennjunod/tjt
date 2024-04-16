---
showLink: "https://www.youtube.com/watch?v=6W-Hkczv92U"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-prisma"
title: "Teach Jenn Prisma"
publishDate: "2022-11-01"
coverImage: "https://i.ytimg.com/vi/6W-Hkczv92U/maxresdefault.jpg"
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

[00:00] - Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech,
[00:06] or as Homie updated the graphic, Teach Gen Prisma, which I'm excited for all of those who have joined in
[00:14] on the journey of the Tweety Tag app. I think that's what we decided it was called.
[00:20] Nicholas is here joining us today from Prisma. And Nicholas, please introduce yourself
[00:26] and what the flow of today is gonna be. - All right, yeah, very happy to do that.
[00:32] First of all, thank you for the invitation, Jen. I'm really looking forward to this.
[00:35] We've talked a little bit before the stream already, and I think we're just in the perfect position
[00:40] to really get a lot out of the stream together. My name is Nicholas, I work at Prisma.
[00:46] We are a startup that is focused on building database tools. So we kind of just want to make it easier
[00:52] for developers to work with databases. And yeah, like over there,
[00:57] I lead the developer advocacy team. We have four developer advocates on the team
[01:02] currently that I'm managing. And I've been actually around at this company
[01:06] for almost six years now. So I started when we were only five people.
[01:10] We were still called Graphcool back at that time, actually, we were like kind of another company
[01:16] with another product. And then we kind of pivoted over time, everything evolved.
[01:21] And now we're called Prisma and are focusing on the database layer
[01:25] of developers applications. - I dig that.
[01:28] And y'all, in case you were curious, like I ended up using Prisma because Anthony said so.
[01:36] This is my like answer to a lot of stuff is Anthony told me to do it.
[01:41] Anthony said so. - Straight from the horse's mouth.
[01:45] - So he does know that half the time. Those are like the two things I say all the time
[01:52] is or Ben D. Myers is always says things about accessibility. So I'm always like, what would Ben do?
[02:01] And then because of like making sure I have my alt text and stuff and then Anthony made me do it
[02:07] is the other thing I say on repeat. So, and what up Ryan and Anthony, yay, you're joining us
[02:14] as I'm talking about you. - All right, it's so fun to be on StreamYard only as a guest
[02:23] when we use it to stream what's new in Prisma every three weeks, I'm in there as an admin
[02:28] and I can also move everything around, highlight comments and all that.
[02:32] And here I, for the first time I see what Prisma, what StreamYard looks like as a guest, that's fun.
[02:37] And Anthony. - Put that one up, there we go.
[02:41] Anthony says you're a StreamYard pro. - Some experience under my belt here.
[02:48] I'm hoping that later this week I'm gonna be starting to use OBS and ping instead.
[02:55] So we'll see, we'll see, I'm getting there. - Yeah, actually we thought about evaluating ping as well.
[03:04] Haven't started really looking into that but it's floating around in our team.
[03:08] And I think at some point we will also see if and maybe serves our requirements better than StreamYard.
[03:14] - I will say it is pretty cool and being able to do like chat overlays and things with OBS
[03:21] and then the easability of going, because I use it for D&D as well.
[03:26] I play D&D on Friday nights and the host has a ping account
[03:32] and it's really easy to get in kind of like StreamYard. So from that aspect, I like it.
[03:37] - Nice. All right, Jen, should we talk a little bit
[03:40] about what we have planned for the stream today? - Yes, I'm also not multitasking very well
[03:48] and making sure that I am putting that we are live on all the things.
[03:54] So people know to come hang out with us, but I try to have it like where I just have to hit enter.
[03:59] And then when I don't, it's this, it is me not being able to multitask.
[04:06] But this I think is the fun thing about streaming live is I don't have to fake it.
[04:14] I'm literally, this is who I am. So this is what everybody gets.
[04:18] And what up, homie? And thank you, Anthony and Ryan.
[04:24] I am working on it. I have like three new lights and lights behind me now.
[04:29] We're gonna, I'm gonna figure it out eventually. It's gonna happen, but yes.
[04:36] Please talk to us about Prisma. - Yeah, so for the stream today,
[04:42] I think on a high level, we'll do two things. So first of all, I went to,
[04:47] I want to give you a thorough introduction to Prisma so that you really understand like what it is,
[04:54] why it's useful, how it fits into the stack and familiarize yourself with the three main
[05:00] Prisma workflows, that's data modeling, that's migrations and that's querying.
[05:04] And we'll talk about all of these in more detail. So again, we'll build up the context slowly
[05:09] for all of that. And then I think in the second part,
[05:12] once we've gained that basic understanding, we can move on and look at the 3D tech app
[05:20] and figure out together if we can make it work. I am also not a Next.js expert.
[05:25] I'm not a front-end developer expert, front-end development expert in general.
[05:30] My background actually is in mobile development. That's what I did before I joined Graphcool
[05:36] or like Prisma, how we are now called. So the last six years,
[05:40] I was able to transition into the JavaScript ecosystem, which by the way,
[05:45] compared to at least the Apple developer ecosystem with iOS, like JavaScript and Node.js is just a hot mess
[05:52] with all the different options and versions and browsers and libraries.
[05:57] That's a lot like more work. You have a lot more paved paths
[06:03] inside of the Apple developer ecosystem. - We have talked about, just so that way you know too,
[06:10] we've talked a little bit about Android development and with Zachary Powell
[06:17] and what we might do someday, might, might, is once I get TweetyTag to work
[06:24] is we actually make it into an Android app and work with him on how to make it into an Android app
[06:30] to do that. - Nice. Very cool. - So it's ever evolving,
[06:33] but yes, where would you like to start? - Let's start on the Prisma landing page
[06:42] and maybe you can already go ahead and share your screen. I was quickly thinking whether I should do that,
[06:46] but I think maybe since I'll walk you also through the main Prisma workflows,
[06:53] we can just start by sharing your screen. And- - I like how it's just like,
[06:59] if I type Prisma, it just knows to go to connect your database, where I was at the entire time.
[07:06] So let me make sure I go to the homepage. - Yeah, it's just prisma.io, exactly.
[07:11] And if you scroll down, there is one section that I want to highlight here to get started.
[07:16] And that's how does Prisma fit in your stack? That's where I want to start.
[07:20] A little bit further down, a little bit further down, this is Prisma Client.
[07:24] I think there's Prisma Studio and Prisma Migrate. Yes, a bit further down.
[07:30] - Oh, there we go. - How does Prisma fit in your stack?
[07:34] So Jen, have you seen such an architecture diagram already with a client and a server and database?
[07:41] - Not specifically this way. The way I've seen it has been more of in a GoDaddy context
[07:53] of when I worked in hosting there, where we would work with my SQL
[08:00] and we would have to help people with their hosting servers. And so not exactly, but kind of.
[08:09] - All right, all right. So let me untangle this then a little bit
[08:14] and explain the context for why I want to start with this diagram to explain what Prisma is
[08:19] and like where it fits into one stack. So these three components here
[08:25] are typically also called the three-tier architecture. And that's like pretty much the standard way
[08:31] how to build web applications these days. Three-tier because we have these three main components.
[08:36] We have the client, we have the server and the database. And the terms for this are somewhat ambiguous sometimes.
[08:44] So a client sometimes is also called the front-end. You could call the server and the database
[08:49] together the back-end. Sometimes people call only the server the back-end.
[08:54] Sometimes they call the server the API. So the terminology is a little bit ambiguous,
[08:58] but these three components, I think in general, are just like very good as a mental model
[09:04] for how to think about a web application. And if we start at the front-end,
[09:09] you, I think in previous streams, for example, have built React applications, right?
[09:13] And you also just talked about a mobile application. So on the front-end, that's exactly the kinds
[09:21] of applications that are being built there. It's mobile applications and it's web applications
[09:26] that are running in the browser that might be built with React, with Angular, with Vue, with Svelte.
[09:32] All of these like UI, JavaScript frameworks, they give you a way how to build JavaScript applications
[09:42] that are running on the front-end on the client. The main purpose of these client applications
[09:49] is to render a user interface to the users so that they can interact with the application.
[09:56] So it's usually very heavy in terms of building user interactions,
[10:02] building a user interface, building views. And then because views just by themselves
[10:08] would be pretty useless, most of the time, these applications also need some data, right?
[10:13] Inside of the application, if we are talking about an application like Twitter,
[10:18] then if I'm on the feed, I need to fetch the data that is the input for my feed.
[10:25] Or if I click on somebody's profile, I need to render the information for that particular person.
[10:31] If we didn't have this aspect of the data that we're pulling into the front-end, into the client,
[10:37] then we would really only have like a skeleton of our view without anything to really look at.
[10:43] So that's the client and it needs data. Where does it get the data from?
[10:48] Well, if we look at the right side of this diagram, we see the database and that's where the data
[10:55] is being stored, where it's persisted, where it's going to just stay over time.
[11:00] And yeah, it's just, that's the place where the data lives, where it exists in the physical world, so to say.
[11:07] But these client applications, so you could now say that, okay, that's convenient.
[11:14] I already know how to build kind of like a client application with views, but I need data.
[11:19] So I have my database on the other side. So why doesn't my front-end just fetch the data
[11:26] from the database directly? And that's actually a really valid question,
[11:31] I think that a lot of people might ask. Have you had this question yourself in the past
[11:37] or do you have any thoughts about this? - Again, I'm horrible at multitasking
[11:42] and I feel like I'm really, really happy that Ramon and Anthony are here today.
[11:47] Because if I remember correctly, Ramon and I, and I was looking for the link
[11:56] because I'm pretty sure it was this. Yes, Ramon and I built an Express API.
[12:03] - Yeah, yeah. - And I think that's like literally the most like direct way
[12:13] that I've ever done it. Like I might've done some of it when I did the...
[12:19] Yes, we did, Ramon, we connected it with Mongo. - Okay, yes.
[12:29] - So I was like, I'm pretty sure I've done this kind of a very long time ago.
[12:35] It was a long time ago now, but. - All right, but yeah, that's the client and the database.
[12:41] So why do we need this server in the middle, this like middleman?
[12:45] There are multiple reasons to that. Maybe if you were to redesign the web from the ground up,
[12:53] maybe you would come up with a way how the client could interact with the database directly.
[12:57] But the way how the web is built today and the infrastructure it runs on,
[13:03] it just makes sense to put the server in between for several reasons.
[13:08] One reason is that most databases, if we're talking about the most mature and popular ones,
[13:14] like Postgres, like MySQL, like MongoDB, they don't work with the like most popular protocol
[13:22] that we're using on the web and that's HTTP. You connect to them with another protocol
[13:28] that's on a lower level, TCP. And that's just one incompatibility of why a client
[13:33] who typically sends HTTP requests can't really talk to a database directly
[13:38] because the database only understands TCP. So that's one reason the client wants to talk HTTP,
[13:44] but the database only accepts TCP. So the client cannot directly talk to the database.
[13:52] That's one reason why we put the server in between. Another reason is that we need some business logic
[13:57] for our app. And with business logic,
[14:00] I mean such features already as user authentication. If we want to be able to provide a way for a user
[14:07] to log into our application with a username, with an email and a password,
[14:12] that's something that we cannot implement in the database because we actually need to write code.
[14:17] We need to do more than just store data inside of a data store.
[14:21] We actually have to implement some code, some logic, and that's not possible in the database.
[14:27] Maybe there would be ways, things like store procedures, but I don't even want to get into that
[14:31] because it's just not the way how we want to build modern applications.
[14:34] So yeah, the business logic, things like authentication, or if you need to implement a payment process,
[14:43] or if you need to communicate with external services, all of these things, they count as business logic
[14:48] and you would implement them on the server side. So now we have an understanding of these three components.
[14:56] We have an understanding of the client. That's where we have the UI, JavaScript frameworks.
[15:01] Then we have the database, Postgres, MySQL, Mongo to store the data and in the middle, this middleman,
[15:08] the API server that somehow mediates between the two. Yeah.
[15:16] - Okay, first off, like I think that's a first time and y'all, especially with Ramon and Anthony here,
[15:24] I feel like I need to say this caveat. Y'all might've told me this, but it didn't click.
[15:29] At least now it kind of makes sense of why it needs to be the server in the middle
[15:34] and why my front end couldn't connect to the backend of the translation of the two protocols.
[15:41] I will say, I'm just putting this out in the world. If anybody knows someone that wants to come on the show
[15:48] and just talk protocols, and teach us about all of the protocols
[15:52] 'cause there's so many out there and what we all use them for,
[15:55] please send them my way. But thank you, Nicholas,
[15:58] for at least this is making sense right now. - That's great.
[16:03] Yeah, so let's zoom a little bit into the API server and the different kinds of things
[16:10] that it's typically also responsible for. So like when you build a front end app,
[16:18] for example, with React, what kind of app did you actually build, Jen?
[16:21] And where did you get the data from back then? - Run that by me one more time.
[16:28] - When you built a React app here on the stream or like some other app where you built a front end,
[16:36] where did these get their data from? - For the React one,
[16:42] it was just like Googling build React app. And that was it.
[16:48] It just was the front end of it. - Oh, okay.
[16:51] - And then when I did the one with Ramon on Express, I'm pretty sure we just put in data to query it
[17:02] and just that was it. It wasn't like, oh, actually on the Express one,
[17:10] we were putting in things people say to us that are nice. - Oh, okay.
[17:17] - If you have a bad day, let's make an API that will call goodness
[17:23] that people have sent you. - Okay, okay.
[17:26] And you stored that manually inside of the MongoDB database, which you were using then
[17:34] and then you were putting an API on top of that. - And please know this was stream number three.
[17:40] So we're talking about stream number two and three. And the only one I had before that is,
[17:45] do I know the difference between HTML, CSS and JavaScript? And back then, no, no, I did not.
[17:53] So this was all new to me at that point. But yes, we did definitely, if I remember correctly.
[18:00] And then this is a question from Homie of if they become proficient using Prisma,
[18:09] will they have to write very little SQL, if at all? - That's a really good question.
[18:17] And I think this is already a good statement as well. They indeed will have to write very little SQL
[18:23] because what Prisma does, it abstracts the SQL away. Usually when you are working as a backend developer,
[18:31] so the person implementing the server here. Again, your job is to mediate
[18:35] between the client and the database. So what that means is that the client
[18:40] will send you requests, typically HTTP requests via REST API, such as the one that you have built
[18:49] with ExpressGen or a GraphQL API. That's in principle, very similar to a REST API.
[18:55] It also delivers data. It also allows you to invoke operations on the backend,
[19:00] but it's just a little bit more developer friendly, I would say, if you work with a GraphQL API.
[19:05] But in principle, they have the same responsibilities and that's to deliver data to the client.
[19:10] So as a backend developer, as a server side developer, what I need to do is I need to somehow process
[19:17] incoming requests and I have to then write code that understands what exactly is being requested.
[19:28] It creates a corresponding database query, reads that data from the database,
[19:34] packages the data that I just received from the database as a response up in a structure
[19:39] that's expected by the client and send it back to the client.
[19:43] Maybe we take an example, just the example about the Twitter profile,
[19:50] which I've mentioned before. So assume that you're opening the Twitter application
[19:56] in your web browser and you're navigating to someone's profile.
[20:00] What then happens is that the Twitter app on the front end, it sends an HTTP request to the server.
[20:10] And in that HTTP request, it includes information about who is the user that you're requesting
[20:17] the profile from. - My messages aren't up,
[20:21] just so that way I can go through these at the same time. And we'll go look at your profile.
[20:26] - All right. Yeah, if you actually open the console here,
[20:32] that might be interesting to look at this and see the network requests that are being sent.
[20:41] If you click on the arrows there, so yeah, you're now in the console view.
[20:49] I meant the network request tab, sorry, inside of the developer tools there.
[20:53] Yeah, network. And let's see, I haven't tried this myself before.
[20:59] If you select the box for fetch/xhr first, because that will only show us the HTTP requests,
[21:08] it's on top. Yes, this.
[21:11] And now if you refresh the page, let's see if there is some kind of...
[21:20] Okay, this looks way too complicated. I don't really know how to parse this right now.
[21:25] But just in principle, what happens is that, and it's like vastly simplified the scenario
[21:31] I'm opening up here. Obviously, when you actually use twitter.com,
[21:36] it's much more complicated what's happening under the hood. But in principle, what happens is that the front end,
[21:42] it needs the data that you see here on my profile. It needs my name, it needs my Twitter handle,
[21:47] it needs my bio. And all of that, it requests from the server
[21:52] by sending this HTTP request to the Twitter API and includes probably my user ID or my user handle
[22:01] some way to uniquely identify me as a user. So then the backend developers at Twitter,
[22:08] they certainly have gone through that process. Oh, there you go.
[22:12] - Make it giant. - Yeah, the backend developers at Twitter,
[22:22] they have implemented logic to then receive such a request from the front end and extract my username
[22:31] or my user ID, my handle from that request and use that as a variable inside of a database query
[22:39] that there's then sending off to the database. The database responds with the data of my profile
[22:44] and the backend developer, again, writes code to package the data that they just received
[22:50] from the database, package it into the structure that's expected on the front end
[22:54] and then return it to the front end. So this kind of journey of the data
[22:58] traveling from the front end as a request to the server, then to the database and back through the server
[23:05] to the client, I think is like really important to understand kind of where Prisma fits into that.
[23:12] - And he got us an example while you were explaining too. - Yes, so here we are in the network tab again for this URL
[23:25] and there we specifically see what kind of HTTP request has been sent.
[23:31] So all of this, what you see there on the right side in the general and response header sections
[23:36] are part of the HTTP request that has been sent through your browser in this particular situation.
[23:44] - Nice, okay. Thank you, Anthony as well.
[23:50] - Yes, it's always so good to have people on the stream who think along and who don't let you down
[23:57] when you're stuck and you have to debug something. - Oh, it's been fun.
[24:04] We've gotten stuck on having to debug stuff in like so many different streams.
[24:09] It's a lot of fun. I feel encouraged that it's not just me.
[24:13] - All right, so that's how I wanted to start just with this kind of basic understanding
[24:21] of these three components and how the data flows in between them and where Prisma is relevant.
[24:28] Because as a front-end developer, if you're building a React app,
[24:32] and I'm not talking about Next.js at this moment or anything where you can also execute server-side code
[24:39] from a front-end framework, but just a React app or a Vue app,
[24:45] which is just an app that's running inside the browser. As a front-end developer who's building an app like this,
[24:52] you will not get in touch with Prisma directly because Prisma really only happens on the backend
[24:59] or is used on the backend because it needs to interact with a database.
[25:03] And this database interaction is implemented on the server side.
[25:08] So again, as a front-end developer, you're not interacting with Prisma directly,
[25:11] but you're always just like sending HTTP requests to some kind of API that will serve you the data
[25:18] that you need for your application. So if it's not for front-end developers, okay,
[25:24] it must be for backend developers. And that's indeed the case.
[25:27] As a backend developer, when I start building a new application
[25:30] and I have these three components and I'm the backend developer,
[25:34] I'm using a relational database like Postgres or MySQL. I have several kinds of choices
[25:40] for how I want to interact with this database in terms of abstraction level.
[25:45] The lowest level of abstraction would be to just send plain SQL strings
[25:50] that I can write inside of my JavaScript code. I just write a SQL string and I submit that to the database
[25:56] and I receive a response back. That's totally possible,
[26:00] but it has several flaws or drawbacks. So first you actually have to really know
[26:07] what you're doing in terms of using SQL because SQL I think is one of the oldest technologies
[26:14] that we're using these days that is still kind of state-of-the-art in the industry.
[26:18] SQL has been developed in the '60s or '70s and it has been around for that long.
[26:23] And we're still using it. It's still the default for building applications.
[26:30] So it's still a great technology, but it's also really powerful and really complex
[26:35] and makes it very easy to shoot yourself in the foot. So usually you want to use higher level abstractions
[26:42] that are more developer-friendly and let you reach your goals as a developer faster.
[26:48] Another problem just with the fact that we are writing SQL strings inside of our application
[26:56] means that a string is not type-checked at all. We don't get any syntax highlighting or auto-completion
[27:03] or for that matter, any red squiggly lines underneath when we're making a typo.
[27:09] So it's also very easy to accidentally introduce any typos or other kinds of mistakes
[27:17] inside of your SQL queries that might blow up the entire application.
[27:21] So really working on the lowest level of SQL, I think I've seen only very, very few teams
[27:28] who actually do this. And typically these are the teams that are staffed
[27:31] with very experienced SQL engineers. And I think that's also the only kind of situation
[27:37] where it's reasonable to choose that approach and not choose a higher level abstraction.
[27:44] - Got it. - Then the next level of abstraction
[27:48] is what we call SQL query builders. In the Node.js ecosystem,
[27:53] there is a popular one that's called knex.js. And that's basically just a way to compose a SQL string
[28:01] by calling functions. So a very standard SQL query
[28:07] that would just return all the records from a table that's called users,
[28:11] it's just select star from users. That's a pretty standard SQL string,
[28:16] SQL query that you could write. And if you're using a SQL query builder,
[28:21] then you don't write this as a string anymore, but you would call a function that's called select.
[28:27] And then as an argument to that function, you would pass the name of the table.
[28:32] So you would call dot select and then from users. And so it's already a little bit nicer
[28:39] because we're calling a function and then this actual string is composed
[28:43] for me under the hood. I don't have to type the string anymore inside of my code,
[28:47] but it's still very error prone. And it's also actually still requires
[28:52] quite a high level knowledge of SQL if you follow that approach.
[28:56] And now we're getting to the highest level of abstraction to so-called ORMs, object relational mappers.
[29:04] And when we're talking about object relational mappers, the reason why they're called like this
[29:09] is because they map the data structures between the relational database
[29:15] and the object oriented programming language that we're using.
[29:19] And the difference is that inside of our object oriented programming language,
[29:24] we may have objects that are nested. So nested structures inside of our application
[29:31] and inside of a database, you can't inside of a relational database at least,
[29:36] you cannot have nested structures. There you have a so-called flat or normalized data model
[29:43] where the data is organized in tables. And when you want to represent any kind of relations
[29:48] between your entities, between your data, then what you have to do is you have to reference the tables
[29:57] with each other with so-called foreign keys. Whereas again, in our object oriented programming language,
[30:02] when we want to represent related data, we just use nesting.
[30:06] We can just nest our objects deeply inside of each other. And that mapping that has to happen somewhere,
[30:13] and that's what's happening inside of the ORM. And that's the problem that Prisma solves.
[30:18] It makes it easier for primarily backend developers, but also to front-end developers,
[30:23] thanks to framework like Next.js where you can write server-side code as well.
[30:27] But primarily backend developers makes their lives easier by giving them a nicer abstraction
[30:32] to work with a database instead of using SQL. (phone ringing)
[30:40] - I'm letting it sink in. I'm letting it sink in.
[30:42] And Anthony, are you talking about TweetyTag? 'Cause he's seen it.
[30:52] There's a PR chillin' in there of how to probably fix it. And this is how he came on, Nicholas, joined the show,
[31:00] is he has seen TweetyTag and looked at all of this because, and I just wanna throw this out there,
[31:09] it was actually Laura who is on on Mondays. We mostly talk about Python
[31:17] and we were talking about how to get questions answered. And I did not realize that Prisma had a Slack channel.
[31:26] So I hit up Prisma and was like, "Y'all, I'm stuck, please help."
[31:33] And, yeah, so it was pretty good. - Yeah, we'll look at the TweetyTag in a little bit,
[31:42] but let's maybe first familiarize yourself with the main workflows of Prisma that I mentioned before.
[31:48] And again, we are now working on the backend side. And the goal of working on a backend
[31:55] usually is to build some kind of API that's exposed to a frontend later down the line
[32:00] so that the frontend developers can get the data that they need when they're actually building the product.
[32:06] All right, how about you hit the big Get Started button in the top right corner
[32:12] and we'll walk through the quick start together. And I will show you,
[32:19] or I will provide you a couple of more in-depth explanations here as we go along
[32:25] than is provided in the quick start. - Yay.
[32:28] - All right, you don't have... We can just use this guide here.
[32:36] You don't have to click on that link. There you go.
[32:40] This is the instructions to start with Prisma. So what we want to do now in this guide
[32:45] is we want to set up a local database. For that, we're going to use SQLite.
[32:51] Have you heard of SQLite before or do you know how it's different
[32:57] from traditional databases like Postgres or MySQL? - No.
[33:01] - All right, SQLite is a super simple and straightforward relational database
[33:08] that just stores all its data inside of a single file with a .db suffix.
[33:17] And the reason why that's super simple compared to other databases
[33:21] is that with other databases, Postgres or MySQL, you actually have to install a piece of software
[33:27] on your computer in order to interact with that database. So you first would have to install Postgres now
[33:35] or you're using Docker to spin up a Postgres instance, but you somehow need to get a database server running
[33:42] on your machine or on some kind of remote machine that you can then connect to.
[33:46] With SQLite, you can skip that step. And that's why we chose that for our quick start.
[33:53] It allows you to still persist data on the file system, but you don't need to have an extra piece of software
[33:58] running on your computer. And it just makes the entire process
[34:01] of getting to know Prisma a lot simpler as well. That's why we're using SQLite here.
[34:06] - I like Anthony's add-in for it too. It's like a regular SQL database, but way more doper.
[34:12] - Way more doper, I like that. (both laughing)
[34:16] - I like it, I like it. Okay, cool.
[34:20] So... - Yeah, let's get started with these first commands.
[34:24] Let's create your project directory here. Nice, yeah, if you just type that in,
[34:36] you created the directory and you navigated into it immediately.
[34:40] And the next step here is to initialize a node project. Have you seen this before, this npm init?
[34:47] - Yes, I believe I ended up doing this at some point while trying to figure this out last week.
[34:54] - All right, what the npm init is for, it basically just creates the package.json file
[35:01] that then lists all of your dependencies, right? The npm init, like, yeah, I don't think it does a lot more
[35:09] than just create the package.json file. And then in the second step here,
[35:13] we had npm install TypeScript, ts-node, and the types from nodes.
[35:17] So just a couple of more dependencies. Actually, these are all development dependencies
[35:22] that we don't need at runtime, that we only need at development time
[35:26] to get TypeScript to work here in this context. And what we ultimately want to do here
[35:32] is we want to write a TypeScript script. So a little program that's just running from top to bottom.
[35:38] So no complicated server or anything, just a script that's running from top to bottom,
[35:43] and that will then read and write data in our SQLite database that we're going to use as well.
[35:49] - Got it. - All right, next we need a ts-config file,
[35:55] and the touch-ts-config is the command for creating that. And at this point, you can actually already go maybe
[36:01] and open this directory inside of VS Code if that's possible. Oh, nice, you're using the code shortcut.
[36:11] I love this one. - Ta-da! - Perfect.
[36:14] So yes, the ts-config JSON is already there, and it's empty, so you can now go ahead
[36:22] and copy the boilerplate from the quick start. It's really nothing special in there,
[36:26] just some default TypeScript configuration. All right, and at this point,
[36:38] I think actually from this point, I will guide you a little bit further
[36:43] instead of using the quick start. So now we have just the basic TypeScript project set up,
[36:52] and as a next step, we want to set up Prisma and the database.
[36:59] And then in the last step, we'll write the TypeScript program,
[37:04] the TypeScript script that will read and write data into the database.
[37:09] - Okay. - So to set up Prisma, you can install Prisma as a development dependency as well.
[37:17] That's with the command npm install just Prisma, and then -D or --save-dev
[37:26] to store it as a development dependency. If you just do -D now with a space,
[37:35] it will put this into your development dependencies. Have you seen this before?
[37:41] Are you aware of the difference between a regular dependency
[37:44] and a development dependency? - I'm gonna go with no. - What, if no, it's fine?
[37:51] Okay. - I don't know the difference.
[37:53] - So then maybe quickly hit enter, and then I'll explain the difference between the two.
[37:58] And to understand the difference, I think it's best to look at the package file,
[38:04] package.json in your side nav on the left. If you select that and you scroll a little bit, yes,
[38:13] or just make it bigger, you see that you have these dev dependencies right there.
[38:18] And usually you have, so at the moment you have only the dev dependencies,
[38:22] but usually you also have regular dependencies. And in fact, we'll install one in just a second.
[38:26] The regular dependencies that you don't see here yet are the ones that are being packaged
[38:36] with your application when you deploy it. So for example, when you deploy your application to Verso,
[38:41] then it packages all the dependencies, the regular dependencies into your application bundle,
[38:47] because these dependencies are needed in order to make your application work.
[38:52] The development dependencies, on the other hand, they are not needed for the application at runtime.
[38:58] So they aren't bundled into that application bundle that you're uploading to Verso,
[39:03] because you only need them at development time. For example, TypeScript is not what is running
[39:12] inside of your web browser, right? It's only JavaScript.
[39:16] So TypeScript kind of gets removed from the application bundle when you deploy it.
[39:21] The same with Prisma here. The Prisma dependency is just the Prisma CLI.
[39:26] The Prisma CLI helps you with your workflows that you do during development,
[39:31] but it won't help you when you do, or it's not useful for the application at runtime.
[39:38] Once the application has been deployed, the Prisma CLI has no use anymore.
[39:44] It's only useful for the developer as they build their application.
[39:48] - Really quick, just because I, definitely this is how my brain works,
[39:55] even though sometimes it can be very annoying, of like going, okay, cool.
[40:01] So we have like the dev dependencies and there's four of them here.
[40:07] And then I'm looking at TweetyTag. So the one I get that we built it totally different,
[40:13] but it only has one dev dependency. - Well, now I think you're in the root folder of TweetyTag,
[40:22] if I remember the package structure correctly. If you go back or if you, yeah, if you go to the root
[40:31] and now you click on the next forms app, you'll find another package.json in there.
[40:36] And there you'll find a whole lot more dependencies. And these are all the dependencies for your React app,
[40:44] for your next step. And that's actually also just like the one issue I saw
[40:50] with your repo that you basically have two like separate projects in one repo at the moment.
[40:57] And I think that's our main task later to kind of merge them into a single one.
[41:02] - Got it. And Anthony, thank you.
[41:05] That also really does help. I'm a what?
[41:12] I don't even know. - Monorepo is I think like a new trend at the moment
[41:17] to structure all of your applications inside of a single repo.
[41:21] So you're kind of the natural born monorepoist because you put all of your apps into a single repo.
[41:29] - Oh. I'm gonna pretend that I totally get that, I don't.
[41:33] I was gonna say thank you for this one though. This is helpful to know when we deployed the React app
[41:42] that I built with Anthony, it was React was a dependency, not a dev dependency.
[41:48] So this is starting to make a little more sense. - Nice.
[41:52] All right, great. So now we have all the development dependencies set up
[41:58] and now we can invoke the Prisma CLI that you just installed. And what we want to do is we want to create
[42:06] a Prisma schema file that we're going to use to define our database schema.
[42:12] And the command that you can do this with is called NPX. You prefix it with NPX.
[42:19] Then Prisma, just like the dependency itself exactly. And then the init command and you can hit enter.
[42:28] That's enough already. And what this is going to do,
[42:34] it just creates a new directory on your file system that's called Prisma and it creates this .env file.
[42:40] That's everything that this command did. So have you seen .env files before
[42:46] or have you heard of the concept of environment variables? - All I know, and this is probably not enough about them
[42:54] is they are in git ignores because you don't want them uploaded.
[42:58] And that is where you put your API keys and such. And that's basically all I know about them.
[43:06] I don't know what it stands for or anything, but yeah. - No problem.
[43:10] In that case, I would even say that we removed that additional layer of indirection.
[43:15] You can delete this .env file here because for teaching purposes,
[43:21] I think it's easier to just do it without. You can just go ahead and delete this file.
[43:26] - I will say while I was building a Tweety tag, I was okay showing all of that
[43:33] because I was like, y'all, this is learning. I'm not keeping anything secret in here right now.
[43:38] I'll change it later on. It's fine.
[43:41] - Right. - So thank you.
[43:43] - Yeah, but the .env file is usually used to define your database URL.
[43:49] But in this case, I think we can do it directly inside of the Prisma schema.
[43:53] So if you look at this file, schema.prisma, it currently contains these two blocks, how we call them,
[44:00] a generator and a data source. The generator, really, you can ignore at this point.
[44:05] You don't really need to understand what it's used for at this point.
[44:08] It just should suffice to say that it's responsible to generate Prisma Client later on.
[44:14] And Prisma Client is what's responsible to the component that lets you interact with your database,
[44:21] read data from it and write data into it. More important here is the data source.
[44:27] And that's where you specify the connection to a database. And this connection consists of two things.
[44:33] One is the provider. That means the kind of database that you're using
[44:37] and the URL, that is where to find the database. With Postgres, the URL would have to point
[44:44] to a Postgres server. It's what I mentioned in the beginning
[44:48] that with Postgres, with MySQL, you always need to have a server running
[44:52] and then this URL would actually point to that server. In our case, since we want to use SQLite,
[44:58] you can first go ahead and adjust the provider from Postgres to SQLite.
[45:03] And you can do that also by using the auto-completion. If you stop now, and if you hit Control + Space
[45:09] on your keyboard, it shows you all the options that you can choose with this.
[45:17] And that, by the way, is one of the things that you should get used to
[45:20] when you're using Prisma, Control + Space, because auto-completion is really a thing
[45:25] that we're optimizing for you to get as much progress as possible inside of your editor.
[45:32] And really, if you're completely blocked or stuck, we want you to go into the Prisma documentation
[45:39] to figure out more specifics about what you want to achieve.
[45:43] - Very cool, thank you. - Next, we need to set the database URL.
[45:47] And for that, because we're just specifying the location on our file system,
[45:55] you can type the following. So first you can delete this entire ENV,
[46:00] including the ENV. You can delete everything there, yeah.
[46:06] And now open new double quotes. And inside of these quotes, you type file,
[46:12] colon, dot, slash, def, D-E-V, dot, D-B.
[46:21] D-B, like database, exactly, yes, yes. So what this means is that we want
[46:31] the SQLite database file to live on our file system in the current directory.
[46:37] That's what we specify with a dot slash. We say that this is in our current directory,
[46:42] so inside of the Prisma directory, actually, where the schema.prisma file is also located.
[46:47] And the name of our database, we want to be def.db. We could also call it hello.db.
[46:53] We could call it gen.db or users.db. But in this case, we just want to call it def.db
[47:01] as our name. - Awesome, and we do have a question in here.
[47:06] So Homie's asking, Prisma does a great job creating a layer between the dev and SQL.
[47:13] With that in mind, briefly, what are some of the reasons they should reach out for MySQL versus Postgres?
[47:21] See if I can talk. They have worked with Postgres so far
[47:27] and are becoming comfortable. Are there reasons that they should look
[47:31] at other SQL database types? - That's a really good question.
[47:36] It basically comes down to what database should I pick for my application?
[47:41] And there are a lot of different trade-offs. Although, I will say that for the majority of applications,
[47:47] it probably won't make a big difference whether you use Postgres or you use MySQL
[47:52] or even SQL Server. These have, if you look closer,
[47:58] all of these have different kinds of characteristics here and there, different kinds of trade-offs.
[48:04] Postgres, for example, has a rich extension system, a great way to work then with geolocation data
[48:11] via extensions, for example. So Postgres, from what I've heard, is a very solid choice.
[48:17] And if you already are familiar with Postgres and you don't have a very application-specific reason
[48:23] to switch to another database for maybe specific performance reasons
[48:27] or something like this, I think just using Postgres as kind of the default is totally fine.
[48:33] - Got it, thank you. - And we also have, by the way, in the Prisma Data Guide,
[48:41] which is a resource that we're maintaining with all kinds of information,
[48:45] just about databases in general, we do have an article
[48:53] that compares all the different database types. So I just dropped this in our internal chat here,
[48:59] in our private chat in StreamYard Gen, and you can share this maybe in the public chat
[49:05] so that others can find it. - Just to show what it looks like real quick.
[49:10] And here we go. Oh, this is great.
[49:18] I definitely will want to look at this as well. - Yes, it's a very kind of thorough introduction
[49:24] to the topic of databases in general. And it's not Prisma-specific.
[49:28] The entire Prisma Data Guide, it carries our name, but it's really a very generic resource
[49:36] that doesn't talk about Prisma specifically, but just teaching database concepts.
[49:42] - I like what Anthony said of, for example, I used MySQL because I had a personal score to settle,
[49:49] which it is, it's just because that's what GoDaddy used. And I would have to like talk about it.
[49:54] And I still, to this day, I'm like, I just want to understand databases
[49:58] because I'm like, why, like with WordPress and so much of it of, I've been tech adjacent for so long,
[50:05] now that I'm learning, I'm like, I'm just going to figure them out.
[50:07] It's going to be great. - All right, then we have the Prisma schema in place.
[50:17] We defined our database connection. So the next thing that you'll have to do
[50:23] is you'll need to write a model. And the models is what we use to define
[50:30] the structure of our database. So usually when you're working with SQL database,
[50:35] you now would have to write some SQL code to even create tables inside of the database.
[50:41] And so that you can then later store data inside of the tables.
[50:46] So you first need tables, and then you can fill these tables with records.
[50:51] In our SQLite database, we have nothing. In fact, we don't even have the SQLite database file yet.
[50:56] We don't see the dev.db file inside of the Prisma directory yet, right?
[51:02] So we, ah, you don't have to create it manually. I see that, I think you wanted to do that,
[51:09] but actually Prisma will create that file for you when you run your first migration.
[51:14] So that would be the workflow if you didn't use Prisma, you actually indeed now would have to manually create
[51:22] the dev.db file. And then you would have to find some way
[51:26] to send the instructions to the database to create some tables so that you can then store data.
[51:31] With Prisma, you just define the structure of your database right here inside the Prisma schema.
[51:38] And then you can run the Prisma CLI commands to put the structures in the database in place
[51:44] to sync up the structure of your Prisma schema with the structure inside of the database.
[51:52] And yes, at this point I would say you can copy the two models here and just paste them in.
[51:58] - I will say, I want to give a shout out to Homie. Homie had to come on the stream with me for a little bit
[52:07] to start understanding these models 'cause it was not syncing in.
[52:13] And that's why I like got excited. I was like, I know they go in here
[52:16] and I know what they do a bit better now. So yes, thank you, Homie.
[52:20] And thank you for the graphic today. It was a great graphic.
[52:23] - Okay, so in the spirit of making this a little bit like educational, I'm just interested kind of in
[52:32] how would you describe the Prisma schema after my explanations, kind of in your own words,
[52:37] like what these models are for and what your current understanding now is
[52:42] of like where we are in the workflow in terms of the database and all that.
[52:47] - I would say just on what we've done so far, the ones that actually don't make as much sense,
[52:58] but I don't think I focused as much on is the package.json or tsconfig.json.
[53:05] Like those were new to me, or if I did them, I don't remember it.
[53:11] The explanation of the data source, that made a lot of sense to me.
[53:18] That's what I connected to Ivan. And it was cool to hear more about SQLite.
[53:26] I didn't know that was a thing, so yay. The generator client actually makes more sense now
[53:35] because of, oh, let's see if I can go back to it, because of this, because I'm like,
[53:41] oh, that's the generator client, at least in my head, is that it translated.
[53:46] So it's what the generator that translate between the two. So that made a lot more sense.
[53:52] And then the models are basically what is the information you want
[54:00] about something or someone. So for the TweetyTag app, it was like,
[54:07] I want to, and this is where I really, really appreciate Homie having me write it out,
[54:15] because I was not getting, it just wasn't clicking. And so by putting it in a Miro board,
[54:25] which sounds a little weird to do for a database, but I'm loading it up right now, I'm over here.
[54:36] It helped me understand, ah, go away, please, what I would want to have as models
[54:45] of a Twitter handle. I don't need more than a Twitter handle in one model.
[54:53] I don't want their first name. I just want their Twitter handle.
[54:56] And I would want, maybe the Twitter space may have the Twitter space link
[55:04] and the Twitter space name as one model. So it really helped like conceptualize it,
[55:10] putting it all on here. And look, Prisma's there, yay.
[55:16] - Very nice. - So it definitely, that's how I would explain it,
[55:20] because then once this was done, I could use index, wait, no, I'm skipping a step.
[55:28] Index, wait, no, I'm skipping a step. The part that I'm skipping to in just like memory
[55:41] is after all of this, when it calls it. So I don't remember all the stuff between it.
[55:49] That's cool. - All right, all right.
[55:51] But I think that was a great explanation, especially like with the models
[55:55] that the models represent the information that we need to store inside of the database
[56:00] to make the application work basically. But again, at this point inside of your editor,
[56:06] you only have defined these models, but we don't have a database yet.
[56:10] And we also don't have the tables yet. So that's what we'll do in the next step.
[56:14] We will run a Prisma command in the terminal to sync the Prisma schema with a database schema
[56:22] and make sure that the database has the same structure as we defined in the Prisma schema file.
[56:27] And the command that you can run for this is called npx. Again, that's the prefix.
[56:32] And then Prisma, and the next word is migrate. And the actual command now is called dev, D-E-V again.
[56:43] Npx Prisma migrate dev. So what this is going to do
[56:47] is going to read the Prisma schema and now asks for a name that you should give this.
[56:55] Ah, I think you didn't save the Prisma schema file and it complains that there are no models
[57:01] inside of it right now. If you save it and rerun the command,
[57:04] then it should ask you for a name for the migration. You can just call it init at this point
[57:09] because it's the first one that we're running. We're initializing the database.
[57:12] You can hit enter. And you see that some things have happened here.
[57:17] Actually, let's look at the terminal output and understand piece by piece what has happened.
[57:25] If you scroll up again to where you ran the command, there you go.
[57:28] - And as everyone will probably tell you that watch the stream a lot,
[57:31] I like to click things too fast. I get really excited and I hit enter or I click it.
[57:36] So that is- - Well, so far you had the perfect pace
[57:41] in terms of hitting enter. So, yeah.
[57:46] So first it loaded the Prisma schema from its location on the file system.
[57:51] It read the file system and then it understood, okay, there should be a SQLite database file called devdb.
[57:58] And then it created that file. So on the left-hand side of your side nav
[58:03] in the file system, you already see that there is one that's called dev.db now.
[58:08] And you can ignore the one with dash journal in the end. That's just like a helper SQLite file,
[58:16] but you can ignore that. So we have dev.db.
[58:20] That's our database. And at this point,
[58:23] we also already created two tables inside of the database because the command that you just executed,
[58:29] not only created the database files, but also the two tables that we had,
[58:35] that we defined inside of the Prisma schema. So if you now want to know what these tables look like
[58:43] or what the SQL code looks like that you would have to write when you don't use Prisma,
[58:49] you can indeed open up the migrations folder there. - Oh, not node.
[58:54] I don't want node. - And this one as well,
[58:58] that's the folder for the migration that you just created. It is named with a timestamp at first.
[59:05] So that's what all of these numbers are. And then you see underscore init.
[59:08] And init is just the name of the migration that you provided.
[59:11] And that's the SQL code that was auto-generated by Prisma. And that was already sent to the database as well.
[59:19] So inside of dev.db, you already have these tables now, but both of them are empty.
[59:24] You can actually validate that they are empty in a tool that's called Prisma Studio
[59:30] that comes with every Prisma project. It's a web UI to inspect the data inside of your database.
[59:37] And you can open that by running NPX Prisma Studio inside of your terminal.
[59:42] - Sorry, my dog just scared the bananas out of me. Just a second.
[59:50] Oy vey, that is, she does, she's a wild old lady. That is what my dog is.
[60:06] What was the command again? Sorry.
[60:09] - It's NPX Prisma Studio. - NPX.
[60:14] - NPX. - This will open a browser window.
[60:21] - Ooh. Whoa.
[60:25] Okay, I definitely wasn't doing this. - With your Prisma models.
[60:29] And you can select post end user. - Whoa.
[60:36] - Yeah, if you zoom out. If you hit command plus, I think it's,
[60:40] it's zooming in a bit more convenient way, yeah. Because it keeps the entire screen or UI at least.
[60:48] Yeah, so here you could already start creating records for users and posts now, if you wanted to.
[60:53] So you could click the add record button on top, but, or actually, yeah.
[61:00] Let's maybe add a user, not a post, because here you have to write, I think an author ID.
[61:06] If you just hit discard changes, yeah. And then you click on the plus on top
[61:13] and then you can select user. And now you're on the user table
[61:18] and then you can add a record and you can add, yeah. The ID, you don't have to add just an email.
[61:26] That's the only field that's required. You can add anything, you don't have to add.
[61:32] It won't validate like the structure of an email. And now you can, you can either enter a name
[61:39] or just hit save when change. - Yeah, yay, save.
[61:45] - All right, I think this, so that's the long outstanding UX bug in Prisma Studio
[61:51] that already got, I think Jason Langsdorf on our stream when I did the same with him one and a half years ago.
[61:58] In Prisma Studio, when you type something into a field, you have, and it's still selected
[62:03] and you click like save changes, then it actually won't change.
[62:07] You have to click outside of that field once. So yeah, you can add Jen again and click somewhere else.
[62:14] And now you can hit save one change and then it'll process. Yeah, that's, I've reported it back then.
[62:20] It still hasn't been picked up, but it's one of the things that you have to be aware of
[62:25] when getting started with Prisma Studio. Me too, Anthony, me too, Anthony.
[62:34] I don't, I don't understand what our product and engineering teams are doing all day.
[62:38] - Jason is actually gonna be on the show later this month and I'm pretty excited about that too.
[62:43] - Nice, all right, yeah, I had a huge, or just like a very, very fun time when I was on his stream.
[62:49] - Yay. - Cool. So now Jen, we have a database in place
[62:57] and we already stored one record inside of the user table. So now starts the fun part.
[63:03] And that's where we will read and write data in the database from the TypeScript program
[63:08] that we want to write from a TypeScript script. And that's by the way,
[63:13] the only reason why we needed the TS config file because we want to use TypeScript
[63:17] and we just set some specific configurations for using TypeScript,
[63:21] but otherwise you can ignore that file. All right, you can hit control C, I guess,
[63:28] to stop Prisma Studio inside of your terminal. Yeah, kill that process.
[63:34] And now we need a file that's called script TS and you can just, again, just execute a command
[63:39] that's called touch to create this file. And then script.ts will be the name of the file
[63:46] as the next word, yes, script.ts. Could also be called hello.ts or demo.ts,
[63:53] app.ts, index.ts, we just call it script here. And yeah, it should have been created on your file system.
[64:02] So in your file tree on the left, you should be able to find it.
[64:05] And if you open it, you'll see that it's empty. Yeah, so now you can quickly head back to the quick start
[64:14] and copy the boilerplate for that script. That's a little bit further down, a little bit,
[64:22] there you go, that's the boilerplate. So a TypeScript script is just a file
[64:33] that gets executed from top to bottom. And if you scroll up what this basically does at the moment,
[64:41] it imports Prisma Client, that's the component that we'll use to interact with the database
[64:47] to send queries to read and write data. The next line is const Prisma equals new Prisma Client.
[64:55] That's where we instantiate Prisma Client. That's where we actually like create the physical instance
[65:01] inside of our application that lets us do this, that lets us interact with the database.
[65:07] The next one is a main function. We need this because we want to,
[65:13] we want to use the await keyword. So we need an async function here where we can do this
[65:21] to resolve the promises of our database queries. And then in the end, we just call the main function
[65:28] so that it gets executed and have some additional boilerplate code
[65:32] that you also don't need to really worry about. - I'm not sure if this is just the way
[65:40] I was trying to do things or not, but when I was trying to do like a,
[65:45] like a read query and a write query separately, they wouldn't do them separately unless I had
[65:54] the index file, which we don't have an index file here. We have script.ts, but not sure.
[66:03] Like if I had the index file and I wanted to read it, I could, or if I wanted to write it, I could,
[66:10] but without the index file, the read and write wouldn't work.
[66:12] - Interesting. I think that's,
[66:15] like if it came down to what it was named, it probably was relevant in the context of the Next.js app
[66:25] or the framework that you were using, because these frameworks have conventions
[66:30] for how files should be named. In this case, we're not using a framework.
[66:34] We're just using plain TypeScript. So we can really name the file, whatever we want.
[66:40] It's not yet in the context of any framework. So we don't have to call it index.ts.
[66:43] We don't need to signal to the framework through the name of our file,
[66:47] what the purpose of the file is. - Got it.
[66:52] Thank you. - So yeah, you can already run this file, by the way,
[66:58] if you run, if you execute the command npm run dev. It's actually not the command, sorry.
[67:06] It's actually npx, because we're using plain ts-node here,
[67:11] and then npx ts-node. And now the name of the file, script.ts.
[67:20] So this just executes your TypeScript script from top to bottom,
[67:27] but there is nothing in there that we would see in the console at the moment,
[67:31] because we don't have any console lock statements. So it just executes all of these lines of code here
[67:37] that you see, importing Prisma, instantiating Prisma Client,
[67:41] executing an empty main function, but nothing really happens.
[67:44] So how about you just, like, for our own understanding, put a console lock statement,
[67:50] even before the definition of the main function? Yeah, and just, like, put one there,
[67:58] and you can just write something like hello, or we haven't executed the main function yet,
[68:04] or something like this. - I don't even remember how to do a console log.
[68:07] It's been so long. - That is console.log.
[68:12] - Okay, and then- - Now you open parentheses,
[68:15] and then you can put in a string. If you hit escape, escape should, yeah, hello.
[68:26] - That's what I put on all of them. Yay, okay.
[68:28] - Yes, so if you save it, and in the terminal, run the same command again,
[68:33] then it will print this, because we are just executing this script file
[68:41] from top to bottom. Okay? - Got it, okay.
[68:46] - All right, so now comes the interesting part, and that's where we are going to explore
[68:50] the Prisma Client querying API to send queries to the database.
[68:57] And when I use the term API here in the context of Prisma Client,
[69:03] it's important to distinguish it from, or to disambiguate it from the term API
[69:11] that we have talked about before already when we were talking about a web API
[69:16] that's consumed by a front-end. The term API is very ambiguous.
[69:21] It only means application programming interface, and that can literally be anything
[69:26] that allows you to interact with any kind of piece of software.
[69:30] And if we're talking about APIs in the context of web applications,
[69:36] we often call them web APIs, or HTTP APIs, or REST APIs, or GraphQL APIs.
[69:41] These are the ways how a client, a front-end mobile application, browser application,
[69:46] will fetch data from the server via the HTTP API. When I talk about the Prisma Client API,
[69:54] what I mean is the functions and methods that Prisma Client exposes to send queries to the database.
[70:00] So in this case, it's more of a database API that lets me talk to a database.
[70:05] But that's the term API when I use it as Prisma Client API. And the Prisma Client API,
[70:14] we're going to explore inside of the main function. And I would say that we're starting
[70:19] by trying to read the record from the user table that you just created inside of Prisma Studio.
[70:27] So you can delete this comment inside of the main function. And let's write our first Prisma Client query here.
[70:38] And we are storing the results of the query inside of a constant that we want to call users.
[70:44] So what you can write is const users. Const, that's, yeah.
[70:50] And then users equals. And now you can use the await keyword, await.
[71:00] And now you can type Prisma as the next word. And now you say dot.
[71:12] And again, here's the cool part about Prisma, the auto-completion.
[71:17] So now you don't have to type a lot anymore. You basically only have to know
[71:20] when you have to open braces and parentheses, but otherwise you can let yourself be guided
[71:28] through the experience of composing a Prisma Client query using the auto-completion.
[71:33] And in this case, we want to retrieve all of the users that are currently stored inside of the database.
[71:40] So you can go prisma.user. And if you put another dot,
[71:45] you will have another palette of suggestions. And in this case, we want to use the findMany query
[71:51] because that just fetches all of the users that are currently inside of the database.
[71:56] And maybe to just adhere to the TypeScript conventions, you can indent this line with one tab.
[72:03] So yes, perfect. And behind findMany,
[72:09] you also have to open and close parentheses because we're calling a function here,
[72:15] findMany is a function. And whenever we call a function,
[72:18] we have to use parentheses. All right, this line itself already is going to execute
[72:25] a database query against the SQLite database file that you have on your file system here, the devdb,
[72:32] and it will retrieve all the user records and store it inside of the variable called,
[72:38] inside of the constant called users. So if you execute this,
[72:42] you can do this, npxt is node, exactly. The output in the terminal still won't change
[72:49] because while this code is being executed, we don't do anything with the users
[72:55] to actually show them on the console. So what you can do next,
[72:59] you can insert a new console.log statement in the next line after const users,
[73:05] immediately after const users, not after the brace. Yeah, exactly in that line.
[73:11] And you can say console.log. And this time inside of the parentheses,
[73:16] you just put users. So again, and inside of parentheses.
[73:22] So after console.log, you have to open parentheses. - Oh yeah, yeah, yeah.
[73:29] Okay, let me just, stop highlighting it. - Yeah, these, that's indeed annoying about this code.
[73:37] All right, so if you execute this again, (mouse clicking)
[73:43] then you'll actually see the database entry now logged to the console.
[73:50] - Interesting. - All right, how about we quickly look
[73:55] at what Prisma is actually doing under the hood to just put some pieces together in your head, maybe?
[74:01] - Yeah. - If you scroll up in the file to line three,
[74:05] where we instantiate Prisma Client, and inside of the parentheses there,
[74:09] after new Prisma Client, the empty parentheses, if you put in curly braces there and hit Enter once,
[74:17] and now you hit Control + Space again, you'll see some options that you can use
[74:24] to configure Prisma Client. And in this case, we want to use the log option.
[74:30] So you can say log here. Now a colon, and then you can open square brackets.
[74:39] And inside of the square brackets, you can start or open quotes,
[74:42] double quotes or single quotes, doesn't matter. And there you see the different things
[74:47] that you can ask Prisma Client to log for you under the hood.
[74:51] And if you select query here, it will log the SQL queries that are being executed
[74:57] against the database under the hood by your Prisma Client instance.
[75:01] So yes, if you save the file and run it again, you now not only see the output in JSON format,
[75:13] but we actually see the Prisma Client, the SQL query that is generated
[75:18] based on the TypeScript query that you've created there. Select a user.
[75:24] So it specifies all the individual fields, the user.id field, the user.email field,
[75:30] the user.name field from the user table. And then it's just like some more cryptic stuff
[75:36] because this is auto-generated SQL code. So in a plain or more simple form,
[75:42] you could also write this query as SELECT * from users and it would have the same effect basically.
[75:48] It gives you all of the tables. - Interesting.
[75:53] Fokui, what does limit mean and where are the params in the query?
[76:07] - We are using, okay, this gets a little bit more into the weeds.
[76:12] I'll just give a couple of short hints here. The params for the SQL query are passed separately
[76:20] because we are using prepared statements with Prisma. Prepared statements are a concept in SQL
[76:26] where you can already define SQL snippets. You store them on the database server
[76:32] and then just pass the parameters like separately. That's why we don't see any parameters here.
[76:41] And also the limit and offset, these are keywords to specify pagination,
[76:46] which in this case we're also not using. And yeah, like the SQL query here
[76:52] could be like very much simplified, but because it's auto-generated,
[76:57] it looks a little bit more cryptic sometimes or includes information that's not always needed
[77:02] at this particular point. All right, how about we create another record
[77:10] in the database? And this time I would say that we're creating a post record
[77:15] and we are going to do this in code now, Jen, not in Prisma Studio, but in code.
[77:20] - Okay, okay. - So what you can do inside of the main function again,
[77:28] and I would say we do this even before, yeah, before the current line.
[77:35] So you can go ahead and write const. Again, we will store the result of this operation
[77:42] in a variable or inside of a constant. And let's just call it post.
[77:46] It's going to be a single post object equals await Prisma. This time we want to create a post, not a user.
[77:58] So you can select post here in the auto-completion. And if you hit dot again,
[78:05] this time we don't want to retrieve or read a post, but we want to create one.
[78:10] And there is a method or function that's called exactly that. Now you have to open parentheses again,
[78:16] because it's a function that we want to call. And inside of there, we now have to provide some arguments.
[78:21] So at this point, if I'm not mistaken, TypeScript will actually yell at you
[78:25] because you say, or like you're telling TypeScript that you want to create a post record in the database.
[78:35] But if you look back at the schema.prisma file, actually, if you quickly open that,
[78:39] it's a good opportunity to talk about some of the concepts in here and scroll to the post model.
[78:46] Like, how do you understand the different fields of that post model?
[78:56] Maybe you can explain to me what you can read and understand from these field definitions here.
[79:03] So how many fields first are there on this post model? - Would it be,
[79:13] I'm not sure if it would be five or six. I say that because the ID is like auto-created,
[79:22] but it's still something that's created. So it could be six, but the type, oh, go ahead.
[79:29] - We do have six fields indeed on this post model. The ID does count as a field.
[79:39] And so does the author field, which is of type user. That's a special field actually,
[79:45] because that's a relation field. It denotes a relation to another model.
[79:50] And all of the others are so-called scalar types or primitive types that are stored directly in the database.
[79:58] So we have six fields here indeed. And each field has a name, it has a type,
[80:05] and it has potentially some attributes. And it also potentially has a type modifier.
[80:11] Now what's a type modifier and what's it used for? Inside of the, or in the fields of the post model here,
[80:18] we only have one type modifier. And that's the question mark after the string
[80:23] on the content field indeed. Can you imagine what this question mark means semantically
[80:34] in the context of what we're doing? Or have any idea?
[80:38] It can be a wild guess. - This actually got me kind of stuck
[80:42] when I was trying to make the models myself was, I wasn't sure if like the title was something
[80:52] because the title has the string by itself. If then content has a string
[81:01] because they can't be the same type of string, they have to be two different strings
[81:05] to be read by the database. - That's, that goes into the right direction already.
[81:12] But I think this would rather be a unique attribute, how you could prevent two titles
[81:19] from being exactly the same or from preventing two posts to have exactly the same.
[81:25] Actually, if you scroll up to the user model, there is a unique attribute on the email field here.
[81:32] And that guarantees that the database will not allow that you ever create two users with the same email.
[81:43] So the database is going to prevent that if you are using the add unique attribute here.
[81:48] The type modifier, the question mark is slightly different. It is used to indicate to the database
[81:55] which columns need to have a value when you create a record.
[82:00] For example, when you created the user record, remember how you had to put in an email
[82:06] but you didn't have to put in a name. That's because inside of the Prisma schema here,
[82:11] the email is marked as required because it doesn't have the question mark at the end.
[82:16] When a field inside of the Prisma schema has no question mark in the end,
[82:21] it means it's required inside of the database. The database will ensure
[82:26] that whenever you create a new record, that there is a value
[82:31] for that particular column in that record. You can never have a database record in the user table
[82:37] that has no email because it's required. - Got it.
[82:40] - The name is optional. That's why we put the string here.
[82:43] The same with the post model. All of the properties,
[82:47] all of the fields on the post model are required except for the content.
[82:51] So when you create a new post, you don't have to submit information for the content
[82:59] but you have to submit values for everything else. Actually, that's not quite true
[83:04] because the published field as you see there right below content has the default attribute.
[83:10] So because the value in the database is still required but if you don't provide one yourself
[83:21] when creating a new post record, the database will provide it for you
[83:25] and we'll just set it to false as specified here. - Would it only do this as a Boolean
[83:30] or could it do like a string default? - It can also do a default string.
[83:35] It can do a default integer and default, yeah, for pretty much any other type
[83:41] except for relation fields. There you can specify a default.
[83:46] - Oh, this is fine. Okay.
[83:49] - Yes. All right.
[83:51] So if we go back into the script file now, so we have seen now that you at least need to provide
[83:58] a title and an author ID because these are the two fields on the post model
[84:03] that are required and that don't have a default value assigned to them.
[84:07] So it's understandable that TypeScript is now yelling at you and like showing these red squiggly lines
[84:16] because you're trying to create a new post record inside of the database,
[84:20] but you don't provide the content and the title. And before you spell out the title here,
[84:29] you should open curly braces again because you're passing the title and the author ID
[84:35] as an object here. So inside of this curly brace object,
[84:40] you can now hit control space and it'll show you what you can submit here.
[84:47] And again, the title and the author information are wrapped inside of this data object.
[84:53] So yes, you need to select data here and now colon and opening braces again,
[85:03] the curly ones, I'm sorry. Open curly braces and hit enter
[85:07] and now control space again. And now you can actually select the properties
[85:17] that you have to submit. So title, world or anything you like.
[85:23] - Because it would have to be within strings, right? Or no?
[85:26] - Yes, it has to be submitted as a string. That's correct.
[85:33] Nice. So TypeScript is still complaining.
[85:37] So first you have to add a comma after the title line, the end.
[85:42] And now in the next line, if you hit control space again.
[85:46] - Yeah, gonna do it that way. There we go, control space.
[85:51] - All right, you now have two different ways how you can connect an existing user record
[85:57] to this post that you're about to create. Either via the author field or the author ID field.
[86:05] If you do it via the author ID field, you have to know the ID of the user record
[86:10] that you want to connect it to. You can use this here actually
[86:14] because I know what the ID is. It's just one because you only created a single one
[86:18] and it's auto incrementing. So the only author, the only user record
[86:23] that you can even connect it to is the author with ID one. And you see the TypeScript error went away
[86:30] because now we specified a title and an author ID. So the only two required fields
[86:35] that didn't have a default value are now provided with values.
[86:41] So what you can do now is you can save the file and run the query and run the script again.
[86:51] And maybe we remove the log now because now it's just going to clutter
[87:01] the console log statements. So up in the Prisma Client Constructor,
[87:08] ah, yes, and the log option inside of Prisma Client. You can just like put a comment there as well.
[87:15] Yes. And if you save the file and run it again,
[87:19] we will only see the output of the user find many query because we aren't actually not logging anything else.
[87:30] If you hit command K in your terminal, by the way, you can clear it.
[87:35] And it's, and if you run the script a couple of more times, you'll see that it never will make a difference.
[87:42] We don't see anything, but with every time that you execute the script,
[87:48] the prisma.post.create query will be executed. And every time you're creating the same post record
[87:57] all over again in the database. Let's quickly validate this in Prisma Studio.
[88:02] If you run NPS Prisma Studio again, and you open the post table inside there.
[88:13] - Oh, cool. - You see that several of these posts have been created
[88:20] and they all belong to this one user that you created before.
[88:23] So if you go to the user table inside of Prisma Studio here and you click on post the four posts there,
[88:31] you actually can see the relation between the two. But so it's because the user with ID one.
[88:41] So if you close this relation view again, so the user has ID one, right?
[88:49] And in your code, when you specify the author ID for all the new posts that you're creating,
[88:56] you specified author ID one, right? And that's how you connected the two.
[89:02] - That makes sense. But if I wanted to,
[89:10] if I had a lot more in there and I just knew the title, could I query it without the title or without the number?
[89:22] If I didn't know anything else? - Of course, querying, yes.
[89:25] But here you're creating it, right? I think we can distinguish a create query
[89:31] from an update query, from a delete query, from a read, like find many query or find unique.
[89:35] And each of these will have different kinds of values that you have to put in first to tell Prisma
[89:40] what exactly you're looking for or what you want to do. And when you create, then of course you don't need,
[89:47] then you have to provide the value of the author that you want to connect it to.
[89:53] Or alternatively, actually we can go the alternative path. If you delete the author ID line there,
[90:00] just the author ID. - Author ID, yeah.
[90:06] - And instead we are now using author. So if you go in author colon braces, enter,
[90:15] colon curly braces, enter, colon braces empty. And control space for auto-completion.
[90:24] Connect, because we want to connect this new post record to an existing user record.
[90:30] Again, colon curly braces, enter. And again, control space.
[90:38] And now you can decide how do you want to connect it? Either by ID, that's what you already did.
[90:44] But here you can also choose the email because the email is specified as unique
[90:49] inside of the Prisma schema. So Prisma knows that there can only be one user
[90:54] with a particular email. And indeed, if you now choose the email
[91:01] that you've used before for this one user record, and you run the script again.
[91:06] You could also start Prisma Studio in a separate tab, by the way.
[91:14] Or now just, if you click on the plus inside of the local VS code.
[91:19] So now it has five posts. You see that it's still connected to this one user,
[91:25] this time by the email. If you type in, by the way, an email that doesn't exist,
[91:31] you can try that. Oh, yeah.
[91:38] So if you just have a type on there or an empty string or, yes.
[91:45] And you run npxt as node to run the script. - Oh, yeah.
[91:52] Okay. - You can still, yeah, leave this running
[91:57] and just hit the plus on top of the terminal there. And that open, yeah.
[92:03] No, further down, further down. - Oh, thank you. - The plus, the plus.
[92:07] You open a second terminal. - Okay.
[92:12] - And you can hit, yeah. Npxt as node, script.ts.
[92:20] - Is it dash ts node? - Dash ts node, yes.
[92:23] - Script. I feel like I typed this wrong, but.
[92:32] - I think it should work. So now. - Okay.
[92:38] - Did you save the script.ts file? - I thought so, but why are you not saving?
[92:47] Okay, save. - All right, can you run it again?
[92:51] - Ah, okay. - There you go. Now it runs into an error because no user record
[93:06] was found for the nested connect one to many. But like fundamentally the issue here is,
[93:14] I think if you scroll up, maybe you also have a bit more. No record was found or something.
[93:24] An operation failed because it depends on one or more records that were required, but not found, right?
[93:31] A post needs an author, but you provided invalid information for the author
[93:36] that you wanted to connect this new post to. So it didn't work.
[93:42] But we still don't see the, we still don't see the posts of the user record printed here
[93:51] and that's because Prisma by default, it only prints all the scalar fields of the models,
[93:59] of the objects that it sends queries for. So in this case, ID, email, and name are all scalar fields,
[94:05] but the post relation field is not included. However, you can include that.
[94:11] And we'll do that next inside of the Prisma client query, the find many query actually,
[94:15] that we have prisma.user.findmany. A bit further down.
[94:26] Yeah. A bit further up inside of the mainframe.
[94:28] - Oh, there we go. - Prisma.user.findmany. In there you can open curly braces.
[94:34] - Within find many or? - Yes. It's within the parentheses and control space.
[94:41] Now you have their include, and that allows you to include relation fields
[94:48] in the same query when you're reading data. So a colon, braces, enter.
[94:55] Control space. And this now shows you the options
[95:04] that you can include inside of the query result. And in this case, we want to include the posts.
[95:09] So you can click on posts and then it's colon and true. You can just write true here.
[95:14] It tells Prisma that you also want to include all of the posts of each user record
[95:22] that you're fetching from the database. So if you run this again, npxts-node script,
[95:28] the output will change and it will now include the posts key here,
[95:34] but it doesn't render the posts properly because that's how console.log works.
[95:38] What you can do is you can switch it to console.dir, D-I-R. - Oh, I'm down here.
[95:48] - And no, sorry, inside of your code where you currently have console.log users
[95:53] after the prisma.user.findmany query, but further down, but further down, yes.
[96:00] And you can switch that to console.dir, D-I-R. And then after users, inside of the parentheses,
[96:08] you put a comma, curly brace, and then curly braces. Yeah, and now you type depth, depth, colon,
[96:20] and then just the number zero. All right, if you save this and run it again,
[96:32] and yeah, maybe make a bit more space for the terminal. Now it just renders a single object.
[96:46] Actually, ah, sorry, ah, ah, sorry. Instead of zero, it's now, not zero, but actually now, yes.
[96:54] And now if you run it again, now you should see the nested object.
[97:01] So that's, by the way, what I initially referred to as nested objects.
[97:07] If you like make even more space for the terminal, if you scroll up, we have a lot of posts
[97:13] for this particular user already, but if you scroll up to the beginning
[97:18] of where you ran the query, you see that all of these posts are actually nested
[97:23] inside of a user object, right? On the root level inside of this object,
[97:28] you have the fields of the user. So again, if you scroll up a little bit to the user,
[97:34] the entire object starts with the scalar fields of the user, ID, email, and name.
[97:41] But then you also include inside of the same object, you're nesting more objects,
[97:46] and this time inside of an array. So posts has an array of more objects now.
[97:53] And that's what I refer to as nested objects in the beginning, because in the database,
[97:58] you recall that these are not stored physically together. They are stored in separate tables.
[98:04] And the only way how an application can now know which record is associated with which record
[98:12] in the other table is by following the reference from the foreign key, the author ID.
[98:17] But here inside of our JavaScript code, we now have them co-located,
[98:22] physically co-located inside of the same object. So that's kind of the different paradigm
[98:26] between relational databases and object-oriented programming language,
[98:31] where we can have nested data, whereas the flat and normalized tables
[98:35] always have references to each other. - What you're saying makes sense.
[98:40] I feel like I'm definitely going to need to mess with this more,
[98:43] and I cannot believe that it's already been over an hour and a half.
[98:47] - Oof, wow, okay, yeah, that is super fast. - So on that note, I am gonna save this
[98:53] and I'll get it uploaded to my creative repo for it, 'cause I feel like this is probably a good pausing point.
[99:02] And I absolutely love this because there are a lot of steps that I didn't do,
[99:09] and I don't know if it was on the walkthroughs or what, or I was just super enjoying it.
[99:17] Anthony says that Prisma is quite the rabbit hole. They've been tumbling down it for three years now.
[99:24] Of course you would send this my way, Anthony. Of course you would.
[99:28] I am totally sidetracking to see if I can find someone to raid to that look cool.
[99:38] So hopefully Coding Garden looks cool. It looks like they're doing cool things right now.
[99:43] And any questions that y'all have before we raid out? Y'all have before we raid out?
[99:52] Oh yes, yes, I agree with this. Now that I know what I was trying to do,
[100:01] yeah, like this would be way harder if I wasn't using Prisma, 100%, 100% agree with this,
[100:08] Anthony. - All right.
[100:11] - Anything that you think we should have been asking? - I think we went through all the main workflows.
[100:19] We looked at data modeling, we looked at the migrations, how you apply the data model to your database,
[100:24] and also at some queries. So yeah, the next step is for anybody
[100:28] to try it out themselves and integrate it in their applications.
[100:32] And yeah, if you like want to follow up about the PR or about your next JS app,
[100:37] if you have further questions there, the things don't work,
[100:40] then feel free to ping me again on Twitter, Jen. - Or we're all just gonna try to convince you
[100:45] to come on the show again sometime. - I can also do that.
[100:47] I will be very happy to do a follow-up now that we have the basics out of the way.
[100:54] - This was very, very cool. And thank you and agreed with everyone.
[101:00] This was great. Thank you for being on the show today.
[101:04] And I'm gonna get y'all rated. And thank you everyone for joining today
[101:12] and asking great questions. This was definitely, oh goodness,
[101:17] not the way I went about building my Prisma stuff. It is always good to have that.
[101:24] So thank you again and goodbye everyone. See you Thursday.

