---
showLink: "https://www.youtube.com/watch?v=QqPkzy89tBc"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "jenn-makes-tech-adding-database-to-http-jennjunod-com"
title: "Jenn Makes Tech: Adding Database to http://jennjunod.com"
publishDate: "2023-05-17"
coverImage: "https://i.ytimg.com/vi/QqPkzy89tBc/maxresdefault.jpg"
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

[00:00] you you
[00:04] you you
[00:08] you you
[00:12] you you
[00:16] you you
[00:20] you you
[00:24] you you
[00:28] you you
[00:32] you you
[00:37] you you
[00:41] you you
[00:45] you you
[00:49] you you
[00:53] you you
[00:57] you you
[01:01] you you
[01:05] you you
[01:10] you you
[01:14] you you
[01:18] you you
[01:22] you you
[01:26] you you
[01:30] you you
[01:34] you you
[01:38] you you
[01:43] you you
[01:47] you you
[01:51] you you
[01:55] you you
[01:59] you you
[02:03] you you
[02:07] you you
[02:11] you you
[02:15] you you
[02:20] you you
[02:24] you you
[02:28] you you
[02:32] you you
[02:36] you you
[02:40] you you
[02:44] you you
[02:48] you you
[02:53] you you
[02:57] you you
[03:01] you you
[03:05] you you
[03:09] you you
[03:13] you you
[03:17] you you
[03:21] you you
[03:26] you you
[03:30] you you
[03:34] you you
[03:38] you you
[03:42] you you
[03:46] you you
[03:50] you you
[03:54] you you
[03:58] you you
[04:03] you you
[04:07] you you
[04:11] you you
[04:15] you you
[04:19] you you
[04:23] you you
[04:28] you you
[04:35] you hello hello beautiful humans
[04:56] hello hello hello
[05:01] hello hello
[05:09] hello hello
[05:19] hello hello hello and I just saw that Cindy posted on I haven't talked to Cindy in such a long time such a dope human Cindy actually asked about it on LinkedIn right before the stream so I'm going to defer for a second see if you guys can actually see this
[05:55] because do you hide
[06:00] yes oh I don't know if I'm friends friends connected
[06:08] with alien alien alien damn it dude so bad with names but how are all of you doing
[06:20] how's it going today are you excited to see more database stuff I feel like that's majority of what I talk about other than yesterday yesterday I did talk about typescript the other thing I talk about a lot typescript and databases
[06:35] okay we're gonna work on this later it's fine we'll go away from that let's go to github and
[06:52] oh that's awkward
[06:58] github can we be friends uh
[07:06] is github down right now y'all and I just didn't realize that um
[07:19] yes you can see where I go for my source of truth of twitter
[07:28] see if anybody else is uh I think they have a support one no they don't it's just like a regular github
[07:40] I don't know okay
[07:48] well whale
[07:52] incognito window it worked there
[08:00] oh rude
[08:09] well thank you Chris I'm I'm glad it's not just me um but that's really weird I'm kind of trying to like let's go through the google way and see sign in sign in maybe oh
[08:28] you know what no no uh
[08:38] I'm trying to think if I have do I still have firefox on here no
[08:45] not now github
[08:54] not github not circleci there we go hey it likes me here I think
[09:01] that means I have to remember my information which is is really smart you should remember all this you should also have a password keeper that I need to
[09:19] maybe we're thinking about it
[09:27] oh well
[09:32] huh github what's going on bro
[09:41] let's actually put this in the other browser where I have Twitter like actually functioning what up and um yeah
[09:52] hey since we we made a story about you that you're an Australian uh hacker oscrypter do you want to tell us if you're having problems with github on your side of the world
[10:04] yeah I don't like the angry unicorn um today's the sixth oh my gosh today's the 16th y'all oh my goodness
[10:16] um well let's write a tweet I don't know get status anyone else having issues with github
[10:36] I don't know what do you guys do when stuff doesn't work like this my default has become take a picture of it and share with Twitter
[10:50] I do like the angry unicorn though it is uh it's pretty cute it's pretty cute well it's what up Danny tag it with angry okay I will tag it with angry unicorn uh Danny
[11:10] we are talking about that uh right now I was going to work on my stuff but we are dealing with angry unicorns at the moment but it's a cute angry unicorn
[11:24] although I wonder if for those who I don't know if anybody else has experienced this um in Denver Colorado there uh there is a statue of a bronco a blue bronco by the airport
[11:40] a blue bronco Denver airport and it's apparently cursed because it killed the person that made it um Lucifer okay cool that's what it's called is Lucifer but it kind of looks like the angry unicorn
[12:00] I don't know maybe I'm just going a horse looks like a horse but I feel like they both kind of have the grumpy vibe going on anybody else maybe all right well let's uh
[12:21] yes the grumpy unicorn unicorn is adorbs yes yes you are also from Denver I I've only lived here for two years and I can't believe
[12:45] I can't believe I'm already moving away I also uh uh really please tell me you went to my drafts oh it's gonna make me retweet retype it fine anyone anyone else sitting at github air
[13:21] angry grumpy unicorn is cute though oh my gosh but not to fear once I am done with my random tweets and stuff I have other things
[13:46] to work on like database design and you don't need to work on your website and have access to that when you're working on designing your database because we can go do that with everything else
[13:55] I was just also kind of excited to work on like some CSS stuff but meh also to figure out music because that's also been something I've been planning on doing
[14:12] but I haven't yet we should do these first he's really adorable what are all of you working on today anything fun
[14:40] save tweet there we go we didn't make it go away this time that's exciting
[14:57] do you want oh go back there it is this one's like cute but not as cute
[15:27] okay that was fun okay Miro hey Chris I don't know if you've had a chance um to talk to Christian yet
[15:54] he watched our stream from last week and we connected and he's also from Denver he's in San Francisco now but I was like dude that's so cool
[16:05] yay databases Miro that's what I'm doing and Oz you're do you normally work on a couple at a time or do you go like back and forth on stuff
[16:27] or do you focus on one and really quick I feel like I should look at this first because it's weird to me that I don't have music either so we should do that first
[16:39] other people it's working for them I'm jealous Twitter twitch twitch twitch come here what did we sign up for for music that we can actually use
[17:03] channel and in case anybody was curious and wants to set up twitch someday yes you're gonna have a little bit of inception but it's really weird that if you want to go edit your about area
[17:23] you have to go in from this side of things which is very bananas to me like I feel like this is very backwards but it's the way they do it so yay user music
[17:40] oh that totally makes more sense being freelance we've already signed up login login we've connected the channel create your account browsing download
[17:55] well okay once you sign up maybe it'll be like connect my channel I have an account being a hacker from Austin you know hacking today hey I remember my login that is always exciting
[18:27] um y'all live streams ooh can we just no I can't hear myself think um
[18:46] go quieter can you guys hear that though I don't think so because I don't think I'm sharing the screen volume okay let's say
[19:04] share audio ah I know it only lets me select it
[19:20] I will come up with another way let's go back to sharing that one yay
[19:34] and it's weird that I've learned how to do this in OBS now but like you don't do the same thing in StreamYard StreamYard is different
[19:45] music add music
[19:58] let's see ooh you can download it
[20:04] and they do say that you can use this for streaming too so I'm not using this illegally ah thank you yeah I have a ton of different glasses which I should probably actually look into but
[20:26] um like I need to get my eyes checked because I've had the same script for so long okay hide this and pause okay thank you
[20:39] oh but it won't continue playing I think I have to make like a full playlist oh that one was cool too
[20:58] okay we're gonna look into this another time because me trying to do it and wanting to work we're gonna listen to Feeding the Ducks in the background
[21:09] this one did probably um because it's through StreamYard but it only does the one song at a time oh that is really loud really loud
[21:20] oh well we can loop this one song maybe I should find a longer song to loop and then we will get started let's go search
[21:32] that's a decent song I want a long song um
[21:49] like it doesn't show me bye so
[22:06] yeah this one's a new release so that's something um
[22:30] you know what I'm just doing this is very I don't know why I'm getting so confused on this one right now
[22:56] but we will browse the music and try to find something that is longer to repeat like it just lets you like do it like this that's why I'm like I don't know I just want a longer song
[23:12] so it doesn't get super annoying in StreamYard when I have it loop come on we need like a five minute song
[23:23] we got a three minute song okay
[23:31] no no we're gonna put this on the back burner all right that was fun
[23:40] okay let's go with Database Design because I was working on this this weekend and then I haven't looked at it and when I was trying to explain it earlier today
[23:53] it got a bit confusing for me of going what was I working on all right so those who are new on the stream thank you for joining
[24:03] my name is Jen Teach Jen Tech or as I have it of Jen Makes Tech Today and I have two shows one's called Shit You Don't Want To Talk About
[24:12] the other is called Teach Jen Tech and since I have both of them going on I am using Astro to work on my website and I made it so that way this is my homepage
[24:25] you know a little bit about and then I'm gonna have something link out to Teach Jen Tech where it has all of that information of each of the episodes something for Shit You Don't Want To Talk About
[24:38] the podcast have everything go there and then eventually I'm gonna get like a virtual business card for work and that will link out there so when this is all said and done people can go to my name
[24:50] and be able to find all the things and I'm really looking forward to that yet I haven't I figured out what I kind of wanted to do and I was like you know
[25:05] this is as far as I got when Chris and I started of hey these are all things I want as part of my database I think I have no idea how to do any of this like I didn't realize that you have to have different tables
[25:22] and then being able to call each of them which does totally make sense but before last week it didn't really make sense and I am gonna go to YouTube and grab that video
[25:36] because it was good video it's fun stream thank you Chris I really appreciate it Database Basics
[25:56] Here we go and so I learned a lot that day and going to moving on from there I took what we previously had written out
[26:10] which was like a version of this which was like show table or the show is one table channel is one table if we create a table for show then it's gonna go into show ID in the episode table
[26:26] and then episode channel is gonna go into episode ID pulling it from there and then channel ID pulling it from channel totally made sense to me I was like cool I got this
[26:41] yet and this is my graphic of all of this what up Anthony Anthony have you met Christian yet such a dope human more people to get excited about databases
[26:55] okay we'll get there we'll get there let's let's learn one thing at a time one thing at a time if I used a NoSQL database I could have just just shove a JSON object in well
[27:14] okay I was gonna say because I did do JSON files previously if Anthony is GitHub working for you because it wasn't working for me or Chris I don't know why let's see if it works now it works now
[27:32] it was not working though it wasn't working well you know I kind of did that
[27:53] oh okay yay let's see it's working for Gareth I am jealous but what you missed Anthony is the grumpy unicorn and the grumpy unicorn is very cute which I should just go here
[28:20] oh that is fun yay huh all right well
[28:32] oh this is who I was gonna say open in a tab
[28:45] thank you Anthony thank you luckily it's not down and I was trying to show people to where is your website there we go I don't think I've I don't know if aliens on LinkedIn I'm getting distracted to back to where I was earlier
[29:12] this is probably not the best but hey let's see I'm doing this off-screen for a second y'all and then I will be back because yeah I'll just comment this okay this is what we'll do
[29:32] yes I'm making this way too complicated and I'm gonna forget if I don't do this later do you have sex on it
[29:49] uh I like we should just like try to see if oh yay
[30:05] I'm using a theme that boot check out wow there we go that is what I was overthinking way too much and it's now done so we can get over it
[30:27] oh yay all systems operational no more angry unicorns okay we will go here and we will go here and we will do this quit tweet yay
[30:52] I don't know how you say operational why does spellcheck not actually want to work operational
[31:20] yay okay well even though it's that I'm still gonna go back to my Miro board and work on this for a bit
[31:34] because trying to think if these are all like their own tables um like this is a table I feel like I can make this a little clearer let's table show table it's giant okay maybe not that giant
[32:07] channel um
[32:25] I think it was for all of them yeah it was just the apis were being a little taken a little longer but this one was for all of them I'm pretty sure no no no we don't need this anymore go here channel table
[32:55] no go back get back I'm gonna be weird about this uh
[33:03] okay and why am I doing it I don't know
[33:15] episode table hey what up is it ellian or elian I do this every single I feel like I'm gonna do this till you're on the show but did you see that I tagged you is that what you showed up you like magically show up when um but this time I actually did tag you sometimes you just show up magically
[33:40] but uh somebody was talking about using astro and I was like hey I'm actually gonna be working on my site today yay really oh okay so I'm just gonna say the person that has hung out with floor and floor is super cool to uh
[34:09] oh I did tag you on LinkedIn like two minutes ago so that's great timing I and I just closed out your website that is kind of creepy
[34:26] I'm so just I love floor uh for those who don't know floor is my wonderful amazing co-worker and she is in the Netherlands and is just such an incredible human and luckily I've been able to hang out with her twice this year in person and uh yeah she is she's actually a big reason that I kept whoa what are you doing wow okay apparently I can't multitask on that one
[34:55] she's a big reason I was able to keep going when I was in my job search and I actually met her from my job search and delete this it's like resolve delete delete um database normalization
[35:23] does not sound familiar if Chris is still around I feel like Chris would be able to tell us but I don't think so I feel like we talked about normalization like it's something you can do to like clean up okay cool Chris okay
[35:48] oh I'm gonna sidetrack um do I need to worry about normalization yet I don't I don't know if I want to know about that isn't that where it like cleans up the code or not the code but the data in it and that's that's all I got of me trying to guess what or remember what it is
[36:31] do these do these do these do these actions share copy okay that's good I'm happy to hear that I don't need to know it to get off the ground to get this going and
[36:57] astro human that I'm going to end up saying your name a million times wrong and I'm sorry I just sent you the form to fill out to be on the show on Twitter is basically making your tables so reusable and clean as possible oh that's smart
[37:21] and so last week when we when Chris and I were working together we were talking about that to be able and the reason I have these lines we should go actually look up pg admin so I remember what I was doing of because it was using the information we had in a number another table it is called something functional so like that's on it damn it I'm gonna look it up see oh hey
[38:11] okay hey yay I might have deleted it that would have been annoying but I might have
[38:36] am I logged into the right account hmm no I don't think so
[38:52] no okay let's see this log out okay
[39:02] I don't think I deleted it this might come up in a technical interview but if you follow good logical practices understanding the ins and outs of it more trivia than inherent value and Anthony yeah I still really don't know how to do normalization and use databases all the time but that's mainly because you're deploying them and not data model more than data modeling
[39:38] yes and something that I I'm very feel very fortunate that the like sales the sales architect and the customer success manager is letting me like hit them up from time to time because I've been there talking helping me understand like why people may like have multiple use cases of like different databases on there but then also something they first told me about was which like I knew it but I didn't know it of dropping data like you don't necessarily like it's not going to store the data the entire time and I'm like wait what what it's totally logical but I don't know why I hadn't thought of it
[40:32] oh that's good yeah I did code first databases with some of the t3 sack app that Theo has a tutorial on and I was like so during our that Jacob has a Twitter space every week that is called code in life so I got really excited to tell them I was like I did go first and I actually knew what it was it's very exciting.
[41:02] Okay, you have scheduled scheduled maintenance but that doesn't mean that's, I don't think it's this but let's find out. Okay.
[41:12] Ah. Yeah.
[41:18] This I should look at tables that. I think it's this one.
[41:38] It is this one. Okay. Oh, okay, I will look at for that now.
[41:45] Maybe. I just had the other one listed. Save.
[42:01] Yay. Okay, that is not great I do not like all the logins. No, that's not what we want. Oh.
[42:07] Hmm. I don't think this is the one we used. Damn it.
[42:20] Prisma. I like Prisma. It's also what I've been using the most, it's like the OG for me, because I first did it when I was trying to get a job. It is I really love Prisma it's just so easy to use. Even before I didn't like really understand databases, it's so easy.
[42:45] Um, and yes, this is not what I don't like. No, I'm gonna have started from scratch, which is fine, because I thought it was this one but I don't remember which one we used.
[43:10] Drizzle and Kaisele? Are they like Prisma? Like they help connect on the back end? Hmm.
[43:40] Hmm. Hmm.
[43:45] Hmm. Hmm.
[43:50] Hmm. Hmm.
[43:55] Hmm. Hmm.
[44:00] Hmm. Hmm.
[44:03] Okay, fine. We will set up a new one, because I don't think this is it. Let me just kind of set.
[44:15] Can I just delete all of these? Maybe? No, it's not that one either. Remove from server. Yes.
[44:27] And, uh, that one was when I used when I was doing it via Docker. So that was the reason. Yeah, you have no tables.
[44:54] It's a okay though, because until I'm about to start this new one. We don't need to worry about, uh, yeah.
[45:09] No, you can't delete a server. Okay. Because what I will do is luckily when you are just trying a bunch of things, it's okay if you delete things because you.
[45:28] It's not as detrimental. Delete service. There we go.
[45:45] Yes. Yes. Okay. We're going to create a service and it's going to be Postgres and we're going to do the free plan. And we're on the list, blah, blah, blah. And we are going to name this one, teach gen tech.
[46:10] Now, actually, we should call it ngenad-website. Don't do not delete. That is going to be a complicated name.
[46:30] But hey. Oh, hey, everybody. Do you have examples of why like if I were setting up my website just for me, why you might want to do secure any inbound IP addresses?
[46:54] Yeah, it makes a lot of sense when you're working with teams, but I'm just wondering if anybody has ideas of a way that you would talk about this in a skip, skip, skip, skip, skip, skip, finish. Okay.
[47:08] If you're using Prisma, I really recommend doing code first. Oh, that's a good call.
[47:19] Mm hmm. I'm debating that because you are absolutely right.
[47:40] Rivet on doing it that way because it would be cleaner, yet I'm wondering if I'm going to have a hard time like conceptualizing it because I'm doing it from code first instead of the database first. I don't know.
[47:57] Let's try it. And as an inbound connections to database. Yes, you probably won't want to.
[48:09] We don't want to secure individual IPs, but you might want to block some. That does make sense.
[48:15] I need to remember. Yeah, just so that way you guys can see more about it.
[48:29] I'm just trying to think of, is there anything else that I would want to add here? I'm going to take a screenshot of this just in case I need it later.
[48:45] Yeah, that was fine. Okay.
[48:47] Well, then we will. GitHub is working now.
[48:53] Let's see. Desktop code.
[49:01] Oh, I do not like it when it's in this form. More.
[49:05] Columns. Thank you.
[49:08] I'm going to delete this because I don't know how old that is on the website. Why am I moved to trash?
[49:18] Wow. I'm blind right now.
[49:21] We're not seeing things as clearly. Hyper.
[49:26] Pathos is a code first GraphQL library. It's what's used if you had GraphQL and want to do code first approach.
[49:51] Oh. You can do code first with Prisma and with Postgres, and it is.
[50:08] Yes, I'm going to go back up. I think it's NPX push.
[50:18] Let's keep going up. Go up.
[50:21] Go up. Keep going.
[50:23] Who's going to go? Yes!
[50:26] NPX Prisma DB push. Oh, uh oh.
[50:31] I don't like Prisma issues. I got excited because I learned this from doing the T3 stack.
[50:47] Let me show you. Maybe.
[50:50] Maybe. Okay.
[50:52] Hold on. And we're going to see.
[50:57] Okay. I guess I'm referencing this is because this is where I learned it.
[51:19] So. I don't honestly know.
[51:26] Schema. I've been doing it off of the video, so I'm just curious if.
[51:45] I'm not seeing it in here, but. The video itself.
[51:51] I don't want noise. It's like back here.
[52:01] I think it's before Clark. I'm trying to like do this off of memory.
[52:07] And I haven't been able to. Because it's setting it up with.
[52:14] Clerk and for authorization. And then he set up planet scale, but I set it up with.
[52:23] Ivan, just to see if it, it did it. I'm going to do this just so that way I can like, try to see.
[52:30] You know what? Maybe.
[52:41] I don't know. I will look it up later.
[52:43] And see if I can. We'll see if I can figure it out.
[52:45] But I originally learned from watching this video. I will say something that.
[53:07] I wish. Maybe if I open it in YouTube, it will help.
[53:11] No, I don't want to see your ads. Go away.
[53:14] Show more. Ha.
[53:16] Oh, we got to watch the ad really quick, guys. Please stand by.
[53:25] Good news. It's silent.
[53:27] No, I don't want that. I don't want that.
[53:29] Oh, we got to watch the ad really quick, guys. Please stand by.
[53:33] Good news. It's silent.
[53:35] No, I don't want the trial. What I wanted was.
[53:42] No, it was the first one. Anyway.
[53:55] In here, it shows how it's setting it up. And.
[54:01] OK, that is. OK, first question, Anthony.
[54:17] I don't think you're doing it. I like that answer.
[54:24] Yes, because it's way doper on Ivan. The way like I've been working on understanding it is with.
[54:31] And this is, again, me, newer in the industry. So trying to understand why.
[54:37] Why would people go to AWS or Google Cloud or something? The way I've been understood is you can have your database host like put there.
[54:46] And then it will charge you as you expand it in the storage you have. But you have to manage all of like your updates and your security on it.
[54:56] You're all of that. And with Ivan, you don't have to.
[55:00] So especially they just launched their free tier about a month ago. And so that's kind of what I've been learning on.
[55:10] And a big reason. I'm only like three months old at Ivan.
[55:14] So a lot of my learning has been based on using Ivan just so that way I understand the product. Yeah.
[55:26] I don't know what neon is and. OK, that's good to know.
[55:34] I will say with Ivan, it's still hosted on Google Cloud or AWS. Hold on.
[55:51] I'll have to log into another account. I already closed it. Let's go back.
[56:05] OK. I know that I said don't delete on this, but I'm totally going to delete it since it's brand new.
[56:18] Just because I think this will help me be able to explain to you. OK, create a service under Postgres so you can still set up your cloud provider.
[56:32] So it's still being hosted on your cloud provider of your choice. So when we go with a free plan, it's on AWS.
[56:48] And then you can still like choose your service region. And name it literally just going to set it up.
[57:05] No, you're helping me learn. It's really important. And it's hard to when you don't know the ins and outs of databases or like what they all do to be able to talk to it. Granted, I am three months old.
[57:20] And I've only been. Oh, my gosh. Yo, teach gen tech. It's almost a year old. Oh, that's exciting. That is really crazy to think that I didn't know the difference between CSS, HTML and JavaScript three months ago.
[57:37] Oh, just as like a Ram's eye note that has nothing to do with databases is. I'm going to start applying for talks on TypeScript, too.
[57:50] Because that's cool. I like databases and TypeScript. Why? So weird. I never would have imagined that.
[58:05] But yes. Oh, yeah. Talks are the easy part. If I know a topic, I'll talk about it. Talks are that sounds really weird. It's not like they're easy. It's.
[58:19] I don't knowing the tech and how to talk about it is what I have a hard, hard time with, where if somebody wants me to go up and stage and talk to people about stuff. Yeah, I've been handed the mic many times that they're like, hey, Jen, go talk.
[58:34] OK. Cute. I will say that also live streaming and having a podcast makes it a lot easier, too, because then you learn how to work on it on the fly as well. Oh. That's a good call. That's a good call, Anthony.
[59:04] I. It's something that I I don't know why the both two of them like are really cool to me, I still feel like that's weird, but that's OK. Let's skip the step. We are skipping the step. Skip again.
[59:18] OK. And we're going to go to. Oh, now I have to remember how to install the code.
[59:31] Yeah, I'll be this. Get my website on my computer. Maybe.
[60:16] What no. For the sponsor one.
[60:21] Is that what gets the sponsorship on here? That goes to you.
[60:28] I'm not I'm not mad at it. I talk about it a lot and I try to reference that.
[60:41] I don't mind. I think it's a good thing because you're the one who built it. OK, yes, yes, that is something y'all I am working on is I need to start looking for sponsorships because if I get a sponsor who can do like everything post episodes on both on both like shows, then I can get my podcast back.
[61:09] That would be exciting because that's the biggest thing is I'm not great at the pre and post stuff. I can do them. I can't do that. I know how to do them. I don't enjoy doing them.
[61:23] OK, let's do an update. That's fine. Maybe it doesn't take that long. Maybe.
[61:42] Yay. This one.
[62:04] OK, yeah, yeah. Look at the docks. Oh, my goodness.
[62:34] Is this. Anthony, I feel like I'm actually listening to you. I'm going to the docks. You and Josh.
[62:45] I'm giggling because it's kind of funny when. If I like miss something on the book or something along the lines, it was they are important. I just I forget about them a lot.
[63:06] I do, especially when they have a quick start thing. I'm like, oh, quick start. I can just do that. And then I'm not reading through everything. That's the problem. They are so good.
[63:20] I know. I know they are. They are. I want to add it to an existing project.
[63:52] I will say that Astros docks have definitely improved. Or I got more knowledge, but I'm pretty sure it's both.
[64:02] I say it that way because I used to get really stuck, but it was also my first website that I ever built with Astro, my old website. And since then, I actually know what to look for.
[64:15] But it's also just pretty. These docks are pretty. Oh, hey, this one's newer. Learn in reference. That is fun.
[64:26] OK, not what we're doing right now. Stay on task, Jen. Settle Prisma. OK.
[64:41] Yeah, that's not what I wanted. I want these. And go like these. That should be fine.
[64:50] We don't need. Thank you. Go over here. Minimize that. We got the angry unicorn. Oh, I feel like something.
[65:24] I would want to work on at some point would be like Postgres docs, at least as a new user. It was very, very confusing to get started. But I'm also waiting to see if it's something.
[65:40] That I just didn't understand very well. Oh, you should be on his show. You'd be an Anthony show. That would be cool.
[66:15] Well. You're going to build. Wait.
[66:58] Before you do that, Anthony, is your whisper AI thing live yet? Because I want to use it.
[67:08] So could you go build that, please? Thanks. That would be totally happy.
[67:47] Like the I really want to use it so that way I can actually start putting that as part of it. I'm making the databases and stuff. But then I also have to remember.
[68:22] So I am using an existing project. I'm pretty sure I do have guests next week. I don't know. Let me look.
[68:56] Wrong calendar. Wrong calendar. This calendar. What am I doing next week?
[69:07] Oh, hey, I'm doing a talk next week. That's good to know. That's next week.
[69:16] I do have. A veil next week, Monday and Tuesday, Anthony.
[69:28] But I know you've been on the show like a million times, but I finally got like a form. For all this setup. So I'm going to send it to you.
[69:41] And then I'm going to like. Keep track and be like, oh, hey, this person was on the show.
[69:49] I should probably follow up with them. Granted, everybody's really cool and normally comes to hang out.
[69:57] Give me a second. I'm going to say 12 PM.
[70:08] Mountain. So 1 PM your time. I mean, I could do Wednesday if you wanted to, but it would have to be later in the day.
[70:24] My time 1 PM your time. Okay.
[71:01] Oh, yay. Thank you, Chris. Yeah, I know this is taking forever.
[71:06] I'm not always the fastest when doing this by myself. So I'm going to say 12 PM.
[71:14] My time is a okay. Thank you for coming to hang out. Okay.
[71:33] You can now invoke CLI by prefixing it. Okay. That was a prefix. I hate when it does that.
[71:48] Open a new tab. Oh, geez, go to bed.
[72:06] Oh, you can schedule too. So you don't forget.
[72:10] Because it can we can schedule up to like a week out or a month out. I mean, wow. Words help.
[72:23] Thank you for coming to hang out. Yeah.
[73:03] Yeah. Okay.
[73:34] Okay. Okay.
[74:06] Okay. Okay. Okay. We'll go to bed.
[74:30] It was fun hanging out. I will be.
[74:33] Doing the things. Prisma.
[74:37] Schema. Oh.
[74:46] I actually have to think about this. Yes.
[74:50] And do this part offline. I'm so excited. I'm actually properly working on doing something.
[74:55] While streaming. And by that, I mean, like, I'm not throwing something away when I'm done.
[75:01] It's actually like to be in use. So.
[75:10] Yeah. You to do.
[75:39] Okay. Okay.
[75:43] I think. I have that done. Right. We'll see.
[75:53] So if we do save. Okay.
[76:08] Okay. Okay.
[76:44] This means I actually have to go back here. Okay.
[76:47] What are we doing? I need a table and to have these things.
[76:55] A table and things a table and things. Okay.
[77:50] I need a new song. Hello.
[77:54] Hello. Okay.
[78:24] Okay. Oh.
[79:05] This looks like a great one to work with. I'm going to put this right here. So.
[79:21] Stupid. Okay.
[79:27] Okay. Okay.
[79:58] I need a new song. New song. Yes, I am.
[80:05] I hate that it doesn't like let you play like multiple songs on stream yard. I wish it let you.
[80:13] Do that compared to. Only looping one song.
[80:24] We've been listening to this one for an hour, hour and a half, I think. Processing zone.
[80:33] Cool. New background music. Okay.
[80:53] And for those curious, I am. Working on.
[81:02] How I'm going to set up my tables and. Okay.
[81:22] Okay. Okay.
[81:48] Okay. Okay.
[82:23] Okay. Okay.
[82:55] Okay. Okay.
[83:45] Okay. Okay.
[84:43] Okay. Okay.
[84:54] Okay. Okay.
[85:15] Okay. Okay.
[86:05] Okay. Okay.
[86:37] Okay. Okay.
[87:29] Okay. Hi, Graham.
[87:37] And isn't it really. Late there.
[87:47] I'm like, I feel like I keep saying hi to so many of my, my friends overseas and I'm like, but isn't it late?
[87:53] And yes, I'm learning about tags for. Yeah.
[87:59] Oh yeah. That's not too bad. That's not too bad. I go to bed at like eight here.
[88:06] Like really early because I have to leave my first call starts. Around six. So if I aim to go to bed by eight,
[88:17] I'm normally like actually in bed by like nine or 10. Yeah.
[88:40] He did this out. Okay.
[88:50] Yeah. Okay.
[89:15] Okay. Okay.
[89:47] Okay. Okay.
[90:17] Okay. Okay.
[90:47] Oh, yay. Thank you. Thank you, Chris.
[90:53] I appreciate it. I don't even know where my Twitch thing went.
[91:02] Yes, that does help. Okay.
[91:59] Okay. I think relation is going to work.
[92:15] Relation. Oh,
[92:40] Okay. I don't know if this is actually a thing.
[93:33] Okay. Now I need to remember what it's called.
[93:43] Oh, I don't know what it's called. When you reference another table.
[93:54] When a table. References another table.
[94:03] Foreign key. That is what I need. Yay.
[94:06] Okay, so. Foreign key.
[94:12] Prisma schema. Prisma schema.
[94:27] Yes. We're going to get there. We are going to get there.
[94:31] Oh, yes. Yes. I didn't look up.
[94:34] You were absolutely right. Yes, it is.
[94:42] And day. I don't know what time it is, where I am. And yes, it is foreign schema.
[94:47] So I'm very excited about. Foreign schema. Wow.
[94:49] Wow. Foreign key in the Prisma schema is what I'm looking at.
[94:56] Okay. Oh, that's I think what I'm missing.
[95:23] Yes. That it's for.
[95:29] Show. Relation.
[95:36] Fields. And tax.
[95:44] Oh, we're going to close that. Okay.
[96:01] So author ID is combining the two. It's an integer.
[96:09] Okay. Okay.
[96:58] It is a one to one. Okay.
[97:09] So this one's user ID, but then it pulls. Both of them.
[97:16] Okay. Okay.
[97:49] So I was doing this with Prisma and Postgres. And.
[97:57] I felt like I understood it when I was doing it with PG admin. And now that I'm trying to do a code for us, I'm like.
[98:01] Dude, this doesn't make any sense. But Hey, this is, this is part of the learning processes.
[98:06] Learning how to do it. Okay.
[98:35] Okay. It's using show.
[98:47] At relation. Okay.
[99:31] Okay. Okay.
[100:04] Post. Okay.
[100:46] Okay. Oh, I do need not know. And my things.
[101:00] Okay. Okay.
[101:50] Okay. Okay.
[102:28] Okay. Okay.
[103:06] Okay. Okay.
[103:42] Okay. I'm going to get this.
[104:09] I'm going to get this. And handles.
[104:19] Okay. Cause this is referencing this model. It's in relation to tax.
[104:45] Okay. You don't need to.
[105:01] Yeah, I know. Negative.
[105:28] Db push. Okay.
[105:43] So that means it just touched to Prisma. Just what I wanted it to do, but.
[105:51] See if I can. Okay.
[105:58] Understand this, you will create. A new server.
[106:08] Let's name it the same thing we have. Okay.
[106:30] No, no way. Thank you. Okay.
[106:44] I gave it a great name. That way I know that I don't call it something else.
[106:51] And the connection. And.
[107:10] Y'all I'm going to do the password off screen because actually do you want to keep this one. It's kind of fun. It's the first time I've actually wanted to keep it going.
[107:19] Yay. Okay.
[107:33] It's thinking about it. Okay.
[108:09] I'm digging the song we have on repeat right now. Yeah.
[108:42] Okay. I know this is a lot of fun, but I'm working on getting it working.
[108:57] And. See.
[109:05] Oh, I know what I'm missing. This is kind of exciting.
[109:13] I need to do a PG connect for it for Postgres. That may help.
[109:45] Okay. Open.
[110:11] Okay. Open.
[110:21] Desktop code. This one.
[110:25] This one. I'm going to pause the off screen for a second.
[110:49] Okay. Okay.
[111:41] Save. We can follow directions.
[111:50] And hopefully, make this work. So let's go back over here. You guys can see this part this should be fine.
[112:03] Close. This can go back over here. Yay.
[112:16] And this can go over here. Okay, so we're going to do. Yes, close.
[112:28] Import export. We're going to import.
[112:36] This one. Yay. Next.
[112:48] Fine, we will select that group. Finish. Yay.
[112:54] Holy bananas. Oh, my goodness.
[113:13] It's a lot of steps. Which do get easier with practice, but it's like.
[113:19] Okay. Databases.
[113:27] Defaults. Schemas.
[113:40] Okay. Tables, there we go.
[114:18] Yay, it did put the tables in there. So what I was trying to do with. Earlier.
[114:27] So. I feel like I'm kind of cheating because.
[114:34] I didn't know how to do this. So I am. Didn't do it through the properties.
[114:41] Golems. I don't know.
[114:48] Okay, so I did all those rights. And I want to add one.
[114:56] Not this. This is not where you do it. You do constraints.
[115:06] Foreign key. Add.
[115:16] Oh, this is going to make me. Okay.
[115:45] I'm let me go back over here. Okay.
[115:51] So I just like totally named it wrong. It was just supposed to be episode and I called it episode table.
[115:58] You are. Correct. I just named it episode table when I didn't mean to.
[116:06] But Hey, I can fix this here. I believe.
[116:09] Yes, I want to change it. Okay.
[116:19] Here because I wanted to reference. Tags in show and I couldn't get it to do.
[116:29] Yes. Yes. I probably wouldn't have noticed it for.
[116:41] Okay. Can I rename you?
[116:45] I don't know. Properties.
[116:58] Oh, yay. I can rename you right here. But this is going to make me.
[117:07] Oh, this is okay. Okay. Why, why do I have one name table?
[117:13] What is the one called table? Oh, it is this one. Okay.
[117:17] So there were two. Wow. Y'all I am.
[117:22] Doing phenomenal. I'm glad that I saw a different one than the one you even meant.
[117:28] This one is called. Properties.
[117:36] Save. Okay. So we got show channel episode.
[117:44] Cool. We're doing better now. And I need.
[117:51] Episode to reference show tags and show ID. So let's go in here. We're going to go to properties.
[118:02] And we're going to go to constraints for key. And what are we going to name it?
[118:10] Let's make this voice. I can look at them side by side. We're going to name this one.
[118:17] Why is this so difficult to see? Bro.
[118:23] That's annoying. Okay, fine.
[118:27] Let's do this. This up here.
[118:36] Fine. Fine. We will play by your rules. Don't like your rules, but we will play by them.
[118:42] All right. So I want to name this one.
[118:52] Oh. It is.
[119:12] In. Show.
[119:29] Exit. Want to have its own text. So do I have to create that first?
[119:47] Oh, my God. Yes, we said.
[119:52] Cool. Columns.
[119:56] So add a column. Show text.
[120:04] And it's text. Not null.
[120:09] Save. Go back.
[120:26] Constraints. Foreign key.
[120:30] We will add one. This one is.
[120:42] Show tax. It's going to go into show tax.
[120:46] It is referencing. Show.
[120:51] Tax. Add.
[120:58] Show. There is no unique constraint matching, giving keys for reference table.
[121:09] Show. I don't even know what that means.
[121:29] Let's Google. Google is fun.
[121:32] Google is a lot of fun. But.
[121:38] Show tax uses task reference tables. Yes, changes will be lost.
[121:49] Let's go show and go into properties. Columns.
[121:56] ID is primary key. I don't.
[122:11] I don't even know what that means. I don't even know what that means.
[122:15] I don't even know what that means. I don't even know what that means.
[122:18] I don't even know what that means. I don't even know what that means.
[122:21] I don't even know what that means. I don't even know what that means.
[122:23] I don't even know what that means. I don't even know what that means.
[122:25] I don't even know what that means. I don't even know what that means.
[122:27] I don't even know what that means. I don't even know what that means.
[122:29] I don't even know what that means. I don't even know what that means.
[122:31] I don't even know what that means. I don't even know what that means.
[122:33] I don't even know what that means. I don't even know what that means.
[122:35] I don't even know what that means. I don't even know what that means.
[122:38] I don't even know what that means. I don't even know what that means.
[122:40] I don't even know what that means. I don't even know what that means.
[122:42] I don't even know what that means. I don't even know what that means.
[122:44] I don't even know what that means. I don't even know what that means.
[122:46] I don't even know what that means. I don't even know what that means.
[122:48] I don't even know what that means. I don't even know what that means.
[122:50] I don't even know what that means. I don't even know what that means.
[122:52] I don't even know what that means. I don't even know what that means.
[122:54] I don't even know what that means. I don't even know what that means.
[122:56] I don't even know what that means. I don't even know what that means.
[122:59] I don't even know what that means. I don't even know what that means.
[123:01] I don't even know what that means. I don't even know what that means.
[123:03] I don't even know what that means. I don't even know what that means.
[123:05] I don't even know what that means. I don't even know what that means.
[123:07] I don't even know what that means. I don't even know what that means.
[123:09] I don't even know what that means. I don't even know what that means.
[123:11] I don't even know what that means. I don't even know what that means.
[123:13] I don't even know what that means. I don't even know what that means.
[123:15] I don't even know what that means. I don't even know what that means.
[123:17] I don't even know what that means. I don't even know what that means.
[123:20] Save. There's no un-
[123:25] Ugh. Okay, Google, it's fine.
[123:28] You win. You win.
[123:30] We go. Error.
[123:37] Error. Just do it in all caps.
[123:42] There we go. There is no unique constraint.
[123:48] Matching given keys. For reference.
[123:53] Guess we will look at this one. Create table for.
[123:55] For reference. Here we go.
[123:57] For reference. Here we go.
[123:59] For reference. Here we go.
[124:01] For reference. Here we go.
[124:03] For reference. Here we go.
[124:05] For reference. Here we go.
[124:07] For reference. Here we go.
[124:09] For reference. Here we go.
[124:11] For reference. Here we go.
[124:13] For reference. Here we go.
[124:15] For reference. Here we go.
[124:17] For reference. Here we go.
[124:19] For reference. Here we go.
[124:21] For reference. Here we go.
[124:23] For reference. Here we go.
[124:25] For reference. Here we go.
[124:27] For reference. Here we go.
[124:29] For reference. Here we go.
[124:31] For reference. Here we go.
[124:33] For reference. Here we go.
[124:35] For reference. Here we go.
[124:37] For reference. Here we go.
[124:39] For reference. Here we go.
[124:41] For reference. Here we go.
[124:43] For reference. Here we go.
[124:45] For reference. Here we go.
[124:47] For reference. Here we go.
[124:49] For reference. Here we go.
[124:51] For reference. Here we go.
[124:53] For reference. Here we go.
[124:55] For reference. Here we go.
[124:57] For reference. Here we go.
[124:59] For reference. Here we go.
[125:01] For reference. Here we go.
[125:03] For reference. Here we go.
[125:05] For reference. Here we go.
[125:07] For reference. Here we go.
[125:09] For reference. Here we go.
[125:11] For reference. Here we go.
[125:13] For reference. Here we go.
[125:15] For reference. Here we go.
[125:17] For reference. Here we go.
[125:19] For reference. Here we go.
[125:21] For reference. Here we go.
[125:23] For reference. Here we go.
[125:25] For reference. Here we go.
[125:27] For reference. Here we go.
[125:29] For reference. Here we go.
[125:31] For reference. Here we go.
[125:33] For reference. Here we go.
[125:35] For reference. Here we go.
[125:37] For reference. Here we go.
[125:39] For reference. Here we go.
[125:41] For reference. Here we go.
[125:43] For reference. Here we go.
[125:45] For reference. Here we go.
[125:47] For reference. Here we go.
[125:49] For reference. Here we go.
[125:51] For reference. Here we go.
[125:53] For reference. Here we go.
[125:55] For reference. Here we go.
[125:57] For reference. Here we go.
[125:59] For reference. Here we go.
[126:01] For reference. Here we go.
[126:03] For reference. Here we go.
[126:05] For reference. Here we go.
[126:07] For reference. Here we go.
[126:09] For reference. Here we go.
[126:11] For reference. Here we go.
[126:13] For reference. Here we go.
[126:15] For reference. Here we go.
[126:17] For reference. Here we go.
[126:19] For reference. Here we go.
[126:21] For reference. Here we go.
[126:23] For reference. Here we go.
[126:25] For reference. Here we go.
[126:27] For reference. Here we go.
[126:29] For reference. Here we go.
[126:31] For reference. Here we go.
[126:33] For reference. Here we go.
[126:35] For reference. Here we go.
[126:37] For reference. Here we go.
[126:39] For reference. Here we go.
[126:41] For reference. Here we go.
[126:43] For reference. Here we go.
[126:45] For reference. Here we go.
[126:47] For reference. Here we go.
[126:49] For reference. Here we go.
[126:51] For reference. Here we go.
[126:53] For reference. Here we go.
[126:55] For reference. Here we go.
[126:57] For reference. Here we go.
[126:59] For reference. Here we go.
[127:01] For reference. Here we go.
[127:03] For reference. Here we go.
[127:05] For reference. Here we go.
[127:07] For reference. Here we go.
[127:09] For reference. Here we go.
[127:11] For reference. Here we go.
[127:13] For reference. Here we go.
[127:15] For reference. Here we go.
[127:17] For reference. Here we go.
[127:19] For reference. Here we go.
[127:21] For reference. Here we go.
[127:23] For reference. Here we go.
[127:25] For reference. Here we go.
[127:27] For reference. Here we go.
[127:29] For reference. Here we go.
[127:31] For reference. Here we go.
[127:33] For reference. Here we go.
[127:35] For reference. Here we go.
[127:37] For reference. Here we go.
[127:39] For reference. Here we go.
[127:41] For reference. Here we go.
[127:43] For reference. Here we go.
[127:45] For reference. Here we go.
[127:47] For reference. Here we go.
[127:49] For reference. Here we go.
[127:51] For reference. Here we go.
[127:53] For reference. Here we go.
[127:55] For reference. Here we go.
[127:57] For reference. Here we go.
[127:59] For reference. Here we go.
[128:01] For reference. Here we go.
[128:03] For reference. Here we go.
[128:05] For reference. Here we go.
[128:07] For reference. Here we go.
[128:09] For reference. Here we go.
[128:11] For reference. Here we go.
[128:13] For reference. Here we go.
[128:15] For reference. Here we go.
[128:17] For reference. Here we go.
[128:19] For reference. Here we go.
[128:21] For reference. Here we go.
[128:23] For reference. Here we go.
[128:25] For reference. Here we go.
[128:27] For reference. Here we go.
[128:29] For reference. Here we go.
[128:31] For reference. Here we go.
[128:33] For reference. Here we go.
[128:35] For reference. Here we go.
[128:37] For reference. Here we go.
[128:39] For reference. Here we go.
[128:41] For reference. Here we go.
[128:43] For reference. Here we go.
[128:45] For reference. Here we go.
[128:47] For reference. Here we go.
[128:49] For reference. Here we go.
[128:51] For reference. Here we go.
[128:53] For reference. Here we go.
[128:55] For reference. Here we go.
[128:57] For reference. Here we go.
[128:59] For reference. Here we go.
[129:01] For reference. Here we go.
[129:03] For reference. Here we go.
[129:05] For reference. Here we go.
[129:07] For reference. Here we go.
[129:09] For reference. Here we go.
[129:11] For reference. Here we go.
[129:13] For reference. Here we go.
[129:15] For reference. Here we go.
[129:17] For reference. Here we go.
[129:19] For reference. Here we go.
[129:21] For reference. Here we go.
[129:23] For reference. Here we go.
[129:25] For reference. Here we go.
[129:27] For reference. Here we go.
[129:29] For reference. Here we go.
[129:31] For reference. Here we go.
[129:33] For reference. Here we go.
[129:35] For reference. Here we go.
[129:37] For reference. Here we go.
[129:39] For reference. Here we go.
[129:41] For reference. Here we go.
[129:43] For reference. Here we go.
[129:45] For reference. Here we go.
[129:47] For reference. Here we go.
[129:49] For reference. Here we go.
[129:51] For reference. Here we go.
[129:53] For reference. Here we go.
[129:55] For reference. Here we go.
[129:57] For reference. Here we go.
[129:59] For reference. Here we go.
[130:01] For reference. Here we go.
[130:03] For reference. Here we go.
[130:05] For reference. Here we go.
[130:07] For reference. Here we go.
[130:09] For reference. Here we go.
[130:11] For reference. Here we go.
[130:13] For reference. Here we go.
[130:15] For reference. Here we go.
[130:17] For reference. Here we go.
[130:19] For reference. Here we go.
[130:21] For reference. Here we go.
[130:23] For reference. Here we go.
[130:25] For reference. Here we go.
[130:27] For reference. Here we go.
[130:29] For reference. Here we go.
[130:31] For reference. Here we go.
[130:33] For reference. Here we go.
[130:35] For reference. Here we go.
[130:37] For reference. Here we go.
[130:39] For reference. Here we go.
[130:41] For reference. Here we go.
[130:43] For reference. Here we go.
[130:45] For reference. Here we go.
[130:47] For reference. Here we go.
[130:49] For reference. Here we go.
[130:51] For reference. Here we go.
[130:53] For reference. Here we go.
[130:55] For reference. Here we go.
[130:57] For reference. Here we go.
[130:59] For reference. Here we go.
[131:01] For reference. Here we go.
[131:03] For reference. Here we go.
[131:05] For reference. Here we go.
[131:07] For reference. Here we go.
[131:09] For reference. Here we go.
[131:11] For reference. Here we go.
[131:13] For reference. Here we go.
[131:15] For reference. Here we go.
[131:17] For reference. Here we go.
[131:19] For reference. Here we go.
[131:21] For reference. Here we go.
[131:23] For reference. Here we go.
[131:25] For reference. Here we go.
[131:27] For reference. Here we go.
[131:29] For reference. Here we go.
[131:31] For reference. Here we go.
[131:33] For reference. Here we go.
[131:35] For reference. Here we go.
[131:37] For reference. Here we go.
[131:39] For reference. Here we go.
[131:41] For reference. Here we go.
[131:43] For reference. Here we go.
[131:45] For reference. Here we go.
[131:47] For reference. Here we go.
[131:49] For reference. Here we go.
[131:51] For reference. Here we go.
[131:53] For reference. Here we go.
[131:55] For reference. Here we go.
[131:57] For reference. Here we go.
[131:59] For reference. Here we go.
[132:01] For reference. Here we go.
[132:03] For reference. Here we go.
[132:05] For reference. Here we go.
[132:07] For reference. Here we go.
[132:09] For reference. Here we go.
[132:11] For reference. Here we go.
[132:13] For reference. Here we go.
[132:15] For reference. Here we go.
[132:17] For reference. Here we go.
[132:19] For reference. Here we go.
[132:21] For reference. Here we go.
[132:23] For reference. Here we go.
[132:25] For reference. Here we go.
[132:27] For reference. Here we go.
[132:29] For reference. Here we go.
[132:31] For reference. Here we go.
[132:33] For reference. Here we go.
[132:35] For reference. Here we go.
[132:37] For reference. Here we go.
[132:39] For reference. Here we go.
[132:41] For reference. Here we go.
[132:43] For reference. Here we go.
[132:45] For reference. Here we go.
[132:47] For reference. Here we go.
[132:49] For reference. Here we go.
[132:51] For reference. Here we go.
[132:53] For reference. Here we go.
[132:55] For reference. Here we go.
[132:57] For reference. Here we go.
[132:59] For reference. Here we go.
[133:01] For reference. Here we go.
[133:03] For reference. Here we go.
[133:05] For reference. Here we go.
[133:07] For reference. Here we go.
[133:09] For reference. Here we go.
[133:11] For reference. Here we go.
[133:13] For reference. Here we go.
[133:15] For reference. Here we go.
[133:17] For reference. Here we go.
[133:19] For reference. Here we go.
[133:21] For reference. Here we go.
[133:23] For reference. Here we go.
[133:25] For reference. Here we go.
[133:27] For reference. Here we go.
[133:29] For reference. Here we go.
[133:31] For reference. Here we go.
[133:33] For reference. Here we go.
[133:35] For reference. Here we go.
[133:37] For reference. Here we go.
[133:39] For reference. Here we go.
[133:41] For reference. Here we go.
[133:43] For reference. Here we go.
[133:45] For reference. Here we go.
[133:47] For reference. Here we go.
[133:49] For reference. Here we go.
[133:51] For reference. Here we go.
[133:53] For reference. Here we go.
[133:55] For reference. Here we go.
[133:57] For reference. Here we go.
[133:59] For reference. Here we go.
[134:01] For reference. Here we go.
[134:03] For reference. Here we go.
[134:05] For reference. Here we go.
[134:07] For reference. Here we go.
[134:09] For reference. Here we go.
[134:11] For reference. Here we go.
[134:13] For reference. Here we go.
[134:15] For reference. Here we go.
[134:17] For reference. Here we go.
[134:19] For reference. Here we go.
[134:21] For reference. Here we go.
[134:23] For reference. Here we go.
[134:25] For reference. Here we go.
[134:27] For reference. Here we go.
[134:29] For reference. Here we go.
[134:31] For reference. Here we go.
[134:33] For reference. Here we go.
[134:35] For reference. Here we go.
[134:37] For reference. Here we go.
[134:39] For reference. Here we go.
[134:41] For reference. Here we go.
[134:43] For reference. Here we go.
[134:45] For reference. Here we go.
[134:47] For reference. Here we go.
[134:49] For reference. Here we go.
[134:51] For reference. Here we go.
[134:53] For reference. Here we go.
[134:55] For reference. Here we go.
[134:57] For reference. Here we go.
[134:59] For reference. Here we go.
[135:01] For reference. Here we go.
[135:03] For reference. Here we go.
[135:05] For reference. Here we go.
[135:07] For reference. Here we go.
[135:09] For reference. Here we go.
[135:11] For reference. Here we go.
[135:13] For reference. Here we go.
[135:15] For reference. Here we go.
[135:17] For reference. Here we go.
[135:19] For reference. Here we go.
[135:21] For reference. Here we go.
[135:23] For reference. Here we go.
[135:25] For reference. Here we go.
[135:27] For reference. Here we go.
[135:29] For reference. Here we go.
[135:31] For reference. Here we go.
[135:33] For reference. Here we go.
[135:35] For reference. Here we go.
[135:37] For reference. Here we go.
[135:39] For reference. Here we go.
[135:41] For reference. Here we go.
[135:43] For reference. Here we go.
[135:45] For reference. Here we go.
[135:47] For reference. Here we go.
[135:49] For reference. Here we go.
[135:51] For reference. Here we go.
[135:53] For reference. Here we go.
[135:55] For reference. Here we go.
[135:57] For reference. Here we go.
[135:59] For reference. Here we go.
[136:01] For reference. Here we go.
[136:03] For reference. Here we go.
[136:05] For reference. Here we go.
[136:07] For reference. Here we go.
[136:09] For reference. Here we go.
[136:11] For reference. Here we go.
[136:13] For reference. Here we go.
[136:15] For reference. Here we go.
[136:17] For reference. Here we go.
[136:19] For reference. Here we go.
[136:21] For reference. Here we go.
[136:23] For reference. Here we go.
[136:25] For reference. Here we go.
[136:27] For reference. Here we go.
[136:29] For reference. Here we go.
[136:31] For reference. Here we go.
[136:33] For reference. Here we go.
[136:35] For reference. Here we go.
[136:37] For reference. Here we go.
[136:39] For reference. Here we go.
[136:41] For reference. Here we go.
[136:43] For reference. Here we go.
[136:45] For reference. Here we go.
[136:47] For reference. Here we go.
[136:49] For reference. Here we go.
[136:51] For reference. Here we go.
[136:53] For reference. Here we go.
[136:55] For reference. Here we go.
[136:57] For reference. Here we go.
[136:59] For reference. Here we go.
[137:01] For reference. Here we go.
[137:03] For reference. Here we go.
[137:05] For reference. Here we go.
[137:07] For reference. Here we go.
[137:09] For reference. Here we go.
[137:11] For reference. Here we go.
[137:13] For reference. Here we go.
[137:15] For reference. Here we go.
[137:17] For reference. Here we go.
[137:19] For reference. Here we go.
[137:21] For reference. Here we go.
[137:23] For reference. Here we go.
[137:25] For reference. Here we go.
[137:27] For reference. Here we go.
[137:29] For reference. Here we go.
[137:31] For reference. Here we go.
[137:33] For reference. Here we go.
[137:35] For reference. Here we go.
[137:37] For reference. Here we go.
[137:39] For reference. Here we go.
[137:41] For reference. Here we go.
[137:43] For reference. Here we go.
[137:45] For reference. Here we go.
[137:47] For reference. Here we go.
[137:49] For reference. Here we go.
[137:51] For reference. Here we go.
[137:53] For reference. Here we go.
[137:55] For reference. Here we go.
[137:57] For reference. Here we go.
[137:59] For reference. Here we go.
[138:01] For reference. Here we go.
[138:03] For reference. Here we go.
[138:05] For reference. Here we go.
[138:07] For reference. Here we go.
[138:09] For reference. Here we go.
[138:11] For reference. Here we go.
[138:13] For reference. Here we go.
[138:15] For reference. Here we go.
[138:17] For reference. Here we go.
[138:19] For reference. Here we go.
[138:21] For reference. Here we go.
[138:23] For reference. Here we go.
[138:25] For reference. Here we go.
[138:27] For reference. Here we go.
[138:29] For reference. Here we go.
[138:31] For reference. Here we go.
[138:33] For reference. Here we go.
[138:35] For reference. Here we go.
[138:37] For reference. Here we go.
[138:39] For reference. Here we go.
[138:41] For reference. Here we go.
[138:43] For reference. Here we go.
[138:45] For reference. Here we go.
[138:47] For reference. Here we go.
[138:49] For reference. Here we go.
[138:51] For reference. Here we go.
[138:53] For reference. Here we go.
[138:55] For reference. Here we go.
[138:57] For reference. Here we go.
[138:59] For reference. Here we go.
[139:01] For reference. Here we go.
[139:03] For reference. Here we go.
[139:05] For reference. Here we go.
[139:07] For reference. Here we go.
[139:09] For reference. Here we go.
[139:11] For reference. Here we go.
[139:13] For reference. Here we go.
[139:15] For reference. Here we go.
[139:17] For reference. Here we go.
[139:19] For reference. Here we go.
[139:21] For reference. Here we go.
[139:23] For reference. Here we go.
[139:25] For reference. Here we go.
[139:27] For reference. Here we go.
[139:29] For reference. Here we go.
[139:31] For reference. Here we go.
[139:33] For reference. Here we go.
[139:35] For reference. Here we go.
[139:37] For reference. Here we go.
[139:39] For reference. Here we go.
[139:41] For reference. Here we go.
[139:43] For reference. Here we go.
[139:45] For reference. Here we go.
[139:47] For reference. Here we go.
[139:49] For reference. Here we go.
[139:51] For reference. Here we go.
[139:53] For reference. Here we go.
[139:55] For reference. Here we go.
[139:57] For reference. Here we go.
[139:59] For reference. Here we go.
[140:01] For reference. Here we go.
[140:03] For reference. Here we go.
[140:05] For reference. Here we go.
[140:07] For reference. Here we go.
[140:09] For reference. Here we go.
[140:11] For reference. Here we go.
[140:13] For reference. Here we go.
[140:15] For reference. Here we go.
[140:17] For reference. Here we go.
[140:19] For reference. Here we go.
[140:21] For reference. Here we go.
[140:23] For reference. Here we go.
[140:25] For reference. Here we go.
[140:27] For reference. Here we go.
[140:29] For reference. Here we go.
[140:31] For reference. Here we go.
[140:33] For reference. Here we go.
[140:35] For reference. Here we go.
[140:37] For reference. Here we go.
[140:39] For reference. Here we go.
[140:41] For reference. Here we go.
[140:43] For reference. Here we go.
[140:45] For reference. Here we go.
[140:47] For reference. Here we go.
[140:49] For reference. Here we go.
[140:51] For reference. Here we go.
[140:53] For reference. Here we go.
[140:55] For reference. Here we go.
[140:57] For reference. Here we go.
[140:59] For reference. Here we go.
[141:01] For reference. Here we go.
[141:03] For reference. Here we go.
[141:05] For reference. Here we go.
[141:07] For reference. Here we go.
[141:09] For reference. Here we go.
[141:11] For reference. Here we go.
[141:13] For reference. Here we go.
[141:15] For reference. Here we go.
[141:17] For reference. Here we go.
[141:19] For reference. Here we go.
[141:21] For reference. Here we go.
[141:23] For reference. Here we go.
[141:25] For reference. Here we go.
[141:27] For reference. Here we go.
[141:29] For reference. Here we go.
[141:31] For reference. Here we go.
[141:33] For reference. Here we go.
[141:35] For reference. Here we go.
[141:37] For reference. Here we go.
[141:39] For reference. Here we go.
[141:41] For reference. Here we go.
[141:43] For reference. Here we go.
[141:45] For reference. Here we go.
[141:47] For reference. Here we go.
[141:49] For reference. Here we go.
[141:51] For reference. Here we go.
[141:53] For reference. Here we go.
[141:55] For reference. Here we go.
[141:57] For reference. Here we go.
[141:59] For reference. Here we go.
[142:01] For reference. Here we go.
[142:03] For reference. Here we go.
[142:05] For reference. Here we go.
[142:07] For reference. Here we go.
[142:09] For reference. Here we go.
[142:11] For reference. Here we go.
[142:13] For reference. Here we go.
[142:15] For reference. Here we go.
[142:17] For reference. Here we go.
[142:19] For reference. Here we go.
[142:21] For reference. Here we go.
[142:23] For reference. Here we go.
[142:25] For reference. Here we go.
[142:27] For reference. Here we go.
[142:29] For reference. Here we go.
[142:31] For reference. Here we go.
[142:33] For reference. Here we go.
[142:35] For reference. Here we go.
[142:37] For reference. Here we go.
[142:39] For reference. Here we go.
[142:41] For reference. Here we go.
[142:43] For reference. Here we go.
[142:45] For reference. Here we go.
[142:47] For reference. Here we go.
[142:49] For reference. Here we go.
[142:51] For reference. Here we go.
[142:53] For reference. Here we go.
[142:55] For reference. Here we go.
[142:57] For reference. Here we go.
[142:59] For reference. Here we go.
[143:01] For reference. Here we go.
[143:03] For reference. Here we go.
[143:05] For reference. Here we go.
[143:07] For reference. Here we go.
[143:09] For reference. Here we go.
[143:11] For reference. Here we go.
[143:13] For reference. Here we go.
[143:15] For reference. Here we go.
[143:17] For reference. Here we go.
[143:19] For reference. Here we go.
[143:21] For reference. Here we go.
[143:23] For reference. Here we go.
[143:25] For reference. Here we go.
[143:27] For reference. Here we go.
[143:29] For reference. Here we go.
[143:31] For reference. Here we go.
[143:33] For reference. Here we go.
[143:35] For reference. Here we go.
[143:37] For reference. Here we go.
[143:39] For reference. Here we go.
[143:41] For reference. Here we go.
[143:43] For reference. Here we go.
[143:45] For reference. Here we go.
[143:47] For reference. Here we go.
[143:49] For reference. Here we go.
[143:51] For reference. Here we go.
[143:53] For reference. Here we go.
[143:55] For reference. Here we go.
[143:57] For reference. Here we go.
[143:59] For reference. Here we go.
[144:01] For reference. Here we go.
[144:03] For reference. Here we go.
[144:05] For reference. Here we go.
[144:07] For reference. Here we go.
[144:09] For reference. Here we go.
[144:11] For reference. Here we go.
[144:13] For reference. Here we go.
[144:15] For reference. Here we go.
[144:17] For reference. Here we go.
[144:19] For reference. Here we go.
[144:21] For reference. Here we go.
[144:23] For reference. Here we go.
[144:25] For reference. Here we go.
[144:27] For reference. Here we go.
[144:29] For reference. Here we go.
[144:31] For reference. Here we go.
[144:33] For reference. Here we go.
[144:35] For reference. Here we go.
[144:37] For reference. Here we go.
[144:39] For reference. Here we go.
[144:41] For reference. Here we go.
[144:43] For reference. Here we go.
[144:45] For reference. Here we go.
[144:47] For reference. Here we go.
[144:49] For reference. Here we go.
[144:51] For reference. Here we go.
[144:53] For reference. Here we go.
[144:55] For reference. Here we go.
[144:57] For reference. Here we go.
[144:59] For reference. Here we go.
[145:01] For reference. Here we go.
[145:03] For reference. Here we go.
[145:05] For reference. Here we go.
[145:07] For reference. Here we go.
[145:09] For reference. Here we go.
[145:11] For reference. Here we go.
[145:13] For reference. Here we go.
[145:15] For reference. Here we go.
[145:17] For reference. Here we go.
[145:19] For reference. Here we go.
[145:21] For reference. Here we go.
[145:23] For reference. Here we go.
[145:25] For reference. Here we go.
[145:27] For reference. Here we go.
[145:29] For reference. Here we go.
[145:31] For reference. Here we go.
[145:33] For reference. Here we go.
[145:35] For reference. Here we go.
[145:37] For reference. Here we go.
[145:39] For reference. Here we go.
[145:41] For reference. Here we go.
[145:43] For reference. Here we go.
[145:45] For reference. Here we go.
[145:47] For reference. Here we go.
[145:49] For reference. Here we go.
[145:51] For reference. Here we go.
[145:53] For reference. Here we go.
[145:55] For reference. Here we go.
[145:57] For reference. Here we go.
[145:59] For reference. Here we go.
[146:01] For reference. Here we go.
[146:03] For reference. Here we go.
[146:05] For reference. Here we go.
[146:07] For reference. Here we go.
[146:09] For reference. Here we go.
[146:11] For reference. Here we go.
[146:13] For reference. Here we go.
[146:15] For reference. Here we go.
[146:17] For reference. Here we go.
[146:19] For reference. Here we go.
[146:21] For reference. Here we go.
[146:23] For reference. Here we go.
[146:25] For reference. Here we go.
[146:27] For reference. Here we go.
[146:29] For reference. Here we go.
[146:31] For reference. Here we go.
[146:33] For reference. Here we go.
[146:35] For reference. Here we go.
[146:37] For reference. Here we go.
[146:39] For reference. Here we go.
[146:41] For reference. Here we go.
[146:43] For reference. Here we go.
[146:45] For reference. Here we go.
[146:47] For reference. Here we go.
[146:49] For reference. Here we go.
[146:51] For reference. Here we go.
[146:53] For reference. Here we go.
[146:55] For reference. Here we go.
[146:57] For reference. Here we go.
[146:59] For reference. Here we go.
[147:01] For reference. Here we go.
[147:03] For reference. Here we go.
[147:05] For reference. Here we go.
[147:07] For reference. Here we go.
[147:09] For reference. Here we go.
[147:11] For reference. Here we go.
[147:13] For reference. Here we go.
[147:15] For reference. Here we go.
[147:17] For reference. Here we go.
[147:19] For reference. Here we go.
[147:21] For reference. Here we go.
[147:23] For reference. Here we go.
[147:25] For reference. Here we go.
[147:27] For reference. Here we go.
[147:29] For reference. Here we go.
[147:31] For reference. Here we go.
[147:33] For reference. Here we go.
[147:35] For reference. Here we go.
[147:37] For reference. Here we go.
[147:39] For reference. Here we go.
[147:41] For reference. Here we go.
[147:43] For reference. Here we go.
[147:45] For reference. Here we go.
[147:47] For reference. Here we go.
[147:49] For reference. Here we go.
[147:51] For reference. Here we go.
[147:53] For reference. Here we go.
[147:55] For reference. Here we go.
[147:57] For reference. Here we go.
[147:59] For reference. Here we go.
[148:01] For reference. Here we go.
[148:03] For reference. Here we go.
[148:05] For reference. Here we go.
[148:07] For reference. Here we go.
[148:09] For reference. Here we go.
[148:11] For reference. Here we go.
[148:13] For reference. Here we go.
[148:15] For reference. Here we go.
[148:17] For reference. Here we go.
[148:19] For reference. Here we go.
[148:21] For reference. Here we go.
[148:23] For reference. Here we go.
[148:25] For reference. Here we go.
[148:27] For reference. Here we go.
[148:29] For reference. Here we go.
[148:31] For reference. Here we go.
[148:33] For reference. Here we go.
[148:35] For reference. Here we go.
[148:37] For reference. Here we go.
[148:39] For reference. Here we go.
[148:41] For reference. Here we go.
[148:43] For reference. Here we go.
[148:45] For reference. Here we go.
[148:47] For reference. Here we go.
[148:49] For reference. Here we go.
[148:51] For reference. Here we go.
[148:53] For reference. Here we go.
[148:55] For reference. Here we go.
[148:57] For reference. Here we go.
[148:59] For reference. Here we go.
[149:01] For reference. Here we go.
[149:03] For reference. Here we go.
[149:05] For reference. Here we go.
[149:07] For reference. Here we go.
[149:09] For reference. Here we go.
[149:11] For reference. Here we go.
[149:13] For reference. Here we go.
[149:15] For reference. Here we go.
[149:17] For reference. Here we go.
[149:19] For reference. Here we go.
[149:21] For reference. Here we go.
[149:23] For reference. Here we go.
[149:25] For reference. Here we go.
[149:27] For reference. Here we go.
[149:29] For reference. Here we go.
[149:31] For reference. Here we go.
[149:33] For reference. Here we go.
[149:35] For reference. Here we go.
[149:37] For reference. Here we go.
[149:39] For reference. Here we go.
[149:41] For reference. Here we go.
[149:43] For reference. Here we go.
[149:45] For reference. Here we go.
[149:47] For reference. Here we go.
[149:49] For reference. Here we go.
[149:51] For reference. Here we go.
[149:53] For reference. Here we go.
[149:55] For reference. Here we go.
[149:57] For reference. Here we go.
[149:59] For reference. Here we go.
[150:01] For reference. Here we go.
[150:03] For reference. Here we go.
[150:05] For reference. Here we go.
[150:07] For reference. Here we go.
[150:09] For reference. Here we go.
[150:11] For reference. Here we go.
[150:13] For reference. Here we go.
[150:15] For reference. Here we go.
[150:17] For reference. Here we go.
[150:19] For reference. Here we go.
[150:21] For reference. Here we go.
[150:23] For reference. Here we go.
[150:25] For reference. Here we go.
[150:27] For reference. Here we go.
[150:29] For reference. Here we go.
[150:31] For reference. Here we go.
[150:33] For reference. Here we go.
[150:35] For reference. Here we go.
[150:37] For reference. Here we go.
[150:39] For reference. Here we go.
[150:41] For reference. Here we go.
[150:43] For reference. Here we go.
[150:45] For reference. Here we go.
[150:47] For reference. Here we go.
[150:49] For reference. Here we go.
[150:51] For reference. Here we go.
[150:53] For reference. Here we go.
[150:55] For reference. Here we go.
[150:57] For reference. Here we go.
[150:59] For reference. Here we go.
[151:01] For reference. Here we go.
[151:03] For reference. Here we go.
[151:05] For reference. Here we go.
[151:07] For reference. Here we go.
[151:09] For reference. Here we go.
[151:11] For reference. Here we go.
[151:13] For reference. Here we go.
[151:15] For reference. Here we go.
[151:17] For reference. Here we go.
[151:19] For reference. Here we go.
[151:21] For reference. Here we go.
[151:23] For reference. Here we go.
[151:25] For reference. Here we go.
[151:27] For reference. Here we go.
[151:29] For reference. Here we go.
[151:31] For reference. Here we go.
[151:33] For reference. Here we go.
[151:35] For reference. Here we go.
[151:37] For reference. Here we go.
[151:39] For reference. Here we go.
[151:41] For reference. Here we go.
[151:43] For reference. Here we go.
[151:45] For reference. Here we go.
[151:47] For reference. Here we go.
[151:49] For reference. Here we go.
[151:51] For reference. Here we go.
[151:53] For reference. Here we go.
[151:55] For reference. Here we go.
[151:57] For reference. Here we go.
[151:59] For reference. Here we go.
[152:01] For reference. Here we go.
[152:03] For reference. Here we go.
[152:05] For reference. Here we go.
[152:07] For reference. Here we go.
[152:09] For reference. Here we go.
[152:11] For reference. Here we go.
[152:13] For reference. Here we go.
[152:15] For reference. Here we go.
[152:17] For reference. Here we go.
[152:19] For reference. Here we go.
[152:21] For reference. Here we go.
[152:23] For reference. Here we go.
[152:25] For reference. Here we go.
[152:27] For reference. Here we go.
[152:29] For reference. Here we go.
[152:31] For reference. Here we go.
[152:33] For reference. Here we go.
[152:35] For reference. Here we go.
[152:37] For reference. Here we go.
[152:39] For reference. Here we go.
[152:41] For reference. Here we go.
[152:43] For reference. Here we go.
[152:45] For reference. Here we go.
[152:47] For reference. Here we go.
[152:49] For reference. Here we go.
[152:51] For reference. Here we go.
[152:53] For reference. Here we go.
[152:55] For reference. Here we go.
[152:57] For reference. Here we go.
[152:59] For reference. Here we go.
[153:01] For reference. Here we go.
[153:03] For reference. Here we go.
[153:05] For reference. Here we go.
[153:07] For reference. Here we go.
[153:09] For reference. Here we go.
[153:11] For reference. Here we go.
[153:13] For reference. Here we go.
[153:15] For reference. Here we go.
[153:17] For reference. Here we go.
[153:19] For reference. Here we go.
[153:21] For reference. Here we go.
[153:23] For reference. Here we go.
[153:25] For reference. Here we go.
[153:27] For reference. Here we go.
[153:29] For reference. Here we go.
[153:31] For reference. Here we go.
[153:33] For reference. Here we go.
[153:35] For reference. Here we go.
[153:37] For reference. Here we go.
[153:39] For reference. Here we go.
[153:41] For reference. Here we go.
[153:43] For reference. Here we go.
[153:45] For reference. Here we go.
[153:47] For reference. Here we go.
[153:49] For reference. Here we go.
[153:51] For reference. Here we go.
[153:53] For reference. Here we go.
[153:55] For reference. Here we go.
[153:57] For reference. Here we go.
[153:59] For reference. Here we go.
[154:01] For reference. Here we go.
[154:03] For reference. Here we go.
[154:05] For reference. Here we go.
[154:07] For reference. Here we go.
[154:09] For reference. Here we go.
[154:11] For reference. Here we go.
[154:13] For reference. Here we go.
[154:15] For reference. Here we go.
[154:17] For reference. Here we go.
[154:19] For reference. Here we go.
[154:21] For reference. Here we go.
[154:23] For reference. Here we go.
[154:25] For reference. Here we go.
[154:27] For reference. Here we go.
[154:29] For reference. Here we go.
[154:31] For reference. Here we go.
[154:33] For reference. Here we go.
[154:35] For reference. Here we go.
[154:37] For reference. Here we go.
[154:39] For reference. Here we go.
[154:41] For reference. Here we go.
[154:43] For reference. Here we go.
[154:45] For reference. Here we go.
[154:47] For reference. Here we go.
[154:49] For reference. Here we go.
[154:51] For reference. Here we go.
[154:53] For reference. Here we go.
[154:55] For reference. Here we go.
[154:57] For reference. Here we go.
[154:59] For reference. Here we go.
[155:01] For reference. Here we go.
[155:03] For reference. Here we go.
[155:05] For reference. Here we go.
[155:07] For reference. Here we go.
[155:09] For reference. Here we go.
[155:11] For reference. Here we go.
[155:13] For reference. Here we go.
[155:15] For reference. Here we go.
[155:17] For reference. Here we go.
[155:19] For reference. Here we go.
[155:21] For reference. Here we go.
[155:23] For reference. Here we go.
[155:25] For reference. Here we go.
[155:27] For reference. Here we go.
[155:29] For reference. Here we go.
[155:31] For reference. Here we go.
[155:33] For reference. Here we go.
[155:35] For reference. Here we go.
[155:37] For reference. Here we go.
[155:39] For reference. Here we go.
[155:41] For reference. Here we go.
[155:43] For reference. Here we go.
[155:45] For reference. Here we go.
[155:47] For reference. Here we go.
[155:49] For reference. Here we go.
[155:51] For reference. Here we go.
[155:53] For reference. Here we go.
[155:55] For reference. Here we go.
[155:57] For reference. Here we go.
[155:59] For reference. Here we go.
[156:01] For reference. Here we go.
[156:03] For reference. Here we go.
[156:05] For reference. Here we go.
[156:07] For reference. Here we go.
[156:09] For reference. Here we go.
[156:11] For reference. Here we go.
[156:13] For reference. Here we go.
[156:15] For reference. Here we go.
[156:17] For reference. Here we go.
[156:19] For reference. Here we go.
[156:21] For reference. Here we go.
[156:23] For reference. Here we go.
[156:25] For reference. Here we go.
[156:27] For reference. Here we go.
[156:29] For reference. Here we go.
[156:31] For reference. Here we go.
[156:33] For reference. Here we go.
[156:35] For reference. Here we go.
[156:37] For reference. Here we go.
[156:39] For reference. Here we go.
[156:41] For reference. Here we go.
[156:43] For reference. Here we go.
[156:45] For reference. Here we go.
[156:47] For reference. Here we go.
[156:49] For reference. Here we go.
[156:51] For reference. Here we go.
[156:53] For reference. Here we go.
[156:55] For reference. Here we go.
[156:57] For reference. Here we go.
[156:59] For reference. Here we go.
[157:01] For reference. Here we go.
[157:03] For reference. Here we go.
[157:05] For reference. Here we go.
[157:07] For reference. Here we go.
[157:09] For reference. Here we go.
[157:11] For reference. Here we go.
[157:13] For reference. Here we go.
[157:15] For reference. Here we go.
[157:17] For reference. Here we go.
[157:19] For reference. Here we go.
[157:21] For reference. Here we go.
[157:23] For reference. Here we go.
[157:25] For reference. Here we go.
[157:27] For reference. Here we go.
[157:29] For reference. Here we go.
[157:31] For reference. Here we go.
[157:33] For reference. Here we go.
[157:35] For reference. Here we go.
[157:37] For reference. Here we go.
[157:39] For reference. Here we go.
[157:41] For reference. Here we go.
[157:43] For reference. Here we go.
[157:45] For reference. Here we go.
[157:47] For reference. Here we go.
[157:49] For reference. Here we go.
[157:51] For reference. Here we go.
[157:53] For reference. Here we go.
[157:55] For reference. Here we go.
[157:57] For reference. Here we go.
[157:59] For reference. Here we go.
[158:01] For reference. Here we go.
[158:03] For reference. Here we go.
[158:05] For reference. Here we go.
[158:07] For reference. Here we go.
[158:09] For reference. Here we go.
[158:11] For reference. Here we go.
[158:13] For reference. Here we go.
[158:15] For reference. Here we go.
[158:17] For reference. Here we go.
[158:19] For reference. Here we go.
[158:21] For reference. Here we go.
[158:23] For reference. Here we go.
[158:25] For reference. Here we go.
[158:27] For reference. Here we go.
[158:29] For reference. Here we go.
[158:31] For reference. Here we go.
[158:33] For reference. Here we go.
[158:35] For reference. Here we go.
[158:37] For reference. Here we go.
[158:39] For reference. Here we go.
[158:41] For reference. Here we go.
[158:43] For reference. Here we go.
[158:45] For reference. Here we go.
[158:47] For reference. Here we go.
[158:49] For reference. Here we go.
[158:51] For reference. Here we go.
[158:53] For reference. Here we go.
[158:55] For reference. Here we go.
[158:57] For reference. Here we go.
[158:59] For reference. Here we go.
[159:01] For reference. Here we go.
[159:03] For reference. Here we go.
[159:05] For reference. Here we go.
[159:07] For reference. Here we go.
[159:09] For reference. Here we go.
[159:11] For reference. Here we go.
[159:13] For reference. Here we go.
[159:15] For reference. Here we go.
[159:17] For reference. Here we go.
[159:19] For reference. Here we go.
[159:21] For reference. Here we go.
[159:23] For reference. Here we go.
[159:25] For reference. Here we go.
[159:27] For reference. Here we go.
[159:29] For reference. Here we go.
[159:31] For reference. Here we go.
[159:33] For reference. Here we go.
[159:35] For reference. Here we go.
[159:37] For reference. Here we go.
[159:39] For reference. Here we go.
[159:41] For reference. Here we go.
[159:43] For reference. Here we go.
[159:45] For reference. Here we go.
[159:47] For reference. Here we go.
[159:49] For reference. Here we go.
[159:51] For reference. Here we go.
[159:53] For reference. Here we go.
[159:55] For reference. Here we go.
[159:57] For reference. Here we go.
[159:59] For reference. Here we go.
[160:01] For reference. Here we go.
[160:03] For reference. Here we go.
[160:05] For reference. Here we go.
[160:07] For reference. Here we go.
[160:09] For reference. Here we go.
[160:11] For reference. Here we go.
[160:13] For reference. Here we go.
[160:15] For reference. Here we go.
[160:17] For reference. Here we go.
[160:19] For reference. Here we go.
[160:21] For reference. Here we go.
[160:23] For reference. Here we go.
[160:25] For reference. Here we go.
[160:27] For reference. Here we go.
[160:29] For reference. Here we go.
[160:31] For reference. Here we go.
[160:33] For reference. Here we go.
[160:35] For reference. Here we go.
[160:37] For reference. Here we go.
[160:39] For reference. Here we go.
[160:41] For reference. Here we go.
[160:43] For reference. Here we go.
[160:45] For reference. Here we go.
[160:47] For reference. Here we go.
[160:49] For reference. Here we go.
[160:51] For reference. Here we go.
[160:53] For reference. Here we go.
[160:55] For reference. Here we go.
[160:57] For reference. Here we go.
[160:59] For reference. Here we go.
[161:01] For reference. Here we go.
[161:03] For reference. Here we go.
[161:05] For reference. Here we go.
[161:07] For reference. Here we go.
[161:09] For reference. Here we go.
[161:11] For reference. Here we go.
[161:13] For reference. Here we go.
[161:15] For reference. Here we go.
[161:17] For reference. Here we go.
[161:19] For reference. Here we go.
[161:21] For reference. Here we go.
[161:23] For reference. Here we go.
[161:25] For reference. Here we go.
[161:27] For reference. Here we go.
[161:29] For reference. Here we go.
[161:31] For reference. Here we go.
[161:33] For reference. Here we go.
[161:35] For reference. Here we go.
[161:37] For reference. Here we go.
[161:39] For reference. Here we go.
[161:41] For reference. Here we go.
[161:43] For reference. Here we go.
[161:45] For reference. Here we go.
[161:47] For reference. Here we go.
[161:49] For reference. Here we go.
[161:51] For reference. Here we go.
[161:53] For reference. Here we go.
[161:55] For reference. Here we go.
[161:57] For reference. Here we go.
[161:59] For reference. Here we go.
[162:01] For reference. Here we go.
[162:03] For reference. Here we go.
[162:05] For reference. Here we go.
[162:07] For reference. Here we go.
[162:09] For reference. Here we go.
[162:11] For reference. Here we go.
[162:13] For reference. Here we go.
[162:15] For reference. Here we go.
[162:17] For reference. Here we go.
[162:19] For reference. Here we go.
[162:21] For reference. Here we go.
[162:23] For reference. Here we go.
[162:25] For reference. Here we go.
[162:27] For reference. Here we go.
[162:29] For reference. Here we go.
[162:31] For reference. Here we go.
[162:33] For reference. Here we go.
[162:35] For reference. Here we go.
[162:37] For reference. Here we go.
[162:39] For reference. Here we go.
[162:41] For reference. Here we go.
[162:43] For reference. Here we go.
[162:45] For reference. Here we go.
[162:47] For reference. Here we go.
[162:49] For reference. Here we go.
[162:51] For reference. Here we go.
[162:53] For reference. Here we go.
[162:55] For reference. Here we go.
[162:57] For reference. Here we go.
[162:59] For reference. Here we go.
[163:01] For reference. Here we go.
[163:03] For reference. Here we go.
[163:05] For reference. Here we go.
[163:07] For reference. Here we go.
[163:09] For reference. Here we go.
[163:11] For reference. Here we go.
[163:13] For reference. Here we go.
[163:15] For reference. Here we go.
[163:17] For reference. Here we go.
[163:19] For reference. Here we go.
[163:21] For reference. Here we go.
[163:23] For reference. Here we go.
[163:25] For reference. Here we go.
[163:27] For reference. Here we go.
[163:29] For reference. Here we go.
[163:31] For reference. Here we go.
[163:33] For reference. Here we go.
[163:35] For reference. Here we go.
[163:37] For reference. Here we go.
[163:39] For reference. Here we go.
[163:41] For reference. Here we go.
[163:43] For reference. Here we go.
[163:45] For reference. Here we go.
[163:47] For reference. Here we go.
[163:49] For reference. Here we go.
[163:51] For reference. Here we go.
[163:53] For reference. Here we go.
[163:55] For reference. Here we go.
[163:57] For reference. Here we go.
[163:59] For reference. Here we go.
[164:01] For reference. Here we go.
[164:03] For reference. Here we go.
[164:05] For reference. Here we go.
[164:07] For reference. Here we go.
[164:09] For reference. Here we go.
[164:11] For reference. Here we go.
[164:13] For reference. Here we go.
[164:15] For reference. Here we go.
[164:17] For reference. Here we go.
[164:19] For reference. Here we go.
[164:21] For reference. Here we go.
[164:23] For reference. Here we go.
[164:25] For reference. Here we go.
[164:27] For reference. Here we go.
[164:29] For reference. Here we go.
[164:31] For reference. Here we go.
[164:33] For reference. Here we go.
[164:35] For reference. Here we go.
[164:37] For reference. Here we go.
[164:39] For reference. Here we go.
[164:41] For reference. Here we go.
[164:43] For reference. Here we go.
[164:45] For reference. Here we go.
[164:47] For reference. Here we go.
[164:49] For reference. Here we go.
[164:51] For reference. Here we go.
[164:53] For reference. Here we go.
[164:55] For reference. Here we go.
[164:57] For reference. Here we go.
[164:59] For reference. Here we go.
[165:01] For reference. Here we go.
[165:03] For reference. Here we go.
[165:05] For reference. Here we go.
[165:07] For reference. Here we go.
[165:09] For reference. Here we go.
[165:11] For reference. Here we go.
[165:13] For reference. Here we go.
[165:15] For reference. Here we go.
[165:17] For reference. Here we go.
[165:19] For reference. Here we go.
[165:21] For reference. Here we go.
[165:23] For reference. Here we go.
[165:25] For reference. Here we go.
[165:27] For reference. Here we go.
[165:29] For reference. Here we go.
[165:31] For reference. Here we go.
[165:33] For reference. Here we go.
[165:35] For reference. Here we go.
[165:37] For reference. 
