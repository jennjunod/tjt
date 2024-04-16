---
showLink: "https://www.youtube.com/watch?v=dQHg4EAI7W4"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-kafka-with-lucia-cerchie"
title: "Teach Jenn Kafka with Lucia Cerchie"
publishDate: "2023-03-15"
coverImage: "https://i.ytimg.com/vi/dQHg4EAI7W4/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:06] Today, we have Lucia here and I'm excited, and nervous, and anxious,
[00:12] and going back to the excited bit about what we're talking about today.
[00:16] >> Yeah, let's lean into the excitement. That's what I like to do when I'm feeling anxious.
[00:21] Am I anxious or am I actually just really excited to do this? I'm Lucia Cerchi.
[00:26] I am a Developer Advocate at Confluent. I guess I could put a link in the live stream.
[00:33] I'm wondering what that is. But I'm here to talk to you today about Apache Kafka.
[00:39] We'll get an intro on what basic structure is, and then we'll run through working with
[00:46] a little app in the Cloud. I'm excited for that.
[00:50] I'm also excited to be here with Jen. We both came into tech from non-tech backgrounds.
[00:58] We have a lot in common there. I used to be an elementary school teacher
[01:02] and I love bringing that teaching spirit to tech. Because I find it's just really fun to learn
[01:09] something new and then turn around and share it with everybody else I know.
[01:13] >> Thank you, Ben, for this sub. I appreciate it, and yay, and hi.
[01:19] It's not showing in stream here for some reason, but Ben Meyers said hi.
[01:25] I love Ben. Ben is the best. >> Yeah.
[01:29] >> Yes. Ben is one of the OGs of the stream. They were one of my very first guests
[01:39] and original people that always pushed me to go forward. I appreciate it, Ben.
[01:44] Yes, Lucia and I both, I like to say I was tech adjacent.
[01:50] Because I've always been in tech sales or support, but never like the nitty-gritty of like, "Yo, go build shit."
[01:58] I wouldn't have no idea. I knew all the lingo,
[02:02] but I didn't know how to actually do something. >> Got you.
[02:07] >> How did you go from being a teacher to tech? >> I spent four years teaching in elementary school and I was
[02:17] teaching mostly two to 10-year-olds how to read. My specialization was in helping people with
[02:25] learning differences and disabilities get up to speed on reading for their grade level.
[02:30] I knew I wanted to go into something that had a maker's aspect to it.
[02:38] At that point, I did end up going into something tech adjacent. I was in digital marketing for a little bit.
[02:45] Yeah, one of my contracts was with SAS. I was talking to their CEO,
[02:50] who did a lot of the coding because it was a small company. I was like, "I want to do the coding part."
[02:55] [LAUGHTER] >> That sounds good.
[02:57] >> Yeah. Then from there, I signed up for an online boot camp.
[03:01] That was in 2020 and got my first job at a startup that helped with hosted
[03:09] GraphQL APIs and federation and fun stuff. >> Very cool.
[03:15] >> Yeah. From there, I moved to Confluent, where I'm working on spreading the good news of Apache Kafka.
[03:20] >> Nice. Well, I feel like this is really interesting, because I was totally going to put out this tweet yesterday,
[03:29] and lo and behold, this happens. I want to see how many
[03:36] previous teachers or professors I can get on this stream. >> There you go.
[03:43] >> I think I'm up to four. I think Bakari was, Laura was, you were.
[03:54] I feel like there's another one that I'm missing. But how many can I get on this stream?
[03:58] Oh, Anthony? Was it Anthony? I don't remember now, but it's going to be.
[04:04] >> Anthony Campolo? >> Yeah.
[04:06] >> Good question. I know there was music. [LAUGHTER] Hi, Anthony, if you're listening.
[04:14] >> I always call them their, you know people's last names,
[04:20] I just call them their Twitter handle. It's Anthony, AJCWebDev.
[04:26] >> Right. >> Ramon, HolaSoyMilk.
[04:29] >> Yeah. >> That's their last name, that's their Twitter handle.
[04:32] >> No, I would say that for me, breaking into tech was very,
[04:39] I worked at Verizon when iPhones and Androids came out, and had to build that and re-teach it,
[04:45] and then I worked at GoDaddy for quite some time, and had to understand, it's crazy,
[04:53] I don't know if they still do it, but it's a five-week course where if you don't pass the final test,
[05:01] they'll pay you for the training, but then you don't get hired.
[05:04] I think I made it by one question, and I guessed on the question.
[05:15] I'm very, very grateful that I got the job, and it's cool because that gave me a bit more experience.
[05:23] You were asking offline, but if I was from web development,
[05:27] not necessarily because I worked in the e-mail department, and then I worked in the hosting department,
[05:32] but not ever knowing how to build a website or anything. It was more of just how to troubleshoot what was there.
[05:40] I knew concepts, but not, my SQL was a thing.
[05:45] I knew it was called a database. Did I know how to build,
[05:49] what to do with it, or anything like that? No.
[05:52] >> Right. At the same time, it sounds like you were learning to adjust to new concepts very quickly,
[06:00] and how to ramp up on new ideas there. >> That is very true, and I think that is something that I feel very,
[06:07] very grateful for. It's also something that I interned in video production,
[06:13] and to this day, me and a camera on manual does not make sense.
[06:21] It just doesn't make sense. I have taken multiple camera courses.
[06:26] I interned as a videographer, still does not make sense.
[06:31] I'm just like, you know what? Anthony, did you know we were talking about you?
[06:37] Anthony, did you used to be a teacher? We were talking about you.
[06:43] I like to call him my Internet big brother, and then I call Ramon my Internet best friend.
[06:53] >> Okay. I'm going to keep talking because I know it can take forever for replies. But it also is something that,
[07:01] oh, they're not showing up in StreamYard. Yes. Anthony said, yes, Ben.
[07:12] Yes. Okay. All of the things, all of the things. That is true. That is true, Anthony.
[07:21] I do talk about you a lot, especially because when we're talking about breaking into tech,
[07:25] Anthony was one of the first people to introduce me to others, Anthony and Ramon.
[07:32] Yes, that's right. There are at least four teachers now.
[07:37] Also, yes, Ben. Yes, just hands down.
[07:44] You are a lot of guidance. I really should, yes.
[07:48] That is such a good explanation of Ben. You are my Internet Jiminy Cricket,
[07:54] because you always are kind, yet call me out on when I don't do things accessible,
[08:00] and it's hard to remember it all, and I appreciate it. You guys know each other.
[08:08] >> Yeah. >> You guys go way back, way back.
[08:12] Now, I'm curious. >> Yeah. We worked together at a small startup, so yeah.
[08:18] >> Nice. Well, Anthony, she could actually say your last name.
[08:23] I still say Anthony AJC Web Dev. >> Yeah. Now, Anthony introduced me to live streaming, so I'm very grateful.
[08:33] >> Nice. Look at you go, Anthony. Bravo. Yeah, I get that.
[08:43] I do get it that it's like camping in Olo like water polo. It doesn't register when somebody asked me what your last name is.
[08:52] It starts with a C, and then it's like a blink the rest of the letters.
[08:56] I could put a sticky note on my computer, but that'd be weird. We're just going to go with that.
[09:04] Now, this is something that you were talking about offline, Lucia, of how did you get into breaking down really big topics and concepts?
[09:16] Was it specifically going through a bootcamp that did it, or how did you start being able to conceptualize this stuff?
[09:25] >> Yeah. No, that's a great question. I don't know if it was necessarily going through a bootcamp.
[09:31] Introduce me to the specific topic of tech and web development with JavaScript and Python.
[09:37] But it comes to breaking stuff down. It's hard. I remember,
[09:44] I think it was just a lot of self-reflection on how I learn, which is maybe if I share that,
[09:52] it will be helpful to other people. But when I was,
[09:55] say, first learning about things, so even in college,
[10:02] I would get bogged down in details, and I wouldn't necessarily look for the common threads and things,
[10:09] so I'd end up memorizing a lot of stuff, which in tech, nobody wants to memorize stuff.
[10:14] But then I started realizing in a common thread of things, as I started becoming comfortable with different concepts in different areas,
[10:21] like say, when I was learning to teach students how to read, I learned how to teach them how to read using one method,
[10:28] and then I learned a different specific method invented by somebody else at a different time,
[10:34] and then I learned a third method. By that point, I was like, "Okay,
[10:37] I'm seeing the common threads here. I'm starting to see what kinds of teaching methods would fit whichever students."
[10:46] For me, at least, it takes three different implementations of an idea to start really understanding
[10:52] the root concepts and separating that out from the details. Similarly, in tech,
[10:58] I was familiar with building JavaScript APIs and building Python APIs, and then one day I was like, "I'm going to do a Golang tutorial,"
[11:09] and then all of a sudden, all of these things that REST APIs had in common were jumping out at me,
[11:14] like the paradigms with the CRUD applications, and it's all these terms that you hear thrown around,
[11:21] but then you really concretize what that means for yourself when you start actually working with the material.
[11:29] >> Interesting. I love that you break that down. It's definitely something that people keep replying.
[11:42] Bakari, were you a teacher? I need to know. I think you said you were.
[11:48] I know he ran bootcamps. Does that count? I think that counts.
[11:52] Then if that counts, then Ian, we're up to five.
[11:56] Five teacher-professor bootcamp runners. I'm seeing how many I can get on the show.
[12:04] >> Yes. I'm starting to remember these things. To your point about seeing patterns and starting to bring that up,
[12:16] and you talk about reading, which I did not realize this,
[12:21] but I am, we'll change the terminology of it. I am wonderfully dyslexic,
[12:29] and also really annoyed all the time when I have to read. >> Yeah.
[12:34] >> Having to read these comments out loud is always really hard for me. But Ramon, when we first started streaming,
[12:41] he was like, "Jen, you got to do it and you'll get better." Thank you. Good thing I don't have to read right now.
[12:50] >> Do different fonts help you out? >> Not really, because I would say for myself,
[12:59] it's a lot of mixing. The fonts, yeah, they can help,
[13:03] but I still skip words or I still skip letters. There's plenty of times, especially when I am writing,
[13:11] I will just skip words altogether. I'm just like, "Oh, that would have helped."
[13:18] Well, we'll get there, maybe. Concepts and patterns are one thing that really,
[13:25] really stuck out to me and I subconsciously was doing, but didn't realize until two of the concepts that you mentioned,
[13:33] which are APIs. I used to work for an API company,
[13:37] and to this day, I get what an API is,
[13:43] yet I really struggle with the fact of remembering what REST is and all the different parts of it.
[13:54] We've done APIs on Teach Gen Tech. I believe in two weeks,
[14:00] Ian from Postman is going to come on and talk bare basics of APIs. I'm so excited because I'm like,
[14:07] I need a refresher. It's been a while. Yes,
[14:12] we are talking. Is it Kafka or Kafka?
[14:16] >> It's Kafka. >> Kafka.
[14:19] >> Yeah. >> Like, is it like a tomato,
[14:24] tomato kind of thing or? >> Good question. I think it's,
[14:31] well, so it was named because Kafka producers, which we'll talk about in a second,
[14:37] are great at writing at high throughput and low latency. It was named after Franz Kafka, the writer.
[14:47] Since most people whom I've heard refer to him as Kafka instead of Kafka, but yeah, I personally am not going to come after you if you call it Kafka.
[15:00] >> I think I keep calling it both and every single time I say it. >> Because somebody's telling you together.
[15:05] >> Yeah, because it's also like my last name is Junod, but everybody says Junod because Americans.
[15:17] I think that's the other thing that goes through my head. I'm like, Kafka, Kafka, Kafka, Kafka.
[15:24] Whatever. Yes, yes, and Laura, I dig it. She is not dyslexic,
[15:29] but she thinks we get smart fast. It's crazy. Yes, Bakari, I agree with that one.
[15:37] Kafka is the Midwestern version? Okay, this is me not knowing how to sound out my words,
[15:46] so I'm just going to put it in. >> I know. Maybe it's Kafka.
[15:50] >> Tell us about the scary thing we are learning today. >> Yeah.
[15:57] >> Very exciting. >> Very exciting. Apache Kafka is an event streaming platform.
[16:09] It's open source, it's distributed. There's a lot of different use cases.
[16:13] You can use it for event-driven applications, and basically we're going to get started on doing one of those today.
[16:20] You can also use it for constructing things like data pipelines. I don't know much about this,
[16:27] but you can use it for modernizing your mainframe. Basically, anything where you need to move a lot of data
[16:36] very quickly is a good use case for Apache Kafka. First of all, I'm going to stop and see if we have any questions about that.
[16:48] I was just going to say that I'm guessing you're going to break down half the words you just said and ask through there.
[16:56] I wasn't going to go too worried about it because as many of you know, I got a new job, finally, yay.
[17:03] I work at Ivy, which is data infrastructure. We also do things with Kafka and Flink and a whole bunch of other things.
[17:15] One of the things that are said often is event-driven or event-stream, and I'm like, what?
[17:24] It does a thing, it does a thing, and that is why I have to teach Gen Tech is to learn these things.
[17:30] >> Let's focus in on that term event. An event is a thing that happens,
[17:36] which is not going to be news to many people. But in Kafka, they're represented by key and a value.
[17:45] They usually also have a timestamp that's important to mention. One of the things that I was a little bit confused by when I was
[17:58] first learning about events was like, okay, what makes these special because people are telling me,
[18:04] events are replacing objects and that just makes everything great. It's an event-driven application.
[18:11] I was like, what? Because with events, they're often encoded in JSON or Avra,
[18:18] which is like JSON with special rules, and that looks like an object.
[18:23] But what makes it different is how events are handled in event-driven applications.
[18:32] Say you were coding a ride-share app, and you had an object that was represented a request from a user,
[18:40] and you want to represent a new request, so you send a request to the API for that object and it comes back.
[18:46] That's one pattern. But when it comes to events,
[18:50] that event is a new update in an event streaming application, and it's part of a subscriber subscribed to it.
[19:02] As soon as that event happens, the subscriber reacts to it.
[19:06] So it's a different pattern of designing applications. >> We're going to go with, yeah.
[19:17] >> Anthony is the head of the game. But yeah, so events are stored.
[19:21] I'm going to use these beads that my daughter uses to represent each of these beads as an event.
[19:28] They're stored in something that's called a topic, and the underlying data structure of a topic is a log,
[19:35] and you can't change the events once they're in the log. So I don't know enough about Blockchain to answer you on that, Anthony.
[19:44] >> I do think it is in the fact that once it's there, you can't change it whatsoever.
[19:51] You know how in a website, you can go back and change something and then publish it?
[19:56] In Blockchain, you can change something, but it's going to create a new block instead of just replacing what's there.
[20:05] >> Right. So if you wanted to filter out all of the circles on this topic, you'd have to make a new one based on this one.
[20:13] There is a similarity there, yeah. >> Okay.
[20:16] >> You also can't delete one of these events. That's another. So it's coming from a GraphQL world
[20:24] where literally everything is mutable and deletable. So it's like, "Oh, that's new."
[20:28] The other thing about topics is that they are split up into partitions.
[20:35] So it's like, you have two logs here. Let me see if I can move them on the screen.
[20:40] These partitions, each of them can go live on a different server, and that makes Kafka very performant.
[20:50] So I have a co-worker this morning, and we're talking about this like,
[20:53] "What is it about partitions that makes them performant?" My co-worker's name is Chris Jenkins,
[20:58] came up with a great example for why partitions make apps so performant. Basically, he said, he's like, "Think about sending out emails or SMSs."
[21:09] Now, sometimes the servers for those can be very slow, and you might only be able to send one outbound message per second.
[21:17] So think about what that means for an hour. You're limited to 3,600 messages,
[21:23] given that that's the number of seconds in an hour. What if your business is larger than that, right?
[21:30] So in Kafka, if you have like 10 partitions in a topic, and you have 10...
[21:37] So I need to back up a little bit. It's like a publish-subscribe system.
[21:42] So you have publishers called producers and subscribers, which will register and read those events,
[21:47] like called consumers. - Let's go, yeah.
[21:51] - Yeah, let's do it. - Yes, yes.
[21:53] That actually made it really funny because it is blockchain, because you, Lucia, did have blockchain on the screen.
[22:00] But yes, it was also like... - There's always something about these analogies that is not perfect.
[22:06] So I'm always trying to find the perfect partition analogy. But you had a question.
[22:10] - But just on blockchain, you can't delete either. So that one is very similar as well.
[22:17] Okay, so I think this is also, when we were talking about earlier, like really difficult topics and concepts,
[22:26] a lot of what is hard to learn are all the new words, or words that you know but mean something else in tech.
[22:34] - Yeah. - Which is not my favorite. It is like my least favorite.
[22:39] - Yeah, naming things is hard, right? And sometimes in tech, like people will pick a cute name very quickly,
[22:46] and then it doesn't exactly work out for like helping people understand what it is. - And y'all may have seen me look down quite a bit.
[22:54] I am taking very random notes to try to like keep up and understand. And okay, so what is the topic?
[23:06] - Right, so the topic is that log of events. - Okay.
[23:10] - And it could be like emails, right? Or in that ride share app example, it could be like ride requests.
[23:20] - Okay, that makes sense. So before we go to partitions, what were you saying about subscribers and what?
[23:29] - Right, so let's back up the whole, I got into the example too quickly. Let's back up the whole bus and get into, yeah.
[23:36] So Kafka is an example of, basically an example of a Pub/Sub system. So, and what that is, is basically it's a system where the publishers of data
[23:51] don't have to be connected to the subscribers, so the things that are reading the data.
[23:57] They're decoupled entirely. There's like a central place where the messages are published and read.
[24:03] In Kafka, that's a topic. Now, those publishers in Kafka are called producers,
[24:08] and those subscribers in Kafka are called consumers. And it's important to remember with consumers,
[24:14] consumer sounds like it's eating it, right? It's not actually consuming it.
[24:19] So once a consumer consumes an event from a topic, that event remains in the topic. And two consumers can read two events from the same topic at the same time due to...
[24:33] - Okay. - ...partitioning thing, which we'll get into in a second.
[24:35] So I'm going to stop here and we'll... - Really quick.
[24:41] Anthony, I'm actually looking at getting an iPad that I'm hoping I can also screen share if needed, like during this type of example,
[24:49] so that way I can draw things out when people are talking because I don't type fast. - Wow, that would be awesome.
[24:55] That would really help me understand, too, like the quality of my explanations. Yeah.
[25:00] - And then just before I go into, Ben said, "You can also think of topics as like a physical message board that multiple people can stop by and read."
[25:10] Okay, so topics by itself totally make sense to me. - Cool. It's a log of events.
[25:16] Got it. What you just said about the Pub/Sub system and that publishers are produced...
[25:27] - Okay, so if Pub/Sub is confusing, let's drop it right now and just talk about how do events get into topics.
[25:36] - Okay, I like that. - All right.
[25:39] That is a producer's job. - Okay.
[25:43] - Yeah, so a producer writes events to topics, and I'll wait for you to finish your note, and then we can continue.
[25:50] - Okay. Okay.
[25:59] Got it. - The other things that it can do is, like, it can batch data and send a bunch
[26:05] at the same time. - Okay.
[26:07] - And then the next part is...this is a little bit...so, every event had a key and a value, like I mentioned before, right?
[26:21] And every topic is split into these partitions that can live on different servers.
[26:26] - Mm-hmm. - Okay.
[26:27] - Producers assign events to different partitions based on a hash of that event's key.
[26:38] - Assigns events to producers. - To partitions.
[26:43] - To partitions, thank you. Well, this actually brings to my next question.
[26:51] So, assigns events to partitions based on hash key? - On a hash of the key.
[26:57] So, basically, what that means is it'll perform, like, a hash function on the key, and events with the same key will end up in the same partition.
[27:08] - Okay. So, like, a value makes sense to me.
[27:14] An API key makes sense, but more of just because you have to pull it and put it somewhere.
[27:19] - Right. This key has nothing to do with authentication.
[27:22] It's just, like, key value pairs. - Where do you get a key?
[27:27] Can I put, like, gens as the key? - So, I mean, you could.
[27:33] - Or, like, 42 is the, you know, the answer to life? Like, how do you make a key?
[27:39] - So, this is a great question, and it's the right question to ask when you're thinking about Kafka applications, right?
[27:44] Is when you're thinking about writing your events, you're thinking about since they're partitioned by key, you want to think about what you put in the key so
[27:54] that, you know, you have your events basically, like, organized within your topic.
[28:05] - What goes into it? Like, how do you create a key?
[28:07] Like, does a key have... I feel like I'm going to use the Googles.
[28:11] The Googles and I are friends. - Yeah, I could also start showing you what they look like.
[28:16] - Okay, cool. - Yeah.
[28:19] Our keys, actually, in this example, are going to be null, so they're not going to...
[28:23] They're going to be a size... There's, like, a round-robin method used instead when your keys are null.
[28:27] So, we're not... But they can be null or, like, a string.
[28:33] So, we were on keys, not partitions. - Okay, but they can be strings?
[28:39] - Yeah. - Okay.
[28:41] - I mean, it all goes down to bytes in the end, but, like, kind of everything does in text, so I don't like...
[28:45] - Right, but it doesn't mean to be, like, a specific integer or something like that.
[28:50] - Yeah, no, it would be, like, a byte type, converted into bytes. And it could probably be an integer or two.
[28:59] I would have to check. Pretty sure I used one of my last applications, but...
[29:06] - Nope. - Yeah.
[29:08] - Okay, cool. - Yeah, so...
[29:12] Now, reading these is another thing. And we're going to need to get to consumers.
[29:22] So, consumers are the things that read the events from the topics. - Okay.
[29:29] - All right, and they don't have to do any compression or, like, key assignment or anything like that.
[29:36] More than one consumer can read from more than one topic. They'll both read from different partitions.
[29:44] - Okay. - So, what that allows you to do is scale things up, right?
[29:55] So, do we have more questions? We're good to go back to the email example.
[30:02] - I think I'm good. If anybody else in the chat has questions, let us know.
[30:07] We can go back. - Okay. - I don't think we're good.
[30:13] - Yeah, so, if you're, like, limited to that number of messages an hour because you've got one server, you can use Kafka to send and read
[30:26] these messages, which is a good mechanism for scaling because each of those partitions lives on a different server, and you could create,
[30:34] like, 10 partitions in a topic and get up to, like, 36,000 messages an hour, which is a lot better than 3,600.
[30:42] Does that make sense? - It makes me think that Twilio uses Kafka.
[30:48] - I don't know the answer to that question. It wouldn't surprise me if it did, but...
[30:53] - Anybody know, like, in our chat? I'm curious now, but please continue.
[30:59] - Yeah. So, with that in mind, I'm going to try to think over what I've gone over.
[31:07] I think we've gone over, like, the key concepts that I wanted to treat before I share my screen and get into what we're going to do.
[31:16] But with that in mind, we're going to start out with a fun type of event. I'm going to get a link to it into the chat here.
[31:22] Hold on. - Cool.
[31:25] - So, we're going to be working with... I can only put it in the private chat, apparently.
[31:30] - That's fine. I'll copy and paste it over.
[31:32] - Yeah. We're going to work with data from automatic identification systems for boats.
[31:39] So, basically, it's kind of like FAA traffic for planes, but for boats. All boats that are over, like, a certain weight and are international have to send
[31:55] out signals that define, like, their location and their speed and, like, other information.
[32:01] And we're going to connect to a web port that gives us that data live. And then we're going to pipe that into a Kafka topic.
[32:11] So, that's, like, two steps. Let's just focus on those for now.
[32:16] Yeah. So, let's look at what that data looks like.
[32:19] I will pull up my screen and kind of get this terminal nice and big here so that we don't...
[32:32] - Great. I will add yours to the stream.
[32:35] Yay. - Yay.
[32:37] - Can you just make the text a bit bigger, please? - Yes.
[32:42] How is that? - Yay.
[32:44] Much better. Thank you.
[32:47] - I'm going to grab... So, this...
[32:50] I have a command here, and this is doing a few different things. So, we're going to go through it by pipe and just walk through what it does before
[32:57] we see the output. So, this is the NC stands for Netcat, and that allows you to, like,
[33:04] connect to random ports on the internet. This one's maintained by the Norwegian...
[33:10] I don't think it's, like, port authority, but it's, like, the Norwegian government.
[33:15] And so, we're connecting into that port, and they send out the data that they get in there.
[33:19] This is GPS decode, which basically takes the format of that data, makes it more readable.
[33:24] However, that's not necessarily in the nicest, like, JSON ever. So, I'm using this utility called jq in order to format the JSON in,
[33:34] like, a readable way. So, when I enter, this command will...
[33:41] All of this data will be piped through, like, all of that, and we'll begin to see the different ports coming in.
[33:51] Give me a second. Sometimes these things take...
[33:52] There we go. So, I'll hit pause just so we can, like, scroll through some of this.
[33:59] But yeah, so, this data is... It's AS data, right?
[34:04] And then, not all of the ships give out the same pieces of data, but what we are going to be looking for eventually will be this,
[34:14] which is, like, a ship's ID, the MMSI. I don't know what that stands for, but it's the ID.
[34:20] And then, the Latin one. And then, we can even get, like, the speed.
[34:23] I think this is in knots. I hope it's accurate.
[34:26] That's kind of a funny field to me. And then, other things like that, like, maybe this is a radio address,
[34:33] and you could, like, radio them. That would be cool.
[34:36] But that's the data that we are going to work on piping into Kafka. - Okay.
[34:41] So, to repeat that back to you, you sent us a link to a wiki page. That is where you got the connection to the boat data.
[34:57] - So, yeah, I can give you the link to the Norwegian government's page, too, for that, when I'm finished sharing my screen.
[35:05] - Yeah. I'm guessing it's probably one of the things here that we could always look into.
[35:10] And then, we go to the Norwegian human's port and use their IP address to go into it to get the GPS, but it's decoded, but not very easy to read.
[35:26] So, we use the jqunbuffed to make it readable. - Right, right.
[35:32] And unbuffered does something, I think it just makes sure that all the data is sent before you hit exit out.
[35:38] That's what that flag does. I can relook that up, but I remember making sure that I knew what that meant,
[35:44] and that's what that does, so. - And then, are we using...
[35:48] I get that the MMSI is the identifier, but are we using that as the key? - No, we will just actually be piping into a topic with a null key in this demo,
[36:00] but that might be... - Oh, yeah, yeah, yeah.
[36:02] - ...used as a key, right, if we wanted one partition per vote. - Okay.
[36:08] - Yeah. Yeah, good thinking.
[36:10] - Cool. So far, I'm picking up what you're putting down.
[36:14] - Awesome. So, the next thing that we're going to do is...
[36:17] So, this command is a bit long, so I'm going to format it. We're going to use a utility called kcat, and what that stands for is Kafka Cat.
[36:30] I have a link, again, that I will... I'll just do a big link dump at the end of this.
[36:34] - Cool, thank you. - Yeah, of course.
[36:38] And I have put in all of this... I've gone into, like, a kcat configuration file, and I've put in a bunch of
[36:44] connection details, and that is connecting up to Confluent Cloud. But let me back up a second.
[36:51] Hold on. So, kcat is, like, used to be called Kafka Cat, and you know how, like,
[36:56] when you hit cat and then a file, and then you can see what's in the file? Kcat lets you see, like, what's inside your Kafka topics.
[37:06] And it also allows you to produce to them by passing this cool little flag. But before we even do that, we have to back up a step.
[37:17] I realized I was getting ahead of myself. And we have to jump into Confluent Cloud and create a topic to pipe this to, right?
[37:23] Because if there's no topic, then it's going to send... Actually, it'll be interesting to see what kind of error that sent.
[37:30] Let's see. Might just not do anything for me.
[37:36] But we're definitely going to go into Confluent Cloud and create that topic so that it has something to pipe to.
[37:45] So, I'm going to log in here. Okay.
[37:58] So, this is, like, my Confluent Cloud dashboard. And I'll be managing basically the servers that I've got running
[38:04] through Confluent Cloud here. I've got different environments set up.
[38:08] These are, like, side projects. - Can you make it a smidge bigger, please?
[38:12] - Yes, of course. Is that better?
[38:16] - So much better. Thank you.
[38:19] - Yeah. And I've created an environment for this demo here.
[38:23] We've got one cluster of servers running already. So, I'm going to click on that.
[38:30] Okay. I'm going to make a topic.
[38:33] I'm going to accept the default configuration here. But I'm going to change my topic name to one that'll fit.
[38:41] So, AIS. I'm going to skip defining a data contract for now.
[38:49] So, this is my topic in Confluent Cloud. I have a configuration panel with some default details, which we're going to leave
[38:58] for now, and I could make a schema, which we could get into later, maybe at the end of the live stream when we're talking about different applications for this.
[39:08] But we don't need a schema for right now. And then this panel is the messages panel, we'll see messages coming in once we start
[39:15] piping in that data. But there won't be any data coming in now because we're not producing any data there.
[39:24] So, let's return to the terminal and run that command. Okay, so, another important thing is that I have in the KCAT configuration file, I've
[39:41] put the authentication or the, yeah, the authentication details. So, there's like a key in there that enables me to connect to that cloud.
[39:49] So, when I run this, it might take a couple seconds, but we'll get new messages in here. >> And where do you edit your KCAT?
[40:03] >> That is a great question. So, let me pull up, oh, there's no data coming in.
[40:08] Let me pull up, there's a great blog post. So, I rely a lot on the blog posts of my coworkers.
[40:16] So, for example, this AAS demo is based on a blog post by my coworker, or former coworker Robin Moffat, who made a whole app to find out which boats were clustered together closely
[40:33] using Kafka. So, I'll put that in the chat as well.
[40:36] >> Cool. >> So, you'll see infinite me for a second.
[40:39] But then there's also a blog that my current coworker Chris Jenkins made about how to configure your KCAT utility.
[40:48] So, those two. >> Sweet.
[40:50] Oh, it made it as, I'll post them twice, because sometimes StreamYard likes to try to put them all together as one, not what I want.
[41:05] >> Okay. So, we've got this message coming in.
[41:10] And it's got the value, and that's just the JSON data that we piped in. The header is empty for now.
[41:18] We could put metadata in there, if we wanted. And as you can see, the key for this is null, so it's all going to be assigned to the different
[41:28] partitions. Right, Robin?
[41:30] Sorry. I'm going to drink some water.
[41:32] >> Do it. >> All right.
[41:34] So, this data is coming in basically non-filtered, right? We just got all of the data that we could.
[41:44] So, the next step is going to be using ksqlDB to filter the data. And what ksql, okay, I'll back up a second, too, because there's like an underlying, what
[42:02] underlies ksqlDB is this library called Kafka Streams, and you can implement your own solution yourself with Java and filter streams data that way.
[42:14] Or you can use ksqlDB, which uses SQLite syntax, and then you can start creating streams and filtering your data using SQLite syntax here, so that's what we're going to do today.
[42:29] And if at any point you have questions, you can just go ahead and interrupt me, because since I can't see your face, I can't take cues.
[42:38] I think it's definitely something where, like, what you're saying is starting to conceptually make sense, but there are still like a ton of words that don't, but I'm writing them
[42:50] down as we go, so that way I don't have to ask you about every single one of them, because that would take us forever.
[42:56] So, you're giving me a lot to think on. >> Yeah, any questions after, like, we're finished creating the cluster and filtering
[43:03] stuff? >> Basically, what we're going to do is we're going to use SQL syntax to create new streams
[43:11] and filter them. So I'm going to create this cluster, continue.
[43:21] Global access should be fine. I'm also just going to accept the cluster name, and it takes a couple seconds to launch
[43:29] the cluster. Oh, no.
[43:31] Something went wrong. I'm going to fix it.
[43:34] It could be that I'm out of API keys, so because that's an API key issue, I'm going to stop sharing my screen for a moment and double check that.
[43:47] >> Sweet. Definitely, you've given me a lot to look at, but, like, I know for myself, it's, like,
[43:57] what you're saying makes sense. Like, I know SQL is a thing.
[43:59] Like, I am going to start doing my own, like, understanding walkthroughs of, like, Postgres and MySQL and those type of things, but at the same time, when you're, like, SQL syntax,
[44:13] I'm, like, I don't know what that is yet, but I'll get there. Another one is, like, creating a cluster, and I think this is something that we added
[44:24] to, like, my to-do list of figuring out streaming of, like, does that have something to do clouds having something to do with, like, does cluster have something to do with clouds?
[44:39] Wow. Words.
[44:41] They help. And looking more into that, because I think that's a little confusing, but also something
[44:49] that would make more sense when I'm actually going through it and can, like, Google these certain things that I don't understand.
[44:56] Yeah. So here, that was definitely something that I was, like, everybody's using cluster, or,
[45:04] like, it's, you know, an assumed, it's a cluster of servers, so it's, like, a group of servers, and provisioning them using the cloud, so I don't know.
[45:18] Hopefully that helps. That's what I was guessing.
[45:20] Yeah, cluster sounds yummy, like cookies or something, it's just servers. That's funny.
[45:29] That's funny. I feel like that would be really cool.
[45:33] I don't know if Laura is still watching, but we talked about it yesterday that we need to do, like, a makeup markdown stream, just, like, hey, for those who enjoy makeup, join
[45:45] us and we'll create a markdown. I don't know.
[45:48] Yeah. Can we, like, do a markdown while we're doing our makeup?
[45:52] Ooh, that sounds like a TikTok. That would be kind of complicated, though, because I don't know how you would talk about
[45:59] markdown without showing what you're doing, so I don't think you could do makeup at the same time.
[46:06] Yeah. I don't know.
[46:08] And you could probably, like, have one person doing their makeup and then a person doing a markdown and then switch.
[46:13] That is true. Laura, yay.
[46:15] And did you hear what Lucia just said? Like, we could take turns doing makeup and one of us explaining markdown.
[46:27] I'm so down. I'm so down.
[46:29] All right. So, got through the cluster issue.
[46:35] It's still busy provisioning, which means just getting set up so we can connect to it. So we'll wait for that.
[46:42] Let me see if I have any fun links to share while we're waiting for that to go. Sweet.
[46:47] Laura just said, "Devrel, get ready with me." I like it.
[46:51] Awesome. I have a blog post here, we were talking about learning things earlier.
[46:58] That's kind of, like, my little take on how to, like, learn new things. I like it.
[47:05] Yeah. And then we've got, let's see.
[47:12] Oh, here's a couple of really fun Kafka resources. It'll be interesting to see how these, I had them in bullet points so they might translate
[47:18] funny. They did.
[47:20] Hold on. But one of them is called "Gently Down the Stream" and it's, like, it's basically, like,
[47:27] an online comic book that uses little otters to describe Kafka and I love it so much. Yes.
[47:33] Yes. Yeah.
[47:35] So that's really great. And then Confluent Developer has this, like, one-on-one course on Apache Kafka, in case
[47:45] the stream peaked your curiosity. Sweet.
[47:47] Yeah. Those are two, like, good introductory resources or clusters up.
[47:52] And I was sharing my screen with infinite share while I was sharing this link, so I apologize.
[47:56] I just realized. All right.
[47:58] So I will add you back to the stream. All right.
[48:00] We can see Confluent. Okay.
[48:02] Awesome. So let's go ahead and get started.
[48:04] So let's go ahead and get started. So let's go ahead and get started.
[48:06] So let's go ahead and get started. So let's go ahead and get started.
[48:08] So let's go ahead and get started. So let's go ahead and get started.
[48:10] So let's go ahead and get started. So let's go ahead and get started.
[48:12] So let's go ahead and get started. So let's go ahead and get started.
[48:14] So let's go ahead and get started. So let's go ahead and get started.
[48:16] So let's go ahead and get started. So let's go ahead and get started.
[48:18] So let's go ahead and get started. So let's go ahead and get started.
[48:20] So let's go ahead and get started. So let's go ahead and get started.
[48:22] So let's go ahead and get started. So let's go ahead and get started.
[48:25] So let's go ahead and get started. So let's go ahead and get started.
[48:27] So let's go ahead and get started. So let's go ahead and get started.
[48:29] So let's go ahead and get started. So let's go ahead and get started.
[48:31] So let's go ahead and get started. So let's go ahead and get started.
[48:33] So let's go ahead and get started. So let's go ahead and get started.
[48:35] So let's go ahead and get started. So let's go ahead and get started.
[48:37] So let's go ahead and get started. So let's go ahead and get started.
[48:39] So let's go ahead and get started. So let's go ahead and get started.
[48:41] So let's go ahead and get started. So let's go ahead and get started.
[48:43] So let's go ahead and get started. So let's go ahead and get started.
[48:46] So let's go ahead and get started. So let's go ahead and get started.
[48:48] So let's go ahead and get started. So let's go ahead and get started.
[48:50] So let's go ahead and get started. So let's go ahead and get started.
[48:52] So let's go ahead and get started. So let's go ahead and get started.
[48:54] So let's go ahead and get started. So let's go ahead and get started.
[48:56] So let's go ahead and get started. So let's go ahead and get started.
[48:58] So let's go ahead and get started. So let's go ahead and get started.
[49:00] So let's go ahead and get started. So let's go ahead and get started.
[49:02] So let's go ahead and get started. So let's go ahead and get started.
[49:04] So let's go ahead and get started. So let's go ahead and get started.
[49:07] So let's go ahead and get started. So let's go ahead and get started.
[49:09] So let's go ahead and get started. So let's go ahead and get started.
[49:11] So let's go ahead and get started. So let's go ahead and get started.
[49:13] So let's go ahead and get started. So let's go ahead and get started.
[49:15] So let's go ahead and get started. So let's go ahead and get started.
[49:17] So let's go ahead and get started. So let's go ahead and get started.
[49:19] So let's go ahead and get started. So let's go ahead and get started.
[49:21] So let's go ahead and get started. So let's go ahead and get started.
[49:23] So let's go ahead and get started. So let's go ahead and get started.
[49:25] So let's go ahead and get started. And the source is the Kafka topic that we created.
[49:29] The AIS data topic. So when I run this query, we get a response with a success status.
[49:39] That's what I'm looking for. And if we go over to the streams tab, we'll see it come up in a minute here
[49:47] because we just created it. There it is.
[49:50] Side note, this ksql processing log is cool. You can query it and get, like, errors if your streams aren't working the way
[49:57] you thought they were. Good thing we're not seeing any messages right now.
[50:00] That makes me happy. Yay.
[50:03] But -- oops. There we go.
[50:08] I just -- my mouse is, like -- it's getting a little, like, sweaty. So, all right.
[50:12] So this is our AIS stream, and we would like to query it and see if it works. So this looks like sql here, select star, which means all of those columns
[50:25] from the AIS stream. Emit changes means it's going to be picking up all of the -- stop and try again.
[50:34] Oh, there we go. It's going to be picking up all of the changes in that topic as they're
[50:39] piped in. So we have all of the data there.
[50:43] So it's a little bit -- it's a little bit of, like, a mindset change I found from making queries on database tables, which are static, right, whereas
[50:53] topics are constantly flowing with data. So that's a little bit of a difference.
[50:59] But we're seeing our data come in here, which is what we wanted. Now I'm going to stop in case we have questions, and then we can continue
[51:08] to the next query. >> I feel like -- can you go up a little bit on your screen?
[51:13] >> Yeah. >> Down a smidge, just to go over.
[51:17] So we have the editor, which is where we told it what JSON -- like, the source is JSON and what we wanted to pull.
[51:29] Flow is -- do we need to know what flow is? >> It's kind of like a visualization of the streams.
[51:36] >> Okay, cool. Yeah, so there's no connection between these two in particular right now.
[51:42] But I think when I create a filtered one, we'll see, like, an arrow and a new one.
[51:48] So let's experiment in a second with that. >> Great.
[51:52] >> Yeah. And then under persistent queries, we'll -- we may see -- this is, like, if
[51:59] you have a query that is continuously transforming data, it would show up there.
[52:06] I'm going to go back. I'm going to keep -- I'm going to run this query one more time, because I
[52:11] want to see some messages coming in. Now, the new query that I'm going to run is going to look something like
[52:18] -- I'm going to paste it into the editor here. It's going to look something like that.
[52:23] And we want to pick an ID that shows up. And so we want to see one that comes up, like, more than once.
[52:32] Just to make sure that we can have a flow, right? Because if it's a boat that's, like, stopped and only sent out one piece of
[52:38] data, we don't want to try to make a stream based on that. So 259.
[52:44] I'm just going to scroll through these really quick and then, like, pick one. Is this the same 258?
[52:52] Okay. This is going to take, like, a little -- actually, it might make more sense to
[52:57] pull one from the terminal, but we'll see. So, yeah.
[53:11] Okay. That one showed up more than once.
[53:13] We'll use that. All right.
[53:15] So what this does is it uses the AS stream that we just created as a base. And we're going to be selecting the ID, the latitude and longitude from that
[53:27] stream where the MMSI equals this particular ID, so for a specific boat. So we're going to run that query now.
[53:40] Okay. And we've created it.
[53:42] Now we can query it. Actually, let's -- I'm curious about the flow.
[53:46] There we go. Yeah.
[53:48] So now that we've created that stream based on the original stream that we created here, so the filtered stream for one boat, and we can see the data
[53:57] coming in. Lat/long is null.
[54:00] Aw. It must be, like, static.
[54:03] So sometimes the boats don't move, and so the lat/long is not coming in. But, yeah, you can see the data coming in for that particular boat based on
[54:11] this stream. I mean, you could also query it to see that information, too.
[54:17] Yeah. And that's actually a persistent query because it's continuously filtering the
[54:27] original stream. And then remind me, what is the difference between a stream and an event?
[54:39] So an event just is, like, something that happens, you know, with -- but what is a stream?
[54:47] And a stream is different than a cluster, but a stream happens on a cluster? Okay.
[54:50] Yeah. So let's take that one at a time.
[54:53] Difference between a stream and an event, this whole collection here is a stream, and then these particular messages coming in are the events.
[55:03] Okay. So multiple events make a stream.
[55:07] Right. A stream is basically -- it's like a flowing table.
[55:18] We also have tables, which are, like, snapshots that you can take. But it's like a flowing table that you can -- that's informed by a topic, and
[55:30] you can perform, like, different transformations or aggregations on these different streams.
[55:39] Okay. And then what about, like, the stream versus, like -- just to, like, get to
[55:53] where we are right now is so we had the boat data, which is just ongoing data that they're, like, yo, this is where we put all our boat information.
[56:03] And then we put it into -- by running it with the net cap and GPS decode and JQ unbuffed, it created it and put it into a JSON file?
[56:20] So it actually piped it into -- it put it into JSON format, and then that was piped into Kafka from the terminal.
[56:34] So into a topic from the terminal. And you had to create the cluster and create the topic in Confluent, but once
[56:43] you did that, then you could tell -- in terminal, tell it to run KCAP, to then put it into the cluster.
[56:57] And then we told it to run ksqlDB to be able to decode it. Yeah, good question.
[57:11] So it's already, like, decoded in the interface for you. So within the context of Kafka, decoding and encoding means something that
[57:23] relates to the serialization of bytes. So let's -- what it does is you can filter it based on the streams.
[57:35] Okay. Which created filters.
[57:40] Okay. And then which that then created, like, we had AIS, which is the original
[57:52] topic that we created, and then the ksql processing log is the stream we created, and then we created the filter, which connected the two.
[58:03] Yeah, so this is actually in a separate topic that Confluent is running in the background to give you, like, error messages, this ksql processing log.
[58:12] This is run based on our topic, the AIS stream, and then this one is a filter on that AIS stream.
[58:25] This AIS filtered topic. Does that help?
[58:30] Kind of. I'm going with, like, what you're saying makes enough sense, but there's
[58:35] so many things that are also still very confusing. At one point you used the word broker.
[58:44] Oh, sorry. That is a server with, like, that has, like, metadata information on it.
[58:53] It's -- yeah, it's a server. I think that's going to be the funniest thing is, like, so far we have a
[59:04] producer, we have consumers, we have a broker. It sounds like a joke about people going into a bar.
[59:15] Yeah, yeah. So a broker and some streams and, yeah.
[59:21] Yeah, no, that's -- that's fair, yeah. I think it's definitely a lot that I need to look into, because, like,
[59:29] what you're saying and talking about does make enough sense. I don't think that I've, I guess could say, like, I've leveled up enough
[59:40] to get to the point where I'm fully understanding where we're at. I feel like I am soon, especially with all of the streams I'll be having,
[59:49] because we're, like, starting as small as, like, what is data. So you gave us a really big topic, and this has happened a lot.
[60:01] Like, I had Trevor on the show, and he talks about Kubernetes and Docker and PowerShell.
[60:16] No idea what he was saying. Like, it made sense, but it didn't make sense.
[60:21] I've also had somebody come on about Golang. So it's definitely something that I'm, like --
[60:26] Yeah, you will learn so much, too, just by osmosis, by listening to these conversations and being part of them.
[60:33] Yeah, it's definitely -- I've really felt like that when I was first learning Kafka and then also when I was first learning how to code, right?
[60:43] Like, there's a lot of new vocabulary, and that can lead to, like, some overwhelm, too, right?
[60:51] A hundred percent. I think it's important to, like, have patience with yourself and realize,
[60:55] like, hey, if I didn't know something today, it just means I learned something, right?
[61:01] Yes. Yeah, and I'll be able to apply it later in the future.
[61:06] And then, like, in a few months, like, I'm sure you've had this experience with learning new things.
[61:12] All of a sudden, you'll be able to, like, pull a definition for something out, or you'll be able to help someone else learn a new concept by using
[61:20] some kind of analogy, and you realized, oh, I've internalized this new knowledge, and you'll feel really good about it.
[61:25] Yeah, I feel like that is a big part of what I love about Teach Gen Tech and, like, the show is, like, learning it, they always build on top of each
[61:35] other, even if they're not always in a linear order. Like, we went really high level for this one, and then I'm going to go back
[61:45] to the basics. This is also something that I love about, like, my stream with Laura, we do
[61:52] Python every other Friday, and then I also am learning TypeScript with Josh the opposite Fridays, and it's, like, those are teaching me the fundamentals
[62:02] that I kind of, like, knew existed, but I didn't really have the words to it, like we were talking about earlier.
[62:09] What would you say was somebody's -- or, like, your favorite resource when you were learning about all of this?
[62:17] I just put down a couple of them already. Yeah, yeah, and I shared those.
[62:22] There's a couple -- let's see if I have any more in my -- But, like, overall, because we were talking about, like, learning big topics,
[62:30] and I really like the one that you shared about framework for knowing what you don't know.
[62:36] Yeah. That one I'm looking forward to.
[62:39] So for that, one of the things that got me started, like, it's a tutorial, but it's, like, a good starter that I return to a lot.
[62:49] I'll see if I can find it here on Confluent Developer, and I like this because it's available in a lot of different languages.
[62:55] Nice. Yeah.
[62:59] Hold on. I just need to find language -- oh, Thunder Language Guides.
[63:03] Sorry. So this resource here, I built this out in Node and Python, and it helped me
[63:15] understand a little bit about -- because what KCAT was doing for us is you can do that, like, in code in Python or in Node.
[63:23] Oh, okay. Yeah, and that really helped me kind of see what was common to the different
[63:28] clients, what things I would always need to do when it came to, like, running Apache Kafka in an application.
[63:34] So that was really, really helpful. I should do it in Go next.
[63:39] That's what I should do. That would be fun.
[63:41] There you go. Giving you some ideas.
[63:43] Yeah. So that's definitely a resource that I enjoyed.
[63:46] One that's, like, helping me with, like, osmosis-wise and kind of understanding the different use cases for Apache Kafka across the entire huge
[63:58] tech industry is my co-worker, Chris Jenkins, has a podcast. Here's the link to the website, but it's on YouTube as well.
[64:10] It's called Streaming Audio. And guess what?
[64:13] The latest one is How to Use Python with Apache Kafka, so you might like that one.
[64:19] But that's been really, really fun because, like, the topics are, like you said, they're not, like, linear, but they're all very deep, super interesting
[64:28] conversations. I, like, turn it on, fold my laundry, and it's, like, a great time.
[64:33] So that's definitely one of my favorites as well. I know you shared a specific one, but now I'm joining.
[64:43] I was, like, oh, yeah, Ben was on the show with Chris, and Ben's one of my co-workers, so I went and grabbed that one.
[64:54] >> Awesome. >> Because that one is a really good one.
[64:57] And, yes, osmosis is -- the thing to do is what I'm realizing, and I know that there's a lot of people that we can learn from, and the Twitters.
[65:11] The Twitters is always very, very good and very fun. So definitely suggest.
[65:16] Go follow Lucia. Do you use Twitter that much?
[65:19] Are you more of a Mastodon or LinkedIn? >> I'm on all of those right today.
[65:24] I'm on data folks on Mastodon, so I'll put that into the chat, and then my Twitter is -- my Twitter username is -- it annoys me, but it's, like, slightly
[65:36] different. >> Oh, no.
[65:38] >> Yeah, it's slightly different than my other handles, because I think I, like, before I was in tech, I got onto Twitter, and then I, like, locked myself out, so
[65:47] I gave myself this handle thinking it wouldn't matter very much, and now it's, like, the bane of my existence.
[65:52] >> I get that. I get that.
[65:54] >> Yeah. And then I'm on GitHub as well, so I'll push -- I like to push up different,
[66:00] like, tutorials on there, so. And all of these links will be in YouTube as well, so don't worry if you're not
[66:10] seeing them now. They will be linked, and, yeah, I mean, I personally feel like I'm at the point
[66:17] where, like, I get it, but I don't get it, and if you try to tell me more, I'm going to be, like, I don't know.
[66:24] >> You're all -- you're learned out. >> Well, I feel like it's a lot of also, like, letting it simmer in the
[66:31] background for a while, and then learning more, which is something that I've learned is -- how do I say it?
[66:39] Laura and I talk about this a lot. Where it's, like, even if you're not going to understand it, still trying to,
[66:46] like, consume some of it to, like, a certain point. So -- and that is something that I've been working on learning, and thank you.
[66:58] Is it Henry Ortega? I want to say that's how you say your name, but I don't know.
[67:06] I'm horrible at names, so that is definitely -- feel free to hit follow on Twitter or on YouTube, wherever you're watching this, because there is going to
[67:15] be so much more data infrastructure coming out in the future. I am excited.
[67:20] >> I'm excited to follow you, and I really appreciated your feedback and questions.
[67:26] It's helped me, like, refine my approach, too, in teaching, so that's awesome.
[67:31] >> Yay. >> And, yeah, I feel like you're going to do great.
[67:35] >> Thank you. Thank you.
[67:39] You as well. And Anthony said that you've got to build something, then stuff will click
[67:43] more. Yes.
[67:47] Yes, I do. And I can't build a Kafka hello world app.
[67:51] I can build a hello beautiful human app, but not hello world. I have yet to build a hello world app.
[68:00] Everything I've renamed. Well, thank you again, everyone, and let's go find someone to read to.
[68:10] I love reading. Ian.
[68:14] We've got Ian and James. I feel like we've been talking about Ian.
[68:18] Also, James always reads me, so we're going to go to James. Thank you, everybody, for joining today, and see you again on Thursday.
[68:29] Yay. Maybe it will read.
[68:33] I don't know. It's counting down.
[68:37] Why are reads so complicated? They take forever.
[68:41] Okay, bye. And, and.

