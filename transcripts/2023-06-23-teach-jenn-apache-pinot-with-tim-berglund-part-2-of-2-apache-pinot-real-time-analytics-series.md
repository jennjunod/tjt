---
showLink: "https://www.youtube.com/watch?v=dw4pz2qSKS0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-apache-pinot-with-tim-berglund-part-2-of-2-apache-pinot-real-time-analytics-series"
title: "Teach Jenn Apache Pinot with Tim Berglund  Part 2 of 2 Apache Pinot, Real Time Analytics Series"
publishDate: "2023-06-23"
coverImage: "https://i.ytimg.com/vi/dw4pz2qSKS0/sddefault.jpg"
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

[00:00] Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:07] I'm Jen and today's guest, we have Tim and Tim, what are we learning about as of last week, this week, and who are you?
[00:17] Okay. Last week we talked about real-time analytics and we kind of just walked through a history
[00:23] of computing. That makes it sound a little grandiose, but like how we came to be in this world of real-time
[00:31] analytics and this week we're going to talk about a particular real-time analytics database called Apache Pino.
[00:39] And who am I? I'm some guy.
[00:41] I am the VP of developer relations at a company called StarTree. StarTree is founded by the creators of Apache Pino.
[00:52] It's a company that makes a fully managed cloud service based on Apache Pino. Very cool.
[00:58] And what is something cool that you, what did you do last weekend and what's coming up this coming weekend?
[01:06] Yes. My plans.
[01:08] Well, so last week, it was a big week, I turned 51. It was a lot of work, but I woke up and there I was, so yeah, it was a good birthday.
[01:20] And we talked about this last week. I have just moved to California, so it was my first, I suppose I'm a Californian now.
[01:28] And this weekend, I have some big plans on Saturday the 24th. I am marrying a woman currently named Rachel Stark.
[01:40] Later that day, she'll be named Rachel Berglund and I am very happy about that. Yay.
[01:48] And where are you guys going on your honeymoon? We are going to an all-inclusive resort in Playa del Carmen, Riviera Maya, Yucatan Peninsula
[01:56] of Mexico. Seven days.
[01:58] How did you find that? That's like a very, it sounds very specific.
[02:05] Yeah, it's, I mean, the Riviera Maya is not like a find. I mean, it's just that strip of Cozumel, Cancun, Cancun is on the land side, Cozumel is the
[02:20] island. It's, you know, people go there and there's a bunch of all-inclusive resorts there.
[02:24] However, we have an excellent travel agent who is a longtime friend of Rachel's who helped hook us up.
[02:32] Look, you know, kind of searched a bunch of places in the Caribbean and Mexico and we narrowed in on this place.
[02:37] Nice. Yay.
[02:39] Yeah. All right.
[02:41] So now I have to like see if I could recap last week, if I can remember what we talked about to lead up to the question I have.
[02:51] I'm looking at my notes. I'm going to try it.
[02:54] I don't think it's going to work. No, it's not going to work.
[02:56] So we're just not even going to try it. Sorry, y'all.
[02:58] You don't get to see my notes. I will fix it when I move.
[03:00] Okay. I know that moving pan, Jen.
[03:02] I am still here on my laptop webcam with AirPods in my ears. Decent lighting, but I just, it's not, it's disruptive to life and stressful.
[03:19] It is. Okay.
[03:21] So basically I'm going to start with analytics itself started with, and this is also a recap from another talk or something I saw from someone.
[03:40] So see if the two go together. Before even punch cards, it was also the like books themselves of just taking notes and
[03:55] like for bookies or accounting, would that be considered part of like analytics as well? Yeah.
[04:02] If you have a bunch of data just written in columns in a book, and if you wanted insight into the data, you know, all the particulars is a lot, there's just a lot of things.
[04:14] And it's, it's hard to understand list of numbers. You know, you want to know what to expect or what, what is an interesting thing that
[04:21] has happened that helps you make a prediction about what is going to happen in the future. And that involves you doing some kind of reducing of that set of notes.
[04:29] You can do that. If you just have pencil and paper and a list of numbers in a book, you don't even need
[04:34] a punch card or a mechanical tabulating device or anything. It's a lot harder and slower.
[04:41] Terrifying. Yeah.
[04:43] But an analytic in like, let's say an accounting notebook would be like, how many transactions did I have on Monday?
[04:55] And that tells, that number of how many transactions is getting an analysis of the data, which is an analytic.
[05:04] Yeah. Or what's my average selling price in March?
[05:08] Okay. Cool.
[05:10] Cool, cool, cool, cool, cool. And then, so for this next one, we went to punch cards.
[05:15] That's making sense. We moved on from there.
[05:18] And then we went from in the eighties is when we started seeing a lot more about databases. And we went from it being the mainframe to being on a single machine and people were
[05:43] using a LAN to get to the single machine. And then it was duplicating all of, you had one database with a lot of computers, but
[05:54] it would take forever. And then we updated to client server.
[06:03] That thing you just described is client server. So in between the original punch cards and client server, you just had mainframes and
[06:11] punch cards were a part of that story. But one big computer where everything happened, all the analytics, all the everything, and
[06:20] the client server transition was now there's lots of little computers on a network and the data is in a little database, smaller database, but there might be lots of those
[06:32] servers with databases on them. So during the mainframe era, it was all in one place.
[06:37] Got it. You could see it.
[06:39] And now, "Oh, what the crap? There's all these databases everywhere."
[06:41] That's the client server thing. It was an important economic innovation and architectural innovation and it was very successful,
[06:49] but it caused a problem in understanding, getting insights into what's going on. Got it.
[06:54] And that's why they would rewrite from all of the department's databases and basically batch once a day.
[07:02] Into the data warehouse. Data warehouse.
[07:07] Yes. Yes.
[07:09] That's how the data warehouse came to be. I wrote this down and now I'm going to read it out loud to see what it is.
[07:18] Analytics was a batch data process each night. Okay.
[07:22] That is accurate. And then in the early '90s, the web hit and we're still using the client service, which
[07:30] we just talked about, but now it's going to a website. So nothing really changed.
[07:37] All the processes is just like, now it's through a website. Yeah.
[07:41] Application architecture and the batch nature of analytics, completely unchanged. It looked like our whole world was changing and the web changed a lot.
[07:50] Just behind the curtains, not necessarily. And then in 2010, places like Hadoop and Data Lake and Spark decided that one computer shouldn't
[08:03] have all the data. So they started to have clusters that connected to each other?
[08:10] Yes. Because data got big.
[08:13] This was the so-called big data era and you couldn't fit it on one machine, the machines we could build.
[08:20] And so you had to build clusters and distribute it over lots, distribute the storage and the computation over lots of machines.
[08:27] But we still had a batch. So nothing really changed there.
[08:31] Again, the distributed thing was a big deal, but it's still not exactly freeing our minds yet.
[08:40] And so that's what people would refer to as the monolith, that it takes too long to load the data, which is why microservices and LinkedIn built Kafka for event-driven architecture.
[08:54] Yes. Let me nuance that a tiny bit.
[08:58] The monolith was just a client-server paradigm pushed to its limits and it didn't scale in a few important ways.
[09:13] It was a great idea in the '80s and '90s when it was taking over the world. And then we started to find in the 2010s, late 2000s, early 2010s, there were limits.
[09:25] So microservices, LinkedIn jumped on board, created Kafka. Got it.
[09:32] Got it. That makes sense.
[09:34] All right. And so that is a modern application program, and we went to event-driven and then events
[09:49] go to logs, which is part of what Kafka does, and mainframe to client-server to event-driven to real-time analytics was the entire process.
[10:04] Yes. And I'm stuck because I don't know what an event is to know what a log is, and that's
[10:12] where we landed. So let's talk about what events are.
[10:22] I'm going to back up a little bit and restate the summary of event-driven architecture. So the client-server paradigm grew to its limits and we discovered these big, giant
[10:34] apps. We didn't call them client-server anymore, but they were big, giant applications which
[10:38] is too hard to deal with. We started calling them this bad word, the monolith, broke them up into little pieces.
[10:44] And once you break a perfectly good program up into pieces, those pieces have to talk. And we experimented for a few years with various crappy ways of getting them to talk.
[10:54] And the way of making your microservices talk to each other that seems to be sticking is to have them throw events at one another and be event-driven things.
[11:08] So a microservices life is to sit there, this is a terrible simplification, but to sit there and wait for it to receive an event from a Kafka topic and, "Oh, look, I have work to
[11:19] do." And then it does that work and puts its results somewhere else.
[11:23] I feel like this is not going to be the best place, but I feel like eventually I need to figure out what workers are.
[11:30] And just the way you explained that made me think of workers in like words, not in what it actually does.
[11:40] Yes. So we might actually get there.
[11:48] We go through Pino. There's a thing called minions that are like workers and they're not...
[11:56] It's ambiguous. They're not the little yellow things that work for Gru.
[12:01] Gru is the boss, right? Is his name Gru?
[12:03] I don't remember. Yeah.
[12:06] All I know is when you told me about minions earlier, that's what I thought of. And I'm like, "That's probably not what you're researching."
[12:12] But it is what a normal person would think. So there you go.
[12:15] And yes, it's Gru. It's Gru.
[12:17] That's good to know. It's Gru.
[12:19] Okay. Voiced by Steve Carell.
[12:21] Thank you. So event.
[12:23] What's an event? Yeah.
[12:26] Okay. That's a great place to go before we get into Pino, because Pino's life is fairly tightly
[12:37] coupled to the idea of an event. So an event is, in the most abstract sense, a thing that happens.
[12:48] And you can really honestly start with just things in life. Like you clicked a button that started the broadcast today.
[13:03] And well, that's an event. You are in the process of moving.
[13:10] That moving is an event. There are lots of events in there.
[13:12] I'm getting married on Saturday. That's an event.
[13:16] I took a sip of water. So just things, right?
[13:21] And so events tend to be things that are localized in time, right? They happen at a time.
[13:33] And they're not things that, and this is a little bit metaphysical, but they're not things that take up space.
[13:39] So it's kind of an abstract thing. It happens in time.
[13:43] And it has some kind of information that goes along with it, which we'll get to in a minute. So my next question on that one is more of how large or small can an event be, yet in
[14:02] this context, I want to ask it as an example of, have you ever played D&D? Absolutely.
[14:11] Not a whole bunch, but I'm familiar. Cool.
[14:15] For those who may be watching, D&D is Dungeons and Dragons. It is a tabletop game where you basically role-play what your characters on a table
[14:26] are doing. I'm playing a version right now with my Discord group called, it's not D&D, it's called The
[14:34] Expanse, but it is also a tabletop game. And a remarkable television series.
[14:42] It is. On Amazon Prime and a series of novels.
[14:46] It is. Let's talk about Naomi Nagata's journey in season five.
[14:51] Don't tell me about it. I'm like, if I could put on earmuffs, I'm not there yet because I didn't start watching
[14:57] it until our campaign for D&D stopped. So they decided to do The Expanse and I was one of the only ones that hadn't watched it.
[15:07] So I'm learning about The Expanse at the same time. I can actually describe it without spoilers.
[15:13] I will say it is the most beautiful televised portrayal of abuse and trauma recovery that I've ever seen.
[15:21] Absolutely remarkable story arc in season five. If you know, you know.
[15:24] If you don't, DM me, message me, find me, I'll tell you what I mean if you've seen the season.
[15:29] Go on Jen, please. So-
[15:31] D&D. Yeah.
[15:33] Yeah. In tabletop games, you have to explain what you're going to go do.
[15:38] Like, if I'm going to, okay, this is a very weird way of thinking about it, but I'm going to use it, of the characters in the game got into a fight, somebody unalived, and I had
[15:55] to go get their terminal off of them to get data. But to say that I need to say, all right, now I'm going to go walk over to this person,
[16:09] look for the terminal, pick it up and do my thing. So is walking over there, would that be considered an event?
[16:19] Because that is so small, not something that people would necessarily think as an event because you would just be like, oh, I got to search for it.
[16:28] It's like searching for it is a very broad definition of something, where saying I'm going to walk over there is a very small part of it that goes into the big part.
[16:39] Yeah. Yeah.
[16:41] But within the rules of D&D, moving your character, deciding in a turn to move your character is one of the things that you can do.
[16:48] And that's absolutely an event. And if you were to think of a D&D game unfolding as a sequence of events, you could 100% model
[16:56] a D&D game as a sequence of events and your decisions with what you do with the character. And what do you play?
[17:05] What's the character you say? Her name's Luna.
[17:09] Okay. Since it's in the Expanse, she's Belter.
[17:12] Oh, sorry. It's not D&D.
[17:15] It's okay. So she's Belter.
[17:17] I know. Yeah.
[17:19] Yeah. Sorry, I got confused.
[17:21] Okay. So moving is a thing.
[17:23] And then, or if she has technical skills or something, in a turn, and I don't know the Expanse rules, but tabletop RPG, you're going to make a decision to do some other thing.
[17:32] And then, don't say DM, but whoever is running the story is also going to make decisions and actions on the part of NPCs.
[17:43] So there'll be non-player characters that are also producing events. But the whole game is a sequence of events.
[17:52] It's like a log of things that happen. And if you kept track, if there was some chronicler in the room that was just writing down every
[18:03] action everybody took in order and preserving the order of those things, that log could faithfully reproduce the state of the game and the history of the game as it unfolds.
[18:18] Your whole, however many nights, however long the campaign lasts, or whatever you call it in the Expanse, I need to play this game, you could represent that whole game as a sequence
[18:30] of events. And those are the things that you do and the things that the NPCs do.
[18:34] And that's kind of it, right? I feel like this is a very random way to describe it.
[18:41] It is. And this is good.
[18:43] I mean, this is a good lead into Pino, and it's so important. It's so important.
[18:47] But there's a few other things I want to say about events. Another way you might think about your game is the current state.
[18:55] And that's usually what you're trying to persist, because usually you get together or you do a Discord where there's a time when you synchronously get together with your fellow players, and
[19:06] you play the game. You block off time and do that together.
[19:11] And you move the story forward. And then at the end, you have some means of remembering where you are.
[19:16] So you kind of persist the current state of the world, the map, your characters, their character sheets, items they've picked up, things they've learned, damage they've taken,
[19:28] like whatever that state is, and what the protomolecule is doing or whatever. And you want a snapshot of that state.
[19:41] So next week you get together, you know where to pick up, right? So that snapshot of state-- and that's kind of how you do it with a weekly RPG.
[19:53] That snapshot of state is the thing you think about. The event log is usually not what you think about.
[19:59] These are two different ways of keeping track of what's going on. So you could just log every single thing that happens.
[20:05] And if you had that log, you could always play that log back to get to the current state. Or you could say, I'm not going to remember any of those actions or movements or decisions.
[20:18] I'm just going to remember the current state of the game. So that current state of the game is kind of like what you'd put in a database table.
[20:29] Or you could-- and you could literally do this with your Expanse. You could serialize it as JSON.
[20:34] You could make it YAML. You could come up with some format that serializes the current state of things and just decide
[20:40] not to remember how you got there. And honestly, that's how you do it as a normal person playing an RPG.
[20:49] But this whole thing with Kafka and event-driven architecture and all of these things that were kind of the end of our story last week and the beginning of our story this week,
[21:00] we find that when we're writing programs that need to talk to each other, like we do now with microservices architectures, that keeping a log of the events of how we got to where
[21:11] we are is an easier thing to do than keeping a snapshot of the current state of the system and sharing that snapshot.
[21:20] And there's a reason for that. And it has to do with the fundamental nature of events and the fundamental nature of state.
[21:27] Now, the current state of me is mutable. I change.
[21:37] I learn. I get tired.
[21:41] I rest. I become rested.
[21:43] I get hungry. I get full.
[21:46] I happen to have a shoulder injury right now. I think I have a rotator cuff injury, which is like typical middle-aged dude who exercises
[21:53] thing sucks, right? That's a mutation in my state, okay?
[22:02] And state is always mutable. The state of your Expanse game changes every time anybody does anything.
[22:06] When you have mutable state, when you try to share that with multiple people who are trying to mutate it, who are trying to make changes to it, that's really complicated.
[22:16] The rules of a desktop RPG game reflect this because you have, and I'll just say DM because I don't know what it's called in your case, but the person who runs the game, right, is
[22:25] kind of responsible for negotiating those changes. They ask, "Jen, what are you going to do next?"
[22:32] Okay, I am going to accept a write from you and let the state mutate. That's sort of like the lead node in this cluster.
[22:41] You get to suggest things and the DM gets to say, "Okay, that's going to happen," or "Wait, no, the rules don't allow that."
[22:49] If there's five people talking at once, they're going to say, "You know what? You four shut up.
[22:52] I'm talking to Jen right now. I can't take writes from all of you at the same time."
[22:56] That person is negotiating among all those clients trying to mutate the state at once. Doing that in software is notoriously difficult, okay?
[23:06] That's among the harder problems in distributed systems is ... I mean, some people say that's the fundamental problem in distributed systems is negotiating changing state with multiple
[23:18] actors interested in doing that. If I have a shared snapshot of what's true and 10 services are trying to change that,
[23:28] life sucks. State is mutable.
[23:31] Events are immutable. When a thing happens, it has happened.
[23:38] As I like to say in the heat of an argument, you say words that you don't mean and later you wish you hadn't said them, well, you have said them.
[23:47] You actually don't get to unsay them. You don't get to undo events.
[23:51] They have been written to an immutable log. All you can do is produce new events.
[23:57] Events are immutable, state is mutable, and it's easier to share things that can't change. Sharing an event log, you're sharing a record of immutable events.
[24:13] It's a lot easier to do that among all these services than it is to have everybody writing to the same row and a table at the same time and hoping that you can get that right.
[24:28] >> No, no, we really are talking about these in D&D terms because I needed a way to break it down.
[24:38] >> Seriously. There are so many great analogies.
[24:44] If you were a chess player, we can talk about a chess game as a sequence of events or the snapshot of the board.
[24:50] If you were a cook, we could talk about steps in a recipe versus the finished meal. There's state and there's events that lead to state.
[25:03] Those things work. Now, the problem is the state is often the interesting thing.
[25:12] You might not want to know what you had your character do an hour and 15 minutes into the game six weeks ago.
[25:23] It might be interesting if you just had that record, but maybe you don't care. When you're starting the game, you want to know where are we?
[25:30] What can I look at that says where everything -- it's the state that you want. State's hard to share.
[25:36] It's what you want. And that event log is the thing that's easy to share when it comes to computers.
[25:43] There are other advantages to having an event log. It's notoriously difficult and it would be a massive pain for you to start at the beginning
[25:52] of your chronicles of your game and read through every event and refresh your memory of where you are.
[26:00] That's ridiculous. You're never going to do that.
[26:03] You need to know what the state is. And if you want to ask other questions, like if there were an ESPN SportsCenter show on
[26:13] your Expanse game and you'd have analysts thinking, "Well, Jens Belter, 67% of the time when confronted with the Martian Navy fires first," how would you know that?
[26:31] You'd have to go through -- number one, you can't know that by looking at the state. You need the history.
[26:40] But it's hard to kind of manually go through that history. The history is literally just a sequence of events.
[26:47] All you can do is read through it in order. And so we need ways of materializing views of that to start playing the game.
[26:56] And if we want insight into what has happened, well, it's not quite time to pivot to Pino, but that's why Pino exists.
[27:06] I think I'm getting there. I'm going to go see if this analogy makes any sense as well.
[27:13] So if we're just talking about building a website and we have an error coming up, that error is a snapshot of what's currently going on, but won't show all of the changes that
[27:33] went into it to show it where logs would do that. I'm not saying it's exactly like events.
[27:43] I'm just trying to think of another way of comparing the two. Yes.
[27:51] That's a little muddled because the error is also really an event. Let me try this.
[27:56] Let me try this. We're both talking about relocating.
[27:59] I just moved and I still have a place in Colorado that I actually haven't closed on yet because it's new construction and renting a place here, but right now I want all my Amazon shipments
[28:12] to go to California. And so I go to amazon.com and I change my default shipping address.
[28:19] So that's an event. I made that edit.
[28:24] I'm mutating my customer profile to change my default address to be in Mountain View. The current state of my profile is kind of the thing I want to see.
[28:40] I don't really want to see a history of the changes I've made. I want the state.
[28:43] What's my address? That makes sense.
[28:46] Okay. Yeah.
[28:48] Graham, you are absolutely right. Like from what I'm understanding.
[28:51] I'm not seeing the chat. I'm like, "Oh, look, here's the chat."
[28:56] From what I understand, I'm just trying to like put it into other contexts, contexts, to work on really having it make sense because like what you wrote, Graham, like it makes
[29:15] sense by itself, but when I try to compare it to something else to break down these like new terms or technologies, it doesn't always sink in unless I basically put a bunch of
[29:30] different situations around it to have it make sense. So that's why we were talking about D&D.
[29:37] And that's not a Gen thing. I mean, it is a Gen thing, but it is not nearly a Gen thing.
[29:43] That's everybody. That's true.
[29:45] So this stuff is not obvious the first time you encounter it at all. It takes a while to make it make sense to you and Graham, I 100% endorse your snapshot
[29:56] versus each move thing there. And-
[30:00] Also, Robert linked to a Martin Fowler article and basically you should always read Martin Fowler on things like this.
[30:06] So thank you, Robert. I'm excited to look it up and read it later.
[30:10] Yeah. This'll be good.
[30:12] Okay. Well, I feel like I now have a better understanding about events and logs and would it just, is
[30:20] it... Oh, go ahead.
[30:22] Well, there's one more less conceptual thing I want to say about events, but ask your question first.
[30:27] Is it called state or always called current state? If you were to be like talking about this topic, how would you say it?
[30:34] I would just say state. And state is kind of the abstract notion of like things in memory right now or what is
[30:42] currently true of the world or that kind of thing. So the events are the things that happen that lead up to the current state.
[30:54] Like this week I did a dumbbell press exercise and that event did a thing to my shoulder and now my current state is shoulder injury.
[31:08] But that usually state. Yeah.
[31:10] Okay. Thank you.
[31:12] Thank you. I just said current state.
[31:14] Now, a somewhat less abstract thing about events, there's sort of the philosophical notion of just things that happen and they're immutable and they're local all the time and
[31:25] not extended in space, blah, blah, blah. In somewhat more computer science terms, we want to think of them as notification plus
[31:39] state. So events have a when-ness to them, they happen at a time.
[31:49] And so an event, like in terms of an event-driven microservice is a notification, "Hey, wake up.
[31:56] There's a customer. There's work to do."
[32:00] And there's information, that event carries information. So it does itself have this little chunk of immutable state.
[32:07] It says, "What happened?" So there is that it happened, the notification, and then the what happened.
[32:16] And so typically like in Kafka, just to be very concrete about this, an event is modeled as a key and a value.
[32:24] And Kafka is not opinionated about the type of those things. I mean, they're internally, they're just bytes.
[32:30] So like maybe the key is a string and the value is also a string, but it's a blob of JSON or something like that, that represents the temperature and the location and the humidity
[32:42] at the time the smart thermostat pinged headquarters or whatever. There is event, pardon me.
[32:52] There's notification plus state in an event. Okay.
[32:57] Yeah. And to Graham, technically, I don't even know why it's injured.
[33:03] Like I know what I was doing, but it was nothing different than usual and just, you know, welcome to my fifties.
[33:12] So an event is notification plus state and state is what happened. That part.
[33:19] Cool. Making sense.
[33:21] Good. Notification is, I don't know why this is hard to conceptualize right now, but I get
[33:30] like a notification on your phone, but I'm not sure why it would be part of an event because wouldn't it just be like an event is just like a state taken as a piece of information
[33:48] multiple times. Yeah.
[33:51] And the ways that we manage them and the places that we put them and the software infrastructure, we kind of wrap around them provides a mechanism for causing code to run when the event happens.
[34:09] So I mean, like a notification on your phone, the fact that that thing happened in the abstract and it's, you know, you had 22 cents of Apple cash deposited today or whatever, it's a good
[34:22] happy notification. Right.
[34:24] That's just a fact and it's out there and there's a certain time when that's determination is made.
[34:30] Um, I don't have to know about it. It's still an event, but then there's a bunch of software that sends, uh, you know, packet
[34:41] to my phone, uh, UDP packet, the data datagram is my guest to my phone. And this thing happens and it wakes up and it puts a little thing on the display.
[34:51] So it does a thing to tell me that it happened. And similarly in say Kafka, um, events can be produced to a topic and maybe there's nobody
[35:03] consuming those events. You know, the tree is falling in the forest.
[35:06] There's no one around to hear it. There's still events.
[35:08] All right. Okay.
[35:10] So there can still be notifications even if nobody's seeing them. Well that's just it.
[35:15] There wouldn't really be a notification if they're just being put in a topic, they're just being stored and no one's going to know.
[35:23] Now if there's a consumer of that topic, if somebody's reading that topic and they're all signed up and connected and ready, when the next event happens, that consumer is going
[35:33] to go, Oh, I have work to do and code is going to run. So there's a mechanism for that code to wake up when the event lands.
[35:41] If nobody's subscribed to the topic, are they still considered events? Yes, yes.
[35:49] So Kafka has a point of view on the question. If a tree falls in the forest and no one is around to hear it, uh, did it still make a
[35:57] sound? Kafka's answer is yes.
[35:59] Kafka is not a radical, uh, empiricist with apologies to, I think his first name is George Barkley, spelled Berkeley.
[36:08] Anyway, um, it, it, so still an event, doesn't have to be consumed, still an event. And so the notifications are for when it's consumed, but it is still creating the notifications
[36:24] even though they're not going anywhere when someone's not consuming it. Yeah.
[36:29] I mean, it's, you're still creating the message in the log and an event has still happened and has been logged.
[36:35] Um, but if there are no subscribers to that topic, then, then the, the notifying part isn't happening, but it'll start happening as soon as there's a subscriber.
[36:47] I feel like this is actually starting to make sense. Nice.
[36:52] Very weird. And thank you for going on this very random journey with me.
[36:56] Um. I'm happy to do it.
[36:59] Uh, cram what? If a tree falls in a forest last week, events let you look back one week and hear the tree
[37:07] fall. It still happened.
[37:10] I like that. It still happens.
[37:12] You just get to know about it. Yeah.
[37:14] I like that. Okay, cool.
[37:16] Thank you. Because this was a big disconnect when we were finishing up last week.
[37:19] I didn't expect it to take this long, but I'm glad that we talked about it. This is important material.
[37:25] It, it, it is helpful because I've, I had Lucia on, um, from Confluent talk about Kafka and it, a lot of what you're saying is starting to make her stream from a while ago start
[37:40] to make more sense. Excellent.
[37:44] Still work through it. Cool.
[37:46] All right. Well, do you, are we at a point where we actually get to talk about what we meant to talk about
[37:52] today? Let's, let's do it.
[37:55] Let's do it. Um, Robert, let's assume we have a longer retention period than a week.
[38:02] Yes, that's the default, but, uh, this is, uh, this is sort of the, the, the epistemology of Kafka here.
[38:10] Um, okay. Uh, now, so we've pivoted to this world where we love events and increasingly the, the way
[38:18] we know things is that we have produced them to a Kafka topic for consumption by some other microservice in our, in our system.
[38:26] And so, um, there's this direction in the event driven world to make the system of record be those event logs and to make our software be things that respond in real time to those
[38:39] events. Right.
[38:41] Um, and we'll, we'll, we'll pick up Pino here. We were talking at the very beginning about how the transition from mainframe to client
[38:51] server created this crisis in the way we understand what has happened. The reporting used to be a feature of our mainframe software because all the data was
[39:01] in one place, but now the data is in 20 places. How do we have a complete picture?
[39:05] And so we had to create a whole new thing and that was data warehousing and that, that modern era of analytics.
[39:10] Well, now that we've gone from client server to event driven, instead of nice, polite databases with our system of record, we've got these logs of events, uh, and, and that's a sliding
[39:22] scale. Okay.
[39:24] Not everybody is obsessive about topics being their system of record for everything, but there's this, there's this tendency now, um, and, and that is breaking the way we've been
[39:32] doing analytics, um, because, um, you could then extract those topics and dump them into a, into a data lake, but that's not real time.
[39:45] Everything else we're doing is real time and, um, you, you can't very well query those logs like we talked about in the role playing case.
[39:54] You're not just going to read through all the, that's ridiculous, right? They need to be somewhere where you can ask questions.
[40:00] And that is why after creating Kafka, the folks at LinkedIn, a slightly different, but, but nearby team created Apache Pino.
[40:11] So Pino is fundamentally a database and I would like to spend, we have 45 minutes, right? I mean, up to you.
[40:20] I have more time than that, but yes. Okay.
[40:23] Let me, let me just look at how much time I have. I have, um, oh no, I have, uh, no.
[40:30] Okay. We have till, till 1245, like an hour.
[40:34] Okay, good. We'll see.
[40:36] We'll see what we do. Okay.
[40:38] Um, Pino is a database and Pino is a database designed to ingest event streams. We'll just say from Kafka, they don't have to be from Kafka.
[40:48] They could be from Kinesis or Pulsar, but you know, concepts here, uh, to ingest an event stream from Kafka and make those events queryable in a table, like a, like a regular
[41:02] database table. Uh, now before we get too far, uh, Pino can ingest other things.
[41:12] If you've got a data lake, you know, gigantic terabytes of, of Parquet files in Amazon S3, of course you can ingest those too.
[41:21] It's not limited to Kafka, but, um, let's just kind of keep going with this event discussion and say, how do I make those events queryable?
[41:29] That's what Pino is trying to do. Really quick.
[41:32] Event stream is the same as event log? Yes.
[41:36] Event stream is, is just, uh, almost more marketing-y way of saying event log or Kafka topic.
[41:43] Yeah. Cool.
[41:45] Um. And Kafka, Kafka topic is the same?
[41:48] So like- It's a log.
[41:50] It's not synonyms. The topic is the, the technical name.
[41:54] If you look at like Kafka API documentation, it's a, it's a topic. Um, but fundamentally in terms of its structure as a data structure, it's a log and event
[42:03] stream is just a dorky way of saying that. Um, really quick, whoo, now we're going to see, because Lerner just joined as well.
[42:13] And I think that's a great point to do a very quick recap. Hi Lerner, glad you came and dude, it's late there.
[42:20] So, okay. So far we have gone through me trying to understand what an event is, which an event is a thing
[42:30] that happens and it could be, uh, we started talking about D&D and the expanse of RPG tabletop games as a way to understand them, which I really appreciate.
[42:44] So I think Graham's way or, uh, like chess is a little easier for everyone to understand, but I wouldn't have gotten there at first.
[42:55] So every time you move your chess piece is an event. And if you want to take a snapshot of the board and come back later, like you're like,
[43:06] Hey, this chess match has taken two hours. I need to go eat.
[43:11] You take a snapshot of it and that is the state of it. And an event you want to come in logs.
[43:21] So you keep track of all the events that happen, but it would be really annoying to read every single move somebody made to see where they're at now.
[43:30] So that's why you have a state, but an event is created by what just happened. So the state, what just happened, and then it creates a notification, go, yo, this thing
[43:41] just happened. And if nobody is looking at the event, like if they're just going into a log, nobody's
[43:49] actually notified their notifications are being made, but nobody's hearing it. But if somebody is subscribed to the Kafka topic or the stream or the law event logs,
[44:03] they will receive these notifications from Kafka. Yes.
[44:10] And Kafka is designed because it's like, you got all this events stuff. Now what are we going to do with it?
[44:18] And so far, we just started going into that. It goes in to Pino.
[44:25] So that way people can make a table to query, because it is very difficult to query events. Yes, because it's difficult to query logs.
[44:39] And so if you want insight into what has happened, you want to understand what has happened. That's where Pino enters the chat.
[44:53] It's less about materializing the current state and more about creating insights into the things that have gone on.
[45:01] In the role playing game, what percentage of the time does your belter character decide to fire first when encountering the Martian Navy versus a rival belter clan versus the
[45:15] UN Navy? And thank you, Nick, for rating.
[45:22] Yay. Welcome, everyone.
[45:24] And I did just do a recap right before this, which is kind of funny. But we're talking about Apache Pino and Kafka.
[45:34] That is how Kafka goes into Apache Pino in the fact of events and event logs. We just went over all of that.
[45:43] But if you hear mention of anything from Dungeons and Dragons or The Expanse, that is how I was understanding events.
[45:53] So I play The Expanse, which is another tabletop game on Sundays. And that is why it really helped.
[46:01] And if you hear stuff about it, that is why. And all right.
[46:05] So... Lerner said it's a little bit confusing how a log file is converted to a queryable structure.
[46:10] Fair, because all I've done so far is say that it happens. I haven't said anything about how, so it is appropriate to be confused about that.
[46:19] And then Robert is... Events are also about creating loosely coupled systems.
[46:25] And they should have schemas. Oh, I feel like that is something that we should talk about at some point.
[46:30] Just to hear the way you would describe what's the difference between events or schemas, databases and tables.
[46:38] Just because I want to start asking people that, because I think it's kind of fun. Okay.
[46:44] So, that is true. I agree.
[46:51] And also, putting that in chat is, and Robert 100% knows this, is a little bit like lighting a fuse and stepping away.
[47:00] I don't know. Nobody disagrees that they should have schemas, Robert.
[47:04] That's not controversial. If you said...
[47:06] If you took a particular position on how they should be serialized, or how the schemas should be managed, or how schema change should be negotiated, that would 100% be a troll, which
[47:15] I invite you to do. But let's not talk about schema yet.
[47:20] I'm sure it'll come up in the next hour. So shall we pinot a little bit?
[47:29] I'm excited. Okay.
[47:31] Good. And it's not quite noon in Pacific time where I am.
[47:35] It's mountain time where you are. So you're, at least after lunch, technically, you know, no, it's not.
[47:42] For me, if I have alcohol at lunchtime, that just means I fall asleep at 2 p.m. That's not good during a work day.
[47:48] I don't know how that was ever modeled. It matters if I'm traveling.
[47:51] If I'm like, especially with my European counterparts, a lot of them drink at lunch and they're very active.
[48:01] Yes. Yes.
[48:03] You're walking everywhere. Right.
[48:05] Where in the States, you don't do that as much. No.
[48:07] No. There's parts of the world where it's completely normal.
[48:09] In the U.S. these days, I mean, you know, 50 years ago, I guess it was normal, but you drink at lunch now.
[48:14] People are like, are you okay? But no, there are maybe geographies where that's less of an issue.
[48:21] I should live there. Okay.
[48:23] All right. Graham.
[48:25] No. All right.
[48:27] Can I, yeah, when I say pinot, I mean noir. Sometimes in U.S. restaurants, this rarely happens, if you just say pinot, they expect
[48:40] you mean noir. Every once in a while, somebody will bring me a grigio, I'm like, did you just tell me
[48:47] to go screw myself? I think you did.
[48:49] Yeah. I, for some reason didn't realize that a pinot grigio, like I always heard it together that
[48:56] I always thought they were like one word where like pinot noir, I hear noir, those ones considered a pinot, just like by itself.
[49:06] And yeah. Now let's, let's talk about how to be a database, right?
[49:12] There's there's there's just a lot of decisions you have to make. And I want to kind of walk through this tree and sort of dissect things and walk through
[49:22] the path that pinot took to arrive at being a database based on its goals. It wanted to be a real time analytics database.
[49:29] So you start off with this decision tree that I'm suggesting here. You kind of want to decide up front what you're doing, right?
[49:41] Because like Kafka is is keeping track of things that happen. A database like Postgres is kind of keeping track of things.
[49:54] It's remembering things. It's best at state, right?
[49:59] It's the current state of things, right? But if your goal is to understand what has happened, not remember it, not just get the
[50:08] current state of the board, but to get insight into what has happened. That is what you're doing as an analytics database.
[50:16] And that is going to impact the way we store data. The the way we organize it on disk, the way we think about indexes, there's just all kinds
[50:29] of all kinds of things that are going to happen. So I'm just I'm just trying to think of the I know how I want to do this.
[50:39] I'm just pausing to think about the smartest, least confusing way. You're doing better than me.
[50:48] I'm getting distracted, really trying to get my iPad to work again. Well, I'm just giving you giving you a minute to think now.
[50:57] Imagine I am Pino and I'm ingesting messages from Kafka, these events from Kafka, right? My whole goal is to read in all these events and make them queryable.
[51:16] Now, the way that works is and I'm going to make this I'm going to make an oversimplification. So if you know how Pino works and it sounds like I'm leaving some things out, I absolutely
[51:30] am. I've got these events coming in from somewhere, from Kafka, from a file, I don't know, from
[51:36] somewhere. I'm going to write them into a thing that I'm going to store on disk called a segment.
[51:42] OK. Yep, I'm going to write them into a segment.
[51:48] And that segment, a bunch of those segments are going to make up a thing called a table. So if I'm reading data in, that data is going to go into a table, just like any database
[51:58] table you ever thought of. It's got rows and columns.
[52:01] Pino is a database that uses tables with rows and columns. It's super simple.
[52:08] And as I'm reading that data in, I'm going to create these things on locally attached storage called segments.
[52:17] Those are just chunks of the table. And the reason I want to break my table up into segments is because Pino is a distributed
[52:24] database. Just like that thing happened 15 years ago, almost with the big data revolution, where
[52:30] we decided to make all of our things distributed, Pino lives in that tradition. So an actual Pino database is this big cluster of lots of machines.
[52:41] So I have to break my tables up into lots of these, we'll just call them files, called segments.
[52:46] OK. Make sense?
[52:48] Yeah. OK.
[52:50] Enough. I want to back up a little bit, because I have a presentation where I do this in this
[52:59] order, and I'm just trying to remember what order is without looking at the slides. But fundamentally, I'm ingesting data, and I'm ingesting it into a table.
[53:09] So whether it's messages coming in from Kafka, stuff coming in from a file on disk, files out in S3, whatever, I'm bringing them in, and I'm putting them into a table.
[53:20] And that table has a schema, and that schema is just the column names and the types of the columns.
[53:27] OK. Good so far?
[53:30] Yes. OK.
[53:32] And the way we store that data, since we've decided to be a distributed database, we have to store it in little chunks, or big chunks, really, but these big chunks called segments.
[53:46] And now I'm going to get to decide to distribute those segments over lots of different servers that make up my Pino cluster.
[53:56] So my one table that I've got might be enormous, right? It might be petabytes of data.
[54:02] So I'm going to need lots and lots of machines to hold all that, and it's going to be broken up into these segments that are living over all these machines all over the cluster.
[54:11] I'll let you write that down, and I want you to ask questions, because I feel like I'm not being entirely clear yet.
[54:20] Like, OK. So the data in, I'm going to simplify it as well, because I'm not there yet.
[54:29] You take, I'm going to say, again, we've said it enough in the stream, if somebody comes at us, I'm going to have to tell them back off, because I'm learning, and I need to learn
[54:37] Kafka, too, so I'm going to stick with Kafka. So you get Kafka events, and so when you say messages, just for clarification, I know Kafka
[54:48] can do like text messages. I mean the same thing.
[54:54] I mean, event and message are similar. It's like reading Lord of the Rings.
[54:58] You're like, LSR? Who's LSR?
[55:00] Well, that's the same as Strider. Who's Strider?
[55:02] I'm sorry. I'm using...
[55:04] Cool. No problem.
[55:06] That's why I'm... So data in, we're just going to say data in, and then it goes into Pino, and it creates
[55:11] a table. I know I'm skipping some steps, but I'll build on it.
[55:15] No, no. This is good.
[55:17] It creates a table, which the schema itself, for the tables, just give it the column name and the data type that go into the table.
[55:28] Yes. That's what we mean by schema, those column names and data types.
[55:31] Yeah. Okay.
[55:33] Cool. But this table is just like so giant with the amount of data in it.
[55:38] Potentially. That we're getting so much stuff because for some reason, in my mind, I think it was confirmed
[55:46] at one point, but don't quote me on this. In my head, Vonage, because they do SMS messaging, uses Kafka.
[55:55] In my head, that's what they do on a very large scale. And I'm saying, I have no idea, but in my head, that's what they do.
[56:03] But they have so many messages, actual text messages everywhere. It's way too much to have in one area that they have to have different segments, which
[56:11] have all of the data all over the world in different areas because it's so much data. And that is what segments are, is when they have it in different data centers.
[56:28] You added a thing that I, it sounded like you had added. So Pino is still assuming that it lives in one data center.
[56:34] So it's not like parts of the cluster in one data center and parts in another. It's all of the nodes of the cluster are close to each other and have low latency between
[56:45] each other. But we could still have 100, 200, maybe just 10, maybe 20, whatever servers that are storing
[56:56] all of those segments. We're assuming that it's too much for one machine.
[57:02] Okay. And Lerner, I'm going to, you're asking perfect questions.
[57:11] We're going to get to those in just a few, so keep going. I think I'm picking up what you're putting down.
[57:18] Okay. All right.
[57:20] Shall I, can I go to Lerner's questions? Yeah, do it.
[57:22] And sorry guys, I tried to get my iPad working so you could actually see the notes I'm taking to like put a visual to this stuff, but it's not going to happen.
[57:31] After the move. All right.
[57:33] So Lerner says in simple words, it's just loading into some DB tables, but the schema format is pre-decided like relation model.
[57:40] Yes. So the actual creating of the table requires you to specify the schema and some other metadata.
[57:46] You actually do that with a JSON file. You know, uses SQL, but didn't bother with a bloated create table options, blah, blah,
[57:58] blah sort of thing. It's, it's a somewhat more manageable JSON format.
[58:01] So yes, you have to know the schema first. And of course you could change that over time.
[58:07] Schema always mutates, but yeah, that's pre-decided when you make the table. And next one.
[58:13] So we're batch loading messages, but over some small timeframe, no, I don't want to say that.
[58:20] Batches is a, is a very difficult word. Now, if you have static data, like your example, some CSV or massive pile of parquet files
[58:29] in S3 or something like that. Right.
[58:32] And you want to load that into a Pinot table. Well then yes, there's a worker that's going to ingest that file and spit out a segment
[58:44] when it's got enough. You know, say, well, here's 500 megabytes of stuff.
[58:48] I'm going to call that a segment. So that is in that sense, batched, I've got this static pile of batch data and I emit
[58:56] segments in, you know, say 500 megabyte pieces or something like that. So that would be batched over some small timeframe if it's streaming data.
[59:05] So if it's a so-called real time table ingesting data from Kafka, there is absolutely no batching. So when Pinot, and again, skipping ahead over a lot of stuff here, Pinot is a native Kafka
[59:17] consumer. So if you know Kafka, there's no Kafka connect going on here or anything.
[59:21] It is its own Kafka consumer. And when it consumes a message, when it has successfully consumed a message and the offset
[59:29] advances from the Kafka topic, that message is queryable. So it has been ingested into the table and will show up in the next result if the next
[59:40] result selects that record. So in a sense, batching, when you're reading batch data, when you're reading streaming
[59:49] data, there's no batching in any sense. And I'm just...
[59:56] And that was skipping way ahead. So we can come back to that if you want to get that question on the table there.
[60:03] Yay. Learner said, "Thank you for making it simple."
[60:06] I agree with that. The only thing that I was going to verify is because so many words are like the same
[60:12] word but different. When we're talking about streaming data, it is just the event stream or the Kafka topic
[60:19] or the log or the event log or a message. All the same thing.
[60:24] So event streaming as well. I'm literally writing these all down because they're all the same yet different.
[60:32] And especially with where I work with Ivan, it's like people use them so interchangeably that I'm always like, "I'm so lost."
[60:39] But if I start documenting them, maybe I'll get better at it. And it really is just as bad as Lord of the Rings where characters have five names and
[60:47] you just have to know. But other than that, I did follow along.
[60:53] I'm quite excited. Good questions, Learner.
[60:56] We're somehow ingesting data, whether it's a batch source or a streaming source, we're going to just not care for now, into this table, which has a defined schema and is broken
[61:07] up into segments and those segments live in... I've been saying the word "server."
[61:15] That's actually the name of a Pinot component. So a Pinot cluster is composed of servers, brokers, a controller, zookeeper, and minion
[61:23] workers, and the server, unfortunately, kind of means computer. But in the Pinot sense, it's the component of the cluster that holds the segments.
[61:38] So it's where the data lives. Okay, that part makes sense.
[61:45] Everything you said after that, no. Okay, we'll get there.
[61:50] Cool. So we're making a Pinot table, we're ingesting data, we're emitting segments.
[61:56] These segments live on this distributed cluster. Let's say our cluster has 10 servers.
[62:04] And so as we create segments, they will be allocated to balance among those 10 servers. Good so far?
[62:16] A server is a cluster of that. Is a component of a cluster.
[62:22] So there's one machine, visually, because these things are just abstractions in the cloud now, right?
[62:29] But visually, it helps me to think of an actual data center with actual, and this is a little bit old timey, but rack mount machines.
[62:37] Yeah, for bare metal. Yeah, make it super concrete.
[62:42] And think there are 10 of those one rack unit things with blinky lights, and they say Dell on the front, and they're labeled Pinot server.
[62:51] And that's where this data we're ingesting actually gets written to SSDs on those Pinot servers.
[62:58] Okay. Yeah.
[63:00] Yes, enough. Enough yes for me.
[63:02] Yes. And I'm going to take it, learn this other question, like a load balance NAS for a data
[63:11] center? Yes, except not the NA part.
[63:16] Because in open source Apache Pinot storage is locally attached. So if you have a segment that is active and can be queried, it is on an SSD on a server.
[63:30] It's not on a network attached device. It's right there, which gets us to the next thing that's going on, which is queries, right?
[63:38] Okay. It's nice to store that data, but what about when we query it, right?
[63:44] So queries get sent to those servers. We don't know how yet, but they land, and these are just regular old SQL queries.
[63:55] And that server has parts of the table, right? The table's broken up into all these segments.
[64:01] Maybe our table has a hundred segments, and 10 of those are going to be on this server. So whatever parts of that query have data that live in some of those 10 segments, this
[64:16] server that has those 10 segments can execute those parts of the query. It can deal with the rows, basically, of the table that it has.
[64:27] Because not every server in the cluster has every row of the table, since the rows are written to segments, and the segments live on different servers.
[64:41] Make sense? So you can or cannot query for all the segments?
[64:49] You definitely can, and we'll get to that. So we're still in the world of this one little server here, and somebody sends this poor
[64:56] little server a SQL query, and it says, "Well, I definitely have these rows. I'm just going to execute that on the little part of the table that I have, and come up
[65:09] with the result that I can come up with." That's what that server does.
[65:11] That's not a complete answer yet, so we need to add some things to the picture. So, kind of like alphabetical, when you old records, they only have A through D.
[65:24] I have A through D. I can give you A through D. Best I can do, A through D, like the pawn shop show.
[65:29] Best I can do, M through P. Sorry, that's all I got. Okay, cool.
[65:35] Yes. Yes.
[65:37] And so it'll do that, calculate that average, or whatever it is there, because remember, we're doing analytics queries, so there are going to be things like averages, and mins
[65:46] and maxes, and stuff. Okay, so how do you bring all that together?
[65:52] Now you've got these servers, which have these segments, and everything's all split up. Well, there's another component in the Pino cluster, and it's called a broker.
[66:04] Not to be confused with a Kafka broker. That is a different distributed system, so if anybody's thinking Kafka brokers, push
[66:14] that to the side. This is a component of a Pino cluster called a broker.
[66:22] Okay. Now when I am an application, and I have a query, I don't know anything about servers
[66:36] or segments. It's interesting for us to talk about, and thinking about how a system like this works,
[66:43] but I can't know that. There's data, and I have SQL, and I need a result, and I need it 50 milliseconds from
[66:52] now. So I'm going to send that to my Pino cluster, I don't know anything about servers or anything,
[66:59] which means a broker. So I'm going to send that query to a broker, that broker is going to look at the query,
[67:08] and it knows enough about my table to know, okay, I know you're going to need these 17 segments to answer that query.
[67:24] The broker is going to know where those segments are. I'm never going to know that as an application developer.
[67:34] So learner, yes, you know the address that you are posting your query to, is what you're doing.
[67:42] So assume we're using the REST interface here. I'm just posting a query to an address, that's a broker.
[67:49] That broker is going to know, oh, I need these 17 segments, they're on these three servers. So it's going to take that query and send them to those three servers.
[67:59] Those three servers are going to work on it at the same time, right? So it's not just about scaling storage, but we scale compute also.
[68:08] I've got three machines working on that query in parallel. And say we're calculating an average.
[68:15] Each one of those machines will calculate their average, send them back to the broker, the broker will gather those results together, basically, in this case, average the averages,
[68:28] and I have my answer. Okay, so all of that makes sense.
[68:42] Something I don't think I wrote down right is, a segment is a component of a server? A segment is a thing stored on a server.
[68:56] So the job of a server is to store table segments, and to do the compute involved in processing queries.
[69:07] So segments are kind of the real heroes of the cluster. They're the ones doing the work.
[69:13] They store the data, they get the query, they do the actual scanning, filtering, sorting, reducing.
[69:22] Brokers help do the scattering and the gathering. Brokers help say, "All right, this is the query.
[69:28] Which servers do I need to get involved? And when I get the results back, how do I unify those several results into one?"
[69:37] Okay. Yeah, yeah.
[69:42] And Lerna, the terminology is tough, because server, that's so ambiguous, right? But that's the words that we use in PNAP.
[69:50] Yeah, brokers kind of help orchestrate the servers. That's right.
[69:54] Yeah. And that makes sense.
[69:56] Like, what you were saying about the broker made sense to me, but the server, so a segment is a component of the server.
[70:07] No. Yeah.
[70:09] I would say a segment is a thing stored on a server. Stored on a server.
[70:14] Okay. And then what are the other parts of a server?
[70:19] The broker? No.
[70:21] A broker is a separate box. So if you're drawing the diagram, usually you draw a few server boxes along the bottom,
[70:31] right? And then up here, you'd have a few broker boxes, and the brokers are talking to the
[70:36] servers. Okay.
[70:38] I'm going to go back and re-watch that, because it's making sense, but it's not making sense, and I'm kind of stuck on it.
[70:46] But that's okay. That happens.
[70:48] I can send you a picture. Okay, cool.
[70:50] Is there a convenient way to, I don't have it online anymore, it'd be something I'd paste. I'll send you a picture later.
[70:57] Okay. And I'll clean up my notes so we can share them afterwards.
[71:01] And what up, Maddy? Hey, look, it's my boss.
[71:03] Hey. Hi, Matt.
[71:05] Can I, wait, can I share? I can share.
[71:07] Yeah. Yeah.
[71:09] Okay. Ever since I had my computer fixed two, three weeks ago, Alfred is just not indexing things
[71:28] properly, and that makes me upset. So.
[71:31] All right. [71:32]j Let me, real quick, like, present, share your screen, of course, if it's going to
[71:51] require me to quit, and I'm not going to do that. Sorry.
[71:56] Okay. Chrome.
[71:58] I had my computer serviced and all the permissions are reset and things, so I'd have to quit and come back in.
[72:06] So I don't, it would be too disruptive. I don't want to do it.
[72:08] Okay. Well.
[72:10] Alfred is a Mac application launcher and it's treating me very badly, so anyway. I'll send you a picture later.
[72:17] Okay. Thank you.
[72:19] Let's get out of the architecture. I mean, I think that's interesting and it's helpful to see how a distributed database
[72:25] is set up. There are some other really interesting decisions that a database has to make.
[72:31] If you, if you look at the, the things Pino had to do, okay, it had to ingest event data from Kafka, streaming data from Kafka.
[72:42] And the whole idea, like we talked about last week in real-time analytics is, is not that we're updating a dashboard every 15 minutes, but people are doing things in an application,
[72:59] tapping on controls, entering searches, you know, stuff like this, and they're expecting results synchronously and they don't wait very long.
[73:08] And so I need to be able to hit this database with potentially very large amounts of data and get a result in what I am calling quote unquote real-time.
[73:18] And real-time just means fast enough that I'll wait for it and not think the app is broken.
[73:24] That's, that's how I'm defining real-time. Okay.
[73:26] Okay. And I, I actually like that definition that we, it's, it's just mine, you know?
[73:34] But when we say, when I say real-time analytics, I mean, you can show it to a user and it doesn't look broken.
[73:41] So, you know, 10 seconds to spin up a Spark job and go get a query, get it, get a result and get it back.
[73:47] That's real-time. I'm not going to wait.
[73:49] You know, so maybe 50, a hundred milliseconds, something like that. And some people have more stringent requirements.
[73:56] There are some like, you know, 15, 20 millisecond P90 latencies that I've seen, which is insane, but it's fast.
[74:04] Right. And so being a database designed to work over all this amount, amount of data and run that
[74:09] fast and, and be an analytics database affects the way certain other decisions are made. And I think it's worth it to talk through a little bit of this in, in your own database
[74:21] journey, because it's been helpful for me in the last year to think through some of this stuff.
[74:25] So for example, if you're an analytics database, you are often interested in many things in a single query.
[74:42] So I probably let's, let's go with my smart thermostat example that I always like to go back to.
[74:48] Right. I've got 10 million smart thermostats of a certain type in the United States.
[74:52] They report back a temperature every minute. And I want to compute an average in, you know, between one and 2 PM in the eight zero zero
[75:02] zero two area code of all those sensors. Right.
[75:08] Okay. So there's a lot of them.
[75:11] There's a measurement every minute. There's a lot of sensors in, in Arvada, we'll assume I've got, you know, successful smart
[75:17] thermostat. And so I am scanning lots of those numbers.
[75:23] That query is interested in lots of numbers and I want to average them. Okay.
[75:30] That's an analytics query. A transactional query might be something like somebody just set up a new smart thermostat
[75:43] and I need to insert a row into a table of all my smart thermostats or somebody is running the app and is trying to remember what did I call the thermostat in the kitchen?
[75:55] And they want to look at the record for that app. So I need to go look up that, that, that one record.
[76:02] So on the transactional side of the world, and broadly the two categories of databases are transactional and analytic.
[76:08] On the transactional side of the world, I'm usually interested in this one thing. I'm creating a thing.
[76:14] I'm looking at a thing. I'm changing a thing.
[76:17] I'm deleting a thing. We talked about CRUD last week, create, read, update, delete of one thing.
[76:25] In analytics, I'm probably interested in all these things. Makes sense.
[76:29] And I want to scan lots of results and compute, say, an average of them or, you know, reduce that to a single number.
[76:37] Make sense so far? Yes.
[76:39] Yes. And I want to go through this point, see what questions you have, see where I want to go
[76:45] from here. This is my last kind of interesting little piece of database architecture.
[76:53] If you look inside a segment, right, if we had segments, we're creating segments as we're ingesting data constantly.
[77:00] Our assumption would be that I get an event from Kafka. Let me just, oh, look at this.
[77:07] I finally got it working. Sorry.
[77:10] I've been working really hard to, ah, I didn't hit the right button. Oh boy.
[77:14] That was me. I meant to click the hide, but we got it working.
[77:19] We got it working. Nice.
[77:21] Okay. What?
[77:23] So when you're ingesting data, your assumption might be, I'm just going to write that data. I've got that event and it's got fields and values and stuff.
[77:36] I'm just going to write that into my segment. And so I have a list of these events, right?
[77:42] Well, that's what you would do if you were a transactional database, you'd want to write your whole thing, your whole row in one place.
[77:52] Right. Interestingly, analytics databases generally don't do that.
[77:59] What you do when you're creating the segment, you say, well, I'm ingesting a hundred thousand of these things as I'm writing this segment.
[78:07] I want to write, okay, so let's go with our smart thermostat example. Temperature is one of my fields, right?
[78:17] For this segment, I want to write all of my temperature values together. So you may encounter this term column oriented storage or column oriented database or something
[78:29] like that. That is generally the storage architecture used by an analytics database.
[78:35] You actually break up each event, each entity, each thing, and write all the column values together.
[78:47] It's the craziest thing. It sounds very counterintuitive, but you batch up the columns together and write them together
[78:55] because what you're going to do is you're going to scan through all of the... At the end of the day, what a query is doing is scanning a bunch of column values.
[79:08] You want them all to be together. And that's what transactional does.
[79:12] No, this is... Transactional is you store the row in one piece.
[79:20] Analytics is you store all the columns together. Because in transactional, you almost always want the whole row at once because you're
[79:37] doing that crud over a single thing. So you store the whole row, the whole entity together.
[79:46] In analytics database, you store the columns together. This is what I was trying to do last time and for this because it gives a visual and
[80:07] it also makes sure that you're able to see that I wrote it down right, that I comprehended it right.
[80:14] Yeah, yeah, yeah. This is great.
[80:17] I love it. Sorry that it took so long to get it to work, but I figured it out.
[80:26] Okay. Last thing.
[80:28] Hey, Glassy is right. Yes, it is.
[80:30] It is all a table. These are just different ways of organizing the storage.
[80:35] And again, as a user, it's a schema. You write SQL, you get answers.
[80:41] What do you know? What do you care?
[80:43] Right? So to get the kind of performance to be a real-time analytics database, there are certain
[80:49] kinds of decisions that had to be made. Last thing I want to talk about is indexes.
[80:59] Okay. And you are probably comfortable with the idea that databases have indexes.
[81:08] You create indexes on columns. And the idea is, so we kind of talked about how to write data.
[81:15] We're ingesting data. We're putting it in these segments.
[81:17] We store it in this column-oriented way. And yeah, we read it, but we haven't really thought much about how that works.
[81:25] So part of what Pino is trying to do is to give you the flexibility that you're used to with a traditional relational database.
[81:36] And what we're used to there is when I've got a column that shows up in a query, I can create an index on that column and make that query perform well, for some value of well,
[81:51] right? And in a relational...
[81:53] I feel like I know what an index is, but at the moment, it's totally spacing me. Let's do it.
[81:59] Okay. Absolutely.
[82:01] This is the time to talk about it. My...
[82:06] Okay. Let's say I have a segment, right?
[82:08] Because that's kind of where I go to do queries. I get my results from the segment, and I mush all those together at the broker level.
[82:18] So in a segment, I've got, let's say, 500,000 rows of my table are stored in a segment. That's probably a lot, but just let's work with it.
[82:30] Yeah. Well, 100,000.
[82:32] Easier number. 100,000 rows.
[82:34] And I'm filtering by zip code and maybe time, but let's just say zip code, right? Postal code.
[82:46] Well, I don't want to have to go through every one of those 100,000 measurements and look up what the zip code is and throw it out if it's not my zip code.
[82:55] That would be like the log problem, right? We didn't want to just...
[83:00] That's terrible. I want to say, "Hey, segment 80002.
[83:07] Where are the rows?" And it'll say, "Ah, okay.
[83:11] Well, it's actually in this part of the segment file that those postal codes are, or that postal code is."
[83:19] So if you just seek on disk to this little chunk right here, you'll get those measurements out that you want.
[83:25] Here exactly are where the 80002 temperature readings are. So just go read this little chunk.
[83:33] So the index is a fast way of narrowing down the range you have to look in. Would you say the broker does that then?
[83:41] No, the server does that. The broker...
[83:45] Okay. Yes.
[83:47] I see where you're going. The broker has ways of knowing what ranges of certain values are in certain segments.
[83:58] So it's doing the smart scattering, but it's indexes are processed at the server level. I'm just going to...
[84:10] It can find stuff. Indexes will from server.
[84:19] Fast way to narrow down your search. Cool.
[84:24] Cool. Thank you.
[84:29] Yeah. Okay.
[84:31] Lerner just brought up a great point, which is that in the relational world, there's pressure not to index too much because when I write to the table, I have to update all the indexes
[84:43] on the table. So if I've got 10 indexes on a table, 10 columns are indexed in different ways.
[84:51] Every time I write a row, I have to go change all 10 of those indexes in the relational world.
[84:59] And so writes... I create those indexes to make reads go faster, but I pay the penalty in writes.
[85:07] So Lerner is responding to real world feedback that you have to think carefully about the right performance trade-off in creating indexes in a relational table.
[85:19] Now ingesting into Pino is a little bit different. It's not like that concern doesn't exist at all, but there's less pressure there.
[85:34] And I need you to let me wave my hands on that just for purposes of time. It's not as severe of a problem.
[85:45] It's not because it's magical. It's just because of when that computation takes place.
[85:49] Oh, you like that one? When something decides to pop up, I guess you get to start listening.
[85:55] Okay. So the whole...
[85:58] I know it's amazing. Back to indexes.
[86:06] There's not just one way of indexing things, right? I gave the example of where is this postal code, but I might also want to know where
[86:14] is this time range? It's Pacific time, 1228 PM, Wednesday, June 21st.
[86:22] What if I want just the measurements from that minute? That's going to be a different kind of index.
[86:29] What if I've got a field that's got JSON in it? It's just a blob of JSON in that field.
[86:36] There's an index for JSON. There's an index for blocks of text doing interesting kinds of queries on blocks of
[86:43] text. There's this whole family of these really cool indexes that I can define on a table
[86:52] that support different kinds of read patterns. JSON, text.
[86:59] Yeah, it'll remind me to keep going. Okay.
[87:08] There you go. And this is Pino specific, right?
[87:18] This is how Pino does it. It's pretty common for databases to have different index types.
[87:26] Postgres would have this story. Other real-time analytics databases in the world, Druid, Clickhouse, they would have
[87:36] an indexing story. Everybody's got that story to one degree or another.
[87:41] Pino has a really cool index called the StarTree index, not to be confused with the company name.
[87:48] We took our company name from a cool index that is... If you've ever done a pivot table in a spreadsheet, it's like making a pivot table in real-time
[88:01] for that table and persisting that pivot table to disk. Oh, it's so cool.
[88:06] Yeah. And a lot of queries are just dramatically sped up by that.
[88:11] And there's even a pluggable mechanism for Pino indexes. So people in the community want to create a new kind of index.
[88:19] You don't even have to. It's through the Java service provider interface mechanism.
[88:23] So you don't even have to rebuild Pino. You just drop a jar file in the right place and Pino can gain new index types.
[88:30] So it's pretty cool. Interesting.
[88:32] That's cool. All right.
[88:34] Now... Ooh.
[88:36] We should probably move towards wrapping up. There's much more to say, but what are you thinking?
[88:44] I'm saving... I'm just going to say, Tim, you might have to come back for a third one when you get
[88:53] back from your honeymoon someday. Okay.
[88:56] Because I feel like I just enjoy talking about databases and learning about all of this. You know where to find me.
[89:05] So if we don't get through everything, just know we can add to it later on or there's lots of different options.
[89:13] Yeah. I mean, this gets into like real specifics at this point that like...
[89:21] Tim teaches databases all the time. Yeah.
[89:28] Well, for example, like remember we said before how events are immutable, an event happens and it has happened.
[89:37] And like click stream data, I clicked on this button in a website, there are little things that capture that and produce those events.
[89:47] Those are immutable events. It's not meaningful for them to change.
[89:50] And so as we're ingesting these things from a Kafka topic and writing them into segments and they're queryable all the time, those just don't change.
[90:00] And that's kind of the assumption with an analytics database is that it's looking at things that have happened in the past.
[90:07] And so once you ingest, you have ingested and those facts never change. Well, you know, not exactly true.
[90:18] Sometimes an event stream is a record of changes to something. Okay.
[90:25] Let's take a thermostat example. When the thermostats report their temperature every minute, that's an event.
[90:34] And once that happens, it is not meaningful for that to change. There's no such thing.
[90:38] Like if you try to alter one of those, you're like covering up a murder or some weird thing. I don't know.
[90:44] You know, that doesn't make any sense to change that. But what about my thermostats themselves?
[90:49] Like what if I take one and rename it and move it from the living room to my office? Well, now it has changed itself, right?
[90:58] The record of the entity has changed. And if that stream is getting ingested into Pino, then I really do have a new event that
[91:10] overwrites an old event. So this is a thing that Pino does really well.
[91:15] If I have a Kafka topic of things like that, where it's updates to things that exist, that's called an upsert.
[91:23] It's an update and an insert combined. You call it an upsert.
[91:27] And that's a, I mean, I don't need to go through that, the whole process. Like I said, the kind of presentation, visuals and everything, but yeah.
[91:34] Would it be kind of like your address change example? Yes, exactly.
[91:39] Like your Amazon. Amazon?
[91:41] Amazon? Amazon.
[91:43] Amazon.com. Yeah, I like it.
[91:48] So for the example you already gave for that one, just for some reason, it's clicking more. It would be Amazon, you want to, you move, you want to change your address.
[92:03] Amazon has your address. It consumed the information, but when you change your address, it creates an event and
[92:11] you have to insert the same thing for the same and replace the value. You have to update, yeah.
[92:17] And there are certain kinds of things in an analytics data stream for certain use cases that have that upsert behavior and Pino has a way of managing those upserts in a high
[92:29] performance way. That's cool.
[92:31] Yeah, it's very cool. Pino can do upsert.
[92:33] That's all we need. All right, well.
[92:50] I'll remember what it means. It's like weird because like, these are my notes from the last streams.
[92:57] Oh, that's so neat. Here's the first one.
[93:03] There we go. This is from the very beginning, but it's me trying to, this is what I was doing on
[93:10] our last stream, but you couldn't see it. And then this is today's stream of random things, so this is, I will make it more consumable.
[93:25] I love it. Thank you.
[93:28] Is there anything else that you wanted to make sure we covered today? No, I mean, this is pretty good.
[93:35] I just kind of wanted to give a little bit of a breakdown of how Pino works and the, I guess in summary, every architectural choice and engineering trade-off inside it is all
[93:47] driven by the idea that it needs to do analytical queries over large sets of data, highly concurrently. So potentially thousands or tens of thousands of, or hundreds of thousand query, a hundred
[94:06] thousand queries per second. That's that once you go user facing, it's not just 10 executives refreshing a dashboard.
[94:14] It could be very large sets of people doing queries all the time. So highly concurrent, very low latency, very fresh data.
[94:24] So all of the engineering decisions are designed to support low latency. So a hundred milliseconds or under for typical stuff, highly concurrent, a hundred thousand
[94:37] concurrent queries per second and data that is seconds old. There's no batch process that you're ingesting every 20 minutes or overnight or anything
[94:47] like that. It's just things happen and they get through the Kafka pipeline and you ingest them and
[94:53] they're queryable. Those are the priorities.
[94:55] All right. Cool.
[94:57] Cool. I definitely will say we went through a lot.
[95:03] I feel like we went on a very long journey and basically we're like D&D, The Expanse and Lord of the Rings with so many different names for the same stuff.
[95:16] All those things happened. They did.
[95:18] They did. And we went through adventures in San Francisco, which I definitely want to go to that museum
[95:28] now, the Computer History Museum. In Mountain View.
[95:33] Yes. That is five minutes away from-
[95:35] How far is Mountain View from San Francisco? Depends on traffic.
[95:39] Okay. Middle of the night, 30 minutes, middle of the day, rush hour, could be an hour.
[95:46] Not horrible. It's not horrible at all.
[95:48] No, it's kind of middle. The Palo Alto Mountain View sort of section is, if you think of San Francisco up here
[95:57] and you kind of come down Silicon Valley proper and San Jose is down here and San Francisco is up here, it's kind of in the middle-ish of the so-called peninsula, which is not really
[96:10] a peninsula, but California makes its own rules. That's okay.
[96:17] That is okay. And before we finish wrapping up, anybody else have questions that you want to ask Tim?
[96:24] Because I know we'll all always have questions. It's a fact.
[96:28] I will be back. You know where to find me.
[96:31] Yes. Yes.
[96:33] All right, y'all. I am going to go raid you over to Coding Garden, dope soul over there.
[96:42] And yes, definitely watch it, Christian. I will be posting it on YouTube, this one on YouTube soon too, so that way you have
[96:54] the playlist. So thank you all.
[96:57] And as a heads up, everyone, Christian's going to come on the stream as well. Yay.
[97:02] Thank you, Lerner. Oh, hey.
[97:04] Hi. We'll see if the raid goes through.
[97:10] I always hit it like too soon, too soon. And I love that you, for everybody that is still here, I love that Alina was on your
[97:17] podcast. Oh yes.
[97:19] Oh my goodness. She's so great.
[97:21] Okay. And...
[97:22] Okay. And... 
