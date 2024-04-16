---
showLink: "https://www.youtube.com/watch?v=HIlgA9ScCLs"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-automated-deployments-and-testing-with-maciek-palmowski"
title: "Teach Jenn Automated Deployments and Testing with Maciek Palmowski"
publishDate: "2022-09-15"
coverImage: "https://i.ytimg.com/vi/HIlgA9ScCLs/maxresdefault.jpg"
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

[00:00] >> Hello, hello, beautiful humans. Welcome to another episode of Teach Gen Tech.
[00:08] Today we have, before the show, I asked him how to say his name.
[00:13] Now we're going to, because I started saying in my head, Magic, but it's magic.
[00:18] >> I mean, I like this version. I know that some people that
[00:23] have a problem pronouncing my name, which is Maciek. >> Maciek. If you say it,
[00:31] I feel like I can say it, but then after that, I can't wait.
[00:34] >> I even have a photo when I was at Starbucks buying coffee and they asked me for my name,
[00:41] and I have it written on the cup, Magic. >> Okay.
[00:47] >> It's official. >> I will say, I hate this.
[00:52] It's something that I've always struggled with, and I feel very,
[00:56] very fortunate for those from all around the world are patient. I hate that as Americans,
[01:04] we've cut it short for everybody. We give them nicknames and stuff,
[01:08] and I'm like, I don't want to do that. I just, it's frustrating, so thank you.
[01:14] I mean, I like magic too, but. >> But still, there are many good news.
[01:18] For example, I could be called Grzegorz. >> What is that?
[01:25] >> I mean, the cool part about Grzegorz that there is Greg, it's short for, Greg is short for Grzegorz,
[01:33] and Magic doesn't have the English form, so it's more difficult.
[01:40] >> Got it. Okay. Well, please introduce yourself as I got stuck on names
[01:45] and what we're going to be learning about today. >> Okay. I work as a WordPress Ambassador,
[01:54] so this is a typical DevRel role at the Polish company called Buddy.Works.
[02:00] We are working on a CI/CD application, so application that will help you automate all your deployments,
[02:09] and not only because you can do lots of different magical stuff if you just have some time and some ideas.
[02:18] Yeah, we're going to talk about automation because for most of my life,
[02:24] I was a developer before I became a DevRel. The thing that unites us and
[02:31] system administrators is the fact that we are lazy. I mean, I know that I always should say the word efficient.
[02:40] Many people say that using the word efficient rather than lazy sounds better,
[02:45] but let's be honest, it's not about efficiency, it's about this laziness.
[02:49] But this is the laziness that drives us forward and make us do different things thanks to which we don't have
[02:58] to waste so many time doing those boring, repeatable things. We'll talk about this, how to automate our deployments,
[03:13] and what in general the CI/CD is. I think this is just like the week.
[03:20] Homi and I had a call earlier today talking about a lot of this, just automation in life, just like everything,
[03:29] because I definitely am falling behind on a lot of stuff. Then also, earlier this week,
[03:35] we talked to Leo about data models. It's like figuring out that data model
[03:42] to find out what you can automate. I'm excited to learn about this because I feel
[03:49] like laziness is working smarter, not harder. Thank you, Homi, for joining me again today.
[04:00] What is CI/CD? CI/CD, yes, so this is one of those abbreviations
[04:13] that people in IT love to use to show how smart they are and that no one knows what we are talking about.
[04:22] This is cool, but in general, CI/CD means the CI part means continuous integration,
[04:28] which is just every time you push a change to your code, test it. That's it. The whole philosophy behind CI/CD is really simple.
[04:39] The CD part means two things, because it's either about continuous delivery or deployment.
[04:46] One means that every time when we tested our code, we prepare everything to make it,
[04:55] let's say, deployable. We're just waiting for a sign of our,
[05:01] let's say, senior developer or manager that, "Okay, let's release this today."
[05:07] But everything, every time the code passes the test, it's ready. We aren't in a situation when our code is ready,
[05:17] but we can't deploy it yet because we have to do something more. No, it's everything always prepared for it,
[05:23] just pressing the button to release it. Continuous deployment means that every time when the test passes,
[05:29] we are deploying everything automatically, just like this. This means we have to have our test suite really strict,
[05:39] really great, and we have to be prepared for it. It's difficult to achieve, but it's doable.
[05:50] On the other hand, there is nothing wrong in releasing everything manually,
[05:56] I mean, having designed to release it. But on the other hand,
[06:02] when we try to introduce CI/CD into our flow, sometimes the introductions looks a bit weird
[06:10] because sometimes we start with the CD part because it's easier to do rather than the CI part.
[06:16] And what is the most important about CI/CD, or let's call it really deployment automation
[06:21] because that's all what it is, it's not a tool, it's not a tool,
[06:27] it's not even not a tool set, it's a philosophy or a methodology of how we work.
[06:35] So we don't really, we don't need any tool for it. We could do everything just by remembering to run some tasks
[06:43] before pushing our code into the Git repository because that's it.
[06:48] But it's really important to be, first of all, very transparent with all the team
[06:53] because we are using, we have to use a repository and we have to be strict about the test
[07:01] and also we need to write them at some point. But the good news is, oh, and it's also very,
[07:09] what's important, it's like language agnostic. So we can use CI/CD in whichever language we write
[07:19] and it doesn't matter. And this was kind of a problem for me
[07:22] because I wanted to prepare something cool and I started wondering, yeah, but if I,
[07:27] I know that PHP is not so sexy anymore, so, and I'm mostly PHP developer.
[07:32] - We can try it, but really, really quick. - But I decided that I will show,
[07:38] I will show the also language agnostic approach, how to create part of our CI/CD deployment
[07:46] on the website that really, it doesn't matter in which it is written, we will be able to use it.
[07:55] - I dig it. And hello, Noelle.
[07:58] And okay, so continuous or CI/CD is continuous integration and continuous deployment.
[08:09] - Deployment and delivery, there are a few parts under the CD
[08:13] and it's not compact anymore. - Okay.
[08:17] I was just writing it and I was like, I just want to put it in the chat
[08:20] so I make sure everybody had that written out. All right, well, where does one start with CI/CD?
[08:29] 'Cause you said that not everybody can do the CI part, but may do the CD part.
[08:39] And what have been? - I see it like this because most companies start
[08:47] at one of two moments. First of all, thanks to the fact that
[08:55] if we're using some CI/CD application, it also helps us when it comes to security
[09:01] because this is this hub for which everything has to go. So we don't have to share FTP passwords
[09:09] and logins to users. So the moment when we have, for example,
[09:14] a breach or a person left the company and for some reason, some changes appeared
[09:19] on one of the websites he used because we forgot to rest his password
[09:23] or something like this. This is one of the moments when some people,
[09:27] okay, we need to centralize it and how to do it. And they learn, okay, maybe let's use something
[09:33] to automate the whole deployments. So we won't have to give away those logins and passwords.
[09:39] So this is one way. And the second one is the moment
[09:43] when we just deployed on production a major fuck-up rather than working code.
[09:52] So we try to learn, okay, so what to do, not to do it again, how to prevent it.
[10:00] How could we test it? How could we check it?
[10:02] And this is the moment when they probably start learning about some testing.
[10:09] And when they start about testing, they learn about the whole flow of CI/CD.
[10:14] - Interesting. - And sometimes it's all about,
[10:17] I mean, my way was with the laziness because at the moment where I started playing around
[10:28] with all those, with converting SAS into CSS, building JavaScript and doing many, many things
[10:39] before deploying code, it started to get a bit annoying to always prepare it locally
[10:45] and remember to deploy everything. So like I said, it's just boring.
[10:50] So I don't like boring stuff. - Real quick, a homie asked a question in the chat for Ben.
[11:00] So maybe Ben's still listening of if Ben's site is still using CI/DC tasks or flow.
[11:08] I asked, I wanted to call that one out because my question was also gonna be
[11:13] to everybody joining us. Like how well known is like CI/DC?
[11:19] Is it like, everybody kind of uses it on the down low or not really.
[11:26] Let's see. Ben did reply.
[11:31] - For sure, we have full-fledged CI/CD pipelines that take ages.
[11:37] For my posts. Sort of, yeah, exactly.
[11:41] That's it because we don't always have to run all the tests because we can run like gazillions of tests
[11:47] that will take an hour. But sometimes we just need a simple check.
[11:51] Okay, everything looks as it looked like and we can deploy it.
[11:55] That's it. And it's working after deployment.
[11:57] So sometimes it's very simple. It's, yeah, it's not the full CI/CD methodology,
[12:02] but we automated it. We automated it enough to not worry
[12:07] about what happened after us pressing the deploy button. And if something goes wrong, we'll get, I don't know,
[12:13] email or message on Slack that, "Yeah, something go wrong.
[12:18] "Go back to your computer, fix it." - I mean, that's probably what Zoom is feeling.
[12:24] I feel like Zoom had an outage. I heard they had an outage today.
[12:29] So it was like something happened that they couldn't check or something.
[12:35] - Yeah, I read about it. Yeah.
[12:38] - It's crazy how quickly news spreads when something that is so used,
[12:46] like everyone knows, like if Slack goes down, you know, there's, I'm interested.
[12:54] So would something like CI/DC help prevent any bugs going out then because it's being checked
[13:02] or can things still pass through it even if you ran all your checks?
[13:06] - Of course they can because someone has to write those tests and we are human, so we are making mistakes.
[13:12] So it's more important right now is to find what was the problem,
[13:21] why the bug went through and fix the test. So the next time when we'll make a similar mistake,
[13:29] it will be caught before pushing. Yeah, because I'm sure that all those enormous companies
[13:37] like Slack, like Zoom, like Microsoft, thanks to CI/CD, they are preventing
[13:44] like at least few times a day, a deployment that would crash and burn
[13:51] the moment when it reached the final server. And everyone will be like on Twitter,
[13:56] "Hey, Microsoft isn't working again, they messed it up." And I'm sure they're preventing it
[14:03] like really many, many times. The thing is that still we have to write some of those tests
[14:10] so it's still likely that something will go wrong or sometimes the infrastructure will go wrong.
[14:15] So, and there is also one thing and this is something that I can't wait
[14:21] because I will be doing a webinar in a month about this because there is a huge segment
[14:26] of automating manual testing because there are things that only humans can test
[14:32] in a proper way because automated tests will have some, let's call it, they will be a bit flaky.
[14:40] We will be never sure if it was for sure working or kind of not.
[14:45] So it's also a whole segment of automating the human test. So in general, testing is such a wide area.
[14:55] We can like test everything. We can start with those simple things like automate,
[15:02] for example, if our Lighthouse score went up or down because it's a great thing to check, right?
[15:09] If our Lighthouse score went down, maybe we shouldn't release it
[15:14] because something is wrong with our code. We can compare screenshots of our website
[15:21] before and after the deployment. So we can check if our small change in CSS
[15:26] didn't break something on the other hand about which we forgot.
[15:30] And thanks to something like this, we can see that there is a difference
[15:33] and we didn't thought about it. So we can block the release.
[15:37] We can, yeah, there are many, many things we can check. We can check the behavior.
[15:44] So for example, if I will go to my website, click on the about section, click here, click here,
[15:52] it should show some, let's say H1 header. If it doesn't, it's a bug because it only should be here.
[16:01] And for some reason it wasn't. And it's also great that there are so many tests
[16:07] that we can run like only by providing, I don't know, a URL or just clicking some stuff.
[16:15] - Interesting. - I will show how to use, for example, Ghost Inspector.
[16:19] This is something really remarkable how easy it is to create those simple end-to-end tests.
[16:25] So, I mean, we are really living in a beautiful world here. - Quick break from Ben saying,
[16:34] yeah, definitely bugs sneak in, but being able to run your linter and tests
[16:40] every time you make code changes and then failing the build so you can't deploy it
[16:46] if your lint tests fail can keep you from a lot of bugs getting released.
[16:52] And another thing, the whole team can see the states of your CI/CD pipelines, which encourages transparency
[17:01] rather than only relying on Scouts Honor that everyone is running lint tests locally.
[17:09] And, oh, I like this way of explaining it. CI/DC as automated accountability.
[17:18] - That's true. That's true.
[17:19] And that is really true because, yeah, this is a totally different way of thinking
[17:28] about how we are working with our code. I remember that one company,
[17:33] we had a problem with one developer who felt, in short, he didn't felt well
[17:41] about the fact that his code had to be checked. It had to be reviewed.
[17:48] It was checked by those machines. He felt really bad about it.
[17:53] And at some point he just stopped working with us because he didn't like it.
[18:00] - Interesting. - Yeah, it's, I mean, it's another thing
[18:04] about talking about code review, the way how we are doing them.
[18:07] For example, I learned last week about something called blameless debrief.
[18:12] This is really interesting because this is also a bit connected with this.
[18:17] It's a part of this, it's called site reliability engineering.
[18:24] And this blameless debrief is, yeah, because bugs happen.
[18:31] We make mistakes. But when we are trying to find out what happened,
[18:36] we don't care about who did it. We are trying not to blame a person.
[18:41] It's more about why it happened and what steps we should do
[18:46] to prevent from it happening again, just like this. We are not concentrating on a person.
[18:51] We are just concentrating on the why. - Interesting.
[18:57] I am going to paste this into the chat. I just Googled it a bit.
[19:03] A few things that come to mind is the fact that, first off, linting, just I'm pretty sure,
[19:13] like tons of people probably know this, but to make sure I check, fact check my understanding,
[19:18] is linting is just something to kind of like the prettier app in VS Code
[19:25] where it just checks your code, are, do you have the right spacing?
[19:32] Is there a comma? Is there a semicolon?
[19:35] Did you close that bracket? Also have, are you, goodness, what is it called now?
[19:42] Where there's a, at least in JavaScript, where if you don't use that,
[19:55] I'm totally spacing what they're called right now. Not variable.
[19:59] - Constants and all those things. - Thank you.
[20:02] If you don't use your constant, it likes to freak out and be like, you're not using it.
[20:06] What are you doing? So linting is literally just making sure,
[20:09] like giving your code some guidelines and letting you know as you code that there's issues, right?
[20:16] - Yes, but still this is, and this is something that Ben mentioned.
[20:22] It's relying on Scout's honor that everyone is using it. That's why we always should add such a step
[20:31] in our CI/CD pipeline. So for example, every time we deploy code,
[20:38] one of the first steps, we are using prettier or linter, or if we are using PHP, we are using PHP code sniffer,
[20:47] something like this. It's like I said, different languages,
[20:49] different technologies, but they all do the same. And we are making sure that everyone did it.
[20:57] Because we, I know that we should trust people. - Right.
[21:02] - But on the other hand, we shouldn't trust people. - Yeah, yeah.
[21:05] It's like you trust people, but it's not because you don't think
[21:09] they don't have good intentions. It's because we all make mistakes, no matter what.
[21:14] - Exactly, because we are people. We are people.
[21:17] And sometimes during, I don't know, we are trying to release a hotfix.
[21:21] I don't know, something is happening outside because we never know.
[21:26] We, I mean, we very often judge a developer just by the code he pushed.
[21:32] And sometimes we don't know what just happened on the other end of the monitor.
[21:36] I don't know, his baby started crying. Something happened and he just missed something.
[21:42] And he just pressed push. And that's why we should check for it
[21:47] because it wasn't his bad intention. I mean, in most cases, I mean,
[21:54] if a developer is trying to push an error because he wants to push an error, that's a problem.
[22:02] But in most cases, they don't. They just want to release a good code.
[22:07] But again, we are humans. Sometimes we just stop thinking about something.
[22:14] We just make a mistake. - And Ben added this earlier
[22:21] that CI/CD isn't just about testing at his old job. Anytime they wanted to release,
[22:31] they had to submit a hella tedious form describing what the changes were going live.
[22:37] So tedious and no one wanted to do it by getting it wrong could lead to the team's risk
[22:44] of getting slapped. So we wrote a script that automatically submitted
[22:48] that form in our CI/CD. So all devs had to do was give it a once-over.
[22:55] And I find that interesting, but I, okay. - I can tell that I just, for example,
[23:08] when it comes to those scripts lately, because we know that we shouldn't release on Friday, right?
[23:13] So I lately wrote a small script that runs always before the deploy.
[23:18] If it's Friday, it's always failing. It's blocking us.
[23:22] Just a joke. - Oh, that's cool. - It's not only about testing.
[23:25] It's sometimes about those small things like this. - Interesting.
[23:30] I, and I will say it wasn't until this morning that I'm talking to a Android developer
[23:38] that I was like, I used to tell people in 2007 when Android phones like first got launched that,
[23:48] oh, it's open source so anybody can develop those apps. Y'all, I just realized this morning
[23:57] that I was talking about open source, like OSS open source. I was like, like mind blown.
[24:04] I'm sharing that because now that I've like seen GitHub and stuff like that.
[24:11] And like, as you're starting to explain CIDC, CICD, I'm gonna get the acronyms,
[24:21] is so how do people go in and submit these if like submit hacking things,
[24:32] if they have to be approved or if somebody does have CIDC, CICD.
[24:39] I don't know why that catches my curiosity so much. - No, no, but it's a very good,
[24:48] it's a very good and valid question because yeah, we can think of, yeah,
[24:52] we have all those automation, we have all those tasks and still some people are able to push something through.
[25:02] - First of all, many tests are just checking if the code is correct.
[25:06] - Oh, okay. - Because in most cases, we are writing a function
[25:14] or method, whatever. We are writing tests to check if it works correct.
[25:20] So probably there won't be any test that will check that yeah, someone is trying to download something
[25:31] from another website and it's a virus and something like this, not out of the box.
[25:35] Of course, there are services that are doing it. - Yeah, the way that I'm like hearing that
[25:42] is basically like these tests can check to see if I wrote my name, I am Jen,
[25:51] but they're not gonna catch it if it uses one N instead of two Ns
[25:55] 'cause technically it's correct, it is I am Jen. It's kind of how I'm hearing that as a way
[26:01] that the tests do it is they just check, is it correct, but not is it spelled right?
[26:08] - Or I would even say that, or yeah, this is one example. And another thing is that someone just submitted
[26:16] something totally different that doesn't affect this part. And this is the moment when we humans are so important
[26:27] in maintaining a project because the whole point of CI/CD is making us developers focus on what matter.
[26:37] So it's more important how to write an algorithm, how to create the idea behind,
[26:46] or when it comes to open source project to maintain and check if someone didn't just submitted
[26:56] a really horrible pull request that I don't know, delete our database or something like this.
[27:03] It's on us, on the human. But thanks to CI/CD, we don't have to worry
[27:08] about all those things we just automated. We can just focus on the things
[27:13] because every time when we are using this, we are using CI/CD when it comes to pull requests.
[27:21] First, we are running everything that is automated. So if something is broken,
[27:25] the user that submitted the pull request gets the line, "Sorry, there is an error in this task.
[27:33] Do something about it." So this person will either first try to make it working
[27:38] or will describe why he thinks that the test is failing because it's written in a wrong way
[27:45] because tests sometimes are also written in a bad way 'cause we are humans.
[27:52] But still, we have like most of the boring, tedious work done by a machine.
[28:01] We can just focus on checking out the code, seeing it, okay, this code really doesn't look good.
[28:08] Someone is trying to push something bad into our repository. We should just delete this pull request like this.
[28:18] So, but like I said, there are also services, if I remember the time, that are checking for security.
[28:25] So it's also changing in this way. So more and more things,
[28:32] because sometimes it's really hard to spot something. I mean, there are, for example,
[28:39] ways how to inject some really not nice code inside of a SVG file because it's JavaScript, right?
[28:50] So let's be honest, if someone would submit a pull request and one of its parts would be a SVG image
[29:02] that you are suspecting that should be there because of an icon that should be added,
[29:07] let's be honest, you will never, never check what's inside of the SVG file, right?
[29:12] Because yeah, it's an SVG file, it's great code. - All right, all right, I dig it.
[29:18] - And this may be the problem. And this may be the problem.
[29:20] So yeah, it's really all about making the machine take over the boring stuff, the tedious stuff,
[29:30] the things that we can miss. So we can focus only on the things
[29:34] that we know the machine can miss and that we don't have to worry about
[29:39] looking at like everything because we are just have a small portion left
[29:45] to check if it's okay. - Okay, I feel like I now have
[29:50] a better understanding about it. Now I'm excited to see like this in action.
[29:55] - Okay, so we are going to, okay, let me just move this as I will be looking a bit more here.
[30:06] Let's share the screen. It will be, okay, it's this one.
[30:17] Okay, can you, okay, that's perfect. So we are going to deploy
[30:24] and test this small little Astro site. So I will be using Buddy because of few reasons.
[30:34] First of all, I work there and I have access to it. So it's great.
[30:39] And on the other hand, Buddy has really one amazing feature. It has the whole UI and you don't need to worry
[30:48] about writing, for example, like selections, all those JSON files and anything.
[30:56] You can just click here and there and everything will be working.
[31:02] Okay, so I have this here deployment pipeline called just in case.
[31:07] So if I will forget something or I will have a place to go and see what I have messed up.
[31:15] I already connected my repository of this palmiac/webinar.astro.
[31:21] And it's nothing more than a simple static Astro website. Okay, so let's do some, let's start with the CD part.
[31:33] Let's start with deployment. So let's call this action deploy
[31:39] and let's set it that it will deploy every time we will change something in the master branch.
[31:48] So we don't have to even go later into Buddy every time when we will change our code,
[31:54] something will deploy. So, and we will deploy it to Netlify
[32:00] because everyone is using Netlify in GateGuide. So we have Netlify.
[32:08] If I remember when it comes to Astro, it will be this product log and we need this.
[32:14] I have set up some things that we will be deploying this folder into.
[32:20] Okay, but there is a problem. If we want to deploy an Astro website,
[32:29] we first have to build it. There is this.
[32:33] First, we have to install all the npm packages and then we have to build it every time.
[32:38] So we have to first add one more action called Node.js and we have to do something like this.
[32:47] We have to run two commands, npm install and npm run build. So what does it mean?
[32:52] That every time when we will change something into our repository, first, we will rebuild the whole,
[33:00] we will rebuild this folder and this folder will be deployed to Netlify.
[33:07] So let's change something in our code, right? So let's go into src, let's go to pages.
[33:15] Let's go into the index. Yeah, I will use the GitHub editor, it's enough.
[33:23] Hello, let's call it hello-cicd-astrolabs, right? Let's commit the change.
[33:33] And I push the deployment and you see it's already running. I didn't press anything here, it's running automatically.
[33:42] First deployment takes a bit longer, but we'll see what is happening.
[33:46] So right now, the Docker image was downloaded. We've built everything.
[33:53] We can see the whole structure that was built. And right now we are deploying the dist folder
[34:01] into Netlify. So let's, and here we have the website URL.
[34:11] So maybe it's, oh, I have this. So that caching, but it was simple,
[34:21] but it happens automatically. So every time when we will check something,
[34:27] if we'll change something, it will get automatically deployed to our server.
[34:32] Amazing. The problem is if we will mess up something,
[34:38] I mean, the good part is if we'll mess up something that probably the build action will crash.
[34:48] So it won't go further to the deploy. So it's okay.
[34:53] But let's start doing some, maybe some tests before those simple one.
[35:00] First, there is this really cool thing about Netlify that each deployment has this unique deploy URL.
[35:14] So right now, let's just go here to, we are using this proud if unlocked.
[35:21] So in short, we are deploying it on production, which is cool, but it's kind of not safe
[35:29] because we don't know. Because if we broke something, we deployed it to production.
[35:36] So that's why we are going to play around a bit with this, with the fact that Netlify is always providing us
[35:45] with those cool things here. And we can do something about it.
[35:53] So it will be great to get this unique deploy URL. So this is when a bit of coding is useful.
[36:03] So first of all, just a few, I will read. We have to install this library called jq.
[36:11] It's for parsing JSON files. And we are going to do something like this.
[36:18] I have it. So we will assign the deploy URL
[36:26] from everything we had there to a variable called deploy URL.
[36:32] And having this variable inside of body, we can pass it to different actions.
[36:39] But we have to first create one more small thing, but let's save it right now.
[36:44] And let's go back to actions and to variables. We're gonna create a variable called deploy URL,
[36:54] it's not hidden. And it enabled changing the value
[36:59] during pipeline execution. Because this is what we are doing
[37:03] in the middle of the action. So let's run it right now manually
[37:09] and see what will happen. Because one thing will, I mean, it should change.
[37:14] I hope I didn't break something. Because this is the cool part
[37:18] about all those live webinars. Every time when you are so sure that everything will work,
[37:25] you will mess up something. But I hope not this time.
[37:28] So yeah, the cool part also when it comes to, not only body because every CI/CD application
[37:37] works like this right now, that every step is executed
[37:41] in a separate Docker based container. So we can use different...
[37:49] Oh, and you see, we have added this deploy URL as this variable called...
[37:56] I mean, this URL is set as this deploy URL, which is cool.
[38:02] And now let's add something. Let's add something more.
[38:08] Oh, and one thing. You see, there is no prod if unlocked.
[38:12] So we are not deploying this on production yet. That's why now we are going to do a simple,
[38:19] let's say a Lighthouse, Lighthouse test. It looks cool.
[38:26] See, it's helping it by URL. And we have to be sure that our performance,
[38:32] accessibility, best practices, SEO score is better than 50. It's easy to pass.
[38:38] And because we passed it, so we won't be reaching production yet.
[38:42] So if the score will be lower than one of those values, our deployment will stop.
[38:49] So let's do it. And let's see what will happen right now.
[38:54] This will probably take a second. - So is Buddy Astro,
[39:03] like is Buddy a plugin for Astro? - No, no, Buddy is totally language framework
[39:13] and everything agnostic. We can use it with everything.
[39:19] - Okay, so. - In my cases, I use Buddy mostly with WordPress,
[39:25] but also with different frameworks. I have my website built on Statemik.
[39:32] So I'm also deploying it using Statemik. I'm also deploying Statemik using Buddy.
[39:37] So you can use everything you want with it. If there is a Docker image, you can run it.
[39:44] - Okay. I'm gonna send this link to you in the private chat
[39:48] before I send it out in the main chat, because if I'm reading this right,
[39:55] this is just talking through, because Astro is something that a lot of people use as well.
[40:00] - This is the link, the documentation I've written for Astro, 'cause I'm a big fan of Astro, so.
[40:07] - Okay, okay, so this is the proper link. - Exactly.
[40:11] - Okay. - Oh, and take a look. Astro is really fast, and we have this performance,
[40:16] accessibility, best practices, and what have. But right now, we didn't deploy it to production, right?
[40:24] Because we only, we checked if everything's, so right now, we should add another Netlify deployment.
[40:35] This time to production, we don't have to worry. It should be something, okay.
[40:42] So right now, between this and this, we can run all those different tests
[40:52] we want to check if we didn't screw something up. So let's add something more.
[40:59] Maybe it was called a screen, oh, it's called a visual test.
[41:06] Visual test is amazing. It shows out, so we will have to run it twice.
[41:12] But first time, we can set some options here, like the width and height of the screen,
[41:19] the pixel tolerance, whatever. But let's leave it as it is, the most basic comparison.
[41:26] So the first time. Oh, I see that someone asking
[41:34] about Netlify has a build plugin. No, we are using our own, and why?
[41:41] To be honest, I always prefer the approach to have all the heavy lifting in one place
[41:52] and use Netlify as just a hosting platform. So for me, I will always use,
[42:00] because it's imagined that at some point you have this really long CI/CD flow.
[42:06] You really done a lot of work towards it. It's working at some point, Netlify.
[42:13] Oh, and you are keeping all the CI/CD stuff inside of Netlify, you are not using body.
[42:17] And at some point, Netlify decided to change their pricing. And now you are starting moving everything.
[42:23] And right here, I have all the heavy lifting inside of body and I'm just deploying it to Netlify.
[42:30] If at some point, Netlify decides, okay, we will have a more expensive pricing.
[42:35] And I decide, okay, so let me move to, I don't know, clubs or pages or whatever.
[42:40] I will just change to actions and what the rest will happen as it was happening before.
[42:47] So I prefer to have everything as those small blocks that I can every time change a bit
[42:56] without worrying about the rest. So this is my approach.
[42:59] I mean, I understand that if the same could happen with raising prices on body or removing some features,
[43:07] but still, I would prefer to keep... I mean, I kind of don't trust all those hosting companies.
[43:19] Netlify is still a hosting company and I prefer to have the heavy lifting outside of it.
[43:24] Still, I like Netlify, it works really great. - Nice.
[43:29] Cynthia, did that make sense to you? Just to double check.
[43:33] - In the meantime, I will run it for the first time because like I said, we will need to run twice
[43:42] because first, it will take the initial screenshot and the second time we'll correct something,
[43:48] we'll change something in our code and we will see if we'd catch it as a,
[43:58] not as a bug, but as a change that we will have to approve manual
[44:02] because those visual tests are more about approving something or not.
[44:07] And yeah, visual tests can save. I mean, especially when you...
[44:14] I mean, imagine you have a website that have like four crucial pages.
[44:19] Let's say it's contact, it's about us and something else. And you should check those crucial sites
[44:27] every time with visual tests. So you are sure that the small change you added to a CSS,
[44:33] for example, that should only affect, let's say a cart page,
[44:40] by some reason affected one of those. You will be able to see it.
[44:46] So, okay, so we have this initial change and now let's go back into the code
[44:52] and let's change something in it. So, hello CI/CD astronaut,
[44:59] and maybe let's have, let's be professional, let's add an owl here, right?
[45:06] So let's commit the change. And it's running already.
[45:15] You can see it here. It's in progress, so we'll have to wait a second.
[45:24] Yeah, and also the cool part, while during webinars, it may seem that, yes, CI/CD is only taking time.
[45:31] Yeah, that's true, it is taking time. But when we are working with it every day,
[45:36] the moment when we push something, we just push it into our background.
[45:42] We don't have to focus on it. We can work on something else
[45:45] and we don't have to worry about it until the moment when it, for example,
[45:51] informs us that, yeah, you made a mistake. We should, you will get a slight notification, for example.
[46:00] I mean, this will be our next step. We'll add a notification for ourself that we did something.
[46:06] - So that way it really can run in the background without paying attention.
[46:11] - Exactly, exactly, and this is something so amazing that, yeah, I can just go and do myself a coffee
[46:17] and until I will hear my phone doing a thing or we did a, and this is interesting
[46:27] why it passed without, you see this is the really cool part about, oh, this is kind of weird, wait a second.
[46:38] Huh, interesting, yeah, I like this. I like this, like I said, always during the live webinars
[46:46] when something can go wrong. Let's see what happened here.
[46:54] Interesting thing that for some reason this action has problems with emojis.
[47:04] It's really great to discover a bug during a webinar, right? - Yes, I do have a like badge in at work
[47:16] on our community page that I'm the bug finder. - No, this is something really great
[47:21] because we can see that it should see the bug, but it, okay, so if you are not using emojis,
[47:32] which I will, like I said, check after the webinar because it's not the time, it should spot an error
[47:41] that something changed in there. - Okay.
[47:44] - And then we should get the option to approve or not because sometimes the change that happened
[47:51] that the screen change is something that we wanted to happen because we change the content, we change the colors,
[47:57] we change something. So let me just disable this.
[48:01] But I mentioned the cool thing about the Ghost Inspector. The Ghost Inspector is something really, really cool.
[48:07] It's one of the easiest way to write end-to-end tests without touching a line of code.
[48:16] So for example, let's go to our website. It also has this add-on that helps you record a new test.
[48:29] So you just record it by clicking from site to site. So let's go for it, let's record.
[48:37] So we are here, we went and go to the blog page and then we go to the About page, and that's it.
[48:44] That's it for now, let's call it NameWebinarTesting. And let's be part of the Astro Suite,
[48:57] and let's create a new one, that it's called also. Execute initial test from now,
[49:09] default to, okay, save. Okay, and now if we go into our dashboard,
[49:18] see our webinar testing, we can edit the steps. Because let's say that, because on About Me,
[49:30] we see that About Me is, let's inspect it for a second. It's a H1 headache.
[49:37] So we want also to check if, let's add the step and element text equals About, okay.
[49:47] So the step is added, so let's see if it changes, perfect. And now let's go into our body and let's add a new step.
[50:07] That is called, of course, a ghost inspector. I already integrated it and I can use another folder,
[50:15] the suite called Webinar, and I'm from more of the Ireland place, it's great, we don't have to worry.
[50:23] And the start URL, this is of course the great thing. We can use the start URL of the deploy URL that is passed,
[50:29] so it won't reach the production before we do this. Do we need anything else?
[50:36] No, we don't, let's add this action. So you know what, let me just disable the Lighthouse for now,
[50:42] it will be a bit faster. So let's run it again.
[50:46] And in a moment, we'll see that this ghost inspector gets, we'll start running, so let's wait a second.
[50:58] Yeah, like I said, it's much better when it comes, when it works in the background.
[51:03] Oh, I forgot about the notification, oh, next time. Yeah, this is, especially when I was doing
[51:13] some live workshops about doing it in WordPress, this waiting times, I had to be prepared for many, many,
[51:22] and we see that it's running, it's running, it was triggered, and let's see what will happen.
[51:33] Will it pass, or will it not? Let's go back into body, let's see here.
[51:39] Oh, it's like, yeah, we're sending data, so we are waiting. Yeah, this, like I said, this waiting part is always,
[51:49] always a bit annoying, especially doing webinars, because, and the cool part is when,
[51:57] at least there is a second person during the webinar, so you can chat about something.
[52:02] The fail, it failed, why? So let's go here, and let's see.
[52:07] Because, oh, because I messed up the test, right? Because I forgot, not the element equals,
[52:16] but it should be, sorry, my mistake, it should be h1 equals about, right?
[52:22] Let's see, and then we can, for example, run it again to see, yeah, let's run it again.
[52:31] And we can see if our test will pass this time. Yeah, because I made a mistake.
[52:37] I was looking for an element called about me rather than. - Instead of the h1.
[52:45] - Instead of h1, and let's be honest, the element about me didn't exist,
[52:49] so the test failed correctly. And this is also a great thing,
[52:54] because it shows that, yeah, it's working, it's working. And right now, let's go.
[53:00] - And I think this is definitely something that I'm gonna have to come back to later on, too,
[53:06] in the fact that it's good to know these processes, and that it's out there, yet at the same time,
[53:13] I haven't done any of it yet. So I'm like, I get it, but I don't get it.
[53:18] - And now look here. It failed again, but now I knew it will fail,
[53:23] because h1 text equals about me, and the found text was about me with a capital M.
[53:28] This is a small typo, but of course we won't be, in real life, we won't be writing something like this,
[53:38] but those tests will be different. And this attention to small details, it's important.
[53:44] When I was typing about me, did you remember that there was a difference in characters?
[53:53] Of course not. - No. - Of course, and that's important.
[53:57] And right now, we should either correct our code, or correct our test.
[54:03] It depends on where is the bug. I think we should correct the code, right?
[54:08] Okay, so let's go here, let's go to the about, let's edit it, and it should be about me
[54:17] with a small M, right? So it will be, so let's commit the change.
[54:25] And right now, everything is running again. So yeah, the fact that something fails,
[54:30] yes, that's great, it's better. This is also the thing we always have to learn
[54:36] when it comes to CI/CD, because very often we think that if something failed, that's bad.
[54:43] No, it's great, because if something failed before reaching the production, that's great.
[54:51] We won't be hot-fixing something on production, like hearing, for example, our boss screaming at us
[55:00] that our website is down, or it has bugs, or something like this.
[55:06] We are keeping everything out of production, so this is amazing.
[55:12] I mean, that's great that we are having bugs. So then when we go, and it's running?
[55:20] Oh, it's still sending data, so I don't know how to scan, so let's go here.
[55:27] Oh, it passed? Oh, it passed, so we have the H1 about me, so.
[55:36] Okay, it was that easy to create a simple test. And of course, we can do much more using the Ghost Inspector
[55:47] because it has unlimited possibilities. So you see, webinar passed,
[55:52] and then we deployed everything to production. So, and until it passed, it was prevented,
[56:00] so this is the cool stuff. I mentioned about notification, right?
[56:05] I will just show it because here we have a possibility to run different actions,
[56:13] because on run is when everything is okay. On failure, so every time when, let's say, something fails,
[56:20] we want to send ourselves a Slack message. Yeah, I think I have all those.
[56:31] Oh, yeah, let's say to random. And every time, it's kind of interesting
[56:39] because right now I'm not using Slack at the moment, but if something would fail,
[56:44] this general channel would get the message that body execution that started by me failed.
[56:52] - That's smart. - Let me just add this action to see, so.
[56:57] And we can, of course, also add an action that when everything goes back to normal.
[57:04] - Right. - Because this is also a really cool thing that we can do,
[57:09] because here, all our changes run at the moment when either we run it manually
[57:16] or when we push a change to our code. But we can also create a pipeline
[57:21] that will run on schedule. So for example, it will run every five minutes.
[57:28] So we can build a very simple uptime robot, just like this. So let's do it, right?
[57:38] - All right. - Let's build ourself, we did it, one, two, three.
[57:41] Oh, robot, cheaper. Okay, and we have this cool thing here called,
[57:53] if I remember, it was, because we have quite a few of them, it's called website monitoring.
[58:00] And we can pass the URL, what was the URL? This was this one.
[58:08] - I like what Cynthia said, fail fast. - Exactly.
[58:13] - And that is such a true point. And then Homie said, these checks will really help
[58:18] 'cause small detailed syntax typos cause big and bigger problems.
[58:22] This is super interesting, the GUI looks intuitive. - Oh, thank you, that's really,
[58:29] I mean, I really often wonder how Buddy was born because I know that the guys behind in the dev team,
[58:39] there are real nerds that they, I think that they are mostly using CLIs and everything.
[58:46] At some point they decided, yeah, let's make a user-friendly tool.
[58:51] Oh, and apart from the URL, we have this really great thing, check for string.
[58:56] This is one of the, at least for me, I think it's one of those very useful
[59:02] and important things to always add because it is possible to deploy a website
[59:08] that will return a status of 200. So it means that that website is in theory working,
[59:15] but for example, it's blank. For example, it's blank.
[59:19] So let's be sure that our footer is always deployed. So we know that it always should consist
[59:28] of these frames, right? So this means that the whole website rendered
[59:34] at least until the footer, so. - Interesting, okay.
[59:38] - Quite useful. So we have it.
[59:40] So every five minutes it will, we can already see the countdown,
[59:44] but we don't have time to waste. So let's run it, let's run it manually.
[59:50] Yeah, it was that quick because it just downloaded. It found that your name here was on the website.
[59:58] So we don't have to worry. And of course we should add into our Uptime robot
[60:04] an action that on failure, you know, send us a notification, send us a email, whatever.
[60:13] It's really up to us. I mean, really sky's the limit.
[60:18] I can say that one of the, oh, let me show you because when I was having those workshops for WordPress,
[60:28] the pipeline that I showed here was that long. - Oh, wow.
[60:35] Yeah, I think even at this point, because I know we got to wrap soon,
[60:39] is that it's something that once I build more, I think I'll be able to comprehend it a lot more like.
[60:49] - Because this is the most important part. I mean, we can stop sharing already
[60:55] because I will go back more. - There we go.
[60:58] - Okay, so because one of the most important things when it comes to CI/CD is really go step-by-step.
[61:06] The worst thing you can do, yes, let's add everything. Let's unit testing, end-to-end testing,
[61:13] whatever checks we have. If you try to add everything at the same time,
[61:19] you will probably fail because it's not that easy to do it at once.
[61:24] - Yeah, I think even just checking, trying to add some random checks,
[61:31] and I feel like that's something that I could at least try to test now
[61:35] just to get in the habit of testing, yet. - Exactly.
[61:39] - So at the same time, I'm like, this is such a big concept. This is gonna take me some time.
[61:44] - But you use one of the most important words, habit. Developing a habit.
[61:51] - Yes. Really, CI/CD is simple
[61:56] when it comes to the whole concept. It's really that simple.
[62:01] On the other hand, it can get complicated the moment when we,
[62:05] with how the project grows, with how many tests we have and everything,
[62:11] but still, the concept behind is still simple. And having this as a habit,
[62:18] it's the most important thing. It's about not to, I don't know,
[62:22] deploy everything using FTP or some files in LA or everything.
[62:26] It's to have a script, a set of actions that will always work in the same way.
[62:32] And if you will have one script, you will probably at some point create a template out of it.
[62:37] When you have a template, you will start cloning it for every website you have.
[62:41] And at some point you realize, yeah, quite often I have this and this mistake,
[62:47] so maybe I should add a check for it. And at some point after, I don't know,
[62:52] a year or something of adding those small checks, you realize I have a quite long and detailed pipeline
[62:59] that checks many, many things for me, and I don't have to worry about it.
[63:04] At the moment when someone say, hey, could you deploy using files in LA?
[63:08] And your reaction will be, what, without any testing, without anything?
[63:12] - Right, right. - Because it will become one of your habits.
[63:16] And it doesn't matter what applications you will use. It's really most about this.
[63:21] Like I said, it's a methodology, so it's all about habits,
[63:24] about spreading this across the teams, that's it. - I think that's one of the hardest ones
[63:31] is when people are coming on and we need to talk about theory.
[63:35] Like the same with some of the theory, gosh, now I don't even remember what they're called.
[63:43] Yeah, like theories I think are harder to conceptualize and until you get to that point,
[63:49] but being aware of them beforehand helps you get through them when you get to them.
[63:54] So thank you once again for being on the show. And I'm also really excited
[64:00] because I feel like this could, Cynthia, maybe one day if I can convince Cynthia to do it,
[64:07] is gonna come on the show to talk about creating a Discord app.
[64:14] And I think that's something that like, we could tie this into, you know, even if--
[64:20] - Of course, because I can also tell you that we can have a notification on Discord
[64:25] so we can connect the things or we can prepare the whole deployment
[64:29] of those Discord applications using a CI/CD. - Exactly.
[64:33] - There are so many ways we can connect everything with everything.
[64:37] I can tell you that one of them, yeah, it was one of the stupidest thing I did
[64:44] when it comes to CI/CD or the most smart idea. It really depends on which way you look at it.
[64:51] I created a pipeline and I connect, and after everything run correctly,
[64:59] it pinged this application, IFTTT, something like this, it's for automation.
[65:05] And it played the Eye of the Tiger on Spotify on my mobile phone.
[65:09] So every time when everything went great, it played Eye of the Tiger on my mobile phone.
[65:16] - Okay, that's fun. Now I just, ah.
[65:19] - It was horrible after the first time, really. Because when you heard the Eye of the Tiger every time,
[65:27] it's, I mean, it's one of the best ideas you can have. But it shows you that, and this is also great
[65:34] because we have so many APIs right now. We can connect everything with everything.
[65:40] We can connect what's virtual inside of this testing thing. And after, we don't only have to deploy something.
[65:48] We can, I don't know, connect it with our Philips Hue light and it will light up.
[65:54] - I was just thinking about that because there's Ian from Postman.
[66:00] He's created lights in his background. I'm like, that's cool, I wanna do that.
[66:05] So someday I will. And thank you, Magic, for coming on today.
[66:11] It was magical. - Oh, thank you, thank you.
[66:14] And especially this bug we discovered all together. But that's great, that's great.
[66:21] This is the beauty of live webinars. We are all learning.
[66:25] We are all learning from our mistakes and, yeah. - So much learning, so much learning.
[66:31] - So much learning, exactly. - Well, thank you again.
[66:34] And y'all- - Thank you for having me, Faye. - You can find his Twitter over there.
[66:39] Go follow, ask questions. Yeah, it's always weird to point at our things.
[66:46] So, well, thank you all. And you, as a heads up for everybody,
[66:53] no live stream tomorrow, Monday or Tuesday. So I'll be back next Thursday.
[66:58] Next week is Denver Startup Week. So I'm gonna be in person at Denver Startup.
[67:04] But if you're in town, come hang out. - With real people, amazing.
[67:09] - Real people, real people, not online. I'm gonna be with real people.
[67:12] Everyone's real, just internet buddies versus in-person buddies.
[67:16] Thank you all, bye. 
