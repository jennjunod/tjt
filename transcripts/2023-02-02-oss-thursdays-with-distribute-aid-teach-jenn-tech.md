---
showLink: "https://www.youtube.com/watch?v=wuNX8NlhM6Q"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "oss-thursdays-with-distribute-aid-teach-jenn-tech"
title: "OSS Thursdays with Distribute Aid & Teach Jenn Tech"
publishDate: "2023-02-02"
coverImage: "https://i.ytimg.com/vi/wuNX8NlhM6Q/maxresdefault.jpg"
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

[00:00] Yeah. Yay.
[00:02] Hello, everybody. How you doing?
[00:04] When, when, I feel like we both don't know what to do when Ramon isn't here. Yeah, I know, but he's on a beach in some South American.
[00:21] Do we remember which South American country is that? Because he's there.
[00:24] Is it a vacation or a conference? It's a conference.
[00:27] Conference. Yeah.
[00:29] Yeah. Yeah.
[00:31] I think he went to Chile. Yeah.
[00:33] That's right. That's right.
[00:35] Yeah. Yeah.
[00:37] Yeah. So he is off doing that and Taylor and I are streaming and we're so used to Ramon.
[00:43] At least I'm used to Ramon just like, you know, introducing us, taking, getting mad. And I love it that I'm just like, wait, who, what are we doing?
[00:52] We can start with intros. I'm Taylor.
[00:55] I'm the director of growth at Distribute Aid Now. We just turned four actually, which just makes me feel super old, but I'm very, very proud
[01:05] of reaching that milestone. And yeah, I maintain our landing site at Distribute Aid and I'm generally involved with the open
[01:14] source tech and open source content that we produce. So that's me.
[01:19] I have a web dev background, but I wouldn't call myself a developer anymore. Aid worker sounds much cooler.
[01:25] Yeah. Jen, do you want to introduce yourself?
[01:29] Yeah. Yeah.
[01:31] I am the host of a couple shows. Teach Jen Tech is how I met Taylor and Ramon and I'm also a developer advocate.
[01:41] And one of the biggest things that I'm excited about is that I'll be working on building out a champion program.
[01:53] We don't really have a name for it yet, like an official name. Our working name is Aid Actually Impactful Developers.
[02:01] Yeah. Yeah.
[02:03] So it's been a little hit or miss if people are digging it or not. And what we're doing is getting started with just laying out the groundwork.
[02:14] And there's going to be a lot behind the scenes yet on Thursdays, you may see the two of us, you may see Ramon and one of us or something along those lines, because we are all working
[02:24] together to get this done, as well as everything else Distribute Aid does, and they are an open source as well.
[02:32] Yeah, no, it's really cool. And I think we've seen lots of like, examples of big tech dev champions programs, right?
[02:40] Like Mozilla Tech Speakers, I know Microsoft and Google and all of them have their own. And I like it.
[02:47] Like what we've discovered is that adding structure for our new contributors helps a lot.
[02:53] So we've been doing these live streams and doing code jams. But even that I feel like, is still in the territory of like, oh, it's cool to submit
[03:02] a couple of pull requests to an open source project, right? We are a great first open source project to contribute to what we want to do is kind of
[03:09] extend that energy by creating a structured program, you know, that gets people to commit to eight to 12 weeks.
[03:18] And you know, it's designed around advancing their skills and showing off their skills as contributors.
[03:24] You know, and also like reaching a milestone, right, I think that like, it's cool to contribute anywhere in open source, but it's really cool if you're like, I built that feature, like
[03:33] me and you know, my friends like handle that one. And that's something that you can really show off to people and we want to thank folks who
[03:41] contribute consistently over time. So building it out in the open, if you're watching the stream today, like, please, please
[03:47] chime in, we read those comments, you know, and we're really building this for you as as potential contributors want to make it exciting for you.
[03:57] So Yes, yes.
[03:59] And I'm going to go ahead and share my screen because we are getting started on a lucid chart to take notes, get us going.
[04:08] And I let me zoom in a bit that way everybody can see it pretty well the overall page. Something that I want to put down here is so name what aid currently means.
[04:28] Actually impactful developers. It's a little bit of like poking fun at Silicon Valley with the save the world mentality.
[04:39] And maybe Yeah, yeah, and the acronym is nice, like aid, aid work. Okay, I want to make this like giant, this one needs to be big, this one needs to be
[04:59] bold, not underlined, I bold, bold, there we go. What did I just paste in there?
[05:07] I should probably whatever link that is. We'll get to that later.
[05:12] All right, so we know, okay, this is just gonna bug me, let me let me and that's all good.
[05:21] I apparently pasted something, we're just going to delete it, it's fine. Delete this, and then no, bold there, okay, that way, I'm not linking to anything that
[05:42] I don't want to be linking to because that would be awkward. So now we talked about it and you said and this is and y'all just so that way, you know,
[05:55] we do have where they already have a repo made for this and GitHub. There's also a discussion board.
[06:03] This is something that I specifically asked for something like lucidchart or Miro or along those lines, because I personally am very visual.
[06:15] And this will help me get like the concepts down and then putting stuff in the you know, words.
[06:22] Right, exactly, like, let's build out the map, right. And then we can describe different points on the map.
[06:28] Absolutely. And what I love is like, we do have that repo, we, you know, it's using the same tools we
[06:32] use to develop code, we're trying to build this out in the open. And so that's another way that you can contribute is like, let us know your thoughts, you know,
[06:41] everything is up in the air right now, we're still figuring it out ourselves. But even when we do, like offline work like this, you know, or we develop stuff on our
[06:52] own, we can upload it to that repo, right, that becomes our collaboration form. So totally great idea to, you know, use lucidchart, start building that map, and then we can just
[07:03] export it at the end of the show and add it to the repo. And if we want to iterate on it, we can make some updates and, you know, update the file
[07:10] on the repo. Like I said, repo 20 times there.
[07:15] Okay, I'm arguing with this, this, this one. So I'm just gonna make that go away.
[07:22] Also, y'all, in case anybody wanted to know, this is my first time using lucidchart. So it might be me arguing with it.
[07:29] Yeah, and I can definitely help navigate you, Jen. But I do need to know what direction you're going in as the driver.
[07:37] So we're looking at maybe right now, the length of the program and how we want to structure that over time.
[07:42] I feel like there's a few different dimensions. There's like people, right?
[07:45] Yeah. I just wanted to put like, 10 weeks.
[07:49] Yeah, it doesn't let me like, you know, maybe if you do a shift enter or something like a soft line break.
[07:57] Yeah, that's good. Cool.
[07:59] You're so smart. Yeah.
[08:01] Like, why is this? Because I'm used to Miro.
[08:04] And I'm like, I just want it to be like, even if these aren't like solid, just like some things that we've talked about in the idea, which length is 8-10 weeks.
[08:18] And I feel like that length, there's an important bit there, which is the cycle, right? We want to run this program on a quarterly cycle.
[08:26] And that kind of winds up with like some of our other activities at DA and our quarterly and annual planning.
[08:32] And so that 8-10 weeks is important. We don't want to do 12 weeks, right?
[08:36] Like if we were full time, if we're paying you, Jen, sure, we could do 12 weeks and you get a week between each cohort.
[08:42] But since this is a volunteer effort, I think it's important, let's give ourselves like a few weeks off between each cohort to rest, recuperate, you know, kind of prep for the
[08:51] next one. Exactly.
[08:53] Yeah. And maybe there's something there.
[08:55] It's like eight weeks of structured time, and then a final project for four weeks. So we could look at breaking it up in a couple of different ways of like, here's the like,
[09:04] very structured component. And then, you know, here's more of a independent final project for a few people to work on.
[09:11] You know, if we wanted to extend the program, like for that, closer to that 10 to 12 week mark.
[09:18] Now, I'm just having fun with shapes, but... Oh, there's so many shapes on Lucidchart.
[09:23] There's more shapes? There's a whole shape library down there.
[09:26] Yeah. What?
[09:28] The button at the bottom. And they got like swim lanes and things like...
[09:31] Oh, this is going to be fun. All right.
[09:34] I probably shouldn't get this distracted with them, but I'm very excited about it. Okay.
[09:39] There's so many fun ones. Yeah.
[09:42] There's a lot of corporate ones. Like some of the AWS architecture doesn't really make sense, but...
[09:48] There's colors. There's color bubbles.
[09:51] There's color bubble. We're going to use some color bubbles.
[09:53] This is fantastic. Okay, now we need a type.
[10:00] Types are up here. There we go.
[10:03] All right. So we have...
[10:05] What are the channels or verticals, however you want to call that, for... I'm calling them tracks is what I'm using.
[10:16] So yeah, I think I don't want to overdo it at the start. I feel like...
[10:21] Let me just kind of brain dump what possible tracks there could be, and then let's think about if those make sense, right?
[10:27] Because we can start off with a couple of tracks and add more tracks in the future. So what comes to mind here?
[10:34] I feel like on the frontend side, there could be a solid frontend track or two. Maybe kind of general website.
[10:46] We got a few things going on on the site, right? So on the frontend, there's this concept of generic pages, right?
[10:54] Which is like pages that our team can basically say, "Here are the components I want listed on the page."
[11:01] And so that could be one track is building out more components, like adding... Right now, just title and text.
[11:07] So can we add a YouTube component where our team can just go into our CMS and click, like, "Add YouTube component."
[11:13] Here's the YouTube URL, here's the video title, and there's no custom coding. It just says, "Oh, when you get component data that looks like this, render a YouTube
[11:22] video here." So I feel like that kind of generic pages...
[11:26] And that probably relates to just our kind of custom pages, right? Things like our region pages and stuff.
[11:35] We can kind of get some custom pages up, data-driven pages, and then take those components and transform those into generic pages.
[11:42] So I feel like that's like building out frontend components. And that would be kind of holistic, so that would include frontend testing, that would
[11:49] include maybe some data architecture of how to structure things for the frontend. It's not just going to be, like, make pretty things appear on the webpage, but that would
[12:00] be more of the focus. I feel like there's a related frontend track, which would be visualizations, right?
[12:10] So we just launched our first big visualization tool, and you can find that on our website if you go to distributeaid.org and click on the "Needs Assessment."
[12:21] >> Wow. We're going to just Google it, because...
[12:29] >> There we go. >> We were trying to type.
[12:31] It wasn't working very well. >> So if you click on "Needs" there, that will take you to our Data Explorer.
[12:39] Exactly. And so this is really good.
[12:42] We have enough data at this point about our supply chain, about our partners, about their needs.
[12:48] And the trick is we use that all the time internally. So we use this Data Explorer to know which in-kind donations to go after, or set up aid
[12:56] swaps between groups that each have extra some things that the other needs, right? And what we want to do now with this Data Explorer tool is we can list the top needs
[13:08] for each region, right? So you can just explore all the data through the Explorer, or you can look at it, sort
[13:14] by top needs in this region. If you're planning a collection to help Ukrainians right now, what are the Ukrainian groups saying
[13:22] they need? So on and so forth.
[13:24] So I feel like there's more data from our needs assessment. We have impact data, like how many people are you reaching?
[13:32] We have infrastructure data, like how much warehouse space do you have and what capacity is that?
[13:38] All of those would be great to create visualizations for. And then we're working on releasing a new dataset, which is our shipping data.
[13:46] And I think that combination of like, here are the needs, here's our shipping data. How much did we meet?
[13:52] If we can get that going, that starts to set the stage for DA to grow beyond our own supply chain efforts.
[13:59] But eventually the goal would be to collect data from our partner shipping as well. So it's like this refugee aid movement, here's what we're all doing together.
[14:08] Here's the total needs, where are the gaps, let's hone in on those, right? And using visualizations to make the data actionable, I think, is going to be a really
[14:18] important thing. Yeah.
[14:21] So I feel like that's another track right there. Visualization or just like data?
[14:29] We talked about two different things right there. Yeah.
[14:34] I think that would be a good one to pair people up. I think for visualizations, there's like the data side, right?
[14:43] So importing data from an API or from a JSON file or something, processing that in Gatsby to like expose it correctly through the GraphQL API and getting it like to a front end component.
[14:56] So that'd be a bit more backend work there. And then there's the actual like creating the visualization.
[15:01] So I feel like a visualization track would be great for a couple of people to pair up on, someone who's more interested on like the front end visualization side, and maybe
[15:10] someone who's more interested in like the kind of data management and processing side. I'm seeing if I'm computing this well, because I feel like there's different things going
[15:28] on and I like doing height. Like if somebody was to look at this and be like, "Hey, I want to do like all these, you
[15:37] know, fill in the components and stuff." I don't think somebody that is newer would necessarily understand that, where they might
[15:46] understand like data or visualization. I feel like we're going to need to get a page in that GitHub repo for each track, right?
[15:55] So like as long as we understand that we can plan the tracks out, but then I want a page like we have examples of all this in our code base.
[16:02] So let's link to code, let's link to like code seed maps, highlighting the right files to look at.
[16:07] Let's link to like screenshots and examples of like, "Oh, you could build something that looks like this."
[16:12] And it's like a screenshot of a visualization or a screenshot of a component or something. Yeah.
[16:19] What else here? I feel like we could use a testing track.
[16:26] I think that that's like probably, you know, something that could support the other tracks. There's also like some, for legacy reasons, like we have untested code, you know, there's
[16:35] plenty of that. And that could be interesting looking, you know, an interesting experience for someone
[16:41] going through like data testing, going through end-to-end testing, going through kind of like unit testing at the kind of functional level and at the component level.
[16:54] And so that could be a track that like both supports the other tracks, like fills in tests that we don't need to fill in and provides a well-rounded like JavaScript testing experience.
[17:07] These are just questions for myself to go research, not necessarily for like you or anything like that.
[17:15] It's more of like, "Let me go research this later because I'm not going to think about it right now."
[17:21] I feel like we could get you connected, you know, since this is like a feel-good open source effort.
[17:26] Like we could probably reach out to, you know, the big corporate programs and actually get you to like talk to the people, you know, running those for some of these questions.
[17:37] Right. Right.
[17:39] Yeah. What else?
[17:41] So are you wanting people to just for like front end to also just being able to like fill in information or do you want them to create it as well?
[17:53] No. So we have all of this stuff, like we already have content in our CMS or working on like
[18:00] data pipelines or something. So we've spent a lot of time figuring out how to empower our content contributors.
[18:09] So I think that what you might see is like there's this wonderful guy, Weston, he's our head of projects and administration, and I meet with him to kind of talk about, you know,
[18:19] maintaining our tech projects once a week. So Weston might work with you to define like, you know, what should the fields in our content
[18:28] management system be, right? Like what information do you need?
[18:32] And then he'll work with our content team to produce that. But yeah, content, if there's someone interested in like content copyright, I might throw design
[18:42] in there. I'm not sure how if that would be a big enough track just by itself, like just for content
[18:49] or copy. Yeah, like a presentation, like a presentation track or something.
[18:55] Hmm, how? I agree with you.
[18:58] I'm also thinking like, content and copy makes me think like, because it would be really helpful if people learned how to do blogs, how to, you know, and that's what I'm thinking
[19:14] with content where like, with design, I'm like, design is kind of cross cutting a little bit.
[19:23] Yeah. So I'm just gonna put it out there and not overthink it.
[19:27] We're just gonna put it. That's cool.
[19:29] Yeah, we're just getting ideas down. Now we can decide like, which ones make sense for us to move on versus not.
[19:34] One of the issues with content, though, is like, this is why we've kind of created things that are like separating the content from the devs a little bit is that we want to encapsulate
[19:45] like the complexity of our content space with those content creators. So I think a content track would like, also involve a lot of like, training about logistics
[19:56] and things like that, which is not super relevant to contributors, like dev or kind of contribution experience, but would be much more relative to like, our logistics coordinator.
[20:07] So what I could see here is like, the logistics coordinator should create guides and create content, but maybe someone needs to work with them on like how to structure that.
[20:15] So they don't write like a 30 page report or something like that, and then try to hand that off to our devs like, Oh, just make it show up on the website, like, no, like, you
[20:24] got to break things down, we want it to be repeatable, you know, things like that. I think one of the big things to add to that point would be also still showing people that
[20:36] they can contribute without it being development too, because you know how we talked about that during like Hacktoberfest.
[20:44] Yeah, the non-technical contributions are so important. So I guess that's where I was thinking with the content copy, but I totally getting what
[20:55] you're saying too. So yeah, what about something like and we can leave content copy up there is like a
[21:02] potential thing. I just wanted to highlight kind of, you know, where my thoughts were at on it already.
[21:07] I feel like a maintainers track would be really valuable. Like are there one or two people that would like to, you know, again, kind of support
[21:14] the other tracks, but also help us like, get issues kind of, you know, like review PRs like, and that could be more technical or less technical, I think.
[21:26] But just the, the maintenance. Yeah, like project management, open source maintainer, sort of like activities.
[21:44] And then that would be a good one to like, we, our needs assessment software is like pretty set.
[21:52] We don't need to make too many changes to it coming up here. But we are looking for someone to become the maintainer for that needs assessment project.
[22:01] So kind of talk to the team once a quarter, make sure the surveys are up to date. You know, if there's issues, like for whatever reason, you know, kind of be responsible for
[22:11] for taking point on them. I'm not sure if that's a good thing for this program, though, or if we should just like
[22:16] find someone who just wants to kind of like adopt that as a side project. I would think adopted as a side project, but teach people how to be an maintainer.
[22:27] So that way, as things grow, you actually have people you could reach out to later on that already know distributing.
[22:33] Yeah, that might be the way is like someone adopts it as a side project, but we still have a couple of people, you know, like looking at it, learning about it.
[22:43] Let's see, and then I'm almost wondering if there needs to be like a front and back end kind of breakdown and then going through there.
[23:03] But at the same time, I'm like, I don't think people like when they first start, they necessarily know what front end and back end is.
[23:10] Yeah. And I'm not sure we don't have like a real back end.
[23:13] Like we have that Gatsby layer, right? So that ingests all the data, processes it and exposes it through a GraphQL API.
[23:20] But we don't have like a server. We're not necessarily building, you know, our own API layer, we're just using Gatsby.
[23:26] So that's where I feel like the experience, you know, for front end, like, you can be more into the front end side of front end, or you can be more into the data side, you
[23:35] know, and that's fine, but you should probably own the like, data coming and being transformed in Gatsby, because that'll directly affect like how you build the components, right?
[23:46] I want to minimize like, communication overhead and kind of like, you know, the potential for things to go in different directions and create conflict.
[23:54] Same thing with visualization is like, you know, processing that visualization data is going to be key to making those visualizations in the right way.
[24:03] And I think that also gives people like a bit of that variety of experience where like, you might prefer to do like making the visualizations, but you also get some experience thinking
[24:12] through data architecture as like a part of that track, right? Yes, because what I'm also thinking right now, too, is being able to show like, which
[24:30] ones may go together and be their own separate tracks. Like the data and visualization would complement each other, for example.
[24:39] Yeah. Or maybe like front end and content copyright, you know, that might be like a combined track
[24:44] at first, and then we split them up later or something. Yeah.
[24:48] Because then we also have the project management, just kind of thing, yeah, goes over here. And then chair, chair, whatever.
[25:07] And then design probably goes over here, too. Yeah.
[25:12] I would think. Yeah.
[25:15] I'm going to delete this one for now, because I think the other thing that if we're good here, other than me, like trying to like, just make them really pretty, and add to this,
[25:33] I definitely will say, y'all, I spend way too much time on like this stuff. Because I'm like, I just want it to be pretty so I can read it.
[25:44] Yeah. And there are definitely things that we could do to make that easy.
[25:48] Like if we wanted to set up swim lanes, for example, to kind of create like rows of things, we could have the tracks in the left hand column, and then like the progression through
[25:57] those tracks going across or something. So I feel like there's definitely some good tools in Lucidchart.
[26:02] But it does take a bit of fiddling to like, have figure out what the best layout and stuff is.
[26:07] Right. Now, something that we talked about, but we haven't fully talked about that I want to
[26:15] put on here is also, what is your timeline to have this like the first cohort? Totally.
[26:25] I think that I would like to kick off the first cohort in Q2. So starting, you know, April 1st kind of deal.
[26:34] And the thinking behind that is like, I want to give us plenty of time to build out the program.
[26:39] We're also going to have to recruit the program, right. So we can kind of build it out over two months, we can recruit for it for a month.
[26:47] And in the next like, month, month and a half, we're going to be making some like, larger upgrades to our dependencies, we have to swap out our content management system to like
[26:58] the new version, you know, that the company is producing, we might make some other changes, I need to bump up like the node version, so we can upgrade to Gatsby five.
[27:08] So I feel like that's not a good time to like start people in the immediate future. But let's give ourselves a couple of months spec this out, focus on setting the groundwork.
[27:19] You know, creating the examples we need to like creating the code, see maps, we need to and then and then we can we can set people up, right.
[27:28] And I feel like that prep time is going to help us like when the program's running, like, you know, it should all be specked out.
[27:35] So there's not as much like short term kind of high pressure maintenance work we need to do to keep it running.
[27:41] Yeah. And something that I think really helps with visualization, especially if nobody's ever
[27:47] done a project like this, or project management is what the questions that I'm asking Taylor are basically, what are you thinking of?
[27:58] Like what like, none of this is like a full thought out process yet. We're like, we're not going to jump there.
[28:04] But knowing about the program, knowing about like, okay, is our goal to launch Q2, I'm just put Q2, April launch, Q2 is multiple months, what goes into that.
[28:22] So it's going to be knowing the tracks. Yeah, like specking those out totally.
[28:29] So we need to know what tracks, what goes into the tracks, who's our audience, because we have an idea about it, but we don't fully know, like, we need to be able to.
[28:48] Yeah, and we'll want to specifically recruit people who commit to the program, you know, for each of those tracks.
[28:58] Absolutely. Recruitment, what is the acronym, it's like, what do I get out of this?
[29:13] Like, Oh, I'm just calling it like, thank yous or rewards, maybe like return on investment is
[29:19] what you're thinking. I'm just going to put attendee ROI, and then writing out like, DA ROI, like making sure
[29:38] that that's public as well, like, getting that solidified to people fully understand what's the mutual aid here, like we get structured contributions and a certain commitment, you
[29:49] get, you know, learning through doing and, you know, LinkedIn, shout out posts and support, I'm like the job hunt or something, right?
[29:57] Like, yeah, yeah, definitely important to think through both sides there, make sure that it's aligned.
[30:03] And like, we're mutually supporting each other. And then I would say, like, the big final part of this is, um, well, it's not final,
[30:14] it's not, it's not, it's not, I don't know, like, I don't, I don't, I don't know, I don't know how to spell it.
[30:25] I don't know how to spell maintenance. I always have such a hard time spelling maintenance.
[30:27] I don't know if that's right. But, you know, whatever.
[30:29] It does have a lot of weird vowels in it, like random places. I can never spell it.
[30:31] I don't know why. Um, and then also like, how and y'all, I 100% appreciate this about Taylor, but it still
[30:40] needs to be on here because not everyone is in Taylor's head of how do we talk about it? Of like, what is the program, uh, doing the, you know, the who, what, where, when, why,
[30:52] what is distribute aid? What is this program?
[30:54] You know, how can we connect the tech work people do to like, you know, actual aid getting delivered?
[31:01] Right. Like, what's that like kind of impact point totally.
[31:06] So there's a lot of questions that we'll be solving through each, maybe not all of them on streams, but a lot of them, like, um, when we're doing, uh, like a lot of times Taylor
[31:21] and Ramon will do like coding things. I'll be working on my stuff at the same time, even though we're streaming just so that way
[31:27] I can ask questions as I'm going through because, uh, that is something that like, why do we not have a backend track being able to answer that?
[31:37] Oh, FAQs. That's going to, that's also something that needs to be developed, uh, location.
[31:47] Yeah. I think the location is a hundred percent going to be remote, but I think there's sub
[31:53] questions in there, um, because people need to collaborate on time zones. So it'd probably be better to group like, you know, different people on the same track.
[32:02] Like roughly in the same time zone to make it easier for them to communicate and collaborate. Right.
[32:08] Um, that's not necessarily a hard rule, but we should think about how location, you know, in a remote contributor context, like affects people's ability to contribute and coordinate
[32:18] with each other. Yeah.
[32:20] And I think that's so cool. And this is why I love doing this live because y'all, I said location.
[32:26] And in my head, I was thinking of where are people going to go through these tracks? Like how are we going to process it?
[32:33] And you thought like physical location and this is like a huge thing on what happens with these, like when you plan these projects, like this is like a big part of projects of
[32:47] going like what words mean the same thing, but then context is everything. So I love that that actually came up because my hope of us doing this live is also people
[33:00] see how to work through a project because it's such a, a skill set that you have to learn.
[33:10] Yep. And also doing that with like a bottom up approach, right.
[33:13] Instead of like a top down and kind of command and control approach like, um, I'm going to do location and then do, what would I call this then, um, for where we're doing the train,
[33:35] not trainings, but the kind of trainings, but not really like how are we, yeah, yeah, I'm not sure on, on that yet.
[33:43] I'm going to say LMS for now. That means learning management system.
[33:48] Okay. Um, just so that way I remember that it's like a thing that needs to be figured out.
[33:55] Not that it's necessarily, cause y'all, this is something that I think is a really good call out to, uh, um, I kind of want to, I don't want questions.
[34:07] I kind of want statements. Let's do, let's start our own, uh, FAQ thing.
[34:14] It seems all we're really doing is we're like diving into like, how do the individual pieces of this work.
[34:20] And if we make those statements, we'll be able to review those statements at the end to make sure they like all align with each other.
[34:26] Right. We can kind of like build up each piece by itself so we don't get overwhelmed and then
[34:30] do like kind of a review and alignment sort of phase. Oh, my mic.
[34:35] I really, I hate my mic being in my camera, like, so I have it off to the side, but then I can't see my full screen, so I feel like, uh, I'll do that.
[34:47] So statements. So, um, I'm going to add like, why no backend in there because, well, it's because the Gatsby.
[34:57] Um, and then for like, why are we not calling this training? Like you, you said this so well, like a few months ago and I'm just like, so we don't
[35:10] have the capacity to teach people. They're much better programs out there.
[35:15] If you want to learn how to code, um, I think that everyone can learn through contributing to DA, but that's going to be in a practical, like action oriented sense of like, you know,
[35:27] let's talk about, let's talk through an issue, right. Come to a, come to a code jam or, you know, maybe through the tracks, like let's like
[35:33] build that understanding together, but you gotta be able to go out and like write code to, to move the needle on that issue on your own.
[35:40] And then there's another round of learning during the PR process, right. Where like, we'll double check your code, we'll talk through anything missing so that
[35:46] you can learn about it. Um, we do these work in progress PR so you can get feedback, you know, before you're
[35:51] ready to submit, like as you're building it out. Um, but I just want to be very clear, like I'm not trained as an educator and this is
[35:58] not supposed to be an educational program. Um, this is probably a great next step, right.
[36:04] For people coming out of bootcamps that no react already, you know, maybe still need to learn typescripts, but you can pick up typescripts like as you go on a project.
[36:13] Um, but yeah, yeah, there's gotta be a certain level of like, you're ready to contribute. And then this is like a good capstone, you know, on that educational experience or a
[36:23] good way to show off a new skill you're, you're learning, you know, before you try to get that next job or something like that.
[36:32] I just want to be clear about that because I don't want to do people a disservice. Right.
[36:44] Or like, you know, I'm excited about the wrong thing. Yeah.
[36:48] And, um, and I think it's something that a lot of people may still associate it to the same thing, meaning that like what you just said, I'm like, oh yeah, I'll gain experience
[37:01] and I'll learn. But that doesn't necessarily mean training.
[37:05] Yeah. Um, and I think, so do you think experience not training is a good way of summarizing
[37:12] that? Yeah, I think so.
[37:14] I think you learn by doing with this project, right. That learning will happen.
[37:17] Um, you know, but we are not educators. We are not here to train you, like teach you how to code or something.
[37:24] Um, we're here to create a like safe and like approachable environment for you to hone your skills like while making meaningful contributions.
[37:32] So I think that really captures like the idea there. Okay.
[37:36] So if we were to define a track, not like, like what would you want somebody to get out of a track?
[37:45] Like they come in not knowing, choose any of them. I don't care which one.
[37:49] Um, but if you were like, yo, I really want them to be able to do X, Y, Z when they're done with the track.
[37:56] Do you have like an idea? So let's say like for that, that kind of front end track, right.
[38:03] You might come into it knowing react and, um, like CSS, right. Um, and, uh, um, JavaScript obviously like through react.
[38:17] So like if you know, react and CSS and have like a, you know, basic idea of like what web dev is, right.
[38:23] You can pick up typescript as you go. Um, that's not going to be that hard.
[38:28] Maybe you also know testing like unit testing, right. So like react CSS unit testing, those are usually core concepts covered by a bootcamp.
[38:35] You'll pick up end to end testing as you go. Um, and, uh, um, you'll pick up like Gatsby, right.
[38:43] So you'll learn a couple of new frameworks. You'll learn, you know, uh, a new like derivative language.
[38:49] Um, you'll expand your testing knowledge. Um, and I think that like what that looks like is what it looks like when you first
[38:57] start any job, right? Like you're not going to know all the technology that you use at that job, but you should be,
[39:03] you know, like, like your skills should be there where you can pick that up as you go. And so I think that this offers like a very practical experience for, uh, for like what
[39:13] getting a new job and getting on board into like a new tech team looks like. Um, so incoming, they know like react and CSS, what web dev is, but like, and they know
[39:24] a bit about testing. Yep.
[39:27] I'm going to say like high level, maybe not. Yeah.
[39:31] Like, like, have you written a unit test before? Do you understand like what testing is, you know, but like, you don't need to be like
[39:37] a professional tester or anything. Okay.
[39:49] And then outgoing, um, you said that they would learn like Gatsby, they would what were the other ones?
[39:58] TypeScript. Um, probably Tailwind as like a CSS framework, um, they'll enhance their knowledge on testing
[40:09] like end to end testing maybe is something folks like get less experience with, uh, kind of like new greenfield projects, um, yeah.
[40:22] And then they'll also be more confident, right? It's just like the non tangible, like, you know, but like, you'll be able to approach
[40:27] like a blank page and kind of know like what components might need to be going on there and how to lay it out and stuff.
[40:33] Um, so just kind of that general, like, Oh, I've done this a few times before. Like I have some confidence I've done it in a environment, you know, not a toy projects,
[40:42] but like a real thing that's live and people are using, um, yeah. And then I think there's like a number of like, less like learning related kind of outgoing
[40:55] benefits. But we can do things like a LinkedIn recommendation or a, you know, certification of completion
[41:02] or something like that. Right.
[41:04] Um, you know, to highlight the, you know, the fact that someone made it through this program and what they accomplished.
[41:14] Okay. And I know like, this is all like this spit ball in here and this makes sense.
[41:26] Um, so let me grab some arrows. I want some arrows.
[41:32] Give me some arrows. Okay.
[41:39] Oh yeah. We can do it.
[41:41] No, that didn't get close. You might need to click on the front end box and then, yeah, there you go.
[41:47] Wait, this one? Yeah.
[41:49] Okay. You know what?
[41:51] We're just going to delete it. It's fine.
[42:01] We'll go back and do it later because I will get like really, um, so you just need to like get some practice with the mechanics of lucid charting.
[42:11] Yes. Yes.
[42:13] Cool. This way.
[42:15] So whatever you're not getting any arrows right now. So we'll just do this there, there.
[42:22] So what are they doing in between? Are they like, how do we structure like, and I'm, I'm just spit balling on this one of
[42:30] like they need to do X amount of projects. Like what are you thinking that, yeah, so I think, um, what would be great for something
[42:40] like the front end track is like, we should come prepared with a number of issues. And I think like a week by week approach would make sense.
[42:48] That's like a good cadence where people have some flexibility, you know, but also like are expected to like make some progress each week, um, to prevent situations where people
[42:57] like don't do anything for a month and then have to catch up a lot. Right.
[43:02] Um, it also facilitates like, you know, things like, um, multiple people on the same track can get together once a week and kind of support each other, like join a co-gen at the same
[43:11] time. Um, so the types of issues here would be, you know, maybe thinking through a theoretical
[43:17] progression, like, um, we have, uh, images for those generic pages. Like the data is already there in our CMS.
[43:26] We don't have an image component, you know, so week one might be like, you know, review existing code, get familiar with like how the generic pages work, right.
[43:38] Maybe write some tasks or, you know, do some like lightweight stuff to like show that knowledge, right.
[43:44] Um, week two might be, okay, let's focus in on this one component and let me go ahead and build out like importing that into Gatsby and exposing that through the Gatsby GraphQL
[43:56] API. Can I take this YouTube data in the CMS and get like a YouTube component node in Gatsby's,
[44:04] you know, GraphQL API. Would you be wanting them to just like find a component that just works or would you want
[44:13] them to build it or like. So this isn't even a component level.
[44:17] This is just the data level, like data exists in the CMS. We need to load that in the Gatsby and expose it through the Gatsby API.
[44:24] And that would be something I'd expect them to write, right. It's like, can you grab this node?
[44:29] There's example code, you know, so like do the same thing we do for titles, but do it for YouTube, right.
[44:35] Or images or something. Um, yeah.
[44:42] And then week three might be, uh, you know, like, um, like building the component. So building that image component or building that YouTube component and making sure it
[44:52] works on the existing generic pages, you know, based on, on what those are. So that kind of, you know, in three weeks that completes one like component that you've
[45:03] developed end to end. And then I think like we can repeat that cycle.
[45:08] Maybe week four is like testing or something, you know, give people the first month to like get their hands dirty with the, uh, the first one and kind of figure it out.
[45:16] And then I think we want to, now that they've like had the time to figure out that development cycle, right.
[45:22] They got their first component launched. We want to accelerate it.
[45:25] So maybe then it kind of gets into two week chunks. You pick your next component, you got two weeks to like get the data in, build the component,
[45:33] get it reviewed and out the door. Um, you know, we repeat that for the next month.
[45:38] Right. Um, and this would all be kind of driven by, you know, what the existing needs are.
[45:45] People kind of set up the issues maybe in the last, you know, a couple of weeks or something. It's like, Hey, like now that you've done this a few times, what do you want to see
[45:53] on the website? Like, can you make your own issue and, you know, ask for new content from our content
[45:59] team to get a cool component up there, right? Like if you want it to upgrade, you know, images to galleries, right?
[46:07] Can you define what, how that works and what that looks like? Tell the content team, Hey, instead of uploading one image, I need you to upload a bunch of
[46:14] images for this page or something and build out a gallery component, but have that be a little bit self-directed, you know, um, on the, uh, on the tail end of the program.
[46:32] Um, something that comes to mind that, uh, the problem, not the solution, but the problem of creating consistency for people going through the program.
[46:47] Yep. So I'm gonna put that over in my questions.
[46:52] Yeah. And I think that's it.
[46:54] Right. I think what we've seen so far is like lots of people make it through that first cycle
[46:58] and they'll like get their component launched or something or get whatever they're working on launched, but then they don't come back to repeat the cycle and really solidify what
[47:08] they learned, you know, solidify. All right.
[47:11] Because it's always so much easier once you figure something out, like go do that a few more times and it should be easier, but you get to work on different things, right?
[47:18] You get to like, if you're like learning about some of these new languages or frameworks as you're going that first time, like the second time around, you should be able to
[47:27] test that knowledge and kind of validate that, you know, and like not get stuck where you got stuck last time.
[47:32] So I think that's part of this is like, I feel like we do a disservice to people without the structured program.
[47:37] Cause they come through, they make their contribution, they feel good about it, they move on. It's like, well, like spend that extra month, like doubling down on that.
[47:44] Right. You know, getting a few more things out the door.
[47:49] Yeah. Yeah.
[47:51] So what I just added up here, I don't know if you saw it, was how to create consistency of the program for each cohort while thinking of DA's needs, because it's like, you need
[48:02] to think of both, but like if we were just, so for example, for those who may be unfamiliar with any of the like champion programs that companies have, a lot of times they are just
[48:17] like the same workshop or the same program or the same examples that they go through for a lot of them and how to do that because on these bigger companies, they may not necessarily
[48:31] need help. They just want people to be like, Hey, you do X, Y, Z.
[48:36] So maybe like better for hiring or an ambassador or something where for DA, I think it's very important.
[48:45] So it's a practical need as well. So maybe that's a bit of like mixing in, you know, the two, maybe, maybe like week one
[48:53] through four is the same for everyone. And then the repeats are, you know, well, I think that's where the idea track comes
[49:03] in. Right.
[49:05] I don't think people should be working on literally the same code because that's like, that doesn't advance if like three people make the YouTube component, like that doesn't
[49:13] really help us. But what we could do is like, if we get two or three people in on the front end track,
[49:18] you know, it's the same process, right? We all meet once a week, right?
[49:22] You know, and we kind of guide people through that first month, you know, using those meetings to check in with folks, and everyone gets their component and like works through it,
[49:32] but they can also like collaborate and support each other, you know, would be the idea. So I think that, like, can we make the process consistent, even if the content is like a
[49:41] little bit unique, so that people are making like their own contributions. And you're probably right, it's like the first month is going to look the same regardless
[49:49] of what track of like, do this chunk, then do that chunk, then do this chunk. And now you're like wrapping up with testing and reviews, and you got a feature out the
[49:57] door, right? And then from there, it's like, okay, we don't need to do as much handholding or as many
[50:02] check ins, you know, let's go back to that, like two week cycle and, you know, complete some of these chunks together at the same time or something.
[50:14] I do think it would be a really good idea to have at least two people on each track so that they can support each other.
[50:22] And also so that we have some like backup and resiliency in case someone can't complete the program.
[50:29] Excuse me, Kiona has decided to brace us with her presence. Are you going to come lay down?
[50:52] So for those who may not know, I have a bulldog, and she likes to be annoying. She's 12.
[51:02] I don't even know. You're not even looking up.
[51:04] Look up. Hey.
[51:06] There you go. Wait, there we go.
[51:08] There's the dog. We'll see if she, now that she's in here, if she decides to play nice.
[51:19] Okay, so doggo aside, hopefully she just lays down and chills out. We were talking about at least two people per.
[51:34] So I think that's right there, like two people on track for, you know, for them to support each other and also for us to have some resiliency.
[51:44] I don't know if resilience, like I get it in context, but if I go back and read this, I'm like, I don't think I'm going to know.
[51:59] So basically like if it doesn't work out for someone, are we canceling that or if there's another person there, we can like, you know, keep making progress, right?
[52:10] Like that kind of like, there we go, there we go, it'll be, the statements will be better later on.
[52:21] Yep. No.
[52:23] That's cool. I didn't know you could do bullet points in the, neither did I, I didn't mean to.
[52:33] So that was cool. Cool.
[52:35] Oh, it's because these ones don't have spaces. Ah, so if you do the dash and then the space, it's kind of cool.
[52:46] Oh, now you got to go do this to everything. So I think that, that one didn't do it, right?
[52:55] Maybe it's a space ahead of it or something. Probably.
[53:00] I think this is a really good start on everything. Do you think there's anything on here just as like the basics of what you're envisioning
[53:09] on the program that is not currently on this? I feel like we have a good idea of like, you know, what are the tracks and for every track
[53:18] we can build them the same way where we have certain expectations for folks coming in. There's like a progression pathway that we can define ahead of time through the track,
[53:27] you know, and there's like, here's the like leveling up and, you know, kind of thank you. So you'll get after completing the program.
[53:34] So I feel like the tracks, like we got good ideas there. We got an idea for the format.
[53:40] What I'm not seeing here is the people, because it's going to take me more than me, you and Ramon to run this.
[53:46] Right. So I think we should think through like, what's our ideal setup.
[53:49] One thought I had there was that every track should have like a mentor, you know, some like mid to senior level dev that is not responsible necessarily for contributing code to distribute
[54:00] aid, but is responsible for supporting the people going through that track and maybe meeting with them once every other week, you know, kind of hosting an office hours for
[54:09] that track or something. But I feel like that would be a great way to connect more experienced devs with folks
[54:15] that are like, still kind of getting their feet in the industry in a way that like, isn't asking the more experienced devs to just like do more coding that they do at work.
[54:26] It's a bit more fun and exciting and, you know, like, feels better for them. So I feel like that would be a good reach goal.
[54:34] Obviously like I can take a track, I'm sure Ramon will take a track, I don't know if you want to take a track, Jen, but I feel like maybe you shouldn't because you're going to
[54:40] be like, looking at the program as a whole, which means that we just need like a couple more folks that want to, you know, have that once a week meeting, you know, office hour
[54:50] style to, to help folks progress through the track. Yeah.
[54:55] Yeah. And I think that is, I'll work on that later.
[55:00] But every track would have a mentor to allow for office hours and mentorship. I think that's a great way to summarize that eventually.
[55:08] And I think something that I'm really excited for is for the streams, it's basically like, let me info dump so that way by next week I can work through all of this.
[55:20] That's exactly. Yeah.
[55:22] Yeah. I feel like like next week, you know, I can be getting some more time to play around with
[55:25] Lucidchart. We can kind of like present this in a structured way and that's where we can really engage
[55:29] our audience. You know, what do y'all think?
[55:31] Like, does this see any red flags we don't, or, you know, do you have any preferences? By the way, to our viewers, please do chime in.
[55:38] I am checking the, the comments and stuff and your feedback is certainly appreciated. Yes.
[55:43] Yes. Agreed.
[55:45] Agreed. Agreed.
[55:47] Agreed. And something else that behind the scenes, I will start meeting with more of the DA team
[55:52] and learning more about it because this, I might have more experience with yet at the same time, I'm not as familiar doing this for developer tracks or for with DA specifically.
[56:06] Specifically. I can word.
[56:11] And I think this is just a great way to get started. I know for myself, that was a lot of what I wanted to get out of today.
[56:19] Is there anything else that you wanted to add? I know we're cutting our time short.
[56:23] I'm feeling pretty good, honestly, and I don't mind, you know, keeping the stream to an hour here.
[56:28] Like I think that, you know, we got some structure and you just got access to our tooling and our kind of internal spaces.
[56:34] So yeah, I think it's probably best to like take this, run with it for a week and let's check in next week, see where it's at.
[56:42] Very cool. Very cool.
[56:44] Well, thank you everyone for joining today and next week we will see you again and have more structure for you to have some input, which I'm going to tell your friends, be sure
[56:54] to show up. Start getting excited.
[56:56] If you want to join our program and help us build it out in a way that's right for you. So.
[57:01] Yay. Thank you.
[57:03] Cool. 
