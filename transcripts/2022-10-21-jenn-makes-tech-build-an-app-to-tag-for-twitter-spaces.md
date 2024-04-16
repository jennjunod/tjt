---
showLink: "https://www.youtube.com/watch?v=6Vk9aSe058Y"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "jenn-makes-tech-build-an-app-to-tag-for-twitter-spaces"
title: "Jenn Makes Tech: Build an App to Tag for Twitter Spaces"
publishDate: "2022-10-21"
coverImage: "https://i.ytimg.com/vi/6Vk9aSe058Y/maxresdefault.jpg"
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

[00:00] (claps) Hello, hello, beautiful humans.
[00:04] Random stream time, because I needed more time to figure out this project.
[00:11] I really wanna build this web app thing, and I'm not 100% sure where to start,
[00:23] but I figure streaming it, A, I'll be able to keep it for my information,
[00:29] and B, it'll just help in the long run. You know, like, why not?
[00:35] Why not? So, the goal is to create a something
[00:41] that I can tell people to enter in their Twitter names. I think it'll just be easier to show you.
[00:50] Give me a moment. Okay, good my provo, only tweeters.
[00:59] Easy said. Uh, no.
[01:12] Okay, I'm still looking. Give me a second.
[01:22] All right, all right. So, every week, I need to share my screen
[01:30] to be able to show you what I do every week. All right, so, what I'm trying to solve for today
[01:41] is every week I create my Twitter space, and then I ask everyone, please share, set the reminder.
[01:49] It's literally the same tweet. I copy and paste it,
[01:52] and then I copy and paste all of everybody's Twitter's names so they get tagged,
[01:59] and it's a hassle because half the time I forget to do it. Yes, I could go into, like, Buffer or something
[02:08] and, like, sign up, like, have it autopost, but I don't want to do that
[02:14] because then people can't, like, remove themselves or just, like, auto-add people.
[02:19] Maybe I could do that if I did, like, Zapier from a Google form.
[02:27] I have done something kind of similar with monday.com, but I basically want to be able to create the Twitter space,
[02:35] paste it into this app, and then it create the rest of this for me
[02:40] and allow people to fill in a form to get added to this list.
[02:46] So, like, it knows if I have more than the character limit,
[02:53] it'll tag the person in the next one. I feel like this is very ambitious,
[02:59] but I really want to make it. So that is what I'm gonna be working on.
[03:05] Oh, yay. Ta-da, okay.
[03:09] So we are going through the bare basics to start with. I am gonna be creating a readme in all of that
[03:20] and be able to create this in GitHub, and I need to remember all of the things
[03:30] to be able to create in GitHub. So please bear with me while I Google all the things.
[03:39] I guess I could Google over here, too. Hmm.
[03:43] CLI, create, GitHub, repo. Oh, that works.
[03:55] Close enough, right? Close enough.
[03:58] I feel like it is. And also, and as we're going along with this today,
[04:05] feel free to ask questions or be able to give suggestions.
[04:11] This is something that I'm doing for live learning because I really want to get this done.
[04:17] Again, open to suggestions, yet I may also say,
[04:23] just kidding, I'm gonna awkwardly struggle through this. Oh, I almost forgot.
[04:28] Feed the duck. The music.
[04:31] Yes. (upbeat music)
[04:38] I don't wanna... GitHub repo, create.
[04:58] Oh, okay. So let's do something.
[05:01] Cd code, cd desktop, cd code. GitHub repo, create.
[05:19] And I'm pretty sure I already installed the GitHub CLI, but again, we're gonna find out.
[05:30] Oh, we want to create a new one. We want to call them with Twitter space ads, maybe?
[05:39] Description. Wow.
[05:51] Users, new printer. (upbeat music)
[06:01] Twitter handle will be added to the posts for Twitter space notification.
[06:13] Wow. So fun.
[06:21] Fun. I am curious, like, what are you all up to?
[06:30] Like, anything fun today? 'Cause I'm actually really excited
[06:36] to be able to get this done. I have no idea how long it's gonna take,
[06:39] 'cause I'm starting from scratch. And to paste.
[06:46] To paste Twitter space link into. To auto-generate posts.
[07:05] Tagging. (upbeat music)
[07:13] Sure. This is gonna be public.
[07:25] Yes, we need that readme file. We're gonna say yes.
[07:29] Yes, we want MIT. Nope, go back.
[07:39] (upbeat music) Yes, I want to continue.
[07:44] Yes, we want to claim it locally. Yay.
[07:51] Okay, so we need to go to CD, or like, let's see. CD, yes.
[08:00] I hit Tab, so that way it auto-filled. That is something that, oh goodness.
[08:06] Eddie taught me when he was on the stream about that the tab can let you, allow you to auto-fill.
[08:12] So, Twitter space tags. And then we're gonna go code and enter.
[08:19] All right, let's find out why VS Code does not like me to do this.
[08:23] I feel like I had it working, and now it doesn't work again.
[08:28] So I can hit Enter, consult. I do the same thing.
[08:34] I don't know. I don't know.
[08:39] All right. So, I'm not sure.
[08:45] Yes, what up, Frank? Tab, Tab, it's happiness.
[08:54] So I think to get this started, I need to verify that a bit of the Twitter API,
[09:07] a bit of a React app. I don't even know if this is gonna work,
[09:10] so I'm going to pause with the project and create a mirror board, just something visual,
[09:19] so that way I can be like, this is what I'm trying to do. And also be able to take notes for myself
[09:25] of this works, this didn't work, and the visualization of them all.
[09:30] So. (upbeat music)
[09:35] Sure. What are you up to today, tonight?
[09:46] Afternoon, evening, Frank? I don't even know what time zone anybody's in.
[09:52] Could be middle of the night for all I know. Okay.
[09:57] Okay. All right.
[10:12] So again, like Miro is just a way of visually seeing things. I'm pretty sure a lot of people have,
[10:26] like, compared Miro to Figma, but it's, like, not as detailed as Figma.
[10:31] If I were to talk about Miro, I would maybe compare, Miro is, like, Canva is to Photoshop,
[10:39] and Miro is to Figma, which is kind of weird because didn't Adobe buy out Figma?
[10:48] It's a little weird, a little weird, same. Anyway, so.
[10:55] (upbeat music) I totally get that.
[11:03] What part of the world are you in, Frank? I won't.
[11:10] (upbeat music) Oh, okay.
[11:29] I always try to include, like, UTC, which is, I think, four hours after Eastern.
[11:39] So, yeah, like, plus two. Is UTC, I should actually look this up on a map.
[11:46] (upbeat music) Where is, oh.
[11:58] So UTC is, what, London? Wait, ah.
[12:06] Stop. Okay.
[12:11] And then you're plus two, so, ah, you're in this bracket. Which, when I was spending time in Europe,
[12:25] I mean, goodness, this was, like, four years ago now. It was kind of weird because I would go from London
[12:32] to, like, Cologne, and then to Bulgaria, then to London, and I get that it's only, like, two-hour difference
[12:41] between, like, London and Bulgaria, but it would always, like, throw me off so bad.
[12:46] So I'd be like, wait, it's such a small, like, continent. How am I getting so mixed up?
[12:51] Well, thanks for hanging out for a bit. Yes, go to bed.
[12:55] Sleep is important. (upbeat music)
[13:04] Okay, so, I want... (laughs)
[13:17] Yes, time zones are so weird. Luckily, I haven't dealt with too much
[13:23] of, like, dealing with time zones and having to update it within apps,
[13:27] but, I mean, who knows? I might have to with this.
[13:32] I'm gonna put the results, too, is... (upbeat music)
[13:42] (upbeat music) Mm-hmm.
[13:51] (upbeat music) Oh, let's do this.
[14:06] (upbeat music) (upbeat music)
[14:12] (upbeat music) (upbeat music)
[14:17] (upbeat music) (upbeat music)
[14:42] (upbeat music) (upbeat music)
[14:47] (upbeat music) (upbeat music)
[15:16] (upbeat music) (upbeat music)
[15:43] Okay. (upbeat music)
[15:51] (mumbles) (upbeat music)
[16:08] (mumbles) (upbeat music)
[16:20] (upbeat music) (upbeat music)
[16:26] (upbeat music) (upbeat music)
[16:31] (upbeat music) (upbeat music)
[17:01] (upbeat music) - And hello, hello, everybody joining us.
[17:07] This is me working through a giant project that I really wanna work on figuring out.
[17:13] I don't know if it's gonna be possible. I'm writing out currently what I want it to do.
[17:20] And then as a visual, next I'm gonna be working through seeing if it's gonna be possible
[17:27] with the technology that I'm gonna be trying to use and then actually try and build it.
[17:35] So we're getting there. (upbeat music)
[17:40] Okay. (upbeat music)
[17:49] (upbeat music) I feel like this is me actually listening
[18:13] from Leo trying to teach me Twitter spaces, teach me data models.
[18:18] Who knows though? Who knows?
[18:20] (upbeat music) And I know that social media apps may be able to do this,
[18:29] but I literally just wanna enter the Twitter space information.
[18:39] (upbeat music) (upbeat music)
[18:44] What up, Ryan? How is it going?
[18:58] I'm enjoying seeing if I can stumble through all of this. It's gonna be so much fun.
[19:08] (upbeat music) I'm trying to make a new app
[19:14] and I don't know if it's gonna work at all, but I'm gonna try it.
[19:21] I am excited actually. I don't know if that was sarcastic,
[19:24] but I actually am excited. (upbeat music)
[19:28] I want to... (upbeat music)
[19:37] (upbeat music) Yeah, I think I'm just like nervous
[19:51] about... (upbeat music)
[19:58] I will explain it and show it to you here shortly. Give me a second.
[20:02] (upbeat music) Taking screenshot examples.
[20:06] (upbeat music) All right, so on Wednesdays, I host this Twitter space
[20:26] and what ends up happening... I guess I don't need these.
[20:30] I can just do it like this. But what ends up happening is every week,
[20:38] I have to create the Twitter space information and then create
[20:44] all of these tags. And then I have to go look if somebody DM'd me
[20:55] or if I have a form. Thank you.
[20:59] And what I'm working on is seeing if I can make an app auto-do this for me.
[21:06] A, I know that social media tools like Buffer can do a lot of this,
[21:13] yet... Yes, I get to do this stuff with my tablet tomorrow.
[21:19] Thanks for asking, Ryan. I don't know if...
[21:22] We'll see if I can get it figured out tomorrow when I'm supposed to live stream with it,
[21:29] but hey, we'll see. So I'm trying to basically make an app do this for me
[21:38] where other people just need to enter in their Twitter name and then my app I'm gonna attempt to build
[21:48] is going to spit out all of the information. And so that way, all I have to enter every week
[21:55] is create the Twitter space and put it in there and then it does the rest,
[21:59] no matter who wants to sign up for it. Like a database will hold it and spit out the information,
[22:06] but you have joined at a good time because what I think I'm gonna need is...
[22:12] And I'm having fun doing this visually on... The narrow board,
[22:24] because I like looking at it on a visual standpoint, but if we go...
[22:34] So now I'm gonna look at... I feel like this is just giant though.
[22:42] I think all of this is smaller. What do we need?
[22:47] Go smaller. Nobody needs to read that, right?
[22:51] If we zoom in, we can read it. What up, homie?
[22:57] Thank you for joining. Let's see if I can make this app thing.
[23:02] I'm a jig. So here's what the tools I think I'm gonna need.
[23:09] So the Twitter API information is gonna be posting to Twitter.
[23:27] And then I feel like I want to make it with a React web app. I'm not sure if that's correct or not,
[23:45] but that's where my head's going. And then for the database,
[23:52] we are going to use my SQL. (upbeat music)
[23:59] This is where things will enter into this. And then we'll spit out for this.
[24:26] (upbeat music) I'm pretty sure there's an easier way of doing this,
[24:35] like going and probably finding one that somebody's already done,
[24:41] but I'm stubborn and I want to learn the process, even if there is another way of doing it,
[24:47] because in my mind, these aren't all connected yet. Like I want to use my SQL
[24:52] because it's what they used a lot of GoDaddy. And React web app is something
[24:58] I've done on the show enough of. So this is kind of like the plan.
[25:05] I have no idea if I'm going to get it done tonight, but so (hums)
[25:14] (upbeat music) Yeah, I'm gonna be so good.
[25:21] (upbeat music) I learned, yay.
[25:26] We do have a README, which is exciting. And for the README,
[25:33] I'm actually gonna go open it in GitHub. So that way.
[25:37] (upbeat music) Ha ha, nice.
[25:46] I'm glad. Well, I hope the process works.
[25:48] We're gonna find out. We are gonna find out,
[25:52] but we are also gonna fill out the README. The README may be a little dumbed down
[25:58] because I'm gonna write it in a way for me to understand, not necessarily how another developer would understand it,
[26:06] which is okay to me. And if anybody is just like,
[26:11] if you're looking at READMEs going like, what are you talking about?
[26:18] You will not tell you how far then make it in said process. (laughs)
[26:26] I totally get that. Markdown.
[26:29] Markdown, basic syntax. This is like, everybody's different.
[26:37] (upbeat music) I mean, that is a very, very great question, Lucas.
[26:48] And thanks for joining me. (upbeat music)
[26:52] Do I not get React to do that? Or am I missing a step?
[27:00] 'Cause like, mind you, this is me, like my first time doing this.
[27:04] So am I missing a step for it? Yeah, that's what I thought.
[27:09] But is that because MySQL is just the database, it's not actually processing stuff?
[27:16] (upbeat music) Yeah, 'cause I was thinking I could probably
[27:26] make a form on the web app and then... Ooh, okay, okay.
[27:40] Let's make a, what's the comment? Comment, right here.
[27:46] (mumbles) Okay.
[28:04] Ooh, that was fun. I made a note.
[28:07] Did I just make it visible? Do we have to like, in the note?
[28:13] There we go, yay. (upbeat music)
[28:17] Oh, okay, okay. So, I'm gonna start by just like, note.
[28:25] So maybe it would go. Maybe I don't wanna comment.
[28:33] I might. (upbeat music)
[28:37] (humming) Well, I have this zoomed in and I find this hard to read,
[28:56] so I'm putting these fonts bigger. Blah, okay, maybe not that big.
[29:00] So in my mind, I was previously going from here to here, but it's probably like, this.
[29:08] Oh, I don't want you to like, bring you up here. Thank you.
[29:12] To this. To this.
[29:17] What do you think, y'all? Do we have this?
[29:23] And then... I use a track pad instead of a mouse
[29:30] because one day my mouse died, and I had a track pad, and then I haven't gone back since.
[29:35] So if I like, I'm wondering when something's not moving for me,
[29:39] it's just I'm not used to doing it from a track pad. And then, Twitter thread.
[29:47] (upbeat music) Post Twitter thread.
[29:55] Thanks. I think.
[29:59] And I'm giving it a few hours tonight because if I don't get that far, I might come back to this.
[30:07] There'll probably be backend code involved with the connection of my SQL and Twitter as well.
[30:16] Tonight is three hours. 'Cause I wanna get this done by like, Sunday.
[30:27] I'm giving myself a deadline. 'Cause this is the thing that I've really realized
[30:32] with having this show is like, people come on and teach me all of this stuff,
[30:36] but I'm not doing as great as going and practicing it by myself.
[30:42] Because like, Laura's live streams that are on Mondays, she definitely has me practice while I'm on the show.
[30:48] But the rest of them are like, I just kind of, I soak it in, but I don't do anything with it.
[30:56] That I really wanna make this work and be like, look. And also to show on like, when I'm applying for jobs
[31:03] and stuff, okay, I did this mostly by myself. And why I say that is because like,
[31:08] if Lucas wasn't here telling me about, you know, skipping stuff, I probably would have gotten there.
[31:14] It just would have taken more time. So yeah.
[31:18] And I'm hoping this also helps other people learn about it too.
[31:21] We will go. And.
[31:27] (upbeat music) We're just gonna leave it blank
[31:36] 'cause I don't know what will go into it. So.
[31:39] We'll just go like that for now. And.
[31:51] I guess I could just write my notes here and then go back and do my,
[31:57] my read me. That'll work.
[32:06] Plus, you know, this is recorded, which makes it fun. So if I miss something.
[32:11] Have you decided what app to do? I was thinking a React web app.
[32:18] Is that what you're asking? Or are you thinking something else?
[32:25] Anthony has taught me the React web app a few times. So that's kind of why I'm thinking that.
[32:30] And I was about to actually go download it or go try to find it, download it.
[32:39] And then once I get it downloaded, I was gonna try to put in the fields I wanted to do
[32:45] and then find my sequel. Oh, I just want it to be like a form,
[32:55] like a, kind of like a Google form. Maybe.
[33:02] I don't know. I haven't gotten there yet.
[33:13] But it's a great question. I love how all of you are asking me really good questions.
[33:21] Thank you, thank you. React web app.
[33:26] Creating new React app. (upbeat music)
[33:41] (indistinct) (upbeat music continues)
[33:46] (indistinct) This one's fast.
[34:09] (upbeat music continues) (upbeat music continues)
[34:16] (upbeat music continues) (upbeat music continues)
[34:23] (upbeat music continues) (upbeat music continues)
[34:30] (upbeat music continues) (upbeat music continues)
[34:58] I am pretty sure this is what Anthony and I did. I also did new pages with,
[35:22] Oh, I don't know if you saw this, homie. And so I basically want them to enter their Twitter handle
[35:32] and I separately, somewhere, and I'm not sure where in the process,
[35:37] need to enter the Twitter space link. And then it's gonna combine it,
[35:43] the database of the Twitter handle, and then somehow spit out this.
[35:52] Like you can see me pointing at my computer. You kind of can.
[35:54] So it's auto-linking these types of things. So does that make sense?
[36:06] Or do you still think I'm skipping steps? In my head, I'm not skipping a step,
[36:14] but that does not mean I'm not skipping a step out loud. (upbeat music continues)
[36:20] I hope so. I mean, I think a lot of like social media things,
[36:41] like Buffer does it as well, but I'm more just like really wanted to see
[36:46] if I can make it happen, even though there's something probably out there that can.
[36:51] (upbeat music continues) So I am here.
[37:01] We're gonna create a new React app. And also yell at my dog for being annoying.
[37:10] She's not yelling at her, she's leaning. Bingham, meow.
[37:16] Can you stop? Hey, stop, you're okay.
[37:20] You're okay. Yeah, you are.
[37:25] You're fine. I know, she's sassy pants.
[37:32] Sassy pants. All right.
[37:35] Did I just close the one I didn't mean to close? Oh, it just scrolled down.
[37:43] (upbeat music continues) Okay, so pretty sure I already have node.
[37:50] (upbeat music continues) No, dash B.
[38:13] Hey, I got node. Oh, thank you.
[38:22] Okay, so we're doing it there. We have...
[38:28] I don't wanna call up my app. We will do...
[38:42] I don't know if I'm gonna be able to do this. Ha, ha, ha, ha, ha.
[38:50] That's a good one. That is a good one.
[38:52] I'm gonna see if instead of my app, if I can name it Twitter tagging.
[38:59] Let's see what happens. Yes.
[39:05] (upbeat music continues) Oh, Twitter dash tagging.
[39:14] (upbeat music continues) Yes, dash tagging.
[39:28] (upbeat music continues) (upbeat music continues)
[39:35] And homie, I think this was before you got here. The very, very first thing I did
[39:47] was create a new repo through command line so I get used to it more.
[39:53] And so that way, as I am figuring this all out, I at least have it set up.
[39:59] I, of course, will still need to upload, but at least that's in there.
[40:03] I have no idea how long this is gonna take, but hopefully not long.
[40:15] Hey. Happy hacking.
[40:28] Ho, ho, ho, ho, ho, ho, ho, ho. You guys are coming up with some good names.
[40:33] Thank you. Some good terms.
[40:35] All right. So, NPMs.
[40:39] I'm gonna take a screenshot of this because I have a feeling I'm gonna forget it,
[40:43] but I don't need it right now. So I need to do CV.
[40:47] Okay. And that means.
[40:58] Twitter tagging is right here. Oh, it's within.
[41:01] Oops. Well, you know what?
[41:13] We're just gonna roll with this and hope that it works. Why are you saying close VS Code?
[41:23] I'm still gonna be doing things in VS Code. I was just getting it working.
[41:28] Oh, yeah. I did do that, but look,
[41:39] I made it within to a folder within a folder. And I didn't mean to do that.
[41:47] And I did that the second time I've done it. So.
[41:52] So. I'm more thinking that I put something inside of something.
[42:06] So. I'm gonna.
[42:13] We're gonna start over for a second. And I don't remember how to do this,
[42:25] but I want to do it quickly, not necessarily. 'Cause look, I made it within.
[42:31] So I'm gonna do this. We're gonna find out if this was like
[42:44] the most regrettable thing ever, or if this actually helped.
[42:47] I don't know which. (humming)
[42:53] I understand. God.
[43:13] I'm not, oh my God, I knew guys. I am.
[43:19] Tooth factor is so smart. It's just like, when you're trying to get stuff done,
[43:24] it's like, no, just do it for me. But also, thank you for showing me,
[43:29] making sure that. All day.
[43:32] All right. So we will start this from.
[43:37] We will, oh, no, we want to be in. (humming)
[43:48] See me. Desktop.
[43:54] And then do this. We should team life code this, so.
[44:14] (laughing) We should do that sometime, that would be fun.
[44:20] All right. Okay.
[44:45] Yay. All right, so we have the parent folder,
[44:58] which is exciting. Our, wait, what, what, code, oh, there we go.
[45:05] Oh, it's because I didn't cd into that one. Right, well, we'll do that.
[45:12] (upbeat music) Yeah, yeah.
[45:21] All right, this is something that I need to pause, though, really quick, and make sure I do,
[45:25] of getting it uploaded to GitHub. Which I think I just did.
[45:36] GitHub. New repo.
[45:40] (upbeat music) Which.
[45:47] Yeah, it's this one, it's this one. I want to create a new repo.
[46:11] All right, this is not what I want to do. Oh, wait, maybe it is.
[46:20] (upbeat music) We do.
[46:30] (upbeat music) (laughing)
[46:35] Oh, look. Yes.
[46:54] (upbeat music) Oh, I don't like it.
[47:02] I don't know. I actually don't want this, but.
[47:08] (upbeat music) Is there an exit?
[47:15] There's no exit. (upbeat music)
[47:22] (laughing) (upbeat music)
[47:28] Oh, wait. Yes.
[47:43] (upbeat music) Yes.
[47:45] (upbeat music) Yes.
[47:47] (upbeat music) Let's see.
[47:51] (upbeat music) Yes.
[47:54] (upbeat music) Yes.
[48:01] (upbeat music) Eh?
[48:05] (upbeat music) Eh?
[48:07] (upbeat music) Ah!
[48:14] (upbeat music) It's there.
[48:17] (upbeat music) No.
[48:23] No, I have it. It's this weird thing that actually a lot of people
[48:26] have been like, Jen, why are you doing it through Command Line?
[48:29] And I think just because I was familiar enough with Command Line before I started this journey,
[48:38] I was like, oh, I'm just gonna keep doing it this way. And so many people have shown me this way
[48:43] that I'm just like, I'm gonna stick with one thing until I have like it down so well that it's like
[48:52] second nature. Then I'm gonna venture out to other stuff.
[48:55] But we have it. We have, wait.
[49:00] Do we have it? I thought I, aw.
[49:04] (upbeat music) No.
[49:09] (upbeat music) I just did the same thing opposite.
[49:23] (upbeat music) Okay, well, good news is I can just ignore this.
[49:43] This one is already here and I just need it. It's fine.
[49:52] It's fine. I will figure it out.
[49:55] (upbeat music) Okay, I did it the first time.
[50:13] (upbeat music) Upload.
[50:17] (upbeat music) Current project to GitHub.
[50:24] (upbeat music) [50:26],
[50:56] Let's see if this works. (upbeat music)
[51:01], Oh, guys, y'all, y'all, I can't read.
[51:34] (upbeat music) Oh, look.
[51:37] Path to local repository. (upbeat music)
[51:42] If you want your project to belong in organization. Okay.
[51:51] Path to local is this. (upbeat music)
[51:59] I think. (upbeat music)
[52:02] We're about to find out. (upbeat music)
[52:05] Oh, wait. Let me get this.
[52:07] (upbeat music) [52:09],
[52:13] At least I'm making the screen look cool. (upbeat music)
[52:42] Okay. (upbeat music)
[52:46] (upbeat music) (upbeat music)
[52:51] (upbeat music) (upbeat music)
[52:56] (upbeat music) (upbeat music)
[53:01] (upbeat music) (upbeat music)
[53:26] (upbeat music) (upbeat music)
[53:46] (upbeat music) (upbeat music)
[54:09] I don't know if this is gonna work. (upbeat music)
[54:20] Okay. (upbeat music)
[54:28] Refresh. (upbeat music)
[54:32] (upbeat music) Yay.
[54:35] (upbeat music) Okay.
[54:40] (upbeat music) I'm somewhere.
[54:42] I have gotten further. (upbeat music)
[54:48] I think so. (upbeat music)
[54:50] I'm pretty sure. I am pretty sure.
[54:53] (upbeat music) I am there.
[54:55] (upbeat music) VS code and I are fighting again, but that's okay.
[55:02] This happens every time. (upbeat music)
[55:07] Yeah, I don't blame you. I do not blame you.
[55:32] But we haven't made it. This is on GitHub.
[55:40] Yay. Okay.
[55:43] We have, we have made it. We are further.
[55:47] And I, yeah, I really feel like I probably should do that because I've been struggle busting, but all right.
[56:01] So. (upbeat music)
[56:05] Let's try. (upbeat music)
[56:16] Run our NPM start. (upbeat music)
[56:22] Okay. (upbeat music)
[56:31] (upbeat music) (laughs)
[56:35] Hey, what do you know? We have, we have a page.
[56:42] Yay. (upbeat music)
[56:44] I am on a Mac. Yeah.
[56:47] Me and Windows didn't get along very well. (upbeat music)
[56:52] Okay. So this was step number one.
[56:55] We have a lot of steps to go. All right.
[56:58] (upbeat music) SRC app.
[57:03] (upbeat music) Let me do this.
[57:06] (upbeat music) (upbeat music)
[57:11] (upbeat music) (upbeat music)
[57:17] (upbeat music) (upbeat music)
[57:22] (upbeat music) (upbeat music)
[57:27] (upbeat music) (upbeat music)
[57:32] (upbeat music) So SRC app.js.
[57:35] (upbeat music) (upbeat music)
[57:40] (upbeat music) Okay.
[57:42] (upbeat music) (upbeat music)
[57:47] (upbeat music) (upbeat music)
[57:51] Import logo. (upbeat music)
[57:55] (upbeat music) No references.
[57:59] No, that's not what I want. (upbeat music)
[58:03] (upbeat music) Logo.
[58:05] (upbeat music) Go to definition.
[58:09] (upbeat music) I guess we love going here.
[58:17] Now you open node. Oh, there we go.
[58:27] And, um, y'all, I just want to say I may not be doing this and like the most logical order either.
[58:58] But the first thing I want to do is see if I can change one of the logos. That first.
[59:14] Canva. Here.
[59:20] And screw. Well, this one.
[59:46] And yes, for this one, I do think I am going to just upload it here, but I do want to rename this one, but I'm just going to get it.
[60:33] Cool. Right.
[60:35] That means. Okay.
[60:43] Oh, I'm clicking everything. I don't know where I'm going.
[61:27] I'm going to go to the next one. Okay.
[61:58] I'm going to go to the next one. I am, uh, wait, maybe do it in your local project.
[62:47] You can merge trouble, but oh, yes, um, I didn't do that just like the second time. Um, it previously, the react one was named 512 and I named that one 512 and, uh, yes,
[63:13] I am Ryan and I just named the react app something else or the react logo, something else. But I'm just, there we go, we're just going to say, yes, um.
[63:47] That is true. That is true.
[64:01] Um, I would say for both of you, you think developer advocates are the easiest to chat with?
[64:08], because I think they're the easiest to chat with. Oh yeah, it did.
[64:50] It definitely did. That's normally how a lot of these, um, start is by me asking them to hang out with me.
[64:59] Uh, tomorrow's, uh, live stream will be at the normal time, which is 9 AM Pacific, 12 PM Eastern 1600 UTC.
[65:48] Um, that's what I was thinking. But if you, so if I re-enable the app, NPM start, it's doing the same thing, but let
[66:32] me see if it's just caching, it might be caching. It's not caching.
[67:02] No, you won't be sick. Hello? um.
[67:56] I don't know. No, still, it's not a happy camper.
[68:43] Which is okay. I am going to see if maybe it's just used somewhere else.
[68:52] Use the logo PNG, which should be that. Uh, yeah.
[69:04] Oh, maybe it's this. Oh, that's not even.
[69:18] This is off somewhere online, but it uploaded it. Okay.
[69:25] Sorry. You asked to see that and I just disappeared as soon as I saw that.
[69:37] I'll show it to everyone too, but I forget in StreamYard, you can't, um, like copy and paste from there.
[69:51] Yes, that is my GitHub though. Yeah, so this might sound kind of funny, but, um, I wonder if I could just import it from
[70:30] a PNG instead of an SVG, I'm going to take a picture just in case I need it. Uh, oh, I see what I did.
[71:24] I don't know why I did image, but, yeah, there, that's what I thought it was going to do. Oh, you know what, I'm going to do this really quick.
[72:19] What happens? No.
[72:23] Cause I. Oh, I'm sorry.
[72:50] Oh yeah, it's looking for it in the users.js, uh, Twitter tagging SRC. So I was looking at, uh, what is flying or 0 through 3, 3.
[73:20] So I was seeing that it was adding it right here for the, um, srcapp.js because I think it's all this function, I don't know how to do this very well for all of them, but I'm
[73:51] working on it, um, oh, well, that was fun. Okay.
[74:18] I tried it. This is really easy to undo.
[74:29] Import app, just CSS, let's save it. Okay.
[74:58] Okay. I believe it's saying it can't find the logo.
[75:27] You can't import SRC, but if you put the logo in SRC directory, then you have to import it.
[75:35] Um, but if you put the logo in the public directory, you can rename the image, uh, image SRC online.
[75:51] So what I'm getting from that is, okay. So, um, let's see.
[76:34] Yeah, we're going to have to, um. Logo is in the public folder update after I upload each thing into SRC.
[77:18] Oh. Okay.
[77:22] Okay. Okay.
[77:26] Okay. Okay.
[77:30] Okay. Okay.
[77:56] Okay. Ah, it was also, this is a little weird.
[78:53] A lot of weird. We did it.
[78:57] And it also had to do with, it was still trying to import a logo. So I disabled that.
[79:03] Now, if I disable import app CSS, I am pretty sure it will stop the screen. I mean.
[79:17] So maybe we just, oh, goodness. Okay.
[79:24] Don't, I don't want to do that. There we go.
[79:31] And now I just need to go figure out the CSS. I don't know what it is to disable.
[80:14] I don't know what CSS is. Ah.
[80:32] Oh. Oh, no.
[80:45] That wasn't helpful. There we go.
[81:17] There we go. Yay.
[81:38] Okay. Getting somewhere.
[81:46] And then. Okay.
[82:28] I don't know. I'll figure that.
[82:43] Yeah, well, I just wanted to say, like, click here to be a part of the. I just wanted to say, like, click here to be a part, wow, words, words and I.
[83:01] Okay. Well.
[83:24] Okay. Okay.
[83:54] Okay. I don't think it's going to go well because I didn't put it at the string.
[84:27] Oh, we did. Oh.
[84:32] Why do I keep clicking here? What does it say?
[84:53] Learn React. Yeah.
[84:57] Yay. I can't say that it's pretty, but we can change the rest of this CSS later.
[85:03] So. Okay.
[85:09] Let's see what. Is next. So.
[85:18] We got the app there. We have progress.
[85:22] And I have no idea what we would do for. The sequel.
[85:36] Okay. To.
[85:51] Okay. Okay.
[86:23] Let's see. We have some new viewers. So what up?
[86:27] My name is Jen. I am.
[86:32] Probably making this a lot more complicated than. It needs to be, but let me go back to the beginning.
[86:38] I am currently. In Twitter.
[86:55] I host a Twitter space every Wednesday about neurodiversity and mental health and tech.
[86:59] So today I'm working on building an app that if somebody wants to be tagged in it, like what I've been manually doing.
[87:05] It's really annoying like this. Instead of manually doing it.
[87:08] I'm going to be. Placing in what the Twitter space.
[87:13] Link is going to be. I don't know if this is going to be possible.
[87:18] It might be. It might not be, but we are.
[87:24] Luckily Ryan and. Homey are.
[87:28] With me. I'm struggling through it.
[87:36] I have built a few react apps before. It's not been anything too cool.
[87:43] And at the moment. Probably the last like 20 minutes or so we've been working on.
[87:49] Changing. The background.
[88:00] Which I get that I still need to change react app and all that up there, but Hey, we are getting somewhere.
[88:04] So. We are now working on getting.
[88:10] My SQL set up and then importing that. So, and thank you Ryan for tagging all this stuff.
[88:15] And welcome, welcome. And if you feel like talking.
[88:21] I'm curious, what are y'all up to today, tonight, tomorrow? I know we're all in different time zones.
[88:25] So. How to implement a server for.
[88:33] I'm going to. I'm going to.
[89:12] Feel like I need to go. My end goal.
[89:18] Is to implement a server for my SQL. I saw this.
[89:26] So we'll do. I've been.
[89:30] My SQL. I don't know how this is going to work.
[89:35] But we're going to give it a shot. Give me just a second.
[90:17] Okay. Okay.
[91:14] Okay. Okay.
[91:17] Okay. Okay.
[91:21] Okay. Okay.
[91:48] Okay. I don't know how. Because I am wanting to use more open source ones.
[91:54] And instead of like Mongo, which is actually not open source. So.
[92:06] We'll click that we're going to do something new. In my SQL.
[92:11] Next. Okay, let's get building.
[92:18] Create a service. There's a lot.
[92:24] So I'm going to click my SQL. I don't know what happened.
[92:36] Why are you all grayed out? And then we scroll down.
[92:56] And. And we'll go with that.
[93:12] So this is the way I understand it is I'm a hobbyist y'all. Like let's not get crazy.
[93:18] And it's doing it where it's like a month free. Luckily. So I'm just like testing this out as a platform to try it out.
[93:27] And then I'm going to go back to Mongo. And I'm going to try the database services and stuff.
[93:32] I know AWS has one. I think it's like. RSW or something.
[93:40] I don't know why I can't think of it at the moment, but. Basically I'm just trying this out to see if it works.
[93:47] I'm going to go back to Mongo. Just try the Mongo.
[93:50] Or the mango. I always think that when I hear Mongo.
[93:56] I'm like, oh, okay. Amazon is RDS. Okay.
[94:02] Oh, okay. Most functions become available once the first note is up green,
[94:11] including the one we'll show you next. Yay.
[94:16] And power off your service when you don't use it. Okay.
[94:19] That's kind of cool. I am curious though, like if.
[94:25] How to say this. Like, what is the difference between like a managed.
[94:34] Database and an unmanaged database. But like the way I understand it, at least when I was at go, daddy.
[94:40] Was like. Managed meant that if anything broke or anything,
[94:46] somebody else could deal with it. But it costs gobs amount of money.
[94:49] And if you have a managed. And you have somebody that knows how to do it all.
[94:53] It can be a lot less expensive. We're going to find out.
[94:59] All right. So we got a database.
[95:05] That is rebuilding. Okay.
[95:15] We got that far. Okay.
[95:19] Let's take care. Okay.
[95:48] I have a. I have built a new app with a crate.
[95:56] The store I'm using is. On local storage.
[96:02] Now created my SQL database and I wanted to connect database. So.
[96:15] Not speak to my SQL protocol. No.
[96:24] And create a web service and a language of your choice, which could be JavaScript running on node.
[96:29] Okay. Okay. Can we just like, I don't think that.
[96:41] It was Lucas, right? I'm pretty sure it was Lucas. Let me see if I remember.
[96:44] Yeah. Lucas was the one that mentioned it earlier.
[96:50] We needed this. General solution for the.
[96:56] Okay. And react.
[97:00] Okay. You search for any internet configuration of a full stack architecture
[97:10] using react and my SQL. You'll find similar results.
[97:13] Okay. Huh.
[97:24] Okay. We'll have it and you'll have it.
[97:30] Okay. Okay.
[98:11] I would say. First off.
[98:17] Okay. Okay.
[98:49] I don't think I've ever connected. A friend and in the backend app.
[98:54] Hmm. Well.
[99:03] Yes. Okay.
[99:38] Like I should be following all these people. Okay.
[99:52] Okay. Okay.
[100:25] Okay. Okay.
[100:59] Or have fun or BRB or whatever you're doing. I am.
[101:04] Yeah. Okay.
[101:35] I'm going to start trying to do what they're saying in here. And.
[101:39] They're looking pretty. Smart about this because I am.
[101:45] Definitely struggle. It's also really cool to be able.
[101:49] I've done. Next.
[101:53] JS stuff. And I don't know if.
[102:00] Okay. In one of these, I just thought it said.
[102:07] Oh, express. I don't think I've done.
[102:12] I'm going to look. Look at all the past episodes.
[102:16] See if I have. Okay.
[102:41] No, I did next JS. So this one is new.
[102:46] Okay. Control C.
[102:54] I'm going to like it. Just because they took time to write it.
[103:00] Oh, I have a dog. What are you doing?
[103:09] I mean, that is a solid question. Okay.
[103:20] I'm not going to lie. And what.
[103:23] I. When next year has to be able to do the same things on the backend.
[103:34] No JS would. Because the goal is to do.
[103:41] So. My Google's.
[103:49] Is how I got to know jazz. Not that that's necessarily the best reason.
[103:53] Okay. Okay.
[104:45] Okay. Okay.
[104:50] Okay. Okay.
[105:27] Okay. The reason is because it says backend is node express.
[105:36] Or like database connections. And at least the Google's is saying that next JS is front end.
[105:44] And. Thank you, Ryan, for visiting.
[105:51] Yeah, I don't know if I can make it a full three hours going through this because.
[105:54] Okay. I can only do an extra stream tomorrow to finish working through this.
[106:03] That is a good call. I don't know.
[106:12] I think. For now, I'm going to just.
[106:17] Do this app. But.
[106:22] Okay. Melty brain.
[106:30] Oh, okay. Hmm.
[106:40] All right. I feel like I'm getting melty brain though, because like.
[106:49] Yeah, I don't know. Interesting.
[106:55] But. I mean, I could definitely do something else just so that we can kind
[107:06] of see if this is what I'm setting up right now. And working on making it.
[107:11] So that way it posts my Twitter. Who wants to be tagged in Twitter every week.
[107:16] Because right now I'm manually doing it. Okay.
[107:24] Tell me next task has the backend connected for you already. I felt like I'm like not computing words right now.
[107:36] Is where I feel like I'm going. Okay.
[108:05] That's kind of where I'm at is I'm like, I'm not computing. Like right now, like y'all are clearly speaking normal words.
[108:11] So I feel like I've. Made it.
[108:15] And definitely got through a lot. I need to make sure that I.
[108:24] Okay. Okay.
[109:21] Okay. Okay.
[110:14] Okay. Okay.
[110:25] Okay. Okay.
[110:56] Okay. Okay.
[111:03] Okay. Okay.
[111:05] Okay. Okay.
[111:07] Okay. Okay.
[111:57] Okay. Okay.
[112:02] Okay. Okay.
[112:08] Okay. Okay.
[112:25] Okay. Okay.
[112:29] Okay. Okay.
[112:58] Okay. Okay.
[113:09] Okay. Okay.
[113:13] Okay. Okay.
[114:00] Okay. Okay.
[114:10] Okay. Okay.
[114:14] Okay. Okay.
[114:18] Okay. Okay.
[115:09] Okay. I can listen to my own music.
[115:33] I honestly just like block it out. I used to listen to.
[115:38] What is it called? No, no, no.
[115:48] Honestly, I think it's called like. Spotify, please tell me. I don't know if Spotify, like it's mad.
[115:58] Or like YouTube gets mad to say upload this on YouTube too. If they would get mad at this kind of stuff.
[116:07] Okay. That is who I normally listen to.
[116:12] Do you have any suggestions? Let's see. It does let me add music.
[116:17] Only upload music you have authorized. You are authorized to use.
[116:22] Okay. I feel like I don't.
[116:35] Okay. Oh, I feel like maybe I don't have to have it on. No, it does.
[116:43] Oh, wait. It doesn't look.
[116:47] Turn the loop off. I can't do that.
[117:02] I don't know why it's not working. It just keeps playing through them all. If we do it like this,
[117:08] which could be a winner. Okay.
[117:39] Okay. Okay.
[118:20] This finally updates that you guys kind of see my screen for a minute. Might actually be out of here.
[118:25] No. Okay.
[118:40] No. All right. I don't know.
[118:43] I have. So I am signing off.
[118:48] I will let you know about the music next time. If you have suggestions, please like, you know,
[118:53] Hit us up. All that stuff.
[118:58] And I will be back at some point. On this as well.
[119:02] Okay. All right. Bye y'all.
[119:09] Have a wonderful day, week, evening. Bye.

