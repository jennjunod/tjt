---
showLink: "https://www.youtube.com/watch?v=H_LSQVRkgjk"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-svelte-web-development-with-brittney-postma"
title: "Teach Jenn Svelte & Web Development with Brittney Postma"
publishDate: "2022-10-11"
coverImage: "https://i.ytimg.com/vi/H_LSQVRkgjk/maxresdefault.jpg"
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

[00:00] Hello, hello, beautiful humans. And yes, I was totally doing a dance that nobody could see.
[00:07] They just saw the shoulder motions. Welcome to another episode of Teach Gen Tech.
[00:14] I should, at some point, really look up what episode numbers there are so that way I can track
[00:19] how many there have been. Today we have Brittany on the show.
[00:23] And Brittany does a ton of stuff, but I'm going to let her introduce that.
[00:28] That's a great introduction. That's it.
[00:31] I just do too many things. I never said too many.
[00:33] I said you do a ton. There is a difference.
[00:36] There is a difference. Because when people are like, Jen, what do you do?
[00:39] And I'm like, I do stuff. I do things and stuff.
[00:45] Because I think I do too many, so I get you there. So thank you, Ben.
[00:51] There is a difference. Yay, Ben.
[00:55] Who are you, and what do you do? Yeah, absolutely.
[00:59] So like you said, I do a lot of things. But first and foremost, I guess I'm a developer experience
[01:04] engineer at Netlify. We're still trying to figure out what developer experience,
[01:08] DevRel, like developer avocado. What does that mean?
[01:12] But I basically get to do a lot of content like this. I get to do a lot of podcasts.
[01:17] So I work with CodingCat.dev. We do a podcast there.
[01:19] I'm on Svelte Radio. I do remotely interesting with the Netlify folks.
[01:25] What else do I do? I run the Svelte Sirens, or I help run the Svelte Sirens.
[01:29] I'm the co-founder of that community for women and non-binary people in the Svelte community, which
[01:34] is what we're kind of here to talk about today with what the Svelte, right?
[01:37] I love the title. I remember when-- so y'all, I just
[01:44] want to say I've talked about this in Twitter spaces. I feel like this is a big thing in the community of you
[01:52] don't DM people just like hey or hello. I awkwardly DM people all the time.
[01:58] It's just not hey or hello. I was looking at Brittany's, and this is back in August.
[02:05] And I'm like, I never realized you are you, and I follow you on Twitch.
[02:09] And Ben was on your show yesterday, too. That is-- and hi.
[02:15] I feel like this is Jamstack. And I'm wearing a Jamstack t-shirt today.
[02:19] But this is the Jamstack community where you will run into people in places
[02:24] that you don't think you will. And then you'll know people that you
[02:27] don't recognize right away. But you're like, oh, I saw you in this other place.
[02:31] And I feel like that happens all the time in this community, which is why I love it.
[02:34] Agreed, agreed. And good morning, homie.
[02:38] Yes. And I love-- one of the first things I saw was--
[02:43] I feel like now that I-- Svite?
[02:46] Svelte. Svelte.
[02:47] What the Svelte? Because I kept trying to say Svite,
[02:50] and I think it's like me getting mixed up with veet, invite. So there's actually an emoji.
[02:57] So I'm also doing veet conf today. I'm helping moderate the chat.
[03:01] And veet conf's going all day. And so earlier, since it's veet conf,
[03:05] we have a Svelte and veet emoji. And it's called like veet Svite.
[03:10] I don't know how you say it either. But it's the two words mashed together.
[03:14] And it could be that confusion there. It's a weird, strange world we're living in.
[03:21] I guess all these French words are-- Yes.
[03:24] --confusing us. Yes.
[03:25] And on the point of being a developer experience and stuff, you were talking about the--
[03:32] yes. Yes.
[03:34] That's going to make it even more confusing. Yes.
[03:38] I started using the term developcado because I'm like-- Just smash them together.
[03:44] Yeah, I just smushed them together. I was like, this is just what I am going to call it,
[03:48] is developcado. Done.
[03:52] Yeah, it's just done. And what does that mean?
[03:55] What do we do? Nobody knows.
[03:58] Content. Yeah, we create content.
[04:00] I've actually come-- I really like the way Netlify does it. They integrate us with the engineering and the pillar
[04:06] team. So we're making the experience better for the developers
[04:11] once it's released. So we're actually making sure that the tooling works well
[04:14] for the company you work at. And I really like that format of it,
[04:17] more than being like developer marketers have a place, but that is not what we do.
[04:23] We're not marketing Netlify. We're using it and making it better for--
[04:28] Yeah. OK, so super weird randomness, but lunch dev,
[04:35] I can see the comment in Twitch, but I can't see the comment in StreamYard.
[04:43] Yeah, I noticed that too. Sometimes Twitch does that to us too,
[04:46] because we do this where we push out to YouTube and we push out to Twitch.
[04:50] And if we go live somehow through OBS, Alex does it on his end.
[04:55] And it won't show any of the comments from Twitch. It will just show them from YouTube.
[05:01] And it's really strange. Oh, thank you.
[05:05] Thank you, Ben. Coding Cat hat.
[05:07] And I have my Netlify hat over here. I'm starting to swag.
[05:11] Love it. That is one thing that is too addicting and probably not
[05:16] sustainable at all, is all the swag. Oh, I know.
[05:20] And then my sticker board is too full. I actually am really cheap with stickers,
[05:24] because I know I only get one or two of them usually. So I put Scotch tape on the back of them
[05:28] and tape them to this board so I can replace them. And so I can take them off and change them out.
[05:35] I really like the idea of a sticker board, though. Yeah, instead of all over my laptop,
[05:40] I just have a board up here. It's just a piece of wood, like a square board
[05:43] that I got from Walmart or something, and throw some stickers on it.
[05:47] I dig it. I dig it.
[05:49] And Ben, yes, Ben has swag too. I have one of his HTML shirts.
[05:56] I want to get one. Once I get a job, Ben, I'm ordering one.
[06:01] I'm so excited. All right.
[06:02] So yes, what the spite? Svelte.
[06:07] Damn it. It's OK.
[06:09] We're going to get you hired, though. And that's kind of what we're going to talk about today.
[06:13] I have a talk coming up in a couple of weeks at Web Unleashed. And it's called Starting with Svelte.
[06:18] And this is really where I'm trying to get in my head, is that I think web developers who are just beginning
[06:24] their journey and have maybe a basic HTML/CSS understanding, maybe some JavaScript, should actually
[06:31] start building with Svelte because it helps you build projects faster.
[06:35] So if you can build faster, you can get your projects built, you can get your portfolio built,
[06:40] you can get your resume up, and you can get a job, which I think is the goal of most people
[06:45] beginning web development, right? Yes, yes.
[06:49] I dig it. I dig it.
[06:50] And I told you that we are on the Windows machine, which-- hey, y'all, we have improvement.
[06:58] Brittany uses a Windows machine. I do.
[07:01] I use-- for all of my streaming, I use a Windows PC, which is not becoming the norm anymore.
[07:06] It used to be the norm for streamers, but it's not anymore. So I'm all WSL.
[07:11] I use all the things Windows. It's fine.
[07:14] Yeah. So we've got some goodness there.
[07:16] And hopefully-- I will say, hopefully, I get my Mac back tomorrow.
[07:20] I'm hoping. I hope they say that it's there tonight, so by Thursday,
[07:24] I can start streaming on my Mac. And then we also installed Volta.
[07:31] But I don't know. Can I download--
[07:34] I'm interested to see that, too, by the way. I don't know how you download the Volta front or Svelte.
[07:44] Did I actually say it right this time? You did, yeah.
[07:46] Yes. If I can download Svelte from it,
[07:50] because it was talking like you could download languages, too. Yeah, that's kind of a weird thing.
[07:55] And I don't know if languages-- if it means JavaScript, Python.
[08:00] Does it mean those kind of languages, or does it mean libraries, frameworks?
[08:04] Because there is a Svelte VS Code extension that you can have that will pretty much give you
[08:09] everything that you need. So it's just one extension in Svelte.
[08:14] And, well, so this is Volta. This is what I was installing for all the Node modules
[08:24] that I was having issues with last week. So let's go grab a different tab.
[08:35] And you said that there is one for Svelte plug-in on VS Code? Yes, it's the Svelte VS Code extension,
[08:46] I think is what it's called. I might have to bring my VS Code up.
[08:48] And Homie Codes had a question. Can I give two sentences why Svelte allows noobs to build
[08:54] so quickly in general? So I don't know if I can make it in two sentences,
[09:00] but I think that it keeps the code as close as possible to being vanilla HTML, CSS, and JavaScript.
[09:08] There's very little Svelte-specific syntax in there.
[09:11] So you're writing things that you're already familiar with, and then you're adding those kind of niceties
[09:18] that Svelte gives you on top of it to make it easier and faster to build projects.
[09:23] Hope that was a good sales pitch. Homie's so good at asking those type of questions.
[09:31] I love it. Ask the hard questions, or I don't even know.
[09:36] Was it hard? I say the good questions.
[09:39] Yeah, very good questions. Yeah, Svelte for VS Code.
[09:43] That's it. There we go.
[09:45] And stop. There we go, sorry.
[09:49] Installing. So what was your experience that you found?
[09:54] You, a little before we got on, we were talking about your background.
[09:59] And what was your experience with getting into these JavaScript frameworks?
[10:02] You said Anthony came on and made you build a React web app, which I was like, why did you do that, Anthony?
[10:08] Where are you at, by the way? I need everybody to go tag Anthony Campola right now,
[10:13] AJC web dev on Twitter, and get him in here so I can fight with him about why he made Jen build a React
[10:19] web app as her first intro to JavaScript. So a lot of it has to do with I've worked in the tech
[10:28] industry. And I say I was adjacent to it in the fact
[10:34] that I was a part of sales, or I was a part of marketing. But when I was at Verizon, it was
[10:47] when the iPhone and Android first came out. So it was a lot more technical.
[10:54] And it was where I definitely learned a lot, got to this point.
[11:03] I've done advocacy for other things. I have the podcast, Shit You Don't Want to Talk About.
[11:08] And it was in January, I was let go from an API design first company.
[11:16] And they taught me all about the APIs, because they wanted me to create a curriculum about it.
[11:25] And yes. And thank you.
[11:29] And so I built this. I was working, I was learning how to build the curriculum.
[11:34] Then I'm working on learning all of this. And they let me go in January 2021.
[11:37] And I was like, I'm never doing tech again. I refuse.
[11:42] Yeah. Well, once I was healed from surgery
[11:46] I had to have in February, and I healed from getting let go, I joined the Denver API meetup team and co-organizer there.
[11:56] And one of the co-organizers, Ori, from API Days was like--
[12:02] this is me paraphrasing horribly, because Ori does not talk like this--
[12:05] but was like, yo, if you could describe a perfect job, what would it be?
[12:10] And without knowing it, I described DevRel. Oh, that's amazing.
[12:15] It was like, dude, you got to do that. And I was like, cool.
[12:17] So Adam Duvander, I met him. He's big in the marketing for developers,
[12:25] because developers hate marketing. And it's so true.
[12:29] And so I knew him from Stoplight. And he posted-- this is when I didn't know how to Twitter.
[12:36] Yeah, I didn't know how to Twitter. I did not know how to Twitter for a very long time.
[12:40] Yeah, not knowing how to Twitter. So I didn't know how to Twitter.
[12:44] And I replied-- he put a tweet out there of like, all DevRels, please reply if you're
[12:50] open to other people talking, like reaching out to you. I'm literally replying to each person.
[12:58] I'm sending them a tweet. Not their DMs, because I don't know how this works.
[13:02] And almost all of them were like, yo, just DM me. And so the first person I met was Wesley Faulkner,
[13:13] which was phenomenal to meet him first. He's over at AWS.
[13:16] And he was just like, yeah, you can be dyslexic in code. Why can't you?
[13:22] And I was like, what? This is the entire reason I never went into code.
[13:28] And then the second person I met was Ramon. And Ramon-- hola, soy milk, for anybody that
[13:37] wants to find him on Twitter. And he was like, yo, we should do some live learning.
[13:43] You can peer program, and you can come on my show. And I'm like, OK, sure.
[13:49] And Anthony, being the third person I met, he was like, you should start your own show.
[13:55] And no, I am not answering any questions about NFPs and whatever they're called, and Web3.
[14:04] He's like, no, no. But yes, you should start your own show.
[14:08] And I was like, OK. And all of them were like, you have no content,
[14:14] you have the personality, and you know how to do everything else except technical content.
[14:22] And I was like-- So you were tech-adjacent for a long time, though.
[14:27] So you kind of got familiar with it that way. Yeah, I was familiar with it.
[14:30] I hung out with developers almost my entire career, but I was never in the code itself.
[14:37] And so that's what I did a lot of, why I had consulted over at Gravity,
[14:44] because they need somebody to know more about the-- help with the community side, because they do have a community
[14:51] manager. And then more of getting out there, the brand awareness,
[14:55] the getting feedback from people, the demos. And I loved it.
[15:00] It was just, I never knew what language to start with. And Anthony being the--
[15:06] It's overwhelming, isn't it? There's so many choices.
[15:09] It is. And I tried, I think, to answer your question, JavaScript,
[15:15] because I heard that it was the most popular thing. And so I tried taking a course through LinkedIn
[15:24] about JavaScript. And I'm still, to this day, really stuck on classes.
[15:29] Yeah, so when you take a course on JavaScript, it goes so far into everything about JavaScript.
[15:36] And JavaScript is a massive language. And probably one of the reasons that people
[15:41] told you to learn JavaScript is that you can do everything with it.
[15:44] You can do front-end, back-end. Instead of writing Python, which I
[15:47] know you had some experience with, you could write Node, Arduino now, which is JavaScript.
[15:53] So you can use JavaScript on both sides. But it's a massive language.
[15:58] And it gets-- to me, the algorithmic parts of JavaScript never made sense to me, and I hated it.
[16:05] I wanted to build. I was a graphic designer.
[16:08] I did a couple of years in college, and then I quit to make money.
[16:11] I needed money, so I was working in restaurants. I worked at a bank.
[16:16] And then I had kids, and I was a stay-at-home mom. And I didn't realize that coding,
[16:20] like front-end web development, was a job I could do. And I just-- I found Free Code Camp,
[16:25] and I started teaching myself to code. And I loved bringing my designs to life,
[16:31] but doing JavaScript just where I needed it. Like, little bits of JavaScript just
[16:35] to interact with the page, not classes and building. Like, I don't want to build a game in JavaScript.
[16:41] That's not me. So I see where that could have been.
[16:46] Classes are just overwhelming. And that was what React was.
[16:49] I actually did the same thing that you did. I kind of looked around to see what I could get a job in,
[16:56] and everything kept saying React, React, React everywhere. And so I knew a little bit of JavaScript,
[17:02] but I jumped almost straight into React, and it was class-based at the time.
[17:06] So it was all class components. It wasn't these, like, you state.
[17:09] We didn't have the hooks yet. And it was just at the time when we were switching over to that
[17:14] that the classes just threw me for a loop. I couldn't tell what was React and what was JavaScript.
[17:18] I was overwhelmed. Yeah.
[17:21] And that's something that I think is big in-- like, Anthony has said this.
[17:29] Ben, I think you had the conversation with Anthony about this, of, like, I need to choose, like,
[17:36] become a bit more niched down. And I agree.
[17:41] So first off, I do need to say I totally agree that I need to niche down.
[17:46] Yet I don't know what to niche down in yet, because I'm not like, oh, this is so much easier.
[17:55] I love that Laura is coming on to do Python stuff. I'm like, that's convenient, because I enjoy learning it.
[18:02] Do I love Python? I don't know yet.
[18:04] I don't know what I love. I've been around APIs a ton.
[18:08] Do I love APIs? And you're in that discovery phase,
[18:11] like, trying to figure out what you actually-- what niche area, like you said, you want to be in.
[18:16] So yeah, I get that. And what up, Cynthia?
[18:20] Thank you for joining today. And yes, OK, so I have--
[18:26] I did download-- I see your question, too, homie.
[18:30] I don't know if we want to dive into that yet. I will touch on that.
[18:34] Do you want me to go ahead and answer that? Yeah, go for it.
[18:37] So first, like, do you know the difference between back end and front end?
[18:43] Like, do you know what we're talking about when we say that? I mean, good question, in the fact
[18:48] that-- let's see if I can say it. Front end-- front end is where it's more public facing.
[18:58] So like, a website or-- if you're talking about, like, a product,
[19:07] it's what the product actually looks like, not what the product does.
[19:12] What the product does is back end. What the product looks like is front end.
[19:17] Yeah, I mean, that's it to a degree. And I think that, like, databases, your--
[19:24] if you're using GraphQL, your API, that kind of stuff is your back end stuff.
[19:29] So what you're doing in Python is probably back end coding. Or you're doing some task, like a bot.
[19:37] Or you're doing something that's processing something. So the front end is what you see on the website.
[19:44] You're absolutely right about that. So in Svelte, we would use SvelteKit, probably,
[19:50] at this point. But there's things like Astro Remix
[19:52] is working on a Svelte router that you can use serverless functions to do those back end pieces.
[20:00] So really, as a front end developer, I feel power--
[20:03] superpowers, kind of, to be able to do that front end code, but still touch my back end without actually
[20:12] having to write back end code. And that's what I really like about these newer frameworks,
[20:16] because they use that serverless mindset, I guess. I dig it.
[20:22] I dig it. There's Anthony.
[20:26] I need to talk to you, Anthony. [LAUGHS]
[20:30] And thank you, Homie. Homie said that I'm getting better
[20:37] every time I describe it. That's why I'm like, I like when new people come on the show,
[20:41] because they're like, what do you know? Well, I don't want to be rude, either.
[20:45] I don't want to be like, oh, you're new to this. No, I'm not trying to be rude.
[20:48] I was just trying to get your understanding of what-- because, I mean, front end, back end, node, Python, modules,
[20:55] what are all these things? Yes, yes.
[20:58] And Chan said, if it's helpful, I think front end, back end split like this.
[21:04] Front end is what runs the browser. Back end is what runs on the server.
[21:08] That is perfect. And yes.
[21:10] Yes. OK, that does clarify--
[21:13] That's a better definition. I was just saying what the product looks like
[21:18] versus what the product does. And I think that's really where server versus the browser.
[21:26] So I dig that. And Anthony, Brittany has a question for you.
[21:33] Why did you teach Jen to build a React app as her first venture into frameworks?
[21:43] Why? Just why?
[21:47] You missed a little bit of the pre, because you wanted her to get a job.
[21:52] So I'm working on this talk called Starting with Svelte. And I think that beginner web developers should use Svelte,
[21:58] because I think it allows them to learn the fundamentals along with building projects quickly and getting them out the door
[22:05] so they can get their resume. And then they have the JavaScript experience.
[22:09] And then maybe you touch React if you want a React job. But jumping into React too early,
[22:15] I feel like adds complexity and confusion to new developers. I would say, though, something that I think
[22:23] has been really, really helpful-- But how do you prototype quickly with vanilla JS?
[22:31] How can you build projects? Yeah, I think something that's become really cool
[22:35] is getting an idea of what all of these frameworks are. And definitely, when I started learning Python compared
[22:44] to React or Next or whatever, I was like, I don't understand. It was very, very altering.
[22:53] Like, ugh, this is too much. I don't understand.
[22:56] Because I was doing all these things in JavaScript that I didn't know I was doing.
[23:00] Now, seeing the different frameworks is very helpful, even within JavaScript,
[23:05] because I'm starting to see how they may connect a bit differently.
[23:10] Yeah, like you said earlier, how you can take these things-- and even though you may not understand it now, later,
[23:17] it comes up. And you're like, oh, now I get what that means.
[23:20] So I think it makes those connections for you. But I think-- because I did it--
[23:26] when I was learning to code, I learned React. And I felt like I got held back a little bit
[23:30] because of that confusion. I feel like just--
[23:33] if I had learned Svelte first, I feel like I would have gotten farther faster.
[23:38] And that's a really good way of explaining it. And I'm looking at what the episode was--
[23:45] deploy a React app with Vite and Vercel. That is technically what he taught me.
[23:51] So I probably said it wrong. No, I was just wondering--
[23:55] yeah, I asked if it was create React app. So I was wondering--
[23:58] oh, so it's Vite instead of using-- you're not a monster.
[24:02] No webpack here. OK, good.
[24:04] I mean, I'm glad it was at least Vite and React, but-- Oh, it still doesn't-- it makes more sense.
[24:09] But I'm still getting to understand Vite and Vercel and Netlify.
[24:16] And I'm just like, I'm not-- all the terms, too.
[24:19] And then all the acronyms on top of all the terms. It's a lot.
[24:24] It is a lot. It is a lot.
[24:26] So as a random update for everyone, I am very excited that, yes, yesterday-- it took a minute,
[24:36] but we downloaded-- or cloned the project yesterday for Python off of GitHub.
[24:47] But before the stream was over, I did not upload it. And this morning, I did all by myself,
[24:54] which I know sounds very silly. But it's like, I kept doing it based on everybody else
[25:00] telling me to do it and telling me how to do it instead of figuring out on my own, which
[25:06] has been very, very helpful and annoying. But helpful.
[25:09] I did it. I was very excited.
[25:11] So I wanted to share that. And if you--
[25:15] I will start sharing my screen. But I'm now going to be really annoying
[25:20] and see if I can create a new folder. So I think you're even farther than I
[25:28] was with learning web development. Because using the command line, you're using VS Code,
[25:35] you're taking yourself out of the browser. I learned on Free Code Camp, so everything
[25:40] was in this REPL-style thing. Tooling is another complexity.
[25:46] Having to have node modules, having to have command line experience, knowing
[25:50] how to move around folders, they're all things that you have to learn.
[25:54] And that was difficult for me. And so I also recommend newer people
[26:01] to just use the browser tools. StackBlitz is amazing, CodePens, CodeSandbox.
[26:09] There's so many tools. Gitpod, I'm trying to think of all the ones,
[26:13] so I don't leave anybody out. I see Willow in the chat, and she's interning at Gitpod now.
[26:18] So I'm making sure that I hit all my bases here. I dig it.
[26:23] I dig it. I would say thank you for that, and that is a good call out.
[26:28] I used to work at GoDaddy, which taught me a ton by itself. But then also in their hosting department,
[26:37] I was tech support. And it's crazy how you don't always
[26:44] realize what you learn at the job is actually something that other people don't learn.
[26:51] So I think that is-- thank you for that call out.
[26:55] I would also say that it's still frustrating, because I'm like, I'll hang out with all the cool kids that
[27:02] know how to do all of this, and I'm not there yet. It's frustrating.
[27:06] [LAUGHS] I'm interested to see what Cynthia says to this,
[27:11] because she said she pushes tools on her students. So I'm wondering, if you're a teacher,
[27:16] I really want that feedback of, if you're teaching web development to students, do you make them learn the command
[27:23] line first? Do you make them learn about node modules?
[27:27] And Webpack and V are those things that bundle those node modules together and make it all work.
[27:33] And learning all of that as a new developer was just like--
[27:36] I had no idea. I started up a Create React app, and I'm like,
[27:39] what are all these folders? I don't know what any of this is doing.
[27:44] Do you want me to walk you through getting-- do you want to stick with vanilla Svelte
[27:48] before we add on the meta framework? So Anthony said you had had someone
[27:52] on that had done Next before. So the difference between a framework and a meta framework
[27:56] is when you take something like Svelte Reactor View and you add functionality on top of it-- so routing,
[28:03] API endpoints, those kind of things get added on top of the framework itself.
[28:08] So Svelte Kit would be the way to kind of create a new Svelte app that would have that back end and front end functionality
[28:17] that we were talking about. But vanilla Svelte would just be using the browser.
[28:20] So it would just be client-side rendered. I'm down for either.
[28:27] At this point, I've messed with something-- how to say this--
[28:31] I'm not going to know the difference. And I think this is the fun thing and the frustrating thing
[28:37] is if somebody says, yo, go do this, I'm going to be like, OK, cool.
[28:42] And then it may take me questions later on to go, oh, that's the difference of the two.
[28:49] Yeah, like Anthony said, I'm probably fine. It's funny.
[28:53] In case anybody wants to know, when I have somebody that's going to come on the show,
[28:57] half the time I'm going, what am I asking? What is this?
[29:02] Oh, you want to use Svelte Kit? You think it's probably fine, even
[29:05] with the new crazy routing? So I have some hot takes about the way Svelte Kit is going.
[29:10] And not everyone agrees with me. And not everyone agrees with the way it's going either.
[29:14] So Svelte Kit has had some major routing changes. They went from a directory file-based routing
[29:20] where you could just create a new file, .svelte file, and that would generate a route.
[29:25] But now you have to do a plus sign prefixed in front of any new route.
[29:29] And then it has to be page.svelte for the front end part, and then plus page.server,
[29:34] or plus page.js or ts for the loading that API endpoint like I was talking about, which is a lot.
[29:45] It's a lot. You need to know what a single component file is first.
[29:50] Then we need to do just Svelte. Yeah. I don't want to create the confusion that Svelte Kit will
[29:59] add. OK, so I'm putting in our private chat the command
[30:05] that you run to just get up and running with a Vite Svelte template project.
[30:11] So Svelte just itself is run with a Vite plug-in. It's just a plug-in in the Vite ecosystem
[30:19] that runs Vite as the build tooling and allows you to write Svelte. Does that make sense?
[30:26] Am I explaining that well? So Vite is the build tool that builds everything and bundles
[30:31] it together. And Svelte is the framework library
[30:36] that we're using to write the code. So that's the syntax.
[30:39] And then Vite is the build tool. And that my app part is what you call your app.
[30:48] Oh, you got it. I think I need to make our screen a little bit bigger
[30:58] so I can see your screen. I don't-- I guess I could have said no.
[31:07] OK, what is happening here? So what--
[31:10] Get ignore. I'm creating a repo.
[31:12] Oh, so that would be Node, probably, is-- I think, is Node in there?
[31:20] Maybe. Let's-- yes.
[31:22] Yeah, OK. And again, that was a huge list.
[31:26] Did you need that huge list? What was that?
[31:31] Even the CLI tool is a little overwhelming. Yes.
[31:37] Build tool is the engine. Framework is the car.
[31:40] That's a good way to put it. Ooh.
[31:43] At some point, we'll be using emojis to define special routes. That would be amazing.
[31:49] I like-- yes. Yes to all of that.
[31:52] I was very, very entrenched in actually getting-- creating a repo from here.
[32:00] I'm very excited. I'm like-- OK, so y'all, I don't know why I just found this.
[32:07] I love it. I just found it a couple days ago.
[32:10] Like, no idea this existed. And I'm like, it has all the commands.
[32:15] So I don't know if you use Netlify at all, but Netlify also has a CLI.
[32:20] So I can push to GitHub and deploy my website without leaving my terminal.
[32:25] I love it. I feel like we should do something about Netlify
[32:31] at some point because-- Yeah.
[32:32] --like, I know it's a thing. It is a thing.
[32:36] And isn't Jason over at Netlify too? Jason Linkstorp is my boss, yes.
[32:41] Oh, yeah. He's coming on the show next month.
[32:47] Sweet. Couple weeks, month-ish.
[32:50] We're going to go with that. Yeah, I'm actually really excited because he--
[32:54] I reached out to him. Again, awkward intro conversations.
[33:00] Hey, so you do Learning with Jason, and I'm going to start a show called Teach Gen Tech.
[33:05] And someday it'd be really cool if Learning with Jason, Jason, is on Teach Gen Tech.
[33:11] That's amazing. And you get so much more comfortable.
[33:14] I was so awkward and felt so bad asking people at first with the podcast.
[33:18] And now I'm just like-- everybody is just a person, right?
[33:21] Like, nobody cares. Just ask.
[33:25] Worst they say is no. Yes, yes.
[33:28] Or they don't reply. I'd have people on there.
[33:31] And you spelled my name correctly. Thank you.
[33:32] Oh, I had to squint because it went smaller. And I'm like, I hate spelling people's names wrong.
[33:38] I can't say names either. But yes, yes.
[33:43] OK, I finally have our folder created. Yay, OK.
[33:49] So we can walk through all of this, too. And actually, if you want to start with doing push
[33:54] to GitHub, and then we'll set up the Netlify CLI. I can walk you through all that and maybe deploy the site just
[34:00] as it is, what you have out of the box. So you want to open it up in VS Code.
[34:08] Yeah. Oh, OK.
[34:13] Sweet. This was exciting because--
[34:17] And what you need to get for Windows, by the way, if you're going to keep using Windows, Power Toys
[34:22] is my favorite thing for window management. It lets you hold Shift or whatever key you select.
[34:28] And you can place them into predefined areas. So I have one for my coding screen and one for my browser.
[34:36] My hope is I never have to run Windows machine again. But y'all, you can see my very, very messy desk.
[34:46] I'm OK. You guys can go on a tour of--
[34:49] so I have three screens. So then I have my coding screen, my live stream,
[34:56] and then having Twitch open because you don't always get everybody's messages or anything.
[35:04] But yes, I would be so happy to never, ever, ever touch Windows again.
[35:12] No offense to you or to Ben. So are you coding in Windows also
[35:17] or do you have WSL on top of this? Because that might be some of the frustration.
[35:22] So WSL is Windows Subsystem for Linux. So it uses Linux-based instead of the Windows-based,
[35:31] which is horrible. So we tried installing that yesterday.
[35:35] But to do it, it had to restart the system. And we were live streaming.
[35:40] And I will say, since I had a restart right before our stream, it tried to install it.
[35:46] And then it errored out. And I was like, I'm not even going to worry about it.
[35:49] You know Windows. So I was like, I'm just going to leave it there.
[35:53] It's going to be great. It's going to be fine.
[35:56] You're going to stop trying to install stuff during streams. Yeah, but how are you going to install stuff
[36:00] during streams? But how is anybody going to know how to do stuff if we don't?
[36:06] I love that attitude. It's like you just do it.
[36:09] And you see what happens. I don't think I need to paste that all together.
[36:14] OK, so we have a directory. OK, let's see what happens.
[36:22] So the My App part of that is it's going to call it My App now.
[36:25] And I think what's going to happen is it's going to create a directory inside
[36:29] this directory, which may not be what you want to happen. But we can CD into it.
[36:35] That is what happened. OK.
[36:41] So if you want to rename it, you can. Or you can just leave it in that top folder.
[36:44] And then we can CD into that and then open that in VS Code. To learn Remix, and we spent 90 minutes debugging Node.
[36:54] That sounds amazing. That stuff is very important.
[37:00] But I do like Remix a lot, too. And I can understand, though, with the new--
[37:05] I heard that Node 18 is hitting LTS soon. So I've also done that on a live stream.
[37:12] So when BDougie was able-- I told you I spilled water all over my laptop.
[37:20] So the following Monday, I was on the PC. And we were trying to install Node and stuff.
[37:27] So that way, we did Node 18. That's why we ended up doing Volta now,
[37:31] because we spent 30 minutes trying to debug and figure out how to get the project to work.
[37:37] It was entertaining. Yeah.
[37:40] Wow. Yay, we are here.
[37:43] We got it. OK, so we now have it open.
[37:47] Let's open-- do you like to use the terminal? Or do you like to use the integrated terminal in VS Code?
[37:54] I use the integrated terminal, but you use what you're comfortable with.
[37:57] I'm down for whatever. To do the integrated terminal, it's just you click Run, right?
[38:04] Maybe. Or View, I think.
[38:07] Nope. Control, and then the little backtick button on your keyboard
[38:12] will open it for sure. I don't know what that opened.
[38:17] Actually, it opened a group. There we go.
[38:19] Like I thought that would. Let me minimize this one, then.
[38:23] And voila. Yay.
[38:27] OK, it looks like there's already a git initiated, but we might want to run git init just to make sure
[38:33] that it's initiated already. Yeah.
[38:42] And so already initialized-- or OK, it's initialized now. So now we want to create the GitHub repository.
[38:49] So you want to run your CLI. Oh, you already did.
[38:52] Yes, I did it backwards, though. So--
[38:55] So maybe what we need to do is get your-- copy your clone code.
[39:00] Do you know what I'm talking about, to git clone? I'm moving this over here because--
[39:09] What did we call it? We called it spelt V--
[39:12] Brittany? Yeah.
[39:13] So I did create it. And so go to-- at the top, go to click on Code.
[39:19] I'm pointing at the screen like you can see where I'm like-- Yeah, and copy that.
[39:24] And instead of clone, though, we actually want just the HTTPS. So switch over to HTTPS and copy that one.
[39:31] Yep. And then in your terminal, you're
[39:35] going to say git remote, and then RM for remove, and then origin.
[39:44] OK, this is like-- Yeah, going on to the next line.
[39:50] And then hit Enter. And that'll remove your current origin
[39:52] if it has one, no such origin. OK, so now you want to git remote add origin,
[39:59] and then paste that link. OK, so now it's linked up to that repo.
[40:10] So what we can now do is try to push. And it's probably going to complain because the version
[40:17] history is messed up. So my GitHub CLI also does this.
[40:23] So you're actually on the main branch, it says. But it doesn't do that.
[40:27] So what I do in this case, I do git checkout -b main. And then hit Enter.
[40:36] And now it's switched to the new branch main. And do a git push, and then do --force, I think.
[40:45] And that will force a push. - Dash-- no, wait.
[40:49] - Hacking, yep. - Force?
[40:52] - Force, yeah. Oh, it wants you to do the full thing.
[40:57] OK, so in this case, copy that. And then try Enter, and see if it'll just push to that.
[41:05] And then if not, we'll have to do the force again. Yeah, so paste again, and then do the --force
[41:11] at the end of it. Git punch-- yes, I need a git punch.
[41:15] Like, just make it do what you want it-- what?
[41:19] Failed to push some refs. Is it not force?
[41:21] Is it one dash? What am I missing here?
[41:24] Git push force. Is it one dash?
[41:31] Is it-- - Oh, it says two dashes.
[41:34] - What? So maybe you can't do it.
[41:36] So why is this not working? Can we just create a new group?
[41:44] - Create a new group? No space.
[41:46] OK, no space. But she doesn't have a space.
[41:51] You don't mean after main, right? - I'll try that, too.
[41:58] Welcome to the live stream. - Now we are debugging Git, because you
[42:06] are in an existing repo. But if the histories don't match up,
[42:12] it should let you push over that, right? You have to get rid of the outer repo.
[42:19] Oh, because of the folder structure. So it wants you to basically CD up to the main one
[42:26] and push if you want to do it that way. But that's going to mess everything up.
[42:29] So-- - OK, I have a new idea.
[42:32] We're just going to go here, go here. Can I delete this one?
[42:39] How do I delete-- - It's in settings, and it's--
[42:41] - OK. We're just going to--
[42:45] down the bottom? - Down the bottom, yep.
[42:46] You have to-- I would copy that whole thing, because it's
[42:53] like, you have to do your name and that whole teach-gen-tech slash--
[42:58] - Oh. Helps if I could read.
[43:00] - Oh, Lord, the 2FA. - OK.
[43:10] OK. We're going to get there.
[43:13] And y'all, I finally got access to my gengenod git. So I really should start using that, too.
[43:25] Because I thought I deleted it on here, and I didn't. And I am so lucky, because I thought
[43:31] I was locked out forever. - I made the stupidest username when I first started out.
[43:35] It was like, back in AOL days, I had this username that I kept for a very long time.
[43:40] And I made that as my GitHub username. So when I started getting serious about tech,
[43:44] I was like, I have to change this. And changing it in so many places was really annoying.
[43:50] But it was totally worth it. - Yes.
[43:52] I need to do that. I mean-- OK.
[43:56] I'm just going to copy it over later. We're not going to make us go through this now.
[44:01] OK. It was successfully deleted.
[44:03] I am just-- - Now you can create a new one right here.
[44:07] Don't-- yeah. - OK.
[44:09] So clear your-- there we go. OK.
[44:14] So now gh-repo-create, and hit Enter, and see what happens. Yeah.
[44:23] Push an existing local repository. Path is dot the same one we're in.
[44:31] And you can name it what we had it before. It doesn't matter.
[44:37] Now that it's deleted, it's gone. Wait, AOL.
[44:41] That's OG. I know.
[44:42] That's like a long time ago. I'm showing my age, people, back in the '90s.
[44:47] Yes. - Oh, my goodness.
[44:56] - Origin is fine. Unable to add remote origin because we already added it.
[45:00] But now if you do git remote-v to check what remote we're on, it should say the same URL that we had set.
[45:09] Yes. So that's correct.
[45:12] - So did it create it? - Yes.
[45:14] So it should be available on GitHub now. Your code may not have pushed up yet,
[45:20] but it should be created. I don't know if it automatically pushed it.
[45:25] - Well, let's find out. - Yeah.
[45:32] No, no code. So we need to push.
[45:35] So maybe do a git add, git commit init something. - Is it just git add?
[45:41] Oh, git add dot. OK.
[45:43] - Yeah, git add dot. Or you can do individual folders,
[45:46] but dot just adds all of them. Oh, this is the fun Windows stuff
[45:51] I haven't seen in a very long time. So these line ending warnings that you're getting are because--
[45:57] - Hover over Control-Click. Sorry.
[46:00] Yes, go ahead. I also was reading the comments at the same time.
[46:03] - Hover over the linkage. Oh, yeah.
[46:06] So you could actually Control-Click that, and it would open for the repo that it pasted the link.
[46:12] And you could Control-Click out of the terminal to get to the repo.
[46:17] - Just goes right there. - That's your path that you're in on your computer.
[46:23] But when we did the git remote dash v, it pasted the link. - Oh.
[46:29] - So you would have to scroll it back to where we were. Or do it again, either way.
[46:33] Where did we do that? Just above that, git remote.
[46:39] - Oh, this one. - Yeah.
[46:41] And Control-Click, and it will actually open it in your browser.
[46:43] But we need to push the code up. So that's where we were.
[46:49] So git add dot, and then we might have already done that. We did.
[46:54] And then I went off on my change about Windows because of all those line ending warnings.
[47:00] Dash m, and then a net or something, some more relevant. I'm always bad with git commit messages,
[47:11] especially if it's a project that I'm mainly just working on. I'm just like, I don't care.
[47:17] And then now, do that git push. But it's going to ask you to do git push dash dash set
[47:24] with no space, dash upstream, space origin, and then main. Enter.
[47:41] That work? I did it for my brain.
[47:44] I can never remember that. I always have to copy it.
[47:49] But it doesn't seem to be pushing anything either. - It's asking me to sign in.
[47:53] - Oh, OK. - Which is weird because I thought
[47:57] I was already signed in. - Yeah, it was doing it a minute ago,
[48:00] and now it's not working. Page has these instructions, step by step.
[48:06] She may want to use them in the process. Oh, yeah.
[48:09] So originally, that page that you brought up in the browser before you had--
[48:14] what was I going to say? Before you had the code in the browser,
[48:21] GitHub will actually tell you the steps that I just kind of walked you through.
[48:25] - Oh, yeah. I think where this was a little messed up
[48:30] is I tried to create the repo beforehand. And so my hope is that it's not going to happen again.
[48:40] - No, it shouldn't happen. And do you want to go ahead and--
[48:44] let's first install our node modules because I don't see them.
[48:47] So let's run npm i. Or if you don't want to use node,
[48:52] we could use something else. But I'm sure that's overwhelming you with tooling.
[48:56] - A? I?
[48:57] - Space. Space I.
[48:59] - Space I. - Yep.
[49:01] And that's just short for install. I'm doing all the bad things I tell myself
[49:06] not to do when I'm teaching people, is make all these shorthand things.
[49:10] And OK, so now we have node modules. So we can try to run the app locally with npm run dev.
[49:20] And that should open up at port 5173, which is apparently the new VEET thing.
[49:26] This is the Roman numerals that spell VEET. But 7 couldn't be done, so 7 was the closest to the T.
[49:36] - Yay. - OK, so we have a counter.
[49:39] And you can click the counter, and it should work. There we go.
[49:42] - So I have done not as complicated as I made it for us, but I have done this, where I'm like, cool, OK,
[49:51] so this is technically a web app, isn't it? Just a--
[49:55] - So yeah, so we're running just Svelte right now with VEET. And so this is all running on the client.
[50:01] We're not doing any server-side rendering. We're not pre-building and pre-generating our app.
[50:07] So it's all in-house. We're not pre-building and pre-generating our app.
[50:12] So it's all in the browser. So whatever browser you're using,
[50:17] the engine that runs the JavaScript is running all of the JavaScript needed to load the page.
[50:22] - Dope, OK, cool. - Cool, OK, so now we can deploy this as it is,
[50:32] or we can start diving into more Svelte stuff. - Let's dive in more.
[50:38] So you open up the SRC folder. And I like to close my terminal once I have it running,
[50:44] unless we need something in there. So I do that Control-Backtick.
[50:48] Again, we'll minimize it. And then you can pop it out whenever you need it.
[50:53] There you go. And so in the SRC folder, we have an assets directory.
[51:00] This is not how I really recommend-- I guess because it's an SVG, it has it in the SRC folder.
[51:07] But the public folder is actually where static assets go.
[51:11] So it's a little confusing that they have this here. I noticed this the other day when I was playing with this.
[51:15] But that's just an SVG file. The lib folder is where all of your Svelte components
[51:22] are going to be. So Anthony was talking about having that single file
[51:25] component. And that's what that counter.svelte file is.
[51:29] That counter.svelte file is just that counter component. That button that you saw is just that file.
[51:36] So that's a single file component. It's where you can take these frameworks or libraries
[51:41] and make these little pieces, chunks like Lego blocks, and build your app in those pieces.
[51:47] I would go ahead and enable it because there's a lot of TypeScript things that will not--
[51:57] it will give you little red squigglies if you don't do that. So I don't like little red squigglies.
[52:03] I don't blame you. And Homie has a question of an example of what
[52:10] would go in server assets. I really don't know.
[52:14] I don't know why assets is listed there. I've never used assets in a folder like that.
[52:20] I don't know what the benefit or the negatives are to even doing that.
[52:24] I always put them in the public folder so that they are available at build time, which I assume
[52:30] these would be, too, because Svelte is a compiler. So that's the first thing to learn about Svelte.
[52:35] That's what makes it a little different than React and Vue is that it compiles all the code.
[52:40] So it needs a build step, where React and Vue-- I think Vue is actually moving more towards this, too,
[52:47] where they're going to be compiling or they have been compiling since Vue 2, maybe.
[52:52] But React, for sure, uses a virtual DOM. Have you ever heard of the virtual DOM?
[52:57] OK, so in the browser is a document object model. That's the DOM tree that the browser
[53:03] creates to structure your site like a family tree. You can think of it like that, like the body and everything
[53:09] gets structured together. So the virtual DOM that React uses is a diff of that.
[53:14] So they copy it, and then they see what changes so that they can update the virtual DOM
[53:20] to the regular DOM. React takes care of that by loading React into the browser
[53:25] and doing those updates inside the browser. Svelte compiles during a build step.
[53:31] So when you put it on Netlify or wherever you host this app, there's a build step that actually
[53:37] compiles all of this code down into vanilla HTML, CSS, and JavaScript.
[53:42] And then the Svelte pieces are JavaScript, but they're done in a more surgical slicing way.
[53:52] So it updates the DOM because it knows everything that you've created when it was compiled.
[53:58] It can actually update things faster. And the bundle size is smaller because it
[54:03] doesn't have to have the library in the browser to do that. What you're saying makes sense.
[54:11] The part that I'm noodling on is I've also had someone on for Qwik JS 2.
[54:23] So I'm kind of like-- Was it Mishko?
[54:25] It was. You had Mishko on.
[54:27] Wow. OK.
[54:28] Yeah. So it's also trying to compile, putting all of that together.
[54:34] Most of the new frameworks are using this because Svelte popularized this compiler-based framework.
[54:41] And so Solid also does that. Qwik does it.
[54:45] Astro, I think, is a compiler, too. I mean, all of the newer frameworks
[54:51] are kind of using this. And the islands architecture, all of it
[54:53] is kind of just trying to make it faster so we're not loading. React is, I think, 128 kilobytes in the browser.
[55:00] So you put React in the browser to do this virtual DOM dipping, and you're adding 128 kilobytes of JavaScript
[55:07] that you don't need. Homie, am I familiar with what diff is?
[55:13] I'm going with context of-- so we'll see.
[55:19] But if I was picking up what Brittany was putting down, it's where diff is where it will see
[55:29] if there's changes in the JavaScript already loaded. And if there's a change, it will load it,
[55:36] which would cause slower load times because it's having to reload it.
[55:42] Where if it's already existing, it will just load what's already there that's cached.
[55:51] Where React does it in the web every single time, but Svelte compiles it before it even hits the browser.
[56:03] Yeah, so diff is basically just short for difference. So it's seeing what the difference is
[56:08] between what's in the actual document object model and what's in the virtual one that React is holding.
[56:14] And React does that very performantly. They do update the DOM quickly, but it loads more JavaScript
[56:20] up front to the browser. And you can create some of those things
[56:24] that you were talking about, like caching and server-side rendering static generation with Next in those meta frameworks.
[56:30] But if you're just using React like Anthony taught you, like the React beat, that's the same as this.
[56:36] It's just in the browser. Then what does-- could you explain,
[56:42] because I think I was kind of stuck on this question, what Qwik does?
[56:46] Because Qwik will only load what you're currently using instead of loading the full page, right?
[56:52] Yeah, yeah. And so I can't even wrap my mind around everything
[56:57] that Qwik does. But I've had Misko on our podcast too and talk to him about it.
[57:01] I've seen it demoed a couple of times. But from what I gather, it is compiled,
[57:06] and it runs everything on the server. So that means that you put it on a host,
[57:11] and everything is generated on the server. And then each of these single-file components
[57:17] that you're getting are dynamically grabbed from the server when they're needed, not beforehand.
[57:24] So it's all loaded asynchronously. And they do that faster, in Misko's mind,
[57:31] by serializing all of the HTML, or all of the JavaScript that's needed, into these objects
[57:40] that he puts on classes and IDs in the HTML itself. So you can do key-value pair matching inside of the HTML,
[57:51] which is-- that's like a bunch of JavaScript that even I
[57:55] can't wrap my head around, how they do that. OK.
[58:00] I don't feel like I'm going to build a framework anytime soon. No, me either.
[58:05] Exactly. Other people have fun with that.
[58:07] Just have fun. OK.
[58:10] So this does make sense. Dropping knowledge of all the things.
[58:16] I feel like that's the job a little bit, is that I need to know a little bit.
[58:21] So we use this T-shaped comb. Most developers have this T-shaped comb.
[58:25] But we're just like the full comb. We have a little bit of knowledge in everything.
[58:29] And we maybe have one that's a little bit longer. So it just goes across.
[58:33] Yes, I agree, homie. And I love that you ask if I know something, homie,
[58:38] that I'm like, ooh, do I? Because I think that's something that I struggle with,
[58:44] is I'm understanding what you're saying. Bye, Chan.
[58:51] Have a wonderful day. I almost thought you said you're going to lunch,
[58:54] because your name's lunch. That's amazing.
[59:02] So anyway, I love that y'all ask me the questions to see if I know it.
[59:08] Because I think I can understand what people are saying doesn't mean that I, A, remember the term, and B,
[59:16] know how to say it back to someone. So I appreciate these questions, because I don't always
[59:22] remember. That was when I started feeling like I was actually
[59:25] getting a grasp on things, is when you can explain it to other people.
[59:29] And I use this philosophy. I'm in the Learn, Build, Teach Discord server.
[59:32] And we go by the philosophy of learning it, building with it, and then teaching it to other people.
[59:38] And once you start teaching, you actually teach yourself, too. You learn more by teaching.
[59:43] I really should start putting this stuff in there. I just realized that.
[59:47] I'm in that. I don't Discord well, or Slack well,
[59:51] or I Slack off pretty well. But I don't use Slack well.
[59:54] Use Slack well, yeah. OK, so this is making a lot of sense.
[60:03] So let's look at that counter component real quick and see if we can actually break down what is going on here.
[60:07] So this is kind of the structure of a Svelte file. A .svelte file is basically a script tag, like an HTML file.
[60:16] Think of it. You have a script tag that holds your JavaScript.
[60:19] You have your templating, which is a superset of HTML. So you can write vanilla HTML in there.
[60:25] But you also have these things like that on colon click. And then the curly braces puts you into JavaScript.
[60:32] So it's taking HTML and giving it superpowers. So the on colon part of that is the event listeners
[60:42] that we get from JavaScript. So on click is a JavaScript API that we
[60:46] could call the function on. But this on colon is Svelte's version
[60:50] of that that does a lot of the stuff behind the scenes that takes care of the state management for us
[60:56] so we don't have to do as much work. And it does that by the equal sign.
[61:02] So the equal sign in Svelte makes a variable reactive. So that let count equals 0 on line 2
[61:09] is a variable declared count, is the name of it, set to 0. And then when we increment that count in the function,
[61:19] even though it's an arrow function on the next line on 3, we're incrementing that count by 1.
[61:25] And that plus equals is important. You have to set it again in Svelte.
[61:30] So this is one thing that does throw some people off. So if you're using array methods like array.push,
[61:37] and you're trying to update an array without actually setting it and assigning it to a new value,
[61:42] Svelte doesn't catch on to the reactivity. So its reactivity is based on the assignment.
[61:47] It needs the equal sign to actually update. And so that function is then being called
[61:53] in that onClick handler. And Svelte is doing the work behind the scenes
[61:58] of actually creating the JavaScript function for you so it's less boilerplate.
[62:05] OK, I have questions on that. First off, homie, did you hear me thanking you
[62:11] for asking questions? I see that you dropped.
[62:14] So I just want to make sure-- go back and watch that later, because I did thank you.
[62:19] Just want to make sure you know that. And something that, even as you're saying this,
[62:24] and my very, very first stream was about with Yere. And it was about CSS, JavaScript, and HTML.
[62:37] And it was to do something. And I actually ended up building it in HTML,
[62:40] because it made more sense than JavaScript. But you were talking about how this has HTML.
[62:47] Is there a plugin that will identify what each line is? Like, this is TypeScript.
[62:56] This is Svelte. This is HTML.
[62:58] That's a great question. I wonder if there's something out there that does that.
[63:04] I don't know off the top of my head, but that would be amazing.
[63:10] And I would be willing to come on your stream any time and help with that.
[63:14] Because I felt like that was really what I struggled with as a new developer,
[63:18] also, is looking at this stuff. It's like, what is happening here?
[63:22] Yeah, I can kind of-- I'm pointing at my--
[63:27] I know. I was just--
[63:28] --and see. I feel like I can understand what's going on right here.
[63:33] I'm like, OK, cool. That totally makes sense.
[63:36] You click on the button, it increments it. I could change the count plus equal to 2,
[63:41] and it would go up by twos. You always want it to load at 0.
[63:45] All of this made sense. What doesn't make sense to me, and I
[63:50] think this is a reason why I'm not partial to one framework, is I'm like, they all kind of look the same.
[64:01] Yeah. I wish I had a comparison here for you.
[64:04] So to me, what React confused me with is that it has to be wrapped in a JavaScript function.
[64:10] So you're having a JavaScript function, and then you're having your HTML in JavaScript, JSX.
[64:17] So JSX uses JavaScript to transpile the HTML, basically, that you're writing, so React can read it.
[64:26] And that flip in my brain from having to write JavaScript and then JSX and then flip to JavaScript,
[64:32] and it was too many mind switches for me. It's like I was trying to switch from HTML
[64:36] to JavaScript constantly, but this keeps them separated in my brain a little bit.
[64:41] So it helped destructure that for me. And then in the same format of writing an HTML file,
[64:49] if we created another file in that lib folder called HTML.svelte, we could just start writing HTML,
[64:57] and it would just work. If you don't need JavaScript, you
[65:00] could just write vanilla HTML in a Svelte file. I can copy the last tutorial from Free Code Camp for the Cat
[65:07] Photo app that they do. Even the HTML and the head tag and everything
[65:11] that shouldn't even be in a file, I can put it into a Svelte REPL, and even the form
[65:16] will post and work. Everything just works, which I can actually
[65:23] send you the link to that if I could find it. And I think I just closed it.
[65:26] I didn't mean to close you. I think at this point, it talks us
[65:33] through a bit of the beginning of it that-- I'm going to say you or someone else from Svelte
[65:41] ever wants to come back on. It would kind of be cool to compare it
[65:49] if, let's say, I just load a React app and be able to show them side by side,
[65:57] because that really helped with TypeScript. And to understand the differences, just so that way,
[66:05] A, it helps-- in my opinion, it really helps with understanding something
[66:11] when you're comparing it to something else. Where right now, again, I'm just like, OK, cool.
[66:16] Yeah, this is it. I get what you're saying.
[66:19] I'm just not going to know why or how it's different than React.
[66:24] Yeah, in that code, too, you can do a style tag. And that will allow you to do CSS.
[66:30] But it's actually scoped just to that component. So that's another thing that Svelte gives you
[66:35] is that your styling doesn't leak out unless you want it to. So you can style that button.
[66:41] And it would only affect the button that's in that file. But it uses a style tag.
[66:45] It uses vanilla CSS. So if you're writing an HTML file,
[66:49] you have a script tag for your JavaScript, a style tag for your CSS, and then your markup.
[66:54] And it follows the same patterns. Interesting.
[66:59] Interesting. OK.
[67:02] Anything else you think we should go through today specifically?
[67:06] No, I think that would be really good if somebody came back on or I came back on and did a comparison.
[67:12] Because having that, I see where that really helps. And I think you've helped me with my talk a little bit now.
[67:19] Because I know I made the React and Svelte side by side. Yeah, I would just say something like that,
[67:25] just to be able to see if I go-- I mean, y'all, let's see if I--
[67:32] this might help us a little bit for today. I'm not going to fully go into it.
[67:39] But this is why you have repos, if you can figure out where you're doing stuff.
[67:48] Did we push the code? I'm not sure, but I want to see--
[67:56] yes, this is back when-- OK, there we go, my React app.
[68:02] And source, source. I thought that was my--
[68:14] I have a command that opened a color picker, and I can't find it.
[68:18] Nope, that's the-- I might have deleted the--
[68:21] Oh, the React app? The counter.
[68:29] Oh, oh, did you-- in the SRC file, maybe? And there's no counter in there, yeah.
[68:38] Yeah, I think I deleted it. So yeah, I think if you're willing to come on the show
[68:43] again, I think it would be really fun to, A, also see if I can properly build the two of them,
[68:51] just install the two, and then we can compare them. I think that would be really, really fun.
[68:56] Yes, yes, we are learning all of the learning. And just to, as you so properly said--
[69:06] apparently, I'm having really fun, like having a lot of fun with resharing and unsharing
[69:11] and resharing. So can we add a scoped style, too, to that,
[69:15] so we have a change, too? Yeah.
[69:18] So in that counter.svelte file, at the bottom or wherever you want to put it, just add a style tag.
[69:29] Bye, Cynthia. Bye.
[69:32] Run Lighthouse on the two. I'm actually-- oh, a Lighthouse build plug-in for Netlify
[69:38] makes me so excited. So spelt sirens, the thing that I run or help co-run--
[69:44] I keep saying that. But we have speltsirens.dev.
[69:47] And the Lighthouse build plug-in lets you run your Lighthouse scores on builds on Netlify.
[69:53] And you can see your scores right on your deploy. So you don't even have to go to web.dev
[69:58] and type it in as an extra step. It just shows it on my deploy now.
[70:01] And I can see what each deploy's scores get on Lighthouse. That's cool.
[70:08] I was just going to say, y'all, I clearly cannot read, because I glance.
[70:13] This happens to me all the time. If anybody's wondering, this is something
[70:17] that happens with dyslexia. I saw run, so I thought she was running.
[70:22] Because even if I sit here and read the entire sentence, my head went to run.
[70:30] When Chan said bye, it read, he's going to lunch. Yeah.
[70:34] OK, so it's super fun, y'all. That's fine.
[70:43] It's very entertaining. But yeah.
[70:46] So on line 12, just do a style. So the little hashtag style.
[70:52] I said hashtag. Oh, my gosh.
[70:57] Less than. I'm sorry.
[70:59] Wow. If that's greater than, less than.
[71:05] It's lunchtime. I think the first one is greater than.
[71:12] Erase that first one. And then we should be good.
[71:17] And then in the style tag, so inside of the two there, hit Enter, and we'll go to a new line.
[71:22] And just say button, lowercase. Yeah, there we go.
[71:28] And curly braces. And we can just give it a background color,
[71:33] I guess, of teal, maybe. Just do something easy.
[71:38] Or blue-violet. That works.
[71:44] Save it. And then now we can push it to GitHub.
[71:51] You've already shut down the server, so we could see it if we ran the server again.
[71:55] That was-- it had it on a different line. That was kind of interesting.
[72:05] Why did you move it all the way over here? OK, whatever.
[72:08] I love it when it does that. And now we have a purple button.
[72:11] But if we created a button in a different component, it wouldn't grab those styles.
[72:16] That makes sense. And I don't know if that's accessible.
[72:19] Ben might still be here yelling at us. We could do maybe color white, and it would be accessible.
[72:26] Yes, yes. And I feel like, Ben's always in the back of my head.
[72:30] And I'm like, OK. So I do-- it's so funny.
[72:36] Because I'll post something, and I'm like, shit. I did not put something as the alt description.
[72:42] And then randomly, I'll be doing a GIF. That's good that people are there advocating for that
[72:48] and making you think about it, which is, I think, the important part.
[72:54] And so now, if you want to push all of these changes, we can shut the server down again and do get add.
[73:00] And we can get commit new spell tab or something. Ah.
[73:07] Did I do it right? Why do you look so weird?
[73:12] OK. It's because of the warnings that you're
[73:15] getting because of Windows. Oh.
[73:17] Those will pull away in Mac. OK.
[73:22] Windows has different line endings. So when you hit Enter on Windows,
[73:25] it's formatted differently than a Mac is. And so GitHub automatically knows that--
[73:31] or Git itself maybe automatically knows that and changes it.
[73:36] Do you have to do git-- wait.
[73:39] Did I do all of them? Did you do commit?
[73:42] Yeah, I just did commit. OK, so git push should work now because we've already
[73:46] done the hard one. And it's still a period, right?
[73:50] No, you don't have to do anything on that. OK.
[73:54] There we go. Now it should be up.
[73:58] Ah, this one. Maybe next time I can show you the Netlify CLI, too.
[74:02] Because I really love that I can just pull it right from my command line.
[74:05] It's so easy. Yeah.
[74:09] Yay. It's all there.
[74:12] Yay. Sweet.
[74:14] We have done it. We got through it.
[74:17] Oh, Cynthia posted the link for handling line endings, too. She may not want to worry about that, though,
[74:23] if you're getting your Mac back. No, I'm totally OK if I never touch Windows again.
[74:31] I will say it did teach me a lot. But I personally really--
[74:39] I just like using a Mac better. But it has a lot to do with small features.
[74:45] It's familiarity, too. You're used to using a Mac.
[74:48] So I get it. But I don't get random pop-ups.
[74:52] Like, if I go through my-- down below, it'll randomly pop up the weather.
[74:58] And I'm like, yo, my cursor just happened to be there. Don't do that.
[75:03] It's distracting. And then-- or I love the search on the Spotlight Search,
[75:11] and that I can get all of my texts on my MacBook. And I'm like, these are dumb things
[75:17] to be really grateful for. I think I have something that does the Spotlight Search
[75:21] on Windows, because I was trying to help my husband do something the other day.
[75:25] And I'm like, just do Command Space, because that's the same key combo on my Windows, too.
[75:31] And it didn't work for him. So I think I have an app or something that does that.
[75:35] Oh, yeah. That makes sense.
[75:37] That makes sense. All right.
[75:39] Anyone else have questions before we end today's stream? And please help me bug Brittany to coming back on the show
[75:50] again. Yes.
[75:53] I would love to come back on the show. It's going to be fun.
[75:58] And hopefully, all my stuff is working again. And then Apple did a great job tying us into their eco--
[76:05] Ecosystem, yeah. Yeah, yeah.
[76:08] I like what you did there, homie. I like what you did there.
[76:11] Because yes, yes, I am putting up with a lot. And I don't even know if I'm getting it back today.
[76:19] Hopefully, hopefully. I hope you do.
[76:22] Me too. Well, thank you, everyone.
[76:24] And tomorrow is going to be our mental health and neurodiversity and tech Twitter space, same time, every Wednesday.
[76:32] And Thursday, we're doing something. I should probably look at the schedule.
[76:37] I'll be somewhere doing something. You can find me somewhere.
[76:41] We're doing a live stream, but-- You can find me at VConf the rest of the day.
[76:45] I will be swollen at VConf. 9.45 PM tonight, I go live for VConf.
[76:52] Yeah. You told me you were going to take a nap.
[76:55] No, I probably won't take a nap. But I will take a break.
[76:58] I have three kids. So I have to take them to orthodontist appointment,
[77:02] library, busy life. Well, thank you so much for your time.
[77:09] Bye, everyone. 
