---
showLink: "https://www.youtube.com/watch?v=VWbB-tQ_dOU"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-how-to-integrate-payments-into-your-react-app-with-square-with-bakari-holmes-pt-2"
title: "Teach Jenn how to Integrate Payments into your React App with Square with Bakari Holmes Pt 2"
publishDate: "2022-07-29"
coverImage: "https://i.ytimg.com/vi/VWbB-tQ_dOU/maxresdefault.jpg"
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

[00:00] - One. - Oh, see, it doesn't give me the countdown.
[00:04] And yes, everyone, hello, this is Teach Gen Tech and we have Bakari again.
[00:09] And yes, he like had the perfect timing for when we were at the countdown to go live.
[00:15] And I'm like, StreamYard doesn't even show the countdown. What?
[00:19] - I actually didn't even have a countdown. I just.
[00:22] - Yeah. - Did it. - You just have
[00:24] magical timing. - Exactly. - That's just what it is.
[00:27] And for those of you who didn't catch earlier this week, this is part two of integrate payments
[00:35] into your React app with Square. So we are doing part two today.
[00:41] And in case anybody didn't catch part one, it will be linked in the comments.
[00:48] And also Bakari, please introduce yourself for anybody that didn't see you on Wednesday.
[00:55] - All right, well, I am Mr. Bakari Holmes. I am a developer advocate and content creator,
[01:04] also software engineer, physicist, teacher, musician, a whole bunch of things.
[01:09] So I recently connected with Gen, I believe it was through Twitter,
[01:15] and it has been really awesome. And we actually talked about doing this session.
[01:24] It was originally supposed to be one session and it ended up getting stretched to two sessions
[01:28] because we'd be talking. So yeah, I'm just happy to be back
[01:34] and to close this out and seeing all your comments. - I would, I just wanna shout out
[01:43] to just all the guests that have been on here because they all end up being like a two-part process
[01:48] of like they're doing one thing and then they come back to either finish it out
[01:53] or do something else. And it's just really cool that people can get used to
[01:58] some of the guests on the show and learn who they can reach out about a specific topic.
[02:04] So like, for example, if somebody had questions on integrating payments,
[02:10] they're like, "Oh, I can hit up Bakari, he probably knows what's up."
[02:14] Or if they want to look into like Veet and Vercel, they could reach out to Anthony.
[02:24] And Yeray helped me with the bare basics of JavaScript back in the day.
[02:30] And it's crazy 'cause I'm like, "Oh, I actually kind of get that."
[02:33] So people should hit them up for so much more. And I should have them back on the show
[02:37] since it's not a complete newbie thing anymore. I mean, we're like getting there 1% at a time
[02:44] with all the shows. But with being just slightly over a month old,
[02:51] we have had, I think this is our 12th Aerie live, our 12th live, which is exciting.
[03:01] And we have a ton for like, a ton for August. So this is really cool,
[03:08] even though everybody's on vacation or holiday in August, this is exciting.
[03:14] So, all right. I have to get back into what we were working on.
[03:21] I have my index, which we, where we left off the other day that kind of took us a bit
[03:29] was troubleshooting an error we were getting from starting it up.
[03:33] And it was because I put payments or I put payment instead of payments.
[03:38] And it took three of us troubleshooting to realize that that is what I did,
[03:43] which did make me feel a lot better about being a newbie because it's like,
[03:49] y'all have a ton of knowledge and experience. And this is something that all coders run into.
[03:56] It's not just a newbie thing. It is an everyone thing.
[04:01] - Right. - So I really appreciated that.
[04:03] And we also decided that Anthony is gonna come on the show and talk to us about documentation,
[04:12] which is gonna be dope too. - Yep.
[04:14] I think the lesson there is that troubleshooting is not a magical process.
[04:19] You don't wave a wand and then figure out the problem. It is a trial and error many times,
[04:25] or it is, if your code is modular and it's divided into pieces,
[04:29] testing each piece out to try to figure out where the problem is.
[04:34] So, or looking at an error that's been logged to or shown to you and then looking at the documentation.
[04:41] And then from there, going back to your code and then trying to have a better idea of what to look for.
[04:48] So it is not magical. - I wish it was.
[04:51] I do wish it was because that would make things so much easier, but I am looking forward to now.
[05:00] Now, the one part I don't remember from the other day of what were we doing to run and find the error?
[05:10] It was like, I thought it was like NPN something, but I don't quite remember.
[05:17] - So this is in the Next documentation, or most applications have like an NPM run
[05:27] or NPM run something. For Next to run your local,
[05:34] to run your application on your local computer, you do NPM run dev and that's development.
[05:40] That's the development version of your application. And this typically is, you know, to,
[05:47] as you're developing, as you're building features, as you're building out your code,
[05:51] you can run the development version. It'll run on your local host, typically.
[05:56] - That is really cool. And as something that I learned from working on doing this
[06:03] myself with VEET is these formats do have updates and can like change things around.
[06:13] And something that I was running into there is they created a very random local host number,
[06:19] not the usual like 3000. So definitely read your, you know what it is saying
[06:27] because it doesn't always, it's not always the same for everything.
[06:33] - Right. - If I take that local host 3000
[06:39] and put it into a browser, we got it. It's the normal Next.js from the pages/index.js,
[06:48] which is under the pages folder, the index.js. - And if you look at the JSX,
[06:57] which is basically HTML in JavaScript. - Okay.
[07:02] - Your index.js file, let's just kind of take a look at what's on the screen versus what's in your code.
[07:09] - No, okay. Whatever.
[07:15] Oh, there we go. - There you go.
[07:16] - I'm like, I'm gonna get that. - So if you see on the bottom,
[07:20] there it says create next app. - Yeah.
[07:23] - And then if you hover over, if you look at your tab, see what it says?
[07:29] - Yeah, 'cause we got documentation. - Higher, higher on the top of the page.
[07:34] - Oh yeah, welcome to Next. - Your Chrome tab, higher.
[07:37] Right there. - Ah.
[07:39] - That's where that text comes from. - Oh, that's cool.
[07:42] - Your title tag. And that's all part of your head tag.
[07:47] So these are things that, yep, Valkyrie is dope. You can change that.
[07:52] And once you save it, it should hot reload. Meaning once you save,
[07:57] the builder detects those changes and then should re-render. - All right.
[08:13] And save. Oh, declined.
[08:15] Don't even talk to my friend. It's supposed to be ignoring it.
[08:19] But you know, that's cool. - So there you go.
[08:23] You just made a change. - Yay.
[08:27] - And now it's showing that change. You didn't even have to run NPM again.
[08:32] You didn't have to run your server again. It actually built into the Next.js packaging.
[08:38] - That is cool. - Is that hot reloading.
[08:40] Yeah, and it really comes in handy when you're developing because you can just, on one screen,
[08:46] you can have what you're rendering or what you're running. And then on another screen, you can have your code.
[08:53] Maybe you can have your command line on another place and it helps your workflow.
[08:58] - Nice. - I mean, lots of people have different ways that they work
[09:01] and they like to have all kinds of different colors on their command line and their Git.
[09:08] They would like to have their Git status maybe. There's all kinds of really cool
[09:13] and complicated, colorful tools that you can use. - That's cool.
[09:16] - We're gonna stick with the basics for right now because our focus here is to build a working
[09:22] Next.js and Square integration. So what I want you to do is I actually want you
[09:30] to erase in Next.js, erase everything. Do you have an import at the top?
[09:38] Credit card, okay. Everything except that from line two down.
[09:44] So from line two down, erase everything. We're gonna start over.
[09:49] Okay. - And hit save, I'm guessing?
[09:52] - Yeah, if you hit save, then now there's gonna be a blank page.
[09:56] - Yay. 'Cause there's nothing to render or do anything with.
[10:01] Okay. - Okay, so now what we are doing right now
[10:05] is we are importing three things and we are using the import that's a command in JavaScript
[10:13] and that's recognized in React. And that open curly brace
[10:19] and that credit card payment form, I'm just explaining it to you one at a time.
[10:24] Credit card payment form and ACH, those are three different components
[10:30] or types in the React Square Web Payments SDK. If you go to your web browser
[10:40] and Google React Square Web Payments SDK. - React Square, I can't find it,
[10:48] Square Payments SDK, yay for coming up. - Yep.
[10:52] You wanna go, yeah, there you go. That's actually an NPM.
[11:01] We want the GitHub. - Oh, there we go.
[11:06] - Yeah. There we go.
[11:09] And if you now click the, see the link to their website.
[11:16] - This one? - Yep.
[11:17] - Yep. - Click that.
[11:19] Yeah, and there should be some documentation. So do get started.
[11:27] - There's docs up here. - Oh, oh, or you can do that.
[11:30] Okay, awesome. So now you notice there's introduction
[11:36] and you can go back and read this in depth, but there's getting started and then there's credit card.
[11:43] You see how there's credit card there on the left-hand side? If you expand that, it says usage.
[11:48] So click on usage and it'll tell you like how to use credit card in the documentation.
[11:56] And if you notice, the first thing it tells you to do is to import credit card in payment form.
[12:02] And that's what we've done. - And then, so that means the next one,
[12:07] I'm not like saying anything, but like since we did the ACH right here,
[12:12] that's gonna be under ACH right down here because-- - You got it.
[12:17] - Okay. - But we already have the payment form,
[12:19] so all we have to do for ACH is just import ACH. - Okay.
[12:24] So that means that we need the export information as well? - We are going to be doing that, but we're gonna go,
[12:31] that's at the bottom of the file typically or at the beginning of the function.
[12:37] So we're gonna go line by line and we're gonna build out our components.
[12:42] - Okay. - Our components within components.
[12:48] So one of the things I wanted to talk about is that components can stand on their own in React.
[12:55] Components can be functions or they can be classes. Talked about classes yesterday, right?
[13:03] Components also can house other components as children. So in other words, like you can have an outer component,
[13:12] like let me share my screen here. - Yeah, for sure, let me switch it over.
[13:18] There we go. - Okay, here, let me see.
[13:21] Oh, you've already got it there. Ah, I didn't realize it was already sharing.
[13:28] So here we have an outer function called MyPaymentForm. And if I click here, right?
[13:37] On the starting open paren, it ends way down here, right?
[13:47] So that means this function, all of this stuff is inside this function.
[13:54] - Okay. - MyPaymentForm. So when this file runs, it's going to,
[14:01] well, this function is defined here, but I think if we go to, what is it?
[14:09] App.js. So yeah, we have my app and we have component
[14:14] and page props. That actually, it's not very clear,
[14:21] but basically it's going to grab what's in index.js. - Okay. - And it's going to run it.
[14:28] And there's some steps missing because there's some things that Nex is doing
[14:31] behind the scenes. - Right. - But essentially,
[14:35] it's going to take this index.js. That's why it's given us this.
[14:38] And it's going to run this function. It's going to fire.
[14:43] It's actually going to run this whole file. So first thing it's going to do is go,
[14:46] oh, okay, you want to import credit card payment form in ACH. All right, I'm going to go and I'm going to grab this.
[14:52] Now remember the whole code splitting thing and the whole preloading, prefetching.
[14:57] So I'm not sure when it's going to do this, but it's going to do it at an opportune time
[15:01] that optimizes your page load time. Now, when your application is small,
[15:07] doesn't make a whole lot of difference. But when your application starts to scale up and be larger,
[15:14] then it starts to make a whole lot of difference. You know, it's like your page loading
[15:18] and depending on the size, your page loading in a second versus like,
[15:23] you know, four seconds. And also depending on your device.
[15:28] - Right, we compared that one to, or I compared it to like Quick
[15:34] because in Quick it only loads what you need it to load. - Exactly, exactly.
[15:41] And in a code splitting, it loads what you need it to load. And it also determines the order that things need to load in.
[15:49] So that's also important. Okay, so the first thing I want you to do
[15:53] is I want you to do const my payment form. - Okay, so we got,
[16:00] I'm working on also doing it where I get the lines right because of like proper coding.
[16:10] Okay, so const my payment form. - So I'm going to, I just got rid of that.
[16:19] Just for clarity sake. (indistinct)
[16:24] - And this syntax is what's called an arrow function. - Okay.
[16:35] - It's the same as going function, my payment form. And then, you know, here's our parameters.
[16:50] And then we want to pass in, if we would've had a parameter here,
[16:55] that would be called a prop, but we don't have any props here, but we'd say, you know,
[17:00] prop one, whatever. - Okay.
[17:04] - Customer name, let's say it was customer name. All right, this is the payment form.
[17:14] Let's say the payment form needed a customer name. We could pass it in there to my payment form.
[17:20] But right now we don't need any, we don't need any props. - Okay.
[17:25] - Props are just, they're just arguments or parameters to the function.
[17:32] - Okay. - Okay, so this is just another way
[17:36] of doing the same thing, declaring this function. And we're actually, you know,
[17:43] my payment form is going to be also a variable that holds a function, because we say const, right?
[17:50] Just like we created variables before with const. We say, my payment form, and then we are,
[17:58] it's saying it's equals, or it's going to get, it's going to be assigned to this,
[18:05] which is just an empty function at this point. - Okay.
[18:10] - Okay, all right, so let me get rid of that. Now what we're going to do,
[18:16] one of the first things we're going to do is we are going to do payment form.
[18:21] And then for, again, for clarity's sake, and I'm going from the outermost component
[18:27] to the innermost component. So I'm starting with payment form.
[18:30] Do that. So that's what you want to do.
[18:37] You want to have payment form. Actually, hold up, wait a minute.
[18:47] Here, I can just type it like this. (mouse clicking)
[19:04] So this is that payment form we just imported. - Okay.
[19:30] - And it's the open, opening, and closing tag. - Okay, and is line three,
[19:44] is that very part at the end, is that a regular bracket or is it a squiggly bracket?
[19:51] - This here? - Yeah.
[19:53] - That's an open paren. - Okay, cool.
[19:56] - Yep, and then the close paren's down here. - Cool, that's what I got.
[20:00] - Yeah, and you're going to want to, you know, to make a one like that.
[20:03] Okay, so we have the payment form. All right, so the next thing we're going to do,
[20:09] we do undo, is inside your... Let's see here, actually.
[20:18] We're not going to need this, that there. What you want to do is hit enter,
[20:25] and then we're going to enter a whole bunch of stuff inside a payment form.
[20:30] Now, for Square, for Square Payments, the form that you're sending in
[20:41] when you have a transaction needs certain things. One of the things is an application ID,
[20:49] and you created an application before, and you were given an application ID.
[20:55] So what it does is it identifies the calling form with a verified application ID
[21:02] generated from the Square dashboard. So they want to control what applications
[21:08] are actually making these calls, and the users tied to those applications.
[21:14] - Yes. - Especially when you're dealing with finances,
[21:18] you're dealing with people's money, people's identity. Those two things are high security risks.
[21:26] - Cool. - I'm also remembering how to get back there,
[21:37] so that way I can ensure I have those, that information.
[21:46] - Cool. - And I'm displaying my sandbox value
[22:02] for the world to see here. And what you want to do is have application ID equals,
[22:15] you know, open quotes, and it's going to be a string,
[22:21] which is your sandbox dash SQ something, something, something, something.
[22:28] - Am I not scrolling? I can't find it again.
[22:34] - Did you put it on your? - Oh, I might've put it all of it,
[22:41] but I'm not sure if I put all of it on my notepad. Let's see if I did all of it.
[22:46] Oh, I did all of it. Okay.
[22:48] - Yeah, I think I remember us doing that. - Okay, so we've got payment form,
[22:56] and then we need to do application ID, equals,
[23:08] (indistinct) All right, I am there.
[23:21] - All right, awesome. - And then card token response.
[23:28] - Yep, this is, sounds a little heady, but I'm gonna just kind of break this down.
[23:34] So the purpose of this is kind of twofold. When you are making a,
[23:44] when you want to have a transaction, like for instance, you want to charge a credit card,
[23:51] two things need to happen. According to the square documentation,
[23:55] and we can actually go to the square documentation. Let me see here.
[24:00] I think I pulled it up. Somewhere, here it is.
[24:08] Okay. So you should be able to hopefully see
[24:30] the square documentation page here on web, get started with web payments SDK.
[24:35] So there's a ton of great information here. If you go down here to the overall implementation flow
[24:43] of an online payment option, it works as follows. You need to do two things.
[24:46] One, you need to configure the web payments SDK client library with your application
[24:52] to render a payment method form and add, and to generate a payment token.
[24:58] So we are configuring our client library by using those React components that we just imported.
[25:10] - Okay. - And we are importing them
[25:16] and then placing them inside the payment form. We haven't gotten to that yet.
[25:21] And that's going to, it's gonna configure, it's part of the configuration.
[25:27] Then also we are doing this card tokenize response received function.
[25:35] And that does a few things. One, it does a fetch request,
[25:38] which a fetch request is just what it sounds like. You're asking someone to go fetch something.
[25:43] It's fetch as a function. And let me go back to my code.
[25:49] So fetch is just a function here. And we are saying, okay, we want to go,
[25:56] we want you to go fetch some information from a database or from a URL.
[26:03] The URL in this case is API pay. We haven't set that up yet, but we will in a second.
[26:08] And then it's method is post. There are, these are the types associated
[26:14] with rest in HTTP. Typically HTTP is hypertext transfer protocol.
[26:21] It's the protocol or the way of communication in the web. And that's get, put, post, delete, and update, I believe.
[26:30] The most common ones are crud or create, read, update, delete.
[26:40] Those are the most common. - I feel like I need to do an episode just on that.
[26:45] And then an episode just on protocols. Because like I get them, but I don't get them.
[26:51] - Would you say criticals? - On those and then protocols.
[26:59] - Protocols. - Like HTTPS and then IMAP, POP.
[27:05] - Yep. - There's more than that.
[27:08] - The rabbit hole goes deep. The rabbit hole goes deep, definitely.
[27:13] But for right now, all we need to worry about is post. And when you're post, when you're doing a post request,
[27:19] you are sending a body of information in along, you know, along, you know, along with your request.
[27:28] You have a header and you have a body. And that body is in a certain format.
[27:35] In this case, it's JSON. You're gonna hear that a lot,
[27:38] especially if you're dealing with the web, you're gonna hear JSON, JavaScript Object Notation.
[27:43] It's really just a JavaScript object. In this case, it's gonna have a whole bunch of things
[27:47] inside the JavaScript object. This is going to have source ID.
[27:52] That source ID is the token we just read about in the documentation that we need to generate a token.
[28:00] So we are, when this function, card tokenized response received, which it is a function,
[28:13] we're passing in the token and the buyer. But when this fires off,
[28:18] when the payment form receives the result of a tokenized generation request,
[28:26] the result is gonna be a valid credit card or wallet token, or you're getting an error.
[28:33] So the Square API is gonna give you one of those. - Okay.
[28:38] - Okay, so if it's an error, you know, it'll be a helpful error that tells you,
[28:42] hey, you know, credit card was invalid, or, you know, sometimes you see those actually when you,
[28:49] you know, you swipe your card, you know, it's a pin was invalid, whatever, you know, something.
[28:58] Hopefully you don't get a 500, which is basically like an internal server error.
[29:03] You can't do anything about that, but hopefully it's something you can do.
[29:07] If you're writing the code, you can do something about,
[29:10] but if you're like the customer and you make that, you swipe your card and you see a 500,
[29:15] it's like, oh man, I can't buy it. - Yeah. - I'll go to another store.
[29:22] So you wanna have helpful errors. Okay, so we talked about methods.
[29:29] We talked about headers. In the header, we're just gonna say
[29:33] what the content type is. And we say application JSON,
[29:38] because we want the type for this request that's coming from the front end to our backend.
[29:46] We want it to be in JSON. - Okay. - We're sending some JSON.
[29:50] In this body, just JSON.stringify. What this does is, oh, look, if you hover over it,
[29:59] it tells you what it does. It converts a JavaScript value to JSON.
[30:06] The JSON string. So it's still JSON, but it's in a string,
[30:11] because the web likes strings. - Yeah. - Things in quotes.
[30:15] - Oddly, because my mom was joining yesterday, she was talking about it,
[30:23] and I don't know if you know this, but she said back in the day, she heard that string,
[30:29] instead of being like something in quotes meant like multiple files in a string,
[30:36] it meant like files working together, was a string of files kind of thing.
[30:40] - Yes. - And that's, so was it called string, and is that still called string?
[30:44] - You know what, I'd have to look into the origins of like string.
[30:48] I know strings have been around a long time. But yes, there can be a string of files,
[30:56] and you can process them one by one, or process them in a batch.
[31:04] But yes, they are, so a string of files, so the word string still means the same thing,
[31:10] but it could be like a string of files. It could be a string of characters.
[31:15] And in the case of the string we're talking about, it's a string of characters,
[31:18] because every character has an index. - Okay. - They start at the index zero.
[31:23] So index zero of, let's say your application ID. Index zero of application ID would give you the S.
[31:31] - Okay. - Index one would give you the A.
[31:35] - Okay. - So they're like an array, really,
[31:37] 'cause they're stored like an array in memory, in these different memory slots.
[31:42] - I'm gonna say, I think I understand what you're saying, but I don't understand what you're saying,
[31:46] but I think it'll click later on. - Okay, I wish I had a whiteboard.
[31:50] I would just draw some boxes, and each box would be a memory slot.
[31:55] And then I would put S in the first box, and then A in the next box,
[31:59] and then I would label the first box zero. - Okay.
[32:03] - So in order to access that memory, you need a way to do that.
[32:06] - Okay. - And in strings, they use numbers.
[32:09] So you say like application ID, and then like if you did, here, I'll just, for now,
[32:15] let's say we did application ID, and then zero, right? So what that is going to do, it's going to say,
[32:24] okay, look at the string application ID, and get the zeroth character.
[32:30] - Okay. - Which is S.
[32:34] So that's gonna return, that would return S. That would give you S.
[32:40] - Okay. - If you wanted application ID one,
[32:45] that would give you A. So it just goes zero, one, two, three, four, five,
[32:56] all the way to the end. And you could also say, you know, application ID dot length.
[33:03] It has a length property that you can access. I can't remember if there's, that's a function,
[33:09] or if it's just length, but that would give you the length, like how many characters long this is.
[33:15] - Okay. - So just some things about strings,
[33:23] and about like accessing strings, and kind of, we're not manipulating them yet,
[33:28] but just some stuff about strings. And that is actually across languages.
[33:36] - Okay. - That's in Python, that's in JavaScript, that's in Java,
[33:40] that's in C++, C#, like all these languages that I've dealt with,
[33:45] all of them have a way of dealing with strings, and all of them, they're stored as arrays.
[33:51] In some cases, they are, well, I'm not gonna get into that,
[33:55] but we don't need to get into that. - Okay.
[33:58] As a total side note, after writing this all out, it looks like awake and fetch are underlined for me.
[34:09] And I'm wondering, is that just because we're not to what it's gonna be using?
[34:15] Because right now it says parsing error, missing semicolon for awake, and--
[34:22] - For await? Oh, oh, oh, that's why.
[34:26] Me and dyslexia. Like, this is gonna be, oh my gosh.
[34:32] Oh, hey, what do you know, it's itself. - All right, so I'm not sure how far down the rabbit hole
[34:40] you wanna go. Basically, await and async, they go together.
[34:46] - Okay. - So there are different,
[34:48] so JavaScript is an asynchronous language, meaning JavaScript doesn't just execute first line,
[34:53] second line, third line, fourth line, fifth line. It doesn't execute like that.
[34:57] There are ways that you can introduce things to control when functions are called
[35:09] or when this line is executed. You can actually, like, for instance,
[35:14] you can go to a database. Maybe you're going to a database
[35:18] and you wanna wait until that database returns with a value before you continue your execution.
[35:25] Does that make sense? So in this case, this card tokenized response received,
[35:31] right, we want it to set our value or to do this alert. We want it to do that after we have fetched this data from,
[35:46] after we've gotten a response from the database or from our backend.
[35:50] - That makes sense. - Okay, so you don't want it before that, right?
[35:54] You want it to be able to process. If there's an error, you want it to return that error
[35:58] and give you good information. So this is kind of getting into a RESTful API.
[36:06] Somebody, I think, might be coming on and doing REST with you. - Yes.
[36:11] - So some of this is gonna be, like I was saying, like this brings up together a whole bunch of different,
[36:17] you know, I'm blanking out. - No, like there's, they all interconnect
[36:27] at some way or another and- - Concepts.
[36:31] - Yes, like there's so much out there in the world which makes this show really fun because at the moment,
[36:37] I'm just kind of like scraping the surface of everything instead of diving in deep.
[36:43] And a big reason I'm doing that is because I feel like so many newbies are asked,
[36:50] well, what do you wanna do with it? Like, what do you want to learn?
[36:53] Do you wanna be backend or front end or full stack or like figuring all that out?
[36:57] And I'm like, I don't even know. - You don't know enough to make that decision yet.
[37:02] - Yeah. - Yeah. - So I'm excited to, for this month that we,
[37:07] I was able to focus on a lot more of JavaScript. So that way I feel like I have a bit of an understanding
[37:14] before I at least see examples of Python. Now, one day trying to understand GraphQL,
[37:22] I'm not sure if I'll ever get there, but for today, figuring out web payments.
[37:29] - Yeah, so do you have this whole function here? - Yes.
[37:35] - Okay, and are you, you have the await here? The await response.
[37:41] So again, there's one async here inside this bracket. And it's saying, okay, this is gonna be an asynchronous,
[37:56] this is gonna be an asynchronous operation. And I want you to wait on this FEST request
[38:03] going to api/pay. And then I also want you to await the response.json.
[38:11] So, once this response happens and then converting it to JSON, right?
[38:20] There's what's called a promise and I'm not gonna get into what promises are,
[38:24] but basically I want you to wait for this to complete. And then I want you to execute the rest of this.
[38:32] JSON.stringify, which we already saw, it's taking JSON and turning it into a JSON string,
[38:38] basically putting quotes around it. So it could be, you know, parsed by, you know,
[38:42] the web parser. And then this alert,
[38:46] have you ever seen something pop up on your, in a little box on your web browser?
[38:51] That's an alert. So what we wanna do is we wanna actually alert the response.
[38:58] And it's going to be in JSON and we'll go through it and look at, you know,
[39:05] when we get the response, what it says, assuming, you know, we get a successful one.
[39:10] Okay. And then the last thing we want here
[39:15] inside of our payment form is our location ID. And this just identifies the location of the merchant
[39:31] that is taking the payment. And that's from the Square application dashboard,
[39:36] the location step. Uh-oh, I can't hear you.
[39:46] - I muted myself because I was drinking water. I didn't think you wanted to hear me drink water.
[39:53] Okay, now I was just gonna say, I really, I'm glad that the other day
[39:58] I copy and pasted all three because I was like, I don't remember how to get there.
[40:03] And now I understand why you're supposed to take notes on this stuff.
[40:07] I'll get there. I am excited for Anthony to come on the show
[40:11] and teach me about that. All right, so I'm seeing how that's done.
[40:18] Curiosity on the note on component for taking credit card payments.
[40:26] That one is inside of curly brackets. - This is actually a comment.
[40:32] - Oh. - And because JSX is not HTML
[40:37] and it's not JavaScript necessarily, it's both of them put together.
[40:43] Instead of just doing that where you would take a comment, you put a comment there.
[40:49] That's how you do a comment, by the way, in JavaScript. - Yeah.
[40:52] - You actually would say, okay, this is JavaScript right here.
[40:57] So it knows how to parse it. And then you put the component inside of there.
[41:03] So it doesn't think that this is some JSX or HTML. - Okay, and then why on line 31 do we have a bracket
[41:12] or not a bracket? - Because this closes out this component.
[41:21] - Oh, okay. - These, remember how I showed you
[41:26] there were arguments that go to this function? - Yeah.
[41:33] - Say customer, seller. And those things are properties of the function.
[41:40] Well, these things, they're much more long and drawn out, but these are properties of this component.
[41:53] - Okay. - They're essentially properties being passed into the component.
[41:58] Application ID, card tokenized response received, that whole function, alert.
[42:04] Actually, I think that's inside of card tokenized response received, it is.
[42:09] And then location ID. So there's those three properties.
[42:14] Application ID, this function, and this alert. Now in JavaScript, yes, you can pass functions as,
[42:22] you can pass functions to other functions. Those are called callback functions.
[42:28] - Makes sense. I'm looking at the documentation,
[42:31] that's why I'm staring at the other screen. - Oh, okay. - Is to see
[42:34] if I can follow along if I were just looking at the documentation.
[42:38] Okay, I'm seeing where we're at now. I see where we're at, and then.
[42:45] - Good job, looking at the docs. - I'm learning, I'm working on it.
[42:51] Okay. Okay, I thought I had it,
[42:58] and it's like close, but not close. Oh, that's why.
[43:10] Because I was looking at card payments, but not payment form.
[43:16] And payment form is gonna be different than card payment, because we're gonna do card payment next.
[43:22] - Yes. - Right? Okay. - Yes.
[43:24] So payment form needs to be there, I think, for all of the payment types.
[43:28] So they all need the payment form. Then the payment type goes there
[43:35] in addition to the payment form. It comes after it or before it.
[43:41] But essentially, like here with credit card, all we have to do,
[43:46] and the cool thing that I wanted to show you, all you have to do, because we imported it,
[43:52] because this third party library is, we just do credit card, and then close.
[43:57] We close it out, and then boom, we have a credit card payment.
[44:00] - So I guess where I'm stuck, if I'm like looking at the documentation,
[44:05] is I remember when you were showing us and looking at web payments,
[44:16] it said that it needed the payment form,
[44:25] but I'm not seeing how the payment forms are added on their documentation.
[44:35] - On Square's documentation? - Yeah.
[44:39] - Okay, so remember, Square has just a bare SDK. - Oh.
[44:46] - And they give an example, but it's just in HTML and plain JavaScript.
[44:52] - Okay. - It's not specific to React.
[44:55] It's not specific to Python or anything. It's just an example with index and index,
[45:02] I'm sorry, index HTML, which with HTML and JavaScript
[45:08] that you can use in any of those environments. And then they actually,
[45:12] Square has also published extra tutorials on React, Index, and on these different platforms
[45:21] or these different frameworks. - Got it, so that's why the credit card
[45:26] or card payment is showing, but not payment form, is because payment form is much more universal
[45:34] for all payment forms? - Yeah, all types of payment, yep.
[45:38] - Okay. - And you'll see either payment form,
[45:41] I think it's payment form on the documentation, but you won't see like components
[45:48] because components are specific to React. - Okay.
[45:54] - And this third-party library has taken what Square has done
[45:58] and then has housed them all in components. So it's made a payment form component.
[46:02] It's made a credit card component, and it's made a payment ACH component.
[46:09] It's made a Afterpay component. So there's a,
[46:14] if you're already developing in React and you're making components,
[46:19] this makes it so much easier to implement because you just import it, right?
[46:24] You NPM install it, and then you import it, and then you can just use those components
[46:29] to add payments to your existing React app. - Yeah.
[46:35] Makes sense. It does make sense.
[46:40] I think it's gonna take me a hot minute to get there of like fully, fully understanding it,
[46:46] but it definitely does make sense now how to implement it later on.
[46:52] You know, I will get there. - Yeah, you're getting introduced to Square.
[46:56] You're getting introduced to some JavaScript promises. You're getting introduced to like RESTful APIs.
[47:03] It's like a whole, it's a lot of stuff. It's a lot of stuff at once.
[47:06] - But I feel like, I will say, I feel very fortunate getting introduced
[47:11] to all of it at once because that's kind of how my brain works
[47:15] is just, you know, being able to take in all the information to know,
[47:21] okay, that's how what I'm learning right now will connect to X, Y, Z.
[47:26] So, and then really quick for the account charge, did you just put in random things right there?
[47:37] - Yes, I just, I was trying to be funny. You know how people usually say John Doe?
[47:43] - Yeah. - I just put John don't.
[47:46] - I get ya, I get ya. I just wanted to make sure I didn't have to like
[47:48] literally say that, but. - Yeah, so ACH for a direct debit,
[47:53] you do need an account holder. You need a redirect URI and you need a transaction ID.
[47:58] So I just like made up, you know, five, four, three, two, one and just example.com,
[48:03] which, oh, look at this. Moot Woot is in the house.
[48:10] - What up? - What up?
[48:13] I don't know if I should say his real name. I'll just call him Moot Woot.
[48:15] He said, if you didn't use a wrapper, oh, you want to put that one on the screen?
[48:20] 'Cause that's really germane to what we're talking about. - Wait, what?
[48:26] - Do you want to put Moot Woot's comment on the screen? - Oh, thank you.
[48:30] I was like, wait, what are we talking about? - He said, if you didn't use the wrapper,
[48:35] that's the, not the wrapper, not me, but dad joke. If you didn't use the wrapper,
[48:43] that's the third party library that we're importing, using to import our components.
[48:50] He said, you would need to code up a way to delay rendering React
[48:55] because the Square JavaScript loads async in the browser. - Oh, okay.
[49:01] - He's typing, he's typing. - Yeah, the React Square web payments SDK library.
[49:09] - Yeah, yep, yep. - Okay.
[49:12] - Exactly. - It's definitely a lot to learn.
[49:17] Something that may be a bit interesting of, every time that I've created the account holder name
[49:27] and then redirect URI, it's creating a single quote instead of a double quote.
[49:34] And... - You mean by default?
[49:38] - Yeah. - Yeah, I think it's, I think, I believe it's convention,
[49:45] but I, the convention I was using was double quotes. So let's just stick with double quotes.
[49:53] - Okay, I just wanted to know if it was like something I needed to be concerned about,
[50:00] or if it's just like, you know, because I've been told about,
[50:03] you can also change a lot of the structure of what it defaults to do.
[50:12] So I just wanted to make sense. It wasn't like a code issue.
[50:17] - Yeah, what I like to do is, I like to have my outer, is this right?
[50:26] Is my brain dying? I usually, I think I have my outer.
[50:31] So let's say you have like quotes and within those quotes, you need another quote, right?
[50:36] - Okay. - I usually like to have my outer quotes be double.
[50:40] And then like, if I have to have an escape character, then like, then it can be single.
[50:45] But I like to have the outer ones double and the inner ones, you know, single.
[50:49] Like John don't, I guess I could have escaped that. Anyways, yeah.
[50:56] Anyways, it's just, it's just convention, but. - Okay.
[50:59] - Double, there you go. - Cool, yay.
[51:01] Then if I bring up my local host again. Oh, okay.
[51:07] Now I gotta like show everybody because this is cool. I might be getting, skipping ahead, but look.
[51:14] - Look at that. Oh, I'm so happy I knocked something over.
[51:19] Look at that. - We did it.
[51:22] We did it. Okay, so that's, yes, that's cool.
[51:26] One of the things you're gonna need is you're gonna need, I think you're gonna need values,
[51:33] but I think I remember what they are 'cause I've done this too, done this so many times.
[51:37] You can just click on Chase. - Oh, okay.
[51:41] - Let's just use Chase Bank. Okay, and I think it's user underscore good.
[51:53] And this is on the documentation, so I'm not like revealing anything, you know, super secret.
[52:00] And I think it's past good. - With a capital P.
[52:04] - Just a lowercase P-A-S-S underscore good. - Check your passwords.
[52:14] Never, all right. Let's do, you know, savings counter.
[52:19] - We'll do savings, okay, all right. - Continue, and this is success.
[52:24] All right. - Yay. - There you go.
[52:28] You see that? What does that say?
[52:29] - See, this one says John Doe. I didn't actually name mine John Doe,
[52:34] but it just uses the default of what, of that account, right?
[52:41] - Yes, that's what, remember that's what we passed in as a prop to account holder?
[52:45] - Yeah, okay. - I'm sorry, it's the ACH. The account holder name was John Doe,
[52:49] so it returned, you know, John Doe. - Even though like yours, for example, says John don't.
[52:56] - Oh, that is a good point. - Because like, look, I named my account holder, hi.
[53:03] - Oh, ho, ho, ho, that is very interesting. Let's open up your,
[53:09] we're gonna have to do some troubleshooting here. - Well, I'm wondering if it's because the square account
[53:15] is to John Doe. That's what I'm wondering.
[53:17] If that's why, or not the square account, but the- - Square API.
[53:23] - That, but the credit card, Chase. Chase account is to John Doe.
[53:27] Look for your alert function call. - Hmm, that's the same thing.
[53:46] - I mean, so it should be alerting. Let's look at your developer tools
[53:56] and look at what is happening. Now, exactly, now we have a puzzle.
[54:05] Now he's with me. - Okay, inspect.
[54:11] - Inspect. And then I don't fully understand what all of these are for.
[54:18] So would I go to console? - Let's go to console.
[54:23] Let's just see if anything was logged on the console. Unchecked runtime last error, loss.
[54:33] No message port. - Actually, I've run into this one before.
[54:39] Hold on. This is where it closed before.
[54:44] - It's plugins, extensions, turn them all off. I don't know if that's causing the other one,
[54:52] but that is what causes that error. - Okay, so we can try to go through again
[55:01] after having eliminated that one thing. Let's see what happens.
[55:08] - Okay, hold on. - Let's move this down, move this one down.
[55:11] - User. User, good.
[55:25] - And then- - Past, good.
[55:30] - Underscore, good. Emits.
[55:35] Close. Now.
[55:39] - Just try checking. - Okay, then I'm gonna do...
[55:45] Nope, still John Doe. - Still John Doe.
[55:50] That is interesting. Let's look at the CLI.
[55:54] So this is your server side. - Moot was going to say go to the network tab
[56:08] and turn on recording of requests. - Oh.
[56:12] - Okay. - Cool.
[56:13] - Network tab. - I was just thinking about the network tab.
[56:16] I was like, we go to the network tab or we could go to your server side.
[56:19] But yeah, that's- - No, we don't want beat.
[56:25] We don't need to invert it. - There's a, looks like there's a record button.
[56:32] - Yep. I think it's recording now.
[56:35] I'm guessing. - Are you recording?
[56:40] I guess we'll find out. - So what we want to do is do another request.
[56:47] There you go. - I don't know if it's recording though.
[57:03] - Your filter should change from JS to. Oh.
[57:12] It's under, should I change my filter then? - To fetch?
[57:19] - Yeah. - Yeah.
[57:21] - Okay. There we go.
[57:23] Fetch. Sweet.
[57:29] The last time I did that stuff was with Nishko that built quick because he was showing me like load times.
[57:41] It was so cool. - Yeah.
[57:43] - Never continue because it was same for checking I'm doing savings again.
[57:53] - Yep. - And then stop.
[57:59] - Oh, interesting. I didn't see a fetch request.
[58:07] And I'm actually seeing an error on your server side. Like in your.
[58:14] (murmurs) Unhandled rejection, error aborted.
[58:31] Connection reset exception. Socket.
[58:37] Oh, you know what's happening? - What?
[58:45] - I just realized we have API/pay but we haven't built the backend.
[58:51] - 'Cause I got excited to see it. - Yeah, yeah, yeah.
[58:55] - Okay, well, you know, using that content, it works. - Yep.
[59:03] - I will learn that. I will learn that.
[59:06] Follow directions and don't get too excited to skip ahead. - I mean, we could set it up so it runs without the backend
[59:12] but you know, we might as well just set the backend up. - Yes, I dig it.
[59:17] Do you have time? Because we're right at the hour mark
[59:20] and I have another half hour before I need to go do anything so I feel like we can do this.
[59:25] - We can do this, we can do it fast. - All right.
[59:28] - So what you wanna do is I'm gonna go to pay.js. Remember we.
[59:36] - Here we go. - Set up that file.
[59:41] - Yes. - It's in API.
[59:48] API, there you go. And then pay.js, there we go.
[59:51] All right, so what we wanna do is we wanna import client. - Okay.
[59:57] - Can you see my screen? Can you see my screen?
[60:00] - No, let me go back to your screen. - Okay.
[60:02] All right, so let me make this big. - Yay, thank you.
[60:07] - We're gonna import client from Square. - Okay.
[60:11] - And we need that to create an instance of client. Remember you're talking about object-oriented, right?
[60:19] So client is the class and then we wanna create an object, an instance of that class.
[60:27] And remember your imports are in, your external imports are in quotes.
[60:37] - Yes. - You're gonna import random UUID from crypto.
[60:45] And I mean, without getting too deep in the weeds, I have a comment about it,
[60:54] but it's basically gonna generate a random and unique number up to a certain percentage.
[61:04] - Okay. That's gonna be fun.
[61:09] - Yeah. - Because me and crypto, we're not even there yet.
[61:14] And that's like what Anthony, who was hanging out with us the other day, what he does.
[61:20] And when I first met him, he was just like, don't even look at it yet.
[61:24] Just don't worry about trying to understand all of that. - And this isn't like cryptocurrency, this is cryptography.
[61:33] This is a branch of, I guess, cybersecurity. So it's gonna be used to generate a number
[61:42] that has a key that is attached to the block of information that you get from the front end.
[61:50] - Okay. - Yeah.
[61:57] - So I got my imports done and then the next one is the- - BigInt.prototype.toJSON.
[62:05] And then you wanna do function and then return this to string.
[62:10] This is gonna allow you to stringify BigInt, it's basically long numbers.
[62:16] It was just something that we have to, I was like, I actually went on Stack Overflow
[62:24] and looked this up and it was just like kind of a rabbit hole but I was just like, okay, I just need to just include it
[62:34] because if I wanna have long numbers, for instance, a long account number,
[62:41] and I wanna be able to convert it to string, then I'm gonna need this.
[62:46] And there are different types of ints and there's like what's called a BigInt,
[62:52] which is one of the types of ints. Integers, when I say int.
[62:58] - Okay, cool. - Okay, and then the next thing is
[63:05] creating this instance of payments API. I'm sorry, the instance of client
[63:09] and calling it payments API. So you wanna do const payments API and then do client.
[63:14] And then in new client as a parameter, you wanna pass in a object
[63:22] with two key value pairs, one access token and then process.env.squareAccessToken.
[63:32] Now remember that square access token? We created that last time or we didn't create it.
[63:39] We got it from the square dashboard. - And we created the env.local, right?
[63:45] - Yep, we put it in that file. - Okay, cool.
[63:48] - So this should work. Since it's in the root folder, it should find it.
[63:52] - Can you move your mouse a little bit? - Oh, sorry.
[63:57] - I like that, your way of teaching this, of taking it off of your screen,
[64:01] because it's like getting me used to seeing what you've written
[64:06] and getting used to writing it myself, but then being able to look for my own errors,
[64:14] which is really annoying. - It's a scaffolding, it's a scaffolding technique
[64:19] because some people learn visually, some people learn by hearing,
[64:23] some people learn by tactile, actually typing. And this allows multiple modalities
[64:32] when someone is learning, because I'm actually explaining as I'm going through,
[64:36] but you're also seeing it and then you're also typing it. So it's like three of the four main modalities.
[64:42] - Oh, geez, that's a... Yeah, because I definitely do better by hearing,
[64:49] but then being able to see it and type it myself, you're right, I'm like, okay, cool.
[64:54] I have something to compare it to as well, which makes it a lot easier to see,
[64:59] oh, did I get that right? Which granted, I didn't see that I typed await as away.
[65:06] - Right. - At least that one was a little easier to find.
[65:12] - Yeah, and as you do this more and you kind of get used to some of the JavaScript conventions
[65:19] you'll be like, oh, this is a async await, the async await, like I've seen it a bunch of times.
[65:24] So when I see like an async, I'm like, oh, okay, I know what that is.
[65:28] But it just takes like doing it over and over and over again you start to get used to those things.
[65:33] And you start to write them yourself when you're writing applications.
[65:38] Now I put some console logs in here, they're not necessary. They were like for troubleshooting purposes.
[65:47] - Okay, I'm just getting a parsing error for new with a comma, like in front of new for new client.
[66:01] - Oh, can you show your screen please? - Yeah.
[66:03] There we go. Right here.
[66:08] - You're missing an equal sign. - Oh my God.
[66:12] - Where? - Right after payment API and then the close braces.
[66:18] Now, let me take a second to explain what's happening here. This is actually called object destructuring
[66:27] and it's a very, very complicated term. But basically what it's gonna do is this,
[66:34] it's going to go into a client. It's gonna see if it can find a key payments API
[66:42] and it's going to save what you're creating into a variable called payments API.
[66:49] - Okay. - So it's gonna see if there's something matching.
[66:54] The same thing with client from square. It's gonna look in the square library
[67:00] or the square NPM registry or whatever and see if there's something called client.
[67:06] And then it's going to create a variable called client and save it in there.
[67:10] And now you can use it in this file. - Got it, okay.
[67:15] - That's what that notation is. It's object destructuring.
[67:18] - Okay, so that made sense. And I'm just taking a look.
[67:22] Oh, okay, this is gonna be something that I just got to learn how to see.
[67:28] Like I was staring at the new client thing before asking you and you're like,
[67:33] you're missing your equals. And I'm like, dude, I've been staring at this.
[67:35] Why didn't I register that I'm missing the equals? I'm gonna learn.
[67:40] - It's gonna happen. - Oh.
[67:42] - I'm like missing stuff, it's really annoying. But I'm not the only one that does it.
[67:48] And learning from other people that are dyslexic, it's gonna be good.
[67:55] - Yay, yay. - It's gonna take me a minute.
[67:59] - Yeah, so this, notice there's an export here, an export default.
[68:05] So there has to be a default export. From your JavaScript file in the next,
[68:14] in the React ecosystem. So this one specifically says this function
[68:21] is going to be your default export. And it's also gonna be an async function.
[68:27] So there's that async word again. So this is-- - Means there's an await.
[68:31] - Yeah, there's gonna be another await that pairs with that, at least one,
[68:35] that pairs with that async. Now, the first one is we have an if check.
[68:41] If the request method is post, remember our front end, it was the post request.
[68:47] That means like a post request could be like, you're sending information to a database
[68:53] and you want that database to save it. But you have to send them the information
[68:57] that you want it to save. So in the body of that post request
[69:02] would be the information that you want. And it could be, it has to be stringified.
[69:10] We did that stringification, json.stringify. But this request.method, this standard REQ,
[69:18] this is being passed into the handler, request and the response.
[69:25] So there's a request to an HTTP request and there's an HTTP response.
[69:31] So it's going to take your request and it's going to look at the method on your request,
[69:35] which we sent in the fetch request. And we remember we named it post.
[69:41] If we go back to index.js and we go here to this fetch, here's our method.
[69:48] - We called it post. - We called it post.
[69:50] So it's going to look at that object and look at the method key and see if it's post.
[69:57] - Okay. - And so, yeah, that's the first thing.
[70:06] - Why are there three equals for require method post? - So yeah, there's single equals
[70:17] in JavaScript is assignment. That's when you're assigning one value
[70:22] to another value in memory. - Okay.
[70:25] - Double equals is when you're checking to see if two things are the same,
[70:30] but if they aren't the same type, it's going to change the type of one of those things
[70:35] to match the other. And I think it's the second to match the first.
[70:40] I believe that's how it is. It might be the other way around.
[70:42] But it's basically, it has type conversion. Triple equals means it compares their value
[70:52] and it compares their type. And they have to be both equal in order for that to be true.
[70:59] So double equals, their type doesn't have to be the same. So like one can be an integer and one can be a string.
[71:05] You can compare, like for instance, let's see here. Like, let's say if I just wanted to do,
[71:12] if six equals, whoops, equals six, right? That would come back false
[71:29] because yes, they're both sixes, but this is a string six and this is a number six
[71:40] or an integer. - Okay.
[71:43] - If I did this double equals, that would be true. - I'm getting it, not getting it.
[71:52] - 'Cause it's going to change, like it would change this six to a string
[71:57] or change this to a number. - Okay.
[72:01] - So in memory, it would be going, oh, hey, this is what I see.
[72:10] Those are equal, true. Says, okay, that if check is true.
[72:15] Oh, that's what that triple equals mean. It's the deep equals
[72:21] where it doesn't do any type conversion. It doesn't convert the type.
[72:26] It just compares them as they are to see if they're exactly equal.
[72:30] - I'm missing something, so I'm trying to find what I'm missing.
[72:40] - Oh, okay. (indistinct)
[72:43] - Because you said that I don't need the console log, right? - No, you don't.
[73:02] - And then do I, oh, I need rest status though and rest that you rest status.
[73:12] - Yes, those are very important. So what RES is,
[73:18] remember there's request and response. So this is going to say,
[73:23] assuming everything is happy and you get a good response, it's going to return 200 and then JSONify the results
[73:32] and return the result, which is this very,
[73:36] what's stored in this variable from create payment. And I wanted to mention that,
[73:43] remember there was two things you had to do. You had to initiate a payment
[73:50] and you had to generate a token. You also need a backend to actually process that token.
[73:57] And that's what this backend, that simple backend code is doing
[74:02] is processing that token that we got from the front end. So, that's just how the Square API works.
[74:12] They want to make sure double, triple check. And if you initiate a credit card payment, for instance,
[74:20] it checks the credit card and make sure it's valid, right? And make sure any other information associated is valid.
[74:27] And then it sends, once it gets a success and it generates a token,
[74:32] then it sends it to the backend or wherever backend you want to send it to.
[74:37] And then, that backend needs to process the token. So, you have to make some logic to process the token.
[74:46] - I get it in theory. I think some of this is still the, I'll get there.
[74:54] I will understand the words you're saying. - A token really is just a, it's just a long number.
[75:04] And it's this token means this was a valid, this was a valid Square transaction that just happened.
[75:13] It's like if you buy something at a store. - Sorry, I got a, for my export
[75:27] default async function handler, it says parsing error identifier handler has already been,
[75:35] trying to move so I can see. - Oh, you can go ahead and share your screen.
[75:41] - Okay. Gonna be mad if it's another like comma.
[75:58] Yeah, so parsing error identify handler has already been declared 1530.
[76:06] Oh, up here. Oh, because this was already here.
[76:20] So, I can delete this one, right? - Yep. - Because this one
[76:23] was already here. - Yep.
[76:25] Yeah, you can only have one default. - Okay, well, and then am I done?
[76:33] Do I get to test it? - Yes, you do.
[76:40] - Yay. - That is your reward.
[76:44] - And it is making a lot of sense. Like looking at it,
[76:50] I feel like I could at least figure my way through it. Now, I don't think I'll remember exactly
[77:00] how to reset it up by myself, but I would at least be like, okay, cool.
[77:04] I think I can read enough of it, which it is definitely getting easier as I have these.
[77:12] Oh, and Moot Woot, I know that I've been very excited
[77:17] about learning all of this right now. How's filming?
[77:25] They just released a new video I saw pop up on my phone. Square.
[77:32] - Oh, I should check it out then. - Yeah, they're on their YouTube channel.
[77:36] - All right, I'm gonna do checking just to see if it works. I'm glad to hear that it was great.
[77:45] I didn't get any pop-up. - Okay, let's go back.
[77:53] Unauthorized, okay, let's read that. Authentication error, okay.
[78:02] - Trying to make it bigger to read it all. HTTP header of your request was incorrect or expired.
[78:14] The header value is expected to be in the format bearer token without quotation marks
[78:20] where the token is. So, I just need to call it bearer token instead of token.
[78:25] Ooh, okay, I'll definitely have to check out that Moot Woot. I can, maybe I'll watch it to see if I can replicate this.
[78:50] (mouse clicking) - Yes, did he just say he, I can't see the comments,
[79:00] but did he just say he has a YouTube channel where he walks through building a next React app?
[79:06] - A React Web Payments SDK. - Yeah, it's, yes.
[79:12] - He just said we should check the ENVE file and how you're importing the access token
[79:19] when initializing the square node SDK. So, that would be my ENVE file.
[79:27] I named it square access token. - You're missing a C.
[79:31] It says access. - This is gonna drive me freaking bonkers.
[79:43] Like, I'm looking at it and it looks fine. - Welcome to software development.
[79:48] - Make sure you save the file. There you go, yeah.
[79:52] - All right, so. - We're gonna need to rerun that unless it ran, reran.
[79:58] Oh yeah, okay, yep. Here we go, here we go.
[80:02] - Oh my goodness. - Every time I see that user good, cast good,
[80:14] I always think of Joey or the Hulk. - Oh, that's funny.
[80:20] - Or Joey on friends. - Meet good.
[80:25] - Okay, do we have it? Please work, continue, okay.
[80:30] Oh, it's at this unauthorized authentication error bearer app.
[80:45] Or bearer token. K.js file.
[80:55] - Yeah, it's your backend. - Square access token is access token.
[81:06] I got my C's and my S's, at least this time. - Mm-hmm.
[81:10] - Okay. - Create payment amount money.
[81:22] Just for kicks, let's go back to, where did I have it?
[81:32] Our config file. - Which is an API, no.
[81:40] - Next config.js, yeah. And let's put in, you know what I had before?
[81:52] The env as a key, above react strict mode true. You're gonna put in env with a colon.
[82:05] And then open brace. - That one?
[82:18] - Yep. - Okay.
[82:20] - And you're gonna need a comma after the brace, the last brace.
[82:24] - Goodness gracious. You need to tell Amory.
[82:28] I keep telling her that I'm doing lives right now and she's gonna keep calling.
[82:32] We'll talk later. Okay, env close brackets, comma.
[82:37] - Yep, and then just in there, you're gonna put in square access token.
[82:41] - In the brackets? - Yep.
[82:46] - I'm trying to, am I putting it where it has the token information
[82:59] or am I putting it just the file name? - What we're gonna try,
[83:04] we're gonna try to put the token in. - So the actual numbers?
[83:10] - Yes. It's a long stream.
[83:17] Should be. - Okay, and since this is just me doing some,
[83:27] oh, it says, oh, that we may just have needed to restart the server.
[83:38] So if I remember correctly, then I can just do, save our spot just in case.
[83:49] All right, and then restart our server. All right, and do these, do these, do these, do these.
[84:00] These are good. Close, never, checking, continue.
[84:29] It really likes the bearer token. Okay, so.
[84:50] - Incorrect or expired. - Yeah.
[84:52] Chttps developer.square.com docs build, oh, you got it.
[85:09] There we go. - Yeah, let's do this.
[85:11] Wait. - Okay.
[85:17] - Yeah, I'm gonna need to jump off here in a second. - Okay.
[85:30] - Not right now, but just. - Yeah, no, you're good.
[85:33] I was just gonna say. - I believe so.
[85:43] He asked, am I using the sandbox token that matches the application ID
[85:49] that I have set in my payment form? - Yeah, I mean, we can go back and on your dashboard,
[85:57] just make sure that that's, those things match up. - I feel like if I remember correctly,
[86:09] it was really hard to get back to the screen that showed like the sandboxes.
[86:16] Oh, apparently not, 'cause it's developer.square.com/apps.
[86:25] developer.square.com/apps. Okay.
[86:42] And I need to sandbox token that matches my application ID you have set.
[86:50] - Yeah, you wanna go to open. - On this one?
[86:52] - Yep. So yeah, and then scroll down.
[86:59] So this is a sandbox and there's your access token right there.
[87:04] - Okay, so. Well, you guys can see this one
[87:10] 'cause I'm learning, but I know that you're normally not gonna do this
[87:16] because it's not what you're supposed to do. Nobody needs to know this stuff.
[87:22] Okay, save. - Just make sure we restart the server this time.
[87:29] - Okay. Okay.
[87:38] Okay. Wait, there we go.
[87:42] All right. Yes, 'cause knowing me,
[87:51] it was a copy and paste error or something. Oh, the credentials you provided
[88:07] were incorrect, okay. User_good.
[88:11] Pass_good. Close.
[88:24] Never checking. Continue.
[88:27] Continue. Same error.
[88:35] - Oh. - Hmm.
[88:38] - Wow. This does make it tricky.
[88:49] - Yeah, it does. - And this is like- - A little frustrating.
[88:54] - Yes, yes. And I would say, you know,
[88:57] a little bit about why we learn and, you know, going in looking for the errors.
[89:02] And I mean, at this point, I feel like I have a good idea
[89:07] of what's going on. And maybe, yeah,
[89:12] I'll double check my application ID before we go. I'm gonna put this server really quick.
[89:17] Application ID is in my index file. Yeah.
[89:24] All right. But then my sandbox application ID is right here.
[89:33] And I'm gonna put it here and we paste it. - Yeah, it doesn't look like it changed.
[89:41] - And we have here. New.
[89:45] New. Wait. - I'm curious.
[89:54] Oh, go ahead. - I'm gonna do an incognito, just to be sure.
[89:59] (mouse clicking) Hey.
[90:05] Continue. Chase.
[90:10] User_good. (mouse clicking)
[90:19] Yay. Yay.
[90:26] Continue. No go.
[90:30] - Same error. - Yep.
[90:33] So we're getting a successful generation of the token, it looks like.
[90:41] But it's actually the processing of that token on the backend where we are getting some trouble.
[90:49] - Did they have a temporary credit card I could use? - Yep.
[90:58] Yeah, so we could try credit card. - Let's just see if that, so what?
[91:04] - Go to the, yeah, go to there. And you want to...
[91:10] Go, I can't remember exactly where it is, but if you go through here, you're probably.
[91:24] So it was like four, one, one, one, one, one, one, one, one. I actually think I might-- - Oh.
[91:32] Whatever you want for those ones. Okay, cool.
[91:34] (humming) Oh, input card number.
[91:43] All right. Yeah, let's do it in incognito,
[91:52] just to make sure it's not caching. And I think that can just be something greater than today.
[91:58] One, one, one, four, six, oh, okay. That has to be a valid zip code.
[92:10] - Hey. (humming)
[92:22] - Okay, well, it didn't do anything. - Is your server running?
[92:29] - Yes. - Okay.
[92:34] - Not in sandbox, it can be whatever. Oh, in for a zip code.
[92:43] But it's not even registering that we're doing anything. It's just doing.
[92:50] (humming) Yeah, I'm gonna need to jump off here.
[92:56] - Yeah, for sure. - Sorry to leave you hanging.
[92:57] But-- - No, it's good. - We can come back to this and finish out the last flourish.
[93:04] Clearing this error, essentially. - I'm gonna work on trying to figure it out.
[93:11] Now I'm like, maybe this is what I'm gonna do for my first thing, to do it on my own.
[93:17] Although it gets really confusing not understanding it all. - Yeah.
[93:21] - But Moot Loot is gonna be on the show, too. So hopefully we get it figured out by then.
[93:26] - Yeah, you can send me the stack trace from your command line.
[93:31] You can also just get the main error message and Google that.
[93:37] You'll come up with some different stack overflow examples of people doing authorization of bear token.
[93:46] You can add plus square. If people have run into those same issues before
[93:52] and what they had to do. Checking the environment local file.
[93:59] Checking your application ID. Checking where it's stored.
[94:04] All of those things. - Cool, cool.
[94:07] And yes, I do. Thank you for giving me the Slack URL
[94:11] 'cause I need to download that for so many Slacks. I don't know how everybody keeps up with all of the Slacks
[94:21] in Discord and forums and Twitter and LinkedIn. It's a lot.
[94:26] - They're multiplying. - They are.
[94:28] Well, thank you so much. I appreciate you both for tuning in
[94:33] and helping us through this. And I'll post if I figure it out on my own.
[94:38] - Okay, sounds good. - Sounds good. - Till next time, Bakari.
[94:40] Talk soon. - Yeah, okay, see ya.

