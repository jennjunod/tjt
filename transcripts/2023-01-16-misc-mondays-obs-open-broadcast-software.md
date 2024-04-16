---
showLink: "https://www.youtube.com/watch?v=E_D5Q2NiD3s"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "misc-mondays-obs-open-broadcast-software"
title: "Misc. Mondays: OBS (Open Broadcast Software)"
publishDate: "2023-01-16"
coverImage: "https://i.ytimg.com/vi/E_D5Q2NiD3s/maxresdefault.jpg"
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

[00:00] Hello, hello, beautiful humans! Welcome to another episode of Misk Monday, where Laura and I go through a bunch of random shit and miscellaneous things. There's the proper way
[00:15] of saying things. I'm Jen, that's Laura, and we have a special guest, Ramon! And hello, everyone!
[00:24] On my end, you're pointing in different directions, but I'm sure it's fine. It's true. Mine, too.
[00:27] Oh, really? Probably. You know what? We have our names on ourselves, so, yeah.
[00:32] That's me, yeah. I'm going to hold it here, and look at... Oh, they're backwards from the screen itself.
[00:38] I think your camera might, like... Because, like, from some places, the camera gets flipped, which is a point about streaming, right?
[00:44] Huh. You're right. Okay, well, swap them. How about this? One of these are Laura, one of these are Ramon. They're just above me. There we go.
[00:56] I wish I was as cool as Laura. Oh, come on now. I mean, we're all pretty cool. This is why we're doing this stream.
[01:06] Laura is phenomenal, because she does Misc Monday with me and has taught me a lot. Somebody was asking me about that, of, like, what are some things I've learned from streaming, and
[01:17] I was like, dude, I don't even know where to start with my list of what I've learned with streaming. It's been a lot.
[01:25] Mm-hmm. But one thing that we've been struggling with, which for those whose it's been a minute since
[01:33] you've joined us is OBS has been on the plan. It's been on the docket for a very, very, very long time.
[01:41] Mm-hmm. And...
[01:43] I'd love to hear... Oh, sorry. Go ahead. Go ahead.
[01:46] Jen, this is your show. I don't want to, like, push things in random directions, but I'm curious, why are you keen to try out OBS?
[01:58] Because streaming is fucking expensive. Oh.
[02:02] That's fair. For me, it's because I want to be able to do, like, transitions and, like, all the cool
[02:10] things. I want to do all the cool things. And I was going... I was using... I tried... What was it? Twitch has its own one. Is it called Twitch Studio?
[02:22] Oh, yeah. Something like that. I tried that. And, like, I don't remember what I didn't like about
[02:26] it. And so then I switched to Streamlabs. And I thought that was going to be, like, OBS with training wheels, which is what I need. But I couldn't... I couldn't get it
[02:37] to work either. And I was, like, if I'm going to invest this much, like, energy into learning the system, it might as well just be OBS. So, yeah. Here we are. And I have also learned
[02:49] so much from Ramon. Ramon walked me through my very first PR for any repo that was not my own, I think. Almost. Yeah. Almost my very first. And my very first that, like, was going
[03:05] to affect things that were, like, publicly visible and so on. I dig it. I dig it.
[03:12] Laura, I'm so sorry. It's been a while. What repo was that? The Docs repo. Like, in my first week at Suborbital.
[03:21] That's right. Oh! For those who don't know, Ramon and I are home workers. That's my... My 5-year-old
[03:29] refers to my coworkers as my home workers because he's heard of homework. And I work at home, and everybody's at home. And so, he just says home workers, and I don't correct
[03:38] him because it's so cute and so apt. And so, now I have adopted home workers. So, Ramon is one of my home workers. Today's actually a holiday in the US, but Ramon is in Vienna,
[03:48] and it's not a holiday there. And so, today, I'm not working, but I still get to see Ramon. So that's it.
[03:55] Yay! And you actually brought up something that I want to talk about. And welcome, Jay, and thank you for happy MLK Day as well. And this is something that, well, y'all, the three
[04:10] of us have talked about on and off again in random spaces about how fucked up racism is and how a lot of tools are still very colorblind. Colorblind? Is that the right way of saying
[04:26] it? I don't even think colorblind, right? It's just fucking racist, right? Because colorblind
[04:32] would be like, we don't see color, which is totally not a thing at all. Oh, I meant like, they don't read color?
[04:39] They do though, because they read some colors, they just don't read them all. So, we're just going to go with racist.
[04:45] Yeah, I'm down with that. And something that I really, really wanted to... I've been noodling on quite a bit is the fact that, you know, you have a ton of white folk who will post
[05:01] very, very well-known photos that are normally in black and white and that make it look like a bunch of white folk. We're really active in helping Martin Luther King. And that wasn't
[05:18] the case at all. There were some, which is dope, but not many. And I just wanted to take time to say, like, I don't even know how to really say something. I'm trying to think
[05:33] of words of how I appreciate that there are many people in this world that are working on being a part of the change and making it more well-known of how fucked up the past
[05:48] is and actively talking about these really difficult topics because... Oh, sorry, I got interrupted. Oh, I hate... Oh, you're so right. I hate that.
[06:06] Yeah, absolutely. You're so articulate. So well-spoken. Let's break down what Jay just put in the comments. A form of racism and ableism, it
[06:19] can be many, many different ways of saying. So the way that Jay mentioned is he's very articulated for a black man, is what a lot of... It's something that people, I will say
[06:33] people because, yes, racism is very, very taught, but it's something that is enablism as well, ableism as well. You're reading really well for being dyslexic. That is also like
[06:51] a form of ableism. And what people don't realize is you can be very articulated just for being articulated because you're a dope human and you are great at it. And that's something
[07:04] that I have learned. To Jay's point, it has been very, very interesting helping past generations re-learn vocabulary of... Instead of saying they're very articulated for Ed because of
[07:26] their... For being Indian. That's where I got a lot of mine was I grew up in the Southwest in the US and I feel like it's something that's slowly being changed yet. I mean, it's like
[07:41] we have this smidge of movement and it's great and I do want to celebrate it, but it's not enough. And there's still a bunch of really dope shit in the world.
[07:53] The work is not over and you mentioned racism being taught in schools. What I have learned by people who have been kind enough to help me, guide me through the work is that what
[08:08] we're lacking is deliberate action in anti-racism. And this is where a lot of the work remains to be done by those of us who can do our part in the work.
[08:21] Yeah, I was really excited. This is going to be a theme, I guess, in all of the Miscellaneous Mondays or many of them anyway, how much I like my kid's school. Because a lot of schools,
[08:34] if they talk about Martin Luther King at all, it's this perception is created that everybody loved Martin Luther King. When in fact, Martin Luther King was on the terrorist list, right?
[08:46] Like the FBI watch list. And people were scared shitless of, I mean, white people were scared shitless of Martin Luther King. And it wasn't until after he was like safely dead that white
[09:01] people could be like, oh, you know, Martin Luther King, great dude. Right. And it's a much more modern, it's a very modern lens to look on the situation. And my kid's school
[09:21] did not, they didn't go for like the, I have a dream speech, which is the default it seems in the States where everybody's like, yeah, that. And then I saw a post something about
[09:33] Martin Luther King said more than 35 words, but you wouldn't know that from what conservatives are going to say on Martin Luther King day. And that's going to be the quote about like,
[09:41] I want my children to be judged not by the color of their skin, but by the content of their character and so on. And this is supposed to be like promoting the idea of color blindness
[09:51] as like a virtue when it's not even a thing. Right. And my kid's school did not, did not go for that. And they didn't sugarcoat it, even though he's in a class of three to five
[10:02] year olds and he came home. It's also clear that like some, some parts are a little bit fuzzy because these are very small children. Cause he came home and he said to us, did
[10:13] you hear that Dr. King was shot? Like it happened yesterday. And we were like, yeah, we did hear about that. And do you want to talk about that? And he, he had a lot to say about it
[10:28] and yeah, Jay again. Yeah. One of the magical things about, about some of these folks is that they can be assassinated more than once. Yeah. So I, I really appreciated that about,
[10:42] about his school that they don't, they don't sugarcoat it even for the little ones. And I just thank you both for having this conversation to start off our stream, especially
[10:56] because I didn't tell you about it. That is the joy. I'm going to, I've given the weird look because I, I feel like this, when I talk about the podcast too, when I'm like, thank
[11:06] you for joining shit you don't want to talk about, please introduce yourself in the shit you want to talk about. And then I'm like, I'm really excited about this topic. No, I'm
[11:15] not. Yes I am. I don't know. Ooh, okay. Jay just said they should also mention before someone reads this out of context, that he's a black male that grew up in the South, US
[11:31] Southeast is still very racist. Yes, yes, yes, yes and yes. I, I can only say that one of my favorite humans in the world who is a big brother to me, taught me so much just
[11:51] being my friend and a big brother and society taught me more because people would be scared of him and would talk to me and ignore his existence or cower around him. And I appreciate
[12:12] you joining the conversation and just being as cool as a human. You're like so dope and you bring up so many really, really important topics while we've been streaming. Um, my,
[12:25] Oh, really? This, this was a game. Call of Duty was as a game that I, uh, my, so I have a kid who will be 18 in fact, in like four weeks, three weeks, four weeks, five weeks,
[12:44] and happy early birthday. Thank you. And something that we, the, a video game that we had have argued about is like, why is he allowed to play? He was allowed to play left for dead
[12:57] when he was fairly young. Right. And that's like shooting humanoid figures with guns. And I said, absolutely not to call of duty. And he was like, really like, okay, but what,
[13:11] what on earth is the difference, you know, between these, besides like the fantasy elements or whatever. And I said, it was specifically because call of duty was fucking racist. Um,
[13:20] because who are you shooting in call of duty? You know, like what there's, there's no, there's no, um, pretense about what we're up to here. Um, not that pretense would be better, I guess,
[13:35] but it's just so, yeah, it's so not good. Um, and, and yeah, exactly. And welcome again to misc Mondays and how we will talk about difficult topics and about
[13:49] privilege. I'd love to ask if I may, for those of us that are, that are watching, listening and learning, um, in the chat as well, please, if there are any race resources or further
[14:03] reading we can do to, um, improve, to improve our understanding, to improve our, I find, I find that for myself, for example, cause you know, y'all, y'all were talking about
[14:14] a very us centric systemic racism. And I think it needs to be acknowledged given that I'm, I'm coming to you live from Europe and a big part of the hubris I see here, a lot of part
[14:26] of a big part of the lack of listening I see here is that some folks will claim that it does not exist here when it very much does. Um, and how it takes different shapes and
[14:39] forms and is perhaps in some ways more insidious. What kind of recommended reading or, or, or resources or people to follow or talk to? For example, I always, um, I always recommend
[14:51] the works of Kim Creighton. Uh, that's Kim underscore Creighton one on Twitter. Um, her teachings have been life-changing for me. And one thing I've learned through that is
[15:07] that, you know, this is work that for a long time she's provided for free and yeah. And she's got that book. When is her book out? It's like next week. Is it? Yeah. Something
[15:19] like that. Could one of you link that one? Yeah. Um, I'm looking for it. Uh, white fragility and one thing that I, um, find very interesting is, and for a lot of people, I don't think
[15:37] that they realize how unfortunately powerful white woman tears are and it's really fucked up. And, um, we can go through that, read this book, let's have a conversation about
[15:55] it. Uh, and Jay said, uh, that they love hearing about racism in European places. Uh, they went to a U S civil rights exhibit in Dublin and it was absolutely amazing.
[16:10] If I may, I'm also going to throw out, um, a book that I read last year that I very much recommend. Um, it's called, uh, so you want to talk about race by, uh, Joe Moe Luo. Um,
[16:22] really, really good. Um, she also wrote a full, it's not a directly related followup, but she also wrote a book called, I'm going to need to get to the title because I don't
[16:31] want to get it all wrong. What was it called? Sorry, carry on. Oh, mediocre, the dangerous leg, legacy of white male America. Also fantastic. Sorry for the repeat. I'm going and trying
[16:45] to get Laura's link so I can link it everywhere. Uh, didn't know the volume was on. And yeah, let's get, uh, let's get Kim's book as well. I did. Yeah. That's what Jen is. She posted
[16:59] it after her Twitch and I was going to post it to everybody's. Um, cause yeah, we're cool and we're just streaming to all three of our twitches cause why not? Um, you know, it's
[17:09] a fun thing to do. Okay. So I know that we could talk about this topic for forever and it is a topic that needs to be talked about for forever, but I also know that we have
[17:22] a time limit and I appreciate all of us. What's your, I'm sorry, can I add one tiny thing? Yeah, no, just very tiny Jen. I promise. I think, I think it's important for us, especially
[17:36] us, uh, white folks to not only talk but also listen. And I think that needs to be, okay, I'm just going to keep going for a second cause you know, um, that is one of the biggest
[17:49] benefits that I've received from Twitter. The listening opportunities are so huge. I have learned so much from listening to people, um, especially about racism on Twitter.
[18:04] Um, sorry, I'm putting my computer on do not disturb. So it stops beeping. I have learned a lot about it from Twitter as well as Tik TOK. I've learned so much about Tik TOK and
[18:24] I think we had somebody say hi earlier too, and I skipped it. Uh, Taka Nome, what up? And Pipo.
[18:31] People, Dev. Hey, yeah, see you. So hello to both of you. Sorry. We, we were very deep into conversation, um, that we,
[18:44] uh, we're kind of missing. Um, and I agree that listening and is one of the biggest parts that we can do. And one of the, another big thing that I think we can do is having these
[19:03] conversations with our friends and family without others in the room, because we're not doing this to impress others or be woke or, you know, we're doing this to make the
[19:15] change and that's, it's important to have these conversations no matter what. And also bringing up people that may not always be brought up, um, to have the same opportunities
[19:35] and especially those of color that are skipped over by their resumes. Like this still happens where if somebody has a unique name that they're skipped over. Um, so this is a very, very
[19:49] layered thing and very systemic. So it's definitely not something that I, we can even, I don't even, we could do a whole conference on this.
[19:57] I mean, there is, um, in fact, uh, if you're in the United States and you're interested, the CFP for Juneteenth conf closes today.
[20:08] Ooh, yeah, please. So there are a bunch of resources. Anything else that you two want to say other than linking
[20:21] for CFP and that all day, anything we move on? No, you have today to do your CFP, do it today.
[20:37] Yeah, it closes later today. I think it's like quarter to midnight Eastern, something like that. All right. I'm all over the place.
[20:57] I'm looking at 2020 registration. Maybe it's there. I'm not seeing the CFP for it. Why? I saw somewhere and I was talking to a friend and they said that it closed today,
[21:09] but I don't have a link now. Huh? Did it close already? Or am I scrolling too fast? I mean, it could be all of the above.
[21:24] We'll find it. We'll, we'll get a link. Dude, yes. Submit. Submit. And for those who are looking at doing CFPs and want to
[21:41] practice any talks, Ramon and Rizal have a really, really dope streams that they'll be doing about that.
[21:48] In fact, they're here today. Found it. Found the CFP. Found the CFP. Ah, thank you, Jay. You found it before me. Nice.
[21:57] And I will get that link to all the other ones. Give me just a second. And I do want to give both of you a shout out for your talk set. You got this conf.
[22:09] Jen was, was amazing. I am assuming that Ramon was amazing. It was at like 2am my time. And so I haven't seen it yet, but I know Ramon and our other homeworker, Taryn, well enough
[22:21] to know that it was definitely amazing. And I'm really looking forward to the, to the recording.
[22:29] Thank you, Laura, for being there. And yeah, it's definitely, it was exciting to tell people to fuck it in public.
[22:41] For context, that was the title of the talk and that, and yeah. Go find me on Twitter if you would like to know more. I posted my deck. It's pretty exciting.
[22:53] @jenjanod. Yeah, I gotta say fuck it a lot. Okay, look, it's in my box. I can point to it. I think
[23:00] I'm pointing the right direction. And I think, I think, I think it's important to mention Jay's disclosure here. While not
[23:07] fully a Microsoft event, that is Juneteenth conf, I believe. I do think a lot of the folks organized it are Microsoft individuals, which is good to know. Thank you very much. And
[23:15] you know what? Since I have admin control here, I'm just going to say thank you, Suze, for pointing out my curls today. Very much appreciate it.
[23:23] And also, hi. Hi, Suze. Hi.
[23:26] Hello, hello. All right.
[23:28] Thank you for the detour, everyone, and yeah, I'll come out. That is what we do on Miss Mondays.
[23:37] Yeah, and thank you for talking about shit you don't want to talk about because this is so much, so important to me. And I know it's important to y'all, too. And Ren Taxor,
[23:54] is there anywhere else live? So you're talking about CFPs because that is Calls for Proposals. I could link a website
[24:03] that I go to quite often, if I may, which is ccfp.com, which has a nice table with open Calls for Proposals to conferences, that is, so you can go and submit a proposal for a
[24:19] talk. And what I like about it is that it not only tells you where it is, when it's going to take place, when it closes, but also whether they cover travel and accommodation,
[24:28] which I think is, and whether it's online or not, both of which I find can be very important if, say, for example, for a long time, I was funding my own travel for conference speaking
[24:38] because I was self-employed. And I find that to be a really helpful resource. So thank you very much, Ren Taxor, for asking, if that is indeed what you were asking, which I would
[24:52] assume it is. My laptop died. But not my laptop, my keyboard.
[25:04] And yeah, Suze is so right that covering the expenses for travel is such a key factor in increasing the diversity amongst speakers, such an important inclusion factor.
[25:18] All right. All right. Last two minutes, and then I'm going to, like, just try to force us to change
[25:32] into the topics, because we only have Ramon today. So any other last thoughts, anyone? All right. Last call. We got a minute.
[25:55] What I like about the format of Miscellaneous Mondays is that it really is just an invitation for topics to go wherever, and it's more of an interaction. This is one thing that I really
[26:07] love about streaming is that it kind of gives you that opportunity to sort of really engage with your viewers or listeners and see what it is that folks are curious about or what
[26:23] is going on. Miscellaneous. All right. I'm about to be curious about something. Is there an earthquake where you are, Ramon?
[26:31] Well, Austria is nowhere near any tectonic plates, but I tend to lean on my desk a lot when I'm talking, and my camera, which is my phone, is attached to an arm, and it's
[26:47] not – yeah, sorry about that. It's not very stable. That's okay. See, because I live in – well, okay, for any people who don't know, I live
[26:55] in the San Francisco Bay Area, and so, you know, the ground, it shakes around here, and we're fairly chill about it. We sort of assess, like, oh, is this a big one? No. Okay. And
[27:05] then we do actually just keep going. In fact, okay, here we go. I used to have a squirrel. He was a tiny baby, and he had fallen out of his nest or whatever it is that squirrels
[27:17] have. I don't actually know. And my husband found him, and he watched him all day to see if the mother was going to come back, and she didn't, and so he brought him home, and
[27:27] we were going to take him to a wildlife refuge, and they were like, well, if you've already handled him and so on, then he's probably not going to be rehabilitatable. In other
[27:35] words, they would just put him down, and we were like, okay, well, I guess we screwed up, so we will foster a squirrel. And so he was our squirrel, and when he was, like, two
[27:47] months old, we had a whole bunch of earthquakes in a row, and on, like, the sixth earthquake of like 36 hours or something, he had a little toy that was, like, hanging in his enclosure,
[28:04] and it was swaying. And you know the opening scenes of Mary Poppins when there's the dude that, like, has cannons, and he, like, sets the cannons off, and so it's, like, at the
[28:14] same time every day, and so it's everybody, like, runs around, like, steadying things because they know that at, like, six o'clock or whatever the cannon's going to go and,
[28:23] like, various things are going to, like, fall and shake and so on, and they, like, steady them, you know. Yeah. Okay, so that happens, and then the squirrel on, like, the sixth
[28:33] earthquake just reaches out very nonchalantly and holds his swaying toy until the earthquake finishes, and then he lets go and goes about his day, and I was like, you're a Bay Area
[28:46] squirrel now, baby. I was so worried you were going to say, like, it crushed him. Oh, god, no. I was like, oh, no. No, no, no. Goodness. No, no, no, it's a funny story. Okay, thank
[29:06] you. Okay, I'm done now. Okay, so after talking about some squirrels and racism, because that's Misc Mondays, let's talk about OBS and what OBS is. So, Ramon, I'm just going to hand
[29:27] it over to you because you know OBS, and I don't even know where to start to ask questions. Sure, sure. Before I go in, I just want to say, like, you know, I love, again, I know
[29:40] I said this already, but, like, I just love that we have these, the nature of this flow of conversations because, sure, we can switch around topics, but these topics don't go away
[29:48] just because we stop talking about them, so I think it's good to always be conscious and voicing and, I said, willing to listen, ready to listen, pardon me. Cool. Yeah, let's talk
[29:57] about OBS, and I'm going to start, if I may, by, you know, we've all heard that term, OBS stands for, as you see in the title of the stream, Open Broadcast Software, and it is
[30:08] a piece of software that runs natively on your computer, all about video recording and transmission, right? Mm-hmm. Oh, can I do, oh, do we want to do, like, screen sharing
[30:18] and stuff so we can, like, look at the website and all that good stuff? Sure. Yeah, I would love, in fact, to see-- Oh, sorry. I was just going to say, we are currently in StreamYard,
[30:31] and StreamYard is where you can do it from a browser, and it does, gives you seven formats by default, so you can only use seven different versions. You cannot customize the way it
[30:48] looks outside of those seven choices, and you can, it's not as customizable, but it also works really well and is, can be easier, but it's also, like, if you see somebody that
[31:03] is putting a chat on their screen while they're streaming, like, Learn With Jason does, and that's not something you can do in StreamYard. That's something that you can do in OBS, and
[31:19] I think that's another reason why I really want to look at it. Again, for those looking into streaming, if you just want to get started, go with, I personally think, go with, like,
[31:31] StreamYard, because it can be free, and it is a lot easier learning curve. Absolutely. I mean, you know, I've actually given a presentation-- Oh, can I, oh, can I be cheeky and promote
[31:45] this stuff I've done? Yeah. You're showing up and teaching us stuff, so however you want to do it. Well, thank you. I actually gave a talk about this, which is about, you know,
[32:02] sorry, didn't realize it was playing. I gave a talk about, well, it was at DevRelCon, and it was about streaming for DevRel, but I think a lot of this applies to what we're doing
[32:14] with streaming overall, not just for tech, but also for things like what we're doing now, learning and chatting, right? And I think there's merits to both. If we stay on StreamYard,
[32:30] right? StreamYard's great because for your guests, and we'll talk about guests later on, all you've got to worry about is giving them a link and saying, "Show up here. This
[32:40] is, you know, this is how it works. You're not going to be on stage until I bring you on stage, so you can, like, turn on your lights, adjust your camera angle and all that good
[32:47] stuff, make sure your camera's working, make sure your microphone's working," and they're just in a browser as if it were any other voice-- sorry, video call software, which
[32:56] is great. Same goes for you as a streamer. You don't have to worry about, like, messing around with credentials with Twitch. You connect your channel once, and you're done. You can
[33:05] stream to, like, as we're doing here, right? We're streaming to YouTube and three Twitch channels at the same time, which is awesome, but what happens when you want to take that
[33:15] step further, right? For me, actually, I started out on OBS Studio. My first streaming experience was here because I thought, well, you know, I was working at my previous job. I was at
[33:30] an early-stage start-up, and we were figuring things out, as many early-stage start-ups do, and we're just like, "Well, we've got to start streaming. Okay, Ramón, make us
[33:39] a Twitch account, and let's have you start streaming to it," so that's what we did, was use OBS Studio, and what was cool about it is that, as you can see here, free and open-source
[33:50] software for video recording and live streaming, and yes, I use it for that to this day. I'd love OBS for recording video. It's super cool. It's super straightforward, and you can connect
[34:00] it to all the kind of software you want. However, I'm not going to say because it's open-source, but one of the downfalls of it being open-source is that it doesn't have the resources that
[34:11] usually is thrown by mostly venture-capital-backed companies to be able to give it all of those, let's say, bells and whistles that make it more straightforward to work with, right?
[34:23] So there is a learning curve for OBS. Fortunately, they have not just extensive documentation, which I have referred to many times in the past, but it is a barrier to entry. Same goes
[34:39] for a forum for asking questions. Lots of good stuff there. So right, OBS lets you link up your Twitch channel or YouTube channel or whatever, and be able to stream to it directly.
[34:54] So I don't know. Shall I give you a tour of how I use OBS? Yes, please. So much. And if possible, I think it would be really, really cool to see how
[35:08] you set up your layout. Is that what you would call it? That is exactly what I plan on doing.
[35:15] Oh, yay. Because I think that's something I've been really struggling with is figuring out all the different layers, where you put the videos, and there's a lot that goes into
[35:26] it. So yes, yay. Thank you. And I'm going to be extremely painfully upfront and tell you right away that I am not an expert,
[35:37] and I'm also extremely disorganized with it. So my apologies in advance. You're doing more than we currently are.
[35:46] And look what Suze Shardlow says very, very fairly, OBS fries my computer. And that is another thing to mention, right? Because StreamYard runs on the cloud, all of those resources
[35:57] that video processing resources don't come from your computer, they come from the cloud, someone else's computer, and that is something else to take into account. Thank you, Suze.
[36:07] All right, let me share my screen with OBS on it. And I will give you a very brief, like, what I would encourage all of you to do is to please interrupt me and ask me about things
[36:21] because I will likely forget because I am a harbinger of chaos sometimes. So here's what you see, right? This is OBS as I use it running on my Mac. Now, as you
[36:34] saw on the website, OBS runs on Windows, Linux, Mac OS, and probably other but probably it's been built to run on things like, oh, I don't know, OpenBSD or something. Given that it's,
[36:47] you know, open source. And as Suze very correctly says, I also find that there are so many things you can tweak on OBS, so it's hard to know where to start. So it's great if someone can
[36:56] walk you through or better still give you a template to use, which is all entirely fair. I started with nothing, essentially. Let me, let me give you a...
[37:05] Ramon, when he started, it was uphill in the snow both ways with OBS. Really quick, I do want to say for templates and things like that, stream elements is very,
[37:20] very helpful. Yet, I think doing things in like Canva, and then uploading them and doing them in OBS by layers could be a very helpful option, too. Yet stream elements is definitely
[37:38] an option there. So please continue, Ramon, as I so rudely interrupted you. No, no, that is entirely fair. So I mean, I wouldn't call this, I wouldn't call this
[37:50] going uphill in the snow, because really what I did was do the minimum that I needed in order to get it working, and then sort of add to it as I go. Let's walk through this
[38:02] real quick, and it's going to be a bit chaotic. Again, apologies in advance, because I'm going to just resize my window real quick. It's going to look a little bit gnarly, so I apologize
[38:10] in advance. Unfortunately, I don't believe that it's possible for me to increase the font size of OBS, so if anything looks out of sorts, please let me know and I'll happily
[38:19] read it. Oh, okay, I do have a mouse. Fantastic. Let me just give you a brief tour of what I have. What you'll see here on the left-most bottom column is scenes, and scenes you're
[38:35] going to recognize from StreamYard. In fact, Laura and Jen, you might see, depending on whether you're managing the stream, you know where we have those different layouts that
[38:44] we can have with the person photo and the different layouts? In OBS, these are called scenes. The difference between OBS and StreamYard in this case is that StreamYard has a fixed
[38:58] set of scenes, whereas OBS lets you run freely with whatever you want to do with them. I'll show you what I have here. What you're seeing here is what I call my browser scene. What
[39:13] I've got at the top is a background image. Jen mentioned Canva, love Canva, I used Canva to make this. It's just got my name and my Twitter handle. Below that are one, two, three,
[39:28] four elements that you see. One is a browser window, which is sharing my browser's window, as you would on StreamYard. You've also got here an app that I believe is also free and
[39:40] open source called Chatterino. What Chatterino lets me do is have my chat on the stream. You might be wondering, "Ramon, why would you want to do that?" What I like about it
[39:51] is that it lets me show the viewers what the chat sees and also lets them see what I see by the time they see it. What does that mean? You see, most streaming platforms, including
[40:04] Twitch, do have a delay. This can be about 30 seconds between someone sending something into the chat and the person streaming seeing it. This way, I can see -- you see, Suze just
[40:18] wrote, "Ah, yes, the delay? I just saw it." That helps me keep an eye on what's going on. You'll see here my webcam. What about here? Here's a blank piece of space and also
[40:36] -- hold on. Let me see if I got it here. These are the elements that make up my scene. You see, I mentioned a window capture, an audio output capture -- more on that later -- and
[40:46] then something I call OC. You'll see that it's a blank piece of text. Now, I can't show you it directly now, but I'm going to start recording a video and I want to show -- I
[40:56] hope this works. What this is doing is open captions. Now, this is something that StreamYard unfortunately does not have built in. Neither does OBS. However, because OBS is open source
[41:19] by nature -- I'm just marveling that everything is working. It's not 100% accurate -- is that there is a plugin, which I will link shortly, that lets me integrate this into OBS. For
[41:36] me, accessibility matters a lot. And it's never going to be perfect. Fun fact, these are called open captions. You might have heard of closed captions. This plugin allows you
[41:47] to do that, too. So, this plugin lets you not only have the open captions, which you see here, but also the closed captions that go directly and embed into Twitch.
[41:57] >> Oh. >> Yeah. So, you might see most streams -- sorry. A lot of streams that have closed captioning, when you're watching, will have a little CC
[42:11] button next to them, you know, in the player options, so that you can turn on those closed captions. Fun fact, I learned this from my ex-co-worker, Liz, who is brilliant. She told
[42:22] -- because she works -- she makes indie films. And she told me that that turn of phrase comes from cinema. Open captions being they're directly embedded into the film. And closed captions
[42:35] being optionally put in. >> Ramon, will it auto-switch languages, or will it need to -- do you need to switch the input language for it to switch to Spanish
[42:48] or something else? >> That's an excellent question. And as people Dev says here, speak in Spanish to see, please. I'll speak very briefly. [Spanish] Unfortunately,
[43:04] it does not work with Spanish. I think it's only English. And as you can see, it didn't really capture any of my Spanish. So that is a limitation.
[43:13] >> I'm surprised that it literally printed nothing. It didn't say something like unintelligible or like foreign language can't translate, something like that. It just was like, nothing.
[43:28] Nothing happened. >> Yeah, it doesn't even try. Some of the time. [Spanish] I said with some words, maybe. But I guess not. It depends. It depends
[43:39] really because -- oh, so this is using Google -- I always mix this up -- speech-to-text to do it. So, again, this is something that's built in -- sorry, this is a plug-in, and
[43:54] Laura, let's grab that link, because that is correct. What is it? OBS. It's in my Firefox license. I'm going to post that link. It is the correct one, the one you linked. I'm just
[44:07] going to put it here so it goes to all of the channels we're streaming to. So I stopped the recording. It's not going to capture them anymore. This is the essential make-up of
[44:17] my OBS set-up. And you'll see that I have lots of options. Sorry, lots of scenes here. For example, I have a code one. Usually what you'll see here -- I don't know which way
[44:31] I'm mirrored. Am I pointing to my screen now? To my window? >> Yes. >> No.
[44:36] >> Oh, to me you are. Oh, wait. Which one? Because in StreamYard, yes. In OBS, no. >> See? I'm getting the mirrored effect. >> Oh, yeah, I was looking at OBS.
[44:51] >> So to my left -- goodness, I'm going to stop gesturing. To my left, you will see blank. This is because I would usually have VS Code open here. This is my coding scene. Let's
[45:09] see what else we got. This is what I call the play date scene. Now, it's not -- this is not to do with actual play dates, but rather a console, a games console that I sometimes
[45:20] develop games for called the play date. Super fun, by the way. I used to do lots of streams about that, so I can show it off, and I have an emulator running somewhere here where you
[45:31] can see that in action. It gives me the flexibility to be as creative as I like with my scenes. I also just have a generally chatting scene, so I can be up front and say hi, just sort
[45:42] of be there, have the chat, have my captions. But here's another thing I have. Because I have that flexibility to do so with my scenes, I have a starting soon scene. What's this
[45:54] about? And this might be interesting to folks who are looking into streaming. Usually when people are following you, not subscribers, see, I got to get the Twitch terminology right.
[46:05] When folks are following you on Twitch, when you start streaming, they will -- Twitch will send out notifications. And these can take up to about five minutes to send. So what
[46:17] I usually do when I start streaming is I will give it about five minutes before my allotted time and show the screen and have some music, more on music in just a moment. I also have
[46:27] a goodbye one. I don't -- I'm torn on these. I don't think you need them, but I like sort of telling folks, like, I'm gone now. Sue says the push notification was how I knew
[46:41] you were streaming right now. There you go. >> That being said, definitely go follow all three of us. Because we happen to be on each other's streams a lot. So -- and it's -- that's
[46:57] one of the reasons why we're streaming to all of them right now. Not always something that we can do. Yet all of our names are actually -- Laura is -- it's still Laura Langdon on
[47:10] Twitch. So Ramones is HolaSoyMilk, Laura's is Lauren Langdon, mine is Jen Jenaud. Because we all talk about this educational stuff in some aspect. Because we're all about learning
[47:29] life. >> Thank you, Jen. I just want to mention a couple of things that folks have said in the chat. People have said maybe if you start
[47:39] with one language, it will stick with it. I don't think so. I really think it just sticks with English. It could be. Have a look at the link that I posted. Maybe it says so there
[47:49] in the repo. The Git repository, that is. Ryan says something here that I want to point out as well. I know when some streamers rate a channel, they would like to know if you're
[47:59] ending soon. That's helpful as well. If you see this. And my friend Flacky, who is a joy, he told me it's good for video recordings to also know the cutoff point. So that's helpful
[48:12] to know as well. Cool. What do we got? I also stream sometimes in -- my goodness, I don't even know what's going on here. You'll see my entire mess.
[48:21] >> It's Spanish. >> Yeah, sorry about that. I've got some streams in Spanish, too. And you'll see that I've got -- I'm just going to switch back to something
[48:28] less screaming. I've got a bunch of scenes. And you're actually getting an inside look into how utterly disorganized I am. And I apologize.
[48:37] >> Aren't we all? >> Ramon, can I steal the screen share really quick? >> Go for it.
[48:46] >> For like a second to talk about languages. >> Please. >> Okay. Because this is also a really cool part about when you have multiple people streaming
[49:00] is you can multitask more, which I enjoy because then I'm like, oh, I can go look. But in the OBS captions, they did include some screenshots. And it looks like you can change the language.
[49:15] >> Awesome. Thank you. Good to know. Jen, would you mind please making it bigger? >> Yeah. >> Phone size is a bit small.
[49:25] >> No, maybe. Okay. There we go. >> Much better. Thank you. Folks, if at any point something is too small, please let us know.
[49:34] >> So I don't know what languages may be an option, but it does look like it is at least -- it would be a drop down here. Okay. Back to you, Ramon. Thank you.
[49:47] >> No, no. This is fantastic. Thank you so much, Jen, for pointing this out. Let's look at the settings of closed captioning real quick. Let me see where I can find that. I'm
[50:02] going to have to share a different window now. This is what we can examine, and I can already see that you can indeed pick the language. So I'm glad we went down that path. Oh, I
[50:15] can't make it smaller. Fabulous. I hope that's okay. Again, since I'm streaming software instead of a browser, I don't know if I can -- I cannot make it larger. But what you can
[50:25] do here is, you know, enable captioning, choose the source, which I think is important, because when you're streaming, and because OBS is open source, you can pick a myriad of different
[50:38] microphones and cameras. Some streamers you'll see have different cameras pointing at different things. For example, I have done it before where I've had my phone filming one thing
[50:49] and my webcam at my hands when I was doing hardware stuff, which is always good fun. It's good to have that option. And, yes, indeed, we have a myriad of options. Not only can
[51:01] we have Spanish -- >> You can't see them. >> Oh, no, you can't. I'll read them out, if I may. Not only do we have Spanish, but
[51:07] we have a myriad of Spanish options. Pick your favourite. Peru, Puerto Rico, Dominican Republic, Venezuela, Argentina, Chile, Colombia, Costa Rica. We have different flavours of
[51:19] Spanish, which is quite cool. I think these come from Google's engines, which is -- there's even a profanity filter? I've got to turn this on. Unreliable. Oh, you can't see, but
[51:29] the dropdown has off and on and then in brackets unreliable. You can see it here if I pick it. I'm going to leave it, because why not? Capitalization.
[51:36] >> I feel like it will just bleep out everything I say. >> Which is fair. What else we got? Transcripts. You can download transcripts. You can save
[51:47] transcripts of your captions. Open captions, this is what you saw me using. You can pick a text source, which is that very specific element that you put into your scene. I'd
[51:57] love to explore creating a scene, if I may. Would that be compelling? >> Yes. >> Definitely.
[52:03] >> Oh, you can even have text filtering. I'm glad we went into these options, because, again, I'm a very lazy person, and I don't take the time to explore options enough. Before
[52:17] we do that, I'd love to explore the options of StreamYard, because I think these are relevant as well. And I have -- I don't even know what to call it. A secret nugget of wisdom to share
[52:32] about testing your streaming, because this is something I get quite anxious about. I'll get to that in a second. You've got your options for the software itself, but also some options
[52:42] for streaming as well that I think are important to note here. Because as I said, you can stream to different places. It looks like you can only stream to one at a time. Maybe there's
[52:51] a plugin to make that more flexible. But you can pick -- oh, you can't see. There's Twitch, YouTube, Facebook Live, freestream.io, Twitter, and there's more options. Also, there's very
[53:04] specific URLs for something called RTMP, I believe it's called. It's some kind of protocol. I'm not actually sure what it stands for. But if somebody's curious, maybe they can
[53:15] help us find out. Pick your server. I'm streaming in Europe, in Vienna, in Austria, so I pick that. And have your stream key. Now, I'm not going to click on "show", because if I show
[53:26] that -- I will not endanger my streams. I'm very sorry, folks. But, yeah, you can post your stream key there. And you can get -- they even have options for getting them and connecting
[53:40] your account directly, which I find to be helpful. But as I said before, it's not just for streaming. It's also for recording. I do -- I'm working on a course in collaboration
[53:52] with Egghead and Escuela Frontend to make a TypeScript course. If you're following me, or if you're people that have even helped me, thank you once again. I was streaming
[54:03] live the course materials. And I record them with this. And it's good -- I mean, you know, it's processing video. Why not use it to record videos as well? It gives you that flexibility
[54:15] of having layouts and this sort of thing. I think that that about covers everything to do with options for OBS, except for one part. I'm going to go back to sharing my browser
[54:29] now. So, let's see. Twitch test stream without going live. So, there is -- I just want to check if it's going to show you my key. So, I'm just going to -- I'm just going to briefly
[54:44] share my screen. >> I am so glad that you're covering this. Because I have so much anxiety about this. I tried when I very first started to set up
[54:55] a stream channel, I tried testing -- I was trying to test. And it actually went live. And I panicked. And I'm probably still panicking. And that was six months ago.
[55:05] >> I had to test it out to see if it would give a Discord notification. So, I purposely went live. And I was like -- and somebody got the notification. They're like, I got
[55:14] duped. I was like, no! I had to test some stuff. I'll DM you on Discord. Calm down. >> In that case, I highly recommend this tool. I'm going to paste the link here. It's called
[55:29] the Twitch Inspector. And what it lets you do is precisely that. Test your stream before you go live. Now, I'm going to steal my window here for a second. So, I'm just going to log
[55:39] in with Twitch and essentially see what happens. Because I quite frankly have no idea if it's going to show my key. But if it does not -- which I don't believe it does. Hold on a second.
[55:54] I have to diagnose issues. Ah, brilliant. Brilliant, brilliant, brilliant. So, give me one second, folks. Because I do think this is, like, really interesting. Really interesting
[56:12] stuff. As I said, for testing that stream. Okay. So, since I'm streaming live right now, this is what you see. You can see that I've got a stable bitrate. You can see that I'm
[56:25] streaming today at January 16th. I started at half past 6 p.m. Central European time. And that I'm live. Which is all well and good. And I need to double check what that is. But
[56:39] I believe I'm not in any danger by doing this. Help guide. Broadcast URLs. Now, let me see if I can make this larger so we can all read it. It's best to understand what a broadcast
[56:53] URL looks like and what it does. And this is the critical part that I want to add here. This bandwidth test option. Bandwidth test equals true. What this does is if you add
[57:05] it to your key in OBS, so, like, you know how your key is a string, right? When you link up your Twitch to OBS, you're giving it a stream key. Like a piece of text that
[57:17] is essentially kind of a password that Twitch looks like. Ah, I know who you are. You're HolaSoyMilk_. You want to stream. I gotcha. Now, if you add this bandwidth test equals
[57:30] true, what it does is it says, all right, I will stream, but nobody's gonna see it. And as far as your viewers and followers are concerned, they're not gonna know. However,
[57:40] you can come here to inspector.twitch.tv and you'll see this. And you'll see that you're live and that you're streaming this much and your bit rate looks good, it's stable and
[57:50] all of that, and all of that stuff. So, highly recommend that. >> Mm-hmm. Yeah. That is very cool. I think I actually I used this, but somehow because
[58:03] I was using it when I first started trying out Stream Lab, my brain made it a Stream Lab feature.
[58:10] >> Gotcha. >> Oh, yeah.
[58:12] >> Which it isn't. >> Gotcha. Actually, that is a good point, Laura.
[58:17] >> Apparently, that happened. I just found out that happened in my brain. >> And that --
[58:24] >> Streams are big. Like, they're real. They are real. >> But I think, Laura, you're making a very important point. This is limited to Twitch.
[58:34] So, if you're streaming to YouTube, unfortunately, I don't know of a solution off the top of my head. If somebody else does, please feel free to share it. But, yeah. So, this inspector
[58:45] for testing your stream, just to make sure that the connection is right and you got the correct key, which is a big part of it. Again, like, it being so kind of like hodgepodgey,
[58:54] you know, kind of Lego bricks put together, it can be a little bit nerve-wracking to be like, did I do everything correctly? So, yeah, it's super helpful.
[59:01] >> Yeah. I think it -- I also -- I ended up not using -- it didn't do what I wanted it to do. Like, I actually wasn't really worried about the technical part.
[59:12] >> Yeah. >> I just sort of assumed that all that shit was going to work. I wanted to experience
[59:19] like, okay, this is what it feels like. This is what it looks like for me. This is -- so, making sure that, like, my transitions are going the way that I want them to and that
[59:28] everything looks right. And that part, I think you can preview, at least in Streamlabs, you could preview it. And I'm sure you can preview it in OBS, too. But I wanted to see what it
[59:36] -- like, I wanted the entire experience of streaming without anybody seeing. And that I was not able to make happen.
[59:49] >> I guess that's where the video recording might be suited best, huh? >> I don't know. Because I wanted to play with, like, chat features. And, like, I wanted
[60:01] the entire experience. So, actually, what we did was my husband created a Twitch account. And I used his key. And it had no followers and so on. So, I just, like, streamed to an
[60:16] account that nobody was looking at. >> Yeah.
[60:19] >> And, like, that did what I needed it to do. But that feels like an elegant solution. It feels like you should be able to just do that.
[60:28] >> I feel like I would just stream and let people watch it. And if I need to, just ignore them. Be like, hey, I like that you're here, but I can't talk to you right now. I am focusing
[60:39] on this. And if I acknowledge your existence at the moment, I'm gonna get embarrassed. So, you don't exist at the moment. And I'm gonna be trying stuff. So, hang out if you
[60:49] want. >> Jen, you know, if you haven't yet, I think you should give a talk about this topic. I
[60:54] think it would be helpful. >> Yeah.
[60:57] >> Let's do it. >> For context, folks, Jen Kava talking. You got this broadcast service on Saturday, Sunday
[61:05] very early here. About how to go about this. Getting over that speed bump of -- can we call it perfectionism?
[61:20] >> Yeah. Yeah. Suze says that they're stream buffered. And what did I not want people to see? Anything. I didn't want people to see anything. I wanted no eyes upon me while I
[61:35] experienced everything except eyes upon me. >> Until you're good and ready. No, I feel you. I feel you very strongly.
[61:44] >> I will say, and I do want to give a shout out to these two right now. I am very much a fuck it, let's do it. It'll be fine. I'll just do it in front of everybody. I'll be
[61:57] really embarrassed. It'll be great. I don't care. And I need structure. Or people to tell me that this is stupid. No, not stupid, because I don't like that terminology anymore, but
[62:08] this is silly. Or this just doesn't flow very well. And y'all, in the last minute, I'll noodle about things. I found out I think on Wednesday that I was giving a talk on Saturday.
[62:23] So I just thought about it for four days and then actually put it together on Saturday. And then was like, hey, I don't know if you guys are actually up to this, because my talk
[62:33] is in three hours, but if you could, please review my deck. And they both did. Ramon actually went through it slide by slide with me, and I really enjoyed it. And that is a big part
[62:44] of why I think we still need people that say fuck it in the world and encourage others to just get started. And then we need people with structure.
[62:53] >> I need more of that fuck it energy. >> And I need a structure. This is why we get along so well. >> I don't even know where I fall on that.
[63:02] I mean, I think it also varies from thing to thing that we're doing. For example, talking about this, you got this talk, not to take us too far off topic, but I've been nervous
[63:11] about this talk since it got accepted, I want to say September, October. But I only finished it on not too long ago. To be discreet for my co-speaker's tarn sake, I don't want to
[63:30] something divulge too much to respect them. Oh, I want to highlight what Sue says. I think it's important to note. To be honest, it takes so long to build an audience that someone
[63:48] new to Twitch could be streaming every week for months and only have a couple of viewers. And this is something that my dear friend Rizel actually touched upon that I really
[63:54] liked, which is even if you have no viewers, you're still getting something out of this. Especially when it comes to learning in public. Like one of the best things that's ever happened,
[64:05] one of the best things I ever realized from streaming, and I realize this is not super on topic with OBS, but I think it's still worth mentioning, is that you're explaining
[64:12] things out loud, especially if you're like me and you have a lot of anxiety and you don't want to be just coding silently on stream. Not that it's bad to do that. That's just
[64:21] me imposing on myself how I should stream. Explaining things out loud forces you to kind of understand it. And so when I realized that teaching is one of the best learning tools.
[64:35] So much. Yep. That's what I... So for those of you who are new to me, I was a math professor until a year ago. And that was something that I really enforced for my students. Because
[64:55] I would, and they would push back a bit because students are really used to the format, especially in a math class where the professor stands at the board and write stuff down and solves
[65:08] problems from beginning to end and so on. And so you just get to see, this is how you do this and this is how you do that and blah, blah, blah. And I didn't teach that way. I
[65:18] would solve an example problem and then I would turn it over to the students to do it in groups. Because you can watch somebody do something and think, "Oh yeah, that makes
[65:30] complete sense. I've got this." And then you go to do it yourself and you're like, "Oh, I don't got this at all. Nope." And that's when you find out. And so what I would tell
[65:39] the students is it's way better for you to find out where the gaps in your understanding or things that you thought worked one way, but they actually don't. It's way better to
[65:49] find out like here, while we're all still together, instead of having a dark night of the soul about it at home when you're trying to do your homework or take the exam or whatever.
[66:03] And then especially since they were, a lot of students were also, they were working in groups and so a lot of students were uncomfortable with that. They wanted to just do it by themselves,
[66:11] which I completely empathize with. And so I would say, I 100% empathize with you right now. I am still going to encourage, not require, because that's not helpful. I am still going
[66:22] to encourage you to work together because teaching something is the best way to learn it.
[66:30] Absolutely. Yeah.
[66:32] Reading out loud is great too. Actually, that's the way I made my one so far free Code Camp contribution was I was, for work, I was setting up free code. What was I doing? Maybe it wasn't
[66:45] for work. I can't remember. Sorry, it's not relevant. I was going through the free Code Camp documentation and reading it out loud. And that's how I found a typo, a typing error.
[66:57] Because I was reading out loud, I literally stumbled over the word, well, not literally, you know what I mean? I stumbled over the word and I was like, hold on, that's a typo.
[67:05] I'll go fix it. And that's how, that's, that was my contribution to free Code Camp. I give Ramon a funny look every time he says read out loud, because this is the reason
[67:19] I read out loud is because of Ramon and I don't wanna, because it's really hard for me. As for those who may not know and be new to me is I am very, very dyslexic. So reading
[67:33] out loud is a great practice. And it's something that I've done research on being dyslexic that it is, I have a really hard time sounding out words. And luckily being that one of the
[67:48] streams that I do the most is with Laura and Laura is very patient with me while I'm trying to sound out words and read them out loud and comments are a great way to get started.
[68:00] And I know that we only have 20 more minutes and I just, I'm going to pause this really quick because I feel like we did go through a lot of OBS things. This is Misc Monday,
[68:15] so this is what happens. So I am just going to awkwardly ask on, on the screen if Ramon will come on again sometime because I feel like we could go more into deep diving on
[68:29] creating the layouts and like starting from scratch. I think it would be really cool maybe if you walked through like next week, Laura or I setting up a layout and us-
[68:43] I was so going to ask. I realized I went off topic. Yeah. Going from Canva to going to OBS because something I've learned quite a bit, especially
[68:54] working with these two is I get what you're saying. Like everything you said makes sense, but going from the what to the how is a huge blocker for me that I think it would be really
[69:09] helpful seeing that from scratch. We can do, we can do, Ramon can be me and we can be my students where you can hear somebody say something and be like, yep, that all makes
[69:22] sense. But then when you go to do it, you're like, oh no, I don't get it. Yeah. And I think, I think that's a great idea and I'm super happy to do it. I would love to,
[69:33] if I may just point out a couple of caveats of using OBS because I don't think we got there yet and I know we have, we're running out of time, but I do want to point out a
[69:40] couple of caveats and also one more technical part. So I'll start with the one more technical part because this differs from person to person and I've actually met, I've actually streamed
[69:51] with people who are like Ramon, please do not do this when I'm on background music. Let's talk about background music because I think this is relevant. So let's start with
[70:00] StreamYard. StreamYard has built in background music. Warning in advance, I'm going to play just a tiny bit. Do feeding ducks, do feeding the ducks.
[70:11] Feeding the ducks it is. We'll clarify what this means in just a moment. So you're about to hear some music, right? What you're listening to now is built in music created by or licensed
[70:28] to folks at StreamYard. The problem with music in StreamYard, and this goes for video as well, is that algorithms are constantly running on Twitch and I believe YouTube as well, to
[70:41] make sure that there's no copyrighted content on your stream. So if you start playing, name me an artist, please. If you try to, like any artist, basically,
[70:52] you have to have royalty free music or have a license to use it. Like there's actually an announcement, random announcement, is there is a musician that I made friends with on
[71:04] TikTok that is like, yo, dude, if you want to start using my music on your streams, do it. I'd be, that would be down. So no. So the way that something like that would go
[71:18] is I would need written permission from them and I have to at least have it in the description and if possible, also saying it in the stream as well. Because it's also like, you know,
[71:33] you don't want to not give somebody credit if they're doing dope here. So, but if you just want random music, look for royalty free.
[71:44] So that's the thing. The royalty of music, very important, and having that written permission also very important. I think the problem, and I'm not an expert, so I am not, and I
[71:55] am definitely not a lawyer, so don't take this as super solid advice here, but I don't think that circumvents the algorithm. The algorithm doesn't know that you have that
[72:03] written permission. So when in doubt, try to avoid using music that is copyrighted. That said, StreamYard, what about OBS? And this is where I want to introduce another
[72:16] piece of software that I would love to recommend. That comes with its own caveats. If you have the monies, Jay recommends Epic Mic Sounds or Storyblocks.com. Super cool.
[72:31] Both of those are really cool, and Epidemic also does, I believe, Elements 2, which it will have a lot of graphics and so much more that you can use as well. And I think Storyblocks
[72:47] does too. Here's another platform and tool that I would love to recommend. Whoops, I am zooming into
[72:54] the wrong website. So this is Pretzel. Pretzel is a DMCA, Digital Rights Millennium Copyright Act, something like this, which is an American law, but also most copyright-free radio. This
[73:13] is a radio that you can set up on your computer to play royalty-free music. And I have this installed on my computer. I'd love to just briefly show you it. No, I need to log into
[73:28] Twitch with it real quick. Give me two seconds, folks. I promise, this is super, super relevant and I think you'll like it.
[73:34] As a side note, while they're working on that is music is very, very debatable, whether or not people want to have it on their streams. It's not just because of what we're talking
[73:47] about right now, but because of distractions, how people learn, neurodivergencies, like there is a lot that goes into it. Like right now, if we had music going, it would be like
[74:00] too much. Like I would like literally be like crawling in my skin trying to hear and talk at the same time. And like, probably just like at mystery because it's really hard for
[74:13] me to do both at the same time. Where is if I'm streaming alone, it's really weird to not have something talk back to me that I'll put music in the background because I'm like,
[74:23] I'm just talking out loud to myself. I don't really need to listen, but it happens. And that is exactly it. So like, you know, keep in mind of keep your audience in mind.
[74:33] And if somebody says like, Hey, can we turn off the music? Totally, like, absolutely keep that in mind. Now, this is pretzel rocks running on my computer. It's linked to my Twitch.
[74:43] I'll show you why in a moment. It's also I've also enabled YouTube safety, because YouTube and Twitch have different licensing thingy bobs. And I have it on instrumental because
[74:53] lyrics distract me. Yes. Talk about stations for a second. Again, you have a whole bunch of options. I'm a lofi person myself. So I'll put on the lofi channel and just but you've
[75:05] got a whole bunch of stuff you got if you want to code to metal. Be my guest. You want to code to pop EDM, classic rock, chill, and so on. This is really cool. And I said this
[75:15] is all royalty free. And I'm going to show you in just a second what happens if I play it because I want to show you something that's gonna like, I hope this works. Give it a minute.
[75:29] The way it works with the copyright, and I hope this shows up. I'm waiting for it. Let me put on another so I'm going to skip to the next one. I promise there's this is relevant.
[75:41] Because it's linked to my Twitch. Hey, there it is. Fantastic. This is how it gives credit. A comment shows up in your Twitch chat, saying who it's by, and a link to cool. So this is
[75:58] this is a really useful tool for that. Jason says if somebody asked me to turn off my music, it's the block. I'm only slightly kidding. My stream in my environment, I'm not going
[76:08] to conform to super fair, super fair, happy to lower the volume if it's too loud, and you can't hear it. But I'm not changing things. And that's absolutely, absolutely fair. This
[76:16] is you have the liberty, the flexibility to be able to choose how you best stream. On that note, really, really quick is that you can wear headphones and you don't have
[76:28] to stream your music. So that way, if it's something that is, like personally something that you need to do it, but you'd like a lot of your listeners, viewers, outvote you, you
[76:43] can find other ways to work with it. Or you can choose to do what Jay said and not conform to them. You're sharing your power. Exactly. This is the wonderful thing about livestreaming.
[76:59] You don't have to conform with any trends. You don't have to have, you know, I can't think of an option. You don't have to have a green screen. You can be like me and just
[77:06] have a mess behind you. You know what I mean? Like the options are yours. And I think, ah, technical caveat to streaming music from Pretzel Rocks, and that comes down to an operating
[77:17] system level. One of the inputs you can have on OBS is called audio output. What this means is that you can say, hey, have the audio that's going to my headphones also go to the stream.
[77:29] Super helpful if you want to stream music. Works great on Windows. Tricky on macOS. It is possible. And you'll have to install some open source software. But it is a mess. So.
[77:46] I'm going to pause us right there. Because I'm sorry. Because, you know, we got I have a hard stop at nine minutes. So I'm going to start wrapping us because this is what
[78:05] we normally do is an hour and a half. And for those who may or may not have noticed, on Mondays for Misc Monday, Laura and I will be starting a half hour later, which is 930
[78:18] Pacific, 1230 Eastern, 7 6. And more times as well. 6 30. Yeah. I don't know. I don't know. It's somewhere. It's half an hour later than normal. How about that? And just wanting
[78:37] to give everybody a heads up. We actually for those who are coming to my channel, I guess I'll say Mondays are still going to be Misc Mondays with Laura. Tuesdays are going
[78:49] to be just like whatever random guests. Wednesdays are. Neurodiversity and mental health Twitter spaces Thursdays are distributed with Ramon. And I don't know if you're there in my screen.
[79:06] You're there. Maybe you're over here. I don't know. And on Fridays, every other Friday, it's either TypeScript with Josh Goldberg or Python with Laura. So I basically have
[79:20] a pretty consistent schedule now. It's crazy. I'm very excited about this. And please, please, please. If you're joining in from my channel, go follow the beautiful humans that are joining
[79:34] us today. Look, this works. This works. I'll just like try to push you up and hold you up and be like, Hey, I don't. And yes, bunch of random shit. Yeah. So sorry. Just a gentle
[79:49] reminder, because we were talking about this earlier. I did notice that you use the word crazy. Try to opt for using something like wild or incredible stuff like this.
[79:59] Fair enough. I feel like that's gonna be really, really struggle bus for me. I feel like struggle bus is okay because it's a bus and it's not saying like the short bus. It's a struggle
[80:13] and it's a bus because I also say bus chat. I'm just very bus themed. Jen, it's not called if if it were easy, it wouldn't be called the work.
[80:26] It's true. It's true. And I appreciate the call out because that is something that society has taught me taught us all one way that we have to many of us have to put in the work
[80:35] to relearn. And it helps having people call us out. So we actually take time to go. Like, I don't even know where I said it. But I'm like, Oh, yeah, I probably did say it. So
[80:47] be more conscious about that. Thank you. Thank you for being so receptive and willing to listen.
[80:54] Never. I don't wanna. I don't wanna. Fair. Well, hey, listen, it was it was a joint chat with y'all. We definitely want to cover
[81:05] like, talk about like, having guests on OBS, which is a whole topic. Sometime that we're actually planning on doing so and got a little sidetracked because it's miscellaneous. See,
[81:21] that's what it is. I actually did reach out to the person that I was telling you to about no reply yet, but we'll see if they want to come on the show as well. I think to be to
[81:32] be determined. Mm hmm. And to be continued, hopefully. Mm hmm. Yes. And I hope you all have a wonderful Monday on. I can say that I don't know what I would do without Laura
[81:48] on Mondays because y'all I missed a very important meeting this morning. And I will say by the time I get to miss Mondays, no matter how bad my morning was, it resets. And I really,
[82:03] really appreciate it. So much likewise, because, you know, it's it's earlier for me. So it's it's almost the first thing my first thing on Mondays. I do now have a meeting on Mondays.
[82:16] That's before this. That's why we have shifted back half an hour. And and so it's almost my first thing on Mondays. And so it just sets like a lovely tone for starting the week.
[82:27] Yeah. And for me, it's a good it's a good end to the day. There you go. Yes. Yes. All right. I am going to read y'all over to I don't actually I've never said their name
[82:41] out loud. I'm Prime Agen, Prime Agen, Prime Agen. I don't know. We're just going to raid. So bye, everybody. Bye. As it counts down. Because I hit Prime Agent. Oh, it's Prime
[83:08] Agen. Oh, cool. OK, well, y'all are going to Prime Agen. OK, bye. See you later. - Bye.
[83:18] [BLANK_AUDIO] 
