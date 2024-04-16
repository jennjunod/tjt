---
showLink: "https://www.youtube.com/watch?v=WVPm5jxJI90"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-to-start-understand-produce-documentation-with-matthias-dugu"
title: "Teach Jenn to Start, Understand, & Produce Documentation with Matthias Dugué"
publishDate: "2022-08-12"
coverImage: "https://i.ytimg.com/vi/WVPm5jxJI90/maxresdefault.jpg"
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

[00:00] for joining another Teach Gen Tech. Today we have Mads here,
[00:04] and y'all before like Mad gets to introduce himself and talk about what we're learning,
[00:10] his like Twitter name is M4DZ. And every single time until today,
[00:19] that is how I've been talking about him. And it's so simple, it's Mads.
[00:23] And now that you've told me that, I'm like, that makes so much sense.
[00:28] So Mads, please introduce yourself and let us know what we're gonna be learning about today.
[00:37] - Yeah, thank you. Thank you for having me today on the show.
[00:39] I'm really happy, really excited to be here today. It's been a while since I was on the show
[00:45] because, so I'm Mads. I'm a former front-end developer,
[00:54] former developer advocate. But I moved in a new company really recently
[01:03] and now I'm more responsible about developer experience and so on.
[01:06] And not that much involved in developer relations directly, let's say that.
[01:14] But yeah, the fact is, most of all, I'm a dev tool nerd.
[01:21] I like the tools, I like developer tools because I'm developer.
[01:26] And probably one of the things that I really love to do is just tweaking things just to be sure
[01:35] that everything is working really well to help people to better work
[01:41] or better do their job simply. So it was a long journey because I'm old.
[01:49] (laughs) And I had a long career over something like 20 years
[01:58] in the web ecosystem. So it was really interesting and really passionate
[02:05] to be there, seeing the world evolving and the web platform evolving and so on.
[02:10] But yeah, right now I'm mainly working on improving the developer experience with some tools.
[02:19] And today we're gonna talk about documenting because documentation is a key
[02:24] to help people to understand your project and work with your project.
[02:28] It's something that is not really easy to dive in and really easy to understand at first
[02:36] because nobody loves documentation. So yeah, I hope that we're gonna cover
[02:47] as many things as we can to help you to better understand how to well
[02:54] architect your documentation and so on. - Thank you.
[02:59] - And yeah, that's it. - Yay, and Anthony and Ben, hello, hello.
[03:05] Yes, I am very excited about this today and the fact that I am not great at documentation in general.
[03:17] I've had roles where they actually hired someone to follow me around to figure out what I was doing.
[03:27] Hi Bakari, thank you for joining. And they literally, it took a month for him
[03:35] to figure out what I was doing and document everything where as Anthony showed me how to do the read me yesterday,
[03:45] if I did that along the way, that would have been so much easier
[03:49] and documentation from doing it myself. So I am very nervously excited about today.
[03:57] Yeah, so where do we start? What is documentation?
[04:04] If you were to like explain documentation, how would you explain it?
[04:09] - Exactly, that's a good question. What is documentation?
[04:15] This is a story of the trees falling in the forest. Does a tree that fall in the forest make sounds or not?
[04:27] Is nobody is here to hear the sound. Maybe we could assume that the tree doesn't make sense,
[04:34] it doesn't make a sound at all when it's falling. And this is exactly the same thing
[04:38] with documentation and project. You can do the best project of the world
[04:43] and it can be just extraordinary to help your teammates, but without a good documentation,
[04:51] nobody would want to use it and nobody would want to work with it
[04:54] because nobody will be able to understand how it works. And nothing is really intuitive.
[05:02] We have to learn every day, all our lives, how things is working and how to work with different things.
[05:10] So documentation is just that, it's just a way to help you to understand things
[05:18] and start working with different kinds of things. And I guess that the key in documentation is exactly that.
[05:26] It's here to help people to start. And because if you don't know where to start,
[05:32] you just can't use anything. So yeah, read me is a real good point
[05:37] because when you check out a new project, especially when you work in the open
[05:44] and you are checking out a new open source project and something like that,
[05:48] with no read me at all, I'm just closing the page. I don't want to deep dive into the tool
[05:55] to understand how it works and so on. And the first thing that I'm doing,
[06:02] each time I'm installing a new tool or something like that,
[06:06] the first thing that I'm doing is just to launch the command with the help flag,
[06:12] just to see the documentation in the CLI, just to understand, okay, is there a good documentation?
[06:17] What are my different options? How can I use this?
[06:21] What is intended for? And if you're not able to give that
[06:28] to the rest of the world, it would be complex for your project
[06:33] to be really adopted by different kinds of people. But I don't know.
[06:40] When I say different kinds of people, it's also just be you in the future.
[06:47] You're not the same person today than you will be in two months or in two years.
[06:53] And I can't count the number of different projects that I just started without any documentation,
[07:01] just for myself, just saying, okay, it's just a small tool. I just need a little script to do something,
[07:06] just coding it easily, quickly. And two months later, just diving into this project
[07:13] and saying, okay, what I tried to do with that? I don't understand what I want to do with it.
[07:20] So yeah, living documentation, it's at first, it's also for you,
[07:25] just to understand your work better. But it's not that easy
[07:32] because nobody is really good at writing documentation and except for a few people, I guess so.
[07:43] But generally developers prefer code. And I often heard in the past that many developers saying,
[07:53] you know, code should be self-explanatory and so on. But I did trust it in the past.
[08:04] I don't trust this vision anymore because it's not really helpful.
[08:10] I mean, code need you to focus really heavily on what is written to really understand it
[08:20] because it's not natural language. It's a language with its grammar, with its vocabulary,
[08:28] but it's not natural language. And you can't read the code
[08:32] like you are reading a page in Wikipedia. And it's really not the same thing.
[08:38] So if you have to make this effort to understand what is really written in the code,
[08:44] you probably missed some point of how the tool is made or what is intended for and so on.
[08:53] So yeah, you have to write it at some point, you have to document things, but nobody's really,
[09:02] I mean, developers are probably not that comfortable at writing.
[09:06] I'm not, definitely producing documentation is something that is really, really complex to me
[09:12] because I'm not good at writing. I can, but it's a lot of efforts for me.
[09:20] So I definitely need some kind of frameworks and some kind of tools to help me
[09:27] to write better documentation. - Got it.
[09:31] And thank you for that. You just, Anthony also put it in the chat
[09:37] about that docs are primarily for yourself and then it's a second word for others.
[09:44] And I feel like you said that as well. I will say, I completely understand your example on,
[09:53] we're not gonna be the same person in two months. It has been exactly,
[09:57] Anthony came on the show again yesterday and it was, he was my second guest
[10:03] and we did the read me for what he taught me a month ago. And I didn't remember anything
[10:09] that he taught me a month ago at all. Like, I was like, okay, cool.
[10:15] And so it's interesting how quickly we forget these things and how useful it can be.
[10:22] So I'm excited to talk about more of the theory today and doing, when Ben was on the show,
[10:32] we did it more as a go through examples to discuss what we could or should
[10:38] or why something needs to be changed for web accessibility. And later on, he'll be back on
[10:45] so we can do examples of how to make that or how to make the changes.
[10:51] So I'm glad we're doing the same thing 'cause there's, it's a lot to go through.
[10:57] Now, as a very random side note, do you know why there are so many startups
[11:07] and API and tech companies from France? I'm still like trying to figure this out
[11:15] because there, as a co-organizer in the Denver API meetup, all three of the other co-organizers are from France.
[11:23] My, I got, I just was hired as a contractor for Devereux and Community, which everybody else listening,
[11:34] I will tell you details later. And my boss there also lived in France and speaks French.
[11:39] And my last name is French. And I'm like, what, how is there like so much
[11:44] coming out of France specifically? And I, do you know why?
[11:51] Do you have theories? - Yeah, I, we have many theories around this one,
[11:57] but there is a proverb in France that is saying, we don't have oil, but we have ideas.
[12:06] And this is probably exactly that. We are not a rich country producing a lot of resources.
[12:16] We don't have any petrol. We don't have, yeah, we don't have any rare metals,
[12:22] mines or things like that. We don't have anything.
[12:27] We just have our brains and that's all. And there is a long, long, long tradition in France
[12:34] over the centuries about thinking and philosophy and technical thinking and so on.
[12:41] So we have, I guess, are really, really good schools in terms of techs and not only on the technical side,
[12:52] for sure, there are so many things, but this is something that French people really love,
[12:58] make things complex, overthinking things. So I guess that we're producing a lot of good engineers
[13:05] because we love to overthink things. So I guess that's why,
[13:09] but it's just one theory among many others, I guess so. - Ben just said that I hold people hostage.
[13:18] Like I get one guest. It's because I meet so many people.
[13:21] I've asked a lot of French individuals the same question just to see, because I keep meeting them.
[13:29] And like, it's interesting. I don't know, because a lot of companies are there too.
[13:34] So Ben, I'm going to ask you as the one person for accessibility now, like you were the one person.
[13:41] Well, and that's true because with Bakari, I would ask him about FinTech stuff.
[13:46] And with Anthony, I would talk one day, maybe about Web3 stuff, maybe.
[13:53] So yeah, I kind of asked the person from the area. So good call out, Ben, good call out.
[14:00] All right, we're just back on track. So I know when we first met, you showed me a tool of,
[14:07] I said it correctly earlier, Diataxis. - Yeah, that's it.
[14:15] - Is that a good place to start or is there somewhere else
[14:21] that you think we should go through first? - I guess that we will jump on it in a minute,
[14:29] but the reason I was, I just want to explain that, but because the reason I was that interesting
[14:38] about documentation and things like that, is that because in the longterm,
[14:44] it's really complex to maintain the documentation. Writing a documentation is something complex,
[14:48] but maintaining a documentation over the time to help people to continuously find the right things
[14:55] at the right place and don't have content that is suddenly outdated or something like that,
[15:02] it's also something really complex. And when I was young,
[15:07] there was something in the DuckTales comics, the junior Woodchuck's manual, something like that,
[15:18] which was for the Donald Duck's nephews, they had this kind of fictional scooting company,
[15:28] something like that, and they have a manual. And each time they had a question about something,
[15:34] anything in the world to just open the manual and they have a great description of what it is,
[15:39] how to deal with it, how to work with it and how to get some advantage of it.
[15:45] And I was just fascinated about this book. What is it?
[15:49] How it works? What is this thing?
[15:51] This is just insane. How could the whole knowledge of humanity
[15:57] could be resumed in just one book and with not only something really exhaustive
[16:04] like Wikipedia, where you have just a big description of what things are, but also a lot of instruction
[16:13] on how to use it and how to take advantage of things. And it was just really something crazy to me.
[16:21] So this is probably the things that I'm really seeking when working on documentation.
[16:29] Having this kind of efficiency when you are writing content to help people,
[16:34] not only what it is or just a short description of, well, this is my project
[16:40] and this is what I wanna do with it, but really something helpful.
[16:43] What is it? How you can use it?
[16:46] What it will provide you and so on. But it's a lot of content.
[16:51] So you have to structure the content. And this is where the Diataxis Framework
[16:55] is entering the stage. The thing is that I spent a lot of time
[17:03] trying to figure out how to create good documentation and how to organize the content.
[17:12] And the first time I was really involved in it were in my company,
[17:21] because we had some kind of documentation and working at a hosting provider.
[17:26] So there is a lot of things to cover how to pull your web pages or to deploy
[17:31] or to run a CI or to, I don't know, commit some new stuff or to configure some content
[17:38] or to use some kind of database, which is MySQL or Postgre
[17:43] or using a broker or using, well, you name it, the whole web ecosystem is really complex,
[17:49] especially in the backend. So we had this big amount of documentation
[17:56] that was just built over the time by just making some additions at some point.
[18:01] Okay, we are missing this part. Let's edit.
[18:05] But nothing was really well-structured. So I started to handle it and quickly I figured out,
[18:12] okay, we will have a problem with this one because we really can't use the documentation right now.
[18:20] It's not usable. People are not finding the thing in it.
[18:24] So we have to revamp everything from scratch and trying to figure what the content
[18:30] we really need to use. And during this big search,
[18:38] I watched a lot of different content and different conferences.
[18:43] And there was one by the main maintainer of the documentation for the Django framework,
[18:51] which is a framework in Python, which is, it's totally unrelated,
[18:58] but which is a framework that we're using on the platform, the company I'm working in.
[19:03] And he explained in one hour, how they finally decided to decouple
[19:15] different parts of the documentation. And it finally leads to the Diataxis framework.
[19:21] - Interesting. And I like the way you led up to that.
[19:27] And now I want to find that book and see if they have it in an English version.
[19:33] - Yeah, I guess there were some additions. I had a French edition somewhere in my pile of books,
[19:43] but yeah, it's definitely not that complex that it is in the comics because yeah, it's just comics.
[19:52] But yeah, it was fun. - Okay, and I'm going to put the link in here
[20:00] before I forget. So anyone else that wants to look at this,
[20:03] they can on the, what we're using today. And now you mentioned that it was the Django
[20:13] and which is a Python framework. And now is this, doesn't matter on the backend
[20:30] or using a certain type of document, do you have a suggestion on documentation platform?
[20:37] Like if we want to create documentation, is there a good way to start thinking about that
[20:44] of where it should go before we go into what is it? It could just be me thinking about this to conceptualize
[20:51] is like seeing what the big picture is to go to the small picture.
[20:56] - Yeah, nothing forces you to build a comprehensive whole documentation at first, it will help you.
[21:07] But more often, this is just you gathering some different pieces of information
[21:14] and trying to put everything at the same, in the same place, in the same shape.
[21:19] So generally when you're starting a project, you just want to start with a really small amount
[21:27] of documentation, like just to read me with what are the prerequisites to run the project,
[21:33] how to quick start it, how to work in it and develop in it, is there is some kind of conventions
[21:39] or things that you have to follow to work with it, how to use it quickly, probably something like a license,
[21:48] list of contributions of contributors on the project, how to get support on it, because at first,
[21:56] probably you won't have enough time to write everything. So it would be probably better if people are just popping
[22:05] and asking for some things saying, okay, I'm trying to do this or that, how to do it.
[22:11] And after that, you could progressively gather different pieces of information and trying to organize it.
[22:19] And it's not always true because there is projects that are really good at writing documentation.
[22:28] I have in mind the Vue.js framework. This is just, to me, this is just, I don't know,
[22:37] some kind of alien in the space of web development because the first time I discovered Vue.js,
[22:46] it was with the first version. And at that time, it was just the beginning
[22:52] of the reactive interfaces and people were all saying about talking about React and working with React and so on.
[23:03] And I wasn't really convinced by React at this time. So I just had to look through different alternatives
[23:11] and I discovered Vue.js, which was some kind of side project or something like that, a really small one
[23:19] with not a lot of contributors. But the documentation, my God, it was just terribly good.
[23:26] It was just perfect. I just read it like a book from A to Z
[23:32] and it was just, okay. After that, I felt ready to use it
[23:37] because I saw the big level of how to use it and what is it intended for.
[23:46] But I had also the opportunity to dive into the API and the primitives and how it is working under the hood.
[23:54] So you are more confident in using the product because you can understand how it works.
[24:00] And yeah, but this is really not common. A lot of different projects don't have this high level
[24:09] of documentation production. And I guess this is probably because even the creator
[24:16] of Vue.js really loves writing documentation. So he's spending a lot of time on it, but yeah,
[24:24] not all project, especially project maintainers in open source have this amount of time dedicated
[24:30] to write things and maintaining documentation. So at first, producing a really small content
[24:36] of documentation is probably enough. But as you are working in it and as you are fixing bugs
[24:43] and adding new features and new things, you will probably have too much content
[24:50] than just you need to fit into the readmes. This is just really good.
[24:56] So you have to start to decouple the content and keep the readme really small
[25:00] and understandable for newcomers. But after that, something like a wiki
[25:05] is probably something really great, because you are just putting the documentation
[25:10] and you are just saving stuff for later. And just for the future, as a reference,
[25:16] like, okay, how does this thing work? Or how I fix this specific bug
[25:23] or this specific issue and so on. So this is great, especially when you are trying to work
[25:31] with different kinds of people. But quickly, you will probably have a project
[25:35] where in the wiki, everything is just, overwhelmed and just put at the same place
[25:47] without really a real organization or a real architecture and so on.
[25:51] So when you are touching this point where your documentation is not reliable enough,
[25:57] and you don't want to read it anymore because it's not that good,
[26:03] and you know that it would be a pain to just find the right information
[26:07] into this amount of big wiki, then you will have to revamp it
[26:11] and work on a dedicated, well-organized documentation. You could start with it directly at first.
[26:19] It's totally up to you. And it's nice things to do,
[26:21] but it needs you to be really focused on how to use it and how to use the content and so on.
[26:30] And it's a lot of efforts. And at first, you probably want just to produce code
[26:37] rather than writing, writing, writing, writing, and so on. - I will say that I do want to get to writing more.
[26:45] This last week, I actually posted my first blog. I felt like such a cool kid.
[26:51] And I do want to go back and listen to my previous episodes to go through and be like,
[26:59] this is what I was hoping to get out of it. This is what I did get out of it.
[27:03] And these are things now I want to learn. But to give more of an access
[27:09] to those who want to watch the videos to learn more, because yes, this is video documentation,
[27:15] but not everybody learns by video documentation. I know that a lot of people learn by reading documentation
[27:22] where me on the other hand, I'm like, I'll read it. I'll probably get a decent understanding about it,
[27:28] but it doesn't always compute then how to do it or without like the screenshots or something like that.
[27:37] So it's, we all learn so differently. And that's, I think the beauty of it,
[27:41] of when we have video or we have webinars and we have documentation.
[27:46] There's so much that goes into it to read the code. - Yeah, yeah, definitely, definitely.
[27:52] You know, when I'm applying at different kind of conferences, I often apply with regular talks like 45 minutes
[28:04] or one hour on stage in front of people and just talking and explaining things and so on.
[28:11] But I also love to submit workshops because workshops are a really different way to learn.
[28:18] You know, you have three to four hours or even sometimes a full day
[28:23] and you're totally dedicated to, okay, we're going to see how it works,
[28:29] working within, failing, fixing things, tasting and discussing with the audience.
[28:36] And you're just not in front of people and just clamoring and just explaining big stuff
[28:44] but you are more into the dirt. And this is what is really interesting.
[28:50] And it's a different way to learn, as you said. And some people need just text,
[28:55] some people need code examples or screen shots or videos or demonstrations.
[29:01] Workshop is also good. So yeah, it's, this is why producing documentation
[29:08] is that complex because not all the people want the same thing.
[29:13] So we have to find a way to help people to access the documentation.
[29:19] And we need to find a way to help people to contribute to documentation
[29:24] because the more contributor we will have, the best documentation will be at some point.
[29:29] And if you are a bit in the design side or something like that,
[29:39] it's definitely sounds like working with personals. So we, before writing documentation
[29:47] and this is why I really love the Direct Access Framework. This is, it's, the first question is, okay,
[29:54] for who are we writing this documentation right now? Who are our users of the documentation?
[30:02] Because this is probably not users as a product, as a framework and so on.
[30:06] And we have to keep that in mind. - That brings up, reminds me of yesterday,
[30:15] Anthony and I took a moment at looking at this, but it is interesting to think about how,
[30:22] like who is gonna be using this, as you said. Yeah, and I think this is where I got a little lost
[30:32] and sometimes I do of, so like, why would somebody do understanding-oriented explanation
[30:41] instead of information-oriented reference or, you know, so for those who are listening and watching,
[30:50] I've already put this in the chat and will you go through explaining this a bit more?
[30:58] 'Cause I feel like it's, since you're familiar with it, it's gonna be better than me explaining it.
[31:03] - Yeah, for sure, for sure. I think that I really love with the direct access framework
[31:09] is that it's not a tool. Because as technical people, we often like tools
[31:17] because we often think that it will solve our problems, but it's not true.
[31:23] The tools are just the things that we are doing with it and that's all.
[31:26] So direct access is totally agnostic. It's just a framework,
[31:31] not in the technical sense of the term, but just give you frame
[31:36] and it's like a decision matrix. So the idea is that you don't have,
[31:42] you can't write just one documentation because people, not all the people
[31:50] need the same kind of content, but you will probably have to maintain
[31:54] four different kind of documentation for the same products. And they split the different parts of the documentation
[32:03] in four big sections. The first one is the tutorial sides.
[32:10] This is exactly what beginners want when they start with the project.
[32:15] I'm totally new with it. I don't know how it works.
[32:20] I just need some kind of quick start to quickly understand who it is
[32:27] and to have this really rewarding effort that suddenly, boom, it works.
[32:34] And you don't really understand what you are doing. You are just probably copy pasting some kind of commands
[32:40] or some chunks of codes, but suddenly it works and you are really happy with it
[32:45] because you were able to have it running and working. And this is a really great experience.
[32:51] This is probably what will make the difference between leaving the product and not using it anymore
[32:57] because you are not able to run it and to have it working or being able to have some things,
[33:03] which is probably not what you want in the end, but just at start, it's a good start, you know?
[33:11] So you have the tutorials and the tutorials are all dedicated to those different quick starting guides.
[33:18] And that's all. They are like recipes in a kitchen, you know?
[33:26] You are following the instruction and at the end, you will have a cake.
[33:30] And independently of the context, independently of anything, you are in a situation,
[33:35] you have flour and eggs and blah, blah, blah. And you're following the instruction.
[33:40] In the end, you will have the same result and you could replay it over and over and over
[33:45] and you will also have the same result. It's really strong because it will structure
[33:50] the first impression on your product. On the other hand, you will also have
[33:56] some kind of how-to guides, which are more dedicated to solve a specific problem.
[34:02] Like, okay, in this particular context, I'm using this product or I'm using this framework
[34:09] in a React application. And in this particular context, I'm facing this issue.
[34:16] How could I solve it? So there are more oriented guides
[34:20] on when I'm in this kind of situation, how could I find an answer to my problem?
[34:30] So it's probably some content that is gathered over time
[34:36] from the different kind of issues that were solved. Like, okay, you are using the product,
[34:43] it's compatible with this and this and this and this. So if you are using A, do that.
[34:49] If you are using B, do that and so on. So it's a great place.
[34:56] It probably replaced the Wiki at some point. It's a place where you are just gathering
[35:02] different kinds of content and different kinds of information.
[35:05] But they're all technically oriented. It's for practicing, for doing things.
[35:14] Third party, it's the explanation things where you are giving some kind of insights
[35:24] or on what is it, how this content is working. Like, we made a decision in the past.
[35:34] Just a little story, parenthesis, but I first started my career as a freelancer
[35:44] and after five years, something like that, I joined a web agency.
[35:49] And the first project I was working as well, I was really young.
[35:52] I had, I don't know, 25, something like that. And so I was in this agency
[36:00] and the first project I was working in was some kind of website factory
[36:06] met with Drupal in PHP. And they asked me to add a new site into the factory.
[36:12] And I was starting to work on it. And the more I worked on it,
[36:17] the more I was, what is this code? This is just, this is just crap.
[36:23] Oh, how could we work with that? How did you, were able to produce that piece of shit?
[36:31] And this is for our clients. And I was young and I was really not humble at this time.
[36:38] And I worked on the project. And after that I was, okay, okay, okay.
[36:42] I do understand why we're doing things like that. And it's not finally, okay, it's crap,
[36:48] but it's probably, it could be more crappy like that, than it is right now.
[36:55] So we have to be humble on what we are producing in our daily basis,
[37:02] because there is, there is context and there is things that are some kind of impact
[37:11] of what you are doing in your, in your product. But if you're not able to explain that
[37:17] and to explain why you made this decision at some point to just to, why I'm using this particular library,
[37:26] why did I fork it rather than using the main one? What was the features that was missing and so on?
[37:37] People will probably quickly judge you on what you did. And it's not personal, but it's human.
[37:48] They will try to fix it. And they will try to do better things
[37:52] because they don't understand the context. And they will last a lot of time,
[37:57] probably a lot of frustration, trying to fix things that could not be fixed at some point
[38:03] or something like that. But if you are able to give some kind of information
[38:08] in front of that, explain, okay, we're using this in this particular context
[38:12] because there is this specific things that we need to address and so on.
[38:18] It will make your code and your decision more understandable for the rest of the contributors
[38:25] and the rest of the users. So this is exactly what the explanation part
[38:31] are dedicated to. The context, design decisions, architecture decisions.
[38:38] So it's kind of contents that help to understand who it works behind the hood
[38:45] and how you could work on it to improve it. And finally, the fourth one is the reference.
[38:56] That is probably more something dedicated to a big comprehensive documentation
[39:05] of the different parts. Like, okay, I made a, I don't know,
[39:09] I made a component and this component is exposing those properties.
[39:14] And this component is exposing those methods and you could call this API and so on.
[39:21] This is like the manual pages in Unix, when you type man and a command in your terminal
[39:28] to get some information. This is exactly that.
[39:31] So if you organize your documentation and you put different parts of your documentation
[39:38] in one of those four parts, then you will be able to build
[39:43] a really comprehensive documentation. Because what is interesting is that they are working,
[39:48] they're working together. I mean, if you are more interested into practical example,
[39:57] you will have a look at tutorials and you will have a look at auto guides
[40:00] because they are the technical side of the documentation. When if you are working on understanding the basic,
[40:07] understanding the gears that powering the product and so on, you will probably have a look more at the explanation
[40:14] to understand the context and understand why it is working like that and so on.
[40:18] And you will have a look at the references to have a big overview and big comprehension of the content.
[40:23] But if you want to study on the product, just to understand how it works at first,
[40:28] then you are running the tutorials. And when you are comfortable with the tutorials,
[40:32] you will probably have a look at the explanations because they are all dedicated to understand
[40:38] the big picture of the product and how it works. But if you are facing some issue at some point
[40:43] and you are working, really working with the product, then you will have a look at the auto guides
[40:47] to help you to fix the issues and to the references, just to understand the API and the content behind it.
[40:53] So it's well made when you are looking for a content because you just have to ask yourself, OK,
[41:07] what kind of content I'm looking for? Am I looking for a big, comprehensive content?
[41:12] Or I am looking for some kind of context and so on? And you will be able to just pick the right part.
[41:18] But if you are contributing to documentation, the first question is, OK, I want
[41:24] to add this kind of content because it's something that I miss in the documentation right now.
[41:30] What is the purposes of this content that I will produce to find the right place to put in it?
[41:36] I know. This is a lot to take in.
[41:42] I always say, I've got to start with your notes. So would it-- OK, words.
[41:56] So for example, a readme may be a bit more of an explanation and could be a bit of tutorial and how to as well,
[42:10] mattering on what it needs to do and how big the project is. Yeah, yeah, because readme is--
[42:24] it's sometimes the right place just to put everything in it, you know?
[42:29] And being just well-organized in different kinds of chapters, like, OK, a quick start section, then a how-to section,
[42:38] then some kind of explanation sections. And the references could be in a dedicated page
[42:45] somewhere else. I'm seeing a lot of really small tools in the Unix world
[42:56] just dedicated to do just one thing and do it really well. And they just have a simple readme.
[43:02] And everything is in the readme because you don't have to cover a lot of information.
[43:06] It's probably a script with three flags and just one feature and that's all.
[43:11] You don't have to produce big documentation around that. Probably readme is just enough.
[43:15] And everything is gathered at the same place. So you don't have to follow a bunch of links and so on.
[43:21] But if you are working on something really huge and really complex, like a library, like React or Django
[43:27] and so on, then, yeah, you will probably need this kind of frameworks to help you well-organized
[43:35] and keeping things well-maintained over time. Another thing is that you don't have necessarily
[43:45] to build a big architecture and different kind of pages. You could do it step by step, just starting the product,
[43:58] starting your project with a simple readme. And as you are adding documentation in the readme,
[44:05] starting to create sections like, OK, I will add a simple how-to pointing to some issues
[44:12] or some PRs. And over the time, you will refine it and have
[44:16] it more and more organized. But without really organizing your content
[44:24] in the Data Access Framework, but just having it in mind and just asking each time you are adding just a few words
[44:32] in the documentation, OK, what kind of content I'm trying to produce and what it will be used after that.
[44:41] It's sometime enough. It's just a way to put you in the right mindset
[44:47] to write the proper piece of documentation. I'm also-- and thank you for that.
[44:55] I'm also like-- and it definitely is over here on the side for anybody
[45:00] that is wondering and wanting to go through this of-- so tutorials, how-to guides, reference, explanation,
[45:08] and then understanding users' needs, tutorials versus how-to guides.
[45:13] I think something that I'm not seeing here that you used as a reference yet,
[45:21] it's not completely clicking, is tutorials versus reference or explanation versus reference.
[45:29] The other three seem to be pretty self-explanatory. Explanation-- anyway.
[45:37] But reference, I think, would it be something like-- so yesterday, I used some--
[45:47] part of my README had documentation that I needed to use from somewhere else.
[45:54] And I put in the link to that website. Would that be reference or--
[46:02] Yeah, definitely. Definitely, reference is where you
[46:07] will have a look when you are looking for extensive documentation, which
[46:16] could be something directly written in your documentation, but where you will probably also point
[46:23] to different kind of links and different kind of external resources to help you to better understand
[46:30] which works. You don't have to rewrite everything.
[46:33] I mean, if you are creating an interface that is using React, you won't rewrite the React
[46:42] documentation. You will point to the different parts of the documentation
[46:45] in the React framework, the React documentations that are relevant to the different parts that you are looking for.
[46:52] So reference, to me, it's probably something like big Wikipedia.
[46:59] I love just wasting time in Wikipedia. Open a page, starting to look at it,
[47:05] and open in the background 5, 6, 10, 12 links, because I'm just facing a new concept.
[47:13] And I'm just, OK, what that? I don't know this one.
[47:17] So I jump to the concept, read it, and so on. And suddenly, it's four letters.
[47:21] And you are just saying, OK, I just wanted to learn a simple thing about plants.
[47:27] But yeah, it's definitely that. Good reference, it's something where
[47:34] you could easily go over different kind of concepts. I feel like-- let's see if this one would work.
[47:42] So I used to work at Stoplight. And Stoplight creates API specs, design-first API specs.
[47:50] And Gravity, for example, or Axway does API management. So let's say that they created their documentation.
[48:02] And explanation is why they created something or more details of it, where reference could be linking out
[48:10] to what is an API, or what is governance, or something like that.
[48:16] Yes. This is exactly that.
[48:20] But then explanation could be, for the Stoplight reference, why is design-first better than code-first?
[48:33] Yeah, exactly. Or something really trivial, like, OK,
[48:38] why did we choose this yellow shade for the primary color in the design?
[48:48] Sometimes it's just as simple as that. Why are you using this yellow?
[48:53] Hey, why are you using this-- I have a friend that is working at a company in France,
[49:00] Orange, which is the telecom official provider, phone provider, and so on.
[49:09] And they are doing a lot of work on accessibility. And the orange, which is their primary color, for sure,
[49:17] with a name like that, is a particular shade that is used because it's well-tested in terms of contrast,
[49:28] in terms of accessibility needs, and so on. And this is exactly the right place
[49:33] in the documentation. The explanation is, OK, why is this shade of orange?
[49:38] Because it fits different needs. Because it's OK in terms of contrast,
[49:44] in terms of accessibility, in terms of blah, blah, blah. And this is just understanding everything
[49:52] that is running outside the product, which made the nest of your product.
[49:59] Now, would-- I totally get it from a company standpoint with documentation.
[50:08] Do developers ever make their own documentation, like, hey, this is all the stuff I've ever
[50:13] done to go with all of their projects, like their Git repository?
[50:17] And be like, hey, here's why I did all of these, or something like that?
[50:22] Yeah, I don't know. I don't know, to be honest.
[50:28] But, yeah. And it's interesting how people, especially developers,
[50:38] are trying to document their own lives, you know? It's-- yeah, I don't know.
[50:49] Maybe because I have a developer mind, because maybe because I'm just a dev tool nerd, I don't know.
[50:59] But we were currently revamping our whole apartment. You can see in the back that this is definitely not finished.
[51:07] But we are working on it. And yesterday, I was just, OK, I want to remap.
[51:14] Finally, I want to remap the slides, because this is not exactly what we want.
[51:18] So I kind of remember that I have some wires coming from here to here.
[51:27] And suddenly, I couldn't remember what I did, because it was one year and a half ago.
[51:33] But I know that I have a lot of notes. And I just have to take my book.
[51:37] And in it, I will find the schemas of different wiring process and so on.
[51:43] And I know that everything is documented. And it's really--
[51:47] I don't know, I'm using a lot of different tools to take notes and keep tracks of different things.
[51:55] And I know that there is a lot of people that are doing that and that are not necessarily developers.
[52:06] I have a really good friend. She loves going into bars and restaurants.
[52:13] And she had a pile of notebooks where she just writes everything she knows about--
[52:21] I had to test Zeus and Zeus and Zeus restaurants. And I want to keep this note.
[52:27] And I have that in mind and so on. So we are all taking notes all over the time.
[52:33] We are all documenting our lives. And yeah, it's not that different than just
[52:41] documenting a project. At least, it would probably be simpler to document a project,
[52:49] because it's just a small part of our lives. But yeah, I don't know.
[52:56] That does make sense, and I like what Anthony said to do-- when I asked, do developers document their projects
[53:05] for themselves and their work? And he said, only the selfless ones.
[53:10] And I feel like this-- oddly to your example, it makes sense
[53:15] where people that have written journals their entire life, it may be easier for them to one day write a book,
[53:22] because they have all of that documentation. Whereas people that don't, it's just based off of memory
[53:28] and probably forgot a bunch. So it's so interesting.
[53:32] It's interesting what you are saying about this concept of books and so on, because--
[53:38] this concept of books. I tried to write technical books twice,
[53:47] I guess, something like that. It was a big failure each time, because I don't know.
[53:53] It's really hard for me to write stuff and produce 200 pages of content and something like that.
[54:01] I don't have the right organization to do it the right way and so on.
[54:09] And it's a shame, because I have a lot of personal documentation all over my notebooks
[54:15] and my journals and so on. So this is always the same thing.
[54:19] Why can't I convert those notes that I'm taking for myself into something more understandable
[54:25] for the rest of the world? And the complexity of the documentation is exactly that.
[54:30] You are not writing only for you at some point. You start for you, but at some point,
[54:36] you are also writing for the others and contributing and working with the others
[54:41] to build this documentation. So it needs an effort to twist your mindset into something
[54:48] that is not understandable only for you, but also for the rest of the world.
[54:52] And it's definitely not that easy. And that also does make sense in--
[55:00] Anthony told me that when starting to write my read-me's or something like that
[55:05] or documenting, it's also a lot easier to create blog posts, because then you're--
[55:11] and in my mind, that is like taking documentation and then telling a story with it,
[55:16] like what you were-- to be able to write your--
[55:19] ooh, I haven't done it yet, so we'll see. We'll see how that goes.
[55:23] [LAUGHTER] At least I have them recorded.
[55:28] I have the video. Yeah, that is something that I really do want to do.
[55:31] So that way-- this was really helpful, thinking of a way to--
[55:40] what video-- if I write a blog about a certain video or series, like for example, Bakari, we had part one,
[55:51] part two, what am I going to do as a tutorial, a how-to guide, why did we do it that way, references to--
[56:01] for his, we used Square, so references to Square. Very interesting.
[56:08] Yeah, it's-- yeah, it's-- I guess it's a complex thing to handle it well.
[56:19] And you don't have to be too rude with yourself when you are working, because nothing is never perfect.
[56:26] So I started, I don't know, three months ago, four months ago, something like that,
[56:37] I started to write a simple blog post about my video setup, because I'm also hosting a show, and I have a conversation
[56:48] on Twitter with people saying, oh, I see a lot of different people using this tool,
[56:53] and I don't know exactly how it works, and so on. And this is exactly my setup.
[56:57] I can help you. I can document that and help you to understand it well.
[57:01] So I started to work at first a simple blog post. It's still in the process of writing,
[57:07] because the more I'm working on it, the more I'm just saying, OK, I need to add that, and I need to add this,
[57:13] and oh, I'm missing this part, too. And it starts to become a big monster, you know?
[57:19] And I'm really bad at writing blog posts, because I can't just cut at some point and just say, OK,
[57:27] it's enough for this one, and I will make another one later, or maybe in three months to cover another part,
[57:34] or making a series. But when I'm starting to think, OK, I have to make a series,
[57:40] suddenly it's just, OK, but I have to architecture. What I will put in the first blog post,
[57:44] and what in the second? And oh, and if I miss some point in the first one.
[57:47] So it's really, really hard. And yeah, you don't have to be too rude with yourself.
[57:55] Just let the content flow, and nothing is definitely done. Especially in the digital world, you know?
[58:04] We could also unpublish it if it's not that good, or we could just rewrite it and make another one.
[58:12] I don't know. I really admire people that are blogging
[58:16] for the last 15 or 20 years. Wow, this is just incredible, being
[58:23] able to document their daily work in different kind of articles.
[58:28] Yeah, that's really good. I admire that as well, and it is hard work.
[58:33] So for all of those out there doing that, thank you for doing it and teaching us so much.
[58:39] I will say that I have a lot of thoughts in my head right now that I think if we were to go through websites,
[58:48] I'd be like, I don't know. I feel like I need to sit with it in the fact of comparing
[58:55] them for myself for a bit. And that is something that I've been learning
[59:00] for the entire time I've been learning live, is things may not make all the way make sense.
[59:08] They don't need to. And sometimes we just have to think on it,
[59:11] or as one of my old bosses would say, noodle on it. Just let it sit and passively think of it.
[59:21] And I really appreciate you coming on the show today. Is there anything that you specifically
[59:26] wanted to go over today that we haven't touched on? I guess it's already a lot of things.
[59:33] So maybe it's good to stop it right now. And it was a real pleasure to be here.
[59:43] And yeah, maybe next time we could talk a bit more about something more technical,
[59:49] starting a documentation, maybe covering different parts like front-end versus back-end, which
[59:56] are different kinds of documentation to products. So yeah, let's think about it.
[60:02] But yeah, for sure, I'd be happy to be there for a second one. Thank you.
[60:07] And before we go, anyone listening and watching, do you have any questions before we end today?
[60:15] So I'm still taking notes. Front-end versus back-end, technical.
[60:21] Oh, yeah, you've also given me ideas of how networking is teaching me to code.
[60:28] The power of networking is teaching me to code. Yeah, yeah, for sure.
[60:35] Yeah, I have a lot of people in mind, so yeah. Yes, awesome.
[60:39] I will drop names. Yes, awesome.
[60:44] Well, thank you for joining, Anthony. I appreciate it, because he helps me course-correct
[60:50] when I'm like, wait, these ideas are like, what? And awesome.
[60:55] Then we will schedule again. And thank you, Matt.
[60:59] Bye. Thank you for having me.

