---
showLink: "https://www.youtube.com/watch?v=QTctf0aDNBo"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-github-how-and-why-developers-store-their-code-on-github-with-rizel-scarlett"
title: "Teach Jenn GitHub -  How and Why Developers Store their Code on GitHub with Rizel Scarlett"
publishDate: "2022-07-13"
coverImage: "https://i.ytimg.com/vi/QTctf0aDNBo/maxresdefault.jpg"
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

[00:00] >> Hello, hello. Thank you everyone for joining Teach Gen Tech.
[00:06] I am slowly getting used to saying that instead of shit you don't want to talk about.
[00:11] Keep catching myself, I'm like, "No, it's not my podcast, it's Learning Tech."
[00:15] Today we have Rizal. Am I saying your name properly?
[00:19] >> Yeah, you are perfectly. Some people be saying Rizal, Rizal, but it's Rizal.
[00:25] >> Sweet. As most of my guests have known, I'm horrible at names and I'm working on them.
[00:32] I'm glad I got one of them right. This is exciting. Please introduce yourself and a bit about
[00:38] what we are going to go over today. Hello, hello, lovely people joining our stream.
[00:45] >> Hey everyone. My name is Rizal Scarlett. I'm a Developer Advocate at GitHub.
[00:51] I've been here for about 10 months or so. In the past, I was a software engineer,
[00:55] but I like doing this way better because I get to talk with people again.
[00:59] What we're going to talk about is I'm just going to do a little introduction to Git and GitHub because I remember,
[01:06] when I first chatted with Jen, she mentioned that she knows
[01:10] a little bit about GitHub but wanted to know more. >> Yeah. Anthony had me put something with Git,
[01:19] and I'm following directions, but I don't quite comprehend it,
[01:23] so I'm pretty excited that we're going through this today. I will go ahead and get your deck loaded,
[01:31] which by the way, y'all, StreamYard is pretty legit in its ease of use.
[01:36] It doesn't do everything everyone wants, but it's actually pretty easy. I'm excited.
[01:40] >> Yeah, I love it. I'll get into this. Basically, this is a deck that I use at other talks,
[01:46] and I'm not going to do it in the talk like way, but I'm just using it to guide me to make sure I don't ramble.
[01:56] But basically, first, I usually start by telling people that software engineering terms are confusing.
[02:05] Back in the day, I used to think Java and JavaScript were the same thing.
[02:08] Apparently, they're not. That's the same for Git and GitHub.
[02:12] I don't know if you already knew that, Jen, but for anyone listening,
[02:15] plus you, Git and GitHub are not the same thing. They're completely different,
[02:20] but they are interdependent on each other. At least GitHub depends on Git.
[02:28] First, I'm going to talk to you about, let me just skip through all this that I have.
[02:33] >> You have a cool deck though. I'm enjoying all the animations.
[02:37] >> Thank you. Shout out to Canva. But first, we're going to talk about
[02:42] the difference between Git and GitHub. Then I'm going to talk
[02:46] about a couple of features that GitHub has, and then we'll walk through uploading things to GitHub,
[02:54] depending on how much time we have. I might show you the different ways
[02:57] that you can upload stuff to GitHub. If not, we'll just do one.
[03:02] >> I'm stoked for this because when I first started learning JavaScript, probably only a few weeks ago,
[03:11] I was doing it on LinkedIn, and it wanted you to download Git.
[03:16] I believe I'm going off of memory, and then I was like,
[03:21] "Well, why don't I just use GitHub?" I didn't understand the difference and even Googling it,
[03:27] I'm like, "Okay, they do two different things." I got that far. That's all I know.
[03:31] They have two different things, very similar names, and that's it.
[03:35] >> Yeah. No, I was the same way. I was even working as a software engineer,
[03:39] I'm telling people, "Yeah, I know Git," referring to GitHub or vice versa,
[03:44] not realizing they were two different things. No worries. Git is a version control system,
[03:53] and I usually tell people, "Yeah, okay, so what? What is a version control system even mean?"
[03:58] Basically, it's something that enables you to record snapshots of your projects as you save them through history.
[04:08] If you make a change to one of your codebases or your projects, it allows you to save it and be like,
[04:15] "On June 25th at 1 PM, I made this change and I saved it right here."
[04:20] The reason why this is relevant or important, I usually give this example that think about,
[04:30] well, for me, I have a lot of different versions of my resume. I know you probably can't see the screenshot as clearly,
[04:37] but basically, it says copy of Rizal, Bob Simple's resume, that's my maiden name, Rizal's resume 4, Rizal's resume 1.
[04:44] It's very hard to tell the differences between them and why I made them.
[04:49] Sometimes I've made them when I was in school for scholarships or for different jobs.
[04:54] That can be the same with software engineering. Imagine you have many different versions of code.
[05:02] In addition to that, right now, it's just me working on my resume.
[05:06] But once you're working on a team with multiple different people, that makes it even harder to
[05:12] track and things can be poorly named and stuff like that. >> Real quick, after this,
[05:19] can you share your deck so that way we can share it out? We had a comment about it and I'm like,
[05:24] this is going to be so good even for myself to go back and be like, "Okay, what's the difference again?"
[05:29] >> Cool. Awesome. Yeah. If you're wondering what different versions
[05:35] they would even have in codebases, you'll have the production version or people call it a branch,
[05:41] where that's what users are using and touching. Then if you find out or a user reports a bug or you have to add a new feature,
[05:50] you'll make a copy of production on your local computer. Then now you have a local version that you've updated and changed and added.
[05:59] You either fix the bug or you added a new feature on, so that's a little bit different than production.
[06:04] Then you'll put it up to another version called staging, where everybody tests their code
[06:09] before it goes out to production to see if everything's working. Just giving more examples of the different versioning,
[06:17] because before I worked as a software engineer, and I know you've had a lot of more experience in tech,
[06:22] but before I worked as a software engineer, I was just like, I don't know why they would have different versions.
[06:29] >> No, that is so helpful. Also, I think something that I always got really stuck on is,
[06:37] I believe this is GitHub instead of Git, but the master or the top level,
[06:43] and I think that's on GitHub, so I'll ask more about that question later,
[06:47] but it's like all of these blurred together from my past knowledge. I'm excited that we're picking them apart finally.
[06:55] >> Yeah, and I can even answer that one right now. Master would probably be your production version.
[07:03] I think they've started to stop using that word, because the origin was like master slave or something like that.
[07:12] Then once the George Floyd stuff started coming out, people were like, "Yeah, let's change
[07:17] our terminology because it's messed up." People have been using the term main now,
[07:23] but somehow codebases are still on master because it's a lot to migrate over. But that's a good question.
[07:29] >> Thank you. >> But basically, Git manages all the different versions for you,
[07:35] so you don't have to manage them yourself, because doing it manually is a pain in the butt.
[07:42] It'll tell you what the latest version is, who made the specific changes,
[07:48] why those changes were made, because sometimes you'll see a change in
[07:51] the codebase and you'll be like, "What the heck is that?" Usually, people use Git in the terminal or the command prompt.
[07:59] I've seen you using it when Ramon did his session, so you are familiar with it.
[08:06] Usually, I tell people, it looks like the thing on movies where people say,
[08:09] "I'm hacking into the mainframe," but it just helps you interact with the computer. You know that.
[08:14] >> Really, really quick. Can we just comment? I get that I can't really,
[08:17] I am starting to just put code on the screen and going into a browser, and I'm like, "I feel like a hacker."
[08:24] I'm like, "I can't do anything, but I feel like a hacker."
[08:28] >> It does. That's what I thought engineers were doing when I would try to imagine.
[08:34] I'm like, "What the heck are engineers doing? They're hacking into the mainframe or something?"
[08:38] But no, it's not that cool, but it still does feel fun.
[08:45] >> Thank you, Ramon. >> Ramon, I'm not even looking at the comments. Hold on.
[08:53] Hey, people. I was literally in the private chat section. Ramon already knows this deck because I actually did
[09:01] this at his coding bootcamp. >> Please.
[09:05] >> Yeah. Then for GitHub, you've used that a little bit,
[09:10] so you know it's a web platform. At the simplest level,
[09:17] it's a place that developers store their code. I remember you talking to me and you were like,
[09:22] you think companies do or something like that? Yeah, like open-source maintainers,
[09:27] companies that have private code, people that are storing their own personal projects.
[09:34] Some people actually even store their blog post or just regular written content on there.
[09:40] It's just like Google Drive for code. But there's a whole bunch of other stuff on there.
[09:48] There's security features on there, there's automation features called GitHub Actions.
[09:53] I don't know if you've heard of GitHub Copilot. There's so many things on there,
[09:56] but at the lowest base, the first thing is you store code on there.
[10:02] Does that make sense? >> It does.
[10:06] The question that's coming to mind right now is, why would someone use Git instead of GitHub?
[10:12] >> Git is helping you to manage the versions, and GitHub is just storing the code for you.
[10:24] Let me go through the rest of this and maybe it will make more sense. >> Yeah, for sure.
[10:28] >> Yeah, I usually get really wrinkled. Let's see. Here, this should answer it, I think.
[10:37] GitHub is a website that uses Git to show you all the changes that you made to your code.
[10:43] You'll put your code on GitHub using Git, and then Git will recognize the changes that you made,
[10:50] the times you made them, and it'll display it to you in GitHub.
[10:55] I think I have a couple of screenshots coming up. Basically, you're using GitHub because it
[11:01] makes it easy for you to share your code with other people. Sorry, I just started coughing.
[11:08] But back in the day, I heard, before I was a software engineer,
[11:12] I heard people were sharing their code via e-mail, via FTP, and different stuff
[11:20] that made it really hard for them to share it amongst each other. Having Git was really helpful,
[11:26] but having GitHub is even more helpful because people can just send a link to each other and be like,
[11:31] "Hey, here's my code." Then Git will do the magic behind the scenes at recognizing,
[11:40] here's when it was changed, here's when this project started, and stuff like that.
[11:45] Real quick, that is pretty funny, Joe, and hello, Dustin, what up?
[11:52] Real quick, that makes sense, but I guess where I'm stuck is,
[11:57] and again, this is all pieces just because learning out of order, causes the confusion a lot too,
[12:04] is I used to work at an API spec company called Stoplight. When you would log into a project and create a project,
[12:14] you'd have a connect to Git or GitHub, and then it would make it so that way,
[12:22] if you submitted something, it would create a branch or you could submit it to the main branch.
[12:31] But I guess where I'm confused is, can't you have versioning there like you can in Git?
[12:40] >> GitHub is using Git to identify when you're on the main branch, or identify what you're submitting it to.
[12:50] GitHub is just visually showing you those changes, or visually showing you what you did,
[13:00] whereas Git is identifying that you submitted this on the main branch or here are the different branches.
[13:07] Does that make sense? >> It's like GitHub is the UI or the website for you to see it better,
[13:16] rather than just looking in your terminal. Because before, people were just looking in
[13:20] their terminal, I guess, to see all of that. Then GitHub is where you can actually see it,
[13:26] and see what happened, and what changes are made,
[13:28] and you can use GitHub. I don't know if that's making any sense.
[13:35] >> It's starting to make sense. Git is like you're just using it in the terminal,
[13:40] and GitHub made it so that everyone can see it. Because not everyone can see your terminal,
[13:46] not everyone can see what's going on within your terminal, because that's just on your local computer.
[13:53] Now that you're using GitHub, which is on the Cloud and your code's on the Cloud or whatever,
[13:59] everybody else can, if you make your project public,
[14:03] everybody else can see what's going on. GitHub is just reflecting the changes that happened within Git.
[14:09] People can, in the comments, go ahead, feel free to add in more clarification there,
[14:15] because I don't think I did a great job. >> No, it does make sense.
[14:20] It's starting to make sense. I think it's going to be a lot of like when we go through it,
[14:24] it'll make even more sense. >> Yeah. I think I'm going to do you doing it from
[14:28] the terminal and then within GitHub's UI, and then hopefully it'll help it click a little bit more.
[14:34] >> As Joe was saying, GitHub is a collection of repositories.
[14:40] It's a lot of things. Here's my GitHub profile. It reminds me of a social media network
[14:46] because I have followers, I'm following people. It says a little bit about myself here,
[14:51] and it talks about different orgs I have. But most importantly, it has all the repositories I made.
[14:58] Repositories are just folders that hold your different projects, or projects that I've interacted with.
[15:07] I've interacted with OpenSoft, which is an open-source project.
[15:11] I made my own projects. I got a social card generator over here.
[15:15] If we go deeper into that project, it'll show me the different files that exist.
[15:21] I have a gitignore file, a readme, a JavaScript file, a package.json.
[15:26] I have here, it reflects which branch, or which version of the code is on it.
[15:32] You can interact with that, click that little drop-down,
[15:35] and you'll see the different branches. You'll click it and be like, "Oh,
[15:38] what happened in this branch?" On someone's local branch,
[15:42] or what does it look like in production or staging? I hope that gives a little bit more clarity.
[15:49] This is the UI to see what's going on within your code. It just makes it look better.
[15:55] You can also see right here, it has how many days ago things were changed and updated.
[16:01] It says 20 days ago. I'll stop if you have any questions.
[16:08] >> No, I'm just going to give you what I've been telling all the other guests of like,
[16:12] it makes sense, but it doesn't make sense. I'm just going to let it soak in and we'll keep going.
[16:18] >> Yeah. I think sometimes things start to make more sense as you make your own projects.
[16:23] I hope that helps. I also circled in on one of these files here.
[16:32] If I clicked on the generate social image JavaScript file, it went backwards.
[16:39] No. If I click on there, I'll see the actual code that I wrote.
[16:46] This is some really terrible code I wrote that you can see. But that way, just showing you,
[16:53] people can literally see what's inside of this file. Then you can also see commits.
[17:01] What do we do in the event that we submit applications that are rejected by the bot?
[17:07] To whom do we appeal? What bot? I'm confused. No lie.
[17:12] What bot are you talking about, Joe? There's a lot of bots on GitHub.
[17:23] I don't know. When Joe comes back, I'll try to answer that.
[17:29] But commits are just another way of saying changes that happened in your code or times
[17:39] that you saved changes inside of your code. Like you can see here,
[17:44] on January 14th, I made an update. On January 4th, I made an update and it even has
[17:51] the message that I added just to let people know. Could they mean CI bots that review code?
[17:59] Winget installer. To be honest, Joe,
[18:03] I don't know too much about that. But I could ask somebody at GitHub.
[18:08] I don't think I've interacted much with that Winget installer. Yeah, sorry.
[18:18] But basically, what am I saying? I can leave a message of why I added certain changes.
[18:30] I say right here that this was a fix to add a comment response. You can see that bdougie,
[18:36] who's my manager, added something to the code base. You can see mtfoley updated a file called readme.md.
[18:43] If you wanted to, you can click on each of these commits and it'll show you
[18:47] the exact change that was made. That message just gives context as to why.
[18:52] Because sometimes somebody made a change to code and you're like, this change makes no sense, why would you do that?
[18:59] But having that context is good, and you can always go back to the person and be like,
[19:04] hey, bdougie, why did you do this? I see that you made this message,
[19:08] I see that you updated this code, but I need to have more context on why.
[19:12] >> On that note, the commits makes sense, and I'm guessing you're going to be going through this,
[19:19] but I just want to call it out so that way in case you're not, we know. What is a PR and is that different from a commit?
[19:31] >> Good question. A PR stands for pull request. What you're essentially doing with a pull request is you're
[19:40] saying whether it's an open-source project or your company's project
[19:47] or somebody else's project, you're saying, I see that you have this code,
[19:51] I want to contribute or add my changes to it. But because people don't want people just
[19:58] jumping in and changing their code all willy-nilly, it's like you're saying,
[20:03] here's the change I want to make. Do you like it?
[20:07] If yes, the person will approve it and merge it into their codebase. If no, they'll leave a couple of comments for
[20:16] review to say, can you change this first, and then they'll merge it in.
[20:20] Pull request is like a little bit of a stopper to say, hey, this person wants to add code to your codebase,
[20:27] are you okay with it? You'll open up a pull request.
[20:30] Then the way that it's different than a commit, is a commit is just a saved spot
[20:43] or saved snapshot every time you make a change within a codebase. It's like pressing the "Save" button
[20:50] on your Google Doc or something, and it'll just say, "Oh,
[20:54] this was saved at 5.42 PM." The reason that's helpful in addition to this,
[21:01] is if you're coding on your own and you're like, "Yo, this new change I made doesn't work,
[21:08] it ruined everything," you could always go back to 5.42 PM or 3 AM or whatever you were coding,
[21:16] and it'll bring you to that point in time. Does that make sense? >> Yes. Once a PR is approved,
[21:24] will it show up as a commit or no? Because it wasn't a save,
[21:27] it may just go into an approved branch or a different branch. >> Yeah. It'll show up as a merge commit.
[21:35] Right here, you can see BDougie made a merge commit. He merged somebody's,
[21:41] I think he might have merged MT Foley's change. Yeah, right here. He merged MT Foley's pull request,
[21:52] and now it shows up as a commit right here. >> Okay.
[21:57] >> GitHub is a lot, Git is a lot. People have a hard time understanding it,
[22:03] and there's no way anybody can know everything about it. Just to get [inaudible]
[22:07] >> Thank you. I'm getting there. I'm getting there. I'm following along,
[22:11] but at the same time I'm like, I still don't get it, but I get it.
[22:15] >> It's so much. I wrote a blog post once and someone was like, "If you don't understand Git, don't write about it."
[22:22] I'm like, nobody understands everything about Git, relax. >> I loved your Struggles of a DevRel.
[22:30] >> Thank you. >> I love that one.
[22:32] >> Thanks. I appreciate it. Also, I just wanted to make you aware that GitHub is not
[22:41] the only platform you can use, not the only website that stores code.
[22:48] It just has a bit of a monopoly, I guess. When I wrote this, it had 73 million users.
[22:54] It has way more now. But there's other options like GitLab, Bitbucket,
[22:59] GitBucket, AWS CodeCommit, SourceForge. I like to make people aware of this because
[23:03] after I graduated my coding bootcamp, I had learned GitHub and then I
[23:07] joined the job and they were using Bitbucket, and I was like, what is this?
[23:12] >> Those are all just different company names and different websites using it,
[23:16] but they all basically do the same thing. >> Yeah. Basically, all do the same thing.
[23:20] >> Basically, all interact with Git or a similar version control system.
[23:28] There's other ones like Mercurial and, I don't know, things that people don't use anymore.
[23:35] Maybe people in the chat know them, but yeah. >> Now, for something,
[23:43] and this could be a piece I'm missing too. We've done stuff on VS Code.
[23:49] >> Yeah. >> So when we do stuff to VS Code,
[23:53] if it is, I'm trying to work on thinking this out, and it creates a project in GitHub.
[24:07] I don't know where I'm going with this question. I know they talk together,
[24:11] but I don't know how or how to break that one down. >> I think you would and we could try this out.
[24:18] You would go in VS Code, you will start typing some code,
[24:23] and then when you're like, "You know what? I don't want to lose this,"
[24:27] because you could totally lose your code from VS Code. Let's say your computer shuts down forever.
[24:33] You're like, "Okay, I'm at a point that I think this is good."
[24:36] You'll write Git in your terminal, and you'll use Git to push your code to GitHub,
[24:45] or to store your code on GitHub. >> When it's in VS Code,
[24:51] it's just that's like a text editor thing. Then when you push a Git,
[24:58] that's when it creates a Git, so it creates a Git file,
[25:02] and then it'll push to GitHub? >> Kind of, yeah. That's pretty close.
[25:09] Yeah. You'll type in your text editor. Yeah. You'll use Git,
[25:14] and then you'll say, "Git, I want this to go to GitHub.
[25:17] I want this to live on GitHub." It'll be like, "Okay," then everybody can see it,
[25:23] or you'll be able to access it from that URL. Ramon said he used a version control system called Subversion,
[25:36] and I agree with Joe. I hate Mercurial. Well, not hate.
[25:39] I'm not a fan. >> I know it's a lot, sorry.
[25:45] >> No, you're good. I'm getting there. >> Cool. Now we're going to talk
[25:50] about how to store code on GitHub. We're going to create a GitHub account.
[25:58] You have that. You install Git via your terminal. You might have that.
[26:02] I think you mentioned that. If not, we'll do it. It'll look like that.
[26:07] This is the website where you sign up, and then if you were installing it in your terminal,
[26:11] this is how it will look. We'll do that later. You're going to create a repository,
[26:16] and a repository again is, maybe we should do this right now.
[26:22] >> Okay. >> Yeah. Let me stop sharing,
[26:30] and then you can share, and we just do this.
[26:35] >> Okay. >> Joe said, "Do you suggest
[26:38] using the desktop application for GitHub and Git?" Oh my gosh, wait, that's actually at the end of this.
[26:44] >> Okay. Let's go back. >> Yeah. Well, first of all,
[26:51] I think it's a good option for people who, I learned that scientific researchers and stuff like that,
[27:00] store code on Git, but they're not really necessarily familiar with Git.
[27:08] Well, sorry, scientific researchers store code on GitHub, but they're not necessarily familiar with Git,
[27:14] and they may not have time to learn that. Or like a beginner too,
[27:17] who's just learning to code, they may not know Git,
[27:21] so I think it's completely fine to use GitHub Desktop. In fact, before I worked at GitHub,
[27:27] I thought, "No, you've got to use the terminal." Then now that I'm working here,
[27:31] there's so many people just using GitHub's web UI, just dragging and dropping things,
[27:37] just editing the files directly. I know there's other tooling,
[27:43] like GitKraken and stuff like that, I'm all for it. Whatever works to help you submit your code, do it.
[27:50] Because the important part is making sure that you store your code and you have those different versions.
[27:55] Because I had people tell me they're using Dropbox. I'm like, "Please, don't use Dropbox."
[28:01] It's okay that you jumped ahead because I think I was going to skip this.
[28:06] Because it was something I say. >> I was just about to say, it's so good
[28:11] to just ask these questions because even if it is making us skip ahead,
[28:16] we got to learn and we're doing this together. That's why it's Teach Gen Tech because I'm like,
[28:20] there's other people that don't know this stuff. >> Exactly. Someone said, "Drag and drop gang."
[28:26] Yep, I agree with that. Go ahead and share and I will walk you through this first thing.
[28:33] >> Yay. >> Cool.
[28:36] >> My photo is really big over here, so we can minimize that a little bit.
[28:40] >> But it's so cute. >> Thank you. Great photographer here in Denver.
[28:45] If anybody needs one, I know one. >> I think we have time to do multiple options.
[28:56] Let's do it in the GitHub UI first, then we'll do it in the terminal.
[29:03] You don't even need the terminal for this one. Let's just do it, yeah.
[29:07] You can just make that one bigger. We're going to go to,
[29:12] on the top right-hand corner, there's a plus sign.
[29:16] We're going to click "New Repository". Basically, repository just is
[29:22] a folder for whatever project you have. Let's go ahead and click that.
[29:26] >> Really quick, new organization, I'm guessing that's just like a different company or something,
[29:32] you want other people involved. But what's a new gist?
[29:37] >> I barely use those, but it's like people save code snippets in there,
[29:43] from what I've seen. I've literally never used it. I haven't found a reason that I needed to.
[29:48] But whenever I see people use it, it just has a code snippet that they want to share with people.
[29:53] >> Then import repository, can that do it with VS Code?
[29:58] Is that where you would import something or am I just still not doing it?
[30:03] >> No, I think you're right. It's like if you were on Google Drive
[30:07] and uploading a folder that existed on your computer. I think you can upload a folder of code that exists
[30:13] on your computer that you wrote in VS Code or something like that. I haven't used that much either, to be honest.
[30:19] There's so many ways, you just made me realize that that way is a thing.
[30:24] Let's go ahead and we can name this repository. I don't know, what do you want to name it?
[30:33] We can call it learning GitHub, I don't know. Cool. [inaudible] Jen is the best.
[30:43] Cool. Then you can see that there are options to make it public or private.
[30:47] Let's just make it public. People that make things private,
[30:51] it's maybe they don't want people to see their code yet, or it's a proprietary company and they're like,
[30:56] "Don't steal my code." We can go ahead and add a README file.
[31:02] >> Do people ever look at the README files? >> You said do people not or do they ever?
[31:08] >> Do they ever? Because I feel like when I install something on my computer,
[31:12] I never read the README file, but I don't know if it's different for code.
[31:17] I think I'm not a big reader either when it comes to technical things,
[31:23] but there are times where I do have to read it. If I want to contribute to an open-source project,
[31:29] that'll have links and information on how I should interact in that project.
[31:34] Then sometimes at different jobs I've had, people would use that as an area for documentation.
[31:41] But it's just like, "Hey, this is my project, here's how you use it."
[31:46] But I don't always read it. >> Good call, Ramon. He said,
[31:51] README files are super helpful for getting started. >> Yeah.
[31:55] >> So I should probably read them. >> If you need to,
[31:58] if you're like, "I know what to do," you're good. But if it's an open-source project or a company,
[32:03] then you're like, "I don't know what to do," it'll tell you. Cool. It already says that it's
[32:08] setting main as your default branch. I didn't explain branches that much to you,
[32:14] but basically, you'll have this main version of your code, and you can "Branch" off of it and add changes.
[32:24] Then once those changes are added and you're ready, and they look good to you,
[32:27] you can merge it back into the main branch. >> How many branches are normal?
[32:35] >> A million, I don't know. >> If I'm working on a project,
[32:40] how many branches is good to have or not have, or do they just chill there for forever?
[32:47] >> Hey, AJ, it's a good practice to delete your branches after they were merged.
[32:55] But I don't think there's a set number of how many you should have. It's just how many you need type of thing.
[33:04] It's almost like asking how much? I don't know.
[33:10] >> Okay. These are the random things that I get stuck on, so I appreciate it.
[33:16] >> These are good questions. But yeah, I don't know.
[33:21] I've seen a various amount, and it's just depending on how big the project is.
[33:27] There's no rules or anything about branches. It's just nice to delete them after you're done,
[33:32] that way you're not being cluttered. >> I get that. Hi, AJ,
[33:37] and thank you for joining for a bit. Next question for you, Rizal.
[33:43] Add the what? >> The gitignore.
[33:48] Yeah, that's a place where, how can I describe that?
[33:53] It's a file. We can add it if you want. But it's a file,
[33:59] and actually they have different templates, and this file essentially tells you,
[34:06] how do I say what I'm trying to say? It tells GitHub to not upload certain files within your project.
[34:16] If you have secret passwords that people can easily look
[34:24] through and scan your code base and stuff like that, you can say, "Hey,
[34:28] don't put that file in there," and GitHub will ignore that file and not add it.
[34:33] Or if you have dependencies and libraries that will make uploading
[34:39] your project and downloading your project take forever, you can say, "Hey, don't add those."
[34:44] This is literally its name, telling Git, "Ignore these files." Does that make sense?
[34:50] >> It does. Thank you. I think we went through licenses yesterday.
[34:56] >> Yeah. >> I bet. Yeah, we did the MIT license.
[35:00] Cool. I remembered. Yay. >> Cool. Let's create this repository.
[35:08] One of the simplest ways to add a new file is where it says, "Joe said most coders,
[35:20] in my honest opinion, are not super organized, so that they are in branches that go somewhere as a benefit."
[35:28] Yeah, we're not organized. Go ahead and just click "Add File."
[35:34] This is one method of adding code, and we can say, "Create new file."
[35:40] Are you familiar with HTML a little? Because I was thinking of making an HTML file.
[35:48] >> That is groovy. I've been working on JavaScript,
[35:52] although I think he's going to be coming on tomorrow to do a code review from my very first stream.
[35:59] I think I ended up actually writing it in HTML instead of JavaScript, but we'll find out.
[36:05] >> Okay. Well, we can make this super simple then. You can name this index.html.
[36:14] Perfect. Then in edit new file, we can just do an h1.
[36:24] I don't know if you're familiar with that. Perfect. Then you can close that tag with a closing h1,
[36:33] and inside of it, we can add whatever you want.
[36:38] You can say Jenna's the best. >> All right.
[36:46] >> Yeah, so it's remote, so it's everybody that really sat down here to join the stream.
[36:54] >> Right. These are people that show up often, so anybody else keep showing up and you'll get added to this list.
[37:02] >> Cool. Now we made this file. Let's scroll down and shout out to Ramon,
[37:11] and I don't know how to say Jerry's name. Is it Jerry? >> I'm saying it wrong.
[37:17] I've tried really hard for it, but it's like Jarry.
[37:23] There are roles, I'm pretty sure. Join tomorrow night and we'll be
[37:28] able to have him say his name seven times. >> Perfect. Then what we're doing right now is we're going to make a commit.
[37:37] We're just doing it in the user interface, and we're saying we want to save this.
[37:41] We'll commit it directly to the main branch just for the sake of this demo. >> Then something that I'm just realizing that I
[37:52] saw that was different here is creating the file here, it doesn't have all the pretty stuff that VS Code really
[38:02] helps with where I'm like it didn't auto-close my H1 or anything like that. I'm like, "Oh, I like that VS Code does that."
[38:11] >> Yes, I do too, and that's why people don't normally write their code inside of GitHub.
[38:18] They just use it to push their code up. I'm just showing you so you can be able to connect the dots once we do that.
[38:26] >> Yes, and it's so helpful because I wouldn't have thought of that. This is why Bold Bearded Builder says this is why he never,
[38:34] they never, I really need to start working on pronouns y'all because I'm always like, I need to not assume that they have.
[38:43] >> Commitment issues, that's hilarious because they have to do commits. >> Yes, all right.
[38:50] >> Wait, before you do that, actually you can make a commit message. In the top bar,
[38:57] it defaults to saying create index.html, the one above it. >> Okay.
[39:02] >> But you can give more detail or whatever. You can say, "Created an h1 element inside an index.html."
[39:13] >> Yay, that was super exciting. >> Yeah, and then we can go ahead and commit that new file.
[39:32] >> All right. >> Cool. You have your first repository,
[39:39] you created a new file, you committed a new file to there.
[39:45] We can do the same thing in the terminal. >> Okay.
[39:52] >> Also, great job. >> Thank you. Other than seeing it in terminal,
[39:59] if we have time, seeing it in VS Code I think would be so helpful.
[40:03] >> Yeah, sorry. We're going to use the terminal,
[40:08] but we're also going to use VS Code. >> Okay, sweet. Because I was like.
[40:13] >> You can't, yeah. >> Which I'm pretty sure we did yesterday with Ramon, a bit.
[40:19] Ramon, I feel like he had me create my own folder that I put code into, and then we made a file and put it in there.
[40:30] I don't remember all those steps, but we did. >> No worries. One thing we need to do before we do all of what you're doing,
[40:39] I was going to clone this repository that you just named. Basically, if somebody else wanted to use your project or contribute to your project,
[40:52] yeah, they can use the GitHub UI and edit the files directly there. But like you mentioned,
[40:57] there's no highlighting, there's no linting to tell you if you made a mistake,
[41:01] there's nothing to help protect you. What people like to do is download it or
[41:07] clone it to their local repository and use VS Code. >> Really quick, something that you said that I know what it is,
[41:16] but I feel like any noobs like me normally wouldn't, is linting. Linting is a tool that will tell you if you have mistakes,
[41:25] and it is really helpful. There's a lot of linting tools out there,
[41:34] seeing if I can talk. I like to think of it as it's like a spell check for your code.
[41:39] >> Yeah. It is. It's like Grammarly. >> Yeah. It's like Grammarly and spell check put together.
[41:47] But I just wanted to call out that's what linting is because that was a really hard word for me to remember what I did because I'm like,
[41:54] it's not removing lint, so why is it called linting? >> No, I understand.
[41:59] It's a weird concept. Thanks for calling that out.
[42:03] >> Yeah, for sure. >> Click the "Code" button and that should have instructions.
[42:09] Okay, cool. Then where it says, you see that https/github.nl has a copy button?
[42:16] Yeah, let's copy that. That's like the URL for this repository.
[42:21] Now we're going to head to the terminal and go to a folder that,
[42:29] well, do you know how to navigate to different folders in the terminal? Okay, cool. Go to a folder that you want to save this to.
[42:35] Cool. >> I got to remember what the folder is called.
[42:38] It's called code folder. >> Cool.
[42:40] >> Okay. Let's see if I remember what Ramon said. It's called code-folder, if we want to do it.
[42:49] >> If you don't remember, you can do ls and you'll see
[42:54] where you are and what folders exist. >> How do you do it without the quote marks?
[43:01] Is it a dash or is it? >> I don't know if I know the answer to this question.
[43:07] >> That's okay. I'll do it the way I remember doing it yesterday. >> I'm not in.
[43:15] >> Yeah. You're not in your documents folder or your desktop folder. >> Yeah. If you type ls,
[43:23] it'll show you what folders are around. Ramon said something about it being the percent sign.
[43:32] Cool. >> Now I want to see if it's this way.
[43:43] No, okay. >> Yeah, I'm in the problem folder.
[43:52] >> Cool. Now you can type git clone and then paste, so git space clone, sorry,
[44:00] and then paste that URL that you copied. Cool. Then if you type ls,
[44:09] cool, you'll see the results of the best folder, and then you'll see the other files
[44:18] that you made with Ramon when you were learning Express. >> I'm totally just curious what would happen if I pasted it.
[44:28] >> Yeah, it's just the link to there. But now you can open it in VS Code.
[44:34] Now that it's on your local computer. >> That's how we got it to the local.
[44:42] Open. >> Yeah, perfect.
[44:46] >> Then you can click the "Results Best Folder". >> I open the folder,
[44:53] not just the file, right? >> Yes, that's correct.
[44:57] Because now if you see those files, you'll have that H1 that you made,
[45:04] and you'll have the README that you need too. >> When I save this because I cloned it,
[45:15] does that mean it's only saving locally or is it resubmitting to the original?
[45:22] >> It'll only save locally, but we'll use Git to push up your new changes to GitHub.
[45:30] >> Okay. >> If that makes sense. Sorry, this is so much.
[45:34] First thing we're going to do is, let's add your changes.
[45:43] Let's add some new changes. You can add an H2 that says something else random.
[45:49] >> Just for those watching, if you didn't catch that,
[45:58] this is something that I was talking about earlier. When I was writing H2, how did I do it?
[46:05] I did it two seconds ago and then I auto-added my closing H2,
[46:11] and that's something that I really like. >> Me too. You'll love Copilot if you like that.
[46:19] >> Here we go. >> Perfect. Then we'll press "Save".
[46:34] We know that it's not on GitHub yet. It's like those changes are not going to be there.
[46:41] >> I'm just going to go double-check, making sure it clicks in my head.
[46:45] >> Yeah. >> Cool.
[46:47] >> Cool. It only has that. What we can do now though is, we can add it.
[46:54] In our terminal, let's go back there and let's cd into Rosella's the best folder.
[47:01] It feels really weird saying, but yeah. Cool.
[47:06] >> Yay. >> We did it. Now we want to create a new branch.
[47:11] That way, this is a best practice because you can commit this new change to main,
[47:18] but it's easier to make sure you didn't make any mistakes or roll back your mistakes if
[47:25] you create a new branch or new version of your code and then merge it in.
[47:29] The way you're creating your branch is by using this command that says git checkout -b.
[47:35] You can type git and then space, checkout and then space -b and then space.
[47:49] Inside of quotation marks, we're going to name our branch.
[47:54] Regularly, you don't have spaces in branches. I don't know, you can name it whatever you want.
[48:02] >> Something, I don't remember the order he said, but it was when I was working with Anthony,
[48:12] he was telling me, so I'll just do that. >> Cool. Just so you know too,
[48:17] it'll still put the date, but that's interesting.
[48:21] I think that makes sense for today too. Then we can press "Enter" and it created a new branch for us.
[48:31] Somebody told me, can you go to VS Code? I want to see if this is true.
[48:36] >> Cool. In the left-bottom corner of your VS Code, it says the branch name.
[48:43] If you're ever like, "Oh, I don't know what branch I'm on."
[48:46] It's right there. You can create new branches within VS Code too.
[48:50] Maybe I can show you that after. We do the terminal and then we do that because we have.
[48:54] It's like we only did 48 minutes. We'll see how much time we have.
[48:58] But okay, now in the terminal, so you made a new branch.
[49:03] Now we can do git status to see which files we changed. Git space status.
[49:11] Cool. It says we only changed the index.html. I always like to check that because sometimes,
[49:19] you could have accidentally changed another file. I just like checking.
[49:24] Yeah, that's happened to me multiple times where I've left in things that I was using to debug.
[49:29] I'll leave console logs that say, "What's up?" Then I don't want to merge those in to the code base.
[49:38] All right, cool. Then we can do git add, so git space add,
[49:44] and then space, oh, not done yet. >> I got excited, but it's cool that it adds hints.
[49:51] Maybe you wanted to say git add period. Another hint is turn this message off by
[49:58] running git configure advice.addEmptyPathSpec false. >> That's cool.
[50:05] >> I like that it gives hints. >> Yeah, I like that too because I don't remember
[50:09] giving hints when I first learned to code. >> So git add without hitting enter.
[50:14] >> Then we want to put the file name that we're adding, so index.html.
[50:19] If you had multiple files that you changed, you can add each one of them separately or you can do,
[50:25] like it said, git add dot, which adds all the files.
[50:28] But like I said, I try to stay away from that just in case there's any mistakes.
[50:33] Cool. You did that. Now we want to do git commit,
[50:36] and this is where we're saving it in time. You do git commit dash m.
[50:42] Oh, sorry, actually space dash m, my bad. >> Above that, just really quick,
[50:50] it says git commit dash a. What's the difference between dash m and dash a?
[50:56] >> I think that's amending or editing your commit message. I believe. Someone correct me, it could be wrong.
[51:06] But that's like when you're saying, so you make a message or you make
[51:10] a commit and you want to update it or change it. You're like, "Dang, that's not what I meant."
[51:14] You'll use git commit dash a, I think, or not. I'm not sure.
[51:19] But feel free to correct me. >> We can Google it later.
[51:21] >> Yeah. >> We can Google it later. All right, so dash m.
[51:25] >> Yeah. Then you do a space inside of quotation marks is where you'll do that message
[51:32] on saying what you've changed or added. >> Ramon says what you said sounds right.
[51:47] >> Okay, cool. I trust Ramon. >> Cool. Then close it with quotation marks and then enter.
[51:59] Then last but not least, we want to do. No, I'm wrong. Ramon said it sounded right.
[52:07] I say a lot of things that sound right, but they're not. While Ramon helps us out.
[52:16] He said, I mean, don't trust me. No, I trust you.
[52:22] >> Yeah, Ramon, you're right a lot of the times. So is Rizal. I'm trusting you all,
[52:27] but I can fact-check as well. Even though I'm going to be like, hey,
[52:32] I heard this at some point, not sure if it's right, but I heard this.
[52:36] >> Yeah, fact-check me, please. Now you're going to do git push.
[52:43] It may come up with a message, but we'll see. Just copy that line right there.
[52:52] >> I never remember it. I always just type git push and wait for it to tell me this.
[52:58] >> I like that idea. >> Ramon said that -a is for all.
[53:07] So it's another option to doing git add and then that dot. >> Just so this one, we can show this.
[53:17] Tell the command to automatically stage files that have been modified and deleted,
[53:23] but new files you have not told Git about are not reflected. >> Okay, I'm wrong.
[53:31] I think the amend one is like -am or something. All right, cool. We did this part,
[53:36] and let's go to GitHub and see if our changes are in there. Cool. So they're not in the main branch,
[53:49] but if you press that "Dropdown", you'll see that you made a branch called July 12 dot dot dot.
[53:56] You can click it and you can see the changes if you press that "Index.html" file.
[54:05] You'll see both of them, right? But you're going to talk.
[54:10] >> Oh, yeah. I got a question. Okay. So if we do things in VS Code and Terminal,
[54:23] we've been able to do local host to see what it actually looks like. Is there a way to see how it actually shows up?
[54:32] Is there a local host for that? >> Yeah, we can. So let's merge this in,
[54:38] and then I can show you one way that you can see those code changes.
[54:43] >> Okay, cool. >> If you go back to the main branch by switching that thing.
[54:50] Yeah, that's a good question. Just click the "Code" tab.
[54:56] I don't want to be inside of this file anymore. >> There we go.
[55:00] >> Yeah. Let's click "Compare and Pull Requests". So we can make a pull request to merge
[55:04] the changes you made in the July 12 branch to the main branch. So, yeah.
[55:12] >> Exactly. >> It was weird. When I worked there,
[55:22] our marketing team would have to do stuff, and they taught me how to approve pull requests,
[55:27] because the way it was set up is you couldn't just commit, somebody had to approve it.
[55:31] >> Yeah. >> I was just like, "I don't know."
[55:34] Okay. So that's cool. There's a draft, there's a not draft. You can change reviewers,
[55:39] you can assign it to people who got some labels. >> Yeah. All good stuff.
[55:46] I like the draft one because it's like, I put those up sometimes if my work's in progress,
[55:51] and I just want people to know I'm not being lazy, but I'm still working through it.
[55:56] >> Do it, Ramon. >> Review it. Add him as a reviewer.
[56:02] >> Okay. >> Well, maybe you can't.
[56:04] Maybe you'll just go ahead and review it. >> What's your GitHub name, Ramon?
[56:11] Is it OlaSoyMilk, with some underscores? >> I think that was a bad idea from me. My bad.
[56:26] >> I kind of like it. But I'm going to go to a new tab, so I keep this one open.
[56:34] Because I wonder if you have to follow them first. Do you have to follow them to add them?
[56:41] >> Ramon wants to make a PR. He doesn't want to approve it.
[56:46] Got you. Sorry. Yeah, I mean, you could. Let's do it.
[56:52] >> It's here. Oh, wait. That's a different. >> I never did that before.
[56:58] >> Then it's a code. >> There we go.
[57:04] Maybe. There we go. >> If you don't want to make PRs, go ahead. Let's do it.
[57:13] Okay, cool. Now, let's go to your PR. I mean, you don't need an approver
[57:20] because you're the owner of this code base, so you can go ahead and merge it in.
[57:24] >> You have to click into it. You can't just approve it.
[57:30] >> Yeah. Because you need to see, I guess they want you to see that.
[57:34] Make sure you're looking at the code before you approve it, and look at the changes.
[57:40] >> Interesting. >> Yeah.
[57:42] >> Okay. >> If we go to it,
[57:44] you can see if you go to files changed at the top. >> Thanks. I was staring at it for a moment.
[57:54] I'm like, where is that? >> No worries. I didn't really say my bad.
[57:58] But yeah, you can see and it'll say, this green line means you added that line.
[58:03] They want to make sure you look at the stuff before you just go approve things.
[58:08] But if you go to, oh, go ahead. >> Okay. I was just reading it out loud.
[58:12] No new line at end of file. >> Yeah.
[58:19] >> What do these mean? The at at minus one, plus one, two?
[58:26] >> No clue, but I think they just mean you added one line. Now you have two lines, but no clue.
[58:35] I just [inaudible] >> Oh. I don't know.
[58:39] >> Yeah. >> One line is the same.
[58:42] One line is the same. We added a line,
[58:44] so there's total of two lines? >> Yeah, I guess so.
[58:47] >> We'll go with that. >> You have some good questions.
[58:49] That's stuff I just accepted and ignored. Ramon said, I think it's from
[58:55] Git command line stuff telling you what changed. Yeah. Git gobbled. I can't even say that.
[59:03] You can't even approve your own stuff, but we can just merge it.
[59:10] >> I want to approve my own stuff. >> I know.
[59:13] >> That would be fun. I go back to the conversation. >> Yeah.
[59:17] >> Merge and then commence to show where are the checks? >> I think sometimes people have tests that
[59:27] run to make sure that they didn't break anything within the code. If you had any tests that were running,
[59:34] it'll show up here and be like failed or passed. >> Joe, I'm going to add you in the future and you're just going to get
[59:42] sent random things as I'm figuring this out just as a heads up. Merge pull request.
[59:49] >> Yeah. >> I'm just reading it. Merge pull request number 1,
[59:55] and it says who's it's from, and then the file,
[59:58] and my note of added h2 inside index.html. I can leave another comment.
[60:05] >> Yeah. You can be like, good job or not good job.
[60:10] >> Cheer myself on. Yay, done. >> Let's go.
[60:17] >> Then so we can create a merge commit which commits all from this branch, will be added the base branch via a merge commit, squash and merge.
[60:30] That's just really fun to say. The one commit from this branch will be added to the base branch and rebase and merge.
[60:40] The one commit from this base branch will be rebase and added to the base branch. >> Yeah. Lots of confusing.
[60:50] >> I'm not even going to ask about those right now. I'm just going to do the commit.
[60:54] >> Cool. Then press "Merge". Yeah. Okay, cool. I thought you're going to forget that.
[60:58] >> Confirm. Merging. >> You did it.
[61:03] >> Yay. >> Cool. Then you said you wanted to see it live.
[61:08] Then is this where people delete the branch after they merge it? >> That's a good question.
[61:14] Hold on. Let me remind myself where you do that because I will just have you not knowing how. Give me a second.
[61:23] >> Yeah, because it says it can be safely deleted. >> Yeah, do it. Delete branch.
[61:28] I didn't even see that. >> Okay. It says pull requests successfully merged and closed.
[61:33] You're all set that July 12th, 2022 branch can successfully be deleted. Okay. Bye, branch.
[61:40] >> Bye, branch. >> You're not a tree anymore.
[61:43] You just got one main area. No more trees or roots for you.
[61:49] >> I know you wanted to preview. How much time do we have?
[61:54] Like 21 minutes? >> Yeah.
[61:56] >> You wanted to preview the code like you do in localhost. There's a thing called code spaces.
[62:02] I don't think you have access to it, but just for people who are watching,
[62:07] you can use code spaces to code in your browser, and you can look at your code locally there.
[62:12] But another option is- >> I'm just going to Google it.
[62:15] >> Yeah. Go ahead. Yeah. Google that, and then I'll show you a different way.
[62:19] PR is open, and we can approve Ramon soon. >> This is just fun. Okay.
[62:27] But to go back to where you were, you wanted me to go to a different one other than code spaces?
[62:36] >> Yeah. But I don't know. What do you want to do first?
[62:40] Ramon just made a PR. Do you want to approve this PR and merge it,
[62:44] and then we do the other one? >> Yeah. We got one pull request,
[62:50] which I'm not going to lie, it doesn't like earlier,
[62:54] it made that one pull request really well-known, and this one I'm just like,
[62:58] I didn't even see it unless I looked for the one. >> I think because you made it,
[63:04] and it's telling you, "Hey, you committed, open a pull request."
[63:08] But I don't see Ramon's refresh. >> It has the one. That's weird.
[63:17] >> Oh, he said, "Whoops, one sec." >> JK.
[63:22] >> And he said, "One." >> Yeah, it has the one that's closed.
[63:26] >> Okay. Let's go back. >> Yay.
[63:32] >> This is good. He might make us do a comment to make it be approved.
[63:39] >> Okay. No description provided, but that's his comment.
[63:47] >> Yeah. >> Interesting. Okay.
[63:49] >> We can look at the files changed to see his code. >> Cool.
[63:57] >> Oh, yeah. I think it is. One stayed the same,
[64:00] line two stayed the same, maybe so we added a third line.
[64:07] I don't know. I'm just guessing on that now. >> Yeah, it does seem like.
[64:11] Now we can make a comment and tell him to improve something, or we can suggest something.
[64:18] >> Can I fix it from here instead of asking him to fix it? >> You can suggest the change,
[64:26] but he's got to fix it, or he still has to accept the change.
[64:30] So let's do it. >> Wait, I would.
[64:35] >> You can do it where we were in the files changed, and hover over wherever you see
[64:43] the mistake and you've seen those little plus signs if you click them.
[64:47] How do I do a suggestion again? I can't forget. What's that plus or minus sign?
[64:58] I wish I could circle. >> This one?
[65:02] >> Yeah. There it is. Add a suggestion. Click that, and then there you go.
[65:06] You can add that suggestion for him. >> Typo.
[65:13] >> Typo. >> Cool.
[65:17] >> Corrected typo or typo. I think that's what you had it as.
[65:39] >> So meta because you corrected a typo of the word typo. >> Yeah. All right. Start a review.
[65:54] >> Yeah, you can do that. I guess you can do finish your review.
[66:01] If that's all you wanted to change. >> Yeah. That's cool.
[66:07] >> All right. Finish your review. Why would I comment it?
[66:18] Submit general feedback without explicit approval. That would just mean that I'm getting feedback from my teacher,
[66:28] and they're just going to give me feedback, but it doesn't go into the main branch?
[66:33] >> Yeah. Sometimes people just want to make a comment. Maybe they have questions,
[66:38] or they just have a small nitpick or something like that, or they're just sharing you on,
[66:46] but it's not necessarily that they need you to make any changes. It's just like a free-form comment like,
[66:51] "Oh, this is cool," or "Why did you add this?" Something like that.
[66:55] >> Okay, cool. Then approve. We know what that one is, and submit.
[67:00] >> Yeah. >> Okay.
[67:04] >> Cool. Then I guess we wait for Ramon. >> To fix it.
[67:11] >> This was fun. I like that Ramon added in this part. It already came through.
[67:23] >> I'm so confused by this. Okay. It made it.
[67:30] >> Yay. >> It's fixed.
[67:32] What is, I don't understand this. Why it's not moving?
[67:39] >> What part? >> The no new line at end of file,
[67:45] and why it's in between line 2 and line 3. >> I think it's just saying that in that,
[67:56] the old way you had it, when you first added that H2,
[68:00] you didn't press "Enter" and add a new white space. Because sometimes people do that,
[68:06] and it's good to notice those changes. >> I got it. I'm going to approve.
[68:14] Thank you for fixing it. Cool. Merge.
[68:29] >> Let's do this. Ramon said, "I think some coding editors
[68:37] are different about adding that end-line thing." >> Okay. All right.
[68:43] We have approved the merges, and now when we get, how do we?
[68:53] Oh, that's cool. It also says. Okay. Whatever.
[69:00] >> Maybe you have two accounts. >> I probably have two or three accounts.
[69:05] I don't have access to all of them either. But how do I see it live?
[69:15] Let's do it. Can you make your browser bigger? Because I don't know, this view, I forgot.
[69:24] Ramon made a good point that this was essentially us doing open-source.
[69:29] That's how open-source is. People will open a pull request and then you approve it.
[69:34] All right. GitHub has this thing called GitHub Pages, that you can see your code live if it's a front-end,
[69:47] if it only has front-end. If it has back-end, it doesn't support that.
[69:50] But if it's like HTML, CSS, or React, or something like that,
[69:54] or Jekyll, you can see it there. I think if you go to "Settings", I hope I'm right.
[70:02] It's actually not there, not that settings. There's two different settings.
[70:09] >> I'm just kidding. >> Yeah. But I see where you're going.
[70:13] If you go to on the left-hand side, there's the word "Pages".
[70:19] Yeah, we're putting it on GitHub Pages. Right here, it says, "Choose the source."
[70:28] You can choose if you want it on which branch, and we can put the main branch, yeah.
[70:35] If you press "Save". It's going to be published at teachmegen.github.io/roselle is the best.
[70:49] When we go there, we might get a 404 page, but click it and let's see.
[70:53] >> I don't like that it didn't open a new tab. That always frustrates me.
[70:58] I'm like, "Can't you just open a new tab, so I don't have to go back to this?"
[71:01] >> I know, I hate that too. Sometimes I right-click it, and then it'll show.
[71:06] >> Yeah. Okay. Site not found. >> Yeah. We can see it's probably in progress.
[71:15] If we go to scroll up a little bit, there's the word "Actions" at the top.
[71:22] We'll see it being built out. If we click into that action,
[71:29] this is a little bit more advanced. But basically, it's using automation to take
[71:37] your code and deploy it onto this live site. It shows you when it's done.
[71:43] It's done now, and we can go back to that tab and press "Refresh". >> Yeah. Like a different letter.
[71:52] Yay. >> There it is. It's not necessarily local home,
[71:57] but you can use it to preview your code, and you can share that link with other people,
[72:03] and make little websites for free. >> I'm just thinking back on all the other ones.
[72:15] I feel like I'm good. Was there anything else you wanted to teach me? Because I feel like I'm knowledged out at the moment.
[72:25] In the fact that, I didn't mean to make that bigger. There we go. I was like, "Yeah, hello."
[72:33] That is something that I think is a, he mentioned, Ramon mentioned portfolios.
[72:46] How do you figure out what projects to create? So many people have been like, "Hey,
[72:51] to get noticed, you got to go make some projects, and commits to open source."
[72:58] I'm just like, "I don't even know the words you just said." Which I mean, now I do,
[73:02] and thank you Rizal, this is super, super helpful. I'm like, "Okay."
[73:06] So I'm at least seeing how these are all put together. Yet I'm like, "I don't know."
[73:12] Because I don't know much about it yet, that I don't understand what they all do.
[73:16] >> Yeah. >> Where did you start?
[73:20] >> Great questions. I agree, Ramon, it's a hard question.
[73:26] People ask me that a lot, like what projects do you make?
[73:32] I'm not really like a project person much, to be honest. I mostly, some people like to code for fun.
[73:42] They're just sitting there, I think, thinking of cool things that they wish existed,
[73:48] and they're like, "I'm going to spend my weekend doing this." I'm not that kind of person.
[73:51] I'm spending my weekend outside. But when I have projects,
[73:57] it's been like from my bootcamp, they show me how to make something,
[74:02] or they tell me about making something, I upload it to GitHub,
[74:05] or they have a final demo day, and they're like, "What is the final project you want to have?"
[74:09] I sat there and thought of something, I made a natural hair augmented reality thing,
[74:16] so people took a little quiz, they decided on what hair type they had,
[74:22] and then there was a little augmented reality pop-up girl that popped up, and it was like, "This is you."
[74:28] But yeah, you can-- - That seems very advanced.
[74:33] I get excited for just having text on the screen. - I followed multiple tutorials,
[74:39] and just bunched them all together. - Nice, nice.
[74:43] That's like, the next couple of days, I'm going to be doing co-working with Jen,
[74:49] as well, I redo a lot of these projects, of doing them live,
[74:55] and hoping that I can figure it out, but I will say this is starting to make sense, more sense.
[75:03] I'm very excited. - That's good, yay, I'm so happy.
[75:07] And yeah, if you have project ideas, go ahead, or what some people do is they follow a tutorial,
[75:14] and then they build up on it. They'll follow a tutorial on building an Instagram clone,
[75:18] and then they're like, "What if I added in this?" And they'll just Google their way to doing it.
[75:23] But I'm glad that it's starting to make sense. I hope it wasn't too overwhelming,
[75:27] 'cause it's a lot of work. - No. Yeah, I know that you wanted to come back on,
[75:31] and talk about it more too, because also, I do want to say
[75:36] that Yere is coming on again tomorrow night, and Ramon is coming on again on Monday,
[75:43] and AJ said he'd be back, and then we're gonna have Ramon and AJ together.
[75:49] - Oh, that's so fun. - Like merging a front-end and back-end to make a full API.
[75:55] Is that what we were talking about, Ramon? I think so, we'll see.
[76:01] So it is definitely growing, and I'm learning, and for y'all listening and watching,
[76:09] please let me know, yes, it was a full stack app, full stack app.
[76:13] Please let me know what questions you have, what you want to learn,
[76:16] if you want to come on Learn Live with me, that is dope too.
[76:21] We have lots of really cool teachers, or if you think there's somebody I should reach out to
[76:25] to have on the show, 'cause this is a thing that two weeks ago did not exist,
[76:31] or did I know that it would exist? So just get out there.
[76:36] - Yeah. - And Rizal, I know we have your Twitter on tagged.
[76:43] Anywhere else you would suggest people reach out to you at? - Nope, Twitter's good.
[76:49] - I really like Twitter. - Yeah, it's easy.
[76:55] - Now that I'm learning it, but thank you so much, everyone, for joining.
[76:59] See you again tomorrow. - Bye.
[77:02] [BLANK_AUDIO] 
