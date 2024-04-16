---
showLink: "https://www.youtube.com/watch?v=eKhJiBHaWpA"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-code-review-with-jere-suikkila"
title: "Teach Jenn Code Review with Jere Suikkila"
publishDate: "2022-07-14"
coverImage: "https://i.ytimg.com/vi/eKhJiBHaWpA/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome to our return guest,
[00:08] who was our very first guest, Yere. I try to do the role because Ramon also told me,
[00:15] there needs to be a role in his name too, Ramon. I'm working with everybody's names.
[00:22] Once again, welcome to Teach Gen Tech. For all of those tuning in for the first time,
[00:31] we've had, let's see, it's been a week and a half since Teach Gen Tech has launched.
[00:38] I guess I've shown up because Teach Gen Tech came from, I really want to get into the DevRel role,
[00:47] which is developer relations. That is a whole another topic in video,
[00:51] yet something a lot of people were saying was that, I need to have content and I need to know how to code.
[00:59] Well, I didn't have either, so we'll lock. This was launched of Teach Gen Tech and Yere was
[01:06] the very first guest and teaching me how to build this really cool site of what are we going to
[01:17] do in using JavaScript and HTML and CSS, and we're doing a code review,
[01:23] which I'm pretty sure you're going to tell me I built it all in HTML. Yeah.
[01:31] Hi, Yere, please introduce yourself. >> Hi, indeed. I'm Yere.
[01:36] Glad to be back and I'm glad to be following your journey. I also do developer relations.
[01:42] I work for a company called MappedIn. We do indoor maps, mostly for malls.
[01:47] I think some people might consider me to be a map geek, so I follow subreddits where there's pictures
[01:53] of cool maps and things like that. I also love coding and I enjoy talking about it.
[02:01] When I saw you were wanting to learn something about tech, I figured, hey, I might just come on with you and see
[02:08] what we can learn here, what I could teach you. Because that's also part of what you do in developer relations.
[02:17] You're trying to teach other people code or some technologies. This is all learning for me as well,
[02:23] and I think it's great to be here. >> Thank you. I think that's the cool thing with Teach Gen Tech.
[02:31] First off, if anybody wants to come on live and learn with me, totally down, let me know.
[02:36] We also have, you can submit for guests on my Twitter page. Sure, we're going to go with that. It's the pinned tweets.
[02:44] Yeah, I think that's the beauty of it, is we are all learning and teaching at the same time.
[02:53] It's having that empathy for ourselves, but then for others. Yare and the rest of the guests that I've had on so far
[03:01] have been very kind when I'm just like, I don't even know what you're saying,
[03:05] because it's like it needs to sink in, but it won't always click at the moment.
[03:09] That's what I keep having to remind myself and go, sure, and yet I've seen so many of the building blocks
[03:18] of what you taught me actually makes sense now because of other conversations that we've had so far.
[03:25] It's been quite a journey. >> That's awesome. That's why I also wanted to
[03:31] go a little bit further that I knew that you maybe weren't quite ready yet.
[03:36] I was showing you things that you had never seen before, and I knew that it's out there.
[03:40] It's not just basic HTML. But I wanted to go a little bit further because on your journey,
[03:46] you're going to be facing a lot of these things, and the more often you see them,
[03:51] they start clicking in better, and you start making these connections.
[03:53] You remember all that piece there from the second stream I had, connects to this one now that I'm doing four weeks later.
[04:00] Is that it? Then you start making these connections. That's when you really start getting the feeling that,
[04:05] oh, I have learned something. You get those aha moments.
[04:08] I know what this is. That's one part of learning tech.
[04:14] You get those feelings, I know what this is. The second part is, there's two modes of
[04:21] this learning technology is I have no idea what I'm doing. You're just staring some piece of code,
[04:27] happens to me every day. I'm like, I don't know what I'm doing here.
[04:31] I touched so many different coding languages today, it was incredible.
[04:35] I think I wrote or read code in five different coding languages today.
[04:42] I'm really not an expert on most of those. But honestly, at some point I was completely lost.
[04:52] I had no idea what I was doing or what I was supposed to do. >> Did you have to get them all talking together?
[05:00] >> No, not together. Luckily, they were like individual pieces that were independent.
[05:07] But it highlights the fact that doing tech, in DevRel especially, it's you're always learning something,
[05:15] and you're always going to feel like you don't know everything because the truth is you don't know everything.
[05:21] That's something you'll just have to live with. >> Yeah. Thank you for saying that because I
[05:26] think we're going to have a guest come on. Twitter handle is M4DZ.
[05:34] They're going to be going over how to start reading documentation, like how you use documentation,
[05:44] how to create good documentation. Because to your point,
[05:47] you had to use five different coding languages today. Where do you start when you're looking at them?
[05:54] I'm excited for that. >> Yesterday, we had Rizal from GitHub on,
[06:01] and she was explaining the differences between Git and GitHub. I'm like, "Whoa, it's finally starting to click."
[06:09] To repeat and echo what you said, we can learn a lot and still feel like we have no idea what is going on.
[06:18] Yes, Anthony, sit down and be humble. >> Yes. We're working on doing so.
[06:29] >> I'm glad we're doing it live. It's really fun to do it this way too.
[06:33] It does humble you definitely when you're doing it live in front of an audience. That's a brave thing to do as well.
[06:42] >> Anthony, I appreciate all your help and earlier, that's why I was just like, "I'm not computing now, okay, bye."
[06:50] Because that was the cool thing is I really appreciate that a lot of you have been joining multiple streams to see the journey,
[06:59] and then helping me on my way. It's also really cool having to learn that about myself and being like,
[07:04] "Okay, Jen, they're helping you, calm down. They're not just trying to boss you around, it's cool."
[07:12] Having to, what Anthony just said, it was just like being humble and appreciating others wanting to help.
[07:20] It's been definitely a learning part on my own too. >> Yeah.
[07:26] >> Awesome. Are we ready to look at my code? >> Yeah. Let's look at some code.
[07:33] Let's see what happened. What are we looking at here? >> Really quick, just so that way we have it on the record.
[07:44] How would you explain what a code review is and why it's important? >> Yeah. Code review means that you're looking through the code,
[07:55] so you read it and you have to understand what's happening there, and you're giving feedback about it.
[08:01] That's part of the software development process, software engineering process where somebody else writes a piece of code,
[08:10] and then their code gets reviewed before it's put forward, let's say, to a live service or in front of an audience and actual users.
[08:20] If you think about how books or newspaper articles or something like that are written,
[08:26] they also have editors, right? There's always somebody else who goes through the work before it gets published.
[08:32] The principle is the same. People make mistakes, we're all human.
[08:38] We also get blind to our own mistakes very easily. It's very difficult for us if we write something and we try to read it
[08:47] back and see if there is a mistake in there. It's part of creating quality software,
[08:56] especially in Teams, that somebody else goes through the code before it's put forward and merged with everything else.
[09:04] Merging means putting together everybody else's contributions, and I think that's something that you've covered with Resell as well.
[09:11] >> Yeah. It makes a lot more sense, at least seeing it. We did an example where we gave feedback for somebody to correct.
[09:21] Ramon actually sent a PR in and we were able to say, "Hey, this is a typo,
[09:27] please fix and then submit," or then we could commit it. It's very interesting and it's starting to sink in.
[09:35] Yet in the real world, how often is code review done every single time?
[09:41] I know that in theory, like in an old job,
[09:46] I knew that people would submit PRs to me, but I didn't know what I was doing.
[09:53] It was just set up in the GitHub area, however you say for a company,
[10:00] that it would need to be approved. It had to be approved from someone.
[10:04] It was on the marketing side and I would just hit "Approve." I didn't know what I was approved,
[10:09] I didn't even know what I was looking at. But they just needed it approved because it was set up that way.
[10:15] How often does it actually get looked at and what's the process normally look? Is it like a weekly thing?
[10:22] Is it an every time thing? How does that structure get set up?
[10:26] >> Yeah. Very often used, I think we could do a whole episode,
[10:32] but what is Scrum and Agile software development methodologies and how software is often developed
[10:40] in terms of how that process is organized very often. But as part of all that,
[10:48] there is that review process that's sometimes, if you think about it, also mandated by a third party,
[10:53] let's say an auditor or something like that. Otherwise, a single malicious actor could inject code
[11:00] into a program that's not supposed to be there. There are that compliance aspects to this code review as well.
[11:10] I can't speak for all companies, but oftentimes what happens is every piece of
[11:17] code that becomes part of the application has been reviewed. Everything has been reviewed.
[11:23] As you noticed in your previous experience as well, the GitHub was set up so that
[11:29] everything that goes live needs to be reviewed. In some cases, it was reviewed by someone in marketing,
[11:35] but which defeats the purpose a little bit. You can't really give good feedback suggestions
[11:41] because not only can you do malicious things, you can do honest mistakes that causes bugs,
[11:47] but it's also performance improvements. Because there are different ways and
[11:52] algorithms that you can write these things. If another set of eyes goes through it,
[11:58] they can get more performance out of the code. They can say, "Hey, look, there's a better way of doing this."
[12:03] We save a couple of orders of magnitude of running time. Let's say something that should take a few milliseconds,
[12:13] takes a second to do, and then somebody else looks at it and says,
[12:17] "Hey, I know that there's a better way of doing this." There are a lot of benefits to it,
[12:22] and that's why it's done every time, all the time. >> Very cool, and thank you.
[12:27] Yeah, I just put that on my notes to bring that up, maybe on Theory Thursdays,
[12:35] doing something along for Scrum and Agile. Because I think that's something that a lot of people are like,
[12:41] "Oh, it's maybe two weeks or something, and some daily meetings,
[12:45] and not something that's really talked about on the human aspects side of it."
[12:51] I don't want to get too caught up on that, especially because I've been sharing
[12:55] my screen while we've been talking. Where do I start with a code review here?
[13:04] >> Yeah. I think usually how code reviews happens is basically, you set that pull request to me,
[13:10] and then I'll go through the code on my own. Maybe in this case, I'll guide you through
[13:17] the files that I want to see what you've done where. >> Sweet.
[13:23] >> I'll talk to my observations, and then maybe I'll ask you some questions.
[13:29] If we were not doing code review live, as it often happens these days, for a couple of reasons.
[13:35] Of course, you get the record of it for posterity for somebody later, if you write this in the comments in that pull request.
[13:42] But also, like you asked, there's not a meeting time once per week when code reviews are done.
[13:52] They are sent and then everybody does them when they have the time to do it, so it's asynchronous work.
[13:57] We're doing a little different here today. First, let's look at the output.
[14:03] What's here on the white background on the output? Maybe you can describe to me why you did this,
[14:11] what was the purpose that you were working towards, and does it do what you expect it to?
[14:18] >> This is something that I am remembering from last week when I was working on this.
[14:26] It's not doing exactly what I expect it to because I thought I deleted all of this and it was all gone here.
[14:37] I thought I deleted Hello Vanilla and the text underneath that and added Hello Beautiful Humans and some of my favorite podcasts.
[14:47] Yet, when I went to look at the domain name in a different tab,
[14:57] it added it back in there. I was like, well,
[15:02] I got it to do what I wanted to do below, so I'm going to call it.
[15:06] The goal was to replicate what we did in the index.js file and the index.html file
[15:20] to hyperlink three podcasts that I listened to and have them go as bullet points instead of all on
[15:28] one page and using JavaScript to help put them into the mapping for it. Again, I think I somehow built this all in HTML and no JavaScript.
[15:47] >> Yeah, I think that's what happened. Now, if we wanted to get rid of this Hello Vanilla part,
[15:55] clearly we don't want it to be here, so I'll comment on that first.
[15:59] Oftentimes, in pull requests or code reviews, you also look at the output of the code.
[16:05] Then based on that, we can already see it's a little wrong from what you were trying to do.
[16:11] To get rid of that, we have two ways of doing it,
[16:16] but maybe we'll just take off this JavaScript here that sets the app element and everything from line 3-10,
[16:29] you can just delete in this JavaScript file. >> Out of curiosity,
[16:33] I wonder if I did that and if the app is still in the HTML file, could it have re-added?
[16:42] >> No, I think maybe it wasn't saved. If you play with this from here,
[16:47] it could just be that it wasn't saved. Because it does take it out now even without saving,
[16:54] but then when you go see it in another tab, it's not saved. >> Is there a safety for that?
[17:01] Because has that ever happened to you where you did a bunch of work and then didn't save?
[17:05] Is this a common fear to have? >> It's a common fear.
[17:10] That's one of the reasons we use, even for our personal projects,
[17:13] we use Git very often to save our changes. >> I've had it happen when I've been doing video editing
[17:22] and it's heart-wrenching to do two days' worth of work without
[17:30] realizing I didn't save a really important part. Anthony, has that happened to you,
[17:37] not saving something? >> Funny thing is a lot of
[17:43] computer or programmer jokes revolve around the fact that computers just use Control or Command C,
[17:49] Command V, so copy-pasting. But actually, the key combination I use more is Command S.
[17:58] I might write three lines of code and save. There's a couple of reasons for that.
[18:05] I want to make sure my changes are saved. I want to make sure they're there.
[18:10] It also formats my code. I have my editor set up so that
[18:15] whenever I save my file, it formats the code. >> Okay.
[18:20] >> Yeah. We use these formatters and configure them so that everybody writes their code in the same style.
[18:26] For example, in JavaScript, you don't need to have the semicolons at the end of the line.
[18:31] If we didn't have the standard within the team, it would get really difficult to compare what was changed.
[18:41] >> Would that be considered governance or a part of governance? >> Yeah. I think the fact that we have
[18:50] that guideline would be considered part of that, yeah. >> Real quick for those listening,
[18:58] and I did this yesterday when we were talking to Rizal. She was talking about linting
[19:03] and how it's like a spell check for your code. Let's see if I can explain it.
[19:11] The way that governance works is that when an organization or a team, it can even be a specific person,
[19:20] creates a way that things are going to be structured. It can also go into a style sheet so that way
[19:27] everyone knows what they're going to be doing the same. You write a document that outlines how we do things,
[19:38] because there are many things you can do a little bit different. But usually you benefit if everybody does it the same way,
[19:44] because then you don't start bike shedding, which is when you build a nuclear plant,
[19:51] but you start talking about what color should we paint the bike shed for the employees in the parking lot.
[19:57] >> That's where I would go. I would care more about that.
[20:01] >> It is super easy to care about the minute details. But if you have those agreed in a document,
[20:07] then you don't have to argue about them all over again. They're there, you adopt them,
[20:12] whatever the team uses, maybe you change them. It doesn't have to be a static document.
[20:17] Of course, it can change for a good reason, but it helps people work better in a team together.
[20:24] >> One other thing that I do want to mention is, y'all, the last few live streams has been with Terminal and VS Code.
[20:34] I personally do love VS Code, it definitely helps me auto-correct a lot of things.
[20:41] I'm learning so much more about it. Yet, it doesn't do this instant output,
[20:46] which is by far a much, it makes it a lot easier to learn yet and see visually what it is right away.
[20:56] I just want to give a shout-out to you, Jere, for suggesting this because it's like, "Okay, cool."
[21:03] This is at least giving an example, even though you can do the same in other ways,
[21:09] it's just a lot harder or more steps. I wouldn't say necessarily harder, just more steps.
[21:15] >> Yeah. There's a time and place for all of that. I feel like for beginners,
[21:21] whenever they start learning things like coding, it's very important to get fast feedback of what you're doing.
[21:27] If you have to write something for an hour and read something before you see the result of two plus two in your console,
[21:34] it might not be the most motivating experience. It might be like, "Is this really this hard?"
[21:40] >> Very, very true. I deleted the JavaScript that was pulling HTML
[21:50] to delete the stuff above. >> Yeah. Now the page looks correct.
[21:57] Of course, we did it with JavaScript before, but to be honest,
[22:01] you've done it the smart way. There's no need for JavaScript in this page.
[22:07] Let's go have a look at the index HTML. Honestly, the reason we did
[22:12] JavaScript was just to get an introduction into that. But of course, a lot of pages today are written in JavaScript,
[22:20] and then the HTML is built on the client side and then displayed. But in something simple as this,
[22:29] there's no need for that. We were doing JavaScript for JavaScript's sake.
[22:33] >> Okay. Yay. >> You've done it the website developer way,
[22:38] which is going the smart and easy way out. >> Okay.
[22:44] >> You often want to do that as a developer. You want your output to be simple and input to be simple,
[22:50] so now it's easy and modifiable. Let's start with the row 9 here because that's the first line.
[22:57] That's not part of the template. Now that we changed JavaScript so that nothing is written
[23:06] into this div that has ID of app, we don't need that at all.
[23:12] Nothing changes if you delete it, right? >> I was actually just going to ask that.
[23:16] Now, do we need a space between the body and the, should I delete both 9 and 10 or just line 9 and leave a space?
[23:26] >> You can delete both lines. That's one of those style things that would
[23:29] be your linter would take care of probably. What happens if you hit "Command + Save"?
[23:35] Yeah. Sometimes for me, for example, if I would save and there was an extra space there,
[23:43] it would actually take that space away. >> Okay.
[23:47] >> HTML does not care about whitespace. That means that you can have all of
[23:56] this on one line and it does not care. What it cares about is the tags and the elements.
[24:04] You have the HTML head, so it has the opening tag for head on line 3 and
[24:09] the closing tag for head on line 6. That's what HTML cares about.
[24:14] They just need to be there in the document so they can be parsed. Whether they're on the same line, it doesn't matter.
[24:20] The reason we usually do have things on more lines, it's easier for the reader, right?
[24:26] >> That makes sense. >> Yeah. I mean, but this looks great.
[24:31] We have "Hello, beautiful humans." That's a heading. Then you have,
[24:39] yeah. >> I think something that confused me a bit was what exactly?
[24:51] H1 is header 1. That one made sense to me.
[24:54] It seems self-explanatory with fonts. It's the heading, it's the top and the body of a message.
[25:04] Maybe just because of writing, it made sense to me. But what's a div in an LI?
[25:10] Hey, look, if I just highlight it, it tells me. >> You answered your own question.
[25:19] >> A div is the div element has no special meaning at all. It represents its children.
[25:28] It can be used with a class, lang, and title attributes to mark
[25:33] semantics common to a group of consecutive elements. Interesting.
[25:40] >> Yeah. I actually wasn't going to give you the answer to this question.
[25:43] I was going to help you find the ways how you can find the answer. When you have that question, how to find the answer.
[25:52] >> I was going to Google it. >> Yeah. Let's see what happens if you Google it.
[25:57] How would you go about Googling this? I think we did some Googling last time as well.
[26:03] >> What is a div tag? >> You know what? In all reality,
[26:10] I think tag is something that I've recently learned that it would be a div tag.
[26:15] I would honestly Google what is a div. >> Yeah. I like the second link a lot better than the first one.
[26:26] That's done by the developers at Mozilla. >> Yes. You taught us that the very first time. I appreciate it.
[26:34] I've gone back and looked at a few things, but it makes sense,
[26:38] but it doesn't make sense. I was trying to make sense of a ray and I'm like,
[26:42] I did something. >> Yeah. But that's good.
[26:47] Then that's part of the learning process like figuring out how to find the information,
[26:52] and then going back to it a couple of times, and then going deeper into it,
[26:56] and eventually you notice that things you didn't know a couple of weeks ago,
[26:59] now you're mastering them. Repetition is the key here too.
[27:04] >> Yes. This is the second week I've been doing this of having the coworking days with Jen
[27:15] because I need to practice this, and without having the scheduled time, I'm like, "Oh, I'll do it.
[27:21] I'll do it later when I feel like it." I'm like, "I'm never going to fail like it."
[27:27] >> Yeah. >> Having the scheduled time,
[27:29] I actually showed up today and I was like, "Cool." I was able to put it into
[27:34] practice after learning so much of this. >> Yeah.
[27:37] >> Yes. Okay, cool. This says a div is the content division element.
[27:45] The div HTML element is a generic container for flow content. It has no effect on the content or layout
[27:54] until styled by some way using CSS, e.g. styling is directly applied to it,
[28:02] or some kind of layout model like Flexbox is applied to its parent element.
[28:08] >> Yeah. >> Okay.
[28:10] >> So what does the div do? Nothing. Nothing by default, right?
[28:15] It doesn't do anything necessarily unless you add some styles to it,
[28:22] or decide to use it as like it. It's like a container for content that you can style,
[28:30] so that you have a specific group or something like that, that you can then get a hold of and then style in some way.
[28:39] >> I'm letting that sink in. >> Yeah. Basically, do we need the div tags here?
[28:49] This would be a question for me if I would ask in a code review. >> I'm going to answer with, I don't know.
[28:59] Let me try it without it. No, I guess not.
[29:08] >> Yeah. So in this case, not. I've been taught and I'm not sure how necessary it really is today,
[29:18] that all our texts should be wrapped in some tags. In this case, I would put that in a p tag,
[29:26] which represents a paragraph. >> Yeah. I was looking that up.
[29:32] That was something that I spent a lot of time on, was the types of tags,
[29:38] because I wasn't able to get the spacing I wanted. That's where I spent the majority of my time.
[29:47] That time, I was like, I need a specific spacing, and I think maybe I just figured out.
[29:58] It was like, I don't know. I'm not seeing them in here.
[30:04] I don't know. Maybe I am. Is that what the L and LI do?
[30:09] >> That's what creates the list. >> All right. The next thing I'm going to ask,
[30:18] what's the purpose of this line 13? What is it there for?
[30:24] >> Leftover code from previously that I didn't delete or? >> Yeah.
[30:34] >> Okay. >> Because it doesn't do anything, right?
[30:37] It's empty. It doesn't render anything,
[30:41] like there's no text in it. This is so cool because I was just like,
[30:46] "Oh, I got it to do what I wanted to do. Okay, done." I didn't even think about looking to see and make
[30:53] sure that the code that was there was actually doing something, which just causes a ton of clutter.
[30:59] If somebody else needs to look at it, oh, jeez, okay. >> Yeah. That's one thing about
[31:05] software development and pair programming and these different methodologies that help
[31:10] eliminate that type of stuff like unnecessary code, for example. There's a methodology called test-driven development,
[31:19] where you write a test first, and then you write the code that makes the test pass.
[31:25] You write a code saying, "Hey, we have a function to add two numbers together.
[31:32] If we give it number 2 and 2, does it give us 4 or not?"
[31:37] Then after that, we write the function add. Then once we've written that,
[31:44] there's a third step, not just to make the test pass, but the third step is to actually to refactor the code.
[31:50] We don't only want to make the code work, but we take it like another pass through the code and see,
[31:56] can we do it better? That test-driven methodology can help you do that by yourself.
[32:05] It makes you do the code review yourself. >> That makes sense. If I was doing that type of methodology,
[32:14] it would be like, "Cool, stuff is showing up," and then it would just be random.
[32:21] Anything would show up and then have it say what I wanted to say, "Okay, cool, it's doing that," and then going back and
[32:29] actually making it all work properly. >> Yeah, making sure that you don't do anything unnecessary.
[32:36] For example, put an h1 tag where there's no need for one. >> Okay.
[32:40] >> Basically, make sure that you know what you want, then have your code do that,
[32:48] and then go another time and see, is there a better way of doing it?
[32:51] Is it missing something or is there something extra there? >> Okay.
[32:56] >> Part of that editing process, right? >> Yeah. I've already noticed this,
[33:03] that there's things that I write that I'm blind to. I'm also horribly dyslexic that I am learning to work with it.
[33:13] But how long do you normally give yourself from taking a break from it to going back and reviewing it?
[33:22] >> I would say a lunch break, coffee break, maybe doing another task in between,
[33:30] do somebody else's pull request to review, and then get back to it.
[33:36] I think the important thing is to get your brain out of it so that you have to start from scratch to reorient yourself through the code.
[33:45] >> Got it. Cool. Thank you. Now I'm thinking that I can look at this and review it to you.
[33:54] Let's see. I'm pretty sure this all, I wish this would go away.
[34:00] >> Yes. You can get it to go away if you click there. >> Okay. There we go. Then I can move this over because we need this here.
[34:12] That puts it in the list view. This adds the A. Is it called an href?
[34:23] >> Yeah. href is how it's, I think, referred. >> Okay. Cool. It puts the link to the text.
[34:34] Then we close that out, make a new list.
[34:41] On this one, this one I have on the same line and this one I have on two different lines, doesn't matter?
[34:51] Is there a proper way of doing that? >> For the HTML and the browser, it doesn't matter.
[34:56] For anybody who's reading your code or editing your code, it might matter. It might be easier to read if they are on separate pages.
[35:06] Typically, with HTML where you would put the line break after the closing. You would put the line break before the S. There you go.
[35:19] >> Okay. I can fix that. I honestly don't remember saving it like this,
[35:25] but it definitely could have been because I didn't really know 100 percent what I was doing.
[35:30] >> Yeah. >> I don't want to say that I didn't do that.
[35:34] >> Yeah. Then the other thing is that I would drop the /a to the next line from there then as well,
[35:42] just because it looks better to me that way. I don't know if someone might disagree,
[35:48] but it indents how deep you are in the document object. Then it makes it easier for your eyes.
[35:58] Oftentimes, when you want to write code that's easy to read, you want to make the cognitive load needed
[36:07] for reading the code as little as possible. Because then I can actually focus on what the code is doing
[36:14] instead of trying to figure out how it's doing it. Making sure that this A tag matches the A tag on row 26,
[36:24] for example, will become much easier if they're aligned. >> Now, if I'm keeping going,
[36:30] I don't need this script anymore because we're not running JavaScript.
[36:34] >> That's correct as well. Almost. >> Almost.
[36:39] >> We are doing one thing in the JavaScript file. We are importing the CSS file in the JavaScript.
[36:46] Normally, that would be done for a page like this, it would be done in the HTML.
[36:52] >> Okay. >> But because we are doing in the JavaScript file
[36:56] and maybe we want to build on this, we could leave it here for now.
[37:00] >> Okay. Then this closes us out, body and then HTML. >> Yeah. There is one thing that I would do different,
[37:12] like I would add to this. I think it's not breaking anything.
[37:19] I would wrap the LI elements into a UL element. Basically, above the first LI,
[37:28] I would put a UL and then I would close. After the last LI,
[37:35] I would put a closing tag for the UL. Then maybe it's a good idea to go see what it does,
[37:43] maybe from MDN or? >> It moved everything over to make it prettier.
[37:50] >> Yeah, that's what it does. Actually, the tool that does it is literally called Prettier.
[37:56] >> Oh, yeah. It's like a plug-in for VS Code. >> Yeah. This uses the same thing.
[38:05] >> Yeah. It does make it prettier because it just made it easier to read with the UL.
[38:10] I'm going to highlight the UL. The UL element represents a list of items where
[38:16] the order of the items is not important. That is, where changing the order would
[38:22] not materially change the meaning of the document. >> Yeah. What does the last sentence mean?
[38:32] That raises more questions than it answers. Let's try to figure out.
[38:39] Change that into OL, both that and the closing tag.
[38:45] You, of course, always need that matching closing tag for everything that you do.
[38:50] Now, look at the output. What changed? >> I need to turn off the plug-ins.
[39:03] They get in my way for some stuff and it drives me nuts. Oh, it put the numbers.
[39:10] Oh, hey. >> What does an OL tag then say about itself?
[39:16] >> The OL element represents a list of items where the items have been intentionally ordered
[39:23] such that changing the order would change the meaning of the document.
[39:27] It literally is bullet points versus numbering. >> Exactly. Now, you've given a ranking to these items.
[39:37] Clearly, you have one podcast that you care more about than the others.
[39:40] If you mark it as UL, it's just the list of let's say ingredients in a recipe.
[39:49] Order doesn't matter when you're just listing them what to buy from the store.
[39:54] But you can turn off your Grammarly plug-in from top right of your browser.
[40:00] There you go. I think that if you click somewhere there. >> There we go. No, turn off.
[40:08] I don't want to remove you. >> Is there like a? No,
[40:12] I thought there would be like an option where you could say, oh, there's like websites.
[40:17] I don't know. I don't think we have an option to turn it off with this one.
[40:21] >> No, I've had to turn it on and off when I was trying to. When I was doing it through LinkedIn learning,
[40:31] when VS Code would go live in a browser, I would have to turn them on all my extensions
[40:40] off because console would error out. Learned that the hard way. Lots of Googling.
[40:48] >> Yeah. >> Yeah.
[40:52] >> But we did it. We did it. >> We did it. I think we're at the end of the code review.
[41:00] Maybe we want to change it back to UL if we don't have an ordering for them.
[41:05] So that's probably something that we can change. >> I'll leave it. We'll leave.
[41:11] You don't want to talk about at the top of it. I'm totally okay with that.
[41:15] >> Okay. Yeah. It's good that there's something to still do in the future. Yeah. That's basically our code review.
[41:23] At this point, I'd be like, okay, now it does what our customer wanted,
[41:29] whether it was the product owner or some customer giving us feedback about a feature,
[41:34] or whoever gives us the definition of what needs to be done. At this point, I'd be like, yeah,
[41:40] it looks good to me and let's move this forward. Let's put it to production.
[41:47] Congrats. You passed the code review with some comments. >> Yes. Just thinking about it.
[41:58] I learned that SRC has the majority of the files you want, like the CSS and the index.js.
[42:15] If I want to do color again, I will Google it because I don't remember.
[42:26] Let's see if we can Google this. CSS color, applying color to HTML elements using CSS.
[42:41] Not going to lie, how I normally would do it is just scroll through this to see if I can figure it out.
[42:49] >> Find an example or something that pops out, right? >> Yeah. But I'm like, maybe I should be actually reading this.
[42:56] But it's a lot of text to read just to find one little thing. >> It is. It depends what you're doing,
[43:03] whether you want to read it or not. In the beginning stages,
[43:08] it can be really nice to get just something working quickly, and when you should get more senior and more comfortable with things,
[43:18] you also just want to move fast. You got to know what you want,
[43:21] just give me the exact answer to the question I'm looking for. >> Yeah.
[43:25] >> But especially when something doesn't work or you still need to understand the foundations a little bit better,
[43:32] it's a good idea to read what's offered. But of course, for this and for today,
[43:41] we could just hop in and I can tell you how to do the colors or maybe you can. >> I'm seeing if I can find it.
[43:51] >> What color do you want to change? >> The header.
[43:56] >> The color of the header. The text, right? >> Yeah.
[44:00] >> Honestly, this is a long page. What I would do, I would hit "Command F" and search on that page.
[44:09] I don't think there is a color specifically for a header, but maybe the text color you can change.
[44:20] That might help you. >> This is going to be like me trying to handle different text directions.
[44:31] Nope, we don't need that. Styling text, maybe.
[44:35] Guides, assessments. No, okay, cool.
[44:47] No, those are just fonts to import. We have that already.
[44:57] Not going to lie, this is probably why it's really frustrating to watch my homeworks, like my co-working sessions because I'm staring at it,
[45:07] trying to find it, and people are like, "It's right there in front of you. This is how."
[45:11] >> Yeah. >> I get that.
[45:12] >> It happens. I like watching text streams on Twitch, and it does happen where I watch something,
[45:21] I'm like, "It's right there." It depends on who's streaming.
[45:26] Some people are like, "Please, no backseating. Don't try to tell me how it is."
[45:31] Some people welcome that. That's something that you get to define what's good for you
[45:36] as well as the person running the stream. If you want people to help you out,
[45:42] give you those hints. Of course, I wanted you to look through there
[45:47] instead of giving you the answer in this case as well, even though I was like a observer or like a viewing what you're looking for.
[45:56] >> While we were talking about that, I remembered that it guesses it.
[46:01] If the body is font family sans-serif, maybe header color, nope, no.
[46:13] >> You just want to change the h1 tag color, right? >> Yeah.
[46:20] >> Yeah. For that, you get out of the body and below it, you write h1.
[46:30] What's happening now is you're modifying everything inside the body tag. What you see here on line 1 corresponds to a tag in HTML.
[46:40] Every body tag would get font family sans-serif. >> This is when you do the squiggly lines, the squiggly lines.
[46:48] I've been getting lost on the squiggly lines, what I use them for,
[46:52] but I think a lot of it. Yay. Then I could look up what this text is and change that.
[47:01] >> Hey. I got frustrated at trying to search it, that I just decided to type color and this thing guesses it,
[47:10] which I think is another really cool feature to learn with. Just like, I don't know, I'll try it. Let's see what happens.
[47:16] >> Yeah. Experimenting is one of the best ways to learn coding and technologies anyways.
[47:21] That's how I learned most of the things that I worked with technology. >> Wait, why is it trying to save it? There we go.
[47:28] >> If you hover color, it actually links you to the MDN reference there and you can click on that link as well.
[47:36] That's really cool. Those are called selectors. You have a body selector.
[47:44] You're selecting by the HTML tag right now. But remember how we also had IDs,
[47:51] like we had the div with an ID of app. We could also, I don't have editing rights.
[48:02] Could you add editing rights for me for a moment? I'll show you something with what happens with the IDs.
[48:09] >> There we go. >> If we go to the index.html and we see the paragraph there with,
[48:20] here are some of Jen's favorite podcast. We give it an ID now.
[48:26] The ID is podcasts. We save that and then we go to the style CSS.
[48:34] Now, I'll add another paragraph here to demonstrate something. Welcome to MySpace.
[48:51] Just to demonstrate something. Now we have one P tag with an ID of podcast and one P tag in general.
[49:00] >> Okay. >> Two P tags and I need to find the right page.
[49:05] If we now want to target everything that is a P tag, we could change their background color, for example.
[49:17] See, I even typoed it and it's so smart that it can tell me it's background color.
[49:22] >> Okay. >> We're going to choose a color for here.
[49:28] This sounds good. This I can pronounce, cornflower blue, and we save it.
[49:34] Now we can see where the P tags are. Those are the P tags.
[49:40] However, I actually just wanted to change the one that talks about the podcasts.
[49:48] >> Okay. >> In order to do that,
[49:50] we can also target the ID. Now only one of them is colored.
[49:58] >> Okay. >> That's one of the reasons you would give an ID to an element,
[50:03] because that can be then used as a selector in CSS and JS or JavaScript to find that specific tag within your code.
[50:12] >> Come back. Let me choose a color. You just let me do it.
[50:31] Now you won't let me go. >> I think if you start writing, yeah.
[50:37] >> Here we go. Even though it's second, oh, you just deleted a color and just changed the text weight.
[50:46] If I add a color in there, we'll just make it blue because it does override it.
[50:59] That's cool. >> Yeah. What we see here is a demonstration
[51:05] of the priority of the selectors. Selector with that just targets a tag like P,
[51:17] has a lower priority than a selector that targets something based on an ID.
[51:24] >> That's why I wanted to move it up just to see if it changed it. Even though, seeing if it reads it from top to bottom,
[51:36] or if it reads it by priority. You're saying CSS reads it by priority.
[51:43] >> Yeah. It does have some priority in it. If things are in same priority,
[51:49] they overwrite the previous rule. >> I feel like this is definitely giving me a good grasp.
[51:55] I'm finally starting to see how I can start to build things myself. I get that HTML and CSS are very, very basic.
[52:07] Yet, now that I've also been able to see a little bit of Express and React, I'm like, "Oh, okay.
[52:17] I think maybe in a few more sessions, I'm going to be there that I can actually build something myself."
[52:24] Which is going to be cool. Thank you. >> No problem. Yeah. I wanted to do a little bit like
[52:31] at least a couple more tidbits here at the end of the code review as well, to maybe answer a few things that you might have run
[52:39] into or might have questions about next. Yeah, that was fun.
[52:45] >> It's definitely cool. That was fun. This is definitely something.
[52:49] I think you also really did teach me how to do a code review. Because this was something that I was running into.
[52:58] I think in a lot of them, where I'm still trying to understand the content that's coming at me,
[53:05] that I'm not necessarily reading through everything because I'm just like, "Oh, I need to keep up with someone."
[53:12] Anthony brought this up earlier of like, "You should probably write down your own instructions
[53:19] or read what Terminal is putting out." I'm like, "I don't always know what each of those pieces mean,
[53:25] so I'm just skipping over them, too." >> If you have some time when you do all this,
[53:36] like if you do a session on your free time and things like that, Free Code Camp is a really great resource for beginners.
[53:43] I think they go through some of these beginning stages in a very nice structured way where you do learn,
[53:50] but you also build things along the way. That way, you'll definitely get a hang of all this.
[53:57] I think now might be the right time to go there for HTML and CSS. If you wait too long,
[54:06] the beginning sessions will feel like, "Oh, I already know this," and then you skip over them,
[54:11] and then you might lose something that was an interesting tidbit there that you otherwise wouldn't have run into.
[54:20] That might be something that would support your learning HTML and CSS really fast right now.
[54:26] >> That'd be cool. I remember being very, very stuck in my learning on JavaScript, on LinkedIn learning.
[54:36] I feel like if I restart the learning, I might get a little more or less stuck now.
[54:43] I'm like, "Maybe I should actually finish that one, too." >> That's a good idea as well.
[54:49] Get that one done. But yeah, I really appreciate you coming on the show today and being
[54:55] our first guest, our first returning guest as well. >> That's awesome. Breaking records here.
[55:03] That's amazing. Happy to be here, and I hope to be there,
[55:09] the first one to make it here two times. >> Yes.
[55:13] >> [inaudible] >> Thank you again, Yeri. Talk soon.
[55:16] >> Thank you. Bye. 
