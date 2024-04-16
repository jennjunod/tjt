---
showLink: "https://www.youtube.com/watch?v=bDUDLmk3bp0"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "episode-11-of-teach-jenn-tech-learning-with-laura-about-python"
title: "Episode 11 of Teach Jenn Tech Learning with Laura about #Python"
publishDate: "2022-10-24"
coverImage: "https://i.ytimg.com/vi/bDUDLmk3bp0/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech, Learning with Laura.
[00:09] Is that like learning with Laura, Teach Gen Tech? >> Yeah.
[00:18] >> Welcome back to our Monday. Monday is a weekly mini-series.
[00:28] >> There was a book years ago called Tuesdays with Morrie. Yeah, so back story for y'all tuning in.
[00:41] Thank you for joining us. Jen and I were just talking off air about how this series has sort of,
[00:49] well, first of all, it wasn't going to be a series. The first day that we did this,
[00:53] it was going to be an episode and then it was like, "Oh, well, we could just keep going with this."
[00:57] Then, "Oh, actually, we could do it every week instead of every other week." It just keeps in beginning.
[01:03] We don't only talk about Python. We talk about learning theory and we've done some Git stuff,
[01:11] and we've done some command line stuff, and we've done just some background CS topics,
[01:21] and neurodiversity type topics, and all kinds of stuff.
[01:25] We're talking about how it's not strictly Python that we're talking about and trying to figure out how does naming work with all of this.
[01:36] >> Python's the overall, like how we came together and-
[01:42] >> Like a common thread. >> Yeah, it's the common thread.
[01:45] It has to do with everything, but we're not always talking about Python.
[01:51] I personally like learning with Laura because we do talk about ways to learn as well,
[02:00] because that is something I really struggled with, and also a big reason for today's topic as I've changed the topic.
[02:11] Yes, and hi, homie. What up? I agree.
[02:17] This is like, I just enjoy Mondays because I'm not dreading the stream. It's not like I ever dread them,
[02:23] but I'm like, it's comfortable. I know I'll push myself to learn,
[02:29] but it feels more like you're a co-host instead of just a guest. That's where I land on in my mind.
[02:41] >> Yeah. Sounds good to me. >> For everyone hanging out with us today,
[02:51] we're going to get to Anki because last week I promised, I did say I would do it. I totally didn't do it.
[03:00] I would set up my Anki account and get, and Anki is like flashcards to learn how to do things.
[03:09] This is a lot of where we talk about learning theory and how to learn, and these are habits and structures that I never set up in my life.
[03:21] I never knew, and I think this does have a lot to do with neurodiversities and learning. I'm learning how to learn for myself,
[03:28] and Laura is like a master at this, so that's why I like learning from her.
[03:35] But then I also worked on, like last week, Tuesday I got a stomach bug,
[03:41] then Wednesday I fell off of a chair. It's totally my own fault. It was very great.
[03:51] I laugh because people that have known me for years know that this is just what happens in my life.
[03:56] I am so clumsy, where I didn't realize that when I posted on Twitter about it,
[04:02] and everyone's like, "Oh my God, Jen, are you okay?" I'm like, "Yeah, this is just my luck.
[04:09] This is what happens." I'm fine. I'm just hanging around with a boot on.
[04:18] Then I really wanted to get this project made. I'm calling it Tweety Tag,
[04:26] and it's where I am working on getting it set up to, on Wednesdays, I host a Neurodiversity in Tech Twitter space.
[04:41] Again, the cool thing about learning live and doing things online is when people want to be a part of it,
[04:50] you just get to move with it, you evolve. It evolved, you pivot, you evolve,
[04:58] and so I didn't realize that everyone, I said at the very beginning,
[05:05] I was like, "Oh, DM me if you want me to tag you in the reminders, so you show up on Wednesdays."
[05:11] Well, I had no idea what the undertaking would be if we fast-forward three months afterwards.
[05:21] I'm going to work on explaining it to Laura, and showing her where I'm stuck just in general.
[05:27] I think it'd be cool to explain. Then we're going to get into Anki, because, yeah.
[05:33] Am I missing anything? >> I don't think so.
[05:38] >> Sweet. I hope everyone is having a lovely Monday and start of your week whatever what time it is in the world,
[05:47] because I feel like Mondays are just known to be dreaded, and I'm like, "Dude, I actually really like Mondays."
[05:55] But I think a lot of that has to do with Laura. >> You guys are killing me. I'm going to actually cry on screen sometime.
[06:03] It's going to be real. >> I mean, it might happen,
[06:08] it might happen, but that's it. Yeah, it's welcome to be real,
[06:12] and what up? Is it Grat-can? Cane? Grat-cane. Grat-cane.
[06:19] I think that's how you say it. Hello. Happy that you're here.
[06:25] We are going to do this. I'm going to open the project, and Laura,
[06:35] I started using my VS code more to update to GitHub. But I created my repo and are updating it as we go.
[06:48] >> Nice. >> There is progress,
[06:51] but it is cd s-c-p-o-d-w-e-t-t-a-g-m-n-c-o-d-s-p-a-c-e. Stupid VS code. That part's not working again,
[07:10] but I don't even know why it stopped working. That's okay. >> I do.
[07:16] >> Why? >> Actually, this is how we met, isn't it?
[07:21] >> Oh, yeah, it is. >> This is a jush thing, and we can fix it.
[07:31] >> Okay. Let me show you all of this, and then Enki, and then fix it.
[07:41] Because I feel like if we throw that in, I'm like, wait. I'm normally very adaptable,
[07:47] but for some reason that's just like screwing up my head right now. >> I understand.
[07:51] >> That is the cool thing with and y'all, just something I really do want to call out is,
[07:58] learning about yourself is a huge learning process, but being very open with it.
[08:04] Honestly, a lot of times Laura and I just get on this call and I'm like, "Hey, what do you think about doing this today?"
[08:11] We are both, I would say, very adaptable yet sometimes there is such a thing as over adaptability,
[08:20] or going too far where that's why I say, "Okay, hold on. I'm going to lose train of thought if I add in that as well."
[08:30] I say all that just to, y'all, you're not alone.
[08:33] This is all the weird things we do. >> We are both on the ADHD train.
[08:39] >> Yes. >> That is a good call out.
[08:44] >> The rabbit holes have rabbit holes around here? >> Yes.
[08:50] >> I'm going to do this because Homie's here and it reminds me of always making sure that I pull the current one because that caused a mess last time too,
[09:02] or throughout. All right. I'm going to show you my Mira board version first.
[09:11] Because what I manually do every week is I post the Twitter space, I put the same thread tweet here.
[09:29] It says the same thing. Then I go through and tag everyone that wants to be tagged. I forget people, I lose people.
[09:36] I also am like, "Dude, I forget to look at my DMs half the time,
[09:39] so my bad." My goal is if somebody enters their Twitter handle,
[09:46] and I enter this Twitter space information, I want it to combine it,
[09:51] and then auto-post all of this for me. Which in theory, I thought would be really cool.
[09:57] It's a lot more complicated than I imagined, which is cool because so far we have Prisma,
[10:07] which I'm going to look this up because I didn't know what Prisma was before this, and it makes it so I found out that I needed
[10:18] a back-end and a front-end tool to be able to make this happen. Front-end to be able to gain the content,
[10:26] make it look pretty, and then a back-end to be able to put it into the database,
[10:31] and then eventually connect to the Twitter API. Eventually, so there might be more in there, but I'm still learning.
[10:39] What I did is it created this Prisma database client to be able to read a database,
[10:57] and I created this database with Ivan, which does manage databases.
[11:02] So my end goal after all this is done is to see how that works on Ivan, because it's supposed to make it that you can just switch your databases
[11:12] without causing a conniption for the front-end people. So I'm going to leave it there,
[11:21] and then hopefully the Twitter API, I can get that to work.
[11:26] I was thinking I would test the Autopost and then do the front-end, and I realized that's not how my brain works.
[11:36] That happened, and then one part that I got really stuck on is I've worked in databases,
[11:49] but I've never built a database, and building the models and things,
[11:57] and that was really, thank you, homie, for coming on the stream for a little bit to help me through this,
[12:03] because it was easy for me to start writing this out, but actually creating the models.
[12:11] So I'm now going to go to my project. So if I look here,
[12:21] at first, when I created the Prisma, it created our scheme Prisma,
[12:32] which put in our data source, so that connected the database and the.ev file,
[12:37] and then we created our models for our database. >> Okay.
[12:44] >> Dope. Got it, got that far. Then I was like, "Oh, what do I do now?"
[12:49] I need to have a, we queried this, it was working, great.
[12:55] Then I needed to make a front-end, because I was like, "How am I going to test
[13:01] if people can actually put something in there?" I didn't know yet, so I was like, "I'll make a front-end."
[13:06] You did, homie, you did. Then if we go into pages in index,
[13:20] it will ask for your Twitter handle. So let me do cd node.
[13:31] Oh no, right, non-models? No, just kidding. Is it lscd to go back one?
[13:40] >> No. Remember last week we were talking about the dots, and how the dot always means the same thing.
[13:49] Dot means this directory that we're in right now. Dot dot is the directory that we are nested within.
[14:00] One directory from where we are. >> Like that's.
[14:07] >> Yes, and it always means that. Dot always means where we are,
[14:14] and dot dot always means one directory up from us. >> So if I do dot dot,
[14:19] will it take me to the directory above? >> Cd, so change directory,
[14:23] space, dot dot, means we go up one directory. >> Boom. Okay. That was really exciting, y'all. I don't know.
[14:32] Okay, come back. Thank you. Then I need to do cd next forms app,
[14:39] and then it is npm run dev. Yay. I don't know why I had to look that up so many times yesterday,
[14:51] but I can not remember it. But I've been also over since Thursday about this project by itself,
[14:58] I've streamed, I think like 15 hours, so I've been very stuck.
[15:04] Look, it made a thing, and it was very exciting.
[15:08] But if I do my name and I hit "Submit", I've even got this to work.
[15:14] Is this your Twitter handle? Yes. Yay. It's beautiful.
[15:20] I can open a new one, and we're in TweetyTag, perfect.
[15:28] Then I need to do node. I need to look up what the other one is.
[15:34] I put it in my notes. Node, node, node index JS.
[15:43] So if I do node index JS, delete all your things.
[15:50] It gives me a bunch of error messages. Yes, I need forums, I need index,
[15:58] and why am I in my Git ignore? I don't know. Then I need this index,
[16:09] and then go like this. So to query the database,
[16:15] if I'm in index.js, if I query Twitter handle,
[16:22] and I do my name, I think it was like this.
[16:28] Not to whatever. I think that's all my name.
[16:31] It doesn't really matter. I save it, and I query it.
[16:38] Look, it pulls it. But I can't get
[16:46] my Next Form app to go into the database. I don't know how to get
[16:57] the front end to talk to the back end, and this is where I'm stuck.
[17:01] But I just wanted to show you because I felt so cool doing all this. I was like, I'm really excited and feel
[17:08] like I'm a real coder, like I'm a developer, and this is crazy.
[17:15] >> Yeah, this is super cool. I'm trying to figure out what might be wrong.
[17:22] So I am not a web dev, right? >> Yeah, that's okay.
[17:26] >> I definitely don't know off the top of my head. >> There's TypeScript, and JavaScript,
[17:33] and an API, it's a hot mess. But it's getting there.
[17:41] It is getting there. But I was just really excited to show you that I actually, a lot of it was starting to make
[17:47] sense based on things that we've been talking about. Yes, we are talking different languages.
[17:58] So first off, I want to say that Laura and I have mainly been talking about Python. Everything I'm building is mostly with databases,
[18:07] and JavaScript, and TypeScript. This is just the way my brain works is I like to,
[18:15] why do I not have? Okay, sorry. What's the book we've been learning?
[18:26] >> Automate the Boring Stuff. >> Automate the Boring Stuff.com.
[18:31] For some reason, I bookmarked it. I don't know where I bookmarked it.
[18:35] As we're going through Automate the Boring Stuff, it's teaching about the way coding works in general.
[18:48] Not just Python stuff. This is the really cool thing is working with Laura has
[18:55] been learning how these different statements work together, how this all works because as we've been testing it out,
[19:04] or she lets me go off on a total tangent and like, "Oh, let me go to skip far ahead."
[19:10] It's also taught me how to use VS Code better and being able to understand what a property is,
[19:16] or being able to go in this as a function. Python will use very similar things.
[19:22] If you were to ask me right now, I'm going to totally space which does what,
[19:26] but it's similar enough that the concepts are starting to sink in, that are making learning both oddly,
[19:35] really a lot easier than if I feel like if I was stuck on one. Because if I get stuck on one,
[19:42] then I can go figure out more on the other. >> Yes.
[19:44] >> It might be the ADHD in me. >> Yeah. I think of it as an advantage.
[19:53] That is true. Oh, I need to call this out. It's time for dancing because it's progress,
[20:01] so I'm putting it on there and dance. Just had to get that out. We got the dance done.
[20:11] Yes. I just want to say that y'all helped me and I learned a lot so far. >> Yeah. Because all programming languages
[20:23] have a lot of the basic concepts in common, just like human languages have a lot of basic concepts in common.
[20:33] There are going to be verbs, there are going to be nouns and pronouns,
[20:37] and how do you express these kinds of ideas? The idea is the same and the syntax is different.
[20:45] Programming languages are exactly the same way. They're all going to have like for loops and while loops
[20:51] and Booleans and data types, and how do they handle data types
[20:58] and print statements and all of that kind of stuff. VS Code is going to say,
[21:03] you can hover over your function name, they're all going to have functions,
[21:06] so you can hover over your function name and see the declaration of this function.
[21:12] You can see what the function expects you to give it, and what it's going to give back to you should
[21:17] everything go correctly. All that stuff stays the same.
[21:22] >> That's just like something that I wish more people realized, because how to say it?
[21:32] I think people get really stuck on the scariness of learning another language,
[21:40] because it's like and I really feel it now where it's like, once you start learning your second language,
[21:50] it makes it easier for all the future languages. >> Exactly.
[21:54] >> Because you see the concepts are the same, you just need to change the syntax.
[21:58] >> Sometimes it helps you understand your first language better. >> Yes, and that's happened a lot too.
[22:05] That is definitely something that has taught me a lot, and that is a big reason I really just want to show you all of it,
[22:15] because I'm like, even though this is all Python, that you and I talk about,
[22:21] it really helped all of this, and that's probably why I was like,
[22:27] can we do the, what is it called? Anki? If we can do the Anki stuff,
[22:35] because I got stuck on it, and I think it's also like I've never seen it,
[22:43] like it's worked and I get it, but I don't get it. It's like this weird until you start to do it,
[22:51] you might not realize that you don't get it. >> Sure.
[22:55] >> Still, on that note, and let me reshare my screen.
[23:01] Wait, add stream. There we go. I can use StreamYard, it'll work.
[23:09] I got it. Anki, and we downloaded it. I downloaded it, so I just need to go look for it.
[23:24] Anki. Can we make you smaller? >> Thanks. Yes, we will.
[23:38] I have to re-download it? We'll go with the same one.
[23:44] >> This is because you're not downloading it from the Microsoft App Store.
[23:53] I mean, sometimes it can update itself, and sometimes you have to download a new version.
[24:01] I don't think that you can get it from the App Store, but I don't remember.
[24:06] I don't know if I've tried, I probably have not tried. Thank you, Ben.
[24:12] That's awfully sweet. >> All right. Are you saying that I need to do it right now then?
[24:20] >> No. >> Okay, cool.
[24:22] >> Just that you can. >> All right. If I remember correctly,
[24:27] decks are like if I want to do one on Python, and then I want to do one on Twitter,
[24:33] like decks can be about totally different subject. >> Sure, yep.
[24:38] >> Okay. I don't know. Maybe somebody would want to do it about Twitter. You never know.
[24:44] >> Yeah, I mean, I could see it. Twitter was a learning curve for me.
[24:51] >> It is a learning curve. >> When I joined.
[24:53] >> I love Twitter. >> Me too, and I will actually cry if we have to go because of fucking Musk.
[25:05] >> Yeah. >> Right? I'm on Mastodon and that's fine.
[25:11] But Twitter is like for all that people refer to it as like a hell site, and I totally understand why it is that for a lot of people.
[25:21] >> Yeah. >> For me, it is my safe, happy place.
[25:26] >> Agreed. I love Twitter. Tech Twitter has been such a good space that I've really grown into.
[25:39] It sounds weird, but because of Twitter, and I'm going to go back to us because this is a random shit we talk about,
[25:47] and thank you everybody for going on this ride with us. We need a special musical sound for like,
[25:55] here we are, we're just going to wax politic about Twitter for a minute. >> Yeah. I mean, we can do, let's see.
[26:01] I can do, we do have a little bit of music. Let's see. [MUSIC]
[26:08] >> There we go. I'm going to turn it down. This is our ode to Twitter.
[26:14] >> Tech Twitter itself, A, I didn't realize it was a thing,
[26:20] but it's been so amazing having people that I never would have been able to talk to. You and I would not be connected if it wasn't for Twitter,
[26:31] because I met Ramon on Twitter. >> I wouldn't have my job with.
[26:35] >> Yeah. Ramon is one of my- >> I wouldn't even know Ramon either.
[26:40] >> It's such a good space. Yes, there are some really big dum-dums there,
[26:45] and it's really fun to block people, and Twitter spaces have helped so much with my own learning experience,
[26:54] but also finding this community of people, of like-minded people that I don't know if I would have found,
[27:04] because a lot of developers aren't on LinkedIn. They hang out on Reddit, maybe Stack Overflow,
[27:14] but not everyone is, but there's a lot more developers and tech community on Twitter than any other platform.
[27:22] >> I always tell people who are talking about getting into how to get a tech job and so on, that hot take,
[27:31] Twitter is way more valuable than LinkedIn, and they're always astonished.
[27:36] They're like, "No way." >> Actually, yeah. I posted that I'm looking for a DevRel job,
[27:44] and a lot of the places I'm interviewing are because of that post, 100 percent. I think that I can't do this at the same time.
[28:02] Somebody else is looking at my project, and they're like, "What's wrong with it? It's fine."
[28:06] I'm like, "I can't get the front end and the back end to connect. It's not fine." Anyway, sorry, I can't.
[28:12] >> Yeah. >> Just a random other thing on Mac,
[28:17] if you put do not disturb and stuff, it doesn't do it for Discord,
[28:22] which I wish it did. >> It doesn't mean.
[28:26] >> Really? I still get notifications. >> You can change it in the focus settings.
[28:32] You can say which apps it needs to apply to. >> That totally makes more sense,
[28:39] because I'm like, Discord will hardcore distract me. I'm like, what?
[28:46] Okay. No, do not allow notifications. This is splendid.
[28:53] Well, at least, I think I got that figured out. I don't know. It's fine. All right.
[29:00] Back to, oh, we have so many more fun people that I didn't even see. Hack with Coding, what up?
[29:09] Didn't we talk about this yesterday? Do you want to come and hang out with us on Twitch?
[29:14] Because you're the only one on YouTube. Can you get Twitch where you're at?
[29:20] That's the other thing I always forget is, I don't know where.
[29:23] You're watching from Kenya, so I don't know if Kenya, anybody know?
[29:29] I think Kenya can do Twitch. >> I haven't heard that Twitch is blocked in Kenya.
[29:37] >> All right. Well, I got that posted. I posted to your channel too.
[29:43] Then we got, B1 mind is LinkedIn is sad. Your Twitter's not much better.
[29:56] Why is your Twitter not much better? What? You need more Twitter peoples?
[30:04] >> On the topic of people who are trying to get into tech, I actually have one of my blog post drafts,
[30:11] it's how to use Twitter to get embedded in the tech industry and use it to find a job. Now I'm wondering whether it's going to be moot now because
[30:22] maybe Twitter is like we're going to have an exodus from Twitter, super sad. But yeah, it's a total thing,
[30:31] figuring out how to get connected to people on Twitter. >> On that note, let's talk about a little bit,
[30:43] and this is for my own understanding too. Basically, the Rocket guy wanted to buy Twitter and Twitter was like, "Nah, brah."
[30:56] He's like, "Let me go do my own thing and create a new thing that's just going to take away from Twitter."
[31:02] >> Not really. He wanted to buy Twitter itself and he made an offer, it was like 44 billion or something,
[31:13] this is like in April, and it was agreed that he was going to buy it. However, lots of people speculated that
[31:21] he had no actual intention of buying Twitter at the time, he just wanted to throw his weight around.
[31:29] Then he started talking about how there were too many bots on Twitter, that if Twitter's value is in the number of accounts,
[31:38] and this is a massive oversimplification, but if Twitter's value is in the number of accounts,
[31:43] and this percentage of accounts is actually bots, not real people, then it's overvalued by that percent, say.
[31:51] He came up with a much larger percentage of bot accounts than was real. Then he said, "Yeah, so never mind.
[31:59] I don't want to buy Twitter because Twitter sucks. It's all bots." Then Twitter was like, "No,
[32:06] you can't do that because you just made up that it's all bots. We're going to sue you and say you have to buy us because
[32:15] you entered into an agreement to buy us, and the premise upon which you left was false.
[32:23] You still have to buy us." He was trying to not do it and trying to not do it,
[32:27] but he wasn't going to succeed. He got other people with more money than sense to help him do this.
[32:35] Now, it appears that it's going to go through unless the government says, "Hey, actually, you are too cozy with Russia,
[32:48] and this is too big of a thing to hand over to somebody who's cozy with Russia." It's against public interest for you to buy Twitter as a security problem,
[33:02] which is goofy when you think about it. But also, it makes sense because modern life, right?
[33:14] >> I almost feel like random shit and learning with Laura Mondays, like random stuff.
[33:25] But I'm bringing this back a little bit too because I don't want to skip over this one. Is Fordotus, I get really stuck on trying to figure out people's names.
[33:42] Note that in Stack Overflow, there are people with so much knowledge and most probably,
[33:48] the people on Twitter are searching on Stack Overflow first. I think if people know how to search things.
[33:57] >> I think we were more talking about finding humans, as opposed to answering specific questions.
[34:07] Certainly, if I have a question like, how do I do this get thing or whatever,
[34:15] I search for it, not necessarily on Stack Overflow itself,
[34:20] but I'll search for it in search engine. Then very often, the website that I end up finding the answer on is Stack Overflow, for sure.
[34:31] >> Interesting because granted, I've only started doing this new project that's been very,
[34:37] very technical, but I actually created something on Stack Overflow and nobody replied. I was like, I need this answer.
[34:46] I just started hitting up all my communities in Twitter and being like, someone, come help me.
[34:52] >> I have never asked a question on Stack Overflow. >> See, that deterred me from Stack Overflow,
[34:59] because I couldn't find the answer and nobody's replied to me yet. But I feel like that's forums in general.
[35:05] That's like if you ask a question in a Facebook group, not everybody's going to see it.
[35:11] I do find that very interesting. But yes, I agree with both.
[35:18] I feel like Twitter, you can have more of a community,
[35:20] but that could just be if I can't get Stack Overflow and I to be friends. >> I mean, it's not really what Stack Overflow is for.
[35:29] >> That's true. >> It's for answering very specific questions
[35:34] as opposed to forming those human connections. I'm sure that human connections have been formed on Stack Overflow,
[35:41] but that's not its purpose. That's not its reason for living.
[35:47] Whereas that totally is the reason for living for Twitter. >> News. Half the time I find out
[35:55] something because Twitter decided to notify me and I'm like, "Oh, hello." >> Right.
[35:58] >> Hello. Also, where did he go? Ryan, I saw that you're here too, so hello.
[36:07] >> Oh, hey, Ryan. >> Say hello. Hello yet?
[36:10] Hello. Wow, I can't talk. This is part of Monday.
[36:14] >> I just have to say one more thing in praise of Twitter, which is that watching the pandemic unfold from the perspective of
[36:24] somebody who was active on Twitter in the tech community at the time was wild. Because everything that was coming out through the news was like three or four weeks
[36:39] behind what was already known in a lot of like if you follow Dr. Eric Feigl-Deng on Twitter, he tweeted on February 5th,
[36:52] his classic Holy Mother of God tweet where it was about what was going on with COVID in China.
[36:58] That was right before it started getting everywhere else. I wasn't following him yet then,
[37:07] but people that I knew were, or not knew, but like Twitter knew.
[37:11] So I was talking about it with my parents, and my parents were in their 70s at the time,
[37:19] and most of the people who were dying at the time were old people. I remember telling my parents on March 11th,
[37:27] that we are trying to adapt our lifestyles in order to save your asses, and you are just like going about,
[37:37] you're going to Target and you're doing the whatever. Because Twitter knew about this,
[37:44] everything, weeks and weeks before, the CDC was saying anything.
[37:50] So it was really, really weird. Then it's ended up being that way still now,
[37:56] where according to the CDC itself, like the pandemic is over, there's no problem here,
[38:01] nothing to see, move on. - I do find that really interesting.
[38:06] I think also, so I didn't join Twitter until June. I had a Twitter account,
[38:16] but I didn't start posting until June, and it's just wild,
[38:24] the content and people you can learn from, and conversations you could just have.
[38:29] I don't know, it's like my favorite part, and I do feel like this ended up all about Twitter.
[38:34] But we're going to stop. No more acoustic music.
[38:42] I can't talk, it's cool. Fine. It's fine.
[38:46] All right. So we're going to talk about Anki. I'm going to leave this up over here,
[38:54] just in case we need Anki for any documentation or anything. I'm about to break the rule that you just set out right away,
[39:03] and say, "I'm pretty sure that I discovered Anki on Twitter." - What? Oh, did you?
[39:09] Oh, okay. You probably took me a minute. I was like, "What rule?"
[39:13] Oh. All right. I mean, that is pretty good. That is pretty good.
[39:19] I think that... Ryan, were you there last week on...
[39:27] Who was it that said that they use Anki? Was it Ryan?
[39:30] Ryan, how did you find Anki? I think it was Ryan.
[39:35] Okay. We're going to delete this one, because I didn't. All right. I have an Anki thing
[39:41] that does not let me make anything bigger, so please zoom in yourself.
[39:50] - Oh, yeah. I think it's in settings. In the Anki settings, you can make it bigger.
[39:58] Yeah. Preferences. Sorry. - I always just hate how it says that.
[40:04] Default. Oh, yes. We're going to make it giant.
[40:09] I'm also blind, so close. Oh. Restart. Okay.
[40:16] Quit. Start. No. Oh, it's so much bigger.
[40:25] Yay. Is that easier for everybody to read? Do I need to make it even bigger?
[40:32] - It was good for me before. I wouldn't need it to be any bigger,
[40:36] but I have a big screen, so hard to say. - Fair enough. Fair enough.
[40:42] All right. Fordotus got back to us about...
[40:47] Of course, Stack Overflow will be the first on Search Reflex, because Stack Overflow is community-based
[40:53] on coding questions and answers. Twitter, on the other hand, is social networking.
[40:58] Also, there is code review Stack Exchange. They do code reviews?
[41:08] Wait. What is Stack? All the knowledge. All the things.
[41:14] - I mean, it's certainly the case that you see, at least I've seen people post code on Stack Exchange,
[41:24] and other people have critiqued it, said like, "Oh, hey, this is how you can improve this code,"
[41:32] or, "You can make it more efficient. You can make it useless memory," or whatever.
[41:39] Maybe there's an official code review on Stack Exchange. If there is, this is the first I've heard.
[41:45] - But does that mean that in Stack Exchange, I could maybe ask someone and be like,
[41:50] "Yo, look at my Git project, and why can't I get the front end to talk to the back end?
[41:57] Please and thank you." - Very, yeah, for sure.
[42:01] Whether people answer, I don't... That feels...
[42:05] I guess if I were going to ask a question, like if I had...
[42:10] I have benefited from other people asking questions on Stack Overflow and then getting answers to them.
[42:16] - Yes. - I feel like a faster way for me
[42:25] to get an answer to a specific question is to ask a smaller, more connected community.
[42:35] Okay, and then to immediately contradict myself, then the other place that I would be more likely
[42:42] to ask a question is actually the free Code Camp Forum, which is not a small community,
[42:46] but it is super active. - Okay, that's as big as that one's gonna go.
[42:53] But I feel like these are things that we don't talk about. Like, I don't know, but...
[43:04] A Discord service, yeah. - Yeah, that's the other thing I was going to say,
[43:08] is like if I had a question that made... Like, we use something called Docusaurus at Suborbital
[43:21] for serving our... Well, not serving, but like formatting our docs.
[43:27] And I am part of the Docusaurus Discord so that if I have Docusaurus questions,
[43:33] I can ask on their Discord. So if you're having a question about Ivan,
[43:40] if Ivan has a Discord community, I would totally be hitting them up directly.
[43:48] - 'Cause I don't know if it's a Prisma or I think it's a Prisma question.
[43:53] - Okay. - But... - Community! - There you go.
[43:57] - Bam, okay. So if product on a...
[44:05] Wow, y'all, I can't type. Product/language-specific,
[44:16] see if they have a community. - Discord. - Mm-hmm.
[44:24] - Slack forum. - If must, yeah.
[44:30] - To ask. - Mm-hmm. - And then you said...
[44:35] - CodeCamp would be the next one. If I had had more of a general question,
[44:40] Free CodeCamp would absolutely be where I'd be going. - All right.
[44:48] - There was a time, and I know that Stack Overflow has really tried to fix this,
[44:56] but there was a time when Stack Overflow, like asking a question on Stack Overflow was like,
[45:03] yes, you would maybe get an answer, but people would be really horrible to you first.
[45:09] - I've heard that. I've heard that. - Yeah, yeah.
[45:12] I'm trying to remember. I think it's Meg Rizdal,
[45:17] and you can find her on Twitter. Sorry to break the rule again.
[45:19] Took over at, well, not like CEO of Stack Overflow, I don't think, but she was an uppity-up,
[45:31] and that was one of her big foci was making Stack Overflow be a friendly place
[45:38] where you could ask questions instead of, "We'll answer your question,
[45:44] but we'll, you know, like tie you to the whipping post first." - Why can I not make inferences?
[45:56] Text size, giant, 'cause I am blind. And honestly, I'm not just doing it for y'all.
[46:03] I'm doing it for myself, too. Okay, let me catch up on comments really quick
[46:09] to see if y'all put anything else in here. I'm gonna mention Discord servers, and then...
[46:17] Yes, yes, 100%. Great, Gratcane about, like,
[46:27] how some communities are negative. Okay, so Stack Overflow will, say, keep questions short
[46:42] and may have... I wonder what the turnaround time is.
[46:52] - For getting questions answered on Stack Overflow? - Yeah.
[46:58] - I don't know. - Okay, what is Stack Exchange, then?
[47:06] And I'm doing these without the research just because I want to see what the community
[47:10] actually uses it as. So you and I talked about, like, you can...
[47:18] Not maybe, like, a proper code review, but a, like, just a code efficiency.
[47:32] I don't know if that's the word I'm looking for. Hmm.
[47:42] I'm gonna throw a link in for Meg's post about Stack Overflow just because I thought
[47:50] it was really interesting to hear from someone on the inside who was really, really working on that problem.
[48:07] It's sweet. Okay.
[48:35] Okay, let me put hers in here. Will you DM that or private chat that to me, too,
[48:42] because that one went on your Twitch channel? 'Cause we do stream to both, y'all, as a heads up.
[48:48] We stream to my Twitch channel and Laura's Twitch channel, which y'all should definitely go follow Laura, too.
[48:57] She needs--we all need the followers. If she's doing something, y'all can still catch it.
[49:11] And hers is gogadget. Oh, okay, so I'm just gonna have to throw this in here.
[49:24] So my usernames on most places is some variation of gogogadget from inspectorgadget, of course.
[49:32] And I don't know if everyone who does not have children knows that there's a reboot of inspectorgadget on Netflix.
[49:40] And it's actually really good. They've changed some things, but they've changed some things
[49:44] in some ways that I approve of. And my five-year-old likes to watch Netflix
[49:51] with the narration on where it, like, describes what's happening on the screen.
[49:59] And a few days ago, he was watching inspectorgadget and listening to the narration, and the narrator literally said,
[50:09] "Meanwhile, brain's just vibing." I was dead.
[50:17] I was like, that is so good. "Brain's just vibing."
[50:23] I mean, I feel like that's a real thing. "Brain's just vibing."
[50:26] All right. I dig it.
[50:29] I dig it. It was funny.
[50:32] OK, I got that one on there. Stack exchange.
[50:36] Ooh. Keep questions short.
[50:41] In my opinion, it's not valid because the logic would be something like, ask your error, provide your code,
[50:46] and ask what's working instead. Ah, I dig it.
[50:51] This is why I'm doing it all together. This is a group project.
[50:54] I'll put these notes in the YouTube video, so y'all will have it on the YouTube description.
[51:02] But-- I do have some recommendations for how to ask good questions.
[51:12] Oh, so I wouldn't actually say that people who want to learn about how to ask questions
[51:18] need to read that post from Meg Risdahl. It's more just sort of interesting
[51:23] to hear about thoughts behind Stack Overflow, but not specifically about how to ask questions.
[51:30] But yeah, so for asking questions-- and this applies to asking questions in pretty much
[51:41] any context at all. So this is something that I sort of learned
[51:48] when I was a grad student. If I were emailing a professor to say,
[51:53] like, I have a question about this, I would state what I was having the problem with.
[52:00] Like, OK, I'm working on problem five from homework two or whatever.
[52:07] I am-- this is why I'm confused or the specific thing that's going wrong, followed by, these are all of the things
[52:20] that I have tried to fix my problem. And for each of those, why that didn't work out.
[52:29] Because people are very often inclined to just say, oh, hey, I'm having trouble with this thing.
[52:39] Can you help me? And it's like, OK, sure.
[52:42] And then you tell me what the problem is. And then I say, OK, well, maybe I can help you.
[52:47] But what have you tried? OK, well, I've tried this.
[52:49] OK, why didn't that work out? And there's just so much back and forth.
[52:53] But if you provide all of that background to the person at the time that you are asking the question so
[53:03] that they don't have to seek out all the rest of that stuff, then it helps them.
[53:10] It makes it less work for someone to help you. And that feels better on the part of someone
[53:21] who's doing the helping. If you have to do a lot of work just
[53:26] to figure out what someone's problem is and how they've tried to solve it
[53:29] and all of that background, that doesn't feel so good. Because it's like, why are you making me work so
[53:35] hard to answer your question? Yeah, and then-- but then the other thing
[53:43] is that more often than not, if I go through the process of starting to type up an email, say, to a professor saying,
[53:54] this is my problem, and this is what I've done, and all of that stuff, the process
[53:59] of saying, of demonstrating that I have exhausted all ways to solve this problem myself generally
[54:09] leads to me solving the problem. Not always.
[54:12] I wish it worked for me, at least for this problem. And I feel like I am opening my Discord back up because I
[54:22] didn't turn off the right thing. So I was just like, I'm going to quit it.
[54:25] Because interestingly enough, I'm just going to pick apart something that I posted
[54:33] and see what y'all think. I also-- I'm going to do it in a random VS Code file, just
[54:45] a file, because it's hard to see all of the colors without it. Gabby, wait.
[54:55] No, give me all of this. Appreciate it.
[54:59] Gabby. Oh, we'll do Markdown.
[55:04] All right, so this is-- so I gave them my repo, and I'm also
[55:30] trying to figure out how to make this the coding version, too. And that's another question, actually, for everyone.
[55:44] When you're putting it in Stack Overflow or something, do you put it in Markdown?
[55:51] Oh, I certainly would. Absolutely.
[55:57] And why do I need to rename you? What are you trying to do right now?
[56:07] I show you guys the questions, but it's really hard to show you the question I asked with all--
[56:12] with the coding and colors not showing up. Oh, so save this as a Markdown file.
[56:25] OK, it is Markdown. Oh, you might need--
[56:34] I have prettier. Yeah.
[56:36] Oh, ha-ha, preview question. There you go.
[56:44] We will have preview as well, but-- The colors thing is determined by your VS Code theme.
[56:54] Oh. I thought prettier would help me, but apparently not.
[56:59] It's not going to do anything with colors. It's only going to do--
[57:02] prettier is only about formatting. Oh.
[57:07] For DOTUS, on some things, but a programmer uses all weapons sources to find the solution.
[57:23] Yeah, I get that. We got to do all of our homework, which--
[57:33] why-- why-- OK, y'all, bear with me. I don't know how to make this pretty at the moment.
[57:39] But basically, in my TweetyTag.index JavaScript, I ran nodeindex.js.
[57:50] And if the Twitter handle that I showed you earlier was-- it's basically asking the question
[57:55] I asked you at the beginning of the call when I was describing this and showing where I was stuck.
[58:00] And I think this is a good way. I'm following your instructions.
[58:10] But now I think I'm going to post it later on on Stack Overflow just to see if I can have
[58:19] someone answer the question. But again, if not, then I definitely
[58:24] have gone through my Discord channels. And I think I'm going to--
[58:29] didn't even think about it earlier. But I think this is a Prisma thing.
[58:32] So I can ask the Prisma community too. Sure.
[58:36] I am curious, when you say you run nodeindex.js, what does that mean?
[58:45] In CLI. How would you say that?
[58:49] If you-- if I run node.cls-- run command, run CLI command.
[58:58] OK. OK, so in the terminal, you're typing nodeindex.js.
[59:12] And then this is happening. Yes, if I have the Twitter handle equal to my name,
[59:19] it will add it to the database. If I have it equal to Twitter handle, it will not run.
[59:30] OK, so I am not a web dev. But it's not obvious to me that you would necessarily
[59:39] have node in particular run your index.js file, like execute it. OK, so adding in, because it's connected to the database
[59:52] query, that's why I do it. OK, what I'm wondering is if actually running
[59:58] that is your problem. It's how Prisma is saying that you check the query,
[60:05] the database. Always?
[60:10] Or just when you're testing it one by one? Because if I'm understanding your problem correctly,
[60:19] when you're testing it one by one, it works. But when you're trying to actually run it connected
[60:23] to the front end, it's not working? Right?
[60:30] Let me open it. And we'll just-- let's work through this.
[60:34] I'll ask. I am spitballing 100% right now.
[60:38] Anybody on hanging out with us today understand TypeScript or Prisma?
[60:44] TypeScript is just a subset of JavaScript. It is, it is.
[60:51] But my job-- hold on. Hold, please.
[60:55] Hold. Get a VS Code.
[60:59] I'm going to close these really quick. Just-- they can save or not.
[61:02] I don't really care. Go away.
[61:04] Thank you. Open.
[61:07] Oh, it was right there. Tweety tag.
[61:10] All right. And if-- just to make sure that--
[61:23] that's-- whatever. It's the most recent, because we just looked at this.
[61:27] All right. So now that I have all these beautiful things open, in--
[61:33] all right. So in Prisma, they have you do your schema.prisma
[61:43] to be able to connect it to the database and say what you want in the database.
[61:49] OK. So I named it--
[61:51] Twitter handle is the first one I'm working on. So I was like, they use the index.js file
[62:00] to be able to query the database. So I have Twitter handle.
[62:07] And if I enter Twitter handle gen-- not genod, just because I couldn't type earlier,
[62:14] it will show-- and it's node-- what did I say it was?
[62:21] Index.js. Thank you.
[62:23] Index.js. And just-- we can know that it should be that,
[62:30] because that's literally-- you're saying, execute this file.
[62:34] The file that you want to execute is that one. Right.
[62:37] Mm-hmm. OK.
[62:40] Superscript? Oh, it's a superscript.
[62:44] Superset. Yeah, what I said was subset, and that
[62:47] is what I meant, superset. So if you see, if I'm entering a written Twitter handle,
[62:53] it is adding a Twitter handle every single time. OK.
[62:58] So cool. That is what I want.
[63:00] I want Twitter handles to be added. But if I go--
[63:04] and this is just in the overall file. But if I go into Next Forms app and go ahead and run this one,
[63:16] which is cd Next Forms app. And I do npm run dev.
[63:28] Ah, dev, if I can type. Please open this.
[63:36] Thank you. I can enter it, but it doesn't go anywhere.
[63:47] It just gives me this pop-up. And the way that this one works is to--
[63:56] if I go into this one's index.tsx file. So that is the one on the right.
[64:05] It's saying, hey, the Twitter handle is from the form value, and it gives you the pop-up.
[64:16] So if I go under API and go to Forms, it is here, and it reads it.
[64:25] But I've been trying to do-- I need to pull what it's putting in here
[64:31] to put it into the database. Yeah.
[64:36] OK. So your form-- so you've got a--
[64:40] you had a constant-- I don't see it right now-- the constant that gets the handle.
[64:45] Maybe we need to scroll down to-- The constant is on the index.tsx file.
[64:55] OK, right. So that's the constant.
[65:00] But when-- OK, so wait. Do we want that to be a constant?
[65:13] Because then it wouldn't change, right? What up, JD, Kano, and Kano?
[65:22] JD and Kano, hopefully that's right. And for DOTAS, I will ask more about that once Laura
[65:29] gets her thought out. I don't want to--
[65:33] I mean, it's just sort of a wandering thought. It's interesting to me that these would be--
[65:39] the form and the data would be declared as constants, because we need to update them pretty regularly, right?
[65:48] But maybe that isn't going to matter. Are you using a tutorial or something to--
[65:57] Yes. --do this?
[65:58] Oh, wait. Let me actually have this on my Git.
[66:13] Oh, I just noticed the time. How important is it to you that we actually do
[66:22] some Anki on this stream today? I will say not as important as what we're working on right
[66:27] now. OK.
[66:28] But I mean, that's up to you. This is also-- you co-host Mondays, so--
[66:33] It's true. It's true.
[66:34] What do you want to do? I wonder if--
[66:41] I don't know. I mean, I really don't have a preference, honestly.
[66:44] Then if you're cool with it, I would love to-- because I might actually end up continuing to stream
[66:51] when we're done, because I just really want to figure this out, because it's like driving me insane.
[66:57] OK, in that case, let's do the Anki now. And then when you continue, you can carry on with this.
[67:05] I dig it. I dig it.
[67:06] All right, y'all. Then on that note, I'm going to pause on this thing
[67:12] that I'm driving me bonkers and work on it later today, which I will stream to do.
[67:21] So make sure you're following my Twitch account. And we will follow up with--
[67:31] I do think it's really good for us to have this question as well.
[67:35] And I will also add in-- if it lets me share my Anki decks, I will do that too.
[67:44] You can. Yeah.
[67:45] Sweet. All right, so we're on Anki.
[67:50] Let me also do this one. Do you have a bird?
[67:56] Oh, it's the birds outside. I have-- yeah, I have a window.
[68:00] And there's a bird beyond the window. But I do not claim ownership of the bird.
[68:06] That-- that's a really fun way of saying that. Do not claim ownership of the bird.
[68:12] All right, you know, I-- what?
[68:16] I don't know why I do this to myself. I like minimize things.
[68:19] And then I'm like, where did it go? I want it back.
[68:23] No, it's not that one either. Have you met Command-H, which is hide instead of minimize?
[68:30] Because I use-- I don't know if--
[68:37] Oh, I hate it so much. I'm just hiding everything now.
[68:41] This is kind of fun. Yeah, so-- and then if you-- do you do Command-Tab?
[68:48] No, but I could. So this is-- I-- this is my best friend for, like,
[68:57] moving around between my open apps. And I love Command-H because if you Command-M, if you minimize,
[69:05] then when you Command-Tab back to something, it'll stay minimized.
[69:08] And I'm like, I don't want you to do that. I want you out of my face.
[69:12] But I still want you to, like, be accessible from Command-Tab. So if you press Tab again, you can
[69:19] Tab through all of your open apps and then just open them from there.
[69:25] So it's a way of not having to, like, grab your mouse quite so often.
[69:30] I dig it. I dig it.
[69:31] And then Command-Shift-Tab goes backwards in the list. I dig it.
[69:38] I dig it. Thank you.
[69:40] OK, so I have this. And then we're going to do this Command-Tab thing.
[69:45] And Anki, there we go. All right, so we have the Anki.
[69:53] Yes, all right. So what do you want to make be your first deck?
[69:58] You know, we just haven't-- no, that would be weird.
[70:02] Let's do some Python just to work it out or get actions, either one.
[70:07] I'm down for both. OK, so if you look down at the bottom, there's a Create Deck.
[70:13] Yeah, Deck Name. I almost want to do a Learning with Laura deck, where it's
[70:19] just, like, I associate it all with you. But that's not always going to be helpful.
[70:25] So I'm going to do Python in general. I'll do Python in general.
[70:30] Sure. And we can go back to Automate the Boring Stuff,
[70:34] because we were talking about Python basics and, like, adding in these questions.
[70:44] Go to the bottom. Go to the bottom.
[70:47] Summary. There we go.
[70:50] All right, and then Add. Add.
[70:54] OK, Type. There's a bunch.
[70:58] So let's start with Basic and Reversed Card, because that's going to be the one that
[71:07] is most intuitive for anyone who has ever used a physical flashcard.
[71:13] OK. Choose.
[71:16] It might have been-- can you click Basic again?
[71:20] Because I think it's on Basic, but not-- and Reversed Card. There we go.
[71:24] Oh, OK. And then which of the following operators are values?
[71:32] And would I post all of them or just the ones that are correct? So in this case, you'd probably want to put all of those,
[71:48] but put them in the question box, yeah, on the front. OK.
[71:53] And then just choose the correct ones to go on the back. Which of the following operator--
[71:59] which of the following are operators and which are values? So on the back, do Values and then-- or Operators,
[72:07] and then do Values. So star is an operator.
[72:23] Below is a value. Negative 8.8 is a minus.
[72:45] Where are you out of order? Plus 5, and bold, bold, underline, underline,
[73:12] and bold, underline, or not. OK, whatever.
[73:20] And-- You know, I would take out the 1,
[73:25] just because this isn't necessarily-- like, in the future, when you have lots of cards,
[73:29] it'll be shuffling through them a bit. And so the 1 would be like, wait, what is-- 1 what?
[73:33] 1 what? 1 what?
[73:35] What are we doing? And then would you say the tags are Python operators
[73:48] and values? Up to you.
[73:50] Yeah. So for me, I would probably not put Python on it, necessarily,
[73:57] just because this is already living in the Python deck. And so I'm not likely to be looking for it across decks.
[74:05] But like, it's not going to hurt. So sure, why not?
[74:08] Did I do it? Did it make it?
[74:15] Yeah. Sweet.
[74:17] And wait. I think so.
[74:18] Wait, wait, wait, wait, wait. Python should say-- click on your Python deck in the--
[74:26] yeah. There we go.
[74:27] Oh, no. Hmm.
[74:31] The default-- what do you-- Oh, I think that it's like a tour of thing.
[74:41] But why did it not show up? Oh.
[74:45] It has two cards for it. So whose card won?
[74:53] Yes, I think maybe you made it in the default deck instead of the Python deck.
[75:00] Oh. And for Dodus, you just unlocked it.
[75:07] Unlocked what? So you can do change deck.
[75:16] And you know what? I think I may have been wrong when I said do basic and
[75:19] reversed card, because I think that's why there are two cards. I think it should have been just basic.
[75:23] Sorry, I haven't had to set up a deck from scratch in so long.
[75:28] My bad. But you can change the type.
[75:31] So if you-- I want to delete this one.
[75:32] Forget. There we go.
[75:35] You can delete it as well. But I think you have to actually open the card in order
[75:43] to delete it. Oh, there we go.
[75:49] If you go under Notes-- so when you right-click, and then go to bottom Notes,
[75:56] and then Delete. There you go.
[75:59] OK. We will now start--
[76:02] yay! That is my favorite emoji.
[76:05] Is that weird? Oh.
[76:08] I really like that emoji. What is it?
[76:10] I don't know. It's something holding a little heart, and it's really happy.
[76:13] Yeah, that looks really cute. It's really happy.
[76:17] I love-- I don't know. OK, so now I go to my deck.
[76:26] Yeah. Python.
[76:27] Python. Now add one.
[76:30] Add. And then--
[76:32] I guess we can just do the same. Yeah, go back to basic.
[76:35] Oh, deck right here. Yeah, yeah, yeah.
[76:37] It's totally what Caff-- Caff-C?
[76:44] Caa-- we're going with Caff-C was saying. OK, so now we'll minimize that.
[76:53] [HUMMING] [HUMMING]
[77:49] Yeah, there we go. And I don't know if it shows up for y'all,
[77:54] but it looks like it kept some of that yellow screen. So I'm just going to make sure that they are--
[78:03] no, no. I don't see it.
[78:05] Cool, well, hopefully not. And add it.
[78:09] Mm-hmm. All right, so now if you go back to the big Anki window--
[78:14] yeah, and if you click Study Now, you can see your card. Oh, and then show answer.
[78:26] And I'm going to say that it was easy. Mm-hmm, and that 4D that was above the easy meant four days.
[78:36] So it'll ask you again in four days. Oh.
[78:41] But it's not going to notify you. So what that means is that if you
[78:48] are using Anki in the next three days, it won't ask you about that card.
[78:55] But if you don't use Anki for two weeks, four days will have passed.
[79:00] So it will ask you about that card. OK, got it.
[79:06] All right, so which of the following? Add basic-- OK, so this has gotten easier.
[79:23] I feel like I can at least keep going with these. Mm-hmm.
[79:30] Good. String.
[79:34] So the question that it's asking is, which of them is a variable and which is a string?
[79:43] See, it's a good thing you read it. This is probably one of the biggest things that
[79:50] are really, really hard for me is I don't mean to, but I will skip through it.
[79:56] And I'm like, no, no, no, I got to read it. You got to read it.
[79:58] But my brain just honestly does not do it. And from what I've understood, that actually
[80:04] is something with dyslexia because it's where we just will skip letters or skip entire words
[80:13] that a lot of people with dyslexia will just go for context.
[80:18] Just the way the brain works, I'm like, oh. I don't think that I'm dyslexic, but I totally do that.
[80:26] I think of it as more to do with my ADHD, but maybe they're interrelated because brains, man.
[80:37] Brains are weird, and they're cool. Now I feel like I want to end on these when we take them.
[80:47] I can be like, we will just answer the questions and as we're typing them.
[80:53] I need to type. I'll close.
[81:00] I'll work on this later. I was going to say, let's try another type of card.
[81:06] Oh, OK. Which is the closed deletion kind.
[81:11] And I have to remember how we do this. So you have to--
[81:17] it's a plug-in, the closed deletion. So what you have to do is I would literally--
[81:24] I am, in fact, Googling closed deletion Anki plug-in. Mm-hmm, mm-hmm, OK.
[81:40] Close. But we want closed deletion, and we definitely
[81:47] are going to have to install this plug-in. Nope.
[82:00] Yeah, so literally search for it in a browser. I think you sent this to me already.
[82:10] So we do need to get to the plug-in itself. Oh, so down the third one from the bottom
[82:31] is closed deletion, which is going to tell us how to use it, but you have to get it first.
[82:40] So search for Anki closed deletion plug-in. Ah, I'm clicking too many buttons, y'all.
[82:48] Add-on, right? Maybe it's called an add-on.
[82:58] OK. Yeah, let me make sure that I know which one I have so
[83:09] that I'm telling you the same thing that I use. [INAUDIBLE]
[83:30] Yeah, OK, so go for that. Yeah, there we go.
[83:34] OK, so if you-- oh, if you go back one, I think you were on--
[83:46] scroll up. Yeah, OK, so scroll down again.
[83:56] And what we're looking for is a number. Maybe it's all the way at the bottom.
[84:06] Hmm. Because there will be a number that you use-- oh, wait.
[84:11] Go back down a bit. Down, going-- oh, this is from 2019.
[84:26] It may be too old. OK, then let's look at the-- there's a YouTube video.
[84:36] There's a YouTuber, like Anki-- Anking, I think, is his YouTube channel.
[84:44] And this is literally how I learn to do and relearn, because sometimes I forget my memory
[84:50] and how to use my memory tool. OK, yeah, so a lot of Anki users are medical students.
[85:09] But that's OK, because the tool works the same. And so if you look--
[85:15] if you search this channel for clothes deletion-- OK, yeah.
[85:29] And Frank is saying there are multiple clothes add-ons on the Anki 2.1 add-on page.
[85:43] All the ads, always the ads. This isn't what I saw before.
[85:50] No, it's literally not. [VIDEO PLAYBACK]
[85:57] --single card. If you're like me and use clothes deletions,
[86:00] but use the C1 most of the time, this is for you. So clothes deletion single card, I really like,
[86:08] although I have some friends that don't like it very much. I made an example card.
[86:13] As you can see, I tried to make a really good one with bolds, underlining italics.
[86:18] But with this particular card, it makes sense to have this, the potassium and the sodium,
[86:24] both be a part of one card, because they're kind of one idea.
[86:27] Normally, if we're creating a card-- I'm just going to go A, clothes deletion B, clothes deletion C,
[86:35] clothes deletion D. Now, you can see mine goes 1, 1, 1. Anki's default settings would do this.
[86:43] And if I added another clothes deletion, it would be C4. But with mine, you can see no matter how many I add,
[86:51] it's always C1, which I think is really nice, because they're all together.
[86:56] And I tend to use the C1s more often than not. So if you're tending to do C1, C2, C3 more than you're
[87:05] using the card that has multiple clothes deletions that are all C1, it's out.
[87:09] This is maybe not the video. It's this channel, but it's not this video that I used,
[87:16] because this is more advanced. This is once you're already in there.
[87:20] I can do search. I think this is showing all of that, but--
[87:35] well, we can look into it, because I know that you're at time.
[87:41] I don't know where the last hour and a half went. Like, I feel like we just had so much fun.
[87:46] Yep. And that tends to happen when you're on the stream.
[87:51] But we do have more people here. And y'all kind of heard and saw, like, wow, long button,
[88:00] like, how Lauren and I just do this thing, where it's like, just come hang out with us.
[88:06] We're going to work on some random shit. And that's-- we went over a little inky.
[88:12] We wanted to figure out how to ask questions. We did go on a pretty good tangent about Twitter.
[88:19] And that is honestly what Mondays are going to be. Yes, they'll all be based around Python,
[88:27] yet it's not necessarily going to be just Python. So if you want to come up with some ideas for what we should
[88:36] call this mini-series, or series within a series, a series-- I don't know what it is, but--
[88:44] Laura's here every Monday. That's what I'm trying to say.
[88:46] We start the week with Laura. I just found the plug-in that I was thinking of.
[88:54] So I'm going to send you the link. Nice.
[88:57] And the reason that we weren't finding it is because it does not have closed deletion in the title.
[89:04] That's what it is, but it's not. There we go.
[89:12] Yay. And so far, they're saying, learning with Laura.
[89:15] I think it sounds good. But yeah.
[89:21] Yes. That's what I put today's as, is I'm like,
[89:23] it's always learning with Laura. I just don't know what it's going to be about,
[89:26] because we are always learning. So this one that I just sent you, if you pull it up--
[89:40] Download this add-on. Yeah.
[89:48] Do you want to share the screen? Oh, hey.
[89:52] I thought I would still. I clicked the buttons, y'all, but you just couldn't see me.
[90:00] The reason that this one is so cool is because it lets you put in more than one line.
[90:06] And if you're doing code, very often you want to be able to enter more than one line of code.
[90:13] And so that's why we weren't finding it, because it is a closed deletion thing,
[90:19] but it's not called closed deletion. There it is.
[90:23] Oh. That's not the plugin or the add-on.
[90:27] It's called multi-line type answer box. I'm seeing if I can log in so I can get that part of it
[90:35] to get download at all. And I can show you what that looks like on my end.
[90:43] Is it OK if we go over by a minute or two? Yeah, I'm good.
[90:46] OK. OK, cool.
[90:48] Oh, yeah. Go share your screen so I can set up my account.
[90:51] Sure thing. Please.
[90:54] OK. He's a thank you.
[90:55] So Google, present, share screen, looking for that. OK, there we go.
[91:07] OK. So here's my deck on Vim.
[91:15] And so if I say study now, so this is go back to where you came from in a search.
[91:21] So for this particular deck, I don't necessarily need the type answer box to contain more than one line.
[91:30] But it's like there's no reason-- I always use the multi-line type answer card type
[91:37] for closed deletions because then I have the option of using more than one line.
[91:43] Whereas with a regular closed deletion, then I don't. And so I can go back to where I came from in a search
[91:50] if I type. I literally don't remember.
[91:55] But it might be Control-I. So Control-I. Oh, it's Control-O. OK, so it doesn't like that I didn't capitalize the C
[92:11] in Control. I don't care about whether I capitalize that because I'm not
[92:15] actually going to type CTRL. I'm going to press the Control key.
[92:21] However, I do care that it was I instead of-- I mean, that it's supposed to be O instead of I.
[92:26] So I'm going to say that I got this one wrong. But yeah, anyway.
[92:32] So then I'm just going to finish this one for now. I can show you another one where we have--
[92:39] so this is a tech that I made. So I am on a developer relations team.
[92:44] My job title is technical writer. But I am slightly also doing some advocacy.
[92:54] And so I made this deck. I don't want that one.
[92:58] I want the Wasm one. So this is our WebAssembly, my WebAssembly deck.
[93:01] So I made this deck to help me understand-- or well, first of all, to help me
[93:08] be able to deliver an elevator pitch. Why is WebAssembly good?
[93:13] What is WebAssembly? What is it good for?
[93:15] And all of that kind of stuff. And so this card, it asks me, so what
[93:22] is the original use case for Wasm? It was running compiled languages like C++
[93:27] in the web browser. But since then, it has evolved to include
[93:30] non-browser environments like something and IoT, and so server-side environments, say.
[93:38] And so there we go. And that's my-- so I can stick that in there.
[93:44] So I know this is a classic closed deletion case, where I can have everything there, but the little piece
[93:53] that I want to have myself fill in, in this case, the server. So I got that.
[93:59] So I'll say that that was good. And then-- oops.
[94:05] This card is wrong. So I'm going to have to fix that.
[94:09] I'll just say again, and then we'll keep going. I'll fix that later.
[94:13] So in my background here, so I've got all of this context. But the part that I want to be able to state right here
[94:22] is so you can compile, apparently, all these different languages.
[94:27] So what kinds of languages can you compile to WebAssembly? You can compile TypeScript, and Go, and Rust, and JavaScript.
[94:39] So let's see how I did on those. Yep.
[94:43] OK. So I said, too, that we're not on the list.
[94:47] But it is the case that those are also available to compile to WebAssembly.
[94:55] So that lets me know that I knew this thing. So I can say that that one was good as well.
[95:01] So what does it look like to actually create one of these cards?
[95:07] Oops. I just closed the window.
[95:09] I just closed the window. I'm going to have to open it again.
[95:12] And then Frank just sent for chat, multiline, type, answer box, or add-on.
[95:21] Thank you, Frank. I'm getting it on my computer as we talk,
[95:26] getting it updated for here. So that way, I can, by the time you're done showing us,
[95:35] I have it working. Yep.
[95:38] So say I wanted to create a new card here. So I can add.
[95:46] And for this card type, I'm actually using this other add-on called Catech and Markdown Close.
[95:56] I'm just going to choose that. And then I can type in a bunch of text.
[96:01] So this is-- oops. I'm typing on my keyboard in a different position
[96:11] than I usually do. Oh, y'all, it helps if I add her back to the stream, right?
[96:15] Yeah, there we go. OK.
[96:18] And so then in order to occlude, to hide the word bunch, or say I wanted to say this is a bunch of--
[96:29] what is it a bunch of? It's a bunch of text.
[96:32] I can type in a bunch of text. I can say C1 is text and then add.
[96:44] And then if we look at that card, which I'm going to have to find in my deck,
[96:52] because otherwise it's going to show me a bunch of other stuff, I can search this deck for text.
[96:58] I'm just seeing the main deck. I'm not seeing anything else.
[97:05] Oh, because I shared the one window. But that's OK.
[97:10] I can-- let me reshare. Oops, I have code showing that needs to not be on the stream.
[97:43] So just a sec. Dialing my workspace here.
[97:49] I will say I need to actually-- like, read this closer because I'm like,
[97:56] I don't know how to get it actually working with-- oh, go to Tools menu, Add-ons.
[98:05] So if you read, it tells you how to do it. Add the heads up.
[98:13] OK. So-- and I've got one more here.
[98:17] And I will hide us so that we're not doing inception. OK.
[98:22] So we have-- clean these up, too. There we go.
[98:28] So the way I found this-- let's reverse engineer this. The card that I just made, if I click Study Now,
[98:38] it's just going to show me card by card. But if I want to see the card that I just made,
[98:42] I can go to Browse. The deck that I made this card in is my WASM deck.
[98:47] And then I can search my WASM deck for the word text, or I can search for the phrase.
[98:53] This is a bunch, because that's what I had going. There we go.
[99:08] This is a bunch of-- and then we can see how it's got the two curly braces, and then C1,
[99:13] and colon, colon, text. And what does that even look like when
[99:18] it's being used as a card? I can click Preview.
[99:21] And so then it says, this is a bunch of what? It's a bunch of text.
[99:27] I feel like-- OK, y'all, because we did totally go over all of this stuff.
[99:38] Next week, what if we literally only focus on Anki and work on what we want to do and come up with questions?
[99:53] Because I feel like that is also-- you ask me, you're like, well, what
[99:58] do you want to build them for? And I'm like, I don't know.
[100:02] What should I be studying? And because that kind of stuff doesn't show up for me,
[100:09] like on repetitive stuff, like GitHub and stuff like that, I'm like, OK, how do I open something?
[100:18] And I'm like-- so that's why I'm kind of wondering. I feel like if we--
[100:26] I can work on coming up with ideas of what to make. Does this make sense?
[100:33] I feel like I'm going around trying to describe-- I'm not sure.
[100:37] I am going to push very gently back on the plan to talk only about Anki.
[100:44] Because I feel like it will-- doing it, doing something in the context
[100:52] where you would normally use it. And so normally, if you were using an Anki deck
[100:57] to learn something, you'd be doing-- you'd be embedded in the learning, the thing
[101:01] that you're learning. And then when you came across something that was new,
[101:04] you would add it as a card to your Anki deck. Oh, OK, OK.
[101:09] So I can get the app installed, because I almost have it totally installed.
[101:13] So when we go back to probably Python next week, we can add it from there.
[101:21] I dig it. I dig it.
[101:22] Yeah. And we can review--
[101:24] like if you have the spoons to add some more cards before then, we can review from the cards that you already
[101:31] have before then. And then be making new ones.
[101:39] I like it. I like it.
[101:41] I dig it. Thank you.
[101:43] That is a good idea. And yes, everyone, so Laura will be back on Monday.
[101:51] I will be streaming later today working through this project, because this project is driving me bonkers.
[101:59] I don't know when, but I will be back later today. And yes, tomorrow, I don't think I have a guest tomorrow,
[102:06] actually. I should probably go look.
[102:10] I'll be streaming something tomorrow. I just don't know what yet.
[102:14] Yeah, I don't have a guest tomorrow. That's crazy.
[102:16] All right, so hit y'all up later. We are going to raid into Anthony's channel,
[102:23] because Anthony is dope as shit and who I like to call my internet big brother.
[102:32] So I'm going to send you guys over there. And if there's anything else, hit us up on Twitter.
[102:41] Those are our names on Twitter. We talk enough about Twitter today.
[102:45] And we will be back next week. Bye.
[102:48] Bye-bye. In however many seconds this is going to take to raid.
[102:54] Just awkwardly stare at y'all. [LAUGHS]
[102:59] [AUDIO OUT] [BLANK_AUDIO]

