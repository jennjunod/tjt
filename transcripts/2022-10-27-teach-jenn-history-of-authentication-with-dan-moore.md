---
showLink: "https://www.youtube.com/watch?v=HNRiMKdIzZQ"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-history-of-authentication-with-dan-moore"
title: "Teach Jenn History of Authentication with Dan Moore"
publishDate: "2022-10-27"
coverImage: "https://i.ytimg.com/vi/HNRiMKdIzZQ/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:07] Today we have Dan joining us and I'm excited about today. We met at Denver Startup Week,
[00:14] which was, oh goodness, about a month ago now.
[00:18] Y'all, I just want to let you know for especially those going in to DevRel is you can be
[00:26] not technical and really just walk up to people and ask questions. That's what I did and this is how Dan is on the show.
[00:34] Dan, please introduce yourself and what you're going to be talking about today.
[00:38] >> Yeah, Jen, thank you so much for having me. I really appreciate the chance to chat with you today.
[00:44] I think that is good advice for DevRel. You want to be curious and be interested in helping people.
[00:51] I am head of DevRel at a company called FusionAuth. We're a Denver company and what we do is we
[00:58] help developers add authentication into their applications. It's undifferentiated functionality that
[01:05] is a little bit risky and critical to your users, but I always say no one ever said,
[01:11] "Oh my God, what a great logging experience." People just want to get to the features that your application has.
[01:17] Today I'm going to be talking about authentication in general. Don't worry, it won't be a FusionAuth ad.
[01:22] We're going to talk about authentication in a historical sense and some other things too.
[01:26] >> Good morning, homie. Thank you for joining.
[01:31] Yeah, y'all. I also just want to say, I ended up going to a CTO luncheon during Denver Startup Week.
[01:42] I was like, "I don't know if they're going to let me in, but I need food," and so I went.
[01:48] They did and FusionAuth was there, so I ended up talking to a few other members of the team,
[01:56] and I was like, "I don't even understand what this is." I will say you guys have nice shirts.
[02:01] It's very soft, so they're swag, and they have good coffee cups.
[02:07] I will say that, but I didn't know that when I walked up to all of them.
[02:12] >> Actually, real quick, I'm happy to give away a t-shirt to randomly selected stream viewer if they'd be interested.
[02:18] If you'd be okay with that. Okay, cool. Great. >> One stipulation, they need to share the video from YouTube.
[02:25] >> I guess the second stipulation is they need to be in the US or Canada, shipping out to that place in the world is tough.
[02:30] Sorry. Sorry, everyone. >> Yeah. Y'all, share the YouTube video and tag us.
[02:38] It can be me, FusionAuth, and Dan, or at least tag me so I know that you're sharing it.
[02:45] I can tag everybody else. >> Exactly, homie. I'm like authentication is not fun,
[02:53] but I'm like, "Why do we have to?" Okay. Y'all, please ignore my dog in the background.
[03:00] She doesn't know if she's coming or going, and she's driving me bonkers today.
[03:05] She's a regular on the show. Doggo, ma'am, please stop.
[03:11] Well, we'll see if she decides to calm down. Okay. She's not going to calm down. BRB.
[03:20] >> This is how you-all know it's really live. It's really live. >> Especially when my partner works from home.
[03:30] She's like, "I don't know whose office I want to be in, but you guys shut your doors.
[03:35] I want to be where the door is shut." >> Always.
[03:39] >> Always. But I'm actually really excited about this because I learned a lot from your presentation
[03:47] of the history of authentication, and I do want to get into that,
[03:52] but I don't necessarily understand. What is authentication? Please explain.
[03:59] >> Sure. I think the easiest way to think about authentication is when we were all hunter-gatherers,
[04:06] everyone knew everybody else, and I could immediately know if someone was a member of my tribe
[04:13] or a stranger because I recognized their faces and I had grown up with them.
[04:19] When we started organizing the societies and people started traveling more,
[04:24] there needed to be some way to trust people that you didn't know personally
[04:30] or you didn't know through a friend or a friend or anything like that.
[04:33] Obviously, with the Internet, we have that even at a wider scale. So authentication, at its root,
[04:38] is a way for someone to prove their identity to someone who doesn't know them in the sense of a hunter-gatherer.
[04:48] And there's obviously a lot of ways to do it, but at its root, it is a way to know
[04:54] someone is who they say they are, basically. >> Okay. And that totally makes sense.
[05:01] When I think of authentication, I think about, like, SSO, which we're going to knowledge check myself,
[05:11] SSO is single sign-on? >> Correct. >> Yes.
[05:16] And if I understand, like, the example I like to use is when I worked for a corporate company,
[05:23] you would sign into the computer, and therefore the computer would sign you
[05:27] into all of your other applications, email, all of it, you didn't have to log in every single time.
[05:36] >> Yep. >> And then there's, like, Facebook and Google and GitHub
[05:41] that you can use those accounts to log into other products. And then we have things like VPNs
[05:50] and, like, the tokens you got to use and two-factor, and then I get lost.
[05:56] And especially with, like, all the passwords people need, and then, especially in, like, the API world or cloud world,
[06:05] like, there's also a ton of authentication that I'm just like, what?
[06:10] If we're just going in, like, if we were to know about authentication,
[06:15] and you're talking to us like we know what we're talking about, what types of authentication are being used right now?
[06:22] >> Sure, sure. So kind of an easy way to think about it is,
[06:26] well, there's a couple ways to think about it, right? The first is, what steps do I take to prove I am who I say I am?
[06:33] And people in authentication, like people in technology all over the place, love jargon.
[06:38] And so the technical term for that is a factor of authentication. So when you hear MFA,
[06:44] that just means you use more than one way to prove yourself. So the three big categories that are something you know,
[06:52] something you have, or something you are. So an example of something you know is a username and password.
[06:58] Something you have might be, you can prove that you have access to a phone
[07:04] if it gets an SMS message that has a particular code. And so you're proving you have access to the phone,
[07:10] which presumably, or at least to the SMS, the account receiving the SMS,
[07:16] it could not necessarily be a phone, but, and then something you are is an example
[07:22] as like a fingerprint or facial recognition. So those factors are kind of the foundational level.
[07:29] And then things are built on top of it. Like single sign-on is built on top of that.
[07:33] And that's basically kind of a trust relationship between two or more parties.
[07:38] So your computer had a trust relationship with all those applications
[07:43] that once you logged into your computer, all those applications said, oh yeah, we know, right?
[07:48] We know that Jen has logged in. Or as you said, a lot of applications
[07:55] have a trust relationship with Google. So they say, hey, go log in in Google.
[07:59] And if Google comes back and says, you're Jen Janode at foo.com, we trust that.
[08:06] And we're gonna treat you as an authenticated user. So those are kind of,
[08:13] there's multiple layers of the authentication cake, which is as Homi said, right?
[08:19] It's not fun, but I found after a couple of years of it, it's interesting because you start off and you say,
[08:24] oh, it's just an username and password, right? That's pretty easy, but you start to peel this back.
[08:29] And the question of how you prove someone, how you trust someone is who they say they are
[08:36] at scale in a way that is secure, but isn't super painful for the user
[08:42] and is cost-effective for the company is turned out to be a really interesting problem.
[08:48] - And that's something that I'm definitely like, I'm getting way ahead of myself wanting to know about this,
[08:53] but like how it works into like APIs and all of that, because I'm like, I can't picture it,
[09:00] but now I wanna see it like happen. And a lot of that is like skipping way ahead.
[09:05] A, that's totally where my mind goes like half the time, but, and luckily in like having teached you on tech,
[09:12] I have people like you that will just come on and talk about a random topic.
[09:17] And I'm like, cool, we can noodle on that for a while and eventually get there because I'm learning Python
[09:24] from like the very, very beginning and like the details of it.
[09:27] And then everything else I've been like, let's just figure it out as we go.
[09:32] We'll just have a one-off call about it. And I think that's been so fun.
[09:37] So that's why I'm like, I need to take a step back. I can not do that.
[09:40] I need to understand security. - And then a homie just said, agreed.
[09:47] Dan, I'm not sure if it will be such a monster with more understanding, teach us sensei.
[09:52] - Awesome, thank you, homie. That's awesome.
[09:56] - So can you go through more of like how we went through like the tribal recognition
[10:06] or like small group recognition? Not sure how that would be said properly to MFA.
[10:12] - MFA? - Yeah, so talking about some more of the history.
[10:16] - Yeah. - Yeah, sure.
[10:18] So, I mean, I did this presentation and it was not a PhD thesis.
[10:23] So please don't quote me if I get some dates wrong, but it looked like the first form of authentication
[10:29] I was able to find were some clay seals that happened in the Sumerian region in about 3500 BCE.
[10:38] And those are basically clay seals that were rolled onto clay tablets
[10:43] and had a certain pattern. And then you could, when the clay tablet dried,
[10:51] you knew that whatever's on that clay tablet, a contract or like a list of grain or whatever,
[10:56] was attested to by whoever held that seal. So that's an example of authentication
[11:00] by holding something, right? That possession of that seal authenticated the user.
[11:05] And typically that seal was handed out by the ruler. So it was, yeah.
[11:10] - It makes me think of like, and I didn't even think of this
[11:14] during the presentation that you gave, but like how it's like your ID
[11:20] is another form of authentication. And that's kind of,
[11:24] and then Rivet just said, "Anyone has seen a horror movie,
[11:31] "they know they shouldn't mess with any." - For sure, for sure.
[11:35] - Sumerian seals you find. - Not always used for boring contracts, right?
[11:39] Sometimes used for more exciting things. - And I feel like even like Jumanji,
[11:45] like you had to like win your way out of it and authenticate yourself and prove that.
[11:50] Interesting, that is a great like wraparound. I like that Rivet.
[11:56] All right, so we're to the point where there's different types of authentic,
[12:02] in like a seal or a, is it up, was like words,
[12:11] were words before that or after that? But I meant out of context, y'all.
[12:16] Dan, through his presentation was talking about how different people from different areas
[12:22] would use like a secret word or a- - Watch what you're talking about.
[12:29] Oh no, the shibboleth, the shibboleth is what you're talking about.
[12:32] - That one. - Yeah, so it's a funny story.
[12:35] So basically, or well, kind of funny now, but basically the idea was that
[12:40] you can authenticate someone based on who they are. And in this particular case,
[12:44] it was the way they pronounced a word. And so there were two tribes fighting in ancient Israel
[12:49] and this is recorded in the Bible. And they were having a war and there was a river.
[12:55] One side was one tribe's property and the other was the other tribe's property.
[13:00] And so someone invaded them, I think it was the Gileadites and the Ephraimites.
[13:06] And the one side was trying to get back across the river to their side.
[13:11] And the Ephraimites, I think, discovered that the Gileadites said a word differently
[13:16] than the Ephraimites did. And that word was shibboleth.
[13:19] They actually pronounced it sibboleth. And so they were authenticating every soldier
[13:24] who was trying to cross the river and saying, "Hey, say this word."
[13:27] And if they didn't say the word correctly, they killed them.
[13:30] And so that was an example of authentication with very high stakes.
[13:34] And it was like an inherent quality of the particular tribe people, right?
[13:39] Or the particular, the way that they pronounce those words. So authentication doesn't just,
[13:44] and both these cases, by the way, are kind of group authentication, right?
[13:48] Like you held the seal because they handed it to you by the ruler or you pronounce the word a certain way.
[13:56] We think of authentication as like a way to identify a single person 'cause it's very common today,
[14:01] but it can be a way to authenticate a group as well. - And that's, because I'm always like, but what's next?
[14:09] How did they move to authenticating computers from words? How did we get there?
[14:17] - So yeah, so the early computer systems, basically when you had access to ENIAC
[14:25] and those other computer systems in the '40s and '50s, the access was the authentication, right?
[14:30] There was no kind of second layer check. If you could put the cards into the card reader,
[14:36] the punch cards, then you were obviously authenticated to be there.
[14:39] So it's worth saying that still authentication happened, it just didn't happen at the computer level, right?
[14:45] There was a security guard probably outside the building. And if you got, they probably checked your ID
[14:50] at that point, right? To your point about IDs.
[14:53] But in the '60s, they started to build these computer systems that had remote access
[14:58] or more than one account, and people were starting to be limited, right?
[15:02] Like some students had a couple hours a week or the professors had more,
[15:08] and people ended up starting to have usernames and passwords. And 1961, I think it was the MIMS system.
[15:18] I'd have to pull up the presentation, but that was the first known instance of a password.
[15:26] And it was, yep, in '61, it was the CTSS, I'm sorry. - We're going through this presentation kind of quickly,
[15:36] just so that way y'all know on a high level thing, because it could take the entire time.
[15:41] But yeah, it's definitely been a very, very fun thing that you said that they,
[15:48] if I remember correctly, the students, like somebody hacked into,
[15:54] like figured out the password so everyone could have more time to use it.
[15:57] - Yeah, so '61 is when the password was invented. And then '62 is when the first password hack happened.
[16:05] So actually one of the students, again, he was a PhD student.
[16:11] He was limited to four hours a week. And so what he did was he found out
[16:16] there was a way to print out the password file. And because the password file wasn't accessible,
[16:21] 'cause they were protecting it to some extent, but so he couldn't look at it online,
[16:26] but he was able to actually print it out. And then he shared it around
[16:30] because he wanted to let other people have access to the system.
[16:33] And the funny story is that 25 years later, he apologized to his PhD advisor and said,
[16:40] "Hey, I'm sorry, I was the one who did that." And they didn't take his PhD away from him.
[16:44] So thankfully he was able to do that. But yeah, so it didn't take very long from '61
[16:50] when they invented the password, to '62 when there's the first kind of password hack
[16:56] that happened. - And Revit said that they're impressed
[17:03] that it even took a year. And yeah, I mean, it was brand new back then.
[17:11] So maybe they were just like, what is it? Who knows?
[17:16] Who knows? And that like definitely brings us more towards like,
[17:22] how did it change? How did authentication change when the internet launched?
[17:27] - Yeah, so the internet kind of opened up this whole, I mean, obviously in the '80s, the '70s, '80s and '90s
[17:33] with the PC, there were, you know, local area networks and things like that.
[17:38] But I think the big thing the internet brought is, it brought so many systems online.
[17:44] And I think that, sorry, online, that's the wrong way to put it.
[17:49] It brought so many systems to be more accessible to everybody.
[17:53] And, you know, a LAN, if I steal someone's password in a local area network, you know, I can do some damage,
[18:00] but I have to have proximate physical access to that LAN, right?
[18:04] I need to be able to go into the office. Even if you're a multinational company with LANs and WANs,
[18:11] which are kind of across all your offices, you still need some kind of access to get there.
[18:16] But the internet changed the game because now if I steal someone's password
[18:22] and I'm in Australia or Russia or China or wherever, I can still get access to their systems
[18:29] and their credentials if that system is on the internet. So that brought in the real need for more security, right?
[18:38] So that's bringing in more multifactor options. And obviously I'm talking about kind of
[18:46] from the consumer perspective, the military and business worlds were kind of,
[18:50] were ahead of the consumer perspective in terms of securing accounts.
[18:55] But, you know, the difference between someone be able to like steal your corporate password
[19:00] and steal your banking password, if your banking software is online,
[19:04] that gets to be pretty small in terms of overall impact to the individual, right?
[19:08] Both of those are really, really bad events. - And for, I'm,
[19:15] I feel like LAN and WAN is both like very common knowledge at the same time.
[19:20] I know I forget what they're called. And when you're talking about LAN,
[19:24] it's a local area network. And for, when I think of that,
[19:30] it was a lot of like gaming, like the gaming cafes where you would all have to like
[19:35] work together to play StarCraft or something like that. And, but to your point is companies would have to use it
[19:43] to share information as well. - Or printers.
[19:47] I remember that being a huge thing, like could the printer work, right?
[19:52] And so yeah, so other resources as well as information. - Printers.
[19:58] Oh, yay. Thank you, Josh, for the raid.
[20:02] Josh is gonna be on the show tomorrow. We are actually, I'm just gonna give a shout out to Joshua
[20:09] 'cause he just raided us. But y'all, I got my book
[20:13] and we're gonna start doing TypeScript shit tomorrow. It's gonna be exciting.
[20:18] Okay, so, and Josh, I'll try to get you the, you know, links and stuff,
[20:24] not right before we stream like I did with Dan. You know, I'll work on that today, but thank you.
[20:31] - Thank you, and for everybody that just raided in, A, also join tomorrow, but this is Teach Gen Tech.
[20:39] Today we are talking about authentication from the very beginning.
[20:43] So this one today is gonna be much more theory-based and yay, Jay's here too.
[20:52] Jay said, I have a VS Code extension that I'm working on. You should, I don't know if that was,
[21:00] okay, yes, you guys are figuring that out. Good job.
[21:03] But we were just talking about how we went from somebody hacking into, in 61 that they hacked the,
[21:14] they printed the password to be able to use internet or computer time for their PhD.
[21:21] And then how going from LAN, really LAN and WAN went to getting, you know,
[21:28] having to be in somebody's bubble to get, you know, past their security.
[21:35] And then how did that move to the internet itself? - Sure, so I think what you're talking about
[21:41] is some of the standards that have kind of come out since the internet.
[21:45] Since, you know, I mean, the internet was really started in the '60s and '70s, so I wanna be careful.
[21:50] Like the web is really the big thing, right? In the '90s, that's what really blew up
[21:54] and made it possible to put all these systems online, right? Like, you know, Gopher was a thing, FTP was a thing,
[22:01] and there was certainly authentication in those protocols, but the browser is kind of really where everyone starts
[22:08] to worry about all the passwords they have to keep track of and my passwords getting stolen and other things like that.
[22:14] So, you know, in the '90s and 2000s, there were some attempts to kind of bring some of the things
[22:24] that had been built for those LANs and WAN systems, some of the same concepts, like single sign-on, right?
[22:31] Which was what you talked about at the very beginning. You know, people wanted to let that happen
[22:39] inside browser applications. And it used to be, this is the single sign-on
[22:43] more data sharing, but it used to be like, if I wanted to let you, sorry, if you wrote an application
[22:49] that was, say, a calendar application or a reminder application, and I wanted to let
[22:54] that application have access to my Google Calendar so that it could automatically pull in my calendar
[23:00] and like send me reminders about stuff I needed to do, like feed the dog or get a gift for my wife or whatever,
[23:06] I would have to just type in my username and password into your application, and then your application
[23:13] would like sign in as me to Google Calendar. And that is one, you know, possibly has some breakage,
[23:23] right, because if I ever change my password, then suddenly my application can't get there.
[23:28] But much more importantly, it's a huge security risk because now if anyone attacks your application
[23:34] and gets access to your database of all the username and passwords for Google Calendar,
[23:39] the attacker has all that valuable information. And so single sign-on with the browser is a way for you
[23:47] to delegate that access without providing the full credentials.
[23:53] Does that make sense? - It does.
[23:58] I'm a bit, I told you, I like, I end up bouncing all over with the thoughts and ideas and concepts.
[24:06] The thought process that I'm also like wanting to think about or going with that popped in my head is,
[24:16] so is using SSO more of than that's using an API compared to when you sign on inside of a program
[24:27] because that's just giving them access, therefore it's not an API.
[24:31] - So I'm not sure I understand your question. Are you, can you, can you rephrase that?
[24:36] Or I don't get it, sorry. - Yeah, I'll work on rephrasing it.
[24:40] So in your calendar example, when you had to log into the other calendar
[24:46] to get to your Google Calendar, because you physically went to,
[24:50] gave them your username and password, that's not an API because it is using their username.
[24:58] You gave them your username and password. So they're entering it in where would SSO,
[25:04] like when you use your Google Calendar or your Google account to authenticate,
[25:10] is that an API or is the authentication different? - Yeah, so, you know, taking a little bit of a step back,
[25:19] I remember when I first heard the word API, I had no idea what it actually meant.
[25:23] And the common parlance these days is, it's really just a way to have the structured communication
[25:31] between two computers. - Right. - Sometimes it's JSON,
[25:34] sometimes it's something else. Usually it's over HTTP in the web world.
[25:38] But, so I would say that it's possible, and maybe I'm being overly programmerish and pedantic,
[25:45] but it's possible for both of those to be an API. It really depends on the implementation details,
[25:52] but in the larger context, the security thing is really what I would worry about
[25:59] rather than kind of how the actual access happens. Although the nice thing about standardized SSO is,
[26:07] let me rephrase this, the standardized SSO is definitely gonna be using an API.
[26:13] The other one, the kind of, where you're presenting the username and password,
[26:18] that's less standardized and it's kind of hard to tell what's happening there.
[26:23] - Got it, and thank you for that. I know that they're not necessarily
[26:27] anywhere near each other in like the same, it's just like to understand it,
[26:32] being able to ask these questions, I find very, very helpful.
[26:35] So thank you for rolling with that one. So we've gotten to SSOs now
[26:42] and we have, like you touched on earlier, multi-factor authentication and how,
[26:54] I think that's like also where I'm stuck 'cause I don't know what all is out there
[27:01] or how you implement them. 'Cause I feel like we're more caught up
[27:05] to where we are today, but I don't really know other than the SSO
[27:11] that we were talking about for authentication or username and password kind of thing.
[27:17] - Yeah, so I wrote this thing where I kind of just try to categorize
[27:21] all the different kinds of authentication factors, right? And again- - Let me share your screen
[27:26] really quick so they can see that. - Oh, sure, sure.
[27:27] - Yeah. - Yeah, yeah. So, and I'm sure we can paste this link in the...
[27:35] I'm not sure how to paste the link there. - Perfect, I'll put it in there.
[27:42] - And this is just 5,000 words on authentication factors, whatever.
[27:48] If you need to go to sleep some night, this can be a useful thing.
[27:52] But so again, kind of stepping back to where we started before.
[27:58] Authentication factor is something you have, something you are, or something you know.
[28:03] And username and password is a very, very common one. And the reason why it's very common
[28:08] is it's easy to implement, it's easy to understand. It is unfortunately kind of easy to share,
[28:17] which has pluses and minuses, especially when you talk about the internet world, right?
[28:22] Because something that's easy to share is also easy to steal.
[28:27] And then the way I probably think about implementing this is you need to think about kind of
[28:36] what the ramifications are if an account is compromised. And I always say if it's a recipe website,
[28:42] it probably doesn't matter that much. If it's your bank, it matters a lot.
[28:45] And so you can start to think about the layers of security you wanna put on top of
[28:51] your authentication process to make sure, again, the person who says they're Dan is really Dan.
[28:58] And you need to, as a developer, think about those layers of security
[29:04] because every layer of security is more work for you and it's more work for your user typically.
[29:11] And so you wanna make sure you match those up. I don't know, is that,
[29:14] 'cause we're, do you wanna actually talk about like what an actual implementation of a certain factor would be,
[29:19] or? - Yeah, I'm curious. - Sure, yeah, so let's talk about,
[29:24] let's not talk about username and password, let's talk about sharing,
[29:28] let's talk about a one-time code, right? And so there's a couple of ways you could implement it,
[29:36] but a very common way is using SMS. Now, a lot of people, if it's a high value account,
[29:42] like a bank account or crypto or whatnot, you probably don't wanna use an SMS.
[29:48] And the reason why is there are a couple of attack vectors that are there for it.
[29:52] But for consumer grade application, it's better to have two factors than none,
[29:57] or two factors than just one. So the way that it works is you have this,
[30:03] you need to, as a developer, build some kind of messaging mechanism.
[30:09] So in this case, you're probably gonna use a tool like Twilio
[30:11] or something like that, right? You're not gonna build that from scratch.
[30:14] And then you need to build a user random number generator. And after the login happens with the first factor,
[30:23] you know who the user is, so therefore you can kind of look up their,
[30:27] sorry, take a step back. You need to have an account system,
[30:30] and that account needs to capture that delivery mechanism. So a phone number or an email address.
[30:36] And then when the user logs in, before you allow them full access to your system,
[30:42] you say, "I'm gonna send you a code." You look up their account, you generate a random number,
[30:47] you send the code to them, again, using Twilio, or if it's an email system,
[30:53] you're gonna use like a SendGrid or something like that. Then you need to build a form
[30:57] that actually they can enter that code into. And then once that's done,
[31:02] you have that additional assurance of what, who that person is, right?
[31:09] Because they've previously associated their phone number with their account,
[31:15] and now they've just provided their password and their username,
[31:17] which is what we call the first factor, and they provide an additional factor.
[31:22] And you can do this a couple of ways. You can do it right at login.
[31:25] And then there's also this concept called step-up authentication.
[31:29] And you may know this, like if you're about to send someone money,
[31:32] sometimes you'll be prompted for a password or a code that's sent.
[31:36] And that's because the developers have, again, modeled out the risks,
[31:40] and they've determined that, if you just wanna go read your bank account balance,
[31:44] that's one level of risk. If you wanna send money to somebody else
[31:48] or to somebody new, then that's a different level of risk.
[31:52] And so we're gonna authenticate you again because it's a riskier operation.
[31:57] - How do you choose as, oh gosh, so many questions coming up at the same time.
[32:08] I'm gonna ask both, and then you can go with whatever direction of like,
[32:14] next time that you're on the show, I guess this is the best way to ask,
[32:17] can we go through like how we would build something to authenticate?
[32:22] Like what that would look like if somebody is wanting to get
[32:25] into authentication and security? Like that's one question.
[32:30] And then, oh gosh, like how do we like know where to start
[32:37] as like a big picture? Like if somebody has an idea,
[32:40] how do you know all the different layers that go into it? - Sure, sure.
[32:45] So let me take your first question, which is, honestly,
[32:48] I probably wouldn't wanna show someone how to build authentication like from the ground up.
[32:54] And the reason for that is that there are a ton of great products out there.
[32:59] Fusion Office One, but there are open source libraries as well,
[33:02] like for Python, for Ruby, for Java, for any language that you can think of,
[33:07] there are libraries out there. And I think it'd be a disservice to your watchers,
[33:14] to your listeners to like tell them, actually go out and build your own, right?
[33:18] 'Cause I've built my own and it's so easy to make so many mistakes.
[33:22] So what might be a more interesting thing to do would be like take an open source library
[33:27] and integrate it with something like Fusion Off, or even just look at the library, right?
[33:32] And say, oh, these are some of the choices they've made. Both those would feel more responsible to me.
[33:39] So... - So, okay, then I guess just to ask these questions too,
[33:46] 'cause like if we're looking at something like Fusion Off, like, okay, now I gotta think about this.
[33:55] I'm building an app and I want to use, like create a username and password database creation.
[34:05] Am I going to build that and then bring in somebody like Fusion Off
[34:10] or does Fusion Off actually do that username and password layering as well?
[34:17] - It's your choice, right? So yeah, Fusion Off does do username and password
[34:20] as well as kind of other SSOs and other functionality. I think it really depends on what you see
[34:27] the scope of your application being. If you're, excuse me,
[34:31] if your application is gonna be one thing, right? Like you're building like a portfolio app
[34:36] or something like that, (coughs) excuse me. I would not start with Fusion Off.
[34:42] I would start with a library. And, you know, I know Django has an authentication library.
[34:48] If you're building on Django, Rails has devise, Spring has Spring security.
[34:55] And because it's a toy application, it's fine to intermingle your username and password data
[35:01] with your other data for your application, right? Your recipes, your to-dos, whatever they are.
[35:06] Where you wanna bring in something like Fusion Off. And again, this is not Fusion Off pitch everyone.
[35:11] There are other options out there and I'm happy to talk about them if you have questions.
[35:16] Auth0 is one, Keycloak is another. But if you have a centralized authentication server,
[35:24] it's very similar to having a centralized database server. Right, like there's no reason that you couldn't
[35:30] for every application, write your own data to and from disk, right?
[35:34] You could absolutely do that. And people did that in the '60s,
[35:38] but then they realized that having a centralized store of data let them control access better.
[35:43] It let them see interrelationships between data better. And it let someone else build software
[35:49] that was specifically for managing data. Authentication is the same way, right?
[35:54] Like if you have two applications or three applications, now suddenly you want single sign-on.
[35:59] Maybe you wanna be able to see correlations between how people use different applications.
[36:03] And it's a lot easier to do if you have a centralized identity store
[36:06] than if you have it kind of, application A manages their users,
[36:10] application B manages their users, application C manages their users.
[36:13] Does that help? - It does.
[36:17] I feel like it's one of those things that I might need to noodle on for a bit
[36:23] because of, like it totally does make sense, but I'm like, what is the part that doesn't make sense?
[36:33] Sorry, sorry, y'all. We got a hello in YouTube
[36:36] 'cause we're streaming there too. And I'm like, oh, I should probably go say hi.
[36:40] So what up, Hack? How's it going?
[36:42] And Rivet also, .NET has identity, which they've always liked working with.
[36:51] I think that's, but that's kind of currently where I'm stuck of like, okay, cool.
[37:00] Like all these libraries have something that we can use for authentication,
[37:05] like starting there and then how you build upon it and seeing like different use cases.
[37:10] And again, y'all, this isn't necessarily like FusionAuth specific.
[37:15] It's just FusionAuth because Dan knows FusionAuth. We can have other guests on from other companies,
[37:21] find someone and we'll talk to them too. And so I think that's really where I'm stuck
[37:27] going from theory to practical in a lot of times, like I'm like, cool theory, I can stick with that.
[37:36] I got it. But this one I'm really struggling with.
[37:40] - Sure, well, let me try to phrase it a different way. So if you're starting out
[37:44] and you're just building one application, first thing you do is don't roll your own username
[37:49] and password, go look for .NET Core Identity or again, some of the other options that I've mentioned
[37:56] because what that will do is that will provide a battle tested way for you
[38:01] to implement authentication in your application. And yes, it will be more things to learn, right?
[38:07] 'Cause you're like, oh man, I'm just trying to write this Python application.
[38:09] Why do I have to learn Django authentication? But by doing that, you're gonna follow best practices
[38:15] and your users are gonna be more secure. Now, then the issue becomes cool.
[38:20] So I have my data for my application and I have my user data in the same database.
[38:26] - Okay. - Means it's easy to deploy, it's easy to upgrade, yada, yada.
[38:31] But then what happens if you're like, okay, my application actually is taking off
[38:37] and I wanna add a forum and I wanna add a help desk and I wanna build a second application.
[38:44] You have two choices there, right? The first choice is each of those things
[38:48] has its own user data store, right? And people, if they wanna sign up for application,
[38:55] the second application, they can do that. If people want, if someone needs to file a support ticket,
[38:59] they need to sign up with the support ticket system. That can work, but you quickly get to the point
[39:05] where you have a lot of applications and somebody is gonna get peeved.
[39:12] I was gonna use a different word, but I'll use the word peeved at having to sign up,
[39:18] especially if they're paying you money. They're like, why do I have to sign up for the application
[39:21] and also sign up for the support ticket system? Or more critically, like what if you have an employee
[39:27] who's on the support ticket system and is an admin and they leave and you remove them
[39:32] from the support ticket system, but you forget to remove them from the application.
[39:36] Now you've introduced a security risk. So that is where it makes sense
[39:41] to start to consolidate these. And again, the nice thing is that in 2012, approximately,
[39:50] we've kind of collapsed authentication across different systems and managing these silos
[39:57] is at least in terms of authenticating with a single user identity store is a solved problem.
[40:06] You wanna use a technology called OIDC, which grew out of OAuth, but OIDC was standardized in 2014.
[40:13] And it's just gonna make it easy for all those different systems
[40:18] to talk to one central data store. And then if Dan leaves,
[40:24] you remove Dan from the central data store, you lock his account.
[40:27] Now he can't log into any of those systems that use the identity store.
[40:32] So if your users only have one takeaway from this, it's don't roll your own, use a library.
[40:41] And then the second thing would be, once you get to a certain size,
[40:45] you're gonna start to wanna look at centralizing your identity store.
[40:49] - Does that help? I don't know, I feel like I rambled a little bit there.
[40:53] - It helps, it helps. And also given the example,
[40:56] and then again, I'm great or horrible, no matter which way you look at it,
[41:03] at asking and comparing it to what I've learned so far from other situations of like working at a startup,
[41:12] they may not have like SSO set up like the same as a corporate, like a big corporate place.
[41:21] So they're more than likely like a startup that may not allow you logging into everything,
[41:30] probably isn't using something like OIDC. They're still doing it as multiple small logins.
[41:38] Therefore, it's a lot easier for somebody to keep their content because they didn't put it
[41:44] into the OSS system. - You mean, it's not easy for someone to-
[41:48] - Oh, SSO system, sorry, I said that backwards. - Keep their access, like after they leave
[41:53] or maybe if they switch departments, yes. Although I will say for startups,
[41:57] like a lot of startups I know of delegate to something like Google Workspaces or Office 365.
[42:05] And that can help a lot, right? Because I'm pretty sure when you leave a startup,
[42:11] they're gonna revoke your Google, your Gmail access. That's like kind of top on the list.
[42:15] And so if all you have, all these other apps hanging off of it,
[42:19] that can be a good start for a centralized identity store. It's got its limits and it's really employee focused
[42:25] rather than customer focused, but it can work. Like you're not gonna give every customer
[42:29] who files a support ticket, a Gmail account. - Right, right.
[42:34] - But certainly for the employee space, that's a good place to start.
[42:39] And then, again, this is for y'all that are watching today, this is a theory based one.
[42:51] So we're not doing any coding, but it's also like the conceptualizing of it.
[42:55] And then we will be like working on another project in the future.
[42:59] So please ask questions and go through it. That does bring me to like the startup idea
[43:06] of, because startups are startups, they're starting, they're not as well established.
[43:14] How, because I think the scalability of, it's like one or two people that started,
[43:21] then they add another person, then you have 10 people, 50 people, 100 people,
[43:26] and they may not have some type of SSO or OIDC. Like how does the company implement that?
[43:35] And is it difficult/expensive to do so? - Yeah, so it can depends on,
[43:43] I mean, I think the first thing you need to do is you need to have that pain or the decision
[43:50] to make that choice, right? And so sometimes that's driven by a large external customer
[43:56] who says, "Hey, our security people are asking us to make sure that you have a certain certification,
[44:04] or you can attest to certain things, right? That like, when an employee leaves your company,
[44:08] they're not gonna continue to have access to our data," or something like that.
[44:12] Or maybe there's an incident of some kind. The other thing to think about
[44:17] is that it does offer some business enablement. It's not all pain,
[44:21] because if you have a central identity store, and this is maybe more for the customer side of things
[44:26] than the employee side of things, but marketing loves that, sales loves that,
[44:34] accounting loves that, because there's kind of one place
[44:36] where all your customers live, and you can go look in and do an audit easily
[44:41] and kind of see who's using what, when was the last time company A logged into our system?
[44:48] Anyway, so that's kind of the motivational part, right? There's the good and the bad, right?
[44:57] The pain or the business enablement. And then I guess how you start,
[45:02] it really depends on where you are. We've definitely had customers who've come to us
[45:06] who have totally custom systems, right? They wrote their own,
[45:11] and so from there, it's really a question of identifying where are the users, where's the passwords,
[45:16] what other data do you wanna pull over to the centralized identity store?
[45:20] If, on the other hand, you've used a library, and there's some kind of internal data store,
[45:27] and it's not custom, then what I'd probably look at is
[45:31] seeing if there's a similar, basically doing kind of a, breaking it apart,
[45:38] and so if before you have your to-dos or your recipes and your user data in one database,
[45:46] I'd probably try to break them apart into two and have the internal, have the application use OIDC
[45:53] to interact with that data store. And then you can start to hang other applications
[45:59] off of that data store, and basically you're running your own identity server
[46:04] at that time, and the question then becomes, well, do you wanna be responsible for that PII?
[46:09] Do you wanna be responsible for maintaining that data store that interfaces with everything else
[46:13] using that standard OIDC, or do you wanna swap it out for a system,
[46:18] again, Fusion Auth, Auth0, Keycloak, et cetera, that will still talk to it,
[46:24] but by separating out those steps, I think you make it a little bit easier to swap in
[46:28] rather than trying to change two things at once. Does that make sense?
[46:32] - Some of it, we're gonna go with some of it. - Sorry, please feel free to stop me.
[46:38] I'm obviously passionate about this. Like, if I say something that doesn't make sense,
[46:41] be like, "Hey, Dan, what on earth did you mean by whatever?" 'Cause this is the great part about your show, right?
[46:48] Like, I don't look at the world through new eyes with at least respect to authentication,
[46:55] kicking through leaves in autumn, yes, but like, you know, so I need your assistance to know
[47:02] when I say something that is a concept that maybe doesn't make sense
[47:05] or I'm talking too fast or whatnot. - I think it's definitely something
[47:09] that is also somewhat hard to do as a newbie because it's like, you don't know what you don't know yet.
[47:16] So like what you're saying may make enough sense that it's, that's why I really love doing these
[47:22] and then having people come back on or multiple people from one industry
[47:27] because it's like learning what different pieces of it may connect them together more,
[47:34] but then also may bring up different questions to put two and two together.
[47:38] I would say, and I'm, the entire time you're telling me about this,
[47:44] I'm coming up with like real life scenarios that I'm like, I don't know if this goes into it.
[47:48] So I have another scenario to like run by you of so can someone have,
[47:56] and I think I know the answer to this, like something open source
[48:01] and 'cause like a lot of startups will have like, you know, their own content and then they have open source.
[48:07] It's where they have to like separate everything because they can't have it all in the same area.
[48:17] Would they only have to separate databases or would they have to separate a ton of,
[48:21] like have private repos for like the product and things like that and then public repos
[48:28] for all of the open source stuff, right? - Yeah, so that's a common pattern.
[48:34] I see that people, you know, separate those out, but at the same time, you probably want one data source
[48:42] and you wanna know like, is this person logging into the public repo
[48:49] or the private repo? And again, you're not gonna want those repos
[48:52] to kind of have their own identity stores. And GitHub is the obvious like choice for source code
[48:58] because you can, they've done a good job of like maintain that level of permission structure,
[49:03] but yeah, does that? - That does, that does.
[49:08] And I like it, homies, like this really helps plus one, a bunch to absorb, but makes sense.
[49:14] Yes, I'm glad you feel the same way, homie. And using a library within a framework,
[49:21] NextAuth with Next.js, for example, what are your thoughts? - It's great, yeah.
[49:25] I think I've actually, that came up just the other day 'cause there's actually a FusionAuth integration
[49:30] for NextAuth out there, but they have integrations for lots of other identity providers.
[49:35] And if you're building on Next.js, please use NextAuth because one,
[49:41] it's gonna save you a bunch of time because you don't have to kind of build
[49:44] your own username and password. You will have to learn the library
[49:48] and that's always the trade-off when you're in software development, right?
[49:51] Like you could write your own and know it intimately, but then guess who's responsible for maintaining it?
[49:56] You are, or you learn the library once and then you can use it on multiple projects.
[50:01] So yes, short answer is NextAuth would be a great choice if you're using Next.js.
[50:06] - Okay, and that goes back to your, how you mentioned earlier that like,
[50:15] like Python and like Ruby or Django, they all have their own security libraries
[50:26] or authentication libraries. - Or more than one, right?
[50:29] Like I know JavaScript has like Passport and I know even some of the, like,
[50:36] and this is a good point, what Homey brought up is, it's not just like the languages,
[50:40] sometimes it's the frameworks within the languages, right? Like, I don't know if you could use Django Auth,
[50:47] I doubt you could use Django Auth with a Flask application, for example.
[50:52] So it's not just learning the languages, libraries. In fact, as far as I know, there's no language
[50:59] that has like built into the language authentication stuff, just 'cause it's a high enough level,
[51:05] it's usually built into a framework. - Okay, I am sending this.
[51:12] Y'all, I just Googled it, so yes, this is the Google link,
[51:16] because I think this is also something that I would have gotten really stuck on,
[51:21] would be like, what do you look up to get started on these? And knowing that it's like
[51:27] the language authentication library, that is something that I think would be very, very helpful.
[51:33] I looked up JavaScript 'cause a lot of what I do is JavaScript,
[51:36] but this makes a lot of sense on how you would get started,
[51:42] so, and then proceed through all of it. I feel like I don't know what to ask you next,
[51:51] because I'm like, this is, there's a lot there. Is there something that you think newbies
[52:00] should be asking about, or I haven't asked about that is a good place to start, or?
[52:06] - Sure, yeah, I mean, so I guess, if you're a newbie on a team,
[52:11] I think asking about how they made their authentication choice is an interesting thing, right?
[52:18] Like, what library do they pick? What issues do they have with it?
[52:25] I think that knowing some of the concepts we've talked about around like,
[52:30] what's a factor of authentication? What's multi-factor?
[52:33] What is a library versus like an author, an identity server, identity data store,
[52:44] are things that are useful. I guess the other thing I would say is,
[52:50] I think there's always this desire on my part to kind of peel the layers back and like dig into like,
[53:05] what actually happens when you do a password, when you enter a username and password,
[53:11] like what are the steps? Just like that old interview question of,
[53:15] walk me through every step of an HTTP request, when I request google.com.
[53:19] I think that can be helpful if you're wanting to nerd out, but the bigger thing I would ask
[53:25] that your users all think about is like, spend the time to read about the library
[53:31] and how to use it, rather than worrying about what it's doing on the covers.
[53:36] Because if it's a kind of a known respected open source library or a product like my employer,
[53:42] we think about all those things under the covers. And so the reason for that is so you don't have to,
[53:52] the same way you don't have to think about what happens when you request Google from the browser.
[53:56] So does that, I don't know whether that's helpful. - Yeah, that does.
[54:00] And it makes me think of, so we just started, I say we, the audience and I,
[54:07] we just started using Anki, which is like flashcards to like learn this type of stuff.
[54:14] And like the questions you were asking, I was like, we can put that on flashcards.
[54:20] - Yeah. - And then, oh, go ahead.
[54:23] - Oh, no, no, please go ahead. - I was just gonna say,
[54:26] somebody had a question of if they understand correctly that Auth0 is trying to solve the auth problem
[54:33] as auth solution that works in most situations. - Yeah, so Auth0 is one of the companies that are doing this
[54:40] and I have a lot of respect for them. They started, oh gosh, I wanna say 2011, 2012,
[54:45] and have done a great job of, especially for developers, especially for the customer market,
[54:52] really being in the forefront of that. We like to think we're a great competitor to Auth0
[54:57] and we're less expensive in most cases, but yeah, Auth0 is one of them.
[55:04] I think if you're on AWS a lot, Cognito is another one. Microsoft has their own option.
[55:12] I think a lot of companies are realizing this is a real issue
[55:16] and that by offering this up to developers, again, going back to the very beginning,
[55:23] it's all about taking something that's undifferentiated, that's risky off of developers' plates
[55:27] and letting them focus on the features that people actually really want.
[55:32] And so again, Auth0 is doing a good job. I think Fusionauts has its own strengths.
[55:39] - I'm giggling because y'all, I even said Auth0 because I get that it's a zero,
[55:45] but still looks like Auth0. - So here's the funny thing
[55:50] and this is like totally tangential to authentication. Like this is something I would tell all newbies.
[55:56] Like when you live in a world, like you get enmeshed in it
[56:02] and the things that seem important in that world seem really important to you.
[56:06] I remember when Auth0 got bought by Okta, it was titanic for our company, right?
[56:11] It was a huge issue and not issue, that's the wrong word, huge opportunity, huge change.
[56:17] And we thought it was huge. And then I listened to some podcasts
[56:21] and there was like a passing mention of it, right? Because it wasn't that big.
[56:26] And I think authentication should be that way for most developers.
[56:28] Like they shouldn't really have to care that much about it. And the same is true of so many other things.
[56:34] But I think that just, it was humbling to me to realize, oh, this thing is at the center of my world right now.
[56:39] And yet for most devs, 99% of devs, they don't care. And nor should they.
[56:45] - Fair enough, fair enough. And good call out, Jay.
[56:49] Some people call it that. Folks may not call me out on it, but I don't know.
[56:56] I come up with some funny names. Like I wanna say, I always wanna say Vite and not Vite.
[57:04] And I'm like, no, no, that's not it either. Or I always say CIDC instead of CICD.
[57:12] - CIDC sounds like an awesome rock band or something. - Right?
[57:18] But, and I think it is because of AC/DC. So I mix them up.
[57:23] Yes, please, please start calling them that. I mean, it'll be great.
[57:29] They'll be like, shit, Jen's like, can't say anything. It'll be fine.
[57:34] It'll be fine. Oh, yay.
[57:39] Homie, it's settled. Fusionauth.
[57:42] Auth0. (laughing)
[57:47] It's fine, but Dan came to teach us and obviously is really passionate about it.
[57:51] Yes. And, oh.
[57:55] Name. (laughing)
[58:00] Yes, yes. I like it.
[58:05] I like it. And yes, actually, y'all, that's funny enough.
[58:10] Just timing on all of this. I did have a conversation with Auth0.
[58:14] Yeah, I'm just gonna call them that now. And I was like, yeah, like Fusionauth is coming on.
[58:22] It's great to always get like different experiences from different companies, different points of view.
[58:28] Like even people within the same company, because hearing it multiple times from different people,
[58:34] different learning styles, like it's just the way we learn. And they were like, yeah, no, bro.
[58:39] Like, if we want to, you gotta like prepare questions. So maybe someday we'll do that.
[58:45] If y'all want to do that, like let's do it. Just help me come up with questions.
[58:50] I'm not doing that by myself. I don't know what questions to ask.
[58:53] So instead, we might just have more Dan. Instead of more Cowbell, we'll have more Dan.
[58:59] I like it. And thank you all for coming in today.
[59:06] You're in a store now. Thank you for coming into the store and, oh yeah.
[59:10] Yeah. - Thank you so much for having me.
[59:14] It was really fun to talk about this. And I appreciate the questions from your audience.
[59:19] That was really great. And I do look forward to coming back
[59:22] and maybe walking through some code, doing some implementation stuff.
[59:25] - I am excited about that. I think that's going to be a lot of fun.
[59:29] And then y'all, just as a heads up, you are totally going to get rated over to learn with Jason,
[59:36] just because I think it's so nice when people rate into other channels,
[59:40] even if, you know, no matter how many people it is, it's always like really nice to do.
[59:45] So I'm rating y'all now and we'll have Dan on again, who knows when, but we will keep you posted.
[59:52] Bye everyone. [BLANK_AUDIO]

