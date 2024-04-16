---
showLink: "https://www.youtube.com/watch?v=TwqP4vcRJ1E"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "learn-with-jenn-navigating-typescript-homework-and-tech-updates"
title: "Learn with Jenn: Navigating TypeScript Homework and Tech Updates"
publishDate: "2023-09-29"
coverImage: "https://i.ytimg.com/vi/TwqP4vcRJ1E/maxresdefault.jpg"
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

[00:00] (upbeat music) (upbeat music)
[00:05] (upbeat music) (upbeat music)
[00:10] (upbeat music) (upbeat music)
[00:15] (upbeat music) (upbeat music)
[00:20] (upbeat music) (upbeat music)
[00:33] (upbeat music) (upbeat music)
[00:45] (upbeat music) (upbeat music)
[00:54] (upbeat music) (upbeat music)
[01:07] (upbeat music) (upbeat music)
[01:16] (upbeat music) (upbeat music)
[01:31] (upbeat music) (upbeat music)
[01:42] (upbeat music) (upbeat music)
[01:54] (upbeat music) (upbeat music)
[02:08] (upbeat music) (upbeat music)
[02:18] (upbeat music) (upbeat music)
[02:32] (upbeat music) (upbeat music)
[02:42] (upbeat music) (upbeat music)
[02:56] (upbeat music) (upbeat music)
[03:05] (upbeat music) (upbeat music)
[03:18] (upbeat music) (upbeat music)
[03:32] (upbeat music) (upbeat music)
[03:51] (upbeat music) (upbeat music)
[04:01] (upbeat music) (upbeat music)
[04:13] (upbeat music) (upbeat music)
[04:23] (upbeat music) (upbeat music)
[04:37] (upbeat music) (upbeat music)
[04:45] - Hello, hello, beautiful humans. Welcome to Teach Gen Tech,
[04:58] where we're learning tech to break down the barriers of getting into tech.
[05:03] And today I am working on some homework, of learning TypeScript.
[05:10] So first off, I am definitely gonna see if I could get this new playlist running,
[05:20] even though I should probably go look at YouTube and see what happened there.
[05:25] While a while back, if you caught errands in my stream, I was working on finding a playlist and music,
[05:33] yet I was told that the music was copyrighted and I'm like, yo, I was given permission from the website.
[05:43] And so what is going on? What songs was it?
[05:50] I'll show this to y'all because, you know, why not? And I gotta figure it out so we can work on this together.
[06:03] And then once I figure out the music and if I can play this playlist, then I will get started.
[06:09] ♪ Doo, doo, doo ♪ 'Cause I don't think everybody wants me to sing to them.
[06:15] I mean, I could, but you know, that could be weird as well. So just a second.
[06:24] And then after that, I will be going and working on learning TypeScript stuff,
[06:34] which I'm excited. I am skipping chapter one.
[06:36] If anyone is curious, I'm definitely skipping chapter one. It has to do with classes.
[06:41] If you caught the last stream with Josh, the author of the book,
[06:45] me and chapters, we're not, I don't know if we'll ever be friends, but maybe.
[06:55] Who knows? Okay, and we are all about the dark mode today.
[07:02] Over on the right, which I need to zoom this in anyway, we are looking at my iPad.
[07:10] Ta-da! Very lovely, which I will zoom in when we get to that point,
[07:15] but we are working on this one right now. So.
[07:21] ♪ Na, na, na, na ♪ Oh, yes, homework.
[07:30] I'm getting to it once I figure out why this music was copyrighted.
[07:34] Because it feels weird not listening to music while I'm doing this.
[07:42] Falling in love instrumental, no impact. Okay, then mute the song.
[07:50] Mute all of the song. Oh, cancel, mute only the song.
[07:58] We'll see, okay. So, we're return to upload, sure, next.
[08:05] Publish this, because Erin's probably wondering why I have never published this, which I don't blame her.
[08:16] Right, I don't get, like, it's so weird with the copyrights. Let's go to HootSuite, is that what I'm using?
[08:28] Should probably look what I'm using for social media. I think it's that one.
[08:32] Sure, let's see. Oh, I'm using Buffer.
[08:41] There's so many different social media ones. Do you ever use social media things?
[08:47] Social media things, that's a very broad term. Posting on multiple social media platforms, like this.
[08:57] ♪ Do, do, do ♪ Do you have a preference on which one?
[09:03] ♪ Do, do, do ♪ Let's paste this before I forget.
[09:10] This is a livestream from a while ago. Zero, generally, all your stuff for Twitch is on Twitter.
[09:27] Okay, oh, that's fair, that's fair. I mostly do, I don't even use Snapchat.
[09:35] I probably should. I wanna start using Instagram more,
[09:39] because, like, Instagram and TikTok. Oh, yeah, totally cool.
[09:46] It's okay if you guys don't reply. And what up, Alex?
[09:49] Even though Alex, just as a heads up, seeing all of your, like, usernames,
[09:54] I'm gonna call you something else at some point. Oh, did you?
[09:59] Oh, that's cool, yay. Let's see if the AI wants to be my friend.
[10:06] I'm very lazy when it comes to this kind of stuff. And just use all AI stuff.
[10:15] AI generate, oh, wait, you just came back. Shorten, oh, what's this AI generator doing?
[10:23] Well, it's thinking. I think it is thinking.
[10:39] Let's do this 20-minute playlist and see what copyrights decide to argue with me.
[10:47] (upbeat music) So, I'm hoping that it can be interesting.
[11:01] Zero, did you work at GoDaddy? That's a very random question.
[11:11] But I wonder if that's how we know each other. Yes, okay, I don't, okay, so did I.
[11:22] So, maybe that's where. I don't know.
[11:25] GoDaddy was such, there were so many people that worked there that it's hard to say if, like, where the overlaps were.
[11:33] That, and I have a horrible memory. (Emmy vocalizing)
[11:46] And write a tweet about, (Emmy vocalizing) So, in ChatGPT, I don't know if y'all knew this,
[12:07] but you can tell it some custom instructions, which is lovely and creepy all at the same time.
[12:15] So, in these custom instructions, I uploaded some of my blogs that I've written,
[12:24] so it knows how I talk, which is lovely. Like, it's just so much fun
[12:31] because it writes things in my language. Right, it's crazy how smart it is.
[12:42] I love it. Almost hate it, but it gets me unstuck for a lot of things.
[12:48] So, it's taken me, like, five minutes to write this, and instead of, like, half an hour
[12:58] trying to figure out how to minimize it. (Emmy vocalizing)
[13:08] (gentle music) It's Erin.
[13:18] You should try to figure out. Erin, oh, wow, I can spell Erin.
[13:26] Customize. Yes, you are way too long, but that's okay.
[13:33] (gentle music) Erin, what is your...
[13:43] I never remember it. (Emmy vocalizing)
[13:52] Yes, I'm totally looking at this one off-screen. I've learned that lesson.
[13:56] It's not worth it to look at this stuff if you have, like, DMs open.
[14:03] (Emmy vocalizing) It definitely could be awkward.
[14:06] Is awkward, could be awkward, all of the above. Sweet.
[14:21] I hope you have a cool client. And Alex, if you are still hanging out a bit,
[14:32] what jobs are you looking for? (gentle music)
[14:37] (upbeat music) (upbeat music)
[14:42] (upbeat music) (upbeat music)
[14:48] (upbeat music) (upbeat music)
[14:53] (upbeat music) (upbeat music)
[15:03] (upbeat music) (upbeat music)
[15:16] (upbeat music) (upbeat music)
[15:31] (upbeat music) (upbeat music)
[15:42] (upbeat music) (upbeat music)
[16:09] (upbeat music) Oh, I can definitely zoom in.
[16:28] I have glasses on and I'm like, I don't know, arm's length away from it.
[16:33] I sit really close. I am gonna be working on the next project soon.
[16:38] I'm getting these posted. But thank you for the call out.
[16:43] They are really small. Ooh, okay, that one's really big.
[16:48] That one was too big. There.
[16:50] And this one, when we get to it, I'll be able to like super,
[16:55] actually, let me do this. The tablet needs to move.
[17:01] There. So when we get to that, it will be much bigger.
[17:08] (upbeat music) Should be easier to read at that point.
[17:13] (upbeat music) Oh, we get examples now.
[17:27] I don't know if this is a good example. Like, I'm a little worried.
[17:31] Oh yeah, thank you. Does it look better now?
[17:38] And are you watching on mobile or on desktop? Oh, here.
[17:54] This is also just taking up way too much room. I am working on some social posts
[18:07] because I went to go check out, we don't need this one,
[18:12] a copyright issue. And then I was like, oh yeah,
[18:24] I didn't actually get this posted. So I should do that really quick.
[18:28] Let me just copy and paste this one. LinkedIn will just be special
[18:31] and have its own special one. (upbeat music)
[18:35] I'm using a tool called Buffer. Even though a minute ago,
[18:50] I couldn't remember what they were called and they're scheduled.
[18:53] And now I can actually move on. Yay.
[18:57] And we will get this much larger. (upbeat music)
[19:05] Also, this is one of those curved screens that I'm like, I'm pretty sure people,
[19:11] like it's so big that I'm like, maybe I shouldn't use this screen as my streaming screen,
[19:17] but you need bigger. Oh, wrong screen, wrong one, wrong one.
[19:22] So what we got going on here is I stream with Josh,
[19:35] the author of this book, which I believe I can do a shout out on here.
[19:39] Y'all should definitely go follow Josh. He's been coming on the stream for,
[19:48] oh gosh, almost a year now. And yes.
[19:57] Oh, ew, oof. That's a hard one, pseudo.
[20:02] Like, that's rough. Because we've been doing this for like two,
[20:12] or almost a year. We have seven episodes and I haven't done the homework.
[20:18] I'm also not always the best at remembering to do the homework.
[20:24] So if you wanna check out the seven episodes we've done so far, a chapter per episode, that is here.
[20:32] And yeah, I'm skipping chapter one. So I have the summary.
[20:45] I'm gonna go through the summaries of each of these first and then go do the homework
[20:50] after I look through the summary, but I am skipping chapter one.
[20:53] Chapter one has what I hate the most. Hate the most, classes.
[21:00] I don't understand them yet, so I'm just skipping chapter one, the homework.
[21:04] Oh, okay. That works, pseudo.
[21:11] Well, if you need anybody to look at, yeah, you wanna come on the stream and teach me classes,
[21:19] you can. Not this stream, but you know, hit me up.
[21:23] I do, oh, I have a new link you can fill out. I just transferred everything over to monday.com
[21:31] and actually have it where people can fill out their information and I can get them scheduled.
[21:40] So I can show you guys the form though. That's okay, that's safe.
[21:47] It's very easy. It's just getting all your information
[21:50] and then we'll get something scheduled. So let me put that.
[21:53] I'll put the form here. Have you, are you in our OSRG Discord?
[22:03] I feel like I never know where anybody is. Just talking to Zero about that.
[22:10] Zero and I are friends from Instagram. I mean, nothing.
[22:15] Well, if you decide to join, this is where I put a lot of the updates.
[22:24] Oh yay, oh yay, double yay. Thank you for the follow.
[22:30] If you do decide to join the Discord, it's cool because we have it where it's,
[22:36] we also play tabletop games. So it's a fun guild to hang out in or Discord,
[22:46] but it's where I put all of my updates and streams, which I should be copying
[22:51] and pasting in there as well. I'm not yet, but I will.
[22:54] And we also, I have a show called "Shit You Don't Want to Talk About"
[22:59] and I put that kind of stuff in there too. It's been on pause while I get Teach Gen Tech
[23:05] back up and running, but I will get both working. But that's why I'm doing TypeScript
[23:09] is to do my homework so I can finish building my site 'cause I've been stuck.
[23:14] Oh, see. Like, I don't want to sell anybody on it.
[23:21] It's like wherever you find your community, I'm in a shit ton of servers,
[23:27] but this one's like special to my heart. Like, I don't know, it's just the easiest.
[23:32] There's super techie people in this Discord that make me level up and it's,
[23:40] one of my favorite things is as a newbie, they've been very patient with me
[23:44] and have learned to help me gauge on, okay, am I just really stuck
[23:48] and I need somebody to help me give me the answer or push back on like, no, Jen, go figure it out yourself.
[23:55] So it's like a mixture of the two. So I really appreciate them.
[23:59] And that's why I love it because I get to talk about mental health
[24:03] and tech newbiness and super techie people, and we're playing The Expanse, which is fun.
[24:10] I love it. It's like a, if you haven't,
[24:15] have y'all seen The Expanse or read the books? Oh, am I, yay.
[24:24] I don't know if my mouse just died. Wait, why did you disconnect?
[24:32] Did you just die? Why?
[24:36] Okay. Momentary pause of,
[24:42] apparently I didn't realize my thing wasn't charging and I need to find, aha, there's the charger.
[24:49] My very messy desk. So messy.
[24:52] Okay, see if that works. I'm gonna plug it in.
[24:57] It should work here momentarily. I'll awkwardly use my laptop for now.
[25:02] And go say hi really quick, yay. Oh damn, you got like a full copy and paste bio.
[25:14] That is cool and smart. Wave hi.
[25:24] Okay, that is smart. I'm like totally smart.
[25:33] I'm gonna leave it there and other people will reply to and say hi.
[25:38] Yay, that's exciting. Thank you.
[25:41] Okay, so, but yes, if you wanna come teach me classes, like let's connect 'cause,
[25:48] have you ever heard of Josh's, or this book, "Learning TypeScript"?
[25:55] I have mine like inverted right now, but I have it on dark mode.
[26:01] I'm gonna go to chapters. Chapters, chapter, chapter.
[26:09] Okay, okay. This book, definitely worthwhile
[26:21] because it talks about like what we've gone through so far. And let me make this one.
[26:28] Oh yeah, my mouse isn't working. We gotta use this one.
[26:31] Make this one bigger so you can see it. Is we've been going through,
[26:38] yes, it's a table of contents of this book, but we've gone through part one,
[26:42] which went from like the very beginning of TypeScript to the type system, unions and literals,
[26:50] objects, functions, arrays. Oh my gosh, interfaces.
[26:57] And we've done this over the last year and next is classes, which Josh was like,
[27:04] "Yo, we can totally go through this chapter or we could skip it,
[27:09] but maybe you should have someone on the show about classes." And when we were going through this,
[27:14] we realized that chapter one, "Homework" had classes in it. And that is why I'm skipping it.
[27:20] Let me go back to finding the correct chapter that I was in.
[27:31] Chapter is this, ah, okay. (gentle music)
[27:36] So, summary of chapter one before I go look at "Homework" for the other one is,
[27:44] just a brief history of JavaScript, the pitfalls of, I think this is really smart
[27:52] because it's like the costly freedom, documentation and developer tooling.
[27:57] I think it's been very interesting and Sudo, just to give you a heads up
[28:02] and any like for background for everybody else too. As much as I know about JavaScript,
[28:09] I know about TypeScript 'cause I've been learning them at the same time
[28:13] where a lot of people are like, "Yeah, you should know JavaScript first."
[28:17] Even Josh was like, "Yeah, you should probably know JavaScript first."
[28:20] I like to do things the hard way apparently and have been learning this as I go,
[28:27] which has been very great because Josh has been very patient
[28:31] with helping me figure out, is this a JavaScript thing or a TypeScript thing,
[28:36] which I'm very, very grateful for. So, some of the, what is TypeScript of the language,
[28:44] the type checker, compiler and language service, the advantages, which I think is pretty self-explanatory,
[28:52] but I like that he put freedom through restriction and I'm like, it's true.
[28:58] It brings structure. I have a talk coming out next week about that.
[29:01] And then write some code and what TypeScript does not,
[29:09] it's not a remedy for bad code. Like if you don't know what you're doing,
[29:11] it's not gonna get any better. You're still not gonna know what you're doing,
[29:14] which is lovely. It's such a wonderful experience.
[29:18] And then extensions to JavaScript. It's not slower to JavaScript and it's not done.
[29:26] And some of the favorite parts of the book are, there's like little funny things in them.
[29:34] What happens if you spot errors running in a TypeScript compiler?
[29:39] You better go catch them. Okay.
[29:46] This is why I told Josh that I can get through his book because there's funny and punny things.
[29:53] And I've been using my iPad to go through this and take notes.
[29:59] So chapter two, the type system, you can kind of see that happening of JavaScript's power
[30:05] comes from flexibility. Be careful with that.
[30:08] I just like things, they're so fun. They're so fun.
[30:12] But okay. I'm gonna mute myself while the dog decides
[30:15] to go a little bananas. Maybe.
[30:20] Is she done? (dog barking)
[30:26] No, no, she's not. BRB on mute.
[30:31] (dog barking) Really dude?
[30:46] Okay, BRBL. I'm gonna go see if I can get the dog to shush.
[30:49] (upbeat music) Okay, I think we're good.
[31:21] And just as to go back here. So Sudo, you stream.
[31:42] And I'm curious, do you have any pets? Because I'm just like,
[31:48] how many people does this happen to where it's like, your animal is inevitably gonna be super annoying?
[31:57] Why I saw in your intro that you definitely work a ton.
[32:18] Is that a big reason why you don't stream a lot? Okay, I'm not gonna go through the entire chapter.
[32:31] But we have it here when we need it. I'm gonna go here.
[32:37] Make this even bigger. Projects.
[32:46] And if anyone wants to follow along, this is Josh's site, or the book site.
[32:58] Okay. (upbeat music)
[33:13] Oh yeah. I totally, yeah, I get that.
[33:22] I totally get that. For those watching back on the playback
[33:29] or just joining the conversation, a bit about like streaming on Twitch
[33:33] or being able to get followers is something I'm not great at.
[33:37] Because you need consistency. Consistency on like times and like,
[33:43] Twitch gets happy and will show up if you stream at the same time every week.
[33:49] And it's hard to do that. Like, it is difficult to always do that no matter what.
[33:57] And even for me, if I have a guest, if I don't have a guest,
[34:00] or if I just don't have the mental capacity to do it, it's a big reason my other show got put on the back burner.
[34:07] And I feel it's a balance. And I think a lot of people don't get that
[34:16] unless you have done content creation or have live streamed.
[34:23] Because people, at least from talking to people, I found that they're like,
[34:29] "Yo, you don't, you just get to talk and hang out." And it's like, "Yes, I do."
[34:33] And it's so fun. But it's also a lot of energy
[34:36] 'cause it's not me just sitting in bed, napping, cuddling with the dog.
[34:41] So, yes. And for networking pseudo,
[34:47] is there like anyone or any job in particular, you're like, "I really wanna meet this person"?
[34:52] Curious. 'Cause networking is so vital.
[35:01] And it's definitely not like the only place where you will or won't get a job,
[35:09] but it helps so much. Incredible amount.
[35:14] And I'm currently trying to find out more about Slush. But I need to focus, focus, focus, focus.
[35:23] We need to do System of the Clown. That is very silly, Josh.
[35:27] Josh isn't here, but I'm still gonna tell him how silly it is.
[35:30] Okay. And yes, y'all, as a heads up,
[35:35] I'm going to awkwardly read some of this out loud because if I don't, I will skip words and letters.
[35:43] And that's what I do and why I hate dogs so much. But hey, practice, practice, practice, practice.
[36:03] That totally makes sense, you know? I agree with that.
[36:07] For me, I guess, like one person I really wanna meet that I feel like I would,
[36:16] I'm gonna stutter one day when I meet her. It's just, I'm gonna go blah, blah, blah.
[36:22] You're so cool, I don't know what to say to you, is Arlen Hamilton.
[36:26] Arlen Hamilton. Yeah, see, I Google her way too much.
[36:33] This is Arlen, in case anyone was curious. I know her, you should be friends.
[36:38] And I would like to be friends too. She wrote this book, "It's About Damn Time."
[36:44] And this may be a horrible paraphrase. It's talking about her experience from
[36:53] knowing that she wants to go out and do more to like she was living,
[37:03] she was homeless for a bit, and then working her ass off through networking,
[37:08] through learning, through doing so much to starting Backstage Capital
[37:12] when she wanted to go into VC funding. And it's just so cool.
[37:19] And then there's like she was a band manager for a while and traveled with, I'm just, yeah.
[37:24] There's so much. And hi, Anthony.
[37:27] I'm gonna meet her someday. We're gonna be friends.
[37:31] Well, that sounds really creepy. But I do wanna be friends.
[37:34] But yeah, that is Arlen. In case anybody would like to go
[37:39] become friends with Arlen. You guys are just gonna get the whole Google search
[37:46] so you can search it yourselves later about how amazing. And Sudo, that's somebody that you could connect with
[37:54] is Anthony. Yeah, Anthony, I'm just volun-telling you.
[37:59] (upbeat music) Anthony is my internet big brother,
[38:05] which congratulations, you got married. I've been telling everybody.
[38:10] Yeah, I know, Anthony. You don't connect with anyone.
[38:14] (laughs) He's sarcastic.
[38:20] I mean, yeah. If you wanna see, oh, Anthony.
[38:27] Well, a lot of people are a part of the talk I just, I'm doing.
[38:36] Yep. This is a problem with me live streaming by myself
[38:40] is I get really distracted. That's okay.
[38:44] We are gonna edit it so you guys can see it. Different pieces.
[38:49] You don't get to see the whole thing. You gotta go to the talk.
[38:52] Yeah, Anthony, aren't you part of OSRG as well? You introduced me to everybody, so you should be.
[39:01] Yay. Okay, look, look, look.
[39:09] I have a clip in this talk from my very first stream with Yeray and then overcoming fear of mistakes.
[39:19] Just kidding, making mistakes. And then it's Anthony.
[39:23] I'm very excited about this. Anthony, do you know what clip this is?
[39:27] Like, just by looking at it, do you remember what clip this is?
[39:31] I'm curious. Yep, yep, yes, yay.
[39:43] And then I have Jay in here. And then I have Josh in here.
[39:48] Oh, I got Laura too. I need to tell Laura that she's in this talk.
[39:52] It's funny, I talk about Laura a lot, but I haven't talked to her in a while.
[39:57] Yes, this is a very fast scroll through of this talk about learning TypeScript too.
[40:02] And look, it's from last week. And apparently I'm wearing the same shirt
[40:07] I was wearing last week on Tuesday. This might be my Tuesday shirt, I'm not sure.
[40:12] And yeah, so there's a clip from Josh. I don't think there's any more clips, no.
[40:17] Wee. (upbeat music)
[40:23] Oh, what is that? ♪ Do, do ♪
[40:30] Oh, interesting. I don't know if I can do that.
[40:44] It looks cool. I also...
[40:48] Maybe. I think it could be good practice.
[40:55] It could be good practice. But I do need to do this.
[40:59] What up, Nami? And you are using it for your talk?
[41:07] How easy is it to do this? Y'all, you are distracting me
[41:16] with all the good info and curiosities. We need to stick to this.
[41:22] We gotta stick to this. We gotta get through at least one chapter.
[41:26] Okay. Easy is subjective.
[41:33] That is so true. It is so true.
[41:35] I just started doing Muay Thai and yesterday was my third day.
[41:40] And I was like, I cannot get the like movements. Like what the teacher kept telling me I was trying to do,
[41:48] but my body was not doing what I thought I was doing. And it was really funny.
[41:52] And he was just like, you know, if I try to go swim right now,
[41:56] I can't really swim. It's not gonna get any better each time
[41:59] if I don't keep trying it. And I was like, oh, thanks.
[42:03] Made me feel better 'cause I just started learning swim too.
[42:07] And I am getting better. Okay.
[42:10] System of a Clown. A learning TypeScript type system appetizer project.
[42:17] You'll practice adding in TypeScript type annotations to JavaScript code to find bucks.
[42:24] Please help me. Help me, please.
[42:25] See, look, I'm like already reading it backwards. Help me, please.
[42:31] I planned an elaborate clown-themed surprise party for my best friend.
[42:35] The whole event was planned using a few files of TypeScript code I've written.
[42:40] My friend somehow caught wind of the party and enlisted the clown's help to vandalize the program.
[42:45] Not only did the clowns remove or make incorrect my TypeScript type annotations,
[42:52] they introduced subtle bugs by subtly changing some of the values.
[42:57] Could you please add correct type annotations in the files and fix any bugs detected in my TypeScript?
[43:04] You're my surprise clown celebration's last hope. And I really just wanna say, Josh,
[43:11] like, why so creepy? Data structures and algorithms.
[43:18] Oh, what part of data structures? Who do we need to have on the show?
[43:23] And algorithms. I don't do a lot of algorithms,
[43:27] but I mean, between all the peoples, we could find people to be on the show about algorithms.
[43:33] That would be, we could definitely do that.
[43:39] (soft upbeat music) So many notifications.
[43:47] I hear things. That's a,
[43:49] (laughs) Sorry, I just said, I hear things.
[43:59] And I'm like, it's like, I hear a ghost. It's my sixth, okay.
[44:04] Too distracted. Oh, that's true, Anthony.
[44:10] Consistency and try to solve a few things each day. This is why we're doing this.
[44:17] I don't think I've set that up yet. Oh my God, I have so many repos that I don't use.
[44:31] I think it's on. It's on.
[44:39] Well, that's weird. Oh, there we go.
[44:47] Learning TypeScript. What?
[44:50] Oh, wow, I haven't updated this in a hot minute. And I didn't put all the other stuff in here.
[44:57] Well, let's do that. We don't need Canva.
[45:02] I'm gonna put this in a different browser so I don't close it.
[45:08] (mouse clicking) Look!
[45:14] It was from eight months ago when we were working on chapter two.
[45:20] Oh, on February 3rd. Hey, that's pretty cool.
[45:24] And so if I want to do these. And do these.
[45:37] Y'all, I haven't done this in a hot minute. 'Cause I know I wanna fork it,
[45:47] but I wanna put it in this repo. So I would fork this.
[45:58] I'm gonna think this one through. And then upload to here.
[46:06] To here? I think?
[46:09] I think? I don't know.
[46:13] Let's try it. Let's...
[46:15] Don't fork it as much as I just wanna local. I need to clone it.
[46:25] Or do I fork it? My head hurts.
[46:36] (upbeat music) Yeah, I just wanna copy.
[46:52] Okay, cool. That's, thank you.
[46:54] And then when I upload it, I can upload it to here. Wait.
[47:05] What? 'Cause I wanna put the copy in here.
[47:10] So if I download it, I can just move the files manually. It'll be fine.
[47:15] We'll figure it out. It'll be great.
[47:18] It's gonna be... This is why I need to do this more often.
[47:23] 'Cause my work has been mostly not this stuff for a while. (upbeat music)
[47:34] Okay, cool. And I'm also going to...
[47:43] Copy this one. (upbeat music)
[47:55] Your camera's in the way. Okay, cool.
[48:07] And then do weird shit over here. Why is this so small?
[48:15] (upbeat music) And then projects.
[48:30] I feel like if I just put projects in there, it should work.
[48:35] I don't think so. I don't know.
[48:42] We're gonna find out if I just broke shit. What did I call it?
[48:49] What is this one called? Learning touch grid.
[48:56] Anthony, if you're still there, have you already gone back to work?
[49:09] (upbeat music) 'Cause I thought you guys were like going
[49:15] on a honeymoon and stuff. And I'm like, you've been online a lot.
[49:18] (upbeat music) Oh, okay.
[49:28] Oh, that's so fun. How long are you guys gonna be in Italy?
[49:31] Okay. Oh, no.
[49:36] We wanna do this. We wanna do this.
[49:40] Yay. And we are going to update this.
[49:49] We are going to say, (upbeat music)
[50:03] going to say I'm script projects. What part of Italy are you going to?
[50:19] Why are you not letting me commit? Oh my God.
[50:29] (upbeat music) Why do you look so weird?
[50:37] (upbeat music) Oh, fun.
[50:57] (upbeat music) Why are you not letting me?
[51:07] Oh, there we go. Maybe.
[51:08] (upbeat music) (upbeat music)
[51:14] (upbeat music) (upbeat music)
[51:19] (upbeat music) (upbeat music)
[51:24] (upbeat music) (upbeat music)
[51:30] (upbeat music) (upbeat music)
[51:35] (upbeat music) I put projects within it.
[52:02] So why is it not uploading? (upbeat music)
[52:06] I'm going to figure this out. At the moment, I really hate you.
[52:12] (upbeat music) What up learner?
[52:30] (upbeat music) There are changes.
[52:34] Okay. Maybe that will tell you to stop being so weird.
[52:40] (upbeat music) I uploaded the folder.
[53:01] So I don't understand why you're telling me that it hasn't updated anything.
[53:05] Okay. Look, it's there.
[53:11] And there's a readme. Fine.
[53:13] We will update something on the readme to see if you want to play nice.
[53:16] I don't mind me y'all. I'm just being grumpy at the computer.
[53:24] Yay. I'm happy you're here learner.
[53:32] And I hope this new time works out for you. I'm trying to be consistent about them.
[53:37] Not always, not always the easiest, but I'm going to start having guests again in October.
[53:46] Most of the streams this month are going to be my streams for just getting this set up
[53:56] and my going through all of these chapters and getting my website set up.
[54:04] It's a big reason I'm doing these ones, but I guess we can
[54:08] update this to see if it decides it wants to go through. Yeah, no.
[54:23] 'Cause we've gone through chapter, gosh, we just completed chapter seven.
[54:30] And let's paste this a million times so we can put, I don't think I need that many,
[54:38] but let's see, chapter three, not 32. Chapter four, chapter five, chapter six, chapter seven.
[54:53] Yay. (laughs)
[54:59] Thanks, Anthony. Learner, what do you want to learn about next?
[55:09] Or hey, Anthony, do you know algorithms? We could work on those.
[55:19] Friend. Learner, what is something you want to learn?
[55:26] So that way I have it on the show. Okay.
[55:34] We're updating this 'cause this sounds more fun. And I got stuck, so I'm just gonna update all these.
[55:45] (upbeat music) What?
[56:03] Yay, learner. What's the test for?
[56:15] Let's see. We need to update that text as well.
[56:19] And get these. I feel like we need to do the live stream
[56:36] and then the project. Yeah.
[56:41] And then the project. And let's do summary bullet points.
[56:47] I feel like I was just here. Here we go.
[57:02] (upbeat music) Is it OOP?
[57:17] Because all I read was, "Oop." Like somebody's gonna go, "Oops."
[57:22] (laughs) Have I done that yet?
[57:32] I can't say that my stream is gonna be the most searchable at the moment
[57:43] because I haven't. I feel like.
[57:49] Not that. I don't know.
[57:58] (upbeat music) I feel like I've talked about it, but maybe not.
[58:09] Okay, we need to go here. And, oh, hey.
[58:17] Yes, y'all, I am totally copying and pasting this, but we're gonna ask Josh if he cares.
[58:31] If he does, I will delete it, but it is to help with his stuff too,
[58:36] so hopefully not. Maybe I should hit him up and be like,
[58:40] "Yo, I know you're about to go live, "but could you double check this and see what you think?"
[58:45] Let's just see if we got this so we can commit now. Why are you not letting me commit?
[58:57] I don't understand. Maybe I didn't save it.
[59:04] There we go. Rude.
[59:08] It's pretty rare to work with purely functional languages unless you're at a company specifically,
[59:21] pick something like Elm or Haxel, but the paradigms,
[59:26] is that technically saying paradigms, but it's paradigms.
[59:33] You learn from it are super useful. Is that how you spell paradigms,
[59:39] or is that a different word? And if anybody wants to know,
[59:44] that is the biggest reason that I did not want to start streaming,
[59:48] is 'cause, okay, so it is paradigms. It's like, it doesn't, words are hard in general,
[59:55] but more specifically, because this kind of stuff is rough.
[60:03] How long do I have for this? Oh.
[60:19] (upbeat music) Right, that just went where I just had it.
[60:46] I wanted it right here. There we go.
[60:50] And do these, do these. Put another emoji.
[60:58] Yay, I'm glad your first workshop went well. Let's rewrite this.
[61:12] Rewrite this. Wow.
[61:16] (laughs) Let's rewrite this.
[61:33] 'Cause this is from a while ago. We'll just copy all of this and chat GPT, be my friend.
[61:46] Wait, wrong one. Rewrite for GitHub readme description.
[61:56] Oh, summarize. And go back up.
[62:16] What? Oh, there we go.
[62:20] Is it a good idea to build physical, fun game ideas for kids' intro workshops into tech?
[62:38] I personally think it's a good idea for all ages, because it's not something that,
[62:48] doing something like fun with it makes it easier to learn and associate with as well.
[62:55] I would say associations are one of the biggest things that help me.
[62:59] I'm curious everybody else's thoughts. (soft music)
[63:10] You tried it like a bit of a group game for the first one and loved how it turned out.
[63:31] Yay, that's cool. This is so tiny.
[63:38] Out the episode. What's inside?
[63:53] It's this one. Okay, cool.
[64:06] You also need to go to Josh's website. We have some edits we gotta make,
[64:14] but you're getting somewhere. And I will get this done.
[64:21] I will get this chapter done. Not just prepping everything for it.
[64:25] There we go. Neatly.
[64:30] What are you thinking about doing for your next one, Learner? (soft music)
[64:52] (soft music) (soft music)
[64:58] (soft music) (soft music)
[65:03] (soft music) (soft music)
[65:08] (soft music) (soft music)
[65:25] (soft music) Yes.
[65:44] Okay. And I should probably put my first and last name.
[65:50] Come on, what do we need to do? Ooh.
[65:56] Personally, Legos are like my favorite. Origami, I used to really love origami.
[66:08] I have no idea why I went away from it. I've heard, I've seen some really cool things with Legos
[66:17] on being able to like talk about building concepts, but also being able to showcase like taking away
[66:25] in the building or those types of things. Ooh.
[66:34] Learner, you're doing some cool shit. (soft music)
[66:45] I need this. No, that wouldn't.
[66:50] (soft music) We'll just do HTTPS.
[66:58] (soft music) Link.
[67:04] As we don't know, I'm on my full setup, so that will work. And we need Josh's website.
[67:14] (soft music) But I don't know if he still has it this way.
[67:18] Let's find out. (laughs)
[67:25] So this is Josh's Twitter. And if you go to his Twitter and click things,
[67:35] like his website, 'cause you wanna link it to things, because that would be really cool and helpful.
[67:40] (soft music) Not cool.
[67:56] Not cool, Josh. Only because it's actually really funny
[68:00] and it gets me every time. All right, there's Josh's website.
[68:05] The actual website. (laughs)
[68:11] Adrian, yes. I know, it's like you can't be mad about it,
[68:17] but it's kind of annoying, but it's really funny. And thank you for the follow.
[68:25] Techtronic, tech? Yeah, that's Techtronic.
[68:30] Okay. Just search gold blog and you might find it.
[68:34] Maybe. (soft music)
[68:39] Going back to where I was. Where was I?
[68:43] I was on this thing. Josh Goldberg.
[68:47] I really do wanna get to the chapter. Apparently I should have done all of this like setup
[68:55] of it beforehand, but hey, it's gonna be done because this is what I'm working on this month.
[69:02] Okay, I need to save. And read me for Josh's approval.
[69:10] Oh, I need to actually do one more thing. I need to do italics somewhere.
[69:27] Maybe at the bottom. I don't know yet, I don't know.
[69:36] (soft music) (soft music)
[69:41] This is some weird verbage, but we're gonna go with it to give him an example
[70:11] because that's what we're sending him right now. We can go, I guess that's fine.
[70:19] The last couple of workshops you planned are about how to have fun with Canvas HTML element.
[70:32] Oh, that's cool. (soft music)
[70:36] Commit. Commit.
[70:42] Sync. Yes, go.
[70:46] So I would like to take a screenshot. I feel like I could just send him this, but.
[71:04] Okay, let's send him this. He might be streaming right now.
[71:15] So we're just gonna go with it and we'll, once he has edits, we will update the edits.
[71:30] And let me view the shout out here because I mean, that's a big part of it.
[71:37] Why do you advise against using it? That's interesting.
[71:59] (soft music) Oh, I can't give Josh another shout out
[72:03] for eight minutes and 19 seconds. I didn't know that was a thing.
[72:06] Okay, that's fine, that's fine. We just won't.
[72:11] Rude. (soft music)
[72:16], Oh, thank you for the follow. Yay.
[72:35] (soft music) (soft music)
[72:40] (soft music) [72:42], Okay.
[72:43] (soft music) [72:46], Okay.
[72:51] (soft music) (soft music)
[73:11] Okay. (soft music)
[73:14] (soft music) Oh, I didn't realize this is something,
[73:26] Oh, we got to have Ben back on the show. Maybe it'll let me do a shout out to Ben Myers.
[73:32] (soft music) I hate that even if I follow them,
[73:42] it doesn't show up their full names. Okay, we will work on that in a minute.
[73:45] But he talks a lot about accessibility and they come on to talk about it a lot.
[73:53] And it's definitely something that I appreciate. We can take screenshots, oh, not a movie, not a movie.
[74:05] What do, do any of you have like screen captures that you love?
[74:14] 'Cause once I found out that, wow, now I'm not even gonna remember what it's called.
[74:25] That, what are you called? Why am I spacing what it's called?
[74:28] Snagit, there we go. Snagit is a thing.
[74:32] I freaking love Snagit. It works for so many random things.
[74:37] 'Cause I can go like this and then I can go into Snagit.
[74:45] And yes, it is very tiny. I know it's very tiny.
[74:48] We will zoom in, there we go. And then we can do little arrows.
[74:57] What up, Shane? I am on a Mac, but it doesn't do the same things.
[75:04] At least it didn't used to on being able to do this.
[75:12] Oh, it caused too many hours of pain for work. Oh, geez.
[75:20] I like it because I can type on it. It copied it and paste really easily.
[75:25] Shane, does it let you like, do you comments on it that easy?
[75:33] And Learner, what do you guys use instead? Do you use like what the Mac does
[75:37] or something else? The editor, you can draw and notate it.
[76:07] That's cool. I started using Snagit in like 2020
[76:11] and you couldn't do that much on Mac stuff yet. At least back when I was trying to do it,
[76:16] it was somebody at an EDU company. At the EDU company, wow.
[76:22] They made like training programs that showed it to me and now it's just like so easy.
[76:31] And you use Snagit on Work for Windows. Oh, that's cool that there's an open source version.
[76:39] I mean, not Snagit per se, but like of that kind of software.
[76:43] That's pretty cool. Okay.
[76:46] Why is this one indented weird? [76:51], let's see.
[76:56] That's only one. (silence)
[77:19] Y'all, I realized that I've been streaming for a while when I have to hit play again on my playlist.
[77:30] And I'm still working on getting to what I need to work on. It's cool.
[77:36] It's cool. I will get there eventually.
[77:38] Let's minimize these. So I can see.
[77:47] Chapter one. Recording.
[78:06] Chapter one. Yeah, we'll do that.
[78:15] We'll do this. So like, I know that I can probably do this
[78:33] in a lot easier way, like, you know, filter and paste them, but sometimes just doing it by hand is like,
[78:41] yourself is just satisfying. It's weird, I know.
[78:45] (silence) Whatever.
[78:48] I'm an odd duck. It's okay.
[78:52] (silence) Jane, what are you working on today?
[79:03] (upbeat music) Seven, oh, let's do this.
[79:16] (upbeat music) Four.
[79:30] Three. (laughs)
[79:43] Yes, learner, the underrated things are some of the most satisfying, yes.
[79:47] Work shit. Building SAP tools on the cloud.
[79:52] Same as always. Okay, is it said SAP or is it said SAP?
[79:55] Because I feel like. That's the biggest ones.
[80:03] SAP, okay. What does the SAP stand for?
[80:09] Shane, when are you coming on the show? I made a new friend today, Sudo.
[80:14] He joined the server. They, I should say they joined the server,
[80:18] 'cause I have no idea who anybody is, but they joined the server
[80:21] and they're gonna come on the show. Learner is going to get good Wi-Fi someday.
[80:29] Good Wi-Fi will get to Learner. That is what I'm going with.
[80:33] Good Wi-Fi will get to Learner, and Learner will be on the show someday.
[80:36] (upbeat music) [80:39], oh, wrong spot. (upbeat music)
[80:44], yay. (upbeat music) Learner, I mean, it might be a little weird,
[81:19] but you don't have to be on camera. Like, you can blur it too.
[81:25] There's a few options. Thank you for the follow, dead frames.
[81:33] Okay, that's, do you just see some names and you're just like, how did, what it,
[81:38] like I see dead frames and I'm like, is that drops of frames per second?
[81:44] Like, or is it a different kind of frames? Like somebody dropped their glasses,
[81:49] which by the way, y'all, I ordered new glasses. I finally had my eye doctor appointment
[81:54] and I'm like, I can't order new glasses until I know my prescription hasn't changed that much
[81:59] because I got new glasses and I found out about the transition stuff.
[82:06] And it's weird that A, I didn't do this until I was like 35 and found out that transitions are really helpful
[82:14] because then I don't have to carry around multiple pairs of sunglasses or glasses.
[82:18] But B, I get more cute pairs and these ones are my favorite glasses,
[82:23] but they do not have transitions. So I have more glasses to throw around,
[82:28] to lose around the house. It's gonna be great.
[82:30] It's gonna be fantastic. (hums)
[82:36] (upbeat music) Okay.
[82:54] Josh got back to me, which this is a good one.
[82:59] (upbeat music) (laughs)
[83:05] Okay. You're scared to go to the eye doctor
[83:29] because it became bad, really bad all these years. Last time you went without spectacles
[83:36] was around 18 years back or so. Oh yeah.
[83:41] I am, don't have horrible vision, but it's definitely something that is tough.
[83:50] I like to think that I can go through life without them, but I can't.
[84:00] And contact, (laughs) you guys, I don't know if you can see.
[84:04] Okay. I always get told if I don't wear my glasses
[84:09] that everyone's like, but you look so tired. 'Cause this is naturally,
[84:14] I just naturally have poofier under eyes. Yeah, like no matter what, it's hereditary.
[84:22] It's stupid. And people are like, you look so tired.
[84:25] Are you sick? So it's almost like I don't wanna have LASIK
[84:29] because of this. It was a big thing that when Josh had LASIK
[84:33] and came on the show, that was a big reason I wasn't gonna have it.
[84:41] Yeah, Lerner. I wish everybody knew that, but they don't.
[84:47] Okay. Unions and literals.
[84:56] Chapter three. Oh, that was chapter three.
[85:02] Silly me. Oh, damn.
[85:09] I feel like at least more cool kids are wearing glasses. Like glasses are for the cool kids now.
[85:17] Not just, they used to have,
[85:22] I personally think they used to have a much bigger stereotype around them.
[85:26] I love glasses. They're fine.
[85:29] My chosen? Oh, I didn't update this.
[85:32] Here we go. It's confusing for a moment.
[85:36] Chapter, what, why? Chapter four, objects.
[85:52] Chapter five, functions. Arrays.
[86:02] Chapter seven, interfaces. Oh, no.
[86:18] What's going on, Shane? Tell me, give me the deets.
[86:21] Give me the deets. Yeah, I totally have been streaming, so I have no idea.
[86:27] But I want to know. Should we go look it up?
[86:33] Apple News. Apple's keynote.
[86:53] Okay, I'm really excited about that. Because, okay, my iPad that I use,
[87:04] that apparently I'm not gonna use today doing this stuff, is on a USB-C.
[87:11] I upgraded my headphones, which, y'all, if you get Bose headphones,
[87:17] don't get the touch ones. The touch ones, they're not your friends.
[87:21] Because I, like, when I'm doing stuff around the house, wearing them, they, like, disconnect on me.
[87:25] It's very annoying. It's also, I upgraded those for USB-C.
[87:30] But... All the news, all the news from The Verge.
[87:41] We're not gonna watch the video. Can we?
[87:43] Adding roadside assistance, that's dope. There's an action button.
[87:50] (upbeat music) Okay.
[87:53] Titanium bodies. I do need some new AirPods, because I lost mine.
[88:04] Oh, on the plane. They went to, I think, the Caribbean without me.
[88:11] USB-C, camera. The dynamic island?
[88:15] What? What is that?
[88:18] (upbeat music) What's that dynamic island?
[88:27] Okay. New cool watch with physical motion detection
[88:31] for primary action. Oh, that's cool.
[88:34] Oh! (laughs)
[88:41] That makes more sense, learner. I'm like, what is this?
[88:44] Oh my gosh. Okay, that's the OS.
[88:47] I don't care. As much.
[88:50] I feel like they're... Y'all, I can't upgrade for a while.
[88:55] Oh. I really wanna try these,
[89:01] but I have no reason to get these. I don't have a legit reason.
[89:06] Okay. I'm very excited about this.
[89:12] This is all... Thanks for the call-out, Shane.
[89:15] These are really dope upgrades. And now I really want all the upgrades,
[89:23] but I don't need them right now. We don't need upgrades.
[89:26] All my stuff works quite well. Okay, back to this.
[89:33] We were going to upload all the videos. Videos.
[89:38] Let's go to playlists. Loading TypeScript.
[89:43] No, I wanna see the videos. I mean, the watches still have to have a charger, though.
[89:51] Like the wireless charger. But I agree.
[89:57] It's less cables. Or at least it's all the same cable.
[90:02] Okay. Apparently we're not gonna get to this yet.
[90:08] We will get to it. I am not gonna finish streaming
[90:11] until I'm done with chapter two. Homework.
[90:14] Or at least started it. If I get really stuck, that's different, but.
[90:17] Videos. Ooh, okay.
[90:21] Let's close this. Close this.
[90:28] Thank you. Chapter one recording.
[90:33] Is this the actual chapter one? I think this is the actual chapter one.
[90:43] (upbeat music) So we are going to make sure that
[90:47] that's what's linked in here. Okay, cool.
[90:54] Whatever. Chapter two.
[90:57] If anybody gets bored and has Canva skills, or like, we could use a new thumbnail.
[91:10] I think I do weird thumbnails and I'm not great at them. So if anybody's like,
[91:18] "Yo, I'm bored and I wanna make a new thumbnail for this stream when we talk about Josh stuff
[91:25] and learning TypeScript." That would be dope.
[91:28] I just found out too. Okay, let me see if I can find them.
[91:36] (upbeat music) Okay, I am not gonna end up saying Joe's last name right,
[91:53] but Joe and I just became friends. And I'm so excited because,
[91:59] A, their work with TypeScript course with TypeScript course, yay.
[92:08] And I've always wanted to learn how to speak Spanish. So double yay.
[92:13] And they're in Phoenix. I'm gonna have Phoenix friends.
[92:18] It's gonna be awesome. Here, let's copy and paste your Twitter
[92:23] because you're cool. Jen, focus, focus, focus, focus, focus, focus.
[92:34] Chapter three. I'm also doing this,
[92:46] like I wanna do all of the chapters, but I'm also doing like this side of things
[92:51] because I have a talk coming out next week that I talk about the lessons learned learning live
[92:58] with TypeScript and I'm like, it was brought to my attention.
[93:02] Hey, if you don't have like stuff about TypeScript, that's gonna be really weird.
[93:07] Fair, I don't do a great job at updating my GitHub with all the knowledge I know.
[93:18] It is something to be worked on. I don't understand why some of them have features,
[93:29] some of them don't, whatever. Oh, I'm missing one on the playlist.
[93:34] Whoa, bro, thank you. Oh, maybe because those other ones were live streams,
[93:48] not uploads, that could be it. And videos.
[93:54] And this one needs to be added to the playlist. Add to playlist.
[93:58] Learning TypeScript. Save.
[94:01] I just posted this video yesterday and I'm pretty excited.
[94:08] I'm like a baby content creator. It has two likes.
[94:14] Oh, hey, this one has two likes too. That's exciting.
[94:18] Oh, that's cool. (upbeat music)
[94:29] They're building TypeHero.dev, we'll have to check it out. And for anybody that is, is it from Trash?
[94:41] Okay. Oh, oh, that's cool.
[94:56] Let's go, let's go look at it. Let's go investigate.
[95:00] Investigate. Many features, wow.
[95:09] Okay, that was just fun. Many features, wow.
[95:17] I mean, that's true. Um, Learner, I did this to you
[95:27] like when you were watching the Ivan live stream and I was just like, uh.
[95:32] I don't know what to call you, but Learner. So it gets weird.
[95:42] It gets weird trying to remember everybody's names. For a very long time, Anthony's last name was AJCWebDev.
[95:52] Well, this is exciting though. Let's tweet about it.
[95:58] Fellow. Fellow.
[96:03] Make a post. This looks dope.
[96:09] This looks dope. Yay.
[96:15] 100 emoji, yes. (upbeat music)
[96:24] Thanks for sharing, Learner. No, your name not Learner on, ah, Learner.
[96:36] I always forget how to spell your name on Twitter 'cause it shows up Learner everywhere else.
[96:42] I have to go through my notifications. I'm so bad with names.
[96:51] It's not cool. Ah, found.
[96:59] I may or may not. Yeah, because you're on Discord.
[97:14] I'm gonna put Anthony here too 'cause Anthony, you supported it.
[97:21] Angie Jones is really cool human. You guys should follow her.
[97:25] There you guys got it. Ta-da.
[97:33] Okay, stop with the distractions, Jen. Okay, and...
[97:43] What did this look like? We need takeaways.
[97:54] We need watch the stream. Or playlists.
[98:02] We'll do it under key resources. (hums)
[98:10] What up, Zero? (upbeat music)
[98:21] I've made progress. (laughs)
[98:26] Progress, but not a lot. (gasps)
[98:32] You were subscribed on YouTube? Subscribe on all the YouTubes.
[98:36] Yes, and if you guys ever want to know a good way of supporting people that post on YouTube
[98:42] or even Twitch, if you just join for even a minute and type something on Twitch and be a part of the chat
[98:51] and just leave it on in the background on silent, that's still really helpful.
[98:56] Same with YouTube videos. If you watch it in the first 24 hours
[99:00] and leave a comment like, "This was dope," and like it, it automatically starts helping people's channels grow.
[99:08] So even if you're like, "I don't wanna invest money," invest things in the background.
[99:14] Okay, so we are going to live stream recording playlist.
[99:26] Hey, well, I'm glad I was... Well, stuff is moving.
[99:38] That is a good call-out. Stuff is moving.
[99:42] Um. It's just, they're not...
[99:50] I haven't gotten to where I want to go, but we're getting this page and it's gonna be delightful.
[99:57] And we double-checked with Josh that he's cool with us doing this.
[100:03] Those are important things to have done. (upbeat music)
[100:08] Thank you. That was actually one of my streams,
[100:18] which we did this. And I think this is something that I find very valuable,
[100:26] is even if I don't remember what it was, I remember who it was with a lot of the times.
[100:36] And, but yes, I do need to update my titles and I've been getting there.
[100:44] Thanks, Anthony, for always calling me out for that. Because you can't search things as easily
[100:52] if you don't have their names in them. And there's so many things that don't have descriptions
[100:56] that we will get to. Maybe that's what I'll do one day.
[101:00] Get your link. This is VS Code.
[101:06] Set up with Jay. Okay.
[101:17] All right. And we're almost done.
[101:23] Almost done. We're gonna get there.
[101:29] We are gonna get there. (upbeat music)
[101:33] I need the project names. ♪ Do, do, do, do, do, do, do, do, do, do, do ♪
[101:48] I'm gonna be lazy and copy and paste this. (upbeat music)
[101:59] Do all of you use VS Code? What does like everybody else use?
[102:05] What do you use? I'm curious.
[102:08] (upbeat music) [102:12], (upbeat music)
[102:17] (upbeat music) Chapter three, unions and literals.
[102:48] I think I could do this one, right? (upbeat music)
[103:13] VS Code is your go-to, but you've tried a handful of other IDEs,
[103:17] but none of them cross-compatible like VS Code. I get that.
[103:22] I think that's one of the biggest reasons that I've never gone away,
[103:27] but also I think there's power in other people knowing, you know, like if everybody else is using it,
[103:36] it can make it a lot easier to use. (upbeat music)
[103:41] (upbeat music) Mostly use VS Code these days.
[103:45] Loved NeoVim before you became Windows only and JetBrains for the JVM support.
[103:56] So I've gotten lost in Vim before. (laughs)
[104:06] And I do say it like that because it wasn't my friend.
[104:11] That's what we should do. So we should do this.
[104:16] (hums) No, we shouldn't.
[104:23] Maybe we should. Oh shit.
[104:26] No, we shouldn't. (upbeat music)
[104:30] This is a lot of debating. (upbeat music)
[104:35] (upbeat music) Everybody has their ways that work for them, 100%.
[104:47] Like I find it, it was so weird for me. So Anthony was, I like to call him my internet big brother.
[104:55] He's also like one of the first people I made friends with on, about all of this stuff.
[105:00] And it was weird to not just like do whatever he was suggesting
[105:07] and learning that there's different ways of doing things, which was nice to learn,
[105:13] but also really weird to go against it. And the added benefit of remote development,
[105:21] I've been curious about that because GitHub has something like,
[105:29] it's not co-pilot, right? Co-pilot's the AI thing, I think.
[105:33] I was gonna have Rizelle back on my show for, Rizelle was at GitHub for a long time
[105:39] and she first did a stream with me of like, what is GitHub?
[105:44] And now I realize it's too late 'cause she left and now I need somebody else.
[105:49] Yeah, okay. That's what I was thinking.
[105:53] Yay. (upbeat music)
[105:57] Okay, I'm gonna do these. I feel like I should upload what I have
[106:13] to make sure this doesn't look really stupid. So here's what I like.
[106:28] (humming) Ooh, not what I meant to do.
[106:46] (upbeat music) Stew, I don't even know how to,
[107:10] like where spaces would be. StewYKsoft, I don't know.
[107:19] I hope you know I'm talking to you. What are you up to today?
[107:23] And thanks for joining. And how would you say somebody says your username?
[107:27] (upbeat music) [107:30], Nancy. (humming)
[107:32] two, three, four, five, six, seven, eight, nine, 10. (upbeat music)
[107:39] Nancy. (humming)
[108:06] Ooh, I like this. Why is chapter two indented like that?
[108:14] Oh, you go by stuck. Okay, that makes sense.
[108:26] Okay, well, that's fair. I get it.
[108:33] I would say that's one of the biggest reasons I started live streaming is because
[108:40] it made me do things even if I didn't want to, but that like the anxiety of this stuff
[108:45] has really gotten to me at times. So it's helped having other distractions.
[108:53] But I hope that, yes, it holds me accountable even when I don't wanna be here.
[109:01] Like, it's like, I love being here and I love doing this stuff.
[109:04] It's just not always in the right mindset and it can be hard to be like, okay, I wanna do this.
[109:12] I know I wanna do it. Anyway, that's what I have the hardest time with
[109:19] is reminding myself that I do want to do this. Oh yeah, I get that.
[109:31] For some of my work, I can't do it live and I have to do, but it's weird because a lot of my work for this show,
[109:39] for Teach Gen Tech goes into my real job. We'll go with that.
[109:46] So they work well together, but I know that's not the same for like everybody.
[109:53] What is your job? What do you do?
[110:00] (gentle music) I don't see why I wanna change over here.
[110:04] Do you like? We need to move this.
[110:15] (gentle music) give it some eyeballs.
[110:23] That sounds weird, saying that one out loud, but that's okay.
[110:39] Eyes, who they know to watch it and I.
[110:48] Blockchain engineer for a Web3 company. Dude, I don't think Anthony is still here,
[111:07] but he worked in Web3 for a while. And it was funny because I was just getting into Debrel
[111:13] or like wanting to go into, oh, you are still there. I wanted to get into Debrel
[111:18] and I didn't know anything about Debrel or developer relations.
[111:23] And he was like the third person I talked to. And it was so funny 'cause he took the call from the car
[111:28] and I was like, so like, why are you taking the call from the car?
[111:32] Like, that's weird. Like, aren't you supposed to be professional?
[111:36] It wasn't not professional. It just like, I didn't realize how like different
[111:41] that type of work is. And he was like, cool, I'll help you,
[111:48] but not with Web3 stuff yet. You have to learn just regular code first.
[111:55] I still need to learn Web3. I do want to learn Web3 and more about blockchain.
[112:01] I don't think, yeah, let's see if this helps clean it. I want more emojis.
[112:13] (soft music) Let me see.
[112:21] It's, I mean, I love my job. I fucking love my job.
[112:33] It's one of the hardest jobs I've ever had in my life. (soft music)
[112:40] I don't know. This is gonna do what I want it to do.
[112:48] Babe, have you ever looked into going into DevRel? (soft music)
[113:05] (soft music) Oh, Anthony, other random thing to tell you about.
[113:13] I met one of my dear friends, their new roommate. She's a teacher and she was talking about hitting teaching.
[113:23] And I'm like, yo, you can get into tech. I know lots of teachers that went into tech.
[113:28] And I thought it was cool 'cause I told her about you. (soft music)
[113:35] Oh shit. Are you applying as a DevRel or are you applying
[113:41] as an engineer? What am I?
[113:49] Okay, read me updates. Make it pretty.
[113:57] Is the best update name ever. (soft music)
[114:05] Anything at this point? Oh yeah.
[114:13] I was unemployed for over a year by the time I got my first DevRel job.
[114:18] I think, maybe. Oh.
[114:30] (soft music) Oh damn.
[114:36] Yeah, I get that. I mean, you're always welcome to come on Teach Gen Tech.
[114:40] Like, I feel like it's a good way of people showcasing their skills while teaching the community,
[114:49] which is like one of my favorite parts. I don't do a ton of streams by myself.
[114:54] I am this month because I got to catch up on a lot of stuff.
[114:57] But I normally do two weeks out of the month, two or three weeks out of the month I stream.
[115:06] Like, with Anthony, who's been on the show a million times. Why am I going Twitter?
[115:14] I want to go to YouTube. Go to the YouTubes.
[115:18] Hey look, there's workouts for software engineers. That's fun.
[115:26] (soft music) Okay, so Anthony, you have a playlist.
[115:36] Look, Anthony has a playlist. His own playlist.
[115:40] Like, it can't be named something. No, stop talking to me.
[115:50] Sorry, I hate autoplays with a passion. Like, View Full Playlist.
[115:59] There we go. There's more on this playlist than the two I have on here.
[116:11] But hey, this is the Anthony Campolo playlist. (humming)
[116:23] (soft music) Y'all should go follow Anthony on Twitch as well.
[116:36] He's cool. And you can learn stuff from him.
[116:40] And ask him a million questions. Seven million different ways.
[116:44] It's fun. Okay, we need to do this.
[116:50] And see if I like it yet. Oh, I didn't update it.
[116:57] That would help. Oh, I did.
[116:59] I didn't commit it. Let's see.
[117:07] I think this will make it easier to see. (soft music)
[117:14] (humming) (soft music)
[117:19] (humming) (soft music)
[117:23] (humming) (soft music)
[117:28] (humming) (soft music)
[117:32] (humming) Anybody excited about Hacktoberfest coming up?
[118:04] I'm kind of excited. Oh, okay.
[118:07] I'm pretty excited. I'm actually excited.
[118:10] Not just kind of excited. Read me emoji updates.
[118:21] This is cool. It's fine.
[118:25] Totally fine. (soft music)
[118:28] Refresh. Oh, not super excited,
[118:45] but you usually get a handful of PRs in some of your own repos
[118:52] that announced participation. Okay.
[118:56] Free t-shirts though. I really wanted last year's t-shirt.
[119:00] Your workplace blocks GitHub? Oh, that's sad.
[119:12] Y'all, I am not making this very readable for myself, which is annoying me.
[119:18] I need something to make this readable. I don't know what it is.
[119:26] Hmm. Space theme this year.
[119:43] That'd be cool. Why is there weird spacing in...
[119:50] I don't know. (soft music)
[119:55] Yo, what up everybody from Jason's Raid? Well, thank you, thank you, thank you.
[120:18] We are currently working on updating my readme as one thing, but working on learning TypeScript stuff.
[120:27] Yeah, yeah. Jason, what were you guys streaming about?
[120:34] Yes, I 100% highly suggest Jason's streams because they are always fun.
[120:43] And Jason, you need to come back on the stream 'cause we need to hear about the studio.
[120:51] Like I want to go visit that area of the world just to go see the studio.
[120:57] And if you guys aren't following Jason, he is also very good at TikTok, which you do it all.
[121:04] You magically do it all. That is what Jason does, is magic.
[121:08] I'm pretty sure. Secretly a magician, maybe.
[121:15] But, yes, we are working on my readmes and they're so fun. This readme, at least.
[121:27] And I don't know. I feel like this readme is just really hard to read.
[121:33] Wow, that made a lot of sense. And...
[121:38] (hums) If y'all want to check out learning TypeScript, readme.
[121:50] It's right there. And that's what I'm working on because we just started.
[122:06] Josh has been on the show for, goodness gracious, like eight or nine episodes.
[122:14] And we've been going through his book, "Learning TypeScript." And I haven't been actually like putting it anywhere
[122:20] in good details. And I'm going through and doing all the homework right now.
[122:23] So, yes, the TypeScript docs are great, 100% agree. And that is something that we're just,
[122:31] I'm going through and just putting stuff from the book inside of here.
[122:36] So that way people can find all the details and stuff from each stream, because we've had seven streams.
[122:44] I mean, it's probably good for now. You can get there, maybe.
[122:52] There was one other thing I wanted to update and I think this was it.
[122:58] What are all of you up to? What did you learn on learning with Jason?
[123:05] I don't know if y'all knew this. Granted, I don't think,
[123:08] I don't even know if Jason knows this, that I purposely did not name my stream, "Learn with Jen,"
[123:14] because his is "Learn with Jason." But like one of the first things I did was,
[123:19] "Hey, I just found out you were a person and a thing. "So will you be on my show someday, please?"
[123:24] And he was, which was really cool. Let's see if I can find it
[123:29] because I need to update all of this anyway. (humming)
[123:34] Goodness gracious, holy bananas. Jason hasn't been on the stream since November.
[123:44] That's over six months, that's very strange. And here is that.
[123:57] If y'all wanna go check out his video, it's really dope. It was fun.
[124:02] (upbeat music) (humming)
[124:09] Okay, do this, update. So I can actually go work on
[124:16] what I was supposed to be working on. Did I?
[124:20] Oh, no, that helps. And I think it's like over, ah, that could be it.
[124:35] Yay. For those of you that are still here,
[124:51] I am curious if there was something that you wanted to learn about on Jason's show
[125:00] or more of a newer newbie perspective, what's something that you would want to learn?
[125:07] We were talking about algorithms earlier. The algorithms were a big thing.
[125:28] Here we go. Do this.
[125:45] Oh, yeah. I like that.
[125:57] And thank you for the follow, yay. One of my first streams was with React,
[126:09] and I haven't been doing a ton since then. I'm just trying to think of
[126:17] all the different streams we've done. Don't know if I've done much more than that.
[126:24] This is why I'm slowly getting these updated, because I'm like, I need to actually remember
[126:28] what streams I've done. That would help.
[126:31] Which I think is just gonna be a lot of coming on here and asking chat GPT to help me.
[126:43] Maybe I'll get to it today. Let's see, I have like an hour left
[126:49] before I gotta start heading out, do some things. Oh.
[126:54] That was the other thing. I wanted to change before I stop.
[127:01] Delete. Oh, we don't want that either.
[127:06] Four. The sooner I'm done with this,
[127:13] the sooner I can go work on the homework. I'm so excited.
[127:18] (upbeat music) Oh wow, there's so many different sevens now.
[127:33] I did not know that. That's cool.
[127:36] Oh, I didn't mean six o'clock. Yo.
[127:42] (upbeat music) Doo, doo, doo.
[127:51] (upbeat music) Lets see if this looks any more readable.
[128:00] (upbeat music) Let's see if this looks any more readable.
[128:29] I guess I could do that too. Let's see.
[128:32] Let's put this at the beginning too. (upbeat music)
[128:38] So that way the homework is at the top as well. Yay.
[128:52] (upbeat music) (upbeat music)
[128:57] Is there a homework type? I don't know if that really reminds me of homework.
[129:14] Is there an emoji that reminds y'all of homework? Is it like a pencil?
[129:17] Well, thank you for hanging out and lurking. There we go.
[129:26] Anthony, that one just kind of reminds me of a teacher
[129:44] instead of school. But I mean, homework, that does make sense.
[129:53] Oh, what do you guys think of this pencil icon that I found?
[129:59] You think it should be one of those two instead? I'm gonna update it and then we can change it.
[130:07] (upbeat music) (upbeat music)
[130:12] Sync changes. Yay.
[130:26] (laughs) Thank you, Anthony.
[130:35] Yes, let's do one of those two. Wow.
[130:40] Why, why? But I do think this makes it easier to read
[130:52] if they weren't on the same line. You know, that would help.
[130:59] (hums) (upbeat music)
[131:10] Probably not how you're supposed to form that name, but that's okay.
[131:24] Figure it out in a bit. Okay, let's see.
[131:33] Please, I want to be done with this. I just want to have it figured out.
[131:38] (upbeat music) Oh, it didn't sync.
[131:41] That would help. Yes, you do need to do that, Jen.
[131:45] Yes, please. Please do that.
[131:47] Thank you. I feel like this is easy enough to read.
[131:54] To find the projects, maybe not that one, but I won't update the rest.
[132:03] I won't update until I do the rest of them. (upbeat music)
[132:08] Okay. Do, do, do.
[132:14] Get the rest of their projects and their abouts. Only five more to go.
[132:24] No big deal. (upbeat music)
[132:28], I know that needs that too. Do, do, do.
[132:56] Okay, smallest font offer. Okay, so you have
[133:04] chapter three. Am I just missing chapter?
[133:26] What did I do? Oh.
[133:36] I don't know. I have two fives.
[133:43] That's fine. (upbeat music)
[133:47] Chapter three is unions and literals. Chapter four is objects.
[134:09] I don't know what I was doing. It's fine.
[134:13] (upbeat music) Okay.
[134:19] (upbeat music) This one.
[134:32] (upbeat music) (upbeat music)
[134:38] (upbeat music) (upbeat music)
[135:08] Yes, you need these things. The undefineds.
[135:16] (upbeat music) Okay.
[135:22] (upbeat music) And back here.
[135:27] (upbeat music) (upbeat music)
[135:59] I know I kept saying that I'm gonna get to doing the chapter, but my hunger may not agree with me,
[136:06] which would be very annoying. (upbeat music)
[136:10] (upbeat music) Okay, chapter four.
[136:31] No. (upbeat music)
[136:33] Do, do, do. (upbeat music)
[136:37] (upbeat music) What time is it where all of you are?
[137:06] 'Cause it's noon here, 12, 14. So not too early, not too late.
[137:13] But I start my day at 5 a.m. Like my first call normally starts at 5 a.m., so.
[137:21] Oh, dude, 10 p.m. Geez, I think it's like midnight-ish,
[137:32] or later where Lerner is, if Lerner's still online. (upbeat music)
[137:38] That's late. I can't even imagine.
[137:42] But it's because I talk to people. And let's see.
[137:46] I think Finland is 10 hours ahead from where I'm at now, not nine hours, so yeah.
[137:55] I have my 5 a.m. calls 'cause it's 3 p.m. there. That makes sense.
[137:59] At least time zone, I think, same time area. (upbeat music)
[138:07] Where are you from, Perseus? Did I say it right?
[138:14] Is Perseus one of the great gods, or Roman gods? (upbeat music)
[138:24] (upbeat music) He was the Slayer of Medusa.
[138:38] Okay. Yeah.
[138:46] That's cool. I'm like, I don't know my Greek mythology enough.
[138:55] Like, I know who Medusa is with churning men to stone and with all the snakes.
[139:03] But not enough to be like, yeah, she deserved it, or no, how could he do that?
[139:09] That one, I don't know. What would you say, Perseus?
[139:16] Do you think she deserved it? You probably know the story better.
[139:21] (upbeat music) Type.
[139:49] (upbeat music) Does it take anybody else as long to do read-me's
[140:01] when they're like this? I feel like, I mean, I get that I keep getting distracted,
[140:07] but I feel like it's taking me a really long time. (upbeat music)
[140:13] (upbeat music) Ah, fair enough.
[140:23] That's a good call-out, because she just kept turning everybody to stone.
[140:28] That makes sense. Protects everybody else.
[140:32] (laughs) ♪ Functions ♪
[140:44] Yeah. Well, Perseus, what are you working on today?
[140:58] And anybody else joining? Are y'all up to anything fun?
[141:02] Or working, or co-working? (upbeat music)
[141:08] (upbeat music) (upbeat music)
[141:14] (upbeat music) Two more chapters left.
[141:44] Oh my gosh, I'm gonna get there. It's gonna happen.
[141:52] It's gonna happen. Oh, a cart system for e-commerce website
[142:04] with Next and Redux. I don't...
[142:08] I feel like this is one of the hardest things that I've learned while learning live
[142:14] and also just being new to tech, is it's like,
[142:17] I think that I would know something, or when somebody references it,
[142:23] I'm like, "Oh, I should know that." So it makes me not wanna ask people,
[142:27] but I'm like, "What is Redux?" Is an open source JavaScript library.
[142:41] Y'all, I don't know how long my camera, or my light's been off back there,
[142:44] but I just heard the dog, and she just knocked it over.
[142:48] She like cuddles on the lights, and I'm like, "Dude, that's, isn't that hot?"
[142:53] But that's okay, she's really cute. But...
[142:57] Oh. With React or Angular.
[143:06] Okay. That's cool.
[143:11] Interesting. Oh, that's fancy.
[143:19] Nice. Are they gonna be selling cool things,
[143:29] or you're like, "I don't even care," because they just need to,
[143:33] they just pay you to do it. (upbeat music)
[143:39] Oh. Is that odd?
[143:45] Okay. Why is it odd?
[143:50] Please tell me. Two more chapters.
[144:07] Okay. Embrace.
[144:13] Oh, shit. Ah, thank you for the follow.
[144:31] R4BC31. That just makes me think of like RAV4,
[144:37] which is like a mini SUV-ish car here in the States. Dot dots.
[144:59] Dot dots. And (gasps)
[145:06] Duples. I remember this one.
[145:09] And then I thought it was such a weird word. Generally speaking, Next.js handles getting data
[145:21] via getServerSideProps and getStaticProps. So Redux in Next.js is an interesting combo.
[145:28] Not knocking it, just haven't really heard of it. (upbeat music)
[145:34] Oh. Huh.
[145:37] I'm curious. That's interesting.
[145:41] I learned, so I talk a lot about OSRG, which I feel like we just need to drop it again
[145:49] because it's like the best Discord server ever. And Jacob's the best
[145:54] because he yells at me to do good things in my life. And he does that to everybody.
[146:04] It's lovely. But I feel like we need to talk about this on our next,
[146:10] his Twitter space tomorrow. What is?
[146:16] Side note, everybody go follow Jacob. We need to follow Jacob.
[146:27] Tell him nice things about himself. Oh, you guys don't need to see that.
[146:32] I do need to follow up with people though. Go here, go here.
[146:40] Go follow Jacob. Oh, I can type.
[146:46] I can kind of type. It's fine.
[146:48] It's cute. But we need to tell him
[146:53] that we want to talk about this next time. Okay, I want to talk about it next time.
[147:00] Shane, I just associate you with it. So therefore it's a we.
[147:03] Post, you post. Jacob and the next code and life.
[147:21] - Life. - Space.
[147:27] - Space. - We gotta talk about using.
[147:34] Yeah, code and life. Wait, unless you're like not the person I thought you were
[147:51] and then that would be cool and you should just join code and life.
[147:55] (upbeat music) Which is totally fine too
[148:04] because I get people mixed up all the time, especially 'cause everybody has different usernames
[148:09] in different places and it gets really confusing. Oh, well, that's where I met you
[148:19] so I'm associated with you there. Like I met you there.
[148:24] (upbeat music) Need some state changes without changing page.
[148:39] Some components are related and need client side changes. You'd use Context API
[148:46] but need Redux Thunk and Redux Toolkit. Makes it so much easier.
[148:56] Well, I can not read. I'm like skipping words.
[148:58] This is the frustrating thing about code and just live streaming.
[149:02] I just copy and pasted that already. Look, it's you.
[149:15] (upbeat music) Oh no, it's not you.
[149:23] Please know that, it is not you. It is, I honestly do skip words.
[149:31] And so it makes it really hard when, like a big reason before many of you joined with the raid,
[149:42] I will have to read a lot of this out loud because I skip words.
[149:48] So even when I'm reading out loud, I still skip words because in my mind, if somebody is saying in first person,
[149:56] I mean, I could say they said in first person and read it that way,
[149:59] but I also translate it from first person to talking about that person.
[150:07] And then I mix up my pretenses, but I'm really bad at English as it is.
[150:13] It's, yeah, it's a thing. It is a thing.
[150:19] Where am I going? I need here.
[150:23] Okay, cool. And you need analyzing data.
[150:30] Analyzing data. Generally speaking, if, oh, rude.
[150:51] Oh, it does that. I'm surprised it made it this long.
[150:56] It randomly, thank you for telling me that. Let's see.
[151:02] Yeah, it just like stops in the, like my OBS camera just like tries to take over.
[151:14] Like my camera is still connected and everything, but it's just like, no, bro.
[151:19] Let's see. Okay, let's try this.
[151:25] And this one. Yay, hello again.
[151:30] Yeah, I was like, I don't want to see you guys anymore. You guys can't see me, just kidding.
[151:37] We can't hang out. (laughing)
[151:42] And generally speaking, if you, oh, really?
[151:48] Oh, geez. I was hiding from creating the tweet.
[151:51] You can't prove that it was me. (laughing)
[151:56] That's actually really weird. Yeah, I don't know why, but like it will,
[152:03] it may happen a few times, but normally it will happen like twice and then be fine.
[152:09] And it hasn't been happening at the very beginning when I start using the camera like it used to.
[152:14] But like it happens in a browser, but it doesn't happen in the computer.
[152:24] Like if I have a photo booth up in the background, and just so that way I can see if it stops as well,
[152:32] it doesn't, it's still going just fine, but the computer or the browser like kicks it to OBS,
[152:38] which is just really weird and annoying. That's hey, that's life, but okay.
[152:44] I'm going to read the things. Generally speaking, if you need state across components,
[152:51] like across other UI, other than UI state, it should be moved to the server.
[152:57] If it's UI state, it should be in the context or via local state.
[153:03] I'm going to pretend like I know what that means. I feel like I know what it means.
[153:07] I'm also thinking a lot about when Roy was on the show, we were talking about a lot of this.
[153:21] I have to think about this. I'm going to analyze DNA, analyzing DNA.
[153:36] There we go. How long did it take all of you to learn all of this?
[153:43] Because I get that I've only been in this for a year, but I feel like it is taking forever.
[154:13] Okay, good shout, Jayden. Like, I get like never stop learning,
[154:19] but I feel like it's like also, is it ever going to get easier?
[154:25] Like, I don't know. I don't think that's the right way of saying it,
[154:28] but like, is it ever going to, the concepts? I feel like they start to click and then they don't click.
[154:38] I don't know. What are things that you all recently learned?
[154:43] I'm curious what other people are working on and learning. Ooh, I feel like Rust is really up and coming right now,
[155:02] which only makes me grumpy because their icon is a crab and the company I work for has a really adorable crab.
[155:12] And so people are like, "Is it Rust?" And I'm like, "No, we're cooler."
[155:16] But you know. A recent TIL, the places, place item CSS property.
[155:28] Huh. Uh.
[155:36] I feel like I need to show you guys the pillow of the crabs because they're cute.
[155:49] Hold on just a sec. And maybe I'll fix my light if my dog will let me.
[155:54] Let's see. We'll see if she lets me.
[156:03] Okay, stop that, can I do this? Can I do this?
[156:06] Maybe? Look, I'm just moving the light there.
[156:11] Ah, I'm gonna plug both of them. Okay, we're going, now we're down to no lights on it.
[156:20] It's fine, it's fine. Light.
[156:22] Without hitting my mic, without hitting the mic. Eh.
[156:30] Look how adorable it is. It's so adorable, and it's Ivan.
[156:35] Adorable. But not Rust.
[156:42] Other than that, I have no context of Rust. So.
[156:47] What is Rust about? Is it?
[156:54] No. Thank you, thank you, but no.
[157:01] This crab's name is Rappo, and which is Finnish for crab
[157:07] because I work for a Finnish company. Oh, you guys are still talking about the server stuff.
[157:22] I feel like I'm gonna have to recap this one. Um.
[157:26] Interesting. That is something that I do definitely want to
[157:40] get to, but I'm also just really loving learning about all the databases and data
[157:48] and all things data. They're a lot of fun.
[157:53] Oh, I forgot to do this. Ch-ch-ch-ch-ch.
[157:56] (upbeat music) (upbeat music)
[158:01] (upbeat music) (upbeat music)
[158:06] (upbeat music) (upbeat music)
[158:25] (upbeat music) (upbeat music)
[158:38] Extends. Ch-ch-ch-ch.
[158:46] Learner. That just like totally went over my head.
[159:06] Like the words you're using make sense. Rust is a programming language
[159:10] that doesn't use garbage collectors, yet still lets you not deal with the complexity
[159:17] of manual deallocating memory yourself in potentially undesirable ways.
[159:25] I feel like that's when I start to get really confused is I'm like,
[159:33] wait, how does that compare to like JavaScript then? Because like the only context I have
[159:42] for like something like Golang is, no, no, no, no.
[159:47] Like, it wasn't, I mean, they're all kind of complicated, but.
[159:54] Oh. Anthony, is that for JavaScript then?
[160:03] Or for Rust? That you have to declare how many bytes?
[160:09] I feel like I haven't done that in JavaScript, but I don't know.
[160:12] Okay. Interesting.
[160:16] Huh. Oh, there's so much to learn.
[160:32] Jayden, are you having, if you're still here, are you having fun learning Rust?
[160:35] Like what other languages do you know? Interesting.
[160:46] I will say, I mean, if the school does find out,
[160:52] if y'all end up telling on me, it's okay, because it's been so long.
[160:57] I never got a degree, but I went to school
[161:03] and took a semester and thought, I was like, this is back when I was like,
[161:07] I want to be a developer. And like 12 years ago,
[161:12] and I took a C++ class and it did not click. No matter what I did, I could not get it.
[161:18] Back then, I also didn't know that I was like ADHD or when I learn the best or any of that,
[161:25] or that I'm dyslexic. So I paid somebody off a Craigslist
[161:30] to do my homework for me, but make the mistakes in there for me.
[161:34] Not the proudest moment, but also I still don't understand C++.
[161:40] That's okay. (soft music)
[161:45] Perseus, okay, this sounds weird because I'm not like trying to push the server.
[162:09] I'm just trying to give a resource of, if you wanted to join our Discord server,
[162:14] we talk about this kind of stuff a lot in there too, of like how to use something,
[162:19] what's the best way to use it, like those types of things or resources.
[162:23] So that is, if you want to check it out,
[162:29] you can join that server too. Continue the conversation.
[162:33] (soft music) I think we're almost done with this stupid stuff.
[162:53] (soft music) [162:55]', and I didn't get the URL, did I?
[163:00] No. (soft music)
[163:25] Yeah, all right. So Rust is developed as a systems programming language,
[163:32] which is aimed at creating fast, concurrent and memory made software.
[163:37] It's often seen as an alternative to C, C++. Interesting.
[163:43] Ooh, an interesting one to let you all know about is working on getting,
[163:56] so somebody from AWS has said yes. Google has said yes.
[164:02] Microsoft has said yes. Jacob or somebody else from Cloudflare will say yes.
[164:08] About like having each of them on the show to have us learn about those clouds,
[164:16] like what they do, those types of things. And then I want to see,
[164:19] this is the part that I'm totally not sure about, seeing if they would be open to like having discussions
[164:25] about what's around the clouds, like in comparisons when people are going to them,
[164:31] because I also kind of want to do that for languages someday too, but that could be weird.
[164:38] They both might be weird. (upbeat music)
[164:44] I think we're almost done. Okay.
[165:04] Interfaces, that only has the one. Arrays have the three functions.
[165:13] I don't think I got those ones. Never.
[165:19] Void. Oops.
[165:37] Objects. Objects doesn't have anything.
[165:49] And I don't get const. And doesn't have any, doesn't have any.
[166:02] (upbeat music) No, yeah, no, whatever.
[166:22] Works for me. Right?
[166:27] R-Crab's cuter. Just saying.
[166:33] R-Crab is cuter. Just saying.
[166:43] Let's see. We'll compare them side by side.
[167:00] I'm trying to think of where I can. I don't know.
[167:02] What is our 404? Oh, they don't have it on the 404.
[167:10] That's fine. We will go to, probably way too much into this
[167:19] because I'm going to go to this and then I'm going to go to press kits
[167:24] 'cause that's where my mind goes. Brand guide.
[167:28] (upbeat music) Maybe.
[167:31] Did y'all know that a lot of websites have this because in case you ever need to use their graphics
[167:37] for anything? Just look how cute R-Crab is.
[167:42] Look. I mean, I personally think R-Crab is cuter.
[167:52] It's friendlier. It's like, hey, how's it going?
[167:58] Not, what up? I don't know.
[168:02] What do you guys think? Hughes is cuter.
[168:06] Rust? And I guess that's the other thing.
[168:09] I'm like, this logo makes sense because rust, they have an R with a gear.
[168:15] That makes sense to me. I think crabs are crusty, but not rusty.
[168:23] They're not metal. (upbeat music)
[168:27] Personal opinion here. (laughing)
[168:37] All right, all right. Okay, I think I'm finally done with this stupid read me.
[168:46] Damn it. Yes.
[168:54] This is also what happens when you don't do them for, and wait till you have seven episodes to update it to
[169:00] instead of doing it as you go, like you were planning on. But, hey.
[169:05] Okay, look. It's the most giantist read me ever.
[169:14] Probably not ever. Okay, we got our takeaways.
[169:23] We got the breakdowns, the recordings, the projects. Some of them didn't go exactly right,
[169:33] and I forgot to put the word project in them. Whatever.
[169:37] Probably bold that final thing. If anybody has time or feels like it.
[169:54] Thank you, Shane. That is awesome.
[169:59] If anybody has time and wants to go through and actually make sure that my links go to things
[170:04] and are right, that would be awesome. And I'm really hoping it does not take me this long
[170:13] to get through. Okay, you guys can buy the book.
[170:15] I didn't even know I had this up. Well, let's copy and paste it.
[170:22] Oh, yeah, because it's one of the links I have in the read me.
[170:24] There is the... What I actually wanted to do two hours ago
[170:35] when I started this stream. No big deal.
[170:37] Okay, we're gonna go to System of the Cloud. We got it downloaded.
[170:45] We got it here. What are we doing?
[170:49] Oh, we probably need this. We need this.
[170:52] Maybe, maybe we need that. (upbeat music)
[170:59] (upbeat music continues) (upbeat music continues)
[171:29] And I should already have Node and all of that. And go into CD.
[171:40] Projects. Archive system.
[171:58] /system of a cloud. Okay, fine.
[172:10] We're just gonna immediately go through it over here because projects.
[172:16] Oh, there's a projects within projects. Well, that's okay.
[172:19] My bad. The type system.
[172:27] System of the Cloud. Okay.
[172:30] I'll just copy and paste this one. (upbeat music)
[172:40] (upbeat music continues) Oh, did it?
[173:01] I didn't even realize that. It's definitely, in my opinion, worth the investment.
[173:06] I was like, this makes it, has made it so much easier and I think it's a great way of breaking it down.
[173:14] That's not like the normal, how to say it? Like the normal, a lot of these books are really boring.
[173:23] That's an easier way of saying it. They're so overly academic and dull
[173:30] that it's like, how am I gonna learn? Okay, we don't need this.
[173:38] We don't need Twitter up anymore. We can ignore the Twitters.
[173:42] Oh, and snag it. And these folders, yay.
[173:49] No, we got left. There we go.
[173:52] So, usually let me move these, vice versa. Open the, your editor and the project stress query
[174:11] in your terminal. Run the TypeScript compiler via TSC script
[174:18] within whichever step you're working on. For example, to start the TypeScript compiler
[174:23] on the first step. Oh.
[174:28] (soft upbeat music) Okay.
[174:40] I'm gonna copy this. Key up and see what happens.
[174:48] Okay. Aced.
[174:57] Oh. Why wouldn't I have to?
[175:03] Yeah. Errors are not my friends,
[175:24] but sometimes they think they are. (soft upbeat music)
[175:29] This is really weird, y'all, because I thought I had TypeScript on here.
[175:43] I don't know why I wouldn't have TypeScript on here. Let's go reinstall it.
[175:52] Let's do this one. (soft upbeat music)
[175:57] Maybe I just, you know. Let me try this just to see if I didn't have it installed.
[176:10] Oh. Well, I wouldn't think.
[176:19] I'm just gonna try this and then I'll try what you just said, learner.
[176:25] Oh, here we go. Okay.
[176:28] So I need to update things. That's fine.
[176:31] It's cool. It's cool.
[176:33] (humming) Can I go close all of these,
[176:40] because I'm gonna get confused out there a bit. Starting compilation in watch mode.
[176:51] The 01-clowning-around/index.ts 3438 error.
[177:00] TS 2365 operator plus equals cannot be applied to types number and string/number.
[177:12] 34 for let. It feels weird trying to read all of these out loud.
[177:18] Okay. Yes, there is an error.
[177:26] We got the error. That's good.
[177:27] We are seeing what we're supposed to see. Let's move this a little more that way, that way.
[177:48] Huh, step one is going to be drink water first, or energy drink, 'cause these are my favorites.
[177:56] Oh, thank you, learner. I was like watching it.
[178:08] We're doing something. So it's
[178:17] errors updates with your code changes. Okay, that's cool.
[178:21] So that means, let's do it like here, and we'll zoom in.
[178:28] Okay. The step one, clowning around.
[178:41] Oh, yeah. Learner, please do not apologize.
[178:47] A, I'm streaming way longer than I normally do. B, you're on the other side of the world.
[178:53] Go to sleep. Like, I'm so used to like,
[178:58] especially with everyone being in, like a lot of the company being in Europe,
[179:06] and I'm on the farthest, almost farthest east, west, west, there we go, west.
[179:15] I'm used to people having to, you know, bounce early.
[179:20] Oh, hey. Oh, a lot of notifications.
[179:25] Guess I should look at these from time to time. Mm-hmm, mm-hmm, mm-hmm, mm-hmm, mm-hmm, mm-hmm.
[179:48] Oh, my God, all the notifications. Okay.
[180:11] I know, I'm not paying attention to my stream for a second. I gotta, when you've been streaming for three hours,
[180:17] there's a lot to catch up on. Zoom.
[180:20] Yay. New game.
[180:31] Oh, we got one more that I. Oh, yay.
[180:38] Okay. Okay, that was fun.
[180:52] All right, so back to this. Step one, clowning around.
[181:01] The first area of code I'll need you to fix is the activity assignment engine.
[181:10] It repeatedly creates groups of size five to 10 guests. Each group is directed to go to an activity
[181:19] which can hold up to a certain number of them at a time. It looks like the clowns didn't change too much on this one.
[181:27] They mostly just removed a few type annotations and changed one value.
[181:34] Could you please add back any missing type annotations and avoid involving, evolving or implicit anys
[181:43] and fix the wrong value? Okay.
[181:48] So we're gonna go to index.ts, yay. ♪ Doo, doo, doo, doo, doo, doo, doo, doo, doo ♪
[181:57] TS, we want that TypeScript one. That would make sense.
[182:07] Yeah, I'm gonna switch sides so I can see this one a bit better.
[182:10] Okay. And minimize this again.
[182:21] Let remaining guests be 20, while true. And then I really do have too many of these all in one page.
[182:32] ♪ Doo, doo, doo, doo, doo, doo, doo, doo ♪ I mean, fine, you can say it that way.
[182:42] And I haven't looked at chapter two in a while so let's go back and look at it.
[182:50] Type is a description of what a JavaScript value might, JavaScript value shape might be.
[183:03] By shape means which properties and methods exist on a value and what the built-in type
[183:12] of operator would describe it as. (gentle upbeat music)
[183:19] If let's see here. (gentle upbeat music)
[183:38] (gentle upbeat music) (gentle upbeat music)
[183:45] (coughing) (gentle upbeat music)
[184:02] (gentle upbeat music) (gentle upbeat music)
[184:09] (gentle upbeat music) (gentle upbeat music)
[184:15] (gentle upbeat music) (sniffing)
[184:45] (gentle upbeat music) (gentle upbeat music)
[184:51] (gentle upbeat music) (gentle upbeat music)
[184:58] (gentle upbeat music) (gentle upbeat music)
[185:04] (gentle upbeat music) (gentle upbeat music)
[185:11] (gentle upbeat music) (gentle upbeat music)
[185:17] (gentle upbeat music) (gentle upbeat music)
[185:23] (gentle upbeat music) (gentle upbeat music)
[185:30] (gentle upbeat music) The music.
[185:58] Gotta get the music back. (sighing)
[186:04] Okay, now I'm gonna put these all right here. And we can put this one right here.
[186:15] (gentle upbeat music) (gentle upbeat music)
[186:21] (gentle upbeat music) Oh, let's see.
[186:46] (gentle upbeat music) Each group of guests will be size five to zero.
[186:58] (gentle upbeat music) Okay, not gonna lie, y'all.
[187:06] I think three hours in and I'm a little brain dead. (gentle upbeat music)
[187:18] (sighing) I think that what this means
[187:23] is I'm basically gonna have to come back and stream later 'cause I wanna get this done
[187:29] and this is gonna take more thought process, but we got the rest of it set up, which is good.
[187:38] Okay, let's make sure everything is committed. (gentle upbeat music)
[187:46] I don't know if it'll do both if I do it up here. (gentle upbeat music)
[187:53] Yeah, 'cause this is a great commit name. Yes.
[187:56] That's what I don't understand. So weird.
[188:07] (gentle upbeat music) Oh, you're still trying to put, oh, cancel.
[188:14] (gentle upbeat music) I didn't.
[188:18] Okay. (sighing)
[188:31] Okay, I will troubleshoot this stuff in another day because it's just easy non-clicking.
[188:37] It's not gonna happen, which is okay. Which is okay, that's what happens.
[188:42] And thank you to everybody that has come to hang out today. It was fun.
[188:50] It's been rad. I will be back next week,
[188:54] probably working on a lot of this again. I will be streaming from Denver, Colorado.
[189:00] If anybody is gonna be at Denver Startup Week, come hang out with me, say hi,
[189:07] and let's see who we might be able to raid. Let's see.
[189:15] I don't know if anybody's still online. Oh, Josh's, yay.
[189:21] We will raid to Josh. I mean, we've been talking about him enough, right?
[189:29] (laughing) All right, y'all have a wonderful evening.
[189:37] (upbeat music) (upbeat music)
[189:42] (upbeat music) 
