---
showLink: "https://www.youtube.com/watch?v=8QEbdZm-qvg"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "try-to-teach-jenn-typescript-with-guest-jacob-evans"
title: "Try to Teach Jenn TypeScript 😅 with guest Jacob Evans"
publishDate: "2022-09-01"
coverImage: "https://i.ytimg.com/vi/8QEbdZm-qvg/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Once again, thank you for joining Teach Gen Tech.
[00:07] Today, we have Jacob on the show. Jacob, please introduce yourself
[00:13] and what we'll be learning about today. >> Hi, I'm Jacob Evans.
[00:19] It's there in the name. I'm also a little sick right now.
[00:26] If I look a little haggard, that's the reason and if any of you watching know me,
[00:33] I'm lying. Anyways, we're going to be learning about TypeScript.
[00:40] I work at Cloudflare as a software engineer. I particularly work on the Cloudflare workers team
[00:49] on the workers CLI called Wrangler. It's written in TypeScript.
[00:57] The way that Jacob ended up on the show, me crashing Friday night like code in life Twitter spaces,
[01:07] and one day it just came up. It's basically what happened and he got stuck being on the show.
[01:16] Hello, Ben and hello, Anthony. Anthony was the second episode
[01:24] and he was teaching me about React. It's definitely something that I feel like I've heard of TypeScript,
[01:38] but I'm still like, "Dude, it doesn't make any sense because everybody
[01:44] tells me how hard and difficult it is." I've heard that a lot.
[01:50] That's all I know about TypeScript. I don't know what TypeScript is,
[01:54] I don't know what it does. I know I think I know that it's something JavaScript,
[02:00] and that it's really difficult and hard to learn. That's what I know about it so far.
[02:07] >> There's a lot of half-truths in there. >> Okay.
[02:11] >> All right. First off, it's what's called a superset language.
[02:18] It is JavaScript at the end of the day. If you remove the whole type system,
[02:24] you have JavaScript, which is what the TypeScript compiler will actually do.
[02:35] It will strip out all the types and leave you with JavaScript to run. Most people don't see that part anymore because of
[02:46] a lot of the tooling and systems in place. I should describe what a type is.
[02:54] That's fair, AJ. >> Hello, Bakari, as well.
[02:59] Yeah, what is a type? Let's go to the bare basics. >> Yeah. It is a way to
[03:09] describe what a thing is inside of the language. You generally have something called primitives,
[03:21] your very lowest level. Thanks, AJ. Just giving out great comments.
[03:36] The primitives are very lowest level in a language. You have things like string.
[03:44] You have things like a Boolean, which is true/false, your one and zero.
[03:51] You have also things that are slightly above the primitives. Well, let's just stick with those for now.
[04:03] We have things like the object, the symbol, the Boolean, the string.
[04:09] I'm missing some, but this isn't an interview. Well, a job interview.
[04:17] Those things we can infer based off of word coding. If I'm writing const,
[04:29] this is a string equals quotations. Those quotations make it a string.
[04:36] I can put a big old sentence or paragraph in that single string. Without TypeScript, if I just did that in JavaScript,
[04:53] JavaScript doesn't care about that until you really are running the JavaScript.
[05:05] Then it will throw error if it's like, let's say you write a bunch of stuff out and there's not quotes around it.
[05:17] It's not a string. Let's see what Ben Myers say.
[05:23] One way to think about it is that types. No, go ahead.
[05:27] Feature. Types is that they define all the possible values a variable have and it excludes values that aren't permissible.
[05:35] Yeah, that's an excellent way to think about it. I also Googled it and a convenient way
[05:44] to refer to different properties and functions that a value has. A value is anything that you can assign a variable,
[05:54] a number, a string, an array, an object, and a function. That is from typescripttutorial.net.
[06:04] Nice. Yeah. First off, Ben, the typos or grammars are okay.
[06:11] We're all human. We're going to make mistakes. It's okay. What you said about the types though was a banger.
[06:22] You nailed it. Yeah, so besides primitives, we have like what was mentioned just a moment ago is like arrays,
[06:32] functions, these also could be typed. The awesome part about having those things when you're coding,
[06:49] is the information, the feedback you get when you're trying to code a bunch of stuff out. You don't want to have to hold all those things in
[07:12] your head while you're trying to solve these complex problems. It's like cognitive load that's just taken off of you,
[07:28] and now handled by the type system. I was also real quick because I didn't want to not say hi.
[07:39] Hi, Mac. Thank you for joining. We are inching towards three average viewers.
[07:45] We are slowly, slowly getting there. What's up, Cynthia?
[07:49] Thank you for joining. Let's see. Oh, so Anthony,
[07:58] the link that Anthony shared. Let me grab that really quick so I can share my screen.
[08:08] Let me click and make this. Oh, well, you just made it pretty.
[08:22] But it is cool going through the rest of it on what is TypeScript. Yeah, I don't know why I gave the random stuff at the end.
[08:32] Mackie, always a start, has net new viewers across all streams, Mac.
[08:37] Okay. Well, I don't know if I should believe you because we haven't met yet. But then also, I'll go be a viewer,
[08:49] share the knowledge and wealth. But back to TypeScript.
[08:56] Back to the TypeScript. When people first get into TypeScript,
[09:05] what is the reason that you would use TypeScript again? Yeah. The funny thing is,
[09:12] is the TypeScript docs themselves are not great for entry level. They're focused on the type system and trying to get
[09:29] people just giving them all that very technical reference information. Whereas the initial strength value of TypeScript just comes
[09:45] from when you change the file from JS to TS, you get a lot of these just inferences and hints and auto suggestions.
[10:04] The other part that was a big overhead for a lot of people initially, was setting it up.
[10:18] There was a lot of setup steps, like you have to understand enough TypeScript to set up to the TS config.
[10:30] You needed to also understand the build step, or the compile step between the TypeScript to
[10:50] JavaScript and what you were doing there with that configuration. But most of those problems in recent times have disappeared.
[11:06] Most frameworks, most bundlers, a lot of tooling out there handle all that for you.
[11:17] They could still hand off the reins so that you can further tweak the environment as necessary.
[11:26] But you don't have to understand every little aspect of how TypeScript needs to be configured,
[11:39] to just start getting the value of TypeScript immediately. >> Couple of questions there and some keywords. What up, Nick?
[11:53] >> I didn't get that. Could you try again? Siri would like to say hi as well.
[11:59] >> Greetings. >> Greetings to Siri.
[12:02] Something that I think that I need to take a step back on that I wish I understood and I think is a missing picture for me is,
[12:13] there's compiler languages and then there's not compiler languages. I don't know what the difference is,
[12:22] but from what I understand is compiler languages are a lot more complex to you.
[12:28] I don't even remember if this was a stream or a meet-up. Yeah, a stream or a meet-up that I learned about this.
[12:38] >> This comes back to the unnecessary cognitive overhead. You, for instance,
[12:58] you don't have to understand how the L1 cache on your motherboard works to leverage all the value of your PC.
[13:18] But some people really care about that stuff and those people also tend to make really cool tools around that stuff.
[13:30] But unless you're planning on making those tools or you just want to learn that stuff out of curiosity,
[13:37] it's not necessary to get that in depth to use TypeScript. Again, at the end of the day,
[13:49] all the TypeScript compiler is doing is taking the types and removing them and you got JavaScript.
[14:03] The funny thing is you could just write JavaScript in the TypeScript files without any of the little colon,
[14:16] assigning a type or the interfaces or the type keywords, and you're still going to get a ton of benefits from TypeScript.
[14:31] >> I feel like to put you on the spot, can you share your screen and go through some of the differences that you would see
[14:42] on let's say a visualization of what you're describing? >> Yeah.
[15:09] >> Because I feel like that's a hard part of it too, like I'm picking up what you're putting down,
[15:15] but like when we were in that Twitter space yesterday, that what Theo is describing with the funnels,
[15:22] I was like, "I get it, but I don't get it," and that image really helps solidifying it.
[15:29] >> Yeah. >> Now I put you on the spot.
[15:38] >> All right. You should be able to see this. >> Zoom it in, please, so we can see it.
[15:47] >> That's the opposite. All right. So this is some of the TypeScript stuff you would normally see.
[16:03] It's somewhat simple, but on the right here,
[16:09] you see that it's getting turned into just basic JavaScript. So let's see if I can wing something here.
[16:25] Just use this instead of re-typing everything. I'm watching on my full screen where it's much bigger,
[16:50] so I can see this. So oddly, and I don't know if it's counting to the numbers or not,
[16:56] but I'm literally watching the stream to see the fonts. When you get a chance,
[17:07] can you make it a little bigger, please? Also dark mode might help, per Anthony.
[17:14] This has dark mode. Does it have dark mode, Anthony?
[17:20] Do you know something I don't? Yeah, there we go. All right.
[17:30] >> Can you zoom it in? I feel like it just deleted the zoom that you've just had.
[17:36] >> No, it's still zoomed in quite a lot. Yeah, it's like 175 percent.
[17:46] >> Yeah, as long as I'm looking at the other screen, I'm good. So let us know, everyone.
[17:53] >> All righty. So something super basic here is I'm writing JavaScript here.
[18:11] It's still JavaScript over here. If I do something where I'm like,
[18:17] "Hey, this is a number," which it could already infer, it's still JavaScript.
[18:25] It doesn't change what this was. We just get more information from the system,
[18:40] from the tools you're using. So if I don't assign this,
[19:01] I've now changed what this could be. I could also, I think,
[19:08] omit this and it will still infer that. No, it doesn't.
[19:13] It just knows that you're going to make it a number. So that's a perfect example of I could tell it what it's going to be.
[19:29] So count is going to equal some sort of number, and it's happy about that.
[19:38] It's like, "Cool, that is a number. You could do that."
[19:42] But if I said, "Hey, I want to make you a number."
[19:48] Actually, let's do better. Let's do this. Suddenly, it's like, "Nice try, bro.
[19:59] That's not a number." You even get there over here too.
[20:05] That's cool. But the main thing here is you see that this is JavaScript. If I wrote this in JavaScript,
[20:16] JavaScript would just do this. That's what it would look like in regular JavaScript.
[20:23] So it's not going to yell at me. This is the simplest example to show the immediate value that you get from TS.
[20:43] >> We got a quick question. Is a transition from TS to JS done in browser,
[20:53] or is there a compile step of some sort? >> There's a compile step.
[21:00] >> Because we're using this TypeScript playground, that's why it's not showing a compile step?
[21:07] >> Yeah, that's happening for you here, which brings me back to my previous comment,
[21:17] which is most tooling is going to be doing that for you. Example, I work on the Cloudflare workers CLI called Wrangler 2,
[21:34] which is written in TypeScript, and it allows you to write your workers in TypeScript.
[21:41] But TypeScript can't run on the node runtime, which we have the workers edge runtime,
[21:57] and it uses node bindings and other compatibility stuff. Anyways, the thing is you can't run the moment I do this,
[22:19] this won't run in a JavaScript runtime because it's now a superset of JavaScript. It's something that sits on top of what's called the ECMAScript,
[22:35] which is the spec of JavaScript, and then they add all the type system on top.
[22:42] So it's built on top of JavaScript, it will never not be JavaScript.
[22:51] But they could do whatever they want with the type system because that's just taken away at the end of the day when it goes for that compile step.
[23:02] But with the workers, when you use that tool and you publish the worker,
[23:10] we do that whole compile step for you. You don't even know that that's necessarily happening.
[23:18] You just are writing TypeScript, getting all those benefits,
[23:23] and then sending your code up to run somewhere, and it magically is becoming JavaScript for you before it goes there.
[23:33] >> Really quick, what is a worker? Other than it totally made me think about minors or something like that.
[23:45] Then we have another question, does TypeScript also allow type checking at runtime or only at compile time?
[23:55] >> Yeah. So it's always compiled away.
[24:04] It's JavaScript that's running at runtime. To answer the worker question,
[24:16] are you familiar with serverless functions and the Edge? >> No. Because it's like,
[24:29] have I heard of them? Yes, I definitely have heard of it.
[24:33] Do I know anything you just mentioned? No. What up lunch?
[24:39] >> All right. I'm going to try to make super condensed answer. Stop it, AJ.
[24:52] >> I do know what a server is. I do know what a server is.
[24:55] >> Get out of here. That's hilarious. >> Yes. I got there.
[25:00] I'm like, Anthony, you basically know what I do know. >> That's so funny though.
[25:07] >> I do know what a server is. Well, I mean, on that note,
[25:11] how would I describe a server? >> AJ is pushing the limit.
[25:20] AJ is just like, how far can I go? >> If I were to describe a server,
[25:28] I would say the servers themselves are hardware that hold content. You could say, but when a lot of people are thinking about servers nowadays,
[25:43] they think about Cloud and AWS and those type of things, where they are Cloud servers,
[25:51] but they're still technically on a hardware server somewhere. >> Okay. AJ, I expect next,
[26:00] you're going to be asking how an electron works. >> Stop. I'm only joking with AJ.
[26:12] No, these are great questions. I would say it's a great answer,
[26:21] but I'm not like one of those must be super technical or they're overly semantic.
[26:34] But serverless, yeah, that's about right. Personally, I don't have a server in my room running
[26:47] a bunch of functions when somebody requests some information. But that has to happen somewhere if you're not running it or you're
[27:01] not using a hosted service that's doing it in one particular spot. What the edge is,
[27:09] is I don't want to just run it in one particular spot, or maybe even have a few major server locations globally.
[27:25] Maybe I want to have, yeah. >> I'm just pausing to get that response in there too.
[27:33] >> Yeah, no, that's great. The edge is basically running that code,
[27:46] so that serverless function on hardware, that's as close to the user as physically possible.
[27:57] Now, currently, that is usually running on things like POPs or Colos, which you can think of as the equivalent of electrical substations,
[28:14] where the electrical substations are things that are close to, say, a large neighborhood or whatnot,
[28:27] and it helps store and boost the signal of the electricity. POPs or Colos are also very similar in that way
[28:43] for networks and we can run code in those locations on that hardware, and that's generally was considered the edge.
[28:58] Now, the edge, at the end of the day, can be any hardware that's close to the user that's requesting the information,
[29:11] that's hitting whatever that serverless stuff is. I should probably close that. There we go.
[29:26] I hope you-all enjoyed looking at that very simple code snippet for 10 minutes. >> Wait, we do have a couple of comments
[29:38] and working on explaining this too. Cynthia says, "A web worker is a JavaScript that runs in the background
[29:46] independently from other scripts without affecting the performance of the page from Web3 schools."
[29:53] >> Yeah, that's not a Cloudflare worker. That is an accurate definition of a worker in the browser.
[30:05] Another one is, "Could a non-technical metaphor be like a local Amazon warehouses stocked with most commonly purchased items for that area?"
[30:16] >> French kiss, or was that chef's kiss, not French kiss. >> I definitely think that's a really good way of explaining that.
[30:29] I do think I missed. A Cloudflare worker is like a Netlify Edge function.
[30:39] >> Yeah, or the Lambdas on the Edge or Deno deploy. Cloudflare, Vercel's Edge functions.
[30:56] Yes, they do. Look, it happens to be that Cloudflare tried this out first,
[31:04] mainly because we had the Edge infrastructure for
[31:12] the other products that Cloudflare got really well known for, like the CDN and the optimized networking,
[31:21] and DDoS support, and stuff like that. >> I think the part that I'm like,
[31:29] so I get Edge, I get that part, but I'm missing,
[31:35] what is serverless again? Because aren't all serverless things still on the server somewhere?
[31:43] >> It's a tad bit of a misnomer. It's serverless for you.
[31:54] Say you're a company, normally, say like even 10 years ago,
[32:01] you would either be paying somebody else an exorbitant amount of money to be acting as your server,
[32:13] all the hardware that you need, the infrastructure for your products,
[32:19] whatever it is, or you would buy your own hardware and then eat the maintenance cost.
[32:29] Again, for the most part, pushing that off onto
[32:41] somebody else where you don't have the servers, that's the serverless part.
[32:47] >> I'm going to see if I can do a comparison based on my experience with GoDaddy.
[32:52] If somebody is calling in to GoDaddy and they want to get a virtual server, that's technically serverless because it's virtual,
[33:03] and Edge is where to pull the data, no matter where the datacenters are,
[33:10] Edge would be pulling it like if there's, I live in Colorado, so let's say GoDaddy is here and they had
[33:20] a datacenter in an hour away, they would do that before going to like Indiana to get the content.
[33:31] >> I feel like you mixed some Edge stuff slightly with some serverless stuff. >> Okay.
[33:44] >> Yeah. Again, like. >> Anthony said, running
[33:56] a virtual machine is a little different from serverless because you need to pick the version of Linux you want.
[34:04] It is technically. >> Yeah. That's the distinction between if you were to go do
[34:18] DigitalOcean or one of these other services versus in specific, I'm just going to write the code for the thing I want the server to do, and that's it.
[34:38] I don't care about the hardware at all. I just want it to do the thing.
[34:45] >> Okay. >> Infrastructure, back-end, well,
[34:50] let's not say back-end, but infrastructure, not something I'm going to worry about with serverless.
[34:57] >> Cool. Makes enough sense. >> I like the smartphones example as well as
[35:08] the breakdown of we're talking about three different things. >> I'm going to hit on that.
[35:19] The Edge currently does not involve IoT devices yet. Now, will we eventually run arbitrary code
[35:39] on IoT devices and maybe smartphones and the like? Yeah, for sure.
[35:49] But currently, the Edge is going as far as the equivalent of, somebody said, warehouses closer to the user or electrical substations,
[36:05] but not as close as literally in your hands. >> We went over what a server is, serverless.
[36:18] >> Type script. >> I'm going to bring it back to that.
[36:21] I'm going to bring it back to that, Edge. >> I love it.
[36:24] >> What is a worker? >> A serverless Edge function.
[36:34] >> Okay. Thank you. That's bringing it all the way back around.
[36:39] >> Full circle. >> Full circle on that one.
[36:43] Then could you re-explain what you would be using a worker for? Could you go through that again?
[36:55] >> You use them for just about anything you would do as a traditional server. They work particularly well with also webhooks and event-based things.
[37:11] They function incredibly well as proxies, middleware, all kinds of stuff. >> Okay. I feel like it's just not clicking,
[37:31] but this also happened the first time I was going through Python 2, where I was just like, "Dude,
[37:36] this is just not clicking at all." I'm thinking. I think just taking a step back.
[37:52] How did you first learn about TypeScript and having to understand it? >> Oh, boy.
[38:02] I went to a coding boot camp, which is they were teaching different level courses.
[38:29] Now, while I was there, what was popular was the Meanstack and later Mearnstack.
[38:43] So we got into the Mongo, Express, React, Node.js.
[38:56] One of the things that happened while I was there was this code editor called Atom that everybody was using,
[39:15] was the most popular thing at the time. It was like the open source,
[39:22] everybody loved it, it was extensible. Then I heard about VS Code because I was in Seattle when I was doing this coding boot camp.
[39:34] So people were going to meetups at Microsoft places and Amazon locations and all kinds of stuff.
[39:46] Somebody had brought up VS Code and I was like, "I like trying new stuff."
[39:58] One of the first things I noticed was when I hovered over certain things, I got this feedback from VS Code.
[40:11] I was like, "What is this? Why is it telling me this is a number or a string?
[40:20] I already know that." You saw that when I hovered over that stuff in the playground.
[40:27] Well, VS Code is written in TypeScript. So it will give you some of those benefits a little bit,
[40:43] the best it can, even in JavaScript.
[40:50] So I had just dug into VS Code a little bit more, looked into what was causing that extra information to show up,
[41:10] and found out about TypeScript. This is back at when, like four and a half, five years ago,
[41:20] when people were arguing if Flow was going to be the next big thing for types. TypeScript was just coming up in the conversations.
[41:43] So I learned about it through just serendipity. >> Through VS Code, kind of.
[41:57] >> Yeah. Just somebody is like, "Hey, have you heard of this thing?"
[42:01] I was like, "No, let me try it." Then I was like, "Oh, wow.
[42:04] What is this thing? Let me go look into that.
[42:06] Oh, what is this language?" >> I get that. I think one thing that I really struggle on,
[42:16] and I don't know if we have enough time to do it today, but I would want to follow up on,
[42:20] is I guess going through an exercise of seeing TypeScript to JavaScript, and what you were showing,
[42:33] because that's just a good experience on seeing it. But then for some reason,
[42:40] I don't even know if this clicks, but actually going through the process of typing it in
[42:45] JavaScript to get to the same point TypeScript took care of. Because from what I saw is TypeScript at least made
[42:55] it a bit more, how do I say this? >> Declarative?
[43:08] >> No, I don't know. If you write in TypeScript,
[43:13] is it smaller amount of text itself than if you write it in JavaScript?
[43:23] >> So yes and no. You can, as I showed,
[43:32] just write JavaScript if you want. But if you were to start adding the colons and defining the types,
[43:48] and then creating actual alias types, you're going to have a lot more text for sure.
[44:03] But that overhead usually comes later in much more complex systems where the inference
[44:16] from TypeScript can't always get the job done. You have to sometimes help TypeScript system know what's going on.
[44:26] That's where the creating your own types or inlining types come in. >> I think I'm just going to need to do TypeScript 101 again.
[44:42] Because this is something that it's very, very difficult for me to wrap my head around
[44:47] in all of the differences that build into TypeScript. >> Yeah.
[44:52] >> I will say beginner Python was way more confusing than the next time.
[45:01] I was like, "Oh, I'm starting to get it. Yay." I feel like this might
[45:05] just be another one of those where I'm just like, "This is a lot to take in."
[45:12] I will ask for everybody watching, what was your first experience with TypeScript too?
[45:19] Because is this something that people just start to get right away, or is it something that is normally pretty
[45:26] convoluted or confusing in general? Because I've heard that a lot with TypeScript.
[45:31] So I at least knew that going into it. >> Yeah. Like I mentioned before,
[45:36] the two pieces that usually cause that cognitive overhead at the beginning is
[45:46] people trying to understand the type system itself too much, like just jumping right into that deep end with no floaties.
[45:59] The setups and the configurations and whatnot that have now been like abstracted away by a lot of these frameworks and other tools.
[46:10] So if you come at it with just a thought of, "I'm just going to write JavaScript in this TS file,"
[46:23] that's a really good place to start. >> Interesting. All right.
[46:32] We do have a few comments of Roy was saying in response to Anthony, "You have to handle the typing,
[46:44] so that takes more, but you save on the other side by not needing to write checks."
[46:52] Interesting. Bakari said, "It's a learning curve even for experienced JavaScript developers."
[47:01] Thank God, because the stuff is like, I get what you're saying for not
[47:11] wanting going to the deep end of wanting to understand the types, Jacob. But I feel like at the same time, I'm like,
[47:18] "But I want to." >> That's a personal choice, Jen.
[47:27] Now, by all means, I also understand that curiosity.
[47:36] >> Yeah. Ben said, "Back in college, I was taught Java,
[47:43] which is strongly typed language, so I started hearing TypeScript and I was like,
[47:48] "Oh, people are cramming Java into JavaScripts." I feel like I need to learn Java someday too.
[47:58] >> No problem. >> Cynthia, "Has students write a Discord bot?"
[48:09] Cynthia, you want to come on the show and let's write a Discord bot? That just sounds fun.
[48:17] >> That's both awesome and savage. >> Cynthia, I feel like even if we have to do it as
[48:25] a multiple episode thing, that could be really cool. Then we go into lunchtime.
[48:35] Ben's less sold to learn Java. Anthony said, "Learning Java will only serve to
[48:46] make you like every other language in the world more." Fair enough. Cynthia, maybe we could just put,
[48:57] you can have a sticky note over your camera, and then nobody would know.
[49:02] We can just change your name. We could come up with ways for you to be on the show
[49:07] without people knowing that you're on the show. I don't know. I'm just bringing that one.
[49:15] Yes, you guys are talking about lunch, which does make me giggle,
[49:18] but I am super, super hungry too. >> I have coffee.
[49:23] >> Well, that's nice. Yeah.
[49:26] >> Go to lunch. >> Yes, Ben. Ben agrees.
[49:30] Cynthia, we got to do this. But we can just like.
[49:39] >> Oh my gosh. Oh my gosh. The comments, the comments.
[49:44] Well, I will say that I'm on brain overload for today working on comprehending all of this.
[49:52] Is there anything else anyone wanted to ask about before we wrap up today?
[49:59] Give you a few minutes, do some random dances. I don't know if I've ever said,
[50:05] I have one of those bike pedal things underneath my desk, and I don't know if anybody ever hears
[50:09] it or can see me randomly moving. But that is my new favorite thing.
[50:14] It's like having a fidget spinner, but for my legs to keep me busy and moving.
[50:20] >> Yeah. You don't have to just ask questions about tight script. You could ask about Cloudflare's stuff,
[50:32] I suppose, or Roy, stop it. Stop. All right.
[50:42] Joe Previtt has a great course coming out for TypeScript. It's going to be good.
[50:55] How many? I don't know. It's pretty long.
[51:07] >> As a super random side note, I guess not this week,
[51:14] but next week, we will start live streaming our D&D campaign. I'm excited about that.
[51:22] I don't know if anybody else cares about it. >> Are you ready?
[51:26] >> I'm excited. >> All right. So to further elaborate,
[51:37] we're having a Friday night D&D Dungeons & Dragons stream. >> Space Hippo. I'm so excited about being a Space Hippo.
[51:49] Okay. Please continue. >> At 9.30 PM Central Time.
[51:55] Now, you're like, what campaign are you going to do?
[52:01] Spelljammer. We're going to be in space. Now, Jen chose the Hippo race.
[52:18] >> I'm going to be a Space Hippo. Who's not excited about that?
[52:23] >> That's a spy. That is a spy.
[52:27] It's a spy Space Hippo. >> That's going to be great.
[52:32] >> I've never played before. Anybody understands building a backstory and stuff,
[52:38] please set me up because I think I'm supposed to have that done by tomorrow.
[52:42] I've never built one. >> Yeah. We're going to be doing an off-stream session zero.
[52:50] I'm going to try to get the virtual tabletop set up properly by then.
[53:00] We'll see. But yeah, it's going to be exciting. Besides that, I don't think anybody else had any questions.
[53:15] Roy is also going to be one of the players. >> I'm the Dungeon Master.
[53:21] I will be telling the story and weaving tales for our intrepid adventurers.
[53:29] >> Yay, Ben. >> I do the D&D's.
[53:35] >> Yes. He was actually someone that I told about when we were, when we were doing character creation,
[53:44] I was talking to Ben about it. I was like, "This is all new.
[53:48] This is fun. Hopefully, my character is cool." >> Yeah. Spelljammer in particular is short.
[53:59] It could be done in 12 sessions, which for us would be 12 weeks.
[54:10] It starts at level five characters. I plan on actually scaling things pretty quick,
[54:19] so that you all experience some pretty cool character development and leveling up.
[54:28] I'm going a little outside the book on that one. I might even add one shots here and there inside
[54:39] of the main story so that we can have special guests come in to the stream.
[54:47] >> Yeah. I was going to say, we've got Ben, Bryn, who else?
[54:53] >> I get people DM me all the time now. It's like, "Can I join your D&D streams?"
[54:59] I'm like, "Maybe." >> I don't even know how I got into being on the campaign.
[55:07] >> You were in a space and you said, "Can I join?" I said, "Sure."
[55:13] >> Figures. Oh my gosh. You said that Dan was a monk named Monkey?
[55:23] >> Yeah. >> A monk named Monkey.
[55:25] That could be a fun one. All right, y'all.
[55:30] >> Don't name your hippo hip or something. >> What about hip hop?
[55:39] >> Oh my God. >> What about hippity hop?
[55:42] >> Could I name it R&B instead and it would be really funny? No? I was liking that idea.
[55:55] What about, do you know hippos are actually really scary? >> Yeah.
[56:08] >> They are really scary. >> They account for most the human fatalities in the,
[56:16] I think it's the savanna or something like that. >> Yeah.
[56:21] >> Like far more than lions and crocodiles, all that stuff. >> Cynthia, thank you for having my back here.
[56:31] I like it. Hippie, I like that. >> Okay. I'll share my screen.
[56:40] >> Hippops, the hippo. Hoppy, the hippo.
[56:47] No, Roy. >> Yeah. Can we work on trying to come up with a name?
[56:54] Let me share my screen. >> Look, if you do R.B.
[57:02] and you have a good name for that acronym, I'll allow it. Diva. Oh, can I do Beyoncé?
[57:20] >> I would be concerned about the streams DMCA. >> Okay. That's fair.
[57:35] >> There's even more names. >> Hippo, hippo.
[57:47] These are interesting names. >> Right? Alvin?
[57:54] I mean, I don't think I can name a hippo Alvin. It's not a chipmunk.
[58:01] >> Baby hippo names. Gummy bear. That's weird. Daisy. >> I feel like they just scuba dive.
[58:13] >> They dive underwater. Okay. Interesting.
[58:22] We got little hippie, so we could do little hip hop, hippity hop.
[58:28] >> Are you going to be a giant hippo, and then call yourself little hippie the hippo?
[58:34] I'm okay with it. >> Maybe. It might happen.
[58:42] I don't know. There's different types of hippos. Famous hippos.
[58:54] I don't get why they put other hippo names and then these ones.
[59:00] Pink hippo. >> Hip hop hippopotamus.
[59:07] >> Yeah. Yes. Dolph. Penelope.
[59:17] I'm not going to lie. These ones are starting to make me think about Pokemon.
[59:31] All right. We got some options of what to name my character. Have fun, Anthony.
[59:43] If anybody comes up with, they think is the coolest,
[59:48] most dopest hippo name ever, please DM me because I have a date to figure this out.
[59:56] Or can I figure it out by next week? I just have to have temporary meeting tomorrow.
[60:00] >> Yeah. >> Okay. I feel like there's hope.
[60:06] I will figure it out. >> Yeah. Tomorrow is going to be mostly just getting familiar with
[60:14] the ping.gg setup, me getting the stream set up, and hopefully figuring out the virtual tabletop a little bit,
[60:31] and then getting you-all familiar with where your character sheets are,
[60:39] and how you could roll for stuff and whatnot. >> All right. Well, bye, Ben.
[60:48] For everybody new hanging out with us today, please click that "Follow" wherever down there.
[60:55] I think it's down there. Tomorrow we will be streaming about Next.js.
[61:01] I've done a little bit of Next.js, so this is to see if we can go through a full setup tomorrow.
[61:08] Make changes because it's going to be fun. Same time, four days a week,
[61:16] Monday, Tuesday, Thursday, and Friday. Wednesdays is my mental health and
[61:22] neurodiversity Twitter space at the same time. Yay. Thank you for coming on the show today, Jacob. Bye.
[61:32] >> Bye. [BLANK_AUDIO]

