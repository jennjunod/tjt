---
showLink: "https://www.youtube.com/watch?v=pRJv_du-0YU"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-data-modeling-and-content-creation-with-guest-leo-guinan"
title: "Teach Jenn Data Modeling and Content Creation with guest Leo Guinan"
publishDate: "2022-09-06"
coverImage: "https://i.ytimg.com/vi/pRJv_du-0YU/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode.
[00:06] I honestly don't know if these are called episode stream. >> Either works, I guess.
[00:12] >> Yeah, I don't know what to call them. Well, thanks for showing up today,
[00:16] everyone for Teach Gen Tech and welcome, Leo. >> I just did like some weird, let it.
[00:22] >> Anyway, it's a Tuesday. Yesterday was a holiday.
[00:27] Today's my Monday and I'm feeling it. Welcome to the show, Leo.
[00:31] See if I can actually talk. Please introduce yourself and what you're
[00:37] currently working on and what you're going to teach us. >> Absolutely. Yes, my name is Leo.
[00:43] I'm currently, by day, a software engineer at a startup called Copy AI.
[00:48] We do a bunch of really cool stuff with GPT and text generation. Then on the side, I've got a number of fun little projects.
[00:59] The current product I'm currently building out is, who should I unfollow to
[01:05] identify dormant Twitter accounts that you follow? >> That's cool.
[01:08] >> It is incredibly useful and it's something I built out of frustration because I follow a lot of people and I
[01:15] kept hitting the 5,000 person limit that you can follow. I'd have to go through and unfollow one at a time.
[01:23] I was like, this should be easier. I made it easier over the course of three months
[01:29] because it's never quite as easy as all of that to actually build a product.
[01:34] Yeah, it's been fun. Then I've got a Twitter CRM that I've been building out now for over a year.
[01:40] Actually, part of this is rebuilding that. Then I do a number of things.
[01:46] I've got a podcast, getting into the streaming realm. That brings us to today's topic of data models.
[01:55] One of the things I find very, very helpful in creating any system,
[02:00] whether it's a full application that I'm building or just basic automations,
[02:06] I like to identify the data I need and build out models. That helps me understand how that data moves through systems.
[02:15] Once you have a good understanding of that, the design of the systems really come into focus pretty well.
[02:24] I figured this would be a great opportunity to dig into a scheduling thing I've been working on and looking at how
[02:32] to allow people to come inbound and schedule either streams or recordings
[02:41] and how we can do some of that modeling. I think that'd be a fun topic for today, so let's do it.
[02:48] >> Yes. Really quick because you didn't mention quite a few, and I think it would be cool because you talked about
[02:55] the podcast and what you're going to be starting streaming. Please fill us in on that too because I'm like,
[03:00] there's so much knowledge drops that we got to make sure we got them all.
[03:04] >> That's the hard part. The podcast is called How to Scale Yourself.
[03:10] I'm in the second season right now. It's all just like conversations with people who
[03:16] are scaling various aspects of themselves using the Internet. Talk to several entrepreneurs,
[03:22] talk to our mutual friend Lobau, he was actually my first guest because he's awesome.
[03:29] But yeah, I see so many people doing really cool things online. Mostly, I started the podcast because I just wanted to talk to
[03:39] some of them and see what people are doing and just have conversations.
[03:43] >> I love that. >> It's actually like I'm really focused
[03:48] on having it just be raw conversations. I don't put a ton of effort into editing.
[03:55] It's really just about the conversation. Because I think one of the biggest issues right now that we
[04:00] have is all of the content that's being put out online is extremely polished because you're having to compete
[04:06] on these external qualities as opposed to the actual meat of the podcast or whatever we're doing.
[04:14] That's one of my ways to fight back against that. Then with the streaming, that's actually part of a thing I'm doing
[04:22] called Building Public University which is really all about capturing those unique essences,
[04:29] being raw and unfiltered and then building out shared media platforms that we can use to share
[04:35] people's stories and help them get to that baseline of quality so they can focus on sharing what matters.
[04:42] In this case, really their story and why they're doing what they're doing
[04:45] and the most important aspects of that as opposed to trying to compete in the realm of SEO
[04:52] and fighting the algorithm for distribution. I think we're just doing a lot of things the wrong way.
[04:58] This is my effort to start doing things the right way and actually focus on the stuff that matters.
[05:06] That's all of that in a nutshell. It is fun. I just have a lot of fun doing it.
[05:12] >> I feel like I'm going to be asking you about a ton of that stuff later on because just scalability.
[05:22] >> It's actually what I'm really good at. I'm really good at the whole scaling thing because I just
[05:27] build systems that can help me scale. That's how I manage doing a whole bunch of different things.
[05:35] I build out systems that can support that because I think that's really the most important thing that we can do because we can achieve all sorts of things,
[05:44] but we need to have those systems in place or it's really easy to burn out. >> Yeah. I mentioned that because I have the,
[05:55] oh, yeah, thank you for saying hi. You got a hello.
[06:00] >> Excellent. >> It's definitely something that I found that I'm like,
[06:07] if I just do the project itself, I have time for all of these projects,
[06:12] but it's the social media. It's the social media.
[06:16] >> Yeah. >> I say it like that because I have my podcast,
[06:19] shit you don't want to talk about. When you talk about unfiltered topics,
[06:22] I'm like, yes, yes, please. Give me more, love them.
[06:26] Then I have Teach Gen Tech, okay, cool. This one at least is somewhat easier because it's all live stream.
[06:34] I just have to make the graphics and tag people. That one is easier.
[06:38] But the Denver API Meetup, I'm like, now I have to think like someone else to be able to post up.
[06:45] Then now I'm consulting with Gravity and being able to do more of that type of content and also be myself tying them all together.
[06:57] >> Right. >> I'm like, so scalability,
[07:02] that is something that I will put a pin in it. >> Scalability, and that actually comes back to the data models
[07:07] because one of the key aspects to being able to scale is to having data models that effectively scale.
[07:14] What you'll find with a lot of just clumsily design systems, as you start to scale,
[07:20] the data models fall apart. They don't work well together.
[07:23] You end up with, as you start scaling, you have to start thinking about things like, okay,
[07:28] what happens if the same data comes in multiple times? How do we handle that?
[07:33] Figuring out how to identify the data that matters and then organize it in a way that does effectively scale,
[07:42] because otherwise you're going to be fighting the system more than it's helping you.
[07:46] That's the balance. I have been known to build systems like,
[07:52] oh, I did this thing once, I'll just build this giant system now,
[07:55] and that's not a great way to do it. But it is a good way to get experience doing it.
[07:59] It's that catch-22. >> Yeah. I would say that something
[08:06] that I realized before our stream, I get what data models are,
[08:11] but I don't get what data models are. It's very abstract, yet at the same time,
[08:16] I'm like, it's another one of those that it makes total sense, yet doesn't make any sense.
[08:21] >> Right. >> Could you define for us what a data model is?
[08:27] >> A data model, in its simplest terms, is a representation of something in the real world.
[08:41] I mean, I say real world, and actually that doesn't even need to technically be true.
[08:45] But the idea with a data model is essentially it's, so a model is a representation of something,
[08:53] and so the data model is the collection of attributes that you care about for that object.
[09:01] You could have a very simple data model that is simply like an ID to determine which one of these things.
[09:11] Like if you have a collection of marbles, okay, well, I've got 400 marbles,
[09:15] how do I identify one from the other? We'll throw a numeric ID on it.
[09:19] They're just numbered, you can count them. >> Okay.
[09:22] >> Now, obviously, that's an incredibly simple example, and not particularly useful.
[09:29] But one of the models that I think is really important, that is also very difficult is a person.
[09:41] I say this because it's really interesting to think about how different social media platforms model people,
[09:48] and more importantly, how they model those relationships. This is something I focused a lot on.
[09:55] You think of a person on Twitter, for example, since I know we're both active there.
[10:01] What does that look like? You've got their display name,
[10:07] you've got their username, you have their profile picture,
[10:14] their header image, their bio. As you start adding in these different pieces,
[10:22] you start to get this more complete picture of what this person is. One of the trickiest things with
[10:30] data modeling is if it's not in the data model, it doesn't exist. Typically, you think of a person,
[10:37] and then you start trying to associate that with a Twitter profile. The natural inclination is to
[10:44] just assume a lot of things about the person. But in terms of the system,
[10:52] if it's not there, it doesn't exist. That's the toughest part with creating these models,
[10:58] is you want to determine what needs to exist to make the system function effectively.
[11:05] It gets trickier, too, when you start thinking about how systems interact,
[11:12] because as I build out, for example, a CRM, and I've got the idea of a person,
[11:21] and I want to get some of that information from Twitter, and so there's Twitter's idea of a person,
[11:27] and then there's my data model of a person. As I'm building out these models,
[11:37] one of the things I like to look at are how do we transform a Twitter person into a Feather person?
[11:48] Feather's my CRM that I'm building. We need to figure out what parts of that model Twitter has,
[11:56] what parts I have, and then where I can get the data that I don't have yet.
[12:03] The way I view this is, if you're familiar with graphs here,
[12:10] and I'm a big fan of a concept called a directed acyclic graph, which sounds horribly complicated,
[12:17] but it's really not. >> It does, it definitely does.
[12:21] >> It does. But if you think of a graph, it's essentially just a collection of nodes and lines.
[12:31] Circles and lines connected, that's in very basic terms a graph.
[12:37] But a directed acyclic graph has two unique properties. Each connection between two nodes can go in a specific direction,
[12:49] so that's the directed part of it. So from node A to node B.
[12:54] For me, this is a lot of system A to system B. It's going from Twitter to Feather.
[13:00] We understand that that connection exists. Then the other part of it is actually acyclic,
[13:07] so there are no cycles. I don't look at it in terms of going
[13:11] from Twitter to Feather and back to Twitter. I look at it as going from Twitter to Feather,
[13:19] and then there's a different graph that would be like Feather to Twitter. What this really maps out then is
[13:24] it's a really good way of mapping the flow of data through time. I did a lot of this when I was working as a data engineer in healthcare,
[13:34] where we're getting all of these data sources in from different places. We had to combine them.
[13:39] They go through this pipeline that does various transformations, reporting, and everything.
[13:45] So the benefit of modeling it in this directed acyclic graph is you have these well-defined steps that the data goes through.
[13:56] So the first step is I get the data from Twitter. Okay, cool. Now I've got this data.
[14:03] Then the next step is I transform this data into the format that Feather is expecting.
[14:11] Then from there, it's like, okay, well, now I know that I'm missing this piece of data,
[14:17] so I can go to this external API to pull that. Then I combine that with the data.
[14:23] Then finally, I pass it on to Feather. You can see these very distinct steps,
[14:29] and it's actually a really good way to just understand how data moves through systems,
[14:35] and these different steps. So that's the flow of data.
[14:44] >> Quick question, just because something that came to mind that may make a bit of sense,
[14:51] and I'm only using these because I think they're a little bit more well-known.
[14:56] So as a comparison, a lot of people have used Salesforce,
[15:02] and a lot of people have used HubSpot. But some people use HubSpot for more marketing than for a CRM.
[15:10] Some people do it for both. So the way I'm thinking about the way you're talking about stuff
[15:16] is you were saying Twitter into Feather, then Feather goes to something else.
[15:21] But it would not be where Salesforce and HubSpot need to talk to each other and pass data back and forth.
[15:28] That would be a different data model? >> No, it can be the same.
[15:33] So you can actually pass data back and forth, but the trick is to instead of it just being a circle
[15:41] where it's happening all the time, you think of it in very specific steps.
[15:47] In actuality, the system might perform these steps very, very quickly.
[15:53] It could be in the order of milliseconds. Even as you're designing an API,
[15:57] you may go out to the system, get some information back based on that information,
[16:04] send another request and go back and forth. But in terms of modeling out the steps you have to go through,
[16:11] this is a really good way to just simplify the thinking about it. So as you're deciding what needs to happen,
[16:18] you can always combine that into steps that again happen very quickly. But you don't need to think about it from this whole perspective of,
[16:28] I've got to do all these things in a single step. So it's really all about breaking out the steps into
[16:33] individual pieces that you can understand as they flow through time. So it's really about ordering
[16:40] the steps and figuring out which steps need to happen. In data pipelines, a lot of times these are very discrete steps,
[16:53] whereas in designing an application, they may be combined together.
[16:59] But if you break them out in that way of thinking, it's just a lot easier to reason about and a lot easier to hold in your mind.
[17:07] That's one of the toughest parts of software engineering, as you start to develop these very complex data models,
[17:13] because the world is a complex place. So the more you have to hold in your mind at any one point in time, the harder it is.
[17:24] So that's why I really like to just focus in on things as fine-grained as possible in these steps. So when I break it out into these individual steps,
[17:36] I can then focus on maybe it's just a single method that I'm trying to implement, as opposed to holding the whole thing in mind.
[17:47] Because when you really do a good job of designing your data models and how that data flows,
[17:53] you shouldn't have to worry about the rest of it, because it should be very tightly controlled
[18:00] as to which part of the system you're affecting for any change. That's really the biggest part to having scalable systems,
[18:08] because it gets tougher when you might have heard like leaky abstractions, that's something that comes up.
[18:18] And so the abstraction is essentially the data model you're using. But the leaky abstraction is saying like,
[18:30] the model that you're using in kind of one specific area of the system is being exposed to other areas of the system that don't need to know about that, right?
[18:40] And so when you're kind of developing these various models, you want to make sure that essentially the part of the system that they're being used in
[18:52] are the only ones that know the inner workings of that model, because you want to be able to change it without affecting external parts, right?
[19:00] So it really comes into just being able to contain what happens in those models. And that's kind of the other aspect that I really like when it comes to these models,
[19:12] is making it to where different parts of the systems don't need to know the specifics of how that information gets to be there,
[19:24] it just needs to know that it's there or not, and probably like what format that goes into, right?
[19:30] And so this might be easier to kind of work with some realistic examples of just kind of how to model this, right?
[19:40] So one of the things I was looking at is kind of figuring out how to set up a system that I could have people, first of all, like...
[19:57] So yeah, let's talk about the goals of the system first, right? Yeah, I'm just posting these in here because these are also resources
[20:04] that individuals can use to look up more about data modeling, because the way you explain them definitely do make sense.
[20:15] These are just like other snippets saying basically the same thing, just as resources. So, but you said first steps.
[20:25] Yeah, so kind of the first steps are to define, you know, what you want a given system to do. - And so... - I'm taking notes now.
[20:36] - This should be good, hopefully. - All right, all right. So we got step one is...
[20:43] So let's see. So what I want to be able to do is I want to create a system
[20:50] that will allow people to schedule on my calendar. And so I probably want them to have a preference of either like pre-recorded or live streamed.
[21:10] Okay. And so, you know, that's not everybody is comfortable live streaming.
[21:19] It's a skill that you need to kind of develop, right? So some people might have a preference as to one or the other.
[21:29] And then, you know, from there, I want the... Ideally, it would create some sort of event,
[21:41] whether that be on Twitch or I use Riverside for kind of my streaming. So I don't know if any of this actually connects.
[21:51] I haven't looked at it yet. So this is all like just thinking out loud here.
[21:59] And let's see. So... I used to use Riverside, but it was so glitchy when I did.
[22:09] And it was like, it was about 10 months ago. - Okay. - So just like any startup, you know,
[22:18] it can scale very quickly and get help and make lots of changes. It was more of, I was just so frustrated with it crashing.
[22:28] I lost interviews, that kind of stuff, that I was like... - Oh, wow. Yeah. No, I definitely see that. - I can't do this. I can't do this.
[22:34] I've only used it for a couple of things so far. And it's worked out well for that.
[22:40] And I was actually really amazed at how nicely it streamed to both Twitter and Twitch. - Nice. - Like, I didn't even realize that you really could stream from Twitter.
[22:50] - There's like a media thing. - Yeah. It's really hard to find.
[22:56] And the fact that I can only find it through Riverside's documentation seemed a little weird. Which, considering I do a lot of work with like the Twitter APIs and everything...
[23:05] - Was it difficult to set up with Riverside? - No. Okay. Because I use StreamYard.
[23:10] And that's the only reason I knew that Twitter live streams. Yeah. Like, it's super easy to set up.
[23:15] Like, you just have to kind of, you know, connect it with kind of the... - ...streaming, what, RTMP address or whatever. - Yeah.
[23:24] And then the key. But it's like, I didn't even know that, like, Media Center for Twitter even existed.
[23:30] - Yeah. - To, like, be able to stream. Which, I feel like that would be better documented.
[23:35] - But, oh well. - It's okay. - We'll figure it out. - Yeah.
[23:39] Okay. So, let's just kind of... You know, we can kind of think here about what this model could look like, right?
[23:49] So, kind of the first steps that I like to do is I like to identify the nouns. And that's kind of the easiest way to think about it.
[23:58] So, the different objects that I care about in this system. And so, you know, starting off, I can kind of see that there's a person, right?
[24:08] So, somebody is doing the scheduling. There is going to be an event.
[24:20] - Let's see. So... - Would we need to define calendar? And also, do you think we could do it from different calendars?
[24:29] So, we could. And so, this is actually... That's a great question. And so, the one thing I would ask then is kind of like, what's a calendar?
[24:39] And I know it seems like a weird question. But the reason I ask that is because if you think of the difference between, like,
[24:50] a Google calendar and, like, you know, Microsoft calendar, Apple calendar, whatever, right? Like, they all kind of represent the same thing, but they're going to do it in different ways.
[25:01] And so, this really comes down to this, like, baseline thinking of, like, what is a calendar in terms of our system?
[25:10] So, for that, I think a calendar makes sense. And we'll call a calendar a collection of events.
[25:21] - Okay, because this is one thing that I struggle with on Calendly. And if there's an update, anybody from Calendly watching, please let me know.
[25:33] But this also piqued my interest because I have my podcast calendar, then I have my Teach Gen Tech calendar, and then I have my Gravity calendar.
[25:45] And I'm like, "Y'all, I can't keep up with all these calendars that..." I'm like, "Can we just, like, have something read to all of it, but also post to all of it?"
[25:54] But Calendly only posts one. - It does. And so, I'm trying to think because...
[26:00] - I don't know if it's possible. - My calendar actually does.
[26:04] And I'm trying to think that I think it's clockwise that, actually, if you're, like, busy on one calendar, it blocks it off in the others.
[26:17] And the only reason I know that is because we started using it for work, and then it popped up, which is handy.
[26:23] It's also kind of annoying because I get, like, two notifications every time it goes off. And it's like, "Hey, here's your actual event, and here's one that just says busy."
[26:31] - I'm not going to lie, though. If that, like, makes it so that way people don't overschedule stuff, I'm kind of...
[26:37] - That's exactly what it's good for. Because it's like, that way, anytime I have something scheduled, like, you know,
[26:44] through my personal calendar, it also blocks it off on my work calendar. And so, you know, as long as nothing, like, blows up catastrophically, you know,
[26:55] I'm able to kind of schedule things that overlap that way. - And it was called clockwise?
[27:00] - Clockwise, yeah. - All right, I'm going to be looking that up after this.
[27:03] Thank you. Look at you and your scalability.
[27:05] - Right. - That helps scaling.
[27:07] - It does. And that's actually a great point.
[27:11] Like, as you start integrating different things in, like, you start running into these kind of different collisions, right?
[27:18] And then it becomes a problem of, like, well, how do I manage all of these? Which is, you know, when you have kind of these data models and understanding, like,
[27:26] the actual ways that kind of these different products can interact, you know, you can see it gets pretty complicated pretty quickly, which is why it's important to kind of simplify
[27:37] as much as possible. - When we have a chance, and yes, I'm being rude and looking on my phone.
[27:43] I'm curious if this would be considered a data model, because I almost feel like I may have gotten stuck on earlier this weekend trying to create a data model in, like, how I'm going
[28:02] to be posting stuff or how I'm going to, like, figure out scheduling, because it's, like, it's so confusing for me.
[28:09] And I mention this because I can see how data models are considered only, could only be considered for tech, yet I think it's, like, really data models are this visualization
[28:22] that we need for so many other topics or things in life. - Everything.
[28:28] Because it's a simplification, right? And that's kind of what it comes down to, being able to identify the parts that you
[28:35] care about. And yeah, this is exactly it.
[28:39] So it's... - Oh, too big, too big.
[28:43] So basically what I was doing, just to try to get it so people can get a visualization, is I need to post content.
[28:51] We talked about this earlier. I have not enough time.
[28:55] Like, I have a content scheduler. That's not my problem.
[28:58] It is literally visualizing what I need to create and how I'm going to create it. And for the most part, like, Teach Gen Tech, cool, that one was pretty figured out.
[29:10] That's the one in green. Gravity, cool.
[29:13] I can Google some stuff, figure it out, ask the team, post some stuff. API Meetup, easy enough.
[29:19] That one's easy peasy. And like, I posted this black graph is just like, okay, what platforms that I'm posting
[29:29] them on. What I was really stuck on, and I'm currently not doing yet, is after I record an episode,
[29:37] what do I do with the podcast? Because live streaming's pretty easy, but I'm so stuck on how to create that data model
[29:47] on the podcast. What do I do?
[29:49] How do I visualize this? How do I think through this?
[29:53] Because I'm going, I don't know how to go to A to Z because it's too much for me. And I don't know if this is how you've ever started a data model or this is how a data
[30:06] model could be started. I am curious, like, do you have any visualizations like this that you've used before?
[30:16] So a lot of times that this is exactly how data models come out, because it's like, okay, I'm trying to figure out how to solve this kind of like complicated problem, right?
[30:26] And there's a lot going on here. And so, and like, that's the reality of life right now.
[30:33] And so I think this, I actually really like the fact that you brought up that this isn't like just a tech problem.
[30:39] Because one of the things that we realize is that tech is actually touching all aspects of our life now, right?
[30:46] And there's apps that like help us manage everything. And that just means we have a million apps that all like, never talk to each other, and
[30:56] they're all a pain. And so I think one of the things we do need to get to is more individualized systems and
[31:05] being able to kind of create our own things. And like Notion is actually a great way to do some of that, right?
[31:11] Because you can create a database, you can build automations off of that. And so in terms of looking at something like that, you know, so I would say like, okay,
[31:23] so, you know, I can bring it back up. I didn't know if you want to still talk about it.
[31:26] Yeah, we can. And so, okay, so we've got some different things there, right?
[31:36] So this is probably the one that was the most complicated was the podcast stuff. Yeah.
[31:43] And so I think that would be a good thing to model, right? And so, you know, a couple of the nouns that jump out.
[31:50] So we've got the podcast, right? And again, this seems simple, because we're only going to talk about like, this specific
[31:57] podcast. But the nice thing is, like, once you solve a problem for like, one thing of yours, if
[32:04] you kind of think about how you solve it, you can see how like, oh, well, I could actually do this to support multiple podcasts, or all of that.
[32:12] So I tend to think of it in like, fairly general terms, even if it's like for a specific instance, just because I do like to constantly have like product ideas.
[32:21] And I've got a million product ideas, probably way too many that are all planned out. And I've bought domains for half of them.
[32:27] But that's another. That's another problem.
[32:30] That's actually a big reason why once I, you and I talked about that we're like, yeah, data models.
[32:36] I'm like, I don't know what that is. So yesterday, Anthony has been one of my mentors.
[32:43] He's AJCDev, I think, on Twitter, I'll have to actually look it up. And he, he was like, yeah, you should watch these videos before you do data modeling.
[32:59] And it wasn't until we started talking about the calendar that you were talking about that I'm like, oh, wait, this is literally what I'm struggling with this last weekend, trying
[33:08] to figure out and I'm like, mind blown. And just how we literally do this out.
[33:15] Because none of this is technically like the tech side of things. I'm not trying to connect an API right now for a data model.
[33:22] I'm literally just trying to figure out the process I'm supposed to do stuff. Well, and that's kind of the cool thing.
[33:27] Because a lot of times I build out these, you know, these DAGs, right? And you think about that in terms of like actually moving data through a system.
[33:36] But it's really like just thinking about the steps I take when I do things manually. And then I look for where can I automate because I don't have to automate all the steps in
[33:46] the process. If I can figure out what the time consuming parts are that I don't like to do, and just
[33:53] how to automate those, then I've gained a lot, right? And so we don't actually have to build out these super complex systems.
[34:01] But just mapping out kind of how different things like fit together, you start to see like, oh, well, this piece, I do the same thing every time.
[34:10] So this would be a good thing I could learn how to automate, right? And so, you know, a lot of times we think like, oh, this is just a complicated process.
[34:20] Like, you know, it's just going to take all of this time forever. When in reality, we could spend, you know, a couple hours probably learning how to automate
[34:28] some like specific piece of it that then saves us, you know, three to five hours a week or a month even.
[34:35] And, you know, it pays for itself over time. And then as you develop these like little like pieces, you start to connect them into
[34:42] more complex systems, right? So when you build out like a tiny system that does one thing well, then that is a node that
[34:50] you can add into a bigger system down the line. And that's really how all systems are developed, right?
[34:56] Like you start off with like, you know, the kind of the MVP, right? Something that does like one thing, and it does it every time you do it, right?
[35:03] And it's repeatable. Because once you have things that are repeatable, then it's like, you can move them around,
[35:10] you can do things in different orders. You can, you know, do things like, you know, kind of build ones published multiple times,
[35:17] right? Like if you have like different places, you want to go with it.
[35:20] And so that's really how things can start scaling. But in terms of this, we can, so, you know, we kind of got the podcast, right?
[35:29] And so the podcast, if we look at like kind of specific attributes, right? So the podcast has like a name and a URL.
[35:38] And then so, and then the podcast has episodes, right? So the episodes are going to have, you know, probably like a title, a guest, maybe more
[35:51] than one guest. So that's something we want to think about.
[35:53] Like when you think about what is contained kind of within that noun, and the different attributes it has, you want to kind of determine like, is this something it only has one of,
[36:03] or is it going to have, you know, more than one? And so, you know, for guests, I'd say, you know, okay, we'll probably want to leave it
[36:12] open that it could potentially be more than one guest, right? And so again, you're going to have a URL that'll go to that specific episode.
[36:22] And, you know, it'll have like a duration of some sort. So it'll be, you know, some amount of time, which may or may not be important, but just
[36:34] kind of as we're thinking about it, you know, that could potentially be important. - Would we put description?
[36:42] - Description would be good, right? And that's actually what I tend to struggle with, with my podcast, because I'm like, oh,
[36:50] I've got the episode back, like, and you know, it's edited, and now I've got to post it. But if I post it, I have to write the description, which means now I've got to think about what
[36:58] I want to write in the description. - Yes, yes, yes, yes.
[37:01] - That's something that I'm still trying to solve. But yeah, the description's good.
[37:06] - That's something that's like, and I was trying to think of it, like you're thinking a lot of like pre stuff.
[37:15] And I will say Monday, I was using Monday before I was using Notion. And they did help quite a bit in automations, which was really helpful.
[37:27] Like if a guest submitted, then it could like send them an email to set up their calendar. So all I had to do was like move in one area instead of sending every single email, which
[37:39] that automation was great. Yet it was way too expensive.
[37:45] And they only had a minimum of three users, blah, blah, blah. - Yeah, that's where it gets to be a problem is like, it does get like a lot of the systems
[37:53] that are built for some of this like automation stuff, they're geared towards larger companies that have a budget for it.
[38:01] - That was gonna be my next question. - One of the things that I really try to do is figure out how to do things as cheaply
[38:09] as possible. Because I believe that like more creators, especially starting out are the ones that
[38:17] need the most help when it comes to automation and kind of creating these sustainable processes, right?
[38:22] Because yeah, it gets to be a ton. And then it's like, okay, well, great.
[38:28] Like eventually, like if you stick to it long enough, you'll have like a big audience, you'll be monetized, you'll be able to afford to like pay people to like manage different aspects
[38:38] of this. But what do you do until you get there, right?
[38:41] And so that's really where automation can come in handy. And just kind of going through this process of like figuring out which pieces you need
[38:54] to kind of automate or which would be the best way to do it, that gives you a way to kind of find the cheapest possible option.
[39:00] Because a lot of times you can do a lot of this for free or very cheap. Actually, there is a service, because you know, like a lot of people like Zapier.
[39:10] - I was just thinking about Zapier, that's funny. - Yeah, and so that's what a lot of people use for automation, but it gets expensive.
[39:17] And so that's one I actually don't pay for, because I think it's a little overpriced. It works well, and it's simple.
[39:28] But the one that I like is actually, and I haven't used it as much as I would like, and I need to play around with it more.
[39:40] But it's cool because I can self-host an instance of it. So I dropped it in the private chat.
[39:47] I don't seem to have. - Oh, yeah, yeah.
[39:48] - So if you want to share that. - I'll share it, thank you.
[39:51] - Yeah, and I don't know how it's actually like pronounced, but it does a lot of the same thing that Zapier does.
[40:00] And it's, excuse me, it's open source. You're able to self-host it for free.
[40:09] And so if it's only you using something and just running it as a Docker image on your own system, that's something pretty straightforward.
[40:19] And maybe not for everybody. Like I say, this is someone who's been in tech for a decade now or so.
[40:24] So I'm like, "Oh, yeah, just put it on a Docker image." - And I think that's also something to call out of like, I think like some of these things,
[40:37] I'm like, "Okay, cool." Like, especially I've been around tech for quite some time before I started teaching
[40:46] on tech. And I was like, "Cool, like I know about Monday, so I'll use Monday."
[40:50] I know I need to automate some of these things, but I don't know necessarily what I can and can't automate.
[40:57] So I love that we're going through this practice because I think that's something that I talk about this on my neurodiversity, mental health airspace that I host is that it just doesn't
[41:12] always connect the same way that it does for everyone. And I love that you're breaking it down and also like, "Hey, let's go through the nouns
[41:22] first to figure this out. And what can we automate?"
[41:24] Because these are things that I'm just like, also, I had no idea how amazing this episode would be because like, you're cool and everything.
[41:33] But I was like, "I haven't met you much yet. I don't know what data models are."
[41:37] And I'm like, "You're finally piecing it together." - That's the thing.
[41:41] And like, I'm always torn because it's like, so I did, I taught a cohort-based course called Supercharge Your Time.
[41:49] And I've only done, I did one cohort of it last year. And it's like talking about the theory and the DAGs and everything are cool.
[42:01] And I'm really fascinated by kind of that aspect of it. But in reality, actually doing it is the best way to kind of think about it.
[42:08] Because you don't quite realize, but you really have created a DAG in this little graph here. - What does DAG stand for again?
[42:17] - So it's a directed acyclic graph. - Okay.
[42:21] - And so I've got the, I can drop the Wikipedia in the thing. But again, it's really like, it's just a very basic model, but it's really about steps moving
[42:36] through time. And that's really all it is.
[42:38] But it's just a really powerful mental concept because then each of these steps here can actually then be broken down into a sub DAG.
[42:52] And so if you think each of these steps is kind of a simple representation, but there's more to it, right?
[43:04] So even listening to the episode, you can break down into the steps of load the episode in the browser or whatever you're using and branching off, take notes based on whatever.
[43:21] And so you can kind of get into these various different pieces. And so there's just a lot of really cool math things that come into these directed acyclic
[43:30] graphs and things that you can count on. And so when companies do a lot of like big data stuff and a lot of like processing just
[43:43] astronomical amounts of data, these DAGs are good ways to ensure that various things are true about how that data moves through.
[43:56] And so it's just... - It's interesting.
[43:59] This is fascinating. Not something I'm good at whatsoever.
[44:03] I'm like, you want me to talk to somebody? I got you.
[44:06] I will, like, I got that. You want me to get on stage?
[44:09] Again, I got you. But it's like this data stuff.
[44:13] I was seriously so stuck until my partner helped me write this out this weekend, asking me questions.
[44:21] And I'm like, oh, I forgot this, this, and this. And even now I'm like looking at it and I'm like, I don't know what I can automate.
[44:28] So I just love that you talk about how important it is to like not just hear it in theory. Because the tangible is so important.
[44:40] - Right, it is. And, you know, I think like people can probably go their entire life without hearing the word
[44:49] DAG, unless they know me. And then they'll probably hear it more than once.
[44:52] But, you know, it's one of those, like, that's not really necessary. But it is good to, like, follow up if that's something that you're interested in learning.
[45:02] And, you know, especially if you want to ever get into, like, data engineering or kind of how those data pipelines are built.
[45:08] It's a super fundamental concept that is, you know, probably going to come up in, like, interviews and things, I would assume.
[45:15] So that's kind of good from that aspect of it. But yeah, so kind of getting back, I guess, into the model here.
[45:26] So, you know, we kind of talked about episodes last. And then kind of I see the clips, right?
[45:33] And so, you know, if we think about the noun of clip, so that's actually going to be, it's going to have a direct relationship.
[45:43] So it's part of a specific episode, right? - Yeah, like, what am I going to put on TikTok as a video clip?
[45:50] - Right, and so that clip is going to be tied to a specific episode. So that's kind of, again, where we were looking at, like, is this going to be one or many?
[45:59] So for a clip, it's going to be related to a single episode. Most likely, unless you do a compilation.
[46:08] But a clip is a specific episode. - Yeah, it's going to be one.
[46:11] - And so that's kind of where it's like, okay, well, is this true? And that's--
[46:16] - Yes, it may be true in the future. That's a great point, actually.
[46:20] When we're building these, because this is another thing that I think I get stuck on, is I'm like, but what about this?
[46:28] Like, kind of like, is that going to be clips from multiple episodes? And then also, like, do I worry about that?
[46:35] Which may make me take a few steps back because that is going to complicate things. Or do I do, like, okay, like, yeah, maybe one day.
[46:45] But right now, I just need to make my dag on what I'm doing right now, because I haven't posted on social for two months.
[46:52] And I should probably start doing that. - That's the thing.
[46:56] Like, it's good to think about how it might evolve. But also, it's more important to know exactly how it is now.
[47:07] And this is something, too, that actually comes up in software engineering as you're, like, doing product requirements.
[47:14] Because most people don't think about things in kind of these types of situations. And so, you know, if you are, like, in a job interview or something,
[47:24] and somebody asks, you know, or says, like, okay, well, here's the requirement. These are good things to ask about.
[47:31] Because a lot of times, and I've had this experience where it's like, oh, well, you know, this particular record will have, you know, this type of value.
[47:42] And you're like, okay, well, is that ever empty? Well, no, it's never empty.
[47:46] And then you, like, come to find out, like, well, I mean, it's pretty much never empty. Like, but, like, maybe sometimes I guess it could be empty.
[47:54] Like, those are very different things, right? Like, so, really, anytime you're looking at, like, words like always or never,
[48:03] those are good places to, like, dig in and be like, are we sure about that? Like, are we actually sure that that's always going to be the case?
[48:11] Or that's never going to be the case? Because that's almost never true.
[48:16] And so, it's, you know, that's a good place to think. But in terms of, like, this, yeah, it's like, okay, so, what I would say is, like,
[48:26] okay, so, we'll say clip is tied to a specific episode. And then potentially, we could have, like, a compilation,
[48:32] which is a collection of clips, right? And so, that would be a good way to kind of branch that out.
[48:38] And so, you know, the clip is also going to have, like, a duration. It'll have some sort of location, whether it be, like,
[48:48] either a URL or just, like, a local file system location, right? And so, okay, that's probably pretty good for that.
[48:59] And then, so, the export is interesting. So, you know.
[49:04] - And that is supposed to be descript. Description is descript.
[49:09] Yeah, because I was like, I ran out of room. - No, I got it.
[49:13] - It was cool. - Okay.
[49:15] - Export takes forever. Because I'm exporting the videos after I edit them.
[49:20] So, that's why I'm like, I need to start really registering that export is going to take me forever.
[49:27] - Right. And so, like, that's something that you could always look at.
[49:34] Either automating or batching. Batching is kind of another good way.
[49:37] So, a good, like, as you're kind of going through this, that's another thing you can kind of identify.
[49:45] Like, oh, if I can't automate it, I could batch it to where, like, okay, well, now I've got all of these things edited or whatever.
[49:52] And instead of just trying to, like, you know, export one of them as I go through the process, well, now I can actually just export
[49:58] a whole bunch of these clips or whatever, right? And so, you know, export is a verb there.
[50:07] So, a verb is a good time to look at, like, okay, well, that's kind of the arrows in the DAG, right?
[50:14] - Right. - And so, if, you know, you kind of think about, like, the nodes,
[50:19] the circles in the graph as nouns, the arrows are the verbs. And so, that's something that would potentially be good.
[50:29] And so, you could even, like, one of the things that I like to do as well, you're like, because what, you know, the tricky thing is, like,
[50:42] anytime you're getting into, like, automation, like, automation is great as long as it works, but then what happens if it doesn't?
[50:48] And so, you know, one thing to kind of keep in mind is, like, okay, how easy is it to recover from failure?
[50:58] And so, the first thing you've got to think about is, like, am I going to know that it failed?
[51:03] And so, as I, like, do actions, so, in this case, like, as I'm exporting, if I did have that automated, like, I would probably either have some sort of, like,
[51:15] record created or some sort of notification that just said, like, hey, this happened. So, that if it didn't come through, I would at least know that, like,
[51:27] something's broken, and I've got to go look. And, you know, that's something, like, Zapier's pretty good about,
[51:33] because that's kind of their, you know, business model. But if you are building stuff out yourself, that's something you want to pay attention to,
[51:43] because otherwise, you'll get down the road and be like, oh, this thing that I thought was running for the last three months never actually ran.
[51:50] - That actually happened with my automations with Monday. I wouldn't know that people aren't getting the email.
[51:57] - Right. - Because, like, I mean, they were my fault.
[52:02] It wasn't, like, it was Monday's fault in the fact that, like, I needed to change my Gmail password that I didn't get a notification to update my password.
[52:11] So, the connection lost, and nobody was getting my emails. - Right.
[52:16] And so, that's, you know, something to kind of keep in mind as you're going through. Just, like, are there notifications in place that either, like,
[52:23] it's notifying me that it happened so that I know if I don't get a notification, it didn't happen or at least needs checked?
[52:30] Or am I notifying in case of an error? You know, just some way to kind of be aware.
[52:38] And then, let's see. So, we've got kind of the description here.
[52:44] And we mentioned that in the, you know, kind of tied into the episode. But if we wanted to make that its own, does that, is that topics?
[52:54] I can't quite see what that is beneath description there. - Graphics.
[52:58] - Oh, graphics. Okay.
[52:59] - Yeah, like, I'll need the description to make the graphics. - Okay.
[53:03] - I think that's where my, I don't know where that, or I need, it could be that I need descriptions for the clips.
[53:12] And then, after I edit them, I need to make the description and the graphics. I'm not 100% sure, but I'm pretty sure that's where my mind is at.
[53:20] - Okay. Yeah.
[53:22] I mean, so that's something to kind of keep in mind too, right? So, you know, a graphic is another potential noun there.
[53:30] And so, one of the things that kind of, I think, might matter there is the destination. So, like, where is this graphic intended for?
[53:38] Because that might inform the size, right? You know, that's something that.
[53:42] - Exactly. - It is kind of ridiculous.
[53:46] Like, you start talking through this and you're like, this is actually really complicated, isn't it?
[53:49] - It is, and people are like, like, when they think about content creation. So, y'all, I get, like, I'm surprised.
[53:57] I don't, we actually don't have very many people here today, but I'm just like, yay, I get to ask all my questions.
[54:03] But, like, content creation is freakishly complicated. Like, having to go through all of these steps.
[54:10] And, like, there's, I've been seeing quite a few, what, like, articles and stuff about,
[54:21] oh, you don't need to make new content. Use one piece of content 10 ways.
[54:24] And I'm like, yeah, okay. I still have to go through all of this.
[54:28] - That's still time. - To do that.
[54:29] - Yeah, oh God, yes. - Yeah.
[54:31] - And actually, one of my famous things is like, oh, I'll just go, like, go back and do all those other steps later.
[54:38] I never do, but. - That is true.
[54:40] I was, this was the one goal this weekend. It just didn't happen.
[54:45] Because for me, it's like so overwhelming that I'm like, but the podcast is so important to me that I'm like, cool.
[54:52] I need to figure out how to make this work. But I love that we're talking about it now
[54:57] because this isn't just me. This isn't just a me issue, you know?
[55:01] Like, this is something that people really struggle with conceptualizing and doing.
[55:06] - Right, and, you know, I think it is, I think it's the reason that a lot of the content
[55:11] is ending up to be very much the same as well, right? Because the, one of the easiest ways
[55:19] to kind of streamline this is to have, you know, so-called best practices or like templates, right?
[55:26] And so we do tend to look for like the shortcuts that we have in terms of like, okay,
[55:33] well, if I just follow this pattern, that'll be good enough.
[55:38] And so the problem is when everybody's doing that over and over, we get this kind of convergence
[55:44] on the same type of content because we're following the best practices
[55:47] that algorithms are rewarding. And like on YouTube, for example, that's a good one.
[55:52] If you look at like the top YouTube creators, all of their videos follow like very similar formats
[55:57] because that's what performs well according to the algorithm.
[56:00] And so there's a lot of work that goes into kind of feeding the algorithm, if you will.
[56:06] And like Mr. Beast did a whole bunch, like I saw him talking about the fact
[56:10] that he spent a ton of time like figuring out exactly what the algorithm rewarded and like doubling down
[56:16] on that content creation. And so it's like, you know, people see it.
[56:18] Oh, you gotta be a YouTuber. Like you just make videos.
[56:21] Like, no, it's actually way more than that. And there's research that goes into it.
[56:25] And in terms of like all of that, and that's what I think we need to kind of get away from,
[56:31] which I think people being able to build these kinds of systems themselves
[56:36] to make the annoying stuff sustainable so they can focus on like the creative aspects of it,
[56:42] I think is gonna like be really beneficial in the long run because it's, you know, that's kind of a part
[56:50] that matters, right? Like it's not the, you know, the thumbnail
[56:54] with like the surprised face, like pointing to the description or whatever.
[56:57] I don't watch that. - Yeah, it's definitely something
[56:59] that I also wanna like point out is like edit. I know how to edit because I interned somewhere.
[57:08] It's not my favorite thing. Definitely not something that I love to do,
[57:11] but I know, okay, cool. This is my intro.
[57:14] I already have that done. This is my outro.
[57:16] I have that done. I just need to make sure the audio is good and export,
[57:19] you know, but there's a lot that goes into the steps of editing.
[57:24] And like, we could be breaking that down even more. I don't want to, but like, that's when people talk
[57:31] about getting into content creation now, I'm like, do it. Just know that it is a process, it is a process.
[57:37] - And that's exactly it. And it's one of those, you don't really,
[57:42] like I've done all sorts of things and I figured out what I like and what I don't like.
[57:46] And like the podcast now that I've got is like actually my third attempt at a podcast.
[57:51] So the first one, there was like one episode published on YouTube.
[57:55] The second one, I recorded a couple of interviews that never actually got published
[57:59] because of the editing part, right? And so now I actually just have Lobo out of my podcast.
[58:05] He's like, I'll let him for you. He's like, just send them to me and I'll send them back.
[58:09] And you know, it's not, again, like I don't, it doesn't need to be like super edited.
[58:14] All it needs is like, just go through and like probably like chop off the junket,
[58:18] like the beginning and the end. And it's all about the conversation.
[58:21] So like, I don't have like an intro or an outro because that's, I don't want to complicate it.
[58:26] And I just wanted it to get to the point where I could easily, I could publish it
[58:31] as easily as possible. And so I think as new creators, that is the thing to get to.
[58:39] And like Lobo always laughs at me because I'm like, he'll like ask me for advice.
[58:44] And I'm like, just publish it. Like, just post it, just post it.
[58:47] Because that is the, that's the hardest thing to get over. Like, you know, even like, you know,
[58:51] he's decently established at this point, but he's like, you know, oh, do I do this?
[58:55] Do I do that? And like, just post it.
[58:57] Like, you know, if you have a hunch, go for it. Maybe it's right.
[59:01] Maybe it's wrong. But the hardest part of content creation
[59:06] is putting yourself out there. And like, it's really easy to pursue perfection
[59:10] and like have the perfect process to get there. But the most important thing is really like,
[59:17] just putting yourself out there some way because it's an iterative process, right?
[59:22] Like it gets better over time. This process develops over time.
[59:26] As you do things over and over, you start to see things that you're repeating, right?
[59:31] And on that point, and that's such a great point is, so for example, and I want to say that about Teach Gen Tech,
[59:40] I actually just posted an article yesterday about this, is I failed my way into becoming a develop-cado
[59:47] is what I'm calling myself because devrels are avocados.
[59:50] Like it's, y'all, it's a thing. My other article will show you why it's a thing.
[59:56] But failing my way to devacado, like I failed so many times.
[60:02] Teach Gen Tech is my third show. So greater than podcast, it did survive,
[60:10] but we had an intern that did the audio and I met him at a coffee shop.
[60:15] Like it was so random. And this was back in like 2016.
[60:20] And then my second show is, shit you don't want to talk about.
[60:24] It is still out there, yet this is the stuff I'm struggling with.
[60:28] What we're going through right now is where I'm like,
[60:30] I don't know if I can keep the podcast because it's like, this is,
[60:36] it's not going to be organic. Where like Teach Gen Tech is very, very organic
[60:42] because people are interested in learning tech. Like it's easier.
[60:46] It's a lot easier to talk about. It's a lot easier to comprehend.
[60:50] It's a lot easier than mental health and all that shit. So it's like, how do we really work
[60:59] on making it accessible when we don't know what we don't know yet?
[61:06] - And that's, you know, I think the... So I kind of realized,
[61:16] the one thing I didn't actually talk about is I'm also writing a book now.
[61:18] - Oh, yay. - And so this came out like last,
[61:22] or I say came out like the idea, I decided to just like announce it last week and do it.
[61:27] And it's called "The Hitchhiker's Guide to the Future." - Oh, I like it.
[61:32] - Because it's, you know, kind of the playoff of "Hitchhiker's Guide to the Galaxy,"
[61:35] which is one of my favorite books of all time. But also one of the things that I'm fascinated with
[61:42] is kind of the evolution of technology and where it's going.
[61:45] And I do think the future is going to look drastically different
[61:52] based, you know, in terms of like future of work, future of education, all of that,
[61:56] because of a number of different factors. But essentially, you know,
[62:03] the skills that are really going to be valuable in the future are not necessarily what people think they are today.
[62:11] And, you know, I think learning tech, you know, a lot of people get into tech
[62:18] because it pays better, right? And I do think that that's going to be
[62:24] not as true in the future as it currently is. I think tech roles are overvalued right now.
[62:31] And as an engineer, like I'm probably pissing off a lot of engineers
[62:35] who are like by saying that. But the reality is like engineers are paid well
[62:43] because of the fact that we have to learn constantly, right? Everything is constantly evolving rapidly
[62:51] and we need to kind of keep up on latest trends. You know, I've used different programming languages
[62:57] throughout my career, different frameworks, and it's still hard to pick up at times,
[63:02] like, you know, because everything is just like, it's evolving so fast.
[63:06] - Right. - But the thing that people don't realize
[63:10] is that's not just true for engineers. You know, you look at like product managers
[63:16] and designers and all of these other roles, software is evolving there too.
[63:21] And companies aren't great at rewarding efficiency right now.
[63:28] And so they actually tend to punish efficiency, which is a whole nother thing.
[63:32] But it's going to result in a lot of people like burning out and just deciding to do their own thing.
[63:38] And I think one of the things that's super cool about where the future is going
[63:45] is even if you end up not in tech, just understanding how tech works
[63:51] and doing things like thinking through this to create like basic automations with Notion, right?
[63:56] And kind of figuring out these steps, that's going to be incredibly valuable
[64:00] because then, you know, you don't need to build the next app
[64:03] that gets a billion downloads. If you can build a small system
[64:08] that saves 10, 15 hours a week based on your daily job
[64:14] and like opens up that time to do things that you care about,
[64:17] like that's going to be what changes your life, right? Because, and then, you know,
[64:22] you start thinking about how you can, you know, start like outsourcing your systems to some extent
[64:30] and being able to like give people the blueprints. And you kind of see that now
[64:35] with people selling like Notion templates and things like that.
[64:39] But just understanding kind of where the future is going, a lot of what I'm playing around with in this book
[64:45] is like, okay, well, here's kind of, I'm breaking it down to like,
[64:49] here's the past technology that kind of like was started.
[64:54] And then I'm going to be doing a bit with like, here's where we're currently at.
[64:58] And then finishing it up with like, and here's kind of where things are headed
[65:03] and why I'm seeing these trends. And it's going to be like,
[65:06] it can be overwhelming because there's so many options,
[65:09] but the real key is like finding out what works the best for you.
[65:13] And like just rolling with that, like you don't actually need
[65:15] to pay attention to everything. - Right.
[65:17] - You need to find what works and then just go with it. Find what you enjoy
[65:21] because that's really going to be what's sustainable in the long run.
[65:25] And then, you know, you build out these systems and then you kind of just like do your own thing.
[65:30] And, you know, you kind of have that level of freedom that people are really struggling with right now
[65:35] 'cause they're just getting worked and, you know, harder and harder.
[65:37] And it's, you get quiet quitting, which no, they're just underpaid
[65:43] because they're forced to learn at the same rate as engineers
[65:46] and they're not getting paid the same. - Yes.
[65:48] Something you mentioned though is about trying things on and seeing if they fit.
[65:53] It kind of is a way of paraphrasing it. And that's something we talk about with mental health
[65:59] so often because tools and techniques that help me may not help the next person and vice versa.
[66:05] Like there's some really cool tools out there that I'm just like don't work for me whatsoever.
[66:10] And again, it's like creating this data model and like things of, okay, cool.
[66:16] I feel like people may interchangeably use like creating mental or like data models to,
[66:27] oh, I also have that in my toolbox. When in reality, we're creating data models about that too.
[66:33] - Right, we totally are. And it's like, we represent everything
[66:38] kind of in our minds with these data models. We don't call them data models.
[66:41] Sometimes they're called mental models. A lot of times they just like the noun
[66:46] that we have in our head and there's some abstract model behind that, right?
[66:50] And so it's not defined. And so creating like these data models
[66:55] is really the process of like defining this. And it is really powerful when you start to go through
[66:59] and like actually try to define the things that you're thinking about
[67:02] as opposed to just like this abstract word because people define things very, very differently.
[67:08] And so one of the things that I've learned is really not to assume that two people
[67:16] mean the same thing with the same word because they're almost never exactly the same.
[67:21] - It's so true. - And so the kind of cool thing about a data model
[67:25] is it's like in that kind of API contract, it's like, here's the data model
[67:30] and this is exactly what it is. And if you wanna talk to me,
[67:33] like here's the model you need to understand that this is using.
[67:38] And so it is really good to think about things in that concrete of terms
[67:42] because it is very different from the way we usually interact.
[67:48] And when you start to realize that people's models are different
[67:51] and that's why they can't connect on certain things, we really start to think about it and like,
[68:01] okay, well, how can we get from like one model to the other? And that's kind of where in like data,
[68:08] it's like data transformations. And like I talked about,
[68:11] going from like Twitter to Feather, we have kind of the same idea of things,
[68:15] but those are actually like different representations. So how do we make one turn into the other?
[68:20] And so that's the idea of like transformation of data. And I think it's actually really handy
[68:25] in like talking with other people too. And like you start to realize like,
[68:28] oh, we need to like get more understanding as to like what we actually mean
[68:32] when we use these words. So those are really good skills to have.
[68:36] - I was just about to say, I think, and I took down the share screen
[68:41] because I think something that would be really cool is to have you on the show again for a second,
[68:47] but to like take something like this. This is a little easier for me to conceptualize
[68:54] 'cause it's where I'm stuck on instead of like your product.
[68:58] I was totally down for your project till I was like, oh wait,
[69:01] I'm actually working on that myself and it's not clicking.
[69:03] Damn. - No, see that's great because it is like,
[69:07] you know, as I said, this was a kind of a new like, okay, I'm trying to figure this out.
[69:11] And it actually comes into the whole book writing process too because I wanna like create some like inbound interviews
[69:19] and things like that. And then actually gamify it a bit.
[69:21] - That'd be cool. - That's another, like I'm having fun with it.
[69:25] - Well, what I'm wondering if we can do next time is, so I have this like out, this photo, it's done.
[69:37] You know, I've created the best I could come up with. And I think it would be cool
[69:41] if we can do it on like a mirror board or something because I'm pretty sure my notes
[69:47] don't look anything like your notes. In the fact of like, you know how to make these gags
[69:52] and I'm just like trying to keep up and those types of things
[69:55] that I think it would be really cool to take and really showcase how we may go from like an info dump
[70:02] of here's all the steps I have to do to then where do I go with this?
[70:08] Because I don't know what I necessarily could automate what like I have a template for graphics
[70:15] but I still need to export those. I still need to add any audiograms.
[70:20] I still need to like, I think it would be really, really cool
[70:24] to showcase how you go from one to another in a technical standpoint
[70:30] but then also just for people that don't naturally know how to go from A to Z
[70:37] because that's a hundred percent me. I'm like--
[70:39] - It's not a natural thing because again, like we're taught to kind of,
[70:44] you know, create these abstract models. And, you know, we figure out the process along the way
[70:50] but we typically don't do a ton of like thinking about the process.
[70:54] And that's something that like actually going through the exercise
[70:58] of modeling these things really helps you do because it takes practice.
[71:03] And it's, I don't think there are very many people who can just kind of do it naturally.
[71:06] But as you do it, you gain experience. You start to, usually you start using them
[71:14] and then realize what you're missing. And then, so in the future, you're like,
[71:18] this is what I always miss because it's something that like
[71:21] doesn't come to mind right away. And so, yeah, experience is absolutely valuable there.
[71:28] So I'd be happy to kind of come again and we can walk through the actual process of it
[71:34] and start outlining exactly like how to do it. And, you know, potentially even like automate some of it
[71:40] just to see like what's possible. - That'd be dope too because this is a kerfuffle,
[71:47] a hot mess of, I don't know, I can do it. But it's an organization that I think,
[71:54] that's what I always refer to it as is I just need to figure out how to organize it.
[71:59] But I don't think it was necessarily organizing. It was the data model, which is kind of organizing.
[72:06] - It is, it's breaking it down into like, you know, very concrete representations of what's happening.
[72:13] And that's essentially if you can kind of figure out how to like represent it,
[72:19] the actual process of automating, it becomes a lot easier.
[72:22] And that's kind of, you know, when I was talking in the beginning
[72:25] about creating these scalable systems that work, like if you define it well, it becomes easy.
[72:33] And that's really what you should be looking for. And if something is hard,
[72:37] you probably don't have it defined well because a well-defined data model,
[72:43] when you really want to like automate something, ideally you have it down to a Google search
[72:48] that you can like type in, and it's like, here's a step-by-step process
[72:51] of how to do this thing you just searched for. And so that's kind of the end goal
[72:57] that we're trying to get it to, right? We want it to be simple enough to Google search
[73:01] for how to automate this, and it'll just pop up. And then, you know, obviously with some things
[73:07] that's not quite reality, but it's true for more than you would imagine.
[73:13] - What up, homie? And I, we went through so much today.
[73:20] Homie, how long have you been hanging out with us? Were you here the entire time?
[73:24] 'Cause if so, like my brain kind of hurts, but I'm really excited for like Leo coming back on the show
[73:31] 'cause this is, it's definitely something that, oh, sorry, I just like glanced over at my notes
[73:40] and I'm like, what's TT video clips? TikTok, TikTok, TikTok video clips.
[73:46] I think it's definitely something that breaking it down and seeing would be so good.
[73:56] Oh, you've been lurking. I agree, we need to have Leo back.
[74:03] Leo, you are amazing. And thank you again for joining
[74:08] because I love how data modeling really does show up. I'm like on repeat right now.
[74:13] I'm like, it just shows up everywhere. - It does.
[74:16] And that's like, it's hard to like create something like, okay, well, here's how you model data.
[74:22] Like, and you know, I, again, I kind of like tried to prepare and I'm like thinking like different things
[74:26] and like we'd talk about, but it's like, it really is just everywhere.
[74:30] And like, you've got to chat about it and eventually you start to see it
[74:33] and then you practice it and it eventually comes out. Like it's chiseling away at the marble
[74:38] until it creates a sculpture, right? - And that's what matters.
[74:41] And when we get off the live stream, we can figure out when.
[74:46] And I do have to say really quick, 'cause you're here, homie.
[74:50] Homie was my first subscriber. - Excellent, how cool.
[74:56] - I'm so excited. I am up to two now.
[75:00] I am very excited and it's growing. It's learning and learning live is hard.
[75:07] It's like, I'm going to make mistakes in front of everybody.
[75:11] - No, but I think you're doing great. And that's part of like the, again,
[75:16] kind of going back to the building public university, a lot of it's learning in public.
[75:21] And so being able to do that, I think actually sets you up very well for success
[75:27] because it's that proof of work, right? Instead of being on a resume,
[75:32] like you're like, oh, like just here's my live stream that I've been doing,
[75:35] that like literally we're going through all these different topics and chatting about them.
[75:40] And it creates this level of proof that you can't quite capture in like a resume or anything.
[75:45] And plus you just actually go do stuff with it, right? Like you're actually like,
[75:49] oh, well now I've got this like distribution channel and I've got these podcasts
[75:53] and like you can start tying things together. And that's really like where I get excited
[75:58] about like as things like start growing and then I can like start connecting them.
[76:03] And like there's all these little overlaps that kind of come into play.
[76:08] And building out these individualized systems that help like help us do whatever we wanna do,
[76:14] even if it's like all this weird stuff and just, you know, but it's fun.
[76:19] And that's the part that I, it's real fun. That's what matters.
[76:23] - And Steph, their Twitter is @StephLikeCurry is also looking at being on the show
[76:32] and they are a data engineer too. - Awesome.
[76:36] - It was the first one that I registered was a data engineer,
[76:39] but I think that's because of Twitter spaces and stuff. And thanks, homie.
[76:44] I appreciate it. Saying no doubt, get to witness a rising star.
[76:49] I kind of want like a star that I can just like start holding up, be fine.
[76:53] - Every episode, hold it up a little higher. - Well, I just did the journeys of a developed Cato.
[77:02] And so my boss was like, can you just have an avocado
[77:06] just slowly sprouting on each of them, on each of the blog posts.
[77:11] And we looked up what an avocado plant looks like. It has really weird flowers.
[77:17] So I'm not gonna do that. - Okay.
[77:18] - Yeah, I was a little sad, but anyway, you and I will, once we end this broadcast,
[77:25] we will figure out when to schedule next. And thank you everyone for joining.
[77:30] Hit us up if you have questions on Twitter. My Twitter is right there.
[77:35] And Leah's Twitter is there ish, something like that. So let us know.
[77:44] I appreciate you and like, no, follow, follow. There we go.
[77:49] Follow, unless you're watching it on YouTube, then you can like it and subscribe and all that.
[77:53] Thank you. Talk soon.
[77:55] - Thanks, homie. 
