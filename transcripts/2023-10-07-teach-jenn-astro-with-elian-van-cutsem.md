---
showLink: "https://www.youtube.com/watch?v=WjHTIVO6C8A"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-astro-with-elian-van-cutsem"
title: "Teach Jenn Astro with Elian Van Cutsem"
publishDate: "2023-10-07"
coverImage: "https://i.ytimg.com/vi/WjHTIVO6C8A/maxresdefault.jpg"
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

[00:00] Hello, hello beautiful humans. Welcome to an episode of Teach Gen Tech. Before I go introducing today, I think I annoyed myself with the intro song. It was just too long.
[00:18] I was like, "Can we just get this over with?" I didn't look into either better music for that or into cutting it down to three minutes or something because I was like, "I'm done.
[00:30] Let's go." But today we are finally, finally, finally talking about Astro. I am very excited about all of this y'all because this theme creator, I'm not even going to try to say
[00:47] your name yet. I will get to that. This theme creator, I found the theme back in I think January and I didn't know much about Astro and was like, "Oh, I'll try Astro because
[01:06] I need to try to make a portfolio." Then I looked through all the themes and then I found your brutal theme and I fell in love. I was like, "And not knowing all the things I could
[01:16] and couldn't do." Yeah, yeah. That's how we got to this point. But who are you and how do you say your name? Because this is the big debate on the fact that I butcher your
[01:30] name every time you've joined and said hi to us. No worries, no worries. Hi everyone. I'm Elian van Kutsem, which is my complete name. Elian,
[01:40] if you say Elian, it's also fine because in English, it's kind of difficult to pronounce. No problem at all. I'm a core member of Astro. I work at the Astro Technology Company. Since
[01:50] August, I've joined full time now. I live in Belgium, if that's something that you want to know. I think that's everything about me. I work specifically in team developer experience.
[02:02] I didn't know if I mentioned that. That might be important. That's it, I guess. I think that's really interesting. I think it is important because the developer experience
[02:13] is a big reason we have this show, is to teach newbies, but also get to know the experience of people, being able to bring it down, explain things. Yes, I think location is good because
[02:28] people know that it is like 7 p.m. for you. "Hello, learner." It's midnight learner's time. Dedicated. Is it Hydeo? Hydeo? We're going to go with that. Hydeo. Hello.
[02:43] He's a member of the community of Astro as well. Yay. Welcome. Welcome. Very involved in Starlight, if you know what
[02:51] that is. If not, we'll get into it later. Oh, please. I'm like, you're going to ... I want to show everyone. We're going to see how different it is now. I'm just so excited
[03:09] about this one that I'm like, "I don't even know how to start," because I'll start with just sharing my window of ... I'm not going to go into too much detail about what
[03:19] Astro is. That's why you're here. This is what happened, y'all, is I kept hearing about Astro from everyone, not really knowing what it is. I'm like, "I don't know what Astro
[03:32] is. Let's go check it out. Let's see." I'm like, "Okay. Here's how you install it. Cool. I can figure that out. I'm looking through everything. Got it." Somehow ... Let's see
[03:46] if it's still here. I haven't looked at this. It's either under showcases or resources. It was like themes. It's in both.
[03:52] It's in both. It's in both? Oh, yeah. Yeah. If you scroll down, it's there. If you go to themes, it's also be there. Yeah.
[03:59] Is your theme still here? It should be. I haven't looked at it in a while, but I think it's on the third page.
[04:08] I think it ranks them by stars. Okay. Ah, so definitely everyone, we need to go star his theme, because this was the
[04:16] first theme that I ... It was like ... I think it was this one that I first tried out with. Let's just say, for not knowing what I was doing, I broke a lot of stuff. I made it look
[04:28] really goofy. It was not ... It was a theme like this one. Then I'm just going to go search for it. See. Yay!
[04:38] There it is. Then I found this theme, and I was like, "Oh, my God. I need this theme in my life. This
[04:47] is everything I need in the world." This is as far as I looking into things, and I was like, "Okay, I can do this." Y'all, I'm working on my website. I actually have the week off
[05:03] next week. I did some of the things. I kind of figured it out, but this is as far as I got. Not what we're focusing on today, because there are a lot more resources. I just need
[05:13] time to work on it. I think what ... Roy was on the stream a bit earlier, and we talked about different website types and those type of things, which I think is a great resource.
[05:28] To get us started, now that we kind of know what caught my attention, I started working on my website, started using your theme, and tweeted you, and that's how we got to know
[05:36] each other. What is Astro? Well, I always used to say Astro is this meta framework for JavaScript that's mainly focused
[05:49] on content websites, but actually, that's not really true anymore, which is also why you saw that our homepage changed a lot. That's because we're trying to adapt with our wording,
[06:01] because right now, you can also use server-side rendering, and you have so many uses for Astro that it's actually not really true anymore, that it's just content only. But we do still
[06:10] say content first, so it's a content-first framework with ... You can use JSX in it. You can use islands in it, and islands is this whole other thing. I'll get to it in
[06:22] a second as well, but now you can also build web applications and APIs in it. The thing is, the weird feature that Astro has is that it doesn't ship any JavaScript
[06:35] by default, so if you just start a new Astro website, you build some content in it, you write some code, it will ship just HTML and CSS without any JavaScript at all, which was
[06:48] like really revolutionary thinking back in, I think, two years ago, something like that. Of course, you can still ship JavaScript where you need it, so you choose little blocks of
[07:00] interactivity, and we call them islands, Astro islands. I think that's the very fast pitch. And then one of the also very cool things is that you can bring your own framework into
[07:13] it, so if you like React, you can totally use React in Astro. If you want to use Vue, you can use Vue in Astro. You can use Svelte and almost any other framework. Of course,
[07:24] that is using JavaScript, but even then, we'll still compile it all down to HTML. Instead, if you choose, of course, to use an island, we'll use an island, and then we'll ship JavaScript.
[07:37] I think that's it. Interesting. And now I'm like, I knew the majority of that. I think something that I've noticed in learning this way and working with, I call
[07:56] them the OSRG team. It's like Jacob and Clerk. They're all at Clerk now, so Jacob and Roy, and they literally are, they're all over there. They're slowly all, everyone's going to Clerk
[08:12] in Astro, so I do hope the two companies are best friends. And a lot of them have been helping me through this journey, and it's like, I know a lot of what I'm doing, but
[08:25] I don't realize the names of what something is. So that being said, could you go a bit more into what the islands are compared to, because I don't think I know that.
[08:40] Probably the easiest would be with a code sample. Do you want me to share a window and do some live coding? Sure. I'm down.
[08:47] Okay. I'll try to share my screen then. I think that would be the easiest. Let me get a second to get it set up. All right. So clicking present, share my screen, and I'll just share
[09:08] my entire screen. That way we're sure. All right. Can anyone confirm you can see my screen? Okay. Yeah. Awesome.
[09:17] Ooh, you're an ARC user. Yes, I am. It makes me very fast, and I like this thing. Cool. So we have this website
[09:28] called astro.new. If you go to that website, you can just instantly start from some bootstrap projects, empty projects, anything you want. So we can go over to the docs, we can get
[09:41] started with themes, of course. So you can try my theme or any other theme. You can try Starlight, which is a separate project that we do that focuses on documentation. But let's
[09:52] just start out with an empty project. Let's do that. So I'm just going to do it in StackBlitz all in the browser, just to make it easy. Is this big enough for y'all? Because I know
[10:01] it's typically not easily readable. Yes, I think it's big enough. What do y'all think? And Larry says that they like the happy
[10:13] Houston. Oh, I love Houston. Yeah. They're so cute. All right. So one of the first concepts in
[10:22] Astro is can we zoom the font? Yeah, we can. I'll try to make it a little bit bigger. Just got to make sure that I also have enough room to type. So this is an Astro file. This is
[10:34] just HTML like you regularly write HTML. Of course, you can see the brackets here, which looks a bit like JSX. Astro is a little bit based on JSX. I'll get into that later. And
[10:46] at the top, we have this, I think we call them code fences. Those define the front matter. And that's actually where you can just write JavaScript. So if I do const hello is a string
[10:58] hello. Now, if I just want to say hello here, then let me just get the hello variable in there. This is probably our concepts that, oh, yeah, I need to fork. Give me a minute.
[11:15] That you're all probably very familiar with. It's just a variable in JavaScript or TypeScript because we do support TypeScript as well. Yes, now we see hello. So if I now change
[11:26] this, hello world, once I save that file, you'll see that it updates instantly. That's because we're in the live preview. Now, we support TypeScript. So if I type, this is
[11:40] a number. I don't know if TypeScript is turned on, but it should give an error. Let me check. That's the base. Let me get that to strict. I don't want to. Yes, hello world. Okay. I
[11:57] don't know why this is not working now. Awesome. It does support TypeScript, believe me. So this is the basic that you need to know. Now, if you want to get into islands, we'll just
[12:11] use our super friendly astro add command here. So I just type in the bottom there, if you can see it. NPX astro add, and then I'll type react. And I'll also like to use tailwind
[12:22] because it's easy. So I just type those two. I say, yep, I want to install those packages. So let me get that done. Let's hope this goes fast because NPM can be quite slow sometimes.
[12:38] Yes, but that's like the risk of live coding, right? It's like, eh, we're going to find out. Yep, exactly. Oh, and hi, open Lord. Oh, and Chris is here as well. Oh, right.
[12:50] It's, um, yep. It's StackBlitz that doesn't support TypeScript. Okay. So now if we, um, we start our project again, NPM run dev or run start, both work. We'll see. Okay. Just
[13:04] the same, but we now see that all styles are reset because we use, um, tailwind. So now if we want to use tailwind, we can just type in our classes, like we usually do, um, text
[13:18] Excel. That should work. Yep. So if I go up to seven, it's big. That works. That's just the same as you usually do. Now the real magic comes in when we start to, when we start to
[13:30] use components. So let me just get a new file here, which we call components slash, um, let me build a counter just because it's, it's the easiest. I'll make it JavaScript
[13:41] since that's. Quick question. So I think this is a great, I also am just enjoying seeing if, uh, asking people random things, um, to see how they answer them. I think it's one
[13:53] of the most fun parts of the show of what are components? Because that was something that I hadn't built in other, uh, projects before. And when I finally somewhat figured
[14:05] them out, well, I was a beginner, like, well, I'm still pretty new, but, uh, being a beginner, I was like, Astro was the first time I saw it. And I was like, huh. Okay. I kind of get
[14:17] these kind of don't. So I'm curious how you would explain components. Okay. Components are actually a way to abstract some of your code into, um, components, which are just
[14:30] separate files. So you do a code splitting, um, see as being good for maintainability written reusability. For instance, if I want an about page, I don't want to copy this over
[14:43] and paste it. It will work because if I now go to slash about that page, it will say the same. Now, if I want to change the title or it's annoying. So if I now go back to the
[14:59] homepage, it will still say hello world. Okay. That's cool. But what if I now want to change the global title for my website? I want this to say, um, it's Astro. And here I want to
[15:11] do that as well. Do you see the problem? If we start to do that repeatable times, it's very annoying. So what we can do is we abstract this, just the head part into a component.
[15:23] So now we make a new component. In this case, it will be an Astro component, um, which is called header dot Astro. Now I put my HTML in there. Make sure this is good in alignment.
[15:36] I make it early on next Astro. Now, if I go to the about page, I can do the, can I type this correctly? Header and import that header, just like you would do with yes modules, um,
[15:59] import header from components, header dot Astro. So now if I save that file, you should see, you can't see here, but that the title has been updated. Maybe I should have done,
[16:18] didn't do this with an header, but, um, I can show these off in a separate tab as well. That should work.
[16:24] And Lerner, I like, uh, the way that you explained it of, uh, you have a, a homepage with different kinds of cards that you might want to reuse. You can make each one their own UI component.
[16:37] Yes, exactly. Um, Sarah, I love this idea. Yes. Have the Astro community call with teach gen tech and
[16:46] we'll just like, start talking about Astro every week. I'm okay with that. I feel like it'd be a great learning opportunity.
[16:54] Sounds like a great plan. I agree. Um, so now that I've made this like my separate component, I can import it into my page and it will display everywhere the same. If I change it here,
[17:07] it will change everywhere. That's the thing about components. Um, so we were looking into react component and a react component is just react. Of course it's a framework. Um, I think
[17:19] you know, react, so it's not that difficult. So I'm just going to import, um, you stay react, not from Astro DS react. We're just using regular react. Then we're exporting
[17:35] a function, which is an anonymous function called counter. And then we can return something, which in this case will be, um, an H one saying hello
[17:49] from react. That's a simple component in react. Um, now if we go to the about page, am I still in the about page? No, I'm not. So I'll do it in the homepage. If I now want to import
[18:09] that, we just do the same like we did with the previous component. We just do counter, which will import components. Now let's see if that works. I'm able to render counter
[18:32] because it's undefined. If that's true, because it's not a default export, then there we go. Now we have a react component. Now you'll note that react is a client side, um, thing.
[18:51] Let me, by the way, close this. So if you would normally use react, you will ship the library itself to, to render, to, um, make sure that it's able to render all the JavaScript.
[19:04] We are going to compile them to HTML. So if I now do NPM and build, and we're building our Astro project and I do NPM run preview, we're just running preview. All right. We
[19:19] have the preview. This is the same website. So you see the hello react. If I now go to the inspect, you should, uh, in the network, I'll see if I can make this bigger for you
[19:32] all. Yeah, we have local scripts and stuff, but there is no JavaScript being shipped from the counter component. Now, if you wanted to, because we need reactivity, for instance,
[19:46] if we want to make our counter, um, have some state, so let's add some state, um, let's do count, uh, set count, which is use state zero. And we'll put this in brackets again.
[20:11] We'll add a button with a plus, we'll add a button with a minus, and we'll close it with a fragment and open it with a fragment as well. These are just react specific things.
[20:38] I'm not doing anything weird. Um, just do count. So if we just again, start our NPM run dev X, we can see plus and minus. Um, I'll make them a little bit larger as well.
[21:08] Oh, Excel as well. And let's make this also, normally I would like put some styling that's good in here, but for now it's just to show it off what he does.
[21:24] I don't feel like we really need fancy styling considering we're doing a live coding really quick to understand islands. So, yeah, exactly. So now what we want to do is of course change
[21:36] that variable. We have a variable that starts with zero, um, and we never update it, but we want it to update when we press zero, uh, when we press plus or minus, um, that makes
[21:45] sense, right? So we can do an on click here. So on a click, I want this, I want this to execute a function and that function will set our count to the value of count. That's
[22:04] fun. That makes sense, right? Yes. Nice. If that reloads, where did I go wrong? Probably just need to refresh again. Okay. So now we have a plus button. And if we copy down again,
[22:34] I make that a minus. Nice. This is just a basic counter component. And if you would do this in react, it would work. You would expect it to work. If you use an Astro, it
[22:45] doesn't work. And that has one simple reason. There is no JavaScript being shipped. It's still being compiled all down to HTML. And in your HTML, there is just zero. Um, so what
[22:56] do we do to change that? Well, we have client directives and those actually, um, define your reactivity and how you do your interactivity, um, or hydration, as we call it. And in this
[23:07] case, we just do client load, which means, hey, this is JavaScript component. Ship some JavaScript to this. And now if we save this, we can see it's working. That's what an island
[23:21] does. So now is the crazy part. If I duplicate this component, it would expect that it would have one. It doesn't have the same state because we're just having two different components.
[23:40] But what happens if I remove that client here, that this one won't work anymore while this one still works? And it would only ship JavaScript for just that one component. That's why we
[23:51] call it an island because it's isolated from everything else. Is everyone following me? So since it doesn't execute JavaScript by default, when it loads a website, it's doing
[24:07] the client load to be able to execute JavaScript is what's called an island. Therefore that's why the... Yes, that makes sense. And also I so wonder if that's where I got really stuck
[24:21] with before. Maybe. The thing is we have a couple of client directives which all react differently. So
[24:27] we have client idle, which will also hydrate your component, but will only do so when everything else from the main thread is ready. For instance, things that aren't like priority. We have
[24:42] client visible. Really interesting one and probably the one that you should use most often, which is exactly what Lerner said. You only ship the JavaScript when a user sees
[24:52] the component, when it's in actual in your view. So that's really interesting. For instance, if you have a lot of content here, if you just go like this and we can actually do it
[25:08] like this, and then I'll copy this and paste these over a couple of times and probably a lot more times. Oh, we can see the other one. I'll save that one and I'll build it.
[25:26] Let me get on this page as well so I can make it a little bit bigger. Let's see when it comes. Now we're running the preview again. Nice. Okay. Now there is no JavaScript being
[25:48] shipped unless I scroll down. This doesn't work like as it should work in StackBlitz, but that's what it's supposed to do. And then when you're down, then it will only ship the
[26:00] JavaScript you need. So for instance, if you have a heavy footer that needs some slider, for instance, you need some slider to display pictures and that needs a lot of JavaScript
[26:12] and a lot of things to load in, like in assets and stuff, then you can actually avoid shipping that to any user when they're not on the component, which indeed will speed up your page loads
[26:25] and also like your bandwidth. You're not shipping anything a user don't need. If a user is navigating before he actually does anything, why would you ship any JavaScript? That's the thing.
[26:38] And then we also have client only and client media, for instance, when you only want it to ship JavaScript when you're on a mobile page or when you're on a desktop page or different
[26:51] stuff, you can navigate that. You can find anything about that in the docs. We have it very well documented for you to try out.
[27:01] I'm like so excited about this. This is really... Well, I thought you knew this. Yeah.
[27:09] I didn't. I didn't know this one. Exciting.
[27:15] This is exciting because I was like, I didn't know this one. And I'm like, I wonder if this is where I got really stuck because I think as I was talking about earlier, it can be
[27:27] hard to ask for help when you don't know what something's called. And if somebody is not familiar with Astro, you don't necessarily know that it's not loading the JavaScript.
[27:37] No, exactly. That's really difficult. And one of the things that we at Astro are really like putting effort into is creating a friendly environment where people can ask for help.
[27:47] We have separate support channels in our Discord where people come in. We have an AI also to help you out if it's faster than us. But we try to make it as friendly as possible. So
[28:00] if you do have a question or someone in the audience about Astro or you're stuck somewhere, you can just come into the Astro Discord. It's very friendly. It's just astro.build/chat
[28:11] and it will take you to the Discord. Yay. Thank you. Okay. I know that we had a lot that we wanted to go over and this was
[28:22] definitely one of them. We can go back more through all of that. But I know that we also wanted to talk about, and I just want to make sure that we have enough time because we only
[28:32] have an hour for today. So it's like we have to put a lot into a little bit of time. I'm very busy.
[28:40] To you and to the rest of the Astro team, all of you are welcome to come back on the show. This could be fun. Josh Goldberg with TypeScript, he comes on like once a month
[28:51] and we are slowly going through the book, which is really helpful for learning TypeScript and that's really fun. Okay. So I want to spend a little bit of time on this because
[29:04] documentation is something that I feel like Astro does a really good job about and also something that we talked a bit about with Hacktoberfest. So how can people help with
[29:18] Hacktoberfest and what, let me ask you, what is Hacktoberfest? Well what is Hacktoberfest? I'm actually not the right person to ask, but Hacktoberfest
[29:30] is just like celebrate the month for open source, help us in open source and try to do something in open source, try something easy. And every big open source project tries
[29:40] to open up a little bit of work for people to join in and help out in open source and learn about open source. And we're also participating in as being Astro, we are helping people to
[29:54] create PRs and help out in documentation, like what can they do and how can they achieve it and we'll try to help them as much as we can. I think that's a good explanation of
[30:06] what Hacktoberfest is. I like it. I like it. And what's Uphuck? Yes, it's definitely something that I brought it up because documentation is something that
[30:22] I do. I personally do a lot of the live streaming because I personally get stuck on docs because being super dyslexic, it's hard for me. That's why I love live streams or watching videos
[30:34] or asking my communities because I struggle with it. Yet at the same time, it's always a starting point. And that is something I'm like, y'all, we need to pay attention to.
[30:48] And if you haven't checked it out, because they are really good at, Astro is really good at their docs. I am going to share my screen really quick. There's a few going on. So let's
[31:01] actually go to the docs first. Resources, which we already, I'm excited that you have integrations like separately too, like and document. There's just so many, there's so
[31:16] many. Oh, there is a lot of work being put in our docs and our lead of the docs is also in the chat.
[31:23] Thank you. Thank you, lead of docs and chat. It's Sarah. It's Sarah. She sent a couple of messages before. Yes. Yes. Hi, Sarah. Thank you, Sarah. It's
[31:34] definitely something that I really appreciate being able to go through all of this and take a look. And that's why I wanted to bring up Hacktoberfest because it's, so Hacktoberfest
[31:48] is where it's for the month of October and people can do, I think it's four accepted PRs and they get, if you get it done early enough that are accepted, you get a shirt.
[32:03] Yeah. You get some free stuff, I think. Yeah. And that's always the fun thing. So I just linked it right beforehand for what they could, what you can do and what you can go into.
[32:16] And this has been linked. So I'm not going to go through all of the nitty-gritty details, but this is a great segue to what is Starlight? Oh, Starlight is our framework, especially
[32:35] for documentation. You should go to the main website. If you never saw it, it might become more and more familiar in the wild as well in the near future because we're starting
[32:46] to see some pop-up in the wild. Starlight is the same way you work with content collections and markdown that you do in Astro. You can do in Starlight. So you have the complete
[32:58] developer experience of Astro, but with a lot of ease of use. And of course, with the good parts like hydration and lazy loading and that stuff.
[33:08] You said that it was on here too. Just if you go to starlight.astro.build, I don't know if it's on there. I don't think so. It might be in the footer. And you can use anything
[33:20] you want. For instance, you can use markdown, markdoc, MDX, anything like that. Or of course, you can use React in it. You can use viewing it like that stuff that Astro does. You can
[33:32] use it as well. And we're also porting our own documentation, of course, over to Starlight as well. So, yeah.
[33:42] It's one of the clerks. Sorry.
[33:44] Jacob. sorry. Yeah, Jacob. And thank you Audre Lorde for the link. But I just realized there's
[33:57] the Jay and Silent Bob. Don't they have a show called Clerks? And now I'm always going to think about that when talking about everybody over at Clerk. Anyway, this is cool.
[34:10] Yeah. And it's really pretty as well. You can kind of see it as, I don't know if you're familiar with them, but like you have
[34:20] other stuff like DocuSaris, for instance, is like one of the most known ones. This is a competitor in a way.
[34:29] Oh, this is cool. So one of the big ones that I used to use was actually Stoplights. I used to work for them. They're an API spec company. They just got bought out by SmartBear, but
[34:46] their documentation was just so easy to set up that I just loved using them. And I'm excited to see it. Now, do I need documentation? I can write documentation for something. It's
[35:01] just so pretty. Of course you can. There is a lot. The thing is that Hectober, if I'm correct, this year
[35:08] is mainly, how do you call it? Encouraging low-code or no-code contributions. So of course, we have a couple of things that you can do in Astro that are no-code even or low-code.
[35:24] For instance, translations is one of the very big things that we do. Of course I chose one that-
[35:29] But the nice thing is that we, Astro, for instance, Starlight, since you're on Starlight anyway, the whole UI is available in a couple of languages and every language is, Sarah
[35:45] is typing some hype. This was created by our Docs team. I like it.
[35:50] Wait, I'm going, oh yeah, there it is. You can read it. Okay. Yeah, for sure. So we need to do the hype, the hype. It's important. This was created
[36:02] by our Docs team, which incorporates everything we know about producing good docs from our writers subtly suggesting good content architecture to choosing fonts that people can read for
[36:14] longer stretches of time. I love that. I love that. That's way better than I can.
[36:21] Yeah. And I'm going to go on the hype train and just say, "Hey, everybody that's currently
[36:26] here, please hit that follow button because I need to grow my channel and we're going to have more dope people on and hopefully more Astro." And eventually, Clerk.
[36:35] I hope so. Jacob, I'm looking at you. Jacob, that's directly at you now that you are at Clerk. Roy can
[36:41] come on, but Jacob, I'm looking at you. Everyone joining Clerk.
[36:49] Yes. Yes. Good night, Lerner. Thank you for joining today. This is so cool. Yeah.
[36:59] I would say then, is it out of, especially since you do developer experience, what is something that you are most excited about with Astro?
[37:14] There is a couple of stuff I'm super excited about. There is a couple of stuff I can't talk about yet, but one of the coolest things of course
[37:23] is we have an open roadmap, so that's nothing secret, is Astro 4. So we are deciding on what we're going to build in Astro 4, and that's super exciting. We're working on a
[37:36] lot of really cool stuff that I wanted to see in Astro itself, and it's coming to Astro, so that's crazy. I'm super excited about that.
[37:45] For instance, we are building translation routing or internationalization into Astro itself, and I'm super excited about that. That will solve a lot of problems I had in
[37:57] the past. One of the really cool things as well is that we're porting our documentation site to Astro, which will also be awesome. So yeah, we're doing really a lot of work
[38:09] and a lot of cool work. Yeah, so I'm mainly excited about that. Yay. And I would say, so for those who are looking at maybe they're like, "Hey, I
[38:23] know what Astro is. This is really cool." How would they go about creating a theme like you did? Could you tell us a bit about your journey on creating your theme and how we
[38:35] can also go star that theme? Actually, it's really easy. I coded it in two days. It doesn't mean that building a theme has to be easy. It can be very hard
[38:49] if you're building something cool, but I built something really, really easy. Actually, it's just building your website like your website is, and then just making it so general that
[38:59] anyone can use it. For instance, actually, the Brutal theme that you used was just my website that I published. So I published it. I removed a couple of things. I removed my
[39:09] name. I gave it another name and made it a little bit more generic, and then I published it. And on the website itself from Astro, you can just submit a theme, and then we'll
[39:21] add it into our team showcase. And the same for the showcase as well. So if you built a website that's live with Astro, you can submit it to our showcase, or you can even
[39:33] submit it in our Discord channel, and then we'll showcase it because we want people to see what people are building with Astro or with Starlight. Starlight also has it. And
[39:44] yeah, you can totally go star the Brutal theme. It also has changed a lot since you used it. Oh, I bet. Yeah. That's one of the sad things about just
[39:58] normal themes is that once I publish an update, you don't get it because you forked it anyway. So that's sad. But yeah, that's how themes work, I guess.
[40:10] That's really cool though, because that's something that actually got me excited about using Astro was checking out your theme and seeing that there's at least a starting point.
[40:24] It taught me a lot about also the differences. These are minor things that I think are still so beneficial that a lot of people may not consider or think about is it really helped
[40:36] me understand differences between Uno and Tailwind, because I hadn't done a lot in CSS and I didn't really know there was- Right. You might think, "Ooh, uses Uno.
[40:46] That's true." Yeah. And it's definitely something where also understanding the components and a bit more of how that's actually described compared
[40:58] to what ... I don't ... Jacob, what did I try explaining components as? Do you remember when I originally started trying to build that site? Poor Jacob. That's all I could
[41:12] say, is I would go down a rabbit hole thinking I fixed it and he's like, "No, you just pivoted at a very random point." But also hearing about islands, I think, is a big part that
[41:25] knowing that and understanding it is something that I'm like, "Okay, cool. I know how to Google it now." That's always the biggest part is knowing how to Google something.
[41:37] Well, we do have a very good tutorial that walks you through everything that Astro has to offer down to content collections, CSS, integrating components and islands and that
[41:48] stuff, on our documentation as well. It's a complete interactive tutorial that you can take on your local computer. You should try it out. Maybe it will help you understand
[41:58] what Astro is better in a way and what all of our newer features are. Well, I won't say it shows you everything. For instance, view transitions aren't in there yet. But I think
[42:12] it's a great starting point. When will those be added in? Now I'm curious. We got the entire team here.
[42:22] The thing is that they are ready to add in. The thing is more that we want to do it at the right moment so they're in draft. And I think, yeah, Sarah just said it. They're
[42:34] in draft PRs. Because we think a lot about how our structure is and how we want people to perceive the documentation. So it will be coming soon. If they're draft PRs, you
[42:50] can check the draft PRs. Yay.
[42:52] Yeah, soon is something we say a lot. Sorry. I mean, that's fair. I think the other word I hear the most since getting into tech, more
[43:07] than probably anything, is "it depends." It depends.
[43:10] It depends. The thing is that it's mostly true.
[43:16] Yes, yes. And Jacob told me what -- I was thinking of components more of separation of functionality rather than combined functionality, styling and structure in one file to represent
[43:32] a section of the UI. I'm glad you remember what I was doing. Because I was trying to figure it out. And that is good to know, Sarah. Thank you. Yeah, that's fair. Nobody wants
[43:49] a tutorial to get bigger. That is definitely fair. No, exactly. Yeah. The tutorial as it is, is great. We have updated it a couple of weeks
[43:58] ago to Astro 3 as well. So it's completely compatible. And now we're just trying to think about how can we extend it. Like extend your blog to use content collections. Extend your
[44:07] blog to use view transitions. So yeah, we're thinking about it. But soon it will be published. Yay. And hello, CodePill. And thank you for the follow. And yes, we totally want a tutorial
[44:30] to include everything. So we get stuck and never, ever finish it. Well, the thing is, no, we don't, of course. I know what he's getting at. But the thing
[44:39] is that a lot of people give us feedback, "Hey, it doesn't use the new content collections. Why is that?" And then we're like, "Yeah, we kind of don't want to overwhelm a starting
[44:48] out person with all this information, all these new features." So yeah, we thought about it. And we have a reason why we didn't do it. Yeah.
[45:00] And that's a big reason to join in on the community. And also, from what I've seen of the Aster team, they do stuff like this where they join other streams or videos and content
[45:13] to be able to get this information out at the different learning levels, which I think is really awesome. But yay, this is a good one to read. CodePill, they just wanted to
[45:37] say that Starlight is incredible and Astra is becoming one of their favorite frameworks. They would love to contribute in any way they can. And they have the GitHub with the information
[45:51] for Hacktoberfest. That's one of the ways. Is there other ways individuals can contribute to helping your team out? Well, the biggest that we're in need of right
[46:03] now is reviews for our translations. So we do have a lot of translations. Our documentation is translated in nine, 10-plus languages, but not all of our pages are. And sometimes
[46:16] you don't have the time to translate all of those pages, but maybe someone else translated it in a language that you know and you just can read them. And if you can read them and
[46:26] you can give them pointers what you think is good or not good, that will help us out because we don't speak 10-plus languages. So that's a terrific way to get started with
[46:37] like a low, low to no code piece of it. You can also, of course, write them because writing documentation is of course very good to getting to know the framework because who actually
[46:48] writes documentation for developers? It's us who do it. So we have to know all the features. We have to know what happens. So I think that's a very good way to also get technically start
[47:00] with Astro and like what it is. For instance, if you translate the Islands page, you will understand better than anyone else what an Astro Island is. So those, oh, maybe I should
[47:15] share our Astro Docs translation status page. So we have, and it's a public page, of course, where you can just see this information. So this is our translation status. And then you
[47:34] can see which languages still need to be translated, how many pages are done and anything else. But this is something that you might want to look at. For instance, a lot of people
[47:44] speak Spanish. We still need reviews on a Cloudflare PR and on an LPGS PR. And if you think, "Hey, that might interest me," go ahead, review it, read it, let us know what
[47:58] you think. And if it's good enough, it'll make it on the page. And then you have contributed us and helped us out in a tremendous way. But this is like our total. So we have a total
[48:09] overview where you can see what pages are missing, what pages are done, et cetera. I'll send you the link for that as well. Oh, this is really cool. Yeah, thank you.
[48:19] Yeah, this is a really, really cool feature. That is definitely cool. And y'all, straight up, I think I just got nervous, as I always do, when I'm like, "Oh, we only have an hour,
[48:31] so we have to go through as much in as little time as possible." And I think I totally rushed everything, which it does happen from time to time.
[48:40] That happens. But it also gives you a little bit of time before your next meeting. That's true. That's true. Perfect. Yeah, yeah.
[48:49] It was planned. It was totally planned. Exactly. But I am curious, just for everybody that's joined today on the Astro side, or those in
[48:59] the chat, or when this gets uploaded to YouTube, what specifically would you want to learn about with Astro? Because there is so much that we could be doing, and I love that we
[49:10] got to learn about islands specifically today, and components, that those are definitely some things I'll be checking out more. But I'm curious what everybody else would want
[49:19] to learn, and maybe we can go bug the team again to come back on the show for a longer time to go into something specific. But I like that we had the high level today.
[49:31] Yeah, exactly. There is so much in Astro that you can still learn from and do. For instance, there always is a thing of state management, global state, how does that work. For instance,
[49:43] you saw those two React components, but they didn't have a shared state. So that's a thing. You have view transitions, which is such a new thing. We were the first one to ship it.
[49:53] Well, view transitions see it as animations in between pages, but with a browser API and not with animations APIs. Well, animation libraries. And then, of course, there is content
[50:07] collections, which is an easier way to organize and write your content, which you probably are already using, Jen, since you're using Google.
[50:15] I was. And I think, actually, that is a great one to start with. So if you or anybody on the team wants to come on, I think talking about content collections would be really
[50:26] cool, but also something that I was trying to do, because I started working at Ivan. So I was like, "Hey, I want to use Postgres from Ivan to see if I can make this work."
[50:38] And it would get rid of the content collection. That I'd be curious to see, to be able to help others, including myself, understand the differences, why somebody would go with
[50:56] content collection instead of with a SQL database. And is there a way to replace it if they wanted to go with Astro, but go with the database? I feel like there could be a lot broken down
[51:09] there that could be really useful. Yeah, totally true. And it's also like, we do have a lot of CMS guides. So if you're
[51:18] interested in those, you can also read those and review those for Hacktoberfest. The thing is that, yeah, this is such a personal thing, a personal opinion on how you personally want
[51:31] to build your website. And it's almost always possible. The thing is that it's just difficult for us to decide how to put it in docs. Because for instance, using Ivan, probably we don't
[51:46] get that question asked that much. But you're always welcome to write a guide if you've actually done it before. For instance, that's like community driven is always welcome. But
[51:57] we won't write the guide for ourselves. But we do have a couple of back end guides on the website, I think. I think we have Superbase, for instance, where you use a database, or
[52:07] Firebase, where you use a database. So we do have those. But they are all community written.
[52:16] That's very cool. Yeah.
[52:18] Yeah, for sure. And I think that's some great callouts. And yes, Mark, I like the idea of your wife helping you with docs. That could be cool.
[52:31] Yeah. Awesome. Thank you, Sarah, for answering for CodePill of where is a good place to help out if English
[52:41] is their only language. I think that is a great callout. And there is a lot that people can do on the docs too. So, so many options.
[52:50] Oh, and I actually saw never contributed to open source before. Well, that's actually funny because contributing to open source, Astro was also my first one. And it was adding
[53:02] a 404 to the Astro website. So you see, it happens. No worries. Don't be scared. We'll walk you through it.
[53:12] Yes. And ask for help. Definitely ask for help. And sometimes I will say in any community, no matter what, sometimes you don't always get the quickest response or something. So
[53:23] give it time and ask again if you need to, because that sometimes has realizing that I was like, "Oh, okay. I can do that." So I may ask again in the future if something
[53:34] isn't responded. So definitely do that. And it's a great team. So stoked that you were able to come on the show today. Thank you. And let's see, I'm going to raid y'all over
[53:49] to learn with Jason, because one of the ideas of how I came up with the name for the show was I didn't want to do learn with Jen because he has learned with Jason. So Teach Gen Tech
[54:04] is how it came to be. So thank you everyone for joining today. Make sure you hit that follow, and this video will be posted on YouTube later this week. Thank you, everyone.
[54:16] Bye. Thanks for being here. And thank you, everyone, for asking great questions. Just so I don't forget to say that.
[54:26] Thank you. It is always very, very helpful. So thank you again. Bye.
[54:35] [BLANK_AUDIO] 
