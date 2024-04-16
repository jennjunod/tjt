---
showLink: "https://www.youtube.com/watch?v=UBKlAms2VNQ"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-readme-driven-development-with-anthony-campolo"
title: "Teach Jenn Readme Driven Development with Anthony Campolo"
publishDate: "2022-08-11"
coverImage: "https://i.ytimg.com/vi/UBKlAms2VNQ/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Thank you again for joining Teach Gen Tech.
[00:06] Today we have Anthony on the show, and I think you were the second episode?
[00:12] >> Number two. >> I don't remember. You were number two.
[00:14] Yay. Please introduce yourself and what we're going to be learning about today.
[00:19] >> Hello, everyone. Happy to be back. This was a really fun show to be on the first time,
[00:23] and I've gotten to watch the progression of it over the last. We were just talking about this. You said it was like
[00:29] a month and two weeks, maybe a month and a half about since we started, I think.
[00:35] You've already done a ton of shows like 15, 20, somewhere on there. >> Yeah. I think I'm right around there.
[00:41] >> Yeah. That's a lot. I don't know anyone who usually started streaming just that many,
[00:47] especially doing a show like this. Most people have a slow roll into it.
[00:51] >> No, I was like, full commit, four days a week, we got this.
[00:56] >> Yeah. That's crazy. >> Yeah. Great job at that. You got to meet a lot of my friends,
[01:02] and a lot of people that I don't know also. There's been guests that I had never
[01:06] been aware of or had seen their stuff either. That was awesome. It's cool that you build up a network already.
[01:13] >> Well, and for everybody watching, it was two main people that gave me the courage to start.
[01:22] It was Ramon gave me the idea of peer programming, and then Anthony was like, "Yeah, you should definitely do it.
[01:28] It's a great way of learning." Then I met Yeray, who is Episode 1.
[01:33] "Oh, hey, I'm talking about you, Yeray." I met him on a Wednesday after I met Ramon and Anthony,
[01:42] and he's like, "Cool, let's do it on Friday." I'm like, "All right.
[01:46] Yeah, I'm starting this." >> Cool. Yes, that was five or six weeks ago.
[01:54] It's just so crazy, so thank you for- >> What are the most important things you think you've learned?
[01:59] You had some high level points. >> High level things.
[02:03] I will say, I think that Mischko summed it up the best on, everything is very, very simple.
[02:14] It's repetition and building upon it, that is what makes any of it work.
[02:22] He was talking about how he told his kids this. It's actually really, really great advice in the fact
[02:29] of a lot of this isn't too complicated. It's more of it looks really scary,
[02:36] and then being able to ask people to fill in the gaps, is probably one of the biggest things,
[02:43] and that even over 50 years of knowledge on one of the streams, people may not see the error of not having
[02:53] an S or having an extra S, because these type of things happen to everyone,
[02:58] and I can do it even though I'm dyslexic. I will say that since doing so much more in JavaScript,
[03:08] I can now tell a lot more of the differences between JavaScript and HTML and CSS,
[03:13] where on Episode 1 with Yare, I was like, what are we doing?
[03:20] >> Yeah. >> I tried to do it. Everybody has their own way of doing things.
[03:26] Even though this is a very, very broad, there's so many people in this industry,
[03:31] everybody has their own unique way of doing it, which I'm learning as well.
[03:36] But things are starting to click, repetition is key. >> Yeah, that's been great. You've also got to
[03:41] see different topics build on each other, because you did React with me on our episode,
[03:47] and then later you did a next project. What was that like? Do you feel like that made React easier?
[03:52] Do you feel like it made it more complicated? >> One thing that I would say from comparing to,
[04:02] I took a semester of CSS or something, I took a semester of some coding language,
[04:08] is I've been given very complicated concepts, and then it mostly makes sense,
[04:17] and then seeing it from somebody else's point of view, can confuse it, and then also make it make more sense.
[04:23] In the fact of I learned React with you, then the next JS with a React wrapper for WebPayments,
[04:33] for Square with Bakari, and then having Richard on from Square,
[04:42] he had me do it just the React app, which made what you taught me make more sense,
[04:47] and also distinguishing between Next and React and how the wrapper worked.
[04:54] It builds upon each other, but also the framework still get a little fuzzy.
[05:01] But sometime this month, I'm also going to have my first look at Python,
[05:06] not because I want to learn a ton about Python, I'm not thinking that I want to go that way,
[05:10] but I know nothing about it. How do I know that JavaScript is like my jam?
[05:15] That's funny. But how do I know that that's what I want to do unless I see and understand what other things are?
[05:24] >> Totally. Yeah, if you try out Python, you're going to find that if you want to do web development,
[05:29] you're going to do JavaScript the vast majority of the time. You can do a Python back-end
[05:33] and then have a JavaScript front-end like Django, but most people who are doing Python
[05:38] are doing data science stuff or machine learning or things like that. So it's good to learn other languages at all, for sure.
[05:45] I definitely would encourage you to do that. I would say there's a certain amount of
[05:51] learning one language first before learning a second language. If you try and learn to program while learning multiple languages,
[05:56] that can be really confusing. So that would be the only thing I would be aware of going into that.
[06:02] But the thing you're going to find with JavaScript and Python is actually very similar comparatively to like crazy languages,
[06:08] like functional languages and stuff like that. They're actually pretty much like if you know one,
[06:13] you compare it to the other one pretty dang quickly. >> I just learned about Go last night.
[06:18] >> Yeah, and Go is another one. Learning a second language is great for
[06:22] fleshing out where and when you might use the first language by contrast. Yeah, exactly. You'll know why you would use
[06:27] JavaScript one place and Python for a different place. >> Yeah, and I'm excited about that.
[06:33] I've found that there's also a lot of people that have been a mentor in some type of coding school,
[06:46] and that's where they're getting most excited about coming on the show in the future.
[06:49] I think that's a great way to also see why people love coding camps, and then also the difference of almost like one-on-one tutoring,
[06:59] but yet having other people ask questions too. >> Yeah, that's what makes boot camps hard is that sometimes you'll have
[07:05] one teacher for a class of 20, 40, sometimes 100 students. When I was at Lambert School, we had literally
[07:13] 150 people in some of these classes. It didn't really work out well if you're
[07:17] someone who needed that individual personalized attention, which I think a lot of people do,
[07:21] and it's like education doesn't scale. I've said this before as part of the problems
[07:26] with just mass public education in general. It's an inherently hard thing to do.
[07:31] It's an unsolved problem. If you can figure out a way to get a whole bunch of
[07:36] really experienced people to come in and teach you one-on-one four times a week, it's so smart.
[07:42] >> I will say that one of the biggest things I've learned, and one of the bigger reasons I'm excited about today,
[07:51] but thank you for helping being part of the beginning. One of the things that you said to me was about consistency.
[07:59] That's why I was like, "Okay, cool. I'm just going to do it these four days a week and at this time."
[08:05] Somebody can't make it, well, I'll just either not do a show that day or do a co-working session.
[08:11] But it was also the fact that building this content very slowly. Doing video is very, very second nature to me.
[08:19] I'm like, "Cool, I can do it non-stop, whatever, no problem."
[08:23] Writing blogs is harder for me, but I know it's something that I want to level up on.
[08:29] I'm like, "Cool, I can start doing that." Then also being able to start contributing to
[08:34] open-source and showing a portfolio on Git. >> You're also a speaker on Twitter Spaces in your podcast.
[08:40] >> Oh, yeah, I thought too. Yeah, I do that. >> Look at that.
[08:44] >> Ben said, "Yeah, boot camps and education in general is
[08:51] severely limited by both the experience and the priorities of the teachers. If, for instance, the teachers find testing complex,
[08:59] they're less likely to have material on testing. Problem is, that reinforces that testing or whatever is hard or less critical."
[09:07] >> Yes, this is the thing I do. >> A hundred percent.
[09:10] >> Ben's calling me out and he's totally right about it because I do not write many tests in my example apps.
[09:15] That is always the thing that you should bring out someone to teach you just testing for sure.
[09:19] That's very important. >> That, I am looking forward to.
[09:23] I feel like maybe Postman would be good at that. >> Well, there's a difference between writing tests and testing something.
[09:31] This is part of the confusion is that writing a test is writing a program to basically run your program and feed it
[09:38] different inputs to see if the inputs are what you think they should be. That involves writing code to do that.
[09:45] Whereas having a tool like Postman, you're hitting an API,
[09:48] doing a thing and seeing what comes back. It's like testing, but it's slightly different because one's like
[09:55] an automated thing and one's like a person running through a certain flow. Usually, you have to try and write tests that are going to be able to
[10:02] test the logic in your program and then hopefully, some end-to-end testing to test the whole thing together.
[10:08] Then you actually have to go through the program yourself and the steps of what it's going to do and verify.
[10:12] It's like what I was talking about with the shopping cart thing, you had to do with Square.
[10:16] You had to go through this whole flow to make this purchase. Along the way, there'd be all those different steps you want to write tests for,
[10:23] and then you still, at the end of the day, have to actually walk through the thing to make sure it works,
[10:27] even if all your tests pass, something might break that you didn't write a test to account for.
[10:30] Testing is really complicated. This is why I leave it out of my tutorials. I think it deserves its own material that's separate from mine.
[10:36] But it's complicated. >> Good to know. I will add that on my list of things
[10:42] to learn because I think that and protocols and there's so much out there. Even as Ben, when he was on the show,
[10:51] said that accessibility, it's such a wide net too.
[10:56] Yes, Ben has made that complete before, that there's a lack of accessibility in education,
[11:04] in boot camps instead of testing. It's definitely a structural problem.
[11:09] I agree, that is a big reason that I failed high school, and also went to way too many colleges.
[11:21] >> By the way, Ben is giving you a very hot tip right here. >> Yes. Please put me in touch.
[11:26] I love. >> Should I flash on the screen so?
[11:29] >> Okay. >> I don't know if you can see that.
[11:31] >> There we go. >> She's a test boss for sure.
[11:36] >> Yeah. That's definitely the person you should get in touch with. >> Yes.
[11:40] >> Don't worry, Ben. I think you're specifically calling me out. I think you accidentally called me out.
[11:43] Don't worry. Because there's certain things that there's always things we know we can improve on. It's like I know that my education,
[11:53] which doesn't have enough stuff about testing and that's why. It's like at least I know that because then I can hopefully one day fix that.
[12:00] There's so many things to do, but you can't really do it all at once.
[12:03] So it's like chipping away piece by piece of like, what is the next thing I can get better at and improve my whole overall deal.
[12:09] >> I am curious about this before we dive into the read me stuff. I learned about the three C's in Debra of community, content, or coding.
[12:22] Normally, people are really good at one or two of them. >> The third one should be product, not coding.
[12:27] I think coding doesn't really quite make that distinction very clear because it's about, there's the community part,
[12:34] there's the content part, that is actually like the thing itself that is
[12:37] like the community is around and the content is created about. I guess whatever the company is actually selling usually are
[12:42] the open-source projects that's actually being done. So coding, because you're still coding when you're doing content stuff,
[12:50] because you're coding projects usually with the products, but you're not like writing the code of the product itself. Does that make sense?
[12:57] Yeah. So I think that's a clear distinction. But I get that three part thing like you're on the money with that.
[13:04] I just think that there's kind of a tweak in that. >> We'll say coding and product because then it still equals three C's.
[13:12] >> Yeah. So if you go to whatisdevrel.com, have you seen this site? >> Yes. There is so much goodness out there.
[13:21] >> Yeah. Because those who do community, content, products and many people have already made this distinction before.
[13:27] So they didn't really invent it, but I think have distilled it in the most explainable way.
[13:34] So that's usually the one that I recommend people check out. >> I think that's something that I've learned
[13:40] is anyone going into the role, I'm a lot better at the community and the content,
[13:49] yet coding or product, however you want to say it, is something that I need to level up on.
[13:55] That's I think the beauty of just learning in general is realizing what you're good at, and then going, "Cool, I can level up on that."
[14:04] Even though that may never be my strong part of my skill set, I can at least be really good at it,
[14:10] maybe not as good as other things. So I think that's really cool talking about the testing there too.
[14:16] So what are we learning today? >> Yeah. So today what we're going to be learning is I want to talk a little bit
[14:22] about documentation and why it's useful or important and a way to get into your workloads hopefully as painless as possible.
[14:32] You actually said you're getting a team on to talk about documentation, and it used to be called Divio,
[14:37] but they just rebranded. I didn't actually know this. What are they called?
[14:41] >> Oh, I don't know. I have it bookmarked. Hold on. >> Yeah. So what this is,
[14:45] there's going to be another follow-up episode of that. I'm definitely going to be X. It's going to be super interesting.
[14:50] They have a theory of docs where they basically break down the four different categories that documentation can be.
[14:58] Yeah, this is the one. So scroll down a little bit to that right there. So you have tutorials which are about walking you
[15:06] through end-to-end experience that hopefully will teach you generally how a thing works.
[15:12] Whereas a how-to guide is something where it's giving you something specific to do that you can accomplish and that you want to do,
[15:19] that is like a self-contained task. Then reference would be just like you'd be like a glossary,
[15:25] like just a list of terms and definitions and stuff like that. Then explanation is just someone actually writing out words to explain a concept,
[15:34] whether that's again a term or something you need to just get about programming or whatever you're documenting.
[15:41] So I find this is a really, really good breakdown of the different things that you need in a whole docs,
[15:48] like a doc website. But this is not what we're going to be doing today.
[15:51] This is how to structure a larger docs project. Whereas I want to show you just what do you need for one single useful read-me.
[15:58] How do you write a read-me that will get you from zero to one in the course of that read-me.
[16:05] This is useful because it will allow you to build a project again or share it with other people who want to know how you built a thing.
[16:13] So I'm just going to walk you through the first thing we did, the first project we did, but we're going to write it out first in actual Markdown.
[16:20] >> Okay. Where do I need to go? Because you told me that we were going to use a tool and I don't remember where.
[16:27] >> We should talk about Markdown a little bit. You said you have some experience with Markdown.
[16:31] >> Yes. >> So how would you explain Markdown?
[16:35] >> How would I explain it? That is, wait, wrong buttons.
[16:40] Wrong buttons. There we go. See if I can get the live stream going right.
[16:45] I don't know if I have a good way of explaining it other than, is Markdown part of HTML?
[16:55] >> That's a good question. That's the key question you need to ask.
[16:59] What Markdown is, is it's a lightweight syntax to write something that will be transformed into HTML.
[17:08] So what you're writing is you're creating headers and you're creating text and then there's links and there's bullet points,
[17:16] or bolded text, or sections, or anything, or tables,
[17:20] and all that eventually ends up as a website in HTML. But writing HTML, as you can see,
[17:27] you have opening and closing tags and then they all have their own tag names, and it's a lot to write if you actually write that just quickly while you're thinking of it.
[17:37] So Markdown was invented as a more human-friendly way to write this, basically, and Markdown is old,
[17:44] Markdown is decades old. It's just constantly had different variations that
[17:48] people had their own specific versions of, and now we're getting to a point where it's getting to be more standardized because of
[17:54] things like GitHub and websites like HashNode and Dev2, and there's all these places now where you can write Markdown.
[18:00] You can write Markdown in Notion, you can write Markdown in Discord,
[18:03] and it's really pretty awesome that it's gotten to be such a widespread tool. Once you learn it, you can write structured documents very,
[18:14] very quickly because you can create the headers and the skeleton outline of it very easily, and then fill in the blanks from there.
[18:23] So I usually will start out, if I'm writing an article for Prismic,
[18:28] they have you first write an outline, and so I can write an outline,
[18:31] and then that outline becomes like the headers of the blog post. >> Really quick for anybody that's super,
[18:40] super new to Markdown and wondering what we're talking about. >> Yeah, at this point, we should just start writing stuff.
[18:46] >> I just Googled it. So that way, because I'm pretty sure it's actually
[18:50] this cheat sheet really shows what they all are. So that way, if you're like-
[18:57] >> Yeah. So stop on the first, just the first part. So just this right here is going to be
[19:02] the vast majority of what you're going to do. When you're writing Markdown, you're going to have headings,
[19:07] then you're going to have the ability to make bolder italics, and then you can do quotes,
[19:11] which just makes it offset a little bit on the screen. Then you have numbers for lists and bullet points for unordered lists,
[19:19] and then you have backticks to make code look like codes. That's when you see a word from
[19:24] code written in documentation or a file name, and that looks different from the other text,
[19:29] that's what's happening there, and then links and images.
[19:34] >> Sweet. >> With the extended syntax.
[19:38] I want to see if we're going to do any of this. So tables are occasionally useful.
[19:43] They don't always look good on mobile, which is part of the problem,
[19:46] but they are really good for if you're on a desktop, which is if you're coding something,
[19:51] that's frequently the way it's going to be. But you don't always want to have a really,
[19:57] really, really long table because it may go totally off the screen. >> Okay.
[20:01] >> But most of this other stuff, we won't really need to go over today.
[20:07] >> Okay. >> But you were talking about how you were using Markdown,
[20:11] that was like Spotlight's Markdown? >> Yeah, Spotlight's Markdown.
[20:15] Just as one thing, I feel like we definitely need to look at the emoji one just because I live by emojis, that is how.
[20:24] >> So the cool thing about what we're going to do is that you'll be able to just put it in an emoji normally and
[20:29] then GitHub will figure out how to turn that into Markdown for you, I'm pretty sure. >> Sweet. Okay, cool.
[20:36] Where am I going now? >> So you're going to gist.github.com.
[20:41] You'll need to be logged into your GitHub account. >> Just like this?
[20:45] >> With a G, like GitHub. >> Yeah.
[20:48] >> Yeah, there we go. Hey, I'm still logged in, thank goodness.
[20:59] >> All righty, cool. This is a gist. Now, this isn't necessarily the nicest way to write Markdown,
[21:07] or write anything really. Your code editor is usually going to be the best place to do that,
[21:11] but for the sake of what's happening here, I want to at least make sure you've done this once,
[21:14] so you can write another gist if you ever need to. Sometimes what I'll do is I'll write something in,
[21:20] like just a file on my computer in my editor, and then I'll eventually just copy-paste the whole thing back into gist,
[21:25] so I can look at what it'll actually look like. But this way we can get
[21:28] some iterations with just actually using the GitHub gist itself. This is a really easy way of both quickly writing something down and saving it,
[21:36] then also having a link you can share with someone. So if you want to write a couple of steps out,
[21:40] you need someone else to help you test or debug, you do that in a gist, you just send them a gist link,
[21:45] then they'll be able to see it and just work with it. You put code samples in there, you can do anything.
[21:49] >> Okay. >> So what we're going to do is there's first a gist description.
[21:57] So we're going to give this a name, and we're going to say,
[22:01] what was the name of the episode? Deploy React to Vercel with Vite.
[22:11] >> What did we call it? I don't remember. You just said it, but I was like.
[22:15] >> Yeah, I was going to say Deploy React, and then get rid of that to Vercel with Vite.
[22:24] Then on the filename, where it says filename including extension,
[22:30] so here you got to make sure. So this is because you can just make this just like a JavaScript file,
[22:34] this could be anything, but if you make it a markdown file, then it will make it look like a markdown thing.
[22:39] So do index.md, that's what I call all of mine. You can give them a name if you want,
[22:45] but I prefer just having a name as the title and then the files just index.md. >> I feel like you're setting it up that I can't
[22:52] put like Anthony is cool or anything like that, like everybody else gets a really cool file name.
[22:57] But all right, you'll be the one that doesn't get one, whatever. >> If you want to, I don't know if it really matters.
[23:04] >> It does. >> Then are they dashes and they're always dashes.
[23:13] >> Dashes, yeah. >> Here we go. I haven't used cool yet, I don't think so.
[23:19] >> All right. Now, so this is the beginning of our page. So you can think of it like HTML where you're going to need an h1.
[23:27] So we'll start by creating h1. So that's going to be just a single hashtag or dollar sign.
[23:33] Then space, and then make it just the title that you call the thing. So deploy React or something,
[23:40] you can just copy and paste that. >> This one?
[23:44] >> Yeah. All right, and then hit two spaces. That's all right, I didn't mean that. Backup and then two,
[23:54] and then hit two enters, I mean, yeah. There we go. So it's fun, mouth coding.
[23:59] >> It's been a challenge for everybody, I dig it. I'm learning a lot easier.
[24:03] >> Yeah. So just write out a little description of what you are doing here. I will let you do this one instead of telling you what to write,
[24:11] because technically you've done this. So see if you can just give a one or two sentence description
[24:16] of what this is and what it does. >> I think the part that I'm getting stuck on is what we did with Vite,
[24:35] is what I don't remember. >> You don't really have to describe what Vite does.
[24:40] The most important thing is that you're just saying that Vite is what you're using with React.
[24:44] That's the more important thing. It's not really that you have to explain what Vite does so much is that people,
[24:51] what they need to know is that this is using the Vite template and it's not using Create React app.
[24:55] So the last time we used React, just the other episode or two ago,
[24:59] they had to use Create React app, and that's what generated the React app.
[25:04] You wrote Create React app and then it created your React app for you. Whereas what we did is we used Vite to do the same thing,
[25:09] to create a React app for us. >> Okay. That makes more sense.
[25:12] That's where I think I was getting really lost. So thank you. >> Yeah. It's pretty good.
[25:35] It's not translating it via Vercel, it's deploying via Vercel.
[25:41] >> Yay. >> So how does that use Vite to create React app,
[25:50] then deploy via Vercel. All right. That's great. That's perfect.
[25:58] So now, let's just first look at this. We can see what we've done and what it looks like.
[26:03] So scroll down a little bit to where it says, Create Zero Gist and click the little drop-down arrow,
[26:09] and say, Create Public Gist. Yeah. Then create that.
[26:15] All right. Great. So there you go. So you notice how the H1 is a lot bigger than the text, right?
[26:21] So that's the markdown in action. It's taking that markdown and it's actually rendering the markdown for you.
[26:26] So that's pretty great. The real thing you want is you want the ability to have your editor,
[26:31] and what your markdown is rendering on-screen at the same time. So there's all these markdown coding things like HedgeDoc is a big one.
[26:40] So there's lots of ways to do this. VS Code itself can actually do
[26:44] a split-screen thing where you can see the two side-by-side. So now that we've done this,
[26:52] we're going to come back to this, but we should really do this through an editor.
[26:55] Let's go and open your Visual Studio Code. You're in a project,
[27:02] so you should get out of that and open a fresh project. >> Just a new file, right?
[27:18] >> Yeah. >> Built-in. Sure.
[27:23] >> Cool. So now just go back and copy-paste what you already have from the first gist.
[27:28] So click "Edit" or actually click "Raw". Let me show you this. So if you click "Raw",
[27:33] then you can see it just the markdown, and then you can just grab that right there.
[27:39] >> Select language or opening different editor. >> Don't worry about that. So just paste it and then save this.
[27:50] I'm going to call it the same file name you called the gist. >> Okay. It's weird doing it through this way.
[28:02] >> Yeah, we could have done it through the terminal. It's all the same at the end of the day.
[28:08] >> Yeah. I've gotten used to doing it through the terminal. No. I need to make you a folder.
[28:14] >> Okay, great. So we're just doing this. Actually, this is going to be important.
[28:26] We need to name this file readme in all caps.md. >> Okay. Well, I hit "Enter".
[28:36] Where did it go? >> It's in Baraka's Dope.
[28:49] >> Damn it. Okay, there we go. >> You want to name this one readme?
[28:57] >> Yeah, allcaps.md. Yeah, that is because if you do that,
[29:05] when we put this repo up on GitHub, then it will display the readme on the front page.
[29:13] That's why when you go see projects and they have that readme, you can just see it if you scroll down on their repo.
[29:18] That's because they wrote a markdown file that's called readme.md. >> Okay. That makes sense. Very cool.
[29:24] >> All right. >> All right. So you should quit as a reopening.
[29:29] She says that slash through on top. It's confused because you moved it around.
[29:33] >> Yeah. So I'm just curious if this is going to open. Because I haven't done it like this.
[29:39] Did. Yay. >> That's a different. That's brackets.
[29:45] >> I didn't even know. >> This is part of the problem is that when you double-click something,
[29:49] it just opens the default app. So your default app for dot markdown files was set to that program.
[29:54] Instead of VSCode. So yeah. So what is brackets? Is that another editor?
[29:58] >> Yeah. I probably downloaded it at some point. Apparently, I did because it's there,
[30:04] but I don't know why I have brackets. >> I've never heard of brackets.
[30:07] It's a source code editor focused on web development created by Adobe. Interesting.
[30:15] >> I actually haven't heard it be used in the community. I've only heard of VSCode.
[30:21] >> No. Literally, 99 percent of people you're going to meet use VSCode, and then one percent of people use WebStorm,
[30:27] and we'll talk very, very long about why you should use WebStorm and not VSCode,
[30:34] but almost everyone uses VSCode at this point. >> All right. So I got my read me going.
[30:40] Open folder. Fine. Open folder. WebStorm. Good folder. There.
[30:51] >> Cool. >> It seems happier now.
[30:54] >> Okay. Here we go. Now, let's add a H2 and then a space.
[31:05] So the first step is going to be create React app. Some people will do title like that,
[31:18] and I think that's what we should do here. Some people will write out a phrase or sentence
[31:24] that is then just only capitalize the beginning. So what you're doing with headers may shift a bit
[31:30] depending on whether you're writing a blog post or writing an outline for documentation.
[31:35] So keep that in mind, but there's going to be different ways to do this.
[31:39] There's no necessarily right or wrong way. This could be longer,
[31:43] shorter, it's whatever it's going to. What I think is important here is that people
[31:47] first start by writing something that makes sense to them, and then they can worry about if there's a way they can
[31:53] refine that to make it more understandable to everyone, then that's good. But the first thing you should do is make sure it actually makes sense to you,
[31:59] because it's most important that you'll be able to read it back and do the steps again and understand it.
[32:05] If you do that, I find usually that then means most other people can understand it as a knock-on effect of that.
[32:12] If you're able to write it clearly enough to make sense to yourself, then as long as you can write it in an orderly way,
[32:18] then people can follow along with the thought process. Does that make sense?
[32:22] Yes. I'm going to be probably way more detailed on it just so that way, if I'm going back to day episode 2 when I had no idea what we were doing,
[32:35] that version of me would understand what I was doing. Yeah. That's when you get into eventually writing a blog post.
[32:43] That's where once you have explained it to that extent, and anyone from 0-1 can understand it based on just what you've written,
[32:51] that's when you've written a really good blog post. That's why writing to your previous self is a good way to do that.
[32:55] [inaudible] I definitely didn't even,
[33:03] I think it was actually the day from talking to you, I did control plus C equals to stop terminal,
[33:11] but it just stops the server running for localhost, and then CD to change directory because I was like,
[33:17] I know these things, but I couldn't remember them. Yes. I got my React app, create React app.
[33:25] Then make two more lines, and then go ahead and write a little description of the first step of this.
[33:32] I'll say what I'll write here. I would say generate boilerplate.
[33:40] Boilerplate would be one word, I think. Then React app.
[33:51] Actually, sorry. Generate boilerplate, application using the React Vite template.
[34:06] Then period. Cool. That'll be good for now. Now, we're going to actually put the command that does this.
[34:17] We're going to start with, this is the important part. This is where you're going to be doing code stuff.
[34:23] The code stuff is what's most important. Everything we're doing here is about the commands and the code,
[34:27] because you want to actually be able to use this document. You want the code to work. That's really important.
[34:33] You're going to do three backticks. That's not the right backtick.
[34:38] Yes. This is the one next to the number one on your keyboard. Yeah. Great. You can do it where you just have the three backticks,
[34:45] but what's better to do in the vast majority of cases is to then say what kind of code is this.
[34:52] You'd write JavaScript or Python or any of those languages, but we're not writing JavaScript yet,
[34:58] because the first thing we're writing is the command to generate it. We're going to write bash.
[35:03] Yeah, this is a bash command. Some people write shell or SH,
[35:08] and it probably depends on what the platform that you're going to be putting this markdown on expects you to write.
[35:14] I find this works in the most cases, but there's some weird subtleties to this,
[35:18] but this is all information that's not super important right now. Good to know though.
[35:23] Create a space. Sorry, not space. Do it again. Do a return line.
[35:29] Now write yarn space, create space, and then create.
[35:41] Sorry. I need to make sure I'm doing this right. Let me go to the beat. Actually, go to the beat JS documentation.
[35:47] I would show you. If I was doing this in the scratch, I had no idea what I was doing.
[35:50] This is how I do this, so go to beatjs.com, and pull this up on screen so people can see it.
[35:57] Yeah, I will. I'm grabbing it. It's loading, because I would also,
[36:05] yes, beatjs.org, beatjs.dev. That's the one. Google is usually the best way to find my stuff like that,
[36:18] and then go to Get Started. Then scroll down, just keep scrolling,
[36:27] keep scrolling, keep scrolling. Yes. You want the one with the React template,
[36:36] so you don't want those first three. You want a little bit down.
[36:39] You want yarn create beat. The yarn one, so grab that whole thing.
[36:45] Actually, copy-paste the one that says yarn. Only the one that says yarn.
[36:50] >> Oh, sorry. >> Yeah. Adjust that line, that's all you need.
[36:55] >> Interesting. I don't know what Grammarly was trying to tell me. >> Then delete all that. There's a couple things you need to change here,
[37:03] because what this is doing is this is not what we did. This is creating a view app,
[37:06] so where it says view, change that to React. Then where it says template view, change that to React.
[37:14] Then on the line below that, do three more backticks, and then save.
[37:24] This is why I call this readme-driven development. This is technically not the exact term being used correctly,
[37:32] because that meant more so you're building a whole library of APIs and stuff. You'd write it and explain it to how you're eventually going to code it,
[37:39] and then you'd code it to make the thing make sense. But the way I'm doing this, I'm just walking
[37:44] through a series of steps that you get first write down and then do. Once you've done that, then any step you're doing,
[37:51] you already know is written down. That means then once you've done it correctly,
[37:55] the way it was written down was done correctly, and you can go back to that example and do it.
[37:59] You know it's going to work consistently the way it did last time. >> I'm making this as a note.
[38:11] >> So if you want to write a note to yourself, you should not make it a two-header thing.
[38:23] >> Well, I'm thinking for somebody that's brand new. For a brand, brand new,
[38:29] reminding them of, "Hey, if you're using Terminal,
[38:33] make sure you're putting it in your code folder," for example. Like those type of things.
[38:38] >> So that is something where they, if you, yeah, I mean. >> If I'm making this for me,
[38:49] the one that went through on day two, like episode two, I would need that.
[38:55] If it's for me when I- >> Well, if they don't know what that means,
[38:58] a proper code folder, would they like, that hasn't even been explained to them.
[39:01] You have to explain what it means to just open anything to do anything. >> Yeah. I'm putting it there,
[39:09] so that way I remember to go back and fill it out. Not that I need to fill it out right now.
[39:14] >> I would be curious how you're going to explain that, but go for it. >> I will show you after today.
[39:19] >> Sweet. Yeah, that's a good point. So for me, I also will include,
[39:25] if we weren't creating this app, it would be like creating a blank directory or something,
[39:29] but then you have the CD command to actually get into it and start doing it. That's a step a lot of people skip.
[39:36] For me, it's like the steps that if you skip them, will people be able to fill in the blanks?
[39:44] Those usually you should assume, no, they're not going to be able to fill in the blanks.
[39:47] You should put that in there. So that's probably a question like experience level and what you need to put in.
[39:54] But for the most part, being more explicit is good. So that's fine if you're trying to explain that because like I said,
[39:59] being more explicit is always good. >> Yeah, that one is just to remind me to go in and make it more explanatory as I go.
[40:07] >> For me actually, my code folder is just the first thing that happens when I open my terminal.
[40:13] I just have that be my code folder. So every time I just open my terminal,
[40:17] I can just start going and then I have a bunch of projects in there, and I just periodically go through and just clean them out.
[40:22] >> That's cool. >> Because I don't like having code projects on my computer.
[40:28] I like for the most part to have all the stuff I've done just be on GitHub repos for most part. So my work is always being saved.
[40:36] I don't have a ton of work just on my computer that could disappear or that other people can't see.
[40:41] So that's why I'll usually have a project, I'll create, I'll work with it for a little bit.
[40:44] Eventually, it'll end up on a GitHub repo in like a day or two, and then I delete it off my computer.
[40:48] So if I want to work with it again, I'll clone it down again,
[40:51] and then do the things I need to do, then push the changes back up and then delete off my computer.
[40:55] >> Interesting. >> For me, it helps keep sanity in both my brain and
[41:00] my computer to allow me to have this all compartmentalized. So I'm not having these long-term projects with lots of work
[41:06] accumulating that isn't always being easily shareable, or documentable, or something like that,
[41:11] because you get much more aware of that once your entire life's work, it becomes like digital artifacts.
[41:16] >> Yeah, and Ben just said, read me as expect folks can fill in the blanks,
[41:25] can be such an obstacle. >> Yeah, and this is why getting into this process,
[41:29] now writing these out and testing them yourself, and going through and make sure,
[41:33] writing a thing out, you can go to it a month later, and then try it and see if it still works, or if you miss steps.
[41:39] That's where usually you'll find the steps you missed the first time, and then you'll refine it and make it a little bit better.
[41:43] These are things you can iterate on over time, and constantly improve and be better and better.
[41:47] >> I feel like you just volunteered yourself to come on the show again, like the end of September,
[41:53] to see if we can actually do this based on it. >> Yeah, and what I'm showing you here, this is my exact process.
[41:59] This is how I build everything that I build. >> Very cool.
[42:03] >> So run this command now, like copy and paste and run this exact command.
[42:06] >> That's actually what made me think that I have to change my folder. >> This is also why you shouldn't have your code folder on your desktop.
[42:17] You should have it in your home directory, so when you open the terminal,
[42:21] you would just do CD into code folder. You should also make code folder all lowercase,
[42:26] that way you're not always having to capitalize every time you type it out. >> Oh, my goodness.
[42:32] >> Just saying. >> You're also making me forget what I was doing.
[42:41] >> I think that's a big reason why I would want to put all of these steps in there. >> But this is specific to you.
[42:48] >> Right. >> This is only because you have to go through those steps.
[42:50] That's why if you have a code folder at all, none of those steps would have needed to be done.
[42:55] So this is specific to your set that requires doing this, that other people wouldn't necessarily have to do.
[43:00] >> Right. But I guess something that I'm wondering, and I'll look around afterwards,
[43:08] is if there's a way or something that people say for super noobs on their read me. >> Super noobs need to watch a video of someone doing it.
[43:18] Some of the stuff you just can't really explain it in words because there's too much context associated with it,
[43:22] because you don't even know what kind of editor they're using. You don't know any of that kind of stuff.
[43:26] >> Okay. So running it. Well, it's been run.
[43:32] >> Great. So now go back to your markdown file. Within those same three black text, create another line.
[43:43] Yeah, and then do cd into my React app. So you need to write out exactly the same.
[43:54] >> Like what it's called? >> So the way it was created the first time.
[43:58] No, no. So see how the first time you already created the name. Yeah, there you go. Yeah,
[44:05] and then run that command in your terminal. Then I will usually write both of those out.
[44:15] Like if I was having to do each one, one by one. Then now you're going to do yarn,
[44:20] just the word yarn, and then space. Sorry, not space, back up line.
[44:28] Then yarn space dev, and then run those two commands. Awesome. Now what I would do at this point is I would create
[44:52] a link in my markdown file to what the local host is going to be. So if you are following along,
[44:57] you'd be able to just click it and it would instantly open. So copy that. Yeah, you got it.
[45:02] Then we're going to do another line. So not in the code box.
[45:08] >> Yeah, okay. >> Yeah. So at this point, we're going to be writing text again.
[45:12] So create one more line and say, open in, and then two brackets.
[45:21] So open bracket, close bracket. So thus the square brackets.
[45:28] Yeah, there you go. Then paste that, and then go one to the right,
[45:37] and then add parentheses, and then copy again, or paste again, I mean.
[45:46] Yeah. So what I would do here, just distinguish these two for myself.
[45:50] In the first half, I would delete HTTP colon forward slash, forward slash.
[45:56] Yeah, delete all of that, and then delete the final closing slash also after 5173.
[46:04] Yeah. So what's happening here is there's the link, which is the part in the parentheses,
[46:08] and then there's what shows the text for the link. So we can have that say anything we wanted,
[46:14] but we want it to also be like descriptive. So someone reading it knows what it is and they click it,
[46:18] and then just put a, so this is the point where you could explain this however you want.
[46:22] You can say open, or actually, get rid of the in, now I realize.
[46:26] Just have it say, open local host in your browser of choice. >> Browser.
[46:38] >> Cool. That works too. Then period. Great. Now, let's actually open this in that local host.
[46:50] There you go. >> Yay.
[46:57] >> Yeah. So if you're doing a blog post or something, what I would usually do at this point,
[47:01] and we don't need to do this, I would take a screenshot, and then actually have an image also as well.
[47:06] Because I want someone who is reading the blog post, or following along to be able to visually see what's actually happening.
[47:13] But this is not really, right now we're not creating a blog post,
[47:16] we just want to walk you through creating a simple series of steps, so we can flesh out more as you want.
[47:22] So let's not do that right now. >> Okay.
[47:24] >> Go out, click out of that. Actually, no. Sorry, I'll click out of that.
[47:28] Let's make that only part of your screen. So make that like, scoot way over.
[47:33] Yeah. Now, go to where your project is. Okay. So the way we did that,
[47:41] actually, so save first. Yeah. So open up your,
[47:46] so you can see the files again. Yeah. So we did this actually a little bit wrong right now.
[47:52] We have the README is not inside our folders, just drag the README into that folder.
[47:58] Yeah. There you go. >> Don't get angry at me again. Okay. Thank you.
[48:03] >> Cool. Sweet. Okay. That is all good. Now, let's go to your SRC folder.
[48:10] Then app.jsx. Then do what we did last time,
[48:16] where we get rid of the state and a bunch of other stuff. So let's start by deleting line 6.
[48:25] >> Is it line 6 down or just line 6? >> Line 6 and 7.
[48:31] Yeah. Then delete line 1. Yeah. Then scroll down a little bit.
[48:45] Okay. Scroll up a little bit. So I can see all the big chunk.
[48:50] Okay. So let's delete line 16, actually 17 to 23.
[49:00] Do that first. Did I do that right?
[49:09] Then delete that div too. Okay. Then now let's just give it our own h1.
[49:21] So give it the h1 is actually that you give the h1 of the README. So you just copy and paste it from the README if you want.
[49:33] >> It's what I'm doing. >> I mean, you should because this is also the thing is you want consistency here.
[49:38] So the more you can copy and paste stuff, the less likely something is to change or break or anything like that.
[49:44] So you should embrace copy-pasting. It's a good thing. >> I've been learning. I've been learning too.
[49:51] >> Just grab exactly what's in the h1 deploy, react to Vercel with feet,
[49:56] and just copy and paste that without the hashtag in front. Then take the description you had and you can make that the p tag.
[50:11] You have an extra space on that line, which is not important but bugs me anyway.
[50:17] On line 3, there's an extra space. If you go over to the very end of the line,
[50:22] just wrap around. So yeah, there you go. >> Awesome.
[50:40] Then do two spaces so it's indented correctly. So two spaces before use.
[50:44] Great. Now save. Then that all looks good.
[50:50] Great. Let's grab all of the code in the app.jsx file. So copy it all and then go back to the readme,
[51:00] and then go to make some new lines. This time we're going to do, go back one line.
[51:08] We're going to do three backticks, and we're not going to write JavaScript.
[51:14] The reason why is because if you look at the file is not.js, it's going to be jsx,
[51:20] and don't put a space there. Get rid of that. Don't put a space at the end or at the beginning of jsx.
[51:29] Then space, sorry, line. This is not something everyone does,
[51:39] but I think this is a really good habit to be in. I like to write a comment at the top of all of my code box that tells you,
[51:45] what is the specific directory in this project that contains this code example.
[51:51] I'll show you what I mean by that. Write two forward slashes,
[51:56] and then go space, and then you're going to write src,
[52:02] all in lowercase, and forward slash, and then capital A, and then pp,
[52:12] so app.jsx. So that is the file that this code is in.
[52:19] Now, I don't put my-react-app and then the src, because you can assume that everyone has their own project with their own name,
[52:28] and what you want to tell them is just where it is in the project itself. So in the project itself,
[52:33] you have the src folder, and you have the app.jsx.
[52:36] So that's where I had you first go to do this. So they need to know if you're going to show a block of code,
[52:41] where is that code? So that's why this will ensure that even if you haven't explained it,
[52:46] somewhere in the text, they can just look at the code blocks itself,
[52:50] and get some understanding of what's actually happening in that code. So this is something that I've seen some docs do,
[52:55] and a lot of docs not. I think every doc should do this,
[52:57] and it makes a really big difference. >> Okay. Then paste in the rest of it.
[53:03] >> Then do one more space. As a stylist, I think some people will not put in a line,
[53:08] or line break, it's only like five times. >> Line break, got it.
[53:12] >> Then copy-paste it, and then do three backticks.
[53:18] There you go. Cool. So the idea being with that is,
[53:23] if you were walking through this again, I will show code blocks when things change usually.
[53:30] So if I need to change something, I'll have a code block.
[53:33] So I'll know that as I'm following along with instructions, I'll first generate a project,
[53:37] I'll do some commands. Now they're showing me code blocks,
[53:39] it means I need to go into my project, look at the code blocks,
[53:42] and get that into the thing we're going to use to get into to make the change happen.
[53:45] So does that all make sense? >> It does.
[53:49] >> Cool. >> I think it's going to take practice of then reading them.
[53:53] >> Yeah, no, totally. Everyone does it differently. Like the way I'm showing you right now is,
[53:57] not always giving the same way other people do it, but I find this usually works
[54:02] pretty well in terms of giving something that is at least reproducible. That's the most important thing to me because
[54:07] someone could follow off these steps and not really know how to code and still do all things as long as they know baseline stuff,
[54:13] like how to open a terminal and how to do stuff like that. So now we have this.
[54:18] That's all we did in the video. So that's all we've done to create this application.
[54:24] The next thing is you'll be deploying it. >> Okay. That's when we went to Vercel, right?
[54:31] >> So yes, I'm going to try something actually. Let's do this.
[54:36] So first, go back to our readme and do two spaces. Let's just get our markdown good first,
[54:42] and they're going to do another h2, which is going to be deploy to Vercel.
[54:47] Then go down to two lines. So I'm going to try and have you do this with the CLI this time.
[55:02] So this is where if I had someone do this, I would write a message that links them to
[55:09] a place where they can get the CLI installed. So let's first figure out where that link is.
[55:14] So just Google Vercel CLI. >> So that means, hold on.
[55:29] I'm going to grab this then and go up here. Would I do it as notes then like this?
[55:40] >> No, not necessarily. So I would have it be explained still where we were already. Because at this point, it's not really a concern up until this point.
[55:50] Sometimes people will put the requirements at the beginning, but for what we're doing here,
[55:56] I think it makes more sense to just build a thing and then be like, now, we're going to deploy.
[56:00] If you already know how to deploy somewhere, you can go do that anywhere.
[56:02] But if you want to do it this way, here's instructions to do that.
[56:05] >> Okay. So, yeah, and I have the link. >> Okay. So first, let's write something out of how we want to explain it.
[56:21] So I'd say I'm like something of the effect to go to this link for instructions to download the first LCLI.
[56:30] >> Then I would be able to do this, right? So it shows what it is and
[56:51] then put this one in here, maybe. >> I'll do it, yeah. Then hit a period.
[57:04] So you should change that a little bit. So it should be go to link for
[57:09] cell CLI download instructions. Let's change that to just four and then get rid of the two,
[57:20] and then copy paste for cell CLI and put it before download instructions. >> I feel like this is going to be what drives
[57:32] everybody insane is my grammar on these. >> As long as it's grammatically correct,
[57:38] that's the most important thing. So we're going for clarity and understandability here.
[57:45] So there's going to be lots of ways you could phrase this that could be correct and it's just a matter of taste.
[57:49] But there's also some things that you want to make sure you have. Because otherwise, other people would go back and they might be confused
[57:55] and it's just a good practice. Some people will write docs who English is
[58:00] not their first language and that's totally valid. That's why you should be trying to help people make their docs more clear,
[58:05] but also be aware of where people are coming from and don't try and put them down for having small little mistakes like that in their stuff.
[58:16] >> So I would just do the NPM, right? >> Yeah, let's see if that works.
[58:22] >> I did an NPX the other day. That was fun. >> Yeah, I saw. So NPX is the same as using yarn the way we've been doing it.
[58:38] >> Oh, okay. >> So this is saying the permissions is denying us.
[58:49] This means that you're trying to download this, but your computer needs you to be in root access for it.
[58:55] So you know sudo, that's how you- have you ever used sudo before? >> I think we had to do this last time.
[59:01] >> Yeah, I had to use sudo once. So I just told you to do that and we're over text,
[59:04] so it probably didn't make any sense. So that's what sudo is. That's why sudo asks you for your passwords.
[59:08] That's why sudo is only something you should ever run. You know you're downloading something that you trust.
[59:13] You trust for sale, it's a giant massive company. They're not going to load random code on your computer to mine Bitcoin.
[59:19] Some stuff on NPM will though. So don't ever just do this and download random packages.
[59:23] >> Good call. >> Think the name of the packages.
[59:26] Because there's squatters who will find packages with slight typos, and then try and put stuff in that.
[59:32] So when people make typos, they'll accidentally download the thing they didn't mean to download.
[59:35] It's a whole thing, the whole supply chain thing.
[59:38] >> Oh, geez. >> This is fine. What we're doing right now is totally safe.
[59:42] >> I don't even know how to spell sudo. >> Okay. Sorry. It's not spelled like the word sudo,
[59:47] it's S-U-D-O, yeah. >> Then install it.
[59:53] >> That exact same command again, and it'll ask you for your password.
[59:56] >> Just in case it's going off screen. >> Installing, hopefully.
[60:16] >> Yay. >> Great. Now, go back to your README again,
[60:22] and then do three backticks with bash. Then you want to put a space after the backticks,
[60:33] it's going to be right next to the backticks, and line break, and then just the word Vercel.
[60:42] Then line break, and then three backticks. Then try running that in here.
[60:50] Now, this is going to ask you to do a couple of things, since we haven't done this before.
[60:53] It's going to have you probably log in and stuff like that. I would not put those instructions in this,
[60:58] because you already said you need to log in and do that, so you can assume people are going to make it through this,
[61:04] and that they can't, that's like on Vercel to document that correctly.
[61:08] But this is going to be extremely simple the way this works. Great. Now, go back to your terminal and see what happened.
[61:15] >> Yay. >> Okay. Now, it's going to ask you to set up and deploy this thing.
[61:20] You're going to just hit "Return" because yes, is the default answer you want.
[61:24] You want to use TeachGenTech. Then we don't want,
[61:29] let's not link this to any existing projects. Let's just select "No",
[61:33] and then that's good, and that's good. That's saying your project is in this folder that you're in right now.
[61:42] Then what that is doing is it's giving us a default build steps, so those are going to be good.
[61:48] No, you don't want to modify these settings, so just hit "Return" again.
[61:53] Great. There's a flag, dash dash confirmed. I think that will have you just answer all the defaults
[61:59] automatically and it would just deploy it straight for you. But it's good to walk through it a couple of times,
[62:04] so you know what you're doing. Sometimes it's not always exactly the same,
[62:06] especially the build step part. See how it says "Beat" and "Beat Build"?
[62:10] So that's beat specific. If you did this with create React app,
[62:13] that would not say "Beat Build", it would be something else.
[62:16] Okay. See if you can go to that link now, my React app, KOL.
[62:23] There you go. There's your website. So now what I would do is I'll go back to my read me and write,
[62:39] open, and then I'll paste that link. So you would link to that.
[62:49] >> Wait, we got to do the square brackets. >> Ben was telling us that sudo stands for super user do,
[62:58] where super user is a word for admin. That's about right. >> I dig it. All right.
[63:07] >> Excellent. Make sure there's a period at the end. That should be pretty much it.
[63:15] Now, copy paste that whole thing and put it back into the gist so we can see what it looks like altogether.
[63:20] Edit it now. Now, when you copy paste it,
[63:32] you're going to have much actual lines at the end, I think, so delete those.
[63:36] Update public gist. >> Well, that was fun.
[63:48] >> So now, you will have this gist for the rest of your life, and anytime you want to deploy a React app to yourself with VT,
[63:53] you'll open this and you will follow these steps and you will say prayer to the coding gods that they told you to write documentation.
[64:03] >> This is happiness. >> See, it's very useful, not only for you, but for others.
[64:13] >> I'm actually really glad because I'm doing the timing of going back and working on when I can work on getting
[64:27] the blogs written from the very beginning. At least one episode is already done,
[64:34] the very first episode or the second episode. There we go. >> Interesting.
[64:41] >> You should also get this project up on GitHub repo. That was one thing we didn't do.
[64:46] Because Vercel lets you do that without needing a GitHub repo, which is nice, but this is a good step to do.
[64:51] >> Teach me the things, please. >> Go down to the bottom of this one.
[64:55] Let's go ahead and put it in the read me too, that way you'll have it. Then make
[64:59] another two-header that says create GitHub repository. >> What I would do here is I would say open and then link to repo.new.
[65:32] >> Would you put repo.new and then put the link, right? >> Yeah. There's different schools of thought around this,
[65:41] but I think that works pretty well. >> I think I'm doing this wrong.
[65:53] >> That'll be an opening square bracket, and then a closing square bracket at the end.
[65:58] Then you have to write that again with HTTPS in front of it, colon slash slash. One step that's also useful to go through is go back through your gist at the end,
[66:15] and click all your links, but let's not do that right now. That's just a hot tip for you.
[66:19] Then let's actually go to this link now and create a repo. You can just call it MyReactApp again, keep it consistent.
[66:38] Then give it a description. >> That's just the description we used up here, right?
[66:48] >> Yeah. >> This one?
[66:50] >> Yeah. >> Then it can be public?
[66:55] >> Yeah. You don't need to add a README, because you already have a README.
[66:57] You don't need a GETIGNORE, because you already have a GETIGNORE. Let's go ahead and create a license at MIT.
[67:03] Actually, no. Sorry, that's going to confuse it. Let's not do that. Hit the X on the top right.
[67:11] Because then if we try and push the changes up, because it's not in there, it's going to get confused,
[67:16] but we'll add a license next time. Create repo. Now, copy-paste that whole chunk,
[67:25] the first chunk, or create a new repository on the command line. Take what's written under that and grab that whole thing.
[67:34] >> Then I just paste it in here, right? >> Yeah. First, go back to your README.
[67:41] >> Okay. >> Yeah. Then do backticks bash.
[67:49] Yep. Lowercase b. Then copy. Then delete line 1, or the first line of that.
[68:01] >> Echo? >> Yeah.
[68:02] >> Because we already have that. >> But if you follow those ones exactly as they're written,
[68:07] then you will have your thing deployed to that repo. Now, it's important though that in
[68:12] these commands there's the name of this specific repo. Every time you do this,
[68:16] these commands are going to be all the same except for git remote add-ors.
[68:20] That's a really important step where you actually link your repo to the repo you just created on GitHub. Does that make sense?
[68:28] Look at line 67 right now. >> Yeah.
[68:35] >> You see how teach-gen-tech is in that URL, right? >> Yeah.
[68:38] >> If someone followed these steps, they would not want to copy that command because they would
[68:42] then be syncing their project to your GitHub, not theirs. >> Oh, yeah.
[68:46] >> Everyone who'd use this when they create it, they're going to have their own name in that right there.
[68:49] They would have even their own name for their app possibly, depending on whether they changed the name when
[68:54] they generated the thing at the beginning of the project. That's an important thing.
[68:58] This is why I always write these commands in just for myself and I have them there so I can
[69:01] go back and I can do it over and over again. But that may potentially confuse people
[69:06] if you're expecting this material to be super-duper new, so you should possibly add
[69:10] an explanation and they're saying, "Follow these steps with
[69:14] your own Git repo in this line," or something like that. >> Okay.
[69:20] >> Oh, sorry. Actually, there's another mistake here. Where it says, "Git add readme,"
[69:26] that should be "Git add period." Yeah, just like that.
[69:33] Then make sure to run that command again. Yeah, there you go. Yeah, so what that does,
[69:39] if you just did "Git add readme," it would only commit that one file,
[69:43] but you want to commit your whole project all in one go. >> Okay. I'm going to make myself notes here in a second.
[69:56] >> Then we should also reconfigure your Git, so it does main by default.
[70:01] We can do that real quick. Okay, that's all good. Before we do anything else,
[70:08] let me just do this real quick. Go up to where in the terminal where it says,
[70:11] "Git config --global" in your error message. It's "Git config --global" and then dot deep.
[70:18] Exactly. Yeah, so grab that whole thing all the way over to "Git config,"
[70:22] and then paste it, and then delete that, and also delete the brackets around it as well,
[70:30] and just write main one word all lowercase. What this is doing is now every time you create a Git,
[70:36] you initialize Git, you're going to start with main as the branch instead of master.
[70:41] >> Okay. >> Yeah. Then do add the actual line.
[70:48] >> I'm making myself a note really, really quick. >> Since you didn't say this, you didn't push
[70:53] these last changes up, so first, let's do that -- and then, yeah.
[70:58] Let's finish this, and then we'll commit it one more time before we're done,
[71:01] so don't worry about that yet. Write whatever you're going to write,
[71:04] and then once you're done writing stuff in this, we'll commit it at the very end.
[71:08] >> Okay, so this is -- >> You're going to want to add a line break
[71:14] there after the code text. That's the thing where Markdown will work fine
[71:17] if you don't have these extra lines, but I try and keep it consistent and clean,
[71:22] because when you're going back and reading these and working with them,
[71:25] the more you can make it clean the first time, the easier it's going to be for others to
[71:28] work with and all that kind of stuff. >> Feedme.md, oh, all caps, okay.
[71:37] >> Yeah. >> Feedme.md, and then --
[72:00] >> This is great. Let me also show you something real quick.
[72:02] This is where you're going to want to put backticks around git add readme and git add period.
[72:09] So just a single backtick. >> Oh, a single one?
[72:15] >> Yeah, just a single one. >> Yeah, okay.
[72:17] >> You'll even see a change in your editor right there. >> Okay, cool.
[72:20] >> Yeah, this is really important and useful for when people are reading these and both,
[72:25] when you're going back and you're like, if you're copying things and stuff,
[72:28] you want to make sure there's a clear distinction between things that are like code stuff
[72:31] and things that are just normal wordy words. >> Mm-hmm, and then.
[72:38] >> You also start by doing the backticks in the exact and then paste it in, yeah.
[72:44] >> Each. >> Individual repo.
[72:52] >> Okay. I was like, how do you say that? >> Let's do this now, hold on,
[72:59] there's something else we can do. This is perfect. >> Can I delete this really quick because I just realized,
[73:04] I could just put gen notes at the bottom and then people can still use them.
[73:09] >> You should make these bullet points also. So what you're going to want to do is,
[73:13] you're going to want to do a dash before each of those, and then a space, dash, space, yeah.
[73:19] You should make gens notes its own header. >> I'll use it, it doesn't need that.
[73:29] >> Well, you shouldn't do three because it's not a subsection of the section before it.
[73:32] It's its own section, yeah, and make sure there's a space after the.
[73:37] You also see how it changes colors every time, whether the syntax is correct or not.
[73:43] So notice how it turned blue once you did that, but it wasn't blue before.
[73:46] Yes, that's important because that'll help you avoid making those mistakes when you're writing this markdown,
[73:52] because you can write markdown and then not really look at what generates for a really long time,
[73:55] and you end up with weird stuff you messed up. That's why the editors give you a lot of useful hints here.
[74:01] >> Use folder name as project name. I'm doing it for myself.
[74:14] So whatever I created the folder on or now. >> I always keep them the same.
[74:20] You don't necessarily have to, and it'll depend on your own style and stuff like that.
[74:27] But I like to keep the product name is always the same as the code folder name which is always the same as the repo name,
[74:32] and it's just always going to be the subdomain of the website, a point of our cell.
[74:36] I keep them all consistent across the entire thing. But for this one, that's probably
[74:41] because you're doing my React app. That's something that there's already
[74:43] hundreds or thousands in the world out there of that. So we couldn't get my react.versell.app,
[74:49] we have one with a bunch of numbers at the end. Now, if it's at ajc-react-app, then it will be taken.
[74:55] That's why ajc-webdev, I have that in all of my project names. They all start with ajc-webdev- whatever
[75:01] the tool is that I'm doing or the project I'm doing. That way, all of them are stamped with something
[75:05] unique so I can do that across the whole thing. >> Then what, and I know that you said that we're going to upload
[75:14] this or re-commit, I want to put that in here, like when I make changes on VS Code,
[75:26] make sure to do this to re-upload to. >> That's one level that
[75:31] you probably aren't going to want to write down, because that's one of the very first things.
[75:35] It's showing us how to get to the right folder, telling us to commit on changes.
[75:40] It's outside the scope of almost anything you're going to write for the most part.
[75:43] >> That's why I put it in gen notes. >> Okay. I mean, yeah, that's fine.
[75:46] I guess there's a question of like, yeah, no, that's valid. >> I think you're absolutely, yeah.
[75:53] >> If you're reminding yourself, that's a good thing to remind yourself of,
[75:56] is that make sure to commit file changes and push to GitHub when you're done,
[76:01] or for the last step or something like that. That's a good note to write yourself.
[76:10] >> What's the way to do it? >> If you look at the first steps on GitHub,
[76:18] the first steps you have where you had to get in it, so you don't need to get in it again,
[76:22] because that just starts it being a Git repo. You do have to do git add period and git commit.
[76:29] Then you skip git branch because we already have done that, and also now your computer does that automatically for you.
[76:35] The remote is never going to have to be done again, but you will have to push each time.
[76:39] So it's three steps, add, commit, push. >> Hold on.
[76:46] >> So first grab add and commit, or yeah, just grab all of them.
[76:50] >> Okay. This is a part where thinking back to Resolve and where I've been getting really confused.
[76:57] If I want to download somebody's, or do something to connect to somebody's Git
[77:03] or a repository I already have, I need to do git init and then that name.
[77:09] >> No. >> No.
[77:11] >> Well, you might be able to do that. I don't know if I see that very often.
[77:18] Let's see. You can do that for template directories and stuff like that.
[77:22] But basically, if you want to connect to someone's Git repo, you need to clone it down,
[77:26] like you clone their Git repository onto your computer, and then you have it on your computer,
[77:30] and you don't run Git init because it's already a Git project. You don't need to initialize it again.
[77:36] You clone it down and then you enter it, and then you're in a GitHub project already.
[77:40] >> I'm going to ask that a different time then. >> I might have misunderstood what you're-
[77:46] >> No. I think you're right. I think I'm just not comprehending yet, which-
[77:51] >> Yeah. Part of it is because something I can show you. This is one where you're going to want to do this.
[77:57] >> We do the git add, we do the git commit,
[78:00] we don't do the main, and we don't do the branch, right?
[78:04] >> Yeah. >> We don't do the main, we don't do the branch.
[78:11] >> If I were you, I would put those in their own code block by itself, like the three backticks,
[78:19] because you're going to want to grab these commands consecutively, so it makes sense for them to all be in their own code block.
[78:25] >> Oh, code block. Okay. >> Yeah.
[78:29] >> I'm going to make sure to get rid of that last one. There's one at the end of the git commit line.
[78:37] Then do a line break after the three backticks at the beginning, and make sure it says bash,
[78:48] so write bash and then hit "Enter". There you go. Then add another line break for 78.
[78:55] Add another line break in between the code block and the- yeah, there you go. Then actually where it says git push,
[79:00] you origin main, it just has to be git push, because you already told it that the origin is main.
[79:05] >> Okay. >> That has to do with connecting it to the- when you're pushing it,
[79:11] are you- because there's a git thing on your computer, which is just a git repo,
[79:18] and then there's a GitHub repo on GitHub, and so that's the remote. When they talk about the remote,
[79:22] they're talking about something that's on GitHub itself, like on the Internet.
[79:25] To get it there, you just push it onto the Internet. That's the most important thing.
[79:29] But I want to show you that there's a folder in your actual project. So go back to your Finder and open this folder up,
[79:36] and actually save first. OCD. Great. Actually, open this in your desktop.
[79:46] Anthony is cool, and make this a lot bigger, so other people can see as well. Is that possible?
[79:54] >> I don't know. >> Okay. Oh, well. So go and then go into- and Anthony is cool.
[80:00] Actually. >> I feel like there's got to be a way.
[80:05] >> Yeah. So if you go to show a few options towards the bottom, and then make it as big as you can.
[80:16] I don't think this is going to be enough though. Yeah, it's going to be barely any different.
[80:20] It's a little better. >> Okay. Well, we're working on it.
[80:23] >> This is confusing. I actually have a project folder, it's not a project folder.
[80:27] You should take my React app and drag that out into the code folder folder. >> It is? Oh. Well,
[80:34] I'm going to leave it there for now because I don't want- >> You should do this.
[80:38] >> Really? >> Yeah. Then delete Anthony is cool.
[80:41] >> Okay. >> And you can- yeah.
[80:45] >> Whatever. I'll delete it in a second. >> Delete. Click out of that,
[80:52] this hit up arrow, then delete. And you do Command D or Command Delete to delete.
[81:00] You don't need to use your mouse at all. >> Oh, that just duplicated it.
[81:04] >> Sorry. I mean, Command D, I'm going to delete the delete key.
[81:07] >> There we go. Got there. >> Sweet. All right. Now we're here.
[81:11] Press Command Shift period. There we go.
[81:21] All right. This is a thing that don't get taught to a lot of junior devs.
[81:24] It's extremely confusing. There are folders in this MyReact app
[81:30] that you were not able to see until you did that because they all have a period in front of them.
[81:35] Now, that period is basically the stuff that's happening under the hood.
[81:40] So you see how it says dot get. So if you click that, this is
[81:45] what didn't exist when you ran get init. So when you run get init,
[81:49] what it does is it creates this folder right here. So if we were to delete this folder, don't do this.
[81:53] If you were to delete this folder and then go back to your project,
[81:57] it would no longer be get. You would not be able to see your changes.
[82:00] There would be no history of what you did and you need to run get init again to re-initialize.
[82:05] Then you could add and commit and do all that. So I end up deleting my dot get folder.
[82:10] Anytime something weird goes on in get because there's crazy get foo
[82:14] you can do to get yourself out of jam. So sometimes just resetting and
[82:17] cloning a repo down and doing it again, it's actually going to be easier.
[82:20] But don't worry about whether to do that or not. The only thing that's important is to know that it's
[82:24] even possible to do that at all. >> Yes. We had to fix
[82:30] my terminal by doing one of these, right? >> Exactly. That's how we got rid of it.
[82:36] >> Yes. Because your dot zhs and dot z profile and all that stuff is also those are dot files.
[82:43] >> So I do remember that, but okay, cool. Yay.
[82:46] >> Great. So now let's make sure to push all these changes up unless you have more notes you got.
[82:50] >> No. Well, if I do. >> We're getting close to time. I should go in here.
[82:56] >> Add. >> Nice. Then since that's in the readme of this repo,
[83:11] you should go back and delete the first gist. You don't really need this to be in a gist if it's in the repo itself.
[83:17] >> Where's the gist? >> Go up where in your tabs,
[83:25] it's your top number one tab, so it's like your browser tab of not in the website at all.
[83:31] Yeah, just delete that. >> It doesn't add it. Yeah, I get what you're saying then.
[83:38] >> Great. Because otherwise, if you're trying to keep that in sync, you have a readme for the same thing in
[83:43] two different places and you're changing one, not the other. You get confused very easily.
[83:46] So keep everything in one place and not duplicated. That way, anytime you're making changes,
[83:51] you only have to make change in one place. So now, anytime you want to add to this,
[83:54] you can go back to this repo, you can add more instructions,
[83:57] you can test those out, and then the instructions will still be there.
[84:00] >> I created my first repository. >> Yay.
[84:05] >> Actually, there's one more thing we can do. Go back to the repository, click on it,
[84:11] and then scroll down to where the link is for your website. It's like the actual website.
[84:19] So scroll down to the very, very bottom. Then click just above the repo.new part.
[84:25] So grab that, copy that, copy the link. Then scroll all the way up to description or about,
[84:39] and click the little icon to the right of about. So over on the right side of your screen,
[84:46] about, and then paste it where it says website. So if you got to have the HTTPS part in front,
[84:51] this is why you got to copy the link itself. Great, and then save that.
[84:59] Then try clicking the link. >> Yay.
[85:04] >> So now when they go to this repo, they can instantly see the website that's linked to the repo.
[85:10] >> Yay. >> Yeah.
[85:13] >> Oh, this is exciting. So much learning and just light years further than I was a month ago.
[85:20] >> Totally. >> Crazy to think that that was only a month ago.
[85:24] >> I know, right? >> I mean, I have debated doing 100 days of code,
[85:31] but I'm like, I do it four days a week, does that count? Thank you, Anthony. I know you need to go.
[85:38] So thank you once again for all the knowledge drops. This is exciting. This is actually really, really cool.
[85:48] >> Hopefully, yeah. If you can come to enjoy the process, it'll be easier to do it and to do it consistently.
[85:55] Once you start to see the virtues of it, it's really awesome. To me, this is like taking
[86:02] documentation and making it more like an iterative, reproducible thing. Because what a lot of people do is they'll write
[86:08] all this code and then try and document after the fact. That's like, it's really hard to do.
[86:13] There's so much context you need, you may just do stuff without thinking about it.
[86:17] Then when you're going back, you forget steps or anything like that. So this way, we actually have to write it down as you're doing it.
[86:22] As long as you write down everything you do, then you're guaranteed to get all the steps in there.
[86:27] >> Yeah. Cool. Well, thank you so much.
[86:32] I greatly appreciate it and so much more learning. Until next time. Thank you.

