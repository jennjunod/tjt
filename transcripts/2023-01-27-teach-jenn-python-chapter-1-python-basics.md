---
showLink: "https://www.youtube.com/watch?v=gAMCN5hb1vs"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-python-chapter-1-python-basics"
title: "Teach Jenn Python Chapter 1: PYTHON BASICS"
publishDate: "2023-01-27"
coverImage: "https://i.ytimg.com/vi/gAMCN5hb1vs/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to the first in this series.
[00:08] We're going to go with this as the first one of us redoing Teaching Jen Python on Teach Jen Tech with Laura,
[00:17] who is also the co-host of MISC Mondays. If you ever want to hang out on Mondays,
[00:23] come hang out with us. My name is Jen. I'm not good at summarizing who I am.
[00:33] We do this like every episode, so I'm just going to say,
[00:36] go to teachjentech.com to find out more. How do people find you and reach out to you and talk to you?
[00:45] Who are you? >> I am Laura.
[00:48] I have to get used to my new spiel because it used to be, I am a technical writer.
[00:55] However, I am now a developer advocate, which I'm very excited about.
[00:59] I work for Suborbital Software Systems and WebAssembly and Extensibility Spaces.
[01:06] People can find me. I exist on Twitter.
[01:09] However, I don't maintain a presence on Twitter anymore. But I am on Mastodon,
[01:19] and I think I've got my handle. Do I have my handle showing?
[01:22] Yes, I do. My handle is in my username. She still gets tagged on everything on Twitter,
[01:35] just so that way people know who she is. Even though I know she doesn't use it, and that's okay.
[01:41] I will eventually have my elevator pitch. I'm still working on trying it out.
[01:47] Although, I did come up with a graphic yesterday for the end of Vue School,
[01:58] and I was like, it's close. Vue School, Vue Nation.
[02:04] For those just joining us, I hosted the last two days at Vue Nation,
[02:12] which is for Vue. That's us. Just kidding.
[02:18] You would think that I'd be like, figure this out because I was doing this all day yesterday.
[02:23] Share screen. What screen am I going to? This one. There we go.
[02:28] Look, it has projects and it has contact me. I guess instead of thank you,
[02:34] I could just be like, yo, hire me for DevRel community. But then I don't have mental health on here.
[02:41] I don't know. I need to figure out how to talk about myself. Are you looking for like a one,
[02:49] like Jen in a single frame, kind of? Like, who is Jen?
[02:54] Because I don't know how to describe it. Every time somebody asks me, they're like, what do you do?
[02:58] And I'm like, I don't know, but I need a job. It doesn't work out well, but Bakari,
[03:08] I heard that you guys had coffee or food or whatever for like two hours. I'm so jealous.
[03:13] Yeah, we did. And that you have to send me these pictures because it's like Bakari going
[03:21] to where I want to go and hanging out with people I want to hang out with. Yeah,
[03:26] I can find the picture. Give me a sec.
[03:29] I saw it on the Twitters. Yeah, and I put it on Mastodon.
[03:39] Here we go. Share my screen or everyone can move to Denver Bakari.
[03:46] I'm just saying. Well, you, Jay, homie.
[03:56] Are all in California, just different. Areas in California.
[04:04] There it is. We are super fun.
[04:09] Yeah. Yeah, I love it.
[04:13] Good sandwich, too. Nice.
[04:16] Oh, we're inception mode. Yeah. All right.
[04:19] So to keep us on track, because this is our keep on track. Yeah, we created an entire extra stream to contain everything else.
[04:33] Yes, yes. All right.
[04:36] So we are learning how to automate boring stuff with Python. And I have learned since Laura and I started doing this many, many months ago.
[04:49] Quick learning recap one. I it's really hard for me to read something in general.
[04:59] I knew that I'm dyslexic on this type of content, reading it on the screen and not having somewhere to put the notes by it.
[05:08] Even if I type by it doesn't make sense to me. So I have a physical book.
[05:13] Other things I've learned is just my own learning styles, how to learn, how to retain knowledge.
[05:23] Keep going, if I don't understand it, don't get stuck and give up. And try to think of anything else.
[05:30] There are flash cards like Anki, Anki, is that how you say it? I think so, I would say Anki.
[05:39] I don't know. I think I've also heard Anki. Anki, OK, I don't know, Anki, like
[05:45] the Egyptian. Symbol, I guess, but that's spelled differently, so cool, cool, cool.
[05:52] Really quick, I think you are frozen. I am totally frozen, why is that?
[05:58] I don't know, but it's kind of you freeze me, Jen. Serious face like, bam.
[06:05] Oh, I'm still frozen, that's fun, I'm still frozen. Yay, take that with me.
[06:11] All right, well, why don't we just we just carry on and I will be trying, I'm going to stop my camera while I try to fix my camera.
[06:20] Sweet. Yes, Ian, we are learning Python.
[06:25] And so a lot of it came to I've been since starting to Gen Tech about six, seven months ago.
[06:34] I've learned that it's a lot easier for me to I guess I'm really good at being handed
[06:42] a really big project and going, hey, figure this out based on something else. And it's like a puzzle.
[06:48] I'm like, yeah, I got that. Yet what I don't quite understand and have had to struggle on is the basics.
[06:55] So I do a lot in JavaScript already. I do a lot of React
[07:02] hosting and doing work with Vue JavaScript, Vue.js, Nuxt.js TypeScript.
[07:12] There's a lot of there's a lot of JavaScript in my world. Yet I'm also learning Python because the way that I've gone after.
[07:22] JavaScript is how I just said of this, like, hey, take this really big idea and see if you can push it together and figure
[07:28] it out and the way that I am learning Python is from the exact opposite of we're going to do the bare basics and figure it out.
[07:39] So we are going to screen share the because this is available online for free.
[07:47] So we are going to go over the parts that I am stuck on.
[07:54] And a lot of it is just the bare basics. And they're more of concepts than necessarily
[08:03] the actual code itself.
[08:07] And I don't know if Laura is still here or if she disappeared on us. I think she disappeared on us.
[08:16] That's okay, because I am going to figure this out. And another reason, in case I didn't say this, is I got the book.
[08:27] So that way I can take notes in the margins.
[08:32] So I actually listen to it with a screen reader or a text to speech.
[08:41] And then I'm reading it at the same time. So I can pause the screen reader and write my notes or go back a few times.
[08:49] And that's helped a ton because I'm visualizing it while I'm hearing it, where me reading out loud, if anybody wants to see something really funny,
[09:01] I have decided that the speaker is some few nation who wanted to have the most syllables ever in their titles.
[09:10] So it was really fun. And I don't think I messed up too many of them.
[09:16] So, yeah, it's all practice and Laura's back. Yay. I'm back.
[09:21] Yeah. Rude of your camera to freeze.
[09:25] I know. But, yes, so this is the Teach Jen Tech Show and it's teaching Jen Python.
[09:35] Yeah, we are going to stream it to Laura's as well because Laura's teaching it and it's true.
[09:41] The mastery. And we're twinning today. We are.
[09:46] I was getting ready and I slapped on some red lipstick, which I never do because I was like, oh, because Jen usually wears red lipstick and then we'll match.
[09:55] And then Jen was not wearing red lipstick. And Jen said, hey, I like your red lipstick.
[09:58] And I was like, yeah, it was going to be this thing. So Jen ran and put on red lipstick.
[10:02] So we're the glasses and red lipstick folks today. Yes. Yes.
[10:07] Agreed. Agreed. All right. So.
[10:11] Because that is one thing people should learn about me is I just love lipstick. Like, it's the easiest thing.
[10:17] Like, you don't have to do the rest of your makeup and we'll still get put together. This is like an old boss told me that when she's like, because I was in person sales.
[10:26] So like your the way you looked did influence more. I don't want to say that it was like necessary, but it did influence more.
[10:34] So she was like, yeah, just throw on lipstick. People will be like, you look more put together if you do what?
[10:40] At first, I was really scared and then I was like, oh, no, I love lipstick. This is like this is life right here.
[10:47] So lipstick goes with anything, y'all. I don't care who you are.
[10:51] You can wear it no matter where you are, who you are, what you want to go to. Doctors may make you remove it for doctor's
[10:59] appointments, but other than that, you know. All right, so a quick run through before I go to chapter one is I can make this even
[11:12] bigger, yay, is automate the boring stuff. And with Al Swigert, is that how we decided his name is said?
[11:23] I think it's maybe Gert like Swigert, Swigert, Swigert. And he wrote, I have the second edition, I have the second edition.
[11:35] There might be many more editions out there. So we we just kind of roll with it and hopefully it works.
[11:43] It is all on Python three. So we don't talk about Python two very much.
[11:48] And this first part of it just goes through a lot of like you can be a total noob. This is to get some basic commands going so you can understand programming enough.
[12:02] And. That's it.
[12:06] So it's definitely oh, yes, let me see if I can do a shout out. Shout out at Al Swigert, Swigert, I don't know if this is going to work.
[12:28] Maybe I think it did, I don't know, but you got a shout out on my channel. And if we keep going down, I really like this because in the book and this is
[12:41] something that I think the book has that is a little. Easier when doing the text to speech is during the introduction, it also went
[12:53] through it might be in the introduction chapter, let's click it probably is. Oh, it is, yeah, it breaks down what all the chapters are for.
[13:03] So I'm going to keep scrolling down, keep going. Yay, let's go.
[13:10] I think it's super awesome of of Al to make this available for free. And if you can buy the book,
[13:18] you should buy the book to support Al's awesome work. But yeah, that's that's an excellent contribution to the community.
[13:27] It is it is and it's something that has made it so much easier to learn at the same time, even like not everyone may be able to buy the book,
[13:38] but they can also use the website to be able to read this. So I do want to go through just the layout of the book.
[13:48] It's part one is programming basics. I'm pretty excited about all of this because I'm still stuck on Python basics.
[13:59] So and then part two is automating tasks. We're actually going to get into creating more
[14:08] projects and if I keep going to do that might be it. Yeah, that's it. I'm really excited for chapter 18.
[14:16] Like getting to chapter 18 is what's going to keep me going. Which I'm guessing I'll probably jump ahead, see if I can figure it out.
[14:25] Knowing me, that's what I would normally do. But we're working on learning from the beginning.
[14:33] So let me go back to chapter. One.
[14:41] And for this, I will link it again, it is also on the repo that was created for this stream, so let me grab that, too.
[14:54] Because we have it where if you're wanting to do follow with us, review every week, read your chapter
[15:06] beforehand with us, you are welcome and we'll be here to ask questions. Well, I did that.
[15:13] Oh, it just shows a window because that's weird. What up, Jay?
[15:22] Hey, Jay. Jay is joining us from the YouTubes.
[15:29] Oh, I don't know why I say the YouTubes or the Twitter or the TikTok.
[15:36] I think it's just showing my age. I'm not I was going to say, I think it's
[15:42] because you're a millennial, because how do I know that? I am a millennial and it was all about the like 10 years ago, maybe 12 years ago.
[15:52] It was all about the. Oh,
[15:55] yeah, I think it was like, oh, no, it's longer ago. It was like two thousand eight.
[15:59] OK. I was hoping it was because I'm an old lady,
[16:05] at least my one year old grandmother calls me an old lady. So I'm going with it.
[16:10] She's been calling me an old lady since I was. Twenty five.
[16:18] OK, so
[16:22] I'm convinced, but, you know, at the same time, all right. So really quick.
[16:28] Well, what did I do? Yeah, yes, yes.
[16:32] OK, cool. It did come over here. We do have this repo where I will put all of our projects if we can.
[16:39] And also it will have all of the links and I will add in the things that I got stuck on down here after the stream every week and some lessons learned.
[16:49] So if you want to stay up to date, know what to read in the future, hang out here. It will be where you can be up to date on everything.
[16:59] All right. On to Python basics
[17:04] and I need to find chapter one because I'm going off of my book to ask questions because that's where I wrote them.
[17:14] Oh, the first thing that I don't want to ask about. Oh, actually, there's one right before it.
[17:23] I know we're not doing this in a IDE right now, but do you have to write out the greater thans
[17:35] or is that just here to show the difference? It's more like.
[17:42] Pop open a terminal. Jay says no.
[17:53] I know. But it's harder to remember, like for my brain anyway,
[17:59] it's harder to remember if you if you don't know why something is the case. It's harder to remember what the answer is.
[18:08] So it's it's more like. Yeah, so I think you've you've changed your
[18:16] your terminal because if you opened like the default terminal, like not hyper, it's just like the the terminal, like if you go into like systems,
[18:25] utility terminal. Or that I don't know where anything is, I just search it all the time.
[18:35] Oh, OK. Well, anyway, see that that like percentage sign?
[18:41] It's the same idea. It's like a prompt. It's like a type here.
[18:48] So that's why if you look at the page again. Back where you type there are the
[18:59] carrots, the right facing carrots as like this is where you type and then where the computer prints it back, it's there's there are no carrots.
[19:10] There's no prompt. Oh, I'm digging what everybody's saying.
[19:15] It's all bits is saying the terminal gives you. I guess this term is carrots, which I'm going to definitely be
[19:21] writing down to show readiness for your typed command. And yes, it is prompt.
[19:26] I wouldn't have thought of that either. And then Jay's question, have I used Jupyter Notebook?
[19:34] No, no, we have not. She has used her rebel in like the new
[19:43] ID, but not actually in a Jupyter Notebook. We haven't gotten there yet.
[19:48] And I'm the book does suggest using you and I do want to say this for everyone there, I'm doing things a little differently on that aspect because I use
[19:58] VSCode for everything I want to learn with VSCode. Yeah, yeah, and that's why because we had
[20:07] talked about this, like maybe we would just switch to a Jupyter Notebook or but you wanted to do it in VSCode so that it was more like.
[20:16] The way that it would be if you were. Building a project for a job.
[20:22] Oh, oh, and then you use. Yes, yes, code does support notebooks.
[20:29] Yeah, so that's it. Oh, I remember Jay was on the stream a while ago.
[20:36] I learned a lot from that stream of. Like all of the customizations and VSCode,
[20:45] and we got my VSCode set up and it's pretty now. So that actually makes a lot of sense on.
[20:56] Let me grab this. Link and send it to everybody so that way.
[21:07] Oh, I need to definitely keep this tab open. I am learning how to use Arc browser in
[21:18] case anybody is wondering why I'm taking so long to do anything. I'm like, I don't know what I'm doing.
[21:25] While you work on that, I want to shout out that Jay is going to be on my stream with me for my company a week from today.
[21:36] This time next week, Jay and I will be streaming. I don't have I'm working on the graphic that's going to happen later today.
[21:42] And then then I'll have a link because I have to have the graphic in order to make the create the thingy and all that stuff.
[21:50] Jay's remark, reply, yes, please email Jay. Yep, will do.
[21:54] And OK, here is the link that Jay posted for all the other channels of VSCode that I have up here.
[22:02] So I will please give me a moment because I am going to take notes really quick and make sure because a big reason that I'm wanting to do live learning and showing
[22:16] that I'm taking these notes is because I feel like I never knew how to study. I never knew how to learn.
[22:24] So that's. That sounds weird saying that out loud,
[22:28] but like if I couldn't figure it out, I didn't necessarily know how to go after it. They don't teach it.
[22:34] They don't teach how to learn in school, which is. Wild, so it should be an ongoing.
[22:42] Yeah, yeah. And and these are things that if you do
[22:46] look at when Laura and I first started kind of going through all of these, it took quite a while to get to this point.
[22:56] This is another reason we started this Monday. And it's been a big journey of just learning how to learn.
[23:03] And so I'm please give me a moment. So.
[23:10] It's. Is.
[23:20] It. Correct.
[23:24] Precinct, that's a percentage percentage in terminal. I'm a pencil.
[23:38] And. She.
[23:44] No, look. It's.
[23:52] Yes, OK, so in my I really should set up my phone so that way I can just show this as well and as I'm writing notes, but basically.
[24:07] We'll do that for next dream, random other notes that are added and it may not make sense to anyone else,
[24:14] but it makes enough sense to me that I know those are called carrots. And that it is the prompt like percentage sign in terminal.
[24:23] And then also V.S. Code works, Jupiter works with V.S. Code, so very exciting things to do.
[24:33] I also called pointy back brackets. And it's actually it's a different spelling.
[24:41] It's not carrot like the vegetable, it's carrot like a diamond. C.A.R.E.T.
[24:51] It sort of works both ways, right, because carrots are pointy. I was going to say, but it's actually right.
[24:57] Yeah, so it works both ways. But if you were to the only reason I mention it is because if you were to search
[25:05] for it, it will get there faster if you know the correct spelling. And I appreciate that because that is definitely something.
[25:15] Y'all. Language,
[25:18] it's a thing. I wish they were carrots, that would be an awesome book.
[25:26] I like that. I feel like, Jay, you now know the title of your book that you will write one day.
[25:35] You're you're like coding Python for babies, but Jay, it should have should have carrot brackets for sure.
[25:46] I just announced that Jay is writing a Python for babies book, and obviously I do not, in fact, dictate what Jay has to do.
[25:58] See, that is a great way of remembering it. Oh, that's so cute.
[26:05] OK, I really want I want Jay's Python for babies book. This is cracking me up.
[26:12] Actually, I like that you have it in quotes because that is like for anybody that may be new to this, this this world of actually is a way that
[26:28] people get into fights on social media of like, actually. So I love that it's in the quotes and like
[26:35] it's carrot points upwards and the angle brackets point left to right. It's true.
[26:42] Carrot without a modifier is the like exponent sign. It's on like six or something.
[26:48] But like in my computer science classes back in the day,
[26:56] they were referred to as left brackets and or like left carrot and right carrot. We didn't call them angle brackets.
[27:02] That's like a term that I've been hearing recently, but we didn't we didn't call them angle brackets or pointy brackets.
[27:07] It was left carrot and right carrot. All of these things, of course, all make a ton of sense and are all good.
[27:17] Also, just want to point out the fact that I am. Yes, and they also said that's the close off in it.
[27:26] They do. Oh, yeah, they make it a funny thing. They make it a funny thing.
[27:33] What? Stop letting me.
[27:36] I think it's distract. Yeah, but I like this better because it made me think of a cat.
[27:42] And yesterday during View Nation, Paige was on and. Anyway, I was going to say, I really appreciate that.
[27:52] It's all but said that it is carrot spelt like this because this is what Laura said as well, but I wrote it with a K.
[28:04] And this is about learning, it's like Laura said it, Laura spelt it right. Didn't realize that I wrote it wrong until I saw it and went, that is not how I did it.
[28:18] All right. Oh, geez, I've never heard of Octothorpe and I love it.
[28:24] What is an Octothorpe? I think it's the same.
[28:27] It's like this symbol has all these different names. Oh.
[28:33] Octothorpe. Octothorpe.
[28:39] All right, I'm this is why we get distracted. It is.
[28:45] OK, everybody needs to make sure that they're here on Mondays because we do learning Python every other week, but we do miss Mondays.
[28:54] I think that we need we like when we start feeling like we need to talk about something else, I'm just going to put it on a list.
[29:01] Yes, it's Monday. OK, so please put Octothorpe.
[29:05] I am putting Octothorpe. Thank you. Thank you.
[29:08] OK, so let's go back here. Let me go to my next thing of what I don't know.
[29:14] Oh, it's this it is this I actually have
[29:22] the operations in a question later on as well of like. How do you remember these?
[29:31] Because math and I not the greatest, which you don't need to know math.
[29:38] We have a full like probably two episodes not needing to know math program yet.
[29:44] I will say. It may help in if you already understand
[29:52] some of these concepts and symbols. I do think that would help, but it's not necessarily something you need.
[30:01] That being said, how if I were like looking at this because I'm going through it and I'm like, OK,
[30:09] cool, like I get all of these, but just like when we did the quiz way back in the day, I was like, I don't actually remember them.
[30:18] The same with like when we went through gosh, see, I don't even remember what they're called now.
[30:26] Data types. I'm like, cool, I probably would have eventually figured that out,
[30:31] but I don't remember actually what they're called. So like, do you have any tips or tricks on how to remember these?
[30:40] Just the flashcards, you think, or is there another way that people use to do them?
[30:45] The. So spaced repetition is going to be well, so I would say two things.
[30:55] Three things. OK, one is spaced repetition and Anki, that's what Anki is all about.
[31:03] That's not those are the digital flashcards you can you can do. You can do
[31:09] spaced repetition without flashcards. I mean, you can do it sort of however you want.
[31:14] Some people keep like a notebook and and review review that way.
[31:20] And then another thing is to actually understand because to a certain degree, I think, especially like in terms of these, they they make sense, I think.
[31:36] Like the well, OK, I'll get to the third thing. The third thing is to make up something.
[31:42] Sometimes people use colors. That's actually a big thing in.
[31:47] Montessori is to use colors like for when they're teaching parts of speech, nouns are black circles, verbs are red triangles.
[31:57] And so you build like the kids start building sentences with actual shapes, not even words.
[32:04] And so it's like and then like when you're doing subject versus predicate, the subject has to have a noun and the predicate, you know, maybe it's a verb
[32:11] and whatever, uh, yeah. So like abstracting it into something else
[32:17] that makes sense, like shapes or colors or songs or all like whatever helps your brain.
[32:28] I feel like I'm missing you said that there were three. Yeah, so there's spaced repetition, OK?
[32:38] Actually, understanding why things are the way that they are, oh, the why? Yeah.
[32:44] OK, so on this one, I do I'm going to put it out, I do have add to.
[33:02] And key and key, however, we're going to say it, that's a flashcard thing. So I'm going to move over it.
[33:08] But I also put out the very end of how to remember things better. So we'll follow up on that next week.
[33:16] The the next bigger thing that makes sense. Oh, yes.
[33:21] Do you want to just go over like an overview of things that didn't make sense or do you want to talk about ways that I think we can make these make sense?
[33:30] So I think these make enough sense. I just wanted to make sure like these do make sense to me.
[33:39] I think it is going to be a lot. I really like the color idea.
[33:43] And that's actually something that I was very annoyed with, with using pencil in the book is I can't.
[33:50] Look at it quickly and know I'm bouncing from ideas because I actually do that a lot of times when I'm taking notes is I use
[33:59] very many different pens because even if. They're not necessarily associated with a certain thing,
[34:08] I can at least tell that it's different than the thing next to it. Right, so they make really good erasable colored pencils now.
[34:17] Do they? Yes. Oh, I need that in my life.
[34:21] All right. All right. I'm just going to write that down. No, not.
[34:25] We'll see. We'll see if I remember that one. But the going off of that, like I'm going
[34:30] through this and I'm like, this all totally makes sense. Except till we get to here,
[34:37] the breakdown of. Visualizing it from a.
[34:47] Mathematical point of view, is that a word of operations, order of operations, and I guess.
[34:53] Oh, when you say it out loud like that, it totally makes more sense.
[34:59] Mm hmm. Yeah. So these these parentheses, they tell you what to do first.
[35:05] Right, and so first we have to we don't we have to we have to find out what five minus one is before we can do anything else with it.
[35:13] Yep, and the seven plus one and the three minus one. So that's so first we go through and five minus one, that's four and so on and so on.
[35:22] This totally makes way more sense now. I think just as like learning that and I'm
[35:29] saying this out loud by myself that it was hard is these all kind of do. They do point out more, but it also doesn't say like step one,
[35:39] just do this one, like as next to it, like as an explanation of like what line one is doing while line one is doing it.
[35:47] Yes, other people can associate it by understanding the context. That's not always something that I do.
[35:54] But now that you're like. You said it like, oh, yeah, that totally does.
[36:00] Yeah, yeah. So like right above, it says Python will
[36:02] keep evaluating parts of the expression until it becomes a single value. And I think that's what is being illustrated here.
[36:09] Yeah, but that's not something that like my language went to. So and Jay, what is?
[36:21] PEMDAS, Parentheses, Exponents, Multiplication, Division, Addition, Subtraction, which is the American
[36:31] mnemonic for order of operations. As a math instructor, I hated it because it reasonably suggests to students that
[36:45] you have to do multiplication before division and addition before subtraction, which is not true.
[36:51] Multiplication and division are in the same hierarchy, like they're in the same they're on the same level in the hierarchy,
[36:59] and so are addition and subtraction. And so the way that I would teach it is parentheses, exponents, dots, lines.
[37:09] So multiplication and division, those are dot operations. Addition and subtraction are line operations.
[37:19] Pedal, yeah, that's exactly it. That's exactly what I taught.
[37:23] I taught it, I started I came up with it for my because I homeschooled my older two, and so I came up with it for them.
[37:30] And then I was using it when I was. Teaching.
[37:34] Sweet, yeah, because I had tons of students who were trying to do multiplication before division and addition before
[37:41] subtraction, because that's literally what it says. I'm no joke.
[37:46] Like I've gotten in debates with people because I'm like, don't you do addition first or like one of the other ones?
[37:54] And I'm like, that's how you do it. And then you do them left to right.
[37:57] They're like, no, no, you don't. This is the entire source of all of those.
[38:02] Nobody, you know, 85 percent of people get this math problem wrong or whatever. Why? Because we lie to our students with PEMDAS.
[38:10] That's why. OK, OK, I'm glad I brought it up.
[38:16] Cool, because I think that's something that and this is also. For ads, get paid.
[38:26] Oh, sorry, Jay, let me know if it gets too much. I can see if I can adjust it.
[38:32] I also don't know if I'm actually getting paid yet on it or not. That being said, if anybody knows of anyone hiring or need work done or need
[38:41] somebody to talk them through stuff, hire me as a coach, as sales, as customer service, as dev rel, as training, hire me.
[38:51] I really need a job. Just going to have that on repeat for everything.
[38:56] Anyway, cool,
[39:00] because I do have a lot of like, add to Anki stuff, um. You know, do you?
[39:11] Uh, there are questions around the integer floating point and string data types, specifically, it's.
[39:25] I'm looking for it on here to go to it. Of.
[39:36] This y'all next week, I am definitely going to set up the camera so you can see my book at the same time, because I can only imagine this is
[39:45] annoying because you're like, I don't know what she's looking at. The lap. Oh, yeah.
[39:54] Thank you, Jay. Is string connotation.
[40:04] And cat nation, can't cat nation, cat nation. Yeah.
[40:12] So. And for for those who are also learning with us, it can.
[40:33] Con job cat annotations. I dig it, um, is.
[40:44] Sometimes it's kind of hard to say, hey, I don't know what I don't know or I don't know why I don't understand it, which does help people trying to teach you things.
[40:53] So, um. Is it just saying and I think it's also
[41:02] just like a word that I haven't heard is when it joins two strings together. This is one thing I don't understand
[41:14] about tech is why do they have to give such complicated multisyllable words to something very simple?
[41:22] Join two strings together, concatenation is fewer syllables, it is fewer syllables.
[41:32] Actually explain what you're doing. It's a word that you also have to learn a definition for.
[41:37] It sort of does explain what you're doing, but you have to understand like. The word parts in Latin.
[41:47] Agreed. Where would you use this word in something
[41:54] else that somebody may actually already know and associate with? I mean.
[42:03] Yeah, so it always means to to. It's not just joining two things together,
[42:10] it's a little bit more specific, because if I say join. Alice with Bob say in terms of not not join in terms of programming,
[42:22] that's a thing, but also like just join in terms of like the English language. If I said join these two things together, it doesn't tell you
[42:29] the order in which like which one is on the left and which one is on the right. It's not actually specific.
[42:35] Right, OK. Whereas if you are concatenating.
[42:40] Something and something else, the something that you read first. Has to be on the left, like you read it from left to right,
[42:50] it's going to be concatenated in the same order. So like where if you when when we have the dictionary.
[43:04] Off of the Alice and Bob. I just really quick concatenation is a series of interconnected things.
[43:20] A syllable, not syllable, a word that replaces it would be series sequence, succession,
[43:28] chain, string, train, course, progression, nexus. We could have used nexus.
[43:36] I don't know. To what Jay said, we already use the word join and also programming is considered
[43:52] a science and comes from academia, which has a history of making things more complicated as a form of validation and gatekeeping.
[44:00] Not all educators, as we have. Laura.
[44:05] Optus wrote Jay's aggressive disdain for the education system. Jay now has two books coming out.
[44:15] We have one which is carrots. We need to write these ones down, Jay.
[44:21] Like, I am very much looking forward to Jay's books. But concatenation or concatenated is when something is joined from left to right.
[44:32] It does mean so here we have Alice plus Bob gets joined as Alice Bob. OK, it's not Bob Alice.
[44:40] OK, it's specifically Alice Bob. Jay saying why when when they could barely write a book.
[44:52] I would say, you know, we people will help you and get ghostwriters. You can use text to speech.
[45:03] There's more options. There's more.
[45:08] And also I would say for books, I don't think you really need to do it as a physical book to start, like as so many of us are making online
[45:20] content and there's transcription options, you can have it transcribe it to give a good basis of books or blogs or whatever you're writing.
[45:30] It does take time, though, and I'm not great at doing that. But this is making a lot more sense,
[45:36] especially now that I understand what can catenated means. OK, cool.
[45:49] I want to just say it's like we can't say you add these two things together because addition is commutative.
[45:58] Two plus three is the same as three plus five. But Alice, Bob is not the same as Bob Alice.
[46:10] Even though we're using the addition symbol. OK, so we're keeping it we're not making people learn a new symbol.
[46:32] We're using that plus sign and it's it's trying to draw an intuition about what plus means.
[46:40] But we can't just call it adding these things together because adding definitely does mean
[46:47] that addition is commutative. So.
[46:51] OK, I want to the notes are weird. Octothrope sounds like a supervillain name.
[47:05] What was the supervillain's name? If anybody see
[47:09] Spider-Man with all the other Spider-Mans, wasn't there a octopus type dude there? There's a Dr.
[47:16] Octopus in the Spider-Man stories. Maybe why didn't they call him Octothrope?
[47:27] Isn't often I think it's Octothrope Thorpe. Yeah, oh, yes, Dr.
[47:42] Otto Octavius. Right.
[47:47] All right, OK, go into the next one, go into the next one. And.
[47:54] Oh, yep, yep, OK, this one's a bit of a scroll, a bit of a scroll. Wait.
[48:16] OK, so I totally get. We are on the overriding.
[48:24] That's what we're looking at right now and assignment statements. So if I understand right, it just means
[48:34] that we can assign. Is it only a number to a word or can
[48:43] something be assigned to something of any thing? Uh, do you mean like this where it says spam equals 42?
[48:54] Could we instead say like 42 equals spam? That and could you say spam equals eggs?
[49:04] Yes, could you say 42 equals spam? No.
[49:11] OK, OK, because 42 is a number and it means 42.
[49:20] And you can't override what a number, the value of a number, that's a fixed.
[49:32] That's a no. So when you say we could write, do you want to pull up?
[49:43] Like an ID or any anything like a text editor or whatever? I don't like VS codes, can we change icon?
[49:54] Jay, you're here, can we change icon colors in? For VS code, is that possible?
[50:02] I don't know if it is, but for some reason it it's not the colors that I I always flip over it because I'm like, this isn't the color of everything else.
[50:13] It doesn't have like a dark mode. Random things I think about.
[50:20] Uh, the actual app icon, yes, but you can do that with any app. Oh.
[50:31] Interesting. I just want a new file.
[50:36] Give me a new file. New file, oh, I clicked the wrong thing.
[50:41] No wonder. Text file. Oh, look, I can start a new notebook.
[50:45] I'm clicking it. It asked, so I'm doing it.
[50:50] OK, so you asked if you could. Put spam equals eggs, and the answer is a yes, with like a caveat.
[51:09] Which is that you would need quotation marks around the eggs. OK, so, so, Sam, yeah.
[51:19] Equals eggs, but we'd have to do it as eggs. It's a string.
[51:29] So I guess it sort of depends on what your intention is, like if you want to say that because otherwise, without the quotation marks, eggs is a variable.
[51:38] So you're saying I've got a variable spam and I am assigning it the value of the variable eggs, but you don't already have
[51:46] a variable eggs declared, so it's like you said eggs equals 42. And then you said spam equals eggs.
[51:55] Then the value that would be stored in spam would be 42. Let's take it.
[52:03] So. I say spam
[52:12] equals 42. I did not need it to be in a string.
[52:20] Or quote, no, I mean, it can be if you want to assign it like the word, like the string version of 42.
[52:31] Where it's not actually a number, it's a string. OK, it's just those two characters,
[52:38] like the character for followed by the character to. Not the numerical value, 42.
[52:46] Can you comment that you can comment out the secret spam for the two in.
[52:58] How do you summarize that? I don't know. What are you trying to say here?
[53:09] That it's. Because the first one without the quote marks is still a variable.
[53:20] The put put put spam equals eggs without eggs in quotation marks, right? Put both have it with have a version of quotes and without.
[53:35] And I'm pretty sure y'all, because you might be wondering this, some languages do allow you to have it
[53:44] with a single quote or double quotes. And some people have it as what up, everyone from James.
[53:56] Why can I not say James's name today? James, the quick James is quick.
[54:02] Thank you. Thank you. Thank you.
[54:03] And to everybody joining, we are learning Python with. Automate the boring stuff.
[54:13] James, the rapid. Oh, I like that.
[54:19] I like that. So thank you. Thank you.
[54:23] And right now we are in chapter one, which are the bare basics. And I know that James is probably talking about something very, very technical.
[54:31] And I will have to say that it was cool because I used James's YouTube video to set up Hyper and that kind
[54:45] of stuff, which is very helpful. So thanks, James. And yes, Gary, thank you.
[54:52] Gary over at YouTube is saying that's a good book to get started with. And for those who don't know,
[54:59] Gary was my first guest on teach and tech many, many months ago when I couldn't tell the difference between HTML, CSS and JavaScript.
[55:08] So. There's been a lot of come so far.
[55:13] Yeah, yeah. Yeah, what up, James?
[55:19] We still need to get James on the show. Like for anybody that doesn't know who James is, how would I summarize how?
[55:27] James, how do you summarize yourself? I would say that Jay is a.
[55:36] Jay, James, damn, so many names today is a full time content creator, which in reality means full time educator.
[55:46] It's kind of what I think of it. Yes, you are all Jays, you are all Jays.
[55:54] Yeah, Jay, James, Jen. We're going to change your name now.
[56:02] I have a child named Jasper. Dude, that is such a cool name.
[56:08] Oh, have I never told you my kid's name before? No.
[56:11] Yeah, we talk about kids. Yeah, I know.
[56:14] Like about them. Anyway, for those who don't know, my name is Jen.
[56:20] I have this show called Teach Jen Tech. And as I said, we're learning Python right now.
[56:26] We do this every other Friday and on Mondays. Laura joins me and we do Misc Mondays
[56:34] where we literally just hang out and talk about the most random shit. And the reason we started that is because we meant to start doing
[56:42] automate the boring stuff and learn Python like six months ago. But then we realized we have a lot of random stuff to say.
[56:48] So to make us more concise, we had to start our own show weekly. So make sure to hit follow and hang out
[56:57] with us because I'm still a noob, yet at the same time, I also do complicated stuff. It's a very confusing thing when I don't know all of the basics.
[57:07] So that's what we're going over today. And thank you, James, for coming to hang out for a bit.
[57:11] And the raid. Enjoy your lunch.
[57:15] Yes, yes. All right.
[57:18] So the up to this, we've got. We are currently going over for those
[57:25] who just joined us assignment statements, and I think of what it was called. And squiggly lines under eggs.
[57:32] Yeah, it doesn't like it hover. Yeah, right. So what it's saying is eggs is not defined.
[57:37] So if you under hover. OK, so but it doesn't mind it when we
[57:44] have spam equals eggs where eggs is in quotation marks, because then what we're saying is spam is equal to this string, which is EGGS.
[57:55] If without the question marks, we're saying this variable spam gets assigned the value of the variable eggs, because without quotation marks,
[58:08] a string without quotation marks is a variable. Right, like spam has no quotation marks because it's a variable.
[58:21] Like if it's a word or something like you would normally think of as a string. Then it either if you want it to actually be a string, then it needs quotation
[58:35] marks, because if you don't put quotation marks on, it's a variable name. And that totally makes sense.
[58:42] And y'all for this stream, I don't have it set up, but I will in the future. I'm writing my notes in my book and nobody can see them.
[58:51] But by next time you will, I will set up another camera and we will have it here so you can see my notes at the same time
[58:59] of the random stuff I'm writing. Yeah. And so the reason that doesn't that's not a problem.
[59:04] So we'll notice, like, even though 42 doesn't have the first 42, the first line doesn't have quotation marks.
[59:11] That's OK, because 42 is a number and it knows what to do with 42. We don't have to define 42 for the
[59:20] computer because the computer knows what numbers are. Got it. Got it.
[59:25] And what up, Anthony? Welcome. Anthony says, oh, this is in case anybody wants to know.
[59:32] Anthony is my Internet big brother. He is the one who between him and Ramon convinced me to start my own stream.
[59:40] Wow. We're like, oh, geez, here. Yeah. All right.
[59:44] I'm going to be my first my first guest. This is exciting.
[59:51] So, yes, Friday Hangout. Yes, so we are this is making a lot more sense and also.
[60:02] About can we replace it? Oh, the next question was, can you
[60:09] replace it and overwrite it in the same file? And I feel like we just answered that
[60:14] because we've literally named spam if we get rid of this one three times. Yeah, and in fact, with the first with the one that you.
[60:30] Had the one that you deleted, that one would actually be OK. So if you go like take that first line
[60:36] where it's a spam equals the string eggs, change that to eggs equals five or whatever.
[60:43] Oh, OK, watch what happened. So delete, delete.
[60:52] Yeah. So it was unhappy with the word string, I mean, with with the string,
[60:58] with the word eggs, right up until you put that equal sign and it said, ah, OK, you're going to make it a variable.
[61:04] I can deal with that. Yeah, well, this is exciting and culminator.
[61:10] Oh, that's a fun name. Culminator just said
[61:14] that Python like the honey badger. Um, yeah.
[61:22] And so so now it's not see we can say spam equals eggs without the the thingy, the squiggly, because you did define the variable eggs.
[61:34] This makes sense. Yeah. And what we did was we we didn't just
[61:39] redefine spam, we didn't just define spam three times. We actually defined it in three different sort of ways,
[61:48] because the first one we say we're assigning spam to the value of another variable and the second time we're assigning to spam the value.
[61:58] That is the numerical numerical value 42. And then we're assigning it a string so you can do all three of those.
[62:05] You can assign a value, a variable to have the value of another variable. You can assign a variable to have the value of a number.
[62:11] You can assign the variable to have the value of a string. And there are also more, but these are the ones that we've talked about so far.
[62:20] Y'all, I'm just going to have to go back and just like clip that entire thing. I've decided that these small clips are
[62:27] what needs to go on like TikTok or something, because like these are the things that I think are harder for people to understand, because I'm like,
[62:35] leave it to me to like have to like go try to figure one of these out. And I will. But knowing what they actually mean, not always.
[62:44] So this is something special about a language like Python, which is what they call it, loosely typed or anyway, it's.
[62:57] You could you couldn't do that in a language that's strongly typed like C, you would with those languages, you have to declare like this variable is of this
[63:06] data type. You would type like if you wanted to give
[63:12] for spam to contain the number 42, then you would say like in spam equals like so. So spam has to be an integer or spam has to contain a string or that kind of thing.
[63:27] Python is not strongly typed, and so it will allow you to just change. You don't have to declare what type
[63:36] of what data type your variable will contain and you can change it. I feel like that makes it even more
[63:43] interesting that my other Friday show, when you're not hanging out, is a script. Exactly.
[63:50] You know, I'm going to extremes. That is that is great.
[63:56] And you got a good luck with the interview. I'm guessing it's to interview to hire people on your team.
[64:03] So, yay. And also, I don't know if Jay's still here.
[64:09] I don't know if Jay's still here. I'm meant to reply to Jay and was he said earlier to add more
[64:18] short keyboard shortcuts on. For VS code and stuff, and I'm like, yes, I still need to do that.
[64:25] I still need to do that. And I just feel like that's the reason Jay needs to come back on the show.
[64:36] Also. Oh.
[64:42] OK, let me find under print function. And function function.
[64:59] Scroll, scroll. Print function.
[65:08] I'm looking for the actual word. A value passed as a function is called an argument.
[65:32] And for some reason that doesn't make any sense to me. Yeah.
[65:44] Probably because we. Colloquially in English, we use argument to mean one very specific thing,
[65:56] which is like where you're having a debate and you're also mad about it. Yeah. You know, yeah.
[66:03] It's just it's just an older. Argument like, yeah, so if you if you like
[66:10] search for like definition of of argument, it's not inherent to the word argument that you're having a debate and you're mad
[66:18] about it, it's more like so we refer to an argument as like. A particular type of discussion that's being had between two people.
[66:28] Oh, oh, oh, but we do we use this word in English colloquially, you'd use it like this, like, OK, you are arguing that.
[66:40] The sky is blue. My argument is that the sky is not actually blue, it's just.
[66:50] Refracted lighter or whatever. Right, and so that's.
[66:56] Where you refer to what the other person is saying, their input to the discussion is their argument, your input to the discussion is your argument.
[67:08] Like we totally do that in English. We'll say that that's exactly what we're doing here.
[67:16] It's the input. OK.
[67:20] Let me let me noodle on this one for a minute. Mm hmm.
[67:32] The words you're saying make sense, like that is something that I've learned a lot about since this entire thing
[67:43] started is like words can make sense now going from like the what to how doesn't always, for example.
[67:54] So a value that is passed to a function is called an argument. So it's the input, it's the input to the function.
[68:05] So in the print hello world, the.
[68:13] Value is hello world and the input, so therefore. This entire thing is a function or an argument.
[68:27] Input and argument are synonyms here. Oh.
[68:38] So hello world would be an argument, got it to the print function.
[68:47] One. One.
[68:52] One. And just so everybody knows,
[69:23] I will take pictures of my notes and I'll put a new Markdown file in the repo created for this, so that way it's
[69:34] you know, documented and. Cole just asked his argument, not.
[69:46] Is oops, I think we just go, OK, I'll go. There is argument, not word in JavaScript, TypeScript worlds,
[69:58] something that just as like a call out is it totally could be like I can get things to work in JavaScript, like great.
[70:08] I can get things to to do magic. I can get APIs to work like it's phenomenal.
[70:15] I have no idea what anything is called at all. And so that's been a big process of learning with Laura on learning
[70:25] or learning Python for this one, because not knowing the terminology does make it so much harder to do the job when you're asking for help.
[70:36] I think being self-taught and I did a poll a while ago that, yes, I totally think almost everyone is self-taught about something
[70:46] in their coding career because you do you have to go figure things out.
[70:52] But it's this is something. So that way I'm learning more of the basics to catch up with what I'm already
[70:59] doing is probably the best way to say it. The idea of an argument to a function is
[71:07] older than programming because that's also what you do in math. So just like you'd have like F of X equals blah, blah, blah.
[71:15] That's a function whose name is F, whose argument is X. So a lot of things like Jay was saying
[71:35] earlier, a lot of stuff in programming, it comes from because programming arose from math, I mean, programming is, in fact, it's all math under the hood.
[71:49] Right. And so it arose from math.
[71:53] Often for the purposes of science, and so that's why so much of the framing comes from the way that mathematicians and scientists refer to things
[72:05] because that's where it came from. And I like your call out on this
[72:11] because Jay said earlier
[72:15] a lot of educators can I don't think that educators necessarily mean to do this, but they can gatekeep content or information because of not understanding
[72:28] this and also not knowing how to break it down for others. One of my like such a dope human I know,
[72:34] Benya, she is I like to call her my academic friend because she has like so many degrees she's taught in universities.
[72:44] She talks very. Academically, that's what I'm going to go
[72:49] with a lot of big words, and I'm just like, dude, I don't context. I can get what you're saying with context,
[72:55] but I need you to break it down like seven times. And that is a cool thing.
[72:59] I love this about her because she doesn't mind doing it and doesn't make me feel bad or anybody bad for doing it
[73:07] because, like, that's just the way she talks in the way she's learned and the way she does everything.
[73:12] So I totally get the whole gatekeeping idea. And I love that you do this as well as
[73:17] like helping people understand it and translate it because it is a translation and learning another language just as learning programming.
[73:25] So cool. That one made sense.
[73:30] So I know that we only have like ten more minutes, so.
[73:46] Going to go back up because I think I skipped over this because it made sense with the I'm going to go down to where I actually wrote it.
[73:56] It made sense to the actual, like, description of it when it came up, but then when it was actually used.
[74:07] Here, it did not make sense. Oh, Len makes sense to me, it's length.
[74:14] This didn't make sense, quite make sense. So it's a string and we talked about a string is just anything in quote.
[74:24] Check, OK, an integer is a number. It is specifically a.
[74:33] Number that does not require a decimal point. You might want to say, like, it's a whole number.
[74:50] The reason that I'm not is because officially in mathematics, whole numbers do not include negative numbers.
[74:59] And so but integers do. So integers expand the whole numbers.
[75:05] It's like then like in a Venn diagram, it's like a series of concentric circles that share the same center.
[75:17] OK, because con means with. And so that's like concatenate.
[75:21] It's like with blah, blah, you know. So, yeah.
[75:25] So in a really fun question, does whole number include zero? Yes, it does.
[75:31] Whole numbers include zero. So natural numbers are like one, two, three, four, five.
[75:36] Whole numbers are the natural numbers plus and also including zero. Integers expand those further because
[75:44] they include all of the all of the whole numbers, but their negative counterparts. And so on and so on.
[75:52] You don't have to know these terms to program, but that's just why I'm not referring to them as whole numbers, as integers, as whole numbers.
[76:00] I'm referring to them as numbers that don't require decimal points. That's why.
[76:05] Can they do negatives, though? Absolutely.
[76:09] Include negative numbers, zero. And I'm just going to put positive numbers.
[76:18] Exactly. No fractions because that's right. Oh, yeah. For anybody who doesn't know me,
[76:35] I forgot to include in my spiel that I used to be a math professor. Yes, yes.
[76:40] And that is this is a really good way.
[76:46] Thank you for explaining that, because this is something. And then if we get to it, because I know we got nine minutes, float.
[76:58] OK, so float is just the short version of floating point point. Floating point is the same as decimal point.
[77:10] It's the point. Yeah.
[77:13] So floating point numbers, those are numbers. That use decimals, decimal points.
[77:28] Oh, it's the same point. OK, just repeating it back, so integers
[77:40] are anything that do not have decimal or fractions and float. Is anything with fractions or decimals?
[77:50] I don't think you can do fractions, but I'm going to say it in there. Yeah.
[77:57] Oh, it's taking everything in me not to not to get into how the nitty gritty of how all these things work, but yeah, you can't you can assign.
[78:10] Like if you said spam equals three over four, it looks like you just what you typed says spam gets the value of three over four,
[78:21] which is a fraction, but it's going to be converted to a decimal. So it's not going to get stored as three over four.
[78:28] It's going to get stored as zero point seven five. OK,
[78:34] so float. Is.
[78:40] Yeah, and so culminator correctly says that to repeating fractions to non repeating
[78:56] fractions, so, yeah, so what what what culminator is is referring to is the fact that like so I chose three over four very carefully because three over four is
[79:08] actually equal to zero point seven five the end one over three is equal to zero point three repeating forever and computers can't actually deal with this
[79:19] repeats forever so they can only go out to. In this case, it would be 32 bits,
[79:27] and so it'll cut it off so it'll be like 32, you know, threes after the zero, which isn't enough threes because you can never have enough.
[79:37] So it's not actually equal to one third. It is merely close.
[79:45] We don't have to worry about that right now. Yeah, I was going to say, I'm cool.
[79:51] Yeah, yeah, totally what you just said. So this is making so much more sense.
[79:59] And makes this make a lot more sense. Well, let me go to this other one.
[80:11] Just to make sure I'm fact checking myself of. So in this example, spam equals input that just means that somebody had to type
[80:32] something back. That means that you're waiting for when this program runs.
[80:40] It will. Pause to wait for
[80:46] you to type something in.
[80:50] And it will wait forever until either you force it to stop or you provide it an input.
[81:00] OK, OK, cool. That makes sense.
[81:04] That makes sense. And.
[81:08] Thank you, I appreciate it. I got another subscription and y'all, I'm actually going to be working on.
[81:20] And hopefully this is news for you, Laura, that we will be using OBS on Monday and I will just be sending you a link to I'm going to be working on using Ping
[81:31] and we're going to try it out for you to test it out. OK, like this is all making way more sense.
[81:41] And got it done in an hour and a half compared to I think it tried taking us like three sessions last time just to get through part one.
[81:50] So this will be linked in the GitHub as well as will be on YouTube, which let me grab the GitHub again, which I can stop sharing.
[82:04] And join us every week or every other week we do this or every Monday if you want to hang out with us when we do that.
[82:13] Miss Mondays, because it's definitely something that. I feel like so many people could really use this information,
[82:24] but it's also like having fun, having so many people join the conversation because, yes, Laura is a teacher, has been a teacher.
[82:34] I feel like that's what a devil is all the time, but Laura may or may not help me
[82:43] format a technical document on her stream at some point. Yeah, whenever whenever you have one.
[82:52] Yes, yes, I will. The next one is I mean, it's a technical document, but it's more of a technical
[82:59] blog, it's definitely not a like tech or anything. So I'm not as worried about that one.
[83:03] But the next one, next one, actually. I have your scheduling link, I need to use it because, y'all,
[83:13] I have an interview next week, I'm very excited. I'm very, very excited because I need a job.
[83:18] If in case I don't say it enough, I need a job, y'all. And.
[83:22] It is for a Web3 company, but they're like, hey, do a presentation and it needs to be about something you're passionate about.
[83:33] That's a developer tool in Web2 or Web3. And I'm like, I've been building an Astro site, so I am going to talk about what I
[83:44] asked for help on and somebody told me I need to understand the code and understand the docs and didn't help.
[83:51] I was like, dude, that was not nice. And not helpful.
[83:56] So I am going to do my presentation on that. But to do that, I could use your help and I
[84:04] will get it done and we can dissect it live. Sounds good.
[84:10] Awesome. And thank you.
[84:14] Yeah, the Python community is. Greater than the JavaScript community.
[84:22] OK, cool. Me trying to work on my.
[84:26] Not going to lie, y'all, the first way I read that is the Python community is carrots JavaScript community.
[84:34] If you weren't there for that part of the conversation, just go back in time, watch the screen.
[84:42] But, yeah, I mean, I like both I like both communities and I like learning because I've also never been the type of person to just hang out in one community.
[84:52] Not I've never been great at that. I like learning both.
[84:58] It's been fun. It also helps me really understand the two languages better
[85:04] because they're not the same. So I'm like, oh, like when I found out what an idea is.
[85:10] Oh, if anybody doesn't know what the acronym.
[85:16] T.I.L. means. I tweeted it because.
[85:22] Today, I learned. What T.I.L. is.
[85:26] Oh, really? Fun.
[85:29] I tweeted that yesterday, I learned about it yesterday, though. I mean, Anthony, he said it and I was like, oh, I got to Google that shit.
[85:38] But thank you, everyone. Laura, anything you want to cover before next time?
[85:45] No, no, thanks for hanging out with us, y'all. Yeah.
[85:51] And we will see you all next week. Let me find someone for us to read to.
[86:00] Maybe it's this one. I don't know this trying to do like everything on.
[86:10] This new browser and I are learning, we will learn, we will get there. It'll be great.
[86:23] And culminator, thank you for the follow. And I hope to see you again next time,
[86:29] because on Mondays we talk about all the random stuff plus Python. I want to have a list Python on this Monday's.
[86:38] Just because it's I think this is kind of like to your
[86:44] coloring, like the color coding that you talked about is association, because I think Python, I think you and Jay.
[86:54] Oh, that's nice. Ian as well.
[86:57] I don't think of Ian as Python. I think of Ian as postman and API or interviews.
[87:04] So, oh, I figured out why Jay left. Jay streaming.
[87:12] Oh, we get to write Jay. You know, we're going to write Jay.
[87:14] This is going to be exciting. All right, now that I figured out who we're
[87:19] reading and wait, can we still somebody just read it. So where's my read button?
[87:24] There's my read button. And.
[87:29] The. Start, right.
[87:41] All right, y'all, we will see you later and enjoy the rest of your day, Friday and weekend, and we will see you on Monday.
[87:54] Bye. [BLANK_AUDIO]

