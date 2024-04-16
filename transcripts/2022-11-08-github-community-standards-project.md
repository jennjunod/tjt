---
showLink: "https://www.youtube.com/watch?v=WPp-hehlu7g"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "github-community-standards-project"
title: "GitHub Community Standards Project"
publishDate: "2022-11-08"
coverImage: "https://i.ytimg.com/vi/WPp-hehlu7g/maxresdefault.jpg"
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

[00:00] Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech. Today, we have Jay and Homi with us. Yay. Jay, because you're on the announcement. So Jay, you get
[00:16] to go first. Please introduce yourself. Yeah, what's up? I'm Jay. Jay Miller, I guess. That's my kettle saying my tea is done. But
[00:26] we're good there. Yeah, I'm a senior cloud advocate at Microsoft in the Python space. And I am here to do JavaScript things, which is, yeah, hold on. It's gonna be a while.
[00:42] He is a Pythoner. Pythonista. Pythonista. I like that. Pythonista. And Homi, you want to introduce yourself? Homi Koder. I'm not sure is my camera working?
[01:01] Yeah, it seems like it is. It is. Yeah, I'm like, Homi is the person behind. He's everybody's Homi. He is the Homi behind the scenes doing everything. Yeah, so just learning new dev.
[01:13] Just got into it. I ran into Jen. Love the stream. Love helping. Love getting involved. Jay's awesome. So we're working on this project that they'll explain. And I'm just I'm glad
[01:22] to be here and help out. Yeah, this is cool. I love the humility because like Homi has done the most work out of all of us so far. Like, if I look at the PR records, he's just
[01:35] like, I'm literally looking at PRs that I was like, Oh, yeah, I was supposed to. I was supposed to go ahead and merge those. So let me do that. All right. Yeah, he is a legend.
[01:49] Homi the legend. He's like, what every Homi should be. Hey, what's up AJC?
[01:58] Hello, Anthony. I agree with you. And yes, we are gonna talk about I feel like you should introduce it, Jay because you this is like your brainchild that we're doing. So you get
[02:20] to introduce it. Yeah, so I mean, I'm gonna try at least. So I created this VS Code extension a while back.
[02:30] Homi's gone. I don't know what happened. I created this VS Code extension that does one thing and does it really well. It adds a code of conduct to a project. And I shouldn't even
[02:40] say it does it well. It just does it. I've found some ways that I can improve it. And I plan to get to those things or maybe have other people contribute those changes. But
[02:51] yeah, and the whole reason behind this was there's this thing that is being talked about more in open source development, which is like community and project health. And one
[03:06] of the best ways to gauge that off the jump is by looking at the GitHub community standards. If that project's on GitHub. If it's not on GitHub, then I mean, I think GitLab might
[03:18] have community standards too. But when we look at this, the idea is pretty simple. There's a few things that you can do. Like does your project have a readme? Does it have a code
[03:31] of conduct? Does it have a contributing document? Does it have a license, a security policy, templates, PR templates, all of those things. What are the things that you can do to make
[03:39] your project, one, more accessible to newcomers, as well as just to give people a sense of okay, this is a project that care has been put into it. And I decided to donate my code
[03:57] of conduct, you know, project. And hopefully we can crib another project that exists already called, you know, add a license. And then from there, use this as a way to give people
[04:10] a quick gauge when they open VS Code, which is, you know, disclosures. I work for Microsoft. We make VS Code. That's a whole thing. But when you open up a new project in VS Code
[04:21] or when you clone a project, the first thing you should see is the health score. And that says, like, all right, here are some simple things that you can do to get this health
[04:29] score up and really start to work on building out this ecosystem that promotes better community standards across the platform and do it in a way that's easy. And I'm sure Homi can talk
[04:45] to how difficult just adding the basics can be at times. You should do that now. It's a list, especially if you weren't aware of them. There's a lot of stuff, but it's
[04:58] all good stuff to add and it should be in every repo. And it's kind of, you know, creating that standard to make sure that everybody's kind of operating on the same field. It gives
[05:06] you all the tools that you need to make sure that you have contributors. They're contributing according to what you set up previously, how you want your repo to flow. Keeps everybody
[05:17] accountable and, you know, there's those that step outside of the rules. But with these things already in place and these policies, you can deal with that swift and move on with
[05:24] your progress because everything's already spelled out. Every repo should have it. You know, and it's a good practice to get in. And what Jay was kind of spearing up and heading
[05:34] up was that everybody should have it, but it's a little bit difficult to do. And it takes a little work and research and process. So we're trying to shorten that down so that,
[05:45] you know, every repo, even the smaller repos can have, you know, the full community standards met.
[05:51] >> Yeah. >> Ditto everything they said. I'm hanging out to learn how to do it. And also just the
[06:02] really cool practice of this is being able to learn how to work together on a project as more of a newbie in the dev side of things. And also being able to see how as from a newbie
[06:17] point of view, I'm like, I don't know how to go about this. Or what to do. Because I'm like, yes, there's like what the project is. And I know how to go find all of this. And
[06:30] like what they're saying makes sense. And going over here to community standards. But even like security policy, adding it over here and going, okay, this is security policy.
[06:44] Got it. Okay. I can do research here. But then that's going to take up so much time and could get me like derailed from what I'm already working on. Or, for example, a pull
[06:56] request template. It doesn't link anywhere. So, you know, trying to go what's a pull request template? I don't know. I'll go Google. So it's like I love being a part of this crew
[07:11] to be able to do all of this. And a big part of where we were at, which by the way, you can join us and contribute. I will paste this here shortly as soon as my computer wants
[07:33] to load. >> Yeah. While you're working on that, that was going to be one of the things that I wanted to throw out there. And no, Homie's extension
[07:42] is actually probably more visible than mine. Mine just does one thing and then you never touch it again until the next project. Homie's got stuff out there that streamers can use
[07:53] and, you know, quickly promote what theme and stuff he's using, which is great. Which I will shout that out, you know, for him. But we definitely want like this is designed
[08:04] to be a project that the people that it benefits the most get to work on. I had a good conversation with a friend that was talking about like it's funny how like people who have to deal
[08:17] with the most stuff tend to make things that reduce the amount of stuff that they have to deal with. And it's like if you're a beginner, like we're trying to make it so that you can
[08:26] easily identify the projects, which also shout out to Open Sauce because I've been talking to them in the back channel and they're heavily interested in what we're doing because they
[08:35] want to see like, again, it's their whole job is making open source contributions easier for people. And we're doing the same thing. We're making it so that like, oh, hey, anybody
[08:45] can just jump in and like know that one, they're not going to get harassed to if they need help even filing an issue or submitting a PR. All that stuff is there to help them out.
[08:57] And then at the end of the day, like you can focus, like Jen said, on just doing the thing like making the changes that you want to make.
[09:04] When I thought about it, Jay, when you spread this out, I was thinking about it the last couple of days and it's weird, right? There's this shift in the tech, in tech and web dev
[09:23] and web development for a lot of the companies are now making big, big company, big products tangible for smaller, you know, smaller organizations. For example, like, you know, using Next.js,
[09:38] big huge companies can use that and they're bringing that down. Like a lot of the software is coming to where, you know, a newer person can use it. And I think that's kind of where
[09:46] you're hitting with this. If I'm making sense that every project could have this without a team to do it or without somebody that's specializing in community standards, everybody's,
[09:56] everyone has access to this in their project, you know? Yeah. That said, we have some, we have some things that we're going to try to knock out
[10:03] today. And I think Jen's supposed to be driving and we're kind of here to pair. I don't know. I just wanted to, well, I'll ask the two of you, which you can say no.
[10:13] Do you mind if I share a bit about our chat? Because I want to show people where I was really getting stuck and how Jay explained it and then how I'm still stuck. And I think
[10:25] a lot of it, this is a big reason I can struggle with getting these projects done. This is something that I've been dealing with on a regular. So it's not just something that is
[10:40] like code specific. This is me dealing with my own neuro diversities when things don't click. And this is a big reason I want to share this part as well.
[10:48] So cool. I get that. I want to go to issues and I want to like, you know, add and I was looking at this one, which was at a templates folder. And I, I asked the team about it and
[11:02] I was like, yo guys, like, what is the next step? Like, how do I go look at this? And we were talking about doing, uh, what is it called again? Now I have to look when it's
[11:15] called. Working with Octokit.
[11:17] Yeah. Octokit. And so I was like, okay, cool. Um, what do I do? Because it was making sense. And as I said, I will share this one part with us. Um, is I was like, do I build an
[11:32] app and then put in Octokit with it? And so Jay was very kind and was like, Hey, here are the steps. And even reading the steps, I'm going, but wait, my head is saying like
[11:48] your steps make sense. They do. I just don't know how to do it. And this is really where I struggled.
[11:57] So, and that's, that's kind of, I mean, that's just the nature of it. Um, in, in some cases, because we're still in that planning stage, like the only code that we have is code that
[12:08] already existed. Um, but one of the things that I wanted to do was, is, you know, come together and figure out, I think I even put it in a comment like right up, like before
[12:19] that of like, Hey, we're not even sure how we're going to go about some of these things. So what we, what we kind of need to work on first and foremost is like, one, let's just
[12:31] figure out how we want to present this information. And one of those, one of those things was like, you know, add code of conduct. The way that that works is it is completely divorced
[12:44] from GitHub's API, which is, you know, there's, they have a JavaScript, you know, wrapper called Octokit. Um, this doesn't use that at all. And that's, that was intentional.
[12:55] That was so that I could ensure that anyone could add the license of their choosing. And even then there's like thoughts that I'm having, like, we may not even want to go down that
[13:06] road, or I may want to pivot from that road of saying, just like the components, um, Homie has been doing a lot of work in terms of like adding like security dot MD files and stuff
[13:17] like that. And one of the biggest challenges there has been like, what do we need for those specific like files? Because if you just copy what GitHub has, they worry about bug bounties
[13:36] and like all this other stuff. And most developers are not going to need to worry about that starting out. So like, how do we how do we like balance that? And right now what I think
[13:49] what I was trying to get across was, can we first start with, let's identify what exists and what's missing. And that was where kind of those comments came in of like, for that
[14:02] Octokit, there's already that works already done, we just need to access it. So what I was hoping we could do is just get into a scratch project. That is like, nothing of
[14:16] importance is like, we're just going to build some stuff and then make it you know, if we get it working, then we can take what we've learned and then apply that to our extensions.
[14:28] And again, that totally does make sense. And thank you again for the explanation. When people are saying let's start a scratch project, I think that's where I might be getting lost
[14:38] of like, throwaway project project that at the end of the day means absolutely nothing. And we're
[14:45] only using it to learn how to do the things that we're going to do. And then later on, we'll worry about getting that incorporated into the extensions. So this is just a blank
[14:54] folder where we're all starting from zero, but we're doing it together. Okay, so I think that sounds weird. But so blank folder within our repo, or
[15:09] Not even in GitHub, on your screen. If we all if we want to do the same thing along with you, we can do it with you. But at the end of the day, no one this this does not
[15:18] exist. This project does not exist.com. Okay. And I think that's a big part where I was getting lost because I was like, uh,
[15:28] I skip steps. And it's so frustrating that I'm like, but it doesn't make sense. All right. So if I'm making a scratch project, I'm basically going to VS code and starting a new, new project
[15:43] and starting from there, right? Right. Yeah, let's just jump into a window and we'll we'll walk through it.
[15:52] Let's go to VS code. Maybe. I don't know where it is. I always get the icon. I always lose the icon. I don't know how but I do.
[16:09] It happens. Nope, I want to do in file.
[16:18] You will want to create a folder. But that's Yeah, I mean, you can just do like new file and then create a new folder in that file or whatever.
[16:26] Like I'm not used to doing it from this. Just call it like octokitlearn or something like that out.
[16:36] That's not how you spell it, y'all. But that's how we're gonna do it today. It doesn't exist. So it's perfectly fine.
[16:48] And I do find this oddly awkward, because so many people are gonna be like, yeah, Jen, this totally makes sense. And I'm like, no, it's not making sense on doing even these
[17:01] like, very, very basic things. And I want to call out that a I don't know if it's just a me thing or an ADHD thing because
[17:12] executive dysfunction also talks about organization and organization is at least for myself, it'll show up where somebody is giving me the steps or there are steps and it's just not making
[17:24] sense. So I'm really excited that we're doing this together, because you are one of the most patient teachers I've ever met. All right, I'm creating a new folder file and
[17:37] don't even need to do that. Oh, sweet. Okay.
[17:40] Let's open up the terminal in there. And then we're gonna so the first thing that you do with it, you know, most JavaScript
[17:51] projects that you're gonna you're gonna want to work with is install what you need. You could do NPM init, but we're not even going to do that. We're just going to NPM install
[18:03] our like, is it Octokit? Is that is that what it is, Octokit.js? Again, I don't do I don't do JavaScript like that. So I want to say
[18:21] Not that I can spell but It's O-C-T-O-kit.
[18:34] I will put this in the chat as well. Yes, I could go through this, but I can probably just do install and Google it.
[18:53] Yeah, I get it. Why do I feel like I'm just like, not seeing this stuff?
[19:17] So, we know that Octokit exists now. So we can just do NPM install Octokit. And that's just how, how did you see that that was Octokit or is it just like putting
[19:33] two and two together that oh, it's probably NPM Octokit install Octokit or So NPM install is always going to be the way I mean, unless you're using something like
[19:42] Yarn, which yeah, there's another one. I tend to just default to NPM because that's what I was taught. I know some things are Yarn. I think when we go to I think it's OCO. If
[19:56] that does if that installs something, yeah, I was OCTO kit. But I know when we go to the actual VS, like the actual VS code and stick extension, it's
[20:14] going to be Yarn. I mean, if we want to do Yarn install Octokit, like we can I don't I don't think it matters. Like again, this is a throwaway project. So at the end of the
[20:24] day, like okay, cool. Package was installed. Can you just type in node? I think that's what you do. Yep. So now let's do how do I use this?
[20:45] I can do the share the live share. I don't know if it's going to give you a link. You probably shouldn't share that publicly. Okay, well, I mean, that's a good call. We'll just
[21:02] do this then nobody can see it. Yay. There you go. Let me authorize some stuff really. I love how it like makes you log in to just be able to do that. I'm like, I've used it
[21:13] with the, you know, GitHub before, but nope, we got to reauthorize everything, which is fine. Why is it asking for app? That's interesting. Oh, because I think it's all TypeScript stuff,
[21:40] which is, that'll be fun. And the reason I didn't want to just like look at what some other projects are doing, because I mean, there are other people that are using OctoKit.
[21:53] Problem that I have with that is my TypeScript is very limited. And what I've learned is that a lot of the stuff that people do always like throws me off. So I'm just like, I don't
[22:08] know what we're doing here. And then like, at the end of the day, I'm like, this was a way so it's good to just learn it together. I dig that. And I just sent you the link.
[22:22] So and then also, the other reason why we are doing this is because we're going to have Josh on on every other Friday doing TypeScript. So this is the project that I can actually
[22:38] work on while I'm learning TypeScript, too. Awesome. Um, I did not get a link if you sent it. You sent it in private chat. That's probably why. I like to make it difficult. What up,
[22:56] Brian? Now I'm trying to figure out how I can do the live share. Oh, join. There we go. There we go. I think I'm there. All right. So I'm gonna I'm gonna throw a small curve
[23:16] ball here. I can't see. Can I see your terminal window? Maybe? I don't know. Let's see. Are you typing in that window? Can you do like LS really quick? Oh, wait, what? LS is not
[23:53] defined. Oh, because you're still in node. That's that's fine. That's fine. Okay. No, that's perfect. I can I can see what you're typing. All right. Um, I'm not gonna see if
[24:06] I pick my nose or something. I'm sorry. I'm not staring at the camera. Such is life. That's kind of what like I've realized. I'm just like, you know what? I may do awkward
[24:15] stuff streaming. If people see it, they see it. That's what it is. So what we what we're trying to get to is the rest GitHub's rest API for community standards,
[24:32] which I think I shared in Discord once upon a time. And it was it's it's not an easy reach. They made it relatively complicated. Where is that? Oh, here it is. I'm gonna send it
[24:56] I'm gonna just throw it in the chat and I'm probably gonna get flagged because it's gonna be like stop spamming because it literally looks like spam. Oh, yeah. Oh, I can't I can't
[25:07] respond in the chat. Okay. Well, I'm gonna just respond in the private chat then. Oh, you should be able to. No, he needs to be on Twitch.
[25:17] Yeah. Oh, yeah. He doesn't like let everybody else reply to that, which is fine.
[25:24] Can we throw that up? Yeah, it's I mean, I just need the Git repos owner repo community profile like that part of it. But basically, if if we go into a web
[25:36] browser, or if you want to even just do it in in the terminal, you'd need to get out of out of this. Well, you're gonna need to exit first. You could also do that. Yeah.
[25:53] No, just just type in exit. X, Ctrl C, Ctrl C. Yeah, Ctrl C. Ctrl C again. There we go. Not exit. See this tells you exactly how much JavaScript I do is I can't even quit JavaScript.
[26:12] I can quit Vim. I can't quit JavaScript. Like I've never had it. Okay. Yes. Okay. Well, that's definitely not gonna work. I'm like, I didn't think so. But I'm like, that's not
[26:27] at all the cool things today. So but you can curl it you can do curl. Yeah, type in curl. And then just the do was a HTTPS colon backslash backslash. Yeah, the whole thing api.github.com.
[26:55] And then just that last part there, the repos owner repo community profile, and we're gonna we're gonna change a couple of things here. So we're gonna keep Oh, yeah, sorry.
[27:08] Thanks, Anthony. Anthony, Anthony pushed up his glasses and said, Well, actually, on me. I don't know.
[27:16] I don't know what I don't know what slashes they are. They are the slashes. The slashes we need. Exactly. So you got the right ones. Instead of owner, what we want
[27:26] to do is let's do let's do ours. So that is was it GitHub community standards? I think that's all dashes. Yeah, those are all dashes. So and then we're gonna do let's just do our
[27:46] actual project, which is also GitHub community standards dashes. And let's just hit enter there and see what we get. Yeah, so we're gonna get a bunch of information here. If
[28:00] you scroll up, you're gonna get like, all this information that's available to us. This is not what we're going to use. This is just the opening to what we're going to use. So
[28:11] now let's just hit up on that. We got to scroll back. Yes, go back down to work. All right. Now it's got another forward slash for the people in the room. And then we'll do community
[28:27] dash profile, and then hit enter. I'm sorry, I said dash sorry, it's community forward slash profile. And then let's say enter there. And what we should get is some different information.
[28:44] We scroll up here. And this is this is what we're looking for. So that health percentage score that is that is what our community health is. And then we can go in and see like what
[28:57] we're missing. So we have a code of conduct. Code of conduct is the contributor covenant, which is kind of funny, because sure, I mean, it is. But it's also not. Because, you know,
[29:09] we customized it. But sure, whatever. Code of conduct file. We have a path to that file. Scroll down. All right. And here's the fun stuff. So we have a license. We don't have
[29:24] a contributing document. We don't have an issue template. We don't have a pull request template. That's what all those nulls are. So what we want to be able to do is we want
[29:31] to be able to build a JavaScript thing that basically takes us here and tells us what we want to know. And then we'll work we'll back work our way into putting this into a
[29:46] VS Code extension. >> Makes sense. >> Yeah. >> I'm following. I'm following.
[29:54] >> So this is where we create a new file. And I'm pretty sure this is all TypeScript. So we well, I think we can just do JavaScript, right? Let's just do JavaScript. We'll see
[30:06] what happens. We'll be adventurous. We might break stuff. >> Are we just going to do an index to start? >> Whatever. You know, just call it whatever.
[30:18] Index.js. That's fine. It could be app.js, main.js, anything.js. >> Anything.js. All of the things. >> All the JS. The first thing we'll need
[30:28] to do is we'll need to import Octokit. Now, this is the challenge. We've got to figure out where in Octokit we need to import. We don't need to import all of Octokit. We need
[30:40] to just import, like, the part that we want. Which is hmm. >> So I have Octokit open over here. >> Octokit.rest endpoint. I mean, I guess
[30:59] we could just import all of Octokit. That wouldn't be a problem. Wasn't necessarily what I was thinking. So that would be -- what is it? Import Octokit from -- and Octokit
[31:20] is the actual class as well. So it's going to be -- let me see where you're at. Where's your screen here? Yeah, it's going to be, like, import Octokit -- oh, can I type?
[31:31] >> Yeah, you can type. >> Is that showing up? Look at that. So import Octokit from Octokit. And then let's just do console log Octokit rest -- oh, yeah. Well,
[31:53] we have to do -- do we have to instantiate a new -- yep. So then you've got to create a new Octokit -- is that an app or -- hmm. Let's see where you're at. You're in there.
[32:11] >> I'm going to go past that. >> Go to usage. Load Octokit. We're going to skip the CDN stuff because we already did that. Octokit API client. Standalone minimal
[32:25] is Octokit core. Requests and queries. Okay. So, yeah. Just new Octokit. And I don't think we need to pass any authentication. So Octokit. Just do that. And then let's just console
[32:54] log that and see what happens. >> And then just to make sure I remember correctly on -- I just can't see it because it's not all the way there. Okay. Cool. And
[33:11] then we will just do run on this. Now I don't remember. Why am I not remembering this? >> We'll let you run it. >> Dev run. I don't remember.
[33:25] >> That's for React and stuff. I think if you just do -- can you just do node stuff? Like node and then the name of the file? >> Oh, yeah. Yes.
[33:35] >> I could be wrong. I don't JS like that. >> I did that in Tweety tag. So, yes. Yes. Can I use import statement outside of a module? What? I have no idea what that means. Is it
[34:00] just yelling that I -- >> Oh. You're joining and leaving us. >> So my guess is that it's yelling about something in here. Do we need NPM or something
[34:37] like this just to make sure that everything is -- I'm going to just Google it. Because why not? Yeah. In the nearest package.json. >> Oh, do we have to have a package.json?
[34:55] >> I'm pretty sure. Yeah. >> Oh, no. Didn't you want to do NPM init? >> Oh, yeah. To get it. Okay. Yeah. I see. So, yes and no. Yes and no.
[35:15] >> Yes. >> Yes, we need a package.json, but no, we need to do it with the -- okay. NPM init. >> The classic British developer joke. Favorite
[35:32] packaging manager for all Brits. NPM init. Just enter, enter, enter. It's fine. Again, we're throwing this away. It doesn't need to be anything great. Perfect. All right.
[35:50] Now let's try it. >> And let's save. I click save now. So -- >> You don't have autosave? >> I haven't gone through and set all of this
[36:01] up. Maybe that's what I should do during your stream next week. Like the official stream next week. >> Yeah. Oh, no, no. Hit command -- or control
[36:10] C, command C. >> I did -- >> Up one more. There we go. >> There we go.
[36:17] >> Okay. See? We did that, though. But we did the NPM init. First install, save. Dev. Is it because we're not doing, like, NPM start or something?
[36:42] >> Oh, do we need to throw a script in there? >> Package type module. Do you just need to add package type module to it in the package.json? Boom. Try it now.
[36:58] >> Oh, hey, look. Checked it. >> It works. >> Sweet. All right. So probably shouldn't have done a, like -- let's just load everything
[37:20] up. Probably didn't like that very much. So now I'm gonna stop typing. I'm gonna take my hands off the keyboard. I'm gonna let Jan or homie type. In index.js, let's go check
[37:33] that out. So the way that Octokit works is you can actually access the API the same way that you would the URL, except for instead of the slashes, they're, like, endpoints.
[37:51] So what we need to do is we need to figure out what is the REST API call for where we're trying to go. And if we look at the repo, there's a couple of ways that they do it.
[38:10] There's, like, you can just do, like, an actual request and just say, like, give me this information. Which I don't really think that that's fun. I think there's probably a better way to do
[38:24] it. Which is -- where are you? Source. Index. That's confusing. I'm gonna just get away from that. Let's see what the choose a license did. API index Octokit/REST. And then they
[38:45] just do new Octokit, get configuration, license, get string token. Then they do some weird promise stuff. That's not it. Oh, so they do Octokit.rest.licenses.kit. So my guess
[39:03] is we can probably do something like Octokit.rest.orgs? >> I feel like we could do an entire book. And thank you for joining. Yes. Jay, what were we gonna talk about next week? Because
[39:28] next week was planned. This week wasn't. >> That could -- next week, I think we're just doing some VS code. Like, hey, let's make our VS code stuff more fun.
[39:41] >> Yay! Yeah, because I haven't done -- my VS code is still out of the box. And I am excited because I feel like I need to use the new theme manager and look at this stuff
[39:56] next week. >> Oh, did you find the -- can you scroll up a little bit? Interesting. Okay. Endpoint methods. That's what we're trying to do. We're
[40:12] trying to find the endpoint method. Scroll up a little bit. Sorry, scroll down a little bit. So, yeah, now we got to figure out what the actual thing is called, which is going
[40:26] to be fun. Oh, see endpoint method, rest endpoint methods for full details. Can you just click on that link? I'm sure that's a link. I hope that's a link. If it's not a link, then they
[40:34] failed us. Where it says Octokit plugin rest endpoint methods and it's in blue. >> Oh, thank you. I'm like, oh, I hate this. No. I want you to go into a new tab. Sorry.
[40:46] I -- >> You're okay? >> Yell at a lot of them. I'm like, why can't it just -- there we go.
[40:53] And the nice thing about this is that the way that they do this is they use like -- it's like an open AI thing. So, like, they create an endpoint for every single endpoint that
[41:04] exists. And it's all, like, built in. Okay. Cool. So, it just shows us how we can use this. I don't think we need to actually mess with any of this stuff. We just need to figure
[41:19] out what we're looking for in here. But you may want to bookmark this page. Because if they're talking about how to use stuff in TypeScript, we're probably going to need -- we'll
[41:30] need this again in the future. >> You'll get your own folder. GitHub community standards. BCS. Yay. Which we will call this -- I don't know. We'll just leave it what
[41:48] it's called. >> That works. >> And I should probably do it for this one, too. Just to make sure I got it. Okay. Cool.
[41:57] Yay. Wah. This one. >> All right. In order to get types beyond parameters and responses, open AI types, direct translation of the official open AI spec.
[42:08] Go up. Okay. So, let's check out that link there. All endpoint methods are documented in the docs folder. Let's go to the docs folder. See what we got in there. All right. Scroll
[42:33] down. I love how there's codes of conduct there. But that's not what we're looking for. We are looking probably for -- hmm. Repos? It would be my guess.
[42:57] >> All right. I'm just making sure I go to the -- >> Yeah. So, out of all of those, repos is probably closest. Hmm. Okay. Or wait. What was the URL? You keep looking. Community profile.
[43:22] There wasn't a community one in there, was there? >> This is why I don't like when they don't open a new tab. Okay. So, is there a community
[43:32] one in here? >> Let's just do command find and type community. Or command F community. >> I'm hitting control F and it's not control
[43:44] F in case anybody wanted to know on a Mac. It's command F. It's not what I'm typing. >> Community profile metrics. Boom. All right. Yeah. Let's just click on that and see what
[43:56] it tells us. Definitely want to bookmark this one. Okay. That's perfect. This is exactly what we need. This example here. Just copy that. Paste that in and go over here. Why
[44:23] are you saying one's unsaved? I just clicked save. Maybe I didn't. >> Let's get rid of that console log. We don't want that printing again. That's not necessary.
[44:35] Okay. But we do want to console log this output. So, let's do like a const of that API call. So we just call it a request or something or API. It doesn't matter. Again, we're not
[44:58] plugging this into anything. Love it. >> And then what I call it, do that. >> Yep. >> Okay. And then console.log.
[45:10] >> I'm just going to clean this up a little bit for you. >> There you go. >> Oh, yeah, yeah, yeah. Good call. And then
[45:21] console.log API request. >> Awesome. Now, we've got to do something. Don't run it yet. Let's go over to, again, we're just cleaning this up a bit. We're not
[45:36] doing anything of too much value here. We're just making it so that we can actually look at it and see what's going on. All right. Cool. I'm a Python person. So, I indent everything.
[45:49] And if you don't like it, sorry. So, if we're looking at this, we need to define who the owner is and who the repo is. Now, we could just do it directly in there. And I would
[46:04] probably say it would be easier to just type them in here. But we want to make sure that we actually know what we're looking at in the future. So, let's just create two new
[46:12] variables. And we can const those. Those can be constants. So, we just do const owner and const repo. And owner is going to be well, they're both going to be the same thing.
[46:24] >> Can I do them before this? Or do I have to do them after? >> You have to do it before. >> Okay. That's what I thought. But I'm like,
[46:31] okay. So, const owner. Oh, no. It's okay. So, owner. I'll finish them. I just want to make sure. >> Well, they're the same thing in our case,
[46:46] which is kind of nice. >> Well, if we did it, yeah. Because and then we >> It's going to be in quotes, by the way. I
[47:04] think it's GitHub community standards. Here we go. >> Yay. >> And now this should run. So, if we save,
[47:25] we run. Ah! So, this is good to know. It's a promise. So, it's an asynchronous request. And the way that that works is we need to await it. So, let's put all of this in a function.
[47:53] At the top. Let's go well, let's go up to everything below const octakit. We're going to do what is it? Is it async function? I think it's like async function. And then you're
[48:20] going to need to do the empty yep, you got it. And then the brackets around those objects. This is fine. This is fine. I won't yell at your nope, nope, nope, nope. We're just going
[48:38] to hard code them in. There's no reason to make this more complicated. >> So, no curly brackets? Because I thought we would have a curly bracket here.
[48:46] >> You do, but you want to have it >> Your name. You got to put your name, async function, then name. >> Oh, okay.
[48:53] >> Parentheses, then open your brackets. >> Yeah. Like that. And I'll let you name it. Because this is your project. You're going to want to get rid of those. The greater than
[49:12] less thans too. And then, yeah, just drag everything or just drag that bracket down. Which if you use >> I started I didn't mean sorry. Yes, if
[49:30] I use >> I'm trying to remember what it is now. I want to say >> Go down and highlight them.
[49:37] >> Not even highlight them. Just do option on that line. Just do option down. >> Drag that curly bracket. Yeah. >> Yeah. Just option down. All the way down.
[49:47] >> All the way down. >> Yeah. Option and arrow. There you go. >> Now we got to do one last we got to do two more things. We need to await that request.
[50:00] So the API request, it needs to be awaited. So we're going to do await. What is it? Const API. I don't think it can be a constant if it's awaited. Maybe it can't. I don't know.
[50:13] We'll see. >> Yeah, I think you do const API request equals await. >> Yeah.
[50:18] >> Await, right? That's okay. Yeah. >> So up there. You're going to do oh, where am I where I'm at? >> 11. I think you're on 11 or 12 down there.
[50:29] >> Yeah, right there. The purple line. >> Oh, okay. And do -- wait, what? >> You're going to type in await. And then, yeah, like that. And are you familiar with
[50:47] async await? Nope, nope, nope. Just await. This is the right format. So JavaScript does this thing where it can operate asynchronously. And in order to do that, that means it's going
[51:01] to get a bunch of information and keep going unless we tell it not to. And that is -- that's what this request is. It's like, oh, hey, I'm giving you a promise that I'm working
[51:14] on it. Okay. Well, we want to wait for you to be done with that so we can get the information from it directly. So what we do is we wrap that in an await clause
[51:23] that says, you know, await. So await do this thing. We're going to -- and then at the end of the parentheses -- is that a parentheses? Is that what they're called? Yeah, parentheses
[51:36] on line 15. After that, we're going to do a .then. And that says, like, once you're done with that, then let's do some other stuff. And what we want to do is we want to just
[51:58] console log it. So we can do -- >> And then we got it. >> Yeah. So instead of doing console log API
[52:04] request, what we're going to do is we're going to do console log -- do you know, Homie, what that calls for? Is it something like -- it's not that; right? Or is it -- what is it? Function.
[52:23] >> So you'd want to log the -- I got to say a little higher on the screen there. That constant that you made. Right? >> Yeah. So that should work; right?
[52:37] >> Yeah. >> Okay. I'm going to just walk through what I just typed. Because I barely know what it is. This is a cheap way of writing a JavaScript
[52:50] function. Like, you could write it, but it only works in, like, certain scenarios. Like, where you have, like, one thing. We're saying, hey, with this being X, return console log
[53:00] of X. The other way to do this would be, like, something like function X console log X. Something like that. Or return console log X. Something like that. In most cases, when you're dealing
[53:24] with just one thing being, like, returned, you can just do that. And then we're not doing that anymore. Does that make sense? Kind of? You can say no. Because it barely makes sense
[53:36] to me. >> Like, it kind of makes sense. Like, it makes enough sense on the logic. I think if I were to try to go make this myself, I would
[53:43] be a little stuck and it wouldn't make sense. But in context, it makes sense. >> And that's why we're doing it this way. Because then we can add doc strings or documentation
[53:53] to all of this or comments to all of this and walk through what we're doing. So that if you want to develop on this because at some point we're going to have to put this
[54:02] into our program. And some things are going to change. So, you know, in our function, we're not passing anything. We are going to have to pass something because we're going
[54:13] to have to get that information from the VS Code client itself. But, yeah, if we run this now, it does nothing. Oh, because we didn't call it. So, at the bottom, let's just do
[54:31] API request. And you need to I think you need to put open and closing parentheses at the end. Which says, hey, run that. And what we should now get is some information. API
[54:57] request is not defined. Oh, we didn't close our function, did we? I thought we did. Did we not? Yeah, it's closed right there. Oh, no. No, no, you have to we'd have to return
[55:15] that API request. No, return it out of the function. Or no, no, no, no, that's just a console log. No, it's that's not the function. API request isn't the function. The function
[55:24] is more up the GCS. Is that what you call it? GCS is the function. Yeah. GCS is the function. Yeah. Foiled by our own naming. Yeah. I was going to say something. Naming
[55:37] is hard. There we go. Yay. All right. So, this gives us this gives us the information that we want. Also, it tells us how many we've used and how many we have left. Let's scroll
[55:50] down there. Scroll down a little bit. So, this will be important. Up a little bit. This is great. Up a little bit more. Okay. So, you see that X rate limit. Limit 60 remaining.
[56:07] That is because we're not authenticated. We can authenticate and this will change this. And what I've noticed they do in choose a license is they authenticate using the user's
[56:19] API key. I don't know how that works. So, I'm probably just going to copy and paste what they did and be like, cool. Also, their project is MIT licensed. We have full permission
[56:32] to do that. Technically, if we wanted to just make our own version and put it in and keep it synced, we could. But why? Let's just give them all the props because they did the work.
[56:42] So, we got time. We don't like we've got 48 more requests that we can use. It's not the end of the world. But if we start seeing that go down a little bit, what we may need to
[56:54] do is throw in an API key and we'll have to figure that out when we get there. So, this is this is the information that we need to pull. But what I would like to see us be able
[57:12] to do here is a couple of things. And that's create a function that is like, hey, we've got we've got content. Like, here's where we are. So, if we just say, like, what the
[57:25] health score is. Like, your health score is 62. And then we have here are the files that you're missing. So, out of that files path, here's everything that's null.
[57:41] >> Yeah, because that's all our stuff right there that we need. >> Yeah, exactly. Exactly. And then that's where I'm going to be like, homie, do the
[57:54] thing where you make a notification pop up that says, like, your health score is this. These are the files that you're missing. And then we'll pop up, give them the option to
[58:04] do an, yeah. Yeah, yeah, yeah, yeah, yeah. >> And then we just need to focus on and then at that point, like, the base level extension
[58:13] is done. And then we have those other extensions that we're talking about developing after the fact that are like, oh, hey, add a contributing document. And then we go through the process
[58:22] of building that contributing document, which, again, I think that there's that's easier said than done. Like, what we're hoping to do is basically build off of the backs of
[58:33] giants and say, we can't build your contributing document for you. But what we can do is look at videos and blog posts and things and tell, like, what a good contributing document will
[58:45] need. And then create prompts that allow them to kind of assemble or what I would say put all the things together, everything in one place. All of the different pieces and then
[58:59] create a file based off of those individual pieces. But we got a long way for that. So, let's start first with the contribute, like, detecting null in those files.
[59:14] Mise en place is one of my favorites. I actually have a project that I dubbed Mise en place, which is, like, it's a text user interface that just gives me, like, the latest things
[59:26] happening in, like, Python's Reddit as well as, like, stuff that I've bookmarked. I want to check that out.
[59:35] I mean, it's garbage. I would not. I would not. Not for public consumption?
[59:42] No, it's really not. I don't even know if it's on GitHub. It might not be on GitHub. So, yeah, I would definitely look at creating an issue. I don't know what the issue would be. You
[59:53] can do a blank issue. You don't have to do a blank report. Or you can just clear all that out. That's kind of fine, too. Because we don't really -- unless you have a bug. I don't think we have a bug.
[60:03] >> We don't have a bug yet. >> Yeah.
[60:05] >> I was just going to say, so, next steps is we would need to figure out what null -- like, how to --
[60:13] >> How to grab null from -- yeah. Or how to grab -- how to discover which files are missing. Or which components are missing.
[60:26] I guess that would be the right word. >> Also, maybe I was thinking, too, it showed in there an object. You know, in the fields that
[60:35] had objects. But how do we -- maybe we should look at how do we verify that that object satisfies the community standards? See that piece of data. That object, they have that check mark. You know,
[60:48] they have that green check mark. >> So, I would say I don't -- I mean, we can. The challenge with that is I don't even think
[60:56] GitHub does any of that. It's just, like, do you have this file? If so, cool. >> Okay.
[61:03] >> There might be some logic for things like licenses and things like that. But, I mean, how does it know what my GitHub issue template is? Like, hey, I have an issue template. Yeah,
[61:18] it's garbage. But it's an issue template. Like, it's not gonna -- that's not gonna change anything. >> Mm-hmm.
[61:24] >> So, I would just say, like, if we just find null, like, null is probably good enough in this case.
[61:31] >> Okay. >> I don't know if I'm -- but request. There we go.
[61:47] [ Video playing ] But how would we say that, then? Need to define null components?
[62:08] >> Yeah. Well, just need to -- need to identify which components are null. >> Mm-hmm.
[62:15] >> And if it has that object array showing, then we'll just return. We'll just leave that alone. Yeah.
[62:30] >> Yeah. I don't even -- I don't even think we think about that too much. We're just, like -- >> Yeah. So, I used to say, we just search for just the null.
[62:41] >> Yeah. >> Just look for the null, if it's null.
[62:43] >> You just -- I mean, we only have a limited number of objects, so we don't need to worry about, like, again, the JavaScript people will probably yell at me for this. We don't
[62:55] need to make it the most performant thing possible. We literally need to iterate through these eight objects and figure out which ones are null. If we just do a for loop here, like,
[63:05] it's fine. We don't need to do a map and filter. We could probably do a map and filter just to make it easier, like, if we just do, like, filter this, you know, x is null, which now,
[63:19] actually, I want to try that and just see, like -- >> Yeah, that would be perfect, right? Because it would pull out all those x's. Yeah.
[63:24] >> Mm-hmm. >> Would -- for our GitHub, would we -- it's not going to be an ad. Would it just be -- would
[63:35] that be enough for the issue, or do we need to define it more? Because it's not a feature or anything.
[63:42] >> Oh, no, don't worry about that. I would just assign it to yourself if you want to, and then, like, let's just work on it. While you're doing that, I'm just seeing, like,
[63:53] if I can sketch out, like, what this should look like. Hmm...
[64:13] How does that work, though? Because that's not going to be -- that's not -- that's a -- it's an object. It's not necessarily a -- hmm.
[64:45] >> Oh, yeah, the whole thing was an object, not an array. Yeah, let's see. >> Let's see. JavaScript.
[64:52] >> You got to drill into these funnels. >> Object. Filter. I'm pretty sure there's, like, an object filter. How to filter an object
[64:59] with JavaScript. Using reduce and keys. Okay. Object entries. Oh, and that's just an array. That just makes it -- okay.
[65:18] >> So, I guess we want to look at the files and then by index or by their key and then find the ones with a value of null, yeah?
[65:29] >> Yeah. There's a -- >> A way to drill that in there, huh?
[65:33] >> Yeah, there's a way to drill into it. You can implement this more elegantly using lodash's flow function, which behaves like a pipe function that lets you change static
[65:44] methods, like object from entries. >> This one is starting to go above my head. So, I vote you share your screen, Jay, because
[65:54] then you can see what you're searching for and as you're going through. >> I mean, don't feel bad. I'm trying to -- I'm figuring out the same stuff. I'm just reading
[66:06] and, like, scrolling and being like, does this work? Because there's a couple of thoughts here because we're not sure what the -- we're not sure what this output is and I don't necessarily
[66:25] -- oh, wait. Let's just do this. Copy and paste this output. Your actual output. Just paste that in there. Paste the whole thing. Because we're going to need to -- yeah. Because
[66:39] we need to make sure that we can actually get to it correctly. Perfect. And just paste that. Put it on, like, line 17. Yeah.
[66:53] All right. So, we've got this object here. Let's just call this -- I'm just going to comment this out just to save us some API calls.
[67:23] Because then -- and we're not going to do that. So, now we can test -- we can hammer this all we want for free. All right. So, we have this object. What do we do with this object?
[67:39] Oh. Did I -- did I put something in the wrong spot here? Nope, nope, nope, nope. This. Cool. We can also -- yeah. There we go. All right. So, if we have that
[68:04] and we just want to see what we're working with, let's play around a little bit. Console log request dot -- this is what I was -- this is what I figured. All right. So,
[68:25] we need to first get to it, which means that it is in data. Request dot data. Files? Is that files? There? Was that it? Data? Files. Actually, first and foremost, health percentage.
[68:41] Your health score is that. Can you run that? Oh, I should save it. Can you save it? I don't know if I can save it.
[69:00] I got it saved. Okay. Oh, I didn't get the output, so now I'm having to jump over here. Did it -- it said that it yelled?
[69:27] Oh, yeah. I probably -- yeah. I forgot to do a thing there. Try again. Apparently, it does let me save, by the way.
[69:42] Okay. Reading health percentage. Read properties of undefined.
[69:47] Is it not -- oh, maybe it's not a dot. Maybe it's -- Is it date or -- is it supposed to be date or data?
[70:01] Oh, yeah. It's supposed to be data. Good catch. Good catch.
[70:05] I'll let you do that. You got that. You earned that one. Thank you. Thank you.
[70:09] You earned that one. All right. Let's see if we --
[70:15] Okay. Boom. Your health score is 62. There. Look at that.
[70:18] So, homie's literally going to copy and paste that and be like, my job is done. [Laughter]
[70:26] You may even be able to put that down in the little bottom bar and be like, health score is six. You know, all of those things.
[70:34] That's a health score right there. Show that off. Yeah. Just -- because if -- especially if you, like, pull, like, a brand new project and you're
[70:41] like, oh, why is the health score so low? Like -- Right. Right.
[70:44] That's just -- that's a non-invasive reminder. Right. And then what you should do is make an inactive button, Jay.
[70:50] We -- where you click on the button, it takes you -- it opens it up. Opens up the community standards.
[70:54] See? See? This is -- And runs through it for you real quick.
[70:57] Teamwork. Teamwork. All right. So, Jen, all we've done, this -- we made that input, that output there that we got, we made that into a variable called request.
[71:10] And now we're just drilling into request. Tracking?
[71:18] Yes. Okay. And that's what we said. Your health score is whatever this value was. Go get that value.
[71:26] And now we can actually just do the exact same thing again. And instead -- well, let's figure out some stuff first. We're gonna create -- hmm. Files are -- and I don't know -- we'll fire this
[71:45] for now, because I'm sure -- I'm sure I'll break something if I don't. Let's -- no, not let. Request.data.files. Can we do as array? No? No? Okay. So, this is the part that I wasn't sure
[72:12] about. Oh, that's jQuery. No, we don't want jQuery. jQuery doesn't do nothing for us. Okay.
[72:21] And Homie dropped us a heads up. Oh, no.
[72:25] And I just realized my fan on my computer is not on. So, it's, like, freaking out at me. Oh, it's very upset?
[72:31] Yeah, I should probably turn that on so it's not so mad. As one in combination with objects assign.
[72:39] Yay, Homie's back. Hmm. Welcome back, Homie.
[72:44] Object filter. That's a lot of stuff. Using map and spread syntax instead of reduce. Using object entries or from entries.
[72:58] Ah, I think I figured out how to make it so it just follows you around. Oh, very cool.
[73:10] I think so. We're gonna find out. Solution in vanilla JavaScript. Object entries from or dot filter.
[73:18] Yeah, so, it's just saying do the it wants you to do from entries. Or what? Includes. Includes.
[73:27] Oh, okay. Interesting. All right. So, we do request data files from entries.
[73:42] Or is it from entries dot file? Yeah, I did that backwards.
[73:54] So, this is we're creating a new object. Object from the entries of this. And then we need to filter. So, filter what is this?
[74:15] What are you telling me? Filter and then we're gonna do key value? Oh, filter with key value.
[74:24] Key value. Return.
[74:33] Nope. My example is being lost here. Oh, you just do whether or not it's true or false.
[74:46] So, then we say this is the part that I'm going to be sad about leaving StreamYard is not having the ducks.
[74:58] Do you have epidemic sound?
[75:07] No, I need to get it because I need to get more royalty free music for sure. Yeah. Can you run this? I don't think that. Oh, sorry. One second.
[75:20] We're gonna do that and then console log files. Okay. Yeah. Can you run that? Object is not iterable. Cannot read property. Simple iterator.
[75:47] Oh, object entries, whatever the values are. Okay. I missed. I messed up here. Object from entries.
[76:02] Do. Like that.
[76:30] Try that. Not exactly what we were going for, right?
[76:40] No. Okay. I'm like. Oh, yeah. We had that twice. Okay. Let's start with just this. Try that.
[76:56] Okay. So, now it's giving us the data and we need a filter and we need. What do we do? Like code of conduct as a filter and then if equal no.
[77:20] Okay. Well, what we're trying to do is we're trying to avoid having to write it for each one. Okay. And just have it as a one liner. One liner doesn't have to be a one liner. Just
[77:33] it can be, you know, this works too. It's mostly so that like when we go to make the change because we're doing the same thing for all
[77:47] of them, we only have to make that change once instead of making it, you know, like if for some reason they went from being null to being like empty or something like that, then we just change
[77:59] that area. Got it.
[78:01] Okay. Oh, and then value equals.
[78:14] Thank you, Ryan, for sharing. Yeah, we. Try that.
[78:18] This one isn't currently up. What we're currently working on is just a scratch pad, but I might still upload it.
[78:28] There it goes. Yay. Because I feel like we're making progress. Plus,
[78:34] it's a good learning experience that others can possibly use. Yeah. All right. So, let's break down what we did here.
[78:42] Um, we created this files folder, and the first thing in that files folder is like, or sorry, I said folder. We created this files like object type thing.
[78:55] Um, I don't even know if you had to do like that. Now I'm tempted to just be like, can we do. Hmm.
[79:05] Well, before I break it, I mean. I'm glad you thought that because I was like, please don't make it all go away.
[79:29] Like, I will like stop the screen so I can go back and look. Yeah. Request data files. Can we just do filter like that? Does that work?
[79:39] Try that. Filter is not a function. Okay. That's fine.
[80:00] I don't know. We still need files. I know that this is on repeat, but this is still like my favorite.
[80:22] Lo-fi. I just always like, it just makes me happy. The reason I'm trying to figure this out is like, I feel like it's already like,
[80:35] why do we need to, if it's already an object, why do we need to make it an object again? And that's where I'm, I mean, I'm not entirely sure. I could be wrong.
[80:49] Homie, just as a heads up, in case I didn't say this out loud, you're on mute just because it had weird noises, but I don't want to make you think that we're not wanting to talk to you or hear you.
[80:58] Oh, I've been talking. I guess you haven't been hearing. I'm sorry. I'm sorry if we have been ignoring you all this time.
[81:07] I just like they're in the trenches. No worries. They're in the kitchen. No, no, not at all.
[81:12] No, I needed you just because there was like some weird noise and I'm like, I don't know what that is. So I like, I'm testing our mutes on whose noise it is.
[81:22] But I'm like, normally Homie would have something to say about this, so I better make sure he knows.
[81:29] Yeah, obviously. Well, I cannot take blame for the noise, then the noise was not me. Oh, okay.
[81:37] Try it. Try it now. I just really hate the idea. Okay. Yeah.
[81:45] Yeah. Okay. So you made it into an array of arrays. Okay. Huh? An array of arrays.
[81:56] Okay. So that's what the object from entries are. It's basically taking that array of arrays and being like, hey, I turned them into an object for you, which honestly we don't even need.
[82:14] I doubt we want it to look like that, though, to where it says like all lowercase and none of that stuff. So what I would probably do is do like make another object
[82:22] that says like that. As a heads up, I'm going to eat some food while we're streaming, so I'm going to mute myself
[82:46] and turn off my camera, but I'm still here. So if you need me to run something, I'm here. Okay. I will need you to run something in a second, but you got some time.
[82:56] I mean, I think you can give me like the ability to run these. Oh, yeah. In yours, you go ahead and open the terminal to him.
[83:06] So you let him live share your terminal. Then I'm going to delete all your files. Just kidding. I mean, it's just granola bar,
[83:22] so it's not bad, but I know people don't like freak out seeing other people eat like some people have that. So I'm like, I should not eat on camera.
[83:36] I don't know how to do that to give you access for that. So let me see where I found it, but it gives me something to do when you get far enough. So I'm like, yeah, I'll run it.
[83:46] I don't really know the best way to do this, so we're just going to do it that way. Okay. Why am I not copying this? Come on now.
[84:10] Rookie numbers. Let's go. Oh, that's interesting. That's actually interesting because I think code of conduct
[84:44] is attached to, I think it's attached to the file, but I think the file is actually more important. That way, if you provide your own custom code of conduct,
[84:56] I wonder what that does here. If this is null, that might be a test to try out. Okay.
[85:26] Okay. Something like that. Of course, it's going to yell at me because I capitalized the thing. Oh, dear.
[85:47] Oh, it's never right. That's fine. I got back in time. I'm excited. All right. So what we want to do now is this, like, we actually don't want to do,
[86:07] hmm, let's see. Objects from entries. That's what that was. Like that. That. Okay. So we want that still, and then we want to go in and mess with this filter.
[86:25] And instead of actually passing in the filter, we're going to do... Could we just direct it to a different file that had directions? Like,
[86:41] if it was a code of conduct file and it showed, like, it'll run something else? Well, that's kind of what this gh-files here is. We don't necessarily want it to, like,
[86:53] we don't want to do the whole, like, let's start, you know, prompting them to change stuff. We just want to be able to give them a value that they can then decide to do something with
[87:11] if they want. And that's why... Yeah, well, if it's like that, I meant, like, more like, if it showed a different file, just so that way it was, like,
[87:21] another, like, a reading for that code of conduct of what they could change. Um, not sure. Right now, I just wanted to read, instead of saying, like, code of conduct
[87:38] with all lowercase and stuff like that, have it actually output regular text. Okay.
[87:45] What's up? Total side notes real quick. It's bothering me a little. Can I change that name? Your
[87:54] bar name let files. Can I change that? Yeah, sure.
[87:57] I like it. Beautiful. But now what we want to do is we want to filter this based on these keys.
[88:14] So, we're, like, and that's where I'm trying to jump back into this of, like, hmm.
[88:20] Oh, includes, includes key. Hmm. No, it's not includes key. It's, like, like,
[88:36] key value. It's still key value, though. It is still key value where gh files keys. Hmm.
[88:47] Oh, wait, wait, wait, wait. This changes to gh files. And then this is request data files key. So, key is equal to null.
[89:19] Jen, try that. Oh, hold on. Wait, wait, we gotta replace this with missing entries. There we go.
[89:32] Okay, what was the, what was the error? Objects is not defined. Okay, that's, that's because I did objects not object. Okay, there we go.
[89:52] Try again. There we go. Those are the things missing, right? Yeah.
[90:01] Yeah. Yeah.
[90:04] Yeah. Yeah. It's the object, which is three items. That's easy enough. Yeah.
[90:13] Yeah. And, I mean, in reality, like you said, we don't necessarily even need the objects from entries. If we just do that and we get that array of arrays, you just do map,
[90:33] uh, what is it, at index one, so. Look at me acting like I know what I'm doing.
[90:46] No clue what I'm doing. You're doing it.
[90:50] You're doing more than I know how to do. Try that.
[90:55] I'm learning a lot by. Now try it.
[90:57] By watching it all in. Yeah.
[91:02] All right. So, let's, let's add some comments here. Look at that. That had a, that put out an array of just the objects.
[91:14] Yeah. Dude, Jason got the mojo.
[91:19] Now we're, now we're just getting cocky. And then say, oh yeah, he's going to pull apart now.
[91:32] Yeah. Yeah.
[91:33] Oh my goodness. Try that.
[91:49] This could go terribly wrong. Nope.
[91:55] And look at that. Yeah. So, you know, you make it something like you're missing the following files.
[92:05] And that's your, that's your message there. And it's like, oh yeah, you're, you're doing all these things and.
[92:18] I mean, you could also, you could also just join them on a new line too, which probably would look cleaner.
[92:24] Yeah. That might look a little, hey, Jen. I know Jay was saying this is throwaway.
[92:29] Don't throw this away. Yeah, I know, I was just saying that earlier.
[92:33] I was like, no, I'm going to still upload this one. Yeah, that's fine.
[92:36] That's fine. Just, we just have to know where to upload it.
[92:39] That's the, that's the real challenge. Yeah.
[92:43] What this is, is if you run it like this, what we're doing is now that we're just, yeah, we're just styling the, the like, what the error message would be like, you're missing the following files. Bam, bam, bam. And what we may want to do is like, you don't even, you may not even want that in this joint statement like this.
[93:02] You may want it as separate entries. That way each entry could be a clickable thing.
[93:08] Hold on, I'm going to swap these console logs real quick, just because I think it'll look a little better. Or the other side of that is you can, instead of joining them as one, you can do like a for each.
[93:24] So, if we do like, we're going to wrap this, we're going to do like, for let message equal, oh wait, no, it's for, what is it, for let message in missing entries. Yeah, yeah, okay, I see what you're doing.
[93:45] Okay. Oh, okay.
[93:47] And then we'll just, we'll throw this on top of that, like that. Oh yeah, yeah.
[93:51] And then we'll rip this out, that there. And like, I know we're like, we're like playing right now, but this is, this will allow us to like, construct that message in a way of like, you could do something with this.
[94:14] Right, right. Like console log, this is just message.
[94:20] And then, you know, something like that. Run that.
[94:35] I will say I kind of, I also think I like the, the, the run that part because then I get to like, I don't know, I don't know, I don't know, I don't know. I will say I kind of, I also think I like the, the, the run that part because then I get to go, yeah, I get to clicky, clicky.
[94:53] Okay, so this is, this is where we're, we did something wrong. Oh, it's probably just doing the, let's do like this, or no, it's not in, it's of.
[95:06] Oh, okay. Oh, wait, I already did the map. So yeah, just run that.
[95:15] Yeah. Yep, there it is.
[95:19] Yeah. So then like, so this, this console log isn't necessarily a console log, what it becomes later is like, I don't know, VS code button. Something, I don't know.
[95:39] Yeah, right. Yes, that's what it did.
[95:43] Exactly, like. This is just driving me insane, I'm re-gaming this one.
[95:47] Okay, that's fine. Oh, yeah, I was trying to figure out the best way to look at that, because having it as all caps, like, some of these are supposed to be all caps.
[95:58] Yeah. Oh, but did I break it?
[96:02] No, you didn't. Oh.
[96:06] It doesn't know what VS code button is, it's like. I didn't do it.
[96:10] Yeah, no, it was just like, I don't know what you're doing. It's like, I don't know what you're trying to tell me here. Okay, let me say one more time.
[96:18] Yeah. It's easier to read that way.
[96:22] Yeah. The cap one is making me like go, ah.
[96:26] Yes, yes. I randomly click things, and now I have a clicking counter when I randomly click things.
[96:38] Nice one. Nice one, Ryan.
[96:42] Yeah. But, all right.
[96:46] So, this is, like, this is the core logic of what we're trying to do. Right.
[96:54] Now we would need to type scriptify it, which is not a thing that I can do right now. My brain is, I think I'm done.
[97:02] I think I'm brain dead. So, let's do the easy part of this.
[97:06] Okay. Which is documenting the things that we need.
[97:10] And what we can do is we can test this on one of my projects just to make sure that everything still works. So, first things first, we're going to remove these comments.
[97:26] Well, I was thinking, do one of your projects have, like, nothing in it? When you say nothing, probably not.
[97:36] But I probably have some that need a lot of work. So, if we do async function get request, or we can say get standards, get community standards, something like that.
[97:56] And what is this doing? This is -- well, first import -- oh.
[98:12] >> Hey, Jay, what if on that function community standards score? You want to -- did that download?
[98:18] >> Well, because we're getting all of the data itself, I didn't want to do the score. Yeah.
[98:24] >> Yeah, fair enough. So, we're going to say, what, create a new Octokit instance.
[98:34] Then fetch the standards of the current application. Or the current repo.
[98:52] So, what we're going to do is we're going to take those out. Because these are placeholders right now.
[98:58] We're going to pass them into this. Owner.
[99:02] Repo. Like that.
[99:06] And then we're going to pass that stuff in. This can all be one line.
[99:10] We don't need to make that any more complicated. Like that.
[99:20] So, objects like that. It's kind of a weird, weird call.
[99:28] But we're going to keep the then on the next line. So, we can like...
[99:56] And instead of that, we're going to -- instead of console log, we're just going to do... That.
[100:08] I think that works. Don't need...
[100:18] I'm going to comment this out. I'm going to just drag it to the bottom.
[100:22] That way it's all clean. These are also constants.
[100:46] There we go. That way we can test it on something that we haven't messed with before.
[100:50] That will have a different result. >> Let's see.
[100:54] >> I'm embarrassed about. But it's fine.
[100:58] You're already running it. It's probably not ready yet.
[101:02] >> I like to clicky clicky. >> Okay.
[101:06] >> So, this is the fun part about doing it on my computer. And while you're still doing it.
[101:10] >> You can just run it. Well, just remember, we're actually hitting the API.
[101:14] So, every time you use it, that's less API calls we get. >> Except if the request is not defined.
[101:18] Then we aren't hitting it. >> I don't know.
[101:24] Because I think we might still be. I honestly don't know.
[101:34] Because I don't know if creating the actual link is a hit. Because we are doing new Octokit.
[101:42] And that might still be taking that down. So, then.
[101:52] We've done that. And we do, like, all right.
[101:58] Retrieve the missing entries. And return their cleaned up name.
[102:12] >> If you're looking, Jen, it's over on the left side on the bar where the icons are. Way left side on your explorer.
[102:20] And you go down to live share. If you wanted to add it to the terminal.
[102:24] That's what you're looking for. >> Create a new mapper.
[102:28] >> Oh, no. I just didn't -- I want to stop following him.
[102:32] >> Oh, because I'm just all over the place? >> Yeah.
[102:36] And I just don't know how to stop following people. >> I think it's on the left bar.
[102:40] Those three dots. It's probably hidden.
[102:44] It's a live share icon. The three dots on the main left of your explorer.
[102:48] >> Oh. >> Left side.
[102:52] Up, up, up. Those three dots.
[102:56] Click that. And live share is hidden under there.
[103:00] Did you click the three dots? >> Yeah.
[103:04] I'm clicking it. It's not doing anything.
[103:08] But additional views comes up giant. >> There you go.
[103:12] Hit that live share. >> No wonder that was confusing.
[103:16] Ah-ha. Unfollow.
[103:20] Yay. >> There you go.
[103:24] >> Homie, do you see what I'm doing with this? >> Okay.
[103:28] Walk me through. I'm looking.
[103:32] Oh, yeah. Okay.
[103:36] >> Making it an engine as well. Making it an object.
[103:40] So that later on when we call these, we can just say, like, when we go to save it, you're just whatever that file type is called. You know.
[103:52] File. That will also make this easier when we do TypeScript.
[103:58] TypeScript is super finicky about stuff. >> Right.
[104:02] >> So this, like, will have, like, this, like, I don't even know, const. >> Structure.
[104:08] >> Yeah. Oh, yeah, actually, that's what it is, isn't it?
[104:12] It's, like, something struct or. >> Oh, no, you want to do a type art interface.
[104:16] A type art interface. Interface, probably.
[104:20] Yeah, interface. >> Yeah, interface, like, gh file, something like that.
[104:26] And that's a struct. And then you have to do, like, that whole thing.
[104:32] I don't know what I'm doing here. I think it's something like this.
[104:36] And then you would do name. >> I think you could get rid of the struct.
[104:40] >> String. Oh, do you?
[104:44] >> Yeah. Get rid of that.
[104:48] That's it right there. I think it has to be capital, right?
[104:52] >> I don't know. Maybe.
[104:56] >> So then when you do your next interface for, like, whatever gh files are, you're, like -- >> Mm-hmm.
[105:06] >> Then it's -- >> It's typed and consistent, yeah.
[105:14] >> Yeah. And then it's just, like, gh file or something like that.
[105:20] It's something along those lines. I don't really remember.
[105:24] And maybe this isn't an interface or a struct. It's something else.
[105:28] >> A type. >> Well, because each of these are different.
[105:32] So it's, like, I don't know if it's a class or, like, what that is. But it would be something.
[105:36] I'm just going to comment all that out and be, like, we'll need to define a string. Gen, how far are you tracking so far?
[105:54] Are you good? Or do I need to slow down?
[105:58] >> No, no, no. I'm tracking pretty good.
[106:02] I'm letting it sink in. Like, I'm still tracking.
[106:26] But it's a lot of, I think, just being it. >> Well, this file here, it seems like we got ourselves a few things that, like, Jay's notes right now we could do is throw them in as issues.
[106:40] >> Yeah. >> And then start typing them.
[106:44] And then that one, I'll go ahead and get the base extension done today and start that and get that and see if I can get octokit hooked up in there. And then I'm worried about that.
[106:56] I want to make sure we get whatever we've got to do so we can not get limited by the API either. >> So if you go to -- if you look at how Ultra Foreign is doing, I'll put it in the private chat.
[107:12] You can see how he's calling it. Actually, let me just go directly to the file that he does -- calls it in.
[107:24] API indexed, yes. >> Guys, it's just about 11.
[107:38] I got to jump off. >> Yeah.
[107:42] >> I've been doing this forever. >> I'm just going to clean this up and then, yeah, we can bounce off.
[107:48] I got to do some worky work. >> Yeah, yeah.
[107:52] I'm going to go jump in. It will be in the repo.
[107:56] You're going to throw this in there? >> Mm-hmm.
[108:00] >> I don't know how we put it in there. >> Yeah.
[108:04] >> And then I'll get that extension started today. >> I was just going to -- and see if this theory works, but if I add the files to my clone, as long as it's a different file name than index and install Octocat, then it should upload to community standards, shouldn't it?
[108:28] >> Yeah, I mean, if you even want to put it as like a scratch, like, I would just rename it to like scratch and then just put that file name in your clone. And it should work.
[108:40] >> Yeah, yeah. Scratch.
[108:44] I'll be old scratch. Okay, guys.
[108:48] Hey, this was a great session, guys. >> Yay.
[108:52] >> We'll talk later tomorrow. We'll talk on Discord or whatever.
[108:56] >> Absolutely. >> Thank you, homie.
[109:00] >> All right. See you.
[109:04] >> All right, Jen. I think --
[109:08] >> You've done all the things and stuff? >> Well, I didn't do all the things.
[109:12] I'm cleaning up -- I'm basically making it so it's more copy and pasteable into our project, because that's my fear, is that you're going to copy and paste and be like, why didn't it work? And it's because TypeScript is savage at times.
[109:26] >> Fair enough. Fair enough.
[109:30] >> But all this is doing is making it so that as we need to call these things, we'll have a little bit of a nicer time. There's probably also this argument of, like, path options or something like that.
[109:50] That's probably just .github or root. >> I mean, this works for -- like, you and I can still work on this, and I'll keep sharing it with you.
[110:10] But I think for today, like, we are good with the stream. So y'all, as a heads up before I just say goodbye, y'all are getting raided, you know, to another coding stream.
[110:22] So that's starting. And see y'all on Thursday.
[110:26] Thursday I'm probably doing something with this project or with the TweetyTag app. So see you then.
[110:33] Bye, everyone. >> Bye.

