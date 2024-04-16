---
showLink: "https://www.youtube.com/watch?v=0kLczFLBB30"
channel: "Jenn Junod"
channelURL: "https://www.youtube.com/@jennjunod"
slug: "teach-jenn-introduction-to-backend-development-with-express-js-part-2"
title: "Teach Jenn: Introduction to backend development with express.js Part 2"
publishDate: "2022-07-18"
coverImage: "https://i.ytimg.com/vi/0kLczFLBB30/maxresdefault.jpg"
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

[00:00] >> Hello, beautiful humans. Welcome back to Teach Gen Tech.
[00:06] We're starting our week off again, which I'm pretty excited about, with Ramon again.
[00:11] >> Hey, how are we all doing? >> That is one of my favorite parts
[00:16] because you're always so delightful. It's a good way for the rest of us to start our week off.
[00:23] >> It's a joy. I had such a good time last time. I'm excited to hop back on and do it again.
[00:30] >> Yay. As a heads up everyone, Ramon, if you are just catching the live today,
[00:39] Ramon was on the show last Monday and we were learning about back-end development with Express and JS,
[00:52] and we did not get through everything. This is why you're back.
[00:57] >> Yes. What we did, we got started in some Express.
[01:03] Yes, we added one endpoint to our app. We need to expand a little bit on our API,
[01:12] and also add a database layer to it, which is going to be super fun.
[01:17] >> If anybody wants to check out the previous video, I just linked it in the chat.
[01:26] If you need to catch up there, you will be able to find it.
[01:30] We did go ahead and get started on some terminal products because we
[01:38] needed to get set up and get us closer to just getting where we were last week, so here we go.
[01:45] >> Awesome. >> All right. We're there.
[01:48] We are in the Ramonas RAD folder, which is what we are calling this project.
[01:56] >> Who am I to argue with a folder name? >> Yes. That is where we are so far.
[02:04] Now we need to reopen everything, and I'm going to leave that up to you
[02:11] because I don't exactly know where to start again. >> Sure. We're going to open up the folder we're
[02:17] currently in in VS Code. Do you remember how to do that? >> Code, space, dot.
[02:25] >> That's it. >> Yay. Let's see if it works because I've had to do this with,
[02:31] it doesn't, and is it Command Shift P? >> Yeah.
[02:37] >> Okay. I keep enabling this. >> Oh, there it is.
[02:41] >> Yeah, and it's recently used. >> Well, that's odd.
[02:45] >> Yeah, so it just doesn't like me. >> That did it.
[02:54] >> It likes it that time. I have to install it every time.
[02:57] A little annoying, but that's okay. >> Maybe there's something to be done there with your shell settings.
[03:06] Shell being the program that runs commands in your terminal. >> That could be it. That totally could be it.
[03:12] >> Okay, cool. >> We got a quick comment.
[03:19] There's ZSH thing. Wow, I cannot say that from GoGoGadget.
[03:26] That is just a fun name. >> Hey, GoGoGadget. Good to see you.
[03:31] >> There's a new shell. Good to know. Wouldn't happen to have a link to that. Would you, GoGoGadget?
[03:39] >> That'd be super helpful, please. Cool. We've got our VS Code project here,
[03:46] which is our Express backend. Tell you what, let's quickly recap where we were
[03:53] and get ourselves back up to speed before we start messing around with it again.
[03:56] Sound good? >> Yes.
[03:59] >> Awesome. Let's open up App.js and see what this does. What we've got here is we import Express.
[04:09] We create an app based on that Express dependency. We declare one endpoint to
[04:18] the root path that responds with some HTML as a string saying BRB sometime in the next month.
[04:28] Then in line 8, yay, we're back. Love it. Yeah, that was sooner than we thought we'd be.
[04:37] >> Only a week. >> Then on line 8,
[04:41] we set up our server, which is the program that listens out for requests on port 3334,
[04:52] that when it starts up, it says, "Hey, I'm listening on this port."
[04:57] Let's confirm that that's what it's doing. To do that, we're going to run Node.
[05:06] >> Is it Node and then space App.js? >> That's right. We're telling Node, "Hey,
[05:16] run this file." Now it's listening. We can go to the browser,
[05:24] put this over, and then local.334. Yay, it worked.
[05:37] >> We can confirm that, hey, it updated. >> Yes.
[05:42] >> It ran, yay, we're back, which is great. What we're going to do next is start building out an API.
[05:50] Let's not have this return, "Yay, we're back," anymore.
[05:53] Let's instead return some data. Let's pretend we have an API.
[06:00] Google Gadget got us a link, thank you very much. >> Yay, thank you.
[06:05] >> Yeah. Let's remember, this all started last week from wanting to make
[06:13] an app where we would store kind words that are shared about us. You remember?
[06:21] >> Yes. >> Right. What is a kind word?
[06:28] What is it that we want to display? We would want to display a set of messages that
[06:33] consist of the name of the person that sent it to us. What else?
[06:42] >> The message itself. >> Message itself.
[06:47] Sorry? >> Date.
[06:50] >> Date. Perfect. Those three. These are called attributes.
[06:56] These are the three attributes that make up a single. Now we need to come up with a name of the entity.
[07:02] Entity being the thing that we're storing and querying for. Could call it posts,
[07:08] could call it words. No, it doesn't work. I'm for posts.
[07:14] >> Sure. I'm going to go with sure. Hey, Lee, thank you for joining.
[07:20] >> Hey. We're going to send off this data as a collection of posts.
[07:35] >> Okay. >> In order to do that,
[07:39] let's do some JavaScript. Let's hop online.
[07:45] Oh, yeah, we can kill our server. Awesome. Between lines 2 and 3,
[07:50] let's create a new line. We're going to define a const where we will store our posts.
[08:01] We could just call it posts. >> No. Const equals post or can I do const post?
[08:11] >> You were right, but it's a plural. This will be set to be equals an array.
[08:25] Do you remember how to declare an array in JavaScript? Not quite. We want to use the square bracket notation.
[08:39] This is an array. Right now, it's empty because there's nothing in it.
[08:46] >> Right. >> Let's put some data in it.
[08:52] These posts will be objects. We good with JavaScript objects?
[08:59] >> Yes. Good enough. >> Good enough is absolutely plenty.
[09:06] Let's create an object. That's done with the curly brackets.
[09:12] Let's hit "Enter". This object, as all posts,
[09:20] are just going to be made up of three attributes. The first one, let's call it,
[09:26] that's the name of the person who sent us the kind words, sender. >> Now, do I need to do value equals sender or something like that?
[09:39] >> No. These are key value pairs in JavaScript, which means it'll be lowercase key, colon, value.
[09:52] The key in this case is the name of the property, which is sender. Sender is the key.
[10:02] Remember, this is test data for us, so we'll put in a space and then a string.
[10:11] Now, we'll put in the name, any name. This is our test data.
[10:17] Let's start the one from, yes, you read my mind. You read my mind. Yes.
[10:25] That's our first key value pair. After the string,
[10:29] let's put in a comma, hit "Return". Now, we'll do the second attribute,
[10:36] which was message. >> Comment.
[10:40] >> Comment is good. >> Like message. No, it has to be lowercase.
[10:44] >> Yes. >> When you have to make some points differently.
[10:55] >> Yeah. I was like, I don't know, three? >> No, it's three. It's three. We're good.
[11:00] >> I'm glad that you were also like, I've got to get it right.
[11:03] >> I think it would be cool to say not drop my AirPods. That would be helpful.
[11:11] But to say not only the date, which that one's pretty easy.
[11:19] >> Oh, but don't forget we're adding a new attribute. >> Common.
[11:25] >> That's why you're getting the underline and the date. >> Today is July 18th.
[11:36] >> But be careful. Dates are not strings. They're displayed as strings.
[11:43] But in JavaScript, we have a special data type for dates. I can give it to you.
[11:52] It's capital D date. What you can do is remove the string quote marks,
[12:01] and we'll make a date. But the capital gives us
[12:06] the indication that this is a JavaScript class. We want to create a new space date.
[12:13] If you go back to the beginning of the, just before the capital D put in a new N-E-W,
[12:24] but not capital, space date, and let's remove that equals.
[12:37] Now, what we're doing is initializing a date. We want to put in, I call them smooth brackets,
[12:46] like I don't know if that's correct term. Always when putting brackets,
[12:51] we want to not leave a space between the bracket and the keyword. That was a lot. What have we done here?
[12:59] We have created a new date instance. We can actually, let's do that.
[13:05] Let's go to the terminal, or no wait, let's open up your browser.
[13:12] Should have done this from the beginning, I apologize. >> Browser.
[13:19] >> Cool. Could you open up the console? I don't know how to do that from here.
[13:28] >> Like what page? >> Any page.
[13:32] >> Oh, okay. I guess we'll go to Twitter. >> Twitter is a good call.
[13:38] >> That's always my default. [LAUGHTER]
[13:42] >> Let's open up the console. Now, what do we have here?
[13:47] We have a JavaScript playground we can play with. Could you do me a favor and make it slightly bigger?
[13:54] I think it's like shift command plus. Nice.
[14:00] >> Really big now. >> That's perfect. I see it very well. Thank you.
[14:06] What we can do here is essentially mess around with JavaScript. For example, we can do one plus
[14:13] one here at the bottom where the little blue. >> Oh, thank you.
[14:18] >> Chevron is one plus one. >> In this keyboard, I'm going to get used to it.
[14:26] Equals two. >> If you hit "Enter",
[14:29] it'll execute that JavaScript and show us what it returns. This expression, one plus one, gives us two.
[14:37] Let's try it the same with new date. >> Automatically filled that in. That's cool.
[14:50] >> Hit "Enter". What creating a new date does is gives us a date object. Immediately set to the time at which you executed that command.
[15:09] If you run it again, if you press "Up", you can press "Up" to do it.
[15:16] >> Yeah. There we go. >> Yeah. Let's hit "Enter".
[15:22] Now, notice the difference. The first time it was at 10.15.29 seconds,
[15:28] now it's at 10.15.55 seconds. That doesn't mean that it's constantly updating,
[15:34] but rather that that object has its seconds value set to the moment that you hit "Enter".
[15:40] Do it again at 16.14. >> That's fine.
[15:45] >> What we're doing is storing the current date, and date extends to time,
[15:50] which is a weird thing to say, but you know what I mean, right?
[15:54] >> Yeah. >> Cool. Thank you for going with me down this rabbit hole.
[15:58] Let's hop on back to VS Code. Great. We've got a posts set to "Lee loving these videos and date".
[16:08] Now, our- >> I want to add one more.
[16:13] >> Oh, yeah. Go for it. Don't forget the comma. >> Freaking commas. This is going to be platform,
[16:22] and we'll say "LinkedIn Live". >> Comma. I don't remember my commas.
[16:31] >> Yeah. Here's an interesting quirk about JavaScript. The last one doesn't require a comma,
[16:37] but it won't complain if you put it either. >> Okay. I'm glad for that.
[16:42] >> You can totally put them in. Nobody minds. >> All right. Go, go, gadget.
[16:49] Let's see if I can read today. I think I'm going to now.
[16:59] Is it groking or groking? >> I think it's groking.
[17:03] >> Groking, that opening up the browser and trying things out in the console, the JavaScript version of a Jupyter Notebook.
[17:14] >> Are you familiar with Jupyter? >> No. That just sounds cool.
[17:18] >> I think it's like, and I'm going to super get this wrong
[17:21] because I don't do a lot of Python myself. It's like a Python playground that you can write stuff in.
[17:30] It's like a living notebook. I could be totally wrong.
[17:35] >> Yes. I eventually want to get to Python once I learn enough about JavaScript.
[17:45] Yeah, you got it right. >> Nice.
[17:49] >> Go, go, gadget. You'll have to come on or hang out with us when we get
[17:53] to Python. >> I have it on good authority that
[17:56] go, go, gadget would be an excellent guest. No pressure to them.
[18:02] >> That's what I have to remember. Yay. >> Awesome. Right. Back here.
[18:13] Let's define our first proper for our API. Let's keep the lines 9-12.
[18:22] That'll be our hello world. Let's add a new endpoint.
[18:28] That'll be a get request like before. We can put it either before or after the one we currently have.
[18:35] Your call, where we put it. >> We can put it on line 17?
[18:43] >> It does have to be before the listen. >> Line 13.
[18:49] >> For example. >> Okay. It would be app.get.
[18:55] >> We're going to create a get endpoint for getting all of our posts.
[19:02] The string? >> The string would be called posts?
[19:11] >> Yes. >> No.
[19:12] >> Yes. >> But this is what it shows, so it can be cap.
[19:19] That's not quite right. If you've worked, no, you're good.
[19:24] Now, we're finally doing some API design, which I'm quite excited about.
[19:31] If you've worked with APIs, you'll need what's called a path.
[19:37] I don't know, api.github.com/users/repositories. We want to get slash posts.
[19:50] Forward slash. Exactly. We'll be able to try this out.
[20:01] We'll need our function to, yeah, that will look pretty much mostly the same.
[20:09] >> I can't see it, is it? Then do an squiggly?
[20:24] >> Yes. I like the term squiggly. It's good. >> It helps me know which ones people are talking about.
[20:32] >> Totally. Let's now response.send our post. >> Posts?
[20:49] >> Let's try it out. >> Is it a stream or?
[20:54] >> Great question. We're going to be responding with our array of posts.
[21:00] The way you're doing it now, perfect. Now, let's fire up our server and don't forget to save.
[21:13] Somebody recently told me there's a way to get VS Code to autosave, which is quite cool.
[21:21] >> That's fancy. >> If you're like me and you forget to save all the time,
[21:27] which I do a lot. Let's refresh this.
[21:34] This gives us "Yay, we're back." Why? Because we asked for the root path.
[21:40] But if we wanted to get the posts, yeah. This looks good.
[21:48] This is giving us text. >> Right.
[21:52] >> Which we don't quite want. Because what we want to do instead is respond with
[22:03] this data in such a way so that other apps can understand what it is that we're receiving.
[22:09] What does that mean? When, for example, let's say you've got a mobile app.
[22:21] This is a lie, by the way, there's no phone in here. My phone is currently my webcam.
[22:27] Anyway, completely irrelevant. Let's say your phone is interacting with,
[22:35] say you're logged into Twitter on your phone. What you're doing is having
[22:46] your phone app send a request to the server, asking for my latest tweets, right?
[22:54] The app, the server will tell the app, "Hey, this is how I formatted the response,
[23:04] the data," because there are different formats for this kind of data.
[23:09] I don't think we talked about XML. Or do I seem to remember us talking about XML?
[23:16] Do I seem to remember you and Anthony covering RSS feeds? >> We talked about it,
[23:24] but we didn't create one. >> Right. I thought I remembered that.
[23:31] Most RSS feeds are written in a format called XML. >> Right.
[23:37] >> No idea what it is. >> Isn't XML also like CSV?
[23:47] >> CSV is a text-formatting data standard, a format that is different from XML.
[24:04] XML is formatted as a bunch of HTML-like tags. >> Okay.
[24:13] >> Where CSV, as the name says, is comma-separated values.
[24:18] >> Real quick, GoGoGadget, you can add those as many as you want.
[24:23] I'm copying and pasting them and saving them to when we're done today,
[24:28] so I can set all that up. Thank you. >> Yeah. Thank you for sharing.
[24:35] XML, CSV, there's a third one that you've actually worked with called JSON.
[24:46] >> Oh, yeah. We talked about that last time. >> Yeah. In fact, we have a JSON file in our project.
[24:54] Do you remember which one? >> The one that's called .JSON?
[24:58] >> Yes. >> Well, technically, we have two,
[25:02] but it's the package.JSON. >> The reason this looks like a JavaScript object is
[25:08] because it pretty much is. JSON is short for JavaScript Object Notation.
[25:15] This is a way of storing data that looks like JavaScript objects.
[25:26] It's like, I don't want to call it de facto, but it is one of
[25:31] the most widely used ones in modern web development. If you're doing stuff in JSON,
[25:37] you're pretty good to go. But what does that mean for us?
[25:40] It means we need to format our posts to be in JSON. >> Really quick.
[25:46] I don't know if I remember asking you this time, what is the difference between JSON and YAML?
[25:52] >> Formatting. Do you have a YAML file there? >> No. I'm just thinking
[26:04] about because a lot of it is comparing it to things that I know about.
[26:09] >> Sure. >> Then when I worked at Stoplight,
[26:14] the option for some of it was a JSON file or a YAML file. That's where I'm going with it.
[26:21] Not that it necessarily needs to be talked about right now. >> No, you're totally good. That is an excellent because I would
[26:27] argue that YAML and JSON and XML are pretty equivalent in functionality, storing data.
[26:35] >> Right. You write data. Instead of having the curly brackets and name,
[26:42] well, there are colons in YAML. But yeah, it's just formatting.
[26:46] >> Cool. Thank you. >> Gogo Gadget very helpfully and
[26:50] kindly shared the difference between YAML and JSON. Thank you. Super handy.
[26:57] What I love about streaming is that folks are so helpful and send us links and stuff.
[27:03] >> It is here. I do want to point it out and I'll make sure it's in the comments,
[27:08] but I'm going to read it later. >> Awesome.
[27:13] >> Thank you, Gogo Gadget. >> Yeah, thank you.
[27:17] >> What? That is so cool. Gogo Gadget used to be a librarian.
[27:29] Oh my gosh, you're like one of my favorite people. I'm not the best at references.
[27:37] I get frustrated at Googling or looking for it. Thank you for joining today.
[27:43] >> You two need to team up. >> That would be fun.
[27:47] >> Full disclosure, I know Gogo Gadget. >> That's okay.
[27:52] >> Highly recommend. >> App.JS. What we're going to do is respond in JSON.
[28:02] Let's open up App.JS again. Let's toggle away the project because we don't need to see all of it.
[28:15] Yeah. Line 14, response.send. Here we're sending what's called a plain text response.
[28:26] Now, we're going to talk about HTTP. We talked about HTTP last time.
[28:31] We talked about different request types. What also is taking place here is we're also telling the recipient,
[28:44] "Hey, this is the kind of data that I'm responding with. This is the format that I'm responding in."
[28:50] This is a piece of text called a header. A response is like a document and it's got
[28:57] some headers to tell you what to expect from the data that you're getting. What you're essentially saying with the header is,
[29:04] "Hear ye, hear ye, I am a JSON response," or "I am a plain text response,"
[29:08] or "I am some other kind of response." Now, because Express is a very nice piece of tech,
[29:20] it actually gives us a shortcut to be able to do that. Let's replace send in line 14 with JSON.
[29:30] Let's save and restart. Now, you're
[29:57] probably looking at that and thinking, "Well, hello, Twitch."
[30:03] >> It went way too high. There we go. >> Now, you're probably looking at that and thinking, "Well,
[30:11] that's the same," and the reason it is, is because to the browser, it is.
[30:17] The browser got a string of JSON and said, "Well, I'll just display that string," whatever you say.
[30:24] >> Okay. >> But when we start using this API in, say,
[30:30] a mobile app or in some front-end development app, now it's going to be a lot clever and say, "Aha,
[30:37] we're dealing with JSON here," which is all well and good. But we still got stuff to do here.
[30:45] Let's make our lives easier. I don't know about you, but it's getting a bit cumbersome to
[30:56] restart the server every time we make a change. >> Yeah.
[31:05] >> Let's set up something called Node-Mon. I don't know how to pronounce it. Let's go back to
[31:14] the terminal, shut down our server, and we're going to install the NPM package Node-Mon,
[31:25] which is Node and then Mon. First, we need to NPM and then install,
[31:37] and then the name of the package, and then Node. >> Afterwards?
[31:46] >> No, it's one word. It's Node-Mon.
[31:50] Sorry, I described that badly. >> Node-Mon?
[31:55] >> Mon, M-O-N, the second half of my name. Yeah.
[32:00] >> Okay. There we go. >> I'll get there.
[32:03] >> No, you're good. >> Yay.
[32:06] >> Now I've installed something called Node-Mon. Do me a quick favor, please.
[32:11] Let's try running Node-Mon. Just write Node-Mon into your terminal.
[32:16] Let's see what happens. Good. That's fine. We've installed this tool called Node-Mon,
[32:26] which in turn installs an executable file. Let's go over to package.json.
[32:38] Actually, no, let's stay in the terminal for a sec. I'm sorry to take us on so many tangents,
[32:42] but I swear that you're going to love this. Let's type in ./node-modules.
[32:53] Don't forget, you can tap to auto-complete. There's an underscore in between.
[32:59] >> Then enter? >> No, not yet. .bin.
[33:06] Oh, no, no. Keep that slash. .bin, B-I-N. Sorry, the first one was right.
[33:18] .bin, forward slash, Node-Mon. Now, don't hit "Enter" just yet.
[33:26] What's going on here? When we install a package,
[33:30] it also installs all of the executable files, all the executable scripts into this .bin folder.
[33:38] We've got Node-Mon. Now we're going to pass, and now we're going to give it
[33:45] the name of the file that it should monitor. Let's put in space and then app.js.
[33:51] I have no idea if this is going to work, by the way. >> It knows that it's going to monitor this one because we're in
[33:59] the folder that app.js is in. >> Yeah. We're saying, "Hey, run and watch."
[34:10] Yeah. See? It's like, "Hey, I'm watching it." We can actually try it out.
[34:19] Gosh, I don't know. Let's change app.js real quick. Any change? >> Okay. Two seconds.
[34:28] >> Take your time. Let's add an enter between line 15 and 16, for example,
[34:35] because we're going to add a post request in a second. Save that. Now go back to your terminal.
[34:43] Look at that. Restarting due to changes. It started up node.js,
[34:47] node app.js again, which is cool. Now we'll never have to restart the server again.
[34:52] >> Oh, yay. That's fun. >> Actually, we can try it out. How about let's
[34:56] change "Yay, we're" back to "Yay, we're." >> Live.
[35:01] >> You read my mind. Save it. >> Yay.
[35:07] >> Refresh your browser. >> Too many things on one screen.
[35:12] >> Yes. >> Look at that. Now we don't refresh anymore.
[35:16] This is something that you do in a lot of projects. When you're in development mode,
[35:20] you don't want to be starting and shutting down your server all the time.
[35:23] Just use NodeMon, super handy. >> I need to install NodeMon in each project.
[35:32] If I wanted to go back into Anthony's with React, I would need to be in that folder too.
[35:38] >> I believe the project you created with React might have already set up NodeMon or an equivalent.
[35:47] >> Maybe. >> Most likely, yes.
[35:50] >> Okay, cool. >> Because that project is created from a template,
[35:55] and so the people who make this template anticipate what we're going to need.
[36:00] >> Okay. Got it. >> Okay. We got to get to the database part.
[36:12] Let's add another endpoint to our, yeah, which is going to be a post request.
[36:22] >> App.post? >> App.post.
[36:27] Now, this will be the same route. So it'll be posts.
[36:41] This is where things get a little weird, but we'll get there. Same function.
[36:47] >> Okay. >> Go to the bracket, "Enter".
[37:04] >> Now, for now, we're going to have this post request just add a new post,
[37:13] like with data that we're building in now. So do you know how to add a member to an array?
[37:24] >> No. >> So we've got access to our posts from line 3.
[37:29] So we're going to call posts.push. So this will push something new onto our array.
[37:44] Now, we need to give it a parameter, so smooth brackets,
[37:52] and we want to put in an object that represents a new post. That's curly brackets.
[38:00] So let's hit "Enter". Now, let's put in some generic data once again,
[38:07] the four same attributes. But let's make it distinguishable from the first one.
[38:18] So let's make it, well, let's just change it to whatever.
[38:23] >> I have one. >> Oh, you do? Nice.
[38:25] >> Yes. Hold on. I got to get their name.
[38:31] Oh, I forgot my comma. I forgot my comma.
[38:43] >> Don't forget the comma, yeah. >> If it's too long like that,
[38:59] do I just put it into one? >> I think you can do triple quote marks to do a multi-line string.
[39:09] >> Let's just- >> Or just put it all on one string.
[39:12] >> Yeah, I will. >> One line, pardon me.
[39:16] >> Put a space. >> That works.
[39:27] >> You capture space and it doesn't need to have a nice day. That's okay. All right. Then, I've got to put my comma all the way down here.
[39:41] No. There we go. Then dates, new dates, and that one, yeah.
[40:11] Yay, and save. >> Nice. You know what?
[40:17] Let's just so we can monitor on our terminal, let's put a console log, added new post.
[40:27] >> Oh, wait. >> No, you're good.
[40:32] >> Okay. Console dot log, right? >> Yep.
[40:39] >> Wait, would this be a string? >> Yep.
[40:46] >> Is that it? >> Perfect. Let's save that.
[40:57] Now, let's go back to our browser and go to slash posts. Now, we see here our JSON data of our single post.
[41:13] You're probably wondering, okay, but how do I post? Certainly can't do that with how we've been doing it so far.
[41:24] Why? That's because when you put an address in a location bar in a browser, it's sending off a get request because it wants to get data.
[41:36] To post data from a browser, most of the time what we do is fill in an HTML form.
[41:44] We could fill in an HTML form, but that would require creating an HTML file.
[41:51] My question to you, Jen, is do you want to quickly whip up an HTML file to send off that form,
[41:58] or should we be lazy and do it with a terminal command? >> Terminal command.
[42:04] >> Terminal command. Good. Now, the problem is you're currently running your server here,
[42:10] and I don't know about you, but I don't want to stop the server.
[42:12] It's doing its thing. >> Okay.
[42:14] >> Besides, we need to have it running so that we can send the post request. >> Okay.
[42:18] >> Let's open a tab. That would be command T, just like in a browser.
[42:24] >> Okay. >> Yeah. We've still got it running on tab 1,
[42:29] and now we can do stuff here. Now, we're going to be using a tool on the terminal used
[42:35] for sending HTTP requests called cURL. Let's hit "Enter" and see if it's installed on your computer.
[42:44] It is. Nice. By the way, I think it's short for,
[42:48] I don't know what the C is, but URL. You know URL, right?
[42:52] >> Yeah. >> Right.
[42:54] >> Cool. Let's cURL. cURL -X, this is to tell it,
[43:09] we're going to do this kind of HTTP request, so put in a space,
[43:14] and now in all caps, POST, space, and now we're going to put in the URL.
[43:25] That's http://localhost:3334/posts. Now, yeah, and that's it.
[43:49] It's doing a thing. No idea if this is going to work, by the way, as always.
[43:57] >> It is doing a thing. >> It is doing a thing.
[43:59] >> It's thinking. >> It's taking oddly long, I have to be honest.
[44:04] Let's go back to tab 1. Hey, it did do a thing.
[44:12] >> It added the new post. >> Well, then let's refresh here.
[44:15] >> Hey. >> There you go.
[44:18] >> It added it. That's exciting. >> What I'm confused about,
[44:23] go back to tab 2, it did add the new post,
[44:27] but this is still running. Do you know what I mean?
[44:32] >> Yeah. >> I think, well,
[44:37] if you hit "Control C", that's good, but I think the problem is that it
[44:41] thinks the process is still running. Here's what we're going to do.
[44:46] Let's return. Go back to your app.js. Between line 24 and 25, let's return.
[45:02] Sorry, just type in return. Save that. No idea if this is going to work,
[45:16] by the way, as always. Now, hit up, yeah, do it.
[45:22] Would you look at that? That's very odd. Let's see. I'm going to Google that real quick.
[45:30] Yeah, because it added a new post. Let's see. CurlPostRequestNotShowingResponse.
[45:39] Yeah. Express. Process in Express.js when content type is not mentioned.
[45:51] Body parser. I'm going to do that. I believe the problem is that in our curl request,
[46:04] reply empty from server. Did you do that or is that something it did automatically?
[46:08] >> No, I think I did it because I just changed the name to see if it would change.
[46:12] >> Yeah. Okay. >> It did update again,
[46:17] but when I saved it, it said empty reply from server.
[46:25] But it did update it because I changed the name to yo. >> There it is.
[46:31] >> I need to run it again and it freezes, but it added it back properly.
[46:39] >> Nice. Let's go back to our terminal and hit "Control C". You remember when I was talking about headers?
[46:49] We didn't specify a header for our request. Let's try adding one. Go back to our terminal, hit "Up".
[47:04] Now, move your cursor with your keyboard, like with the left arrow key,
[47:09] over to just after post, between post and HTTP.
[47:14] Now, I'm going to send you some stuff that we'll just cover. I'm going to send it to you on the private chat.
[47:24] >> Okay. >> Paste that in, please.
[47:27] It's long to have me spell out to you. >> Do we need spaces?
[47:40] >> You will need a space after the post. You see where it says post-h right now?
[47:45] >> Oh, yes. >> Nice. What we're saying here is, "Hey,
[47:53] to this post request, add this header." The header has this content,
[47:58] it's content type, and we're saying, "Hey, the request I'm sending to you is formatted in JSON."
[48:06] >> It added it again. >> Did we run it? Oh, and it didn't finish.
[48:14] Maybe I'm wrong. Hold on. >> But it's interesting that it added it twice.
[48:25] >> No, it didn't add it twice. You added it twice by running the request twice.
[48:30] Run it again and it'll add it again. >> Yeah, it did it again by running the request twice.
[48:37] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[48:43] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[48:49] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[48:55] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:01] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:06] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:12] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:18] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:23] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:29] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:35] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:40] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:46] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:52] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[49:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:02] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:08] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:13] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:18] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:24] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:29] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:35] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:40] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:46] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[50:56] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:01] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:07] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:12] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:17] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:22] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:38] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:43] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:49] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:54] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[51:59] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:04] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:10] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:20] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:26] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:32] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:37] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:42] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:48] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:53] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[52:59] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:04] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:26] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:31] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:36] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:41] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:46] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[53:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:08] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:14] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:19] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:25] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:31] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:36] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:41] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:47] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:53] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[54:58] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:08] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:13] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:19] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:24] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:30] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:35] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:40] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:46] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[55:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:28] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:34] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:40] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:46] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:52] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[56:59] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:04] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:10] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:16] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[57:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[58:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[59:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[60:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[61:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[62:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[63:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[64:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[65:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[66:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[67:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[68:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[69:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[70:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[71:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[72:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[73:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[74:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[75:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[76:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[77:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[78:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[79:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[80:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[81:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[82:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[83:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[84:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[85:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[86:57] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:03] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:09] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:15] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:21] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:27] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:33] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:39] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:45] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:51] >> Yeah, it did it again by running the request twice. >> Yeah, it did it again by running the request twice.
[87:57] >> Oh, actually, I'm really sorry. Before the, before line 29, sorry, in line 29, before the function?
[88:07] >> Yeah, yes. >> Let's put in async space.
[88:17] Perfect. Now we can -- >> It has a light bulb. Convert to arrow function.
[88:24] >> You can do it if you want. >> Which is just like this?
[88:30] >> Actually, you can let VSCode do it automatically and we can see the difference. >> Oh. Okay.
[88:40] >> You can undo that if you want because I seem to remember you preferring writing functions out. >> Yeah, but I think it'll be good to see that there's differences in it as I'm learning.
[88:51] >> Totally, totally. Okay. So let's have const posts lowercase. If it's a variable, it's lowercase.
[89:06] Post, capital P, the model, dot find. >> Model dot find?
[89:17] >> Oh, sorry, no, I meant the post model with a capital P. So post dot find. And then we'll put in our brackets.
[89:30] And inside that, an empty object. >> Which means nothing?
[89:37] >> It means curly brackets. >> I'm going to learn this stuff.
[89:42] >> It takes time. So what are we doing here? >> We're saying find all of the posts that meet these criteria.
[89:52] >> Okay. >> But we're not passing any criteria.
[89:56] If there's no criteria, it's just like, all right, then you get all the posts. >> Okay.
[90:02] >> We're done. I have no idea if this is going to work. I'm very excited.
[90:09] Oh, we got an error. Oh, my goodness, and I have no idea what that --
[90:15] >> It crashed. >> Yeah, it crashed real good.
[90:20] Let's look at that. Converting circular structure to JSON. Starting at object with constructor topology.
[90:31] S object with constructor object. It's doing something.
[90:48] Tell you what, let's add a -- let's go back to our app.js. And let's do a console log of console.log posts.
[91:05] Oh, my goodness, I'm so sorry. I know it's wrong. In line 30 --
[91:11] >> Did I forget a comma? >> I forgot a thing. Remember how we made this function async?
[91:17] >> Yes. >> In line 30, after the equals, we want to have a wait.
[91:25] >> Is the word wait? >> A wait. So it's like I am -- exactly. That's it.
[91:33] Because find is asynchronous. By doing it this way, we're telling it, no, no. You wait until it's done getting all the posts.
[91:45] Nice. Empty. Why is it empty? >> Because we didn't tell it what to find.
[91:51] >> It's because our database is empty. >> Oh. Yeah. Okay.
[91:57] >> Let's add a post. >> Okay. Which was what we did over here.
[92:07] >> Yep. >> I'm going to add this one.
[92:11] >> Yep. Let's take a look at the terminal first.
[92:19] >> I'm going to add a new post. >> All right. And it added it.
[92:26] >> Now, finishing touch. Let's turn off the server, turn it on, and see if it got persisted. >> So I'm just restarting the server, right?
[92:40] >> NPM start. >> I'm going to refresh this and see if it's still there.
[92:50] >> Yep. >> It's still there.
[92:54] >> Nice. >> But I'm also going to like double, double check it.
[92:59] Because it should come up in incognito. Yay! >> Of course. It absolutely should.
[93:04] So now, Jen, you've got yourself a quantified back-end app with a database connection. And if I want to add more, I --
[93:21] >> Oh. Yes. No, you totally can. Let's -- I don't know about you, but curl is nice, but it's kind of a pain in the butt. >> Okay.
[93:32] >> What a lot of devs do is they use something called Postman. I don't use it much myself, but we can totally use it if you want. It's an app for doing --
[93:40] >> Let's try that next time, because I think I can try doing this a bit the way it is. And I also want to see if I can build this myself with my notes.
[93:55] >> Totally. >> Or at least add more. And possibly pretty it up.
[94:04] >> Sure. We did a lot today. I don't even know how I would do that, but, yeah, between the last one and this one, I'm like, okay.
[94:15] >> Yeah. I commend you. I commend you, Jen. Listen, let me ask, before we wrap up for today, is there anything here that you're like, I absolutely have no idea what we did here?
[94:33] Any questions you might have? >> No. Maybe.
[94:45] If I added -- if I went through and looked up the HTML version to add a post, I could make this pretty. >> Oh, this?
[94:59] This here? >> This, would I just add a HTML insert for this?
[95:07] >> Ah. So you want to make this data look pretty, is what you're saying.
[95:13] >> Just like the dogs go on bananas. >> Take your time.
[95:20] It should be hours. It's already getting time.
[95:25] >> I know, and for that part, I'll go for anybody listening or watching. I don't know why she's barking.
[95:33] I think she's just like, mom, it's time to finish. I want -- she loves cuddles.
[95:38] So I think she's yelling at me for cuddles. Ma'am, ma'am, you've got to stay quiet for like a little bit longer.
[95:50] >> I can answer your question. I can answer your question.
[95:59] >> Aw. She wants a little bit of attention.
[96:07] Sorry, just to make sure I understand correctly. Right now, we're looking at the JSON.
[96:11] It's not pretty. It's kind of messy looking.
[96:15] So your question is, what can we do to make that nicer? >> Yes.
[96:19] >> So, I'm going to give you a little bit of time. >> No, no, no.
[96:26] You're totally good. So the thing is, this API is not meant to render the data, is it?
[96:32] >> Okay. Right.
[96:36] >> It's just meant to be a data -- is the term broker? I'm not sure.
[96:40] It's meant to serve the data. It's just like, hey, you want some data?
[96:44] Here it is. >> Got it.
[96:48] >> Okay. So it's just like, hey, you want some data?
[96:52] Here it is. >> Exactly.
[96:56] So if you had a React app that would be used to display the posts, then you would do an HTTP request to this back end and be like, get the posts, receive that JSON, and then render it in React. >> Okay.
[97:12] I get what you're saying. >> Yeah.
[97:16] >> So it's just like having a little program that serves the data and saves the data. In fact, let's do one more thing before we go.
[97:26] Let's do that same curl -- let's do the same get request, but in the terminal with curl. So let's do curl, space, HTTP, colon, forward slash, forward slash, local host, colon, 3334, slash posts.
[97:56] >> Enter? >> Yep.
[98:00] >> Got it. >> I just showed it.
[98:04] So it's literally just being like, hey, you want the JSON? I got you.
[98:08] >> Cool. This is definitely --
[98:12] >> It's up to you. >> Cool.
[98:16] That makes sense. It also makes a lot more sense, like, with the front end versus the back end and all of that too.
[98:22] >> It's exciting. We covered loads.
[98:26] Like, kudos, Jen. Like, thank you.
[98:30] >> Thank you. It's also -- I'm still at the moment where I'm like, okay.
[98:34] Like, I get it, but I don't get it yet. But I can see that I'm starting to get it because, like, I'm able to guess, like, what we're going to be doing next a lot easier.
[98:44] >> Totally. >> Okay.
[98:48] There's a lot. >> It is a lot.
[98:52] >> And I appreciate it. >> Oh, yeah.
[98:56] >> I think you need to, like, also have some time to let it settle. >> Yes.
[99:02] >> You know, mess around with it. >> That is something that I'm learning that I just need to, like --
[99:06] >> Yeah. >> Let it sit.
[99:10] >> You need to break it. >> I will.
[99:14] >> You got to break it. Like, I think as programmers, like, one of the misconceptions we give newcomers is that, oh, yeah, we never break anything when you have ten years of experience.
[99:24] This is a lie. We break stuff all the time.
[99:28] That's how you learn. >> I think that's also something that I keep trying to rebuild it from scratch, and it takes me forever, where I think if I just try to break it or edit it as it is, it's going to be a lot easier.
[99:38] >> Yeah. Error messages are your friend.
[99:42] >> Yes. Yes.
[99:46] All right. Well, thank you so much for coming on the show today, Ramon.
[99:50] >> Thank you so much for having me. I almost said today's show, which is like a U.S. thing, and I'm like, that's not what we're doing.
[99:56] >> I mix them up. I mix them up, which one the today's show is.
[100:00] I know of it, but I don't know who's on it. >> Neither do I.
[100:04] I never watch it anymore. Okay.
[100:08] Well, thank you once again. We definitely did go through a lot, and I feel like I'm going to be asking you back at some point.
[100:12] >> Awesome. Looking forward to it.
[100:16] >> Thank you. 
