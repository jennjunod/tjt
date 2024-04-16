---
showLink: "https://www.youtube.com/watch?v=TEdGp_j2JI8"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "hangout-with-jacob-evans-and-roy-anger"
title: "Hangout with Jacob Evans and Roy Anger"
publishDate: "2023-11-17"
coverImage: "https://i.ytimg.com/vi_webp/TEdGp_j2JI8/maxresdefault.webp"
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

[00:00] >> Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:08] And I'm excited because we are joined today with two humans that I am fortunate enough to call friends.
[00:16] And who are insanely smart and help me level up all the time because they call me out on making me do things better.
[00:25] So I thought, dude, bro, you got one of the cups. I need to order one of the cups.
[00:31] >> Yes. I've got a Jacob mug.
[00:35] >> I want to put a, like, make a Jacob, like an OSRG Teach Gen Tech mug. And what up, learner?
[00:42] >> Yeah, I plan on rebranding so, like, the logos will eventually change, but, like, you'll have, like, an OG collectible.
[00:52] >> Okay. That'll be amazing.
[00:54] I'm excited for that. And yeah.
[00:58] So I would say question number one. Who are you guys?
[01:02] Who are you? >> Roy.
[01:04] >> It's a deep question. >> My name is Roy.
[01:06] At some point people are going to figure out I'm an imposter and I'll never be in tech again.
[01:15] On a more serious note, I work with the developer success team at Clerk right now. And yeah, as Jen mentioned, Jacob, her, and I know each other from a bunch of different
[01:27] things, whether it's tech or gaming, and just happy to be on the stream for my second time. >> Yeah.
[01:35] Wait. I think this might be your third time.
[01:39] Were you there when we did the weird coworking session with, like, 12 people on the stream? >> Oh, yeah.
[01:47] If you want to count that, yes. >> I counted.
[01:49] >> I don't think I ever kept the episode, but I counted it. >> It was because it was my stream.
[01:56] >> Oh, yeah. That's true.
[01:58] But it was in my stream yard. >> Yep.
[02:00] >> Okay. Okay.
[02:02] Yay. >> So this is the 2.5 time I've been in Jen's stream.
[02:08] >> We'll go with that. And Jacob, who are you?
[02:14] >> Yeah. Names.
[02:16] Names right there. So I worked at Cloudflare for the last three years.
[02:25] If you use Cloudflare stuff as a developer, you've probably used something that I touched, like Wrangler, the worker CLI.
[02:35] I currently work at Clerc as well, with the magnificent Roy here. I am on the DevRel team as a senior developer experience engineer.
[02:50] So very, very fancy title. >> I dig it.
[02:56] I dig it. And to fill in some pieces here, Jacob was on my stream in the very beginning, like probably
[03:12] the first month or two. And y'all, I've been joining or, like, learning TypeScript and JavaScript at the same time.
[03:23] It wasn't like a, hey, I'm going to work with React or anything. It was a, yo, I'm going to do -- I don't know what I'm learning, because I'm just going
[03:32] to start learning. And then Jacob came on the stream to talk about TypeScript, which I don't even know
[03:44] what we ended up talking about. Headless something, I think.
[03:50] >> Workers. >> Yeah.
[03:52] >> Yep. >> Yep.
[03:54] Yep. So let's just say for anybody that watches that, it'll be painful for you and everyone
[04:00] involved, because it just was not clicking, like, at all. But it was very amusing.
[04:10] And then Roy was on the stream to talk about a lot of the behind the scenes items that I was struggling with to understand coming from a GoDaddy point of view, because I was
[04:25] learning about, like, trying to understand all these different website structures and building apps, when my point of reference was WordPress and website builders.
[04:38] Like Squarespace or GoDaddy or Weebly and those type of things. So both of those, very spaced out, actually.
[04:48] Jacob was here, like, a year ago, and Roy was here in April. >> Yeah, six or seven months ago.
[04:55] >> Yeah, if you're just kind of, like, clueless about the whole, like, what is SSR, what is client rendered, what is server rendered, what is all of that kind of stuff, that stream
[05:06] was kind of, like, a good intro stream, I think. I know a lot of people who are kind of getting into that stuff struggle with all of these
[05:15] terms and concepts, though we probably have to go back and talk about server components and server actions now, because they're here to play.
[05:26] >> I almost put Rith Rowe, like, your name was about to be Rowe while I was putting this in the chat.
[05:33] So yes, y'all, definitely something, too, that I think would be very helpful. I am curious, because this is -- it'll be fun.
[05:45] How did we meet, y'all? Do you remember?
[05:50] >> I think you met Jacob first, didn't you? I'm trying to remember now.
[05:59] >> Yep. Yep.
[06:01] Yep. Jacob hosts a Code in Life, I'm still going to call it a Twitter space, three days a week,
[06:09] the evening time in the U.S. And I think Anthony Campolo, or as I like to say, his last name is AJCWebDev, which
[06:22] is his Twitter handle, helps me get in, start TeachGenTech, and then he was friends with someone named Bro Nifty, and Bro Nifty was in Jacob's Twitter space, and I kept showing
[06:37] up, and this is a very technical Twitter space, and I kept going on -- I don't know why Jacob let me on stage, but I kept going on stage and asking lots and lots and lots of questions.
[06:49] And then they talked about D&D. And I was like, that's a thing.
[06:56] I've heard at school, I've always wanted to learn how to play D&D. And they were starting a new campaign, and Jacob said yes.
[07:07] And Roy was part of that campaign. And I annoyed the shit out of them with my character, and it was so much fun, because
[07:16] I did not understand D&D or anything. So when did you guys start playing D&D?
[07:23] Jacob, you get to go first this time. All right.
[07:31] I started playing back in high school, like most uber nerds. That was -- we were primarily playing 3.5 and the spinoff Pathfinder and stuff.
[07:53] I would say another big upsurgence of me playing D&D -- I played Magic the Gathering back then, and I did all the nerd games.
[08:13] Around right before COVID, one of my friends had reached out to me, and he wanted to start playing D&D more, but he wanted to do it remotely, because he was in Hawaii, and I was in Illinois,
[08:26] and he just didn't have anybody to play with and play seriously. And I was like, yeah, certainly, I'll play.
[08:35] And then COVID happened, and so we were playing D&D a lot. And yeah, I just got back into it pretty hard after that.
[08:50] Nice. And Roy, when did you start playing?
[08:54] So I first played when I was a kid. I don't even remember how long ago it was.
[09:03] So I'm 44. It would have been sometime around 15.
[09:08] I don't remember exactly. And I played on and off for a while, for probably about 10 years, through university and a little
[09:16] bit after. Played some D&D, played some Shadowrun.
[09:22] Played a little bit with a couple other systems, but nothing serious, nothing more than a couple of sessions.
[09:27] And then I just didn't have anyone to play with, so I had stopped playing for the longest time.
[09:33] And I started with the old advanced Dungeons & Dragons, like the second edition, the really old stuff.
[09:41] So I saw 3 come along, I saw OGL get released, and that effect on roleplaying and everything like that.
[09:53] And then I got back into it when Jacobs started talking about it, and I was like, yeah, I would like to play that again.
[10:00] That would be fun. Yeah, I didn't even remember that, Mark.
[10:05] Fact zero. Yeah.
[10:07] Fact zero. That is old.
[10:12] No idea on that one. I want to make a comment, too.
[10:18] For those that don't know what OGL is, it's called the Open Gaming License. It is probably one of the best things to happen to any type of game community industry.
[10:32] It is basically what allows people to create all that homebrew content. If you know who Critical Role is, it's what allowed them to exist.
[10:48] All the other companies that end up making their own campaigns and settings and all this other stuff, it's basically open source coding as we know it, right?
[11:02] Open source software. But it's for a game system.
[11:08] So it's a very cool thing if you look into it. Yeah.
[11:15] What is the acronym one more time? OGL, Open Gaming License.
[11:21] It's all of the core rules, so how to generate a character, what stats, how to roll, how to perform combat, all that kind of stuff.
[11:31] All the core stats are included in OGL. So all of the actual flavor content, so the worlds, the campaigns, the stories, all that
[11:41] kind of stuff is all-- that's not covered by OGL. That's specific to the particular book that you purchase or license that you purchase.
[11:50] But yeah, OGL is free to use, so you can create your own content. And you have a really tried and true game system to build off of, instead of if you're
[12:01] building your own content, trying to come up with a game system that works and doesn't suck.
[12:06] So yeah, it's pretty awesome. It's a huge stepping stone to creating your own content.
[12:11] You don't have to do any of the rules. You just create the world and publish the book, and away you go.
[12:17] So it's awesome. I'm trying to read what Chris wrote, which, by the way-- OK, so many thoughts going on
[12:27] at the same time. Taking a few steps back.
[12:32] So when we were talking about gaming, there are multiple versions of gaming and different ways of gaming that is-- some of which we've talked about already, some of which we haven't.
[12:47] But there's video games that you can do on your phone, on the computer, on gaming systems like Xbox or PlayStation, those type of things.
[13:00] Within that, there's subsets of areas of gaming, like an RPG is role playing, meaning that you are-- it's like a story.
[13:14] There is first-person shooter, which is something like Halo, where you can play more violent games we're going to go with.
[13:31] And then there's also something called an MMORPG, which is a multi-- Massive multi-online.
[13:42] Massive multi-online. Massive multi-online gaming.
[13:48] And then you also-- so I'm going to put those on pause, because I do have a story there. And then you also have tabletop games and card games.
[13:59] And so is Risk considered a tabletop game? No.
[14:05] So tabletop games would be all games that you play on a table, like Sorry 2, any type of board games?
[14:14] Yeah, it's all tabletop games. OK.
[14:17] And it's interesting-- Anything that is a board that you put on a table--
[14:22] Is a tabletop game. Which is weird, because it makes me think about when we talk about D&D or Dungeons and
[14:33] Dragons or-- right now, we're doing a campaign in the Expanse, which I will go through in a bit.
[14:40] But by that, I mean, I'm just going to ask Roy to talk about it. Those are considered tabletop and not called board games, where board games are technically
[14:51] tabletop games, too? Yeah.
[14:55] So how would you define a tabletop game, especially since we're talking about D&D? Well, it would be a tabletop role-playing game, TTRPG.
[15:07] Ooh, more acronyms. That is exciting.
[15:12] And my journey to get to gaming and all of this is I started with video games, playing like Crash Bandicoot and IQ Cube and Mario Brothers and those type of games on the original
[15:30] Nintendo, then PlayStations, and Xboxes. I've been an on-again, off-again gamer-- on-again, off-again gamer.
[15:38] Until I found World of Warcraft. And I became a hardcore wower, which is a mass multi-online-- what did we say it was?
[15:54] Massive multiplayer online role-playing game. Yes.
[16:00] So I became addicted. I played for two years and was calling in to work and stuff, to raid.
[16:14] And a raid-- and I'm bringing all of this up for a reason-- is a raid is where it's multiple people playing for a specific outcome at the same time.
[16:26] So everybody working as a group to get an outcome, right? Basically, yeah.
[16:32] So everyone on a mission together and trying to succeed. Yeah.
[16:38] Okay. So these raids would be scheduled at a certain point, and you would all have to show up at
[16:44] the same time, and I would call in to work for it. And that is when I realized I had a really bad addiction to it, and yet it also helped
[16:53] me grow as a human and get out of a bad space in my life. So with that addiction, though, I quit cold turkey.
[17:04] I was like, I'm never playing video games again, or any games. Just not going to happen.
[17:09] And I'm glad I finally came back, but that was in 2010. And I didn't play very many video games until the last two years, three years, when I had
[17:21] brain surgery in 2020. I started playing video games again because I had nothing else to do.
[17:26] And then I found tabletop games, which is like just D&D was my total game changer. It helps me understand and talk to conceptualize tech, but also challenging different sides
[17:43] of myself, because it's also like improv and acting and role playing. Exactly.
[17:51] It's role. Yeah.
[17:53] That's all those things. Yes.
[17:55] How would you define role playing then? You take a role and then you play it.
[18:01] Jake, with the most literal, literal definition ever. No fun in Jacob's definition, just exactly what it is.
[18:11] It's exactly what it is. So are we talking about like a rolling pin?
[18:16] I take a role and I just play with it? No.
[18:19] A role like R-O-L-L. No, no, no.
[18:21] I was just taking his literal definition into account. R-O-L-E.
[18:26] Role. The role you're playing right now.
[18:32] And it's helped me so much with my job overall and playing well with others because they make me level up in life on everything.
[18:41] So I'm curious, all of this is a big explanation to what is OSRG? Oh my God.
[18:51] All right. You're welcome.
[18:53] You're welcome for that really big buildup. So, all right.
[19:01] So OSRG is a community that I started. It actually was kind of a spinoff from Kent C. Dodds' Discord server where I saw some
[19:17] people doing some like kind of like crowdsourcing of like working on open source projects together. And I was like, hey, I have an idea.
[19:28] So I'm a huge fan. I have like I've written articles in the past and done a lot of research on gamification,
[19:36] crowdsourcing and stuff like that. And I'd heard about mob programming when I first started coding.
[19:42] And so this whole community is like core principles where basically we were going to go using crowdsourcing of essentially a bunch of developers and our time and whatnot.
[20:01] We're going to go and find open source projects to raid, right? Because this is the gamified aspect is we were to start creating a game system, right?
[20:14] Think like how D&D has rules. We were to create a game system that has rules, that has stats and all kinds of other stuff.
[20:28] And we would basically mob program together massive problem domains that were very simple. So a big problem domain that is very simple would be something like refactor all your
[20:39] tests from enzyme to React testing library. That was like the big one that we were doing at the time.
[20:45] Or JavaScript to TypeScript was another one that we could do. And we'd find projects where it was like maybe like a handful of maintainers with a big popular
[20:57] project or even a medium sized project that's still very popular or heavily used. And they're just drowning in issues, right?
[21:07] But they have like these like big tech debts that need hurdles that they need to get through. One of our biggest ones is still to this day is a bit of like a magnus opus to this idea
[21:22] that like it can work. It could work.
[21:25] It did work. And that is hospital run, where they had thousands of tests, hundreds of files, they had one
[21:37] maintainer assigned to convert it all to enzyme, update all the tests and make sure that they're all passing.
[21:44] That one maintainer they projected like was going to take like, I don't know, like a year or so, maybe more.
[21:51] They were definitely drowning. And we came in.
[21:55] And at any given point, there was like five or 10 people live sharing like a VS code instance, while we're all coding like in the same file or adjacent files.
[22:10] And we would just be kind of on a call like we are now, but it'd be like, you know, five to 10 people at a time, a total of 27, I think, contributors, and it took only 30 days to
[22:20] do the entire thing. Wow.
[22:23] That's actually really cool. I never knew that's how OSRG came about.
[22:29] Yeah, yeah, I used to talk about it a lot. The origins like, like, like, over a year ago, but I stopped recently because it's,
[22:39] it's still a learner community, which is what I wanted to be. It's still a developer community, which I wanted to be.
[22:46] But it's also evolved a bit into like a gaming community. And it, you know, it could still be all those things.
[22:56] And eventually, maybe, you know, what it was before, but no, no rush here. The the community itself is, is, as Jen knows, I'm very much like a huge fan of bringing
[23:13] people in and letting them kind of build out their communities. And actually, Dio was one of like, he was very interested in the concept as well early
[23:28] on, and had like, hung out in our discord, but eventually he created his own company discord and then eventually created his own personal discord for for streaming and stuff.
[23:40] But I'm perfectly okay being a launching pad community for other streamers and other other people making really cool stuff.
[23:50] So you know, at some point, if Jen decides, I'm gonna go create my own discord, the support that 100% you know, for Roy's like, I'm gonna go create my own community somewhere and support
[23:59] that 100%. That's
[24:01] I don't even stream on my own channel. It doesn't have to be it doesn't have to be streaming Roy, Roy, Roy, for all I know, is
[24:08] gonna end up creating like the next like, you know, breakthrough technology. I don't know.
[24:14] Yeah. So like, we never know.
[24:16] And so like, the best thing you can do for people in a community like that is just support each other.
[24:23] And that's, that's really what it's there for. And that's a, oh, yes, I agree with that, Jasmine, there, there's something really cool
[24:35] about the community in the fact that it's y'all who got me started and kept me going of my learning and also building out my communities.
[24:48] Yeah. And this is something that I really, I wish I could explain in, like, tell people more
[24:56] about is there is a lot of there's a lot of tech bros out there in the world. There are a shit ton of tech bros.
[25:06] And by tech bros, I mean, at least my lingo is like, male figures that yeah, and are condescending and especially to women or diversity, and it's really hard to break into tech and especially
[25:24] when you deal with them nonstop. And having these two around of Roy and Jacob and being an OSRG gives me hope of seeing
[25:35] that there's supportive dudes out there in the world that want to see others succeed and build them up instead of just doing it for their own benefit.
[25:48] And that's something that I, I don't think it's talked about enough and a big reason that I wanted to join the community because when I was talking about starting my own discord,
[25:59] they were like, yo, who's going to moderate it? How are you going to moderate it?
[26:03] How are you going to do all of this? How are you going to think that through?
[26:07] Which doesn't always happen. I kind of shoot from the hip and then they tell me to maybe think this through a few
[26:13] steps. And part of being in that community is Roy, you started talking about building a keyboard.
[26:24] That's really cool. Tell us more.
[26:27] Yeah. I mean, it's just one of my hobbies.
[26:31] Let me show you the one I'm using right now that I just recently finished, not the best camera for it, but yeah, it's basically when you look at doing like custom keyboards, you're
[26:49] basically choosing the different parts. You're choosing like the, the keyboard case itself, which a lot of these are like their
[26:58] custom ones and no, it's not a new fee. This is a TGR Tomo.
[27:06] So it's a CNC aluminum case. Like you can even see like, this one isn't the best on the back.
[27:13] If I have my mammoth, come on camera, she has like a silver back with like a, yeah, the stuff is like cutting it out.
[27:25] My mammoth has this beautiful, I'll check it. I can share a link to the actual keyboard, but my mammoth 75 has this like beautiful
[27:34] stainless steel back with this like slightly 3d gold elephant on it. It's absolutely gorgeous on the back, but yeah, you pick your case, you pick your switches,
[27:45] you pick your key caps, and then you usually like modify the switches. So like I use tactile switches and I'll, you open them up and you lube them.
[27:55] You'll sometimes do film, which is like a gasket between the top and the bottom to change the feel and the sound.
[28:01] And then sometimes even do like a swap the springs to make the switch stiffer or lighter to use.
[28:08] And then you assemble it all together and have a keyboard that, that really suits like what you, what you like, how in terms of feel, in terms of look, in terms of sound, you can
[28:19] probably hear this. I don't know how well that's coming through, but like it's, it's all custom lubes.
[28:28] So it has this nice smooth sound to it. There's no like scratchiness or like spring ping that you can get from other keyboards.
[28:34] So I've got, what do I have five, five right now, custom keyboards and kind of switch between them depending on what I want to feel and what I want it to look like and stuff like
[28:44] that. That's pretty dope.
[28:50] I will say that is something that I think is so cool. And then I'm like, oh yeah.
[28:57] And then I can hear it type. And then even if I get a keyboard that is for myself and no one's around, I'm like,
[29:02] I can hear it type. And for other people, it's so calming.
[29:08] And I love that. And now something that I realized and asking about the keyboard stuff, because it started
[29:16] quite the conversation in the discord of awkward segue from me is what is it like working with newbies on any of this tech or gaming stuff?
[29:31] I like it. It's for me, it's, it's fine.
[29:35] I don't mind helping people out. I don't mind talking through it and teaching people.
[29:40] I think that's different for everyone. Like there's some people that are better suited to that.
[29:44] And some people that should probably never talk to someone who's new, because it's not good.
[29:49] It's not their personality. So don't keep them away from the new people and keep them in the closet in the back and
[29:55] just doing the hard work. And there's people in between that to different levels.
[30:01] So I think it's finding what works for you. And if it's not your strength, don't do it.
[30:09] Don't talk to people who are new. Go help other people.
[30:14] Like I love Theo, but I can't imagine Theo teaching new people. Not his jam.
[30:20] He would probably lose his mind pretty quickly, but sit down and talk about like more advanced topics and he would be fine.
[30:27] So yeah, he doesn't like when I ask questions during Code in Life that are fundamental questions, not advanced questions.
[30:39] Yeah. So I find working with people that are new to anything, right, D&D, networking, soft
[30:53] skills, which is still poorly named. We need to find a better name for that as just as a culture.
[31:01] Human skills. I feel like soft skills are human skills compared to technical skills.
[31:07] Human skills is, yeah, I like that. But the overall, just like teaching and working with people who are new to something.
[31:24] First off, I have a fondness for the Feynman technique when it comes to teaching people, which is basically just a concept of like a principle of like, if you are unable to
[31:42] explain it to a five-year-old, you don't know it well enough to explain it, right? Or teach it, is the other way of putting it.
[31:52] But the idea there is you have to have such a fundamental understanding of something that you can create analogies and metaphors and these ways of connecting the information to
[32:07] how the person is thinking about something or how they personally think about things. Maybe they have things that they can relate it to and you can try to create some sort
[32:19] of analogous situation to their knowledge that they already have, which fast tracks them to fully understanding this thing as it is.
[32:32] That is a skill and it is part of being not just knowledgeable, but charismatic in your knowledge, i.e. wise, and you have to practice wisdom.
[32:45] Wisdom doesn't just grow out of a tree or come out your ass. So you have to practice it.
[32:51] And so like working with people who are new all the time is something that I think fortifies and builds those skills themselves for yourself.
[33:04] Follow-up question on that one of, I know that I love driving you two insane of, I don't know what I'm doing.
[33:17] I'm going to try doing this thing because I think I know what I'm doing and I think I can figure it out.
[33:22] But if not, can I, like, try to, like, how do I say what I need to Google it and give you enough information to be able to answer my question of what I tried to do?
[33:41] How do you suggest people do that? Or as Jason asked, any tips for newbies approaching elders?
[33:51] Yeah. Don't call them elders.
[33:53] Well, it depends on how old they are. It's probably okay to call me an elder because I'm older than pretty much everyone here.
[34:02] No, joking aside, though, the first things first is there's lots of content out there that's not just tech-related, but a lot of tech people have created this as well.
[34:16] Things like don't ask to ask, right? That's a big one.
[34:22] There's a lot of content around that. How to create an email for a busy person.
[34:29] If you go look at Syntax FM, the podcast, they have episodes on both of these topics. Those two things will actually get you really far.
[34:40] If you go learn how to email or DM somebody who's busy, and you also learn how to ask a question, and you're like, "Learn how to ask a question," and you just ask the question.
[34:55] No. No, not at all.
[34:58] No. If you come and ask me, "Hey, I have a question.
[35:02] Do you have time?" I'm going to be like, "Nope, I don't have time."
[35:08] If you come to me and you're like, "Hey, I have a question about this. This is what I did.
[35:13] This is the context behind it. This is the research that I did."
[35:16] If you come to me with that already, I'm going to be like, "Yeah, let me help you out." Yep.
[35:25] To expand on that, what Jacob's talking about is don't come with a super vague, open-ended question.
[35:33] There's obviously literally don't say, "Hey, is it okay if I ask a question?" That's the bare minimum.
[35:41] Even beyond that, it's like, don't come to us and be like, "Hey, do you mind if I talk about auth with you?"
[35:49] That's open-ended. Are you talking about clerk in specific, because obviously, we both work clerk?
[35:54] Are you talking about auth in general? Are you talking about OAuth?
[35:58] Are you talking about password/email auth? Are you talking about SAML auth?
[36:03] That's just like the tip of the iceberg. Are you talking about auth and how it applies to user management, organizations, roles?
[36:13] That question, "Hey, do you mind if I talk about auth?" It's that if you've ever seen, and most of you probably have, the whole picture of the
[36:21] iceberg, how there's that little tip of the iceberg above the water, and then the bulk of it below the water, you're asking about that little tip, and the answer could be anything
[36:29] that's below. That's a hugely hard question to ask, because one, we don't know what you're asking, and
[36:37] two, we don't know how long we're going to take answering your questions. We're going to be hesitant to say, "Yeah, sure," because we don't know if that's a five-minute
[36:43] conversation or a five-hour conversation. We don't even know if we actually have the right auth information to give you, because
[36:51] maybe you're asking about something that's outside of our field of expertise, or the product that we offer, or whatever the case is.
[36:58] Asking a more specific question, like, "Hey, I have some questions about OAuth and how to set it up," or whatever, that frames the conversation ahead of time, and then the person
[37:09] that you're asking knows, one, do they have the knowledge to help you, and two, they have a rough idea of what that help could entail, and what they're committing to by answering
[37:20] your question. You're putting that person in a better spot, and that's kind of what Jake was referring
[37:27] to as well, with how do you email busy people, it's the same idea. When you send emails that are super open-ended and don't have information in them, the person
[37:36] on the other end is like, "Why do I want to respond to this? I don't know what I'm getting into.
[37:39] I don't know how much time and effort I need to answer these questions." When you send an email that has specific questions, then that person can evaluate that email and
[37:48] answer those questions, or if they're too busy or whatever, they can obviously say no, but you're much more likely to get a response when you have those specific questions.
[37:59] The other thing that I'll add to this, and this comes from my work as developer success where I'm talking with developers that are using Clerk's product all the time every day,
[38:14] we're going to ask questions back, and when we do, answer them, and answer them as specifically as you can.
[38:20] We don't want stories or a lot of information, just give us that answer, and the reason I say that is because we're usually asking those questions to narrow down the answer or the
[38:30] information we need to give you or the suggestion we need to give you, and if you don't answer our questions, it's super frustrating because we're trying to help you and you're not meeting
[38:40] us in the middle by answering those questions. If you're approaching someone for help and they ask you something, definitely answer
[38:47] that question, definitely meet them in the middle. And something that I do really want to call out, and you two have been great at it, and
[39:00] something that I see a lot of from people that are joining the tech field, any field in general, but specifically the tech field is something that I've heard quite a bit is,
[39:14] oh, go find yourself a mentor. Trying to find a mentor, A, is really difficult, because if you just ask somebody, hey, will
[39:20] you be my mentor, they're going to probably say no, because they don't know you, and that's a lot of work and effort and follow-up, and it's definitely something that you can have
[39:34] mentors without calling them your mentor, of people that you can ask questions and have a dialogue with, and also asking in return if you can follow up with them as the process
[39:51] is going. Instead of saying, hey, can I talk to you once a month for the next year and a half
[39:58] for me to get through this project, if somebody asked me that, I would straight up say no. I would just be like, no, go away, go buzz off, where if we're saying, Roy called me
[40:10] out on the fact that I keep trying to work on all my websites and I am doing a million things and asking different people to try to get it figured out, that both Jacob and
[40:23] Roy and our expanse team was like, Jen, you kind of need to stick with one person and stop trying to ask everybody for help, because you're just making it worse for yourself.
[40:33] Not specifically one person to jump in, but more like one lane. Don't go to a NeXT expert and ask questions, and then an Astro, and then a Solid, and then
[40:44] a Svelte, and then a Vue, and then a PHP, and then back to NeXT, and then back to PHP, and then to Vue.
[40:50] And then for some reason Kafka. Kafka.
[40:52] I don't even know how you would fit that in there, but sure, yeah, a hundred percent. I do, and I bring these up because there was a lot of growing pains for myself, and I feel
[41:15] very fortunate with these two specifically, because I've currently been stuck on one thing that I'm working on of understanding a specific part, because Roy was like, I'm not helping
[41:29] you until you get past this point, and you have to understand it, which is really helpful, because I know that I need to understand it to be able to not just make something work,
[41:41] but understand why it works. And it can be hard as somebody that has worked with others and talked to newbies about other
[41:52] topics, it's hard to not want to fix something for them and just give them the answer. And it can take a lot of time for somebody to be like, oh, you've got to go figure that
[42:05] out yourself, but I'm here when you get to that point, and that's why I wanted to ask about how people ask questions, because that's where it all starts, and having community
[42:21] is such a big part of that, because asking one person all the time, which I'm pretty sure Theo has talked about this before, I like to pick on Theo, if you DM him every
[42:33] single day asking him the same thing, and asking him for help, he will probably just yell at you, or ignore you, and where as if like I've messaged him when I first started,
[42:49] and I was like, hey, what do you use for X, and I think I was asking him about a mic or a camera or something, and that's going to get a response, because it's a very short
[42:58] yes or no answer, where, hey, Josh, you're a perfect reference for this, where somebody that there was a win-win of I'm learning TypeScript, I have been using Josh's book, Learning TypeScript,
[43:14] and Josh was coming on the stream once a week so we could learn together, that was very synergistic instead of just like, take, take, take, take, take, oh, yeah, you got the book.
[43:26] It's another thing that I've been stuck on is I really need to learn about classes, and I will get there, and this is also why Kafka just randomly shows up in the conversation
[43:36] is because I also have to learn the company I work for, and then I just randomly throw things at all of you, and it's really fun. Yeah, so go ahead. Go ahead. Okay, I'll take
[43:50] it. No, I'll take it now. You already passed it. So the thing that I wanted to say is, because this is going back to the mentor stuff, and I've been talking about this for years
[44:02] now, one thing is I tell people you can have role models that you can interact with, you can talk to, you can, you know, follow how they do things without asking them to be your
[44:21] mentor. What Jen has been describing, too, about reaching out to certain people and building these relationships and getting help from them, that's just networking, and that is
[44:43] also a key part of that is you're networking for a support network, right? So you have a network of people who will support you when you need it. I reached out to a friend the
[44:57] other day, because I don't know Remix all that well, but I know that Maple Leaf is one of the best Remix individuals out there, and I was like, "Hey, can you make sure that my
[45:07] Remix doesn't suck because I'm making this reproduction?" They were super happy to help. I know a dozen people that I can reach out to do that with, and that takes a place of
[45:23] the role model and your support network takes place of this mentor that people usually think about when they're thinking of mentorship. When I talk about mentorship, I'm actually
[45:34] usually referring to something more along the lines of somebody who's actually more sponsoring you, like a sponsorship. What that means is that they are investing time, energy,
[45:46] resources, even potentially money, their own network, right? They're putting their neck out there for you in some cases, maybe giving you referrals or vouching for you directly
[46:00] to higher-ups. These types of things, those are what I think of when I say mentorship, and it's more of a sponsorship. Now, that's the type of stuff that I provide for people
[46:11] that I think not only are reaching out and asking me for mentorship, I'm not going to do that. I'm going to basically give you the, like, "Here's what you actually need. You
[46:23] need a community," right? There's just some people, as you build that relationship with them, that type of mentorship, that kind of sponsorship, just happens. It's like a burgeoning
[46:36] part of that network. For instance, with Jen, I've spent a lot of time helping Jen. Would I do that for literally anyone out there? No. No. That's something that happened through
[46:54] the networking and through building that relationship. When people talk about, like, networking is really important, it's because it leads to that mentorship that you probably are thinking
[47:05] of, that you're like, "This is what I want for my mentorship," but you're DMing them on Twitter. That's not going to get you what you want. You have to go about this. It's
[47:18] kind of a long game. That's my take on the mentorship stuff. >> Yep. I was going to speak on that as well. It echoes a lot of what Jacob said. Jacob's
[47:31] heard me say this. He doesn't agree, but it's still true. Jacob is definitely a mentor to me. You can see him shaking his head. It doesn't make it less true. The reason I say that,
[47:43] and I've never once gone to Jacob and said, "Hey, can you be my mentor?" And he's never once said yes or no. If anyone comes to me, or I think anyone really, and says, "Hey,
[47:55] can you be my mentor?" For the most part, you're going to say no, because the people who do that probably don't know you. The people who are coming and saying, "Hey, can you be
[48:03] my mentor?" You've probably barely interacted with them, or never interacted with them. I've had people do that. I'm like, "I don't even know who you ... How do I even know you?
[48:12] You're DMing me on Discord, and I've got to check and see what server they're on to figure out how they found me. Oh, you saw me on the Tailwind server, and I haven't posted there
[48:22] in three months. Why are you DMing me? What is happening right now?" That's not a way to get a mentor. Even if someone says yes, they're not actually going to help you in
[48:30] a significant way, because they don't know you. I think the approach is that I've taken, and I think that helps people, is be part of the community that shares your beliefs
[48:47] and your goals. I started hanging out with Jacob's Twitter spaces, and I liked a lot of the content that was being discussed. Then I started coming up and speaking, and that's
[48:57] how Jacob and Theo and other people got to know me. The key there is that I wasn't messaging Theo, I wasn't messaging Jacob and asking them for a bunch of help. I was speaking in
[49:09] Twitter spaces, having conversations with them and other people, and they got to know me that way. Then when I did ask any questions specific to them, they knew who I was, which
[49:21] is huge. They interacted with me, and it was more than just, "Yes, I've seen his name there." They can think of my voice so they remember type of conversations, whatever the case is.
[49:34] More importantly, they have a rough idea of what my abilities and skill are, and they know how I think and how I carry myself in terms of interacting with the community. It
[49:48] makes it much easier to make a choice, like, "Is this guy a dick? No, I don't want to help him." Or, "Is this guy always just asking questions and never providing information?"
[49:56] Or, "Does he ask questions and ignore the answers?" Things like that that would, if I'd done that, Jacob and Theo would have ignored me. They would have just been, "This guy's
[50:06] a dick. Don't care about him." That lets you become part of that community and develop that mentorship/mentee relationship very organically. It just ends up kind of happening.
[50:21] And then when you need help, they're there to refer you to a company. Theo referred me for the job here at Clerk, and he happily did that. I'm pretty positive he would happily
[50:37] do it again without even thinking, because you've proven your kind of value in that community, and that lets someone like Theo or Jacob trust you. They know who you are and what you know,
[50:52] so if they're referring you to a job, they know what you bring to the table. They can speak about what you bring to the table, but more importantly, they have trust that you're
[51:02] not an idiot or an asshole who's going to get the job and end up embarrassing them. If Jacob referred me to a job and I started working there, and three weeks later the company
[51:12] owner is DMing him and being like, "Jacob, who is this guy you sent to me? He doesn't do any work. He insults other people. He made someone cry the other day. He doesn't listen
[51:24] to any feedback. Why did you send this guy to me?" And Jacob's like, "I don't know. He asked for a job, so I helped him." Jacob doesn't want to be in that position. You want
[51:36] to be successful, so you want to create that relationship where you can be successful. Agreed. Yes, Alex/Bumpy Lumps, 100% this is different
[51:46] than what a company might do, where you're going to create, there's going to be an artificial creation of that mentorship. Really quick, I do want to call out the first
[51:57] one, too, because these do go hand-in-hand together. A big part of what the unexpected asked, "What do you think I should do to make money while on the side with coding?"
[52:17] Well, that's very broad in general, but if you're learning to code and you're like, "Well, how am I going to join a community and show my value? Or how am I going to be in the room
[52:32] with people with the jobs that I want to have someday or learn about all these jobs or see what's out there?" You have value just for being you. You don't need to know the tech
[52:44] to get there. A big part of what I'm passionate about is being neurodivergent, talking about mental health, talking about shit you don't want to talk about. That was something I brought
[53:00] to the table and saw how people found value in that, that there was still that value exchange. That was a big reason where I got hired as a dev rel six months after I started my dev
[53:16] rel journey, because I brought a lot of other items to the table outside of tech. That's something I just want to say. You can do other things than just tech to be part of a community
[53:32] and bring value. Then to Alex's question of, I think it matters on the company. I've been lucky enough that at my current job, there is a mentorship program. The person that was
[53:48] like, my boss was like, "Yo, you should probably find someone to mentor." He's like, "Can I mentor Jen?" My boss was like, "Sure, if that works, whatever. You guys do what you want
[53:58] to do." Francesco has been one of the best mentors I've ever had because he helps me with the technical side of things, but also conference side of things, peopling side of
[54:10] things. What is business? Having business relationships, and even if they're not who I would be friends with, per se. There's been a lot of that. I think there is something
[54:30] that could definitely work out. There's ways to do that within a company. There's also, I find organically how we've been talking about up until this point is one of the best
[54:42] ways to find mentorship, even within a company. For most people, what you're going to come across is the enterprise environment. You're
[55:00] going to get jobs. They're not going to be these super savvy, trendy startups or fan companies or whatever. You might end up in just some enterprise company somewhere, might
[55:18] be a no-name. It might not be any name that you recognize. This is the thing. If they have mentorship programs, in my experience so far, it's anecdotal, but I've heard it
[55:34] from other people as well, it's pretty shallow. It's not going to provide you a tremendous amount of value. It sounds like Jen is very lucky in that sense.
[55:48] Overall, it really, really, really, really depends on you and you going out there and doing what it takes to actually network and create those relationships. At the end of
[56:00] the day, nobody's going to do it for you. People can literally walk you up to the water. They can't force you to drink it. You have to do the work.
[56:12] Yep. I can't agree more. Like Jen said, her mentor is someone who knows her, and that's why that works for her at her company. That's the key. Where we're getting here is you build
[56:26] that relationship, you build that community so that people are at least colleagues of interest, if not friends. They care about you, so they want to mentor you to help you
[56:43] because they care about you as a person versus the average, like Jacob was saying, enterprise company where you get a mentor who may not even know you, or you don't normally talk
[56:54] to them. They're sitting there like, "Okay, well, what do I have to mentor this person for an hour a week? Okay, I'll do that," and whatever. If they succeed, cool. If not, whatever.
[57:04] They don't care about you because they don't know you, and they shouldn't care about you because they don't know you yet. You're in a different department. I don't think that
[57:15] that's a bad thing. I think those kind of programs are broken because they're pairing people up who don't know each other, and there's no investment in the mentor helping the mentee
[57:24] because they didn't know you until they sat down. Now, sometimes they'll work out because you'll get to know each other and become friends, and it can be successful, but I don't think
[57:35] there's any guarantee of that, and I don't think you should expect there to be any guarantee of that. This is something you want to be invested in. You want to find someone who's
[57:42] invested in you and cares about your help. That's just how you're both going to be successful because the person who's mentoring you, what they're going to get out of it is someone
[57:58] that they can rely on in some way, whether it's someone they can bring into their company to work or their team to work, whether it's someone they can refer to a friend and bring
[58:06] value to their friends project, whatever the case is. A mentor is looking for value. It's not a one-way mentor gives value to mentee and that's it. It has to be a two-way street.
[58:18] Obviously, the mentor will get less out of it typically because they're helping the other person learn, but if it's just a one-way street, they don't care. It's got to be two ways.
[58:29] And then Jen called this out, but real quick, Jen or Jacob, do you know who the unexpected is who commented in chat? Is this someone you guys know?
[58:42] No. No.
[58:44] So I don't want to pick on the unexpected. If you're still in the chat, understand I'm not trying to be mean to you, but this is what we were talking about earlier with questions.
[58:51] You've come in here and said, "What do you think I should do to make money on the side with coding?" Three of us don't know you. I have no idea what your skillsets are, what
[59:01] your interests are. My only answer to you is something that you're good at. I don't know whether that's writing essays, whether that's painting art, whether that's delivering
[59:12] food, whether that's something else. This is the exact kind of open-ended question that we were talking about earlier. We can't help you because we don't know. And you've given
[59:21] this super, super vague question, super open-ended question that we just can't answer. Well, it's with coding. So Craig's list...
[59:32] There's still one. Yeah.
[59:35] Is that front-end coding, back-end coding? Is that... Oh, Upwork?
[59:41] I mean, yeah. Any of those? Well, the main thing I'm being very facetious about and Roy is being serious about is, again,
[59:55] we have to have context, right? We have to have information, context. You have to provide this stuff when you ask people these types of questions. Context is king. If you don't
[60:04] provide context, you're going to get a vague, ephemeral answer just as much as you asked a vague, ephemeral question.
[60:13] Well, yeah, exactly. Or I'm just going to ignore it. The thing is, if you're specifying, "Hey, I have some front-end skills I've been practicing. I just learned React, whatnot.
[60:32] What's something I could do to earn some cash?" Oh, look around and see if there's some mom and pop shops that need some new simple websites for their stores. Right there, you can make
[60:44] a few hundred bucks just from one website revamp. If it's back-end though, that changes it entirely. A mom and pop shop is probably not going to know what a back-end is, let
[60:57] alone need one. And that brings up a really great way of something I want to call out Jasmine for, and then also
[61:10] get into a big reason I brought all of this up, is Jasmine mentioned to me, she reached out to me on my DMs and was like, "Yo, you do these mental health and neurodiversity
[61:23] Twitter spaces. Can I set a time with you to chat at some point getting into tech?" I was like, "Fuck yeah. Sounds like we have common ground. I don't know much about it.
[61:34] I have a bandwidth, so let's do it." And I found out that she really likes gaming and live streaming. And I was like, "Those are things I'm interested in." And a lot of times
[61:49] without that context though, I wouldn't quite understand what she wanted to go into and also give her ideas of community or things to look into.
[62:02] And also want to say that, so yay, Jasmine. And also want to say that keep showing up and being part of these communities, even if you're not specifically asking for help,
[62:17] just being a part of the conversation really helps when you do have questions. Because I was like, "Hey, y'all, I'm going to write down some questions I may ask you." And two
[62:27] of the questions was, what is authentication? And second one was, I started writing, what is the difference between authentication and security? And Roy and Jacob know me pretty
[62:38] well and I mix up a lot of my terminologies. I comprehend, like I can comprehend a lot of complex problems. It doesn't mean I quite understand the doing process of it and building
[62:53] it myself. And so I mix up a lot of those words. I am very dyslexic. It is something that I get very self-conscious about and try to push through. And knowing, building these
[63:06] relationships, I know that they aren't going to be saying something like that meanly. They're doing it so that way I learn. And Roy was like, "I'm pretty sure you mean authentication
[63:18] and authorization." I was like, "Yes. Yes, that is what I mean. Thank you." But without being around them all the time, without being a part of this community, without showing
[63:28] up to these Twitter spaces, they wouldn't know where I struggle with my communication. A lot of times I've had to ask the group, "Hey, I don't know how to Google this. What
[63:39] am I Googling?" because I just space words. It is the most frustrating thing in the world. And they agree on-
[63:46] Let me add on to that too. When you're learning stuff, you almost always initially don't know what to Google because you don't know what you're learning. That's not a gen thing. That's
[64:00] just a thing. That's something where you have to start Googling and figure out if you're on the right path and then narrow it down. Or if you're on the wrong path, try other
[64:11] terms and searches. Because when you don't know something and you start searching, you need to learn enough to search for what you want. That's a general thing that's not specific
[64:29] to Jen or anyone. It's something we all struggle with. I still feel like I do it more. Because y'all, I don't even know how to Google things outside
[64:42] of tech and I struggle with Googling. I have to walk up to my partner and be like, "Hey, I'm trying to look for... You know those yellow... You know that thing that we saw at the garage
[64:57] sale that's a little boxy thing and it was yellow? How do I Google this?" That's exactly what I'm talking about. What is the yellow box thing? Did you know what
[65:06] it was called? At one point I did. Yeah. If you don't remember it or you didn't know, how do you Google that? There's that
[65:14] thing that I like, but I don't even know what the term is. You've got to figure out the term so then you can Google it. That's a prime example of what I'm talking about. You can't
[65:29] Google the yellow box thing until you know what the yellow box thing is, or you're going to start Googling things that are a yellow box. In a situation like that, I'll go to
[65:41] Google images and just yellow box and try to figure out if I'm on the right track and then narrow that search down. Big yellow box or little yellow box or metal yellow box or
[65:51] whatever and try to get to what I'm looking for and then be like, "Oh, it's a... I don't know. Whatever. A mailbox." That's a dumb example, but okay. Now I can go and do Google
[66:02] yellow mailboxes and be Googling the right thing. It's a legitimate thing that we go through.
[66:09] Yes. Thank you. Mark, if you find that blog, will you paste the link for that? Because that sounds interesting. It also brought up the one more piece that I did want to call
[66:24] out that you guys taught me a lot about was challenge yourself, yet embrace the way you learn. I really struggle with docs, yet I've learned through all of this and also with...
[66:43] There is another human named Laura Langdon that joined Tshantek for a while of learning... I know that I'm super dyslexic, so at least going through and using text-to-speech to
[67:02] try to read docs is a way that I've gotten over trying to read docs. I still struggle, but that's at least giving myself more resources and learning how to learn. I feel like that
[67:17] can be a very big struggle in all of this. Yeah. I have pretty bad ADHD. H-A-D-H-D. Oh, I didn't say it properly today. There we go.
[67:33] Working on the docs, I can't read them. They're just not written in a way that I can sit there and read through them in a comprehensive way. That doesn't mean the docs are bad. It means
[67:46] they're bad for me. A prime example is the React Writer docs. I just cannot consume those docs for whatever reason, unless I very specifically land on the piece that I need, the paragraph
[67:59] or two that I need. But trying to go through those docs drives me nuts, personally. They don't click with me. And again, I'm not saying they're bad. Don't go and be like, "Oh, Roy,
[68:11] the React Writer docs are terrible." They are bad for me. And I'm sure they're great for a lot of people.
[68:19] So you want to understand quickly what kind of docs work for you, or whatever it is, whatever you're learning, look at the docs. And if they don't help you, look for other stuff.
[68:35] I learn a lot with examples. Give me examples of the code, and I'm going to comprehend a lot quicker. Give me just a function and tell me what to do with the function, and it's
[68:46] a much bigger struggle for me. So that I know. And learn that and lean into that. Don't be like, "Well, other people read the docs. I need to read the docs more." If that doesn't
[68:58] work for you, that doesn't work for you. Do what works for you. If it means reading the docs with text-to-speech, do that. If it means don't use the docs, go get examples, blog
[69:09] posts, videos, whatever that is, do that for you. Figure out your solution and embrace that.
[69:17] Thoughts? No? That is something that Clerk does, I think, pretty well, is doing the docs because they
[69:34] also have it where they even do -- do share screen. Go to that window. There we go. In the docs itself, under Quick Start and Tutorials, they're learned by example, which is really
[69:56] helpful. Or just like Quick Starts, there's different ways that it can be done, which is pretty cool. And that does lead me to -- oh, yeah. The JavaScript way out, I agree. It's
[70:14] helpful. I will say I don't think he's here anymore. As from reading from a book, Josh Goldberg's book Learning TypeScript is actually pretty funny. It's a great learning book.
[70:31] I was entertained while I read it. Plus, he's fun to talk to about everything. But before we keep going, I'm going to totally pivot and ask the original questions that
[70:45] we were going to do today's stream for. And then we decided to do, you know, just let's hang out. Which I'm also grateful for. Because sometimes that just needs to be done. Is what
[70:58] is authentication? >> Authentication is just -- like, at the base level, it's just logging in and having
[71:09] a user account. So, it's just the ability to create a user for yourself on a website and then log in and out of that user.
[71:20] >> What's the difference -- Jacob, I'm going to ask you this one now, because Roy answered the first one. What's the difference between authentication and authorization?
[71:31] >> So, you think about, like, authentication as, like, having the key and being able to walk through the door. And then authorization is actually being allowed to be on the other
[71:41] side of the door. So, like, if I -- if I, say, have access to -- what would be a good example here? That was a metaphor. So, let's think of an example that we have. So, like,
[72:06] let's say I authenticate and I sign in to your website. Right? And you have a route that's, like, a member's route. You're now authorized to enter that member's route. But
[72:20] you may try to go to the admin route. And you will be, like, hit with a not authorized. Right? It will just be, like, hey, you're not allowed in here. But it's, like, hey,
[72:31] but I authenticated. Yeah, but you're not an admin. Right? So, you're not authorized as an admin. You're authorized as a member. Right? So, that's kind of a fundamental difference.
[72:48] >> Could it be, like, if I'm watching all of, like, the spy movies and stuff and they have hackers, that they skip the authentication to, say, a specific user and hack their way
[73:08] in to give them authorization to see it all? >> Kind of. They're, like, they're finding an unlocked door would be the best way to put it. Either finding an unlocked door or
[73:23] cloning your key. One or the other. Also, there's a lot of make believe magic in the shows. But we won't talk about that. The way that, so, like, Jacob talked about a key.
[73:36] My explanation for authorization is very similar. But it's basically authentication lets you open the front door. Authorization is keys for different rooms. Some people only get
[73:49] one key for, like, the basic room where you can just, like, sit on the couch and watch TV and other people get the key to the room where you can change the channels on the TV
[73:56] and change the programming. Or other rooms where you can turn the lights off and turn the heat up and down. So, depending on the keys you have, you have different levels of
[74:05] access. And your user management system is going to say, hey, that user signed in. Cool. Here are the keys that they have or here's essentially what we call roles or permissions
[74:18] depending on how you structure your system. And so, that user has these different permissions whereas that user only has this one permission or this one level of access. So, similar concepts.
[74:31] Just framing it that way in case that makes more sense to people. Either one works as long as it makes sense to you. >> Exactly.
[74:39] >> So, if we go off of what Jasmine said of, like, so, authentication gets you into the building and authorization gets you to which floor you can get to of the security clearance.
[74:53] >> Yep. >> Okay. We're talking like the FBI. There we go. >> Yeah.
[74:58] >> That's how I'm going to conceptualize it now. >> Exactly. I mean, that's a perfect example. Like, anyone in the U.S. could walk in the
[75:02] front door of the FBI to their lobby, right? Of, like, an average FBI office. You can walk into the lobby. But most people don't have any of the clearance levels or the keys or
[75:12] the access to go through the FBI-only door into the, you know, the back offices. And even within the FBI, some of the agents might have more access to go to certain files or
[75:22] certain rooms and stuff like that. >> Yeah. To expand a little bit on because I like that different floors metaphor. Think of it this way. When you first join a job,
[75:36] right? First join a company and say that they have access control, okay? So that's like when I worked at Cloudflare, they had access control. Your authentication is them essentially
[75:49] hiring you. You're given a key card as this individual. This is your authentication. This is you. It has your information on it. That is the thing that you will be using to authenticate.
[76:05] And then the authorization is essentially, like, what that key card as you will be allowed to go to different places. And somebody can come up to you and say, hey, show me your
[76:18] badge, right? And they can compare it to, like, your key card and your, like, who you are, what you look like. And that's them reauthenticating you. They're like, hey, this is you, okay?
[76:33] You're on the wrong floor, mother****. You're not authorized to be here. >> To be really clear there, to actually be super pedantic, this is you. That's reauthenticating.
[76:47] That's who you are. And the you're on the wrong floor is checking the authorization and seeing that you don't have access. Sorry to jump in there, Jacob. You are both in play
[76:59] there in that little space. >> Exactly. Can people also get into, like, so, like, we're talking in physical examples. This is because we're trying to have analogies
[77:13] here, right? Can people get into those same situations in, say, like, in real-world web apps and stuff? Absolutely. Can you be authenticated and be in an unauthorized area? Yes, that
[77:27] can happen. Unless you use Clerk. >> Bugs exist. In fairness, even with Clerk, because you're still implementing things and you can implement them incorrectly or whatnot.
[77:39] So, like, there is some of that. >> Yeah, yeah. >> What? >> Clerk makes it a lot harder to make the
[77:47] mistake. >> There you go, Roy. There we go. >> Does it have anything to do -- >> It's not magic, unfortunately.
[77:57] >> I mean, it's pretty magic. >> It's pretty close, but it's not quite there. >> Jen saw where you are. >> It is pretty cool. Like, it's interesting.
[78:10] We were talking about Theo earlier, and Theo has a T3 app chirp thing that he was, like, if I -- if you finish this and do the entire thing, I will answer any question you want.
[78:25] >> Yep. >> I'm still not done. I'm still learning. There's been a lot of learning in the process. But it did get me to find out more about Clerk
[78:35] and then also seeing it being used when -- for our Expanse stuff. By the way, I end up saying that what we're doing is D&D to people, because they can conceptualize D&D, but they can't
[78:51] conceptualize the Expanse. So I still call our gaming stuff D&D. >> That's super common, yeah. Like, people usually refer to things as D&D or TTRPG, especially
[79:04] when you're using other systems. Because, like, saying, oh, yeah, I play modern age, a lot of people don't know that's the system that's in place for the Expanse. So, like,
[79:14] oh, I play modern age. People are like, what? What is that? >> Or Illuminated World System. Like, do you know what that is? That's created by the Critical
[79:25] World Team for Candela Obscura campaign. Or if I say Pathfinder, which is a spin-off of D&D 3.5 rule set game system, right? If I just say D&D or TTRPG, people understand
[79:42] it just fine. >> It's very similar to how at least in North America, most people say Kleenex instead of, like, tissue.
[79:50] >> Yeah. >> That's true. >> Because there's also, like, bathroom tissue. >> It's like a brand name, yeah. I like that.
[79:55] >> Paper towel tissue. Kleenex is a tissue. Not everyone's using an actual Kleenex. But everyone knows what a Kleenex is. And very specific to the one that you're going to blow
[80:05] your nose in versus, like, wipe your butt. >> Thanks. >> It is what it is. >> Yes. Yes. And so, doing the T3 app, Chirp,
[80:19] and then all the D&D stuff is what helped me understand a bit more about the authentication. And what I'm a bit curious about, because -- and this might be a -- Roy, this might
[80:34] be a you question -- is, with GoDaddy or, like, WordPress, those type of platforms, there were users that could be created. But then there was also, like, file read/write
[80:50] roles. So, are file read/write roles associated with users, therefore associated with authentication? Their authorization. They are the access that you have as a user. Some users may have authorization
[81:07] access to read and write files. And other users may have authorization to not just read and write files, but also read and write/delete other users' files. For example, an admin
[81:18] could go in and view everyone's files and potentially delete unwanted files. Whereas a user would only be authorized to see their own files and modify their own files and not
[81:28] other user files. >> Got it. Hmm. Hmm. There's a lot to think about here. And I appreciate the breakdown. There -- and y'all, I don't know when, but
[81:48] at some point, these two are gonna be back. Because we have lots to learn from them. And I'm working on scrolling back to all of the ideas we had. And I'm curious what y'all would
[82:02] be interested in of -- we could talk about just, like, installing it. What does it look like to install it? How orgs and setup, the backend to SDKs and webhooks and custom flows
[82:17] and users? >> I think the next stream, we should just talk about installing it and talk about what makes Quark more unique than other solutions
[82:26] in the space. And to kind of preview that really briefly, to install and set up Quark on your application for just authentication, just to get started, you don't need a backend.
[82:38] You could have a React app that runs solely as a straight single-page app. Like, straight on a -- only in a user's browser. No Node Express, no backend of any sort. No, like,
[82:51] next API routes. Nothing. Just that frontend React application. And Quark will load and work in the frontend. We actually have -- so, actually, let me just deviate for a second
[83:05] to answer Jasmine's question. Quark is a software as a service product that offers authentication and user management. You can add it to your -- to your web application. And we, Quark,
[83:19] the company, basically manage all of that hard stuff for you. You just need to implement. Like, you just need to, you know, make the sign-in component available. Make the sign-out
[83:29] button work. The user profile. But we basically -- we handle all of the work. We have the infrastructure for, like, saving all that user information. Handling all the requests.
[83:40] All of that stuff. Anyway. So, just to kind of go back to what I was talking about. You drop in Quark. It's a JS package in your React application. And it connects with our frontend
[83:53] API. So, Quark actually has three APIs. Two of which you would interact with as a customer. We have a frontend API, a backend API. We also have a dashboard API, which is what our
[84:03] dashboard interacts with. So, you, as a customer, you would never need to worry about that. But our frontend API is what is used for all the sign-ins, sign-ups, you know, changing
[84:14] your user profile, adding your avatar, selecting which organization you're currently active in, all that stuff. And that all happens on the frontend. No server needed. You just drop
[84:27] that stuff in. And within minutes, literally just a couple minutes, you have authentication working on your site. And then later, you may implement some of the backend stuff for
[84:37] more advanced features as you need them. And the key there is because you're just dropping in JavaScript, there's nothing to set up. There's no database to set up. There's no
[84:47] server to set up. You don't have to worry about managing sessions or cookies. You don't have to worry about any of that stuff. And you don't have to worry about how fast your
[84:54] services are. If you have your own database to manage sessions, you're handling requests through your server, performance, speed, cost, these are all factors that are removed from
[85:04] the picture that Cork handles for you. Obviously, it is software as a service. We have a free plan. We have paid plans. Spoiler alert. We're actually switching to a much better plan structure
[85:16] in Q1. Way more free users. It's going to be awesome for our customers. Super excited about that switch in Q1. But yeah, we take a lot of stuff off your plate. And you can
[85:29] then have authentication within minutes. You can even have authorization through our organizations within just a few minutes with no back end. And we can do that. We can set up Cork with
[85:42] a next app on the next stream. Just take a next app and add to it. Talk about doing it and walk through the different steps. >> Yep. Yep. That would be a good one. The
[85:55] other thing, too, that was mentioned is user management. Right? So, what you'll notice is Roy had said, like, you don't even need the database. Like, if you are just setting
[86:12] a bare, bare, bare minimum React app that's just that you have no back end, no database, you're like, well, where are the users going, then? Cork manages those, too. And you have
[86:25] in your dashboard, you have a lot of control over that as well as there's a very nice graphical interface that allows you to interact with your users. So, besides even just like the
[86:43] initial setup, the experience that you get continuing forward is also, like, really streamlined and really just very nice to deal with. And that's, again, if you don't want to have to,
[86:59] like, deal with putting your users in a database and all this other stuff. You have it all in one. All in one go. >> And to extend just a tiny bit on there,
[87:13] not only do we handle all that user information, we provide a unique user ID for each of your users that you can then use in your database. So, you don't need a user table anymore. You
[87:27] can get rid of the user table, depending on the needs for your application. And then in all of your other tables, your orders tables or your posts or whatever that is, you just
[87:36] use that user ID from Cork as a relation. So, you can just take that user ID and query your database and get your posts. No user table in place. We have options to sync that
[87:46] if you need it. Because realistically, people need it for various reasons. But if you don't need it, you don't even have to have a users table. You just have that unique ID. People
[87:55] ask, what is it? It's not a CCUID or a UID, even though it looks like it. It's a KUID, which is a Go thing. But very similar to the others. It's a static 24 character string
[88:07] preceded with a user ID prefix that is unique and consistent. That was a little geeky right at the end there.
[88:16] Yeah, it was. But there's a few people who want to know that, because there's always questions like,
[88:24] what is that? Is it reliable? Is it unique? What's the structure so I can put a type on it? That kind of stuff.
[88:30] That is the cool thing with the crowd that shows up for the stream. And also, I would say what shows up for the live stream and who watches the videos is a very broad audience.
[88:46] There's the very technical people, like y'all that are like, you know what each other's talking about. I don't know what you're talking about, but you two know what you're talking
[88:55] about. And then there's super noobs. And I like that we can vary between all of it. And also, at some point with Alien showing up, I'm like, so could I do Astro with Clerk
[89:12] and then Strappy and Vercel and Railway? And I'm just going to name a bunch of tools and see if it actually works.
[89:21] Almost. But we don't have Clerk working with Astro's middleware currently. Yet.
[89:26] Yet. Currently/yet, but it's definitely something that's on our radar.
[89:34] Yeah. As for getting Clerk to work with other integrations, especially SaaS integrations like Strappy or Stripe or whatever, there's a lot of, let's just say tooling and whatnot
[89:50] for enabling that. So, Clerk has webhooks, metadata, and just a fairly low level API as well that you can interact with. All these things would allow you to build out more and
[90:15] more complex and custom integrations and more of a system as well. And if you ever need people to break shit, give me something that says, "Jen, this is
[90:31] how it's set up. You're going to try to break it doing something else with it that it wasn't meant to do." And then I'll find that out. And I'm glad that I asked beforehand of, will
[90:42] it work with Astro? Because knowing Malik, I would try doing that someday. But instead, I just don't have an up-to-date website, which is improvement.
[90:52] Yes. Jen is a professional at breaking stuff, like a certified professional. I'm very good at it because I want it to try to do stuff that I think it can do and it
[91:02] doesn't always do it. But when I do learn the tech, it is a bit dangerous because I do things on theory. And doing that when you're working at a production studio with conferences
[91:16] with a few thousand, if not 10,000 people and doing something on theory, probably not your best idea, but I did it. It worked out 99% of the time. But yes, I love to find bugs
[91:34] and break things. It's fun. And yes. So we will announce at some point what we're doing when we're doing another ClerkStream. Is it on December 5th, the next one?
[91:51] Jacob, I'm saying that to you. Is that the agreed date? Yeah, I don't know. There's a lot of stuff going on right now.
[92:02] It might be Roy, it might be Jacob, it might be Roy and Jacob, but it's probably going to be December 5th. We'll go with that.
[92:10] And I thought we'll announce it with more warning. Yes. And next week we have someone coming on that is part of our OSRG group and going
[92:27] to teach me a bit about cloud. Kat is someone who is not Katnipp. Katnipp is Jasmine. Kat, who isn't here, is going to be coming on next week and talking about she is a recent Bootcamp
[92:44] graduate who's been really into cloud. And I'm going to AWS reinvent the week after Thanksgiving in the US. So next week, Kat is going to come on to talk to me and give me the low down
[92:58] about cloud, which I'm very excited about because I need to know these things. And eventually, AWS. Which cloud, cloud compute, cloud storage,
[93:14] cloud networking, cloud CDN, cloud email? We'll get there. Cloud DNS. We'll get there. It may not be on next week's
[93:24] streams, but we'll get there. Because I'm in the works of getting all the cloud-ish, more cloudy people on the stream, like Google and Digital Ocean and Azure, Microsoft
[93:47] Azure and asking Jacob for some intros for some CloudFlare. All the clouds. There's a lot of clouds, y'all. There is a lot of clouds. Yeah. If you see what I just typed into the
[94:04] Twitch chat, clerk is cloud user management. There you go. There you go. So y'all, it'll be fun. Join us next week. Hit us up when you --
[94:18] No, I don't. No, I don't. This is why I adore the two of you, because it's never a dull moment. Ever. Ever. And for everyone, we've talked about our community quite a bit. And
[94:33] I just dropped the link again. If you go to this website in the upper left, left, that's the left, is where you can click Discord. And, yes. Everybody, come join us. Come hang
[94:48] out. Ask us questions. And hit us up if you have any ideas on something that you want to have on the show. And Ilyan, just because I also see you still here, we need to have
[95:02] more Astro stuff on, too. One of these days, I'm gonna come up with a tech stack that will work of, like, Astro to, I don't know, and have everybody on at the same time to build
[95:17] an app together. That would be so entertaining. You guys don't look as entertained as I am. But I think it would be so fun. >> I'm just gonna make it so people can buy
[95:31] his merch. >> I'm never entertained. >> Oh, yeah. I forgot I have stickers. >> Yeah. You guys have stickers for all your
[95:45] characters. You can definitely -- >> Yeah, we need to look at this really quick. I -- Roy, did we talk about doing a -- >> Yeah, you signed up and were supposed to
[95:54] tell me when you got the fourth wall invite, which I'm sure you've gotten a while ago. >> Yep. That doesn't surprise me. >> Yep. Very ADHD to just completely forget
[96:09] about that. >> Yeah. But, hey, we have all of our characters. And it's very exciting. >> Yep. They're awesome. Those portraits are
[96:20] amazing. >> And I want to get these stickers and then put it on my mug. It would be really cool. >> I mean, if you want a mug with Luna or
[96:32] one of the characters on it, I can add that to the store. >> I kind of somehow -- like, this doesn't even, like, logically make sense. And it wouldn't
[96:46] look very good. But to get, like, an OSRG hoodie with the, like, Luna on there, too, and, like, the D&D ones here. That would just be a really happy --
[96:59] >> I mean, we can talk. It's probably pretty quick for me to throw that together and add it. It's all the shit. >> Weird, though. Just all the shit all together
[97:08] on one hoodie. It would be great. >> There's also front and back. It'll make it cost a little bit more. But you could do, like, OSRG on the front and, like, something
[97:16] else on the back, too. >> There's options, y'all. There is options. >> Jen's going to have custom-made merch. >> I -- there are -- yeah. There's all the
[97:31] things. >> And now Alex is going to decorate his laptop with the campaign group. >> Figurines.
[97:36] >> He'd have to create a figurine one, too. >> Oh, Alex, you need to -- yes! Actually, I will look for a thrift -- at the thrift shops, I go thrifting a lot. A lot, Mark.
[97:53] I will get you -- I will see if I can find, like, you know, a leather jacket we could, like, destroy. >> Put a hole in it.
[98:01] >> And then if we get a patch, we could iron it on there. >> Yeah, I can turn these into patches. >> Oh, my God. That would actually be --
[98:11] >> Terrifying and hilarious at the same time. >> Yes. Yes. Okay. Here are our options for raiding. Jason, linksdorf, which we raid to quite a bit. Learn with Jason. Or the other
[98:28] one I got is Primogen. Primogen. How do you say his name? >> Primogen. >> Primogen. Primogen. Who should we raid
[98:38] to, y'all? >> Jason, I would say. That's my vote. >> Okay. >> Yeah.
[98:46] >> That works for me. Thank you. And see all of you next week. And thank you for joining today. Have a wonderful week. Bye, y'all. >> Bye.
[98:58] >> Take care, everyone. >> Peace. 
