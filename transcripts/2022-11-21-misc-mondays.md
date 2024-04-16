---
showLink: "https://www.youtube.com/watch?v=-uR-ExeyYzc"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "misc-mondays"
title: "Misc Mondays"
publishDate: "2022-11-21"
coverImage: "https://i.ytimg.com/vi/-uR-ExeyYzc/maxresdefault.jpg"
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

[00:00] questions now. Hello, hello beautiful humans. Welcome to Misk Mondays with... Hi, I'm Jen and that's Laura. Hi, Laura. Hi, I'm Laura. I'm drinking coffee. Yes. Oh, I forgot my coffee.
[00:16] I have water. I need to drink water. We'll drink with water. Well, we'll stick with water. And before we get started on today's random topics, y'all can tell I cannot multitask and are hitting
[00:29] the we're live thing. I'll post in a group. Why not? LinkedIn always asked me if I want to post in a group. I'm like, okay, I don't care. I'll spam this group. What's a group in a LinkedIn
[00:44] context? There's like groups you can join and like premium career group is where I just posted this. Cool. I don't know. Yeah, but there's also like developers, Python, web... Oh, I should invite
[01:02] you to this one. Can I invite people? I don't hang on. I mostly don't fuck with LinkedIn. I dig it. I only do anything on it because of the stream. So that's about as far as I get.
[01:19] I'm not very exciting. Do we get traffic from LinkedIn? Do you know? I don't stream from LinkedIn. I used to, and I did get traffic, but a lot of people do find it because of LinkedIn,
[01:37] more of like the CTO type people. Okay. Okay. Because like those higher level roles I've noticed and hi, homie, I'm not ignoring you. But those higher level roles don't always
[01:55] like use Twitter as much. I don't know. It's been really, really hit or miss. So I just post to both. I have found people because they have been like, they use LinkedIn
[02:09] and have shared it because of LinkedIn. So I'm like, yeah, works for me. I will continue to post. But how was your stream? You streamed last week. Yeah. Yeah. It went super well. I was
[02:26] interviewing Andy Piper. Let me grab a link to that, I guess. And yeah, Andy had so much info to share about MicroPython and versions of Python that can run in small environments. And so
[02:47] MicroPython, that's really what it means. It means that it can run without taking up a ton of space. And so if you're trying to run on like a microcontroller, like if you've heard of Arduino,
[02:59] then you can use, I think it's actually CircuitPython that you would use on Arduino, but actually, no, you can do both. Or like if you're making, so something I would be interested
[03:13] in is writing my own IoT type devices because I have Nest devices, but the city I'm in is in the San Francisco Bay Area. And the city of San Francisco, so not my city, but a nearby city,
[03:34] voted recently, not the citizens of San Francisco, but the board of supervisors, the board voted to make it so that the police can tap into your private security systems, like without a warrant.
[03:52] That's not cool. No. And like, I bought Nest instead of Ring because I did not want to be part of the police state, right? And so then they're just basically saying the police get to
[04:06] log into these things regardless, whether Google wants to hand over your data or not, like they just get to tap in, which is complete bullshit, right? And so I kind of want to make my own IoT,
[04:23] like my own cameras and whatever at some point. So that's something that MicroPython would be potentially useful for because like the just, I mean, it's literally a tiny environment. If
[04:38] you're talking about something like a chip that's fitting in your little camera or whatever, literally small. Could it still record? So the recording would happen on like a server. So it
[04:51] would send the data, but I can have my own, I can have my own database, like locally I can have my own. Okay. I think that would be the only thing that I would be cautious about is like, how do
[05:03] you make it record? Yeah. Yeah. I mean, or you could record to the cloud, but if you're not using something like Google Assistant or, I mean, you could even use those assistants, but if you're not
[05:20] using Nest or Ring or whatever, like there isn't an interface that the police would know about to use to get in. Right. So interesting. Be fine. Yeah.
[05:35] Ben, you're going to be on Laura's stream and my stream. Yes. Oh yeah. I was looking for a link to the thing and then I got talking about the MicroPython.
[05:46] Oh, and MicroPython is relevant to WebAssembly because WebAssembly is a runtime that can run in teeny tiny places as well. And so that's, that's exciting. Cause I work for a company
[05:58] that works in the WebAssembly space. I was going to say that. That is really creepy. Oh, the San Francisco thing. I was like, what?
[06:11] I'm a nerd. It's okay. This is why we have our MISC Mondays. I got a background updated. Yes. And in, in StreamYard to go to our Twitches, our Twitch Eye?
[06:29] I think it would be Twitches. Twitches? Okay. Yeah. Okay. Yeah. I don't think it's Greek because it's, it's Greek stuff where you would, it's, it's, if a word base comes from, from the,
[06:43] wait, no, it's the other way around. Oh shit. I can't remember which way it goes. Is it the Latin gets pluralized sometimes with an I or the Greek? It's one or the other.
[06:53] I'm ridiculously distracted. Look, it only changed going to my background color, going to red. But if I go to pink, it's almost the same. It looks blue and I just changed it to blue and it's just
[07:12] slightly deeper blue. Let's go white. There we go. I was trying to think of a different color to match our news, news stream colors. And Ben just said, usually Latin is responsible for weird
[07:33] I, I plurals? I dash I plurals? Yeah. Yeah. It's the Latin and then it's the Greek that doesn't go that way. So yeah. So that's why it's octopuses, not octopi.
[07:48] That's what it is. What? Oh, I'm a 12 year old. It's okay. Yes. I, same. Oh man. Well, hello again, everybody to Misk Mondays. Laura is gonna
[08:08] find the link to her stream last week. I'm typing now. I'm typing it in the Twitch chat. Wait, I have a hot take about the octopus pluralization thing. Okay. Yes. Okay.
[08:28] Uh, Ben says TLDR, octopuses, octopi, octopeds are all fine. Interesting. I think, I think the same, honestly. Octopeds? Octopodes. Podes? Yes. Podes. Okay.
[08:47] Octopodes. I don't know how, but I am very, very happy that whenever we stream, it somehow comes on language and how to pronounce things. And, uh, Ben said that they are happy to go to Pat
[09:03] for octopi from a Latinist perspective any day. Octopodes. What? I am not good at sounding things out. So I'm just going to hide this and pretend. Yeah. Yeah. That's what I'm going to do,
[09:28] but thank you, Ben. And okay. So today, what do we want to talk about? Um, you said a thing before we started. I did. My brain is, is not with us today. It's,
[09:50] you know, it's around here somewhere. I'm cool with bullshitting the entire time because Oh, it was ducks. That's what it was. Yeah. Or we can do technical documentation,
[10:00] but at the same time, I'm like, I don't know how much concentration I want to do, but that is the fun of Monday is we get to choose. Then also I wanted to say,
[10:12] thank you to homie for making our background and our graphic for our streams. Cause you're way better at it than I am. Yep. We, uh, let us, let us know what we,
[10:24] what we can do for you, homie. Cause we're not about that free labor. No, no, we are not. No, we are not. Homie does a lot of random stuff for everyone. Like homie. Oh my gosh. Okay. We
[10:39] need to go. Did you see Tuesday stream by chance, Laura? Okay. First off it was with Jay about VS code, which was super dope. I suggest everyone watch it. And then, uh, we got to see a homies,
[10:56] uh, app, uh, the manager being, it also looks like theme anger. So we all know, um, Ben, it was because of your
[11:16] stream that homie found me. Cause Ben gave me a shout out on their stream. Oh yeah. So Ben's going to be on my stream next week. Um, a week from tomorrow. I have not,
[11:34] I've got it scheduled, but I hadn't posted about it yet, but I can grab the link anyway. Um, here we go. And we're going to be talking about accessibility in docs. Um,
[11:50] because I write, I write docs for living. Um, and I have run into some questions like beyond, um, beyond like, okay, I need to make, you know, an alt text for this image. Um, some like nuances
[12:10] about that, like, or is there like still a purpose for an image? Do we just not like do these or what? Like screenshots of things, you know, that kind of, that kind of thing. So we'll see.
[12:25] Now I'm intrigued. And Ben, you asked me what I wanted to talk about on my stream with you. And now I want to talk about it more like as a, like, you know, how do you
[12:39] create docs? But then like, if we just like tie in, like, Hey, here's how to create docs. So including, uh, the accessibility stuff. Interesting. Oh, I didn't realize that,
[12:52] that Ben also builds a doc site. I think I feel like I knew this and forgot. So it's like exciting new news for me. But then at the same time, I'm going, I should have known they don't, they do
[13:06] that. I forget that Ben works at Microsoft. Didn't know that either. Oh, well, Hey, they work at Microsoft learn formerly Microsoft docs. Okay. Yes. Um, because I got really excited
[13:28] when I realized that Jay and Ben both work at Microsoft. Oh, right. And I was like, do you guys know each other? I don't remember what they said, but I hope they know each other now because they're
[13:40] both amazing humans. It's a big world. Like the opposite of a small world, obviously. Right. Like at Microsoft, you know what I mean? Y'all that was my favorite, favorite, favorite ride in the entire
[13:58] Disney thing. It was, it was a small world case. Anybody wants to know, do you have a stream this week other than this one tomorrow? Oh, as a random thing. Um, before I go,
[14:18] uh, Oh, Ben said, uh, they didn't know each other at the time. Uh, but we had a family, friend, family chat. I can't read friendly chat and you can be a family chat too.
[14:32] And, uh, Grat said, uh, sleeping at, uh, last does a beautiful cover of the small world. Ooh, please post the link. Um, as a random thing with Jason, Jason being on the show last week,
[14:55] which, um, for those who may not have seen last week, last Fridays, as well as know who teach with Jason is I am grabbing the link.
[15:11] Uh, he was on the show last week and we talked about rebuilding a website on Netlify. And it was actually really cool because he was talking about some streaming stuff that he does.
[15:29] Um, and like auto generating, how did he say it? I'm thinking I'm paraphrasing horribly, but there is a tool within Netlify that you can upload the photos and it will use the information
[15:47] to create the graph. And I feel like I also heard of this during next nation when I was emceeing that last week. So I feel like I heard it from two different spots and now I need to
[16:01] go investigate it. But that is also something that yes, yes, Ben said it. Clara cloud cloudinary. I have to check out that too.
[16:16] Yeah. Um, so yeah, I mean, we can, we can talk, you know, like I can, I can talk a little bit about, about docs and we can see how much attention span we have and
[16:36] make no promises. I dig it. And thank you Ben for posting that. Here's a stream from last week too. And thank you for the, it's a small world cover. I feel like I need a, we've got it. We've got it.
[16:54] All right. Well, where would you like to start with docs? I am just dropping a link in the chat to the blog post I wrote about how I became a technical writer.
[17:09] There we go. Um, yeah, so, so I was originally, um, well, okay. Originally is, is not the correct word here because I have planned on about 27 different careers. Um, but the, the one that,
[17:32] the first one that stuck for more than a couple of years at a time was I was going to be a mathematician. I have graduate degrees in math, but, um, it turns out that academics don't make
[17:43] any money, um, especially adjuncts. And that's what I was. And, uh, I mean, so like for reference, I made $23,000 a year in the San Francisco Bay area. And that's not like reasonable money
[18:00] anywhere in the U S um, but in the San Francisco Bay area in particular, that's like way below poverty line type money. Um, and I was completely naive because I just assumed that, uh, my
[18:21] professors and so on made money that made sense. Like literally, I just assumed that that was a thing. Um, and, uh, it turned out, no, you, uh, you can only be an academic if you have a, uh,
[18:36] some other source of money, right? Like if your spouse makes more money than you do, or your parents support your lifestyle or whatever. Um, and so I was privileged enough to be able to
[18:53] take my time to make a decision about what I was going to do instead. And so I decided, well, like the most natural move seemed to be like into data science from, from math. And so I was going
[19:05] to do that. And that's when I learned the Python, um, and so on. And then, but I was kind of dragging my feet about the career switch and I, uh, wanted to continue teaching. And then with the pandemic,
[19:18] with the pivot to remote learning, I thought that I would be able to keep teaching. Like when I became a data scientist, I would still be able to teach like a section or two online, but then
[19:30] the university that I worked for, um, went back to all in person. So there are zero, going back to zero math classes online, which is a problem for all kinds of reasons. But, um,
[19:42] not only that I have, um, highly reactive airways. And so I can't be in rooms without ventilation with 40 folks, uh, since COVID. And so I had to relinquish my classes, um, that I was scheduled
[20:00] for. Like I had, I had a whole, like everything was all scheduled for this for last spring. And, uh, I had to say, I guess it was about a year ago now that I finally had to say, okay,
[20:09] I guess if you're going to make these classes be in person with no other options, then I actually have to choose between potentially dying for this job that pays me $23,000 a year, or, um,
[20:22] I have to do something else. I was like, okay, well, I guess it's time. Yeah. And that same week or the same week that the semester was ending. And I was, I was, my heart was breaking
[20:35] about not teaching anymore. Um, people on Twitter started talking about technical writing and I sort of ignored it for a bit. And then I checked it out. Um, this was a few days before
[20:48] Christmas. And I was like, oh, this sounds, this sounds like me because if you look at the, um, Google has a, um, let me find a link to it. Google has, um, a,
[21:04] a course, free course on technical writing, which I think I probably linked to on my blog post. I'm literally looking at my own blog post to try to find there is, um, and I will drop that in the
[21:20] chat too. Um, this description from Google, um, Google's course about, um, the field. Um, and they say you need to write clearly in English, uh, learn complex technologies relatively quickly,
[21:38] explain complex technologies and useful ways for the target audience, wield strong interpersonal skills and understand code. Technical writers are rare hybrids possessing an uncommon mixture
[21:48] of talents. And I was like, oh, but that's me. Um, and so, but I, I felt a little bit, I was pretty conflicted because I had already spent a couple of years like
[22:00] studying data science and saying that I was going to go into data science. And I didn't want to come across as flaky because it already was a pivot. Like I was going to be a mathematician, right?
[22:10] And then it was like, oh, okay. And now I'm going to actually be a data scientist. And then to then pivot again and be like, actually, it's going to be technical writing felt flaky. Um, but then I
[22:20] decided, you know, it's just, you gotta be, um, embracing, embracing your own actual talents as opposed to what you thought your pet talents were two years ago, you know, uh, makes a lot more
[22:34] sense. So I decided to do it. Um, and I did Google's Google's course, um, which is like self-paced. Um, and it, it was pretty quick for me. Um, and then from there, the, the, how you become a technical
[22:54] writer sort of path, uh, has forks with like many times, right? So I think everybody can benefit from that, that free, um, Google course. Oh, I think I posted the wrong link there.
[23:11] Uh, damn. I don't know. Sorry about that. I'll have to look for that in a minute. Um, but so some, some technical writers, right. Sort of maybe that the biggest, the, the first,
[23:27] the first fork is, do you want to be a technical writer who writes for it's sort of determining which, who's your audience going to be. So I interviewed with a company that is a cable
[23:45] alternative company, um, like cable television alternative company. Um, and there, uh, yeah, yeah. And so there, um, their deal was they were looking for a technical writer to be writing.
[24:05] It was more like the customer support docs. Right. And so they, uh, they, they were really concerned while talking to me that it wasn't a technical enough position for me. Like I wouldn't
[24:20] be happy in this role. And so I would be more likely to jump into a different role when I had the opportunity. And they were completely correct that that was my plan. Um, so for them, the
[24:34] technical writer was in the marketing department. Okay. And so that's like one way of being a technical writer. So you can think about like, you're the person who writes the, the documentation
[24:47] that is viewed by, you know, my, my cable box is broken. What do I do? That, that kind of thing. Um, and then there are technical writers who work for whose audience will be developers
[25:05] instead of the, the customers. I mean, in the case of the company that I'm working for our, our customers and their customers are developers. So it's like developers all the way down, but,
[25:17] um, yeah, so, so that's, that's one thing that you have to decide is how technical you want to be with your technical writing. So I don't know about the path where you think, okay, I think I'd rather
[25:34] be the kind of technical writer that is embedded in a marketing team. I don't know anything about that because I didn't do it. I know the technical writer who's embedded in, um, either developer,
[25:48] a developer relations team or an engineering team. And so there are sort of two different ways of doing that as well. Um, and yeah, so that's, that's kind of the thing about how I,
[26:04] how I got here. Oh, except I forgot the entire part where like I wrote a blog. Um, and so all the entirely before I decided to become a technical writer,
[26:17] I had been maintaining this blog, um, the same blog I've already linked to, um, which was my, like, I'm learning data science blog. And I actually didn't write any blog posts between
[26:28] the time that I decided to switch to becoming a technical writer and actually becoming one because that process was only about six weeks. Um, so yes, lots and lots of questions, but also
[26:44] okay, go here and share my screen. Cause I have questions, but I want to show everyone why I click the wrong button. I try to share a file, not the screen.
[27:00] Um, homie asked a great question of, uh, Laura, you, uh, just curious. You seem like a social person is technical writing kind of isolated. I think it depends a lot on your company. Um, so
[27:24] my company is fully remote and so yes, it's kind of isolating, um, because we're remote, but other companies that like work in person. So you might have a DevRel team you see. So as
[27:40] a technical writer, um, there are more ways than just these two, but you're probably either on a developer relations team or a, an engineering team. Um, and so either way you're like on a team.
[27:56] Um, I am technically on the developer relations team within my company, but I also attend like all the, um, engineering meetings, uh, because the engineers are the ones that need to tell me
[28:09] what needs to go in the docs, um, and, and so on. So I'm also an entire hermit. Um, and so I can realize that it's actually been three weeks since I have left my house and be like, Oh yeah,
[28:29] I'm fine. I can just stay here. Um, and, uh, I shouldn't laugh at this. I'm sorry. It's like this relative ability that I'm giggling at. Um, and so, so it's perfect for me. So I'm a
[28:45] social person in the sense that I love, um, I love chatting with y'all. Uh, but like the idea, like if this were a meetup in person, this would be much more draining for me.
[28:58] Uh, and I don't totally know why, but it's true. Ooh, I feel that. And that was a great question, homie. Yes. Uh, on the fact that like,
[29:11] I could easily not leave my house for a week. I would love it. Although Tyler makes me leave the house. He's like, you're leaving. We are going to go get like something to get you to leave the
[29:24] house. So he'll bribe me with thrift shopping to get me to leave the house. So, um, he at least knows what will bribe me. It's either food or, um, going thrifting. And I, I don't know, like
[29:39] at least in Laura, I'm curious to follow up question from what you just said is I know for myself is at least getting like, once I start writing, it's a very, very, like I have to finish
[29:54] it now. And yet a very calming and almost frantic at the same time experience. We're going to go with that experience now. And I haven't read the article y'all. So it might be in here and I'm
[30:10] going to put a pin in this question, although it would be cool to see like how you get into writing in like your writing mode, because I have a blog post about that too, sort of, please post it
[30:24] because, um, I'm going to, I also, this was the question I was going to have earlier is if y'all take a look and I find this so funny because like funny, not really funny, it's not the right word,
[30:37] but like if Ben is still watching, since they deal with the accessibility, everything, this website is way more accessible than a lot because you can listen to the article and you can double time it.
[30:51] And that makes me happy. So I love Hashnode. That's actually one of the reasons that I, that's one of the reasons that I use Hashnode instead of, um, other possibilities, uh, because,
[31:08] because of that feature. Sweet. That is something that's what we're debating. We are debating. I'm debating. Homie helps me debate on, um, going to Netlify if Netlify has a tool like this,
[31:32] um, for their blogs. So, yeah, I don't know. Um, I do, so this is, this is under my domain lauralingdon.io because you can use your own debate, uh, domain for, um, Hashnode.
[31:50] So it doesn't, like you can make your site with Netlify and still have your blog on Hashnode under your domain if you want. Yeah. And I've done that kind of stuff, like with WordPress and stuff.
[32:06] Um, I just as like in case anybody wanted to know, um, if you want to get more visibility on things, you can do con, conical, canonical, canonical, canonical, canonical. Y'all we're going to make
[32:23] a clip out of this because this is important. I didn't know what it was, although, okay. So if you go into, I'm going to edit this one just because it's here and scroll all the way down.
[32:35] Oh, I don't need to. It's like this button and there's canonical change, beta tag, canonical underscore URL. If this post was first published somewhere else, like your own blog.
[32:47] So I actually have my blog page hidden because mine, I like this look of it just being a landing page. But if I go here, this is the actual, it was originally linked. And then you put the
[33:12] canonical link here. And the reason you do this is because then a, you still have rights to the original posts in case this other website ever goes down. And then Google doesn't get mad that
[33:25] you double posted something that's saying, Oh, Hey, you, you acknowledge that you posted it somewhere else because dev two is a pretty well-known area that a lot of people post to.
[33:39] So you can still keep your own content. And so that is why I'm asking as well. And Ben has a more comments that, so no, uh, I, I mean, I, I have found because I have
[33:58] yelled. I don't really yell, but my exacerbated annoyance of reading out loud. And Ramon keeps telling me that I need to do it since becoming a streamer. And then also an MC of like having to
[34:11] I want to anyway, Ben says, so Netlify is really just a deployment target. So you can build your own website separately and then host it on Netlify. So I don't think, uh, Netlify will support a, uh,
[34:28] support, listen to this article out of the box. And sometime we got to talk about search engine optimization. It's, uh, that's such a hell of cool rabbit hole to go down. Yes. And then something
[34:44] that also makes me think of SEO for search engine optimization is the fact that if I remember correctly, an annoyance that Ben had is that people would use alt text for SEO and not for
[35:00] image description. And I think that would be a really interesting topic to bring about SEO because SEO is important. It is really difficult and it takes time. Or is this new saying that,
[35:17] I don't know if I heard it somewhere, but consistency takes time. It's really annoying. Yeah. I have not done any SEO. I have read a little bit here and there and just being like,
[35:35] oh my God, that sounds exhausting. It's, um, where, like if I Google stuff, like I've noticed in my own, cause, cause this is what I do y'all. Um, I don't know if it's,
[35:50] it's like Google myself just to see what is getting the best SEO. Um, and it's, it's not bad, but I'm like, this isn't me. This is the, I mean, I'm on this podcast, but that's somebody else's
[36:05] podcast. And that's why it always like amazes me. Um, but develop Cato, develop Cato is something that I use very often. And I'm a develop Cato is not the first post. It is a develop, uh, develop
[36:26] Cato's practical field guide to saying, fuck it. And I'm like, what? So it's a very interesting, Hey, next nation came up. That's exciting. Okay. Anyway. So Ben, um, has said that a great person
[36:42] to talk to about SEO from a Dev's perspective is Monica Lent. And, um, I actually, I had a newsletter from her. It might've been around the time that I, I was going to, Oh, I was trying
[36:54] convert kit. I think is what it was. Yeah. And yeah. So yeah. Tons of information from Monica about SEO and I am just, I'm too tired. Um, Ben, please introduce us. And also,
[37:12] um, the other person that you introduced me to many, many moons ago that I was texting with, I believe she gave you, I hope you know who I'm talking about just so that way I can,
[37:31] uh, Oh yes. Thank you, Ben. Now I know who to follow up with. I forgot their name. Yes. Yes. Thank you. Thank you. Um, and Monica let's, well, we'll see if Monica will come on.
[37:47] I mean, we've had random, very well-known people on the show, so who knows? Maybe Monica will say, yes, you never know. Okay. So thank you for the random, uh, let's go down the rabbit hole of
[38:04] accessibility. Now that I'm looking at your, uh, blog posts and I'm so excited about this. How would you say, like, if I'm like, I want to go get a freelance job of a technical writer
[38:19] and I need, and they have no, like, how do I say this? Do most companies have like something written and you have to rewrite it or you just start from scratch or how do you even go about it?
[38:37] I guess I don't know how to address most, I guess. Okay. So probably unless you're, unless you're getting hired by a company that is brand new baby startup, right. Um, that probably
[38:59] there's something written down somewhere, um, that needs to be revised and edited and built out from, um, and yeah, so it's unlikely that you're getting hired to
[39:18] instantiate documentation where there existed exactly zero documentation beforehand. Probably that's not the case. I don't know if that answers your question.
[39:39] Instantiate represent as or by an instance. I'm Googling words. Oh, um, uh, like create from nothing. Oh, okay. So a lot of times you were creating from something and just updating stuff
[39:56] or finding out information and making it consumable. Yeah. Yeah. Okay. How do people hand you stuff that they want documented? Like how do you know what to document?
[40:11] So, I mean, it will depend a lot from team to team how this would work out. Okay. Um, on my team, the way that it's working out is when I started, it was kind of a brand new baby startup because
[40:27] it was only eight months old when I joined, but there were already, yeah, um, some docs. And so my, like the first thing that I did really was actually an accessibility thing, um, going through
[40:43] and fixing links because we had a lot of links that were like, click here and here is hyperlinked for information about blah, blah, blah. And so then what that means is that if you're using a
[40:57] screenwriter to see like a, or here rather, um, a list of all of, of like the links on the page, like for navigational purposes, then you've got like seven links that are all just here, here,
[41:10] here, here. And that's not useful at all. And so learning about like, okay, so what, what information should be in that hyperlink? And so rewording sentences so that they'll
[41:26] make sense. Um, and, and keeping, putting the information that's useful in, into the hyperlink. And so that gave me kind of a tour of our entire docs base. Um, because I was going through every
[41:43] single page to look at every single hyperlink and say, okay, so what would be, what would be, is this sufficient or what would be a better, what would be more useful, um, in this,
[41:58] in this case for this hyperlink to read instead of here or whatever. Um, and so that, that turned out to be great. And then, um,
[42:09] from there we had kind of a, we've, we pivoted our product a bit. And so it was like, okay, so now we need new docs for this new thing that we're doing. And, um, that meeting is in two days.
[42:25] Um, and not, I mean, I've done, I've done a lot more docs stuff like in the intervening time, but in terms of, but that was basically working with
[42:36] refining docs that already existed. Um, and spending a lot of time looking at the docs for other sites, actually Netlify is one of them. I really like Netlify's docs. Um,
[42:50] and sort of for two reasons. One is to get inspiration for how to do things and like, what looks nice and so on, but also what would people expect? So like, if most documentation
[43:06] sites, um, start have like a, a get started link with like a quick start, um, then people would expect that. And so you want to have that and physically like, where is that in the navigation?
[43:22] And usually it'll be like in the left-hand navigation, like sidebar, pretty much toward the top. Whereas with in my company, we actually had it kind of buried in a, in a sub menu.
[43:38] So you had to like know which of our projects you wanted to work with before you could get to a quick start. And so that meant you had to, you had to understand the differences between these
[43:55] projects and which did what, and that kind of stuff. And there were a lot of discussions about naming of things, um, and so on like things like that. So a lot more sort of philosophical stuff
[44:07] and like little fiddly things that don't feel like it feels sort of like you're just, you know, rearranging. I mean, you are actually just rearranging things, but it's, it's a lot
[44:17] of research into where would people expect to find this information? Where do we currently have this information and how can I make this information conform to what people would expect
[44:30] so that they can have the best user experience possible. So I've been doing for the last like six months or so, mostly UX improvements to our docs, not actually so much rewriting the docs
[44:50] as rearranging the information, not just in the sidebar, but like within the pages themselves, just reorganizing the information to make it easier to access, um, both for literal accessibility and,
[45:03] and just for general, where do I, if I landed here, what, where would I, where would I go? Where would I think to look? Um, and why am I here? You know? So what would you do to,
[45:19] I guess, like, how would you choose to organize that? And again, like, where did you get your information to, like, I, I understand, I guess, the part where you're going through and making
[45:42] it more consumable. And I feel like that would have to be a bit more intuitive than anything. Um, and also with the accessibility of the linking and then also, um, like the UX of making sure that
[45:58] it it's consumable that way. But a big part of why I'm asking is when I've had to do videos for companies in the past, people have just been like, Hey, I'm going to record the screen grab.
[46:12] So to talk you through it, meaning me, and then I have to go rerecord it with fanciness and talking through all of it. So is that kind of how, like, if somebody hands you a doc that needs updated,
[46:23] or if you need something updated or more detail of something? And also, I know this is a very multifaceted question, but I kind of think they go together of, does that mean that you have to
[46:35] physically go through the motions of the doc to make sure that the doc is correct? Oh, yes. Oh, yes. Okay. Um, yeah. So, so that's, that's sort of what, um,
[46:50] so that's sort of the other place that I've spent the most, the majority of my time. Um, I did not already know anything about WebAssembly when I joined this company. So I had to learn
[47:06] about WebAssembly. And I had to learn about our product. And our product has changed in some pretty fundamental ways. And so that has happened more than once, where I had to, like, spend some
[47:19] weeks plural, just being like, so what are we building? Because if I don't know what it is, good luck people reading the docs written by me. So, so that so yeah, so, um, when I am writing
[47:38] our docs, I go through, um, I would link our, our docs right now so that I could physically show you but the thing is that they're, they're the ones that are available are way out of date. Because
[47:52] we're bringing out, we're bringing out a new thing. And, and so on. So it's, it's too bad. Next in like, two or three weeks, then I could I could show like the differences between what how
[48:07] our docs currently look and function and how our docs now function, or then then now so that actually might be a fun thing to do in a few weeks when that's when that's finished as I can show
[48:21] like, I think yeah, because I think like you've given us an idea of like, we're to start on docs just because I feel like this is a very, and y'all I did do a stream many moons ago about docs and
[48:40] with a diet taxes diet. Oh, yeah. And that was a pretty cool way of setting this up. And I did really enjoy that, that stream. Yeah, I feel like this is something that needs to be done
[49:00] like multiple times because it is such a, it is a theoretical it is as we I said earlier, like a bit of intuition, at least that's what I feel it is that doesn't mean it is.
[49:12] And then also the practice of what goes into it. So I feel like this is not going to be the end of the conversation. No, I'm going to link a book called docs for developers, which is, it's just
[49:32] incredibly helpful for figuring out how to put your documentation together. There are lots of really good books. Actually, I'd link more. Okay, I'm going to just link yet another blog post.
[49:50] I dig it. Okay, I have another blog post on my favorite technical resources. And tech writing in general, or specifically, as a side note, just telling Laura this before
[50:17] we stream next time is Laura, we got to get you logged into stream yard at the same time. So they post all three. Yeah, how do we Okay, we I guess we can talk off. Yeah, we'll do that next time.
[50:31] Because I've seen that you don't have access to it. And I'm like, Oh, that's dumb. I need to make sure you have access to it because I'm copying pasting them. Which is fine, which is fine. And
[50:43] I totally dig it. I'm just going, Oh, I probably should have thought about beforehand. But that's okay. That is totally fine. Yeah, so lots of lots of good books. That one, I think is a great place
[51:02] to start docs for developers, because it just gives like a really great kind of overview of I mean, it's not just an overview. It's actually really quite specific. It's just Yeah, I would I
[51:16] would consider that. So when I used to homeschool my older kids, and in the homeschooling world, you very often had something you refer to as a spine. And you're like, Yeah, so this is our spine.
[51:29] And then we're supplementing with whatever. And so like, this particular some some textbook or book or whatever would be like, forming the basis of the content that you were covering
[51:41] for that particular topic. And then you'd be bringing in these supplemental resources. So I would I consider that my spine, the docs for developers, book, and then everything else sort of
[51:58] comes out like is sort of supplementary to that. The the diataxis method is a strong contender for being like a co spine, but that doesn't really make sense.
[52:11] It could, you know, it'd be like connected to be connected up at the hips. So they have two spine up to two heads. Oh, there you go. They're like Siamese twins. Yeah, yeah, yeah. Also,
[52:27] I'm posted. And this reminds me of somebody that could be really, really good to be on the show is Adam Duvander, because he owns, runs every developer and talks about developer experience
[52:43] and developer marketing. And from what I've gathered, it's like, is so much of developer experience and developer marketing is the docs of how usable they are. And I'm mattering on that,
[52:59] like, you want to think of that as necessarily marketing. Yet, if you want developers to use your product, the first thing they're going to look at is your docs, which is Yeah. Oh, Ben has
[53:13] a they Ben likes the diataxis system, but they think that they're very, very insistent that their four categories should never mix or intermingle. Whereas they prefer to think
[53:29] of them as helpful guidelines that you can break with intent. Pretty same. That's good, because I'm not good at like, just staying in my lane. Mm hmm. I like to find rules to break them.
[53:43] Yeah, so I like it, too. It's sort of a, I got check for me, like, okay, so is this content, should this content be in one of these four categories? And I've sort of like, for me,
[53:59] it's like, almost all the time, the four categories should be like sacrosanct, we'll just keep keep things in the four categories. But if there's if there's a good reason for
[54:11] straddling a couple of categories, then that's okay. But it's sort of a an opportunity for me to reflect upon, like, why do I think that this needs to straddle like that this is a candidate
[54:25] for straddling these two categories? And is that like, for my benefit? Because it's easier for me to write? Or is it for the user's benefit? And if it's for my benefit, that's not a good enough
[54:39] reason. But if it's for the user's benefit, that is a good enough reason. And that's kind of my decision boundary. Ben, do you ever stream you making a doc? Because I honestly just want to
[54:55] like, have one of you stream and talk out loud the process of you making it. Like, I'll co work with you at the same time. So that way, I can just like get stuff done. Because I feel like
[55:08] I started my stream. That is exactly what I was going to do. The problem was that it we used to be I was what I was documenting was open source. And our pivot was to closed source. So I can't
[55:24] stream it. But we still have an open source project. And that will be needing some documentation. And so that but that's coming the docs for that will get updated after the new docs for the enterprise
[55:41] product are finished. So sometime in the next six weeks to eight weeks, maybe because of holidays, I should be working on the open source docs as well. And so those I can stream.
[55:55] And I think that would just be Yes, Ben, keep us posted when you return from your hiatus. And I think that's like something that I and I'll just selfishly say it that that could be like so
[56:14] helpful is being able to just honestly see how somebody is doing it. Because that's something that I've noticed quite a bit is people are like, Yeah, I'm gonna do this and go from x, y, z. And
[56:25] I'm like, No, no, there's something. Yes, that was exactly it. Yeah, yeah. Yeah. I honestly would. I would watch it. I would I would co work at the same time while one of you were doing that because
[56:41] you both are entertaining is entertaining still a compliment when it comes to streaming. It sounds like the kind of thing that would it depends on who's saying it. Like, if a British
[56:57] person said it might be an insult. But if an American says that it's probably not. You're making me face. They're making me think and bed says that they think it is too.
[57:16] I'm thinking a compliment. Because this is something that I think streamers kind of need to have is a bit of entertainment. But at the same time, like, if you're working on something,
[57:28] it's harder to be entertaining. So that being said, if y'all are working and need a co working person to be the entertainment, I volunteer myself. I'll answer the chats and
[57:45] stuff for you. So you don't need to, or I'll be the one to ask you questions. Either one, I'll volunteer myself because I would. I have random stuff that I'm supposed to be working on,
[57:56] like being podcast stuff. Yeah. And really mean to all my own. Oh, Laura, I did. Oh, I love that rebel for hire. Yes. Yes. Um, I should get a shirt says that.
[58:17] That would be fun. Anyway, but um, okay. Words. Thank Jen. Think, think, think, think, think. Um, this was a serious question to
[58:30] know. Nope, it's got streaming of the docs and co working and something about the show that I'm, Oh, that is it. You, thank you. Thank you. We got there.
[58:50] Do you know how chapters in YouTube? I know we talked about this, but I just learned this and why it's not intuitive. Oh, so I put in chapters. That's where I was going with all of
[59:05] that. Um, because somebody actually posted about it on, um, on Twitter. And then I was like, ah, yeah, it's like non-intuitive. And they were like, yeah. Uh, and then someone else shared it. And
[59:25] that's really helpful y'all because you have no idea who I'm talking about. So I'm honestly going through my, um, notifications to see if I can find it again because somebody also shared their
[59:42] workflow as well, which I was really excited about. Um, yes. Copy. But also I need to bookmark this one, bookmark, bookmark, bookmark, copy link. All right. Um, so it's not intuitive at all. You
[60:19] actually have to put time codes in the chapters or time codes in the description. And you have to start with zero zero as your first one. So it knows where the beginning is. And I was like,
[60:32] that is, it's not, it's not intuitive whatsoever. It kind of makes sense to me. Um, sort of mapping it onto like a, like a sidebar actually in the docs. Cause I've spent a lot of
[60:55] time on this in the last month. Um, there has to be somewhere that you start. Right. And then like from there, what are the options? And so basically that's what you're creating is a nav bar.
[61:08] See, and that wasn't intuitive to me at all because I am going on the backend y'all really quick. If I go into one of these videos and let's say that I want to add, um, cards, which I think
[61:25] I'd need to do unstring. Yeah. And then I like can add this or I can add right here. This is where I thought you would do it because you have to be on a timeline to be able to do it or add an element.
[61:38] I can add a playlist right there. Like that is where I thought it would be like that would just like logically make sense to me because this is where you put all the other stuff. What you're
[61:50] saying also makes sense, but not to me in the way you do. Sure. But I now know, and I was very excited about that. Um, yeah. Yeah. It should be, there should be a tool I think is maybe what I'm
[62:15] getting from what you're saying. Like instead of manually typing out the timestamps and so on, there should be like a timeline where you're like, okay, so make this chapter one from them.
[62:29] And that would start at zero, zero and go to whatever here's chapter one. And that you're like literally clicking on there's where chapter two begins and click there's where chapter three
[62:38] begins. There should be a tool for sure. That should be the case. But, uh, what, um, they suggested in the tweet is from parasocial fix is, um, that they put it in, uh, descript, which I
[62:58] think we've talked about on this show before to translate, to translate, to trans transcribe. And then it's easier to find the text where the segments start. And I was like, Oh, this is
[63:13] anyway, I'm excited to start adding chapters and tags to them because lives don't add tags. If you have, um, captions turned on in YouTube,
[63:25] then you can do it all in YouTube without using Descript. Does YouTube allow you to see it as a full text file? Cause I'm not always, I have yet to be
[63:40] successful on exporting my text file for captions. Um, I, I mean, you can just copy and paste it. Um, but, uh, let me see, where's, I'm just trying to look at one of mine. Um, okay.
[64:05] Oops. All right. Um, um, um, um, um, um, um, you know what? I could just share my screen and that would
[64:19] be better. Do do. Reset. Share screen. Why can I not just, okay. And in here, oops.
[64:51] We lost her. She will be back. But in the meantime, I don't know about y'all, but I have been loving Mondays with Laura.
[65:15] Miscellaneous Mondays. I, I feel like I always learn way more than I thought imaginable with Laura. Like she's such a good teacher.
[65:26] And I, I know some people may not consider this a good thing, but she also always calls me on my shit. I didn't mean to close that tab. That's okay. I was just saying that I always have fun
[65:44] with streaming with you and you always call me out on my shit, which I really appreciate. Do I? You do. In a very kind way. Oh, well that's good. I prefer to be kind than not kind. Yeah,
[65:55] it's a very kind thing. I think when people challenge you to be better in a kind way, is my way of saying that they call you out on your shit and I appreciate it. Okay. I have
[66:09] your share screen. Here we go. Okay. So this is my stream from last week with Andy and I'll mute that so that we're not doing double talking here and do we have the captions and then where is it?
[66:35] There's a thing where you can see, Oh, show transcript. And so it's already got the timestamps. And so you can just like literally like click here and it's already giving you the right times.
[66:54] So I feel like that would maybe be easier than Descript just because it's literally already in YouTube. Yeah. And also it's free and I kind of think that Descript is not free for everything.
[67:12] You are correct. And I am now going and seeing if I can do the same thing you did. I feel like y'all can see my screen for this one, so I'm not sharing it.
[67:33] I, I have like just done select all and copied and pasted this into a text file before. But I don't think I would, I think that for my brain anyway, this would be a better format than
[67:52] the X, the different text file, separate text file. Oh, you know what? I think I, if I remember correctly, I also tried this like way
[68:09] too quickly, like after the. Oh yeah. It takes hours for the transcript to get generated.
[68:22] Yeah. And I think that was it because yeah, what you just said worked and yeah, it doesn't let me copy and paste them the easiest, but it still does. So yeah.
[68:39] Let me just, I'm going to go verify. Yep. It worked beautifully. Thank you for showing me your tips and tricks.
[68:54] And that helps with knowing the exact time code to put as the highlight or the chapters. Well, I feel like we talked about a lot today, a lot, a lot of random things. This is why I
[69:14] love MISC Monday. Yes, for sure. Because it's always learning, which is, I think also really fun. So it's like, it's a learning thing and we get to talk about random shit. It's like.
[69:28] Definitely. It's all the happiness. Um,
[69:34] oh, Homie said that he actually brought out hardware. Yeah. Homie joined us. Um, that was super fun. Yeah. Yeah. He, um, he showed all the,
[69:45] all these different, um, bits and bits and pieces of different types of hardware and different systems like Raspberry Pi or microcontrollers. And like, this is what you can
[69:54] do, or an example of a thing you can do with a microcontroller. And this is an example of the thing you can do with the Raspberry Pi and different, different cool stuff.
[70:03] I love that. I love that. Well, cool. Uh, yes. Yep. That is, that's a good way of saying it. But, uh, MISC Monday tips and tricks you
[70:23] didn't, you needed, but we'll use today. Yeah. Yeah. I mean, another, um, title that I had, I had proposed for this,
[70:33] this series was brain dump Mondays and it's, it's seeming, it's a little bit like, um, so I have never, I, I had my first two kids when I was really young. And so I never actually
[70:45] attended parties of like the, the late teens, early twenties variety kind of thing, but I have seen it on television. So it must be true. Right. Where, uh, people like dump various
[70:59] kinds of alcohol or whatever into like a bowl and make some kind of kind of thing. And I feel that's sort of like what we're doing with our, like brain dump Mondays is like, we just sort
[71:10] of like everybody dumps their like random facts and tricks in the bowl. And then we all get to share, except it's not gross. Yeah. I like MISC Mondays better than jungle juice y'all. I'm just
[71:26] gonna. Jungle juice. I didn't know it had a name. Yes. So yes. Uh, surprisingly helpful ideas and tips you do want to talk about. That is a good play on words. I like that one, especially with
[71:42] the show. That is fun. That is fun. Yeah. Um, but yeah. Uh, so that's all I had for today. Is there anything else you wanted to go over today, Laura? You know, I think I had some things in mind last
[72:00] week and, uh, it just got obliterated by the weekend. So, uh, I get that. Maybe, maybe I will remember. We'll put it public and then, you know, like other people can add to it.
[72:16] What's that? Put what? Ideas of us to talk about on Mondays. Like people can tweet us and then we can, we can like. I was gonna say we could have like a type form, but tweet, tweeting would make
[72:31] sense too. I mean, type form would actually keep it in the right, same area. I dig it. I dig it. I'll work on that. Well, thank you everyone. And we will see you next week for those in the U.S.
[72:50] I hope you have a good holiday week and yeah, we will see you next week. Yeah. Bye. Bye. Thanks for joining us. Oh, I wanted to raid. I always forget that I want to raid. Oh yeah. Raiding is
[73:06] good. Let's see if anybody's live right now. Ooh, we got, all right. Y'all are being raided. See you in a bit or not see you in a bit, whatever.
[73:24] Oh, it has the countdown, the countdown. Raid now. 
