---
showLink: "https://www.youtube.com/watch?v=baB7cyCwk-E"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-data-modeling-with-leo-guinan"
title: "Teach Jenn Data Modeling with Leo Guinan"
publishDate: "2022-09-13"
coverImage: "https://i.ytimg.com/vi/baB7cyCwk-E/maxresdefault.jpg"
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

[00:00] Hello, beautiful humans. Welcome back to another episode of Teach Gen Tech. And I will say, I think this is the first time I actually started it right when it said to go live,
[00:12] instead of me going, "Oh, shit, we forgot something. I need to finish this thought." So welcome back, Leo. For those who didn't join last week, we talked a lot of theory of data
[00:25] modeling. And we stumbled our way, ooh, I have flying pens. We stumbled our way into me finding out that I could really use a data model for my podcasting process and creating
[00:42] content for that. So we are going to use that as an example. And we will, yeah, that's where I got to. And Leo, please introduce yourself. >> Yes. So I am a software engineer. I'm
[00:58] currently with Copy AI for kind of the day job and then building a number of products on the side. I'm also kind of an all around creator, working on a book, podcasts, plural, YouTube channels,
[01:11] a little bit of everything. So if you want details on any of that, you can check it out at Twitter. That's probably that's where I'm most active and kind of it's my hub for everything. But yeah,
[01:23] happy to be back. It should be fun and practical. >> Yes. And I think that's one of the best parts about this show is it is a lot about theory, but a lot of it is also about the practical use of it.
[01:35] And that's a big reason. I will link and also thank you for helping me figure out what I was actually trying to say about data modeling in my article instead of the very convoluted way I wrote
[01:51] it. >> Yeah. No worries. It's one of those things it's like it's kind of awkward to talk about, especially because, you know, as I kind of pointed out, like there's two definitions of
[01:59] data models, right? Like there's the data models that are actually like talking about like what you're trying to model and kind of like modeling real world objects. And then there's like the more
[02:08] like formal definition of data models and kind of how they are set up and kind of the relationships between them. And so using the term can just be confusing kind of by nature. Got to love words
[02:21] like that. So yeah, I hope the practical kind of exercise of going through it will like help everybody just kind of see what's going on. >> Yeah, for sure. And good morning or afternoon,
[02:34] everyone. Homie, I know it's morning your time, I believe. So in the chat, I'm trying to keep up with chat and also copy and paste everything where it goes. For those, the blog I was talking about
[02:53] that I got input on is right here. And then I will pop out the chat now that I know I can do that. Very exciting. Because then I'm not missing everybody's stuff. I still kind of do. I'm not
[03:11] going to lie, I still kind of do. >> That's all good. We have Blushing. Hey, Blushing, how's it going? >> What up, Blushing? And hi, Jay. Yay.
[03:20] Oh, that's fun. Jay, yay. Yay. Homie, I don't have some... Okay, we're not going down to rhyming thing today. It's not going to... Blushing, crushing? Hey, that one kind of works, though.
[03:37] Blushing is crushing it? I don't know. >> Blushing is crushing it. >> Y'all, I will totally admit that I have been running around like a chicken with my head cut
[03:51] off. So that and my ADHD self is on fire this morning. If you need me to slow down and stop being so all over the board, please keep me posted. I'm working on adjusting the screen.
[04:08] I can show everybody that I'm working on adjusting the screen. Do, do, do. Do. Okay. So I feel like this might be the best way of doing it. I don't know.
[04:25] >> Should work. We could try it. And if it doesn't work, then we can try something different. >> Yes. All right. So I do not have a great way of talking through, and everybody watching,
[04:40] please let me know if I need to zoom this in more. I do not have a great way of figuring out how to make content for the podcast that I completely froze. I'm not doing anything. I have episodes
[04:55] backlogged that all I have to do is upload them, but I'm so overwhelmed and stuck that I haven't, I'm like, no touchy touchy. And it just, now it's so big of a monster that I'm like,
[05:07] I know I need to do it. I don't know where to start. And this is, I would say, kind of like a start on data modeling. >> Yeah. It's kind of outlining the
[05:19] workflow. And I think that that's really great. And when it comes to actually like where to start the modeling process, because again, you kind of run into the same issue, right? Like we could just
[05:29] start at the beginning. But one of the things that I like to do, I like to start with two questions. So first of all, what is the, is there a place that you tend to forget to do a step? Because
[05:44] I know with ADHD, that's something that this is how I pretty much function every time. As soon as I forget to do something, I can pretty much guarantee I'm going to forget to do it again,
[05:56] because ADHD. And so I work on a way to automate that step as much as possible. So I can't forget. So either it's an automation of the step itself, or it's an automated alert that if I forget the
[06:09] step, it'll let me know and not let me continue. So that's kind of the one approach. And then the second place that I like to start is any place that is just like time consuming. Is there a
[06:25] bottleneck in the process somewhere? Because again, kind of from the ADHD perspective, right? It's like, knowing that there's something time consuming. It doesn't have to be hard. But it's
[06:42] just kind of painful in that sense, right? It just takes up so much time, and so it stops us from doing it. And so that's where I like to start in the process and just say, hey, where are the
[06:53] biggest pain points? And when it comes to building products as well, this is a good way to design products. Instead of focusing on what you think the world looks like, start with the problem.
[07:06] Where is the problem? And then kind of move out from there. So I find this a helpful process. So if you've got a place that fits either of those, I think that would be a good place to start.
[07:17] - All right. And that being said, thank you for that explanation, because I think that does make a lot of sense. I think for myself is I'm stuck on social... I'm like stuck at the end. Because I
[07:36] know I need to plan stuff from the beginning. But I'm like, oh shit, I need an audiogram or graphics or where am I uploading? Am I doing something with Patreon? And these are all thoughts that I'm like,
[07:58] it's terrifying. Because I've realized if I don't do social media, no one's going to find out about the podcast. It's definitely a niche. It is not teach gen tech, which it's a lot easier to get
[08:15] traction. - Yeah. So that's a good point. So we can start with social media then. Because I think that's good. So the first thing I would do is I would break that down into what social media
[08:26] platforms you care about. That way, you know, social media is kind of a broad term. So if we break that out into the various platforms that you use, that'll probably be a good bit easier.
[08:36] - And y'all, I like it, Jay. You just don't do any social. I don't blame you. I definitely don't blame you. So this was the beginning of me trying to figure out social. Because I have four projects.
[08:55] And so we're just going to skip the other ones. Because the only one that I'm mostly doing for social is teach gen tech. Because people won't show up. And I'm like, I want people to show up.
[09:05] This is good content to learn. So for the podcast, which is called Shit You Don't Want to Talk About. So if you see the word shit, that is why it's not shit. It is actually really good.
[09:17] But it's Twitter, LinkedIn, Instagram, and TikTok. - Okay. So, you know, that kind of tells me that we probably need like four different flows, right? And so, you know,
[09:37] in kind of breaking this out, I like to get it down to, you know, as simple as possible, right? Like just a very simple workflow. Because then we can come back and we can actually like make
[09:50] composite workflows that are built up of the workflows that you've kind of broken apart, right? So, yeah. Let's just start with Twitter. We don't even need to worry about the rest of it.
[10:00] So we'll just start with Twitter. So what kind of content do you have to push out to Twitter? - Okay. Now I'm just like totally frozen. I would say some of the content is the same
[10:22] across platforms. So like episode announcements and episode live. There we go. That's what I'll call it. And then I have, you know, past episodes. Causes. Like causes to contribute to or important
[10:56] hot topics. I'm going to do hot topic just because hot topic. - I really want a studded belt. - Yeah. I know. That's why I was just thinking about it. So the young me that always wanted to
[11:12] look like a really cool emo punk goth kid, it never happened. But I finally got the purple hair. - The purple hair rocks. And it like matches the whole like Twitch stream, which I think is
[11:23] fantastic. Like it's very color coordinated. - Thank you. Thank you. - And I actually used to have like a ton of facial piercings and worked at Spencer's for a number of
[11:31] years. So yeah, no, I'm right there with you. Like I was right there in all of that. So, but yeah, I think it is two words to go back to the original question. - Yes. And thank you, Ben, for commenting
[11:43] my hair. It is also something that I'm pretty sure and Ben, this is before I knew you. So I'm like, I think it was Ben, but I'm not a hundred percent sure that he was posting stuff in
[11:58] one of the discords. And I was like trying to model my stuff, like kept like seeing other people's graphics. I'm not sure. It was two and a half months ago. That was a long time ago. I don't
[12:11] remember. All right. What else do I need to post on Twitter? Oh, something I'm supposed to be posting there too and not is Wednesday Twitterspaces. - How's it going, Ben? Yeah. So,
[12:40] okay. So I see a couple of different things popping out, right? And so this is why it's always helpful to like go through this process because now I see, so we've got kind of the
[12:51] um, announcements, right? And so there's something happening at a specific time. And so, you know, you want to be able to alert people that it's live.
[13:04] And then there's kind of the like discussion category, right? So that's like the hot topic causes, what do we want to get into? So that's kind of an interactive thing. And then like
[13:22] past episodes, I would say is kind of, let's see, I guess we can call it like archive, right? And so that that's kind of a, just something we can kind of like reach back and pull things out from the
[13:44] past to kind of get people interested into what's going on, right? And so kind of looking at this here. So, you know, if we start breaking it down and kind of just start thinking about what we
[14:01] might want to do for the announcements, because I think that's probably the easiest, right? And so, you know, we've kind of got the event name, right? We could probably say like
[14:23] event, I'm going to say category, that may not be the best word, but you know, kind of in terms of like, so you've got like the four different projects, right? So you probably want to
[14:35] categorize it that way. Project, maybe project might be better. Just some way to campaign. There we go. That's a good one. - Yeah. It's the marketing term for it.
[14:46] - Yes. That's an excellent one. - Yeah. Okay. I know I'm totally making a slow down because I'm trying to organize this to where I can like do it again.
[14:56] - No, no, it's cool. And I think that is a really handy thing to do. And I do that pretty much with everything I do. Like the first time I do something, I tried to go through it slower to make
[15:09] it more repeatable in the future, because then it's more likely that I'll do it again in the future. Again, ADHD, got to play tricks with ourselves, right? Like we've got to make it as easy as
[15:18] possible on our future selves. - Yes. Yes. Okay. So you were saying for announcements, it's like, oh, I could do this. So it's, at least for this announcement, it would
[15:36] be campaign. I really, so campaign to me is saying, yeah, what like project it is, like you said. But I do think that I need to start putting tags like on, hey, this is this topic.
[15:56] - So I'd probably separate that out into something else. So that was actually the next thing on my list that I was just thinking about. Because the tags could actually be shared between campaigns,
[16:08] right? - Yeah. - Because there's a lot of overlap in the different things. So I think tags are important.
[16:16] - So, but campaigns, so would I put campaign on like each of them, or that's like a hierarchy, like up here kind of thing? Like all of them need campaigns?
[16:26] - Yeah. Yeah. I would say that that's probably shared between all of them. - Okay. - And so...
[16:31] - Tags are also shared. - Right. - Yeah. Because like trying to figure out hashtags is interesting, just to say the least.
[16:40] - Yeah. - Just in case anybody was curious. - Because of that, it's like, I don't know what to use. I'm just not gonna use any,
[16:46] or I'll create my own and then nobody will use it except for me. And that's fine too. - JavaScript and JS get retweeted by bots. - I know.
[16:55] - And it's amazing because it does get more visibility. Although I do feel really bad if I use like 100 devs, because I'm like, I'm not doing that program. I shouldn't use that hashtag,
[17:07] but it gets retweeted. - But it's also helpful for people in the 100 devs community, right? And that's kind of the thing. So if it's something that they're
[17:14] interested in learning, I actually love the 100 devs community. I've had a lot of coffee chats with people from there, and I think it's a fantastic group, but that's an aside there.
[17:24] - Okay. So an episode would have... Well, where do I put... Like episodes content, like I should know the episode name and everything
[17:42] by this point. So I would be using like episode title and one-liner. - Okay. So we've got like a title and a description, which I think...
[17:52] And yeah, like titles probably, I said kind of like event name, right? But yeah, title is... But yeah, the description is handy. And then I think the date of it is probably helpful
[18:13] for people to show up maybe. - Well, these ones, when the episodes are live, I mean that they go live that day. They're not live streams. They're supposed to
[18:26] come out on Wednesdays. - Cool. Yeah. Okay. That makes sense. And so I was thinking of like the event is live, not like... But anyway, it's about the same,
[18:41] right? It's actually... - Airs. Episode airs. - Episode airs. There we go. - There we go.
[18:46] - And then... So yeah, that... - And then I feel like I can make these smaller to also work better. And then because these would also need to go to this one and
[19:03] this one... Oh, I definitely need to like move stuff around. There we go. This one would also have date because it's a Twitter space.
[19:18] - Right. - By date, I do mean date and time. I feel like they can be lumped together. - That sounds good.
[19:25] - Okay. So... And... - Oh, sorry. I just remembered one that I'm really bad at and... Tagging people. We talked about this. And if we want to create
[19:44] something that can tag people, I would love that. But I need to tag all the humans. - So we can absolutely create something that does that.
[19:55] - That's going to be a one-day thing. I like that we're starting to have repeat... I almost said repeat customers. Repeat guests. Ben's coming on once a month to talk about accessibility.
[20:08] - Excellent. - And Jay will be on at some point. He has a talk tomorrow and just raised money yesterday.
[20:15] - Nice. - I was watching that livestream for a bit. All right. So we are... - So, yeah. Let's see.
[20:29] Is there anything else you like to include in those? - In those two specifically? Oh, yes. Graphic. Graphic.
[20:49] Oh, dope. If I can make it, I totally will. I really like watching other people's livestreams. Because especially people I know, it's kind of like... What is it called again? The
[21:06] buddy system? Not buddy system. Body doubling. And it's very calming. And I learn so much. - So much.
[21:20] - So true. - But... Oh, you're not doing a stream? You're doing it while you're watching? Okay. That's fair.
[21:27] You do cool things while you stream, too. - Reverse body doubling here. - All right. So we have episode airs. We need the title, description, and graphic.
[21:37] - Okay. - And Wednesday is title, description, date and time, and tag all the humans. - So for the Twitter space,
[21:51] in terms of tagging humans, are they people who have been there before? Are they people that you expect to be there? Where are we getting the humans? - The humans are...
[22:04] Magical creatures that just showed up enough that I started tagging them, or they requested to be tagged. - All right.
[22:15] - I have a very ad hoc list of people that I try to tag across all of them. I've had to create, I think, three posts yesterday and three posts today just to try to get everybody tagged
[22:33] for tomorrow's Twitter space. But I mean, the Wednesday Twitter space is technically like my social media thing, but the podcast definitely needs to start doing it too, because
[22:51] it's where my two lives overlap. - Right. Okay. Well, that's something to think about, because we can think about good ways to do that, because there are limits on kind
[23:04] of how many people you can tag. But if we have the idea of tagging people, I think that would be useful, right? And so human tags as opposed to topic tags.
[23:16] - Yeah. Oh, that's a great way of saying that. - That's the problem. Words just start overlapping, and you're like, okay, well, now I'm using the same word for multiple things, and that just,
[23:30] that gets tricky. - I'm going to pause us really quick. - Yes. - And say, Jay, I watched Al's
[23:38] stream last night, and I didn't want to get booted, so I was like, yo, can I, like, talk about other people? So I totally talked about you and just tagged your Twitter space or your Twitter.
[23:51] And you do cool things, so everybody should, like, basically anybody that's, like, hanging out with us, you should just go follow them. So if y'all want to just, like, drop your Twitters, do it,
[24:05] because everybody really does cool things here. So everyone should be friends. That's just where I'm at. All right. - I'll share with you.
[24:14] - So these are created from requests. Tag requests. - Yeah. Like, people asking to be on it, to be tagged.
[24:35] - Right. So I was looking at Blushing's question there, and I don't know the answer to that. - Wait. What? - The link looks like it showed up.
[24:48] So I think just anybody who drops links in the chat are not getting deleted by a bot if they don't subscribe, or maybe they do subscribe. I don't know. I'm super new to Twitch, so I'm just
[24:59] trying to, like, decipher this and understand it. - Oh, me too. Ben might know this one, or Jay, or... I'm just trying to think. I honestly have reached out to Ben so many times about
[25:10] Twitch that that's just my go-to person, but probably other people know, too. - I was going to say, Blushing's probably one of the more experienced Twitch streamers here, too,
[25:21] so it might be a setting or something. I don't know. Or perhaps it just works. But you should totally go follow Blushing. I will totally vouch for everything she does there.
[25:33] - Blushing, we're going to be friends. It's going to happen, and I will follow you after this, maybe. Let's see how I... I'm getting confused, so I'm not going to...
[25:43] I'm working on focusing today, because we have to stop at the end of the hour. - We do. - All right. So tag requests,
[25:51] that's how I tag all the humans, is a request, and I... So just out of to know that I have to create something here, I'm just going to put, "Need to create list process to do the things
[26:15] of tagging." - Yeah, that's good. The nice thing is we can just... These chains can go on forever, and we can kind of do it.
[26:28] So it's okay to just stop and be like, "That's good enough for now." - Yeah. - Okay, cool. So let's actually
[26:37] go down to the bottom and see what we've got for these two, right? - All right. Go over there. I want to put them closer together, just so that way I can
[26:49] look at them all, but that's a cool thing with Miro. So a past episode would probably... - So would the past episode just be the same as the episode airs,
[27:03] except after it initially airs? - Yes, but that's another question, is do I create the same type of post and repost it, or do I scroll to death and retweet the same
[27:24] post? - So I think there are a few different approaches there. So the thing that I've actually found works fairly well. So I use a tool called
[27:38] Hypefury that allows me to set recurrent posts and what they say are evergreen tweets, and it'll periodically retweet those for me. So you could totally use a tool like that to just... And then
[27:54] you can even say, at the end of the day, go back and get rid of all of my retweets, so that if somebody just comes to my profile and scrolls through, it won't just be a bunch of crap retweeted.
[28:04] - Wait, it deletes your retweet? - Yeah, it un-retweets it, and so the idea for the retweet is really just get it live again in people's feeds for a day, and then at the end
[28:15] of the day, just go back and undo that, and then do it again later. - What is that called again? - So it's called Hypefury. - I'm not the best at spelling.
[28:31] No one look at my... - I'll drop it in the private chat there. I don't have the... - Sweet.
[28:39] - Yeah, and so they can do all sorts of magic with that, and so that's a good way to kind of automate that part out. And so really, after you create the initial tweet, you can add it to your
[29:04] list of just evergreen tweets or whatever, and then so periodically, it'll just put it in. And you can set schedules for how often you want that stuff to happen. As you go up through the tiers,
[29:20] you can also integrate Instagram and LinkedIn, but I know the LinkedIn version is more than I want to pay for it, so I don't do that part of it. But yeah, something to think about,
[29:36] and especially if you can expense it to work, I recommend that, because then you could actually probably set it up for everything. - I'm just going back here, and I'm like,
[29:45] oh yeah, you guys are technically co-workers, and that is fantastic, because you both are good humans. They both work at Microsoft. - Oh, very cool.
[29:54] - Yeah, that is cool. I didn't even think of that, because I think you guys, A, it's just such a giant company, and B, it's like... All right, awesome. Glad you guys connected. I need
[30:06] to concentrate. All right, so past... That's an option, or just schedule... Can schedule episode... Duplicate of episode... Right? That's another way I could do it?
[30:41] - Yeah, absolutely. And one thing to possibly consider here, too, is just maybe the cadence that you want to do that, right? So how often do you want to share old episodes?
[30:53] - So that's, I think, another thing is... Oh, shit. This is why it's so complicated for me. So episode airs, I also have to do hype... Or, I mean, do I need to do hype stuff?
[31:13] - Well, so what do you normally do in terms of hype stuff? - What I normally do, or back in the day when I had a real job and paid somebody to do this stuff,
[31:24] because it doesn't... It clicks for me for Teach Gen Tech. It does not click for me for doing podcasting stuff. But creating audiograms, so that way people post them and get excited.
[31:40] And going back a step, I'm like, "Cool. I can create the audiogram. I just don't know what to cut. I don't know what's going to be an important clip." And then doing a different
[31:52] graphic, like a text graphic of them... Like a quote, or something like that. So what do I do for that one? How do I figure out that quote? I can create it. I just don't know
[32:06] what to do, like how to get there. And that is what I mean by hypes. - Okay. Yeah, that makes sense. So you said you use Descript, right?
[32:18] - I do. - Okay. And so do you record the video and audio for your podcast? Okay.
[32:29] So I'll let you in on a little secret that actually Lobau told me about editing and finding the highlights. He said instead of listening to it, or looking at the words,
[32:40] and Descript does the transcript, right? He said, "Just scroll through and watch the faces. And when faces light up, that's a highlight."
[32:50] So you can see it on people's faces when they get excited about something, or something is interesting. You can just kind of do a quick scroll through and say like, "Oh, this was kind
[33:06] of like a high-energy moment." And that's a good opportunity for a highlight clip. So that might be helpful. And this part, I'm not going to be terribly useful on,
[33:18] other than that one tip, because I don't do that. - Yeah. And on this one, and I think that's a really good call-out, and I want to write it out.
[33:25] I'm trying to think it through a little bit of... When they're shitty topics, I'm like, what will that expression be? In the fact that if we're talking about generational trauma,
[33:44] if we're talking about... - That does make it a little harder. - Like where... I really like that hack though. That's why I'm like...
[33:54] - I think it's good. And I think instead of looking for maybe the eyes light up, because that would not quite apply, but you can definitely see emotional responses,
[34:06] right? And those emotional responses are a good place to cut the clip or whatever. But I would even say for this part of it, we don't necessarily need to model all of that out,
[34:20] right? Again, this can go on forever as much as we want. - It really could. I'm going to do... So those are announcements, which this is looking good,
[34:29] but then I'm actually going to do... I'm just going to copy both of these, so it makes my life easier. Nice. Hypes. What would I call hype ones? I like how you put a very logical...
[34:44] This is an archive, this is an interactive. What would a hype be? Would that be an announcement too? - So I would say
[34:53] we could call it a couple of different things. Potentially an artifact, right? So something that is shareable, like a concrete representation of something. And they're actually different types,
[35:10] so I would even separate those out, right? So there are audiograms, there are video clips, there are static images, right? And so, yeah, I think probably the classifier I'd put would be
[35:28] just artifacts or... That's the only word I can think of, which may be not even the best one, but it's the one, so... You can always rename it.
[35:46] - No, I kind of like artifacts because it makes me feel like Indiana Jones. - Right. - And that's...
[35:54] - And you could do an entire Indiana Jones-themed workflow, to where you rename all of the steps, like something that makes you think of Indiana Jones. And then the whole workflow is more fun
[36:05] too. So that's the other thing that I... The other trick that I sometimes use to make myself do stuff. - Yes, and I like that,
[36:13] because it's like the audiograms, the text quote... Yeah, whatever. And so for those... And this is also the other thing, is how much... We're putting what I need to put into them,
[36:31] but not necessarily how to create them. But I am going to do this really quick, so I don't forget. In the script, use visual cues from facial expressions to create... To find
[36:59] a good audiogram. Right. Cool. - And so one way to actually kind of streamline this too, is once you find... You could start by doing the audiogram,
[37:22] because if you can quickly scan to get that, then you can just make a text quote of that audiogram. To kind of streamline it, and then... - Would you reshare the same
[37:32] information though? Or would it... Because they're hype ones. This is literally what I get stuck on, is, "Oh, I like that idea, but is that good enough?" - So if it's done, it's good enough.
[37:46] And you can always modify the process later, but I'm a big believer in just making it as easy as possible from the get-go, and then optimizing later. So the answer is,
[38:00] I have no idea if it'll work. But I would start there, and then see how they perform. If you start to see things go down and go, "Well, maybe people aren't all that interested."
[38:11] But what I found is that typically... First of all, Twitter doesn't show everybody everything anyway. And so you could share the same thing five times, and nobody's going to see it five
[38:22] times most likely. They might see it once. And so that's kind of the trick there. But also, people are attracted by different things. So they may see both of them,
[38:36] but based on what they're more interested in, they may actually engage with the audiogram, or they might engage with the text quote. Whereas they probably wouldn't necessarily
[38:51] engage with both, because people are attracted to different cues, right? And so being able to just give people options to... It's tough. With social media and trying to get people to do
[39:05] things in that feed, it's such a crapshoot anyway. - I think that's another great question, too. And Ben, you're going to be stuck in the back of my head about accessibility for the rest of my life.
[39:19] Thanks, but no thanks. I will say it like that. Is it open captions that are burned in to the video? Because I'm wondering if Descript does that. So that way, you can post with...
[39:39] Okay. So I don't know if Descript does open captions, but it's to be able to read it at the same time. - Right. Yeah. And that's something that is good to figure out. And unfortunately,
[39:52] I don't know the answer to that. - That's okay. We're going to put Descript. We can go back and fix that later. You can export closed, but do you know if it can do
[40:12] open for audiograms? Because I think it has an audiogram export option. Okay. Anyway. Got to keep going. Got to keep going. All right. So audiogram is also going to have the graphic.
[40:38] And then it's going to have... Oh, yeah. That would have been fine. It will have the title. It will have audio. And I don't know if it does open captions,
[41:04] but I can look into it. I think folks may use CapCut. All right. I'll just put it. And this is the other thing. I'm like, y'all, I don't have a real job yet. So I'm buying shit.
[41:27] And that's a big thing. Because when I first launched the podcast, I had a lot of automation. Which did make it easier. But very expensive. Very, very, very expensive.
[41:37] - It adds up so quickly. - So expensive. - Yeah. And so that's why I say just do what you can and don't worry about doing everything. Like,
[41:51] especially on a limited budget. Because, you know, yeah. All of that stuff can be added later. And, you know, like, keep in mind, like, these can definitely, like...
[42:05] First of all, a lot of this is shared information. So, you know, if we look at kind of how different, like, you know, the title shared and everything. And, yeah, like, the automation triggers are a
[42:19] great way to, like, you know, so as things happen, you can just kind of pass that information down the line, right? And so... Oh, that's cool. - Yeah. Like, Jay, there's so many things
[42:37] I want you on the show for. So first we got to get you on the show. And then you can be requested as a repeat person, too. - Right. Can't do it once. That's the trick.
[42:47] But, yeah. So that's cool. - Okay. Yeah. And it's showing, like, it's repeat content, repeat content. - And, like, the graphics for episode airs,
[43:01] the audiogram, and then, you know, I'm going to say that the text quote has some sort of caption there, as well. - Yeah. So...
[43:09] - Can those all be, like, the same graphic or the same template, at least? - So I can use this. - Because if you have a template,
[43:17] which if you don't, I would highly recommend, like, spending a little bit of time to develop that template where you can just drop in what you need. - Yeah. Luckily, those... Yes. I do have
[43:29] those. - Okay. I figured as much. - It's just... I don't know why they're so time-consuming for me, but they are. This is
[43:36] also a big reason, like, I've been slacking on, like, teach gen tech stuff, too, because I'm just, like, there's so many steps. Did I forget a step? So I'll also be doing this for that, too. This
[43:48] mural board is going to go on forever. - And that's kind of the great part about it, is, like, just starting it, you can always add to it, right? And you can keep adding levels of
[44:01] detail. And as you do that, you start to see, like, oh, well, this is shared here and there. Because then you can kind of start, like, rearranging things. And then you say, like,
[44:11] oh, well, actually, I only need to, like, do this one thing, and then that unlocks the data that I need for, like, these next four things. And then maybe I can automate some of those or all of them,
[44:21] right? And so you'll be able to kind of do things in different orders as you realize that it's, you know, we typically think of things linearly. But when designing workflows, you'll start to see,
[44:34] like, where there's a lot of repeat work in various steps, right? And so if you can extract that repeat work out into, like, a preliminary step and then just share it between the rest of
[44:45] the tasks, all those other tasks get smaller and, therefore, easier to manage. And that's why I think this is just such a valuable exercise in terms of, like, figuring out, like, what pieces
[45:00] go where. And so, you know, we can kind of see that, like, all of this data for this is pretty much something we can capture, right, in terms of -- so, like, you know, most of it's shared. And
[45:20] I think the only things that, like, necessarily require new work are, you know, putting the information into the graphic for each one, right? And so, like, those will be slightly different.
[45:40] >> Yeah. >> Right? >> But almost -- well, let me delete this one. Because I think the graphic -- I'm going to put
[45:50] these ones up here. I think the graphic for, like, episode airs is going to be the same graphic for, like, the audiogram. >> Okay.
[45:59] >> So, I can put it there. Put this there. But it's not the same graphic as the text quote, because I'm not going to be able to fit it all on there if it is, you know?
[46:10] >> Right. >> So, yeah, graphic. We got title is the same for everybody. Okay. And I will color code these later so they're easier to
[46:28] read. And then description would only go into episode airs. Because that's going to be longer. I can get rid of these. And all of this stuff, it's all on its -- by itself. So.
[46:48] >> Oh. >> Okay. So, now I think we can actually step out of the workflow for a minute. And if you remember last time, we were talking about, like,
[47:01] identifying the nouns that we care about, right? >> Yeah. >> And so, I think the most important noun here is episode, right?
[47:08] >> Mm-hmm. >> And so, like, that episode then contains the title. You know, the description. The date and time of airing.
[47:27] Let's see. And then so, we have two graphics. So, there's the, like, announcement graphic and the text quote graphic.
[47:49] >> Yeah. So. And the audiogram. >>
[48:11] And I think this is something that I definitely would want to do more on a -- another episode. Because it's, like,
[48:36] at least in my head where I think this would be really helpful is we're taking it and so, we're looking at the data model and the workflow. We're creating the nouns. But just, like, when I'm,
[48:48] like, hey, what do we want to make? It's going to be cool. I don't know what to make in, like, a program. Like, you know, do I want to make a web app? Do I -- like, I don't know where to start
[49:02] for what the naming convention should be and all the things I should name and actually translating that to a program. So, I'm just going to -- Leo or anybody else that one day when Leo and I are
[49:16] done with this want to create something that can, like, show people this or talk me through it, I'll figure it out, too. But being able to, like, you know, go from step A to Z,
[49:29] even though they're two different projects. >> So, I mean, the cool thing about this, so, actually, and I will say for the nouns, really episode was the noun. All of that other stuff is
[49:40] kind of under episode. So, like, and when I say nouns, a lot of times this is something that will be a table in a database. Or that's kind of the easiest way to think about it, right?
[49:54] And then so, all of those will be columns within that database. Potentially. And so, when you start looking at these and you say, okay, well, if I have a database that has this
[50:08] information, then I can generate all of the artifacts that I need from that information, right? And so, you know, kind of just starting out by then, like, okay, when I create an episode,
[50:23] these are the things I need to fill out. And then it's probably just a matter of, like, copying and pasting into tweets for now. But then later you can be like, oh, I can actually just
[50:33] automate, you know, this step of the process to post these tweets. And ideally what would happen is you'd be able to record the information or, you know, record the episode, put in this
[50:43] information, and then it would automatically do the rest of it. Because these are really the most important pieces of the workflow, right? The rest of it's just kind of, like, breaking it up
[50:55] into various pieces and putting it out to different destinations. And that's really, like, what an app is about, right? Or a program. Except typically when we think of that, we think of, like, a web
[51:07] app. It's displaying all this information, like, somewhere in our own web app. Whereas this workflow, we're displaying bits and pieces of information on Twitter or on Instagram or on
[51:18] LinkedIn or wherever. And so that's why it's such a good idea to kind of get this handle on, like, what are the most important pieces of things I've got? Because once I get that data,
[51:30] I can do all sorts of things with it. And I can even, like, transform it into various, you know, different representations of that data. But the data is what is actually needed. Because
[51:44] then you start thinking, okay, well, where do I get that data? Can I get any of that data automatically? And so you create the database table. And maybe you start off by just putting
[51:55] it in manually. But then you realize, oh, actually, when I post this episode or, you know, when StreamYard saves this episode or whatever, right? I can save that to a specific location
[52:10] and then pre-populate all this information or at least, like, some section of it, right? And so you can start getting a little bit of this information, like, pieces at a time
[52:19] automatically. And so all of that then becomes a bigger app. Because you've broken it down into, like, small pieces and say, okay, I need this, this, and this. Where do I get those? And, you
[52:35] know, it's easiest to just start off manually. Like, just give yourself a place to start off manually. And so, like, Airtable or Notion, great. >> I love Notion.
[52:46] >> I do, too. And I'm still learning it. But, like, I'm a Cub Scout leader for my son's Cub Scout den this year. And so one of the first things I did is I created a Notion dashboard to, like,
[53:00] keep track of, like, what I need to do. Because I'm that guy. But, yeah, like, just being able to have, like, a representation of this data and just being able to see, like, oh, I need this.
[53:13] And I can fill all this in. And then, like, oh, for this next step, I just have to copy and paste all of this. That makes it so much easier. And, like, yeah, just going through the process,
[53:26] I think, is so helpful in seeing that. Because, again, then you start being able to reorganize. You start being able to optimize various workflows. And you start to see, like, where your
[53:35] pain points are. And, like, oh, well, like, 90% of this is okay. But this one piece is a real pain in the ass. Like, okay, well, how can I break that down further? How can I fix that? Do I need
[53:47] that piece? Maybe I don't. Maybe I can just scrap it and say it's not worth the effort, right, for what we're getting. And that's really where the good optimizations can come in.
[53:58] - And I'm totally digging this. And it was really, really helpful, like, A, just being able to go, okay, Jen, stop being so ADHD and, like, refocus. In the fact that
[54:13] this is a big problem that I have when trying to get this stuff done without having, like, a list written out. Because I'm like, oh, shiny, that's over there. And I don't mean that as, like,
[54:24] I hate the term when people are like, oh, Dory. And I'm like, no. It's just naturally, I'm like, oh, but this needs to get done, too. - There's a million things that need to
[54:35] be done. And the nice thing about this, you can branch off for a while. You can follow the rabbit hole, right, and go, like, oh, well, this actually leads here, here, and here. But then you can go,
[54:44] oh, actually, I just need to come back to here. I don't need to focus on that right now. But when I do need to focus it, I've already got the connection started. So, I can come back in and
[54:52] then, like, work on that. - Exactly. - So, I do find it really helpful to kind of, because it just builds on itself, right? And so,
[54:58] as you start modeling it out, you kind of get this more complex thing over time that allows you to more easily come back to where you were before. And, you know, so you have that diagram. And then
[55:13] you have the database. And, like, so once you have that, like, and you start putting things in, it all starts coming together, because that part becomes easier. And then you're like, oh, well,
[55:22] now I have extra time that I can spend on this part of it. And do I want to automate this? Yes, no, I don't know. - I'm not gonna lie. This is,
[55:31] I'm gonna be sending you the link to, like, schedule your next episode. - Absolutely. - You know, because I think something
[55:39] that, and LaBao is, like, so many quotes from LaBao. Something that he said that really stuck with me is, like, when people, and I'm totally paraphrasing this, of, like, when people are,
[55:54] like, hey, you're here, but go over to that island. And, like, we can all logically be, like, okay, cool, I need to get to that island. But how do we go from A to B? Like,
[56:09] like, okay, you're telling me how, but it's just, I don't, you're saying words, but I don't get it. And I think that is something that I'm like, okay, cool, like, you've shown me how to do this,
[56:21] it makes enough sense that I'm, I feel like I can work through my diagrams for everything. But then the database stuff, I'm like, I get it, but I don't get it.
[56:35] - So it sounds like next time we need to be working on a database. - Yes, yes. And Leo is good at this stuff, definitely, I agree. And,
[56:46] homie, Leo definitely needs to come back. This is his, I'm surprised, I'm kind of glad, but I'm kind of surprised that nobody showed up last week for our episode.
[56:57] Because it was not as organized. It was just, like, a bunch of, but it was a lot of theory that's set up for today, which I'm very, very grateful for.
[57:06] - Yeah. And, you know, theory is good, and it's, but honestly, like, just going through the process, I'm always torn of, like, do I do theory first or practice first? Because it doesn't really matter,
[57:19] because, like, they kind of, like, feed into each other. And so, you know, we can go through, like, the process of just doing it and then talk about the theory and why all of it works.
[57:28] You don't actually need the theory, but it does get you to some places, like, earlier sometimes. And that's something I always, like, go back and forth on. Because, like, I'm really, like,
[57:40] interested in the theory, because it's like, oh, yeah, this is why all of this works, because I've been doing this for a long time. But in reality, you don't actually need to know
[57:48] a lot of it. Like, it's helpful, kind of, maybe it's interesting, I don't know, but. - I find it interesting, interesting. I can't talk. Interesting. There we go. And once again,
[58:00] Leo, thank you for joining today. I know you and I both have meetings at the top of the hour, so I'm going to end the broadcast. And thank you all for joining. Please also tweet us, like,
[58:12] if you want to see shows on, like, specific people, tag them and tag me to have them on TeachGenTech. Tag Leo, too, so, you know, we can convince them. Well, I don't want to say I will
[58:22] bully them onto the show. That's mean, Jen. - We'll aggressively convince them, because it'll be so much fun and beneficial for all involved. - Yes. Yes. What he said. What he said. All right.
[58:34] Thank you all. Bye! 
